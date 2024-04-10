# Comparing `tmp/pyloobins-1.5.0.tar.gz` & `tmp/pyloobins-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloobins-1.5.0.tar", max compression
+gzip compressed data, was "pyloobins-1.6.0.tar", max compression
```

## Comparing `pyloobins-1.5.0.tar` & `pyloobins-1.6.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    35149 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LICENSE
--rw-r--r--   0        0        0      852 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/GetFileInfo.yml
--rw-r--r--   0        0        0     1402 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/SetFile.yml
--rw-r--r--   0        0        0     1382 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/caffeinate.yml
--rw-r--r--   0        0        0     1411 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/csrutil.yml
--rw-r--r--   0        0        0     1596 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/defaults.yml
--rw-r--r--   0        0        0     2467 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/ditto.yml
--rw-r--r--   0        0        0     1769 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/dns-sd.yml
--rw-r--r--   0        0        0     1088 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/dscacheutil.yml
--rw-r--r--   0        0        0     3538 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/dscl.yml
--rw-r--r--   0        0        0     1214 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/dsconfigad.yml
--rw-r--r--   0        0        0     1098 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/dsexport.yml
--rw-r--r--   0        0        0     2044 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/hdiutil.yml
--rw-r--r--   0        0        0     2117 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/ioreg.yml
--rw-r--r--   0        0        0      652 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/kextstat.yml
--rw-r--r--   0        0        0     1531 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/last.yml
--rw-r--r--   0        0        0     1207 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/launchctl.yml
--rw-r--r--   0        0        0     1118 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/log.yml
--rw-r--r--   0        0        0     1869 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/lsregister.yml
--rw-r--r--   0        0        0     1831 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/mdfind.yml
--rw-r--r--   0        0        0      961 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/mdls.yml
--rw-r--r--   0        0        0     1332 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/mktemp.yml
--rw-r--r--   0        0        0     4420 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/networksetup.yml
--rw-r--r--   0        0        0      754 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/nscurl.yml
--rw-r--r--   0        0        0      689 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/nvram.yml
--rw-r--r--   0        0        0     1379 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/odutil.yml
--rw-r--r--   0        0        0      939 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/open.yml
--rw-r--r--   0        0        0     1327 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/osacompile.yml
--rw-r--r--   0        0        0     3231 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/osascript.yml
--rw-r--r--   0        0        0     1263 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/pbpaste.yml
--rw-r--r--   0        0        0     1259 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/plutil.yml
--rw-r--r--   0        0        0     1249 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/profiles.yml
--rw-r--r--   0        0        0     1206 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/safaridriver.yml
--rw-r--r--   0        0        0     1267 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/say.yml
--rw-r--r--   0        0        0     1051 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/screencapture.yml
--rw-r--r--   0        0        0     1611 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/scutil.yml
--rw-r--r--   0        0        0     2458 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/security.yml
--rw-r--r--   0        0        0     1073 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/sfltool.yml
--rw-r--r--   0        0        0      864 2024-01-06 13:41:51.659552 pyloobins-1.5.0/LOOBins/softwareupdate.yml
--rw-r--r--   0        0        0     1114 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/spctl.yml
--rw-r--r--   0        0        0     2423 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/sqlite3.yml
--rw-r--r--   0        0        0     1139 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/ssh-keygen.yml
--rw-r--r--   0        0        0     1356 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/sw_vers.yml
--rw-r--r--   0        0        0     2366 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/swift.yml
--rw-r--r--   0        0        0      785 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/sysctl.yml
--rw-r--r--   0        0        0     1930 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/system_profiler.yml
--rw-r--r--   0        0        0     1339 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/systemsetup.yml
--rw-r--r--   0        0        0     1159 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/tclsh.yml
--rw-r--r--   0        0        0     1993 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/textutil.yml
--rw-r--r--   0        0        0     2021 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/tmutil.yml
--rw-r--r--   0        0        0     1587 2024-01-06 13:41:51.663552 pyloobins-1.5.0/LOOBins/xattr.yml
--rw-r--r--   0        0        0     2863 2024-01-06 13:41:51.663552 pyloobins-1.5.0/docs/pyloobins/README.md
--rw-r--r--   0        0        0     1222 2024-01-06 13:41:51.663552 pyloobins-1.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-06 13:41:51.663552 pyloobins-1.5.0/src/pyloobins/__init__.py
--rw-r--r--   0        0        0     2238 2024-01-06 13:41:51.663552 pyloobins-1.5.0/src/pyloobins/cli.py
--rw-r--r--   0        0        0     4092 2024-01-06 13:41:51.663552 pyloobins-1.5.0/src/pyloobins/models.py
--rw-r--r--   0        0        0     1311 2024-01-06 13:41:51.663552 pyloobins-1.5.0/src/pyloobins/templates/loobin.md.j2
--rw-r--r--   0        0        0     2779 2024-01-06 13:41:51.663552 pyloobins-1.5.0/src/pyloobins/util.py
--rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 pyloobins-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LICENSE
+-rw-r--r--   0        0        0      852 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/GetFileInfo.yml
+-rw-r--r--   0        0        0     1402 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/SetFile.yml
+-rw-r--r--   0        0        0     1382 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/caffeinate.yml
+-rw-r--r--   0        0        0     1411 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/csrutil.yml
+-rw-r--r--   0        0        0     1816 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/defaults.yml
+-rw-r--r--   0        0        0     2467 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/ditto.yml
+-rw-r--r--   0        0        0     1769 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/dns-sd.yml
+-rw-r--r--   0        0        0     1088 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/dscacheutil.yml
+-rw-r--r--   0        0        0     4647 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/dscl.yml
+-rw-r--r--   0        0        0     1214 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/dsconfigad.yml
+-rw-r--r--   0        0        0     1098 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/dsexport.yml
+-rw-r--r--   0        0        0     2044 2024-04-10 00:28:43.451856 pyloobins-1.6.0/LOOBins/hdiutil.yml
+-rw-r--r--   0        0        0     2232 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/ioreg.yml
+-rw-r--r--   0        0        0      652 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/kextstat.yml
+-rw-r--r--   0        0        0     1531 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/last.yml
+-rw-r--r--   0        0        0     1207 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/launchctl.yml
+-rw-r--r--   0        0        0     1118 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/log.yml
+-rw-r--r--   0        0        0     1869 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/lsregister.yml
+-rw-r--r--   0        0        0     1831 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/mdfind.yml
+-rw-r--r--   0        0        0      961 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/mdls.yml
+-rw-r--r--   0        0        0     1332 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/mktemp.yml
+-rw-r--r--   0        0        0     4420 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/networksetup.yml
+-rw-r--r--   0        0        0     1390 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/nscurl.yml
+-rw-r--r--   0        0        0      689 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/nvram.yml
+-rw-r--r--   0        0        0     1379 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/odutil.yml
+-rw-r--r--   0        0        0      939 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/open.yml
+-rw-r--r--   0        0        0     1327 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/osacompile.yml
+-rw-r--r--   0        0        0     3231 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/osascript.yml
+-rw-r--r--   0        0        0     1263 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/pbpaste.yml
+-rw-r--r--   0        0        0     1259 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/plutil.yml
+-rw-r--r--   0        0        0     1249 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/profiles.yml
+-rw-r--r--   0        0        0     1206 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/safaridriver.yml
+-rw-r--r--   0        0        0     1267 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/say.yml
+-rw-r--r--   0        0        0     1051 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/screencapture.yml
+-rw-r--r--   0        0        0     1611 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/scutil.yml
+-rw-r--r--   0        0        0     2458 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/security.yml
+-rw-r--r--   0        0        0     1073 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/sfltool.yml
+-rw-r--r--   0        0        0      864 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/softwareupdate.yml
+-rw-r--r--   0        0        0     1114 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/spctl.yml
+-rw-r--r--   0        0        0     2423 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/sqlite3.yml
+-rw-r--r--   0        0        0     1139 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/ssh-keygen.yml
+-rw-r--r--   0        0        0     1356 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/sw_vers.yml
+-rw-r--r--   0        0        0     2366 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/swift.yml
+-rw-r--r--   0        0        0      785 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/sysctl.yml
+-rw-r--r--   0        0        0     2065 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/system_profiler.yml
+-rw-r--r--   0        0        0     1339 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/systemsetup.yml
+-rw-r--r--   0        0        0     1159 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/tclsh.yml
+-rw-r--r--   0        0        0     1993 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/textutil.yml
+-rw-r--r--   0        0        0     2021 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/tmutil.yml
+-rw-r--r--   0        0        0     1587 2024-04-10 00:28:43.455856 pyloobins-1.6.0/LOOBins/xattr.yml
+-rw-r--r--   0        0        0     2863 2024-04-10 00:28:43.455856 pyloobins-1.6.0/docs/pyloobins/README.md
+-rw-r--r--   0        0        0     1228 2024-04-10 00:28:43.455856 pyloobins-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 00:28:43.455856 pyloobins-1.6.0/src/pyloobins/__init__.py
+-rw-r--r--   0        0        0     2238 2024-04-10 00:28:43.455856 pyloobins-1.6.0/src/pyloobins/cli.py
+-rw-r--r--   0        0        0     4092 2024-04-10 00:28:43.455856 pyloobins-1.6.0/src/pyloobins/models.py
+-rw-r--r--   0        0        0     1311 2024-04-10 00:28:43.455856 pyloobins-1.6.0/src/pyloobins/templates/loobin.md.j2
+-rw-r--r--   0        0        0     2779 2024-04-10 00:28:43.455856 pyloobins-1.6.0/src/pyloobins/util.py
+-rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 pyloobins-1.6.0/PKG-INFO
```

### Comparing `pyloobins-1.5.0/LICENSE` & `pyloobins-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/GetFileInfo.yml` & `pyloobins-1.6.0/LOOBins/GetFileInfo.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/SetFile.yml` & `pyloobins-1.6.0/LOOBins/SetFile.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/caffeinate.yml` & `pyloobins-1.6.0/LOOBins/caffeinate.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/csrutil.yml` & `pyloobins-1.6.0/LOOBins/csrutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/defaults.yml` & `pyloobins-1.6.0/LOOBins/defaults.yml`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,19 @@
   tactics:
   - Discovery
 - name: Add a login item to the current user
   description: An attacker can use defaults to add a login hook in attempt to gain persistence. This command requires root privileges.
   code: sudo defaults write /Library/Preferences/com.apple.loginwindow LoginHook gain_persistence.sh
   tactics:
   - Persistence
+- name: Get Active Directory user info from Jamf Connect
+  description: Retrieve Active Directory user info from Jamf Connect defaults configuration.
+  code: defaults read com.jamf.connect.state
+  tactics:
+  - Discovery
 paths:
 - /usr/bin/defaults
 detections:
 - name: No detections at time of publishing
   url: N/A
 resources:
 - name: "macOS defaults list: Uncomplete list of macOS defaults commands with demos"
```

