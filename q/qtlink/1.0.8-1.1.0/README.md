# Comparing `tmp/qtlink-1.0.8.tar.gz` & `tmp/qtlink-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.0.8.tar", last modified: Sat Apr  6 06:18:11 2024, max compression
+gzip compressed data, was "qtlink-1.1.0.tar", last modified: Wed Apr 10 12:06:38 2024, max compression
```

## Comparing `qtlink-1.0.8.tar` & `qtlink-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 06:18:11.378814 qtlink-1.0.8/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      515 2024-04-06 06:18:11.375077 qtlink-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 06:18:11.347523 qtlink-1.0.8/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-04 02:24:16.000000 qtlink-1.0.8/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 06:18:11.366078 qtlink-1.0.8/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.0.8/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.0.8/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.0.8/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1874 2024-04-03 12:51:18.000000 qtlink-1.0.8/qtlink/dialog/dialog_use_table.py
-drwxrwxrwx   0        0        0        0 2024-04-06 06:18:11.367076 qtlink-1.0.8/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.8/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     1887 2024-04-06 06:14:57.000000 qtlink-1.0.8/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-06 06:18:11.370076 qtlink-1.0.8/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.8/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     5653 2024-04-05 13:55:23.000000 qtlink-1.0.8/qtlink/table/multiple_select_table_controller.py
--rw-rw-rw-   0        0        0     2107 2024-04-05 13:55:23.000000 qtlink-1.0.8/qtlink/table/single_select_table_controller.py
--rw-rw-rw-   0        0        0     6207 2024-04-05 13:55:23.000000 qtlink-1.0.8/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     3645 2024-04-04 02:24:16.000000 qtlink-1.0.8/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-06 06:18:11.373079 qtlink-1.0.8/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.0.8/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.0.8/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.0.8/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-06 06:18:11.374080 qtlink-1.0.8/qtlink.egg-info/
--rw-rw-rw-   0        0        0      515 2024-04-06 06:18:11.000000 qtlink-1.0.8/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2024-04-06 06:18:11.000000 qtlink-1.0.8/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 06:18:11.000000 qtlink-1.0.8/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-06 06:18:11.000000 qtlink-1.0.8/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-06 06:18:11.000000 qtlink-1.0.8/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 06:18:11.378814 qtlink-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      660 2024-04-06 06:17:55.000000 qtlink-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:06:38.077870 qtlink-1.1.0/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-04-10 12:06:38.077870 qtlink-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 12:06:38.046566 qtlink-1.1.0/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.1.0/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:06:38.062229 qtlink-1.1.0/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.1.0/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.1.0/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.1.0/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     1406 2024-04-10 11:53:14.000000 qtlink-1.1.0/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     1086 2024-04-10 11:53:14.000000 qtlink-1.1.0/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:06:38.077870 qtlink-1.1.0/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.0/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     1971 2024-04-10 06:55:58.000000 qtlink-1.1.0/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:06:38.077870 qtlink-1.1.0/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.1.0/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     6668 2024-04-10 12:00:18.000000 qtlink-1.1.0/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     5455 2024-04-10 11:53:14.000000 qtlink-1.1.0/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     1919 2024-04-10 11:59:10.000000 qtlink-1.1.0/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     3647 2024-04-10 12:00:18.000000 qtlink-1.1.0/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:06:38.077870 qtlink-1.1.0/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.1.0/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.1.0/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.1.0/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:06:38.077870 qtlink-1.1.0/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-04-10 12:06:38.000000 qtlink-1.1.0/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-10 12:06:38.000000 qtlink-1.1.0/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 12:06:38.000000 qtlink-1.1.0/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-10 12:06:38.000000 qtlink-1.1.0/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 12:06:38.000000 qtlink-1.1.0/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 12:06:38.077870 qtlink-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      660 2024-04-10 12:06:36.000000 qtlink-1.1.0/setup.py
```

### Comparing `qtlink-1.0.8/LICENSE` & `qtlink-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.8/PKG-INFO` & `qtlink-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.0.8
+Version: 1.1.0
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.0.8/qtlink/dialog/dialog_choice.py` & `qtlink-1.1.0/qtlink/dialog/dialog_choice.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.8/qtlink/dialog/dialog_info.py` & `qtlink-1.1.0/qtlink/dialog/dialog_info.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.8/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.1.0/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from PySide6.QtWidgets import QVBoxLayout, QWidget
-from matplotlib import pyplot as plt
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas, \
-    NavigationToolbar2QT as NavigationToolbar
-from matplotlib.figure import Figure
-
-plt.rcParams['font.sans-serif'] = ['SimHei']  # 用来正常显示中文标签
-plt.rcParams['axes.unicode_minus'] = False  # 用来正常显示负号
+from PySide6.QtWidgets import QWidget
 
 
 class MplCanvas(QWidget):
     def __init__(self, enable_toolbar: bool = True, parent=None):
