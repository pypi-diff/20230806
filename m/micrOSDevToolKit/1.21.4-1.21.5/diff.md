# Comparing `tmp/micrOSDevToolKit-1.21.4.tar.gz` & `tmp/micrOSDevToolKit-1.21.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.21.4.tar", last modified: Fri Aug  4 12:17:36 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.21.5.tar", last modified: Sun Aug  6 19:17:14 2023, max compression
```

## Comparing `micrOSDevToolKit-1.21.4.tar` & `micrOSDevToolKit-1.21.5.tar`

### file list

```diff
@@ -1,277 +1,277 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.621102 micrOSDevToolKit-1.21.4/
--rw-r--r--   0 bnm        (501) staff       (20)      358 2023-08-03 17:06:55.000000 micrOSDevToolKit-1.21.4/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-08-04 12:17:36.620602 micrOSDevToolKit-1.21.4/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.21.4/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.21.4/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.101214 micrOSDevToolKit-1.21.4/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.094636 micrOSDevToolKit-1.21.4/env/driver_cp210x/
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.149070 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/
--rw-r--r--   0 bnm        (501) staff       (20)  1049848 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe
--rw-r--r--   0 bnm        (501) staff       (20)   924408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe
--rw-r--r--   0 bnm        (501) staff       (20)    25165 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt
--rw-r--r--   0 bnm        (501) staff       (20)     8370 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.150043 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/
--rw-r--r--   0 bnm        (501) staff       (20)    95408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.154247 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/
--rw-r--r--   0 bnm        (501) staff       (20)   111792 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml
--rw-r--r--   0 bnm        (501) staff       (20)    12624 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat
--rw-r--r--   0 bnm        (501) staff       (20)    10453 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.156811 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/
--rw-r--r--   0 bnm        (501) staff       (20)   110768 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.158785 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/
--rw-r--r--   0 bnm        (501) staff       (20)    98480 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.169938 micrOSDevToolKit-1.21.4/env/driver_cp210x/macOS_VCP_Driver/
--rwxr-xr-x   0 bnm        (501) staff       (20)  2004490 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg
--rwxr-xr-x   0 bnm        (501) staff       (20)    10569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.177094 micrOSDevToolKit-1.21.4/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.4/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.4/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.179780 micrOSDevToolKit-1.21.4/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.21.4/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.214173 micrOSDevToolKit-1.21.4/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.21.4/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.21.4/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.454550 micrOSDevToolKit-1.21.4/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.21.4/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6218 2023-08-02 12:29:26.000000 micrOSDevToolKit-1.21.4/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.21.4/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6443 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.4/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.21.4/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.21.4/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-08-04 11:01:34.000000 micrOSDevToolKit-1.21.4/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.21.4/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     3786 2023-08-01 19:30:57.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_aht10.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     3559 2023-08-02 17:26:12.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_lmpacman.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    19328 2023-07-26 14:42:47.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11897 2023-08-04 10:52:35.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     1629 2023-08-04 11:24:20.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_rgbcct.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.21.4/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.21.4/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.4/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.21.4/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.21.4/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.21.4/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.21.4/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-29 10:25:26.000000 micrOSDevToolKit-1.21.4/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-07-29 10:13:31.000000 micrOSDevToolKit-1.21.4/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.21.4/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.4/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.21.4/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.21.4/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.21.4/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.21.4/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.457634 micrOSDevToolKit-1.21.4/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-08-04 12:17:35.000000 micrOSDevToolKit-1.21.4/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     9934 2023-08-04 12:17:35.000000 micrOSDevToolKit-1.21.4/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-08-04 12:17:35.000000 micrOSDevToolKit-1.21.4/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-08-04 12:17:35.000000 micrOSDevToolKit-1.21.4/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-08-04 12:17:35.000000 micrOSDevToolKit-1.21.4/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-08-04 12:17:36.621249 micrOSDevToolKit-1.21.4/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-08-04 12:15:11.000000 micrOSDevToolKit-1.21.4/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.466662 micrOSDevToolKit-1.21.4/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.21.4/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.21.4/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.21.4/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.21.4/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.501520 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.506711 micrOSDevToolKit-1.21.4/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.21.4/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.21.4/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.21.4/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.21.4/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.534348 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.566565 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7455 2023-08-02 12:44:06.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5415 2023-08-01 19:28:24.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4828 2023-08-02 12:43:56.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6584 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.21.4/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.567488 micrOSDevToolKit-1.21.4/toolkit/user_data/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.21.4/toolkit/user_data/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.567921 micrOSDevToolKit-1.21.4/toolkit/user_data/node_config_archive/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/user_data/node_config_archive/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.568323 micrOSDevToolKit-1.21.4/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-04 12:17:36.619068 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1990 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      759 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     1297 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_aht10.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1193 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_lmpacman.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6191 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3501 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      557 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_rgbcct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5718 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-08-04 12:02:42.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-08-04 12:02:43.000000 micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.535475 micrOSDevToolKit-1.21.5/
+-rw-r--r--   0 bnm        (501) staff       (20)      358 2023-08-03 17:06:55.000000 micrOSDevToolKit-1.21.5/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-06 19:17:14.534935 micrOSDevToolKit-1.21.5/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45495 2023-08-05 00:33:02.000000 micrOSDevToolKit-1.21.5/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.21.5/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.113460 micrOSDevToolKit-1.21.5/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.107223 micrOSDevToolKit-1.21.5/env/driver_cp210x/
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.155197 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/
+-rw-r--r--   0 bnm        (501) staff       (20)  1049848 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe
+-rw-r--r--   0 bnm        (501) staff       (20)   924408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe
+-rw-r--r--   0 bnm        (501) staff       (20)    25165 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt
+-rw-r--r--   0 bnm        (501) staff       (20)     8370 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.157739 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/
+-rw-r--r--   0 bnm        (501) staff       (20)    95408 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.160306 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/
+-rw-r--r--   0 bnm        (501) staff       (20)   111792 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml
+-rw-r--r--   0 bnm        (501) staff       (20)    12624 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat
+-rw-r--r--   0 bnm        (501) staff       (20)    10453 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.162763 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/
+-rw-r--r--   0 bnm        (501) staff       (20)   110768 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.173232 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/
+-rw-r--r--   0 bnm        (501) staff       (20)    98480 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.192409 micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/
+-rwxr-xr-x   0 bnm        (501) staff       (20)  2004490 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg
+-rwxr-xr-x   0 bnm        (501) staff       (20)    10569 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.207922 micrOSDevToolKit-1.21.5/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.5/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.5/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.214175 micrOSDevToolKit-1.21.5/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.21.5/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.246400 micrOSDevToolKit-1.21.5/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.311374 micrOSDevToolKit-1.21.5/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.21.5/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6218 2023-08-02 12:29:26.000000 micrOSDevToolKit-1.21.5/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.21.5/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6443 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.5/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.21.5/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.21.5/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-08-06 19:04:54.000000 micrOSDevToolKit-1.21.5/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.21.5/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3786 2023-08-01 19:30:57.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_aht10.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3559 2023-08-02 17:26:12.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19504 2023-08-04 14:14:52.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11897 2023-08-04 10:52:35.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1629 2023-08-04 11:24:20.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_rgbcct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.5/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.21.5/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.21.5/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.21.5/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.21.5/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-29 10:25:26.000000 micrOSDevToolKit-1.21.5/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-08-06 19:01:22.000000 micrOSDevToolKit-1.21.5/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.21.5/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.5/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.21.5/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.21.5/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.21.5/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.21.5/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.314783 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    55058 2023-08-06 19:17:13.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     9934 2023-08-06 19:17:14.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-08-06 19:17:13.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-08-06 19:17:13.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-08-06 19:17:13.000000 micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-08-06 19:17:14.535640 micrOSDevToolKit-1.21.5/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-08-06 19:12:41.000000 micrOSDevToolKit-1.21.5/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.340715 micrOSDevToolKit-1.21.5/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.21.5/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.21.5/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.21.5/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.21.5/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.429294 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.434325 micrOSDevToolKit-1.21.5/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.21.5/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.21.5/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.21.5/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.21.5/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.454203 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.488318 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7455 2023-08-02 12:44:06.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5415 2023-08-01 19:28:24.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4828 2023-08-02 12:43:56.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6584 2023-08-01 19:27:35.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.21.5/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.489151 micrOSDevToolKit-1.21.5/toolkit/user_data/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.21.5/toolkit/user_data/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.489530 micrOSDevToolKit-1.21.5/toolkit/user_data/node_config_archive/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/user_data/node_config_archive/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.489887 micrOSDevToolKit-1.21.5/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-08-06 19:17:14.533491 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1990 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1297 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_aht10.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1193 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6207 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3501 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      557 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rgbcct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5714 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-08-06 19:13:33.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-08-06 19:13:32.000000 micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.21.4/PKG-INFO` & `micrOSDevToolKit-1.21.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.21.4
+Version: 1.21.5
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
@@ -551,21 +551,22 @@
         > Secure Core (OTA static modules): `boot.py`, `micrOSloader.mpy`, `Network.mpy`, `ConfigHandler.mpy`, `Debug.mpy`
         
         
         ### RELESE NOTE
         
         |  VERSION (TAG) |    RELEASE INFO    |  MICROS CORE MEMORY USAGE  |  SUPPORTED DEVICE(S) | APP PROFILES | Load Modules  |     NOTE       |
         | :----------: | :----------------: | :------------------------:   |  :-----------------: | :------------: | :------------:| -------------- |
-        |  **v0.1.0-0** | [release_Info-0.1.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.1.0-0_note.md)| 13 - 28 % (1216-2544byte) | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.1.0-0.json)| Stable Core with applications - first release
-        |  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp8266.md)| 26 - 53 % (2512-5072byte) | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| micrOS multi device support with finalized core and so more. OTA update feature.
-        |  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp32.md)| 23 - 28 % (17250-20976byte) | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| *micrOS multi device support with finalized core and advanced task scheduler based on time, and and so more. OTA update feature.*
-        |  **v1.0.0-0** | [release_Info-1.0.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.0.0-0_note_esp32.md)| 15 - 23 % (10394-15488byte) | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.0.0-0.json)| Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA, etc.
-        |  **v1.2.2-0** | [release_Info-1.2.2-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.2.2-0_note_esp32.md)|  10-25 % | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.2.2-0.json)| Public Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA update, thread from socket shell (beta) etc.
+        |  **v0.1.0-0** | [release_Info-0.1.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.1.0-0_note.md)| **78,4%** 29 776 byte | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.1.0-0.json)| Stable Core with applications - first release
+        |  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp8266.md)| **81,0%** 30768 byte | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| micrOS multi device support with finalized core and so more. OTA update feature.
+        |  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp32.md)| **47,1%** 52 416 byte | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| *micrOS multi device support with finalized core and advanced task scheduler based on time, and and so more. OTA update feature.*
+        |  **v1.0.0-0** | [release_Info-1.0.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.0.0-0_note_esp32.md)| **47,9%** 53 280 byte | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.0.0-0.json)| Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA, etc.
+        |  **v1.2.2-0** | [release_Info-1.2.2-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.2.2-0_note_esp32.md)|  **48,6%** 54 032 byte | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.2.2-0.json)| Public Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA update, thread from socket shell (beta) etc.
         |  **v light-1.3.0-0** | - |  - | **esp8266** | [lightweight branch](https://github.com/BxNxM/micrOS/tree/lightweight)| - |remove esp8266 due to memory limitation - BUT still supported with limited functionalities on **`lightweight`** branch. Hint: Change branch on github and download zip file, then start micrOSDevToolKit dashboard GUI
-        |  **v 1.5.0-1** | [release_Info-1.5.0-1](./micrOS/release_info/micrOS_ReleaseInfo/release_1.5.0-1_note_esp32.md) |  5-14% (6176-16192 byte) | esp32, tinyPico | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.5.0-1.json) | Advanced Timer IRQ based scheduling (cron & timirq), Geolocation based timing features, External IRQs with 4 channel (event filtering), finalized light controls, Device-Device comminucation support, etc.
+        |  **v 1.5.0-1** | [release_Info-1.5.0-1](./micrOS/release_info/micrOS_ReleaseInfo/release_1.5.0-1_note_esp32.md) |  **58,2%** 64 704 byte | esp32 (tinyPico) | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.5.0-1.json) | Advanced Timer IRQ based scheduling (cron & timirq), Geolocation based timing features, External IRQs with 4 channel (event filtering), finalized light controls, Device-Device comminucation support, etc.
+        |  **v 1.21.0-4** | [release_Info-1.21.0-4](./micrOS/release_info/micrOS_ReleaseInfo/release_1.21.0-4_note_esp32.md) |  **57.3%** 63 728 byte | esp32 (tinyPico, esp32s2, esp32s3) | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.21.0-4.json) | Full async core system with advanced task management and device to device communication, task scheduling and much more ... with more then 30 application/pheriphery support.
         
         
         ----------------------------------------
         ----------------------------------------
         
         
         ## Developer Quick guide
```

### Comparing `micrOSDevToolKit-1.21.4/README.md` & `micrOSDevToolKit-1.21.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -541,21 +541,22 @@
 > Secure Core (OTA static modules): `boot.py`, `micrOSloader.mpy`, `Network.mpy`, `ConfigHandler.mpy`, `Debug.mpy`
 
 
 ### RELESE NOTE
 
 |  VERSION (TAG) |    RELEASE INFO    |  MICROS CORE MEMORY USAGE  |  SUPPORTED DEVICE(S) | APP PROFILES | Load Modules  |     NOTE       |
 | :----------: | :----------------: | :------------------------:   |  :-----------------: | :------------: | :------------:| -------------- |
-|  **v0.1.0-0** | [release_Info-0.1.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.1.0-0_note.md)| 13 - 28 % (1216-2544byte) | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.1.0-0.json)| Stable Core with applications - first release
-|  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp8266.md)| 26 - 53 % (2512-5072byte) | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| micrOS multi device support with finalized core and so more. OTA update feature.
-|  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp32.md)| 23 - 28 % (17250-20976byte) | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| *micrOS multi device support with finalized core and advanced task scheduler based on time, and and so more. OTA update feature.*
-|  **v1.0.0-0** | [release_Info-1.0.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.0.0-0_note_esp32.md)| 15 - 23 % (10394-15488byte) | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.0.0-0.json)| Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA, etc.
-|  **v1.2.2-0** | [release_Info-1.2.2-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.2.2-0_note_esp32.md)|  10-25 % | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.2.2-0.json)| Public Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA update, thread from socket shell (beta) etc.
+|  **v0.1.0-0** | [release_Info-0.1.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.1.0-0_note.md)| **78,4%** 29 776 byte | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.1.0-0.json)| Stable Core with applications - first release
+|  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp8266.md)| **81,0%** 30768 byte | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| micrOS multi device support with finalized core and so more. OTA update feature.
+|  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp32.md)| **47,1%** 52 416 byte | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| *micrOS multi device support with finalized core and advanced task scheduler based on time, and and so more. OTA update feature.*
+|  **v1.0.0-0** | [release_Info-1.0.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.0.0-0_note_esp32.md)| **47,9%** 53 280 byte | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.0.0-0.json)| Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA, etc.
+|  **v1.2.2-0** | [release_Info-1.2.2-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.2.2-0_note_esp32.md)|  **48,6%** 54 032 byte | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.2.2-0.json)| Public Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA update, thread from socket shell (beta) etc.
 |  **v light-1.3.0-0** | - |  - | **esp8266** | [lightweight branch](https://github.com/BxNxM/micrOS/tree/lightweight)| - |remove esp8266 due to memory limitation - BUT still supported with limited functionalities on **`lightweight`** branch. Hint: Change branch on github and download zip file, then start micrOSDevToolKit dashboard GUI
-|  **v 1.5.0-1** | [release_Info-1.5.0-1](./micrOS/release_info/micrOS_ReleaseInfo/release_1.5.0-1_note_esp32.md) |  5-14% (6176-16192 byte) | esp32, tinyPico | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.5.0-1.json) | Advanced Timer IRQ based scheduling (cron & timirq), Geolocation based timing features, External IRQs with 4 channel (event filtering), finalized light controls, Device-Device comminucation support, etc.
+|  **v 1.5.0-1** | [release_Info-1.5.0-1](./micrOS/release_info/micrOS_ReleaseInfo/release_1.5.0-1_note_esp32.md) |  **58,2%** 64 704 byte | esp32 (tinyPico) | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.5.0-1.json) | Advanced Timer IRQ based scheduling (cron & timirq), Geolocation based timing features, External IRQs with 4 channel (event filtering), finalized light controls, Device-Device comminucation support, etc.
+|  **v 1.21.0-4** | [release_Info-1.21.0-4](./micrOS/release_info/micrOS_ReleaseInfo/release_1.21.0-4_note_esp32.md) |  **57.3%** 63 728 byte | esp32 (tinyPico, esp32s2, esp32s3) | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.21.0-4.json) | Full async core system with advanced task management and device to device communication, task scheduling and much more ... with more then 30 application/pheriphery support.
 
 
 ----------------------------------------
 ----------------------------------------
 
 
 ## Developer Quick guide
```

### Comparing `micrOSDevToolKit-1.21.4/devToolKit.py` & `micrOSDevToolKit-1.21.5/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x64.exe`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210xVCPInstaller_x86.exe`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/CP210x_Universal_Windows_Driver_ReleaseNotes.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/SLAB_License_Agreement_VCP_Windows.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/arm64/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/dpinst.xml`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.cat`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/silabser.inf`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x64/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/CP210x_Universal_Windows_Driver/x86/silabser.sys`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/SiLabsUSBDriverDisk.dmg`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt` & `micrOSDevToolKit-1.21.5/env/driver_cp210x/macOS_VCP_Driver/macOS_VCP_Driver_Release_Notes.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/media/dnd.png` & `micrOSDevToolKit-1.21.5/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/media/logo.png` & `micrOSDevToolKit-1.21.5/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/media/logo_mini.png` & `micrOSDevToolKit-1.21.5/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.21.5/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.5/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.5/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.21.5/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.21.5/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.5/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.21.5/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/Common.py` & `micrOSDevToolKit-1.21.5/micrOS/source/Common.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.21.5/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/Debug.py` & `micrOSDevToolKit-1.21.5/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.21.5/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.21.5/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.21.5/micrOS/source/InterpreterShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.21.0-4'
+    MICROS_VERSION = '1.21.1-0'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply('msg')
         """
         self.msg_obj = msg_obj
```

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.21.5/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_aht10.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_aht10.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_lmpacman.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_lmpacman.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_oled_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,39 +46,43 @@
         else:
             errlog_add(f"Oled UI unknown oled_type: {oled_type}")
             Exception(f"Oled UI unknown oled_type: {oled_type}")
         self.page_callback_list = page_callbacks
         self.active_page = page
         self.width = w
         self.height = h
+        self.oled_state = True      # ON-True, OFF-False
+
+        # Message box - message text and msgbox blink effect
         self.show_msg = None
         self.blink_effect = False
-        self.oled_state = True
-        # OK/CENTER button state values
-        self.bttn_press_callback = None
+
         # Intercon connection state values
         self.open_intercons = []
         self.cmd_out = "n/a"
         self.cmd_task_tag = None
-        # Create built-in event/button IRQ
+
+        # Create built-in button IRQ - OK button (center)
+        self.bttn_press_callback = None
         self.irq_ok = False
         self.__create_button_irq()
+
         # Power saver state machine - turn off sec, deltaT (timirq executor seq loop), counter
         self.pwr_saver_state = [pwr_sec, round(cfgget('timirqseq') / 1000, 2), pwr_sec]
+
         # Store instance - use as singleton
         PageUI.PAGE_UI_OBJ = self
 
     #############################
     #        INTERNAL MAGIC     #
     #############################
     def __page_header(self):
         """Generates header bar with NW mode + Clock + wifi rssi"""
 
-        def __draw_rssi():
-            value = WLAN(STA_IF).status('rssi')
+        def __draw_rssi(value):
             show_range = round(((value + 91) / 30) * 8)  # pixel height 8
             PageUI.DISPLAY.line(self.width - 10, 8, self.width - 8, 8)
             PageUI.DISPLAY.line(self.width - 17, 1, self.width, 1)
             for _h in range(0, show_range):
                 PageUI.DISPLAY.line(118 - _h, 8 - _h, 120 + _h, 8 - _h)
 
         def __pwr_off():
