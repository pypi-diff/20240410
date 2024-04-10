# Comparing `tmp/python_swidget-0.0.9.tar.gz` & `tmp/python_swidget-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_swidget-0.0.9.tar", max compression
+gzip compressed data, was "python_swidget-1.0.0.tar", max compression
```

## Comparing `python_swidget-0.0.9.tar` & `python_swidget-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0       59 2023-01-11 19:11:12.359430 python_swidget-0.0.9/README.md
--rw-r--r--   0        0        0     2112 2023-01-11 22:03:19.879384 python_swidget-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1264 2023-01-11 19:11:12.359430 python_swidget-0.0.9/swidget/__init__.py
--rw-r--r--   0        0        0     6327 2023-01-11 19:11:12.359430 python_swidget-0.0.9/swidget/cli.py
--rw-r--r--   0        0        0     3483 2023-01-11 19:37:08.299444 python_swidget-0.0.9/swidget/discovery.py
--rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-0.0.9/swidget/exceptions.py
--rw-r--r--   0        0        0      595 2023-01-11 19:17:05.439433 python_swidget-0.0.9/swidget/provision.py
--rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-0.0.9/swidget/py.typed
--rw-r--r--   0        0        0    12739 2023-01-11 22:02:31.839384 python_swidget-0.0.9/swidget/swidgetdevice.py
--rw-r--r--   0        0        0     1525 2023-01-11 19:46:28.219448 python_swidget-0.0.9/swidget/swidgetdimmer.py
--rw-r--r--   0        0        0      384 2023-01-11 19:46:48.669448 python_swidget-0.0.9/swidget/swidgetoutlet.py
--rw-r--r--   0        0        0      574 2023-01-11 19:46:59.259448 python_swidget-0.0.9/swidget/swidgetswitch.py
--rw-r--r--   0        0        0      649 2023-01-11 19:47:08.599449 python_swidget-0.0.9/swidget/swidgettimerswitch.py
--rw-r--r--   0        0        0     4521 2023-01-11 20:18:00.769464 python_swidget-0.0.9/swidget/websocket.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 python_swidget-0.0.9/setup.py
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 python_swidget-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      539 2024-04-09 14:23:01.746129 python_swidget-1.0.0/README.md
+-rw-r--r--   0        0        0     2112 2024-04-09 14:23:01.746129 python_swidget-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1330 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/__init__.py
+-rw-r--r--   0        0        0     9045 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/cli.py
+-rw-r--r--   0        0        0     3899 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/discovery.py
+-rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-1.0.0/swidget/exceptions.py
+-rw-r--r--   0        0        0     4591 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/provision.py
+-rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-1.0.0/swidget/py.typed
+-rw-r--r--   0        0        0    18663 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/swidgetdevice.py
+-rw-r--r--   0        0        0     1680 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/swidgetdimmer.py
+-rw-r--r--   0        0        0      402 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/swidgetoutlet.py
+-rw-r--r--   0        0        0      592 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/swidgetswitch.py
+-rw-r--r--   0        0        0      789 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/swidgettimerswitch.py
+-rw-r--r--   0        0        0     3163 2024-04-09 14:23:01.746129 python_swidget-1.0.0/swidget/websocket.py
+-rw-r--r--   0        0        0     1741 1970-01-01 00:00:00.000000 python_swidget-1.0.0/PKG-INFO
```

### Comparing `python_swidget-0.0.9/pyproject.toml` & `python_swidget-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-swidget"
-version = "0.0.9"
+version = "1.0.0"
 description = "Python API for Swidget smart devices"
 license = "GPL-3.0-or-later"
 authors = ["Swidget"]
 repository = "https://github.com/swidget/python-swidget"
 readme = "README.md"
 packages = [
   { include = "swidget" }
```

### Comparing `python_swidget-0.0.9/swidget/__init__.py` & `python_swidget-1.0.0/swidget/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 Module-specific errors are raised as `SwidgetException` and are expected
 to be handled by the user of the library.
 """
 from importlib_metadata import version  # type: ignore
 
 from swidget.discovery import discover_devices, discover_single, SwidgetDiscoveredDevice
 from swidget.exceptions import SwidgetException
+from swidget.provision import provision_wifi
 from swidget.swidgetdevice import DeviceType, SwidgetAssembly, SwidgetDevice, SwidgetComponent
 from swidget.swidgetdimmer import SwidgetDimmer
 from swidget.swidgetoutlet import SwidgetOutlet
 from swidget.swidgetswitch import SwidgetSwitch
 from swidget.swidgettimerswitch import SwidgetTimerSwitch
 
 
 __version__ = version("python-swidget")
 
 
 __all__ = [
     "discover_devices",
     "discover_single",
+    "provision_wifi"
     "SwidgetDiscoveredDevice",
     "SwidgetException",
     "DeviceType",
     "SwidgetAssembly",
     "SwidgetDevice",
     "SwidgetComponent",
     "SwidgetDimmer",
```

### Comparing `python_swidget-0.0.9/swidget/cli.py` & `python_swidget-1.0.0/swidget/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """python-swidget cli tool."""
-import asyncio
 import logging
 import sys
 from pprint import pformat as pf
 from typing import cast
 
 import asyncclick as click
+from contextlib import asynccontextmanager
 
 from swidget import (
     discover_devices,
     discover_single,
+    provision_wifi,
     SwidgetDevice,
     SwidgetDimmer,
     SwidgetSwitch,
     SwidgetOutlet,
     SwidgetTimerSwitch
 )
 
@@ -27,91 +28,106 @@
 click.anyio_backend = "asyncio"
 
 
 pass_dev = click.make_pass_decorator(SwidgetDevice)
 
 
 @click.group(invoke_without_command=True)
-@click.option(
-    "--host",
+@click.option("--host",
     envvar="SWIDGET_HOST",
     required=False,
     help="The host name or IP address of the device to connect to.",
 )
-@click.option(
-    "--password",
+@click.option("-p", "--password",
     envvar="SWIDGET_PASSWORD",
     required=False,
     help="The password of the device to connect to.",
 )
 @click.option("-d", "--debug",
     envvar="SWIDGET_DEBUG",
     default=False,
     is_flag=True)
+@click.option("--http_only",
+    envvar="SWIDGET_HTTP_ONLY",
+    default=True,
+    is_flag=True)
 @click.option(
     "--type",
     envvar="SWIDGET_TYPE",
     default=None,
     type=click.Choice(list(TYPE_TO_CLASS), case_sensitive=False),
 )
 @click.version_option(package_name="python-swidget")
 @click.pass_context
-async def cli(ctx, host, password, debug, type):
+async def cli(ctx, host, password, debug, http_only, type):
     """A tool for controlling Swidget smart home devices."""  # noqa
     # no need to perform any checks if we are just displaying the help
     if sys.argv[-1] == "--help":
-        # Context object is required to avoid crashing on sub-groups
-        ctx.obj = SwidgetDevice(None)
         return
 
     if debug:
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.INFO)
 
-    if ctx.invoked_subcommand == "discover":
+    if ctx.invoked_subcommand == "discover" or ctx.invoked_subcommand == "wifi":
         return
-
     if host is None:
         click.echo("No host name given, trying discovery..")
         await ctx.invoke(discover)
         return
-
     if type is not None:
-        dev = TYPE_TO_CLASS[type](host, password, False, False)
+        dev = TYPE_TO_CLASS[type](host=host,
+                                  token_name='x-secret-key',
+                                  secret_key=password,
+                                  use_https=http_only,
+                                  use_websockets=False)
     else:
-        click.echo("No --type defined, discovering..")
-        dev = await discover_single(host, password, False, False)
+        click.echo("No --type defined, discovering...")
+        dev = await discover_single(host=host,
+                                    token_name='x-secret-key',
+                                    password=password,
+                                    use_https=http_only,
+                                    use_websockets=False)
+        await dev.update()
+
+    @asynccontextmanager
+    async def async_wrapped_device(dev: SwidgetDevice):
+        try:
+            yield dev
+        finally:
+            await dev.stop()
 
-    await dev.update()
-    ctx.obj = dev
+    ctx.obj = await ctx.with_async_resource(async_wrapped_device(dev))
 
     if ctx.invoked_subcommand is None:
-        await ctx.invoke(state)
+        return await ctx.invoke(state)
 
 
 @cli.group()
-@pass_dev
-def wifi(dev):
+def wifi():
     """Commands to control wifi settings."""
 
+
 @wifi.command()
-@click.argument("ssid")
-@click.option("--password", prompt=True, hide_input=True)
-@click.option("--keytype", default=3)
-@pass_dev
-async def join(dev: SwidgetDevice, ssid, password, keytype):
+@click.option("--ssid", prompt=True, hide_input=False)
+@click.option("--network_password", prompt=True, hide_input=True)
+@click.option("--secret_key", prompt=True, hide_input=True)
+@click.option("--friendly_name", prompt=True, hide_input=False)
+def join(ssid, network_password, secret_key, friendly_name):
     """Join the given wifi network."""
-    click.echo(f"Asking the device to connect to {ssid}..")
-    res = await dev.wifi_join(ssid, password, keytype=keytype)
-    click.echo(
-        f"Response: {res} - if the device is not able to join the network, it will revert back to its previous state."
-    )
-
-    return res
+    confirmation = click.prompt(f"Are you connected to a wifi network that stars with the name 'Swidget-' (y/n)")
+    if confirmation == "y":
+        click.echo(f"Asking the device to connect to network {ssid}..")
+        # def provision_wifi(ssid, network_password, token_name, secret_key, friendly_name):
+        provision_wifi(friendly_name, ssid, network_password, secret_key)
+        return True
+    else:
+        click.echo("Not provisioning wifi")
+        return False
 
 
 @cli.command()
 @click.option("--timeout", default=5, required=False)
 @click.pass_context
 async def discover(ctx, timeout):
     """Discover devices in the network."""
@@ -131,29 +147,31 @@
 
 
 @cli.command()
 @pass_dev
 async def state(dev: SwidgetDevice):
     """Print out device state and versions."""
     click.echo(click.style(f"== {dev.friendly_name} - {dev.model} ==", bold=True))
+    click.echo(f"\tFriendly Name:  {dev.friendly_name}")
     click.echo(f"\tHost: {dev.ip_address}")
     click.echo(
         click.style(
             "\tDevice state: {}\n".format("ON" if dev.is_on else "OFF"),
             fg="green" if dev.is_on else "red",
         )
     )
 
     click.echo(click.style("\t== Generic information ==", bold=True))
     click.echo(f"\tHardware:     {dev.hw_info['model']}")
     click.echo(f"\tSoftware:     {dev.hw_info['version']}")
     click.echo(f"\tMAC (rssi):   {dev.mac_address} ({dev.rssi})")
 
     click.echo(click.style("\n\t== Current State ==", bold=True))
-    for info_name, info_data in dev.realtime_values.items():
+    realtime_values = await dev.realtime_values
+    for info_name, info_data in realtime_values.items():
         if isinstance(info_data, list):
             click.echo(f"\t{info_name}:")
             for item in info_data:
                 click.echo(f"\t\t{item}")
         else:
             click.echo(f"\t{info_name}: {info_data}")
 
@@ -163,15 +181,14 @@
 
 
     click.echo(click.style("\n\t== Insert Features ==", bold=True))
     for function in dev.insert_features:
         click.echo(click.style(f"\t+ {function}", fg="green"))
 
 
-
 @cli.command()
 @pass_dev
 @click.argument("assembly")
 @click.argument("component")
 @click.argument("function")
 @click.argument("command")
 async def raw_command(dev: SwidgetDevice, assembly, component, function, command):
@@ -183,15 +200,14 @@
 
     res = await dev.send_command(assembly, component, function, command)
 
     click.echo(res)
     return res
 
 
-
 @cli.command()
 @click.argument("brightness", type=click.IntRange(0, 100), default=None, required=False)
 @pass_dev
 async def brightness(dev: SwidgetDimmer, brightness: int):
     """Get or set brightness."""
     if not dev.is_dimmer:
         click.echo("This device does not support brightness.")
@@ -210,23 +226,74 @@
     """Set the device insert to blink"""
     click.echo(f"Requesting the device to blink")
     return await dev.blink()
 
 
 @cli.command()
 @pass_dev
+async def ping(dev):
+    """Ping the device"""
+    click.echo(f"Pinging the device")
+    try:
+        result = await dev.ping()
+        if result == 200:
+            click.echo("Successfully pinged device")
+        else:
+            click.echo(result.status_code)
+    except:
+        click.echo("Unable to ping device")
+
+@cli.command()
+@pass_dev
 async def on(dev: SwidgetDevice):
     """Turn the device on."""
     click.echo(f"Turning on {dev.friendly_name}")
     return await dev.turn_on()
 
 
 @cli.command()
 @pass_dev
 async def off(dev: SwidgetDevice):
     """Turn the device off."""
     click.echo(f"Turning off {dev.friendly_name}")
     return await dev.turn_off()
 
 
+@cli.command()
+@pass_dev
+async def enable_debug_server(dev: SwidgetDevice):
+    """Enable Debug Server"""
+    click.echo(f"Enabling debug server")
+    return await dev.enable_debug_server()
+
+
+@cli.command()
+@pass_dev
+async def check_for_updates(dev: SwidgetDevice):
+    click.echo("Contacting Swidget servers to fetch for updates...")
+    available_updates = await dev.check_for_updates()
+    if len(available_updates['updates']) == 0:
+        click.echo("No available updates")
+    else:
+        click.echo("The following versions are available to update to")
+        for version in available_updates['updates']:
+            click.echo(click.style(f"\t+ {version}", fg="green"))
+
+
+@cli.command()
+@click.option("--version", required=False)
+@pass_dev
+async def upgrade(dev: SwidgetDevice, version: str):
+    if version is None:
+        click.echo("Contacting Swidget servers to fetch for latest version")
+        available_updates = await dev.check_for_updates()
+        if len(available_updates['updates']) == 0:
+            click.echo("No available updates")
+        else:
+            version = available_updates[-1]
+    click.echo(f"Upgrading to version: {version}")
+    response = await dev.update_version(version)
+    click.echo(response)
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `python_swidget-0.0.9/swidget/discovery.py` & `python_swidget-1.0.0/swidget/discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,20 +33,26 @@
         "Handle an incoming response."
         headers = {h[0]: h[1] for h in response.headers}
         mac_address = headers["USN"].split("-")[-1]
         ip_address = urlparse(headers["LOCATION"]).hostname
         if headers["ST"] == SWIDGET_ST:
             device_type = headers["SERVER"].split(" ")[1].split("+")[0]
             insert_type = headers["SERVER"].split(" ")[1].split("+")[1].split("/")[0]
-            friendly_name = f"Swidget {device_type} w/{insert_type} insert"
+            friendly_name = headers["SERVER"].split("/")[2].strip('"')
             devices[mac_address] = SwidgetDiscoveredDevice(mac_address, ip_address, friendly_name)
+<<<<<<< HEAD
+=======
+            _LOGGER.debug(f"Swidget device '{friendly_name}' at {ip_address}")
+>>>>>>> 690a0c560a8b2ff39245d1a8354ced968d79e5de
 
 
 async def discover_devices(timeout=RESPONSE_SEC):
+    global devices
     loop = asyncio.get_event_loop()
+    devices = dict()
     transport, protocol = await loop.create_datagram_endpoint(
         SwidgetProtocol, family=socket.AF_INET
     )
 
     # Send out an M-SEARCH request, requesting Swidget service types.
     search_request = ssdp.SSDPRequest(
         "M-SEARCH",
@@ -55,31 +61,37 @@
             "MAN": '"ssdp:discover"',
             "MX": timeout,
             "ST": SWIDGET_ST,
         },
     )
     search_request.sendto(transport, (SwidgetProtocol.MULTICAST_ADDRESS, 1900))
     await asyncio.sleep(timeout)
-    _LOGGER.debug(f"Found the following Swidget devices from SSDP discovery: {devices}")
     return devices
 
 
-async def discover_single(host: str, token_name: str, password: str, ssl: bool, use_websockets: bool) -> SwidgetDevice:
+async def discover_single(host: str, token_name: str, password: str, use_https: bool, use_websockets: bool) -> SwidgetDevice:
     """Discover a single device by the given IP address.
 
     :param host: Hostname of device to query
     :rtype: SwidgetDevice
     :return: Object for querying/controlling found device.
     """
-    swidget_device = SwidgetDevice(host, token_name, password, ssl, use_websockets)
+    _LOGGER.debug(f"Checking for device at {host}")
+    swidget_device = SwidgetDevice(host, token_name, password, use_https, use_websockets=False)
+    _LOGGER.debug(f"Asking {host} for summary data")
     await swidget_device.get_summary()
     device_type = swidget_device.device_type
+    _LOGGER.debug(f"{host} is of type {device_type}")
+    await swidget_device.stop()
+
+    _LOGGER.debug(f"Creating new device class of type: {device_type}")
     device_class = _get_device_class(device_type)
-    dev = device_class(host, token_name, password, False, use_websockets)
-    await dev.update()
+    _LOGGER.debug(f"{device_class}")
+    dev = device_class(host, token_name, password, use_https, use_websockets)
+    await dev.start()
     return dev
 
 
 def _get_device_class(device_type: str) -> Type[SwidgetDevice]:
     """Find SmartDevice subclass for device described by passed data."""
     if device_type == "outlet":
         return SwidgetOutlet
```

### Comparing `python_swidget-0.0.9/swidget/swidgetdevice.py` & `python_swidget-1.0.0/swidget/swidgetdevice.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,309 @@
 import json
 import logging
 import time
 
 from aiohttp import ClientSession, TCPConnector
+import asyncio
 from enum import Enum
 from typing import Dict, List, Set
 
 from .exceptions import SwidgetException
 from .websocket import SwidgetWebsocket
 
 _LOGGER = logging.getLogger(__name__)
 
-
 class DeviceType(Enum):
     """Device type enum."""
 
     Dimmer = "dimmer"
     Outlet = "outlet"
     Switch = "switch"
     TimerSwitch = "pana_switch"
     RelaySwitch = "relay_switch"
     Unknown = -1
 
 
 class SwidgetDevice:
-    def __init__(self, host, token_name, secret_key, ssl=False, use_websockets=True):
+    def __init__(self, host, token_name, secret_key, use_https=True, use_websockets=True):
         self.token_name = token_name
         self.ip_address = host
-        self.ssl = ssl
+
+        self.use_https = use_https
+        self.uri_scheme = 'https' if self.use_https is True else 'http'
         self.secret_key = secret_key
         self.use_websockets = use_websockets
         self.device_type = DeviceType.Unknown
-        headers = {self.token_name: self.secret_key}
-        connector = TCPConnector(force_close=True)
+        self._friendly_name = "Unknown Swidget Device"
+        headers = {self.token_name: self.secret_key,
+                   'Connection': 'keep-alive'}
+        connector = TCPConnector(verify_ssl=False, force_close=True)
         self._session = ClientSession(headers=headers, connector=connector)
         self._last_update = None
         if self.use_websockets:
             self._websocket = SwidgetWebsocket(
                 host=self.ip_address,
                 token_name=self.token_name,
                 secret_key=self.secret_key,
                 callback=self.message_callback,
                 session=self._session)
 
+    def get_websocket(self):
+        if self.use_websockets:
+            return self._websocket
+        return None
+
     def set_countdown_timer(self, minutes):
         raise NotImplementedError()
 
-    def stop(self):
+    async def connect(self):
+        await self._websocket.connect()
+
+    async def start(self):
+        """Start the websocket."""
+        _LOGGER.debug("SwidgetDevice.start()")
+        if self.use_websockets:
+            _LOGGER.debug("Calling self._websocket.connect()")
+            await self._websocket.connect()
+            _LOGGER.debug("Calling self._websocket.listen() ")
+            asyncio.create_task(self._websocket.listen())
+
+    async def stop(self):
         """Stop the websocket."""
-        if self._websocket is not None:
-            self._websocket.stop()
+        _LOGGER.debug("SwidgetDevice.stop()")
+        if hasattr(self, '_websocket'):
+            await self._websocket.close()
+        await self._session.close()
 
     async def message_callback(self, message):
         """Entrypoint for a websocket callback"""
+        _LOGGER.debug("SwidgetDevice.message_callback() called")
         if message["request_id"] == "summary":
+            _LOGGER.debug("Calling SwidgetDevice.process_summary()")
             await self.process_summary(message)
         elif message["request_id"] == "state" or message["request_id"] == "DYNAMIC_UPDATE" or message["request_id"] == "command":
+            _LOGGER.debug("Calling SwidgetDevice.process_state()")
             await self.process_state(message)
+        else:
+            _LOGGER.error(f"Unknown message type from websocket. Type given was: {message["request_id"]}")
 
     async def get_summary(self):
         """Get a summary of the device over HTTP"""
-        async with self._session.get(
-            url=f"https://{self.ip_address}/api/v1/summary", ssl=self.ssl
-        ) as response:
-            summary = await response.json()
-        await self.process_summary(summary)
+        _LOGGER.debug("SwidgetDevice.get_summary() called")
+        if self.use_websockets:
+            _LOGGER.debug("In websocket mode. Sending get_summary() command over websocket")
+            await self._websocket.send_str(json.dumps({"type": "summary", "request_id": "summary"}))
+        else:
+            _LOGGER.debug("In http mode. Sending get_summary() command over http")
+            async with self._session.get(
+                url=f"{self.uri_scheme}://{self.ip_address}/api/v1/summary", ssl=False
+            ) as response:
+                summary = await response.json()
+            await self.process_summary(summary)
 
     async def process_summary(self, summary):
         """ Process the data around the summary of the device"""
+        _LOGGER.debug("SwidgetDevice.process_summary() called")
+        _LOGGER.debug(f"Summary to process: {summary}")
         self.model = summary["model"]
         self.mac_address = summary["mac"]
         self.version = summary["version"]
         self.assemblies = {
             "host": SwidgetAssembly(summary["host"]),
             "insert": SwidgetAssembly(summary["insert"]),
         }
         self.device_type = self.assemblies['host'].type
         self.insert_type = self.assemblies['insert'].type
         self.id = self.assemblies['host'].id
         self._last_update = int(time.time())
 
+    async def get_friendly_name(self):
+        _LOGGER.debug("SwidgetDevice.get_friendly_name() called")
+        try:
+            async with self._session.get(
+                url=f"{self.uri_scheme}://{self.ip_address}/api/v1/name", ssl=False
+            ) as response:
+                name = await response.json()
+        except Exception:
+            name = {"name": f"Swidget {self.device_type} w/{self.insert_type} insert"}
+        await self.process_friendly_name(name['name'])
+
+    async def process_friendly_name(self, name):
+        _LOGGER.debug("SwidgetDevice.process_friendly_name() called")
+        self._friendly_name = name
+        self._last_update = int(time.time())
+
     async def get_state(self):
         """ Get the state of the device over HTTP"""
-        async with self._session.get(
-            url=f"https://{self.ip_address}/api/v1/state", ssl=self.ssl
-        ) as response:
-            state = await response.json()
-        await self.process_state(state)
+        _LOGGER.debug("SwidgetDevice.get_state() called")
+        if self.use_websockets:
+            _LOGGER.debug("In websocket mode. Sending get_summary() command over websocket")
+            await self._websocket.send_str(json.dumps({"type": "state", "request_id": "state"}))
+        else:
+            _LOGGER.debug("In http mode. Sending get_summary() command over http")
+            async with self._session.get(
+                url=f"{self.uri_scheme}://{self.ip_address}/api/v1/state", ssl=False
+            ) as response:
+                state = await response.json()
+            await self.process_state(state)
 
     async def process_state(self, state):
         """ Process any information about the state of the device or insert"""
-        _LOGGER.debug(f"Processing state: {state}")
         # State is not always in the state (during callback)
+        _LOGGER.debug("SwidgetDevice.process_state() called")
+        _LOGGER.debug(f"State to process: {state}")
         try:
             self.rssi = state["connection"]["rssi"]
         except:
             pass
-
         for assembly in self.assemblies:
             for id, component in self.assemblies[assembly].components.items():
                 try:
                     component.functions.update(state[assembly]["components"][id])
                 except:
                     pass
         self._last_update = int(time.time())
 
     async def update(self):
+        _LOGGER.debug("SwidgetDevice.update() called")
         if self._last_update is None:
             _LOGGER.debug("Performing the initial update to obtain sysinfo")
-        await self.get_summary()
-        await self.get_state()
+            await self.get_summary()
+            await self.get_state()
+            if self._friendly_name == "Unknown Swidget Device":
+                await self.get_friendly_name()
+        elif (int(time.time()) - self._last_update) < 5:
+            _LOGGER.debug("update() recently called, not executing")
+        else:
+            _LOGGER.debug("Requesting an update of the device")
+            await self.get_summary()
+            await self.get_state()
 
     async def send_config(self, payload: dict):
-        data = json.dumps({"type":"config","request_id":"abcd", "payload": payload})
+        _LOGGER.debug("SwidgetDevice.send_config() called")
+        data = json.dumps({"type":"config","request_id":"send_config", "payload": payload})
         await self._websocket.send_str(data)
 
     async def send_command(
         self, assembly: str, component: str, function: str, command: dict
     ):
+        _LOGGER.debug("SwidgetDevice.send_command() called")
         """Send a command to the Swidget device either using a HTTP call or the existing websocket"""
         data = {assembly: {"components": {component: {function: command}}}}
-
+        _LOGGER.debug(f"Command to send: {data}")
         if self.use_websockets:
+            _LOGGER.debug("In websocket mode. Sending command over websocket")
             data = json.dumps({"type": "command",
                                "request_id": "command",
                                "payload": data
                                })
-            _LOGGER.debug(f"About to send data: {data}")
             await self._websocket.send_str(data)
         else:
+            _LOGGER.debug("NOT in websocket mode, sending command over HTTP")
             async with self._session.post(
-                url=f"https://{self.ip_address}/api/v1/command",
-                ssl=self.ssl,
+                url=f"{self.uri_scheme}://{self.ip_address}/api/v1/command",
+                ssl=False,
                 data=json.dumps(data),
             ) as response:
                 state = await response.json()
 
+            # Do a hard set of the new state of the device. May change this in the future
             function_value = state[assembly]["components"][component][function]
             self.assemblies[assembly].components[component].functions[function] = function_value  # fmt: skip
 
     async def ping(self):
         """Ping the device to ensure it's devices
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
+        _LOGGER.debug("SwidgetDevice.ping() called")
         try:
             async with self._session.get(
-                url=f"https://{self.ip_address}/ping",
-                ssl=self.ssl
+                url=f"{self.uri_scheme}://{self.ip_address}/ping",
+                ssl=False
             ) as response:
-                return response.text
+                return response.status
         except:
             raise SwidgetException
 
     async def blink(self):
         """Make the device LED blink
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
+        _LOGGER.debug("SwidgetDevice.blink() called")
+        try:
+            async with self._session.get(
+                url=f"{self.uri_scheme}://{self.ip_address}/blink",
+                ssl=False
+            ) as response:
+                return await response.json()
+        except:
+            raise SwidgetException
+
+    async def enable_debug_server(self):
+        """Enable the Swidget local debug server
+
+        :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
+        """
+        _LOGGER.debug("SwidgetDevice.enable_debug_server() called")
         try:
             async with self._session.get(
-                url=f"https://{self.ip_address}/blink?x-user-key=dqMMBX9deuwtkkp784ewTjqo76IYfThV",
-                ssl=self.ssl
+                url=f"{self.uri_scheme}://{self.ip_address}/debug?x-secret-key={self.secret_key}",
+                ssl=False
             ) as response:
-                return response.text
+                return await response.json()
+        except:
+            raise SwidgetException
+
+    async def factory_reset(self):
+        """Factory reset the Swidget device
+
+        :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
+        """
+        try:
+
+            async with self._session.delete(
+                url=f"{self.uri_scheme}://{self.ip_address}/api/v1/reset",
+                ssl=False
+            ) as response:
+                return await response.json()
+        except:
+            raise SwidgetException
+
+    async def check_for_updates(self):
+        """Tell the device to contact the Swidget servers to see if there is an available update
+
+        :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
+        """
+        try:
+
+            async with self._session.get(
+                url=f"{self.uri_scheme}://{self.ip_address}/api/v1/update",
+                ssl=False
+            ) as response:
+                return await response.json()
+        except:
+            raise SwidgetException
+
+    async def update_version(self, version):
+        """Tell the device to download and apply an update
+
+        :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
+        """
+        try:
+            data = {
+                "version": version
+            }
+            async with self._session.post(
+                url=f"{self.uri_scheme}://{self.ip_address}/api/v1/update",
+                ssl=False,
+                data=json.dumps(data)
+            ) as response:
+                return await response
         except:
             raise SwidgetException
 
     @property
     def hw_info(self) -> Dict:
         """
         Return hardware information.
@@ -182,15 +318,15 @@
             "model": self.model,
             "insert_type": self.insert_type,
             "insert_features": self.insert_features,
             "host_features": self.host_features,
             "rssi": self.rssi
         }
 
