# Comparing `tmp/fv1_programmer-0.5.1.tar.gz` & `tmp/fv1_programmer-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fv1_programmer-0.5.1.tar", max compression
+gzip compressed data, was "fv1_programmer-0.5.2.tar", max compression
```

## Comparing `fv1_programmer-0.5.1.tar` & `fv1_programmer-0.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1065 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/LICENSE
--rw-r--r--   0        0        0     4277 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/README.md
--rw-r--r--   0        0        0     1140 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/adaptor/adapter.py
--rw-r--r--   0        0        0     1083 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/adaptor/mcp2221.py
--rw-r--r--   0        0        0       30 2024-04-05 13:10:34.329520 fv1_programmer-0.5.1/asfv1/.git
--rw-r--r--   0        0        0     1157 2024-04-05 13:10:35.113519 fv1_programmer-0.5.1/asfv1/.gitignore
--rw-r--r--   0        0        0     1075 2024-04-05 13:10:35.113519 fv1_programmer-0.5.1/asfv1/LICENSE
--rw-r--r--   0        0        0    36334 2024-04-05 13:10:35.113519 fv1_programmer-0.5.1/asfv1/README.md
--rw-r--r--   0        0        0    54482 2024-04-05 13:10:35.113519 fv1_programmer-0.5.1/asfv1/asfv1.py
--rw-r--r--   0        0        0      561 2024-04-05 13:10:35.113519 fv1_programmer-0.5.1/asfv1/example.asm
--rw-r--r--   0        0        0      801 2024-04-05 13:10:35.113519 fv1_programmer-0.5.1/asfv1/setup.py
--rw-r--r--   0        0        0       31 2024-04-05 13:10:34.601519 fv1_programmer-0.5.1/disfv1/.git
--rw-r--r--   0        0        0     1157 2024-04-05 13:10:35.121518 fv1_programmer-0.5.1/disfv1/.gitignore
--rw-r--r--   0        0        0     1075 2024-04-05 13:10:35.121518 fv1_programmer-0.5.1/disfv1/LICENSE
--rw-r--r--   0        0        0     4816 2024-04-05 13:10:35.121518 fv1_programmer-0.5.1/disfv1/README.md
--rw-r--r--   0        0        0    17532 2024-04-05 13:10:35.121518 fv1_programmer-0.5.1/disfv1/disfv1.py
--rw-r--r--   0        0        0      512 2024-04-05 13:10:35.121518 fv1_programmer-0.5.1/disfv1/example.bin
--rw-r--r--   0        0        0      798 2024-04-05 13:10:35.121518 fv1_programmer-0.5.1/disfv1/setup.py
--rw-r--r--   0        0        0     6485 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/eeprom/eeprom.py
--rw-r--r--   0        0        0     1587 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/fv1_programmer/dialogs.css
--rw-r--r--   0        0        0     4809 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/fv1_programmer/dialogs.py
--rw-r--r--   0        0        0     1729 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/fv1_programmer/fv1.py
--rw-r--r--   0        0        0     3081 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/fv1_programmer/main.py
--rw-r--r--   0        0        0      875 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/fv1_programmer/pyinstaller.py
--rw-r--r--   0        0        0     1785 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/fv1_programmer/tui.css
--rw-r--r--   0        0        0    26725 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/fv1_programmer/tui.py
--rw-r--r--   0        0        0     1404 2024-04-05 13:10:34.013521 fv1_programmer-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5642 1970-01-01 00:00:00.000000 fv1_programmer-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4278 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/README.md
+-rw-r--r--   0        0        0     1140 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/adaptor/adapter.py
+-rw-r--r--   0        0        0     1604 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/adaptor/mcp2221.py
+-rw-r--r--   0        0        0       30 2024-04-10 01:33:28.005708 fv1_programmer-0.5.2/asfv1/.git
+-rw-r--r--   0        0        0     1157 2024-04-10 01:33:28.769714 fv1_programmer-0.5.2/asfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2024-04-10 01:33:28.769714 fv1_programmer-0.5.2/asfv1/LICENSE
+-rw-r--r--   0        0        0    36334 2024-04-10 01:33:28.769714 fv1_programmer-0.5.2/asfv1/README.md
+-rw-r--r--   0        0        0    54482 2024-04-10 01:33:28.769714 fv1_programmer-0.5.2/asfv1/asfv1.py
+-rw-r--r--   0        0        0      561 2024-04-10 01:33:28.769714 fv1_programmer-0.5.2/asfv1/example.asm
+-rw-r--r--   0        0        0      801 2024-04-10 01:33:28.769714 fv1_programmer-0.5.2/asfv1/setup.py
+-rw-r--r--   0        0        0       31 2024-04-10 01:33:28.261710 fv1_programmer-0.5.2/disfv1/.git
+-rw-r--r--   0        0        0     1157 2024-04-10 01:33:28.777714 fv1_programmer-0.5.2/disfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2024-04-10 01:33:28.777714 fv1_programmer-0.5.2/disfv1/LICENSE
+-rw-r--r--   0        0        0     4816 2024-04-10 01:33:28.777714 fv1_programmer-0.5.2/disfv1/README.md
+-rw-r--r--   0        0        0    17532 2024-04-10 01:33:28.777714 fv1_programmer-0.5.2/disfv1/disfv1.py
+-rw-r--r--   0        0        0      512 2024-04-10 01:33:28.777714 fv1_programmer-0.5.2/disfv1/example.bin
+-rw-r--r--   0        0        0      798 2024-04-10 01:33:28.777714 fv1_programmer-0.5.2/disfv1/setup.py
+-rw-r--r--   0        0        0     6485 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/eeprom/eeprom.py
+-rw-r--r--   0        0        0     1582 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/fv1_programmer/dialogs.css
+-rw-r--r--   0        0        0     4809 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/fv1_programmer/dialogs.py
+-rw-r--r--   0        0        0     2055 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/fv1_programmer/fv1.py
+-rw-r--r--   0        0        0     3081 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/fv1_programmer/main.py
+-rw-r--r--   0        0        0      875 2024-04-10 01:33:27.645704 fv1_programmer-0.5.2/fv1_programmer/pyinstaller.py
+-rw-r--r--   0        0        0     1785 2024-04-10 01:33:27.649705 fv1_programmer-0.5.2/fv1_programmer/tui.css
+-rw-r--r--   0        0        0    28492 2024-04-10 01:33:27.649705 fv1_programmer-0.5.2/fv1_programmer/tui.py
+-rw-r--r--   0        0        0     1404 2024-04-10 01:33:27.649705 fv1_programmer-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5643 1970-01-01 00:00:00.000000 fv1_programmer-0.5.2/PKG-INFO
```

### Comparing `fv1_programmer-0.5.1/LICENSE` & `fv1_programmer-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/README.md` & `fv1_programmer-0.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ```
 $ fv1_programmer
 ```
 
 This will bring up a user interface that will allow you to configure all 8 program slots of the Easy Spin's FV-1 DSP and write the EEPROM.
 
