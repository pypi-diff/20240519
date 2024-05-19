# Comparing `tmp/routersploit-3.4.2.tar.gz` & `tmp/routersploit-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routersploit-3.4.2.tar", last modified: Sun Apr 14 13:58:44 2024, max compression
+gzip compressed data, was "routersploit-3.4.3.tar", last modified: Sun May 19 17:59:08 2024, max compression
```

## Comparing `routersploit-3.4.2.tar` & `routersploit-3.4.3.tar`

### file list

```diff
@@ -1,1229 +1,1230 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.551218 routersploit-3.4.2/
--rw-r--r--   0 user       (501) staff       (20)     1844 2024-04-08 16:47:10.000000 routersploit-3.4.2/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      175 2024-04-08 16:47:10.000000 routersploit-3.4.2/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     4519 2024-04-14 13:58:44.550940 routersploit-3.4.2/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3515 2024-04-08 16:47:10.000000 routersploit-3.4.2/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.040208 routersploit-3.4.2/routersploit/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.043119 routersploit-3.4.2/routersploit/core/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.043790 routersploit-3.4.2/routersploit/core/bluetooth/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/bluetooth/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.045464 routersploit-3.4.2/routersploit/core/bluetooth/btle/
--rw-r--r--   0 user       (501) staff       (20)      173 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/bluetooth/btle/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    12363 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/bluetooth/btle/btle_device.py
--rw-r--r--   0 user       (501) staff       (20)     2083 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/bluetooth/btle/btle_scanner.py
--rw-r--r--   0 user       (501) staff       (20)     1403 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/bluetooth/btle_client.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.050993 routersploit-3.4.2/routersploit/core/exploit/
--rw-r--r--   0 user       (501) staff       (20)      826 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/exploit/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/exploit/encoders.py
--rw-r--r--   0 user       (501) staff       (20)      263 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/exploit/exceptions.py
--rw-r--r--   0 user       (501) staff       (20)     6511 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/exploit/exploit.py
--rw-r--r--   0 user       (501) staff       (20)     5513 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/exploit/option.py
--rw-r--r--   0 user       (501) staff       (20)     8713 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/exploit/payloads.py
--rw-r--r--   0 user       (501) staff       (20)     5522 2024-04-14 11:08:48.000000 routersploit-3.4.2/routersploit/core/exploit/printer.py
--rw-r--r--   0 user       (501) staff       (20)    13490 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/exploit/shell.py
--rw-r--r--   0 user       (501) staff       (20)    10620 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/exploit/utils.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.052283 routersploit-3.4.2/routersploit/core/ftp/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/ftp/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4359 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/ftp/ftp_client.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.053393 routersploit-3.4.2/routersploit/core/http/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/http/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2830 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/http/http_client.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.054415 routersploit-3.4.2/routersploit/core/snmp/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/snmp/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2893 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/snmp/snmp_client.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.055405 routersploit-3.4.2/routersploit/core/ssh/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/ssh/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    11443 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/ssh/ssh_client.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.056735 routersploit-3.4.2/routersploit/core/tcp/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/tcp/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4676 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/tcp/tcp_client.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.057769 routersploit-3.4.2/routersploit/core/telnet/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/telnet/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     6005 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/telnet/telnet_client.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.059334 routersploit-3.4.2/routersploit/core/udp/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/udp/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3337 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/core/udp/udp_client.py
--rw-r--r--   0 user       (501) staff       (20)    25107 2024-04-14 13:51:02.000000 routersploit-3.4.2/routersploit/interpreter.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.061593 routersploit-3.4.2/routersploit/libs/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/libs/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.063011 routersploit-3.4.2/routersploit/libs/apiros/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/libs/apiros/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     9779 2024-04-10 18:54:42.000000 routersploit-3.4.2/routersploit/libs/apiros/apiros_client.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.064604 routersploit-3.4.2/routersploit/libs/lzs/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/libs/lzs/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3842 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/libs/lzs/lzs.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.065309 routersploit-3.4.2/routersploit/modules/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.065801 routersploit-3.4.2/routersploit/modules/creds/
--rw-r--r--   0 user       (501) staff       (20)       20 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.066583 routersploit-3.4.2/routersploit/modules/creds/cameras/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.069321 routersploit-3.4.2/routersploit/modules/creds/cameras/acti/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/acti/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      906 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/acti/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      907 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/acti/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      925 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/acti/telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)     3079 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/acti/webinterface_http_form_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.071768 routersploit-3.4.2/routersploit/modules/creds/cameras/american_dynamics/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/american_dynamics/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      895 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/american_dynamics/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      894 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/american_dynamics/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      896 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/american_dynamics/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.074349 routersploit-3.4.2/routersploit/modules/creds/cameras/arecont/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/arecont/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/arecont/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/arecont/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/arecont/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.077160 routersploit-3.4.2/routersploit/modules/creds/cameras/avigilon/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/avigilon/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/avigilon/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      870 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/avigilon/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      888 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/avigilon/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.079875 routersploit-3.4.2/routersploit/modules/creds/cameras/avtech/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/avtech/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/avtech/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/avtech/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      867 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/avtech/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.085565 routersploit-3.4.2/routersploit/modules/creds/cameras/axis/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/axis/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/axis/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/axis/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      872 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/axis/telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      915 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/axis/webinterface_http_auth_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.088234 routersploit-3.4.2/routersploit/modules/creds/cameras/basler/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/basler/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/basler/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/basler/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      866 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/basler/telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)     3003 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/basler/webinterface_http_form_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.091935 routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      854 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      855 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      866 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      946 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/webinterface_http_auth_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.096148 routersploit-3.4.2/routersploit/modules/creds/cameras/canon/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/canon/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      846 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/canon/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      846 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/canon/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/canon/telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      965 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/canon/webinterface_http_auth_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.099060 routersploit-3.4.2/routersploit/modules/creds/cameras/cisco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/cisco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      755 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/cisco/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      823 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/cisco/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      840 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/cisco/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.100859 routersploit-3.4.2/routersploit/modules/creds/cameras/dlink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/dlink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      848 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/dlink/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      825 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/dlink/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      866 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/dlink/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.103283 routersploit-3.4.2/routersploit/modules/creds/cameras/geovision/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/geovision/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      858 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/geovision/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/geovision/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/geovision/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.105826 routersploit-3.4.2/routersploit/modules/creds/cameras/grandstream/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/grandstream/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/grandstream/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/grandstream/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/grandstream/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.107977 routersploit-3.4.2/routersploit/modules/creds/cameras/hikvision/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/hikvision/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      847 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/hikvision/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      858 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/hikvision/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      877 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/hikvision/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.110288 routersploit-3.4.2/routersploit/modules/creds/cameras/honeywell/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/honeywell/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/honeywell/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      858 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/honeywell/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/honeywell/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.112852 routersploit-3.4.2/routersploit/modules/creds/cameras/iqinvision/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/iqinvision/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      861 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/iqinvision/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      861 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/iqinvision/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      878 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/iqinvision/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.114896 routersploit-3.4.2/routersploit/modules/creds/cameras/jvc/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/jvc/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      838 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/jvc/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      838 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/jvc/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/jvc/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.117169 routersploit-3.4.2/routersploit/modules/creds/cameras/mobotix/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/mobotix/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/mobotix/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/mobotix/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      870 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/mobotix/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.119378 routersploit-3.4.2/routersploit/modules/creds/cameras/samsung/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/samsung/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      875 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/samsung/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/samsung/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      894 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/samsung/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.121728 routersploit-3.4.2/routersploit/modules/creds/cameras/sentry360/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/sentry360/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/sentry360/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/sentry360/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      874 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/sentry360/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.124117 routersploit-3.4.2/routersploit/modules/creds/cameras/siemens/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/siemens/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/siemens/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/siemens/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      870 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/siemens/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.126392 routersploit-3.4.2/routersploit/modules/creds/cameras/speco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/speco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      845 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/speco/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      845 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/speco/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      862 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/speco/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.129202 routersploit-3.4.2/routersploit/modules/creds/cameras/stardot/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/stardot/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/stardot/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/stardot/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/stardot/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.131402 routersploit-3.4.2/routersploit/modules/creds/cameras/vacron/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/vacron/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/vacron/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/vacron/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      869 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/vacron/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.133444 routersploit-3.4.2/routersploit/modules/creds/cameras/videoiq/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/videoiq/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      863 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/videoiq/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      862 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/videoiq/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      880 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/cameras/videoiq/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.138646 routersploit-3.4.2/routersploit/modules/creds/generic/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3118 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/ftp_bruteforce.py
--rw-r--r--   0 user       (501) staff       (20)     2968 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/ftp_default.py
--rw-r--r--   0 user       (501) staff       (20)     4427 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/http_basic_digest_bruteforce.py
--rw-r--r--   0 user       (501) staff       (20)     4312 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/http_basic_digest_default.py
--rw-r--r--   0 user       (501) staff       (20)     2511 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/snmp_bruteforce.py
--rw-r--r--   0 user       (501) staff       (20)     2920 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/ssh_bruteforce.py
--rw-r--r--   0 user       (501) staff       (20)     2784 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/ssh_default.py
--rw-r--r--   0 user       (501) staff       (20)     2990 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/telnet_bruteforce.py
--rw-r--r--   0 user       (501) staff       (20)     2879 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/generic/telnet_default.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.139024 routersploit-3.4.2/routersploit/modules/creds/printers/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/printers/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.139318 routersploit-3.4.2/routersploit/modules/creds/routers/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.141173 routersploit-3.4.2/routersploit/modules/creds/routers/2wire/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/2wire/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      915 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/2wire/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      915 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/2wire/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      930 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/2wire/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.143457 routersploit-3.4.2/routersploit/modules/creds/routers/3com/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/3com/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      912 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/3com/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      912 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/3com/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      927 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/3com/telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.145651 routersploit-3.4.2/routersploit/modules/creds/routers/asmax/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/asmax/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      873 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/asmax/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      873 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/asmax/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      888 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/asmax/telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      977 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/asmax/webinterface_http_auth_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.147430 routersploit-3.4.2/routersploit/modules/creds/routers/asus/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/asus/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/asus/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/asus/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      899 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/asus/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.149313 routersploit-3.4.2/routersploit/modules/creds/routers/belkin/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/belkin/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/belkin/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/belkin/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      883 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/belkin/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.150927 routersploit-3.4.2/routersploit/modules/creds/routers/bhu/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/bhu/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/bhu/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/bhu/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      860 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/bhu/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.152827 routersploit-3.4.2/routersploit/modules/creds/routers/billion/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/billion/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/billion/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/billion/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/billion/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.154906 routersploit-3.4.2/routersploit/modules/creds/routers/cisco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/cisco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      847 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/cisco/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      847 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/cisco/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      866 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/cisco/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.156695 routersploit-3.4.2/routersploit/modules/creds/routers/comtrend/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/comtrend/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      856 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/comtrend/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      856 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/comtrend/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      875 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/comtrend/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.158399 routersploit-3.4.2/routersploit/modules/creds/routers/dlink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/dlink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/dlink/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/dlink/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      899 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/dlink/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.161919 routersploit-3.4.2/routersploit/modules/creds/routers/fortinet/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/fortinet/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      892 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/fortinet/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      892 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/fortinet/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      910 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/fortinet/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.163943 routersploit-3.4.2/routersploit/modules/creds/routers/huawei/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/huawei/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      965 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/huawei/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      965 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/huawei/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      983 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/huawei/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.165655 routersploit-3.4.2/routersploit/modules/creds/routers/ipfire/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/ipfire/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      867 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/ipfire/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      867 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/ipfire/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      885 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/ipfire/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.167283 routersploit-3.4.2/routersploit/modules/creds/routers/juniper/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/juniper/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      901 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/juniper/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      899 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/juniper/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      919 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/juniper/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.168755 routersploit-3.4.2/routersploit/modules/creds/routers/linksys/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/linksys/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/linksys/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/linksys/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      905 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/linksys/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.170843 routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3970 2024-04-10 18:54:42.000000 routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/api_ros_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      854 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      854 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      872 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.173223 routersploit-3.4.2/routersploit/modules/creds/routers/movistar/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/movistar/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/movistar/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/movistar/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      883 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/movistar/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.174713 routersploit-3.4.2/routersploit/modules/creds/routers/netcore/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netcore/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netcore/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netcore/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      882 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netcore/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.176640 routersploit-3.4.2/routersploit/modules/creds/routers/netgear/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netgear/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netgear/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netgear/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      889 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netgear/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.178480 routersploit-3.4.2/routersploit/modules/creds/routers/netsys/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netsys/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netsys/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netsys/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      862 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/netsys/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.179613 routersploit-3.4.2/routersploit/modules/creds/routers/pfsense/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/pfsense/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      848 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/pfsense/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)     2144 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/pfsense/webinterface_http_form_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.181438 routersploit-3.4.2/routersploit/modules/creds/routers/technicolor/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/technicolor/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      906 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/technicolor/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      906 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/technicolor/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      924 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/technicolor/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.183220 routersploit-3.4.2/routersploit/modules/creds/routers/thomson/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/thomson/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      868 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/thomson/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      868 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/thomson/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      886 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/thomson/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.184741 routersploit-3.4.2/routersploit/modules/creds/routers/tplink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/tplink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/tplink/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/tplink/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/tplink/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.186501 routersploit-3.4.2/routersploit/modules/creds/routers/ubiquiti/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/ubiquiti/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/ubiquiti/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/ubiquiti/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      894 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/ubiquiti/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.188426 routersploit-3.4.2/routersploit/modules/creds/routers/zte/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/zte/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      896 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/zte/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      896 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/zte/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      914 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/zte/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.190794 routersploit-3.4.2/routersploit/modules/creds/routers/zyxel/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/zyxel/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/zyxel/ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/zyxel/ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      905 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/creds/routers/zyxel/telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.191207 routersploit-3.4.2/routersploit/modules/encoders/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/encoders/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.192481 routersploit-3.4.2/routersploit/modules/encoders/php/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/encoders/php/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      630 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/encoders/php/base64.py
--rw-r--r--   0 user       (501) staff       (20)      616 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/encoders/php/hex.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.195047 routersploit-3.4.2/routersploit/modules/encoders/python/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/encoders/python/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      640 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/encoders/python/base64.py
--rw-r--r--   0 user       (501) staff       (20)      583 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/encoders/python/hex.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.195838 routersploit-3.4.2/routersploit/modules/exploits/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.196242 routersploit-3.4.2/routersploit/modules/exploits/cameras/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.196863 routersploit-3.4.2/routersploit/modules/exploits/cameras/avigilon/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/avigilon/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2282 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/avigilon/videoiq_camera_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.198400 routersploit-3.4.2/routersploit/modules/exploits/cameras/brickcom/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/brickcom/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3907 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/brickcom/corp_network_cameras_conf_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2342 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/brickcom/users_cgi_creds_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.199521 routersploit-3.4.2/routersploit/modules/exploits/cameras/cisco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/cisco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2160 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/cisco/video_surv_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.200646 routersploit-3.4.2/routersploit/modules/exploits/cameras/dlink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/dlink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3754 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/dlink/dcs_930l_932l_auth_bypass.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.202404 routersploit-3.4.2/routersploit/modules/exploits/cameras/grandstream/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/grandstream/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2200 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/grandstream/gxv3611hd_ip_camera_backdoor.py
--rw-r--r--   0 user       (501) staff       (20)     2388 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/grandstream/gxv3611hd_ip_camera_sqli.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.203460 routersploit-3.4.2/routersploit/modules/exploits/cameras/honeywell/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/honeywell/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1500 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/honeywell/hicc_1100pt_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.204516 routersploit-3.4.2/routersploit/modules/exploits/cameras/jovision/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/jovision/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2820 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/jovision/jovision_credentials_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.207395 routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/
--rw-r--r--   0 user       (501) staff       (20)    41546 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/P2P_wificam_credential_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)    42581 2024-04-09 15:50:17.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/P2P_wificam_rce.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2137 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/dvr_creds_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2555 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/jvc_vanderbilt_honeywell_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     2874 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/netwave_ip_camera_information_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.208038 routersploit-3.4.2/routersploit/modules/exploits/cameras/mvpower/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/mvpower/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1978 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/mvpower/dvr_jaws_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.208727 routersploit-3.4.2/routersploit/modules/exploits/cameras/siemens/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/siemens/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1634 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/siemens/cvms2025_credentials_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.209428 routersploit-3.4.2/routersploit/modules/exploits/cameras/xiongmai/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/xiongmai/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2076 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/cameras/xiongmai/uc_httpd_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.211815 routersploit-3.4.2/routersploit/modules/exploits/generic/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/generic/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    14911 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/generic/heartbleed.py
--rw-r--r--   0 user       (501) staff       (20)     2982 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/generic/shellshock.py
--rw-r--r--   0 user       (501) staff       (20)     4092 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/generic/ssh_auth_keys.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.212370 routersploit-3.4.2/routersploit/modules/exploits/misc/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/misc/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.213324 routersploit-3.4.2/routersploit/modules/exploits/misc/asus/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/misc/asus/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1667 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/misc/asus/b1m_projector_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.214395 routersploit-3.4.2/routersploit/modules/exploits/misc/miele/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/misc/miele/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1962 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/misc/miele/pg8528_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.215253 routersploit-3.4.2/routersploit/modules/exploits/misc/wepresent/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/misc/wepresent/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1842 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/misc/wepresent/wipg1000_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.215661 routersploit-3.4.2/routersploit/modules/exploits/routers/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.216745 routersploit-3.4.2/routersploit/modules/exploits/routers/2wire/
--rw-r--r--   0 user       (501) staff       (20)     2601 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/2wire/4011g_5012nv_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/2wire/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1982 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/2wire/gateway_auth_bypass.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.219629 routersploit-3.4.2/routersploit/modules/exploits/routers/3com/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/3com/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2033 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/3com/ap8760_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2293 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/3com/imc_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2244 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/3com/imc_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     2233 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/3com/officeconnect_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2013 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/3com/officeconnect_rce.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.221115 routersploit-3.4.2/routersploit/modules/exploits/routers/asmax/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/asmax/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2087 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/asmax/ar_1004g_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2009 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/asmax/ar_804_gu_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.222898 routersploit-3.4.2/routersploit/modules/exploits/routers/asus/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/asus/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3476 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/asus/asuswrt_lan_rce.py
--rw-r--r--   0 user       (501) staff       (20)     3353 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/asus/infosvr_backdoor_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2052 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/asus/rt_n16_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.226324 routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2254 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/auth_bypass.py
--rw-r--r--   0 user       (501) staff       (20)     1968 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/g_n150_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2430 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/g_plus_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2080 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/n150_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     1902 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/n750_rce.py
--rw-r--r--   0 user       (501) staff       (20)     3737 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/play_max_prce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.227254 routersploit-3.4.2/routersploit/modules/exploits/routers/bhu/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/bhu/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3099 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/bhu/bhu_urouter_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.229097 routersploit-3.4.2/routersploit/modules/exploits/routers/billion/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/billion/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     5149 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/billion/billion_5200w_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2321 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/billion/billion_7700nr4_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.233950 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     9688 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/catalyst_2960_rocem.py
--rw-r--r--   0 user       (501) staff       (20)     1718 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/dpc2420_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     3554 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/firepower_management60_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     5241 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/firepower_management60_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2323 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/ios_http_authorization_bypass.py
--rw-r--r--   0 user       (501) staff       (20)     3768 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/secure_acs_bypass.py
--rw-r--r--   0 user       (501) staff       (20)     1932 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/ucm_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2042 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/ucs_manager_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2863 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/unified_multi_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.234708 routersploit-3.4.2/routersploit/modules/exploits/routers/comtrend/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/comtrend/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2598 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/comtrend/ct_5361t_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.247331 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2585 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dcs_930l_auth_rce.py
--rw-r--r--   0 user       (501) staff       (20)     5438 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dgs_1510_add_user.py
--rw-r--r--   0 user       (501) staff       (20)     2117 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_300_320_600_615_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2408 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_300_320_615_auth_bypass.py
--rw-r--r--   0 user       (501) staff       (20)     1948 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_300_600_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2451 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_300_645_815_upnp_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2469 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_645_815_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2251 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_645_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1738 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_815_850l_rce.py
--rw-r--r--   0 user       (501) staff       (20)     3044 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_825_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     2237 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_850l_creds_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2148 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_8xx_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2286 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dns_320l_327l_rce.py
--rw-r--r--   0 user       (501) staff       (20)     1959 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2640b_dns_change.py
--rw-r--r--   0 user       (501) staff       (20)     2171 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2730_2750_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     2003 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2730b_2780b_526b_dns_change.py
--rw-r--r--   0 user       (501) staff       (20)     1861 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2740r_dns_change.py
--rw-r--r--   0 user       (501) staff       (20)     2133 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2750b_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1722 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2750b_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2000 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsp_w110_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2693 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dvg_n5402sp_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     2935 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dwl_3200ap_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2650 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dwr_932_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1654 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dwr_932b_backdoor.py
--rw-r--r--   0 user       (501) staff       (20)     2826 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/multi_hedwig_cgi_exec.py
--rw-r--r--   0 user       (501) staff       (20)     2701 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/multi_hnap_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.248242 routersploit-3.4.2/routersploit/modules/exploits/routers/fortinet/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/fortinet/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3412 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/fortinet/fortigate_os_backdoor.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.251079 routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2304 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/e5331_mifi_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     6409 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/hg520_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     3157 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/hg530_hg520b_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2379 2024-04-14 11:08:48.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/hg532_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2142 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/hg866_password_change.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.252859 routersploit-3.4.2/routersploit/modules/exploits/routers/ipfire/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/ipfire/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2732 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/ipfire/ipfire_oinkcode_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2583 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/ipfire/ipfire_proxy_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2615 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/ipfire/ipfire_shellshock.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.256551 routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/
--rw-r--r--   0 user       (501) staff       (20)     2747 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/1500_2500_rce.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3564 2024-04-14 11:08:48.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/eseries_themoon_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2582 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/smartwifi_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1853 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/wap54gv3_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2681 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/wrt100_110_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.258245 routersploit-3.4.2/routersploit/modules/exploits/routers/mikrotik/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/mikrotik/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4161 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/mikrotik/routeros_jailbreak.py
--rw-r--r--   0 user       (501) staff       (20)     4260 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/mikrotik/winbox_auth_bypass_creds_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.259068 routersploit-3.4.2/routersploit/modules/exploits/routers/movistar/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/movistar/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1964 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/movistar/adsl_router_bhs_rta_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.263069 routersploit-3.4.2/routersploit/modules/exploits/routers/multi/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/multi/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2309 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/multi/gpon_home_gateway_rce.py
--rw-r--r--   0 user       (501) staff       (20)    17579 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/multi/misfortune_cookie.py
--rw-r--r--   0 user       (501) staff       (20)     3372 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/multi/rom0.py
--rw-r--r--   0 user       (501) staff       (20)     3610 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/multi/tcp_32764_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     3145 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/multi/tcp_32764_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.263909 routersploit-3.4.2/routersploit/modules/exploits/routers/netcore/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netcore/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2133 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netcore/udp_53413_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.268721 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1714 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/dgn2200_dnslookup_cgi_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/dgn2200_ping_cgi_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2301 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/jnr1010_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     5350 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/multi_password_disclosure-2017-5521.py
--rw-r--r--   0 user       (501) staff       (20)     3365 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/multi_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2461 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/n300_auth_bypass.py
--rw-r--r--   0 user       (501) staff       (20)     2281 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/prosafe_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2356 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/r7000_r6400_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2449 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/wnr500_612v3_jnr1010_2010_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.269392 routersploit-3.4.2/routersploit/modules/exploits/routers/netsys/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netsys/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2656 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/netsys/multi_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.270499 routersploit-3.4.2/routersploit/modules/exploits/routers/shuttle/
--rw-r--r--   0 user       (501) staff       (20)     1907 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/shuttle/915wm_dns_change.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/shuttle/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.273245 routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3360 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/dwg855_authbypass.py
--rw-r--r--   0 user       (501) staff       (20)     1713 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/tc7200_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2875 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/tc7200_password_disclosure_v2.py
--rw-r--r--   0 user       (501) staff       (20)     2926 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/tg784_authbypass.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.274604 routersploit-3.4.2/routersploit/modules/exploits/routers/thomson/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/thomson/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2449 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/thomson/twg849_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1712 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/thomson/twg850_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.277386 routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3280 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/archer_c2_c20i_rce.py
--rw-r--r--   0 user       (501) staff       (20)     4631 2024-04-14 11:13:53.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/archer_c9_admin_password_reset.py
--rw-r--r--   0 user       (501) staff       (20)     2212 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/wdr740nd_wdr740n_backdoor.py
--rw-r--r--   0 user       (501) staff       (20)     2310 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/wdr740nd_wdr740n_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     4315 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/wdr842nd_wdr842n_configure_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.278242 routersploit-3.4.2/routersploit/modules/exploits/routers/ubiquiti/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/ubiquiti/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3802 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/ubiquiti/airos_6_x.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.280221 routersploit-3.4.2/routersploit/modules/exploits/routers/zte/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zte/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2133 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zte/f460_f660_backdoor.py
--rw-r--r--   0 user       (501) staff       (20)     2191 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zte/zxhn_h108n_wifi_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     5245 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zte/zxv10_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.282661 routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2897 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/d1000_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2421 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/d1000_wifi_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2158 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/p660hn_t_v1_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2941 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/p660hn_t_v2_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2404 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/zywall_usg_extract_hashes.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.283186 routersploit-3.4.2/routersploit/modules/generic/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/generic/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.284738 routersploit-3.4.2/routersploit/modules/generic/bluetooth/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/generic/bluetooth/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      795 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/generic/bluetooth/btle_enumerate.py
--rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/generic/bluetooth/btle_scan.py
--rw-r--r--   0 user       (501) staff       (20)     1102 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/generic/bluetooth/btle_write.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.285576 routersploit-3.4.2/routersploit/modules/generic/upnp/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/generic/upnp/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1795 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/generic/upnp/ssdp_msearch.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.286100 routersploit-3.4.2/routersploit/modules/payloads/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.287498 routersploit-3.4.2/routersploit/modules/payloads/armle/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/armle/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2861 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/armle/bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     1409 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/armle/reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.296050 routersploit-3.4.2/routersploit/modules/payloads/cmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      706 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/awk_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      706 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/awk_bind_udp.py
--rw-r--r--   0 user       (501) staff       (20)      740 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/awk_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      583 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/bash_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      701 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/netcat_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      758 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/netcat_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      597 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/perl_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      612 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/perl_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      583 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/php_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      598 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/php_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      607 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/python_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      603 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/python_bind_udp.py
--rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/python_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      612 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/cmd/python_reverse_udp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.297200 routersploit-3.4.2/routersploit/modules/payloads/mipsbe/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/mipsbe/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4812 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/mipsbe/bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     3942 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/mipsbe/reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.298745 routersploit-3.4.2/routersploit/modules/payloads/mipsle/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/mipsle/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4089 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/mipsle/bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     3891 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/mipsle/reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.299938 routersploit-3.4.2/routersploit/modules/payloads/perl/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/perl/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      967 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/perl/bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      985 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/perl/reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.301086 routersploit-3.4.2/routersploit/modules/payloads/php/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/php/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1212 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/php/bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/php/reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.303395 routersploit-3.4.2/routersploit/modules/payloads/python/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/python/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1160 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/python/bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     1159 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/python/bind_udp.py
--rw-r--r--   0 user       (501) staff       (20)     1042 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/python/reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     1148 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/python/reverse_udp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.304929 routersploit-3.4.2/routersploit/modules/payloads/x64/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/x64/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3368 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/x64/bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     2998 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/x64/reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.306372 routersploit-3.4.2/routersploit/modules/payloads/x86/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/x86/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3211 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/x86/bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     2815 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/payloads/x86/reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.307098 routersploit-3.4.2/routersploit/modules/scanners/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/scanners/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    10271 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/scanners/autopwn.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.308004 routersploit-3.4.2/routersploit/modules/scanners/cameras/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/scanners/cameras/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      427 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/scanners/cameras/camera_scan.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.308903 routersploit-3.4.2/routersploit/modules/scanners/misc/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/scanners/misc/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      431 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/scanners/misc/misc_scan.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.309594 routersploit-3.4.2/routersploit/modules/scanners/routers/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/scanners/routers/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      426 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/modules/scanners/routers/router_scan.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.310051 routersploit-3.4.2/routersploit/resources/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.319349 routersploit-3.4.2/routersploit/resources/ssh_keys/
--rw-r--r--   0 user       (501) staff       (20)      634 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/array-networks-vapv-vxag.json
--rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/array-networks-vapv-vxag.key
--rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/barracuda_load_balancer_vm.json
--rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/barracuda_load_balancer_vm.key
--rw-r--r--   0 user       (501) staff       (20)      275 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/ceragon-fibeair-cve-2015-0936.json
--rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/ceragon-fibeair-cve-2015-0936.key
--rw-r--r--   0 user       (501) staff       (20)      254 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/exagrid-cve-2016-1561.json
--rw-r--r--   0 user       (501) staff       (20)      883 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/exagrid-cve-2016-1561.key
--rw-r--r--   0 user       (501) staff       (20)      271 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/f5-bigip-cve-2012-1493.json
--rw-r--r--   0 user       (501) staff       (20)      883 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/f5-bigip-cve-2012-1493.key
--rw-r--r--   0 user       (501) staff       (20)      647 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/loadbalancer.org-enterprise-va.json
--rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/loadbalancer.org-enterprise-va.key
--rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/monroe-dasdec-cve-2013-0137.json
--rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/monroe-dasdec-cve-2013-0137.key
--rw-r--r--   0 user       (501) staff       (20)      634 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/quantum-dxi-v1000.json
--rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/quantum-dxi-v1000.key
--rw-r--r--   0 user       (501) staff       (20)      457 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/vagrant.json
--rw-r--r--   0 user       (501) staff       (20)     1675 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/ssh_keys/vagrant.key
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.319927 routersploit-3.4.2/routersploit/resources/vendors/
--rw-r--r--   0 user       (501) staff       (20)   589907 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/vendors/oui.dat
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.324764 routersploit-3.4.2/routersploit/resources/wordlists/
--rw-r--r--   0 user       (501) staff       (20)      343 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/wordlists/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     9596 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/wordlists/defaults.txt
--rw-r--r--   0 user       (501) staff       (20)     5946 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/wordlists/passwords.txt
--rw-r--r--   0 user       (501) staff       (20)      839 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/wordlists/snmp.txt
--rw-r--r--   0 user       (501) staff       (20)     2512 2024-04-08 16:47:10.000000 routersploit-3.4.2/routersploit/resources/wordlists/usernames.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.042613 routersploit-3.4.2/routersploit.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     4519 2024-04-14 13:58:43.000000 routersploit-3.4.2/routersploit.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)    53910 2024-04-14 13:58:43.000000 routersploit-3.4.2/routersploit.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-14 13:58:43.000000 routersploit-3.4.2/routersploit.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       95 2024-04-14 13:58:43.000000 routersploit-3.4.2/routersploit.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       19 2024-04-14 13:58:43.000000 routersploit-3.4.2/routersploit.egg-info/top_level.txt
--rwxr-xr-x   0 user       (501) staff       (20)      884 2024-04-08 16:47:10.000000 routersploit-3.4.2/rsf.py
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-14 13:58:44.551360 routersploit-3.4.2/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)     1507 2024-04-14 13:51:45.000000 routersploit-3.4.2/setup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.329527 routersploit-3.4.2/tests/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2118 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/conftest.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.330993 routersploit-3.4.2/tests/core/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/core/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     7275 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/core/test_option.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.331830 routersploit-3.4.2/tests/creds/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.332411 routersploit-3.4.2/tests/creds/cameras/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.335569 routersploit-3.4.2/tests/creds/cameras/acti/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/acti/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      663 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/acti/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      639 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/acti/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      672 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/acti/test_telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      988 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/acti/test_webinterface_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.337833 routersploit-3.4.2/tests/creds/cameras/american_dynamics/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/american_dynamics/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/american_dynamics/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/american_dynamics/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      651 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/american_dynamics/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.340791 routersploit-3.4.2/tests/creds/cameras/arecont/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/arecont/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/arecont/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      594 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/arecont/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/arecont/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.343585 routersploit-3.4.2/tests/creds/cameras/avigilon/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/avigilon/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/avigilon/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      613 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/avigilon/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/avigilon/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.346495 routersploit-3.4.2/tests/creds/cameras/avtech/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/avtech/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/avtech/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      593 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/avtech/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      626 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/avtech/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.349874 routersploit-3.4.2/tests/creds/cameras/axis/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/axis/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/axis/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      604 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/axis/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/axis/test_telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)     1182 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/axis/test_webinterface_http_auth_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.351932 routersploit-3.4.2/tests/creds/cameras/basler/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/basler/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/basler/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      593 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/basler/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      626 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/basler/test_telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      751 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/basler/test_webinterface_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.354653 routersploit-3.4.2/tests/creds/cameras/brickcom/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/brickcom/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/brickcom/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      595 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/brickcom/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/brickcom/test_telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)     1162 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/brickcom/test_webinterface_http_auth_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.357082 routersploit-3.4.2/tests/creds/cameras/canon/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/canon/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      616 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/canon/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      592 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/canon/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      625 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/canon/test_telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)     1175 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/canon/test_webinterface_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.359701 routersploit-3.4.2/tests/creds/cameras/cisco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/cisco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      616 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/cisco/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      592 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/cisco/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      625 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/cisco/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.362326 routersploit-3.4.2/tests/creds/cameras/dlink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/dlink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      616 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/dlink/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      592 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/dlink/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      625 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/dlink/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.364482 routersploit-3.4.2/tests/creds/cameras/geovision/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/geovision/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/geovision/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      596 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/geovision/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      629 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/geovision/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.366239 routersploit-3.4.2/tests/creds/cameras/grandstream/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/grandstream/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      622 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/grandstream/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      598 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/grandstream/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      631 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/grandstream/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.367748 routersploit-3.4.2/tests/creds/cameras/hikvision/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/hikvision/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/hikvision/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      597 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/hikvision/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      629 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/hikvision/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.369405 routersploit-3.4.2/tests/creds/cameras/honeywell/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/honeywell/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/honeywell/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      595 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/honeywell/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/honeywell/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.371572 routersploit-3.4.2/tests/creds/cameras/iqinvision/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/iqinvision/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      621 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/iqinvision/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      597 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/iqinvision/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      630 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/iqinvision/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.373240 routersploit-3.4.2/tests/creds/cameras/jvc/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/jvc/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      612 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/jvc/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      588 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/jvc/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      621 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/jvc/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.374675 routersploit-3.4.2/tests/creds/cameras/mobotix/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/mobotix/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/mobotix/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      595 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/mobotix/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/mobotix/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.376262 routersploit-3.4.2/tests/creds/cameras/samsung/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/samsung/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      648 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/samsung/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      624 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/samsung/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      657 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/samsung/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.378123 routersploit-3.4.2/tests/creds/cameras/sentry360/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/sentry360/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/sentry360/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      595 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/sentry360/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/sentry360/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.379936 routersploit-3.4.2/tests/creds/cameras/siemens/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/siemens/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/siemens/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      594 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/siemens/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/siemens/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.381516 routersploit-3.4.2/tests/creds/cameras/speco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/speco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      615 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/speco/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      591 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/speco/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      624 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/speco/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.382989 routersploit-3.4.2/tests/creds/cameras/stardot/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/stardot/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/stardot/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      594 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/stardot/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/stardot/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.384370 routersploit-3.4.2/tests/creds/cameras/vacron/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/vacron/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/vacron/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      593 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/vacron/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      626 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/vacron/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.385775 routersploit-3.4.2/tests/creds/cameras/videoiq/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/videoiq/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/videoiq/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      604 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/videoiq/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/cameras/videoiq/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.386133 routersploit-3.4.2/tests/creds/routers/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.387552 routersploit-3.4.2/tests/creds/routers/2wire/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/2wire/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      749 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/2wire/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      725 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/2wire/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      758 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/2wire/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.389735 routersploit-3.4.2/tests/creds/routers/3com/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/3com/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      748 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/3com/test_3com_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      724 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/3com/test_3com_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      757 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/3com/test_3com_telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.392143 routersploit-3.4.2/tests/creds/routers/asmax/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/asmax/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      649 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/asmax/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      625 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/asmax/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      658 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/asmax/test_telnet_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)     1213 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/asmax/test_webinterface_http_auth_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.394578 routersploit-3.4.2/tests/creds/routers/asus/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/asus/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/asus/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/asus/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      671 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/asus/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.396485 routersploit-3.4.2/tests/creds/routers/belkin/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/belkin/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      636 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/belkin/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      636 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/belkin/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      645 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/belkin/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.398528 routersploit-3.4.2/tests/creds/routers/bhu/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/bhu/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      615 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/bhu/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      615 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/bhu/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      624 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/bhu/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.401099 routersploit-3.4.2/tests/creds/routers/billion/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/billion/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/billion/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/billion/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/billion/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.402916 routersploit-3.4.2/tests/creds/routers/cisco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/cisco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/cisco/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/cisco/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      626 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/cisco/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.404669 routersploit-3.4.2/tests/creds/routers/comtrend/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/comtrend/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/comtrend/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/comtrend/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      629 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/comtrend/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.406731 routersploit-3.4.2/tests/creds/routers/dlink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/dlink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      657 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/dlink/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      657 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/dlink/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      666 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/dlink/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.408335 routersploit-3.4.2/tests/creds/routers/fortinet/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/fortinet/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/fortinet/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/fortinet/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      671 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/fortinet/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.410161 routersploit-3.4.2/tests/creds/routers/huawei/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/huawei/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      758 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/huawei/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      758 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/huawei/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      767 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/huawei/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.411907 routersploit-3.4.2/tests/creds/routers/ipfire/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/ipfire/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/ipfire/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/ipfire/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      651 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/ipfire/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.413486 routersploit-3.4.2/tests/creds/routers/juniper/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/juniper/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      671 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/juniper/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      671 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/juniper/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      680 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/juniper/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.415097 routersploit-3.4.2/tests/creds/routers/linksys/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/linksys/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      663 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/linksys/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      663 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/linksys/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      672 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/linksys/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.417095 routersploit-3.4.2/tests/creds/routers/mikrotik/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/mikrotik/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      396 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/mikrotik/test_api_ros_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/mikrotik/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/mikrotik/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      629 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/mikrotik/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.418609 routersploit-3.4.2/tests/creds/routers/movistar/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/movistar/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      633 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/movistar/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      633 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/movistar/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/movistar/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.420323 routersploit-3.4.2/tests/creds/routers/netcore/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netcore/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      634 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netcore/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      634 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netcore/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      643 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netcore/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.422135 routersploit-3.4.2/tests/creds/routers/netgear/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netgear/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      643 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netgear/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      643 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netgear/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      652 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netgear/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.424349 routersploit-3.4.2/tests/creds/routers/netsys/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netsys/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netsys/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netsys/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/netsys/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.425304 routersploit-3.4.2/tests/creds/routers/pfsense/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/pfsense/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      621 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/pfsense/test_ssh_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.427905 routersploit-3.4.2/tests/creds/routers/technicolor/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/technicolor/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      673 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/technicolor/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      673 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/technicolor/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      682 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/technicolor/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.429816 routersploit-3.4.2/tests/creds/routers/thomson/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/thomson/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/thomson/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/thomson/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/thomson/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.431553 routersploit-3.4.2/tests/creds/routers/tplink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/tplink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/tplink/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/tplink/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/tplink/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.433207 routersploit-3.4.2/tests/creds/routers/ubiquiti/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/ubiquiti/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/ubiquiti/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/ubiquiti/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      655 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/ubiquiti/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.434869 routersploit-3.4.2/tests/creds/routers/zte/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/zte/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      685 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/zte/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      685 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/zte/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      694 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/zte/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.436343 routersploit-3.4.2/tests/creds/routers/zyxel/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/zyxel/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      665 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/zyxel/test_ftp_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      665 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/zyxel/test_ssh_default_creds.py
--rw-r--r--   0 user       (501) staff       (20)      674 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/creds/routers/zyxel/test_telnet_default_creds.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.436768 routersploit-3.4.2/tests/encoders/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.438180 routersploit-3.4.2/tests/encoders/perl/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/perl/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      952 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/perl/test_base64.py
--rw-r--r--   0 user       (501) staff       (20)     1065 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/perl/test_hex.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.439526 routersploit-3.4.2/tests/encoders/php/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/php/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1155 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/php/test_base64.py
--rw-r--r--   0 user       (501) staff       (20)     1325 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/php/test_hex.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.440533 routersploit-3.4.2/tests/encoders/python/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/python/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1154 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/python/test_base64.py
--rw-r--r--   0 user       (501) staff       (20)     1325 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/encoders/python/test_hex.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.440933 routersploit-3.4.2/tests/exploits/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.441260 routersploit-3.4.2/tests/exploits/cameras/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.441816 routersploit-3.4.2/tests/exploits/cameras/avigilon/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/avigilon/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1321 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/avigilon/test_videoiq_camera_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.442831 routersploit-3.4.2/tests/exploits/cameras/brickcom/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/brickcom/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1638 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/brickcom/test_corp_network_cameras_conf_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1382 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/brickcom/test_users_cgi_creds_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.443515 routersploit-3.4.2/tests/exploits/cameras/cisco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/cisco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1320 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/cisco/test_video_surv_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.444304 routersploit-3.4.2/tests/exploits/cameras/dlink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/dlink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     6441 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/dlink/test_dcs_930l_932l_auth_bypass.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.445078 routersploit-3.4.2/tests/exploits/cameras/honeywell/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/honeywell/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/honeywell/test_hicc_1100pt_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.445761 routersploit-3.4.2/tests/exploits/cameras/jovision/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/jovision/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      935 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/jovision/test_jovision_camera_credential_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.447299 routersploit-3.4.2/tests/exploits/cameras/multi/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/multi/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/multi/test_dvr_creds_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     2489 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/multi/test_jvc_vanderbilt_honeywell_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     1088 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/multi/test_netwave_ip_camera_information_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.448127 routersploit-3.4.2/tests/exploits/cameras/mvpower/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/mvpower/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      839 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/mvpower/test_dvr_jaws_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.448897 routersploit-3.4.2/tests/exploits/cameras/siemens/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/siemens/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      543 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/siemens/test_cvms2025_credentials_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.449617 routersploit-3.4.2/tests/exploits/cameras/xiongmai/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/xiongmai/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      602 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/cameras/xiongmai/test_uc_httpd_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.449997 routersploit-3.4.2/tests/exploits/misc/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/misc/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.450568 routersploit-3.4.2/tests/exploits/misc/miele/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/misc/miele/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1332 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/misc/miele/test_pg8528_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.451221 routersploit-3.4.2/tests/exploits/misc/wepresent/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/misc/wepresent/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      703 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/misc/wepresent/test_wipg1000_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.451581 routersploit-3.4.2/tests/exploits/routers/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.453070 routersploit-3.4.2/tests/exploits/routers/2wire/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/2wire/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1456 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/2wire/test_4011g_5012nv_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)      893 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/2wire/test_gateway_auth_bypass.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.483990 routersploit-3.4.2/tests/exploits/routers/3com/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/3com/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      836 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/3com/test_ap8760_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      732 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/3com/test_imc_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      747 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/3com/test_imc_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)      732 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/3com/test_officeconnect_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      814 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/3com/test_officeconnect_rce.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.485484 routersploit-3.4.2/tests/exploits/routers/asmax/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/asmax/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      654 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/asmax/test_ar_1004g_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1369 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/asmax/test_ar_804_gu_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.487802 routersploit-3.4.2/tests/exploits/routers/asus/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/asus/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2930 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/asus/test_asuswrt_lan_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2398 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/asus/test_infosvr_backdoor_rce.py
--rw-r--r--   0 user       (501) staff       (20)      580 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/asus/test_rt_n16_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.491579 routersploit-3.4.2/tests/exploits/routers/belkin/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/belkin/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      542 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/belkin/test_auth_bypass.py
--rw-r--r--   0 user       (501) staff       (20)      567 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/belkin/test_g_n150_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      738 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/belkin/test_g_plus_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1303 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/belkin/test_n150_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)      763 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/belkin/test_n750_rce.py
--rw-r--r--   0 user       (501) staff       (20)      701 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/belkin/test_play_mac_prce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.492332 routersploit-3.4.2/tests/exploits/routers/bhu/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/bhu/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      833 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/bhu/test_bhu_urouter_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.494491 routersploit-3.4.2/tests/exploits/routers/billion/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/billion/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      650 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/billion/test_billion_5200w_rce.py
--rw-r--r--   0 user       (501) staff       (20)      679 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/billion/test_billion_7700n4_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.498875 routersploit-3.4.2/tests/exploits/routers/cisco/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/cisco/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      539 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/cisco/test_dpc2420_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      679 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/cisco/test_firepower_management60_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)      757 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/cisco/test_firepower_management60_rce.py
--rw-r--r--   0 user       (501) staff       (20)      653 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/cisco/test_ios_http_authorization_bypass.py
--rw-r--r--   0 user       (501) staff       (20)      556 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/cisco/test_secure_acs_bypass.py
--rw-r--r--   0 user       (501) staff       (20)      546 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/cisco/test_ucm_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      768 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/cisco/test_ucs_manager_rce.py
--rw-r--r--   0 user       (501) staff       (20)     1322 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/cisco/test_unified_multi_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.499537 routersploit-3.4.2/tests/exploits/routers/comtrend/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/comtrend/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      631 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/comtrend/test_ct_5361t_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.510075 routersploit-3.4.2/tests/exploits/routers/dlink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      757 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dcs_930l_auth_rce.py
--rw-r--r--   0 user       (501) staff       (20)      600 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_300_320_600_615_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      575 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_300_320_615_auth_bypass.py
--rw-r--r--   0 user       (501) staff       (20)      747 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_300_600_rce.py
--rw-r--r--   0 user       (501) staff       (20)      838 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_300_645_815_upnp_rce.py
--rw-r--r--   0 user       (501) staff       (20)      639 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_645_815_rce.py
--rw-r--r--   0 user       (501) staff       (20)     2021 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_645_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      518 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_815_850l_rce.py
--rw-r--r--   0 user       (501) staff       (20)     1373 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_825_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)     1624 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_850l_creds_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1734 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_8xx_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      919 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dns_320l_327l_rce.py
--rw-r--r--   0 user       (501) staff       (20)     1304 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dsl_2730_2750_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)      604 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dsl_2730b_2780b_526b_dns_change.py
--rw-r--r--   0 user       (501) staff       (20)      583 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dsl_2750b_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1117 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dsl_2750b_rce.py
--rw-r--r--   0 user       (501) staff       (20)      751 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dsp_w110_rce.py
--rw-r--r--   0 user       (501) staff       (20)     1312 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dvg_n5402sp_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)      582 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dwl_3200ap_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1019 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dwr_932_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      624 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_dwr_932b_backdoor.py
--rw-r--r--   0 user       (501) staff       (20)      766 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_multi_hedwig_cgi_exec.py
--rw-r--r--   0 user       (501) staff       (20)      667 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/dlink/test_multi_hnap_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.512443 routersploit-3.4.2/tests/exploits/routers/huawei/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/huawei/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1157 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/huawei/test_e5331_mifi_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     5344 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/huawei/test_hg520_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      576 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/huawei/test_hg530_hg520b_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      631 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/huawei/test_hg866_password_change.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.513756 routersploit-3.4.2/tests/exploits/routers/ipfire/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/ipfire/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      901 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/ipfire/test_ipfire_proxy_rce.py
--rw-r--r--   0 user       (501) staff       (20)      898 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/ipfire/test_ipfire_shellshock.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.516176 routersploit-3.4.2/tests/exploits/routers/linksys/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/linksys/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      968 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/linksys/test_1500_2500_rce.py
--rw-r--r--   0 user       (501) staff       (20)     1629 2024-04-14 11:08:48.000000 routersploit-3.4.2/tests/exploits/routers/linksys/test_eseries_themoon_rce.py
--rw-r--r--   0 user       (501) staff       (20)      549 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/linksys/test_smartwifi_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      783 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/linksys/test_wap54gv3_rce.py
--rw-r--r--   0 user       (501) staff       (20)      750 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/linksys/test_wrt100_110_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.516837 routersploit-3.4.2/tests/exploits/routers/mikrotik/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/mikrotik/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3375 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/mikrotik/test_winbox_auth_bypass_creds_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.517480 routersploit-3.4.2/tests/exploits/routers/movistar/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/movistar/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      762 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/movistar/test_adsl_router_bhs_rta_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.519916 routersploit-3.4.2/tests/exploits/routers/multi/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/multi/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2076 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/multi/test_gpon_home_gateway_rce.py
--rw-r--r--   0 user       (501) staff       (20)      695 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/multi/test_misfortune_cookie.py
--rw-r--r--   0 user       (501) staff       (20)    22373 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/multi/test_rom0.py
--rw-r--r--   0 user       (501) staff       (20)      878 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/multi/test_tcp_32764_info_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)     1883 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/multi/test_tcp_32764_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.520659 routersploit-3.4.2/tests/exploits/routers/netcore/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netcore/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1108 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netcore/test_udp_53413_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.524883 routersploit-3.4.2/tests/exploits/routers/netgear/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netgear/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      892 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netgear/test_dgn2200_ping_cgi_rce.py
--rw-r--r--   0 user       (501) staff       (20)      830 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netgear/test_jnr1010_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)      966 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netgear/test_n300_auth_bypass.py
--rw-r--r--   0 user       (501) staff       (20)     3288 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netgear/test_netgear_multi_rce.py
--rw-r--r--   0 user       (501) staff       (20)      778 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netgear/test_prosafe_rce.py
--rw-r--r--   0 user       (501) staff       (20)      791 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netgear/test_r7000_r6400_rce.py
--rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netgear/test_wnr500_612v3_jnr1010_2010_path_traversal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.526145 routersploit-3.4.2/tests/exploits/routers/netsys/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netsys/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1838 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/netsys/test_multi_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.527256 routersploit-3.4.2/tests/exploits/routers/shuttle/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/shuttle/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      722 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/shuttle/test_915wm_dns_change.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.529541 routersploit-3.4.2/tests/exploits/routers/technicolor/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/technicolor/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      601 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/technicolor/test_dwg855_authbypass.py
--rw-r--r--   0 user       (501) staff       (20)      569 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/technicolor/test_tc7200_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/technicolor/test_tc7200_password_disclosure_v2.py
--rw-r--r--   0 user       (501) staff       (20)      479 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/technicolor/test_tg784_authbypass.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.530357 routersploit-3.4.2/tests/exploits/routers/thomson/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/thomson/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      560 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/thomson/test_twg850_password_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.532172 routersploit-3.4.2/tests/exploits/routers/tplink/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/tplink/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      655 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/tplink/test_archer_c2_c20i_rce.py
--rw-r--r--   0 user       (501) staff       (20)      917 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/tplink/test_wdr740nd_wdr740n_backdoor.py
--rw-r--r--   0 user       (501) staff       (20)      875 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/tplink/test_wdr740nd_wdr740n_path_traversal.py
--rw-r--r--   0 user       (501) staff       (20)      690 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/tplink/test_wdr842nd_wdr842n_configure_disclosure.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.533521 routersploit-3.4.2/tests/exploits/routers/zte/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zte/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      831 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zte/test_f460_f660_backdoor.py
--rw-r--r--   0 user       (501) staff       (20)     3803 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zte/test_zxhn_h108n_wifi_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      872 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zte/test_zxv10_rce.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.535495 routersploit-3.4.2/tests/exploits/routers/zyxel/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zyxel/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      735 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zyxel/test_d1000_rce.py
--rw-r--r--   0 user       (501) staff       (20)      582 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zyxel/test_d1000_wifi_password_disclosure.py
--rw-r--r--   0 user       (501) staff       (20)      673 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zyxel/test_p660hn_t_v1_rce.py
--rw-r--r--   0 user       (501) staff       (20)      757 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zyxel/test_p660hn_t_v2_rce.py
--rw-r--r--   0 user       (501) staff       (20)      656 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/exploits/routers/zyxel/test_zywall_usg_extract_hashes.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.535848 routersploit-3.4.2/tests/generic/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/generic/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.536119 routersploit-3.4.2/tests/payloads/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.537168 routersploit-3.4.2/tests/payloads/armle/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/armle/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3151 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/armle/test_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     1516 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/armle/test_reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.543266 routersploit-3.4.2/tests/payloads/cmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      396 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_awk_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      396 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_awk_bind_udp.py
--rw-r--r--   0 user       (501) staff       (20)      471 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_awk_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      405 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_bash_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      327 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_netcat_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      398 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_netcat_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_perl_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      694 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_perl_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      705 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_php_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      557 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_php_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      707 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_python_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      715 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_python_bind_udp.py
--rw-r--r--   0 user       (501) staff       (20)      691 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_python_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      699 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/cmd/test_python_reverse_udp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.544365 routersploit-3.4.2/tests/payloads/mipsbe/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/mipsbe/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2908 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/mipsbe/test_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     2649 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/mipsbe/test_reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.545417 routersploit-3.4.2/tests/payloads/mipsle/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/mipsle/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2908 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/mipsle/test_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     2649 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/mipsle/test_reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.546435 routersploit-3.4.2/tests/payloads/php/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/php/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1218 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/php/test_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/php/test_reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.548267 routersploit-3.4.2/tests/payloads/python/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/python/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1216 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/python/test_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     1198 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/python/test_bind_udp.py
--rw-r--r--   0 user       (501) staff       (20)     1126 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/python/test_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     1168 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/python/test_reverse_udp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.549376 routersploit-3.4.2/tests/payloads/x64/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/x64/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1721 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/x64/test_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     1678 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/x64/test_reverse_tcp.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-14 13:58:44.550458 routersploit-3.4.2/tests/payloads/x86/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/x86/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1433 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/x86/test_bind_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     1402 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/payloads/x86/test_reverse_tcp.py
--rw-r--r--   0 user       (501) staff       (20)     1758 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/test_exploit_scenarios.py
--rw-r--r--   0 user       (501) staff       (20)     2449 2024-04-08 16:47:10.000000 routersploit-3.4.2/tests/test_module_info.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.630016 routersploit-3.4.3/
+-rw-r--r--   0 user       (501) staff       (20)     1844 2024-04-08 16:47:10.000000 routersploit-3.4.3/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      175 2024-04-08 16:47:10.000000 routersploit-3.4.3/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     4519 2024-05-19 17:59:08.629218 routersploit-3.4.3/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3515 2024-04-08 16:47:10.000000 routersploit-3.4.3/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.030715 routersploit-3.4.3/routersploit/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.033862 routersploit-3.4.3/routersploit/core/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.034879 routersploit-3.4.3/routersploit/core/bluetooth/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/bluetooth/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.036033 routersploit-3.4.3/routersploit/core/bluetooth/btle/
+-rw-r--r--   0 user       (501) staff       (20)      173 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/bluetooth/btle/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    12363 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/bluetooth/btle/btle_device.py
+-rw-r--r--   0 user       (501) staff       (20)     2083 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/bluetooth/btle/btle_scanner.py
+-rw-r--r--   0 user       (501) staff       (20)     1403 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/bluetooth/btle_client.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.051819 routersploit-3.4.3/routersploit/core/exploit/
+-rw-r--r--   0 user       (501) staff       (20)      826 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/exploit/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/exploit/encoders.py
+-rw-r--r--   0 user       (501) staff       (20)      263 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/exploit/exceptions.py
+-rw-r--r--   0 user       (501) staff       (20)     6511 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/exploit/exploit.py
+-rw-r--r--   0 user       (501) staff       (20)     5513 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/exploit/option.py
+-rw-r--r--   0 user       (501) staff       (20)     8713 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/exploit/payloads.py
+-rw-r--r--   0 user       (501) staff       (20)     5522 2024-04-14 11:08:48.000000 routersploit-3.4.3/routersploit/core/exploit/printer.py
+-rw-r--r--   0 user       (501) staff       (20)    13490 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/exploit/shell.py
+-rw-r--r--   0 user       (501) staff       (20)    10620 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/exploit/utils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.052822 routersploit-3.4.3/routersploit/core/ftp/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/ftp/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4359 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/ftp/ftp_client.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.053996 routersploit-3.4.3/routersploit/core/http/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/http/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2830 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/http/http_client.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.055036 routersploit-3.4.3/routersploit/core/snmp/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/snmp/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2893 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/snmp/snmp_client.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.056372 routersploit-3.4.3/routersploit/core/ssh/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/ssh/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    11443 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/ssh/ssh_client.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.057227 routersploit-3.4.3/routersploit/core/tcp/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/tcp/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4676 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/tcp/tcp_client.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.057992 routersploit-3.4.3/routersploit/core/telnet/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/telnet/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     6005 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/telnet/telnet_client.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.058745 routersploit-3.4.3/routersploit/core/udp/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/udp/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3337 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/core/udp/udp_client.py
+-rw-r--r--   0 user       (501) staff       (20)    25107 2024-05-19 17:52:42.000000 routersploit-3.4.3/routersploit/interpreter.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.059146 routersploit-3.4.3/routersploit/libs/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/libs/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.059770 routersploit-3.4.3/routersploit/libs/apiros/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/libs/apiros/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     9779 2024-04-10 18:54:42.000000 routersploit-3.4.3/routersploit/libs/apiros/apiros_client.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.060509 routersploit-3.4.3/routersploit/libs/lzs/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/libs/lzs/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3842 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/libs/lzs/lzs.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.060893 routersploit-3.4.3/routersploit/modules/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.061182 routersploit-3.4.3/routersploit/modules/creds/
+-rw-r--r--   0 user       (501) staff       (20)       20 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.061664 routersploit-3.4.3/routersploit/modules/creds/cameras/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.063499 routersploit-3.4.3/routersploit/modules/creds/cameras/acti/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/acti/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      906 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/acti/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      907 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/acti/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      925 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/acti/telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)     3079 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/acti/webinterface_http_form_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.067455 routersploit-3.4.3/routersploit/modules/creds/cameras/american_dynamics/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/american_dynamics/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      895 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/american_dynamics/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      894 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/american_dynamics/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      896 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/american_dynamics/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.068918 routersploit-3.4.3/routersploit/modules/creds/cameras/arecont/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/arecont/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/arecont/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/arecont/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/arecont/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.070279 routersploit-3.4.3/routersploit/modules/creds/cameras/avigilon/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/avigilon/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/avigilon/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      870 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/avigilon/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      888 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/avigilon/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.071622 routersploit-3.4.3/routersploit/modules/creds/cameras/avtech/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/avtech/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/avtech/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/avtech/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      867 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/avtech/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.073316 routersploit-3.4.3/routersploit/modules/creds/cameras/axis/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/axis/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/axis/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/axis/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      872 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/axis/telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      915 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/axis/webinterface_http_auth_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.075227 routersploit-3.4.3/routersploit/modules/creds/cameras/basler/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/basler/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/basler/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/basler/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      866 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/basler/telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)     3003 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/basler/webinterface_http_form_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.076916 routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      854 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      855 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      866 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      946 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/webinterface_http_auth_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.078767 routersploit-3.4.3/routersploit/modules/creds/cameras/canon/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/canon/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      846 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/canon/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      846 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/canon/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/canon/telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      965 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/canon/webinterface_http_auth_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.084141 routersploit-3.4.3/routersploit/modules/creds/cameras/cisco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/cisco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      755 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/cisco/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      823 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/cisco/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      840 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/cisco/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.085550 routersploit-3.4.3/routersploit/modules/creds/cameras/dlink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/dlink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      848 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/dlink/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      825 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/dlink/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      866 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/dlink/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.087255 routersploit-3.4.3/routersploit/modules/creds/cameras/geovision/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/geovision/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      858 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/geovision/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/geovision/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/geovision/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.089034 routersploit-3.4.3/routersploit/modules/creds/cameras/grandstream/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/grandstream/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/grandstream/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/grandstream/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/grandstream/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.090390 routersploit-3.4.3/routersploit/modules/creds/cameras/hikvision/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/hikvision/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      847 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/hikvision/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      858 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/hikvision/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      877 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/hikvision/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.091687 routersploit-3.4.3/routersploit/modules/creds/cameras/honeywell/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/honeywell/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/honeywell/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      858 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/honeywell/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/honeywell/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.092999 routersploit-3.4.3/routersploit/modules/creds/cameras/iqinvision/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/iqinvision/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      861 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/iqinvision/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      861 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/iqinvision/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      878 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/iqinvision/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.094275 routersploit-3.4.3/routersploit/modules/creds/cameras/jvc/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/jvc/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      838 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/jvc/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      838 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/jvc/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/jvc/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.095549 routersploit-3.4.3/routersploit/modules/creds/cameras/mobotix/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/mobotix/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/mobotix/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/mobotix/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      870 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/mobotix/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.096785 routersploit-3.4.3/routersploit/modules/creds/cameras/samsung/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/samsung/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      875 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/samsung/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/samsung/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      894 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/samsung/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.098061 routersploit-3.4.3/routersploit/modules/creds/cameras/sentry360/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/sentry360/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/sentry360/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/sentry360/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      874 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/sentry360/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.099503 routersploit-3.4.3/routersploit/modules/creds/cameras/siemens/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/siemens/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/siemens/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/siemens/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      870 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/siemens/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.100873 routersploit-3.4.3/routersploit/modules/creds/cameras/speco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/speco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      845 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/speco/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      845 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/speco/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      862 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/speco/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.102092 routersploit-3.4.3/routersploit/modules/creds/cameras/stardot/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/stardot/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/stardot/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/stardot/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/stardot/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.103292 routersploit-3.4.3/routersploit/modules/creds/cameras/vacron/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/vacron/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/vacron/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/vacron/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      869 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/vacron/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.118837 routersploit-3.4.3/routersploit/modules/creds/cameras/videoiq/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/videoiq/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      863 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/videoiq/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      862 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/videoiq/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      880 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/cameras/videoiq/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.124387 routersploit-3.4.3/routersploit/modules/creds/generic/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3118 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/ftp_bruteforce.py
+-rw-r--r--   0 user       (501) staff       (20)     2968 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/ftp_default.py
+-rw-r--r--   0 user       (501) staff       (20)     4427 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/http_basic_digest_bruteforce.py
+-rw-r--r--   0 user       (501) staff       (20)     4312 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/http_basic_digest_default.py
+-rw-r--r--   0 user       (501) staff       (20)     2511 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/snmp_bruteforce.py
+-rw-r--r--   0 user       (501) staff       (20)     2920 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/ssh_bruteforce.py
+-rw-r--r--   0 user       (501) staff       (20)     2784 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/ssh_default.py
+-rw-r--r--   0 user       (501) staff       (20)     2990 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/telnet_bruteforce.py
+-rw-r--r--   0 user       (501) staff       (20)     2879 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/generic/telnet_default.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.124786 routersploit-3.4.3/routersploit/modules/creds/printers/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/printers/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.125101 routersploit-3.4.3/routersploit/modules/creds/routers/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.126685 routersploit-3.4.3/routersploit/modules/creds/routers/2wire/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/2wire/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      915 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/2wire/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      915 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/2wire/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      930 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/2wire/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.128252 routersploit-3.4.3/routersploit/modules/creds/routers/3com/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/3com/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      912 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/3com/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      912 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/3com/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      927 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/3com/telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.130297 routersploit-3.4.3/routersploit/modules/creds/routers/asmax/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/asmax/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      873 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/asmax/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      873 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/asmax/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      888 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/asmax/telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      977 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/asmax/webinterface_http_auth_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.131685 routersploit-3.4.3/routersploit/modules/creds/routers/asus/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/asus/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/asus/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/asus/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      899 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/asus/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.133372 routersploit-3.4.3/routersploit/modules/creds/routers/belkin/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/belkin/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/belkin/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/belkin/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      883 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/belkin/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.134807 routersploit-3.4.3/routersploit/modules/creds/routers/bhu/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/bhu/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/bhu/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/bhu/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      860 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/bhu/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.136178 routersploit-3.4.3/routersploit/modules/creds/routers/billion/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/billion/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      852 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/billion/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/billion/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/billion/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.151596 routersploit-3.4.3/routersploit/modules/creds/routers/cisco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/cisco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      847 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/cisco/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      847 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/cisco/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      866 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/cisco/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.153810 routersploit-3.4.3/routersploit/modules/creds/routers/comtrend/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/comtrend/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      856 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/comtrend/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      856 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/comtrend/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      875 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/comtrend/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.156116 routersploit-3.4.3/routersploit/modules/creds/routers/dlink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/dlink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/dlink/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      881 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/dlink/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      899 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/dlink/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.157831 routersploit-3.4.3/routersploit/modules/creds/routers/fortinet/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/fortinet/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      892 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/fortinet/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      892 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/fortinet/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      910 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/fortinet/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.159337 routersploit-3.4.3/routersploit/modules/creds/routers/huawei/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/huawei/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      965 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/huawei/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      965 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/huawei/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      983 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/huawei/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.160903 routersploit-3.4.3/routersploit/modules/creds/routers/ipfire/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/ipfire/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      867 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/ipfire/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      867 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/ipfire/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      885 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/ipfire/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.162411 routersploit-3.4.3/routersploit/modules/creds/routers/juniper/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/juniper/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      901 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/juniper/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      899 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/juniper/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      919 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/juniper/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.164034 routersploit-3.4.3/routersploit/modules/creds/routers/linksys/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/linksys/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/linksys/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/linksys/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      905 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/linksys/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.166012 routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3970 2024-04-10 18:54:42.000000 routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/api_ros_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      854 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      854 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      872 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.167452 routersploit-3.4.3/routersploit/modules/creds/routers/movistar/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/movistar/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/movistar/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      865 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/movistar/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      883 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/movistar/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.168816 routersploit-3.4.3/routersploit/modules/creds/routers/netcore/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netcore/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netcore/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      864 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netcore/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      882 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netcore/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.170143 routersploit-3.4.3/routersploit/modules/creds/routers/netgear/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netgear/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netgear/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netgear/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      889 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netgear/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.185181 routersploit-3.4.3/routersploit/modules/creds/routers/netsys/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netsys/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netsys/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      850 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netsys/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      862 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/netsys/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.186938 routersploit-3.4.3/routersploit/modules/creds/routers/pfsense/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/pfsense/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      848 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/pfsense/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)     2144 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/pfsense/webinterface_http_form_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.189322 routersploit-3.4.3/routersploit/modules/creds/routers/technicolor/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/technicolor/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      906 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/technicolor/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      906 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/technicolor/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      924 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/technicolor/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.191170 routersploit-3.4.3/routersploit/modules/creds/routers/thomson/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/thomson/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      868 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/thomson/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      868 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/thomson/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      886 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/thomson/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.193190 routersploit-3.4.3/routersploit/modules/creds/routers/tplink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/tplink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/tplink/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/tplink/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      871 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/tplink/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.194963 routersploit-3.4.3/routersploit/modules/creds/routers/ubiquiti/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/ubiquiti/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/ubiquiti/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      876 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/ubiquiti/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      894 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/ubiquiti/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.196543 routersploit-3.4.3/routersploit/modules/creds/routers/zte/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/zte/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      896 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/zte/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      896 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/zte/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      914 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/zte/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.198058 routersploit-3.4.3/routersploit/modules/creds/routers/zyxel/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/zyxel/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/zyxel/ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/zyxel/ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      905 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/creds/routers/zyxel/telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.198452 routersploit-3.4.3/routersploit/modules/encoders/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/encoders/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.199713 routersploit-3.4.3/routersploit/modules/encoders/php/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/encoders/php/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      630 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/encoders/php/base64.py
+-rw-r--r--   0 user       (501) staff       (20)      616 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/encoders/php/hex.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.200893 routersploit-3.4.3/routersploit/modules/encoders/python/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/encoders/python/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      640 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/encoders/python/base64.py
+-rw-r--r--   0 user       (501) staff       (20)      583 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/encoders/python/hex.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.201293 routersploit-3.4.3/routersploit/modules/exploits/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.201604 routersploit-3.4.3/routersploit/modules/exploits/cameras/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.202257 routersploit-3.4.3/routersploit/modules/exploits/cameras/avigilon/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/avigilon/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2282 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/avigilon/videoiq_camera_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.203426 routersploit-3.4.3/routersploit/modules/exploits/cameras/brickcom/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/brickcom/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3907 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/brickcom/corp_network_cameras_conf_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2342 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/brickcom/users_cgi_creds_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.216627 routersploit-3.4.3/routersploit/modules/exploits/cameras/cisco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/cisco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2160 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/cisco/video_surv_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.217412 routersploit-3.4.3/routersploit/modules/exploits/cameras/dlink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/dlink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3754 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/dlink/dcs_930l_932l_auth_bypass.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.218598 routersploit-3.4.3/routersploit/modules/exploits/cameras/grandstream/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/grandstream/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2200 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/grandstream/gxv3611hd_ip_camera_backdoor.py
+-rw-r--r--   0 user       (501) staff       (20)     2388 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/grandstream/gxv3611hd_ip_camera_sqli.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.219412 routersploit-3.4.3/routersploit/modules/exploits/cameras/honeywell/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/honeywell/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1500 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/honeywell/hicc_1100pt_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.220465 routersploit-3.4.3/routersploit/modules/exploits/cameras/jovision/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/jovision/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2820 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/jovision/jovision_credentials_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.223488 routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/
+-rw-r--r--   0 user       (501) staff       (20)    41546 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/P2P_wificam_credential_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)    42581 2024-04-09 15:50:17.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/P2P_wificam_rce.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2137 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/dvr_creds_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2555 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/jvc_vanderbilt_honeywell_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     2874 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/netwave_ip_camera_information_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.224204 routersploit-3.4.3/routersploit/modules/exploits/cameras/mvpower/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/mvpower/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1978 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/mvpower/dvr_jaws_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.224997 routersploit-3.4.3/routersploit/modules/exploits/cameras/siemens/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/siemens/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1634 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/siemens/cvms2025_credentials_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.225715 routersploit-3.4.3/routersploit/modules/exploits/cameras/xiongmai/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/xiongmai/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2076 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/cameras/xiongmai/uc_httpd_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.227298 routersploit-3.4.3/routersploit/modules/exploits/generic/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/generic/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    14911 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/generic/heartbleed.py
+-rw-r--r--   0 user       (501) staff       (20)     2982 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/generic/shellshock.py
+-rw-r--r--   0 user       (501) staff       (20)     4092 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/generic/ssh_auth_keys.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.227702 routersploit-3.4.3/routersploit/modules/exploits/misc/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/misc/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.228367 routersploit-3.4.3/routersploit/modules/exploits/misc/asus/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/misc/asus/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1667 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/misc/asus/b1m_projector_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.229084 routersploit-3.4.3/routersploit/modules/exploits/misc/miele/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/misc/miele/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1962 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/misc/miele/pg8528_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.229763 routersploit-3.4.3/routersploit/modules/exploits/misc/wepresent/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/misc/wepresent/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1842 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/misc/wepresent/wipg1000_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.230134 routersploit-3.4.3/routersploit/modules/exploits/routers/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.231102 routersploit-3.4.3/routersploit/modules/exploits/routers/2wire/
+-rw-r--r--   0 user       (501) staff       (20)     2601 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/2wire/4011g_5012nv_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/2wire/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1982 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/2wire/gateway_auth_bypass.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.233402 routersploit-3.4.3/routersploit/modules/exploits/routers/3com/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/3com/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2033 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/3com/ap8760_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2293 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/3com/imc_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2244 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/3com/imc_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     2233 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/3com/officeconnect_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2013 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/3com/officeconnect_rce.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.234425 routersploit-3.4.3/routersploit/modules/exploits/routers/asmax/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/asmax/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2087 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/asmax/ar_1004g_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2009 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/asmax/ar_804_gu_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.235727 routersploit-3.4.3/routersploit/modules/exploits/routers/asus/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/asus/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3476 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/asus/asuswrt_lan_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     3353 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/asus/infosvr_backdoor_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2052 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/asus/rt_n16_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.251127 routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2254 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/auth_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)     1968 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/g_n150_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2430 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/g_plus_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2080 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/n150_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     1902 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/n750_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     3737 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/play_max_prce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.251780 routersploit-3.4.3/routersploit/modules/exploits/routers/bhu/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/bhu/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3099 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/bhu/bhu_urouter_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.252826 routersploit-3.4.3/routersploit/modules/exploits/routers/billion/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/billion/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     5149 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/billion/billion_5200w_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2321 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/billion/billion_7700nr4_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.256704 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     9688 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/catalyst_2960_rocem.py
+-rw-r--r--   0 user       (501) staff       (20)     1718 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/dpc2420_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     3554 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/firepower_management60_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     5241 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/firepower_management60_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2323 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/ios_http_authorization_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)     3768 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/secure_acs_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)     1932 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/ucm_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2042 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/ucs_manager_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2863 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/unified_multi_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.257312 routersploit-3.4.3/routersploit/modules/exploits/routers/comtrend/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/comtrend/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2598 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/comtrend/ct_5361t_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.265666 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2585 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dcs_930l_auth_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     5438 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dgs_1510_add_user.py
+-rw-r--r--   0 user       (501) staff       (20)     2117 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_300_320_600_615_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2408 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_300_320_615_auth_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)     1948 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_300_600_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2451 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_300_645_815_upnp_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2469 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_645_815_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2251 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_645_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1738 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_815_850l_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     3044 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_825_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     2237 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_850l_creds_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2148 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_8xx_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2286 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dns_320l_327l_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     1959 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2640b_dns_change.py
+-rw-r--r--   0 user       (501) staff       (20)     2171 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2730_2750_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     2003 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2730b_2780b_526b_dns_change.py
+-rw-r--r--   0 user       (501) staff       (20)     1861 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2740r_dns_change.py
+-rw-r--r--   0 user       (501) staff       (20)     2133 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2750b_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1722 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2750b_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2000 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsp_w110_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2693 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dvg_n5402sp_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     2935 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dwl_3200ap_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2650 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dwr_932_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1654 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dwr_932b_backdoor.py
+-rw-r--r--   0 user       (501) staff       (20)     2826 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/multi_hedwig_cgi_exec.py
+-rw-r--r--   0 user       (501) staff       (20)     2701 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/multi_hnap_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.266566 routersploit-3.4.3/routersploit/modules/exploits/routers/fortinet/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/fortinet/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3412 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/fortinet/fortigate_os_backdoor.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.268444 routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2304 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/e5331_mifi_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     6409 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/hg520_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     3157 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/hg530_hg520b_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2379 2024-04-14 11:08:48.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/hg532_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2142 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/hg866_password_change.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.269643 routersploit-3.4.3/routersploit/modules/exploits/routers/ipfire/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/ipfire/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2732 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/ipfire/ipfire_oinkcode_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2583 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/ipfire/ipfire_proxy_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2615 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/ipfire/ipfire_shellshock.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.284940 routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/
+-rw-r--r--   0 user       (501) staff       (20)     2747 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/1500_2500_rce.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3661 2024-05-19 16:21:20.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/eseries_themoon_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2766 2024-05-19 16:21:20.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/smartwifi_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1853 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/wap54gv3_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2681 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/wrt100_110_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.286005 routersploit-3.4.3/routersploit/modules/exploits/routers/mikrotik/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/mikrotik/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4161 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/mikrotik/routeros_jailbreak.py
+-rw-r--r--   0 user       (501) staff       (20)     4260 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/mikrotik/winbox_auth_bypass_creds_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.286736 routersploit-3.4.3/routersploit/modules/exploits/routers/movistar/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/movistar/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1964 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/movistar/adsl_router_bhs_rta_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.289723 routersploit-3.4.3/routersploit/modules/exploits/routers/multi/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/multi/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2309 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/multi/gpon_home_gateway_rce.py
+-rw-r--r--   0 user       (501) staff       (20)    17579 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/multi/misfortune_cookie.py
+-rw-r--r--   0 user       (501) staff       (20)     3372 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/multi/rom0.py
+-rw-r--r--   0 user       (501) staff       (20)     3610 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/multi/tcp_32764_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     3145 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/multi/tcp_32764_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.290323 routersploit-3.4.3/routersploit/modules/exploits/routers/netcore/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netcore/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2133 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netcore/udp_53413_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.294787 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1714 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/dgn2200_dnslookup_cgi_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/dgn2200_ping_cgi_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2301 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/jnr1010_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     5350 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/multi_password_disclosure-2017-5521.py
+-rw-r--r--   0 user       (501) staff       (20)     3365 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/multi_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2461 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/n300_auth_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)     2281 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/prosafe_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2356 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/r7000_r6400_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2050 2024-05-19 17:52:13.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/rax30_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2449 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/wnr500_612v3_jnr1010_2010_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.295376 routersploit-3.4.3/routersploit/modules/exploits/routers/netsys/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netsys/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2656 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/netsys/multi_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.296031 routersploit-3.4.3/routersploit/modules/exploits/routers/shuttle/
+-rw-r--r--   0 user       (501) staff       (20)     1907 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/shuttle/915wm_dns_change.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/shuttle/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.297520 routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3360 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/dwg855_authbypass.py
+-rw-r--r--   0 user       (501) staff       (20)     1713 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/tc7200_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2875 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/tc7200_password_disclosure_v2.py
+-rw-r--r--   0 user       (501) staff       (20)     2926 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/tg784_authbypass.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.298392 routersploit-3.4.3/routersploit/modules/exploits/routers/thomson/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/thomson/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2449 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/thomson/twg849_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1712 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/thomson/twg850_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.300697 routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3280 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/archer_c2_c20i_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     4631 2024-04-14 11:13:53.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/archer_c9_admin_password_reset.py
+-rw-r--r--   0 user       (501) staff       (20)     2212 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/wdr740nd_wdr740n_backdoor.py
+-rw-r--r--   0 user       (501) staff       (20)     2310 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/wdr740nd_wdr740n_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     4315 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/wdr842nd_wdr842n_configure_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.301351 routersploit-3.4.3/routersploit/modules/exploits/routers/ubiquiti/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/ubiquiti/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3802 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/ubiquiti/airos_6_x.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.302655 routersploit-3.4.3/routersploit/modules/exploits/routers/zte/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zte/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2133 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zte/f460_f660_backdoor.py
+-rw-r--r--   0 user       (501) staff       (20)     2191 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zte/zxhn_h108n_wifi_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     5245 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zte/zxv10_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.317856 routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2897 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/d1000_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2421 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/d1000_wifi_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2158 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/p660hn_t_v1_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2941 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/p660hn_t_v2_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2404 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/zywall_usg_extract_hashes.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.318178 routersploit-3.4.3/routersploit/modules/generic/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/generic/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.319577 routersploit-3.4.3/routersploit/modules/generic/bluetooth/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/generic/bluetooth/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      795 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/generic/bluetooth/btle_enumerate.py
+-rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/generic/bluetooth/btle_scan.py
+-rw-r--r--   0 user       (501) staff       (20)     1102 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/generic/bluetooth/btle_write.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.320272 routersploit-3.4.3/routersploit/modules/generic/upnp/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/generic/upnp/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1795 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/generic/upnp/ssdp_msearch.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.320706 routersploit-3.4.3/routersploit/modules/payloads/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.321692 routersploit-3.4.3/routersploit/modules/payloads/armle/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/armle/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2861 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/armle/bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     1409 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/armle/reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.327046 routersploit-3.4.3/routersploit/modules/payloads/cmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      706 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/awk_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      706 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/awk_bind_udp.py
+-rw-r--r--   0 user       (501) staff       (20)      740 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/awk_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      583 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/bash_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      701 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/netcat_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      758 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/netcat_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      597 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/perl_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      612 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/perl_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      583 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/php_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      598 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/php_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      607 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/python_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      603 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/python_bind_udp.py
+-rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/python_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      612 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/cmd/python_reverse_udp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.328045 routersploit-3.4.3/routersploit/modules/payloads/mipsbe/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/mipsbe/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4812 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/mipsbe/bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     3942 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/mipsbe/reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.329126 routersploit-3.4.3/routersploit/modules/payloads/mipsle/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/mipsle/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4089 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/mipsle/bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     3891 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/mipsle/reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.330054 routersploit-3.4.3/routersploit/modules/payloads/perl/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/perl/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      967 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/perl/bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      985 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/perl/reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.330986 routersploit-3.4.3/routersploit/modules/payloads/php/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/php/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1212 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/php/bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/php/reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.332715 routersploit-3.4.3/routersploit/modules/payloads/python/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/python/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1160 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/python/bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     1159 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/python/bind_udp.py
+-rw-r--r--   0 user       (501) staff       (20)     1042 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/python/reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     1148 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/python/reverse_udp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.333812 routersploit-3.4.3/routersploit/modules/payloads/x64/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/x64/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3368 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/x64/bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     2998 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/x64/reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.334719 routersploit-3.4.3/routersploit/modules/payloads/x86/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/x86/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3211 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/x86/bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     2815 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/payloads/x86/reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.335290 routersploit-3.4.3/routersploit/modules/scanners/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/scanners/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    10271 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/scanners/autopwn.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.335942 routersploit-3.4.3/routersploit/modules/scanners/cameras/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/scanners/cameras/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      427 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/scanners/cameras/camera_scan.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.336517 routersploit-3.4.3/routersploit/modules/scanners/misc/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/scanners/misc/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      431 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/scanners/misc/misc_scan.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.349887 routersploit-3.4.3/routersploit/modules/scanners/routers/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/scanners/routers/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      426 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/modules/scanners/routers/router_scan.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.350463 routersploit-3.4.3/routersploit/resources/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.358108 routersploit-3.4.3/routersploit/resources/ssh_keys/
+-rw-r--r--   0 user       (501) staff       (20)      634 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/array-networks-vapv-vxag.json
+-rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/array-networks-vapv-vxag.key
+-rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/barracuda_load_balancer_vm.json
+-rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/barracuda_load_balancer_vm.key
+-rw-r--r--   0 user       (501) staff       (20)      275 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/ceragon-fibeair-cve-2015-0936.json
+-rw-r--r--   0 user       (501) staff       (20)      887 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/ceragon-fibeair-cve-2015-0936.key
+-rw-r--r--   0 user       (501) staff       (20)      254 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/exagrid-cve-2016-1561.json
+-rw-r--r--   0 user       (501) staff       (20)      883 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/exagrid-cve-2016-1561.key
+-rw-r--r--   0 user       (501) staff       (20)      271 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/f5-bigip-cve-2012-1493.json
+-rw-r--r--   0 user       (501) staff       (20)      883 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/f5-bigip-cve-2012-1493.key
+-rw-r--r--   0 user       (501) staff       (20)      647 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/loadbalancer.org-enterprise-va.json
+-rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/loadbalancer.org-enterprise-va.key
+-rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/monroe-dasdec-cve-2013-0137.json
+-rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/monroe-dasdec-cve-2013-0137.key
+-rw-r--r--   0 user       (501) staff       (20)      634 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/quantum-dxi-v1000.json
+-rw-r--r--   0 user       (501) staff       (20)      668 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/quantum-dxi-v1000.key
+-rw-r--r--   0 user       (501) staff       (20)      457 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/vagrant.json
+-rw-r--r--   0 user       (501) staff       (20)     1675 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/ssh_keys/vagrant.key
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.358478 routersploit-3.4.3/routersploit/resources/vendors/
+-rw-r--r--   0 user       (501) staff       (20)   589907 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/vendors/oui.dat
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.361799 routersploit-3.4.3/routersploit/resources/wordlists/
+-rw-r--r--   0 user       (501) staff       (20)      343 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/wordlists/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     9596 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/wordlists/defaults.txt
+-rw-r--r--   0 user       (501) staff       (20)     5946 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/wordlists/passwords.txt
+-rw-r--r--   0 user       (501) staff       (20)      839 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/wordlists/snmp.txt
+-rw-r--r--   0 user       (501) staff       (20)     2512 2024-04-08 16:47:10.000000 routersploit-3.4.3/routersploit/resources/wordlists/usernames.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.033400 routersploit-3.4.3/routersploit.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     4519 2024-05-19 17:59:07.000000 routersploit-3.4.3/routersploit.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)    53969 2024-05-19 17:59:07.000000 routersploit-3.4.3/routersploit.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-05-19 17:59:07.000000 routersploit-3.4.3/routersploit.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       95 2024-05-19 17:59:07.000000 routersploit-3.4.3/routersploit.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       19 2024-05-19 17:59:07.000000 routersploit-3.4.3/routersploit.egg-info/top_level.txt
+-rwxr-xr-x   0 user       (501) staff       (20)      884 2024-04-08 16:47:10.000000 routersploit-3.4.3/rsf.py
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-05-19 17:59:08.630265 routersploit-3.4.3/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     1507 2024-05-19 17:56:21.000000 routersploit-3.4.3/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.363058 routersploit-3.4.3/tests/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2118 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/conftest.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.363639 routersploit-3.4.3/tests/core/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/core/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     7275 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/core/test_option.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.363998 routersploit-3.4.3/tests/creds/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.364261 routersploit-3.4.3/tests/creds/cameras/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.366037 routersploit-3.4.3/tests/creds/cameras/acti/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/acti/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      663 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/acti/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      639 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/acti/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      672 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/acti/test_telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      988 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/acti/test_webinterface_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.367507 routersploit-3.4.3/tests/creds/cameras/american_dynamics/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/american_dynamics/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/american_dynamics/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/american_dynamics/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      651 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/american_dynamics/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.368800 routersploit-3.4.3/tests/creds/cameras/arecont/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/arecont/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/arecont/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      594 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/arecont/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/arecont/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.370085 routersploit-3.4.3/tests/creds/cameras/avigilon/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/avigilon/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/avigilon/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      613 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/avigilon/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/avigilon/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.384860 routersploit-3.4.3/tests/creds/cameras/avtech/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/avtech/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/avtech/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      593 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/avtech/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      626 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/avtech/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.387084 routersploit-3.4.3/tests/creds/cameras/axis/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/axis/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/axis/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      604 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/axis/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/axis/test_telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)     1182 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/axis/test_webinterface_http_auth_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.389403 routersploit-3.4.3/tests/creds/cameras/basler/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/basler/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/basler/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      593 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/basler/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      626 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/basler/test_telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      751 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/basler/test_webinterface_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.391312 routersploit-3.4.3/tests/creds/cameras/brickcom/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/brickcom/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/brickcom/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      595 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/brickcom/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/brickcom/test_telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)     1162 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/brickcom/test_webinterface_http_auth_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.393221 routersploit-3.4.3/tests/creds/cameras/canon/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/canon/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      616 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/canon/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      592 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/canon/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      625 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/canon/test_telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)     1175 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/canon/test_webinterface_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.394628 routersploit-3.4.3/tests/creds/cameras/cisco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/cisco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      616 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/cisco/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      592 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/cisco/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      625 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/cisco/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.396109 routersploit-3.4.3/tests/creds/cameras/dlink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/dlink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      616 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/dlink/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      592 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/dlink/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      625 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/dlink/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.397592 routersploit-3.4.3/tests/creds/cameras/geovision/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/geovision/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/geovision/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      596 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/geovision/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      629 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/geovision/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.399067 routersploit-3.4.3/tests/creds/cameras/grandstream/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/grandstream/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      622 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/grandstream/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      598 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/grandstream/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      631 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/grandstream/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.400533 routersploit-3.4.3/tests/creds/cameras/hikvision/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/hikvision/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/hikvision/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      597 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/hikvision/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      629 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/hikvision/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.401849 routersploit-3.4.3/tests/creds/cameras/honeywell/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/honeywell/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/honeywell/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      595 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/honeywell/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/honeywell/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.403137 routersploit-3.4.3/tests/creds/cameras/iqinvision/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/iqinvision/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      621 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/iqinvision/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      597 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/iqinvision/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      630 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/iqinvision/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.416622 routersploit-3.4.3/tests/creds/cameras/jvc/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/jvc/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      612 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/jvc/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      588 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/jvc/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      621 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/jvc/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.418545 routersploit-3.4.3/tests/creds/cameras/mobotix/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/mobotix/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/mobotix/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      595 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/mobotix/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/mobotix/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.420670 routersploit-3.4.3/tests/creds/cameras/samsung/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/samsung/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      648 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/samsung/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      624 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/samsung/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      657 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/samsung/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.422324 routersploit-3.4.3/tests/creds/cameras/sentry360/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/sentry360/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/sentry360/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      595 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/sentry360/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/sentry360/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.423996 routersploit-3.4.3/tests/creds/cameras/siemens/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/siemens/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/siemens/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      594 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/siemens/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/siemens/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.425449 routersploit-3.4.3/tests/creds/cameras/speco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/speco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      615 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/speco/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      591 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/speco/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      624 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/speco/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.426845 routersploit-3.4.3/tests/creds/cameras/stardot/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/stardot/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/stardot/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      594 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/stardot/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/stardot/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.428250 routersploit-3.4.3/tests/creds/cameras/vacron/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/vacron/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/vacron/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      593 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/vacron/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      626 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/vacron/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.429617 routersploit-3.4.3/tests/creds/cameras/videoiq/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/videoiq/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/videoiq/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      604 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/videoiq/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/cameras/videoiq/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.429964 routersploit-3.4.3/tests/creds/routers/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.431220 routersploit-3.4.3/tests/creds/routers/2wire/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/2wire/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      749 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/2wire/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      725 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/2wire/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      758 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/2wire/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.432694 routersploit-3.4.3/tests/creds/routers/3com/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/3com/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      748 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/3com/test_3com_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      724 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/3com/test_3com_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      757 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/3com/test_3com_telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.434620 routersploit-3.4.3/tests/creds/routers/asmax/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/asmax/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      649 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/asmax/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      625 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/asmax/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      658 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/asmax/test_telnet_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)     1213 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/asmax/test_webinterface_http_auth_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.435893 routersploit-3.4.3/tests/creds/routers/asus/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/asus/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/asus/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/asus/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      671 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/asus/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.437120 routersploit-3.4.3/tests/creds/routers/belkin/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/belkin/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      636 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/belkin/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      636 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/belkin/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      645 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/belkin/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.452322 routersploit-3.4.3/tests/creds/routers/bhu/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/bhu/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      615 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/bhu/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      615 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/bhu/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      624 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/bhu/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.454455 routersploit-3.4.3/tests/creds/routers/billion/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/billion/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/billion/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      619 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/billion/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      628 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/billion/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.456375 routersploit-3.4.3/tests/creds/routers/cisco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/cisco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/cisco/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      617 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/cisco/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      626 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/cisco/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.458289 routersploit-3.4.3/tests/creds/routers/comtrend/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/comtrend/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/comtrend/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/comtrend/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      629 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/comtrend/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.459852 routersploit-3.4.3/tests/creds/routers/dlink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/dlink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      657 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/dlink/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      657 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/dlink/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      666 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/dlink/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.461307 routersploit-3.4.3/tests/creds/routers/fortinet/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/fortinet/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/fortinet/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/fortinet/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      671 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/fortinet/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.462753 routersploit-3.4.3/tests/creds/routers/huawei/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/huawei/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      758 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/huawei/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      758 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/huawei/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      767 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/huawei/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.464284 routersploit-3.4.3/tests/creds/routers/ipfire/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/ipfire/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/ipfire/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/ipfire/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      651 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/ipfire/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.465784 routersploit-3.4.3/tests/creds/routers/juniper/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/juniper/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      671 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/juniper/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      671 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/juniper/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      680 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/juniper/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.467515 routersploit-3.4.3/tests/creds/routers/linksys/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/linksys/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      663 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/linksys/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      663 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/linksys/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      672 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/linksys/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.469340 routersploit-3.4.3/tests/creds/routers/mikrotik/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/mikrotik/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      396 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/mikrotik/test_api_ros_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/mikrotik/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      620 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/mikrotik/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      629 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/mikrotik/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.470678 routersploit-3.4.3/tests/creds/routers/movistar/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/movistar/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      633 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/movistar/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      633 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/movistar/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/movistar/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.485071 routersploit-3.4.3/tests/creds/routers/netcore/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netcore/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      634 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netcore/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      634 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netcore/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      643 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netcore/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.486724 routersploit-3.4.3/tests/creds/routers/netgear/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netgear/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      643 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netgear/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      643 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netgear/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      652 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netgear/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.488485 routersploit-3.4.3/tests/creds/routers/netsys/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netsys/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netsys/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netsys/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/netsys/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.489294 routersploit-3.4.3/tests/creds/routers/pfsense/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/pfsense/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      621 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/pfsense/test_ssh_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.490833 routersploit-3.4.3/tests/creds/routers/technicolor/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/technicolor/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      673 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/technicolor/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      673 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/technicolor/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      682 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/technicolor/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.492255 routersploit-3.4.3/tests/creds/routers/thomson/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/thomson/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/thomson/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      637 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/thomson/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/thomson/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.493688 routersploit-3.4.3/tests/creds/routers/tplink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/tplink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/tplink/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      618 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/tplink/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      627 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/tplink/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.495084 routersploit-3.4.3/tests/creds/routers/ubiquiti/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/ubiquiti/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/ubiquiti/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      646 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/ubiquiti/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      655 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/ubiquiti/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.496560 routersploit-3.4.3/tests/creds/routers/zte/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/zte/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      685 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/zte/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      685 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/zte/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      694 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/zte/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.498046 routersploit-3.4.3/tests/creds/routers/zyxel/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/zyxel/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      665 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/zyxel/test_ftp_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      665 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/zyxel/test_ssh_default_creds.py
+-rw-r--r--   0 user       (501) staff       (20)      674 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/creds/routers/zyxel/test_telnet_default_creds.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.498408 routersploit-3.4.3/tests/encoders/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.499435 routersploit-3.4.3/tests/encoders/perl/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/perl/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      952 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/perl/test_base64.py
+-rw-r--r--   0 user       (501) staff       (20)     1065 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/perl/test_hex.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.500568 routersploit-3.4.3/tests/encoders/php/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/php/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1155 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/php/test_base64.py
+-rw-r--r--   0 user       (501) staff       (20)     1325 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/php/test_hex.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.501546 routersploit-3.4.3/tests/encoders/python/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/python/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1154 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/python/test_base64.py
+-rw-r--r--   0 user       (501) staff       (20)     1325 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/encoders/python/test_hex.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.501897 routersploit-3.4.3/tests/exploits/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.502172 routersploit-3.4.3/tests/exploits/cameras/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.502731 routersploit-3.4.3/tests/exploits/cameras/avigilon/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/avigilon/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1321 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/avigilon/test_videoiq_camera_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.503713 routersploit-3.4.3/tests/exploits/cameras/brickcom/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/brickcom/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1638 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/brickcom/test_corp_network_cameras_conf_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1382 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/brickcom/test_users_cgi_creds_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.504468 routersploit-3.4.3/tests/exploits/cameras/cisco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/cisco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1320 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/cisco/test_video_surv_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.518057 routersploit-3.4.3/tests/exploits/cameras/dlink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/dlink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     6441 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/dlink/test_dcs_930l_932l_auth_bypass.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.519253 routersploit-3.4.3/tests/exploits/cameras/honeywell/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/honeywell/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      662 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/honeywell/test_hicc_1100pt_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.520312 routersploit-3.4.3/tests/exploits/cameras/jovision/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/jovision/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      935 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/jovision/test_jovision_camera_credential_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.522598 routersploit-3.4.3/tests/exploits/cameras/multi/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/multi/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      853 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/multi/test_dvr_creds_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     2489 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/multi/test_jvc_vanderbilt_honeywell_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     1088 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/multi/test_netwave_ip_camera_information_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.523582 routersploit-3.4.3/tests/exploits/cameras/mvpower/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/mvpower/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      839 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/mvpower/test_dvr_jaws_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.524398 routersploit-3.4.3/tests/exploits/cameras/siemens/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/siemens/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      543 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/siemens/test_cvms2025_credentials_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.525135 routersploit-3.4.3/tests/exploits/cameras/xiongmai/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/xiongmai/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      602 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/cameras/xiongmai/test_uc_httpd_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.525557 routersploit-3.4.3/tests/exploits/misc/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/misc/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.526302 routersploit-3.4.3/tests/exploits/misc/miele/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/misc/miele/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1332 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/misc/miele/test_pg8528_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.527152 routersploit-3.4.3/tests/exploits/misc/wepresent/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/misc/wepresent/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      703 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/misc/wepresent/test_wipg1000_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.527666 routersploit-3.4.3/tests/exploits/routers/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.528823 routersploit-3.4.3/tests/exploits/routers/2wire/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/2wire/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1456 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/2wire/test_4011g_5012nv_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)      893 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/2wire/test_gateway_auth_bypass.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.531116 routersploit-3.4.3/tests/exploits/routers/3com/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/3com/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      836 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/3com/test_ap8760_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      732 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/3com/test_imc_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      747 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/3com/test_imc_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)      732 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/3com/test_officeconnect_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      814 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/3com/test_officeconnect_rce.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.532287 routersploit-3.4.3/tests/exploits/routers/asmax/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/asmax/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      654 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/asmax/test_ar_1004g_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1369 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/asmax/test_ar_804_gu_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.533907 routersploit-3.4.3/tests/exploits/routers/asus/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/asus/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2930 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/asus/test_asuswrt_lan_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2398 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/asus/test_infosvr_backdoor_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      580 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/asus/test_rt_n16_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.536530 routersploit-3.4.3/tests/exploits/routers/belkin/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/belkin/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      542 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/belkin/test_auth_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)      567 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/belkin/test_g_n150_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      738 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/belkin/test_g_plus_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1303 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/belkin/test_n150_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)      763 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/belkin/test_n750_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      701 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/belkin/test_play_mac_prce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.537184 routersploit-3.4.3/tests/exploits/routers/bhu/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/bhu/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      833 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/bhu/test_bhu_urouter_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.549925 routersploit-3.4.3/tests/exploits/routers/billion/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/billion/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      650 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/billion/test_billion_5200w_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      679 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/billion/test_billion_7700n4_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.555178 routersploit-3.4.3/tests/exploits/routers/cisco/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/cisco/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      539 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/cisco/test_dpc2420_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      679 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/cisco/test_firepower_management60_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)      757 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/cisco/test_firepower_management60_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      653 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/cisco/test_ios_http_authorization_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)      556 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/cisco/test_secure_acs_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)      546 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/cisco/test_ucm_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      768 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/cisco/test_ucs_manager_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     1322 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/cisco/test_unified_multi_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.556223 routersploit-3.4.3/tests/exploits/routers/comtrend/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/comtrend/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      631 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/comtrend/test_ct_5361t_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.566769 routersploit-3.4.3/tests/exploits/routers/dlink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      757 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dcs_930l_auth_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      600 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_300_320_600_615_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      575 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_300_320_615_auth_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)      747 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_300_600_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      838 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_300_645_815_upnp_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      639 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_645_815_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     2021 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_645_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      518 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_815_850l_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     1373 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_825_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)     1624 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_850l_creds_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1734 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_8xx_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      919 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dns_320l_327l_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     1304 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dsl_2730_2750_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)      604 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dsl_2730b_2780b_526b_dns_change.py
+-rw-r--r--   0 user       (501) staff       (20)      583 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dsl_2750b_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1117 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dsl_2750b_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      751 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dsp_w110_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     1312 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dvg_n5402sp_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)      582 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dwl_3200ap_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1019 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dwr_932_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      624 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_dwr_932b_backdoor.py
+-rw-r--r--   0 user       (501) staff       (20)      766 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_multi_hedwig_cgi_exec.py
+-rw-r--r--   0 user       (501) staff       (20)      667 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/dlink/test_multi_hnap_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.568603 routersploit-3.4.3/tests/exploits/routers/huawei/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/huawei/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1157 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/huawei/test_e5331_mifi_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     5344 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/huawei/test_hg520_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      576 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/huawei/test_hg530_hg520b_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      631 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/huawei/test_hg866_password_change.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.569548 routersploit-3.4.3/tests/exploits/routers/ipfire/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/ipfire/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      901 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/ipfire/test_ipfire_proxy_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      898 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/ipfire/test_ipfire_shellshock.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.571477 routersploit-3.4.3/tests/exploits/routers/linksys/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/linksys/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      968 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/linksys/test_1500_2500_rce.py
+-rw-r--r--   0 user       (501) staff       (20)     1629 2024-04-14 11:08:48.000000 routersploit-3.4.3/tests/exploits/routers/linksys/test_eseries_themoon_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      549 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/linksys/test_smartwifi_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      783 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/linksys/test_wap54gv3_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      750 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/linksys/test_wrt100_110_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.572044 routersploit-3.4.3/tests/exploits/routers/mikrotik/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/mikrotik/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3375 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/mikrotik/test_winbox_auth_bypass_creds_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.572613 routersploit-3.4.3/tests/exploits/routers/movistar/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/movistar/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      762 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/movistar/test_adsl_router_bhs_rta_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.575500 routersploit-3.4.3/tests/exploits/routers/multi/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/multi/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2076 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/multi/test_gpon_home_gateway_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      695 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/multi/test_misfortune_cookie.py
+-rw-r--r--   0 user       (501) staff       (20)    22373 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/multi/test_rom0.py
+-rw-r--r--   0 user       (501) staff       (20)      878 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/multi/test_tcp_32764_info_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)     1883 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/multi/test_tcp_32764_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.576089 routersploit-3.4.3/tests/exploits/routers/netcore/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netcore/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1108 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netcore/test_udp_53413_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.578685 routersploit-3.4.3/tests/exploits/routers/netgear/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netgear/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      892 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netgear/test_dgn2200_ping_cgi_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      830 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netgear/test_jnr1010_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)      966 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netgear/test_n300_auth_bypass.py
+-rw-r--r--   0 user       (501) staff       (20)     3288 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netgear/test_netgear_multi_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      778 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netgear/test_prosafe_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      791 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netgear/test_r7000_r6400_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      857 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netgear/test_wnr500_612v3_jnr1010_2010_path_traversal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.583207 routersploit-3.4.3/tests/exploits/routers/netsys/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netsys/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1838 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/netsys/test_multi_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.584289 routersploit-3.4.3/tests/exploits/routers/shuttle/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/shuttle/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      722 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/shuttle/test_915wm_dns_change.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.589050 routersploit-3.4.3/tests/exploits/routers/technicolor/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/technicolor/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      601 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/technicolor/test_dwg855_authbypass.py
+-rw-r--r--   0 user       (501) staff       (20)      569 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/technicolor/test_tc7200_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/technicolor/test_tc7200_password_disclosure_v2.py
+-rw-r--r--   0 user       (501) staff       (20)      479 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/technicolor/test_tg784_authbypass.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.590826 routersploit-3.4.3/tests/exploits/routers/thomson/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/thomson/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      560 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/thomson/test_twg850_password_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.593571 routersploit-3.4.3/tests/exploits/routers/tplink/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/tplink/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      655 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/tplink/test_archer_c2_c20i_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      917 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/tplink/test_wdr740nd_wdr740n_backdoor.py
+-rw-r--r--   0 user       (501) staff       (20)      875 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/tplink/test_wdr740nd_wdr740n_path_traversal.py
+-rw-r--r--   0 user       (501) staff       (20)      690 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/tplink/test_wdr842nd_wdr842n_configure_disclosure.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.595604 routersploit-3.4.3/tests/exploits/routers/zte/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zte/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      831 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zte/test_f460_f660_backdoor.py
+-rw-r--r--   0 user       (501) staff       (20)     3803 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zte/test_zxhn_h108n_wifi_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      872 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zte/test_zxv10_rce.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.598017 routersploit-3.4.3/tests/exploits/routers/zyxel/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zyxel/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      735 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zyxel/test_d1000_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      582 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zyxel/test_d1000_wifi_password_disclosure.py
+-rw-r--r--   0 user       (501) staff       (20)      673 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zyxel/test_p660hn_t_v1_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      757 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zyxel/test_p660hn_t_v2_rce.py
+-rw-r--r--   0 user       (501) staff       (20)      656 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/exploits/routers/zyxel/test_zywall_usg_extract_hashes.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.598413 routersploit-3.4.3/tests/generic/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/generic/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.598770 routersploit-3.4.3/tests/payloads/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.600888 routersploit-3.4.3/tests/payloads/armle/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/armle/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3151 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/armle/test_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     1516 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/armle/test_reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.616948 routersploit-3.4.3/tests/payloads/cmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      396 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_awk_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      396 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_awk_bind_udp.py
+-rw-r--r--   0 user       (501) staff       (20)      471 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_awk_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      405 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_bash_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      327 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_netcat_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      398 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_netcat_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      642 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_perl_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      694 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_perl_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      705 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_php_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      557 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_php_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      707 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_python_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      715 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_python_bind_udp.py
+-rw-r--r--   0 user       (501) staff       (20)      691 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_python_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      699 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/cmd/test_python_reverse_udp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.618895 routersploit-3.4.3/tests/payloads/mipsbe/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/mipsbe/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2908 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/mipsbe/test_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     2649 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/mipsbe/test_reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.621594 routersploit-3.4.3/tests/payloads/mipsle/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/mipsle/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2908 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/mipsle/test_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     2649 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/mipsle/test_reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.624184 routersploit-3.4.3/tests/payloads/php/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/php/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1218 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/php/test_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)      849 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/php/test_reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.626020 routersploit-3.4.3/tests/payloads/python/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/python/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1216 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/python/test_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     1198 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/python/test_bind_udp.py
+-rw-r--r--   0 user       (501) staff       (20)     1126 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/python/test_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     1168 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/python/test_reverse_udp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.627121 routersploit-3.4.3/tests/payloads/x64/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/x64/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1721 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/x64/test_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/x64/test_reverse_tcp.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-19 17:59:08.628373 routersploit-3.4.3/tests/payloads/x86/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/x86/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1433 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/x86/test_bind_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     1402 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/payloads/x86/test_reverse_tcp.py
+-rw-r--r--   0 user       (501) staff       (20)     1758 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/test_exploit_scenarios.py
+-rw-r--r--   0 user       (501) staff       (20)     2449 2024-04-08 16:47:10.000000 routersploit-3.4.3/tests/test_module_info.py
```

### Comparing `routersploit-3.4.2/LICENSE` & `routersploit-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/PKG-INFO` & `routersploit-3.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routersploit
-Version: 3.4.2
+Version: 3.4.3
 Summary: Exploitation Framework for Embedded Devices
 Home-page: https://www.threat9.com
 Author: Threat9
 Author-email: marcin@threat9.com
 License: UNKNOWN
 Download-URL: https://github.com/threat9/routersploit/
 Platform: UNKNOWN
