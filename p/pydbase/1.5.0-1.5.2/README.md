# Comparing `tmp/pydbase-1.5.0.tar.gz` & `tmp/pydbase-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbase-1.5.0.tar", last modified: Tue Apr  2 05:36:08 2024, max compression
+gzip compressed data, was "pydbase-1.5.2.tar", last modified: Wed Apr 10 07:28:05 2024, max compression
```

## Comparing `pydbase-1.5.0.tar` & `pydbase-1.5.2.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.914493 pydbase-1.5.0/
--rw-r--r--   0 peterglen  (1000) users      (100)    14848 2024-04-02 05:36:08.914493 pydbase-1.5.0/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)    14434 2024-03-15 17:13:31.000000 pydbase-1.5.0/README.md
--rwxrwxr-x   0 peterglen  (1000) users      (100)     7869 2024-04-01 08:34:35.000000 pydbase-1.5.0/chainadm.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    10897 2024-04-01 03:23:33.000000 pydbase-1.5.0/dbaseadm.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.902492 pydbase-1.5.0/pydbase/
--rwxr-xr-x   0 peterglen  (1000) users      (100)        9 2023-09-25 19:38:11.000000 pydbase-1.5.0/pydbase/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5144 2024-04-02 05:00:59.000000 pydbase-1.5.0/pydbase/dbutils.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.902492 pydbase-1.5.0/pydbase/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)    30170 2024-04-02 05:33:18.000000 pydbase-1.5.0/pydbase/docs/twinbase.html
--rw-r--r--   0 peterglen  (1000) users      (100)    46450 2024-04-02 05:33:17.000000 pydbase-1.5.0/pydbase/docs/twinchain.html
--rw-r--r--   0 peterglen  (1000) users      (100)   143801 2024-04-02 05:33:18.000000 pydbase-1.5.0/pydbase/docs/twincore.html
--rw-rw-r--   0 peterglen  (1000) users      (100)     3453 2024-04-01 01:42:37.000000 pydbase-1.5.0/pydbase/portalocker.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6495 2024-04-01 05:05:24.000000 pydbase-1.5.0/pydbase/twinbase.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    12457 2024-04-02 05:05:37.000000 pydbase-1.5.0/pydbase/twinchain.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    47269 2024-04-02 05:16:26.000000 pydbase-1.5.0/pydbase/twincore.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.914493 pydbase-1.5.0/pydbase.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)    14848 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)      876 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       76 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/entry_points.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/top_level.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-02 05:36:08.914493 pydbase-1.5.0/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     1926 2024-04-02 05:31:14.000000 pydbase-1.5.0/setup.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.914493 pydbase-1.5.0/tests/
--rw-rw-r--   0 peterglen  (1000) users      (100)     1436 2024-04-01 04:09:23.000000 pydbase-1.5.0/tests/test_acreate.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1470 2024-04-01 08:57:38.000000 pydbase-1.5.0/tests/test_bigdata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1399 2024-04-01 07:47:06.000000 pydbase-1.5.0/tests/test_bindata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1497 2024-03-07 15:25:35.000000 pydbase-1.5.0/tests/test_chain.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     2046 2024-04-01 02:59:49.000000 pydbase-1.5.0/tests/test_chain_data.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     2333 2024-04-01 03:03:51.000000 pydbase-1.5.0/tests/test_chain_link.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1189 2024-02-28 03:53:28.000000 pydbase-1.5.0/tests/test_del.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1273 2024-02-28 03:53:43.000000 pydbase-1.5.0/tests/test_dump.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1305 2024-04-01 04:15:24.000000 pydbase-1.5.0/tests/test_find.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1310 2024-04-01 04:09:03.000000 pydbase-1.5.0/tests/test_findrec.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1385 2024-04-01 04:21:29.000000 pydbase-1.5.0/tests/test_getoffs.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1567 2024-02-28 04:02:31.000000 pydbase-1.5.0/tests/test_getrec.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1931 2024-04-01 04:17:37.000000 pydbase-1.5.0/tests/test_handles.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1471 2024-04-01 04:18:57.000000 pydbase-1.5.0/tests/test_inplace.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1108 2024-04-01 04:23:28.000000 pydbase-1.5.0/tests/test_integrity.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1574 2024-04-01 04:20:53.000000 pydbase-1.5.0/tests/test_list.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1541 2024-03-10 04:45:43.000000 pydbase-1.5.0/tests/test_lockrel.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1799 2024-04-02 05:26:52.000000 pydbase-1.5.0/tests/test_multi.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1927 2024-02-28 04:05:14.000000 pydbase-1.5.0/tests/test_packer.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1654 2024-04-01 09:10:20.000000 pydbase-1.5.0/tests/test_reindex.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1503 2024-04-01 04:22:41.000000 pydbase-1.5.0/tests/test_search.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1676 2024-04-01 03:36:26.000000 pydbase-1.5.0/tests/test_vacuum.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.782636 pydbase-1.5.2/
+-rw-r--r--   0 peterglen  (1000) users      (100)    15090 2024-04-10 07:28:05.778636 pydbase-1.5.2/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14676 2024-04-10 04:30:09.000000 pydbase-1.5.2/README.md
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     7868 2024-04-10 04:06:28.000000 pydbase-1.5.2/chainadm.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    10564 2024-04-10 05:43:45.000000 pydbase-1.5.2/dbaseadm.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.762635 pydbase-1.5.2/man/
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.766635 pydbase-1.5.2/man/man1/
+-rwxrwxr--   0 peterglen  (1000) users      (100)     4965 2024-04-10 05:42:53.000000 pydbase-1.5.2/man/man1/pydbase.1
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.766635 pydbase-1.5.2/pydbase/
+-rwxr-xr-x   0 peterglen  (1000) users      (100)        9 2023-09-25 19:38:11.000000 pydbase-1.5.2/pydbase/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5225 2024-04-10 04:19:06.000000 pydbase-1.5.2/pydbase/dbutils.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.766635 pydbase-1.5.2/pydbase/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    30197 2024-04-09 10:03:09.000000 pydbase-1.5.2/pydbase/docs/twinbase.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    47882 2024-04-09 10:03:08.000000 pydbase-1.5.2/pydbase/docs/twinchain.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   143863 2024-04-09 10:03:09.000000 pydbase-1.5.2/pydbase/docs/twincore.html
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3453 2024-04-01 01:42:37.000000 pydbase-1.5.2/pydbase/portalocker.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6514 2024-04-09 09:24:34.000000 pydbase-1.5.2/pydbase/twinbase.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    12981 2024-04-07 03:32:50.000000 pydbase-1.5.2/pydbase/twinchain.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    47418 2024-04-10 04:19:44.000000 pydbase-1.5.2/pydbase/twincore.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.778636 pydbase-1.5.2/pydbase.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)    15090 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)      895 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       76 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/entry_points.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-04-10 07:28:05.000000 pydbase-1.5.2/pydbase.egg-info/top_level.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-10 07:28:05.782636 pydbase-1.5.2/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2335 2024-04-09 10:17:21.000000 pydbase-1.5.2/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 07:28:05.778636 pydbase-1.5.2/tests/
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1436 2024-04-01 04:09:23.000000 pydbase-1.5.2/tests/test_acreate.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1470 2024-04-01 08:57:38.000000 pydbase-1.5.2/tests/test_bigdata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1399 2024-04-01 07:47:06.000000 pydbase-1.5.2/tests/test_bindata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1497 2024-03-07 15:25:35.000000 pydbase-1.5.2/tests/test_chain.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2045 2024-04-10 04:00:21.000000 pydbase-1.5.2/tests/test_chain_data.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2350 2024-04-10 04:12:19.000000 pydbase-1.5.2/tests/test_chain_link.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1189 2024-02-28 03:53:28.000000 pydbase-1.5.2/tests/test_del.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1273 2024-02-28 03:53:43.000000 pydbase-1.5.2/tests/test_dump.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1305 2024-04-01 04:15:24.000000 pydbase-1.5.2/tests/test_find.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1310 2024-04-01 04:09:03.000000 pydbase-1.5.2/tests/test_findrec.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1385 2024-04-01 04:21:29.000000 pydbase-1.5.2/tests/test_getoffs.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1567 2024-02-28 04:02:31.000000 pydbase-1.5.2/tests/test_getrec.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1931 2024-04-01 04:17:37.000000 pydbase-1.5.2/tests/test_handles.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1471 2024-04-01 04:18:57.000000 pydbase-1.5.2/tests/test_inplace.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1108 2024-04-01 04:23:28.000000 pydbase-1.5.2/tests/test_integrity.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1574 2024-04-01 04:20:53.000000 pydbase-1.5.2/tests/test_list.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1541 2024-03-10 04:45:43.000000 pydbase-1.5.2/tests/test_lockrel.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1799 2024-04-02 05:26:52.000000 pydbase-1.5.2/tests/test_multi.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1927 2024-02-28 04:05:14.000000 pydbase-1.5.2/tests/test_packer.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1654 2024-04-01 09:10:20.000000 pydbase-1.5.2/tests/test_reindex.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1503 2024-04-01 04:22:41.000000 pydbase-1.5.2/tests/test_search.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1676 2024-04-01 03:36:26.000000 pydbase-1.5.2/tests/test_vacuum.py
```

### Comparing `pydbase-1.5.0/PKG-INFO` & `pydbase-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbase
-Version: 1.5.0
+Version: 1.5.2
 Summary: High speed database with key / data in python.
 Home-page: https://github.com/pglen/pydbase
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,38 +18,29 @@
 #### see: blockchain functions at the end
 
  &nbsp; The motivation was to create a no frills way of saving / retrieving data.
 It is fast, and the time test shows that this is an order of magnitude
 faster than most mainstream databases. This is due to the engine's simplicity.
 It avoids expensive computations in favor of quickly saving data.
 
-### Fast data save / retrieve 
+### Fast data save / retrieve
 
  &nbsp; Mostly ready for production. All tests pass. Please use caution, as this is new.
 The command line tester can drive most aspects of this API; and it is somewhat
 complete. It is also  good way to see the API / Module in action.
 
 ## API
 
   &nbsp; The module 'twincore' uses two data files and a lock file. The file
  names are generated from the base name of the data file;
 name.pydb for data; name.pidx for the index, name.lock for the lock file.
  In case of frozen process the lock file times out in xx seconds
 and breaks the lock. If the locking process (id in lockfile) does
 not exist, the lock breaks immediately.
 
-### Setting verbosity and debug level:
-
-    twincore.core_quiet   = quiet
-    twincore.core_verbose = verbose
-    twincore.core_pgdebug = pgdebug
-    twincore.core_showdel = sdelx
-
- (Setting before data creation will display mesages from the construtor)
-
 Example DB creation:
 
     core = twincore.TwinCore(datafile_name)
 
 Some basic ops:
 
     dbsize = core.getdbsize()
@@ -62,14 +53,22 @@
 
     core = twinchain.TwinChain(datafile_name)
     core.append(keyx, datax)
     recnum = core.getdbsize()
     rec = core.get_payload(recnum)
     print(recnum, rec)
 
+### Setting verbosity and debug level:
+
+    twincore.core_quiet   = quiet
+    twincore.core_verbose = verbose
+    twincore.core_pgdebug = pgdebug
+
+ (Setting before data creation will display mesages from the construtor)
+
 ### Structure of the data:
 
     32 byte header, starting with FILESIG
 
     4 bytes    4 bytes          4 bytes         Variable
     ------------------------------------------------------------
     RECSIG     Hash_of_key      Len_of_key      DATA_for_key
@@ -170,33 +169,36 @@
     user	0m0.154s
     sys	0m0.071s
     sqlite time test, writing 500 records ...
     real	0m1.465s
     user	0m0.130s
     sys	0m0.292s
 
-  Please mind the fact that the sqlite engine has to do a lot of parsing which we
+  Please note that the sqlite engine has to do a lot of parsing which we
 skip doing; That is why pydbase is more than an order of magnitude faster ...
 even with all the hashing for data integrity check
 
 ### Saving more complex data
 
   The database saves a key / value pair. However, the key can be mutated
 to contain more sophisticated data. For example: adding a string in front of it.
 [ Like: the string CUST_ for customer data / details]. Also the key can be made
 unique by adding a UUID to it, or using pyvpacker to construct it. (see below)
 