-        super(MplCanvas, self).__init__(parent)
+        from matplotlib import pyplot as plt
+        from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas, \
+            NavigationToolbar2QT as NavigationToolbar
+        from matplotlib.figure import Figure
+        from PySide6.QtWidgets import QVBoxLayout
+        plt.rcParams['font.sans-serif'] = ['SimHei']  # 用来正常显示中文标签
+        plt.rcParams['axes.unicode_minus'] = False  # 用来正常显示负号
 
+        super(MplCanvas, self).__init__(parent)
         self.canvas = FigureCanvas(Figure(figsize=(5, 4), constrained_layout=True))
         self.ax = self.canvas.figure.subplots()
 
         self.vertical_layout = QVBoxLayout()
         if enable_toolbar:
             self.toolbar = NavigationToolbar(self.canvas, self)
             self.vertical_layout.addWidget(self.toolbar)
```

### Comparing `qtlink-1.0.8/qtlink/table/multiple_select_table_controller.py` & `qtlink-1.1.0/qtlink/table/table_controller_multiple_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 # -*- coding:utf-8 -*-
 from PySide6.QtCore import Qt, QRect
 from PySide6.QtGui import QStandardItem
-from PySide6.QtWidgets import QTableView, QStyleOptionButton, QStyle, QHeaderView
+from PySide6.QtWidgets import QStyleOptionButton, QStyle, QHeaderView
 
 from qtlink.table.table_controller import TableController
 from qtlink.util import create_signal
 
 
-class MultipleSelectTableController(TableController):
-    def __init__(self, tableview: QTableView):
+class TableControllerMultipleCheck(TableController):
+    def __init__(self, tableview):
         super().__init__(tableview)
         self.model.itemChanged.connect(self.on_item_changed)
-        self.signal_select_rows = create_signal(list)
+        self.signal_checked_rows = create_signal(list)
 
         self.header = CustomHeader(toggle_check_state=self.toggle_check_state, parent=self.tableview)
         self.tableview.setHorizontalHeader(self.header)
 
         self.always_checked_data = []
 
