# Comparing `tmp/tplinkrouterc6u-3.5.0.tar.gz` & `tmp/tplinkrouterc6u-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tplinkrouterc6u-3.5.0.tar", last modified: Mon Apr  1 05:49:09 2024, max compression
+gzip compressed data, was "tplinkrouterc6u-4.0.0.tar", last modified: Wed Apr 10 07:40:58 2024, max compression
```

## Comparing `tplinkrouterc6u-3.5.0.tar` & `tplinkrouterc6u-4.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:49:09.400915 tplinkrouterc6u-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-01 05:49:09.400915 tplinkrouterc6u-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 05:49:09.400915 tplinkrouterc6u-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:49:09.396914 tplinkrouterc6u-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30437 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/test/test_client_deco.py
--rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/test/test_client_mr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:49:09.396914 tplinkrouterc6u-3.5.0/tplinkrouterc6u/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45691 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 05:49:05.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:49:09.400915 tplinkrouterc6u-3.5.0/tplinkrouterc6u.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-01 05:49:09.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-01 05:49:09.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 05:49:09.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 05:49:09.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 05:49:09.000000 tplinkrouterc6u-3.5.0/tplinkrouterc6u.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:40:58.016698 tplinkrouterc6u-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-04-10 07:40:58.016698 tplinkrouterc6u-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:40:58.016698 tplinkrouterc6u-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:40:58.012698 tplinkrouterc6u-4.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30473 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/test/test_client_deco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/test/test_client_mr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:40:58.012698 tplinkrouterc6u-4.0.0/tplinkrouterc6u/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48696 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 07:40:52.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:40:58.016698 tplinkrouterc6u-4.0.0/tplinkrouterc6u.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-04-10 07:40:58.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-10 07:40:58.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:40:58.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 07:40:58.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 07:40:58.000000 tplinkrouterc6u-4.0.0/tplinkrouterc6u.egg-info/top_level.txt
```

### Comparing `tplinkrouterc6u-3.5.0/LICENSE` & `tplinkrouterc6u-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-3.5.0/PKG-INFO` & `tplinkrouterc6u-4.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplinkrouterc6u
-Version: 3.5.0
+Version: 4.0.0
 Summary: TP-Link Router API
 Home-page: https://github.com/AlexandrErohin/TP-Link-Archer-C6U
 Author: Alex Erohin
 Author-email: alexanderErohin@yandex.ru
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -34,20 +34,20 @@
  - [pycryptodome](https://pypi.org/project/pycryptodome/)
 
 ## Usage
 Enter the host & credentials used to log in to your router management page. Username is admin by default. But you may pass username as third parameter
 
 ```python
 from tplinkrouterc6u import (
-    TplinkRouterProvider, 
+    TplinkRouterProvider,
     TplinkRouter,
     TplinkC1200Router,
     TPLinkMRClient,
     TPLinkDecoClient,
-    Wifi
+    Connection
 )
 from logging import Logger
 
 router = TplinkRouterProvider.get_client('http://192.168.0.1', 'password')
 # You may use client directly like
 # router = TplinkRouter('http://192.168.0.1', 'password')
 # You may also pass username if it is different and a logger to log errors as
@@ -61,15 +61,15 @@
     router.authorize()  # authorizing
     # Get firmware info - returns Firmware
     firmware = router.get_firmware()
 
     # Get status info - returns Status
     status = router.get_status()
     if not status.guest_2g_enable:  # check if guest 2.4G wifi is disable
-        router.set_wifi(Wifi.WIFI_GUEST_2G, True)  # turn on guest 2.4G wifi
+        router.set_wifi(Connection.GUEST_2G, True)  # turn on guest 2.4G wifi
 
     # Get Address reservations, sort by ipaddr
     reservations = router.get_ipv4_reservations()
     reservations.sort(key=lambda a: a.ipaddr)
     for res in reservations:
         print(f"{res.macaddr} {res.ipaddr:16s} {res.hostname:36} {'Permanent':12}")
 
@@ -93,25 +93,25 @@
 3. Click somewhere else on the page so that the password field is not selected anymore.
 4. Open the JavaScript console of your browser (usually by pressing F12 and then clicking on "Console").
 5. Type `document.getElementById("login-password").value;`
 6. Copy the returned value as password and use it.
 
 ## Functions
 | Function | Args | Description | Return |
-|--|--|--|--|
-| get_firmware |  | Gets firmware info about the router | [Firmware](#firmware) |
-| get_status |  | Gets status about the router info including wifi statuses and wifi clients info | [Status](#status) |
-| get_ipv4_status |  | Gets WAN and LAN IPv4 status info, gateway, DNS, netmask | [IPv4Status](#IPv4Status) |
-| get_ipv4_reservations |  | Gets IPv4 reserved addresses (static) | [[IPv4Reservation]](#IPv4Reservation) |
-| get_ipv4_dhcp_leases |  | Gets IPv4 addresses assigned via DHCP | [[IPv4DHCPLease]](#IPv4DHCPLease) | 
-| set_wifi | wifi: [Wifi](#wifi), enable: bool | Allow to turn on/of 4 wifi networks |  |
-| send_sms | phone_number: str, message: str | Send sms for LTE routers |  |
-| reboot |  | reboot router |
-| authorize |  | authorize for actions |
-| logout |  | logout after all is done |
+|---|---|---|---|
+| get_firmware |   | Gets firmware info about the router | [Firmware](#firmware) |
+| get_status |   | Gets status about the router info including wifi statuses and connected devices info | [Status](#status) |
+| get_ipv4_status |   | Gets WAN and LAN IPv4 status info, gateway, DNS, netmask | [IPv4Status](#IPv4Status) |
+| get_ipv4_reservations |   | Gets IPv4 reserved addresses (static) | [[IPv4Reservation]](#IPv4Reservation) |
+| get_ipv4_dhcp_leases |   | Gets IPv4 addresses assigned via DHCP | [[IPv4DHCPLease]](#IPv4DHCPLease) | 
+| set_wifi | wifi: [Connection](#connection), enable: bool | Allow to turn on/of 4 wifi networks |   |
+| send_sms | phone_number: str, message: str | Send sms for LTE routers |   |
+| reboot |   | reboot router |
+| authorize |   | authorize for actions |
+| logout |   | logout after all is done |
 
 ## Dataclass
 ### <a id="firmware">Firmware</a>
 | Field | Description | Type |
 | --- |----|----|
 | hardware_version | Returns like - Archer C6U | str |
 | model | Returns like - Archer C6U v1.0 | str |
@@ -127,36 +127,36 @@
 | wan_ipv4_addr | router wan ipv4 address | str, None |
 | wan_ipv4_address | router wan ipv4 address | ipaddress.IPv4Address, None |
 | lan_ipv4_addr | router lan ipv4 address | str, None |
 | lan_ipv4_address | router lan ipv4 address | ipaddress.IPv4Address, None |
 | wan_ipv4_gateway | router wan ipv4 gateway | str, None |
 | wan_ipv4_gateway_address | router wan ipv4 gateway address | ipaddress.IPv4Address, None |
 | wired_total | Total amount of wired clients | int |
-| wifi_clients_total | Total amount of main wifi clients | int |
+| wifi_clients_total | Total amount of host wifi clients | int |
 | guest_clients_total | Total amount of guest wifi clients | int |
 | clients_total | Total amount of all connected clients | int |
 | iot_clients_total | Total amount of all iot connected clients | int, None |
 | guest_2g_enable | Is guest wifi 2.4G enabled | bool |
 | guest_5g_enable | Is guest wifi 5G enabled | bool, None |
 | guest_6g_enable | Is guest wifi 6G enabled | bool, None |
 | iot_2g_enable | Is IoT wifi 2.4G enabled | bool, None |
 | iot_5g_enable | Is IoT wifi 5G enabled | bool, None |
 | iot_6g_enable | Is IoT wifi 6G enabled | bool, None |
-| wifi_2g_enable | Is main wifi 2.4G enabled | bool |
-| wifi_5g_enable | Is main wifi 5G enabled | bool, None |
-| wifi_6g_enable | Is main wifi 6G enabled | bool, None |
+| wifi_2g_enable | Is host wifi 2.4G enabled | bool |
+| wifi_5g_enable | Is host wifi 5G enabled | bool, None |
+| wifi_6g_enable | Is host wifi 6G enabled | bool, None |
 | wan_ipv4_uptime | Internet Uptime | int, None |
-| mem_usage | Memory usage | float, None |
-| cpu_usage | CPU usage | float, None |
-| devices | List of all wifi clients | list[[Device](#device)] |
+| mem_usage | Memory usage in percentage between 0 and 1 | float, None |
+| cpu_usage | CPU usage in percentage between 0 and 1 | float, None |
+| devices | List of all connectedd devices | list[[Device](#device)] |
 
 ### <a id="device">Device</a>
 | Field | Description | Type |
 | --- |---|---|
-| type | client connection type (2.4G or 5G, guest wifi or main wifi) | [Wifi](#wifi) |
+| type | client connection type (2.4G or 5G, guest wifi or host wifi, wired) | [Connection](#connection) |
 | macaddr | client mac address | str |
 | macaddress | client mac address | macaddress |
 | ipaddr | client ip address | str |
 | ipaddress | client ip address | ipaddress |
 | hostname | client hostname | str |
 | packets_sent | total packets sent | int, None |
 | packets_received | total packets received | int, None |
@@ -203,32 +203,34 @@
 | lan_ipv4_ipaddress | router LAN IP address | ipaddress |
 | lan_ipv4_dhcp_enable | router LAN DHCP enabled | bool |
 | lan_ipv4_netmask | router LAN gateway IP netmask | str |
 | lan_ipv4_netmask_address | router LAN gateway IP netmask | ipaddress |
 | remote | router remote | bool, None |
 
 ## Enum
-### <a id="wifi">Wifi</a>
-- Wifi.WIFI_2G - main wifi 2.4G
-- Wifi.WIFI_5G - main wifi 5G
-- Wifi.WIFI_6G - main wifi 5G
-- Wifi.WIFI_GUEST_2G - guest wifi 2.4G
-- Wifi.WIFI_GUEST_5G - guest wifi 5G
-- Wifi.WIFI_GUEST_6G - guest wifi 5G
-- Wifi.WIFI_IOT_2G - IoT wifi 2.4G
-- Wifi.WIFI_IOT_5G - IoT wifi 5G
-- Wifi.WIFI_IOT_6G - IoT wifi 6G
+### <a id="connection">Connection</a>
+- Connection.HOST_2G - host wifi 2.4G
+- Connection.HOST_5G - host wifi 5G
+- Connection.HOST_6G - host wifi 5G
+- Connection.GUEST_2G - guest wifi 2.4G
+- Connection.GUEST_5G - guest wifi 5G
+- Connection.GUEST_6G - guest wifi 5G
+- Connection.IOT_2G - IoT wifi 2.4G
+- Connection.IOT_5G - IoT wifi 5G
+- Connection.IOT_6G - IoT wifi 6G
+- Connection.WIRED - Wired
 
 ## <a id="supports">Supported routers</a>
 ### Fully tested Hardware Versions
 - Archer A7 V5
 - Archer AX10 v1.0
 - Archer AX12 v1.0
 - Archer AX20 v1.0
 - Archer AX21 v1.20
+- Archer AX23 v1.0
 - Archer AX50 v1.0
 - Archer AX55 v1.0
 - Archer AX55 V1.60
 - Archer AX72 V1
 - Archer AX73 V1
 - Archer AX75 V1
 - Archer AXE75 V1
```

### Comparing `tplinkrouterc6u-3.5.0/README.md` & `tplinkrouterc6u-4.0.0/tplinkrouterc6u.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: tplinkrouterc6u
+Version: 4.0.0
+Summary: TP-Link Router API
+Home-page: https://github.com/AlexandrErohin/TP-Link-Archer-C6U
+Author: Alex Erohin
+Author-email: alexanderErohin@yandex.ru
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pycryptodome
+Requires-Dist: macaddress
+
 # TP-Link Router API
 Python package for API access and management for TP-Link Routers. See [Supported routers](#supports)
 
 [![Pypi](https://img.shields.io/pypi/v/tplinkrouterc6u)](https://pypi.org/project/tplinkrouterc6u/)
 [![Downloads](https://static.pepy.tech/personalized-badge/tplinkrouterc6u?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pypi.org/project/tplinkrouterc6u/)
 ![Python versions](https://img.shields.io/pypi/pyversions/tplinkrouterc6u)
 
@@ -13,20 +34,20 @@
  - [pycryptodome](https://pypi.org/project/pycryptodome/)
 
 ## Usage
 Enter the host & credentials used to log in to your router management page. Username is admin by default. But you may pass username as third parameter
 
 ```python
 from tplinkrouterc6u import (
-    TplinkRouterProvider, 
+    TplinkRouterProvider,
     TplinkRouter,
     TplinkC1200Router,
     TPLinkMRClient,
     TPLinkDecoClient,
-    Wifi
+    Connection
 )
 from logging import Logger
 
 router = TplinkRouterProvider.get_client('http://192.168.0.1', 'password')
 # You may use client directly like
 # router = TplinkRouter('http://192.168.0.1', 'password')
 # You may also pass username if it is different and a logger to log errors as
@@ -40,15 +61,15 @@
     router.authorize()  # authorizing
     # Get firmware info - returns Firmware
     firmware = router.get_firmware()
 
     # Get status info - returns Status
     status = router.get_status()
     if not status.guest_2g_enable:  # check if guest 2.4G wifi is disable
-        router.set_wifi(Wifi.WIFI_GUEST_2G, True)  # turn on guest 2.4G wifi
+        router.set_wifi(Connection.GUEST_2G, True)  # turn on guest 2.4G wifi
 
     # Get Address reservations, sort by ipaddr
     reservations = router.get_ipv4_reservations()
     reservations.sort(key=lambda a: a.ipaddr)
     for res in reservations:
         print(f"{res.macaddr} {res.ipaddr:16s} {res.hostname:36} {'Permanent':12}")
 
@@ -72,25 +93,25 @@
 3. Click somewhere else on the page so that the password field is not selected anymore.
 4. Open the JavaScript console of your browser (usually by pressing F12 and then clicking on "Console").
 5. Type `document.getElementById("login-password").value;`
 6. Copy the returned value as password and use it.
 
 ## Functions
 | Function | Args | Description | Return |
-|--|--|--|--|
-| get_firmware |  | Gets firmware info about the router | [Firmware](#firmware) |
-| get_status |  | Gets status about the router info including wifi statuses and wifi clients info | [Status](#status) |
-| get_ipv4_status |  | Gets WAN and LAN IPv4 status info, gateway, DNS, netmask | [IPv4Status](#IPv4Status) |
-| get_ipv4_reservations |  | Gets IPv4 reserved addresses (static) | [[IPv4Reservation]](#IPv4Reservation) |
-| get_ipv4_dhcp_leases |  | Gets IPv4 addresses assigned via DHCP | [[IPv4DHCPLease]](#IPv4DHCPLease) | 
-| set_wifi | wifi: [Wifi](#wifi), enable: bool | Allow to turn on/of 4 wifi networks |  |
-| send_sms | phone_number: str, message: str | Send sms for LTE routers |  |
-| reboot |  | reboot router |
-| authorize |  | authorize for actions |
-| logout |  | logout after all is done |
+|---|---|---|---|
+| get_firmware |   | Gets firmware info about the router | [Firmware](#firmware) |
+| get_status |   | Gets status about the router info including wifi statuses and connected devices info | [Status](#status) |
+| get_ipv4_status |   | Gets WAN and LAN IPv4 status info, gateway, DNS, netmask | [IPv4Status](#IPv4Status) |
+| get_ipv4_reservations |   | Gets IPv4 reserved addresses (static) | [[IPv4Reservation]](#IPv4Reservation) |
+| get_ipv4_dhcp_leases |   | Gets IPv4 addresses assigned via DHCP | [[IPv4DHCPLease]](#IPv4DHCPLease) | 
+| set_wifi | wifi: [Connection](#connection), enable: bool | Allow to turn on/of 4 wifi networks |   |
+| send_sms | phone_number: str, message: str | Send sms for LTE routers |   |
+| reboot |   | reboot router |
+| authorize |   | authorize for actions |
+| logout |   | logout after all is done |
 
 ## Dataclass
 ### <a id="firmware">Firmware</a>
 | Field | Description | Type |
 | --- |----|----|
 | hardware_version | Returns like - Archer C6U | str |
 | model | Returns like - Archer C6U v1.0 | str |
@@ -106,36 +127,36 @@
 | wan_ipv4_addr | router wan ipv4 address | str, None |
 | wan_ipv4_address | router wan ipv4 address | ipaddress.IPv4Address, None |
 | lan_ipv4_addr | router lan ipv4 address | str, None |
 | lan_ipv4_address | router lan ipv4 address | ipaddress.IPv4Address, None |
 | wan_ipv4_gateway | router wan ipv4 gateway | str, None |
 | wan_ipv4_gateway_address | router wan ipv4 gateway address | ipaddress.IPv4Address, None |
 | wired_total | Total amount of wired clients | int |
-| wifi_clients_total | Total amount of main wifi clients | int |
+| wifi_clients_total | Total amount of host wifi clients | int |
 | guest_clients_total | Total amount of guest wifi clients | int |
 | clients_total | Total amount of all connected clients | int |
 | iot_clients_total | Total amount of all iot connected clients | int, None |
 | guest_2g_enable | Is guest wifi 2.4G enabled | bool |
 | guest_5g_enable | Is guest wifi 5G enabled | bool, None |
 | guest_6g_enable | Is guest wifi 6G enabled | bool, None |
 | iot_2g_enable | Is IoT wifi 2.4G enabled | bool, None |
 | iot_5g_enable | Is IoT wifi 5G enabled | bool, None |
 | iot_6g_enable | Is IoT wifi 6G enabled | bool, None |
-| wifi_2g_enable | Is main wifi 2.4G enabled | bool |
-| wifi_5g_enable | Is main wifi 5G enabled | bool, None |
-| wifi_6g_enable | Is main wifi 6G enabled | bool, None |
+| wifi_2g_enable | Is host wifi 2.4G enabled | bool |
+| wifi_5g_enable | Is host wifi 5G enabled | bool, None |
+| wifi_6g_enable | Is host wifi 6G enabled | bool, None |
 | wan_ipv4_uptime | Internet Uptime | int, None |
-| mem_usage | Memory usage | float, None |
-| cpu_usage | CPU usage | float, None |
-| devices | List of all wifi clients | list[[Device](#device)] |
+| mem_usage | Memory usage in percentage between 0 and 1 | float, None |
+| cpu_usage | CPU usage in percentage between 0 and 1 | float, None |
+| devices | List of all connectedd devices | list[[Device](#device)] |
 
 ### <a id="device">Device</a>
 | Field | Description | Type |
 | --- |---|---|
-| type | client connection type (2.4G or 5G, guest wifi or main wifi) | [Wifi](#wifi) |
+| type | client connection type (2.4G or 5G, guest wifi or host wifi, wired) | [Connection](#connection) |
 | macaddr | client mac address | str |
 | macaddress | client mac address | macaddress |
 | ipaddr | client ip address | str |
 | ipaddress | client ip address | ipaddress |
 | hostname | client hostname | str |
 | packets_sent | total packets sent | int, None |
 | packets_received | total packets received | int, None |
@@ -182,32 +203,34 @@
 | lan_ipv4_ipaddress | router LAN IP address | ipaddress |
 | lan_ipv4_dhcp_enable | router LAN DHCP enabled | bool |
 | lan_ipv4_netmask | router LAN gateway IP netmask | str |
 | lan_ipv4_netmask_address | router LAN gateway IP netmask | ipaddress |
 | remote | router remote | bool, None |
 
 ## Enum
-### <a id="wifi">Wifi</a>
-- Wifi.WIFI_2G - main wifi 2.4G
-- Wifi.WIFI_5G - main wifi 5G
-- Wifi.WIFI_6G - main wifi 5G
-- Wifi.WIFI_GUEST_2G - guest wifi 2.4G
-- Wifi.WIFI_GUEST_5G - guest wifi 5G
-- Wifi.WIFI_GUEST_6G - guest wifi 5G
-- Wifi.WIFI_IOT_2G - IoT wifi 2.4G
-- Wifi.WIFI_IOT_5G - IoT wifi 5G
-- Wifi.WIFI_IOT_6G - IoT wifi 6G
+### <a id="connection">Connection</a>
+- Connection.HOST_2G - host wifi 2.4G
+- Connection.HOST_5G - host wifi 5G
+- Connection.HOST_6G - host wifi 5G
+- Connection.GUEST_2G - guest wifi 2.4G
+- Connection.GUEST_5G - guest wifi 5G
+- Connection.GUEST_6G - guest wifi 5G
+- Connection.IOT_2G - IoT wifi 2.4G
+- Connection.IOT_5G - IoT wifi 5G
+- Connection.IOT_6G - IoT wifi 6G
+- Connection.WIRED - Wired
 
 ## <a id="supports">Supported routers</a>
 ### Fully tested Hardware Versions
 - Archer A7 V5
 - Archer AX10 v1.0
 - Archer AX12 v1.0
 - Archer AX20 v1.0
 - Archer AX21 v1.20
+- Archer AX23 v1.0
 - Archer AX50 v1.0
 - Archer AX55 v1.0
 - Archer AX55 V1.60
 - Archer AX72 V1
 - Archer AX73 V1
 - Archer AX75 V1
 - Archer AXE75 V1
```

### Comparing `tplinkrouterc6u-3.5.0/setup.py` & `tplinkrouterc6u-4.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tplinkrouterc6u",
-    version="3.5.0",
+    version="4.0.0",
     author="Alex Erohin",
     author_email="alexanderErohin@yandex.ru",
     description="TP-Link Router API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AlexandrErohin/TP-Link-Archer-C6U",
     packages=setuptools.find_packages(),
```

### Comparing `tplinkrouterc6u-3.5.0/test/test_client_deco.py` & `tplinkrouterc6u-4.0.0/test/test_client_deco.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 import json
 import macaddress
 import ipaddress
 from tplinkrouterc6u import (
     TPLinkDecoClient,
-    Wifi,
+    Connection,
     Firmware,
     Status,
     Device,
     IPv4Status,
 )
 
 
@@ -112,51 +112,52 @@
         self.assertEqual(status.iot_6g_enable, None)
         self.assertEqual(status.wifi_2g_enable, True)
         self.assertEqual(status.wifi_5g_enable, True)
         self.assertEqual(status.wifi_6g_enable, None)
         self.assertEqual(status.wan_ipv4_uptime, None)
         self.assertEqual(status.mem_usage, 0.43)
         self.assertEqual(status.cpu_usage, 0.1)
-        self.assertEqual(len(status.devices), 4)
+        self.assertEqual(len(status.devices), 5)
         self.assertIsInstance(status.devices[0], Device)
-        self.assertEqual(status.devices[0].type, Wifi.WIFI_5G)
+        self.assertEqual(status.devices[0].type, Connection.HOST_5G)
         self.assertEqual(status.devices[0].macaddr, 'CF-51-C9-04-E1-02')
         self.assertIsInstance(status.devices[0].macaddress, macaddress.EUI48)
         self.assertEqual(status.devices[0].ipaddr, '192.168.68.101')
         self.assertIsInstance(status.devices[0].ipaddress, ipaddress.IPv4Address)
         self.assertEqual(status.devices[0].hostname, 'wireless1')
         self.assertEqual(status.devices[0].packets_sent, None)
         self.assertEqual(status.devices[0].packets_received, None)
         self.assertIsInstance(status.devices[1], Device)
-        self.assertEqual(status.devices[1].type, Wifi.WIFI_2G)
-        self.assertEqual(status.devices[1].macaddr, '6B-35-FE-21-A7-73')
-        self.assertIsInstance(status.devices[1].macaddress, macaddress.EUI48)
-        self.assertEqual(status.devices[1].ipaddr, '192.168.68.103')
-        self.assertIsInstance(status.devices[1].ipaddress, ipaddress.IPv4Address)
-        self.assertEqual(status.devices[1].hostname, 'wireless3')
+        self.assertEqual(status.devices[1].type, Connection.WIRED)
+        self.assertEqual(status.devices[1].macaddr, '5F-F8-08-28-AF-54')
+        self.assertEqual(status.devices[1].ipaddr, '192.168.68.100')
+        self.assertEqual(status.devices[1].hostname, 'wired1')
         self.assertEqual(status.devices[1].packets_sent, None)
         self.assertEqual(status.devices[1].packets_received, None)
         self.assertIsInstance(status.devices[2], Device)
-        self.assertEqual(status.devices[2].type, Wifi.WIFI_GUEST_5G)
-        self.assertEqual(status.devices[2].macaddr, '19-90-F7-61-66-B2')
-        self.assertIsInstance(status.devices[2].macaddress, macaddress.EUI48)
-        self.assertEqual(status.devices[2].ipaddr, '192.168.68.104')
-        self.assertIsInstance(status.devices[2].ipaddress, ipaddress.IPv4Address)
-        self.assertEqual(status.devices[2].hostname, 'wireless4')
+        self.assertEqual(status.devices[2].type, Connection.HOST_2G)
+        self.assertEqual(status.devices[2].macaddr, '6B-35-FE-21-A7-73')
+        self.assertEqual(status.devices[2].ipaddr, '192.168.68.103')
+        self.assertEqual(status.devices[2].hostname, 'wireless3')
         self.assertEqual(status.devices[2].packets_sent, None)
         self.assertEqual(status.devices[2].packets_received, None)
         self.assertIsInstance(status.devices[3], Device)
-        self.assertEqual(status.devices[3].type, Wifi.WIFI_GUEST_2G)
-        self.assertEqual(status.devices[3].macaddr, '56-32-C3-DE-CE-F0')
-        self.assertIsInstance(status.devices[3].macaddress, macaddress.EUI48)
-        self.assertEqual(status.devices[3].ipaddr, '192.168.68.105')
-        self.assertIsInstance(status.devices[3].ipaddress, ipaddress.IPv4Address)
-        self.assertEqual(status.devices[3].hostname, 'wireless5')
+        self.assertEqual(status.devices[3].type, Connection.GUEST_5G)
+        self.assertEqual(status.devices[3].macaddr, '19-90-F7-61-66-B2')
+        self.assertEqual(status.devices[3].ipaddr, '192.168.68.104')
+        self.assertEqual(status.devices[3].hostname, 'wireless4')
         self.assertEqual(status.devices[3].packets_sent, None)
         self.assertEqual(status.devices[3].packets_received, None)
+        self.assertIsInstance(status.devices[4], Device)
+        self.assertEqual(status.devices[4].type, Connection.GUEST_2G)
+        self.assertEqual(status.devices[4].macaddr, '56-32-C3-DE-CE-F0')
+        self.assertEqual(status.devices[4].ipaddr, '192.168.68.105')
+        self.assertEqual(status.devices[4].hostname, 'wireless5')
+        self.assertEqual(status.devices[4].packets_sent, None)
+        self.assertEqual(status.devices[4].packets_received, None)
 
     def test_get_status_iot(self) -> None:
         response_network = '''
 {"result": {
     "wan": {
         "ip_info": {
             "mac": "44:e1:52:8c:40:36", "dns2": "0.0.0.0", "dns1": "0.0.0.0", "mask": "", "gateway": "", "ip": ""
@@ -239,28 +240,28 @@
         self.assertEqual(status.iot_6g_enable, None)
         self.assertEqual(status.wifi_2g_enable, True)
         self.assertEqual(status.wifi_5g_enable, False)
         self.assertEqual(status.wifi_6g_enable, True)
 
         self.assertEqual(len(status.devices), 5)
         self.assertIsInstance(status.devices[0], Device)
-        self.assertEqual(status.devices[0].type, Wifi.WIFI_5G)
+        self.assertEqual(status.devices[0].type, Connection.HOST_5G)
         self.assertEqual(status.devices[0].macaddr, 'CF-51-C9-04-E1-02')
         self.assertIsInstance(status.devices[0].macaddress, macaddress.EUI48)
         self.assertIsInstance(status.devices[1], Device)
-        self.assertEqual(status.devices[1].type, Wifi.WIFI_IOT_2G)
+        self.assertEqual(status.devices[1].type, Connection.IOT_2G)
         self.assertEqual(status.devices[1].macaddr, '5F-F8-08-28-AF-54')
         self.assertIsInstance(status.devices[2], Device)
-        self.assertEqual(status.devices[2].type, Wifi.WIFI_IOT_5G)
+        self.assertEqual(status.devices[2].type, Connection.IOT_5G)
         self.assertEqual(status.devices[2].macaddr, '5F-F8-08-28-AF-55')
         self.assertIsInstance(status.devices[3], Device)
-        self.assertEqual(status.devices[3].type, Wifi.WIFI_IOT_6G)
+        self.assertEqual(status.devices[3].type, Connection.IOT_6G)
         self.assertEqual(status.devices[3].macaddr, '5F-F8-08-28-AF-56')
         self.assertIsInstance(status.devices[4], Device)
-        self.assertEqual(status.devices[4].type, Wifi.WIFI_UNKNOWN)
+        self.assertEqual(status.devices[4].type, Connection.UNKNOWN)
         self.assertEqual(status.devices[4].macaddr, '5F-F8-08-28-AF-57')
 
     def test_get_status_no_internet(self) -> None:
         response_network = '''
 {"result": {
     "wan": {
         "ip_info": {
@@ -474,29 +475,29 @@
             def request(self, path: str, data: str,
                         ignore_response: bool = False, ignore_errors: bool = False) -> dict | None:
                 nonlocal check_url, check_data
                 check_url = path
                 check_data = data
 
         client = TPLinkRouterTest('', '')
-        result = client.set_wifi(Wifi.WIFI_2G, False)
+        result = client.set_wifi(Connection.HOST_2G, False)
         self.assertIsNone(result)
         self.assertEqual(check_url, 'admin/wireless?form=wlan')
         self.assertEqual(check_data, '{"operation": "write", "params": {"band2_4": {"host": {"enable": false}}}}')
-        client.set_wifi(Wifi.WIFI_2G, True)
+        client.set_wifi(Connection.HOST_2G, True)
         self.assertEqual(check_data, '{"operation": "write", "params": {"band2_4": {"host": {"enable": true}}}}')
-        client.set_wifi(Wifi.WIFI_5G, True)
+        client.set_wifi(Connection.HOST_5G, True)
         self.assertEqual(check_data, '{"operation": "write", "params": {"band5_1": {"host": {"enable": true}}}}')
-        client.set_wifi(Wifi.WIFI_GUEST_2G, True)
+        client.set_wifi(Connection.GUEST_2G, True)
         self.assertEqual(check_data, '{"operation": "write", "params": {"band2_4": {"guest": {"enable": true}}}}')
-        client.set_wifi(Wifi.WIFI_GUEST_5G, True)
+        client.set_wifi(Connection.GUEST_5G, True)
         self.assertEqual(check_data, '{"operation": "write", "params": {"band5_1": {"guest": {"enable": true}}}}')
-        client.set_wifi(Wifi.WIFI_6G, True)
+        client.set_wifi(Connection.HOST_6G, True)
         self.assertEqual(check_data, '{"operation": "write", "params": {"band6": {"host": {"enable": true}}}}')
-        client.set_wifi(Wifi.WIFI_GUEST_6G, True)
+        client.set_wifi(Connection.GUEST_6G, True)
         self.assertEqual(check_data, '{"operation": "write", "params": {"band6": {"guest": {"enable": true}}}}')
 
     def test_reboot_with_firmware(self) -> None:
         check_url = ''
         check_data = ''
 
         class TPLinkRouterTest(TPLinkDecoClient):
```

### Comparing `tplinkrouterc6u-3.5.0/test/test_client_mr.py` & `tplinkrouterc6u-4.0.0/test/test_client_mr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 import macaddress
 import ipaddress
 from tplinkrouterc6u import (
     TPLinkMRClient,
-    Wifi,
+    Connection,
     Firmware,
     Status,
     Device,
     IPv4Reservation,
     IPv4DHCPLease,
     IPv4Status,
 )
@@ -177,24 +177,33 @@
         self.assertEqual(status.iot_2g_enable, None)
         self.assertEqual(status.iot_5g_enable, None)
         self.assertEqual(status.wifi_2g_enable, True)
         self.assertEqual(status.wifi_5g_enable, False)
         self.assertEqual(status.wan_ipv4_uptime, None)
         self.assertEqual(status.mem_usage, None)
         self.assertEqual(status.cpu_usage, None)
-        self.assertEqual(len(status.devices), 1)
+        self.assertEqual(len(status.devices), 2)
         self.assertIsInstance(status.devices[0], Device)
-        self.assertEqual(status.devices[0].type, Wifi.WIFI_5G)
-        self.assertEqual(status.devices[0].macaddr, 'F4-A3-86-2D-41-B5')
+        self.assertEqual(status.devices[0].type, Connection.WIRED)
+        self.assertEqual(status.devices[0].macaddr, '66-E2-02-BD-B5-1B')
         self.assertIsInstance(status.devices[0].macaddress, macaddress.EUI48)
-        self.assertEqual(status.devices[0].ipaddr, '192.168.30.11')
+        self.assertEqual(status.devices[0].ipaddr, '192.168.30.10')
         self.assertIsInstance(status.devices[0].ipaddress, ipaddress.IPv4Address)
-        self.assertEqual(status.devices[0].hostname, 'host2')
-        self.assertEqual(status.devices[0].packets_sent, 176)
-        self.assertEqual(status.devices[0].packets_received, 467)
+        self.assertEqual(status.devices[0].hostname, 'host1')
+        self.assertEqual(status.devices[0].packets_sent, None)
+        self.assertEqual(status.devices[0].packets_received, None)
+        self.assertIsInstance(status.devices[1], Device)
+        self.assertEqual(status.devices[1].type, Connection.HOST_5G)
+        self.assertEqual(status.devices[1].macaddr, 'F4-A3-86-2D-41-B5')
+        self.assertIsInstance(status.devices[1].macaddress, macaddress.EUI48)
+        self.assertEqual(status.devices[1].ipaddr, '192.168.30.11')
+        self.assertIsInstance(status.devices[1].ipaddress, ipaddress.IPv4Address)
+        self.assertEqual(status.devices[1].hostname, 'host2')
+        self.assertEqual(status.devices[1].packets_sent, 176)
+        self.assertEqual(status.devices[1].packets_received, 467)
 
     def test_get_status_without_5G(self) -> None:
         response = '''[1,1,0,0,0,0]0
 X_TP_MACAddress=a0:28:84:de:dd:5c
 IPInterfaceIPAddress=192.168.4.1
 [1,1,1,0,0,0]1
 enable=0
@@ -241,15 +250,24 @@
         self.assertEqual(status.iot_2g_enable, None)
         self.assertEqual(status.iot_5g_enable, None)
         self.assertEqual(status.wifi_2g_enable, True)
         self.assertEqual(status.wifi_5g_enable, None)
         self.assertEqual(status.wan_ipv4_uptime, None)
         self.assertEqual(status.mem_usage, None)
         self.assertEqual(status.cpu_usage, None)
-        self.assertEqual(len(status.devices), 0)
+        self.assertEqual(len(status.devices), 1)
+        self.assertIsInstance(status.devices[0], Device)
+        self.assertEqual(status.devices[0].type, Connection.WIRED)
+        self.assertEqual(status.devices[0].macaddr, '66-E2-02-BD-B5-1B')
+        self.assertIsInstance(status.devices[0].macaddress, macaddress.EUI48)
+        self.assertEqual(status.devices[0].ipaddr, '192.168.30.10')
+        self.assertIsInstance(status.devices[0].ipaddress, ipaddress.IPv4Address)
+        self.assertEqual(status.devices[0].hostname, 'host1')
+        self.assertEqual(status.devices[0].packets_sent, None)
+        self.assertEqual(status.devices[0].packets_received, None)
 
     def test_get_status_with_wlan_dev(self) -> None:
         response = '''
 [1,1,0,0,0,0]0
 X_TP_MACAddress=a0:28:84:de:dd:5c
 IPInterfaceIPAddress=192.168.4.1
 [1,1,1,0,0,0]1
@@ -299,15 +317,15 @@
         self.assertEqual(status.wifi_2g_enable, True)
         self.assertEqual(status.wifi_5g_enable, None)
         self.assertEqual(status.wifi_6g_enable, None)
         self.assertEqual(status.wan_ipv4_uptime, None)
         self.assertEqual(status.mem_usage, None)
         self.assertEqual(status.cpu_usage, None)
         self.assertEqual(len(status.devices), 1)
-        self.assertEqual(status.devices[0].type, Wifi.WIFI_2G)
+        self.assertEqual(status.devices[0].type, Connection.HOST_2G)
         self.assertEqual(status.devices[0].macaddr, 'F4-A3-86-2D-41-B8')
         self.assertEqual(status.devices[0].ipaddr, '0.0.0.0')
         self.assertEqual(status.devices[0].hostname, '')
         self.assertEqual(status.devices[0].packets_sent, 176)
         self.assertEqual(status.devices[0].packets_received, 467)
 
     def test_get_status_two_lan_ip(self) -> None:
@@ -582,15 +600,15 @@
             def _request(self, url, method='POST', data_str=None, encrypt=False):
                 nonlocal check_url, check_data
                 check_url = url
                 check_data = data_str
                 return 200, response
 
         client = TPLinkMRClientTest('', '')
-        client.set_wifi(Wifi.WIFI_2G, True)
+        client.set_wifi(Connection.HOST_2G, True)
 
         self.assertIn('http:///cgi_gdpr?_=', check_url)
         self.assertEqual(check_data, '2\r\n[LAN_WLAN#1,1,0,0,0,0#0,0,0,0,0,0]0,1\r\nenable=1\r\n')
 
     def test_send_sms(self) -> None:
         response = '''
 [error]0
```

### Comparing `tplinkrouterc6u-3.5.0/tplinkrouterc6u/client.py` & `tplinkrouterc6u-4.0.0/tplinkrouterc6u/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import urllib
 import requests
 import datetime
 import macaddress
 import ipaddress
 from logging import Logger
 from tplinkrouterc6u.encryption import EncryptionWrapper, EncryptionWrapperMR
-from tplinkrouterc6u.enum import Wifi
+from tplinkrouterc6u.enum import Connection
 from tplinkrouterc6u.dataclass import Firmware, Status, Device, IPv4Reservation, IPv4DHCPLease, IPv4Status
 from tplinkrouterc6u.exception import ClientException, ClientError
 from abc import ABC, abstractmethod
 
 
 class AbstractRouter(ABC):
     def __init__(self, host: str, password: str, username: str = 'admin', logger: Logger = None,
@@ -51,15 +51,15 @@
         pass
 
     @abstractmethod
     def reboot(self) -> None:
         pass
 
     @abstractmethod
-    def set_wifi(self, wifi: Wifi, enable: bool) -> None:
+    def set_wifi(self, wifi: Connection, enable: bool) -> None:
         pass
 
 
 class TplinkRequest:
     host = ''
     _stok = ''
     timeout = 10
@@ -261,33 +261,47 @@
         return {'sign': sign, 'data': encrypted_data}
 
     def _decrypt_response(self, data: dict) -> dict:
         return json.loads(self._encryption.aes_decrypt(data['data']))
 
 
 class TplinkBaseRouter(AbstractRouter, TplinkRequest):
+    _smart_network = True
+    _perf_status = True
+
     def __init__(self, host: str, password: str, username: str = 'admin', logger: Logger = None,
                  verify_ssl: bool = True, timeout: int = 10) -> None:
         super().__init__(host, password, username, logger, verify_ssl, timeout)
 
         self._url_firmware = 'admin/firmware?form=upgrade&operation=read'
-        self._url_wireless_stats = 'admin/wireless?form=statistics'
         self._url_ipv4_reservations = 'admin/dhcps?form=reservation&operation=load'
         self._url_ipv4_dhcp_leases = 'admin/dhcps?form=client&operation=load'
         referer = '{}/webpages/index.html'.format(self.host)
         self._headers_request = {'Referer': referer}
         self._headers_login = {'Referer': referer, 'Content-Type': 'application/x-www-form-urlencoded'}
 
     @abstractmethod
     def authorize(self) -> bool:
         pass
 
-    def set_wifi(self, wifi: Wifi, enable: bool) -> None:
-        path = f"admin/wireless?&form=guest&form={wifi.value}"
-        data = f"operation=write&{wifi.value}_enable={'on' if enable else 'off'}"
+    def set_wifi(self, wifi: Connection, enable: bool) -> None:
+        values = {
+            Connection.HOST_2G: 'wireless_2g',
+            Connection.HOST_5G: 'wireless_5g',
+            Connection.HOST_6G: 'wireless_6g',
+            Connection.GUEST_2G: 'guest_2g',
+            Connection.GUEST_5G: 'guest_5g',
+            Connection.GUEST_6G: 'guest_6g',
+            Connection.IOT_2G: 'iot_2g',
+            Connection.IOT_5G: 'iot_5g',
+            Connection.IOT_6G: 'iot_6g',
+        }
+        value = values.get(wifi)
+        path = f"admin/wireless?&form=guest&form={value}"
+        data = f"operation=write&{value}_enable={'on' if enable else 'off'}"
         self.request(path, data)
 
     def reboot(self) -> None:
         self.request('admin/system?form=reboot', 'operation=write', True)
 
     def logout(self) -> None:
         self.request('admin/system?form=logout', 'operation=write', True)
@@ -298,64 +312,90 @@
     def get_firmware(self) -> Firmware:
         data = self.request(self._url_firmware, 'operation=read')
         firmware = Firmware(data.get('hardware_version', ''), data.get('model', ''), data.get('firmware_version', ''))
 
         return firmware
 
     def get_status(self) -> Status:
-
-        def _calc_cpu_usage(data: dict) -> float | None:
-            cpu_usage = (data.get('cpu_usage', 0) + data.get('cpu1_usage', 0)
-                         + data.get('cpu2_usage', 0) + data.get('cpu3_usage', 0))
-            return cpu_usage / 4 if cpu_usage != 0 else None
-
         data = self.request('admin/status?form=all&operation=read', 'operation=read')
         status = Status()
         status._wan_macaddr = macaddress.EUI48(data['wan_macaddr']) if 'wan_macaddr' in data else None
         status._lan_macaddr = macaddress.EUI48(data['lan_macaddr'])
         status._wan_ipv4_addr = ipaddress.IPv4Address(data['wan_ipv4_ipaddr']) if 'wan_ipv4_ipaddr' in data else None
         status._lan_ipv4_addr = ipaddress.IPv4Address(data['lan_ipv4_ipaddr']) if 'lan_ipv4_ipaddr' in data else None
         status._wan_ipv4_gateway = ipaddress.IPv4Address(
             data['wan_ipv4_gateway']) if 'wan_ipv4_gateway' in data else None
         status.wan_ipv4_uptime = data.get('wan_ipv4_uptime')
         status.mem_usage = data.get('mem_usage')
-        status.cpu_usage = _calc_cpu_usage(data)
+        status.cpu_usage = data.get('cpu_usage')
         status.wired_total = len(data.get('access_devices_wired', []))
         status.wifi_clients_total = len(data.get('access_devices_wireless_host', []))
         status.guest_clients_total = len(data.get('access_devices_wireless_guest', []))
         status.guest_2g_enable = self._str2bool(data.get('guest_2g_enable'))
         status.guest_5g_enable = self._str2bool(data.get('guest_5g_enable'))
         status.guest_6g_enable = self._str2bool(data.get('guest_6g_enable'))
         status.iot_2g_enable = self._str2bool(data.get('iot_2g_enable'))
         status.iot_5g_enable = self._str2bool(data.get('iot_5g_enable'))
         status.iot_6g_enable = self._str2bool(data.get('iot_6g_enable'))
         status.wifi_2g_enable = self._str2bool(data.get('wireless_2g_enable'))
         status.wifi_5g_enable = self._str2bool(data.get('wireless_5g_enable'))
         status.wifi_6g_enable = self._str2bool(data.get('wireless_6g_enable'))
 
+        if (status.mem_usage is None or status.mem_usage is None) and self._perf_status:
+            try:
+                performance = self.request('admin/status?form=perf&operation=read', 'operation=read')
+                status.mem_usage = performance.get('mem_usage')
+                status.cpu_usage = performance.get('cpu_usage')
+            except:
+                self._perf_status = False
+
         devices = {}
 
-        def _add_device(type: Wifi, item: dict) -> None:
-            devices[item['macaddr']] = Device(type, macaddress.EUI48(item['macaddr']),
+        def _add_device(conn: Connection, item: dict) -> None:
+            devices[item['macaddr']] = Device(conn, macaddress.EUI48(item['macaddr']),
                                               ipaddress.IPv4Address(item['ipaddr']),
                                               item['hostname'])
 
+        for item in data.get('access_devices_wired', []):
+            type = self._map_wire_type(item.get('wire_type'))
+            _add_device(type, item)
+
         for item in data.get('access_devices_wireless_host', []):
             type = self._map_wire_type(item.get('wire_type'))
             _add_device(type, item)
 
         for item in data.get('access_devices_wireless_guest', []):
             type = self._map_wire_type(item.get('wire_type'), False)
             _add_device(type, item)
 
-        for item in self.request(self._url_wireless_stats, 'operation=load'):
+        smart_network = None
+        if self._smart_network:
+            try:
+                smart_network = self.request('admin/smart_network?form=game_accelerator', 'operation=loadDevice')
+            except Exception:
+                self._smart_network = False
+
+        if smart_network:
+            for item in smart_network:
+                if item['mac'] not in devices:
+                    conn = self._map_wire_type(item.get('deviceTag'), not item.get('isGuest'))
+                    devices[item['mac']] = Device(conn, macaddress.EUI48(item['mac']),
+                                                  ipaddress.IPv4Address(item['ip']),
+                                                  item['deviceName'])
+                    if conn.is_iot():
+                        if status.iot_clients_total is None:
+                            status.iot_clients_total = 0
+                        status.iot_clients_total += 1
+
+        for item in self.request('admin/wireless?form=statistics', 'operation=load'):
             if item['mac'] not in devices:
                 status.wifi_clients_total += 1
                 type = self._map_wire_type(item.get('type'))
-                devices[item['mac']] = Device(type, macaddress.EUI48(item['mac']), ipaddress.IPv4Address('0.0.0.0'), '')
+                devices[item['mac']] = Device(type, macaddress.EUI48(item['mac']), ipaddress.IPv4Address('0.0.0.0'),
+                                              '')
             devices[item['mac']].packets_sent = item.get('txpkts')
             devices[item['mac']].packets_received = item.get('rxpkts')
 
         status.devices = list(devices.values())
         status.clients_total = status.wired_total + status.wifi_clients_total + status.guest_clients_total
 
         return status
@@ -401,34 +441,41 @@
         return dhcp_leases
 
     @staticmethod
     def _str2bool(v) -> bool | None:
         return str(v).lower() in ("yes", "true", "on") if v is not None else None
 
     @staticmethod
-    def _map_wire_type(data: str | None, host: bool = True) -> Wifi:
-        result = Wifi.WIFI_UNKNOWN
+    def _map_wire_type(data: str | None, host: bool = True) -> Connection:
+        result = Connection.UNKNOWN
         if data is None:
             return result
+        if data == 'wired':
+            result = Connection.WIRED
         if data.startswith('2.4'):
-            result = Wifi.WIFI_2G if host else Wifi.WIFI_GUEST_2G
+            result = Connection.HOST_2G if host else Connection.GUEST_2G
         elif data.startswith('5'):
-            result = Wifi.WIFI_5G if host else Wifi.WIFI_GUEST_5G
+            result = Connection.HOST_5G if host else Connection.GUEST_5G
         elif data.startswith('6'):
-            result = Wifi.WIFI_6G if host else Wifi.WIFI_GUEST_6G
+            result = Connection.HOST_6G if host else Connection.GUEST_6G
+        elif data.startswith('iot_2'):
+            result = Connection.IOT_2G
+        elif data.startswith('iot_5'):
+            result = Connection.IOT_5G
+        elif data.startswith('iot_6'):
+            result = Connection.IOT_6G
         return result
 
 
 class TplinkRouter(TplinkEncryption, TplinkBaseRouter):
     def __init__(self, host: str, password: str, username: str = 'admin', logger: Logger = None,
                  verify_ssl: bool = True, timeout: int = 10) -> None:
         super().__init__(host, password, username, logger, verify_ssl, timeout)
 
         self._url_firmware = 'admin/firmware?form=upgrade'
-        self._url_wireless_stats = 'admin/wireless?form=statistics'
         self._url_ipv4_reservations = 'admin/dhcps?form=reservation'
         self._url_ipv4_dhcp_leases = 'admin/dhcps?form=client'
 
 
 class TPLinkDecoClient(TplinkEncryption, AbstractRouter):
     def __init__(self, host: str, password: str, username: str = 'admin', logger: Logger = None,
                  verify_ssl: bool = True, timeout: int = 10) -> None:
@@ -441,25 +488,25 @@
 
     def logout(self) -> None:
         self.request('admin/system?form=logout', json.dumps({'operation': 'logout'}), True)
         self._stok = ''
         self._sysauth = ''
         self._logged = False
 
-    def set_wifi(self, wifi: Wifi, enable: bool) -> None:
+    def set_wifi(self, wifi: Connection, enable: bool) -> None:
         en = {'enable': enable}
-        if Wifi.WIFI_2G == wifi:
+        if Connection.HOST_2G == wifi:
             params = {'band2_4': {'host': en}}
-        elif Wifi.WIFI_5G == wifi:
+        elif Connection.HOST_5G == wifi:
             params = {'band5_1': {'host': en}}
-        elif Wifi.WIFI_GUEST_5G == wifi:
+        elif Connection.GUEST_5G == wifi:
             params = {'band5_1': {'guest': en}}
-        elif Wifi.WIFI_6G == wifi:
+        elif Connection.HOST_6G == wifi:
             params = {'band6': {'host': en}}
-        elif Wifi.WIFI_GUEST_6G == wifi:
+        elif Connection.GUEST_6G == wifi:
             params = {'band6': {'guest': en}}
         else:
             params = {'band2_4': {'guest': en}}
 
         self.request('admin/wireless?form=wlan', json.dumps({'operation': 'write', 'params': params}))
 
     def reboot(self) -> None:
@@ -511,29 +558,28 @@
         devices = []
         data = self.request('admin/client?form=client_list', json.dumps(
             {"operation": "read", "params": {"device_mac": "default"}})).get('client_list', [])
 
         for item in data:
             if not item.get('online'):
                 continue
-            if item.get('wire_type') == 'wired':
+            conn = self._map_wire_type(item)
+            if conn == Connection.WIRED:
                 status.wired_total += 1
-                continue
-            wifi = self._map_wire_type(item)
-            if wifi in [Wifi.WIFI_2G, Wifi.WIFI_5G, Wifi.WIFI_6G]:
+            elif conn.is_host_wifi():
                 status.wifi_clients_total += 1
-            elif wifi in [Wifi.WIFI_GUEST_2G, Wifi.WIFI_GUEST_5G, Wifi.WIFI_GUEST_5G]:
+            elif conn.is_guest_wifi():
                 status.guest_clients_total += 1
-            elif wifi in [Wifi.WIFI_IOT_2G, Wifi.WIFI_IOT_5G, Wifi.WIFI_IOT_6G]:
+            elif conn.is_iot():
                 if status.iot_clients_total is None:
                     status.iot_clients_total = 0
                 status.iot_clients_total += 1
 
             ip = item['ip'] if item.get('ip') else '0.0.0.0'
-            devices.append(Device(wifi,
+            devices.append(Device(conn,
                                   macaddress.EUI48(item['mac']),
                                   ipaddress.IPv4Address(ip),
                                   base64.b64decode(item['name']).decode()))
 
         status.clients_total = (status.wired_total + status.wifi_clients_total + status.guest_clients_total
                                 + (0 if status.iot_clients_total is None else status.iot_clients_total))
         status.devices = devices
@@ -567,36 +613,69 @@
         for key in keys:
             try:
                 nested_dict = nested_dict[key]
             except Exception:
                 return None
         return nested_dict
 
-    def _map_wire_type(self, data: dict) -> Wifi:
-        mapping = {'band2_4': {'main': Wifi.WIFI_2G, 'guest': Wifi.WIFI_GUEST_2G, 'iot': Wifi.WIFI_IOT_2G},
-                   'band5': {'main': Wifi.WIFI_5G, 'guest': Wifi.WIFI_GUEST_5G, 'iot': Wifi.WIFI_IOT_5G},
-                   'band6': {'main': Wifi.WIFI_6G, 'guest': Wifi.WIFI_GUEST_6G, 'iot': Wifi.WIFI_IOT_6G}
+    def _map_wire_type(self, data: dict) -> Connection:
+        if data.get('wire_type') == 'wired':
+            return Connection.WIRED
+        mapping = {'band2_4': {'main': Connection.HOST_2G, 'guest': Connection.GUEST_2G, 'iot': Connection.IOT_2G},
+                   'band5': {'main': Connection.HOST_5G, 'guest': Connection.GUEST_5G, 'iot': Connection.IOT_5G},
+                   'band6': {'main': Connection.HOST_6G, 'guest': Connection.GUEST_6G, 'iot': Connection.IOT_6G}
                    }
         result = self._get_value(mapping, [data.get('connection_type'), data.get('interface')])
 
-        return result if result else Wifi.WIFI_UNKNOWN
+        return result if result else Connection.UNKNOWN
 
     @staticmethod
     def _get_login_data(crypted_pwd: str) -> str:
         data = {
             "params": {"password": crypted_pwd},
             "operation": "login",
         }
 
         return json.dumps(data)
 
     def _is_valid_response(self, data: dict) -> bool:
         return 'error_code' in data and data['error_code'] == 0
 
 
+class TplinkC6V4Router(AbstractRouter):
+    def supports(self) -> bool:
+        url = '{}/?code=2&asyn=1'.format(self.host)
+        try:
+            response = requests.post(url, timeout=self.timeout, verify=self._verify_ssl)
+        except:
+            return False
+        if response.status_code == 401 and response.text.startswith('00'):
+            raise ClientException(
+                'Your router is not supported. Please add your router support to https://github.com/AlexandrErohin/TP-Link-Archer-C6U by implementing methods for TplinkC6V4Router class')
+        return False
+
+    def authorize(self) -> None:
+        raise ClientException('Not Implemented')
+
+    def logout(self) -> None:
+        raise ClientException('Not Implemented')
+
+    def get_firmware(self) -> Firmware:
+        raise ClientException('Not Implemented')
+
+    def get_status(self) -> Status:
+        raise ClientException('Not Implemented')
+
+    def reboot(self) -> None:
+        raise ClientException('Not Implemented')
+
+    def set_wifi(self, wifi: Connection, enable: bool) -> None:
+        raise ClientException('Not Implemented')
+
+
 class TplinkC1200Router(TplinkBaseRouter):
     def supports(self) -> bool:
         return True
 
     def authorize(self) -> None:
         if len(self.password) < 200:
             raise Exception('You need to use web encrypted password instead. Check the documentation!')
@@ -634,32 +713,27 @@
     }
 
     HTTP_RET_OK = 0
     HTTP_ERR_CGI_INVALID_ANSI = 71017
     HTTP_ERR_USER_PWD_NOT_CORRECT = 71233
     HTTP_ERR_USER_BAD_REQUEST = 71234
 
-    LAN = 0
-    WIFI_2G = 1
-    WIFI_5G = 3
-    WIFI_GUEST_2G = 2
-    WIFI_GUEST_5G = 4
-
     CLIENT_TYPES = {
-        WIFI_2G: Wifi.WIFI_2G,
-        WIFI_5G: Wifi.WIFI_5G,
-        WIFI_GUEST_2G: Wifi.WIFI_GUEST_2G,
-        WIFI_GUEST_5G: Wifi.WIFI_GUEST_5G,
+        0: Connection.WIRED,
+        1: Connection.HOST_2G,
+        3: Connection.HOST_5G,
+        2: Connection.GUEST_2G,
+        4: Connection.GUEST_5G,
     }
 
     WIFI_SET = {
-        Wifi.WIFI_2G: '1,1,0,0,0,0',
-        Wifi.WIFI_5G: '1,2,0,0,0,0',
-        Wifi.WIFI_GUEST_2G: '1,1,1,0,0,0',
-        Wifi.WIFI_GUEST_5G: '1,2,1,0,0,0',
+        Connection.HOST_2G: '1,1,0,0,0,0',
+        Connection.HOST_5G: '1,2,0,0,0,0',
+        Connection.GUEST_2G: '1,1,1,0,0,0',
+        Connection.GUEST_5G: '1,2,1,0,0,0',
     }
 
     class ActItem:
         GET = 1
         SET = 2
         ADD = 3
         DEL = 4
@@ -792,34 +866,33 @@
             status.guest_2g_enable = bool(int(values['3'][0]['enable']))
             status.guest_5g_enable = bool(int(values['3'][1]['enable']))
 
         devices = {}
         for val in self._to_list(values.get('4')):
             if int(val['active']) == 0:
                 continue
-            type = int(val['X_TP_ConnType'])
-            if type == self.LAN:
-                status.wired_total += 1
+            conn = self.CLIENT_TYPES.get(int(val['X_TP_ConnType']))
+            if conn is None:
                 continue
-            if type in [self.WIFI_GUEST_2G, self.WIFI_GUEST_5G]:
+            elif conn == Connection.WIRED:
+                status.wired_total += 1
+            elif conn.is_guest_wifi():
                 status.guest_clients_total += 1
-            elif type in [self.WIFI_2G, self.WIFI_5G]:
+            elif conn.is_host_wifi():
                 status.wifi_clients_total += 1
-            else:
-                continue
-            devices[val['MACAddress']] = Device(self.CLIENT_TYPES[type],
+            devices[val['MACAddress']] = Device(conn,
                                                 macaddress.EUI48(val['MACAddress']),
                                                 ipaddress.IPv4Address(val['IPAddress']),
                                                 val['hostName'])
 
         for val in self._to_list(values.get('5')):
             if val['associatedDeviceMACAddress'] not in devices:
                 status.wifi_clients_total += 1
                 devices[val['associatedDeviceMACAddress']] = Device(
-                    Wifi.WIFI_2G,
+                    Connection.HOST_2G,
                     macaddress.EUI48(val['associatedDeviceMACAddress']),
                     ipaddress.IPv4Address('0.0.0.0'),
                     '')
             devices[val['associatedDeviceMACAddress']].packets_sent = int(val['X_TP_TotalPacketsSent'])
             devices[val['associatedDeviceMACAddress']].packets_received = int(val['X_TP_TotalPacketsReceived'])
 
         status.devices = list(devices.values())
@@ -891,19 +964,19 @@
             ipv4_status._wan_ipv4_netmask = ipaddress.IPv4Address(item['subnetMask'])
             dns = item['DNSServers'].split(',')
             ipv4_status._wan_ipv4_pridns = ipaddress.IPv4Address(dns[0])
             ipv4_status._wan_ipv4_snddns = ipaddress.IPv4Address(dns[1])
 
         return ipv4_status
 
-    def set_wifi(self, wifi: Wifi, enable: bool) -> None:
+    def set_wifi(self, wifi: Connection, enable: bool) -> None:
         acts = [
             self.ActItem(
                 self.ActItem.SET,
-                'LAN_WLAN' if wifi in [Wifi.WIFI_2G, Wifi.WIFI_5G] else 'LAN_WLAN_MSSIDENTRY',
+                'LAN_WLAN' if wifi in [Connection.HOST_2G, Connection.HOST_5G] else 'LAN_WLAN_MSSIDENTRY',
                 self.WIFI_SET[wifi],
                 attrs=['enable={}'.format(int(enable))]),
         ]
         self.req_act(acts)
 
     def send_sms(self, phone_number: str, message: str) -> None:
         acts = [
@@ -1175,13 +1248,13 @@
         return signature, encrypted_data
 
 
 class TplinkRouterProvider:
     @staticmethod
     def get_client(host: str, password: str, username: str = 'admin', logger: Logger = None,
                    verify_ssl: bool = True, timeout: int = 10) -> AbstractRouter | None:
-        for client in [TPLinkMRClient, TPLinkDecoClient, TplinkRouter, TplinkC1200Router]:
+        for client in [TPLinkMRClient, TplinkC6V4Router, TPLinkDecoClient, TplinkRouter, TplinkC1200Router]:
             router = client(host, password, username, logger, verify_ssl, timeout)
             if router.supports():
                 return router
 
         return None
```

### Comparing `tplinkrouterc6u-3.5.0/tplinkrouterc6u/dataclass.py` & `tplinkrouterc6u-4.0.0/tplinkrouterc6u/dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import macaddress
 import ipaddress
 from dataclasses import dataclass, field
-from tplinkrouterc6u.enum import Wifi
+from tplinkrouterc6u.enum import Connection
 
 
 @dataclass
 class Firmware:
     def __init__(self, hardware: str, model: str, firmware: str) -> None:
         self.hardware_version = hardware
         self.model = model
         self.firmware_version = firmware
 
 
 @dataclass
 class Device:
-    def __init__(self, type: Wifi, macaddr: macaddress, ipaddr: ipaddress, hostname: str) -> None:
+    def __init__(self, type: Connection, macaddr: macaddress, ipaddr: ipaddress, hostname: str) -> None:
         self.type = type
         self._macaddr = macaddr
         self._ipaddr = ipaddr
         self.hostname = hostname
         self.packets_sent: int | None = None
         self.packets_received: int | None = None
```

### Comparing `tplinkrouterc6u-3.5.0/tplinkrouterc6u/encryption.py` & `tplinkrouterc6u-4.0.0/tplinkrouterc6u/encryption.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-3.5.0/tplinkrouterc6u.egg-info/PKG-INFO` & `tplinkrouterc6u-4.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: tplinkrouterc6u
-Version: 3.5.0
-Summary: TP-Link Router API
-Home-page: https://github.com/AlexandrErohin/TP-Link-Archer-C6U
-Author: Alex Erohin
-Author-email: alexanderErohin@yandex.ru
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: pycryptodome
-Requires-Dist: macaddress
-
 # TP-Link Router API
 Python package for API access and management for TP-Link Routers. See [Supported routers](#supports)
 
 [![Pypi](https://img.shields.io/pypi/v/tplinkrouterc6u)](https://pypi.org/project/tplinkrouterc6u/)
 [![Downloads](https://static.pepy.tech/personalized-badge/tplinkrouterc6u?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pypi.org/project/tplinkrouterc6u/)
 ![Python versions](https://img.shields.io/pypi/pyversions/tplinkrouterc6u)
 
@@ -34,20 +13,20 @@
  - [pycryptodome](https://pypi.org/project/pycryptodome/)
 
 ## Usage
 Enter the host & credentials used to log in to your router management page. Username is admin by default. But you may pass username as third parameter
 
 ```python
 from tplinkrouterc6u import (
-    TplinkRouterProvider, 
+    TplinkRouterProvider,
     TplinkRouter,
     TplinkC1200Router,
     TPLinkMRClient,
     TPLinkDecoClient,
-    Wifi
+    Connection
 )
 from logging import Logger
 
 router = TplinkRouterProvider.get_client('http://192.168.0.1', 'password')
 # You may use client directly like
 # router = TplinkRouter('http://192.168.0.1', 'password')
 # You may also pass username if it is different and a logger to log errors as
@@ -61,15 +40,15 @@
     router.authorize()  # authorizing
     # Get firmware info - returns Firmware
     firmware = router.get_firmware()
 
     # Get status info - returns Status
     status = router.get_status()
     if not status.guest_2g_enable:  # check if guest 2.4G wifi is disable
-        router.set_wifi(Wifi.WIFI_GUEST_2G, True)  # turn on guest 2.4G wifi
+        router.set_wifi(Connection.GUEST_2G, True)  # turn on guest 2.4G wifi
 
     # Get Address reservations, sort by ipaddr
     reservations = router.get_ipv4_reservations()
     reservations.sort(key=lambda a: a.ipaddr)
     for res in reservations:
         print(f"{res.macaddr} {res.ipaddr:16s} {res.hostname:36} {'Permanent':12}")
 
@@ -93,25 +72,25 @@
 3. Click somewhere else on the page so that the password field is not selected anymore.
 4. Open the JavaScript console of your browser (usually by pressing F12 and then clicking on "Console").
 5. Type `document.getElementById("login-password").value;`
 6. Copy the returned value as password and use it.
 
 ## Functions
 | Function | Args | Description | Return |
-|--|--|--|--|
-| get_firmware |  | Gets firmware info about the router | [Firmware](#firmware) |
-| get_status |  | Gets status about the router info including wifi statuses and wifi clients info | [Status](#status) |
-| get_ipv4_status |  | Gets WAN and LAN IPv4 status info, gateway, DNS, netmask | [IPv4Status](#IPv4Status) |
-| get_ipv4_reservations |  | Gets IPv4 reserved addresses (static) | [[IPv4Reservation]](#IPv4Reservation) |
-| get_ipv4_dhcp_leases |  | Gets IPv4 addresses assigned via DHCP | [[IPv4DHCPLease]](#IPv4DHCPLease) | 
-| set_wifi | wifi: [Wifi](#wifi), enable: bool | Allow to turn on/of 4 wifi networks |  |
-| send_sms | phone_number: str, message: str | Send sms for LTE routers |  |
-| reboot |  | reboot router |
-| authorize |  | authorize for actions |
-| logout |  | logout after all is done |
+|---|---|---|---|
+| get_firmware |   | Gets firmware info about the router | [Firmware](#firmware) |
+| get_status |   | Gets status about the router info including wifi statuses and connected devices info | [Status](#status) |
+| get_ipv4_status |   | Gets WAN and LAN IPv4 status info, gateway, DNS, netmask | [IPv4Status](#IPv4Status) |
+| get_ipv4_reservations |   | Gets IPv4 reserved addresses (static) | [[IPv4Reservation]](#IPv4Reservation) |
+| get_ipv4_dhcp_leases |   | Gets IPv4 addresses assigned via DHCP | [[IPv4DHCPLease]](#IPv4DHCPLease) | 
+| set_wifi | wifi: [Connection](#connection), enable: bool | Allow to turn on/of 4 wifi networks |   |
+| send_sms | phone_number: str, message: str | Send sms for LTE routers |   |
+| reboot |   | reboot router |
+| authorize |   | authorize for actions |
+| logout |   | logout after all is done |
 
 ## Dataclass
 ### <a id="firmware">Firmware</a>
 | Field | Description | Type |
 | --- |----|----|
 | hardware_version | Returns like - Archer C6U | str |
 | model | Returns like - Archer C6U v1.0 | str |
@@ -127,36 +106,36 @@
 | wan_ipv4_addr | router wan ipv4 address | str, None |
 | wan_ipv4_address | router wan ipv4 address | ipaddress.IPv4Address, None |
 | lan_ipv4_addr | router lan ipv4 address | str, None |
 | lan_ipv4_address | router lan ipv4 address | ipaddress.IPv4Address, None |
 | wan_ipv4_gateway | router wan ipv4 gateway | str, None |
 | wan_ipv4_gateway_address | router wan ipv4 gateway address | ipaddress.IPv4Address, None |
 | wired_total | Total amount of wired clients | int |
-| wifi_clients_total | Total amount of main wifi clients | int |
+| wifi_clients_total | Total amount of host wifi clients | int |
 | guest_clients_total | Total amount of guest wifi clients | int |
 | clients_total | Total amount of all connected clients | int |
 | iot_clients_total | Total amount of all iot connected clients | int, None |
 | guest_2g_enable | Is guest wifi 2.4G enabled | bool |
 | guest_5g_enable | Is guest wifi 5G enabled | bool, None |
 | guest_6g_enable | Is guest wifi 6G enabled | bool, None |
 | iot_2g_enable | Is IoT wifi 2.4G enabled | bool, None |
 | iot_5g_enable | Is IoT wifi 5G enabled | bool, None |
 | iot_6g_enable | Is IoT wifi 6G enabled | bool, None |
-| wifi_2g_enable | Is main wifi 2.4G enabled | bool |
-| wifi_5g_enable | Is main wifi 5G enabled | bool, None |
-| wifi_6g_enable | Is main wifi 6G enabled | bool, None |
+| wifi_2g_enable | Is host wifi 2.4G enabled | bool |
+| wifi_5g_enable | Is host wifi 5G enabled | bool, None |
+| wifi_6g_enable | Is host wifi 6G enabled | bool, None |
 | wan_ipv4_uptime | Internet Uptime | int, None |
-| mem_usage | Memory usage | float, None |
-| cpu_usage | CPU usage | float, None |
-| devices | List of all wifi clients | list[[Device](#device)] |
+| mem_usage | Memory usage in percentage between 0 and 1 | float, None |
+| cpu_usage | CPU usage in percentage between 0 and 1 | float, None |
+| devices | List of all connectedd devices | list[[Device](#device)] |
 
 ### <a id="device">Device</a>
 | Field | Description | Type |
 | --- |---|---|
-| type | client connection type (2.4G or 5G, guest wifi or main wifi) | [Wifi](#wifi) |
+| type | client connection type (2.4G or 5G, guest wifi or host wifi, wired) | [Connection](#connection) |
 | macaddr | client mac address | str |
 | macaddress | client mac address | macaddress |
 | ipaddr | client ip address | str |
 | ipaddress | client ip address | ipaddress |
 | hostname | client hostname | str |
 | packets_sent | total packets sent | int, None |
 | packets_received | total packets received | int, None |
@@ -203,32 +182,34 @@
 | lan_ipv4_ipaddress | router LAN IP address | ipaddress |
 | lan_ipv4_dhcp_enable | router LAN DHCP enabled | bool |
 | lan_ipv4_netmask | router LAN gateway IP netmask | str |
 | lan_ipv4_netmask_address | router LAN gateway IP netmask | ipaddress |
 | remote | router remote | bool, None |
 
 ## Enum
-### <a id="wifi">Wifi</a>
-- Wifi.WIFI_2G - main wifi 2.4G
-- Wifi.WIFI_5G - main wifi 5G
-- Wifi.WIFI_6G - main wifi 5G
-- Wifi.WIFI_GUEST_2G - guest wifi 2.4G
-- Wifi.WIFI_GUEST_5G - guest wifi 5G
-- Wifi.WIFI_GUEST_6G - guest wifi 5G
-- Wifi.WIFI_IOT_2G - IoT wifi 2.4G
-- Wifi.WIFI_IOT_5G - IoT wifi 5G
-- Wifi.WIFI_IOT_6G - IoT wifi 6G
+### <a id="connection">Connection</a>
+- Connection.HOST_2G - host wifi 2.4G
+- Connection.HOST_5G - host wifi 5G
+- Connection.HOST_6G - host wifi 5G
+- Connection.GUEST_2G - guest wifi 2.4G
+- Connection.GUEST_5G - guest wifi 5G
+- Connection.GUEST_6G - guest wifi 5G
+- Connection.IOT_2G - IoT wifi 2.4G
+- Connection.IOT_5G - IoT wifi 5G
+- Connection.IOT_6G - IoT wifi 6G
+- Connection.WIRED - Wired
 
 ## <a id="supports">Supported routers</a>
 ### Fully tested Hardware Versions
 - Archer A7 V5
 - Archer AX10 v1.0
 - Archer AX12 v1.0
 - Archer AX20 v1.0
 - Archer AX21 v1.20
+- Archer AX23 v1.0
 - Archer AX50 v1.0
 - Archer AX55 v1.0
 - Archer AX55 V1.60
 - Archer AX72 V1
 - Archer AX73 V1
 - Archer AX75 V1
 - Archer AXE75 V1
```