-![image](https://github.com/audiofab/fv1_programmer/assets/1384978/36d8e9b9-4fe6-4cc4-b7b3-194910aaff97)
+![image](https://github.com/audiofab/fv1_programmer/assets/1384978/300f1d0a-0dfc-4b63-8364-a8b2a8e76c65)
 
 NOTE: On Linux you likely still need to install `libusb` and add a udev rule separately. See [Ubuntu Linux](README.md#Ubuntu-linux).
 
 ## Using One Of The Pre-Built Binaries
 
 ### Windows
 
@@ -73,8 +73,8 @@
 
 
 
 # Known Issues
 
 ## Drag and drop not working reliably
 
-On Windows 10 Terminal we have seen some issues with drag and drop not always working reliably. If you find that dragging a file from Explorer onto the application is not working, try dropping the file on the upper part of the user-interface (or even on the Program tabs) instead.
+On Windows 10 Terminal we have seen some issues with drag and drop not always working reliably. If you find that dragging a file from Explorer onto the application is not working, try dropping the file on the upper part of the user-interface (or even on the Program tabs) instead.
```

### Comparing `fv1_programmer-0.5.1/adaptor/adapter.py` & `fv1_programmer-0.5.2/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/adaptor/mcp2221.py` & `fv1_programmer-0.5.2/adaptor/mcp2221.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import EasyMCP2221
+from EasyMCP2221.exceptions import LowSCLError, LowSDAError
 from .adapter import I2CAdaptor
 
 
+class UnexpectedHardwareException(Exception):
+    pass
+
+
 class MCP2221I2CAdaptor(I2CAdaptor):
     def __init__(self, i2c_address, i2c_clock_speed=100000, transaction_timeout_ms=20):
         super(MCP2221I2CAdaptor, self).__init__(i2c_address, i2c_clock_speed)
         self.timeout = transaction_timeout_ms
         self.mcp = None
 
     def open(self,):
@@ -15,15 +20,21 @@
         # Ensure there is something connected by doing a dummy read
         return self.mcp.I2C_read(self.address)
 
     def close(self,):
         pass
 
     def read_bytes(self, num_bytes):
-        return self.mcp.I2C_read(self.address, size=num_bytes, timeout_ms=self.timeout)
+        try:
+            return self.mcp.I2C_read(self.address, size=num_bytes, timeout_ms=self.timeout)
+        except (LowSCLError, LowSDAError):
+            raise UnexpectedHardwareException("Unexpected programmer state. Try unplugging and re-plugging the programmer and trying again.")
 
     def write_bytes(self, byte_list):
-        self.mcp.I2C_write(self.address, byte_list, timeout_ms=self.timeout)
+        try:
+            self.mcp.I2C_write(self.address, byte_list, timeout_ms=self.timeout)
+        except (LowSCLError, LowSDAError):
+            raise UnexpectedHardwareException("Unexpected programmer state. Try unplugging and re-plugging the programmer and trying again.")
 
     def write_then_read_bytes(self, byte_list, num_read_bytes):
         self.mcp.I2C_write(self.address, byte_list, kind='nonstop', timeout_ms=self.timeout)
         return self.mcp.I2C_read(self.address, num_read_bytes, kind='restart', timeout_ms=self.timeout)
```

### Comparing `fv1_programmer-0.5.1/asfv1/.gitignore` & `fv1_programmer-0.5.2/asfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/asfv1/LICENSE` & `fv1_programmer-0.5.2/asfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/asfv1/README.md` & `fv1_programmer-0.5.2/asfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/asfv1/asfv1.py` & `fv1_programmer-0.5.2/asfv1/asfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/asfv1/example.asm` & `fv1_programmer-0.5.2/asfv1/example.asm`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/asfv1/setup.py` & `fv1_programmer-0.5.2/asfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/disfv1/.gitignore` & `fv1_programmer-0.5.2/disfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/disfv1/LICENSE` & `fv1_programmer-0.5.2/disfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/disfv1/README.md` & `fv1_programmer-0.5.2/disfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/disfv1/disfv1.py` & `fv1_programmer-0.5.2/disfv1/disfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/disfv1/setup.py` & `fv1_programmer-0.5.2/disfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/eeprom/eeprom.py` & `fv1_programmer-0.5.2/eeprom/eeprom.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/fv1_programmer/dialogs.css` & `fv1_programmer-0.5.2/fv1_programmer/dialogs.css`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,28 @@
     border: thick $background 80%;
     background: $surface;
 }
 
 #renameslotdialog {
     padding: 0 1;
     width: 80vw;
-    height: 30vh;
+    height: 8;
     border: thick $background 80%;
     background: $surface;
 }
 
 #renameslotdialog > Input {
     margin: 1 1;
     border: $primary;
 }
 
 #filesavedialog {
     padding: 0 1;
     width: 80vw;