-    def get_child_consumption(self, plug_id=0):
+    async def get_child_consumption(self, plug_id=0):
         """Get the power consumption of a plug in watts."""
         if plug_id == "all":
             return_dict = {}
             for id, properties in self.assemblies['host'].components.items():
                 try:
                     return_dict[f"power_{id}"] = properties.functions['power']['current']
                 except KeyError: # Hits this when there is no power metering
@@ -202,45 +338,43 @@
         """Get the total power consumption in watts."""
         total_consumption = 0
         for id, properties in self.assemblies['host'].components.items():
             total_consumption += properties.functions['power']['current']
         return total_consumption
 
     @property
-    def realtime_values(self):
+    async def realtime_values(self):
         """Get a dict of realtime value attributes from the insert and host
 
         :return: A dictionary of insert sensor values and power consumption values
         :rtype: dict
         """
         return_dict = {}
         for feature in self.insert_features:
             return_dict.update(self.get_function_values(feature))
         return_dict.update({'rssi': self.rssi})
-        power_values = self.get_child_consumption("all")
+        power_values = await self.get_child_consumption("all")
         if power_values:
             return_dict.update(power_values)
         return return_dict
 
     @property
     def host_features(self) -> List[str]:
         """Return a set of features that the host supports."""
         try:
             return list(self.assemblies['host'].components['0'].functions.keys())
         except KeyError:
