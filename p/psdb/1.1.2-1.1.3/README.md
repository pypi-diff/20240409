# Comparing `tmp/psdb-1.1.2.tar.gz` & `tmp/psdb-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdb-1.1.2.tar", last modified: Tue Dec 12 01:11:05 2023, max compression
+gzip compressed data, was "psdb-1.1.3.tar", last modified: Tue Apr  9 21:18:54 2024, max compression
```

## Comparing `psdb-1.1.2.tar` & `psdb-1.1.3.tar`

### file list

```diff
@@ -1,216 +1,233 @@
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.769446 psdb-1.1.2/
--rw-r--r--   0 greent7    (502) staff       (20)    26526 2021-11-05 03:30:42.000000 psdb-1.1.2/LICENSE
--rw-r--r--   0 greent7    (502) staff       (20)     8117 2023-12-12 01:11:05.769389 psdb-1.1.2/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     7465 2021-11-05 03:30:42.000000 psdb-1.1.2/README.rst
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.750082 psdb-1.1.2/psdb/
--rw-r--r--   0 greent7    (502) staff       (20)      493 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     6131 2022-07-23 01:35:07.000000 psdb-1.1.2/psdb/access_port.py
--rw-r--r--   0 greent7    (502) staff       (20)     7531 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/ble_tool.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.751031 psdb-1.1.2/psdb/block/
--rw-r--r--   0 greent7    (502) staff       (20)      229 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/block/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      860 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/block/bd.py
--rw-r--r--   0 greent7    (502) staff       (20)     1262 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/block/rambd.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.751699 psdb-1.1.2/psdb/component/
--rw-r--r--   0 greent7    (502) staff       (20)      265 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/component/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     4737 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/component/component.py
--rw-r--r--   0 greent7    (502) staff       (20)     2262 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/component/matcher.py
--rw-r--r--   0 greent7    (502) staff       (20)     1809 2023-02-19 02:03:20.000000 psdb-1.1.2/psdb/cordic_test.py
--rw-r--r--   0 greent7    (502) staff       (20)     3070 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/core_tool.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.752342 psdb-1.1.2/psdb/cpus/
--rw-r--r--   0 greent7    (502) staff       (20)     2010 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/cpus/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     3729 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/cpus/cortex.py
--rw-r--r--   0 greent7    (502) staff       (20)      213 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/cpus/cortex_m0p.py
--rw-r--r--   0 greent7    (502) staff       (20)      211 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/cpus/cortex_m33.py
--rw-r--r--   0 greent7    (502) staff       (20)      211 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/cpus/cortex_m4.py
--rw-r--r--   0 greent7    (502) staff       (20)      211 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/cpus/cortex_m7.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.752641 psdb-1.1.2/psdb/devices/
--rw-r--r--   0 greent7    (502) staff       (20)      760 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/__init__.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.753861 psdb-1.1.2/psdb/devices/core/
--rw-r--r--   0 greent7    (502) staff       (20)     1898 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     2140 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/bpu.py
--rw-r--r--   0 greent7    (502) staff       (20)     2430 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/coresight_0x9.py
--rw-r--r--   0 greent7    (502) staff       (20)      631 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/devices/core/cortex_subdevice.py
--rw-r--r--   0 greent7    (502) staff       (20)     6013 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/dwt_m4.py
--rw-r--r--   0 greent7    (502) staff       (20)     3775 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/fpb.py
--rw-r--r--   0 greent7    (502) staff       (20)     5703 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/itm_m4.py
--rw-r--r--   0 greent7    (502) staff       (20)     3003 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/scs_base.py
--rw-r--r--   0 greent7    (502) staff       (20)     5837 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/scs_v6_m.py
--rw-r--r--   0 greent7    (502) staff       (20)    12220 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/scs_v7_m.py
--rw-r--r--   0 greent7    (502) staff       (20)    17713 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/scs_v8_m.py
--rw-r--r--   0 greent7    (502) staff       (20)     3885 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/core/tpiu_m4.py
--rw-r--r--   0 greent7    (502) staff       (20)     9842 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/device.py
--rw-r--r--   0 greent7    (502) staff       (20)     6805 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/flash.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.754056 psdb-1.1.2/psdb/devices/msp432/
--rw-r--r--   0 greent7    (502) staff       (20)      117 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/devices/msp432/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)    17844 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/msp432/flctl.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.756353 psdb-1.1.2/psdb/devices/stm32/
--rw-r--r--   0 greent7    (502) staff       (20)     1228 2023-02-19 02:03:20.000000 psdb-1.1.2/psdb/devices/stm32/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)    16303 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/adc.py
--rw-r--r--   0 greent7    (502) staff       (20)    14259 2023-02-14 21:53:38.000000 psdb-1.1.2/psdb/devices/stm32/adc_14.py
--rw-r--r--   0 greent7    (502) staff       (20)    16199 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/adc_16.py
--rw-r--r--   0 greent7    (502) staff       (20)     1379 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/advanced_control_timer.py
--rw-r--r--   0 greent7    (502) staff       (20)      663 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/basic_timer.py
--rw-r--r--   0 greent7    (502) staff       (20)     1273 2023-02-19 02:03:20.000000 psdb-1.1.2/psdb/devices/stm32/cordic.py
--rw-r--r--   0 greent7    (502) staff       (20)     2087 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/devices/stm32/crs.py
--rw-r--r--   0 greent7    (502) staff       (20)     4605 2023-02-14 21:53:33.000000 psdb-1.1.2/psdb/devices/stm32/dac.py
--rw-r--r--   0 greent7    (502) staff       (20)     5710 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/dma.py
--rw-r--r--   0 greent7    (502) staff       (20)      659 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/dma_mux.py
--rw-r--r--   0 greent7    (502) staff       (20)     9499 2023-03-02 05:44:33.000000 psdb-1.1.2/psdb/devices/stm32/flash_type1.py
--rw-r--r--   0 greent7    (502) staff       (20)     7927 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/general_purpose_timer_16x1.py
--rw-r--r--   0 greent7    (502) staff       (20)     1189 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/general_purpose_timer_16x2.py
--rw-r--r--   0 greent7    (502) staff       (20)     1227 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/general_purpose_timer_16x4.py
--rw-r--r--   0 greent7    (502) staff       (20)     9751 2023-02-14 21:53:36.000000 psdb-1.1.2/psdb/devices/stm32/general_purpose_timer_32.py
--rw-r--r--   0 greent7    (502) staff       (20)      995 2023-02-14 21:53:41.000000 psdb-1.1.2/psdb/devices/stm32/gpdma.py
--rw-r--r--   0 greent7    (502) staff       (20)    11305 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/gpio.py
--rw-r--r--   0 greent7    (502) staff       (20)     9200 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/lpuart.py
--rw-r--r--   0 greent7    (502) staff       (20)     4055 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/qspi.py
--rw-r--r--   0 greent7    (502) staff       (20)     8373 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/usb.py
--rw-r--r--   0 greent7    (502) staff       (20)    62011 2021-11-26 09:53:24.000000 psdb-1.1.2/psdb/devices/stm32/usb_hs.py
--rw-r--r--   0 greent7    (502) staff       (20)      708 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32/vrefbuf.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.756543 psdb-1.1.2/psdb/devices/stm32g0/
--rw-r--r--   0 greent7    (502) staff       (20)      117 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/devices/stm32g0/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     4907 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g0/flash.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.758054 psdb-1.1.2/psdb/devices/stm32g4/
--rw-r--r--   0 greent7    (502) staff       (20)      578 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/devices/stm32g4/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      564 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g4/comparator.py
--rw-r--r--   0 greent7    (502) staff       (20)     3048 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g4/dbgmcu.py
--rw-r--r--   0 greent7    (502) staff       (20)     4386 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g4/flash_2.py
--rw-r--r--   0 greent7    (502) staff       (20)     7799 2022-07-23 01:35:42.000000 psdb-1.1.2/psdb/devices/stm32g4/flash_3.py
--rw-r--r--   0 greent7    (502) staff       (20)     4450 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g4/flash_4.py
--rw-r--r--   0 greent7    (502) staff       (20)      732 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g4/opamp.py
--rw-r--r--   0 greent7    (502) staff       (20)    18411 2023-02-19 02:03:20.000000 psdb-1.1.2/psdb/devices/stm32g4/pwr.py
--rw-r--r--   0 greent7    (502) staff       (20)    26502 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g4/rcc.py
--rw-r--r--   0 greent7    (502) staff       (20)    11684 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g4/rtc.py
--rw-r--r--   0 greent7    (502) staff       (20)     4862 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g4/syscfg.py
--rw-r--r--   0 greent7    (502) staff       (20)     5060 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32g4/tamp.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.759463 psdb-1.1.2/psdb/devices/stm32h7/
--rw-r--r--   0 greent7    (502) staff       (20)      602 2023-02-14 21:49:51.000000 psdb-1.1.2/psdb/devices/stm32h7/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      539 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/devices/stm32h7/art.py
--rw-r--r--   0 greent7    (502) staff       (20)    10859 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32h7/flash.py
--rw-r--r--   0 greent7    (502) staff       (20)     7152 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32h7/flash_dp.py
--rw-r--r--   0 greent7    (502) staff       (20)     1325 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32h7/flash_up.py
--rw-r--r--   0 greent7    (502) staff       (20)     2777 2023-02-14 21:49:43.000000 psdb-1.1.2/psdb/devices/stm32h7/opamp.py
--rw-r--r--   0 greent7    (502) staff       (20)     7767 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32h7/pwr.py
--rw-r--r--   0 greent7    (502) staff       (20)   107742 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32h7/rcc.py
--rw-r--r--   0 greent7    (502) staff       (20)     8613 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32h7/syscfg.py
--rw-r--r--   0 greent7    (502) staff       (20)     1050 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32h7/tim15.py
--rw-r--r--   0 greent7    (502) staff       (20)     6348 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32h7/tim17.py
--rw-r--r--   0 greent7    (502) staff       (20)     8952 2023-02-14 21:50:27.000000 psdb-1.1.2/psdb/devices/stm32h7/tim2_5.py
--rw-r--r--   0 greent7    (502) staff       (20)     1847 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32h7/tim6.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.760412 psdb-1.1.2/psdb/devices/stm32u5/
--rw-r--r--   0 greent7    (502) staff       (20)      324 2023-12-12 01:09:19.000000 psdb-1.1.2/psdb/devices/stm32u5/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     4236 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32u5/dbgmcu.py
--rw-r--r--   0 greent7    (502) staff       (20)    21891 2023-03-02 05:49:54.000000 psdb-1.1.2/psdb/devices/stm32u5/flash.py
--rw-r--r--   0 greent7    (502) staff       (20)     6342 2023-12-12 01:09:19.000000 psdb-1.1.2/psdb/devices/stm32u5/i2c.py
--rw-r--r--   0 greent7    (502) staff       (20)    28925 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32u5/pwr.py
--rw-r--r--   0 greent7    (502) staff       (20)    38490 2023-09-29 22:54:27.000000 psdb-1.1.2/psdb/devices/stm32u5/rcc.py
--rw-r--r--   0 greent7    (502) staff       (20)    12112 2023-09-29 22:54:27.000000 psdb-1.1.2/psdb/devices/stm32u5/rtc.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.761188 psdb-1.1.2/psdb/devices/stm32wb55/
--rw-r--r--   0 greent7    (502) staff       (20)      237 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/devices/stm32wb55/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)    14327 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/flash.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.763110 psdb-1.1.2/psdb/devices/stm32wb55/ipc/
--rw-r--r--   0 greent7    (502) staff       (20)     2502 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     7156 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/binaries.py
--rw-r--r--   0 greent7    (502) staff       (20)    23377 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/ble_channel.py
--rw-r--r--   0 greent7    (502) staff       (20)      130 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/ble_client.py
--rw-r--r--   0 greent7    (502) staff       (20)     3718 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/circular_queue.py
--rw-r--r--   0 greent7    (502) staff       (20)     7214 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/fus_client.py
--rw-r--r--   0 greent7    (502) staff       (20)     1139 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/gatt.py
--rw-r--r--   0 greent7    (502) staff       (20)     4117 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/ipc.py
--rw-r--r--   0 greent7    (502) staff       (20)    10378 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/mailbox.py
--rw-r--r--   0 greent7    (502) staff       (20)     1800 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/mm_channel.py
--rw-r--r--   0 greent7    (502) staff       (20)    12799 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/packet.py
--rw-r--r--   0 greent7    (502) staff       (20)     5859 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/system_channel.py
--rw-r--r--   0 greent7    (502) staff       (20)     2296 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/ws_client.py
--rw-r--r--   0 greent7    (502) staff       (20)     2967 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipc/ws_factory.py
--rw-r--r--   0 greent7    (502) staff       (20)     7278 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/ipcc.py
--rw-r--r--   0 greent7    (502) staff       (20)     7600 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/pwr.py
--rw-r--r--   0 greent7    (502) staff       (20)    39824 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/devices/stm32wb55/rcc.py
--rw-r--r--   0 greent7    (502) staff       (20)      752 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/dump_stats.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.763822 psdb-1.1.2/psdb/elf/
--rw-r--r--   0 greent7    (502) staff       (20)      211 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/elf/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     5919 2022-07-25 08:13:33.000000 psdb-1.1.2/psdb/elf/core.py
--rw-r--r--   0 greent7    (502) staff       (20)     2023 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/elf/dv.py
--rw-r--r--   0 greent7    (502) staff       (20)     2080 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/elf/elf_binary.py
--rw-r--r--   0 greent7    (502) staff       (20)      159 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/elf/mmap.py
--rw-r--r--   0 greent7    (502) staff       (20)     2767 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/elf/note.py
--rw-r--r--   0 greent7    (502) staff       (20)      149 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/exception.py
--rwxr-xr-x   0 greent7    (502) staff       (20)     6517 2023-03-02 04:47:57.000000 psdb-1.1.2/psdb/flash_tool.py
--rw-r--r--   0 greent7    (502) staff       (20)     3748 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/fus_tool.py
--rwxr-xr-x   0 greent7    (502) staff       (20)    13910 2023-03-02 04:34:42.000000 psdb-1.1.2/psdb/gdb_tool.py
--rw-r--r--   0 greent7    (502) staff       (20)      327 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/hexdump.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.764060 psdb-1.1.2/psdb/hexfile/
--rw-r--r--   0 greent7    (502) staff       (20)      123 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/hexfile/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     2738 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/hexfile/hexfile.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.764881 psdb-1.1.2/psdb/inspect_tool/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2022-02-10 10:00:14.000000 psdb-1.1.2/psdb/inspect_tool/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1063 2022-02-10 10:00:14.000000 psdb-1.1.2/psdb/inspect_tool/cpu_register_window.py
--rw-r--r--   0 greent7    (502) staff       (20)     6951 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/inspect_tool/device_decode_window.py
--rw-r--r--   0 greent7    (502) staff       (20)     7007 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/inspect_tool/device_register_window.py
--rw-r--r--   0 greent7    (502) staff       (20)     1422 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/inspect_tool/device_selector_window.py
--rwxr-xr-x   0 greent7    (502) staff       (20)     7079 2023-09-29 22:54:27.000000 psdb-1.1.2/psdb/inspect_tool/inspect_tool.py
--rw-r--r--   0 greent7    (502) staff       (20)     2853 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/inspect_tool/memory_window.py
--rw-r--r--   0 greent7    (502) staff       (20)     6855 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/mem_ap_test.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.765228 psdb-1.1.2/psdb/probes/
--rw-r--r--   0 greent7    (502) staff       (20)      865 2023-03-02 04:38:57.000000 psdb-1.1.2/psdb/probes/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)    10128 2023-03-02 04:43:51.000000 psdb-1.1.2/psdb/probes/probe.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.765962 psdb-1.1.2/psdb/probes/stlink/
--rw-r--r--   0 greent7    (502) staff       (20)      686 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/probes/stlink/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)    52494 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/probes/stlink/cdb.py
--rw-r--r--   0 greent7    (502) staff       (20)     2027 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/probes/stlink/errors.py
--rw-r--r--   0 greent7    (502) staff       (20)    10734 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/probes/stlink/stlink.py
--rw-r--r--   0 greent7    (502) staff       (20)     3674 2023-02-19 02:03:20.000000 psdb-1.1.2/psdb/probes/stlink/stlink_v2_1.py
--rw-r--r--   0 greent7    (502) staff       (20)     5520 2023-02-19 02:03:20.000000 psdb-1.1.2/psdb/probes/stlink/stlink_v3.py
--rw-r--r--   0 greent7    (502) staff       (20)     3191 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/probes/usb_probe.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.766217 psdb-1.1.2/psdb/probes/xds110/
--rw-r--r--   0 greent7    (502) staff       (20)      398 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/probes/xds110/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)    16846 2023-02-19 02:03:20.000000 psdb-1.1.2/psdb/probes/xds110/xds110.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.766859 psdb-1.1.2/psdb/probes/xtswd/
--rw-r--r--   0 greent7    (502) staff       (20)      359 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/probes/xtswd/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     4383 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/probes/xtswd/abort_test.py
--rw-r--r--   0 greent7    (502) staff       (20)     2640 2023-02-14 21:49:24.000000 psdb-1.1.2/psdb/probes/xtswd/imon.py
--rw-r--r--   0 greent7    (502) staff       (20)     2698 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/probes/xtswd/plot_imon.py
--rw-r--r--   0 greent7    (502) staff       (20)     3870 2023-09-29 23:13:01.000000 psdb-1.1.2/psdb/probes/xtswd/plot_imon_realtime.py
--rw-r--r--   0 greent7    (502) staff       (20)    11468 2023-09-29 23:13:01.000000 psdb-1.1.2/psdb/probes/xtswd/xtswd.py
--rw-r--r--   0 greent7    (502) staff       (20)     2596 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/reg_dump_tool.py
--rwxr-xr-x   0 greent7    (502) staff       (20)      874 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/scan_tool.py
--rw-r--r--   0 greent7    (502) staff       (20)      925 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/srst_tool.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.767085 psdb-1.1.2/psdb/targets/
--rw-r--r--   0 greent7    (502) staff       (20)      728 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/targets/__init__.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.767274 psdb-1.1.2/psdb/targets/msp432/
--rw-r--r--   0 greent7    (502) staff       (20)      120 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/targets/msp432/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     2744 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/targets/msp432/msp432.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.767480 psdb-1.1.2/psdb/targets/stm32g0/
--rw-r--r--   0 greent7    (502) staff       (20)      110 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/targets/stm32g0/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     2625 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/targets/stm32g0/stm32g0.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.767776 psdb-1.1.2/psdb/targets/stm32g4/
--rw-r--r--   0 greent7    (502) staff       (20)      110 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/targets/stm32g4/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      362 2021-12-02 06:31:30.000000 psdb-1.1.2/psdb/targets/stm32g4/dbgmcu.py
--rw-r--r--   0 greent7    (502) staff       (20)    13837 2023-02-19 02:03:20.000000 psdb-1.1.2/psdb/targets/stm32g4/stm32g4.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.768151 psdb-1.1.2/psdb/targets/stm32h7/
--rw-r--r--   0 greent7    (502) staff       (20)      170 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/targets/stm32h7/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      572 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/targets/stm32h7/dbgmcu.py
--rw-r--r--   0 greent7    (502) staff       (20)     4207 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/targets/stm32h7/stm32h7.py
--rw-r--r--   0 greent7    (502) staff       (20)    13032 2023-02-14 21:50:59.000000 psdb-1.1.2/psdb/targets/stm32h7/stm32h7_dp.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.768439 psdb-1.1.2/psdb/targets/stm32u5/
--rw-r--r--   0 greent7    (502) staff       (20)      113 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/targets/stm32u5/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      367 2022-07-23 01:30:10.000000 psdb-1.1.2/psdb/targets/stm32u5/dbgmcu.py
--rw-r--r--   0 greent7    (502) staff       (20)     5823 2023-12-12 01:09:19.000000 psdb-1.1.2/psdb/targets/stm32u5/stm32u5.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.768633 psdb-1.1.2/psdb/targets/stm32wb55/
--rw-r--r--   0 greent7    (502) staff       (20)      116 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/targets/stm32wb55/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     6651 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/targets/stm32wb55/stm32wb55.py
--rw-r--r--   0 greent7    (502) staff       (20)     3751 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/targets/target.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.768918 psdb-1.1.2/psdb/util/
--rw-r--r--   0 greent7    (502) staff       (20)      289 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/util/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      123 2021-11-05 03:30:42.000000 psdb-1.1.2/psdb/util/hexify.py
--rw-r--r--   0 greent7    (502) staff       (20)     1339 2022-07-23 01:32:30.000000 psdb-1.1.2/psdb/util/prange.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-12-12 01:11:05.769072 psdb-1.1.2/psdb.egg-info/
--rw-r--r--   0 greent7    (502) staff       (20)     8117 2023-12-12 01:11:05.000000 psdb-1.1.2/psdb.egg-info/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     5324 2023-12-12 01:11:05.000000 psdb-1.1.2/psdb.egg-info/SOURCES.txt
--rw-r--r--   0 greent7    (502) staff       (20)        1 2023-12-12 01:11:05.000000 psdb-1.1.2/psdb.egg-info/dependency_links.txt
--rw-r--r--   0 greent7    (502) staff       (20)      501 2023-12-12 01:11:05.000000 psdb-1.1.2/psdb.egg-info/entry_points.txt
--rw-r--r--   0 greent7    (502) staff       (20)       46 2023-12-12 01:11:05.000000 psdb-1.1.2/psdb.egg-info/requires.txt
--rw-r--r--   0 greent7    (502) staff       (20)        5 2023-12-12 01:11:05.000000 psdb-1.1.2/psdb.egg-info/top_level.txt
--rw-r--r--   0 greent7    (502) staff       (20)       85 2022-07-23 01:32:30.000000 psdb-1.1.2/pyproject.toml
--rw-r--r--   0 greent7    (502) staff       (20)     1767 2023-12-12 01:11:05.769753 psdb-1.1.2/setup.cfg
--rw-r--r--   0 greent7    (502) staff       (20)       38 2021-11-05 03:30:42.000000 psdb-1.1.2/setup.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.297059 psdb-1.1.3/
+-rw-r--r--   0 greent7    (502) staff       (20)    26526 2021-11-05 03:30:42.000000 psdb-1.1.3/LICENSE
+-rw-r--r--   0 greent7    (502) staff       (20)     8117 2024-04-09 21:18:54.296981 psdb-1.1.3/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     7465 2021-11-05 03:30:42.000000 psdb-1.1.3/README.rst
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.270892 psdb-1.1.3/psdb/
+-rw-r--r--   0 greent7    (502) staff       (20)      493 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     6131 2024-04-03 05:29:48.000000 psdb-1.1.3/psdb/access_port.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7531 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/ble_tool.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.272075 psdb-1.1.3/psdb/block/
+-rw-r--r--   0 greent7    (502) staff       (20)      229 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/block/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      860 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/block/bd.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1262 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/block/rambd.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.272481 psdb-1.1.3/psdb/component/
+-rw-r--r--   0 greent7    (502) staff       (20)      265 2022-07-23 01:30:10.000000 psdb-1.1.3/psdb/component/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4737 2024-04-03 05:29:53.000000 psdb-1.1.3/psdb/component/component.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2262 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/component/matcher.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1809 2023-02-19 02:03:20.000000 psdb-1.1.3/psdb/cordic_test.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3070 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/core_tool.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.273610 psdb-1.1.3/psdb/cpus/
+-rw-r--r--   0 greent7    (502) staff       (20)     2321 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/cpus/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3729 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/cpus/cortex.py
+-rw-r--r--   0 greent7    (502) staff       (20)      213 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/cpus/cortex_m0p.py
+-rw-r--r--   0 greent7    (502) staff       (20)      211 2022-07-23 01:30:10.000000 psdb-1.1.3/psdb/cpus/cortex_m33.py
+-rw-r--r--   0 greent7    (502) staff       (20)      211 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/cpus/cortex_m4.py
+-rw-r--r--   0 greent7    (502) staff       (20)      211 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/cpus/cortex_m7.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.274054 psdb-1.1.3/psdb/devices/
+-rw-r--r--   0 greent7    (502) staff       (20)      760 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/__init__.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.275806 psdb-1.1.3/psdb/devices/core/
+-rw-r--r--   0 greent7    (502) staff       (20)     1898 2024-02-21 05:47:51.000000 psdb-1.1.3/psdb/devices/core/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2140 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/core/bpu.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2430 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/core/coresight_0x9.py
+-rw-r--r--   0 greent7    (502) staff       (20)      631 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/devices/core/cortex_subdevice.py
+-rw-r--r--   0 greent7    (502) staff       (20)     6013 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/core/dwt_m4.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3775 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/core/fpb.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5703 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/core/itm_m4.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3003 2024-04-03 05:30:20.000000 psdb-1.1.3/psdb/devices/core/scs_base.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5837 2024-04-03 05:30:30.000000 psdb-1.1.3/psdb/devices/core/scs_v6_m.py
+-rw-r--r--   0 greent7    (502) staff       (20)    12220 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/core/scs_v7_m.py
+-rw-r--r--   0 greent7    (502) staff       (20)    20529 2024-03-22 23:54:54.000000 psdb-1.1.3/psdb/devices/core/scs_v8_m.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3885 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/core/tpiu_m4.py
+-rw-r--r--   0 greent7    (502) staff       (20)     9842 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/device.py
+-rw-r--r--   0 greent7    (502) staff       (20)     6805 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/flash.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.276104 psdb-1.1.3/psdb/devices/msp432/
+-rw-r--r--   0 greent7    (502) staff       (20)      117 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/devices/msp432/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)    17844 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/msp432/flctl.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.279700 psdb-1.1.3/psdb/devices/stm32/
+-rw-r--r--   0 greent7    (502) staff       (20)     1274 2024-04-03 04:10:09.000000 psdb-1.1.3/psdb/devices/stm32/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)    16310 2024-03-22 23:54:54.000000 psdb-1.1.3/psdb/devices/stm32/adc.py
+-rw-r--r--   0 greent7    (502) staff       (20)    10382 2024-03-22 23:54:54.000000 psdb-1.1.3/psdb/devices/stm32/adc_12.py
+-rw-r--r--   0 greent7    (502) staff       (20)    14259 2024-03-22 23:54:54.000000 psdb-1.1.3/psdb/devices/stm32/adc_14.py
+-rw-r--r--   0 greent7    (502) staff       (20)    16199 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/adc_16.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1379 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/advanced_control_timer.py
+-rw-r--r--   0 greent7    (502) staff       (20)      663 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/basic_timer.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1273 2023-02-19 02:03:20.000000 psdb-1.1.3/psdb/devices/stm32/cordic.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2087 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/devices/stm32/crs.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4605 2024-02-20 23:13:05.000000 psdb-1.1.3/psdb/devices/stm32/dac.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5710 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/dma.py
+-rw-r--r--   0 greent7    (502) staff       (20)      659 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/dma_mux.py
+-rw-r--r--   0 greent7    (502) staff       (20)     9499 2024-04-09 20:26:48.000000 psdb-1.1.3/psdb/devices/stm32/flash_type1.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7927 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/general_purpose_timer_16x1.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1189 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/general_purpose_timer_16x2.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1227 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/general_purpose_timer_16x4.py
+-rw-r--r--   0 greent7    (502) staff       (20)     9751 2023-02-14 21:53:36.000000 psdb-1.1.3/psdb/devices/stm32/general_purpose_timer_32.py
+-rw-r--r--   0 greent7    (502) staff       (20)      995 2023-02-14 21:53:41.000000 psdb-1.1.3/psdb/devices/stm32/gpdma.py
+-rw-r--r--   0 greent7    (502) staff       (20)    11305 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/gpio.py
+-rw-r--r--   0 greent7    (502) staff       (20)     9200 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/lpuart.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4055 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/qspi.py
+-rw-r--r--   0 greent7    (502) staff       (20)     8373 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/usb.py
+-rw-r--r--   0 greent7    (502) staff       (20)    62011 2021-11-26 09:53:24.000000 psdb-1.1.3/psdb/devices/stm32/usb_hs.py
+-rw-r--r--   0 greent7    (502) staff       (20)      708 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32/vrefbuf.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.280123 psdb-1.1.3/psdb/devices/stm32c0/
+-rw-r--r--   0 greent7    (502) staff       (20)      117 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/devices/stm32c0/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5603 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/devices/stm32c0/flash.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.280379 psdb-1.1.3/psdb/devices/stm32g0/
+-rw-r--r--   0 greent7    (502) staff       (20)      117 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/devices/stm32g0/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4907 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32g0/flash.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.282140 psdb-1.1.3/psdb/devices/stm32g4/
+-rw-r--r--   0 greent7    (502) staff       (20)      578 2022-07-23 01:30:10.000000 psdb-1.1.3/psdb/devices/stm32g4/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      564 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32g4/comparator.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3048 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32g4/dbgmcu.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4386 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32g4/flash_2.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7799 2022-07-23 01:35:42.000000 psdb-1.1.3/psdb/devices/stm32g4/flash_3.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4450 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32g4/flash_4.py
+-rw-r--r--   0 greent7    (502) staff       (20)      732 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32g4/opamp.py
+-rw-r--r--   0 greent7    (502) staff       (20)    18411 2023-02-19 02:03:20.000000 psdb-1.1.3/psdb/devices/stm32g4/pwr.py
+-rw-r--r--   0 greent7    (502) staff       (20)    26502 2024-02-20 23:13:05.000000 psdb-1.1.3/psdb/devices/stm32g4/rcc.py
+-rw-r--r--   0 greent7    (502) staff       (20)    11684 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32g4/rtc.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4862 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32g4/syscfg.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5060 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32g4/tamp.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.284103 psdb-1.1.3/psdb/devices/stm32h7/
+-rw-r--r--   0 greent7    (502) staff       (20)      602 2023-02-14 21:49:51.000000 psdb-1.1.3/psdb/devices/stm32h7/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      539 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/devices/stm32h7/art.py
+-rw-r--r--   0 greent7    (502) staff       (20)    10859 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32h7/flash.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7152 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32h7/flash_dp.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1325 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32h7/flash_up.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2777 2023-02-14 21:49:43.000000 psdb-1.1.3/psdb/devices/stm32h7/opamp.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7767 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32h7/pwr.py
+-rw-r--r--   0 greent7    (502) staff       (20)   107742 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32h7/rcc.py
+-rw-r--r--   0 greent7    (502) staff       (20)     8613 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32h7/syscfg.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1050 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32h7/tim15.py
+-rw-r--r--   0 greent7    (502) staff       (20)     6348 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32h7/tim17.py
+-rw-r--r--   0 greent7    (502) staff       (20)     8952 2023-02-14 21:50:27.000000 psdb-1.1.3/psdb/devices/stm32h7/tim2_5.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1847 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32h7/tim6.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.284382 psdb-1.1.3/psdb/devices/stm32l4/
+-rw-r--r--   0 greent7    (502) staff       (20)      117 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/devices/stm32l4/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4955 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/devices/stm32l4/flash.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.285491 psdb-1.1.3/psdb/devices/stm32u5/
+-rw-r--r--   0 greent7    (502) staff       (20)      324 2024-02-20 23:13:15.000000 psdb-1.1.3/psdb/devices/stm32u5/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4236 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32u5/dbgmcu.py
+-rw-r--r--   0 greent7    (502) staff       (20)    21891 2023-03-02 05:49:54.000000 psdb-1.1.3/psdb/devices/stm32u5/flash.py
+-rw-r--r--   0 greent7    (502) staff       (20)     6342 2024-04-03 04:10:09.000000 psdb-1.1.3/psdb/devices/stm32u5/i2c.py
+-rw-r--r--   0 greent7    (502) staff       (20)    28925 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32u5/pwr.py
+-rw-r--r--   0 greent7    (502) staff       (20)    38490 2023-09-29 22:54:27.000000 psdb-1.1.3/psdb/devices/stm32u5/rcc.py
+-rw-r--r--   0 greent7    (502) staff       (20)    12083 2024-03-22 23:54:54.000000 psdb-1.1.3/psdb/devices/stm32u5/rtc.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.286227 psdb-1.1.3/psdb/devices/stm32wb55/
+-rw-r--r--   0 greent7    (502) staff       (20)      237 2024-04-03 03:41:01.000000 psdb-1.1.3/psdb/devices/stm32wb55/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)    14327 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/flash.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.288427 psdb-1.1.3/psdb/devices/stm32wb55/ipc/
+-rw-r--r--   0 greent7    (502) staff       (20)     2502 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7156 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/binaries.py
+-rw-r--r--   0 greent7    (502) staff       (20)    23377 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/ble_channel.py
+-rw-r--r--   0 greent7    (502) staff       (20)      130 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/ble_client.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3718 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/circular_queue.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7214 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/fus_client.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1139 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/gatt.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4117 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/ipc.py
+-rw-r--r--   0 greent7    (502) staff       (20)    10378 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/mailbox.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1800 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/mm_channel.py
+-rw-r--r--   0 greent7    (502) staff       (20)    12799 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/packet.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5859 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/system_channel.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2296 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/ws_client.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2967 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipc/ws_factory.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7278 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/ipcc.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7600 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/pwr.py
+-rw-r--r--   0 greent7    (502) staff       (20)    39824 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/devices/stm32wb55/rcc.py
+-rw-r--r--   0 greent7    (502) staff       (20)      752 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/dump_stats.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.289253 psdb-1.1.3/psdb/elf/
+-rw-r--r--   0 greent7    (502) staff       (20)      211 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/elf/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5919 2022-07-25 08:13:33.000000 psdb-1.1.3/psdb/elf/core.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2023 2022-07-23 01:30:10.000000 psdb-1.1.3/psdb/elf/dv.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2080 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/elf/elf_binary.py
+-rw-r--r--   0 greent7    (502) staff       (20)      159 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/elf/mmap.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2767 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/elf/note.py
+-rw-r--r--   0 greent7    (502) staff       (20)      149 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/exception.py
+-rwxr-xr-x   0 greent7    (502) staff       (20)     6517 2023-03-02 04:47:57.000000 psdb-1.1.3/psdb/flash_tool.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3748 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/fus_tool.py
+-rwxr-xr-x   0 greent7    (502) staff       (20)    13910 2023-03-02 04:34:42.000000 psdb-1.1.3/psdb/gdb_tool.py
+-rw-r--r--   0 greent7    (502) staff       (20)      327 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/hexdump.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.289538 psdb-1.1.3/psdb/hexfile/
+-rw-r--r--   0 greent7    (502) staff       (20)      123 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/hexfile/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2738 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/hexfile/hexfile.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.290441 psdb-1.1.3/psdb/inspect_tool/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2022-02-10 10:00:14.000000 psdb-1.1.3/psdb/inspect_tool/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1063 2022-02-10 10:00:14.000000 psdb-1.1.3/psdb/inspect_tool/cpu_register_window.py
+-rw-r--r--   0 greent7    (502) staff       (20)     6951 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/inspect_tool/device_decode_window.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7007 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/inspect_tool/device_register_window.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1422 2022-07-23 01:30:10.000000 psdb-1.1.3/psdb/inspect_tool/device_selector_window.py
+-rwxr-xr-x   0 greent7    (502) staff       (20)     7079 2023-09-29 22:54:27.000000 psdb-1.1.3/psdb/inspect_tool/inspect_tool.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2853 2022-07-23 01:30:10.000000 psdb-1.1.3/psdb/inspect_tool/memory_window.py
+-rw-r--r--   0 greent7    (502) staff       (20)     6855 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/mem_ap_test.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.290825 psdb-1.1.3/psdb/probes/
+-rw-r--r--   0 greent7    (502) staff       (20)      865 2023-03-02 04:38:57.000000 psdb-1.1.3/psdb/probes/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)    10128 2024-04-03 05:28:20.000000 psdb-1.1.3/psdb/probes/probe.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.291586 psdb-1.1.3/psdb/probes/stlink/
+-rw-r--r--   0 greent7    (502) staff       (20)      686 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/probes/stlink/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)    52494 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/probes/stlink/cdb.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2027 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/probes/stlink/errors.py
+-rw-r--r--   0 greent7    (502) staff       (20)    10734 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/probes/stlink/stlink.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3674 2023-02-19 02:03:20.000000 psdb-1.1.3/psdb/probes/stlink/stlink_v2_1.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5520 2023-02-19 02:03:20.000000 psdb-1.1.3/psdb/probes/stlink/stlink_v3.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3191 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/probes/usb_probe.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.291851 psdb-1.1.3/psdb/probes/xds110/
+-rw-r--r--   0 greent7    (502) staff       (20)      398 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/probes/xds110/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)    16846 2023-02-19 02:03:20.000000 psdb-1.1.3/psdb/probes/xds110/xds110.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.292590 psdb-1.1.3/psdb/probes/xtswd/
+-rw-r--r--   0 greent7    (502) staff       (20)      359 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/probes/xtswd/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4383 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/probes/xtswd/abort_test.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4423 2024-03-22 23:54:54.000000 psdb-1.1.3/psdb/probes/xtswd/gl_plot_imon_realtime.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2640 2023-02-14 21:49:24.000000 psdb-1.1.3/psdb/probes/xtswd/imon.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2698 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/probes/xtswd/plot_imon.py
+-rw-r--r--   0 greent7    (502) staff       (20)    11913 2024-03-22 23:54:54.000000 psdb-1.1.3/psdb/probes/xtswd/xtswd.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2648 2024-03-22 23:54:54.000000 psdb-1.1.3/psdb/reg_dump_tool.py
+-rwxr-xr-x   0 greent7    (502) staff       (20)      874 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/scan_tool.py
+-rw-r--r--   0 greent7    (502) staff       (20)      925 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/srst_tool.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.292842 psdb-1.1.3/psdb/targets/
+-rw-r--r--   0 greent7    (502) staff       (20)      828 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/__init__.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.293093 psdb-1.1.3/psdb/targets/msp432/
+-rw-r--r--   0 greent7    (502) staff       (20)      120 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/targets/msp432/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2744 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/targets/msp432/msp432.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.293469 psdb-1.1.3/psdb/targets/stm32c0/
+-rw-r--r--   0 greent7    (502) staff       (20)      110 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32c0/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      362 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32c0/dbgmcu.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2847 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32c0/stm32c0.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.293904 psdb-1.1.3/psdb/targets/stm32g0/
+-rw-r--r--   0 greent7    (502) staff       (20)      110 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/targets/stm32g0/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      362 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32g0/dbgmcu.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3488 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32g0/stm32g0.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.294261 psdb-1.1.3/psdb/targets/stm32g4/
+-rw-r--r--   0 greent7    (502) staff       (20)      110 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/targets/stm32g4/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      362 2021-12-02 06:31:30.000000 psdb-1.1.3/psdb/targets/stm32g4/dbgmcu.py
+-rw-r--r--   0 greent7    (502) staff       (20)    13837 2024-04-09 20:26:48.000000 psdb-1.1.3/psdb/targets/stm32g4/stm32g4.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.294954 psdb-1.1.3/psdb/targets/stm32h7/
+-rw-r--r--   0 greent7    (502) staff       (20)      170 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/targets/stm32h7/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      572 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/targets/stm32h7/dbgmcu.py
+-rw-r--r--   0 greent7    (502) staff       (20)     4207 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/targets/stm32h7/stm32h7.py
+-rw-r--r--   0 greent7    (502) staff       (20)    13032 2023-02-14 21:50:59.000000 psdb-1.1.3/psdb/targets/stm32h7/stm32h7_dp.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.295380 psdb-1.1.3/psdb/targets/stm32l4/
+-rw-r--r--   0 greent7    (502) staff       (20)      110 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32l4/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      362 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32l4/dbgmcu.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3017 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32l4/stm32l4.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.295770 psdb-1.1.3/psdb/targets/stm32u5/
+-rw-r--r--   0 greent7    (502) staff       (20)      113 2022-07-23 01:30:10.000000 psdb-1.1.3/psdb/targets/stm32u5/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      367 2022-07-23 01:30:10.000000 psdb-1.1.3/psdb/targets/stm32u5/dbgmcu.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5886 2024-03-22 23:54:54.000000 psdb-1.1.3/psdb/targets/stm32u5/stm32u5.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.296136 psdb-1.1.3/psdb/targets/stm32wb55/
+-rw-r--r--   0 greent7    (502) staff       (20)      116 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/targets/stm32wb55/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      362 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32wb55/dbgmcu.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7630 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/stm32wb55/stm32wb55.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3861 2024-04-09 21:18:33.000000 psdb-1.1.3/psdb/targets/target.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.296519 psdb-1.1.3/psdb/util/
+-rw-r--r--   0 greent7    (502) staff       (20)      289 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/util/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      123 2021-11-05 03:30:42.000000 psdb-1.1.3/psdb/util/hexify.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1339 2022-07-23 01:32:30.000000 psdb-1.1.3/psdb/util/prange.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-04-09 21:18:54.296710 psdb-1.1.3/psdb.egg-info/
+-rw-r--r--   0 greent7    (502) staff       (20)     8117 2024-04-09 21:18:54.000000 psdb-1.1.3/psdb.egg-info/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     5738 2024-04-09 21:18:54.000000 psdb-1.1.3/psdb.egg-info/SOURCES.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        1 2024-04-09 21:18:54.000000 psdb-1.1.3/psdb.egg-info/dependency_links.txt
+-rw-r--r--   0 greent7    (502) staff       (20)      501 2024-04-09 21:18:54.000000 psdb-1.1.3/psdb.egg-info/entry_points.txt
+-rw-r--r--   0 greent7    (502) staff       (20)       46 2024-04-09 21:18:54.000000 psdb-1.1.3/psdb.egg-info/requires.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        5 2024-04-09 21:18:54.000000 psdb-1.1.3/psdb.egg-info/top_level.txt
+-rw-r--r--   0 greent7    (502) staff       (20)       85 2022-07-23 01:32:30.000000 psdb-1.1.3/pyproject.toml
+-rw-r--r--   0 greent7    (502) staff       (20)     1855 2024-04-09 21:18:54.297397 psdb-1.1.3/setup.cfg
+-rw-r--r--   0 greent7    (502) staff       (20)       38 2021-11-05 03:30:42.000000 psdb-1.1.3/setup.py
```

### Comparing `psdb-1.1.2/LICENSE` & `psdb-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/PKG-INFO` & `psdb-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdb
-Version: 1.1.2
+Version: 1.1.3
 Summary: Package for interfacing with ARM-compatible debug probes
 Home-page: https://github.com/tgree/psdb
 Author: Terry Greeniaus
 Author-email: terrygreeniaus@gmail.com
 License: LGPLv2
 Keywords: stlink xds110 arm swd fus stm32 msp432
 Classifier: Operating System :: OS Independent
