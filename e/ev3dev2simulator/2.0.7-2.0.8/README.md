# Comparing `tmp/ev3dev2simulator-2.0.7.tar.gz` & `tmp/ev3dev2simulator-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ev3dev2simulator-2.0.7.tar", last modified: Sun May 19 13:53:33 2024, max compression
+gzip compressed data, was "ev3dev2simulator-2.0.8.tar", last modified: Sun May 19 14:37:18 2024, max compression
```

## Comparing `ev3dev2simulator-2.0.7.tar` & `ev3dev2simulator-2.0.8.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.217051 ev3dev2simulator-2.0.7/
--rw-r--r--   0 harcok     (501) staff       (20)     1081 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/LICENSE.txt
--rw-r--r--   0 harcok     (501) staff       (20)     4949 2024-05-19 13:53:33.216804 ev3dev2simulator-2.0.7/PKG-INFO
--rw-r--r--   0 harcok     (501) staff       (20)     2415 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/README.md
--rw-r--r--   0 harcok     (501) staff       (20)     2665 2024-05-19 06:36:16.000000 ev3dev2simulator-2.0.7/pyproject.toml
--rw-r--r--   0 harcok     (501) staff       (20)       38 2024-05-19 13:53:33.217102 ev3dev2simulator-2.0.7/setup.cfg
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.190314 ev3dev2simulator-2.0.7/src/
--rw-r--r--   0 harcok     (501) staff       (20)     5033 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/bluetooth.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.195120 ev3dev2simulator-2.0.7/src/ev3dev2/
--rw-r--r--   0 harcok     (501) staff       (20)     6864 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/__init__.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.195433 ev3dev2simulator-2.0.7/src/ev3dev2/_platform/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/_platform/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)     2284 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/_platform/ev3.py
--rw-r--r--   0 harcok     (501) staff       (20)      626 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/auto.py
--rw-r--r--   0 harcok     (501) staff       (20)     8935 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/button.py
--rw-r--r--   0 harcok     (501) staff       (20)     6032 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/console.py
--rw-r--r--   0 harcok     (501) staff       (20)    10393 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/display.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.195596 ev3dev2simulator-2.0.7/src/ev3dev2/fonts/
--rw-r--r--   0 harcok     (501) staff       (20)      935 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/fonts/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)    16482 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/led.py
--rw-r--r--   0 harcok     (501) staff       (20)    72743 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/motor.py
--rw-r--r--   0 harcok     (501) staff       (20)     5664 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/port.py
--rw-r--r--   0 harcok     (501) staff       (20)     3257 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/power.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.196021 ev3dev2simulator-2.0.7/src/ev3dev2/sensor/
--rw-r--r--   0 harcok     (501) staff       (20)     7394 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/sensor/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)    30430 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/sensor/lego.py
--rw-r--r--   0 harcok     (501) staff       (20)    25098 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/sound.py
--rw-r--r--   0 harcok     (501) staff       (20)     1909 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/stopwatch.py
--rw-r--r--   0 harcok     (501) staff       (20)     5836 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/unit.py
--rw-r--r--   0 harcok     (501) staff       (20)       27 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/version.py
--rw-r--r--   0 harcok     (501) staff       (20)     1646 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2/wheel.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.196811 ev3dev2simulator-2.0.7/src/ev3dev2simulator/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)     1395 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/__main__.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.188879 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.202688 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/
--rw-r--r--   0 harcok     (501) staff       (20)     1264 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/arm.png
--rw-r--r--   0 harcok     (501) staff       (20)     5175 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/arm_large.png
--rw-r--r--   0 harcok     (501) staff       (20)    10434 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/body.png
--rw-r--r--   0 harcok     (501) staff       (20)   122910 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/bottle.png
--rw-r--r--   0 harcok     (501) staff       (20)    59554 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/brick.png
--rw-r--r--   0 harcok     (501) staff       (20)     1460 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_black.png
--rw-r--r--   0 harcok     (501) staff       (20)     2391 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_blue.png
--rw-r--r--   0 harcok     (501) staff       (20)     2423 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_green.png
--rw-r--r--   0 harcok     (501) staff       (20)     2401 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_red.png
--rw-r--r--   0 harcok     (501) staff       (20)     2272 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_white.png
--rw-r--r--   0 harcok     (501) staff       (20)     2382 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_yellow.png
--rw-r--r--   0 harcok     (501) staff       (20)     1362 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_amber.png
--rw-r--r--   0 harcok     (501) staff       (20)     1338 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_black.png
--rw-r--r--   0 harcok     (501) staff       (20)     1473 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_green.png
--rw-r--r--   0 harcok     (501) staff       (20)     1459 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_orange.png
--rw-r--r--   0 harcok     (501) staff       (20)     1391 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_red.png
--rw-r--r--   0 harcok     (501) staff       (20)     1389 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_yellow.png
--rw-r--r--   0 harcok     (501) staff       (20)     2925 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/touch_sensor_left.png
--rw-r--r--   0 harcok     (501) staff       (20)     1422 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/touch_sensor_rear.png
--rw-r--r--   0 harcok     (501) staff       (20)     2869 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/touch_sensor_right.png
--rw-r--r--   0 harcok     (501) staff       (20)     4315 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/ultrasonic_sensor_bottom.png
--rw-r--r--   0 harcok     (501) staff       (20)     2808 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/ultrasonic_sensor_top.png
--rw-r--r--   0 harcok     (501) staff       (20)     2771 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/wheel.png
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.203390 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)     4034 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/config.py
--rw-r--r--   0 harcok     (501) staff       (20)     5655 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/config_checker.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.203756 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/robot_configurations/
--rw-r--r--   0 harcok     (501) staff       (20)     1619 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/robot_configurations/large_robot.yaml
--rw-r--r--   0 harcok     (501) staff       (20)      861 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/robot_configurations/small_robot.yaml
--rw-r--r--   0 harcok     (501) staff       (20)     2637 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/simulation_settings.yaml
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.204491 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/world_configurations/
--rw-r--r--   0 harcok     (501) staff       (20)      952 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/world_configurations/config_large.yaml
--rw-r--r--   0 harcok     (501) staff       (20)     1049 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/world_configurations/config_large2.yaml
--rw-r--r--   0 harcok     (501) staff       (20)      804 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/world_configurations/config_small.yaml
--rw-r--r--   0 harcok     (501) staff       (20)      901 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/world_configurations/config_small2.yaml
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.205371 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)     3214 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/client_socket.py
--rw-r--r--   0 harcok     (501) staff       (20)     2125 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/client_socket_handler.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.206859 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)      384 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/command.py
--rw-r--r--   0 harcok     (501) staff       (20)      681 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/config_request.py
--rw-r--r--   0 harcok     (501) staff       (20)      495 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/data_request.py
--rw-r--r--   0 harcok     (501) staff       (20)      840 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/led_command.py
--rw-r--r--   0 harcok     (501) staff       (20)      709 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/motor_command.py
--rw-r--r--   0 harcok     (501) staff       (20)     1856 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/rotate_command.py
--rw-r--r--   0 harcok     (501) staff       (20)      809 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/sound_command.py
--rw-r--r--   0 harcok     (501) staff       (20)      929 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/stop_command.py
--rw-r--r--   0 harcok     (501) staff       (20)     5177 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message_handler.py
--rw-r--r--   0 harcok     (501) staff       (20)     3779 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/server_sockets.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.207826 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)     1316 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/device_connector.py
--rw-r--r--   0 harcok     (501) staff       (20)     1042 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/led_connector.py
--rw-r--r--   0 harcok     (501) staff       (20)     4960 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/motor_connector.py
--rw-r--r--   0 harcok     (501) staff       (20)     2118 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/sensor_connector.py
--rw-r--r--   0 harcok     (501) staff       (20)     7785 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/sound_connector.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.210093 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)      789 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/arm_floor.py
--rw-r--r--   0 harcok     (501) staff       (20)     2340 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/board.py
--rw-r--r--   0 harcok     (501) staff       (20)     1609 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/border.py
--rw-r--r--   0 harcok     (501) staff       (20)     2983 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/border_obstacle.py
--rw-r--r--   0 harcok     (501) staff       (20)     1700 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/bottle.py
--rw-r--r--   0 harcok     (501) staff       (20)      746 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/color_obstacle.py
--rw-r--r--   0 harcok     (501) staff       (20)      971 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/edge.py
--rw-r--r--   0 harcok     (501) staff       (20)     1417 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/hole.py
--rw-r--r--   0 harcok     (501) staff       (20)     3981 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/lake.py
--rw-r--r--   0 harcok     (501) staff       (20)     1465 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/movable_object.py
--rw-r--r--   0 harcok     (501) staff       (20)     2637 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/rock.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.212749 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)     1366 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/arm.py
--rw-r--r--   0 harcok     (501) staff       (20)     2245 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/arm_large.py
--rw-r--r--   0 harcok     (501) staff       (20)     3021 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/body_part.py
--rw-r--r--   0 harcok     (501) staff       (20)      728 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/brick.py
--rw-r--r--   0 harcok     (501) staff       (20)     2281 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/color_sensor.py
--rw-r--r--   0 harcok     (501) staff       (20)     1486 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/led.py
--rw-r--r--   0 harcok     (501) staff       (20)      995 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/speaker.py
--rw-r--r--   0 harcok     (501) staff       (20)     1733 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/touch_sensor.py
--rw-r--r--   0 harcok     (501) staff       (20)     2211 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/ultrasonic_sensor_bottom.py
--rw-r--r--   0 harcok     (501) staff       (20)     4811 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/ultrasonic_sensor_top.py
--rw-r--r--   0 harcok     (501) staff       (20)     1345 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/wheel.py
--rw-r--r--   0 harcok     (501) staff       (20)     3013 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/simulator.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.214714 ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)     8584 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/message_processor.py
--rw-r--r--   0 harcok     (501) staff       (20)     7062 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/motor_command_processor.py
--rw-r--r--   0 harcok     (501) staff       (20)     8634 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/robot_simulator.py
--rw-r--r--   0 harcok     (501) staff       (20)    15515 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/robot_state.py
--rw-r--r--   0 harcok     (501) staff       (20)     3296 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/world_simulator.py
--rw-r--r--   0 harcok     (501) staff       (20)     6252 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/world_state.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.215531 ev3dev2simulator-2.0.7/src/ev3dev2simulator/util/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/util/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)      388 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/util/dimensions.py
--rw-r--r--   0 harcok     (501) staff       (20)     2246 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/util/instance_checker.py
--rw-r--r--   0 harcok     (501) staff       (20)      222 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/util/point.py
--rw-r--r--   0 harcok     (501) staff       (20)     3666 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/util/util.py
--rw-r--r--   0 harcok     (501) staff       (20)      149 2024-05-19 06:37:07.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/version.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.216175 ev3dev2simulator-2.0.7/src/ev3dev2simulator/visualisation/
--rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/visualisation/__init__.py
--rw-r--r--   0 harcok     (501) staff       (20)      777 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/visualisation/robot_part_sprite.py
--rw-r--r--   0 harcok     (501) staff       (20)     4381 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/visualisation/sidebar.py
--rw-r--r--   0 harcok     (501) staff       (20)    17348 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator/visualisation/visualiser.py
-drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 13:53:33.216457 ev3dev2simulator-2.0.7/src/ev3dev2simulator.egg-info/
--rw-r--r--   0 harcok     (501) staff       (20)     4949 2024-05-19 13:53:33.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator.egg-info/PKG-INFO
--rw-r--r--   0 harcok     (501) staff       (20)     5484 2024-05-19 13:53:33.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator.egg-info/SOURCES.txt
--rw-r--r--   0 harcok     (501) staff       (20)        1 2024-05-19 13:53:33.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator.egg-info/dependency_links.txt
--rw-r--r--   0 harcok     (501) staff       (20)       68 2024-05-19 13:53:33.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator.egg-info/entry_points.txt
--rw-r--r--   0 harcok     (501) staff       (20)      130 2024-05-19 13:53:33.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator.egg-info/requires.txt
--rw-r--r--   0 harcok     (501) staff       (20)       35 2024-05-19 13:53:33.000000 ev3dev2simulator-2.0.7/src/ev3dev2simulator.egg-info/top_level.txt
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.374108 ev3dev2simulator-2.0.8/
+-rw-r--r--   0 harcok     (501) staff       (20)     1081 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/LICENSE.txt
+-rw-r--r--   0 harcok     (501) staff       (20)     5043 2024-05-19 14:37:18.373847 ev3dev2simulator-2.0.8/PKG-INFO
+-rw-r--r--   0 harcok     (501) staff       (20)     2509 2024-05-19 14:24:09.000000 ev3dev2simulator-2.0.8/README.md
+-rw-r--r--   0 harcok     (501) staff       (20)     2665 2024-05-19 06:36:16.000000 ev3dev2simulator-2.0.8/pyproject.toml
+-rw-r--r--   0 harcok     (501) staff       (20)       38 2024-05-19 14:37:18.374158 ev3dev2simulator-2.0.8/setup.cfg
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.329469 ev3dev2simulator-2.0.8/src/
+-rw-r--r--   0 harcok     (501) staff       (20)     5033 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/bluetooth.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.334762 ev3dev2simulator-2.0.8/src/ev3dev2/
+-rw-r--r--   0 harcok     (501) staff       (20)     6864 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/__init__.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.335314 ev3dev2simulator-2.0.8/src/ev3dev2/_platform/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/_platform/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2284 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/_platform/ev3.py
+-rw-r--r--   0 harcok     (501) staff       (20)      626 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/auto.py
+-rw-r--r--   0 harcok     (501) staff       (20)     8935 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/button.py
+-rw-r--r--   0 harcok     (501) staff       (20)     6032 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/console.py
+-rw-r--r--   0 harcok     (501) staff       (20)    10393 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/display.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.335569 ev3dev2simulator-2.0.8/src/ev3dev2/fonts/
+-rw-r--r--   0 harcok     (501) staff       (20)      935 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/fonts/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)    16482 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/led.py
+-rw-r--r--   0 harcok     (501) staff       (20)    72743 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/motor.py
+-rw-r--r--   0 harcok     (501) staff       (20)     5664 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/port.py
+-rw-r--r--   0 harcok     (501) staff       (20)     3257 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/power.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.336096 ev3dev2simulator-2.0.8/src/ev3dev2/sensor/
+-rw-r--r--   0 harcok     (501) staff       (20)     7394 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/sensor/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)    30430 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/sensor/lego.py
+-rw-r--r--   0 harcok     (501) staff       (20)    25098 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/sound.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1909 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/stopwatch.py
+-rw-r--r--   0 harcok     (501) staff       (20)     5836 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/unit.py
+-rw-r--r--   0 harcok     (501) staff       (20)       27 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/version.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1646 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2/wheel.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.337052 ev3dev2simulator-2.0.8/src/ev3dev2simulator/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1395 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/__main__.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.328033 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.345967 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/
+-rw-r--r--   0 harcok     (501) staff       (20)     1264 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/arm.png
+-rw-r--r--   0 harcok     (501) staff       (20)     5175 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/arm_large.png
+-rw-r--r--   0 harcok     (501) staff       (20)    10434 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/body.png
+-rw-r--r--   0 harcok     (501) staff       (20)   122910 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/bottle.png
+-rw-r--r--   0 harcok     (501) staff       (20)    59554 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/brick.png
+-rw-r--r--   0 harcok     (501) staff       (20)     1460 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_black.png
+-rw-r--r--   0 harcok     (501) staff       (20)     2391 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_blue.png
+-rw-r--r--   0 harcok     (501) staff       (20)     2423 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_green.png
+-rw-r--r--   0 harcok     (501) staff       (20)     2401 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_red.png
+-rw-r--r--   0 harcok     (501) staff       (20)     2272 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_white.png
+-rw-r--r--   0 harcok     (501) staff       (20)     2382 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_yellow.png
+-rw-r--r--   0 harcok     (501) staff       (20)     1362 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_amber.png
+-rw-r--r--   0 harcok     (501) staff       (20)     1338 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_black.png
+-rw-r--r--   0 harcok     (501) staff       (20)     1473 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_green.png
+-rw-r--r--   0 harcok     (501) staff       (20)     1459 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_orange.png
+-rw-r--r--   0 harcok     (501) staff       (20)     1391 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_red.png
+-rw-r--r--   0 harcok     (501) staff       (20)     1389 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_yellow.png
+-rw-r--r--   0 harcok     (501) staff       (20)     2925 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/touch_sensor_left.png
+-rw-r--r--   0 harcok     (501) staff       (20)     1422 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/touch_sensor_rear.png
+-rw-r--r--   0 harcok     (501) staff       (20)     2869 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/touch_sensor_right.png
+-rw-r--r--   0 harcok     (501) staff       (20)     4315 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/ultrasonic_sensor_bottom.png
+-rw-r--r--   0 harcok     (501) staff       (20)     2808 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/ultrasonic_sensor_top.png
+-rw-r--r--   0 harcok     (501) staff       (20)     2771 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/wheel.png
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.346847 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)     4034 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/config.py
+-rw-r--r--   0 harcok     (501) staff       (20)     5655 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/config_checker.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.347261 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/robot_configurations/
+-rw-r--r--   0 harcok     (501) staff       (20)     1619 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/robot_configurations/large_robot.yaml
+-rw-r--r--   0 harcok     (501) staff       (20)      861 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/robot_configurations/small_robot.yaml
+-rw-r--r--   0 harcok     (501) staff       (20)     2637 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/simulation_settings.yaml
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.348061 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/world_configurations/
+-rw-r--r--   0 harcok     (501) staff       (20)      952 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/world_configurations/config_large.yaml
+-rw-r--r--   0 harcok     (501) staff       (20)     1049 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/world_configurations/config_large2.yaml
+-rw-r--r--   0 harcok     (501) staff       (20)      804 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/world_configurations/config_small.yaml
+-rw-r--r--   0 harcok     (501) staff       (20)      901 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/world_configurations/config_small2.yaml
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.349091 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)     3214 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/client_socket.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2125 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/client_socket_handler.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.354771 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)      384 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/command.py
+-rw-r--r--   0 harcok     (501) staff       (20)      681 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/config_request.py
+-rw-r--r--   0 harcok     (501) staff       (20)      495 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/data_request.py
+-rw-r--r--   0 harcok     (501) staff       (20)      840 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/led_command.py
+-rw-r--r--   0 harcok     (501) staff       (20)      709 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/motor_command.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1856 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/rotate_command.py
+-rw-r--r--   0 harcok     (501) staff       (20)      809 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/sound_command.py
+-rw-r--r--   0 harcok     (501) staff       (20)      929 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/stop_command.py
+-rw-r--r--   0 harcok     (501) staff       (20)     5177 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message_handler.py
+-rw-r--r--   0 harcok     (501) staff       (20)     3779 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/server_sockets.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.356774 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1316 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/device_connector.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1042 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/led_connector.py
+-rw-r--r--   0 harcok     (501) staff       (20)     4960 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/motor_connector.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2118 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/sensor_connector.py
+-rw-r--r--   0 harcok     (501) staff       (20)     7785 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/sound_connector.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.362916 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)      789 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/arm_floor.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2340 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/board.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1609 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/border.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2983 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/border_obstacle.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1700 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/bottle.py
+-rw-r--r--   0 harcok     (501) staff       (20)      746 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/color_obstacle.py
+-rw-r--r--   0 harcok     (501) staff       (20)      971 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/edge.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1417 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/hole.py
+-rw-r--r--   0 harcok     (501) staff       (20)     3981 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/lake.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1465 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/movable_object.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2637 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/rock.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.369039 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1366 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/arm.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2245 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/arm_large.py
+-rw-r--r--   0 harcok     (501) staff       (20)     3021 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/body_part.py
+-rw-r--r--   0 harcok     (501) staff       (20)      728 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/brick.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2281 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/color_sensor.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1486 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/led.py
+-rw-r--r--   0 harcok     (501) staff       (20)      995 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/speaker.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1733 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/touch_sensor.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2211 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/ultrasonic_sensor_bottom.py
+-rw-r--r--   0 harcok     (501) staff       (20)     4811 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/ultrasonic_sensor_top.py
+-rw-r--r--   0 harcok     (501) staff       (20)     1345 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/wheel.py
+-rw-r--r--   0 harcok     (501) staff       (20)     3013 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/simulator.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.371042 ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)     8584 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/message_processor.py
+-rw-r--r--   0 harcok     (501) staff       (20)     7062 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/motor_command_processor.py
+-rw-r--r--   0 harcok     (501) staff       (20)     8634 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/robot_simulator.py
+-rw-r--r--   0 harcok     (501) staff       (20)    15515 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/robot_state.py
+-rw-r--r--   0 harcok     (501) staff       (20)     3296 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/world_simulator.py
+-rw-r--r--   0 harcok     (501) staff       (20)     6252 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/world_state.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.372216 ev3dev2simulator-2.0.8/src/ev3dev2simulator/util/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/util/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)      388 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/util/dimensions.py
+-rw-r--r--   0 harcok     (501) staff       (20)     2246 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/util/instance_checker.py
+-rw-r--r--   0 harcok     (501) staff       (20)      222 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/util/point.py
+-rw-r--r--   0 harcok     (501) staff       (20)     3666 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/util/util.py
+-rw-r--r--   0 harcok     (501) staff       (20)      149 2024-05-19 14:37:08.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/version.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.373009 ev3dev2simulator-2.0.8/src/ev3dev2simulator/visualisation/
+-rw-r--r--   0 harcok     (501) staff       (20)        0 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/visualisation/__init__.py
+-rw-r--r--   0 harcok     (501) staff       (20)      777 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/visualisation/robot_part_sprite.py
+-rw-r--r--   0 harcok     (501) staff       (20)     4381 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/visualisation/sidebar.py
+-rw-r--r--   0 harcok     (501) staff       (20)    17348 2024-04-15 11:46:25.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator/visualisation/visualiser.py
+drwxr-xr-x   0 harcok     (501) staff       (20)        0 2024-05-19 14:37:18.373520 ev3dev2simulator-2.0.8/src/ev3dev2simulator.egg-info/
+-rw-r--r--   0 harcok     (501) staff       (20)     5043 2024-05-19 14:37:18.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator.egg-info/PKG-INFO
+-rw-r--r--   0 harcok     (501) staff       (20)     5484 2024-05-19 14:37:18.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 harcok     (501) staff       (20)        1 2024-05-19 14:37:18.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 harcok     (501) staff       (20)       68 2024-05-19 14:37:18.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator.egg-info/entry_points.txt
+-rw-r--r--   0 harcok     (501) staff       (20)      130 2024-05-19 14:37:18.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator.egg-info/requires.txt
+-rw-r--r--   0 harcok     (501) staff       (20)       35 2024-05-19 14:37:18.000000 ev3dev2simulator-2.0.8/src/ev3dev2simulator.egg-info/top_level.txt
```

### Comparing `ev3dev2simulator-2.0.7/LICENSE.txt` & `ev3dev2simulator-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/PKG-INFO` & `ev3dev2simulator-2.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ev3dev2simulator
-Version: 2.0.7
+Version: 2.0.8
 Summary: EV3 simulator for the ev3dev2 library
 Author: Sam Jansen, Niels Okker
 Author-email: Harco Kuppens <h.kuppens@cs.ru.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Harco Kuppens
         
