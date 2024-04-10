# Comparing `tmp/fortiedr-3.5.tar.gz` & `tmp/fortiedr-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortiedr-3.5.tar", last modified: Wed Apr  3 22:19:01 2024, max compression
+gzip compressed data, was "fortiedr-3.6.tar", last modified: Wed Apr 10 20:53:15 2024, max compression
```

## Comparing `fortiedr-3.5.tar` & `fortiedr-3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-03 22:19:01.054580 fortiedr-3.5/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1070 2024-03-26 20:15:27.000000 fortiedr-3.5/LICENSE
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       24 2024-04-03 22:14:23.000000 fortiedr-3.5/MANIFEST.in
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2728 2024-04-03 22:19:01.054580 fortiedr-3.5/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     2117 2024-04-03 22:14:23.000000 fortiedr-3.5/README.md
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-03 22:19:01.050580 fortiedr-3.5/fortiedr/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      930 2024-04-03 22:14:23.000000 fortiedr-3.5/fortiedr/__init__.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1633 2024-04-03 22:14:23.000000 fortiedr-3.5/fortiedr/auth.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     4311 2024-04-03 22:14:23.000000 fortiedr-3.5/fortiedr/connector.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)   236357 2024-04-03 22:14:23.000000 fortiedr-3.5/fortiedr/fortiedr.py
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-03 22:19:01.054580 fortiedr-3.5/fortiedr.egg-info/
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2728 2024-04-03 22:19:01.000000 fortiedr-3.5/fortiedr.egg-info/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      279 2024-04-03 22:19:01.000000 fortiedr-3.5/fortiedr.egg-info/SOURCES.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-04-03 22:19:01.000000 fortiedr-3.5/fortiedr.egg-info/dependency_links.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        9 2024-04-03 22:19:01.000000 fortiedr-3.5/fortiedr.egg-info/top_level.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      571 2024-04-03 22:18:48.000000 fortiedr-3.5/pyproject.toml
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       36 2024-03-28 19:25:38.000000 fortiedr-3.5/requirements.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2024-04-03 22:19:01.054580 fortiedr-3.5/setup.cfg
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      878 2024-04-03 22:14:23.000000 fortiedr-3.5/setup.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-10 20:53:15.415654 fortiedr-3.6/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1070 2024-04-10 20:52:30.000000 fortiedr-3.6/LICENSE
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       61 2024-04-10 20:52:30.000000 fortiedr-3.6/MANIFEST.in
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2728 2024-04-10 20:53:15.415654 fortiedr-3.6/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     2117 2024-04-10 20:52:30.000000 fortiedr-3.6/README.md
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-10 20:53:15.411654 fortiedr-3.6/fortiedr/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      930 2024-04-10 20:52:30.000000 fortiedr-3.6/fortiedr/__init__.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1633 2024-04-10 20:52:30.000000 fortiedr-3.6/fortiedr/auth.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     4311 2024-04-10 20:52:30.000000 fortiedr-3.6/fortiedr/connector.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)   236327 2024-04-10 20:52:30.000000 fortiedr-3.6/fortiedr/fortiedr.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-04-10 20:53:15.411654 fortiedr-3.6/fortiedr.egg-info/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2728 2024-04-10 20:53:15.000000 fortiedr-3.6/fortiedr.egg-info/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      279 2024-04-10 20:53:15.000000 fortiedr-3.6/fortiedr.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-04-10 20:53:15.000000 fortiedr-3.6/fortiedr.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        9 2024-04-10 20:53:15.000000 fortiedr-3.6/fortiedr.egg-info/top_level.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      570 2024-04-10 20:52:30.000000 fortiedr-3.6/pyproject.toml
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       36 2024-04-10 20:52:30.000000 fortiedr-3.6/requirements.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2024-04-10 20:53:15.415654 fortiedr-3.6/setup.cfg
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      876 2024-04-10 20:52:30.000000 fortiedr-3.6/setup.py
```

### Comparing `fortiedr-3.5/LICENSE` & `fortiedr-3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fortiedr-3.5/PKG-INFO` & `fortiedr-3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.5
+Version: 3.6
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.5/README.md` & `fortiedr-3.6/README.md`

 * *Files identical despite different names*

### Comparing `fortiedr-3.5/fortiedr/__init__.py` & `fortiedr-3.6/fortiedr/__init__.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.5/fortiedr/auth.py` & `fortiedr-3.6/fortiedr/auth.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.5/fortiedr/connector.py` & `fortiedr-3.6/fortiedr/connector.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.5/fortiedr/fortiedr.py` & `fortiedr-3.6/fortiedr/fortiedr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 
 import os
 import json
 from typing import BinaryIO
 from fortiedr.auth import Auth as fedrAuth
 from fortiedr.connector import FortiEDR_API_GW
 
+version = 3.6
+
 fortiedr_connection = None
 
 class ApplicationControl:
 	'''Application Control Rest Api Controller'''
 
-	def get_applications(self, currentPage: int, organization: str, fileName: str = None, path: str = None, signer: str = None, enabled: bool = None, hash: str = None, operatingSystem: str = None, policyIds: dict = None, tag: str = None) -> tuple[bool, None]:
+	def get_applications(self, currentPage: int, organization: str, fileName: str = None, path: str = None, signer: str = None, enabled: bool = None, hash: str = None, operatingSystem: str = None, policyIds: list = None, tag: str = None) -> tuple[bool, None]:
 		'''
 		Class ApplicationControl
 		Description: Get application controls.
         
 		Args:
 			fileName (str): Specifies the file name, if contains special characters - encode to HTML URL Encoding.
 			attributes.fileName (str): Specifies the file name, if contains special characters - encode to HTML URL Encoding.
@@ -23,15 +25,15 @@
 			signer (str): Specifies the value, if contains special characters - encode to HTML URL Encoding.
 			attributes.signer (str): Specifies the value, if contains special characters - encode to HTML URL Encoding.
 			currentPage (int): Specifies the current page.
 			enabled (bool): Specifies the state of the application control.
 			hash (str): Specifies the hash of the application control.
 			operatingSystem (str): Specifies the operating system of the application control.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
-			policyIds (dict): Specifies the IDs of the relevant policies for application control.
+			policyIds (list): Specifies the IDs of the relevant policies for application control.
 			tag (str): Specifies the tag related to application control.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("get_applications", locals())
@@ -57,15 +59,15 @@
 		if policyIds:
 			url_params.append('policyIds=' + policyIds)
 		if tag:
 			url_params.append('tag=' + tag)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def send_applications(self, applicationControls: dict = None, organization: str = None) -> tuple[bool, None]:
+	def send_applications(self, applicationControls: list = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class ApplicationControl
 		Description: Saves new application controls and returns a list of them.
         
 		Args:
 			applicationControlSaveRequest (Object): Check 'applicationControlSaveRequest' in the API documentation for further information.
 
@@ -79,21 +81,21 @@
 
 		applicationControlSaveRequest = {
 			"applicationControls": applicationControls,
 			"organization": organization,
 		}
 		return fortiedr_connection.send(url, applicationControlSaveRequest)
 
-	def insert_applications(self, appIds: dict, organization: str, enabled: bool = None, groupIds: dict = None, isOverridePolicies: bool = None, policyIds: dict = None, tagId: int = None) -> tuple[bool, list]:
+	def insert_applications(self, appIds: list, organization: str, enabled: bool = None, groupIds: list = None, isOverridePolicies: bool = None, policyIds: list = None, tagId: int = None) -> tuple[bool, list]:
 		'''
 		Class ApplicationControl
 		Description: Edits existing application control and returns the affected ones.
         
 		Args:
-			appIds (dict): The relevant application IDs to edit.
+			appIds (list): The relevant application IDs to edit.
 			modifiedFields (Object): Check 'modifiedFields' in the API documentation for further information.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
@@ -112,21 +114,21 @@
 			"groupIds": groupIds,
 			"isOverridePolicies": isOverridePolicies,
 			"policyIds": policyIds,
 			"tagId": str(tagId),
 		}
 		return fortiedr_connection.insert(url, modifiedFields)
 
-	def delete_applications(self, organization: str, applicationIds: dict = None) -> tuple[bool, None]:
+	def delete_applications(self, organization: str, applicationIds: list = None) -> tuple[bool, None]:
 		'''
 		Class ApplicationControl
 		Description: Deletes application controls.
         
 		Args:
-			applicationIds (dict): The IDs of the applications to be deleted.
+			applicationIds (list): The IDs of the applications to be deleted.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_applications", locals())
@@ -236,15 +238,15 @@
 		return fortiedr_connection.get(url)
 
 class Administrator:
 	'''The Administrator module enables administrators to perform administrative operations, such as handling licenses and users.'''
 
 	def set_tray_notification_settings(self, enabledPopup: bool = None, enabledTrayNotification: bool = None, message: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		Class Administrator
+		Class Admin
 		Description: Update tray notification settings.
         
 		Args:
 			adminSetTrayNotificationSettingsRequest (Object): Check 'adminSetTrayNotificationSettingsRequest' in the API documentation for further information.
 
 		Returns:
 			bool: Status of the request (True or False). 
@@ -417,22 +419,22 @@
 		if mode:
 			url_params.append('mode=' + mode)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-	def update_collector_installer(self, collectorGroupIds: dict = None, collectorGroups: dict = None, organization: str = None, updateVersions: dict = None) -> tuple[bool, None]:
+	def update_collector_installer(self, collectorGroupIds: list = None, collectorGroups: list = None, organization: str = None, updateVersions: list = None) -> tuple[bool, None]:
 		'''
 		Class Administrator
 		Description: This API update collectors target version for collector groups.
         
 		Args:
-			collectorGroupIds (dict): Specifies the list of IDs of all the collector groups which should be updated..
-			collectorGroups (dict): Specifies the list of all the collector groups which should be updated..
+			collectorGroupIds (list): Specifies the list of IDs of all the collector groups which should be updated..
+			collectorGroups (list): Specifies the list of all the collector groups which should be updated..
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			requestUpdateData (Object): Check 'requestUpdateData' in the API documentation for further information.
 
 		Returns:
 			bool: Status of the request (True or False). 
@@ -468,15 +470,15 @@
 			str
 		'''
 		validate_params("upload_content", locals())
 
 		url = '/management-rest/admin/upload-content'
 		if file:
 			file = {'file': file}
-		return fortiedr_connection.upload(url, file, request_type="multipart/form-data")
+		return fortiedr_connection.upload(url, file)
 
 	def upload_license(self, licenseBlob: str = None) -> tuple[bool, None]:
 		'''
 		Class Administrator
 		Description: Upload license to the system.
         
 		Args:
@@ -526,21 +528,21 @@
 			url_params.append('toTime=' + toTime)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
 class CommunicationControl:
 	'''Fortinet Endpoint Protection and Response Platform’s Communication Control module is responsible for monitoring and handling non-disguised security events. The module uses a set of policies that contain recommendations about whether an application should be approved or denied from communicating outside your organization.'''
 