```

### Comparing `psdb-1.1.2/README.rst` & `psdb-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/access_port.py` & `psdb-1.1.3/psdb/access_port.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/ble_tool.py` & `psdb-1.1.3/psdb/ble_tool.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/block/bd.py` & `psdb-1.1.3/psdb/block/bd.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/block/rambd.py` & `psdb-1.1.3/psdb/block/rambd.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/component/component.py` & `psdb-1.1.3/psdb/component/component.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/component/matcher.py` & `psdb-1.1.3/psdb/component/matcher.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/cordic_test.py` & `psdb-1.1.3/psdb/cordic_test.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/core_tool.py` & `psdb-1.1.3/psdb/core_tool.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/cpus/__init__.py` & `psdb-1.1.3/psdb/cpus/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 # It's common practice for third-party vendors to put their own identifying
 # information in the top-level Cortex ROM Table.  It's implied that this is
 # normal in the Cortex-M4 spec, although the Cortex-M7 spec is silent about it.
 psdb.component.StaticMatcher(cortex_m4.CortexM4, 0, 0xE00FF000, 0xB105100D,
                              0x000000000B1979AF,
                              subtype='MSP432P401R Cortex-M4')
 psdb.component.StaticMatcher(cortex_m0p.CortexM0P, 0, 0xF0000000, 0xB105100D,
+                             0x00000000000A0466, subtype='STM32C0 Cortex-M0+')
+psdb.component.StaticMatcher(cortex_m0p.CortexM0P, 0, 0xF0000000, 0xB105100D,
                              0x00000000000A0460, subtype='STM32G0 Cortex-M0+')
 psdb.component.StaticMatcher(cortex_m4.CortexM4, 0, 0xE00FF000, 0xB105100D,
+                             0x00000000000A0464, subtype='STM32L4 Cortex-M4')
+psdb.component.StaticMatcher(cortex_m4.CortexM4, 0, 0xE00FF000, 0xB105100D,
                              0x00000000000A0468, subtype='STM32G4 Cortex-M4')
 psdb.component.StaticMatcher(cortex_m4.CortexM4, 0, 0xE00FF000, 0xB105100D,
                              0x00000000000A0469, subtype='STM32G4 Cortex-M4')
 psdb.component.StaticMatcher(cortex_m4.CortexM4, 0, 0xE00FF000, 0xB105100D,
                              0x00000000000A0479, subtype='STM32G4 Cortex-M4')
 psdb.component.StaticMatcher(cortex_m7.CortexM7, 0, 0xE00FE000, 0xB105100D,
                              0x00000000000A0450, subtype='STM32H7 Cortex-M7')