### Comparing `pyloobins-1.5.0/LOOBins/ditto.yml` & `pyloobins-1.6.0/LOOBins/ditto.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/dns-sd.yml` & `pyloobins-1.6.0/LOOBins/dns-sd.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/dscacheutil.yml` & `pyloobins-1.6.0/LOOBins/dscacheutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/dsconfigad.yml` & `pyloobins-1.6.0/LOOBins/dsconfigad.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/dsexport.yml` & `pyloobins-1.6.0/LOOBins/dsexport.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/hdiutil.yml` & `pyloobins-1.6.0/LOOBins/hdiutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/ioreg.yml` & `pyloobins-1.6.0/LOOBins/ioreg.yml`

 * *Files 15% similar despite different names*

```diff
@@ -39,14 +39,14 @@
   - Collection
   tags:
   - oneliner
   - vmcheck
 paths:
 - /usr/sbin/ioreg
 detections:
-- name: No detections at time of publishing
-  url: N/A
+- name: System Information Discovery Using Ioreg
+  url: https://github.com/SigmaHQ/sigma/blob/master/rules/macos/process_creation/proc_creation_macos_ioreg_discovery.yml
 resources:
   - name: 'Evasions: macOS'
     url: https://evasions.checkpoint.com/techniques/macos.html
   - name: 'SwiftBelt-JXA Situational Awareness Tool'
     url: https://github.com/cedowens/SwiftBelt-JXA/blob/main/SwiftBelt-JXA.js#520
```

