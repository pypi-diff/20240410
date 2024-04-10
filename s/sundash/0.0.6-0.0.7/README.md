# Comparing `tmp/sundash-0.0.6.tar.gz` & `tmp/sundash-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sundash-0.0.6.tar", max compression
+gzip compressed data, was "sundash-0.0.7.tar", max compression
```

## Comparing `sundash-0.0.6.tar` & `sundash-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1081 2023-10-16 04:23:44.524607 sundash-0.0.6/LICENSE
--rw-r--r--   0        0        0     2379 2023-12-02 19:05:44.939174 sundash-0.0.6/README.md
--rw-r--r--   0        0        0     1410 2023-12-21 04:18:00.027905 sundash-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      161 2023-11-19 22:18:45.435543 sundash-0.0.6/sundash/__init__.py
--rw-r--r--   0        0        0      348 2023-11-19 11:58:55.518286 sundash-0.0.6/sundash/_utils.py
--rw-r--r--   0        0        0     3290 2023-12-09 05:07:31.163351 sundash-0.0.6/sundash/core.py
--rw-r--r--   0        0        0     3757 2023-12-02 21:24:32.520121 sundash-0.0.6/sundash/layout.py
--rw-r--r--   0        0        0     1030 2023-12-02 19:02:27.620554 sundash-0.0.6/sundash/logging.py
--rw-r--r--   0        0        0     5019 2023-12-21 04:17:31.519953 sundash-0.0.6/sundash/server.py
--rw-r--r--   0        0        0      840 2023-12-21 01:14:06.577645 sundash-0.0.6/sundash/tables.py
--rw-r--r--   0        0        0     2424 2023-12-02 21:37:07.939941 sundash-0.0.6/sundash/web/app.js
--rw-r--r--   0        0        0    16958 2023-10-07 04:34:35.207533 sundash-0.0.6/sundash/web/favicon.ico
--rw-r--r--   0        0        0      347 2023-12-02 22:54:18.682740 sundash-0.0.6/sundash/web/index.html
--rw-r--r--   0        0        0     1479 2023-12-21 00:35:58.433207 sundash-0.0.6/sundash/web/style.css
--rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 sundash-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-02-01 03:27:07.719839 sundash-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3256 2024-04-10 05:12:40.699945 sundash-0.0.7/README.md
+-rw-r--r--   0        0        0     1452 2024-04-10 05:22:42.862155 sundash-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      121 2024-03-31 15:33:49.198939 sundash-0.0.7/sundash/__init__.py
+-rw-r--r--   0        0        0     6144 2024-04-10 05:05:48.824502 sundash-0.0.7/sundash/app.py
+-rw-r--r--   0        0        0     1133 2024-04-08 02:12:10.280561 sundash-0.0.7/sundash/html.py
+-rw-r--r--   0        0        0      980 2024-04-06 17:33:28.867805 sundash-0.0.7/sundash/logging.py
+-rw-r--r--   0        0        0      667 2024-04-06 21:06:06.925089 sundash-0.0.7/sundash/messages.py
+-rw-r--r--   0        0        0     1121 2024-04-10 03:54:36.441448 sundash-0.0.7/sundash/scheduler.py
+-rw-r--r--   0        0        0     4344 2024-04-10 05:06:46.725423 sundash-0.0.7/sundash/server.py
+-rw-r--r--   0        0        0     2173 2024-04-10 05:03:38.322678 sundash-0.0.7/sundash/sessions.py
+-rw-r--r--   0        0        0      780 2024-04-08 03:03:46.602150 sundash-0.0.7/sundash/tables.py
+-rw-r--r--   0        0        0      348 2024-03-23 14:05:10.127805 sundash-0.0.7/sundash/utils.py
+-rw-r--r--   0        0        0     2424 2024-04-06 21:13:47.562598 sundash-0.0.7/sundash/web/client.js
+-rw-r--r--   0        0        0    16958 2023-10-07 04:34:35.207533 sundash-0.0.7/sundash/web/favicon.ico
+-rw-r--r--   0        0        0      350 2024-02-10 08:59:35.763541 sundash-0.0.7/sundash/web/index.html
+-rw-r--r--   0        0        0     1524 2024-04-06 15:15:40.253135 sundash-0.0.7/sundash/web/style.css
+-rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 sundash-0.0.7/PKG-INFO
```

### Comparing `sundash-0.0.6/LICENSE` & `sundash-0.0.7/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 Danil Tryapchev
+Copyright (c) 2024 Danil Tryapchev
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sundash-0.0.6/pyproject.toml` & `sundash-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 [tool.poetry]
 name = "sundash"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python & JS micro framework for realtime web UI applications"
 authors = ["Danil Tryapchev <ruthus18@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ruthus18/sundash"
 keywords = ["backend", "frontend", "server", "client", "ws", "framework"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
-uvicorn = "^0.23.2"
+uvicorn = "^0.29.0"
 websockets = "^12.0"
-starlette = "^0.33.0"
-colorlog = "^6.7.0"
+starlette = "^0.37.2"
+colorlog = "^6.8.2"
 
 [tool.poetry.group.dev.dependencies]
-ipython = "^8.17.2"
+ipython = "^8.21.0"
 ipdb = "^0.13.13"
-flake8 = "^6.1.0"
+flake8 = "^7.0.0"
 flake8-pyproject = "^1.2.3"
-isort = "^5.12.0"
-poethepoet = "^0.24.4"
+isort = "^5.13.2"
+poethepoet = "^0.25.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.flake8]
 max-complexity = 8
-max-line-length = 120
+max-line-length = 79
 ignore = [
     "E701",  # multiple statements on one line
     "E704",  # multiple statements on one line
     "E203",  # whitespace before ':'
     "E731",  # do not assign a lambda expression, use a def
     "E402",  # module level import not at top of file
     "W504",  # line break after binary operator
 ]
+exclude = ["docs", "examples/__main__.py"]
 
 [tool.isort]
 multi_line_output = 3
 line_length = 79
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
```

### Comparing `sundash-0.0.6/sundash/logging.py` & `sundash-0.0.7/sundash/logging.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 
 log_config = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
         "default": {
             "class": "colorlog.ColoredFormatter",
-            "format": ("{green}[{asctime}]{reset} {bg_green}{levelname}{reset} {blue}{name}:{reset} {message}"),
+            "format": (
+                "{green}[{asctime}]{reset} {bg_green}{levelname}{reset} "
+                "{blue}{name}:{reset} {message}"
+            ),
             "style": "{",
         },
     },
     "filters": {},
     "handlers": {
         "stdout": {
             "level": "INFO",
@@ -24,21 +27,17 @@
         },
     },
     "loggers": {
         "": {
             "handlers": ["stdout"],
             "level": logging.DEBUG,
         },
-        "uvicorn.access": {
-            "handlers": ["null"],
-            "propagate": False,
-        },
         "asyncio": {
-            "handlers": ["null"],
-            "propagate": False,
+            "handlers": ["stdout"],
+            "level": logging.ERROR,
         },
     },
 }
 
 
 def setup():
     logging.config.dictConfig(log_config)
