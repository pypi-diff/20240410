# Comparing `tmp/wawona-1.0.0.tar.gz` & `tmp/wawona-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wawona-1.0.0.tar", last modified: Wed Mar 27 12:25:06 2024, max compression
+gzip compressed data, was "wawona-1.1.0.tar", last modified: Wed Apr 10 12:10:10 2024, max compression
```

## Comparing `wawona-1.0.0.tar` & `wawona-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-03-27 12:25:06.140952 wawona-1.0.0/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.0.0/LICENSE
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     4999 2024-03-27 12:25:06.139998 wawona-1.0.0/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     3960 2024-03-27 12:17:52.000000 wawona-1.0.0/README.md
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1075 2024-03-27 12:20:31.000000 wawona-1.0.0/pyproject.toml
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-03-27 12:25:06.141134 wawona-1.0.0/setup.cfg
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-03-27 12:25:06.077357 wawona-1.0.0/src/
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-03-27 12:25:06.107329 wawona-1.0.0/src/wawona/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.0.0/src/wawona/__init__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.0.0/src/wawona/__main__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)    18045 2024-03-25 12:34:23.000000 wawona-1.0.0/src/wawona/wawona.py
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-03-27 12:25:06.139084 wawona-1.0.0/src/wawona.egg-info/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     4999 2024-03-27 12:25:06.000000 wawona-1.0.0/src/wawona.egg-info/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-03-27 12:25:06.000000 wawona-1.0.0/src/wawona.egg-info/SOURCES.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-03-27 12:25:06.000000 wawona-1.0.0/src/wawona.egg-info/dependency_links.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-03-27 12:25:06.000000 wawona-1.0.0/src/wawona.egg-info/entry_points.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       79 2024-03-27 12:25:06.000000 wawona-1.0.0/src/wawona.egg-info/requires.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-03-27 12:25:06.000000 wawona-1.0.0/src/wawona.egg-info/top_level.txt
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-10 12:10:10.335307 wawona-1.1.0/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.1.0/LICENSE
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5087 2024-04-10 12:10:10.334512 wawona-1.1.0/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     4048 2024-04-03 23:20:59.000000 wawona-1.1.0/README.md
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1075 2024-04-10 12:09:00.000000 wawona-1.1.0/pyproject.toml
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-04-10 12:10:10.335673 wawona-1.1.0/setup.cfg
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-10 12:10:10.326083 wawona-1.1.0/src/
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-10 12:10:10.329921 wawona-1.1.0/src/wawona/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.1.0/src/wawona/__init__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.1.0/src/wawona/__main__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)    19224 2024-04-03 23:29:59.000000 wawona-1.1.0/src/wawona/wawona.py
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-10 12:10:10.333827 wawona-1.1.0/src/wawona.egg-info/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5087 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/SOURCES.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/dependency_links.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/entry_points.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       79 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/requires.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/top_level.txt
```

### Comparing `wawona-1.0.0/LICENSE` & `wawona-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wawona-1.0.0/PKG-INFO` & `wawona-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.0.0
+Version: 1.1.0
 Summary: Easily make office reservations in sequoia from the command line.
 Author-email: yuzawa-san <jtyuzawa@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