-            _LOGGER.debug("Host does not have feature information")
             return set()
 
     @property
     def insert_features(self) -> List[str]:
         """Return a set of features that the insert supports."""
         try:
             return list(self.assemblies['insert'].components.keys())
         except KeyError:
-            _LOGGER.debug("Insert does not have feature information")
             return set()
 
     def get_function_values(self, function: str):
         """Return the values of an insert function."""
         return_values = dict()
         for function, data in self.assemblies['insert'].components[function].functions.items():
             if function == "occupied":
@@ -277,36 +411,39 @@
     def is_dimmer(self) -> bool:
         """Return True if the device is a dimmer"""
         return self.device_type == "dimmer"
 
     @property
     def is_dimmable(self) -> bool:
         """Return  True if the device is dimmable."""
-        return False
+        return self.is_dimmer
 
-    @property
+    @property  # type: ignore
     def friendly_name(self) -> str:
         """Return a friendly description of the device"""
-        return f"Swidget {self.device_type} w/{self.insert_type} insert"
+        return self._friendly_name
 
     @property  # type: ignore
     def is_on(self) -> bool:
         """Return whether device is on."""
         dimmer_state = self.assemblies['host'].components["0"].functions['toggle']["state"]
         if dimmer_state == "on":
             return True
         return False
 
     async def turn_on(self):
         """Turn the device on."""