### Comparing `pyloobins-1.5.0/LOOBins/kextstat.yml` & `pyloobins-1.6.0/LOOBins/kextstat.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/last.yml` & `pyloobins-1.6.0/LOOBins/last.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/launchctl.yml` & `pyloobins-1.6.0/LOOBins/launchctl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/log.yml` & `pyloobins-1.6.0/LOOBins/log.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/lsregister.yml` & `pyloobins-1.6.0/LOOBins/lsregister.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/mdfind.yml` & `pyloobins-1.6.0/LOOBins/mdfind.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/mdls.yml` & `pyloobins-1.6.0/LOOBins/mdls.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/mktemp.yml` & `pyloobins-1.6.0/LOOBins/mktemp.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/networksetup.yml` & `pyloobins-1.6.0/LOOBins/networksetup.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/nscurl.yml` & `pyloobins-1.6.0/LOOBins/nscurl.yml`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,30 @@
 created: 2023-05-22
 example_use_cases:
   - name: Download file
     description: Download file and ignore cert checking 
     code: nscurl -k https://google.com -o /private/tmp/google
     tactics:
       - Defense Evasion
+      - Command and Control
+  - name: Download file
+    description: Download file to the Downloads directory using -dl 
+    code: nscurl https://google.com -dl
+    tactics:
+      - Defense Evasion
+      - Command and Control
+  - name: Download file
+    description: Download file to a designated directory using -dir 
+    code: nscurl https://google.com -dir /private/tmp/google
+    tactics:
+      - Defense Evasion
+      - Command and Control             
 paths:
   - /usr/bin/nscurl
 detections:
   - name: No detections at time of publishing
     url: N/A
 resources:
   - name: "How to Diagnose App Transport Security Issues using nscurl and OpenSSL"
     url: https://www.agnosticdev.com/content/how-diagnose-app-transport-security-issues-using-nscurl-and-openssl