@@ -28,15 +28,15 @@
 by [@yuzawa-san](https://github.com/yuzawa-san/)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/wawona)](https://pypi.org/project/wawona/)
 
 Easily make office reservations in sequoia from the command line.
 This tool is provides streamlined workflows:
 
-- viewing the next two week's bookings from coworkers that you have followed
+- viewing the next two week's bookings from coworkers that you have followed (in the app/[site](https://px.sequoia.com/workplace))
 - booking multiple days at a time
 - doing space reservations (with the ability to save your preferred space)
 - if an option contains a single choice, automatically select that choice
 
 ```
 +----------------------+-----+-----+-----+-----+-----+
 | WEEK OF 11 MAR       | Mon | Tue | Wed | Thu | Fri |
@@ -78,16 +78,14 @@
   Mar 27 New York Reservation
   Complete Self-Screening
   Seat Not Selected
 
 [?] Complete task? (Y/n): 
 [?] I am healthy and not sick?: Yes (only choice)
 [?] Floor: Floor 2 (only choice)
-[?] Preferred space ID (press return for none): 
-Preferred space is not available
 [?] Space: 
    Desk 35
    Desk 36
    Desk 37
    Desk 38
    Desk 39
    Desk 40
@@ -127,20 +125,27 @@
 
 ## Usage 
 
 - Run it from your terminal: `wawona`
 - On initial run, you will be asked provide configuration: email and password.
 - You may be prompted to for an MFA token periodically.
 - Use the up/down arrows, spacebar, and return keys to select items in lists
+- Troubleshooting errors with `wawona --verbose`
 
 ### Reset
 
 If you need to reset to factory defaults (maybe if you changed your password), remove the configuration:
 
 ```console
+wawona reset
+```
+
+As a last resort, if all else fails:
+
+```console
 rm -rf ~/.config/wawona/
 ```
 
 ## Notes
 
 - Not affliated with sequoia
 - Uses public endpoints discovered from the web UI
```

### Comparing `wawona-1.0.0/README.md` & `wawona-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 by [@yuzawa-san](https://github.com/yuzawa-san/)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/wawona)](https://pypi.org/project/wawona/)
 
 Easily make office reservations in sequoia from the command line.
 This tool is provides streamlined workflows:
 
-- viewing the next two week's bookings from coworkers that you have followed
+- viewing the next two week's bookings from coworkers that you have followed (in the app/[site](https://px.sequoia.com/workplace))
 - booking multiple days at a time
 - doing space reservations (with the ability to save your preferred space)
 - if an option contains a single choice, automatically select that choice
 
 ```
 +----------------------+-----+-----+-----+-----+-----+
 | WEEK OF 11 MAR       | Mon | Tue | Wed | Thu | Fri |
@@ -53,16 +53,14 @@
   Mar 27 New York Reservation
   Complete Self-Screening
   Seat Not Selected
 
 [?] Complete task? (Y/n): 
 [?] I am healthy and not sick?: Yes (only choice)
 [?] Floor: Floor 2 (only choice)
-[?] Preferred space ID (press return for none): 
-Preferred space is not available
 [?] Space: 
    Desk 35
    Desk 36
    Desk 37
    Desk 38
    Desk 39
    Desk 40
@@ -102,20 +100,27 @@
 
 ## Usage 
 
 - Run it from your terminal: `wawona`
 - On initial run, you will be asked provide configuration: email and password.
 - You may be prompted to for an MFA token periodically.
 - Use the up/down arrows, spacebar, and return keys to select items in lists
+- Troubleshooting errors with `wawona --verbose`
 
 ### Reset
 
 If you need to reset to factory defaults (maybe if you changed your password), remove the configuration:
 
 ```console
+wawona reset
+```
+
+As a last resort, if all else fails:
+
+```console
 rm -rf ~/.config/wawona/
 ```
 
 ## Notes
 
 - Not affliated with sequoia
 - Uses public endpoints discovered from the web UI
```

### Comparing `wawona-1.0.0/pyproject.toml` & `wawona-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wawona"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="yuzawa-san", email="jtyuzawa@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Easily make office reservations in sequoia from the command line."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `wawona-1.0.0/src/wawona/wawona.py` & `wawona-1.1.0/src/wawona/wawona.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import locale
 import os
 import re
+import sys
 from datetime import date, datetime, time, timedelta
 from os.path import isfile, isdir
 from time import sleep
 
 import inquirer
 import keyring
 import pytz
@@ -29,53 +30,71 @@
                   'Chrome/122.0.0.0 Safari/537.36'
 }
 KEYRING_EMAIL = "login.sequoia.com"
 KEYRING_TOKEN = "hrx-backend.sequoia.com"
 CHECK_MARK = "\u2705"
 CONFIG_VERSION = 1
 
+VERBOSE = False
+for arg in sys.argv:
+    if arg == "reset":
+        print("Removing config file")
+        os.remove(config_file)
+    elif arg == "--verbose":
+        VERBOSE = True
+
 
 class ApiException(Exception):
     pass
 
 
-def check(response):
+def api_call(method, url, **kwargs):
+    if VERBOSE:
+        print("API REQUEST: %s %s %s %s" % (method, url, kwargs.get("headers"), kwargs.get("json")))
+    response = requests.request(method, url, **kwargs)
     if response.status_code != 200:
-        raise ApiException("%s %s" % (response, response.json()))
+        raise ApiException("%s %s %s %s %s" % (method, url, kwargs.get("headers"), response, response.json()))
+    if VERBOSE:
+        print("API RESPONSE: %s %s" % (response, response.json()))
     return response
 
 
 def get_token(config, refresh=False):
     email = config["email"]
     token = keyring.get_password(KEYRING_TOKEN, email)
     if token and not refresh:
         return token
