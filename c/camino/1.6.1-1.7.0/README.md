# Comparing `tmp/camino-1.6.1.tar.gz` & `tmp/camino-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camino-1.6.1.tar", last modified: Mon Feb 13 03:51:49 2023, max compression
+gzip compressed data, was "camino-1.7.0.tar", last modified: Sat May 18 23:24:11 2024, max compression
```

## Comparing `camino-1.6.1.tar` & `camino-1.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-13 03:51:49.367254 camino-1.6.1/
--rw-rw-r--   0 me        (1000) me        (1000)      126 2023-01-16 03:22:08.000000 camino-1.6.1/.gitignore
--rw-rw-r--   0 me        (1000) me        (1000)     1078 2022-07-29 07:24:33.000000 camino-1.6.1/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)    14027 2023-02-13 03:51:49.367254 camino-1.6.1/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)    13567 2023-01-24 04:24:08.000000 camino-1.6.1/README.md
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-13 03:51:49.363254 camino-1.6.1/camino/
--rw-rw-r--   0 me        (1000) me        (1000)     5576 2023-01-24 04:22:00.000000 camino-1.6.1/camino/__init__.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-13 03:51:49.363254 camino-1.6.1/camino.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)    14027 2023-02-13 03:51:49.000000 camino-1.6.1/camino.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      353 2023-02-13 03:51:49.000000 camino-1.6.1/camino.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-02-13 03:51:49.000000 camino-1.6.1/camino.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)        9 2023-02-13 03:51:49.000000 camino-1.6.1/camino.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        7 2023-02-13 03:51:49.000000 camino-1.6.1/camino.egg-info/top_level.txt
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-13 03:51:49.363254 camino-1.6.1/examples/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-13 03:51:49.363254 camino-1.6.1/examples/CaminoExample/
--rw-rw-r--   0 me        (1000) me        (1000)     1278 2023-02-13 03:42:05.000000 camino-1.6.1/examples/CaminoExample/CaminoExample.ino
--rw-rw-r--   0 me        (1000) me        (1000)      682 2023-02-13 03:50:37.000000 camino-1.6.1/library.properties
--rwxrwxr-x   0 me        (1000) me        (1000)      262 2023-01-10 16:55:14.000000 camino-1.6.1/release.sh
--rw-rw-r--   0 me        (1000) me        (1000)       12 2022-07-29 07:23:34.000000 camino-1.6.1/requirements.txt
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-02-13 03:51:49.367254 camino-1.6.1/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)      970 2023-01-14 22:53:27.000000 camino-1.6.1/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-13 03:51:49.367254 camino-1.6.1/src/
--rw-rw-r--   0 me        (1000) me        (1000)    12292 2023-01-31 04:14:47.000000 camino-1.6.1/src/Camino.cpp
--rw-rw-r--   0 me        (1000) me        (1000)     2598 2023-01-16 00:30:18.000000 camino-1.6.1/src/Camino.h
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-13 03:51:49.367254 camino-1.6.1/test/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-02-13 03:51:49.367254 camino-1.6.1/test/Test/
--rw-rw-r--   0 me        (1000) me        (1000)     1399 2023-01-16 01:53:49.000000 camino-1.6.1/test/Test/Test.ino
--rw-rw-r--   0 me        (1000) me        (1000)      920 2023-01-16 03:20:51.000000 camino-1.6.1/test/test.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-18 23:24:11.237201 camino-1.7.0/
+-rw-rw-r--   0 me        (1000) me        (1000)      124 2024-05-18 21:04:12.000000 camino-1.7.0/.gitignore
+-rw-rw-r--   0 me        (1000) me        (1000)     1078 2021-12-12 23:08:40.000000 camino-1.7.0/LICENSE
+-rw-r--r--   0 me        (1000) me        (1000)    12249 2024-05-18 23:24:11.237201 camino-1.7.0/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)    11765 2024-05-18 21:04:12.000000 camino-1.7.0/README.md
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-18 23:24:11.233201 camino-1.7.0/camino/
+-rw-rw-r--   0 me        (1000) me        (1000)     5617 2024-05-18 23:05:12.000000 camino-1.7.0/camino/__init__.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-18 23:24:11.237201 camino-1.7.0/camino.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)    12249 2024-05-18 23:24:11.000000 camino-1.7.0/camino.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      363 2024-05-18 23:24:11.000000 camino-1.7.0/camino.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2024-05-18 23:24:11.000000 camino-1.7.0/camino.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        9 2024-05-18 23:24:11.000000 camino-1.7.0/camino.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        7 2024-05-18 23:24:11.000000 camino-1.7.0/camino.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-18 23:24:11.233201 camino-1.7.0/examples/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-18 23:24:11.233201 camino-1.7.0/examples/CaminoExample/
+-rw-rw-r--   0 me        (1000) me        (1000)     1268 2024-05-18 22:55:45.000000 camino-1.7.0/examples/CaminoExample/CaminoExample.ino
+-rw-rw-r--   0 me        (1000) me        (1000)      574 2024-05-18 22:56:33.000000 camino-1.7.0/library.properties
+-rwxrwxr-x   0 me        (1000) me        (1000)      262 2024-05-18 17:00:19.000000 camino-1.7.0/release.sh
+-rw-rw-r--   0 me        (1000) me        (1000)       12 2021-12-12 21:50:50.000000 camino-1.7.0/requirements.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2024-05-18 23:24:11.237201 camino-1.7.0/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)      970 2024-05-18 17:00:19.000000 camino-1.7.0/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-18 23:24:11.233201 camino-1.7.0/src/
+-rw-rw-r--   0 me        (1000) me        (1000)    10980 2024-05-18 22:56:19.000000 camino-1.7.0/src/Camino.h
+-rw-rw-r--   0 me        (1000) me        (1000)     7043 2024-05-18 22:56:19.000000 camino-1.7.0/src/arch.h
+-rw-rw-r--   0 me        (1000) me        (1000)     1655 2024-05-18 17:46:48.000000 camino-1.7.0/src/options.h
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-18 23:24:11.233201 camino-1.7.0/test/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-05-18 23:24:11.237201 camino-1.7.0/test/Test/
+-rw-rw-r--   0 me        (1000) me        (1000)     1399 2024-05-18 17:00:19.000000 camino-1.7.0/test/Test/Test.ino
+-rw-rw-r--   0 me        (1000) me        (1000)      920 2024-05-18 23:10:23.000000 camino-1.7.0/test/test.py
```

### Comparing `camino-1.6.1/LICENSE` & `camino-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `camino-1.6.1/PKG-INFO` & `camino-1.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: camino
-Version: 1.6.1
+Version: 1.7.0
 Summary: A library for controlling an Arduino from Python over Serial
 Home-page: https://github.com/n-wach/camino
 Author: Nathan Wachholz
 Author-email: camino@nathanwachholz.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyserial
 
 # Camino
 
-Camino enables blazing fast, non-intrusive communication over a serial connection between 
-Python and up to 256 Arduinos. It provides a simple way to call functions on a remote
-Arduino, sending and receiving up to 255 bytes of data. Besides the built in functions 
-(`digital_write`, `pin_mode`, `analog_read`, etc.), approximately 250 user-defined 
-functions can be defined.
-
+Camino enables blazing fast, non-intrusive communication between Python and
+one or more Arduinos over a serial connection. Besides built in functions
+(`digital_write`, `pin_mode`, etc.), Camino can call user-defined functions
+to send and recieve arbitrary data.
 
 ## Table of Contents
 
 - [Installation](#Installation)
 - [Example](#Example)
 - [Adding Custom Functions](#Adding-Custom-Functions)
 - [Features and Limitations](#Features-and-Limitations)
@@ -79,17 +78,17 @@
 
 void setup() {
   camino.begin(9600);
 }
 
 void loop() {}
 
-// Example that returns the sum of some data (%256)
+// Example that returns the sum of some data
 void add(byte dataLength, byte *dataArray) {
-  byte sum = 0;
+  int sum = 0;
   for(byte i = 0; i < dataLength; i++){
     sum += dataArray[i];
   }
   returns(sum);
 }
 
 // Example that returns a string
@@ -259,69 +258,30 @@
 when polled using a callable.
 
 Lastly, Camino is incredibly fast, with low overhead. Even at low baud-rates, it is
 possible to PWM digital pins using only `digital_write` from within Python.
 
 ## Options
 
-A few options are listed in `Camino.h` for more advanced use cases.
-
-If you want to use values other than the defaults, you'll need to manually download
-and include the library in your sketch, and change them in `Camino.h`.
-
-### UART Port: `PORT`
-
-The UART port used by Camino. Can be `-1`, `0`, `1`, `2`. We default to UART0, which is 
-usually the USB port. This means you can't use Serial in your sketch. For
-other boards, like the Arduino Mega, you could have Camino listen on UART2 
-(`Serial2`) and use the normal Serial port in parallel.
-
-### Maximum Data Length in Packets: `MAX_DATA_LENGTH`
-
-The maximum length of the data section for packets (to and from the Arduino). 
-Value must be at least 16 and at most 255. Making it smaller reduces the
-memory footprint of Camino.
-
-### Command Timeout: `COMMAND_TIMEOUT_MS`.
-
-The command timeout in milliseconds. When a new byte in a packet is received,
-if this period has elapsed since the start of the packet, the earlier
-bytes are discarded and Camino assumes that a new packet is beginning.
-
-Defaults to 100 milliseconds. With a well-behaved connection, this should 
-never matter.
-
-### Transmission Hooks
-
-There are three possible macros that act as hooks into the lifecycle of a 
-packet transmission:
-
-- `initTransmissions()` is called in begin()
-- `beginTransmission()`is called before the first byte is sent in a response packet.
-- `endTransmission()` is called after the last byte is sent in a response packet.
+A few options are listed in [`options.h`](/src/options.h) for more advanced use cases,
+such as changing the ports/pins used.
 
-Sometimes you may need to do some preparation before a packet can be sent. 
-For instance, you may have a pin that enables a pull down resistor to remove 
-noise from your transmission line when not sending anything. Or when debugging, it
-may be useful to shine an LED when packets are being sent.
+If you want to use values other than the defaults, place `#define` calls before
+`#include "Camino.h"`.
 
 ## Protocol
 