+  - name: "Living-off-the-Land: Exploring macOS LOOBins and Crafting Detection Rules - nscurl"
+    url: https://danielcortez.substack.com/p/living-off-the-land-exploring-macos
```

### Comparing `pyloobins-1.5.0/LOOBins/nvram.yml` & `pyloobins-1.6.0/LOOBins/nvram.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/odutil.yml` & `pyloobins-1.6.0/LOOBins/odutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/open.yml` & `pyloobins-1.6.0/LOOBins/open.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/osacompile.yml` & `pyloobins-1.6.0/LOOBins/osacompile.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/osascript.yml` & `pyloobins-1.6.0/LOOBins/osascript.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/pbpaste.yml` & `pyloobins-1.6.0/LOOBins/pbpaste.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/plutil.yml` & `pyloobins-1.6.0/LOOBins/plutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/profiles.yml` & `pyloobins-1.6.0/LOOBins/profiles.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/safaridriver.yml` & `pyloobins-1.6.0/LOOBins/safaridriver.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/say.yml` & `pyloobins-1.6.0/LOOBins/say.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/screencapture.yml` & `pyloobins-1.6.0/LOOBins/screencapture.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/scutil.yml` & `pyloobins-1.6.0/LOOBins/scutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/security.yml` & `pyloobins-1.6.0/LOOBins/security.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/sfltool.yml` & `pyloobins-1.6.0/LOOBins/sfltool.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/softwareupdate.yml` & `pyloobins-1.6.0/LOOBins/softwareupdate.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/spctl.yml` & `pyloobins-1.6.0/LOOBins/spctl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/sqlite3.yml` & `pyloobins-1.6.0/LOOBins/sqlite3.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/ssh-keygen.yml` & `pyloobins-1.6.0/LOOBins/ssh-keygen.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/sw_vers.yml` & `pyloobins-1.6.0/LOOBins/sw_vers.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/swift.yml` & `pyloobins-1.6.0/LOOBins/swift.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/sysctl.yml` & `pyloobins-1.6.0/LOOBins/sysctl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/system_profiler.yml` & `pyloobins-1.6.0/LOOBins/system_profiler.yml`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,14 @@
       - Discovery
     tags:
       - bash
       - zsh
 paths:
   - /usr/sbin/system_profiler
 detections:
-  - name: No detections at time of publishing
-    url: N/A
+  - name: System Information Discovery Using System_Profiler
+    url: https://github.com/SigmaHQ/sigma/blob/master/rules/macos/process_creation/proc_creation_macos_system_profiler_discovery.yml
 resources:
   - name: "macOS/binaries/system_profiler"
     url: https://macosbin.com/bin/system_profiler
   - name: "system_profiler man page"
     url: https://ss64.com/osx/system_profiler.html
```

