# Comparing `tmp/PythonForWindows-0.6.5.tar.gz` & `tmp/PythonForWindows-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\hakril\Documents\projets\PythonForWindows\dist\tmpzguc7ukl\PythonForWindows-0.6.5.tar", last modified: Mon Sep 20 15:52:45 2021, max compression
+gzip compressed data, was "PythonForWindows-0.6.8.tar", last modified: Sun May 19 17:21:22 2024, max compression
```

## Comparing `PythonForWindows-0.6.5.tar` & `PythonForWindows-0.6.8.tar`

### file list

```diff
@@ -1,121 +1,125 @@
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/
--rw-rw-rw-   0        0        0        8 2018-06-24 19:03:34.000000 PythonForWindows-0.6.5/AUTHORS
--rw-rw-rw-   0        0        0     1516 2018-06-24 19:03:34.000000 PythonForWindows-0.6.5/LICENSE
--rw-rw-rw-   0        0        0    20699 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/PythonForWindows.egg-info/
--rw-rw-rw-   0        0        0        1 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/PythonForWindows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    20699 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/PythonForWindows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3063 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/PythonForWindows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/PythonForWindows.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    20195 2021-04-28 11:54:31.000000 PythonForWindows-0.6.5/README.md
--rw-rw-rw-   0        0        0       42 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1242 2021-09-20 15:49:48.000000 PythonForWindows-0.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/
--rw-rw-rw-   0        0        0    25032 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/alpc.py
--rw-rw-rw-   0        0        0    12783 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/com.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/crypto/
--rw-rw-rw-   0        0        0       93 2018-06-24 19:03:35.000000 PythonForWindows-0.6.5/windows/crypto/catalog.py
--rw-rw-rw-   0        0        0    22523 2021-07-28 11:47:56.000000 PythonForWindows-0.6.5/windows/crypto/certificate.py
--rw-rw-rw-   0        0        0     4825 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/crypto/cryptmsg.py
--rw-rw-rw-   0        0        0     1646 2021-06-15 13:38:35.000000 PythonForWindows-0.6.5/windows/crypto/dpapi.py
--rw-rw-rw-   0        0        0     4789 2021-06-04 11:08:11.000000 PythonForWindows-0.6.5/windows/crypto/encrypt_decrypt.py
--rw-rw-rw-   0        0        0     2338 2019-03-23 17:38:21.000000 PythonForWindows-0.6.5/windows/crypto/generation.py
--rw-rw-rw-   0        0        0     2944 2020-01-26 14:53:43.000000 PythonForWindows-0.6.5/windows/crypto/sign_verify.py
--rw-rw-rw-   0        0        0      443 2021-06-15 13:38:35.000000 PythonForWindows-0.6.5/windows/crypto/__init__.py
--rw-rw-rw-   0        0        0     1527 2018-06-24 19:03:35.000000 PythonForWindows-0.6.5/windows/dbgprint.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/debug/
--rw-rw-rw-   0        0        0     9952 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/debug/breakpoints.py
--rw-rw-rw-   0        0        0    53395 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/debug/debugger.py
--rw-rw-rw-   0        0        0    13131 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/debug/localdbg.py
--rw-rw-rw-   0        0        0     2042 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/debug/symboldbg.py
--rw-rw-rw-   0        0        0    28878 2021-06-21 08:47:20.000000 PythonForWindows-0.6.5/windows/debug/symbols.py
--rw-rw-rw-   0        0        0      176 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/debug/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/generated_def/
--rw-rw-rw-   0        0        0      665 2018-06-24 19:03:35.000000 PythonForWindows-0.6.5/windows/generated_def/auto_doc_tst.py
--rw-rw-rw-   0        0        0     2003 2021-09-10 10:58:01.000000 PythonForWindows-0.6.5/windows/generated_def/flag.py
--rw-rw-rw-   0        0        0   190579 2021-09-10 10:58:06.000000 PythonForWindows-0.6.5/windows/generated_def/interfaces.py
--rw-rw-rw-   0        0        0   492976 2021-09-10 10:58:07.000000 PythonForWindows-0.6.5/windows/generated_def/meta.py
--rw-rw-rw-   0        0        0   355335 2021-09-10 10:58:02.000000 PythonForWindows-0.6.5/windows/generated_def/ntstatus.py
--rw-rw-rw-   0        0        0   208325 2021-09-10 10:58:02.000000 PythonForWindows-0.6.5/windows/generated_def/windef.py
--rw-rw-rw-   0        0        0   570899 2021-09-10 10:58:04.000000 PythonForWindows-0.6.5/windows/generated_def/winerror.py
--rw-rw-rw-   0        0        0   282394 2021-09-10 10:58:07.000000 PythonForWindows-0.6.5/windows/generated_def/winfuncs.py
--rw-rw-rw-   0        0        0   478904 2021-09-10 10:58:05.000000 PythonForWindows-0.6.5/windows/generated_def/winstructs.py
--rw-rw-rw-   0        0        0     2063 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/generated_def/__init__.py
--rw-rw-rw-   0        0        0     4704 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/hooks.py
--rw-rw-rw-   0        0        0    19189 2021-08-24 15:14:29.000000 PythonForWindows-0.6.5/windows/injection.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/native_exec/
--rw-rw-rw-   0        0        0     4974 2018-06-24 19:03:35.000000 PythonForWindows-0.6.5/windows/native_exec/cpuid.py
--rw-rw-rw-   0        0        0    12465 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/native_exec/nativeutils.py
--rw-rw-rw-   0        0        0     2681 2021-08-04 13:19:24.000000 PythonForWindows-0.6.5/windows/native_exec/native_function.py
--rw-rw-rw-   0        0        0    47071 2021-05-24 13:16:33.000000 PythonForWindows-0.6.5/windows/native_exec/simple_x64.py
--rw-rw-rw-   0        0        0    40279 2021-08-24 13:00:56.000000 PythonForWindows-0.6.5/windows/native_exec/simple_x86.py
--rw-rw-rw-   0        0        0       79 2018-06-24 19:03:35.000000 PythonForWindows-0.6.5/windows/native_exec/__init__.py
--rw-rw-rw-   0        0        0    18194 2021-07-29 18:01:29.000000 PythonForWindows-0.6.5/windows/pe_parse.py
--rw-rw-rw-   0        0        0     4567 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/pipe.py
--rw-rw-rw-   0        0        0      802 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/pycompat.py
--rw-rw-rw-   0        0        0    18773 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/remotectypes.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/rpc/
--rw-rw-rw-   0        0        0     7936 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/rpc/client.py
--rw-rw-rw-   0        0        0     7945 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/rpc/epmapper.py
--rw-rw-rw-   0        0        0    19540 2021-09-10 11:03:00.000000 PythonForWindows-0.6.5/windows/rpc/ndr.py
--rw-rw-rw-   0        0        0      145 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/rpc/__init__.py
--rw-rw-rw-   0        0        0    36704 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/security.py
--rw-rw-rw-   0        0        0    15242 2021-09-07 15:55:32.000000 PythonForWindows-0.6.5/windows/syswow64.py
--rw-rw-rw-   0        0        0     1340 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/test.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/utils/
--rw-rw-rw-   0        0        0     4648 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/utils/improved_buffer.py
--rw-rw-rw-   0        0        0     4062 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/utils/pythonutils.py
--rw-rw-rw-   0        0        0    26125 2021-07-28 11:47:56.000000 PythonForWindows-0.6.5/windows/utils/winutils.py
--rw-rw-rw-   0        0        0       85 2020-01-26 15:03:03.000000 PythonForWindows-0.6.5/windows/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/winobject/
--rw-rw-rw-   0        0        0     6591 2018-06-24 19:03:35.000000 PythonForWindows-0.6.5/windows/winobject/apisetmap.py
--rw-rw-rw-   0        0        0     8016 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winobject/bits.py
--rw-rw-rw-   0        0        0    20159 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winobject/device_manager.py
--rw-rw-rw-   0        0        0    41856 2021-04-28 11:54:31.000000 PythonForWindows-0.6.5/windows/winobject/event_log.py
--rw-rw-rw-   0        0        0    17104 2021-06-18 15:31:09.000000 PythonForWindows-0.6.5/windows/winobject/event_trace.py
--rw-rw-rw-   0        0        0    12445 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winobject/exception.py
--rw-rw-rw-   0        0        0     2388 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winobject/file.py
--rw-rw-rw-   0        0        0     7893 2020-01-26 14:53:43.000000 PythonForWindows-0.6.5/windows/winobject/handle.py
--rw-rw-rw-   0        0        0    13322 2019-03-23 17:38:21.000000 PythonForWindows-0.6.5/windows/winobject/network.py
--rw-rw-rw-   0        0        0     8742 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winobject/object_manager.py
--rw-rw-rw-   0        0        0    57178 2021-09-01 15:51:04.000000 PythonForWindows-0.6.5/windows/winobject/process.py
--rw-rw-rw-   0        0        0    16982 2021-04-28 11:54:31.000000 PythonForWindows-0.6.5/windows/winobject/registry.py
--rw-rw-rw-   0        0        0     6789 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winobject/service.py
--rw-rw-rw-   0        0        0    19517 2021-06-22 16:18:17.000000 PythonForWindows-0.6.5/windows/winobject/system.py
--rw-rw-rw-   0        0        0     2207 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winobject/system_module.py
--rw-rw-rw-   0        0        0    16491 2021-06-25 15:32:43.000000 PythonForWindows-0.6.5/windows/winobject/task_scheduler.py
--rw-rw-rw-   0        0        0    27791 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winobject/token.py
--rw-rw-rw-   0        0        0     2846 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winobject/volume.py
--rw-rw-rw-   0        0        0    19161 2021-07-28 11:47:56.000000 PythonForWindows-0.6.5/windows/winobject/wmi.py
--rw-rw-rw-   0        0        0        0 2018-06-24 19:03:35.000000 PythonForWindows-0.6.5/windows/winobject/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/winproxy/
--rw-rw-rw-   0        0        0     4705 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winproxy/apiproxy.py
-drwxrwxrwx   0        0        0        0 2021-09-20 15:52:45.000000 PythonForWindows-0.6.5/windows/winproxy/apis/
--rw-rw-rw-   0        0        0    36551 2021-06-25 15:32:43.000000 PythonForWindows-0.6.5/windows/winproxy/apis/advapi32.py
--rw-rw-rw-   0        0        0     4631 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winproxy/apis/cfgmgr32.py
--rw-rw-rw-   0        0        0    12625 2021-06-15 13:38:35.000000 PythonForWindows-0.6.5/windows/winproxy/apis/crypt32.py
--rw-rw-rw-   0        0        0      477 2019-03-23 17:38:21.000000 PythonForWindows-0.6.5/windows/winproxy/apis/cryptui.py
--rw-rw-rw-   0        0        0     8703 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winproxy/apis/dbghelp.py
--rw-rw-rw-   0        0        0      990 2021-05-24 13:16:33.000000 PythonForWindows-0.6.5/windows/winproxy/apis/dnsapi.py
--rw-rw-rw-   0        0        0     1359 2021-05-24 13:16:33.000000 PythonForWindows-0.6.5/windows/winproxy/apis/iphlpapi.py
--rw-rw-rw-   0        0        0    34879 2021-07-28 11:44:13.000000 PythonForWindows-0.6.5/windows/winproxy/apis/kernel32.py
--rw-rw-rw-   0        0        0      946 2019-03-23 17:38:21.000000 PythonForWindows-0.6.5/windows/winproxy/apis/ktmw32.py
--rw-rw-rw-   0        0        0    21619 2021-09-10 10:58:39.000000 PythonForWindows-0.6.5/windows/winproxy/apis/ntdll.py
--rw-rw-rw-   0        0        0     1875 2020-01-26 14:53:43.000000 PythonForWindows-0.6.5/windows/winproxy/apis/ole32.py
--rw-rw-rw-   0        0        0      426 2019-03-23 17:38:21.000000 PythonForWindows-0.6.5/windows/winproxy/apis/oleacc.py
--rw-rw-rw-   0        0        0     2017 2019-03-23 17:38:21.000000 PythonForWindows-0.6.5/windows/winproxy/apis/psapi.py
--rw-rw-rw-   0        0        0     3255 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winproxy/apis/setupapi.py
--rw-rw-rw-   0        0        0     1067 2021-05-24 13:16:33.000000 PythonForWindows-0.6.5/windows/winproxy/apis/shell32.py
--rw-rw-rw-   0        0        0      852 2019-03-23 17:38:22.000000 PythonForWindows-0.6.5/windows/winproxy/apis/shlwapi.py
--rw-rw-rw-   0        0        0      509 2020-01-26 14:53:43.000000 PythonForWindows-0.6.5/windows/winproxy/apis/tdh.py
--rw-rw-rw-   0        0        0     3877 2020-01-26 14:53:43.000000 PythonForWindows-0.6.5/windows/winproxy/apis/user32.py
--rw-rw-rw-   0        0        0     2378 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winproxy/apis/version.py
--rw-rw-rw-   0        0        0      800 2020-01-26 14:53:43.000000 PythonForWindows-0.6.5/windows/winproxy/apis/virtdisk.py
--rw-rw-rw-   0        0        0     5162 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/winproxy/apis/wevtapi.py
--rw-rw-rw-   0        0        0     4853 2021-08-04 13:47:16.000000 PythonForWindows-0.6.5/windows/winproxy/apis/wininet.py
--rw-rw-rw-   0        0        0     2632 2019-03-23 17:38:22.000000 PythonForWindows-0.6.5/windows/winproxy/apis/wintrust.py
--rw-rw-rw-   0        0        0      543 2021-08-04 13:47:56.000000 PythonForWindows-0.6.5/windows/winproxy/apis/__init__.py
--rw-rw-rw-   0        0        0     2503 2020-01-26 14:53:43.000000 PythonForWindows-0.6.5/windows/winproxy/error.py
--rw-rw-rw-   0        0        0      151 2020-01-26 14:53:43.000000 PythonForWindows-0.6.5/windows/winproxy/__init__.py
--rw-rw-rw-   0        0        0     6809 2020-08-06 08:37:51.000000 PythonForWindows-0.6.5/windows/wintrust.py
--rw-rw-rw-   0        0        0     1178 2021-04-28 11:54:31.000000 PythonForWindows-0.6.5/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.657541 PythonForWindows-0.6.8/
+-rw-rw-rw-   0        0        0        8 2018-06-24 19:03:34.000000 PythonForWindows-0.6.8/AUTHORS
+-rw-rw-rw-   0        0        0     1516 2018-06-24 19:03:34.000000 PythonForWindows-0.6.8/LICENSE
+-rw-rw-rw-   0        0        0    21138 2024-05-19 17:21:22.653532 PythonForWindows-0.6.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.483784 PythonForWindows-0.6.8/PythonForWindows.egg-info/
+-rw-rw-rw-   0        0        0    21138 2024-05-19 17:21:22.000000 PythonForWindows-0.6.8/PythonForWindows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3196 2024-05-19 17:21:22.000000 PythonForWindows-0.6.8/PythonForWindows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 17:21:22.000000 PythonForWindows-0.6.8/PythonForWindows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 17:21:22.000000 PythonForWindows-0.6.8/PythonForWindows.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    20655 2024-05-19 17:04:30.000000 PythonForWindows-0.6.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 17:21:22.657541 PythonForWindows-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-05-26 07:30:28.000000 PythonForWindows-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.531008 PythonForWindows-0.6.8/windows/
+-rw-rw-rw-   0        0        0     1178 2021-04-28 11:54:31.000000 PythonForWindows-0.6.8/windows/__init__.py
+-rw-rw-rw-   0        0        0    24953 2022-04-21 08:21:48.000000 PythonForWindows-0.6.8/windows/alpc.py
+-rw-rw-rw-   0        0        0    12783 2024-05-19 17:17:04.000000 PythonForWindows-0.6.8/windows/com.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.544570 PythonForWindows-0.6.8/windows/crypto/
+-rw-rw-rw-   0        0        0      443 2021-06-15 13:38:35.000000 PythonForWindows-0.6.8/windows/crypto/__init__.py
+-rw-rw-rw-   0        0        0       93 2018-06-24 19:03:35.000000 PythonForWindows-0.6.8/windows/crypto/catalog.py
+-rw-rw-rw-   0        0        0    22516 2024-05-19 17:17:04.000000 PythonForWindows-0.6.8/windows/crypto/certificate.py
+-rw-rw-rw-   0        0        0     4825 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/crypto/cryptmsg.py
+-rw-rw-rw-   0        0        0     1646 2021-06-15 13:38:35.000000 PythonForWindows-0.6.8/windows/crypto/dpapi.py
+-rw-rw-rw-   0        0        0     4789 2021-06-04 11:08:11.000000 PythonForWindows-0.6.8/windows/crypto/encrypt_decrypt.py
+-rw-rw-rw-   0        0        0     2338 2019-03-23 17:38:21.000000 PythonForWindows-0.6.8/windows/crypto/generation.py
+-rw-rw-rw-   0        0        0     2944 2020-01-26 14:53:43.000000 PythonForWindows-0.6.8/windows/crypto/sign_verify.py
+-rw-rw-rw-   0        0        0     1527 2024-05-18 20:46:46.000000 PythonForWindows-0.6.8/windows/dbgprint.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.553471 PythonForWindows-0.6.8/windows/debug/
+-rw-rw-rw-   0        0        0      176 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/debug/__init__.py
+-rw-rw-rw-   0        0        0     9952 2024-05-18 12:38:24.000000 PythonForWindows-0.6.8/windows/debug/breakpoints.py
+-rw-rw-rw-   0        0        0    53395 2024-05-18 21:30:10.000000 PythonForWindows-0.6.8/windows/debug/debugger.py
+-rw-rw-rw-   0        0        0    13131 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/debug/localdbg.py
+-rw-rw-rw-   0        0        0     2042 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/debug/symboldbg.py
+-rw-rw-rw-   0        0        0    28878 2021-06-21 08:47:20.000000 PythonForWindows-0.6.8/windows/debug/symbols.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.569553 PythonForWindows-0.6.8/windows/generated_def/
+-rw-rw-rw-   0        0        0     2311 2024-05-13 21:02:42.000000 PythonForWindows-0.6.8/windows/generated_def/__init__.py
+-rw-rw-rw-   0        0        0      665 2018-06-24 19:03:35.000000 PythonForWindows-0.6.8/windows/generated_def/auto_doc_tst.py
+-rw-rw-rw-   0        0        0     2003 2024-05-18 20:15:58.000000 PythonForWindows-0.6.8/windows/generated_def/flag.py
+-rw-rw-rw-   0        0        0   191665 2024-05-18 20:16:00.000000 PythonForWindows-0.6.8/windows/generated_def/interfaces.py
+-rw-rw-rw-   0        0        0   511039 2024-05-18 20:16:00.000000 PythonForWindows-0.6.8/windows/generated_def/meta.py
+-rw-rw-rw-   0        0        0   355335 2024-05-18 20:15:58.000000 PythonForWindows-0.6.8/windows/generated_def/ntstatus.py
+-rw-rw-rw-   0        0        0   238350 2024-05-18 20:15:58.000000 PythonForWindows-0.6.8/windows/generated_def/windef.py
+-rw-rw-rw-   0        0        0   570899 2024-05-18 20:15:59.000000 PythonForWindows-0.6.8/windows/generated_def/winerror.py
+-rw-rw-rw-   0        0        0   309229 2024-05-18 20:16:00.000000 PythonForWindows-0.6.8/windows/generated_def/winfuncs.py
+-rw-rw-rw-   0        0        0   501674 2024-05-18 21:30:17.000000 PythonForWindows-0.6.8/windows/generated_def/winstructs.py
+-rw-rw-rw-   0        0        0     4704 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/hooks.py
+-rw-rw-rw-   0        0        0    19193 2024-05-14 16:56:12.000000 PythonForWindows-0.6.8/windows/injection.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.578081 PythonForWindows-0.6.8/windows/native_exec/
+-rw-rw-rw-   0        0        0       79 2018-06-24 19:03:35.000000 PythonForWindows-0.6.8/windows/native_exec/__init__.py
+-rw-rw-rw-   0        0        0     4974 2018-06-24 19:03:35.000000 PythonForWindows-0.6.8/windows/native_exec/cpuid.py
+-rw-rw-rw-   0        0        0     2681 2022-04-21 08:21:48.000000 PythonForWindows-0.6.8/windows/native_exec/native_function.py
+-rw-rw-rw-   0        0        0    12465 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/native_exec/nativeutils.py
+-rw-rw-rw-   0        0        0    47071 2021-05-24 13:16:33.000000 PythonForWindows-0.6.8/windows/native_exec/simple_x64.py
+-rw-rw-rw-   0        0        0    40279 2021-08-24 13:00:56.000000 PythonForWindows-0.6.8/windows/native_exec/simple_x86.py
+-rw-rw-rw-   0        0        0    18194 2022-04-21 08:21:48.000000 PythonForWindows-0.6.8/windows/pe_parse.py
+-rw-rw-rw-   0        0        0     4567 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/pipe.py
+-rw-rw-rw-   0        0        0      802 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/pycompat.py
+-rw-rw-rw-   0        0        0    18773 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/remotectypes.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.582622 PythonForWindows-0.6.8/windows/rpc/
+-rw-rw-rw-   0        0        0      145 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/rpc/__init__.py
+-rw-rw-rw-   0        0        0     7936 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/rpc/client.py
+-rw-rw-rw-   0        0        0     7945 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/rpc/epmapper.py
+-rw-rw-rw-   0        0        0    19540 2024-05-14 17:01:50.000000 PythonForWindows-0.6.8/windows/rpc/ndr.py
+-rw-rw-rw-   0        0        0    40320 2024-05-13 21:02:42.000000 PythonForWindows-0.6.8/windows/security.py
+-rw-rw-rw-   0        0        0    15242 2021-09-07 15:55:32.000000 PythonForWindows-0.6.8/windows/syswow64.py
+-rw-rw-rw-   0        0        0     1340 2024-05-19 17:17:04.000000 PythonForWindows-0.6.8/windows/test.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.588648 PythonForWindows-0.6.8/windows/utils/
+-rw-rw-rw-   0        0        0       85 2020-01-26 15:03:03.000000 PythonForWindows-0.6.8/windows/utils/__init__.py
+-rw-rw-rw-   0        0        0     4648 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/utils/improved_buffer.py
+-rw-rw-rw-   0        0        0     4062 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/utils/pythonutils.py
+-rw-rw-rw-   0        0        0    25849 2024-05-19 17:17:04.000000 PythonForWindows-0.6.8/windows/utils/winutils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.613828 PythonForWindows-0.6.8/windows/winobject/
+-rw-rw-rw-   0        0        0        0 2018-06-24 19:03:35.000000 PythonForWindows-0.6.8/windows/winobject/__init__.py
+-rw-rw-rw-   0        0        0     6591 2018-06-24 19:03:35.000000 PythonForWindows-0.6.8/windows/winobject/apisetmap.py
+-rw-rw-rw-   0        0        0     8016 2024-05-19 17:17:04.000000 PythonForWindows-0.6.8/windows/winobject/bits.py
+-rw-rw-rw-   0        0        0    20159 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winobject/device_manager.py
+-rw-rw-rw-   0        0        0    41990 2024-05-19 17:17:04.000000 PythonForWindows-0.6.8/windows/winobject/event_log.py
+-rw-rw-rw-   0        0        0    17104 2021-06-18 15:31:09.000000 PythonForWindows-0.6.8/windows/winobject/event_trace.py
+-rw-rw-rw-   0        0        0    12445 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winobject/exception.py
+-rw-rw-rw-   0        0        0     2388 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winobject/file.py
+-rw-rw-rw-   0        0        0     8022 2022-04-21 08:21:48.000000 PythonForWindows-0.6.8/windows/winobject/handle.py
+-rw-rw-rw-   0        0        0    13322 2019-03-23 17:38:21.000000 PythonForWindows-0.6.8/windows/winobject/network.py
+-rw-rw-rw-   0        0        0     8742 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winobject/object_manager.py
+-rw-rw-rw-   0        0        0    58224 2024-05-14 16:56:12.000000 PythonForWindows-0.6.8/windows/winobject/process.py
+-rw-rw-rw-   0        0        0    16982 2024-05-19 17:17:04.000000 PythonForWindows-0.6.8/windows/winobject/registry.py
+-rw-rw-rw-   0        0        0     6790 2024-05-13 21:02:42.000000 PythonForWindows-0.6.8/windows/winobject/service.py
+-rw-rw-rw-   0        0        0    22298 2024-05-13 21:02:42.000000 PythonForWindows-0.6.8/windows/winobject/system.py
+-rw-rw-rw-   0        0        0     2207 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winobject/system_module.py
+-rw-rw-rw-   0        0        0    16491 2021-06-25 15:32:43.000000 PythonForWindows-0.6.8/windows/winobject/task_scheduler.py
+-rw-rw-rw-   0        0        0    27967 2022-05-09 15:41:01.000000 PythonForWindows-0.6.8/windows/winobject/token.py
+-rw-rw-rw-   0        0        0     2846 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winobject/volume.py
+-rw-rw-rw-   0        0        0    18622 2024-05-19 17:17:04.000000 PythonForWindows-0.6.8/windows/winobject/wmi.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.619878 PythonForWindows-0.6.8/windows/winproxy/
+-rw-rw-rw-   0        0        0      151 2020-01-26 14:53:43.000000 PythonForWindows-0.6.8/windows/winproxy/__init__.py
+-rw-rw-rw-   0        0        0     4705 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winproxy/apiproxy.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:21:22.653532 PythonForWindows-0.6.8/windows/winproxy/apis/
+-rw-rw-rw-   0        0        0      640 2024-05-13 21:02:42.000000 PythonForWindows-0.6.8/windows/winproxy/apis/__init__.py
+-rw-rw-rw-   0        0        0    38269 2022-08-05 10:46:15.000000 PythonForWindows-0.6.8/windows/winproxy/apis/advapi32.py
+-rw-rw-rw-   0        0        0     4631 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winproxy/apis/cfgmgr32.py
+-rw-rw-rw-   0        0        0    12625 2021-06-15 13:38:35.000000 PythonForWindows-0.6.8/windows/winproxy/apis/crypt32.py
+-rw-rw-rw-   0        0        0      477 2019-03-23 17:38:21.000000 PythonForWindows-0.6.8/windows/winproxy/apis/cryptui.py
+-rw-rw-rw-   0        0        0     8703 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winproxy/apis/dbghelp.py
+-rw-rw-rw-   0        0        0     1186 2022-04-21 08:21:48.000000 PythonForWindows-0.6.8/windows/winproxy/apis/dnsapi.py
+-rw-rw-rw-   0        0        0     1663 2022-08-05 10:46:15.000000 PythonForWindows-0.6.8/windows/winproxy/apis/iphlpapi.py
+-rw-rw-rw-   0        0        0    38824 2024-05-13 21:02:42.000000 PythonForWindows-0.6.8/windows/winproxy/apis/kernel32.py
+-rw-rw-rw-   0        0        0      946 2019-03-23 17:38:21.000000 PythonForWindows-0.6.8/windows/winproxy/apis/ktmw32.py
+-rw-rw-rw-   0        0        0     3046 2024-05-13 21:02:42.000000 PythonForWindows-0.6.8/windows/winproxy/apis/netapi32.py
+-rw-rw-rw-   0        0        0    21772 2024-05-13 21:02:42.000000 PythonForWindows-0.6.8/windows/winproxy/apis/ntdll.py
+-rw-rw-rw-   0        0        0     1875 2020-01-26 14:53:43.000000 PythonForWindows-0.6.8/windows/winproxy/apis/ole32.py
+-rw-rw-rw-   0        0        0      426 2019-03-23 17:38:21.000000 PythonForWindows-0.6.8/windows/winproxy/apis/oleacc.py
+-rw-rw-rw-   0        0        0     1234 2022-08-05 10:46:15.000000 PythonForWindows-0.6.8/windows/winproxy/apis/oleaut32.py
+-rw-rw-rw-   0        0        0     2017 2019-03-23 17:38:21.000000 PythonForWindows-0.6.8/windows/winproxy/apis/psapi.py
+-rw-rw-rw-   0        0        0     3255 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winproxy/apis/setupapi.py
+-rw-rw-rw-   0        0        0     1067 2021-05-24 13:16:33.000000 PythonForWindows-0.6.8/windows/winproxy/apis/shell32.py
+-rw-rw-rw-   0        0        0      852 2019-03-23 17:38:22.000000 PythonForWindows-0.6.8/windows/winproxy/apis/shlwapi.py
+-rw-rw-rw-   0        0        0      509 2020-01-26 14:53:43.000000 PythonForWindows-0.6.8/windows/winproxy/apis/tdh.py
+-rw-rw-rw-   0        0        0     3877 2020-01-26 14:53:43.000000 PythonForWindows-0.6.8/windows/winproxy/apis/user32.py
+-rw-rw-rw-   0        0        0     2378 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winproxy/apis/version.py
+-rw-rw-rw-   0        0        0      800 2020-01-26 14:53:43.000000 PythonForWindows-0.6.8/windows/winproxy/apis/virtdisk.py
+-rw-rw-rw-   0        0        0     5162 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/winproxy/apis/wevtapi.py
+-rw-rw-rw-   0        0        0     2296 2022-04-21 08:21:48.000000 PythonForWindows-0.6.8/windows/winproxy/apis/winhttp.py
+-rw-rw-rw-   0        0        0     4853 2022-04-21 08:21:48.000000 PythonForWindows-0.6.8/windows/winproxy/apis/wininet.py
+-rw-rw-rw-   0        0        0     2632 2019-03-23 17:38:22.000000 PythonForWindows-0.6.8/windows/winproxy/apis/wintrust.py
+-rw-rw-rw-   0        0        0     2684 2024-05-13 21:02:42.000000 PythonForWindows-0.6.8/windows/winproxy/apis/ws2_32.py
+-rw-rw-rw-   0        0        0     2503 2020-01-26 14:53:43.000000 PythonForWindows-0.6.8/windows/winproxy/error.py
+-rw-rw-rw-   0        0        0     6809 2020-08-06 08:37:51.000000 PythonForWindows-0.6.8/windows/wintrust.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PythonForWindows-0.6.5/LICENSE` & `PythonForWindows-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/PKG-INFO` & `PythonForWindows-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: PythonForWindows
-Version: 0.6.5
+Version: 0.6.8
 Summary: A codebase aimed to make interaction with Windows and native execution easier
 Home-page: https://github.com/hakril/PythonForWindows
 Author: Hakril
 Author-email: pfw@hakril.net
 License: BSD
 Keywords: windows python
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # PythonForWindows
 
 [![Join the chat at https://gitter.im/PythonForWindows/general](https://badges.gitter.im/PythonForWindows/general.svg)](https://gitter.im/PythonForWindows/general)
+[![Pytest](https://github.com/hakril/PythonForWindows/actions/workflows/mypytest.yml/badge.svg?branch=master)](https://github.com/hakril/PythonForWindows/actions/workflows/mypytest.yml)
 
 PythonForWindows (PFW) is a base of code aimed to make interaction with `Windows` (on X86/X64) easier (for both 32 and 64 bits Python).
 Its goal is to offer abstractions around some of the OS features in a (I hope) pythonic way.
 It also tries to make the barrier between python and native execution thinner in both ways.
 There is no external dependencies but it relies heavily on the `ctypes` module.
 
 
@@ -49,17 +49,18 @@
 
 ``
 python setup.py install
 ``
 
 #### Python3
 
-python3 support is still in beta.
-All the tests pass on master, but I did not test it heavily on real case.
-Do not hesitate report bugs and issues.
+PythonForWindows support python3 and is currently tested for Python2.7, 3.6 & 3.11 via [Github Workflow](https://github.com/hakril/PythonForWindows/actions/workflows/mypytest.yml)
+Regarding the handling of encoding in the project it's currently a mix of Ascii & Unicode that may be awkward on Python3 as automatic encoding/decoding is not present.
+
+The aim of passing the whole project under unicode is actvily ongoing.
 
 ## Overview
 
 ### Processes / Threads
 
 PythonForWindows offers objects around processes and allows you to:
 
@@ -558,8 +559,7 @@
 [LKD_GITHUB]: https://github.com/sogeti-esec-lab/LKD/
 [SAMPLE_DIR]: https://github.com/hakril/PythonForWindows/tree/master/samples
 [ONLINE_DOC]: http://hakril.github.io/PythonForWindows/
 [ONLINE_SAMPLE]: http://hakril.github.io/PythonForWindows/build/html/sample.html
 [ONLINE_SAMPLE_ALPC]: http://hakril.github.io/PythonForWindows/build/html/sample.html#windows-alpc
 [ONLINE_SAMPLE_RPC]: http://hakril.github.io/PythonForWindows/build/html/sample.html#windows-rpc
 [ONLINE_IATHOOK]: http://hakril.github.io/PythonForWindows/build/html/iat_hook.html
-
```

### Comparing `PythonForWindows-0.6.5/PythonForWindows.egg-info/PKG-INFO` & `PythonForWindows-0.6.8/PythonForWindows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: PythonForWindows
-Version: 0.6.5
+Version: 0.6.8
 Summary: A codebase aimed to make interaction with Windows and native execution easier
 Home-page: https://github.com/hakril/PythonForWindows
 Author: Hakril
 Author-email: pfw@hakril.net
 License: BSD
 Keywords: windows python
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # PythonForWindows
 
 [![Join the chat at https://gitter.im/PythonForWindows/general](https://badges.gitter.im/PythonForWindows/general.svg)](https://gitter.im/PythonForWindows/general)
+[![Pytest](https://github.com/hakril/PythonForWindows/actions/workflows/mypytest.yml/badge.svg?branch=master)](https://github.com/hakril/PythonForWindows/actions/workflows/mypytest.yml)
 
 PythonForWindows (PFW) is a base of code aimed to make interaction with `Windows` (on X86/X64) easier (for both 32 and 64 bits Python).
 Its goal is to offer abstractions around some of the OS features in a (I hope) pythonic way.
 It also tries to make the barrier between python and native execution thinner in both ways.
 There is no external dependencies but it relies heavily on the `ctypes` module.
 
 
@@ -49,17 +49,18 @@
 
 ``
 python setup.py install
 ``
 
 #### Python3
 
-python3 support is still in beta.
-All the tests pass on master, but I did not test it heavily on real case.
-Do not hesitate report bugs and issues.
+PythonForWindows support python3 and is currently tested for Python2.7, 3.6 & 3.11 via [Github Workflow](https://github.com/hakril/PythonForWindows/actions/workflows/mypytest.yml)
+Regarding the handling of encoding in the project it's currently a mix of Ascii & Unicode that may be awkward on Python3 as automatic encoding/decoding is not present.
+
+The aim of passing the whole project under unicode is actvily ongoing.
 
 ## Overview
 
 ### Processes / Threads
 
 PythonForWindows offers objects around processes and allows you to:
 
@@ -558,8 +559,7 @@
 [LKD_GITHUB]: https://github.com/sogeti-esec-lab/LKD/
 [SAMPLE_DIR]: https://github.com/hakril/PythonForWindows/tree/master/samples
 [ONLINE_DOC]: http://hakril.github.io/PythonForWindows/
 [ONLINE_SAMPLE]: http://hakril.github.io/PythonForWindows/build/html/sample.html
 [ONLINE_SAMPLE_ALPC]: http://hakril.github.io/PythonForWindows/build/html/sample.html#windows-alpc
 [ONLINE_SAMPLE_RPC]: http://hakril.github.io/PythonForWindows/build/html/sample.html#windows-rpc
 [ONLINE_IATHOOK]: http://hakril.github.io/PythonForWindows/build/html/iat_hook.html
-
```

### Comparing `PythonForWindows-0.6.5/PythonForWindows.egg-info/SOURCES.txt` & `PythonForWindows-0.6.8/PythonForWindows.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -87,21 +87,25 @@
 windows/winproxy/apis/crypt32.py
 windows/winproxy/apis/cryptui.py
 windows/winproxy/apis/dbghelp.py
 windows/winproxy/apis/dnsapi.py
 windows/winproxy/apis/iphlpapi.py
 windows/winproxy/apis/kernel32.py
 windows/winproxy/apis/ktmw32.py
+windows/winproxy/apis/netapi32.py
 windows/winproxy/apis/ntdll.py
 windows/winproxy/apis/ole32.py
 windows/winproxy/apis/oleacc.py
+windows/winproxy/apis/oleaut32.py
 windows/winproxy/apis/psapi.py
 windows/winproxy/apis/setupapi.py
 windows/winproxy/apis/shell32.py
 windows/winproxy/apis/shlwapi.py
 windows/winproxy/apis/tdh.py
 windows/winproxy/apis/user32.py
 windows/winproxy/apis/version.py
 windows/winproxy/apis/virtdisk.py
 windows/winproxy/apis/wevtapi.py
+windows/winproxy/apis/winhttp.py
 windows/winproxy/apis/wininet.py
-windows/winproxy/apis/wintrust.py
+windows/winproxy/apis/wintrust.py
+windows/winproxy/apis/ws2_32.py
```

### Comparing `PythonForWindows-0.6.5/README.md` & `PythonForWindows-0.6.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # PythonForWindows
 
 [![Join the chat at https://gitter.im/PythonForWindows/general](https://badges.gitter.im/PythonForWindows/general.svg)](https://gitter.im/PythonForWindows/general)
+[![Pytest](https://github.com/hakril/PythonForWindows/actions/workflows/mypytest.yml/badge.svg?branch=master)](https://github.com/hakril/PythonForWindows/actions/workflows/mypytest.yml)
 
 PythonForWindows (PFW) is a base of code aimed to make interaction with `Windows` (on X86/X64) easier (for both 32 and 64 bits Python).
 Its goal is to offer abstractions around some of the OS features in a (I hope) pythonic way.
 It also tries to make the barrier between python and native execution thinner in both ways.
 There is no external dependencies but it relies heavily on the `ctypes` module.
 
 
@@ -33,17 +34,18 @@
 
 ``
 python setup.py install
 ``
 
 #### Python3
 
-python3 support is still in beta.
-All the tests pass on master, but I did not test it heavily on real case.
-Do not hesitate report bugs and issues.
+PythonForWindows support python3 and is currently tested for Python2.7, 3.6 & 3.11 via [Github Workflow](https://github.com/hakril/PythonForWindows/actions/workflows/mypytest.yml)
+Regarding the handling of encoding in the project it's currently a mix of Ascii & Unicode that may be awkward on Python3 as automatic encoding/decoding is not present.
+
+The aim of passing the whole project under unicode is actvily ongoing.
 
 ## Overview
 
 ### Processes / Threads
 
 PythonForWindows offers objects around processes and allows you to:
```

### Comparing `PythonForWindows-0.6.5/setup.py` & `PythonForWindows-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿# -*- coding: utf-8 -*-
 import sys
 import os.path
 from setuptools import setup
 
 PKG_NAME = "PythonForWindows"
-VERSION  = "0.6.5"
+VERSION  = "0.6.8"
 
 # Load long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
```

### Comparing `PythonForWindows-0.6.5/windows/alpc.py` & `PythonForWindows-0.6.8/windows/alpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 # 0x1e: 0x40000000: ALPC_MESSAGE_VIEW_ATTRIBUTE(0x40000000): size=0x20
 # 0x1d: 0x20000000: ALPC_MESSAGE_CONTEXT_ATTRIBUTE(0x20000000): size=0x20
 # 0x1c: 0x10000000: ALPC_MESSAGE_HANDLE_ATTRIBUTE(0x10000000): size=0x18
 # 0x1b: 0x8000000: ALPC_MESSAGE_TOKEN_ATTRIBUTE(0x8000000): size=0x18
 # 0x1a: 0x4000000: ALPC_MESSAGE_DIRECT_ATTRIBUTE(0x4000000) size=0x8
 # 0x19: 0x2000000: ALPC_MESSAGE_WORK_ON_BEHALF_ATTRIBUTE(0x2000000) size=0x8
 
+DEFAULT_MESSAGE_SIZE = 0x1000
+
 class AlpcMessage(object):
     """Represent a full ALPC Message: a :class:`AlpcMessagePort` and a :class:`MessageAttribute`"""
     # PORT_MESSAGE + MessageAttribute
-    def __init__(self, msg_or_size=0x1000, attributes=None):
+    def __init__(self, msg_or_size=DEFAULT_MESSAGE_SIZE, attributes=None):
         # Init the PORT_MESSAGE
         if isinstance(msg_or_size, windows.pycompat.int_types):
             self.port_message_buffer_size = msg_or_size
             self.port_message_raw_buffer = ctypes.c_buffer(msg_or_size)
             self.port_message = AlpcMessagePort.from_buffer(self.port_message_raw_buffer)
             self.port_message.set_datalen(0)
         elif isinstance(msg_or_size, AlpcMessagePort):
@@ -156,14 +158,15 @@
         return cls.from_buffer(buffer)
 
     def read_data(self):
         return self.raw_buffer[ctypes.sizeof(self):ctypes.sizeof(self) + self.u1.s1.DataLength]
 
     def write_data(self, data):
         if len(data) > self.max_datasize:
+            import pdb; pdb.set_trace()
             raise ValueError("Cannot write data of len <{0}> (raw_buffer size == <{1}>)".format(len(data), self.buffer_size))
         self.raw_buffer[self.header_size: self.header_size + len(data)] = data
         self.set_datalen(len(data))
 
     data = property(read_data, write_data)
     "The data of the message (located after the header)"
 
@@ -300,60 +303,57 @@
             :type alpc_message: AlpcMessage or str
             :param receive_msg: The message to send. If ``receive_msg`` is a ``None`` it create and return a simple :class:`AlpcMessage`
             :type receive_msg: AlpcMessage or None
             :param int flags: The flags for :func:`NtAlpcSendWaitReceivePort`
         """
         if isinstance(alpc_message, windows.pycompat.anybuff):
             raw_alpc_message = alpc_message
-            if len(alpc_message) > 0x1000:
-                import pdb;pdb.set_trace()
             alpc_message = AlpcMessage(max(0x1000, len(alpc_message) + 0x200))
             alpc_message.port_message.data = raw_alpc_message
 
         if receive_msg is None:
-            receive_msg = AlpcMessage(0x1000)
+            receive_msg = AlpcMessage(DEFAULT_MESSAGE_SIZE)
         receive_size = gdef.SIZE_T(receive_msg.port_message_buffer_size)
         winproxy.NtAlpcSendWaitReceivePort(self.handle, flags, alpc_message.port_message, alpc_message.attributes, receive_msg.port_message, receive_size, receive_msg.attributes, timeout)
         return receive_msg
 
     def send(self, alpc_message, flags=0):
         """Send the ``alpc_message`` with ``flags``
 
             :param alpc_message: The message to send. If ``alpc_message`` is a :class:`str` it build an AlpcMessage with the message as data.
             :type alpc_message: AlpcMessage or str
             :param int flags: The flags for :func:`NtAlpcSendWaitReceivePort`
         """
         if isinstance(alpc_message, windows.pycompat.anybuff):
             raw_alpc_message = alpc_message
-            alpc_message = AlpcMessage(max(0x1000, len(alpc_message)))
+            alpc_message = AlpcMessage(max(0x1000, len(alpc_message) + 0x200))
             alpc_message.port_message.data = raw_alpc_message
         winproxy.NtAlpcSendWaitReceivePort(self.handle, flags, alpc_message.port_message, alpc_message.attributes, None, None, None, None)
 
     def recv(self, receive_msg=None, flags=0):
         """Receive a message into ``alpc_message`` with ``flags``.
 
             :param receive_msg: The message to send. If ``receive_msg`` is a ``None`` it create and return a simple :class:`AlpcMessage`
             :type receive_msg: AlpcMessage or None
             :param int flags: The flags for :func:`NtAlpcSendWaitReceivePort`
         """
         if receive_msg is None:
-            receive_msg = AlpcMessage(0x1000)
+            receive_msg = AlpcMessage(DEFAULT_MESSAGE_SIZE)
         receive_size = gdef.SIZE_T(receive_msg.port_message_buffer_size)
         winproxy.NtAlpcSendWaitReceivePort(self.handle, flags, None, None, receive_msg.port_message, receive_size, receive_msg.attributes, None)
         return receive_msg
 
     def _close_port(self, port_handle):
         windows.winproxy.NtAlpcDisconnectPort(port_handle, 0)
         windows.winproxy.CloseHandle(port_handle)
 
 
 
 class AlpcClient(AlpcTransportBase):
     "An ALPC client able to connect to a port and send/receive messages"
-    DEFAULT_MAX_MESSAGE_LENGTH = 0x9000
 
     def __init__(self, port_name=None):
         """Init the :class:`AlpcClient` automatically connect to ``port_name`` using default values if given"""
         self.handle = None
         self.port_name = None #: The name of the ALPC port the client is connect to.
         if port_name is not None:
             x = self.connect_to_port(port_name, "")
@@ -378,15 +378,15 @@
             raise ValueError("Client already connected")
         handle = gdef.HANDLE()
         port_name_unicode = self._alpc_port_to_unicode_string(port_name)
 
         if port_attr is None:
             port_attr = gdef.ALPC_PORT_ATTRIBUTES()
             port_attr.Flags = port_attr_flags # Flag qui fonctionne pour l'UAC
-            port_attr.MaxMessageLength = self.DEFAULT_MAX_MESSAGE_LENGTH
+            port_attr.MaxMessageLength = DEFAULT_MESSAGE_SIZE
             port_attr.MemoryBandwidth = 0
             port_attr.MaxPoolUsage = 0xffffffff
             port_attr.MaxSectionSize = 0xffffffff
             port_attr.MaxViewSize = 0xffffffff
             port_attr.MaxTotalSectionSize = 0xffffffff
             port_attr.DupObjectTypes = 0xffffffff
 
@@ -441,15 +441,14 @@
     def __del__(self):
         if sys.path is not None:
             self.disconnect()
 
 
 class AlpcServer(AlpcTransportBase):
     """An ALPC server able to create a port, accept connections and send/receive messages"""
-    DEFAULT_MAX_MESSAGE_LENGTH = 0x1000
 
     def __init__(self, port_name=None):
         self.port_name = None
         self.communication_port_list = []
         self.handle = None
         if port_name is not None:
             self.create_port(port_name)
@@ -470,15 +469,15 @@
         handle = gdef.HANDLE()
         raw_name =  port_name
         if not raw_name.startswith("\\"):
             raw_name = "\\" + port_name
         port_name = self._alpc_port_to_unicode_string(raw_name)
 
         if msglen is None:
-            msglen = self.DEFAULT_MAX_MESSAGE_LENGTH
+            msglen = DEFAULT_MESSAGE_SIZE
         if obj_attr is None:
             obj_attr = gdef.OBJECT_ATTRIBUTES()
             obj_attr.Length = ctypes.sizeof(obj_attr)
             obj_attr.RootDirectory = None
             obj_attr.ObjectName = ctypes.pointer(port_name)
             obj_attr.Attributes = 0
             obj_attr.SecurityDescriptor = None
@@ -513,15 +512,15 @@
         rhandle = gdef.HANDLE()
 
         if port_attr is None:
             port_attr = gdef.ALPC_PORT_ATTRIBUTES()
             port_attr.Flags = 0x80000
             # port_attr.Flags = 0x80000 + 0x2000000
             # port_attr.Flags =  0x2000000
-            port_attr.MaxMessageLength = self.DEFAULT_MAX_MESSAGE_LENGTH
+            port_attr.MaxMessageLength = DEFAULT_MESSAGE_SIZE
             port_attr.MemoryBandwidth = 0
             port_attr.MaxPoolUsage = 0xffffffff
             port_attr.MaxSectionSize = 0xffffffff
             port_attr.MaxViewSize = 0xffffffff
             port_attr.MaxTotalSectionSize = 0xffffffff
             port_attr.DupObjectTypes = 0xffffffff
         # windows.utils.print_ctypes_struct(port_attr, "   - CONN_PORT_ATTR", hexa=True)
```

### Comparing `PythonForWindows-0.6.5/windows/com.py` & `PythonForWindows-0.6.8/windows/com.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/crypto/certificate.py` & `PythonForWindows-0.6.8/windows/crypto/certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,30 +39,30 @@
 
     Current main use is extracting the signers certificates from a PE file.
     """
     MSG_PARAM_KNOW_TYPES = {gdef.CMSG_SIGNER_INFO_PARAM: gdef.CMSG_SIGNER_INFO,
                             gdef.CMSG_SIGNER_COUNT_PARAM: gdef.DWORD,
                             gdef.CMSG_CERT_COUNT_PARAM: gdef.DWORD}
 
-    def __init__(self, filename, content_type=gdef.CERT_QUERY_CONTENT_FLAG_ALL, x=0, tt=gdef.CERT_QUERY_OBJECT_FILE):
+    def __init__(self, filename, content_type=gdef.CERT_QUERY_CONTENT_FLAG_ALL):
         # No other API than filename for now..
         self.filename = filename
 
         dwEncoding    = gdef.DWORD()
         dwContentType = gdef.DWORD()
         dwFormatType  = gdef.DWORD()
         hStore        = CertificateStore()
         hMsg          = windows.crypto.CryptMessage()
 
-        winproxy.CryptQueryObject(tt,
+        winproxy.CryptQueryObject(gdef.CERT_QUERY_OBJECT_FILE,
             gdef.LPWSTR(filename),
             # filename,
             content_type,
-            gdef.CERT_QUERY_FORMAT_FLAG_BINARY, # CERT_QUERY_FORMAT_FLAG_ALL ?
-            x,
+            gdef.CERT_QUERY_FORMAT_FLAG_BINARY,
+            0,
             dwEncoding,
             dwContentType,
             dwFormatType,
             hStore,
             hMsg,
             None)
 
@@ -559,14 +559,15 @@
 
     def __init__(self, pszContainer=None, pszProvider=None, dwProvType=0, dwFlags=0, retrycreate=False):
         self.pszContainer = pszContainer
         self.pszProvider = pszProvider
         self.dwProvType = dwProvType
         self.dwFlags = dwFlags
         self.retrycreate = True
+        #self.value = HCRYPTPROV()
         pass
 
     def __enter__(self):
         self.acquire()
         return self
 
     def __exit__(self, *args):
```

### Comparing `PythonForWindows-0.6.5/windows/crypto/cryptmsg.py` & `PythonForWindows-0.6.8/windows/crypto/cryptmsg.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/crypto/dpapi.py` & `PythonForWindows-0.6.8/windows/crypto/dpapi.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/crypto/encrypt_decrypt.py` & `PythonForWindows-0.6.8/windows/crypto/encrypt_decrypt.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/crypto/generation.py` & `PythonForWindows-0.6.8/windows/crypto/generation.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/crypto/sign_verify.py` & `PythonForWindows-0.6.8/windows/crypto/sign_verify.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/dbgprint.py` & `PythonForWindows-0.6.8/windows/dbgprint.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/debug/breakpoints.py` & `PythonForWindows-0.6.8/windows/debug/breakpoints.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/debug/debugger.py` & `PythonForWindows-0.6.8/windows/debug/debugger.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/debug/localdbg.py` & `PythonForWindows-0.6.8/windows/debug/localdbg.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/debug/symboldbg.py` & `PythonForWindows-0.6.8/windows/debug/symboldbg.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/debug/symbols.py` & `PythonForWindows-0.6.8/windows/debug/symbols.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/generated_def/auto_doc_tst.py` & `PythonForWindows-0.6.8/windows/generated_def/auto_doc_tst.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/generated_def/flag.py` & `PythonForWindows-0.6.8/windows/generated_def/flag.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/generated_def/interfaces.py` & `PythonForWindows-0.6.8/windows/generated_def/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,14 +272,17 @@
 
 class IWbemLocator(COMInterface):
     IID = generate_IID(0xDC12A687, 0x737F, 0x11CF, 0x88, 0x4D, 0x00, 0xAA, 0x00, 0x4B, 0x2E, 0x24, name="IWbemLocator", strid="DC12A687-737F-11CF-884D-00AA004B2E24")
 
 class IWbemObjectSink(COMInterface):
     IID = generate_IID(0x7C857801, 0x7381, 0x11CF, 0x88, 0x4D, 0x00, 0xAA, 0x00, 0x4B, 0x2E, 0x24, name="IWbemObjectSink", strid="7C857801-7381-11CF-884D-00AA004B2E24")
 
+class IWbemObjectTextSrc(COMInterface):
+    IID = generate_IID(0xBFBF883A, 0xCAD7, 0x11D3, 0xA1, 0x1B, 0x00, 0x10, 0x5A, 0x1F, 0x51, 0x5A, name="IWbemObjectTextSrc", strid="BFBF883A-CAD7-11D3-A11B-00105A1F515A")
+
 class IWbemQualifierSet(COMInterface):
     IID = generate_IID(0xDC12A680, 0x737F, 0x11CF, 0x88, 0x4D, 0x00, 0xAA, 0x00, 0x4B, 0x2E, 0x24, name="IWbemQualifierSet", strid="DC12A680-737F-11CF-884D-00AA004B2E24")
 
 class IWbemServices(COMInterface):
     IID = generate_IID(0x9556DC99, 0x828C, 0x11CF, 0xA3, 0x7E, 0x00, 0xAA, 0x00, 0x32, 0x40, 0xC7, name="IWbemServices", strid="9556DC99-828C-11CF-A37E-00AA003240C7")
 
 ICallFrame._functions_ = {
@@ -2657,14 +2660,27 @@
         "Release": ctypes.WINFUNCTYPE(ULONG)(2, "Release"),
         # Indicate -> lObjectCount:LONG, apObjArray:**IWbemClassObject
         "Indicate": ctypes.WINFUNCTYPE(HRESULT, LONG, POINTER(IWbemClassObject))(3, "Indicate"),
         # SetStatus -> lFlags:LONG, hResult:HRESULT, strParam:BSTR, pObjParam:*IWbemClassObject
         "SetStatus": ctypes.WINFUNCTYPE(HRESULT, LONG, HRESULT, BSTR, IWbemClassObject)(4, "SetStatus"),
     }
 
+IWbemObjectTextSrc._functions_ = {
+        # QueryInterface -> riid:REFIID, ppvObject:**void
+        "QueryInterface": ctypes.WINFUNCTYPE(HRESULT, REFIID, POINTER(PVOID))(0, "QueryInterface"),
+        # AddRef -> 
+        "AddRef": ctypes.WINFUNCTYPE(ULONG)(1, "AddRef"),
+        # Release -> 
+        "Release": ctypes.WINFUNCTYPE(ULONG)(2, "Release"),
+        # GetText -> lFlags:LONG, pObj:*IWbemClassObject, uObjTextFormat:ULONG, pCtx:*IWbemContext, strText:*BSTR
+        "GetText": ctypes.WINFUNCTYPE(HRESULT, LONG, IWbemClassObject, ULONG, IWbemContext, POINTER(BSTR))(3, "GetText"),
+        # CreateFromText -> lFlags:LONG, strText:BSTR, uObjTextFormat:ULONG, pCtx:*IWbemContext, pNewObj:**IWbemClassObject
+        "CreateFromText": ctypes.WINFUNCTYPE(HRESULT, LONG, BSTR, ULONG, IWbemContext, POINTER(IWbemClassObject))(4, "CreateFromText"),
+    }
+
 IWbemQualifierSet._functions_ = {
         # QueryInterface -> riid:REFIID, ppvObject:**void
         "QueryInterface": ctypes.WINFUNCTYPE(HRESULT, REFIID, POINTER(PVOID))(0, "QueryInterface"),
         # AddRef -> 
         "AddRef": ctypes.WINFUNCTYPE(ULONG)(1, "AddRef"),
         # Release -> 
         "Release": ctypes.WINFUNCTYPE(ULONG)(2, "Release"),
```

### Comparing `PythonForWindows-0.6.5/windows/generated_def/meta.py` & `PythonForWindows-0.6.8/windows/generated_def/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
      'AF_IMPLINK',
      'AF_INET',
      'AF_INET6',
      'AF_IPX',
      'AF_IRDA',
      'AF_ISO',
      'AF_LAT',
+     'AF_MAX',
      'AF_NETBIOS',
      'AF_NETDES',
      'AF_NS',
      'AF_OSI',
      'AF_PUP',
      'AF_SNA',
      'AF_UNIX',
@@ -196,14 +197,15 @@
      'ATM_AESA',
      'ATM_E164',
      'ATM_NSAP',
      'ATTRIBUTE_SECURITY_INFORMATION',
      'AT_KEYEXCHANGE',
      'AT_SIGNATURE',
      'BACKUP_SECURITY_INFORMATION',
+     'BASE_PROTOCOL',
      'BASIC_LOG_CONF',
      'BELOW_NORMAL_PRIORITY_CLASS',
      'BG_JOB_ENUM_ALL_USERS',
      'BG_NOTIFY_DISABLE',
      'BG_NOTIFY_FILE_TRANSFERRED',
      'BG_NOTIFY_JOB_ERROR',
      'BG_NOTIFY_JOB_MODIFICATION',
@@ -822,21 +824,23 @@
      'DEBUG_EVENT_EXIT_THREAD',
      'DEBUG_EVENT_LOAD_MODULE',
      'DEBUG_EVENT_SESSION_STATUS',
      'DEBUG_EVENT_SYSTEM_ERROR',
      'DEBUG_EVENT_UNLOAD_MODULE',
      'DEBUG_ONLY_THIS_PROCESS',
      'DEBUG_PROCESS',
+     'DEFAULT_MINIMUM_ENTITIES',
      'DELETE',
      'DETACHED_PROCESS',
      'DIRECTORY_ALL_ACCESS',
      'DIRECTORY_CREATE_OBJECT',
      'DIRECTORY_CREATE_SUBDIRECTORY',
      'DIRECTORY_QUERY',
      'DIRECTORY_TRAVERSE',
+     'DNS_ADDR_MAX_SOCKADDR_LENGTH',
      'DNS_ATMA_FORMAT_AESA',
      'DNS_ATMA_FORMAT_E164',
      'DNS_ATMA_MAX_ADDR_LENGTH',
      'DNS_QUERY_ACCEPT_TRUNCATED_RESPONSE',
      'DNS_QUERY_ADDRCONFIG',
      'DNS_QUERY_APPEND_MULTILABEL',
      'DNS_QUERY_BYPASS_CACHE',
@@ -1160,18 +1164,24 @@
      'FAX_PORT_SET',
      'FC_ALLOCATE_ALL_NODES',
      'FC_ALLOCED_ON_STACK',
      'FC_DONT_FREE',
      'FC_POINTER_DEREF',
      'FC_SIMPLE_POINTER',
      'FILE_ACTION_ADDED',
+     'FILE_ACTION_ADDED_STREAM',
+     'FILE_ACTION_ID_NOT_TUNNELLED',
      'FILE_ACTION_MODIFIED',
+     'FILE_ACTION_MODIFIED_STREAM',
      'FILE_ACTION_REMOVED',
+     'FILE_ACTION_REMOVED_BY_DELETE',
+     'FILE_ACTION_REMOVED_STREAM',
      'FILE_ACTION_RENAMED_NEW_NAME',
      'FILE_ACTION_RENAMED_OLD_NAME',
+     'FILE_ACTION_TUNNELLED_ID_COLLISION',
      'FILE_ADD_FILE',
      'FILE_ADD_SUBDIRECTORY',
      'FILE_ALL_ACCESS',
      'FILE_APPEND_DATA',
      'FILE_ATTRIBUTE_ARCHIVE',
      'FILE_ATTRIBUTE_COMPRESSED',
      'FILE_ATTRIBUTE_DEVICE',
@@ -1281,19 +1291,25 @@
      'FILE_MAP_WRITE',
      'FILE_MAXIMUM_DISPOSITION',
      'FILE_NAMED_STREAMS',
      'FILE_NON_DIRECTORY_FILE',
      'FILE_NOTIFY_CHANGE_ATTRIBUTES',
      'FILE_NOTIFY_CHANGE_CREATION',
      'FILE_NOTIFY_CHANGE_DIR_NAME',
+     'FILE_NOTIFY_CHANGE_EA',
      'FILE_NOTIFY_CHANGE_FILE_NAME',
      'FILE_NOTIFY_CHANGE_LAST_ACCESS',
      'FILE_NOTIFY_CHANGE_LAST_WRITE',
+     'FILE_NOTIFY_CHANGE_NAME',
      'FILE_NOTIFY_CHANGE_SECURITY',
      'FILE_NOTIFY_CHANGE_SIZE',
+     'FILE_NOTIFY_CHANGE_STREAM_NAME',
+     'FILE_NOTIFY_CHANGE_STREAM_SIZE',
+     'FILE_NOTIFY_CHANGE_STREAM_WRITE',
+     'FILE_NOTIFY_VALID_MASK',
      'FILE_NO_COMPRESSION',
      'FILE_NO_EA_KNOWLEDGE',
      'FILE_NO_INTERMEDIATE_BUFFERING',
      'FILE_OPEN',
      'FILE_OPENED',
      'FILE_OPEN_BY_FILE_ID',
      'FILE_OPEN_FOR_BACKUP_INTENT',
@@ -1533,17 +1549,42 @@
      'IMAGE_SIZEOF_STD_OPTIONAL_HEADER',
      'INFINITE',
      'INHERITED_ACE',
      'INHERIT_CALLER_PRIORITY',
      'INHERIT_ONLY_ACE',
      'INHERIT_PARENT_AFFINITY',
      'INVALID_HANDLE_VALUE',
+     'INVALID_SOCKET32',
+     'INVALID_SOCKET64',
      'IO_COMPLETION_ALL_ACCESS',
      'IO_COMPLETION_MODIFY_STATE',
      'IO_COMPLETION_QUERY_STATE',
+     'IPPORT_DAYTIME',
+     'IPPORT_DISCARD',
+     'IPPORT_ECHO',
+     'IPPORT_FTP',
+     'IPPORT_MTP',
+     'IPPORT_NAMESERVER',
+     'IPPORT_NETSTAT',
+     'IPPORT_SMTP',
+     'IPPORT_SYSTAT',
+     'IPPORT_TELNET',
+     'IPPORT_TIMESERVER',
+     'IPPORT_WHOIS',
+     'IPPROTO_GGP',
+     'IPPROTO_ICMP',
+     'IPPROTO_IDP',
+     'IPPROTO_IGMP',
+     'IPPROTO_IP',
+     'IPPROTO_MAX',
+     'IPPROTO_ND',
+     'IPPROTO_PUP',
+     'IPPROTO_RAW',
+     'IPPROTO_TCP',
+     'IPPROTO_UDP',
      'JOB_OBJECT_ALL_ACCESS',
      'JOB_OBJECT_ASSIGN_PROCESS',
      'JOB_OBJECT_QUERY',
      'JOB_OBJECT_SET_ATTRIBUTES',
      'JOB_OBJECT_SET_SECURITY_ATTRIBUTES',
      'JOB_OBJECT_TERMINATE',
      'KEY_ALL_ACCESS',
@@ -1556,14 +1597,15 @@
      'KEY_READ',
      'KEY_SET_VALUE',
      'KEY_WOW64_32KEY',
      'KEY_WOW64_64KEY',
      'KEY_WOW64_RES',
      'KEY_WRITE',
      'LABEL_SECURITY_INFORMATION',
+     'LAYERED_PROTOCOL',
      'LOAD_DLL_DEBUG_EVENT',
      'LOG_CONF_BITS',
      'LPC_CLIENT_DIED',
      'LPC_CONNECTION_REQUEST',
      'LPC_DATAGRAM',
      'LPC_DEBUG_EVENT',
      'LPC_ERROR_EVENT',
@@ -1573,28 +1615,39 @@
      'LPC_REPLY',
      'LPC_REQUEST',
      'MAILSLOT_NO_MESSAGE',
      'MAILSLOT_WAIT_FOREVER',
      'MAXIMUM_ALLOWED',
      'MAXLEN_IFDESCR',
      'MAXLEN_PHYSADDR',
+     'MAX_ADAPTER_ADDRESS_LENGTH',
+     'MAX_ADAPTER_DESCRIPTION_LENGTH',
      'MAX_ADAPTER_NAME',
+     'MAX_ADAPTER_NAME_LENGTH',
      'MAX_CLASS_NAME_LEN',
      'MAX_CONFIG_VALUE',
      'MAX_DEVICE_ID_LEN',
      'MAX_DEVNODE_ID_LEN',
+     'MAX_DHCPV6_DUID_LENGTH',
      'MAX_DMA_CHANNELS',
+     'MAX_DNS_SUFFIX_STRING_LENGTH',
+     'MAX_DOMAIN_NAME_LEN',
      'MAX_GUID_STRING_LEN',
+     'MAX_HOSTNAME_LEN',
      'MAX_INSTANCE_VALUE',
      'MAX_INTERFACE_NAME_LEN',
      'MAX_IO_PORTS',
      'MAX_IRQS',
      'MAX_MEM_REGISTERS',
+     'MAX_NERR',
      'MAX_PATH',
+     'MAX_PREFERRED_LENGTH',
      'MAX_PROFILE_LEN',
+     'MAX_PROTOCOL_CHAIN',
+     'MAX_SCOPE_ID_LEN',
      'MEM_4MB_PAGES',
      'MEM_COMMIT',
      'MEM_DECOMMIT',
      'MEM_FREE',
      'MEM_IMAGE',
      'MEM_LARGE_PAGES',
      'MEM_MAPPED',
@@ -1622,14 +1675,347 @@
      'MS_ENH_RSA_AES_PROV_XP_A',
      'MS_ENH_RSA_AES_PROV_XP_W',
      'MS_STRONG_PROV',
      'MS_STRONG_PROV_A',
      'MS_STRONG_PROV_W',
      'MUTANT_ALL_ACCESS',
      'MUTANT_QUERY_STATE',
+     'NERR_ACFFileIOFail',
+     'NERR_ACFNoParent',
+     'NERR_ACFNoRoom',
+     'NERR_ACFNotFound',
+     'NERR_ACFNotLoaded',
+     'NERR_ACFTooManyLists',
+     'NERR_AccountExpired',
+     'NERR_AccountLockedOut',
+     'NERR_AccountUndefined',
+     'NERR_AcctLimitExceeded',
+     'NERR_ActiveConns',
+     'NERR_AddForwarded',
+     'NERR_AlertExists',
+     'NERR_AlreadyCloudDomainJoined',
+     'NERR_AlreadyExists',
+     'NERR_AlreadyForwarded',
+     'NERR_AlreadyLoggedOn',
+     'NERR_BASE',
+     'NERR_BadAsgType',
+     'NERR_BadComponent',
+     'NERR_BadControlRecv',
+     'NERR_BadDest',
+     'NERR_BadDev',
+     'NERR_BadDevString',
+     'NERR_BadDomainJoinInfo',
+     'NERR_BadDosFunction',
+     'NERR_BadDosRetCode',
+     'NERR_BadEventName',
+     'NERR_BadFileCheckSum',
+     'NERR_BadOfflineJoinInfo',
+     'NERR_BadPassword',
+     'NERR_BadPasswordCore',
+     'NERR_BadQueueDevString',
+     'NERR_BadQueuePriority',
+     'NERR_BadReceive',
+     'NERR_BadRecipient',
+     'NERR_BadServiceName',
+     'NERR_BadServiceProgName',
+     'NERR_BadSource',
+     'NERR_BadTransactConfig',
+     'NERR_BadUasConfig',
+     'NERR_BadUsername',
+     'NERR_BrowserConfiguredToNotRun',
+     'NERR_BrowserNotStarted',
+     'NERR_BrowserTableIncomplete',
+     'NERR_BufTooSmall',
+     'NERR_CallingRplSrvr',
+     'NERR_CanNotGrowSegment',
+     'NERR_CanNotGrowUASFile',
+     'NERR_CannotUnjoinAadDomain',
+     'NERR_CantConnectRplSrvr',
+     'NERR_CantCreateJoinInfo',
+     'NERR_CantLoadOfflineHive',
+     'NERR_CantOpenImageFile',
+     'NERR_CantType',
+     'NERR_CantVerifyHostname',
+     'NERR_CfgCompNotFound',
+     'NERR_CfgParamNotFound',
+     'NERR_ClientNameNotFound',
+     'NERR_CommDevInUse',
+     'NERR_ComputerAccountNotFound',
+     'NERR_ConnectionInsecure',
+     'NERR_DCNotFound',
+     'NERR_DS8DCNotFound',
+     'NERR_DS8DCRequired',
+     'NERR_DS9DCNotFound',
+     'NERR_DataTypeInvalid',
+     'NERR_DatabaseUpToDate',
+     'NERR_DefaultJoinRequired',
+     'NERR_DelComputerName',
+     'NERR_DeleteLater',
+     'NERR_DestExists',
+     'NERR_DestIdle',
+     'NERR_DestInvalidOp',
+     'NERR_DestInvalidState',
+     'NERR_DestNoRoom',
+     'NERR_DestNotFound',
+     'NERR_DevInUse',
+     'NERR_DevInvalidOpCode',
+     'NERR_DevNotFound',
+     'NERR_DevNotOpen',
+     'NERR_DevNotRedirected',
+     'NERR_DeviceIsShared',
+     'NERR_DeviceNotShared',
+     'NERR_DeviceShareConflict',
+     'NERR_DfsAlreadyShared',
+     'NERR_DfsBadRenamePath',
+     'NERR_DfsCantCreateJunctionPoint',
+     'NERR_DfsCantRemoveDfsRoot',
+     'NERR_DfsCantRemoveLastServerShare',
+     'NERR_DfsChildOrParentInDfs',
+     'NERR_DfsCyclicalName',
+     'NERR_DfsDataIsIdentical',
+     'NERR_DfsDuplicateService',
+     'NERR_DfsInconsistent',
+     'NERR_DfsInternalCorruption',
+     'NERR_DfsInternalError',
+     'NERR_DfsLeafVolume',
+     'NERR_DfsNoSuchServer',
+     'NERR_DfsNoSuchShare',
+     'NERR_DfsNoSuchVolume',
+     'NERR_DfsNotALeafVolume',
+     'NERR_DfsNotSupportedInServerDfs',
+     'NERR_DfsServerNotDfsAware',
+     'NERR_DfsServerUpgraded',
+     'NERR_DfsVolumeAlreadyExists',
+     'NERR_DfsVolumeDataCorrupt',
+     'NERR_DfsVolumeHasMultipleServers',
+     'NERR_DfsVolumeIsInterDfs',
+     'NERR_DfsVolumeIsOffline',
+     'NERR_DifferentServers',
+     'NERR_DriverNotFound',
+     'NERR_DupNameReboot',
+     'NERR_DuplicateName',
+     'NERR_DuplicateShare',
+     'NERR_ErrCommRunSrv',
+     'NERR_ErrorExecingGhost',
+     'NERR_ExecFailure',
+     'NERR_FileIdNotFound',
+     'NERR_GroupExists',
+     'NERR_GroupNotFound',
+     'NERR_GrpMsgProcessor',
+     'NERR_ImageParamErr',
+     'NERR_InUseBySpooler',
+     'NERR_IncompleteDel',
+     'NERR_InternalError',
+     'NERR_InvalidAPI',
+     'NERR_InvalidComputer',
+     'NERR_InvalidDatabase',
+     'NERR_InvalidDevice',
+     'NERR_InvalidLana',
+     'NERR_InvalidLogSeek',
+     'NERR_InvalidLogonHours',
+     'NERR_InvalidMachineNameForJoin',
+     'NERR_InvalidMaxUsers',
+     'NERR_InvalidUASOp',
+     'NERR_InvalidWorkgroupName',
+     'NERR_InvalidWorkstation',
+     'NERR_IsDfsShare',
+     'NERR_ItemNotFound',
+     'NERR_JobInvalidState',
+     'NERR_JobNoRoom',
+     'NERR_JobNotFound',
+     'NERR_JoinPerformedMustRestart',
+     'NERR_LDAPCapableDCRequired',
+     'NERR_LanmanIniError',
+     'NERR_LastAdmin',
+     'NERR_LineTooLong',
+     'NERR_LocalDrive',
+     'NERR_LocalForward',
+     'NERR_LogFileChanged',
+     'NERR_LogFileCorrupt',
+     'NERR_LogOverflow',
+     'NERR_LogonDomainExists',
+     'NERR_LogonNoUserPath',
+     'NERR_LogonScriptError',
+     'NERR_LogonServerConflict',
+     'NERR_LogonServerNotFound',
+     'NERR_LogonTrackingError',
+     'NERR_LogonsPaused',
+     'NERR_MaxLenExceeded',
+     'NERR_MsgAlreadyStarted',
+     'NERR_MsgInitFailed',
+     'NERR_MsgNotStarted',
+     'NERR_MultipleNets',
+     'NERR_NameInUse',
+     'NERR_NameNotForwarded',
+     'NERR_NameNotFound',
+     'NERR_NameUsesIncompatibleCodePage',
+     'NERR_NetNameNotFound',
+     'NERR_NetNotStarted',
+     'NERR_NetlogonNotStarted',
+     'NERR_NetworkError',
+     'NERR_NoAlternateServers',
+     'NERR_NoCommDevs',
+     'NERR_NoComputerName',
+     'NERR_NoForwardName',
+     'NERR_NoJoinPending',
+     'NERR_NoNetworkResource',
+     'NERR_NoOfflineJoinInfo',
+     'NERR_NoRoom',
+     'NERR_NoRplBootSystem',
+     'NERR_NoSuchAlert',
+     'NERR_NoSuchConnection',
+     'NERR_NoSuchServer',
+     'NERR_NoSuchSession',
+     'NERR_NonDosFloppyUsed',
+     'NERR_NonValidatedLogon',
+     'NERR_NotInCache',
+     'NERR_NotInDispatchTbl',
+     'NERR_NotLocalDomain',
+     'NERR_NotLocalName',
+     'NERR_NotLoggedOn',
+     'NERR_NotPrimary',
+     'NERR_OpenFiles',
+     'NERR_PasswordCantChange',
+     'NERR_PasswordExpired',
+     'NERR_PasswordFilterError',
+     'NERR_PasswordHistConflict',
+     'NERR_PasswordMismatch',
+     'NERR_PasswordMustChange',
+     'NERR_PasswordNotComplexEnough',
+     'NERR_PasswordTooLong',
+     'NERR_PasswordTooRecent',
+     'NERR_PasswordTooShort',
+     'NERR_PausedRemote',
+     'NERR_PersonalSku',
+     'NERR_PlainTextSecretsRequired',
+     'NERR_ProcNoRespond',
+     'NERR_ProcNotFound',
+     'NERR_ProfileCleanup',
+     'NERR_ProfileFileTooBig',
+     'NERR_ProfileLoadErr',
+     'NERR_ProfileOffset',
+     'NERR_ProfileSaveErr',
+     'NERR_ProfileUnknownCmd',
+     'NERR_ProgNeedsExtraMem',
+     'NERR_ProvisioningBlobUnsupported',
+     'NERR_QExists',
+     'NERR_QInvalidState',
+     'NERR_QNoRoom',
+     'NERR_QNotFound',
+     'NERR_QueueNotFound',
+     'NERR_RPL_CONNECTED',
+     'NERR_RedirectedPath',
+     'NERR_RemoteBootFailed',
+     'NERR_RemoteErr',
+     'NERR_RemoteFull',
+     'NERR_RemoteOnly',
+     'NERR_ResourceExists',
+     'NERR_ResourceNotFound',
+     'NERR_RplAdapterInfoCorrupted',
+     'NERR_RplAdapterNameUnavailable',
+     'NERR_RplAdapterNotFound',
+     'NERR_RplBackupDatabase',
+     'NERR_RplBadDatabase',
+     'NERR_RplBadRegistry',
+     'NERR_RplBootInUse',
+     'NERR_RplBootInfoCorrupted',
+     'NERR_RplBootNameUnavailable',
+     'NERR_RplBootNotFound',
+     'NERR_RplBootRestart',
+     'NERR_RplBootServiceTerm',
+     'NERR_RplBootStartFailed',
+     'NERR_RplCannotEnum',
+     'NERR_RplConfigInfoCorrupted',
+     'NERR_RplConfigNameUnavailable',
+     'NERR_RplConfigNotEmpty',
+     'NERR_RplConfigNotFound',
+     'NERR_RplIncompatibleProfile',
+     'NERR_RplInternal',
+     'NERR_RplLoadrDiskErr',
+     'NERR_RplLoadrNetBiosErr',
+     'NERR_RplNeedsRPLUSERAcct',
+     'NERR_RplNoAdaptersStarted',
+     'NERR_RplNotRplServer',
+     'NERR_RplProfileInfoCorrupted',
+     'NERR_RplProfileNameUnavailable',
+     'NERR_RplProfileNotEmpty',
+     'NERR_RplProfileNotFound',
+     'NERR_RplRplfilesShare',
+     'NERR_RplSrvrCallFailed',
+     'NERR_RplVendorInfoCorrupted',
+     'NERR_RplVendorNameUnavailable',
+     'NERR_RplVendorNotFound',
+     'NERR_RplWkstaInfoCorrupted',
+     'NERR_RplWkstaNameUnavailable',
+     'NERR_RplWkstaNeedsUserAcct',
+     'NERR_RplWkstaNotFound',
+     'NERR_RunSrvPaused',
+     'NERR_SameAsComputerName',
+     'NERR_ServerNotStarted',
+     'NERR_ServiceCtlBusy',
+     'NERR_ServiceCtlNotValid',
+     'NERR_ServiceCtlTimeout',
+     'NERR_ServiceEntryLocked',
+     'NERR_ServiceInstalled',
+     'NERR_ServiceKillProc',
+     'NERR_ServiceNotCtrl',
+     'NERR_ServiceNotInstalled',
+     'NERR_ServiceNotStarting',
+     'NERR_ServiceTableFull',
+     'NERR_ServiceTableLocked',
+     'NERR_SetupAlreadyJoined',
+     'NERR_SetupCheckDNSConfig',
+     'NERR_SetupDomainController',
+     'NERR_SetupNotJoined',
+     'NERR_ShareMem',
+     'NERR_ShareNotFound',
+     'NERR_SourceIsDir',
+     'NERR_SpeGroupOp',
+     'NERR_SpoolNoMemory',
+     'NERR_SpoolerNotLoaded',
+     'NERR_StandaloneLogon',
+     'NERR_StartingRplBoot',
+     'NERR_Success',
+     'NERR_SyncRequired',
+     'NERR_TargetVersionUnsupported',
+     'NERR_TimeDiffAtDC',
+     'NERR_TmpFile',
+     'NERR_TooManyAlerts',
+     'NERR_TooManyConnections',
+     'NERR_TooManyEntries',
+     'NERR_TooManyFiles',
+     'NERR_TooManyImageParams',
+     'NERR_TooManyItems',
+     'NERR_TooManyNames',
+     'NERR_TooManyServers',
+     'NERR_TooManySessions',
+     'NERR_TooMuchData',
+     'NERR_TruncatedBroadcast',
+     'NERR_TryDownLevel',
+     'NERR_UPSDriverNotStarted',
+     'NERR_UPSInvalidCommPort',
+     'NERR_UPSInvalidConfig',
+     'NERR_UPSShutdownFailed',
+     'NERR_UPSSignalAsserted',
+     'NERR_UnableToAddName_F',
+     'NERR_UnableToAddName_W',
+     'NERR_UnableToDelName_F',
+     'NERR_UnableToDelName_W',
+     'NERR_UnknownDevDir',
+     'NERR_UnknownServer',
+     'NERR_UseNotFound',
+     'NERR_UserExists',
+     'NERR_UserInGroup',
+     'NERR_UserLogon',
+     'NERR_UserNotFound',
+     'NERR_UserNotInGroup',
+     'NERR_ValuesNotSet',
+     'NERR_WkstaInconsistentState',
+     'NERR_WkstaNotStarted',
+     'NERR_WriteFault',
      'NMPWAIT_NOWAIT',
      'NMPWAIT_USE_DEFAULT_WAIT',
      'NMPWAIT_WAIT_FOREVER',
      'NORMAL_PRIORITY_CLASS',
      'NO_PROPAGATE_INHERIT_ACE',
      'NULL',
      'NUM_CR_RESULTS',
@@ -1971,14 +2357,15 @@
      'SECTION_ALL_ACCESS',
      'SECTION_EXTEND_SIZE',
      'SECTION_MAP_EXECUTE',
      'SECTION_MAP_EXECUTE_EXPLICIT',
      'SECTION_MAP_READ',
      'SECTION_MAP_WRITE',
      'SECTION_QUERY',
+     'SECURITY_DESCRIPTOR_REVISION',
      'SECURITY_MANDATORY_HIGH_RID',
      'SECURITY_MANDATORY_LOW_RID',
      'SECURITY_MANDATORY_MEDIUM_PLUS_RID',
      'SECURITY_MANDATORY_MEDIUM_RID',
      'SECURITY_MANDATORY_PROTECTED_PROCESS_RID',
      'SECURITY_MANDATORY_SYSTEM_RID',
      'SECURITY_MANDATORY_UNTRUSTED_RID',
@@ -2238,14 +2625,20 @@
      'SM_SHUTTINGDOWN',
      'SM_SLOWMACHINE',
      'SM_STARTER',
      'SM_SWAPBUTTON',
      'SM_TABLETPC',
      'SM_XVIRTUALSCREEN',
      'SM_YVIRTUALSCREEN',
+     'SOCKET_ERROR',
+     'SOCK_DGRAM',
+     'SOCK_RAW',
+     'SOCK_RDM',
+     'SOCK_SEQPACKET',
+     'SOCK_STREAM',
      'SPC_CAB_DATA_OBJID',
      'SPC_CERT_EXTENSIONS_OBJID',
      'SPC_COMMERCIAL_SP_KEY_PURPOSE_OBJID',
      'SPC_COMMON_NAME_OBJID',
      'SPC_FINANCIAL_CRITERIA_OBJID',
      'SPC_GLUE_RDN_OBJID',
      'SPC_INDIRECT_DATA_OBJID',
@@ -2498,14 +2891,17 @@
      'WIN_CERT_TYPE_TS_STACK_SIGNED',
      'WIN_CERT_TYPE_X509',
      'WOW64_MAXIMUM_SUPPORTED_EXTENSION',
      'WOW64_SIZE_OF_80387_REGISTERS',
      'WRITE_DAC',
      'WRITE_OWNER',
      'WRITE_WATCH_FLAG_RESET',
+     'WSADESCRIPTION_LEN',
+     'WSAPROTOCOL_LEN',
+     'WSASYS_STATUS_LEN',
      'WTD_CHOICE_BLOB',
      'WTD_CHOICE_CATALOG',
      'WTD_CHOICE_CERT',
      'WTD_CHOICE_FILE',
      'WTD_CHOICE_SIGNER',
      'WTD_REVOKE_NONE',
      'WTD_REVOKE_WHOLECHAIN',
@@ -11416,14 +11812,16 @@
      'ACCESS_DENIED_OBJECT_ACE',
      'ACE_HEADER',
      'ACL',
      'ACL_REVISION_INFORMATION',
      'ACL_SIZE_INFORMATION',
      'ADDRESS',
      'ADDRESS64',
+     'ADDRINFOA',
+     'ADDRINFOW',
      'ALPC_CONTEXT_ATTR',
      'ALPC_CONTEXT_ATTR32',
      'ALPC_CONTEXT_ATTR64',
      'ALPC_DATA_VIEW_ATTR',
      'ALPC_DATA_VIEW_ATTR32',
      'ALPC_DATA_VIEW_ATTR64',
      'ALPC_DIRECT_ATTR',
@@ -11616,14 +12014,16 @@
      'DMA_DES',
      'DMA_Des_s',
      'DMA_RANGE',
      'DMA_RESOURCE',
      'DMA_Range_s',
      'DMA_Resource_s',
      'DNS_AAAA_DATA',
+     'DNS_ADDR',
+     'DNS_ADDR_ARRAY',
      'DNS_ATMA_DATA',
      'DNS_A_DATA',
      'DNS_CACHE_ENTRY',
      'DNS_DHCID_DATA',
      'DNS_DNSKEY_DATA',
      'DNS_DS_DATA',
      'DNS_KEY_DATA',
@@ -11640,14 +12040,17 @@
      'DNS_NSEC_DATAW',
      'DNS_NULL_DATA',
      'DNS_NXT_DATAA',
      'DNS_NXT_DATAW',
      'DNS_OPT_DATA',
      'DNS_PTR_DATAA',
      'DNS_PTR_DATAW',
+     'DNS_QUERY_CANCEL',
+     'DNS_QUERY_REQUEST',
+     'DNS_QUERY_RESULT',
      'DNS_RECORDA',
      'DNS_RECORDW',
      'DNS_RECORD_FLAGS',
      'DNS_RRSIG_DATAA',
      'DNS_RRSIG_DATAW',
      'DNS_SIG_DATAA',
      'DNS_SIG_DATAW',
@@ -11723,20 +12126,29 @@
      'FILE_INTERNAL_INFORMATION',
      'FILE_IO_PRIORITY_HINT_INFORMATION',
      'FILE_IS_REMOTE_DEVICE_INFORMATION',
      'FILE_LINK_INFORMATION',
      'FILE_MODE_INFORMATION',
      'FILE_NAME_INFORMATION',
      'FILE_NETWORK_OPEN_INFORMATION',
+     'FILE_NOTIFY_EXTENDED_INFORMATION',
+     'FILE_NOTIFY_INFORMATION',
      'FILE_POSITION_INFORMATION',
+     'FILE_RENAME_INFORMATION',
      'FILE_STANDARD_INFORMATION',
      'FILE_STREAM_INFORMATION',
      'FLOATING_SAVE_AREA',
      'FUNCDESC',
      'GENERIC_MAPPING',
+     'GROUP_INFO_0',
+     'GROUP_INFO_1',
+     'GROUP_INFO_2',
+     'GROUP_INFO_3',
+     'GROUP_USERS_INFO_0',
+     'GROUP_USERS_INFO_1',
      'GUID',
      'IDLDESC',
      'IID',
      'IMAGEHLP_CBA_EVENT',
      'IMAGEHLP_CBA_EVENTW',
      'IMAGEHLP_CBA_READ_MEMORY',
      'IMAGEHLP_DEFERRED_SYMBOL_LOAD',
@@ -11769,15 +12181,21 @@
      'IO_RANGE',
      'IO_RESOURCE',
      'IO_Range_s',
      'IO_Resource_s',
      'IO_STATUS_BLOCK',
      'IP6_ADDRESS',
      'IP_ADAPTER_INDEX_MAP',
+     'IP_ADAPTER_INFO',
+     'IP_ADDRESS_STRING',
+     'IP_ADDR_STRING',
      'IP_INTERFACE_INFO',
+     'IP_MASK_STRING',
+     'IP_PER_ADAPTER_INFO',
+     'IP_PER_ADAPTER_INFO_W2KSP1',
      'IRQ_DES_32',
      'IRQ_DES_64',
      'IRQ_Des_32_s',
      'IRQ_Des_64_s',
      'IRQ_RANGE',
      'IRQ_RESOURCE_32',
      'IRQ_RESOURCE_64',
@@ -11790,14 +12208,20 @@
      'KDHELP64',
      'KEY_VALUE_BASIC_INFORMATION',
      'KEY_VALUE_FULL_INFORMATION',
      'KEY_VALUE_PARTIAL_INFORMATION',
      'LDR_DATA_TABLE_ENTRY',
      'LIST_ENTRY',
      'LOAD_DLL_DEBUG_INFO',
+     'LOCALGROUP_INFO_0',
+     'LOCALGROUP_INFO_1',
+     'LOCALGROUP_MEMBERS_INFO_0',
+     'LOCALGROUP_MEMBERS_INFO_1',
+     'LOCALGROUP_MEMBERS_INFO_2',
+     'LOCALGROUP_MEMBERS_INFO_3',
      'LOCALTHIS',
      'LPADDRESS',
      'LPADDRESS64',
      'LPBINDPTR',
      'LPBIND_OPTS',
      'LPBITMAP',
      'LPBITMAPCOREHEADER',
@@ -11819,20 +12243,30 @@
      'LPENUM_SERVICE_STATUS_PROCESSW',
      'LPEVENTLOG_FULL_INFORMATION',
      'LPEXCEPTION_DEBUG_INFO',
      'LPEXIT_PROCESS_DEBUG_INFO',
      'LPEXIT_THREAD_DEBUG_INFO',
      'LPFILETIME',
      'LPFUNCDESC',
+     'LPGROUP_INFO_0',
+     'LPGROUP_INFO_1',
+     'LPGROUP_USERS_INFO_0',
+     'LPGROUP_USERS_INFO_1',
      'LPGUID',
      'LPIDLDESC',
      'LPINTERNET_BUFFERSA',
      'LPINTERNET_BUFFERSW',
      'LPJIT_DEBUG_INFO',
      'LPLOAD_DLL_DEBUG_INFO',
+     'LPLOCALGROUP_INFO_0',
+     'LPLOCALGROUP_INFO_1',
+     'LPLOCALGROUP_MEMBERS_INFO_0',
+     'LPLOCALGROUP_MEMBERS_INFO_1',
+     'LPLOCALGROUP_MEMBERS_INFO_2',
+     'LPLOCALGROUP_MEMBERS_INFO_3',
      'LPOSVERSIONINFOA',
      'LPOSVERSIONINFOEXA',
      'LPOSVERSIONINFOEXW',
      'LPOSVERSIONINFOW',
      'LPOUTPUT_DEBUG_STRING_INFO',
      'LPOVERLAPPED',
      'LPPARAMDESC',
@@ -11840,14 +12274,15 @@
      'LPPROCESSENTRY32',
      'LPPROCESSENTRY32W',
      'LPPROCESS_INFORMATION',
      'LPQUERY_SERVICE_CONFIGA',
      'LPQUERY_SERVICE_CONFIGW',
      'LPRGBTRIPLE',
      'LPRIP_INFO',
+     'LPSAFEARRAY',
      'LPSAFEARRAYBOUND',
      'LPSECURITY_ATTRIBUTES',
      'LPSERVICE_STATUS',
      'LPSERVICE_STATUS_PROCESS',
      'LPSERVICE_TABLE_ENTRYA',
      'LPSERVICE_TABLE_ENTRYW',
      'LPSHFILEOPSTRUCTA',
@@ -11860,21 +12295,34 @@
      'LPSTARTUPINFOW',
      'LPSYSTEMTIME',
      'LPTHREADENTRY32',
      'LPTIME_ZONE_INFORMATION',
      'LPTLIBATTR',
      'LPTYPEATTR',
      'LPUNLOAD_DLL_DEBUG_INFO',
+     'LPUSER_INFO_0',
+     'LPUSER_INFO_1',
+     'LPUSER_INFO_10',
+     'LPUSER_INFO_11',
+     'LPUSER_INFO_2',
+     'LPUSER_INFO_20',
+     'LPUSER_INFO_23',
+     'LPUSER_INFO_3',
      'LPVARDESC',
      'LPVARIANT',
      'LPVARIANTARG',
      'LPWIN32_FIND_DATAA',
      'LPWIN32_FIND_DATAW',
      'LPWNDCLASSEXA',
      'LPWNDCLASSEXW',
+     'LPWSADATA32',
+     'LPWSADATA64',
+     'LPWSAPROTOCOLCHAIN',
+     'LPWSAPROTOCOL_INFOA',
+     'LPWSAPROTOCOL_INFOW',
      'LSA_OBJECT_ATTRIBUTES',
      'LSA_REFERENCED_DOMAIN_LIST',
      'LSA_TRANSLATED_NAME',
      'LSA_TRANSLATED_SID',
      'LSA_TRANSLATED_SID2',
      'LSA_TRUST_INFORMATION',
      'LSA_UNICODE_STRING',
@@ -11915,14 +12363,17 @@
      'Mem_Large_Des_s',
      'Mem_Large_Range_s',
      'Mem_Large_Resource_s',
      'Mem_Range_s',
      'Mem_Resource_s',
      'MfCard_Des_s',
      'MfCard_Resource_s',
+     'NET_DISPLAY_GROUP',
+     'NET_DISPLAY_MACHINE',
+     'NET_DISPLAY_USER',
      'NPBITMAP',
      'NPRGBTRIPLE',
      'OBJECTS_AND_NAME_A',
      'OBJECTS_AND_NAME_W',
      'OBJECTS_AND_SID',
      'OBJECT_ATTRIBUTES',
      'OBJECT_DIRECTORY_INFORMATION',
@@ -11943,14 +12394,16 @@
      'PACCESS_DENIED_CALLBACK_ACE',
      'PACCESS_DENIED_CALLBACK_OBJECT_ACE',
      'PACCESS_DENIED_OBJECT_ACE',
      'PACE_HEADER',
      'PACL',
      'PACL_REVISION_INFORMATION',
      'PACL_SIZE_INFORMATION',
+     'PADDRINFOA',
+     'PADDRINFOW',
      'PALPC_CONTEXT_ATTR',
      'PALPC_CONTEXT_ATTR32',
      'PALPC_CONTEXT_ATTR64',
      'PALPC_DATA_VIEW_ATTR',
      'PALPC_DATA_VIEW_ATTR32',
      'PALPC_DATA_VIEW_ATTR64',
      'PALPC_DIRECT_ATTR',
@@ -12107,14 +12560,16 @@
      'PDEBUG_SYMBOL_PARAMETERS',
      'PDEBUG_SYMBOL_SOURCE_ENTRY',
      'PDEBUG_VALUE',
      'PDMA_DES',
      'PDMA_RANGE',
      'PDMA_RESOURCE',
      'PDNS_AAAA_DATA',
+     'PDNS_ADDR',
+     'PDNS_ADDR_ARRAY',
      'PDNS_ATMA_DATA',
      'PDNS_A_DATA',
      'PDNS_CACHE_ENTRY',
      'PDNS_DHCID_DATA',
      'PDNS_DNSKEY_DATA',
      'PDNS_DS_DATA',
      'PDNS_KEY_DATA',
@@ -12131,14 +12586,17 @@
      'PDNS_NSEC_DATAW',
      'PDNS_NULL_DATA',
      'PDNS_NXT_DATAA',
      'PDNS_NXT_DATAW',
      'PDNS_OPT_DATA',
      'PDNS_PTR_DATAA',
      'PDNS_PTR_DATAW',
+     'PDNS_QUERY_CANCEL',
+     'PDNS_QUERY_REQUEST',
+     'PDNS_QUERY_RESULT',
      'PDNS_RECORDA',
      'PDNS_RECORDW',
      'PDNS_RRSIG_DATAA',
      'PDNS_RRSIG_DATAW',
      'PDNS_SIG_DATAA',
      'PDNS_SIG_DATAW',
      'PDNS_SOA_DATAA',
@@ -12204,18 +12662,27 @@
      'PFILE_INTERNAL_INFORMATION',
      'PFILE_IO_PRIORITY_HINT_INFORMATION',
      'PFILE_IS_REMOTE_DEVICE_INFORMATION',
      'PFILE_LINK_INFORMATION',
      'PFILE_MODE_INFORMATION',
      'PFILE_NAME_INFORMATION',
      'PFILE_NETWORK_OPEN_INFORMATION',
+     'PFILE_NOTIFY_EXTENDED_INFORMATION',
+     'PFILE_NOTIFY_INFORMATION',
      'PFILE_POSITION_INFORMATION',
+     'PFILE_RENAME_INFORMATION',
      'PFILE_STANDARD_INFORMATION',
      'PFILE_STREAM_INFORMATION',
      'PGENERIC_MAPPING',
+     'PGROUP_INFO_0',
+     'PGROUP_INFO_1',
+     'PGROUP_INFO_2',
+     'PGROUP_INFO_3',
+     'PGROUP_USERS_INFO_0',
+     'PGROUP_USERS_INFO_1',
      'PIDLIST_ABSOLUTE',
      'PIMAGEHLP_CBA_EVENT',
      'PIMAGEHLP_CBA_EVENTW',
      'PIMAGEHLP_CBA_READ_MEMORY',
      'PIMAGEHLP_DEFERRED_SYMBOL_LOAD',
      'PIMAGEHLP_DEFERRED_SYMBOL_LOAD64',
      'PIMAGEHLP_DEFERRED_SYMBOL_LOADW64',
@@ -12241,28 +12708,40 @@
      'PIMAGE_SECTION_HEADER',
      'PIO_DES',
      'PIO_RANGE',
      'PIO_RESOURCE',
      'PIO_STATUS_BLOCK',
      'PIP6_ADDRESS',
      'PIP_ADAPTER_INDEX_MAP',
+     'PIP_ADAPTER_INFO',
+     'PIP_ADDRESS_STRING',
+     'PIP_ADDR_STRING',
      'PIP_INTERFACE_INFO',
+     'PIP_MASK_STRING',
+     'PIP_PER_ADAPTER_INFO',
+     'PIP_PER_ADAPTER_INFO_W2KSP1',
      'PIRQ_DES_32',
      'PIRQ_DES_64',
      'PIRQ_RANGE',
      'PIRQ_RESOURCE_32',
      'PIRQ_RESOURCE_64',
      'PISECURITY_DESCRIPTOR',
      'PKDHELP',
      'PKDHELP64',
      'PKEY_VALUE_BASIC_INFORMATION',
      'PKEY_VALUE_FULL_INFORMATION',
      'PKEY_VALUE_PARTIAL_INFORMATION',
      'PLDR_DATA_TABLE_ENTRY',
      'PLIST_ENTRY',
+     'PLOCALGROUP_INFO_0',
+     'PLOCALGROUP_INFO_1',
+     'PLOCALGROUP_MEMBERS_INFO_0',
+     'PLOCALGROUP_MEMBERS_INFO_1',
+     'PLOCALGROUP_MEMBERS_INFO_2',
+     'PLOCALGROUP_MEMBERS_INFO_3',
      'PLSA_OBJECT_ATTRIBUTES',
      'PLSA_REFERENCED_DOMAIN_LIST',
      'PLSA_TRANSLATED_NAME',
      'PLSA_TRANSLATED_SID',
      'PLSA_TRANSLATED_SID2',
      'PLSA_TRUST_INFORMATION',
      'PLSA_UNICODE_STRING',
@@ -12292,14 +12771,17 @@
      'PMIB_TCPROW_OWNER_PID',
      'PMIB_TCPTABLE_OWNER_PID',
      'PMIB_UDP6ROW_OWNER_PID',
      'PMIB_UDP6TABLE_OWNER_PID',
      'PMIB_UDPROW_OWNER_PID',
      'PMIB_UDPTABLE_OWNER_PID',
      'PMODLOAD_DATA',
+     'PNET_DISPLAY_GROUP',
+     'PNET_DISPLAY_MACHINE',
+     'PNET_DISPLAY_USER',
      'POBJECTS_AND_NAME_A',
      'POBJECTS_AND_NAME_W',
      'POBJECTS_AND_SID',
      'POBJECT_ATTRIBUTES',
      'POBJECT_DIRECTORY_INFORMATION',
      'POBJECT_TYPES_INFORMATION',
      'POLICY_ACCOUNT_DOMAIN_INFO',
@@ -12473,14 +12955,22 @@
      'PTRUSTEEW',
      'PTRUSTEE_A',
      'PTRUSTEE_W',
      'PUBLICKEYSTRUC',
      'PUBLIC_OBJECT_BASIC_INFORMATION',
      'PUBLIC_OBJECT_TYPE_INFORMATION',
      'PUNICODE_STRING',
+     'PUSER_INFO_0',
+     'PUSER_INFO_1',
+     'PUSER_INFO_10',
+     'PUSER_INFO_11',
+     'PUSER_INFO_2',
+     'PUSER_INFO_20',
+     'PUSER_INFO_23',
+     'PUSER_INFO_3',
      'PVIRTUAL_STORAGE_TYPE',
      'PWIN32_FIND_DATAA',
      'PWIN32_FIND_DATAW',
      'PWINTRUST_BLOB_INFO',
      'PWINTRUST_CATALOG_INFO',
      'PWINTRUST_CERT_INFO',
      'PWINTRUST_DATA',
@@ -12632,14 +13122,22 @@
      'TRUSTEEW',
      'TRUSTEE_A',
      'TRUSTEE_W',
      'TYPEATTR',
      'TYPEDESC',
      'UNICODE_STRING',
      'UNLOAD_DLL_DEBUG_INFO',
+     'USER_INFO_0',
+     'USER_INFO_1',
+     'USER_INFO_10',
+     'USER_INFO_11',
+     'USER_INFO_2',
+     'USER_INFO_20',
+     'USER_INFO_23',
+     'USER_INFO_3',
      'VARDESC',
      'VARIANT',
      'VARIANTARG',
      'VIRTUAL_STORAGE_TYPE',
      'VS_FIXEDFILEINFO',
      'WIN32_FIND_DATAA',
      'WIN32_FIND_DATAW',
@@ -12655,14 +13153,21 @@
      'WINTRUST_SGNR_INFO',
      'WINTRUST_SGNR_INFO_',
      'WNDCLASSEXA',
      'WNDCLASSEXW',
      'WNODE_HEADER',
      'WOW64_CONTEXT',
      'WOW64_FLOATING_SAVE_AREA',
+     'WSADATA32',
+     'WSADATA64',
+     'WSAData32',
+     'WSAData64',
+     'WSAPROTOCOLCHAIN',
+     'WSAPROTOCOL_INFOA',
+     'WSAPROTOCOL_INFOW',
      'XSAVE_FORMAT_32',
      'XSAVE_FORMAT_64',
      '_ACCESS_ALLOWED_ACE',
      '_ACCESS_ALLOWED_CALLBACK_ACE',
      '_ACCESS_ALLOWED_CALLBACK_OBJECT_ACE',
      '_ACCESS_ALLOWED_OBJECT_ACE',
      '_ACCESS_DENIED_ACE',
@@ -12823,14 +13328,19 @@
      '_DEBUG_SYMBOL_SOURCE_ENTRY',
      '_DEBUG_VALUE',
      '_DEBUG_VALUE_TMP_SUBSTRUCT1',
      '_DEBUG_VALUE_TMP_SUBSTRUCT2',
      '_DEBUG_VALUE_TMP_SUBSTRUCT3',
      '_DEBUG_VALUE_TMP_UNION',
      '_DNS_CACHE_ENTRY',
+     '_DNS_QUERY_CANCEL',
+     '_DNS_QUERY_REQUEST',
+     '_DNS_QUERY_RESULT',
+     '_DnsAddr',
+     '_DnsAddrArray',
      '_DnsRecordA',
      '_DnsRecordFlags',
      '_DnsRecordW',
      '_ENABLE_TRACE_PARAMETERS',
      '_ENUM_SERVICE_STATUSA',
      '_ENUM_SERVICE_STATUSW',
      '_ENUM_SERVICE_STATUS_PROCESSA',
@@ -12883,19 +13393,28 @@
      '_FILE_INTERNAL_INFORMATION',
      '_FILE_IO_PRIORITY_HINT_INFORMATION',
      '_FILE_IS_REMOTE_DEVICE_INFORMATION',
      '_FILE_LINK_INFORMATION',
      '_FILE_MODE_INFORMATION',
      '_FILE_NAME_INFORMATION',
      '_FILE_NETWORK_OPEN_INFORMATION',
+     '_FILE_NOTIFY_EXTENDED_INFORMATION',
+     '_FILE_NOTIFY_INFORMATION',
      '_FILE_POSITION_INFORMATION',
+     '_FILE_RENAME_INFORMATION',
      '_FILE_STANDARD_INFORMATION',
      '_FILE_STREAM_INFORMATION',
      '_FLOATING_SAVE_AREA',
      '_GENERIC_MAPPING',
+     '_GROUP_INFO_0',
+     '_GROUP_INFO_1',
+     '_GROUP_INFO_2',
+     '_GROUP_INFO_3',
+     '_GROUP_USERS_INFO_0',
+     '_GROUP_USERS_INFO_1',
      '_GUID',
      '_IMAGEHLP_CBA_EVENT',
      '_IMAGEHLP_CBA_EVENTW',
      '_IMAGEHLP_CBA_READ_MEMORY',
      '_IMAGEHLP_DEFERRED_SYMBOL_LOAD',
      '_IMAGEHLP_DEFERRED_SYMBOL_LOAD64',
      '_IMAGEHLP_DEFERRED_SYMBOL_LOADW64',
@@ -12919,25 +13438,34 @@
      '_IMAGE_OPTIONAL_HEADER',
      '_IMAGE_OPTIONAL_HEADER64',
      '_IMAGE_SECTION_HEADER',
      '_INTERNET_BUFFERSA',
      '_INTERNET_BUFFERSW',
      '_IO_STATUS_BLOCK',
      '_IP_ADAPTER_INDEX_MAP',
+     '_IP_ADAPTER_INFO',
+     '_IP_ADDR_STRING',
      '_IP_INTERFACE_INFO',
+     '_IP_PER_ADAPTER_INFO_W2KSP1',
      '_ITEMIDLIST',
      '_JIT_DEBUG_INFO',
      '_KDHELP',
      '_KDHELP64',
      '_KEY_VALUE_BASIC_INFORMATION',
      '_KEY_VALUE_FULL_INFORMATION',
      '_KEY_VALUE_PARTIAL_INFORMATION',
      '_LDR_DATA_TABLE_ENTRY',
      '_LIST_ENTRY',
      '_LOAD_DLL_DEBUG_INFO',
+     '_LOCALGROUP_INFO_0',
+     '_LOCALGROUP_INFO_1',
+     '_LOCALGROUP_MEMBERS_INFO_0',
+     '_LOCALGROUP_MEMBERS_INFO_1',
+     '_LOCALGROUP_MEMBERS_INFO_2',
+     '_LOCALGROUP_MEMBERS_INFO_3',
      '_LOCALTHIS',
      '_LSA_OBJECT_ATTRIBUTES',
      '_LSA_REFERENCED_DOMAIN_LIST',
      '_LSA_TRANSLATED_NAME',
      '_LSA_TRANSLATED_SID',
      '_LSA_TRANSLATED_SID2',
      '_LSA_TRUST_INFORMATION',
@@ -12960,14 +13488,17 @@
      '_MIB_TCPROW_OWNER_PID',
      '_MIB_TCPTABLE_OWNER_PID',
      '_MIB_UDP6ROW_OWNER_PID',
      '_MIB_UDP6TABLE_OWNER_PID',
      '_MIB_UDPROW_OWNER_PID',
      '_MIB_UDPTABLE_OWNER_PID',
      '_MODLOAD_DATA',
+     '_NET_DISPLAY_GROUP',
+     '_NET_DISPLAY_MACHINE',
+     '_NET_DISPLAY_USER',
      '_OBJECTS_AND_NAME_A',
      '_OBJECTS_AND_NAME_W',
      '_OBJECTS_AND_SID',
      '_OBJECT_ATTRIBUTES',
      '_OBJECT_DIRECTORY_INFORMATION',
      '_OBJECT_TYPES_INFORMATION',
      '_OPEN_VIRTUAL_DISK_PARAMETERS',
@@ -13130,21 +13661,32 @@
      '_TRACE_GUID_REGISTRATION',
      '_TRACE_LOGFILE_HEADER',
      '_TRACE_PROVIDER_INFO',
      '_TRACE_PROVIDER_INSTANCE_INFO',
      '_TRUSTEE_A',
      '_TRUSTEE_W',
      '_UNLOAD_DLL_DEBUG_INFO',
+     '_USER_INFO_0',
+     '_USER_INFO_1',
+     '_USER_INFO_10',
+     '_USER_INFO_11',
+     '_USER_INFO_2',
+     '_USER_INFO_20',
+     '_USER_INFO_23',
+     '_USER_INFO_3',
      '_VIRTUAL_STORAGE_TYPE',
      '_WIN32_FIND_DATAA',
      '_WIN32_FIND_DATAW',
      '_WINTRUST_DATA',
      '_WNODE_HEADER',
      '_WOW64_CONTEXT',
      '_WOW64_FLOATING_SAVE_AREA',
+     '_WSAPROTOCOLCHAIN',
+     '_WSAPROTOCOL_INFOA',
+     '_WSAPROTOCOL_INFOW',
      '_XSAVE_FORMAT_32',
      '_XSAVE_FORMAT_64',
      '__MIDL_IBackgroundCopyJob2_0003',
      '__MIDL_IBackgroundCopyJob2_0004',
      '__MIDL_XmitDefs_0001',
      '__PUBLIC_OBJECT_TYPE_INFORMATION',
      '__tagBRECORD',
@@ -13153,14 +13695,19 @@
      '_tagADDRESS64',
      '_tagBRECORD',
      '_tagSTACKFRAME',
      '_tagSTACKFRAME64',
      '_tagSTACKFRAME_EX',
      '_tagVARIANT',
      '_tagpropertykey',
+     'addrinfo',
+     'addrinfoW',
+     'in_addr',
+     'sockaddr',
+     'sockaddr_in',
      'tagARRAYDESC',
      'tagBINDPTR',
      'tagBIND_OPTS',
      'tagBITMAP',
      'tagBITMAPCOREHEADER',
      'tagBITMAPCOREINFO',
      'tagBITMAPFILEHEADER',
@@ -13211,14 +13758,15 @@
      'BasicType',
      'CALLCONV',
      'CALLFRAME_COPY',
      'CALLFRAME_WALK',
      'CBA_EVENT_SEVERITY',
      'CLSCTX',
      'COINIT',
+     'COMPUTER_NAME_FORMAT',
      'COMSD',
      'DESCKIND',
      'DNS_FREE_TYPE',
      'DataKind',
      'EVT_CHANNEL_CONFIG_PROPERTY_ID',
      'EVT_CHANNEL_ISOLATION_TYPE',
      'EVT_CHANNEL_TYPE',
@@ -13269,22 +13817,24 @@
      'PALPC_MESSAGE_INFORMATION_CLASS',
      'PFILE_INFORMATION_CLASS',
      'POLICY_INFORMATION_CLASS',
      'POLICY_LSA_SERVER_ROLE',
      'PPOLICY_INFORMATION_CLASS',
      'PPOLICY_LSA_SERVER_ROLE',
      'PPROCESS_MITIGATION_POLICY',
+     'PREAD_DIRECTORY_NOTIFY_INFORMATION_CLASS',
      'PROCESSINFOCLASS',
      'PROCESS_MITIGATION_POLICY',
      'PSECURITY_IMPERSONATION_LEVEL',
      'PSID_NAME_USE',
      'PTHREAD_INFORMATION_CLASS',
      'PTOKEN_ELEVATION_TYPE',
      'PTOKEN_INFORMATION_CLASS',
      'PTOKEN_TYPE',
+     'READ_DIRECTORY_NOTIFY_INFORMATION_CLASS',
      'RTL_PATH_TYPE',
      'SC_ENUM_TYPE',
      'SC_STATUS_TYPE',
      'SECTION_INHERIT',
      'SECURITY_IMPERSONATION_LEVEL',
      'SE_OBJECT_TYPE',
      'SIATTRIBFLAGS',
@@ -13338,14 +13888,15 @@
      '_BG_ERROR_CONTEXT',
      '_BG_JOB_PRIORITY',
      '_BG_JOB_PROXY_USAGE',
      '_BG_JOB_STATE',
      '_BG_JOB_TYPE',
      '_CALLFRAME_COPY',
      '_CBA_EVENT_SEVERITY',
+     '_COMPUTER_NAME_FORMAT',
      '_EVT_CHANNEL_CONFIG_PROPERTY_ID',
      '_EVT_CHANNEL_ISOLATION_TYPE',
      '_EVT_CHANNEL_TYPE',
      '_EVT_EVENT_METADATA_PROPERTY_ID',
      '_EVT_FORMAT_MESSAGE_FLAGS',
      '_EVT_LOGIN_CLASS',
      '_EVT_LOG_PROPERTY_ID',
@@ -13373,14 +13924,15 @@
      '_OBJECT_INFORMATION_CLASS',
      '_OPEN_VIRTUAL_DISK_FLAG',
      '_OPEN_VIRTUAL_DISK_VERSION',
      '_POLICY_INFORMATION_CLASS',
      '_POLICY_LSA_SERVER_ROLE',
      '_PROCESSINFOCLASS',
      '_PROCESS_MITIGATION_POLICY',
+     '_READ_DIRECTORY_NOTIFY_INFORMATION_CLASS',
      '_RTL_PATH_TYPE',
      '_SC_ENUM_TYPE',
      '_SC_STATUS_TYPE',
      '_SECTION_INHERIT',
      '_SECURITY_IMPERSONATION_LEVEL',
      '_SE_OBJECT_TYPE',
      '_SID_NAME_USE',
@@ -13613,14 +14165,15 @@
      'DebugBreakProcess',
      'DebugSetProcessKillOnExit',
      'DeleteProcThreadAttributeList',
      'DeleteService',
      'DeviceIoControl',
      'DnsFree',
      'DnsGetCacheDataTable',
+     'DnsQueryEx',
      'DnsQuery_A',
      'DnsQuery_W',
      'DuplicateHandle',
      'DuplicateToken',
      'DuplicateTokenEx',
      'EmptyClipboard',
      'EnableTrace',
@@ -13662,49 +14215,63 @@
      'EvtQuery',
      'EvtRender',
      'EvtSeek',
      'ExitProcess',
      'ExitThread',
      'FileTimeToSystemTime',
      'FindClose',
+     'FindCloseChangeNotification',
+     'FindFirstChangeNotificationA',
+     'FindFirstChangeNotificationW',
      'FindFirstFileA',
      'FindFirstFileW',
      'FindFirstVolumeA',
      'FindFirstVolumeW',
+     'FindNextChangeNotification',
      'FindNextFileA',
      'FindNextFileW',
      'FindNextVolumeA',
      'FindNextVolumeW',
      'FindResourceA',
      'FindResourceW',
      'FindWindowA',
      'FindWindowW',
      'FreeConsole',
+     'FreeEnvironmentStringsA',
+     'FreeEnvironmentStringsW',
      'FreeLibrary',
      'FreeResource',
      'FreeSid',
      'GetAce',
      'GetAclInformation',
+     'GetAdaptersInfo',
+     'GetAddrInfoW',
      'GetClassInfoExA',
      'GetClassInfoExW',
      'GetClassNameA',
      'GetClassNameW',
      'GetClipboardData',
      'GetClipboardFormatNameA',
      'GetClipboardFormatNameW',
      'GetComputerNameA',
+     'GetComputerNameExA',
+     'GetComputerNameExW',
      'GetComputerNameW',
      'GetCurrentProcess',
      'GetCurrentProcessorNumber',
      'GetCurrentThread',
      'GetCurrentThreadId',
      'GetCursorPos',
      'GetDesktopWindow',
      'GetDriveTypeA',
      'GetDriveTypeW',
+     'GetEnvironmentStringsA',
+     'GetEnvironmentStringsW',
+     'GetEnvironmentVariableA',
+     'GetEnvironmentVariableW',
      'GetEventLogInformation',
      'GetExitCodeProcess',
      'GetExitCodeThread',
      'GetExtendedTcpTable',
      'GetExtendedUdpTable',
      'GetFileVersionInfoA',
      'GetFileVersionInfoExA',
@@ -13738,14 +14305,15 @@
      'GetModuleFileNameW',
      'GetModuleHandleA',
      'GetModuleHandleW',
      'GetNamedSecurityInfoA',
      'GetNamedSecurityInfoW',
      'GetNumberOfEventLogRecords',
      'GetParent',
+     'GetPerAdapterInfo',
      'GetPriorityClass',
      'GetProcAddress',
      'GetProcessDEPPolicy',
      'GetProcessId',
      'GetProcessImageFileNameA',
      'GetProcessImageFileNameW',
      'GetProcessMemoryInfo',
@@ -13837,14 +14405,16 @@
      'LdrLoadDll',
      'LoadLibraryA',
      'LoadLibraryExA',
      'LoadLibraryExW',
      'LoadLibraryW',
      'LoadResource',
      'LocalFree',
+     'LockFile',
+     'LockFileEx',
      'LockResource',
      'LookupAccountNameA',
      'LookupAccountNameW',
      'LookupAccountSidA',
      'LookupAccountSidW',
      'LookupPrivilegeNameA',
      'LookupPrivilegeNameW',
@@ -13854,19 +14424,30 @@
      'LsaLookupNames',
      'LsaLookupNames2',
      'LsaLookupSids',
      'LsaLookupSids2',
      'LsaNtStatusToWinError',
      'LsaOpenPolicy',
      'LsaQueryInformationPolicy',
+     'MakeAbsoluteSD',
+     'MakeSelfRelativeSD',
      'MapGenericMask',
      'MapViewOfFile',
      'MessageBoxA',
      'MessageBoxW',
      'MoveWindow',
+     'NetApiBufferFree',
+     'NetGroupEnum',
+     'NetGroupGetInfo',
+     'NetGroupGetUsers',
+     'NetLocalGroupEnum',
+     'NetLocalGroupGetInfo',
+     'NetLocalGroupGetMembers',
+     'NetQueryDisplayInformation',
+     'NetUserEnum',
      'NtAllocateVirtualMemory',
      'NtAlpcAcceptConnectPort',
      'NtAlpcConnectPort',
      'NtAlpcConnectPortEx',
      'NtAlpcCreatePort',
      'NtAlpcCreatePortSection',
      'NtAlpcCreateResourceReserve',
@@ -13970,14 +14551,16 @@
      'QueryServiceConfigA',
      'QueryServiceConfigW',
      'QueryServiceDynamicInformation',
      'QueryServiceStatus',
      'QueryServiceStatusEx',
      'QueryWorkingSet',
      'QueryWorkingSetEx',
+     'ReadDirectoryChangesExW',
+     'ReadDirectoryChangesW',
      'ReadEventLogA',
      'ReadEventLogW',
      'ReadFile',
      'ReadProcessMemory',
      'RealGetWindowClassA',
      'RealGetWindowClassW',
      'RegCloseKey',
@@ -13994,28 +14577,32 @@
      'RegEnumKeyExA',
      'RegEnumKeyExW',
      'RegEnumValueA',
      'RegEnumValueW',
      'RegGetKeySecurity',
      'RegGetValueA',
      'RegGetValueW',
+     'RegLoadKeyA',
+     'RegLoadKeyW',
      'RegOpenKeyExA',
      'RegOpenKeyExW',
      'RegQueryInfoKeyA',
      'RegQueryInfoKeyW',
      'RegQueryValueExA',
      'RegQueryValueExW',
      'RegSaveKeyA',
      'RegSaveKeyExA',
      'RegSaveKeyExW',
      'RegSaveKeyW',
      'RegSetKeyValueA',
      'RegSetKeyValueW',
      'RegSetValueExA',
      'RegSetValueExW',
+     'RegUnLoadKeyA',
+     'RegUnLoadKeyW',
      'RegisterTraceGuidsA',
      'RegisterTraceGuidsW',
      'RemoveVectoredExceptionHandler',
      'ResumeThread',
      'RollbackTransaction',
      'RtlAnsiStringToUnicodeString',
      'RtlCompressBuffer',
@@ -14023,26 +14610,44 @@
      'RtlDecompressBufferEx',
      'RtlDosPathNameToNtPathName_U',
      'RtlEqualUnicodeString',
      'RtlGetCompressionWorkSpaceSize',
      'RtlGetUnloadEventTraceEx',
      'RtlInitString',
      'RtlInitUnicodeString',
+     'RtlMoveMemory',
      'SHFileOperationA',
      'SHGetPathFromIDListA',
      'SHGetPathFromIDListW',
+     'SafeArrayCopy',
+     'SafeArrayCopyData',
+     'SafeArrayCreate',
+     'SafeArrayCreateVector',
+     'SafeArrayDestroy',
+     'SafeArrayDestroyData',
+     'SafeArrayGetDim',
+     'SafeArrayGetElement',
+     'SafeArrayGetElemsize',
+     'SafeArrayGetLBound',
+     'SafeArrayGetUBound',
+     'SafeArrayGetVartype',
+     'SafeArrayPutElement',
      'SetAclInformation',
      'SetClipboardData',
      'SetConsoleCtrlHandler',
+     'SetEnvironmentStringsW',
+     'SetEnvironmentVariableA',
+     'SetEnvironmentVariableW',
      'SetNamedPipeHandleState',
      'SetNamedSecurityInfoA',
      'SetNamedSecurityInfoW',
      'SetPriorityClass',
      'SetProcessMitigationPolicy',
      'SetSecurityDescriptorDacl',
+     'SetSecurityDescriptorOwner',
      'SetSecurityInfo',
      'SetStdHandle',
      'SetTcpEntry',
      'SetThreadAffinityMask',
      'SetThreadContext',
      'SetThreadToken',
      'SetTokenInformation',
@@ -14128,14 +14733,16 @@
      'SymSrvGetFileIndexStringW',
      'SymSrvGetFileIndexes',
      'SymSrvGetFileIndexesW',
      'SymUnDName',
      'SymUnDName64',
      'SymUnloadModule',
      'SymUnloadModule64',
+     'SysAllocString',
+     'SysFreeString',
      'SystemTimeToFileTime',
      'TdhEnumerateProviders',
      'TerminateProcess',
      'TerminateThread',
      'Thread32First',
      'Thread32Next',
      'TpCallbackSendAlpcMessageOnCompletion',
@@ -14152,28 +14759,50 @@
      'VirtualAllocEx',
      'VirtualFree',
      'VirtualFreeEx',
      'VirtualProtect',
      'VirtualProtectEx',
      'VirtualQuery',
      'VirtualQueryEx',
+     'WSACleanup',
+     'WSAGetLastError',
+     'WSASocketA',
+     'WSASocketW',
+     'WSAStartup',
      'WaitForDebugEvent',
      'WaitForSingleObject',
+     'WinHttpAddRequestHeaders',
+     'WinHttpCloseHandle',
+     'WinHttpConnect',
+     'WinHttpOpen',
+     'WinHttpOpenRequest',
+     'WinHttpQueryDataAvailable',
+     'WinHttpQueryHeaders',
+     'WinHttpReadData',
+     'WinHttpReceiveResponse',
+     'WinHttpSendRequest',
      'WinVerifyTrust',
      'WindowFromPoint',
      'Wow64DisableWow64FsRedirection',
      'Wow64EnableWow64FsRedirection',
      'Wow64GetThreadContext',
      'Wow64RevertWow64FsRedirection',
      'Wow64SetThreadContext',
      'WriteFile',
      'WriteProcessMemory',
      'ZwDuplicateObject',
+     'closesocket',
+     'connect',
+     'getaddrinfo',
      'lstrcmpA',
-     'lstrcmpW'])
+     'lstrcmpW',
+     'recv',
+     'send',
+     'shutdown',
+     'socket'])
 interfaces = set(['IAction',
      'IActionCollection',
      'IApplicationActivationManager',
      'IBackgroundCopyCallback',
      'IBackgroundCopyError',
      'IBackgroundCopyFile',
      'IBackgroundCopyFile2',
@@ -14238,14 +14867,15 @@
      'ITypeLib',
      'IUnknown',
      'IWbemCallResult',
      'IWbemClassObject',
      'IWbemContext',
      'IWbemLocator',
      'IWbemObjectSink',
+     'IWbemObjectTextSrc',
      'IWbemQualifierSet',
      'IWbemServices',
      'IWebBrowser2'])
 
 def generate_walker(namelist, target_module):
     def my_walker():
         for name in namelist:
```

### Comparing `PythonForWindows-0.6.5/windows/generated_def/ntstatus.py` & `PythonForWindows-0.6.8/windows/generated_def/ntstatus.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/generated_def/windef.py` & `PythonForWindows-0.6.8/windows/generated_def/windef.py`

 * *Files 23% similar despite different names*

```diff
@@ -544,14 +544,77 @@
 EVENT_TRACE_FLAG_DISK_FILE_IO = make_flag("EVENT_TRACE_FLAG_DISK_FILE_IO", 0x00000200)
 EVENT_TRACE_FLAG_MEMORY_PAGE_FAULTS = make_flag("EVENT_TRACE_FLAG_MEMORY_PAGE_FAULTS", 0x00001000)
 EVENT_TRACE_FLAG_MEMORY_HARD_FAULTS = make_flag("EVENT_TRACE_FLAG_MEMORY_HARD_FAULTS", 0x00002000)
 EVENT_TRACE_FLAG_NETWORK_TCPIP = make_flag("EVENT_TRACE_FLAG_NETWORK_TCPIP", 0x00010000)
 EVENT_TRACE_FLAG_REGISTRY = make_flag("EVENT_TRACE_FLAG_REGISTRY", 0x00020000)
 EVENT_TRACE_FLAG_DBGPRINT = make_flag("EVENT_TRACE_FLAG_DBGPRINT", 0x00040000)
 EVENT_TRACE_FLAG_VOLMGR = make_flag("EVENT_TRACE_FLAG_VOLMGR", 0x00200000)
+FILE_NOTIFY_CHANGE_FILE_NAME = make_flag("FILE_NOTIFY_CHANGE_FILE_NAME", 0x00000001)
+FILE_NOTIFY_CHANGE_DIR_NAME = make_flag("FILE_NOTIFY_CHANGE_DIR_NAME", 0x00000002)
+FILE_NOTIFY_CHANGE_NAME = make_flag("FILE_NOTIFY_CHANGE_NAME", 0x00000003)
+FILE_NOTIFY_CHANGE_ATTRIBUTES = make_flag("FILE_NOTIFY_CHANGE_ATTRIBUTES", 0x00000004)
+FILE_NOTIFY_CHANGE_SIZE = make_flag("FILE_NOTIFY_CHANGE_SIZE", 0x00000008)
+FILE_NOTIFY_CHANGE_LAST_WRITE = make_flag("FILE_NOTIFY_CHANGE_LAST_WRITE", 0x00000010)
+FILE_NOTIFY_CHANGE_LAST_ACCESS = make_flag("FILE_NOTIFY_CHANGE_LAST_ACCESS", 0x00000020)
+FILE_NOTIFY_CHANGE_CREATION = make_flag("FILE_NOTIFY_CHANGE_CREATION", 0x00000040)
+FILE_NOTIFY_CHANGE_EA = make_flag("FILE_NOTIFY_CHANGE_EA", 0x00000080)
+FILE_NOTIFY_CHANGE_SECURITY = make_flag("FILE_NOTIFY_CHANGE_SECURITY", 0x00000100)
+FILE_NOTIFY_CHANGE_STREAM_NAME = make_flag("FILE_NOTIFY_CHANGE_STREAM_NAME", 0x00000200)
+FILE_NOTIFY_CHANGE_STREAM_SIZE = make_flag("FILE_NOTIFY_CHANGE_STREAM_SIZE", 0x00000400)
+FILE_NOTIFY_CHANGE_STREAM_WRITE = make_flag("FILE_NOTIFY_CHANGE_STREAM_WRITE", 0x00000800)
+FILE_NOTIFY_VALID_MASK = make_flag("FILE_NOTIFY_VALID_MASK", 0x00000fff)
+FILE_ACTION_ADDED = make_flag("FILE_ACTION_ADDED", 0x00000001)
+FILE_ACTION_REMOVED = make_flag("FILE_ACTION_REMOVED", 0x00000002)
+FILE_ACTION_MODIFIED = make_flag("FILE_ACTION_MODIFIED", 0x00000003)
+FILE_ACTION_RENAMED_OLD_NAME = make_flag("FILE_ACTION_RENAMED_OLD_NAME", 0x00000004)
+FILE_ACTION_RENAMED_NEW_NAME = make_flag("FILE_ACTION_RENAMED_NEW_NAME", 0x00000005)
+FILE_ACTION_ADDED_STREAM = make_flag("FILE_ACTION_ADDED_STREAM", 0x00000006)
+FILE_ACTION_REMOVED_STREAM = make_flag("FILE_ACTION_REMOVED_STREAM", 0x00000007)
+FILE_ACTION_MODIFIED_STREAM = make_flag("FILE_ACTION_MODIFIED_STREAM", 0x00000008)
+FILE_ACTION_REMOVED_BY_DELETE = make_flag("FILE_ACTION_REMOVED_BY_DELETE", 0x00000009)
+FILE_ACTION_ID_NOT_TUNNELLED = make_flag("FILE_ACTION_ID_NOT_TUNNELLED", 0x0000000A)
+FILE_ACTION_TUNNELLED_ID_COLLISION = make_flag("FILE_ACTION_TUNNELLED_ID_COLLISION", 0x0000000B)
+FILE_CASE_SENSITIVE_SEARCH = make_flag("FILE_CASE_SENSITIVE_SEARCH", 0x00000001)
+FILE_CASE_PRESERVED_NAMES = make_flag("FILE_CASE_PRESERVED_NAMES", 0x00000002)
+FILE_UNICODE_ON_DISK = make_flag("FILE_UNICODE_ON_DISK", 0x00000004)
+FILE_PERSISTENT_ACLS = make_flag("FILE_PERSISTENT_ACLS", 0x00000008)
+FILE_FILE_COMPRESSION = make_flag("FILE_FILE_COMPRESSION", 0x00000010)
+FILE_VOLUME_QUOTAS = make_flag("FILE_VOLUME_QUOTAS", 0x00000020)
+FILE_SUPPORTS_SPARSE_FILES = make_flag("FILE_SUPPORTS_SPARSE_FILES", 0x00000040)
+FILE_SUPPORTS_REPARSE_POINTS = make_flag("FILE_SUPPORTS_REPARSE_POINTS", 0x00000080)
+FILE_SUPPORTS_REMOTE_STORAGE = make_flag("FILE_SUPPORTS_REMOTE_STORAGE", 0x00000100)
+FILE_VOLUME_IS_COMPRESSED = make_flag("FILE_VOLUME_IS_COMPRESSED", 0x00008000)
+FILE_SUPPORTS_OBJECT_IDS = make_flag("FILE_SUPPORTS_OBJECT_IDS", 0x00010000)
+FILE_SUPPORTS_ENCRYPTION = make_flag("FILE_SUPPORTS_ENCRYPTION", 0x00020000)
+FILE_NAMED_STREAMS = make_flag("FILE_NAMED_STREAMS", 0x00040000)
+FILE_READ_ONLY_VOLUME = make_flag("FILE_READ_ONLY_VOLUME", 0x00080000)
+FILE_SEQUENTIAL_WRITE_ONCE = make_flag("FILE_SEQUENTIAL_WRITE_ONCE", 0x00100000)
+FILE_SUPPORTS_TRANSACTIONS = make_flag("FILE_SUPPORTS_TRANSACTIONS", 0x00200000)
+FILE_SUPPORTS_HARD_LINKS = make_flag("FILE_SUPPORTS_HARD_LINKS", 0x00400000)
+FILE_SUPPORTS_EXTENDED_ATTRIBUTES = make_flag("FILE_SUPPORTS_EXTENDED_ATTRIBUTES", 0x00800000)
+FILE_SUPPORTS_OPEN_BY_FILE_ID = make_flag("FILE_SUPPORTS_OPEN_BY_FILE_ID", 0x01000000)
+FILE_SUPPORTS_USN_JOURNAL = make_flag("FILE_SUPPORTS_USN_JOURNAL", 0x02000000)
+FILE_SHARE_READ = make_flag("FILE_SHARE_READ", 0x00000001)
+FILE_SHARE_WRITE = make_flag("FILE_SHARE_WRITE", 0x00000002)
+FILE_SHARE_DELETE = make_flag("FILE_SHARE_DELETE", 0x00000004)
+FILE_ATTRIBUTE_READONLY = make_flag("FILE_ATTRIBUTE_READONLY", 0x00000001)
+FILE_ATTRIBUTE_HIDDEN = make_flag("FILE_ATTRIBUTE_HIDDEN", 0x00000002)
+FILE_ATTRIBUTE_SYSTEM = make_flag("FILE_ATTRIBUTE_SYSTEM", 0x00000004)
+FILE_ATTRIBUTE_DIRECTORY = make_flag("FILE_ATTRIBUTE_DIRECTORY", 0x00000010)
+FILE_ATTRIBUTE_ARCHIVE = make_flag("FILE_ATTRIBUTE_ARCHIVE", 0x00000020)
+FILE_ATTRIBUTE_DEVICE = make_flag("FILE_ATTRIBUTE_DEVICE", 0x00000040)
+FILE_ATTRIBUTE_NORMAL = make_flag("FILE_ATTRIBUTE_NORMAL", 0x00000080)
+FILE_ATTRIBUTE_TEMPORARY = make_flag("FILE_ATTRIBUTE_TEMPORARY", 0x00000100)
+FILE_ATTRIBUTE_SPARSE_FILE = make_flag("FILE_ATTRIBUTE_SPARSE_FILE", 0x00000200)
+FILE_ATTRIBUTE_REPARSE_POINT = make_flag("FILE_ATTRIBUTE_REPARSE_POINT", 0x00000400)
+FILE_ATTRIBUTE_COMPRESSED = make_flag("FILE_ATTRIBUTE_COMPRESSED", 0x00000800)
+FILE_ATTRIBUTE_OFFLINE = make_flag("FILE_ATTRIBUTE_OFFLINE", 0x00001000)
+FILE_ATTRIBUTE_NOT_CONTENT_INDEXED = make_flag("FILE_ATTRIBUTE_NOT_CONTENT_INDEXED", 0x00002000)
+FILE_ATTRIBUTE_ENCRYPTED = make_flag("FILE_ATTRIBUTE_ENCRYPTED", 0x00004000)
+FILE_ATTRIBUTE_VIRTUAL = make_flag("FILE_ATTRIBUTE_VIRTUAL", 0x00010000)
 X86_KGDT_NULL = make_flag("X86_KGDT_NULL", 0)
 X86_KGDT_R0_CODE = make_flag("X86_KGDT_R0_CODE", 8)
 X86_KGDT_R0_DATA = make_flag("X86_KGDT_R0_DATA", 16)
 X86_KGDT_R3_CODE = make_flag("X86_KGDT_R3_CODE", 24)
 X86_KGDT_R3_DATA = make_flag("X86_KGDT_R3_DATA", 32)
 X86_KGDT_TSS = make_flag("X86_KGDT_TSS", 40)
 X86_KGDT_R0_PCR = make_flag("X86_KGDT_R0_PCR", 48)
@@ -578,21 +641,357 @@
 CS_USER_32B = make_flag("CS_USER_32B", ( AMD64_KGDT64_R3_CMCODE | RPL_MASK ))
 CS_USER_64B = make_flag("CS_USER_64B", ( AMD64_KGDT64_R3_CODE | RPL_MASK ))
 FC_ALLOCATE_ALL_NODES = make_flag("FC_ALLOCATE_ALL_NODES", 0x01)
 FC_DONT_FREE = make_flag("FC_DONT_FREE", 0x02)
 FC_ALLOCED_ON_STACK = make_flag("FC_ALLOCED_ON_STACK", 0x04)
 FC_SIMPLE_POINTER = make_flag("FC_SIMPLE_POINTER", 0x08)
 FC_POINTER_DEREF = make_flag("FC_POINTER_DEREF", 0x10)
+MAX_PREFERRED_LENGTH = make_flag("MAX_PREFERRED_LENGTH", 0xffffffff)
+NERR_Success = make_flag("NERR_Success", 0)
+NERR_BASE = make_flag("NERR_BASE", 2100)
+NERR_NetNotStarted = make_flag("NERR_NetNotStarted", ( NERR_BASE + 2 ))
+NERR_UnknownServer = make_flag("NERR_UnknownServer", ( NERR_BASE + 3 ))
+NERR_ShareMem = make_flag("NERR_ShareMem", ( NERR_BASE + 4 ))
+NERR_NoNetworkResource = make_flag("NERR_NoNetworkResource", ( NERR_BASE + 5 ))
+NERR_RemoteOnly = make_flag("NERR_RemoteOnly", ( NERR_BASE + 6 ))
+NERR_DevNotRedirected = make_flag("NERR_DevNotRedirected", ( NERR_BASE + 7 ))
+NERR_ServerNotStarted = make_flag("NERR_ServerNotStarted", ( NERR_BASE + 14 ))
+NERR_ItemNotFound = make_flag("NERR_ItemNotFound", ( NERR_BASE + 15 ))
+NERR_UnknownDevDir = make_flag("NERR_UnknownDevDir", ( NERR_BASE + 16 ))
+NERR_RedirectedPath = make_flag("NERR_RedirectedPath", ( NERR_BASE + 17 ))
+NERR_DuplicateShare = make_flag("NERR_DuplicateShare", ( NERR_BASE + 18 ))
+NERR_NoRoom = make_flag("NERR_NoRoom", ( NERR_BASE + 19 ))
+NERR_TooManyItems = make_flag("NERR_TooManyItems", ( NERR_BASE + 21 ))
+NERR_InvalidMaxUsers = make_flag("NERR_InvalidMaxUsers", ( NERR_BASE + 22 ))
+NERR_BufTooSmall = make_flag("NERR_BufTooSmall", ( NERR_BASE + 23 ))
+NERR_RemoteErr = make_flag("NERR_RemoteErr", ( NERR_BASE + 27 ))
+NERR_LanmanIniError = make_flag("NERR_LanmanIniError", ( NERR_BASE + 31 ))
+NERR_NetworkError = make_flag("NERR_NetworkError", ( NERR_BASE + 36 ))
+NERR_WkstaInconsistentState = make_flag("NERR_WkstaInconsistentState", ( NERR_BASE + 37 ))
+NERR_WkstaNotStarted = make_flag("NERR_WkstaNotStarted", ( NERR_BASE + 38 ))
+NERR_BrowserNotStarted = make_flag("NERR_BrowserNotStarted", ( NERR_BASE + 39 ))
+NERR_InternalError = make_flag("NERR_InternalError", ( NERR_BASE + 40 ))
+NERR_BadTransactConfig = make_flag("NERR_BadTransactConfig", ( NERR_BASE + 41 ))
+NERR_InvalidAPI = make_flag("NERR_InvalidAPI", ( NERR_BASE + 42 ))
+NERR_BadEventName = make_flag("NERR_BadEventName", ( NERR_BASE + 43 ))
+NERR_DupNameReboot = make_flag("NERR_DupNameReboot", ( NERR_BASE + 44 ))
+NERR_CfgCompNotFound = make_flag("NERR_CfgCompNotFound", ( NERR_BASE + 46 ))
+NERR_CfgParamNotFound = make_flag("NERR_CfgParamNotFound", ( NERR_BASE + 47 ))
+NERR_LineTooLong = make_flag("NERR_LineTooLong", ( NERR_BASE + 49 ))
+NERR_QNotFound = make_flag("NERR_QNotFound", ( NERR_BASE + 50 ))
+NERR_JobNotFound = make_flag("NERR_JobNotFound", ( NERR_BASE + 51 ))
+NERR_DestNotFound = make_flag("NERR_DestNotFound", ( NERR_BASE + 52 ))
+NERR_DestExists = make_flag("NERR_DestExists", ( NERR_BASE + 53 ))
+NERR_QExists = make_flag("NERR_QExists", ( NERR_BASE + 54 ))
+NERR_QNoRoom = make_flag("NERR_QNoRoom", ( NERR_BASE + 55 ))
+NERR_JobNoRoom = make_flag("NERR_JobNoRoom", ( NERR_BASE + 56 ))
+NERR_DestNoRoom = make_flag("NERR_DestNoRoom", ( NERR_BASE + 57 ))
+NERR_DestIdle = make_flag("NERR_DestIdle", ( NERR_BASE + 58 ))
+NERR_DestInvalidOp = make_flag("NERR_DestInvalidOp", ( NERR_BASE + 59 ))
+NERR_ProcNoRespond = make_flag("NERR_ProcNoRespond", ( NERR_BASE + 60 ))
+NERR_SpoolerNotLoaded = make_flag("NERR_SpoolerNotLoaded", ( NERR_BASE + 61 ))
+NERR_DestInvalidState = make_flag("NERR_DestInvalidState", ( NERR_BASE + 62 ))
+NERR_QInvalidState = make_flag("NERR_QInvalidState", ( NERR_BASE + 63 ))
+NERR_JobInvalidState = make_flag("NERR_JobInvalidState", ( NERR_BASE + 64 ))
+NERR_SpoolNoMemory = make_flag("NERR_SpoolNoMemory", ( NERR_BASE + 65 ))
+NERR_DriverNotFound = make_flag("NERR_DriverNotFound", ( NERR_BASE + 66 ))
+NERR_DataTypeInvalid = make_flag("NERR_DataTypeInvalid", ( NERR_BASE + 67 ))
+NERR_ProcNotFound = make_flag("NERR_ProcNotFound", ( NERR_BASE + 68 ))
+NERR_ServiceTableLocked = make_flag("NERR_ServiceTableLocked", ( NERR_BASE + 80 ))
+NERR_ServiceTableFull = make_flag("NERR_ServiceTableFull", ( NERR_BASE + 81 ))
+NERR_ServiceInstalled = make_flag("NERR_ServiceInstalled", ( NERR_BASE + 82 ))
+NERR_ServiceEntryLocked = make_flag("NERR_ServiceEntryLocked", ( NERR_BASE + 83 ))
+NERR_ServiceNotInstalled = make_flag("NERR_ServiceNotInstalled", ( NERR_BASE + 84 ))
+NERR_BadServiceName = make_flag("NERR_BadServiceName", ( NERR_BASE + 85 ))
+NERR_ServiceCtlTimeout = make_flag("NERR_ServiceCtlTimeout", ( NERR_BASE + 86 ))
+NERR_ServiceCtlBusy = make_flag("NERR_ServiceCtlBusy", ( NERR_BASE + 87 ))
+NERR_BadServiceProgName = make_flag("NERR_BadServiceProgName", ( NERR_BASE + 88 ))
+NERR_ServiceNotCtrl = make_flag("NERR_ServiceNotCtrl", ( NERR_BASE + 89 ))
+NERR_ServiceKillProc = make_flag("NERR_ServiceKillProc", ( NERR_BASE + 90 ))
+NERR_ServiceCtlNotValid = make_flag("NERR_ServiceCtlNotValid", ( NERR_BASE + 91 ))
+NERR_NotInDispatchTbl = make_flag("NERR_NotInDispatchTbl", ( NERR_BASE + 92 ))
+NERR_BadControlRecv = make_flag("NERR_BadControlRecv", ( NERR_BASE + 93 ))
+NERR_ServiceNotStarting = make_flag("NERR_ServiceNotStarting", ( NERR_BASE + 94 ))
+NERR_AlreadyLoggedOn = make_flag("NERR_AlreadyLoggedOn", ( NERR_BASE + 100 ))
+NERR_NotLoggedOn = make_flag("NERR_NotLoggedOn", ( NERR_BASE + 101 ))
+NERR_BadUsername = make_flag("NERR_BadUsername", ( NERR_BASE + 102 ))
+NERR_BadPassword = make_flag("NERR_BadPassword", ( NERR_BASE + 103 ))
+NERR_UnableToAddName_W = make_flag("NERR_UnableToAddName_W", ( NERR_BASE + 104 ))
+NERR_UnableToAddName_F = make_flag("NERR_UnableToAddName_F", ( NERR_BASE + 105 ))
+NERR_UnableToDelName_W = make_flag("NERR_UnableToDelName_W", ( NERR_BASE + 106 ))
+NERR_UnableToDelName_F = make_flag("NERR_UnableToDelName_F", ( NERR_BASE + 107 ))
+NERR_LogonsPaused = make_flag("NERR_LogonsPaused", ( NERR_BASE + 109 ))
+NERR_LogonServerConflict = make_flag("NERR_LogonServerConflict", ( NERR_BASE + 110 ))
+NERR_LogonNoUserPath = make_flag("NERR_LogonNoUserPath", ( NERR_BASE + 111 ))
+NERR_LogonScriptError = make_flag("NERR_LogonScriptError", ( NERR_BASE + 112 ))
+NERR_StandaloneLogon = make_flag("NERR_StandaloneLogon", ( NERR_BASE + 114 ))
+NERR_LogonServerNotFound = make_flag("NERR_LogonServerNotFound", ( NERR_BASE + 115 ))
+NERR_LogonDomainExists = make_flag("NERR_LogonDomainExists", ( NERR_BASE + 116 ))
+NERR_NonValidatedLogon = make_flag("NERR_NonValidatedLogon", ( NERR_BASE + 117 ))
+NERR_ACFNotFound = make_flag("NERR_ACFNotFound", ( NERR_BASE + 119 ))
+NERR_GroupNotFound = make_flag("NERR_GroupNotFound", ( NERR_BASE + 120 ))
+NERR_UserNotFound = make_flag("NERR_UserNotFound", ( NERR_BASE + 121 ))
+NERR_ResourceNotFound = make_flag("NERR_ResourceNotFound", ( NERR_BASE + 122 ))
+NERR_GroupExists = make_flag("NERR_GroupExists", ( NERR_BASE + 123 ))
+NERR_UserExists = make_flag("NERR_UserExists", ( NERR_BASE + 124 ))
+NERR_ResourceExists = make_flag("NERR_ResourceExists", ( NERR_BASE + 125 ))
+NERR_NotPrimary = make_flag("NERR_NotPrimary", ( NERR_BASE + 126 ))
+NERR_ACFNotLoaded = make_flag("NERR_ACFNotLoaded", ( NERR_BASE + 127 ))
+NERR_ACFNoRoom = make_flag("NERR_ACFNoRoom", ( NERR_BASE + 128 ))
+NERR_ACFFileIOFail = make_flag("NERR_ACFFileIOFail", ( NERR_BASE + 129 ))
+NERR_ACFTooManyLists = make_flag("NERR_ACFTooManyLists", ( NERR_BASE + 130 ))
+NERR_UserLogon = make_flag("NERR_UserLogon", ( NERR_BASE + 131 ))
+NERR_ACFNoParent = make_flag("NERR_ACFNoParent", ( NERR_BASE + 132 ))
+NERR_CanNotGrowSegment = make_flag("NERR_CanNotGrowSegment", ( NERR_BASE + 133 ))
+NERR_SpeGroupOp = make_flag("NERR_SpeGroupOp", ( NERR_BASE + 134 ))
+NERR_NotInCache = make_flag("NERR_NotInCache", ( NERR_BASE + 135 ))
+NERR_UserInGroup = make_flag("NERR_UserInGroup", ( NERR_BASE + 136 ))
+NERR_UserNotInGroup = make_flag("NERR_UserNotInGroup", ( NERR_BASE + 137 ))
+NERR_AccountUndefined = make_flag("NERR_AccountUndefined", ( NERR_BASE + 138 ))
+NERR_AccountExpired = make_flag("NERR_AccountExpired", ( NERR_BASE + 139 ))
+NERR_InvalidWorkstation = make_flag("NERR_InvalidWorkstation", ( NERR_BASE + 140 ))
+NERR_InvalidLogonHours = make_flag("NERR_InvalidLogonHours", ( NERR_BASE + 141 ))
+NERR_PasswordExpired = make_flag("NERR_PasswordExpired", ( NERR_BASE + 142 ))
+NERR_PasswordCantChange = make_flag("NERR_PasswordCantChange", ( NERR_BASE + 143 ))
+NERR_PasswordHistConflict = make_flag("NERR_PasswordHistConflict", ( NERR_BASE + 144 ))
+NERR_PasswordTooShort = make_flag("NERR_PasswordTooShort", ( NERR_BASE + 145 ))
+NERR_PasswordTooRecent = make_flag("NERR_PasswordTooRecent", ( NERR_BASE + 146 ))
+NERR_InvalidDatabase = make_flag("NERR_InvalidDatabase", ( NERR_BASE + 147 ))
+NERR_DatabaseUpToDate = make_flag("NERR_DatabaseUpToDate", ( NERR_BASE + 148 ))
+NERR_SyncRequired = make_flag("NERR_SyncRequired", ( NERR_BASE + 149 ))
+NERR_UseNotFound = make_flag("NERR_UseNotFound", ( NERR_BASE + 150 ))
+NERR_BadAsgType = make_flag("NERR_BadAsgType", ( NERR_BASE + 151 ))
+NERR_DeviceIsShared = make_flag("NERR_DeviceIsShared", ( NERR_BASE + 152 ))
+NERR_SameAsComputerName = make_flag("NERR_SameAsComputerName", ( NERR_BASE + 153 ))
+NERR_NoComputerName = make_flag("NERR_NoComputerName", ( NERR_BASE + 170 ))
+NERR_MsgAlreadyStarted = make_flag("NERR_MsgAlreadyStarted", ( NERR_BASE + 171 ))
+NERR_MsgInitFailed = make_flag("NERR_MsgInitFailed", ( NERR_BASE + 172 ))
+NERR_NameNotFound = make_flag("NERR_NameNotFound", ( NERR_BASE + 173 ))
+NERR_AlreadyForwarded = make_flag("NERR_AlreadyForwarded", ( NERR_BASE + 174 ))
+NERR_AddForwarded = make_flag("NERR_AddForwarded", ( NERR_BASE + 175 ))
+NERR_AlreadyExists = make_flag("NERR_AlreadyExists", ( NERR_BASE + 176 ))
+NERR_TooManyNames = make_flag("NERR_TooManyNames", ( NERR_BASE + 177 ))
+NERR_DelComputerName = make_flag("NERR_DelComputerName", ( NERR_BASE + 178 ))
+NERR_LocalForward = make_flag("NERR_LocalForward", ( NERR_BASE + 179 ))
+NERR_GrpMsgProcessor = make_flag("NERR_GrpMsgProcessor", ( NERR_BASE + 180 ))
+NERR_PausedRemote = make_flag("NERR_PausedRemote", ( NERR_BASE + 181 ))
+NERR_BadReceive = make_flag("NERR_BadReceive", ( NERR_BASE + 182 ))
+NERR_NameInUse = make_flag("NERR_NameInUse", ( NERR_BASE + 183 ))
+NERR_MsgNotStarted = make_flag("NERR_MsgNotStarted", ( NERR_BASE + 184 ))
+NERR_NotLocalName = make_flag("NERR_NotLocalName", ( NERR_BASE + 185 ))
+NERR_NoForwardName = make_flag("NERR_NoForwardName", ( NERR_BASE + 186 ))
+NERR_RemoteFull = make_flag("NERR_RemoteFull", ( NERR_BASE + 187 ))
+NERR_NameNotForwarded = make_flag("NERR_NameNotForwarded", ( NERR_BASE + 188 ))
+NERR_TruncatedBroadcast = make_flag("NERR_TruncatedBroadcast", ( NERR_BASE + 189 ))
+NERR_InvalidDevice = make_flag("NERR_InvalidDevice", ( NERR_BASE + 194 ))
+NERR_WriteFault = make_flag("NERR_WriteFault", ( NERR_BASE + 195 ))
+NERR_DuplicateName = make_flag("NERR_DuplicateName", ( NERR_BASE + 197 ))
+NERR_DeleteLater = make_flag("NERR_DeleteLater", ( NERR_BASE + 198 ))
+NERR_IncompleteDel = make_flag("NERR_IncompleteDel", ( NERR_BASE + 199 ))
+NERR_MultipleNets = make_flag("NERR_MultipleNets", ( NERR_BASE + 200 ))
+NERR_NetNameNotFound = make_flag("NERR_NetNameNotFound", ( NERR_BASE + 210 ))
+NERR_DeviceNotShared = make_flag("NERR_DeviceNotShared", ( NERR_BASE + 211 ))
+NERR_ClientNameNotFound = make_flag("NERR_ClientNameNotFound", ( NERR_BASE + 212 ))
+NERR_FileIdNotFound = make_flag("NERR_FileIdNotFound", ( NERR_BASE + 214 ))
+NERR_ExecFailure = make_flag("NERR_ExecFailure", ( NERR_BASE + 215 ))
+NERR_TmpFile = make_flag("NERR_TmpFile", ( NERR_BASE + 216 ))
+NERR_TooMuchData = make_flag("NERR_TooMuchData", ( NERR_BASE + 217 ))
+NERR_DeviceShareConflict = make_flag("NERR_DeviceShareConflict", ( NERR_BASE + 218 ))
+NERR_BrowserTableIncomplete = make_flag("NERR_BrowserTableIncomplete", ( NERR_BASE + 219 ))
+NERR_NotLocalDomain = make_flag("NERR_NotLocalDomain", ( NERR_BASE + 220 ))
+NERR_IsDfsShare = make_flag("NERR_IsDfsShare", ( NERR_BASE + 221 ))
+NERR_DevInvalidOpCode = make_flag("NERR_DevInvalidOpCode", ( NERR_BASE + 231 ))
+NERR_DevNotFound = make_flag("NERR_DevNotFound", ( NERR_BASE + 232 ))
+NERR_DevNotOpen = make_flag("NERR_DevNotOpen", ( NERR_BASE + 233 ))
+NERR_BadQueueDevString = make_flag("NERR_BadQueueDevString", ( NERR_BASE + 234 ))
+NERR_BadQueuePriority = make_flag("NERR_BadQueuePriority", ( NERR_BASE + 235 ))
+NERR_NoCommDevs = make_flag("NERR_NoCommDevs", ( NERR_BASE + 237 ))
+NERR_QueueNotFound = make_flag("NERR_QueueNotFound", ( NERR_BASE + 238 ))
+NERR_BadDevString = make_flag("NERR_BadDevString", ( NERR_BASE + 240 ))
+NERR_BadDev = make_flag("NERR_BadDev", ( NERR_BASE + 241 ))
+NERR_InUseBySpooler = make_flag("NERR_InUseBySpooler", ( NERR_BASE + 242 ))
+NERR_CommDevInUse = make_flag("NERR_CommDevInUse", ( NERR_BASE + 243 ))
+NERR_InvalidComputer = make_flag("NERR_InvalidComputer", ( NERR_BASE + 251 ))
+NERR_MaxLenExceeded = make_flag("NERR_MaxLenExceeded", ( NERR_BASE + 254 ))
+NERR_BadComponent = make_flag("NERR_BadComponent", ( NERR_BASE + 256 ))
+NERR_CantType = make_flag("NERR_CantType", ( NERR_BASE + 257 ))
+NERR_TooManyEntries = make_flag("NERR_TooManyEntries", ( NERR_BASE + 262 ))
+NERR_ProfileFileTooBig = make_flag("NERR_ProfileFileTooBig", ( NERR_BASE + 270 ))
+NERR_ProfileOffset = make_flag("NERR_ProfileOffset", ( NERR_BASE + 271 ))
+NERR_ProfileCleanup = make_flag("NERR_ProfileCleanup", ( NERR_BASE + 272 ))
+NERR_ProfileUnknownCmd = make_flag("NERR_ProfileUnknownCmd", ( NERR_BASE + 273 ))
+NERR_ProfileLoadErr = make_flag("NERR_ProfileLoadErr", ( NERR_BASE + 274 ))
+NERR_ProfileSaveErr = make_flag("NERR_ProfileSaveErr", ( NERR_BASE + 275 ))
+NERR_LogOverflow = make_flag("NERR_LogOverflow", ( NERR_BASE + 277 ))
+NERR_LogFileChanged = make_flag("NERR_LogFileChanged", ( NERR_BASE + 278 ))
+NERR_LogFileCorrupt = make_flag("NERR_LogFileCorrupt", ( NERR_BASE + 279 ))
+NERR_SourceIsDir = make_flag("NERR_SourceIsDir", ( NERR_BASE + 280 ))
+NERR_BadSource = make_flag("NERR_BadSource", ( NERR_BASE + 281 ))
+NERR_BadDest = make_flag("NERR_BadDest", ( NERR_BASE + 282 ))
+NERR_DifferentServers = make_flag("NERR_DifferentServers", ( NERR_BASE + 283 ))
+NERR_RunSrvPaused = make_flag("NERR_RunSrvPaused", ( NERR_BASE + 285 ))
+NERR_ErrCommRunSrv = make_flag("NERR_ErrCommRunSrv", ( NERR_BASE + 289 ))
+NERR_ErrorExecingGhost = make_flag("NERR_ErrorExecingGhost", ( NERR_BASE + 291 ))
+NERR_ShareNotFound = make_flag("NERR_ShareNotFound", ( NERR_BASE + 292 ))
+NERR_InvalidLana = make_flag("NERR_InvalidLana", ( NERR_BASE + 300 ))
+NERR_OpenFiles = make_flag("NERR_OpenFiles", ( NERR_BASE + 301 ))
+NERR_ActiveConns = make_flag("NERR_ActiveConns", ( NERR_BASE + 302 ))
+NERR_BadPasswordCore = make_flag("NERR_BadPasswordCore", ( NERR_BASE + 303 ))
+NERR_DevInUse = make_flag("NERR_DevInUse", ( NERR_BASE + 304 ))
+NERR_LocalDrive = make_flag("NERR_LocalDrive", ( NERR_BASE + 305 ))
+NERR_AlertExists = make_flag("NERR_AlertExists", ( NERR_BASE + 330 ))
+NERR_TooManyAlerts = make_flag("NERR_TooManyAlerts", ( NERR_BASE + 331 ))
+NERR_NoSuchAlert = make_flag("NERR_NoSuchAlert", ( NERR_BASE + 332 ))
+NERR_BadRecipient = make_flag("NERR_BadRecipient", ( NERR_BASE + 333 ))
+NERR_AcctLimitExceeded = make_flag("NERR_AcctLimitExceeded", ( NERR_BASE + 334 ))
+NERR_InvalidLogSeek = make_flag("NERR_InvalidLogSeek", ( NERR_BASE + 340 ))
+NERR_BadUasConfig = make_flag("NERR_BadUasConfig", ( NERR_BASE + 350 ))
+NERR_InvalidUASOp = make_flag("NERR_InvalidUASOp", ( NERR_BASE + 351 ))
+NERR_LastAdmin = make_flag("NERR_LastAdmin", ( NERR_BASE + 352 ))
+NERR_DCNotFound = make_flag("NERR_DCNotFound", ( NERR_BASE + 353 ))
+NERR_LogonTrackingError = make_flag("NERR_LogonTrackingError", ( NERR_BASE + 354 ))
+NERR_NetlogonNotStarted = make_flag("NERR_NetlogonNotStarted", ( NERR_BASE + 355 ))
+NERR_CanNotGrowUASFile = make_flag("NERR_CanNotGrowUASFile", ( NERR_BASE + 356 ))
+NERR_TimeDiffAtDC = make_flag("NERR_TimeDiffAtDC", ( NERR_BASE + 357 ))
+NERR_PasswordMismatch = make_flag("NERR_PasswordMismatch", ( NERR_BASE + 358 ))
+NERR_NoSuchServer = make_flag("NERR_NoSuchServer", ( NERR_BASE + 360 ))
+NERR_NoSuchSession = make_flag("NERR_NoSuchSession", ( NERR_BASE + 361 ))
+NERR_NoSuchConnection = make_flag("NERR_NoSuchConnection", ( NERR_BASE + 362 ))
+NERR_TooManyServers = make_flag("NERR_TooManyServers", ( NERR_BASE + 363 ))
+NERR_TooManySessions = make_flag("NERR_TooManySessions", ( NERR_BASE + 364 ))
+NERR_TooManyConnections = make_flag("NERR_TooManyConnections", ( NERR_BASE + 365 ))
+NERR_TooManyFiles = make_flag("NERR_TooManyFiles", ( NERR_BASE + 366 ))
+NERR_NoAlternateServers = make_flag("NERR_NoAlternateServers", ( NERR_BASE + 367 ))
+NERR_TryDownLevel = make_flag("NERR_TryDownLevel", ( NERR_BASE + 370 ))
+NERR_UPSDriverNotStarted = make_flag("NERR_UPSDriverNotStarted", ( NERR_BASE + 380 ))
+NERR_UPSInvalidConfig = make_flag("NERR_UPSInvalidConfig", ( NERR_BASE + 381 ))
+NERR_UPSInvalidCommPort = make_flag("NERR_UPSInvalidCommPort", ( NERR_BASE + 382 ))
+NERR_UPSSignalAsserted = make_flag("NERR_UPSSignalAsserted", ( NERR_BASE + 383 ))
+NERR_UPSShutdownFailed = make_flag("NERR_UPSShutdownFailed", ( NERR_BASE + 384 ))
+NERR_BadDosRetCode = make_flag("NERR_BadDosRetCode", ( NERR_BASE + 400 ))
+NERR_ProgNeedsExtraMem = make_flag("NERR_ProgNeedsExtraMem", ( NERR_BASE + 401 ))
+NERR_BadDosFunction = make_flag("NERR_BadDosFunction", ( NERR_BASE + 402 ))
+NERR_RemoteBootFailed = make_flag("NERR_RemoteBootFailed", ( NERR_BASE + 403 ))
+NERR_BadFileCheckSum = make_flag("NERR_BadFileCheckSum", ( NERR_BASE + 404 ))
+NERR_NoRplBootSystem = make_flag("NERR_NoRplBootSystem", ( NERR_BASE + 405 ))
+NERR_RplLoadrNetBiosErr = make_flag("NERR_RplLoadrNetBiosErr", ( NERR_BASE + 406 ))
+NERR_RplLoadrDiskErr = make_flag("NERR_RplLoadrDiskErr", ( NERR_BASE + 407 ))
+NERR_ImageParamErr = make_flag("NERR_ImageParamErr", ( NERR_BASE + 408 ))
+NERR_TooManyImageParams = make_flag("NERR_TooManyImageParams", ( NERR_BASE + 409 ))
+NERR_NonDosFloppyUsed = make_flag("NERR_NonDosFloppyUsed", ( NERR_BASE + 410 ))
+NERR_RplBootRestart = make_flag("NERR_RplBootRestart", ( NERR_BASE + 411 ))
+NERR_RplSrvrCallFailed = make_flag("NERR_RplSrvrCallFailed", ( NERR_BASE + 412 ))
+NERR_CantConnectRplSrvr = make_flag("NERR_CantConnectRplSrvr", ( NERR_BASE + 413 ))
+NERR_CantOpenImageFile = make_flag("NERR_CantOpenImageFile", ( NERR_BASE + 414 ))
+NERR_CallingRplSrvr = make_flag("NERR_CallingRplSrvr", ( NERR_BASE + 415 ))
+NERR_StartingRplBoot = make_flag("NERR_StartingRplBoot", ( NERR_BASE + 416 ))
+NERR_RplBootServiceTerm = make_flag("NERR_RplBootServiceTerm", ( NERR_BASE + 417 ))
+NERR_RplBootStartFailed = make_flag("NERR_RplBootStartFailed", ( NERR_BASE + 418 ))
+NERR_RPL_CONNECTED = make_flag("NERR_RPL_CONNECTED", ( NERR_BASE + 419 ))
+NERR_BrowserConfiguredToNotRun = make_flag("NERR_BrowserConfiguredToNotRun", ( NERR_BASE + 450 ))
+NERR_RplNoAdaptersStarted = make_flag("NERR_RplNoAdaptersStarted", ( NERR_BASE + 510 ))
+NERR_RplBadRegistry = make_flag("NERR_RplBadRegistry", ( NERR_BASE + 511 ))
+NERR_RplBadDatabase = make_flag("NERR_RplBadDatabase", ( NERR_BASE + 512 ))
+NERR_RplRplfilesShare = make_flag("NERR_RplRplfilesShare", ( NERR_BASE + 513 ))
+NERR_RplNotRplServer = make_flag("NERR_RplNotRplServer", ( NERR_BASE + 514 ))
+NERR_RplCannotEnum = make_flag("NERR_RplCannotEnum", ( NERR_BASE + 515 ))
+NERR_RplWkstaInfoCorrupted = make_flag("NERR_RplWkstaInfoCorrupted", ( NERR_BASE + 516 ))
+NERR_RplWkstaNotFound = make_flag("NERR_RplWkstaNotFound", ( NERR_BASE + 517 ))
+NERR_RplWkstaNameUnavailable = make_flag("NERR_RplWkstaNameUnavailable", ( NERR_BASE + 518 ))
+NERR_RplProfileInfoCorrupted = make_flag("NERR_RplProfileInfoCorrupted", ( NERR_BASE + 519 ))
+NERR_RplProfileNotFound = make_flag("NERR_RplProfileNotFound", ( NERR_BASE + 520 ))
+NERR_RplProfileNameUnavailable = make_flag("NERR_RplProfileNameUnavailable", ( NERR_BASE + 521 ))
+NERR_RplProfileNotEmpty = make_flag("NERR_RplProfileNotEmpty", ( NERR_BASE + 522 ))
+NERR_RplConfigInfoCorrupted = make_flag("NERR_RplConfigInfoCorrupted", ( NERR_BASE + 523 ))
+NERR_RplConfigNotFound = make_flag("NERR_RplConfigNotFound", ( NERR_BASE + 524 ))
+NERR_RplAdapterInfoCorrupted = make_flag("NERR_RplAdapterInfoCorrupted", ( NERR_BASE + 525 ))
+NERR_RplInternal = make_flag("NERR_RplInternal", ( NERR_BASE + 526 ))
+NERR_RplVendorInfoCorrupted = make_flag("NERR_RplVendorInfoCorrupted", ( NERR_BASE + 527 ))
+NERR_RplBootInfoCorrupted = make_flag("NERR_RplBootInfoCorrupted", ( NERR_BASE + 528 ))
+NERR_RplWkstaNeedsUserAcct = make_flag("NERR_RplWkstaNeedsUserAcct", ( NERR_BASE + 529 ))
+NERR_RplNeedsRPLUSERAcct = make_flag("NERR_RplNeedsRPLUSERAcct", ( NERR_BASE + 530 ))
+NERR_RplBootNotFound = make_flag("NERR_RplBootNotFound", ( NERR_BASE + 531 ))
+NERR_RplIncompatibleProfile = make_flag("NERR_RplIncompatibleProfile", ( NERR_BASE + 532 ))
+NERR_RplAdapterNameUnavailable = make_flag("NERR_RplAdapterNameUnavailable", ( NERR_BASE + 533 ))
+NERR_RplConfigNotEmpty = make_flag("NERR_RplConfigNotEmpty", ( NERR_BASE + 534 ))
+NERR_RplBootInUse = make_flag("NERR_RplBootInUse", ( NERR_BASE + 535 ))
+NERR_RplBackupDatabase = make_flag("NERR_RplBackupDatabase", ( NERR_BASE + 536 ))
+NERR_RplAdapterNotFound = make_flag("NERR_RplAdapterNotFound", ( NERR_BASE + 537 ))
+NERR_RplVendorNotFound = make_flag("NERR_RplVendorNotFound", ( NERR_BASE + 538 ))
+NERR_RplVendorNameUnavailable = make_flag("NERR_RplVendorNameUnavailable", ( NERR_BASE + 539 ))
+NERR_RplBootNameUnavailable = make_flag("NERR_RplBootNameUnavailable", ( NERR_BASE + 540 ))
+NERR_RplConfigNameUnavailable = make_flag("NERR_RplConfigNameUnavailable", ( NERR_BASE + 541 ))
+NERR_DfsInternalCorruption = make_flag("NERR_DfsInternalCorruption", ( NERR_BASE + 560 ))
+NERR_DfsVolumeDataCorrupt = make_flag("NERR_DfsVolumeDataCorrupt", ( NERR_BASE + 561 ))
+NERR_DfsNoSuchVolume = make_flag("NERR_DfsNoSuchVolume", ( NERR_BASE + 562 ))
+NERR_DfsVolumeAlreadyExists = make_flag("NERR_DfsVolumeAlreadyExists", ( NERR_BASE + 563 ))
+NERR_DfsAlreadyShared = make_flag("NERR_DfsAlreadyShared", ( NERR_BASE + 564 ))
+NERR_DfsNoSuchShare = make_flag("NERR_DfsNoSuchShare", ( NERR_BASE + 565 ))
+NERR_DfsNotALeafVolume = make_flag("NERR_DfsNotALeafVolume", ( NERR_BASE + 566 ))
+NERR_DfsLeafVolume = make_flag("NERR_DfsLeafVolume", ( NERR_BASE + 567 ))
+NERR_DfsVolumeHasMultipleServers = make_flag("NERR_DfsVolumeHasMultipleServers", ( NERR_BASE + 568 ))
+NERR_DfsCantCreateJunctionPoint = make_flag("NERR_DfsCantCreateJunctionPoint", ( NERR_BASE + 569 ))
+NERR_DfsServerNotDfsAware = make_flag("NERR_DfsServerNotDfsAware", ( NERR_BASE + 570 ))
+NERR_DfsBadRenamePath = make_flag("NERR_DfsBadRenamePath", ( NERR_BASE + 571 ))
+NERR_DfsVolumeIsOffline = make_flag("NERR_DfsVolumeIsOffline", ( NERR_BASE + 572 ))
+NERR_DfsNoSuchServer = make_flag("NERR_DfsNoSuchServer", ( NERR_BASE + 573 ))
+NERR_DfsCyclicalName = make_flag("NERR_DfsCyclicalName", ( NERR_BASE + 574 ))
+NERR_DfsNotSupportedInServerDfs = make_flag("NERR_DfsNotSupportedInServerDfs", ( NERR_BASE + 575 ))
+NERR_DfsDuplicateService = make_flag("NERR_DfsDuplicateService", ( NERR_BASE + 576 ))
+NERR_DfsCantRemoveLastServerShare = make_flag("NERR_DfsCantRemoveLastServerShare", ( NERR_BASE + 577 ))
+NERR_DfsVolumeIsInterDfs = make_flag("NERR_DfsVolumeIsInterDfs", ( NERR_BASE + 578 ))
+NERR_DfsInconsistent = make_flag("NERR_DfsInconsistent", ( NERR_BASE + 579 ))
+NERR_DfsServerUpgraded = make_flag("NERR_DfsServerUpgraded", ( NERR_BASE + 580 ))
+NERR_DfsDataIsIdentical = make_flag("NERR_DfsDataIsIdentical", ( NERR_BASE + 581 ))
+NERR_DfsCantRemoveDfsRoot = make_flag("NERR_DfsCantRemoveDfsRoot", ( NERR_BASE + 582 ))
+NERR_DfsChildOrParentInDfs = make_flag("NERR_DfsChildOrParentInDfs", ( NERR_BASE + 583 ))
+NERR_DfsInternalError = make_flag("NERR_DfsInternalError", ( NERR_BASE + 590 ))
+NERR_SetupAlreadyJoined = make_flag("NERR_SetupAlreadyJoined", ( NERR_BASE + 591 ))
+NERR_SetupNotJoined = make_flag("NERR_SetupNotJoined", ( NERR_BASE + 592 ))
+NERR_SetupDomainController = make_flag("NERR_SetupDomainController", ( NERR_BASE + 593 ))
+NERR_DefaultJoinRequired = make_flag("NERR_DefaultJoinRequired", ( NERR_BASE + 594 ))
+NERR_InvalidWorkgroupName = make_flag("NERR_InvalidWorkgroupName", ( NERR_BASE + 595 ))
+NERR_NameUsesIncompatibleCodePage = make_flag("NERR_NameUsesIncompatibleCodePage", ( NERR_BASE + 596 ))
+NERR_ComputerAccountNotFound = make_flag("NERR_ComputerAccountNotFound", ( NERR_BASE + 597 ))
+NERR_PersonalSku = make_flag("NERR_PersonalSku", ( NERR_BASE + 598 ))
+NERR_SetupCheckDNSConfig = make_flag("NERR_SetupCheckDNSConfig", ( NERR_BASE + 599 ))
+NERR_AlreadyCloudDomainJoined = make_flag("NERR_AlreadyCloudDomainJoined", ( NERR_BASE + 600 ))
+NERR_PasswordMustChange = make_flag("NERR_PasswordMustChange", ( NERR_BASE + 601 ))
+NERR_AccountLockedOut = make_flag("NERR_AccountLockedOut", ( NERR_BASE + 602 ))
+NERR_PasswordTooLong = make_flag("NERR_PasswordTooLong", ( NERR_BASE + 603 ))
+NERR_PasswordNotComplexEnough = make_flag("NERR_PasswordNotComplexEnough", ( NERR_BASE + 604 ))
+NERR_PasswordFilterError = make_flag("NERR_PasswordFilterError", ( NERR_BASE + 605 ))
+NERR_NoOfflineJoinInfo = make_flag("NERR_NoOfflineJoinInfo", ( NERR_BASE + 609 ))
+NERR_BadOfflineJoinInfo = make_flag("NERR_BadOfflineJoinInfo", ( NERR_BASE + 610 ))
+NERR_CantCreateJoinInfo = make_flag("NERR_CantCreateJoinInfo", ( NERR_BASE + 611 ))
+NERR_BadDomainJoinInfo = make_flag("NERR_BadDomainJoinInfo", ( NERR_BASE + 612 ))
+NERR_JoinPerformedMustRestart = make_flag("NERR_JoinPerformedMustRestart", ( NERR_BASE + 613 ))
+NERR_NoJoinPending = make_flag("NERR_NoJoinPending", ( NERR_BASE + 614 ))
+NERR_ValuesNotSet = make_flag("NERR_ValuesNotSet", ( NERR_BASE + 615 ))
+NERR_CantVerifyHostname = make_flag("NERR_CantVerifyHostname", ( NERR_BASE + 616 ))
+NERR_CantLoadOfflineHive = make_flag("NERR_CantLoadOfflineHive", ( NERR_BASE + 617 ))
+NERR_ConnectionInsecure = make_flag("NERR_ConnectionInsecure", ( NERR_BASE + 618 ))
+NERR_ProvisioningBlobUnsupported = make_flag("NERR_ProvisioningBlobUnsupported", ( NERR_BASE + 619 ))
+NERR_DS8DCRequired = make_flag("NERR_DS8DCRequired", ( NERR_BASE + 620 ))
+NERR_LDAPCapableDCRequired = make_flag("NERR_LDAPCapableDCRequired", ( NERR_BASE + 621 ))
+NERR_DS8DCNotFound = make_flag("NERR_DS8DCNotFound", ( NERR_BASE + 622 ))
+NERR_TargetVersionUnsupported = make_flag("NERR_TargetVersionUnsupported", ( NERR_BASE + 623 ))
+NERR_InvalidMachineNameForJoin = make_flag("NERR_InvalidMachineNameForJoin", ( NERR_BASE + 624 ))
+NERR_DS9DCNotFound = make_flag("NERR_DS9DCNotFound", ( NERR_BASE + 625 ))
+NERR_PlainTextSecretsRequired = make_flag("NERR_PlainTextSecretsRequired", ( NERR_BASE + 626 ))
+NERR_CannotUnjoinAadDomain = make_flag("NERR_CannotUnjoinAadDomain", ( NERR_BASE + 627 ))
+MAX_NERR = make_flag("MAX_NERR", ( NERR_BASE + 899 ))
 ATM_E164 = make_flag("ATM_E164", 0x01)
 ATM_NSAP = make_flag("ATM_NSAP", 0x02)
 ATM_AESA = make_flag("ATM_AESA", 0x02)
 ATM_ADDR_SIZE = make_flag("ATM_ADDR_SIZE", 20)
 DNS_ATMA_FORMAT_E164 = make_flag("DNS_ATMA_FORMAT_E164", ATM_E164)
 DNS_ATMA_FORMAT_AESA = make_flag("DNS_ATMA_FORMAT_AESA", ATM_AESA)
 DNS_ATMA_MAX_ADDR_LENGTH = make_flag("DNS_ATMA_MAX_ADDR_LENGTH", ATM_ADDR_SIZE)
+DNS_ADDR_MAX_SOCKADDR_LENGTH = make_flag("DNS_ADDR_MAX_SOCKADDR_LENGTH", ( 32 ))
 DNS_TYPE_ZERO = make_flag("DNS_TYPE_ZERO", 0x0000)
 DNS_TYPE_A = make_flag("DNS_TYPE_A", 0x0001)
 DNS_TYPE_NS = make_flag("DNS_TYPE_NS", 0x0002)
 DNS_TYPE_MD = make_flag("DNS_TYPE_MD", 0x0003)
 DNS_TYPE_MF = make_flag("DNS_TYPE_MF", 0x0004)
 DNS_TYPE_CNAME = make_flag("DNS_TYPE_CNAME", 0x0005)
 DNS_TYPE_SOA = make_flag("DNS_TYPE_SOA", 0x0006)
@@ -672,14 +1071,23 @@
 DNS_QUERY_DUAL_ADDR = make_flag("DNS_QUERY_DUAL_ADDR", 0x00004000)
 DNS_QUERY_DONT_RESET_TTL_VALUES = make_flag("DNS_QUERY_DONT_RESET_TTL_VALUES", 0x00100000)
 DNS_QUERY_DISABLE_IDN_ENCODING = make_flag("DNS_QUERY_DISABLE_IDN_ENCODING", 0x00200000)
 DNS_QUERY_APPEND_MULTILABEL = make_flag("DNS_QUERY_APPEND_MULTILABEL", 0x00800000)
 DNS_QUERY_DNSSEC_OK = make_flag("DNS_QUERY_DNSSEC_OK", 0x01000000)
 DNS_QUERY_DNSSEC_CHECKING_DISABLED = make_flag("DNS_QUERY_DNSSEC_CHECKING_DISABLED", 0x02000000)
 DNS_QUERY_RESERVED = make_flag("DNS_QUERY_RESERVED", 0xf0000000)
+MAX_ADAPTER_DESCRIPTION_LENGTH = make_flag("MAX_ADAPTER_DESCRIPTION_LENGTH", 128)
+MAX_ADAPTER_NAME_LENGTH = make_flag("MAX_ADAPTER_NAME_LENGTH", 256)
+MAX_ADAPTER_ADDRESS_LENGTH = make_flag("MAX_ADAPTER_ADDRESS_LENGTH", 8)
+DEFAULT_MINIMUM_ENTITIES = make_flag("DEFAULT_MINIMUM_ENTITIES", 32)
+MAX_HOSTNAME_LEN = make_flag("MAX_HOSTNAME_LEN", 128)
+MAX_DOMAIN_NAME_LEN = make_flag("MAX_DOMAIN_NAME_LEN", 128)
+MAX_SCOPE_ID_LEN = make_flag("MAX_SCOPE_ID_LEN", 256)
+MAX_DHCPV6_DUID_LENGTH = make_flag("MAX_DHCPV6_DUID_LENGTH", 130)
+MAX_DNS_SUFFIX_STRING_LENGTH = make_flag("MAX_DNS_SUFFIX_STRING_LENGTH", 256)
 PIPE_ACCESS_INBOUND = make_flag("PIPE_ACCESS_INBOUND", 0x00000001)
 PIPE_ACCESS_OUTBOUND = make_flag("PIPE_ACCESS_OUTBOUND", 0x00000002)
 PIPE_ACCESS_DUPLEX = make_flag("PIPE_ACCESS_DUPLEX", 0x00000003)
 PIPE_CLIENT_END = make_flag("PIPE_CLIENT_END", 0x00000000)
 PIPE_SERVER_END = make_flag("PIPE_SERVER_END", 0x00000001)
 PIPE_WAIT = make_flag("PIPE_WAIT", 0x00000000)
 PIPE_NOWAIT = make_flag("PIPE_NOWAIT", 0x00000001)
@@ -804,14 +1212,15 @@
 SCOPE_SECURITY_INFORMATION = make_flag("SCOPE_SECURITY_INFORMATION", ( 0x00000040 ))
 PROCESS_TRUST_LABEL_SECURITY_INFORMATION = make_flag("PROCESS_TRUST_LABEL_SECURITY_INFORMATION", ( 0x00000080 ))
 BACKUP_SECURITY_INFORMATION = make_flag("BACKUP_SECURITY_INFORMATION", ( 0x00010000 ))
 PROTECTED_DACL_SECURITY_INFORMATION = make_flag("PROTECTED_DACL_SECURITY_INFORMATION", ( 0x80000000 ))
 PROTECTED_SACL_SECURITY_INFORMATION = make_flag("PROTECTED_SACL_SECURITY_INFORMATION", ( 0x40000000 ))
 UNPROTECTED_DACL_SECURITY_INFORMATION = make_flag("UNPROTECTED_DACL_SECURITY_INFORMATION", ( 0x20000000 ))
 UNPROTECTED_SACL_SECURITY_INFORMATION = make_flag("UNPROTECTED_SACL_SECURITY_INFORMATION", ( 0x10000000 ))
+SECURITY_DESCRIPTOR_REVISION = make_flag("SECURITY_DESCRIPTOR_REVISION", 1)
 SERVICE_TRIGGER_TYPE_DEVICE_INTERFACE_ARRIVAL = make_flag("SERVICE_TRIGGER_TYPE_DEVICE_INTERFACE_ARRIVAL", 1)
 SERVICE_TRIGGER_TYPE_IP_ADDRESS_AVAILABILITY = make_flag("SERVICE_TRIGGER_TYPE_IP_ADDRESS_AVAILABILITY", 2)
 SERVICE_TRIGGER_TYPE_DOMAIN_JOIN = make_flag("SERVICE_TRIGGER_TYPE_DOMAIN_JOIN", 3)
 SERVICE_TRIGGER_TYPE_FIREWALL_PORT_EVENT = make_flag("SERVICE_TRIGGER_TYPE_FIREWALL_PORT_EVENT", 4)
 SERVICE_TRIGGER_TYPE_GROUP_POLICY = make_flag("SERVICE_TRIGGER_TYPE_GROUP_POLICY", 5)
 SERVICE_TRIGGER_TYPE_NETWORK_ENDPOINT = make_flag("SERVICE_TRIGGER_TYPE_NETWORK_ENDPOINT", 6)
 SERVICE_TRIGGER_TYPE_CUSTOM_SYSTEM_STATE_CHANGE = make_flag("SERVICE_TRIGGER_TYPE_CUSTOM_SYSTEM_STATE_CHANGE", 7)
@@ -1475,44 +1884,14 @@
 SYNCHRONIZE = make_flag("SYNCHRONIZE", ( 0x00100000 ))
 STANDARD_RIGHTS_REQUIRED = make_flag("STANDARD_RIGHTS_REQUIRED", ( 0x000F0000 ))
 STANDARD_RIGHTS_READ = make_flag("STANDARD_RIGHTS_READ", ( READ_CONTROL ))
 STANDARD_RIGHTS_WRITE = make_flag("STANDARD_RIGHTS_WRITE", ( READ_CONTROL ))
 STANDARD_RIGHTS_EXECUTE = make_flag("STANDARD_RIGHTS_EXECUTE", ( READ_CONTROL ))
 STANDARD_RIGHTS_ALL = make_flag("STANDARD_RIGHTS_ALL", ( 0x001F0000 ))
 SPECIFIC_RIGHTS_ALL = make_flag("SPECIFIC_RIGHTS_ALL", ( 0x0000FFFF ))
-AF_UNSPEC = make_flag("AF_UNSPEC", 0)
-AF_UNIX = make_flag("AF_UNIX", 1)
-AF_INET = make_flag("AF_INET", 2)
-AF_IMPLINK = make_flag("AF_IMPLINK", 3)
-AF_PUP = make_flag("AF_PUP", 4)
-AF_CHAOS = make_flag("AF_CHAOS", 5)
-AF_NS = make_flag("AF_NS", 6)
-AF_IPX = make_flag("AF_IPX", AF_NS)
-AF_ISO = make_flag("AF_ISO", 7)
-AF_OSI = make_flag("AF_OSI", AF_ISO)
-AF_ECMA = make_flag("AF_ECMA", 8)
-AF_DATAKIT = make_flag("AF_DATAKIT", 9)
-AF_CCITT = make_flag("AF_CCITT", 10)
-AF_SNA = make_flag("AF_SNA", 11)
-AF_DECnet = make_flag("AF_DECnet", 12)
-AF_DLI = make_flag("AF_DLI", 13)
-AF_LAT = make_flag("AF_LAT", 14)
-AF_HYLINK = make_flag("AF_HYLINK", 15)
-AF_APPLETALK = make_flag("AF_APPLETALK", 16)
-AF_NETBIOS = make_flag("AF_NETBIOS", 17)
-AF_VOICEVIEW = make_flag("AF_VOICEVIEW", 18)
-AF_FIREFOX = make_flag("AF_FIREFOX", 19)
-AF_UNKNOWN1 = make_flag("AF_UNKNOWN1", 20)
-AF_BAN = make_flag("AF_BAN", 21)
-AF_ATM = make_flag("AF_ATM", 22)
-AF_INET6 = make_flag("AF_INET6", 23)
-AF_CLUSTER = make_flag("AF_CLUSTER", 24)
-AF_12844 = make_flag("AF_12844", 25)
-AF_IRDA = make_flag("AF_IRDA", 26)
-AF_NETDES = make_flag("AF_NETDES", 28)
 EXCEPTION_NONCONTINUABLE = make_flag("EXCEPTION_NONCONTINUABLE", 0x1)
 EXCEPTION_MAXIMUM_PARAMETERS = make_flag("EXCEPTION_MAXIMUM_PARAMETERS", 15)
 EXCEPTION_EXECUTE_HANDLER = make_flag("EXCEPTION_EXECUTE_HANDLER", 1)
 EXCEPTION_CONTINUE_SEARCH = make_flag("EXCEPTION_CONTINUE_SEARCH", 0)
 EXCEPTION_CONTINUE_EXECUTION = make_flag("EXCEPTION_CONTINUE_EXECUTION", -1)
 GENERIC_READ = make_flag("GENERIC_READ", ( 0x80000000 ))
 GENERIC_WRITE = make_flag("GENERIC_WRITE", ( 0x40000000 ))
@@ -1530,67 +1909,16 @@
 FILE_FLAG_OPEN_NO_RECALL = make_flag("FILE_FLAG_OPEN_NO_RECALL", 0x00100000)
 FILE_FLAG_FIRST_PIPE_INSTANCE = make_flag("FILE_FLAG_FIRST_PIPE_INSTANCE", 0x00080000)
 CREATE_NEW = make_flag("CREATE_NEW", 1)
 CREATE_ALWAYS = make_flag("CREATE_ALWAYS", 2)
 OPEN_EXISTING = make_flag("OPEN_EXISTING", 3)
 OPEN_ALWAYS = make_flag("OPEN_ALWAYS", 4)
 TRUNCATE_EXISTING = make_flag("TRUNCATE_EXISTING", 5)
-FILE_SHARE_READ = make_flag("FILE_SHARE_READ", 0x00000001)
-FILE_SHARE_WRITE = make_flag("FILE_SHARE_WRITE", 0x00000002)
-FILE_SHARE_DELETE = make_flag("FILE_SHARE_DELETE", 0x00000004)
-FILE_ATTRIBUTE_READONLY = make_flag("FILE_ATTRIBUTE_READONLY", 0x00000001)
-FILE_ATTRIBUTE_HIDDEN = make_flag("FILE_ATTRIBUTE_HIDDEN", 0x00000002)
-FILE_ATTRIBUTE_SYSTEM = make_flag("FILE_ATTRIBUTE_SYSTEM", 0x00000004)
-FILE_ATTRIBUTE_DIRECTORY = make_flag("FILE_ATTRIBUTE_DIRECTORY", 0x00000010)
-FILE_ATTRIBUTE_ARCHIVE = make_flag("FILE_ATTRIBUTE_ARCHIVE", 0x00000020)
-FILE_ATTRIBUTE_DEVICE = make_flag("FILE_ATTRIBUTE_DEVICE", 0x00000040)
-FILE_ATTRIBUTE_NORMAL = make_flag("FILE_ATTRIBUTE_NORMAL", 0x00000080)
-FILE_ATTRIBUTE_TEMPORARY = make_flag("FILE_ATTRIBUTE_TEMPORARY", 0x00000100)
-FILE_ATTRIBUTE_SPARSE_FILE = make_flag("FILE_ATTRIBUTE_SPARSE_FILE", 0x00000200)
-FILE_ATTRIBUTE_REPARSE_POINT = make_flag("FILE_ATTRIBUTE_REPARSE_POINT", 0x00000400)
-FILE_ATTRIBUTE_COMPRESSED = make_flag("FILE_ATTRIBUTE_COMPRESSED", 0x00000800)
-FILE_ATTRIBUTE_OFFLINE = make_flag("FILE_ATTRIBUTE_OFFLINE", 0x00001000)
-FILE_ATTRIBUTE_NOT_CONTENT_INDEXED = make_flag("FILE_ATTRIBUTE_NOT_CONTENT_INDEXED", 0x00002000)
-FILE_ATTRIBUTE_ENCRYPTED = make_flag("FILE_ATTRIBUTE_ENCRYPTED", 0x00004000)
-FILE_ATTRIBUTE_VIRTUAL = make_flag("FILE_ATTRIBUTE_VIRTUAL", 0x00010000)
-FILE_NOTIFY_CHANGE_FILE_NAME = make_flag("FILE_NOTIFY_CHANGE_FILE_NAME", 0x00000001)
-FILE_NOTIFY_CHANGE_DIR_NAME = make_flag("FILE_NOTIFY_CHANGE_DIR_NAME", 0x00000002)
-FILE_NOTIFY_CHANGE_ATTRIBUTES = make_flag("FILE_NOTIFY_CHANGE_ATTRIBUTES", 0x00000004)
-FILE_NOTIFY_CHANGE_SIZE = make_flag("FILE_NOTIFY_CHANGE_SIZE", 0x00000008)
-FILE_NOTIFY_CHANGE_LAST_WRITE = make_flag("FILE_NOTIFY_CHANGE_LAST_WRITE", 0x00000010)
-FILE_NOTIFY_CHANGE_LAST_ACCESS = make_flag("FILE_NOTIFY_CHANGE_LAST_ACCESS", 0x00000020)
-FILE_NOTIFY_CHANGE_CREATION = make_flag("FILE_NOTIFY_CHANGE_CREATION", 0x00000040)
-FILE_NOTIFY_CHANGE_SECURITY = make_flag("FILE_NOTIFY_CHANGE_SECURITY", 0x00000100)
-FILE_ACTION_ADDED = make_flag("FILE_ACTION_ADDED", 0x00000001)
-FILE_ACTION_REMOVED = make_flag("FILE_ACTION_REMOVED", 0x00000002)
-FILE_ACTION_MODIFIED = make_flag("FILE_ACTION_MODIFIED", 0x00000003)
-FILE_ACTION_RENAMED_OLD_NAME = make_flag("FILE_ACTION_RENAMED_OLD_NAME", 0x00000004)
-FILE_ACTION_RENAMED_NEW_NAME = make_flag("FILE_ACTION_RENAMED_NEW_NAME", 0x00000005)
 MAILSLOT_NO_MESSAGE = make_flag("MAILSLOT_NO_MESSAGE", ( -1 ))
 MAILSLOT_WAIT_FOREVER = make_flag("MAILSLOT_WAIT_FOREVER", ( -1 ))
-FILE_CASE_SENSITIVE_SEARCH = make_flag("FILE_CASE_SENSITIVE_SEARCH", 0x00000001)
-FILE_CASE_PRESERVED_NAMES = make_flag("FILE_CASE_PRESERVED_NAMES", 0x00000002)
-FILE_UNICODE_ON_DISK = make_flag("FILE_UNICODE_ON_DISK", 0x00000004)
-FILE_PERSISTENT_ACLS = make_flag("FILE_PERSISTENT_ACLS", 0x00000008)
-FILE_FILE_COMPRESSION = make_flag("FILE_FILE_COMPRESSION", 0x00000010)
-FILE_VOLUME_QUOTAS = make_flag("FILE_VOLUME_QUOTAS", 0x00000020)
-FILE_SUPPORTS_SPARSE_FILES = make_flag("FILE_SUPPORTS_SPARSE_FILES", 0x00000040)
-FILE_SUPPORTS_REPARSE_POINTS = make_flag("FILE_SUPPORTS_REPARSE_POINTS", 0x00000080)
-FILE_SUPPORTS_REMOTE_STORAGE = make_flag("FILE_SUPPORTS_REMOTE_STORAGE", 0x00000100)
-FILE_VOLUME_IS_COMPRESSED = make_flag("FILE_VOLUME_IS_COMPRESSED", 0x00008000)
-FILE_SUPPORTS_OBJECT_IDS = make_flag("FILE_SUPPORTS_OBJECT_IDS", 0x00010000)
-FILE_SUPPORTS_ENCRYPTION = make_flag("FILE_SUPPORTS_ENCRYPTION", 0x00020000)
-FILE_NAMED_STREAMS = make_flag("FILE_NAMED_STREAMS", 0x00040000)
-FILE_READ_ONLY_VOLUME = make_flag("FILE_READ_ONLY_VOLUME", 0x00080000)
-FILE_SEQUENTIAL_WRITE_ONCE = make_flag("FILE_SEQUENTIAL_WRITE_ONCE", 0x00100000)
-FILE_SUPPORTS_TRANSACTIONS = make_flag("FILE_SUPPORTS_TRANSACTIONS", 0x00200000)
-FILE_SUPPORTS_HARD_LINKS = make_flag("FILE_SUPPORTS_HARD_LINKS", 0x00400000)
-FILE_SUPPORTS_EXTENDED_ATTRIBUTES = make_flag("FILE_SUPPORTS_EXTENDED_ATTRIBUTES", 0x00800000)
-FILE_SUPPORTS_OPEN_BY_FILE_ID = make_flag("FILE_SUPPORTS_OPEN_BY_FILE_ID", 0x01000000)
-FILE_SUPPORTS_USN_JOURNAL = make_flag("FILE_SUPPORTS_USN_JOURNAL", 0x02000000)
 RRF_RT_REG_NONE = make_flag("RRF_RT_REG_NONE", 0x00000001)
 RRF_RT_REG_SZ = make_flag("RRF_RT_REG_SZ", 0x00000002)
 RRF_RT_REG_EXPAND_SZ = make_flag("RRF_RT_REG_EXPAND_SZ", 0x00000004)
 RRF_RT_REG_BINARY = make_flag("RRF_RT_REG_BINARY", 0x00000008)
 RRF_RT_REG_DWORD = make_flag("RRF_RT_REG_DWORD", 0x00000010)
 RRF_RT_REG_MULTI_SZ = make_flag("RRF_RT_REG_MULTI_SZ", 0x00000020)
 RRF_RT_REG_QWORD = make_flag("RRF_RT_REG_QWORD", 0x00000040)
@@ -2732,7 +3060,75 @@
 CMSG_CTRL_DEL_ATTR_CERT = make_flag("CMSG_CTRL_DEL_ATTR_CERT", 15)
 CMSG_CTRL_KEY_TRANS_DECRYPT = make_flag("CMSG_CTRL_KEY_TRANS_DECRYPT", 16)
 CMSG_CTRL_KEY_AGREE_DECRYPT = make_flag("CMSG_CTRL_KEY_AGREE_DECRYPT", 17)
 CMSG_CTRL_MAIL_LIST_DECRYPT = make_flag("CMSG_CTRL_MAIL_LIST_DECRYPT", 18)
 CMSG_CTRL_VERIFY_SIGNATURE_EX = make_flag("CMSG_CTRL_VERIFY_SIGNATURE_EX", 19)
 CMSG_CTRL_ADD_CMS_SIGNER_INFO = make_flag("CMSG_CTRL_ADD_CMS_SIGNER_INFO", 20)
 CMSG_CTRL_ENABLE_STRONG_SIGNATURE = make_flag("CMSG_CTRL_ENABLE_STRONG_SIGNATURE", 21)
+WSADESCRIPTION_LEN = make_flag("WSADESCRIPTION_LEN", 256)
+WSASYS_STATUS_LEN = make_flag("WSASYS_STATUS_LEN", 128)
+WSAPROTOCOL_LEN = make_flag("WSAPROTOCOL_LEN", 255)
+MAX_PROTOCOL_CHAIN = make_flag("MAX_PROTOCOL_CHAIN", 7)
+BASE_PROTOCOL = make_flag("BASE_PROTOCOL", 1)
+LAYERED_PROTOCOL = make_flag("LAYERED_PROTOCOL", 0)
+INVALID_SOCKET32 = make_flag("INVALID_SOCKET32", ( 0xffffffff ))
+INVALID_SOCKET64 = make_flag("INVALID_SOCKET64", ( 0xffffffffffffffff ))
+SOCKET_ERROR = make_flag("SOCKET_ERROR", ( -1 ))
+SOCK_STREAM = make_flag("SOCK_STREAM", 1)
+SOCK_DGRAM = make_flag("SOCK_DGRAM", 2)
+SOCK_RAW = make_flag("SOCK_RAW", 3)
+SOCK_RDM = make_flag("SOCK_RDM", 4)
+SOCK_SEQPACKET = make_flag("SOCK_SEQPACKET", 5)
+IPPROTO_IP = make_flag("IPPROTO_IP", 0)
+IPPROTO_ICMP = make_flag("IPPROTO_ICMP", 1)
+IPPROTO_IGMP = make_flag("IPPROTO_IGMP", 2)
+IPPROTO_GGP = make_flag("IPPROTO_GGP", 3)
+IPPROTO_TCP = make_flag("IPPROTO_TCP", 6)
+IPPROTO_PUP = make_flag("IPPROTO_PUP", 12)
+IPPROTO_UDP = make_flag("IPPROTO_UDP", 17)
+IPPROTO_IDP = make_flag("IPPROTO_IDP", 22)
+IPPROTO_ND = make_flag("IPPROTO_ND", 77)
+IPPROTO_RAW = make_flag("IPPROTO_RAW", 255)
+IPPROTO_MAX = make_flag("IPPROTO_MAX", 256)
+IPPORT_ECHO = make_flag("IPPORT_ECHO", 7)
+IPPORT_DISCARD = make_flag("IPPORT_DISCARD", 9)
+IPPORT_SYSTAT = make_flag("IPPORT_SYSTAT", 11)
+IPPORT_DAYTIME = make_flag("IPPORT_DAYTIME", 13)
+IPPORT_NETSTAT = make_flag("IPPORT_NETSTAT", 15)
+IPPORT_FTP = make_flag("IPPORT_FTP", 21)
+IPPORT_TELNET = make_flag("IPPORT_TELNET", 23)
+IPPORT_SMTP = make_flag("IPPORT_SMTP", 25)
+IPPORT_TIMESERVER = make_flag("IPPORT_TIMESERVER", 37)
+IPPORT_NAMESERVER = make_flag("IPPORT_NAMESERVER", 42)
+IPPORT_WHOIS = make_flag("IPPORT_WHOIS", 43)
+IPPORT_MTP = make_flag("IPPORT_MTP", 57)
+AF_UNSPEC = make_flag("AF_UNSPEC", 0)
+AF_UNIX = make_flag("AF_UNIX", 1)
+AF_INET = make_flag("AF_INET", 2)
+AF_IMPLINK = make_flag("AF_IMPLINK", 3)
+AF_PUP = make_flag("AF_PUP", 4)
+AF_CHAOS = make_flag("AF_CHAOS", 5)
+AF_IPX = make_flag("AF_IPX", 6)
+AF_NS = make_flag("AF_NS", 6)
+AF_ISO = make_flag("AF_ISO", 7)
+AF_OSI = make_flag("AF_OSI", AF_ISO)
+AF_ECMA = make_flag("AF_ECMA", 8)
+AF_DATAKIT = make_flag("AF_DATAKIT", 9)
+AF_CCITT = make_flag("AF_CCITT", 10)
+AF_SNA = make_flag("AF_SNA", 11)
+AF_DECnet = make_flag("AF_DECnet", 12)
+AF_DLI = make_flag("AF_DLI", 13)
+AF_LAT = make_flag("AF_LAT", 14)
+AF_HYLINK = make_flag("AF_HYLINK", 15)
+AF_APPLETALK = make_flag("AF_APPLETALK", 16)
+AF_NETBIOS = make_flag("AF_NETBIOS", 17)
+AF_VOICEVIEW = make_flag("AF_VOICEVIEW", 18)
+AF_FIREFOX = make_flag("AF_FIREFOX", 19)
+AF_UNKNOWN1 = make_flag("AF_UNKNOWN1", 20)
+AF_BAN = make_flag("AF_BAN", 21)
+AF_ATM = make_flag("AF_ATM", 22)
+AF_INET6 = make_flag("AF_INET6", 23)
+AF_CLUSTER = make_flag("AF_CLUSTER", 24)
+AF_12844 = make_flag("AF_12844", 25)
+AF_IRDA = make_flag("AF_IRDA", 26)
+AF_NETDES = make_flag("AF_NETDES", 28)
+AF_MAX = make_flag("AF_MAX", 22)
```

### Comparing `PythonForWindows-0.6.5/windows/generated_def/winerror.py` & `PythonForWindows-0.6.8/windows/generated_def/winerror.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/generated_def/winfuncs.py` & `PythonForWindows-0.6.8/windows/generated_def/winfuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,14 +326,94 @@
 CLSIDFromProgIDParams = ((1, 'lpszProgID'), (1, 'lpclsid'))
 
 #def CoTaskMemFree(pv):
 #    return CoTaskMemFree.ctypes_function(pv)
 CoTaskMemFreePrototype = WINFUNCTYPE(PVOID, LPVOID)
 CoTaskMemFreeParams = ((1, 'pv'),)
 
+#def SafeArrayCreate(vt, cDims, rgsabound):
+#    return SafeArrayCreate.ctypes_function(vt, cDims, rgsabound)
+SafeArrayCreatePrototype = WINFUNCTYPE(LPSAFEARRAY, VARTYPE, UINT, POINTER(SAFEARRAYBOUND))
+SafeArrayCreateParams = ((1, 'vt'), (1, 'cDims'), (1, 'rgsabound'))
+
+#def SafeArrayCreateVector(vt, lLbound, cElements):
+#    return SafeArrayCreateVector.ctypes_function(vt, lLbound, cElements)
+SafeArrayCreateVectorPrototype = WINFUNCTYPE(LPSAFEARRAY, VARTYPE, LONG, ULONG)
+SafeArrayCreateVectorParams = ((1, 'vt'), (1, 'lLbound'), (1, 'cElements'))
+
+#def SafeArrayDestroy(psa):
+#    return SafeArrayDestroy.ctypes_function(psa)
+SafeArrayDestroyPrototype = WINFUNCTYPE(HRESULT, POINTER(SAFEARRAY))
+SafeArrayDestroyParams = ((1, 'psa'),)
+
+#def SafeArrayDestroyData(psa):
+#    return SafeArrayDestroyData.ctypes_function(psa)
+SafeArrayDestroyDataPrototype = WINFUNCTYPE(HRESULT, POINTER(SAFEARRAY))
+SafeArrayDestroyDataParams = ((1, 'psa'),)
+
+#def SafeArrayGetElement(psa, rgIndices, pv):
+#    return SafeArrayGetElement.ctypes_function(psa, rgIndices, pv)
+SafeArrayGetElementPrototype = WINFUNCTYPE(HRESULT, POINTER(SAFEARRAY), POINTER(LONG), PVOID)
+SafeArrayGetElementParams = ((1, 'psa'), (1, 'rgIndices'), (1, 'pv'))
+
+#def SafeArrayGetElemsize(psa):
+#    return SafeArrayGetElemsize.ctypes_function(psa)
+SafeArrayGetElemsizePrototype = WINFUNCTYPE(UINT, POINTER(SAFEARRAY))
+SafeArrayGetElemsizeParams = ((1, 'psa'),)
+
+#def SafeArrayGetLBound(psa, nDim, plLbound):
+#    return SafeArrayGetLBound.ctypes_function(psa, nDim, plLbound)
+SafeArrayGetLBoundPrototype = WINFUNCTYPE(HRESULT, POINTER(SAFEARRAY), UINT, POINTER(LONG))
+SafeArrayGetLBoundParams = ((1, 'psa'), (1, 'nDim'), (1, 'plLbound'))
+
+#def SafeArrayGetUBound(psa, nDim, plUbound):
+#    return SafeArrayGetUBound.ctypes_function(psa, nDim, plUbound)
+SafeArrayGetUBoundPrototype = WINFUNCTYPE(HRESULT, POINTER(SAFEARRAY), UINT, POINTER(LONG))
+SafeArrayGetUBoundParams = ((1, 'psa'), (1, 'nDim'), (1, 'plUbound'))
+
+#def SafeArrayGetDim(psa):
+#    return SafeArrayGetDim.ctypes_function(psa)
+SafeArrayGetDimPrototype = WINFUNCTYPE(UINT, POINTER(SAFEARRAY))
+SafeArrayGetDimParams = ((1, 'psa'),)
+
+#def SafeArrayPutElement(psa, rgIndices, pv):
+#    return SafeArrayPutElement.ctypes_function(psa, rgIndices, pv)
+SafeArrayPutElementPrototype = WINFUNCTYPE(HRESULT, POINTER(SAFEARRAY), POINTER(LONG), PVOID)
+SafeArrayPutElementParams = ((1, 'psa'), (1, 'rgIndices'), (1, 'pv'))
+
+#def SafeArrayGetVartype(psa, pvt):
+#    return SafeArrayGetVartype.ctypes_function(psa, pvt)
+SafeArrayGetVartypePrototype = WINFUNCTYPE(HRESULT, POINTER(SAFEARRAY), POINTER(VARTYPE))
+SafeArrayGetVartypeParams = ((1, 'psa'), (1, 'pvt'))
+
+#def SysFreeString(bstrString):
+#    return SysFreeString.ctypes_function(bstrString)
+SysFreeStringPrototype = WINFUNCTYPE(VOID, BSTR)
+SysFreeStringParams = ((1, 'bstrString'),)
+
+#def SafeArrayCopy(psa, ppsaOut):
+#    return SafeArrayCopy.ctypes_function(psa, ppsaOut)
+SafeArrayCopyPrototype = WINFUNCTYPE(HRESULT, POINTER(SAFEARRAY), POINTER(LPSAFEARRAY))
+SafeArrayCopyParams = ((1, 'psa'), (1, 'ppsaOut'))
+
+#def SafeArrayCopyData(psaSource, psaTarget):
+#    return SafeArrayCopyData.ctypes_function(psaSource, psaTarget)
+SafeArrayCopyDataPrototype = WINFUNCTYPE(HRESULT, POINTER(SAFEARRAY), POINTER(SAFEARRAY))
+SafeArrayCopyDataParams = ((1, 'psaSource'), (1, 'psaTarget'))
+
+#def SysAllocString(psz):
+#    return SysAllocString.ctypes_function(psz)
+SysAllocStringPrototype = WINFUNCTYPE(PVOID, POINTER(OLECHAR))
+SysAllocStringParams = ((1, 'psz'),)
+
+#def SysFreeString(bstrString):
+#    return SysFreeString.ctypes_function(bstrString)
+SysFreeStringPrototype = WINFUNCTYPE(VOID, BSTR)
+SysFreeStringParams = ((1, 'bstrString'),)
+
 #def CryptCATAdminCalcHashFromFileHandle(hFile, pcbHash, pbHash, dwFlags):
 #    return CryptCATAdminCalcHashFromFileHandle.ctypes_function(hFile, pcbHash, pbHash, dwFlags)
 CryptCATAdminCalcHashFromFileHandlePrototype = WINFUNCTYPE(BOOL, HANDLE, POINTER(DWORD), POINTER(BYTE), DWORD)
 CryptCATAdminCalcHashFromFileHandleParams = ((1, 'hFile'), (1, 'pcbHash'), (1, 'pbHash'), (1, 'dwFlags'))
 
 #def CryptCATAdminCalcHashFromFileHandle2(hCatAdmin, hFile, pcbHash, pbHash, dwFlags):
 #    return CryptCATAdminCalcHashFromFileHandle2.ctypes_function(hCatAdmin, hFile, pcbHash, pbHash, dwFlags)
@@ -756,14 +836,59 @@
 CryptProtectMemoryParams = ((1, 'pDataIn'), (1, 'cbDataIn'), (1, 'dwFlags'))
 
 #def CryptUnprotectMemory(pDataIn, cbDataIn, dwFlags):
 #    return CryptUnprotectMemory.ctypes_function(pDataIn, cbDataIn, dwFlags)
 CryptUnprotectMemoryPrototype = WINFUNCTYPE(BOOL, LPVOID, DWORD, DWORD)
 CryptUnprotectMemoryParams = ((1, 'pDataIn'), (1, 'cbDataIn'), (1, 'dwFlags'))
 
+#def GetEnvironmentVariableA(lpName, lpBuffer, nSize):
+#    return GetEnvironmentVariableA.ctypes_function(lpName, lpBuffer, nSize)
+GetEnvironmentVariableAPrototype = WINFUNCTYPE(DWORD, LPCSTR, LPSTR, DWORD)
+GetEnvironmentVariableAParams = ((1, 'lpName'), (1, 'lpBuffer'), (1, 'nSize'))
+
+#def GetEnvironmentVariableW(lpName, lpBuffer, nSize):
+#    return GetEnvironmentVariableW.ctypes_function(lpName, lpBuffer, nSize)
+GetEnvironmentVariableWPrototype = WINFUNCTYPE(DWORD, LPCWSTR, LPWSTR, DWORD)
+GetEnvironmentVariableWParams = ((1, 'lpName'), (1, 'lpBuffer'), (1, 'nSize'))
+
+#def SetEnvironmentVariableA(lpName, lpValue):
+#    return SetEnvironmentVariableA.ctypes_function(lpName, lpValue)
+SetEnvironmentVariableAPrototype = WINFUNCTYPE(BOOL, LPCSTR, LPCSTR)
+SetEnvironmentVariableAParams = ((1, 'lpName'), (1, 'lpValue'))
+
+#def SetEnvironmentVariableW(lpName, lpValue):
+#    return SetEnvironmentVariableW.ctypes_function(lpName, lpValue)
+SetEnvironmentVariableWPrototype = WINFUNCTYPE(BOOL, LPCWSTR, LPCWSTR)
+SetEnvironmentVariableWParams = ((1, 'lpName'), (1, 'lpValue'))
+
+#def GetEnvironmentStringsA():
+#    return GetEnvironmentStringsA.ctypes_function()
+GetEnvironmentStringsAPrototype = WINFUNCTYPE(PVOID)
+GetEnvironmentStringsAParams = ()
+
+#def GetEnvironmentStringsW():
+#    return GetEnvironmentStringsW.ctypes_function()
+GetEnvironmentStringsWPrototype = WINFUNCTYPE(PVOID)
+GetEnvironmentStringsWParams = ()
+
+#def SetEnvironmentStringsW(NewEnvironment):
+#    return SetEnvironmentStringsW.ctypes_function(NewEnvironment)
+SetEnvironmentStringsWPrototype = WINFUNCTYPE(BOOL, LPWCH)
+SetEnvironmentStringsWParams = ((1, 'NewEnvironment'),)
+
+#def FreeEnvironmentStringsA(penv):
+#    return FreeEnvironmentStringsA.ctypes_function(penv)
+FreeEnvironmentStringsAPrototype = WINFUNCTYPE(BOOL, PVOID)
+FreeEnvironmentStringsAParams = ((1, 'penv'),)
+
+#def FreeEnvironmentStringsW(penv):
+#    return FreeEnvironmentStringsW.ctypes_function(penv)
+FreeEnvironmentStringsWPrototype = WINFUNCTYPE(BOOL, PVOID)
+FreeEnvironmentStringsWParams = ((1, 'penv'),)
+
 #def EnumerateTraceGuidsEx(TraceQueryInfoClass, InBuffer, InBufferSize, OutBuffer, OutBufferSize, ReturnLength):
 #    return EnumerateTraceGuidsEx.ctypes_function(TraceQueryInfoClass, InBuffer, InBufferSize, OutBuffer, OutBufferSize, ReturnLength)
 EnumerateTraceGuidsExPrototype = WINFUNCTYPE(ULONG, TRACE_QUERY_INFO_CLASS, PVOID, ULONG, PVOID, ULONG, PULONG)
 EnumerateTraceGuidsExParams = ((1, 'TraceQueryInfoClass'), (1, 'InBuffer'), (1, 'InBufferSize'), (1, 'OutBuffer'), (1, 'OutBufferSize'), (1, 'ReturnLength'))
 
 #def QueryAllTracesA(PropertyArray, PropertyArrayCount, SessionCount):
 #    return QueryAllTracesA.ctypes_function(PropertyArray, PropertyArrayCount, SessionCount)
@@ -1046,14 +1171,59 @@
 FindNextFileWParams = ((1, 'hFindFile'), (1, 'lpFindFileData'))
 
 #def FindClose(hFindFile):
 #    return FindClose.ctypes_function(hFindFile)
 FindClosePrototype = WINFUNCTYPE(BOOL, HANDLE)
 FindCloseParams = ((1, 'hFindFile'),)
 
+#def FindFirstChangeNotificationA(lpPathName, bWatchSubtree, dwNotifyFilter):
+#    return FindFirstChangeNotificationA.ctypes_function(lpPathName, bWatchSubtree, dwNotifyFilter)
+FindFirstChangeNotificationAPrototype = WINFUNCTYPE(HANDLE, LPCSTR, BOOL, DWORD)
+FindFirstChangeNotificationAParams = ((1, 'lpPathName'), (1, 'bWatchSubtree'), (1, 'dwNotifyFilter'))
+
+#def FindFirstChangeNotificationW(lpPathName, bWatchSubtree, dwNotifyFilter):
+#    return FindFirstChangeNotificationW.ctypes_function(lpPathName, bWatchSubtree, dwNotifyFilter)
+FindFirstChangeNotificationWPrototype = WINFUNCTYPE(HANDLE, LPCWSTR, BOOL, DWORD)
+FindFirstChangeNotificationWParams = ((1, 'lpPathName'), (1, 'bWatchSubtree'), (1, 'dwNotifyFilter'))
+
+#def FindNextChangeNotification(hChangeHandle):
+#    return FindNextChangeNotification.ctypes_function(hChangeHandle)
+FindNextChangeNotificationPrototype = WINFUNCTYPE(BOOL, HANDLE)
+FindNextChangeNotificationParams = ((1, 'hChangeHandle'),)
+
+#def FindCloseChangeNotification(hChangeHandle):
+#    return FindCloseChangeNotification.ctypes_function(hChangeHandle)
+FindCloseChangeNotificationPrototype = WINFUNCTYPE(BOOL, HANDLE)
+FindCloseChangeNotificationParams = ((1, 'hChangeHandle'),)
+
+#def FindNextChangeNotification(hChangeHandle):
+#    return FindNextChangeNotification.ctypes_function(hChangeHandle)
+FindNextChangeNotificationPrototype = WINFUNCTYPE(BOOL, HANDLE)
+FindNextChangeNotificationParams = ((1, 'hChangeHandle'),)
+
+#def ReadDirectoryChangesW(hDirectory, lpBuffer, nBufferLength, bWatchSubtree, dwNotifyFilter, lpBytesReturned, lpOverlapped, lpCompletionRoutine):
+#    return ReadDirectoryChangesW.ctypes_function(hDirectory, lpBuffer, nBufferLength, bWatchSubtree, dwNotifyFilter, lpBytesReturned, lpOverlapped, lpCompletionRoutine)
+ReadDirectoryChangesWPrototype = WINFUNCTYPE(BOOL, HANDLE, LPVOID, DWORD, BOOL, DWORD, LPDWORD, LPOVERLAPPED, LPOVERLAPPED_COMPLETION_ROUTINE)
+ReadDirectoryChangesWParams = ((1, 'hDirectory'), (1, 'lpBuffer'), (1, 'nBufferLength'), (1, 'bWatchSubtree'), (1, 'dwNotifyFilter'), (1, 'lpBytesReturned'), (1, 'lpOverlapped'), (1, 'lpCompletionRoutine'))
+
+#def ReadDirectoryChangesExW(hDirectory, lpBuffer, nBufferLength, bWatchSubtree, dwNotifyFilter, lpBytesReturned, lpOverlapped, lpCompletionRoutine, ReadDirectoryNotifyInformationClass):
+#    return ReadDirectoryChangesExW.ctypes_function(hDirectory, lpBuffer, nBufferLength, bWatchSubtree, dwNotifyFilter, lpBytesReturned, lpOverlapped, lpCompletionRoutine, ReadDirectoryNotifyInformationClass)
+ReadDirectoryChangesExWPrototype = WINFUNCTYPE(BOOL, HANDLE, LPVOID, DWORD, BOOL, DWORD, LPDWORD, LPOVERLAPPED, LPOVERLAPPED_COMPLETION_ROUTINE, READ_DIRECTORY_NOTIFY_INFORMATION_CLASS)
+ReadDirectoryChangesExWParams = ((1, 'hDirectory'), (1, 'lpBuffer'), (1, 'nBufferLength'), (1, 'bWatchSubtree'), (1, 'dwNotifyFilter'), (1, 'lpBytesReturned'), (1, 'lpOverlapped'), (1, 'lpCompletionRoutine'), (1, 'ReadDirectoryNotifyInformationClass'))
+
+#def LockFile(hFile, dwFileOffsetLow, dwFileOffsetHigh, nNumberOfBytesToLockLow, nNumberOfBytesToLockHigh):
+#    return LockFile.ctypes_function(hFile, dwFileOffsetLow, dwFileOffsetHigh, nNumberOfBytesToLockLow, nNumberOfBytesToLockHigh)
+LockFilePrototype = WINFUNCTYPE(BOOL, HANDLE, DWORD, DWORD, DWORD, DWORD)
+LockFileParams = ((1, 'hFile'), (1, 'dwFileOffsetLow'), (1, 'dwFileOffsetHigh'), (1, 'nNumberOfBytesToLockLow'), (1, 'nNumberOfBytesToLockHigh'))
+
+#def LockFileEx(hFile, dwFlags, dwReserved, nNumberOfBytesToLockLow, nNumberOfBytesToLockHigh, lpOverlapped):
+#    return LockFileEx.ctypes_function(hFile, dwFlags, dwReserved, nNumberOfBytesToLockLow, nNumberOfBytesToLockHigh, lpOverlapped)
+LockFileExPrototype = WINFUNCTYPE(BOOL, HANDLE, DWORD, DWORD, DWORD, DWORD, LPOVERLAPPED)
+LockFileExParams = ((1, 'hFile'), (1, 'dwFlags'), (1, 'dwReserved'), (1, 'nNumberOfBytesToLockLow'), (1, 'nNumberOfBytesToLockHigh'), (1, 'lpOverlapped'))
+
 #def HeapAlloc(hHeap, dwFlags, dwBytes):
 #    return HeapAlloc.ctypes_function(hHeap, dwFlags, dwBytes)
 HeapAllocPrototype = WINFUNCTYPE(LPVOID, HANDLE, DWORD, SIZE_T)
 HeapAllocParams = ((1, 'hHeap'), (1, 'dwFlags'), (1, 'dwBytes'))
 
 #def InternetCheckConnectionA(lpszUrl, dwFlags, dwReserved):
 #    return InternetCheckConnectionA.ctypes_function(lpszUrl, dwFlags, dwReserved)
@@ -1156,14 +1326,64 @@
 HttpSendRequestAParams = ((1, 'hRequest'), (1, 'lpszHeaders'), (1, 'dwHeadersLength'), (1, 'lpOptional'), (1, 'dwOptionalLength'))
 
 #def HttpSendRequestW(hRequest, lpszHeaders, dwHeadersLength, lpOptional, dwOptionalLength):
 #    return HttpSendRequestW.ctypes_function(hRequest, lpszHeaders, dwHeadersLength, lpOptional, dwOptionalLength)
 HttpSendRequestWPrototype = WINFUNCTYPE(BOOL, HINTERNET, LPCWSTR, DWORD, LPVOID, DWORD)
 HttpSendRequestWParams = ((1, 'hRequest'), (1, 'lpszHeaders'), (1, 'dwHeadersLength'), (1, 'lpOptional'), (1, 'dwOptionalLength'))
 
+#def WinHttpOpen(pszAgentW, dwAccessType, pszProxyW, pszProxyBypassW, dwFlags):
+#    return WinHttpOpen.ctypes_function(pszAgentW, dwAccessType, pszProxyW, pszProxyBypassW, dwFlags)
+WinHttpOpenPrototype = WINFUNCTYPE(HINTERNET, LPCWSTR, DWORD, LPCWSTR, LPCWSTR, DWORD)
+WinHttpOpenParams = ((1, 'pszAgentW'), (1, 'dwAccessType'), (1, 'pszProxyW'), (1, 'pszProxyBypassW'), (1, 'dwFlags'))
+
+#def WinHttpCloseHandle(hInternet):
+#    return WinHttpCloseHandle.ctypes_function(hInternet)
+WinHttpCloseHandlePrototype = WINFUNCTYPE(BOOL, HINTERNET)
+WinHttpCloseHandleParams = ((1, 'hInternet'),)
+
+#def WinHttpConnect(hSession, pswzServerName, nServerPort, dwReserved):
+#    return WinHttpConnect.ctypes_function(hSession, pswzServerName, nServerPort, dwReserved)
+WinHttpConnectPrototype = WINFUNCTYPE(HINTERNET, HINTERNET, LPCWSTR, INTERNET_PORT, DWORD)
+WinHttpConnectParams = ((1, 'hSession'), (1, 'pswzServerName'), (1, 'nServerPort'), (1, 'dwReserved'))
+
+#def WinHttpQueryDataAvailable(hRequest, lpdwNumberOfBytesAvailable):
+#    return WinHttpQueryDataAvailable.ctypes_function(hRequest, lpdwNumberOfBytesAvailable)
+WinHttpQueryDataAvailablePrototype = WINFUNCTYPE(BOOL, HINTERNET, LPDWORD)
+WinHttpQueryDataAvailableParams = ((1, 'hRequest'), (1, 'lpdwNumberOfBytesAvailable'))
+
+#def WinHttpReadData(hRequest, lpBuffer, dwNumberOfBytesToRead, lpdwNumberOfBytesRead):
+#    return WinHttpReadData.ctypes_function(hRequest, lpBuffer, dwNumberOfBytesToRead, lpdwNumberOfBytesRead)
+WinHttpReadDataPrototype = WINFUNCTYPE(BOOL, HINTERNET, LPVOID, DWORD, LPDWORD)
+WinHttpReadDataParams = ((1, 'hRequest'), (1, 'lpBuffer'), (1, 'dwNumberOfBytesToRead'), (1, 'lpdwNumberOfBytesRead'))
+
+#def WinHttpOpenRequest(hConnect, pwszVerb, pwszObjectName, pwszVersion, pwszReferrer, ppwszAcceptTypes, dwFlags):
+#    return WinHttpOpenRequest.ctypes_function(hConnect, pwszVerb, pwszObjectName, pwszVersion, pwszReferrer, ppwszAcceptTypes, dwFlags)
+WinHttpOpenRequestPrototype = WINFUNCTYPE(HINTERNET, HINTERNET, LPCWSTR, LPCWSTR, LPCWSTR, LPCWSTR, POINTER(LPCWSTR), DWORD)
+WinHttpOpenRequestParams = ((1, 'hConnect'), (1, 'pwszVerb'), (1, 'pwszObjectName'), (1, 'pwszVersion'), (1, 'pwszReferrer'), (1, 'ppwszAcceptTypes'), (1, 'dwFlags'))
+
+#def WinHttpSendRequest(hRequest, lpszHeaders, dwHeadersLength, lpOptional, dwOptionalLength, dwTotalLength, dwContext):
+#    return WinHttpSendRequest.ctypes_function(hRequest, lpszHeaders, dwHeadersLength, lpOptional, dwOptionalLength, dwTotalLength, dwContext)
+WinHttpSendRequestPrototype = WINFUNCTYPE(BOOL, HINTERNET, LPCWSTR, DWORD, LPVOID, DWORD, DWORD, DWORD_PTR)
+WinHttpSendRequestParams = ((1, 'hRequest'), (1, 'lpszHeaders'), (1, 'dwHeadersLength'), (1, 'lpOptional'), (1, 'dwOptionalLength'), (1, 'dwTotalLength'), (1, 'dwContext'))
+
+#def WinHttpReceiveResponse(hRequest, lpReserved):
+#    return WinHttpReceiveResponse.ctypes_function(hRequest, lpReserved)
+WinHttpReceiveResponsePrototype = WINFUNCTYPE(BOOL, HINTERNET, LPVOID)
+WinHttpReceiveResponseParams = ((1, 'hRequest'), (1, 'lpReserved'))
+
+#def WinHttpAddRequestHeaders(hRequest, lpszHeaders, dwHeadersLength, dwModifiers):
+#    return WinHttpAddRequestHeaders.ctypes_function(hRequest, lpszHeaders, dwHeadersLength, dwModifiers)
+WinHttpAddRequestHeadersPrototype = WINFUNCTYPE(BOOL, HINTERNET, LPCWSTR, DWORD, DWORD)
+WinHttpAddRequestHeadersParams = ((1, 'hRequest'), (1, 'lpszHeaders'), (1, 'dwHeadersLength'), (1, 'dwModifiers'))
+
+#def WinHttpQueryHeaders(hRequest, dwInfoLevel, pwszName, lpBuffer, lpdwBufferLength, lpdwIndex):
+#    return WinHttpQueryHeaders.ctypes_function(hRequest, dwInfoLevel, pwszName, lpBuffer, lpdwBufferLength, lpdwIndex)
+WinHttpQueryHeadersPrototype = WINFUNCTYPE(BOOL, HINTERNET, DWORD, LPCWSTR, LPVOID, LPDWORD, LPDWORD)
+WinHttpQueryHeadersParams = ((1, 'hRequest'), (1, 'dwInfoLevel'), (1, 'pwszName'), (1, 'lpBuffer'), (1, 'lpdwBufferLength'), (1, 'lpdwIndex'))
+
 #def LsaOpenPolicy(SystemName, ObjectAttributes, DesiredAccess, PolicyHandle):
 #    return LsaOpenPolicy.ctypes_function(SystemName, ObjectAttributes, DesiredAccess, PolicyHandle)
 LsaOpenPolicyPrototype = WINFUNCTYPE(NTSTATUS, PLSA_UNICODE_STRING, PLSA_OBJECT_ATTRIBUTES, ACCESS_MASK, PLSA_HANDLE)
 LsaOpenPolicyParams = ((1, 'SystemName'), (1, 'ObjectAttributes'), (1, 'DesiredAccess'), (1, 'PolicyHandle'))
 
 #def LsaQueryInformationPolicy(PolicyHandle, InformationClass, Buffer):
 #    return LsaQueryInformationPolicy.ctypes_function(PolicyHandle, InformationClass, Buffer)
@@ -1211,14 +1431,74 @@
 OpenFileMappingAParams = ((1, 'dwDesiredAccess'), (1, 'bInheritHandle'), (1, 'lpName'))
 
 #def UnmapViewOfFile(lpBaseAddress):
 #    return UnmapViewOfFile.ctypes_function(lpBaseAddress)
 UnmapViewOfFilePrototype = WINFUNCTYPE(BOOL, LPCVOID)
 UnmapViewOfFileParams = ((1, 'lpBaseAddress'),)
 
+#def NetLocalGroupGetMembers(servername, localgroupname, level, bufptr, prefmaxlen, entriesread, totalentries, resumehandle):
+#    return NetLocalGroupGetMembers.ctypes_function(servername, localgroupname, level, bufptr, prefmaxlen, entriesread, totalentries, resumehandle)
+NetLocalGroupGetMembersPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, LPCWSTR, DWORD, POINTER(LPBYTE), DWORD, LPDWORD, LPDWORD, PDWORD_PTR)
+NetLocalGroupGetMembersParams = ((1, 'servername'), (1, 'localgroupname'), (1, 'level'), (1, 'bufptr'), (1, 'prefmaxlen'), (1, 'entriesread'), (1, 'totalentries'), (1, 'resumehandle'))
+
+#def NetQueryDisplayInformation(ServerName, Level, Index, EntriesRequested, PreferredMaximumLength, ReturnedEntryCount, SortedBuffer):
+#    return NetQueryDisplayInformation.ctypes_function(ServerName, Level, Index, EntriesRequested, PreferredMaximumLength, ReturnedEntryCount, SortedBuffer)
+NetQueryDisplayInformationPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, DWORD, DWORD, DWORD, DWORD, LPDWORD, POINTER(PVOID))
+NetQueryDisplayInformationParams = ((1, 'ServerName'), (1, 'Level'), (1, 'Index'), (1, 'EntriesRequested'), (1, 'PreferredMaximumLength'), (1, 'ReturnedEntryCount'), (1, 'SortedBuffer'))
+
+#def NetUserEnum(servername, level, filter, bufptr, prefmaxlen, entriesread, totalentries, resume_handle):
+#    return NetUserEnum.ctypes_function(servername, level, filter, bufptr, prefmaxlen, entriesread, totalentries, resume_handle)
+NetUserEnumPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, DWORD, DWORD, POINTER(LPBYTE), DWORD, LPDWORD, LPDWORD, PDWORD)
+NetUserEnumParams = ((1, 'servername'), (1, 'level'), (1, 'filter'), (1, 'bufptr'), (1, 'prefmaxlen'), (1, 'entriesread'), (1, 'totalentries'), (1, 'resume_handle'))
+
+#def NetGroupEnum(servername, level, bufptr, prefmaxlen, entriesread, totalentries, resume_handle):
+#    return NetGroupEnum.ctypes_function(servername, level, bufptr, prefmaxlen, entriesread, totalentries, resume_handle)
+NetGroupEnumPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, DWORD, POINTER(LPBYTE), DWORD, LPDWORD, LPDWORD, PDWORD_PTR)
+NetGroupEnumParams = ((1, 'servername'), (1, 'level'), (1, 'bufptr'), (1, 'prefmaxlen'), (1, 'entriesread'), (1, 'totalentries'), (1, 'resume_handle'))
+
+#def NetGroupGetInfo(servername, groupname, level, bufptr):
+#    return NetGroupGetInfo.ctypes_function(servername, groupname, level, bufptr)
+NetGroupGetInfoPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, LPCWSTR, DWORD, POINTER(LPBYTE))
+NetGroupGetInfoParams = ((1, 'servername'), (1, 'groupname'), (1, 'level'), (1, 'bufptr'))
+
+#def NetGroupGetUsers(servername, groupname, level, bufptr, prefmaxlen, entriesread, totalentries, ResumeHandle):
+#    return NetGroupGetUsers.ctypes_function(servername, groupname, level, bufptr, prefmaxlen, entriesread, totalentries, ResumeHandle)
+NetGroupGetUsersPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, LPCWSTR, DWORD, POINTER(LPBYTE), DWORD, LPDWORD, LPDWORD, PDWORD_PTR)
+NetGroupGetUsersParams = ((1, 'servername'), (1, 'groupname'), (1, 'level'), (1, 'bufptr'), (1, 'prefmaxlen'), (1, 'entriesread'), (1, 'totalentries'), (1, 'ResumeHandle'))
+
+#def NetLocalGroupEnum(servername, level, bufptr, prefmaxlen, entriesread, totalentries, resumehandle):
+#    return NetLocalGroupEnum.ctypes_function(servername, level, bufptr, prefmaxlen, entriesread, totalentries, resumehandle)
+NetLocalGroupEnumPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, DWORD, POINTER(LPBYTE), DWORD, LPDWORD, LPDWORD, PDWORD_PTR)
+NetLocalGroupEnumParams = ((1, 'servername'), (1, 'level'), (1, 'bufptr'), (1, 'prefmaxlen'), (1, 'entriesread'), (1, 'totalentries'), (1, 'resumehandle'))
+
+#def NetLocalGroupGetInfo(servername, groupname, level, bufptr):
+#    return NetLocalGroupGetInfo.ctypes_function(servername, groupname, level, bufptr)
+NetLocalGroupGetInfoPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, LPCWSTR, DWORD, POINTER(LPBYTE))
+NetLocalGroupGetInfoParams = ((1, 'servername'), (1, 'groupname'), (1, 'level'), (1, 'bufptr'))
+
+#def NetLocalGroupGetMembers(servername, localgroupname, level, bufptr, prefmaxlen, entriesread, totalentries, resumehandle):
+#    return NetLocalGroupGetMembers.ctypes_function(servername, localgroupname, level, bufptr, prefmaxlen, entriesread, totalentries, resumehandle)
+NetLocalGroupGetMembersPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, LPCWSTR, DWORD, POINTER(LPBYTE), DWORD, LPDWORD, LPDWORD, PDWORD_PTR)
+NetLocalGroupGetMembersParams = ((1, 'servername'), (1, 'localgroupname'), (1, 'level'), (1, 'bufptr'), (1, 'prefmaxlen'), (1, 'entriesread'), (1, 'totalentries'), (1, 'resumehandle'))
+
+#def NetLocalGroupGetInfo(servername, groupname, level, bufptr):
+#    return NetLocalGroupGetInfo.ctypes_function(servername, groupname, level, bufptr)
+NetLocalGroupGetInfoPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, LPCWSTR, DWORD, POINTER(LPBYTE))
+NetLocalGroupGetInfoParams = ((1, 'servername'), (1, 'groupname'), (1, 'level'), (1, 'bufptr'))
+
+#def NetLocalGroupEnum(servername, level, bufptr, prefmaxlen, entriesread, totalentries, resumehandle):
+#    return NetLocalGroupEnum.ctypes_function(servername, level, bufptr, prefmaxlen, entriesread, totalentries, resumehandle)
+NetLocalGroupEnumPrototype = WINFUNCTYPE(NET_API_STATUS, LPCWSTR, DWORD, POINTER(LPBYTE), DWORD, LPDWORD, LPDWORD, PDWORD_PTR)
+NetLocalGroupEnumParams = ((1, 'servername'), (1, 'level'), (1, 'bufptr'), (1, 'prefmaxlen'), (1, 'entriesread'), (1, 'totalentries'), (1, 'resumehandle'))
+
+#def NetApiBufferFree(Buffer):
+#    return NetApiBufferFree.ctypes_function(Buffer)
+NetApiBufferFreePrototype = WINFUNCTYPE(NET_API_STATUS, LPVOID)
+NetApiBufferFreeParams = ((1, 'Buffer'),)
+
 #def GetIpNetTable(IpNetTable, SizePointer, Order):
 #    return GetIpNetTable.ctypes_function(IpNetTable, SizePointer, Order)
 GetIpNetTablePrototype = WINFUNCTYPE(ULONG, PMIB_IPNETTABLE, PULONG, BOOL)
 GetIpNetTableParams = ((1, 'IpNetTable'), (1, 'SizePointer'), (1, 'Order'))
 
 #def GetExtendedTcpTable(pTcpTable, pdwSize, bOrder, ulAf, TableClass, Reserved):
 #    return GetExtendedTcpTable.ctypes_function(pTcpTable, pdwSize, bOrder, ulAf, TableClass, Reserved)
@@ -1251,14 +1531,29 @@
 DnsQuery_AParams = ((1, 'pszName'), (1, 'wType'), (1, 'Options'), (1, 'pExtra'), (1, 'ppQueryResults'), (1, 'pReserved'))
 
 #def DnsQuery_W(pszName, wType, Options, pExtra, ppQueryResults, pReserved):
 #    return DnsQuery_W.ctypes_function(pszName, wType, Options, pExtra, ppQueryResults, pReserved)
 DnsQuery_WPrototype = WINFUNCTYPE(DNS_STATUS, PCWSTR, WORD, DWORD, PVOID, POINTER(PDNS_RECORDW), POINTER(PVOID))
 DnsQuery_WParams = ((1, 'pszName'), (1, 'wType'), (1, 'Options'), (1, 'pExtra'), (1, 'ppQueryResults'), (1, 'pReserved'))
 
+#def DnsQueryEx(pQueryRequest, pQueryResults, pCancelHandle):
+#    return DnsQueryEx.ctypes_function(pQueryRequest, pQueryResults, pCancelHandle)
+DnsQueryExPrototype = WINFUNCTYPE(DNS_STATUS, PDNS_QUERY_REQUEST, PDNS_QUERY_RESULT, PDNS_QUERY_CANCEL)
+DnsQueryExParams = ((1, 'pQueryRequest'), (1, 'pQueryResults'), (1, 'pCancelHandle'))
+
+#def GetAdaptersInfo(AdapterInfo, SizePointer):
+#    return GetAdaptersInfo.ctypes_function(AdapterInfo, SizePointer)
+GetAdaptersInfoPrototype = WINFUNCTYPE(ULONG, PIP_ADAPTER_INFO, PULONG)
+GetAdaptersInfoParams = ((1, 'AdapterInfo'), (1, 'SizePointer'))
+
+#def GetPerAdapterInfo(IfIndex, pPerAdapterInfo, pOutBufLen):
+#    return GetPerAdapterInfo.ctypes_function(IfIndex, pPerAdapterInfo, pOutBufLen)
+GetPerAdapterInfoPrototype = WINFUNCTYPE(DWORD, ULONG, PIP_PER_ADAPTER_INFO, PULONG)
+GetPerAdapterInfoParams = ((1, 'IfIndex'), (1, 'pPerAdapterInfo'), (1, 'pOutBufLen'))
+
 #def CreateFileTransactedA(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile, hTransaction, pusMiniVersion, pExtendedParameter):
 #    return CreateFileTransactedA.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile, hTransaction, pusMiniVersion, pExtendedParameter)
 CreateFileTransactedAPrototype = WINFUNCTYPE(HANDLE, LPCSTR, DWORD, DWORD, LPSECURITY_ATTRIBUTES, DWORD, DWORD, HANDLE, HANDLE, PUSHORT, PVOID)
 CreateFileTransactedAParams = ((1, 'lpFileName'), (1, 'dwDesiredAccess'), (1, 'dwShareMode'), (1, 'lpSecurityAttributes'), (1, 'dwCreationDisposition'), (1, 'dwFlagsAndAttributes'), (1, 'hTemplateFile'), (1, 'hTransaction'), (1, 'pusMiniVersion'), (1, 'pExtendedParameter'))
 
 #def CreateFileTransactedW(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile, hTransaction, pusMiniVersion, pExtendedParameter):
 #    return CreateFileTransactedW.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile, hTransaction, pusMiniVersion, pExtendedParameter)
@@ -1346,14 +1641,79 @@
 SetNamedPipeHandleStateParams = ((1, 'hNamedPipe'), (1, 'lpMode'), (1, 'lpMaxCollectionCount'), (1, 'lpCollectDataTimeout'))
 
 #def PeekNamedPipe(hNamedPipe, lpBuffer, nBufferSize, lpBytesRead, lpTotalBytesAvail, lpBytesLeftThisMessage):
 #    return PeekNamedPipe.ctypes_function(hNamedPipe, lpBuffer, nBufferSize, lpBytesRead, lpTotalBytesAvail, lpBytesLeftThisMessage)
 PeekNamedPipePrototype = WINFUNCTYPE(BOOL, HANDLE, LPVOID, DWORD, LPDWORD, LPDWORD, LPDWORD)
 PeekNamedPipeParams = ((1, 'hNamedPipe'), (1, 'lpBuffer'), (1, 'nBufferSize'), (1, 'lpBytesRead'), (1, 'lpTotalBytesAvail'), (1, 'lpBytesLeftThisMessage'))
 
+#def CreateToolhelp32Snapshot(dwFlags, th32ProcessID):
+#    return CreateToolhelp32Snapshot.ctypes_function(dwFlags, th32ProcessID)
+CreateToolhelp32SnapshotPrototype = WINFUNCTYPE(HANDLE, DWORD, DWORD)
+CreateToolhelp32SnapshotParams = ((1, 'dwFlags'), (1, 'th32ProcessID'))
+
+#def Thread32First(hSnapshot, lpte):
+#    return Thread32First.ctypes_function(hSnapshot, lpte)
+Thread32FirstPrototype = WINFUNCTYPE(BOOL, HANDLE, LPTHREADENTRY32)
+Thread32FirstParams = ((1, 'hSnapshot'), (1, 'lpte'))
+
+#def Thread32Next(hSnapshot, lpte):
+#    return Thread32Next.ctypes_function(hSnapshot, lpte)
+Thread32NextPrototype = WINFUNCTYPE(BOOL, HANDLE, LPTHREADENTRY32)
+Thread32NextParams = ((1, 'hSnapshot'), (1, 'lpte'))
+
+#def Process32First(hSnapshot, lppe):
+#    return Process32First.ctypes_function(hSnapshot, lppe)
+Process32FirstPrototype = WINFUNCTYPE(BOOL, HANDLE, LPPROCESSENTRY32)
+Process32FirstParams = ((1, 'hSnapshot'), (1, 'lppe'))
+
+#def Process32Next(hSnapshot, lppe):
+#    return Process32Next.ctypes_function(hSnapshot, lppe)
+Process32NextPrototype = WINFUNCTYPE(BOOL, HANDLE, LPPROCESSENTRY32)
+Process32NextParams = ((1, 'hSnapshot'), (1, 'lppe'))
+
+#def Process32FirstW(hSnapshot, lppe):
+#    return Process32FirstW.ctypes_function(hSnapshot, lppe)
+Process32FirstWPrototype = WINFUNCTYPE(BOOL, HANDLE, LPPROCESSENTRY32W)
+Process32FirstWParams = ((1, 'hSnapshot'), (1, 'lppe'))
+
+#def Process32NextW(hSnapshot, lppe):
+#    return Process32NextW.ctypes_function(hSnapshot, lppe)
+Process32NextWPrototype = WINFUNCTYPE(BOOL, HANDLE, LPPROCESSENTRY32W)
+Process32NextWParams = ((1, 'hSnapshot'), (1, 'lppe'))
+
+#def GetProcAddress(hModule, lpProcName):
+#    return GetProcAddress.ctypes_function(hModule, lpProcName)
+GetProcAddressPrototype = WINFUNCTYPE(FARPROC, HMODULE, LPCSTR)
+GetProcAddressParams = ((1, 'hModule'), (1, 'lpProcName'))
+
+#def LoadLibraryA(lpFileName):
+#    return LoadLibraryA.ctypes_function(lpFileName)
+LoadLibraryAPrototype = WINFUNCTYPE(HMODULE, LPCSTR)
+LoadLibraryAParams = ((1, 'lpFileName'),)
+
+#def LoadLibraryW(lpFileName):
+#    return LoadLibraryW.ctypes_function(lpFileName)
+LoadLibraryWPrototype = WINFUNCTYPE(HMODULE, LPCWSTR)
+LoadLibraryWParams = ((1, 'lpFileName'),)
+
+#def LoadLibraryExA(lpLibFileName, hFile, dwFlags):
+#    return LoadLibraryExA.ctypes_function(lpLibFileName, hFile, dwFlags)
+LoadLibraryExAPrototype = WINFUNCTYPE(HMODULE, LPCSTR, HANDLE, DWORD)
+LoadLibraryExAParams = ((1, 'lpLibFileName'), (1, 'hFile'), (1, 'dwFlags'))
+
+#def LoadLibraryExW(lpLibFileName, hFile, dwFlags):
+#    return LoadLibraryExW.ctypes_function(lpLibFileName, hFile, dwFlags)
+LoadLibraryExWPrototype = WINFUNCTYPE(HMODULE, LPCWSTR, HANDLE, DWORD)
+LoadLibraryExWParams = ((1, 'lpLibFileName'), (1, 'hFile'), (1, 'dwFlags'))
+
+#def FreeLibrary(hLibModule):
+#    return FreeLibrary.ctypes_function(hLibModule)
+FreeLibraryPrototype = WINFUNCTYPE(BOOL, HMODULE)
+FreeLibraryParams = ((1, 'hLibModule'),)
+
 #def RegQueryValueExA(hKey, lpValueName, lpReserved, lpType, lpData, lpcbData):
 #    return RegQueryValueExA.ctypes_function(hKey, lpValueName, lpReserved, lpType, lpData, lpcbData)
 RegQueryValueExAPrototype = WINFUNCTYPE(LSTATUS, HKEY, LPCSTR, LPDWORD, LPDWORD, LPBYTE, LPDWORD)
 RegQueryValueExAParams = ((1, 'hKey'), (1, 'lpValueName'), (1, 'lpReserved'), (1, 'lpType'), (1, 'lpData'), (1, 'lpcbData'))
 
 #def RegQueryValueExW(hKey, lpValueName, lpReserved, lpType, lpData, lpcbData):
 #    return RegQueryValueExW.ctypes_function(hKey, lpValueName, lpReserved, lpType, lpData, lpcbData)
@@ -1506,14 +1866,34 @@
 RegSaveKeyExAParams = ((1, 'hKey'), (1, 'lpFile'), (1, 'lpSecurityAttributes'), (1, 'Flags'))
 
 #def RegSaveKeyExW(hKey, lpFile, lpSecurityAttributes, Flags):
 #    return RegSaveKeyExW.ctypes_function(hKey, lpFile, lpSecurityAttributes, Flags)
 RegSaveKeyExWPrototype = WINFUNCTYPE(LSTATUS, HKEY, LPCWSTR, LPSECURITY_ATTRIBUTES, DWORD)
 RegSaveKeyExWParams = ((1, 'hKey'), (1, 'lpFile'), (1, 'lpSecurityAttributes'), (1, 'Flags'))
 
+#def RegLoadKeyA(hKey, lpSubKey, lpFile):
+#    return RegLoadKeyA.ctypes_function(hKey, lpSubKey, lpFile)
+RegLoadKeyAPrototype = WINFUNCTYPE(LSTATUS, HKEY, LPCSTR, LPCSTR)
+RegLoadKeyAParams = ((1, 'hKey'), (1, 'lpSubKey'), (1, 'lpFile'))
+
+#def RegLoadKeyW(hKey, lpSubKey, lpFile):
+#    return RegLoadKeyW.ctypes_function(hKey, lpSubKey, lpFile)
+RegLoadKeyWPrototype = WINFUNCTYPE(LSTATUS, HKEY, LPCWSTR, LPCWSTR)
+RegLoadKeyWParams = ((1, 'hKey'), (1, 'lpSubKey'), (1, 'lpFile'))
+
+#def RegUnLoadKeyA(hKey, lpSubKey):
+#    return RegUnLoadKeyA.ctypes_function(hKey, lpSubKey)
+RegUnLoadKeyAPrototype = WINFUNCTYPE(LSTATUS, HKEY, LPCSTR)
+RegUnLoadKeyAParams = ((1, 'hKey'), (1, 'lpSubKey'))
+
+#def RegUnLoadKeyW(hKey, lpSubKey):
+#    return RegUnLoadKeyW.ctypes_function(hKey, lpSubKey)
+RegUnLoadKeyWPrototype = WINFUNCTYPE(LSTATUS, HKEY, LPCWSTR)
+RegUnLoadKeyWParams = ((1, 'hKey'), (1, 'lpSubKey'))
+
 #def IsValidSecurityDescriptor(pSecurityDescriptor):
 #    return IsValidSecurityDescriptor.ctypes_function(pSecurityDescriptor)
 IsValidSecurityDescriptorPrototype = WINFUNCTYPE(BOOL, PSECURITY_DESCRIPTOR)
 IsValidSecurityDescriptorParams = ((1, 'pSecurityDescriptor'),)
 
 #def ConvertStringSecurityDescriptorToSecurityDescriptorA(StringSecurityDescriptor, StringSDRevision, SecurityDescriptor, SecurityDescriptorSize):
 #    return ConvertStringSecurityDescriptorToSecurityDescriptorA.ctypes_function(StringSecurityDescriptor, StringSDRevision, SecurityDescriptor, SecurityDescriptorSize)
@@ -1556,14 +1936,19 @@
 GetSecurityDescriptorLengthParams = ((1, 'pSecurityDescriptor'),)
 
 #def GetSecurityDescriptorOwner(pSecurityDescriptor, pOwner, lpbOwnerDefaulted):
 #    return GetSecurityDescriptorOwner.ctypes_function(pSecurityDescriptor, pOwner, lpbOwnerDefaulted)
 GetSecurityDescriptorOwnerPrototype = WINFUNCTYPE(BOOL, PSECURITY_DESCRIPTOR, POINTER(PSID), LPBOOL)
 GetSecurityDescriptorOwnerParams = ((1, 'pSecurityDescriptor'), (1, 'pOwner'), (1, 'lpbOwnerDefaulted'))
 
+#def SetSecurityDescriptorOwner(pSecurityDescriptor, pOwner, bOwnerDefaulted):
+#    return SetSecurityDescriptorOwner.ctypes_function(pSecurityDescriptor, pOwner, bOwnerDefaulted)
+SetSecurityDescriptorOwnerPrototype = WINFUNCTYPE(BOOL, PSECURITY_DESCRIPTOR, PSID, BOOL)
+SetSecurityDescriptorOwnerParams = ((1, 'pSecurityDescriptor'), (1, 'pOwner'), (1, 'bOwnerDefaulted'))
+
 #def GetSecurityDescriptorRMControl(SecurityDescriptor, RMControl):
 #    return GetSecurityDescriptorRMControl.ctypes_function(SecurityDescriptor, RMControl)
 GetSecurityDescriptorRMControlPrototype = WINFUNCTYPE(DWORD, PSECURITY_DESCRIPTOR, PUCHAR)
 GetSecurityDescriptorRMControlParams = ((1, 'SecurityDescriptor'), (1, 'RMControl'))
 
 #def GetSecurityDescriptorSacl(pSecurityDescriptor, lpbSaclPresent, pSacl, lpbSaclDefaulted):
 #    return GetSecurityDescriptorSacl.ctypes_function(pSecurityDescriptor, lpbSaclPresent, pSacl, lpbSaclDefaulted)
@@ -1706,14 +2091,29 @@
 AddAccessDeniedAceExParams = ((1, 'pAcl'), (1, 'dwAceRevision'), (1, 'AceFlags'), (1, 'AccessMask'), (1, 'pSid'))
 
 #def BuildSecurityDescriptorW(pOwner, pGroup, cCountOfAccessEntries, pListOfAccessEntries, cCountOfAuditEntries, pListOfAuditEntries, pOldSD, pSizeNewSD, pNewSD):
 #    return BuildSecurityDescriptorW.ctypes_function(pOwner, pGroup, cCountOfAccessEntries, pListOfAccessEntries, cCountOfAuditEntries, pListOfAuditEntries, pOldSD, pSizeNewSD, pNewSD)
 BuildSecurityDescriptorWPrototype = WINFUNCTYPE(DWORD, PTRUSTEE_W, PTRUSTEE_W, ULONG, PEXPLICIT_ACCESS_W, ULONG, PEXPLICIT_ACCESS_W, PSECURITY_DESCRIPTOR, PULONG, POINTER(PSECURITY_DESCRIPTOR))
 BuildSecurityDescriptorWParams = ((1, 'pOwner'), (1, 'pGroup'), (1, 'cCountOfAccessEntries'), (1, 'pListOfAccessEntries'), (1, 'cCountOfAuditEntries'), (1, 'pListOfAuditEntries'), (1, 'pOldSD'), (1, 'pSizeNewSD'), (1, 'pNewSD'))
 
+#def MakeAbsoluteSD(pSelfRelativeSecurityDescriptor, pAbsoluteSecurityDescriptor, lpdwAbsoluteSecurityDescriptorSize, pDacl, lpdwDaclSize, pSacl, lpdwSaclSize, pOwner, lpdwOwnerSize, pPrimaryGroup, lpdwPrimaryGroupSize):
+#    return MakeAbsoluteSD.ctypes_function(pSelfRelativeSecurityDescriptor, pAbsoluteSecurityDescriptor, lpdwAbsoluteSecurityDescriptorSize, pDacl, lpdwDaclSize, pSacl, lpdwSaclSize, pOwner, lpdwOwnerSize, pPrimaryGroup, lpdwPrimaryGroupSize)
+MakeAbsoluteSDPrototype = WINFUNCTYPE(BOOL, PSECURITY_DESCRIPTOR, PSECURITY_DESCRIPTOR, LPDWORD, PACL, LPDWORD, PACL, LPDWORD, PSID, LPDWORD, PSID, LPDWORD)
+MakeAbsoluteSDParams = ((1, 'pSelfRelativeSecurityDescriptor'), (1, 'pAbsoluteSecurityDescriptor'), (1, 'lpdwAbsoluteSecurityDescriptorSize'), (1, 'pDacl'), (1, 'lpdwDaclSize'), (1, 'pSacl'), (1, 'lpdwSaclSize'), (1, 'pOwner'), (1, 'lpdwOwnerSize'), (1, 'pPrimaryGroup'), (1, 'lpdwPrimaryGroupSize'))
+
+#def MakeSelfRelativeSD(pAbsoluteSecurityDescriptor, pSelfRelativeSecurityDescriptor, lpdwBufferLength):
+#    return MakeSelfRelativeSD.ctypes_function(pAbsoluteSecurityDescriptor, pSelfRelativeSecurityDescriptor, lpdwBufferLength)
+MakeSelfRelativeSDPrototype = WINFUNCTYPE(BOOL, PSECURITY_DESCRIPTOR, PSECURITY_DESCRIPTOR, LPDWORD)
+MakeSelfRelativeSDParams = ((1, 'pAbsoluteSecurityDescriptor'), (1, 'pSelfRelativeSecurityDescriptor'), (1, 'lpdwBufferLength'))
+
+#def InitializeSecurityDescriptor(pSecurityDescriptor, dwRevision):
+#    return InitializeSecurityDescriptor.ctypes_function(pSecurityDescriptor, dwRevision)
+InitializeSecurityDescriptorPrototype = WINFUNCTYPE(BOOL, PSECURITY_DESCRIPTOR, DWORD)
+InitializeSecurityDescriptorParams = ((1, 'pSecurityDescriptor'), (1, 'dwRevision'))
+
 #def OpenSCManagerA(lpMachineName, lpDatabaseName, dwDesiredAccess):
 #    return OpenSCManagerA.ctypes_function(lpMachineName, lpDatabaseName, dwDesiredAccess)
 OpenSCManagerAPrototype = WINFUNCTYPE(SC_HANDLE, LPCSTR, LPCSTR, DWORD)
 OpenSCManagerAParams = ((1, 'lpMachineName'), (1, 'lpDatabaseName'), (1, 'dwDesiredAccess'))
 
 #def OpenSCManagerW(lpMachineName, lpDatabaseName, dwDesiredAccess):
 #    return OpenSCManagerW.ctypes_function(lpMachineName, lpDatabaseName, dwDesiredAccess)
@@ -2501,14 +2901,54 @@
 NtDelayExecutionParams = ((1, 'Alertable'), (1, 'DelayInterval'))
 
 #def NtTerminateProcess(ProcessHandle, ExitStatus):
 #    return NtTerminateProcess.ctypes_function(ProcessHandle, ExitStatus)
 NtTerminateProcessPrototype = WINFUNCTYPE(NTSTATUS, HANDLE, NTSTATUS)
 NtTerminateProcessParams = ((1, 'ProcessHandle'), (1, 'ExitStatus'))
 
+#def GetComputerNameExA(NameType, lpBuffer, nSize):
+#    return GetComputerNameExA.ctypes_function(NameType, lpBuffer, nSize)
+GetComputerNameExAPrototype = WINFUNCTYPE(BOOL, COMPUTER_NAME_FORMAT, LPSTR, LPDWORD)
+GetComputerNameExAParams = ((1, 'NameType'), (1, 'lpBuffer'), (1, 'nSize'))
+
+#def GetComputerNameExW(NameType, lpBuffer, nSize):
+#    return GetComputerNameExW.ctypes_function(NameType, lpBuffer, nSize)
+GetComputerNameExWPrototype = WINFUNCTYPE(BOOL, COMPUTER_NAME_FORMAT, LPWSTR, LPDWORD)
+GetComputerNameExWParams = ((1, 'NameType'), (1, 'lpBuffer'), (1, 'nSize'))
+
+#def GetComputerNameA(lpBuffer, lpnSize):
+#    return GetComputerNameA.ctypes_function(lpBuffer, lpnSize)
+GetComputerNameAPrototype = WINFUNCTYPE(BOOL, LPCSTR, LPDWORD)
+GetComputerNameAParams = ((1, 'lpBuffer'), (1, 'lpnSize'))
+
+#def GetComputerNameW(lpBuffer, lpnSize):
+#    return GetComputerNameW.ctypes_function(lpBuffer, lpnSize)
+GetComputerNameWPrototype = WINFUNCTYPE(BOOL, LPWSTR, LPDWORD)
+GetComputerNameWParams = ((1, 'lpBuffer'), (1, 'lpnSize'))
+
+#def LookupAccountSidA(lpSystemName, lpSid, lpName, cchName, lpReferencedDomainName, cchReferencedDomainName, peUse):
+#    return LookupAccountSidA.ctypes_function(lpSystemName, lpSid, lpName, cchName, lpReferencedDomainName, cchReferencedDomainName, peUse)
+LookupAccountSidAPrototype = WINFUNCTYPE(BOOL, LPCSTR, PSID, LPCSTR, LPDWORD, LPCSTR, LPDWORD, PSID_NAME_USE)
+LookupAccountSidAParams = ((1, 'lpSystemName'), (1, 'lpSid'), (1, 'lpName'), (1, 'cchName'), (1, 'lpReferencedDomainName'), (1, 'cchReferencedDomainName'), (1, 'peUse'))
+
+#def LookupAccountSidW(lpSystemName, lpSid, lpName, cchName, lpReferencedDomainName, cchReferencedDomainName, peUse):
+#    return LookupAccountSidW.ctypes_function(lpSystemName, lpSid, lpName, cchName, lpReferencedDomainName, cchReferencedDomainName, peUse)
+LookupAccountSidWPrototype = WINFUNCTYPE(BOOL, LPWSTR, PSID, LPWSTR, LPDWORD, LPWSTR, LPDWORD, PSID_NAME_USE)
+LookupAccountSidWParams = ((1, 'lpSystemName'), (1, 'lpSid'), (1, 'lpName'), (1, 'cchName'), (1, 'lpReferencedDomainName'), (1, 'cchReferencedDomainName'), (1, 'peUse'))
+
+#def LookupAccountNameA(lpSystemName, lpAccountName, Sid, cbSid, ReferencedDomainName, cchReferencedDomainName, peUse):
+#    return LookupAccountNameA.ctypes_function(lpSystemName, lpAccountName, Sid, cbSid, ReferencedDomainName, cchReferencedDomainName, peUse)
+LookupAccountNameAPrototype = WINFUNCTYPE(BOOL, LPCSTR, LPCSTR, PSID, LPDWORD, LPSTR, LPDWORD, PSID_NAME_USE)
+LookupAccountNameAParams = ((1, 'lpSystemName'), (1, 'lpAccountName'), (1, 'Sid'), (1, 'cbSid'), (1, 'ReferencedDomainName'), (1, 'cchReferencedDomainName'), (1, 'peUse'))
+
+#def LookupAccountNameW(lpSystemName, lpAccountName, Sid, cbSid, ReferencedDomainName, cchReferencedDomainName, peUse):
+#    return LookupAccountNameW.ctypes_function(lpSystemName, lpAccountName, Sid, cbSid, ReferencedDomainName, cchReferencedDomainName, peUse)
+LookupAccountNameWPrototype = WINFUNCTYPE(BOOL, LPCWSTR, LPCWSTR, PSID, LPDWORD, LPWSTR, LPDWORD, PSID_NAME_USE)
+LookupAccountNameWParams = ((1, 'lpSystemName'), (1, 'lpAccountName'), (1, 'Sid'), (1, 'cbSid'), (1, 'ReferencedDomainName'), (1, 'cchReferencedDomainName'), (1, 'peUse'))
+
 #def FileTimeToSystemTime(lpFileTime, lpSystemTime):
 #    return FileTimeToSystemTime.ctypes_function(lpFileTime, lpSystemTime)
 FileTimeToSystemTimePrototype = WINFUNCTYPE(BOOL, POINTER(FILETIME), LPSYSTEMTIME)
 FileTimeToSystemTimeParams = ((1, 'lpFileTime'), (1, 'lpSystemTime'))
 
 #def SystemTimeToFileTime(lpSystemTime, lpFileTime):
 #    return SystemTimeToFileTime.ctypes_function(lpSystemTime, lpFileTime)
@@ -2746,29 +3186,14 @@
 TerminateProcessParams = ((1, 'hProcess'), (1, 'uExitCode'))
 
 #def GetLastError():
 #    return GetLastError.ctypes_function()
 GetLastErrorPrototype = WINFUNCTYPE(DWORD)
 GetLastErrorParams = ()
 
-#def GetCurrentProcess():
-#    return GetCurrentProcess.ctypes_function()
-GetCurrentProcessPrototype = WINFUNCTYPE(HANDLE)
-GetCurrentProcessParams = ()
-
-#def CreateFileA(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile):
-#    return CreateFileA.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile)
-CreateFileAPrototype = WINFUNCTYPE(HANDLE, LPCSTR, DWORD, DWORD, LPSECURITY_ATTRIBUTES, DWORD, DWORD, HANDLE)
-CreateFileAParams = ((1, 'lpFileName'), (1, 'dwDesiredAccess'), (1, 'dwShareMode'), (1, 'lpSecurityAttributes'), (1, 'dwCreationDisposition'), (1, 'dwFlagsAndAttributes'), (1, 'hTemplateFile'))
-
-#def CreateFileW(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile):
-#    return CreateFileW.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile)
-CreateFileWPrototype = WINFUNCTYPE(HANDLE, LPCWSTR, DWORD, DWORD, LPSECURITY_ATTRIBUTES, DWORD, DWORD, HANDLE)
-CreateFileWParams = ((1, 'lpFileName'), (1, 'dwDesiredAccess'), (1, 'dwShareMode'), (1, 'lpSecurityAttributes'), (1, 'dwCreationDisposition'), (1, 'dwFlagsAndAttributes'), (1, 'hTemplateFile'))
-
 #def LdrLoadDll(PathToFile, Flags, ModuleFileName, ModuleHandle):
 #    return LdrLoadDll.ctypes_function(PathToFile, Flags, ModuleFileName, ModuleHandle)
 LdrLoadDllPrototype = WINFUNCTYPE(NTSTATUS, LPCWSTR, PVOID, PUNICODE_STRING, PHANDLE)
 LdrLoadDllParams = ((1, 'PathToFile'), (1, 'Flags'), (1, 'ModuleFileName'), (1, 'ModuleHandle'))
 
 #def GetExitCodeThread(hThread, lpExitCode):
 #    return GetExitCodeThread.ctypes_function(hThread, lpExitCode)
@@ -2926,78 +3351,28 @@
 WriteProcessMemoryParams = ((1, 'hProcess'), (1, 'lpBaseAddress'), (1, 'lpBuffer'), (1, 'nSize'), (1, 'lpNumberOfBytesWritten'))
 
 #def NtWow64WriteVirtualMemory64(hProcess, lpBaseAddress, lpBuffer, nSize, lpNumberOfBytesWritten):
 #    return NtWow64WriteVirtualMemory64.ctypes_function(hProcess, lpBaseAddress, lpBuffer, nSize, lpNumberOfBytesWritten)
 NtWow64WriteVirtualMemory64Prototype = WINFUNCTYPE(NTSTATUS, HANDLE, ULONG64, LPVOID, ULONG64, PULONG64)
 NtWow64WriteVirtualMemory64Params = ((1, 'hProcess'), (1, 'lpBaseAddress'), (1, 'lpBuffer'), (1, 'nSize'), (1, 'lpNumberOfBytesWritten'))
 
-#def CreateToolhelp32Snapshot(dwFlags, th32ProcessID):
-#    return CreateToolhelp32Snapshot.ctypes_function(dwFlags, th32ProcessID)
-CreateToolhelp32SnapshotPrototype = WINFUNCTYPE(HANDLE, DWORD, DWORD)
-CreateToolhelp32SnapshotParams = ((1, 'dwFlags'), (1, 'th32ProcessID'))
-
-#def Thread32First(hSnapshot, lpte):
-#    return Thread32First.ctypes_function(hSnapshot, lpte)
-Thread32FirstPrototype = WINFUNCTYPE(BOOL, HANDLE, LPTHREADENTRY32)
-Thread32FirstParams = ((1, 'hSnapshot'), (1, 'lpte'))
-
-#def Thread32Next(hSnapshot, lpte):
-#    return Thread32Next.ctypes_function(hSnapshot, lpte)
-Thread32NextPrototype = WINFUNCTYPE(BOOL, HANDLE, LPTHREADENTRY32)
-Thread32NextParams = ((1, 'hSnapshot'), (1, 'lpte'))
-
-#def Process32First(hSnapshot, lppe):
-#    return Process32First.ctypes_function(hSnapshot, lppe)
-Process32FirstPrototype = WINFUNCTYPE(BOOL, HANDLE, LPPROCESSENTRY32)
-Process32FirstParams = ((1, 'hSnapshot'), (1, 'lppe'))
-
-#def Process32Next(hSnapshot, lppe):
-#    return Process32Next.ctypes_function(hSnapshot, lppe)
-Process32NextPrototype = WINFUNCTYPE(BOOL, HANDLE, LPPROCESSENTRY32)
-Process32NextParams = ((1, 'hSnapshot'), (1, 'lppe'))
-
-#def Process32FirstW(hSnapshot, lppe):
-#    return Process32FirstW.ctypes_function(hSnapshot, lppe)
-Process32FirstWPrototype = WINFUNCTYPE(BOOL, HANDLE, LPPROCESSENTRY32W)
-Process32FirstWParams = ((1, 'hSnapshot'), (1, 'lppe'))
-
-#def Process32NextW(hSnapshot, lppe):
-#    return Process32NextW.ctypes_function(hSnapshot, lppe)
-Process32NextWPrototype = WINFUNCTYPE(BOOL, HANDLE, LPPROCESSENTRY32W)
-Process32NextWParams = ((1, 'hSnapshot'), (1, 'lppe'))
-
-#def GetProcAddress(hModule, lpProcName):
-#    return GetProcAddress.ctypes_function(hModule, lpProcName)
-GetProcAddressPrototype = WINFUNCTYPE(FARPROC, HMODULE, LPCSTR)
-GetProcAddressParams = ((1, 'hModule'), (1, 'lpProcName'))
-
-#def LoadLibraryA(lpFileName):
-#    return LoadLibraryA.ctypes_function(lpFileName)
-LoadLibraryAPrototype = WINFUNCTYPE(HMODULE, LPCSTR)
-LoadLibraryAParams = ((1, 'lpFileName'),)
-
-#def LoadLibraryW(lpFileName):
-#    return LoadLibraryW.ctypes_function(lpFileName)
-LoadLibraryWPrototype = WINFUNCTYPE(HMODULE, LPCWSTR)
-LoadLibraryWParams = ((1, 'lpFileName'),)
-
-#def LoadLibraryExA(lpLibFileName, hFile, dwFlags):
-#    return LoadLibraryExA.ctypes_function(lpLibFileName, hFile, dwFlags)
-LoadLibraryExAPrototype = WINFUNCTYPE(HMODULE, LPCSTR, HANDLE, DWORD)
-LoadLibraryExAParams = ((1, 'lpLibFileName'), (1, 'hFile'), (1, 'dwFlags'))
+#def GetCurrentProcess():
+#    return GetCurrentProcess.ctypes_function()
+GetCurrentProcessPrototype = WINFUNCTYPE(HANDLE)
+GetCurrentProcessParams = ()
 
-#def LoadLibraryExW(lpLibFileName, hFile, dwFlags):
-#    return LoadLibraryExW.ctypes_function(lpLibFileName, hFile, dwFlags)
-LoadLibraryExWPrototype = WINFUNCTYPE(HMODULE, LPCWSTR, HANDLE, DWORD)
-LoadLibraryExWParams = ((1, 'lpLibFileName'), (1, 'hFile'), (1, 'dwFlags'))
+#def CreateFileA(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile):
+#    return CreateFileA.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile)
+CreateFileAPrototype = WINFUNCTYPE(HANDLE, LPCSTR, DWORD, DWORD, LPSECURITY_ATTRIBUTES, DWORD, DWORD, HANDLE)
+CreateFileAParams = ((1, 'lpFileName'), (1, 'dwDesiredAccess'), (1, 'dwShareMode'), (1, 'lpSecurityAttributes'), (1, 'dwCreationDisposition'), (1, 'dwFlagsAndAttributes'), (1, 'hTemplateFile'))
 
-#def FreeLibrary(hLibModule):
-#    return FreeLibrary.ctypes_function(hLibModule)
-FreeLibraryPrototype = WINFUNCTYPE(BOOL, HMODULE)
-FreeLibraryParams = ((1, 'hLibModule'),)
+#def CreateFileW(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile):
+#    return CreateFileW.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile)
+CreateFileWPrototype = WINFUNCTYPE(HANDLE, LPCWSTR, DWORD, DWORD, LPSECURITY_ATTRIBUTES, DWORD, DWORD, HANDLE)
+CreateFileWParams = ((1, 'lpFileName'), (1, 'dwDesiredAccess'), (1, 'dwShareMode'), (1, 'lpSecurityAttributes'), (1, 'dwCreationDisposition'), (1, 'dwFlagsAndAttributes'), (1, 'hTemplateFile'))
 
 #def OpenProcessToken(ProcessHandle, DesiredAccess, TokenHandle):
 #    return OpenProcessToken.ctypes_function(ProcessHandle, DesiredAccess, TokenHandle)
 OpenProcessTokenPrototype = WINFUNCTYPE(BOOL, HANDLE, DWORD, PHANDLE)
 OpenProcessTokenParams = ((1, 'ProcessHandle'), (1, 'DesiredAccess'), (1, 'TokenHandle'))
 
 #def DuplicateToken(ExistingTokenHandle, ImpersonationLevel, DuplicateTokenHandle):
@@ -3201,24 +3576,14 @@
 WaitForSingleObjectParams = ((1, 'hHandle'), (1, 'dwMilliseconds'))
 
 #def GetThreadId(Thread):
 #    return GetThreadId.ctypes_function(Thread)
 GetThreadIdPrototype = WINFUNCTYPE(DWORD, HANDLE)
 GetThreadIdParams = ((1, 'Thread'),)
 
-#def LoadLibraryExA(lpFileName, hFile, dwFlags):
-#    return LoadLibraryExA.ctypes_function(lpFileName, hFile, dwFlags)
-LoadLibraryExAPrototype = WINFUNCTYPE(HMODULE, LPCSTR, HANDLE, DWORD)
-LoadLibraryExAParams = ((1, 'lpFileName'), (1, 'hFile'), (1, 'dwFlags'))
-
-#def LoadLibraryExW(lpFileName, hFile, dwFlags):
-#    return LoadLibraryExW.ctypes_function(lpFileName, hFile, dwFlags)
-LoadLibraryExWPrototype = WINFUNCTYPE(HMODULE, LPCWSTR, HANDLE, DWORD)
-LoadLibraryExWParams = ((1, 'lpFileName'), (1, 'hFile'), (1, 'dwFlags'))
-
 #def DeviceIoControl(hDevice, dwIoControlCode, lpInBuffer, nInBufferSize, lpOutBuffer, nOutBufferSize, lpBytesReturned, lpOverlapped):
 #    return DeviceIoControl.ctypes_function(hDevice, dwIoControlCode, lpInBuffer, nInBufferSize, lpOutBuffer, nOutBufferSize, lpBytesReturned, lpOverlapped)
 DeviceIoControlPrototype = WINFUNCTYPE(BOOL, HANDLE, DWORD, LPVOID, DWORD, LPVOID, DWORD, LPDWORD, LPOVERLAPPED)
 DeviceIoControlParams = ((1, 'hDevice'), (1, 'dwIoControlCode'), (1, 'lpInBuffer'), (1, 'nInBufferSize'), (1, 'lpOutBuffer'), (1, 'nOutBufferSize'), (1, 'lpBytesReturned'), (1, 'lpOverlapped'))
 
 #def GetTokenInformation(TokenHandle, TokenInformationClass, TokenInformation, TokenInformationLength, ReturnLength):
 #    return GetTokenInformation.ctypes_function(TokenHandle, TokenInformationClass, TokenInformation, TokenInformationLength, ReturnLength)
@@ -3431,14 +3796,19 @@
 RtlDecompressBufferExParams = ((1, 'CompressionFormat'), (1, 'UncompressedBuffer'), (1, 'UncompressedBufferSize'), (1, 'CompressedBuffer'), (1, 'CompressedBufferSize'), (1, 'FinalUncompressedSize'), (1, 'WorkSpace'))
 
 #def RtlGetCompressionWorkSpaceSize(CompressionFormatAndEngine, CompressBufferWorkSpaceSize, CompressFragmentWorkSpaceSize):
 #    return RtlGetCompressionWorkSpaceSize.ctypes_function(CompressionFormatAndEngine, CompressBufferWorkSpaceSize, CompressFragmentWorkSpaceSize)
 RtlGetCompressionWorkSpaceSizePrototype = WINFUNCTYPE(NTSTATUS, USHORT, PULONG, PULONG)
 RtlGetCompressionWorkSpaceSizeParams = ((1, 'CompressionFormatAndEngine'), (1, 'CompressBufferWorkSpaceSize'), (1, 'CompressFragmentWorkSpaceSize'))
 
+#def RtlMoveMemory(Destination, Source, Length):
+#    return RtlMoveMemory.ctypes_function(Destination, Source, Length)
+RtlMoveMemoryPrototype = WINFUNCTYPE(VOID, PVOID, PVOID, SIZE_T)
+RtlMoveMemoryParams = ((1, 'Destination'), (1, 'Source'), (1, 'Length'))
+
 #def lstrcmpA(lpString1, lpString2):
 #    return lstrcmpA.ctypes_function(lpString1, lpString2)
 lstrcmpAPrototype = WINFUNCTYPE(INT, LPCSTR, LPCSTR)
 lstrcmpAParams = ((1, 'lpString1'), (1, 'lpString2'))
 
 #def lstrcmpW(lpString1, lpString2):
 #    return lstrcmpW.ctypes_function(lpString1, lpString2)
@@ -3561,44 +3931,14 @@
 GetProcessImageFileNameWParams = ((1, 'hProcess'), (1, 'lpImageFileName'), (1, 'nSize'))
 
 #def GetSystemMetrics(nIndex):
 #    return GetSystemMetrics.ctypes_function(nIndex)
 GetSystemMetricsPrototype = WINFUNCTYPE(INT, INT)
 GetSystemMetricsParams = ((1, 'nIndex'),)
 
-#def GetComputerNameA(lpBuffer, lpnSize):
-#    return GetComputerNameA.ctypes_function(lpBuffer, lpnSize)
-GetComputerNameAPrototype = WINFUNCTYPE(BOOL, LPCSTR, LPDWORD)
-GetComputerNameAParams = ((1, 'lpBuffer'), (1, 'lpnSize'))
-
-#def GetComputerNameW(lpBuffer, lpnSize):
-#    return GetComputerNameW.ctypes_function(lpBuffer, lpnSize)
-GetComputerNameWPrototype = WINFUNCTYPE(BOOL, LPWSTR, LPDWORD)
-GetComputerNameWParams = ((1, 'lpBuffer'), (1, 'lpnSize'))
-
-#def LookupAccountSidA(lpSystemName, lpSid, lpName, cchName, lpReferencedDomainName, cchReferencedDomainName, peUse):
-#    return LookupAccountSidA.ctypes_function(lpSystemName, lpSid, lpName, cchName, lpReferencedDomainName, cchReferencedDomainName, peUse)
-LookupAccountSidAPrototype = WINFUNCTYPE(BOOL, LPCSTR, PSID, LPCSTR, LPDWORD, LPCSTR, LPDWORD, PSID_NAME_USE)
-LookupAccountSidAParams = ((1, 'lpSystemName'), (1, 'lpSid'), (1, 'lpName'), (1, 'cchName'), (1, 'lpReferencedDomainName'), (1, 'cchReferencedDomainName'), (1, 'peUse'))
-
-#def LookupAccountSidW(lpSystemName, lpSid, lpName, cchName, lpReferencedDomainName, cchReferencedDomainName, peUse):
-#    return LookupAccountSidW.ctypes_function(lpSystemName, lpSid, lpName, cchName, lpReferencedDomainName, cchReferencedDomainName, peUse)
-LookupAccountSidWPrototype = WINFUNCTYPE(BOOL, LPWSTR, PSID, LPWSTR, LPDWORD, LPWSTR, LPDWORD, PSID_NAME_USE)
-LookupAccountSidWParams = ((1, 'lpSystemName'), (1, 'lpSid'), (1, 'lpName'), (1, 'cchName'), (1, 'lpReferencedDomainName'), (1, 'cchReferencedDomainName'), (1, 'peUse'))
-
-#def LookupAccountNameA(lpSystemName, lpAccountName, Sid, cbSid, ReferencedDomainName, cchReferencedDomainName, peUse):
-#    return LookupAccountNameA.ctypes_function(lpSystemName, lpAccountName, Sid, cbSid, ReferencedDomainName, cchReferencedDomainName, peUse)
-LookupAccountNameAPrototype = WINFUNCTYPE(BOOL, LPCSTR, LPCSTR, PSID, LPDWORD, LPSTR, LPDWORD, PSID_NAME_USE)
-LookupAccountNameAParams = ((1, 'lpSystemName'), (1, 'lpAccountName'), (1, 'Sid'), (1, 'cbSid'), (1, 'ReferencedDomainName'), (1, 'cchReferencedDomainName'), (1, 'peUse'))
-
-#def LookupAccountNameW(lpSystemName, lpAccountName, Sid, cbSid, ReferencedDomainName, cchReferencedDomainName, peUse):
-#    return LookupAccountNameW.ctypes_function(lpSystemName, lpAccountName, Sid, cbSid, ReferencedDomainName, cchReferencedDomainName, peUse)
-LookupAccountNameWPrototype = WINFUNCTYPE(BOOL, LPCWSTR, LPCWSTR, PSID, LPDWORD, LPWSTR, LPDWORD, PSID_NAME_USE)
-LookupAccountNameWParams = ((1, 'lpSystemName'), (1, 'lpAccountName'), (1, 'Sid'), (1, 'cbSid'), (1, 'ReferencedDomainName'), (1, 'cchReferencedDomainName'), (1, 'peUse'))
-
 #def GetInterfaceInfo(pIfTable, dwOutBufLen):
 #    return GetInterfaceInfo.ctypes_function(pIfTable, dwOutBufLen)
 GetInterfaceInfoPrototype = WINFUNCTYPE(DWORD, PIP_INTERFACE_INFO, PULONG)
 GetInterfaceInfoParams = ((1, 'pIfTable'), (1, 'dwOutBufLen'))
 
 #def GetIfTable(pIfTable, pdwSize, bOrder):
 #    return GetIfTable.ctypes_function(pIfTable, pdwSize, bOrder)
@@ -3781,7 +4121,72 @@
 GetFirmwareEnvironmentVariableExWParams = ((1, 'lpName'), (1, 'lpGuid'), (1, 'pBuffer'), (1, 'nSize'), (1, 'pdwAttribubutes'))
 
 #def IsDebuggerPresent():
 #    return IsDebuggerPresent.ctypes_function()
 IsDebuggerPresentPrototype = WINFUNCTYPE(BOOL)
 IsDebuggerPresentParams = ()
 
+#def WSAStartup(wVersionRequested, lpWSAData):
+#    return WSAStartup.ctypes_function(wVersionRequested, lpWSAData)
+WSAStartupPrototype = WINFUNCTYPE(INT, WORD, LPWSADATA)
+WSAStartupParams = ((1, 'wVersionRequested'), (1, 'lpWSAData'))
+
+#def WSACleanup():
+#    return WSACleanup.ctypes_function()
+WSACleanupPrototype = WINFUNCTYPE(INT)
+WSACleanupParams = ()
+
+#def WSAGetLastError():
+#    return WSAGetLastError.ctypes_function()
+WSAGetLastErrorPrototype = WINFUNCTYPE(INT)
+WSAGetLastErrorParams = ()
+
+#def getaddrinfo(pNodeName, pServiceName, pHints, ppResult):
+#    return getaddrinfo.ctypes_function(pNodeName, pServiceName, pHints, ppResult)
+getaddrinfoPrototype = WINFUNCTYPE(INT, PCSTR, PCSTR, POINTER(ADDRINFOA), POINTER(PADDRINFOA))
+getaddrinfoParams = ((1, 'pNodeName'), (1, 'pServiceName'), (1, 'pHints'), (1, 'ppResult'))
+
+#def GetAddrInfoW(pNodeName, pServiceName, pHints, ppResult):
+#    return GetAddrInfoW.ctypes_function(pNodeName, pServiceName, pHints, ppResult)
+GetAddrInfoWPrototype = WINFUNCTYPE(INT, PCWSTR, PCWSTR, POINTER(ADDRINFOW), POINTER(PADDRINFOW))
+GetAddrInfoWParams = ((1, 'pNodeName'), (1, 'pServiceName'), (1, 'pHints'), (1, 'ppResult'))
+
+#def WSASocketA(af, type, protocol, lpProtocolInfo, g, dwFlags):
+#    return WSASocketA.ctypes_function(af, type, protocol, lpProtocolInfo, g, dwFlags)
+WSASocketAPrototype = WINFUNCTYPE(SOCKET, INT, INT, INT, LPWSAPROTOCOL_INFOA, GROUP, DWORD)
+WSASocketAParams = ((1, 'af'), (1, 'type'), (1, 'protocol'), (1, 'lpProtocolInfo'), (1, 'g'), (1, 'dwFlags'))
+
+#def WSASocketW(af, type, protocol, lpProtocolInfo, g, dwFlags):
+#    return WSASocketW.ctypes_function(af, type, protocol, lpProtocolInfo, g, dwFlags)
+WSASocketWPrototype = WINFUNCTYPE(SOCKET, INT, INT, INT, LPWSAPROTOCOL_INFOW, GROUP, DWORD)
+WSASocketWParams = ((1, 'af'), (1, 'type'), (1, 'protocol'), (1, 'lpProtocolInfo'), (1, 'g'), (1, 'dwFlags'))
+
+#def socket(af, type, protocol):
+#    return socket.ctypes_function(af, type, protocol)
+socketPrototype = WINFUNCTYPE(SOCKET, INT, INT, INT)
+socketParams = ((1, 'af'), (1, 'type'), (1, 'protocol'))
+
+#def connect(s, name, namelen):
+#    return connect.ctypes_function(s, name, namelen)
+connectPrototype = WINFUNCTYPE(INT, SOCKET, POINTER(sockaddr), INT)
+connectParams = ((1, 's'), (1, 'name'), (1, 'namelen'))
+
+#def send(s, buf, len, flags):
+#    return send.ctypes_function(s, buf, len, flags)
+sendPrototype = WINFUNCTYPE(INT, SOCKET, POINTER(CHAR), INT, INT)
+sendParams = ((1, 's'), (1, 'buf'), (1, 'len'), (1, 'flags'))
+
+#def recv(s, buf, len, flags):
+#    return recv.ctypes_function(s, buf, len, flags)
+recvPrototype = WINFUNCTYPE(INT, SOCKET, POINTER(CHAR), INT, INT)
+recvParams = ((1, 's'), (1, 'buf'), (1, 'len'), (1, 'flags'))
+
+#def shutdown(s, how):
+#    return shutdown.ctypes_function(s, how)
+shutdownPrototype = WINFUNCTYPE(INT, SOCKET, INT)
+shutdownParams = ((1, 's'), (1, 'how'))
+
+#def closesocket(s):
+#    return closesocket.ctypes_function(s)
+closesocketPrototype = WINFUNCTYPE(INT, SOCKET)
+closesocketParams = ((1, 's'),)
+
```

### Comparing `PythonForWindows-0.6.5/windows/generated_def/winstructs.py` & `PythonForWindows-0.6.8/windows/generated_def/winstructs.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 PULONG = POINTER(ULONG)
 PDWORD = POINTER(DWORD)
 LPDWORD = POINTER(DWORD)
 LPBYTE = POINTER(BYTE)
 ULONG_PTR = PVOID
 LONG_PTR = PVOID
 DWORD_PTR = ULONG_PTR
+PDWORD_PTR = POINTER(DWORD_PTR)
 KAFFINITY = ULONG_PTR
 KPRIORITY = LONG
 INTERNET_PORT = WORD
 CHAR = c_char
 PCHAR = POINTER(CHAR)
 UCHAR = c_char
 CSHORT = c_short
@@ -132,14 +133,15 @@
 LPPOINT = POINTER(POINT)
 LPRECT = POINTER(RECT)
 SPC_UUID = BYTE*16
 DEVICE_TYPE = DWORD
 PWINDBG_EXTENSION_APIS32 = PVOID
 PWINDBG_EXTENSION_APIS64 = PVOID
 FILEOP_FLAGS = WORD
+NET_API_STATUS = DWORD
 NCRYPT_HANDLE = ULONG_PTR
 NCRYPT_PROV_HANDLE = ULONG_PTR
 NCRYPT_KEY_HANDLE = ULONG_PTR
 NCRYPT_HASH_HANDLE = ULONG_PTR
 NCRYPT_SECRET_HANDLE = ULONG_PTR
 TRACEHANDLE = ULONG64
 PTRACEHANDLE = POINTER(TRACEHANDLE)
@@ -248,14 +250,16 @@
 DEVNODEID_A = PCSTR
 DEVINSTID_A = PCSTR
 DEVNODEID_W = LPWSTR
 DEVINSTID_W = LPWSTR
 RPCOLEDATAREP = ULONG
 HREFTYPE = DWORD
 SFGAOF = ULONG
+GROUP = UINT
+SOCKET = HANDLE
 WNDPROC = PVOID
 LPPROC_THREAD_ATTRIBUTE_LIST = PVOID
 PPS_POST_PROCESS_INIT_ROUTINE = PVOID
 LPTHREAD_START_ROUTINE = PVOID
 WNDENUMPROC = PVOID
 PHANDLER_ROUTINE = PVOID
 FARPROC = PVOID
@@ -282,19 +286,22 @@
 PSYM_ENUMPROCESSES_CALLBACK = PVOID#Symbols
 ENUMRESNAMEPROCA = PVOID#Resources
 ENUMRESNAMEPROCW = PVOID#Resources
 ENUMRESTYPEPROCA = PVOID#Resources
 ENUMRESTYPEPROCW = PVOID#Resources
 LPSERVICE_MAIN_FUNCTIONA = PVOID
 LPSERVICE_MAIN_FUNCTIONW = PVOID
+LPOVERLAPPED_COMPLETION_ROUTINE = PVOID
+PDNS_QUERY_COMPLETION_ROUTINE = PVOID
 LPCONTEXT = PVOID
 HCERTSTORE = PVOID
 HCRYPTMSG = PVOID
 PALPC_PORT_ATTRIBUTES = PVOID
 PPORT_MESSAGE = PVOID
+LPWSADATA = PVOID
 FC_ZERO = EnumValue("NDR_FORMAT_CHARACTER", "FC_ZERO", 0x0)
 FC_BYTE = EnumValue("NDR_FORMAT_CHARACTER", "FC_BYTE", 0x1)
 FC_CHAR = EnumValue("NDR_FORMAT_CHARACTER", "FC_CHAR", 0x2)
 FC_SMALL = EnumValue("NDR_FORMAT_CHARACTER", "FC_SMALL", 0x3)
 FC_USMALL = EnumValue("NDR_FORMAT_CHARACTER", "FC_USMALL", 0x4)
 FC_WCHAR = EnumValue("NDR_FORMAT_CHARACTER", "FC_WCHAR", 0x5)
 FC_SHORT = EnumValue("NDR_FORMAT_CHARACTER", "FC_SHORT", 0x6)
@@ -954,14 +961,15 @@
         ("fFeatures", USHORT),
         ("cbElements", ULONG),
         ("cLocks", ULONG),
         ("pvData", PVOID),
         ("rgsabound", SAFEARRAYBOUND * (1)),
     ]
 SAFEARRAY = tagSAFEARRAY
+LPSAFEARRAY = POINTER(tagSAFEARRAY)
 
 class __tagBRECORD(Structure):
     _fields_ = [
         ("pvRecord", PVOID),
         ("pRecInfo", PVOID),
     ]
 _tagBRECORD = __tagBRECORD
@@ -2331,14 +2339,126 @@
     ("wDataLength", WORD),
     ("Flags", _ANON__DNSRECORDW_SUB_UNION_1),
     ("dwTtl", DWORD),
     ("dwReserved", DWORD),
     ("Data", _ANON__DNSRECORDW_SUB_UNION_2),
 ]
 
+class _DnsAddr(Structure):
+    _fields_ = [
+        ("MaxSa", CHAR * (DNS_ADDR_MAX_SOCKADDR_LENGTH)),
+        ("DnsAddrUserDword", DWORD * (8)),
+    ]
+PDNS_ADDR = POINTER(_DnsAddr)
+DNS_ADDR = _DnsAddr
+
+class _DnsAddrArray(Structure):
+    _fields_ = [
+        ("MaxCount", DWORD),
+        ("AddrCount", DWORD),
+        ("Tag", DWORD),
+        ("Family", WORD),
+        ("WordReserved", WORD),
+        ("Flags", DWORD),
+        ("MatchFlag", DWORD),
+        ("Reserved1", DWORD),
+        ("Reserved2", DWORD),
+        ("AddrArray", DNS_ADDR * (ANY_SIZE)),
+    ]
+PDNS_ADDR_ARRAY = POINTER(_DnsAddrArray)
+DNS_ADDR_ARRAY = _DnsAddrArray
+
+class _DNS_QUERY_REQUEST(Structure):
+    _fields_ = [
+        ("Version", ULONG),
+        ("QueryName", PCWSTR),
+        ("QueryType", WORD),
+        ("QueryOptions", ULONG64),
+        ("pDnsServerList", PDNS_ADDR_ARRAY),
+        ("InterfaceIndex", ULONG),
+        ("pQueryCompletionCallback", PDNS_QUERY_COMPLETION_ROUTINE),
+        ("pQueryContext", PVOID),
+    ]
+PDNS_QUERY_REQUEST = POINTER(_DNS_QUERY_REQUEST)
+DNS_QUERY_REQUEST = _DNS_QUERY_REQUEST
+
+class _DNS_QUERY_CANCEL(Structure):
+    _fields_ = [
+        ("Reserved", CHAR * (32)),
+    ]
+PDNS_QUERY_CANCEL = POINTER(_DNS_QUERY_CANCEL)
+DNS_QUERY_CANCEL = _DNS_QUERY_CANCEL
+
+class _DNS_QUERY_RESULT(Structure):
+    _fields_ = [
+        ("Version", ULONG),
+        ("QueryStatus", DNS_STATUS),
+        ("QueryOptions", ULONG64),
+        ("pQueryRecords", PVOID),
+        ("Reserved", PVOID),
+    ]
+DNS_QUERY_RESULT = _DNS_QUERY_RESULT
+PDNS_QUERY_RESULT = POINTER(_DNS_QUERY_RESULT)
+
+class IP_ADDRESS_STRING(Structure):
+    _fields_ = [
+        ("String", CHAR * (4 * 4)),
+    ]
+IP_MASK_STRING = IP_ADDRESS_STRING
+PIP_MASK_STRING = POINTER(IP_ADDRESS_STRING)
+PIP_ADDRESS_STRING = POINTER(IP_ADDRESS_STRING)
+
+# Self referencing struct tricks
+class _IP_ADDR_STRING(Structure): pass
+PIP_ADDR_STRING = POINTER(_IP_ADDR_STRING)
+IP_ADDR_STRING = _IP_ADDR_STRING
+_IP_ADDR_STRING._fields_ = [
+    ("Next", POINTER(_IP_ADDR_STRING)),
+    ("IpAddress", IP_ADDRESS_STRING),
+    ("IpMask", IP_MASK_STRING),
+    ("Context", DWORD),
+]
+
+# Self referencing struct tricks
+class _IP_ADAPTER_INFO(Structure): pass
+IP_ADAPTER_INFO = _IP_ADAPTER_INFO
+PIP_ADAPTER_INFO = POINTER(_IP_ADAPTER_INFO)
+_IP_ADAPTER_INFO._fields_ = [
+    ("Next", POINTER(_IP_ADAPTER_INFO)),
+    ("ComboIndex", DWORD),
+    ("AdapterName", CHAR * (MAX_ADAPTER_NAME_LENGTH + 4)),
+    ("Description", CHAR * (MAX_ADAPTER_DESCRIPTION_LENGTH + 4)),
+    ("AddressLength", UINT),
+    ("Address", BYTE * (MAX_ADAPTER_ADDRESS_LENGTH)),
+    ("Index", DWORD),
+    ("Type", UINT),
+    ("DhcpEnabled", UINT),
+    ("CurrentIpAddress", PIP_ADDR_STRING),
+    ("IpAddressList", IP_ADDR_STRING),
+    ("GatewayList", IP_ADDR_STRING),
+    ("DhcpServer", IP_ADDR_STRING),
+    ("HaveWins", BOOL),
+    ("PrimaryWinsServer", IP_ADDR_STRING),
+    ("SecondaryWinsServer", IP_ADDR_STRING),
+    ("LeaseObtained", ULONGLONG),
+    ("LeaseExpires", ULONGLONG),
+]
+
+class _IP_PER_ADAPTER_INFO_W2KSP1(Structure):
+    _fields_ = [
+        ("AutoconfigEnabled", UINT),
+        ("AutoconfigActive", UINT),
+        ("CurrentDnsServer", PIP_ADDR_STRING),
+        ("DnsServerList", IP_ADDR_STRING),
+    ]
+PIP_PER_ADAPTER_INFO = POINTER(_IP_PER_ADAPTER_INFO_W2KSP1)
+IP_PER_ADAPTER_INFO = _IP_PER_ADAPTER_INFO_W2KSP1
+PIP_PER_ADAPTER_INFO_W2KSP1 = POINTER(_IP_PER_ADAPTER_INFO_W2KSP1)
+IP_PER_ADAPTER_INFO_W2KSP1 = _IP_PER_ADAPTER_INFO_W2KSP1
+
 KeyValueBasicInformation = EnumValue("_KEY_VALUE_INFORMATION_CLASS", "KeyValueBasicInformation", 0x0)
 KeyValueFullInformation = EnumValue("_KEY_VALUE_INFORMATION_CLASS", "KeyValueFullInformation", 0x1)
 KeyValuePartialInformation = EnumValue("_KEY_VALUE_INFORMATION_CLASS", "KeyValuePartialInformation", 0x2)
 KeyValueFullInformationAlign64 = EnumValue("_KEY_VALUE_INFORMATION_CLASS", "KeyValueFullInformationAlign64", 0x3)
 KeyValuePartialInformationAlign64 = EnumValue("_KEY_VALUE_INFORMATION_CLASS", "KeyValuePartialInformationAlign64", 0x4)
 KeyValueLayerInformation = EnumValue("_KEY_VALUE_INFORMATION_CLASS", "KeyValueLayerInformation", 0x5)
 MaxKeyValueInfoClass = EnumValue("_KEY_VALUE_INFORMATION_CLASS", "MaxKeyValueInfoClass", 0x6)
@@ -5380,19 +5500,33 @@
     ]
 PRTL_OSVERSIONINFOEXW = POINTER(_OSVERSIONINFOEXW)
 LPOSVERSIONINFOEXW = POINTER(_OSVERSIONINFOEXW)
 OSVERSIONINFOEXW = _OSVERSIONINFOEXW
 POSVERSIONINFOEXW = POINTER(_OSVERSIONINFOEXW)
 RTL_OSVERSIONINFOEXW = _OSVERSIONINFOEXW
 
+class _ANON__ANON__OVERLAPPED_SUB_UNION_1_SUB_STRUCTURE_1(Structure):
+    _fields_ = [
+        ("Offset", DWORD),
+        ("OffsetHigh", DWORD),
+    ]
+
+class _ANON__OVERLAPPED_SUB_UNION_1(Union):
+    _anonymous_ = ("_ANON_OVERLAPPED_DUMMYSTRUCTNAME",)
+    _fields_ = [
+        ("_ANON_OVERLAPPED_DUMMYSTRUCTNAME", _ANON__ANON__OVERLAPPED_SUB_UNION_1_SUB_STRUCTURE_1),
+        ("Pointer", PVOID),
+    ]
+
 class _OVERLAPPED(Structure):
+    _anonymous_ = ("_ANON_OVERLAPPED_DUMMYUNIONNAME",)
     _fields_ = [
         ("Internal", ULONG_PTR),
         ("InternalHigh", ULONG_PTR),
-        ("Pointer", PVOID),
+        ("_ANON_OVERLAPPED_DUMMYUNIONNAME", _ANON__OVERLAPPED_SUB_UNION_1),
         ("hEvent", HANDLE),
     ]
 LPOVERLAPPED = POINTER(_OVERLAPPED)
 OVERLAPPED = _OVERLAPPED
 
 # Self referencing struct tricks
 class _EXCEPTION_RECORD(Structure): pass
@@ -5809,15 +5943,16 @@
         self.SecurityDescriptor = 0
         self.SecurityQualityOfService = 0
         return self
 
     def __repr__(self):
         if not self.ObjectName:
             return super(_OBJECT_ATTRIBUTES, self).__repr__()
-        return """<{0} ObjectName="{1}">""".format(type(self).__name__, self.ObjectName[0].str)
+        # .contents allow compatibility with remotectypes
+        return """<{0} ObjectName="{1}">""".format(type(self).__name__, self.ObjectName.contents.str)
 POBJECT_ATTRIBUTES = POINTER(_OBJECT_ATTRIBUTES)
 OBJECT_ATTRIBUTES = _OBJECT_ATTRIBUTES
 class _TMP_UNION_IO_STATUS_BLOCK(Union):
     _fields_ = [
         ("Status", NTSTATUS),
         ("Pointer", PVOID),
     ]
@@ -8531,14 +8666,23 @@
 MaxIoPriorityTypes = EnumValue("_IO_PRIORITY_HINT", "MaxIoPriorityTypes", 0x5)
 class _IO_PRIORITY_HINT(EnumType):
     values = [IoPriorityVeryLow, IoPriorityLow, IoPriorityNormal, IoPriorityHigh, IoPriorityCritical, MaxIoPriorityTypes]
     mapper = FlagMapper(*values)
 IO_PRIORITY_HINT = _IO_PRIORITY_HINT
 
 
+ReadDirectoryNotifyInformation = EnumValue("_READ_DIRECTORY_NOTIFY_INFORMATION_CLASS", "ReadDirectoryNotifyInformation", 0x0)
+ReadDirectoryNotifyExtendedInformation = EnumValue("_READ_DIRECTORY_NOTIFY_INFORMATION_CLASS", "ReadDirectoryNotifyExtendedInformation", 0x1)
+class _READ_DIRECTORY_NOTIFY_INFORMATION_CLASS(EnumType):
+    values = [ReadDirectoryNotifyInformation, ReadDirectoryNotifyExtendedInformation]
+    mapper = FlagMapper(*values)
+PREAD_DIRECTORY_NOTIFY_INFORMATION_CLASS = POINTER(_READ_DIRECTORY_NOTIFY_INFORMATION_CLASS)
+READ_DIRECTORY_NOTIFY_INFORMATION_CLASS = _READ_DIRECTORY_NOTIFY_INFORMATION_CLASS
+
+
 class _FILE_INTERNAL_INFORMATION(Structure):
     _fields_ = [
         ("IndexNumber", LARGE_INTEGER),
     ]
 FILE_INTERNAL_INFORMATION = _FILE_INTERNAL_INFORMATION
 PFILE_INTERNAL_INFORMATION = POINTER(_FILE_INTERNAL_INFORMATION)
 
@@ -8766,14 +8910,75 @@
         ("dwCreatorType", DWORD),
         ("wFinderFlags", WORD),
     ]
 PWIN32_FIND_DATAW = POINTER(_WIN32_FIND_DATAW)
 WIN32_FIND_DATAW = _WIN32_FIND_DATAW
 LPWIN32_FIND_DATAW = POINTER(_WIN32_FIND_DATAW)
 
+class _FILE_NOTIFY_INFORMATION(Structure):
+    _fields_ = [
+        ("NextEntryOffset", DWORD),
+        ("Action", DWORD),
+        ("FileNameLength", DWORD),
+        ("FileName", WCHAR * (1)),
+    ]
+FILE_NOTIFY_INFORMATION = _FILE_NOTIFY_INFORMATION
+PFILE_NOTIFY_INFORMATION = POINTER(_FILE_NOTIFY_INFORMATION)
+
+class _FILE_NOTIFY_EXTENDED_INFORMATION(Structure):
+    _fields_ = [
+        ("NextEntryOffset", DWORD),
+        ("Action", DWORD),
+        ("CreationTime", LARGE_INTEGER),
+        ("LastModificationTime", LARGE_INTEGER),
+        ("LastChangeTime", LARGE_INTEGER),
+        ("LastAccessTime", LARGE_INTEGER),
+        ("AllocatedLength", LARGE_INTEGER),
+        ("FileSize", LARGE_INTEGER),
+        ("FileAttributes", DWORD),
+        ("ReparsePointTag", DWORD),
+        ("FileId", LARGE_INTEGER),
+        ("ParentFileId", LARGE_INTEGER),
+        ("FileNameLength", DWORD),
+        ("FileName", WCHAR * (1)),
+    ]
+PFILE_NOTIFY_EXTENDED_INFORMATION = POINTER(_FILE_NOTIFY_EXTENDED_INFORMATION)
+FILE_NOTIFY_EXTENDED_INFORMATION = _FILE_NOTIFY_EXTENDED_INFORMATION
+
+class _ANON__FILE_RENAME_INFORMATION_SUB_UNION_1(Union):
+    _fields_ = [
+        ("ReplaceIfExists", BOOLEAN),
+        ("Flags", ULONG),
+    ]
+
+class _FILE_RENAME_INFORMATION(Structure):
+    _anonymous_ = ("__ANON_DUMMYUNIONNAME_FILE_RENAME_INFORMATION",)
+    _fields_ = [
+        ("__ANON_DUMMYUNIONNAME_FILE_RENAME_INFORMATION", _ANON__FILE_RENAME_INFORMATION_SUB_UNION_1),
+        ("RootDirectory", HANDLE),
+        ("FileNameLength", ULONG),
+        ("FileName", WCHAR * (1)),
+    ]
+FILE_RENAME_INFORMATION = _FILE_RENAME_INFORMATION
+PFILE_RENAME_INFORMATION = POINTER(_FILE_RENAME_INFORMATION)
+
+INITIAL_FILE_RENAME_INFORMATION = _FILE_RENAME_INFORMATION
+
+class _FILE_RENAME_INFORMATION(INITIAL_FILE_RENAME_INFORMATION):
+    @property
+    def filename(self):
+        filename_addr = ctypes.addressof(self) + type(self).FileName.offset
+        if getattr(self, "_target", None) is not None: #remote ctypes :D -> TRICKS OF THE YEAR
+            raw_data = self._target.read_memory(filename_addr, self.FileNameLength)
+            return raw_data.decode("utf16")
+        size = int(self.FileNameLength / 2)
+        return (ctypes.c_wchar * size).from_address(filename_addr)[:]
+
+FILE_RENAME_INFORMATION = _FILE_RENAME_INFORMATION
+PFILE_RENAME_INFORMATION = POINTER(_FILE_RENAME_INFORMATION)
 PolicyAuditLogInformation = EnumValue("_POLICY_INFORMATION_CLASS", "PolicyAuditLogInformation", 0x1)
 PolicyAuditEventsInformation = EnumValue("_POLICY_INFORMATION_CLASS", "PolicyAuditEventsInformation", 0x2)
 PolicyPrimaryDomainInformation = EnumValue("_POLICY_INFORMATION_CLASS", "PolicyPrimaryDomainInformation", 0x3)
 PolicyPdAccountInformation = EnumValue("_POLICY_INFORMATION_CLASS", "PolicyPdAccountInformation", 0x4)
 PolicyAccountDomainInformation = EnumValue("_POLICY_INFORMATION_CLASS", "PolicyAccountDomainInformation", 0x5)
 PolicyLsaServerRoleInformation = EnumValue("_POLICY_INFORMATION_CLASS", "PolicyLsaServerRoleInformation", 0x6)
 PolicyReplicaSourceInformation = EnumValue("_POLICY_INFORMATION_CLASS", "PolicyReplicaSourceInformation", 0x7)
@@ -8885,14 +9090,307 @@
     _fields_ = [
         ("Entries", ULONG),
         ("Domains", PLSA_TRUST_INFORMATION),
     ]
 LSA_REFERENCED_DOMAIN_LIST = _LSA_REFERENCED_DOMAIN_LIST
 PLSA_REFERENCED_DOMAIN_LIST = POINTER(_LSA_REFERENCED_DOMAIN_LIST)
 
+class _LOCALGROUP_INFO_0(Structure):
+    _fields_ = [
+        ("lgrpi0_name", LPWSTR),
+    ]
+LPLOCALGROUP_INFO_0 = POINTER(_LOCALGROUP_INFO_0)
+LOCALGROUP_INFO_0 = _LOCALGROUP_INFO_0
+PLOCALGROUP_INFO_0 = POINTER(_LOCALGROUP_INFO_0)
+
+class _LOCALGROUP_INFO_1(Structure):
+    _fields_ = [
+        ("lgrpi1_name", LPWSTR),
+        ("lgrpi1_comment", LPWSTR),
+    ]
+LPLOCALGROUP_INFO_1 = POINTER(_LOCALGROUP_INFO_1)
+LOCALGROUP_INFO_1 = _LOCALGROUP_INFO_1
+PLOCALGROUP_INFO_1 = POINTER(_LOCALGROUP_INFO_1)
+
+class _LOCALGROUP_MEMBERS_INFO_0(Structure):
+    _fields_ = [
+        ("lgrmi0_sid", PSID),
+    ]
+LPLOCALGROUP_MEMBERS_INFO_0 = POINTER(_LOCALGROUP_MEMBERS_INFO_0)
+LOCALGROUP_MEMBERS_INFO_0 = _LOCALGROUP_MEMBERS_INFO_0
+PLOCALGROUP_MEMBERS_INFO_0 = POINTER(_LOCALGROUP_MEMBERS_INFO_0)
+
+class _LOCALGROUP_MEMBERS_INFO_1(Structure):
+    _fields_ = [
+        ("lgrmi1_sid", PSID),
+        ("lgrmi1_sidusage", SID_NAME_USE),
+        ("lgrmi1_name", LPWSTR),
+    ]
+LPLOCALGROUP_MEMBERS_INFO_1 = POINTER(_LOCALGROUP_MEMBERS_INFO_1)
+LOCALGROUP_MEMBERS_INFO_1 = _LOCALGROUP_MEMBERS_INFO_1
+PLOCALGROUP_MEMBERS_INFO_1 = POINTER(_LOCALGROUP_MEMBERS_INFO_1)
+
+class _LOCALGROUP_MEMBERS_INFO_2(Structure):
+    _fields_ = [
+        ("lgrmi2_sid", PSID),
+        ("lgrmi2_sidusage", SID_NAME_USE),
+        ("lgrmi2_domainandname", LPWSTR),
+    ]
+LPLOCALGROUP_MEMBERS_INFO_2 = POINTER(_LOCALGROUP_MEMBERS_INFO_2)
+PLOCALGROUP_MEMBERS_INFO_2 = POINTER(_LOCALGROUP_MEMBERS_INFO_2)
+LOCALGROUP_MEMBERS_INFO_2 = _LOCALGROUP_MEMBERS_INFO_2
+
+class _LOCALGROUP_MEMBERS_INFO_3(Structure):
+    _fields_ = [
+        ("lgrmi3_domainandname", LPWSTR),
+    ]
+LPLOCALGROUP_MEMBERS_INFO_3 = POINTER(_LOCALGROUP_MEMBERS_INFO_3)
+PLOCALGROUP_MEMBERS_INFO_3 = POINTER(_LOCALGROUP_MEMBERS_INFO_3)
+LOCALGROUP_MEMBERS_INFO_3 = _LOCALGROUP_MEMBERS_INFO_3
+
+class _NET_DISPLAY_USER(Structure):
+    _fields_ = [
+        ("usri1_name", LPWSTR),
+        ("usri1_comment", LPWSTR),
+        ("usri1_flags", DWORD),
+        ("usri1_full_name", LPWSTR),
+        ("usri1_user_id", DWORD),
+        ("usri1_next_index", DWORD),
+    ]
+NET_DISPLAY_USER = _NET_DISPLAY_USER
+PNET_DISPLAY_USER = POINTER(_NET_DISPLAY_USER)
+
+class _NET_DISPLAY_MACHINE(Structure):
+    _fields_ = [
+        ("usri2_name", LPWSTR),
+        ("usri2_comment", LPWSTR),
+        ("usri2_flags", DWORD),
+        ("usri2_user_id", DWORD),
+        ("usri2_next_index", DWORD),
+    ]
+PNET_DISPLAY_MACHINE = POINTER(_NET_DISPLAY_MACHINE)
+NET_DISPLAY_MACHINE = _NET_DISPLAY_MACHINE
+
+class _NET_DISPLAY_GROUP(Structure):
+    _fields_ = [
+        ("grpi3_name", LPWSTR),
+        ("grpi3_comment", LPWSTR),
+        ("grpi3_group_id", DWORD),
+        ("grpi3_attributes", DWORD),
+        ("grpi3_next_index", DWORD),
+    ]
+PNET_DISPLAY_GROUP = POINTER(_NET_DISPLAY_GROUP)
+NET_DISPLAY_GROUP = _NET_DISPLAY_GROUP
+
+class _USER_INFO_0(Structure):
+    _fields_ = [
+        ("usri0_name", LPWSTR),
+    ]
+PUSER_INFO_0 = POINTER(_USER_INFO_0)
+LPUSER_INFO_0 = POINTER(_USER_INFO_0)
+USER_INFO_0 = _USER_INFO_0
+
+class _USER_INFO_1(Structure):
+    _fields_ = [
+        ("usri1_name", LPWSTR),
+        ("usri1_password", LPWSTR),
+        ("usri1_password_age", DWORD),
+        ("usri1_priv", DWORD),
+        ("usri1_home_dir", LPWSTR),
+        ("usri1_comment", LPWSTR),
+        ("usri1_flags", DWORD),
+        ("usri1_script_path", LPWSTR),
+    ]
+PUSER_INFO_1 = POINTER(_USER_INFO_1)
+LPUSER_INFO_1 = POINTER(_USER_INFO_1)
+USER_INFO_1 = _USER_INFO_1
+
+class _USER_INFO_2(Structure):
+    _fields_ = [
+        ("usri2_name", LPWSTR),
+        ("usri2_password", LPWSTR),
+        ("usri2_password_age", DWORD),
+        ("usri2_priv", DWORD),
+        ("usri2_home_dir", LPWSTR),
+        ("usri2_comment", LPWSTR),
+        ("usri2_flags", DWORD),
+        ("usri2_script_path", LPWSTR),
+        ("usri2_auth_flags", DWORD),
+        ("usri2_full_name", LPWSTR),
+        ("usri2_usr_comment", LPWSTR),
+        ("usri2_parms", LPWSTR),
+        ("usri2_workstations", LPWSTR),
+        ("usri2_last_logon", DWORD),
+        ("usri2_last_logoff", DWORD),
+        ("usri2_acct_expires", DWORD),
+        ("usri2_max_storage", DWORD),
+        ("usri2_units_per_week", DWORD),
+        ("usri2_logon_hours", PBYTE),
+        ("usri2_bad_pw_count", DWORD),
+        ("usri2_num_logons", DWORD),
+        ("usri2_logon_server", LPWSTR),
+        ("usri2_country_code", DWORD),
+        ("usri2_code_page", DWORD),
+    ]
+PUSER_INFO_2 = POINTER(_USER_INFO_2)
+USER_INFO_2 = _USER_INFO_2
+LPUSER_INFO_2 = POINTER(_USER_INFO_2)
+
+class _USER_INFO_3(Structure):
+    _fields_ = [
+        ("usri3_name", LPWSTR),
+        ("usri3_password", LPWSTR),
+        ("usri3_password_age", DWORD),
+        ("usri3_priv", DWORD),
+        ("usri3_home_dir", LPWSTR),
+        ("usri3_comment", LPWSTR),
+        ("usri3_flags", DWORD),
+        ("usri3_script_path", LPWSTR),
+        ("usri3_auth_flags", DWORD),
+        ("usri3_full_name", LPWSTR),
+        ("usri3_usr_comment", LPWSTR),
+        ("usri3_parms", LPWSTR),
+        ("usri3_workstations", LPWSTR),
+        ("usri3_last_logon", DWORD),
+        ("usri3_last_logoff", DWORD),
+        ("usri3_acct_expires", DWORD),
+        ("usri3_max_storage", DWORD),
+        ("usri3_units_per_week", DWORD),
+        ("usri3_logon_hours", PBYTE),
+        ("usri3_bad_pw_count", DWORD),
+        ("usri3_num_logons", DWORD),
+        ("usri3_logon_server", LPWSTR),
+        ("usri3_country_code", DWORD),
+        ("usri3_code_page", DWORD),
+        ("usri3_user_id", DWORD),
+        ("usri3_primary_group_id", DWORD),
+        ("usri3_profile", LPWSTR),
+        ("usri3_home_dir_drive", LPWSTR),
+        ("usri3_password_expired", DWORD),
+    ]
+PUSER_INFO_3 = POINTER(_USER_INFO_3)
+USER_INFO_3 = _USER_INFO_3
+LPUSER_INFO_3 = POINTER(_USER_INFO_3)
+
+class _USER_INFO_10(Structure):
+    _fields_ = [
+        ("usri10_name", LPWSTR),
+        ("usri10_comment", LPWSTR),
+        ("usri10_usr_comment", LPWSTR),
+        ("usri10_full_name", LPWSTR),
+    ]
+USER_INFO_10 = _USER_INFO_10
+PUSER_INFO_10 = POINTER(_USER_INFO_10)
+LPUSER_INFO_10 = POINTER(_USER_INFO_10)
+
+class _USER_INFO_11(Structure):
+    _fields_ = [
+        ("usri11_name", LPWSTR),
+        ("usri11_comment", LPWSTR),
+        ("usri11_usr_comment", LPWSTR),
+        ("usri11_full_name", LPWSTR),
+        ("usri11_priv", DWORD),
+        ("usri11_auth_flags", DWORD),
+        ("usri11_password_age", DWORD),
+        ("usri11_home_dir", LPWSTR),
+        ("usri11_parms", LPWSTR),
+        ("usri11_last_logon", DWORD),
+        ("usri11_last_logoff", DWORD),
+        ("usri11_bad_pw_count", DWORD),
+        ("usri11_num_logons", DWORD),
+        ("usri11_logon_server", LPWSTR),
+        ("usri11_country_code", DWORD),
+        ("usri11_workstations", LPWSTR),
+        ("usri11_max_storage", DWORD),
+        ("usri11_units_per_week", DWORD),
+        ("usri11_logon_hours", PBYTE),
+        ("usri11_code_page", DWORD),
+    ]
+PUSER_INFO_11 = POINTER(_USER_INFO_11)
+USER_INFO_11 = _USER_INFO_11
+LPUSER_INFO_11 = POINTER(_USER_INFO_11)
+
+class _USER_INFO_20(Structure):
+    _fields_ = [
+        ("usri20_name", LPWSTR),
+        ("usri20_full_name", LPWSTR),
+        ("usri20_comment", LPWSTR),
+        ("usri20_flags", DWORD),
+        ("usri20_user_id", DWORD),
+    ]
+PUSER_INFO_20 = POINTER(_USER_INFO_20)
+USER_INFO_20 = _USER_INFO_20
+LPUSER_INFO_20 = POINTER(_USER_INFO_20)
+
+class _USER_INFO_23(Structure):
+    _fields_ = [
+        ("usri23_name", LPWSTR),
+        ("usri23_full_name", LPWSTR),
+        ("usri23_comment", LPWSTR),
+        ("usri23_flags", DWORD),
+        ("usri23_user_sid", PSID),
+    ]
+USER_INFO_23 = _USER_INFO_23
+PUSER_INFO_23 = POINTER(_USER_INFO_23)
+LPUSER_INFO_23 = POINTER(_USER_INFO_23)
+
+class _GROUP_INFO_0(Structure):
+    _fields_ = [
+        ("grpi0_name", LPWSTR),
+    ]
+PGROUP_INFO_0 = POINTER(_GROUP_INFO_0)
+GROUP_INFO_0 = _GROUP_INFO_0
+LPGROUP_INFO_0 = POINTER(_GROUP_INFO_0)
+
+class _GROUP_INFO_1(Structure):
+    _fields_ = [
+        ("grpi1_name", LPWSTR),
+        ("grpi1_comment", LPWSTR),
+    ]
+GROUP_INFO_1 = _GROUP_INFO_1
+PGROUP_INFO_1 = POINTER(_GROUP_INFO_1)
+LPGROUP_INFO_1 = POINTER(_GROUP_INFO_1)
+
+class _GROUP_INFO_2(Structure):
+    _fields_ = [
+        ("grpi2_name", LPWSTR),
+        ("grpi2_comment", LPWSTR),
+        ("grpi2_group_id", DWORD),
+        ("grpi2_attributes", DWORD),
+    ]
+PGROUP_INFO_2 = POINTER(_GROUP_INFO_2)
+GROUP_INFO_2 = _GROUP_INFO_2
+
+class _GROUP_INFO_3(Structure):
+    _fields_ = [
+        ("grpi3_name", LPWSTR),
+        ("grpi3_comment", LPWSTR),
+        ("grpi3_group_sid", PSID),
+        ("grpi3_attributes", DWORD),
+    ]
+GROUP_INFO_3 = _GROUP_INFO_3
+PGROUP_INFO_3 = POINTER(_GROUP_INFO_3)
+
+class _GROUP_USERS_INFO_0(Structure):
+    _fields_ = [
+        ("grui0_name", LPWSTR),
+    ]
+GROUP_USERS_INFO_0 = _GROUP_USERS_INFO_0
+PGROUP_USERS_INFO_0 = POINTER(_GROUP_USERS_INFO_0)
+LPGROUP_USERS_INFO_0 = POINTER(_GROUP_USERS_INFO_0)
+
+class _GROUP_USERS_INFO_1(Structure):
+    _fields_ = [
+        ("grui1_name", LPWSTR),
+        ("grui1_attributes", DWORD),
+    ]
+PGROUP_USERS_INFO_1 = POINTER(_GROUP_USERS_INFO_1)
+GROUP_USERS_INFO_1 = _GROUP_USERS_INFO_1
+LPGROUP_USERS_INFO_1 = POINTER(_GROUP_USERS_INFO_1)
+
 AclRevisionInformation = EnumValue("_ACL_INFORMATION_CLASS", "AclRevisionInformation", 0x1)
 AclSizeInformation = EnumValue("_ACL_INFORMATION_CLASS", "AclSizeInformation", 0x2)
 class _ACL_INFORMATION_CLASS(EnumType):
     values = [AclRevisionInformation, AclSizeInformation]
     mapper = FlagMapper(*values)
 ACL_INFORMATION_CLASS = _ACL_INFORMATION_CLASS
 
@@ -9384,14 +9882,29 @@
         ("Trustee", TRUSTEE_W),
     ]
 EXPLICIT_ACCESSW = _EXPLICIT_ACCESS_W
 PEXPLICIT_ACCESSW = POINTER(_EXPLICIT_ACCESS_W)
 PEXPLICIT_ACCESS_W = POINTER(_EXPLICIT_ACCESS_W)
 EXPLICIT_ACCESS_W = _EXPLICIT_ACCESS_W
 
+ComputerNameNetBIOS = EnumValue("_COMPUTER_NAME_FORMAT", "ComputerNameNetBIOS", 0x0)
+ComputerNameDnsHostname = EnumValue("_COMPUTER_NAME_FORMAT", "ComputerNameDnsHostname", 0x1)
+ComputerNameDnsDomain = EnumValue("_COMPUTER_NAME_FORMAT", "ComputerNameDnsDomain", 0x2)
+ComputerNameDnsFullyQualified = EnumValue("_COMPUTER_NAME_FORMAT", "ComputerNameDnsFullyQualified", 0x3)
+ComputerNamePhysicalNetBIOS = EnumValue("_COMPUTER_NAME_FORMAT", "ComputerNamePhysicalNetBIOS", 0x4)
+ComputerNamePhysicalDnsHostname = EnumValue("_COMPUTER_NAME_FORMAT", "ComputerNamePhysicalDnsHostname", 0x5)
+ComputerNamePhysicalDnsDomain = EnumValue("_COMPUTER_NAME_FORMAT", "ComputerNamePhysicalDnsDomain", 0x6)
+ComputerNamePhysicalDnsFullyQualified = EnumValue("_COMPUTER_NAME_FORMAT", "ComputerNamePhysicalDnsFullyQualified", 0x7)
+ComputerNameMax = EnumValue("_COMPUTER_NAME_FORMAT", "ComputerNameMax", 0x8)
+class _COMPUTER_NAME_FORMAT(EnumType):
+    values = [ComputerNameNetBIOS, ComputerNameDnsHostname, ComputerNameDnsDomain, ComputerNameDnsFullyQualified, ComputerNamePhysicalNetBIOS, ComputerNamePhysicalDnsHostname, ComputerNamePhysicalDnsDomain, ComputerNamePhysicalDnsFullyQualified, ComputerNameMax]
+    mapper = FlagMapper(*values)
+COMPUTER_NAME_FORMAT = _COMPUTER_NAME_FORMAT
+
+
 class _SYSTEM_PROCESS_INFORMATION(Structure):
     _fields_ = [
         ("NextEntryOffset", ULONG),
         ("NumberOfThreads", ULONG),
         ("Reserved1", BYTE * (24)),
         ("CreateTime", LARGE_INTEGER),
         ("UserTime", LARGE_INTEGER),
@@ -10758,7 +11271,169 @@
 WMI_REGINFO = EnumValue("WMIDPREQUESTCODE", "WMI_REGINFO", 0x8)
 WMI_EXECUTE_METHOD = EnumValue("WMIDPREQUESTCODE", "WMI_EXECUTE_METHOD", 0x9)
 class WMIDPREQUESTCODE(EnumType):
     values = [WMI_GET_ALL_DATA, WMI_GET_SINGLE_INSTANCE, WMI_SET_SINGLE_INSTANCE, WMI_SET_SINGLE_ITEM, WMI_ENABLE_EVENTS, WMI_DISABLE_EVENTS, WMI_ENABLE_COLLECTION, WMI_DISABLE_COLLECTION, WMI_REGINFO, WMI_EXECUTE_METHOD]
     mapper = FlagMapper(*values)
 
 
+class WSAData64(Structure):
+    _fields_ = [
+        ("wVersion", WORD),
+        ("wHighVersion", WORD),
+        ("iMaxSockets", USHORT),
+        ("iMaxUdpDg", USHORT),
+        ("lpVendorInfo", POINTER(CHAR)),
+        ("szDescription", CHAR * (WSADESCRIPTION_LEN + 1)),
+        ("szSystemStatus", CHAR * (WSASYS_STATUS_LEN + 1)),
+    ]
+WSADATA64 = WSAData64
+LPWSADATA64 = POINTER(WSAData64)
+
+class WSAData32(Structure):
+    _fields_ = [
+        ("wVersion", WORD),
+        ("wHighVersion", WORD),
+        ("szDescription", CHAR * (WSADESCRIPTION_LEN + 1)),
+        ("szSystemStatus", CHAR * (WSASYS_STATUS_LEN + 1)),
+        ("iMaxSockets", USHORT),
+        ("iMaxUdpDg", USHORT),
+        ("lpVendorInfo", POINTER(CHAR)),
+    ]
+LPWSADATA32 = POINTER(WSAData32)
+WSADATA32 = WSAData32
+
+class _ANON__ANON_IN_ADDR_SUB_UNION_1_SUB_STRUCTURE_1(Structure):
+    _fields_ = [
+        ("s_b1", UCHAR),
+        ("s_b2", UCHAR),
+        ("s_b3", UCHAR),
+        ("s_b4", UCHAR),
+    ]
+
+
+class _ANON__ANON_IN_ADDR_SUB_UNION_1_SUB_STRUCTURE_2(Structure):
+    _fields_ = [
+        ("s_w1", USHORT),
+        ("s_w2", USHORT),
+    ]
+
+class _ANON_IN_ADDR_SUB_UNION_1(Union):
+    _anonymous_ = ("S_un_b","S_un_w")
+    _fields_ = [
+        ("S_un_b", _ANON__ANON_IN_ADDR_SUB_UNION_1_SUB_STRUCTURE_1),
+        ("S_un_w", _ANON__ANON_IN_ADDR_SUB_UNION_1_SUB_STRUCTURE_2),
+        ("S_addr", ULONG),
+    ]
+
+class in_addr(Structure):
+    _anonymous_ = ("S_un",)
+    _fields_ = [
+        ("S_un", _ANON_IN_ADDR_SUB_UNION_1),
+    ]
+
+
+class sockaddr(Structure):
+    _fields_ = [
+        ("sa_family", USHORT),
+        ("sa_data", CHAR * (14)),
+    ]
+
+
+class sockaddr_in(Structure):
+    _fields_ = [
+        ("sin_family", SHORT),
+        ("sin_port", USHORT),
+        ("sin_addr", in_addr),
+        ("sin_zero", CHAR * (8)),
+    ]
+
+
+# Self referencing struct tricks
+class addrinfoW(Structure): pass
+ADDRINFOW = addrinfoW
+PADDRINFOW = POINTER(addrinfoW)
+addrinfoW._fields_ = [
+    ("ai_flags", INT),
+    ("ai_family", INT),
+    ("ai_socktype", INT),
+    ("ai_protocol", INT),
+    ("ai_addrlen", SIZE_T),
+    ("ai_canonname", PWSTR),
+    ("ai_addr", POINTER(sockaddr)),
+    ("ai_next", POINTER(addrinfoW)),
+]
+
+class _WSAPROTOCOLCHAIN(Structure):
+    _fields_ = [
+        ("ChainLen", INT),
+        ("ChainEntries", DWORD * (MAX_PROTOCOL_CHAIN)),
+    ]
+LPWSAPROTOCOLCHAIN = POINTER(_WSAPROTOCOLCHAIN)
+WSAPROTOCOLCHAIN = _WSAPROTOCOLCHAIN
+
+class _WSAPROTOCOL_INFOA(Structure):
+    _fields_ = [
+        ("dwServiceFlags1", DWORD),
+        ("dwServiceFlags2", DWORD),
+        ("dwServiceFlags3", DWORD),
+        ("dwServiceFlags4", DWORD),
+        ("dwProviderFlags", DWORD),
+        ("ProviderId", GUID),
+        ("dwCatalogEntryId", DWORD),
+        ("ProtocolChain", WSAPROTOCOLCHAIN),
+        ("iVersion", INT),
+        ("iAddressFamily", INT),
+        ("iMaxSockAddr", INT),
+        ("iMinSockAddr", INT),
+        ("iSocketType", INT),
+        ("iProtocol", INT),
+        ("iProtocolMaxOffset", INT),
+        ("iNetworkByteOrder", INT),
+        ("iSecurityScheme", INT),
+        ("dwMessageSize", DWORD),
+        ("dwProviderReserved", DWORD),
+        ("szProtocol", CHAR * (WSAPROTOCOL_LEN + 1)),
+    ]
+WSAPROTOCOL_INFOA = _WSAPROTOCOL_INFOA
+LPWSAPROTOCOL_INFOA = POINTER(_WSAPROTOCOL_INFOA)
+
+class _WSAPROTOCOL_INFOW(Structure):
+    _fields_ = [
+        ("dwServiceFlags1", DWORD),
+        ("dwServiceFlags2", DWORD),
+        ("dwServiceFlags3", DWORD),
+        ("dwServiceFlags4", DWORD),
+        ("dwProviderFlags", DWORD),
+        ("ProviderId", GUID),
+        ("dwCatalogEntryId", DWORD),
+        ("ProtocolChain", WSAPROTOCOLCHAIN),
+        ("iVersion", INT),
+        ("iAddressFamily", INT),
+        ("iMaxSockAddr", INT),
+        ("iMinSockAddr", INT),
+        ("iSocketType", INT),
+        ("iProtocol", INT),
+        ("iProtocolMaxOffset", INT),
+        ("iNetworkByteOrder", INT),
+        ("iSecurityScheme", INT),
+        ("dwMessageSize", DWORD),
+        ("dwProviderReserved", DWORD),
+        ("szProtocol", WCHAR * (WSAPROTOCOL_LEN + 1)),
+    ]
+LPWSAPROTOCOL_INFOW = POINTER(_WSAPROTOCOL_INFOW)
+WSAPROTOCOL_INFOW = _WSAPROTOCOL_INFOW
+
+# Self referencing struct tricks
+class addrinfo(Structure): pass
+PADDRINFOA = POINTER(addrinfo)
+ADDRINFOA = addrinfo
+addrinfo._fields_ = [
+    ("ai_flags", INT),
+    ("ai_family", INT),
+    ("ai_socktype", INT),
+    ("ai_protocol", INT),
+    ("ai_addrlen", SIZE_T),
+    ("ai_canonname", POINTER(CHAR)),
+    ("ai_addr", POINTER(sockaddr)),
+    ("ai_next", POINTER(addrinfo)),
+]
+
```

### Comparing `PythonForWindows-0.6.5/windows/generated_def/__init__.py` & `PythonForWindows-0.6.8/windows/generated_def/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from . import windef
 from . import winstructs
 
 def bitness():
     """Return 32 or 64"""
     import platform
     bits = platform.architecture()[0]
     return int(bits[:2])
@@ -23,14 +24,19 @@
 
     winstructs.PORT_MESSAGE = winstructs.PORT_MESSAGE32
     winstructs.PPORT_MESSAGE = winstructs.PPORT_MESSAGE32
 
     # CFGMGR32
     winstructs.IRQ_RESOURCE = winstructs.IRQ_RESOURCE_32
 
+    # Socket
+    windef.WSADATA = winstructs.WSADATA32
+    windef.INVALID_SOCKET = windef.INVALID_SOCKET32
+
+
 else:
     winstructs.CONTEXT = winstructs.CONTEXT64
     winstructs.PCONTEXT = winstructs.PCONTEXT64
     winstructs.LPCONTEXT = winstructs.LPCONTEXT64
 
     winstructs.EXCEPTION_POINTERS = winstructs.EXCEPTION_POINTERS64
     winstructs.PEXCEPTION_POINTERS = winstructs.PEXCEPTION_POINTERS64
@@ -43,14 +49,18 @@
 
     winstructs.PORT_MESSAGE = winstructs.PORT_MESSAGE64
     winstructs.PPORT_MESSAGE = winstructs.PPORT_MESSAGE64
 
     # CFGMGR32
     winstructs.IRQ_RESOURCE = winstructs.IRQ_RESOURCE_64
 
+    # Socket
+    windef.WSADATA = winstructs.WSADATA64
+    windef.INVALID_SOCKET = windef.INVALID_SOCKET64
+
 from . import winfuncs
 from . import windef
 from . import interfaces
 
 # Fuck it
 from .winstructs import *
 from .winfuncs import *
```

### Comparing `PythonForWindows-0.6.5/windows/hooks.py` & `PythonForWindows-0.6.8/windows/hooks.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/injection.py` & `PythonForWindows-0.6.8/windows/injection.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,16 +356,16 @@
     # Python 3 dll must be located using the registry
     for base_key in "HKEY_LOCAL_MACHINE", "HKEY_CURRENT_USER":
         # Open the registry in 64b view regardless of current process bitness
         regbase = windows.system.registry(base_key, gdef.KEY_WOW64_64KEY | gdef.KEY_READ)
         # we cannot use sys.winver as we are looking for the OTHER version
         # But from Python <PCbuild/python.props> it looks like format is
         # {Major}.{Minor}{-32}(for 32b build)
-        # This code do not handle -test version
-        winver_base = sys.winver[:3] # major-minor
+        # filter out anything after the -
+        winver_base = sys.winver.split("-")[0] # major-minor
         if target_bitness == 64:
             pyinstallkeys = [regbase(r"SOFTWARE\Python\PythonCore")(winver_base)]
         else:
             pyinstallkeys = [regbase(r"SOFTWARE\Python\PythonCore")(winver_base + "-32"),
                                 regbase(r"SOFTWARE\WOW6432Node\Python\PythonCore")(winver_base + "-32")]
         for pyinstallkey in pyinstallkeys:
             if not pyinstallkey.exists:
```

### Comparing `PythonForWindows-0.6.5/windows/native_exec/cpuid.py` & `PythonForWindows-0.6.8/windows/native_exec/cpuid.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/native_exec/nativeutils.py` & `PythonForWindows-0.6.8/windows/native_exec/nativeutils.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/native_exec/native_function.py` & `PythonForWindows-0.6.8/windows/native_exec/native_function.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/native_exec/simple_x64.py` & `PythonForWindows-0.6.8/windows/native_exec/simple_x64.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/native_exec/simple_x86.py` & `PythonForWindows-0.6.8/windows/native_exec/simple_x86.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/pe_parse.py` & `PythonForWindows-0.6.8/windows/pe_parse.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/pipe.py` & `PythonForWindows-0.6.8/windows/pipe.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/pycompat.py` & `PythonForWindows-0.6.8/windows/pycompat.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/remotectypes.py` & `PythonForWindows-0.6.8/windows/remotectypes.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/rpc/client.py` & `PythonForWindows-0.6.8/windows/rpc/client.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/rpc/epmapper.py` & `PythonForWindows-0.6.8/windows/rpc/epmapper.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/rpc/ndr.py` & `PythonForWindows-0.6.8/windows/rpc/ndr.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/security.py` & `PythonForWindows-0.6.8/windows/security.py`

 * *Files 4% similar despite different names*

```diff
@@ -281,14 +281,16 @@
 
 MANDATORY_LABEL_ACE_MASK = gdef.FlagMapper(
     gdef.SYSTEM_MANDATORY_LABEL_NO_WRITE_UP,
     gdef.SYSTEM_MANDATORY_LABEL_NO_READ_UP,
     gdef.SYSTEM_MANDATORY_LABEL_NO_EXECUTE_UP,
 )
 
+
+
 class AceHeader(gdef.ACE_HEADER):
     """Improved ACE_HEADER"""
     def _to_ace_type(self, ace_type):
         return ctypes.cast(ctypes.byref(self), ctypes.POINTER(ace_type))[0]
 
     @property
     def AceType(self):
@@ -711,14 +713,20 @@
         To query the SACL enable the ``SeSecurityPrivilege`` and use the parameter ``query_sacl=True`` on the functions expecting a ``flags``
 
         see :ref:`Query SACL sample <sample_security_sacl>`
     """
 
     _close_function = winproxy.LocalFree
 
+    @classmethod
+    def create(cls):
+        buff = windows.utils.BUFFER(gdef.SECURITY_DESCRIPTOR, 1)()
+        winproxy.InitializeSecurityDescriptor(buff, gdef.SECURITY_DESCRIPTOR_REVISION)
+        return buff.cast(windows.security.SecurityDescriptor)
+
     @property
     def control(self):
         """The security descriptor control
 
         :type: :class:`~windows.generated_def.winstructs.SECURITY_DESCRIPTOR_CONTROL`
         """
         lpdwRevision = gdef.DWORD()
@@ -733,26 +741,30 @@
         :type: :class:`int`
         """
         lpdwRevision = gdef.DWORD()
         control = gdef.SECURITY_DESCRIPTOR_CONTROL()
         winproxy.GetSecurityDescriptorControl(self, control, lpdwRevision)
         return lpdwRevision.value
 
-    @property
-    def owner(self):
+    def get_owner(self):
         """The owner of the security descriptor
 
         :type: :class:`~windows.generated_def.winstructs.PSID` or ``None``
         """
         owner = gdef.PSID()
         lpbOwnerDefaulted = gdef.BOOL()
         winproxy.GetSecurityDescriptorOwner(self, owner, lpbOwnerDefaulted)
         # Return None of owner is NULL
         return owner or None
 
+    def set_owner(self, new_owner):
+        winproxy.SetSecurityDescriptorOwner(self, new_owner, bOwnerDefaulted=False)
+
+    owner = property(get_owner, set_owner)
+
     @property
     def group(self):
         """The group of the security descriptor
 
         :type: :class:`~windows.generated_def.winstructs.PSID` or ``None``
         """
         group = gdef.PSID()
@@ -816,15 +828,15 @@
     @classmethod
     def _from_name_and_type(cls, objname, objtype, flags=DEFAULT_SECURITY_INFORMATION, query_sacl=False):
         self = cls()
 
         if query_sacl:
             flags |= gdef.SACL_SECURITY_INFORMATION
 
-        winproxy.GetNamedSecurityInfoA(
+        winproxy.GetNamedSecurityInfoW(
             objname,
             objtype,
             flags,
             None,
             None,
             None,
             None,
@@ -939,29 +951,89 @@
             None)
         result = result_cstr.value # Retrieve a python-str copy
         winproxy.LocalFree(result_cstr)
         return result.decode()
 
     __str__ = to_string
 
+    def isrelative(self):
+        """[WIP] api may change"""
+        return bool(self.control & gdef.SE_SELF_RELATIVE)
+
+    def make_absolute(self):
+        """[WIP] api may change"""
+        # Assert relative ?
+        abs_descriptor_size = gdef.DWORD(0)
+        dacl_size =  gdef.DWORD(0)
+        sacl_size =  gdef.DWORD(0)
+        owner_size =  gdef.DWORD(0)
+        prim_groupe_size =  gdef.DWORD(0)
+
+        try:
+            windows.winproxy.MakeAbsoluteSD(self, None, abs_descriptor_size,
+                    None,
+                    dacl_size,
+                    None,
+                    sacl_size,
+                    None,
+                    owner_size,
+                    None,
+                    prim_groupe_size)
+        except WindowsError as e:
+            if e.winerror != gdef.ERROR_INSUFFICIENT_BUFFER:
+                raise
+
+        abs_sd = windows.utils.BUFFER(gdef.BYTE, abs_descriptor_size.value)().cast(SecurityDescriptor)
+        # dacl = ctypes.create_string_buffer(dacl_size.value)
+        dacl = windows.utils.BUFFER(gdef.BYTE, dacl_size.value)()
+        sacl = windows.utils.BUFFER(gdef.BYTE, sacl_size.value)()
+        owner = ctypes.create_string_buffer(owner_size.value)
+        prim_groupe = ctypes.create_string_buffer(prim_groupe_size.value)
+
+        windows.winproxy.MakeAbsoluteSD(self, abs_sd, abs_descriptor_size,
+                dacl.cast(gdef.PACL),
+                dacl_size,
+                sacl.cast(gdef.PACL),
+                sacl_size,
+                owner,
+                owner_size,
+                prim_groupe,
+                prim_groupe_size)
+
+        abs_sd._save = [dacl, sacl, owner, prim_groupe]
+        return abs_sd
+
+    def make_relative(self):
+        """[WIP] api may change"""
+        srsd_size =  gdef.DWORD(0)
+        try:
+            windows.winproxy.MakeSelfRelativeSD(self, None, srsd_size)
+        except WindowsError as e:
+            if e.winerror != gdef.ERROR_INSUFFICIENT_BUFFER:
+                raise
 
-    # TST
+        srsd = windows.utils.BUFFER(gdef.BYTE, srsd_size.value)().cast(SecurityDescriptor)
+        windows.winproxy.MakeSelfRelativeSD(self, srsd, srsd_size)
+        return srsd
 
-    # def relative(self):
-        # return bool(self.control & gdef.SE_SELF_RELATIVE)
 
     # If we want auto-free we need to handle relf-relative SD
     # We need to keep-track of sub-object of the SD
     # Just a ref to SD from SACL / DACL ?
 
     # def __del__(self):
         # if self._needs_free and sys.path is not None:
             # print("FREE SELF")
             # self._close_function(self)
 
+    def __repr__(self):
+        if (self.isrelative()):
+            return "<{0} (self relative format) at {1:#x}>".format(type(self).__name__, id(self))
+        return "<{0} (absolute format) at {1:#x}>".format(type(self).__name__, id(self))
+
     def explain(self, type=None):
         if type is  None:
             type = getattr(self, "obj_type", None)
         return explain_sd(self, sdtype=type)
 
 # Explain SD POC
 # If ok -> new file
@@ -1039,32 +1111,55 @@
     yield u"HeaderFlags:"
     yield u"  {0:#x}".format(ace.Header.AceFlags)
     yield u"SID:"
     yield u"  " + explain_sid(ace.sid)
     yield u"Mask:"
     mapper = windows.security.SPECIFIC_ACCESS_RIGTH_BY_TYPE[sdtype]
     yield u"  " + str(list(mapper[x] for x in ace.mask))
-    yield "Application data:"
-    yield "  " + repr(ace.application_data.replace("\x00", ""))
+    yield u"Application data:"
+    yield u"  " + repr(ace.application_data.replace(b"\x00", b""))
     try:
         condition = ace.condition
-        yield "Condition:"
-        yield "  " + condition
+        yield u"Condition:"
+        yield u"  " + condition
     except ValueError:
         pass
 
+def explain_resource_attribute(ace, sdtype):
+    yield u"Type:"
+    yield u"  " + str(ace.Header.AceType)
+    yield u"HeaderFlags:"
+    yield u"  {0:#x}".format(ace.Header.AceFlags)
+    yield u"SID:"
+    yield u"  " + explain_sid(ace.sid)
+    yield u"Mask:"
+    mapper = windows.security.SPECIFIC_ACCESS_RIGTH_BY_TYPE[sdtype]
+    yield u"  " + str(list(mapper[x] for x in ace.mask))
+
+    attribute = ace.attribute
+    yield u"Attribute Name:"
+    yield u"  " + attribute.name
+    yield u"Attribute Type:"
+    yield u"  {0:#x}".format(attribute.ValueType)
+    yield u"Attribute Flags:"
+    yield u"  {0:#x}".format(attribute.Flags)
+    yield u"Values:"
+    for value in attribute.values:
+        yield u"  " + repr(value)
+
 
 ACE_EXPLAINER = {
     gdef.ACCESS_ALLOWED_ACE_TYPE: explain_simple_ace,
     gdef.ACCESS_DENIED_ACE_TYPE: explain_simple_ace,
     gdef.SYSTEM_MANDATORY_LABEL_ACE_TYPE: explain_mandatory_label_ace,
     gdef.SYSTEM_AUDIT_ACE_TYPE: explain_simple_ace,
     gdef.ACCESS_ALLOWED_OBJECT_ACE_TYPE: explain_object_related_ace,
     gdef.ACCESS_DENIED_OBJECT_ACE_TYPE: explain_object_related_ace,
     gdef.ACCESS_ALLOWED_CALLBACK_ACE_TYPE: explain_callback_ace,
+    gdef.SYSTEM_RESOURCE_ATTRIBUTE_ACE_TYPE: explain_resource_attribute,
 }
 
 
 def explain_acl(acl, sdtype=None):
     if acl is None:
         yield u"None"
     for ace in acl.aces:
```

### Comparing `PythonForWindows-0.6.5/windows/syswow64.py` & `PythonForWindows-0.6.8/windows/syswow64.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/test.py` & `PythonForWindows-0.6.8/windows/test.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/utils/improved_buffer.py` & `PythonForWindows-0.6.8/windows/utils/improved_buffer.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/utils/pythonutils.py` & `PythonForWindows-0.6.8/windows/utils/pythonutils.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/utils/winutils.py` & `PythonForWindows-0.6.8/windows/utils/winutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,33 +153,14 @@
     computernamesize = gdef.DWORD(0x1000)
     username = ctypes.create_unicode_buffer(usernamesize.value)
     computername = ctypes.create_unicode_buffer(computernamesize.value)
     peUse = gdef.SID_NAME_USE()
     winproxy.LookupAccountSidW(None, psid, username, usernamesize, computername, computernamesize, peUse)
     return computername[:computernamesize.value], username[:usernamesize.value]
 
-
-def lookup_name(computer, user):
-    sid_size = gdef.DWORD()
-    domain_size = gdef.DWORD(0)
-    stype = gdef.SID_NAME_USE()
-
-    try:
-        windows.winproxy.LookupAccountNameW(computer, user, None, sid_size, None, domain_size, stype)
-    except WindowsError as e:
-        pass
-
-    domain = ctypes.create_unicode_buffer(domain_size.value)
-    sid = ctypes.c_buffer(sid_size.value)
-    windows.winproxy.LookupAccountNameW(computer, user, sid, sid_size, domain, domain_size, stype)
-
-    psid = PSID.from_buffer_copy(ctypes.pointer(sid))
-    return domain[:domain_size.value], psid, stype.value
-
-
 def enable_privilege(lpszPrivilege, bEnablePrivilege):
     """
     Enable or disable a privilege::
 
         enable_privilege(SE_DEBUG_NAME, True)
     """
     tp = TOKEN_PRIVILEGES()
@@ -283,14 +264,25 @@
         # other words, the whole-number part of the date value may be positive or negative, while the fractional part of the date value is always added to the overall logical date.
         # WTF :D
         dec, nb = math.modf(comtime)
         final_delta = nb + abs(dec)
         return COMDATE_EPOCH + datetime.timedelta(final_delta)
     return COMDATE_EPOCH + datetime.timedelta(comtime)
 
+def datetime_from_systemtime(systime):
+    return datetime.datetime(
+            year=systime.wYear,
+            month=systime.wMonth,
+            day=systime.wDay,
+            hour=systime.wHour,
+            minute=systime.wMinute,
+            second=systime.wSecond,
+            microsecond=systime.wMilliseconds * 1000,
+    )
+
 class FixedInteractiveConsole(code.InteractiveConsole):
     def raw_input(self, prompt=">>>"):
         sys.stdout.write(prompt)
         return raw_input("")
 
 
 def pop_shell(locs=None):
```

### Comparing `PythonForWindows-0.6.5/windows/winobject/apisetmap.py` & `PythonForWindows-0.6.8/windows/winobject/apisetmap.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/bits.py` & `PythonForWindows-0.6.8/windows/winobject/bits.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/device_manager.py` & `PythonForWindows-0.6.8/windows/winobject/device_manager.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/event_log.py` & `PythonForWindows-0.6.8/windows/winobject/event_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,26 +62,27 @@
         if not bool(self):
             return
         self._close_function()
 
 # Class high-level API
 class EvtQuery(EvtHandle):
     """Represent an Event-log query"""
-    TIMEOUT = 0x1000
+    DEFAULT_TIMEOUT = 0x1000
 
-    def __init__(self, handle=0, channel=None):
+    def __init__(self, handle=0, channel=None, timeout=None):
         super(EvtQuery, self).__init__(handle)
         self.channel = channel
+        self.timeout = timeout if timeout is not None else self.DEFAULT_TIMEOUT
 
     def __next__(self):
         """Return the next :class:`EvtEvent` matching the query"""
         try:
             event = EvtEvent(channel=self.channel)
             ret = gdef.DWORD()
-            windows.winproxy.EvtNext(self, 1, event, self.TIMEOUT, 0, ret)
+            windows.winproxy.EvtNext(self, 1, event, self.timeout, 0, ret)
         except WindowsError as e:
             if e.winerror == gdef.ERROR_NO_MORE_ITEMS:
                 raise StopIteration
             raise
         assert ret.value == 1
         return event
 
@@ -433,15 +434,15 @@
     DEFAULT_QUERY_FLAGS = gdef.EvtQueryChannelPath + gdef.EvtQueryForwardDirection
 
     def __init__(self, name):
         self.name = name
         self.event_metadata_by_id = {}
         self.classic_event_metadata_by_id = {} # For classic only
 
-    def query(self, filter=None, ids=None):
+    def query(self, filter=None, ids=None, timeout=None):
         """Query the event with the ``ids`` or perform a query with the raw query ``filter``
 
         Both parameters are mutually exclusive.
 
         .. note:: Here are some query examples
 
             List all events with a event data attribute named 'RuleName':
@@ -462,15 +463,15 @@
             raise ValueError("<ids> and <filter> are mutually exclusive")
         if ids is not None:
             if isinstance(ids, int_types):
                 ids = (ids,)
             ids_filter = " or ".join("EventID={0}".format(id) for id in ids)
             filter = "Event/System[{0}]".format(ids_filter)
         query_handle = winproxy.EvtQuery(None, self.name, filter, self.DEFAULT_QUERY_FLAGS)
-        return EvtQuery(query_handle, self)
+        return EvtQuery(query_handle, self, timeout=timeout)
 
     @property
     def events(self):
         """The list of all events in the channels, an alias for ``channel.query().all()``
 
         :type: [:class:`EvtEvent`] -- A list of :class:`EvtEvent`
         """
```

### Comparing `PythonForWindows-0.6.5/windows/winobject/event_trace.py` & `PythonForWindows-0.6.8/windows/winobject/event_trace.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/exception.py` & `PythonForWindows-0.6.8/windows/winobject/exception.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/file.py` & `PythonForWindows-0.6.8/windows/winobject/file.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/handle.py` & `PythonForWindows-0.6.8/windows/winobject/handle.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from windows import winproxy
 from windows.generated_def import windef
 import windows.generated_def as gdef
 
 current_process_pid = os.getpid()
 
 class BaseSystemHandle(object):
+    # Big bypass to prevent missing reference at programm exit..
+    _close_function = ctypes.WinDLL("kernel32").CloseHandle
+
     """A handle of the system"""
     @windows.utils.fixedpropety
     def process(self):
         """The process possessing the handle
 
         :type: :class:`WinProcess <windows.winobject.process.WinProcess>`"""
         # "TODO: something smart ? :D"
@@ -110,15 +113,15 @@
     def __repr__(self):
         return "<{0} value=<0x{1:x}> in process pid={2}>".format(type(self).__name__, self.wValue, self.dwProcessId)
 
     def __del__(self):
         if self.dwProcessId == current_process_pid:
             return
         if hasattr(self, "_local_handle"):
-            return winproxy.CloseHandle(self._local_handle)
+            return self._close_function(self._local_handle)
 
 class Handle(gdef.SYSTEM_HANDLE, BaseSystemHandle):
     pass
 
 class HandleWow64(gdef.SYSTEM_HANDLE64, BaseSystemHandle):
     pass # For wow64 process
```

### Comparing `PythonForWindows-0.6.5/windows/winobject/network.py` & `PythonForWindows-0.6.8/windows/winobject/network.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/object_manager.py` & `PythonForWindows-0.6.8/windows/winobject/object_manager.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/process.py` & `PythonForWindows-0.6.8/windows/winobject/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -861,36 +861,65 @@
         if res_size == 32:
             res = ULONG()
         else:
             res = ULONGLONG()
         winproxy.NtQueryInformationThread(self.handle, ThreadQuerySetWin32StartAddress, byref(res), ctypes.sizeof(res))
         return res.value
 
-    @property
-    def teb_base(self):
-        """The address of the thread's TEB
-
-            :type: :class:`int`
-		"""
-        if windows.current_process.bitness == 32 and self.owner.bitness == 64:
+    def _get_principal_teb_addr(self):
+        # Returns the 64bits TEB on a 64bits computer (syswow process or not)
+        # Returns the 32bits TEB on a 32bits computer
+
+        # If we are wow64 process its means we either
+        # - Want the TEB of a 64b process
+        # - Want the TEB64 of a Wowprocess
+        # It's the same code for both
+        if windows.current_process.is_wow_64:
             restype = rctypes.transform_type_to_remote64bits(THREAD_BASIC_INFORMATION)
             ressize = (ctypes.sizeof(restype))
             # Manual aligned allocation :DDDD
-            nb_qword = (ressize + 8) / ctypes.sizeof(ULONGLONG)
+            nb_qword = int((ressize + 8) / ctypes.sizeof(ULONGLONG))
             buffer = (nb_qword * ULONGLONG)()
             struct_address = ctypes.addressof(buffer)
             if (struct_address & 0xf) not in [0, 8]:
                 raise ValueError("ULONGLONG array not aligned on 8")
             windows.syswow64.NtQueryInformationThread_32_to_64(self.handle, ThreadBasicInformation, struct_address, ressize)
             return restype(struct_address, windows.current_process).TebBaseAddress
 
         res = THREAD_BASIC_INFORMATION()
         windows.winproxy.NtQueryInformationThread(self.handle, ThreadBasicInformation, byref(res), ctypes.sizeof(res))
         return res.TebBaseAddress
 
+    @property
+    def teb_base(self):
+        """The address of the thread's TEB. If the owner is a SysWow64 process, return the TEB32.
+
+            :type: :class:`int`
+		"""
+        main_teb_addr = self._get_principal_teb_addr()
+        if not self.owner.is_wow_64:
+            return main_teb_addr
+        # TEB32 is pointed at the begining of the TEB64
+        # TebBase->NtTib.ExceptionList = (PVOID)Teb32Base;
+        return self.owner.read_dword(main_teb_addr)
+
+
+
+    @property
+    def teb_syswow_base(self):
+        """The address of the thread's TEB64 for a SysWow64 process
+
+        :type: :class:`int`
+		"""
+        if not self.owner.is_wow_64:
+            raise ValueError("Not a syswow process")
+        # just return the main TEB
+        return self._get_principal_teb_addr()
+
+
     def exit(self, code=0):
         """Exit the thread"""
         return winproxy.TerminateThread(self.handle, code)
 
     def resume(self):
         """Resume the thread"""
         return winproxy.ResumeThread(self.handle)
@@ -969,16 +998,16 @@
         #proc = [p for p in windows.system.processes if p.pid == pid][0]
         #proc._handle = handle
         #dbgprint("Process {0} from handle {1}".format(proc, hex(handle)), "HANDLE")
         return WinProcess(handle=handle)
 
     @classmethod
     def _from_PROCESSENTRY32(cls, entry):
-        #print("_from_PROCESSENTRY32")
-        name = entry.szExeFile.decode()
+        # Temporary encoded name
+        name = entry.szExeFile.encode(errors="backslashreplace")
         pid = entry.th32ProcessID
         ppid = entry.th32ParentProcessID
         return cls(pid=pid, name=name, ppid=ppid)
 
 
     @utils.fixedpropety
     def name(self):
@@ -1111,14 +1140,17 @@
     def execute_python_unsafe(self, pycode):
         """Execute Python code into the remote process.
 
         :rtype: :rtype: :class:`WinThread` or :class:`DeadThread` : The thread executing the python code
         """
         return injection.execute_python_code(self, pycode)
 
+
+
+
     @utils.fixedpropety
     def peb_addr(self):
         """The address of the PEB
 
             :type: :class:`int`
 		"""
         if windows.current_process.bitness == 32 and self.bitness == 64:
```

### Comparing `PythonForWindows-0.6.5/windows/winobject/registry.py` & `PythonForWindows-0.6.8/windows/winobject/registry.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/service.py` & `PythonForWindows-0.6.8/windows/winobject/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 
 """
 
 
 class ServiceManager(utils.AutoHandle):
     """An object to query, list and explore services"""
     def _get_handle(self):
-        return windows.winproxy.OpenSCManagerA(dwDesiredAccess=gdef.MAXIMUM_ALLOWED)
+        return windows.winproxy.OpenSCManagerW(dwDesiredAccess=gdef.MAXIMUM_ALLOWED)
 
     def open_service(self, name, access=gdef.MAXIMUM_ALLOWED):
-        return windows.winproxy.OpenServiceA(self.handle, name, access) # Check service exists :)
+        return windows.winproxy.OpenServiceW(self.handle, name, access) # Check service exists :)
 
     def get_service(self, key, access=gdef.MAXIMUM_ALLOWED):
         """Get a service by its name/index or a list of services via a slice
 
         :return: :class:`Service` or [:class:`Service`] -- A :class:`Service` or list of :class:`Service`
         """
         if isinstance(key, int_types):
@@ -69,40 +69,40 @@
     :return: :class:`Service` or [:class:`Service`] -- A :class:`Service` or list of :class:`Service`
     """
 
     def get_service_display_name(self, name):
         # This API is strange..
         # Why can't we retrieve the display name for a service handle ?
         BUFFER_SIZE = 0x1000
-        result = (CHAR * BUFFER_SIZE)()
+        result = (WCHAR * BUFFER_SIZE)()
         size_needed = gdef.DWORD(BUFFER_SIZE)
-        windows.winproxy.GetServiceDisplayNameA(self.handle, name, result, size_needed)
+        windows.winproxy.GetServiceDisplayNameW(self.handle, name, result, size_needed)
         return result.value
 
     def _enumerate_services_generator(self):
         """The generator code behind __iter__.
         Allow to iter over the services on the system
         """
         size_needed = gdef.DWORD()
         nb_services =  gdef.DWORD()
         counter =  gdef.DWORD()
         try:
-            windows.winproxy.EnumServicesStatusExA(self.handle, SC_ENUM_PROCESS_INFO, SERVICE_TYPE_ALL, SERVICE_STATE_ALL, None, 0, ctypes.byref(size_needed), ctypes.byref(nb_services), byref(counter), None)
+            windows.winproxy.EnumServicesStatusExW(self.handle, SC_ENUM_PROCESS_INFO, SERVICE_TYPE_ALL, SERVICE_STATE_ALL, None, 0, ctypes.byref(size_needed), ctypes.byref(nb_services), byref(counter), None)
         except WindowsError:
             pass
 
         while True:
             size = size_needed.value
             buffer = (BYTE * size)()
             try:
-                windows.winproxy.EnumServicesStatusExA(self.handle, SC_ENUM_PROCESS_INFO, SERVICE_TYPE_ALL, SERVICE_STATE_ALL, buffer, size, ctypes.byref(size_needed), ctypes.byref(nb_services), byref(counter), None)
+                windows.winproxy.EnumServicesStatusExW(self.handle, SC_ENUM_PROCESS_INFO, SERVICE_TYPE_ALL, SERVICE_STATE_ALL, buffer, size, ctypes.byref(size_needed), ctypes.byref(nb_services), byref(counter), None)
             except WindowsError as e:
                 continue
             break
-        services_array = (gdef.ENUM_SERVICE_STATUS_PROCESSA * nb_services.value).from_buffer(buffer)
+        services_array = (gdef.ENUM_SERVICE_STATUS_PROCESSW * nb_services.value).from_buffer(buffer)
         for service_info in services_array:
             shandle = self.open_service(service_info.lpServiceName)
             yield Service(handle=shandle, name=service_info.lpServiceName, description=service_info.lpDisplayName)
         return
 
     __iter__ = _enumerate_services_generator
     """Iter over the services on the system
@@ -171,16 +171,16 @@
         :param args: a list of :class:`str`
         """
         nbelt = 0
         if args is not None:
             if isinstance(args, windows.pycompat.anybuff):
                 args = [args]
             nbelt = len(args)
-            args = (gdef.LPCSTR * (nbelt))(*args)
-        return windows.winproxy.StartServiceA(self, nbelt, args)
+            args = (gdef.LPWSTR * (nbelt))(*args)
+        return windows.winproxy.StartServiceW(self, nbelt, args)
 
     def stop(self):
         """Stop the service"""
         status = SERVICE_STATUS()
         windows.winproxy.ControlService(self, gdef.SERVICE_CONTROL_STOP, status)
         return status
```

### Comparing `PythonForWindows-0.6.5/windows/winobject/system.py` & `PythonForWindows-0.6.8/windows/winobject/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,45 @@
 from windows.winobject import event_trace
 from windows.winobject import task_scheduler
 from windows.winobject import system_module
 from windows.winobject import bits
 
 from windows.dbgprint import dbgprint
 
+
+class UnicodeEnvironment(dict):
+    def __getitem__(self, key):
+        key = key.upper()
+        return super(UnicodeEnvironment, self).__getitem__(key)
+
+    def __delitem__(self, key):
+        key = key.upper()
+        windows.winproxy.SetEnvironmentVariableW(key, None)
+        return super(UnicodeEnvironment, self).__delitem__(key)
+
+    def __contains__(self, key):
+        key = key.upper()
+        return super(UnicodeEnvironment, self).__contains__(key)
+
+    def __setitem__(self, key, value):
+        if value is None:
+            # SetEnvironmentVariableW
+            # If this parameter is NULL, the variable is deleted from the current process's environment.
+            del self[key]
+            return
+        key = key.upper()
+        windows.winproxy.SetEnvironmentVariableW(key, value)
+        return super(UnicodeEnvironment, self).__setitem__(key, value)
+
+    def update(self, *args, **kwargs):
+        for k, v in dict(*args, **kwargs).items():
+            self[k.upper()] = v
+
+    # Setitem -> SetEnvironmement variable
+
 class System(object):
     """The state of the current ``Windows`` system ``Python`` is running on"""
 
     # Setup these in a fixedproperty ?
     network = network.Network()
     """Object of class :class:`windows.winobject.network.Network`"""
     registry = registry.Registry()
@@ -94,14 +125,43 @@
         if os.environ["PROCESSOR_ARCHITECTURE"].lower() != "x86":
             return 64
         if "PROCESSOR_ARCHITEW6432" in os.environ:
             return 64
         return 32
 
     @utils.fixedpropety
+    def environ(self):
+        """A unicode version of os.environ
+        Same as os.environ on py3
+        Custom dict built on GetEnvironmentStringsW() on py2
+
+        :type: :class:`dict` -- {unicode: unicode}
+		"""
+        if windows.pycompat.is_py3:
+            return os.environ # Py3 environ is already unicode
+        # Create a unicode wrapper environment
+        return self._create_unicode_environ_dict()
+
+    def _create_unicode_environ_dict(self):
+        rawdictenv = {}
+        curenv = envptr = windows.winproxy.GetEnvironmentStringsW()
+        while True:
+            envstr = ctypes.c_wchar_p(curenv).value
+            if not envstr:
+                break
+            try:
+                key, value = envstr.split("=", 1)
+            except ValueError as e: # No =
+                pass
+            rawdictenv[key.upper()] = value
+            curenv += (len(envstr) + 1) * 2
+        windows.winproxy.FreeEnvironmentStringsW(envptr)
+        return UnicodeEnvironment(rawdictenv)
+
+    @utils.fixedpropety
     def wmi(self):
         r"""An object to perform wmi requests to various namespaces
 
         :type: :class:`~windows.winobject.wmi.WmiManager`"""
         return wmi.WmiManager()
 
 
@@ -170,14 +230,31 @@
             buf = ctypes.create_unicode_buffer(size.value)
             winproxy.GetComputerNameW(buf, ctypes.byref(size))
         else:
             buf = ctypes.create_string_buffer(size.value)
             winproxy.GetComputerNameA(buf, ctypes.byref(size))
         return buf[:size.value]
 
+    def _computer_name_ex(self, nametype):
+        size = gdef.DWORD(0)
+        try:
+            winproxy.GetComputerNameExW(nametype, None, ctypes.byref(size))
+        except WindowsError as e:
+            if e.winerror != gdef.ERROR_MORE_DATA:
+                raise
+
+        buf = ctypes.create_unicode_buffer(size.value)
+        winproxy.GetComputerNameExW(nametype, buf, ctypes.byref(size))
+        return buf[:size.value]
+
+    @utils.fixedproperty
+    def domain(self):
+        # [WIP] name of the domain joined by the computer, None is no domain joined
+        return self._computer_name_ex(gdef.ComputerNameDnsDomain) or None
+
     @utils.fixedpropety
     def version(self):
         """The version of the system
 
         :type: (:class:`int`, :class:`int`) -- (Major, Minor)
         """
         data = self.get_version()
@@ -419,21 +496,21 @@
         except (WindowsError, ValueError):
             return self.get_file_version("ntdll")
 
 
     @staticmethod
     def enumerate_processes():
         dbgprint("Enumerating processes with CreateToolhelp32Snapshot", "SLOW")
-        process_entry = gdef.PROCESSENTRY32()
+        process_entry = gdef.PROCESSENTRY32W()
         process_entry.dwSize = ctypes.sizeof(process_entry)
         snap = winproxy.CreateToolhelp32Snapshot(gdef.TH32CS_SNAPPROCESS, 0)
-        winproxy.Process32First(snap, process_entry)
+        winproxy.Process32FirstW(snap, process_entry)
         res = []
         res.append(process.WinProcess._from_PROCESSENTRY32(process_entry))
-        while winproxy.Process32Next(snap, process_entry):
+        while winproxy.Process32NextW(snap, process_entry):
             res.append(process.WinProcess._from_PROCESSENTRY32(process_entry))
         winproxy.CloseHandle(snap)
         return res
 
     @staticmethod
     def enumerate_threads_generator():
         # Ptet dangereux, parce que on yield la meme THREADENTRY32 a chaque fois
@@ -463,20 +540,20 @@
         # (as we need to get a handle on the process)
         # So, this implementation of enumerate_thread also setup the owner with the result of enumerate_processes
         dbgprint("Enumerating threads with CreateToolhelp32Snapshot and setup owner", "SLOW")
 
         # One snap for both enum to be prevent race
         snap = winproxy.CreateToolhelp32Snapshot(gdef.TH32CS_SNAPTHREAD | gdef.TH32CS_SNAPPROCESS, 0)
 
-        process_entry = gdef.PROCESSENTRY32()
+        process_entry = gdef.PROCESSENTRY32W()
         process_entry.dwSize = ctypes.sizeof(process_entry)
-        winproxy.Process32First(snap, process_entry)
+        winproxy.Process32FirstW(snap, process_entry)
         processes = []
         processes.append(process.WinProcess._from_PROCESSENTRY32(process_entry))
-        while winproxy.Process32Next(snap, process_entry):
+        while winproxy.Process32NextW(snap, process_entry):
             processes.append(process.WinProcess._from_PROCESSENTRY32(process_entry))
 
         # Forge a dict pid -> process
         proc_dict = {proc.pid: proc for proc in processes}
 
         thread_entry = gdef.THREADENTRY32()
         thread_entry.dwSize = ctypes.sizeof(thread_entry)
```

### Comparing `PythonForWindows-0.6.5/windows/winobject/system_module.py` & `PythonForWindows-0.6.8/windows/winobject/system_module.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/task_scheduler.py` & `PythonForWindows-0.6.8/windows/winobject/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/token.py` & `PythonForWindows-0.6.8/windows/winobject/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,21 +110,21 @@
             raise KeyError(name)
         priv.Attributes = value
 
     # __delitem__ that set SE_PRIVILEGE_REMOVED ?
 
     def _lookup_name(self, luid):
         size = gdef.DWORD(0x100)
-        buff = ctypes.c_buffer(size.value)
-        winproxy.LookupPrivilegeNameA(None, luid, buff, size)
+        buff = ctypes.create_unicode_buffer(size.value)
+        winproxy.LookupPrivilegeNameW(None, luid, buff, size)
         return buff[:size.value]
 
     def _lookup_value(self, name):
         luid = gdef.LUID()
-        winproxy.LookupPrivilegeValueA(None, name, ctypes.byref(luid))
+        winproxy.LookupPrivilegeValueW(None, name, ctypes.byref(luid))
         return luid
 
 
 
 TokenPrivilegesType = TokenPrivileges
 
 class TokenSecurityAttributesInformation(gdef.TOKEN_SECURITY_ATTRIBUTES_INFORMATION):
@@ -609,15 +609,18 @@
         except KeyError as e:
             # Emulate the WindowsError that would be triggered in 'adjust_privileges' ?
             raise ValueError("{0} has no privilege <{1}>".format(self, name))
         return self.adjust_privileges(privs)
 
     def __repr__(self):
         flag_repr = gdef.Flag.__repr__
-        tid_int = int(self.TokenStatistics.TokenId)
+        try:
+            tid_int = int(self.TokenStatistics.TokenId) # May raise -> which is bad as __repr__ may be called on __del__...
+        except WindowsError as e:
+            return object.__repr__(self)
         toktype = self.type
         if toktype == gdef.TokenPrimary:
             return "<{0} TokenId={1:#x} Type={2}>".format(type(self).__name__, tid_int, flag_repr(toktype))
         return "<{0} TokenId={1:#x} Type={2} ImpersonationLevel={3}>".format(type(self).__name__, tid_int, flag_repr(toktype), flag_repr(self.impersonation_level))
 
 
 import windows.security
```

### Comparing `PythonForWindows-0.6.5/windows/winobject/volume.py` & `PythonForWindows-0.6.8/windows/winobject/volume.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winobject/wmi.py` & `PythonForWindows-0.6.8/windows/winobject/wmi.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,28 +76,14 @@
         if not isinstance(name, basestring):
             nametype = type(name).__name__
             raise TypeError("WmiObject attributes name must be str, not <{0}>".format(nametype))
         variant_res = windows.com.Variant()
         self.Get(name, 0, variant_res, None, None)
         return variant_res
 
-    def tst(self, name):
-        """Retrieve the value of property ``name`` as a :class:`~windows.com.Variant`
-
-        :return: :class:`~windows.com.Variant`
-        """
-        if not isinstance(name, basestring):
-            nametype = type(name).__name__
-            raise TypeError("WmiObject attributes name must be str, not <{0}>".format(nametype))
-        variant_res = windows.com.Variant()
-        cimtype = gdef.CIMTYPE()
-        self.Get(name, 0, variant_res, cimtype, None)
-        return variant_res, cimtype
-
-
     def get(self, name):
         """Return the value of the property ``name``. The return value depends of the type of the property and can vary"""
         return self.get_variant(name).value
 
     def get_method(self, name):
         """Return the information about the method ``name``
```

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apiproxy.py` & `PythonForWindows-0.6.8/windows/winproxy/apiproxy.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/advapi32.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/advapi32.py`

 * *Files 8% similar despite different names*

```diff
@@ -193,14 +193,18 @@
 
 @Advapi32Proxy(error_check=result_is_error_code)
 def SetNamedSecurityInfoW(pObjectName, ObjectType, SecurityInfo, psidOwner, psidGroup, pDacl, pSacl):
     return SetNamedSecurityInfoW.ctypes_function(pObjectName, ObjectType, SecurityInfo, psidOwner, psidGroup, pDacl, pSacl)
 
 
 @Advapi32Proxy()
+def InitializeSecurityDescriptor(pSecurityDescriptor, dwRevision):
+   return InitializeSecurityDescriptor.ctypes_function(pSecurityDescriptor, dwRevision)
+
+@Advapi32Proxy()
 def IsValidSecurityDescriptor(pSecurityDescriptor):
    return IsValidSecurityDescriptor.ctypes_function(pSecurityDescriptor)
 
 @Advapi32Proxy()
 def ConvertStringSecurityDescriptorToSecurityDescriptorA(StringSecurityDescriptor, StringSDRevision, SecurityDescriptor, SecurityDescriptorSize):
    return ConvertStringSecurityDescriptorToSecurityDescriptorA.ctypes_function(StringSecurityDescriptor, StringSDRevision, SecurityDescriptor, SecurityDescriptorSize)
 
@@ -229,21 +233,33 @@
    return GetSecurityDescriptorControl.ctypes_function(pSecurityDescriptor, pControl, lpdwRevision)
 
 @Advapi32Proxy()
 def GetSecurityDescriptorOwner(pSecurityDescriptor, pOwner, lpbOwnerDefaulted):
    return GetSecurityDescriptorOwner.ctypes_function(pSecurityDescriptor, pOwner, lpbOwnerDefaulted)
 
 @Advapi32Proxy()
+def SetSecurityDescriptorOwner(pSecurityDescriptor, pOwner, bOwnerDefaulted):
+   return SetSecurityDescriptorOwner.ctypes_function(pSecurityDescriptor, pOwner, bOwnerDefaulted)
+
+@Advapi32Proxy()
 def GetSecurityDescriptorGroup(pSecurityDescriptor, pGroup, lpbGroupDefaulted):
    return GetSecurityDescriptorGroup.ctypes_function(pSecurityDescriptor, pGroup, lpbGroupDefaulted)
 
 @Advapi32Proxy()
 def GetSecurityDescriptorSacl(pSecurityDescriptor, lpbSaclPresent, pSacl, lpbSaclDefaulted):
    return GetSecurityDescriptorSacl.ctypes_function(pSecurityDescriptor, lpbSaclPresent, pSacl, lpbSaclDefaulted)
 
+@Advapi32Proxy()
+def MakeAbsoluteSD(pSelfRelativeSecurityDescriptor, pAbsoluteSecurityDescriptor, lpdwAbsoluteSecurityDescriptorSize, pDacl, lpdwDaclSize, pSacl, lpdwSaclSize, pOwner, lpdwOwnerSize, pPrimaryGroup, lpdwPrimaryGroupSize):
+   return MakeAbsoluteSD.ctypes_function(pSelfRelativeSecurityDescriptor, pAbsoluteSecurityDescriptor, lpdwAbsoluteSecurityDescriptorSize, pDacl, lpdwDaclSize, pSacl, lpdwSaclSize, pOwner, lpdwOwnerSize, pPrimaryGroup, lpdwPrimaryGroupSize)
+
+@Advapi32Proxy()
+def MakeSelfRelativeSD(pAbsoluteSecurityDescriptor, pSelfRelativeSecurityDescriptor, lpdwBufferLength):
+   return MakeSelfRelativeSD.ctypes_function(pAbsoluteSecurityDescriptor, pSelfRelativeSecurityDescriptor, lpdwBufferLength)
+
 # ACE - ACL
 
 @Advapi32Proxy()
 def GetAclInformation(pAcl, pAclInformation, nAclInformationLength, dwAclInformationClass):
     return GetAclInformation.ctypes_function(pAcl, pAclInformation, nAclInformationLength, dwAclInformationClass)
 
 @Advapi32Proxy()
@@ -383,14 +399,30 @@
 def RegSaveKeyExA(hKey, lpFile, lpSecurityAttributes, Flags):
     return RegSaveKeyExA.ctypes_function(hKey, lpFile, lpSecurityAttributes, Flags)
 
 @Advapi32Proxy(error_check=result_is_error_code)
 def RegSaveKeyExW(hKey, lpFile, lpSecurityAttributes, Flags):
     return RegSaveKeyExW.ctypes_function(hKey, lpFile, lpSecurityAttributes, Flags)
 
+@Advapi32Proxy(error_check=result_is_error_code)
+def RegLoadKeyA(hKey, lpSubKey, lpFile):
+    return RegLoadKeyA.ctypes_function(hKey, lpSubKey, lpFile)
+
+@Advapi32Proxy(error_check=result_is_error_code)
+def RegLoadKeyW(hKey, lpSubKey, lpFile):
+    return RegLoadKeyW.ctypes_function(hKey, lpSubKey, lpFile)
+
+@Advapi32Proxy(error_check=result_is_error_code)
+def RegUnLoadKeyA(hKey, lpSubKey):
+    return RegUnLoadKeyA.ctypes_function(hKey, lpSubKey)
+
+@Advapi32Proxy(error_check=result_is_error_code)
+def RegUnLoadKeyW(hKey, lpSubKey):
+    return RegUnLoadKeyW.ctypes_function(hKey, lpSubKey)
+
 # Service
 
 @Advapi32Proxy()
 def OpenSCManagerA(lpMachineName=None, lpDatabaseName=None, dwDesiredAccess=gdef.SC_MANAGER_ALL_ACCESS):
     return OpenSCManagerA.ctypes_function(lpMachineName, lpDatabaseName, dwDesiredAccess)
 
 @Advapi32Proxy()
```

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/cfgmgr32.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/cfgmgr32.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/crypt32.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/crypt32.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/dbghelp.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/dbghelp.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/dnsapi.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/dnsapi.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,10 +19,14 @@
     return DnsQuery_A.ctypes_function(pszName, wType, Options, pExtra, ppQueryResults, pReserved)
 
 
 @DNSapiProxy(error_check=result_is_error_code)
 def DnsQuery_W(pszName, wType, Options, pExtra, ppQueryResults, pReserved):
     return DnsQuery_W.ctypes_function(pszName, wType, Options, pExtra, ppQueryResults, pReserved)
 
+@DNSapiProxy(error_check=result_is_error_code)
+def DnsQueryEx(pQueryRequest, pQueryResults, pCancelHandle):
+    return DnsQueryEx.ctypes_function(pQueryRequest, pQueryResults, pCancelHandle)
+
 @DNSapiProxy(error_check=no_error_check)
 def DnsFree(pData, FreeType):
     return DnsFree.ctypes_function(pData, FreeType)
```

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/iphlpapi.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/iphlpapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,8 +32,16 @@
 @IphlpapiProxy()
 def GetIpAddrTable(pIpAddrTable, pdwSize, bOrder=False):
     return GetIpAddrTable.ctypes_function(pIpAddrTable, pdwSize, bOrder)
 
 
 @IphlpapiProxy()
 def GetIpNetTable(IpNetTable, SizePointer, Order):
-   return GetIpNetTable.ctypes_function(IpNetTable, SizePointer, Order)
+   return GetIpNetTable.ctypes_function(IpNetTable, SizePointer, Order)
+
+@IphlpapiProxy()
+def GetAdaptersInfo(AdapterInfo, SizePointer):
+    return GetAdaptersInfo.ctypes_function(AdapterInfo, SizePointer)
+
+@IphlpapiProxy()
+def GetPerAdapterInfo(IfIndex, pPerAdapterInfo, pOutBufLen):
+    return GetPerAdapterInfo.ctypes_function(IfIndex, pPerAdapterInfo, pOutBufLen)
```

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/kernel32.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/kernel32.py`

 * *Files 12% similar despite different names*

```diff
@@ -331,14 +331,16 @@
 def GetVersionExA(lpVersionInformation):
     return GetVersionExA.ctypes_function(lpVersionInformation)
 
 @Kernel32Proxy()
 def GetVersionExW(lpVersionInformation):
     return GetVersionExW.ctypes_function(lpVersionInformation)
 
+
+
 ## Hardware
 
 @Kernel32Proxy()
 def GetCurrentProcessorNumber():
     return GetCurrentProcessorNumber.ctypes_function()
 
 ## Console
@@ -370,14 +372,22 @@
     return GetComputerNameA.ctypes_function(lpBuffer, lpnSize)
 
 @Kernel32Proxy()
 def GetComputerNameW(lpBuffer, lpnSize):
     return GetComputerNameW.ctypes_function(lpBuffer, lpnSize)
 
 @Kernel32Proxy()
+def GetComputerNameExA(NameType, lpBuffer, nSize):
+    return GetComputerNameExA.ctypes_function(NameType, lpBuffer, nSize)
+
+@Kernel32Proxy()
+def GetComputerNameExW(NameType, lpBuffer, nSize):
+    return GetComputerNameExW.ctypes_function(NameType, lpBuffer, nSize)
+
+@Kernel32Proxy()
 def GetWindowsDirectoryA(lpBuffer, uSize=None):
     if uSize is None:
         uSize = gdef.DWORD(len(lpBuffer))
     return GetWindowsDirectoryA.ctypes_function(lpBuffer, uSize)
 
 @Kernel32Proxy()
 def GetWindowsDirectoryW(lpBuffer, uSize=None):
@@ -385,14 +395,17 @@
         uSize = gdef.DWORD(len(lpBuffer))
     return GetWindowsDirectoryW.ctypes_function(lpBuffer, uSize)
 
 @Kernel32Proxy()
 def GetProductInfo(dwOSMajorVersion, dwOSMinorVersion, dwSpMajorVersion, dwSpMinorVersion, pdwReturnedProductType):
    return GetProductInfo.ctypes_function(dwOSMajorVersion, dwOSMinorVersion, dwSpMajorVersion, dwSpMinorVersion, pdwReturnedProductType)
 
+
+
+
 ## Other
 
 @Kernel32Proxy(error_check=no_error_check)
 def lstrcmpA(lpString1, lpString2):
     return lstrcmpA.ctypes_function(lpString1, lpString2)
 
 @Kernel32Proxy(error_check=no_error_check)
@@ -457,15 +470,15 @@
 @Kernel32Proxy(error_check=result_is_handle)
 def CreateFileA(lpFileName, dwDesiredAccess=gdef.GENERIC_READ, dwShareMode=0, lpSecurityAttributes=None, dwCreationDisposition=gdef.OPEN_EXISTING, dwFlagsAndAttributes=gdef.FILE_ATTRIBUTE_NORMAL, hTemplateFile=None):
     return CreateFileA.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile)
 
 
 @Kernel32Proxy(error_check=result_is_handle)
 def CreateFileW(lpFileName, dwDesiredAccess=gdef.GENERIC_READ, dwShareMode=0, lpSecurityAttributes=None, dwCreationDisposition=gdef.OPEN_EXISTING, dwFlagsAndAttributes=gdef.FILE_ATTRIBUTE_NORMAL, hTemplateFile=None):
-    return CreateFileA.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile)
+    return CreateFileW.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile)
 
 @Kernel32Proxy(error_check=result_is_handle)
 def CreateFileTransactedA(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile, hTransaction, pusMiniVersion, pExtendedParameter):
     return CreateFileTransactedA.ctypes_function(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile, hTransaction, pusMiniVersion, pExtendedParameter)
 
 @Kernel32Proxy(error_check=result_is_handle)
 def CreateFileTransactedW(lpFileName, dwDesiredAccess, dwShareMode, lpSecurityAttributes, dwCreationDisposition, dwFlagsAndAttributes, hTemplateFile, hTransaction, pusMiniVersion, pExtendedParameter):
@@ -534,14 +547,50 @@
     return FindNextFileW.ctypes_function(hFindFile, lpFindFileData)
 
 
 @Kernel32Proxy()
 def FindClose(hFindFile):
     return FindClose.ctypes_function(hFindFile)
 
+@Kernel32Proxy()
+def FindFirstChangeNotificationA(lpPathName, bWatchSubtree, dwNotifyFilter):
+    return FindFirstChangeNotificationA.ctypes_function(lpPathName, bWatchSubtree, dwNotifyFilter)
+
+@Kernel32Proxy()
+def FindFirstChangeNotificationW(lpPathName, bWatchSubtree, dwNotifyFilter):
+    return FindFirstChangeNotificationW.ctypes_function(lpPathName, bWatchSubtree, dwNotifyFilter)
+
+@Kernel32Proxy()
+def FindNextChangeNotification(hChangeHandle):
+    return FindNextChangeNotification.ctypes_function(hChangeHandle)
+
+@Kernel32Proxy()
+def FindCloseChangeNotification(hChangeHandle):
+    return FindCloseChange
+    Notification.ctypes_function(hChangeHandle)
+
+@Kernel32Proxy()
+def FindNextChangeNotification(hChangeHandle):
+    return FindNextChangeNotification.ctypes_function(hChangeHandle)
+
+@Kernel32Proxy()
+def ReadDirectoryChangesW(hDirectory, lpBuffer, nBufferLength, bWatchSubtree, dwNotifyFilter, lpBytesReturned, lpOverlapped, lpCompletionRoutine):
+    return ReadDirectoryChangesW.ctypes_function(hDirectory, lpBuffer, nBufferLength, bWatchSubtree, dwNotifyFilter, lpBytesReturned, lpOverlapped, lpCompletionRoutine)
+
+@Kernel32Proxy()
+def ReadDirectoryChangesExW(hDirectory, lpBuffer, nBufferLength, bWatchSubtree, dwNotifyFilter, lpBytesReturned, lpOverlapped, lpCompletionRoutine, ReadDirectoryNotifyInformationClass):
+    return ReadDirectoryChangesExW.ctypes_function(hDirectory, lpBuffer, nBufferLength, bWatchSubtree, dwNotifyFilter, lpBytesReturned, lpOverlapped, lpCompletionRoutine, ReadDirectoryNotifyInformationClass)
+
+@Kernel32Proxy()
+def LockFile(hFile, dwFileOffsetLow, dwFileOffsetHigh, nNumberOfBytesToLockLow, nNumberOfBytesToLockHigh):
+    return LockFile.ctypes_function(hFile, dwFileOffsetLow, dwFileOffsetHigh, nNumberOfBytesToLockLow, nNumberOfBytesToLockHigh)
+
+@Kernel32Proxy()
+def LockFileEx(hFile, dwFlags, dwReserved, nNumberOfBytesToLockLow, nNumberOfBytesToLockHigh, lpOverlapped):
+    return LockFileEx.ctypes_function(hFile, dwFlags, dwReserved, nNumberOfBytesToLockLow, nNumberOfBytesToLockHigh, lpOverlapped)
 
 ## Tlhelp (snapshoot)
 
 @Kernel32Proxy()
 def CreateToolhelp32Snapshot(dwFlags, th32ProcessID=0):
     return CreateToolhelp32Snapshot.ctypes_function(dwFlags, th32ProcessID)
 
@@ -563,14 +612,23 @@
 def Process32First(hSnapshot, lpte):
     return Process32First.ctypes_function(hSnapshot, lpte)
 
 @Kernel32Proxy(error_check=no_error_check)
 def Process32Next(hSnapshot, lpte):
     return Process32Next.ctypes_function(hSnapshot, lpte)
 
+@Kernel32Proxy()
+def Process32FirstW(hSnapshot, lppe):
+    return Process32FirstW.ctypes_function(hSnapshot, lppe)
+
+@Kernel32Proxy(error_check=no_error_check)
+def Process32NextW(hSnapshot, lppe):
+    return Process32NextW.ctypes_function(hSnapshot, lppe)
+
+
 ## VEH
 
 @Kernel32Proxy()
 def AddVectoredContinueHandler(FirstHandler=1, VectoredHandler=NeededParameter):
     return AddVectoredContinueHandler.ctypes_function(FirstHandler, VectoredHandler)
 
 
@@ -876,8 +934,49 @@
 
 @Kernel32Proxy()
 def EnumResourceNamesA(hModule, lpType, lpEnumFunc, lParam):
     return EnumResourceNamesA.ctypes_function(hModule, lpType, lpEnumFunc, lParam)
 
 @Kernel32Proxy()
 def EnumResourceNamesW(hModule, lpType, lpEnumFunc, lParam):
-    return EnumResourceNamesW.ctypes_function(hModule, lpType, lpEnumFunc, lParam)
+    return EnumResourceNamesW.ctypes_function(hModule, lpType, lpEnumFunc, lParam)
+
+# Environment
+@Kernel32Proxy()
+def GetEnvironmentVariableA(lpName, lpBuffer, nSize):
+    if nSize is None:
+        nSize = ctypes.sizeof(lpBuffer)
+    return GetEnvironmentVariableA.ctypes_function(lpName, lpBuffer, nSize)
+
+@Kernel32Proxy()
+def GetEnvironmentVariableW(lpName, lpBuffer, nSize):
+    if nSize is None:
+        nSize = ctypes.sizeof(lpBuffer)
+    return GetEnvironmentVariableW.ctypes_function(lpName, lpBuffer, nSize)
+
+@Kernel32Proxy()
+def SetEnvironmentVariableA(lpName, lpValue):
+    return SetEnvironmentVariableA.ctypes_function(lpName, lpValue)
+
+@Kernel32Proxy()
+def SetEnvironmentVariableW(lpName, lpValue):
+    return SetEnvironmentVariableW.ctypes_function(lpName, lpValue)
+
+@Kernel32Proxy()
+def GetEnvironmentStringsA():
+    return GetEnvironmentStringsA.ctypes_function()
+
+@Kernel32Proxy()
+def GetEnvironmentStringsW():
+    return GetEnvironmentStringsW.ctypes_function()
+
+@Kernel32Proxy()
+def SetEnvironmentStringsW(NewEnvironment):
+    return SetEnvironmentStringsW.ctypes_function(NewEnvironment)
+
+@Kernel32Proxy()
+def FreeEnvironmentStringsA(penv):
+    return FreeEnvironmentStringsA.ctypes_function(penv)
+
+@Kernel32Proxy()
+def FreeEnvironmentStringsW(penv):
+    return FreeEnvironmentStringsW.ctypes_function(penv)
```

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/ktmw32.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/ktmw32.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/ntdll.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/ntdll.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,18 @@
 
 # Other
 
 @NtdllProxy()
 def RtlEqualUnicodeString(String1, String2, CaseInSensitive):
    return RtlEqualUnicodeString.ctypes_function(String1, String2, CaseInSensitive)
 
+@NtdllProxy(error_check=None)
+def RtlMoveMemory(Destination, Source, Length):
+    return RtlMoveMemory.ctypes_function(Destination, Source, Length)
+
 
 # Firmware
 @NtdllProxy()
 def NtEnumerateSystemEnvironmentValuesEx(InformationClass, Buffer, BufferLength):
     return NtEnumerateSystemEnvironmentValuesEx.ctypes_function(InformationClass, Buffer, BufferLength)
```

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/ole32.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/ole32.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/psapi.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/psapi.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/setupapi.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/setupapi.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/shell32.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/shell32.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/shlwapi.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/shlwapi.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/user32.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/user32.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/version.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/version.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/virtdisk.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/virtdisk.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/wevtapi.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/wevtapi.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/wininet.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/wininet.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/wintrust.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/wintrust.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/winproxy/apis/__init__.py` & `PythonForWindows-0.6.8/windows/winproxy/apis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 from .cryptui import *
 from .dbghelp import *
 from .dnsapi import *
 from .iphlpapi import *
 from .kernel32 import *
 from .ktmw32 import *
 from .ntdll import *
+from .netapi32 import *
 from .ole32 import *
+from .oleaut32 import *
 from .oleacc import *
 from .psapi import *
 from .setupapi import *
 from .shell32 import *
 from .shlwapi import *
 from .tdh import *
 from .user32 import *
 from .version import *
 from .virtdisk import *
 from .wevtapi import *
+from .winhttp import *
 from .wininet import *
-from .wintrust import *
+from .wintrust import *
+from .ws2_32 import *
```

### Comparing `PythonForWindows-0.6.5/windows/winproxy/error.py` & `PythonForWindows-0.6.8/windows/winproxy/error.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/wintrust.py` & `PythonForWindows-0.6.8/windows/wintrust.py`

 * *Files identical despite different names*

### Comparing `PythonForWindows-0.6.5/windows/__init__.py` & `PythonForWindows-0.6.8/windows/__init__.py`

 * *Files identical despite different names*