-	def assign_collector_group(self, collectorGroups: dict, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
+	def assign_collector_group(self, collectorGroups: list, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class CommunicationControl
 		Description: Assign collector group to application policy.
         
 		Args:
-			collectorGroups (dict):  Specifies the collector groups whose collector reported the events.
+			collectorGroups (list):  Specifies the collector groups whose collector reported the events.
 			forceAssign (bool): Indicates whether to force the assignment even if the group is assigned to similar policies.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			policyName (str): Specifies the list of policies.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -581,30 +583,30 @@
 		if newPolicyName:
 			url_params.append('newPolicyName=' + newPolicyName)
 		if organization:
 			url_params.append('organization=' + organization)
 		if sourcePolicyName:
 			url_params.append('sourcePolicyName=' + sourcePolicyName)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url)
+		return fortiedr_connection.send(url)
 
-	def list_policies(self, decisions: dict, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, policies: dict = None, rules: dict = None, sorting: str = None, sources: dict = None, state: str = None, strictMode: bool = None) -> tuple[bool, list]:
+	def list_policies(self, decisions: list, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, policies: list = None, rules: list = None, sorting: str = None, sources: list = None, state: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
 		Class CommunicationControl
 		Description: This API call outputs a list of all the communication control policies in the system, and information about each of them.
         
 		Args:
-			decisions (dict): Indicates the action.
+			decisions (list): Indicates the action.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			pageNumber (int): An integer used for paging that indicates the required page number.
-			policies (dict): Specifies the list of policy names.
-			rules (dict): Specifies the list of rules.
+			policies (list): Specifies the list of policy names.
+			rules (list): Specifies the list of rules.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
-			sources (dict): Specifies who created the policy.
+			sources (list): Specifies who created the policy.
 			state (str): Policy rule state.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
@@ -631,52 +633,52 @@
 		if state:
 			url_params.append('state=' + state)
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def list_products(self, action: str = None, collectorGroups: dict = None, cveIdentifier: str = None, destinationIp: dict = None, devices: dict = None, firstConnectionTimeEnd: str = None, firstConnectionTimeStart: str = None, handled: bool = None, includeStatistics: bool = None, ips: dict = None, itemsPerPage: int = None, lastConnectionTimeEnd: str = None, lastConnectionTimeStart: str = None, organization: str = None, os: dict = None, pageNumber: int = None, policies: dict = None, processHash: str = None, processes: dict = None, product: str = None, products: dict = None, reputation: dict = None, rule: str = None, rulePolicy: str = None, seen: bool = None, sorting: str = None, strictMode: bool = None, vendor: str = None, vendors: dict = None, version: str = None, versions: dict = None, vulnerabilities: dict = None) -> tuple[bool, list]:
+	def list_products(self, action: str = None, collectorGroups: list = None, cveIdentifier: str = None, destinationIp: list = None, devices: list = None, firstConnectionTimeEnd: str = None, firstConnectionTimeStart: str = None, handled: bool = None, includeStatistics: bool = None, ips: list = None, itemsPerPage: int = None, lastConnectionTimeEnd: str = None, lastConnectionTimeStart: str = None, organization: str = None, os: list = None, pageNumber: int = None, policies: list = None, processHash: str = None, processes: list = None, product: str = None, products: list = None, reputation: list = None, rule: str = None, rulePolicy: str = None, seen: bool = None, sorting: str = None, strictMode: bool = None, vendor: str = None, vendors: list = None, version: str = None, versions: list = None, vulnerabilities: list = None) -> tuple[bool, list]:
 		'''
 		Class CommunicationControl
 		Description: This API call outputs a list of all the communicating applications in the system, and information about each of them.
         
 		Args:
 			action (str): Indicates the action: Allow/Deny. This parameter is irrelevant without policies parameter.
-			collectorGroups (dict): Specifies the list of collector groups where the products were seen.
+			collectorGroups (list): Specifies the list of collector groups where the products were seen.
 			cveIdentifier (str): Specifies the CVE identifier.
-			destinationIp (dict): Destination IPs.
-			devices (dict): Specifies the list of device names where the products were seen.
+			destinationIp (list): Destination IPs.
+			devices (list): Specifies the list of device names where the products were seen.
 			firstConnectionTimeEnd (str):  Retrieves products whose first connection time is less than the value assigned to this date.
 			firstConnectionTimeStart (str):  Retrieves products whose first connection time is greater than the value assigned to this date.
 			handled (bool): A true/false parameter indicating whether events were handled/unhandled.
 			includeStatistics (bool): A true/false parameter indicating including statistics data.
-			ips (dict): Specifies the list of IPs where the products were seen.
+			ips (list): Specifies the list of IPs where the products were seen.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastConnectionTimeEnd (str):  Retrieves products whose last connection time is less than the value assigned to this date.
 			lastConnectionTimeStart (str):  Retrieves products whose last connection time is greater than the value assigned to this date.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
-			os (dict): Specifies the list of operating system families where the products were seen.
+			os (list): Specifies the list of operating system families where the products were seen.
 			pageNumber (int): An integer used for paging that indicates the required page number.
-			policies (dict): Specifies the list of policy names whose products have a specific decision, as specified in the action parameter.
+			policies (list): Specifies the list of policy names whose products have a specific decision, as specified in the action parameter.
 			processHash (str): Specifies the process hash name.
-			processes (dict): Specifies the list of process names running alongside the products.
+			processes (list): Specifies the list of process names running alongside the products.
 			product (str): Specifies a single value for the product name. By default, strictMode is false.
-			products (dict): Specifies the list of product names. Names must match exactly (strictMode is always true).
-			reputation (dict): Specifies the recommendation of the application: Unknown, Known bad, Assumed bad, Contradiction, Assumed good or Known good.
+			products (list): Specifies the list of product names. Names must match exactly (strictMode is always true).
+			reputation (list): Specifies the recommendation of the application: Unknown, Known bad, Assumed bad, Contradiction, Assumed good or Known good.
 			rule (str): Indicates the rule. This parameter is irrelevant without rulePolicy parameter.
 			rulePolicy (str): Specifies the policy name whose products have a specific rule, as specified in the rule parameter.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			vendor (str): Specifies a single value for the vendor name. By default, strictMode is false.
-			vendors (dict): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
+			vendors (list): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
 			version (str): Specifies a single value for the version name. By default, strictMode is false.
-			versions (dict): Specifies the list of versions. Names must match exactly (strictMode is always true).
-			vulnerabilities (dict): Specifies the list of vulnerabilities where the products were seen.
+			versions (list): Specifies the list of versions. Names must match exactly (strictMode is always true).
+			vulnerabilities (list): Specifies the list of vulnerabilities where the products were seen.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_products", locals())
 
@@ -745,28 +747,28 @@
 		if versions:
 			url_params.append('versions=' + versions)
 		if vulnerabilities:
 			url_params.append('vulnerabilities=' + vulnerabilities)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def resolve_applications(self, applyNested: bool = None, comment: str = None, organization: str = None, products: dict = None, resolve: bool = None, signed: bool = None, vendors: dict = None, versions: dict = None) -> tuple[bool, None]:
+	def resolve_applications(self, applyNested: bool = None, comment: str = None, organization: str = None, products: list = None, resolve: bool = None, signed: bool = None, vendors: list = None, versions: list = None) -> tuple[bool, None]:
 		'''
 		Class CommunicationControl
 		Description: Enable resolving/unresolving applications.
         
 		Args:
 			applyNested (bool): A true/false parameter indicating updating inherited.
 			comment (str): Specifies a user-defined string to attach to the policy.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
-			products (dict): Specifies the list of product names. Names must match exactly (strictMode is always true).
+			products (list): Specifies the list of product names. Names must match exactly (strictMode is always true).
 			resolve (bool): A true/false parameter indicating update the application resolve/unresolve.
 			signed (bool): A true/false parameter indicating if the policy is signed.
-			vendors (dict): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
-			versions (dict): Specifies the list of versions. Names must match exactly (strictMode is always true).
+			vendors (list): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
+			versions (list): Specifies the list of versions. Names must match exactly (strictMode is always true).
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("resolve_applications", locals())
 
@@ -787,23 +789,23 @@
 		if vendors:
 			url_params.append('vendors=' + vendors)
 		if versions:
 			url_params.append('versions=' + versions)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-	def set_policy_mode(self, mode: str, policyNames: dict, organization: str = None) -> tuple[bool, None]:
+	def set_policy_mode(self, mode: str, policyNames: list, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class CommunicationControl
 		Description: Set policy to simulation/prevention.
         
 		Args:
 			mode (str): Operation mode.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
-			policyNames (dict): Specifies the list of policies.
+			policyNames (list): Specifies the list of policies.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("set_policy_mode", locals())
 
@@ -814,28 +816,28 @@
 		if organization:
 			url_params.append('organization=' + organization)
 		if policyNames:
 			url_params.append('policyNames=' + policyNames)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-	def set_policy_permission(self, decision: str, policies: dict, applyNested: bool = None, organization: str = None, products: dict = None, signed: bool = None, vendors: dict = None, versions: dict = None) -> tuple[bool, None]:
+	def set_policy_permission(self, decision: str, policies: list, applyNested: bool = None, organization: str = None, products: list = None, signed: bool = None, vendors: list = None, versions: list = None) -> tuple[bool, None]:
 		'''
 		Class CommunicationControl
 		Description: Set the application allow/deny.
         
 		Args:
 			applyNested (bool): A true/false parameter indicating updating inherited.
 			decision (str): Indicates the action.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
-			policies (dict): Specifies the list of policies names.
-			products (dict): Specifies the list of product names. Names must match exactly (strictMode is always true).
+			policies (list): Specifies the list of policies names.
+			products (list): Specifies the list of product names. Names must match exactly (strictMode is always true).
 			signed (bool): A true/false parameter indicating if the policy is signed.
-			vendors (dict): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
-			versions (dict): Specifies the list of versions. Names must match exactly (strictMode is always true).
+			vendors (list): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
+			versions (list): Specifies the list of versions. Names must match exactly (strictMode is always true).
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("set_policy_permission", locals())
 
@@ -889,54 +891,54 @@
 			url_params.append('state=' + state)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 class Events:
 	'''This API call outputs all the events in the system that match the condition(s) you specify in the call. An AND relationship exists when specifying multiple input parameters. When no input parameters are matched, an empty result set is returned'''
 
-	def insert_events(self, actions: dict = None, applicationControl: bool = None, archived: bool = None, classifications: dict = None, collectorGroups: dict = None, destinations: dict = None, device: str = None, deviceControl: bool = None, deviceIps: dict = None, eventIds: dict = None, eventType: dict = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: dict = None, muted: bool = None, operatingSystems: dict = None, organization: str = None, pageNumber: int = None, paths: dict = None, process: str = None, rule: str = None, seen: bool = None, severities: dict = None, signed: bool = None, sorting: str = None, strictMode: bool = None, archive: bool = None, classification: str = None, comment: str = None, familyName: str = None, forceUnmute: bool = None, handle: bool = None, malwareType: str = None, mute: bool = None, muteDuration: str = None, read: bool = None, threatName: str = None) -> tuple[bool, None]:
+	def insert_events(self, actions: list = None, applicationControl: bool = None, archived: bool = None, classifications: list = None, collectorGroups: list = None, destinations: list = None, device: str = None, deviceControl: bool = None, deviceIps: list = None, eventIds: list = None, eventType: list = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: list = None, muted: bool = None, operatingSystems: list = None, organization: str = None, pageNumber: int = None, paths: list = None, process: str = None, rule: str = None, seen: bool = None, severities: list = None, signed: bool = None, sorting: str = None, strictMode: bool = None, archive: bool = None, classification: str = None, comment: str = None, familyName: str = None, forceUnmute: bool = None, handle: bool = None, malwareType: str = None, mute: bool = None, muteDuration: str = None, read: bool = None, threatName: str = None) -> tuple[bool, None]:
 		'''
 		Class Events
 		Description: This API call updates the read/unread, handled/unhandled or archived/unarchived state of an event. The output of this call is a message indicating whether the update succeeded or failed.
         
 		Args:
-			actions (dict): Specifies the action of the event.
+			actions (list): Specifies the action of the event.
 			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
 			archived (bool): A true/false parameter indicating whether to include only archived events.
-			classifications (dict): Specifies the classification of the event.
-			collectorGroups (dict): Specifies the collector groups whose collector reported the events.
-			destinations (dict): Specifies the connection destination(s) of the events.
+			classifications (list): Specifies the classification of the event.
+			collectorGroups (list): Specifies the collector groups whose collector reported the events.
+			destinations (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the device name where the events occurred.
 			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
-			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
-			eventIds (dict): Specifies the required event IDs.
-			eventType (dict): Specifies the type of the event.
+			deviceIps (list): Specifies the IPs of the devices where the event occurred.
+			eventIds (list): Specifies the required event IDs.
+			eventType (list): Specifies the type of the event.
 			expired (bool): A true/false parameter indicating whether to include only expired events.
 			fileHash (str): Specifies the hash signature of the main process of the event.
 			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the event was first seen.
 			firstSeenTo (str): Specifies the to date when the event was first seen.
 			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the event was last seen.
 			lastSeenTo (str): Specifies the to date when the event was last seen.
 			loggedUser (str): Specifies the logged user.
-			macAddresses (dict): Specifies the mac addresses where the event occurred.
+			macAddresses (list): Specifies the mac addresses where the event occurred.
 			muted (bool): A true/false parameter indicating if the event is muted.
-			operatingSystems (dict): Specifies the operating system of the devices where the events occurred.
+			operatingSystems (list): Specifies the operating system of the devices where the events occurred.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
-			paths (dict): Specifies the paths of the processes related to the event.
+			paths (list): Specifies the paths of the processes related to the event.
 			process (str): Specifies the main process of the event.
 			rule (str): Specifies the short rule name of the rule that triggered the events.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
-			severities (dict): Specifies the severity of the event (Deprecated).
+			severities (list): Specifies the severity of the event (Deprecated).
 			signed (bool): A true/false parameter indicating if the event is signed.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			updateEventsRequest (Object): Check 'updateEventsRequest' in the API documentation for further information.
 
 		Returns:
 			bool: Status of the request (True or False). 
@@ -1029,55 +1031,55 @@
 			"mute": mute,
 			"muteDuration": muteDuration,
 			"read": read,
 			"threatName": threatName,
 		}
 		return fortiedr_connection.insert(url, updateEventsRequest)
 
-	def delete_events(self, actions: dict = None, applicationControl: bool = None, archived: bool = None, classifications: dict = None, collectorGroups: dict = None, deleteAll: bool = None, destinations: dict = None, device: str = None, deviceControl: bool = None, deviceIps: dict = None, eventIds: dict = None, eventType: dict = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: dict = None, muted: bool = None, operatingSystems: dict = None, organization: str = None, pageNumber: int = None, paths: dict = None, process: str = None, rule: str = None, seen: bool = None, severities: dict = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, None]:
+	def delete_events(self, actions: list = None, applicationControl: bool = None, archived: bool = None, classifications: list = None, collectorGroups: list = None, deleteAll: bool = None, destinations: list = None, device: str = None, deviceControl: bool = None, deviceIps: list = None, eventIds: list = None, eventType: list = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: list = None, muted: bool = None, operatingSystems: list = None, organization: str = None, pageNumber: int = None, paths: list = None, process: str = None, rule: str = None, seen: bool = None, severities: list = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, None]:
 		'''
 		Class Events
 		Description: This API call delete events.
         
 		Args:
-			actions (dict): Specifies the action of the event.
+			actions (list): Specifies the action of the event.
 			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
 			archived (bool): A true/false parameter indicating whether to include only archived events.
-			classifications (dict): Specifies the classification of the event.
-			collectorGroups (dict): Specifies the collector groups whose collector reported the events.
+			classifications (list): Specifies the classification of the event.
+			collectorGroups (list): Specifies the collector groups whose collector reported the events.
 			deleteAll (bool): A true/false parameter indicating if all events should be deleted.
-			destinations (dict): Specifies the connection destination(s) of the events.
+			destinations (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the device name where the events occurred.
 			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
-			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
-			eventIds (dict): Specifies the required event IDs.
-			eventType (dict): Specifies the type of the event.
+			deviceIps (list): Specifies the IPs of the devices where the event occurred.
+			eventIds (list): Specifies the required event IDs.
+			eventType (list): Specifies the type of the event.
 			expired (bool): A true/false parameter indicating whether to include only expired events.
 			fileHash (str): Specifies the hash signature of the main process of the event.
 			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the event was first seen.
 			firstSeenTo (str): Specifies the to date when the event was first seen.
 			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the event was last seen.
 			lastSeenTo (str): Specifies the to date when the event was last seen.
 			loggedUser (str): Specifies the logged user.
-			macAddresses (dict): Specifies the mac addresses where the event occurred.
+			macAddresses (list): Specifies the mac addresses where the event occurred.
 			muted (bool): A true/false parameter indicating if the event is muted.
-			operatingSystems (dict): Specifies the operating system of the devices where the events occurred.
+			operatingSystems (list): Specifies the operating system of the devices where the events occurred.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
-			paths (dict): Specifies the paths of the processes related to the event.
+			paths (list): Specifies the paths of the processes related to the event.
 			process (str): Specifies the main process of the event.
 			rule (str): Specifies the short rule name of the rule that triggered the events.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
-			severities (dict): Specifies the severity of the event (Deprecated).
+			severities (list): Specifies the severity of the event (Deprecated).
 			signed (bool): A true/false parameter indicating if the event is signed.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -1157,54 +1159,54 @@
 		if sorting:
 			url_params.append('sorting=' + sorting)
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-	def count_events(self, actions: dict = None, applicationControl: bool = None, archived: bool = None, classifications: dict = None, collectorGroups: dict = None, destinations: dict = None, device: str = None, deviceControl: bool = None, deviceIps: dict = None, eventIds: dict = None, eventType: dict = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: dict = None, muted: bool = None, operatingSystems: dict = None, organization: str = None, pageNumber: int = None, paths: dict = None, process: str = None, rule: str = None, seen: bool = None, severities: dict = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, int]:
+	def count_events(self, actions: list = None, applicationControl: bool = None, archived: bool = None, classifications: list = None, collectorGroups: list = None, destinations: list = None, device: str = None, deviceControl: bool = None, deviceIps: list = None, eventIds: list = None, eventType: list = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: list = None, muted: bool = None, operatingSystems: list = None, organization: str = None, pageNumber: int = None, paths: list = None, process: str = None, rule: str = None, seen: bool = None, severities: list = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, int]:
 		'''
 		Class Events
 		Description: Count Events.
         
 		Args:
-			actions (dict): Specifies the action of the event.
+			actions (list): Specifies the action of the event.
 			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
 			archived (bool): A true/false parameter indicating whether to include only archived events.
-			classifications (dict): Specifies the classification of the event.
-			collectorGroups (dict): Specifies the collector groups whose collector reported the events.
-			destinations (dict): Specifies the connection destination(s) of the events.
+			classifications (list): Specifies the classification of the event.
+			collectorGroups (list): Specifies the collector groups whose collector reported the events.
+			destinations (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the device name where the events occurred.
 			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
-			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
-			eventIds (dict): Specifies the required event IDs.
-			eventType (dict): Specifies the type of the event.
+			deviceIps (list): Specifies the IPs of the devices where the event occurred.
+			eventIds (list): Specifies the required event IDs.
+			eventType (list): Specifies the type of the event.
 			expired (bool): A true/false parameter indicating whether to include only expired events.
 			fileHash (str): Specifies the hash signature of the main process of the event.
 			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the event was first seen.
 			firstSeenTo (str): Specifies the to date when the event was first seen.
 			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the event was last seen.
 			lastSeenTo (str): Specifies the to date when the event was last seen.
 			loggedUser (str): Specifies the logged user.
-			macAddresses (dict): Specifies the mac addresses where the event occurred.
+			macAddresses (list): Specifies the mac addresses where the event occurred.
 			muted (bool): A true/false parameter indicating if the event is muted.
-			operatingSystems (dict): Specifies the operating system of the devices where the events occurred.
+			operatingSystems (list): Specifies the operating system of the devices where the events occurred.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
-			paths (dict): Specifies the paths of the processes related to the event.
+			paths (list): Specifies the paths of the processes related to the event.
 			process (str): Specifies the main process of the event.
 			rule (str): Specifies the short rule name of the rule that triggered the events.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
-			severities (dict): Specifies the severity of the event (Deprecated).
+			severities (list): Specifies the severity of the event (Deprecated).
 			signed (bool): A true/false parameter indicating if the event is signed.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			int
@@ -1282,33 +1284,33 @@
 		if sorting:
 			url_params.append('sorting=' + sorting)
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def create_exception(self, allCollectorGroups: bool = None, allDestinations: bool = None, allOrganizations: bool = None, allUsers: bool = None, collectorGroups: dict = None, comment: str = None, destinations: dict = None, eventId: int = None, exceptionId: int = None, useAnyPath: object = None, useInException: object = None, wildcardFiles: object = None, wildcardPaths: object = None, forceCreate: bool = None, organization: str = None, users: dict = None) -> tuple[bool, str]:
+	def create_exception(self, allCollectorGroups: bool = None, allDestinations: bool = None, allOrganizations: bool = None, allUsers: bool = None, collectorGroups: list = None, comment: str = None, destinations: list = None, eventId: int = None, exceptionId: int = None, useAnyPath: object = None, useInException: object = None, wildcardFiles: object = None, wildcardPaths: object = None, forceCreate: bool = None, organization: str = None, users: list = None) -> tuple[bool, str]:
 		'''
 		Class Events
 		Description: This API call adds an exception to a specific event. The output of this call is a message indicating whether the creation of the exception .
         
 		Args:
 			allCollectorGroups (bool): A true/false parameter indicating whether the exception should be applied to all collector groups. When not used, all collector groups are selected.
 			allDestinations (bool): A true/false parameter indicating whether the exception should be applied to all destinations. When not used, all destinations are selected.
 			allOrganizations (bool): A true/false parameter indicating whether the exception should be applied to all the organizations (tenants). This parameter is only relevant in multi-tenancy environment. This parameter is only allowed for user with Hoster privilege (general admin).
 			allUsers (bool): A true/false parameter indicating whether the exception should be applied to all users. When not used, all users are selected.
-			collectorGroups (dict): Specifies the list of all the collector groups to which the exception should be applied. When not used, all collector groups are selected.
+			collectorGroups (list): Specifies the list of all the collector groups to which the exception should be applied. When not used, all collector groups are selected.
 			comment (str): Specifies a user-defined string to attach to the exception.
-			destinations (dict): A list of IPs to which the exception applies and/or the value all internal destinations.
+			destinations (list): A list of IPs to which the exception applies and/or the value all internal destinations.
 			eventId (int): Specifies the event ID on which to create the exception.
 			exceptionId (int): Specifies the exception ID to edit.
 			exceptionRequest (Object): Check 'exceptionRequest' in the API documentation for further information.
 			forceCreate (bool): A true/false parameter indicating whether to create the exception, even if there are already exceptions that cover this given event.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
-			users (dict): A list of users to which the exception.
+			users (list): A list of users to which the exception.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			str
 		'''
 		validate_params("create_exception", locals())
 
@@ -1342,15 +1344,15 @@
 
 		exceptionRequest = {
 			"useAnyPath": useAnyPath,
 			"useInException": useInException,
 			"wildcardFiles": wildcardFiles,
 			"wildcardPaths": wildcardPaths,
 		}
-		return fortiedr_connection.upload(url, exceptionRequest)
+		return fortiedr_connection.send(url, exceptionRequest)
 
 	def export_raw_data_items_json(self, organization: str = None, rawItemIds: str = None) -> tuple[bool, None]:
 		'''
 		Class Events
 		Description: Get event as Json format.
         
 		Args:
@@ -1366,56 +1368,56 @@
 		url = '/management-rest/events/export-raw-data-items-json'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		if rawItemIds:
 			url_params.append('rawItemIds=' + rawItemIds)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
+		return fortiedr_connection.download(url, file_format='json')
 
-	def list_events(self, actions: dict = None, applicationControl: bool = None, archived: bool = None, classifications: dict = None, collectorGroups: dict = None, destinations: dict = None, device: str = None, deviceControl: bool = None, deviceIps: dict = None, eventIds: dict = None, eventType: dict = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: dict = None, muted: bool = None, operatingSystems: dict = None, organization: str = None, pageNumber: int = None, paths: dict = None, process: str = None, rule: str = None, seen: bool = None, severities: dict = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, list]:
+	def list_events(self, actions: list = None, applicationControl: bool = None, archived: bool = None, classifications: list = None, collectorGroups: list = None, destinations: list = None, device: str = None, deviceControl: bool = None, deviceIps: list = None, eventIds: list = None, eventType: list = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: list = None, muted: bool = None, operatingSystems: list = None, organization: str = None, pageNumber: int = None, paths: list = None, process: str = None, rule: str = None, seen: bool = None, severities: list = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
 		Class Events
 		Description: List Events.
         
 		Args:
-			actions (dict): Specifies the action of the event.
+			actions (list): Specifies the action of the event.
 			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
 			archived (bool): A true/false parameter indicating whether to include only archived events.
-			classifications (dict): Specifies the classification of the event.
-			collectorGroups (dict): Specifies the collector groups whose collector reported the events.
-			destinations (dict): Specifies the connection destination(s) of the events.
+			classifications (list): Specifies the classification of the event.
+			collectorGroups (list): Specifies the collector groups whose collector reported the events.
+			destinations (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the device name where the events occurred.
 			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
-			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
-			eventIds (dict): Specifies the required event IDs.
-			eventType (dict): Specifies the type of the event.
+			deviceIps (list): Specifies the IPs of the devices where the event occurred.
+			eventIds (list): Specifies the required event IDs.
+			eventType (list): Specifies the type of the event.
 			expired (bool): A true/false parameter indicating whether to include only expired events.
 			fileHash (str): Specifies the hash signature of the main process of the event.
 			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the event was first seen.
 			firstSeenTo (str): Specifies the to date when the event was first seen.
 			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the event was last seen.
 			lastSeenTo (str): Specifies the to date when the event was last seen.
 			loggedUser (str): Specifies the logged user.
-			macAddresses (dict): Specifies the mac addresses where the event occurred.
+			macAddresses (list): Specifies the mac addresses where the event occurred.
 			muted (bool): A true/false parameter indicating if the event is muted.
-			operatingSystems (dict): Specifies the operating system of the devices where the events occurred.
+			operatingSystems (list): Specifies the operating system of the devices where the events occurred.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
-			paths (dict): Specifies the paths of the processes related to the event.
+			paths (list): Specifies the paths of the processes related to the event.
 			process (str): Specifies the main process of the event.
 			rule (str): Specifies the short rule name of the rule that triggered the events.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
-			severities (dict): Specifies the severity of the event (Deprecated).
+			severities (list): Specifies the severity of the event (Deprecated).
 			signed (bool): A true/false parameter indicating if the event is signed.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
@@ -1493,37 +1495,37 @@
 		if sorting:
 			url_params.append('sorting=' + sorting)
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def list_raw_data_items(self, eventId: int, collectorGroups: dict = None, destinations: dict = None, device: str = None, deviceIps: dict = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, fullDataRequested: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, organization: str = None, pageNumber: int = None, rawEventIds: dict = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, list]:
+	def list_raw_data_items(self, eventId: int, collectorGroups: list = None, destinations: list = None, device: str = None, deviceIps: list = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, fullDataRequested: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, organization: str = None, pageNumber: int = None, rawEventIds: list = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
 		Class Events
 		Description: List raw data items.
         
 		Args:
-			collectorGroups (dict): Specifies the collector groups whose collector reported the raw events.
-			destinations (dict): Specifies the connection destination(s) of the events.
+			collectorGroups (list): Specifies the collector groups whose collector reported the raw events.
+			destinations (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the name of the device where the raw event occurred.
-			deviceIps (dict): Specifies the IPs of the devices where the event occurred.
+			deviceIps (list): Specifies the IPs of the devices where the event occurred.
 			eventId (int): Specifies the ID of the event that holds the raw data items.
 			firstSeen (str): Specifies the date when the raw data item was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the raw data item was first seen.
 			firstSeenTo (str): Specifies the to date when the raw data item was first seen.
 			fullDataRequested (bool): A true/false parameter indicating whether to include the event internal information.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str): Specifies the date when the raw data item was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the raw data item was last seen.
 			lastSeenTo (str): Specifies the to date when the raw data item was last seen.
 			loggedUser (str): Specifies the logged user.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			pageNumber (int): An integer used for paging that indicates the required page number.
-			rawEventIds (dict): Specifies the list of raw data item event IDs.
+			rawEventIds (list): Specifies the list of raw data item event IDs.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
@@ -1594,36 +1596,36 @@
 		url = '/management-rest/exceptions/create-or-edit-exception'
 		url_params = []
 		if confirmEdit:
 			url_params.append('confirmEdit=' + confirmEdit)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url, exceptionJSON)
+		return fortiedr_connection.send(url, exceptionJSON)
 
-	def delete(self, collectorGroups: dict = None, comment: str = None, createdAfter: str = None, createdBefore: str = None, deleteAll: bool = None, destination: str = None, exceptionId: int = None, exceptionIds: dict = None, organization: str = None, path: str = None, process: str = None, rules: dict = None, updatedAfter: str = None, updatedBefore: str = None, user: str = None) -> tuple[bool, None]:
+	def delete(self, collectorGroups: list = None, comment: str = None, createdAfter: str = None, createdBefore: str = None, deleteAll: bool = None, destination: str = None, exceptionId: int = None, exceptionIds: list = None, organization: str = None, path: str = None, process: str = None, rules: list = None, updatedAfter: str = None, updatedBefore: str = None, user: str = None) -> tuple[bool, None]:
 		'''
 		Class Exceptions
 		Description: Delete exceptions.
         
 		Args:
-			collectorGroups (dict): Specifies the list of all the collector groups to which the exception applied.
+			collectorGroups (list): Specifies the list of all the collector groups to which the exception applied.
 			comment (str): Specifies a comment attach to the exception.
 			createdAfter (str): Specifies the date after which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			createdBefore (str): Specifies the date before which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			deleteAll (bool): A true/false parameter indicating if all exception should be deleted.
 			destination (str): Specifies a destination IP of the exception.
 			exceptionId (int): Specifies the required exception ID.
-			exceptionIds (dict): Specifies a list of exception ids.
+			exceptionIds (list): Specifies a list of exception ids.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			path (str): Specifies the path of the exception.
 			process (str): Specifies the process of the exception.
-			rules (dict): Specifies a list of rule names.
+			rules (list): Specifies a list of rule names.
 			updatedAfter (str): Specifies the date after which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			updatedBefore (str): Specifies the date before which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			user (str): Specifies a user of the exception.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -1685,32 +1687,32 @@
 		if eventId:
 			url_params.append('eventId=' + str(eventId))
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def list_exceptions(self, collectorGroups: dict = None, comment: str = None, createdAfter: str = None, createdBefore: str = None, destination: str = None, exceptionIds: dict = None, organization: str = None, path: str = None, process: str = None, rules: dict = None, updatedAfter: str = None, updatedBefore: str = None, user: str = None) -> tuple[bool, list]:
+	def list_exceptions(self, collectorGroups: list = None, comment: str = None, createdAfter: str = None, createdBefore: str = None, destination: str = None, exceptionIds: list = None, organization: str = None, path: str = None, process: str = None, rules: list = None, updatedAfter: str = None, updatedBefore: str = None, user: str = None) -> tuple[bool, list]:
 		'''
 		Class Exceptions
 		Description: List of exceptions.
         
 		Args:
-			collectorGroups (dict): Specifies the list of all the collector groups to which the exception applied.
+			collectorGroups (list): Specifies the list of all the collector groups to which the exception applied.
 			comment (str): Specifies a comment attach to the exception.
 			createdAfter (str): Specifies the date after which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			createdBefore (str): Specifies the date before which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			destination (str): Specifies a destination IP of the exception.
-			exceptionIds (dict): Specifies a list of exception ids.
+			exceptionIds (list): Specifies a list of exception ids.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			path (str): Specifies the path of the exception.
 			process (str): Specifies the process of the exception.
-			rules (dict): Specifies a list of rule names.
+			rules (list): Specifies a list of rule names.
 			updatedAfter (str): Specifies the date after which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			updatedBefore (str): Specifies the date before which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			user (str): Specifies a user of the exception.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
@@ -1747,23 +1749,23 @@
 			url_params.append('user=' + user)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
 class Forensics:
 	'''The Forensics module facilitates deep analysis into the actual internals of the communicating devices operating system that led up to an event.'''
 
-	def get_event_file(self, rawEventId: int, disk: bool = None, endRange: str = None, filePaths: dict = None, memory: bool = None, organization: str = None, processId: int = None, startRange: str = None) -> tuple[bool, None]:
+	def get_event_file(self, rawEventId: int, disk: bool = None, endRange: str = None, filePaths: list = None, memory: bool = None, organization: str = None, processId: int = None, startRange: str = None) -> tuple[bool, None]:
 		'''
 		Class Forensics
 		Description: This API call retrieves a file or memory.
         
 		Args:
 			disk (bool): A true/false parameter indicating whether find in the disk.
 			endRange (str): Specifies the memory end range, in Hexadecimal format.
-			filePaths (dict): Specifies the list of file paths.
+			filePaths (list): Specifies the list of file paths.
 			memory (bool): A true/false parameter indicating whether find in the memory.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			processId (int): Specifies the ID of the process from which to take a memory image. required for memory base action.
 			rawEventId (int): Specifies the ID of the raw event on which to perform the memory retrieval.
 			startRange (str): Specifies the memory start range, in Hexadecimal format.
 
 		Returns:
@@ -1789,22 +1791,22 @@
 		if rawEventId:
 			url_params.append('rawEventId=' + str(rawEventId))
 		if startRange:
 			url_params.append('startRange=' + startRange)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def get_file(self, device: str, filePaths: dict, type: str, organization: str = None) -> tuple[bool, None]:
+	def get_file(self, device: str, filePaths: list, type: str, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Forensics
 		Description: This API call retrieves a file or memory.
         
 		Args:
 			device (str): Specifies the name or id of the device to remediate.
-			filePaths (dict): Specifies the list of file paths.
+			filePaths (list): Specifies the list of file paths.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			type (str): Specifies the device parameter type used in the request : Name or ID.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
@@ -1819,23 +1821,23 @@
 		if organization:
 			url_params.append('organization=' + organization)
 		if type:
 			url_params.append('type=' + type)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def remediate_device(self, terminatedProcessId: int, device: str = None, deviceId: int = None, executablesToRemove: dict = None, organization: str = None, persistenceDataAction: str = None, persistenceDataNewContent: str = None, persistenceDataPath: str = None, persistenceDataValueName: str = None, persistenceDataValueNewType: str = None, processName: str = None, threadId: int = None) -> tuple[bool, None]:
+	def remediate_device(self, terminatedProcessId: int, device: str = None, deviceId: int = None, executablesToRemove: list = None, organization: str = None, persistenceDataAction: str = None, persistenceDataNewContent: str = None, persistenceDataPath: str = None, persistenceDataValueName: str = None, persistenceDataValueNewType: str = None, processName: str = None, threadId: int = None) -> tuple[bool, None]:
 		'''
 		Class Forensics
 		Description: This API kill process / delete file / clean persistence, File and persistence paths must be specified in a logical format.
         
 		Args:
 			device (str): Specifies the name of the device to remediate. You must specify a value for either device or deviceId (see below).
 			deviceId (int): Specifies the unique identifier (ID) of the device to remediate. You must specify a value for either deviceId or device (see above).
-			executablesToRemove (dict): Specifies the list of full paths of executable files (*.exe) to delete on the
+			executablesToRemove (list): Specifies the list of full paths of executable files (*.exe) to delete on the
 given device.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			persistenceDataAction (str): persistence data desired action.
 			persistenceDataNewContent (str): persistence data new content.
 			persistenceDataPath (str): persistence data path.
 			persistenceDataValueName (str): persistence data value name.
 			persistenceDataValueNewType (str): persistence data value new type.
@@ -1877,21 +1879,21 @@
 			url_params.append('threadId=' + str(threadId))
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 class HashSearch:
 	'''The Hash Search API'''
 
-	def search(self, fileHashes: dict, organization: str = None) -> tuple[bool, None]:
+	def search(self, fileHashes: list, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class HashSearch
 		Description: This API enables the user to search a file hash among the current events, threat hunting repository and communicating applications that exist in the system.
         
 		Args:
-			fileHashes (dict): Specifies the list of files hashes.
+			fileHashes (list): Specifies the list of files hashes.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -1927,15 +1929,15 @@
 		url = '/management-rest/integrations/connectors-metadata'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def create_connector(self, apiKey: str = None, connectorActions: dict = None, coreId: int = None, enabled: bool = None, host: str = None, name: str = None, organization: str = None, password: str = None, port: str = None, type: str = None, username: str = None, vendor: str = None) -> tuple[bool, None]:
+	def create_connector(self, apiKey: str = None, connectorActions: list = None, coreId: int = None, enabled: bool = None, host: str = None, name: str = None, organization: str = None, password: str = None, port: str = None, type: str = None, username: str = None, vendor: str = None) -> tuple[bool, None]:
 		'''
 		Class Integrations
 		Description: Creates a new connector. Please note: Creation of Custom connectors/actions is not yet support..
         
 		Args:
 			createConnectorRequest (Object): Check 'createConnectorRequest' in the API documentation for further information.
 
@@ -1957,15 +1959,15 @@
 			"organization": organization,
 			"password": password,
 			"port": port,
 			"type": type,
 			"username": username,
 			"vendor": vendor,
 		}
-		return fortiedr_connection.upload(url, createConnectorRequest)
+		return fortiedr_connection.send(url, createConnectorRequest)
 
 	def delete_connector(self, connectorName: str, connectorType: str, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Integrations
 		Description: Deletes a connector.
         
 		Args:
@@ -2037,15 +2039,15 @@
 		if connectorType:
 			url_params.append('connectorType=' + connectorType)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def update_connector(self, apiKey: str = None, connectorActions: dict = None, coreId: int = None, enabled: bool = None, host: str = None, name: str = None, organization: str = None, password: str = None, port: str = None, type: str = None, username: str = None, vendor: str = None) -> tuple[bool, None]:
+	def update_connector(self, apiKey: str = None, connectorActions: list = None, coreId: int = None, enabled: bool = None, host: str = None, name: str = None, organization: str = None, password: str = None, port: str = None, type: str = None, username: str = None, vendor: str = None) -> tuple[bool, None]:
 		'''
 		Class Integrations
 		Description: Updates an existing connector based on (name, type, organization). Please note: Modification of Custom connectors/actions is not yet support..
         
 		Args:
 			updateConnectorRequest (Object): Check 'updateConnectorRequest' in the API documentation for further information.
 
@@ -2196,15 +2198,15 @@
 		url = '/management-rest/inventory/create-collector-group'
 		url_params = []
 		if name:
 			url_params.append('name=' + name)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url)
+		return fortiedr_connection.send(url)
 
 	def create_ems_custom_installer(self, osType: str, aggregatorAddress: str = None, aggregatorPort: int = None, citrixPVS: bool = None, collectorGroup: str = None, collectorVersion: str = None, distro: str = None, is64bit: bool = None, organization: str = None, proxy: bool = None, vdi: bool = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call sends request for creating custom-installer for EMS integration.
         
 		Args:
@@ -2247,54 +2249,54 @@
 		if osType:
 			url_params.append('osType=' + osType)
 		if proxy:
 			url_params.append('proxy=' + proxy)
 		if vdi:
 			url_params.append('vdi=' + vdi)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url)
+		return fortiedr_connection.send(url)
 
-	def delete_collectors(self, cloudAccounts: dict = None, cloudProviders: dict = None, clusters: dict = None, collectorGroups: dict = None, collectorGroupsIds: dict = None, collectorType: str = None, confirmDeletion: bool = None, deleteAll: bool = None, devices: dict = None, devicesIds: dict = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: dict = None, organization: str = None, osFamilies: dict = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: dict = None, strictMode: bool = None, versions: dict = None) -> tuple[bool, None]:
+	def delete_collectors(self, cloudAccounts: list = None, cloudProviders: list = None, clusters: list = None, collectorGroups: list = None, collectorGroupsIds: list = None, collectorType: str = None, confirmDeletion: bool = None, deleteAll: bool = None, devices: list = None, devicesIds: list = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: list = None, organization: str = None, osFamilies: list = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: list = None, strictMode: bool = None, versions: list = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call deletes a Collector(s).
         
 		Args:
-			cloudAccounts (dict): Specifies the list cloud account names.
-			cloudProviders (dict): Specifies the list of cloud providers: AWS, Azure, GCP.
-			clusters (dict): Specifies the list of cluster.
-			collectorGroups (dict): Specifies the list of collector group names and retrieves collectors under the
+			cloudAccounts (list): Specifies the list cloud account names.
+			cloudProviders (list): Specifies the list of cloud providers: AWS, Azure, GCP.
+			clusters (list): Specifies the list of cluster.
+			collectorGroups (list): Specifies the list of collector group names and retrieves collectors under the
 given groups.
-			collectorGroupsIds (dict): Specifies the list of collector group Ids and retrieves collectors under the
+			collectorGroupsIds (list): Specifies the list of collector group Ids and retrieves collectors under the
 given groups.
 			collectorType (str): Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default.
 			confirmDeletion (bool): A true/false parameter indicating if to detach/delete relevant exceptions from Collector groups about to be deleted.
 			deleteAll (bool): A true/false parameter indicating if all collectors should be deleted.
-			devices (dict): Specifies the list of device names.
-			devicesIds (dict): Specifies the list of device ids.
+			devices (list): Specifies the list of device names.
+			devicesIds (list): Specifies the list of device ids.
 			firstSeen (str): Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			hasCrashDumps (bool): Retrieves collectors that have crash dumps.
-			ips (dict): Specifies the list of IP values.
+			ips (list): Specifies the list of IP values.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			loggedUser (str): Specifies the user that was logged when the event occurred.
-			operatingSystems (dict): Specifies the list of specific operating systems. For example, Windows 7 Pro.
+			operatingSystems (list): Specifies the list of specific operating systems. For example, Windows 7 Pro.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
-			osFamilies (dict): Specifies the list of operating system families: Windows, Windows Server or OS X.
+			osFamilies (list): Specifies the list of operating system families: Windows, Windows Server or OS X.
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
-			states (dict): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
+			states (list): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
 Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
-			versions (dict): Specifies the list of collector versions.
+			versions (list): Specifies the list of collector versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_collectors", locals())
 
@@ -2351,22 +2353,22 @@
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		if versions:
 			url_params.append('versions=' + versions)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-	def isolate_collectors(self, devices: dict = None, devicesIds: dict = None, organization: str = None) -> tuple[bool, None]:
+	def isolate_collectors(self, devices: list = None, devicesIds: list = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call isolate collector functionality.
         
 		Args:
-			devices (dict): Specifies the list of device names.
-			devicesIds (dict): Specifies the list of device ids.
+			devices (list): Specifies the list of device names.
+			devicesIds (list): Specifies the list of device ids.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("isolate_collectors", locals())
@@ -2378,26 +2380,26 @@
 		if devicesIds:
 			url_params.append('devicesIds=' + devicesIds)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-	def list_aggregators(self, ip: str = None, names: dict = None, organization: str = None, versions: dict = None) -> tuple[bool, list]:
+	def list_aggregators(self, ip: str = None, names: list = None, organization: str = None, versions: list = None) -> tuple[bool, list]:
 		'''
 		Class SystemInventory
 		Description: This API call output the list of aggregators.
         
 		Args:
 			ip (str): IP.
-			names (dict): List of aggregators names.
+			names (list): List of aggregators names.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
-			versions (dict): List of aggregators versions.
+			versions (list): List of aggregators versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_aggregators", locals())
 
@@ -2433,50 +2435,50 @@
 		url = '/management-rest/inventory/list-collector-groups'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def list_collectors(self, cloudAccounts: dict = None, cloudProviders: dict = None, clusters: dict = None, collectorGroups: dict = None, collectorGroupsIds: dict = None, collectorType: str = None, devices: dict = None, devicesIds: dict = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: dict = None, organization: str = None, osFamilies: dict = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: dict = None, strictMode: bool = None, versions: dict = None) -> tuple[bool, list]:
+	def list_collectors(self, cloudAccounts: list = None, cloudProviders: list = None, clusters: list = None, collectorGroups: list = None, collectorGroupsIds: list = None, collectorType: str = None, devices: list = None, devicesIds: list = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: list = None, organization: str = None, osFamilies: list = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: list = None, strictMode: bool = None, versions: list = None) -> tuple[bool, list]:
 		'''
 		Class SystemInventory
 		Description: This API call outputs a list of the Collectors in the system. Use the input parameters to filter the list.
         
 		Args:
-			cloudAccounts (dict): Specifies the list cloud account names.
-			cloudProviders (dict): Specifies the list of cloud providers: AWS, Azure, GCP.
-			clusters (dict): Specifies the list of cluster.
-			collectorGroups (dict): Specifies the list of collector group names and retrieves collectors under the
+			cloudAccounts (list): Specifies the list cloud account names.
+			cloudProviders (list): Specifies the list of cloud providers: AWS, Azure, GCP.
+			clusters (list): Specifies the list of cluster.
+			collectorGroups (list): Specifies the list of collector group names and retrieves collectors under the
 given groups.
-			collectorGroupsIds (dict): Specifies the list of collector group Ids and retrieves collectors under the
+			collectorGroupsIds (list): Specifies the list of collector group Ids and retrieves collectors under the
 given groups.
 			collectorType (str): Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default.
-			devices (dict): Specifies the list of device names.
-			devicesIds (dict): Specifies the list of device ids.
+			devices (list): Specifies the list of device names.
+			devicesIds (list): Specifies the list of device ids.
 			firstSeen (str): Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			hasCrashDumps (bool): Retrieves collectors that have crash dumps.
-			ips (dict): Specifies the list of IP values.
+			ips (list): Specifies the list of IP values.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			loggedUser (str): Specifies the user that was logged when the event occurred.
-			operatingSystems (dict): Specifies the list of specific operating systems. For example, Windows 7 Pro.
+			operatingSystems (list): Specifies the list of specific operating systems. For example, Windows 7 Pro.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
-			osFamilies (dict): Specifies the list of operating system families: Windows, Windows Server or OS X.
+			osFamilies (list): Specifies the list of operating system families: Windows, Windows Server or OS X.
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
-			states (dict): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
+			states (list): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
 Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
-			versions (dict): Specifies the list of collector versions.
+			versions (list): Specifies the list of collector versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_collectors", locals())
 
@@ -2529,28 +2531,28 @@
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		if versions:
 			url_params.append('versions=' + versions)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def list_cores(self, deploymentModes: dict = None, hasCrashDumps: bool = None, ip: str = None, names: dict = None, organization: str = None, versions: dict = None) -> tuple[bool, list]:
+	def list_cores(self, deploymentModes: list = None, hasCrashDumps: bool = None, ip: str = None, names: list = None, organization: str = None, versions: list = None) -> tuple[bool, list]:
 		'''
 		Class SystemInventory
 		Description: This API call output the list of cores.
         
 		Args:
-			deploymentModes (dict): List of cores deployments modes.
+			deploymentModes (list): List of cores deployments modes.
 			hasCrashDumps (bool): Has crash dumps.
 			ip (str): IP.
-			names (dict): List of cores names.
+			names (list): List of cores names.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
-			versions (dict): List of cores versions.
+			versions (list): List of cores versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_cores", locals())
 
@@ -2618,23 +2620,23 @@
 		if sorting:
 			url_params.append('sorting=' + sorting)
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def move_collectors(self, targetCollectorGroup: str, collectorIds: dict = None, collectorSIDs: dict = None, collectors: dict = None, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
+	def move_collectors(self, targetCollectorGroup: str, collectorIds: list = None, collectorSIDs: list = None, collectors: list = None, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call move collector between groups.
         
 		Args:
-			collectorIds (dict): value = Array of collectors Ids. To move collectors from one organization to another.
-			collectorSIDs (dict): value = Array of collectors SIDS. To move collectors from one organization to another.
-			collectors (dict): Array of collectors names. To move collectors from one organization to another, for each collector please add the organization name before the collector name (<organization-name>\\<collector-name>).
+			collectorIds (list): value = Array of collectors Ids. To move collectors from one organization to another.
+			collectorSIDs (list): value = Array of collectors SIDS. To move collectors from one organization to another.
+			collectors (list): Array of collectors names. To move collectors from one organization to another, for each collector please add the organization name before the collector name (<organization-name>\\<collector-name>).
 			forceAssign (bool): Indicates whether to force the assignment even if the organization of the target Collector group is under migration.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			targetCollectorGroup (str): Collector group. To move collectors from one organization to another, please add the organization name before the target collector group (<organization-name>\\<collector-group-name>).
 
 		Returns:
@@ -2672,51 +2674,51 @@
 			None: This function does not return any data.
 		'''
 		validate_params("system_logs", locals())
 
 		url = '/management-rest/inventory/system-logs'
 		return fortiedr_connection.get(url)
 
-	def toggle_collectors(self, enable: bool, cloudAccounts: dict = None, cloudProviders: dict = None, clusters: dict = None, collectorGroups: dict = None, collectorGroupsIds: dict = None, collectorType: str = None, devices: dict = None, devicesIds: dict = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: dict = None, organization: str = None, osFamilies: dict = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: dict = None, strictMode: bool = None, versions: dict = None) -> tuple[bool, str]:
+	def toggle_collectors(self, enable: bool, cloudAccounts: list = None, cloudProviders: list = None, clusters: list = None, collectorGroups: list = None, collectorGroupsIds: list = None, collectorType: str = None, devices: list = None, devicesIds: list = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: list = None, organization: str = None, osFamilies: list = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: list = None, strictMode: bool = None, versions: list = None) -> tuple[bool, str]:
 		'''
 		Class SystemInventory
 		Description: This API call enables/disables a Collector(s). You must specify whether the Collector is to be enabled or disabled.
         
 		Args:
-			cloudAccounts (dict): Specifies the list cloud account names.
-			cloudProviders (dict): Specifies the list of cloud providers: AWS, Azure, GCP.
-			clusters (dict): Specifies the list of cluster.
-			collectorGroups (dict): Specifies the list of collector group names and retrieves collectors under the
+			cloudAccounts (list): Specifies the list cloud account names.
+			cloudProviders (list): Specifies the list of cloud providers: AWS, Azure, GCP.
+			clusters (list): Specifies the list of cluster.
+			collectorGroups (list): Specifies the list of collector group names and retrieves collectors under the
 given groups.
-			collectorGroupsIds (dict): Specifies the list of collector group Ids and retrieves collectors under the
+			collectorGroupsIds (list): Specifies the list of collector group Ids and retrieves collectors under the
 given groups.
 			collectorType (str): Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default.
-			devices (dict): Specifies the list of device names.
-			devicesIds (dict): Specifies the list of device ids.
+			devices (list): Specifies the list of device names.
+			devicesIds (list): Specifies the list of device ids.
 			enable (bool): Toggle enable.
 			firstSeen (str): Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			hasCrashDumps (bool): Retrieves collectors that have crash dumps.
-			ips (dict): Specifies the list of IP values.
+			ips (list): Specifies the list of IP values.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			loggedUser (str): Specifies the user that was logged when the event occurred.
-			operatingSystems (dict): Specifies the list of specific operating systems. For example, Windows 7 Pro.
+			operatingSystems (list): Specifies the list of specific operating systems. For example, Windows 7 Pro.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
-			osFamilies (dict): Specifies the list of operating system families: Windows, Windows Server or OS X.
+			osFamilies (list): Specifies the list of operating system families: Windows, Windows Server or OS X.
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
-			states (dict): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
+			states (list): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
 Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
-			versions (dict): Specifies the list of collector versions.
+			versions (list): Specifies the list of collector versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			str
 		'''
 		validate_params("toggle_collectors", locals())
 
@@ -2771,22 +2773,22 @@
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		if versions:
 			url_params.append('versions=' + versions)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-	def unisolate_collectors(self, devices: dict = None, devicesIds: dict = None, organization: str = None) -> tuple[bool, None]:
+	def unisolate_collectors(self, devices: list = None, devicesIds: list = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call isolate collector functionality.
         
 		Args:
-			devices (dict): Specifies the list of device names.
-			devicesIds (dict): Specifies the list of device ids.
+			devices (list): Specifies the list of device names.
+			devicesIds (list): Specifies the list of device ids.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("unisolate_collectors", locals())
@@ -2823,45 +2825,45 @@
 		url = '/management-rest/iot/create-iot-group'
 		url_params = []
 		if name:
 			url_params.append('name=' + name)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url)
+		return fortiedr_connection.send(url)
 
-	def delete_devices(self, categories: dict = None, devices: dict = None, devicesIds: dict = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: dict = None, iotGroups: dict = None, iotGroupsIds: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: dict = None, macAddresses: dict = None, models: dict = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: dict = None) -> tuple[bool, None]:
+	def delete_devices(self, categories: list = None, devices: list = None, devicesIds: list = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: list = None, iotGroups: list = None, iotGroupsIds: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: list = None, macAddresses: list = None, models: list = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: list = None) -> tuple[bool, None]:
 		'''
 		Class IoT
 		Description: This API call deletes a IoT device(s).
         
 		Args:
-			categories (dict): Specifies the list of categories values.
-			devices (dict): Specifies the list of device names.
-			devicesIds (dict): Specifies the list of device ids.
+			categories (list): Specifies the list of categories values.
+			devices (list): Specifies the list of device names.
+			devicesIds (list): Specifies the list of device ids.
 			firstSeenEnd (str): Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			firstSeenStart (str): Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
-			internalIps (dict): Specifies the list of IP values.
-			iotGroups (dict): Specifies the list of collector group names and retrieves collectors under the given groups.
-			iotGroupsIds (dict): Specifies the list of collector group ids and retrieves collectors under the given groups.
+			internalIps (list): Specifies the list of IP values.
+			iotGroups (list): Specifies the list of collector group names and retrieves collectors under the given groups.
+			iotGroupsIds (list): Specifies the list of collector group ids and retrieves collectors under the given groups.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
-			locations (dict): Specifies the list of locations values.
-			macAddresses (dict): Specifies the list of mac address values.
-			models (dict): Specifies the list of models values.
+			locations (list): Specifies the list of locations values.
+			macAddresses (list): Specifies the list of mac address values.
+			models (list): Specifies the list of models values.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
-			vendors (dict): Specifies the list of vendors values.
+			vendors (list): Specifies the list of vendors values.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_devices", locals())
 
@@ -2906,21 +2908,21 @@
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		if vendors:
 			url_params.append('vendors=' + vendors)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-	def export_iot_json(self, iotDeviceIds: dict, organization: str = None) -> tuple[bool, None]:
+	def export_iot_json(self, iotDeviceIds: list, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class IoT
 		Description: This API call outputs a list of the IoT devices info.
         
 		Args:
-			iotDeviceIds (dict): Specifies the list of device ids.
+			iotDeviceIds (list): Specifies the list of device ids.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -2932,43 +2934,43 @@
 		if iotDeviceIds:
 			url_params.append('iotDeviceIds=' + iotDeviceIds)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def list_iot_devices(self, categories: dict = None, devices: dict = None, devicesIds: dict = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: dict = None, iotGroups: dict = None, iotGroupsIds: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: dict = None, macAddresses: dict = None, models: dict = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: dict = None) -> tuple[bool, list]:
+	def list_iot_devices(self, categories: list = None, devices: list = None, devicesIds: list = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: list = None, iotGroups: list = None, iotGroupsIds: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: list = None, macAddresses: list = None, models: list = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: list = None) -> tuple[bool, list]:
 		'''
 		Class IoT
 		Description: This API call outputs a list of the IoT devices in the system. Use the input parameters to filter the list.
         
 		Args:
-			categories (dict): Specifies the list of categories values.
-			devices (dict): Specifies the list of device names.
-			devicesIds (dict): Specifies the list of device ids.
+			categories (list): Specifies the list of categories values.
+			devices (list): Specifies the list of device names.
+			devicesIds (list): Specifies the list of device ids.
 			firstSeenEnd (str): Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			firstSeenStart (str): Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
-			internalIps (dict): Specifies the list of IP values.
-			iotGroups (dict): Specifies the list of collector group names and retrieves collectors under the given groups.
-			iotGroupsIds (dict): Specifies the list of collector group ids and retrieves collectors under the given groups.
+			internalIps (list): Specifies the list of IP values.
+			iotGroups (list): Specifies the list of collector group names and retrieves collectors under the given groups.
+			iotGroupsIds (list): Specifies the list of collector group ids and retrieves collectors under the given groups.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
-			locations (dict): Specifies the list of locations values.
-			macAddresses (dict): Specifies the list of mac address values.
-			models (dict): Specifies the list of models values.
+			locations (list): Specifies the list of locations values.
+			macAddresses (list): Specifies the list of mac address values.
+			models (list): Specifies the list of models values.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
-			vendors (dict): Specifies the list of vendors values.
+			vendors (list): Specifies the list of vendors values.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_iot_devices", locals())
 
@@ -3036,21 +3038,21 @@
 		url = '/management-rest/iot/list-iot-groups'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def move_iot_devices(self, iotDeviceIds: dict, targetIotGroup: str, organization: str = None) -> tuple[bool, None]:
+	def move_iot_devices(self, iotDeviceIds: list, targetIotGroup: str, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class IoT
 		Description: This API call move IoT devices between groups.
         
 		Args:
-			iotDeviceIds (dict): Array of IoT device ids.
+			iotDeviceIds (list): Array of IoT device ids.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			targetIotGroup (str): IoT target group name.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
@@ -3063,43 +3065,43 @@
 		if organization:
 			url_params.append('organization=' + organization)
 		if targetIotGroup:
 			url_params.append('targetIotGroup=' + targetIotGroup)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
-	def rescan_iot_device_details(self, categories: dict = None, devices: dict = None, devicesIds: dict = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: dict = None, iotGroups: dict = None, iotGroupsIds: dict = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: dict = None, macAddresses: dict = None, models: dict = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: dict = None) -> tuple[bool, str]:
+	def rescan_iot_device_details(self, categories: list = None, devices: list = None, devicesIds: list = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: list = None, iotGroups: list = None, iotGroupsIds: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: list = None, macAddresses: list = None, models: list = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: list = None) -> tuple[bool, str]:
 		'''
 		Class IoT
 		Description: This API call device details scan on IoT device(s).
         
 		Args:
-			categories (dict): Specifies the list of categories values.
-			devices (dict): Specifies the list of device names.
-			devicesIds (dict): Specifies the list of device ids.
+			categories (list): Specifies the list of categories values.
+			devices (list): Specifies the list of device names.
+			devicesIds (list): Specifies the list of device ids.
 			firstSeenEnd (str): Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			firstSeenStart (str): Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
-			internalIps (dict): Specifies the list of IP values.
-			iotGroups (dict): Specifies the list of collector group names and retrieves collectors under the given groups.
-			iotGroupsIds (dict): Specifies the list of collector group ids and retrieves collectors under the given groups.
+			internalIps (list): Specifies the list of IP values.
+			iotGroups (list): Specifies the list of collector group names and retrieves collectors under the given groups.
+			iotGroupsIds (list): Specifies the list of collector group ids and retrieves collectors under the given groups.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
-			locations (dict): Specifies the list of locations values.
-			macAddresses (dict): Specifies the list of mac address values.
-			models (dict): Specifies the list of models values.
+			locations (list): Specifies the list of locations values.
+			macAddresses (list): Specifies the list of mac address values.
+			models (list): Specifies the list of models values.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
-			vendors (dict): Specifies the list of vendors values.
+			vendors (list): Specifies the list of vendors values.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			str
 		'''
 		validate_params("rescan_iot_device_details", locals())
 
@@ -3147,15 +3149,15 @@
 			url_params.append('vendors=' + vendors)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 class IPsets:
 	'''API to define IPs sets and use them for exceptions'''
 
-	def create_ip_set(self, description: str = None, exclude: dict = None, include: dict = None, name: str = None, organization: str = None) -> tuple[bool, None]:
+	def create_ip_set(self, description: str = None, exclude: list = None, include: list = None, name: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class IPsets
 		Description: This API create IP sets in the system.
 	Use the input parameter organization=All organizations to create for all the organization. (only for Admin role.
         
 		Args:
 			ipGroupsRequest (Object): Check 'ipGroupsRequest' in the API documentation for further information.
@@ -3171,23 +3173,23 @@
 		ipGroupsRequest = {
 			"description": description,
 			"exclude": exclude,
 			"include": include,
 			"name": name,
 			"organization": organization,
 		}
-		return fortiedr_connection.upload(url, ipGroupsRequest)
+		return fortiedr_connection.send(url, ipGroupsRequest)
 
-	def delete_ip_set(self, ipSets: dict, organization: str = None) -> tuple[bool, None]:
+	def delete_ip_set(self, ipSets: list, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class IPsets
 		Description: This API delete IP sets from the system. Use the input parameters to filter organization.
         
 		Args:
-			ipSets (dict): Specifies the list of IP name to delete.
+			ipSets (list): Specifies the list of IP name to delete.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -3225,15 +3227,15 @@
 		if ip:
 			url_params.append('ip=' + ip)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def update_ip_set(self, description: str = None, exclude: dict = None, include: dict = None, name: str = None, organization: str = None) -> tuple[bool, None]:
+	def update_ip_set(self, description: str = None, exclude: list = None, include: list = None, name: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class IPsets
 		Description: This API update IP sets in the system. Use the input parameters to filter organization.
         
 		Args:
 			ipGroupsRequest (Object): Check 'ipGroupsRequest' in the API documentation for further information.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non-shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
@@ -3296,15 +3298,15 @@
 			"passwordConfirmation": passwordConfirmation,
 			"requestPolicyEngineLibUpdates": requestPolicyEngineLibUpdates,
 			"serialNumber": serialNumber,
 			"serversAllocated": str(serversAllocated),
 			"vulnerabilityAndIoT": vulnerabilityAndIoT,
 			"workstationsAllocated": str(workstationsAllocated),
 		}
-		return fortiedr_connection.upload(url, createAccountRequest)
+		return fortiedr_connection.send(url, createAccountRequest)
 
 	def delete_organization(self, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Organizations
 		Description: This API delete organization in the system (only for Admin role).
         
 		Args:
@@ -3360,15 +3362,15 @@
 			None: This function does not return any data.
 		'''
 		validate_params("import_organization", locals())
 
 		url = '/management-rest/organizations/import-organization'
 		if file:
 			file = {'file': file}
-		return fortiedr_connection.upload(url, file, request_type="multipart/form-data")
+		return fortiedr_connection.upload(url, file)
 
 	def list_organizations(self) -> tuple[bool, list]:
 		'''
 		Class Organizations
 		Description: This API call outputs a list of the accounts in the system..
         
 		Args:
@@ -3378,15 +3380,15 @@
 			list
 		'''
 		validate_params("list_organizations", locals())
 
 		url = '/management-rest/organizations/list-organizations'
 		return fortiedr_connection.get(url)
 
-	def transfer_collectors(self, aggregatorsMap: dict = None, sourceOrganization: str = None, targetOrganization: str = None, verificationCode: str = None) -> tuple[bool, None]:
+	def transfer_collectors(self, aggregatorsMap: list = None, sourceOrganization: str = None, targetOrganization: str = None, verificationCode: str = None) -> tuple[bool, None]:
 		'''
 		Class Organizations
 		Description: Transfer collectors from aggregator to aggregator as the organization migration process.
         
 		Args:
 			transferCollectorRequests (Object): Check 'transferCollectorRequests' in the API documentation for further information.
 
@@ -3400,15 +3402,15 @@
 
 		transferCollectorRequests = {
 			"aggregatorsMap": aggregatorsMap,
 			"sourceOrganization": sourceOrganization,
 			"targetOrganization": targetOrganization,
 			"verificationCode": verificationCode,
 		}
-		return fortiedr_connection.upload(url, transferCollectorRequests)
+		return fortiedr_connection.send(url, transferCollectorRequests)
 
 	def transfer_collectors_stop(self, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Organizations
 		Description: Transfer collector stop.
         
 		Args:
@@ -3421,15 +3423,15 @@
 		validate_params("transfer_collectors_stop", locals())
 
 		url = '/management-rest/organizations/transfer-collectors-stop'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url)
+		return fortiedr_connection.send(url)
 
 	def update_organization(self, eXtendedDetection: bool = None, edr: bool = None, edrAddOnsAllocated: int = None, edrBackupEnabled: bool = None, edrEnabled: bool = None, edrNumberOfShards: int = None, edrStorageAllocatedInMb: int = None, expirationDate: str = None, forensics: bool = None, iotAllocated: int = None, name: str = None, requestPolicyEngineLibUpdates: bool = None, serialNumber: str = None, serversAllocated: int = None, vulnerabilityAndIoT: bool = None, workstationsAllocated: int = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Organizations
 		Description: This API update organization in the system (only for Admin role).
         
 		Args:
@@ -3467,21 +3469,21 @@
 			"workstationsAllocated": str(workstationsAllocated),
 		}
 		return fortiedr_connection.insert(url, accountRequest)
 
 class Playbookspolicies:
 	'''Playbooks-policies API'''
 
-	def assign_collector_group(self, collectorGroupNames: dict, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
+	def assign_collector_group(self, collectorGroupNames: list, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Playbookspolicies
 		Description: Assign collector group to air policy.
         
 		Args:
-			collectorGroupNames (dict): Specifies the list of collector group names.
+			collectorGroupNames (list): Specifies the list of collector group names.
 			forceAssign (bool): Indicates whether to force the assignment even if the group is assigned to similar policies.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			policyName (str): Specifies policy name.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -3522,15 +3524,15 @@
 		if newPolicyName:
 			url_params.append('newPolicyName=' + newPolicyName)
 		if organization:
 			url_params.append('organization=' + organization)
 		if sourcePolicyName:
 			url_params.append('sourcePolicyName=' + sourcePolicyName)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url)
+		return fortiedr_connection.send(url)
 
 	def list_policies(self, organization: str = None) -> tuple[bool, list]:
 		'''
 		Class Playbookspolicies
 		Description: List policies.
         
 		Args:
@@ -3547,15 +3549,15 @@
 		url = '/management-rest/playbooks-policies/list-policies'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def map_connectors_to_actions(self, customActionsToConnectorsMaps: dict = None, fortinetActionsToConnectorsMaps: dict = None, policyName: str = None, organization: str = None) -> tuple[bool, None]:
+	def map_connectors_to_actions(self, customActionsToConnectorsMaps: list = None, fortinetActionsToConnectorsMaps: list = None, policyName: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Playbookspolicies
 		Description: Assign policy actions with connectors..
         
 		Args:
 			assignAIRActionsWithConnectorsRequest (Object): Check 'assignAIRActionsWithConnectorsRequest' in the API documentation for further information.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
@@ -3575,15 +3577,15 @@
 		assignAIRActionsWithConnectorsRequest = {
 			"customActionsToConnectorsMaps": customActionsToConnectorsMaps,
 			"fortinetActionsToConnectorsMaps": fortinetActionsToConnectorsMaps,
 			"policyName": policyName,
 		}
 		return fortiedr_connection.insert(url, assignAIRActionsWithConnectorsRequest)
 
-	def set_action_classification(self, organization: str = None, customActionsToClassificationMaps: dict = None, fortinetActionsToClassificationMaps: dict = None, policyName: str = None) -> tuple[bool, None]:
+	def set_action_classification(self, organization: str = None, customActionsToClassificationMaps: list = None, fortinetActionsToClassificationMaps: list = None, policyName: str = None) -> tuple[bool, None]:
 		'''
 		Class Playbookspolicies
 		Description: Set the air policy actions' classifications..
         
 		Args:
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			setActionsClassificationRequest (Object): Check 'setActionsClassificationRequest' in the API documentation for further information.
@@ -3633,21 +3635,21 @@
 			url_params.append('policyName=' + policyName)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 class Policies:
 	'''Policies API'''
 
-	def assign_collector_group(self, collectorsGroupName: dict, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
+	def assign_collector_group(self, collectorsGroupName: list, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Policies
 		Description: Assign collector group to policy.
         
 		Args:
-			collectorsGroupName (dict): Specifies the list of collector group names.
+			collectorsGroupName (list): Specifies the list of collector group names.
 			forceAssign (bool): Indicates whether to force the assignment even if the group is assigned to similar policies.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			policyName (str): Specifies security policy name.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -3688,15 +3690,15 @@
 		if newPolicyName:
 			url_params.append('newPolicyName=' + newPolicyName)
 		if organization:
 			url_params.append('organization=' + organization)
 		if sourcePolicyName:
 			url_params.append('sourcePolicyName=' + sourcePolicyName)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url)
+		return fortiedr_connection.send(url)
 
 	def list_policies(self, organization: str = None) -> tuple[bool, list]:
 		'''
 		Class Policies
 		Description: List policies.
         
 		Args:
@@ -3713,27 +3715,27 @@
 		url = '/management-rest/policies/list-policies'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def scan_files(self, applyRecursiveScan: bool, executableFilesOnly: bool, origin: str, scanBy: str, filePaths: dict = None, organization: str = None, scanSelection: dict = None) -> tuple[bool, None]:
+	def scan_files(self, applyRecursiveScan: bool, executableFilesOnly: bool, origin: str, scanBy: str, filePaths: list = None, organization: str = None, scanSelection: list = None) -> tuple[bool, None]:
 		'''
 		Class Policies
 		Description: Scan Files.
         
 		Args:
 			applyRecursiveScan (bool): Specifies if execution includes recursive scan.
 			executableFilesOnly (bool): Specifies if execution includes only files.
-			filePaths (dict): Specifies file path.
+			filePaths (list): Specifies file path.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			origin (str): Specifies scan origin.
 			scanBy (str): Specifies scan by choice.
-			scanSelection (dict): Specifies scan selection.
+			scanSelection (list): Specifies scan selection.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("scan_files", locals())
 
@@ -3750,15 +3752,15 @@
 		if origin:
 			url_params.append('origin=' + origin)
 		if scanBy:
 			url_params.append('scanBy=' + scanBy)
 		if scanSelection:
 			url_params.append('scanSelection=' + scanSelection)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url)
+		return fortiedr_connection.send(url)
 
 	def set_mode(self, mode: str, policyName: str, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Policies
 		Description: Set policy to simulation/prevention.
         
 		Args:
@@ -3901,27 +3903,27 @@
 			"privateKeyFile": privateKeyFile,
 			"privateKeyPassword": privateKeyPassword,
 			"protocol": protocol,
 			"syslogFormat": syslogFormat,
 			"useClientCertificate": useClientCertificate,
 			"useSSL": useSSL,
 		}
-		return fortiedr_connection.upload(url, syslogRequest)
+		return fortiedr_connection.send(url, syslogRequest)
 
 class SystemEvents:
 	'''System Events API'''
 
-	def list_system_events(self, componentNames: dict = None, componentTypes: dict = None, fromDate: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, sorting: str = None, strictMode: bool = None, toDate: str = None) -> tuple[bool, list]:
+	def list_system_events(self, componentNames: list = None, componentTypes: list = None, fromDate: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, sorting: str = None, strictMode: bool = None, toDate: str = None) -> tuple[bool, list]:
 		'''
 		Class SystemEvents
 		Description: Retrieve system events.
         
 		Args:
-			componentNames (dict):  Specifies one or more names. The name is the customer name for license-related system events and the device name for all others events.
-			componentTypes (dict): Specifies one or more component type.
+			componentNames (list):  Specifies one or more names. The name is the customer name for license-related system events and the device name for all others events.
+			componentTypes (list): Specifies one or more component type.
 			fromDate (str): Searches for system events that occurred after this date.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
@@ -3956,38 +3958,38 @@
 			url_params.append('toDate=' + toDate)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
 class ThreatHuntingExclusions:
 	'''API to create Threat Hunting exclusions.'''
 
-	def upload_exclusion(self, exclusionListName: str = None, exclusions: dict = None, organization: str = None) -> tuple[bool, list]:
+	def send_exclusion(self, exclusionListName: str = None, exclusions: list = None, organization: str = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Creates exclusions..
         
 		Args:
 			createExclusionsRequest (Object): Check 'createExclusionsRequest' in the API documentation for further information.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
-		validate_params("upload_exclusion", locals())
+		validate_params("send_exclusion", locals())
 
 		url = '/management-rest/threat-hunting-exclusions/exclusion'
 
 		createExclusionsRequest = {
 			"exclusionListName": exclusionListName,
 			"exclusions": exclusions,
 			"organization": organization,
 		}
-		return fortiedr_connection.upload(url, createExclusionsRequest)
+		return fortiedr_connection.send(url, createExclusionsRequest)
 
-	def insert_exclusions(self, exclusionListName: str = None, exclusions: dict = None, organization: str = None) -> tuple[bool, list]:
+	def insert_exclusions(self, exclusionListName: str = None, exclusions: list = None, organization: str = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Update exclusions..
         
 		Args:
 			updateExclusionsRequest (Object): Check 'updateExclusionsRequest' in the API documentation for further information.
 
@@ -4002,15 +4004,15 @@
 		updateExclusionsRequest = {
 			"exclusionListName": exclusionListName,
 			"exclusions": exclusions,
 			"organization": organization,
 		}
 		return fortiedr_connection.insert(url, updateExclusionsRequest)
 
-	def delete_exclusion(self, exclusionIds: dict = None, organization: str = None) -> tuple[bool, str]:
+	def delete_exclusion(self, exclusionIds: list = None, organization: str = None) -> tuple[bool, str]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Deletes one or more exclusions by Id..
         
 		Args:
 			deleteExclusionsRequest (Object): Check 'deleteExclusionsRequest' in the API documentation for further information.
 
@@ -4045,38 +4047,38 @@
 		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def upload_exclusions_list(self, collectorGroupIds: dict = None, name: str = None, organization: str = None) -> tuple[bool, None]:
+	def send_exclusions_list(self, collectorGroupIds: list = None, name: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Creates an exclusions list.
         
 		Args:
 			createExclusionListRequest (Object): Check 'createExclusionListRequest' in the API documentation for further information.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
-		validate_params("upload_exclusions_list", locals())
+		validate_params("send_exclusions_list", locals())
 
 		url = '/management-rest/threat-hunting-exclusions/exclusions-list'
 
 		createExclusionListRequest = {
 			"collectorGroupIds": collectorGroupIds,
 			"name": name,
 			"organization": organization,
 		}
-		return fortiedr_connection.upload(url, createExclusionListRequest)
+		return fortiedr_connection.send(url, createExclusionListRequest)
 
-	def insert_exclusions_list(self, collectorGroupIds: dict = None, listName: str = None, newName: str = None, organization: str = None) -> tuple[bool, None]:
+	def insert_exclusions_list(self, collectorGroupIds: list = None, listName: str = None, newName: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Updates an exclusions list.
         
 		Args:
 			updateExclusionListRequest (Object): Check 'updateExclusionListRequest' in the API documentation for further information.
 
@@ -4132,22 +4134,22 @@
 			None: This function does not return any data.
 		'''
 		validate_params("exclusions_metadata", locals())
 
 		url = '/management-rest/threat-hunting-exclusions/exclusions-metadata'
 		return fortiedr_connection.get(url)
 
-	def exclusions_search(self, searchText: str, organization: str = None, os: dict = None) -> tuple[bool, list]:
+	def exclusions_search(self, searchText: str, organization: str = None, os: list = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHuntingExclusions
 		Description: Free-text search of exclusions.
         
 		Args:
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
-			os (dict): OS identifiers list..
+			os (list): OS identifiers list..
 			searchText (str): The free text search string. The API will return every exclusion list that contains this string, or contains an exclusion with any field that contains it..
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("exclusions_search", locals())
@@ -4199,38 +4201,38 @@
 		url = '/management-rest/threat-hunting-settings/threat-hunting-profile'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def upload_threat_hunting_profile(self, associatedCollectorGroupIds: dict = None, name: str = None, newName: str = None, organization: str = None, threatHuntingCategoryList: dict = None) -> tuple[bool, None]:
+	def send_threat_hunting_profile(self, associatedCollectorGroupIds: list = None, name: str = None, newName: str = None, organization: str = None, threatHuntingCategoryList: list = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHuntingSettings
 		Description: Update Threat Hunting profile.
         
 		Args:
 			threatHuntingUpdateRequest (Object): Check 'threatHuntingUpdateRequest' in the API documentation for further information.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
-		validate_params("upload_threat_hunting_profile", locals())
+		validate_params("send_threat_hunting_profile", locals())
 
 		url = '/management-rest/threat-hunting-settings/threat-hunting-profile'
 
 		threatHuntingUpdateRequest = {
 			"associatedCollectorGroupIds": associatedCollectorGroupIds,
 			"name": name,
 			"newName": newName,
 			"organization": organization,
 			"threatHuntingCategoryList": threatHuntingCategoryList,
 		}
-		return fortiedr_connection.upload(url, threatHuntingUpdateRequest)
+		return fortiedr_connection.send(url, threatHuntingUpdateRequest)
 
 	def delete_threat_hunting_profile(self, name: str, organization: str, ) -> tuple[bool, None]:
 		'''
 		Class ThreatHuntingSettings
 		Description: Deletes a Threat Hunting profile..
         
 		Args:
@@ -4273,17 +4275,17 @@
 		if cloneProfileName:
 			url_params.append('cloneProfileName=' + cloneProfileName)
 		if existingProfileName:
 			url_params.append('existingProfileName=' + existingProfileName)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.upload(url)
+		return fortiedr_connection.send(url)
 
-	def threat_hunting_profile_assign_collector_groups(self, associatedCollectorGroupIds: dict = None, name: str = None, organization: str = None) -> tuple[bool, list]:
+	def threat_hunting_profile_assign_collector_groups(self, associatedCollectorGroupIds: list = None, name: str = None, organization: str = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHuntingSettings
 		Description: Update Threat Hunting profile assigned collector groups. Returns the updated list of assigned collector groups..
         
 		Args:
 			threatHuntingAssignGroupsRequest (Object): Check 'threatHuntingAssignGroupsRequest' in the API documentation for further information.
 
@@ -4296,20 +4298,20 @@
 		url = '/management-rest/threat-hunting-settings/threat-hunting-profile/collector-groups'
 
 		threatHuntingAssignGroupsRequest = {
 			"associatedCollectorGroupIds": associatedCollectorGroupIds,
 			"name": name,
 			"organization": organization,
 		}
-		return fortiedr_connection.upload(url, threatHuntingAssignGroupsRequest)
+		return fortiedr_connection.send(url, threatHuntingAssignGroupsRequest)
 
 class ThreatHunting:
 	'''API for Activity events'''
 
-	def counts(self, accountId: int = None, category: str = None, devices: dict = None, filters: dict = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: dict = None, time: str = None, toTime: str = None) -> tuple[bool, None]:
+	def counts(self, accountId: int = None, category: str = None, devices: list = None, filters: list = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: list = None, time: str = None, toTime: str = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API call outputs EDR total events for every EDR category.
         
 		Args:
 			edrRequest (Object): Check 'edrRequest' in the API documentation for further information.
 
@@ -4331,15 +4333,15 @@
 			"organization": organization,
 			"pageNumber": str(pageNumber),
 			"query": query,
 			"sorting": sorting,
 			"time": time,
 			"toTime": toTime,
 		}
-		return fortiedr_connection.upload(url, edrRequest)
+		return fortiedr_connection.send(url, edrRequest)
 
 	def create_or_edit_tag(self, newTagName: str = None, organization: str = None, tagId: int = None, tagName: str = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API creates or edits the saved queries tag.
         
 		Args:
@@ -4355,15 +4357,15 @@
 
 		createOrEditTagRequest = {
 			"newTagName": newTagName,
 			"organization": organization,
 			"tagId": str(tagId),
 			"tagName": tagName,
 		}
-		return fortiedr_connection.upload(url, createOrEditTagRequest)
+		return fortiedr_connection.send(url, createOrEditTagRequest)
 
 	def customize_fortinet_query(self, id: int = None, dayOfMonth: int = None, dayOfWeek: int = None, forceSaving: bool = None, frequency: int = None, frequencyUnit: str = None, fromTime: str = None, hour: int = None, organization: str = None, scheduled: bool = None, state: bool = None, time: str = None, toTime: str = None, queryToEdit: str = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API customizes the scheduling properties of a Fortinet query.
         
 		Args:
@@ -4395,31 +4397,31 @@
 			"hour": str(hour),
 			"organization": organization,
 			"scheduled": scheduled,
 			"state": state,
 			"time": time,
 			"toTime": toTime,
 		}
-		return fortiedr_connection.upload(url, ootbQueryCustomizeRequest)
+		return fortiedr_connection.send(url, ootbQueryCustomizeRequest)
 
-	def delete_saved_queries(self, deleteAll: bool = None, deleteFromCommunity: bool = None, organization: str = None, queryIds: dict = None, queryNames: dict = None, scheduled: bool = None, source: dict = None) -> tuple[bool, None]:
+	def delete_saved_queries(self, deleteAll: bool = None, deleteFromCommunity: bool = None, organization: str = None, queryIds: list = None, queryNames: list = None, scheduled: bool = None, source: list = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API deletes the saved queries.
         
 		Args:
 			deleteAll (bool): A true/false parameter indicating whether all queries should be deleted. False by default.
 			deleteFromCommunity (bool): A true/false parameter indicating if whether to delete a query from the FortiEDR Community also.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
-			queryIds (dict): Specifies the query IDs list.
-			queryNames (dict): Specifies the query names list.
+			queryIds (list): Specifies the query IDs list.
+			queryNames (list): Specifies the query names list.
 			scheduled (bool): A true/false parameter indicating whether the query is scheduled.
-			source (dict): Specifies the query source list.
+			source (list): Specifies the query source list.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_saved_queries", locals())
 
@@ -4438,25 +4440,25 @@
 		if scheduled:
 			url_params.append('scheduled=' + scheduled)
 		if source:
 			url_params.append('source=' + source)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-	def delete_tags(self, organization: str = None, tagIds: dict = None, tagNames: dict = None) -> tuple[bool, None]:
+	def delete_tags(self, organization: str = None, tagIds: list = None, tagNames: list = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API deletes the saved queries tags.
         
 		Args:
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
-			tagIds (dict): Specifies the tag ID list.
-			tagNames (dict): Specifies the tag name list.
+			tagIds (list): Specifies the tag ID list.
+			tagNames (list): Specifies the tag name list.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_tags", locals())
 
@@ -4467,15 +4469,15 @@
 		if tagIds:
 			url_params.append('tagIds=' + tagIds)
 		if tagNames:
 			url_params.append('tagNames=' + tagNames)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
-	def facets(self, accountId: int = None, category: str = None, devices: dict = None, facets: dict = None, filters: dict = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: dict = None, time: str = None, toTime: str = None) -> tuple[bool, list]:
+	def facets(self, accountId: int = None, category: str = None, devices: list = None, facets: list = None, filters: list = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: list = None, time: str = None, toTime: str = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHunting
 		Description: This API retrieves EDR total events for every EDR facet item.
         
 		Args:
 			facetsRequest (Object): Check 'facetsRequest' in the API documentation for further information.
 
@@ -4498,27 +4500,27 @@
 			"organization": organization,
 			"pageNumber": str(pageNumber),
 			"query": query,
 			"sorting": sorting,
 			"time": time,
 			"toTime": toTime,
 		}
-		return fortiedr_connection.upload(url, facetsRequest)
+		return fortiedr_connection.send(url, facetsRequest)
 
-	def list_saved_queries(self, organization: str = None, scheduled: bool = None, source: dict = None) -> tuple[bool, list]:
+	def list_saved_queries(self, organization: str = None, scheduled: bool = None, source: list = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHunting
 		Description: This API retrieves the existing saved queries list.
         
 		Args:
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			scheduled (bool): A true/false parameter indicating whether the query is scheduled.
-			source (dict): Specifies the query source list.
+			source (list): Specifies the query source list.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_saved_queries", locals())
 
@@ -4552,15 +4554,15 @@
 		url = '/management-rest/threat-hunting/list-tags'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
-	def save_query(self, id: int = None, queryToEdit: str = None, category: str = None, classification: str = None, collectorNames: dict = None, community: bool = None, dayOfMonth: int = None, dayOfWeek: int = None, description: str = None, forceSaving: bool = None, frequency: int = None, frequencyUnit: str = None, fromTime: str = None, hour: int = None, name: str = None, organization: str = None, query: str = None, scheduled: bool = None, state: bool = None, tagIds: dict = None, tagNames: dict = None, time: str = None, toTime: str = None) -> tuple[bool, None]:
+	def save_query(self, id: int = None, queryToEdit: str = None, category: str = None, classification: str = None, collectorNames: list = None, community: bool = None, dayOfMonth: int = None, dayOfWeek: int = None, description: str = None, forceSaving: bool = None, frequency: int = None, frequencyUnit: str = None, fromTime: str = None, hour: int = None, name: str = None, organization: str = None, query: str = None, scheduled: bool = None, state: bool = None, tagIds: list = None, tagNames: list = None, time: str = None, toTime: str = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API saves the query.
         
 		Args:
 			id (int): Specifies the query ID to edit.
 			queryToEdit (str): Specifies the query name to edit.
@@ -4599,17 +4601,17 @@
 			"scheduled": scheduled,
 			"state": state,
 			"tagIds": tagIds,
 			"tagNames": tagNames,
 			"time": time,
 			"toTime": toTime,
 		}
-		return fortiedr_connection.upload(url, saveQueryRequest)
+		return fortiedr_connection.send(url, saveQueryRequest)
 
-	def search(self, accountId: int = None, category: str = None, devices: dict = None, filters: dict = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: dict = None, time: str = None, toTime: str = None) -> tuple[bool, list]:
+	def search(self, accountId: int = None, category: str = None, devices: list = None, filters: list = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: list = None, time: str = None, toTime: str = None) -> tuple[bool, list]:
 		'''
 		Class ThreatHunting
 		Description: This API call outputs a list of Activity events from middleware..
         
 		Args:
 			edrRequest (Object): Check 'edrRequest' in the API documentation for further information.
 
@@ -4631,29 +4633,29 @@
 			"organization": organization,
 			"pageNumber": str(pageNumber),
 			"query": query,
 			"sorting": sorting,
 			"time": time,
 			"toTime": toTime,
 		}
-		return fortiedr_connection.upload(url, edrRequest)
+		return fortiedr_connection.send(url, edrRequest)
 
-	def set_query_state(self, state: bool, markAll: bool = None, organization: str = None, queryIds: dict = None, queryNames: dict = None, source: dict = None) -> tuple[bool, None]:
+	def set_query_state(self, state: bool, markAll: bool = None, organization: str = None, queryIds: list = None, queryNames: list = None, source: list = None) -> tuple[bool, None]:
 		'''
 		Class ThreatHunting
 		Description: This API updates the scheduled saved query state.
         
 		Args:
 			markAll (bool): A true/false parameter indicating whether all queries should be marked with the same value as 'state' property. False by default.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
-			queryIds (dict): Specifies the query ID list.
-			queryNames (dict): Specifies the query name list.
-			source (dict): Specifies the query source list.
+			queryIds (list): Specifies the query ID list.
+			queryNames (list): Specifies the query name list.
+			source (list): Specifies the query source list.
 			state (bool): A true/false parameter indicating whether to save the query as enabled.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("set_query_state", locals())
@@ -4710,15 +4712,15 @@
 			"password": password,
 			"remoteShell": remoteShell,
 			"restApi": restApi,
 			"role": role,
 			"title": title,
 			"username": username,
 		}
-		return fortiedr_connection.upload(url, userRequest)
+		return fortiedr_connection.send(url, userRequest)
 
 	def delete_saml_settings(self, organizationNameRequest: str, ) -> tuple[bool, None]:
 		'''
 		Class Users
 		Description: Delete SAML authentication settings per organization.
         
 		Args:
@@ -4848,15 +4850,15 @@
 			None: This function does not return any data.
 		'''
 		validate_params("update_saml_settings", locals())
 
 		url = '/management-rest/users/update-saml-settings'
 		if idpMetadataFile:
 			idpMetadataFile = {'idpMetadataFile': idpMetadataFile}
-		return fortiedr_connection.upload(url, idpMetadataFile, request_type="multipart/form-data")
+		return fortiedr_connection.upload(url, idpMetadataFile)
 
 	def update_user(self, username: str, organization: str = None, customScript: bool = None, email: str = None, firstName: str = None, lastName: str = None, remoteShell: bool = None, restApi: bool = None, role: str = None, title: str = None) -> tuple[bool, None]:
 		'''
 		Class Users
 		Description: This API update user in the system. Use the input parameters to filter organization.
         
 		Args:
@@ -4897,30 +4899,36 @@
 debug = None
 ssl_enabled = True
 organization = None
 api_json_params = None
 
 def validate_params(function_name, local_params):
 	global api_json_params
+	if not api_json_params:
+		print("Have you authenticated first?")
+		exit() 
+
 	data_types = {
 		'int': int,
+		'set': set,
 		'str': str,
+		'bool': bool,
 		'dict': dict,
 		'list': list,
-		'set': set
+		'NoneType': None,
+		'BinaryIO': bytes,
 	}
 	json_params = api_json_params[function_name]
 	for key, value in local_params.items():
 		if key == "self" or value is None: continue
+		print(json_params[key])
 		t = data_types[json_params[key]]
 		r = str(type(value))
 		if not isinstance(value, t):
-			print(f"Error on defined params!")
-			print(f"Function: {function_name}()")
-			print(f"Param '{key}' should be defined as type '{json_params[key]}', not {r}")
+			print(f"Error on defined params!\nParam '{key}' should be defined as type '{json_params[key]}', not {r}")
 			exit()
                         
 def ignore_certificate():
 	global ssl_enabled
 	ssl_enabled = False
 	print("[!] - We strongly advise you to enable SSL validations. Use this at your own risk!")
 
@@ -4930,15 +4938,14 @@
 
 def set_organization(orgname):
 	global organization
 	organization = orgname
 
 def auth( host: str, user: str, passw: str, org: str = None):
 	global debug
-	global api_json_params
 	global fortiedr_connection
 	login = fedrAuth()
 
 	if org:
 		set_organization(org)
 
 	headers, host = login.get_headers(
@@ -4953,15 +4960,15 @@
 		data = host
 	else:
 		status = True
 		data = 'AUTHENTICATION_SUCCEEDED'
 
 		fortiedr_connection = FortiEDR_API_GW()
 		authentication = fortiedr_connection.conn(headers, host, debug, ssl_enabled, organization)
-
+                            
 		cur_dir = os.path.dirname(__file__)
 		json_file = f'{cur_dir}/api_parameters.json'
 		with open(json_file, 'r') as fp:
 			api_json_params = json.loads(fp.read())
 
 	return {
 		'status': status,
```

### Comparing `fortiedr-3.5/fortiedr.egg-info/PKG-INFO` & `fortiedr-3.6/fortiedr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.5
+Version: 3.6
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.5/pyproject.toml` & `fortiedr-3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "fortiedr"
-version = "3.5"
+version = "3.6"
 authors = [
   { name="Rafael Foster", email="rafaelgfoster@gmail.com" },
 ]
 description = "This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/rafaelfoster/fortiedr"
-Issues = "https://github.com/rafaelfoster/fortiedr/issues"
+Issues = "https://github.com/rafaelfoster/fortiedr/issues"
```

### Comparing `fortiedr-3.5/setup.py` & `fortiedr-3.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 cur_dir = os.path.dirname(__file__)
 
 with open(f"{cur_dir}/requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="fortiedr",
-    version="3.5",
+    version=3.6,
     description="This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.",
     author="Rafael Foster",
     author_email="rafaelgfoster@gmail.com",
     project_urls={
         "GitHub": "https://github.com/rafaelfoster/fortiedr",
     },
     python_requires=">=3.8",
```

