# Comparing `tmp/reemployct_data_entry-2.0.5.tar.gz` & `tmp/reemployct_data_entry-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reemployct_data_entry-2.0.5.tar", max compression
+gzip compressed data, was "reemployct_data_entry-2.0.6.tar", max compression
```

## Comparing `reemployct_data_entry-2.0.5.tar` & `reemployct_data_entry-2.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2024-01-21 06:38:07.750088 reemployct_data_entry-2.0.5/LICENSE
--rw-r--r--   0        0        0     4428 2024-01-21 06:38:07.750088 reemployct_data_entry-2.0.5/README.md
--rw-r--r--   0        0        0      799 2024-01-21 06:38:07.750088 reemployct_data_entry-2.0.5/pyproject.toml
--rw-r--r--   0        0        0      651 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/__init__.py
--rw-r--r--   0        0        0    12227 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/controller_credentials.py
--rw-r--r--   0        0        0     3443 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/entry.py
--rw-r--r--   0        0        0     2819 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/entry_weeklyCertification.py
--rw-r--r--   0        0        0     4910 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/entry_workSearch.py
--rw-r--r--   0        0        0        0 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/lib/__init__.py
--rw-r--r--   0        0        0     7059 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/lib/browser_control.py
--rw-r--r--   0        0        0      880 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/lib/class_enum.py
--rw-r--r--   0        0        0     2355 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/lib/filepaths.py
--rw-r--r--   0        0        0    15580 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/lib/job_control.py
--rw-r--r--   0        0        0     1296 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/lib/stateDictionary.py
--rw-r--r--   0        0        0     2191 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/lib/wrangle_job_data.py
--rw-r--r--   0        0        0     8391 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/navigate_ReEmployCT.py
--rw-r--r--   0        0        0     1351 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/screenIDInfo.md
--rw-r--r--   0        0        0      981 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/upgrade_check.py
--rw-r--r--   0        0        0     9130 2024-01-21 06:38:07.754088 reemployct_data_entry-2.0.5/reemployct_data_entry/workSearch_template.xlsx
--rw-r--r--   0        0        0     5507 1970-01-01 00:00:00.000000 reemployct_data_entry-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/LICENSE
+-rw-r--r--   0        0        0     4428 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/README.md
+-rw-r--r--   0        0        0      799 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0      651 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/__init__.py
+-rw-r--r--   0        0        0    12227 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/controller_credentials.py
+-rw-r--r--   0        0        0     3612 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/entry.py
+-rw-r--r--   0        0        0     2819 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/entry_weeklyCertification.py
+-rw-r--r--   0        0        0     4910 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/entry_workSearch.py
+-rw-r--r--   0        0        0        0 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/lib/__init__.py
+-rw-r--r--   0        0        0     7069 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/lib/browser_control.py
+-rw-r--r--   0        0        0      880 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/lib/class_enum.py
+-rw-r--r--   0        0        0     2355 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/lib/filepaths.py
+-rw-r--r--   0        0        0    15933 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/lib/job_control.py
+-rw-r--r--   0        0        0     1296 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/lib/stateDictionary.py
+-rw-r--r--   0        0        0     2191 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/lib/wrangle_job_data.py
+-rw-r--r--   0        0        0     8391 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/navigate_ReEmployCT.py
+-rw-r--r--   0        0        0     1351 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/screenIDInfo.md
+-rw-r--r--   0        0        0      981 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/upgrade_check.py
+-rw-r--r--   0        0        0     9130 2024-04-10 02:36:47.603721 reemployct_data_entry-2.0.6/reemployct_data_entry/workSearch_template.xlsx
+-rw-r--r--   0        0        0     5507 1970-01-01 00:00:00.000000 reemployct_data_entry-2.0.6/PKG-INFO
```

### Comparing `reemployct_data_entry-2.0.5/LICENSE` & `reemployct_data_entry-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/README.md` & `reemployct_data_entry-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/pyproject.toml` & `reemployct_data_entry-2.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reemployct-data-entry"
-version = "2.0.5"
+version = "2.0.6"
 description = "Automated entry of job application data into Connecticut's DOL ReEmployCT portal."
 authors = ["Ariff Jeff <ariffjeff@icloud.com>"]
 readme = "README.md"
 packages = [{include = "reemployct_data_entry"}]
 license = "AGPL-3.0-only"
 repository = "https://github.com/ariffjeff/ReEmployCT-Data-Entry"
 keywords = ["unemployment", "benefits"]