```

### Comparing `sundash-0.0.6/sundash/web/app.js` & `sundash-0.0.7/sundash/web/client.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -9,22 +9,22 @@
     data = data.join(' ')
     console.log(`${name} ${data}`)
 
     if (data != undefined) {
         data = JSON.parse(data)
     }
 
-    if (name == 'CLEAR_LAYOUT') {
+    if (name == 'ClearLayout') {
         clear_layout()
-    } else if (name == 'UPDATE_LAYOUT') {
+    } else if (name == 'UpdateLayout') {
         update_layout(data)
-    } else if (name == 'SET_VAR') {
+    } else if (name == 'SetVar') {
         set_var(data)
     } else {
-        console.error(`dispatching error: ${event.data}`)
+        console.error(`[!!!] dispatching error: ${event.data}`)
     }
 }
 
 socket.onclose = event => {
     if (event.wasClean) {
         console.log(
             `[WS] CONN_CLOSED: code=${event.code} reason=${event.reason}`
@@ -44,34 +44,34 @@
 
 
 const app = document.getElementById('app')
 
 
 function clear_layout() {
     app.innerHTML = ''
-    socket.send('LAYOUT_CLEAN {}')
+    socket.send('LayoutClean {}')
 }
 
 
 function _init_buttons() {
     const buttons = [...document.getElementsByTagName('button')]
     buttons.forEach(button => {
         button.onclick = () => {
-            socket.send(`BUTTON_CLICK {"button_id": "${button.id}"}`)
+            socket.send(`ButtonClick {"button_id": "${button.id}"}`)
         }
     })
 }
 
 
 function _init_inputs() {
     const inputs = [...document.getElementsByTagName('input')]
     inputs.forEach(input => {
         console.log(input)
         input.onchange = (e) => {
-            socket.send(`INPUT_UPDATED {"name": "${input.name}", "value": "${input.value}"}`)
+            socket.send(`InputUpdated {"name": "${input.name}", "value": "${input.value}"}`)
             e.target.value = ''
         }
     })
 }
 
 
 function update_layout(data) {
@@ -85,19 +85,19 @@
         response_html = response_html.replace(`{{ ${key} }}`, value)
     }
 
     app.innerHTML = response_html
     _init_buttons()
     _init_inputs()
 
-    socket.send('LAYOUT_UPDATED {}')
+    socket.send('LayoutUpdated {}')
 }
 
 
 function set_var(data) {
-    app.__vars[data.key] = data.value
-    app.innerHTML = app.__html.replace(`{{ ${data.key} }}`, data.value)
+    app.__vars[data.name] = data.value
+    app.innerHTML = app.__html.replace(`{{ ${data.name} }}`, data.value)
     _init_buttons()
     _init_inputs()
 
-    socket.send('VAR_SET {}')
+    socket.send('VarSet {}')
 }
```

### Comparing `sundash-0.0.6/sundash/web/favicon.ico` & `sundash-0.0.7/sundash/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `sundash-0.0.6/sundash/web/style.css` & `sundash-0.0.7/sundash/web/style.css`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,18 @@
 }
 
 th,td {
     padding: 10px 5px;
     border-bottom: 1px solid #928374;
 }
 
+tr:hover {
+    background-color: #282828;
+}
+
 
 #app {
     width: 1000px;
     margin-left: auto;
     margin-right: auto;
 }