-  The data may consist of any text / binary. The library pyvpacker and can pack any data
-into a string; It is installed as a dependency, and a copy of pyvpacker can be
-obtained from pip or github.
+ &nbsp; The data may consist of any text / binary. The library pyvpacker and can pack
+any data into a string; It is installed as a dependency, and a copy of
+pyvpacker can be obtained from pip or github.
 
-## pyvpacker.py
+## the pyvpacker.py module:
 
- This module can pack arbitrary python data into a string; which can be used to store
-anything in the pydbase's key / data sections.
+ This module can pack arbitrary python data into a string; which can be
+used to store anything in the pydbase's key / data sections. Note that
+data type is limited to the python native data types and compounds thereof.
+
+        Types: (int, real, str, array, hash)
 
 Example from running testpacker.py:
 
     org: (1, 2, 'aa', ['bb', b'dd'])
     packed: pg s4 'iisa' i4 1 i4 2 s2 'aa' a29 'pg s2 'sb' s2 'bb' b4 'ZGQ=' '
     unpacked: [1, 2, 'aa', ['bb', b'dd']]
     rec_arr: pg s4 'iisa' i4 1 i4 2 s2 'aa' a29 'pg s2 'sb' s2 'bb' b4 'ZGQ=' '
@@ -241,17 +243,17 @@
 this same key, except the last one.
 
 ## Blockchain implementation
 
    The database is extended with a blockhcain implementation. The new class
 is called twinchain; and it is a class derived from twincore.
 
-  To drive the blockchain, just use the append method. Th database will calculate
+  To drive the blockchain, just use the append method. The database will calculate
 all the hashes, integrate it into the existing chain with the new item getting
-a backlink field. This field is calulated based upon the previous record's
+a backlink field. This field is calculated based upon the previous record's
 hash and the previous record's frozen date. This assures that identical data
 will have a different hash, so data cannot be anticipated based upon its hash
 alone. The hash is done with 256 bits, and assumed to be very secure.
 
 To drive it:
 
         core = twinchain.TwinChain()    # Takes an optional file name
@@ -271,23 +273,14 @@
     The hashed sum of fields saved to the next backlink.
 
 ## Integrity check
 
    Two levels; Level one is checking if the record checksums are correct;
    Level two checks if the linkage is correct.
 
-### TODO
-
-    Speed this up by implementing this as a 'C' module
-
-## PyTest
-
- The pytest passes with no errors;
- The following (and more) test are created / executed:
-
 ## The in-place update
 
   The save operation has a flag for in-place update. This is useful for updating
 without the data storage extending. Useful for counts and timers. The in-place
 update operates as a record overwrite, and has to be equal length than the existing
 record. If shorter, the record is padded to the original data's length by appending
 spaces. Below is an example to update a counter in the database, which will execute
@@ -297,62 +290,66 @@
     rec = dbcore.get_rec(xxx)
     # Increment count:
     arr = self.packer.decode_data(rec[1])[0]
     arr[0] = "%05d" % (int(arr[0]) + 1)
     strx = str(self.packer.encode_data("", arr))
     ret = dbcore.save_data(rec[0], strx, True)
 
- If the in-place data is longer, a new record is created, just like a normal
-operation. This new, longer record than accommodates all the new in-place requests.
+ If the new data (relativeto the in-place data) is longer, a new record is
+created, just like a normal operation. This new, longer record than accommodates all the new in-place requests.
 It is recommended that one produces a fixed record size for consistent results.
 (See: sprintf (python % operator) in the example above.)
 
+## PyTest
+
+ The pytest passes with no errors;
+ The following (and more) test are created / executed:
+
 ### Test results:
 
     ============================= test session starts ==============================
     platform linux -- Python 3.10.12, pytest-7.4.3, pluggy-1.0.0
     rootdir: /home/peterglen/pgpygtk/pydbase
-    collected 43 items
+    collected 44 items
 
-    test_acreate.py .....                                                    [ 11%]
-    test_bindata.py .                                                        [ 13%]
-    test_chain.py .                                                          [ 16%]
-    test_chain_integ.py ..                                                   [ 20%]
-    test_chain_link.py ..                                                    [ 25%]
-    test_del.py .                                                            [ 27%]
-    test_dump.py .                                                           [ 30%]
-    test_find.py ..                                                          [ 34%]
-    test_findrec.py ..                                                       [ 39%]
-    test_getoffs.py ...                                                      [ 46%]
-    test_getrec.py .                                                         [ 48%]
-    test_inplace.py ...                                                      [ 55%]
-    test_integrity.py .                                                      [ 58%]
-    test_list.py ..                                                          [ 62%]
-    test_lockrel.py ..                                                       [ 67%]
-    test_multi.py ..                                                         [ 72%]
-    test_packer.py ......                                                    [ 86%]
-    test_randdata.py .                                                       [ 88%]
+    test_acreate.py ...                                                      [  6%]
+    test_bigdata.py .                                                        [  9%]
+    test_bindata.py .                                                        [ 11%]
+    test_chain.py .                                                          [ 13%]
+    test_chain_data.py .                                                     [ 15%]
+    test_chain_link.py ..                                                    [ 20%]
+    test_del.py .                                                            [ 22%]
+    test_dump.py .                                                           [ 25%]
+    test_find.py ..                                                          [ 29%]
+    test_findrec.py ..                                                       [ 34%]
+    test_getoffs.py ...                                                      [ 40%]
+    test_getrec.py .                                                         [ 43%]
+    test_handles.py .....                                                    [ 54%]
+    test_inplace.py ...                                                      [ 61%]
+    test_integrity.py .                                                      [ 63%]
+    test_list.py ..                                                          [ 68%]
+    test_lockrel.py .                                                        [ 70%]
+    test_multi.py ..                                                         [ 75%]
+    test_packer.py ......                                                    [ 88%]
     test_reindex.py .                                                        [ 90%]
     test_search.py ...                                                       [ 97%]
     test_vacuum.py .                                                         [100%]
 
-    ============================== 43 passed in 0.68s ==============================
+    ============================== 44 passed in 0.57s ==============================
 
 ## History
 
     1.1         Tue 20.Feb.2024     Initial release
     1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
     1.4.0       Tue 27.Feb.2024     Addedd pgdebug
     1.4.2       Wed 28.Feb.2024     Fixed multiple instances
     1.4.3       Wed 28.Feb.2024     ChainAdm added
     1.4.4       Fri 01.Mar.2024     Tests for chain functions
     1.4.5       Fri 01.Mar.2024     Misc fixes
     1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
     1.4.7       Tue 05.Mar.2024     In place record update
     1.4.8       Sat 09.Mar.2024     Added new locking mechanism
-
-## Errata
-
-    Chain is still in development, most of it functions well.
-    Not for production.
+    1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
+    1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
+    1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
 
 // EOF
```

### Comparing `pydbase-1.5.0/README.md` & `pydbase-1.5.2/pydbase.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,46 @@
+Metadata-Version: 2.1
+Name: pydbase
+Version: 1.5.2
+Summary: High speed database with key / data in python.
+Home-page: https://github.com/pglen/pydbase
+Author: Peter Glen
+Author-email: peterglen99@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+
 # pydbase
 
 ## High speed database with key / data
 
 #### see: blockchain functions at the end
 
  &nbsp; The motivation was to create a no frills way of saving / retrieving data.
 It is fast, and the time test shows that this is an order of magnitude
 faster than most mainstream databases. This is due to the engine's simplicity.
 It avoids expensive computations in favor of quickly saving data.
 
-### Fast data save / retrieve 
+### Fast data save / retrieve
 
  &nbsp; Mostly ready for production. All tests pass. Please use caution, as this is new.
 The command line tester can drive most aspects of this API; and it is somewhat
 complete. It is also  good way to see the API / Module in action.
 
 ## API
 
   &nbsp; The module 'twincore' uses two data files and a lock file. The file
  names are generated from the base name of the data file;
 name.pydb for data; name.pidx for the index, name.lock for the lock file.
  In case of frozen process the lock file times out in xx seconds
 and breaks the lock. If the locking process (id in lockfile) does
 not exist, the lock breaks immediately.
 
-### Setting verbosity and debug level:
-
-    twincore.core_quiet   = quiet
-    twincore.core_verbose = verbose
-    twincore.core_pgdebug = pgdebug
-    twincore.core_showdel = sdelx
-
- (Setting before data creation will display mesages from the construtor)
-
 Example DB creation:
 
     core = twincore.TwinCore(datafile_name)
 
 Some basic ops:
 
     dbsize = core.getdbsize()
@@ -49,14 +53,22 @@
 
     core = twinchain.TwinChain(datafile_name)
     core.append(keyx, datax)
     recnum = core.getdbsize()
     rec = core.get_payload(recnum)
     print(recnum, rec)
 
+### Setting verbosity and debug level:
+
+    twincore.core_quiet   = quiet
+    twincore.core_verbose = verbose
+    twincore.core_pgdebug = pgdebug
+
+ (Setting before data creation will display mesages from the construtor)
+
 ### Structure of the data:
 
     32 byte header, starting with FILESIG
 
     4 bytes    4 bytes          4 bytes         Variable
     ------------------------------------------------------------
     RECSIG     Hash_of_key      Len_of_key      DATA_for_key
@@ -157,33 +169,36 @@
     user	0m0.154s
     sys	0m0.071s
     sqlite time test, writing 500 records ...
     real	0m1.465s
     user	0m0.130s
     sys	0m0.292s
 
-  Please mind the fact that the sqlite engine has to do a lot of parsing which we
+  Please note that the sqlite engine has to do a lot of parsing which we
 skip doing; That is why pydbase is more than an order of magnitude faster ...
 even with all the hashing for data integrity check
 
 ### Saving more complex data
 
   The database saves a key / value pair. However, the key can be mutated
 to contain more sophisticated data. For example: adding a string in front of it.
 [ Like: the string CUST_ for customer data / details]. Also the key can be made
 unique by adding a UUID to it, or using pyvpacker to construct it. (see below)
 
-  The data may consist of any text / binary. The library pyvpacker and can pack any data
-into a string; It is installed as a dependency, and a copy of pyvpacker can be
-obtained from pip or github.
+ &nbsp; The data may consist of any text / binary. The library pyvpacker and can pack
+any data into a string; It is installed as a dependency, and a copy of
+pyvpacker can be obtained from pip or github.
+
+## the pyvpacker.py module:
 
-## pyvpacker.py
+ This module can pack arbitrary python data into a string; which can be
+used to store anything in the pydbase's key / data sections. Note that
+data type is limited to the python native data types and compounds thereof.
 
- This module can pack arbitrary python data into a string; which can be used to store
-anything in the pydbase's key / data sections.
+        Types: (int, real, str, array, hash)
 
 Example from running testpacker.py:
 
     org: (1, 2, 'aa', ['bb', b'dd'])
     packed: pg s4 'iisa' i4 1 i4 2 s2 'aa' a29 'pg s2 'sb' s2 'bb' b4 'ZGQ=' '
     unpacked: [1, 2, 'aa', ['bb', b'dd']]
     rec_arr: pg s4 'iisa' i4 1 i4 2 s2 'aa' a29 'pg s2 'sb' s2 'bb' b4 'ZGQ=' '
@@ -228,17 +243,17 @@
 this same key, except the last one.
 
 ## Blockchain implementation
 
    The database is extended with a blockhcain implementation. The new class
 is called twinchain; and it is a class derived from twincore.
 
-  To drive the blockchain, just use the append method. Th database will calculate
+  To drive the blockchain, just use the append method. The database will calculate
 all the hashes, integrate it into the existing chain with the new item getting
-a backlink field. This field is calulated based upon the previous record's
+a backlink field. This field is calculated based upon the previous record's
 hash and the previous record's frozen date. This assures that identical data
 will have a different hash, so data cannot be anticipated based upon its hash
 alone. The hash is done with 256 bits, and assumed to be very secure.
 
 To drive it:
 
         core = twinchain.TwinChain()    # Takes an optional file name