@@ -87,15 +91,15 @@
             if sec is None:
                 return
             indicator = round(cnt / sec, 1) * 8       # pixel height 8
             for i in range(indicator):
                 PageUI.DISPLAY.line(self.width-x_offset, 6-i, self.width-x_offset-2, 6-i)
 
         try:
-            __draw_rssi()
+            __draw_rssi(value=WLAN(STA_IF).status('rssi'))
             __pwr_off()
         except:
             pass
 
         ltime = localtime()
         h = "0{}".format(ltime[-5]) if len(str(ltime[-5])) < 2 else ltime[-5]
         m = "0{}".format(ltime[-4]) if len(str(ltime[-4])) < 2 else ltime[-4]
@@ -153,14 +157,17 @@
         if pin:
             pin_obj = Pin(pin, Pin.IN, Pin.PULL_DOWN)
             # [IRQ] - event type setup
             pin_obj.irq(trigger=Pin.IRQ_RISING, handler=lambda pin: self.control('press'))
             self.irq_ok = True
 
     def __power_save(self):
+        """
+        Automatically put screen to off after self.pwr_saver_state[2] (counter) is 0
+        """
         sec, dt, cnt = self.pwr_saver_state
         if sec is None:
             # Power saver off - no auto turn off
             return
         if cnt > 0:
             self.pwr_saver_state[2] = cnt - dt
         else:
@@ -172,15 +179,15 @@
     #############################
     def add_page(self, page_callback):
         if page_callback in self.page_callback_list:
             return True
         self.page_callback_list.append(page_callback)
         return True
 
-    def show_page(self):
+    def render_page(self):
         """Re/draw active page"""
         PageUI.DISPLAY.clean()
         msg_event = self.__msgbox()
         if self.oled_state:
             self.__page_header()
             self.__page_bar()
             if not msg_event:
@@ -201,23 +208,23 @@
             """Simulate button press"""
             self._page_button_press()  # Execute button callback
         elif cmd.strip() == 'next':
             """Change page - next & Draw"""
             self.active_page += 1
             if self.active_page > len(self.page_callback_list) - 1:
                 self.active_page = 0
-            self.show_page()
+            self.render_page()
             self.bttn_press_callback = None
             self.cmd_out = 'n/a'
         elif cmd.strip() == 'prev':
             """Change page - previous & Draw"""
             self.active_page -= 1
             if self.active_page < 0:
                 self.active_page = len(self.page_callback_list) - 1
-            self.show_page()
+            self.render_page()
             self.bttn_press_callback = None
             self.cmd_out = 'n/a'
         elif cmd.strip() == 'on':
             PageUI.DISPLAY.poweron()
             self.oled_state = True
         elif cmd.strip() == 'off':
             PageUI.DISPLAY.poweroff()
@@ -445,15 +452,15 @@
     :param pwr_sec: power down oled after given sec - power safe
     :param oled_type: oled type selection: ssd1306 or sh1106
     :param page: start page index, start from 0
     """
     if PageUI.PAGE_UI_OBJ is None:
         pages = [_sys_page, _intercon_cache, _adc_page, _micros_welcome]  # <== Add page function HERE
         PageUI(pages, 128, 64, page=page, pwr_sec=pwr_sec, oled_type=oled_type)
-    PageUI.PAGE_UI_OBJ.show_page()
+    PageUI.PAGE_UI_OBJ.render_page()
 
 
 def control(cmd='next'):
     """
     OLED UI control
     :param cmd str: next, prev, press, on, off
     :return str: verdict
@@ -466,15 +473,15 @@
 
 def msgbox(msg='micrOS msg'):
     """
     POP-UP message function
     :param msg: message string
     """
     PageUI.PAGE_UI_OBJ.show_msg = msg
-    PageUI.PAGE_UI_OBJ.show_page()
+    PageUI.PAGE_UI_OBJ.render_page()
     return 'Show msg'
 
 
 def intercon_genpage(cmd=None, run=False):
     """
     Create intercon pages dynamically :)
     - based on cmd value.
```

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_rgbcct.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_rgbcct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.21.5/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/Network.py` & `micrOSDevToolKit-1.21.5/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/Notify.py` & `micrOSDevToolKit-1.21.5/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.21.5/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.21.5/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.21.5/micrOS/source/TaskManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,18 +58,17 @@
 
     def __task_del(self, keep_cache=False):
         """
         Delete task from TASKS
         """
         self.done.set()
         if self.tag in Task.TASKS.keys():
-            if keep_cache:              # True - In case of destructor
+            if not keep_cache:              # True - In case of destructor
                 del Task.TASKS[self.tag]
-            del self.task
-        collect()                       # GC collect
+        collect()                           # GC collect
 
     def __enter__(self):
         """
         START CONDITION
         Helper function for Task creation in Load Modules
         [HINT] Use python with feature to utilize this feature
         """
@@ -96,15 +95,15 @@
         if Task.is_busy(self.tag):
             # Skip task if already running
             return False
 
         # Start task with coroutine callback
         self.task = asyncio.get_event_loop().create_task(callback)
         # Store Task object by key - for task control
-        Task.TASKS[tag] = self
+        Task.TASKS[self.tag] = self
         return True
 
     def create_lm(self, callback=None, loop=None, sleep=None):
         """
         Create async task with function callback (with queue limit check)
         - wrap (sync) function into async task (task_wrapper)
         - callback: <load_module> <function> <param> <param2>
@@ -303,15 +302,15 @@
 
     @staticmethod
     def kill(tag):
         """
         Primary interface
         Kill/terminate async task
         - by tag: module.function
-        - by killall, module-tag: module.*
+        - by tag module.*, kill all for selected module
         """
 
         def terminate(_tag):
             to_kill = Task.TASKS.get(_tag, None)
             try:
                 return False if to_kill is None else to_kill.cancel()
             except Exception as e:
```

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/Time.py` & `micrOSDevToolKit-1.21.5/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.21.5/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.21.5/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.21.5/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOS/source/urequests.py` & `micrOSDevToolKit-1.21.5/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.21.4
+Version: 1.21.5
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
@@ -551,21 +551,22 @@
         > Secure Core (OTA static modules): `boot.py`, `micrOSloader.mpy`, `Network.mpy`, `ConfigHandler.mpy`, `Debug.mpy`
         
         
         ### RELESE NOTE
         
         |  VERSION (TAG) |    RELEASE INFO    |  MICROS CORE MEMORY USAGE  |  SUPPORTED DEVICE(S) | APP PROFILES | Load Modules  |     NOTE       |
         | :----------: | :----------------: | :------------------------:   |  :-----------------: | :------------: | :------------:| -------------- |
-        |  **v0.1.0-0** | [release_Info-0.1.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.1.0-0_note.md)| 13 - 28 % (1216-2544byte) | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.1.0-0.json)| Stable Core with applications - first release
-        |  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp8266.md)| 26 - 53 % (2512-5072byte) | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| micrOS multi device support with finalized core and so more. OTA update feature.
-        |  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp32.md)| 23 - 28 % (17250-20976byte) | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| *micrOS multi device support with finalized core and advanced task scheduler based on time, and and so more. OTA update feature.*
-        |  **v1.0.0-0** | [release_Info-1.0.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.0.0-0_note_esp32.md)| 15 - 23 % (10394-15488byte) | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.0.0-0.json)| Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA, etc.
-        |  **v1.2.2-0** | [release_Info-1.2.2-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.2.2-0_note_esp32.md)|  10-25 % | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.2.2-0.json)| Public Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA update, thread from socket shell (beta) etc.
+        |  **v0.1.0-0** | [release_Info-0.1.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.1.0-0_note.md)| **78,4%** 29 776 byte | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.1.0-0.json)| Stable Core with applications - first release
+        |  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp8266.md)| **81,0%** 30768 byte | esp8266 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| micrOS multi device support with finalized core and so more. OTA update feature.
+        |  **v0.4.0-0** | [release_Info-0.4.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_0.4.0-0_note_esp32.md)| **47,1%** 52 416 byte | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_0.4.0-0.json)| *micrOS multi device support with finalized core and advanced task scheduler based on time, and and so more. OTA update feature.*
+        |  **v1.0.0-0** | [release_Info-1.0.0-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.0.0-0_note_esp32.md)| **47,9%** 53 280 byte | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.0.0-0.json)| Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA, etc.
+        |  **v1.2.2-0** | [release_Info-1.2.2-0](./micrOS/release_info/micrOS_ReleaseInfo/release_1.2.2-0_note_esp32.md)|  **48,6%** 54 032 byte | esp32 | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.2.2-0.json)| Public Release of v1 micrOS, timer and event based irqs, cron task scheduling, realtime communication, multiple device support. OTA update, thread from socket shell (beta) etc.
         |  **v light-1.3.0-0** | - |  - | **esp8266** | [lightweight branch](https://github.com/BxNxM/micrOS/tree/lightweight)| - |remove esp8266 due to memory limitation - BUT still supported with limited functionalities on **`lightweight`** branch. Hint: Change branch on github and download zip file, then start micrOSDevToolKit dashboard GUI
-        |  **v 1.5.0-1** | [release_Info-1.5.0-1](./micrOS/release_info/micrOS_ReleaseInfo/release_1.5.0-1_note_esp32.md) |  5-14% (6176-16192 byte) | esp32, tinyPico | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.5.0-1.json) | Advanced Timer IRQ based scheduling (cron & timirq), Geolocation based timing features, External IRQs with 4 channel (event filtering), finalized light controls, Device-Device comminucation support, etc.
+        |  **v 1.5.0-1** | [release_Info-1.5.0-1](./micrOS/release_info/micrOS_ReleaseInfo/release_1.5.0-1_note_esp32.md) |  **58,2%** 64 704 byte | esp32 (tinyPico) | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.5.0-1.json) | Advanced Timer IRQ based scheduling (cron & timirq), Geolocation based timing features, External IRQs with 4 channel (event filtering), finalized light controls, Device-Device comminucation support, etc.
+        |  **v 1.21.0-4** | [release_Info-1.21.0-4](./micrOS/release_info/micrOS_ReleaseInfo/release_1.21.0-4_note_esp32.md) |  **57.3%** 63 728 byte | esp32 (tinyPico, esp32s2, esp32s3) | [App Profiles](./micrOS/release_info/node_config_profiles/) | [LM manual](./micrOS/client/sfuncman/sfuncman_1.21.0-4.json) | Full async core system with advanced task management and device to device communication, task scheduling and much more ... with more then 30 application/pheriphery support.
         
         
         ----------------------------------------
         ----------------------------------------
         
         
         ## Developer Quick guide
```

### Comparing `micrOSDevToolKit-1.21.4/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.21.5/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/setup.py` & `micrOSDevToolKit-1.21.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.21.4',
+    version='1.21.5',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.21.4/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.21.5/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.21.5/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.21.5/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/Gateway.py` & `micrOSDevToolKit-1.21.5/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.21.5/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.21.5/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.21.5/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.21.5/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.21.5/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.21.5/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.21.5/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.21.5/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.21.5/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/socketClient.py` & `micrOSDevToolKit-1.21.5/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Debug.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 1473 6f66 745f  ug..reset..soft_
 000000a0: 7265 7365 7400 0e6d 6163 6869 6e65 000a  reset..machine..
-000000b0: 5368 656c 6c00 1031 2e32 312e 302d 3400  Shell..1.21.0-4.
+000000b0: 5368 656c 6c00 1031 2e32 312e 312d 3000  Shell..1.21.1-0.
 000000c0: 230e 6d73 675f 6f62 6a00 0c64 6576 6669  #.msg_obj..devfi
 000000d0: 6400 105f 5f64 6576 6669 6400 0861 7574  d..__devfid..aut
 000000e0: 6800 165f 5f61 7574 685f 6d6f 6465 000a  h..__auth_mode..
 000000f0: 6877 7569 6400 0e5f 5f68 7775 6964 0012  hwuid..__hwuid..
 00000100: 5f5f 6175 7468 5f6f 6b00 165f 5f63 6f6e  __auth_ok..__con
 00000110: 665f 6d6f 6465 000e 7665 7273 696f 6e00  f_mode..version.
 00000120: 1c4d 4943 524f 535f 5645 5253 494f 4e00  .MICROS_VERSION.