+        _LOGGER.debug("SwidgetDevice.turn_on() called")
         await self.send_command(
             assembly="host", component="0", function="toggle", command={"state": "on"}
         )
+
     async def turn_off(self):
         """Turn the device off."""
+        _LOGGER.debug("SwidgetDevice.turn_off() called")
         await self.send_command(
             assembly="host", component="0", function="toggle", command={"state": "off"}
         )
 
     async def turn_on_usb_insert(self):
         """Turn the USB insert on."""
         await self.send_command(
@@ -328,25 +465,21 @@
         return False
 
     def __repr__(self):
         if self._last_update is None:
             return f"<{self.device_type} at {self.ip_address} - update() needed>"
         return f"<{self.device_type} model {self.model} at {self.ip_address}>"
 
-    def __del__(self):
-        if self.use_websockets:
-            self.stop()
-
 
 class SwidgetAssembly:
     def __init__(self, summary: dict):
         self.type = summary["type"]
         self.components = {
             c["id"]: SwidgetComponent(c["functions"]) for c in summary["components"]
         }
         self.id = summary.get("id")
         self.error = summary.get("error")
 
 
 class SwidgetComponent:
     def __init__(self, functions):
-        self.functions = {f: None for f in functions}
+        self.functions = {f: None for f in functions}
```

### Comparing `python_swidget-0.0.9/swidget/swidgetdimmer.py` & `python_swidget-1.0.0/swidget/swidgetdimmer.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 from swidget.swidgetdevice import (
     DeviceType,
     SwidgetDevice
 )
 from swidget.exceptions import SwidgetException
 
+_LOGGER = logging.getLogger(__name__)
 
 
-log = logging.getLogger(__name__)
-
 class SwidgetDimmer(SwidgetDevice):
 
-    def __init__(self, host,  token_name: str, secret_key: str, ssl: bool, use_websockets: bool) -> None:
-        super().__init__(host=host, token_name=token_name, secret_key=secret_key, ssl=ssl, use_websockets=use_websockets)
+    def __init__(self, host,  token_name: str, secret_key: str, use_https: bool, use_websockets: bool) -> None:
+        super().__init__(host=host, token_name=token_name, secret_key=secret_key, use_https=use_https, use_websockets=use_websockets)
         self._device_type = "dimmer"
 
     @property  # type: ignore
     def brightness(self) -> int:
         """Return current brightness on dimmers.
 
         Will return a range between 0 - 100.
@@ -27,19 +26,21 @@
         try:
             return self.assemblies['host'].components["0"].functions["level"]["now"]
         except KeyError:
             return self.assemblies['host'].components["0"].functions["level"]["default"]
 
     async def set_brightness(self, brightness):
         """Set the brightness of the device."""
+        _LOGGER.debug("SwidgetDimmer.set_brightness() called")
         await self.send_command(
             assembly="host", component="0", function="level", command={"now": brightness}
         )
 
     async def set_default_brightness(self, brightness):
+        _LOGGER.debug("SwidgetDimmer.set_default_brightness() called")
         await self.send_command(
             assembly="host", component="0", function="level", command={"default": brightness}
         )
 
     @property  # type: ignore
     def is_dimmable(self) -> bool:
         """Whether the switch supports brightness changes."""
```

### Comparing `python_swidget-0.0.9/swidget/swidgetswitch.py` & `python_swidget-1.0.0/swidget/swidgetswitch.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,14 @@
     DeviceType,
     SwidgetDevice
 )
 
 
 class SwidgetSwitch(SwidgetDevice):
 
-    def __init__(self, host,  token_name: str, secret_key: str, ssl: bool, use_websockets: bool) -> None:
-        super().__init__(host=host, token_name=token_name, secret_key=secret_key, ssl=ssl, use_websockets=use_websockets)
+    def __init__(self, host,  token_name: str, secret_key: str, use_https: bool, use_websockets: bool) -> None:
+        super().__init__(host=host, token_name=token_name, secret_key=secret_key, use_https=use_https, use_websockets=use_websockets)
         self._device_type = DeviceType.Switch
 
     async def current_consumption(self) -> float:
         """Get the current power consumption in watts."""
         return sum([await plug.current_consumption() for plug in self.children])
```

### Comparing `python_swidget-0.0.9/swidget/swidgettimerswitch.py` & `python_swidget-1.0.0/swidget/swidgettimerswitch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import logging
 from swidget.swidgetdevice import (
     DeviceType,
 )
 from swidget.swidgetswitch import SwidgetSwitch
 
+_LOGGER = logging.getLogger(__name__)
+
 
 class SwidgetTimerSwitch(SwidgetSwitch):
 
-    def __init__(self, host,  token_name: str, secret_key: str, ssl: bool, use_websockets: bool) -> None:
-        super().__init__(host=host, token_name=token_name, secret_key=secret_key, ssl=ssl, use_websockets=use_websockets)
+    def __init__(self, host,  token_name: str, secret_key: str, use_https: bool, use_websockets: bool) -> None:
+        super().__init__(host=host, token_name=token_name, secret_key=secret_key, use_https=use_https, use_websockets=use_websockets)
         self._device_type = DeviceType.TimerSwitch
 
     async def set_countdown_timer(self, minutes):
         """Set the countdown timer."""
+        _LOGGER.debug("SwidgetTimerSwitch.set_brightness() called")
         await self.send_command(
             assembly="host", component="0", function="timer", command={"duration": minutes}
         )
```