@@ -258,23 +273,14 @@
     The hashed sum of fields saved to the next backlink.
 
 ## Integrity check
 
    Two levels; Level one is checking if the record checksums are correct;
    Level two checks if the linkage is correct.
 
-### TODO
-
-    Speed this up by implementing this as a 'C' module
-
-## PyTest
-
- The pytest passes with no errors;
- The following (and more) test are created / executed:
-
 ## The in-place update
 
   The save operation has a flag for in-place update. This is useful for updating
 without the data storage extending. Useful for counts and timers. The in-place
 update operates as a record overwrite, and has to be equal length than the existing
 record. If shorter, the record is padded to the original data's length by appending
 spaces. Below is an example to update a counter in the database, which will execute
@@ -284,62 +290,66 @@
     rec = dbcore.get_rec(xxx)
     # Increment count:
     arr = self.packer.decode_data(rec[1])[0]
     arr[0] = "%05d" % (int(arr[0]) + 1)
     strx = str(self.packer.encode_data("", arr))
     ret = dbcore.save_data(rec[0], strx, True)
 
- If the in-place data is longer, a new record is created, just like a normal
-operation. This new, longer record than accommodates all the new in-place requests.
+ If the new data (relativeto the in-place data) is longer, a new record is
+created, just like a normal operation. This new, longer record than accommodates all the new in-place requests.
 It is recommended that one produces a fixed record size for consistent results.
 (See: sprintf (python % operator) in the example above.)
 
+## PyTest
+
+ The pytest passes with no errors;
+ The following (and more) test are created / executed:
+
 ### Test results:
 
     ============================= test session starts ==============================
     platform linux -- Python 3.10.12, pytest-7.4.3, pluggy-1.0.0
     rootdir: /home/peterglen/pgpygtk/pydbase
-    collected 43 items
+    collected 44 items
 
-    test_acreate.py .....                                                    [ 11%]
-    test_bindata.py .                                                        [ 13%]
-    test_chain.py .                                                          [ 16%]
-    test_chain_integ.py ..                                                   [ 20%]
-    test_chain_link.py ..                                                    [ 25%]
-    test_del.py .                                                            [ 27%]
-    test_dump.py .                                                           [ 30%]
-    test_find.py ..                                                          [ 34%]
-    test_findrec.py ..                                                       [ 39%]
-    test_getoffs.py ...                                                      [ 46%]
-    test_getrec.py .                                                         [ 48%]
-    test_inplace.py ...                                                      [ 55%]
-    test_integrity.py .                                                      [ 58%]
-    test_list.py ..                                                          [ 62%]
-    test_lockrel.py ..                                                       [ 67%]
-    test_multi.py ..                                                         [ 72%]
-    test_packer.py ......                                                    [ 86%]
-    test_randdata.py .                                                       [ 88%]
+    test_acreate.py ...                                                      [  6%]
+    test_bigdata.py .                                                        [  9%]
+    test_bindata.py .                                                        [ 11%]
+    test_chain.py .                                                          [ 13%]
+    test_chain_data.py .                                                     [ 15%]
+    test_chain_link.py ..                                                    [ 20%]
+    test_del.py .                                                            [ 22%]
+    test_dump.py .                                                           [ 25%]
+    test_find.py ..                                                          [ 29%]
+    test_findrec.py ..                                                       [ 34%]
+    test_getoffs.py ...                                                      [ 40%]
+    test_getrec.py .                                                         [ 43%]
+    test_handles.py .....                                                    [ 54%]
+    test_inplace.py ...                                                      [ 61%]
+    test_integrity.py .                                                      [ 63%]
+    test_list.py ..                                                          [ 68%]
+    test_lockrel.py .                                                        [ 70%]
+    test_multi.py ..                                                         [ 75%]
+    test_packer.py ......                                                    [ 88%]
     test_reindex.py .                                                        [ 90%]
     test_search.py ...                                                       [ 97%]
     test_vacuum.py .                                                         [100%]
 
-    ============================== 43 passed in 0.68s ==============================
+    ============================== 44 passed in 0.57s ==============================
 
 ## History
 
     1.1         Tue 20.Feb.2024     Initial release
     1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
     1.4.0       Tue 27.Feb.2024     Addedd pgdebug
     1.4.2       Wed 28.Feb.2024     Fixed multiple instances
     1.4.3       Wed 28.Feb.2024     ChainAdm added
     1.4.4       Fri 01.Mar.2024     Tests for chain functions
     1.4.5       Fri 01.Mar.2024     Misc fixes
     1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
     1.4.7       Tue 05.Mar.2024     In place record update
     1.4.8       Sat 09.Mar.2024     Added new locking mechanism
-
-## Errata
-
-    Chain is still in development, most of it functions well.
-    Not for production.
+    1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
+    1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
+    1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
 
 // EOF
```

### Comparing `pydbase-1.5.0/chainadm.py` & `pydbase-1.5.2/chainadm.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,30 +148,29 @@
 
     #print("Use: pychain.py -h to see options and help")
 
 def execfunc():
 
     ''' Execute individual function from command line '''
 
-
     # Create our database
     core = twinchain.TwinChain(_c.deffile, _c.pgdebug, _c.verbose)
 
     core.base_quiet     = _c.quiet
     core.base_pgdebug   = _c.pgdebug
     core.base_showdel   = _c.sdelx
     core.base_integrity = _c.checkx
     core.base_pgdebug   = _c.pgdebug
 
     if _c.integx:
         #print("Integrity", _c.integx)
         errx = False; cnt = []
         sss = core.getdbsize()
         # Remember record zero is the anchor
-        for aa in range(1, sss):
+        for aa in range(0, sss):
             ppp = core.linkintegrity(aa)
             if _c.verbose:
                 print(aa, ppp)
             if not ppp: errx = True; cnt.append(aa)
         if errx:
             print("error on rec", cnt)
         else:
```

### Comparing `pydbase-1.5.0/dbaseadm.py` & `pydbase-1.5.2/dbaseadm.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,42 +12,34 @@
 _ = gettext.gettext
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base, 'pydbase'))
 
 from pydbase import twincore
 
+#print(sys.prefix)
+
 # ------------------------------------------------------------------------
 
 gl_lockname = "pydbase.main.lock"
 
 # Module variables (pushed to a class)
 
 class _m():
-    pgdebug = 0
-    verbose = 0
-    keyonly = 0
-    ncount  = 1
-    skipcnt = 0
-    maxx    = 1; maxdel = 0xffffffff
+    pgdebug = 0;  verbose = 0
+    keyonly = 0;  ncount  = 1
+    skipcnt = 0;  maxdel = 0xffffffff
     lcount  = twincore.INT_MAX
-    quiet   = 0; writex  = 0
-    randx   = 0; skipx   = 0
-    offsx   = 0; delx    = 0
-    delrx   = 0; delrx2  = 0
-    backx   = 0; sdelx   = 0
-    vacx    = 0; recx    = 0
-    integx  = 0; checkx  = 0
-    sizex   = 0; findx   = ""
-    retrx   = ""; getit  = ""
-    keyx    = ""; datax  = ""
-    dkeyx   = ""; dumpx  = 0
-    findrec = ""; getrec = 0
-    replace = 0 ; recpos = 0
-    inplace = 0
+    quiet   = 0; writex  = 0;   randx   = 0; skipx   = 0
+    offsx   = 0; delx    = 0;   delrx   = 0; delrx2  = 0
+    backx   = 0; sdelx   = 0;   vacx    = 0; recx    = 0
+    integx  = 0; checkx  = 0;   sizex   = 0; findx   = ""
+    retrx   = ""; getit  = "";  keyx    = ""; datax  = ""
+    dkeyx   = ""; dumpx  = 0;   findrec = ""; getrec = 0
+    replace = 0 ; recpos = 0;   inplace = 0
     deffile = "pydbase.pydb"
 
 version = "0.4.1"
 vdate   = "Fri 01.Mar.2024"
 allstr  =    " " + \
                 string.ascii_lowercase +  string.ascii_uppercase +  \
                     string.digits
@@ -62,39 +54,45 @@
     strx = ""
     for aa in range(lenx):
         ridx = random.randint(0, len(allstr)-1)
         rr = allstr[ridx]
         strx += str(rr)
     return strx
 
+pname = os.path.split(sys.argv[0])[1]
+
+__doc__ = ''' \
+Usage: %s [options] [arg_key arg_data]
+   -h         Help (this screen)   -|-  -E         Replace record in place
+   -V         Print version        -|-  -q         Quiet on, less printing
+   -d         Debug level (0-10)   -|-  -v         Increment verbosity level
+   -r         Randomize (with -w)  -|-  -w         Write random record(s)
+   -z         Dump backwards(s)    -|-  -i         Show deleted record(s)
+   -U         Vacuum DB            -|-  -R         Re-index / recover DB
+   -I         DB Integrity check   -|-  -c         Set check integrity flag
+   -s         Skip to count recs   -|-  -K         List keys only
+   -S         Print num recs       -|-  -m         Dump data to console
+   -n  num    Num of recs (with -w)-|-  -t  keyval Retrieve by key
+   -o  offs   Get data from offset -|-  -G  num    Get record by number
+   -F  subkey Find by sub str      -|-  -g  num    Get number of recs.
+   -k  keyval Key to save          -|-  -a  str    Data to save
+   -y  keyval Find by key          -|-  -D  keyval Delete by key
+   -p  num    Skip number of recs  -|-  -u  recnum Delete at recnum
+   -l  lim    Limit get records    -|-  -e  offs   Delete at offset
+   -Z  keyval Get record position  -|-  -X  max    Limit recs on delete
+   -f  file   DB file for save/retrieve default: 'pydbase.pydb')
+The verbosity / debug  level influences the amount of printout presented.
+Use quotes for multi word arguments.''' \
+     % (pname)
+
 def help():
-    ''' Program usage information '''
 
-    pname = os.path.split(sys.argv[0])[1]
-    print("Usage: %s [options] [arg_key arg_data]" %  pname)
-    print("   -h         Help (this screen)   -|-  -E         Replace record in place")
-    print("   -V         Print version        -|-  -q         Quiet on, less printing")
-    print("   -d         Debug level (0-10)   -|-  -v         Increment verbosity level")
-    print("   -r         Randomize data       -|-  -w         Write random record(s)")
-    print("   -z         Dump backwards(s)    -|-  -i         Show deleted record(s)")
-    print("   -U         Vacuum DB            -|-  -R         Re-index / recover DB")
-    print("   -I         DB Integrity check   -|-  -c         Set check integrity flag")
-    print("   -s         Skip to count recs   -|-  -K         List keys only")
-    print("   -S         Print num recs       -|-  -m         Dump data to console")
-    print("   -o  offs   Get data from offset -|-  -G  num    Get record by number ")
-    print("   -F  subkey Find by sub str      -|-  -g  num    Get number of recs.")
-    print("   -k  keyval Key to save          -|-  -a  str    Data to save ")
-    print("   -y  keyval Find by key          -|-  -D  keyval Delete by key ")
-    print("   -n  num    Number of records    -|-  -t  keyval Retrieve by key")
-    print("   -p  num    Skip number of recs  -|-  -u  recnum Delete at recnum")
-    print("   -l  lim    Limit get records    -|-  -e  offs   Delete at offset")
-    print("   -Z  keyval Get record position  -|-  -X  max    Limit recs on delete ")
-    print("   -f  file   DB file for save/retrieve default: 'pydbase.pydb')")
-    print("The verbosity / debug  level influences the amount of data presented.")
-    print("Use quotes for multi word arguments.")
+    ''' Program usage information '''
+    print(__doc__)
+    sys.exit(0)
 
 def mainfunc():
 
     ''' Exercise most / all functions of the twincore library '''
 
     opts = []; args = []
 
@@ -143,16 +141,14 @@
             _m.quiet = True
         if aa[0] == "-n":
             _m.ncount = int(aa[1])
         if aa[0] == "-t":
             _m.retrx = aa[1]
         if aa[0] == "-l":
             _m.lcount = int(aa[1])