```

### Comparing `routersploit-3.4.2/README.md` & `routersploit-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/bluetooth/btle/btle_device.py` & `routersploit-3.4.3/routersploit/core/bluetooth/btle/btle_device.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/bluetooth/btle/btle_scanner.py` & `routersploit-3.4.3/routersploit/core/bluetooth/btle/btle_scanner.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/bluetooth/btle_client.py` & `routersploit-3.4.3/routersploit/core/bluetooth/btle_client.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/exploit/__init__.py` & `routersploit-3.4.3/routersploit/core/exploit/__init__.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/exploit/encoders.py` & `routersploit-3.4.3/routersploit/core/exploit/encoders.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/exploit/exploit.py` & `routersploit-3.4.3/routersploit/core/exploit/exploit.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/exploit/option.py` & `routersploit-3.4.3/routersploit/core/exploit/option.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/exploit/payloads.py` & `routersploit-3.4.3/routersploit/core/exploit/payloads.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/exploit/printer.py` & `routersploit-3.4.3/routersploit/core/exploit/printer.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/exploit/shell.py` & `routersploit-3.4.3/routersploit/core/exploit/shell.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/exploit/utils.py` & `routersploit-3.4.3/routersploit/core/exploit/utils.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/ftp/ftp_client.py` & `routersploit-3.4.3/routersploit/core/ftp/ftp_client.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/http/http_client.py` & `routersploit-3.4.3/routersploit/core/http/http_client.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/snmp/snmp_client.py` & `routersploit-3.4.3/routersploit/core/snmp/snmp_client.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/ssh/ssh_client.py` & `routersploit-3.4.3/routersploit/core/ssh/ssh_client.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/tcp/tcp_client.py` & `routersploit-3.4.3/routersploit/core/tcp/tcp_client.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/telnet/telnet_client.py` & `routersploit-3.4.3/routersploit/core/telnet/telnet_client.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/core/udp/udp_client.py` & `routersploit-3.4.3/routersploit/core/udp/udp_client.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/interpreter.py` & `routersploit-3.4.3/routersploit/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
  | |\\ \\ (_) | |_| | ||  __/ |  /\\__/ / |_) | | (_) | | |_
  \\_| \\_\\___/ \\__,_|\\__\\___|_|  \\____/| .__/|_|\\___/|_|\\__|
                                      | |
        Exploitation Framework for    |_|    by Threat9
             Embedded Devices
 
  Codename   : I Knew You Were Trouble