-    check(requests.post("https://hrx-backend.sequoia.com/idm/v1/contacts/verify-email", headers=HEADERS,
-                        json={"email": email}))
+    api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/v1/contacts/verify-email", headers=HEADERS,
+             json={"email": email})
     password = keyring.get_password(KEYRING_EMAIL, email)
     if not password:
         password = inquirer.password(message='Password')
-    response = check(requests.post("https://hrx-backend.sequoia.com/idm/users/login", headers=HEADERS,
-                                   json={"email": email, "password": password, "browserHash": BROWSER_HASH,
-                                         "userType": "employee"}))
+    response = api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/users/login", headers=HEADERS,
+                        json={"email": email, "password": password, "browserHash": BROWSER_HASH,
+                              "userType": "employee"})
     login_json = response.json()
     login_data = login_json["data"]
     user_details = login_data["userDetails"]
     token = user_details["apiToken"]
-    if user_details["oktaStatus"] == "MFA_CHALLENGE":
+    okta_status = user_details["oktaStatus"]
+    if okta_status == "MFA_CHALLENGE":
         factors = login_data.get("factors")
         if factors:
             factor = factors[0]
             print(
                 "Using MFA %s %s" % (factor.get("factorType", "unknown"), factor.get("profile", {}).get("phoneNumber")))
         mfa_code = inquirer.text(message="MFA Code")
         headers = {"apitoken": token}
         headers.update(HEADERS)
-        check(requests.post("https://hrx-backend.sequoia.com/idm/users/login/verify-mfa", headers=headers,
-                            json={"passCode": mfa_code, "browserHash": BROWSER_HASH}))
+        api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/users/login/verify-mfa", headers=headers,
+                 json={"passCode": mfa_code, "browserHash": BROWSER_HASH})
+    elif okta_status != "SUCCESS":
+        # https://developer.okta.com/docs/reference/api/authn/#transaction-state
+        raise ApiException("Invalid okta status %s: "
+                           "Please authenticate via https://px.sequoia.com/workplace before retrying." % okta_status)
     keyring.set_password(KEYRING_EMAIL, email, password)
     keyring.set_password(KEYRING_TOKEN, email, token)
     return token
 
 
 def get_config():
     config: dict[str, str] = {}
@@ -134,43 +153,48 @@
 def token_headers(token):
     headers = {"token": token}
     headers.update(HEADERS)
     return headers
 
 
 def get_locations(token):
-    response = check(
-        requests.get("https://hrx-backend.sequoia.com/rtw/resv/client/locations", headers=token_headers(token)))
+    response = api_call(
+        method='GET', url="https://hrx-backend.sequoia.com/rtw/resv/client/locations", headers=token_headers(token))
     return [(x["locationName"], x) for x in response.json()["data"]["locations"]]
 
 
 def format_date(dt):
     return "%02d-%02d-%d" % (dt.day, dt.month, dt.year)
 
 
 def parse_date(dt):
     day, month, year = dt.split("-")
     return date(int(year), int(month), int(day))
 
 
 def get_summary(token, start, end):
-    response = check(requests.get(
-        "https://hrx-backend.sequoia.com/rtw/client/dashboard/summary?statStart=%s&statEnd=%s" % (
-            format_date(start), format_date(end)), headers=token_headers(token)))
+    response = api_call(method='GET',
+                        url="https://hrx-backend.sequoia.com/rtw/client/dashboard/summary?statStart=%s&statEnd=%s" % (
+                            format_date(start), format_date(end)), headers=token_headers(token))
     out = set()
     for stat in response.json()["data"]["weeklyStats"]:
         out.add(parse_date(stat["date"]))
     return out
 
 
 def get_followings(token, start, end):
-    response = check(requests.get("https://hrx-backend.sequoia.com/rtw/client/followings?startDate=%s&endDate=%s" % (
-        format_date(start), format_date(end)), headers=token_headers(token)))
+    response = api_call(method='GET',
+                        url="https://hrx-backend.sequoia.com/rtw/client/followings?startDate=%s&endDate=%s" % (
+                            format_date(start), format_date(end)), headers=token_headers(token))
     out = []