```

### Comparing `psdb-1.1.2/psdb/cpus/cortex.py` & `psdb-1.1.3/psdb/cpus/cortex.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/__init__.py` & `psdb-1.1.3/psdb/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/__init__.py` & `psdb-1.1.3/psdb/devices/core/__init__.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/bpu.py` & `psdb-1.1.3/psdb/devices/core/bpu.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/coresight_0x9.py` & `psdb-1.1.3/psdb/devices/core/coresight_0x9.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/cortex_subdevice.py` & `psdb-1.1.3/psdb/devices/core/cortex_subdevice.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/dwt_m4.py` & `psdb-1.1.3/psdb/devices/core/dwt_m4.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/fpb.py` & `psdb-1.1.3/psdb/devices/core/fpb.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/itm_m4.py` & `psdb-1.1.3/psdb/devices/core/itm_m4.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/scs_base.py` & `psdb-1.1.3/psdb/devices/core/scs_base.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/scs_v6_m.py` & `psdb-1.1.3/psdb/devices/core/scs_v6_m.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/scs_v7_m.py` & `psdb-1.1.3/psdb/devices/core/scs_v7_m.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/core/scs_v8_m.py` & `psdb-1.1.3/psdb/devices/stm32/adc_16.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,305 +1,243 @@
 # Copyright (c) 2019-2021 Phase Advanced Sensor Systems, Inc.
-import collections
+from builtins import range
 
-from psdb.devices import AReg32, AReg32R, AReg32W
-from . import scs_base
+from ..device import Device, AReg32, AReg32R
 
 
-# The core registers and the selector value they map to in the DCRSR.
-CORE_REGISTERS = collections.OrderedDict([
-    ('r0',      0),
-    ('r1',      1),
-    ('r2',      2),
-    ('r3',      3),
-    ('r4',      4),
-    ('r5',      5),
-    ('r6',      6),
-    ('r7',      7),
-    ('r8',      8),
-    ('r9',      9),
-    ('r10',     10),
-    ('r11',     11),
-    ('r12',     12),
-    ('sp',      13),
-    ('lr',      14),
-    ('pc',      15),
-    ('xpsr',    16),
-    ('msp',     17),
-    ('psp',     18),
-    ('cfbp',    20),   # CONTROL, FAULTMASK, BASEPRI, PRIMASK
-    ('fpscr',   33),
-    ('s0',      64),
-    ('s1',      65),
-    ('s2',      66),
-    ('s3',      67),
-    ('s4',      68),
-    ('s5',      69),
-    ('s6',      70),
-    ('s7',      71),
-    ('s8',      72),
-    ('s9',      73),
-    ('s10',     74),
-    ('s11',     75),
-    ('s12',     76),
-    ('s13',     77),
-    ('s14',     78),
-    ('s15',     79),
-    ('s16',     80),
-    ('s17',     81),
-    ('s18',     82),
-    ('s19',     83),
-    ('s20',     84),
-    ('s21',     85),
-    ('s22',     86),
-    ('s23',     87),
-    ('s24',     88),
-    ('s25',     89),
-    ('s26',     90),
-    ('s27',     91),
-    ('s28',     92),
-    ('s29',     93),
-    ('s30',     94),
-    ('s31',     95),
-])
-
-
-class SCS(scs_base.SCS):
+class ADC16(Device):
     '''
-    Driver for Cortex V8-M (M33) System Control Space.
+    Driver for the STM32H7 16-bit ADC.
     '''
