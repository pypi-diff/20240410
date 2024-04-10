# Comparing `tmp/texttoolspy-0.0.2-py3-none-any.whl.zip` & `tmp/texttoolspy-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3230 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     2133 b- defN 24-Mar-18 19:33 texttoolspy/__init__.py
+Zip file size: 3231 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     2129 b- defN 24-Apr-09 18:37 texttoolspy/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-08 20:02 texttoolspy/main.py
--rw-rw-rw-  2.0 fat     1083 b- defN 24-Apr-09 18:31 texttoolspy-0.0.2.dist-info/Licence.txt
--rw-rw-rw-  2.0 fat      635 b- defN 24-Apr-09 18:31 texttoolspy-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-09 18:31 texttoolspy-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-09 18:31 texttoolspy-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      562 b- defN 24-Apr-09 18:31 texttoolspy-0.0.2.dist-info/RECORD
-7 files, 4517 bytes uncompressed, 2226 bytes compressed:  50.7%
+-rw-rw-rw-  2.0 fat     1083 b- defN 24-Apr-09 18:38 texttoolspy-0.0.3.dist-info/Licence.txt
+-rw-rw-rw-  2.0 fat      635 b- defN 24-Apr-09 18:38 texttoolspy-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-09 18:38 texttoolspy-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-09 18:38 texttoolspy-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      562 b- defN 24-Apr-09 18:38 texttoolspy-0.0.3.dist-info/RECORD
+7 files, 4513 bytes uncompressed, 2227 bytes compressed:  50.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: texttoolspy/__init__.py
 Comment: 
 
 Filename: texttoolspy/main.py
 Comment: 
 
-Filename: texttoolspy-0.0.2.dist-info/Licence.txt
+Filename: texttoolspy-0.0.3.dist-info/Licence.txt
 Comment: 
 
-Filename: texttoolspy-0.0.2.dist-info/METADATA
+Filename: texttoolspy-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: texttoolspy-0.0.2.dist-info/WHEEL
+Filename: texttoolspy-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: texttoolspy-0.0.2.dist-info/top_level.txt
+Filename: texttoolspy-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: texttoolspy-0.0.2.dist-info/RECORD
+Filename: texttoolspy-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## texttoolspy/__init__.py

```diff
@@ -44,15 +44,15 @@
 def LineBreak(lines):
   for x in range(0,lines):
     print("  ")
 def menu(menu_items,menu_type):
   selected_menu = 1
   answer = ""
   while answer != key.ENTER:
-    os.system("clear")
+    os.system("cls")
     for x in range(0,len(menu_items)):
       if selected_menu == x+1:
         if str(menu_type)=="1":
           print(f"> {italic}{menu_items[x]} \n")
         elif str(menu_type)=="2":
           print(colored(f"{bold}{menu_items[x]} \n","black","on_white"))
         elif str(menu_type) == "3":
@@ -64,10 +64,10 @@
     if answer == key.DOWN and selected_menu < len(menu_items):
       selected_menu += 1
     elif answer == key.UP and selected_menu > 1:
       selected_menu -= 1
   
   Selected = menu_items[selected_menu-1]
   return Selected
-  os.system("clear")
+  os.system("cls")
```

## Comparing `texttoolspy-0.0.2.dist-info/Licence.txt` & `texttoolspy-0.0.3.dist-info/Licence.txt`

 * *Files identical despite different names*

## Comparing `texttoolspy-0.0.2.dist-info/METADATA` & `texttoolspy-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texttoolspy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool that allows you to create responsive tools in text
 Author: MilesWK
 Author-email: your_name@example.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `texttoolspy-0.0.2.dist-info/RECORD` & `texttoolspy-0.0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-texttoolspy/__init__.py,sha256=bBGcILIUo10wCTLm2kHKNekCaBxrnRM0Qeh6tcYnLaE,2133
+texttoolspy/__init__.py,sha256=yxAh0W5P4rOE8dGKgyUYZyCja77WiU-KmrN_YBIKOH8,2129
 texttoolspy/main.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-texttoolspy-0.0.2.dist-info/Licence.txt,sha256=xmmaISdPorZT-rPBZ0F43fqfVLcQxkrldRFyJJNQW9I,1083
-texttoolspy-0.0.2.dist-info/METADATA,sha256=5yq9G9WbzhFBgaCG0Qdx9J-5q9IpauEDXsduANI1j2k,635
-texttoolspy-0.0.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-texttoolspy-0.0.2.dist-info/top_level.txt,sha256=pPT7_1Oiuya1rnSvm9vrpptDLGsFrvmVBm96CS7_fxM,12
-texttoolspy-0.0.2.dist-info/RECORD,,
+texttoolspy-0.0.3.dist-info/Licence.txt,sha256=xmmaISdPorZT-rPBZ0F43fqfVLcQxkrldRFyJJNQW9I,1083
+texttoolspy-0.0.3.dist-info/METADATA,sha256=b0uXoo0xqCkp21_RGx1eRK9Cx_ADf5GIHczsKzLVoNU,635
+texttoolspy-0.0.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+texttoolspy-0.0.3.dist-info/top_level.txt,sha256=pPT7_1Oiuya1rnSvm9vrpptDLGsFrvmVBm96CS7_fxM,12
+texttoolspy-0.0.3.dist-info/RECORD,,
```