-    def update_model_data(self, model_data: list[dict],
+    def update_table_data(self, table_data: list[dict],
                           hide_columns: list[str] = None,
                           always_checked_data: list = None):
         # 断开信号连接
         self.model.itemChanged.disconnect(self.on_item_changed)
 
+        self.before_update_table_data(table_data)
+        self.always_checked_data = always_checked_data if always_checked_data else []
+
         if hide_columns is None:
             hide_columns = []
-        if not self.first_load:
-            # 保存当前列宽
-            self.save_current_column_widths()
-        self.first_load = False
-
-        self.model.clear()
-        self.raw_data = model_data
-        self.always_checked_data = always_checked_data if always_checked_data else []
-        for data in model_data:
+        for data in table_data:
             items = [QStandardItem(str(data.get(column, None)) if data.get(column, None) is not None else '')
                      for column in self.table_columns
                      if column not in hide_columns]
             items[0].setCheckable(True)
             if data in self.always_checked_data:
                 items[0].setCheckState(Qt.Checked)
                 # 禁用交互
                 for item in items:
                     item.setFlags(Qt.ItemIsUserCheckable | Qt.ItemIsSelectable)
-
             self.model.appendRow(items)
-        self.update_table_columns(self.table_columns)
+
+        self.set_table()
         # 重新连接信号
         self.model.itemChanged.connect(self.on_item_changed)
         self.on_item_changed()
 
     def toggle_check_state(self, is_checked):
         # 断开信号连接
         self.model.itemChanged.disconnect(self.on_item_changed)
@@ -61,28 +56,28 @@
             if self.raw_data[row] not in self.always_checked_data:
                 item.setCheckState(Qt.Checked if is_checked else Qt.Unchecked)
 
         # 重新连接信号
         self.model.itemChanged.connect(self.on_item_changed)
         self.on_item_changed()
 
-    def get_checked_rows(self):
+    def get_checked_rows(self) -> list[dict]:
         checked_rows = []
         for row in range(self.model.rowCount()):
             item = self.model.item(row, 0)  # 勾选框在第一列
             if item.checkState() == Qt.Checked:
                 checked_rows.append(self.raw_data[row])
         return checked_rows
 
     def on_item_changed(self, item: QStandardItem = None):
         if self.hover_delegate is not None and self.hover_delegate.is_hovering:
             return
 
         checked_rows = self.get_checked_rows()
-        self.signal_select_rows.signal.emit(checked_rows)
+        self.signal_checked_rows.signal.emit(checked_rows)
         checked_rows_num = len(checked_rows)
         if checked_rows_num and checked_rows_num == len(self.raw_data):
             self.set_header_check_state(True)
         else:
             self.set_header_check_state(False)
 
     def set_header_check_state(self, is_checked: bool):
```

### Comparing `qtlink-1.0.8/qtlink/table/single_select_table_controller.py` & `qtlink-1.1.0/qtlink/table/table_controller_single_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 # -*- coding:utf-8 -*-
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QStandardItem
-from PySide6.QtWidgets import QTableView
 
 from qtlink.table.table_controller import TableController
 from qtlink.util import create_signal
 
 
-class SingleSelectTableController(TableController):
-    def __init__(self, tableview: QTableView):
+class TableControllerSingleCheck(TableController):
+    def __init__(self, tableview):
         super().__init__(tableview)
         self.model.itemChanged.connect(self.on_item_changed)
-        self.signal_select_row = create_signal(dict)
+        self.signal_checked_rows = create_signal(list)
 
-    def update_model_data(self, model_data: list[dict], hide_columns: list[str] = None):
+    def update_table_data(self, table_data: list[dict], hide_columns: list[str] = None):
         # 断开信号连接
         self.model.itemChanged.disconnect(self.on_item_changed)
 
+        self.before_update_table_data(table_data)
         if hide_columns is None:
             hide_columns = []
-        if not self.first_load:
-            # 保存当前列宽
-            self.save_current_column_widths()
-        self.first_load = False
-
-        self.model.clear()
-        self.raw_data = model_data
-        for data in model_data:
+        for data in table_data:
             items = [QStandardItem(str(data.get(column, None)) if data.get(column, None) is not None else '')
                      for column in self.table_columns
                      if column not in hide_columns]
             items[0].setCheckable(True)
             self.model.appendRow(items)
-        self.update_table_columns(self.table_columns)
+
+        self.set_table()
         # 重新连接信号
         self.model.itemChanged.connect(self.on_item_changed)
         self.on_item_changed()
 
     def on_item_changed(self, item: QStandardItem = None):
         if item is None or item.checkState() != Qt.Checked:
             return
 
         for row in range(self.model.rowCount()):
             if self.model.item(row, 0) != item:
                 self.model.item(row, 0).setCheckState(Qt.Unchecked)
+        checked_rows = self.get_checked_rows()
+        self.signal_checked_rows.signal.emit(checked_rows)
 
-        self.signal_select_row.signal.emit(self.raw_data[item.row()])
-
-    def get_checked_row(self):
+    def get_checked_rows(self) -> list[dict]:
         for row in range(self.model.rowCount()):
             item = self.model.item(row, 0)  # 勾选框在第一列
             if item.checkState() == Qt.Checked:
-                return self.raw_data[row]
+                return [self.raw_data[row], ]
```

### Comparing `qtlink-1.0.8/qtlink/table/table_controller.py` & `qtlink-1.1.0/qtlink/table/table_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding:utf-8 -*-
-from PySide6 import QtGui, QtCore
-from PySide6.QtCore import QItemSelectionModel, Qt
-from PySide6.QtGui import QStandardItem
-from PySide6.QtWidgets import QTableView
+from collections import OrderedDict
+
+from PySide6.QtCore import QItemSelectionModel, Qt, QObject, QModelIndex, QEvent
+from PySide6.QtGui import QStandardItem, QColor, QStandardItemModel
 
 from qtlink.util import create_signal
 
 
 class TableController:
-    def __init__(self, tableview: QTableView,
-                 highlight_hover_row: bool = False):
+    def __init__(self, tableview, highlight_hover_row: bool = False):
         self.tableview = tableview
-        self.table_columns = None
+        self.table_columns = []
         self.raw_data = None
         self.column_widths = None
         self.first_load = True
-        self.model = QtGui.QStandardItemModel()
+        self.model = QStandardItemModel()
         self.signal_click_row = create_signal(dict)
         # 连接信号
         self.tableview.clicked.connect(self.on_table_clicked)
         # 禁止上下文菜单
         scrollBar = self.tableview.verticalScrollBar()
         scrollBar.setContextMenuPolicy(Qt.NoContextMenu)
         scrollBar = self.tableview.horizontalScrollBar()
@@ -28,43 +27,57 @@
         if highlight_hover_row:
             self.tableview.setMouseTracking(True)
             self.hover_delegate = HoverDelegate(tableview=tableview)
             self.tableview.entered.connect(self.hover_delegate.on_entered)
         else:
             self.hover_delegate = None
 
-    def update_model_data(self, model_data: list[dict], hide_columns: list[str] = None):
+    def update_table_data(self, table_data: list[dict], hide_columns: list[str] = None):
+        self.before_update_table_data(table_data)
+
         if hide_columns is None:
             hide_columns = []
+        for data in table_data:
+            items = [QStandardItem(str(data.get(column, None)) if data.get(column, None) is not None else '')
+                     for column in self.table_columns
+                     if column not in hide_columns]
+            self.model.appendRow(items)
+
+        self.set_table()
+
+    def before_update_table_data(self, table_data):
         if not self.first_load:
             # 保存当前列宽
             self.save_current_column_widths()
         self.first_load = False
-
+        self.raw_data = table_data
+        # 传入空数据将不会影响表头。用于传过数据，后来清空后保持显示表头的场景。
+        if table_data:
+            self.table_columns = self.get_table_columns_from_data(table_data)
         self.model.clear()
-        self.raw_data = model_data
-        for data in model_data:
-            items = [QStandardItem(str(data.get(column, None)) if data.get(column, None) is not None else '')
-                     for column in self.table_columns
-                     if column not in hide_columns]
-            self.model.appendRow(items)
-        self.update_table_columns(self.table_columns)
 
-    def update_table_columns(self, table_columns: list[str]):
-        self.table_columns = table_columns
-        self.model.setHorizontalHeaderLabels(table_columns)
+    def set_table(self):
+        self.model.setHorizontalHeaderLabels(self.table_columns)
         self.tableview.setModel(self.model)
 
         if self.column_widths is not None:
             for item in self.column_widths:
                 index, width = item
                 self.tableview.setColumnWidth(index, width)
 
-    def clear_model_data(self):
-        self.update_model_data(model_data=[])
+    def get_table_columns_from_data(self, data: list[dict]):
+        ordered_keys = OrderedDict()
+        for d in data:
+            for key in d.keys():
+                ordered_keys[key] = None
+        # 将OrderedDict的键转换为列表
+        return list(ordered_keys.keys())
+
+    def clear_table_data(self):
+        self.update_table_data(table_data=[])
 
     def save_current_column_widths(self):
         if self.column_widths is None:
             return
         for index in range(self.model.columnCount()):
             width = self.tableview.columnWidth(index)
             # 确保保存的列宽信息与列的数量相匹配
@@ -96,29 +109,29 @@
                                                    QItemSelectionModel.Deselect | QItemSelectionModel.Rows)
 
     def __del__(self):
         if self.hover_delegate and self.tableview.viewport():
             self.tableview.viewport().removeEventFilter(self.hover_delegate)
 
 