-    height: 30vh;
+    height: 12;
     border: thick $background 80%;
     background: $surface;
 }
 
 #filesavedialog > Input {
     margin: 1 1;
     border: $primary;
```

### Comparing `fv1_programmer-0.5.1/fv1_programmer/dialogs.py` & `fv1_programmer-0.5.2/fv1_programmer/dialogs.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/fv1_programmer/fv1.py` & `fv1_programmer-0.5.2/fv1_programmer/fv1.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,18 @@
                       wfunc=warning, efunc=error)
         try:
             fp.parse()
         except ASFV1Error:
             if len(errors) == 0:
                 errors = ["Failed to assemble program"]
             return None, fp.icnt, warnings, errors
+        except Exception as e:
+            if len(errors) == 0:
+                errors = [f"An unknown error occurred on line {fp.sline}"]
+            return None, fp.icnt, warnings, errors
 
         return fp.program, fp.icnt, warnings, errors
 
     def from_bytearray(self, data : bytearray, relative=False, suppressraw=False) -> str:
         """
         Disassembles a binary FV1 program and sets the internal asm property to
         the disassembled output. Returns any warnings in a concatenated string.
@@ -47,15 +51,18 @@
         def warning(msg):
             nonlocal warnings
             warnings.append(msg)
 
         fp = fv1deparse(data,
                         relative=relative, nopraw=suppressraw,
                         wfunc=warning)
-        fp.deparse()
-        self.asm = fp.listing
+        try:
+            fp.deparse()
+            self.asm = fp.listing
+        except Exception as e:
+            self.asm = "; Failed when trying to disassemble! Invalid program data?"
 
         return warnings
 
     @property
     def assembly(self,) -> str:
         return self.asm
```

### Comparing `fv1_programmer-0.5.1/fv1_programmer/main.py` & `fv1_programmer-0.5.2/fv1_programmer/main.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/fv1_programmer/pyinstaller.py` & `fv1_programmer-0.5.2/fv1_programmer/pyinstaller.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/fv1_programmer/tui.css` & `fv1_programmer-0.5.2/fv1_programmer/tui.css`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.5.1/fv1_programmer/tui.py` & `fv1_programmer-0.5.2/fv1_programmer/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,28 @@
     Footer,
     Header,
     Static,
     RichLog,
     TabbedContent,
     TabPane,
     Switch,
-    DirectoryTree,
     TextArea,
     ContentSwitcher,
     Markdown,
 )
 
 from functools import partial
-from typing import Iterable
+from typing import Iterable, Tuple
 from pathlib import Path
 import pyperclip
 from fv1_programmer.fv1 import FV1Program, FV1_PROGRAM_MAX_BYTES
 from fv1_programmer.dialogs import *
 
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 _title = "FV1 Programmer"
 MIN_PROGRAM_NUM = 1
 MAX_PROGRAM_NUM = 8
 
 class FV1AppCommands(Provider):
     """A command provider to open a Python file in the current working directory."""
@@ -81,46 +80,55 @@
                 )
 
 
 class FV1ProgramPane(Widget):
     program : reactive[FV1Program | None] = reactive(None)
 
     def compose(self) -> ComposeResult:
-        with ContentSwitcher(initial="empty-slot"):  
-            yield Markdown(id="empty-slot")
+        with ContentSwitcher(initial="empty-slot"):
+            with VerticalScroll(id="empty-slot"):
+                yield Markdown()
             yield TextArea.code_editor("", id="text-area-slot")
 
     def watch_program(self, new_program: FV1Program):
         if new_program is not None:
             self.query_one(ContentSwitcher).current = "text-area-slot"
             self.query_one(TextArea).text = new_program.assembly
         else:
             self.query_one(ContentSwitcher).current = "empty-slot"
 
     def on_mount(self) -> None:
         self.query_one(Markdown).update("""# Empty Program Slot