```

### Comparing `sundash-0.0.6/PKG-INFO` & `sundash-0.0.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: sundash
-Version: 0.0.6
-Summary: Python & JS micro framework for realtime web UI applications
-Home-page: https://github.com/ruthus18/sundash
-License: MIT
-Keywords: backend,frontend,server,client,ws,framework
-Author: Danil Tryapchev
-Author-email: ruthus18@gmail.com
-Requires-Python: >=3.12,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: colorlog (>=6.7.0,<7.0.0)
-Requires-Dist: starlette (>=0.33.0,<0.34.0)
-Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
-Requires-Dist: websockets (>=12.0,<13.0)
-Project-URL: Repository, https://github.com/ruthus18/sundash
-Description-Content-Type: text/markdown
-
 # Sundash
 
 **Python & JS micro framework for realtime web UI applications**
 
 * **ASGI-based** -- minimal 3rd party dependencies and clean core part
 * **Flexible and extensible** -- easy to customize, add 3rd party integrations
 * **Realtime** -- operating through websockets bus, client & backend in app
@@ -31,58 +12,108 @@
 
 ### Installation
 
 ```bash
     pip install sundash
 ```
 
+
 ### Examples
 
-Check `examples` folder.
+```bash
+    python -m examples <num | name>
+```
 
-Run example (counter with buttons and user interaction):
+To run Hello World example:
 
 ```bash
-    python -m examples counter
+    python -m examples hello  # passing 01 also works
 ```
 
+Available examples:
+
+* `01 hello` - show plain HTML string
+* `02 buttons` - counter with clickable buttons
+* `03 clock` - realtime clock (scheduler events)
+* `04 menu` - simple page routing
+* `05 search` - handling signle form input
+* `06 tables` - static tables
+
 
-### Basic example
+**Client interaction example:**
 
 ```python
-    import datetime as dt
+from dataclasses import dataclass
 
-    from sundash import EVERY_SECOND
-    from sundash import App
-    from sundash import Component
-    from sundash import on
-    
+from sundash import App
+from sundash import Component
+from sundash import on
+from sundash.app import ButtonClick
 
-    app = App()
+app = App()
 
-    now = lambda: dt.datetime.now().strftime('%H:%M:%S')
 
+class Counter(Component):
+    html = '''
+        <button id="minus">-</button>
+        <b>{{ count }}</b>
+        <button id="plus">+</button>
+    '''
 
-    class Clock(Component):
-        html = '<p><b>Time: </b>{{ time }}<p/>'
+    @dataclass
+    class Vars:
+        count: int = 0
 
-        class Vars:
-            # you can pass init values (static or procedural)
-            time: str = now
+    @on(ButtonClick)
+    async def on_click(self, event: ButtonClick):
+        if 'plus' == event.button_id:
+            self.vars.count += 1
 
-        # run callback when user open webpage
-        @on(EVERY_SECOND)
-        async def update(self, _):
-            await self.set('time', now())  # live update of value
+        elif 'minus' == event.button_id:
+            self.vars.count -= 1
 
-    # add plain HTML or own components
-    app.run(layout=('<h1>🕰️ Clock</h1>', Clock))
+        await self.update_var('count')
+
+
+app.run_sync(['<h1>🧮 Counter</h1>', Counter])
 ```
 
-![clock](examples/img/_02_clock.png "Clock")
+
+**Server Interaction Example:**
+
+```python
+import dataclasses as dc
+import datetime as dt
+
+from sundash import Component
+from sundash import on
+from sundash.scheduler import EverySecond
+from sundash.scheduler import SchedulerApp
+
+app = SchedulerApp()
+
+
+now = lambda: dt.datetime.now().strftime('%H:%M:%S')
+
+
+class Clock(Component):
+    html = '<p><b>Time:</b> {{ time }}<p/>'
+
+    @dc.dataclass
+    class Vars:
+        time: str = dc.field(default_factory=now)
+
+    @on(EverySecond)
+    async def update(self, _):
+        self.vars.time = now()
+        await self.update_var('time')
+
+
+app.run_sync(['<h1>🕰️ Clock</h1>', Clock])
+```
 
 
 ### В чем идея?
 
 Хочу пробрасывать real-time интерфейс к JS либам, чтобы была возможность
 написать любую веб-морду для любых системных инструментов.
 
@@ -94,8 +125,7 @@
 
 ### Development
 
 * Required: python 3.12, poetry, virtualenv
 * Install Python dependencies: `poetry install --with=dev`
 * Run local linters: `poe q`
 * Publish package: `poetry publish --build`
-
```

