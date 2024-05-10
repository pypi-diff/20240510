# Comparing `tmp/heatmiser_wifi-1.2.0.tar.gz` & `tmp/heatmiser_wifi-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\heatmiser_wifi-1.2.0.tar", last modified: Mon Oct 19 18:16:11 2020, max compression
+gzip compressed data, was "dist\heatmiser_wifi-1.3.0.tar", last modified: Fri May 10 16:13:54 2024, max compression
```

## Comparing `heatmiser_wifi-1.2.0.tar` & `heatmiser_wifi-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/
--rw-rw-rw-   0        0        0     2701 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1504 2020-10-19 18:15:43.000000 heatmiser_wifi-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/heatmiser_wifi/
--rw-rw-rw-   0        0        0       37 2020-10-19 18:15:43.000000 heatmiser_wifi-1.2.0/heatmiser_wifi/__init__.py
--rw-rw-rw-   0        0        0    17443 2020-10-19 18:15:43.000000 heatmiser_wifi-1.2.0/heatmiser_wifi/heatmiser_wifi.py
-drwxrwxrwx   0        0        0        0 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/heatmiser_wifi.egg-info/
--rw-rw-rw-   0        0        0     2701 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/heatmiser_wifi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/heatmiser_wifi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/heatmiser_wifi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/heatmiser_wifi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-10-19 18:15:54.000000 heatmiser_wifi-1.2.0/heatmiser_wifi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/heatmiser_wifi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2020-10-19 18:16:11.000000 heatmiser_wifi-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1281 2020-10-19 18:15:43.000000 heatmiser_wifi-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/
+-rw-rw-rw-   0        0        0     1073 2024-05-10 16:13:19.000000 heatmiser_wifi-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4092 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3196 2024-05-10 16:13:19.000000 heatmiser_wifi-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/heatmiser_wifi/
+-rw-rw-rw-   0        0        0       37 2024-05-10 16:13:19.000000 heatmiser_wifi-1.3.0/heatmiser_wifi/__init__.py
+-rw-rw-rw-   0        0        0    25521 2024-05-10 16:13:19.000000 heatmiser_wifi-1.3.0/heatmiser_wifi/heatmiser_wifi.py
+drwxrwxrwx   0        0        0        0 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/heatmiser_wifi.egg-info/
+-rw-rw-rw-   0        0        0     4092 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/heatmiser_wifi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/heatmiser_wifi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/heatmiser_wifi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/heatmiser_wifi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-10 16:13:36.000000 heatmiser_wifi-1.3.0/heatmiser_wifi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/heatmiser_wifi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-10 16:13:54.000000 heatmiser_wifi-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2024-05-10 16:13:19.000000 heatmiser_wifi-1.3.0/setup.py
```

### Comparing `heatmiser_wifi-1.2.0/README.md` & `heatmiser_wifi-1.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 [![AppVeyor](https://ci.appveyor.com/api/projects/status/github/midstar/heatmiser_wifi?svg=true)](https://ci.appveyor.com/api/projects/status/github/midstar/heatmiser_wifi)
 
 ## Overview
 A [Heatmiser](http://www.heatmiser.com/) WiFi Thermostat communication tool and library for python.
 
 Supported Heatmiser Thermostats are DT, DT-E, PRT and PRT-E.
 
-The main class of the library is Heatmiser. It supports retrieval of all Thermostat parameters as a dictionary. It also supports setting of some (but not all) of the Thermostat parameters. 
+This release (v1.3.0) adds support for the PRT-HW WiFi thermostat, and adds the following functionality (for PRT-HW, maybe others):
+* Setting timers for heating (should work for all models)
+* Setting timers for hot water (for PRT-HW)
+* Setting clock on thermostat with option offset (should work for all models)
+
+The main class of the library is Heatmiser. It supports retrieval of all Thermostat parameters as a dictionary. It also supports setting of most (but not all) of the Thermostat parameters. 
 
 ## Supported platforms
 The application is written in Python and has been successfully tested with Python version 2.7 and 3.4.
 
-Both Windows and Linux has been tested successfully. Mac OS X has not been tested, but should work as well.
+For versions prior to v1.3.0 both Windows and Linux had been tested successfully. Mac OS X has not been tested, but should work as well. For this release v.1.3.0, only Linux has been tested, though I see no reason why it wouldn't work on the other platforms.
 
 ## Installation
 Run 
 
     python -m pip install heatmiser_wifi
 
 This will install both the library and the command line tool.
@@ -31,10 +36,29 @@
 To list all parameters write:
 
     heatmiser_wifi -c <pincode> <themostat_ip_address> -l 
 
 It is also possible to read and write specific parameters. For instructions, write:
 
     heatmiser_wifi -h
- 
+
+When setting triggers for heating / hot water use comma separated values for the trigger parameters
+
+For heating triggers: Time1Hour,Time1Minute,Time1Temp,Time2Hour,Time2Minute,Time2Temp,Time3Hour,Time3Minute,Time3Temp,Time4Hour,Time4Minute,Time4Temp
+
+For hot water triggers: Time1OnHour,Time1OnMinute,Time1OffHour,Time1OffMinute,Time2OnHour,Time2OnMinute,Time2OffHour,Time2OffMinute,Time3OnHour,Time3OnMinute,Time3OffHour,Time3OffMinute,Time4OnHour,Time4OnMinute,Time4OffHour,Time4OffMinute
+
+Note the thermostat only allows minutes to be either 0 or 30
+
+For example:
+    
+    heatmiser_wifi -c <pincode> <themostat_ip_address> -w mon_triggers 7,30,20,9,0,5,16,0,22,22,0,5
+    heatmiser_wifi -c <pincode> <themostat_ip_address> -w tue_hw_triggers 7,30,8,0,9,0,9,30,13,30,14,30,22,0,23,0
+
+When setting date / time, the parameter is an offset which added to the system date before sending to the thermostat. I use this to partially get round the limitation on the trigger minute only being 0 or 30
+
+For example, this will set the thermostat clock to be 15 mins behind the system time:
+
+    heatmiser_wifi -c <pincode> <themostat_ip_address> -w date_time -15
+
 ### Author and license
-This application is written by Joel Midstjärna and is licensed under the MIT License.
+This application is written by Joel Midstjärna and is licensed under the MIT License. Additional functionality and support for PRT-HW written by Iain Bullock
```

### Comparing `heatmiser_wifi-1.2.0/heatmiser_wifi/heatmiser_wifi.py` & `heatmiser_wifi-1.3.0/heatmiser_wifi/heatmiser_wifi.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 ###############################################################################
 #   - heatmiser_wifi -
 #
 #   Copyright 2020 by Joel Midstjärna (joel.midstjarna@gmail.com)
 #
 #   A Heatmiser WiFi Thermostat communication library. 
 #
-#   Supported Heatmiser Thermostats are DT, DT-E, PRT and PRT-E.
+#   Supported Heatmiser Thermostats orignally were DT, DT-E, PRT and PRT-E.
+#
+#   Update by Iain Bullock Nov 2023 to add support for PRTHW, 
+#   and to be able to read and write more things 
 #
 #   It is also possible to run this file as a command line executable.
 #
 #   All rights reserved.
 #   This file is part of the heatmiser_wifi python library and is
 #   released under the "MIT License Agreement". Please see the LICENSE
 #   file that should have been included as part of this package.
 ###############################################################################
 
 import socket, time, sys
 from optparse import OptionParser
 from collections import OrderedDict
+from datetime import datetime, timedelta
 
 class CRC16:
     CRC16_LookupHigh = [0x00, 0x10, 0x20, 0x30, 0x40, 0x50, 0x60, 0x70,
                         0x81, 0x91, 0xA1, 0xB1, 0xC1, 0xD1, 0xE1, 0xF1]
     CRC16_LookupLow  = [0x00, 0x21, 0x42, 0x63, 0x84, 0xA5, 0xC6, 0xE7,
                         0x08, 0x29, 0x4A, 0x6B, 0x8C, 0xAD, 0xCE, 0xEF]
                         
@@ -154,34 +158,53 @@
         self._send_read_request()
         (dcb_start, dcb_data) = self._receive_dcb()
         return dcb_data
         
     def set_dcb(self, dcb_address, dcb_data):
         self._send_write_request(dcb_address, dcb_data)
         # Just get an ACK from the Thermostat (don't use the result)
-        dcb = self._receive_dcb()
+        # Actually don't bother waiting for the ACK. Reduce comms with thermostat to potentially reduce errors
+        # dcb = self._receive_dcb()
 
 class Heatmiser(HeatmiserTransport):
     ''' This class handles the Heatmiser application (DCB) protocol '''
     
+    modelNumber = -1
+    programMode = -1
+    
     def _get_info_time_triggers(self, dcb, first_index):
         index = first_index
         info = OrderedDict()
         for i in range (1,5):
             trigger = OrderedDict()
             trigger['hour'] = dcb[index]
             index = index + 1
             trigger['minute'] = dcb[index]
             index = index + 1     
             trigger['set_temp'] = dcb[index]
             index = index + 1
             info['time'+str(i)] = trigger
-         
+        return info
+        
+    def _get_info_time_triggers_hw(self, dcb, first_index):
+        index = first_index
+        info = OrderedDict()
+        for i in range (1,5):
+            trigger = OrderedDict()
+            trigger['hour_on'] = dcb[index]
+            index = index + 1
+            trigger['minute_on'] = dcb[index]
+            index = index + 1     
+            trigger['hour_off'] = dcb[index]
+            index = index + 1
+            trigger['minute_off'] = dcb[index]
+            index = index + 1            
+            info['time'+str(i)] = trigger
         return info 
-    
+          
     def get_info(self):
         ''' Returns an ordered dictionary with all Thermostat values '''
         dcb = self.get_dcb()
         
         if(len(dcb) < 41):
             raise Exception("Size of DCB received from Thermostat is too small")
         
@@ -189,173 +212,329 @@
         
         if(dcb[2] == 0):
             info["vendor_id"] = "HEATMISER"
         else:
             info["vendor_id"] = "OEM"           
         info["version"] = dcb[3] & 0x7F  
         info["in_floor_limit_state"] = ((dcb[3] & 0x8F) > 0)
-        if(dcb[4] == 0):
+        
+        self.modelNumber = dcb[4]
+        if(self.modelNumber == 0):
             info["model"] = "DT"
-        elif(dcb[4] == 1):
+        elif(self.modelNumber == 1):
             info["model"] = "DT-E"       
-        elif(dcb[4] == 2):
+        elif(self.modelNumber == 2):
             info["model"] = "PRT" 
-        elif(dcb[4] == 3):
+        elif(self.modelNumber == 3):
             info["model"] = "PRT-E"
+        elif(self.modelNumber == 4):
+            info["model"] = "PRT-HW"
         else:
             info["model"] = "Unknown"
+            
         if(dcb[5] == 0):
             info["temperature_format"] = "Celsius"
         else:
             info["temperature_format"] = "Fahrenheit"
+            
         info["switch_differential"] = dcb[6]
         info["frost_protection_enable"] = (dcb[7] == 1)
         info["calibration_offset"] = ((dcb[8] << 8) | dcb[9])
         info["output_delay_in_minutes"] = dcb[10]
         # dcb[11] = address (not used)
         info['up_down_key_limit'] = dcb[12]
+        
         if(dcb[13] == 0):
             info['sensor_selection'] = "Built in air sensor only"
         elif(dcb[13] == 1):
             info['sensor_selection'] = "Remote air sensor only"
         elif(dcb[13] == 2):
             info['sensor_selection'] = "Floor sensor only"
         elif(dcb[13] == 3):
             info['sensor_selection'] = "Built in air and floor sensor"
         elif(dcb[13] == 4):
             info['sensor_selection'] = "Remote air and floor sensor"
         else:
             info['sensor_selection'] = "Unknown"
+            
         info['optimum_start'] = dcb[14]
         info['rate_of_change'] = dcb[15]
-        if(dcb[16] == 0):
+
+        self.programMode = dcb[16]
+        if(self.programMode == 0):
             info['program_mode'] = "2/5 mode"
         else:
             info['program_mode'] = "7 day mode"
+            
         info['frost_protect_temperature'] = dcb[17]
         info['set_room_temp'] = dcb[18]
         info['floor_max_limit'] = dcb[19]
         info['floor_max_limit_enable'] = (dcb[20] == 1)
+        
         if(dcb[21] == 1):
             info['on_off'] = "On"
         else:
             info['on_off'] = "Off"
+            
         if(dcb[22] == 0):
             info['key_lock'] = "Unlock"
         else:
             info['key_lock'] = "Lock"  
+            
         if(dcb[23] == 0):
             info['run_mode'] = "Heating mode (normal mode)"
         else:
             info['run_mode'] = "Frost protection mode"
-        # dcb[24] = away mode (not used)
+            
+        if(dcb[24] == 0):
+            info['away_mode'] = 'Off'
+        else:
+            info['away_mode'] = 'On'
+            
         info['holiday_return_date_year'] = 2000 + dcb[25]
         info['holiday_return_date_month'] = dcb[26]
         info['holiday_return_date_day_of_month'] = dcb[27]
         info['holiday_return_date_hour'] = dcb[28]
         info['holiday_return_date_minute'] = dcb[29]
         info['holiday_enable'] = (dcb[30] == 1)
         info['temp_hold_minutes'] = ((dcb[31] << 8) | dcb[32])
+        
         if((dcb[13] == 1) or (dcb[13] == 4)):
             info['air_temp'] = (float((dcb[34] << 8) | dcb[33]) / 10.0)   
         if((dcb[13] == 2) or (dcb[13] == 3) or (dcb[13] == 4)):
             info['floor_temp'] = (float((dcb[36] << 8) | dcb[35]) / 10.0)               
         if((dcb[13] == 0) or (dcb[13] == 3)):
             info['air_temp'] = (float((dcb[38] << 8) | dcb[37]) / 10.0)
+            
         info['error_code'] = dcb[39]
         info['heating_is_currently_on'] = (dcb[40] == 1)
         
         # Model DT and DT-E stops here
-        if(dcb[4] <= 1):
+        if(self.modelNumber <= 1):
             return info
         
         if(len(dcb) < 72):
             raise Exception("Size of DCB received from Thermostat is too small")        
 
-        info['year'] = 2000 + dcb[41]
-        info['month'] = dcb[42]
-        info['day_of_month'] = dcb[43]
-        info['weekday'] = dcb[44]
-        info['hour'] = dcb[45]
-        info['minute'] = dcb[46]
-        info['second'] = dcb[47]
-        info['weekday_triggers'] = self._get_info_time_triggers(dcb, 48)
-        info['weekend_triggers'] = self._get_info_time_triggers(dcb, 60)
-        
+        # Model PRT-HW has extra fields and offsets for the rest
+        if(self.modelNumber != 4):
+            info['year'] = 2000 + dcb[41]
+            info['month'] = dcb[42]
+            info['day_of_month'] = dcb[43]
+            info['weekday'] = dcb[44]
+            info['hour'] = dcb[45]
+            info['minute'] = dcb[46]
+            info['second'] = dcb[47]
+            info['date_time'] = str(info['year']) + '/' + str(info['month']) + '/' + str(info['day_of_month']) + " " + str(info['hour']) + ':' + str(info['minute']) + ':' + str(info['second'])
+            info['weekday_triggers'] = self._get_info_time_triggers(dcb, 48)
+            info['weekend_triggers'] = self._get_info_time_triggers(dcb, 60)
+        else:
+            info['boost'] = ((dcb[41] << 8) | dcb[42])
+            if(dcb[43] == 1):
+                info['hot_water_state'] = 'On'
+            else:
+                info['hot_water_state'] = 'Off'
+            info['year'] = 2000 + dcb[44]
+            info['month'] = dcb[45]
+            info['day_of_month'] = dcb[46]
+            info['weekday'] = dcb[47]
+            info['hour'] = dcb[48]
+            info['minute'] = dcb[49]
+            info['second'] = dcb[50]
+            info['date_time'] = str(info['year']) + '/' + str(info['month']) + '/' + str(info['day_of_month']) + " " + str(info['hour']) + ':' + str(info['minute']) + ':' + str(info['second'])
+            info['weekday_triggers'] = self._get_info_time_triggers(dcb, 51)
+            info['weekend_triggers'] = self._get_info_time_triggers(dcb, 63)            
+            info['weekday_hw_triggers'] = self._get_info_time_triggers_hw(dcb, 75)
+            info['weekend_hw_triggers'] = self._get_info_time_triggers_hw(dcb, 91)     
+            
         # If mode is 5/2 stop here
-        if(dcb[16] == 0):
+        if(self.programMode == 0):
             return info      
             
         if(len(dcb) < 156):
             raise Exception("Size of DCB received from Thermostat is too small")    
             
-        info['mon_triggers'] = self._get_info_time_triggers(dcb, 72) 
-        info['tue_triggers'] = self._get_info_time_triggers(dcb, 84) 
-        info['wed_triggers'] = self._get_info_time_triggers(dcb, 96)
-        info['thu_triggers'] = self._get_info_time_triggers(dcb, 108)
-        info['fri_triggers'] = self._get_info_time_triggers(dcb, 120) 
-        info['sat_triggers'] = self._get_info_time_triggers(dcb, 132)
-        info['sun_triggers'] = self._get_info_time_triggers(dcb, 144)   
-        
+        # Model PRT-HW has extra fields and offsets for the rest    
+        if(self.modelNumber != 4):
+            info['mon_triggers'] = self._get_info_time_triggers(dcb, 72) 
+            info['tue_triggers'] = self._get_info_time_triggers(dcb, 84) 
+            info['wed_triggers'] = self._get_info_time_triggers(dcb, 96)
+            info['thu_triggers'] = self._get_info_time_triggers(dcb, 108)
+            info['fri_triggers'] = self._get_info_time_triggers(dcb, 120) 
+            info['sat_triggers'] = self._get_info_time_triggers(dcb, 132)
+            info['sun_triggers'] = self._get_info_time_triggers(dcb, 144)  
+        else:
+            info['mon_triggers'] = self._get_info_time_triggers(dcb, 107) 
+            info['tue_triggers'] = self._get_info_time_triggers(dcb, 119) 
+            info['wed_triggers'] = self._get_info_time_triggers(dcb, 131)
+            info['thu_triggers'] = self._get_info_time_triggers(dcb, 143)
+            info['fri_triggers'] = self._get_info_time_triggers(dcb, 155) 
+            info['sat_triggers'] = self._get_info_time_triggers(dcb, 167)
+            info['sun_triggers'] = self._get_info_time_triggers(dcb, 179)  
+            
+            info['mon_hw_triggers'] = self._get_info_time_triggers_hw(dcb, 191) 
+            info['tue_hw_triggers'] = self._get_info_time_triggers_hw(dcb, 207) 
+            info['wed_hw_triggers'] = self._get_info_time_triggers_hw(dcb, 223)
+            info['thu_hw_triggers'] = self._get_info_time_triggers_hw(dcb, 239)
+            info['fri_hw_triggers'] = self._get_info_time_triggers_hw(dcb, 255) 
+            info['sat_hw_triggers'] = self._get_info_time_triggers_hw(dcb, 271)
+            info['sun_hw_triggers'] = self._get_info_time_triggers_hw(dcb, 287) 
+            
         return info
 
     def set_value(self, name, value):
         ''' Use the same name and value as returned in get_info. Only a few
             name/keys are supported in this implementation. Use the set_dcb
             method to set any value. '''
-        if(name == "switch_differential"):
-            self.set_dcb(6,bytearray([int(value)]))
-        elif(name == "frost_protect_temperature"):
-            self.set_dcb(17,bytearray([int(value)]))            
+
+        # Read only 
+        #if(name == "switch_differential"):
+        #    self.set_dcb(6,bytearray([int(value)]))
+
+        # Read only
+        #elif(name == "program_mode"):
+        #    if(value == '2/5 mode'):
+        #        value = 0
+        #    elif(value == '7 day mode'):
+        #        value = 1
+        #    else:
+        #        raise Exception("'"+name+"' invalid value '"+str(value)+"'\n" +
+        #                        "Valid values: '7 day mode' or '2/5 mode'")
+        #    self.set_dcb(16,bytearray([value]))
+
+        if(name == "frost_protect_temperature"):
+            self.set_dcb(17,bytearray([int(value)]))         
+            
         elif(name == "set_room_temp"):
             self.set_dcb(18,bytearray([int(value)]))  
+
         elif(name == "floor_max_limit"):
             self.set_dcb(19,bytearray([int(value)]))  
-        elif(name == "floor_max_limit_enable"):
-            if((value == True) or (value == "True") or (value == "1") or (value == 1)):
-                value = 1
-            elif((value == False) or (value == "False") or (value == "0") or (value == 0)):
-                value = 0
-            else:
-                raise Exception("'"+name+"' invalid value '"+str(value)+"'\n" +
-                                "Valid values: True, 1, False or 0")
-            self.set_dcb(20,bytearray([value]))  
+
+        # Read only
+        #elif(name == "floor_max_limit_enable"):
+        #    if((value == True) or (value == "True") or (value == "1") or (value == 1)):
+        #        value = 1
+        #    elif((value == False) or (value == "False") or (value == "0") or (value == 0)):
+        #        value = 0
+        #    else:
+        #        raise Exception("'"+name+"' invalid value '"+str(value)+"'\n" +
+        #                        "Valid values: True, 1, False or 0")
+        #    self.set_dcb(20,bytearray([value]))  
+            
         elif(name == "on_off"):
             if(value == "On"):
                 value = 1
             elif(value == "Off"):
                 value = 0
             else:
                 raise Exception("'"+name+"' invalid value '"+str(value)+"'\n" +
                                 "Valid values: 'On' or 'Off'")
             self.set_dcb(21,bytearray([value])) 
+            
         elif(name == "key_lock"):
             if(value == "Lock"):
                 value = 1
             elif(value == "Unlock"):
                 value = 0
             else:
                 raise Exception("'"+name+"' invalid value '"+str(value)+"'\n" +
                                 "Valid values: 'Lock' or 'Unlock'")
             self.set_dcb(22,bytearray([value]))
+            
         elif(name == "run_mode"):
             if(value == "Frost protection mode"):
                 value = 1
             elif(value == "Heating mode (normal mode)"):
                 value = 0
             else:
                 raise Exception("'"+name+"' invalid value '"+str(value)+"'\n" +
                                 "Valid values: 'Frost protection mode' or " +
                                 "'Heating mode (normal mode)'")
-            self.set_dcb(23,bytearray([value]))                            
-        else:
-            raise Exception("'"+name+"' not supported to be set")
-
-
+            self.set_dcb(23,bytearray([value]))    
+            
+        elif(name == "away_mode"):
+            if(value == "Off"):
+                value = 0
+            elif(value == "On"):
+                value = 1
+            else:
+                raise Exception("'"+name+"' invalid value '"+str(value)+"'\n" +
+                                "Valid values: 'On' or 'Off'")
+            self.set_dcb(31,bytearray([value]))
+            
+        elif(name == "hot_water_state"):
+            if(value == "Off"):
+                value = 2
+            elif(value == "On"):
+                value = 1
+            elif(value == "Prog"):
+                value = 0
+            else:
+                raise Exception("'"+name+"' invalid value '"+str(value)+"'\n" +
+                                "Valid values: 'On', 'Off' or 'Prog'")
+            self.set_dcb(42,bytearray([value]))
+            
+        # Model DT and DT-E stops here
+        if(self.modelNumber <= 1):
+            return 
+            
+        if(name == "date_time"):
+            # the passed value is used as an offset in minutes to apply to the system time
+            todays_date = datetime.now() + timedelta(minutes=int(value))
+            self.set_dcb(43,bytearray([todays_date.year-2000,todays_date.month,todays_date.day,todays_date.weekday()+1,todays_date.hour,todays_date.minute,todays_date.second]))        
+            
+        if(name == "weekday_triggers"):
+            self.set_dcb(47,bytearray(value))
+        elif(name == "weekend_triggers"):
+            self.set_dcb(59,bytearray(value))
+
+        if(self.modelNumber == 4):
+            if(name == "weekday_hw_triggers"):
+                self.set_dcb(71,bytearray(value))
+            elif(name == "weekend_hw_triggers"):
+                self.set_dcb(87,bytearray(value))
+                    
+        # If mode is 5/2 stop here
+        if(self.programMode == 0):
+            return 
 
+        if(name == "mon_triggers"):
+            self.set_dcb(103,bytearray(value))
+        elif(name == "tue_triggers"):
+            self.set_dcb(115,bytearray(value))
+        elif(name == "wed_triggers"):
+            self.set_dcb(127,bytearray(value))
+        elif(name == "thu_triggers"):
+            self.set_dcb(139,bytearray(value))            
+        elif(name == "fri_triggers"):
+            self.set_dcb(151,bytearray(value))
+        elif(name == "sat_triggers"):
+            self.set_dcb(163,bytearray(value))            
+        elif(name == "sun_triggers"):
+            self.set_dcb(175,bytearray(value))            
+
+        # If model is not PRT-HW stop here
+        if(self.modelNumber != 4):
+            return 
+
+        if(name == "mon_hw_triggers"):
+            self.set_dcb(187,bytearray(value))
+        elif(name == "tue_hw_triggers"):
+            self.set_dcb(203,bytearray(value))
+        elif(name == "wed_hw_triggers"):
+            self.set_dcb(219,bytearray(value))
+        elif(name == "thu_hw_triggers"):
+            self.set_dcb(235,bytearray(value))            
+        elif(name == "fri_hw_triggers"):
+            self.set_dcb(251,bytearray(value))
+        elif(name == "sat_hw_triggers"):
+            self.set_dcb(267,bytearray(value))            
+        elif(name == "sun_hw_triggers"):
+            self.set_dcb(283,bytearray(value))     
 
 ###############################################################################
 # Below is a command line tool for reading and setting parameters of a
 # Heatmiser Wifi thermostat. It can also be seen as an example on how to use
 # the library.
 
 
@@ -408,23 +587,29 @@
         else:
             sys.stderr.write("Error!\n"+
                 "Parameter '"+options.parameter+"' does not exist\n")
     
     # Write value to one parameter in Thermostat
     if(options.param_value != None):
         param = options.param_value[0]
-        value = options.param_value[1]
+
+        if (param in ['weekday_triggers', 'weekend_triggers', 'mon_triggers', 'tue_triggers', 'wed_triggers', 'thu_triggers', 'fri_triggers', 'sat_triggers', 'sun_triggers', 'weekday_hw_triggers', 'weekend_hw_triggers', 'mon_hw_triggers', 'tue_hw_triggers', 'wed_hw_triggers', 'thu_hw_triggers', 'fri_hw_triggers', 'sat_hw_triggers', 'sun_hw_triggers']):
+            # Form array of integers for these
+            value = [int(e) for e in options.param_value[1].split(",")]
+        else:
+            value = options.param_value[1]
+            
         if (param in info):
             try:
                 heatmiser.set_value(param,value)
                 info2 = heatmiser.get_info()
                 print("Before change: " + param + " = " + str(info[param]))
                 print("After change:  " + param + " = " + str(info2[param]))
             except Exception as e:
                 sys.stderr.write(e.args[0]+"\n")
         else:
             sys.stderr.write("Error!\n"+
                 "Parameter '"+param+"' does not exist\n")
     heatmiser.disconnect()
         
 if __name__ == '__main__':
-    main()    
+    main()
```

### Comparing `heatmiser_wifi-1.2.0/setup.py` & `heatmiser_wifi-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 try:
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except:
       long_description = ""
 
 setup(name='heatmiser_wifi',
-      version='1.2.0',
+      version='1.3.0',
       description='Library for communication with Heatmiser Wifi thermostats',
       long_description=long_description,
        long_description_content_type="text/markdown",
       url='http://github.com/midstar/heatmiser_wifi',
       project_urls={
             'Bug Tracker': 'https://github.com/midstar/heatmiser_wifi/issues',
             'Source Code': 'https://github.com/midstar/heatmiser_wifi',
```

