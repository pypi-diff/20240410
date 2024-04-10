# Comparing `tmp/losant-mqtt-1.2.0.tar.gz` & `tmp/losant-mqtt-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/losant-mqtt-1.2.0.tar", last modified: Tue May 14 03:15:13 2019, max compression
+gzip compressed data, was "losant-mqtt-1.2.1.tar", last modified: Wed Apr 10 18:54:38 2024, max compression
```

## Comparing `losant-mqtt-1.2.0.tar` & `losant-mqtt-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mkuehl     (501) staff       (20)        0 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/
--rw-r--r--   0 mkuehl     (501) staff       (20)     9672 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/PKG-INFO
-drwxr-xr-x   0 mkuehl     (501) staff       (20)        0 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/losant_mqtt.egg-info/
--rw-r--r--   0 mkuehl     (501) staff       (20)     9672 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/losant_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 mkuehl     (501) staff       (20)      279 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/losant_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 mkuehl     (501) staff       (20)       18 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/losant_mqtt.egg-info/requires.txt
--rw-r--r--   0 mkuehl     (501) staff       (20)       11 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/losant_mqtt.egg-info/top_level.txt
--rw-r--r--   0 mkuehl     (501) staff       (20)        1 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/losant_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 mkuehl     (501) staff       (20)     1082 2019-01-02 22:21:44.000000 losant-mqtt-1.2.0/LICENSE
--rw-r--r--   0 mkuehl     (501) staff       (20)       46 2016-06-01 16:16:54.000000 losant-mqtt-1.2.0/MANIFEST.in
--rw-r--r--   0 mkuehl     (501) staff       (20)     1351 2019-05-14 02:55:34.000000 losant-mqtt-1.2.0/setup.py
--rw-r--r--   0 mkuehl     (501) staff       (20)       38 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/setup.cfg
--rw-r--r--   0 mkuehl     (501) staff       (20)     6821 2019-01-02 22:21:01.000000 losant-mqtt-1.2.0/README.rst
-drwxr-xr-x   0 mkuehl     (501) staff       (20)        0 2019-05-14 03:15:13.000000 losant-mqtt-1.2.0/losantmqtt/
--rw-r--r--   0 mkuehl     (501) staff       (20)    10237 2019-01-02 22:21:27.000000 losant-mqtt-1.2.0/losantmqtt/device.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     1338 2019-05-14 02:55:23.000000 losant-mqtt-1.2.0/losantmqtt/RootCA.crt
--rw-r--r--   0 mkuehl     (501) staff       (20)     1119 2019-01-02 22:21:24.000000 losant-mqtt-1.2.0/losantmqtt/__init__.py
+drwxr-xr-x   0 michael@losant.com   (501) staff       (20)        0 2024-04-10 18:54:38.659512 losant-mqtt-1.2.1/
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)     1082 2024-04-10 18:01:46.000000 losant-mqtt-1.2.1/LICENSE
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)       46 2016-06-01 16:16:54.000000 losant-mqtt-1.2.1/MANIFEST.in
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)     7662 2024-04-10 18:54:38.658743 losant-mqtt-1.2.1/PKG-INFO
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)     6833 2024-04-10 18:01:46.000000 losant-mqtt-1.2.1/README.rst
+drwxr-xr-x   0 michael@losant.com   (501) staff       (20)        0 2024-04-10 18:54:38.657975 losant-mqtt-1.2.1/losant_mqtt.egg-info/
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)     7662 2024-04-10 18:54:38.000000 losant-mqtt-1.2.1/losant_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)      279 2024-04-10 18:54:38.000000 losant-mqtt-1.2.1/losant_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)        1 2024-04-10 18:54:38.000000 losant-mqtt-1.2.1/losant_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)       20 2024-04-10 18:54:38.000000 losant-mqtt-1.2.1/losant_mqtt.egg-info/requires.txt
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)       11 2024-04-10 18:54:38.000000 losant-mqtt-1.2.1/losant_mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 michael@losant.com   (501) staff       (20)        0 2024-04-10 18:54:38.656518 losant-mqtt-1.2.1/losantmqtt/
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)     2631 2024-04-10 18:01:46.000000 losant-mqtt-1.2.1/losantmqtt/RootCA.crt
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)     1119 2024-04-10 18:01:46.000000 losant-mqtt-1.2.1/losantmqtt/__init__.py
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)    10237 2024-04-10 18:01:46.000000 losant-mqtt-1.2.1/losantmqtt/device.py
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)       38 2024-04-10 18:54:38.659595 losant-mqtt-1.2.1/setup.cfg
+-rw-r--r--   0 michael@losant.com   (501) staff       (20)     1353 2024-04-10 18:01:46.000000 losant-mqtt-1.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `losant-mqtt-1.2.0/PKG-INFO` & `losant-mqtt-1.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,279 +1,280 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: losant-mqtt
-Version: 1.2.0
+Version: 1.2.1
 Summary: An MQTT client for Losant
 Home-page: https://github.com/Losant/losant-mqtt-python
 Author: Losant
 Author-email: hello@losant.com
 License: MIT
-Description: Losant Python MQTT Client
-        =========================
-        
-        |travis-badge|_ |pypi-badge|_
-        
-        .. |travis-badge| image:: https://travis-ci.org/Losant/losant-mqtt-python.svg?branch=master
-        .. _travis-badge: https://travis-ci.org/Losant/losant-mqtt-python
-        
-        .. |pypi-badge| image:: https://badge.fury.io/py/losant-mqtt.svg
-        .. _pypi-badge: https://badge.fury.io/py/losant-mqtt
-        
-        The `Losant <https://www.losant.com>`_ MQTT client provides a simple way for
-        custom things to communicate with the Losant platform over MQTT.  You can authenticate
-        as a device, publish device state, and listen for device commands.
-        
-        This client works with both Python 2.7 and 3. It uses the
-        `Paho MQTT Client <https://github.com/eclipse/paho.mqtt.python>`_ under the
-        covers for the actual MQTT communication.
-        
-        Installation
-        ------------
-        
-        The latest stable version is available in the Python Package Index (PyPi)
-        and can be installed using
-        
-        ::
-        
-            pip install losant-mqtt
-        
-        
-        Example
-        -------
-        
-        Below is a high-level example of using the Losant Python MQTT client to send the value
-        of a temperature sensor to the Losant platform.
-        
-        ::
-        
-            import time
-            from losantmqtt import Device
-        
-            # Construct device
-            device = Device("my-device-id", "my-app-access-key", "my-app-access-secret")
-        
-            def on_command(device, command):
-                print("Command received.")
-                print(command["name"])
-                print(command["payload"])
-        
-            # Listen for commands.
-            device.add_event_observer("command", on_command)
-        
-            # Connect to Losant.
-            device.connect(blocking=False)
-        
-            # Send temperature once every second.
-            while True:
-                device.loop()
-                if device.is_connected():
-                    temp = call_out_to_your_sensor_here()
-                    device.send_state({"temperature": temp})
-                time.sleep(1)
-        
-        
-        API Documentation
-        -----------------
-        
-        * `Device`_
-            * `constructor`_
-            * `connect`_
-            * `is_connected`_
-            * `close`_
-            * `send_state`_
-            * `loop`_
-            * `add_event_observer`_
-            * `remove_event_observer`_
-        
-        Device
-        ******
-        
-        A device represents a single thing or widget that you'd like to connect to the Losant platform.
-        A single device can contain many different sensors or other attached peripherals.
-        Devices can either report state or respond to commands.
-        
-        A device's state represents a snapshot of the device at some point in time.
-        If the device has a temperature sensor, it might report state every few seconds
-        with the temperature. If a device has a button, it might only report state when
-        the button is pressed. Devices can report state as often as needed by your specific application.
-        
-        Commands instruct a device to take a specific action. Commands are defined as a
-        name and an optional payload. For example, if the device is a scrolling marquee,
-        the command might be "update text" and the payload would include the text to update.
-        
-        constructor
-        ```````````
-        
-        ::
-        
-            Device(device_id, key, secret, secure=True, transport="tcp")
-        
-        The ``Device()`` constructor takes the following arguments:
-        
-        device_id
-            The device's ID. Obtained by first registering a device using the Losant platform.
-        
-        key
-            The Losant access key.
-        
-        secret
-            The Losant access secret.
-        
-        secure
-            If the client should connect to Losant over SSL - default is true.
-        
-        transport
-            Allowed values are "tcp" and "websockets". Defaults to "tcp", which is a raw TCP connection over
-            ports 1883 (insecure) or 8883 (secure). When "websockets" is passed in, connects using MQTT over
-            WebSockets, which uses either port 80 (insecure) or port 443 (secure).
-        
-        Example
-        .......
-        
-        ::
-        
-            from losantmqtt import Device
-        
-            device = Device("my-device-id", "my-app-access-key", "my-app-access-secret")
-        
-        connect
-        ```````
-        
-        ::
-        
-            connect(blocking=True)
-        
-        Connects the device to the Losant platform. Hook the connect event to know when a connection
-        has been successfully established.  Connect takes the following arguments:
-        
-        blocking
-            If the connect method should block or not.  True is the default, which means that the connect
-            call will be a blocking call that will not return until the connection is closed or an error
-            occurs - all interaction has to be done through the various event callbacks.  If blocking is
-            set to False, the function will only block until the connection is kicked off - after that point
-            you must run the network loop yourself, by calling the `loop`_ method periodically.
-        
-        is_connected
-        ````````````
-        
-        ::
-        
-            is_connected()
-        
-        Returns a boolean indicating whether or not the device is currently connected
-        to the Losant platform.
-        
-        close
-        `````
-        
-        ::
-        
-            close()
-        
-        Closes the device's connection to the Losant platform.
-        
-        send_state
-        ``````````
-        
-        ::
-        
-            send_state(state, time_like=None)
-        
-        Sends a device state to the Losant platform. In many scenarios, device states will
-        change rapidly. For example a GPS device will report GPS coordinates once a second or
-        more. Because of this, sendState is typically the most invoked function. Any state
-        data sent to Losant is stored and made available in data visualization tools
-        and workflow triggers.
-        
-        state
-            The state to send as a Dict.
-        
-        time_like
-            When the state occurred - if None or not set, will default to now.
-        
-        Example
-        .......
-        
-        ::
-        
-            device.send_state({ "voltage": read_analog_in() })
-        
-        loop
-        `````
-        
-        ::
-        
-            loop(timeout=1)
-        
-        Loops the network stack for the connection.  Only valid to call when connected in non-blocking mode.
-        Be sure to call this reasonably frequently when in that model to make sure the underlying
-        MQTT connection does not get timed out.
-        
-        timeout
-            Max time to block on the socket before continuing - defaults to 1 second.
-        
-        add_event_observer
-        ``````````````````
-        
-        ::
-        
-            add_event_observer(event_name, observer)
-        
-        Adds an observer to listen for an event on this device.
-        
-        event_name
-            The event to listen for.  Possible events are: "connect" (the device has connected),
-            "reconnect" (the device lost its connection and reconnected),
-            "close" (the device's connection was closed), and
-            "command" (the device has received a command from Losant).
-        
-        observer
-            Callback method to call when the given event fires.  The first argument for all callbacks
-            will be the device instance.  Command callbacks have a second argument - the command
-            received.
-        
-        
-        Example
-        .......
-        
-        ::
-        
-            def on_command(device, cmd):
-                print(cmd["time"]) # time of the command
-                print(cmd["name"]) # name of the command
-                print(cmd["payload"]) # payload of the command
-        
-            device.add_event_observer("command", on_command)
-        
-        remove_event_observer
-        `````````````````````
-        
-        ::
-        
-            remove_event_observer(event_name, observer)
-        
-        Removes an observer from listening for an event on this device.
-        
-        event_name
-            The event to stop listening for.  Same events as `add_event_observer`_.
-        
-        observer
-            Callback method to remove.
-        
-        
-        Copyright (c) 2019 Losant IoT, Inc
-        
-        https://www.losant.com
-        
 Keywords: MQTT,Losant,IoT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+Requires-Dist: paho-mqtt<2,>=1.6.1
+
+Losant Python MQTT Client
+=========================
+
+|travis-badge|_ |pypi-badge|_
+
+.. |travis-badge| image:: https://travis-ci.com/Losant/losant-mqtt-python.svg?branch=master
+.. _travis-badge:  https://app.travis-ci.com/github/Losant/losant-mqtt-python
+
+.. |pypi-badge| image:: https://badge.fury.io/py/losant-mqtt.svg
+.. _pypi-badge: https://badge.fury.io/py/losant-mqtt
+
+The `Losant <https://www.losant.com>`_ MQTT client provides a simple way for
+custom things to communicate with the Losant platform over MQTT.  You can authenticate
+as a device, publish device state, and listen for device commands.
+
+This client works with both Python 2.7 and 3. It uses the
+`Paho MQTT Client <https://github.com/eclipse/paho.mqtt.python>`_ under the
+covers for the actual MQTT communication.
+
+Installation
+------------
+
+The latest stable version is available in the Python Package Index (PyPi)
+and can be installed using
+
+::
+
+    pip install losant-mqtt
+
+
+Example
+-------
+
+Below is a high-level example of using the Losant Python MQTT client to send the value
+of a temperature sensor to the Losant platform.
+
+::
+
+    import time
+    from losantmqtt import Device
+
+    # Construct device
+    device = Device("my-device-id", "my-app-access-key", "my-app-access-secret")
+
+    def on_command(device, command):
+        print("Command received.")
+        print(command["name"])
+        print(command["payload"])
+
+    # Listen for commands.
+    device.add_event_observer("command", on_command)
+
+    # Connect to Losant.
+    device.connect(blocking=False)
+
+    # Send temperature once every second.
+    while True:
+        device.loop()
+        if device.is_connected():
+            temp = call_out_to_your_sensor_here()
+            device.send_state({"temperature": temp})
+        time.sleep(1)
+
+
+API Documentation
+-----------------
+
+* `Device`_
+    * `constructor`_
+    * `connect`_
+    * `is_connected`_
+    * `close`_
+    * `send_state`_
+    * `loop`_
+    * `add_event_observer`_
+    * `remove_event_observer`_
+
+Device
+******
+
+A device represents a single thing or widget that you'd like to connect to the Losant platform.
+A single device can contain many different sensors or other attached peripherals.
+Devices can either report state or respond to commands.
+
+A device's state represents a snapshot of the device at some point in time.
+If the device has a temperature sensor, it might report state every few seconds
+with the temperature. If a device has a button, it might only report state when
+the button is pressed. Devices can report state as often as needed by your specific application.
+
+Commands instruct a device to take a specific action. Commands are defined as a
+name and an optional payload. For example, if the device is a scrolling marquee,
+the command might be "update text" and the payload would include the text to update.
+
+constructor
+```````````
+
+::
+
+    Device(device_id, key, secret, secure=True, transport="tcp")
+
+The ``Device()`` constructor takes the following arguments:
+
+device_id
+    The device's ID. Obtained by first registering a device using the Losant platform.
+
+key
+    The Losant access key.
+
+secret
+    The Losant access secret.
+
+secure
+    If the client should connect to Losant over SSL - default is true.
+
+transport
+    Allowed values are "tcp" and "websockets". Defaults to "tcp", which is a raw TCP connection over
+    ports 1883 (insecure) or 8883 (secure). When "websockets" is passed in, connects using MQTT over
+    WebSockets, which uses either port 80 (insecure) or port 443 (secure).
+
+Example
+.......
+
+::
+
+    from losantmqtt import Device
+
+    device = Device("my-device-id", "my-app-access-key", "my-app-access-secret")
+
+connect
+```````
+
+::
+
+    connect(blocking=True)
+
+Connects the device to the Losant platform. Hook the connect event to know when a connection
+has been successfully established.  Connect takes the following arguments:
+
+blocking
+    If the connect method should block or not.  True is the default, which means that the connect
+    call will be a blocking call that will not return until the connection is closed or an error
+    occurs - all interaction has to be done through the various event callbacks.  If blocking is
+    set to False, the function will only block until the connection is kicked off - after that point
+    you must run the network loop yourself, by calling the `loop`_ method periodically.
+
+is_connected
+````````````
+
+::
+
+    is_connected()
+
+Returns a boolean indicating whether or not the device is currently connected
+to the Losant platform.
+
+close
+`````
+
+::
+
+    close()
+
+Closes the device's connection to the Losant platform.
+
+send_state
+``````````
+
+::
+
+    send_state(state, time_like=None)
+
+Sends a device state to the Losant platform. In many scenarios, device states will
+change rapidly. For example a GPS device will report GPS coordinates once a second or
+more. Because of this, sendState is typically the most invoked function. Any state
+data sent to Losant is stored and made available in data visualization tools
+and workflow triggers.
+
+state
+    The state to send as a Dict.
+
+time_like
+    When the state occurred - if None or not set, will default to now.
+
+Example
+.......
+
+::
+
+    device.send_state({ "voltage": read_analog_in() })
+
+loop
+`````
+
+::
+
+    loop(timeout=1)
+
+Loops the network stack for the connection.  Only valid to call when connected in non-blocking mode.
+Be sure to call this reasonably frequently when in that model to make sure the underlying
+MQTT connection does not get timed out.
+
+timeout
+    Max time to block on the socket before continuing - defaults to 1 second.
+
+add_event_observer
+``````````````````
+
+::
+
+    add_event_observer(event_name, observer)
+
+Adds an observer to listen for an event on this device.
+
+event_name
+    The event to listen for.  Possible events are: "connect" (the device has connected),
+    "reconnect" (the device lost its connection and reconnected),
+    "close" (the device's connection was closed), and
+    "command" (the device has received a command from Losant).
+
+observer
+    Callback method to call when the given event fires.  The first argument for all callbacks
+    will be the device instance.  Command callbacks have a second argument - the command
+    received.
+
+
+Example
+.......
+
+::
+
+    def on_command(device, cmd):
+        print(cmd["time"]) # time of the command
+        print(cmd["name"]) # name of the command
+        print(cmd["payload"]) # payload of the command
+
+    device.add_event_observer("command", on_command)
+
+remove_event_observer
+`````````````````````
+
+::
+
+    remove_event_observer(event_name, observer)
+
+Removes an observer from listening for an event on this device.
+
+event_name
+    The event to stop listening for.  Same events as `add_event_observer`_.
+
+observer
+    Callback method to remove.
+
+
+Copyright (c) 2024 Losant IoT, Inc
+
+https://www.losant.com
```

### Comparing `losant-mqtt-1.2.0/losant_mqtt.egg-info/PKG-INFO` & `losant-mqtt-1.2.1/losant_mqtt.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,279 +1,280 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: losant-mqtt
-Version: 1.2.0
+Version: 1.2.1
 Summary: An MQTT client for Losant
 Home-page: https://github.com/Losant/losant-mqtt-python
 Author: Losant
 Author-email: hello@losant.com
 License: MIT
-Description: Losant Python MQTT Client
-        =========================
-        
-        |travis-badge|_ |pypi-badge|_
-        
-        .. |travis-badge| image:: https://travis-ci.org/Losant/losant-mqtt-python.svg?branch=master
-        .. _travis-badge: https://travis-ci.org/Losant/losant-mqtt-python
-        
-        .. |pypi-badge| image:: https://badge.fury.io/py/losant-mqtt.svg
-        .. _pypi-badge: https://badge.fury.io/py/losant-mqtt
-        
-        The `Losant <https://www.losant.com>`_ MQTT client provides a simple way for
-        custom things to communicate with the Losant platform over MQTT.  You can authenticate
-        as a device, publish device state, and listen for device commands.
-        
-        This client works with both Python 2.7 and 3. It uses the
-        `Paho MQTT Client <https://github.com/eclipse/paho.mqtt.python>`_ under the
-        covers for the actual MQTT communication.
-        
-        Installation
-        ------------
-        
-        The latest stable version is available in the Python Package Index (PyPi)
-        and can be installed using
-        
-        ::
-        
-            pip install losant-mqtt
-        
-        
-        Example
-        -------
-        
-        Below is a high-level example of using the Losant Python MQTT client to send the value
-        of a temperature sensor to the Losant platform.
-        
-        ::
-        
-            import time
-            from losantmqtt import Device
-        
-            # Construct device
-            device = Device("my-device-id", "my-app-access-key", "my-app-access-secret")
-        
-            def on_command(device, command):
-                print("Command received.")
-                print(command["name"])
-                print(command["payload"])
-        
-            # Listen for commands.
-            device.add_event_observer("command", on_command)
-        
-            # Connect to Losant.
-            device.connect(blocking=False)
-        
-            # Send temperature once every second.
-            while True:
-                device.loop()
-                if device.is_connected():
-                    temp = call_out_to_your_sensor_here()
-                    device.send_state({"temperature": temp})
-                time.sleep(1)
-        
-        
-        API Documentation
-        -----------------
-        
-        * `Device`_
-            * `constructor`_
-            * `connect`_
-            * `is_connected`_
-            * `close`_
-            * `send_state`_
-            * `loop`_
-            * `add_event_observer`_
-            * `remove_event_observer`_
-        
-        Device
-        ******
-        
-        A device represents a single thing or widget that you'd like to connect to the Losant platform.
-        A single device can contain many different sensors or other attached peripherals.
-        Devices can either report state or respond to commands.
-        
-        A device's state represents a snapshot of the device at some point in time.
-        If the device has a temperature sensor, it might report state every few seconds
-        with the temperature. If a device has a button, it might only report state when
-        the button is pressed. Devices can report state as often as needed by your specific application.
-        
-        Commands instruct a device to take a specific action. Commands are defined as a
-        name and an optional payload. For example, if the device is a scrolling marquee,
-        the command might be "update text" and the payload would include the text to update.
-        
-        constructor
-        ```````````
-        
-        ::
-        
-            Device(device_id, key, secret, secure=True, transport="tcp")
-        
-        The ``Device()`` constructor takes the following arguments:
-        
-        device_id
-            The device's ID. Obtained by first registering a device using the Losant platform.
-        
-        key
-            The Losant access key.
-        
-        secret
-            The Losant access secret.
-        
-        secure
-            If the client should connect to Losant over SSL - default is true.
-        
-        transport
-            Allowed values are "tcp" and "websockets". Defaults to "tcp", which is a raw TCP connection over
-            ports 1883 (insecure) or 8883 (secure). When "websockets" is passed in, connects using MQTT over
-            WebSockets, which uses either port 80 (insecure) or port 443 (secure).
-        
-        Example
-        .......
-        
-        ::
-        
-            from losantmqtt import Device
-        
-            device = Device("my-device-id", "my-app-access-key", "my-app-access-secret")
-        
-        connect
-        ```````
-        
-        ::
-        
-            connect(blocking=True)
-        
-        Connects the device to the Losant platform. Hook the connect event to know when a connection
-        has been successfully established.  Connect takes the following arguments:
-        
-        blocking
-            If the connect method should block or not.  True is the default, which means that the connect
-            call will be a blocking call that will not return until the connection is closed or an error
-            occurs - all interaction has to be done through the various event callbacks.  If blocking is
-            set to False, the function will only block until the connection is kicked off - after that point
-            you must run the network loop yourself, by calling the `loop`_ method periodically.
-        
-        is_connected
-        ````````````
-        
-        ::
-        
-            is_connected()
-        
-        Returns a boolean indicating whether or not the device is currently connected
-        to the Losant platform.
-        
-        close
-        `````
-        
-        ::
-        
-            close()
-        
-        Closes the device's connection to the Losant platform.
-        
-        send_state
-        ``````````
-        
-        ::
-        
-            send_state(state, time_like=None)
-        
-        Sends a device state to the Losant platform. In many scenarios, device states will
-        change rapidly. For example a GPS device will report GPS coordinates once a second or
-        more. Because of this, sendState is typically the most invoked function. Any state
-        data sent to Losant is stored and made available in data visualization tools
-        and workflow triggers.
-        
-        state
-            The state to send as a Dict.
-        
-        time_like
-            When the state occurred - if None or not set, will default to now.
-        
-        Example
-        .......
-        
-        ::
-        
-            device.send_state({ "voltage": read_analog_in() })
-        
-        loop
-        `````
-        
-        ::
-        
-            loop(timeout=1)
-        
-        Loops the network stack for the connection.  Only valid to call when connected in non-blocking mode.
-        Be sure to call this reasonably frequently when in that model to make sure the underlying
-        MQTT connection does not get timed out.
-        
-        timeout
-            Max time to block on the socket before continuing - defaults to 1 second.
-        
-        add_event_observer
-        ``````````````````
-        
-        ::
-        
-            add_event_observer(event_name, observer)
-        
-        Adds an observer to listen for an event on this device.
-        
-        event_name
-            The event to listen for.  Possible events are: "connect" (the device has connected),
-            "reconnect" (the device lost its connection and reconnected),
-            "close" (the device's connection was closed), and
-            "command" (the device has received a command from Losant).
-        
-        observer
-            Callback method to call when the given event fires.  The first argument for all callbacks
-            will be the device instance.  Command callbacks have a second argument - the command
-            received.
-        
-        
-        Example
-        .......
-        
-        ::
-        
-            def on_command(device, cmd):
-                print(cmd["time"]) # time of the command
-                print(cmd["name"]) # name of the command
-                print(cmd["payload"]) # payload of the command
-        
-            device.add_event_observer("command", on_command)
-        
-        remove_event_observer
-        `````````````````````
-        
-        ::
-        
-            remove_event_observer(event_name, observer)
-        
-        Removes an observer from listening for an event on this device.
-        
-        event_name
-            The event to stop listening for.  Same events as `add_event_observer`_.
-        
-        observer
-            Callback method to remove.
-        
-        
-        Copyright (c) 2019 Losant IoT, Inc
-        
-        https://www.losant.com
-        
 Keywords: MQTT,Losant,IoT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+Requires-Dist: paho-mqtt<2,>=1.6.1
+
+Losant Python MQTT Client
+=========================
+
+|travis-badge|_ |pypi-badge|_
+
+.. |travis-badge| image:: https://travis-ci.com/Losant/losant-mqtt-python.svg?branch=master
+.. _travis-badge:  https://app.travis-ci.com/github/Losant/losant-mqtt-python
+
+.. |pypi-badge| image:: https://badge.fury.io/py/losant-mqtt.svg
+.. _pypi-badge: https://badge.fury.io/py/losant-mqtt
+
+The `Losant <https://www.losant.com>`_ MQTT client provides a simple way for
+custom things to communicate with the Losant platform over MQTT.  You can authenticate
+as a device, publish device state, and listen for device commands.
+
+This client works with both Python 2.7 and 3. It uses the
+`Paho MQTT Client <https://github.com/eclipse/paho.mqtt.python>`_ under the
+covers for the actual MQTT communication.
+
+Installation
+------------
+
+The latest stable version is available in the Python Package Index (PyPi)
+and can be installed using
+
+::
+
+    pip install losant-mqtt
+
+
+Example
+-------
+
+Below is a high-level example of using the Losant Python MQTT client to send the value
+of a temperature sensor to the Losant platform.
+
+::
+
+    import time
+    from losantmqtt import Device
+
+    # Construct device
+    device = Device("my-device-id", "my-app-access-key", "my-app-access-secret")
+
+    def on_command(device, command):
+        print("Command received.")
+        print(command["name"])
+        print(command["payload"])
+
+    # Listen for commands.
+    device.add_event_observer("command", on_command)
+
+    # Connect to Losant.
+    device.connect(blocking=False)
+
+    # Send temperature once every second.
+    while True:
+        device.loop()
+        if device.is_connected():
+            temp = call_out_to_your_sensor_here()
+            device.send_state({"temperature": temp})
+        time.sleep(1)
+
+
+API Documentation
+-----------------
+
+* `Device`_
+    * `constructor`_
+    * `connect`_
+    * `is_connected`_
+    * `close`_
+    * `send_state`_
+    * `loop`_
+    * `add_event_observer`_
+    * `remove_event_observer`_
+
+Device
+******
+
+A device represents a single thing or widget that you'd like to connect to the Losant platform.
+A single device can contain many different sensors or other attached peripherals.
+Devices can either report state or respond to commands.
+
+A device's state represents a snapshot of the device at some point in time.
+If the device has a temperature sensor, it might report state every few seconds
+with the temperature. If a device has a button, it might only report state when
+the button is pressed. Devices can report state as often as needed by your specific application.
+
+Commands instruct a device to take a specific action. Commands are defined as a
+name and an optional payload. For example, if the device is a scrolling marquee,
+the command might be "update text" and the payload would include the text to update.
+
+constructor
+```````````
+
+::
+
+    Device(device_id, key, secret, secure=True, transport="tcp")
+
+The ``Device()`` constructor takes the following arguments:
+
+device_id
+    The device's ID. Obtained by first registering a device using the Losant platform.
+
+key
+    The Losant access key.
+
+secret
+    The Losant access secret.
+
+secure
+    If the client should connect to Losant over SSL - default is true.
+
+transport
+    Allowed values are "tcp" and "websockets". Defaults to "tcp", which is a raw TCP connection over
+    ports 1883 (insecure) or 8883 (secure). When "websockets" is passed in, connects using MQTT over
+    WebSockets, which uses either port 80 (insecure) or port 443 (secure).
+
+Example
+.......
+
+::
+
+    from losantmqtt import Device
+
+    device = Device("my-device-id", "my-app-access-key", "my-app-access-secret")
+
+connect
+```````
+
+::
+
+    connect(blocking=True)
+
+Connects the device to the Losant platform. Hook the connect event to know when a connection
+has been successfully established.  Connect takes the following arguments:
+
+blocking
+    If the connect method should block or not.  True is the default, which means that the connect
+    call will be a blocking call that will not return until the connection is closed or an error
+    occurs - all interaction has to be done through the various event callbacks.  If blocking is
+    set to False, the function will only block until the connection is kicked off - after that point
+    you must run the network loop yourself, by calling the `loop`_ method periodically.
+
+is_connected
+````````````
+
+::
+
+    is_connected()
+
+Returns a boolean indicating whether or not the device is currently connected
+to the Losant platform.
+
+close
+`````
+
+::
+
+    close()
+
+Closes the device's connection to the Losant platform.
+
+send_state
+``````````
+
+::
+
+    send_state(state, time_like=None)
+
+Sends a device state to the Losant platform. In many scenarios, device states will
+change rapidly. For example a GPS device will report GPS coordinates once a second or
+more. Because of this, sendState is typically the most invoked function. Any state
+data sent to Losant is stored and made available in data visualization tools
+and workflow triggers.
+
+state
+    The state to send as a Dict.
+
+time_like
+    When the state occurred - if None or not set, will default to now.
+
+Example
+.......
+
+::
+
+    device.send_state({ "voltage": read_analog_in() })
+
+loop
+`````
+
+::
+
+    loop(timeout=1)
+
+Loops the network stack for the connection.  Only valid to call when connected in non-blocking mode.
+Be sure to call this reasonably frequently when in that model to make sure the underlying
+MQTT connection does not get timed out.
+
+timeout
+    Max time to block on the socket before continuing - defaults to 1 second.
+
+add_event_observer
+``````````````````
+
+::
+
+    add_event_observer(event_name, observer)
+
+Adds an observer to listen for an event on this device.
+
+event_name
+    The event to listen for.  Possible events are: "connect" (the device has connected),
+    "reconnect" (the device lost its connection and reconnected),
+    "close" (the device's connection was closed), and
+    "command" (the device has received a command from Losant).
+
+observer
+    Callback method to call when the given event fires.  The first argument for all callbacks
+    will be the device instance.  Command callbacks have a second argument - the command
+    received.
+
+
+Example
+.......
+
+::
+
+    def on_command(device, cmd):
+        print(cmd["time"]) # time of the command
+        print(cmd["name"]) # name of the command
+        print(cmd["payload"]) # payload of the command
+
+    device.add_event_observer("command", on_command)
+
+remove_event_observer
+`````````````````````
+
+::
+
+    remove_event_observer(event_name, observer)
+
+Removes an observer from listening for an event on this device.
+
+event_name
+    The event to stop listening for.  Same events as `add_event_observer`_.
+
+observer
+    Callback method to remove.
+
+
+Copyright (c) 2024 Losant IoT, Inc
+
+https://www.losant.com
```

### Comparing `losant-mqtt-1.2.0/LICENSE` & `losant-mqtt-1.2.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2019 Losant IoT Inc.
+Copyright (c) 2024 Losant IoT Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `losant-mqtt-1.2.0/setup.py` & `losant-mqtt-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='losant-mqtt',
-    version='1.2.0',
+    version='1.2.1',
     description='An MQTT client for Losant',
     long_description=long_description,
     url='https://github.com/Losant/losant-mqtt-python',
     author='Losant',
     author_email='hello@losant.com',
     license='MIT',
     classifiers=[
@@ -34,9 +34,9 @@
     packages=find_packages(exclude=['tests']),
     include_package_data=True,
     package_data={
         'losantmqtt': ['RootCA.crt']
     },
     keywords=["MQTT", "Losant", "IoT"],
     test_suite='tests',
-    install_requires=['paho-mqtt>=1.2,<2']
+    install_requires=['paho-mqtt>=1.6.1,<2']
 )
```

### Comparing `losant-mqtt-1.2.0/README.rst` & `losant-mqtt-1.2.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Losant Python MQTT Client
 =========================
 
 |travis-badge|_ |pypi-badge|_
 
-.. |travis-badge| image:: https://travis-ci.org/Losant/losant-mqtt-python.svg?branch=master
-.. _travis-badge: https://travis-ci.org/Losant/losant-mqtt-python
+.. |travis-badge| image:: https://travis-ci.com/Losant/losant-mqtt-python.svg?branch=master
+.. _travis-badge:  https://app.travis-ci.com/github/Losant/losant-mqtt-python
 
 .. |pypi-badge| image:: https://badge.fury.io/py/losant-mqtt.svg
 .. _pypi-badge: https://badge.fury.io/py/losant-mqtt
 
 The `Losant <https://www.losant.com>`_ MQTT client provides a simple way for
 custom things to communicate with the Losant platform over MQTT.  You can authenticate
 as a device, publish device state, and listen for device commands.
@@ -247,10 +247,10 @@
 event_name
     The event to stop listening for.  Same events as `add_event_observer`_.
 
 observer
     Callback method to remove.
 
 
-Copyright (c) 2019 Losant IoT, Inc
+Copyright (c) 2024 Losant IoT, Inc
 
 https://www.losant.com
```

### Comparing `losant-mqtt-1.2.0/losantmqtt/device.py` & `losant-mqtt-1.2.1/losantmqtt/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 The MIT License (MIT)
 
-Copyright (c) 2019 Losant IoT, Inc.
+Copyright (c) 2024 Losant IoT, Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `losant-mqtt-1.2.0/losantmqtt/__init__.py` & `losant-mqtt-1.2.1/losantmqtt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 The MIT License (MIT)
 
-Copyright (c) 2019 Losant IoT, Inc.
+Copyright (c) 2024 Losant IoT, Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