```

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/__init__.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import colorama
 
 PACKAGE_NAME = 'reemployct_data_entry'
 
 # can't use stdlib importlib.metadata here because remote tests will fail due to needing the package build
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 # on `import reemployct_data_entry`, print the excel job data template file path for user convenience
 if __name__ == PACKAGE_NAME:
   colorama.init() # init colored text to work on Windows
 
   from reemployct_data_entry.lib import filepaths
```

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/controller_credentials.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/controller_credentials.py`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/entry.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,23 +66,24 @@
         credCon.create_user_credentials()
 
 
     ##########
     # Job Data
     ##########
 
+    print(colorama.Fore.GREEN + "\nParsing user job data..." + colorama.Style.RESET_ALL)
     jobs = job_control.Jobs(json_jobDataFilepath['filepath_jobData'])
     jobs.isolate_columns(job_control.Jobs_RequiredData)
     jobs.isolate_week(datetime.date.today() - datetime.timedelta(7))
     if(not jobs.target_week_has_jobs()): return
     jobs.sanitize()
     jobs.us_only_addresses()
     if(not jobs.target_week_has_jobs()): return
     jobs.portal_format()
-
+    print(colorama.Fore.GREEN + "Parsing completed." + colorama.Style.RESET_ALL)
 
     ############
     # Data Entry
     ############
     
     driver = navigate_ReEmployCT.navigate(creds, jobs)
     print(colorama.Fore.GREEN + "\nData entry finished.\n")
```

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/entry_weeklyCertification.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/entry_weeklyCertification.py`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/entry_workSearch.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/entry_workSearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def enterWorkSearch(driver: webdriver.Firefox, entry: PortalJobEntry) -> None:
   ############################
   # Work Search Record Details
   ############################
 
   # work search type dropdown - employer contact
-  browser_control.wait_find_element(driver, By.ID, 'j_id_46_label', 120, forceDelay=0.3).click() # Type of Work Search - Dropdown
+  browser_control.wait_find_element(driver, By.ID, 'j_id_46_label', 120, forceDelay=0.6).click() # Type of Work Search - Dropdown
   driver.find_element(by=By.ID, value='j_id_46_1').click() # Type of Work Search - Employer Contact
   
   # Date of Work Search
   input_month = browser_control.wait_find_element(driver, By.ID, 'wsrDate_-month') # MM
   input_day = driver.find_element(by=By.ID, value='wsrDate_-day') # DD
   input_year = driver.find_element(by=By.ID, value='wsrDate_-year') # YYYY
```

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/lib/browser_control.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/lib/browser_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     + "\n"
     + "Solve the captcha and then go to the next page. " + str(timeout) + " seconds until timeout."
     + "\n"
     + "**"*37
     + colorama.Style.RESET_ALL + "\n")
 
 def start_driver(site) -> webdriver.Firefox:
-    print(colorama.Fore.YELLOW + "\n*** AVOID MOVING YOUR MOUSE OVER THE WEB PAGE DURING ELEMENT NAVIGATION TO PREVENT UNEXPECTED BEHAVIOUR AND ERRORS ***\n" + colorama.Style.RESET_ALL)
+    print(colorama.Fore.YELLOW + "\n*** AVOID MOVING YOUR MOUSE OVER THE WEB PAGE DURING AUTOMATED ELEMENT NAVIGATION TO PREVENT UNEXPECTED BEHAVIOUR AND ERRORS ***\n" + colorama.Style.RESET_ALL)
     print("Starting web driver...")
     driver = webdriver.Firefox()
     print("Loading: {}".format(site))
     driver.get(site)
     driver.maximize_window()
     return driver