-class HoverDelegate(QtCore.QObject):
+class HoverDelegate(QObject):
     def __init__(self, tableview):
         super().__init__(tableview)
         self.tableview = tableview
         self.row_under_mouse = -1
-        self.hover_color = QtGui.QColor(240, 240, 240)
+        self.hover_color = QColor(240, 240, 240)
         # 安装事件过滤器到表格视图的视口上
         self.tableview.viewport().installEventFilter(self)
         self.is_hovering = False
 
     def on_entered(self, index):
         self.is_hovering = True
         hover_row = index.row()
         # 检查当前行是否被选中
-        is_row_selected = self.tableview.selectionModel().isRowSelected(hover_row, QtCore.QModelIndex())
+        is_row_selected = self.tableview.selectionModel().isRowSelected(hover_row, QModelIndex())
         if hover_row != self.row_under_mouse:
             # 还原上一行的背景色
             if self.row_under_mouse >= 0:
                 self.set_row_background(self.row_under_mouse, self.tableview.palette().base())
             # 重设当前行背景色
             if not is_row_selected:
                 self.set_row_background(hover_row, self.hover_color)
@@ -135,10 +148,10 @@
     def clear_hover_style(self):
         if self.row_under_mouse >= 0:
             self.set_row_background(self.row_under_mouse, self.tableview.palette().base())
             self.row_under_mouse = -1
             self.tableview.viewport().update()  # 更新视图以反映背景色的变化
 
     def eventFilter(self, watched, event):