-    for user in response.json()["data"]["followings"]:
+    followings = response.json()["data"]["followings"]
+    if not followings:
+        print("You are not following any coworkers.\n"
+              "Add them in https://px.sequoia.com/workplace or the app, and they will appear calendar below.")
+    for user in followings:
         name = user["fullName"]
         reservations = user.get("reservationsMetadata", [])
         days = set()
         if reservations:
             for reservation in reservations:
                 year, month, day = reservation["reservationStartTime"].split(" ")[0].split("-")
                 dt = date(int(year), int(month), int(day))
@@ -204,17 +228,18 @@
         if start < end:
             body['reservations'].append({
                 "startTimeUtc": pretty_time(start),
                 "endTimeUtc": pretty_time(end),
                 "isPrivate": False
             })
     if body['reservations']:
-        check(
-            requests.post("https://hrx-backend.sequoia.com/rtw/resv/client/reservations", headers=token_headers(token),
-                          json=body))
+        api_call(
+            method='POST', url="https://hrx-backend.sequoia.com/rtw/resv/client/reservations",
+            headers=token_headers(token),
+            json=body)
     return check_tasks
 
 
 def do_inquiry(message, choices, default=None):
     if len(choices) == 0:
         raise Exception("No choices")
     if len(choices) == 1:
@@ -232,72 +257,74 @@
     answers = inquirer.prompt(questions)
     if not answers:
         raise Exception("No choice")
     return answers['choice']
 
 
 def get_pending_tasks(token):
-    response = check(
-        requests.get("https://hrx-backend.sequoia.com/rtw/client/pending-task", headers=token_headers(token)))
+    response = api_call(method='GET', url="https://hrx-backend.sequoia.com/rtw/client/pending-task",
+                        headers=token_headers(token))
     return [x["taskId"] for x in response.json()["data"]["tasks"]]
 
 
 def get_task(token, task_id):
-    response = check(requests.get("https://hrx-backend.sequoia.com/rtw/client/task/info?taskId=%s" % task_id,
-                                  headers=token_headers(token)))
+    response = api_call(method='GET', url="https://hrx-backend.sequoia.com/rtw/client/task/info?taskId=%s" % task_id,
+                        headers=token_headers(token))
     return response.json()["data"]
 
 
 def respond_to_task(token, task_id, answers):
-    check(requests.post("https://hrx-backend.sequoia.com/rtw/client/task-response", headers=token_headers(token),
-                        json={"taskId": task_id, "response": answers}))
+    api_call(method='POST', url="https://hrx-backend.sequoia.com/rtw/client/task-response",
+             headers=token_headers(token),
+             json={"taskId": task_id, "response": answers})
 
 
 def get_floors(token, task_id):
-    response = check(
-        requests.get("https://hrx-backend.sequoia.com/rtw/client/space-bookings/floors?taskId=%s" % task_id,
-                     headers=token_headers(token)))
+    response = api_call(
+        method='GET', url="https://hrx-backend.sequoia.com/rtw/client/space-bookings/floors?taskId=%s" % task_id,
+        headers=token_headers(token))
     return [(x["floorName"], x["floorId"]) for x in response.json()["data"]["floors"] if x["status"] == "active"]
 
 
 def get_spaces(token, adjective, task_id, floor_id, start_time, end_time):
     url = ("https://hrx-backend.sequoia.com/rtw/client/space-bookings/%s/spaces?taskId=%s&floorId=%s&startTime=%s"
            "&endTime=%s") % (
               adjective, task_id, floor_id, start_time, end_time)
-    response = check(requests.get(url, headers=token_headers(token)))
+    response = api_call(method='GET', url=url, headers=token_headers(token))
     return response.json()["data"]["spaces"]
 
 
 def reserve_space(token, task_id, start_time, end_time, space_id, user_id, reservation_id):
-    response = check(
-        requests.post("https://hrx-backend.sequoia.com/rtw/client/space-bookings/space", headers=token_headers(token),
-                      json={"taskId": task_id, "startTime": start_time, "endTime": end_time, "spaceId": space_id,
-                            "userId": user_id, "reservationId": reservation_id}
-                      ))
+    response = api_call(method='POST', url="https://hrx-backend.sequoia.com/rtw/client/space-bookings/space",
+                        headers=token_headers(token),
+                        json={"taskId": task_id, "startTime": start_time, "endTime": end_time, "spaceId": space_id,
+                              "userId": user_id, "reservationId": reservation_id}
+                        )
     return response.json()["data"]["label"]
 
 
 def get_space(token, task, floor_id, config):
     task_id = task["taskId"]
     start_time = task["reservationStartTime"]
     end_time = task["reservationEndTime"]
     available_spaces = get_spaces(token, "available", task_id, floor_id, start_time, end_time)
