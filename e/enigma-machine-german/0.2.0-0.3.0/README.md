# Comparing `tmp/enigma_machine_german-0.2.0.tar.gz` & `tmp/enigma_machine_german-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enigma_machine_german-0.2.0.tar", last modified: Fri Mar 17 03:28:11 2023, max compression
+gzip compressed data, was "enigma_machine_german-0.3.0.tar", last modified: Wed Apr 10 01:28:02 2024, max compression
```

## Comparing `enigma_machine_german-0.2.0.tar` & `enigma_machine_german-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 03:28:11.849952 enigma_machine_german-0.2.0/
--rw-rw-rw-   0        0        0      335 2023-03-17 03:28:11.849952 enigma_machine_german-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-17 03:28:11.835953 enigma_machine_german-0.2.0/enigma_machine_german/
--rw-rw-rw-   0        0        0       48 2023-03-17 03:23:14.000000 enigma_machine_german-0.2.0/enigma_machine_german/__init__.py
--rw-rw-rw-   0        0        0     5240 2023-03-17 03:23:14.000000 enigma_machine_german-0.2.0/enigma_machine_german/enigma_machine_german.py
-drwxrwxrwx   0        0        0        0 2023-03-17 03:28:11.848953 enigma_machine_german-0.2.0/enigma_machine_german.egg-info/
--rw-rw-rw-   0        0        0      335 2023-03-17 03:28:11.000000 enigma_machine_german-0.2.0/enigma_machine_german.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-03-17 03:28:11.000000 enigma_machine_german-0.2.0/enigma_machine_german.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 03:28:11.000000 enigma_machine_german-0.2.0/enigma_machine_german.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-03-17 03:28:11.000000 enigma_machine_german-0.2.0/enigma_machine_german.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 03:28:11.850463 enigma_machine_german-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      444 2023-03-17 03:28:09.000000 enigma_machine_german-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:28:02.363807 enigma_machine_german-0.3.0/
+-rw-rw-rw-   0        0        0      296 2024-04-10 01:28:02.361307 enigma_machine_german-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:28:02.351311 enigma_machine_german-0.3.0/enigma_machine_german/
+-rw-rw-rw-   0        0        0       48 2023-03-17 03:23:14.000000 enigma_machine_german-0.3.0/enigma_machine_german/__init__.py
+-rw-rw-rw-   0        0        0     6437 2024-04-08 15:30:10.000000 enigma_machine_german-0.3.0/enigma_machine_german/enigma_machine_german.py
+drwxrwxrwx   0        0        0        0 2024-04-10 01:28:02.360313 enigma_machine_german-0.3.0/enigma_machine_german.egg-info/
+-rw-rw-rw-   0        0        0      296 2024-04-10 01:28:02.000000 enigma_machine_german-0.3.0/enigma_machine_german.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-10 01:28:02.000000 enigma_machine_german-0.3.0/enigma_machine_german.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:28:02.000000 enigma_machine_german-0.3.0/enigma_machine_german.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-10 01:28:02.000000 enigma_machine_german-0.3.0/enigma_machine_german.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:28:02.363807 enigma_machine_german-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      444 2024-04-10 01:27:17.000000 enigma_machine_german-0.3.0/setup.py
```

### Comparing `enigma_machine_german-0.2.0/enigma_machine_german/enigma_machine_german.py` & `enigma_machine_german-0.3.0/enigma_machine_german/enigma_machine_german.py`

 * *Files 16% similar despite different names*

```diff
@@ -244,14 +244,33 @@
                 The encrypted character.
         """
         temp = R[self.wheel3[ATON[self.wheel2[ATON[self.wheel1[ATON[ETW[char]]]]]]]]
         temp2 = self._find_key_by_value(ETW, NTOA[self.wheel1.index(NTOA[self.wheel2.index(NTOA[self.wheel3.index(temp)])])])
         self.rotate_wheels()
         return temp2
 
+    def decrypt_char(self, char):
+        """
+            Decrypt a single character using the Enigma machine.
+
+            Parameters
+            ----------
+            char : str
+                The character to be decrypted.
+
+            Returns
+            -------
+            str
+                The decrypted character.
+        """
+        temp = ETW[self.wheel1[ATON[self.wheel2[ATON[self.wheel3[ATON[R[char]]]]]]]]
+        temp2 = self._find_key_by_value(R, NTOA[self.wheel3.index(NTOA[self.wheel2.index(NTOA[self.wheel1.index(temp)])])])
+        self.rotate_wheels()
+        return temp2
+
     def encrypt_message(self, message):
         """
             Encrypt a message using the Enigma machine.
 
             Parameters
             ----------
             message : str
@@ -266,14 +285,37 @@
         for char in message:
             if char.isalpha():
                 encrypted += self.encrypt_char(char.upper())
             else:
                 encrypted += char
         return encrypted
 
+
+    def decrypt_message(self, message):
+        """
+            Decrypt a message using the Enigma machine.
+
+            Parameters
+            ----------
+            message : str
+                The message to be decrypted.
+
+            Returns
+            -------
+            str
+                The decrypted message.
+        """
+        decrypted = ""
+        for char in message:
+            if char.isalpha():
+                decrypted += self.decrypt_char(char.upper())
+            else:
+                decrypted += char
+        return decrypted
+
     def _find_key_by_value(self, dictionary, value):
         """
            Find a key in a dictionary based on its value.
 
            Parameters
            ----------
            dictionary : dict
```