-        if watched and watched == self.tableview.viewport() and event.type() == QtCore.QEvent.Leave:  # noqa
+        if watched and watched == self.tableview.viewport() and event.type() == QEvent.Leave:
             self.clear_hover_style()
         return super().eventFilter(watched, event)
```

### Comparing `qtlink-1.0.8/qtlink/util.py` & `qtlink-1.1.0/qtlink/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from PySide6.QtCore import QObject, Signal
 
 
 def create_signal(signal_type):
     """根据传入类型，创建相应的信号类。"""
+
     class CustomSignal(QObject):
         signal = Signal(signal_type)
 
     return CustomSignal()
 
 
 class ResponseProgressSignal:
```

### Comparing `qtlink-1.0.8/qtlink/widgets/drop_widget.py` & `qtlink-1.1.0/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.8/qtlink/widgets/list_widget.py` & `qtlink-1.1.0/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.8/qtlink.egg-info/PKG-INFO` & `qtlink-1.1.0/qtlink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.0.8
+Version: 1.1.0
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.0.8/qtlink.egg-info/SOURCES.txt` & `qtlink-1.1.0/qtlink.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 qtlink.egg-info/SOURCES.txt
 qtlink.egg-info/dependency_links.txt
 qtlink.egg-info/requires.txt
 qtlink.egg-info/top_level.txt
 qtlink/dialog/__init__.py
 qtlink/dialog/dialog_choice.py
 qtlink/dialog/dialog_info.py
-qtlink/dialog/dialog_use_table.py
+qtlink/dialog/dialog_table_check.py
+qtlink/dialog/dialog_table_display.py
 qtlink/mpl_canvas/__init__.py
 qtlink/mpl_canvas/mpl_canvas.py
 qtlink/table/__init__.py
-qtlink/table/multiple_select_table_controller.py
-qtlink/table/single_select_table_controller.py
 qtlink/table/table_controller.py
+qtlink/table/table_controller_multiple_check.py
+qtlink/table/table_controller_single_check.py
 qtlink/widgets/__init__.py
 qtlink/widgets/drop_widget.py
 qtlink/widgets/list_widget.py
```