### Comparing `pyloobins-1.5.0/LOOBins/systemsetup.yml` & `pyloobins-1.6.0/LOOBins/systemsetup.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/tclsh.yml` & `pyloobins-1.6.0/LOOBins/tclsh.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/textutil.yml` & `pyloobins-1.6.0/LOOBins/textutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/tmutil.yml` & `pyloobins-1.6.0/LOOBins/tmutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/LOOBins/xattr.yml` & `pyloobins-1.6.0/LOOBins/xattr.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/docs/pyloobins/README.md` & `pyloobins-1.6.0/docs/pyloobins/README.md`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/pyproject.toml` & `pyloobins-1.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyLOOBins"
-version = "1.5.0"
+version = "1.6.0"
 description = "Python package for managing the LOOBins model and schema."
 authors = ["infosecB <brendan@infosecb.com>"]
 readme = "docs/pyloobins/README.md"
 packages = [{include = "pyloobins", from = "src"}]
 include = ["LOOBins/*.yml"]
 homepage = "https://loobins.io/"
 repository = "https://github.com/infosecB/LOOBins"
@@ -40,15 +40,15 @@
   'too-few-public-methods'
 ]
 
 [tool.tox]
 legacy_tox_ini = """
   [tox]
   env_list =
-      py38,py39,py310,py311
+      py38,py39,py310,py311,py312
   minversion = 4.5.1
 
   [testenv]
   description = run the tests with pytest
   package = wheel
   wheel_build_env = .pkg
   deps =
```

### Comparing `pyloobins-1.5.0/src/pyloobins/cli.py` & `pyloobins-1.6.0/src/pyloobins/cli.py`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/src/pyloobins/models.py` & `pyloobins-1.6.0/src/pyloobins/models.py`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/src/pyloobins/templates/loobin.md.j2` & `pyloobins-1.6.0/src/pyloobins/templates/loobin.md.j2`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/src/pyloobins/util.py` & `pyloobins-1.6.0/src/pyloobins/util.py`

 * *Files identical despite different names*

### Comparing `pyloobins-1.5.0/PKG-INFO` & `pyloobins-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLOOBins
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python package for managing the LOOBins model and schema.
 Home-page: https://loobins.io/
 License: GPL-3.0-or-later
 Keywords: cybersecurity,cli,lol
 Author: infosecB
 Author-email: brendan@infosecb.com
 Requires-Python: >=3.8,<4.0
```