-This is an empty program slot that will be ignored when downloading to the Easy Spin pedal. <br>
+This is an empty program slot that will be ignored when downloading to the Easy Spin pedal (unless you add a program). <br>
 
 To add a program to this slot, you can do one of the following:
 
-- Click here or press Ctrl+N to [create a new program for editing](#new-program)
-- Drag and drop an appropriate file onto this window (.spn, .json)
+- Click [here](#new-program) or press Ctrl+N to [create a new program for editing](#new-program)
+- Drag and drop an appropriate file onto this window (SpinASM .spn file, Audiofab fv1_programmer .json)
 
-Press *Ctrl+D* to delete a program and reset the program slot to be empty (ignored during download) <br>
+## Useful Information
+
+To bring up a command palette of possible commands, press [Ctrl+P](#command-palette). <br>
 
 Also see these helpful links: <br>
 
-Textual documentation for the editor keybindings: https://textual.textualize.io/widgets/text_area/#bindings <br>
-Easy Spin webpage: https://audiofab.com/products/easy-spin <br>
+fv1_programmer GitHub page (source and documentation): https://github.com/audiofab/fv1_programmer \n
+Easy Spin webpage: https://audiofab.com/products/easy-spin \n
+Spin Semiconductor: http://www.spinsemi.com/products.html \n
+SpinCAD Designer: https://holy-city-audio.gitbook.io/spincad-designer \n
+Mark Stratman's FV-1 Programs Directory: https://mstratman.github.io/fv1-programs/ \n
+Textual documentation for the editor keybindings: https://textual.textualize.io/widgets/text_area/#bindings \n
 """)
 
     @on(Markdown.LinkClicked)
     def on_click(self, event):
         if event.href == "#new-program":
             self.program = FV1Program("")
+        elif event.href == "#command-palette":
+            self.app.main_screen.action_command_palette()
 
     @on(TextArea.Changed)
     def on_changed(self, event):
         self.program.asm = self.query_one(TextArea).text
         self.query_one(TextArea).focus()
 
 
@@ -199,14 +207,15 @@
     BINDINGS = [
         Binding("ctrl+n", "new", "New Program", show=False, priority=True),
         Binding("ctrl+p", "command_palette", show=False, priority=True),
         Binding("ctrl+l", "load_file", "Load", priority=True),
         Binding("ctrl+s", "save", "Save", priority=True),
         Binding("ctrl+r", "read_eeprom", "Read", priority=True),
         Binding("ctrl+w", "write_eeprom", "Write", priority=True),
+        Binding("ctrl+b", "assemble_programs", "Assemble", priority=True),
         ("f1", "app.toggle_class('RichLog', '-hidden')", "Log"),
         ("f2", "toggle_sidebar", "Settings"),
         ("ctrl+q", "request_quit", "Quit"),
     ]
     COMMANDS = {FV1AppCommands}
 
     show_sidebar = reactive(False)
@@ -386,39 +395,48 @@
                     self.app.push_screen(YesNoScreen("File exists. Overwrite?"), check_overwrite)
 
                 else:
                     do_save_file(save_path)
 
         self.app.push_screen(SaveFileScreen(), handle_save_file)
 
-    def action_write_eeprom(self) -> None:
+    def action_assemble_programs(self,) -> Tuple[Iterable, int]:
         programs = []
-        errors = 0
+        num_errors = 0
         for i in range(MIN_PROGRAM_NUM, MAX_PROGRAM_NUM + 1):
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
             if program_pane.program is not None:
                 bin_array = self.assemble_and_validate_program(program_pane.program)
                 if bin_array is not None:
                     if len(bin_array):
                         programs.append({"program": i, "address" : (i - 1)*FV1_PROGRAM_MAX_BYTES, "data" : bin_array})
                     else:
                         # Program assembled but there are no instructions
                         self.app.show_toast(f"Program {i} has no instructions.")
                 else:
                     self.app.show_toast(f"Program {i} failed to assemble. See log for details.")
-                    errors += 1
+                    num_errors += 1
 
-        if errors > 0:
-            self.app.show_toast("Errors while assembling. Download aborted.", severity="warning")
-        else:
-            if len(programs) == 0:
-                self.app.show_toast("Nothing to do!", severity="warning")
-            else:
-                self.app.push_screen(BusyScreen("Downloading to pedal..."))
-                self.write_eeprom(programs, self.app.setting_simulate)
+        if num_errors > 0:
+            self.app.show_toast("Errors while assembling.", severity="warning")
+
+        if len(programs) == 0:
+            self.app.show_toast("Nothing to do!", severity="warning")
+
+        if num_errors == 0 and len(programs):
+            self.app.show_toast(f"Successfully assembled {len(programs)} programs.", severity="info")
+
+        return programs, num_errors
+
+    def action_write_eeprom(self) -> None:
+        programs, num_errors = self.action_assemble_programs()
+
+        if num_errors == 0 and len(programs):
+            self.app.push_screen(BusyScreen("Downloading to pedal..."))
+            self.write_eeprom(programs, self.app.setting_simulate)
 
     def _get_eeprom(self,):
         if self.app.setting_simulate:
             from eeprom.eeprom import DummyEEPROM
             return DummyEEPROM(Path(self.app.cmdline_args.sim), self.app.cmdline_args.ee_size)
         else:
             from adaptor.mcp2221 import MCP2221I2CAdaptor
@@ -543,24 +561,44 @@
         else:
             self.app.show_toast("EEPROM read complete.")
 
     def action_delete(self) -> None:
         active_tab_id = self.query_one(TabbedContent).active
         active_slot = active_tab_id.split("prog")[1]
         active_program_pane = self.query_one(f"#fv1{active_tab_id}", FV1ProgramPane)
-        active_program_pane.program = None
-        self.rename_program_slot(active_slot, f"Program {active_slot}")
+
+        def do_delete_program():
+            active_program_pane.program = None
+            self.rename_program_slot(active_slot, f"Program {active_slot}")
+
+        if active_program_pane.program is not None:
+            def check_overwrite(should_overwrite : bool) -> None:
+                if should_overwrite:
+                    do_delete_program()
+            self.app.push_screen(YesNoScreen("Reset current slot?"), check_overwrite)
+        else:
+            do_delete_program()
 
     def action_new(self) -> None:
         active_tab_id = self.query_one(TabbedContent).active
         active_slot = active_tab_id.split("prog")[1]
         active_program_pane = self.query_one(f"#fv1{active_tab_id}", FV1ProgramPane)
-        active_program_pane.program = FV1Program("")
-        self.rename_program_slot(active_slot, f"Program {active_slot}")
-        active_program_pane.query_one(TextArea).focus()
+
+        def do_new_program():
+            active_program_pane.program = FV1Program("")
+            self.rename_program_slot(active_slot, f"Program {active_slot}")
+            active_program_pane.query_one(TextArea).focus()
+
+        if active_program_pane.program is not None:
+            def check_overwrite(should_overwrite : bool) -> None:
+                if should_overwrite:
+                    do_new_program()
+            self.app.push_screen(YesNoScreen("Replace current program with an empty one?"), check_overwrite)
+        else:
+            do_new_program()
 
     def assemble_and_validate_program(self, program) -> bytearray:
         bin_array, num_instructions, warnings, errors = program.assemble(clamp=self.app.setting_asfv1_clamp,
                                                                          spinreals=self.app.setting_asfv1_spinreals)
         [self.app.logger.info(w) for w in warnings]
         [self.app.logger.info(e) for e in errors]
         if len(errors) == 0:
@@ -640,7 +678,11 @@
         super().exit(result)
 
     def on_mount(self) -> None:
         self.push_screen("main")
 
     def show_toast(self, message, title=None, severity="information", timeout=4.0) -> None:
         self.notify(message, title=title, severity=severity, timeout=timeout)
+
+    @property
+    def main_screen(self,) -> Screen:
+        return self.SCREENS["main"]
```

### Comparing `fv1_programmer-0.5.1/pyproject.toml` & `fv1_programmer-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fv1-programmer"
-version = "0.5.1"
+version = "0.5.2"
 homepage = "https://github.com/audiofab/fv1_programmer"
 description = "An FV-1 assembler/disassembler and EEPROM programming tool for the Spin Semiconductor FV-1 DSP"
 authors = ["Mark Melvin <mark.melvin@audiofab.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `fv1_programmer-0.5.1/PKG-INFO` & `fv1_programmer-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fv1-programmer
-Version: 0.5.1
+Version: 0.5.2
 Summary: An FV-1 assembler/disassembler and EEPROM programming tool for the Spin Semiconductor FV-1 DSP
 Home-page: https://github.com/audiofab/fv1_programmer
 License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@audiofab.com
 Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -56,15 +56,15 @@
 
 ```
 $ fv1_programmer
 ```
 
 This will bring up a user interface that will allow you to configure all 8 program slots of the Easy Spin's FV-1 DSP and write the EEPROM.
 
-![image](https://github.com/audiofab/fv1_programmer/assets/1384978/36d8e9b9-4fe6-4cc4-b7b3-194910aaff97)
+![image](https://github.com/audiofab/fv1_programmer/assets/1384978/300f1d0a-0dfc-4b63-8364-a8b2a8e76c65)
 
 NOTE: On Linux you likely still need to install `libusb` and add a udev rule separately. See [Ubuntu Linux](README.md#Ubuntu-linux).
 
 ## Using One Of The Pre-Built Binaries
 
 ### Windows
 
@@ -106,7 +106,8 @@
 
 
 # Known Issues
 
 ## Drag and drop not working reliably
 
 On Windows 10 Terminal we have seen some issues with drag and drop not always working reliably. If you find that dragging a file from Explorer onto the application is not working, try dropping the file on the upper part of the user-interface (or even on the Program tabs) instead.
+
```