-        if aa[0] == "-x":
-            _m.maxx = int(aa[1])
         if aa[0] == "-X":
             _m.maxdel = int(aa[1])
         if aa[0] == "-s":
             _m.skipcnt = int(aa[1])
         if aa[0] == "-f":
             _m.deffile = aa[1]
         if aa[0] == "-g":
@@ -219,17 +215,14 @@
     if len(args) == 2:
         #print("args", args)
         curr = core.save_data(args[0], args[1])
         sys.exit(0)
 
     #print(dir(core))
 
-    # Correct maxx
-    if _m.maxx <= 0 : _m.maxx = 1
-
     dbsize = core.getdbsize()
     #print("DBsize", dbsize)
 
     if _m.keyx and _m.datax:
         curr = 0
         if _m.verbose:
             print("adding", _m.keyx, _m.datax)
```

### Comparing `pydbase-1.5.0/pydbase/dbutils.py` & `pydbase-1.5.2/pydbase/dbutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         if fcntl:
             try:
                 self.fpx = open(lockname, "wb")
             except:
                 if utils_pgdebug > 1:
                     print("Cannot create lock file")
 
-                raise ValuError("Cannot create lock file")
+                raise ValueError("Cannot create lock file")
 
     def waitlock(self):
         if utils_pgdebug > 1:
             print("Waitlock", self.lockname)
         if fcntl:
             cnt2 = 0
             while True:
@@ -159,16 +159,18 @@
                     print("unlock", self.lockname, sys.exc_info())
 
     def __del__(self):
 
         #print("__del__ lock", self.lockname)
         try:
             if fcntl:
-                # Do not remove, others may have locked it
+                # Do not remove, others may have locked it ...
+                # ... but close our handle
                 fcntl.flock(self.fpx, fcntl.LOCK_UN | fcntl.LOCK_NB)
+                self.fpx.close()
                 pass
 
             # Always remove file
             try:
                 os.remove(self.lockname)
             except:
                 pass
```

### Comparing `pydbase-1.5.0/pydbase/docs/twinbase.html` & `pydbase-1.5.2/pydbase/docs/twinbase.html`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 FILESIG     = b&#34;PYDB&#34;
 IDXSIG      = b&#34;PYIX&#34;
 RECSIG      = b&#34;RECB&#34;
 RECDEL      = b&#34;RECX&#34;
 RECSEP      = b&#34;RECS&#34;
 RECEND      = b&#34;RECE&#34;
 
+version = &#34;1.5.2&#34;
+
 # Accessed from the main file as well
 
 base_locktout   = LOCK_TIMEOUT   # Settable from ...
 base_pgdebug    = 0
 base_quiet      = 0
 base_integrity  = 0
 base_showdel    = 0
```

#### html2text {}

```diff
@@ -34,14 +34,16 @@
 FILESIG     = b"PYDB"
 IDXSIG      = b"PYIX"
 RECSIG      = b"RECB"
 RECDEL      = b"RECX"
 RECSEP      = b"RECS"
 RECEND      = b"RECE"
 
+version = "1.5.2"
+
 # Accessed from the main file as well
 
 base_locktout   = LOCK_TIMEOUT   # Settable from ...
 base_pgdebug    = 0
 base_quiet      = 0
 base_integrity  = 0
 base_showdel    = 0
```

### Comparing `pydbase-1.5.0/pydbase/docs/twinchain.html` & `pydbase-1.5.2/pydbase/docs/twinchain.html`

 * *Files 2% similar despite different names*

```diff
@@ -126,37 +126,46 @@
         ulockname = os.path.splitext(fname)[0] + &#34;.ulock&#34;
         self.ulock = FileLock(ulockname)
         self.ulock.waitlock()    #(self.ulockname)
 
         super(TwinChain, self).__init__(fname, pgdebug)
 
         self.packer = pyvpacker.packbin()
-        sss = self.getdbsize()
-        if sss == 0:
-            payload = {&#34;Initial&#34;: &#34;Initial record, do not use.&#34;}
-            #print(&#34;Init anchor record&#34;, payload)
-
-            # Here we fake the initial backlink for the anchor record
-            self.old_dicx = {}
 
+        sss = self.getdbsize()
+        &#39;&#39;&#39;if sss == 0:
             # Produce initial data structure
+            # This is the wron place to produce it, as the chain has no
+            # knowledge of the actual structure ... we provide minimum here
             header = str(uuid.uuid1())
-
             dt = datetime.datetime.utcnow()
             fdt = dt.strftime(&#39;%a, %d %b %Y %H:%M:%S`&#39;)