-The protocol refers to the host Python machine as the Master, and the Arduino
-as the Slave.
+No Arduino may transmit unless it is in response to a command from Python, and
+only one response per command is allowed.
 
-The protocol follows a simple rule that no slave may transmit unless it is in
-response to a command from the master, and only one response per command is 
-allowed.
-
-The master's command packet always takes the same format. It specifies which
-Arduino is being addressed, which command should be run, and what data to
-pass to the command.
+A command packet always takes the same format. It specifies which Arduino is
+being addressed, which command should be run, and what data to pass to the
+command.
 
-The slave can respond in one of three ways:
+The Ardunio can respond in one of three ways:
 
 - Response with data, for instance with `digital_read`
 - Response with no data, for instance with `digital_write`
 - Resend request, if there is a problem understanding the command.
 
 ### Single Command Communication Flow
```

### Comparing `camino-1.6.1/README.md` & `camino-1.7.0/camino.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,28 @@
-# Camino
+Metadata-Version: 2.1
+Name: camino
+Version: 1.7.0
+Summary: A library for controlling an Arduino from Python over Serial
+Home-page: https://github.com/n-wach/camino
+Author: Nathan Wachholz
+Author-email: camino@nathanwachholz.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyserial
 
-Camino enables blazing fast, non-intrusive communication over a serial connection between 
-Python and up to 256 Arduinos. It provides a simple way to call functions on a remote
-Arduino, sending and receiving up to 255 bytes of data. Besides the built in functions 
-(`digital_write`, `pin_mode`, `analog_read`, etc.), approximately 250 user-defined 
-functions can be defined.
+# Camino
 