-    preferred_space_id = inquirer.text(message="Preferred space ID (press return for none)",
-                                       default=config.get("preferred_space_id"))
+    default = None
+    preferred_space_id = config.get("preferred_space_id")
+    if not preferred_space_id:
+        preferred_space_id = inquirer.text(message="Preferred space ID (press return for none)")
     all_spaces = []
     available_space_set = set()
     for available_space in available_spaces:
         space_id = available_space["spaceId"]
         unique_space_id = available_space["uniqueSpaceId"]
         if space_id == preferred_space_id:
-            return unique_space_id
+            default = unique_space_id
         all_spaces.append(available_space)
         available_space_set.add(unique_space_id)
     booked_spaces = get_spaces(token, "booked", task_id, floor_id, start_time, end_time)
-    default = None
     for booked_space in booked_spaces:
         space_id = booked_space["spaceId"]
         if space_id == preferred_space_id:
             default = booked_space["uniqueSpaceId"]
         all_spaces.append(booked_space)
     all_spaces.sort(key=lambda s: [int(t) if t.isdigit() else t.lower() for t in re.split(r'(\d+)', s["label"])])
     choices = []
@@ -306,18 +333,18 @@
         first_name = space.get("firstName")
         if first_name:
             label = "\033[31m%s (%s %s)\033[0m" % (raw_label, first_name, space["lastName"])
         else:
             label = "\033[32m%s\033[0m" % raw_label
         choices.append((label, space["uniqueSpaceId"]))
     while True:
-        print("Preferred space is not available")
         unique_space_id = do_inquiry("Space", choices, default)
         if unique_space_id in available_space_set:
             return unique_space_id
+        print("Invalid selection")
 
 
 def run_tasks(token, config, pending_task_ids):
     for pending_task_id in pending_task_ids:
         task = get_task(token, pending_task_id)
         task_id = task["taskId"]
         task_metadata = task["taskMetadata"]
```

### Comparing `wawona-1.0.0/src/wawona.egg-info/PKG-INFO` & `wawona-1.1.0/src/wawona.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.0.0
+Version: 1.1.0
 Summary: Easily make office reservations in sequoia from the command line.
 Author-email: yuzawa-san <jtyuzawa@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
@@ -28,15 +28,15 @@
 by [@yuzawa-san](https://github.com/yuzawa-san/)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/wawona)](https://pypi.org/project/wawona/)
 
 Easily make office reservations in sequoia from the command line.
 This tool is provides streamlined workflows:
 
-- viewing the next two week's bookings from coworkers that you have followed
+- viewing the next two week's bookings from coworkers that you have followed (in the app/[site](https://px.sequoia.com/workplace))
 - booking multiple days at a time
 - doing space reservations (with the ability to save your preferred space)
 - if an option contains a single choice, automatically select that choice
 
 ```
 +----------------------+-----+-----+-----+-----+-----+
 | WEEK OF 11 MAR       | Mon | Tue | Wed | Thu | Fri |
@@ -78,16 +78,14 @@
   Mar 27 New York Reservation
   Complete Self-Screening
   Seat Not Selected
 
 [?] Complete task? (Y/n): 
 [?] I am healthy and not sick?: Yes (only choice)
 [?] Floor: Floor 2 (only choice)
-[?] Preferred space ID (press return for none): 
-Preferred space is not available
 [?] Space: 
    Desk 35
    Desk 36
    Desk 37
    Desk 38
    Desk 39
    Desk 40
@@ -127,20 +125,27 @@
 
 ## Usage 
 
 - Run it from your terminal: `wawona`
 - On initial run, you will be asked provide configuration: email and password.
 - You may be prompted to for an MFA token periodically.
 - Use the up/down arrows, spacebar, and return keys to select items in lists
+- Troubleshooting errors with `wawona --verbose`
 
 ### Reset
 
 If you need to reset to factory defaults (maybe if you changed your password), remove the configuration:
 
 ```console
+wawona reset
+```
+
+As a last resort, if all else fails:
+
+```console
 rm -rf ~/.config/wawona/
 ```
 
 ## Notes
 
 - Not affliated with sequoia
 - Uses public endpoints discovered from the web UI
```

