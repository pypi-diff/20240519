# Comparing `tmp/pymscada-0.1.0a6.tar.gz` & `tmp/pymscada-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymscada-0.1.0a6.tar", last modified: Thu Mar 28 21:44:51 2024, max compression
+gzip compressed data, was "pymscada-0.1.1a2.tar", last modified: Sun May 19 09:20:08 2024, max compression
```

## Comparing `pymscada-0.1.0a6.tar` & `pymscada-0.1.1a2.tar`

### file list

```diff
@@ -1,77 +1,82 @@
--rw-r--r--   0        0        0    35149 2024-03-11 18:47:50.842266 pymscada-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     2464 2024-03-11 18:47:50.842266 pymscada-0.1.0a6/README.md
--rw-r--r--   0        0        0     1105 2024-03-28 21:44:51.166891 pymscada-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0      653 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/__init__.py
--rw-r--r--   0        0        0      272 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/__main__.py
--rw-r--r--   0        0        0     8695 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/bus_client.py
--rw-r--r--   0        0        0    11255 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/bus_server.py
--rw-r--r--   0        0        0     3351 2024-03-28 20:57:42.947538 pymscada-0.1.0a6/src/pymscada/checkout.py
--rw-r--r--   0        0        0     1851 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/config.py
--rw-r--r--   0        0        0      946 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/console.py
--rw-r--r--   0        0        0      880 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/README.md
--rw-r--r--   0        0        0       29 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/__init__.py
--rw-r--r--   0        0        0       26 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/bus.yaml
--rw-r--r--   0        0        0      169 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/files.yaml
--rw-r--r--   0        0        0       46 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/history.yaml
--rw-r--r--   0        0        0      912 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/logixclient.yaml
--rw-r--r--   0        0        0     2397 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/modbus_plc.py
--rw-r--r--   0        0        0     1099 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/modbusclient.yaml
--rw-r--r--   0        0        0     1133 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/modbusserver.yaml
--rw-r--r--   0        0        0      210 2024-03-28 20:57:42.947538 pymscada-0.1.0a6/src/pymscada/demo/ping.yaml
--rw-r--r--   0        0        0      257 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/pymscada-bus.service
--rw-r--r--   0        0        0      316 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/pymscada-demo-modbus_plc.service
--rw-r--r--   0        0        0      322 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/pymscada-files.service
--rw-r--r--   0        0        0      382 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/pymscada-history.service
--rw-r--r--   0        0        0      344 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/pymscada-io-logixclient.service
--rw-r--r--   0        0        0      344 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/pymscada-io-modbusclient.service
--rw-r--r--   0        0        0      344 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/pymscada-io-modbusserver.service
--rw-r--r--   0        0        0      327 2024-03-28 20:57:42.951538 pymscada-0.1.0a6/src/pymscada/demo/pymscada-io-ping.service
--rw-r--r--   0        0        0      339 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/pymscada-io-snmpclient.service
--rw-r--r--   0        0        0      366 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/pymscada-wwwserver.service
--rw-r--r--   0        0        0     2013 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/demo/snmpclient.yaml
--rw-r--r--   0        0        0     4231 2024-03-28 20:57:42.955538 pymscada-0.1.0a6/src/pymscada/demo/tags.yaml
--rw-r--r--   0        0        0    12493 2024-03-28 20:57:42.955538 pymscada-0.1.0a6/src/pymscada/demo/wwwserver.yaml
--rw-r--r--   0        0        0     1784 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/files.py
--rw-r--r--   0        0        0     9455 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/history.py
--rw-r--r--   0        0        0        0 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/iodrivers/__init__.py
--rw-r--r--   0        0        0     2806 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/iodrivers/logix_client.py
--rw-r--r--   0        0        0     5401 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/iodrivers/logix_map.py
--rw-r--r--   0        0        0     9529 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/iodrivers/modbus_client.py
--rw-r--r--   0        0        0     7172 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/iodrivers/modbus_map.py
--rw-r--r--   0        0        0     6507 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/iodrivers/modbus_server.py
--rw-r--r--   0        0        0     4166 2024-03-28 20:57:42.955538 pymscada-0.1.0a6/src/pymscada/iodrivers/ping_client.py
--rw-r--r--   0        0        0     1403 2024-03-28 20:57:42.955538 pymscada-0.1.0a6/src/pymscada/iodrivers/ping_map.py
--rw-r--r--   0        0        0     2601 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/iodrivers/snmp_client.py
--rw-r--r--   0        0        0     2369 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/iodrivers/snmp_map.py
--rw-r--r--   0        0        0     5998 2024-03-28 20:57:42.959538 pymscada-0.1.0a6/src/pymscada/main.py
--rw-r--r--   0        0        0      622 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/misc.py
--rw-r--r--   0        0        0       29 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/pdf/__init__.py
--rw-r--r--   0        0        0     1488 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/pdf/one.pdf
--rw-r--r--   0        0        0     1516 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/pdf/two.pdf
--rw-r--r--   0        0        0     1235 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/periodic.py
--rw-r--r--   0        0        0     1997 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/protocol_constants.py
--rw-r--r--   0        0        0     2583 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/samplers.py
--rw-r--r--   0        0        0     9463 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/tag.py
--rw-r--r--   0        0        0     1675 2024-03-28 20:57:42.959538 pymscada-0.1.0a6/src/pymscada/tools/snmp_client2.py
--rw-r--r--   0        0        0     1625 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/tools/walk.py
--rw-r--r--   0        0        0    13125 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/validate.py
--rw-r--r--   0        0        0    11473 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/src/pymscada/www_server.py
--rw-r--r--   0        0        0       13 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/__init__.py
--rw-r--r--   0        0        0     1259 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/bus_echo.py
--rw-r--r--   0        0        0     3827 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/iodrivers/test_logix.py
--rw-r--r--   0        0        0     4517 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/iodrivers/test_modbus.py
--rw-r--r--   0        0        0       25 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/test_assets/busserver.yaml
--rw-r--r--   0        0        0      240 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/test_assets/hist_tag_0_0.dat
--rw-r--r--   0        0        0        0 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/test_assets/hist_tag_0_10_2.dat
--rw-r--r--   0        0        0      176 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/test_assets/hist_tag_0_15.dat
--rw-r--r--   0        0        0      384 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/test_assets/hist_tag_0_26.dat
--rw-r--r--   0        0        0      160 2024-03-11 18:47:50.846266 pymscada-0.1.0a6/tests/test_assets/hist_tag_0_50.dat
--rw-r--r--   0        0        0    10782 2024-03-11 18:47:50.850266 pymscada-0.1.0a6/tests/test_bus_server.py
--rw-r--r--   0        0        0      669 2024-03-11 18:47:50.850266 pymscada-0.1.0a6/tests/test_config.py
--rw-r--r--   0        0        0      719 2024-03-11 18:47:50.850266 pymscada-0.1.0a6/tests/test_misc.py
--rw-r--r--   0        0        0      964 2024-03-11 18:47:50.850266 pymscada-0.1.0a6/tests/test_periodic.py
--rw-r--r--   0        0        0     1104 2024-03-11 18:47:50.850266 pymscada-0.1.0a6/tests/test_samplers.py
--rw-r--r--   0        0        0     5548 2024-03-11 18:47:50.850266 pymscada-0.1.0a6/tests/test_tag.py
--rw-r--r--   0        0        0     6078 2024-03-11 18:47:50.850266 pymscada-0.1.0a6/tests/test_tag_history.py
--rw-r--r--   0        0        0      233 2024-03-11 18:47:50.850266 pymscada-0.1.0a6/tests/test_validate.py
--rw-r--r--   0        0        0     3216 1970-01-01 00:00:00.000000 pymscada-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-11 18:47:50.842266 pymscada-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0     2464 2024-03-11 18:47:50.842266 pymscada-0.1.1a2/README.md
+-rw-r--r--   0        0        0     1103 2024-05-19 09:20:08.314233 pymscada-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0      653 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/__init__.py
+-rw-r--r--   0        0        0      272 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/__main__.py
+-rw-r--r--   0        0        0     8884 2024-05-07 18:36:35.801103 pymscada-0.1.1a2/src/pymscada/bus_client.py
+-rw-r--r--   0        0        0    11544 2024-05-06 18:34:41.345807 pymscada-0.1.1a2/src/pymscada/bus_server.py
+-rw-r--r--   0        0        0     3351 2024-03-28 20:57:42.947538 pymscada-0.1.1a2/src/pymscada/checkout.py
+-rw-r--r--   0        0        0     1851 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/config.py
+-rw-r--r--   0        0        0     8011 2024-05-19 09:17:19.996214 pymscada-0.1.1a2/src/pymscada/console.py
+-rw-r--r--   0        0        0      880 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/README.md
+-rw-r--r--   0        0        0       29 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/__init__.py
+-rw-r--r--   0        0        0       26 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/bus.yaml
+-rw-r--r--   0        0        0      197 2024-04-20 02:06:25.201818 pymscada-0.1.1a2/src/pymscada/demo/files.yaml
+-rw-r--r--   0        0        0       46 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/history.yaml
+-rw-r--r--   0        0        0      912 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/logixclient.yaml
+-rw-r--r--   0        0        0     2397 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/modbus_plc.py
+-rw-r--r--   0        0        0     1099 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/modbusclient.yaml
+-rw-r--r--   0        0        0     1133 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/modbusserver.yaml
+-rw-r--r--   0        0        0      111 2024-04-28 03:27:06.732698 pymscada-0.1.1a2/src/pymscada/demo/opnotes.yaml
+-rw-r--r--   0        0        0      210 2024-03-28 20:57:42.947538 pymscada-0.1.1a2/src/pymscada/demo/ping.yaml
+-rw-r--r--   0        0        0      257 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/pymscada-bus.service
+-rw-r--r--   0        0        0      316 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/pymscada-demo-modbus_plc.service
+-rw-r--r--   0        0        0      322 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/pymscada-files.service
+-rw-r--r--   0        0        0      382 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/pymscada-history.service
+-rw-r--r--   0        0        0      344 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/pymscada-io-logixclient.service
+-rw-r--r--   0        0        0      344 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/pymscada-io-modbusclient.service
+-rw-r--r--   0        0        0      344 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/pymscada-io-modbusserver.service
+-rw-r--r--   0        0        0      327 2024-03-28 20:57:42.951538 pymscada-0.1.1a2/src/pymscada/demo/pymscada-io-ping.service
+-rw-r--r--   0        0        0      339 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/pymscada-io-snmpclient.service
+-rw-r--r--   0        0        0      350 2024-05-06 18:20:51.032565 pymscada-0.1.1a2/src/pymscada/demo/pymscada-opnotes.service
+-rw-r--r--   0        0        0      366 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/pymscada-wwwserver.service
+-rw-r--r--   0        0        0     2013 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/demo/snmpclient.yaml
+-rw-r--r--   0        0        0     4231 2024-03-28 20:57:42.955538 pymscada-0.1.1a2/src/pymscada/demo/tags.yaml
+-rw-r--r--   0        0        0    12543 2024-04-20 02:51:52.134070 pymscada-0.1.1a2/src/pymscada/demo/wwwserver.yaml
+-rw-r--r--   0        0        0     2439 2024-05-07 09:29:48.993848 pymscada-0.1.1a2/src/pymscada/files.py
+-rw-r--r--   0        0        0     9504 2024-05-07 09:30:47.170725 pymscada-0.1.1a2/src/pymscada/history.py
+-rw-r--r--   0        0        0        0 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/iodrivers/__init__.py
+-rw-r--r--   0        0        0     2829 2024-05-07 09:31:36.215235 pymscada-0.1.1a2/src/pymscada/iodrivers/logix_client.py
+-rw-r--r--   0        0        0     5401 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/iodrivers/logix_map.py
+-rw-r--r--   0        0        0     9592 2024-05-07 09:32:09.463498 pymscada-0.1.1a2/src/pymscada/iodrivers/modbus_client.py
+-rw-r--r--   0        0        0     7255 2024-03-30 04:44:50.599889 pymscada-0.1.1a2/src/pymscada/iodrivers/modbus_map.py
+-rw-r--r--   0        0        0     6570 2024-05-07 09:32:27.991623 pymscada-0.1.1a2/src/pymscada/iodrivers/modbus_server.py
+-rw-r--r--   0        0        0     4188 2024-05-07 09:32:48.791748 pymscada-0.1.1a2/src/pymscada/iodrivers/ping_client.py
+-rw-r--r--   0        0        0     1403 2024-03-28 20:57:42.955538 pymscada-0.1.1a2/src/pymscada/iodrivers/ping_map.py
+-rw-r--r--   0        0        0     2623 2024-05-07 09:33:08.111851 pymscada-0.1.1a2/src/pymscada/iodrivers/snmp_client.py
+-rw-r--r--   0        0        0     2369 2024-03-30 04:44:50.599889 pymscada-0.1.1a2/src/pymscada/iodrivers/snmp_map.py
+-rw-r--r--   0        0        0     8097 2024-05-18 00:36:46.922222 pymscada-0.1.1a2/src/pymscada/main.py
+-rw-r--r--   0        0        0      622 2024-05-12 02:29:33.647803 pymscada-0.1.1a2/src/pymscada/misc.py
+-rw-r--r--   0        0        0     4377 2024-05-07 09:51:16.616213 pymscada-0.1.1a2/src/pymscada/opnotes.py
+-rw-r--r--   0        0        0       29 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/pdf/__init__.py
+-rw-r--r--   0        0        0     1488 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/pdf/one.pdf
+-rw-r--r--   0        0        0     1516 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/pdf/two.pdf
+-rw-r--r--   0        0        0     1235 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/periodic.py
+-rw-r--r--   0        0        0     2094 2024-05-06 18:31:04.906327 pymscada-0.1.1a2/src/pymscada/protocol_constants.py
+-rw-r--r--   0        0        0     2583 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/samplers.py
+-rw-r--r--   0        0        0    10095 2024-05-12 02:30:20.048693 pymscada-0.1.1a2/src/pymscada/tag.py
+-rw-r--r--   0        0        0     1675 2024-03-28 20:57:42.959538 pymscada-0.1.1a2/src/pymscada/tools/snmp_client2.py
+-rw-r--r--   0        0        0     1625 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/tools/walk.py
+-rw-r--r--   0        0        0    13125 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/src/pymscada/validate.py
+-rw-r--r--   0        0        0    11465 2024-05-18 17:38:35.589343 pymscada-0.1.1a2/src/pymscada/www_server.py
+-rw-r--r--   0        0        0       13 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/tests/__init__.py
+-rw-r--r--   0        0        0     1259 2024-04-26 23:49:30.963430 pymscada-0.1.1a2/tests/bus_echo.py
+-rw-r--r--   0        0        0     3827 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/tests/iodrivers/test_logix.py
+-rw-r--r--   0        0        0     4517 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/tests/iodrivers/test_modbus.py
+-rw-r--r--   0        0        0       25 2024-03-11 18:47:50.846266 pymscada-0.1.1a2/tests/test_assets/busserver.yaml
+-rw-r--r--   0        0        0     8192 2024-05-06 18:07:50.000101 pymscada-0.1.1a2/tests/test_assets/db.sqlite
+-rw-r--r--   0        0        0      240 2024-05-03 22:45:32.184176 pymscada-0.1.1a2/tests/test_assets/hist_tag_0_0.dat
+-rw-r--r--   0        0        0        0 2024-05-03 22:45:32.188176 pymscada-0.1.1a2/tests/test_assets/hist_tag_0_10_2.dat
+-rw-r--r--   0        0        0      176 2024-05-03 22:45:32.184176 pymscada-0.1.1a2/tests/test_assets/hist_tag_0_15.dat
+-rw-r--r--   0        0        0      384 2024-05-03 22:45:32.188176 pymscada-0.1.1a2/tests/test_assets/hist_tag_0_26.dat
+-rw-r--r--   0        0        0      160 2024-05-03 22:45:38.556272 pymscada-0.1.1a2/tests/test_assets/hist_tag_0_50.dat
+-rw-r--r--   0        0        0    10835 2024-05-03 23:55:18.610297 pymscada-0.1.1a2/tests/test_bus_server.py
+-rw-r--r--   0        0        0      669 2024-03-11 18:47:50.850266 pymscada-0.1.1a2/tests/test_config.py
+-rw-r--r--   0        0        0     6078 2024-04-26 23:50:43.356643 pymscada-0.1.1a2/tests/test_history.py
+-rw-r--r--   0        0        0      719 2024-03-11 18:47:50.850266 pymscada-0.1.1a2/tests/test_misc.py
+-rw-r--r--   0        0        0     2395 2024-05-06 18:07:40.463947 pymscada-0.1.1a2/tests/test_opnotes.py
+-rw-r--r--   0        0        0      964 2024-03-11 18:47:50.850266 pymscada-0.1.1a2/tests/test_periodic.py
+-rw-r--r--   0        0        0     1104 2024-03-11 18:47:50.850266 pymscada-0.1.1a2/tests/test_samplers.py
+-rw-r--r--   0        0        0     5548 2024-03-11 18:47:50.850266 pymscada-0.1.1a2/tests/test_tag.py
+-rw-r--r--   0        0        0      233 2024-03-11 18:47:50.850266 pymscada-0.1.1a2/tests/test_validate.py
+-rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 pymscada-0.1.1a2/PKG-INFO
```

### Comparing `pymscada-0.1.0a6/LICENSE` & `pymscada-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/README.md` & `pymscada-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/pyproject.toml` & `pymscada-0.1.1a2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "pymscada"
-version = "0.1.0a6"
+version = "0.1.1a2"
 description = "Shared tag value SCADA with python backup and Angular UI"
 authors = [
     { name = "Jamie Walton", email = "jamie@walton.net.nz" },
 ]
 dependencies = [
     "PyYAML>=6.0.1",
     "aiohttp>=3.8.5",
-    "pymscada-html==0.1.0a1",
+    "pymscada-html==0.1.0",
     "cerberus>=1.3.5",
     "pycomm3>=1.2.14",
     "pysnmplib>=5.0.24",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
```

### Comparing `pymscada-0.1.0a6/src/pymscada/__init__.py` & `pymscada-0.1.1a2/src/pymscada/__init__.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/bus_client.py` & `pymscada-0.1.1a2/src/pymscada/bus_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,26 @@
     """
     Connects to a Bus Server.
 
     await client.connect() to make the connection. If bus server connection
     fails, die.
     """
 
-    def __init__(self, ip: str = '127.0.0.1', port: int = 1324, tag_info=None):
+    def __init__(self, ip: str = '127.0.0.1', port: int = 1324, tag_info=None,
+                 module: str = '_unset_'):
         """Create bus server."""
         self.ip = ip
         self.port = port
         self.read_task = None
         self.tag_info = tag_info
+        self.module = module
         self.tag_by_id: dict[int, Tag] = {}
         self.tag_by_name: dict[str, Tag] = {}
         self.to_publish: dict[str, Tag] = {}
-        self.rqs_handlers: dict[str, object] = {}
+        self.rta_handlers: dict[str, object] = {}
         self.pending = {}
 
     def publish(self, tag: Tag):
         """
         Update bus server with tag value change.
 
         A tag is given bus_id id(self) when set from bus. Don't publish to
@@ -57,28 +59,28 @@
             size = len(jsonstr)
             data = struct.pack(f'!B{size}s', pc.TYPE_JSON, jsonstr)
         else:
             logging.warning(f'publish {tag.name} unhandled {tag.type}')
             return
         self.write(pc.CMD_SET, tag.id, tag.time_us, data)
 
-    def add_callback_rqs(self, tagname, handler):
+    def add_callback_rta(self, tagname, handler):
         """Collect callback handlers."""
         if callable(handler):
-            self.rqs_handlers[tagname] = handler
+            self.rta_handlers[tagname] = handler
         else:
-            logging.error(f'invalid RQS handler for {tagname}')
+            logging.error(f'invalid RTA handler for {tagname}')
 
-    def rqs(self, tagname: str, request: dict):
+    def rta(self, tagname: str, request: dict):
         """Send a Request Set message."""
         time_us = int(time.time() * 1e6)
         jsonstr = json.dumps(request).encode()
         size = len(jsonstr)
         data = struct.pack(f'>B{size}s', pc.TYPE_JSON, jsonstr)
-        self.write(pc.CMD_RQS, self.tag_by_name[tagname].id, time_us, data)
+        self.write(pc.CMD_RTA, self.tag_by_name[tagname].id, time_us, data)
 
     def write(self, command: pc.COMMANDS, tag_id: int, time_us: int,
               data: bytes):
         """Write a message."""
         if data is None:
             data = b''
         for i in range(0, len(data) + 1, pc.MAX_LEN):
@@ -102,14 +104,15 @@
         self.write(pc.CMD_ID, 0, 0, tag.name.encode())
 
     async def open_connection(self):
         """Establish connection and callbacks."""
         self.reader, self.writer = await asyncio.open_connection(
             self.ip, self.port)
         self.addr = self.writer.get_extra_info('sockname')
+        self.write(pc.CMD_LOG, 0, 0, f'{self.module} connected'.encode())
         logging.info(f'connected {self.addr}')
         for tag in Tag.get_all_tags().values():
             self.add_tag(tag)
         Tag.set_notify(self.add_tag)
 
     async def close_connection(self):
         """Close connection and remove callbacks."""
@@ -123,15 +126,16 @@
     async def read(self):
         """Read forever."""
         await self.open_connection()
         while True:
             try:
                 head = await self.reader.readexactly(14)
                 _, cmd, tag_id, size, time_us = struct.unpack('>BBHHQ', head)
-            except (ConnectionResetError, asyncio.IncompleteReadError):
+            except (ConnectionResetError, asyncio.IncompleteReadError,
+                    asyncio.CancelledError):
                 break
             if size == 0:
                 self.process(cmd, tag_id, time_us, None)
                 continue
             try:
                 payload = await self.reader.readexactly(size)
                 data = struct.unpack(f'>{size}s', payload)[0]
@@ -196,22 +200,22 @@
                 data = json.loads(struct.unpack_from(f'!{len(value) - 1}s',
                                                      value, offset=1
                                                      )[0].decode())
             else:
                 logging.warning(f'process error {tag.name} {tag.type} {value}')
                 return
             tag.value = data, time_us, id(self)
-        elif cmd == pc.CMD_RQS:
+        elif cmd == pc.CMD_RTA:
             data = struct.unpack_from(f'!{len(value) - 1}s', value, offset=1
                                       )[0].decode()
             data = json.loads(data)
             try:
-                self.rqs_handlers[tag.name](data)
+                self.rta_handlers[tag.name](data)
             except KeyError:
-                logging.warning(f'unhandled RQS for {tag.name} {data}')
+                logging.warning(f'unhandled RTA for {tag.name} {data}')
         else:
             raise SystemExit(f'Invalid message {cmd}')
 
     async def shutdown(self):
         """Shutdown starts with closing the writer."""
         self.writer.close()
         await self.writer.wait_closed()
```

### Comparing `pymscada-0.1.0a6/src/pymscada/bus_server.py` & `pymscada-0.1.1a2/src/pymscada/bus_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,34 +137,35 @@
         # on broken connection
         self.read_callback((bus_id, None, 0, 0, None))
 
 
 class BusServer:
     """Serve Tags on ip:port, echoing changes to any subscribers."""
 
-    __slots__ = ('ip', 'port', 'server', 'connections')
+    __slots__ = ('ip', 'port', 'server', 'connections', 'bus_tag')
 
-    def __init__(self, ip: str = '127.0.0.1', port: int = 1324):
+    def __init__(self, ip: str = '127.0.0.1', port: int = 1324,
+                 bus_tag: str = '__bus__'):
         """
         Serve Tags on ip:port, echoing changes to any subscribers.
 
         Each connection can publish and subscribe to tags. Any tag set is
         broadcast to any listeners excepting the connection that sets the
         tag value.
 
         Event loop must be running.
         """
         self.ip = ip
         self.port = port
         self.server = None
         self.connections: dict[int, BusConnection] = {}
-        bus_tag = BusTag(b'__bus__')
-        bus_tag.value = b'\x03started'  # \x03 is string type
-        bus_tag.time_us = int(time.time() * 1e6)
-        bus_tag.from_bus = 0
+        self.bus_tag = BusTag(bus_tag.encode())
+        self.bus_tag.value = b'\x03started'  # \x03 is string type
+        self.bus_tag.time_us = int(time.time() * 1e6)
+        self.bus_tag.from_bus = 0
 
     def publish(self, tag: BusTag, bus_id):
         """Update subcribers with tag value change."""
         if tag.from_bus == bus_id:
             return
         try:
             self.connections[bus_id].write(pc.CMD_SET, tag.id, tag.time_us,
@@ -180,30 +181,30 @@
             try:
                 tag = BusTags._tag_by_id[tag_id]
                 tag.update(data, time_us, bus_id)
             except KeyError:
                 self.connections[bus_id].write(
                     pc.CMD_ERR, tag_id, time_us,
                     f"SET KeyError {tag_id}".encode())
-        elif cmd == pc.CMD_RQS:
+        elif cmd == pc.CMD_RTA:
             try:
                 tag = BusTags._tag_by_id[tag_id]
             except KeyError:
                 self.connections[bus_id].write(
                     pc.CMD_ERR, tag_id, time_us,
-                    f"RQS KeyError {tag_id}".encode())
+                    f"RTA KeyError {tag_id}".encode())
             try:
                 self.connections[tag.from_bus].write(
-                    pc.CMD_RQS, tag_id, tag.time_us, data)
+                    pc.CMD_RTA, tag_id, tag.time_us, data)
             except KeyError:
                 logging.warning(f'likely busclient for {tag.name} is gone')
             except Exception as e:
                 self.connections[bus_id].write(
                     pc.CMD_ERR, tag_id, time_us,
-                    f"RQS {tag_id} {e}".encode())
+                    f"RTA {tag_id} {e}".encode())
             """Reply comes from another BusClient, not the Server."""
         elif cmd == pc.CMD_SUB:
             try:
                 tag = BusTags._tag_by_id[tag_id]
             except KeyError:
                 self.connections[bus_id].write(
                     pc.CMD_ERR, tag_id, time_us,
@@ -256,14 +257,19 @@
                         tagname_list.append(tag.name)
             else:
                 for _, tag in BusTags._tag_by_id.items():
                     if data in tag.name:
                         tagname_list.append(tag.name)
             self.connections[bus_id].write(
                 pc.CMD_LIST, 0, time_us, b' '.join(tagname_list))
+        elif cmd == pc.CMD_LOG:
+            if len(data) > 300:
+                logging.warning(f'process: log message too long from {bus_id}')
+            else:
+                logging.warning(data.decode())
         else:  # consider disconnecting
             logging.warn(f'invalid message {cmd}')
 
     def read_callback(self, command):
         """Process read messages, delete broken connections."""
         bus_id, cmd, tag_id, time_us, data = command
         if cmd is None:
```

### Comparing `pymscada-0.1.0a6/src/pymscada/checkout.py` & `pymscada-0.1.1a2/src/pymscada/checkout.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/config.py` & `pymscada-0.1.1a2/src/pymscada/config.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/demo/README.md` & `pymscada-0.1.1a2/src/pymscada/demo/README.md`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/demo/logixclient.yaml` & `pymscada-0.1.1a2/src/pymscada/demo/logixclient.yaml`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/demo/modbus_plc.py` & `pymscada-0.1.1a2/src/pymscada/demo/modbus_plc.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/demo/modbusclient.yaml` & `pymscada-0.1.1a2/src/pymscada/demo/modbusclient.yaml`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/demo/modbusserver.yaml` & `pymscada-0.1.1a2/src/pymscada/demo/modbusserver.yaml`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/demo/snmpclient.yaml` & `pymscada-0.1.1a2/src/pymscada/demo/snmpclient.yaml`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/demo/tags.yaml` & `pymscada-0.1.1a2/src/pymscada/demo/tags.yaml`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/demo/wwwserver.yaml` & `pymscada-0.1.1a2/src/pymscada/demo/wwwserver.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 bus_ip: 127.0.0.1
 bus_port: 1324
 ip: 0.0.0.0
 port: 8324
-get_path:
-paths:
-- history
-- config
-- pdf
+get_path: /home/mscada/Documents/angmscada/dist/angmscada
+serve_path: /home/mscada/pymscada
 pages:
 - name: Default Main
   parent:
   items:
   - {desc: Default tags, type: h1}
   - {tagname: IntSet, type: setpoint}
   - {tagname: IntVal, type: value}
```

### Comparing `pymscada-0.1.0a6/src/pymscada/history.py` & `pymscada-0.1.1a2/src/pymscada/history.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             tag = super().__new__(cls)
             tag.__init__(tagname, tagtype, path, **kwds)
             cls._tags[tagname] = tag
         return cls._tags[tagname]
 
     def __init__(self, tagname: str, tagtype, path: str,
                  min=None, max=None, deadband=None):
-        """Create persistent tag store. Respond to RQS."""
+        """Create persistent tag store. Respond to RTA."""
         self.name = tagname
         if type(tagtype) is type:
             self.type = tagtype
         else:
             self.type = TYPES[tagtype]
         if tagtype is int:
             self.packstr = '!Qq'
@@ -185,70 +185,71 @@
         self.append(tag.time_us, tag.value)
 
 
 class History():
     """Connect to bus_ip:bus_port, store and provide a value history."""
 
     def __init__(self, bus_ip: str = '127.0.0.1', bus_port: int = 1324,
-                 path: str = 'history', tag_info: dict = {}) -> None:
+                 path: str = 'history', tag_info: dict = {},
+                 rta_tag: str = '__history__') -> None:
         """
         Connect to bus_ip:bus_port, store and provide a value history.
 
         History files are binary files named <tagname>_<time_us>.dat. On
-        receipt of a request via RQS message, History will send the data
-        via __history__.value which you can watch with a tag.add_callback.
+        receipt of a request via RTA message, History will send the data
+        via rta_tag.value which you can watch with a tag.add_callback.
 
         Event loop must be running.
         """
-        self.busclient = BusClient(bus_ip, bus_port)
+        self.busclient = BusClient(bus_ip, bus_port, module='History')
         self.path = path
         self.tags: dict[str, Tag] = {}
         self.hist_tags: dict[str, TagHistory] = {}
         for tagname, tag in tag_info.items():
             tag_for_history(tagname, tag)
             if tag['type'] not in [float, int]:
                 continue
             self.hist_tags[tagname] = TagHistory(
                 tagname, tag['type'], path, min=tag['min'], max=tag['max'],
                 deadband=tag['deadband'])
             self.tags[tagname] = Tag(tagname, tag['type'])
             self.tags[tagname].add_callback(self.hist_tags[tagname].callback)
-        self.rqs = Tag('__history__', bytes)
-        self.rqs.value = b'\x00\x00\x00\x00\x00\x00'
-        self.busclient.add_callback_rqs('__history__', self.rqs_cb)
+        self.rta = Tag(rta_tag, bytes)
+        self.rta.value = b'\x00\x00\x00\x00\x00\x00'
+        self.busclient.add_callback_rta(rta_tag, self.rta_cb)
 
-    def rqs_cb(self, request):
-        """Respond to bus requests for data to publish on rqs."""
+    def rta_cb(self, request):
+        """Respond to bus requests for data to publish on rta."""
         if 'start_ms' in request:
             request['start_us'] = request['start_ms'] * 1000
             request['end_us'] = request['end_ms'] * 1000
-        rqs_id = 0
-        if '__rqs_id__' in request:
-            rqs_id = request['__rqs_id__']
+        rta_id = 0
+        if '__rta_id__' in request:
+            rta_id = request['__rta_id__']
         tagname = request['tagname']
         start_time = time.asctime(time.localtime(
             request['start_us'] / 1000000))
         end_time = time.asctime(time.localtime(
             request['end_us'] / 1000000))
-        logging.info(f"RQS {tagname} {start_time} {end_time}")
+        logging.info(f"RTA {tagname} {start_time} {end_time}")
         try:
             data = self.hist_tags[request['tagname']].read_bytes(
                 request['start_us'], request['end_us'])
             tagid = self.tags[request['tagname']].id
             tagtype = self.tags[request['tagname']].type
             packtype = 0
             if tagtype == int:
                 packtype = 1
             elif tagtype == float:
                 packtype = 2
-            self.rqs.value = pack('>HHH', rqs_id, tagid, packtype) + data
+            self.rta.value = pack('>HHH', rta_id, tagid, packtype) + data
             logging.info(f'sent {len(data)} bytes for {request["tagname"]}')
-            self.rqs.value = b'\x00\x00\x00\x00\x00\x00'
+            self.rta.value = b'\x00\x00\x00\x00\x00\x00'
         except Exception as e:
-            logging.error(f'history rqs_cb {e}')
+            logging.error(f'history rta_cb {e}')
 
     async def start(self):
         """Async startup."""
         await self.busclient.start()
 
 
 @atexit.register
```

### Comparing `pymscada-0.1.0a6/src/pymscada/iodrivers/logix_client.py` & `pymscada-0.1.1a2/src/pymscada/iodrivers/logix_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         """
         Connect to bus on bus_ip:bus_port, connect to Logix PLCs.
 
         Event loop must be running.
         """
         self.busclient = None
         if bus_ip is not None:
-            self.busclient = BusClient(bus_ip, bus_port)
+            self.busclient = BusClient(bus_ip, bus_port, module='Logix Client')
         self.mapping = LogixMaps(tags)
         self.connections: list[LogixClientConnector] = []
         for rtu in rtus:
             connection = LogixClientConnector(**rtu, mapping=self.mapping)
             self.connections.append(connection)
 
     async def _poll(self):
```

### Comparing `pymscada-0.1.0a6/src/pymscada/iodrivers/logix_map.py` & `pymscada-0.1.1a2/src/pymscada/iodrivers/logix_map.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/iodrivers/modbus_client.py` & `pymscada-0.1.1a2/src/pymscada/iodrivers/modbus_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,16 @@
         a websocket connection to request and set tag values and subscribe to
         changes.
 
         Event loop must be running.
         """
         self.busclient = None
         if bus_ip is not None:
-            self.busclient = BusClient(bus_ip, bus_port)
+            self.busclient = BusClient(bus_ip, bus_port,
+                                       module='Modbus Client')
         self.mapping = ModbusMaps(tags)
         self.connections: list[ModbusClientConnector] = []
         for rtu in rtus:
             connection = ModbusClientConnector(**rtu, mapping=self.mapping)
             self.connections.append(connection)
         self.mapping.make_map()
```

### Comparing `pymscada-0.1.0a6/src/pymscada/iodrivers/modbus_map.py` & `pymscada-0.1.1a2/src/pymscada/iodrivers/modbus_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,18 @@
             self.data[table] = bytearray(2 * (tables[table] - 1))
             self.value_chg[table] = value_chg
 
     def make_map(self):
         """Make the maps."""
         for tagname, v in self.tags.items():
             dtype = v['type']
-            addr = v['read']
+            try:
+                addr = v['read']
+            except KeyError:
+                addr = v['addr']
             map = ModbusMap(tagname, dtype, addr, self.data, self.value_chg)
             size = DTYPES[dtype][3]
             name, unit, file, word = addr.split(':')
             for i in range(0, size):
                 addr = f'{name}:{unit}:{file}:{int(word) + i}'
                 self.maps[addr] = map
```

### Comparing `pymscada-0.1.0a6/src/pymscada/iodrivers/modbus_server.py` & `pymscada-0.1.1a2/src/pymscada/iodrivers/modbus_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,16 @@
         a websocket connection to request and set tag values and subscribe to
         changes.
 
         Event loop must be running.
         """
         self.busclient = None
         if bus_ip is not None:
-            self.busclient = BusClient(bus_ip, bus_port)
+            self.busclient = BusClient(bus_ip, bus_port,
+                                       module='Modbus Server')
         self.mapping = ModbusMaps(tags)
         self.connections: list[ModbusServerConnector] = []
         for rtu in rtus:
             connection = ModbusServerConnector(**rtu, mapping=self.mapping)
             self.connections.append(connection)
         self.mapping.make_map()
```

### Comparing `pymscada-0.1.0a6/src/pymscada/iodrivers/ping_client.py` & `pymscada-0.1.1a2/src/pymscada/iodrivers/ping_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         """
         Connect to bus on bus_ip:bus_port, ping a list.
 
         Event loop must be running.
         """
         self.busclient = None
         if bus_ip is not None:
-            self.busclient = BusClient(bus_ip, bus_port)
+            self.busclient = BusClient(bus_ip, bus_port, module='Ping Client')
         self.mapping = PingMaps(tags)
         self.pinger = PingClientConnector(mapping=self.mapping)
 
     async def _poll(self):
         """For testing."""
         for connection in self.connections:
             await connection.poll()
```

### Comparing `pymscada-0.1.0a6/src/pymscada/iodrivers/ping_map.py` & `pymscada-0.1.1a2/src/pymscada/iodrivers/ping_map.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/iodrivers/snmp_client.py` & `pymscada-0.1.1a2/src/pymscada/iodrivers/snmp_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from pymscada.periodic import Periodic
 from pymscada.iodrivers.snmp_map import SnmpMaps
 
 
 class SnmpClientConnector:
     """Poll snmp devices, write and traps are not implemented."""
 
-    def __init__(self, name: str, ip: str, rate: float, read: list,
+    def __init__(self, name: str, ip: str, rate: float, poll: list,
                  community: str, mapping: SnmpMaps):
         """Set up polling client."""
         self.snmp_name = name
         self.ip = ip
         self.community = community
         self.read_oids = [snmp.ObjectType(snmp.ObjectIdentity(x))
-                          for x in read]
+                          for x in poll]
         self.mapping = mapping
         self.periodic = Periodic(self.poll, rate)
         self.snmp_engine = snmp.SnmpEngine()
 
     async def poll(self):
         """Poll data."""
         r = await snmp.getCmd(
@@ -53,15 +53,15 @@
         """
         Connect to bus on bus_ip:bus_port, connect to snmp devices.
 
         Event loop must be running.
         """
         self.busclient = None
         if bus_ip is not None:
-            self.busclient = BusClient(bus_ip, bus_port)
+            self.busclient = BusClient(bus_ip, bus_port, module='SNMP Client')
         self.mapping = SnmpMaps(tags)
         self.connections: list[SnmpClientConnector] = []
         for rtu in rtus:
             connection = SnmpClientConnector(**rtu, mapping=self.mapping)
             self.connections.append(connection)
 
     async def _poll(self):
```

### Comparing `pymscada-0.1.0a6/src/pymscada/iodrivers/snmp_map.py` & `pymscada-0.1.1a2/src/pymscada/iodrivers/snmp_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def __init__(self, tags: dict):
         """Collect maps based on a tag dictionary."""
         # use the tagname to access the map.
         self.tag_map: dict[str, SnmpMap] = {}
         # use the plc_name then variable name to access a list of maps.
         self.var_map: dict[str, dict[str, list[SnmpMap]]] = {}
         for tagname, v in tags.items():
-            addr = v['addr']
+            addr = v['read']
             map = SnmpMap(tagname, v['type'], addr)
             if map.plc not in self.var_map:
                 self.var_map[map.plc] = {}
             if map.var not in self.var_map[map.plc]:
                 # make a list so multiple bits can map to a word
                 self.var_map[map.plc][map.var] = []
             self.var_map[map.plc][map.var].append(map)
```

### Comparing `pymscada-0.1.0a6/src/pymscada/misc.py` & `pymscada-0.1.1a2/src/pymscada/misc.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/pdf/one.pdf` & `pymscada-0.1.1a2/src/pymscada/pdf/one.pdf`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/pdf/two.pdf` & `pymscada-0.1.1a2/src/pymscada/pdf/two.pdf`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/periodic.py` & `pymscada-0.1.1a2/src/pymscada/periodic.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/protocol_constants.py` & `pymscada-0.1.1a2/src/pymscada/protocol_constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,74 @@
 """
 Protocol description and protocol constants.
 
 Bus holds a tag forever, assigns a tag id forever, holds a tag value with len
 < 1000 forever, otherwise wipes periodically. So assign tagnames once, at the
-start of your program; use RQS as an update messenger, share whole structures
+start of your program; use RTA as an update messenger, share whole structures
 rarely.
 
 - version 16-bit unsigned int == 0x01
 - command 16-bit unsigned int
-- tag_id 32-bit unsigned int
+- tag_id 32-bit unsigned int     0 is not a valid tag_id
 - size 32-bit unsigned int
   - if size == 0xff  continuation mandatory
   - size 0x00 completes an empty continuation
 - time_us 128-bit unsigned int, UTC microseconds
 - data size of 8-bit char
 
 command
 - CMD_ID data is tagname
   - reply: CMD_ID with tag_id and data as tagname
 - CMD_SET id, data is typed or json packed
   - no reply
 - CMD_UNSUB id
   - no reply
 - CMD_GET id
-- CMD_RQS id, data is request to tag creator
+- CMD_RTA id, data is request to author
 - CMD_SUB id
   - reply: SET id and value, value may be None
 - CMD_LIST
   - size == 0x00
     - tags with values newer than time_us
   - size > 0x00
     - ^text matches start of tagname
     - text$ matches start of tagname
     - text matches anywhere in tagname
   - reply: LIST data as space separated tagnames
+- CMD_LOG data to logging.warning
 """
 
 # Tuning constants
 MAX_LEN = 65535 - 14  # TODO fix server(?) when 3
 
 # Network protocol commands
 CMD_ID = 1  # query / inform tag ID - data is tagname bytes string
 CMD_SET = 2  # set a tag
 CMD_GET = 3  # get a tag
-CMD_RQS = 4  # request set - request passed to last tag setter
+CMD_RTA = 4  # request to author
 CMD_SUB = 5  # subscribe to a tag
 CMD_UNSUB = 6  # unsubscribe from a tag
 CMD_LIST = 7  # bus list tags
 CMD_ERR = 8  # action failed
+CMD_LOG = 9  # bus print a logging message
 
 CMD_TEXT = {
     1: 'CMD_ID',
     2: 'CMD_SET',
     3: 'CMD_GET',
-    4: 'CMD_RQS',
+    4: 'CMD_RTA',
     5: 'CMD_SUB',
     6: 'CMD_UNSUB',
     7: 'CMD_LIST',
-    8: 'CMD_ERR'
+    8: 'CMD_ERR',
+    9: 'CMD_LOG'
 }
 
-COMMANDS = [CMD_ID, CMD_SET, CMD_GET, CMD_RQS, CMD_SUB, CMD_UNSUB, CMD_LIST,
-            CMD_ERR]
+COMMANDS = [CMD_ID, CMD_SET, CMD_GET, CMD_RTA, CMD_SUB, CMD_UNSUB, CMD_LIST,
+            CMD_ERR, CMD_LOG]
 
 # data types
 TYPE_INT = 1  # 64 bit signed integer
 TYPE_FLOAT = 2  # 64 bit IEEE float
 TYPE_STR = 3  # string
 TYPE_BYTES = 4
 TYPE_JSON = 5
```

### Comparing `pymscada-0.1.0a6/src/pymscada/samplers.py` & `pymscada-0.1.1a2/src/pymscada/samplers.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/tag.py` & `pymscada-0.1.1a2/src/pymscada/tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,36 @@
     'float': float,
     'list': list,
     'dict': dict,
     'bytes': bytes
 }
 
 
+def tag_for_web(tagname: str, tag: dict):
+    """Correct tag dictionary in place to be suitable for web client."""
+    tag['name'] = tagname
+    tag['id'] = None
+    if 'desc' not in tag:
+        tag['desc'] = tag.name
+    if 'multi' in tag:
+        tag['type'] = 'int'
+    else:
+        if 'type' not in tag:
+            tag['type'] = 'float'
+        else:
+            if tag['type'] not in TYPES:
+                tag['type'] = 'str'
+    if tag['type'] == 'int':
+        tag['dp'] = 0
+    elif tag['type'] == 'float' and 'dp' not in tag:
+        tag['dp'] = 2
+    elif tag['type'] == 'str' and 'dp' in tag:
+        del tag['dp']
+
+
 class UniqueTag(type):
     """Super Tag class only create unique tags for unique tag names."""
 
     __cache = {}
     __notify = None
 
     def __call__(cls, tagname: str, tagtype: type = None):
```

### Comparing `pymscada-0.1.0a6/src/pymscada/tools/snmp_client2.py` & `pymscada-0.1.1a2/src/pymscada/tools/snmp_client2.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/tools/walk.py` & `pymscada-0.1.1a2/src/pymscada/tools/walk.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/validate.py` & `pymscada-0.1.1a2/src/pymscada/validate.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/src/pymscada/www_server.py` & `pymscada-0.1.1a2/src/pymscada/www_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,78 +3,69 @@
 from aiohttp import web, WSMsgType
 import logging
 from pathlib import Path
 from struct import pack, unpack_from
 import time
 from pymscada.bus_client import BusClient
 import pymscada.protocol_constants as pc
-from pymscada.tag import Tag, TYPES
+from pymscada.tag import Tag, tag_for_web, TYPES
 from pymscada_html import get_html_file
 
 
-def tag_for_web(tagname: str, tag: dict):
-    """Correct tag dictionary in place to be suitable for web client."""
-    tag['name'] = tagname
-    tag['id'] = None
-    if 'desc' not in tag:
-        tag['desc'] = tag.name
-    if 'multi' in tag:
-        tag['type'] = 'int'
-    else:
-        if 'type' not in tag:
-            tag['type'] = 'float'
-        else:
-            if tag['type'] not in TYPES:
-                tag['type'] = 'str'
-    if tag['type'] == 'int':
-        tag['dp'] = 0
-    elif tag['type'] == 'float' and 'dp' not in tag:
-        tag['dp'] = 2
-    elif tag['type'] == 'str' and 'dp' in tag:
-        del tag['dp']
+class Interface():
+    """Provide an interface between web client rta and the action."""
+
+    def __init__(self, tagname: str) -> None:
+        """Return path tagname for rta requests."""
+        self.tag = Tag(tagname, dict)
+
+    def ask(self, message):
+        """Process the message."""
+        logging.warning(message)
 
 
 class WSHandler():
     """
     Websocket handler pushes displays, tags and values to client.
 
     Maintains a client state insofar as tag updates are concerned.
     This are transitory, lasting for a given web browser client.
     """
 
     ids = set(range(1, 100))
 
     def __init__(self, ws: web.WebSocketResponse, pages: dict,
-                 tag_info: dict[str, Tag], do_rqs):
+                 tag_info: dict[str, Tag], do_rta, interface: Interface):
         """Create callbacks to monitor tag values."""
         self.ws = ws
         self.pages = pages
         self.tag_info = tag_info
         self.tag_by_id: dict[int, Tag] = {}
         self.tag_by_name: dict[str, Tag] = {}
         self.queue = asyncio.Queue()
-        self.do_rqs = do_rqs
-        self.rqs_id = self.ids.pop()
-        logging.info(f'weksocket id {self.rqs_id}')
+        self.do_rta = do_rta
+        self.rta_id = self.ids.pop()
+        logging.info(f'websocket id {self.rta_id}')
+        self.interface = interface
 
     def __del__(self):
         """Depends on garbage collector. Is OK."""
-        self.ids.add(self.rqs_id)
+        self.ids.add(self.rta_id)
 
     async def send_queue(self):
         """Run forever, write from queue."""
         try:
             while True:
                 as_bytes, message = await self.queue.get()
                 if as_bytes:
                     await self.ws.send_bytes(message)
                 else:
                     await self.ws.send_json(message)
         except asyncio.CancelledError:
-            logging.warn(f'{self.rqs_id}: send queue error, close '
+            logging.warn(f'{self.rta_id}: send queue error, close '
                          f'{self.ws.exception()}')
             return
 
     def publish(self, tag: Tag):
         """
         Prepare message for web client.
 
@@ -87,75 +78,75 @@
         Use q, Q and d for time, int and float.
         i.e. Uint64, Int64, Float64.
         """
         if tag.type == int:
             self.queue.put_nowait((True, pack(
                 '!HHQq',            # Network big-endian
                 tag.id,             # Uint16
-                pc.TYPE_INT,           # Uint16
+                pc.TYPE_INT,        # Uint16
                 tag.time_us,        # Uint64
                 tag.value           # Int64
             )))
         elif tag.type == float:
             self.queue.put_nowait((True, pack(
                 '!HHQd',            # Network big-endian
                 tag.id,             # Uint16
-                pc.TYPE_FLOAT,         # Uint16
+                pc.TYPE_FLOAT,      # Uint16
                 tag.time_us,        # Uint64
                 tag.value           # Float64
             )))
         elif tag.type == str:
             asbytes = tag.value.encode()
             self.queue.put_nowait((True, pack(
                 f'!HHQ{len(asbytes)}s',  # Network big-endian
                 tag.id,             # Uint16
                 pc.TYPE_STR,        # Uint16
                 tag.time_us,        # Uint64
                 asbytes             # Char as needed
             )))
         elif tag.type == bytes:
-            rqs_id = unpack_from('>H', tag.value)[0]
-            if rqs_id in [0, self.rqs_id]:
+            rta_id = unpack_from('>H', tag.value)[0]
+            if rta_id in [0, self.rta_id]:
                 self.queue.put_nowait((True, pack(
                     f'!HHQ{len(tag.value)}s',  # Network big-endian
                     tag.id,             # Uint16
-                    pc.TYPE_BYTES,        # Uint16
+                    pc.TYPE_BYTES,      # Uint16
                     tag.time_us,        # Uint64
                     tag.value           # Char as needed
                 )))
             else:
-                logging.info(f'{self.rqs_id}: {tag.name} bytes mismatch id')
+                logging.info(f'{self.rta_id}: {tag.name} bytes mismatch id')
         elif tag.type in [dict, list]:
             self.queue.put_nowait((False, {
                 'type': 'tag',
                 'payload': {
                     'tagid': tag.id,
                     'time_us': tag.time_us,
                     'value': tag.value
                 }
             }))
 
     def notify_id(self, tag: Tag):
         """Must be done here."""
-        logging.info(f'{self.rqs_id}: send id to webclient for {tag.name}')
+        logging.info(f'{self.rta_id}: send id to webclient for {tag.name}')
         self.tag_info[tag.name]['id'] = tag.id
         self.tag_by_id[tag.id] = tag
         self.tag_by_name[tag.name] = tag
         self.queue.put_nowait(
             (False, {'type': 'tag_info', 'payload': self.tag_info[tag.name]}))
         tag.add_callback(self.publish)
         tag.del_callback_id(self.notify_id)
 
     def do_sub(self, tagname: str):
         """Subscribe to tag value."""
         try:
             tag = self.tag_by_name[tagname]
         except KeyError:
             if tagname not in self.tag_info:
-                logging.warning(f'{self.rqs_id}: no {tagname} in tag_info')
+                logging.warning(f'{self.rta_id}: no {tagname} in tag_info')
                 return
             tag = Tag(tagname, TYPES[self.tag_info[tagname]['type']])
         if tag.id is None:
             tag.add_callback_id(self.notify_id)
         else:
             self.notify_id(tag)
             if tag.value is not None:
@@ -164,72 +155,77 @@
     async def connection_active(self):
         """Run while the connection is active and don't return."""
         send_queue = asyncio.create_task(self.send_queue())
         self.queue.put_nowait(
             (False, {'type': 'pages', 'payload': self.pages}))
         async for msg in self.ws:
             if msg.type == WSMsgType.TEXT:
-                logging.info(f'{self.rqs_id}: websocket recv {msg.json()}')
+                logging.info(f'{self.rta_id}: websocket recv {msg.json()}')
                 command = msg.json()
                 action = command['type']
                 tagname = command['tagname']
                 value = command['value']
                 time_us = int(time.time() * 1e6)
                 bus = None
                 if action == 'set':  # pc.CMD_SET
                     self.tag_by_name[tagname].value = value, time_us, bus
-                elif action == 'rqs':  # pc.CMD_RQS
+                elif action == 'rta':  # pc.CMD_RTA
                     if 'File' in value:
                         file = await anext(self.ws)
                         value['_file_data'] = file.data
-                    value['__rqs_id__'] = self.rqs_id
-                    self.do_rqs(tagname, value)
+                    value['__rta_id__'] = self.rta_id
+                    self.do_rta(tagname, value)
+                elif action == 'request_to_author':
+                    self.interface.ask(command)
                 elif action == 'sub':  # pc.CMD_SUB
                     self.do_sub(tagname)
                 elif action == 'get':  # pc.CMD_GET
-                    logging.warning(f'{self.rqs_id}: CMD_GET not implemented.')
+                    logging.warning(f'{self.rta_id}: CMD_GET not implemented.')
                 elif action == 'unsub':  # pc.CMD_UNSUB
-                    logging.warning(f'{self.rqs_id}: CMD_UNSUB not '
+                    logging.warning(f'{self.rta_id}: CMD_UNSUB not '
                                     'implemented.')
             elif msg.type == WSMsgType.BINARY:
                 logging.info(f'{msg.data}')
             elif msg.type == WSMsgType.ERROR:
-                logging.warn(f'{self.rqs_id}: ws closing error '
+                logging.warn(f'{self.rta_id}: ws closing error '
                              f'{self.ws.exception()}')
         send_queue.cancel()
         for tag in self.tag_by_id.values():
             tag.del_callback_id(self.notify_id)
             tag.del_callback(self.publish)
 
 
 class WwwServer:
     """Connect to bus on bus_ip:bus_port, serve on ip:port for webclient."""
 
     def __init__(self, bus_ip: str = '127.0.0.1', bus_port: int = 1324,
                  ip: str = '127.0.0.1', port: int = 8324, get_path: str = None,
-                 tag_info: dict = {}, pages: dict = {}, paths: list[str] = []
+                 tag_info: dict = {}, pages: dict = {}, serve_path: str = None,
+                 www_tag: str = '__wwwserver__'
                  ) -> None:
         """
         Connect to bus on bus_ip:bus_port, serve on ip:port for webclient.
 
         Serves the webclient files at /, as a relative path. The webclient uses
         a websocket connection to request and set tag values and subscribe to
         changes.
 
         Event loop must be running.
         """
-        self.busclient = BusClient(bus_ip, bus_port, tag_info)
+        self.busclient = BusClient(bus_ip, bus_port, tag_info,
+                                   module='WWW Server')
         self.ip = ip
         self.port = port
         self.get_path = get_path
+        self.serve_path = Path(serve_path)
         for tagname, tag in tag_info.items():
             tag_for_web(tagname, tag)
         self.tag_info = tag_info
         self.pages = pages
-        self.paths = paths
+        self.interface = Interface(www_tag)
 
     async def redirect_handler(self, _request: web.Request):
         """Point an empty request to the index."""
         if self.get_path is None:
             file = get_html_file('index.html')
         else:
             file = Path(self.get_path, 'index.html')
@@ -243,32 +239,31 @@
         else:
             file = Path(self.get_path, request.match_info['file'])
         return web.FileResponse(file)
 
     async def path_handler(self, request: web.Request):
         """Plain files."""
         logging.info(f"path {request.match_info['path']}")
-        path = Path(request.match_info['path'])
+        path = self.serve_path.joinpath(request.match_info['path'])
         if path.is_dir():
             return web.HTTPForbidden(reason='folder not permitted')
-        if '/'.join(path.parts[:-1]) in self.paths:
-            if not path.exists():
-                return web.HTTPNotFound(reason='no such file in path')
-            return web.FileResponse(path)
+        if not path.exists():
+            return web.HTTPNotFound(reason='no such file in path')
+        return web.FileResponse(path)
         logging.warning(f"path not configured {request.match_info['path']}")
         return web.HTTPForbidden(reason='path not permitted')
 
     async def websocket_handler(self, request: web.Request):
         """Wait for connections. Create a new one each time."""
         peer = request.transport.get_extra_info('peername')
         logging.info(f"WS from {peer}")
         ws = web.WebSocketResponse(max_msg_size=0)  # disables max message size
         await ws.prepare(request)
-        await WSHandler(ws, self.pages, self.tag_info, self.busclient.rqs
-                        ).connection_active()
+        await WSHandler(ws, self.pages, self.tag_info, self.busclient.rta,
+                        self.interface).connection_active()
         await ws.close()
         logging.info(f"WS closed {peer}")
         return ws
 
     async def on_prepare(self, request, response):
         """Set the cache headers. Angular builds apps with a hash."""
         if request.path == '/index.html':
```

### Comparing `pymscada-0.1.0a6/tests/bus_echo.py` & `pymscada-0.1.1a2/tests/bus_echo.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 
 def callback(a: Tag, b: Tag):
     """Map values from tag to tag."""
     a.value = b.value
 
 
-def rqs_handler(tag: Tag):
+def rta_handler(tag: Tag):
     """__bus_echo__."""
 
-    def rqs(data: dict):
+    def rta(data: dict):
         """Process request set."""
         nonlocal tag
         if data == 'ping':
             tag.value = 'pong'
 
-    return rqs
+    return rta
 
 
 async def main(port):
     """Set up maps."""
     tag = Tag('__bus_echo__', str)
     tag.value = 'started'
     tag1 = Tag('one', str)
@@ -36,13 +36,13 @@
     tagpo = Tag('pipeout', int)
     tagpi = Tag('pipein', int)
     tagpo.add_callback(partial(callback, tagpi))
     tagspo = Tag('spipeout', str)
     tagspi = Tag('spipein', str)
     tagspo.add_callback(partial(callback, tagspi))
     client = BusClient(port=port)
-    client.add_callback_rqs(tag.name, rqs_handler(tag))
+    client.add_callback_rta(tag.name, rta_handler(tag))
     await client.start()
     await asyncio.get_event_loop().create_future()
 
 if __name__ == '__main__':
     asyncio.run(main(int(sys.argv[1])))
```

### Comparing `pymscada-0.1.0a6/tests/iodrivers/test_logix.py` & `pymscada-0.1.1a2/tests/iodrivers/test_logix.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/tests/iodrivers/test_modbus.py` & `pymscada-0.1.1a2/tests/iodrivers/test_modbus.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/tests/test_bus_server.py` & `pymscada-0.1.1a2/tests/test_bus_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,23 +43,14 @@
     """TODO the following is wrong."""
     tag_2.del_callback(cb, None)  # deletes callback on tag_0 as same tag
     tag_0.update(b'new again', 1000, 55)
     assert cb0 == b'tag_0 1 newer'
     tag_0.del_callback(cb, None)
 
 
-@pytest.fixture(scope='module')
-def event_loop():
-    """Override default scope from function to module."""
-    policy = asyncio.get_event_loop_policy()
-    loop = policy.new_event_loop()
-    yield loop
-    loop.close()
-
-
 @pytest_asyncio.fixture(scope='module')
 async def bus_server():
     """Run a live server on an unused port."""
     global server_port
     busserver = BusServer(port=0)
     server = await busserver.start()
     server_port = server.sockets[0].getsockname()[1]
@@ -95,15 +86,15 @@
      'recv': [None]},  # SUB does not return as this is sending bus
     {'desc': 'LIST bus tags',
      'send': (pc.CMD_LIST, 0, 0, b'^t_0'),
      'recv': [(pc.CMD_LIST, 0, None, b't_0')]},
 ]
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio(scope='module')
 async def test_protocol_message(bus_server):
     """Connect to the server and test the protocol."""
     global server_port
     t_id = None
     data = b''
     reader, writer = await asyncio.open_connection('127.0.0.1', server_port)
     for test in PROTOCOL_TESTS:
@@ -111,24 +102,27 @@
         if s_tag_id == 'ID':
             s_tag_id = t_id
         size = len(s_value)
         msg = pack(f'!BBHHQ{size}s', 1, s_cmd, s_tag_id, size, s_time_us,
                    s_value)
         writer.write(msg)
         for reply in test['recv']:
+            # Accumulate responses, can be zero or more
             try:
                 async with asyncio.timeout(0.1):
                     data += await reader.read(1000)
             except TimeoutError:
                 pass
+            # confirm there no data when no reply is wanted
             if reply is None:
                 if data == b'':
                     assert True
                     continue
                 assert False, test['desc']
+            # A reply is wanted and not received
             elif reply is not None and data == b'':
                 assert False, test['desc']
             r_cmd, r_tag_id, r_time_us, r_value = reply
             _v, cmd, tag_id, size, time_us = unpack_from(
                 '!BBHHQ', data, offset=0)
             data = data[14:]
             if cmd == pc.CMD_ID:
@@ -165,15 +159,15 @@
     """Pipe all tag updates through here."""
     global queue
     global qhist
     qhist.append(msg)
     queue.put_nowait(msg)
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio(scope='module')
 async def test_client_init(bus_server):
     """Check a busclient cleans up on deletion."""
     global server_port
     global queue
     # Hack the tag value straight into the bus
     mybustag = BusTag(b'myinit')
     mybustag.value = pack('!B4s', pc.TYPE_STR, b'init')
@@ -199,15 +193,15 @@
     assert await queue.get() == 'finalized'
     # For all that, normally, one client should be open for the life of the
     # program.
     # Remove the tag from callback otherwise other clients will notice.
     mytag.del_callback(tag_callback)
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio(scope='module')
 async def test_tag_info(bus_server):
     """Check tag info init works."""
     global server_port
     global queue
     tag_info = {
         'ftag1': {'init': 123.456},
         'dtag1': {'init': {'look': 'here'}},
@@ -223,15 +217,15 @@
     # cleanup, normally don't bother with this, but tests check more
     # internals that ever done in an application
     await client.shutdown()
     del client
     gc.collect()
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio(scope='module')
 async def test_client_speed(capsys, bus_echo):
     """Test for round-trip speed of small packets."""
     global server_port
     global queue
     TEST_COUNT = 1000  # shorter troublesome in windows
     client = BusClient(port=server_port)
     await client.start()
@@ -252,15 +246,15 @@
     ms_per_cycle = (t1 - t0) / 1000000 / TEST_COUNT
     with capsys.disabled():
         print(f'\n{TEST_COUNT} writes, round trip {ms_per_cycle}ms/write')
     assert ms_per_cycle < 10  # less than 10ms per count
     tagpi.del_callback(tag_callback)
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio(scope='module')
 async def test_client_big(capsys, bus_echo):
     """Test a message that needs multiple packets."""
     global server_port
     global queue
     TEST_LENGTH = 100000  # 1MB is 0s, 10MB is 0.2s, 100MB is 22s
     tagspi = Tag('spipein', str)
     tagspo = Tag('spipeout', str)
@@ -277,15 +271,15 @@
     ns_per_byte = (t1 - t0) / 10 / TEST_LENGTH
     with capsys.disabled():
         print(f'\n{10 * TEST_LENGTH} write, time {ns_per_byte}ms/byte')
     assert len(response.value) == 10 * TEST_LENGTH
     tagspi.del_callback(tag_callback)
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio(scope='module')
 async def test_client_echo(capsys, bus_echo):
     """Test echo from a separate process."""
     global server_port
     global queue
     client = BusClient(port=server_port)
     await client.start()
     tag_send_str = Tag('one', str)
@@ -300,22 +294,22 @@
         assert ready.value == i
         assert tag_recv_str.value == tag_send_str.value
         assert tag_recv_int.value == tag_send_int.value
     await client.shutdown()
     tag_recv_int.del_callback(tag_callback)
 
 
-@pytest.mark.asyncio
-async def test_client_rqs(bus_echo):
-    """Test request set (RQS) command with __bus_echo__."""
+@pytest.mark.asyncio(scope='module')
+async def test_client_rta(bus_echo):
+    """Test request to author (RTA) with __bus_echo__."""
     global server_port
     global queue
     client = BusClient(port=server_port)
     await client.start()
     be = Tag('__bus_echo__', str)
     be.add_callback(tag_callback)
     r = await queue.get()
     assert r.value == 'started'
     for _ in range(10):
-        client.rqs(be.name, 'ping')
+        client.rta(be.name, 'ping')
         r = await queue.get()
         assert r.value == 'pong'
```

### Comparing `pymscada-0.1.0a6/tests/test_config.py` & `pymscada-0.1.1a2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/tests/test_misc.py` & `pymscada-0.1.1a2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/tests/test_periodic.py` & `pymscada-0.1.1a2/tests/test_periodic.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/tests/test_samplers.py` & `pymscada-0.1.1a2/tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/tests/test_tag.py` & `pymscada-0.1.1a2/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `pymscada-0.1.0a6/tests/test_tag_history.py` & `pymscada-0.1.1a2/tests/test_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,35 +111,35 @@
     ]:
         p = Path(file)
         assert p.stat().st_size == size
         p.unlink()
 
 
 READ_TESTS = [
-    ({'__rqs_id__': 12345, 'tagname': 'hist_tag_0', 'start_us': 55,
+    ({'__rta_id__': 12345, 'tagname': 'hist_tag_0', 'start_us': 55,
       'end_us': -1},
-     {'rqs_id': 12345, 'tagid': 2, 'packtype': 1, 'start': (55, 55),
+     {'rta_id': 12345, 'tagid': 2, 'packtype': 1, 'start': (55, 55),
       'end': (59, 59)}),
-    ({'__rqs_id__': 255, 'tagname': 'hist_tag_0', 'start_us': 55,
+    ({'__rta_id__': 255, 'tagname': 'hist_tag_0', 'start_us': 55,
       'end_us': 80},
-     {'rqs_id': 255, 'tagid': 2, 'packtype': 1, 'start': (55, 55),
+     {'rta_id': 255, 'tagid': 2, 'packtype': 1, 'start': (55, 55),
       'end': (59, 59)}),
-    ({'__rqs_id__': 303, 'tagname': 'hist_tag_0', 'start_us': 20,
+    ({'__rta_id__': 303, 'tagname': 'hist_tag_0', 'start_us': 20,
       'end_us': 55},
-     {'rqs_id': 303, 'tagid': 2, 'packtype': 1, 'start': (20, 10),
+     {'rta_id': 303, 'tagid': 2, 'packtype': 1, 'start': (20, 10),
       'end': (54, 54)}),
-    ({'__rqs_id__': 305, 'tagname': 'hist_tag_0', 'start_us': -1,
+    ({'__rta_id__': 305, 'tagname': 'hist_tag_0', 'start_us': -1,
      'end_us': 30},
-     {'rqs_id': 305, 'tagid': 2, 'packtype': 1, 'start': (0, 255),
+     {'rta_id': 305, 'tagid': 2, 'packtype': 1, 'start': (0, 255),
       'end': (29, 19)}),
 ]
 
 
-def test_read_rqs_cb(t0: TagHistory):
-    """Test the RQS request data."""
+def test_read_rta_cb(t0: TagHistory):
+    """Test the RTA request data."""
     history = History(path='tests/test_assets',
                       tag_info={'hist_tag_0': {'type': 'int'}})
     history_tag = Tag('__history__', bytes)
     hist_tag_0 = Tag('hist_tag_0', int)
     for time_us, value in zip(TIMES[50:], VALUES[50:]):
         hist_tag_0.value = value, time_us, 999
     history_tag.id = 1  # no bus running in test so force this
@@ -149,29 +149,29 @@
 
     def history_cb(tag: Tag):
         nonlocal results
         results.append(tag.value)
 
     def decode(results):
         size = len(results)
-        rqs_id, tagid, packtype = unpack_from('>HHH', results)
+        rta_id, tagid, packtype = unpack_from('>HHH', results)
         result = {
-            'rqs_id': rqs_id,
+            'rta_id': rta_id,
             'tagid': tagid,
             'packtype': packtype,
             'dat': []
         }
         for offset in range(6, size, 16):
             result['dat'].append(unpack_from('!Qq', results, offset=offset))
         return result
 
     history_tag.add_callback(history_cb, 999)  # fake non-local bus
     """Read in middle of range crossing two files."""
     for test, resp in READ_TESTS:
-        history.rqs_cb(test)
+        history.rta_cb(test)
         decoded = decode(results.pop(0))
-        assert decoded['rqs_id'] == resp['rqs_id']
+        assert decoded['rta_id'] == resp['rta_id']
         assert decoded['tagid'] == resp['tagid']  # as set above
         assert decoded['packtype'] == resp['packtype']  # is integer
         assert decoded['dat'][0] == resp['start']
         assert decoded['dat'][-1] == resp['end']
         assert results.pop(0) == b'\x00\x00\x00\x00\x00\x00'
```

### Comparing `pymscada-0.1.0a6/PKG-INFO` & `pymscada-0.1.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pymscada
-Version: 0.1.0a6
+Version: 0.1.1a2
 Summary: Shared tag value SCADA with python backup and Angular UI
 Author-Email: Jamie Walton <jamie@walton.net.nz>
 License: GPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.9
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: aiohttp>=3.8.5
-Requires-Dist: pymscada-html==0.1.0a1
+Requires-Dist: pymscada-html==0.1.0
 Requires-Dist: cerberus>=1.3.5
 Requires-Dist: pycomm3>=1.2.14
 Requires-Dist: pysnmplib>=5.0.24
 Description-Content-Type: text/markdown
 
 # pymscada
 #### [Docs](https://github.com/jamie0walton/pymscada/blob/main/docs/README.md)
```