-    REGS = [AReg32R('ICTR',         0x004, [('INTLINESNUM',         0,  3),
-                                            ]),
-            AReg32('ACTLR',         0x008),
-            AReg32('CPPWR',         0x00C, [('SU0',                 0),
-                                            ('SUS0',                1),
-                                            ('SU1',                 2),
-                                            ('SUS1',                3),
-                                            ('SU2',                 4),
-                                            ('SUS2',                5),
-                                            ('SU3',                 6),
-                                            ('SUS3',                7),
-                                            ('SU4',                 8),
-                                            ('SUS4',                9),
-                                            ('SU5',                 10),
-                                            ('SUS5',                11),
-                                            ('SU6',                 12),
-                                            ('SUS6',                13),
-                                            ('SU7',                 14),
-                                            ('SUS7',                15),
-                                            ('SU10',                20),
-                                            ('SUS10',               21),
-                                            ('SU11',                22),
-                                            ('SUS11',               23),
-                                            ]),
-            AReg32('SYST_CSR',      0x010, [('ENABLE',              0),
-                                            ('TICKINT',             1),
-                                            ('CLKSOURCE',           2),
-                                            ('COUNTFLAG',           16),
-                                            ]),
-            AReg32('SYST_RVR',      0x014, [('RELOAD',              0,  23),
-                                            ]),
-            AReg32('SYST_CVR',      0x018, [('CURRENT',             0,  23),
-                                            ]),
-            AReg32('SYST_CALIB',    0x01C, [('TENMS',               0,  23),
-                                            ('SKEW',                30),
-                                            ('NOREF',               31),
-                                            ]),
-            AReg32R('REVIDR',       0xCFC),
-            AReg32R('CPUID',        0xD00, [('REVISION',            0,  3),
-                                            ('PARTNO',              4,  15),
-                                            ('ARCHITECTURE',        16, 19),
-                                            ('VARIANT',             20, 23),
-                                            ('IMPLEMENTER',         24, 31),
-                                            ]),
-            AReg32('ICSR',          0xD04, [('VECTACTIVE',          0,  8),
-                                            ('RETTOBASE',           11),
-                                            ('VECTPENDING',         12, 20),
-                                            ('ISRPENDING',          22),
-                                            ('ISRPREEMPT',          23),
-                                            ('STTNS',               24),
-                                            ('PENDSTCLR',           25),
-                                            ('PENDSTSET',           26),
-                                            ('PENDSVCLR',           27),
-                                            ('PENDSVSET',           28),
-                                            ('PENDNMICLR',          30),
-                                            ('PENDNMISET',          31),
-                                            ]),
-            AReg32('VTOR',          0xD08, [('TBLOFF',              7,  31),
-                                            ]),
-            AReg32('AIRCR',         0xD0C, [('VECTCLRACTIVE',       1),
-                                            ('SYSRESETREQ',         2),
-                                            ('SYSRESETREQS',        3),
-                                            ('DIT',                 4),
-                                            ('IESB',                5),
-                                            ('PRIGROUP',            8,  10),
-                                            ('BFHFNMINS',           13),
-                                            ('PRIS',                14),
-                                            ('ENDIANNESS',          15),
-                                            ('VECTKEYSTAT',         16, 31),
-                                            ]),
-            AReg32('SCR',           0xD10, [('SLEEPONEXIT',         1),
-                                            ('SLEEPDEEP',           2),
-                                            ('SLEEPDEEPS',          3),
-                                            ('SEVONPEND',           4),
-                                            ]),
-            AReg32('CCR',           0xD14, [('USERSETMPEND',        1),
-                                            ('UNALIGN_TRP',         3),
-                                            ('DIV_0_TRP',           4),
-                                            ('BFHFNMIGN',           8),
-                                            ('STKOFHFNMIGN',        10),
-                                            ('DC',                  16),
-                                            ('IC',                  17),
-                                            ('BP',                  18),
-                                            ('LOB',                 19),
-                                            ('TRD',                 20),
-                                            ]),
-            AReg32('SHPR1',         0xD18, [('PRI_4',               0,  7),
-                                            ('PRI_5',               8,  15),
-                                            ('PRI_6',               16, 23),
-                                            ('PRI_7',               24, 31),
-                                            ]),
-            AReg32('SHPR2',         0xD1C, [('PRI_8',               0,  7),
-                                            ('PRI_9',               8,  15),
-                                            ('PRI_10',              16, 23),
-                                            ('PRI_11',              24, 31),
-                                            ]),
-            AReg32('SHPR3',         0xD20, [('PRI_12',              0,  7),
-                                            ('PRI_13',              8,  15),
-                                            ('PRI_14',              16, 23),
-                                            ('PRI_15',              24, 31),
-                                            ]),
-            AReg32('SHCSR',         0xD24, [('MEMFAULTACT',         0),
-                                            ('BUSFAULTACT',         1),
-                                            ('HARDFAULTACT',        2),
-                                            ('USGFAULTACT',         3),
-                                            ('SECUREFAULTACT',      4),
-                                            ('NMIACT',              5),
-                                            ('SVCALLACT',           7),
-                                            ('MONITORACT',          8),
-                                            ('PENDSVACT',           10),
-                                            ('SYSTICKACT',          11),
-                                            ('USGFAULTPENDED',      12),
-                                            ('MEMFAULTPENDED',      13),
-                                            ('BUSFAULTPENDED',      14),
-                                            ('SVCALLPENDED',        15),
-                                            ('MEMFAULTENA',         16),
-                                            ('BUSFAULTENA',         17),
-                                            ('USGFAULTENA',         18),
-                                            ('SECUREFAULTENA',      19),
-                                            ('SECUREFAULTPENDED',   20),
-                                            ('HARDFAULTPENDED',     21),
-                                            ]),
-            AReg32('CFSR',          0xD28, [('IACCVIOL',            0),
-                                            ('DACCVIOL',            1),
-                                            ('MUNSTKERR',           3),
-                                            ('MSTKERR',             4),
-                                            ('MLSPERR',             5),
-                                            ('MMARVALID',           7),
-                                            ('IBUSERR',             8),
-                                            ('PRECISERR',           9),
-                                            ('IMPRECISERR',         10),
-                                            ('UNSTKERR',            11),
-                                            ('STKERR',              12),
-                                            ('LSPERR',              13),
-                                            ('BFARVALID',           15),
-                                            ('UNDEFINSTR',          16),
-                                            ('INVSTATE',            17),
-                                            ('INVPC',               18),
-                                            ('NOCP',                19),
-                                            ('STKOF',               20),
-                                            ('UNALIGNED',           24),
-                                            ('DIVBYZERO',           25),
-                                            ]),
-            AReg32('HFSR',          0xD2C, [('VECTTBL',             1),
-                                            ('FORCED',              30),
-                                            ('DEBUGEVT',            31),
-                                            ]),
-            AReg32('DFSR',          0xD30, [('HALTED',              0),
-                                            ('BKPT',                1),
-                                            ('DWTTRAP',             2),
-                                            ('VCATCH',              3),
-                                            ('EXTERNAL',            4),
-                                            ('PMU',                 5),
-                                            ]),
-            AReg32('MMFAR',         0xD34, [('ADDRESS',             0,  31),
-                                            ]),
-            AReg32('BFAR',          0xD38, [('ADDRESS',             0,  31),
-                                            ]),
-            AReg32('AFSR',          0xD3C),
-            AReg32('CPACR',         0xD88, [('CP0',                 0,  1),
-                                            ('CP1',                 2,  3),
-                                            ('CP2',                 4,  5),
-                                            ('CP3',                 6,  7),
-                                            ('CP4',                 8,  9),
-                                            ('CP5',                 10, 11),
-                                            ('CP6',                 12, 13),
-                                            ('CP7',                 14, 15),
-                                            ('CP10',                20, 21),
-                                            ('CP11',                22, 23),
-                                            ]),
-            AReg32('DHCSR',         0xDF0, [('C_DEBUGEN',           0),
-                                            ('C_HALT',              1),
-                                            ('C_STEP',              2),
-                                            ('C_MASKINTS',          3),
-                                            ('C_SNAPSTALL',         5),
-                                            ('C_PMOV',              6),
-                                            ('S_REGRDY',            16),
-                                            ('S_HALT',              17),
-                                            ('S_SLEEP',             18),
-                                            ('S_LOCKUP',            19),
-                                            ('S_SDE',               20),
-                                            ('S_NSUIDE',            21),
-                                            ('S_SUIDE',             22),
-                                            ('S_FPD',               23),
-                                            ('S_RETIRE_ST',         24),
-                                            ('S_RESET_ST',          25),
-                                            ('S_RESTART_ST',        26),
-                                            ]),
-            AReg32W('DCRSR',        0xDF4, [('REGSEL',              0,  7),
-                                            ('REGWnR',              16),
-                                            ]),
-            AReg32('DCRDR',         0xDF8, [('DBGTMP',              0,  31),
-                                            ]),
-            AReg32('DEMCR',         0xDFC, [('VC_CORERESET',        0),
-                                            ('VC_MMERR',            4),
-                                            ('VC_NOCPERR',          5),
-                                            ('VC_CHKERR',           6),
-                                            ('VC_STATEERR',         7),
-                                            ('VC_BUSERR',           8),
-                                            ('VC_INTERR',           9),
-                                            ('VC_HARDERR',          10),
-                                            ('VC_SFERR',            11),
-                                            ('MON_EN',              16),
-                                            ('MON_PEND',            17),
-                                            ('MON_STEP',            18),
-                                            ('MON_REQ',             19),
-                                            ('SDME',                20),
-                                            ('UMON_EN',             21),
-                                            ('MONPRKEY',            23),
-                                            ('TRCENA',              24),
-                                            ]),
-            AReg32('DSCEMCR',       0xE00, [('SET_MON_PEND',        1),
-                                            ('SET_MON_REQ',         3),
-                                            ('CLR_MON_PEND',        17),
-                                            ('CLR_MON_REQ',         19),
-                                            ]),
-            AReg32('DAUTHCTRL',     0xE04, [('SPIDENSEL',           0),
-                                            ('INTSPIDEN',           1),
-                                            ('SPNIDENSEL',          2),
-                                            ('INTSPNIDEN',          3),
-                                            ('FSDMA',               8),
-                                            ('UIDAPEN',             9),
-                                            ('UIDEN',               10),
-                                            ]),
-            AReg32('DSCSR',         0xE08, [('SBRSELEN',            0),
-                                            ('SBRSEL',              1),
-                                            ('CDS',                 16),
-                                            ('CDSKEY',              17),
-                                            ]),
-            ]
-
-    def __init__(self, component, subtype):
-        super().__init__(component, subtype, SCS.REGS, CORE_REGISTERS)
+    PER_ADC_REGS = [(AReg32,  'ISR',      0x00, [('ADRDY',         0),
+                                                 ('EOSMP',         1),
+                                                 ('EOC',           2),
+                                                 ('EOS',           3),
+                                                 ('OVR',           4),
+                                                 ('JEOC',          5),
+                                                 ('JEOS',          6),
+                                                 ('AWD1',          7),
+                                                 ('AWD2',          8),
+                                                 ('AWD3',          9),
+                                                 ('JQOVF',        10),
+                                                 ('LDORDY',       12),
+                                                 ]),
+                    (AReg32,  'IER',      0x04, [('ADRDYIE',       0),
+                                                 ('EOSMPIE',       1),
+                                                 ('EOCIE',         2),
+                                                 ('EOSIE',         3),
+                                                 ('OVRIE',         4),
+                                                 ('JEOCIE',        5),
+                                                 ('JEOSIE',        6),
+                                                 ('AWD1IE',        7),
+                                                 ('AWD2IE',        8),
+                                                 ('AWD3IE',        9),
+                                                 ('JQOVFIE',      10),
+                                                 ]),
+                    (AReg32,  'CR',       0x08, [('ADEN',          0),
+                                                 ('ADDIS',         1),
+                                                 ('ADSTART',       2),
+                                                 ('JADSTART',      3),
+                                                 ('ADSTP',         4),
+                                                 ('JADSTP',        5),
+                                                 ('BOOST',         8,  9),
+                                                 ('ADCALLIN',     16),
+                                                 ('LINCALRDYW1',  22),
+                                                 ('LINCALRDYW2',  23),
+                                                 ('LINCALRDYW3',  24),
+                                                 ('LINCALRDYW4',  25),
+                                                 ('LINCALRDYW5',  26),
+                                                 ('LINCALRDYW6',  27),
+                                                 ('ADVREGEN',     28),
+                                                 ('DEEPPWD',      29),
+                                                 ('ADCALDIF',     30),
+                                                 ('ADCAL',        31),
+                                                 ]),
+                    (AReg32,  'CFGR',     0x0C, [('DMNGT',         0,  1),
+                                                 ('RES',           2,  4),
+                                                 ('EXTSEL',        5,  9),
+                                                 ('EXTEN',        10, 11),
+                                                 ('OVRMOD',       12),
+                                                 ('CONT',         13),
+                                                 ('AUTDLY',       14),
+                                                 ('DISCEN',       16),
+                                                 ('DISCNUM',      17, 19),
+                                                 ('JDISCEN',      20),
+                                                 ('JQM',          21),
+                                                 ('AWD1SGL',      22),
+                                                 ('AWD1EN',       23),
+                                                 ('JAWD1EN',      24),
+                                                 ('JAUTO',        25),
+                                                 ('AWD1CH',       26, 30),
+                                                 ('JQDIS',        31),
+                                                 ]),
+                    (AReg32,  'CFGR2',    0x10, [('ROVSE',         0),
+                                                 ('JOVSE',         1),
+                                                 ('OVSS',          5,  8),
+                                                 ('TROVS',         9),
+                                                 ('ROVSM',        10),
+                                                 ('RSHIFT1',      11),
+                                                 ('RSHIFT2',      12),
+                                                 ('RSHIFT3',      13),
+                                                 ('RSHIFT4',      14),
+                                                 ('OSVR',         16, 25),
+                                                 ('LSHIFT',       28, 31),
+                                                 ]),
+                    (AReg32,  'SMPR1',    0x14, [('SMP0',          0,  2),
+                                                 ('SMP1',          3,  5),
+                                                 ('SMP2',          6,  8),
+                                                 ('SMP3',          9, 11),
+                                                 ('SMP4',         12, 14),
+                                                 ('SMP5',         15, 17),
+                                                 ('SMP6',         18, 20),
+                                                 ('SMP7',         21, 23),
+                                                 ('SMP8',         24, 26),
+                                                 ('SMP9',         27, 29),
+                                                 ]),
+                    (AReg32,  'SMPR2',    0x18, [('SMP10',         0,  2),
+                                                 ('SMP11',         3,  5),
+                                                 ('SMP12',         6,  8),
+                                                 ('SMP13',         9, 11),
+                                                 ('SMP14',        12, 14),
+                                                 ('SMP15',        15, 17),
+                                                 ('SMP16',        18, 20),
+                                                 ('SMP17',        21, 23),
+                                                 ('SMP18',        24, 26),
+                                                 ('SMP19',        27, 29),
+                                                 ]),
+                    (AReg32,  'PCSEL',    0x1C, [('PCSEL0',        0),
+                                                 ('PCSEL1',        1),
+                                                 ('PCSEL2',        2),
+                                                 ('PCSEL3',        3),
+                                                 ('PCSEL4',        4),
+                                                 ('PCSEL5',        5),
+                                                 ('PCSEL6',        6),
+                                                 ('PCSEL7',        7),
+                                                 ('PCSEL8',        8),
+                                                 ('PCSEL9',        9),
+                                                 ('PCSEL10',      10),
+                                                 ('PCSEL11',      11),
+                                                 ('PCSEL12',      12),
+                                                 ('PCSEL13',      13),
+                                                 ('PCSEL14',      14),
+                                                 ('PCSEL15',      15),
+                                                 ('PCSEL16',      16),
+                                                 ('PCSEL17',      17),
+                                                 ('PCSEL18',      18),
+                                                 ('PCSEL19',      19),
+                                                 ]),
+                    (AReg32,  'LTR1',     0x20, [('LTR1',          0, 25),
+                                                 ]),
+                    (AReg32,  'HTR1',     0x24, [('HTR1',          0, 25),
+                                                 ]),
+                    (AReg32,  'SQR1',     0x30, [('L',             0,  4),
+                                                 ('SQ1',           6, 10),
+                                                 ('SQ2',          12, 16),
+                                                 ('SQ3',          18, 22),
+                                                 ('SQ4',          24, 28),
+                                                 ]),
+                    (AReg32,  'SQR2',     0x34, [('SQ5',           0,  4),
+                                                 ('SQ6',           6, 10),
+                                                 ('SQ7',          12, 16),
+                                                 ('SQ8',          18, 22),
+                                                 ('SQ9',          24, 28),
+                                                 ]),
+                    (AReg32,  'SQR3',     0x38, [('SQ10',          0,  4),
+                                                 ('SQ11',          6, 10),
+                                                 ('SQ12',         12, 16),
+                                                 ('SQ13',         18, 22),
+                                                 ('SQ14',         24, 28),
+                                                 ]),
+                    (AReg32,  'SQR4',     0x3C, [('SQ15',          0,  4),
+                                                 ('SQ16',          6, 10),
+                                                 ]),
+                    (AReg32R, 'DR',       0x40, [('RDATA',         0, 31),
+                                                 ]),
+                    (AReg32,  'JSQR',     0x4C, [('JL',            0,  1),
+                                                 ('JEXTSEL',       2,  6),
+                                                 ('JEXTEN',        7,  8),
+                                                 ('JSQ1',          9, 13),
+                                                 ('JSQ2',         15, 19),
+                                                 ('JSQ3',         21, 25),
+                                                 ('JSQ4',         27, 31),
+                                                 ]),
+                    (AReg32,  'OFR1',     0x60, [('OFFSET1',       0, 25),
+                                                 ('OFFSET1_CH',   26, 30),
+                                                 ('SSATE',        31),
+                                                 ]),
+                    (AReg32,  'OFR2',     0x64, [('OFFSET2',       0, 25),
+                                                 ('OFFSET2_CH',   26, 30),
+                                                 ('SSATE',        31),
+                                                 ]),
+                    (AReg32,  'OFR3',     0x68, [('OFFSET3',       0, 25),
+                                                 ('OFFSET3_CH',   26, 30),
+                                                 ('SSATE',        31),
+                                                 ]),
+                    (AReg32,  'OFR4',     0x6C, [('OFFSET4',       0, 25),
+                                                 ('OFFSET4_CH',   26, 30),
+                                                 ('SSATE',        31),
+                                                 ]),
+                    (AReg32R, 'JDR1',     0x80, [('JDATA',         0, 31)]),
+                    (AReg32R, 'JDR2',     0x84, [('JDATA',         0, 31)]),
+                    (AReg32R, 'JDR3',     0x88, [('JDATA',         0, 31)]),
+                    (AReg32R, 'JDR4',     0x8C, [('JDATA',         0, 31)]),
+                    (AReg32,  'AWD2CR',   0xA0, [('AWD2CH',        0, 19)]),
+                    (AReg32,  'AWD3CR',   0xA4, [('AWD3CH',        0, 19)]),
+                    (AReg32,  'LTR2',     0xB0, [('LTR2',          0, 25)]),
+                    (AReg32,  'HTR2',     0xB4, [('HTR2',          0, 25)]),
+                    (AReg32,  'LTR3',     0xB8, [('LTR3',          0, 25)]),
+                    (AReg32,  'HTR3',     0xBC, [('HTR3',          0, 25)]),
+                    (AReg32,  'DIFSEL',   0xC0, [('DIFSEL',        0, 19)]),
+                    (AReg32,  'CALFACT',  0xC4, [('CALFACT_S',     0, 10),
+                                                 ('CALFACT_D',    16, 26),
+                                                 ]),
+                    (AReg32,  'CALFACT2', 0xC8, [('LINCALFACT',    0, 29)]),
+                    ]
+    COM_ADC_REGS = [AReg32R('CSR',  0x300,     [('ADRDY_MST',     0),
+                                                ('EOSMP_MST',     1),
+                                                ('EOC_MST',       2),
+                                                ('EOS_MST',       3),
+                                                ('OVR_MST',       4),
+                                                ('JEOC_MST',      5),
+                                                ('JEOS_MST',      6),
+                                                ('AWD1_MST',      7),
+                                                ('AWD2_MST',      8),
+                                                ('AWD3_MST',      9),
+                                                ('JQOVF_MST',    10),
+                                                ('ADRDY_SLV',    16),
+                                                ('EOSMP_SLV',    17),
+                                                ('EOC_SLV',      18),
+                                                ('EOS_SLV',      19),
+                                                ('OVR_SLV',      20),
+                                                ('JEOC_SLV',     21),
+                                                ('JEOS_SLV',     22),
+                                                ('AWD1_SLV',     23),
+                                                ('AWD2_SLV',     24),
+                                                ('AWD3_SLV',     25),
+                                                ('JQOVF_SLV',    26),
+                                                ]),
+                    AReg32 ('CCR',  0x308,     [('DUAL',          0,  4),
+                                                ('DELAY',         8, 11),
+                                                ('DAMDF',        14, 15),
+                                                ('CKMODE',       16, 17),
+                                                ('PRESC',        18, 21),
+                                                ('VREFEN',       22),
+                                                ('TSEN',         23),
+                                                ('VBATEN',       24),
+                                                ]),
+                    AReg32R('CDR',  0x30C,     [('RDATA_MST',     0, 15),
+                                                ('RDATA_SLV',    16, 31),
+                                                ]),
+                    AReg32R('CDR2', 0x310,     [('RDATA_ALT',     0, 31),
+                                                ]),
+                    ]
+
+    def __init__(self, target, ap, name, addr, first_adc, nadcs, **kwargs):
+        regs = []
+        for i in range(nadcs):
+            base = 0x100*i
+            regs += [cls(_name + ('_%u' % (first_adc + i)), base + offset,
+                         fields)
+                     for cls, _name, offset, fields in ADC16.PER_ADC_REGS]
+        regs += ADC16.COM_ADC_REGS
 
-        # Enable DEMCR.TRCENA so we can probe further.
-        self._DEMCR.TRCENA = 1
+        super().__init__(target, ap, addr, name, regs, **kwargs)
```

### Comparing `psdb-1.1.2/psdb/devices/core/tpiu_m4.py` & `psdb-1.1.3/psdb/devices/core/tpiu_m4.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/device.py` & `psdb-1.1.3/psdb/devices/device.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/flash.py` & `psdb-1.1.3/psdb/devices/flash.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/msp432/flctl.py` & `psdb-1.1.3/psdb/devices/msp432/flctl.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/__init__.py` & `psdb-1.1.3/psdb/devices/stm32/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2019-2020 Phase Advanced Sensor Systems, Inc.
 from .advanced_control_timer import ACT
 from .adc import ADC
+from .adc_12 import ADC12
 from .adc_14 import ADC14
 from .adc_16 import ADC16
 from .basic_timer import BT
 from .dac import DAC, DAC_Saw
 from .vrefbuf import VREF
 from .dma import DMA, DMA_DBM
 from .dma_mux import DMAMUX