```

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_aht10.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_aht10.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_lmpacman.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_lmpacman.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 4d06 001f 813a 0f1a 4c4d 5f6f 6c65 645f  M....:..LM_oled_
+00000000: 4d06 001f 813b 0f1a 4c4d 5f6f 6c65 645f  M....;..LM_oled_
 00000010: 7569 2e70 7900 0f0c 6366 6767 6574 001a  ui.py...cfgget..
 00000020: 436f 6e66 6967 4861 6e64 6c65 7200 126c  ConfigHandler..l
 00000030: 6f63 616c 7469 6d65 000a 736c 6565 7000  ocaltime..sleep.
 00000040: 0a75 7469 6d65 0008 574c 414e 000c 5354  .utime..WLAN..ST
 00000050: 415f 4946 000e 6e65 7477 6f72 6b00 1870  A_IF..network..p
 00000060: 6879 7369 6361 6c5f 7069 6e00 1670 696e  hysical_pin..pin
 00000070: 6d61 705f 6475 6d70 0016 4c6f 6769 6361  map_dump..Logica
@@ -30,358 +30,359 @@
 000001d0: 0014 6d69 6372 4f53 2047 5549 0016 5041  ..micrOS GUI..PA
 000001e0: 4745 5f55 495f 4f42 4a00 2473 6574 5f70  GE_UI_OBJ.$set_p
 000001f0: 7265 7373 5f63 616c 6c62 6163 6b00 125f  ress_callback.._
 00000200: 6164 635f 7061 6765 0008 6e75 6c6c 0008  adc_page..null..
 00000210: 766f 6c74 000c 6765 6e61 6463 0002 7000  volt..genadc..p.
 00000220: 087b 7d20 2500 087b 7d20 5600 0c70 6167  .{} %..{} V..pag
 00000230: 6575 6900 0870 6167 6500 0e70 7772 5f73  eui..page..pwr_s
-00000240: 6563 0012 6f6c 6564 5f74 7970 6500 1273  ec..oled_type..s
-00000250: 686f 775f 7061 6765 000e 636f 6e74 726f  how_page..contro
-00000260: 6c00 0c6d 7367 626f 7800 1073 686f 775f  l..msgbox..show_
-00000270: 6d73 6700 1053 686f 7720 6d73 6700 2069  msg..Show msg. i
-00000280: 6e74 6572 636f 6e5f 6765 6e70 6167 6500  ntercon_genpage.
-00000290: 0910 6164 645f 7061 6765 0016 636d 645f  ..add_page..cmd_
-000002a0: 6765 6e70 6167 6500 0a6c 6d64 6570 000c  genpage..lmdep..
-000002b0: 7069 6e6d 6170 0082 3f08 6865 6c70 0023  pinmap..?.help.#
-000002c0: 8231 0e4c 4d5f 6f6c 6564 001c 4c4d 5f6f  .1.LM_oled..LM_o
-000002d0: 6c65 645f 7368 3131 3036 0024 7061 6765  led_sh1106.$page
-000002e0: 5f63 616c 6c62 6163 6b5f 6c69 7374 0016  _callback_list..
-000002f0: 6163 7469 7665 5f70 6167 6500 0a77 6964  active_page..wid
-00000300: 7468 000c 6865 6967 6874 0018 626c 696e  th..height..blin
-00000310: 6b5f 6566 6665 6374 0014 6f6c 6564 5f73  k_effect..oled_s
-00000320: 7461 7465 0026 6274 746e 5f70 7265 7373  tate.&bttn_press
-00000330: 5f63 616c 6c62 6163 6b00 1c6f 7065 6e5f  _callback..open_
-00000340: 696e 7465 7263 6f6e 7300 066e 2f61 000e  intercons..n/a..
-00000350: 636d 645f 6f75 7400 1863 6d64 5f74 6173  cmd_out..cmd_tas
-00000360: 6b5f 7461 6700 0c69 7271 5f6f 6b00 265f  k_tag..irq_ok.&_
-00000370: 5f63 7265 6174 655f 6275 7474 6f6e 5f69  _create_button_i
-00000380: 7271 0012 7469 6d69 7271 7365 7100 1e70  rq..timirqseq..p
-00000390: 7772 5f73 6176 6572 5f73 7461 7465 001a  wr_saver_state..
-000003a0: 5f5f 7061 6765 5f68 6561 6465 7200 0630  __page_header..0
-000003b0: 7b7d 0002 3000 0b02 2100 145f 5f70 6167  {}..0...!..__pag
-000003c0: 655f 6261 7200 0872 6563 7400 105f 5f6d  e_bar..rect..__m
-000003d0: 7367 626f 7800 0e70 6f77 6572 6f6e 000a  sgbox..poweron..
-000003e0: 7374 6174 6500 0449 4e00 1250 554c 4c5f  state..IN..PULL_
-000003f0: 444f 574e 0006 6972 7100 0e74 7269 6767  DOWN..irq..trigg
-00000400: 6572 0014 4952 515f 5249 5349 4e47 000e  er..IRQ_RISING..
-00000410: 6861 6e64 6c65 7200 185f 5f70 6f77 6572  handler..__power
-00000420: 5f73 6176 6500 066f 6666 0079 0a63 6c65  _save..off.y.cle
-00000430: 616e 0008 7368 6f77 000a 7072 6573 7300  an..show..press.
-00000440: 245f 7061 6765 5f62 7574 746f 6e5f 7072  $_page_button_pr
-00000450: 6573 7300 0870 7265 7600 046f 6e00 1070  ess..prev..on..p
-00000460: 6f77 6572 6f66 6600 0653 3a31 0006 533a  oweroff..S:1..S:
-00000470: 3000 125f 636d 645f 7465 7874 001a 696e  0.._cmd_text..in
-00000480: 7465 7263 6f6e 5f70 6167 6500 0674 6167  tercon_page..tag
-00000490: 0082 0303 06c2 ba43 0002 4300 086b 696c  .......C..C..kil
-000004a0: 6c00 1a63 6d64 5f63 616c 6c5f 7061 6765  l..cmd_call_page
-000004b0: 0014 3c6c 6973 7463 6f6d 703e 000e 5f62  ..<listcomp>.._b
-000004c0: 7574 746f 6e00 1048 454c 4c4f 203a 4400  utton..HELLO :D.
-000004d0: 165f 5f76 6973 7561 6c69 7a65 0008 6669  .__visualize..fi
-000004e0: 6c6c 0020 5f5f 7267 625f 6272 6967 6874  ll. __rgb_bright
-000004f0: 6e65 7373 000e 6d6f 6475 6c65 7300 0673  ness..modules..s
-00000500: 7973 000c 4c4d 5f72 6762 0081 5514 6272  ys..LM_rgb..U.br
-00000510: 6967 6874 6e65 7373 000c 736d 6f6f 7468  ightness..smooth
-00000520: 0010 3c6c 616d 6264 613e 0006 7275 6e00  ..<lambda>..run.
-00000530: 165f 5f64 7261 775f 7273 7369 000c 7374  .__draw_rssi..st
-00000540: 6174 7573 0008 7273 7369 0008 6c69 6e65  atus..rssi..line
-00000550: 0012 5f5f 7077 725f 6f66 6600 105f 5f65  ..__pwr_off..__e
-00000560: 6666 6563 7400 1073 656e 645f 636d 6400  ffect..send_cmd.
-00000570: 0e76 6572 6469 6374 0082 010e 5f62 7566  .verdict...._buf
-00000580: 6665 7200 0c6d 7367 6f62 6a00 1049 6e74  fer..msgobj..Int
-00000590: 6572 436f 6e00 2f2d 3581 3d14 6c69 6e65  erCon./-5.=.line
-000005a0: 5f6c 696d 6974 0082 3349 822f 0663 6d64  _limit..3I./.cmd
-000005b0: 0006 6d73 6700 8143 8177 8213 1c70 6167  ..msg..C.w...pag
-000005c0: 655f 6361 6c6c 6261 636b 7300 0277 0002  e_callbacks..w..
-000005d0: 6800 820d 8157 8179 0c70 696e 6b65 7900  h....W.y.pinkey.
-000005e0: 1a70 6167 655f 6361 6c6c 6261 636b 0010  .page_callback..
-000005f0: 6361 6c6c 6261 636b 0002 7800 0279 0008  callback..x..y..
-00000600: 686f 7374 0006 7069 6e00 050c 2020 7b7d  host..pin...  {}
-00000610: 2520 287b 7d6b 6229 0005 0e49 6e74 6572  % ({}kb)...Inter
-00000620: 436f 6e20 6361 6368 6500 0a05 0504 6e65  Con cache.....ne
-00000630: 7874 0005 0470 7265 7600 0505 7072 6573  xt...prev...pres
-00000640: 7300 0502 6f6e 0005 036f 6666 0005 1c49  s...on...off...I
-00000650: 6e76 616c 6964 2063 6f6d 6d61 6e64 207b  nvalid command {
-00000660: 7d21 2048 696e 743a 207b 7d00 0a03 0504  }! Hint: {}.....
-00000670: 6f6c 6564 0005 0869 6e74 6572 636f 6e00  oled...intercon.
-00000680: 0505 6765 6e49 4f00 0a06 0541 7061 6765  ..genIO....Apage
-00000690: 7569 2070 6167 653d 3020 7077 725f 7365  ui page=0 pwr_se
-000006a0: 633d 4e6f 6e65 2f69 6e74 2873 6563 2920  c=None/int(sec) 
-000006b0: 6f6c 6564 5f74 7970 653d 2273 7364 3133  oled_type="ssd13
-000006c0: 3036 206f 7220 7368 3131 3036 2200 051e  06 or sh1106"...
-000006d0: 636f 6e74 726f 6c20 6e65 7874 2f70 7265  control next/pre
-000006e0: 762f 7072 6573 732f 6f6e 2f6f 6666 0005  v/press/on/off..
-000006f0: 0c6d 7367 626f 7820 226d 7367 2200 0527  .msgbox "msg"..'
-00000700: 696e 7465 7263 6f6e 5f67 656e 7061 6765  intercon_genpage
-00000710: 2022 686f 7374 2220 2263 6d64 2220 7275   "host" "cmd" ru
-00000720: 6e3d 4661 6c73 6500 051b 636d 645f 6765  n=False...cmd_ge
-00000730: 6e70 6167 6520 2263 6d64 2220 7275 6e3d  npage "cmd" run=
-00000740: 4661 6c73 6500 0506 7069 6e6d 6170 000a  False...pinmap..
-00000750: 0205 0773 7364 3133 3036 0005 0673 6831  ...ssd1306...sh1
-00000760: 3130 3600 051d 4f6c 6564 2055 4920 756e  106...Oled UI un
-00000770: 6b6e 6f77 6e20 6f6c 6564 5f74 7970 653a  known oled_type:
-00000780: 207b 7d00 050e 7b7d 207b 7d20 7b7d 3a7b   {}...{} {} {}:{
-00000790: 7d3a 7b7d 0005 165b 4552 525d 2042 7574  }:{}...[ERR] But
-000007a0: 746f 6e20 4952 513a 7b7d 207b 7d00 0510  ton IRQ:{} {}...
-000007b0: 7061 6765 3a20 7b7d 2070 7772 3a20 7b7d  page: {} pwr: {}
-000007c0: 000a 0207 0238 3407 0234 350a 0207 0135  .....84..45....5
-000007d0: 0702 3132 0804 302e 3031 050c 5461 736b  ..12..0.01..Task
-000007e0: 2069 7320 4275 7379 0094 041c 5601 2c32   is Busy....V.,2
-000007f0: 3232 2c2c 2c32 224f 2622 4a27 224f 8607  22,,,2"O&"J'"O..
-00000800: 9945 840d 8813 840f 842a 8b0e 890c 890a  .E.......*......
-00000810: 8916 891b 8409 840c 8010 022a 011b 031c  ...........*....
-00000820: 0216 0259 8010 0410 052a 021b 061c 0416  ...Y.....*......
-00000830: 041c 0516 0559 8010 0710 082a 021b 091c  .....Y.....*....
-00000840: 0716 071c 0816 0859 8010 0a10 0b2a 021b  .......Y.....*..
-00000850: 0c1c 0a16 0a1c 0b16 0b59 8010 0d2a 011b  .........Y...*..
-00000860: 0e1c 0d16 0d59 8010 0f2a 011b 101c 0f16  .....Y...*......
-00000870: 0f59 8010 112a 011b 121c 1116 1159 8010  .Y...*.......Y..
-00000880: 1310 142a 021b 151c 1316 131c 1416 1459  ...*...........Y
-00000890: 480e 8010 162a 011b 171c 1616 1659 4a07  H....*.......YJ.
-000008a0: 5951 1616 4a01 5d48 0980 511b 1816 811f  YQ..J.]H..Q.....
-000008b0: 4a08 5951 1681 1f4a 015d 480e 8010 192a  J.YQ...J.]H....*
-000008c0: 011b 1a1c 1916 1959 4a07 5951 1619 4a01  .......YJ.YQ..J.
-000008d0: 5d54 3200 101b 3402 161b 3201 1620 832a  ]T2...4...2.. .*
-000008e0: 0153 3302 162a 3203 1632 3204 1636 5110  .S3..*2..22..6Q.
-000008f0: 1c80 2a03 5333 0516 3d10 1d2a 0153 3306  ..*.S3..=..*.S3.
-00000900: 1642 101e 2a01 5333 0716 4351 502a 0253  .B..*.S3..CQP*.S
-00000910: 3308 1646 5150 2a02 5333 0916 4932 0a16  3..FQP*.S3..I2..
-00000920: 4a32 0b16 4b32 0c16 4d51 630d 880c 103e  J2..K2..MQc....>
-00000930: 1b8b 1b23 438b 2a84 2384 0a84 1b89 0e84  ...#C.*.#.......
-00000940: 0e64 6084 0f84 2284 0d84 1384 1288 2911  .d`...".......).
-00000950: 8120 1681 2110 1b16 8122 5116 3451 1621  . ..!...."Q.4Q.!
-00000960: 8051 101c 2a03 5333 0016 4e32 0116 6132  .Q..*.S3..N2..a2
-00000970: 0216 6632 0316 6810 1f2a 0153 3304 165e  ..f2..h..*.S3..^
-00000980: 3205 1671 3206 1648 3207 1641 3208 1642  2..q2..H2..A2..B
-00000990: 3209 1677 320a 1635 320b 167d 502a 0153  2..w2..52..}P*.S
-000009a0: 330c 167e 502a 0153 330d 1681 0551 630e  3..~P*.S3....Qc.
-000009b0: 8b78 db85 014a 4e81 2c81 2d81 2e81 2f3e  .x...JN.,.-.../>
-000009c0: 3f40 801f 8008 2a2a 4725 472c 2d24 2424  ?@....**G%G,-$$$
-000009d0: 2424 2444 4425 2544 2446 57b6 144f 3600  $$$DD%%D$FW..O6.
-000009e0: 2306 dd44 5db6 144f 3600 101c d944 4780  #..D]..O6....DG.
-000009f0: 511b 50c7 4245 8051 1b51 c7b7 121b 1821  Q.P.BE.Q.Q.....!
-00000a00: 4259 120f 2307 1425 b636 0134 0159 1281  BY..#..%.6.4.Y..
-00000a10: 2623 0714 25b6 3601 3401 59b1 b018 52b4  &#..%.6.4.Y...R.
-00000a20: b018 53b2 b018 54b3 b018 5551 b018 4450  ..S...T...UQ..DP
-00000a30: b018 5652 b018 5751 b018 582b 00b0 1859  ..VR..WQ..X+...Y
-00000a40: 105a b018 5b51 b018 5c50 b018 5db0 145e  .Z..[Q..\P..]..^
-00000a50: 3600 59b5 1281 3012 0210 5f34 0122 8768  6.Y...0..._4.".h
-00000a60: f782 3402 b52b 03b0 1860 b012 1b18 3451  ..4..+...`....4Q
-00000a70: 638e 2c8d 1031 6181 2c80 4940 8508 8509  c.,..1a.,.I@....
-00000a80: 2224 4743 251f 211f 211f 2127 3239 00b0  "$GC%.!.!.!'29..
-00000a90: 2000 01c1 b020 0101 c248 0ab1 3400 59b2   .... ...H..4.Y.
-00000aa0: 3400 594a 0459 4a01 5d12 0434 00c3 1281  4.YJ.YJ.]..4....
-00000ab0: 3112 8127 b37b 5534 0134 0182 d744 4b10  1..'.{U4.4...DK.
-00000ac0: 6214 25b3 7b55 3601 4243 b37b 55c4 1281  b.%.{U6.BC.{U...
-00000ad0: 3112 8127 b37c 5534 0134 0182 d744 4b10  1..'.|U4.4...DK.
-00000ae0: 6214 25b3 7c55 3601 4243 b37c 55c5 1281  b.%.|U6.BC.|U...
-00000af0: 3112 8127 b37d 5534 0134 0182 d744 4b10  1..'.}U4.4...DK.
-00000b00: 6214 25b3 7d55 3601 4243 b37d 55c6 120d  b.%.}U6.BC.}U...
-00000b10: 3400 8055 c712 8131 b734 0180 d844 45b7  4..U...1.4...DE.
-00000b20: 8055 4242 1063 c725 0013 5851 de44 4410  .UBB.c.%..XQ.DD.
-00000b30: 4742 4c25 0013 5d44 4410 6442 4210 65c8  GBL%..]DD.dBB.e.
-00000b40: 121b 1321 1422 2308 1425 b7b8 b4b5 b636  ...!."#..%.....6
-00000b50: 0580 8036 0359 5163 0288 1861 1481 1464  ...6.YQc...a...d
-00000b60: 804c 2f2f 3836 2612 0712 0834 0114 8115  .L//86&....4....
-00000b70: 1081 1636 01c1 1281 30b1 2280 5bf2 9ef7  ...6....0.".[...
-00000b80: 88f4 3401 c212 1b13 2114 8117 2500 1354  ..4.....!...%..T
-00000b90: 8af3 8825 0013 5488 f388 3604 5912 1b13  ...%..T...6.Y...
-00000ba0: 2114 8117 2500 1354 91f3 8125 0013 5481  !...%..T...%..T.
-00000bb0: 3604 59b2 8042 5e57 c312 1b13 2114 8117  6.Y..B^W....!...
-00000bc0: 2280 76b3 f388 b3f3 2280 78b3 f288 b3f3  ".v.....".x.....
-00000bd0: 3604 5981 e558 5ad7 431d 5959 5163 8550  6.Y..XZ.C.YYQc.P
-00000be0: 7916 8118 6480 5422 2925 222c 269d c125  y...d.T")%",&..%
-00000bf0: 0013 6030 03c2 c3c4 b251 de44 4251 6312  ..`0.....Q.DBQc.
-00000c00: 8130 b4b2 f781 3402 88f4 c5b5 8042 6257  .0....4......BbW
-00000c10: c612 1b13 2114 8117 2500 1354 b1f3 86b6  ....!...%..T....
-00000c20: f325 0013 54b1 f382 f386 b6f3 3604 5981  .%..T.......6.Y.
-00000c30: e558 5ad7 4319 5959 5163 8618 6914 6681  .XZ.C.YYQc..i.f.
-00000c40: 2c80 6c20 2950 2e55 1281 31b0 1352 3401  ,.l )P.U..1..R4.
-00000c50: c112 8123 1281 30b0 1354 b1f7 3401 3401  ...#..0..T..4.4.
-00000c60: c212 8132 80b0 1354 b234 035f 4b16 c312  ...2...T.4._K...
-00000c70: 1b13 2114 67b3 b013 5585 f3b2 81f3 8436  ..!.g...U......6
-00000c80: 0459 4228 121b 1321 1467 b013 53b2 f481  .YB(...!.g..S...
-00000c90: f2b0 1355 84f3 b282 f382 3604 5951 6389  ...U......6.YQc.
-00000ca0: 3c59 2968 812c 8076 6540 2545 2246 2945  <Y)h.,.ve@%E"F)E
-00000cb0: 5324 4a31 2754 2c00 b020 0001 c125 0013  S$J1'T,.. ...%..
-00000cc0: 44c2 b251 de44 4250 6325 0013 5743 4e12  D..Q.DBPc%..WCN.
-00000cd0: 1b13 2114 6936 0059 5225 0018 5712 1b13  ..!.i6.YR%..W...
-00000ce0: 2114 678a 8f22 806c a810 6a81 3682 0459  !.g..".l..j.6..Y
-00000cf0: b134 0059 1281 31b2 3401 8ad8 446c 121b  .4.Y..1.4...Dl..
-00000d00: 1321 1422 b280 8a2e 0255 8f99 3603 59b2  .!.".....U..6.Y.
-00000d10: 8a51 2e02 55c3 1281 31b3 3401 8cd8 4448  .Q..U...1.4...DH
-00000d20: b351 8b2e 0255 4241 b3c2 121b 1321 1422  .Q...UBA.....!."
-00000d30: b28f a836 0359 5263 0184 4051 0e81 1964  ...6.YRc..@Q...d
-00000d40: 8077 293a 2500 1356 d325 0018 5612 1b13  .w):%..V.%..V...
-00000d50: 2114 6722 806a 9189 8510 6a81 1081 0a25  !.g".j....j....%
-00000d60: 0013 5636 8404 5912 1b13 2114 6722 806a  ..V6..Y...!.g".j
-00000d70: 9889 8910 6a81 1081 0a25 0013 5636 8404  ....j....%..V6..
-00000d80: 5951 6386 6ce2 0321 5e81 2c81 3380 9120  YQc.l..!^.,.3.. 
-00000d90: 2252 2922 2f23 4e33 0048 0812 0ab1 3401  "R)"/#N3.H....4.
-00000da0: c24a 2457 1281 26df 445c c349 1223 0914  .J$W..&.D\.I.#..
-00000db0: 25b1 b336 02c4 51c2 120f b434 0159 5151  %..6..Q....4.YQQ
-00000dc0: c328 035d 4a01 5db2 4466 1211 b212 1113  .(.]J.].Df......
-00000dd0: 6b12 1113 6c34 03c5 b514 6d10 6e12 1113  k...l4....m.n...
-00000de0: 6f10 70b0 2000 0136 8400 5952 2500 185d  o.p. ..6..YR%..]
-00000df0: 5163 0181 1022 0e81 1264 8139 809b 2500  Qc..."...d.9..%.
-00000e00: 1442 1076 3601 6383 5831 1671 812c 809f  .B.v6.c.X1.q.,..
-00000e10: 2845 2225 4a28 b013 6030 03c1 c2c3 b151  (E"%J(..`0.....Q
-00000e20: de44 4251 63b3 80d8 444a b3b2 f3b0 1360  .DBQc...DJ.....`
-00000e30: 8256 424e b014 4210 7236 0159 b1b0 1360  .VBN..B.r6.Y...`
-00000e40: 8256 5163 8200 2214 4881 2c81 3480 ad27  .VQc..".H.,.4..'
-00000e50: 2229 b1b0 1352 dd44 4252 63b0 1352 1473  ")...R.DBRc..R.s
-00000e60: b136 0159 5263 8658 2120 4181 2c80 b320  .6.YRc.X! A.,.. 
-00000e70: 2926 2626 2623 304a 2a29 121b 1321 1474  )&&&&#0J*)...!.t
-00000e80: 3600 59b0 1468 3600 c1b0 1357 44c2 80b0  6.Y..h6....WD...
-00000e90: 1461 3600 59b0 1466 3600 59b1 4364 b013  .a6.Y..f6.Y.Cd..
-00000ea0: 5312 8131 b013 5234 0181 f3d8 444a b013  S..1..R4....DJ..
-00000eb0: 5280 5534 0059 424a b013 52b0 1353 5534  R.U4.YBJ..R..SU4
-00000ec0: 0059 121b 1321 1475 3600 59b0 1471 3600  .Y...!.u6.Y..q6.
-00000ed0: 5951 638f 502a 4642 812c 8128 80c3 4a44  YQc.P*FB.,.(..JD
-00000ee0: 2a20 292a 2029 3024 2624 282a 2029 272d  * )* )0$&$(* )'-
-00000ef0: 2624 272a 2926 2a29 2426 b013 6080 55b0  &$'*)&*)$&..`.U.
-00000f00: 1360 8256 51b0 1844 b114 4f36 0010 76d9  .`.VQ..D..O6..v.
-00000f10: 4449 b014 7736 0059 42a7 81b1 144f 3600  DI..w6.YB....O6.
-00000f20: 101d d944 6fb0 5713 5381 e55a 1853 b013  ...Do.W.S..Z.S..
-00000f30: 5312 8131 b013 5234 0181 f3d8 4444 80b0  S..1..R4....DD..
-00000f40: 1853 b014 4136 0059 51b0 1858 105a b018  .S..A6.YQ..X.Z..
-00000f50: 5b42 ee80 b114 4f36 0010 78d9 446e b057  [B....O6..x.Dn.W
-00000f60: 1353 81e6 5a18 53b0 1353 80d7 444d 1281  .S..Z.S..S..DM..
-00000f70: 31b0 1352 3401 81f3 b018 53b0 1441 3600  1..R4.....S..A6.
-00000f80: 5951 b018 5810 5ab0 185b 4276 b114 4f36  YQ..X.Z..[Bv..O6
-00000f90: 0010 79d9 444f 121b 1321 1469 3600 5952  ..y.DO...!.i6.YR
-00000fa0: b018 5742 5db1 144f 3600 1072 d944 5312  ..WB]..O6..r.DS.
-00000fb0: 1b13 2114 7a36 0059 50b0 1857 51b0 1858  ..!.z6.YP..WQ..X
-00000fc0: 4240 230a 1425 b013 53b0 1357 3602 6382  B@#..%..S..W6.c.
-00000fd0: 0811 1477 812c 80e4 6040 2742 46b0 1358  ...w.,..`@'BF..X
-00000fe0: 51de 4442 5163 b014 5836 0059 51b0 1858  Q.DBQc..X6.YQ..X
-00000ff0: 5163 8720 5222 3581 2c81 3580 f120 6426  Qc. R"5.,.5.. d&
-00001000: 316d 2826 2866 27b1 b018 5823 0b30 02c2  1m(&(f'...X#.0..
-00001010: c312 1b13 2114 67b2 83f3 b383 f3ae 8e36  ....!.g........6
-00001020: 0459 121b 1321 1422 1076 b2b3 3603 5910  .Y...!.".v..6.Y.
-00001030: 7bb0 135b dd44 4652 b018 5642 5510 7cb0  {..[.DFR..VBU.|.
-00001040: 135b dd44 4650 b018 5642 47b0 1356 d3b0  .[.DFP..VBG..V..
-00001050: 1856 121b 1321 1467 b282 f3b3 82f3 ac8c  .V...!.g........
-00001060: b013 5636 0559 5163 8a00 4b22 7d81 2c81  ..V6.YQc..K"}.,.
-00001070: 3681 3790 0460 2034 2d35 335b 5712 8123  6.7..` 4-53[W..#
-00001080: 1281 30b0 1354 b1f3 88f7 3401 3401 81f3  ..0..T....4.4...
-00001090: c312 8131 b013 5b34 01b3 d844 da80 121b  ...1..[4...D....
-000010a0: 1321 1422 b013 5b80 b32e 0255 b1b2 8af2  .!."..[....U....
-000010b0: 3603 5912 8131 b013 5bb3 512e 0255 3401  6.Y..1..[.Q..U4.
-000010c0: b385 f3d8 445b 121b 1321 1422 b013 5bb3  ....D[...!."..[.
-000010d0: 82b3 f485 f32e 0255 b1b2 94f2 3603 5942  .......U....6.YB
-000010e0: 5512 1b13 2114 22b0 135b b351 2e02 55b1  U...!."..[.Q..U.
-000010f0: b294 f236 0359 4250 121b 1321 1422 b013  ...6.YBP...!."..
-00001100: 5bb1 b28a f236 0359 5163 8d34 e805 b880  [....6.YQc.4....
-00001110: 017e 812c 8138 8128 8113 9016 2046 880e  .~.,.8.(.... F..
-00001120: 2942 2d4f 2a3f 5050 5145 4b48 2400 0102  )B-O*?PPQEKH$...
-00001130: 0323 0c30 02c4 c5b0 b1b2 b320 0004 c625  .#.0....... ...%
-00001140: 0125 0013 59dd 4442 5163 121b 1321 1422  .%..Y.DBQc...!."
-00001150: 2501 80b5 3603 5912 1b13 2114 2225 02b4  %...6.Y...!."%..
-00001160: b58a f236 0359 2500 135c 51de d344 d580  ...6.Y%..\Q..D..
-00001170: 1281 2712 1434 0014 7510 7f25 0013 5c36  ..'..4..u..%..\6
-00001180: 8200 3401 1481 0010 4710 8101 3602 c7b7  ..4.....G...6...
-00001190: 51de d344 7012 8131 b734 0180 d844 66b7  Q..Dp..1.4...Df.
-000011a0: 1481 0010 8102 1081 0336 0225 0018 5b12  .........6.%..[.
-000011b0: 1434 0014 8104 107f 2500 135c 3682 0059  .4......%..\6..Y
-000011c0: 5125 0018 5c25 0014 7db4 b58a f236 0259  Q%..\%..}....6.Y
-000011d0: 2500 1435 b636 0159 2503 4444 b634 0059  %..5.6.Y%.DD.4.Y
-000011e0: 5163 0187 40d8 061e 8107 6464 6464 901b  Qc..@.....dddd..
-000011f0: 2b42 2d28 2e55 3325 0013 5914 7325 0136  +B-(.U3%..Y.s%.6
-00001200: 0159 482e 1281 1f14 811a 2501 2502 3602  .YH.......%.%.6.
-00001210: c4b4 107f 5525 0018 5c23 0eb4 1081 1b55  ....U%..\#.....U
-00001220: dd44 4d25 0343 49b4 1081 1b55 2500 185b  .DM%.CI....U%..[
-00001230: 4a1d 5712 8126 df44 55c5 490b 1281 27b5  J.W..&.DU.I...'.
-00001240: 3401 2500 185b 5151 c528 055d 4a01 5d25  4.%..[QQ.(.]J.]%
-00001250: 0013 5914 811c 2501 3601 5951 6385 2cdb  ..Y...%.6.YQc.,.
-00001260: 01a9 0181 0581 2c81 2881 1390 3f20 4666  ......,.(...? Ff
-00001270: 6087 0a2d 4948 2300 0106 230c 3002 c3c4  `..-IH#...#.0...
-00001280: b020 0001 2706 b0b1 b620 0103 c512 1b13  . ..'.... ......
-00001290: 2114 2225 0180 b436 0359 2500 147d b3b4  !."%...6.Y%..}..
-000012a0: 3602 5925 0014 35b5 3601 59b2 4444 b534  6.Y%..5.6.Y.DD.4
-000012b0: 0059 5163 0284 783e 1481 1d64 8129 9043  .YQc..x>...d.).C
-000012c0: 221f 5448 2b10 8101 142f b114 4f36 0014  ".TH+..../..O6..
-000012d0: 2d36 0036 0114 8100 1047 1081 0136 0214  -6.6.....G...6..
-000012e0: 8100 1081 0210 8103 3602 2500 185b 4a14  ........6.%..[J.
-000012f0: 5712 8126 df44 4c59 b114 4f36 0025 0018  W..&.DLY..O6.%..
-00001300: 5b4a 015d 5163 8440 d302 1681 0764 6464  [J.]Qc.@.....ddd
-00001310: 9049 2022 4b58 4819 2501 144f 3600 142d  .I "KXH.%..O6..-
-00001320: 3600 c312 13b3 1081 1e25 0234 8201 594a  6........%.4..YJ
-00001330: 1d57 1281 26df 4455 c449 0b12 8127 b434  .W..&.DU.I...'.4
-00001340: 0125 0018 5b51 51c4 2804 5d4a 015d 5163  .%..[QQ.(.]J.]Qc
-00001350: 8770 4016 2090 6060 3139 2725 1f23 3712  .p@. .``19'%.#7.
-00001360: 1b13 2114 2212 0210 2334 0180 8f36 0359  ..!."...#4...6.Y
-00001370: 121b 1321 1422 1024 1425 120d 3400 8155  ...!.".$.%..4..U
-00001380: 8055 3601 8099 3603 5912 1651 ded3 4467  .U6...6.Y..Q..Dg
-00001390: 1216 3400 c012 1b13 2114 2223 0014 25b0  ..4.....!."#..%.
-000013a0: 1026 5512 8123 b010 2755 2287 68f7 3401  .&U..#..'U".h.4.
-000013b0: 3602 80a3 3603 5912 1b13 2114 2210 2814  6...6.Y...!.".(.
-000013c0: 2512 0210 2934 0136 0180 ad36 0359 5263  %...)4.6...6.YRc
-000013d0: 8b0c f901 282a 8124 906d 2722 2222 2d35  ....(*.$.m'"""-5
-000013e0: 322a 3337 2425 2922 2f12 811f 51de 4442  2*37$%)"/...Q.DB
-000013f0: 5063 8fc1 81c2 121b 1321 1422 2301 80b1  Pc.......!."#...
-00001400: 3603 5912 8125 3200 1281 1f14 2b36 0034  6.Y..%2.....+6.4
-00001410: 0134 0180 d844 da80 1281 1f14 2b36 0014  .4...D......+6..
-00001420: 2c36 005f 4b4a 3002 c3c4 b314 2d10 2e36  ,6._KJ0.....-..6
-00001430: 0180 55c3 102e 142f b414 2d10 2e36 017e  ..U..../..-..6.~
-00001440: 512e 0255 3601 c412 1b13 2114 2210 3014  Q..U6.....!.".0.
-00001450: 25b4 b336 0280 b1b2 8af4 f236 0359 b281  %..6.......6.Y..
-00001460: e5c2 b2b0 d844 4659 5959 5942 4342 b47f  .....DFYYYYBCB..
-00001470: 5263 121b 1321 1422 1031 a8b1 94f2 3603  Rc...!.".1....6.
-00001480: 5952 6301 8120 390a 8106 6490 722b 00b0  YRc.. 9...d.r+..
-00001490: 5f4b 06c1 812f 1442 3863 843c b802 1432  _K.../.B8c.<...2
-000014a0: 9080 2063 4022 2d56 3032 00c0 4819 121b  .. c@"-V02..H...
-000014b0: 1321 1422 1033 9e8f 3603 5912 1b13 3414  .!.".3..6.Y...4.
-000014c0: 35b0 3601 594a 1a57 1281 26df 4452 c149  5.6.YJ.W..&.DR.I
-000014d0: 0812 8127 b134 0163 5151 c128 015d 4a01  ...'.4.cQQ.(.]J.
-000014e0: 5d52 6301 8208 200c 8107 9082 202e 121b  ]Rc... ..... ...
-000014f0: 1321 1422 1081 08a3 9d36 0359 121b 1321  .!.".....6.Y...!
-00001500: 1475 3600 5951 6387 4c40 1e36 908f 6083  .u6.YQc.L@.6..`.
-00001510: 0f83 082d 272b 2b37 3728 3200 c032 01c1  ...-'++77(2..2..
-00001520: 2c02 1037 1026 6210 3710 3862 c212 1951  ,..7.&b.7.8b...Q
-00001530: ded3 444b 1219 120a 1039 3401 3401 c2b0  ..DK.....94.4...
-00001540: 103a b210 2655 3482 0059 121b 1321 1422  .:..&U4..Y...!."
-00001550: 103b 1425 b210 2655 3601 2280 4194 3603  .;.%..&U6.".A.6.
-00001560: 5912 1b13 2114 2210 3c14 25b2 1038 5536  Y...!.".<.%..8U6
-00001570: 0122 8041 a836 0359 b1b2 1026 5534 0159  .".A.6.Y...&U4.Y
-00001580: 5263 0288 1089 101c 8109 3a90 9323 2529  Rc........:..#%)
-00001590: 4a52 292e 2553 2232 c1b0 230d f4c2 1281  JR).%S"2..#.....
-000015a0: 30b2 b1f4 3401 c3b3 81d7 4443 8142 41b3  0...4.....DC.BA.
-000015b0: c312 1b13 2114 6780 89b3 b310 810a 5236  ....!.g.......R6
-000015c0: 8204 5912 8123 b18a f734 01c4 1281 32b4  ..Y..#...4....2.
-000015d0: b181 f2b4 3403 5f4b 2cc5 b5b3 d744 5312  ....4._K,....DS.
-000015e0: 1b13 2114 6780 89b5 b510 6a80 3682 0459  ..!.g.....j.6..Y
-000015f0: 4251 121b 1321 1467 8089 b5b5 106a 8136  BQ...!.g.....j.6
-00001600: 8204 5942 1251 6384 3831 1481 0b26 90a2  ..YB.Qc.81...&..
-00001610: 2e2c 2e25 2280 1081 0c2a 011b 810d 1c81  .,.%"....*......
-00001620: 0cc1 5910 810e b114 810f 3600 dd44 5f80  ..Y.......6..D_.
-00001630: 1081 102a 011b 810e 1c81 10c2 59b0 51de  ...*........Y.Q.
-00001640: 4442 5163 b2b0 1081 1152 3482 0159 5163  DBQc.....R4..YQc
-00001650: 8418 eb81 0116 3d3f 403e 90b9 8007 282b  ......=?@>....(+
-00001660: 3612 1b13 3451 de44 6112 2012 2a12 3612  6...4Q.Da. .*.6.
-00001670: 322b 04c3 121b b322 8100 2280 4010 3eb2  2+....."..".@.>.
-00001680: 103f b010 40b1 3486 0359 121b 1334 1441  .?..@.4..Y...4.A
-00001690: 3600 5951 6382 40a9 0114 4281 2890 c760  6.YQc.@...B.(..`
-000016a0: 4023 252a 2302 c1b0 b1dd 444a 121b 1334  @#%*#.....DJ...4
-000016b0: 1442 b036 0163 2303 1425 b0b1 3602 6381  .B.6.c#..%..6.c.
-000016c0: 7891 0112 4381 2990 d360 2027 29b0 121b  x...C.)..` ')...
-000016d0: 1334 1844 121b 1334 1441 3600 5910 4563  .4.D...4.A6.Y.Ec
-000016e0: 867c d282 01a3 0146 8128 8113 90dd 8007  .|.....F.(......
-000016f0: 2725 2e48 2542 5b30 0001 0425 0014 2d36  '%.H%B[0...%..-6
-00001700: 00c2 b280 5527 0410 4714 2fb2 8151 2e02  ....U'..G./..Q..
-00001710: 5536 0127 0012 1b13 3451 de44 4512 3d34  U6.'....4Q.DE.=4
-00001720: 0059 4811 121b 1334 1448 b0b1 b420 0003  .YH....4.H... ..
-00001730: 3601 594a 1a57 1281 26df 4452 c349 0812  6.YJ.W..&.DR.I..
-00001740: 8127 b334 0163 5151 c328 035d 4a01 5d52  .'.4.cQQ.(.]J.]R
-00001750: 6301 8160 430e 8112 6464 6490 ec12 1b13  c..`C...ddd.....
-00001760: 3414 7e25 0225 0010 8113 2501 3682 0263  4.~%.%....%.6..c
-00001770: 8644 c282 01a2 0149 8128 8113 90f3 8007  .D.....I.(......
-00001780: 2c42 4825 425a 2730 0001 1281 2a25 0012  ,BH%BZ'0....*%..
-00001790: 8127 3402 4342 5063 121b 1334 51de 4445  .'4.CBPc...4Q.DE
-000017a0: 123d 3400 5948 1012 1b13 3414 48b0 b120  .=4.YH....4.H.. 
-000017b0: 0002 3601 594a 2157 1281 26df 4459 c249  ..6.YJ!W..&.DY.I
-000017c0: 0f12 812b b234 0159 1281 27b2 3401 6351  ...+.4.Y..'.4.cQ
-000017d0: 51c2 2802 5d4a 015d 5263 0181 5032 0c81  Q.(.]J.]Rc..P2..
-000017e0: 1264 64a0 0212 1b13 3414 8105 2500 1081  .dd.....4...%...
-000017f0: 1325 0136 8201 6350 000a 4aa0 0e60 4023  .%.6..cP..J..`@#
-00001800: 0463 8200 200e 4ba0 1760 6029 2c12 1b13  .c.. .K..``),...
-00001810: 2114 4b36 00c0 b014 4c12 0b10 1f34 0136  !.K6....L....4.6
-00001820: 0159 b063 5000 0a4d a023 6040 2305 63    .Y.cP..M.#`@#.c
+00000240: 6563 0012 6f6c 6564 5f74 7970 6500 1672  ec..oled_type..r
+00000250: 656e 6465 725f 7061 6765 000e 636f 6e74  ender_page..cont
+00000260: 726f 6c00 0c6d 7367 626f 7800 1073 686f  rol..msgbox..sho
+00000270: 775f 6d73 6700 1053 686f 7720 6d73 6700  w_msg..Show msg.
+00000280: 2069 6e74 6572 636f 6e5f 6765 6e70 6167   intercon_genpag
+00000290: 6500 0910 6164 645f 7061 6765 0016 636d  e...add_page..cm
+000002a0: 645f 6765 6e70 6167 6500 0a6c 6d64 6570  d_genpage..lmdep
+000002b0: 000c 7069 6e6d 6170 0082 3f08 6865 6c70  ..pinmap..?.help
+000002c0: 0023 8231 0e4c 4d5f 6f6c 6564 001c 4c4d  .#.1.LM_oled..LM
+000002d0: 5f6f 6c65 645f 7368 3131 3036 0024 7061  _oled_sh1106.$pa
+000002e0: 6765 5f63 616c 6c62 6163 6b5f 6c69 7374  ge_callback_list
+000002f0: 0016 6163 7469 7665 5f70 6167 6500 0a77  ..active_page..w
+00000300: 6964 7468 000c 6865 6967 6874 0014 6f6c  idth..height..ol
+00000310: 6564 5f73 7461 7465 0018 626c 696e 6b5f  ed_state..blink_
+00000320: 6566 6665 6374 001c 6f70 656e 5f69 6e74  effect..open_int
+00000330: 6572 636f 6e73 0006 6e2f 6100 0e63 6d64  ercons..n/a..cmd
+00000340: 5f6f 7574 0018 636d 645f 7461 736b 5f74  _out..cmd_task_t
+00000350: 6167 0026 6274 746e 5f70 7265 7373 5f63  ag.&bttn_press_c
+00000360: 616c 6c62 6163 6b00 0c69 7271 5f6f 6b00  allback..irq_ok.
+00000370: 265f 5f63 7265 6174 655f 6275 7474 6f6e  &__create_button
+00000380: 5f69 7271 0012 7469 6d69 7271 7365 7100  _irq..timirqseq.
+00000390: 1e70 7772 5f73 6176 6572 5f73 7461 7465  .pwr_saver_state
+000003a0: 001a 5f5f 7061 6765 5f68 6561 6465 7200  ..__page_header.
+000003b0: 8245 0c73 7461 7475 7300 0872 7373 6900  .E.status..rssi.
+000003c0: 0630 7b7d 0002 3000 0b02 2100 145f 5f70  .0{}..0...!..__p
+000003d0: 6167 655f 6261 7200 0872 6563 7400 105f  age_bar..rect.._
+000003e0: 5f6d 7367 626f 7800 0e70 6f77 6572 6f6e  _msgbox..poweron
+000003f0: 000a 7374 6174 6500 0449 4e00 1250 554c  ..state..IN..PUL
+00000400: 4c5f 444f 574e 0006 6972 7100 0e74 7269  L_DOWN..irq..tri
+00000410: 6767 6572 0014 4952 515f 5249 5349 4e47  gger..IRQ_RISING
+00000420: 000e 6861 6e64 6c65 7200 185f 5f70 6f77  ..handler..__pow
+00000430: 6572 5f73 6176 6500 066f 6666 0079 0a63  er_save..off.y.c
+00000440: 6c65 616e 0008 7368 6f77 000a 7072 6573  lean..show..pres
+00000450: 7300 245f 7061 6765 5f62 7574 746f 6e5f  s.$_page_button_
+00000460: 7072 6573 7300 0870 7265 7600 046f 6e00  press..prev..on.
+00000470: 1070 6f77 6572 6f66 6600 0653 3a31 0006  .poweroff..S:1..
+00000480: 533a 3000 125f 636d 645f 7465 7874 001a  S:0.._cmd_text..
+00000490: 696e 7465 7263 6f6e 5f70 6167 6500 0674  intercon_page..t
+000004a0: 6167 0082 0303 06c2 ba43 0002 4300 086b  ag.......C..C..k
+000004b0: 696c 6c00 1a63 6d64 5f63 616c 6c5f 7061  ill..cmd_call_pa
+000004c0: 6765 0014 3c6c 6973 7463 6f6d 703e 000e  ge..<listcomp>..
+000004d0: 5f62 7574 746f 6e00 1048 454c 4c4f 203a  _button..HELLO :
+000004e0: 4400 165f 5f76 6973 7561 6c69 7a65 0008  D..__visualize..
+000004f0: 6669 6c6c 0020 5f5f 7267 625f 6272 6967  fill. __rgb_brig
+00000500: 6874 6e65 7373 000e 6d6f 6475 6c65 7300  htness..modules.
+00000510: 0673 7973 000c 4c4d 5f72 6762 0081 5514  .sys..LM_rgb..U.
+00000520: 6272 6967 6874 6e65 7373 000c 736d 6f6f  brightness..smoo
+00000530: 7468 0010 3c6c 616d 6264 613e 0006 7275  th..<lambda>..ru
+00000540: 6e00 165f 5f64 7261 775f 7273 7369 0008  n..__draw_rssi..
+00000550: 6c69 6e65 0012 5f5f 7077 725f 6f66 6600  line..__pwr_off.
+00000560: 105f 5f65 6666 6563 7400 1073 656e 645f  .__effect..send_
+00000570: 636d 6400 0e76 6572 6469 6374 0082 010e  cmd..verdict....
+00000580: 5f62 7566 6665 7200 0c6d 7367 6f62 6a00  _buffer..msgobj.
+00000590: 1049 6e74 6572 436f 6e00 2f2d 3581 3d14  .InterCon./-5.=.
+000005a0: 6c69 6e65 5f6c 696d 6974 0082 3349 822f  line_limit..3I./
+000005b0: 0663 6d64 0006 6d73 6700 8143 8177 8213  .cmd..msg..C.w..
+000005c0: 1c70 6167 655f 6361 6c6c 6261 636b 7300  .page_callbacks.
+000005d0: 0277 0002 6800 820d 8157 8179 0c70 696e  .w..h....W.y.pin
+000005e0: 6b65 7900 1a70 6167 655f 6361 6c6c 6261  key..page_callba
+000005f0: 636b 0010 6361 6c6c 6261 636b 0002 7800  ck..callback..x.
+00000600: 0279 0008 686f 7374 0006 7069 6e00 050c  .y..host..pin...
+00000610: 2020 7b7d 2520 287b 7d6b 6229 0005 0e49    {}% ({}kb)...I
+00000620: 6e74 6572 436f 6e20 6361 6368 6500 0a05  nterCon cache...
+00000630: 0504 6e65 7874 0005 0470 7265 7600 0505  ..next...prev...
+00000640: 7072 6573 7300 0502 6f6e 0005 036f 6666  press...on...off
+00000650: 0005 1c49 6e76 616c 6964 2063 6f6d 6d61  ...Invalid comma
+00000660: 6e64 207b 7d21 2048 696e 743a 207b 7d00  nd {}! Hint: {}.
+00000670: 0a03 0504 6f6c 6564 0005 0869 6e74 6572  ....oled...inter
+00000680: 636f 6e00 0505 6765 6e49 4f00 0a06 0541  con...genIO....A
+00000690: 7061 6765 7569 2070 6167 653d 3020 7077  pageui page=0 pw
+000006a0: 725f 7365 633d 4e6f 6e65 2f69 6e74 2873  r_sec=None/int(s
+000006b0: 6563 2920 6f6c 6564 5f74 7970 653d 2273  ec) oled_type="s
+000006c0: 7364 3133 3036 206f 7220 7368 3131 3036  sd1306 or sh1106
+000006d0: 2200 051e 636f 6e74 726f 6c20 6e65 7874  "...control next
+000006e0: 2f70 7265 762f 7072 6573 732f 6f6e 2f6f  /prev/press/on/o
+000006f0: 6666 0005 0c6d 7367 626f 7820 226d 7367  ff...msgbox "msg
+00000700: 2200 0527 696e 7465 7263 6f6e 5f67 656e  "..'intercon_gen
+00000710: 7061 6765 2022 686f 7374 2220 2263 6d64  page "host" "cmd
+00000720: 2220 7275 6e3d 4661 6c73 6500 051b 636d  " run=False...cm
+00000730: 645f 6765 6e70 6167 6520 2263 6d64 2220  d_genpage "cmd" 
+00000740: 7275 6e3d 4661 6c73 6500 0506 7069 6e6d  run=False...pinm
+00000750: 6170 000a 0205 0773 7364 3133 3036 0005  ap.....ssd1306..
+00000760: 0673 6831 3130 3600 051d 4f6c 6564 2055  .sh1106...Oled U
+00000770: 4920 756e 6b6e 6f77 6e20 6f6c 6564 5f74  I unknown oled_t
+00000780: 7970 653a 207b 7d00 050e 7b7d 207b 7d20  ype: {}...{} {} 
+00000790: 7b7d 3a7b 7d3a 7b7d 0005 165b 4552 525d  {}:{}:{}...[ERR]
+000007a0: 2042 7574 746f 6e20 4952 513a 7b7d 207b   Button IRQ:{} {
+000007b0: 7d00 0510 7061 6765 3a20 7b7d 2070 7772  }...page: {} pwr
+000007c0: 3a20 7b7d 000a 0207 0238 3407 0234 350a  : {}.....84..45.
+000007d0: 0207 0135 0702 3132 0804 302e 3031 050c  ...5..12..0.01..
+000007e0: 5461 736b 2069 7320 4275 7379 0094 041c  Task is Busy....
+000007f0: 5601 2c32 3232 2c2c 2c32 224f 2622 4a27  V.,222,,,2"O&"J'
+00000800: 224f 8607 994c 840d 8813 840f 842a 8b0e  "O...L.......*..
+00000810: 890c 890a 8916 891b 8409 840c 8010 022a  ...............*
+00000820: 011b 031c 0216 0259 8010 0410 052a 021b  .......Y.....*..
+00000830: 061c 0416 041c 0516 0559 8010 0710 082a  .........Y.....*
+00000840: 021b 091c 0716 071c 0816 0859 8010 0a10  ...........Y....
+00000850: 0b2a 021b 0c1c 0a16 0a1c 0b16 0b59 8010  .*...........Y..
+00000860: 0d2a 011b 0e1c 0d16 0d59 8010 0f2a 011b  .*.......Y...*..
+00000870: 101c 0f16 0f59 8010 112a 011b 121c 1116  .....Y...*......
+00000880: 1159 8010 1310 142a 021b 151c 1316 131c  .Y.....*........
+00000890: 1416 1459 480e 8010 162a 011b 171c 1616  ...YH....*......
+000008a0: 1659 4a07 5951 1616 4a01 5d48 0980 511b  .YJ.YQ..J.]H..Q.
+000008b0: 1816 8120 4a08 5951 1681 204a 015d 480e  ... J.YQ.. J.]H.
+000008c0: 8010 192a 011b 1a1c 1916 1959 4a07 5951  ...*.......YJ.YQ
+000008d0: 1619 4a01 5d54 3200 101b 3402 161b 3201  ..J.]T2...4...2.
+000008e0: 1620 832a 0153 3302 162a 3203 1632 3204  . .*.S3..*2..22.
+000008f0: 1636 5110 1c80 2a03 5333 0516 3d10 1d2a  .6Q...*.S3..=..*
+00000900: 0153 3306 1642 101e 2a01 5333 0716 4351  .S3..B..*.S3..CQ
+00000910: 502a 0253 3308 1646 5150 2a02 5333 0916  P*.S3..FQP*.S3..
+00000920: 4932 0a16 4a32 0b16 4b32 0c16 4d51 630d  I2..J2..K2..MQc.
+00000930: 881c 103e 1b8b 1b23 438b 2f84 2284 0a84  ...>...#C./."...
+00000940: 1b89 0e84 1164 6084 0f84 2284 0d84 1385  .....d`...".....
+00000950: 1289 2911 8121 1681 2210 1b16 8123 5116  ..)..!.."....#Q.
+00000960: 3451 1621 8051 101c 2a03 5333 0016 4e32  4Q.!.Q..*.S3..N2
+00000970: 0116 6132 0216 6932 0316 6b10 1f2a 0153  ..a2..i2..k..*.S
+00000980: 3304 165e 3205 1674 3206 1648 3207 1641  3..^2..t2..H2..A
+00000990: 3208 1642 3209 167a 320a 1635 320b 1681  2..B2..z2..52...
+000009a0: 0050 2a01 5333 0c16 8101 502a 0153 330d  .P*.S3....P*.S3.
+000009b0: 1681 0851 630e 8b78 db85 014a 4e81 2d81  ...Qc..x...JN.-.
+000009c0: 2e81 2f81 303e 3f40 801f 8008 2a2a 4725  ../.0>?@....**G%
+000009d0: 472c 2d24 2424 2464 2464 2525 6424 2466  G,-$$$$d$d%%d$$f
+000009e0: 77b6 144f 3600 2306 dd44 5db6 144f 3600  w..O6.#..D]..O6.
+000009f0: 101c d944 4780 511b 50c7 4245 8051 1b51  ...DG.Q.P.BE.Q.Q
+00000a00: c7b7 121b 1821 4259 120f 2307 1425 b636  .....!BY..#..%.6
+00000a10: 0134 0159 1281 2723 0714 25b6 3601 3401  .4.Y..'#..%.6.4.
+00000a20: 59b1 b018 52b4 b018 53b2 b018 54b3 b018  Y...R...S...T...
+00000a30: 5552 b018 5651 b018 4450 b018 572b 00b0  UR..VQ..DP..W+..
+00000a40: 1858 1059 b018 5a51 b018 5b51 b018 5c50  .X.Y..ZQ..[Q..\P
+00000a50: b018 5db0 145e 3600 59b5 1281 3112 0210  ..]..^6.Y...1...
+00000a60: 5f34 0122 8768 f782 3402 b52b 03b0 1860  _4.".h..4..+...`
+00000a70: b012 1b18 3451 638f 248d 1031 6181 2d80  ....4Qc.$..1a.-.
+00000a80: 4e40 8507 8509 2233 4743 251f 211f 211f  N@...."3GC%.!.!.
+00000a90: 2127 3239 00b0 2000 01c1 b020 0101 c248  !'29.. .... ...H
+00000aa0: 19b1 1062 1207 1208 3401 1463 1064 3601  ...b....4..c.d6.
+00000ab0: 3482 0059 b234 0059 4a04 594a 015d 1204  4..Y.4.YJ.YJ.]..
+00000ac0: 3400 c312 8132 1281 28b3 7b55 3401 3401  4....2..(.{U4.4.
+00000ad0: 82d7 444b 1065 1425 b37b 5536 0142 43b3  ..DK.e.%.{U6.BC.
+00000ae0: 7b55 c412 8132 1281 28b3 7c55 3401 3401  {U...2..(.|U4.4.
+00000af0: 82d7 444b 1065 1425 b37c 5536 0142 43b3  ..DK.e.%.|U6.BC.
+00000b00: 7c55 c512 8132 1281 28b3 7d55 3401 3401  |U...2..(.}U4.4.
+00000b10: 82d7 444b 1065 1425 b37d 5536 0142 43b3  ..DK.e.%.}U6.BC.
+00000b20: 7d55 c612 0d34 0080 55c7 1281 32b7 3401  }U...4..U...2.4.
+00000b30: 80d8 4445 b780 5542 4210 66c7 2500 135c  ..DE..UBB.f.%..\
+00000b40: 51de 4444 1047 424c 2500 135d 4444 1067  Q.DD.GBL%..]DD.g
+00000b50: 4242 1068 c812 1b13 2114 2223 0814 25b7  BB.h....!."#..%.
+00000b60: b8b4 b5b6 3605 8080 3603 5951 6302 8720  ....6...6.YQc.. 
+00000b70: 6214 8117 6762 8051 2f38 3626 1281 31b1  b...gb.Q/86&..1.
+00000b80: 2280 5bf2 9ef7 88f4 3401 c212 1b13 2114  ".[.....4.....!.
+00000b90: 8118 2500 1354 8af3 8825 0013 5488 f388  ..%..T...%..T...
+00000ba0: 3604 5912 1b13 2114 8118 2500 1354 91f3  6.Y...!...%..T..
+00000bb0: 8125 0013 5481 3604 59b2 8042 5e57 c312  .%..T.6.Y..B^W..
+00000bc0: 1b13 2114 8118 2280 76b3 f388 b3f3 2280  ..!...".v.....".
+00000bd0: 78b3 f288 b3f3 3604 5981 e558 5ad7 431d  x.....6.Y..XZ.C.
+00000be0: 5959 5163 8550 7916 8119 6780 5822 2925  YYQc.Py...g.X")%
+00000bf0: 222c 269d c125 0013 6030 03c2 c3c4 b251  ",&..%..`0.....Q
+00000c00: de44 4251 6312 8131 b4b2 f781 3402 88f4  .DBQc..1....4...
+00000c10: c5b5 8042 6257 c612 1b13 2114 8118 2500  ...BbW....!...%.
+00000c20: 1354 b1f3 86b6 f325 0013 54b1 f382 f386  .T.....%..T.....
+00000c30: b6f3 3604 5981 e558 5ad7 4319 5959 5163  ..6.Y..XZ.C.YYQc
+00000c40: 8618 6914 6981 2d80 7020 2950 2e55 1281  ..i.i.-.p )P.U..
+00000c50: 32b0 1352 3401 c112 8124 1281 31b0 1354  2..R4....$..1..T
+00000c60: b1f7 3401 3401 c212 8133 80b0 1354 b234  ..4.4....3...T.4
+00000c70: 035f 4b16 c312 1b13 2114 6ab3 b013 5585  ._K.....!.j...U.
+00000c80: f3b2 81f3 8436 0459 4228 121b 1321 146a  .....6.YB(...!.j
+00000c90: b013 53b2 f481 f2b0 1355 84f3 b282 f382  ..S......U......
+00000ca0: 3604 5951 6389 3c59 296b 812d 807a 6540  6.YQc.<Y)k.-.ze@
+00000cb0: 2545 2246 2945 5324 4a31 2754 2c00 b020  %E"F)ES$J1'T,.. 
+00000cc0: 0001 c125 0013 44c2 b251 de44 4250 6325  ...%..D..Q.DBPc%
+00000cd0: 0013 5643 4e12 1b13 2114 6c36 0059 5225  ..VCN...!.l6.YR%
+00000ce0: 0018 5612 1b13 2114 6a8a 8f22 806c a810  ..V...!.j..".l..
+00000cf0: 6d81 3682 0459 b134 0059 1281 32b2 3401  m.6..Y.4.Y..2.4.
+00000d00: 8ad8 446c 121b 1321 1422 b280 8a2e 0255  ..Dl...!.".....U
+00000d10: 8f99 3603 59b2 8a51 2e02 55c3 1281 32b3  ..6.Y..Q..U...2.
+00000d20: 3401 8cd8 4448 b351 8b2e 0255 4241 b3c2  4...DH.Q...UBA..
+00000d30: 121b 1321 1422 b28f a836 0359 5263 0184  ...!."...6.YRc..
+00000d40: 4051 0e81 1a67 807b 293a 2500 1357 d325  @Q...g.{):%..W.%
+00000d50: 0018 5712 1b13 2114 6a22 806a 9189 8510  ..W...!.j".j....
+00000d60: 6d81 1081 0d25 0013 5736 8404 5912 1b13  m....%..W6..Y...
+00000d70: 2114 6a22 806a 9889 8910 6d81 1081 0d25  !.j".j....m....%
+00000d80: 0013 5736 8404 5951 6386 6ce2 0321 5e81  ..W6..YQc.l..!^.
+00000d90: 2d81 3480 9520 2252 2922 2f23 4e33 0048  -.4.. "R)"/#N3.H
+00000da0: 0812 0ab1 3401 c24a 2457 1281 27df 445c  ....4..J$W..'.D\
+00000db0: c349 1223 0914 25b1 b336 02c4 51c2 120f  .I.#..%..6..Q...
+00000dc0: b434 0159 5151 c328 035d 4a01 5db2 4466  .4.YQQ.(.]J.].Df
+00000dd0: 1211 b212 1113 6e12 1113 6f34 03c5 b514  ......n...o4....
+00000de0: 7010 7112 1113 7210 73b0 2000 0136 8400  p.q...r.s. ..6..
+00000df0: 5952 2500 185d 5163 0181 1022 0e81 1567  YR%..]Qc..."...g
+00000e00: 813a 809f 2500 1442 1079 3601 6383 6031  .:..%..B.y6.c.`1
+00000e10: 1874 812d 80a3 6028 4522 254a 28b0 1360  .t.-..`(E"%J(..`
+00000e20: 3003 c1c2 c3b1 51de 4442 5163 b380 d844  0.....Q.DBQc...D
+00000e30: 4ab3 b2f3 b013 6082 5642 4eb0 1442 1075  J.....`.VBN..B.u
+00000e40: 3601 59b1 b013 6082 5651 6382 0022 1448  6.Y...`.VQc..".H
+00000e50: 812d 8135 80b4 2722 29b1 b013 52dd 4442  .-.5..'")...R.DB
+00000e60: 5263 b013 5214 76b1 3601 5952 6386 5821  Rc..R.v.6.YRc.X!
+00000e70: 2041 812d 80ba 2029 2626 2626 2330 4a2a   A.-.. )&&&&#0J*
+00000e80: 2912 1b13 2114 7736 0059 b014 6b36 00c1  )...!.w6.Y..k6..
+00000e90: b013 5644 c280 b014 6136 0059 b014 6936  ..VD....a6.Y..i6
+00000ea0: 0059 b143 64b0 1353 1281 32b0 1352 3401  .Y.Cd..S..2..R4.
+00000eb0: 81f3 d844 4ab0 1352 8055 3400 5942 4ab0  ...DJ..R.U4.YBJ.
+00000ec0: 1352 b013 5355 3400 5912 1b13 2114 7836  .R..SU4.Y...!.x6
+00000ed0: 0059 b014 7436 0059 5163 8f50 2a46 4281  .Y..t6.YQc.P*FB.
+00000ee0: 2d81 2980 ca4a 442a 2029 2a20 2930 2426  -.)..JD* )* )0$&
+00000ef0: 2428 2a20 2927 2d26 2427 2a29 262a 2924  $(* )'-&$'*)&*)$
+00000f00: 26b0 1360 8055 b013 6082 5651 b018 44b1  &..`.U..`.VQ..D.
+00000f10: 144f 3600 1079 d944 49b0 147a 3600 5942  .O6..y.DI..z6.YB
+00000f20: a781 b114 4f36 0010 1dd9 446f b057 1353  ....O6....Do.W.S
+00000f30: 81e5 5a18 53b0 1353 1281 32b0 1352 3401  ..Z.S..S..2..R4.
+00000f40: 81f3 d844 4480 b018 53b0 1441 3600 5951  ...DD...S..A6.YQ
+00000f50: b018 5c10 59b0 185a 42ee 80b1 144f 3600  ..\.Y..ZB....O6.
+00000f60: 107b d944 6eb0 5713 5381 e65a 1853 b013  .{.Dn.W.S..Z.S..
+00000f70: 5380 d744 4d12 8132 b013 5234 0181 f3b0  S..DM..2..R4....
+00000f80: 1853 b014 4136 0059 51b0 185c 1059 b018  .S..A6.YQ..\.Y..
+00000f90: 5a42 76b1 144f 3600 107c d944 4f12 1b13  ZBv..O6..|.DO...
+00000fa0: 2114 6c36 0059 52b0 1856 425d b114 4f36  !.l6.YR..VB]..O6
+00000fb0: 0010 75d9 4453 121b 1321 147d 3600 5950  ..u.DS...!.}6.YP
+00000fc0: b018 5651 b018 5c42 4023 0a14 25b0 1353  ..VQ..\B@#..%..S
+00000fd0: b013 5636 0263 8208 1114 7a81 2d80 eb60  ..V6.c....z.-..`
+00000fe0: 4027 4246 b013 5c51 de44 4251 63b0 145c  @'BF..\Q.DBQc..\
+00000ff0: 3600 5951 b018 5c51 6387 2052 2235 812d  6.YQ..\Qc. R"5.-
+00001000: 8136 80f8 2064 2631 6d28 2628 6627 b1b0  .6.. d&1m(&(f'..
+00001010: 185c 230b 3002 c2c3 121b 1321 146a b283  .\#.0......!.j..
+00001020: f3b3 83f3 ae8e 3604 5912 1b13 2114 2210  ......6.Y...!.".
+00001030: 79b2 b336 0359 107e b013 5add 4446 52b0  y..6.Y.~..Z.DFR.
+00001040: 1857 4255 107f b013 5add 4446 50b0 1857  .WBU....Z.DFP..W
+00001050: 4247 b013 57d3 b018 5712 1b13 2114 6ab2  BG..W...W...!.j.
+00001060: 82f3 b382 f3ac 8cb0 1357 3605 5951 638a  .........W6.YQc.
+00001070: 084b 2481 0081 2d81 3781 3890 0b60 2034  .K$...-.7.8..` 4
+00001080: 2d35 335b 5712 8124 1281 31b0 1354 b1f3  -53[W..$..1..T..
+00001090: 88f7 3401 3401 81f3 c312 8132 b013 5a34  ..4.4......2..Z4
+000010a0: 01b3 d844 da80 121b 1321 1422 b013 5a80  ...D.....!."..Z.
+000010b0: b32e 0255 b1b2 8af2 3603 5912 8132 b013  ...U....6.Y..2..
+000010c0: 5ab3 512e 0255 3401 b385 f3d8 445b 121b  Z.Q..U4.....D[..
+000010d0: 1321 1422 b013 5ab3 82b3 f485 f32e 0255  .!."..Z........U
+000010e0: b1b2 94f2 3603 5942 5512 1b13 2114 22b0  ....6.YBU...!.".
+000010f0: 135a b351 2e02 55b1 b294 f236 0359 4250  .Z.Q..U....6.YBP
+00001100: 121b 1321 1422 b013 5ab1 b28a f236 0359  ...!."..Z....6.Y
+00001110: 5163 8d5c e805 bc80 0181 0181 2d81 3981  Qc.\........-.9.
+00001120: 2981 1690 1d20 4688 0e29 422d 4f2a 1f21  ).... F..)B-O*.!
+00001130: 5050 5245 4c48 2400 0102 0323 0c30 02c4  PPRELH$....#.0..
+00001140: c5b0 b1b2 b320 0004 c625 0125 0013 58dd  ..... ...%.%..X.
+00001150: 4442 5163 121b 1321 1422 2501 80b5 3603  DBQc...!."%...6.
+00001160: 5912 1b13 2114 2225 02b4 b58a f236 0359  Y...!."%.....6.Y
+00001170: 2500 135b 51de d344 d780 1281 2812 1434  %..[Q..D....(..4
+00001180: 0014 7810 8102 2500 135b 3682 0034 0114  ..x...%..[6..4..
+00001190: 8103 1047 1081 0436 02c7 b751 ded3 4471  ...G...6...Q..Dq
+000011a0: 1281 32b7 3401 80d8 4467 b714 8103 1081  ..2.4...Dg......
+000011b0: 0510 8106 3602 2500 185a 1214 3400 1481  ....6.%..Z..4...
+000011c0: 0710 8102 2500 135b 3682 0059 5125 0018  ....%..[6..YQ%..
+000011d0: 5b25 0014 8100 b4b5 8af2 3602 5925 0014  [%........6.Y%..
+000011e0: 35b6 3601 5925 0344 44b6 3400 5951 6301  5.6.Y%.DD.4.YQc.
+000011f0: 8748 d806 1e81 0a67 6767 6790 222b 422d  .H.....gggg."+B-
+00001200: 292e 5533 2500 1358 1476 2501 3601 5948  ).U3%..X.v%.6.YH
+00001210: 2f12 8120 1481 1b25 0125 0236 02c4 b410  /.. ...%.%.6....
+00001220: 8102 5525 0018 5b23 0eb4 1081 1c55 dd44  ..U%..[#.....U.D
+00001230: 4d25 0343 49b4 1081 1c55 2500 185a 4a1d  M%.CI....U%..ZJ.
+00001240: 5712 8127 df44 55c5 490b 1281 28b5 3401  W..'.DU.I...(.4.
+00001250: 2500 185a 5151 c528 055d 4a01 5d25 0013  %..ZQQ.(.]J.]%..
+00001260: 5814 811d 2501 3601 5951 6385 34db 01a9  X...%.6.YQc.4...
+00001270: 0181 0881 2d81 2981 1690 4620 4666 6087  ....-.)...F Ff`.
+00001280: 0a2d 4a48 2300 0106 230c 3002 c3c4 b020  .-JH#...#.0.... 
+00001290: 0001 2706 b0b1 b620 0103 c512 1b13 2114  ..'.... ......!.
+000012a0: 2225 0180 b436 0359 2500 1481 00b3 b436  "%...6.Y%......6
+000012b0: 0259 2500 1435 b536 0159 b244 44b5 3400  .Y%..5.6.Y.DD.4.
+000012c0: 5951 6302 8478 3e14 811e 6781 2a90 4a22  YQc..x>...g.*.J"
+000012d0: 1f54 482b 1081 0414 2fb1 144f 3600 142d  .TH+..../..O6..-
+000012e0: 3600 3601 1481 0310 4710 8104 3602 1481  6.6.....G...6...
+000012f0: 0310 8105 1081 0636 0225 0018 5a4a 1457  .......6.%..ZJ.W
+00001300: 1281 27df 444c 59b1 144f 3600 2500 185a  ..'.DLY..O6.%..Z
+00001310: 4a01 5d51 6384 40d3 0216 810a 6767 6790  J.]Qc.@.....ggg.
+00001320: 5020 224b 5848 1925 0114 4f36 0014 2d36  P "KXH.%..O6..-6
+00001330: 00c3 1213 b310 811f 2502 3482 0159 4a1d  ........%.4..YJ.
+00001340: 5712 8127 df44 55c4 490b 1281 28b4 3401  W..'.DU.I...(.4.
+00001350: 2500 185a 5151 c428 045d 4a01 5d51 6387  %..ZQQ.(.]J.]Qc.
+00001360: 7040 1620 9067 6031 3927 251f 2337 121b  p@. .g`19'%.#7..
+00001370: 1321 1422 1202 1023 3401 808f 3603 5912  .!."...#4...6.Y.
+00001380: 1b13 2114 2210 2414 2512 0d34 0081 5580  ..!.".$.%..4..U.
+00001390: 5536 0180 9936 0359 1216 51de d344 6712  U6...6.Y..Q..Dg.
+000013a0: 1634 00c0 121b 1321 1422 2300 1425 b010  .4.....!."#..%..
+000013b0: 2655 1281 24b0 1027 5522 8768 f734 0136  &U..$..'U".h.4.6
+000013c0: 0280 a336 0359 121b 1321 1422 1028 1425  ...6.Y...!.".(.%
+000013d0: 1202 1029 3401 3601 80ad 3603 5952 638b  ...)4.6...6.YRc.
+000013e0: 0cf9 0128 2a81 2590 7427 2222 222d 3532  ...(*.%.t'"""-52
+000013f0: 2a33 3724 2529 222f 1281 2051 de44 4250  *37$%)"/.. Q.DBP
+00001400: 638f c181 c212 1b13 2114 2223 0180 b136  c.......!."#...6
+00001410: 0359 1281 2632 0012 8120 142b 3600 3401  .Y..&2... .+6.4.
+00001420: 3401 80d8 44da 8012 8120 142b 3600 142c  4...D.... .+6..,
+00001430: 3600 5f4b 4a30 02c3 c4b3 142d 102e 3601  6._KJ0.....-..6.
+00001440: 8055 c310 2e14 2fb4 142d 102e 3601 7e51  .U..../..-..6.~Q
+00001450: 2e02 5536 01c4 121b 1321 1422 1030 1425  ..U6.....!.".0.%
+00001460: b4b3 3602 80b1 b28a f4f2 3603 59b2 81e5  ..6.......6.Y...
+00001470: c2b2 b0d8 4446 5959 5959 4243 42b4 7f52  ....DFYYYYBCB..R
+00001480: 6312 1b13 2114 2210 31a8 b194 f236 0359  c...!.".1....6.Y
+00001490: 5263 0181 2039 0a81 0967 9079 2b00 b05f  Rc.. 9...g.y+.._
+000014a0: 4b06 c181 2f14 4238 6384 3cb8 0214 3290  K.../.B8c.<...2.
+000014b0: 8720 6340 222d 5630 3200 c048 1912 1b13  . c@"-V02..H....
+000014c0: 2114 2210 339e 8f36 0359 121b 1334 1435  !.".3..6.Y...4.5
+000014d0: b036 0159 4a1a 5712 8127 df44 52c1 4908  .6.YJ.W..'.DR.I.
+000014e0: 1281 28b1 3401 6351 51c1 2801 5d4a 015d  ..(.4.cQQ.(.]J.]
+000014f0: 5263 0182 0820 0c81 0a90 8920 2e12 1b13  Rc... ..... ....
+00001500: 2114 2210 810b a39d 3603 5912 1b13 2114  !.".....6.Y...!.
+00001510: 7836 0059 5163 874c 401e 3690 9660 830f  x6.YQc.L@.6..`..
+00001520: 8308 2d27 2b2b 3737 2832 00c0 3201 c12c  ..-'++77(2..2..,
+00001530: 0210 3710 2662 1037 1038 62c2 1219 51de  ..7.&b.7.8b...Q.
+00001540: d344 4b12 1912 0a10 3934 0134 01c2 b010  .DK.....94.4....
+00001550: 3ab2 1026 5534 8200 5912 1b13 2114 2210  :..&U4..Y...!.".
+00001560: 3b14 25b2 1026 5536 0122 8041 9436 0359  ;.%..&U6.".A.6.Y
+00001570: 121b 1321 1422 103c 1425 b210 3855 3601  ...!.".<.%..8U6.
+00001580: 2280 41a8 3603 59b1 b210 2655 3401 5952  ".A.6.Y...&U4.YR
+00001590: 6302 8810 8910 1c81 0c3a 909a 2325 294a  c........:..#%)J
+000015a0: 5229 2e25 5322 32c1 b023 0df4 c212 8131  R).%S"2..#.....1
+000015b0: b2b1 f434 01c3 b381 d744 4381 4241 b3c3  ...4.....DC.BA..
+000015c0: 121b 1321 146a 8089 b3b3 1081 0d52 3682  ...!.j.......R6.
+000015d0: 0459 1281 24b1 8af7 3401 c412 8133 b4b1  .Y..$...4....3..
+000015e0: 81f2 b434 035f 4b2c c5b5 b3d7 4453 121b  ...4._K,....DS..
+000015f0: 1321 146a 8089 b5b5 106d 8036 8204 5942  .!.j.....m.6..YB
+00001600: 5112 1b13 2114 6a80 89b5 b510 6d81 3682  Q...!.j.....m.6.
+00001610: 0459 4212 5163 8438 3114 810e 2690 a92e  .YB.Qc.81...&...
+00001620: 2c2e 2522 8010 810f 2a01 1b81 101c 810f  ,.%"....*.......
+00001630: c159 1081 11b1 1481 1236 00dd 445f 8010  .Y.......6..D_..
+00001640: 8113 2a01 1b81 111c 8113 c259 b051 de44  ..*........Y.Q.D
+00001650: 4251 63b2 b010 8114 5234 8201 5951 6384  BQc.....R4..YQc.
+00001660: 18eb 8101 163d 3f40 3e90 c080 0728 2b36  .....=?@>....(+6
+00001670: 121b 1334 51de 4461 1220 122a 1236 1232  ...4Q.Da. .*.6.2
+00001680: 2b04 c312 1bb3 2281 0022 8040 103e b210  +....."..".@.>..
+00001690: 3fb0 1040 b134 8603 5912 1b13 3414 4136  ?..@.4..Y...4.A6
+000016a0: 0059 5163 8240 a901 1442 8129 90ce 6040  .YQc.@...B.)..`@
+000016b0: 2325 2a23 02c1 b0b1 dd44 4a12 1b13 3414  #%*#.....DJ...4.
+000016c0: 42b0 3601 6323 0314 25b0 b136 0263 8178  B.6.c#..%..6.c.x
+000016d0: 9101 1243 812a 90da 6020 2729 b012 1b13  ...C.*..` ')....
+000016e0: 3418 4412 1b13 3414 4136 0059 1045 6386  4.D...4.A6.Y.Ec.
+000016f0: 7cd2 8201 a301 4681 2981 1690 e480 0727  |.....F.)......'
+00001700: 252e 4825 425b 3000 0104 2500 142d 3600  %.H%B[0...%..-6.
+00001710: c2b2 8055 2704 1047 142f b281 512e 0255  ...U'..G./..Q..U
+00001720: 3601 2700 121b 1334 51de 4445 123d 3400  6.'....4Q.DE.=4.
+00001730: 5948 1112 1b13 3414 48b0 b1b4 2000 0336  YH....4.H... ..6
+00001740: 0159 4a1a 5712 8127 df44 52c3 4908 1281  .YJ.W..'.DR.I...
+00001750: 28b3 3401 6351 51c3 2803 5d4a 015d 5263  (.4.cQQ.(.]J.]Rc
+00001760: 0181 6843 0e81 1567 6767 90f3 121b 1334  ..hC...ggg.....4
+00001770: 1481 0125 0225 0010 8116 2501 3682 0263  ...%.%....%.6..c
+00001780: 8644 c282 01a2 0149 8129 8116 90fa 8007  .D.....I.)......
+00001790: 2c42 4825 425a 2730 0001 1281 2b25 0012  ,BH%BZ'0....+%..
+000017a0: 8128 3402 4342 5063 121b 1334 51de 4445  .(4.CBPc...4Q.DE
+000017b0: 123d 3400 5948 1012 1b13 3414 48b0 b120  .=4.YH....4.H.. 
+000017c0: 0002 3601 594a 2157 1281 27df 4459 c249  ..6.YJ!W..'.DY.I
+000017d0: 0f12 812c b234 0159 1281 28b2 3401 6351  ...,.4.Y..(.4.cQ
+000017e0: 51c2 2802 5d4a 015d 5263 0181 5032 0c81  Q.(.]J.]Rc..P2..
+000017f0: 1567 67a0 0912 1b13 3414 8108 2500 1081  .gg.....4...%...
+00001800: 1625 0136 8201 6350 000a 4aa0 1560 4023  .%.6..cP..J..`@#
+00001810: 0463 8200 200e 4ba0 1e60 6029 2c12 1b13  .c.. .K..``),...
+00001820: 2114 4b36 00c0 b014 4c12 0b10 1f34 0136  !.K6....L....4.6
+00001830: 0159 b063 5000 0a4d a02a 6040 2305 63    .Y.cP..M.*`@#.c
```

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_rgbcct.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_rgbcct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files 4% similar despite different names*

```diff
@@ -120,239 +120,239 @@
 00000770: 7374 6f70 7065 643a 207b 7d00 0541 496e  stopped: {}..AIn
 00000780: 7661 6c69 6420 7461 736b 2063 6d64 2120  valid task cmd! 
 00000790: 4865 6c70 3a20 7461 736b 206c 6973 7420  Help: task list 
 000007a0: 2f20 6b69 6c6c 203c 7461 736b 4944 3e20  / kill <taskID> 
 000007b0: 2f20 7368 6f77 203c 7461 736b 4944 3e00  / show <taskID>.
 000007c0: 0513 5b45 5252 5d20 5461 736b 206b 696c  ..[ERR] Task kil
 000007d0: 6c3a 207b 7d00 8c54 2436 0180 0e26 2c2c  l: {}..T$6...&,,
-000007e0: 2c32 2c52 224f 278f 0789 9089 b584 1484  ,2,R"O'.........
+000007e0: 2c32 2c52 224f 278f 0789 8f89 b584 1484  ,2,R"O'.........
 000007f0: 0d88 4084 5180 511b 0216 7f80 1003 2a01  ..@.Q.Q.......*.
 00000800: 1b04 1c03 1603 5980 1005 2a01 1b06 1c05  ......Y...*.....
 00000810: 1605 5980 1007 2a01 1b08 1c07 1607 5980  ..Y...*.......Y.
 00000820: 1009 100a 2a02 1b0b 1c09 1609 1c0a 160a  ....*...........
 00000830: 5980 100c 2a01 1b0d 1c0c 160c 5980 100e  Y...*.......Y...
 00000840: 100f 2a02 1b10 1c0e 160e 1c0f 160f 5948  ..*...........YH
 00000850: 0e80 1011 2a01 1b12 1c11 1611 594a 1759  ....*.......YJ.Y
 00000860: 1109 2300 3401 5980 1011 2a01 1b13 1c11  ..#.4.Y...*.....
 00000870: 1611 594a 015d 5432 0010 1434 0216 1454  ..YJ.]T2...4...T
 00000880: 3201 1015 3402 1615 3202 1617 3203 161d  2...4...2...2...
 00000890: 512a 0153 3304 161e 3205 161f 3206 1627  Q*.S3...2...2..'
 000008a0: 5163 0786 2c10 2c14 8b22 4484 0989 0d88  Qc..,.,.."D.....
-000008b0: 0b84 0984 0989 128a 1984 1484 0f11 8100  ................
+000008b0: 0a84 0984 0989 128a 1984 1484 0f11 8100  ................
 000008c0: 1681 0110 1416 8102 2c00 1633 3200 1628  ........,..32..(
 000008d0: 1181 0332 0134 0116 3250 2a01 5333 0216  ...2.4..2P*.S3..
 000008e0: 3632 0316 3832 0416 3a51 512a 0253 3305  62..82..:QQ*.S3.
 000008f0: 163b 5151 512a 0353 3306 163f 3207 1642  .;QQQ*.S3..?2..B
 00000900: 3208 1641 3209 1645 5163 0a83 0811 1628  2..A2..EQc.....(
 00000910: 810b 8025 2424 2424 2925 51b0 1829 51b0  ...%$$$$)%Q..)Q.
 00000920: 182a 50b0 182b 94b0 182c 127f 142d 3600  .*P..+...,...-6.
 00000930: b018 2e10 2fb0 1830 51b0 1831 5163 8248  ..../..0Q..1Qc.H
 00000940: 2912 3231 802f 6020 2b4f 4212 1413 3314  ).21./` +OB...3.
 00000950: 34b0 5136 02c1 b151 ded3 444b b113 2e14  4.Q6...Q..DK....
-00000960: 3536 0043 4252 6350 6383 70a2 0118 3681  56.CBRcPc.p...6.
-00000970: 0b46 803b 6028 2e23 2a25 b013 2e14 3736  .F.;`(.#*%....76
-00000980: 0059 b013 3112 1413 3314 2636 00dd 4452  .Y..1...3.&6..DR
-00000990: b144 4a12 1413 33b0 1331 535b 56b0 535a  .DJ...3..1S[V.SZ
-000009a0: 1829 1211 3400 5951 6381 2011 1038 810b  .)..4.YQc. ..8..
-000009b0: 8046 6040 28b0 132e 1439 3600 59b0 6382  .F`@(....96.Y.c.
-000009c0: 00a8 041c 3a81 0b81 0c81 0d81 0e80 4f60  ....:.........O`
-000009d0: 4028 b013 2e14 3736 0059 1211 3400 5951  @(....76.Y..4.YQ
-000009e0: 6385 00b3 8001 1c3b 810b 4b31 8058 6060  c......;..K1.X``
-000009f0: 3a4b 624e 27b2 51de 4451 103c 141c 1281  :KbN'.Q.DQ.<....
-00000a00: 0712 1413 3334 0136 0142 41b2 b018 3112  ....34.6.BA...1.
-00000a10: 1414 32b0 1331 3601 4442 5063 127f 143d  ..2..16.DBPc...=
-00000a20: 3600 143e b136 01b0 1829 b012 1413 33b2  6..>.6...)....3.
-00000a30: 5652 6387 48c0 8501 243f 810b 4b53 5480  VRc.H...$?..KST.
-00000a40: 6a80 082f 4b62 244e 5852 2910 4014 23b1  j../Kb$NXR).@.#.
-00000a50: 8082 2e02 5536 01b0 1831 1214 1432 b013  ....U6...1...2..
-00000a60: 3136 0144 4250 63b1 b018 2ab2 51de 4445  16.DBPc...*.Q.DE
-00000a70: b013 2b42 41b2 b018 2bb3 51de 4445 b013  ..+BA...+.Q.DE..
-00000a80: 2c42 4bb3 93d8 4443 b342 43b0 132c b018  ,BK...DC.BC..,..
-00000a90: 2c12 7f14 3d36 0014 3eb0 1441 3600 3601  ,...=6..>..A6.6.
-00000aa0: b018 29b0 1214 1333 b013 3156 5263 8840  ..)....3..1VRc.@
-00000ab0: c502 2242 810b 8083 6022 2924 2254 2b35  .."B....`")$"T+5
-00000ac0: 484e 2c2b 484f b013 2951 ded3 44c2 8050  HN,+HO..)Q..D..P
-00000ad0: b018 2b48 0ab0 1329 1442 3600 594a 2a57  ..+H...).B6.YJ*W
-00000ae0: 1281 05df 4462 c149 1823 0c12 810a b134  ....Db.I.#.....4
-00000af0: 01dc 444c 120a 230d 141c b136 0134 0159  ..DL..#....6.4.Y
-00000b00: 5151 c128 015d 4a01 5db0 1436 3600 5942  QQ.(.]J.]..66.YB
-00000b10: 4250 634a 2157 1281 05df 4459 c149 0f12  BPcJ!W....DY.I..
-00000b20: 0a23 0e14 1cb1 3601 3401 5950 6351 51c1  .#....6.4.YPcQQ.
-00000b30: 2801 5d4a 015d 5263 841c a140 1941 810b  (.]J.]Rc...@.A..
-00000b40: 8097 8007 202e 3026 2400 127f 1443 2500  .... .0&$....C%.
-00000b50: 132c 3601 5e51 6859 121f 2500 132a 1044  .,6.^QhY..%..*.D
-00000b60: b020 0001 3482 0159 2500 132b 4342 4242  . ..4..Y%..+CBBB
-00000b70: 4218 2500 132e 1437 3600 5951 6301 8138  B.%....76.YQc..8
-00000b80: 320c 695b 8116 80a0 1281 1f25 0010 30b1  2.i[.......%..0.
-00000b90: 1468 3600 3403 6383 48c1 020e 4581 0b80  .h6.4.c.H...E...
-00000ba0: a622 5648 0cb0 1436 1046 5236 8200 594a  ."VH...6.FR6..YJ
-00000bb0: 1f57 1281 05df 4457 c149 0d12 0a23 0f14  .W....DW.I...#..
-00000bc0: 1cb1 3601 3401 5951 51c1 2801 5d4a 015d  ..6.4.YQQ.(.]J.]
-00000bd0: 5163 8a74 2039 158b b223 2843 8610 8e07  Qc.t 9...#(C....
-00000be0: 6940 890c 8916 8f0d 890f 890f 8910 8920  i@............. 
-00000bf0: 890b 0011 8100 1681 0110 1516 8102 5116  ..............Q.
-00000c00: 4811 0c10 1634 0116 5180 1652 b020 0001  H....4..Q..R. ..
-00000c10: 1647 1181 0351 512a 0253 3301 3401 164a  .G...QQ*.S3.4..J
-00000c20: 1181 0332 0234 0116 4e11 8103 3203 3401  ...2.4..N...2.4.
-00000c30: 1650 1181 0332 0434 0116 4c11 8103 5150  .P...2.4..L...QP
-00000c40: 512a 0353 3305 3401 163e 1181 0332 0634  Q*.S3.4..>...2.4
-00000c50: 0116 5511 8103 3207 3401 165a 1181 0332  ..U...2.4..Z...2
-00000c60: 0834 0116 5c11 8103 3209 3401 165f 1181  .4..\...2.4.._..
-00000c70: 0332 0a34 0116 6311 8103 320b 3401 1665  .2.4..c...2.4..e
-00000c80: b063 0c84 703a 1847 5b81 0f80 b760 4048  .c..p:.G[....`@H
-00000c90: 4f4e 5612 1513 4851 de44 7312 8110 2500  ONV...HQ.Ds...%.
-00000ca0: b115 47b1 3601 1215 1848 127f 143d 3600  ..G.6....H...=6.
-00000cb0: 1449 b113 4a36 0159 1215 1348 143e 104b  .I..J6.Y...H.>.K
-00000cc0: 1215 144c 3600 1031 104d 3684 0059 1215  ...L6..1.M6..Y..
-00000cd0: 1348 6381 50b2 8001 0e4a 5381 1180 c860  .Hc.P....JS....`
-00000ce0: 120a 2310 141c b0b1 3602 3401 5951 6381  ..#.....6.4.YQc.
-00000cf0: 3c18 064e 80d0 1281 1232 0012 1413 3314  <..N.....2....3.
-00000d00: 4f36 0034 0134 0163 0182 2849 087b 5b80  O6.4.4.c..(I.{[.
-00000d10: d02b 00b0 5f4b 1830 02c1 c2b2 132e 1435  .+.._K.0.......5
-00000d20: 3600 4331 1040 b1dd 442b 812f 1442 2663  6.C1.@..D+./.B&c
-00000d30: 8308 1810 5080 d460 402d 2b26 1215 144e  ....P..`@-+&...N
-00000d40: 3600 1215 1351 db44 5823 1114 1c12 1513  6....Q.DX#......
-00000d50: 5136 01c0 120a b034 0159 1281 05b0 3401  Q6.....4.Y....4.
-00000d60: 6551 638a 00d0 4220 4c80 e060 402b 2922  eQc...B L..`@+)"
-00000d70: 204d 254d 391f 4135 1214 1333 1434 104d   M%M9.A5...3.4.M
-00000d80: 3601 c023 1214 1c36 00b0 1830 484e 127f  6..#...6...0HN..
-00000d90: 1443 2282 2c36 015e 5168 5912 0e34 00c1  .C".,6.^QhY..4..
-00000da0: 127f 1443 2282 2c36 015e 5168 5912 8113  ...C".,6.^QhY...
-00000db0: 120f 120e 3400 b134 0222 822c f781 f322  ....4..4.".,..."
-00000dc0: 8064 f434 01c2 1281 1312 1513 52b2 f282  .d.4........R...
-00000dd0: f734 0112 1518 5242 b47f 4a1f 5712 8105  .4....RB..J.W...
-00000de0: df44 57c3 490d 120a 2313 141c b336 0134  .DW.I...#....6.4
-00000df0: 0159 5151 c328 035d 4a01 5db0 132e 1437  .YQQ.(.]J.]....7
-00000e00: 3600 5951 6384 20d8 8501 183e 4b31 5372  6.YQc. ....>K1Sr
-00000e10: 80f6 6040 4a27 3312 8114 b012 6b34 0244  ..`@J'3.....k4.D
-00000e20: 5a12 1514 5036 0059 1214 3400 143f 104b  Z...P6.Y..4..?.K
-00000e30: b010 53b2 1054 b336 8600 6312 1434 0014  ..S..T.6..c..4..
-00000e40: 3b10 4bb0 1031 b136 8400 6387 0878 1855  ;.K..1.6..c..x.U
-00000e50: 9003 6020 2c32 2f30 2c2a 2912 1513 5112  ..` ,2/0,*)...Q.
-00000e60: 1514 4e36 00f3 c023 1423 1514 1cb0 1215  ..N6...#.#......
-00000e70: 1352 3602 2316 2b03 c112 1413 3314 4f36  .R6.#.+.....3.O6
-00000e80: 005f 4b33 3002 c2c3 b313 2e14 3536 0044  ._K30.......56.D
-00000e90: 4410 5642 4210 57c4 1022 8a12 8107 b434  D.VBB.W..".....4
-00000ea0: 01f3 f4c5 1058 141c b4b5 b236 03c6 b114  .....X.....6....
-00000eb0: 59b6 3601 5942 0b12 8115 b134 0163 8708  Y.6.YB.....4.c..
-00000ec0: 611e 5a31 9012 202b 2623 282c 3c29 2a23  a.Z1.. +&#(,<)*#
-00000ed0: 2212 1413 3314 34b0 5136 02c1 b151 de44  "...3.4.Q6...Q.D
-00000ee0: cb80 2b00 c2b0 141a 1040 3601 c312 1413  ..+......@6.....
-00000ef0: 3314 2636 005f 4b26 c4b4 1418 b380 5536  3.&6._K&......U6
-00000f00: 0144 5912 8107 b334 0181 d844 4fb3 8155  .DY....4...DO..U
-00000f10: 105b d944 47b2 1459 b436 0159 4218 1281  .[.DG..Y.6.YB...
-00000f20: 07b2 3401 80d9 4443 2b00 63b2 63b0 2b01  ..4...DC+.c.c.+.
-00000f30: 6386 3071 1c5c 3190 2160 2028 2a28 2a2b  c.0q.\1.!` (*(*+
-00000f40: 2325 3712 1514 5ab0 3601 c112 8107 b134  #%7...Z.6......4
-00000f50: 0180 d944 4823 1714 1cb0 3601 6312 8107  ...DH#....6.c...
-00000f60: b134 0181 d944 4b12 1413 33b1 8055 5513  .4...DK...3..UU.
-00000f70: 3063 2b00 c2b1 5f4b 18c3 b214 5910 5d14  0c+..._K....Y.].
-00000f80: 1cb3 1214 1333 b355 1330 3602 3601 5942  .....3.U.06.6.YB
-00000f90: 2610 5e14 23b2 3601 6388 5481 1028 5f31  &.^.#.6.c.T..(_1
-00000fa0: 9031 8007 8309 2822 2a2b 2a2b 2a23 2527  .1....("*+*+*#%'
-00000fb0: 302e 3200 c112 1514 5ab0 3601 c252 c312  0.2.....Z.6..R..
-00000fc0: 8107 b234 0180 d944 4bb3 2317 141c b036  ...4...DK.#....6
-00000fd0: 012a 0263 1281 07b2 3401 81d9 4455 2318  .*.c....4...DU#.
-00000fe0: 141c b280 55b3 3602 c4b1 b280 5534 01b4  ....U.6.....U4..
-00000ff0: 2a02 632b 00c5 b25f 4b18 c6b3 b1b6 3401  *.c+..._K.....4.
-00001000: e2c3 b514 5910 6014 1cb6 b336 0236 0159  ....Y.`....6.6.Y
-00001010: 4226 1061 141c 1062 1423 b536 0136 01c4  B&.a...b.#.6.6..
-00001020: b3b4 2a02 6301 8458 c902 127c 8120 9039  ..*.c..X...|. .9
-00001030: 2b22 592c 1214 1333 1434 b051 3602 c148  +"Y,...3.4.Q6..H
-00001040: 0fb1 51de 4442 5063 b114 4236 0063 4a21  ..Q.DBPc..B6.cJ!
-00001050: 5712 8105 df44 59c2 490f 120a 231b 141c  W....DY.I...#...
-00001060: b236 0134 0159 5063 5151 c228 025d 4a01  .6.4.YPcQQ.(.]J.
-00001070: 5d51 6384 28b8 020e 6390 5160 2257 2c48  ]Qc.(...c.Q`"W,H
-00001080: 0d12 7f14 3d36 0014 6336 0059 4a2a 5712  ....=6..c6.YJ*W.
-00001090: 8105 df44 62c0 4918 120a 2319 141c b036  ...Db.I...#....6
-000010a0: 0134 0159 127f 143d 3600 1464 3600 5951  .4.Y...=6..d6.YQ
-000010b0: 51c0 2800 5d4a 015d 5163 8218 2910 6581  Q.(.]J.]Qc..).e.
-000010c0: 1690 5c2c 2522 1214 1333 1434 1066 5136  ..\,%"...3.4.fQ6
-000010d0: 02c1 b151 de44 4251 63b0 b118 3051 6387  ...Q.DBQc...0Qc.
-000010e0: 3cd1 0220 1781 0490 6760 2042 2942 3027  <.. ....g` B)B0'
-000010f0: 5a2d 2c2b 4832 b014 1810 1936 0144 4252  Z-,+H2.....6.DBR
-00001100: 6332 00b0 141a 101b 3601 5e34 015f 4b16  c2......6.^4._K.
-00001110: c112 1eb1 3401 434c 1209 2301 141c b136  ....4.CL..#....6
-00001120: 0134 0159 4228 4a2e 5712 8105 df44 66c2  .4.YB(J.W....Df.
-00001130: 491c 1209 2302 141c b0b2 3602 3401 5912  I...#.....6.4.Y.
-00001140: 0a23 0314 1cb2 3601 3401 5950 6351 51c2  .#....6.4.YPcQQ.
-00001150: 2802 5d4a 015d 5263 0182 38b9 4008 675b  (.]J.]Rc..8.@.g[
-00001160: 9070 53b0 5353 4b18 c112 8107 b134 0180  .pS.SSK......4..
-00001170: d844 33b1 1468 3600 141a 3600 6759 4226  .D3..h6...6.gYB&
-00001180: 5163 8378 c102 161d 8104 907b 6020 2228  Qc.x.......{` "(
-00001190: 4e2c 480c 1203 1217 b034 0259 5263 4a21  N,H......4.YRcJ!
-000011a0: 5712 8105 df44 59c1 490f 120a 2304 141c  W....DY.I...#...
-000011b0: b136 0134 0159 5063 5151 c128 015d 4a01  .6.4.YPcQQ.(.]J.
-000011c0: 5d51 6383 3caa 019e 011e 8106 4490 8880  ]Qc.<.......D...
-000011d0: 0726 4486 2c60 2742 0001 2501 51de 4444  .&D.,`'B..%.Q.DD
-000011e0: 3200 2701 b0b1 2001 02c2 b225 0034 0144  2.'... ....%.4.D
-000011f0: 4252 6312 1f25 0025 0134 0263 0248 090a  BRc..%.%.4.c.H..
-00001200: 6981 1690 9051 6395 0893 124c 6a5b 5b81  i....Qc....Lj[[.
-00001210: 1790 9347 492d 2d28 2642 2528 3026 2228  ...GI--(&B%(0&"(
-00001220: 3122 2742 5028 302e 5122 5c46 2b2e 234e  1"'BP(0.Q"\F+.#N
-00001230: 4c42 1281 07b2 3401 c310 29b2 8055 d944  LB....4...)..U.D
-00001240: f380 b382 d944 6510 6bb2 8155 d944 5d10  .....De.k..U.D].
-00001250: 5e14 2312 1514 5536 0036 01c4 106c 141c  ^.#...U6.6...l..
-00001260: b436 01c4 2501 b434 0159 5263 b382 d844  .6..%..4.YRc...D
-00001270: 7b10 5fb2 8155 d944 5812 1514 5f10 31b2  {._..U.DX..._.1.
-00001280: 8255 3682 0030 02c5 c625 01b6 3401 5952  .U6..0...%..4.YR
-00001290: 6310 5cb2 8155 d944 5325 0112 1514 5c10  c.\..U.DS%....\.
-000012a0: 31b2 8255 3682 0034 0159 5263 2501 231a  1..U6..4.YRc%.#.
-000012b0: 3401 5952 63b3 82d8 449d 8110 6d25 007f  4.YRc...D...m%..
-000012c0: 55dd 4493 8125 0014 6e7f 3601 c7b7 146f  U.D..%..n.6....o
-000012d0: 106d 3601 82d9 4443 5242 4150 c8b7 1470  .m6...DCRBAP...p
-000012e0: 106d 102f 3602 1468 3600 c9b9 1471 3600  .m./6..h6....q6.
-000012f0: 4448 1281 13b9 3401 4241 51c9 4812 1215  DH....4.BAQ.H...
-00001300: 143e 2500 1053 b810 72b9 3684 01c5 4a1b  .>%..S..r.6...J.
-00001310: 5712 8105 df44 53ca 4909 2501 ba34 0159  W....DS.I.%..4.Y
-00001320: 5263 5151 ca28 0a5d 4a01 5d10 4014 2325  RcQQ.(.]J.].@.#%
-00001330: 0080 822e 0255 3601 cbb5 444e 2501 1073  .....U6...DN%..s
-00001340: 141c bb36 0134 0159 424c 2501 1074 141c  ...6.4.YBL%..t..
-00001350: bb36 0134 0159 5263 5063 9554 9e12 4b1f  .6.4.YRcPc.T..K.
-00001360: 8106 4490 c880 0883 0d85 0f27 4d2b 1f21  ..D........'M+.!
-00001370: 6327 2d42 7d2a 4c4d 5270 492b 6f2d 562a  c'-B}*LMRpI+o-V*
-00001380: 462b 2646 0a32 00c2 ba20 0101 c3b0 7f55  F+&F.2... .....U
-00001390: 1020 d9c4 b444 48b0 807f 2e02 5542 41b0  . ...DH.....UBA.
-000013a0: c512 8107 b534 0182 db44 fc81 1021 141c  .....4...D...!..
-000013b0: b580 5536 01b5 8155 b210 2214 23b5 8251  ..U6...U..".#..Q
-000013c0: 2e02 5536 0134 015b 5ac6 c7c8 4890 01b6  ..U6.4.[Z...H...
-000013d0: 1205 ddd3 444d 1281 0810 2414 1cb6 3601  ....DM....$...6.
-000013e0: 3401 5948 1212 8109 1025 141c b6b7 b836  4.YH.....%.....6
-000013f0: 0334 0127 0a4a 5057 1281 05df 44c7 80c9  .4.'.JPW....D...
-00001400: 493d b612 810a b934 01dd 446b 120a 2305  I=.....4..Dk..#.
-00001410: 141c b636 0134 0159 1281 0810 2414 1cb6  ...6.4.Y....$...
-00001420: 3601 3401 5912 8109 1025 141c b6b7 b836  6.4.Y....%.....6
-00001430: 0334 0127 0a42 4712 8105 b934 0165 5151  .4.'.BG....4.eQQ
-00001440: c928 095d 4a01 5db3 b4b7 250a 3403 270a  .(.]J.]...%.4.'.
-00001450: b112 810a 250a 3401 3401 5952 634a 4957  ....%.4.4.YRcJIW
-00001460: 1281 05df 44c0 80c9 4936 b123 0614 1cb6  ....D...I6.#....
-00001470: b7b9 3603 3401 5923 0712 810a b934 01dd  ..6.4.Y#.....4..
-00001480: 434b 2308 1281 0ab9 3401 dd44 52b6 1205  CK#.....4..DR...
-00001490: 1426 3600 dd44 4612 05b6 535b 5650 6351  .&6..DF...S[VPcQ
-000014a0: 51c9 2809 5d4a 015d b123 0934 0159 b123  Q.(.]J.].#.4.Y.#
-000014b0: 0a34 0159 5263 0287 5c59 9c01 7581 1890  .4.YRc..\Y..u...
-000014c0: d122 2e2d 3625 2d2c 2a2a 0003 51c1 1076  .".-6%-,**..Q..v
-000014d0: 2500 dd43 4710 7725 00dd 4475 3200 1281  %..CG.w%..Du2...
-000014e0: 1925 0034 0134 0127 03b0 b320 0102 1281  .%.4.4.'... ....
-000014f0: 1a80 1281 0725 0334 0182 3403 3401 c1b1  .....%.4..4.4...
-00001500: 5f4b 0ec2 2500 1470 b210 7836 0227 0042  _K..%..p..x6.'.B
-00001510: 3025 0014 7010 2210 6236 0227 0012 8114  0%..p.".b6.'....
-00001520: b112 6b34 0244 4a25 0014 1cb1 8137 0127  ..k4.DJ%.....7.'
-00001530: 0025 0063 0282 1049 087b 5b90 d32b 00b0  .%.c...I.{[..+..
-00001540: 5f4b 1530 02c1 c2b2 1077 d943 46b2 1076  _K.0.....w.CF..v
-00001550: d944 2eb1 2f14 4229 6382 286b 0c7b 5b5b  .D../.B)c.(k.{[[
-00001560: 5b90 d42b 00b2 5f4b 16c3 2500 2501 b355  [..+.._K..%.%..U
-00001570: 2501 b381 f255 81f2 2e02 552f 1442 2863  %....U....U/.B(c
-00001580: 853c c004 2479 5b81 1b81 1c81 1d90 de2b  .<..$y[........+
-00001590: 2346 5126 2346 2c12 8114 b312 811e 3402  #FQ&#F,.......4.
-000015a0: 445a b144 4612 07b3 3401 6310 5e14 2332  DZ.DF...4.c.^.#2
-000015b0: 0025 0014 4f36 0034 0136 0163 b210 7ad9  .%..O6.4.6.c..z.
-000015c0: 4455 b144 4612 07b3 3401 6310 5e14 2332  DU.DF...4.c.^.#2
-000015d0: 01b3 3401 3601 63b3 6302 8168 5908 7b5b  ..4.6.c.c..hY.{[
-000015e0: 90e2 2b00 b05f 4b10 3002 c1c2 107d 141c  ..+.._K.0....}..
-000015f0: b1b2 3602 2f14 422e 6381 4849 087b 5b90  ..6./.B.c.HI.{[.
-00001600: e82b 00b0 5f4b 0cc1 107e 141c b136 012f  .+.._K...~...6./
-00001610: 1442 3263 8400 c902 1627 8106 a019 6040  .B2c.....'....`@
-00001620: 2228 4e2d 480c 1203 121e b034 0259 5263  "(N-H......4.YRc
-00001630: 4a22 5712 8105 df44 5ac1 4910 120a 230b  J"W....DZ.I...#.
-00001640: 141c b0b1 3602 3401 5950 6351 51c1 2801  ....6.4.YPcQQ.(.
-00001650: 5d4a 015d 5163                           ]J.]Qc
+00000960: 3536 0043 4252 6350 6383 40a2 0116 3681  56.CBRcPc.@...6.
+00000970: 0b46 803b 6028 2e23 2ab0 132e 1437 3600  .F.;`(.#*....76.
+00000980: 59b0 1331 1214 1333 1426 3600 dd44 4db1  Y..1...3.&6..DM.
+00000990: 434a 1214 1333 b013 3153 5b56 1211 3400  CJ...3..1S[V..4.
+000009a0: 5951 6381 2011 1038 810b 8045 6040 28b0  YQc. ..8...E`@(.
+000009b0: 132e 1439 3600 59b0 6382 00a8 041c 3a81  ...96.Y.c.....:.
+000009c0: 0b81 0c81 0d81 0e80 4e60 4028 b013 2e14  ........N`@(....
+000009d0: 3736 0059 1211 3400 5951 6385 10b3 8001  76.Y..4.YQc.....
+000009e0: 1c3b 810b 4b31 8057 6060 3a4b 624e 29b2  .;..K1.W``:KbN).
+000009f0: 51de 4451 103c 141c 1281 0712 1413 3334  Q.DQ.<........34
+00000a00: 0136 0142 41b2 b018 3112 1414 32b0 1331  .6.BA...1...2..1
+00000a10: 3601 4442 5063 127f 143d 3600 143e b136  6.DBPc...=6..>.6
+00000a20: 01b0 1829 b012 1413 33b0 1331 5652 6387  ...)....3..1VRc.
+00000a30: 48c0 8501 243f 810b 4b53 5480 6980 082f  H...$?..KST.i../
+00000a40: 4b62 244e 5852 2910 4014 23b1 8082 2e02  Kb$NXR).@.#.....
+00000a50: 5536 01b0 1831 1214 1432 b013 3136 0144  U6...1...2..16.D
+00000a60: 4250 63b1 b018 2ab2 51de 4445 b013 2b42  BPc...*.Q.DE..+B
+00000a70: 41b2 b018 2bb3 51de 4445 b013 2c42 4bb3  A...+.Q.DE..,BK.
+00000a80: 93d8 4443 b342 43b0 132c b018 2c12 7f14  ..DC.BC..,..,...
+00000a90: 3d36 0014 3eb0 1441 3600 3601 b018 29b0  =6..>..A6.6...).
+00000aa0: 1214 1333 b013 3156 5263 8840 c502 2242  ...3..1VRc.@.."B
+00000ab0: 810b 8082 6022 2924 2254 2b35 484e 2c2b  ....`")$"T+5HN,+
+00000ac0: 484f b013 2951 ded3 44c2 8050 b018 2b48  HO..)Q..D..P..+H
+00000ad0: 0ab0 1329 1442 3600 594a 2a57 1281 05df  ...).B6.YJ*W....
+00000ae0: 4462 c149 1823 0c12 810a b134 01dc 444c  Db.I.#.....4..DL
+00000af0: 120a 230d 141c b136 0134 0159 5151 c128  ..#....6.4.YQQ.(
+00000b00: 015d 4a01 5db0 1436 3600 5942 4250 634a  .]J.]..66.YBBPcJ
+00000b10: 2157 1281 05df 4459 c149 0f12 0a23 0e14  !W....DY.I...#..
+00000b20: 1cb1 3601 3401 5950 6351 51c1 2801 5d4a  ..6.4.YPcQQ.(.]J
+00000b30: 015d 5263 841c a140 1941 810b 8096 8007  .]Rc...@.A......
+00000b40: 202e 3026 2400 127f 1443 2500 132c 3601   .0&$....C%..,6.
+00000b50: 5e51 6859 121f 2500 132a 1044 b020 0001  ^QhY..%..*.D. ..
+00000b60: 3482 0159 2500 132b 4342 4242 4218 2500  4..Y%..+CBBBB.%.
+00000b70: 132e 1437 3600 5951 6301 8138 320c 695b  ...76.YQc..82.i[
+00000b80: 8116 809f 1281 1f25 0010 30b1 1468 3600  .......%..0..h6.
+00000b90: 3403 6383 48c1 020e 4581 0b80 a522 5648  4.c.H...E...."VH
+00000ba0: 0cb0 1436 1046 5236 8200 594a 1f57 1281  ...6.FR6..YJ.W..
+00000bb0: 05df 4457 c149 0d12 0a23 0f14 1cb1 3601  ..DW.I...#....6.
+00000bc0: 3401 5951 51c1 2801 5d4a 015d 5163 8a74  4.YQQ.(.]J.]Qc.t
+00000bd0: 2039 158b b123 2843 8610 8e07 6940 890c   9...#(C....i@..
+00000be0: 8916 8f0d 890f 890f 8910 8920 890b 0011  ........... ....
+00000bf0: 8100 1681 0110 1516 8102 5116 4811 0c10  ..........Q.H...
+00000c00: 1634 0116 5180 1652 b020 0001 1647 1181  .4..Q..R. ...G..
+00000c10: 0351 512a 0253 3301 3401 164a 1181 0332  .QQ*.S3.4..J...2
+00000c20: 0234 0116 4e11 8103 3203 3401 1650 1181  .4..N...2.4..P..
+00000c30: 0332 0434 0116 4c11 8103 5150 512a 0353  .2.4..L...QPQ*.S
+00000c40: 3305 3401 163e 1181 0332 0634 0116 5511  3.4..>...2.4..U.
+00000c50: 8103 3207 3401 165a 1181 0332 0834 0116  ..2.4..Z...2.4..
+00000c60: 5c11 8103 3209 3401 165f 1181 0332 0a34  \...2.4.._...2.4
+00000c70: 0116 6311 8103 320b 3401 1665 b063 0c84  ..c...2.4..e.c..
+00000c80: 703a 1847 5b81 0f80 b660 4048 4f4e 5612  p:.G[....`@HONV.
+00000c90: 1513 4851 de44 7312 8110 2500 b115 47b1  ..HQ.Ds...%...G.
+00000ca0: 3601 1215 1848 127f 143d 3600 1449 b113  6....H...=6..I..
+00000cb0: 4a36 0159 1215 1348 143e 104b 1215 144c  J6.Y...H.>.K...L
+00000cc0: 3600 1031 104d 3684 0059 1215 1348 6381  6..1.M6..Y...Hc.
+00000cd0: 50b2 8001 0e4a 5381 1180 c760 120a 2310  P....JS....`..#.
+00000ce0: 141c b0b1 3602 3401 5951 6381 3c18 064e  ....6.4.YQc.<..N
+00000cf0: 80cf 1281 1232 0012 1413 3314 4f36 0034  .....2....3.O6.4
+00000d00: 0134 0163 0182 2849 087b 5b80 cf2b 00b0  .4.c..(I.{[..+..
+00000d10: 5f4b 1830 02c1 c2b2 132e 1435 3600 4331  _K.0.......56.C1
+00000d20: 1040 b1dd 442b 812f 1442 2663 8308 1810  .@..D+./.B&c....
+00000d30: 5080 d360 402d 2b26 1215 144e 3600 1215  P..`@-+&...N6...
+00000d40: 1351 db44 5823 1114 1c12 1513 5136 01c0  .Q.DX#......Q6..
+00000d50: 120a b034 0159 1281 05b0 3401 6551 638a  ...4.Y....4.eQc.
+00000d60: 00d0 4220 4c80 df60 402b 2922 204d 254d  ..B L..`@+)" M%M
+00000d70: 391f 4135 1214 1333 1434 104d 3601 c023  9.A5...3.4.M6..#
+00000d80: 1214 1c36 00b0 1830 484e 127f 1443 2282  ...6...0HN...C".
+00000d90: 2c36 015e 5168 5912 0e34 00c1 127f 1443  ,6.^QhY..4.....C
+00000da0: 2282 2c36 015e 5168 5912 8113 120f 120e  ".,6.^QhY.......
+00000db0: 3400 b134 0222 822c f781 f322 8064 f434  4..4.".,...".d.4
+00000dc0: 01c2 1281 1312 1513 52b2 f282 f734 0112  ........R....4..
+00000dd0: 1518 5242 b47f 4a1f 5712 8105 df44 57c3  ..RB..J.W....DW.
+00000de0: 490d 120a 2313 141c b336 0134 0159 5151  I...#....6.4.YQQ
+00000df0: c328 035d 4a01 5db0 132e 1437 3600 5951  .(.]J.]....76.YQ
+00000e00: 6384 20d8 8501 183e 4b31 5372 80f5 6040  c. ....>K1Sr..`@
+00000e10: 4a27 3312 8114 b012 6b34 0244 5a12 1514  J'3.....k4.DZ...
+00000e20: 5036 0059 1214 3400 143f 104b b010 53b2  P6.Y..4..?.K..S.
+00000e30: 1054 b336 8600 6312 1434 0014 3b10 4bb0  .T.6..c..4..;.K.
+00000e40: 1031 b136 8400 6387 0878 1855 9002 6020  .1.6..c..x.U..` 
+00000e50: 2c32 2f30 2c2a 2912 1513 5112 1514 4e36  ,2/0,*)...Q...N6
+00000e60: 00f3 c023 1423 1514 1cb0 1215 1352 3602  ...#.#.......R6.
+00000e70: 2316 2b03 c112 1413 3314 4f36 005f 4b33  #.+.....3.O6._K3
+00000e80: 3002 c2c3 b313 2e14 3536 0044 4410 5642  0.......56.DD.VB
+00000e90: 4210 57c4 1022 8a12 8107 b434 01f3 f4c5  B.W..".....4....
+00000ea0: 1058 141c b4b5 b236 03c6 b114 59b6 3601  .X.....6....Y.6.
+00000eb0: 5942 0b12 8115 b134 0163 8708 611e 5a31  YB.....4.c..a.Z1
+00000ec0: 9011 202b 2623 282c 3c29 2a23 2212 1413  .. +&#(,<)*#"...
+00000ed0: 3314 34b0 5136 02c1 b151 de44 cb80 2b00  3.4.Q6...Q.D..+.
+00000ee0: c2b0 141a 1040 3601 c312 1413 3314 2636  .....@6.....3.&6
+00000ef0: 005f 4b26 c4b4 1418 b380 5536 0144 5912  ._K&......U6.DY.
+00000f00: 8107 b334 0181 d844 4fb3 8155 105b d944  ...4...DO..U.[.D
+00000f10: 47b2 1459 b436 0159 4218 1281 07b2 3401  G..Y.6.YB.....4.
+00000f20: 80d9 4443 2b00 63b2 63b0 2b01 6386 3071  ..DC+.c.c.+.c.0q
+00000f30: 1c5c 3190 2060 2028 2a28 2a2b 2325 3712  .\1. ` (*(*+#%7.
+00000f40: 1514 5ab0 3601 c112 8107 b134 0180 d944  ..Z.6......4...D
+00000f50: 4823 1714 1cb0 3601 6312 8107 b134 0181  H#....6.c....4..
+00000f60: d944 4b12 1413 33b1 8055 5513 3063 2b00  .DK...3..UU.0c+.
+00000f70: c2b1 5f4b 18c3 b214 5910 5d14 1cb3 1214  .._K....Y.].....
+00000f80: 1333 b355 1330 3602 3601 5942 2610 5e14  .3.U.06.6.YB&.^.
+00000f90: 23b2 3601 6388 5481 1028 5f31 9030 8007  #.6.c.T..(_1.0..
+00000fa0: 8309 2822 2a2b 2a2b 2a23 2527 302e 3200  ..("*+*+*#%'0.2.
+00000fb0: c112 1514 5ab0 3601 c252 c312 8107 b234  ....Z.6..R.....4
+00000fc0: 0180 d944 4bb3 2317 141c b036 012a 0263  ...DK.#....6.*.c
+00000fd0: 1281 07b2 3401 81d9 4455 2318 141c b280  ....4...DU#.....
+00000fe0: 55b3 3602 c4b1 b280 5534 01b4 2a02 632b  U.6.....U4..*.c+
+00000ff0: 00c5 b25f 4b18 c6b3 b1b6 3401 e2c3 b514  ..._K.....4.....
+00001000: 5910 6014 1cb6 b336 0236 0159 4226 1061  Y.`....6.6.YB&.a
+00001010: 141c 1062 1423 b536 0136 01c4 b3b4 2a02  ...b.#.6.6....*.
+00001020: 6301 8458 c902 127c 8120 9038 2b22 592c  c..X...|. .8+"Y,
+00001030: 1214 1333 1434 b051 3602 c148 0fb1 51de  ...3.4.Q6..H..Q.
+00001040: 4442 5063 b114 4236 0063 4a21 5712 8105  DBPc..B6.cJ!W...
+00001050: df44 59c2 490f 120a 231b 141c b236 0134  .DY.I...#....6.4
+00001060: 0159 5063 5151 c228 025d 4a01 5d51 6384  .YPcQQ.(.]J.]Qc.
+00001070: 28b8 020e 6390 5060 2257 2c48 0d12 7f14  (...c.P`"W,H....
+00001080: 3d36 0014 6336 0059 4a2a 5712 8105 df44  =6..c6.YJ*W....D
+00001090: 62c0 4918 120a 2319 141c b036 0134 0159  b.I...#....6.4.Y
+000010a0: 127f 143d 3600 1464 3600 5951 51c0 2800  ...=6..d6.YQQ.(.
+000010b0: 5d4a 015d 5163 8218 2910 6581 1690 5b2c  ]J.]Qc..).e...[,
+000010c0: 2522 1214 1333 1434 1066 5136 02c1 b151  %"...3.4.fQ6...Q
+000010d0: de44 4251 63b0 b118 3051 6387 3cd1 0220  .DBQc...0Qc.<.. 
+000010e0: 1781 0490 6660 2042 2942 3027 5a2d 2c2b  ....f` B)B0'Z-,+
+000010f0: 4832 b014 1810 1936 0144 4252 6332 00b0  H2.....6.DBRc2..
+00001100: 141a 101b 3601 5e34 015f 4b16 c112 1eb1  ....6.^4._K.....
+00001110: 3401 434c 1209 2301 141c b136 0134 0159  4.CL..#....6.4.Y
+00001120: 4228 4a2e 5712 8105 df44 66c2 491c 1209  B(J.W....Df.I...
+00001130: 2302 141c b0b2 3602 3401 5912 0a23 0314  #.....6.4.Y..#..
+00001140: 1cb2 3601 3401 5950 6351 51c2 2802 5d4a  ..6.4.YPcQQ.(.]J
+00001150: 015d 5263 0182 38b9 4008 675b 906f 53b0  .]Rc..8.@.g[.oS.
+00001160: 5353 4b18 c112 8107 b134 0180 d844 33b1  SSK......4...D3.
+00001170: 1468 3600 141a 3600 6759 4226 5163 8378  .h6...6.gYB&Qc.x
+00001180: c102 161d 8104 907a 6020 2228 4e2c 480c  .......z` "(N,H.
+00001190: 1203 1217 b034 0259 5263 4a21 5712 8105  .....4.YRcJ!W...
+000011a0: df44 59c1 490f 120a 2304 141c b136 0134  .DY.I...#....6.4
+000011b0: 0159 5063 5151 c128 015d 4a01 5d51 6383  .YPcQQ.(.]J.]Qc.
+000011c0: 3caa 019e 011e 8106 4490 8780 0726 4486  <.......D....&D.
+000011d0: 2c60 2742 0001 2501 51de 4444 3200 2701  ,`'B..%.Q.DD2.'.
+000011e0: b0b1 2001 02c2 b225 0034 0144 4252 6312  .. ....%.4.DBRc.
+000011f0: 1f25 0025 0134 0263 0248 090a 6981 1690  .%.%.4.c.H..i...
+00001200: 8f51 6395 0893 124c 6a5b 5b81 1790 9247  .Qc....Lj[[....G
+00001210: 492d 2d28 2642 2528 3026 2228 3122 2742  I--(&B%(0&"(1"'B
+00001220: 5028 302e 5122 5c46 2b2e 234e 4c42 1281  P(0.Q"\F+.#NLB..
+00001230: 07b2 3401 c310 29b2 8055 d944 f380 b382  ..4...)..U.D....
+00001240: d944 6510 6bb2 8155 d944 5d10 5e14 2312  .De.k..U.D].^.#.
+00001250: 1514 5536 0036 01c4 106c 141c b436 01c4  ..U6.6...l...6..
+00001260: 2501 b434 0159 5263 b382 d844 7b10 5fb2  %..4.YRc...D{._.
+00001270: 8155 d944 5812 1514 5f10 31b2 8255 3682  .U.DX..._.1..U6.
+00001280: 0030 02c5 c625 01b6 3401 5952 6310 5cb2  .0...%..4.YRc.\.
+00001290: 8155 d944 5325 0112 1514 5c10 31b2 8255  .U.DS%....\.1..U
+000012a0: 3682 0034 0159 5263 2501 231a 3401 5952  6..4.YRc%.#.4.YR
+000012b0: 63b3 82d8 449d 8110 6d25 007f 55dd 4493  c...D...m%..U.D.
+000012c0: 8125 0014 6e7f 3601 c7b7 146f 106d 3601  .%..n.6....o.m6.
+000012d0: 82d9 4443 5242 4150 c8b7 1470 106d 102f  ..DCRBAP...p.m./
+000012e0: 3602 1468 3600 c9b9 1471 3600 4448 1281  6..h6....q6.DH..
+000012f0: 13b9 3401 4241 51c9 4812 1215 143e 2500  ..4.BAQ.H....>%.
+00001300: 1053 b810 72b9 3684 01c5 4a1b 5712 8105  .S..r.6...J.W...
+00001310: df44 53ca 4909 2501 ba34 0159 5263 5151  .DS.I.%..4.YRcQQ
+00001320: ca28 0a5d 4a01 5d10 4014 2325 0080 822e  .(.]J.].@.#%....
+00001330: 0255 3601 cbb5 444e 2501 1073 141c bb36  .U6...DN%..s...6
+00001340: 0134 0159 424c 2501 1074 141c bb36 0134  .4.YBL%..t...6.4
+00001350: 0159 5263 5063 9554 9e12 4b1f 8106 4490  .YRcPc.T..K...D.
+00001360: c780 0883 0d85 0f27 4d2b 1f21 6327 2d42  .......'M+.!c'-B
+00001370: 7d2a 4c4d 5270 492b 6f2d 562a 462b 2646  }*LMRpI+o-V*F+&F
+00001380: 0a32 00c2 ba20 0101 c3b0 7f55 1020 d9c4  .2... .....U. ..
+00001390: b444 48b0 807f 2e02 5542 41b0 c512 8107  .DH.....UBA.....
+000013a0: b534 0182 db44 fc81 1021 141c b580 5536  .4...D...!....U6
+000013b0: 01b5 8155 b210 2214 23b5 8251 2e02 5536  ...U..".#..Q..U6
+000013c0: 0134 015b 5ac6 c7c8 4890 01b6 1205 ddd3  .4.[Z...H.......
+000013d0: 444d 1281 0810 2414 1cb6 3601 3401 5948  DM....$...6.4.YH
+000013e0: 1212 8109 1025 141c b6b7 b836 0334 0127  .....%.....6.4.'
+000013f0: 0a4a 5057 1281 05df 44c7 80c9 493d b612  .JPW....D...I=..
+00001400: 810a b934 01dd 446b 120a 2305 141c b636  ...4..Dk..#....6
+00001410: 0134 0159 1281 0810 2414 1cb6 3601 3401  .4.Y....$...6.4.
+00001420: 5912 8109 1025 141c b6b7 b836 0334 0127  Y....%.....6.4.'
+00001430: 0a42 4712 8105 b934 0165 5151 c928 095d  .BG....4.eQQ.(.]
+00001440: 4a01 5db3 b4b7 250a 3403 270a b112 810a  J.]...%.4.'.....
+00001450: 250a 3401 3401 5952 634a 4957 1281 05df  %.4.4.YRcJIW....
+00001460: 44c0 80c9 4936 b123 0614 1cb6 b7b9 3603  D...I6.#......6.
+00001470: 3401 5923 0712 810a b934 01dd 434b 2308  4.Y#.....4..CK#.
+00001480: 1281 0ab9 3401 dd44 52b6 1205 1426 3600  ....4..DR....&6.
+00001490: dd44 4612 05b6 535b 5650 6351 51c9 2809  .DF...S[VPcQQ.(.
+000014a0: 5d4a 015d b123 0934 0159 b123 0a34 0159  ]J.].#.4.Y.#.4.Y
+000014b0: 5263 0287 5c59 9c01 7581 1890 d022 2e2d  Rc..\Y..u....".-
+000014c0: 3625 2d2c 2a2a 0003 51c1 1076 2500 dd43  6%-,**..Q..v%..C
+000014d0: 4710 7725 00dd 4475 3200 1281 1925 0034  G.w%..Du2....%.4
+000014e0: 0134 0127 03b0 b320 0102 1281 1a80 1281  .4.'... ........
+000014f0: 0725 0334 0182 3403 3401 c1b1 5f4b 0ec2  .%.4..4.4..._K..
+00001500: 2500 1470 b210 7836 0227 0042 3025 0014  %..p..x6.'.B0%..
+00001510: 7010 2210 6236 0227 0012 8114 b112 6b34  p.".b6.'......k4
+00001520: 0244 4a25 0014 1cb1 8137 0127 0025 0063  .DJ%.....7.'.%.c
+00001530: 0282 1049 087b 5b90 d22b 00b0 5f4b 1530  ...I.{[..+.._K.0
+00001540: 02c1 c2b2 1077 d943 46b2 1076 d944 2eb1  .....w.CF..v.D..
+00001550: 2f14 4229 6382 286b 0c7b 5b5b 5b90 d32b  /.B)c.(k.{[[[..+
+00001560: 00b2 5f4b 16c3 2500 2501 b355 2501 b381  .._K..%.%..U%...
+00001570: f255 81f2 2e02 552f 1442 2863 853c c004  .U....U/.B(c.<..
+00001580: 2479 5b81 1b81 1c81 1d90 dd2b 2346 5126  $y[........+#FQ&
+00001590: 2346 2c12 8114 b312 811e 3402 445a b144  #F,.......4.DZ.D
+000015a0: 4612 07b3 3401 6310 5e14 2332 0025 0014  F...4.c.^.#2.%..
+000015b0: 4f36 0034 0136 0163 b210 7ad9 4455 b144  O6.4.6.c..z.DU.D
+000015c0: 4612 07b3 3401 6310 5e14 2332 01b3 3401  F...4.c.^.#2..4.
+000015d0: 3601 63b3 6302 8168 5908 7b5b 90e1 2b00  6.c.c..hY.{[..+.
+000015e0: b05f 4b10 3002 c1c2 107d 141c b1b2 3602  ._K.0....}....6.
+000015f0: 2f14 422e 6381 4849 087b 5b90 e72b 00b0  /.B.c.HI.{[..+..
+00001600: 5f4b 0cc1 107e 141c b136 012f 1442 3263  _K...~...6./.B2c
+00001610: 8400 c902 1627 8106 a018 6040 2228 4e2d  .....'....`@"(N-
+00001620: 480c 1203 121e b034 0259 5263 4a22 5712  H......4.YRcJ"W.
+00001630: 8105 df44 5ac1 4910 120a 230b 141c b0b1  ...DZ.I...#.....
+00001640: 3602 3401 5950 6351 51c1 2801 5d4a 015d  6.4.YPcQQ.(.]J.]
+00001650: 5163                                     Qc
```

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.21.4/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.21.5/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*