+Camino enables blazing fast, non-intrusive communication between Python and
+one or more Arduinos over a serial connection. Besides built in functions
+(`digital_write`, `pin_mode`, etc.), Camino can call user-defined functions
+to send and recieve arbitrary data.
 
 ## Table of Contents
 
 - [Installation](#Installation)
 - [Example](#Example)
 - [Adding Custom Functions](#Adding-Custom-Functions)
 - [Features and Limitations](#Features-and-Limitations)
@@ -65,17 +78,17 @@
 
 void setup() {
   camino.begin(9600);
 }
 
 void loop() {}
 
-// Example that returns the sum of some data (%256)
+// Example that returns the sum of some data
 void add(byte dataLength, byte *dataArray) {
-  byte sum = 0;
+  int sum = 0;
   for(byte i = 0; i < dataLength; i++){
     sum += dataArray[i];
   }
   returns(sum);
 }
 
 // Example that returns a string
@@ -245,69 +258,30 @@
 when polled using a callable.
 
 Lastly, Camino is incredibly fast, with low overhead. Even at low baud-rates, it is
 possible to PWM digital pins using only `digital_write` from within Python.
 
 ## Options
 
-A few options are listed in `Camino.h` for more advanced use cases.
-
-If you want to use values other than the defaults, you'll need to manually download
-and include the library in your sketch, and change them in `Camino.h`.
-
-### UART Port: `PORT`
-
-The UART port used by Camino. Can be `-1`, `0`, `1`, `2`. We default to UART0, which is 
-usually the USB port. This means you can't use Serial in your sketch. For
-other boards, like the Arduino Mega, you could have Camino listen on UART2 
-(`Serial2`) and use the normal Serial port in parallel.
-
-### Maximum Data Length in Packets: `MAX_DATA_LENGTH`
-
-The maximum length of the data section for packets (to and from the Arduino). 
-Value must be at least 16 and at most 255. Making it smaller reduces the
-memory footprint of Camino.
-
-### Command Timeout: `COMMAND_TIMEOUT_MS`.
-
-The command timeout in milliseconds. When a new byte in a packet is received,
-if this period has elapsed since the start of the packet, the earlier
-bytes are discarded and Camino assumes that a new packet is beginning.
-
-Defaults to 100 milliseconds. With a well-behaved connection, this should 
-never matter.
-
-### Transmission Hooks
-
-There are three possible macros that act as hooks into the lifecycle of a 
-packet transmission:
-
-- `initTransmissions()` is called in begin()
-- `beginTransmission()`is called before the first byte is sent in a response packet.
-- `endTransmission()` is called after the last byte is sent in a response packet.
+A few options are listed in [`options.h`](/src/options.h) for more advanced use cases,
+such as changing the ports/pins used.
 
-Sometimes you may need to do some preparation before a packet can be sent. 
-For instance, you may have a pin that enables a pull down resistor to remove 
-noise from your transmission line when not sending anything. Or when debugging, it
-may be useful to shine an LED when packets are being sent.
+If you want to use values other than the defaults, place `#define` calls before
+`#include "Camino.h"`.
 
 ## Protocol
 
-The protocol refers to the host Python machine as the Master, and the Arduino
-as the Slave.
+No Arduino may transmit unless it is in response to a command from Python, and
+only one response per command is allowed.
 
-The protocol follows a simple rule that no slave may transmit unless it is in
-response to a command from the master, and only one response per command is 
-allowed.
-
-The master's command packet always takes the same format. It specifies which
-Arduino is being addressed, which command should be run, and what data to
-pass to the command.
+A command packet always takes the same format. It specifies which Arduino is
+being addressed, which command should be run, and what data to pass to the
+command.
 
-The slave can respond in one of three ways:
+The Ardunio can respond in one of three ways:
 
 - Response with data, for instance with `digital_read`
 - Response with no data, for instance with `digital_write`
 - Resend request, if there is a problem understanding the command.
 
 ### Single Command Communication Flow
```

### Comparing `camino-1.6.1/camino/__init__.py` & `camino-1.7.0/camino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from serial import Serial
 import logging
+
 logger = logging.getLogger(__name__)
 
 MAX_DATA_LENGTH = 250
 SEND_ATTEMPTS = 3
 COMMAND_TIMEOUT_PERIOD_S = 1
 
 COMMAND_HEADER_BYTE_1 = 0xAA
@@ -39,15 +40,15 @@
             raise CaminoException(
                 f"Mismatched header bytes: {header_byte_1} vs {header_byte_2}"
             )
 
         if header_byte_1 == RESPONSE_HEADER_WITH_NO_DATA:
             return None
         elif header_byte_1 == RESPONSE_HEADER_WITH_DATA:
-            # slave is going to send some data with the response code
+            # arduino is going to send some data with the response code
             data_length = self.read_byte()
             checksum = data_length
             data = self.port.read(data_length)
             for b in data:
                 checksum += b
             checksum = checksum % 256
             received_checksum = self.read_byte()
@@ -93,15 +94,17 @@
             self.port.write(bytes(packet))
             self.port.flushOutput()
             try:
                 response = self.read_packet()
                 return response
             except CaminoException as e:
                 last_exception = e
-                logger.warning(f"Got error on communication attempt {attempt_number + 1}/{SEND_ATTEMPTS}: {e}")
+                logger.warning(
+                    f"Got error on communication attempt {attempt_number + 1}/{SEND_ATTEMPTS}: {e}"
+                )
                 # flushing
                 self.port.flush()
         raise CaminoException(
             f"All {SEND_ATTEMPTS} consecutive attempts to communicate with device failed."
         ) from last_exception
```

### Comparing `camino-1.6.1/camino.egg-info/PKG-INFO` & `camino-1.7.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,13 @@
-Metadata-Version: 2.1
-Name: camino
-Version: 1.6.1
-Summary: A library for controlling an Arduino from Python over Serial
-Home-page: https://github.com/n-wach/camino
-Author: Nathan Wachholz
-Author-email: camino@nathanwachholz.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Camino
 
-Camino enables blazing fast, non-intrusive communication over a serial connection between 
-Python and up to 256 Arduinos. It provides a simple way to call functions on a remote
-Arduino, sending and receiving up to 255 bytes of data. Besides the built in functions 
-(`digital_write`, `pin_mode`, `analog_read`, etc.), approximately 250 user-defined 
-functions can be defined.
-
+Camino enables blazing fast, non-intrusive communication between Python and
+one or more Arduinos over a serial connection. Besides built in functions
+(`digital_write`, `pin_mode`, etc.), Camino can call user-defined functions
+to send and recieve arbitrary data.
 
 ## Table of Contents
 
 - [Installation](#Installation)
 - [Example](#Example)
 - [Adding Custom Functions](#Adding-Custom-Functions)
 - [Features and Limitations](#Features-and-Limitations)
@@ -79,17 +63,17 @@
 
 void setup() {
   camino.begin(9600);
 }
 
 void loop() {}
 
-// Example that returns the sum of some data (%256)
+// Example that returns the sum of some data
 void add(byte dataLength, byte *dataArray) {
-  byte sum = 0;
+  int sum = 0;
   for(byte i = 0; i < dataLength; i++){
     sum += dataArray[i];
   }
   returns(sum);
 }
 
 // Example that returns a string
@@ -259,69 +243,30 @@
 when polled using a callable.
 
 Lastly, Camino is incredibly fast, with low overhead. Even at low baud-rates, it is
 possible to PWM digital pins using only `digital_write` from within Python.
 
 ## Options
 
-A few options are listed in `Camino.h` for more advanced use cases.
-
-If you want to use values other than the defaults, you'll need to manually download
-and include the library in your sketch, and change them in `Camino.h`.
-
-### UART Port: `PORT`
-
-The UART port used by Camino. Can be `-1`, `0`, `1`, `2`. We default to UART0, which is 
-usually the USB port. This means you can't use Serial in your sketch. For
-other boards, like the Arduino Mega, you could have Camino listen on UART2 
-(`Serial2`) and use the normal Serial port in parallel.
-
-### Maximum Data Length in Packets: `MAX_DATA_LENGTH`
-
-The maximum length of the data section for packets (to and from the Arduino). 
-Value must be at least 16 and at most 255. Making it smaller reduces the
-memory footprint of Camino.
-
-### Command Timeout: `COMMAND_TIMEOUT_MS`.
-
-The command timeout in milliseconds. When a new byte in a packet is received,
-if this period has elapsed since the start of the packet, the earlier
-bytes are discarded and Camino assumes that a new packet is beginning.
-
-Defaults to 100 milliseconds. With a well-behaved connection, this should 
-never matter.
-
-### Transmission Hooks
-
-There are three possible macros that act as hooks into the lifecycle of a 
-packet transmission:
-
-- `initTransmissions()` is called in begin()
-- `beginTransmission()`is called before the first byte is sent in a response packet.
-- `endTransmission()` is called after the last byte is sent in a response packet.
+A few options are listed in [`options.h`](/src/options.h) for more advanced use cases,
+such as changing the ports/pins used.
 
-Sometimes you may need to do some preparation before a packet can be sent. 
-For instance, you may have a pin that enables a pull down resistor to remove 
-noise from your transmission line when not sending anything. Or when debugging, it
-may be useful to shine an LED when packets are being sent.
+If you want to use values other than the defaults, place `#define` calls before
+`#include "Camino.h"`.
 
 ## Protocol
 
-The protocol refers to the host Python machine as the Master, and the Arduino
-as the Slave.
+No Arduino may transmit unless it is in response to a command from Python, and
+only one response per command is allowed.
 
-The protocol follows a simple rule that no slave may transmit unless it is in
-response to a command from the master, and only one response per command is 
-allowed.
-
-The master's command packet always takes the same format. It specifies which
-Arduino is being addressed, which command should be run, and what data to
-pass to the command.
+A command packet always takes the same format. It specifies which Arduino is
+being addressed, which command should be run, and what data to pass to the
+command.
 
-The slave can respond in one of three ways:
+The Ardunio can respond in one of three ways:
 
 - Response with data, for instance with `digital_read`
 - Response with no data, for instance with `digital_write`
 - Resend request, if there is a problem understanding the command.
 
 ### Single Command Communication Flow
```

### Comparing `camino-1.6.1/examples/CaminoExample/CaminoExample.ino` & `camino-1.7.0/examples/CaminoExample/CaminoExample.ino`

 * *Files 6% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     Created 22 March 2022
     By Nathan Wachholz
 */
 
 #include "Camino.h"
 
 void setup() {
-  camino.begin(115200);
+  camino.begin(9600);
 }
 
 void loop() {}
 
-// Example that returns the sum of some data (%256)
+// Example that returns the sum of some data
 void add(byte dataLength, byte *dataArray) {
-  byte sum = 0;
+  int sum = 0;
   for(byte i = 0; i < dataLength; i++){
     sum += dataArray[i];
   }
   returns(sum);
 }
 
 // Example that returns a string
```

### Comparing `camino-1.6.1/setup.py` & `camino-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `camino-1.6.1/test/Test/Test.ino` & `camino-1.7.0/test/Test/Test.ino`

 * *Files identical despite different names*

### Comparing `camino-1.6.1/test/test.py` & `camino-1.7.0/test/test.py`

 * *Files identical despite different names*

