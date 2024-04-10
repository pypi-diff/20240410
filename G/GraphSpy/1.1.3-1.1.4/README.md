# Comparing `tmp/GraphSpy-1.1.3.tar.gz` & `tmp/GraphSpy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSpy-1.1.3.tar", last modified: Sun Apr  7 13:03:08 2024, max compression
+gzip compressed data, was "GraphSpy-1.1.4.tar", last modified: Wed Apr 10 06:45:16 2024, max compression
```

## Comparing `GraphSpy-1.1.3.tar` & `GraphSpy-1.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    41189 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/GraphSpy.py
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/__init__.py
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/static/
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/static/css/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      340 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/static/css/style.css
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/static/js/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    11164 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/static/js/functions.js
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     2430 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/static/js/theme.js
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy/templates/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7747 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/OneDrive.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     8554 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/SharePoint.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5757 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/SharePointDrives.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6379 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/SharePointSites.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5966 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/access_token_modal.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     9657 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/access_tokens.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17378 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/custom_requests.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5969 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/device_codes.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7933 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/generic_search.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      847 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/index.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17710 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/layout.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1923 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/outlook.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5094 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/recent_files.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5679 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/refresh_token_modal.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6820 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/refresh_tokens.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7886 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/settings.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5108 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/templates/shared_with_me.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)        5 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/GraphSpy/version.txt
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/GraphSpy.egg-info/
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     6914 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/PKG-INFO
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     1037 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/SOURCES.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)        1 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/dependency_links.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       52 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/entry_points.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       28 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/requires.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)        9 2024-04-07 13:03:08.000000 GraphSpy-1.1.3/GraphSpy.egg-info/top_level.txt
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1527 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/LICENSE.txt
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)       54 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/MANIFEST.in
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     6914 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/PKG-INFO
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6800 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/README.md
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)       28 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/requirements.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       38 2024-04-07 13:03:08.240714 GraphSpy-1.1.3/setup.cfg
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      916 2024-04-07 13:02:57.000000 GraphSpy-1.1.3/setup.py
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    41189 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/GraphSpy.py
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/__init__.py
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.163317 GraphSpy-1.1.4/GraphSpy/static/
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy/static/css/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      340 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/static/css/style.css
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy/static/js/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    11892 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/static/js/functions.js
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     2430 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/static/js/theme.js
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy/templates/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7747 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/OneDrive.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     8554 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/SharePoint.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5757 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/SharePointDrives.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6379 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/SharePointSites.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6336 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/access_token_modal.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     9996 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/access_tokens.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17378 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/custom_requests.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6512 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/device_codes.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7933 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/generic_search.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      847 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/index.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17710 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/layout.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1923 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/outlook.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5094 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/recent_files.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5679 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/refresh_token_modal.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6820 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/refresh_tokens.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7886 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/settings.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5108 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/shared_with_me.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)        5 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/version.txt
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy.egg-info/
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7098 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/PKG-INFO
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     1037 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/SOURCES.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)        1 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/dependency_links.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       52 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/entry_points.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       28 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/requires.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)        9 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/top_level.txt
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1527 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/LICENSE.txt
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)       54 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/MANIFEST.in
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7098 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/PKG-INFO
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6990 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/README.md
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)       28 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/requirements.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       38 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/setup.cfg
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      916 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/setup.py
```

### Comparing `GraphSpy-1.1.3/GraphSpy/GraphSpy.py` & `GraphSpy-1.1.4/GraphSpy/GraphSpy.py`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/static/js/functions.js` & `GraphSpy-1.1.4/GraphSpy/static/js/functions.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -110,15 +110,15 @@
         async: false,
         url: "/api/generate_device_code",
         data: {
             "resource": resource,
             "client_id": client_id
         }
     });
-    bootstrapToast("Device Code", `[Success] Generated Device Code with User Code '${response.responseText}'.`);
+    bootstrapToast("Device Code", `[Success] Generated Device Code with User Code '${response.responseText}'.`, "primary");
     reloadTables();
 }
 
 function restartDeviceCodePolling() {
     let response = $.ajax({
         type: "POST",
         async: false,
@@ -313,24 +313,36 @@
 // ========== Messages ==========
 
 function bootstrapAlert(message, type) {
     // Types: primary, secondary, success, danger, warning, info, light, dark
     var type_class = `alert-${type}`;
     var dom = $('<div>');
     dom.addClass("alert alert-dismissible");
-    dom.addClass(type_class);
+    validTypes = ["primary", "secondary", "success", "danger", "warning", "info", "light", "dark"]
+    if (type && validTypes.includes(type.toLowerCase())) {
+        dom.addClass(`alert-${type.toLowerCase()}`);
+    }
     dom.attr("role", "alert");
     dom.text(message);
     dom.append($('<button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>'));
     $('#alert_placeholder').append(dom);
 }
 
-function bootstrapToast(title, message) {
+function bootstrapToast(title, message, type = null, alternative = false) {
+    // Types: primary, secondary, success, danger, warning, info, light, dark
     // Wrapper for new Toast Message
     var toast_wrapper = $('<div class="toast" role="alert" aria-live="assertive" aria-atomic="true"></div>');
+    validTypes = ["primary", "secondary", "success", "danger", "warning", "info", "light", "dark"]
+    if (type && validTypes.includes(type.toLowerCase())) {
+        if (alternative) {
+            toast_wrapper.addClass(`bg-${type.toLowerCase()}-subtle`).addClass(`text-${type.toLowerCase()}-emphasis`);
+        } else {
+            toast_wrapper.addClass(`text-bg-${type.toLowerCase()}`);
+        }
+    }
     // Toast header
     var toast_header = $('<div class="toast-header"><small>Just now</small><button type="button" class="btn-close" data-bs-dismiss="toast" aria-label="Close"></button></div>');
     var toast_title = $('<strong class="me-auto"></strong>');
     toast_title.text(title);
     toast_header.prepend(toast_title);
     // Toast body
     var toast_body = $('<div class="toast-body"></div>');
```