@@ -21,14 +22,15 @@
 from .gpdma import GPDMA
 from .cordic import CORDIC
 from . import flash_type1
 
 
 __all__ = ['ACT',
            'ADC',
+           'ADC12',
            'ADC14',
            'ADC16',
            'BT',
            'CORDIC',
            'CRS',
            'DAC',
            'DAC_Saw',
```

### Comparing `psdb-1.1.2/psdb/devices/stm32/adc.py` & `psdb-1.1.3/psdb/devices/stm32/adc.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from builtins import range
 
 from ..device import Device, Reg32, Reg32R
 
 
 class ADC(Device):
     '''
-    Driver for the STM32G4 ADC.
+    Driver for the STM32G4 12-bit ADC.
     '''
     PER_ADC_REGS = [(Reg32,  'ISR',     0x00, [('ADRDY',        1),
                                                ('EOSMP',        1),
                                                ('EOC',          1),
                                                ('EOS',          1),
                                                ('OVR',          1),
                                                ('JEOC',         1),
```

### Comparing `psdb-1.1.2/psdb/devices/stm32/adc_14.py` & `psdb-1.1.3/psdb/devices/stm32/adc_14.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from builtins import range
 
 from ..device import Device, AReg32, AReg32R
 
 
 class ADC14(Device):
     '''
-    Driver for the STM32H7 16-bit ADC.
+    Driver for the STM32U5 14-bit ADC.
     '''
     PER_ADC_REGS = [(AReg32,  'ISR',      0x00, [('ADRDY',         0),
                                                  ('EOSMP',         1),
                                                  ('EOC',           2),
                                                  ('EOS',           3),
                                                  ('OVR',           4),
                                                  ('JEOC',          5),
```

### Comparing `psdb-1.1.2/psdb/devices/stm32/adc_16.py` & `psdb-1.1.3/psdb/devices/stm32g4/pwr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,243 +1,336 @@
-# Copyright (c) 2019-2021 Phase Advanced Sensor Systems, Inc.
-from builtins import range
+# Copyright (c) 2018-2019 Phase Advanced Sensor Systems, Inc.
+import time
 
-from ..device import Device, AReg32, AReg32R
+from ..device import Device, AReg32
 
 
-class ADC16(Device):
+class PWR(Device):
     '''
-    Driver for the STM32H7 16-bit ADC.
+    Driver for the STM Power Control (PWR) device.
     '''
-    PER_ADC_REGS = [(AReg32,  'ISR',      0x00, [('ADRDY',         0),
-                                                 ('EOSMP',         1),
-                                                 ('EOC',           2),
-                                                 ('EOS',           3),
-                                                 ('OVR',           4),
-                                                 ('JEOC',          5),
-                                                 ('JEOS',          6),
-                                                 ('AWD1',          7),
-                                                 ('AWD2',          8),
-                                                 ('AWD3',          9),
-                                                 ('JQOVF',        10),
-                                                 ('LDORDY',       12),
-                                                 ]),
-                    (AReg32,  'IER',      0x04, [('ADRDYIE',       0),
-                                                 ('EOSMPIE',       1),
-                                                 ('EOCIE',         2),
-                                                 ('EOSIE',         3),
-                                                 ('OVRIE',         4),
-                                                 ('JEOCIE',        5),
-                                                 ('JEOSIE',        6),
-                                                 ('AWD1IE',        7),
-                                                 ('AWD2IE',        8),
-                                                 ('AWD3IE',        9),
-                                                 ('JQOVFIE',      10),
-                                                 ]),
-                    (AReg32,  'CR',       0x08, [('ADEN',          0),
-                                                 ('ADDIS',         1),
-                                                 ('ADSTART',       2),
-                                                 ('JADSTART',      3),
-                                                 ('ADSTP',         4),
-                                                 ('JADSTP',        5),
-                                                 ('BOOST',         8,  9),
-                                                 ('ADCALLIN',     16),
-                                                 ('LINCALRDYW1',  22),
-                                                 ('LINCALRDYW2',  23),
-                                                 ('LINCALRDYW3',  24),
-                                                 ('LINCALRDYW4',  25),
-                                                 ('LINCALRDYW5',  26),
-                                                 ('LINCALRDYW6',  27),
-                                                 ('ADVREGEN',     28),
-                                                 ('DEEPPWD',      29),
-                                                 ('ADCALDIF',     30),
-                                                 ('ADCAL',        31),
-                                                 ]),
-                    (AReg32,  'CFGR',     0x0C, [('DMNGT',         0,  1),
-                                                 ('RES',           2,  4),
-                                                 ('EXTSEL',        5,  9),
-                                                 ('EXTEN',        10, 11),
-                                                 ('OVRMOD',       12),
-                                                 ('CONT',         13),
-                                                 ('AUTDLY',       14),
-                                                 ('DISCEN',       16),
-                                                 ('DISCNUM',      17, 19),
-                                                 ('JDISCEN',      20),
-                                                 ('JQM',          21),
-                                                 ('AWD1SGL',      22),
-                                                 ('AWD1EN',       23),
-                                                 ('JAWD1EN',      24),
-                                                 ('JAUTO',        25),
-                                                 ('AWD1CH',       26, 30),
-                                                 ('JQDIS',        31),
-                                                 ]),
-                    (AReg32,  'CFGR2',    0x10, [('ROVSE',         0),
-                                                 ('JOVSE',         1),
-                                                 ('OVSS',          5,  8),
-                                                 ('TROVS',         9),
-                                                 ('ROVSM',        10),
-                                                 ('RSHIFT1',      11),
-                                                 ('RSHIFT2',      12),
-                                                 ('RSHIFT3',      13),
-                                                 ('RSHIFT4',      14),
-                                                 ('OSVR',         16, 25),
-                                                 ('LSHIFT',       28, 31),
-                                                 ]),
-                    (AReg32,  'SMPR1',    0x14, [('SMP0',          0,  2),
-                                                 ('SMP1',          3,  5),
-                                                 ('SMP2',          6,  8),
-                                                 ('SMP3',          9, 11),
-                                                 ('SMP4',         12, 14),
-                                                 ('SMP5',         15, 17),
-                                                 ('SMP6',         18, 20),
-                                                 ('SMP7',         21, 23),
-                                                 ('SMP8',         24, 26),
-                                                 ('SMP9',         27, 29),
-                                                 ]),
-                    (AReg32,  'SMPR2',    0x18, [('SMP10',         0,  2),
-                                                 ('SMP11',         3,  5),
-                                                 ('SMP12',         6,  8),
-                                                 ('SMP13',         9, 11),
-                                                 ('SMP14',        12, 14),
-                                                 ('SMP15',        15, 17),
-                                                 ('SMP16',        18, 20),
-                                                 ('SMP17',        21, 23),
-                                                 ('SMP18',        24, 26),
-                                                 ('SMP19',        27, 29),
-                                                 ]),
-                    (AReg32,  'PCSEL',    0x1C, [('PCSEL0',        0),
-                                                 ('PCSEL1',        1),
-                                                 ('PCSEL2',        2),
-                                                 ('PCSEL3',        3),
-                                                 ('PCSEL4',        4),
-                                                 ('PCSEL5',        5),
-                                                 ('PCSEL6',        6),
-                                                 ('PCSEL7',        7),
-                                                 ('PCSEL8',        8),
-                                                 ('PCSEL9',        9),
-                                                 ('PCSEL10',      10),
-                                                 ('PCSEL11',      11),
-                                                 ('PCSEL12',      12),
-                                                 ('PCSEL13',      13),
-                                                 ('PCSEL14',      14),
-                                                 ('PCSEL15',      15),
-                                                 ('PCSEL16',      16),
-                                                 ('PCSEL17',      17),
-                                                 ('PCSEL18',      18),
-                                                 ('PCSEL19',      19),
-                                                 ]),
-                    (AReg32,  'LTR1',     0x20, [('LTR1',          0, 25),
-                                                 ]),
-                    (AReg32,  'HTR1',     0x24, [('HTR1',          0, 25),
-                                                 ]),
-                    (AReg32,  'SQR1',     0x30, [('L',             0,  4),
-                                                 ('SQ1',           6, 10),
-                                                 ('SQ2',          12, 16),
-                                                 ('SQ3',          18, 22),
-                                                 ('SQ4',          24, 28),
-                                                 ]),
-                    (AReg32,  'SQR2',     0x34, [('SQ5',           0,  4),
-                                                 ('SQ6',           6, 10),
-                                                 ('SQ7',          12, 16),
-                                                 ('SQ8',          18, 22),
-                                                 ('SQ9',          24, 28),
-                                                 ]),
-                    (AReg32,  'SQR3',     0x38, [('SQ10',          0,  4),
-                                                 ('SQ11',          6, 10),
-                                                 ('SQ12',         12, 16),
-                                                 ('SQ13',         18, 22),
-                                                 ('SQ14',         24, 28),
-                                                 ]),
-                    (AReg32,  'SQR4',     0x3C, [('SQ15',          0,  4),
-                                                 ('SQ16',          6, 10),
-                                                 ]),
-                    (AReg32R, 'DR',       0x40, [('RDATA',         0, 31),
-                                                 ]),
-                    (AReg32,  'JSQR',     0x4C, [('JL',            0,  1),
-                                                 ('JEXTSEL',       2,  6),
-                                                 ('JEXTEN',        7,  8),
-                                                 ('JSQ1',          9, 13),
-                                                 ('JSQ2',         15, 19),
-                                                 ('JSQ3',         21, 25),
-                                                 ('JSQ4',         27, 31),
-                                                 ]),
-                    (AReg32,  'OFR1',     0x60, [('OFFSET1',       0, 25),
-                                                 ('OFFSET1_CH',   26, 30),
-                                                 ('SSATE',        31),
-                                                 ]),
-                    (AReg32,  'OFR2',     0x64, [('OFFSET2',       0, 25),
-                                                 ('OFFSET2_CH',   26, 30),
-                                                 ('SSATE',        31),
-                                                 ]),
-                    (AReg32,  'OFR3',     0x68, [('OFFSET3',       0, 25),
-                                                 ('OFFSET3_CH',   26, 30),
-                                                 ('SSATE',        31),
-                                                 ]),
-                    (AReg32,  'OFR4',     0x6C, [('OFFSET4',       0, 25),
-                                                 ('OFFSET4_CH',   26, 30),
-                                                 ('SSATE',        31),
-                                                 ]),
-                    (AReg32R, 'JDR1',     0x80, [('JDATA',         0, 31)]),
-                    (AReg32R, 'JDR2',     0x84, [('JDATA',         0, 31)]),
-                    (AReg32R, 'JDR3',     0x88, [('JDATA',         0, 31)]),
-                    (AReg32R, 'JDR4',     0x8C, [('JDATA',         0, 31)]),
-                    (AReg32,  'AWD2CR',   0xA0, [('AWD2CH',        0, 19)]),
-                    (AReg32,  'AWD3CR',   0xA4, [('AWD3CH',        0, 19)]),
-                    (AReg32,  'LTR2',     0xB0, [('LTR2',          0, 25)]),
-                    (AReg32,  'HTR2',     0xB4, [('HTR2',          0, 25)]),
-                    (AReg32,  'LTR3',     0xB8, [('LTR3',          0, 25)]),
-                    (AReg32,  'HTR3',     0xBC, [('HTR3',          0, 25)]),
-                    (AReg32,  'DIFSEL',   0xC0, [('DIFSEL',        0, 19)]),
-                    (AReg32,  'CALFACT',  0xC4, [('CALFACT_S',     0, 10),
-                                                 ('CALFACT_D',    16, 26),
-                                                 ]),
-                    (AReg32,  'CALFACT2', 0xC8, [('LINCALFACT',    0, 29)]),
-                    ]
-    COM_ADC_REGS = [AReg32R('CSR',  0x300,     [('ADRDY_MST',     0),
-                                                ('EOSMP_MST',     1),
-                                                ('EOC_MST',       2),
-                                                ('EOS_MST',       3),
-                                                ('OVR_MST',       4),
-                                                ('JEOC_MST',      5),
-                                                ('JEOS_MST',      6),
-                                                ('AWD1_MST',      7),
-                                                ('AWD2_MST',      8),
-                                                ('AWD3_MST',      9),
-                                                ('JQOVF_MST',    10),
-                                                ('ADRDY_SLV',    16),
-                                                ('EOSMP_SLV',    17),
-                                                ('EOC_SLV',      18),
-                                                ('EOS_SLV',      19),
-                                                ('OVR_SLV',      20),
-                                                ('JEOC_SLV',     21),
-                                                ('JEOS_SLV',     22),
-                                                ('AWD1_SLV',     23),
-                                                ('AWD2_SLV',     24),
-                                                ('AWD3_SLV',     25),
-                                                ('JQOVF_SLV',    26),
-                                                ]),
-                    AReg32 ('CCR',  0x308,     [('DUAL',          0,  4),
-                                                ('DELAY',         8, 11),
-                                                ('DAMDF',        14, 15),
-                                                ('CKMODE',       16, 17),
-                                                ('PRESC',        18, 21),
-                                                ('VREFEN',       22),
-                                                ('TSEN',         23),
-                                                ('VBATEN',       24),
-                                                ]),
-                    AReg32R('CDR',  0x30C,     [('RDATA_MST',     0, 15),
-                                                ('RDATA_SLV',    16, 31),
-                                                ]),
-                    AReg32R('CDR2', 0x310,     [('RDATA_ALT',     0, 31),
-                                                ]),
-                    ]
-
-    def __init__(self, target, ap, name, addr, first_adc, nadcs, **kwargs):
-        regs = []
-        for i in range(nadcs):
-            base = 0x100*i
-            regs += [cls(_name + ('_%u' % (first_adc + i)), base + offset,
-                         fields)
-                     for cls, _name, offset, fields in ADC16.PER_ADC_REGS]
-        regs += ADC16.COM_ADC_REGS
+    VCORE_1V00 = 0
+    VCORE_1V20 = 1
+    VCORE_1V28 = 2
 
-        super().__init__(target, ap, addr, name, regs, **kwargs)
+    REGS = [AReg32('CR1',       0x000, [('LPMS',        0, 2),
+                                        ('DBP',         8),
+                                        ('VOS',         9, 10),
+                                        ('LPR',         14),
+                                        ]),
+            AReg32('CR2',       0x004, [('PVDE',        0),
+                                        ('PLS',         1, 3),
+                                        ('PVMEN1',      6),
+                                        ('PVMEN2',      7),
+                                        ]),
+            AReg32('CR3',       0x008, [('EWUP1',       0),
+                                        ('EWUP2',       1),
+                                        ('EWUP3',       2),
+                                        ('EWUP4',       3),
+                                        ('EWUP5',       4),
+                                        ('RRS',         8),
+                                        ('APC',         10),
+                                        ('UCPD1_STDBY', 13),
+                                        ('UCPD1_DBDIS', 14),
+                                        ('EIWUL',       15),
+                                        ]),
+            AReg32('CR4',       0x00C, [('WP1',         0),
+                                        ('WP2',         1),
+                                        ('WP3',         2),
+                                        ('WP4',         3),
+                                        ('WP5',         4),
+                                        ('VBE',         8),
+                                        ('VBRS',        9),
+                                        ]),
+            AReg32('SR1',       0x010, [('WUF1',        0),
+                                        ('WUF2',        1),
+                                        ('WUF3',        2),
+                                        ('WUF4',        3),
+                                        ('WUF5',        4),
+                                        ('SBF',         8),
+                                        ('WUFI',        15),
+                                        ]),
+            AReg32('SR2',       0x014, [('REGLPS',      8),
+                                        ('REGLPF',      9),
+                                        ('VOSF',        10),
+                                        ('PVDO',        11),
+                                        ('PVMO1',       14),
+                                        ('PVMO2',       15),
+                                        ]),
+            AReg32('SCR',       0x018, [('CWUF1',       0),
+                                        ('CWUF2',       1),
+                                        ('CWUF3',       2),
+                                        ('CWUF4',       3),
+                                        ('CWUF5',       4),
+                                        ('CSBF',        8),
+                                        ]),
+            AReg32('PUCRA',     0x020, [('PU0',         0),
+                                        ('PU1',         1),
+                                        ('PU2',         2),
+                                        ('PU3',         3),
+                                        ('PU4',         4),
+                                        ('PU5',         5),
+                                        ('PU6',         6),
+                                        ('PU7',         7),
+                                        ('PU8',         8),
+                                        ('PU9',         9),
+                                        ('PU10',        10),
+                                        ('PU11',        11),
+                                        ('PU12',        12),
+                                        ('PU13',        13),
+                                        # ('PU14',        14),
+                                        ('PU15',        15),
+                                        ]),
+            AReg32('PDCRA',     0x024, [('PD0',         0),
+                                        ('PD1',         1),
+                                        ('PD2',         2),
+                                        ('PD3',         3),
+                                        ('PD4',         4),
+                                        ('PD5',         5),
+                                        ('PD6',         6),
+                                        ('PD7',         7),
+                                        ('PD8',         8),
+                                        ('PD9',         9),
+                                        ('PD10',        10),
+                                        ('PD11',        11),
+                                        ('PD12',        12),
+                                        # ('PD13',        13),
+                                        ('PD14',        14),
+                                        # ('PD15',        15),
+                                        ]),
+            AReg32('PUCRB',     0x028, [('PU0',         0),
+                                        ('PU1',         1),
+                                        ('PU2',         2),
+                                        ('PU3',         3),
+                                        ('PU4',         4),
+                                        ('PU5',         5),
+                                        ('PU6',         6),
+                                        ('PU7',         7),
+                                        ('PU8',         8),
+                                        ('PU9',         9),
+                                        ('PU10',        10),
+                                        ('PU11',        11),
+                                        ('PU12',        12),
+                                        ('PU13',        13),
+                                        ('PU14',        14),
+                                        ('PU15',        15),
+                                        ]),
+            AReg32('PDCRB',     0x02C, [('PD0',         0),
+                                        ('PD1',         1),
+                                        ('PD2',         2),
+                                        ('PD3',         3),
+                                        # ('PD4',         4),
+                                        ('PD5',         5),
+                                        ('PD6',         6),
+                                        ('PD7',         7),
+                                        ('PD8',         8),
+                                        ('PD9',         9),
+                                        ('PD10',        10),
+                                        ('PD11',        11),
+                                        ('PD12',        12),
+                                        ('PD13',        13),
+                                        ('PD14',        14),
+                                        ('PD15',        15),
+                                        ]),
+            AReg32('PUCRC',     0x030, [('PU0',         0),
+                                        ('PU1',         1),
+                                        ('PU2',         2),
+                                        ('PU3',         3),
+                                        ('PU4',         4),
+                                        ('PU5',         5),
+                                        ('PU6',         6),
+                                        ('PU7',         7),
+                                        ('PU8',         8),
+                                        ('PU9',         9),
+                                        ('PU10',        10),
+                                        ('PU11',        11),
+                                        ('PU12',        12),
+                                        ('PU13',        13),
+                                        ('PU14',        14),
+                                        ('PU15',        15),
+                                        ]),
+            AReg32('PDCRC',     0x034, [('PD0',         0),
+                                        ('PD1',         1),
+                                        ('PD2',         2),
+                                        ('PD3',         3),
+                                        ('PD4',         4),
+                                        ('PD5',         5),
+                                        ('PD6',         6),
+                                        ('PD7',         7),
+                                        ('PD8',         8),
+                                        ('PD9',         9),
+                                        ('PD10',        10),
+                                        ('PD11',        11),
+                                        ('PD12',        12),
+                                        ('PD13',        13),
+                                        ('PD14',        14),
+                                        ('PD15',        15),
+                                        ]),
+            AReg32('PUCRD',     0x038, [('PU0',         0),
+                                        ('PU1',         1),
+                                        ('PU2',         2),
+                                        ('PU3',         3),
+                                        ('PU4',         4),
+                                        ('PU5',         5),
+                                        ('PU6',         6),
+                                        ('PU7',         7),
+                                        ('PU8',         8),
+                                        ('PU9',         9),
+                                        ('PU10',        10),
+                                        ('PU11',        11),
+                                        ('PU12',        12),
+                                        ('PU13',        13),
+                                        ('PU14',        14),
+                                        ('PU15',        15),
+                                        ]),
+            AReg32('PDCRD',     0x03C, [('PD0',         0),
+                                        ('PD1',         1),
+                                        ('PD2',         2),
+                                        ('PD3',         3),
+                                        ('PD4',         4),
+                                        ('PD5',         5),
+                                        ('PD6',         6),
+                                        ('PD7',         7),
+                                        ('PD8',         8),
+                                        ('PD9',         9),
+                                        ('PD10',        10),
+                                        ('PD11',        11),
+                                        ('PD12',        12),
+                                        ('PD13',        13),
+                                        ('PD14',        14),
+                                        ('PD15',        15),
+                                        ]),
+            AReg32('PUCRE',     0x040, [('PU0',         0),
+                                        ('PU1',         1),
+                                        ('PU2',         2),
+                                        ('PU3',         3),
+                                        ('PU4',         4),
+                                        ('PU5',         5),
+                                        ('PU6',         6),
+                                        ('PU7',         7),
+                                        ('PU8',         8),
+                                        ('PU9',         9),
+                                        ('PU10',        10),
+                                        ('PU11',        11),
+                                        ('PU12',        12),
+                                        ('PU13',        13),
+                                        ('PU14',        14),
+                                        ('PU15',        15),
+                                        ]),
+            AReg32('PDCRE',     0x044, [('PD0',         0),
+                                        ('PD1',         1),
+                                        ('PD2',         2),
+                                        ('PD3',         3),
+                                        ('PD4',         4),
+                                        ('PD5',         5),
+                                        ('PD6',         6),
+                                        ('PD7',         7),
+                                        ('PD8',         8),
+                                        ('PD9',         9),
+                                        ('PD10',        10),
+                                        ('PD11',        11),
+                                        ('PD12',        12),
+                                        ('PD13',        13),
+                                        ('PD14',        14),
+                                        ('PD15',        15),
+                                        ]),
+            AReg32('PUCRF',     0x048, [('PU0',         0),
+                                        ('PU1',         1),
+                                        ('PU2',         2),
+                                        ('PU3',         3),
+                                        ('PU4',         4),
+                                        ('PU5',         5),
+                                        ('PU6',         6),
+                                        ('PU7',         7),
+                                        ('PU8',         8),
+                                        ('PU9',         9),
+                                        ('PU10',        10),
+                                        ('PU11',        11),
+                                        ('PU12',        12),
+                                        ('PU13',        13),
+                                        ('PU14',        14),
+                                        ('PU15',        15),
+                                        ]),
+            AReg32('PDCRF',     0x04C, [('PD0',         0),
+                                        ('PD1',         1),
+                                        ('PD2',         2),
+                                        ('PD3',         3),
+                                        ('PD4',         4),
+                                        ('PD5',         5),
+                                        ('PD6',         6),
+                                        ('PD7',         7),
+                                        ('PD8',         8),
+                                        ('PD9',         9),
+                                        ('PD10',        10),
+                                        ('PD11',        11),
+                                        ('PD12',        12),
+                                        ('PD13',        13),
+                                        ('PD14',        14),
+                                        ('PD15',        15),
+                                        ]),
+            AReg32('PUCRG',     0x050, [('PU0',         0),
+                                        ('PU1',         1),
+                                        ('PU2',         2),
+                                        ('PU3',         3),
+                                        ('PU4',         4),
+                                        ('PU5',         5),
+                                        ('PU6',         6),
+                                        ('PU7',         7),
+                                        ('PU8',         8),
+                                        ('PU9',         9),
+                                        ('PU10',        10),
+                                        # ('PU11',        11),
+                                        # ('PU12',        12),
+                                        # ('PU13',        13),
+                                        # ('PU14',        14),
+                                        # ('PU15',        15),
+                                        ]),
+            AReg32('PDCRG',     0x054, [('PD0',         0),
+                                        ('PD1',         1),
+                                        ('PD2',         2),
+                                        ('PD3',         3),
+                                        ('PD4',         4),
+                                        ('PD5',         5),
+                                        ('PD6',         6),
+                                        ('PD7',         7),
+                                        ('PD8',         8),
+                                        ('PD9',         9),
+                                        ('PD10',        10),
+                                        # ('PD11',        11),
+                                        # ('PD12',        12),
+                                        # ('PD13',        13),
+                                        # ('PD14',        14),
+                                        # ('PD15',        15),
+                                        ]),
+            AReg32('CR5',       0x080, [('R1MODE',      8),
+                                        ]),
+            ]
+
+    def __init__(self, target, ap, name, addr, **kwargs):
+        super().__init__(target, ap, addr, name, PWR.REGS, **kwargs)
+
+    def unlock_backup_domain(self):
+        self._CR1.DBP = 1
+        while self._CR1.DBP == 0:
+            time.sleep(0.01)
+
+    def wait_vosf_ready(self):
+        while self._SR2.VOSF == 1:
+            time.sleep(0.01)
+
+    def set_vcore_voltage(self, vcv):
+        if vcv == self.VCORE_1V00:
+            self._CR5.R1MODE = 1
+            self.wait_vosf_ready()
+            self._CR1.VOS = 2
+        elif vcv == self.VCORE_1V20:
+            self._CR5.R1MODE = 1
+            self.wait_vosf_ready()
+            self._CR1.VOS = 1
+        elif vcv == self.VCORE_1V28:
+            self._CR1.VOS = 1
+            self.wait_vosf_ready()
+            self._CR5.R1MODE = 0
+        else:
+            raise Exception('Invalid vcore voltage %s' % vcv)
+
+        self.wait_vosf_ready()
```

### Comparing `psdb-1.1.2/psdb/devices/stm32/advanced_control_timer.py` & `psdb-1.1.3/psdb/devices/stm32/advanced_control_timer.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/basic_timer.py` & `psdb-1.1.3/psdb/devices/stm32/basic_timer.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/cordic.py` & `psdb-1.1.3/psdb/devices/stm32/cordic.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/crs.py` & `psdb-1.1.3/psdb/devices/stm32/crs.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/dac.py` & `psdb-1.1.3/psdb/devices/stm32/dac.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/dma.py` & `psdb-1.1.3/psdb/devices/stm32/dma.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/dma_mux.py` & `psdb-1.1.3/psdb/devices/stm32/dma_mux.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/flash_type1.py` & `psdb-1.1.3/psdb/devices/stm32/flash_type1.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/general_purpose_timer_16x1.py` & `psdb-1.1.3/psdb/devices/stm32/general_purpose_timer_16x1.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/general_purpose_timer_16x2.py` & `psdb-1.1.3/psdb/devices/stm32/general_purpose_timer_16x2.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/general_purpose_timer_16x4.py` & `psdb-1.1.3/psdb/devices/stm32/general_purpose_timer_16x4.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/general_purpose_timer_32.py` & `psdb-1.1.3/psdb/devices/stm32/general_purpose_timer_32.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/gpdma.py` & `psdb-1.1.3/psdb/devices/stm32/gpdma.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/gpio.py` & `psdb-1.1.3/psdb/devices/stm32/gpio.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/lpuart.py` & `psdb-1.1.3/psdb/devices/stm32/lpuart.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/qspi.py` & `psdb-1.1.3/psdb/devices/stm32/qspi.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/usb.py` & `psdb-1.1.3/psdb/devices/stm32/usb.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/usb_hs.py` & `psdb-1.1.3/psdb/devices/stm32/usb_hs.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32/vrefbuf.py` & `psdb-1.1.3/psdb/devices/stm32/vrefbuf.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g0/flash.py` & `psdb-1.1.3/psdb/devices/stm32g0/flash.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/__init__.py` & `psdb-1.1.3/psdb/devices/stm32g4/__init__.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/comparator.py` & `psdb-1.1.3/psdb/devices/stm32g4/comparator.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/dbgmcu.py` & `psdb-1.1.3/psdb/devices/stm32g4/dbgmcu.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/flash_2.py` & `psdb-1.1.3/psdb/devices/stm32g4/flash_2.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/flash_3.py` & `psdb-1.1.3/psdb/devices/stm32g4/flash_3.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/flash_4.py` & `psdb-1.1.3/psdb/devices/stm32g4/flash_4.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/opamp.py` & `psdb-1.1.3/psdb/devices/stm32g4/opamp.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/pwr.py` & `psdb-1.1.3/psdb/devices/stm32u5/pwr.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,336 +1,446 @@
-# Copyright (c) 2018-2019 Phase Advanced Sensor Systems, Inc.
+# Copyright (c) 2022 Phase Advanced Sensor Systems, Inc.
 import time
 
 from ..device import Device, AReg32
 
 
 class PWR(Device):
     '''
-    Driver for the STM Power Control (PWR) device.
+    Driver for the STM32U5 Power Control (PWR) device.
     '''
-    VCORE_1V00 = 0
-    VCORE_1V20 = 1
-    VCORE_1V28 = 2
-
-    REGS = [AReg32('CR1',       0x000, [('LPMS',        0, 2),
-                                        ('DBP',         8),
-                                        ('VOS',         9, 10),
-                                        ('LPR',         14),
-                                        ]),
-            AReg32('CR2',       0x004, [('PVDE',        0),
-                                        ('PLS',         1, 3),
-                                        ('PVMEN1',      6),
-                                        ('PVMEN2',      7),
-                                        ]),
-            AReg32('CR3',       0x008, [('EWUP1',       0),
-                                        ('EWUP2',       1),
-                                        ('EWUP3',       2),
-                                        ('EWUP4',       3),
-                                        ('EWUP5',       4),
-                                        ('RRS',         8),
-                                        ('APC',         10),
-                                        ('UCPD1_STDBY', 13),
-                                        ('UCPD1_DBDIS', 14),
-                                        ('EIWUL',       15),
-                                        ]),
-            AReg32('CR4',       0x00C, [('WP1',         0),
-                                        ('WP2',         1),
-                                        ('WP3',         2),
-                                        ('WP4',         3),
-                                        ('WP5',         4),
-                                        ('VBE',         8),
-                                        ('VBRS',        9),
-                                        ]),
-            AReg32('SR1',       0x010, [('WUF1',        0),
-                                        ('WUF2',        1),
-                                        ('WUF3',        2),
-                                        ('WUF4',        3),
-                                        ('WUF5',        4),
-                                        ('SBF',         8),
-                                        ('WUFI',        15),
-                                        ]),
-            AReg32('SR2',       0x014, [('REGLPS',      8),
-                                        ('REGLPF',      9),
-                                        ('VOSF',        10),
-                                        ('PVDO',        11),
-                                        ('PVMO1',       14),
-                                        ('PVMO2',       15),
-                                        ]),
-            AReg32('SCR',       0x018, [('CWUF1',       0),
-                                        ('CWUF2',       1),
-                                        ('CWUF3',       2),
-                                        ('CWUF4',       3),
-                                        ('CWUF5',       4),
-                                        ('CSBF',        8),
-                                        ]),
-            AReg32('PUCRA',     0x020, [('PU0',         0),
-                                        ('PU1',         1),
-                                        ('PU2',         2),
-                                        ('PU3',         3),
-                                        ('PU4',         4),
-                                        ('PU5',         5),
-                                        ('PU6',         6),
-                                        ('PU7',         7),
-                                        ('PU8',         8),
-                                        ('PU9',         9),
-                                        ('PU10',        10),
-                                        ('PU11',        11),
-                                        ('PU12',        12),
-                                        ('PU13',        13),
-                                        # ('PU14',        14),
-                                        ('PU15',        15),
-                                        ]),
-            AReg32('PDCRA',     0x024, [('PD0',         0),
-                                        ('PD1',         1),
-                                        ('PD2',         2),
-                                        ('PD3',         3),
-                                        ('PD4',         4),
-                                        ('PD5',         5),
-                                        ('PD6',         6),
-                                        ('PD7',         7),
-                                        ('PD8',         8),
-                                        ('PD9',         9),
-                                        ('PD10',        10),
-                                        ('PD11',        11),
-                                        ('PD12',        12),
-                                        # ('PD13',        13),
-                                        ('PD14',        14),
-                                        # ('PD15',        15),
-                                        ]),
-            AReg32('PUCRB',     0x028, [('PU0',         0),
-                                        ('PU1',         1),
-                                        ('PU2',         2),
-                                        ('PU3',         3),
-                                        ('PU4',         4),
-                                        ('PU5',         5),
-                                        ('PU6',         6),
-                                        ('PU7',         7),
-                                        ('PU8',         8),
-                                        ('PU9',         9),
-                                        ('PU10',        10),
-                                        ('PU11',        11),
-                                        ('PU12',        12),
-                                        ('PU13',        13),
-                                        ('PU14',        14),
-                                        ('PU15',        15),
-                                        ]),
-            AReg32('PDCRB',     0x02C, [('PD0',         0),
-                                        ('PD1',         1),
-                                        ('PD2',         2),
-                                        ('PD3',         3),
-                                        # ('PD4',         4),
-                                        ('PD5',         5),
-                                        ('PD6',         6),
-                                        ('PD7',         7),
-                                        ('PD8',         8),
-                                        ('PD9',         9),
-                                        ('PD10',        10),
-                                        ('PD11',        11),
-                                        ('PD12',        12),
-                                        ('PD13',        13),
-                                        ('PD14',        14),
-                                        ('PD15',        15),
-                                        ]),
-            AReg32('PUCRC',     0x030, [('PU0',         0),
-                                        ('PU1',         1),
-                                        ('PU2',         2),
-                                        ('PU3',         3),
-                                        ('PU4',         4),
-                                        ('PU5',         5),
-                                        ('PU6',         6),
-                                        ('PU7',         7),
-                                        ('PU8',         8),
-                                        ('PU9',         9),
-                                        ('PU10',        10),
-                                        ('PU11',        11),
-                                        ('PU12',        12),
-                                        ('PU13',        13),
-                                        ('PU14',        14),
-                                        ('PU15',        15),
-                                        ]),
-            AReg32('PDCRC',     0x034, [('PD0',         0),
-                                        ('PD1',         1),
-                                        ('PD2',         2),
-                                        ('PD3',         3),
-                                        ('PD4',         4),
-                                        ('PD5',         5),
-                                        ('PD6',         6),
-                                        ('PD7',         7),
-                                        ('PD8',         8),
-                                        ('PD9',         9),
-                                        ('PD10',        10),
-                                        ('PD11',        11),
-                                        ('PD12',        12),
-                                        ('PD13',        13),
-                                        ('PD14',        14),
-                                        ('PD15',        15),
-                                        ]),
-            AReg32('PUCRD',     0x038, [('PU0',         0),
-                                        ('PU1',         1),
-                                        ('PU2',         2),
-                                        ('PU3',         3),
-                                        ('PU4',         4),
-                                        ('PU5',         5),
-                                        ('PU6',         6),
-                                        ('PU7',         7),
-                                        ('PU8',         8),
-                                        ('PU9',         9),
-                                        ('PU10',        10),
-                                        ('PU11',        11),
-                                        ('PU12',        12),
-                                        ('PU13',        13),
-                                        ('PU14',        14),
-                                        ('PU15',        15),
-                                        ]),
-            AReg32('PDCRD',     0x03C, [('PD0',         0),
-                                        ('PD1',         1),
-                                        ('PD2',         2),
-                                        ('PD3',         3),
-                                        ('PD4',         4),
-                                        ('PD5',         5),
-                                        ('PD6',         6),
-                                        ('PD7',         7),
-                                        ('PD8',         8),
-                                        ('PD9',         9),
-                                        ('PD10',        10),
-                                        ('PD11',        11),
-                                        ('PD12',        12),
-                                        ('PD13',        13),
-                                        ('PD14',        14),
-                                        ('PD15',        15),
-                                        ]),
-            AReg32('PUCRE',     0x040, [('PU0',         0),
-                                        ('PU1',         1),
-                                        ('PU2',         2),
-                                        ('PU3',         3),
-                                        ('PU4',         4),
-                                        ('PU5',         5),
-                                        ('PU6',         6),
-                                        ('PU7',         7),
-                                        ('PU8',         8),
-                                        ('PU9',         9),
-                                        ('PU10',        10),
-                                        ('PU11',        11),
-                                        ('PU12',        12),
-                                        ('PU13',        13),
-                                        ('PU14',        14),
-                                        ('PU15',        15),
-                                        ]),
-            AReg32('PDCRE',     0x044, [('PD0',         0),
-                                        ('PD1',         1),
-                                        ('PD2',         2),
-                                        ('PD3',         3),
-                                        ('PD4',         4),
-                                        ('PD5',         5),
-                                        ('PD6',         6),
-                                        ('PD7',         7),
-                                        ('PD8',         8),
-                                        ('PD9',         9),
-                                        ('PD10',        10),
-                                        ('PD11',        11),
-                                        ('PD12',        12),
-                                        ('PD13',        13),
-                                        ('PD14',        14),
-                                        ('PD15',        15),
-                                        ]),
-            AReg32('PUCRF',     0x048, [('PU0',         0),
-                                        ('PU1',         1),
-                                        ('PU2',         2),
-                                        ('PU3',         3),
-                                        ('PU4',         4),
-                                        ('PU5',         5),
-                                        ('PU6',         6),
-                                        ('PU7',         7),
-                                        ('PU8',         8),
-                                        ('PU9',         9),
-                                        ('PU10',        10),
-                                        ('PU11',        11),
-                                        ('PU12',        12),
-                                        ('PU13',        13),
-                                        ('PU14',        14),
-                                        ('PU15',        15),
-                                        ]),
-            AReg32('PDCRF',     0x04C, [('PD0',         0),
-                                        ('PD1',         1),
-                                        ('PD2',         2),
-                                        ('PD3',         3),
-                                        ('PD4',         4),
-                                        ('PD5',         5),
-                                        ('PD6',         6),
-                                        ('PD7',         7),
-                                        ('PD8',         8),
-                                        ('PD9',         9),
-                                        ('PD10',        10),
-                                        ('PD11',        11),
-                                        ('PD12',        12),
-                                        ('PD13',        13),
-                                        ('PD14',        14),
-                                        ('PD15',        15),
-                                        ]),
-            AReg32('PUCRG',     0x050, [('PU0',         0),
-                                        ('PU1',         1),
-                                        ('PU2',         2),
-                                        ('PU3',         3),
-                                        ('PU4',         4),
-                                        ('PU5',         5),
-                                        ('PU6',         6),
-                                        ('PU7',         7),
-                                        ('PU8',         8),
-                                        ('PU9',         9),
-                                        ('PU10',        10),
-                                        # ('PU11',        11),
-                                        # ('PU12',        12),
-                                        # ('PU13',        13),
-                                        # ('PU14',        14),
-                                        # ('PU15',        15),
-                                        ]),
-            AReg32('PDCRG',     0x054, [('PD0',         0),
-                                        ('PD1',         1),
-                                        ('PD2',         2),
-                                        ('PD3',         3),
-                                        ('PD4',         4),
-                                        ('PD5',         5),
-                                        ('PD6',         6),
-                                        ('PD7',         7),
-                                        ('PD8',         8),
-                                        ('PD9',         9),
-                                        ('PD10',        10),
-                                        # ('PD11',        11),
-                                        # ('PD12',        12),
-                                        # ('PD13',        13),
-                                        # ('PD14',        14),
-                                        # ('PD15',        15),
-                                        ]),
-            AReg32('CR5',       0x080, [('R1MODE',      8),
-                                        ]),
+    REGS = [AReg32('CR1',           0x000, [('LPMS',            0,  2),
+                                            ('RRSB1',           5),
+                                            ('RRSB2',           6),
+                                            ('ULPMEN',          7),
+                                            ('SRAM1PD',         8),
+                                            ('SRAM2PD',         9),
+                                            ('SRAM3PD',         10),
+                                            ('SRAM4PD',         11),
+                                            ]),
+            AReg32('CR2',           0x004, [('SRAM1PDS1',       0),
+                                            ('SRAM1PDS2',       1),
+                                            ('SRAM1PDS3',       2),
+                                            ('SRAM2PDS1',       4),
+                                            ('SRAM2PDS2',       5),
+                                            ('SRAM4PDS',        6),
+                                            ('ICRAMPDS',        8),
+                                            ('DC1RAMPDS',       9),
+                                            ('DMA2DRAMPDS',     10),
+                                            ('PRAMPDS',         11),
+                                            ('PKARAMPDS',       12),
+                                            ('SRAM4FWU',        13),
+                                            ('FLASHFWU',        14),
+                                            ('SRAM3PDS1',       16),
+                                            ('SRAM3PDS2',       17),
+                                            ('SRAM3PDS3',       18),
+                                            ('SRAM3PDS4',       19),
+                                            ('SRAM3PDS5',       20),
+                                            ('SRAM3PDS6',       21),
+                                            ('SRAM3PDS7',       22),
+                                            ('SRAM3PDS8',       23),
+                                            ('SRDRUN',          31),
+                                            ]),
+            AReg32('CR3',           0x008, [('REGSEL',          1),
+                                            ('FSTEN',           2),
+                                            ]),
+            AReg32('VOSR',          0x00C, [('BOOSTRDY',        14),
+                                            ('VOSRDY',          15),
+                                            ('VOS',             16, 17),
+                                            ('BOOSTEN',         18),
+                                            ]),
+            AReg32('SVMCR',         0x010, [('PVDE',            4),
+                                            ('PVDLS',           5,  7),
+                                            ('UVMEN',           24),
+                                            ('IO2VMEN',         25),
+                                            ('AVM1EN',          26),
+                                            ('AVM2EN',          27),
+                                            ('USV',             28),
+                                            ('IO2SV',           29),
+                                            ('ASV',             30),
+                                            ]),
+            AReg32('WUCR1',         0x014, [('WUPEN1',          0),
+                                            ('WUPEN2',          1),
+                                            ('WUPEN3',          2),
+                                            ('WUPEN4',          3),
+                                            ('WUPEN5',          4),
+                                            ('WUPEN6',          5),
+                                            ('WUPEN7',          6),
+                                            ('WUPEN8',          7),
+                                            ]),
+            AReg32('WUCR2',         0x018, [('WUPP1',           0),
+                                            ('WUPP2',           1),
+                                            ('WUPP3',           2),
+                                            ('WUPP4',           3),
+                                            ('WUPP5',           4),
+                                            ('WUPP6',           5),
+                                            ('WUPP7',           6),
+                                            ('WUPP8',           7),
+                                            ]),
+            AReg32('WUCR3',         0x01C, [('WUSEL1',          0,  1),
+                                            ('WUSEL2',          2,  3),
+                                            ('WUSEL3',          4,  5),
+                                            ('WUSEL4',          6,  7),
+                                            ('WUSEL5',          8,  9),
+                                            ('WUSEL6',          10, 11),
+                                            ('WUSEL7',          12, 13),
+                                            ('WUSEL8',          14, 15),
+                                            ]),
+            AReg32('BDCR1',         0x020, [('BREN',            0),
+                                            ('MONEN',           4),
+                                            ]),
+            AReg32('BDCR2',         0x024, [('VBE',             0),
+                                            ('VBRS',            1),
+                                            ]),
+            AReg32('DBPR',          0x028, [('DBP',             0),
+                                            ]),
+            AReg32('UCPDR',         0x02C, [('UCPD_DBDIS',      0),
+                                            ('UCPD_STBY',       1),
+                                            ]),
+            AReg32('SECCFGR',       0x030, [('WUP1SEC',         0),
+                                            ('WUP2SEC',         1),
+                                            ('WUP3SEC',         2),
+                                            ('WUP4SEC',         3),
+                                            ('WUP5SEC',         4),
+                                            ('WUP6SEC',         5),
+                                            ('WUP7SEC',         6),
+                                            ('WUP8SEC',         7),
+                                            ('LPMSEC',          12),
+                                            ('VDMSEC',          13),
+                                            ('VBSEC',           14),
+                                            ('APCSEC',          15),
+                                            ]),
+            AReg32('PRIVCFGR',      0x034, [('SPRIV',           0),
+                                            ('NSPRIV',          1),
+                                            ]),
+            AReg32('SR',            0x038, [('CSSF',            0),
+                                            ('STOPF',           1),
+                                            ('SBF',             2),
+                                            ]),
+            AReg32('SVMSR',         0x03C, [('REGS',            1),
+                                            ('PVDO',            4),
+                                            ('ACTVOSRDY',       15),
+                                            ('ACTVOS',          16, 17),
+                                            ('VDDUSBRDY',       24),
+                                            ('VDDIO2RDY',       25),
+                                            ('VDDA1RDY',        26),
+                                            ('VDDA2RDY',        27),
+                                            ]),
+            AReg32('BDSR',          0x040, [('VBATH',           1),
+                                            ('TEMPL',           2),
+                                            ('TEMPH',           3),
+                                            ]),
+            AReg32('WUSR',          0x044, [('WUF1',            0),
+                                            ('WUF2',            1),
+                                            ('WUF3',            2),
+                                            ('WUF4',            3),
+                                            ('WUF5',            4),
+                                            ('WUF6',            5),
+                                            ('WUF7',            6),
+                                            ('WUF8',            7),
+                                            ]),
+            AReg32('WUSCR',         0x048, [('CWUF1',           0),
+                                            ('CWUF2',           1),
+                                            ('CWUF3',           2),
+                                            ('CWUF4',           3),
+                                            ('CWUF5',           4),
+                                            ('CWUF6',           5),
+                                            ('CWUF7',           6),
+                                            ('CWUF8',           7),
+                                            ]),
+            AReg32('APCR',          0x04C, [('APC',             0),
+                                            ]),
+            AReg32('PUCRA',         0x050, [('PU0',             0),
+                                            ('PU1',             1),
+                                            ('PU2',             2),
+                                            ('PU3',             3),
+                                            ('PU4',             4),
+                                            ('PU5',             5),
+                                            ('PU6',             6),
+                                            ('PU7',             7),
+                                            ('PU8',             8),
+                                            ('PU9',             9),
+                                            ('PU10',            10),
+                                            ('PU11',            11),
+                                            ('PU12',            12),
+                                            ('PU13',            13),
+                                            ('PU15',            15),
+                                            ]),
+            AReg32('PDCRA',         0x054, [('PD0',             0),
+                                            ('PD1',             1),
+                                            ('PD2',             2),
+                                            ('PD3',             3),
+                                            ('PD4',             4),
+                                            ('PD5',             5),
+                                            ('PD6',             6),
+                                            ('PD7',             7),
+                                            ('PD8',             8),
+                                            ('PD9',             9),
+                                            ('PD10',            10),
+                                            ('PD11',            11),
+                                            ('PD12',            12),
+                                            ('PD14',            14),
+                                            ]),
+            AReg32('PUCRB',         0x058, [('PU0',             0),
+                                            ('PU1',             1),
+                                            ('PU2',             2),
+                                            ('PU3',             3),
+                                            ('PU4',             4),
+                                            ('PU5',             5),
+                                            ('PU6',             6),
+                                            ('PU7',             7),
+                                            ('PU8',             8),
+                                            ('PU9',             9),
+                                            ('PU10',            10),
+                                            ('PU11',            11),
+                                            ('PU12',            12),
+                                            ('PU13',            13),
+                                            ('PU14',            14),
+                                            ('PU15',            15),
+                                            ]),
+            AReg32('PDCRB',         0x05C, [('PD0',             0),
+                                            ('PD1',             1),
+                                            ('PD2',             2),
+                                            ('PD3',             3),
+                                            ('PD5',             5),
+                                            ('PD6',             6),
+                                            ('PD7',             7),
+                                            ('PD8',             8),
+                                            ('PD9',             9),
+                                            ('PD10',            10),
+                                            ('PD11',            11),
+                                            ('PD12',            12),
+                                            ('PD13',            13),
+                                            ('PD14',            14),
+                                            ('PD15',            15),
+                                            ]),
+            AReg32('PUCRC',         0x060, [('PU0',             0),
+                                            ('PU1',             1),
+                                            ('PU2',             2),
+                                            ('PU3',             3),
+                                            ('PU4',             4),
+                                            ('PU5',             5),
+                                            ('PU6',             6),
+                                            ('PU7',             7),
+                                            ('PU8',             8),
+                                            ('PU9',             9),
+                                            ('PU10',            10),
+                                            ('PU11',            11),
+                                            ('PU12',            12),
+                                            ('PU13',            13),
+                                            ('PU14',            14),
+                                            ('PU15',            15),
+                                            ]),
+            AReg32('PDCRC',         0x064, [('PD0',             0),
+                                            ('PD1',             1),
+                                            ('PD2',             2),
+                                            ('PD3',             3),
+                                            ('PD4',             4),
+                                            ('PD5',             5),
+                                            ('PD6',             6),
+                                            ('PD7',             7),
+                                            ('PD8',             8),
+                                            ('PD9',             9),
+                                            ('PD10',            10),
+                                            ('PD11',            11),
+                                            ('PD12',            12),
+                                            ('PD13',            13),
+                                            ('PD14',            14),
+                                            ('PD15',            15),
+                                            ]),
+            AReg32('PUCRD',         0x068, [('PU0',             0),
+                                            ('PU1',             1),
+                                            ('PU2',             2),
+                                            ('PU3',             3),
+                                            ('PU4',             4),
+                                            ('PU5',             5),
+                                            ('PU6',             6),
+                                            ('PU7',             7),
+                                            ('PU8',             8),
+                                            ('PU9',             9),
+                                            ('PU10',            10),
+                                            ('PU11',            11),
+                                            ('PU12',            12),
+                                            ('PU13',            13),
+                                            ('PU14',            14),
+                                            ('PU15',            15),
+                                            ]),
+            AReg32('PDCRD',         0x06C, [('PD0',             0),
+                                            ('PD1',             1),
+                                            ('PD2',             2),
+                                            ('PD3',             3),
+                                            ('PD4',             4),
+                                            ('PD5',             5),
+                                            ('PD6',             6),
+                                            ('PD7',             7),
+                                            ('PD8',             8),
+                                            ('PD9',             9),
+                                            ('PD10',            10),
+                                            ('PD11',            11),
+                                            ('PD12',            12),
+                                            ('PD13',            13),
+                                            ('PD14',            14),
+                                            ('PD15',            15),
+                                            ]),
+            AReg32('PUCRE',         0x070, [('PU0',             0),
+                                            ('PU1',             1),
+                                            ('PU2',             2),
+                                            ('PU3',             3),
+                                            ('PU4',             4),
+                                            ('PU5',             5),
+                                            ('PU6',             6),
+                                            ('PU7',             7),
+                                            ('PU8',             8),
+                                            ('PU9',             9),
+                                            ('PU10',            10),
+                                            ('PU11',            11),
+                                            ('PU12',            12),
+                                            ('PU13',            13),
+                                            ('PU14',            14),
+                                            ('PU15',            15),
+                                            ]),
+            AReg32('PDCRE',         0x074, [('PD0',             0),
+                                            ('PD1',             1),
+                                            ('PD2',             2),
+                                            ('PD3',             3),
+                                            ('PD4',             4),
+                                            ('PD5',             5),
+                                            ('PD6',             6),
+                                            ('PD7',             7),
+                                            ('PD8',             8),
+                                            ('PD9',             9),
+                                            ('PD10',            10),
+                                            ('PD11',            11),
+                                            ('PD12',            12),
+                                            ('PD13',            13),
+                                            ('PD14',            14),
+                                            ('PD15',            15),
+                                            ]),
+            AReg32('PUCRF',         0x078, [('PU0',             0),
+                                            ('PU1',             1),
+                                            ('PU2',             2),
+                                            ('PU3',             3),
+                                            ('PU4',             4),
+                                            ('PU5',             5),
+                                            ('PU6',             6),
+                                            ('PU7',             7),
+                                            ('PU8',             8),
+                                            ('PU9',             9),
+                                            ('PU10',            10),
+                                            ('PU11',            11),
+                                            ('PU12',            12),
+                                            ('PU13',            13),
+                                            ('PU14',            14),
+                                            ('PU15',            15),
+                                            ]),
+            AReg32('PDCRF',         0x07C, [('PD0',             0),
+                                            ('PD1',             1),
+                                            ('PD2',             2),
+                                            ('PD3',             3),
+                                            ('PD4',             4),
+                                            ('PD5',             5),
+                                            ('PD6',             6),
+                                            ('PD7',             7),
+                                            ('PD8',             8),
+                                            ('PD9',             9),
+                                            ('PD10',            10),
+                                            ('PD11',            11),
+                                            ('PD12',            12),
+                                            ('PD13',            13),
+                                            ('PD14',            14),
+                                            ('PD15',            15),
+                                            ]),
+            AReg32('PUCRG',         0x080, [('PU0',             0),
+                                            ('PU1',             1),
+                                            ('PU2',             2),
+                                            ('PU3',             3),
+                                            ('PU4',             4),
+                                            ('PU5',             5),
+                                            ('PU6',             6),
+                                            ('PU7',             7),
+                                            ('PU8',             8),
+                                            ('PU9',             9),
+                                            ('PU10',            10),
+                                            ('PU11',            11),
+                                            ('PU12',            12),
+                                            ('PU13',            13),
+                                            ('PU14',            14),
+                                            ('PU15',            15),
+                                            ]),
+            AReg32('PDCRG',         0x084, [('PD0',             0),
+                                            ('PD1',             1),
+                                            ('PD2',             2),
+                                            ('PD3',             3),
+                                            ('PD4',             4),
+                                            ('PD5',             5),
+                                            ('PD6',             6),
+                                            ('PD7',             7),
+                                            ('PD8',             8),
+                                            ('PD9',             9),
+                                            ('PD10',            10),
+                                            ('PD11',            11),
+                                            ('PD12',            12),
+                                            ('PD13',            13),
+                                            ('PD14',            14),
+                                            ('PD15',            15),
+                                            ]),
+            AReg32('PUCRH',         0x088, [('PU0',             0),
+                                            ('PU1',             1),
+                                            ('PU2',             2),
+                                            ('PU3',             3),
+                                            ('PU4',             4),
+                                            ('PU5',             5),
+                                            ('PU6',             6),
+                                            ('PU7',             7),
+                                            ('PU8',             8),
+                                            ('PU9',             9),
+                                            ('PU10',            10),
+                                            ('PU11',            11),
+                                            ('PU12',            12),
+                                            ('PU13',            13),
+                                            ('PU14',            14),
+                                            ('PU15',            15),
+                                            ]),
+            AReg32('PDCRH',         0x08C, [('PD0',             0),
+                                            ('PD1',             1),
+                                            ('PD2',             2),
+                                            ('PD3',             3),
+                                            ('PD4',             4),
+                                            ('PD5',             5),
+                                            ('PD6',             6),
+                                            ('PD7',             7),
+                                            ('PD8',             8),
+                                            ('PD9',             9),
+                                            ('PD10',            10),
+                                            ('PD11',            11),
+                                            ('PD12',            12),
+                                            ('PD13',            13),
+                                            ('PD14',            14),
+                                            ('PD15',            15),
+                                            ]),
+            AReg32('PUCRI',         0x090, [('PU0',             0),
+                                            ('PU1',             1),
+                                            ('PU2',             2),
+                                            ('PU3',             3),
+                                            ('PU4',             4),
+                                            ('PU5',             5),
+                                            ('PU6',             6),
+                                            ('PU7',             7),
+                                            ]),
+            AReg32('PDCRI',         0x094, [('PD0',             0),
+                                            ('PD1',             1),
+                                            ('PD2',             2),
+                                            ('PD3',             3),
+                                            ('PD4',             4),
+                                            ('PD5',             5),
+                                            ('PD6',             6),
+                                            ('PD7',             7),
+                                            ]),
             ]
 
     def __init__(self, target, ap, name, addr, **kwargs):
         super().__init__(target, ap, addr, name, PWR.REGS, **kwargs)
 
     def unlock_backup_domain(self):
-        self._CR1.DBP = 1
-        while self._CR1.DBP == 0:
-            time.sleep(0.01)
-
-    def wait_vosf_ready(self):
-        while self._SR2.VOSF == 1:
+        self._DBPR.DBP = 1
+        while self._DBPR.DBP == 0:
             time.sleep(0.01)
-
-    def set_vcore_voltage(self, vcv):
-        if vcv == self.VCORE_1V00:
-            self._CR5.R1MODE = 1
-            self.wait_vosf_ready()
-            self._CR1.VOS = 2
-        elif vcv == self.VCORE_1V20:
-            self._CR5.R1MODE = 1
-            self.wait_vosf_ready()
-            self._CR1.VOS = 1
-        elif vcv == self.VCORE_1V28:
-            self._CR1.VOS = 1
-            self.wait_vosf_ready()
-            self._CR5.R1MODE = 0
-        else:
-            raise Exception('Invalid vcore voltage %s' % vcv)
-
-        self.wait_vosf_ready()
```

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/rcc.py` & `psdb-1.1.3/psdb/devices/stm32g4/rcc.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/rtc.py` & `psdb-1.1.3/psdb/devices/stm32g4/rtc.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/syscfg.py` & `psdb-1.1.3/psdb/devices/stm32g4/syscfg.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32g4/tamp.py` & `psdb-1.1.3/psdb/devices/stm32g4/tamp.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/__init__.py` & `psdb-1.1.3/psdb/devices/stm32h7/__init__.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/art.py` & `psdb-1.1.3/psdb/devices/stm32h7/art.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/flash.py` & `psdb-1.1.3/psdb/devices/stm32h7/flash.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/flash_dp.py` & `psdb-1.1.3/psdb/devices/stm32h7/flash_dp.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/flash_up.py` & `psdb-1.1.3/psdb/devices/stm32h7/flash_up.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/opamp.py` & `psdb-1.1.3/psdb/devices/stm32h7/opamp.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/pwr.py` & `psdb-1.1.3/psdb/devices/stm32h7/pwr.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/rcc.py` & `psdb-1.1.3/psdb/devices/stm32h7/rcc.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/syscfg.py` & `psdb-1.1.3/psdb/devices/stm32h7/syscfg.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/tim15.py` & `psdb-1.1.3/psdb/devices/stm32h7/tim15.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/tim17.py` & `psdb-1.1.3/psdb/devices/stm32h7/tim17.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/tim2_5.py` & `psdb-1.1.3/psdb/devices/stm32h7/tim2_5.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32h7/tim6.py` & `psdb-1.1.3/psdb/devices/stm32h7/tim6.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32u5/dbgmcu.py` & `psdb-1.1.3/psdb/devices/stm32u5/dbgmcu.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32u5/flash.py` & `psdb-1.1.3/psdb/devices/stm32u5/flash.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32u5/i2c.py` & `psdb-1.1.3/psdb/devices/stm32u5/i2c.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32u5/rcc.py` & `psdb-1.1.3/psdb/devices/stm32u5/rcc.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32u5/rtc.py` & `psdb-1.1.3/psdb/devices/stm32u5/rtc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # Copyright (c) 2020-2023 Phase Advanced Sensor Systems, Inc.
-import time
-import datetime
-
 from ..device import Device, AReg32
 
 
 class UnlockedContextManager:
     def __init__(self, rtc):
         self.rtc = rtc
```

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/flash.py` & `psdb-1.1.3/psdb/devices/stm32wb55/flash.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/__init__.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/__init__.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/binaries.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/binaries.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/ble_channel.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/ble_channel.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/circular_queue.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/circular_queue.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/fus_client.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/fus_client.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/gatt.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/gatt.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/ipc.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/ipc.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/mailbox.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/mailbox.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/mm_channel.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/mm_channel.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/packet.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/packet.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/system_channel.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/system_channel.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/ws_client.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/ws_client.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipc/ws_factory.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipc/ws_factory.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/ipcc.py` & `psdb-1.1.3/psdb/devices/stm32wb55/ipcc.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/pwr.py` & `psdb-1.1.3/psdb/devices/stm32wb55/pwr.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/devices/stm32wb55/rcc.py` & `psdb-1.1.3/psdb/devices/stm32wb55/rcc.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/dump_stats.py` & `psdb-1.1.3/psdb/dump_stats.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/elf/core.py` & `psdb-1.1.3/psdb/elf/core.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/elf/dv.py` & `psdb-1.1.3/psdb/elf/dv.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/elf/elf_binary.py` & `psdb-1.1.3/psdb/elf/elf_binary.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/elf/note.py` & `psdb-1.1.3/psdb/elf/note.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/flash_tool.py` & `psdb-1.1.3/psdb/flash_tool.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/fus_tool.py` & `psdb-1.1.3/psdb/fus_tool.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/gdb_tool.py` & `psdb-1.1.3/psdb/gdb_tool.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/hexfile/hexfile.py` & `psdb-1.1.3/psdb/hexfile/hexfile.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/inspect_tool/cpu_register_window.py` & `psdb-1.1.3/psdb/inspect_tool/cpu_register_window.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/inspect_tool/device_decode_window.py` & `psdb-1.1.3/psdb/inspect_tool/device_decode_window.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/inspect_tool/device_register_window.py` & `psdb-1.1.3/psdb/inspect_tool/device_register_window.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/inspect_tool/device_selector_window.py` & `psdb-1.1.3/psdb/inspect_tool/device_selector_window.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/inspect_tool/inspect_tool.py` & `psdb-1.1.3/psdb/inspect_tool/inspect_tool.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/inspect_tool/memory_window.py` & `psdb-1.1.3/psdb/inspect_tool/memory_window.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/mem_ap_test.py` & `psdb-1.1.3/psdb/mem_ap_test.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/__init__.py` & `psdb-1.1.3/psdb/probes/__init__.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/probe.py` & `psdb-1.1.3/psdb/probes/probe.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/stlink/__init__.py` & `psdb-1.1.3/psdb/probes/stlink/__init__.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/stlink/cdb.py` & `psdb-1.1.3/psdb/probes/stlink/cdb.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/stlink/errors.py` & `psdb-1.1.3/psdb/probes/stlink/errors.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/stlink/stlink.py` & `psdb-1.1.3/psdb/probes/stlink/stlink.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/stlink/stlink_v2_1.py` & `psdb-1.1.3/psdb/probes/stlink/stlink_v2_1.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/stlink/stlink_v3.py` & `psdb-1.1.3/psdb/probes/stlink/stlink_v3.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/usb_probe.py` & `psdb-1.1.3/psdb/probes/usb_probe.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/xds110/xds110.py` & `psdb-1.1.3/psdb/probes/xds110/xds110.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/xtswd/abort_test.py` & `psdb-1.1.3/psdb/probes/xtswd/abort_test.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/xtswd/imon.py` & `psdb-1.1.3/psdb/probes/xtswd/imon.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/xtswd/plot_imon.py` & `psdb-1.1.3/psdb/probes/xtswd/plot_imon.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/probes/xtswd/xtswd.py` & `psdb-1.1.3/psdb/probes/xtswd/xtswd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2022 Phase Advanced Sensor Systems, Inc.
 from enum import IntEnum
 import random
 import usb.core
 import usb.util
 
 import btype
+import numpy as np
 
 import psdb
 from .. import usb_probe
 
 
 TRACE_EN   = False
 
@@ -52,14 +53,15 @@
     CONNECT     = 0x02
     SET_SRST    = 0x03
     ENABLE_INA  = 0x04
     DISABLE_INA = 0x05
     START_IMON  = 0x06
     STOP_IMON   = 0x07
     GET_STATS   = 0x08
+    SET_DDRIVE  = 0x09
     READ_DP     = 0x10
     WRITE_DP    = 0x11
     READ_AP     = 0x20
     WRITE_AP    = 0x21
     READ8       = 0x30
     WRITE8      = 0x31
     READ16      = 0x32
@@ -82,14 +84,22 @@
     opcode         = btype.uint16_t()
     tag            = btype.uint16_t()
     status         = btype.uint32_t()
     params         = btype.Array(btype.uint32_t(), 6)
     _EXPECTED_SIZE = 32
 
 
+class IMonSettings:
+    def __init__(self, calfact, f_numerator, f_denominator):
+        self.calfact       = calfact
+        self.f_numerator   = f_numerator
+        self.f_denominator = f_denominator
+        self.f             = f_numerator / f_denominator
+
+
 class IMonData(btype.Struct):
     tag             = btype.uint16_t()
     oversample_log2 = btype.uint8_t()
     rsrv            = btype.uint8_t()
     seq             = btype.uint32_t()
     freq_num        = btype.uint32_t()
     freq_denom      = btype.uint32_t()
@@ -250,41 +260,44 @@
 
     def enable_instrumentation_amp(self):
         self._exec_command(Opcode.ENABLE_INA)
 
     def disable_instrumentation_amp(self):
         self._exec_command(Opcode.DISABLE_INA)
 
-    def start_current_monitoring(self):
-        rsp, _ = self._exec_command(Opcode.START_IMON)
+    def start_current_monitoring(self, calfact=0):
+        rsp, _ = self._exec_command(Opcode.START_IMON, [calfact])
         self.imon_tag = rsp.tag
+        return IMonSettings(rsp.params[0], rsp.params[1], rsp.params[2])
 
     def stop_current_monitoring(self):
         self._exec_command(Opcode.STOP_IMON)
 
-    def read_current_monitor_data(self):
+    def read_current_monitor_raw_data(self):
         while True:
             data = self.usb_dev.read(self.IMON_EP, IMonData._STRUCT.size,
                                      timeout=1000)
             idata = IMonData.unpack(data)
             if idata.tag == self.imon_tag:
                 return idata, data[-20000:]
 
+    def read_current_monitor_data(self):
+        idata, _ = self.read_current_monitor_raw_data()
+        ovr      = (1 << idata.oversample_log2)
+        V        = np.array(idata.samples)
+        V        = V / ovr
+        V        = (53.8206644205 + 10.6461162703 * V) / 1000
+        return idata, V
+
     def read_current_consumption(self):
-        while True:
-            data = self.usb_dev.read(self.IMON_EP, IMonData._STRUCT.size,
-                                     timeout=1000)
-            idata = IMonData.unpack(data)
-            if idata.tag == self.imon_tag:
-                break
+        _, V = self.read_current_monitor_data()
+        return sum(V) / len(V)
 
-        ovr  = (1 << idata.oversample_log2)
-        vals = [v / ovr for v in idata.samples]
-        vals = [v / MA_RATIO for v in vals]
-        return sum(vals) / len(vals)
+    def set_dac_drive(self, dac):
+        self._exec_command(Opcode.SET_DDRIVE, [dac])
 
     def get_stats(self):
         rsp, _ = self._exec_command(Opcode.GET_STATS)
         return Stats(rsp)
 
     def open_ap(self, ap_num):
         pass
```

### Comparing `psdb-1.1.2/psdb/reg_dump_tool.py` & `psdb-1.1.3/psdb/reg_dump_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 def _main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--dump-debuggers', '-d', action='store_true')
     parser.add_argument('--usb-path')
     parser.add_argument('--serial-num')
     parser.add_argument('--halt', action='store_true')
     parser.add_argument('--probe-freq', type=int, default=1000000)
+    parser.add_argument('--max-tck-freq', type=int)
     parser.add_argument('--verbose', '-v', action='store_true')
     parser.add_argument('--output-path', '-o', required=True)
     rv = parser.parse_args()
 
     try:
         main(rv)
     except psdb.ProbeException as e:
```

### Comparing `psdb-1.1.2/psdb/scan_tool.py` & `psdb-1.1.3/psdb/scan_tool.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/srst_tool.py` & `psdb-1.1.3/psdb/srst_tool.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/targets/msp432/msp432.py` & `psdb-1.1.3/psdb/targets/msp432/msp432.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/targets/stm32g0/stm32g0.py` & `psdb-1.1.3/psdb/targets/stm32l4/stm32l4.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,94 @@
-# Copyright (c) 2020 by Phase Advanced Sensor Systems, Inc.
+# Copyright (c) 2019-2024 Phase Advanced Sensor Systems, Inc.
 import psdb
-from psdb.devices import MemDevice, RAMDevice, stm32g0
+from psdb.devices import MemDevice, RAMDevice, stm32l4
 from psdb.targets import Target
+from . import dbgmcu
 
 
-# Verified with Nucleo-G071RB and V2J39S27 that flash writes work at 4 MHz, the
-# fastest speed available on the STLINK-V2E debugger.
-DEVICES = [
-           (stm32g0.FLASH,  'FLASH',    0x40022000, 0x08000000, 4000000,
-                                        0x1FFF7000, 1024),  # noqa: E127
+DEVICES = [(RAMDevice,      'SRAM2 S', 0x10000000, 0x00002000),
+           (RAMDevice,      'SRAM1',   0x20000000, 0x00008000),
+           (RAMDevice,      'SRAM2',   0x20008000, 0x00002000),
+           (stm32l4.FLASH,  'FLASH',   0x40022000, 0x08000000, 4000000,
+                                       0x1FFF7000, 1024),  # noqa: E127
            ]
 
 
-class STM32G0(Target):
+class STM32L4(Target):
     def __init__(self, db):
         # Max SWD speed is not specified in the data sheet.
         super().__init__(db, 24000000)
         self.ahb_ap     = self.db.aps[0]
         self.uuid       = self.ahb_ap.read_bulk(0x1FFF7590, 12)
         self.flash_size = (self.ahb_ap.read_32(0x1FFF75E0) & 0x0000FFFF)*1024
-        self.package    = self.ahb_ap.read_32(0x1FFF7500) & 0x0000000F
-        self.mcu_idcode = self.ahb_ap.read_32(0x40015800)
+        self.package    = self.ahb_ap.read_32(0x1FFF7500) & 0x0000001F
+        self.mcu_idcode = self.ahb_ap.read_32(0xE0042000)
 
         for d in DEVICES:
             cls  = d[0]
             name = d[1]
             addr = d[2]
             args = d[3:]
             cls(self, self.ahb_ap, name, addr, *args)
 
         self.flash = self.devs['FLASH']
-
-        dev_id = (self.mcu_idcode & 0x0FFF)
-        if dev_id == 0x460:
-            # STM32G071xx and STM32G081xx
-            if self.flash._OPTR.RAM_PARITY_CHECK:
-                # Parity check disabled if RAM_PARITY_CHECK=1
-                sram_len = 36 * 1024
-            else:
-                # Parity check enabled if RAM_PARITY_CHECK=0
-                sram_len = 32 * 1024
-        elif dev_id == 0x466:
-            # STM32G031xx and STM32G041xx
-            sram_len = 8 * 1024
-
-        RAMDevice(self, self.ahb_ap, 'SRAM', 0x20000000, sram_len)
         MemDevice(self, self.ahb_ap, 'FBANKS', self.flash.mem_base,
                   self.flash.flash_size)
         MemDevice(self, self.ahb_ap, 'OTP', self.flash.otp_base,
                   self.flash.otp_len)
 
     def __repr__(self):
-        return 'STM32G0 MCU_IDCODE 0x%08X' % self.mcu_idcode
+        return 'STM32L4 MCU_IDCODE 0x%08X' % self.mcu_idcode
 
     @staticmethod
-    def probe(db):
-        # APSEL 0 should be populated.
-        if 0 not in db.aps:
-            return None
+    def is_mcu(db):
+        # Only APSEL 0 should be populated.
+        if set(db.aps) != set((0,)):
+            return False
 
         # APSEL 0 should be an AHB3 AP.
         ap = db.aps[0]
         if not isinstance(ap, psdb.access_port.AHB3AP):
-            return None
+            return False
 
-        # Identify the STM32G0 through the base component's CIDR/PIDR
+        # Identify the STM32L4 through the base component's CIDR/PIDR
         # registers.
         c = db.aps[0].base_component
-        if not c or c.cidr != 0xB105100D or c.pidr != 0x00000000000A0460:
+        if not c:
+            c = db.aps[0].probe_components(match=False, recurse=False)
+        if not c:
+            return False
+        if c.cidr != 0xB105100D:
+            return False
+        if c.pidr != 0xA0464:
+            return False
+
+        # Finally, we can match on the DBGMCU IDC value.
+        if dbgmcu.read_idc_dev_id(db) != 0x464:
+            return False
+
+        return True
+
+    @staticmethod
+    def pre_probe(db, verbose):
+        # Ensure this is an STM32L4 part.
+        if not STM32L4.is_mcu(db):
+            return
+
+        # Enable all the clocks we want to use.
+        cr = dbgmcu.read_cr(db)
+        if (cr & 0x00000007) != 0x00000007:
+            if verbose:
+                print('Detected STM32L4, enabling all DBGMCU debug clocks.')
+            dbgmcu.write_cr(db, cr | 0x00000007)
+
+    @staticmethod
+    def probe(db):
+        # Ensure this is an STM32L4 part.
+        if not STM32L4.is_mcu(db):
             return None
 
         # There should be exactly one CPU.
         if len(db.cpus) != 1:
             return None
 
-        return STM32G0(db)
+        return STM32L4(db)
```

### Comparing `psdb-1.1.2/psdb/targets/stm32g4/stm32g4.py` & `psdb-1.1.3/psdb/targets/stm32g4/stm32g4.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/targets/stm32h7/dbgmcu.py` & `psdb-1.1.3/psdb/targets/stm32h7/dbgmcu.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/targets/stm32h7/stm32h7.py` & `psdb-1.1.3/psdb/targets/stm32h7/stm32h7.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/targets/stm32h7/stm32h7_dp.py` & `psdb-1.1.3/psdb/targets/stm32h7/stm32h7_dp.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb/targets/stm32u5/stm32u5.py` & `psdb-1.1.3/psdb/targets/stm32u5/stm32u5.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
            (stm32.GPIO,      'GPIOI',       0x42022000),
            (stm32.ADC14,     'ADC1',        0x42028000, 1, 1),
            (stm32.USB_HS,    'USB1',        0x42040000),
            (stm32u5.I2C,     'I2C3',        0x46002800),
            (stm32u5.RTC,     'RTC',         0x46007800),
            (stm32u5.PWR,     'PWR',         0x46020800),
            (stm32u5.RCC,     'RCC',         0x46020C00),
+           (stm32.ADC12,     'ADC4',        0x46021000, 4, 1),
            (stm32.DAC,       'DAC',         0x46021800),
            (stm32.GPDMA,     'GPDMA',       0x50020000),
            (stm32u5.DBGMCU,  'DBGMCU',      0xE0044000),
            ]
 
 
 class STM32U5MCU(psdb.component.Component):
```

### Comparing `psdb-1.1.2/psdb/targets/stm32wb55/stm32wb55.py` & `psdb-1.1.3/psdb/targets/stm32wb55/stm32wb55.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2020 by Phase Advanced Sensor Systems, Inc.
 import struct
 
 import psdb
 from psdb.devices.stm32wb55.ipc import IPC
 from psdb.devices import MemDevice, RAMDevice, stm32, stm32wb55
 from psdb.targets import Target
+from . import dbgmcu
 
 
 DEVICES = [(RAMDevice,        'SRAM1',    0x20000000, 0x00030000),
            (RAMDevice,        'SRAM2a',   0x20030000, 0x00008000),
            (RAMDevice,        'SRAM2b',   0x20038000, 0x00008000),
            (stm32.GPT32,      'TIM2',     0x40000000),
            (stm32.USB,        'USB',      0x40006800),
@@ -149,29 +150,63 @@
         rcc.set_usart1clock_source(0)
         rcc.set_lpuartclock_source(0)
         rcc.set_rfwakeupclock_source(1)
         rcc.set_smps_div(1)
         rcc.set_smpsclock_source(2)
 
     @staticmethod
-    def probe(db):
-        # APSEL 0 and 1 should be populated and be AHB3 APs.
-        for i in range(2):
-            if i not in db.aps:
-                return None
-
-            ap = db.aps[i]
-            if not isinstance(ap, psdb.access_port.AHB3AP):
-                return None
+    def is_mcu(db):
+        # APSEL 0 should be populated.
+        if set(db.aps) != set((0, 1)):
+            return False
+
+        # APSEL 0 and 1 should be AHB3 APs.
+        ap = db.aps[0]
+        if not isinstance(ap, psdb.access_port.AHB3AP):
+            return False
+        ap = db.aps[1]
+        if not isinstance(ap, psdb.access_port.AHB3AP):
+            return False
 
         # Identify the STM32WB55 through the base component's CIDR/PIDR
         # registers.
         c = db.aps[0].base_component
-        if not c or c.cidr != 0xB105100D or c.pidr != 0x00000000000A0495:
-            return None
+        if not c:
+            c = db.aps[0].probe_components(match=False, recurse=False)
+        if not c:
+            return False
+        if c.cidr != 0xB105100D:
+            return False
+        if c.pidr != 0xA0495:
+            return False
+
+        # Finally, we can match on the DBGMCU IDC value.
+        if dbgmcu.read_idc_dev_id(db) != 0x495:
+            return False
+
+        return True
+
+    @staticmethod
+    def pre_probe(db, verbose):
+        # Ensure this is an STM32WB55 part.
+        if not STM32WB55.is_mcu(db):
+            return
+
+        # Enable all the clocks we want to use.
+        cr = dbgmcu.read_cr(db)
+        if (cr & 0x00000007) != 0x00000007:
+            if verbose:
+                print('Detected STM32WB55, enabling all DBGMCU debug clocks.')
+            dbgmcu.write_cr(db, cr | 0x00000007)
+
+    @staticmethod
+    def probe(db):
+        # Ensure this is an STM32WB55 part.
+        if not STM32WB55.is_mcu(db):
+            return
 
         # While the STM32WB55 has two CPUs, the second one is inaccessible due
         # to ST security.
         if len(db.cpus) != 1:
             return None
 
         return STM32WB55(db)
```

### Comparing `psdb-1.1.2/psdb/targets/target.py` & `psdb-1.1.3/psdb/targets/target.py`

 * *Files 12% similar despite different names*

```diff
@@ -90,18 +90,19 @@
             c.enable_reset_vector_catch()
 
     def disable_reset_vector_catch(self):
         for c in self.cpus:
             c.disable_reset_vector_catch()
 
     def wait_reset(self):
-        # Wait for the initial disconnect.
+        # Wait for the initial disconnect.  We detect this be either getting an
+        # exception (most targets) or reading a 0 for the CPUID (STM32G0,
+        # STM32C0).
         try:
-            while True:
-                self.cpus[0].scs.read_cpuid()
+            while self.cpus[0].scs.read_cpuid():
                 time.sleep(0.1)
         except psdb.ProbeException:
             time.sleep(0.1)
 
     def wait_reset_and_reprobe(self, **kwargs):
         self.wait_reset()
         return self.reprobe(**kwargs)
```

### Comparing `psdb-1.1.2/psdb/util/prange.py` & `psdb-1.1.3/psdb/util/prange.py`

 * *Files identical despite different names*

### Comparing `psdb-1.1.2/psdb.egg-info/PKG-INFO` & `psdb-1.1.3/psdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdb
-Version: 1.1.2
+Version: 1.1.3
 Summary: Package for interfacing with ARM-compatible debug probes
 Home-page: https://github.com/tgree/psdb
 Author: Terry Greeniaus
 Author-email: terrygreeniaus@gmail.com
 License: LGPLv2
 Keywords: stlink xds110 arm swd fus stm32 msp432
 Classifier: Operating System :: OS Independent
```

### Comparing `psdb-1.1.2/psdb.egg-info/SOURCES.txt` & `psdb-1.1.3/psdb.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 psdb/devices/core/scs_v7_m.py
 psdb/devices/core/scs_v8_m.py
 psdb/devices/core/tpiu_m4.py
 psdb/devices/msp432/__init__.py
 psdb/devices/msp432/flctl.py
 psdb/devices/stm32/__init__.py
 psdb/devices/stm32/adc.py
+psdb/devices/stm32/adc_12.py
 psdb/devices/stm32/adc_14.py
 psdb/devices/stm32/adc_16.py
 psdb/devices/stm32/advanced_control_timer.py
 psdb/devices/stm32/basic_timer.py
 psdb/devices/stm32/cordic.py
 psdb/devices/stm32/crs.py
 psdb/devices/stm32/dac.py
@@ -72,14 +73,16 @@
 psdb/devices/stm32/gpdma.py
 psdb/devices/stm32/gpio.py
 psdb/devices/stm32/lpuart.py
 psdb/devices/stm32/qspi.py
 psdb/devices/stm32/usb.py
 psdb/devices/stm32/usb_hs.py
 psdb/devices/stm32/vrefbuf.py
+psdb/devices/stm32c0/__init__.py
+psdb/devices/stm32c0/flash.py
 psdb/devices/stm32g0/__init__.py
 psdb/devices/stm32g0/flash.py
 psdb/devices/stm32g4/__init__.py
 psdb/devices/stm32g4/comparator.py
 psdb/devices/stm32g4/dbgmcu.py
 psdb/devices/stm32g4/flash_2.py
 psdb/devices/stm32g4/flash_3.py
@@ -99,14 +102,16 @@
 psdb/devices/stm32h7/pwr.py
 psdb/devices/stm32h7/rcc.py
 psdb/devices/stm32h7/syscfg.py
 psdb/devices/stm32h7/tim15.py
 psdb/devices/stm32h7/tim17.py
 psdb/devices/stm32h7/tim2_5.py
 psdb/devices/stm32h7/tim6.py
+psdb/devices/stm32l4/__init__.py
+psdb/devices/stm32l4/flash.py
 psdb/devices/stm32u5/__init__.py
 psdb/devices/stm32u5/dbgmcu.py
 psdb/devices/stm32u5/flash.py
 psdb/devices/stm32u5/i2c.py
 psdb/devices/stm32u5/pwr.py
 psdb/devices/stm32u5/rcc.py
 psdb/devices/stm32u5/rtc.py
@@ -153,32 +158,40 @@
 psdb/probes/stlink/stlink.py
 psdb/probes/stlink/stlink_v2_1.py
 psdb/probes/stlink/stlink_v3.py
 psdb/probes/xds110/__init__.py
 psdb/probes/xds110/xds110.py
 psdb/probes/xtswd/__init__.py
 psdb/probes/xtswd/abort_test.py
+psdb/probes/xtswd/gl_plot_imon_realtime.py
 psdb/probes/xtswd/imon.py
 psdb/probes/xtswd/plot_imon.py
-psdb/probes/xtswd/plot_imon_realtime.py
 psdb/probes/xtswd/xtswd.py
 psdb/targets/__init__.py
 psdb/targets/target.py
 psdb/targets/msp432/__init__.py
 psdb/targets/msp432/msp432.py
+psdb/targets/stm32c0/__init__.py
+psdb/targets/stm32c0/dbgmcu.py
+psdb/targets/stm32c0/stm32c0.py
 psdb/targets/stm32g0/__init__.py
+psdb/targets/stm32g0/dbgmcu.py
 psdb/targets/stm32g0/stm32g0.py
 psdb/targets/stm32g4/__init__.py
 psdb/targets/stm32g4/dbgmcu.py
 psdb/targets/stm32g4/stm32g4.py
 psdb/targets/stm32h7/__init__.py
 psdb/targets/stm32h7/dbgmcu.py
 psdb/targets/stm32h7/stm32h7.py
 psdb/targets/stm32h7/stm32h7_dp.py
+psdb/targets/stm32l4/__init__.py
+psdb/targets/stm32l4/dbgmcu.py
+psdb/targets/stm32l4/stm32l4.py
 psdb/targets/stm32u5/__init__.py
 psdb/targets/stm32u5/dbgmcu.py
 psdb/targets/stm32u5/stm32u5.py
 psdb/targets/stm32wb55/__init__.py
+psdb/targets/stm32wb55/dbgmcu.py
 psdb/targets/stm32wb55/stm32wb55.py
 psdb/util/__init__.py
 psdb/util/hexify.py
 psdb/util/prange.py
```

### Comparing `psdb-1.1.2/setup.cfg` & `psdb-1.1.3/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = psdb
-version = 1.1.2
+version = 1.1.3
 author = Terry Greeniaus
 author_email = terrygreeniaus@gmail.com
 description = Package for interfacing with ARM-compatible debug probes
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = stlink xds110 arm swd fus stm32 msp432
 url = https://github.com/tgree/psdb
@@ -22,32 +22,36 @@
 	psdb.block
 	psdb.component
 	psdb.cpus
 	psdb.devices
 	psdb.devices.core
 	psdb.devices.msp432
 	psdb.devices.stm32
+	psdb.devices.stm32c0
 	psdb.devices.stm32g0
 	psdb.devices.stm32g4
 	psdb.devices.stm32h7
+	psdb.devices.stm32l4
 	psdb.devices.stm32u5
 	psdb.devices.stm32wb55
 	psdb.devices.stm32wb55.ipc
 	psdb.elf
 	psdb.hexfile
 	psdb.inspect_tool
 	psdb.probes
 	psdb.probes.stlink
 	psdb.probes.xds110
 	psdb.probes.xtswd
 	psdb.targets
 	psdb.targets.msp432
+	psdb.targets.stm32c0
 	psdb.targets.stm32g0
 	psdb.targets.stm32g4
 	psdb.targets.stm32h7
+	psdb.targets.stm32l4
 	psdb.targets.stm32u5
 	psdb.targets.stm32wb55
 	psdb.util
 install_requires = 
 	btype>=0.1.4
 	pyelftools
 	pyusb
```