```

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/lib/class_enum.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/lib/class_enum.py`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/lib/filepaths.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/lib/filepaths.py`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/lib/job_control.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/lib/job_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,17 @@
     states_full_names = [el.lower() for el in states_full_names]
     states_abbrev_names = States.key_list()
     states_abbrev_names = [el.lower() for el in states_abbrev_names]
     
     initial_n = len(self.jobs)
     indexes_to_drop = []
     for i, row in self.jobs.iterrows():
-      address = Address.parse_us_address(row[Jobs_RequiredData.EMPLOYER_ADDRESS.value])
-      address[Address_RequiredComponents.ADDRESS_LINE_1.value] = Address.build_street_address_from_cleaned_address_dict(address)
+      raw_address = row[Jobs_RequiredData.EMPLOYER_ADDRESS.value]
+      address = Address.parse_us_address(raw_address)
+      address[Address_RequiredComponents.ADDRESS_LINE_1.value] = Address.build_street_address_from_cleaned_address_dict(address, raw_address)
 
       try:
         # check for US state
         if(not(address[Address_RequiredComponents.STATE_NAME.value].lower() in states_abbrev_names or
                address[Address_RequiredComponents.STATE_NAME.value].lower() in states_full_names)):
           indexes_to_drop.append(i)
         else:
@@ -137,17 +138,17 @@
 
     addresses_to_drop = []
     for i in indexes_to_drop:
       addresses_to_drop.append(self.jobs.iloc[i][Jobs_RequiredData.EMPLOYER_ADDRESS.value])
 
     if(len(addresses_to_drop) > 0):
       browser_control.msg_colored(f"{len(addresses_to_drop)} of {initial_n} job rows will be automatically excluded for the target week because they \
-contain invalid addresses and/or are non-U.S. addresses.\
-  \nIf they are supposed to be U.S. addresses, please check they are entered correctly in your Excel data.\
-  \nIf they are non-U.S. addresses, ReEmployCT won't accept them.", color="yellow")
+contain invalid addresses.\nVerify that all addresses are:\
+  \n- valid U.S. addresses. Non U.S. addresses are not accepted by ReEmployCT.\
+  \n- correctly entered in your Excel data. If the address has a number typed as a word, then it WON'T be parsed properly. ('One Mill Road' vs. '1 Mill Road')", color="yellow")
 
       print(colorama.Fore.YELLOW, "Excluding jobs with these addresses...")
       for i in range(len(addresses_to_drop)):
         print(colorama.Fore.YELLOW, i + 1, ":", addresses_to_drop[i])
 
     self.jobs.drop(indexes_to_drop, inplace=True)
 
@@ -352,28 +353,32 @@
         else:
           address_dict[key] += ' ' + address_parsed[div][0]
         if(address_dict[key][-1] == ','): # remove trailing commas
           address_dict[key] = address_dict[key][:-1]
       return address_dict
     
     @classmethod
-    def build_street_address_from_cleaned_address_dict(cls, address_dict) -> str:
+    def build_street_address_from_cleaned_address_dict(cls, address_dict, raw_address=None) -> str:
       '''
       Rebuild street address components of the cleaned address dict from a usaddress package parse into a single string
       '''
 
-      SEPARATER_KEY = 'StreetNamePostDirectional'
+      END_OF_STREET_ADDRESS_KEYS = 'StreetNamePostDirectional'
       address_line_1 = ''
       # US address components are sorted by a US standard, so loop through them to determine which dict elements to combine
       for key in usaddress.LABELS:
         if key in address_dict:
           address_line_1 += address_dict[key] + ' '
-        if(key == SEPARATER_KEY):
+        if(key == END_OF_STREET_ADDRESS_KEYS):
           address_line_1 = address_line_1.rstrip()
           break
+
+      if len(address_line_1) == 0 and raw_address is not None:
+        print(colorama.Fore.RED + f'Error! Employer Address could not be parsed: "{raw_address}"' + colorama.Style.RESET_ALL)
+      
       return address_line_1
     
 
 class Address(AddressControl):
     
     '''
     A standard U.S. address comprised of separated address components.
```

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/lib/stateDictionary.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/lib/stateDictionary.py`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/lib/wrangle_job_data.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/lib/wrangle_job_data.py`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/navigate_ReEmployCT.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/navigate_ReEmployCT.py`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/screenIDInfo.md` & `reemployct_data_entry-2.0.6/reemployct_data_entry/screenIDInfo.md`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/upgrade_check.py` & `reemployct_data_entry-2.0.6/reemployct_data_entry/upgrade_check.py`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/reemployct_data_entry/workSearch_template.xlsx` & `reemployct_data_entry-2.0.6/reemployct_data_entry/workSearch_template.xlsx`

 * *Files identical despite different names*

### Comparing `reemployct_data_entry-2.0.5/PKG-INFO` & `reemployct_data_entry-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reemployct-data-entry
-Version: 2.0.5
+Version: 2.0.6
 Summary: Automated entry of job application data into Connecticut's DOL ReEmployCT portal.
 Home-page: https://github.com/ariffjeff/ReEmployCT-Data-Entry
 License: AGPL-3.0-only
 Keywords: unemployment,benefits
 Author: Ariff Jeff
 Author-email: ariffjeff@icloud.com
 Requires-Python: >=3.10.10,<4.0.0
```