### Comparing `GraphSpy-1.1.3/GraphSpy/static/js/theme.js` & `GraphSpy-1.1.4/GraphSpy/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/OneDrive.html` & `GraphSpy-1.1.4/GraphSpy/templates/OneDrive.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/SharePoint.html` & `GraphSpy-1.1.4/GraphSpy/templates/SharePoint.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/SharePointDrives.html` & `GraphSpy-1.1.4/GraphSpy/templates/SharePointDrives.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/SharePointSites.html` & `GraphSpy-1.1.4/GraphSpy/templates/SharePointSites.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/access_token_modal.html` & `GraphSpy-1.1.4/GraphSpy/templates/access_token_modal.html`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,23 @@
             { data: 'issued_at', 'width': '150px' },
             { data: 'expires_at', 'width': '150px' },
             { data: 'user', 'width': '350px' },
             { data: 'resource', 'width': '350px' },
             { data: 'description' }
         ],
         order: [[4, 'desc']],
-        autoWidth: false
+        autoWidth: false,
+        order: [[4, 'desc']],
+        createdRow: function (row, data, dataIndex) {
+            if (new Date(data.expires_at) > new Date()) {
+                $(row).addClass('bg-success-subtle').addClass('text-success-emphasis');
+            } else {
+                $(row).addClass('bg-danger-subtle').addClass('text-danger-emphasis');
+            }
+        }
     })
 
     accessTokenModalTable.on('click', 'td.dt-control', function (e) {
         let tr = e.target.closest('tr');
         let row = accessTokenModalTable.row(tr);
 
         if (row.child.isShown()) {
```

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/access_tokens.html` & `GraphSpy-1.1.4/GraphSpy/templates/access_tokens.html`

 * *Files 9% similar despite different names*

```diff
@@ -151,15 +151,22 @@
             { data: 'id', 'width': '30px' },
             { data: 'issued_at', 'width': '150px' },
             { data: 'expires_at', 'width': '150px' },
             { data: 'user', 'width': '350px' },
             { data: 'resource', 'width': '350px' },
             { data: 'description' }
         ],
-        order: [[4, 'desc']]
+        order: [[4, 'desc']],
+        createdRow: function (row, data, dataIndex) {
+            if (new Date(data.expires_at) > new Date()) {
+                $(row).addClass('bg-success-subtle').addClass('text-success-emphasis');
+            } else {
+                $(row).addClass('bg-danger-subtle').addClass('text-danger-emphasis');
+            }
+        }
     })
 
     myTable.on('click', 'td.dt-control', function (e) {
         let tr = e.target.closest('tr');
         let row = myTable.row(tr);
 
         if (row.child.isShown()) {
```

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/custom_requests.html` & `GraphSpy-1.1.4/GraphSpy/templates/custom_requests.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/device_codes.html` & `GraphSpy-1.1.4/GraphSpy/templates/device_codes.html`

 * *Files 10% similar despite different names*

```diff
@@ -89,15 +89,27 @@
             { data: 'generated_at', 'width': '150px' },
             { data: 'expires_at', 'width': '150px' },
             { data: 'last_poll', 'width': '150px' },
             { data: 'user_code', 'width': '125px' },
             { data: 'client_id', 'width': '310px' },
             { data: 'status' }
         ],
-        order: [[3, 'desc']]
+        order: [[3, 'desc']],
+        createdRow: function (row, data, dataIndex) {
+            switch (data.status) {
+                case "SUCCESS":
+                    $(row).addClass('bg-success-subtle').addClass('text-success-emphasis');
+                    break;
+                case "EXPIRED":
+                    $(row).addClass('bg-danger-subtle').addClass('text-danger-emphasis');
+                    break;
+                default:
+                    $(row).addClass('bg-primary-subtle').addClass('text-primary-emphasis');
+            }
+        }
     })
 
     myTable.on('click', 'td.dt-control', function (e) {
         let tr = e.target.closest('tr');
         let row = myTable.row(tr);
 
         if (row.child.isShown()) {
```

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/generic_search.html` & `GraphSpy-1.1.4/GraphSpy/templates/generic_search.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/index.html` & `GraphSpy-1.1.4/GraphSpy/templates/index.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/layout.html` & `GraphSpy-1.1.4/GraphSpy/templates/layout.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/outlook.html` & `GraphSpy-1.1.4/GraphSpy/templates/outlook.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/recent_files.html` & `GraphSpy-1.1.4/GraphSpy/templates/recent_files.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/refresh_token_modal.html` & `GraphSpy-1.1.4/GraphSpy/templates/refresh_token_modal.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/refresh_tokens.html` & `GraphSpy-1.1.4/GraphSpy/templates/refresh_tokens.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/settings.html` & `GraphSpy-1.1.4/GraphSpy/templates/settings.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy/templates/shared_with_me.html` & `GraphSpy-1.1.4/GraphSpy/templates/shared_with_me.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/GraphSpy.egg-info/PKG-INFO` & `GraphSpy-1.1.4/GraphSpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: Initial Access and Post-Exploitation Tool for AAD and O365 with a browser-based GUI
 Home-page: https://github.com/RedByte1337/GraphSpy
 Author: RedByte1337
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GraphSpy
@@ -23,15 +23,17 @@
 # Table of Contents
 
 - [GraphSpy](#graphspy)
 - [Table of Contents](#table-of-contents)
 - [Quick Start](#quick-start)
 	- [Installation](#installation)
 	- [Execution](#execution)
+	- [Usage](#usage)
 - [Features](#features)
+- [Release Notes](#release-notes)
 - [Upcoming Features](#upcoming-features)
 - [Credits](#credits)
 
 # Quick Start
 
 ## Installation
 
@@ -71,15 +73,15 @@
 graphspy -i 0.0.0.0 -p 8080
 ```
 
 For detailed instructions and other command line arguments, please refer to the [Execution page](https://github.com/RedByte1337/GraphSpy/wiki/Execution) on the wiki.
 
 ## Usage
 
-Please refer to the [Github Wiki](https://github.com/RedByte1337/GraphSpy/wiki) for full usage details.
+Please refer to the [GitHub Wiki](https://github.com/RedByte1337/GraphSpy/wiki) for full usage details.
 
 For a quick feature overview, check out the [official release blog post](https://insights.spotit.be/2024/04/05/graphspy-the-swiss-army-knife-for-attacking-m365-entra/).
 
 # Features
 
 ## Access and Refresh Tokens
 
@@ -143,14 +145,18 @@
 
 ![Graph Request](images/settings.png)
 
 ## Dark Mode
 
 Use the dark mode by default, or switch to light mode.
 
+# Release Notes
+
+Refer to the [Release Notes](https://github.com/RedByte1337/GraphSpy/wiki/Release-Notes) page on the GitHub Wiki
+
 # Upcoming Features
 
 * Upload, Delete and Rename Files
 * More authentication options
 	* Password, ESTSAuth Cookie, PRT, ...
 * Advanced token customization options and optional v2 API support (CAE)
 * Automatic Access Token Refreshing
```

### Comparing `GraphSpy-1.1.3/GraphSpy.egg-info/SOURCES.txt` & `GraphSpy-1.1.4/GraphSpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/LICENSE.txt` & `GraphSpy-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.3/PKG-INFO` & `GraphSpy-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: Initial Access and Post-Exploitation Tool for AAD and O365 with a browser-based GUI
 Home-page: https://github.com/RedByte1337/GraphSpy
 Author: RedByte1337
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GraphSpy
@@ -23,15 +23,17 @@
 # Table of Contents
 
 - [GraphSpy](#graphspy)
 - [Table of Contents](#table-of-contents)
 - [Quick Start](#quick-start)
 	- [Installation](#installation)
 	- [Execution](#execution)
+	- [Usage](#usage)
 - [Features](#features)
+- [Release Notes](#release-notes)
 - [Upcoming Features](#upcoming-features)
 - [Credits](#credits)
 
 # Quick Start
 
 ## Installation
 
@@ -71,15 +73,15 @@
 graphspy -i 0.0.0.0 -p 8080
 ```
 
 For detailed instructions and other command line arguments, please refer to the [Execution page](https://github.com/RedByte1337/GraphSpy/wiki/Execution) on the wiki.
 
 ## Usage
 
-Please refer to the [Github Wiki](https://github.com/RedByte1337/GraphSpy/wiki) for full usage details.
+Please refer to the [GitHub Wiki](https://github.com/RedByte1337/GraphSpy/wiki) for full usage details.
 
 For a quick feature overview, check out the [official release blog post](https://insights.spotit.be/2024/04/05/graphspy-the-swiss-army-knife-for-attacking-m365-entra/).
 
 # Features
 
 ## Access and Refresh Tokens
 
@@ -143,14 +145,18 @@
 
 ![Graph Request](images/settings.png)
 
 ## Dark Mode
 
 Use the dark mode by default, or switch to light mode.
 
+# Release Notes
+
+Refer to the [Release Notes](https://github.com/RedByte1337/GraphSpy/wiki/Release-Notes) page on the GitHub Wiki
+
 # Upcoming Features
 
 * Upload, Delete and Rename Files
 * More authentication options
 	* Password, ESTSAuth Cookie, PRT, ...
 * Advanced token customization options and optional v2 API support (CAE)
 * Automatic Access Token Refreshing
```

### Comparing `GraphSpy-1.1.3/README.md` & `GraphSpy-1.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 # Table of Contents
 
 - [GraphSpy](#graphspy)
 - [Table of Contents](#table-of-contents)
 - [Quick Start](#quick-start)
 	- [Installation](#installation)
 	- [Execution](#execution)
+	- [Usage](#usage)
 - [Features](#features)
+- [Release Notes](#release-notes)
 - [Upcoming Features](#upcoming-features)
 - [Credits](#credits)
 
 # Quick Start
 
 ## Installation
 
@@ -62,15 +64,15 @@
 graphspy -i 0.0.0.0 -p 8080
 ```
 
 For detailed instructions and other command line arguments, please refer to the [Execution page](https://github.com/RedByte1337/GraphSpy/wiki/Execution) on the wiki.
 
 ## Usage
 
-Please refer to the [Github Wiki](https://github.com/RedByte1337/GraphSpy/wiki) for full usage details.
+Please refer to the [GitHub Wiki](https://github.com/RedByte1337/GraphSpy/wiki) for full usage details.
 
 For a quick feature overview, check out the [official release blog post](https://insights.spotit.be/2024/04/05/graphspy-the-swiss-army-knife-for-attacking-m365-entra/).
 
 # Features
 
 ## Access and Refresh Tokens
 
@@ -134,14 +136,18 @@
 
 ![Graph Request](images/settings.png)
 
 ## Dark Mode
 
 Use the dark mode by default, or switch to light mode.
 
+# Release Notes
+
+Refer to the [Release Notes](https://github.com/RedByte1337/GraphSpy/wiki/Release-Notes) page on the GitHub Wiki
+
 # Upcoming Features
 
 * Upload, Delete and Rename Files
 * More authentication options
 	* Password, ESTSAuth Cookie, PRT, ...
 * Advanced token customization options and optional v2 API support (CAE)
 * Automatic Access Token Refreshing
```

### Comparing `GraphSpy-1.1.3/setup.py` & `GraphSpy-1.1.4/setup.py`

 * *Files identical despite different names*