-            self.old_dicx[&#34;now&#34;] =  fdt
-            self.old_dicx[&#34;hash256&#34;]  =  self._hash_any(payload).hexdigest()
-            self.old_dicx[&#34;header&#34;]   =  header
-            self.old_dicx[&#34;payload&#34;]  =  payload
-            self.old_dicx[&#34;backlink&#34;] =  &#34;&#34;
-
-            aaa = self._fill_record(header, payload)
-            #print(aaa)
-            encoded = self.packer.encode_data(&#34;&#34;, aaa)
+
+            payload = {&#34;Initial&#34;: &#34;Initial record, do not use.&#34;,
+                            &#34;Default&#34; : &#39;None&#39;, &#34;header&#34;: header}
+
+            #payload2 = {&#34;header&#34;: header, &#34;payload&#34; : payload}
+
+            # Here we fake the initial backlink for the anchor record
+            old_dicx = {}
+            old_dicx[&#34;now&#34;] =  fdt
+            old_dicx[&#34;hash256&#34;]  =  self._hash_any(payload).hexdigest()
+            old_dicx[&#34;header&#34;]   =  header
+            old_dicx[&#34;payload&#34;]  =  payload
+            old_dicx[&#34;backlink&#34;] =  &#34;&#34;
+
+            #print(&#34;old_dicx:&#34;, self.old_dicx)
+
+            aaa = self._fill_record(header, payload, old_dicx)
+            #print(&#34;aaa:&#34;, aaa)
+            encoded = self.packer.encode_data(&#34;&#34;, [aaa])
+            #print(&#34;encoded:&#34;, encoded)
+
             self.save_data(header, encoded)
+        &#39;&#39;&#39;
 
         self.ulock.unlock() #self.ulockname)
 
     def _hashtohex(self, varx):
 
         if type(varx) == type(&#34;&#34;):
             varx = varx.encode()
@@ -208,30 +217,30 @@
         backlink += self._expand_dict(dicold.get(&#34;payload&#34;, &#34;&#34;))
         backlink += dicold.get(&#34;backlink&#34;, &#34;&#34;)
         #print(&#34;raw backlink&#34;, backlink)
         return backlink
 
     # --------------------------------------------------------------------
 
-    def _fill_record(self, header, payload):
+    def _fill_record(self, header, payload, old_dict):
 
         aaa = {}
         aaa[&#34;header&#34;] = header
         aaa[&#34;payload&#34;] = payload
         aaa[&#34;protocol&#34;] = ProtocolVersion
 
         dt = datetime.datetime.now()
         fdt = dt.strftime(&#39;%a, %d %b %Y %H:%M:%S&#39;)
         aaa[&#34;now&#34;] = fdt
         #self._key_n_data(aaa, &#34;hash32&#34;, str(self.hash32(payload)))
 
         sumstr = self._build_sumstr(aaa)
         aaa[&#34;hash256&#34;] = self._hashtohex(sumstr)
 
-        backlink = self._build_backlink(self.old_dicx)
+        backlink = self._build_backlink(old_dict)
         aaa[&#34;backlink&#34;] = self._hashtohex(backlink)
 
         return aaa
 
     def get_payload(self, recnum):
 
         &#39;&#39;&#39; Return the payload on record number &#39;&#39;&#39;
@@ -401,40 +410,40 @@
         except:
             if self.core_verbose:
                 print(&#34;Header override must be a valid UUID string.&#34;)
 
             self.ulock.unlock() #self.ulockname)
             raise ValueError(&#34;Header override must be a valid UUID string.&#34;)
 
-        self.old_dicx = {}
+        old_dicx = {}
         # Get last data from db
         sss = self.getdbsize()
         #print(&#34;sss&#34;, sss)
 
+        # We fake an empty set ... checking against an empty set is a valid OP
         if not sss:
-            raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
-
-        ooo = self.get_rec(sss-1)
+            #raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
+            ddd = self.packer.encode_data(&#34;&#34;, {&#34;blank&#34;: 0, })
+            ooo = [0, ddd,]
+        else:
+            ooo = self.get_rec(sss-1)
 
         if self.pgdebug &gt; 5:
             print(&#34;decoding&#34;, ooo)
 
         decoded = self.packer.decode_data(ooo[1])
+        old_dicx = self._get_fields(decoded[0])
 
-        self.old_dicx = self._get_fields(decoded[0])
-
-        #print(&#34;old_fff&#34;, self.old_dicx[&#34;hash256&#34;])
-        #print(&#34;old_time&#34;, self.old_dicx[&#34;now&#34;])
-
-        aaa = self._fill_record(header, datax)
+        #print(&#34;old_fff&#34;, old_dicx[&#34;hash256&#34;])
+        #print(&#34;old_time&#34;, old_dicx[&#34;now&#34;])
 
+        aaa = self._fill_record(header, datax, old_dicx)
         encoded = self.packer.encode_data(&#34;&#34;, aaa)
 
         #print(&#34;save&#34;, header, &#34;-&#34;, encoded)
-
         #print(&#34;bbb&#34;, self.getdbsize())
         self.save_data(header, encoded)
         #print(&#34;eee&#34;, self.getdbsize())
 
         if self.core_verbose &gt; 1:
             bbb = self.packer.decode_data(encoded)
             print(&#34;Rec&#34;, bbb[0])
@@ -446,17 +455,18 @@
 
         &#39;&#39;&#39; Append data to the end of database &#39;&#39;&#39;
 
         if self.core_verbose &gt; 0:
             print(&#34;Append&#34;, datax)
 
         # Get last data from db
-        sss = self.getdbsize()
-        if not sss:
-            raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
+        #sss = self.getdbsize()
+        #if not sss:
+        #    #raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
+        #    pass
 
         # Produce header  structure
         uuu = uuid.uuid1()
         #print(&#34;uuid date&#34;,uuid2date(uuu))
         header = str(uuu)
         uuuu = uuid.UUID(header)
         #print(&#34;uuid date2&#34;, header, uuid2date(uuuu))
@@ -557,37 +567,46 @@
         ulockname = os.path.splitext(fname)[0] + &#34;.ulock&#34;
         self.ulock = FileLock(ulockname)
         self.ulock.waitlock()    #(self.ulockname)
 
         super(TwinChain, self).__init__(fname, pgdebug)
 
         self.packer = pyvpacker.packbin()
-        sss = self.getdbsize()
-        if sss == 0:
-            payload = {&#34;Initial&#34;: &#34;Initial record, do not use.&#34;}
-            #print(&#34;Init anchor record&#34;, payload)
-
-            # Here we fake the initial backlink for the anchor record
-            self.old_dicx = {}
 
+        sss = self.getdbsize()
+        &#39;&#39;&#39;if sss == 0:
             # Produce initial data structure
+            # This is the wron place to produce it, as the chain has no
+            # knowledge of the actual structure ... we provide minimum here
             header = str(uuid.uuid1())
-
             dt = datetime.datetime.utcnow()
             fdt = dt.strftime(&#39;%a, %d %b %Y %H:%M:%S`&#39;)
-            self.old_dicx[&#34;now&#34;] =  fdt
-            self.old_dicx[&#34;hash256&#34;]  =  self._hash_any(payload).hexdigest()
-            self.old_dicx[&#34;header&#34;]   =  header
-            self.old_dicx[&#34;payload&#34;]  =  payload
-            self.old_dicx[&#34;backlink&#34;] =  &#34;&#34;
-
-            aaa = self._fill_record(header, payload)
-            #print(aaa)
-            encoded = self.packer.encode_data(&#34;&#34;, aaa)
+
+            payload = {&#34;Initial&#34;: &#34;Initial record, do not use.&#34;,
+                            &#34;Default&#34; : &#39;None&#39;, &#34;header&#34;: header}
+
+            #payload2 = {&#34;header&#34;: header, &#34;payload&#34; : payload}
+
+            # Here we fake the initial backlink for the anchor record
+            old_dicx = {}
+            old_dicx[&#34;now&#34;] =  fdt
+            old_dicx[&#34;hash256&#34;]  =  self._hash_any(payload).hexdigest()
+            old_dicx[&#34;header&#34;]   =  header
+            old_dicx[&#34;payload&#34;]  =  payload
+            old_dicx[&#34;backlink&#34;] =  &#34;&#34;
+
+            #print(&#34;old_dicx:&#34;, self.old_dicx)
+
+            aaa = self._fill_record(header, payload, old_dicx)
+            #print(&#34;aaa:&#34;, aaa)
+            encoded = self.packer.encode_data(&#34;&#34;, [aaa])
+            #print(&#34;encoded:&#34;, encoded)
+
             self.save_data(header, encoded)
+        &#39;&#39;&#39;
 
         self.ulock.unlock() #self.ulockname)
 
     def _hashtohex(self, varx):
 
         if type(varx) == type(&#34;&#34;):
             varx = varx.encode()
@@ -639,30 +658,30 @@
         backlink += self._expand_dict(dicold.get(&#34;payload&#34;, &#34;&#34;))
         backlink += dicold.get(&#34;backlink&#34;, &#34;&#34;)
         #print(&#34;raw backlink&#34;, backlink)
         return backlink
 
     # --------------------------------------------------------------------
 
-    def _fill_record(self, header, payload):
+    def _fill_record(self, header, payload, old_dict):
 
         aaa = {}
         aaa[&#34;header&#34;] = header
         aaa[&#34;payload&#34;] = payload
         aaa[&#34;protocol&#34;] = ProtocolVersion
 
         dt = datetime.datetime.now()
         fdt = dt.strftime(&#39;%a, %d %b %Y %H:%M:%S&#39;)
         aaa[&#34;now&#34;] = fdt
         #self._key_n_data(aaa, &#34;hash32&#34;, str(self.hash32(payload)))
 
         sumstr = self._build_sumstr(aaa)
         aaa[&#34;hash256&#34;] = self._hashtohex(sumstr)
 
-        backlink = self._build_backlink(self.old_dicx)
+        backlink = self._build_backlink(old_dict)
         aaa[&#34;backlink&#34;] = self._hashtohex(backlink)
 
         return aaa
 
     def get_payload(self, recnum):
 
         &#39;&#39;&#39; Return the payload on record number &#39;&#39;&#39;
@@ -832,40 +851,40 @@
         except:
             if self.core_verbose:
                 print(&#34;Header override must be a valid UUID string.&#34;)
 
             self.ulock.unlock() #self.ulockname)
             raise ValueError(&#34;Header override must be a valid UUID string.&#34;)
 
-        self.old_dicx = {}
+        old_dicx = {}
         # Get last data from db
         sss = self.getdbsize()
         #print(&#34;sss&#34;, sss)
 
+        # We fake an empty set ... checking against an empty set is a valid OP
         if not sss:
-            raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
-
-        ooo = self.get_rec(sss-1)
+            #raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
+            ddd = self.packer.encode_data(&#34;&#34;, {&#34;blank&#34;: 0, })
+            ooo = [0, ddd,]
+        else:
+            ooo = self.get_rec(sss-1)
 
         if self.pgdebug &gt; 5:
             print(&#34;decoding&#34;, ooo)
 
         decoded = self.packer.decode_data(ooo[1])
+        old_dicx = self._get_fields(decoded[0])
 
-        self.old_dicx = self._get_fields(decoded[0])
-
-        #print(&#34;old_fff&#34;, self.old_dicx[&#34;hash256&#34;])
-        #print(&#34;old_time&#34;, self.old_dicx[&#34;now&#34;])
-
-        aaa = self._fill_record(header, datax)
+        #print(&#34;old_fff&#34;, old_dicx[&#34;hash256&#34;])
+        #print(&#34;old_time&#34;, old_dicx[&#34;now&#34;])
 
+        aaa = self._fill_record(header, datax, old_dicx)
         encoded = self.packer.encode_data(&#34;&#34;, aaa)
 
         #print(&#34;save&#34;, header, &#34;-&#34;, encoded)
-
         #print(&#34;bbb&#34;, self.getdbsize())
         self.save_data(header, encoded)
         #print(&#34;eee&#34;, self.getdbsize())
 
         if self.core_verbose &gt; 1:
             bbb = self.packer.decode_data(encoded)
             print(&#34;Rec&#34;, bbb[0])
@@ -877,17 +896,18 @@
 
         &#39;&#39;&#39; Append data to the end of database &#39;&#39;&#39;
 
         if self.core_verbose &gt; 0:
             print(&#34;Append&#34;, datax)
 
         # Get last data from db
-        sss = self.getdbsize()
-        if not sss:
-            raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
+        #sss = self.getdbsize()
+        #if not sss:
+        #    #raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
+        #    pass
 
         # Produce header  structure
         uuu = uuid.uuid1()
         #print(&#34;uuid date&#34;,uuid2date(uuu))
         header = str(uuu)
         uuuu = uuid.UUID(header)
         #print(&#34;uuid date2&#34;, header, uuid2date(uuuu))
@@ -930,17 +950,18 @@
 
     &#39;&#39;&#39; Append data to the end of database &#39;&#39;&#39;
 
     if self.core_verbose &gt; 0:
         print(&#34;Append&#34;, datax)
 
     # Get last data from db
-    sss = self.getdbsize()
-    if not sss:
-        raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
+    #sss = self.getdbsize()
+    #if not sss:
+    #    #raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
+    #    pass
 
     # Produce header  structure
     uuu = uuid.uuid1()
     #print(&#34;uuid date&#34;,uuid2date(uuu))
     header = str(uuu)
     uuuu = uuid.UUID(header)
     #print(&#34;uuid date2&#34;, header, uuid2date(uuuu))
@@ -977,40 +998,40 @@
     except:
         if self.core_verbose:
             print(&#34;Header override must be a valid UUID string.&#34;)
 
         self.ulock.unlock() #self.ulockname)
         raise ValueError(&#34;Header override must be a valid UUID string.&#34;)
 
-    self.old_dicx = {}
+    old_dicx = {}
     # Get last data from db
     sss = self.getdbsize()
     #print(&#34;sss&#34;, sss)
 
+    # We fake an empty set ... checking against an empty set is a valid OP
     if not sss:
-        raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
-
-    ooo = self.get_rec(sss-1)
+        #raise ValueError(&#34;Invalid database, must have at least one record.&#34;)
+        ddd = self.packer.encode_data(&#34;&#34;, {&#34;blank&#34;: 0, })
+        ooo = [0, ddd,]
+    else:
+        ooo = self.get_rec(sss-1)
 
     if self.pgdebug &gt; 5:
         print(&#34;decoding&#34;, ooo)
 
     decoded = self.packer.decode_data(ooo[1])
+    old_dicx = self._get_fields(decoded[0])
 
-    self.old_dicx = self._get_fields(decoded[0])
-
-    #print(&#34;old_fff&#34;, self.old_dicx[&#34;hash256&#34;])
-    #print(&#34;old_time&#34;, self.old_dicx[&#34;now&#34;])
-
-    aaa = self._fill_record(header, datax)
+    #print(&#34;old_fff&#34;, old_dicx[&#34;hash256&#34;])
+    #print(&#34;old_time&#34;, old_dicx[&#34;now&#34;])
 
+    aaa = self._fill_record(header, datax, old_dicx)
     encoded = self.packer.encode_data(&#34;&#34;, aaa)
 
     #print(&#34;save&#34;, header, &#34;-&#34;, encoded)
-
     #print(&#34;bbb&#34;, self.getdbsize())
     self.save_data(header, encoded)
     #print(&#34;eee&#34;, self.getdbsize())
 
     if self.core_verbose &gt; 1:
         bbb = self.packer.decode_data(encoded)
         print(&#34;Rec&#34;, bbb[0])
```

#### html2text {}

```diff
@@ -98,37 +98,46 @@
         ulockname = os.path.splitext(fname)[0] + ".ulock"
         self.ulock = FileLock(ulockname)
         self.ulock.waitlock()    #(self.ulockname)
 
         super(TwinChain, self).__init__(fname, pgdebug)
 
         self.packer = pyvpacker.packbin()
-        sss = self.getdbsize()
-        if sss == 0:
-            payload = {"Initial": "Initial record, do not use."}
-            #print("Init anchor record", payload)
-
-            # Here we fake the initial backlink for the anchor record
-            self.old_dicx = {}
 
+        sss = self.getdbsize()
+        '''if sss == 0:
             # Produce initial data structure
+            # This is the wron place to produce it, as the chain has no
+            # knowledge of the actual structure ... we provide minimum here
             header = str(uuid.uuid1())
-
             dt = datetime.datetime.utcnow()
             fdt = dt.strftime('%a, %d %b %Y %H:%M:%S`')
-            self.old_dicx["now"] =  fdt
-            self.old_dicx["hash256"]  =  self._hash_any(payload).hexdigest()
-            self.old_dicx["header"]   =  header
-            self.old_dicx["payload"]  =  payload
-            self.old_dicx["backlink"] =  ""
-
-            aaa = self._fill_record(header, payload)
-            #print(aaa)
-            encoded = self.packer.encode_data("", aaa)
+
+            payload = {"Initial": "Initial record, do not use.",
+                            "Default" : 'None', "header": header}
+
+            #payload2 = {"header": header, "payload" : payload}
+
+            # Here we fake the initial backlink for the anchor record
+            old_dicx = {}
+            old_dicx["now"] =  fdt
+            old_dicx["hash256"]  =  self._hash_any(payload).hexdigest()
+            old_dicx["header"]   =  header
+            old_dicx["payload"]  =  payload
+            old_dicx["backlink"] =  ""
+
+            #print("old_dicx:", self.old_dicx)
+
+            aaa = self._fill_record(header, payload, old_dicx)
+            #print("aaa:", aaa)
+            encoded = self.packer.encode_data("", [aaa])
+            #print("encoded:", encoded)
+
             self.save_data(header, encoded)
+        '''
 
         self.ulock.unlock() #self.ulockname)
 
     def _hashtohex(self, varx):
 
         if type(varx) == type(""):
             varx = varx.encode()
@@ -180,30 +189,30 @@
         backlink += self._expand_dict(dicold.get("payload", ""))
         backlink += dicold.get("backlink", "")
         #print("raw backlink", backlink)
         return backlink
 
     # --------------------------------------------------------------------
 
-    def _fill_record(self, header, payload):
+    def _fill_record(self, header, payload, old_dict):
 
         aaa = {}
         aaa["header"] = header
         aaa["payload"] = payload
         aaa["protocol"] = ProtocolVersion
 
         dt = datetime.datetime.now()
         fdt = dt.strftime('%a, %d %b %Y %H:%M:%S')
         aaa["now"] = fdt
         #self._key_n_data(aaa, "hash32", str(self.hash32(payload)))
 
         sumstr = self._build_sumstr(aaa)
         aaa["hash256"] = self._hashtohex(sumstr)
 
-        backlink = self._build_backlink(self.old_dicx)
+        backlink = self._build_backlink(old_dict)
         aaa["backlink"] = self._hashtohex(backlink)
 
         return aaa
 
     def get_payload(self, recnum):
 
         ''' Return the payload on record number '''
@@ -374,41 +383,41 @@
         except:
             if self.core_verbose:
                 print("Header override must be a valid UUID string.")
 
             self.ulock.unlock() #self.ulockname)
             raise ValueError("Header override must be a valid UUID string.")
 
-        self.old_dicx = {}
+        old_dicx = {}
         # Get last data from db
         sss = self.getdbsize()
         #print("sss", sss)
 
+        # We fake an empty set ... checking against an empty set is a valid OP
         if not sss:
-            raise ValueError("Invalid database, must have at least one
+            #raise ValueError("Invalid database, must have at least one
 record.")
-
-        ooo = self.get_rec(sss-1)
+            ddd = self.packer.encode_data("", {"blank": 0, })
+            ooo = [0, ddd,]
+        else:
+            ooo = self.get_rec(sss-1)
 
         if self.pgdebug > 5:
             print("decoding", ooo)
 
         decoded = self.packer.decode_data(ooo[1])
+        old_dicx = self._get_fields(decoded[0])
 
-        self.old_dicx = self._get_fields(decoded[0])
-
-        #print("old_fff", self.old_dicx["hash256"])
-        #print("old_time", self.old_dicx["now"])
-
-        aaa = self._fill_record(header, datax)
+        #print("old_fff", old_dicx["hash256"])
+        #print("old_time", old_dicx["now"])
 
+        aaa = self._fill_record(header, datax, old_dicx)
         encoded = self.packer.encode_data("", aaa)
 
         #print("save", header, "-", encoded)
-
         #print("bbb", self.getdbsize())
         self.save_data(header, encoded)
         #print("eee", self.getdbsize())
 
         if self.core_verbose > 1:
             bbb = self.packer.decode_data(encoded)
             print("Rec", bbb[0])
@@ -420,18 +429,19 @@
 
         ''' Append data to the end of database '''
 
         if self.core_verbose > 0:
             print("Append", datax)
 
         # Get last data from db
-        sss = self.getdbsize()
-        if not sss:
-            raise ValueError("Invalid database, must have at least one
+        #sss = self.getdbsize()
+        #if not sss:
+        #    #raise ValueError("Invalid database, must have at least one
 record.")
+        #    pass
 
         # Produce header  structure
         uuu = uuid.uuid1()
         #print("uuid date",uuid2date(uuu))
         header = str(uuu)
         uuuu = uuid.UUID(header)
         #print("uuid date2", header, uuid2date(uuuu))
@@ -494,38 +504,47 @@
               ulockname = os.path.splitext(fname)[0] + ".ulock"
               self.ulock = FileLock(ulockname)
               self.ulock.waitlock()    #(self.ulockname)
 
               super(TwinChain, self).__init__(fname, pgdebug)
 
               self.packer = pyvpacker.packbin()
-              sss = self.getdbsize()
-              if sss == 0:
-                  payload = {"Initial": "Initial record, do not use."}
-                  #print("Init anchor record", payload)
-
-                  # Here we fake the initial backlink for the anchor record
-                  self.old_dicx = {}
 
+              sss = self.getdbsize()
+              '''if sss == 0:
                   # Produce initial data structure
+                  # This is the wron place to produce it, as the chain has no
+                  # knowledge of the actual structure ... we provide minimum
+      here
                   header = str(uuid.uuid1())
-
                   dt = datetime.datetime.utcnow()
                   fdt = dt.strftime('%a, %d %b %Y %H:%M:%S`')
-                  self.old_dicx["now"] =  fdt
-                  self.old_dicx["hash256"]  =  self._hash_any
-      (payload).hexdigest()
-                  self.old_dicx["header"]   =  header
-                  self.old_dicx["payload"]  =  payload
-                  self.old_dicx["backlink"] =  ""
-
-                  aaa = self._fill_record(header, payload)
-                  #print(aaa)
-                  encoded = self.packer.encode_data("", aaa)
+
+                  payload = {"Initial": "Initial record, do not use.",
+                                  "Default" : 'None', "header": header}
+
+                  #payload2 = {"header": header, "payload" : payload}
+
+                  # Here we fake the initial backlink for the anchor record
+                  old_dicx = {}
+                  old_dicx["now"] =  fdt
+                  old_dicx["hash256"]  =  self._hash_any(payload).hexdigest()
+                  old_dicx["header"]   =  header
+                  old_dicx["payload"]  =  payload
+                  old_dicx["backlink"] =  ""
+
+                  #print("old_dicx:", self.old_dicx)
+
+                  aaa = self._fill_record(header, payload, old_dicx)
+                  #print("aaa:", aaa)
+                  encoded = self.packer.encode_data("", [aaa])
+                  #print("encoded:", encoded)
+
                   self.save_data(header, encoded)
+              '''
 
               self.ulock.unlock() #self.ulockname)
 
           def _hashtohex(self, varx):
 
               if type(varx) == type(""):
                   varx = varx.encode()
@@ -578,30 +597,30 @@
               backlink += dicold.get("backlink", "")
               #print("raw backlink", backlink)
               return backlink
 
           # -------------------------------------------------------------------
       -
 
-          def _fill_record(self, header, payload):
+          def _fill_record(self, header, payload, old_dict):
 
               aaa = {}
               aaa["header"] = header
               aaa["payload"] = payload
               aaa["protocol"] = ProtocolVersion
 
               dt = datetime.datetime.now()
               fdt = dt.strftime('%a, %d %b %Y %H:%M:%S')
               aaa["now"] = fdt
               #self._key_n_data(aaa, "hash32", str(self.hash32(payload)))
 
               sumstr = self._build_sumstr(aaa)
               aaa["hash256"] = self._hashtohex(sumstr)
 
-              backlink = self._build_backlink(self.old_dicx)
+              backlink = self._build_backlink(old_dict)
               aaa["backlink"] = self._hashtohex(backlink)
 
               return aaa
 
           def get_payload(self, recnum):
 
               ''' Return the payload on record number '''
@@ -776,41 +795,42 @@
                   if self.core_verbose:
                       print("Header override must be a valid UUID string.")
 
                   self.ulock.unlock() #self.ulockname)
                   raise ValueError("Header override must be a valid UUID
       string.")
 
-              self.old_dicx = {}
+              old_dicx = {}
               # Get last data from db
               sss = self.getdbsize()
               #print("sss", sss)
 
+              # We fake an empty set ... checking against an empty set is a
+      valid OP
               if not sss:
-                  raise ValueError("Invalid database, must have at least one
+                  #raise ValueError("Invalid database, must have at least one
       record.")
-
-              ooo = self.get_rec(sss-1)
+                  ddd = self.packer.encode_data("", {"blank": 0, })
+                  ooo = [0, ddd,]
+              else:
+                  ooo = self.get_rec(sss-1)
 
               if self.pgdebug > 5:
                   print("decoding", ooo)
 
               decoded = self.packer.decode_data(ooo[1])
+              old_dicx = self._get_fields(decoded[0])
 
-              self.old_dicx = self._get_fields(decoded[0])
-
-              #print("old_fff", self.old_dicx["hash256"])
-              #print("old_time", self.old_dicx["now"])
-
-              aaa = self._fill_record(header, datax)
+              #print("old_fff", old_dicx["hash256"])
+              #print("old_time", old_dicx["now"])
 
+              aaa = self._fill_record(header, datax, old_dicx)
               encoded = self.packer.encode_data("", aaa)
 
               #print("save", header, "-", encoded)
-
               #print("bbb", self.getdbsize())
               self.save_data(header, encoded)
               #print("eee", self.getdbsize())
 
               if self.core_verbose > 1:
                   bbb = self.packer.decode_data(encoded)
                   print("Rec", bbb[0])
@@ -822,18 +842,19 @@
 
               ''' Append data to the end of database '''
 
               if self.core_verbose > 0:
                   print("Append", datax)
 
               # Get last data from db
-              sss = self.getdbsize()
-              if not sss:
-                  raise ValueError("Invalid database, must have at least one
+              #sss = self.getdbsize()
+              #if not sss:
+              #    #raise ValueError("Invalid database, must have at least one
       record.")
+              #    pass
 
               # Produce header  structure
               uuu = uuid.uuid1()
               #print("uuid date",uuid2date(uuu))
               header = str(uuu)
               uuuu = uuid.UUID(header)
               #print("uuid date2", header, uuid2date(uuuu))
@@ -866,18 +887,19 @@
 
                 ''' Append data to the end of database '''
 
                 if self.core_verbose > 0:
                     print("Append", datax)
 
                 # Get last data from db
-                sss = self.getdbsize()
-                if not sss:
-                    raise ValueError("Invalid database, must have at least one
-            record.")
+                #sss = self.getdbsize()
+                #if not sss:
+                #    #raise ValueError("Invalid database, must have at least
+            one record.")
+                #    pass
 
                 # Produce header  structure
                 uuu = uuid.uuid1()
                 #print("uuid date",uuid2date(uuu))
                 header = str(uuu)
                 uuuu = uuid.UUID(header)
                 #print("uuid date2", header, uuid2date(uuuu))
@@ -907,41 +929,42 @@
                     if self.core_verbose:
                         print("Header override must be a valid UUID string.")
 
                     self.ulock.unlock() #self.ulockname)
                     raise ValueError("Header override must be a valid UUID
             string.")
 
-                self.old_dicx = {}
+                old_dicx = {}
                 # Get last data from db
                 sss = self.getdbsize()
                 #print("sss", sss)
 
+                # We fake an empty set ... checking against an empty set is a
+            valid OP
                 if not sss:
-                    raise ValueError("Invalid database, must have at least one
+                    #raise ValueError("Invalid database, must have at least one
             record.")
-
-                ooo = self.get_rec(sss-1)
+                    ddd = self.packer.encode_data("", {"blank": 0, })
+                    ooo = [0, ddd,]
+                else:
+                    ooo = self.get_rec(sss-1)
 
                 if self.pgdebug > 5:
                     print("decoding", ooo)
 
                 decoded = self.packer.decode_data(ooo[1])
+                old_dicx = self._get_fields(decoded[0])
 
-                self.old_dicx = self._get_fields(decoded[0])
-
-                #print("old_fff", self.old_dicx["hash256"])
-                #print("old_time", self.old_dicx["now"])
-
-                aaa = self._fill_record(header, datax)
+                #print("old_fff", old_dicx["hash256"])
+                #print("old_time", old_dicx["now"])
 
+                aaa = self._fill_record(header, datax, old_dicx)
                 encoded = self.packer.encode_data("", aaa)
 
                 #print("save", header, "-", encoded)
-
                 #print("bbb", self.getdbsize())
                 self.save_data(header, encoded)
                 #print("eee", self.getdbsize())
 
                 if self.core_verbose > 1:
                     bbb = self.packer.decode_data(encoded)
                     print("Rec", bbb[0])
```

### Comparing `pydbase-1.5.0/pydbase/docs/twincore.html` & `pydbase-1.5.2/pydbase/docs/twincore.html`

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 
         self.cnt = 0
         self.fname = fname
         self.lckname  = os.path.splitext(self.fname)[0] + &#34;.lock&#34;
         self.idxname  = os.path.splitext(self.fname)[0] + &#34;.pidx&#34;
         self.pgdebug = pgdebug
         self.base_verbose  = 0
+        self.core_verbose  = 0
         self.devmode = devmode
         self.lock = FileLock(self.lckname)
 
         # Make sure only one process can use this
         self.lock.waitlock() #self.lckname)
 
         super(TwinCore, self).__init__(pgdebug)
@@ -1554,14 +1555,15 @@
 
         self.cnt = 0
         self.fname = fname
         self.lckname  = os.path.splitext(self.fname)[0] + &#34;.lock&#34;
         self.idxname  = os.path.splitext(self.fname)[0] + &#34;.pidx&#34;
         self.pgdebug = pgdebug
         self.base_verbose  = 0
+        self.core_verbose  = 0
         self.devmode = devmode
         self.lock = FileLock(self.lckname)
 
         # Make sure only one process can use this
         self.lock.waitlock() #self.lckname)
 
         super(TwinCore, self).__init__(pgdebug)
```

#### html2text {}

```diff
@@ -144,14 +144,15 @@
 
         self.cnt = 0
         self.fname = fname
         self.lckname  = os.path.splitext(self.fname)[0] + ".lock"
         self.idxname  = os.path.splitext(self.fname)[0] + ".pidx"
         self.pgdebug = pgdebug
         self.base_verbose  = 0
+        self.core_verbose  = 0
         self.devmode = devmode
         self.lock = FileLock(self.lckname)
 
         # Make sure only one process can use this
         self.lock.waitlock() #self.lckname)
 
         super(TwinCore, self).__init__(pgdebug)
@@ -1540,14 +1541,15 @@
 
               self.cnt = 0
               self.fname = fname
               self.lckname  = os.path.splitext(self.fname)[0] + ".lock"
               self.idxname  = os.path.splitext(self.fname)[0] + ".pidx"
               self.pgdebug = pgdebug
               self.base_verbose  = 0
+              self.core_verbose  = 0
               self.devmode = devmode
               self.lock = FileLock(self.lckname)
 
               # Make sure only one process can use this
               self.lock.waitlock() #self.lckname)
 
               super(TwinCore, self).__init__(pgdebug)
```

### Comparing `pydbase-1.5.0/pydbase/portalocker.py` & `pydbase-1.5.2/pydbase/portalocker.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/pydbase/twinbase.py` & `pydbase-1.5.2/pydbase/twinbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 FILESIG     = b"PYDB"
 IDXSIG      = b"PYIX"
 RECSIG      = b"RECB"
 RECDEL      = b"RECX"
 RECSEP      = b"RECS"
 RECEND      = b"RECE"
 
+version = "1.5.2"
+
 # Accessed from the main file as well
 
 base_locktout   = LOCK_TIMEOUT   # Settable from ...
 base_pgdebug    = 0
 base_quiet      = 0
 base_integrity  = 0
 base_showdel    = 0
```

### Comparing `pydbase-1.5.0/pydbase/twinchain.py` & `pydbase-1.5.2/pydbase/twinchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,37 +72,46 @@
         ulockname = os.path.splitext(fname)[0] + ".ulock"
         self.ulock = FileLock(ulockname)
         self.ulock.waitlock()    #(self.ulockname)
 
         super(TwinChain, self).__init__(fname, pgdebug)
 
         self.packer = pyvpacker.packbin()
-        sss = self.getdbsize()
-        if sss == 0:
-            payload = {"Initial": "Initial record, do not use."}
-            #print("Init anchor record", payload)
-
-            # Here we fake the initial backlink for the anchor record
-            self.old_dicx = {}
 
+        sss = self.getdbsize()
+        '''if sss == 0:
             # Produce initial data structure
+            # This is the wron place to produce it, as the chain has no
+            # knowledge of the actual structure ... we provide minimum here
             header = str(uuid.uuid1())
-
             dt = datetime.datetime.utcnow()
             fdt = dt.strftime('%a, %d %b %Y %H:%M:%S`')
-            self.old_dicx["now"] =  fdt
-            self.old_dicx["hash256"]  =  self._hash_any(payload).hexdigest()
-            self.old_dicx["header"]   =  header
-            self.old_dicx["payload"]  =  payload
-            self.old_dicx["backlink"] =  ""
-
-            aaa = self._fill_record(header, payload)
-            #print(aaa)
-            encoded = self.packer.encode_data("", aaa)
+
+            payload = {"Initial": "Initial record, do not use.",
+                            "Default" : 'None', "header": header}
+
+            #payload2 = {"header": header, "payload" : payload}
+
+            # Here we fake the initial backlink for the anchor record
+            old_dicx = {}
+            old_dicx["now"] =  fdt
+            old_dicx["hash256"]  =  self._hash_any(payload).hexdigest()
+            old_dicx["header"]   =  header
+            old_dicx["payload"]  =  payload
+            old_dicx["backlink"] =  ""
+
+            #print("old_dicx:", self.old_dicx)
+
+            aaa = self._fill_record(header, payload, old_dicx)
+            #print("aaa:", aaa)
+            encoded = self.packer.encode_data("", [aaa])
+            #print("encoded:", encoded)
+
             self.save_data(header, encoded)
+        '''
 
         self.ulock.unlock() #self.ulockname)
 
     def _hashtohex(self, varx):
 
         if type(varx) == type(""):
             varx = varx.encode()
@@ -154,30 +163,30 @@
         backlink += self._expand_dict(dicold.get("payload", ""))
         backlink += dicold.get("backlink", "")
         #print("raw backlink", backlink)
         return backlink
 
     # --------------------------------------------------------------------
 
-    def _fill_record(self, header, payload):
+    def _fill_record(self, header, payload, old_dict):
 
         aaa = {}
         aaa["header"] = header
         aaa["payload"] = payload
         aaa["protocol"] = ProtocolVersion
 
         dt = datetime.datetime.now()
         fdt = dt.strftime('%a, %d %b %Y %H:%M:%S')
         aaa["now"] = fdt
         #self._key_n_data(aaa, "hash32", str(self.hash32(payload)))
 
         sumstr = self._build_sumstr(aaa)
         aaa["hash256"] = self._hashtohex(sumstr)
 
-        backlink = self._build_backlink(self.old_dicx)
+        backlink = self._build_backlink(old_dict)
         aaa["backlink"] = self._hashtohex(backlink)
 
         return aaa
 
     def get_payload(self, recnum):
 
         ''' Return the payload on record number '''
@@ -347,40 +356,40 @@
         except:
             if self.core_verbose:
                 print("Header override must be a valid UUID string.")
 
             self.ulock.unlock() #self.ulockname)
             raise ValueError("Header override must be a valid UUID string.")
 
-        self.old_dicx = {}
+        old_dicx = {}
         # Get last data from db
         sss = self.getdbsize()
         #print("sss", sss)
 
+        # We fake an empty set ... checking against an empty set is a valid OP
         if not sss:
-            raise ValueError("Invalid database, must have at least one record.")
-
-        ooo = self.get_rec(sss-1)
+            #raise ValueError("Invalid database, must have at least one record.")
+            ddd = self.packer.encode_data("", {"blank": 0, })
+            ooo = [0, ddd,]
+        else:
+            ooo = self.get_rec(sss-1)
 
         if self.pgdebug > 5:
             print("decoding", ooo)
 
         decoded = self.packer.decode_data(ooo[1])
+        old_dicx = self._get_fields(decoded[0])
 
-        self.old_dicx = self._get_fields(decoded[0])
-
-        #print("old_fff", self.old_dicx["hash256"])
-        #print("old_time", self.old_dicx["now"])
-
-        aaa = self._fill_record(header, datax)
+        #print("old_fff", old_dicx["hash256"])
+        #print("old_time", old_dicx["now"])
 
+        aaa = self._fill_record(header, datax, old_dicx)
         encoded = self.packer.encode_data("", aaa)
 
         #print("save", header, "-", encoded)
-
         #print("bbb", self.getdbsize())
         self.save_data(header, encoded)
         #print("eee", self.getdbsize())
 
         if self.core_verbose > 1:
             bbb = self.packer.decode_data(encoded)
             print("Rec", bbb[0])
@@ -392,17 +401,18 @@
 
         ''' Append data to the end of database '''
 
         if self.core_verbose > 0:
             print("Append", datax)
 
         # Get last data from db
-        sss = self.getdbsize()
-        if not sss:
-            raise ValueError("Invalid database, must have at least one record.")
+        #sss = self.getdbsize()
+        #if not sss:
+        #    #raise ValueError("Invalid database, must have at least one record.")
+        #    pass
 
         # Produce header  structure
         uuu = uuid.uuid1()
         #print("uuid date",uuid2date(uuu))
         header = str(uuu)
         uuuu = uuid.UUID(header)
         #print("uuid date2", header, uuid2date(uuuu))
```

### Comparing `pydbase-1.5.0/pydbase/twincore.py` & `pydbase-1.5.2/pydbase/twincore.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
         self.cnt = 0
         self.fname = fname
         self.lckname  = os.path.splitext(self.fname)[0] + ".lock"
         self.idxname  = os.path.splitext(self.fname)[0] + ".pidx"
         self.pgdebug = pgdebug
         self.base_verbose  = 0
+        self.core_verbose  = 0
         self.devmode = devmode
         self.lock = FileLock(self.lckname)
 
         # Make sure only one process can use this
         self.lock.waitlock() #self.lckname)
 
         super(TwinCore, self).__init__(pgdebug)
@@ -1428,8 +1429,12 @@
 
         if hasattr(self, "ifp"):
                 if self.ifp:
                     if not self.ifp.closed:
                         self.ifp.flush()
                         self.ifp.close()
 
+        # remove lockfile
+        if hasattr(self, "lock"):
+            self.lock.unlock()    #dellock(self.lckname)
+
 # EOF
```

### Comparing `pydbase-1.5.0/pydbase.egg-info/PKG-INFO` & `pydbase-1.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,33 @@
-Metadata-Version: 2.1
-Name: pydbase
-Version: 1.5.0
-Summary: High speed database with key / data in python.
-Home-page: https://github.com/pglen/pydbase
-Author: Peter Glen
-Author-email: peterglen99@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
 # pydbase
 
 ## High speed database with key / data
 
 #### see: blockchain functions at the end
 
  &nbsp; The motivation was to create a no frills way of saving / retrieving data.
 It is fast, and the time test shows that this is an order of magnitude
 faster than most mainstream databases. This is due to the engine's simplicity.
 It avoids expensive computations in favor of quickly saving data.
 
-### Fast data save / retrieve 
+### Fast data save / retrieve
 
  &nbsp; Mostly ready for production. All tests pass. Please use caution, as this is new.
 The command line tester can drive most aspects of this API; and it is somewhat
 complete. It is also  good way to see the API / Module in action.
 
 ## API
 
   &nbsp; The module 'twincore' uses two data files and a lock file. The file
  names are generated from the base name of the data file;
 name.pydb for data; name.pidx for the index, name.lock for the lock file.
  In case of frozen process the lock file times out in xx seconds
 and breaks the lock. If the locking process (id in lockfile) does
 not exist, the lock breaks immediately.
 
-### Setting verbosity and debug level:
-
-    twincore.core_quiet   = quiet
-    twincore.core_verbose = verbose
-    twincore.core_pgdebug = pgdebug
-    twincore.core_showdel = sdelx
-
- (Setting before data creation will display mesages from the construtor)
-
 Example DB creation:
 
     core = twincore.TwinCore(datafile_name)
 
 Some basic ops:
 
     dbsize = core.getdbsize()
@@ -62,14 +40,22 @@
 
     core = twinchain.TwinChain(datafile_name)
     core.append(keyx, datax)
     recnum = core.getdbsize()
     rec = core.get_payload(recnum)
     print(recnum, rec)
 
+### Setting verbosity and debug level:
+
+    twincore.core_quiet   = quiet
+    twincore.core_verbose = verbose
+    twincore.core_pgdebug = pgdebug
+
+ (Setting before data creation will display mesages from the construtor)
+
 ### Structure of the data:
 
     32 byte header, starting with FILESIG
 
     4 bytes    4 bytes          4 bytes         Variable
     ------------------------------------------------------------
     RECSIG     Hash_of_key      Len_of_key      DATA_for_key
@@ -170,33 +156,36 @@
     user	0m0.154s
     sys	0m0.071s
     sqlite time test, writing 500 records ...
     real	0m1.465s
     user	0m0.130s
     sys	0m0.292s
 
-  Please mind the fact that the sqlite engine has to do a lot of parsing which we
+  Please note that the sqlite engine has to do a lot of parsing which we
 skip doing; That is why pydbase is more than an order of magnitude faster ...
 even with all the hashing for data integrity check
 
 ### Saving more complex data
 
   The database saves a key / value pair. However, the key can be mutated
 to contain more sophisticated data. For example: adding a string in front of it.
 [ Like: the string CUST_ for customer data / details]. Also the key can be made
 unique by adding a UUID to it, or using pyvpacker to construct it. (see below)
 
-  The data may consist of any text / binary. The library pyvpacker and can pack any data
-into a string; It is installed as a dependency, and a copy of pyvpacker can be
-obtained from pip or github.
+ &nbsp; The data may consist of any text / binary. The library pyvpacker and can pack
+any data into a string; It is installed as a dependency, and a copy of
+pyvpacker can be obtained from pip or github.
+
+## the pyvpacker.py module:
 
-## pyvpacker.py
+ This module can pack arbitrary python data into a string; which can be
+used to store anything in the pydbase's key / data sections. Note that
+data type is limited to the python native data types and compounds thereof.
 
- This module can pack arbitrary python data into a string; which can be used to store
-anything in the pydbase's key / data sections.
+        Types: (int, real, str, array, hash)
 
 Example from running testpacker.py:
 
     org: (1, 2, 'aa', ['bb', b'dd'])
     packed: pg s4 'iisa' i4 1 i4 2 s2 'aa' a29 'pg s2 'sb' s2 'bb' b4 'ZGQ=' '
     unpacked: [1, 2, 'aa', ['bb', b'dd']]
     rec_arr: pg s4 'iisa' i4 1 i4 2 s2 'aa' a29 'pg s2 'sb' s2 'bb' b4 'ZGQ=' '
@@ -241,17 +230,17 @@
 this same key, except the last one.
 
 ## Blockchain implementation
 
    The database is extended with a blockhcain implementation. The new class
 is called twinchain; and it is a class derived from twincore.
 
-  To drive the blockchain, just use the append method. Th database will calculate
+  To drive the blockchain, just use the append method. The database will calculate
 all the hashes, integrate it into the existing chain with the new item getting
-a backlink field. This field is calulated based upon the previous record's
+a backlink field. This field is calculated based upon the previous record's
 hash and the previous record's frozen date. This assures that identical data
 will have a different hash, so data cannot be anticipated based upon its hash
 alone. The hash is done with 256 bits, and assumed to be very secure.
 
 To drive it:
 
         core = twinchain.TwinChain()    # Takes an optional file name
@@ -271,23 +260,14 @@
     The hashed sum of fields saved to the next backlink.
 
 ## Integrity check
 
    Two levels; Level one is checking if the record checksums are correct;
    Level two checks if the linkage is correct.
 
-### TODO
-
-    Speed this up by implementing this as a 'C' module
-
-## PyTest
-
- The pytest passes with no errors;
- The following (and more) test are created / executed:
-
 ## The in-place update
 
   The save operation has a flag for in-place update. This is useful for updating
 without the data storage extending. Useful for counts and timers. The in-place
 update operates as a record overwrite, and has to be equal length than the existing
 record. If shorter, the record is padded to the original data's length by appending
 spaces. Below is an example to update a counter in the database, which will execute
@@ -297,62 +277,66 @@
     rec = dbcore.get_rec(xxx)
     # Increment count:
     arr = self.packer.decode_data(rec[1])[0]
     arr[0] = "%05d" % (int(arr[0]) + 1)
     strx = str(self.packer.encode_data("", arr))
     ret = dbcore.save_data(rec[0], strx, True)
 
- If the in-place data is longer, a new record is created, just like a normal
-operation. This new, longer record than accommodates all the new in-place requests.
+ If the new data (relativeto the in-place data) is longer, a new record is
+created, just like a normal operation. This new, longer record than accommodates all the new in-place requests.
 It is recommended that one produces a fixed record size for consistent results.
 (See: sprintf (python % operator) in the example above.)
 
+## PyTest
+
+ The pytest passes with no errors;
+ The following (and more) test are created / executed:
+
 ### Test results:
 
     ============================= test session starts ==============================
     platform linux -- Python 3.10.12, pytest-7.4.3, pluggy-1.0.0
     rootdir: /home/peterglen/pgpygtk/pydbase
-    collected 43 items
+    collected 44 items
 
-    test_acreate.py .....                                                    [ 11%]
-    test_bindata.py .                                                        [ 13%]
-    test_chain.py .                                                          [ 16%]
-    test_chain_integ.py ..                                                   [ 20%]
-    test_chain_link.py ..                                                    [ 25%]
-    test_del.py .                                                            [ 27%]
-    test_dump.py .                                                           [ 30%]
-    test_find.py ..                                                          [ 34%]
-    test_findrec.py ..                                                       [ 39%]
-    test_getoffs.py ...                                                      [ 46%]
-    test_getrec.py .                                                         [ 48%]
-    test_inplace.py ...                                                      [ 55%]
-    test_integrity.py .                                                      [ 58%]
-    test_list.py ..                                                          [ 62%]
-    test_lockrel.py ..                                                       [ 67%]
-    test_multi.py ..                                                         [ 72%]
-    test_packer.py ......                                                    [ 86%]
-    test_randdata.py .                                                       [ 88%]
+    test_acreate.py ...                                                      [  6%]
+    test_bigdata.py .                                                        [  9%]
+    test_bindata.py .                                                        [ 11%]
+    test_chain.py .                                                          [ 13%]
+    test_chain_data.py .                                                     [ 15%]
+    test_chain_link.py ..                                                    [ 20%]
+    test_del.py .                                                            [ 22%]
+    test_dump.py .                                                           [ 25%]
+    test_find.py ..                                                          [ 29%]
+    test_findrec.py ..                                                       [ 34%]
+    test_getoffs.py ...                                                      [ 40%]
+    test_getrec.py .                                                         [ 43%]
+    test_handles.py .....                                                    [ 54%]
+    test_inplace.py ...                                                      [ 61%]
+    test_integrity.py .                                                      [ 63%]
+    test_list.py ..                                                          [ 68%]
+    test_lockrel.py .                                                        [ 70%]
+    test_multi.py ..                                                         [ 75%]
+    test_packer.py ......                                                    [ 88%]
     test_reindex.py .                                                        [ 90%]
     test_search.py ...                                                       [ 97%]
     test_vacuum.py .                                                         [100%]
 
-    ============================== 43 passed in 0.68s ==============================
+    ============================== 44 passed in 0.57s ==============================
 
 ## History
 
     1.1         Tue 20.Feb.2024     Initial release
     1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
     1.4.0       Tue 27.Feb.2024     Addedd pgdebug
     1.4.2       Wed 28.Feb.2024     Fixed multiple instances
     1.4.3       Wed 28.Feb.2024     ChainAdm added
     1.4.4       Fri 01.Mar.2024     Tests for chain functions
     1.4.5       Fri 01.Mar.2024     Misc fixes
     1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
     1.4.7       Tue 05.Mar.2024     In place record update
     1.4.8       Sat 09.Mar.2024     Added new locking mechanism
-
-## Errata
-
-    Chain is still in development, most of it functions well.
-    Not for production.
+    1.4.9       Mon 01.Apr.2024     Updated to run on MSYS2, new locking
+    1.5.0       Tue 02.Apr.2024     Cleaned, pip upload
+    1.5.1       Wed 10.Apr.2024     Dangling lock .. fixed
 
 // EOF
```

### Comparing `pydbase-1.5.0/pydbase.egg-info/SOURCES.txt` & `pydbase-1.5.2/pydbase.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 chainadm.py
 dbaseadm.py
 setup.py
+man/man1/pydbase.1
 pydbase/__init__.py
 pydbase/dbutils.py
 pydbase/portalocker.py
 pydbase/twinbase.py
 pydbase/twinchain.py
 pydbase/twincore.py
 pydbase.egg-info/PKG-INFO
```

### Comparing `pydbase-1.5.0/setup.py` & `pydbase-1.5.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,46 +16,58 @@
           'License :: OSI Approved :: Python Software Foundation License',
           'Operating System :: Microsoft :: Windows',
           'Operating System :: POSIX',
           'Programming Language :: Python',
           'Topic :: Databases',
         ]
 
+# Get version number  from the server support file:
+fp = open("pydbase/twinbase.py", "rt")
+vvv = fp.read(); fp.close()
+loc_vers =  '1.0.0'     # Default
+for aa in vvv.split("\n"):
+    idx = aa.find("version =")
+    if idx == 0:        # At the beginning of line
+        try:
+            loc_vers = aa.split()[2].replace('"', "")
+            break
+        except:
+            pass
+#print("loc_vers:", loc_vers)
+
 includex = ["*", "pydbase/", ]
-versionx = "1.5.0"
 
 doclist = []; droot = "pydbase/docs/"
 doclistx = os.listdir(droot)
 for aa in doclistx:
     doclist.append(droot + aa)
-#print(doclist)
-#sys.exit()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pydbase",
-    version=versionx,
+    version=loc_vers,
     author="Peter Glen",
     author_email="peterglen99@gmail.com",
     description="High speed database with key / data in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pglen/pydbase",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    include_package_data=True,
     packages=setuptools.find_packages(include=includex),
     scripts = ['dbaseadm.py', 'chainadm.py'],
     py_modules = ["pyvpacker",],
-    package_data = {"docs" : doclist},
+    include_package_data=True,
+    package_data = {"pydbase" : doclist},
+    #data_files = {"man/man1/pydbase.1"},
     python_requires='>=3',
     entry_points={
         'console_scripts': [ "dbaseadm=dbaseadm:mainfunc",
                                 "chainadm=chainadm:mainfunc",
                            ],
     },
 )
```

### Comparing `pydbase-1.5.0/tests/test_acreate.py` & `pydbase-1.5.2/tests/test_acreate.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_bigdata.py` & `pydbase-1.5.2/tests/test_bigdata.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_bindata.py` & `pydbase-1.5.2/tests/test_bindata.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_chain.py` & `pydbase-1.5.2/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_chain_data.py` & `pydbase-1.5.2/tests/test_chain_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     dbsize = core2.getdbsize()
 
     #for aa in range(1, dbsize):
     #    print(aa, core2.get_payload(aa))
 
     # The failing record
     ppp = core2.checkdata(1)
-    assert ppp == False
+    assert ppp == True
 
     # All others
     #for aa in range(0, dbsize):
     #    ppp = core2.checkdata(aa)
     #    print(aa, ppp)
     #    #assert ppp == True
     #print(fname)
```

### Comparing `pydbase-1.5.0/tests/test_chain_link.py` & `pydbase-1.5.2/tests/test_chain_link.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
 
     try:
         # No dangling data
-        os.remove(fname)
-        os.remove(iname)
+        #os.remove(fname)
+        #os.remove(iname)
         pass
     except:
         print(sys.exc_info())
         #assert 0
         pass
 
     #assert 0
@@ -67,37 +67,37 @@
 
 def test_links(capsys):
 
     print(fname)
     fp = open(fname, "rb")
     buff = fp.read(); fp.close()
 
-    # Damage file buffer rec 2 -- make sure it is in payload
+    # Damage file buffer rec 1 -- make sure it is in relevant section
     # Please note that this is a hack to test damage
-    pos = 0x370
+    pos = 0x440
     buff = buff[:pos] + b'x' + buff[pos+1:]
 
     fp2 = open(fname, "wb")
     fp2.write(buff);  fp2.close()
 
     # Changed file buffer, reload
     core2 = twinchain.TwinChain(fname)
     assert core2 != 0
     dbsize = core2.getdbsize()
 
     # All others
     #for aa in range(1, dbsize):
     #    print(aa, core2.get_payload(aa))
 
-    # The failing record
-    ppp = core2.checkdata(1)
-    assert ppp == False
+    # The succeeding record
+    ppp = core2.linkintegrity(0)
+    assert ppp == True
 
     # The failing record
-    ppp = core2.linkintegrity(2)
+    ppp = core2.linkintegrity(1)
     assert ppp == False
 
     # Test print of the setup
     #for aa in range(0, dbsize):
     #    ppp = core2.checkdata(aa)
     #    print("data", aa, ppp)
     #
```

### Comparing `pydbase-1.5.0/tests/test_del.py` & `pydbase-1.5.2/tests/test_del.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_dump.py` & `pydbase-1.5.2/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_find.py` & `pydbase-1.5.2/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_findrec.py` & `pydbase-1.5.2/tests/test_findrec.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_getoffs.py` & `pydbase-1.5.2/tests/test_getoffs.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_getrec.py` & `pydbase-1.5.2/tests/test_getrec.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_handles.py` & `pydbase-1.5.2/tests/test_handles.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_inplace.py` & `pydbase-1.5.2/tests/test_inplace.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_integrity.py` & `pydbase-1.5.2/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_list.py` & `pydbase-1.5.2/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_lockrel.py` & `pydbase-1.5.2/tests/test_lockrel.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_multi.py` & `pydbase-1.5.2/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_packer.py` & `pydbase-1.5.2/tests/test_packer.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_reindex.py` & `pydbase-1.5.2/tests/test_reindex.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_search.py` & `pydbase-1.5.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.5.0/tests/test_vacuum.py` & `pydbase-1.5.2/tests/test_vacuum.py`

 * *Files identical despite different names*

