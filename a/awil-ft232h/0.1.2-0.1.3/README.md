# Comparing `tmp/awil_ft232h-0.1.2.tar.gz` & `tmp/awil_ft232h-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awil_ft232h-0.1.2.tar", last modified: Mon Apr 15 01:36:25 2024, max compression
+gzip compressed data, was "awil_ft232h-0.1.3.tar", last modified: Mon Apr 15 05:42:45 2024, max compression
```

## Comparing `awil_ft232h-0.1.2.tar` & `awil_ft232h-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 01:36:25.342550 awil_ft232h-0.1.2/
--rw-rw-rw-   0        0        0     1084 2024-04-09 04:08:59.000000 awil_ft232h-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      521 2024-04-15 01:36:25.341549 awil_ft232h-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-10 09:44:35.000000 awil_ft232h-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 01:36:25.327376 awil_ft232h-0.1.2/awil_ft232h/
--rw-rw-rw-   0        0        0       35 2024-04-09 04:08:59.000000 awil_ft232h-0.1.2/awil_ft232h/__init__.py
--rw-rw-rw-   0        0        0     2202 2024-04-12 10:18:32.000000 awil_ft232h-0.1.2/awil_ft232h/awil_ft232h.py
-drwxrwxrwx   0        0        0        0 2024-04-15 01:36:25.341549 awil_ft232h-0.1.2/awil_ft232h.egg-info/
--rw-rw-rw-   0        0        0      521 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 01:36:25.342550 awil_ft232h-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      395 2024-04-15 01:36:16.000000 awil_ft232h-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:42:45.993243 awil_ft232h-0.1.3/
+-rw-rw-rw-   0        0        0     1084 2024-04-09 04:08:59.000000 awil_ft232h-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      521 2024-04-15 05:42:45.993243 awil_ft232h-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-04-10 09:44:35.000000 awil_ft232h-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 05:42:45.976246 awil_ft232h-0.1.3/awil_ft232h/
+-rw-rw-rw-   0        0        0       35 2024-04-15 05:16:30.000000 awil_ft232h-0.1.3/awil_ft232h/__init__.py
+-rw-rw-rw-   0        0        0     2775 2024-04-15 05:42:03.000000 awil_ft232h-0.1.3/awil_ft232h/awil_ft232h.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:42:45.992243 awil_ft232h-0.1.3/awil_ft232h.egg-info/
+-rw-rw-rw-   0        0        0      521 2024-04-15 05:42:45.000000 awil_ft232h-0.1.3/awil_ft232h.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-15 05:42:45.000000 awil_ft232h-0.1.3/awil_ft232h.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 05:42:45.000000 awil_ft232h-0.1.3/awil_ft232h.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 05:42:45.000000 awil_ft232h-0.1.3/awil_ft232h.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 05:42:45.000000 awil_ft232h-0.1.3/awil_ft232h.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 05:42:45.993243 awil_ft232h-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      395 2024-04-15 05:42:21.000000 awil_ft232h-0.1.3/setup.py
```

### Comparing `awil_ft232h-0.1.2/LICENSE` & `awil_ft232h-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `awil_ft232h-0.1.2/PKG-INFO` & `awil_ft232h-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awil_ft232h
-Version: 0.1.2
+Version: 0.1.3
 Author: Noriki Mochizuki
 Author-email: noriki.mochizuki.mj@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyftdi>=0.55
```

### Comparing `awil_ft232h-0.1.2/awil_ft232h/awil_ft232h.py` & `awil_ft232h-0.1.3/awil_ft232h/awil_ft232h.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pyftdi.spi import SpiController, SpiPort
 from typing import List
 
+
 class AwilFt232h:
     _ADBUS_COUNT = 5
     _ACBUS_COUNT = 10
+    _GPIO_BASE_MASK = 0x0100  # GPIOの開始位置（8bit目から）
 
     def __init__(self) -> None:
         self._spi: SpiController = None
         self._is_open = False
 
     def __del__(self) -> None:
         if self._spi is not None:
@@ -43,12 +45,26 @@
             spi_port = self._spi.get_port(channel, frequency, mode)
             if operation == 'write':
                 spi_port.write(data)
             elif operation == 'read':
                 return list(spi_port.read(length))
             elif operation == 'exchange':
                 return list(spi_port.exchange(data, len(data)))
-        else: # TODO: GPIO単体でのオンオフを実装
-            self._spi.write_gpio(0x0000)
-            result = self._spi.exchange(frequency, data, readlen=length or len(data), duplex=True, cpol=bool(mode & 0x2), cpha=bool(mode & 0x1))
-            self._spi.write_gpio(0xFF00)
+        else:
+            # 対象のGPIOピンマスクを計算
+            gpio_pin_mask = self._GPIO_BASE_MASK << (channel - self._ADBUS_COUNT)
+
+            # 現在のGPIO状態を読み取る
+            current_gpio_state = self._spi.read_gpio()
+
+            # 対象のGPIOピンのみをLOWに設定
+            new_gpio_state = current_gpio_state & ~gpio_pin_mask
+            self._spi.write_gpio(new_gpio_state)
+
+            # 命令を送信
+            result = list(self._spi.exchange(frequency, data, readlen=length or len(data), duplex=True, cpol=bool(mode & 0x2), cpha=bool(mode & 0x1)))
+
+            # 操作後に元のGPIO状態に戻す
+            new_gpio_state = current_gpio_state | gpio_pin_mask
+            self._spi.write_gpio(new_gpio_state)
+
             return result
```

### Comparing `awil_ft232h-0.1.2/awil_ft232h.egg-info/PKG-INFO` & `awil_ft232h-0.1.3/awil_ft232h.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awil_ft232h
-Version: 0.1.2
+Version: 0.1.3
 Author: Noriki Mochizuki
 Author-email: noriki.mochizuki.mj@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyftdi>=0.55
```