- Version    : 3.4.2
+ Version    : 3.4.3
  Homepage   : https://www.threat9.com - @threatnine
 
  Exploits: {exploits_count} Scanners: {scanners_count} Creds: {creds_count} Generic: {generic_count} Payloads: {payloads_count} Encoders: {encoders_count}
 """.format(exploits_count=self.modules_count["exploits"],
            scanners_count=self.modules_count["scanners"],
            creds_count=self.modules_count["creds"],
            generic_count=self.modules_count["generic"],
```

### Comparing `routersploit-3.4.2/routersploit/libs/apiros/apiros_client.py` & `routersploit-3.4.3/routersploit/libs/apiros/apiros_client.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/libs/lzs/lzs.py` & `routersploit-3.4.3/routersploit/libs/lzs/lzs.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/acti/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/acti/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/acti/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/acti/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/acti/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/acti/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/acti/webinterface_http_form_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/acti/webinterface_http_form_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/american_dynamics/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/american_dynamics/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/american_dynamics/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/american_dynamics/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/american_dynamics/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/american_dynamics/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/arecont/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/arecont/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/arecont/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/arecont/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/arecont/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/arecont/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/avigilon/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/avigilon/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/avigilon/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/avigilon/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/avigilon/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/avigilon/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/avtech/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/avtech/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/avtech/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/avtech/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/avtech/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/avtech/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/axis/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/axis/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/axis/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/axis/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/axis/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/axis/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/axis/webinterface_http_auth_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/axis/webinterface_http_auth_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/basler/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/basler/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/basler/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/basler/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/basler/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/basler/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/basler/webinterface_http_form_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/basler/webinterface_http_form_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/brickcom/webinterface_http_auth_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/brickcom/webinterface_http_auth_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/canon/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/canon/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/canon/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/canon/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/canon/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/canon/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/canon/webinterface_http_auth_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/canon/webinterface_http_auth_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/cisco/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/cisco/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/cisco/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/cisco/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/cisco/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/cisco/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/dlink/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/dlink/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/dlink/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/dlink/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/dlink/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/dlink/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/geovision/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/geovision/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/geovision/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/geovision/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/geovision/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/geovision/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/grandstream/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/grandstream/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/grandstream/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/grandstream/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/grandstream/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/grandstream/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/hikvision/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/hikvision/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/hikvision/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/hikvision/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/hikvision/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/hikvision/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/honeywell/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/honeywell/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/honeywell/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/honeywell/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/honeywell/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/honeywell/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/iqinvision/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/iqinvision/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/iqinvision/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/iqinvision/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/iqinvision/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/iqinvision/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/jvc/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/jvc/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/jvc/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/jvc/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/jvc/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/jvc/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/mobotix/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/mobotix/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/mobotix/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/mobotix/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/mobotix/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/mobotix/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/samsung/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/samsung/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/samsung/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/samsung/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/samsung/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/samsung/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/sentry360/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/sentry360/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/sentry360/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/sentry360/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/sentry360/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/sentry360/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/siemens/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/siemens/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/siemens/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/siemens/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/siemens/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/siemens/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/speco/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/speco/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/speco/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/speco/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/speco/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/speco/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/stardot/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/stardot/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/stardot/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/stardot/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/stardot/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/stardot/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/vacron/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/vacron/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/vacron/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/vacron/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/vacron/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/vacron/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/videoiq/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/videoiq/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/videoiq/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/videoiq/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/cameras/videoiq/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/cameras/videoiq/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/generic/ftp_bruteforce.py` & `routersploit-3.4.3/routersploit/modules/creds/generic/ftp_bruteforce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/generic/ftp_default.py` & `routersploit-3.4.3/routersploit/modules/creds/generic/ftp_default.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/generic/http_basic_digest_bruteforce.py` & `routersploit-3.4.3/routersploit/modules/creds/generic/http_basic_digest_bruteforce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/generic/http_basic_digest_default.py` & `routersploit-3.4.3/routersploit/modules/creds/generic/http_basic_digest_default.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/generic/snmp_bruteforce.py` & `routersploit-3.4.3/routersploit/modules/creds/generic/snmp_bruteforce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/generic/ssh_bruteforce.py` & `routersploit-3.4.3/routersploit/modules/creds/generic/ssh_bruteforce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/generic/ssh_default.py` & `routersploit-3.4.3/routersploit/modules/creds/generic/ssh_default.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/generic/telnet_bruteforce.py` & `routersploit-3.4.3/routersploit/modules/creds/generic/telnet_bruteforce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/generic/telnet_default.py` & `routersploit-3.4.3/routersploit/modules/creds/generic/telnet_default.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/2wire/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/2wire/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/2wire/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/2wire/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/2wire/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/2wire/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/3com/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/3com/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/3com/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/3com/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/3com/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/3com/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/asmax/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/asmax/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/asmax/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/asmax/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/asmax/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/asmax/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/asmax/webinterface_http_auth_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/asmax/webinterface_http_auth_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/asus/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/asus/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/asus/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/asus/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/asus/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/asus/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/belkin/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/belkin/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/belkin/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/belkin/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/belkin/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/belkin/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/bhu/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/bhu/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/bhu/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/bhu/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/bhu/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/bhu/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/billion/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/billion/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/billion/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/billion/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/billion/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/billion/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/cisco/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/cisco/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/cisco/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/cisco/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/cisco/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/cisco/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/comtrend/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/comtrend/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/comtrend/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/comtrend/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/comtrend/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/comtrend/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/dlink/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/dlink/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/dlink/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/dlink/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/dlink/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/dlink/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/fortinet/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/fortinet/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/fortinet/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/fortinet/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/fortinet/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/fortinet/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/huawei/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/huawei/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/huawei/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/huawei/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/huawei/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/huawei/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/ipfire/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/ipfire/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/ipfire/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/ipfire/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/ipfire/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/ipfire/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/juniper/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/juniper/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/juniper/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/juniper/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/juniper/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/juniper/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/linksys/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/linksys/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/linksys/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/linksys/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/linksys/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/linksys/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/api_ros_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/api_ros_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/mikrotik/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/mikrotik/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/movistar/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/movistar/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/movistar/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/movistar/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/movistar/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/movistar/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/netcore/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/netcore/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/netcore/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/netcore/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/netcore/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/netcore/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/netgear/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/netgear/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/netgear/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/netgear/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/netgear/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/netgear/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/netsys/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/netsys/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/netsys/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/netsys/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/netsys/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/netsys/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/pfsense/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/pfsense/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/pfsense/webinterface_http_form_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/pfsense/webinterface_http_form_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/technicolor/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/technicolor/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/technicolor/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/technicolor/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/technicolor/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/technicolor/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/thomson/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/thomson/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/thomson/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/thomson/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/thomson/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/thomson/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/tplink/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/tplink/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/tplink/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/tplink/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/tplink/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/tplink/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/ubiquiti/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/ubiquiti/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/ubiquiti/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/ubiquiti/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/ubiquiti/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/ubiquiti/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/zte/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/zte/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/zte/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/zte/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/zte/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/zte/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/zyxel/ftp_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/zyxel/ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/zyxel/ssh_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/zyxel/ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/creds/routers/zyxel/telnet_default_creds.py` & `routersploit-3.4.3/routersploit/modules/creds/routers/zyxel/telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/encoders/php/base64.py` & `routersploit-3.4.3/routersploit/modules/encoders/php/base64.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/encoders/php/hex.py` & `routersploit-3.4.3/routersploit/modules/encoders/php/hex.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/encoders/python/base64.py` & `routersploit-3.4.3/routersploit/modules/encoders/python/base64.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/encoders/python/hex.py` & `routersploit-3.4.3/routersploit/modules/encoders/python/hex.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/avigilon/videoiq_camera_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/avigilon/videoiq_camera_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/brickcom/corp_network_cameras_conf_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/brickcom/corp_network_cameras_conf_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/brickcom/users_cgi_creds_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/brickcom/users_cgi_creds_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/cisco/video_surv_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/cisco/video_surv_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/dlink/dcs_930l_932l_auth_bypass.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/dlink/dcs_930l_932l_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/grandstream/gxv3611hd_ip_camera_backdoor.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/grandstream/gxv3611hd_ip_camera_backdoor.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/grandstream/gxv3611hd_ip_camera_sqli.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/grandstream/gxv3611hd_ip_camera_sqli.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/honeywell/hicc_1100pt_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/honeywell/hicc_1100pt_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/jovision/jovision_credentials_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/jovision/jovision_credentials_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/P2P_wificam_credential_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/P2P_wificam_credential_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/P2P_wificam_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/P2P_wificam_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/dvr_creds_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/dvr_creds_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/jvc_vanderbilt_honeywell_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/jvc_vanderbilt_honeywell_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/multi/netwave_ip_camera_information_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/multi/netwave_ip_camera_information_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/mvpower/dvr_jaws_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/mvpower/dvr_jaws_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/siemens/cvms2025_credentials_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/siemens/cvms2025_credentials_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/cameras/xiongmai/uc_httpd_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/cameras/xiongmai/uc_httpd_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/generic/heartbleed.py` & `routersploit-3.4.3/routersploit/modules/exploits/generic/heartbleed.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/generic/shellshock.py` & `routersploit-3.4.3/routersploit/modules/exploits/generic/shellshock.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/generic/ssh_auth_keys.py` & `routersploit-3.4.3/routersploit/modules/exploits/generic/ssh_auth_keys.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/misc/asus/b1m_projector_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/misc/asus/b1m_projector_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/misc/miele/pg8528_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/misc/miele/pg8528_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/misc/wepresent/wipg1000_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/misc/wepresent/wipg1000_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/2wire/4011g_5012nv_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/2wire/4011g_5012nv_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/2wire/gateway_auth_bypass.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/2wire/gateway_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/3com/ap8760_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/3com/ap8760_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/3com/imc_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/3com/imc_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/3com/imc_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/3com/imc_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/3com/officeconnect_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/3com/officeconnect_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/3com/officeconnect_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/3com/officeconnect_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/asmax/ar_1004g_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/asmax/ar_1004g_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/asmax/ar_804_gu_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/asmax/ar_804_gu_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/asus/asuswrt_lan_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/asus/asuswrt_lan_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/asus/infosvr_backdoor_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/asus/infosvr_backdoor_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/asus/rt_n16_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/asus/rt_n16_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/auth_bypass.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/g_n150_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/g_n150_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/g_plus_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/g_plus_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/n150_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/n150_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/n750_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/n750_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/belkin/play_max_prce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/belkin/play_max_prce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/bhu/bhu_urouter_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/bhu/bhu_urouter_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/billion/billion_5200w_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/billion/billion_5200w_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/billion/billion_7700nr4_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/billion/billion_7700nr4_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/catalyst_2960_rocem.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/catalyst_2960_rocem.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/dpc2420_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/dpc2420_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/firepower_management60_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/firepower_management60_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/firepower_management60_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/firepower_management60_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/ios_http_authorization_bypass.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/ios_http_authorization_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/secure_acs_bypass.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/secure_acs_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/ucm_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/ucm_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/ucs_manager_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/ucs_manager_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/cisco/unified_multi_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/cisco/unified_multi_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/comtrend/ct_5361t_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/comtrend/ct_5361t_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dcs_930l_auth_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dcs_930l_auth_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dgs_1510_add_user.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dgs_1510_add_user.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_300_320_600_615_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_300_320_600_615_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_300_320_615_auth_bypass.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_300_320_615_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_300_600_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_300_600_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_300_645_815_upnp_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_300_645_815_upnp_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_645_815_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_645_815_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_645_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_645_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_815_850l_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_815_850l_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_825_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_825_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_850l_creds_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_850l_creds_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dir_8xx_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dir_8xx_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dns_320l_327l_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dns_320l_327l_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2640b_dns_change.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2640b_dns_change.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2730_2750_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2730_2750_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2730b_2780b_526b_dns_change.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2730b_2780b_526b_dns_change.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2740r_dns_change.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2740r_dns_change.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2750b_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2750b_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsl_2750b_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsl_2750b_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dsp_w110_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dsp_w110_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dvg_n5402sp_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dvg_n5402sp_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dwl_3200ap_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dwl_3200ap_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dwr_932_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dwr_932_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/dwr_932b_backdoor.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/dwr_932b_backdoor.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/multi_hedwig_cgi_exec.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/multi_hedwig_cgi_exec.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/dlink/multi_hnap_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/dlink/multi_hnap_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/fortinet/fortigate_os_backdoor.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/fortinet/fortigate_os_backdoor.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/e5331_mifi_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/e5331_mifi_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/hg520_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/hg520_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/hg530_hg520b_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/hg530_hg520b_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/hg532_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/hg532_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/huawei/hg866_password_change.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/huawei/hg866_password_change.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/ipfire/ipfire_oinkcode_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/ipfire/ipfire_oinkcode_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/ipfire/ipfire_proxy_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/ipfire/ipfire_proxy_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/ipfire/ipfire_shellshock.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/ipfire/ipfire_shellshock.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/1500_2500_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/1500_2500_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/eseries_themoon_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/eseries_themoon_rce.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,11 +95,11 @@
         # target may be vulnerable
 
         response = self.http_request(
             method="GET",
             path="/tmUnblock.cgi",
         )
 
-        if response and response.status_code in [200, 301, 302]:
+        if response and response.status_code in [200, 301, 302] and not any(i in response.text.lower() for i in ["page not found", "error", "404", "not found"]):
             return True  # target is vulnerable
 
         return False  # target is not vulnerable
```

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/smartwifi_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/smartwifi_password_disclosure.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,25 +43,30 @@
                 method="GET",
                 path="/.htpasswd"
             )
             if response is None:
                 print_error("Exploit failed - connection error")
                 return
 
-            print_info("Unix crypt hash: $id$salt$hashed")  # See more at http://man7.org/linux/man-pages/man3/crypt.3.html
+            if (response.text.find('$') != -1):
+                print_info("Likely Unix crypt hash: $id$salt$hashed")  # See more at http://man7.org/linux/man-pages/man3/crypt.3.html
+            else:
+                print_info("Likely base64 encoded .htaccess") # John understands this natively
+                
             print_success("Hash found:", response.text)
         else:
             print_error("Exploit failed - target seems to be not vulnerable")
 
     @mute
     def check(self):
+
         response = self.http_request(
             method="GET",
             path="/.htpasswd"
         )
 
         if response is not None and response.status_code == 200:
-            res = re.findall(r"^([a-zA-Z0-9]+:\$[0-9]\$)", response.text)
+            res = re.findall(r"^([a-zA-Z0-9]+:\S+)", response.text)
             if len(res):
                 return True
 
         return False
```

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/wap54gv3_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/wap54gv3_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/linksys/wrt100_110_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/linksys/wrt100_110_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/mikrotik/routeros_jailbreak.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/mikrotik/routeros_jailbreak.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/mikrotik/winbox_auth_bypass_creds_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/mikrotik/winbox_auth_bypass_creds_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/movistar/adsl_router_bhs_rta_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/movistar/adsl_router_bhs_rta_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/multi/gpon_home_gateway_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/multi/gpon_home_gateway_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/multi/misfortune_cookie.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/multi/misfortune_cookie.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/multi/rom0.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/multi/rom0.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/multi/tcp_32764_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/multi/tcp_32764_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/multi/tcp_32764_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/multi/tcp_32764_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netcore/udp_53413_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netcore/udp_53413_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/dgn2200_dnslookup_cgi_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/dgn2200_dnslookup_cgi_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/dgn2200_ping_cgi_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/dgn2200_ping_cgi_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/jnr1010_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/jnr1010_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/multi_password_disclosure-2017-5521.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/multi_password_disclosure-2017-5521.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/multi_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/multi_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/n300_auth_bypass.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/n300_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/prosafe_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/prosafe_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/r7000_r6400_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/r7000_r6400_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netgear/wnr500_612v3_jnr1010_2010_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netgear/wnr500_612v3_jnr1010_2010_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/netsys/multi_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/netsys/multi_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/shuttle/915wm_dns_change.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/shuttle/915wm_dns_change.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/dwg855_authbypass.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/dwg855_authbypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/tc7200_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/tc7200_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/tc7200_password_disclosure_v2.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/tc7200_password_disclosure_v2.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/technicolor/tg784_authbypass.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/technicolor/tg784_authbypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/thomson/twg849_info_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/thomson/twg849_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/thomson/twg850_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/thomson/twg850_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/archer_c2_c20i_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/archer_c2_c20i_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/archer_c9_admin_password_reset.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/archer_c9_admin_password_reset.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/wdr740nd_wdr740n_backdoor.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/wdr740nd_wdr740n_backdoor.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/wdr740nd_wdr740n_path_traversal.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/wdr740nd_wdr740n_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/tplink/wdr842nd_wdr842n_configure_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/tplink/wdr842nd_wdr842n_configure_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/ubiquiti/airos_6_x.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/ubiquiti/airos_6_x.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/zte/f460_f660_backdoor.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/zte/f460_f660_backdoor.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/zte/zxhn_h108n_wifi_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/zte/zxhn_h108n_wifi_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/zte/zxv10_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/zte/zxv10_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/d1000_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/d1000_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/d1000_wifi_password_disclosure.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/d1000_wifi_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/p660hn_t_v1_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/p660hn_t_v1_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/p660hn_t_v2_rce.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/p660hn_t_v2_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/exploits/routers/zyxel/zywall_usg_extract_hashes.py` & `routersploit-3.4.3/routersploit/modules/exploits/routers/zyxel/zywall_usg_extract_hashes.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/generic/bluetooth/btle_enumerate.py` & `routersploit-3.4.3/routersploit/modules/generic/bluetooth/btle_enumerate.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/generic/bluetooth/btle_scan.py` & `routersploit-3.4.3/routersploit/modules/generic/bluetooth/btle_scan.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/generic/bluetooth/btle_write.py` & `routersploit-3.4.3/routersploit/modules/generic/bluetooth/btle_write.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/generic/upnp/ssdp_msearch.py` & `routersploit-3.4.3/routersploit/modules/generic/upnp/ssdp_msearch.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/armle/bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/armle/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/armle/reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/armle/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/awk_bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/awk_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/awk_bind_udp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/awk_bind_udp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/awk_reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/awk_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/bash_reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/bash_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/netcat_bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/netcat_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/netcat_reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/netcat_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/perl_bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/perl_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/perl_reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/perl_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/php_bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/php_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/php_reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/php_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/python_bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/python_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/python_bind_udp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/python_bind_udp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/python_reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/python_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/cmd/python_reverse_udp.py` & `routersploit-3.4.3/routersploit/modules/payloads/cmd/python_reverse_udp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/mipsbe/bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/mipsbe/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/mipsbe/reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/mipsbe/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/mipsle/bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/mipsle/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/mipsle/reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/mipsle/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/perl/bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/perl/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/perl/reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/perl/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/php/bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/php/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/php/reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/php/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/python/bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/python/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/python/bind_udp.py` & `routersploit-3.4.3/routersploit/modules/payloads/python/bind_udp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/python/reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/python/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/python/reverse_udp.py` & `routersploit-3.4.3/routersploit/modules/payloads/python/reverse_udp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/x64/bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/x64/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/x64/reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/x64/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/x86/bind_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/x86/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/payloads/x86/reverse_tcp.py` & `routersploit-3.4.3/routersploit/modules/payloads/x86/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/modules/scanners/autopwn.py` & `routersploit-3.4.3/routersploit/modules/scanners/autopwn.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/array-networks-vapv-vxag.json` & `routersploit-3.4.3/routersploit/resources/ssh_keys/array-networks-vapv-vxag.json`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/array-networks-vapv-vxag.key` & `routersploit-3.4.3/routersploit/resources/ssh_keys/array-networks-vapv-vxag.key`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/barracuda_load_balancer_vm.json` & `routersploit-3.4.3/routersploit/resources/ssh_keys/barracuda_load_balancer_vm.json`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/barracuda_load_balancer_vm.key` & `routersploit-3.4.3/routersploit/resources/ssh_keys/barracuda_load_balancer_vm.key`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/ceragon-fibeair-cve-2015-0936.key` & `routersploit-3.4.3/routersploit/resources/ssh_keys/ceragon-fibeair-cve-2015-0936.key`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/exagrid-cve-2016-1561.key` & `routersploit-3.4.3/routersploit/resources/ssh_keys/exagrid-cve-2016-1561.key`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/f5-bigip-cve-2012-1493.key` & `routersploit-3.4.3/routersploit/resources/ssh_keys/f5-bigip-cve-2012-1493.key`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/loadbalancer.org-enterprise-va.json` & `routersploit-3.4.3/routersploit/resources/ssh_keys/loadbalancer.org-enterprise-va.json`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/loadbalancer.org-enterprise-va.key` & `routersploit-3.4.3/routersploit/resources/ssh_keys/loadbalancer.org-enterprise-va.key`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/monroe-dasdec-cve-2013-0137.json` & `routersploit-3.4.3/routersploit/resources/ssh_keys/monroe-dasdec-cve-2013-0137.json`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/monroe-dasdec-cve-2013-0137.key` & `routersploit-3.4.3/routersploit/resources/ssh_keys/monroe-dasdec-cve-2013-0137.key`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/quantum-dxi-v1000.json` & `routersploit-3.4.3/routersploit/resources/ssh_keys/quantum-dxi-v1000.json`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/quantum-dxi-v1000.key` & `routersploit-3.4.3/routersploit/resources/ssh_keys/quantum-dxi-v1000.key`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/ssh_keys/vagrant.key` & `routersploit-3.4.3/routersploit/resources/ssh_keys/vagrant.key`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/vendors/oui.dat` & `routersploit-3.4.3/routersploit/resources/vendors/oui.dat`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/wordlists/defaults.txt` & `routersploit-3.4.3/routersploit/resources/wordlists/defaults.txt`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/wordlists/passwords.txt` & `routersploit-3.4.3/routersploit/resources/wordlists/passwords.txt`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/wordlists/snmp.txt` & `routersploit-3.4.3/routersploit/resources/wordlists/snmp.txt`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit/resources/wordlists/usernames.txt` & `routersploit-3.4.3/routersploit/resources/wordlists/usernames.txt`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/routersploit.egg-info/PKG-INFO` & `routersploit-3.4.3/routersploit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routersploit
-Version: 3.4.2
+Version: 3.4.3
 Summary: Exploitation Framework for Embedded Devices
 Home-page: https://www.threat9.com
 Author: Threat9
 Author-email: marcin@threat9.com
 License: UNKNOWN
 Download-URL: https://github.com/threat9/routersploit/
 Platform: UNKNOWN
```

### Comparing `routersploit-3.4.2/routersploit.egg-info/SOURCES.txt` & `routersploit-3.4.3/routersploit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -425,14 +425,15 @@
 routersploit/modules/exploits/routers/netgear/dgn2200_ping_cgi_rce.py
 routersploit/modules/exploits/routers/netgear/jnr1010_path_traversal.py
 routersploit/modules/exploits/routers/netgear/multi_password_disclosure-2017-5521.py
 routersploit/modules/exploits/routers/netgear/multi_rce.py
 routersploit/modules/exploits/routers/netgear/n300_auth_bypass.py
 routersploit/modules/exploits/routers/netgear/prosafe_rce.py
 routersploit/modules/exploits/routers/netgear/r7000_r6400_rce.py
+routersploit/modules/exploits/routers/netgear/rax30_rce.py
 routersploit/modules/exploits/routers/netgear/wnr500_612v3_jnr1010_2010_path_traversal.py
 routersploit/modules/exploits/routers/netsys/__init__.py
 routersploit/modules/exploits/routers/netsys/multi_rce.py
 routersploit/modules/exploits/routers/shuttle/915wm_dns_change.py
 routersploit/modules/exploits/routers/shuttle/__init__.py
 routersploit/modules/exploits/routers/technicolor/__init__.py
 routersploit/modules/exploits/routers/technicolor/dwg855_authbypass.py
```

### Comparing `routersploit-3.4.2/rsf.py` & `routersploit-3.4.3/rsf.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/setup.py` & `routersploit-3.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="routersploit",
-    version="3.4.2",
+    version="3.4.3",
     description="Exploitation Framework for Embedded Devices",
     long_description=long_description,
     author="Threat9",
     author_email="marcin@threat9.com",
     url="https://www.threat9.com",
     download_url="https://github.com/threat9/routersploit/",
     packages=find_packages(),
```

### Comparing `routersploit-3.4.2/tests/conftest.py` & `routersploit-3.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/core/test_option.py` & `routersploit-3.4.3/tests/core/test_option.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/acti/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/acti/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/acti/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/acti/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/acti/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/acti/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/acti/test_webinterface_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/acti/test_webinterface_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/american_dynamics/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/american_dynamics/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/american_dynamics/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/american_dynamics/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/american_dynamics/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/american_dynamics/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/arecont/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/arecont/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/arecont/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/arecont/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/arecont/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/arecont/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/avigilon/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/avigilon/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/avigilon/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/avigilon/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/avigilon/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/avigilon/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/avtech/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/avtech/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/avtech/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/avtech/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/avtech/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/avtech/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/axis/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/axis/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/axis/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/axis/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/axis/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/axis/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/axis/test_webinterface_http_auth_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/axis/test_webinterface_http_auth_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/basler/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/basler/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/basler/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/basler/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/basler/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/basler/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/basler/test_webinterface_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/basler/test_webinterface_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/brickcom/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/brickcom/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/brickcom/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/brickcom/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/brickcom/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/brickcom/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/brickcom/test_webinterface_http_auth_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/brickcom/test_webinterface_http_auth_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/canon/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/canon/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/canon/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/canon/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/canon/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/canon/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/canon/test_webinterface_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/canon/test_webinterface_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/cisco/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/cisco/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/cisco/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/cisco/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/cisco/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/cisco/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/dlink/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/dlink/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/dlink/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/dlink/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/dlink/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/dlink/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/geovision/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/geovision/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/geovision/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/geovision/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/geovision/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/geovision/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/grandstream/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/grandstream/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/grandstream/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/grandstream/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/grandstream/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/grandstream/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/hikvision/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/hikvision/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/hikvision/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/hikvision/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/hikvision/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/hikvision/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/honeywell/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/honeywell/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/honeywell/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/honeywell/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/honeywell/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/honeywell/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/iqinvision/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/iqinvision/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/iqinvision/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/iqinvision/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/iqinvision/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/iqinvision/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/jvc/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/jvc/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/jvc/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/jvc/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/jvc/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/jvc/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/mobotix/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/mobotix/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/mobotix/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/mobotix/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/mobotix/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/mobotix/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/samsung/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/samsung/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/samsung/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/samsung/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/samsung/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/samsung/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/sentry360/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/sentry360/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/sentry360/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/sentry360/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/sentry360/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/sentry360/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/siemens/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/siemens/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/siemens/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/siemens/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/siemens/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/siemens/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/speco/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/speco/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/speco/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/speco/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/speco/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/speco/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/stardot/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/stardot/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/stardot/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/stardot/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/stardot/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/stardot/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/vacron/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/vacron/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/vacron/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/vacron/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/vacron/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/vacron/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/videoiq/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/videoiq/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/videoiq/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/videoiq/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/cameras/videoiq/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/cameras/videoiq/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/2wire/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/2wire/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/2wire/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/2wire/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/2wire/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/2wire/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/3com/test_3com_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/3com/test_3com_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/3com/test_3com_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/3com/test_3com_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/3com/test_3com_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/3com/test_3com_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/asmax/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/asmax/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/asmax/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/asmax/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/asmax/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/asmax/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/asmax/test_webinterface_http_auth_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/asmax/test_webinterface_http_auth_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/asus/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/asus/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/asus/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/asus/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/asus/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/asus/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/belkin/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/belkin/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/belkin/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/belkin/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/belkin/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/belkin/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/bhu/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/bhu/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/bhu/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/bhu/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/bhu/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/bhu/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/billion/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/billion/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/billion/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/billion/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/billion/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/billion/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/cisco/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/cisco/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/cisco/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/cisco/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/cisco/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/cisco/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/comtrend/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/comtrend/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/comtrend/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/comtrend/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/comtrend/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/comtrend/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/dlink/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/dlink/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/dlink/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/dlink/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/dlink/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/dlink/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/fortinet/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/fortinet/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/fortinet/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/fortinet/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/fortinet/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/fortinet/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/huawei/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/huawei/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/huawei/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/huawei/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/huawei/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/huawei/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/ipfire/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/ipfire/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/ipfire/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/ipfire/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/ipfire/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/ipfire/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/juniper/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/juniper/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/juniper/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/juniper/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/juniper/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/juniper/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/linksys/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/linksys/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/linksys/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/linksys/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/linksys/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/linksys/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/mikrotik/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/mikrotik/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/mikrotik/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/mikrotik/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/mikrotik/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/mikrotik/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/movistar/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/movistar/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/movistar/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/movistar/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/movistar/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/movistar/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/netcore/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/netcore/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/netcore/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/netcore/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/netcore/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/netcore/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/netgear/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/netgear/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/netgear/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/netgear/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/netgear/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/netgear/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/netsys/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/netsys/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/netsys/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/netsys/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/netsys/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/netsys/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/pfsense/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/pfsense/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/technicolor/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/technicolor/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/technicolor/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/technicolor/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/technicolor/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/technicolor/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/thomson/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/thomson/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/thomson/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/thomson/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/thomson/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/thomson/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/tplink/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/tplink/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/tplink/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/tplink/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/tplink/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/tplink/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/ubiquiti/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/ubiquiti/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/ubiquiti/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/ubiquiti/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/ubiquiti/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/ubiquiti/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/zte/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/zte/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/zte/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/zte/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/zte/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/zte/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/zyxel/test_ftp_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/zyxel/test_ftp_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/zyxel/test_ssh_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/zyxel/test_ssh_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/creds/routers/zyxel/test_telnet_default_creds.py` & `routersploit-3.4.3/tests/creds/routers/zyxel/test_telnet_default_creds.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/encoders/perl/test_base64.py` & `routersploit-3.4.3/tests/encoders/perl/test_base64.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/encoders/perl/test_hex.py` & `routersploit-3.4.3/tests/encoders/perl/test_hex.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/encoders/php/test_base64.py` & `routersploit-3.4.3/tests/encoders/php/test_base64.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/encoders/php/test_hex.py` & `routersploit-3.4.3/tests/encoders/php/test_hex.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/encoders/python/test_base64.py` & `routersploit-3.4.3/tests/encoders/python/test_base64.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/encoders/python/test_hex.py` & `routersploit-3.4.3/tests/encoders/python/test_hex.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/avigilon/test_videoiq_camera_path_traversal.py` & `routersploit-3.4.3/tests/exploits/cameras/avigilon/test_videoiq_camera_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/brickcom/test_corp_network_cameras_conf_disclosure.py` & `routersploit-3.4.3/tests/exploits/cameras/brickcom/test_corp_network_cameras_conf_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/brickcom/test_users_cgi_creds_disclosure.py` & `routersploit-3.4.3/tests/exploits/cameras/brickcom/test_users_cgi_creds_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/cisco/test_video_surv_path_traversal.py` & `routersploit-3.4.3/tests/exploits/cameras/cisco/test_video_surv_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/dlink/test_dcs_930l_932l_auth_bypass.py` & `routersploit-3.4.3/tests/exploits/cameras/dlink/test_dcs_930l_932l_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/honeywell/test_hicc_1100pt_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/cameras/honeywell/test_hicc_1100pt_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/jovision/test_jovision_camera_credential_disclosure.py` & `routersploit-3.4.3/tests/exploits/cameras/jovision/test_jovision_camera_credential_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/multi/test_dvr_creds_disclosure.py` & `routersploit-3.4.3/tests/exploits/cameras/multi/test_dvr_creds_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/multi/test_jvc_vanderbilt_honeywell_path_traversal.py` & `routersploit-3.4.3/tests/exploits/cameras/multi/test_jvc_vanderbilt_honeywell_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/multi/test_netwave_ip_camera_information_disclosure.py` & `routersploit-3.4.3/tests/exploits/cameras/multi/test_netwave_ip_camera_information_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/mvpower/test_dvr_jaws_rce.py` & `routersploit-3.4.3/tests/exploits/cameras/mvpower/test_dvr_jaws_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/siemens/test_cvms2025_credentials_disclosure.py` & `routersploit-3.4.3/tests/exploits/cameras/siemens/test_cvms2025_credentials_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/cameras/xiongmai/test_uc_httpd_path_traversal.py` & `routersploit-3.4.3/tests/exploits/cameras/xiongmai/test_uc_httpd_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/misc/miele/test_pg8528_path_traversal.py` & `routersploit-3.4.3/tests/exploits/misc/miele/test_pg8528_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/misc/wepresent/test_wipg1000_rce.py` & `routersploit-3.4.3/tests/exploits/misc/wepresent/test_wipg1000_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/2wire/test_4011g_5012nv_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/2wire/test_4011g_5012nv_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/2wire/test_gateway_auth_bypass.py` & `routersploit-3.4.3/tests/exploits/routers/2wire/test_gateway_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/3com/test_ap8760_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/3com/test_ap8760_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/3com/test_imc_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/3com/test_imc_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/3com/test_imc_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/3com/test_imc_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/3com/test_officeconnect_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/3com/test_officeconnect_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/3com/test_officeconnect_rce.py` & `routersploit-3.4.3/tests/exploits/routers/3com/test_officeconnect_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/asmax/test_ar_1004g_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/asmax/test_ar_1004g_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/asmax/test_ar_804_gu_rce.py` & `routersploit-3.4.3/tests/exploits/routers/asmax/test_ar_804_gu_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/asus/test_asuswrt_lan_rce.py` & `routersploit-3.4.3/tests/exploits/routers/asus/test_asuswrt_lan_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/asus/test_infosvr_backdoor_rce.py` & `routersploit-3.4.3/tests/exploits/routers/asus/test_infosvr_backdoor_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/asus/test_rt_n16_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/asus/test_rt_n16_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/belkin/test_auth_bypass.py` & `routersploit-3.4.3/tests/exploits/routers/belkin/test_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/belkin/test_g_n150_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/belkin/test_g_n150_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/belkin/test_g_plus_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/belkin/test_g_plus_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/belkin/test_n150_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/belkin/test_n150_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/belkin/test_n750_rce.py` & `routersploit-3.4.3/tests/exploits/routers/belkin/test_n750_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/belkin/test_play_mac_prce.py` & `routersploit-3.4.3/tests/exploits/routers/belkin/test_play_mac_prce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/bhu/test_bhu_urouter_rce.py` & `routersploit-3.4.3/tests/exploits/routers/bhu/test_bhu_urouter_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/billion/test_billion_5200w_rce.py` & `routersploit-3.4.3/tests/exploits/routers/billion/test_billion_5200w_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/billion/test_billion_7700n4_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/billion/test_billion_7700n4_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/cisco/test_dpc2420_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/cisco/test_dpc2420_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/cisco/test_firepower_management60_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/cisco/test_firepower_management60_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/cisco/test_firepower_management60_rce.py` & `routersploit-3.4.3/tests/exploits/routers/cisco/test_firepower_management60_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/cisco/test_ios_http_authorization_bypass.py` & `routersploit-3.4.3/tests/exploits/routers/cisco/test_ios_http_authorization_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/cisco/test_secure_acs_bypass.py` & `routersploit-3.4.3/tests/exploits/routers/cisco/test_secure_acs_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/cisco/test_ucm_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/cisco/test_ucm_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/cisco/test_ucs_manager_rce.py` & `routersploit-3.4.3/tests/exploits/routers/cisco/test_ucs_manager_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/cisco/test_unified_multi_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/cisco/test_unified_multi_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/comtrend/test_ct_5361t_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/comtrend/test_ct_5361t_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dcs_930l_auth_rce.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dcs_930l_auth_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_300_320_600_615_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_300_320_600_615_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_300_320_615_auth_bypass.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_300_320_615_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_300_600_rce.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_300_600_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_300_645_815_upnp_rce.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_300_645_815_upnp_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_645_815_rce.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_645_815_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_645_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_645_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_815_850l_rce.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_815_850l_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_825_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_825_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_850l_creds_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_850l_creds_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dir_8xx_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dir_8xx_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dns_320l_327l_rce.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dns_320l_327l_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dsl_2730_2750_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dsl_2730_2750_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dsl_2730b_2780b_526b_dns_change.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dsl_2730b_2780b_526b_dns_change.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dsl_2750b_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dsl_2750b_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dsl_2750b_rce.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dsl_2750b_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dsp_w110_rce.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dsp_w110_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dvg_n5402sp_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dvg_n5402sp_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dwl_3200ap_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dwl_3200ap_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dwr_932_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dwr_932_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_dwr_932b_backdoor.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_dwr_932b_backdoor.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_multi_hedwig_cgi_exec.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_multi_hedwig_cgi_exec.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/dlink/test_multi_hnap_rce.py` & `routersploit-3.4.3/tests/exploits/routers/dlink/test_multi_hnap_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/huawei/test_e5331_mifi_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/huawei/test_e5331_mifi_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/huawei/test_hg520_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/huawei/test_hg520_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/huawei/test_hg530_hg520b_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/huawei/test_hg530_hg520b_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/huawei/test_hg866_password_change.py` & `routersploit-3.4.3/tests/exploits/routers/huawei/test_hg866_password_change.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/ipfire/test_ipfire_proxy_rce.py` & `routersploit-3.4.3/tests/exploits/routers/ipfire/test_ipfire_proxy_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/ipfire/test_ipfire_shellshock.py` & `routersploit-3.4.3/tests/exploits/routers/ipfire/test_ipfire_shellshock.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/linksys/test_1500_2500_rce.py` & `routersploit-3.4.3/tests/exploits/routers/linksys/test_1500_2500_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/linksys/test_eseries_themoon_rce.py` & `routersploit-3.4.3/tests/exploits/routers/linksys/test_eseries_themoon_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/linksys/test_smartwifi_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/linksys/test_smartwifi_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/linksys/test_wap54gv3_rce.py` & `routersploit-3.4.3/tests/exploits/routers/linksys/test_wap54gv3_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/linksys/test_wrt100_110_rce.py` & `routersploit-3.4.3/tests/exploits/routers/linksys/test_wrt100_110_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/mikrotik/test_winbox_auth_bypass_creds_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/mikrotik/test_winbox_auth_bypass_creds_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/movistar/test_adsl_router_bhs_rta_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/movistar/test_adsl_router_bhs_rta_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/multi/test_gpon_home_gateway_rce.py` & `routersploit-3.4.3/tests/exploits/routers/multi/test_gpon_home_gateway_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/multi/test_misfortune_cookie.py` & `routersploit-3.4.3/tests/exploits/routers/multi/test_misfortune_cookie.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/multi/test_rom0.py` & `routersploit-3.4.3/tests/exploits/routers/multi/test_rom0.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/multi/test_tcp_32764_info_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/multi/test_tcp_32764_info_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/multi/test_tcp_32764_rce.py` & `routersploit-3.4.3/tests/exploits/routers/multi/test_tcp_32764_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/netcore/test_udp_53413_rce.py` & `routersploit-3.4.3/tests/exploits/routers/netcore/test_udp_53413_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/netgear/test_dgn2200_ping_cgi_rce.py` & `routersploit-3.4.3/tests/exploits/routers/netgear/test_dgn2200_ping_cgi_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/netgear/test_jnr1010_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/netgear/test_jnr1010_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/netgear/test_n300_auth_bypass.py` & `routersploit-3.4.3/tests/exploits/routers/netgear/test_n300_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/netgear/test_netgear_multi_rce.py` & `routersploit-3.4.3/tests/exploits/routers/netgear/test_netgear_multi_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/netgear/test_prosafe_rce.py` & `routersploit-3.4.3/tests/exploits/routers/netgear/test_prosafe_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/netgear/test_r7000_r6400_rce.py` & `routersploit-3.4.3/tests/exploits/routers/netgear/test_r7000_r6400_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/netgear/test_wnr500_612v3_jnr1010_2010_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/netgear/test_wnr500_612v3_jnr1010_2010_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/netsys/test_multi_rce.py` & `routersploit-3.4.3/tests/exploits/routers/netsys/test_multi_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/shuttle/test_915wm_dns_change.py` & `routersploit-3.4.3/tests/exploits/routers/shuttle/test_915wm_dns_change.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/technicolor/test_dwg855_authbypass.py` & `routersploit-3.4.3/tests/exploits/routers/technicolor/test_dwg855_authbypass.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/technicolor/test_tc7200_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/technicolor/test_tc7200_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/technicolor/test_tc7200_password_disclosure_v2.py` & `routersploit-3.4.3/tests/exploits/routers/technicolor/test_tc7200_password_disclosure_v2.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/thomson/test_twg850_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/thomson/test_twg850_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/tplink/test_archer_c2_c20i_rce.py` & `routersploit-3.4.3/tests/exploits/routers/tplink/test_archer_c2_c20i_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/tplink/test_wdr740nd_wdr740n_backdoor.py` & `routersploit-3.4.3/tests/exploits/routers/tplink/test_wdr740nd_wdr740n_backdoor.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/tplink/test_wdr740nd_wdr740n_path_traversal.py` & `routersploit-3.4.3/tests/exploits/routers/tplink/test_wdr740nd_wdr740n_path_traversal.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/tplink/test_wdr842nd_wdr842n_configure_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/tplink/test_wdr842nd_wdr842n_configure_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/zte/test_f460_f660_backdoor.py` & `routersploit-3.4.3/tests/exploits/routers/zte/test_f460_f660_backdoor.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/zte/test_zxhn_h108n_wifi_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/zte/test_zxhn_h108n_wifi_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/zte/test_zxv10_rce.py` & `routersploit-3.4.3/tests/exploits/routers/zte/test_zxv10_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/zyxel/test_d1000_rce.py` & `routersploit-3.4.3/tests/exploits/routers/zyxel/test_d1000_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/zyxel/test_d1000_wifi_password_disclosure.py` & `routersploit-3.4.3/tests/exploits/routers/zyxel/test_d1000_wifi_password_disclosure.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/zyxel/test_p660hn_t_v1_rce.py` & `routersploit-3.4.3/tests/exploits/routers/zyxel/test_p660hn_t_v1_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/zyxel/test_p660hn_t_v2_rce.py` & `routersploit-3.4.3/tests/exploits/routers/zyxel/test_p660hn_t_v2_rce.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/exploits/routers/zyxel/test_zywall_usg_extract_hashes.py` & `routersploit-3.4.3/tests/exploits/routers/zyxel/test_zywall_usg_extract_hashes.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/armle/test_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/armle/test_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/armle/test_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/armle/test_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/cmd/test_perl_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/cmd/test_perl_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/cmd/test_perl_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/cmd/test_perl_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/cmd/test_php_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/cmd/test_php_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/cmd/test_php_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/cmd/test_php_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/cmd/test_python_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/cmd/test_python_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/cmd/test_python_bind_udp.py` & `routersploit-3.4.3/tests/payloads/cmd/test_python_bind_udp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/cmd/test_python_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/cmd/test_python_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/cmd/test_python_reverse_udp.py` & `routersploit-3.4.3/tests/payloads/cmd/test_python_reverse_udp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/mipsbe/test_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/mipsbe/test_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/mipsbe/test_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/mipsbe/test_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/mipsle/test_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/mipsle/test_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/mipsle/test_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/mipsle/test_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/php/test_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/php/test_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/php/test_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/php/test_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/python/test_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/python/test_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/python/test_bind_udp.py` & `routersploit-3.4.3/tests/payloads/python/test_bind_udp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/python/test_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/python/test_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/python/test_reverse_udp.py` & `routersploit-3.4.3/tests/payloads/python/test_reverse_udp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/x64/test_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/x64/test_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/x64/test_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/x64/test_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/x86/test_bind_tcp.py` & `routersploit-3.4.3/tests/payloads/x86/test_bind_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/payloads/x86/test_reverse_tcp.py` & `routersploit-3.4.3/tests/payloads/x86/test_reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/test_exploit_scenarios.py` & `routersploit-3.4.3/tests/test_exploit_scenarios.py`

 * *Files identical despite different names*

### Comparing `routersploit-3.4.2/tests/test_module_info.py` & `routersploit-3.4.3/tests/test_module_info.py`

 * *Files identical despite different names*