@@ -70,27 +70,43 @@
 The thonny-ev3dev plugin for the Thonny IDE comes with the ev3dev2simulator.
 
 For more info about the thonny-ev3dev plugin see: https://github.com/ev3dev-python-tools/thonny-ev3dev/wiki <br>
 For more info about Thonny: http://thonny.org
 
 ## Getting started
    
-   The only prerequisites for the simulator are python 3.8.10 and pip. Simulating robot sound works out of the box for Windows and macOS users. Linux user need to install [espeak](http://espeak.sourceforge.net/).
+### Prerequisites needed only for Linux
+
    
-   First, for windows users it is strongly adviced to install **python 3.8.10**. For this python version the installation goes smoothly because there are precompiled binary wheels available for all dependencies. Newer versions of python will also work, but then you need a c build environment installed to build the c-code of the simpleaudio package. For macos and linux a c build environment is standard available and install with compiling c-code will not be a problem.  
+For Macos and Windows you don't need any prerequisites,
+but for linux you do.
+
+The pyttsx3  python speech library  uses system libraries in its implementation. For Macos/Windows the used system 'speak' libraries are always available, but for linux you must sure these are installed with:
+
+     sudo apt update && sudo apt install espeak ffmpeg libespeak1
+
+For linux there are is no binary distribution available for simpleaudio.
+          The Python 3 and ALSA development packages are required for pip to build the extension.
+          For Debian variants (including Raspbian), this will usually get the job done:
+
+     sudo apt-get install -y python3-dev libasound2-dev
+
 
-   Install python3
-      
-      Download Python 3.8.10 from the Python website (https://www.python.org/downloads/). 
-      Note: 3.8.10 is the latest 3.8 version with installers.
-      
-   Install with pip
+### Installation
+
+Install with pip:
    
       pip install ev3dev2simulator
      
-   Then you can just run the simulator by running the executable:
+For Windows and Macos all binary dependencies are provided by wheels on pypi, however for Linux the binary extenssion for simpleaudio is compiled when installing.
+     
+Then you can just run the simulator by running the executable:
    
       ev3dev2simulator
 
+The simulator works on all python versions 3.8 till python 3.12.
+
+   
+
 ## Using the simulator
 
 The user guide of the simulator can be found on the [wiki](https://github.com/ev3dev-python-tools/ev3dev2simulator/wiki).
```

### Comparing `ev3dev2simulator-2.0.7/README.md` & `ev3dev2simulator-2.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,43 @@
 The thonny-ev3dev plugin for the Thonny IDE comes with the ev3dev2simulator.
 
 For more info about the thonny-ev3dev plugin see: https://github.com/ev3dev-python-tools/thonny-ev3dev/wiki <br>
 For more info about Thonny: http://thonny.org
 
 ## Getting started
    
-   The only prerequisites for the simulator are python 3.8.10 and pip. Simulating robot sound works out of the box for Windows and macOS users. Linux user need to install [espeak](http://espeak.sourceforge.net/).
+### Prerequisites needed only for Linux
+
    
-   First, for windows users it is strongly adviced to install **python 3.8.10**. For this python version the installation goes smoothly because there are precompiled binary wheels available for all dependencies. Newer versions of python will also work, but then you need a c build environment installed to build the c-code of the simpleaudio package. For macos and linux a c build environment is standard available and install with compiling c-code will not be a problem.  
+For Macos and Windows you don't need any prerequisites,
+but for linux you do.
+
+The pyttsx3  python speech library  uses system libraries in its implementation. For Macos/Windows the used system 'speak' libraries are always available, but for linux you must sure these are installed with:
+
+     sudo apt update && sudo apt install espeak ffmpeg libespeak1
+
+For linux there are is no binary distribution available for simpleaudio.
+          The Python 3 and ALSA development packages are required for pip to build the extension.
+          For Debian variants (including Raspbian), this will usually get the job done:
+
+     sudo apt-get install -y python3-dev libasound2-dev
+
 
-   Install python3
-      
-      Download Python 3.8.10 from the Python website (https://www.python.org/downloads/). 
-      Note: 3.8.10 is the latest 3.8 version with installers.
-      
-   Install with pip
+### Installation
+
+Install with pip:
    
       pip install ev3dev2simulator
      
-   Then you can just run the simulator by running the executable:
+For Windows and Macos all binary dependencies are provided by wheels on pypi, however for Linux the binary extenssion for simpleaudio is compiled when installing.
+     
+Then you can just run the simulator by running the executable:
    
       ev3dev2simulator
 
+The simulator works on all python versions 3.8 till python 3.12.
+
+   
+
 ## Using the simulator
 
 The user guide of the simulator can be found on the [wiki](https://github.com/ev3dev-python-tools/ev3dev2simulator/wiki).
```

### Comparing `ev3dev2simulator-2.0.7/pyproject.toml` & `ev3dev2simulator-2.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/bluetooth.py` & `ev3dev2simulator-2.0.8/src/bluetooth.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/__init__.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/__init__.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/_platform/ev3.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/_platform/ev3.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/auto.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/auto.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/button.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/button.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/console.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/console.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/display.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/display.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/fonts/__init__.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/led.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/led.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/motor.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/motor.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/port.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/port.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/power.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/power.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/sensor/__init__.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/sensor/lego.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/sensor/lego.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/sound.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/sound.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/stopwatch.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/stopwatch.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/unit.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/unit.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2/wheel.py` & `ev3dev2simulator-2.0.8/src/ev3dev2/wheel.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/__main__.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/__main__.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/arm.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/arm.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/arm_large.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/arm_large.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/body.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/body.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/bottle.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/bottle.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/brick.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/brick.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_black.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_black.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_blue.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_blue.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_green.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_green.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_red.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_red.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_white.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_white.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/color_sensor_yellow.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/color_sensor_yellow.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_amber.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_amber.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_black.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_black.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_green.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_green.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_orange.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_orange.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_red.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_red.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/led_yellow.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/led_yellow.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/touch_sensor_left.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/touch_sensor_left.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/touch_sensor_rear.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/touch_sensor_rear.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/touch_sensor_right.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/touch_sensor_right.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/ultrasonic_sensor_bottom.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/ultrasonic_sensor_bottom.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/ultrasonic_sensor_top.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/ultrasonic_sensor_top.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/assets/images/wheel.png` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/assets/images/wheel.png`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/config.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/config.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/config_checker.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/config_checker.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/robot_configurations/large_robot.yaml` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/robot_configurations/large_robot.yaml`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/robot_configurations/small_robot.yaml` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/robot_configurations/small_robot.yaml`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/simulation_settings.yaml` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/simulation_settings.yaml`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/world_configurations/config_large.yaml` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/world_configurations/config_large.yaml`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/world_configurations/config_large2.yaml` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/world_configurations/config_large2.yaml`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/world_configurations/config_small.yaml` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/world_configurations/config_small.yaml`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/config/world_configurations/config_small2.yaml` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/config/world_configurations/config_small2.yaml`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/client_socket.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/client_socket.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/client_socket_handler.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/client_socket_handler.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/config_request.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/config_request.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/led_command.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/led_command.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/motor_command.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/motor_command.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/rotate_command.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/rotate_command.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/sound_command.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/sound_command.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message/stop_command.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message/stop_command.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/message_handler.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/message_handler.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connection/server_sockets.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connection/server_sockets.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/device_connector.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/device_connector.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/led_connector.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/led_connector.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/motor_connector.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/motor_connector.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/sensor_connector.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/sensor_connector.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/connector/sound_connector.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/connector/sound_connector.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/arm_floor.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/arm_floor.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/board.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/board.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/border.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/border.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/border_obstacle.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/border_obstacle.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/bottle.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/bottle.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/color_obstacle.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/color_obstacle.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/edge.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/edge.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/hole.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/hole.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/lake.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/lake.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/movable_object.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/movable_object.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/obstacle/rock.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/obstacle/rock.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/arm.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/arm.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/arm_large.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/arm_large.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/body_part.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/body_part.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/brick.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/brick.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/color_sensor.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/color_sensor.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/led.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/led.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/speaker.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/speaker.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/touch_sensor.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/touch_sensor.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/ultrasonic_sensor_bottom.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/ultrasonic_sensor_bottom.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/ultrasonic_sensor_top.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/ultrasonic_sensor_top.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/robotpart/wheel.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/robotpart/wheel.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/simulator.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/message_processor.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/message_processor.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/motor_command_processor.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/motor_command_processor.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/robot_simulator.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/robot_simulator.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/robot_state.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/robot_state.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/world_simulator.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/world_simulator.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/state/world_state.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/state/world_state.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/util/instance_checker.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/util/instance_checker.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/util/util.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/util/util.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/visualisation/robot_part_sprite.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/visualisation/robot_part_sprite.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/visualisation/sidebar.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/visualisation/sidebar.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator/visualisation/visualiser.py` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator/visualisation/visualiser.py`

 * *Files identical despite different names*

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator.egg-info/PKG-INFO` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ev3dev2simulator
-Version: 2.0.7
+Version: 2.0.8
 Summary: EV3 simulator for the ev3dev2 library
 Author: Sam Jansen, Niels Okker
 Author-email: Harco Kuppens <h.kuppens@cs.ru.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Harco Kuppens
         
@@ -70,27 +70,43 @@
 The thonny-ev3dev plugin for the Thonny IDE comes with the ev3dev2simulator.
 
 For more info about the thonny-ev3dev plugin see: https://github.com/ev3dev-python-tools/thonny-ev3dev/wiki <br>
 For more info about Thonny: http://thonny.org
 
 ## Getting started
    
-   The only prerequisites for the simulator are python 3.8.10 and pip. Simulating robot sound works out of the box for Windows and macOS users. Linux user need to install [espeak](http://espeak.sourceforge.net/).
+### Prerequisites needed only for Linux
+
    
-   First, for windows users it is strongly adviced to install **python 3.8.10**. For this python version the installation goes smoothly because there are precompiled binary wheels available for all dependencies. Newer versions of python will also work, but then you need a c build environment installed to build the c-code of the simpleaudio package. For macos and linux a c build environment is standard available and install with compiling c-code will not be a problem.  
+For Macos and Windows you don't need any prerequisites,
+but for linux you do.
+
+The pyttsx3  python speech library  uses system libraries in its implementation. For Macos/Windows the used system 'speak' libraries are always available, but for linux you must sure these are installed with:
+
+     sudo apt update && sudo apt install espeak ffmpeg libespeak1
+
+For linux there are is no binary distribution available for simpleaudio.
+          The Python 3 and ALSA development packages are required for pip to build the extension.
+          For Debian variants (including Raspbian), this will usually get the job done:
+
+     sudo apt-get install -y python3-dev libasound2-dev
+
 
-   Install python3
-      
-      Download Python 3.8.10 from the Python website (https://www.python.org/downloads/). 
-      Note: 3.8.10 is the latest 3.8 version with installers.
-      
-   Install with pip
+### Installation
+
+Install with pip:
    
       pip install ev3dev2simulator
      
-   Then you can just run the simulator by running the executable:
+For Windows and Macos all binary dependencies are provided by wheels on pypi, however for Linux the binary extenssion for simpleaudio is compiled when installing.
+     
+Then you can just run the simulator by running the executable:
    
       ev3dev2simulator
 
+The simulator works on all python versions 3.8 till python 3.12.
+
+   
+
 ## Using the simulator
 
 The user guide of the simulator can be found on the [wiki](https://github.com/ev3dev-python-tools/ev3dev2simulator/wiki).
```

### Comparing `ev3dev2simulator-2.0.7/src/ev3dev2simulator.egg-info/SOURCES.txt` & `ev3dev2simulator-2.0.8/src/ev3dev2simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

