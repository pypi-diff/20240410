# Comparing `tmp/guidata-3.4.1.tar.gz` & `tmp/guidata-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guidata-3.4.1.tar", last modified: Tue Mar 12 13:00:34 2024, max compression
+gzip compressed data, was "guidata-3.5.0.tar", last modified: Wed Apr 10 16:45:22 2024, max compression
```

## Comparing `guidata-3.4.1.tar` & `guidata-3.5.0.tar`

### file list

```diff
@@ -1,251 +1,259 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.091486 guidata-3.4.1/
--rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.4.1/LICENSE
--rw-rw-rw-   0        0        0       28 2023-07-28 10:11:21.000000 guidata-3.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6433 2024-03-12 13:00:34.091486 guidata-3.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2635 2023-11-14 15:48:02.000000 guidata-3.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.841097 guidata-3.4.1/doc/
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.841097 guidata-3.4.1/doc/_static/
--rw-rw-rw-   0        0        0    97375 2023-06-30 10:35:52.000000 guidata-3.4.1/doc/_static/favicon.ico
--rw-rw-rw-   0        0        0      689 2023-10-13 14:59:49.000000 guidata-3.4.1/doc/basic_example.py
--rw-rw-rw-   0        0        0       63 2024-03-06 10:46:03.000000 guidata-3.4.1/doc/changelog.rst
--rw-rw-rw-   0        0        0     1548 2024-03-06 10:46:03.000000 guidata-3.4.1/doc/conf.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.841097 guidata-3.4.1/doc/dev/
--rw-rw-rw-   0        0        0     4059 2024-03-06 10:46:03.000000 guidata-3.4.1/doc/dev/contribute.rst
--rw-rw-rw-   0        0        0      979 2023-10-16 12:31:43.000000 guidata-3.4.1/doc/dev/howto.rst
--rw-rw-rw-   0        0        0      136 2023-09-15 16:28:17.000000 guidata-3.4.1/doc/dev/index.rst
--rw-rw-rw-   0        0        0     4030 2023-10-16 12:31:51.000000 guidata-3.4.1/doc/dev/platform.rst
--rw-rw-rw-   0        0        0     2305 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/dev/v2_to_v3.csv
--rw-rw-rw-   0        0        0     1186 2023-07-26 08:50:26.000000 guidata-3.4.1/doc/dev/v2_to_v3.rst
--rw-rw-rw-   0        0        0     2733 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/examples.rst
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.856735 guidata-3.4.1/doc/images/
--rw-rw-rw-   0        0        0     4744 2023-10-23 07:39:27.000000 guidata-3.4.1/doc/images/basic_example.png
--rw-rw-rw-   0        0        0    19715 2023-10-05 13:52:55.000000 guidata-3.4.1/doc/images/guidata-banner.png
--rw-rw-rw-   0        0        0     6669 2023-10-05 13:53:17.000000 guidata-3.4.1/doc/images/guidata-vertical.png
--rw-rw-rw-   0        0        0    14799 2023-07-06 12:21:56.000000 guidata-3.4.1/doc/images/layout_example.png
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.872357 guidata-3.4.1/doc/images/screenshots/
--rw-rw-rw-   0        0        0    84779 2023-10-23 07:18:39.000000 guidata-3.4.1/doc/images/screenshots/__init__.png
--rw-rw-rw-   0        0        0     4672 2023-10-23 07:20:07.000000 guidata-3.4.1/doc/images/screenshots/activable_dataset.png
--rw-rw-rw-   0        0        0    33244 2023-10-23 07:21:39.000000 guidata-3.4.1/doc/images/screenshots/all_features.png
--rw-rw-rw-   0        0        0    38960 2023-10-23 07:22:03.000000 guidata-3.4.1/doc/images/screenshots/all_items.png
--rw-rw-rw-   0        0        0    23930 2023-10-23 07:24:03.000000 guidata-3.4.1/doc/images/screenshots/arrayeditor.png
--rw-rw-rw-   0        0        0     7935 2023-10-23 07:22:22.000000 guidata-3.4.1/doc/images/screenshots/bool_selector.png
--rw-rw-rw-   0        0        0    43676 2023-10-23 07:25:56.000000 guidata-3.4.1/doc/images/screenshots/codeeditor.png
--rw-rw-rw-   0        0        0    25840 2023-10-23 07:26:40.000000 guidata-3.4.1/doc/images/screenshots/collectioneditor.png
--rw-rw-rw-   0        0        0    14535 2023-10-23 07:30:05.000000 guidata-3.4.1/doc/images/screenshots/console.png
--rw-rw-rw-   0        0        0    16805 2023-10-23 07:30:34.000000 guidata-3.4.1/doc/images/screenshots/dataframeeditor.png
--rw-rw-rw-   0        0        0    33475 2023-10-23 07:22:51.000000 guidata-3.4.1/doc/images/screenshots/datasetgroup.png
--rw-rw-rw-   0        0        0    25030 2023-10-23 07:23:14.000000 guidata-3.4.1/doc/images/screenshots/editgroupbox.png
--rw-rw-rw-   0        0        0    15365 2023-10-23 07:31:04.000000 guidata-3.4.1/doc/images/screenshots/importwizard.png
--rw-rw-rw-   0        0        0     1214 2024-03-06 10:46:03.000000 guidata-3.4.1/doc/index.rst
--rw-rw-rw-   0        0        0      540 2023-07-26 16:55:42.000000 guidata-3.4.1/doc/installation.rst
--rw-rw-rw-   0        0        0     2371 2023-10-23 07:35:32.000000 guidata-3.4.1/doc/overview.rst
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.872357 guidata-3.4.1/doc/reference/
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.888011 guidata-3.4.1/doc/reference/dataset/
--rw-rw-rw-   0        0        0       54 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/reference/dataset/conv.rst
--rw-rw-rw-   0        0        0       59 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/reference/dataset/dataitems.rst
--rw-rw-rw-   0        0        0       59 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/reference/dataset/datatypes.rst
--rw-rw-rw-   0        0        0      153 2023-10-13 07:23:56.000000 guidata-3.4.1/doc/reference/dataset/index.rst
--rw-rw-rw-   0        0        0       42 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/reference/dataset/io.rst
--rw-rw-rw-   0        0        0       59 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/reference/dataset/qtwidgets.rst
--rw-rw-rw-   0        0        0       49 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/reference/guitest.rst
--rw-rw-rw-   0        0        0      148 2023-07-07 14:21:56.000000 guidata-3.4.1/doc/reference/index.rst
--rw-rw-rw-   0        0        0       50 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/reference/userconfig.rst
--rw-rw-rw-   0        0        0      146 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/reference/utils.rst
--rw-rw-rw-   0        0        0      136 2024-03-07 13:48:08.000000 guidata-3.4.1/doc/reference/widgets.rst
--rw-rw-rw-   0        0        0     2412 2024-03-11 07:41:58.000000 guidata-3.4.1/doc/requirements.rst
--rw-rw-rw-   0        0        0      721 2023-07-28 12:41:06.000000 guidata-3.4.1/doc/update_requirements.py
--rw-rw-rw-   0        0        0     1699 2023-10-23 07:56:54.000000 guidata-3.4.1/doc/widgets.rst
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.888011 guidata-3.4.1/guidata/
--rw-rw-rw-   0        0        0     3047 2024-03-12 12:58:40.000000 guidata-3.4.1/guidata/__init__.py
--rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.4.1/guidata/config.py
--rw-rw-rw-   0        0        0    13841 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/configtools.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.919261 guidata-3.4.1/guidata/dataset/
--rw-rw-rw-   0        0        0     1059 2024-03-07 08:15:01.000000 guidata-3.4.1/guidata/dataset/__init__.py
--rw-rw-rw-   0        0        0     6974 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/dataset/conv.py
--rw-rw-rw-   0        0        0    35333 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/dataset/dataitems.py
--rw-rw-rw-   0        0        0    48063 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/dataset/datatypes.py
--rw-rw-rw-   0        0        0      557 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/dataset/io.py
--rw-rw-rw-   0        0        0    50712 2024-03-11 07:41:58.000000 guidata-3.4.1/guidata/dataset/qtitemwidgets.py
--rw-rw-rw-   0        0        0    35733 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/dataset/qtwidgets.py
--rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.4.1/guidata/dataset/textedit.py
--rw-rw-rw-   0        0        0     9603 2024-03-08 10:00:31.000000 guidata-3.4.1/guidata/env.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.919261 guidata-3.4.1/guidata/external/
--rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/external/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.919261 guidata-3.4.1/guidata/external/darkdetect/
--rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/external/darkdetect/__init__.py
--rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/external/darkdetect/_dummy.py
--rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/external/darkdetect/_linux_detect.py
--rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/external/darkdetect/_mac_detect.py
--rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/external/darkdetect/_windows_detect.py
--rw-rw-rw-   0        0        0    11402 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/guitest.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.966538 guidata-3.4.1/guidata/images/
--rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/apply.png
--rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/arredit.png
--rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/busy.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/cell_edit.png
--rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/copy.png
--rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/delete.png
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/dictedit.png
--rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/dtype.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/edit.png
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.982163 guidata-3.4.1/guidata/images/editors/
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/copywop.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/edit.png
--rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/edit_add.png
--rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/editclear.png
--rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/editcopy.png
--rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/editcut.png
--rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/editdelete.png
--rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/editpaste.png
--rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/fileimport.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/filesave.png
--rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/imshow.png
--rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/insert.png
--rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/plot.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/rename.png
--rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/editors/selectall.png
--rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/exit.png
--rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/expander_down.png
--rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/expander_right.png
--rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/file.png
--rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/fileclose.png
--rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/fileimport.png
--rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filenew.png
--rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/fileopen.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filesave.png
--rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filesaveas.png
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.997787 guidata-3.4.1/guidata/images/filetypes/
--rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/doc.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/gif.png
--rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/html.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/jpg.png
--rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/pdf.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/png.png
--rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/pps.png
--rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/ps.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/tar.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/tgz.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/tif.png
--rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/txt.png
--rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/xls.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/filetypes/zip.png
--rw-rw-rw-   0        0        0    16638 2023-10-05 13:53:25.000000 guidata-3.4.1/guidata/images/guidata-banner.svg
--rw-rw-rw-   0        0        0    16610 2023-10-05 13:53:21.000000 guidata-3.4.1/guidata/images/guidata-vertical.svg
--rw-rw-rw-   0        0        0    15960 2023-10-05 13:53:23.000000 guidata-3.4.1/guidata/images/guidata.svg
--rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/max.png
--rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/min.png
--rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/none.png
--rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/not_found.png
--rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/python.png
--rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/quickview.png
--rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/save_all.png
--rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/selection.png
--rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/settings.png
--rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/shape.png
--rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/xmax.png
--rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/images/xmin.png
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.997787 guidata-3.4.1/guidata/io/
--rw-rw-rw-   0        0        0     1738 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/io/__init__.py
--rw-rw-rw-   0        0        0     5905 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/io/base.py
--rw-rw-rw-   0        0        0    27914 2024-03-08 14:33:38.000000 guidata-3.4.1/guidata/io/h5fmt.py
--rw-rw-rw-   0        0        0     5138 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/io/inifmt.py
--rw-rw-rw-   0        0        0    10386 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/io/jsonfmt.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.809449 guidata-3.4.1/guidata/locale/
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.809449 guidata-3.4.1/guidata/locale/fr/
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.997787 guidata-3.4.1/guidata/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    13149 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/locale/fr/LC_MESSAGES/guidata.mo
--rw-rw-rw-   0        0        0    20041 2024-03-08 09:10:42.000000 guidata-3.4.1/guidata/qthelpers.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.997787 guidata-3.4.1/guidata/tests/
--rw-rw-rw-   0        0        0      653 2023-10-23 09:01:21.000000 guidata-3.4.1/guidata/tests/__init__.py
--rw-rw-rw-   0        0        0      189 2024-03-11 07:41:58.000000 guidata-3.4.1/guidata/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:33.809449 guidata-3.4.1/guidata/tests/data/
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.013419 guidata-3.4.1/guidata/tests/data/genreqs/
--rw-rw-rw-   0        0        0     1918 2023-10-16 13:20:05.000000 guidata-3.4.1/guidata/tests/data/genreqs/pyproject.toml
--rw-rw-rw-   0        0        0     1475 2023-09-18 09:39:00.000000 guidata-3.4.1/guidata/tests/data/genreqs/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.028963 guidata-3.4.1/guidata/tests/dataset/
--rw-rw-rw-   0        0        0        0 2023-10-23 07:10:13.000000 guidata-3.4.1/guidata/tests/dataset/__init__.py
--rw-rw-rw-   0        0        0     1756 2024-03-07 07:58:12.000000 guidata-3.4.1/guidata/tests/dataset/test_activable_dataset.py
--rw-rw-rw-   0        0        0     1105 2024-01-26 15:37:54.000000 guidata-3.4.1/guidata/tests/dataset/test_activable_items.py
--rw-rw-rw-   0        0        0     4800 2024-03-08 08:29:40.000000 guidata-3.4.1/guidata/tests/dataset/test_all_features.py
--rw-rw-rw-   0        0        0     3882 2024-03-07 07:56:37.000000 guidata-3.4.1/guidata/tests/dataset/test_all_items.py
--rw-rw-rw-   0        0        0     1084 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/tests/dataset/test_all_items_readonly.py
--rw-rw-rw-   0        0        0     1824 2023-10-13 14:55:43.000000 guidata-3.4.1/guidata/tests/dataset/test_bool_selector.py
--rw-rw-rw-   0        0        0     2639 2023-10-13 14:56:43.000000 guidata-3.4.1/guidata/tests/dataset/test_callbacks.py
--rw-rw-rw-   0        0        0     1251 2024-03-07 08:04:32.000000 guidata-3.4.1/guidata/tests/dataset/test_datasetgroup.py
--rw-rw-rw-   0        0        0     6881 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/tests/dataset/test_editgroupbox.py
--rw-rw-rw-   0        0        0     1460 2023-10-13 13:33:58.000000 guidata-3.4.1/guidata/tests/dataset/test_inheritance.py
--rw-rw-rw-   0        0        0     1270 2023-10-13 13:33:58.000000 guidata-3.4.1/guidata/tests/dataset/test_item_order.py
--rw-rw-rw-   0        0        0     1145 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/tests/dataset/test_loadsave_hdf5.py
--rw-rw-rw-   0        0        0     1073 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/tests/dataset/test_loadsave_json.py
--rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.4.1/guidata/tests/dataset/test_rotatedlabel.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.044598 guidata-3.4.1/guidata/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-10-23 07:02:29.000000 guidata-3.4.1/guidata/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     1076 2023-10-23 07:13:17.000000 guidata-3.4.1/guidata/tests/unit/test_config.py
--rw-rw-rw-   0        0        0     1362 2023-10-13 14:57:07.000000 guidata-3.4.1/guidata/tests/unit/test_data.py
--rw-rw-rw-   0        0        0     1054 2023-10-27 13:44:13.000000 guidata-3.4.1/guidata/tests/unit/test_dataset_from_dict.py
--rw-rw-rw-   0        0        0     1451 2023-10-13 07:06:54.000000 guidata-3.4.1/guidata/tests/unit/test_dataset_from_func.py
--rw-rw-rw-   0        0        0      917 2024-03-12 12:49:04.000000 guidata-3.4.1/guidata/tests/unit/test_genreqs.py
--rw-rw-rw-   0        0        0     6538 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/tests/unit/test_h5fmt.py
--rw-rw-rw-   0        0        0     4405 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/tests/unit/test_jsonfmt.py
--rw-rw-rw-   0        0        0      716 2023-10-23 07:01:03.000000 guidata-3.4.1/guidata/tests/unit/test_no_qt.py
--rw-rw-rw-   0        0        0      766 2023-10-13 14:58:03.000000 guidata-3.4.1/guidata/tests/unit/test_text.py
--rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.4.1/guidata/tests/unit/test_translations.py
--rw-rw-rw-   0        0        0     2076 2023-10-23 07:13:22.000000 guidata-3.4.1/guidata/tests/unit/test_updaterestoredataset.py
--rw-rw-rw-   0        0        0      717 2023-10-13 13:35:43.000000 guidata-3.4.1/guidata/tests/unit/test_userconfig_app.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.044598 guidata-3.4.1/guidata/tests/widgets/
--rw-rw-rw-   0        0        0        0 2023-10-23 07:06:39.000000 guidata-3.4.1/guidata/tests/widgets/__init__.py
--rw-rw-rw-   0        0        0     3099 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/tests/widgets/test_arrayeditor.py
--rw-rw-rw-   0        0        0     7116 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/tests/widgets/test_arrayeditor_unit.py
--rw-rw-rw-   0        0        0      795 2023-10-23 07:25:27.000000 guidata-3.4.1/guidata/tests/widgets/test_codeeditor.py
--rw-rw-rw-   0        0        0     3955 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/tests/widgets/test_collectionseditor.py
--rw-rw-rw-   0        0        0      737 2023-10-25 09:45:17.000000 guidata-3.4.1/guidata/tests/widgets/test_console.py
--rw-rw-rw-   0        0        0     2104 2023-07-18 14:56:56.000000 guidata-3.4.1/guidata/tests/widgets/test_dataframeeditor.py
--rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.4.1/guidata/tests/widgets/test_importwizard.py
--rw-rw-rw-   0        0        0     1578 2023-07-18 15:02:08.000000 guidata-3.4.1/guidata/tests/widgets/test_objecteditor.py
--rw-rw-rw-   0        0        0    15206 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/userconfig.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.061349 guidata-3.4.1/guidata/utils/
--rw-rw-rw-   0        0        0       25 2023-10-13 14:50:52.000000 guidata-3.4.1/guidata/utils/__init__.py
--rw-rw-rw-   0        0        0     5535 2023-09-28 10:28:04.000000 guidata-3.4.1/guidata/utils/encoding.py
--rw-rw-rw-   0        0        0     6645 2023-08-31 06:36:26.000000 guidata-3.4.1/guidata/utils/genreqs.py
--rw-rw-rw-   0        0        0     4025 2023-10-05 12:59:50.000000 guidata-3.4.1/guidata/utils/gettext_helpers.py
--rw-rw-rw-   0        0        0    11885 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/utils/misc.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.061349 guidata-3.4.1/guidata/widgets/
--rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.4.1/guidata/widgets/__init__.py
--rw-rw-rw-   0        0        0     4895 2023-10-25 11:49:16.000000 guidata-3.4.1/guidata/widgets/about.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.075854 guidata-3.4.1/guidata/widgets/arrayeditor/
--rw-rw-rw-   0        0        0      578 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/widgets/arrayeditor/__init__.py
--rw-rw-rw-   0        0        0    17492 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/widgets/arrayeditor/arrayeditor.py
--rw-rw-rw-   0        0        0    17283 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/widgets/arrayeditor/arrayhandler.py
--rw-rw-rw-   0        0        0    35219 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/widgets/arrayeditor/datamodel.py
--rw-rw-rw-   0        0        0    35120 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/widgets/arrayeditor/editorwidget.py
--rw-rw-rw-   0        0        0     2668 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/widgets/arrayeditor/utils.py
--rw-rw-rw-   0        0        0    16488 2024-03-12 12:43:19.000000 guidata-3.4.1/guidata/widgets/codeeditor.py
--rw-rw-rw-   0        0        0    55358 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/widgets/collectionseditor.py
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.075854 guidata-3.4.1/guidata/widgets/console/
--rw-rw-rw-   0        0        0     3337 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/widgets/console/__init__.py
--rw-rw-rw-   0        0        0    59030 2023-10-25 09:22:34.000000 guidata-3.4.1/guidata/widgets/console/base.py
--rw-rw-rw-   0        0        0    12498 2023-10-25 09:44:46.000000 guidata-3.4.1/guidata/widgets/console/calltip.py
--rw-rw-rw-   0        0        0    11610 2023-10-25 09:36:22.000000 guidata-3.4.1/guidata/widgets/console/dochelpers.py
--rw-rw-rw-   0        0        0    15710 2023-10-25 08:55:40.000000 guidata-3.4.1/guidata/widgets/console/internalshell.py
--rw-rw-rw-   0        0        0    12586 2023-09-28 09:29:36.000000 guidata-3.4.1/guidata/widgets/console/interpreter.py
--rw-rw-rw-   0        0        0    30961 2023-10-25 09:41:48.000000 guidata-3.4.1/guidata/widgets/console/mixins.py
--rw-rw-rw-   0        0        0    33812 2024-03-06 10:46:03.000000 guidata-3.4.1/guidata/widgets/console/shell.py
--rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/widgets/console/terminal.py
--rw-rw-rw-   0        0        0    32555 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/widgets/dataframeeditor.py
--rw-rw-rw-   0        0        0     3654 2023-09-28 09:24:59.000000 guidata-3.4.1/guidata/widgets/dockable.py
--rw-rw-rw-   0        0        0    24121 2023-10-24 14:09:48.000000 guidata-3.4.1/guidata/widgets/importwizard.py
--rw-rw-rw-   0        0        0    23425 2023-10-12 13:26:00.000000 guidata-3.4.1/guidata/widgets/nsview.py
--rw-rw-rw-   0        0        0     3571 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/widgets/objecteditor.py
--rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.4.1/guidata/widgets/rotatedlabel.py
--rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.4.1/guidata/widgets/syntaxhighlighters.py
--rw-rw-rw-   0        0        0     4014 2024-03-07 13:48:08.000000 guidata-3.4.1/guidata/widgets/texteditor.py
--rw-rw-rw-   0        0        0      280 2023-07-28 09:44:33.000000 guidata-3.4.1/guidata-tests.desktop
-drwxrwxrwx   0        0        0        0 2024-03-12 13:00:34.075854 guidata-3.4.1/guidata.egg-info/
--rw-rw-rw-   0        0        0     6433 2024-03-12 13:00:33.000000 guidata-3.4.1/guidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6941 2024-03-12 13:00:33.000000 guidata-3.4.1/guidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 13:00:33.000000 guidata-3.4.1/guidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-12 13:00:33.000000 guidata-3.4.1/guidata.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      217 2024-03-12 13:00:33.000000 guidata-3.4.1/guidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-12 13:00:33.000000 guidata-3.4.1/guidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2030 2024-03-11 07:41:58.000000 guidata-3.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 13:00:34.091486 guidata-3.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:22.005805 guidata-3.5.0/
+-rw-rw-rw-   0        0        0    33701 2024-04-10 16:45:12.000000 guidata-3.5.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1563 2024-04-10 16:45:12.000000 guidata-3.5.0/LICENSE
+-rw-rw-rw-   0        0        0       97 2024-04-10 16:45:12.000000 guidata-3.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6806 2024-04-10 16:45:22.004805 guidata-3.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2635 2024-04-10 16:45:12.000000 guidata-3.5.0/README.md
+-rw-rw-rw-   0        0        0      189 2024-04-10 16:45:12.000000 guidata-3.5.0/conftest.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.749570 guidata-3.5.0/doc/
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.750570 guidata-3.5.0/doc/_static/
+-rw-rw-rw-   0        0        0    97375 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/_static/favicon.ico
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.752853 guidata-3.5.0/doc/autodoc/
+-rw-rw-rw-   0        0        0     3346 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/autodoc/autodoc_example.py
+-rw-rw-rw-   0        0        0     2746 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/autodoc/index.rst
+-rw-rw-rw-   0        0        0      689 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/basic_example.py
+-rw-rw-rw-   0        0        0       63 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/changelog.rst
+-rw-rw-rw-   0        0        0     1628 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.759856 guidata-3.5.0/doc/dev/
+-rw-rw-rw-   0        0        0     4051 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/dev/contribute.rst
+-rw-rw-rw-   0        0        0      905 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/dev/howto.rst
+-rw-rw-rw-   0        0        0      136 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/dev/index.rst
+-rw-rw-rw-   0        0        0     4014 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/dev/platform.rst
+-rw-rw-rw-   0        0        0     2305 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/dev/v2_to_v3.csv
+-rw-rw-rw-   0        0        0     1186 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/dev/v2_to_v3.rst
+-rw-rw-rw-   0        0        0     2733 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/examples.rst
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.764634 guidata-3.5.0/doc/images/
+-rw-rw-rw-   0        0        0     4744 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/basic_example.png
+-rw-rw-rw-   0        0        0    19715 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/guidata-banner.png
+-rw-rw-rw-   0        0        0     6669 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/guidata-vertical.png
+-rw-rw-rw-   0        0        0    14799 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/layout_example.png
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.780015 guidata-3.5.0/doc/images/screenshots/
+-rw-rw-rw-   0        0        0    84779 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/__init__.png
+-rw-rw-rw-   0        0        0     4672 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/activable_dataset.png
+-rw-rw-rw-   0        0        0    33244 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/all_features.png
+-rw-rw-rw-   0        0        0    38960 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/all_items.png
+-rw-rw-rw-   0        0        0    23930 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/arrayeditor.png
+-rw-rw-rw-   0        0        0     7935 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/bool_selector.png
+-rw-rw-rw-   0        0        0    43676 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/codeeditor.png
+-rw-rw-rw-   0        0        0    25840 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/collectioneditor.png
+-rw-rw-rw-   0        0        0    14535 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/console.png
+-rw-rw-rw-   0        0        0    16805 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/dataframeeditor.png
+-rw-rw-rw-   0        0        0    33475 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/datasetgroup.png
+-rw-rw-rw-   0        0        0    25030 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/editgroupbox.png
+-rw-rw-rw-   0        0        0    15365 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/images/screenshots/importwizard.png
+-rw-rw-rw-   0        0        0     1232 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/index.rst
+-rw-rw-rw-   0        0        0      540 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/installation.rst
+-rw-rw-rw-   0        0        0     2371 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/overview.rst
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.786529 guidata-3.5.0/doc/reference/
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.791530 guidata-3.5.0/doc/reference/dataset/
+-rw-rw-rw-   0        0        0       54 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/dataset/conv.rst
+-rw-rw-rw-   0        0        0       59 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/dataset/dataitems.rst
+-rw-rw-rw-   0        0        0       59 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/dataset/datatypes.rst
+-rw-rw-rw-   0        0        0      153 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/dataset/index.rst
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/dataset/io.rst
+-rw-rw-rw-   0        0        0       59 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/dataset/qtwidgets.rst
+-rw-rw-rw-   0        0        0       49 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/guitest.rst
+-rw-rw-rw-   0        0        0      148 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/index.rst
+-rw-rw-rw-   0        0        0       50 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/userconfig.rst
+-rw-rw-rw-   0        0        0      146 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/utils.rst
+-rw-rw-rw-   0        0        0      136 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/reference/widgets.rst
+-rw-rw-rw-   0        0        0     2387 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/requirements.rst
+-rw-rw-rw-   0        0        0      721 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/update_requirements.py
+-rw-rw-rw-   0        0        0     1699 2024-04-10 16:45:12.000000 guidata-3.5.0/doc/widgets.rst
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.798531 guidata-3.5.0/guidata/
+-rw-rw-rw-   0        0        0     3047 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/__init__.py
+-rw-rw-rw-   0        0        0    11296 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/config.py
+-rw-rw-rw-   0        0        0    13841 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/configtools.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.821430 guidata-3.5.0/guidata/dataset/
+-rw-rw-rw-   0        0        0     1059 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/__init__.py
+-rw-rw-rw-   0        0        0    20008 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/autodoc.py
+-rw-rw-rw-   0        0        0     2620 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/autodoc_method.py
+-rw-rw-rw-   0        0        0     6974 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/conv.py
+-rw-rw-rw-   0        0        0    35890 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/dataitems.py
+-rw-rw-rw-   0        0        0    48314 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/datatypes.py
+-rw-rw-rw-   0        0        0      557 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/io.py
+-rw-rw-rw-   0        0        0     3217 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/note_directive.py
+-rw-rw-rw-   0        0        0    50823 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/qtitemwidgets.py
+-rw-rw-rw-   0        0        0    35733 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/qtwidgets.py
+-rw-rw-rw-   0        0        0      820 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/dataset/textedit.py
+-rw-rw-rw-   0        0        0     9603 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/env.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.822431 guidata-3.5.0/guidata/external/
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/external/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.832455 guidata-3.5.0/guidata/external/darkdetect/
+-rw-rw-rw-   0        0        0     1289 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/external/darkdetect/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/external/darkdetect/_dummy.py
+-rw-rw-rw-   0        0        0      890 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/external/darkdetect/_linux_detect.py
+-rw-rw-rw-   0        0        0     2212 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/external/darkdetect/_mac_detect.py
+-rw-rw-rw-   0        0        0     1257 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/external/darkdetect/_windows_detect.py
+-rw-rw-rw-   0        0        0    11402 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/guitest.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.869623 guidata-3.5.0/guidata/images/
+-rw-rw-rw-   0        0        0      785 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/apply.png
+-rw-rw-rw-   0        0        0     1123 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/arredit.png
+-rw-rw-rw-   0        0        0      721 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/busy.png
+-rw-rw-rw-   0        0        0      689 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/cell_edit.png
+-rw-rw-rw-   0        0        0      830 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/copy.png
+-rw-rw-rw-   0        0        0      722 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/delete.png
+-rw-rw-rw-   0        0        0      911 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/dictedit.png
+-rw-rw-rw-   0        0        0      735 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/dtype.png
+-rw-rw-rw-   0        0        0      929 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/edit.png
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.886706 guidata-3.5.0/guidata/images/editors/
+-rw-rw-rw-   0        0        0      911 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/copywop.png
+-rw-rw-rw-   0        0        0      929 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/edit.png
+-rw-rw-rw-   0        0        0     1001 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/edit_add.png
+-rw-rw-rw-   0        0        0     1777 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/editclear.png
+-rw-rw-rw-   0        0        0     1048 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/editcopy.png
+-rw-rw-rw-   0        0        0      824 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/editcut.png
+-rw-rw-rw-   0        0        0     1453 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/editdelete.png
+-rw-rw-rw-   0        0        0     1295 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/editpaste.png
+-rw-rw-rw-   0        0        0     2248 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/fileimport.png
+-rw-rw-rw-   0        0        0     1144 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/filesave.png
+-rw-rw-rw-   0        0        0      727 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/imshow.png
+-rw-rw-rw-   0        0        0      525 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/insert.png
+-rw-rw-rw-   0        0        0      515 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/plot.png
+-rw-rw-rw-   0        0        0      689 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/rename.png
+-rw-rw-rw-   0        0        0     1184 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/editors/selectall.png
+-rw-rw-rw-   0        0        0     1164 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/exit.png
+-rw-rw-rw-   0        0        0      165 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/expander_down.png
+-rw-rw-rw-   0        0        0      432 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/expander_right.png
+-rw-rw-rw-   0        0        0      530 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/file.png
+-rw-rw-rw-   0        0        0     1424 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/fileclose.png
+-rw-rw-rw-   0        0        0     1556 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/fileimport.png
+-rw-rw-rw-   0        0        0      463 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filenew.png
+-rw-rw-rw-   0        0        0     1539 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/fileopen.png
+-rw-rw-rw-   0        0        0     1144 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filesave.png
+-rw-rw-rw-   0        0        0     1443 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filesaveas.png
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.902370 guidata-3.5.0/guidata/images/filetypes/
+-rw-rw-rw-   0        0        0     1601 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/doc.png
+-rw-rw-rw-   0        0        0     1512 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/gif.png
+-rw-rw-rw-   0        0        0     1848 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/html.png
+-rw-rw-rw-   0        0        0     1512 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/jpg.png
+-rw-rw-rw-   0        0        0     1543 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/pdf.png
+-rw-rw-rw-   0        0        0     1512 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/png.png
+-rw-rw-rw-   0        0        0     1439 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/pps.png
+-rw-rw-rw-   0        0        0     1428 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/ps.png
+-rw-rw-rw-   0        0        0     1577 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/tar.png
+-rw-rw-rw-   0        0        0     1577 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/tgz.png
+-rw-rw-rw-   0        0        0     1512 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/tif.png
+-rw-rw-rw-   0        0        0     1801 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/txt.png
+-rw-rw-rw-   0        0        0     1237 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/xls.png
+-rw-rw-rw-   0        0        0     1577 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/filetypes/zip.png
+-rw-rw-rw-   0        0        0    17125 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/guidata-banner.svg
+-rw-rw-rw-   0        0        0    17097 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/guidata-vertical.svg
+-rw-rw-rw-   0        0        0    16435 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/guidata.svg
+-rw-rw-rw-   0        0        0      356 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/max.png
+-rw-rw-rw-   0        0        0      351 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/min.png
+-rw-rw-rw-   0        0        0      331 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/none.png
+-rw-rw-rw-   0        0        0      531 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/not_found.png
+-rw-rw-rw-   0        0        0      887 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/python.png
+-rw-rw-rw-   0        0        0      888 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/quickview.png
+-rw-rw-rw-   0        0        0     1599 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/save_all.png
+-rw-rw-rw-   0        0        0      744 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/selection.png
+-rw-rw-rw-   0        0        0     2445 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/settings.png
+-rw-rw-rw-   0        0        0      361 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/shape.png
+-rw-rw-rw-   0        0        0      354 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/xmax.png
+-rw-rw-rw-   0        0        0      353 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/images/xmin.png
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.907370 guidata-3.5.0/guidata/io/
+-rw-rw-rw-   0        0        0     1738 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/io/__init__.py
+-rw-rw-rw-   0        0        0     5905 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/io/base.py
+-rw-rw-rw-   0        0        0    27914 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/io/h5fmt.py
+-rw-rw-rw-   0        0        0     4523 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/io/inifmt.py
+-rw-rw-rw-   0        0        0    10386 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/io/jsonfmt.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.717518 guidata-3.5.0/guidata/locale/
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.717518 guidata-3.5.0/guidata/locale/fr/
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.908370 guidata-3.5.0/guidata/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    14175 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/locale/fr/LC_MESSAGES/guidata.mo
+-rw-rw-rw-   0        0        0    20041 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/qthelpers.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.909371 guidata-3.5.0/guidata/tests/
+-rw-rw-rw-   0        0        0      653 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.719346 guidata-3.5.0/guidata/tests/data/
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.912409 guidata-3.5.0/guidata/tests/data/genreqs/
+-rw-rw-rw-   0        0        0     1908 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/data/genreqs/pyproject.toml
+-rw-rw-rw-   0        0        0     1463 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/data/genreqs/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.932095 guidata-3.5.0/guidata/tests/dataset/
+-rw-rw-rw-   0        0        0        0 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/__init__.py
+-rw-rw-rw-   0        0        0     1756 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_activable_dataset.py
+-rw-rw-rw-   0        0        0     1105 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_activable_items.py
+-rw-rw-rw-   0        0        0     4800 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_all_features.py
+-rw-rw-rw-   0        0        0     3882 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_all_items.py
+-rw-rw-rw-   0        0        0     1084 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_all_items_readonly.py
+-rw-rw-rw-   0        0        0     1824 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_bool_selector.py
+-rw-rw-rw-   0        0        0     2790 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_callbacks.py
+-rw-rw-rw-   0        0        0     1251 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_datasetgroup.py
+-rw-rw-rw-   0        0        0     6881 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_editgroupbox.py
+-rw-rw-rw-   0        0        0     1460 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_inheritance.py
+-rw-rw-rw-   0        0        0     1270 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_item_order.py
+-rw-rw-rw-   0        0        0     1145 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_loadsave_hdf5.py
+-rw-rw-rw-   0        0        0     1073 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_loadsave_json.py
+-rw-rw-rw-   0        0        0     1361 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/dataset/test_rotatedlabel.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.947783 guidata-3.5.0/guidata/tests/unit/
+-rw-rw-rw-   0        0        0        0 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     1076 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_config.py
+-rw-rw-rw-   0        0        0     1362 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_data.py
+-rw-rw-rw-   0        0        0     1054 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_dataset_from_dict.py
+-rw-rw-rw-   0        0        0     1451 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_dataset_from_func.py
+-rw-rw-rw-   0        0        0      917 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_genreqs.py
+-rw-rw-rw-   0        0        0     6530 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_h5fmt.py
+-rw-rw-rw-   0        0        0     4469 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_jsonfmt.py
+-rw-rw-rw-   0        0        0      716 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_no_qt.py
+-rw-rw-rw-   0        0        0      766 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_text.py
+-rw-rw-rw-   0        0        0      493 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_translations.py
+-rw-rw-rw-   0        0        0     2076 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_updaterestoredataset.py
+-rw-rw-rw-   0        0        0      717 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/unit/test_userconfig_app.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.960220 guidata-3.5.0/guidata/tests/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3099 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/widgets/test_arrayeditor.py
+-rw-rw-rw-   0        0        0     7116 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/widgets/test_arrayeditor_unit.py
+-rw-rw-rw-   0        0        0      795 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/widgets/test_codeeditor.py
+-rw-rw-rw-   0        0        0     3955 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/widgets/test_collectionseditor.py
+-rw-rw-rw-   0        0        0      737 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/widgets/test_console.py
+-rw-rw-rw-   0        0        0     2104 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/widgets/test_dataframeeditor.py
+-rw-rw-rw-   0        0        0      779 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/widgets/test_importwizard.py
+-rw-rw-rw-   0        0        0     1578 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/tests/widgets/test_objecteditor.py
+-rw-rw-rw-   0        0        0    15206 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/userconfig.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.966219 guidata-3.5.0/guidata/utils/
+-rw-rw-rw-   0        0        0       25 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/utils/__init__.py
+-rw-rw-rw-   0        0        0     5535 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/utils/encoding.py
+-rw-rw-rw-   0        0        0     6722 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/utils/genreqs.py
+-rw-rw-rw-   0        0        0     4025 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/utils/gettext_helpers.py
+-rw-rw-rw-   0        0        0    11885 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/utils/misc.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.982633 guidata-3.5.0/guidata/widgets/
+-rw-rw-rw-   0        0        0      729 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4895 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/about.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:21.990939 guidata-3.5.0/guidata/widgets/arrayeditor/
+-rw-rw-rw-   0        0        0      578 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/arrayeditor/__init__.py
+-rw-rw-rw-   0        0        0    17492 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/arrayeditor/arrayeditor.py
+-rw-rw-rw-   0        0        0    17283 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/arrayeditor/arrayhandler.py
+-rw-rw-rw-   0        0        0    35219 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/arrayeditor/datamodel.py
+-rw-rw-rw-   0        0        0    35120 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/arrayeditor/editorwidget.py
+-rw-rw-rw-   0        0        0     2668 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/arrayeditor/utils.py
+-rw-rw-rw-   0        0        0    16488 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/codeeditor.py
+-rw-rw-rw-   0        0        0    55358 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/collectionseditor.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:22.002804 guidata-3.5.0/guidata/widgets/console/
+-rw-rw-rw-   0        0        0     3337 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/console/__init__.py
+-rw-rw-rw-   0        0        0    59030 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/console/base.py
+-rw-rw-rw-   0        0        0    12498 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/console/calltip.py
+-rw-rw-rw-   0        0        0    11610 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/console/dochelpers.py
+-rw-rw-rw-   0        0        0    15710 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/console/internalshell.py
+-rw-rw-rw-   0        0        0    12586 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/console/interpreter.py
+-rw-rw-rw-   0        0        0    30961 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/console/mixins.py
+-rw-rw-rw-   0        0        0    33812 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/console/shell.py
+-rw-rw-rw-   0        0        0     4099 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/console/terminal.py
+-rw-rw-rw-   0        0        0    32555 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/dataframeeditor.py
+-rw-rw-rw-   0        0        0     3654 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/dockable.py
+-rw-rw-rw-   0        0        0    24121 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/importwizard.py
+-rw-rw-rw-   0        0        0    23425 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/nsview.py
+-rw-rw-rw-   0        0        0     3571 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/objecteditor.py
+-rw-rw-rw-   0        0        0     2122 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/rotatedlabel.py
+-rw-rw-rw-   0        0        0    62527 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/syntaxhighlighters.py
+-rw-rw-rw-   0        0        0     4014 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata/widgets/texteditor.py
+-rw-rw-rw-   0        0        0      290 2024-04-10 16:45:12.000000 guidata-3.5.0/guidata-tests.desktop
+drwxrwxrwx   0        0        0        0 2024-04-10 16:45:22.003804 guidata-3.5.0/guidata.egg-info/
+-rw-rw-rw-   0        0        0     6806 2024-04-10 16:45:21.000000 guidata-3.5.0/guidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7105 2024-04-10 16:45:21.000000 guidata-3.5.0/guidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:45:21.000000 guidata-3.5.0/guidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-10 16:45:21.000000 guidata-3.5.0/guidata.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      210 2024-04-10 16:45:21.000000 guidata-3.5.0/guidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 16:45:21.000000 guidata-3.5.0/guidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3288 2024-04-10 16:45:12.000000 guidata-3.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      202 2024-04-10 16:45:12.000000 guidata-3.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:45:22.005805 guidata-3.5.0/setup.cfg
```

### Comparing `guidata-3.4.1/LICENSE` & `guidata-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/PKG-INFO` & `guidata-3.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guidata
-Version: 3.4.1
+Version: 3.5.0
 Summary: Automatic GUI generation for easy dataset editing and display
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
         
@@ -31,41 +31,46 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/PlotPyStack/guidata/
 Project-URL: Documentation, https://guidata.readthedocs.io/en/latest/
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Software Development :: User Interfaces
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows 7
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Software Development :: Widget Sets
+Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py>=3.0
 Requires-Dist: NumPy>=1.21
 Requires-Dist: QtPy>=1.9
 Requires-Dist: requests
 Requires-Dist: tomli
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: Coverage; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: PyQt5; extra == "doc"
 Requires-Dist: pillow; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
 Requires-Dist: sphinx>6; extra == "doc"
```

### Comparing `guidata-3.4.1/README.md` & `guidata-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/_static/favicon.ico` & `guidata-3.5.0/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/basic_example.py` & `guidata-3.5.0/doc/basic_example.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/conf.py` & `guidata-3.5.0/doc/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(".."))
+sys.path.insert(0, os.path.abspath("autodoc"))
 
 import guidata  # noqa: E402
 
 creator = "Pierre Raybaut"
 project = "guidata"
 copyright = "2009 CEA, " + creator
 version = ".".join(guidata.__version__.split(".")[:2])
@@ -17,14 +18,15 @@
     "sphinx.ext.autodoc",
     "myst_parser",
     "sphinx.ext.intersphinx",
     "sphinx.ext.doctest",
     "sphinx_copybutton",
     "sphinx.ext.napoleon",
     "sphinx_qt_documentation",
+    "guidata.dataset.autodoc",
 ]
 if "htmlhelp" in sys.argv:
     extensions += ["sphinx.ext.imgmath"]
 else:
     extensions += ["sphinx.ext.mathjax"]
 templates_path = ["_templates"]
 source_suffix = ".rst"
```

### Comparing `guidata-3.4.1/doc/dev/contribute.rst` & `guidata-3.5.0/doc/dev/contribute.rst`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
         pylint --disable=fixme,C,R,W guidata
 
 * Run the tests and check that they all pass:
 
     .. code-block:: bash
 
-        pytest guidata
+        pytest
 
 Pull request
 ~~~~~~~~~~~~
 
 If you want to contribute to the project, you can submit a patch. The
 recommended way to do this is to fork the project on GitHub, create a branch
 for your modifications and then send a pull request. The pull request will be
```

### Comparing `guidata-3.4.1/doc/dev/howto.rst` & `guidata-3.5.0/doc/dev/howto.rst`

 * *Files 17% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 
 * Python
 * pytest
 * coverage (optional)
 
 Then run the following command::
 
-    pytest guidata
+    pytest
 
 To run test with coverage support, use the following command::
 
     pytest -v --cov --cov-report=html guidata
 
 
 Code formatting
 ^^^^^^^^^^^^^^^
 
-The code is formatted with `black <https://black.readthedocs.io/en/stable/>`_
-and `isort <https://isort.readthedocs.io/en/stable/>`_.
+The code is formatted with `ruff <https://pypi.org/project/ruff/>`_.
 
 If you are using `Visual Studio Code <https://code.visualstudio.com/>`_,
 the formatting is done automatically when you save a file, thanks to the
 project settings in the `.vscode` directory.
```

### Comparing `guidata-3.4.1/doc/dev/platform.rst` & `guidata-3.5.0/doc/dev/platform.rst`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     pip install -r requirements.txt
 
 That's it, you can now run the tests using the following command:
 
 .. code-block:: bash
 
-    pytest guidata
+    pytest
 
 If you want to rely on Visual Studio Code for editing and take advantage of the
 project settings and tasks, you will need to set the following environment variable:
 
 .. code-block:: bash
 
     set PPSTACK_PYTHONEXE=C:\WPy64-31110\python-3.11.1.amd64\python.exe
@@ -123,8 +123,8 @@
     pip install --upgrade pip
     pip install -r requirements.txt
 
 That's it, you can now run the tests using the following command:
 
 .. code-block:: bash
 
-    pytest guidata
+    pytest
```

### Comparing `guidata-3.4.1/doc/dev/v2_to_v3.csv` & `guidata-3.5.0/doc/dev/v2_to_v3.csv`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/dev/v2_to_v3.rst` & `guidata-3.5.0/doc/dev/v2_to_v3.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/examples.rst` & `guidata-3.5.0/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/basic_example.png` & `guidata-3.5.0/doc/images/basic_example.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/guidata-banner.png` & `guidata-3.5.0/doc/images/guidata-banner.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/guidata-vertical.png` & `guidata-3.5.0/doc/images/guidata-vertical.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/layout_example.png` & `guidata-3.5.0/doc/images/layout_example.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/__init__.png` & `guidata-3.5.0/doc/images/screenshots/__init__.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/activable_dataset.png` & `guidata-3.5.0/doc/images/screenshots/activable_dataset.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/all_features.png` & `guidata-3.5.0/doc/images/screenshots/all_features.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/all_items.png` & `guidata-3.5.0/doc/images/screenshots/all_items.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/arrayeditor.png` & `guidata-3.5.0/doc/images/screenshots/arrayeditor.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/bool_selector.png` & `guidata-3.5.0/doc/images/screenshots/bool_selector.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/codeeditor.png` & `guidata-3.5.0/doc/images/screenshots/codeeditor.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/collectioneditor.png` & `guidata-3.5.0/doc/images/screenshots/collectioneditor.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/console.png` & `guidata-3.5.0/doc/images/screenshots/console.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/dataframeeditor.png` & `guidata-3.5.0/doc/images/screenshots/dataframeeditor.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/datasetgroup.png` & `guidata-3.5.0/doc/images/screenshots/datasetgroup.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/editgroupbox.png` & `guidata-3.5.0/doc/images/screenshots/editgroupbox.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/images/screenshots/importwizard.png` & `guidata-3.5.0/doc/images/screenshots/importwizard.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/index.rst` & `guidata-3.5.0/doc/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -35,12 +35,13 @@
 .. toctree::
    :maxdepth: 2
 
    overview
    installation
    examples
    widgets
+   autodoc/index
    dev/index
    reference/index
    changelog
 
 * :ref:`genindex`
```

### Comparing `guidata-3.4.1/doc/installation.rst` & `guidata-3.5.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/overview.rst` & `guidata-3.5.0/doc/overview.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/requirements.rst` & `guidata-3.5.0/doc/requirements.rst`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     :align: left
 
     * - Name
       - Version
       - Summary
     * - Python
       - >=3.8, <4
-      - 
+      - Python programming language
     * - h5py
       - >=3.0
       - Read and write HDF5 files from Python
     * - NumPy
       - >=1.21
       - Fundamental package for array computing in Python
     * - QtPy
@@ -34,20 +34,17 @@
 .. list-table::
     :header-rows: 1
     :align: left
 
     * - Name
       - Version
       - Summary
-    * - black
-      - 
-      - The uncompromising code formatter.
-    * - isort
+    * - ruff
       - 
-      - A Python utility / library to sort Python imports.
+      - An extremely fast Python linter and code formatter, written in Rust.
     * - pylint
       - 
       - python code static checker
     * - Coverage
       - 
       - Code coverage measurement for Python
```

### Comparing `guidata-3.4.1/doc/update_requirements.py` & `guidata-3.5.0/doc/update_requirements.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/doc/widgets.rst` & `guidata-3.5.0/doc/widgets.rst`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/__init__.py` & `guidata-3.5.0/guidata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 =======
 
 Based on the Qt library :mod:`guidata` is a Python library generating graphical
 user interfaces for easy dataset editing and display. It also provides helpers
 and application development tools for Qt.
 """
 
-__version__ = "3.4.1"
+__version__ = "3.5.0"
 
 
 # Dear (Debian, RPM, ...) package makers, please feel free to customize the
 # following path to module's data (images) and translations:
 DATAPATH = LOCALEPATH = ""
```

### Comparing `guidata-3.4.1/guidata/config.py` & `guidata-3.5.0/guidata/config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/configtools.py` & `guidata-3.5.0/guidata/configtools.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/dataset/__init__.py` & `guidata-3.5.0/guidata/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/dataset/conv.py` & `guidata-3.5.0/guidata/dataset/conv.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/dataset/dataitems.py` & `guidata-3.5.0/guidata/dataset/dataitems.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,31 +92,35 @@
 
 from __future__ import annotations
 
 import datetime
 import os
 import re
 from collections.abc import Callable
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Generic, Iterable, Type, TypeVar, Union
+
+import numpy as np
 
 from guidata.config import _
 from guidata.dataset.datatypes import DataItem, DataSet, ItemProperty
 
 if TYPE_CHECKING:
-    from numpy import ndarray
+    from numpy.typing import NDArray
 
     from guidata.io import (
         HDF5Reader,
         HDF5Writer,
         INIReader,
         INIWriter,
         JSONReader,
         JSONWriter,
     )
 
+_T = TypeVar("_T")
+
 
 class NumericTypeItem(DataItem):
     """Numeric data item
 
     Args:
         label: item name
         default: default value (optional)
@@ -502,15 +506,25 @@
         label: item label
         default: default value (optional)
         format: date format (as in :py:func:`datetime.date.strftime`)
         help: text displayed on data item's tooltip
         check: check value (default: True)
     """
 
-    pass
+    type = datetime.datetime
+
+    def __init__(
+        self,
+        label: str,
+        default: datetime.datetime | None = None,
+        format: str | None = None,
+        help: str | None = "",
+        check: bool | None = True,
+    ) -> None:
+        super().__init__(label, default, format, help, check)
 
 
 class ColorItem(StringItem):
     """Construct a color data item
 
     Args:
         label: item name
@@ -736,15 +750,15 @@
     Special object that means the default value of a ChoiceItem
     is the first item.
     """
 
     pass
 
 
-class ChoiceItem(DataItem):
+class ChoiceItem(DataItem, Generic[_T]):
     """Construct a data item for a list of choices.
 
     Args:
         label: item name
         choices: string list or (key, label) list
          function of two arguments (item, value) returning a list of tuples
          (key, label, image) where image is an icon path, a QIcon instance
@@ -753,19 +767,21 @@
         help: text shown in tooltip (optional)
         check: if False, value is not checked (optional, default=True)
         radio: if True, shows radio buttons instead of a combo box
          (default is False)
         size: size (optional) of the combo box or button widget (for radio buttons)
     """
 
+    type = Any
+
     def __init__(
         self,
         label: str,
-        choices: Any,
-        default: tuple[()] | type[FirstChoice] | int | None = FirstChoice,
+        choices: Iterable[_T] | Callable[[Any], Iterable[_T]],
+        default: tuple[()] | type[FirstChoice] | int | _T | None = FirstChoice,
         help: str = "",
         check: bool = True,
         radio: bool = False,
         size: tuple[int, int] | None = None,
     ) -> None:
         _choices_data: Any
         if isinstance(choices, Callable):
@@ -822,25 +838,25 @@
         default: tuple[()] = (),
         help: str = "",
         check: bool = True,
     ) -> None:
         super().__init__(label, choices, default, help, check=check)
         self.set_prop("display", shape=(1, -1))
 
-    def horizontal(self, row_nb: int = 1) -> "MultipleChoiceItem":
+    def horizontal(self, row_nb: int = 1) -> MultipleChoiceItem:
         """
         Method to arange choice list horizontally on `n` rows
 
         Example:
         nb = MultipleChoiceItem("Number", ['1', '2', '3'] ).horizontal(2)
         """
         self.set_prop("display", shape=(row_nb, -1))
         return self
 
-    def vertical(self, col_nb: int = 1) -> "MultipleChoiceItem":
+    def vertical(self, col_nb: int = 1) -> MultipleChoiceItem:
         """
         Method to arange choice list vertically on `n` columns
 
         Example:
         nb = MultipleChoiceItem("Number", ['1', '2', '3'] ).vertical(2)
         """
         self.set_prop("display", shape=(-1, col_nb))
@@ -917,18 +933,20 @@
         transpose: transpose matrix (display only)
         large: view all float of the array
         minmax: "all" (default), "columns", "rows"
         check: if False, value is not checked (optional, default=True)
         variable_size: if True, allows to add/remove row/columns on all axis
     """
 
+    type = np.ndarray
+
     def __init__(
         self,
         label: str,
-        default: ndarray | None = None,
+        default: NDArray | None = None,
         help: str = "",
         format: str = "%.3f",
         transpose: bool = False,
         minmax: str = "all",
         check: bool = True,
         variable_size=False,
     ) -> None:
@@ -978,16 +996,18 @@
     Args:
         label: item name
         default: default value (optional)
         help: text shown in tooltip (optional)
         check: if False, value is not checked (optional, default=True)
     """
 
+    type: type[dict[str, Any]] = dict
+
     # pylint: disable=redefined-builtin,abstract-method
-    def __init__(self, label, default=None, help="", check=True):
+    def __init__(self, label, default: dict | None = None, help="", check=True):
         super().__init__(label, default=default, help=help, check=check)
         self.set_prop("display", callback=self.__dictedit)
         self.set_prop("display", icon="dictedit.png")
 
     @staticmethod
     # pylint: disable=unused-argument
     def __dictedit(instance: DataSet, item: DataItem, value: dict, parent):
```

### Comparing `guidata-3.4.1/guidata/dataset/datatypes.py` & `guidata-3.5.0/guidata/dataset/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,21 @@
 """
 
 # pylint: disable-msg=W0622
 # pylint: disable-msg=W0212
 
 from __future__ import annotations
 
+import pprint
 import re
 import sys
 from abc import ABC, abstractmethod
 from collections.abc import Callable
 from copy import deepcopy
-from typing import TYPE_CHECKING, Any, TypeVar
+from typing import TYPE_CHECKING, Any, Generic, TypeVar, Union
 
 from guidata.io import INIReader, INIWriter
 from guidata.userconfig import UserConfig
 
 DEBUG_DESERIALIZE = False
 
 if TYPE_CHECKING:
@@ -255,31 +256,32 @@
     Args:
         label (str): item label
         default (Any): default value
         help (str): text displayed on data item's tooltip
         check (bool): check value (default: True)
     """
 
+    type = type
     count = 0
 
     def __init__(
         self,
         label: str,
         default: Any | None = None,
         help: str | None = "",
         check: bool | None = True,
     ) -> None:
         self._order = DataItem.count
         DataItem.count += 1
         self._name: str | None = None
         self._default = default
         self._help = help
-        self._props: dict[Any, Any] = (
-            {}
-        )  # a dict realm->dict containing realm-specific properties
+        self._props: dict[
+            Any, Any
+        ] = {}  # a dict realm->dict containing realm-specific properties
         self.set_prop("display", col=0, colspan=None, row=None, label=label)
         self.set_prop("data", check_value=check)
 
     def get_prop(self, realm: str, name: str, default: Any = NoDefault) -> Any:
         """Get one property of this item
 
         Args:
@@ -452,14 +454,22 @@
         Args:
             instance (DataSet): instance of the DataSet
             string_value (str): string value
         """
         value = self.from_string(string_value)
         self.__set__(instance, value)
 
+    def get_default(self) -> Any:
+        """Return data item's default value
+
+        Returns:
+            Any: default value
+        """
+        return self._default
+
     def set_default(self, instance: DataSet) -> None:
         """Set data item's value to default
 
         Args:
             instance (DataSet): instance of the DataSet
         """
         self.__set__(instance, self._default)
@@ -989,14 +999,15 @@
             if isinstance(value, DataItem):
                 value.set_name(attrname)
                 if attrname in items:
                     value._order = items[attrname]._order
                 items[attrname] = value
         items_list = list(items.values())
         items_list.sort(key=lambda x: x._order)
+
         dct["_items"] = items_list
         return type.__new__(cls, name, bases, dct)
 
 
 Meta_Py3Compat = DataSetMeta("Meta_Py3Compat", (object,), {})
 
 
@@ -1008,15 +1019,15 @@
 
     Args:
         title (str): title
         comment (str): comment. Text shown on the top of the first data item
         icon (str): icon filename as in image search paths
     """
 
-    _items: list[DataItem]
+    _items: list[DataItem] = []
     __metaclass__ = DataSetMeta  # keep it even with Python 3 (see DataSetMeta)
 
     def __init__(
         self,
         title: str | None = None,
         comment: str | None = None,
         icon: str = "",
@@ -1048,15 +1059,15 @@
         Returns:
             _description_
         """
         result_items = self._items if not copy else deepcopy(self._items)
         return list(filter(lambda s: not s.get_name().startswith("_"), result_items))
 
     @classmethod
-    def create(cls, **kwargs) -> DataSet:
+    def create(cls: type[AnyDataSet], **kwargs) -> AnyDataSet:
         """Create a new instance of the DataSet class
 
         Args:
             kwargs: keyword arguments to set the DataItem values
 
         Returns:
             DataSet instance
```

### Comparing `guidata-3.4.1/guidata/dataset/io.py` & `guidata-3.5.0/guidata/dataset/io.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/dataset/qtitemwidgets.py` & `guidata-3.5.0/guidata/dataset/qtitemwidgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,14 +458,15 @@
         """QLineEdit validator"""
         value = self.item.from_string(self.__get_text())
         if not self.item.check_value(value):
             self.edit.setStyleSheet("background-color:rgb(255, 175, 90);")
         else:
             self.edit.setStyleSheet("")
         self.update(value)
+        _display_callback(self, value)
         self.notify_value_change()
 
     def update(self, value: Any) -> Any:
         pass
 
     def value(self) -> str:
         """Returns the widget's current value
@@ -548,14 +549,15 @@
             widget_column = label_column
             column_span += 1
         else:
             self.place_label(layout, row, label_column)
         layout.addWidget(self.group, row, widget_column, row_span, column_span)
 
     def state_changed(self, state: bool) -> None:
+        _display_callback(self, state)
         self.notify_value_change()
         if self.store:
             self.do_store(state)
 
     def do_store(self, state: bool) -> None:
         self.store.set(self.item.instance, self.item.item, state)
         self.parent_layout.refresh_widgets()
@@ -1014,14 +1016,15 @@
 
     def initialize_widget(self) -> None:
         """Widget initialization depending on the type of the widget (combobox or
         radiobuttons)
         """
         if self.is_radio:
             for button in self._buttons:
+                button.hide()
                 button.toggled.disconnect(self.index_changed)  # type:ignore
                 self.vbox.removeWidget(button)
                 button.deleteLater()
             self._buttons = []
         else:
             self.combobox.blockSignals(True)
             while self.combobox.count():
```

### Comparing `guidata-3.4.1/guidata/dataset/qtwidgets.py` & `guidata-3.5.0/guidata/dataset/qtwidgets.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/dataset/textedit.py` & `guidata-3.5.0/guidata/dataset/textedit.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/env.py` & `guidata-3.5.0/guidata/env.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/external/darkdetect/__init__.py` & `guidata-3.5.0/guidata/external/darkdetect/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/external/darkdetect/_linux_detect.py` & `guidata-3.5.0/guidata/external/darkdetect/_linux_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/external/darkdetect/_mac_detect.py` & `guidata-3.5.0/guidata/external/darkdetect/_mac_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/external/darkdetect/_windows_detect.py` & `guidata-3.5.0/guidata/external/darkdetect/_windows_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/guitest.py` & `guidata-3.5.0/guidata/guitest.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/apply.png` & `guidata-3.5.0/guidata/images/apply.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/arredit.png` & `guidata-3.5.0/guidata/images/arredit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/busy.png` & `guidata-3.5.0/guidata/images/busy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/cell_edit.png` & `guidata-3.5.0/guidata/images/cell_edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/copy.png` & `guidata-3.5.0/guidata/images/copy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/delete.png` & `guidata-3.5.0/guidata/images/delete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/dictedit.png` & `guidata-3.5.0/guidata/images/dictedit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/dtype.png` & `guidata-3.5.0/guidata/images/dtype.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/edit.png` & `guidata-3.5.0/guidata/images/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/copywop.png` & `guidata-3.5.0/guidata/images/editors/copywop.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/edit.png` & `guidata-3.5.0/guidata/images/editors/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/edit_add.png` & `guidata-3.5.0/guidata/images/editors/edit_add.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/editclear.png` & `guidata-3.5.0/guidata/images/editors/editclear.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/editcopy.png` & `guidata-3.5.0/guidata/images/editors/editcopy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/editcut.png` & `guidata-3.5.0/guidata/images/editors/editcut.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/editdelete.png` & `guidata-3.5.0/guidata/images/editors/editdelete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/editpaste.png` & `guidata-3.5.0/guidata/images/editors/editpaste.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/fileimport.png` & `guidata-3.5.0/guidata/images/editors/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/filesave.png` & `guidata-3.5.0/guidata/images/editors/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/imshow.png` & `guidata-3.5.0/guidata/images/editors/imshow.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/insert.png` & `guidata-3.5.0/guidata/images/editors/insert.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/plot.png` & `guidata-3.5.0/guidata/images/editors/plot.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/rename.png` & `guidata-3.5.0/guidata/images/editors/rename.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/editors/selectall.png` & `guidata-3.5.0/guidata/images/editors/selectall.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/exit.png` & `guidata-3.5.0/guidata/images/exit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/file.png` & `guidata-3.5.0/guidata/images/file.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/fileclose.png` & `guidata-3.5.0/guidata/images/fileclose.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/fileimport.png` & `guidata-3.5.0/guidata/images/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/fileopen.png` & `guidata-3.5.0/guidata/images/fileopen.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filesave.png` & `guidata-3.5.0/guidata/images/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filesaveas.png` & `guidata-3.5.0/guidata/images/filesaveas.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/doc.png` & `guidata-3.5.0/guidata/images/filetypes/doc.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/gif.png` & `guidata-3.5.0/guidata/images/filetypes/gif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/html.png` & `guidata-3.5.0/guidata/images/filetypes/html.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/jpg.png` & `guidata-3.5.0/guidata/images/filetypes/jpg.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/pdf.png` & `guidata-3.5.0/guidata/images/filetypes/pdf.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/png.png` & `guidata-3.5.0/guidata/images/filetypes/png.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/pps.png` & `guidata-3.5.0/guidata/images/filetypes/pps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/ps.png` & `guidata-3.5.0/guidata/images/filetypes/ps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/tar.png` & `guidata-3.5.0/guidata/images/filetypes/tar.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/tgz.png` & `guidata-3.5.0/guidata/images/filetypes/tgz.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/tif.png` & `guidata-3.5.0/guidata/images/filetypes/tif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/txt.png` & `guidata-3.5.0/guidata/images/filetypes/txt.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/xls.png` & `guidata-3.5.0/guidata/images/filetypes/xls.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/filetypes/zip.png` & `guidata-3.5.0/guidata/images/filetypes/zip.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/guidata-banner.svg` & `guidata-3.5.0/guidata/images/guidata-vertical.svg`

 * *Files 18% similar despite different names*

```diff
@@ -1,1040 +1,1069 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
-00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
-00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
-00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
-00000070: 0a0a 3c73 7667 0a20 2020 7665 7273 696f  ..<svg.   versio
-00000080: 6e3d 2231 2e30 220a 2020 2077 6964 7468  n="1.0".   width
-00000090: 3d22 3435 322e 3836 3437 3222 0a20 2020  ="452.86472".   
-000000a0: 6865 6967 6874 3d22 3134 312e 3636 3139  height="141.6619
-000000b0: 3122 0a20 2020 6964 3d22 7376 6732 220a  1".   id="svg2".
-000000c0: 2020 2073 6f64 6970 6f64 693a 7665 7273     sodipodi:vers
-000000d0: 696f 6e3d 2230 2e33 3222 0a20 2020 696e  ion="0.32".   in
-000000e0: 6b73 6361 7065 3a76 6572 7369 6f6e 3d22  kscape:version="
-000000f0: 312e 3320 2830 6531 3530 6564 3663 342c  1.3 (0e150ed6c4,
-00000100: 2032 3032 332d 3037 2d32 3129 220a 2020   2023-07-21)".  
-00000110: 2073 6f64 6970 6f64 693a 646f 636e 616d   sodipodi:docnam
-00000120: 653d 2267 7569 6461 7461 2d62 616e 6e65  e="guidata-banne
-00000130: 722e 7376 6722 0a20 2020 696e 6b73 6361  r.svg".   inksca
-00000140: 7065 3a6f 7574 7075 745f 6578 7465 6e73  pe:output_extens
-00000150: 696f 6e3d 226f 7267 2e69 6e6b 7363 6170  ion="org.inkscap
-00000160: 652e 6f75 7470 7574 2e73 7667 2e69 6e6b  e.output.svg.ink
-00000170: 7363 6170 6522 0a20 2020 696e 6b73 6361  scape".   inksca
-00000180: 7065 3a65 7870 6f72 742d 6669 6c65 6e61  pe:export-filena
-00000190: 6d65 3d22 2e2e 5c2e 2e5c 646f 635c 696d  me="..\..\doc\im
-000001a0: 6167 6573 5c67 7569 6461 7461 2d62 616e  ages\guidata-ban
-000001b0: 6e65 722e 706e 6722 0a20 2020 696e 6b73  ner.png".   inks
-000001c0: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-000001d0: 3d22 3130 352e 3939 3139 3222 0a20 2020  ="105.99192".   
-000001e0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-000001f0: 7964 7069 3d22 3130 352e 3939 3139 3222  ydpi="105.99192"
-00000200: 0a20 2020 786d 6c6e 733a 696e 6b73 6361  .   xmlns:inksca
-00000210: 7065 3d22 6874 7470 3a2f 2f77 7777 2e69  pe="http://www.i
-00000220: 6e6b 7363 6170 652e 6f72 672f 6e61 6d65  nkscape.org/name
-00000230: 7370 6163 6573 2f69 6e6b 7363 6170 6522  spaces/inkscape"
-00000240: 0a20 2020 786d 6c6e 733a 736f 6469 706f  .   xmlns:sodipo
-00000250: 6469 3d22 6874 7470 3a2f 2f73 6f64 6970  di="http://sodip
-00000260: 6f64 692e 736f 7572 6365 666f 7267 652e  odi.sourceforge.
-00000270: 6e65 742f 4454 442f 736f 6469 706f 6469  net/DTD/sodipodi
-00000280: 2d30 2e64 7464 220a 2020 2078 6d6c 6e73  -0.dtd".   xmlns
-00000290: 3a78 6c69 6e6b 3d22 6874 7470 3a2f 2f77  :xlink="http://w
-000002a0: 7777 2e77 332e 6f72 672f 3139 3939 2f78  ww.w3.org/1999/x
-000002b0: 6c69 6e6b 220a 2020 2078 6d6c 6e73 3d22  link".   xmlns="
-000002c0: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-000002d0: 672f 3230 3030 2f73 7667 220a 2020 2078  g/2000/svg".   x
-000002e0: 6d6c 6e73 3a73 7667 3d22 6874 7470 3a2f  mlns:svg="http:/
-000002f0: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
-00000300: 2f73 7667 220a 2020 2078 6d6c 6e73 3a72  /svg".   xmlns:r
-00000310: 6466 3d22 6874 7470 3a2f 2f77 7777 2e77  df="http://www.w
-00000320: 332e 6f72 672f 3139 3939 2f30 322f 3232  3.org/1999/02/22
-00000330: 2d72 6466 2d73 796e 7461 782d 6e73 2322  -rdf-syntax-ns#"
-00000340: 0a20 2020 786d 6c6e 733a 6363 3d22 6874  .   xmlns:cc="ht
-00000350: 7470 3a2f 2f63 7265 6174 6976 6563 6f6d  tp://creativecom
-00000360: 6d6f 6e73 2e6f 7267 2f6e 7323 220a 2020  mons.org/ns#".  
-00000370: 2078 6d6c 6e73 3a64 633d 2268 7474 703a   xmlns:dc="http:
-00000380: 2f2f 7075 726c 2e6f 7267 2f64 632f 656c  //purl.org/dc/el
-00000390: 656d 656e 7473 2f31 2e31 2f22 3e0a 2020  ements/1.1/">.  
-000003a0: 3c6d 6574 6164 6174 610a 2020 2020 2069  <metadata.     i
-000003b0: 643d 226d 6574 6164 6174 6132 3139 3322  d="metadata2193"
-000003c0: 3e0a 2020 2020 3c72 6466 3a52 4446 3e0a  >.    <rdf:RDF>.
-000003d0: 2020 2020 2020 3c63 633a 576f 726b 0a20        <cc:Work. 
-000003e0: 2020 2020 2020 2020 7264 663a 6162 6f75          rdf:abou
-000003f0: 743d 2222 3e0a 2020 2020 2020 2020 3c64  t="">.        <d
-00000400: 633a 666f 726d 6174 3e69 6d61 6765 2f73  c:format>image/s
-00000410: 7667 2b78 6d6c 3c2f 6463 3a66 6f72 6d61  vg+xml</dc:forma
-00000420: 743e 0a20 2020 2020 2020 203c 6463 3a74  t>.        <dc:t
-00000430: 7970 650a 2020 2020 2020 2020 2020 2072  ype.           r
-00000440: 6466 3a72 6573 6f75 7263 653d 2268 7474  df:resource="htt
-00000450: 703a 2f2f 7075 726c 2e6f 7267 2f64 632f  p://purl.org/dc/
-00000460: 6463 6d69 7479 7065 2f53 7469 6c6c 496d  dcmitype/StillIm
-00000470: 6167 6522 202f 3e0a 2020 2020 2020 3c2f  age" />.      </
-00000480: 6363 3a57 6f72 6b3e 0a20 2020 203c 2f72  cc:Work>.    </r
-00000490: 6466 3a52 4446 3e0a 2020 3c2f 6d65 7461  df:RDF>.  </meta
-000004a0: 6461 7461 3e0a 2020 3c73 6f64 6970 6f64  data>.  <sodipod
-000004b0: 693a 6e61 6d65 6476 6965 770a 2020 2020  i:namedview.    
-000004c0: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
-000004d0: 2d68 6569 6768 743d 2231 3031 3722 0a20  -height="1017". 
-000004e0: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
-000004f0: 646f 772d 7769 6474 683d 2231 3932 3022  dow-width="1920"
-00000500: 0a20 2020 2020 696e 6b73 6361 7065 3a70  .     inkscape:p
-00000510: 6167 6573 6861 646f 773d 2232 220a 2020  ageshadow="2".  
+00000030: 226e 6f22 3f3e 0d0a 3c21 2d2d 2043 7265  "no"?>..<!-- Cre
+00000040: 6174 6564 2077 6974 6820 496e 6b73 6361  ated with Inksca
+00000050: 7065 2028 6874 7470 3a2f 2f77 7777 2e69  pe (http://www.i
+00000060: 6e6b 7363 6170 652e 6f72 672f 2920 2d2d  nkscape.org/) --
+00000070: 3e0d 0a0d 0a3c 7376 670d 0a20 2020 7665  >....<svg..   ve
+00000080: 7273 696f 6e3d 2231 2e30 220d 0a20 2020  rsion="1.0"..   
+00000090: 7769 6474 683d 2232 3830 220d 0a20 2020  width="280"..   
+000000a0: 6865 6967 6874 3d22 3234 3022 0d0a 2020  height="240"..  
+000000b0: 2069 643d 2273 7667 3222 0d0a 2020 2073   id="svg2"..   s
+000000c0: 6f64 6970 6f64 693a 7665 7273 696f 6e3d  odipodi:version=
+000000d0: 2230 2e33 3222 0d0a 2020 2069 6e6b 7363  "0.32"..   inksc
+000000e0: 6170 653a 7665 7273 696f 6e3d 2231 2e33  ape:version="1.3
+000000f0: 2028 3065 3135 3065 6436 6334 2c20 3230   (0e150ed6c4, 20
+00000100: 3233 2d30 372d 3231 2922 0d0a 2020 2073  23-07-21)"..   s
+00000110: 6f64 6970 6f64 693a 646f 636e 616d 653d  odipodi:docname=
+00000120: 2267 7569 6461 7461 2d76 6572 7469 6361  "guidata-vertica
+00000130: 6c2e 7376 6722 0d0a 2020 2069 6e6b 7363  l.svg"..   inksc
+00000140: 6170 653a 6f75 7470 7574 5f65 7874 656e  ape:output_exten
+00000150: 7369 6f6e 3d22 6f72 672e 696e 6b73 6361  sion="org.inksca
+00000160: 7065 2e6f 7574 7075 742e 7376 672e 696e  pe.output.svg.in
+00000170: 6b73 6361 7065 220d 0a20 2020 696e 6b73  kscape"..   inks
+00000180: 6361 7065 3a65 7870 6f72 742d 6669 6c65  cape:export-file
+00000190: 6e61 6d65 3d22 2e2e 5c2e 2e5c 646f 635c  name="..\..\doc\
+000001a0: 696d 6167 6573 5c67 7569 6461 7461 2d76  images\guidata-v
+000001b0: 6572 7469 6361 6c2e 706e 6722 0d0a 2020  ertical.png"..  
+000001c0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+000001d0: 2d78 6470 693d 2234 322e 3835 3731 3433  -xdpi="42.857143
+000001e0: 220d 0a20 2020 696e 6b73 6361 7065 3a65  "..   inkscape:e
+000001f0: 7870 6f72 742d 7964 7069 3d22 3432 2e38  xport-ydpi="42.8
+00000200: 3537 3134 3322 0d0a 2020 2078 6d6c 6e73  57143"..   xmlns
+00000210: 3a69 6e6b 7363 6170 653d 2268 7474 703a  :inkscape="http:
+00000220: 2f2f 7777 772e 696e 6b73 6361 7065 2e6f  //www.inkscape.o
+00000230: 7267 2f6e 616d 6573 7061 6365 732f 696e  rg/namespaces/in
+00000240: 6b73 6361 7065 220d 0a20 2020 786d 6c6e  kscape"..   xmln
+00000250: 733a 736f 6469 706f 6469 3d22 6874 7470  s:sodipodi="http
+00000260: 3a2f 2f73 6f64 6970 6f64 692e 736f 7572  ://sodipodi.sour
+00000270: 6365 666f 7267 652e 6e65 742f 4454 442f  ceforge.net/DTD/
+00000280: 736f 6469 706f 6469 2d30 2e64 7464 220d  sodipodi-0.dtd".
+00000290: 0a20 2020 786d 6c6e 733a 786c 696e 6b3d  .   xmlns:xlink=
+000002a0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+000002b0: 7267 2f31 3939 392f 786c 696e 6b22 0d0a  rg/1999/xlink"..
+000002c0: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
+000002d0: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
+000002e0: 2f73 7667 220d 0a20 2020 786d 6c6e 733a  /svg"..   xmlns:
+000002f0: 7376 673d 2268 7474 703a 2f2f 7777 772e  svg="http://www.
+00000300: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
+00000310: 0d0a 2020 2078 6d6c 6e73 3a72 6466 3d22  ..   xmlns:rdf="
+00000320: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+00000330: 672f 3139 3939 2f30 322f 3232 2d72 6466  g/1999/02/22-rdf
+00000340: 2d73 796e 7461 782d 6e73 2322 0d0a 2020  -syntax-ns#"..  
+00000350: 2078 6d6c 6e73 3a63 633d 2268 7474 703a   xmlns:cc="http:
+00000360: 2f2f 6372 6561 7469 7665 636f 6d6d 6f6e  //creativecommon
+00000370: 732e 6f72 672f 6e73 2322 0d0a 2020 2078  s.org/ns#"..   x
+00000380: 6d6c 6e73 3a64 633d 2268 7474 703a 2f2f  mlns:dc="http://
+00000390: 7075 726c 2e6f 7267 2f64 632f 656c 656d  purl.org/dc/elem
+000003a0: 656e 7473 2f31 2e31 2f22 3e0d 0a20 203c  ents/1.1/">..  <
+000003b0: 6d65 7461 6461 7461 0d0a 2020 2020 2069  metadata..     i
+000003c0: 643d 226d 6574 6164 6174 6132 3139 3322  d="metadata2193"
+000003d0: 3e0d 0a20 2020 203c 7264 663a 5244 463e  >..    <rdf:RDF>
+000003e0: 0d0a 2020 2020 2020 3c63 633a 576f 726b  ..      <cc:Work
+000003f0: 0d0a 2020 2020 2020 2020 2072 6466 3a61  ..         rdf:a
+00000400: 626f 7574 3d22 223e 0d0a 2020 2020 2020  bout="">..      
+00000410: 2020 3c64 633a 666f 726d 6174 3e69 6d61    <dc:format>ima
+00000420: 6765 2f73 7667 2b78 6d6c 3c2f 6463 3a66  ge/svg+xml</dc:f
+00000430: 6f72 6d61 743e 0d0a 2020 2020 2020 2020  ormat>..        
+00000440: 3c64 633a 7479 7065 0d0a 2020 2020 2020  <dc:type..      
+00000450: 2020 2020 2072 6466 3a72 6573 6f75 7263       rdf:resourc
+00000460: 653d 2268 7474 703a 2f2f 7075 726c 2e6f  e="http://purl.o
+00000470: 7267 2f64 632f 6463 6d69 7479 7065 2f53  rg/dc/dcmitype/S
+00000480: 7469 6c6c 496d 6167 6522 202f 3e0d 0a20  tillImage" />.. 
+00000490: 2020 2020 203c 2f63 633a 576f 726b 3e0d       </cc:Work>.
+000004a0: 0a20 2020 203c 2f72 6466 3a52 4446 3e0d  .    </rdf:RDF>.
+000004b0: 0a20 203c 2f6d 6574 6164 6174 613e 0d0a  .  </metadata>..
+000004c0: 2020 3c73 6f64 6970 6f64 693a 6e61 6d65    <sodipodi:name
+000004d0: 6476 6965 770d 0a20 2020 2020 696e 6b73  dview..     inks
+000004e0: 6361 7065 3a77 696e 646f 772d 6865 6967  cape:window-heig
+000004f0: 6874 3d22 3130 3137 220d 0a20 2020 2020  ht="1017"..     
+00000500: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
+00000510: 7769 6474 683d 2231 3932 3022 0d0a 2020  width="1920"..  
 00000520: 2020 2069 6e6b 7363 6170 653a 7061 6765     inkscape:page
-00000530: 6f70 6163 6974 793d 2230 2e30 220a 2020  opacity="0.0".  
-00000540: 2020 2062 6f72 6465 726f 7061 6369 7479     borderopacity
-00000550: 3d22 312e 3022 0a20 2020 2020 626f 7264  ="1.0".     bord
-00000560: 6572 636f 6c6f 723d 2223 3636 3636 3636  ercolor="#666666
-00000570: 220a 2020 2020 2070 6167 6563 6f6c 6f72  ".     pagecolor
-00000580: 3d22 2366 6666 6666 6622 0a20 2020 2020  ="#ffffff".     
-00000590: 6964 3d22 6261 7365 220a 2020 2020 2069  id="base".     i
-000005a0: 6e6b 7363 6170 653a 7a6f 6f6d 3d22 312e  nkscape:zoom="1.
-000005b0: 3939 3939 3939 3922 0a20 2020 2020 696e  9999999".     in
-000005c0: 6b73 6361 7065 3a63 783d 2231 3936 2e30  kscape:cx="196.0
-000005d0: 3030 3031 220a 2020 2020 2069 6e6b 7363  0001".     inksc
-000005e0: 6170 653a 6379 3d22 3736 2e32 3530 3030  ape:cy="76.25000
-000005f0: 3322 0a20 2020 2020 696e 6b73 6361 7065  3".     inkscape
-00000600: 3a77 696e 646f 772d 783d 222d 3822 0a20  :window-x="-8". 
-00000610: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
-00000620: 646f 772d 793d 222d 3822 0a20 2020 2020  dow-y="-8".     
-00000630: 696e 6b73 6361 7065 3a63 7572 7265 6e74  inkscape:current
-00000640: 2d6c 6179 6572 3d22 7376 6732 220a 2020  -layer="svg2".  
-00000650: 2020 2073 686f 7767 7269 643d 2266 616c     showgrid="fal
-00000660: 7365 220a 2020 2020 2066 6974 2d6d 6172  se".     fit-mar
-00000670: 6769 6e2d 746f 703d 2230 220a 2020 2020  gin-top="0".    
-00000680: 2066 6974 2d6d 6172 6769 6e2d 6c65 6674   fit-margin-left
-00000690: 3d22 3022 0a20 2020 2020 6669 742d 6d61  ="0".     fit-ma
-000006a0: 7267 696e 2d72 6967 6874 3d22 3022 0a20  rgin-right="0". 
-000006b0: 2020 2020 6669 742d 6d61 7267 696e 2d62      fit-margin-b
-000006c0: 6f74 746f 6d3d 2230 220a 2020 2020 2069  ottom="0".     i
-000006d0: 6e6b 7363 6170 653a 7769 6e64 6f77 2d6d  nkscape:window-m
-000006e0: 6178 696d 697a 6564 3d22 3122 0a20 2020  aximized="1".   
-000006f0: 2020 696e 6b73 6361 7065 3a73 686f 7770    inkscape:showp
-00000700: 6167 6573 6861 646f 773d 2232 220a 2020  ageshadow="2".  
-00000710: 2020 2069 6e6b 7363 6170 653a 7061 6765     inkscape:page
-00000720: 6368 6563 6b65 7262 6f61 7264 3d22 7472  checkerboard="tr
-00000730: 7565 220a 2020 2020 2069 6e6b 7363 6170  ue".     inkscap
-00000740: 653a 6465 736b 636f 6c6f 723d 2223 6431  e:deskcolor="#d1
-00000750: 6431 6431 2220 2f3e 0a20 203c 6465 6673  d1d1" />.  <defs
-00000760: 0a20 2020 2020 6964 3d22 6465 6673 3422  .     id="defs4"
-00000770: 3e0a 2020 2020 3c6d 6172 6b65 720a 2020  >.    <marker.  
-00000780: 2020 2020 2069 6e6b 7363 6170 653a 7374       inkscape:st
-00000790: 6f63 6b69 643d 2241 7272 6f77 324d 656e  ockid="Arrow2Men
-000007a0: 6422 0a20 2020 2020 2020 6f72 6965 6e74  d".       orient
-000007b0: 3d22 6175 746f 220a 2020 2020 2020 2072  ="auto".       r
-000007c0: 6566 593d 2230 220a 2020 2020 2020 2072  efY="0".       r
-000007d0: 6566 583d 2230 220a 2020 2020 2020 2069  efX="0".       i
-000007e0: 643d 2241 7272 6f77 324d 656e 6422 0a20  d="Arrow2Mend". 
-000007f0: 2020 2020 2020 7374 796c 653d 226f 7665        style="ove
-00000800: 7266 6c6f 773a 7669 7369 626c 6522 3e0a  rflow:visible">.
-00000810: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
-00000820: 2020 2020 2069 643d 2270 6174 6833 3930       id="path390
-00000830: 3822 0a20 2020 2020 2020 2020 7374 796c  8".         styl
-00000840: 653d 2266 6f6e 742d 7369 7a65 3a31 3270  e="font-size:12p
-00000850: 783b 6669 6c6c 2d72 756c 653a 6576 656e  x;fill-rule:even
-00000860: 6f64 643b 7374 726f 6b65 2d77 6964 7468  odd;stroke-width
-00000870: 3a30 2e36 3235 3b73 7472 6f6b 652d 6c69  :0.625;stroke-li
-00000880: 6e65 6a6f 696e 3a72 6f75 6e64 220a 2020  nejoin:round".  
-00000890: 2020 2020 2020 2064 3d22 4d20 382e 3731         d="M 8.71
-000008a0: 3835 3837 382c 342e 3033 3337 3335 3220  85878,4.0337352 
-000008b0: 2d32 2e32 3037 3238 3935 2c30 2e30 3136  -2.2072895,0.016
-000008c0: 3031 3332 3620 382e 3731 3835 3838 342c  01326 8.7185884,
-000008d0: 2d34 2e30 3031 3730 3738 2063 202d 312e  -4.0017078 c -1.
-000008e0: 3734 3534 3938 342c 322e 3337 3230 3630  7454984,2.372060
-000008f0: 3920 2d31 2e37 3335 3434 3038 2c35 2e36  9 -1.7354408,5.6
-00000900: 3137 3435 3139 202d 3665 2d37 2c38 2e30  174519 -6e-7,8.0
-00000910: 3335 3434 3320 7a22 0a20 2020 2020 2020  35443 z".       
-00000920: 2020 7472 616e 7366 6f72 6d3d 2273 6361    transform="sca
-00000930: 6c65 282d 302e 3629 220a 2020 2020 2020  le(-0.6)".      
-00000940: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00000950: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-00000960: 2230 2220 2f3e 0a20 2020 203c 2f6d 6172  "0" />.    </mar
-00000970: 6b65 723e 0a20 2020 203c 6d61 726b 6572  ker>.    <marker
-00000980: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00000990: 3a73 746f 636b 6964 3d22 4172 726f 7731  :stockid="Arrow1
-000009a0: 5365 6e64 220a 2020 2020 2020 206f 7269  Send".       ori
-000009b0: 656e 743d 2261 7574 6f22 0a20 2020 2020  ent="auto".     
-000009c0: 2020 7265 6659 3d22 3022 0a20 2020 2020    refY="0".     
-000009d0: 2020 7265 6658 3d22 3022 0a20 2020 2020    refX="0".     
-000009e0: 2020 6964 3d22 4172 726f 7731 5365 6e64    id="Arrow1Send
-000009f0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-00000a00: 6f76 6572 666c 6f77 3a76 6973 6962 6c65  overflow:visible
-00000a10: 223e 0a20 2020 2020 203c 7061 7468 0a20  ">.      <path. 
-00000a20: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00000a30: 3338 3936 220a 2020 2020 2020 2020 2064  3896".         d
-00000a40: 3d22 4d20 302c 3020 352c 2d35 202d 3132  ="M 0,0 5,-5 -12
-00000a50: 2e35 2c30 2035 2c35 205a 220a 2020 2020  .5,0 5,5 Z".    
-00000a60: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00000a70: 2d72 756c 653a 6576 656e 6f64 643b 7374  -rule:evenodd;st
-00000a80: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
-00000a90: 6f6b 652d 7769 6474 683a 3170 743b 6d61  oke-width:1pt;ma
-00000aa0: 726b 6572 2d73 7461 7274 3a6e 6f6e 6522  rker-start:none"
-00000ab0: 0a20 2020 2020 2020 2020 7472 616e 7366  .         transf
-00000ac0: 6f72 6d3d 226d 6174 7269 7828 2d30 2e32  orm="matrix(-0.2
-00000ad0: 2c30 2c30 2c2d 302e 322c 2d31 2e32 2c30  ,0,0,-0.2,-1.2,0
-00000ae0: 2922 0a20 2020 2020 2020 2020 696e 6b73  )".         inks
-00000af0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-00000b00: 7572 7661 7475 7265 3d22 3022 202f 3e0a  urvature="0" />.
-00000b10: 2020 2020 3c2f 6d61 726b 6572 3e0a 2020      </marker>.  
-00000b20: 2020 3c6d 6172 6b65 720a 2020 2020 2020    <marker.      
-00000b30: 2069 6e6b 7363 6170 653a 7374 6f63 6b69   inkscape:stocki
-00000b40: 643d 2241 7272 6f77 314d 656e 6422 0a20  d="Arrow1Mend". 
-00000b50: 2020 2020 2020 6f72 6965 6e74 3d22 6175        orient="au
-00000b60: 746f 220a 2020 2020 2020 2072 6566 593d  to".       refY=
-00000b70: 2230 220a 2020 2020 2020 2072 6566 583d  "0".       refX=
-00000b80: 2230 220a 2020 2020 2020 2069 643d 2241  "0".       id="A
-00000b90: 7272 6f77 314d 656e 6422 0a20 2020 2020  rrow1Mend".     
-00000ba0: 2020 7374 796c 653d 226f 7665 7266 6c6f    style="overflo
-00000bb0: 773a 7669 7369 626c 6522 3e0a 2020 2020  w:visible">.    
-00000bc0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00000bd0: 2069 643d 2270 6174 6833 3839 3022 0a20   id="path3890". 
-00000be0: 2020 2020 2020 2020 643d 224d 2030 2c30          d="M 0,0
-00000bf0: 2035 2c2d 3520 2d31 322e 352c 3020 352c   5,-5 -12.5,0 5,
-00000c00: 3520 5a22 0a20 2020 2020 2020 2020 7374  5 Z".         st
-00000c10: 796c 653d 2266 696c 6c2d 7275 6c65 3a65  yle="fill-rule:e
-00000c20: 7665 6e6f 6464 3b73 7472 6f6b 653a 2330  venodd;stroke:#0
-00000c30: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
-00000c40: 7468 3a31 7074 3b6d 6172 6b65 722d 7374  th:1pt;marker-st
-00000c50: 6172 743a 6e6f 6e65 220a 2020 2020 2020  art:none".      
-00000c60: 2020 2074 7261 6e73 666f 726d 3d22 6d61     transform="ma
-00000c70: 7472 6978 282d 302e 342c 302c 302c 2d30  trix(-0.4,0,0,-0
-00000c80: 2e34 2c2d 342c 3029 220a 2020 2020 2020  .4,-4,0)".      
-00000c90: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00000ca0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-00000cb0: 2230 2220 2f3e 0a20 2020 203c 2f6d 6172  "0" />.    </mar
-00000cc0: 6b65 723e 0a20 2020 203c 6d61 726b 6572  ker>.    <marker
-00000cd0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00000ce0: 3a73 746f 636b 6964 3d22 4172 726f 7732  :stockid="Arrow2
-00000cf0: 4c65 6e64 220a 2020 2020 2020 206f 7269  Lend".       ori
-00000d00: 656e 743d 2261 7574 6f22 0a20 2020 2020  ent="auto".     
-00000d10: 2020 7265 6659 3d22 3022 0a20 2020 2020    refY="0".     
-00000d20: 2020 7265 6658 3d22 3022 0a20 2020 2020    refX="0".     
-00000d30: 2020 6964 3d22 4172 726f 7732 4c65 6e64    id="Arrow2Lend
-00000d40: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-00000d50: 6f76 6572 666c 6f77 3a76 6973 6962 6c65  overflow:visible
-00000d60: 223e 0a20 2020 2020 203c 7061 7468 0a20  ">.      <path. 
-00000d70: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00000d80: 3339 3032 220a 2020 2020 2020 2020 2073  3902".         s
-00000d90: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
-00000da0: 3132 7078 3b66 696c 6c2d 7275 6c65 3a65  12px;fill-rule:e
-00000db0: 7665 6e6f 6464 3b73 7472 6f6b 652d 7769  venodd;stroke-wi
-00000dc0: 6474 683a 302e 3632 353b 7374 726f 6b65  dth:0.625;stroke
-00000dd0: 2d6c 696e 656a 6f69 6e3a 726f 756e 6422  -linejoin:round"
-00000de0: 0a20 2020 2020 2020 2020 643d 224d 2038  .         d="M 8
-00000df0: 2e37 3138 3538 3738 2c34 2e30 3333 3733  .7185878,4.03373
-00000e00: 3532 202d 322e 3230 3732 3839 352c 302e  52 -2.2072895,0.
-00000e10: 3031 3630 3133 3236 2038 2e37 3138 3538  01601326 8.71858
-00000e20: 3834 2c2d 342e 3030 3137 3037 3820 6320  84,-4.0017078 c 
-00000e30: 2d31 2e37 3435 3439 3834 2c32 2e33 3732  -1.7454984,2.372
-00000e40: 3036 3039 202d 312e 3733 3534 3430 382c  0609 -1.7354408,
-00000e50: 352e 3631 3734 3531 3920 2d36 652d 372c  5.6174519 -6e-7,
-00000e60: 382e 3033 3534 3433 207a 220a 2020 2020  8.035443 z".    
-00000e70: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
-00000e80: 6d61 7472 6978 282d 312e 312c 302c 302c  matrix(-1.1,0,0,
-00000e90: 2d31 2e31 2c2d 312e 312c 3029 220a 2020  -1.1,-1.1,0)".  
-00000ea0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00000eb0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00000ec0: 7572 653d 2230 2220 2f3e 0a20 2020 203c  ure="0" />.    <
-00000ed0: 2f6d 6172 6b65 723e 0a20 2020 203c 6c69  /marker>.    <li
-00000ee0: 6e65 6172 4772 6164 6965 6e74 0a20 2020  nearGradient.   
-00000ef0: 2020 2020 6964 3d22 6c69 6e65 6172 4772      id="linearGr
-00000f00: 6164 6965 6e74 3338 3132 223e 0a20 2020  adient3812">.   
-00000f10: 2020 203c 7374 6f70 0a20 2020 2020 2020     <stop.       
-00000f20: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
-00000f30: 6c6f 723a 2364 3264 3264 323b 7374 6f70  lor:#d2d2d2;stop
-00000f40: 2d6f 7061 6369 7479 3a31 3b22 0a20 2020  -opacity:1;".   
-00000f50: 2020 2020 2020 6f66 6673 6574 3d22 3022        offset="0"
-00000f60: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
-00000f70: 6f70 3338 3134 2220 2f3e 0a20 2020 2020  op3814" />.     
-00000f80: 203c 7374 6f70 0a20 2020 2020 2020 2020   <stop.         
+00000530: 7368 6164 6f77 3d22 3222 0d0a 2020 2020  shadow="2"..    
+00000540: 2069 6e6b 7363 6170 653a 7061 6765 6f70   inkscape:pageop
+00000550: 6163 6974 793d 2230 2e30 220d 0a20 2020  acity="0.0"..   
+00000560: 2020 626f 7264 6572 6f70 6163 6974 793d    borderopacity=
+00000570: 2231 2e30 220d 0a20 2020 2020 626f 7264  "1.0"..     bord
+00000580: 6572 636f 6c6f 723d 2223 3636 3636 3636  ercolor="#666666
+00000590: 220d 0a20 2020 2020 7061 6765 636f 6c6f  "..     pagecolo
+000005a0: 723d 2223 6666 6666 6666 220d 0a20 2020  r="#ffffff"..   
+000005b0: 2020 6964 3d22 6261 7365 220d 0a20 2020    id="base"..   
+000005c0: 2020 696e 6b73 6361 7065 3a7a 6f6f 6d3d    inkscape:zoom=
+000005d0: 2232 2e38 3238 3432 3722 0d0a 2020 2020  "2.828427"..    
+000005e0: 2069 6e6b 7363 6170 653a 6378 3d22 3137   inkscape:cx="17
+000005f0: 392e 3935 3836 3822 0d0a 2020 2020 2069  9.95868"..     i
+00000600: 6e6b 7363 6170 653a 6379 3d22 3133 372e  nkscape:cy="137.
+00000610: 3030 3139 3422 0d0a 2020 2020 2069 6e6b  00194"..     ink
+00000620: 7363 6170 653a 7769 6e64 6f77 2d78 3d22  scape:window-x="
+00000630: 2d38 220d 0a20 2020 2020 696e 6b73 6361  -8"..     inksca
+00000640: 7065 3a77 696e 646f 772d 793d 222d 3822  pe:window-y="-8"
+00000650: 0d0a 2020 2020 2069 6e6b 7363 6170 653a  ..     inkscape:
+00000660: 6375 7272 656e 742d 6c61 7965 723d 2273  current-layer="s
+00000670: 7667 3222 0d0a 2020 2020 2073 686f 7767  vg2"..     showg
+00000680: 7269 643d 2266 616c 7365 220d 0a20 2020  rid="false"..   
+00000690: 2020 6669 742d 6d61 7267 696e 2d74 6f70    fit-margin-top
+000006a0: 3d22 3022 0d0a 2020 2020 2066 6974 2d6d  ="0"..     fit-m
+000006b0: 6172 6769 6e2d 6c65 6674 3d22 3022 0d0a  argin-left="0"..
+000006c0: 2020 2020 2066 6974 2d6d 6172 6769 6e2d       fit-margin-
+000006d0: 7269 6768 743d 2230 220d 0a20 2020 2020  right="0"..     
+000006e0: 6669 742d 6d61 7267 696e 2d62 6f74 746f  fit-margin-botto
+000006f0: 6d3d 2230 220d 0a20 2020 2020 696e 6b73  m="0"..     inks
+00000700: 6361 7065 3a77 696e 646f 772d 6d61 7869  cape:window-maxi
+00000710: 6d69 7a65 643d 2231 220d 0a20 2020 2020  mized="1"..     
+00000720: 696e 6b73 6361 7065 3a73 686f 7770 6167  inkscape:showpag
+00000730: 6573 6861 646f 773d 2232 220d 0a20 2020  eshadow="2"..   
+00000740: 2020 696e 6b73 6361 7065 3a70 6167 6563    inkscape:pagec
+00000750: 6865 636b 6572 626f 6172 643d 2274 7275  heckerboard="tru
+00000760: 6522 0d0a 2020 2020 2069 6e6b 7363 6170  e"..     inkscap
+00000770: 653a 6465 736b 636f 6c6f 723d 2223 6431  e:deskcolor="#d1
+00000780: 6431 6431 2220 2f3e 0d0a 2020 3c64 6566  d1d1" />..  <def
+00000790: 730d 0a20 2020 2020 6964 3d22 6465 6673  s..     id="defs
+000007a0: 3422 3e0d 0a20 2020 203c 6d61 726b 6572  4">..    <marker
+000007b0: 0d0a 2020 2020 2020 2069 6e6b 7363 6170  ..       inkscap
+000007c0: 653a 7374 6f63 6b69 643d 2241 7272 6f77  e:stockid="Arrow
+000007d0: 324d 656e 6422 0d0a 2020 2020 2020 206f  2Mend"..       o
+000007e0: 7269 656e 743d 2261 7574 6f22 0d0a 2020  rient="auto"..  
+000007f0: 2020 2020 2072 6566 593d 2230 220d 0a20       refY="0".. 
+00000800: 2020 2020 2020 7265 6658 3d22 3022 0d0a        refX="0"..
+00000810: 2020 2020 2020 2069 643d 2241 7272 6f77         id="Arrow
+00000820: 324d 656e 6422 0d0a 2020 2020 2020 2073  2Mend"..       s
+00000830: 7479 6c65 3d22 6f76 6572 666c 6f77 3a76  tyle="overflow:v
+00000840: 6973 6962 6c65 223e 0d0a 2020 2020 2020  isible">..      
+00000850: 3c70 6174 680d 0a20 2020 2020 2020 2020  <path..         
+00000860: 6964 3d22 7061 7468 3339 3038 220d 0a20  id="path3908".. 
+00000870: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00000880: 6f6e 742d 7369 7a65 3a31 3270 783b 6669  ont-size:12px;fi
+00000890: 6c6c 2d72 756c 653a 6576 656e 6f64 643b  ll-rule:evenodd;
+000008a0: 7374 726f 6b65 2d77 6964 7468 3a30 2e36  stroke-width:0.6
+000008b0: 3235 3b73 7472 6f6b 652d 6c69 6e65 6a6f  25;stroke-linejo
+000008c0: 696e 3a72 6f75 6e64 220d 0a20 2020 2020  in:round"..     
+000008d0: 2020 2020 643d 224d 2038 2e37 3138 3538      d="M 8.71858
+000008e0: 3738 2c34 2e30 3333 3733 3532 202d 322e  78,4.0337352 -2.
+000008f0: 3230 3732 3839 352c 302e 3031 3630 3133  2072895,0.016013
+00000900: 3236 2038 2e37 3138 3538 3834 2c2d 342e  26 8.7185884,-4.
+00000910: 3030 3137 3037 3820 6320 2d31 2e37 3435  0017078 c -1.745
+00000920: 3439 3834 2c32 2e33 3732 3036 3039 202d  4984,2.3720609 -
+00000930: 312e 3733 3534 3430 382c 352e 3631 3734  1.7354408,5.6174
+00000940: 3531 3920 2d36 652d 372c 382e 3033 3534  519 -6e-7,8.0354
+00000950: 3433 207a 220d 0a20 2020 2020 2020 2020  43 z"..         
+00000960: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
+00000970: 282d 302e 3629 220d 0a20 2020 2020 2020  (-0.6)"..       
+00000980: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+00000990: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+000009a0: 3022 202f 3e0d 0a20 2020 203c 2f6d 6172  0" />..    </mar
+000009b0: 6b65 723e 0d0a 2020 2020 3c6d 6172 6b65  ker>..    <marke
+000009c0: 720d 0a20 2020 2020 2020 696e 6b73 6361  r..       inksca
+000009d0: 7065 3a73 746f 636b 6964 3d22 4172 726f  pe:stockid="Arro
+000009e0: 7731 5365 6e64 220d 0a20 2020 2020 2020  w1Send"..       
+000009f0: 6f72 6965 6e74 3d22 6175 746f 220d 0a20  orient="auto".. 
+00000a00: 2020 2020 2020 7265 6659 3d22 3022 0d0a        refY="0"..
+00000a10: 2020 2020 2020 2072 6566 583d 2230 220d         refX="0".
+00000a20: 0a20 2020 2020 2020 6964 3d22 4172 726f  .       id="Arro
+00000a30: 7731 5365 6e64 220d 0a20 2020 2020 2020  w1Send"..       
+00000a40: 7374 796c 653d 226f 7665 7266 6c6f 773a  style="overflow:
+00000a50: 7669 7369 626c 6522 3e0d 0a20 2020 2020  visible">..     
+00000a60: 203c 7061 7468 0d0a 2020 2020 2020 2020   <path..        
+00000a70: 2069 643d 2270 6174 6833 3839 3622 0d0a   id="path3896"..
+00000a80: 2020 2020 2020 2020 2064 3d22 4d20 302c           d="M 0,
+00000a90: 3020 352c 2d35 202d 3132 2e35 2c30 2035  0 5,-5 -12.5,0 5
+00000aa0: 2c35 205a 220d 0a20 2020 2020 2020 2020  ,5 Z"..         
+00000ab0: 7374 796c 653d 2266 696c 6c2d 7275 6c65  style="fill-rule
+00000ac0: 3a65 7665 6e6f 6464 3b73 7472 6f6b 653a  :evenodd;stroke:
+00000ad0: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+00000ae0: 6964 7468 3a31 7074 3b6d 6172 6b65 722d  idth:1pt;marker-
+00000af0: 7374 6172 743a 6e6f 6e65 220d 0a20 2020  start:none"..   
+00000b00: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
+00000b10: 226d 6174 7269 7828 2d30 2e32 2c30 2c30  "matrix(-0.2,0,0
+00000b20: 2c2d 302e 322c 2d31 2e32 2c30 2922 0d0a  ,-0.2,-1.2,0)"..
+00000b30: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00000b40: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00000b50: 6174 7572 653d 2230 2220 2f3e 0d0a 2020  ature="0" />..  
+00000b60: 2020 3c2f 6d61 726b 6572 3e0d 0a20 2020    </marker>..   
+00000b70: 203c 6d61 726b 6572 0d0a 2020 2020 2020   <marker..      
+00000b80: 2069 6e6b 7363 6170 653a 7374 6f63 6b69   inkscape:stocki
+00000b90: 643d 2241 7272 6f77 314d 656e 6422 0d0a  d="Arrow1Mend"..
+00000ba0: 2020 2020 2020 206f 7269 656e 743d 2261         orient="a
+00000bb0: 7574 6f22 0d0a 2020 2020 2020 2072 6566  uto"..       ref
+00000bc0: 593d 2230 220d 0a20 2020 2020 2020 7265  Y="0"..       re
+00000bd0: 6658 3d22 3022 0d0a 2020 2020 2020 2069  fX="0"..       i
+00000be0: 643d 2241 7272 6f77 314d 656e 6422 0d0a  d="Arrow1Mend"..
+00000bf0: 2020 2020 2020 2073 7479 6c65 3d22 6f76         style="ov
+00000c00: 6572 666c 6f77 3a76 6973 6962 6c65 223e  erflow:visible">
+00000c10: 0d0a 2020 2020 2020 3c70 6174 680d 0a20  ..      <path.. 
+00000c20: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00000c30: 3338 3930 220d 0a20 2020 2020 2020 2020  3890"..         
+00000c40: 643d 224d 2030 2c30 2035 2c2d 3520 2d31  d="M 0,0 5,-5 -1
+00000c50: 322e 352c 3020 352c 3520 5a22 0d0a 2020  2.5,0 5,5 Z"..  
+00000c60: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00000c70: 6c6c 2d72 756c 653a 6576 656e 6f64 643b  ll-rule:evenodd;
+00000c80: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
+00000c90: 7472 6f6b 652d 7769 6474 683a 3170 743b  troke-width:1pt;
+00000ca0: 6d61 726b 6572 2d73 7461 7274 3a6e 6f6e  marker-start:non
+00000cb0: 6522 0d0a 2020 2020 2020 2020 2074 7261  e"..         tra
+00000cc0: 6e73 666f 726d 3d22 6d61 7472 6978 282d  nsform="matrix(-
+00000cd0: 302e 342c 302c 302c 2d30 2e34 2c2d 342c  0.4,0,0,-0.4,-4,
+00000ce0: 3029 220d 0a20 2020 2020 2020 2020 696e  0)"..         in
+00000cf0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00000d00: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
+00000d10: 3e0d 0a20 2020 203c 2f6d 6172 6b65 723e  >..    </marker>
+00000d20: 0d0a 2020 2020 3c6d 6172 6b65 720d 0a20  ..    <marker.. 
+00000d30: 2020 2020 2020 696e 6b73 6361 7065 3a73        inkscape:s
+00000d40: 746f 636b 6964 3d22 4172 726f 7732 4c65  tockid="Arrow2Le
+00000d50: 6e64 220d 0a20 2020 2020 2020 6f72 6965  nd"..       orie
+00000d60: 6e74 3d22 6175 746f 220d 0a20 2020 2020  nt="auto"..     
+00000d70: 2020 7265 6659 3d22 3022 0d0a 2020 2020    refY="0"..    
+00000d80: 2020 2072 6566 583d 2230 220d 0a20 2020     refX="0"..   
+00000d90: 2020 2020 6964 3d22 4172 726f 7732 4c65      id="Arrow2Le
+00000da0: 6e64 220d 0a20 2020 2020 2020 7374 796c  nd"..       styl
+00000db0: 653d 226f 7665 7266 6c6f 773a 7669 7369  e="overflow:visi
+00000dc0: 626c 6522 3e0d 0a20 2020 2020 203c 7061  ble">..      <pa
+00000dd0: 7468 0d0a 2020 2020 2020 2020 2069 643d  th..         id=
+00000de0: 2270 6174 6833 3930 3222 0d0a 2020 2020  "path3902"..    
+00000df0: 2020 2020 2073 7479 6c65 3d22 666f 6e74       style="font
+00000e00: 2d73 697a 653a 3132 7078 3b66 696c 6c2d  -size:12px;fill-
+00000e10: 7275 6c65 3a65 7665 6e6f 6464 3b73 7472  rule:evenodd;str
+00000e20: 6f6b 652d 7769 6474 683a 302e 3632 353b  oke-width:0.625;
+00000e30: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00000e40: 726f 756e 6422 0d0a 2020 2020 2020 2020  round"..        
+00000e50: 2064 3d22 4d20 382e 3731 3835 3837 382c   d="M 8.7185878,
+00000e60: 342e 3033 3337 3335 3220 2d32 2e32 3037  4.0337352 -2.207
+00000e70: 3238 3935 2c30 2e30 3136 3031 3332 3620  2895,0.01601326 
+00000e80: 382e 3731 3835 3838 342c 2d34 2e30 3031  8.7185884,-4.001
+00000e90: 3730 3738 2063 202d 312e 3734 3534 3938  7078 c -1.745498
+00000ea0: 342c 322e 3337 3230 3630 3920 2d31 2e37  4,2.3720609 -1.7
+00000eb0: 3335 3434 3038 2c35 2e36 3137 3435 3139  354408,5.6174519
+00000ec0: 202d 3665 2d37 2c38 2e30 3335 3434 3320   -6e-7,8.035443 
+00000ed0: 7a22 0d0a 2020 2020 2020 2020 2074 7261  z"..         tra
+00000ee0: 6e73 666f 726d 3d22 6d61 7472 6978 282d  nsform="matrix(-
+00000ef0: 312e 312c 302c 302c 2d31 2e31 2c2d 312e  1.1,0,0,-1.1,-1.
+00000f00: 312c 3029 220d 0a20 2020 2020 2020 2020  1,0)"..         
+00000f10: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+00000f20: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+00000f30: 202f 3e0d 0a20 2020 203c 2f6d 6172 6b65   />..    </marke
+00000f40: 723e 0d0a 2020 2020 3c6c 696e 6561 7247  r>..    <linearG
+00000f50: 7261 6469 656e 740d 0a20 2020 2020 2020  radient..       
+00000f60: 6964 3d22 6c69 6e65 6172 4772 6164 6965  id="linearGradie
+00000f70: 6e74 3338 3132 223e 0d0a 2020 2020 2020  nt3812">..      
+00000f80: 3c73 746f 700d 0a20 2020 2020 2020 2020  <stop..         
 00000f90: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
-00000fa0: 723a 2366 6666 6666 663b 7374 6f70 2d6f  r:#ffffff;stop-o
-00000fb0: 7061 6369 7479 3a31 3b22 0a20 2020 2020  pacity:1;".     
-00000fc0: 2020 2020 6f66 6673 6574 3d22 3122 0a20      offset="1". 
-00000fd0: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
-00000fe0: 3338 3136 2220 2f3e 0a20 2020 203c 2f6c  3816" />.    </l
-00000ff0: 696e 6561 7247 7261 6469 656e 743e 0a20  inearGradient>. 
-00001000: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-00001010: 6e74 0a20 2020 2020 2020 6964 3d22 6c69  nt.       id="li
-00001020: 6e65 6172 4772 6164 6965 6e74 3338 3032  nearGradient3802
-00001030: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00001040: 653a 7377 6174 6368 3d22 736f 6c69 6422  e:swatch="solid"
-00001050: 3e0a 2020 2020 2020 3c73 746f 700a 2020  >.      <stop.  
-00001060: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
-00001070: 6f70 2d63 6f6c 6f72 3a23 3830 3830 3830  op-color:#808080
-00001080: 3b73 746f 702d 6f70 6163 6974 793a 313b  ;stop-opacity:1;
-00001090: 220a 2020 2020 2020 2020 206f 6666 7365  ".         offse
-000010a0: 743d 2230 220a 2020 2020 2020 2020 2069  t="0".         i
-000010b0: 643d 2273 746f 7033 3830 3422 202f 3e0a  d="stop3804" />.
-000010c0: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
-000010d0: 6965 6e74 3e0a 2020 2020 3c6c 696e 6561  ient>.    <linea
-000010e0: 7247 7261 6469 656e 740a 2020 2020 2020  rGradient.      
-000010f0: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
-00001100: 656e 7433 3335 3022 3e0a 2020 2020 2020  ent3350">.      
-00001110: 3c73 746f 700a 2020 2020 2020 2020 2073  <stop.         s
-00001120: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
-00001130: 3a23 3030 6362 3262 3b73 746f 702d 6f70  :#00cb2b;stop-op
-00001140: 6163 6974 793a 302e 3234 3739 3333 3838  acity:0.24793388
-00001150: 3b22 0a20 2020 2020 2020 2020 6f66 6673  ;".         offs
-00001160: 6574 3d22 3022 0a20 2020 2020 2020 2020  et="0".         
-00001170: 6964 3d22 7374 6f70 3333 3532 2220 2f3e  id="stop3352" />
-00001180: 0a20 2020 2020 203c 7374 6f70 0a20 2020  .      <stop.   
-00001190: 2020 2020 2020 7374 796c 653d 2273 746f        style="sto
-000011a0: 702d 636f 6c6f 723a 2330 3063 6232 623b  p-color:#00cb2b;
-000011b0: 7374 6f70 2d6f 7061 6369 7479 3a31 3b22  stop-opacity:1;"
-000011c0: 0a20 2020 2020 2020 2020 6f66 6673 6574  .         offset
-000011d0: 3d22 3122 0a20 2020 2020 2020 2020 6964  ="1".         id
-000011e0: 3d22 7374 6f70 3333 3534 2220 2f3e 0a20  ="stop3354" />. 
-000011f0: 2020 203c 2f6c 696e 6561 7247 7261 6469     </linearGradi
-00001200: 656e 743e 0a20 2020 203c 6c69 6e65 6172  ent>.    <linear
-00001210: 4772 6164 6965 6e74 0a20 2020 2020 2020  Gradient.       
-00001220: 6964 3d22 6c69 6e65 6172 4772 6164 6965  id="linearGradie
-00001230: 6e74 3333 3432 223e 0a20 2020 2020 203c  nt3342">.      <
-00001240: 7374 6f70 0a20 2020 2020 2020 2020 7374  stop.         st
-00001250: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
-00001260: 2330 3035 6138 353b 7374 6f70 2d6f 7061  #005a85;stop-opa
-00001270: 6369 7479 3a31 3b22 0a20 2020 2020 2020  city:1;".       
-00001280: 2020 6f66 6673 6574 3d22 3022 0a20 2020    offset="0".   
-00001290: 2020 2020 2020 6964 3d22 7374 6f70 3333        id="stop33
-000012a0: 3434 2220 2f3e 0a20 2020 2020 203c 7374  44" />.      <st
-000012b0: 6f70 0a20 2020 2020 2020 2020 7374 796c  op.         styl
-000012c0: 653d 2273 746f 702d 636f 6c6f 723a 2330  e="stop-color:#0
-000012d0: 3035 6138 353b 7374 6f70 2d6f 7061 6369  05a85;stop-opaci
-000012e0: 7479 3a30 2e37 3532 3036 3631 343b 220a  ty:0.75206614;".
-000012f0: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
-00001300: 2231 220a 2020 2020 2020 2020 2069 643d  "1".         id=
-00001310: 2273 746f 7033 3334 3622 202f 3e0a 2020  "stop3346" />.  
-00001320: 2020 3c2f 6c69 6e65 6172 4772 6164 6965    </linearGradie
-00001330: 6e74 3e0a 2020 2020 3c6c 696e 6561 7247  nt>.    <linearG
-00001340: 7261 6469 656e 740a 2020 2020 2020 2069  radient.       i
-00001350: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
-00001360: 7433 3331 3022 3e0a 2020 2020 2020 3c73  t3310">.      <s
-00001370: 746f 700a 2020 2020 2020 2020 2069 643d  top.         id=
-00001380: 2273 746f 7033 3331 3222 0a20 2020 2020  "stop3312".     
-00001390: 2020 2020 6f66 6673 6574 3d22 3022 0a20      offset="0". 
-000013a0: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
-000013b0: 746f 702d 636f 6c6f 723a 2361 6530 3230  top-color:#ae020
-000013c0: 323b 7374 6f70 2d6f 7061 6369 7479 3a31  2;stop-opacity:1
-000013d0: 3b22 202f 3e0a 2020 2020 2020 3c73 746f  ;" />.      <sto
-000013e0: 700a 2020 2020 2020 2020 2069 643d 2273  p.         id="s
-000013f0: 746f 7033 3331 3422 0a20 2020 2020 2020  top3314".       
-00001400: 2020 6f66 6673 6574 3d22 3122 0a20 2020    offset="1".   
-00001410: 2020 2020 2020 7374 796c 653d 2273 746f        style="sto
-00001420: 702d 636f 6c6f 723a 2362 3437 3537 353b  p-color:#b47575;
-00001430: 7374 6f70 2d6f 7061 6369 7479 3a31 3b22  stop-opacity:1;"
-00001440: 202f 3e0a 2020 2020 3c2f 6c69 6e65 6172   />.    </linear
-00001450: 4772 6164 6965 6e74 3e0a 2020 2020 3c69  Gradient>.    <i
-00001460: 6e6b 7363 6170 653a 7065 7273 7065 6374  nkscape:perspect
-00001470: 6976 650a 2020 2020 2020 2073 6f64 6970  ive.       sodip
-00001480: 6f64 693a 7479 7065 3d22 696e 6b73 6361  odi:type="inksca
-00001490: 7065 3a70 6572 7370 3364 220a 2020 2020  pe:persp3d".    
-000014a0: 2020 2069 6e6b 7363 6170 653a 7670 5f78     inkscape:vp_x
-000014b0: 3d22 3020 3a20 3539 2e39 3833 3538 3220  ="0 : 59.983582 
-000014c0: 3a20 3122 0a20 2020 2020 2020 696e 6b73  : 1".       inks
-000014d0: 6361 7065 3a76 705f 793d 2230 203a 2031  cape:vp_y="0 : 1
-000014e0: 3030 3020 3a20 3022 0a20 2020 2020 2020  000 : 0".       
-000014f0: 696e 6b73 6361 7065 3a76 705f 7a3d 2234  inkscape:vp_z="4
-00001500: 3836 2e30 3439 3939 203a 2035 392e 3938  86.04999 : 59.98
-00001510: 3335 3832 203a 2031 220a 2020 2020 2020  3582 : 1".      
-00001520: 2069 6e6b 7363 6170 653a 7065 7273 7033   inkscape:persp3
-00001530: 642d 6f72 6967 696e 3d22 3234 332e 3032  d-origin="243.02
-00001540: 3439 3920 3a20 3336 2e30 3231 3038 3320  499 : 36.021083 
-00001550: 3a20 3122 0a20 2020 2020 2020 6964 3d22  : 1".       id="
-00001560: 7065 7273 7065 6374 6976 6534 3722 202f  perspective47" /
-00001570: 3e0a 2020 2020 3c6c 696e 6561 7247 7261  >.    <linearGra
-00001580: 6469 656e 740a 2020 2020 2020 2069 643d  dient.       id=
-00001590: 226c 696e 6561 7247 7261 6469 656e 7432  "linearGradient2
-000015a0: 3739 3522 3e0a 2020 2020 2020 3c73 746f  795">.      <sto
-000015b0: 700a 2020 2020 2020 2020 2073 7479 6c65  p.         style
-000015c0: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 6238  ="stop-color:#b8
-000015d0: 6238 6238 3b73 746f 702d 6f70 6163 6974  b8b8;stop-opacit
-000015e0: 793a 302e 3439 3830 3339 3232 220a 2020  y:0.49803922".  
-000015f0: 2020 2020 2020 206f 6666 7365 743d 2230         offset="0
-00001600: 220a 2020 2020 2020 2020 2069 643d 2273  ".         id="s
-00001610: 746f 7032 3739 3722 202f 3e0a 2020 2020  top2797" />.    
-00001620: 2020 3c73 746f 700a 2020 2020 2020 2020    <stop.        
-00001630: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
-00001640: 6f72 3a23 3766 3766 3766 3b73 746f 702d  or:#7f7f7f;stop-
-00001650: 6f70 6163 6974 793a 3022 0a20 2020 2020  opacity:0".     
-00001660: 2020 2020 6f66 6673 6574 3d22 3122 0a20      offset="1". 
-00001670: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
-00001680: 3237 3939 2220 2f3e 0a20 2020 203c 2f6c  2799" />.    </l
-00001690: 696e 6561 7247 7261 6469 656e 743e 0a20  inearGradient>. 
-000016a0: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-000016b0: 6e74 0a20 2020 2020 2020 6964 3d22 6c69  nt.       id="li
-000016c0: 6e65 6172 4772 6164 6965 6e74 3237 3837  nearGradient2787
-000016d0: 223e 0a20 2020 2020 203c 7374 6f70 0a20  ">.      <stop. 
-000016e0: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
-000016f0: 746f 702d 636f 6c6f 723a 2337 6637 6637  top-color:#7f7f7
-00001700: 663b 7374 6f70 2d6f 7061 6369 7479 3a30  f;stop-opacity:0
-00001710: 2e35 220a 2020 2020 2020 2020 206f 6666  .5".         off
-00001720: 7365 743d 2230 220a 2020 2020 2020 2020  set="0".        
-00001730: 2069 643d 2273 746f 7032 3738 3922 202f   id="stop2789" /
-00001740: 3e0a 2020 2020 2020 3c73 746f 700a 2020  >.      <stop.  
-00001750: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
-00001760: 6f70 2d63 6f6c 6f72 3a23 3766 3766 3766  op-color:#7f7f7f
-00001770: 3b73 746f 702d 6f70 6163 6974 793a 3022  ;stop-opacity:0"
-00001780: 0a20 2020 2020 2020 2020 6f66 6673 6574  .         offset
-00001790: 3d22 3122 0a20 2020 2020 2020 2020 6964  ="1".         id
-000017a0: 3d22 7374 6f70 3237 3931 2220 2f3e 0a20  ="stop2791" />. 
-000017b0: 2020 203c 2f6c 696e 6561 7247 7261 6469     </linearGradi
-000017c0: 656e 743e 0a20 2020 203c 6c69 6e65 6172  ent>.    <linear
-000017d0: 4772 6164 6965 6e74 0a20 2020 2020 2020  Gradient.       
-000017e0: 6964 3d22 6c69 6e65 6172 4772 6164 6965  id="linearGradie
-000017f0: 6e74 3336 3736 223e 0a20 2020 2020 203c  nt3676">.      <
-00001800: 7374 6f70 0a20 2020 2020 2020 2020 7374  stop.         st
-00001810: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
-00001820: 2362 3262 3262 323b 7374 6f70 2d6f 7061  #b2b2b2;stop-opa
-00001830: 6369 7479 3a30 2e35 220a 2020 2020 2020  city:0.5".      
-00001840: 2020 206f 6666 7365 743d 2230 220a 2020     offset="0".  
-00001850: 2020 2020 2020 2069 643d 2273 746f 7033         id="stop3
-00001860: 3637 3822 202f 3e0a 2020 2020 2020 3c73  678" />.      <s
-00001870: 746f 700a 2020 2020 2020 2020 2073 7479  top.         sty
-00001880: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
-00001890: 6233 6233 6233 3b73 746f 702d 6f70 6163  b3b3b3;stop-opac
-000018a0: 6974 793a 3022 0a20 2020 2020 2020 2020  ity:0".         
-000018b0: 6f66 6673 6574 3d22 3122 0a20 2020 2020  offset="1".     
-000018c0: 2020 2020 6964 3d22 7374 6f70 3336 3830      id="stop3680
-000018d0: 2220 2f3e 0a20 2020 203c 2f6c 696e 6561  " />.    </linea
-000018e0: 7247 7261 6469 656e 743e 0a20 2020 203c  rGradient>.    <
-000018f0: 6c69 6e65 6172 4772 6164 6965 6e74 0a20  linearGradient. 
-00001900: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
-00001910: 4772 6164 6965 6e74 3332 3336 223e 0a20  Gradient3236">. 
-00001920: 2020 2020 203c 7374 6f70 0a20 2020 2020       <stop.     
-00001930: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
-00001940: 636f 6c6f 723a 2366 3466 3466 343b 7374  color:#f4f4f4;st
-00001950: 6f70 2d6f 7061 6369 7479 3a31 220a 2020  op-opacity:1".  
-00001960: 2020 2020 2020 206f 6666 7365 743d 2230         offset="0
-00001970: 220a 2020 2020 2020 2020 2069 643d 2273  ".         id="s
-00001980: 746f 7033 3234 3422 202f 3e0a 2020 2020  top3244" />.    
-00001990: 2020 3c73 746f 700a 2020 2020 2020 2020    <stop.        
-000019a0: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
-000019b0: 6f72 3a23 6666 6666 6666 3b73 746f 702d  or:#ffffff;stop-
-000019c0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-000019d0: 2020 2020 6f66 6673 6574 3d22 3122 0a20      offset="1". 
-000019e0: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
-000019f0: 3332 3430 2220 2f3e 0a20 2020 203c 2f6c  3240" />.    </l
-00001a00: 696e 6561 7247 7261 6469 656e 743e 0a20  inearGradient>. 
-00001a10: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-00001a20: 6e74 0a20 2020 2020 2020 6964 3d22 6c69  nt.       id="li
-00001a30: 6e65 6172 4772 6164 6965 6e74 3436 3731  nearGradient4671
-00001a40: 223e 0a20 2020 2020 203c 7374 6f70 0a20  ">.      <stop. 
-00001a50: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
-00001a60: 746f 702d 636f 6c6f 723a 2366 6664 3433  top-color:#ffd43
-00001a70: 623b 7374 6f70 2d6f 7061 6369 7479 3a31  b;stop-opacity:1
-00001a80: 220a 2020 2020 2020 2020 206f 6666 7365  ".         offse
-00001a90: 743d 2230 220a 2020 2020 2020 2020 2069  t="0".         i
-00001aa0: 643d 2273 746f 7034 3637 3322 202f 3e0a  d="stop4673" />.
-00001ab0: 2020 2020 2020 3c73 746f 700a 2020 2020        <stop.    
-00001ac0: 2020 2020 2073 7479 6c65 3d22 7374 6f70       style="stop
-00001ad0: 2d63 6f6c 6f72 3a23 6666 6538 3733 3b73  -color:#ffe873;s
-00001ae0: 746f 702d 6f70 6163 6974 793a 3122 0a20  top-opacity:1". 
-00001af0: 2020 2020 2020 2020 6f66 6673 6574 3d22          offset="
-00001b00: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
-00001b10: 7374 6f70 3436 3735 2220 2f3e 0a20 2020  stop4675" />.   
-00001b20: 203c 2f6c 696e 6561 7247 7261 6469 656e   </linearGradien
-00001b30: 743e 0a20 2020 203c 6c69 6e65 6172 4772  t>.    <linearGr
-00001b40: 6164 6965 6e74 0a20 2020 2020 2020 6964  adient.       id
-00001b50: 3d22 6c69 6e65 6172 4772 6164 6965 6e74  ="linearGradient
-00001b60: 3436 3839 223e 0a20 2020 2020 203c 7374  4689">.      <st
-00001b70: 6f70 0a20 2020 2020 2020 2020 7374 796c  op.         styl
-00001b80: 653d 2273 746f 702d 636f 6c6f 723a 2335  e="stop-color:#5
-00001b90: 6139 6664 343b 7374 6f70 2d6f 7061 6369  a9fd4;stop-opaci
-00001ba0: 7479 3a31 220a 2020 2020 2020 2020 206f  ty:1".         o
-00001bb0: 6666 7365 743d 2230 220a 2020 2020 2020  ffset="0".      
-00001bc0: 2020 2069 643d 2273 746f 7034 3639 3122     id="stop4691"
-00001bd0: 202f 3e0a 2020 2020 2020 3c73 746f 700a   />.      <stop.
-00001be0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00001bf0: 7374 6f70 2d63 6f6c 6f72 3a23 3330 3639  stop-color:#3069
-00001c00: 3938 3b73 746f 702d 6f70 6163 6974 793a  98;stop-opacity:
-00001c10: 3122 0a20 2020 2020 2020 2020 6f66 6673  1".         offs
-00001c20: 6574 3d22 3122 0a20 2020 2020 2020 2020  et="1".         
-00001c30: 6964 3d22 7374 6f70 3436 3933 2220 2f3e  id="stop4693" />
-00001c40: 0a20 2020 203c 2f6c 696e 6561 7247 7261  .    </linearGra
-00001c50: 6469 656e 743e 0a20 2020 203c 6c69 6e65  dient>.    <line
-00001c60: 6172 4772 6164 6965 6e74 0a20 2020 2020  arGradient.     
-00001c70: 2020 7831 3d22 3232 342e 3233 3939 3622    x1="224.23996"
-00001c80: 0a20 2020 2020 2020 7931 3d22 3134 342e  .       y1="144.
-00001c90: 3735 3731 3722 0a20 2020 2020 2020 7832  75717".       x2
-00001ca0: 3d22 2d36 352e 3330 3835 3032 220a 2020  ="-65.308502".  
-00001cb0: 2020 2020 2079 323d 2231 3434 2e37 3537       y2="144.757
-00001cc0: 3137 220a 2020 2020 2020 2069 643d 226c  17".       id="l
-00001cd0: 696e 6561 7247 7261 6469 656e 7432 3938  inearGradient298
-00001ce0: 3722 0a20 2020 2020 2020 786c 696e 6b3a  7".       xlink:
-00001cf0: 6872 6566 3d22 236c 696e 6561 7247 7261  href="#linearGra
-00001d00: 6469 656e 7434 3637 3122 0a20 2020 2020  dient4671".     
-00001d10: 2020 6772 6164 6965 6e74 556e 6974 733d    gradientUnits=
-00001d20: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
-00001d30: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
-00001d40: 5472 616e 7366 6f72 6d3d 2274 7261 6e73  Transform="trans
-00001d50: 6c61 7465 2831 3030 2e32 3730 322c 3939  late(100.2702,99
-00001d60: 2e36 3131 3136 2922 202f 3e0a 2020 2020  .61116)" />.    
-00001d70: 3c6c 696e 6561 7247 7261 6469 656e 740a  <linearGradient.
-00001d80: 2020 2020 2020 2078 313d 2231 3732 2e39         x1="172.9
-00001d90: 3432 3038 220a 2020 2020 2020 2079 313d  4208".       y1=
-00001da0: 2237 372e 3437 3539 3833 220a 2020 2020  "77.475983".    
-00001db0: 2020 2078 323d 2232 362e 3637 3032 3938     x2="26.670298
-00001dc0: 220a 2020 2020 2020 2079 323d 2237 362e  ".       y2="76.
-00001dd0: 3331 3331 3333 220a 2020 2020 2020 2069  313133".       i
-00001de0: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
-00001df0: 7432 3939 3022 0a20 2020 2020 2020 786c  t2990".       xl
-00001e00: 696e 6b3a 6872 6566 3d22 236c 696e 6561  ink:href="#linea
-00001e10: 7247 7261 6469 656e 7434 3638 3922 0a20  rGradient4689". 
-00001e20: 2020 2020 2020 6772 6164 6965 6e74 556e        gradientUn
-00001e30: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
-00001e40: 5573 6522 0a20 2020 2020 2020 6772 6164  Use".       grad
-00001e50: 6965 6e74 5472 616e 7366 6f72 6d3d 2274  ientTransform="t
-00001e60: 7261 6e73 6c61 7465 2831 3030 2e32 3730  ranslate(100.270
-00001e70: 322c 3939 2e36 3131 3136 2922 202f 3e0a  2,99.61116)" />.
-00001e80: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
-00001e90: 656e 740a 2020 2020 2020 2078 313d 2231  ent.       x1="1
-00001ea0: 3732 2e39 3432 3038 220a 2020 2020 2020  72.94208".      
-00001eb0: 2079 313d 2237 372e 3437 3539 3833 220a   y1="77.475983".
-00001ec0: 2020 2020 2020 2078 323d 2232 362e 3637         x2="26.67
-00001ed0: 3032 3938 220a 2020 2020 2020 2079 323d  0298".       y2=
-00001ee0: 2237 362e 3331 3331 3333 220a 2020 2020  "76.313133".    
-00001ef0: 2020 2069 643d 226c 696e 6561 7247 7261     id="linearGra
-00001f00: 6469 656e 7432 3538 3722 0a20 2020 2020  dient2587".     
-00001f10: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
-00001f20: 696e 6561 7247 7261 6469 656e 7434 3638  inearGradient468
-00001f30: 3922 0a20 2020 2020 2020 6772 6164 6965  9".       gradie
-00001f40: 6e74 556e 6974 733d 2275 7365 7253 7061  ntUnits="userSpa
-00001f50: 6365 4f6e 5573 6522 0a20 2020 2020 2020  ceOnUse".       
-00001f60: 6772 6164 6965 6e74 5472 616e 7366 6f72  gradientTransfor
-00001f70: 6d3d 2274 7261 6e73 6c61 7465 2831 3030  m="translate(100
-00001f80: 2e32 3730 322c 3939 2e36 3131 3136 2922  .2702,99.61116)"
-00001f90: 202f 3e0a 2020 2020 3c6c 696e 6561 7247   />.    <linearG
-00001fa0: 7261 6469 656e 740a 2020 2020 2020 2078  radient.       x
-00001fb0: 313d 2232 3234 2e32 3339 3936 220a 2020  1="224.23996".  
-00001fc0: 2020 2020 2079 313d 2231 3434 2e37 3537       y1="144.757
-00001fd0: 3137 220a 2020 2020 2020 2078 323d 222d  17".       x2="-
-00001fe0: 3635 2e33 3038 3530 3222 0a20 2020 2020  65.308502".     
-00001ff0: 2020 7932 3d22 3134 342e 3735 3731 3722    y2="144.75717"
-00002000: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
-00002010: 6172 4772 6164 6965 6e74 3235 3839 220a  arGradient2589".
-00002020: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
-00002030: 663d 2223 6c69 6e65 6172 4772 6164 6965  f="#linearGradie
-00002040: 6e74 3436 3731 220a 2020 2020 2020 2067  nt4671".       g
-00002050: 7261 6469 656e 7455 6e69 7473 3d22 7573  radientUnits="us
-00002060: 6572 5370 6163 654f 6e55 7365 220a 2020  erSpaceOnUse".  
-00002070: 2020 2020 2067 7261 6469 656e 7454 7261       gradientTra
-00002080: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-00002090: 6528 3130 302e 3237 3032 2c39 392e 3631  e(100.2702,99.61
-000020a0: 3131 3629 2220 2f3e 0a20 2020 203c 6c69  116)" />.    <li
-000020b0: 6e65 6172 4772 6164 6965 6e74 0a20 2020  nearGradient.   
-000020c0: 2020 2020 7831 3d22 3137 322e 3934 3230      x1="172.9420
-000020d0: 3822 0a20 2020 2020 2020 7931 3d22 3737  8".       y1="77
-000020e0: 2e34 3735 3938 3322 0a20 2020 2020 2020  .475983".       
-000020f0: 7832 3d22 3236 2e36 3730 3239 3822 0a20  x2="26.670298". 
-00002100: 2020 2020 2020 7932 3d22 3736 2e33 3133        y2="76.313
-00002110: 3133 3322 0a20 2020 2020 2020 6964 3d22  133".       id="
-00002120: 6c69 6e65 6172 4772 6164 6965 6e74 3232  linearGradient22
-00002130: 3438 220a 2020 2020 2020 2078 6c69 6e6b  48".       xlink
-00002140: 3a68 7265 663d 2223 6c69 6e65 6172 4772  :href="#linearGr
-00002150: 6164 6965 6e74 3436 3839 220a 2020 2020  adient4689".    
-00002160: 2020 2067 7261 6469 656e 7455 6e69 7473     gradientUnits
-00002170: 3d22 7573 6572 5370 6163 654f 6e55 7365  ="userSpaceOnUse
-00002180: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
-00002190: 7454 7261 6e73 666f 726d 3d22 7472 616e  tTransform="tran
-000021a0: 736c 6174 6528 3130 302e 3237 3032 2c39  slate(100.2702,9
-000021b0: 392e 3631 3131 3629 2220 2f3e 0a20 2020  9.61116)" />.   
-000021c0: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
-000021d0: 0a20 2020 2020 2020 7831 3d22 3232 342e  .       x1="224.
-000021e0: 3233 3939 3622 0a20 2020 2020 2020 7931  23996".       y1
-000021f0: 3d22 3134 342e 3735 3731 3722 0a20 2020  ="144.75717".   
-00002200: 2020 2020 7832 3d22 2d36 352e 3330 3835      x2="-65.3085
-00002210: 3032 220a 2020 2020 2020 2079 323d 2231  02".       y2="1
-00002220: 3434 2e37 3537 3137 220a 2020 2020 2020  44.75717".      
-00002230: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
-00002240: 656e 7432 3235 3022 0a20 2020 2020 2020  ent2250".       
-00002250: 786c 696e 6b3a 6872 6566 3d22 236c 696e  xlink:href="#lin
-00002260: 6561 7247 7261 6469 656e 7434 3637 3122  earGradient4671"
-00002270: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
-00002280: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
-00002290: 4f6e 5573 6522 0a20 2020 2020 2020 6772  OnUse".       gr
-000022a0: 6164 6965 6e74 5472 616e 7366 6f72 6d3d  adientTransform=
-000022b0: 2274 7261 6e73 6c61 7465 2831 3030 2e32  "translate(100.2
-000022c0: 3730 322c 3939 2e36 3131 3136 2922 202f  702,99.61116)" /
-000022d0: 3e0a 2020 2020 3c6c 696e 6561 7247 7261  >.    <linearGra
-000022e0: 6469 656e 740a 2020 2020 2020 2078 313d  dient.       x1=
-000022f0: 2232 3234 2e32 3339 3936 220a 2020 2020  "224.23996".    
-00002300: 2020 2079 313d 2231 3434 2e37 3537 3137     y1="144.75717
-00002310: 220a 2020 2020 2020 2078 323d 222d 3635  ".       x2="-65
-00002320: 2e33 3038 3530 3222 0a20 2020 2020 2020  .308502".       
-00002330: 7932 3d22 3134 342e 3735 3731 3722 0a20  y2="144.75717". 
-00002340: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
-00002350: 4772 6164 6965 6e74 3232 3535 220a 2020  Gradient2255".  
-00002360: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
-00002370: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
-00002380: 3436 3731 220a 2020 2020 2020 2067 7261  4671".       gra
-00002390: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
-000023a0: 5370 6163 654f 6e55 7365 220a 2020 2020  SpaceOnUse".    
-000023b0: 2020 2067 7261 6469 656e 7454 7261 6e73     gradientTrans
-000023c0: 666f 726d 3d22 6d61 7472 6978 2830 2e35  form="matrix(0.5
-000023d0: 3632 3534 312c 302c 302c 302e 3536 3739  62541,0,0,0.5679
-000023e0: 3732 2c2d 3131 2e35 3937 342c 2d37 2e36  72,-11.5974,-7.6
-000023f0: 3039 3534 2922 202f 3e0a 2020 2020 3c6c  0954)" />.    <l
-00002400: 696e 6561 7247 7261 6469 656e 740a 2020  inearGradient.  
-00002410: 2020 2020 2078 313d 2231 3732 2e39 3432       x1="172.942
-00002420: 3038 220a 2020 2020 2020 2079 313d 2237  08".       y1="7
-00002430: 362e 3137 3632 3234 220a 2020 2020 2020  6.176224".      
-00002440: 2078 323d 2232 362e 3637 3032 3938 220a   x2="26.670298".
-00002450: 2020 2020 2020 2079 323d 2237 362e 3331         y2="76.31
-00002460: 3331 3333 220a 2020 2020 2020 2069 643d  3133".       id=
-00002470: 226c 696e 6561 7247 7261 6469 656e 7432  "linearGradient2
-00002480: 3235 3822 0a20 2020 2020 2020 786c 696e  258".       xlin
-00002490: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
-000024a0: 7261 6469 656e 7434 3638 3922 0a20 2020  radient4689".   
-000024b0: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
-000024c0: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
-000024d0: 6522 0a20 2020 2020 2020 6772 6164 6965  e".       gradie
-000024e0: 6e74 5472 616e 7366 6f72 6d3d 226d 6174  ntTransform="mat
-000024f0: 7269 7828 302e 3536 3235 3431 2c30 2c30  rix(0.562541,0,0
-00002500: 2c30 2e35 3637 3937 322c 2d31 312e 3539  ,0.567972,-11.59
-00002510: 3734 2c2d 372e 3630 3935 3429 2220 2f3e  74,-7.60954)" />
-00002520: 0a20 2020 203c 7261 6469 616c 4772 6164  .    <radialGrad
-00002530: 6965 6e74 0a20 2020 2020 2020 6378 3d22  ient.       cx="
-00002540: 3631 2e35 3138 3838 3322 0a20 2020 2020  61.518883".     
-00002550: 2020 6379 3d22 3133 322e 3238 3537 3522    cy="132.28575"
-00002560: 0a20 2020 2020 2020 723d 2232 392e 3033  .       r="29.03
-00002570: 3639 3133 220a 2020 2020 2020 2066 783d  6913".       fx=
-00002580: 2236 312e 3531 3838 3833 220a 2020 2020  "61.518883".    
-00002590: 2020 2066 793d 2231 3332 2e32 3835 3735     fy="132.28575
-000025a0: 220a 2020 2020 2020 2069 643d 2272 6164  ".       id="rad
-000025b0: 6961 6c47 7261 6469 656e 7432 3830 3122  ialGradient2801"
-000025c0: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
-000025d0: 6566 3d22 236c 696e 6561 7247 7261 6469  ef="#linearGradi
-000025e0: 656e 7432 3739 3522 0a20 2020 2020 2020  ent2795".       
-000025f0: 6772 6164 6965 6e74 556e 6974 733d 2275  gradientUnits="u
-00002600: 7365 7253 7061 6365 4f6e 5573 6522 0a20  serSpaceOnUse". 
-00002610: 2020 2020 2020 6772 6164 6965 6e74 5472        gradientTr
-00002620: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
-00002630: 312c 302c 302c 302e 3137 3739 3636 2c30  1,0,0,0.177966,0
-00002640: 2c31 3038 2e37 3433 3429 2220 2f3e 0a20  ,108.7434)" />. 
-00002650: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-00002660: 6e74 0a20 2020 2020 2020 7831 3d22 3135  nt.       x1="15
-00002670: 302e 3936 3131 3122 0a20 2020 2020 2020  0.96111".       
-00002680: 7931 3d22 3139 322e 3335 3137 3622 0a20  y1="192.35176". 
-00002690: 2020 2020 2020 7832 3d22 3131 322e 3033        x2="112.03
-000026a0: 3134 3422 0a20 2020 2020 2020 7932 3d22  144".       y2="
-000026b0: 3133 372e 3237 3239 3922 0a20 2020 2020  137.27299".     
-000026c0: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
-000026d0: 6965 6e74 3134 3735 220a 2020 2020 2020  ient1475".      
-000026e0: 2078 6c69 6e6b 3a68 7265 663d 2223 6c69   xlink:href="#li
-000026f0: 6e65 6172 4772 6164 6965 6e74 3436 3731  nearGradient4671
-00002700: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
-00002710: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
-00002720: 654f 6e55 7365 220a 2020 2020 2020 2067  eOnUse".       g
-00002730: 7261 6469 656e 7454 7261 6e73 666f 726d  radientTransform
-00002740: 3d22 6d61 7472 6978 2830 2e35 3632 3534  ="matrix(0.56254
-00002750: 312c 302c 302c 302e 3536 3739 3732 2c2d  1,0,0,0.567972,-
-00002760: 392e 3339 3937 3439 2c2d 352e 3330 3533  9.399749,-5.3053
-00002770: 3137 2922 202f 3e0a 2020 2020 3c6c 696e  17)" />.    <lin
-00002780: 6561 7247 7261 6469 656e 740a 2020 2020  earGradient.    
-00002790: 2020 2078 313d 2232 362e 3634 3839 3337     x1="26.648937
-000027a0: 220a 2020 2020 2020 2079 313d 2232 302e  ".       y1="20.
-000027b0: 3630 3337 3831 220a 2020 2020 2020 2078  603781".       x
-000027c0: 323d 2231 3335 2e36 3635 3235 220a 2020  2="135.66525".  
-000027d0: 2020 2020 2079 323d 2231 3134 2e33 3937       y2="114.397
-000027e0: 3637 220a 2020 2020 2020 2069 643d 226c  67".       id="l
-000027f0: 696e 6561 7247 7261 6469 656e 7431 3437  inearGradient147
-00002800: 3822 0a20 2020 2020 2020 786c 696e 6b3a  8".       xlink:
-00002810: 6872 6566 3d22 236c 696e 6561 7247 7261  href="#linearGra
-00002820: 6469 656e 7434 3638 3922 0a20 2020 2020  dient4689".     
-00002830: 2020 6772 6164 6965 6e74 556e 6974 733d    gradientUnits=
-00002840: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
-00002850: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
-00002860: 5472 616e 7366 6f72 6d3d 226d 6174 7269  Transform="matri
-00002870: 7828 302e 3536 3235 3431 2c30 2c30 2c30  x(0.562541,0,0,0
-00002880: 2e35 3637 3937 322c 2d39 2e33 3939 3734  .567972,-9.39974
-00002890: 392c 2d35 2e33 3035 3331 3729 2220 2f3e  9,-5.305317)" />
-000028a0: 0a20 2020 203c 7261 6469 616c 4772 6164  .    <radialGrad
-000028b0: 6965 6e74 0a20 2020 2020 2020 6378 3d22  ient.       cx="
-000028c0: 3631 2e35 3138 3838 3322 0a20 2020 2020  61.518883".     
-000028d0: 2020 6379 3d22 3133 322e 3238 3537 3522    cy="132.28575"
-000028e0: 0a20 2020 2020 2020 723d 2232 392e 3033  .       r="29.03
-000028f0: 3639 3133 220a 2020 2020 2020 2066 783d  6913".       fx=
-00002900: 2236 312e 3531 3838 3833 220a 2020 2020  "61.518883".    
-00002910: 2020 2066 793d 2231 3332 2e32 3835 3735     fy="132.28575
-00002920: 220a 2020 2020 2020 2069 643d 2272 6164  ".       id="rad
-00002930: 6961 6c47 7261 6469 656e 7431 3438 3022  ialGradient1480"
-00002940: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
-00002950: 6566 3d22 236c 696e 6561 7247 7261 6469  ef="#linearGradi
-00002960: 656e 7432 3739 3522 0a20 2020 2020 2020  ent2795".       
-00002970: 6772 6164 6965 6e74 556e 6974 733d 2275  gradientUnits="u
-00002980: 7365 7253 7061 6365 4f6e 5573 6522 0a20  serSpaceOnUse". 
-00002990: 2020 2020 2020 6772 6164 6965 6e74 5472        gradientTr
-000029a0: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
-000029b0: 322e 3338 3237 3136 652d 382c 2d30 2e32  2.382716e-8,-0.2
-000029c0: 3936 3430 352c 312e 3433 3637 362c 342e  96405,1.43676,4.
-000029d0: 3638 3336 3733 652d 372c 2d31 3238 2e35  683673e-7,-128.5
-000029e0: 3434 2c31 3530 2e35 3230 3229 2220 2f3e  44,150.5202)" />
-000029f0: 0a20 2020 203c 7261 6469 616c 4772 6164  .    <radialGrad
-00002a00: 6965 6e74 0a20 2020 2020 2020 696e 6b73  ient.       inks
-00002a10: 6361 7065 3a63 6f6c 6c65 6374 3d22 616c  cape:collect="al
-00002a20: 7761 7973 220a 2020 2020 2020 2078 6c69  ways".       xli
-00002a30: 6e6b 3a68 7265 663d 2223 6c69 6e65 6172  nk:href="#linear
-00002a40: 4772 6164 6965 6e74 3237 3935 220a 2020  Gradient2795".  
-00002a50: 2020 2020 2069 643d 2272 6164 6961 6c47       id="radialG
-00002a60: 7261 6469 656e 7432 3432 3122 0a20 2020  radient2421".   
-00002a70: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
-00002a80: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
-00002a90: 6522 0a20 2020 2020 2020 6772 6164 6965  e".       gradie
-00002aa0: 6e74 5472 616e 7366 6f72 6d3d 226d 6174  ntTransform="mat
-00002ab0: 7269 7828 312e 3734 3930 3536 3565 2d38  rix(1.7490565e-8
-00002ac0: 2c2d 302e 3233 3939 3437 2c31 2e30 3534  ,-0.239947,1.054
-00002ad0: 3636 382c 332e 3739 3135 3435 3765 2d37  668,3.7915457e-7
-00002ae0: 2c2d 3738 2e31 3039 3432 392c 3134 382e  ,-78.109429,148.
-00002af0: 3835 3930 3629 220a 2020 2020 2020 2063  85906)".       c
-00002b00: 783d 2236 312e 3531 3838 3833 220a 2020  x="61.518883".  
-00002b10: 2020 2020 2063 793d 2231 3332 2e32 3835       cy="132.285
-00002b20: 3735 220a 2020 2020 2020 2066 783d 2236  75".       fx="6
-00002b30: 312e 3531 3838 3833 220a 2020 2020 2020  1.518883".      
-00002b40: 2066 793d 2231 3332 2e32 3835 3735 220a   fy="132.28575".
-00002b50: 2020 2020 2020 2072 3d22 3239 2e30 3336         r="29.036
-00002b60: 3931 3322 202f 3e0a 2020 2020 3c6c 696e  913" />.    <lin
-00002b70: 6561 7247 7261 6469 656e 740a 2020 2020  earGradient.    
-00002b80: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
-00002b90: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
-00002ba0: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
-00002bb0: 236c 696e 6561 7247 7261 6469 656e 7434  #linearGradient4
-00002bc0: 3637 312d 3822 0a20 2020 2020 2020 6964  671-8".       id
-00002bd0: 3d22 6c69 6e65 6172 4772 6164 6965 6e74  ="linearGradient
-00002be0: 3338 3236 2d36 220a 2020 2020 2020 2078  3826-6".       x
-00002bf0: 313d 2233 362e 3937 3038 3938 220a 2020  1="36.970898".  
-00002c00: 2020 2020 2079 313d 2235 342e 3634 3637       y1="54.6467
-00002c10: 3633 220a 2020 2020 2020 2078 323d 2238  63".       x2="8
-00002c20: 372e 3730 3436 3831 220a 2020 2020 2020  7.704681".      
-00002c30: 2079 323d 2235 342e 3634 3637 3633 220a   y2="54.646763".
-00002c40: 2020 2020 2020 2067 7261 6469 656e 7455         gradientU
-00002c50: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00002c60: 6e55 7365 2220 2f3e 0a20 2020 203c 6c69  nUse" />.    <li
-00002c70: 6e65 6172 4772 6164 6965 6e74 0a20 2020  nearGradient.   
-00002c80: 2020 2020 6964 3d22 6c69 6e65 6172 4772      id="linearGr
-00002c90: 6164 6965 6e74 3436 3731 2d38 223e 0a20  adient4671-8">. 
-00002ca0: 2020 2020 203c 7374 6f70 0a20 2020 2020       <stop.     
-00002cb0: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
-00002cc0: 636f 6c6f 723a 2366 6664 3433 623b 7374  color:#ffd43b;st
-00002cd0: 6f70 2d6f 7061 6369 7479 3a31 220a 2020  op-opacity:1".  
-00002ce0: 2020 2020 2020 206f 6666 7365 743d 2230         offset="0
-00002cf0: 220a 2020 2020 2020 2020 2069 643d 2273  ".         id="s
-00002d00: 746f 7034 3637 332d 3822 202f 3e0a 2020  top4673-8" />.  
-00002d10: 2020 2020 3c73 746f 700a 2020 2020 2020      <stop.      
-00002d20: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
-00002d30: 6f6c 6f72 3a23 6666 6538 3733 3b73 746f  olor:#ffe873;sto
-00002d40: 702d 6f70 6163 6974 793a 3122 0a20 2020  p-opacity:1".   
-00002d50: 2020 2020 2020 6f66 6673 6574 3d22 3122        offset="1"
-00002d60: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
-00002d70: 6f70 3436 3735 2d32 2220 2f3e 0a20 2020  op4675-2" />.   
-00002d80: 203c 2f6c 696e 6561 7247 7261 6469 656e   </linearGradien
-00002d90: 743e 0a20 2020 203c 6c69 6e65 6172 4772  t>.    <linearGr
-00002da0: 6164 6965 6e74 0a20 2020 2020 2020 696e  adient.       in
-00002db0: 6b73 6361 7065 3a63 6f6c 6c65 6374 3d22  kscape:collect="
-00002dc0: 616c 7761 7973 220a 2020 2020 2020 2078  always".       x
-00002dd0: 6c69 6e6b 3a68 7265 663d 2223 6c69 6e65  link:href="#line
-00002de0: 6172 4772 6164 6965 6e74 3338 3132 220a  arGradient3812".
-00002df0: 2020 2020 2020 2069 643d 226c 696e 6561         id="linea
-00002e00: 7247 7261 6469 656e 7433 3831 3822 0a20  rGradient3818". 
-00002e10: 2020 2020 2020 7831 3d22 3738 2e30 3132        x1="78.012
-00002e20: 3032 3422 0a20 2020 2020 2020 7931 3d22  024".       y1="
-00002e30: 3830 2e33 3032 3933 3322 0a20 2020 2020  80.302933".     
-00002e40: 2020 7832 3d22 3132 342e 3637 3936 3422    x2="124.67964"
-00002e50: 0a20 2020 2020 2020 7932 3d22 3238 2e36  .       y2="28.6
-00002e60: 3033 3332 3722 0a20 2020 2020 2020 6772  03327".       gr
-00002e70: 6164 6965 6e74 556e 6974 733d 2275 7365  adientUnits="use
-00002e80: 7253 7061 6365 4f6e 5573 6522 202f 3e0a  rSpaceOnUse" />.
-00002e90: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
-00002ea0: 656e 740a 2020 2020 2020 2069 6e6b 7363  ent.       inksc
-00002eb0: 6170 653a 636f 6c6c 6563 743d 2261 6c77  ape:collect="alw
-00002ec0: 6179 7322 0a20 2020 2020 2020 786c 696e  ays".       xlin
-00002ed0: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
-00002ee0: 7261 6469 656e 7433 3831 3222 0a20 2020  radient3812".   
-00002ef0: 2020 2020 6964 3d22 6c69 6e65 6172 4772      id="linearGr
-00002f00: 6164 6965 6e74 3430 3937 220a 2020 2020  adient4097".    
-00002f10: 2020 2078 313d 222d 3230 352e 3035 3433     x1="-205.0543
-00002f20: 3122 0a20 2020 2020 2020 7931 3d22 3535  1".       y1="55
-00002f30: 2e36 3036 3434 3122 0a20 2020 2020 2020  .606441".       
-00002f40: 7832 3d22 2d36 342e 3830 3632 3539 220a  x2="-64.806259".
-00002f50: 2020 2020 2020 2079 323d 2235 352e 3630         y2="55.60
-00002f60: 3634 3431 220a 2020 2020 2020 2067 7261  6441".       gra
-00002f70: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
-00002f80: 5370 6163 654f 6e55 7365 220a 2020 2020  SpaceOnUse".    
-00002f90: 2020 2067 7261 6469 656e 7454 7261 6e73     gradientTrans
-00002fa0: 666f 726d 3d22 6d61 7472 6978 2831 2e30  form="matrix(1.0
-00002fb0: 3935 3135 3339 2c30 2c30 2c31 2e30 3331  951539,0,0,1.031
-00002fc0: 3532 3638 2c32 3234 2e30 3138 3435 2c2d  5268,224.01845,-
-00002fd0: 332e 3636 3230 3331 2922 202f 3e0a 2020  3.662031)" />.  
-00002fe0: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
-00002ff0: 740a 2020 2020 2020 2069 6e6b 7363 6170  t.       inkscap
-00003000: 653a 636f 6c6c 6563 743d 2261 6c77 6179  e:collect="alway
-00003010: 7322 0a20 2020 2020 2020 786c 696e 6b3a  s".       xlink:
-00003020: 6872 6566 3d22 236c 696e 6561 7247 7261  href="#linearGra
-00003030: 6469 656e 7431 3839 3422 0a20 2020 2020  dient1894".     
-00003040: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
-00003050: 6965 6e74 3430 3937 2d34 220a 2020 2020  ient4097-4".    
-00003060: 2020 2078 313d 222d 3230 352e 3035 3433     x1="-205.0543
-00003070: 3122 0a20 2020 2020 2020 7931 3d22 3535  1".       y1="55
-00003080: 2e36 3036 3434 3122 0a20 2020 2020 2020  .606441".       
-00003090: 7832 3d22 2d36 342e 3830 3632 3539 220a  x2="-64.806259".
-000030a0: 2020 2020 2020 2079 323d 2235 352e 3630         y2="55.60
-000030b0: 3634 3431 220a 2020 2020 2020 2067 7261  6441".       gra
-000030c0: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
-000030d0: 5370 6163 654f 6e55 7365 220a 2020 2020  SpaceOnUse".    
-000030e0: 2020 2067 7261 6469 656e 7454 7261 6e73     gradientTrans
-000030f0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00003100: 3231 322e 3435 3336 342c 2d32 2e36 3936  212.45364,-2.696
-00003110: 3837 3629 2220 2f3e 0a20 2020 203c 6c69  876)" />.    <li
-00003120: 6e65 6172 4772 6164 6965 6e74 0a20 2020  nearGradient.   
-00003130: 2020 2020 6964 3d22 6c69 6e65 6172 4772      id="linearGr
-00003140: 6164 6965 6e74 3138 3934 223e 0a20 2020  adient1894">.   
-00003150: 2020 203c 7374 6f70 0a20 2020 2020 2020     <stop.       
-00003160: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
-00003170: 6c6f 723a 2366 6666 3363 653b 7374 6f70  lor:#fff3ce;stop
-00003180: 2d6f 7061 6369 7479 3a31 3b22 0a20 2020  -opacity:1;".   
-00003190: 2020 2020 2020 6f66 6673 6574 3d22 3022        offset="0"
-000031a0: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
-000031b0: 6f70 3138 3930 2220 2f3e 0a20 2020 2020  op1890" />.     
-000031c0: 203c 7374 6f70 0a20 2020 2020 2020 2020   <stop.         
-000031d0: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
-000031e0: 723a 2366 6665 3837 333b 7374 6f70 2d6f  r:#ffe873;stop-o
-000031f0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00003200: 2020 206f 6666 7365 743d 2231 220a 2020     offset="1".  
-00003210: 2020 2020 2020 2069 643d 2273 746f 7031         id="stop1
-00003220: 3839 3222 202f 3e0a 2020 2020 3c2f 6c69  892" />.    </li
-00003230: 6e65 6172 4772 6164 6965 6e74 3e0a 2020  nearGradient>.  
-00003240: 3c2f 6465 6673 3e0a 2020 3c65 6c6c 6970  </defs>.  <ellip
-00003250: 7365 0a20 2020 2020 7374 796c 653d 2266  se.     style="f
-00003260: 696c 6c3a 7572 6c28 236c 696e 6561 7247  ill:url(#linearG
-00003270: 7261 6469 656e 7434 3039 3729 3b66 696c  radient4097);fil
-00003280: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00003290: 6b65 3a6e 6f6e 653b 7374 726f 6b65 2d77  ke:none;stroke-w
-000032a0: 6964 7468 3a31 2e30 3632 3836 3b73 7472  idth:1.06286;str
-000032b0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-000032c0: 2020 2020 6964 3d22 7061 7468 3430 3839      id="path4089
-000032d0: 220a 2020 2020 2063 783d 2237 362e 3234  ".     cx="76.24
-000032e0: 3930 3233 220a 2020 2020 2063 793d 2235  9023".     cy="5
-000032f0: 332e 3639 3735 3036 220a 2020 2020 2072  3.697506".     r
-00003300: 783d 2237 362e 3234 3930 3233 220a 2020  x="76.249023".  
-00003310: 2020 2072 793d 2235 332e 3136 3833 3639     ry="53.168369
-00003320: 2220 2f3e 0a20 203c 656c 6c69 7073 650a  " />.  <ellipse.
-00003330: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00003340: 3a75 726c 2823 6c69 6e65 6172 4772 6164  :url(#linearGrad
-00003350: 6965 6e74 3430 3937 2d34 293b 6669 6c6c  ient4097-4);fill
-00003360: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00003370: 653a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  e:none;stroke-op
-00003380: 6163 6974 793a 3122 0a20 2020 2020 6964  acity:1".     id
-00003390: 3d22 7061 7468 3430 3839 2d32 220a 2020  ="path4089-2".  
-000033a0: 2020 2063 783d 2237 372e 3532 3333 3534     cx="77.523354
-000033b0: 220a 2020 2020 2063 793d 2235 322e 3930  ".     cy="52.90
-000033c0: 3935 3631 220a 2020 2020 2072 783d 2236  9561".     rx="6
-000033d0: 392e 3632 3430 3233 220a 2020 2020 2072  9.624023".     r
-000033e0: 793d 2235 312e 3534 3333 3639 2220 2f3e  y="51.543369" />
-000033f0: 0a20 203c 7061 7468 0a20 2020 2020 7374  .  <path.     st
-00003400: 796c 653d 2263 6f6c 6f72 3a23 3030 3030  yle="color:#0000
-00003410: 3030 3b66 6f6e 742d 7374 796c 653a 6e6f  00;font-style:no
-00003420: 726d 616c 3b66 6f6e 742d 7661 7269 616e  rmal;font-varian
-00003430: 743a 6e6f 726d 616c 3b66 6f6e 742d 7765  t:normal;font-we
-00003440: 6967 6874 3a6e 6f72 6d61 6c3b 666f 6e74  ight:normal;font
-00003450: 2d73 7472 6574 6368 3a6e 6f72 6d61 6c3b  -stretch:normal;
-00003460: 666f 6e74 2d73 697a 653a 6d65 6469 756d  font-size:medium
-00003470: 3b6c 696e 652d 6865 6967 6874 3a6e 6f72  ;line-height:nor
-00003480: 6d61 6c3b 666f 6e74 2d66 616d 696c 793a  mal;font-family:
-00003490: 5361 6e73 3b2d 696e 6b73 6361 7065 2d66  Sans;-inkscape-f
-000034a0: 6f6e 742d 7370 6563 6966 6963 6174 696f  ont-specificatio
-000034b0: 6e3a 5361 6e73 3b74 6578 742d 696e 6465  n:Sans;text-inde
-000034c0: 6e74 3a30 3b74 6578 742d 616c 6967 6e3a  nt:0;text-align:
-000034d0: 7374 6172 743b 7465 7874 2d64 6563 6f72  start;text-decor
-000034e0: 6174 696f 6e3a 6e6f 6e65 3b74 6578 742d  ation:none;text-
-000034f0: 6465 636f 7261 7469 6f6e 2d6c 696e 653a  decoration-line:
-00003500: 6e6f 6e65 3b6c 6574 7465 722d 7370 6163  none;letter-spac
-00003510: 696e 673a 6e6f 726d 616c 3b77 6f72 642d  ing:normal;word-
-00003520: 7370 6163 696e 673a 6e6f 726d 616c 3b74  spacing:normal;t
-00003530: 6578 742d 7472 616e 7366 6f72 6d3a 6e6f  ext-transform:no
-00003540: 6e65 3b77 7269 7469 6e67 2d6d 6f64 653a  ne;writing-mode:
-00003550: 6c72 2d74 623b 6469 7265 6374 696f 6e3a  lr-tb;direction:
-00003560: 6c74 723b 6261 7365 6c69 6e65 2d73 6869  ltr;baseline-shi
-00003570: 6674 3a62 6173 656c 696e 653b 7465 7874  ft:baseline;text
-00003580: 2d61 6e63 686f 723a 7374 6172 743b 6469  -anchor:start;di
-00003590: 7370 6c61 793a 696e 6c69 6e65 3b6f 7665  splay:inline;ove
-000035a0: 7266 6c6f 773a 7669 7369 626c 653b 7669  rflow:visible;vi
-000035b0: 7369 6269 6c69 7479 3a76 6973 6962 6c65  sibility:visible
-000035c0: 3b66 696c 6c3a 2362 6262 6262 623b 6669  ;fill:#bbbbbb;fi
-000035d0: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
-000035e0: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
-000035f0: 7472 6f6b 653a 6e6f 6e65 3b73 7472 6f6b  troke:none;strok
-00003600: 652d 7769 6474 683a 392e 3538 3436 323b  e-width:9.58462;
-00003610: 6d61 726b 6572 3a6e 6f6e 653b 656e 6162  marker:none;enab
-00003620: 6c65 2d62 6163 6b67 726f 756e 643a 6163  le-background:ac
-00003630: 6375 6d75 6c61 7465 220a 2020 2020 2064  cumulate".     d
-00003640: 3d22 4d20 3737 2e38 3330 3139 372c 3020  ="M 77.830197,0 
-00003650: 4320 3232 2e35 3639 3635 312c 3020 302e  C 22.569651,0 0.
-00003660: 3431 3634 3830 3834 2c32 302e 3036 3632  41648084,20.0662
-00003670: 3436 2030 2e34 3136 3438 3038 342c 3533  46 0.41648084,53
-00003680: 2e32 3132 3033 3520 312e 3230 3538 3630  .212035 1.205860
-00003690: 382c 3830 2e34 3439 3039 2032 352e 3139  8,80.44909 25.19
-000036a0: 3539 3431 2c31 3030 2e39 3036 3220 3437  5941,100.9062 47
-000036b0: 2e33 3434 3737 312c 3130 382e 3731 3230  .344771,108.7120
-000036c0: 3820 6320 392e 3139 3936 322c 332e 3035  8 c 9.19962,3.05
-000036d0: 3932 3620 3335 2e37 3736 3037 352c 3332  926 35.776075,32
-000036e0: 2e39 3439 3833 2034 362e 3430 3337 3133  .94983 46.403713
-000036f0: 2c33 322e 3934 3938 3320 352e 3331 3338  ,32.94983 5.3138
-00003700: 3232 2c30 202d 3139 2e32 3039 3335 332c  22,0 -19.209353,
-00003710: 2d32 302e 3232 3835 3120 2d31 332e 3232  -20.22851 -13.22
-00003720: 3237 3832 2c2d 3234 2e36 3739 3335 2035  2782,-24.67935 5
-00003730: 2e34 3435 3235 322c 2d34 2e30 3438 3338  .445252,-4.04838
-00003740: 2031 332e 3035 3230 3037 2c2d 342e 3031   13.052007,-4.01
-00003750: 3830 3320 3238 2e32 3135 3637 382c 2d31  803 28.215678,-1
-00003760: 302e 3737 3034 3820 3135 2e31 3633 3637  0.77048 15.16367
-00003770: 2c2d 362e 3735 3234 3533 2034 352e 3138  ,-6.752453 45.18
-00003780: 3236 352c 2d32 352e 3233 3232 3031 2034  265,-25.232201 4
-00003790: 352e 3435 3633 352c 2d35 332e 3030 3030  5.45635,-53.0000
-000037a0: 3435 2043 2031 3534 2e31 3937 3733 2c32  45 C 154.19773,2
-000037b0: 302e 3036 3632 3436 2031 3333 2e30 3930  0.066246 133.090
-000037c0: 3735 2c30 2037 372e 3833 3031 3937 2c30  75,0 77.830197,0
-000037d0: 205a 206d 2031 2e30 3339 3732 312c 392e   Z m 1.039721,9.
-000037e0: 3838 3132 3030 3420 4320 3132 342e 3839  8812004 C 124.89
-000037f0: 3835 382c 3130 2e31 3331 3220 3134 332e  858,10.1312 143.
-00003800: 3938 3939 382c 3234 2e30 3639 3330 3120  98998,24.069301 
-00003810: 3134 332e 3938 3939 382c 3533 2e32 3132  143.98998,53.212
-00003820: 3033 3520 3134 322e 3934 3830 342c 3836  035 142.94804,86
-00003830: 2e32 3635 3632 3320 3130 372e 3939 3337  .265623 107.9937
-00003840: 352c 3130 302e 3530 3031 2037 372e 3534  5,100.5001 77.54
-00003850: 3034 3736 2c31 3030 2e37 3534 3932 2034  0476,100.75492 4
-00003860: 372e 3038 3732 3031 2c31 3031 2e30 3039  7.087201,101.009
-00003870: 3734 2031 302e 3632 3432 3331 2c38 322e  74 10.624231,82.
-00003880: 3335 3437 3732 2031 302e 3632 3432 3331  354772 10.624231
-00003890: 2c35 332e 3231 3230 3335 2063 2030 2c2d  ,53.212035 c 0,-
-000038a0: 3239 2e31 3432 3733 3620 3232 2e32 3137  29.142736 22.217
-000038b0: 3033 2c2d 3433 2e35 3830 3833 3436 2036  03,-43.5808346 6
-000038c0: 382e 3234 3536 3837 2c2d 3433 2e33 3330  8.245687,-43.330
-000038d0: 3833 3436 207a 220a 2020 2020 2069 643d  8346 z".     id=
-000038e0: 2270 6174 6833 3033 3222 0a20 2020 2020  "path3032".     
-000038f0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-00003900: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-00003910: 0a20 2020 2020 736f 6469 706f 6469 3a6e  .     sodipodi:n
-00003920: 6f64 6574 7970 6573 3d22 7a63 6373 737a  odetypes="zccssz
-00003930: 637a 7a63 7a7a 7a22 202f 3e0a 2020 3c74  czzczzz" />.  <t
-00003940: 6578 740a 2020 2020 2078 6d6c 3a73 7061  ext.     xml:spa
-00003950: 6365 3d22 7072 6573 6572 7665 220a 2020  ce="preserve".  
-00003960: 2020 2073 7479 6c65 3d22 666f 6e74 2d73     style="font-s
-00003970: 7479 6c65 3a69 7461 6c69 633b 666f 6e74  tyle:italic;font
-00003980: 2d77 6569 6768 743a 626f 6c64 3b66 6f6e  -weight:bold;fon
-00003990: 742d 7369 7a65 3a31 3036 2e36 3637 7078  t-size:106.667px
-000039a0: 3b6c 696e 652d 6865 6967 6874 3a31 2e35  ;line-height:1.5
-000039b0: 3b66 6f6e 742d 6661 6d69 6c79 3a27 4365  ;font-family:'Ce
-000039c0: 6e74 7572 7920 476f 7468 6963 273b 2d69  ntury Gothic';-i
-000039d0: 6e6b 7363 6170 652d 666f 6e74 2d73 7065  nkscape-font-spe
-000039e0: 6369 6669 6361 7469 6f6e 3a27 4365 6e74  cification:'Cent
-000039f0: 7572 7920 476f 7468 6963 2042 6f6c 6420  ury Gothic Bold 
-00003a00: 4974 616c 6963 273b 6c65 7474 6572 2d73  Italic';letter-s
-00003a10: 7061 6369 6e67 3a2d 342e 3734 7078 3b66  pacing:-4.74px;f
-00003a20: 696c 6c3a 2338 3038 3038 303b 7374 726f  ill:#808080;stro
-00003a30: 6b65 2d77 6964 7468 3a31 332e 3430 3322  ke-width:13.403"
-00003a40: 0a20 2020 2020 783d 2231 3539 2e32 3638  .     x="159.268
-00003a50: 3833 220a 2020 2020 2079 3d22 3930 2e38  83".     y="90.8
-00003a60: 3235 3437 3822 0a20 2020 2020 6964 3d22  25478".     id="
-00003a70: 7465 7874 3338 3022 3e3c 7473 7061 6e0a  text380"><tspan.
-00003a80: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-00003a90: 726f 6c65 3d22 6c69 6e65 220a 2020 2020  role="line".    
-00003aa0: 2020 2069 643d 2274 7370 616e 3337 3822     id="tspan378"
-00003ab0: 0a20 2020 2020 2020 783d 2231 3539 2e32  .       x="159.2
-00003ac0: 3638 3833 220a 2020 2020 2020 2079 3d22  6883".       y="
-00003ad0: 3930 2e38 3235 3437 3822 0a20 2020 2020  90.825478".     
-00003ae0: 2020 7374 796c 653d 2266 6f6e 742d 7374    style="font-st
-00003af0: 796c 653a 6e6f 726d 616c 3b66 6f6e 742d  yle:normal;font-
-00003b00: 7661 7269 616e 743a 6e6f 726d 616c 3b66  variant:normal;f
-00003b10: 6f6e 742d 7765 6967 6874 3a33 3030 3b66  ont-weight:300;f
-00003b20: 6f6e 742d 7374 7265 7463 683a 6e6f 726d  ont-stretch:norm
-00003b30: 616c 3b66 6f6e 742d 7369 7a65 3a31 3036  al;font-size:106
-00003b40: 2e36 3637 7078 3b66 6f6e 742d 6661 6d69  .667px;font-fami
-00003b50: 6c79 3a43 6f72 6265 6c3b 2d69 6e6b 7363  ly:Corbel;-inksc
-00003b60: 6170 652d 666f 6e74 2d73 7065 6369 6669  ape-font-specifi
-00003b70: 6361 7469 6f6e 3a27 436f 7262 656c 204c  cation:'Corbel L
-00003b80: 6967 6874 273b 6669 6c6c 3a23 3830 3830  ight';fill:#8080
-00003b90: 3830 223e 6775 6964 6174 613c 2f74 7370  80">guidata</tsp
-00003ba0: 616e 3e3c 2f74 6578 743e 0a20 203c 670a  an></text>.  <g.
-00003bb0: 2020 2020 2069 643d 2267 3222 0a20 2020       id="g2".   
-00003bc0: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
-00003bd0: 6e73 6c61 7465 282d 312e 3739 3634 3231  nslate(-1.796421
-00003be0: 312c 2d38 2e31 3639 3437 3536 2922 3e0a  1,-8.1694756)">.
-00003bf0: 2020 2020 3c72 6563 740a 2020 2020 2020      <rect.      
-00003c00: 2073 7479 6c65 3d22 6669 6c6c 3a23 6666   style="fill:#ff
-00003c10: 6666 6666 3b66 696c 6c2d 6f70 6163 6974  ffff;fill-opacit
-00003c20: 793a 313b 7374 726f 6b65 3a23 6263 6263  y:1;stroke:#bcbc
-00003c30: 6263 3b73 7472 6f6b 652d 7769 6474 683a  bc;stroke-width:
-00003c40: 362e 333b 7374 726f 6b65 2d64 6173 6861  6.3;stroke-dasha
-00003c50: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00003c60: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00003c70: 2020 2069 643d 2272 6563 7431 220a 2020     id="rect1".  
-00003c80: 2020 2020 2077 6964 7468 3d22 3939 2e32       width="99.2
-00003c90: 3432 3537 3722 0a20 2020 2020 2020 6865  42577".       he
-00003ca0: 6967 6874 3d22 3538 2e35 3530 3536 3422  ight="58.550564"
-00003cb0: 0a20 2020 2020 2020 783d 2232 392e 3639  .       x="29.69
-00003cc0: 3834 3836 220a 2020 2020 2020 2079 3d22  8486".       y="
-00003cd0: 3331 2e38 3033 3735 3522 0a20 2020 2020  31.803755".     
-00003ce0: 2020 7279 3d22 362e 3535 3331 3932 3122    ry="6.5531921"
-00003cf0: 202f 3e0a 2020 2020 3c72 6563 740a 2020   />.    <rect.  
-00003d00: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00003d10: 3a23 6263 6263 6263 3b66 696c 6c2d 6f70  :#bcbcbc;fill-op
-00003d20: 6163 6974 793a 313b 7374 726f 6b65 3a6e  acity:1;stroke:n
-00003d30: 6f6e 653b 7374 726f 6b65 2d77 6964 7468  one;stroke-width
-00003d40: 3a31 2e36 3130 3538 3b73 7472 6f6b 652d  :1.61058;stroke-
-00003d50: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00003d60: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00003d70: 0a20 2020 2020 2020 6964 3d22 7265 6374  .       id="rect
-00003d80: 312d 3122 0a20 2020 2020 2020 7769 6474  1-1".       widt
-00003d90: 683d 2237 2e38 3630 3835 3138 220a 2020  h="7.8608518".  
-00003da0: 2020 2020 2068 6569 6768 743d 2234 382e       height="48.
-00003db0: 3331 3036 3639 220a 2020 2020 2020 2078  310669".       x
-00003dc0: 3d22 3933 2e38 3336 3632 3422 0a20 2020  ="93.836624".   
-00003dd0: 2020 2020 793d 2233 362e 3937 3136 3131      y="36.971611
-00003de0: 220a 2020 2020 2020 2072 793d 2235 2e34  ".       ry="5.4
-00003df0: 3037 3130 3539 2220 2f3e 0a20 2020 203c  071059" />.    <
-00003e00: 7465 7874 0a20 2020 2020 2020 786d 6c3a  text.       xml:
-00003e10: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
-00003e20: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00003e30: 6f6e 742d 7765 6967 6874 3a62 6f6c 643b  ont-weight:bold;
-00003e40: 666f 6e74 2d73 697a 653a 3534 2e33 3237  font-size:54.327
-00003e50: 3170 783b 6c69 6e65 2d68 6569 6768 743a  1px;line-height:
-00003e60: 313b 666f 6e74 2d66 616d 696c 793a 436f  1;font-family:Co
-00003e70: 7262 656c 3b2d 696e 6b73 6361 7065 2d66  rbel;-inkscape-f
-00003e80: 6f6e 742d 7370 6563 6966 6963 6174 696f  ont-specificatio
-00003e90: 6e3a 2743 6f72 6265 6c20 426f 6c64 273b  n:'Corbel Bold';
-00003ea0: 7465 7874 2d61 6c69 676e 3a63 656e 7465  text-align:cente
-00003eb0: 723b 6c65 7474 6572 2d73 7061 6369 6e67  r;letter-spacing
-00003ec0: 3a2d 352e 3338 3037 3870 783b 7465 7874  :-5.38078px;text
-00003ed0: 2d61 6e63 686f 723a 6d69 6464 6c65 3b66  -anchor:middle;f
-00003ee0: 696c 6c3a 2333 3834 6539 613b 6669 6c6c  ill:#384e9a;fill
-00003ef0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00003f00: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
-00003f10: 6474 683a 372e 3534 3938 383b 7374 726f  dth:7.54988;stro
-00003f20: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00003f30: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-00003f40: 3a31 220a 2020 2020 2020 2078 3d22 3634  :1".       x="64
-00003f50: 2e30 3230 3130 3322 0a20 2020 2020 2020  .020103".       
-00003f60: 793d 2238 302e 3832 3437 3322 0a20 2020  y="80.82473".   
-00003f70: 2020 2020 6964 3d22 7465 7874 3122 0a20      id="text1". 
-00003f80: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-00003f90: 2273 6361 6c65 2831 2e30 3136 3031 3937  "scale(1.0160197
-00003fa0: 2c30 2e39 3834 3233 3238 3829 223e 3c74  ,0.98423288)"><t
-00003fb0: 7370 616e 0a20 2020 2020 2020 2020 736f  span.         so
-00003fc0: 6469 706f 6469 3a72 6f6c 653d 226c 696e  dipodi:role="lin
-00003fd0: 6522 0a20 2020 2020 2020 2020 6964 3d22  e".         id="
-00003fe0: 7473 7061 6e31 220a 2020 2020 2020 2020  tspan1".        
-00003ff0: 2078 3d22 3631 2e33 3239 3731 3222 0a20   x="61.329712". 
-00004000: 2020 2020 2020 2020 793d 2238 302e 3832          y="80.82
-00004010: 3437 3322 0a20 2020 2020 2020 2020 7374  473".         st
-00004020: 796c 653d 2266 6f6e 742d 7374 796c 653a  yle="font-style:
-00004030: 6e6f 726d 616c 3b66 6f6e 742d 7661 7269  normal;font-vari
-00004040: 616e 743a 6e6f 726d 616c 3b66 6f6e 742d  ant:normal;font-
-00004050: 7765 6967 6874 3a62 6f6c 643b 666f 6e74  weight:bold;font
-00004060: 2d73 7472 6574 6368 3a6e 6f72 6d61 6c3b  -stretch:normal;
-00004070: 666f 6e74 2d66 616d 696c 793a 4172 6961  font-family:Aria
-00004080: 6c3b 2d69 6e6b 7363 6170 652d 666f 6e74  l;-inkscape-font
-00004090: 2d73 7065 6369 6669 6361 7469 6f6e 3a27  -specification:'
-000040a0: 4172 6961 6c20 426f 6c64 273b 6669 6c6c  Arial Bold';fill
-000040b0: 3a23 3338 3465 3961 3b66 696c 6c2d 6f70  :#384e9a;fill-op
-000040c0: 6163 6974 793a 313b 7374 726f 6b65 2d77  acity:1;stroke-w
-000040d0: 6964 7468 3a37 2e35 3439 3838 223e 3031  idth:7.54988">01
-000040e0: 3c2f 7473 7061 6e3e 3c2f 7465 7874 3e0a  </tspan></text>.
-000040f0: 2020 3c2f 673e 0a3c 2f73 7667 3e0a         </g>.</svg>.
+00000fa0: 723a 2364 3264 3264 323b 7374 6f70 2d6f  r:#d2d2d2;stop-o
+00000fb0: 7061 6369 7479 3a31 3b22 0d0a 2020 2020  pacity:1;"..    
+00000fc0: 2020 2020 206f 6666 7365 743d 2230 220d       offset="0".
+00000fd0: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
+00000fe0: 6f70 3338 3134 2220 2f3e 0d0a 2020 2020  op3814" />..    
+00000ff0: 2020 3c73 746f 700d 0a20 2020 2020 2020    <stop..       
+00001000: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
+00001010: 6c6f 723a 2366 6666 6666 663b 7374 6f70  lor:#ffffff;stop
+00001020: 2d6f 7061 6369 7479 3a31 3b22 0d0a 2020  -opacity:1;"..  
+00001030: 2020 2020 2020 206f 6666 7365 743d 2231         offset="1
+00001040: 220d 0a20 2020 2020 2020 2020 6964 3d22  "..         id="
+00001050: 7374 6f70 3338 3136 2220 2f3e 0d0a 2020  stop3816" />..  
+00001060: 2020 3c2f 6c69 6e65 6172 4772 6164 6965    </linearGradie
+00001070: 6e74 3e0d 0a20 2020 203c 6c69 6e65 6172  nt>..    <linear
+00001080: 4772 6164 6965 6e74 0d0a 2020 2020 2020  Gradient..      
+00001090: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
+000010a0: 656e 7433 3830 3222 0d0a 2020 2020 2020  ent3802"..      
+000010b0: 2069 6e6b 7363 6170 653a 7377 6174 6368   inkscape:swatch
+000010c0: 3d22 736f 6c69 6422 3e0d 0a20 2020 2020  ="solid">..     
+000010d0: 203c 7374 6f70 0d0a 2020 2020 2020 2020   <stop..        
+000010e0: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
+000010f0: 6f72 3a23 3830 3830 3830 3b73 746f 702d  or:#808080;stop-
+00001100: 6f70 6163 6974 793a 313b 220d 0a20 2020  opacity:1;"..   
+00001110: 2020 2020 2020 6f66 6673 6574 3d22 3022        offset="0"
+00001120: 0d0a 2020 2020 2020 2020 2069 643d 2273  ..         id="s
+00001130: 746f 7033 3830 3422 202f 3e0d 0a20 2020  top3804" />..   
+00001140: 203c 2f6c 696e 6561 7247 7261 6469 656e   </linearGradien
+00001150: 743e 0d0a 2020 2020 3c6c 696e 6561 7247  t>..    <linearG
+00001160: 7261 6469 656e 740d 0a20 2020 2020 2020  radient..       
+00001170: 6964 3d22 6c69 6e65 6172 4772 6164 6965  id="linearGradie
+00001180: 6e74 3333 3530 223e 0d0a 2020 2020 2020  nt3350">..      
+00001190: 3c73 746f 700d 0a20 2020 2020 2020 2020  <stop..         
+000011a0: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
+000011b0: 723a 2330 3063 6232 623b 7374 6f70 2d6f  r:#00cb2b;stop-o
+000011c0: 7061 6369 7479 3a30 2e32 3437 3933 3338  pacity:0.2479338
+000011d0: 383b 220d 0a20 2020 2020 2020 2020 6f66  8;"..         of
+000011e0: 6673 6574 3d22 3022 0d0a 2020 2020 2020  fset="0"..      
+000011f0: 2020 2069 643d 2273 746f 7033 3335 3222     id="stop3352"
+00001200: 202f 3e0d 0a20 2020 2020 203c 7374 6f70   />..      <stop
+00001210: 0d0a 2020 2020 2020 2020 2073 7479 6c65  ..         style
+00001220: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 3030  ="stop-color:#00
+00001230: 6362 3262 3b73 746f 702d 6f70 6163 6974  cb2b;stop-opacit
+00001240: 793a 313b 220d 0a20 2020 2020 2020 2020  y:1;"..         
+00001250: 6f66 6673 6574 3d22 3122 0d0a 2020 2020  offset="1"..    
+00001260: 2020 2020 2069 643d 2273 746f 7033 3335       id="stop335
+00001270: 3422 202f 3e0d 0a20 2020 203c 2f6c 696e  4" />..    </lin
+00001280: 6561 7247 7261 6469 656e 743e 0d0a 2020  earGradient>..  
+00001290: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
+000012a0: 740d 0a20 2020 2020 2020 6964 3d22 6c69  t..       id="li
+000012b0: 6e65 6172 4772 6164 6965 6e74 3333 3432  nearGradient3342
+000012c0: 223e 0d0a 2020 2020 2020 3c73 746f 700d  ">..      <stop.
+000012d0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000012e0: 2273 746f 702d 636f 6c6f 723a 2330 3035  "stop-color:#005
+000012f0: 6138 353b 7374 6f70 2d6f 7061 6369 7479  a85;stop-opacity
+00001300: 3a31 3b22 0d0a 2020 2020 2020 2020 206f  :1;"..         o
+00001310: 6666 7365 743d 2230 220d 0a20 2020 2020  ffset="0"..     
+00001320: 2020 2020 6964 3d22 7374 6f70 3333 3434      id="stop3344
+00001330: 2220 2f3e 0d0a 2020 2020 2020 3c73 746f  " />..      <sto
+00001340: 700d 0a20 2020 2020 2020 2020 7374 796c  p..         styl
+00001350: 653d 2273 746f 702d 636f 6c6f 723a 2330  e="stop-color:#0
+00001360: 3035 6138 353b 7374 6f70 2d6f 7061 6369  05a85;stop-opaci
+00001370: 7479 3a30 2e37 3532 3036 3631 343b 220d  ty:0.75206614;".
+00001380: 0a20 2020 2020 2020 2020 6f66 6673 6574  .         offset
+00001390: 3d22 3122 0d0a 2020 2020 2020 2020 2069  ="1"..         i
+000013a0: 643d 2273 746f 7033 3334 3622 202f 3e0d  d="stop3346" />.
+000013b0: 0a20 2020 203c 2f6c 696e 6561 7247 7261  .    </linearGra
+000013c0: 6469 656e 743e 0d0a 2020 2020 3c6c 696e  dient>..    <lin
+000013d0: 6561 7247 7261 6469 656e 740d 0a20 2020  earGradient..   
+000013e0: 2020 2020 6964 3d22 6c69 6e65 6172 4772      id="linearGr
+000013f0: 6164 6965 6e74 3333 3130 223e 0d0a 2020  adient3310">..  
+00001400: 2020 2020 3c73 746f 700d 0a20 2020 2020      <stop..     
+00001410: 2020 2020 6964 3d22 7374 6f70 3333 3132      id="stop3312
+00001420: 220d 0a20 2020 2020 2020 2020 6f66 6673  "..         offs
+00001430: 6574 3d22 3022 0d0a 2020 2020 2020 2020  et="0"..        
+00001440: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
+00001450: 6f72 3a23 6165 3032 3032 3b73 746f 702d  or:#ae0202;stop-
+00001460: 6f70 6163 6974 793a 313b 2220 2f3e 0d0a  opacity:1;" />..
+00001470: 2020 2020 2020 3c73 746f 700d 0a20 2020        <stop..   
+00001480: 2020 2020 2020 6964 3d22 7374 6f70 3333        id="stop33
+00001490: 3134 220d 0a20 2020 2020 2020 2020 6f66  14"..         of
+000014a0: 6673 6574 3d22 3122 0d0a 2020 2020 2020  fset="1"..      
+000014b0: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
+000014c0: 6f6c 6f72 3a23 6234 3735 3735 3b73 746f  olor:#b47575;sto
+000014d0: 702d 6f70 6163 6974 793a 313b 2220 2f3e  p-opacity:1;" />
+000014e0: 0d0a 2020 2020 3c2f 6c69 6e65 6172 4772  ..    </linearGr
+000014f0: 6164 6965 6e74 3e0d 0a20 2020 203c 696e  adient>..    <in
+00001500: 6b73 6361 7065 3a70 6572 7370 6563 7469  kscape:perspecti
+00001510: 7665 0d0a 2020 2020 2020 2073 6f64 6970  ve..       sodip
+00001520: 6f64 693a 7479 7065 3d22 696e 6b73 6361  odi:type="inksca
+00001530: 7065 3a70 6572 7370 3364 220d 0a20 2020  pe:persp3d"..   
+00001540: 2020 2020 696e 6b73 6361 7065 3a76 705f      inkscape:vp_
+00001550: 783d 2230 203a 2031 3538 2e33 3231 3636  x="0 : 158.32166
+00001560: 203a 2031 220d 0a20 2020 2020 2020 696e   : 1"..       in
+00001570: 6b73 6361 7065 3a76 705f 793d 2230 203a  kscape:vp_y="0 :
+00001580: 2031 3030 3020 3a20 3022 0d0a 2020 2020   1000 : 0"..    
+00001590: 2020 2069 6e6b 7363 6170 653a 7670 5f7a     inkscape:vp_z
+000015a0: 3d22 3438 362e 3034 3939 3920 3a20 3135  ="486.04999 : 15
+000015b0: 382e 3332 3136 3620 3a20 3122 0d0a 2020  8.32166 : 1"..  
+000015c0: 2020 2020 2069 6e6b 7363 6170 653a 7065       inkscape:pe
+000015d0: 7273 7033 642d 6f72 6967 696e 3d22 3234  rsp3d-origin="24
+000015e0: 332e 3032 3439 3920 3a20 3133 342e 3335  3.02499 : 134.35
+000015f0: 3931 3720 3a20 3122 0d0a 2020 2020 2020  917 : 1"..      
+00001600: 2069 643d 2270 6572 7370 6563 7469 7665   id="perspective
+00001610: 3437 2220 2f3e 0d0a 2020 2020 3c6c 696e  47" />..    <lin
+00001620: 6561 7247 7261 6469 656e 740d 0a20 2020  earGradient..   
+00001630: 2020 2020 6964 3d22 6c69 6e65 6172 4772      id="linearGr
+00001640: 6164 6965 6e74 3237 3935 223e 0d0a 2020  adient2795">..  
+00001650: 2020 2020 3c73 746f 700d 0a20 2020 2020      <stop..     
+00001660: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
+00001670: 636f 6c6f 723a 2362 3862 3862 383b 7374  color:#b8b8b8;st
+00001680: 6f70 2d6f 7061 6369 7479 3a30 2e34 3938  op-opacity:0.498
+00001690: 3033 3932 3222 0d0a 2020 2020 2020 2020  03922"..        
+000016a0: 206f 6666 7365 743d 2230 220d 0a20 2020   offset="0"..   
+000016b0: 2020 2020 2020 6964 3d22 7374 6f70 3237        id="stop27
+000016c0: 3937 2220 2f3e 0d0a 2020 2020 2020 3c73  97" />..      <s
+000016d0: 746f 700d 0a20 2020 2020 2020 2020 7374  top..         st
+000016e0: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
+000016f0: 2337 6637 6637 663b 7374 6f70 2d6f 7061  #7f7f7f;stop-opa
+00001700: 6369 7479 3a30 220d 0a20 2020 2020 2020  city:0"..       
+00001710: 2020 6f66 6673 6574 3d22 3122 0d0a 2020    offset="1"..  
+00001720: 2020 2020 2020 2069 643d 2273 746f 7032         id="stop2
+00001730: 3739 3922 202f 3e0d 0a20 2020 203c 2f6c  799" />..    </l
+00001740: 696e 6561 7247 7261 6469 656e 743e 0d0a  inearGradient>..
+00001750: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
+00001760: 656e 740d 0a20 2020 2020 2020 6964 3d22  ent..       id="
+00001770: 6c69 6e65 6172 4772 6164 6965 6e74 3237  linearGradient27
+00001780: 3837 223e 0d0a 2020 2020 2020 3c73 746f  87">..      <sto
+00001790: 700d 0a20 2020 2020 2020 2020 7374 796c  p..         styl
+000017a0: 653d 2273 746f 702d 636f 6c6f 723a 2337  e="stop-color:#7
+000017b0: 6637 6637 663b 7374 6f70 2d6f 7061 6369  f7f7f;stop-opaci
+000017c0: 7479 3a30 2e35 220d 0a20 2020 2020 2020  ty:0.5"..       
+000017d0: 2020 6f66 6673 6574 3d22 3022 0d0a 2020    offset="0"..  
+000017e0: 2020 2020 2020 2069 643d 2273 746f 7032         id="stop2
+000017f0: 3738 3922 202f 3e0d 0a20 2020 2020 203c  789" />..      <
+00001800: 7374 6f70 0d0a 2020 2020 2020 2020 2073  stop..         s
+00001810: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
+00001820: 3a23 3766 3766 3766 3b73 746f 702d 6f70  :#7f7f7f;stop-op
+00001830: 6163 6974 793a 3022 0d0a 2020 2020 2020  acity:0"..      
+00001840: 2020 206f 6666 7365 743d 2231 220d 0a20     offset="1".. 
+00001850: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
+00001860: 3237 3931 2220 2f3e 0d0a 2020 2020 3c2f  2791" />..    </
+00001870: 6c69 6e65 6172 4772 6164 6965 6e74 3e0d  linearGradient>.
+00001880: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
+00001890: 6965 6e74 0d0a 2020 2020 2020 2069 643d  ient..       id=
+000018a0: 226c 696e 6561 7247 7261 6469 656e 7433  "linearGradient3
+000018b0: 3637 3622 3e0d 0a20 2020 2020 203c 7374  676">..      <st
+000018c0: 6f70 0d0a 2020 2020 2020 2020 2073 7479  op..         sty
+000018d0: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
+000018e0: 6232 6232 6232 3b73 746f 702d 6f70 6163  b2b2b2;stop-opac
+000018f0: 6974 793a 302e 3522 0d0a 2020 2020 2020  ity:0.5"..      
+00001900: 2020 206f 6666 7365 743d 2230 220d 0a20     offset="0".. 
+00001910: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
+00001920: 3336 3738 2220 2f3e 0d0a 2020 2020 2020  3678" />..      
+00001930: 3c73 746f 700d 0a20 2020 2020 2020 2020  <stop..         
+00001940: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
+00001950: 723a 2362 3362 3362 333b 7374 6f70 2d6f  r:#b3b3b3;stop-o
+00001960: 7061 6369 7479 3a30 220d 0a20 2020 2020  pacity:0"..     
+00001970: 2020 2020 6f66 6673 6574 3d22 3122 0d0a      offset="1"..
+00001980: 2020 2020 2020 2020 2069 643d 2273 746f           id="sto
+00001990: 7033 3638 3022 202f 3e0d 0a20 2020 203c  p3680" />..    <
+000019a0: 2f6c 696e 6561 7247 7261 6469 656e 743e  /linearGradient>
+000019b0: 0d0a 2020 2020 3c6c 696e 6561 7247 7261  ..    <linearGra
+000019c0: 6469 656e 740d 0a20 2020 2020 2020 6964  dient..       id
+000019d0: 3d22 6c69 6e65 6172 4772 6164 6965 6e74  ="linearGradient
+000019e0: 3332 3336 223e 0d0a 2020 2020 2020 3c73  3236">..      <s
+000019f0: 746f 700d 0a20 2020 2020 2020 2020 7374  top..         st
+00001a00: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
+00001a10: 2366 3466 3466 343b 7374 6f70 2d6f 7061  #f4f4f4;stop-opa
+00001a20: 6369 7479 3a31 220d 0a20 2020 2020 2020  city:1"..       
+00001a30: 2020 6f66 6673 6574 3d22 3022 0d0a 2020    offset="0"..  
+00001a40: 2020 2020 2020 2069 643d 2273 746f 7033         id="stop3
+00001a50: 3234 3422 202f 3e0d 0a20 2020 2020 203c  244" />..      <
+00001a60: 7374 6f70 0d0a 2020 2020 2020 2020 2073  stop..         s
+00001a70: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
+00001a80: 3a23 6666 6666 6666 3b73 746f 702d 6f70  :#ffffff;stop-op
+00001a90: 6163 6974 793a 3122 0d0a 2020 2020 2020  acity:1"..      
+00001aa0: 2020 206f 6666 7365 743d 2231 220d 0a20     offset="1".. 
+00001ab0: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
+00001ac0: 3332 3430 2220 2f3e 0d0a 2020 2020 3c2f  3240" />..    </
+00001ad0: 6c69 6e65 6172 4772 6164 6965 6e74 3e0d  linearGradient>.
+00001ae0: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
+00001af0: 6965 6e74 0d0a 2020 2020 2020 2069 643d  ient..       id=
+00001b00: 226c 696e 6561 7247 7261 6469 656e 7434  "linearGradient4
+00001b10: 3637 3122 3e0d 0a20 2020 2020 203c 7374  671">..      <st
+00001b20: 6f70 0d0a 2020 2020 2020 2020 2073 7479  op..         sty
+00001b30: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
+00001b40: 6666 6434 3362 3b73 746f 702d 6f70 6163  ffd43b;stop-opac
+00001b50: 6974 793a 3122 0d0a 2020 2020 2020 2020  ity:1"..        
+00001b60: 206f 6666 7365 743d 2230 220d 0a20 2020   offset="0"..   
+00001b70: 2020 2020 2020 6964 3d22 7374 6f70 3436        id="stop46
+00001b80: 3733 2220 2f3e 0d0a 2020 2020 2020 3c73  73" />..      <s
+00001b90: 746f 700d 0a20 2020 2020 2020 2020 7374  top..         st
+00001ba0: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
+00001bb0: 2366 6665 3837 333b 7374 6f70 2d6f 7061  #ffe873;stop-opa
+00001bc0: 6369 7479 3a31 220d 0a20 2020 2020 2020  city:1"..       
+00001bd0: 2020 6f66 6673 6574 3d22 3122 0d0a 2020    offset="1"..  
+00001be0: 2020 2020 2020 2069 643d 2273 746f 7034         id="stop4
+00001bf0: 3637 3522 202f 3e0d 0a20 2020 203c 2f6c  675" />..    </l
+00001c00: 696e 6561 7247 7261 6469 656e 743e 0d0a  inearGradient>..
+00001c10: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
+00001c20: 656e 740d 0a20 2020 2020 2020 6964 3d22  ent..       id="
+00001c30: 6c69 6e65 6172 4772 6164 6965 6e74 3436  linearGradient46
+00001c40: 3839 223e 0d0a 2020 2020 2020 3c73 746f  89">..      <sto
+00001c50: 700d 0a20 2020 2020 2020 2020 7374 796c  p..         styl
+00001c60: 653d 2273 746f 702d 636f 6c6f 723a 2335  e="stop-color:#5
+00001c70: 6139 6664 343b 7374 6f70 2d6f 7061 6369  a9fd4;stop-opaci
+00001c80: 7479 3a31 220d 0a20 2020 2020 2020 2020  ty:1"..         
+00001c90: 6f66 6673 6574 3d22 3022 0d0a 2020 2020  offset="0"..    
+00001ca0: 2020 2020 2069 643d 2273 746f 7034 3639       id="stop469
+00001cb0: 3122 202f 3e0d 0a20 2020 2020 203c 7374  1" />..      <st
+00001cc0: 6f70 0d0a 2020 2020 2020 2020 2073 7479  op..         sty
+00001cd0: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
+00001ce0: 3330 3639 3938 3b73 746f 702d 6f70 6163  306998;stop-opac
+00001cf0: 6974 793a 3122 0d0a 2020 2020 2020 2020  ity:1"..        
+00001d00: 206f 6666 7365 743d 2231 220d 0a20 2020   offset="1"..   
+00001d10: 2020 2020 2020 6964 3d22 7374 6f70 3436        id="stop46
+00001d20: 3933 2220 2f3e 0d0a 2020 2020 3c2f 6c69  93" />..    </li
+00001d30: 6e65 6172 4772 6164 6965 6e74 3e0d 0a20  nearGradient>.. 
+00001d40: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
+00001d50: 6e74 0d0a 2020 2020 2020 2078 313d 2232  nt..       x1="2
+00001d60: 3234 2e32 3339 3936 220d 0a20 2020 2020  24.23996"..     
+00001d70: 2020 7931 3d22 3134 342e 3735 3731 3722    y1="144.75717"
+00001d80: 0d0a 2020 2020 2020 2078 323d 222d 3635  ..       x2="-65
+00001d90: 2e33 3038 3530 3222 0d0a 2020 2020 2020  .308502"..      
+00001da0: 2079 323d 2231 3434 2e37 3537 3137 220d   y2="144.75717".
+00001db0: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
+00001dc0: 6172 4772 6164 6965 6e74 3239 3837 220d  arGradient2987".
+00001dd0: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
+00001de0: 6566 3d22 236c 696e 6561 7247 7261 6469  ef="#linearGradi
+00001df0: 656e 7434 3637 3122 0d0a 2020 2020 2020  ent4671"..      
+00001e00: 2067 7261 6469 656e 7455 6e69 7473 3d22   gradientUnits="
+00001e10: 7573 6572 5370 6163 654f 6e55 7365 220d  userSpaceOnUse".
+00001e20: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+00001e30: 5472 616e 7366 6f72 6d3d 2274 7261 6e73  Transform="trans
+00001e40: 6c61 7465 2831 3030 2e32 3730 322c 3939  late(100.2702,99
+00001e50: 2e36 3131 3136 2922 202f 3e0d 0a20 2020  .61116)" />..   
+00001e60: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
+00001e70: 0d0a 2020 2020 2020 2078 313d 2231 3732  ..       x1="172
+00001e80: 2e39 3432 3038 220d 0a20 2020 2020 2020  .94208"..       
+00001e90: 7931 3d22 3737 2e34 3735 3938 3322 0d0a  y1="77.475983"..
+00001ea0: 2020 2020 2020 2078 323d 2232 362e 3637         x2="26.67
+00001eb0: 3032 3938 220d 0a20 2020 2020 2020 7932  0298"..       y2
+00001ec0: 3d22 3736 2e33 3133 3133 3322 0d0a 2020  ="76.313133"..  
+00001ed0: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
+00001ee0: 7261 6469 656e 7432 3939 3022 0d0a 2020  radient2990"..  
+00001ef0: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
+00001f00: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
+00001f10: 3436 3839 220d 0a20 2020 2020 2020 6772  4689"..       gr
+00001f20: 6164 6965 6e74 556e 6974 733d 2275 7365  adientUnits="use
+00001f30: 7253 7061 6365 4f6e 5573 6522 0d0a 2020  rSpaceOnUse"..  
+00001f40: 2020 2020 2067 7261 6469 656e 7454 7261       gradientTra
+00001f50: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+00001f60: 6528 3130 302e 3237 3032 2c39 392e 3631  e(100.2702,99.61
+00001f70: 3131 3629 2220 2f3e 0d0a 2020 2020 3c6c  116)" />..    <l
+00001f80: 696e 6561 7247 7261 6469 656e 740d 0a20  inearGradient.. 
+00001f90: 2020 2020 2020 7831 3d22 3137 322e 3934        x1="172.94
+00001fa0: 3230 3822 0d0a 2020 2020 2020 2079 313d  208"..       y1=
+00001fb0: 2237 372e 3437 3539 3833 220d 0a20 2020  "77.475983"..   
+00001fc0: 2020 2020 7832 3d22 3236 2e36 3730 3239      x2="26.67029
+00001fd0: 3822 0d0a 2020 2020 2020 2079 323d 2237  8"..       y2="7
+00001fe0: 362e 3331 3331 3333 220d 0a20 2020 2020  6.313133"..     
+00001ff0: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
+00002000: 6965 6e74 3235 3837 220d 0a20 2020 2020  ient2587"..     
+00002010: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
+00002020: 696e 6561 7247 7261 6469 656e 7434 3638  inearGradient468
+00002030: 3922 0d0a 2020 2020 2020 2067 7261 6469  9"..       gradi
+00002040: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00002050: 6163 654f 6e55 7365 220d 0a20 2020 2020  aceOnUse"..     
+00002060: 2020 6772 6164 6965 6e74 5472 616e 7366    gradientTransf
+00002070: 6f72 6d3d 2274 7261 6e73 6c61 7465 2831  orm="translate(1
+00002080: 3030 2e32 3730 322c 3939 2e36 3131 3136  00.2702,99.61116
+00002090: 2922 202f 3e0d 0a20 2020 203c 6c69 6e65  )" />..    <line
+000020a0: 6172 4772 6164 6965 6e74 0d0a 2020 2020  arGradient..    
+000020b0: 2020 2078 313d 2232 3234 2e32 3339 3936     x1="224.23996
+000020c0: 220d 0a20 2020 2020 2020 7931 3d22 3134  "..       y1="14
+000020d0: 342e 3735 3731 3722 0d0a 2020 2020 2020  4.75717"..      
+000020e0: 2078 323d 222d 3635 2e33 3038 3530 3222   x2="-65.308502"
+000020f0: 0d0a 2020 2020 2020 2079 323d 2231 3434  ..       y2="144
+00002100: 2e37 3537 3137 220d 0a20 2020 2020 2020  .75717"..       
+00002110: 6964 3d22 6c69 6e65 6172 4772 6164 6965  id="linearGradie
+00002120: 6e74 3235 3839 220d 0a20 2020 2020 2020  nt2589"..       
+00002130: 786c 696e 6b3a 6872 6566 3d22 236c 696e  xlink:href="#lin
+00002140: 6561 7247 7261 6469 656e 7434 3637 3122  earGradient4671"
+00002150: 0d0a 2020 2020 2020 2067 7261 6469 656e  ..       gradien
+00002160: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
+00002170: 654f 6e55 7365 220d 0a20 2020 2020 2020  eOnUse"..       
+00002180: 6772 6164 6965 6e74 5472 616e 7366 6f72  gradientTransfor
+00002190: 6d3d 2274 7261 6e73 6c61 7465 2831 3030  m="translate(100
+000021a0: 2e32 3730 322c 3939 2e36 3131 3136 2922  .2702,99.61116)"
+000021b0: 202f 3e0d 0a20 2020 203c 6c69 6e65 6172   />..    <linear
+000021c0: 4772 6164 6965 6e74 0d0a 2020 2020 2020  Gradient..      
+000021d0: 2078 313d 2231 3732 2e39 3432 3038 220d   x1="172.94208".
+000021e0: 0a20 2020 2020 2020 7931 3d22 3737 2e34  .       y1="77.4
+000021f0: 3735 3938 3322 0d0a 2020 2020 2020 2078  75983"..       x
+00002200: 323d 2232 362e 3637 3032 3938 220d 0a20  2="26.670298".. 
+00002210: 2020 2020 2020 7932 3d22 3736 2e33 3133        y2="76.313
+00002220: 3133 3322 0d0a 2020 2020 2020 2069 643d  133"..       id=
+00002230: 226c 696e 6561 7247 7261 6469 656e 7432  "linearGradient2
+00002240: 3234 3822 0d0a 2020 2020 2020 2078 6c69  248"..       xli
+00002250: 6e6b 3a68 7265 663d 2223 6c69 6e65 6172  nk:href="#linear
+00002260: 4772 6164 6965 6e74 3436 3839 220d 0a20  Gradient4689".. 
+00002270: 2020 2020 2020 6772 6164 6965 6e74 556e        gradientUn
+00002280: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
+00002290: 5573 6522 0d0a 2020 2020 2020 2067 7261  Use"..       gra
+000022a0: 6469 656e 7454 7261 6e73 666f 726d 3d22  dientTransform="
+000022b0: 7472 616e 736c 6174 6528 3130 302e 3237  translate(100.27
+000022c0: 3032 2c39 392e 3631 3131 3629 2220 2f3e  02,99.61116)" />
+000022d0: 0d0a 2020 2020 3c6c 696e 6561 7247 7261  ..    <linearGra
+000022e0: 6469 656e 740d 0a20 2020 2020 2020 7831  dient..       x1
+000022f0: 3d22 3232 342e 3233 3939 3622 0d0a 2020  ="224.23996"..  
+00002300: 2020 2020 2079 313d 2231 3434 2e37 3537       y1="144.757
+00002310: 3137 220d 0a20 2020 2020 2020 7832 3d22  17"..       x2="
+00002320: 2d36 352e 3330 3835 3032 220d 0a20 2020  -65.308502"..   
+00002330: 2020 2020 7932 3d22 3134 342e 3735 3731      y2="144.7571
+00002340: 3722 0d0a 2020 2020 2020 2069 643d 226c  7"..       id="l
+00002350: 696e 6561 7247 7261 6469 656e 7432 3235  inearGradient225
+00002360: 3022 0d0a 2020 2020 2020 2078 6c69 6e6b  0"..       xlink
+00002370: 3a68 7265 663d 2223 6c69 6e65 6172 4772  :href="#linearGr
+00002380: 6164 6965 6e74 3436 3731 220d 0a20 2020  adient4671"..   
+00002390: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
+000023a0: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
+000023b0: 6522 0d0a 2020 2020 2020 2067 7261 6469  e"..       gradi
+000023c0: 656e 7454 7261 6e73 666f 726d 3d22 7472  entTransform="tr
+000023d0: 616e 736c 6174 6528 3130 302e 3237 3032  anslate(100.2702
+000023e0: 2c39 392e 3631 3131 3629 2220 2f3e 0d0a  ,99.61116)" />..
+000023f0: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
+00002400: 656e 740d 0a20 2020 2020 2020 7831 3d22  ent..       x1="
+00002410: 3232 342e 3233 3939 3622 0d0a 2020 2020  224.23996"..    
+00002420: 2020 2079 313d 2231 3434 2e37 3537 3137     y1="144.75717
+00002430: 220d 0a20 2020 2020 2020 7832 3d22 2d36  "..       x2="-6
+00002440: 352e 3330 3835 3032 220d 0a20 2020 2020  5.308502"..     
+00002450: 2020 7932 3d22 3134 342e 3735 3731 3722    y2="144.75717"
+00002460: 0d0a 2020 2020 2020 2069 643d 226c 696e  ..       id="lin
+00002470: 6561 7247 7261 6469 656e 7432 3235 3522  earGradient2255"
+00002480: 0d0a 2020 2020 2020 2078 6c69 6e6b 3a68  ..       xlink:h
+00002490: 7265 663d 2223 6c69 6e65 6172 4772 6164  ref="#linearGrad
+000024a0: 6965 6e74 3436 3731 220d 0a20 2020 2020  ient4671"..     
+000024b0: 2020 6772 6164 6965 6e74 556e 6974 733d    gradientUnits=
+000024c0: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
+000024d0: 0d0a 2020 2020 2020 2067 7261 6469 656e  ..       gradien
+000024e0: 7454 7261 6e73 666f 726d 3d22 6d61 7472  tTransform="matr
+000024f0: 6978 2830 2e35 3632 3534 312c 302c 302c  ix(0.562541,0,0,
+00002500: 302e 3536 3739 3732 2c2d 3131 2e35 3937  0.567972,-11.597
+00002510: 342c 2d37 2e36 3039 3534 2922 202f 3e0d  4,-7.60954)" />.
+00002520: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
+00002530: 6965 6e74 0d0a 2020 2020 2020 2078 313d  ient..       x1=
+00002540: 2231 3732 2e39 3432 3038 220d 0a20 2020  "172.94208"..   
+00002550: 2020 2020 7931 3d22 3736 2e31 3736 3232      y1="76.17622
+00002560: 3422 0d0a 2020 2020 2020 2078 323d 2232  4"..       x2="2
+00002570: 362e 3637 3032 3938 220d 0a20 2020 2020  6.670298"..     
+00002580: 2020 7932 3d22 3736 2e33 3133 3133 3322    y2="76.313133"
+00002590: 0d0a 2020 2020 2020 2069 643d 226c 696e  ..       id="lin
+000025a0: 6561 7247 7261 6469 656e 7432 3235 3822  earGradient2258"
+000025b0: 0d0a 2020 2020 2020 2078 6c69 6e6b 3a68  ..       xlink:h
+000025c0: 7265 663d 2223 6c69 6e65 6172 4772 6164  ref="#linearGrad
+000025d0: 6965 6e74 3436 3839 220d 0a20 2020 2020  ient4689"..     
+000025e0: 2020 6772 6164 6965 6e74 556e 6974 733d    gradientUnits=
+000025f0: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
+00002600: 0d0a 2020 2020 2020 2067 7261 6469 656e  ..       gradien
+00002610: 7454 7261 6e73 666f 726d 3d22 6d61 7472  tTransform="matr
+00002620: 6978 2830 2e35 3632 3534 312c 302c 302c  ix(0.562541,0,0,
+00002630: 302e 3536 3739 3732 2c2d 3131 2e35 3937  0.567972,-11.597
+00002640: 342c 2d37 2e36 3039 3534 2922 202f 3e0d  4,-7.60954)" />.
+00002650: 0a20 2020 203c 7261 6469 616c 4772 6164  .    <radialGrad
+00002660: 6965 6e74 0d0a 2020 2020 2020 2063 783d  ient..       cx=
+00002670: 2236 312e 3531 3838 3833 220d 0a20 2020  "61.518883"..   
+00002680: 2020 2020 6379 3d22 3133 322e 3238 3537      cy="132.2857
+00002690: 3522 0d0a 2020 2020 2020 2072 3d22 3239  5"..       r="29
+000026a0: 2e30 3336 3931 3322 0d0a 2020 2020 2020  .036913"..      
+000026b0: 2066 783d 2236 312e 3531 3838 3833 220d   fx="61.518883".
+000026c0: 0a20 2020 2020 2020 6679 3d22 3133 322e  .       fy="132.
+000026d0: 3238 3537 3522 0d0a 2020 2020 2020 2069  28575"..       i
+000026e0: 643d 2272 6164 6961 6c47 7261 6469 656e  d="radialGradien
+000026f0: 7432 3830 3122 0d0a 2020 2020 2020 2078  t2801"..       x
+00002700: 6c69 6e6b 3a68 7265 663d 2223 6c69 6e65  link:href="#line
+00002710: 6172 4772 6164 6965 6e74 3237 3935 220d  arGradient2795".
+00002720: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+00002730: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
+00002740: 4f6e 5573 6522 0d0a 2020 2020 2020 2067  OnUse"..       g
+00002750: 7261 6469 656e 7454 7261 6e73 666f 726d  radientTransform
+00002760: 3d22 6d61 7472 6978 2831 2c30 2c30 2c30  ="matrix(1,0,0,0
+00002770: 2e31 3737 3936 362c 302c 3130 382e 3734  .177966,0,108.74
+00002780: 3334 2922 202f 3e0d 0a20 2020 203c 6c69  34)" />..    <li
+00002790: 6e65 6172 4772 6164 6965 6e74 0d0a 2020  nearGradient..  
+000027a0: 2020 2020 2078 313d 2231 3530 2e39 3631       x1="150.961
+000027b0: 3131 220d 0a20 2020 2020 2020 7931 3d22  11"..       y1="
+000027c0: 3139 322e 3335 3137 3622 0d0a 2020 2020  192.35176"..    
+000027d0: 2020 2078 323d 2231 3132 2e30 3331 3434     x2="112.03144
+000027e0: 220d 0a20 2020 2020 2020 7932 3d22 3133  "..       y2="13
+000027f0: 372e 3237 3239 3922 0d0a 2020 2020 2020  7.27299"..      
+00002800: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
+00002810: 656e 7431 3437 3522 0d0a 2020 2020 2020  ent1475"..      
+00002820: 2078 6c69 6e6b 3a68 7265 663d 2223 6c69   xlink:href="#li
+00002830: 6e65 6172 4772 6164 6965 6e74 3436 3731  nearGradient4671
+00002840: 220d 0a20 2020 2020 2020 6772 6164 6965  "..       gradie
+00002850: 6e74 556e 6974 733d 2275 7365 7253 7061  ntUnits="userSpa
+00002860: 6365 4f6e 5573 6522 0d0a 2020 2020 2020  ceOnUse"..      
+00002870: 2067 7261 6469 656e 7454 7261 6e73 666f   gradientTransfo
+00002880: 726d 3d22 6d61 7472 6978 2830 2e35 3632  rm="matrix(0.562
+00002890: 3534 312c 302c 302c 302e 3536 3739 3732  541,0,0,0.567972
+000028a0: 2c2d 392e 3339 3937 3439 2c2d 352e 3330  ,-9.399749,-5.30
+000028b0: 3533 3137 2922 202f 3e0d 0a20 2020 203c  5317)" />..    <
+000028c0: 6c69 6e65 6172 4772 6164 6965 6e74 0d0a  linearGradient..
+000028d0: 2020 2020 2020 2078 313d 2232 362e 3634         x1="26.64
+000028e0: 3839 3337 220d 0a20 2020 2020 2020 7931  8937"..       y1
+000028f0: 3d22 3230 2e36 3033 3738 3122 0d0a 2020  ="20.603781"..  
+00002900: 2020 2020 2078 323d 2231 3335 2e36 3635       x2="135.665
+00002910: 3235 220d 0a20 2020 2020 2020 7932 3d22  25"..       y2="
+00002920: 3131 342e 3339 3736 3722 0d0a 2020 2020  114.39767"..    
+00002930: 2020 2069 643d 226c 696e 6561 7247 7261     id="linearGra
+00002940: 6469 656e 7431 3437 3822 0d0a 2020 2020  dient1478"..    
+00002950: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
+00002960: 6c69 6e65 6172 4772 6164 6965 6e74 3436  linearGradient46
+00002970: 3839 220d 0a20 2020 2020 2020 6772 6164  89"..       grad
+00002980: 6965 6e74 556e 6974 733d 2275 7365 7253  ientUnits="userS
+00002990: 7061 6365 4f6e 5573 6522 0d0a 2020 2020  paceOnUse"..    
+000029a0: 2020 2067 7261 6469 656e 7454 7261 6e73     gradientTrans
+000029b0: 666f 726d 3d22 6d61 7472 6978 2830 2e35  form="matrix(0.5
+000029c0: 3632 3534 312c 302c 302c 302e 3536 3739  62541,0,0,0.5679
+000029d0: 3732 2c2d 392e 3339 3937 3439 2c2d 352e  72,-9.399749,-5.
+000029e0: 3330 3533 3137 2922 202f 3e0d 0a20 2020  305317)" />..   
+000029f0: 203c 7261 6469 616c 4772 6164 6965 6e74   <radialGradient
+00002a00: 0d0a 2020 2020 2020 2063 783d 2236 312e  ..       cx="61.
+00002a10: 3531 3838 3833 220d 0a20 2020 2020 2020  518883"..       
+00002a20: 6379 3d22 3133 322e 3238 3537 3522 0d0a  cy="132.28575"..
+00002a30: 2020 2020 2020 2072 3d22 3239 2e30 3336         r="29.036
+00002a40: 3931 3322 0d0a 2020 2020 2020 2066 783d  913"..       fx=
+00002a50: 2236 312e 3531 3838 3833 220d 0a20 2020  "61.518883"..   
+00002a60: 2020 2020 6679 3d22 3133 322e 3238 3537      fy="132.2857
+00002a70: 3522 0d0a 2020 2020 2020 2069 643d 2272  5"..       id="r
+00002a80: 6164 6961 6c47 7261 6469 656e 7431 3438  adialGradient148
+00002a90: 3022 0d0a 2020 2020 2020 2078 6c69 6e6b  0"..       xlink
+00002aa0: 3a68 7265 663d 2223 6c69 6e65 6172 4772  :href="#linearGr
+00002ab0: 6164 6965 6e74 3237 3935 220d 0a20 2020  adient2795"..   
+00002ac0: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
+00002ad0: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
+00002ae0: 6522 0d0a 2020 2020 2020 2067 7261 6469  e"..       gradi
+00002af0: 656e 7454 7261 6e73 666f 726d 3d22 6d61  entTransform="ma
+00002b00: 7472 6978 2832 2e33 3832 3731 3665 2d38  trix(2.382716e-8
+00002b10: 2c2d 302e 3239 3634 3035 2c31 2e34 3336  ,-0.296405,1.436
+00002b20: 3736 2c34 2e36 3833 3637 3365 2d37 2c2d  76,4.683673e-7,-
+00002b30: 3132 382e 3534 342c 3135 302e 3532 3032  128.544,150.5202
+00002b40: 2922 202f 3e0d 0a20 2020 203c 7261 6469  )" />..    <radi
+00002b50: 616c 4772 6164 6965 6e74 0d0a 2020 2020  alGradient..    
+00002b60: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00002b70: 6563 743d 2261 6c77 6179 7322 0d0a 2020  ect="always"..  
+00002b80: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
+00002b90: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
+00002ba0: 3237 3935 220d 0a20 2020 2020 2020 6964  2795"..       id
+00002bb0: 3d22 7261 6469 616c 4772 6164 6965 6e74  ="radialGradient
+00002bc0: 3234 3231 220d 0a20 2020 2020 2020 6772  2421"..       gr
+00002bd0: 6164 6965 6e74 556e 6974 733d 2275 7365  adientUnits="use
+00002be0: 7253 7061 6365 4f6e 5573 6522 0d0a 2020  rSpaceOnUse"..  
+00002bf0: 2020 2020 2067 7261 6469 656e 7454 7261       gradientTra
+00002c00: 6e73 666f 726d 3d22 6d61 7472 6978 2831  nsform="matrix(1
+00002c10: 2e37 3439 3035 3635 652d 382c 2d30 2e32  .7490565e-8,-0.2
+00002c20: 3339 3934 372c 312e 3035 3436 3638 2c33  39947,1.054668,3
+00002c30: 2e37 3931 3534 3537 652d 372c 2d37 382e  .7915457e-7,-78.
+00002c40: 3130 3934 3239 2c31 3438 2e38 3539 3036  109429,148.85906
+00002c50: 2922 0d0a 2020 2020 2020 2063 783d 2236  )"..       cx="6
+00002c60: 312e 3531 3838 3833 220d 0a20 2020 2020  1.518883"..     
+00002c70: 2020 6379 3d22 3133 322e 3238 3537 3522    cy="132.28575"
+00002c80: 0d0a 2020 2020 2020 2066 783d 2236 312e  ..       fx="61.
+00002c90: 3531 3838 3833 220d 0a20 2020 2020 2020  518883"..       
+00002ca0: 6679 3d22 3133 322e 3238 3537 3522 0d0a  fy="132.28575"..
+00002cb0: 2020 2020 2020 2072 3d22 3239 2e30 3336         r="29.036
+00002cc0: 3931 3322 202f 3e0d 0a20 2020 203c 6c69  913" />..    <li
+00002cd0: 6e65 6172 4772 6164 6965 6e74 0d0a 2020  nearGradient..  
+00002ce0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+00002cf0: 6c6c 6563 743d 2261 6c77 6179 7322 0d0a  llect="always"..
+00002d00: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
+00002d10: 663d 2223 6c69 6e65 6172 4772 6164 6965  f="#linearGradie
+00002d20: 6e74 3436 3731 2d38 220d 0a20 2020 2020  nt4671-8"..     
+00002d30: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
+00002d40: 6965 6e74 3338 3236 2d36 220d 0a20 2020  ient3826-6"..   
+00002d50: 2020 2020 7831 3d22 3336 2e39 3730 3839      x1="36.97089
+00002d60: 3822 0d0a 2020 2020 2020 2079 313d 2235  8"..       y1="5
+00002d70: 342e 3634 3637 3633 220d 0a20 2020 2020  4.646763"..     
+00002d80: 2020 7832 3d22 3837 2e37 3034 3638 3122    x2="87.704681"
+00002d90: 0d0a 2020 2020 2020 2079 323d 2235 342e  ..       y2="54.
+00002da0: 3634 3637 3633 220d 0a20 2020 2020 2020  646763"..       
+00002db0: 6772 6164 6965 6e74 556e 6974 733d 2275  gradientUnits="u
+00002dc0: 7365 7253 7061 6365 4f6e 5573 6522 202f  serSpaceOnUse" /
+00002dd0: 3e0d 0a20 2020 203c 6c69 6e65 6172 4772  >..    <linearGr
+00002de0: 6164 6965 6e74 0d0a 2020 2020 2020 2069  adient..       i
+00002df0: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
+00002e00: 7434 3637 312d 3822 3e0d 0a20 2020 2020  t4671-8">..     
+00002e10: 203c 7374 6f70 0d0a 2020 2020 2020 2020   <stop..        
+00002e20: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
+00002e30: 6f72 3a23 6666 6434 3362 3b73 746f 702d  or:#ffd43b;stop-
+00002e40: 6f70 6163 6974 793a 3122 0d0a 2020 2020  opacity:1"..    
+00002e50: 2020 2020 206f 6666 7365 743d 2230 220d       offset="0".
+00002e60: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
+00002e70: 6f70 3436 3733 2d38 2220 2f3e 0d0a 2020  op4673-8" />..  
+00002e80: 2020 2020 3c73 746f 700d 0a20 2020 2020      <stop..     
+00002e90: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
+00002ea0: 636f 6c6f 723a 2366 6665 3837 333b 7374  color:#ffe873;st
+00002eb0: 6f70 2d6f 7061 6369 7479 3a31 220d 0a20  op-opacity:1".. 
+00002ec0: 2020 2020 2020 2020 6f66 6673 6574 3d22          offset="
+00002ed0: 3122 0d0a 2020 2020 2020 2020 2069 643d  1"..         id=
+00002ee0: 2273 746f 7034 3637 352d 3222 202f 3e0d  "stop4675-2" />.
+00002ef0: 0a20 2020 203c 2f6c 696e 6561 7247 7261  .    </linearGra
+00002f00: 6469 656e 743e 0d0a 2020 2020 3c6c 696e  dient>..    <lin
+00002f10: 6561 7247 7261 6469 656e 740d 0a20 2020  earGradient..   
+00002f20: 2020 2020 696e 6b73 6361 7065 3a63 6f6c      inkscape:col
+00002f30: 6c65 6374 3d22 616c 7761 7973 220d 0a20  lect="always".. 
+00002f40: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
+00002f50: 3d22 236c 696e 6561 7247 7261 6469 656e  ="#linearGradien
+00002f60: 7433 3831 3222 0d0a 2020 2020 2020 2069  t3812"..       i
+00002f70: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
+00002f80: 7433 3831 3822 0d0a 2020 2020 2020 2078  t3818"..       x
+00002f90: 313d 2237 382e 3031 3230 3234 220d 0a20  1="78.012024".. 
+00002fa0: 2020 2020 2020 7931 3d22 3830 2e33 3032        y1="80.302
+00002fb0: 3933 3322 0d0a 2020 2020 2020 2078 323d  933"..       x2=
+00002fc0: 2231 3234 2e36 3739 3634 220d 0a20 2020  "124.67964"..   
+00002fd0: 2020 2020 7932 3d22 3238 2e36 3033 3332      y2="28.60332
+00002fe0: 3722 0d0a 2020 2020 2020 2067 7261 6469  7"..       gradi
+00002ff0: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00003000: 6163 654f 6e55 7365 2220 2f3e 0d0a 2020  aceOnUse" />..  
+00003010: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
+00003020: 740d 0a20 2020 2020 2020 696e 6b73 6361  t..       inksca
+00003030: 7065 3a63 6f6c 6c65 6374 3d22 616c 7761  pe:collect="alwa
+00003040: 7973 220d 0a20 2020 2020 2020 786c 696e  ys"..       xlin
+00003050: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
+00003060: 7261 6469 656e 7433 3831 3222 0d0a 2020  radient3812"..  
+00003070: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
+00003080: 7261 6469 656e 7434 3039 3722 0d0a 2020  radient4097"..  
+00003090: 2020 2020 2078 313d 222d 3230 352e 3035       x1="-205.05
+000030a0: 3433 3122 0d0a 2020 2020 2020 2079 313d  431"..       y1=
+000030b0: 2235 352e 3630 3634 3431 220d 0a20 2020  "55.606441"..   
+000030c0: 2020 2020 7832 3d22 2d36 342e 3830 3632      x2="-64.8062
+000030d0: 3539 220d 0a20 2020 2020 2020 7932 3d22  59"..       y2="
+000030e0: 3535 2e36 3036 3434 3122 0d0a 2020 2020  55.606441"..    
+000030f0: 2020 2067 7261 6469 656e 7455 6e69 7473     gradientUnits
+00003100: 3d22 7573 6572 5370 6163 654f 6e55 7365  ="userSpaceOnUse
+00003110: 220d 0a20 2020 2020 2020 6772 6164 6965  "..       gradie
+00003120: 6e74 5472 616e 7366 6f72 6d3d 226d 6174  ntTransform="mat
+00003130: 7269 7828 312e 3039 3531 3533 392c 302c  rix(1.0951539,0,
+00003140: 302c 312e 3033 3135 3236 382c 3238 332e  0,1.0315268,283.
+00003150: 3739 3331 312c 3134 2e37 3232 3734 3629  79311,14.722746)
+00003160: 2220 2f3e 0d0a 2020 2020 3c6c 696e 6561  " />..    <linea
+00003170: 7247 7261 6469 656e 740d 0a20 2020 2020  rGradient..     
+00003180: 2020 696e 6b73 6361 7065 3a63 6f6c 6c65    inkscape:colle
+00003190: 6374 3d22 616c 7761 7973 220d 0a20 2020  ct="always"..   
+000031a0: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+000031b0: 236c 696e 6561 7247 7261 6469 656e 7431  #linearGradient1
+000031c0: 3839 3422 0d0a 2020 2020 2020 2069 643d  894"..       id=
+000031d0: 226c 696e 6561 7247 7261 6469 656e 7434  "linearGradient4
+000031e0: 3039 372d 3422 0d0a 2020 2020 2020 2078  097-4"..       x
+000031f0: 313d 222d 3230 352e 3035 3433 3122 0d0a  1="-205.05431"..
+00003200: 2020 2020 2020 2079 313d 2235 352e 3630         y1="55.60
+00003210: 3634 3431 220d 0a20 2020 2020 2020 7832  6441"..       x2
+00003220: 3d22 2d36 342e 3830 3632 3539 220d 0a20  ="-64.806259".. 
+00003230: 2020 2020 2020 7932 3d22 3535 2e36 3036        y2="55.606
+00003240: 3434 3122 0d0a 2020 2020 2020 2067 7261  441"..       gra
+00003250: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
+00003260: 5370 6163 654f 6e55 7365 220d 0a20 2020  SpaceOnUse"..   
+00003270: 2020 2020 6772 6164 6965 6e74 5472 616e      gradientTran
+00003280: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00003290: 2832 3732 2e32 3238 332c 3135 2e36 3837  (272.2283,15.687
+000032a0: 3930 3129 2220 2f3e 0d0a 2020 2020 3c6c  901)" />..    <l
+000032b0: 696e 6561 7247 7261 6469 656e 740d 0a20  inearGradient.. 
+000032c0: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
+000032d0: 4772 6164 6965 6e74 3138 3934 223e 0d0a  Gradient1894">..
+000032e0: 2020 2020 2020 3c73 746f 700d 0a20 2020        <stop..   
+000032f0: 2020 2020 2020 7374 796c 653d 2273 746f        style="sto
+00003300: 702d 636f 6c6f 723a 2366 6666 3363 653b  p-color:#fff3ce;
+00003310: 7374 6f70 2d6f 7061 6369 7479 3a31 3b22  stop-opacity:1;"
+00003320: 0d0a 2020 2020 2020 2020 206f 6666 7365  ..         offse
+00003330: 743d 2230 220d 0a20 2020 2020 2020 2020  t="0"..         
+00003340: 6964 3d22 7374 6f70 3138 3930 2220 2f3e  id="stop1890" />
+00003350: 0d0a 2020 2020 2020 3c73 746f 700d 0a20  ..      <stop.. 
+00003360: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
+00003370: 746f 702d 636f 6c6f 723a 2366 6665 3837  top-color:#ffe87
+00003380: 333b 7374 6f70 2d6f 7061 6369 7479 3a31  3;stop-opacity:1
+00003390: 220d 0a20 2020 2020 2020 2020 6f66 6673  "..         offs
+000033a0: 6574 3d22 3122 0d0a 2020 2020 2020 2020  et="1"..        
+000033b0: 2069 643d 2273 746f 7031 3839 3222 202f   id="stop1892" /
+000033c0: 3e0d 0a20 2020 203c 2f6c 696e 6561 7247  >..    </linearG
+000033d0: 7261 6469 656e 743e 0d0a 2020 3c2f 6465  radient>..  </de
+000033e0: 6673 3e0d 0a20 203c 656c 6c69 7073 650d  fs>..  <ellipse.
+000033f0: 0a20 2020 2020 7374 796c 653d 2266 696c  .     style="fil
+00003400: 6c3a 7572 6c28 236c 696e 6561 7247 7261  l:url(#linearGra
+00003410: 6469 656e 7434 3039 3729 3b66 696c 6c2d  dient4097);fill-
+00003420: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00003430: 3a6e 6f6e 653b 7374 726f 6b65 2d77 6964  :none;stroke-wid
+00003440: 7468 3a31 2e30 3632 3836 3b73 7472 6f6b  th:1.06286;strok
+00003450: 652d 6f70 6163 6974 793a 3122 0d0a 2020  e-opacity:1"..  
+00003460: 2020 2069 643d 2270 6174 6834 3038 3922     id="path4089"
+00003470: 0d0a 2020 2020 2063 783d 2231 3336 2e30  ..     cx="136.0
+00003480: 3233 3638 220d 0a20 2020 2020 6379 3d22  2368"..     cy="
+00003490: 3732 2e30 3832 3238 3322 0d0a 2020 2020  72.082283"..    
+000034a0: 2072 783d 2237 362e 3234 3930 3233 220d   rx="76.249023".
+000034b0: 0a20 2020 2020 7279 3d22 3533 2e31 3638  .     ry="53.168
+000034c0: 3336 3922 202f 3e0d 0a20 203c 656c 6c69  369" />..  <elli
+000034d0: 7073 650d 0a20 2020 2020 7374 796c 653d  pse..     style=
+000034e0: 2266 696c 6c3a 7572 6c28 236c 696e 6561  "fill:url(#linea
+000034f0: 7247 7261 6469 656e 7434 3039 372d 3429  rGradient4097-4)
+00003500: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00003510: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
+00003520: 6b65 2d6f 7061 6369 7479 3a31 220d 0a20  ke-opacity:1".. 
+00003530: 2020 2020 6964 3d22 7061 7468 3430 3839      id="path4089
+00003540: 2d32 220d 0a20 2020 2020 6378 3d22 3133  -2"..     cx="13
+00003550: 372e 3239 3830 3222 0d0a 2020 2020 2063  7.29802"..     c
+00003560: 793d 2237 312e 3239 3433 3432 220d 0a20  y="71.294342".. 
+00003570: 2020 2020 7278 3d22 3639 2e36 3234 3032      rx="69.62402
+00003580: 3322 0d0a 2020 2020 2072 793d 2235 312e  3"..     ry="51.
+00003590: 3534 3333 3639 2220 2f3e 0d0a 2020 3c70  543369" />..  <p
+000035a0: 6174 680d 0a20 2020 2020 7374 796c 653d  ath..     style=
+000035b0: 2263 6f6c 6f72 3a23 3030 3030 3030 3b66  "color:#000000;f
+000035c0: 6f6e 742d 7374 796c 653a 6e6f 726d 616c  ont-style:normal
+000035d0: 3b66 6f6e 742d 7661 7269 616e 743a 6e6f  ;font-variant:no
+000035e0: 726d 616c 3b66 6f6e 742d 7765 6967 6874  rmal;font-weight
+000035f0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d73 7472  :normal;font-str
+00003600: 6574 6368 3a6e 6f72 6d61 6c3b 666f 6e74  etch:normal;font
+00003610: 2d73 697a 653a 6d65 6469 756d 3b6c 696e  -size:medium;lin
+00003620: 652d 6865 6967 6874 3a6e 6f72 6d61 6c3b  e-height:normal;
+00003630: 666f 6e74 2d66 616d 696c 793a 5361 6e73  font-family:Sans
+00003640: 3b2d 696e 6b73 6361 7065 2d66 6f6e 742d  ;-inkscape-font-
+00003650: 7370 6563 6966 6963 6174 696f 6e3a 5361  specification:Sa
+00003660: 6e73 3b74 6578 742d 696e 6465 6e74 3a30  ns;text-indent:0
+00003670: 3b74 6578 742d 616c 6967 6e3a 7374 6172  ;text-align:star
+00003680: 743b 7465 7874 2d64 6563 6f72 6174 696f  t;text-decoratio
+00003690: 6e3a 6e6f 6e65 3b74 6578 742d 6465 636f  n:none;text-deco
+000036a0: 7261 7469 6f6e 2d6c 696e 653a 6e6f 6e65  ration-line:none
+000036b0: 3b6c 6574 7465 722d 7370 6163 696e 673a  ;letter-spacing:
+000036c0: 6e6f 726d 616c 3b77 6f72 642d 7370 6163  normal;word-spac
+000036d0: 696e 673a 6e6f 726d 616c 3b74 6578 742d  ing:normal;text-
+000036e0: 7472 616e 7366 6f72 6d3a 6e6f 6e65 3b77  transform:none;w
+000036f0: 7269 7469 6e67 2d6d 6f64 653a 6c72 2d74  riting-mode:lr-t
+00003700: 623b 6469 7265 6374 696f 6e3a 6c74 723b  b;direction:ltr;
+00003710: 6261 7365 6c69 6e65 2d73 6869 6674 3a62  baseline-shift:b
+00003720: 6173 656c 696e 653b 7465 7874 2d61 6e63  aseline;text-anc
+00003730: 686f 723a 7374 6172 743b 6469 7370 6c61  hor:start;displa
+00003740: 793a 696e 6c69 6e65 3b6f 7665 7266 6c6f  y:inline;overflo
+00003750: 773a 7669 7369 626c 653b 7669 7369 6269  w:visible;visibi
+00003760: 6c69 7479 3a76 6973 6962 6c65 3b66 696c  lity:visible;fil
+00003770: 6c3a 2362 6262 6262 623b 6669 6c6c 2d6f  l:#bbbbbb;fill-o
+00003780: 7061 6369 7479 3a31 3b66 696c 6c2d 7275  pacity:1;fill-ru
+00003790: 6c65 3a6e 6f6e 7a65 726f 3b73 7472 6f6b  le:nonzero;strok
+000037a0: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
+000037b0: 6474 683a 392e 3538 3436 323b 6d61 726b  dth:9.58462;mark
+000037c0: 6572 3a6e 6f6e 653b 656e 6162 6c65 2d62  er:none;enable-b
+000037d0: 6163 6b67 726f 756e 643a 6163 6375 6d75  ackground:accumu
+000037e0: 6c61 7465 220d 0a20 2020 2020 643d 226d  late"..     d="m
+000037f0: 2031 3337 2e36 3034 3836 2c31 382e 3338   137.60486,18.38
+00003800: 3437 3737 2063 202d 3535 2e32 3630 3535  4777 c -55.26055
+00003810: 322c 3020 2d37 372e 3431 3337 3232 2c32  2,0 -77.413722,2
+00003820: 302e 3036 3632 3436 202d 3737 2e34 3133  0.066246 -77.413
+00003830: 3732 322c 3533 2e32 3132 3033 3520 302e  722,53.212035 0.
+00003840: 3738 3933 382c 3237 2e32 3337 3035 3520  78938,27.237055 
+00003850: 3234 2e37 3739 3436 2c34 372e 3639 3431  24.77946,47.6941
+00003860: 3638 2034 362e 3932 3832 3932 2c35 352e  68 46.928292,55.
+00003870: 3530 3030 3438 2039 2e31 3939 3632 2c33  500048 9.19962,3
+00003880: 2e30 3539 3236 2033 352e 3737 3630 382c  .05926 35.77608,
+00003890: 3332 2e39 3439 3833 2034 362e 3430 3337  32.94983 46.4037
+000038a0: 312c 3332 2e39 3439 3833 2035 2e33 3133  1,32.94983 5.313
+000038b0: 3833 2c30 202d 3139 2e32 3039 3335 2c2d  83,0 -19.20935,-
+000038c0: 3230 2e32 3238 3531 202d 3133 2e32 3232  20.22851 -13.222
+000038d0: 3738 2c2d 3234 2e36 3739 3335 2035 2e34  78,-24.67935 5.4
+000038e0: 3435 3235 2c2d 342e 3034 3833 3820 3133  4525,-4.04838 13
+000038f0: 2e30 3532 3031 2c2d 342e 3031 3830 3320  .05201,-4.01803 
+00003900: 3238 2e32 3135 3638 2c2d 3130 2e37 3730  28.21568,-10.770
+00003910: 3438 2031 352e 3136 3336 372c 2d36 2e37  48 15.16367,-6.7
+00003920: 3532 3436 2034 352e 3138 3236 352c 2d32  5246 45.18265,-2
+00003930: 352e 3233 3232 3034 2034 352e 3435 3633  5.232204 45.4563
+00003940: 352c 2d35 332e 3030 3030 3438 2030 2c2d  5,-53.000048 0,-
+00003950: 3333 2e31 3435 3738 3920 2d32 312e 3130  33.145789 -21.10
+00003960: 3639 382c 2d35 332e 3231 3230 3335 202d  698,-53.212035 -
+00003970: 3736 2e33 3637 3533 2c2d 3533 2e32 3132  76.36753,-53.212
+00003980: 3033 3520 7a20 6d20 312e 3033 3937 322c  035 z m 1.03972,
+00003990: 392e 3838 3132 3031 2063 2034 362e 3032  9.881201 c 46.02
+000039a0: 3836 362c 302e 3234 3939 3939 2036 352e  866,0.249999 65.
+000039b0: 3132 3030 362c 3134 2e31 3838 3120 3635  12006,14.1881 65
+000039c0: 2e31 3230 3036 2c34 332e 3333 3038 3334  .12006,43.330834
+000039d0: 202d 312e 3034 3139 342c 3333 2e30 3533   -1.04194,33.053
+000039e0: 3538 3820 2d33 352e 3939 3632 332c 3437  588 -35.99623,47
+000039f0: 2e32 3838 3036 3820 2d36 362e 3434 3935  .288068 -66.4495
+00003a00: 2c34 372e 3534 3238 3838 202d 3330 2e34  ,47.542888 -30.4
+00003a10: 3533 3238 2c30 2e32 3534 3832 202d 3636  5328,0.25482 -66
+00003a20: 2e39 3136 3235 322c 2d31 382e 3430 3031  .916252,-18.4001
+00003a30: 3520 2d36 362e 3931 3632 3532 2c2d 3437  5 -66.916252,-47
+00003a40: 2e35 3432 3838 3820 302c 2d32 392e 3134  .542888 0,-29.14
+00003a50: 3237 3336 2032 322e 3231 3730 332c 2d34  2736 22.21703,-4
+00003a60: 332e 3538 3038 3334 2036 382e 3234 3536  3.580834 68.2456
+00003a70: 3932 2c2d 3433 2e33 3330 3833 3420 7a22  92,-43.330834 z"
+00003a80: 0d0a 2020 2020 2069 643d 2270 6174 6833  ..     id="path3
+00003a90: 3033 3222 0d0a 2020 2020 2069 6e6b 7363  032"..     inksc
+00003aa0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00003ab0: 7276 6174 7572 653d 2230 220d 0a20 2020  rvature="0"..   
+00003ac0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+00003ad0: 7970 6573 3d22 7a63 6373 737a 637a 7a63  ypes="zccsszczzc
+00003ae0: 7a7a 7a22 202f 3e0d 0a20 203c 7465 7874  zzz" />..  <text
+00003af0: 0d0a 2020 2020 2078 6d6c 3a73 7061 6365  ..     xml:space
+00003b00: 3d22 7072 6573 6572 7665 220d 0a20 2020  ="preserve"..   
+00003b10: 2020 7374 796c 653d 2266 6f6e 742d 7374    style="font-st
+00003b20: 796c 653a 6974 616c 6963 3b66 6f6e 742d  yle:italic;font-
+00003b30: 7765 6967 6874 3a62 6f6c 643b 666f 6e74  weight:bold;font
+00003b40: 2d73 697a 653a 3936 7078 3b6c 696e 652d  -size:96px;line-
+00003b50: 6865 6967 6874 3a31 2e35 3b66 6f6e 742d  height:1.5;font-
+00003b60: 6661 6d69 6c79 3a27 4365 6e74 7572 7920  family:'Century 
+00003b70: 476f 7468 6963 273b 2d69 6e6b 7363 6170  Gothic';-inkscap
+00003b80: 652d 666f 6e74 2d73 7065 6369 6669 6361  e-font-specifica
+00003b90: 7469 6f6e 3a27 4365 6e74 7572 7920 476f  tion:'Century Go
+00003ba0: 7468 6963 2042 6f6c 6420 4974 616c 6963  thic Bold Italic
+00003bb0: 273b 6c65 7474 6572 2d73 7061 6369 6e67  ';letter-spacing
+00003bc0: 3a2d 342e 3734 7078 3b66 696c 6c3a 2338  :-4.74px;fill:#8
+00003bd0: 3038 3038 303b 7374 726f 6b65 2d77 6964  08080;stroke-wid
+00003be0: 7468 3a31 332e 3430 3322 0d0a 2020 2020  th:13.403"..    
+00003bf0: 2078 3d22 3131 2e31 3534 3038 3122 0d0a   x="11.154081"..
+00003c00: 2020 2020 2079 3d22 3230 312e 3438 3737       y="201.4877
+00003c10: 220d 0a20 2020 2020 6964 3d22 7465 7874  "..     id="text
+00003c20: 3338 3022 3e3c 7473 7061 6e0d 0a20 2020  380"><tspan..   
+00003c30: 2020 2020 736f 6469 706f 6469 3a72 6f6c      sodipodi:rol
+00003c40: 653d 226c 696e 6522 0d0a 2020 2020 2020  e="line"..      
+00003c50: 2069 643d 2274 7370 616e 3337 3822 0d0a   id="tspan378"..
+00003c60: 2020 2020 2020 2078 3d22 3131 2e31 3534         x="11.154
+00003c70: 3038 3122 0d0a 2020 2020 2020 2079 3d22  081"..       y="
+00003c80: 3230 312e 3438 3737 220d 0a20 2020 2020  201.4877"..     
+00003c90: 2020 7374 796c 653d 2266 6f6e 742d 7374    style="font-st
+00003ca0: 796c 653a 6e6f 726d 616c 3b66 6f6e 742d  yle:normal;font-
+00003cb0: 7661 7269 616e 743a 6e6f 726d 616c 3b66  variant:normal;f
+00003cc0: 6f6e 742d 7765 6967 6874 3a33 3030 3b66  ont-weight:300;f
+00003cd0: 6f6e 742d 7374 7265 7463 683a 6e6f 726d  ont-stretch:norm
+00003ce0: 616c 3b66 6f6e 742d 7369 7a65 3a39 3670  al;font-size:96p
+00003cf0: 783b 666f 6e74 2d66 616d 696c 793a 436f  x;font-family:Co
+00003d00: 7262 656c 3b2d 696e 6b73 6361 7065 2d66  rbel;-inkscape-f
+00003d10: 6f6e 742d 7370 6563 6966 6963 6174 696f  ont-specificatio
+00003d20: 6e3a 2743 6f72 6265 6c20 4c69 6768 7427  n:'Corbel Light'
+00003d30: 3b66 696c 6c3a 2338 3038 3038 3022 3e67  ;fill:#808080">g
+00003d40: 7569 6461 7461 3c2f 7473 7061 6e3e 3c2f  uidata</tspan></
+00003d50: 7465 7874 3e0d 0a20 203c 670d 0a20 2020  text>..  <g..   
+00003d60: 2020 6964 3d22 6732 220d 0a20 2020 2020    id="g2"..     
+00003d70: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00003d80: 6c61 7465 2835 372e 3937 3832 3435 2c31  late(57.978245,1
+00003d90: 302e 3231 3533 3035 2922 3e0d 0a20 2020  0.215305)">..   
+00003da0: 203c 7265 6374 0d0a 2020 2020 2020 2073   <rect..       s
+00003db0: 7479 6c65 3d22 6669 6c6c 3a23 6666 6666  tyle="fill:#ffff
+00003dc0: 6666 3b66 696c 6c2d 6f70 6163 6974 793a  ff;fill-opacity:
+00003dd0: 313b 7374 726f 6b65 3a23 6263 6263 6263  1;stroke:#bcbcbc
+00003de0: 3b73 7472 6f6b 652d 7769 6474 683a 362e  ;stroke-width:6.
+00003df0: 333b 7374 726f 6b65 2d64 6173 6861 7272  3;stroke-dasharr
+00003e00: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+00003e10: 7061 6369 7479 3a31 220d 0a20 2020 2020  pacity:1"..     
+00003e20: 2020 6964 3d22 7265 6374 3122 0d0a 2020    id="rect1"..  
+00003e30: 2020 2020 2077 6964 7468 3d22 3939 2e32       width="99.2
+00003e40: 3432 3537 3722 0d0a 2020 2020 2020 2068  42577"..       h
+00003e50: 6569 6768 743d 2235 382e 3535 3035 3634  eight="58.550564
+00003e60: 220d 0a20 2020 2020 2020 783d 2232 392e  "..       x="29.
+00003e70: 3639 3834 3836 220d 0a20 2020 2020 2020  698486"..       
+00003e80: 793d 2233 312e 3830 3337 3535 220d 0a20  y="31.803755".. 
+00003e90: 2020 2020 2020 7279 3d22 362e 3535 3331        ry="6.5531
+00003ea0: 3932 3122 202f 3e0d 0a20 2020 203c 7265  921" />..    <re
+00003eb0: 6374 0d0a 2020 2020 2020 2073 7479 6c65  ct..       style
+00003ec0: 3d22 6669 6c6c 3a23 6263 6263 6263 3b66  ="fill:#bcbcbc;f
+00003ed0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00003ee0: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
+00003ef0: 2d77 6964 7468 3a31 2e36 3130 3538 3b73  -width:1.61058;s
+00003f00: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00003f10: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00003f20: 6974 793a 3122 0d0a 2020 2020 2020 2069  ity:1"..       i
+00003f30: 643d 2272 6563 7431 2d31 220d 0a20 2020  d="rect1-1"..   
+00003f40: 2020 2020 7769 6474 683d 2237 2e38 3630      width="7.860
+00003f50: 3835 3138 220d 0a20 2020 2020 2020 6865  8518"..       he
+00003f60: 6967 6874 3d22 3438 2e33 3130 3636 3922  ight="48.310669"
+00003f70: 0d0a 2020 2020 2020 2078 3d22 3933 2e38  ..       x="93.8
+00003f80: 3336 3632 3422 0d0a 2020 2020 2020 2079  36624"..       y
+00003f90: 3d22 3336 2e39 3731 3631 3122 0d0a 2020  ="36.971611"..  
+00003fa0: 2020 2020 2072 793d 2235 2e34 3037 3130       ry="5.40710
+00003fb0: 3539 2220 2f3e 0d0a 2020 2020 3c74 6578  59" />..    <tex
+00003fc0: 740d 0a20 2020 2020 2020 786d 6c3a 7370  t..       xml:sp
+00003fd0: 6163 653d 2270 7265 7365 7276 6522 0d0a  ace="preserve"..
+00003fe0: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
+00003ff0: 6e74 2d77 6569 6768 743a 626f 6c64 3b66  nt-weight:bold;f
+00004000: 6f6e 742d 7369 7a65 3a35 342e 3332 3731  ont-size:54.3271
+00004010: 7078 3b6c 696e 652d 6865 6967 6874 3a31  px;line-height:1
+00004020: 3b66 6f6e 742d 6661 6d69 6c79 3a43 6f72  ;font-family:Cor
+00004030: 6265 6c3b 2d69 6e6b 7363 6170 652d 666f  bel;-inkscape-fo
+00004040: 6e74 2d73 7065 6369 6669 6361 7469 6f6e  nt-specification
+00004050: 3a27 436f 7262 656c 2042 6f6c 6427 3b74  :'Corbel Bold';t
+00004060: 6578 742d 616c 6967 6e3a 6365 6e74 6572  ext-align:center
+00004070: 3b6c 6574 7465 722d 7370 6163 696e 673a  ;letter-spacing:
+00004080: 2d35 2e33 3830 3738 7078 3b74 6578 742d  -5.38078px;text-
+00004090: 616e 6368 6f72 3a6d 6964 646c 653b 6669  anchor:middle;fi
+000040a0: 6c6c 3a23 3338 3465 3961 3b66 696c 6c2d  ll:#384e9a;fill-
+000040b0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+000040c0: 3a6e 6f6e 653b 7374 726f 6b65 2d77 6964  :none;stroke-wid
+000040d0: 7468 3a37 2e35 3439 3838 3b73 7472 6f6b  th:7.54988;strok
+000040e0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+000040f0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00004100: 3122 0d0a 2020 2020 2020 2078 3d22 3634  1"..       x="64
+00004110: 2e30 3230 3130 3322 0d0a 2020 2020 2020  .020103"..      
+00004120: 2079 3d22 3830 2e38 3234 3733 220d 0a20   y="80.82473".. 
+00004130: 2020 2020 2020 6964 3d22 7465 7874 3122        id="text1"
+00004140: 0d0a 2020 2020 2020 2074 7261 6e73 666f  ..       transfo
+00004150: 726d 3d22 7363 616c 6528 312e 3031 3630  rm="scale(1.0160
+00004160: 3139 372c 302e 3938 3432 3332 3838 2922  197,0.98423288)"
+00004170: 3e3c 7473 7061 6e0d 0a20 2020 2020 2020  ><tspan..       
+00004180: 2020 736f 6469 706f 6469 3a72 6f6c 653d    sodipodi:role=
+00004190: 226c 696e 6522 0d0a 2020 2020 2020 2020  "line"..        
+000041a0: 2069 643d 2274 7370 616e 3122 0d0a 2020   id="tspan1"..  
+000041b0: 2020 2020 2020 2078 3d22 3631 2e33 3239         x="61.329
+000041c0: 3731 3222 0d0a 2020 2020 2020 2020 2079  712"..         y
+000041d0: 3d22 3830 2e38 3234 3733 220d 0a20 2020  ="80.82473"..   
+000041e0: 2020 2020 2020 7374 796c 653d 2266 6f6e        style="fon
+000041f0: 742d 7374 796c 653a 6e6f 726d 616c 3b66  t-style:normal;f
+00004200: 6f6e 742d 7661 7269 616e 743a 6e6f 726d  ont-variant:norm
+00004210: 616c 3b66 6f6e 742d 7765 6967 6874 3a62  al;font-weight:b
+00004220: 6f6c 643b 666f 6e74 2d73 7472 6574 6368  old;font-stretch
+00004230: 3a6e 6f72 6d61 6c3b 666f 6e74 2d66 616d  :normal;font-fam
+00004240: 696c 793a 4172 6961 6c3b 2d69 6e6b 7363  ily:Arial;-inksc
+00004250: 6170 652d 666f 6e74 2d73 7065 6369 6669  ape-font-specifi
+00004260: 6361 7469 6f6e 3a27 4172 6961 6c20 426f  cation:'Arial Bo
+00004270: 6c64 273b 6669 6c6c 3a23 3338 3465 3961  ld';fill:#384e9a
+00004280: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00004290: 7374 726f 6b65 2d77 6964 7468 3a37 2e35  stroke-width:7.5
+000042a0: 3439 3838 223e 3031 3c2f 7473 7061 6e3e  4988">01</tspan>
+000042b0: 3c2f 7465 7874 3e0d 0a20 203c 2f67 3e0d  </text>..  </g>.
+000042c0: 0a3c 2f73 7667 3e0d 0a                   .</svg>..
```

### Comparing `guidata-3.4.1/guidata/images/guidata-vertical.svg` & `guidata-3.5.0/guidata/images/guidata.svg`

 * *Files 26% similar despite different names*

```diff
@@ -1,1039 +1,1028 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
-00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
-00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
-00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
-00000070: 0a0a 3c73 7667 0a20 2020 7665 7273 696f  ..<svg.   versio
-00000080: 6e3d 2231 2e30 220a 2020 2077 6964 7468  n="1.0".   width
-00000090: 3d22 3238 3022 0a20 2020 6865 6967 6874  ="280".   height
-000000a0: 3d22 3234 3022 0a20 2020 6964 3d22 7376  ="240".   id="sv
-000000b0: 6732 220a 2020 2073 6f64 6970 6f64 693a  g2".   sodipodi:
-000000c0: 7665 7273 696f 6e3d 2230 2e33 3222 0a20  version="0.32". 
-000000d0: 2020 696e 6b73 6361 7065 3a76 6572 7369    inkscape:versi
-000000e0: 6f6e 3d22 312e 3320 2830 6531 3530 6564  on="1.3 (0e150ed
-000000f0: 3663 342c 2032 3032 332d 3037 2d32 3129  6c4, 2023-07-21)
-00000100: 220a 2020 2073 6f64 6970 6f64 693a 646f  ".   sodipodi:do
-00000110: 636e 616d 653d 2267 7569 6461 7461 2d76  cname="guidata-v
-00000120: 6572 7469 6361 6c2e 7376 6722 0a20 2020  ertical.svg".   
-00000130: 696e 6b73 6361 7065 3a6f 7574 7075 745f  inkscape:output_
-00000140: 6578 7465 6e73 696f 6e3d 226f 7267 2e69  extension="org.i
-00000150: 6e6b 7363 6170 652e 6f75 7470 7574 2e73  nkscape.output.s
-00000160: 7667 2e69 6e6b 7363 6170 6522 0a20 2020  vg.inkscape".   
-00000170: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00000180: 6669 6c65 6e61 6d65 3d22 2e2e 5c2e 2e5c  filename="..\..\
-00000190: 646f 635c 696d 6167 6573 5c67 7569 6461  doc\images\guida
-000001a0: 7461 2d76 6572 7469 6361 6c2e 706e 6722  ta-vertical.png"
-000001b0: 0a20 2020 696e 6b73 6361 7065 3a65 7870  .   inkscape:exp
-000001c0: 6f72 742d 7864 7069 3d22 3432 2e38 3537  ort-xdpi="42.857
-000001d0: 3134 3322 0a20 2020 696e 6b73 6361 7065  143".   inkscape
-000001e0: 3a65 7870 6f72 742d 7964 7069 3d22 3432  :export-ydpi="42
-000001f0: 2e38 3537 3134 3322 0a20 2020 786d 6c6e  .857143".   xmln
-00000200: 733a 696e 6b73 6361 7065 3d22 6874 7470  s:inkscape="http
-00000210: 3a2f 2f77 7777 2e69 6e6b 7363 6170 652e  ://www.inkscape.
-00000220: 6f72 672f 6e61 6d65 7370 6163 6573 2f69  org/namespaces/i
-00000230: 6e6b 7363 6170 6522 0a20 2020 786d 6c6e  nkscape".   xmln
-00000240: 733a 736f 6469 706f 6469 3d22 6874 7470  s:sodipodi="http
-00000250: 3a2f 2f73 6f64 6970 6f64 692e 736f 7572  ://sodipodi.sour
-00000260: 6365 666f 7267 652e 6e65 742f 4454 442f  ceforge.net/DTD/
-00000270: 736f 6469 706f 6469 2d30 2e64 7464 220a  sodipodi-0.dtd".
-00000280: 2020 2078 6d6c 6e73 3a78 6c69 6e6b 3d22     xmlns:xlink="
-00000290: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-000002a0: 672f 3139 3939 2f78 6c69 6e6b 220a 2020  g/1999/xlink".  
-000002b0: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f77   xmlns="http://w
-000002c0: 7777 2e77 332e 6f72 672f 3230 3030 2f73  ww.w3.org/2000/s
-000002d0: 7667 220a 2020 2078 6d6c 6e73 3a73 7667  vg".   xmlns:svg
-000002e0: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-000002f0: 6f72 672f 3230 3030 2f73 7667 220a 2020  org/2000/svg".  
-00000300: 2078 6d6c 6e73 3a72 6466 3d22 6874 7470   xmlns:rdf="http
-00000310: 3a2f 2f77 7777 2e77 332e 6f72 672f 3139  ://www.w3.org/19
-00000320: 3939 2f30 322f 3232 2d72 6466 2d73 796e  99/02/22-rdf-syn
-00000330: 7461 782d 6e73 2322 0a20 2020 786d 6c6e  tax-ns#".   xmln
-00000340: 733a 6363 3d22 6874 7470 3a2f 2f63 7265  s:cc="http://cre
-00000350: 6174 6976 6563 6f6d 6d6f 6e73 2e6f 7267  ativecommons.org
-00000360: 2f6e 7323 220a 2020 2078 6d6c 6e73 3a64  /ns#".   xmlns:d
-00000370: 633d 2268 7474 703a 2f2f 7075 726c 2e6f  c="http://purl.o
-00000380: 7267 2f64 632f 656c 656d 656e 7473 2f31  rg/dc/elements/1
-00000390: 2e31 2f22 3e0a 2020 3c6d 6574 6164 6174  .1/">.  <metadat
-000003a0: 610a 2020 2020 2069 643d 226d 6574 6164  a.     id="metad
-000003b0: 6174 6132 3139 3322 3e0a 2020 2020 3c72  ata2193">.    <r
-000003c0: 6466 3a52 4446 3e0a 2020 2020 2020 3c63  df:RDF>.      <c
-000003d0: 633a 576f 726b 0a20 2020 2020 2020 2020  c:Work.         
-000003e0: 7264 663a 6162 6f75 743d 2222 3e0a 2020  rdf:about="">.  
-000003f0: 2020 2020 2020 3c64 633a 666f 726d 6174        <dc:format
-00000400: 3e69 6d61 6765 2f73 7667 2b78 6d6c 3c2f  >image/svg+xml</
-00000410: 6463 3a66 6f72 6d61 743e 0a20 2020 2020  dc:format>.     
-00000420: 2020 203c 6463 3a74 7970 650a 2020 2020     <dc:type.    
-00000430: 2020 2020 2020 2072 6466 3a72 6573 6f75         rdf:resou
-00000440: 7263 653d 2268 7474 703a 2f2f 7075 726c  rce="http://purl
-00000450: 2e6f 7267 2f64 632f 6463 6d69 7479 7065  .org/dc/dcmitype
-00000460: 2f53 7469 6c6c 496d 6167 6522 202f 3e0a  /StillImage" />.
-00000470: 2020 2020 2020 3c2f 6363 3a57 6f72 6b3e        </cc:Work>
-00000480: 0a20 2020 203c 2f72 6466 3a52 4446 3e0a  .    </rdf:RDF>.
-00000490: 2020 3c2f 6d65 7461 6461 7461 3e0a 2020    </metadata>.  
-000004a0: 3c73 6f64 6970 6f64 693a 6e61 6d65 6476  <sodipodi:namedv
-000004b0: 6965 770a 2020 2020 2069 6e6b 7363 6170  iew.     inkscap
-000004c0: 653a 7769 6e64 6f77 2d68 6569 6768 743d  e:window-height=
-000004d0: 2231 3031 3722 0a20 2020 2020 696e 6b73  "1017".     inks
-000004e0: 6361 7065 3a77 696e 646f 772d 7769 6474  cape:window-widt
-000004f0: 683d 2231 3932 3022 0a20 2020 2020 696e  h="1920".     in
-00000500: 6b73 6361 7065 3a70 6167 6573 6861 646f  kscape:pageshado
-00000510: 773d 2232 220a 2020 2020 2069 6e6b 7363  w="2".     inksc
-00000520: 6170 653a 7061 6765 6f70 6163 6974 793d  ape:pageopacity=
-00000530: 2230 2e30 220a 2020 2020 2062 6f72 6465  "0.0".     borde
-00000540: 726f 7061 6369 7479 3d22 312e 3022 0a20  ropacity="1.0". 
-00000550: 2020 2020 626f 7264 6572 636f 6c6f 723d      bordercolor=
-00000560: 2223 3636 3636 3636 220a 2020 2020 2070  "#666666".     p
-00000570: 6167 6563 6f6c 6f72 3d22 2366 6666 6666  agecolor="#fffff
-00000580: 6622 0a20 2020 2020 6964 3d22 6261 7365  f".     id="base
-00000590: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-000005a0: 7a6f 6f6d 3d22 322e 3832 3834 3237 220a  zoom="2.828427".
-000005b0: 2020 2020 2069 6e6b 7363 6170 653a 6378       inkscape:cx
-000005c0: 3d22 3137 392e 3935 3836 3822 0a20 2020  ="179.95868".   
-000005d0: 2020 696e 6b73 6361 7065 3a63 793d 2231    inkscape:cy="1
-000005e0: 3337 2e30 3031 3934 220a 2020 2020 2069  37.00194".     i
-000005f0: 6e6b 7363 6170 653a 7769 6e64 6f77 2d78  nkscape:window-x
-00000600: 3d22 2d38 220a 2020 2020 2069 6e6b 7363  ="-8".     inksc
-00000610: 6170 653a 7769 6e64 6f77 2d79 3d22 2d38  ape:window-y="-8
-00000620: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00000630: 6375 7272 656e 742d 6c61 7965 723d 2273  current-layer="s
-00000640: 7667 3222 0a20 2020 2020 7368 6f77 6772  vg2".     showgr
-00000650: 6964 3d22 6661 6c73 6522 0a20 2020 2020  id="false".     
-00000660: 6669 742d 6d61 7267 696e 2d74 6f70 3d22  fit-margin-top="
-00000670: 3022 0a20 2020 2020 6669 742d 6d61 7267  0".     fit-marg
-00000680: 696e 2d6c 6566 743d 2230 220a 2020 2020  in-left="0".    
-00000690: 2066 6974 2d6d 6172 6769 6e2d 7269 6768   fit-margin-righ
-000006a0: 743d 2230 220a 2020 2020 2066 6974 2d6d  t="0".     fit-m
-000006b0: 6172 6769 6e2d 626f 7474 6f6d 3d22 3022  argin-bottom="0"
-000006c0: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
-000006d0: 696e 646f 772d 6d61 7869 6d69 7a65 643d  indow-maximized=
-000006e0: 2231 220a 2020 2020 2069 6e6b 7363 6170  "1".     inkscap
-000006f0: 653a 7368 6f77 7061 6765 7368 6164 6f77  e:showpageshadow
-00000700: 3d22 3222 0a20 2020 2020 696e 6b73 6361  ="2".     inksca
-00000710: 7065 3a70 6167 6563 6865 636b 6572 626f  pe:pagecheckerbo
-00000720: 6172 643d 2274 7275 6522 0a20 2020 2020  ard="true".     
-00000730: 696e 6b73 6361 7065 3a64 6573 6b63 6f6c  inkscape:deskcol
-00000740: 6f72 3d22 2364 3164 3164 3122 202f 3e0a  or="#d1d1d1" />.
-00000750: 2020 3c64 6566 730a 2020 2020 2069 643d    <defs.     id=
-00000760: 2264 6566 7334 223e 0a20 2020 203c 6d61  "defs4">.    <ma
-00000770: 726b 6572 0a20 2020 2020 2020 696e 6b73  rker.       inks
-00000780: 6361 7065 3a73 746f 636b 6964 3d22 4172  cape:stockid="Ar
-00000790: 726f 7732 4d65 6e64 220a 2020 2020 2020  row2Mend".      
-000007a0: 206f 7269 656e 743d 2261 7574 6f22 0a20   orient="auto". 
-000007b0: 2020 2020 2020 7265 6659 3d22 3022 0a20        refY="0". 
-000007c0: 2020 2020 2020 7265 6658 3d22 3022 0a20        refX="0". 
-000007d0: 2020 2020 2020 6964 3d22 4172 726f 7732        id="Arrow2
-000007e0: 4d65 6e64 220a 2020 2020 2020 2073 7479  Mend".       sty
-000007f0: 6c65 3d22 6f76 6572 666c 6f77 3a76 6973  le="overflow:vis
-00000800: 6962 6c65 223e 0a20 2020 2020 203c 7061  ible">.      <pa
-00000810: 7468 0a20 2020 2020 2020 2020 6964 3d22  th.         id="
-00000820: 7061 7468 3339 3038 220a 2020 2020 2020  path3908".      
-00000830: 2020 2073 7479 6c65 3d22 666f 6e74 2d73     style="font-s
-00000840: 697a 653a 3132 7078 3b66 696c 6c2d 7275  ize:12px;fill-ru
-00000850: 6c65 3a65 7665 6e6f 6464 3b73 7472 6f6b  le:evenodd;strok
-00000860: 652d 7769 6474 683a 302e 3632 353b 7374  e-width:0.625;st
-00000870: 726f 6b65 2d6c 696e 656a 6f69 6e3a 726f  roke-linejoin:ro
-00000880: 756e 6422 0a20 2020 2020 2020 2020 643d  und".         d=
-00000890: 224d 2038 2e37 3138 3538 3738 2c34 2e30  "M 8.7185878,4.0
-000008a0: 3333 3733 3532 202d 322e 3230 3732 3839  337352 -2.207289
-000008b0: 352c 302e 3031 3630 3133 3236 2038 2e37  5,0.01601326 8.7
-000008c0: 3138 3538 3834 2c2d 342e 3030 3137 3037  185884,-4.001707
-000008d0: 3820 6320 2d31 2e37 3435 3439 3834 2c32  8 c -1.7454984,2
-000008e0: 2e33 3732 3036 3039 202d 312e 3733 3534  .3720609 -1.7354
-000008f0: 3430 382c 352e 3631 3734 3531 3920 2d36  408,5.6174519 -6
-00000900: 652d 372c 382e 3033 3534 3433 207a 220a  e-7,8.035443 z".
-00000910: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-00000920: 726d 3d22 7363 616c 6528 2d30 2e36 2922  rm="scale(-0.6)"
-00000930: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00000940: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-00000950: 7661 7475 7265 3d22 3022 202f 3e0a 2020  vature="0" />.  
-00000960: 2020 3c2f 6d61 726b 6572 3e0a 2020 2020    </marker>.    
-00000970: 3c6d 6172 6b65 720a 2020 2020 2020 2069  <marker.       i
-00000980: 6e6b 7363 6170 653a 7374 6f63 6b69 643d  nkscape:stockid=
-00000990: 2241 7272 6f77 3153 656e 6422 0a20 2020  "Arrow1Send".   
-000009a0: 2020 2020 6f72 6965 6e74 3d22 6175 746f      orient="auto
-000009b0: 220a 2020 2020 2020 2072 6566 593d 2230  ".       refY="0
-000009c0: 220a 2020 2020 2020 2072 6566 583d 2230  ".       refX="0
-000009d0: 220a 2020 2020 2020 2069 643d 2241 7272  ".       id="Arr
-000009e0: 6f77 3153 656e 6422 0a20 2020 2020 2020  ow1Send".       
-000009f0: 7374 796c 653d 226f 7665 7266 6c6f 773a  style="overflow:
-00000a00: 7669 7369 626c 6522 3e0a 2020 2020 2020  visible">.      
-00000a10: 3c70 6174 680a 2020 2020 2020 2020 2069  <path.         i
-00000a20: 643d 2270 6174 6833 3839 3622 0a20 2020  d="path3896".   
-00000a30: 2020 2020 2020 643d 224d 2030 2c30 2035        d="M 0,0 5
-00000a40: 2c2d 3520 2d31 322e 352c 3020 352c 3520  ,-5 -12.5,0 5,5 
-00000a50: 5a22 0a20 2020 2020 2020 2020 7374 796c  Z".         styl
-00000a60: 653d 2266 696c 6c2d 7275 6c65 3a65 7665  e="fill-rule:eve
-00000a70: 6e6f 6464 3b73 7472 6f6b 653a 2330 3030  nodd;stroke:#000
-00000a80: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
-00000a90: 3a31 7074 3b6d 6172 6b65 722d 7374 6172  :1pt;marker-star
-00000aa0: 743a 6e6f 6e65 220a 2020 2020 2020 2020  t:none".        
-00000ab0: 2074 7261 6e73 666f 726d 3d22 6d61 7472   transform="matr
-00000ac0: 6978 282d 302e 322c 302c 302c 2d30 2e32  ix(-0.2,0,0,-0.2
-00000ad0: 2c2d 312e 322c 3029 220a 2020 2020 2020  ,-1.2,0)".      
-00000ae0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00000af0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-00000b00: 2230 2220 2f3e 0a20 2020 203c 2f6d 6172  "0" />.    </mar
-00000b10: 6b65 723e 0a20 2020 203c 6d61 726b 6572  ker>.    <marker
-00000b20: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00000b30: 3a73 746f 636b 6964 3d22 4172 726f 7731  :stockid="Arrow1
-00000b40: 4d65 6e64 220a 2020 2020 2020 206f 7269  Mend".       ori
-00000b50: 656e 743d 2261 7574 6f22 0a20 2020 2020  ent="auto".     
-00000b60: 2020 7265 6659 3d22 3022 0a20 2020 2020    refY="0".     
-00000b70: 2020 7265 6658 3d22 3022 0a20 2020 2020    refX="0".     
-00000b80: 2020 6964 3d22 4172 726f 7731 4d65 6e64    id="Arrow1Mend
-00000b90: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-00000ba0: 6f76 6572 666c 6f77 3a76 6973 6962 6c65  overflow:visible
-00000bb0: 223e 0a20 2020 2020 203c 7061 7468 0a20  ">.      <path. 
-00000bc0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00000bd0: 3338 3930 220a 2020 2020 2020 2020 2064  3890".         d
-00000be0: 3d22 4d20 302c 3020 352c 2d35 202d 3132  ="M 0,0 5,-5 -12
-00000bf0: 2e35 2c30 2035 2c35 205a 220a 2020 2020  .5,0 5,5 Z".    
-00000c00: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00000c10: 2d72 756c 653a 6576 656e 6f64 643b 7374  -rule:evenodd;st
-00000c20: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
-00000c30: 6f6b 652d 7769 6474 683a 3170 743b 6d61  oke-width:1pt;ma
-00000c40: 726b 6572 2d73 7461 7274 3a6e 6f6e 6522  rker-start:none"
-00000c50: 0a20 2020 2020 2020 2020 7472 616e 7366  .         transf
-00000c60: 6f72 6d3d 226d 6174 7269 7828 2d30 2e34  orm="matrix(-0.4
-00000c70: 2c30 2c30 2c2d 302e 342c 2d34 2c30 2922  ,0,0,-0.4,-4,0)"
-00000c80: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00000c90: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-00000ca0: 7661 7475 7265 3d22 3022 202f 3e0a 2020  vature="0" />.  
-00000cb0: 2020 3c2f 6d61 726b 6572 3e0a 2020 2020    </marker>.    
-00000cc0: 3c6d 6172 6b65 720a 2020 2020 2020 2069  <marker.       i
-00000cd0: 6e6b 7363 6170 653a 7374 6f63 6b69 643d  nkscape:stockid=
-00000ce0: 2241 7272 6f77 324c 656e 6422 0a20 2020  "Arrow2Lend".   
-00000cf0: 2020 2020 6f72 6965 6e74 3d22 6175 746f      orient="auto
-00000d00: 220a 2020 2020 2020 2072 6566 593d 2230  ".       refY="0
-00000d10: 220a 2020 2020 2020 2072 6566 583d 2230  ".       refX="0
-00000d20: 220a 2020 2020 2020 2069 643d 2241 7272  ".       id="Arr
-00000d30: 6f77 324c 656e 6422 0a20 2020 2020 2020  ow2Lend".       
-00000d40: 7374 796c 653d 226f 7665 7266 6c6f 773a  style="overflow:
-00000d50: 7669 7369 626c 6522 3e0a 2020 2020 2020  visible">.      
-00000d60: 3c70 6174 680a 2020 2020 2020 2020 2069  <path.         i
-00000d70: 643d 2270 6174 6833 3930 3222 0a20 2020  d="path3902".   
-00000d80: 2020 2020 2020 7374 796c 653d 2266 6f6e        style="fon
-00000d90: 742d 7369 7a65 3a31 3270 783b 6669 6c6c  t-size:12px;fill
-00000da0: 2d72 756c 653a 6576 656e 6f64 643b 7374  -rule:evenodd;st
-00000db0: 726f 6b65 2d77 6964 7468 3a30 2e36 3235  roke-width:0.625
-00000dc0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00000dd0: 3a72 6f75 6e64 220a 2020 2020 2020 2020  :round".        
-00000de0: 2064 3d22 4d20 382e 3731 3835 3837 382c   d="M 8.7185878,
-00000df0: 342e 3033 3337 3335 3220 2d32 2e32 3037  4.0337352 -2.207
-00000e00: 3238 3935 2c30 2e30 3136 3031 3332 3620  2895,0.01601326 
-00000e10: 382e 3731 3835 3838 342c 2d34 2e30 3031  8.7185884,-4.001
-00000e20: 3730 3738 2063 202d 312e 3734 3534 3938  7078 c -1.745498
-00000e30: 342c 322e 3337 3230 3630 3920 2d31 2e37  4,2.3720609 -1.7
-00000e40: 3335 3434 3038 2c35 2e36 3137 3435 3139  354408,5.6174519
-00000e50: 202d 3665 2d37 2c38 2e30 3335 3434 3320   -6e-7,8.035443 
-00000e60: 7a22 0a20 2020 2020 2020 2020 7472 616e  z".         tran
-00000e70: 7366 6f72 6d3d 226d 6174 7269 7828 2d31  sform="matrix(-1
-00000e80: 2e31 2c30 2c30 2c2d 312e 312c 2d31 2e31  .1,0,0,-1.1,-1.1
-00000e90: 2c30 2922 0a20 2020 2020 2020 2020 696e  ,0)".         in
-00000ea0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00000eb0: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
-00000ec0: 3e0a 2020 2020 3c2f 6d61 726b 6572 3e0a  >.    </marker>.
-00000ed0: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
-00000ee0: 656e 740a 2020 2020 2020 2069 643d 226c  ent.       id="l
-00000ef0: 696e 6561 7247 7261 6469 656e 7433 3831  inearGradient381
-00000f00: 3222 3e0a 2020 2020 2020 3c73 746f 700a  2">.      <stop.
-00000f10: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00000f20: 7374 6f70 2d63 6f6c 6f72 3a23 6432 6432  stop-color:#d2d2
-00000f30: 6432 3b73 746f 702d 6f70 6163 6974 793a  d2;stop-opacity:
-00000f40: 313b 220a 2020 2020 2020 2020 206f 6666  1;".         off
-00000f50: 7365 743d 2230 220a 2020 2020 2020 2020  set="0".        
-00000f60: 2069 643d 2273 746f 7033 3831 3422 202f   id="stop3814" /
-00000f70: 3e0a 2020 2020 2020 3c73 746f 700a 2020  >.      <stop.  
-00000f80: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
-00000f90: 6f70 2d63 6f6c 6f72 3a23 6666 6666 6666  op-color:#ffffff
-00000fa0: 3b73 746f 702d 6f70 6163 6974 793a 313b  ;stop-opacity:1;
-00000fb0: 220a 2020 2020 2020 2020 206f 6666 7365  ".         offse
-00000fc0: 743d 2231 220a 2020 2020 2020 2020 2069  t="1".         i
-00000fd0: 643d 2273 746f 7033 3831 3622 202f 3e0a  d="stop3816" />.
-00000fe0: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
-00000ff0: 6965 6e74 3e0a 2020 2020 3c6c 696e 6561  ient>.    <linea
-00001000: 7247 7261 6469 656e 740a 2020 2020 2020  rGradient.      
-00001010: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
-00001020: 656e 7433 3830 3222 0a20 2020 2020 2020  ent3802".       
-00001030: 696e 6b73 6361 7065 3a73 7761 7463 683d  inkscape:swatch=
-00001040: 2273 6f6c 6964 223e 0a20 2020 2020 203c  "solid">.      <
-00001050: 7374 6f70 0a20 2020 2020 2020 2020 7374  stop.         st
-00001060: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
-00001070: 2338 3038 3038 303b 7374 6f70 2d6f 7061  #808080;stop-opa
-00001080: 6369 7479 3a31 3b22 0a20 2020 2020 2020  city:1;".       
-00001090: 2020 6f66 6673 6574 3d22 3022 0a20 2020    offset="0".   
-000010a0: 2020 2020 2020 6964 3d22 7374 6f70 3338        id="stop38
-000010b0: 3034 2220 2f3e 0a20 2020 203c 2f6c 696e  04" />.    </lin
-000010c0: 6561 7247 7261 6469 656e 743e 0a20 2020  earGradient>.   
-000010d0: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
-000010e0: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
-000010f0: 6172 4772 6164 6965 6e74 3333 3530 223e  arGradient3350">
-00001100: 0a20 2020 2020 203c 7374 6f70 0a20 2020  .      <stop.   
-00001110: 2020 2020 2020 7374 796c 653d 2273 746f        style="sto
-00001120: 702d 636f 6c6f 723a 2330 3063 6232 623b  p-color:#00cb2b;
-00001130: 7374 6f70 2d6f 7061 6369 7479 3a30 2e32  stop-opacity:0.2
-00001140: 3437 3933 3338 383b 220a 2020 2020 2020  4793388;".      
-00001150: 2020 206f 6666 7365 743d 2230 220a 2020     offset="0".  
-00001160: 2020 2020 2020 2069 643d 2273 746f 7033         id="stop3
-00001170: 3335 3222 202f 3e0a 2020 2020 2020 3c73  352" />.      <s
-00001180: 746f 700a 2020 2020 2020 2020 2073 7479  top.         sty
+00000030: 226e 6f22 3f3e 0d0a 3c21 2d2d 2043 7265  "no"?>..<!-- Cre
+00000040: 6174 6564 2077 6974 6820 496e 6b73 6361  ated with Inksca
+00000050: 7065 2028 6874 7470 3a2f 2f77 7777 2e69  pe (http://www.i
+00000060: 6e6b 7363 6170 652e 6f72 672f 2920 2d2d  nkscape.org/) --
+00000070: 3e0d 0a0d 0a3c 7376 670d 0a20 2020 7665  >....<svg..   ve
+00000080: 7273 696f 6e3d 2231 2e30 220d 0a20 2020  rsion="1.0"..   
+00000090: 7769 6474 683d 2231 3533 2e35 3635 3833  width="153.56583
+000000a0: 220d 0a20 2020 6865 6967 6874 3d22 3135  "..   height="15
+000000b0: 332e 3536 3538 3322 0d0a 2020 2069 643d  3.56583"..   id=
+000000c0: 2273 7667 3222 0d0a 2020 2073 6f64 6970  "svg2"..   sodip
+000000d0: 6f64 693a 7665 7273 696f 6e3d 2230 2e33  odi:version="0.3
+000000e0: 3222 0d0a 2020 2069 6e6b 7363 6170 653a  2"..   inkscape:
+000000f0: 7665 7273 696f 6e3d 2231 2e33 2028 3065  version="1.3 (0e
+00000100: 3135 3065 6436 6334 2c20 3230 3233 2d30  150ed6c4, 2023-0
+00000110: 372d 3231 2922 0d0a 2020 2073 6f64 6970  7-21)"..   sodip
+00000120: 6f64 693a 646f 636e 616d 653d 2267 7569  odi:docname="gui
+00000130: 6461 7461 2e73 7667 220d 0a20 2020 696e  data.svg"..   in
+00000140: 6b73 6361 7065 3a6f 7574 7075 745f 6578  kscape:output_ex
+00000150: 7465 6e73 696f 6e3d 226f 7267 2e69 6e6b  tension="org.ink
+00000160: 7363 6170 652e 6f75 7470 7574 2e73 7667  scape.output.svg
+00000170: 2e69 6e6b 7363 6170 6522 0d0a 2020 2069  .inkscape"..   i
+00000180: 6e6b 7363 6170 653a 6578 706f 7274 2d66  nkscape:export-f
+00000190: 696c 656e 616d 653d 2244 3a5c 3132 392e  ilename="D:\129.
+000001a0: 706e 6722 0d0a 2020 2069 6e6b 7363 6170  png"..   inkscap
+000001b0: 653a 6578 706f 7274 2d78 6470 693d 2232  e:export-xdpi="2
+000001c0: 382e 3039 220d 0a20 2020 696e 6b73 6361  8.09"..   inksca
+000001d0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+000001e0: 3238 2e30 3922 0d0a 2020 2078 6d6c 6e73  28.09"..   xmlns
+000001f0: 3a69 6e6b 7363 6170 653d 2268 7474 703a  :inkscape="http:
+00000200: 2f2f 7777 772e 696e 6b73 6361 7065 2e6f  //www.inkscape.o
+00000210: 7267 2f6e 616d 6573 7061 6365 732f 696e  rg/namespaces/in
+00000220: 6b73 6361 7065 220d 0a20 2020 786d 6c6e  kscape"..   xmln
+00000230: 733a 736f 6469 706f 6469 3d22 6874 7470  s:sodipodi="http
+00000240: 3a2f 2f73 6f64 6970 6f64 692e 736f 7572  ://sodipodi.sour
+00000250: 6365 666f 7267 652e 6e65 742f 4454 442f  ceforge.net/DTD/
+00000260: 736f 6469 706f 6469 2d30 2e64 7464 220d  sodipodi-0.dtd".
+00000270: 0a20 2020 786d 6c6e 733a 786c 696e 6b3d  .   xmlns:xlink=
+00000280: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+00000290: 7267 2f31 3939 392f 786c 696e 6b22 0d0a  rg/1999/xlink"..
+000002a0: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
+000002b0: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
+000002c0: 2f73 7667 220d 0a20 2020 786d 6c6e 733a  /svg"..   xmlns:
+000002d0: 7376 673d 2268 7474 703a 2f2f 7777 772e  svg="http://www.
+000002e0: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
+000002f0: 0d0a 2020 2078 6d6c 6e73 3a72 6466 3d22  ..   xmlns:rdf="
+00000300: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+00000310: 672f 3139 3939 2f30 322f 3232 2d72 6466  g/1999/02/22-rdf
+00000320: 2d73 796e 7461 782d 6e73 2322 0d0a 2020  -syntax-ns#"..  
+00000330: 2078 6d6c 6e73 3a63 633d 2268 7474 703a   xmlns:cc="http:
+00000340: 2f2f 6372 6561 7469 7665 636f 6d6d 6f6e  //creativecommon
+00000350: 732e 6f72 672f 6e73 2322 0d0a 2020 2078  s.org/ns#"..   x
+00000360: 6d6c 6e73 3a64 633d 2268 7474 703a 2f2f  mlns:dc="http://
+00000370: 7075 726c 2e6f 7267 2f64 632f 656c 656d  purl.org/dc/elem
+00000380: 656e 7473 2f31 2e31 2f22 3e0d 0a20 203c  ents/1.1/">..  <
+00000390: 6d65 7461 6461 7461 0d0a 2020 2020 2069  metadata..     i
+000003a0: 643d 226d 6574 6164 6174 6132 3139 3322  d="metadata2193"
+000003b0: 3e0d 0a20 2020 203c 7264 663a 5244 463e  >..    <rdf:RDF>
+000003c0: 0d0a 2020 2020 2020 3c63 633a 576f 726b  ..      <cc:Work
+000003d0: 0d0a 2020 2020 2020 2020 2072 6466 3a61  ..         rdf:a
+000003e0: 626f 7574 3d22 223e 0d0a 2020 2020 2020  bout="">..      
+000003f0: 2020 3c64 633a 666f 726d 6174 3e69 6d61    <dc:format>ima
+00000400: 6765 2f73 7667 2b78 6d6c 3c2f 6463 3a66  ge/svg+xml</dc:f
+00000410: 6f72 6d61 743e 0d0a 2020 2020 2020 2020  ormat>..        
+00000420: 3c64 633a 7479 7065 0d0a 2020 2020 2020  <dc:type..      
+00000430: 2020 2020 2072 6466 3a72 6573 6f75 7263       rdf:resourc
+00000440: 653d 2268 7474 703a 2f2f 7075 726c 2e6f  e="http://purl.o
+00000450: 7267 2f64 632f 6463 6d69 7479 7065 2f53  rg/dc/dcmitype/S
+00000460: 7469 6c6c 496d 6167 6522 202f 3e0d 0a20  tillImage" />.. 
+00000470: 2020 2020 203c 2f63 633a 576f 726b 3e0d       </cc:Work>.
+00000480: 0a20 2020 203c 2f72 6466 3a52 4446 3e0d  .    </rdf:RDF>.
+00000490: 0a20 203c 2f6d 6574 6164 6174 613e 0d0a  .  </metadata>..
+000004a0: 2020 3c73 6f64 6970 6f64 693a 6e61 6d65    <sodipodi:name
+000004b0: 6476 6965 770d 0a20 2020 2020 696e 6b73  dview..     inks
+000004c0: 6361 7065 3a77 696e 646f 772d 6865 6967  cape:window-heig
+000004d0: 6874 3d22 3130 3137 220d 0a20 2020 2020  ht="1017"..     
+000004e0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
+000004f0: 7769 6474 683d 2231 3932 3022 0d0a 2020  width="1920"..  
+00000500: 2020 2069 6e6b 7363 6170 653a 7061 6765     inkscape:page
+00000510: 7368 6164 6f77 3d22 3222 0d0a 2020 2020  shadow="2"..    
+00000520: 2069 6e6b 7363 6170 653a 7061 6765 6f70   inkscape:pageop
+00000530: 6163 6974 793d 2230 2e30 220d 0a20 2020  acity="0.0"..   
+00000540: 2020 626f 7264 6572 6f70 6163 6974 793d    borderopacity=
+00000550: 2231 2e30 220d 0a20 2020 2020 626f 7264  "1.0"..     bord
+00000560: 6572 636f 6c6f 723d 2223 3636 3636 3636  ercolor="#666666
+00000570: 220d 0a20 2020 2020 7061 6765 636f 6c6f  "..     pagecolo
+00000580: 723d 2223 6666 6666 6666 220d 0a20 2020  r="#ffffff"..   
+00000590: 2020 6964 3d22 6261 7365 220d 0a20 2020    id="base"..   
+000005a0: 2020 696e 6b73 6361 7065 3a7a 6f6f 6d3d    inkscape:zoom=
+000005b0: 2232 2e38 3238 3432 3722 0d0a 2020 2020  "2.828427"..    
+000005c0: 2069 6e6b 7363 6170 653a 6378 3d22 312e   inkscape:cx="1.
+000005d0: 3431 3432 3133 3622 0d0a 2020 2020 2069  4142136"..     i
+000005e0: 6e6b 7363 6170 653a 6379 3d22 3934 2e32  nkscape:cy="94.2
+000005f0: 3231 3938 3322 0d0a 2020 2020 2069 6e6b  21983"..     ink
+00000600: 7363 6170 653a 7769 6e64 6f77 2d78 3d22  scape:window-x="
+00000610: 2d38 220d 0a20 2020 2020 696e 6b73 6361  -8"..     inksca
+00000620: 7065 3a77 696e 646f 772d 793d 222d 3822  pe:window-y="-8"
+00000630: 0d0a 2020 2020 2069 6e6b 7363 6170 653a  ..     inkscape:
+00000640: 6375 7272 656e 742d 6c61 7965 723d 2273  current-layer="s
+00000650: 7667 3222 0d0a 2020 2020 2073 686f 7767  vg2"..     showg
+00000660: 7269 643d 2266 616c 7365 220d 0a20 2020  rid="false"..   
+00000670: 2020 6669 742d 6d61 7267 696e 2d74 6f70    fit-margin-top
+00000680: 3d22 3022 0d0a 2020 2020 2066 6974 2d6d  ="0"..     fit-m
+00000690: 6172 6769 6e2d 6c65 6674 3d22 3022 0d0a  argin-left="0"..
+000006a0: 2020 2020 2066 6974 2d6d 6172 6769 6e2d       fit-margin-
+000006b0: 7269 6768 743d 2230 220d 0a20 2020 2020  right="0"..     
+000006c0: 6669 742d 6d61 7267 696e 2d62 6f74 746f  fit-margin-botto
+000006d0: 6d3d 2230 220d 0a20 2020 2020 696e 6b73  m="0"..     inks
+000006e0: 6361 7065 3a77 696e 646f 772d 6d61 7869  cape:window-maxi
+000006f0: 6d69 7a65 643d 2231 220d 0a20 2020 2020  mized="1"..     
+00000700: 696e 6b73 6361 7065 3a73 686f 7770 6167  inkscape:showpag
+00000710: 6573 6861 646f 773d 2232 220d 0a20 2020  eshadow="2"..   
+00000720: 2020 696e 6b73 6361 7065 3a70 6167 6563    inkscape:pagec
+00000730: 6865 636b 6572 626f 6172 643d 2274 7275  heckerboard="tru
+00000740: 6522 0d0a 2020 2020 2069 6e6b 7363 6170  e"..     inkscap
+00000750: 653a 6465 736b 636f 6c6f 723d 2223 6431  e:deskcolor="#d1
+00000760: 6431 6431 2220 2f3e 0d0a 2020 3c64 6566  d1d1" />..  <def
+00000770: 730d 0a20 2020 2020 6964 3d22 6465 6673  s..     id="defs
+00000780: 3422 3e0d 0a20 2020 203c 6d61 726b 6572  4">..    <marker
+00000790: 0d0a 2020 2020 2020 2069 6e6b 7363 6170  ..       inkscap
+000007a0: 653a 7374 6f63 6b69 643d 2241 7272 6f77  e:stockid="Arrow
+000007b0: 324d 656e 6422 0d0a 2020 2020 2020 206f  2Mend"..       o
+000007c0: 7269 656e 743d 2261 7574 6f22 0d0a 2020  rient="auto"..  
+000007d0: 2020 2020 2072 6566 593d 2230 220d 0a20       refY="0".. 
+000007e0: 2020 2020 2020 7265 6658 3d22 3022 0d0a        refX="0"..
+000007f0: 2020 2020 2020 2069 643d 2241 7272 6f77         id="Arrow
+00000800: 324d 656e 6422 0d0a 2020 2020 2020 2073  2Mend"..       s
+00000810: 7479 6c65 3d22 6f76 6572 666c 6f77 3a76  tyle="overflow:v
+00000820: 6973 6962 6c65 223e 0d0a 2020 2020 2020  isible">..      
+00000830: 3c70 6174 680d 0a20 2020 2020 2020 2020  <path..         
+00000840: 6964 3d22 7061 7468 3339 3038 220d 0a20  id="path3908".. 
+00000850: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00000860: 6f6e 742d 7369 7a65 3a31 3270 783b 6669  ont-size:12px;fi
+00000870: 6c6c 2d72 756c 653a 6576 656e 6f64 643b  ll-rule:evenodd;
+00000880: 7374 726f 6b65 2d77 6964 7468 3a30 2e36  stroke-width:0.6
+00000890: 3235 3b73 7472 6f6b 652d 6c69 6e65 6a6f  25;stroke-linejo
+000008a0: 696e 3a72 6f75 6e64 220d 0a20 2020 2020  in:round"..     
+000008b0: 2020 2020 643d 224d 2038 2e37 3138 3538      d="M 8.71858
+000008c0: 3738 2c34 2e30 3333 3733 3532 202d 322e  78,4.0337352 -2.
+000008d0: 3230 3732 3839 352c 302e 3031 3630 3133  2072895,0.016013
+000008e0: 3236 2038 2e37 3138 3538 3834 2c2d 342e  26 8.7185884,-4.
+000008f0: 3030 3137 3037 3820 6320 2d31 2e37 3435  0017078 c -1.745
+00000900: 3439 3834 2c32 2e33 3732 3036 3039 202d  4984,2.3720609 -
+00000910: 312e 3733 3534 3430 382c 352e 3631 3734  1.7354408,5.6174
+00000920: 3531 3920 2d36 652d 372c 382e 3033 3534  519 -6e-7,8.0354
+00000930: 3433 207a 220d 0a20 2020 2020 2020 2020  43 z"..         
+00000940: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
+00000950: 282d 302e 362c 2d30 2e36 2922 0d0a 2020  (-0.6,-0.6)"..  
+00000960: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00000970: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00000980: 7572 653d 2230 2220 2f3e 0d0a 2020 2020  ure="0" />..    
+00000990: 3c2f 6d61 726b 6572 3e0d 0a20 2020 203c  </marker>..    <
+000009a0: 6d61 726b 6572 0d0a 2020 2020 2020 2069  marker..       i
+000009b0: 6e6b 7363 6170 653a 7374 6f63 6b69 643d  nkscape:stockid=
+000009c0: 2241 7272 6f77 3153 656e 6422 0d0a 2020  "Arrow1Send"..  
+000009d0: 2020 2020 206f 7269 656e 743d 2261 7574       orient="aut
+000009e0: 6f22 0d0a 2020 2020 2020 2072 6566 593d  o"..       refY=
+000009f0: 2230 220d 0a20 2020 2020 2020 7265 6658  "0"..       refX
+00000a00: 3d22 3022 0d0a 2020 2020 2020 2069 643d  ="0"..       id=
+00000a10: 2241 7272 6f77 3153 656e 6422 0d0a 2020  "Arrow1Send"..  
+00000a20: 2020 2020 2073 7479 6c65 3d22 6f76 6572       style="over
+00000a30: 666c 6f77 3a76 6973 6962 6c65 223e 0d0a  flow:visible">..
+00000a40: 2020 2020 2020 3c70 6174 680d 0a20 2020        <path..   
+00000a50: 2020 2020 2020 6964 3d22 7061 7468 3338        id="path38
+00000a60: 3936 220d 0a20 2020 2020 2020 2020 643d  96"..         d=
+00000a70: 224d 2030 2c30 2035 2c2d 3520 2d31 322e  "M 0,0 5,-5 -12.
+00000a80: 352c 3020 352c 3520 302c 3020 7a22 0d0a  5,0 5,5 0,0 z"..
+00000a90: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00000aa0: 6669 6c6c 2d72 756c 653a 6576 656e 6f64  fill-rule:evenod
+00000ab0: 643b 7374 726f 6b65 3a23 3030 3030 3030  d;stroke:#000000
+00000ac0: 3b73 7472 6f6b 652d 7769 6474 683a 3170  ;stroke-width:1p
+00000ad0: 743b 6d61 726b 6572 2d73 7461 7274 3a6e  t;marker-start:n
+00000ae0: 6f6e 6522 0d0a 2020 2020 2020 2020 2074  one"..         t
+00000af0: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+00000b00: 282d 302e 322c 302c 302c 2d30 2e32 2c2d  (-0.2,0,0,-0.2,-
+00000b10: 312e 322c 3029 220d 0a20 2020 2020 2020  1.2,0)"..       
+00000b20: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+00000b30: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+00000b40: 3022 202f 3e0d 0a20 2020 203c 2f6d 6172  0" />..    </mar
+00000b50: 6b65 723e 0d0a 2020 2020 3c6d 6172 6b65  ker>..    <marke
+00000b60: 720d 0a20 2020 2020 2020 696e 6b73 6361  r..       inksca
+00000b70: 7065 3a73 746f 636b 6964 3d22 4172 726f  pe:stockid="Arro
+00000b80: 7731 4d65 6e64 220d 0a20 2020 2020 2020  w1Mend"..       
+00000b90: 6f72 6965 6e74 3d22 6175 746f 220d 0a20  orient="auto".. 
+00000ba0: 2020 2020 2020 7265 6659 3d22 3022 0d0a        refY="0"..
+00000bb0: 2020 2020 2020 2072 6566 583d 2230 220d         refX="0".
+00000bc0: 0a20 2020 2020 2020 6964 3d22 4172 726f  .       id="Arro
+00000bd0: 7731 4d65 6e64 220d 0a20 2020 2020 2020  w1Mend"..       
+00000be0: 7374 796c 653d 226f 7665 7266 6c6f 773a  style="overflow:
+00000bf0: 7669 7369 626c 6522 3e0d 0a20 2020 2020  visible">..     
+00000c00: 203c 7061 7468 0d0a 2020 2020 2020 2020   <path..        
+00000c10: 2069 643d 2270 6174 6833 3839 3022 0d0a   id="path3890"..
+00000c20: 2020 2020 2020 2020 2064 3d22 4d20 302c           d="M 0,
+00000c30: 3020 352c 2d35 202d 3132 2e35 2c30 2035  0 5,-5 -12.5,0 5
+00000c40: 2c35 2030 2c30 207a 220d 0a20 2020 2020  ,5 0,0 z"..     
+00000c50: 2020 2020 7374 796c 653d 2266 696c 6c2d      style="fill-
+00000c60: 7275 6c65 3a65 7665 6e6f 6464 3b73 7472  rule:evenodd;str
+00000c70: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
+00000c80: 6b65 2d77 6964 7468 3a31 7074 3b6d 6172  ke-width:1pt;mar
+00000c90: 6b65 722d 7374 6172 743a 6e6f 6e65 220d  ker-start:none".
+00000ca0: 0a20 2020 2020 2020 2020 7472 616e 7366  .         transf
+00000cb0: 6f72 6d3d 226d 6174 7269 7828 2d30 2e34  orm="matrix(-0.4
+00000cc0: 2c30 2c30 2c2d 302e 342c 2d34 2c30 2922  ,0,0,-0.4,-4,0)"
+00000cd0: 0d0a 2020 2020 2020 2020 2069 6e6b 7363  ..         inksc
+00000ce0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00000cf0: 7276 6174 7572 653d 2230 2220 2f3e 0d0a  rvature="0" />..
+00000d00: 2020 2020 3c2f 6d61 726b 6572 3e0d 0a20      </marker>.. 
+00000d10: 2020 203c 6d61 726b 6572 0d0a 2020 2020     <marker..    
+00000d20: 2020 2069 6e6b 7363 6170 653a 7374 6f63     inkscape:stoc
+00000d30: 6b69 643d 2241 7272 6f77 324c 656e 6422  kid="Arrow2Lend"
+00000d40: 0d0a 2020 2020 2020 206f 7269 656e 743d  ..       orient=
+00000d50: 2261 7574 6f22 0d0a 2020 2020 2020 2072  "auto"..       r
+00000d60: 6566 593d 2230 220d 0a20 2020 2020 2020  efY="0"..       
+00000d70: 7265 6658 3d22 3022 0d0a 2020 2020 2020  refX="0"..      
+00000d80: 2069 643d 2241 7272 6f77 324c 656e 6422   id="Arrow2Lend"
+00000d90: 0d0a 2020 2020 2020 2073 7479 6c65 3d22  ..       style="
+00000da0: 6f76 6572 666c 6f77 3a76 6973 6962 6c65  overflow:visible
+00000db0: 223e 0d0a 2020 2020 2020 3c70 6174 680d  ">..      <path.
+00000dc0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+00000dd0: 7468 3339 3032 220d 0a20 2020 2020 2020  th3902"..       
+00000de0: 2020 7374 796c 653d 2266 6f6e 742d 7369    style="font-si
+00000df0: 7a65 3a31 3270 783b 6669 6c6c 2d72 756c  ze:12px;fill-rul
+00000e00: 653a 6576 656e 6f64 643b 7374 726f 6b65  e:evenodd;stroke
+00000e10: 2d77 6964 7468 3a30 2e36 3235 3b73 7472  -width:0.625;str
+00000e20: 6f6b 652d 6c69 6e65 6a6f 696e 3a72 6f75  oke-linejoin:rou
+00000e30: 6e64 220d 0a20 2020 2020 2020 2020 643d  nd"..         d=
+00000e40: 224d 2038 2e37 3138 3538 3738 2c34 2e30  "M 8.7185878,4.0
+00000e50: 3333 3733 3532 202d 322e 3230 3732 3839  337352 -2.207289
+00000e60: 352c 302e 3031 3630 3133 3236 2038 2e37  5,0.01601326 8.7
+00000e70: 3138 3538 3834 2c2d 342e 3030 3137 3037  185884,-4.001707
+00000e80: 3820 6320 2d31 2e37 3435 3439 3834 2c32  8 c -1.7454984,2
+00000e90: 2e33 3732 3036 3039 202d 312e 3733 3534  .3720609 -1.7354
+00000ea0: 3430 382c 352e 3631 3734 3531 3920 2d36  408,5.6174519 -6
+00000eb0: 652d 372c 382e 3033 3534 3433 207a 220d  e-7,8.035443 z".
+00000ec0: 0a20 2020 2020 2020 2020 7472 616e 7366  .         transf
+00000ed0: 6f72 6d3d 226d 6174 7269 7828 2d31 2e31  orm="matrix(-1.1
+00000ee0: 2c30 2c30 2c2d 312e 312c 2d31 2e31 2c30  ,0,0,-1.1,-1.1,0
+00000ef0: 2922 0d0a 2020 2020 2020 2020 2069 6e6b  )"..         ink
+00000f00: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00000f10: 6375 7276 6174 7572 653d 2230 2220 2f3e  curvature="0" />
+00000f20: 0d0a 2020 2020 3c2f 6d61 726b 6572 3e0d  ..    </marker>.
+00000f30: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
+00000f40: 6965 6e74 0d0a 2020 2020 2020 2069 643d  ient..       id=
+00000f50: 226c 696e 6561 7247 7261 6469 656e 7433  "linearGradient3
+00000f60: 3831 3222 3e0d 0a20 2020 2020 203c 7374  812">..      <st
+00000f70: 6f70 0d0a 2020 2020 2020 2020 2073 7479  op..         sty
+00000f80: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
+00000f90: 6432 6432 6432 3b73 746f 702d 6f70 6163  d2d2d2;stop-opac
+00000fa0: 6974 793a 313b 220d 0a20 2020 2020 2020  ity:1;"..       
+00000fb0: 2020 6f66 6673 6574 3d22 3022 0d0a 2020    offset="0"..  
+00000fc0: 2020 2020 2020 2069 643d 2273 746f 7033         id="stop3
+00000fd0: 3831 3422 202f 3e0d 0a20 2020 2020 203c  814" />..      <
+00000fe0: 7374 6f70 0d0a 2020 2020 2020 2020 2073  stop..         s
+00000ff0: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
+00001000: 3a23 6666 6666 6666 3b73 746f 702d 6f70  :#ffffff;stop-op
+00001010: 6163 6974 793a 313b 220d 0a20 2020 2020  acity:1;"..     
+00001020: 2020 2020 6f66 6673 6574 3d22 3122 0d0a      offset="1"..
+00001030: 2020 2020 2020 2020 2069 643d 2273 746f           id="sto
+00001040: 7033 3831 3622 202f 3e0d 0a20 2020 203c  p3816" />..    <
+00001050: 2f6c 696e 6561 7247 7261 6469 656e 743e  /linearGradient>
+00001060: 0d0a 2020 2020 3c6c 696e 6561 7247 7261  ..    <linearGra
+00001070: 6469 656e 740d 0a20 2020 2020 2020 6964  dient..       id
+00001080: 3d22 6c69 6e65 6172 4772 6164 6965 6e74  ="linearGradient
+00001090: 3338 3032 220d 0a20 2020 2020 2020 696e  3802"..       in
+000010a0: 6b73 6361 7065 3a73 7761 7463 683d 2273  kscape:swatch="s
+000010b0: 6f6c 6964 223e 0d0a 2020 2020 2020 3c73  olid">..      <s
+000010c0: 746f 700d 0a20 2020 2020 2020 2020 7374  top..         st
+000010d0: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
+000010e0: 2338 3038 3038 303b 7374 6f70 2d6f 7061  #808080;stop-opa
+000010f0: 6369 7479 3a31 3b22 0d0a 2020 2020 2020  city:1;"..      
+00001100: 2020 206f 6666 7365 743d 2230 220d 0a20     offset="0".. 
+00001110: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
+00001120: 3338 3034 2220 2f3e 0d0a 2020 2020 3c2f  3804" />..    </
+00001130: 6c69 6e65 6172 4772 6164 6965 6e74 3e0d  linearGradient>.
+00001140: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
+00001150: 6965 6e74 0d0a 2020 2020 2020 2069 643d  ient..       id=
+00001160: 226c 696e 6561 7247 7261 6469 656e 7433  "linearGradient3
+00001170: 3335 3022 3e0d 0a20 2020 2020 203c 7374  350">..      <st
+00001180: 6f70 0d0a 2020 2020 2020 2020 2073 7479  op..         sty
 00001190: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
 000011a0: 3030 6362 3262 3b73 746f 702d 6f70 6163  00cb2b;stop-opac
-000011b0: 6974 793a 313b 220a 2020 2020 2020 2020  ity:1;".        
-000011c0: 206f 6666 7365 743d 2231 220a 2020 2020   offset="1".    
-000011d0: 2020 2020 2069 643d 2273 746f 7033 3335       id="stop335
-000011e0: 3422 202f 3e0a 2020 2020 3c2f 6c69 6e65  4" />.    </line
-000011f0: 6172 4772 6164 6965 6e74 3e0a 2020 2020  arGradient>.    
-00001200: 3c6c 696e 6561 7247 7261 6469 656e 740a  <linearGradient.
-00001210: 2020 2020 2020 2069 643d 226c 696e 6561         id="linea
-00001220: 7247 7261 6469 656e 7433 3334 3222 3e0a  rGradient3342">.
-00001230: 2020 2020 2020 3c73 746f 700a 2020 2020        <stop.    
-00001240: 2020 2020 2073 7479 6c65 3d22 7374 6f70       style="stop
-00001250: 2d63 6f6c 6f72 3a23 3030 3561 3835 3b73  -color:#005a85;s
-00001260: 746f 702d 6f70 6163 6974 793a 313b 220a  top-opacity:1;".
-00001270: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
-00001280: 2230 220a 2020 2020 2020 2020 2069 643d  "0".         id=
-00001290: 2273 746f 7033 3334 3422 202f 3e0a 2020  "stop3344" />.  
-000012a0: 2020 2020 3c73 746f 700a 2020 2020 2020      <stop.      
-000012b0: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
-000012c0: 6f6c 6f72 3a23 3030 3561 3835 3b73 746f  olor:#005a85;sto
-000012d0: 702d 6f70 6163 6974 793a 302e 3735 3230  p-opacity:0.7520
-000012e0: 3636 3134 3b22 0a20 2020 2020 2020 2020  6614;".         
-000012f0: 6f66 6673 6574 3d22 3122 0a20 2020 2020  offset="1".     
-00001300: 2020 2020 6964 3d22 7374 6f70 3333 3436      id="stop3346
-00001310: 2220 2f3e 0a20 2020 203c 2f6c 696e 6561  " />.    </linea
-00001320: 7247 7261 6469 656e 743e 0a20 2020 203c  rGradient>.    <
-00001330: 6c69 6e65 6172 4772 6164 6965 6e74 0a20  linearGradient. 
-00001340: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
-00001350: 4772 6164 6965 6e74 3333 3130 223e 0a20  Gradient3310">. 
-00001360: 2020 2020 203c 7374 6f70 0a20 2020 2020       <stop.     
-00001370: 2020 2020 6964 3d22 7374 6f70 3333 3132      id="stop3312
-00001380: 220a 2020 2020 2020 2020 206f 6666 7365  ".         offse
-00001390: 743d 2230 220a 2020 2020 2020 2020 2073  t="0".         s
-000013a0: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
-000013b0: 3a23 6165 3032 3032 3b73 746f 702d 6f70  :#ae0202;stop-op
-000013c0: 6163 6974 793a 313b 2220 2f3e 0a20 2020  acity:1;" />.   
-000013d0: 2020 203c 7374 6f70 0a20 2020 2020 2020     <stop.       
-000013e0: 2020 6964 3d22 7374 6f70 3333 3134 220a    id="stop3314".
-000013f0: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
-00001400: 2231 220a 2020 2020 2020 2020 2073 7479  "1".         sty
-00001410: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
-00001420: 6234 3735 3735 3b73 746f 702d 6f70 6163  b47575;stop-opac
-00001430: 6974 793a 313b 2220 2f3e 0a20 2020 203c  ity:1;" />.    <
-00001440: 2f6c 696e 6561 7247 7261 6469 656e 743e  /linearGradient>
-00001450: 0a20 2020 203c 696e 6b73 6361 7065 3a70  .    <inkscape:p
-00001460: 6572 7370 6563 7469 7665 0a20 2020 2020  erspective.     
-00001470: 2020 736f 6469 706f 6469 3a74 7970 653d    sodipodi:type=
-00001480: 2269 6e6b 7363 6170 653a 7065 7273 7033  "inkscape:persp3
-00001490: 6422 0a20 2020 2020 2020 696e 6b73 6361  d".       inksca
-000014a0: 7065 3a76 705f 783d 2230 203a 2031 3538  pe:vp_x="0 : 158
-000014b0: 2e33 3231 3636 203a 2031 220a 2020 2020  .32166 : 1".    
-000014c0: 2020 2069 6e6b 7363 6170 653a 7670 5f79     inkscape:vp_y
-000014d0: 3d22 3020 3a20 3130 3030 203a 2030 220a  ="0 : 1000 : 0".
-000014e0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-000014f0: 7670 5f7a 3d22 3438 362e 3034 3939 3920  vp_z="486.04999 
-00001500: 3a20 3135 382e 3332 3136 3620 3a20 3122  : 158.32166 : 1"
-00001510: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00001520: 3a70 6572 7370 3364 2d6f 7269 6769 6e3d  :persp3d-origin=
-00001530: 2232 3433 2e30 3234 3939 203a 2031 3334  "243.02499 : 134
-00001540: 2e33 3539 3137 203a 2031 220a 2020 2020  .35917 : 1".    
-00001550: 2020 2069 643d 2270 6572 7370 6563 7469     id="perspecti
-00001560: 7665 3437 2220 2f3e 0a20 2020 203c 6c69  ve47" />.    <li
-00001570: 6e65 6172 4772 6164 6965 6e74 0a20 2020  nearGradient.   
-00001580: 2020 2020 6964 3d22 6c69 6e65 6172 4772      id="linearGr
-00001590: 6164 6965 6e74 3237 3935 223e 0a20 2020  adient2795">.   
-000015a0: 2020 203c 7374 6f70 0a20 2020 2020 2020     <stop.       
-000015b0: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
-000015c0: 6c6f 723a 2362 3862 3862 383b 7374 6f70  lor:#b8b8b8;stop
-000015d0: 2d6f 7061 6369 7479 3a30 2e34 3938 3033  -opacity:0.49803
-000015e0: 3932 3222 0a20 2020 2020 2020 2020 6f66  922".         of
-000015f0: 6673 6574 3d22 3022 0a20 2020 2020 2020  fset="0".       
-00001600: 2020 6964 3d22 7374 6f70 3237 3937 2220    id="stop2797" 
-00001610: 2f3e 0a20 2020 2020 203c 7374 6f70 0a20  />.      <stop. 
-00001620: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
-00001630: 746f 702d 636f 6c6f 723a 2337 6637 6637  top-color:#7f7f7
-00001640: 663b 7374 6f70 2d6f 7061 6369 7479 3a30  f;stop-opacity:0
-00001650: 220a 2020 2020 2020 2020 206f 6666 7365  ".         offse
-00001660: 743d 2231 220a 2020 2020 2020 2020 2069  t="1".         i
-00001670: 643d 2273 746f 7032 3739 3922 202f 3e0a  d="stop2799" />.
-00001680: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
-00001690: 6965 6e74 3e0a 2020 2020 3c6c 696e 6561  ient>.    <linea
-000016a0: 7247 7261 6469 656e 740a 2020 2020 2020  rGradient.      
-000016b0: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
-000016c0: 656e 7432 3738 3722 3e0a 2020 2020 2020  ent2787">.      
-000016d0: 3c73 746f 700a 2020 2020 2020 2020 2073  <stop.         s
-000016e0: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
-000016f0: 3a23 3766 3766 3766 3b73 746f 702d 6f70  :#7f7f7f;stop-op
-00001700: 6163 6974 793a 302e 3522 0a20 2020 2020  acity:0.5".     
-00001710: 2020 2020 6f66 6673 6574 3d22 3022 0a20      offset="0". 
-00001720: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
-00001730: 3237 3839 2220 2f3e 0a20 2020 2020 203c  2789" />.      <
-00001740: 7374 6f70 0a20 2020 2020 2020 2020 7374  stop.         st
-00001750: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
-00001760: 2337 6637 6637 663b 7374 6f70 2d6f 7061  #7f7f7f;stop-opa
-00001770: 6369 7479 3a30 220a 2020 2020 2020 2020  city:0".        
-00001780: 206f 6666 7365 743d 2231 220a 2020 2020   offset="1".    
-00001790: 2020 2020 2069 643d 2273 746f 7032 3739       id="stop279
-000017a0: 3122 202f 3e0a 2020 2020 3c2f 6c69 6e65  1" />.    </line
-000017b0: 6172 4772 6164 6965 6e74 3e0a 2020 2020  arGradient>.    
-000017c0: 3c6c 696e 6561 7247 7261 6469 656e 740a  <linearGradient.
-000017d0: 2020 2020 2020 2069 643d 226c 696e 6561         id="linea
-000017e0: 7247 7261 6469 656e 7433 3637 3622 3e0a  rGradient3676">.
-000017f0: 2020 2020 2020 3c73 746f 700a 2020 2020        <stop.    
-00001800: 2020 2020 2073 7479 6c65 3d22 7374 6f70       style="stop
-00001810: 2d63 6f6c 6f72 3a23 6232 6232 6232 3b73  -color:#b2b2b2;s
-00001820: 746f 702d 6f70 6163 6974 793a 302e 3522  top-opacity:0.5"
-00001830: 0a20 2020 2020 2020 2020 6f66 6673 6574  .         offset
-00001840: 3d22 3022 0a20 2020 2020 2020 2020 6964  ="0".         id
-00001850: 3d22 7374 6f70 3336 3738 2220 2f3e 0a20  ="stop3678" />. 
-00001860: 2020 2020 203c 7374 6f70 0a20 2020 2020       <stop.     
-00001870: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
-00001880: 636f 6c6f 723a 2362 3362 3362 333b 7374  color:#b3b3b3;st
-00001890: 6f70 2d6f 7061 6369 7479 3a30 220a 2020  op-opacity:0".  
-000018a0: 2020 2020 2020 206f 6666 7365 743d 2231         offset="1
-000018b0: 220a 2020 2020 2020 2020 2069 643d 2273  ".         id="s
-000018c0: 746f 7033 3638 3022 202f 3e0a 2020 2020  top3680" />.    
-000018d0: 3c2f 6c69 6e65 6172 4772 6164 6965 6e74  </linearGradient
-000018e0: 3e0a 2020 2020 3c6c 696e 6561 7247 7261  >.    <linearGra
-000018f0: 6469 656e 740a 2020 2020 2020 2069 643d  dient.       id=
-00001900: 226c 696e 6561 7247 7261 6469 656e 7433  "linearGradient3
-00001910: 3233 3622 3e0a 2020 2020 2020 3c73 746f  236">.      <sto
-00001920: 700a 2020 2020 2020 2020 2073 7479 6c65  p.         style
-00001930: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 6634  ="stop-color:#f4
-00001940: 6634 6634 3b73 746f 702d 6f70 6163 6974  f4f4;stop-opacit
-00001950: 793a 3122 0a20 2020 2020 2020 2020 6f66  y:1".         of
-00001960: 6673 6574 3d22 3022 0a20 2020 2020 2020  fset="0".       
-00001970: 2020 6964 3d22 7374 6f70 3332 3434 2220    id="stop3244" 
-00001980: 2f3e 0a20 2020 2020 203c 7374 6f70 0a20  />.      <stop. 
-00001990: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
-000019a0: 746f 702d 636f 6c6f 723a 2366 6666 6666  top-color:#fffff
-000019b0: 663b 7374 6f70 2d6f 7061 6369 7479 3a31  f;stop-opacity:1
-000019c0: 220a 2020 2020 2020 2020 206f 6666 7365  ".         offse
-000019d0: 743d 2231 220a 2020 2020 2020 2020 2069  t="1".         i
-000019e0: 643d 2273 746f 7033 3234 3022 202f 3e0a  d="stop3240" />.
-000019f0: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
-00001a00: 6965 6e74 3e0a 2020 2020 3c6c 696e 6561  ient>.    <linea
-00001a10: 7247 7261 6469 656e 740a 2020 2020 2020  rGradient.      
-00001a20: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
-00001a30: 656e 7434 3637 3122 3e0a 2020 2020 2020  ent4671">.      
-00001a40: 3c73 746f 700a 2020 2020 2020 2020 2073  <stop.         s
-00001a50: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
-00001a60: 3a23 6666 6434 3362 3b73 746f 702d 6f70  :#ffd43b;stop-op
-00001a70: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00001a80: 2020 6f66 6673 6574 3d22 3022 0a20 2020    offset="0".   
-00001a90: 2020 2020 2020 6964 3d22 7374 6f70 3436        id="stop46
-00001aa0: 3733 2220 2f3e 0a20 2020 2020 203c 7374  73" />.      <st
-00001ab0: 6f70 0a20 2020 2020 2020 2020 7374 796c  op.         styl
-00001ac0: 653d 2273 746f 702d 636f 6c6f 723a 2366  e="stop-color:#f
-00001ad0: 6665 3837 333b 7374 6f70 2d6f 7061 6369  fe873;stop-opaci
-00001ae0: 7479 3a31 220a 2020 2020 2020 2020 206f  ty:1".         o
-00001af0: 6666 7365 743d 2231 220a 2020 2020 2020  ffset="1".      
-00001b00: 2020 2069 643d 2273 746f 7034 3637 3522     id="stop4675"
-00001b10: 202f 3e0a 2020 2020 3c2f 6c69 6e65 6172   />.    </linear
-00001b20: 4772 6164 6965 6e74 3e0a 2020 2020 3c6c  Gradient>.    <l
-00001b30: 696e 6561 7247 7261 6469 656e 740a 2020  inearGradient.  
-00001b40: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
-00001b50: 7261 6469 656e 7434 3638 3922 3e0a 2020  radient4689">.  
-00001b60: 2020 2020 3c73 746f 700a 2020 2020 2020      <stop.      
-00001b70: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
-00001b80: 6f6c 6f72 3a23 3561 3966 6434 3b73 746f  olor:#5a9fd4;sto
-00001b90: 702d 6f70 6163 6974 793a 3122 0a20 2020  p-opacity:1".   
-00001ba0: 2020 2020 2020 6f66 6673 6574 3d22 3022        offset="0"
-00001bb0: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
-00001bc0: 6f70 3436 3931 2220 2f3e 0a20 2020 2020  op4691" />.     
-00001bd0: 203c 7374 6f70 0a20 2020 2020 2020 2020   <stop.         
-00001be0: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
-00001bf0: 723a 2333 3036 3939 383b 7374 6f70 2d6f  r:#306998;stop-o
-00001c00: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00001c10: 2020 206f 6666 7365 743d 2231 220a 2020     offset="1".  
-00001c20: 2020 2020 2020 2069 643d 2273 746f 7034         id="stop4
-00001c30: 3639 3322 202f 3e0a 2020 2020 3c2f 6c69  693" />.    </li
-00001c40: 6e65 6172 4772 6164 6965 6e74 3e0a 2020  nearGradient>.  
-00001c50: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
-00001c60: 740a 2020 2020 2020 2078 313d 2232 3234  t.       x1="224
-00001c70: 2e32 3339 3936 220a 2020 2020 2020 2079  .23996".       y
-00001c80: 313d 2231 3434 2e37 3537 3137 220a 2020  1="144.75717".  
-00001c90: 2020 2020 2078 323d 222d 3635 2e33 3038       x2="-65.308
-00001ca0: 3530 3222 0a20 2020 2020 2020 7932 3d22  502".       y2="
-00001cb0: 3134 342e 3735 3731 3722 0a20 2020 2020  144.75717".     
-00001cc0: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
-00001cd0: 6965 6e74 3239 3837 220a 2020 2020 2020  ient2987".      
-00001ce0: 2078 6c69 6e6b 3a68 7265 663d 2223 6c69   xlink:href="#li
-00001cf0: 6e65 6172 4772 6164 6965 6e74 3436 3731  nearGradient4671
-00001d00: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
-00001d10: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
-00001d20: 654f 6e55 7365 220a 2020 2020 2020 2067  eOnUse".       g
-00001d30: 7261 6469 656e 7454 7261 6e73 666f 726d  radientTransform
-00001d40: 3d22 7472 616e 736c 6174 6528 3130 302e  ="translate(100.
-00001d50: 3237 3032 2c39 392e 3631 3131 3629 2220  2702,99.61116)" 
-00001d60: 2f3e 0a20 2020 203c 6c69 6e65 6172 4772  />.    <linearGr
-00001d70: 6164 6965 6e74 0a20 2020 2020 2020 7831  adient.       x1
-00001d80: 3d22 3137 322e 3934 3230 3822 0a20 2020  ="172.94208".   
-00001d90: 2020 2020 7931 3d22 3737 2e34 3735 3938      y1="77.47598
-00001da0: 3322 0a20 2020 2020 2020 7832 3d22 3236  3".       x2="26
-00001db0: 2e36 3730 3239 3822 0a20 2020 2020 2020  .670298".       
-00001dc0: 7932 3d22 3736 2e33 3133 3133 3322 0a20  y2="76.313133". 
-00001dd0: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
-00001de0: 4772 6164 6965 6e74 3239 3930 220a 2020  Gradient2990".  
-00001df0: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
-00001e00: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
-00001e10: 3436 3839 220a 2020 2020 2020 2067 7261  4689".       gra
-00001e20: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
-00001e30: 5370 6163 654f 6e55 7365 220a 2020 2020  SpaceOnUse".    
-00001e40: 2020 2067 7261 6469 656e 7454 7261 6e73     gradientTrans
-00001e50: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00001e60: 3130 302e 3237 3032 2c39 392e 3631 3131  100.2702,99.6111
-00001e70: 3629 2220 2f3e 0a20 2020 203c 6c69 6e65  6)" />.    <line
-00001e80: 6172 4772 6164 6965 6e74 0a20 2020 2020  arGradient.     
-00001e90: 2020 7831 3d22 3137 322e 3934 3230 3822    x1="172.94208"
-00001ea0: 0a20 2020 2020 2020 7931 3d22 3737 2e34  .       y1="77.4
-00001eb0: 3735 3938 3322 0a20 2020 2020 2020 7832  75983".       x2
-00001ec0: 3d22 3236 2e36 3730 3239 3822 0a20 2020  ="26.670298".   
-00001ed0: 2020 2020 7932 3d22 3736 2e33 3133 3133      y2="76.31313
-00001ee0: 3322 0a20 2020 2020 2020 6964 3d22 6c69  3".       id="li
-00001ef0: 6e65 6172 4772 6164 6965 6e74 3235 3837  nearGradient2587
-00001f00: 220a 2020 2020 2020 2078 6c69 6e6b 3a68  ".       xlink:h
-00001f10: 7265 663d 2223 6c69 6e65 6172 4772 6164  ref="#linearGrad
-00001f20: 6965 6e74 3436 3839 220a 2020 2020 2020  ient4689".      
-00001f30: 2067 7261 6469 656e 7455 6e69 7473 3d22   gradientUnits="
-00001f40: 7573 6572 5370 6163 654f 6e55 7365 220a  userSpaceOnUse".
-00001f50: 2020 2020 2020 2067 7261 6469 656e 7454         gradientT
-00001f60: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00001f70: 6174 6528 3130 302e 3237 3032 2c39 392e  ate(100.2702,99.
-00001f80: 3631 3131 3629 2220 2f3e 0a20 2020 203c  61116)" />.    <
-00001f90: 6c69 6e65 6172 4772 6164 6965 6e74 0a20  linearGradient. 
-00001fa0: 2020 2020 2020 7831 3d22 3232 342e 3233        x1="224.23
-00001fb0: 3939 3622 0a20 2020 2020 2020 7931 3d22  996".       y1="
-00001fc0: 3134 342e 3735 3731 3722 0a20 2020 2020  144.75717".     
-00001fd0: 2020 7832 3d22 2d36 352e 3330 3835 3032    x2="-65.308502
-00001fe0: 220a 2020 2020 2020 2079 323d 2231 3434  ".       y2="144
-00001ff0: 2e37 3537 3137 220a 2020 2020 2020 2069  .75717".       i
-00002000: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
-00002010: 7432 3538 3922 0a20 2020 2020 2020 786c  t2589".       xl
-00002020: 696e 6b3a 6872 6566 3d22 236c 696e 6561  ink:href="#linea
-00002030: 7247 7261 6469 656e 7434 3637 3122 0a20  rGradient4671". 
-00002040: 2020 2020 2020 6772 6164 6965 6e74 556e        gradientUn
-00002050: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
-00002060: 5573 6522 0a20 2020 2020 2020 6772 6164  Use".       grad
-00002070: 6965 6e74 5472 616e 7366 6f72 6d3d 2274  ientTransform="t
-00002080: 7261 6e73 6c61 7465 2831 3030 2e32 3730  ranslate(100.270
-00002090: 322c 3939 2e36 3131 3136 2922 202f 3e0a  2,99.61116)" />.
-000020a0: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
-000020b0: 656e 740a 2020 2020 2020 2078 313d 2231  ent.       x1="1
-000020c0: 3732 2e39 3432 3038 220a 2020 2020 2020  72.94208".      
-000020d0: 2079 313d 2237 372e 3437 3539 3833 220a   y1="77.475983".
-000020e0: 2020 2020 2020 2078 323d 2232 362e 3637         x2="26.67
-000020f0: 3032 3938 220a 2020 2020 2020 2079 323d  0298".       y2=
-00002100: 2237 362e 3331 3331 3333 220a 2020 2020  "76.313133".    
-00002110: 2020 2069 643d 226c 696e 6561 7247 7261     id="linearGra
-00002120: 6469 656e 7432 3234 3822 0a20 2020 2020  dient2248".     
-00002130: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
-00002140: 696e 6561 7247 7261 6469 656e 7434 3638  inearGradient468
-00002150: 3922 0a20 2020 2020 2020 6772 6164 6965  9".       gradie
-00002160: 6e74 556e 6974 733d 2275 7365 7253 7061  ntUnits="userSpa
-00002170: 6365 4f6e 5573 6522 0a20 2020 2020 2020  ceOnUse".       
-00002180: 6772 6164 6965 6e74 5472 616e 7366 6f72  gradientTransfor
-00002190: 6d3d 2274 7261 6e73 6c61 7465 2831 3030  m="translate(100
-000021a0: 2e32 3730 322c 3939 2e36 3131 3136 2922  .2702,99.61116)"
-000021b0: 202f 3e0a 2020 2020 3c6c 696e 6561 7247   />.    <linearG
-000021c0: 7261 6469 656e 740a 2020 2020 2020 2078  radient.       x
-000021d0: 313d 2232 3234 2e32 3339 3936 220a 2020  1="224.23996".  
-000021e0: 2020 2020 2079 313d 2231 3434 2e37 3537       y1="144.757
-000021f0: 3137 220a 2020 2020 2020 2078 323d 222d  17".       x2="-
-00002200: 3635 2e33 3038 3530 3222 0a20 2020 2020  65.308502".     
-00002210: 2020 7932 3d22 3134 342e 3735 3731 3722    y2="144.75717"
-00002220: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
-00002230: 6172 4772 6164 6965 6e74 3232 3530 220a  arGradient2250".
-00002240: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
-00002250: 663d 2223 6c69 6e65 6172 4772 6164 6965  f="#linearGradie
-00002260: 6e74 3436 3731 220a 2020 2020 2020 2067  nt4671".       g
-00002270: 7261 6469 656e 7455 6e69 7473 3d22 7573  radientUnits="us
-00002280: 6572 5370 6163 654f 6e55 7365 220a 2020  erSpaceOnUse".  
-00002290: 2020 2020 2067 7261 6469 656e 7454 7261       gradientTra
-000022a0: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-000022b0: 6528 3130 302e 3237 3032 2c39 392e 3631  e(100.2702,99.61
-000022c0: 3131 3629 2220 2f3e 0a20 2020 203c 6c69  116)" />.    <li
-000022d0: 6e65 6172 4772 6164 6965 6e74 0a20 2020  nearGradient.   
-000022e0: 2020 2020 7831 3d22 3232 342e 3233 3939      x1="224.2399
-000022f0: 3622 0a20 2020 2020 2020 7931 3d22 3134  6".       y1="14
-00002300: 342e 3735 3731 3722 0a20 2020 2020 2020  4.75717".       
-00002310: 7832 3d22 2d36 352e 3330 3835 3032 220a  x2="-65.308502".
-00002320: 2020 2020 2020 2079 323d 2231 3434 2e37         y2="144.7
-00002330: 3537 3137 220a 2020 2020 2020 2069 643d  5717".       id=
-00002340: 226c 696e 6561 7247 7261 6469 656e 7432  "linearGradient2
-00002350: 3235 3522 0a20 2020 2020 2020 786c 696e  255".       xlin
-00002360: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
-00002370: 7261 6469 656e 7434 3637 3122 0a20 2020  radient4671".   
-00002380: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
-00002390: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
-000023a0: 6522 0a20 2020 2020 2020 6772 6164 6965  e".       gradie
-000023b0: 6e74 5472 616e 7366 6f72 6d3d 226d 6174  ntTransform="mat
-000023c0: 7269 7828 302e 3536 3235 3431 2c30 2c30  rix(0.562541,0,0
-000023d0: 2c30 2e35 3637 3937 322c 2d31 312e 3539  ,0.567972,-11.59
-000023e0: 3734 2c2d 372e 3630 3935 3429 2220 2f3e  74,-7.60954)" />
-000023f0: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
-00002400: 6965 6e74 0a20 2020 2020 2020 7831 3d22  ient.       x1="
-00002410: 3137 322e 3934 3230 3822 0a20 2020 2020  172.94208".     
-00002420: 2020 7931 3d22 3736 2e31 3736 3232 3422    y1="76.176224"
-00002430: 0a20 2020 2020 2020 7832 3d22 3236 2e36  .       x2="26.6
-00002440: 3730 3239 3822 0a20 2020 2020 2020 7932  70298".       y2
-00002450: 3d22 3736 2e33 3133 3133 3322 0a20 2020  ="76.313133".   
-00002460: 2020 2020 6964 3d22 6c69 6e65 6172 4772      id="linearGr
-00002470: 6164 6965 6e74 3232 3538 220a 2020 2020  adient2258".    
-00002480: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
-00002490: 6c69 6e65 6172 4772 6164 6965 6e74 3436  linearGradient46
-000024a0: 3839 220a 2020 2020 2020 2067 7261 6469  89".       gradi
-000024b0: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
-000024c0: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
-000024d0: 2067 7261 6469 656e 7454 7261 6e73 666f   gradientTransfo
-000024e0: 726d 3d22 6d61 7472 6978 2830 2e35 3632  rm="matrix(0.562
-000024f0: 3534 312c 302c 302c 302e 3536 3739 3732  541,0,0,0.567972
-00002500: 2c2d 3131 2e35 3937 342c 2d37 2e36 3039  ,-11.5974,-7.609
-00002510: 3534 2922 202f 3e0a 2020 2020 3c72 6164  54)" />.    <rad
-00002520: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
-00002530: 2020 2063 783d 2236 312e 3531 3838 3833     cx="61.518883
-00002540: 220a 2020 2020 2020 2063 793d 2231 3332  ".       cy="132
-00002550: 2e32 3835 3735 220a 2020 2020 2020 2072  .28575".       r
-00002560: 3d22 3239 2e30 3336 3931 3322 0a20 2020  ="29.036913".   
-00002570: 2020 2020 6678 3d22 3631 2e35 3138 3838      fx="61.51888
-00002580: 3322 0a20 2020 2020 2020 6679 3d22 3133  3".       fy="13
-00002590: 322e 3238 3537 3522 0a20 2020 2020 2020  2.28575".       
-000025a0: 6964 3d22 7261 6469 616c 4772 6164 6965  id="radialGradie
-000025b0: 6e74 3238 3031 220a 2020 2020 2020 2078  nt2801".       x
-000025c0: 6c69 6e6b 3a68 7265 663d 2223 6c69 6e65  link:href="#line
-000025d0: 6172 4772 6164 6965 6e74 3237 3935 220a  arGradient2795".
-000025e0: 2020 2020 2020 2067 7261 6469 656e 7455         gradientU
-000025f0: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00002600: 6e55 7365 220a 2020 2020 2020 2067 7261  nUse".       gra
-00002610: 6469 656e 7454 7261 6e73 666f 726d 3d22  dientTransform="
-00002620: 6d61 7472 6978 2831 2c30 2c30 2c30 2e31  matrix(1,0,0,0.1
-00002630: 3737 3936 362c 302c 3130 382e 3734 3334  77966,0,108.7434
-00002640: 2922 202f 3e0a 2020 2020 3c6c 696e 6561  )" />.    <linea
-00002650: 7247 7261 6469 656e 740a 2020 2020 2020  rGradient.      
-00002660: 2078 313d 2231 3530 2e39 3631 3131 220a   x1="150.96111".
-00002670: 2020 2020 2020 2079 313d 2231 3932 2e33         y1="192.3
-00002680: 3531 3736 220a 2020 2020 2020 2078 323d  5176".       x2=
-00002690: 2231 3132 2e30 3331 3434 220a 2020 2020  "112.03144".    
-000026a0: 2020 2079 323d 2231 3337 2e32 3732 3939     y2="137.27299
-000026b0: 220a 2020 2020 2020 2069 643d 226c 696e  ".       id="lin
-000026c0: 6561 7247 7261 6469 656e 7431 3437 3522  earGradient1475"
-000026d0: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
-000026e0: 6566 3d22 236c 696e 6561 7247 7261 6469  ef="#linearGradi
-000026f0: 656e 7434 3637 3122 0a20 2020 2020 2020  ent4671".       
-00002700: 6772 6164 6965 6e74 556e 6974 733d 2275  gradientUnits="u
-00002710: 7365 7253 7061 6365 4f6e 5573 6522 0a20  serSpaceOnUse". 
-00002720: 2020 2020 2020 6772 6164 6965 6e74 5472        gradientTr
-00002730: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
-00002740: 302e 3536 3235 3431 2c30 2c30 2c30 2e35  0.562541,0,0,0.5
-00002750: 3637 3937 322c 2d39 2e33 3939 3734 392c  67972,-9.399749,
-00002760: 2d35 2e33 3035 3331 3729 2220 2f3e 0a20  -5.305317)" />. 
-00002770: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-00002780: 6e74 0a20 2020 2020 2020 7831 3d22 3236  nt.       x1="26
-00002790: 2e36 3438 3933 3722 0a20 2020 2020 2020  .648937".       
-000027a0: 7931 3d22 3230 2e36 3033 3738 3122 0a20  y1="20.603781". 
-000027b0: 2020 2020 2020 7832 3d22 3133 352e 3636        x2="135.66
-000027c0: 3532 3522 0a20 2020 2020 2020 7932 3d22  525".       y2="
-000027d0: 3131 342e 3339 3736 3722 0a20 2020 2020  114.39767".     
-000027e0: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
-000027f0: 6965 6e74 3134 3738 220a 2020 2020 2020  ient1478".      
-00002800: 2078 6c69 6e6b 3a68 7265 663d 2223 6c69   xlink:href="#li
-00002810: 6e65 6172 4772 6164 6965 6e74 3436 3839  nearGradient4689
-00002820: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
-00002830: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
-00002840: 654f 6e55 7365 220a 2020 2020 2020 2067  eOnUse".       g
-00002850: 7261 6469 656e 7454 7261 6e73 666f 726d  radientTransform
-00002860: 3d22 6d61 7472 6978 2830 2e35 3632 3534  ="matrix(0.56254
-00002870: 312c 302c 302c 302e 3536 3739 3732 2c2d  1,0,0,0.567972,-
-00002880: 392e 3339 3937 3439 2c2d 352e 3330 3533  9.399749,-5.3053
-00002890: 3137 2922 202f 3e0a 2020 2020 3c72 6164  17)" />.    <rad
-000028a0: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
-000028b0: 2020 2063 783d 2236 312e 3531 3838 3833     cx="61.518883
-000028c0: 220a 2020 2020 2020 2063 793d 2231 3332  ".       cy="132
-000028d0: 2e32 3835 3735 220a 2020 2020 2020 2072  .28575".       r
-000028e0: 3d22 3239 2e30 3336 3931 3322 0a20 2020  ="29.036913".   
-000028f0: 2020 2020 6678 3d22 3631 2e35 3138 3838      fx="61.51888
-00002900: 3322 0a20 2020 2020 2020 6679 3d22 3133  3".       fy="13
-00002910: 322e 3238 3537 3522 0a20 2020 2020 2020  2.28575".       
-00002920: 6964 3d22 7261 6469 616c 4772 6164 6965  id="radialGradie
-00002930: 6e74 3134 3830 220a 2020 2020 2020 2078  nt1480".       x
-00002940: 6c69 6e6b 3a68 7265 663d 2223 6c69 6e65  link:href="#line
-00002950: 6172 4772 6164 6965 6e74 3237 3935 220a  arGradient2795".
-00002960: 2020 2020 2020 2067 7261 6469 656e 7455         gradientU
-00002970: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00002980: 6e55 7365 220a 2020 2020 2020 2067 7261  nUse".       gra
-00002990: 6469 656e 7454 7261 6e73 666f 726d 3d22  dientTransform="
-000029a0: 6d61 7472 6978 2832 2e33 3832 3731 3665  matrix(2.382716e
-000029b0: 2d38 2c2d 302e 3239 3634 3035 2c31 2e34  -8,-0.296405,1.4
-000029c0: 3336 3736 2c34 2e36 3833 3637 3365 2d37  3676,4.683673e-7
-000029d0: 2c2d 3132 382e 3534 342c 3135 302e 3532  ,-128.544,150.52
-000029e0: 3032 2922 202f 3e0a 2020 2020 3c72 6164  02)" />.    <rad
-000029f0: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
-00002a00: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
-00002a10: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
-00002a20: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
-00002a30: 236c 696e 6561 7247 7261 6469 656e 7432  #linearGradient2
-00002a40: 3739 3522 0a20 2020 2020 2020 6964 3d22  795".       id="
-00002a50: 7261 6469 616c 4772 6164 6965 6e74 3234  radialGradient24
-00002a60: 3231 220a 2020 2020 2020 2067 7261 6469  21".       gradi
-00002a70: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
-00002a80: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
-00002a90: 2067 7261 6469 656e 7454 7261 6e73 666f   gradientTransfo
-00002aa0: 726d 3d22 6d61 7472 6978 2831 2e37 3439  rm="matrix(1.749
-00002ab0: 3035 3635 652d 382c 2d30 2e32 3339 3934  0565e-8,-0.23994
-00002ac0: 372c 312e 3035 3436 3638 2c33 2e37 3931  7,1.054668,3.791
-00002ad0: 3534 3537 652d 372c 2d37 382e 3130 3934  5457e-7,-78.1094
-00002ae0: 3239 2c31 3438 2e38 3539 3036 2922 0a20  29,148.85906)". 
-00002af0: 2020 2020 2020 6378 3d22 3631 2e35 3138        cx="61.518
-00002b00: 3838 3322 0a20 2020 2020 2020 6379 3d22  883".       cy="
-00002b10: 3133 322e 3238 3537 3522 0a20 2020 2020  132.28575".     
-00002b20: 2020 6678 3d22 3631 2e35 3138 3838 3322    fx="61.518883"
-00002b30: 0a20 2020 2020 2020 6679 3d22 3133 322e  .       fy="132.
-00002b40: 3238 3537 3522 0a20 2020 2020 2020 723d  28575".       r=
-00002b50: 2232 392e 3033 3639 3133 2220 2f3e 0a20  "29.036913" />. 
-00002b60: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-00002b70: 6e74 0a20 2020 2020 2020 696e 6b73 6361  nt.       inksca
-00002b80: 7065 3a63 6f6c 6c65 6374 3d22 616c 7761  pe:collect="alwa
-00002b90: 7973 220a 2020 2020 2020 2078 6c69 6e6b  ys".       xlink
-00002ba0: 3a68 7265 663d 2223 6c69 6e65 6172 4772  :href="#linearGr
-00002bb0: 6164 6965 6e74 3436 3731 2d38 220a 2020  adient4671-8".  
-00002bc0: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
-00002bd0: 7261 6469 656e 7433 3832 362d 3622 0a20  radient3826-6". 
-00002be0: 2020 2020 2020 7831 3d22 3336 2e39 3730        x1="36.970
-00002bf0: 3839 3822 0a20 2020 2020 2020 7931 3d22  898".       y1="
-00002c00: 3534 2e36 3436 3736 3322 0a20 2020 2020  54.646763".     
-00002c10: 2020 7832 3d22 3837 2e37 3034 3638 3122    x2="87.704681"
-00002c20: 0a20 2020 2020 2020 7932 3d22 3534 2e36  .       y2="54.6
-00002c30: 3436 3736 3322 0a20 2020 2020 2020 6772  46763".       gr
-00002c40: 6164 6965 6e74 556e 6974 733d 2275 7365  adientUnits="use
-00002c50: 7253 7061 6365 4f6e 5573 6522 202f 3e0a  rSpaceOnUse" />.
-00002c60: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
-00002c70: 656e 740a 2020 2020 2020 2069 643d 226c  ent.       id="l
-00002c80: 696e 6561 7247 7261 6469 656e 7434 3637  inearGradient467
-00002c90: 312d 3822 3e0a 2020 2020 2020 3c73 746f  1-8">.      <sto
-00002ca0: 700a 2020 2020 2020 2020 2073 7479 6c65  p.         style
-00002cb0: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 6666  ="stop-color:#ff
-00002cc0: 6434 3362 3b73 746f 702d 6f70 6163 6974  d43b;stop-opacit
-00002cd0: 793a 3122 0a20 2020 2020 2020 2020 6f66  y:1".         of
-00002ce0: 6673 6574 3d22 3022 0a20 2020 2020 2020  fset="0".       
-00002cf0: 2020 6964 3d22 7374 6f70 3436 3733 2d38    id="stop4673-8
-00002d00: 2220 2f3e 0a20 2020 2020 203c 7374 6f70  " />.      <stop
-00002d10: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00002d20: 2273 746f 702d 636f 6c6f 723a 2366 6665  "stop-color:#ffe
-00002d30: 3837 333b 7374 6f70 2d6f 7061 6369 7479  873;stop-opacity
-00002d40: 3a31 220a 2020 2020 2020 2020 206f 6666  :1".         off
-00002d50: 7365 743d 2231 220a 2020 2020 2020 2020  set="1".        
-00002d60: 2069 643d 2273 746f 7034 3637 352d 3222   id="stop4675-2"
-00002d70: 202f 3e0a 2020 2020 3c2f 6c69 6e65 6172   />.    </linear
-00002d80: 4772 6164 6965 6e74 3e0a 2020 2020 3c6c  Gradient>.    <l
-00002d90: 696e 6561 7247 7261 6469 656e 740a 2020  inearGradient.  
-00002da0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-00002db0: 6c6c 6563 743d 2261 6c77 6179 7322 0a20  llect="always". 
-00002dc0: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
-00002dd0: 3d22 236c 696e 6561 7247 7261 6469 656e  ="#linearGradien
-00002de0: 7433 3831 3222 0a20 2020 2020 2020 6964  t3812".       id
-00002df0: 3d22 6c69 6e65 6172 4772 6164 6965 6e74  ="linearGradient
-00002e00: 3338 3138 220a 2020 2020 2020 2078 313d  3818".       x1=
-00002e10: 2237 382e 3031 3230 3234 220a 2020 2020  "78.012024".    
-00002e20: 2020 2079 313d 2238 302e 3330 3239 3333     y1="80.302933
-00002e30: 220a 2020 2020 2020 2078 323d 2231 3234  ".       x2="124
-00002e40: 2e36 3739 3634 220a 2020 2020 2020 2079  .67964".       y
-00002e50: 323d 2232 382e 3630 3333 3237 220a 2020  2="28.603327".  
-00002e60: 2020 2020 2067 7261 6469 656e 7455 6e69       gradientUni
-00002e70: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
-00002e80: 7365 2220 2f3e 0a20 2020 203c 6c69 6e65  se" />.    <line
-00002e90: 6172 4772 6164 6965 6e74 0a20 2020 2020  arGradient.     
-00002ea0: 2020 696e 6b73 6361 7065 3a63 6f6c 6c65    inkscape:colle
-00002eb0: 6374 3d22 616c 7761 7973 220a 2020 2020  ct="always".    
-00002ec0: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
-00002ed0: 6c69 6e65 6172 4772 6164 6965 6e74 3338  linearGradient38
-00002ee0: 3132 220a 2020 2020 2020 2069 643d 226c  12".       id="l
-00002ef0: 696e 6561 7247 7261 6469 656e 7434 3039  inearGradient409
-00002f00: 3722 0a20 2020 2020 2020 7831 3d22 2d32  7".       x1="-2
-00002f10: 3035 2e30 3534 3331 220a 2020 2020 2020  05.05431".      
-00002f20: 2079 313d 2235 352e 3630 3634 3431 220a   y1="55.606441".
-00002f30: 2020 2020 2020 2078 323d 222d 3634 2e38         x2="-64.8
-00002f40: 3036 3235 3922 0a20 2020 2020 2020 7932  06259".       y2
-00002f50: 3d22 3535 2e36 3036 3434 3122 0a20 2020  ="55.606441".   
-00002f60: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
-00002f70: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
-00002f80: 6522 0a20 2020 2020 2020 6772 6164 6965  e".       gradie
-00002f90: 6e74 5472 616e 7366 6f72 6d3d 226d 6174  ntTransform="mat
-00002fa0: 7269 7828 312e 3039 3531 3533 392c 302c  rix(1.0951539,0,
-00002fb0: 302c 312e 3033 3135 3236 382c 3238 332e  0,1.0315268,283.
-00002fc0: 3739 3331 312c 3134 2e37 3232 3734 3629  79311,14.722746)
-00002fd0: 2220 2f3e 0a20 2020 203c 6c69 6e65 6172  " />.    <linear
-00002fe0: 4772 6164 6965 6e74 0a20 2020 2020 2020  Gradient.       
-00002ff0: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
-00003000: 3d22 616c 7761 7973 220a 2020 2020 2020  ="always".      
-00003010: 2078 6c69 6e6b 3a68 7265 663d 2223 6c69   xlink:href="#li
-00003020: 6e65 6172 4772 6164 6965 6e74 3138 3934  nearGradient1894
-00003030: 220a 2020 2020 2020 2069 643d 226c 696e  ".       id="lin
-00003040: 6561 7247 7261 6469 656e 7434 3039 372d  earGradient4097-
-00003050: 3422 0a20 2020 2020 2020 7831 3d22 2d32  4".       x1="-2
-00003060: 3035 2e30 3534 3331 220a 2020 2020 2020  05.05431".      
-00003070: 2079 313d 2235 352e 3630 3634 3431 220a   y1="55.606441".
-00003080: 2020 2020 2020 2078 323d 222d 3634 2e38         x2="-64.8
-00003090: 3036 3235 3922 0a20 2020 2020 2020 7932  06259".       y2
-000030a0: 3d22 3535 2e36 3036 3434 3122 0a20 2020  ="55.606441".   
-000030b0: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
-000030c0: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
-000030d0: 6522 0a20 2020 2020 2020 6772 6164 6965  e".       gradie
-000030e0: 6e74 5472 616e 7366 6f72 6d3d 2274 7261  ntTransform="tra
-000030f0: 6e73 6c61 7465 2832 3732 2e32 3238 332c  nslate(272.2283,
-00003100: 3135 2e36 3837 3930 3129 2220 2f3e 0a20  15.687901)" />. 
-00003110: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-00003120: 6e74 0a20 2020 2020 2020 6964 3d22 6c69  nt.       id="li
-00003130: 6e65 6172 4772 6164 6965 6e74 3138 3934  nearGradient1894
-00003140: 223e 0a20 2020 2020 203c 7374 6f70 0a20  ">.      <stop. 
-00003150: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
-00003160: 746f 702d 636f 6c6f 723a 2366 6666 3363  top-color:#fff3c
-00003170: 653b 7374 6f70 2d6f 7061 6369 7479 3a31  e;stop-opacity:1
-00003180: 3b22 0a20 2020 2020 2020 2020 6f66 6673  ;".         offs
-00003190: 6574 3d22 3022 0a20 2020 2020 2020 2020  et="0".         
-000031a0: 6964 3d22 7374 6f70 3138 3930 2220 2f3e  id="stop1890" />
-000031b0: 0a20 2020 2020 203c 7374 6f70 0a20 2020  .      <stop.   
-000031c0: 2020 2020 2020 7374 796c 653d 2273 746f        style="sto
-000031d0: 702d 636f 6c6f 723a 2366 6665 3837 333b  p-color:#ffe873;
-000031e0: 7374 6f70 2d6f 7061 6369 7479 3a31 220a  stop-opacity:1".
-000031f0: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
-00003200: 2231 220a 2020 2020 2020 2020 2069 643d  "1".         id=
-00003210: 2273 746f 7031 3839 3222 202f 3e0a 2020  "stop1892" />.  
-00003220: 2020 3c2f 6c69 6e65 6172 4772 6164 6965    </linearGradie
-00003230: 6e74 3e0a 2020 3c2f 6465 6673 3e0a 2020  nt>.  </defs>.  
-00003240: 3c65 6c6c 6970 7365 0a20 2020 2020 7374  <ellipse.     st
-00003250: 796c 653d 2266 696c 6c3a 7572 6c28 236c  yle="fill:url(#l
-00003260: 696e 6561 7247 7261 6469 656e 7434 3039  inearGradient409
-00003270: 3729 3b66 696c 6c2d 6f70 6163 6974 793a  7);fill-opacity:
-00003280: 313b 7374 726f 6b65 3a6e 6f6e 653b 7374  1;stroke:none;st
-00003290: 726f 6b65 2d77 6964 7468 3a31 2e30 3632  roke-width:1.062
-000032a0: 3836 3b73 7472 6f6b 652d 6f70 6163 6974  86;stroke-opacit
-000032b0: 793a 3122 0a20 2020 2020 6964 3d22 7061  y:1".     id="pa
-000032c0: 7468 3430 3839 220a 2020 2020 2063 783d  th4089".     cx=
-000032d0: 2231 3336 2e30 3233 3638 220a 2020 2020  "136.02368".    
-000032e0: 2063 793d 2237 322e 3038 3232 3833 220a   cy="72.082283".
-000032f0: 2020 2020 2072 783d 2237 362e 3234 3930       rx="76.2490
-00003300: 3233 220a 2020 2020 2072 793d 2235 332e  23".     ry="53.
-00003310: 3136 3833 3639 2220 2f3e 0a20 203c 656c  168369" />.  <el
-00003320: 6c69 7073 650a 2020 2020 2073 7479 6c65  lipse.     style
-00003330: 3d22 6669 6c6c 3a75 726c 2823 6c69 6e65  ="fill:url(#line
-00003340: 6172 4772 6164 6965 6e74 3430 3937 2d34  arGradient4097-4
-00003350: 293b 6669 6c6c 2d6f 7061 6369 7479 3a31  );fill-opacity:1
-00003360: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
-00003370: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00003380: 2020 2020 6964 3d22 7061 7468 3430 3839      id="path4089
-00003390: 2d32 220a 2020 2020 2063 783d 2231 3337  -2".     cx="137
-000033a0: 2e32 3938 3032 220a 2020 2020 2063 793d  .29802".     cy=
-000033b0: 2237 312e 3239 3433 3432 220a 2020 2020  "71.294342".    
-000033c0: 2072 783d 2236 392e 3632 3430 3233 220a   rx="69.624023".
-000033d0: 2020 2020 2072 793d 2235 312e 3534 3333       ry="51.5433
-000033e0: 3639 2220 2f3e 0a20 203c 7061 7468 0a20  69" />.  <path. 
-000033f0: 2020 2020 7374 796c 653d 2263 6f6c 6f72      style="color
-00003400: 3a23 3030 3030 3030 3b66 6f6e 742d 7374  :#000000;font-st
-00003410: 796c 653a 6e6f 726d 616c 3b66 6f6e 742d  yle:normal;font-
-00003420: 7661 7269 616e 743a 6e6f 726d 616c 3b66  variant:normal;f
-00003430: 6f6e 742d 7765 6967 6874 3a6e 6f72 6d61  ont-weight:norma
-00003440: 6c3b 666f 6e74 2d73 7472 6574 6368 3a6e  l;font-stretch:n
-00003450: 6f72 6d61 6c3b 666f 6e74 2d73 697a 653a  ormal;font-size:
-00003460: 6d65 6469 756d 3b6c 696e 652d 6865 6967  medium;line-heig
-00003470: 6874 3a6e 6f72 6d61 6c3b 666f 6e74 2d66  ht:normal;font-f
-00003480: 616d 696c 793a 5361 6e73 3b2d 696e 6b73  amily:Sans;-inks
-00003490: 6361 7065 2d66 6f6e 742d 7370 6563 6966  cape-font-specif
-000034a0: 6963 6174 696f 6e3a 5361 6e73 3b74 6578  ication:Sans;tex
-000034b0: 742d 696e 6465 6e74 3a30 3b74 6578 742d  t-indent:0;text-
-000034c0: 616c 6967 6e3a 7374 6172 743b 7465 7874  align:start;text
-000034d0: 2d64 6563 6f72 6174 696f 6e3a 6e6f 6e65  -decoration:none
-000034e0: 3b74 6578 742d 6465 636f 7261 7469 6f6e  ;text-decoration
-000034f0: 2d6c 696e 653a 6e6f 6e65 3b6c 6574 7465  -line:none;lette
-00003500: 722d 7370 6163 696e 673a 6e6f 726d 616c  r-spacing:normal
-00003510: 3b77 6f72 642d 7370 6163 696e 673a 6e6f  ;word-spacing:no
-00003520: 726d 616c 3b74 6578 742d 7472 616e 7366  rmal;text-transf
-00003530: 6f72 6d3a 6e6f 6e65 3b77 7269 7469 6e67  orm:none;writing
-00003540: 2d6d 6f64 653a 6c72 2d74 623b 6469 7265  -mode:lr-tb;dire
-00003550: 6374 696f 6e3a 6c74 723b 6261 7365 6c69  ction:ltr;baseli
-00003560: 6e65 2d73 6869 6674 3a62 6173 656c 696e  ne-shift:baselin
-00003570: 653b 7465 7874 2d61 6e63 686f 723a 7374  e;text-anchor:st
-00003580: 6172 743b 6469 7370 6c61 793a 696e 6c69  art;display:inli
-00003590: 6e65 3b6f 7665 7266 6c6f 773a 7669 7369  ne;overflow:visi
-000035a0: 626c 653b 7669 7369 6269 6c69 7479 3a76  ble;visibility:v
-000035b0: 6973 6962 6c65 3b66 696c 6c3a 2362 6262  isible;fill:#bbb
-000035c0: 6262 623b 6669 6c6c 2d6f 7061 6369 7479  bbb;fill-opacity
-000035d0: 3a31 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  :1;fill-rule:non
-000035e0: 7a65 726f 3b73 7472 6f6b 653a 6e6f 6e65  zero;stroke:none
-000035f0: 3b73 7472 6f6b 652d 7769 6474 683a 392e  ;stroke-width:9.
-00003600: 3538 3436 323b 6d61 726b 6572 3a6e 6f6e  58462;marker:non
-00003610: 653b 656e 6162 6c65 2d62 6163 6b67 726f  e;enable-backgro
-00003620: 756e 643a 6163 6375 6d75 6c61 7465 220a  und:accumulate".
-00003630: 2020 2020 2064 3d22 6d20 3133 372e 3630       d="m 137.60
-00003640: 3438 362c 3138 2e33 3834 3737 3720 6320  486,18.384777 c 
-00003650: 2d35 352e 3236 3035 3532 2c30 202d 3737  -55.260552,0 -77
-00003660: 2e34 3133 3732 322c 3230 2e30 3636 3234  .413722,20.06624
-00003670: 3620 2d37 372e 3431 3337 3232 2c35 332e  6 -77.413722,53.
-00003680: 3231 3230 3335 2030 2e37 3839 3338 2c32  212035 0.78938,2
-00003690: 372e 3233 3730 3535 2032 342e 3737 3934  7.237055 24.7794
-000036a0: 362c 3437 2e36 3934 3136 3820 3436 2e39  6,47.694168 46.9
-000036b0: 3238 3239 322c 3535 2e35 3030 3034 3820  28292,55.500048 
-000036c0: 392e 3139 3936 322c 332e 3035 3932 3620  9.19962,3.05926 
-000036d0: 3335 2e37 3736 3038 2c33 322e 3934 3938  35.77608,32.9498
-000036e0: 3320 3436 2e34 3033 3731 2c33 322e 3934  3 46.40371,32.94
-000036f0: 3938 3320 352e 3331 3338 332c 3020 2d31  983 5.31383,0 -1
-00003700: 392e 3230 3933 352c 2d32 302e 3232 3835  9.20935,-20.2285
-00003710: 3120 2d31 332e 3232 3237 382c 2d32 342e  1 -13.22278,-24.
-00003720: 3637 3933 3520 352e 3434 3532 352c 2d34  67935 5.44525,-4
-00003730: 2e30 3438 3338 2031 332e 3035 3230 312c  .04838 13.05201,
-00003740: 2d34 2e30 3138 3033 2032 382e 3231 3536  -4.01803 28.2156
-00003750: 382c 2d31 302e 3737 3034 3820 3135 2e31  8,-10.77048 15.1
-00003760: 3633 3637 2c2d 362e 3735 3234 3620 3435  6367,-6.75246 45
-00003770: 2e31 3832 3635 2c2d 3235 2e32 3332 3230  .18265,-25.23220
-00003780: 3420 3435 2e34 3536 3335 2c2d 3533 2e30  4 45.45635,-53.0
-00003790: 3030 3034 3820 302c 2d33 332e 3134 3537  00048 0,-33.1457
-000037a0: 3839 202d 3231 2e31 3036 3938 2c2d 3533  89 -21.10698,-53
-000037b0: 2e32 3132 3033 3520 2d37 362e 3336 3735  .212035 -76.3675
-000037c0: 332c 2d35 332e 3231 3230 3335 207a 206d  3,-53.212035 z m
-000037d0: 2031 2e30 3339 3732 2c39 2e38 3831 3230   1.03972,9.88120
-000037e0: 3120 6320 3436 2e30 3238 3636 2c30 2e32  1 c 46.02866,0.2
-000037f0: 3439 3939 3920 3635 2e31 3230 3036 2c31  49999 65.12006,1
-00003800: 342e 3138 3831 2036 352e 3132 3030 362c  4.1881 65.12006,
-00003810: 3433 2e33 3330 3833 3420 2d31 2e30 3431  43.330834 -1.041
-00003820: 3934 2c33 332e 3035 3335 3838 202d 3335  94,33.053588 -35
-00003830: 2e39 3936 3233 2c34 372e 3238 3830 3638  .99623,47.288068
-00003840: 202d 3636 2e34 3439 352c 3437 2e35 3432   -66.4495,47.542
-00003850: 3838 3820 2d33 302e 3435 3332 382c 302e  888 -30.45328,0.
-00003860: 3235 3438 3220 2d36 362e 3931 3632 3532  25482 -66.916252
-00003870: 2c2d 3138 2e34 3030 3135 202d 3636 2e39  ,-18.40015 -66.9
-00003880: 3136 3235 322c 2d34 372e 3534 3238 3838  16252,-47.542888
-00003890: 2030 2c2d 3239 2e31 3432 3733 3620 3232   0,-29.142736 22
-000038a0: 2e32 3137 3033 2c2d 3433 2e35 3830 3833  .21703,-43.58083
-000038b0: 3420 3638 2e32 3435 3639 322c 2d34 332e  4 68.245692,-43.
-000038c0: 3333 3038 3334 207a 220a 2020 2020 2069  330834 z".     i
-000038d0: 643d 2270 6174 6833 3033 3222 0a20 2020  d="path3032".   
-000038e0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-000038f0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00003900: 3022 0a20 2020 2020 736f 6469 706f 6469  0".     sodipodi
-00003910: 3a6e 6f64 6574 7970 6573 3d22 7a63 6373  :nodetypes="zccs
-00003920: 737a 637a 7a63 7a7a 7a22 202f 3e0a 2020  szczzczzz" />.  
-00003930: 3c74 6578 740a 2020 2020 2078 6d6c 3a73  <text.     xml:s
-00003940: 7061 6365 3d22 7072 6573 6572 7665 220a  pace="preserve".
-00003950: 2020 2020 2073 7479 6c65 3d22 666f 6e74       style="font
-00003960: 2d73 7479 6c65 3a69 7461 6c69 633b 666f  -style:italic;fo
-00003970: 6e74 2d77 6569 6768 743a 626f 6c64 3b66  nt-weight:bold;f
-00003980: 6f6e 742d 7369 7a65 3a39 3670 783b 6c69  ont-size:96px;li
-00003990: 6e65 2d68 6569 6768 743a 312e 353b 666f  ne-height:1.5;fo
-000039a0: 6e74 2d66 616d 696c 793a 2743 656e 7475  nt-family:'Centu
-000039b0: 7279 2047 6f74 6869 6327 3b2d 696e 6b73  ry Gothic';-inks
-000039c0: 6361 7065 2d66 6f6e 742d 7370 6563 6966  cape-font-specif
-000039d0: 6963 6174 696f 6e3a 2743 656e 7475 7279  ication:'Century
-000039e0: 2047 6f74 6869 6320 426f 6c64 2049 7461   Gothic Bold Ita
-000039f0: 6c69 6327 3b6c 6574 7465 722d 7370 6163  lic';letter-spac
-00003a00: 696e 673a 2d34 2e37 3470 783b 6669 6c6c  ing:-4.74px;fill
-00003a10: 3a23 3830 3830 3830 3b73 7472 6f6b 652d  :#808080;stroke-
-00003a20: 7769 6474 683a 3133 2e34 3033 220a 2020  width:13.403".  
-00003a30: 2020 2078 3d22 3131 2e31 3534 3038 3122     x="11.154081"
-00003a40: 0a20 2020 2020 793d 2232 3031 2e34 3837  .     y="201.487
-00003a50: 3722 0a20 2020 2020 6964 3d22 7465 7874  7".     id="text
-00003a60: 3338 3022 3e3c 7473 7061 6e0a 2020 2020  380"><tspan.    
-00003a70: 2020 2073 6f64 6970 6f64 693a 726f 6c65     sodipodi:role
-00003a80: 3d22 6c69 6e65 220a 2020 2020 2020 2069  ="line".       i
-00003a90: 643d 2274 7370 616e 3337 3822 0a20 2020  d="tspan378".   
-00003aa0: 2020 2020 783d 2231 312e 3135 3430 3831      x="11.154081
-00003ab0: 220a 2020 2020 2020 2079 3d22 3230 312e  ".       y="201.
-00003ac0: 3438 3737 220a 2020 2020 2020 2073 7479  4877".       sty
-00003ad0: 6c65 3d22 666f 6e74 2d73 7479 6c65 3a6e  le="font-style:n
-00003ae0: 6f72 6d61 6c3b 666f 6e74 2d76 6172 6961  ormal;font-varia
-00003af0: 6e74 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  nt:normal;font-w
-00003b00: 6569 6768 743a 3330 303b 666f 6e74 2d73  eight:300;font-s
-00003b10: 7472 6574 6368 3a6e 6f72 6d61 6c3b 666f  tretch:normal;fo
-00003b20: 6e74 2d73 697a 653a 3936 7078 3b66 6f6e  nt-size:96px;fon
-00003b30: 742d 6661 6d69 6c79 3a43 6f72 6265 6c3b  t-family:Corbel;
-00003b40: 2d69 6e6b 7363 6170 652d 666f 6e74 2d73  -inkscape-font-s
-00003b50: 7065 6369 6669 6361 7469 6f6e 3a27 436f  pecification:'Co
-00003b60: 7262 656c 204c 6967 6874 273b 6669 6c6c  rbel Light';fill
-00003b70: 3a23 3830 3830 3830 223e 6775 6964 6174  :#808080">guidat
-00003b80: 613c 2f74 7370 616e 3e3c 2f74 6578 743e  a</tspan></text>
-00003b90: 0a20 203c 670a 2020 2020 2069 643d 2267  .  <g.     id="g
-00003ba0: 3222 0a20 2020 2020 7472 616e 7366 6f72  2".     transfor
-00003bb0: 6d3d 2274 7261 6e73 6c61 7465 2835 372e  m="translate(57.
-00003bc0: 3937 3832 3435 2c31 302e 3231 3533 3035  978245,10.215305
-00003bd0: 2922 3e0a 2020 2020 3c72 6563 740a 2020  )">.    <rect.  
-00003be0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00003bf0: 3a23 6666 6666 6666 3b66 696c 6c2d 6f70  :#ffffff;fill-op
-00003c00: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-00003c10: 6263 6263 6263 3b73 7472 6f6b 652d 7769  bcbcbc;stroke-wi
-00003c20: 6474 683a 362e 333b 7374 726f 6b65 2d64  dth:6.3;stroke-d
-00003c30: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00003c40: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00003c50: 2020 2020 2020 2069 643d 2272 6563 7431         id="rect1
-00003c60: 220a 2020 2020 2020 2077 6964 7468 3d22  ".       width="
-00003c70: 3939 2e32 3432 3537 3722 0a20 2020 2020  99.242577".     
-00003c80: 2020 6865 6967 6874 3d22 3538 2e35 3530    height="58.550
-00003c90: 3536 3422 0a20 2020 2020 2020 783d 2232  564".       x="2
-00003ca0: 392e 3639 3834 3836 220a 2020 2020 2020  9.698486".      
-00003cb0: 2079 3d22 3331 2e38 3033 3735 3522 0a20   y="31.803755". 
-00003cc0: 2020 2020 2020 7279 3d22 362e 3535 3331        ry="6.5531
-00003cd0: 3932 3122 202f 3e0a 2020 2020 3c72 6563  921" />.    <rec
-00003ce0: 740a 2020 2020 2020 2073 7479 6c65 3d22  t.       style="
-00003cf0: 6669 6c6c 3a23 6263 6263 6263 3b66 696c  fill:#bcbcbc;fil
-00003d00: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00003d10: 6b65 3a6e 6f6e 653b 7374 726f 6b65 2d77  ke:none;stroke-w
-00003d20: 6964 7468 3a31 2e36 3130 3538 3b73 7472  idth:1.61058;str
-00003d30: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00003d40: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00003d50: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
-00003d60: 7265 6374 312d 3122 0a20 2020 2020 2020  rect1-1".       
-00003d70: 7769 6474 683d 2237 2e38 3630 3835 3138  width="7.8608518
-00003d80: 220a 2020 2020 2020 2068 6569 6768 743d  ".       height=
-00003d90: 2234 382e 3331 3036 3639 220a 2020 2020  "48.310669".    
-00003da0: 2020 2078 3d22 3933 2e38 3336 3632 3422     x="93.836624"
-00003db0: 0a20 2020 2020 2020 793d 2233 362e 3937  .       y="36.97
-00003dc0: 3136 3131 220a 2020 2020 2020 2072 793d  1611".       ry=
-00003dd0: 2235 2e34 3037 3130 3539 2220 2f3e 0a20  "5.4071059" />. 
-00003de0: 2020 203c 7465 7874 0a20 2020 2020 2020     <text.       
-00003df0: 786d 6c3a 7370 6163 653d 2270 7265 7365  xml:space="prese
-00003e00: 7276 6522 0a20 2020 2020 2020 7374 796c  rve".       styl
-00003e10: 653d 2266 6f6e 742d 7765 6967 6874 3a62  e="font-weight:b
-00003e20: 6f6c 643b 666f 6e74 2d73 697a 653a 3534  old;font-size:54
-00003e30: 2e33 3237 3170 783b 6c69 6e65 2d68 6569  .3271px;line-hei
-00003e40: 6768 743a 313b 666f 6e74 2d66 616d 696c  ght:1;font-famil
-00003e50: 793a 436f 7262 656c 3b2d 696e 6b73 6361  y:Corbel;-inksca
-00003e60: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
-00003e70: 6174 696f 6e3a 2743 6f72 6265 6c20 426f  ation:'Corbel Bo
-00003e80: 6c64 273b 7465 7874 2d61 6c69 676e 3a63  ld';text-align:c
-00003e90: 656e 7465 723b 6c65 7474 6572 2d73 7061  enter;letter-spa
-00003ea0: 6369 6e67 3a2d 352e 3338 3037 3870 783b  cing:-5.38078px;
-00003eb0: 7465 7874 2d61 6e63 686f 723a 6d69 6464  text-anchor:midd
-00003ec0: 6c65 3b66 696c 6c3a 2333 3834 6539 613b  le;fill:#384e9a;
-00003ed0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-00003ee0: 7472 6f6b 653a 6e6f 6e65 3b73 7472 6f6b  troke:none;strok
-00003ef0: 652d 7769 6474 683a 372e 3534 3938 383b  e-width:7.54988;
-00003f00: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00003f10: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-00003f20: 6369 7479 3a31 220a 2020 2020 2020 2078  city:1".       x
-00003f30: 3d22 3634 2e30 3230 3130 3322 0a20 2020  ="64.020103".   
-00003f40: 2020 2020 793d 2238 302e 3832 3437 3322      y="80.82473"
-00003f50: 0a20 2020 2020 2020 6964 3d22 7465 7874  .       id="text
-00003f60: 3122 0a20 2020 2020 2020 7472 616e 7366  1".       transf
-00003f70: 6f72 6d3d 2273 6361 6c65 2831 2e30 3136  orm="scale(1.016
-00003f80: 3031 3937 2c30 2e39 3834 3233 3238 3829  0197,0.98423288)
-00003f90: 223e 3c74 7370 616e 0a20 2020 2020 2020  "><tspan.       
-00003fa0: 2020 736f 6469 706f 6469 3a72 6f6c 653d    sodipodi:role=
-00003fb0: 226c 696e 6522 0a20 2020 2020 2020 2020  "line".         
-00003fc0: 6964 3d22 7473 7061 6e31 220a 2020 2020  id="tspan1".    
-00003fd0: 2020 2020 2078 3d22 3631 2e33 3239 3731       x="61.32971
-00003fe0: 3222 0a20 2020 2020 2020 2020 793d 2238  2".         y="8
-00003ff0: 302e 3832 3437 3322 0a20 2020 2020 2020  0.82473".       
-00004000: 2020 7374 796c 653d 2266 6f6e 742d 7374    style="font-st
-00004010: 796c 653a 6e6f 726d 616c 3b66 6f6e 742d  yle:normal;font-
-00004020: 7661 7269 616e 743a 6e6f 726d 616c 3b66  variant:normal;f
-00004030: 6f6e 742d 7765 6967 6874 3a62 6f6c 643b  ont-weight:bold;
-00004040: 666f 6e74 2d73 7472 6574 6368 3a6e 6f72  font-stretch:nor
-00004050: 6d61 6c3b 666f 6e74 2d66 616d 696c 793a  mal;font-family:
-00004060: 4172 6961 6c3b 2d69 6e6b 7363 6170 652d  Arial;-inkscape-
-00004070: 666f 6e74 2d73 7065 6369 6669 6361 7469  font-specificati
-00004080: 6f6e 3a27 4172 6961 6c20 426f 6c64 273b  on:'Arial Bold';
-00004090: 6669 6c6c 3a23 3338 3465 3961 3b66 696c  fill:#384e9a;fil
-000040a0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-000040b0: 6b65 2d77 6964 7468 3a37 2e35 3439 3838  ke-width:7.54988
-000040c0: 223e 3031 3c2f 7473 7061 6e3e 3c2f 7465  ">01</tspan></te
-000040d0: 7874 3e0a 2020 3c2f 673e 0a3c 2f73 7667  xt>.  </g>.</svg
-000040e0: 3e0a                                     >.
+000011b0: 6974 793a 302e 3234 3739 3333 3838 3b22  ity:0.24793388;"
+000011c0: 0d0a 2020 2020 2020 2020 206f 6666 7365  ..         offse
+000011d0: 743d 2230 220d 0a20 2020 2020 2020 2020  t="0"..         
+000011e0: 6964 3d22 7374 6f70 3333 3532 2220 2f3e  id="stop3352" />
+000011f0: 0d0a 2020 2020 2020 3c73 746f 700d 0a20  ..      <stop.. 
+00001200: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
+00001210: 746f 702d 636f 6c6f 723a 2330 3063 6232  top-color:#00cb2
+00001220: 623b 7374 6f70 2d6f 7061 6369 7479 3a31  b;stop-opacity:1
+00001230: 3b22 0d0a 2020 2020 2020 2020 206f 6666  ;"..         off
+00001240: 7365 743d 2231 220d 0a20 2020 2020 2020  set="1"..       
+00001250: 2020 6964 3d22 7374 6f70 3333 3534 2220    id="stop3354" 
+00001260: 2f3e 0d0a 2020 2020 3c2f 6c69 6e65 6172  />..    </linear
+00001270: 4772 6164 6965 6e74 3e0d 0a20 2020 203c  Gradient>..    <
+00001280: 6c69 6e65 6172 4772 6164 6965 6e74 0d0a  linearGradient..
+00001290: 2020 2020 2020 2069 643d 226c 696e 6561         id="linea
+000012a0: 7247 7261 6469 656e 7433 3334 3222 3e0d  rGradient3342">.
+000012b0: 0a20 2020 2020 203c 7374 6f70 0d0a 2020  .      <stop..  
+000012c0: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
+000012d0: 6f70 2d63 6f6c 6f72 3a23 3030 3561 3835  op-color:#005a85
+000012e0: 3b73 746f 702d 6f70 6163 6974 793a 313b  ;stop-opacity:1;
+000012f0: 220d 0a20 2020 2020 2020 2020 6f66 6673  "..         offs
+00001300: 6574 3d22 3022 0d0a 2020 2020 2020 2020  et="0"..        
+00001310: 2069 643d 2273 746f 7033 3334 3422 202f   id="stop3344" /
+00001320: 3e0d 0a20 2020 2020 203c 7374 6f70 0d0a  >..      <stop..
+00001330: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00001340: 7374 6f70 2d63 6f6c 6f72 3a23 3030 3561  stop-color:#005a
+00001350: 3835 3b73 746f 702d 6f70 6163 6974 793a  85;stop-opacity:
+00001360: 302e 3735 3230 3636 3134 3b22 0d0a 2020  0.75206614;"..  
+00001370: 2020 2020 2020 206f 6666 7365 743d 2231         offset="1
+00001380: 220d 0a20 2020 2020 2020 2020 6964 3d22  "..         id="
+00001390: 7374 6f70 3333 3436 2220 2f3e 0d0a 2020  stop3346" />..  
+000013a0: 2020 3c2f 6c69 6e65 6172 4772 6164 6965    </linearGradie
+000013b0: 6e74 3e0d 0a20 2020 203c 6c69 6e65 6172  nt>..    <linear
+000013c0: 4772 6164 6965 6e74 0d0a 2020 2020 2020  Gradient..      
+000013d0: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
+000013e0: 656e 7433 3331 3022 3e0d 0a20 2020 2020  ent3310">..     
+000013f0: 203c 7374 6f70 0d0a 2020 2020 2020 2020   <stop..        
+00001400: 2069 643d 2273 746f 7033 3331 3222 0d0a   id="stop3312"..
+00001410: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
+00001420: 2230 220d 0a20 2020 2020 2020 2020 7374  "0"..         st
+00001430: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
+00001440: 2361 6530 3230 323b 7374 6f70 2d6f 7061  #ae0202;stop-opa
+00001450: 6369 7479 3a31 3b22 202f 3e0d 0a20 2020  city:1;" />..   
+00001460: 2020 203c 7374 6f70 0d0a 2020 2020 2020     <stop..      
+00001470: 2020 2069 643d 2273 746f 7033 3331 3422     id="stop3314"
+00001480: 0d0a 2020 2020 2020 2020 206f 6666 7365  ..         offse
+00001490: 743d 2231 220d 0a20 2020 2020 2020 2020  t="1"..         
+000014a0: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
+000014b0: 723a 2362 3437 3537 353b 7374 6f70 2d6f  r:#b47575;stop-o
+000014c0: 7061 6369 7479 3a31 3b22 202f 3e0d 0a20  pacity:1;" />.. 
+000014d0: 2020 203c 2f6c 696e 6561 7247 7261 6469     </linearGradi
+000014e0: 656e 743e 0d0a 2020 2020 3c69 6e6b 7363  ent>..    <inksc
+000014f0: 6170 653a 7065 7273 7065 6374 6976 650d  ape:perspective.
+00001500: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00001510: 3a74 7970 653d 2269 6e6b 7363 6170 653a  :type="inkscape:
+00001520: 7065 7273 7033 6422 0d0a 2020 2020 2020  persp3d"..      
+00001530: 2069 6e6b 7363 6170 653a 7670 5f78 3d22   inkscape:vp_x="
+00001540: 3020 3a20 3731 2e38 3837 3439 3720 3a20  0 : 71.887497 : 
+00001550: 3122 0d0a 2020 2020 2020 2069 6e6b 7363  1"..       inksc
+00001560: 6170 653a 7670 5f79 3d22 3020 3a20 3130  ape:vp_y="0 : 10
+00001570: 3030 203a 2030 220d 0a20 2020 2020 2020  00 : 0"..       
+00001580: 696e 6b73 6361 7065 3a76 705f 7a3d 2234  inkscape:vp_z="4
+00001590: 3836 2e30 3439 3939 203a 2037 312e 3838  86.04999 : 71.88
+000015a0: 3734 3937 203a 2031 220d 0a20 2020 2020  7497 : 1"..     
+000015b0: 2020 696e 6b73 6361 7065 3a70 6572 7370    inkscape:persp
+000015c0: 3364 2d6f 7269 6769 6e3d 2232 3433 2e30  3d-origin="243.0
+000015d0: 3234 3939 203a 2034 372e 3932 3439 3938  2499 : 47.924998
+000015e0: 203a 2031 220d 0a20 2020 2020 2020 6964   : 1"..       id
+000015f0: 3d22 7065 7273 7065 6374 6976 6534 3722  ="perspective47"
+00001600: 202f 3e0d 0a20 2020 203c 6c69 6e65 6172   />..    <linear
+00001610: 4772 6164 6965 6e74 0d0a 2020 2020 2020  Gradient..      
+00001620: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
+00001630: 656e 7432 3739 3522 3e0d 0a20 2020 2020  ent2795">..     
+00001640: 203c 7374 6f70 0d0a 2020 2020 2020 2020   <stop..        
+00001650: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
+00001660: 6f72 3a23 6238 6238 6238 3b73 746f 702d  or:#b8b8b8;stop-
+00001670: 6f70 6163 6974 793a 302e 3439 3830 3339  opacity:0.498039
+00001680: 3232 220d 0a20 2020 2020 2020 2020 6f66  22"..         of
+00001690: 6673 6574 3d22 3022 0d0a 2020 2020 2020  fset="0"..      
+000016a0: 2020 2069 643d 2273 746f 7032 3739 3722     id="stop2797"
+000016b0: 202f 3e0d 0a20 2020 2020 203c 7374 6f70   />..      <stop
+000016c0: 0d0a 2020 2020 2020 2020 2073 7479 6c65  ..         style
+000016d0: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 3766  ="stop-color:#7f
+000016e0: 3766 3766 3b73 746f 702d 6f70 6163 6974  7f7f;stop-opacit
+000016f0: 793a 3022 0d0a 2020 2020 2020 2020 206f  y:0"..         o
+00001700: 6666 7365 743d 2231 220d 0a20 2020 2020  ffset="1"..     
+00001710: 2020 2020 6964 3d22 7374 6f70 3237 3939      id="stop2799
+00001720: 2220 2f3e 0d0a 2020 2020 3c2f 6c69 6e65  " />..    </line
+00001730: 6172 4772 6164 6965 6e74 3e0d 0a20 2020  arGradient>..   
+00001740: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
+00001750: 0d0a 2020 2020 2020 2069 643d 226c 696e  ..       id="lin
+00001760: 6561 7247 7261 6469 656e 7432 3738 3722  earGradient2787"
+00001770: 3e0d 0a20 2020 2020 203c 7374 6f70 0d0a  >..      <stop..
+00001780: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00001790: 7374 6f70 2d63 6f6c 6f72 3a23 3766 3766  stop-color:#7f7f
+000017a0: 3766 3b73 746f 702d 6f70 6163 6974 793a  7f;stop-opacity:
+000017b0: 302e 3522 0d0a 2020 2020 2020 2020 206f  0.5"..         o
+000017c0: 6666 7365 743d 2230 220d 0a20 2020 2020  ffset="0"..     
+000017d0: 2020 2020 6964 3d22 7374 6f70 3237 3839      id="stop2789
+000017e0: 2220 2f3e 0d0a 2020 2020 2020 3c73 746f  " />..      <sto
+000017f0: 700d 0a20 2020 2020 2020 2020 7374 796c  p..         styl
+00001800: 653d 2273 746f 702d 636f 6c6f 723a 2337  e="stop-color:#7
+00001810: 6637 6637 663b 7374 6f70 2d6f 7061 6369  f7f7f;stop-opaci
+00001820: 7479 3a30 220d 0a20 2020 2020 2020 2020  ty:0"..         
+00001830: 6f66 6673 6574 3d22 3122 0d0a 2020 2020  offset="1"..    
+00001840: 2020 2020 2069 643d 2273 746f 7032 3739       id="stop279
+00001850: 3122 202f 3e0d 0a20 2020 203c 2f6c 696e  1" />..    </lin
+00001860: 6561 7247 7261 6469 656e 743e 0d0a 2020  earGradient>..  
+00001870: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
+00001880: 740d 0a20 2020 2020 2020 6964 3d22 6c69  t..       id="li
+00001890: 6e65 6172 4772 6164 6965 6e74 3336 3736  nearGradient3676
+000018a0: 223e 0d0a 2020 2020 2020 3c73 746f 700d  ">..      <stop.
+000018b0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000018c0: 2273 746f 702d 636f 6c6f 723a 2362 3262  "stop-color:#b2b
+000018d0: 3262 323b 7374 6f70 2d6f 7061 6369 7479  2b2;stop-opacity
+000018e0: 3a30 2e35 220d 0a20 2020 2020 2020 2020  :0.5"..         
+000018f0: 6f66 6673 6574 3d22 3022 0d0a 2020 2020  offset="0"..    
+00001900: 2020 2020 2069 643d 2273 746f 7033 3637       id="stop367
+00001910: 3822 202f 3e0d 0a20 2020 2020 203c 7374  8" />..      <st
+00001920: 6f70 0d0a 2020 2020 2020 2020 2073 7479  op..         sty
+00001930: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
+00001940: 6233 6233 6233 3b73 746f 702d 6f70 6163  b3b3b3;stop-opac
+00001950: 6974 793a 3022 0d0a 2020 2020 2020 2020  ity:0"..        
+00001960: 206f 6666 7365 743d 2231 220d 0a20 2020   offset="1"..   
+00001970: 2020 2020 2020 6964 3d22 7374 6f70 3336        id="stop36
+00001980: 3830 2220 2f3e 0d0a 2020 2020 3c2f 6c69  80" />..    </li
+00001990: 6e65 6172 4772 6164 6965 6e74 3e0d 0a20  nearGradient>.. 
+000019a0: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
+000019b0: 6e74 0d0a 2020 2020 2020 2069 643d 226c  nt..       id="l
+000019c0: 696e 6561 7247 7261 6469 656e 7433 3233  inearGradient323
+000019d0: 3622 3e0d 0a20 2020 2020 203c 7374 6f70  6">..      <stop
+000019e0: 0d0a 2020 2020 2020 2020 2073 7479 6c65  ..         style
+000019f0: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 6634  ="stop-color:#f4
+00001a00: 6634 6634 3b73 746f 702d 6f70 6163 6974  f4f4;stop-opacit
+00001a10: 793a 3122 0d0a 2020 2020 2020 2020 206f  y:1"..         o
+00001a20: 6666 7365 743d 2230 220d 0a20 2020 2020  ffset="0"..     
+00001a30: 2020 2020 6964 3d22 7374 6f70 3332 3434      id="stop3244
+00001a40: 2220 2f3e 0d0a 2020 2020 2020 3c73 746f  " />..      <sto
+00001a50: 700d 0a20 2020 2020 2020 2020 7374 796c  p..         styl
+00001a60: 653d 2273 746f 702d 636f 6c6f 723a 2366  e="stop-color:#f
+00001a70: 6666 6666 663b 7374 6f70 2d6f 7061 6369  fffff;stop-opaci
+00001a80: 7479 3a31 220d 0a20 2020 2020 2020 2020  ty:1"..         
+00001a90: 6f66 6673 6574 3d22 3122 0d0a 2020 2020  offset="1"..    
+00001aa0: 2020 2020 2069 643d 2273 746f 7033 3234       id="stop324
+00001ab0: 3022 202f 3e0d 0a20 2020 203c 2f6c 696e  0" />..    </lin
+00001ac0: 6561 7247 7261 6469 656e 743e 0d0a 2020  earGradient>..  
+00001ad0: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
+00001ae0: 740d 0a20 2020 2020 2020 6964 3d22 6c69  t..       id="li
+00001af0: 6e65 6172 4772 6164 6965 6e74 3436 3731  nearGradient4671
+00001b00: 223e 0d0a 2020 2020 2020 3c73 746f 700d  ">..      <stop.
+00001b10: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00001b20: 2273 746f 702d 636f 6c6f 723a 2366 6664  "stop-color:#ffd
+00001b30: 3433 623b 7374 6f70 2d6f 7061 6369 7479  43b;stop-opacity
+00001b40: 3a31 220d 0a20 2020 2020 2020 2020 6f66  :1"..         of
+00001b50: 6673 6574 3d22 3022 0d0a 2020 2020 2020  fset="0"..      
+00001b60: 2020 2069 643d 2273 746f 7034 3637 3322     id="stop4673"
+00001b70: 202f 3e0d 0a20 2020 2020 203c 7374 6f70   />..      <stop
+00001b80: 0d0a 2020 2020 2020 2020 2073 7479 6c65  ..         style
+00001b90: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 6666  ="stop-color:#ff
+00001ba0: 6538 3733 3b73 746f 702d 6f70 6163 6974  e873;stop-opacit
+00001bb0: 793a 3122 0d0a 2020 2020 2020 2020 206f  y:1"..         o
+00001bc0: 6666 7365 743d 2231 220d 0a20 2020 2020  ffset="1"..     
+00001bd0: 2020 2020 6964 3d22 7374 6f70 3436 3735      id="stop4675
+00001be0: 2220 2f3e 0d0a 2020 2020 3c2f 6c69 6e65  " />..    </line
+00001bf0: 6172 4772 6164 6965 6e74 3e0d 0a20 2020  arGradient>..   
+00001c00: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
+00001c10: 0d0a 2020 2020 2020 2069 643d 226c 696e  ..       id="lin
+00001c20: 6561 7247 7261 6469 656e 7434 3638 3922  earGradient4689"
+00001c30: 3e0d 0a20 2020 2020 203c 7374 6f70 0d0a  >..      <stop..
+00001c40: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00001c50: 7374 6f70 2d63 6f6c 6f72 3a23 3561 3966  stop-color:#5a9f
+00001c60: 6434 3b73 746f 702d 6f70 6163 6974 793a  d4;stop-opacity:
+00001c70: 3122 0d0a 2020 2020 2020 2020 206f 6666  1"..         off
+00001c80: 7365 743d 2230 220d 0a20 2020 2020 2020  set="0"..       
+00001c90: 2020 6964 3d22 7374 6f70 3436 3931 2220    id="stop4691" 
+00001ca0: 2f3e 0d0a 2020 2020 2020 3c73 746f 700d  />..      <stop.
+00001cb0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00001cc0: 2273 746f 702d 636f 6c6f 723a 2333 3036  "stop-color:#306
+00001cd0: 3939 383b 7374 6f70 2d6f 7061 6369 7479  998;stop-opacity
+00001ce0: 3a31 220d 0a20 2020 2020 2020 2020 6f66  :1"..         of
+00001cf0: 6673 6574 3d22 3122 0d0a 2020 2020 2020  fset="1"..      
+00001d00: 2020 2069 643d 2273 746f 7034 3639 3322     id="stop4693"
+00001d10: 202f 3e0d 0a20 2020 203c 2f6c 696e 6561   />..    </linea
+00001d20: 7247 7261 6469 656e 743e 0d0a 2020 2020  rGradient>..    
+00001d30: 3c6c 696e 6561 7247 7261 6469 656e 740d  <linearGradient.
+00001d40: 0a20 2020 2020 2020 7831 3d22 3232 342e  .       x1="224.
+00001d50: 3233 3939 3622 0d0a 2020 2020 2020 2079  23996"..       y
+00001d60: 313d 2231 3434 2e37 3537 3137 220d 0a20  1="144.75717".. 
+00001d70: 2020 2020 2020 7832 3d22 2d36 352e 3330        x2="-65.30
+00001d80: 3835 3032 220d 0a20 2020 2020 2020 7932  8502"..       y2
+00001d90: 3d22 3134 342e 3735 3731 3722 0d0a 2020  ="144.75717"..  
+00001da0: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
+00001db0: 7261 6469 656e 7432 3938 3722 0d0a 2020  radient2987"..  
+00001dc0: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
+00001dd0: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
+00001de0: 3436 3731 220d 0a20 2020 2020 2020 6772  4671"..       gr
+00001df0: 6164 6965 6e74 556e 6974 733d 2275 7365  adientUnits="use
+00001e00: 7253 7061 6365 4f6e 5573 6522 0d0a 2020  rSpaceOnUse"..  
+00001e10: 2020 2020 2067 7261 6469 656e 7454 7261       gradientTra
+00001e20: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+00001e30: 6528 3130 302e 3237 3032 2c39 392e 3631  e(100.2702,99.61
+00001e40: 3131 3629 2220 2f3e 0d0a 2020 2020 3c6c  116)" />..    <l
+00001e50: 696e 6561 7247 7261 6469 656e 740d 0a20  inearGradient.. 
+00001e60: 2020 2020 2020 7831 3d22 3137 322e 3934        x1="172.94
+00001e70: 3230 3822 0d0a 2020 2020 2020 2079 313d  208"..       y1=
+00001e80: 2237 372e 3437 3539 3833 220d 0a20 2020  "77.475983"..   
+00001e90: 2020 2020 7832 3d22 3236 2e36 3730 3239      x2="26.67029
+00001ea0: 3822 0d0a 2020 2020 2020 2079 323d 2237  8"..       y2="7
+00001eb0: 362e 3331 3331 3333 220d 0a20 2020 2020  6.313133"..     
+00001ec0: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
+00001ed0: 6965 6e74 3239 3930 220d 0a20 2020 2020  ient2990"..     
+00001ee0: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
+00001ef0: 696e 6561 7247 7261 6469 656e 7434 3638  inearGradient468
+00001f00: 3922 0d0a 2020 2020 2020 2067 7261 6469  9"..       gradi
+00001f10: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00001f20: 6163 654f 6e55 7365 220d 0a20 2020 2020  aceOnUse"..     
+00001f30: 2020 6772 6164 6965 6e74 5472 616e 7366    gradientTransf
+00001f40: 6f72 6d3d 2274 7261 6e73 6c61 7465 2831  orm="translate(1
+00001f50: 3030 2e32 3730 322c 3939 2e36 3131 3136  00.2702,99.61116
+00001f60: 2922 202f 3e0d 0a20 2020 203c 6c69 6e65  )" />..    <line
+00001f70: 6172 4772 6164 6965 6e74 0d0a 2020 2020  arGradient..    
+00001f80: 2020 2078 313d 2231 3732 2e39 3432 3038     x1="172.94208
+00001f90: 220d 0a20 2020 2020 2020 7931 3d22 3737  "..       y1="77
+00001fa0: 2e34 3735 3938 3322 0d0a 2020 2020 2020  .475983"..      
+00001fb0: 2078 323d 2232 362e 3637 3032 3938 220d   x2="26.670298".
+00001fc0: 0a20 2020 2020 2020 7932 3d22 3736 2e33  .       y2="76.3
+00001fd0: 3133 3133 3322 0d0a 2020 2020 2020 2069  13133"..       i
+00001fe0: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
+00001ff0: 7432 3538 3722 0d0a 2020 2020 2020 2078  t2587"..       x
+00002000: 6c69 6e6b 3a68 7265 663d 2223 6c69 6e65  link:href="#line
+00002010: 6172 4772 6164 6965 6e74 3436 3839 220d  arGradient4689".
+00002020: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+00002030: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
+00002040: 4f6e 5573 6522 0d0a 2020 2020 2020 2067  OnUse"..       g
+00002050: 7261 6469 656e 7454 7261 6e73 666f 726d  radientTransform
+00002060: 3d22 7472 616e 736c 6174 6528 3130 302e  ="translate(100.
+00002070: 3237 3032 2c39 392e 3631 3131 3629 2220  2702,99.61116)" 
+00002080: 2f3e 0d0a 2020 2020 3c6c 696e 6561 7247  />..    <linearG
+00002090: 7261 6469 656e 740d 0a20 2020 2020 2020  radient..       
+000020a0: 7831 3d22 3232 342e 3233 3939 3622 0d0a  x1="224.23996"..
+000020b0: 2020 2020 2020 2079 313d 2231 3434 2e37         y1="144.7
+000020c0: 3537 3137 220d 0a20 2020 2020 2020 7832  5717"..       x2
+000020d0: 3d22 2d36 352e 3330 3835 3032 220d 0a20  ="-65.308502".. 
+000020e0: 2020 2020 2020 7932 3d22 3134 342e 3735        y2="144.75
+000020f0: 3731 3722 0d0a 2020 2020 2020 2069 643d  717"..       id=
+00002100: 226c 696e 6561 7247 7261 6469 656e 7432  "linearGradient2
+00002110: 3538 3922 0d0a 2020 2020 2020 2078 6c69  589"..       xli
+00002120: 6e6b 3a68 7265 663d 2223 6c69 6e65 6172  nk:href="#linear
+00002130: 4772 6164 6965 6e74 3436 3731 220d 0a20  Gradient4671".. 
+00002140: 2020 2020 2020 6772 6164 6965 6e74 556e        gradientUn
+00002150: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
+00002160: 5573 6522 0d0a 2020 2020 2020 2067 7261  Use"..       gra
+00002170: 6469 656e 7454 7261 6e73 666f 726d 3d22  dientTransform="
+00002180: 7472 616e 736c 6174 6528 3130 302e 3237  translate(100.27
+00002190: 3032 2c39 392e 3631 3131 3629 2220 2f3e  02,99.61116)" />
+000021a0: 0d0a 2020 2020 3c6c 696e 6561 7247 7261  ..    <linearGra
+000021b0: 6469 656e 740d 0a20 2020 2020 2020 7831  dient..       x1
+000021c0: 3d22 3137 322e 3934 3230 3822 0d0a 2020  ="172.94208"..  
+000021d0: 2020 2020 2079 313d 2237 372e 3437 3539       y1="77.4759
+000021e0: 3833 220d 0a20 2020 2020 2020 7832 3d22  83"..       x2="
+000021f0: 3236 2e36 3730 3239 3822 0d0a 2020 2020  26.670298"..    
+00002200: 2020 2079 323d 2237 362e 3331 3331 3333     y2="76.313133
+00002210: 220d 0a20 2020 2020 2020 6964 3d22 6c69  "..       id="li
+00002220: 6e65 6172 4772 6164 6965 6e74 3232 3438  nearGradient2248
+00002230: 220d 0a20 2020 2020 2020 786c 696e 6b3a  "..       xlink:
+00002240: 6872 6566 3d22 236c 696e 6561 7247 7261  href="#linearGra
+00002250: 6469 656e 7434 3638 3922 0d0a 2020 2020  dient4689"..    
+00002260: 2020 2067 7261 6469 656e 7455 6e69 7473     gradientUnits
+00002270: 3d22 7573 6572 5370 6163 654f 6e55 7365  ="userSpaceOnUse
+00002280: 220d 0a20 2020 2020 2020 6772 6164 6965  "..       gradie
+00002290: 6e74 5472 616e 7366 6f72 6d3d 2274 7261  ntTransform="tra
+000022a0: 6e73 6c61 7465 2831 3030 2e32 3730 322c  nslate(100.2702,
+000022b0: 3939 2e36 3131 3136 2922 202f 3e0d 0a20  99.61116)" />.. 
+000022c0: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
+000022d0: 6e74 0d0a 2020 2020 2020 2078 313d 2232  nt..       x1="2
+000022e0: 3234 2e32 3339 3936 220d 0a20 2020 2020  24.23996"..     
+000022f0: 2020 7931 3d22 3134 342e 3735 3731 3722    y1="144.75717"
+00002300: 0d0a 2020 2020 2020 2078 323d 222d 3635  ..       x2="-65
+00002310: 2e33 3038 3530 3222 0d0a 2020 2020 2020  .308502"..      
+00002320: 2079 323d 2231 3434 2e37 3537 3137 220d   y2="144.75717".
+00002330: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
+00002340: 6172 4772 6164 6965 6e74 3232 3530 220d  arGradient2250".
+00002350: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
+00002360: 6566 3d22 236c 696e 6561 7247 7261 6469  ef="#linearGradi
+00002370: 656e 7434 3637 3122 0d0a 2020 2020 2020  ent4671"..      
+00002380: 2067 7261 6469 656e 7455 6e69 7473 3d22   gradientUnits="
+00002390: 7573 6572 5370 6163 654f 6e55 7365 220d  userSpaceOnUse".
+000023a0: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+000023b0: 5472 616e 7366 6f72 6d3d 2274 7261 6e73  Transform="trans
+000023c0: 6c61 7465 2831 3030 2e32 3730 322c 3939  late(100.2702,99
+000023d0: 2e36 3131 3136 2922 202f 3e0d 0a20 2020  .61116)" />..   
+000023e0: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
+000023f0: 0d0a 2020 2020 2020 2078 313d 2232 3234  ..       x1="224
+00002400: 2e32 3339 3936 220d 0a20 2020 2020 2020  .23996"..       
+00002410: 7931 3d22 3134 342e 3735 3731 3722 0d0a  y1="144.75717"..
+00002420: 2020 2020 2020 2078 323d 222d 3635 2e33         x2="-65.3
+00002430: 3038 3530 3222 0d0a 2020 2020 2020 2079  08502"..       y
+00002440: 323d 2231 3434 2e37 3537 3137 220d 0a20  2="144.75717".. 
+00002450: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
+00002460: 4772 6164 6965 6e74 3232 3535 220d 0a20  Gradient2255".. 
+00002470: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
+00002480: 3d22 236c 696e 6561 7247 7261 6469 656e  ="#linearGradien
+00002490: 7434 3637 3122 0d0a 2020 2020 2020 2067  t4671"..       g
+000024a0: 7261 6469 656e 7455 6e69 7473 3d22 7573  radientUnits="us
+000024b0: 6572 5370 6163 654f 6e55 7365 220d 0a20  erSpaceOnUse".. 
+000024c0: 2020 2020 2020 6772 6164 6965 6e74 5472        gradientTr
+000024d0: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
+000024e0: 302e 3536 3235 3431 2c30 2c30 2c30 2e35  0.562541,0,0,0.5
+000024f0: 3637 3937 322c 2d31 312e 3539 3734 2c2d  67972,-11.5974,-
+00002500: 372e 3630 3935 3429 2220 2f3e 0d0a 2020  7.60954)" />..  
+00002510: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
+00002520: 740d 0a20 2020 2020 2020 7831 3d22 3137  t..       x1="17
+00002530: 322e 3934 3230 3822 0d0a 2020 2020 2020  2.94208"..      
+00002540: 2079 313d 2237 362e 3137 3632 3234 220d   y1="76.176224".
+00002550: 0a20 2020 2020 2020 7832 3d22 3236 2e36  .       x2="26.6
+00002560: 3730 3239 3822 0d0a 2020 2020 2020 2079  70298"..       y
+00002570: 323d 2237 362e 3331 3331 3333 220d 0a20  2="76.313133".. 
+00002580: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
+00002590: 4772 6164 6965 6e74 3232 3538 220d 0a20  Gradient2258".. 
+000025a0: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
+000025b0: 3d22 236c 696e 6561 7247 7261 6469 656e  ="#linearGradien
+000025c0: 7434 3638 3922 0d0a 2020 2020 2020 2067  t4689"..       g
+000025d0: 7261 6469 656e 7455 6e69 7473 3d22 7573  radientUnits="us
+000025e0: 6572 5370 6163 654f 6e55 7365 220d 0a20  erSpaceOnUse".. 
+000025f0: 2020 2020 2020 6772 6164 6965 6e74 5472        gradientTr
+00002600: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
+00002610: 302e 3536 3235 3431 2c30 2c30 2c30 2e35  0.562541,0,0,0.5
+00002620: 3637 3937 322c 2d31 312e 3539 3734 2c2d  67972,-11.5974,-
+00002630: 372e 3630 3935 3429 2220 2f3e 0d0a 2020  7.60954)" />..  
+00002640: 2020 3c72 6164 6961 6c47 7261 6469 656e    <radialGradien
+00002650: 740d 0a20 2020 2020 2020 6378 3d22 3631  t..       cx="61
+00002660: 2e35 3138 3838 3322 0d0a 2020 2020 2020  .518883"..      
+00002670: 2063 793d 2231 3332 2e32 3835 3735 220d   cy="132.28575".
+00002680: 0a20 2020 2020 2020 723d 2232 392e 3033  .       r="29.03
+00002690: 3639 3133 220d 0a20 2020 2020 2020 6678  6913"..       fx
+000026a0: 3d22 3631 2e35 3138 3838 3322 0d0a 2020  ="61.518883"..  
+000026b0: 2020 2020 2066 793d 2231 3332 2e32 3835       fy="132.285
+000026c0: 3735 220d 0a20 2020 2020 2020 6964 3d22  75"..       id="
+000026d0: 7261 6469 616c 4772 6164 6965 6e74 3238  radialGradient28
+000026e0: 3031 220d 0a20 2020 2020 2020 786c 696e  01"..       xlin
+000026f0: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
+00002700: 7261 6469 656e 7432 3739 3522 0d0a 2020  radient2795"..  
+00002710: 2020 2020 2067 7261 6469 656e 7455 6e69       gradientUni
+00002720: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
+00002730: 7365 220d 0a20 2020 2020 2020 6772 6164  se"..       grad
+00002740: 6965 6e74 5472 616e 7366 6f72 6d3d 226d  ientTransform="m
+00002750: 6174 7269 7828 312c 302c 302c 302e 3137  atrix(1,0,0,0.17
+00002760: 3739 3636 2c30 2c31 3038 2e37 3433 3429  7966,0,108.7434)
+00002770: 2220 2f3e 0d0a 2020 2020 3c6c 696e 6561  " />..    <linea
+00002780: 7247 7261 6469 656e 740d 0a20 2020 2020  rGradient..     
+00002790: 2020 7831 3d22 3135 302e 3936 3131 3122    x1="150.96111"
+000027a0: 0d0a 2020 2020 2020 2079 313d 2231 3932  ..       y1="192
+000027b0: 2e33 3531 3736 220d 0a20 2020 2020 2020  .35176"..       
+000027c0: 7832 3d22 3131 322e 3033 3134 3422 0d0a  x2="112.03144"..
+000027d0: 2020 2020 2020 2079 323d 2231 3337 2e32         y2="137.2
+000027e0: 3732 3939 220d 0a20 2020 2020 2020 6964  7299"..       id
+000027f0: 3d22 6c69 6e65 6172 4772 6164 6965 6e74  ="linearGradient
+00002800: 3134 3735 220d 0a20 2020 2020 2020 786c  1475"..       xl
+00002810: 696e 6b3a 6872 6566 3d22 236c 696e 6561  ink:href="#linea
+00002820: 7247 7261 6469 656e 7434 3637 3122 0d0a  rGradient4671"..
+00002830: 2020 2020 2020 2067 7261 6469 656e 7455         gradientU
+00002840: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
+00002850: 6e55 7365 220d 0a20 2020 2020 2020 6772  nUse"..       gr
+00002860: 6164 6965 6e74 5472 616e 7366 6f72 6d3d  adientTransform=
+00002870: 226d 6174 7269 7828 302e 3536 3235 3431  "matrix(0.562541
+00002880: 2c30 2c30 2c30 2e35 3637 3937 322c 2d39  ,0,0,0.567972,-9
+00002890: 2e33 3939 3734 392c 2d35 2e33 3035 3331  .399749,-5.30531
+000028a0: 3729 2220 2f3e 0d0a 2020 2020 3c6c 696e  7)" />..    <lin
+000028b0: 6561 7247 7261 6469 656e 740d 0a20 2020  earGradient..   
+000028c0: 2020 2020 7831 3d22 3236 2e36 3438 3933      x1="26.64893
+000028d0: 3722 0d0a 2020 2020 2020 2079 313d 2232  7"..       y1="2
+000028e0: 302e 3630 3337 3831 220d 0a20 2020 2020  0.603781"..     
+000028f0: 2020 7832 3d22 3133 352e 3636 3532 3522    x2="135.66525"
+00002900: 0d0a 2020 2020 2020 2079 323d 2231 3134  ..       y2="114
+00002910: 2e33 3937 3637 220d 0a20 2020 2020 2020  .39767"..       
+00002920: 6964 3d22 6c69 6e65 6172 4772 6164 6965  id="linearGradie
+00002930: 6e74 3134 3738 220d 0a20 2020 2020 2020  nt1478"..       
+00002940: 786c 696e 6b3a 6872 6566 3d22 236c 696e  xlink:href="#lin
+00002950: 6561 7247 7261 6469 656e 7434 3638 3922  earGradient4689"
+00002960: 0d0a 2020 2020 2020 2067 7261 6469 656e  ..       gradien
+00002970: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
+00002980: 654f 6e55 7365 220d 0a20 2020 2020 2020  eOnUse"..       
+00002990: 6772 6164 6965 6e74 5472 616e 7366 6f72  gradientTransfor
+000029a0: 6d3d 226d 6174 7269 7828 302e 3536 3235  m="matrix(0.5625
+000029b0: 3431 2c30 2c30 2c30 2e35 3637 3937 322c  41,0,0,0.567972,
+000029c0: 2d39 2e33 3939 3734 392c 2d35 2e33 3035  -9.399749,-5.305
+000029d0: 3331 3729 2220 2f3e 0d0a 2020 2020 3c72  317)" />..    <r
+000029e0: 6164 6961 6c47 7261 6469 656e 740d 0a20  adialGradient.. 
+000029f0: 2020 2020 2020 6378 3d22 3631 2e35 3138        cx="61.518
+00002a00: 3838 3322 0d0a 2020 2020 2020 2063 793d  883"..       cy=
+00002a10: 2231 3332 2e32 3835 3735 220d 0a20 2020  "132.28575"..   
+00002a20: 2020 2020 723d 2232 392e 3033 3639 3133      r="29.036913
+00002a30: 220d 0a20 2020 2020 2020 6678 3d22 3631  "..       fx="61
+00002a40: 2e35 3138 3838 3322 0d0a 2020 2020 2020  .518883"..      
+00002a50: 2066 793d 2231 3332 2e32 3835 3735 220d   fy="132.28575".
+00002a60: 0a20 2020 2020 2020 6964 3d22 7261 6469  .       id="radi
+00002a70: 616c 4772 6164 6965 6e74 3134 3830 220d  alGradient1480".
+00002a80: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
+00002a90: 6566 3d22 236c 696e 6561 7247 7261 6469  ef="#linearGradi
+00002aa0: 656e 7432 3739 3522 0d0a 2020 2020 2020  ent2795"..      
+00002ab0: 2067 7261 6469 656e 7455 6e69 7473 3d22   gradientUnits="
+00002ac0: 7573 6572 5370 6163 654f 6e55 7365 220d  userSpaceOnUse".
+00002ad0: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+00002ae0: 5472 616e 7366 6f72 6d3d 226d 6174 7269  Transform="matri
+00002af0: 7828 322e 3338 3237 3136 652d 382c 2d30  x(2.382716e-8,-0
+00002b00: 2e32 3936 3430 352c 312e 3433 3637 362c  .296405,1.43676,
+00002b10: 342e 3638 3336 3733 652d 372c 2d31 3238  4.683673e-7,-128
+00002b20: 2e35 3434 2c31 3530 2e35 3230 3229 2220  .544,150.5202)" 
+00002b30: 2f3e 0d0a 2020 2020 3c72 6164 6961 6c47  />..    <radialG
+00002b40: 7261 6469 656e 740d 0a20 2020 2020 2020  radient..       
+00002b50: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
+00002b60: 3d22 616c 7761 7973 220d 0a20 2020 2020  ="always"..     
+00002b70: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
+00002b80: 696e 6561 7247 7261 6469 656e 7432 3739  inearGradient279
+00002b90: 3522 0d0a 2020 2020 2020 2069 643d 2272  5"..       id="r
+00002ba0: 6164 6961 6c47 7261 6469 656e 7432 3432  adialGradient242
+00002bb0: 3122 0d0a 2020 2020 2020 2067 7261 6469  1"..       gradi
+00002bc0: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00002bd0: 6163 654f 6e55 7365 220d 0a20 2020 2020  aceOnUse"..     
+00002be0: 2020 6772 6164 6965 6e74 5472 616e 7366    gradientTransf
+00002bf0: 6f72 6d3d 226d 6174 7269 7828 312e 3734  orm="matrix(1.74
+00002c00: 3930 3536 3565 2d38 2c2d 302e 3233 3939  90565e-8,-0.2399
+00002c10: 3437 2c31 2e30 3534 3636 382c 332e 3739  47,1.054668,3.79
+00002c20: 3135 3435 3765 2d37 2c2d 3738 2e31 3039  15457e-7,-78.109
+00002c30: 3432 392c 3134 382e 3835 3930 3629 220d  429,148.85906)".
+00002c40: 0a20 2020 2020 2020 6378 3d22 3631 2e35  .       cx="61.5
+00002c50: 3138 3838 3322 0d0a 2020 2020 2020 2063  18883"..       c
+00002c60: 793d 2231 3332 2e32 3835 3735 220d 0a20  y="132.28575".. 
+00002c70: 2020 2020 2020 6678 3d22 3631 2e35 3138        fx="61.518
+00002c80: 3838 3322 0d0a 2020 2020 2020 2066 793d  883"..       fy=
+00002c90: 2231 3332 2e32 3835 3735 220d 0a20 2020  "132.28575"..   
+00002ca0: 2020 2020 723d 2232 392e 3033 3639 3133      r="29.036913
+00002cb0: 2220 2f3e 0d0a 2020 2020 3c6c 696e 6561  " />..    <linea
+00002cc0: 7247 7261 6469 656e 740d 0a20 2020 2020  rGradient..     
+00002cd0: 2020 696e 6b73 6361 7065 3a63 6f6c 6c65    inkscape:colle
+00002ce0: 6374 3d22 616c 7761 7973 220d 0a20 2020  ct="always"..   
+00002cf0: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00002d00: 236c 696e 6561 7247 7261 6469 656e 7434  #linearGradient4
+00002d10: 3637 312d 3822 0d0a 2020 2020 2020 2069  671-8"..       i
+00002d20: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
+00002d30: 7433 3832 362d 3622 0d0a 2020 2020 2020  t3826-6"..      
+00002d40: 2078 313d 2233 362e 3937 3038 3938 220d   x1="36.970898".
+00002d50: 0a20 2020 2020 2020 7931 3d22 3534 2e36  .       y1="54.6
+00002d60: 3436 3736 3322 0d0a 2020 2020 2020 2078  46763"..       x
+00002d70: 323d 2238 372e 3730 3436 3831 220d 0a20  2="87.704681".. 
+00002d80: 2020 2020 2020 7932 3d22 3534 2e36 3436        y2="54.646
+00002d90: 3736 3322 0d0a 2020 2020 2020 2067 7261  763"..       gra
+00002da0: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
+00002db0: 5370 6163 654f 6e55 7365 2220 2f3e 0d0a  SpaceOnUse" />..
+00002dc0: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
+00002dd0: 656e 740d 0a20 2020 2020 2020 6964 3d22  ent..       id="
+00002de0: 6c69 6e65 6172 4772 6164 6965 6e74 3436  linearGradient46
+00002df0: 3731 2d38 223e 0d0a 2020 2020 2020 3c73  71-8">..      <s
+00002e00: 746f 700d 0a20 2020 2020 2020 2020 7374  top..         st
+00002e10: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
+00002e20: 2366 6664 3433 623b 7374 6f70 2d6f 7061  #ffd43b;stop-opa
+00002e30: 6369 7479 3a31 220d 0a20 2020 2020 2020  city:1"..       
+00002e40: 2020 6f66 6673 6574 3d22 3022 0d0a 2020    offset="0"..  
+00002e50: 2020 2020 2020 2069 643d 2273 746f 7034         id="stop4
+00002e60: 3637 332d 3822 202f 3e0d 0a20 2020 2020  673-8" />..     
+00002e70: 203c 7374 6f70 0d0a 2020 2020 2020 2020   <stop..        
+00002e80: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
+00002e90: 6f72 3a23 6666 6538 3733 3b73 746f 702d  or:#ffe873;stop-
+00002ea0: 6f70 6163 6974 793a 3122 0d0a 2020 2020  opacity:1"..    
+00002eb0: 2020 2020 206f 6666 7365 743d 2231 220d       offset="1".
+00002ec0: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
+00002ed0: 6f70 3436 3735 2d32 2220 2f3e 0d0a 2020  op4675-2" />..  
+00002ee0: 2020 3c2f 6c69 6e65 6172 4772 6164 6965    </linearGradie
+00002ef0: 6e74 3e0d 0a20 2020 203c 6c69 6e65 6172  nt>..    <linear
+00002f00: 4772 6164 6965 6e74 0d0a 2020 2020 2020  Gradient..      
+00002f10: 2069 6e6b 7363 6170 653a 636f 6c6c 6563   inkscape:collec
+00002f20: 743d 2261 6c77 6179 7322 0d0a 2020 2020  t="always"..    
+00002f30: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
+00002f40: 6c69 6e65 6172 4772 6164 6965 6e74 3338  linearGradient38
+00002f50: 3132 220d 0a20 2020 2020 2020 6964 3d22  12"..       id="
+00002f60: 6c69 6e65 6172 4772 6164 6965 6e74 3338  linearGradient38
+00002f70: 3138 220d 0a20 2020 2020 2020 7831 3d22  18"..       x1="
+00002f80: 3738 2e30 3132 3032 3422 0d0a 2020 2020  78.012024"..    
+00002f90: 2020 2079 313d 2238 302e 3330 3239 3333     y1="80.302933
+00002fa0: 220d 0a20 2020 2020 2020 7832 3d22 3132  "..       x2="12
+00002fb0: 342e 3637 3936 3422 0d0a 2020 2020 2020  4.67964"..      
+00002fc0: 2079 323d 2232 382e 3630 3333 3237 220d   y2="28.603327".
+00002fd0: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+00002fe0: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
+00002ff0: 4f6e 5573 6522 202f 3e0d 0a20 2020 203c  OnUse" />..    <
+00003000: 6c69 6e65 6172 4772 6164 6965 6e74 0d0a  linearGradient..
+00003010: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00003020: 636f 6c6c 6563 743d 2261 6c77 6179 7322  collect="always"
+00003030: 0d0a 2020 2020 2020 2078 6c69 6e6b 3a68  ..       xlink:h
+00003040: 7265 663d 2223 6c69 6e65 6172 4772 6164  ref="#linearGrad
+00003050: 6965 6e74 3338 3132 220d 0a20 2020 2020  ient3812"..     
+00003060: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
+00003070: 6965 6e74 3430 3937 220d 0a20 2020 2020  ient4097"..     
+00003080: 2020 7831 3d22 2d32 3035 2e30 3534 3331    x1="-205.05431
+00003090: 220d 0a20 2020 2020 2020 7931 3d22 3535  "..       y1="55
+000030a0: 2e36 3036 3434 3122 0d0a 2020 2020 2020  .606441"..      
+000030b0: 2078 323d 222d 3634 2e38 3036 3235 3922   x2="-64.806259"
+000030c0: 0d0a 2020 2020 2020 2079 323d 2235 352e  ..       y2="55.
+000030d0: 3630 3634 3431 220d 0a20 2020 2020 2020  606441"..       
+000030e0: 6772 6164 6965 6e74 556e 6974 733d 2275  gradientUnits="u
+000030f0: 7365 7253 7061 6365 4f6e 5573 6522 0d0a  serSpaceOnUse"..
+00003100: 2020 2020 2020 2067 7261 6469 656e 7454         gradientT
+00003110: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+00003120: 2831 2e30 3935 3135 3339 2c30 2c30 2c31  (1.0951539,0,0,1
+00003130: 2e30 3331 3532 3638 2c32 3233 2e34 3935  .0315268,223.495
+00003140: 312c 342e 3530 3734 3431 3429 2220 2f3e  1,4.5074414)" />
+00003150: 0d0a 2020 2020 3c6c 696e 6561 7247 7261  ..    <linearGra
+00003160: 6469 656e 740d 0a20 2020 2020 2020 696e  dient..       in
+00003170: 6b73 6361 7065 3a63 6f6c 6c65 6374 3d22  kscape:collect="
+00003180: 616c 7761 7973 220d 0a20 2020 2020 2020  always"..       
+00003190: 786c 696e 6b3a 6872 6566 3d22 236c 696e  xlink:href="#lin
+000031a0: 6561 7247 7261 6469 656e 7431 3839 3422  earGradient1894"
+000031b0: 0d0a 2020 2020 2020 2069 643d 226c 696e  ..       id="lin
+000031c0: 6561 7247 7261 6469 656e 7434 3039 372d  earGradient4097-
+000031d0: 3422 0d0a 2020 2020 2020 2078 313d 222d  4"..       x1="-
+000031e0: 3230 352e 3035 3433 3122 0d0a 2020 2020  205.05431"..    
+000031f0: 2020 2079 313d 2235 352e 3630 3634 3431     y1="55.606441
+00003200: 220d 0a20 2020 2020 2020 7832 3d22 2d36  "..       x2="-6
+00003210: 342e 3830 3632 3539 220d 0a20 2020 2020  4.806259"..     
+00003220: 2020 7932 3d22 3535 2e36 3036 3434 3122    y2="55.606441"
+00003230: 0d0a 2020 2020 2020 2067 7261 6469 656e  ..       gradien
+00003240: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
+00003250: 654f 6e55 7365 220d 0a20 2020 2020 2020  eOnUse"..       
+00003260: 6772 6164 6965 6e74 5472 616e 7366 6f72  gradientTransfor
+00003270: 6d3d 2274 7261 6e73 6c61 7465 2832 3131  m="translate(211
+00003280: 2e39 3330 3239 2c35 2e34 3732 3539 3633  .93029,5.4725963
+00003290: 2922 202f 3e0d 0a20 2020 203c 6c69 6e65  )" />..    <line
+000032a0: 6172 4772 6164 6965 6e74 0d0a 2020 2020  arGradient..    
+000032b0: 2020 2069 643d 226c 696e 6561 7247 7261     id="linearGra
+000032c0: 6469 656e 7431 3839 3422 3e0d 0a20 2020  dient1894">..   
+000032d0: 2020 203c 7374 6f70 0d0a 2020 2020 2020     <stop..      
+000032e0: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
+000032f0: 6f6c 6f72 3a23 6666 6633 6365 3b73 746f  olor:#fff3ce;sto
+00003300: 702d 6f70 6163 6974 793a 313b 220d 0a20  p-opacity:1;".. 
+00003310: 2020 2020 2020 2020 6f66 6673 6574 3d22          offset="
+00003320: 3022 0d0a 2020 2020 2020 2020 2069 643d  0"..         id=
+00003330: 2273 746f 7031 3839 3022 202f 3e0d 0a20  "stop1890" />.. 
+00003340: 2020 2020 203c 7374 6f70 0d0a 2020 2020       <stop..    
+00003350: 2020 2020 2073 7479 6c65 3d22 7374 6f70       style="stop
+00003360: 2d63 6f6c 6f72 3a23 6666 6538 3733 3b73  -color:#ffe873;s
+00003370: 746f 702d 6f70 6163 6974 793a 3122 0d0a  top-opacity:1"..
+00003380: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
+00003390: 2231 220d 0a20 2020 2020 2020 2020 6964  "1"..         id
+000033a0: 3d22 7374 6f70 3138 3932 2220 2f3e 0d0a  ="stop1892" />..
+000033b0: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
+000033c0: 6965 6e74 3e0d 0a20 203c 2f64 6566 733e  ient>..  </defs>
+000033d0: 0d0a 2020 3c65 6c6c 6970 7365 0d0a 2020  ..  <ellipse..  
+000033e0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a75     style="fill:u
+000033f0: 726c 2823 6c69 6e65 6172 4772 6164 6965  rl(#linearGradie
+00003400: 6e74 3430 3937 293b 6669 6c6c 2d6f 7061  nt4097);fill-opa
+00003410: 6369 7479 3a31 3b73 7472 6f6b 653a 6e6f  city:1;stroke:no
+00003420: 6e65 3b73 7472 6f6b 652d 7769 6474 683a  ne;stroke-width:
+00003430: 312e 3036 3238 363b 7374 726f 6b65 2d6f  1.06286;stroke-o
+00003440: 7061 6369 7479 3a31 220d 0a20 2020 2020  pacity:1"..     
+00003450: 6964 3d22 7061 7468 3430 3839 220d 0a20  id="path4089".. 
+00003460: 2020 2020 6378 3d22 3735 2e37 3235 3637      cx="75.72567
+00003470: 3722 0d0a 2020 2020 2063 793d 2236 312e  7"..     cy="61.
+00003480: 3836 3639 3832 220d 0a20 2020 2020 7278  866982"..     rx
+00003490: 3d22 3736 2e32 3439 3032 3322 0d0a 2020  ="76.249023"..  
+000034a0: 2020 2072 793d 2235 332e 3136 3833 3639     ry="53.168369
+000034b0: 2220 2f3e 0d0a 2020 3c65 6c6c 6970 7365  " />..  <ellipse
+000034c0: 0d0a 2020 2020 2073 7479 6c65 3d22 6669  ..     style="fi
+000034d0: 6c6c 3a75 726c 2823 6c69 6e65 6172 4772  ll:url(#linearGr
+000034e0: 6164 6965 6e74 3430 3937 2d34 293b 6669  adient4097-4);fi
+000034f0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00003500: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
+00003510: 6f70 6163 6974 793a 3122 0d0a 2020 2020  opacity:1"..    
+00003520: 2069 643d 2270 6174 6834 3038 392d 3222   id="path4089-2"
+00003530: 0d0a 2020 2020 2063 783d 2237 372e 3030  ..     cx="77.00
+00003540: 3030 3038 220d 0a20 2020 2020 6379 3d22  0008"..     cy="
+00003550: 3631 2e30 3739 3033 3722 0d0a 2020 2020  61.079037"..    
+00003560: 2072 783d 2236 392e 3632 3430 3233 220d   rx="69.624023".
+00003570: 0a20 2020 2020 7279 3d22 3531 2e35 3433  .     ry="51.543
+00003580: 3336 3922 202f 3e0d 0a20 203c 7061 7468  369" />..  <path
+00003590: 0d0a 2020 2020 2073 7479 6c65 3d22 636f  ..     style="co
+000035a0: 6c6f 723a 2330 3030 3030 303b 666f 6e74  lor:#000000;font
+000035b0: 2d73 7479 6c65 3a6e 6f72 6d61 6c3b 666f  -style:normal;fo
+000035c0: 6e74 2d76 6172 6961 6e74 3a6e 6f72 6d61  nt-variant:norma
+000035d0: 6c3b 666f 6e74 2d77 6569 6768 743a 6e6f  l;font-weight:no
+000035e0: 726d 616c 3b66 6f6e 742d 7374 7265 7463  rmal;font-stretc
+000035f0: 683a 6e6f 726d 616c 3b66 6f6e 742d 7369  h:normal;font-si
+00003600: 7a65 3a6d 6564 6975 6d3b 6c69 6e65 2d68  ze:medium;line-h
+00003610: 6569 6768 743a 6e6f 726d 616c 3b66 6f6e  eight:normal;fon
+00003620: 742d 6661 6d69 6c79 3a53 616e 733b 2d69  t-family:Sans;-i
+00003630: 6e6b 7363 6170 652d 666f 6e74 2d73 7065  nkscape-font-spe
+00003640: 6369 6669 6361 7469 6f6e 3a53 616e 733b  cification:Sans;
+00003650: 7465 7874 2d69 6e64 656e 743a 303b 7465  text-indent:0;te
+00003660: 7874 2d61 6c69 676e 3a73 7461 7274 3b74  xt-align:start;t
+00003670: 6578 742d 6465 636f 7261 7469 6f6e 3a6e  ext-decoration:n
+00003680: 6f6e 653b 7465 7874 2d64 6563 6f72 6174  one;text-decorat
+00003690: 696f 6e2d 6c69 6e65 3a6e 6f6e 653b 6c65  ion-line:none;le
+000036a0: 7474 6572 2d73 7061 6369 6e67 3a6e 6f72  tter-spacing:nor
+000036b0: 6d61 6c3b 776f 7264 2d73 7061 6369 6e67  mal;word-spacing
+000036c0: 3a6e 6f72 6d61 6c3b 7465 7874 2d74 7261  :normal;text-tra
+000036d0: 6e73 666f 726d 3a6e 6f6e 653b 7772 6974  nsform:none;writ
+000036e0: 696e 672d 6d6f 6465 3a6c 722d 7462 3b64  ing-mode:lr-tb;d
+000036f0: 6972 6563 7469 6f6e 3a6c 7472 3b62 6173  irection:ltr;bas
+00003700: 656c 696e 652d 7368 6966 743a 6261 7365  eline-shift:base
+00003710: 6c69 6e65 3b74 6578 742d 616e 6368 6f72  line;text-anchor
+00003720: 3a73 7461 7274 3b64 6973 706c 6179 3a69  :start;display:i
+00003730: 6e6c 696e 653b 6f76 6572 666c 6f77 3a76  nline;overflow:v
+00003740: 6973 6962 6c65 3b76 6973 6962 696c 6974  isible;visibilit
+00003750: 793a 7669 7369 626c 653b 6669 6c6c 3a23  y:visible;fill:#
+00003760: 6262 6262 6262 3b66 696c 6c2d 6f70 6163  bbbbbb;fill-opac
+00003770: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
+00003780: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
+00003790: 6f6e 653b 7374 726f 6b65 2d77 6964 7468  one;stroke-width
+000037a0: 3a39 2e35 3834 3632 3b6d 6172 6b65 723a  :9.58462;marker:
+000037b0: 6e6f 6e65 3b65 6e61 626c 652d 6261 636b  none;enable-back
+000037c0: 6772 6f75 6e64 3a61 6363 756d 756c 6174  ground:accumulat
+000037d0: 6522 0d0a 2020 2020 2064 3d22 6d20 3737  e"..     d="m 77
+000037e0: 2e33 3036 3835 312c 382e 3136 3934 3732  .306851,8.169472
+000037f0: 3320 6320 2d35 352e 3236 3035 3438 2c30  3 c -55.260548,0
+00003800: 202d 3737 2e34 3133 3732 312c 3230 2e30   -77.413721,20.0
+00003810: 3636 3234 3637 202d 3737 2e34 3133 3732  662467 -77.41372
+00003820: 312c 3533 2e32 3132 3033 3537 2030 2e37  1,53.2120357 0.7
+00003830: 3839 3338 3339 312c 3237 2e32 3337 3035  8938391,27.23705
+00003840: 3520 3234 2e37 3739 3436 2c34 372e 3639  5 24.77946,47.69
+00003850: 3431 3632 2034 362e 3932 3832 3939 2c35  4162 46.928299,5
+00003860: 352e 3530 3030 3432 2039 2e31 3939 3631  5.500042 9.19961
+00003870: 392c 332e 3035 3932 3620 3335 2e37 3736  9,3.05926 35.776
+00003880: 3037 312c 3332 2e39 3439 3833 2034 362e  071,32.94983 46.
+00003890: 3430 3337 3039 2c33 322e 3934 3938 3320  403709,32.94983 
+000038a0: 352e 3331 3338 3232 2c30 202d 3139 2e32  5.313822,0 -19.2
+000038b0: 3039 3335 382c 2d32 302e 3232 3835 3120  09358,-20.22851 
+000038c0: 2d31 332e 3232 3237 3832 2c2d 3234 2e36  -13.222782,-24.6
+000038d0: 3739 3335 2035 2e34 3435 3235 322c 2d34  7935 5.445252,-4
+000038e0: 2e30 3438 3338 2031 332e 3035 3230 3037  .04838 13.052007
+000038f0: 2c2d 342e 3031 3830 3320 3238 2e32 3135  ,-4.01803 28.215
+00003900: 3637 342c 2d31 302e 3737 3034 3820 3135  674,-10.77048 15
+00003910: 2e31 3633 3637 2c2d 362e 3735 3234 3520  .16367,-6.75245 
+00003920: 3435 2e31 3832 3635 2c2d 3235 2e32 3332  45.18265,-25.232
+00003930: 3139 3820 3435 2e34 3536 3335 2c2d 3533  198 45.45635,-53
+00003940: 2e30 3030 3034 3220 302c 2d33 332e 3134  .000042 0,-33.14
+00003950: 3537 3839 202d 3231 2e31 3036 3938 2c2d  5789 -21.10698,-
+00003960: 3533 2e32 3132 3033 3537 202d 3736 2e33  53.2120357 -76.3
+00003970: 3637 3532 392c 2d35 332e 3231 3230 3335  67529,-53.212035
+00003980: 3720 7a20 6d20 312e 3033 3937 3231 2c39  7 z m 1.039721,9
+00003990: 2e38 3831 3230 3037 2063 2034 362e 3032  .8812007 c 46.02
+000039a0: 3836 3538 2c30 2e32 3520 3635 2e31 3230  8658,0.25 65.120
+000039b0: 3035 382c 3134 2e31 3838 3130 3120 3635  058,14.188101 65
+000039c0: 2e31 3230 3035 382c 3433 2e33 3330 3833  .120058,43.33083
+000039d0: 3520 2d31 2e30 3431 3934 2c33 332e 3035  5 -1.04194,33.05
+000039e0: 3335 3838 202d 3335 2e39 3936 3233 2c34  3588 -35.99623,4
+000039f0: 372e 3238 3830 3632 202d 3636 2e34 3439  7.288062 -66.449
+00003a00: 352c 3437 2e35 3432 3838 3220 2d33 302e  5,47.542882 -30.
+00003a10: 3435 3332 3731 2c30 2e32 3534 3832 202d  453271,0.25482 -
+00003a20: 3636 2e39 3136 3235 2c2d 3138 2e34 3030  66.91625,-18.400
+00003a30: 3134 3520 2d36 362e 3931 3632 352c 2d34  145 -66.91625,-4
+00003a40: 372e 3534 3238 3832 2030 2c2d 3239 2e31  7.542882 0,-29.1
+00003a50: 3432 3733 3620 3232 2e32 3137 3033 352c  42736 22.217035,
+00003a60: 2d34 332e 3538 3038 3335 2036 382e 3234  -43.580835 68.24
+00003a70: 3536 3932 2c2d 3433 2e33 3330 3833 3520  5692,-43.330835 
+00003a80: 7a22 0d0a 2020 2020 2069 643d 2270 6174  z"..     id="pat
+00003a90: 6833 3033 3222 0d0a 2020 2020 2069 6e6b  h3032"..     ink
+00003aa0: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00003ab0: 6375 7276 6174 7572 653d 2230 220d 0a20  curvature="0".. 
+00003ac0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00003ad0: 6574 7970 6573 3d22 7a63 6373 737a 637a  etypes="zccsszcz
+00003ae0: 7a63 7a7a 7a22 202f 3e0d 0a20 203c 670d  zczzz" />..  <g.
+00003af0: 0a20 2020 2020 6964 3d22 6731 223e 0d0a  .     id="g1">..
+00003b00: 2020 2020 3c72 6563 740d 0a20 2020 2020      <rect..     
+00003b10: 2020 7374 796c 653d 2266 696c 6c3a 2366    style="fill:#f
+00003b20: 6666 6666 663b 7374 726f 6b65 3a23 6263  fffff;stroke:#bc
+00003b30: 6263 6263 3b73 7472 6f6b 652d 7769 6474  bcbc;stroke-widt
+00003b40: 683a 362e 3330 3030 3030 3537 3b66 696c  h:6.30000057;fil
+00003b50: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00003b60: 6b65 2d6f 7061 6369 7479 3a31 3b73 7472  ke-opacity:1;str
+00003b70: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00003b80: 6e65 220d 0a20 2020 2020 2020 6964 3d22  ne"..       id="
+00003b90: 7265 6374 3122 0d0a 2020 2020 2020 2077  rect1"..       w
+00003ba0: 6964 7468 3d22 3939 2e32 3432 3537 3722  idth="99.242577"
+00003bb0: 0d0a 2020 2020 2020 2068 6569 6768 743d  ..       height=
+00003bc0: 2235 382e 3535 3035 3634 220d 0a20 2020  "58.550564"..   
+00003bd0: 2020 2020 783d 2232 392e 3639 3834 3836      x="29.698486
+00003be0: 220d 0a20 2020 2020 2020 793d 2233 312e  "..       y="31.
+00003bf0: 3830 3337 3535 220d 0a20 2020 2020 2020  803755"..       
+00003c00: 7279 3d22 362e 3535 3331 3932 3122 202f  ry="6.5531921" /
+00003c10: 3e0d 0a20 2020 203c 7265 6374 0d0a 2020  >..    <rect..  
+00003c20: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00003c30: 3a23 6263 6263 6263 3b66 696c 6c2d 6f70  :#bcbcbc;fill-op
+00003c40: 6163 6974 793a 313b 7374 726f 6b65 3a6e  acity:1;stroke:n
+00003c50: 6f6e 653b 7374 726f 6b65 2d77 6964 7468  one;stroke-width
+00003c60: 3a31 2e36 3130 3538 3b73 7472 6f6b 652d  :1.61058;stroke-
+00003c70: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00003c80: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00003c90: 0d0a 2020 2020 2020 2069 643d 2272 6563  ..       id="rec
+00003ca0: 7431 2d31 220d 0a20 2020 2020 2020 7769  t1-1"..       wi
+00003cb0: 6474 683d 2237 2e38 3630 3835 3138 220d  dth="7.8608518".
+00003cc0: 0a20 2020 2020 2020 6865 6967 6874 3d22  .       height="
+00003cd0: 3438 2e33 3130 3636 3922 0d0a 2020 2020  48.310669"..    
+00003ce0: 2020 2078 3d22 3933 2e38 3336 3632 3422     x="93.836624"
+00003cf0: 0d0a 2020 2020 2020 2079 3d22 3336 2e39  ..       y="36.9
+00003d00: 3731 3631 3122 0d0a 2020 2020 2020 2072  71611"..       r
+00003d10: 793d 2235 2e34 3037 3130 3539 2220 2f3e  y="5.4071059" />
+00003d20: 0d0a 2020 2020 3c74 6578 740d 0a20 2020  ..    <text..   
+00003d30: 2020 2020 786d 6c3a 7370 6163 653d 2270      xml:space="p
+00003d40: 7265 7365 7276 6522 0d0a 2020 2020 2020  reserve"..      
+00003d50: 2073 7479 6c65 3d22 666f 6e74 2d77 6569   style="font-wei
+00003d60: 6768 743a 626f 6c64 3b66 6f6e 742d 7369  ght:bold;font-si
+00003d70: 7a65 3a35 342e 3332 3731 7078 3b6c 696e  ze:54.3271px;lin
+00003d80: 652d 6865 6967 6874 3a31 3b66 6f6e 742d  e-height:1;font-
+00003d90: 6661 6d69 6c79 3a43 6f72 6265 6c3b 2d69  family:Corbel;-i
+00003da0: 6e6b 7363 6170 652d 666f 6e74 2d73 7065  nkscape-font-spe
+00003db0: 6369 6669 6361 7469 6f6e 3a27 436f 7262  cification:'Corb
+00003dc0: 656c 2042 6f6c 6427 3b74 6578 742d 616c  el Bold';text-al
+00003dd0: 6967 6e3a 6365 6e74 6572 3b6c 6574 7465  ign:center;lette
+00003de0: 722d 7370 6163 696e 673a 2d35 2e33 3830  r-spacing:-5.380
+00003df0: 3738 7078 3b74 6578 742d 616e 6368 6f72  78px;text-anchor
+00003e00: 3a6d 6964 646c 653b 6669 6c6c 3a23 3338  :middle;fill:#38
+00003e10: 3465 3961 3b66 696c 6c2d 6f70 6163 6974  4e9a;fill-opacit
+00003e20: 793a 313b 7374 726f 6b65 3a6e 6f6e 653b  y:1;stroke:none;
+00003e30: 7374 726f 6b65 2d77 6964 7468 3a37 2e35  stroke-width:7.5
+00003e40: 3439 3838 3b73 7472 6f6b 652d 6461 7368  4988;stroke-dash
+00003e50: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00003e60: 652d 6f70 6163 6974 793a 3122 0d0a 2020  e-opacity:1"..  
+00003e70: 2020 2020 2078 3d22 3634 2e30 3230 3130       x="64.02010
+00003e80: 3322 0d0a 2020 2020 2020 2079 3d22 3830  3"..       y="80
+00003e90: 2e38 3234 3733 220d 0a20 2020 2020 2020  .82473"..       
+00003ea0: 6964 3d22 7465 7874 3122 0d0a 2020 2020  id="text1"..    
+00003eb0: 2020 2074 7261 6e73 666f 726d 3d22 7363     transform="sc
+00003ec0: 616c 6528 312e 3031 3630 3139 372c 302e  ale(1.0160197,0.
+00003ed0: 3938 3432 3332 3838 2922 3e3c 7473 7061  98423288)"><tspa
+00003ee0: 6e0d 0a20 2020 2020 2020 2020 736f 6469  n..         sodi
+00003ef0: 706f 6469 3a72 6f6c 653d 226c 696e 6522  podi:role="line"
+00003f00: 0d0a 2020 2020 2020 2020 2069 643d 2274  ..         id="t
+00003f10: 7370 616e 3122 0d0a 2020 2020 2020 2020  span1"..        
+00003f20: 2078 3d22 3631 2e33 3239 3731 3222 0d0a   x="61.329712"..
+00003f30: 2020 2020 2020 2020 2079 3d22 3830 2e38           y="80.8
+00003f40: 3234 3733 220d 0a20 2020 2020 2020 2020  2473"..         
+00003f50: 7374 796c 653d 2266 6f6e 742d 7374 796c  style="font-styl
+00003f60: 653a 6e6f 726d 616c 3b66 6f6e 742d 7661  e:normal;font-va
+00003f70: 7269 616e 743a 6e6f 726d 616c 3b66 6f6e  riant:normal;fon
+00003f80: 742d 7765 6967 6874 3a62 6f6c 643b 666f  t-weight:bold;fo
+00003f90: 6e74 2d73 7472 6574 6368 3a6e 6f72 6d61  nt-stretch:norma
+00003fa0: 6c3b 666f 6e74 2d66 616d 696c 793a 4172  l;font-family:Ar
+00003fb0: 6961 6c3b 2d69 6e6b 7363 6170 652d 666f  ial;-inkscape-fo
+00003fc0: 6e74 2d73 7065 6369 6669 6361 7469 6f6e  nt-specification
+00003fd0: 3a27 4172 6961 6c20 426f 6c64 273b 6669  :'Arial Bold';fi
+00003fe0: 6c6c 3a23 3338 3465 3961 3b66 696c 6c2d  ll:#384e9a;fill-
+00003ff0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00004000: 2d77 6964 7468 3a37 2e35 3439 3838 223e  -width:7.54988">
+00004010: 3031 3c2f 7473 7061 6e3e 3c2f 7465 7874  01</tspan></text
+00004020: 3e0d 0a20 203c 2f67 3e0d 0a3c 2f73 7667  >..  </g>..</svg
+00004030: 3e0d 0a                                  >..
```

### Comparing `guidata-3.4.1/guidata/images/not_found.png` & `guidata-3.5.0/guidata/images/not_found.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/python.png` & `guidata-3.5.0/guidata/images/python.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/quickview.png` & `guidata-3.5.0/guidata/images/quickview.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/save_all.png` & `guidata-3.5.0/guidata/images/save_all.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/selection.png` & `guidata-3.5.0/guidata/images/selection.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/images/settings.png` & `guidata-3.5.0/guidata/images/settings.png`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/io/__init__.py` & `guidata-3.5.0/guidata/io/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/io/base.py` & `guidata-3.5.0/guidata/io/base.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/io/h5fmt.py` & `guidata-3.5.0/guidata/io/h5fmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/io/inifmt.py` & `guidata-3.5.0/guidata/io/inifmt.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,19 +58,20 @@
         from the list of options and
         ensures it matches the expected section.
 
         Args:
             section (str): The name of the section to end.
         """
         sect = self.option.pop(-1)
-        assert (
-            sect == section
-        ), "Ending section does not match the current section: %s != %s" % (
-            sect,
-            section,
+        assert sect == section, (
+            "Ending section does not match the current section: %s != %s"
+            % (
+                sect,
+                section,
+            )
         )
 
     def group(self, option: str) -> GroupContext:
         """
         Enter a group.
 
         This returns a context manager, to be used with the `with` statement.
@@ -143,28 +144,8 @@
         val = self.conf.get(self.section, option)
         return val
 
     # Make read_bool, read_int, read_float, read_array, read_sequence, read_none
     # and read_str alias to read_any
     read_bool = read_int = read_float = read_array = read_sequence = read_dict = (
         read_none
-    ) = read_str = read_any
-
-    def read_unicode(self) -> str | None:
-        """
-        Read a unicode string from the configuration.
-
-        This method reads a unicode string from the configuration. If the value
-        read is a string or None, it returns it as is. Otherwise, it delegates
-        the read to read_str method.
-
-        Returns:
-            Union[str, None]: The unicode string read from the configuration.
-        """
-        val = self.read_any()
-        if isinstance(val, str) or val is None:
-            return val
-        else:
-            return self.read_str()
-
-    # Make read_unicode alias to read_str
-    read_unicode = read_str
+    ) = read_str = read_unicode = read_any
```

### Comparing `guidata-3.4.1/guidata/io/jsonfmt.py` & `guidata-3.5.0/guidata/io/jsonfmt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/locale/fr/LC_MESSAGES/guidata.mo` & `guidata-3.5.0/guidata/locale/fr/LC_MESSAGES/guidata.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2024-01-26 15:21+0100\n"
+"POT-Creation-Date: 2024-04-04 16:33+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: utf-8\n"
 "Generated-By: pygettext.py 1.5\n"
 
+msgid "\tNew instance of :py:class:`%s`."
+msgstr "\tNouvelle instance de :py:class:`%s`."
+
 msgid " and "
 msgstr " et "
 
 msgid " between "
 msgstr " compris entre "
 
 msgid " higher than "
@@ -174,14 +177,17 @@
 
 msgid "Data"
 msgstr "Données"
 
 msgid "DataFrame"
 msgstr "DataFrame"
 
+msgid "Default: %s."
+msgstr "Par défaut : %s."
+
 msgid "Definition:"
 msgstr "Définition :"
 
 msgid "Delete"
 msgstr "Supprimer"
 
 msgid "Delete from column"
@@ -228,14 +234,17 @@
 
 msgid "Error"
 msgstr "Erreur"
 
 msgid "External editor:"
 msgstr "Éditeur externe :"
 
+msgid "Failed to import class %s"
+msgstr "Impossible d'importer la classe %s"
+
 msgid "Float formatting"
 msgstr "Format de flottant"
 
 msgid ""
 "For performance reasons, changes applied to masked array won't be reflected "
 "in array's data (and vice-versa)."
 msgstr ""
@@ -352,14 +361,17 @@
 
 msgid "Masked data"
 msgstr "Données masquées"
 
 msgid "More details about %s on %s or %s"
 msgstr "Plus de détails à propos de %s sur %s ou %s"
 
+msgid "Multiple choice from: %s."
+msgstr "Sélection multiple parmi : %s."
+
 msgid "Name"
 msgstr "Nom"
 
 msgid "New variable name:"
 msgstr "Nouveau nom de variable :"
 
 msgid "Next"
@@ -456,14 +468,21 @@
 
 msgid "Resize"
 msgstr "Ajuster"
 
 msgid "Resize rows to contents"
 msgstr "Ajuster les colonnes au contenu"
 
+msgid ""
+"Returns a new instance of :py:class:`%s` with the fields set to the given "
+"values."
+msgstr ""
+"Renvoie une nouvelle instance de :py:class:`%s` avec les champs initialisés "
+"aux valeurs données."
+
 msgid "Row separator:"
 msgstr "Séparateur de ligne :"
 
 msgid "Row(s) deletion"
 msgstr "Suppression de ligne(s)"
 
 msgid "Row(s) insertion"
@@ -503,14 +522,17 @@
 
 msgid "Show image"
 msgstr "Afficher l'image"
 
 msgid "Side areas:"
 msgstr "Zone latérale :"
 
+msgid "Single choice from: %s."
+msgstr "Sélection unique parmi : %s."
+
 msgid "Size"
 msgstr "Taille"
 
 msgid "Skip rows:"
 msgstr "Sauter des lignes :"
 
 msgid ""
@@ -560,14 +582,21 @@
 
 msgid "To complex"
 msgstr "Vers complexe"
 
 msgid "To float"
 msgstr "Vers flottant"
 
+msgid ""
+"To instanciate a new :py:class:`%s` dataset, you can use the classmethod :py:"
+"meth:`%s.create()` like this:"
+msgstr ""
+"Pour instancier un nouveau jeu de données :py:class:`%s`, vous pouvez "
+"utiliser la méthode de classe :py:class:`%s.create()` comme ceci :"
+
 msgid "To int"
 msgstr "Vers entier"
 
 msgid "To str"
 msgstr "Vers chaîne"
 
 msgid "Transpose"
@@ -612,14 +641,21 @@
 
 msgid "Warning"
 msgstr "Avertissement"
 
 msgid "Whitespace"
 msgstr "Espace"
 
+msgid ""
+"You can also first instanciate a default :py:class:`%s` and then set the "
+"fields like this:"
+msgstr ""
+"Vous pouvez également instancier un :py:class:`%s` par défaut puis "
+"initialiser les champs comme ceci :"
+
 msgid "You will not be able to add or remove rows/columns."
 msgstr "Vous ne pourrez pas insérer ou supprimer de lignes/colonnes"
 
 msgid "all file types"
 msgstr "tout type de fichier"
 
 msgid "array"
```

### Comparing `guidata-3.4.1/guidata/qthelpers.py` & `guidata-3.5.0/guidata/qthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/__init__.py` & `guidata-3.5.0/guidata/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/data/genreqs/pyproject.toml` & `guidata-3.5.0/guidata/tests/data/genreqs/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 [project.urls]
 Homepage = "https://github.com/PlotPyStack/guidata/"
 Documentation = "https://guidata.readthedocs.io/en/latest/"
 
 [project.scripts]
 
 [project.optional-dependencies]
-dev = ["black", "isort", "pylint", "Coverage"]
+dev = ["ruff", "pylint", "Coverage"]
 doc = [
     "PyQt5",
     "pillow",
     "pandas",
     "sphinx",
     "sphinx-copybutton",
     "sphinx_qt_documentation",
```

### Comparing `guidata-3.4.1/guidata/tests/data/genreqs/setup.cfg` & `guidata-3.5.0/guidata/tests/data/genreqs/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -71,23 +71,22 @@
 00000460: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
 00000470: 6174 6120 3d20 5472 7565 0d0a 0d0a 5b6f  ata = True....[o
 00000480: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
 00000490: 6669 6e64 5d0d 0a69 6e63 6c75 6465 203d  find]..include =
 000004a0: 2067 7569 6461 7461 2a0d 0a0d 0a5b 6f70   guidata*....[op
 000004b0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
 000004c0: 7569 7265 5d0d 0a64 6576 203d 0d0a 2020  uire]..dev =..  
-000004d0: 2020 626c 6163 6b0d 0a20 2020 2069 736f    black..    iso
-000004e0: 7274 0d0a 2020 2020 7079 6c69 6e74 0d0a  rt..    pylint..
-000004f0: 2020 2020 436f 7665 7261 6765 0d0a 646f      Coverage..do
-00000500: 6320 3d0d 0a20 2020 2050 7951 7435 0d0a  c =..    PyQt5..
-00000510: 2020 2020 7069 6c6c 6f77 0d0a 2020 2020      pillow..    
-00000520: 7061 6e64 6173 0d0a 2020 2020 7370 6869  pandas..    sphi
-00000530: 6e78 0d0a 2020 2020 7370 6869 6e78 2d63  nx..    sphinx-c
-00000540: 6f70 7962 7574 746f 6e0d 0a20 2020 2073  opybutton..    s
-00000550: 7068 696e 785f 7174 5f64 6f63 756d 656e  phinx_qt_documen
-00000560: 7461 7469 6f6e 0d0a 2020 2020 7079 7468  tation..    pyth
-00000570: 6f6e 2d64 6f63 732d 7468 656d 650d 0a74  on-docs-theme..t
-00000580: 6573 7420 3d0d 0a20 2020 2070 7974 6573  est =..    pytes
-00000590: 740d 0a20 2020 2070 7974 6573 742d 636f  t..    pytest-co
-000005a0: 760d 0a20 2020 2070 7974 6573 742d 7174  v..    pytest-qt
-000005b0: 0d0a 2020 2020 7079 7465 7374 2d78 7666  ..    pytest-xvf
-000005c0: 620d 0a                                  b..
+000004d0: 2020 7275 6666 0d0a 2020 2020 7079 6c69    ruff..    pyli
+000004e0: 6e74 0d0a 2020 2020 436f 7665 7261 6765  nt..    Coverage
+000004f0: 0d0a 646f 6320 3d0d 0a20 2020 2050 7951  ..doc =..    PyQ
+00000500: 7435 0d0a 2020 2020 7069 6c6c 6f77 0d0a  t5..    pillow..
+00000510: 2020 2020 7061 6e64 6173 0d0a 2020 2020      pandas..    
+00000520: 7370 6869 6e78 0d0a 2020 2020 7370 6869  sphinx..    sphi
+00000530: 6e78 2d63 6f70 7962 7574 746f 6e0d 0a20  nx-copybutton.. 
+00000540: 2020 2073 7068 696e 785f 7174 5f64 6f63     sphinx_qt_doc
+00000550: 756d 656e 7461 7469 6f6e 0d0a 2020 2020  umentation..    
+00000560: 7079 7468 6f6e 2d64 6f63 732d 7468 656d  python-docs-them
+00000570: 650d 0a74 6573 7420 3d0d 0a20 2020 2070  e..test =..    p
+00000580: 7974 6573 740d 0a20 2020 2070 7974 6573  ytest..    pytes
+00000590: 742d 636f 760d 0a20 2020 2070 7974 6573  t-cov..    pytes
+000005a0: 742d 7174 0d0a 2020 2020 7079 7465 7374  t-qt..    pytest
+000005b0: 2d78 7666 620d 0a                        -xvfb..
```

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_activable_dataset.py` & `guidata-3.5.0/guidata/tests/dataset/test_activable_dataset.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_activable_items.py` & `guidata-3.5.0/guidata/tests/dataset/test_activable_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_all_features.py` & `guidata-3.5.0/guidata/tests/dataset/test_all_features.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_all_items.py` & `guidata-3.5.0/guidata/tests/dataset/test_all_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_all_items_readonly.py` & `guidata-3.5.0/guidata/tests/dataset/test_all_items_readonly.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_bool_selector.py` & `guidata-3.5.0/guidata/tests/dataset/test_bool_selector.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_callbacks.py` & `guidata-3.5.0/guidata/tests/dataset/test_callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
     string = gds.StringItem("String", default="foobar").set_prop(
         "display", callback=cb_example
     )
     x1 = gds.FloatItem("x1").set_prop("display", callback=update_x1plusx2)
     x2 = gds.FloatItem("x2").set_prop("display", callback=update_x1plusx2)
     x1plusx2 = gds.FloatItem("x1+x2").set_prop("display", active=False)
+    boolean = gds.BoolItem("Boolean", default=True).set_prop(
+        "display", callback=cb_example
+    )
     color = gds.ColorItem("Color", default="red").set_prop(
         "display", callback=cb_example
     )
 
     def choices_callback(self, item, value):
         """Choices callback: this demonstrates how to dynamically change
         the list of choices... even if it is not very useful in this case
@@ -62,15 +65,15 @@
             "Single choice",
             choices_callback,
             default=64,
         )
         .set_pos(col=1, colspan=2)
         .set_prop("display", callback=cb_example)
     )
-    results = gds.TextItem("Results")
+    results = gds.TextItem("Results").set_prop("display", callback=cb_example)
 
 
 def test_callbacks():
     """Test callbacks"""
     with qt_app_context():
         prm = Parameters()
         execenv.print(prm)
```

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_datasetgroup.py` & `guidata-3.5.0/guidata/tests/dataset/test_datasetgroup.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_editgroupbox.py` & `guidata-3.5.0/guidata/tests/dataset/test_editgroupbox.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_inheritance.py` & `guidata-3.5.0/guidata/tests/dataset/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_item_order.py` & `guidata-3.5.0/guidata/tests/dataset/test_item_order.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_loadsave_hdf5.py` & `guidata-3.5.0/guidata/tests/dataset/test_loadsave_hdf5.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_loadsave_json.py` & `guidata-3.5.0/guidata/tests/dataset/test_loadsave_json.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/dataset/test_rotatedlabel.py` & `guidata-3.5.0/guidata/tests/dataset/test_rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/unit/test_config.py` & `guidata-3.5.0/guidata/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/unit/test_data.py` & `guidata-3.5.0/guidata/tests/unit/test_data.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/unit/test_dataset_from_dict.py` & `guidata-3.5.0/guidata/tests/unit/test_dataset_from_dict.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/unit/test_dataset_from_func.py` & `guidata-3.5.0/guidata/tests/unit/test_dataset_from_func.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/unit/test_genreqs.py` & `guidata-3.5.0/guidata/tests/unit/test_genreqs.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/unit/test_h5fmt.py` & `guidata-3.5.0/guidata/tests/unit/test_h5fmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         self.param1 = MyFirstDataSetV11()
         self.param2 = MySecondDataSetV11()
 
 
 def test_hdf5_datamodel_compatiblity():
     """Test HDF5 I/O with data model compatibility"""
     path = osp.abspath("test.h5")
-    atexit.register(lambda: os.unlink(path))
+    atexit.register(os.unlink, path)
     # Serialize the first version of the data model
     model_v10 = MyDataModelV10()
     model_v10.save(path)
     # Deserialize the first version of the data model
     model_v10.load(path)
     # Deserialize using the new version of the data model
     model_v11 = MyDataModelV11()
```

### Comparing `guidata-3.4.1/guidata/tests/unit/test_jsonfmt.py` & `guidata-3.5.0/guidata/tests/unit/test_jsonfmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 Testing various use cases of JSON I/O:
 
 * Serialize and deserialize a data model, handling versioning and compatibility breaks.
 """
 
 from __future__ import annotations
 
+import atexit
+import os
 import os.path as osp
 
 from guidata.env import execenv
 from guidata.io import JSONReader, JSONWriter
 
 
 # The following class represents a data model that we want to serialize and deserialize.
@@ -111,14 +113,15 @@
         self.obj1 = MyDataObjectV11("first_obj_title")
         self.obj2 = MyDataObjectV11("second_obj_title")
 
 
 def test_json_datamodel_compatiblity():
     """Test JSON I/O with data model compatibility"""
     path = osp.abspath("test.json")
+    atexit.register(os.unlink, path)
     # atexit.register(lambda: os.unlink(path))
     # Serialize the first version of the data model
     model_v10 = MyDataModelV10()
     model_v10.save(path)
     # Deserialize the first version of the data model
     model_v10.load(path)
     # Deserialize using the new version of the data model
```

### Comparing `guidata-3.4.1/guidata/tests/unit/test_no_qt.py` & `guidata-3.5.0/guidata/tests/unit/test_no_qt.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/unit/test_text.py` & `guidata-3.5.0/guidata/tests/unit/test_text.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/unit/test_updaterestoredataset.py` & `guidata-3.5.0/guidata/tests/unit/test_updaterestoredataset.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/unit/test_userconfig_app.py` & `guidata-3.5.0/guidata/tests/unit/test_userconfig_app.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/widgets/test_arrayeditor.py` & `guidata-3.5.0/guidata/tests/widgets/test_arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/widgets/test_arrayeditor_unit.py` & `guidata-3.5.0/guidata/tests/widgets/test_arrayeditor_unit.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/widgets/test_codeeditor.py` & `guidata-3.5.0/guidata/tests/widgets/test_codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/widgets/test_collectionseditor.py` & `guidata-3.5.0/guidata/tests/widgets/test_collectionseditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/widgets/test_console.py` & `guidata-3.5.0/guidata/tests/widgets/test_console.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/widgets/test_dataframeeditor.py` & `guidata-3.5.0/guidata/tests/widgets/test_dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/widgets/test_importwizard.py` & `guidata-3.5.0/guidata/tests/widgets/test_importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/tests/widgets/test_objecteditor.py` & `guidata-3.5.0/guidata/tests/widgets/test_objecteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/userconfig.py` & `guidata-3.5.0/guidata/userconfig.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/utils/encoding.py` & `guidata-3.5.0/guidata/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/utils/genreqs.py` & `guidata-3.5.0/guidata/utils/genreqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,16 @@
 
     Args:
         package (str): Package name
 
     Returns:
         str: Package summary or empty string if package not found on PyPI
     """
+    if package == "Python":
+        return "Python programming language"
     try:
         response = requests.get(f"https://pypi.org/pypi/{package}/json")
     except requests.exceptions.ConnectionError:
         return ""
     if response.status_code != 200:
         return ""
     return response.json()["info"]["summary"]
@@ -128,15 +130,15 @@
         "    * - Name",
         "      - Version",
         "      - Summary",
     ]
     modlist = []
     for req in reqs:
         try:
-            mod = re.split("(>=|<=|=|<|>)", req)[0]
+            mod = re.split(" ?(>=|<=|=|<|>)", req)[0]
             ver = req[len(mod) :]
         except ValueError:
             mod, ver = req, ""
         if mod.lower() in modlist:
             continue
         modlist.append(mod.lower())
         requirements.append("    * - " + mod)
```

### Comparing `guidata-3.4.1/guidata/utils/gettext_helpers.py` & `guidata-3.5.0/guidata/utils/gettext_helpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/utils/misc.py` & `guidata-3.5.0/guidata/utils/misc.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/__init__.py` & `guidata-3.5.0/guidata/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/about.py` & `guidata-3.5.0/guidata/widgets/about.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/arrayeditor/__init__.py` & `guidata-3.5.0/guidata/widgets/arrayeditor/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/arrayeditor/arrayeditor.py` & `guidata-3.5.0/guidata/widgets/arrayeditor/arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/arrayeditor/arrayhandler.py` & `guidata-3.5.0/guidata/widgets/arrayeditor/arrayhandler.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/arrayeditor/datamodel.py` & `guidata-3.5.0/guidata/widgets/arrayeditor/datamodel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/arrayeditor/editorwidget.py` & `guidata-3.5.0/guidata/widgets/arrayeditor/editorwidget.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/arrayeditor/utils.py` & `guidata-3.5.0/guidata/widgets/arrayeditor/utils.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/codeeditor.py` & `guidata-3.5.0/guidata/widgets/codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/collectionseditor.py` & `guidata-3.5.0/guidata/widgets/collectionseditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/console/__init__.py` & `guidata-3.5.0/guidata/widgets/console/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/console/base.py` & `guidata-3.5.0/guidata/widgets/console/base.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/console/calltip.py` & `guidata-3.5.0/guidata/widgets/console/calltip.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/console/dochelpers.py` & `guidata-3.5.0/guidata/widgets/console/dochelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/console/internalshell.py` & `guidata-3.5.0/guidata/widgets/console/internalshell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/console/interpreter.py` & `guidata-3.5.0/guidata/widgets/console/interpreter.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/console/mixins.py` & `guidata-3.5.0/guidata/widgets/console/mixins.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/console/shell.py` & `guidata-3.5.0/guidata/widgets/console/shell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/console/terminal.py` & `guidata-3.5.0/guidata/widgets/console/terminal.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/dataframeeditor.py` & `guidata-3.5.0/guidata/widgets/dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/dockable.py` & `guidata-3.5.0/guidata/widgets/dockable.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/importwizard.py` & `guidata-3.5.0/guidata/widgets/importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/nsview.py` & `guidata-3.5.0/guidata/widgets/nsview.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/objecteditor.py` & `guidata-3.5.0/guidata/widgets/objecteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/rotatedlabel.py` & `guidata-3.5.0/guidata/widgets/rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/syntaxhighlighters.py` & `guidata-3.5.0/guidata/widgets/syntaxhighlighters.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata/widgets/texteditor.py` & `guidata-3.5.0/guidata/widgets/texteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.4.1/guidata.egg-info/PKG-INFO` & `guidata-3.5.0/guidata.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guidata
-Version: 3.4.1
+Version: 3.5.0
 Summary: Automatic GUI generation for easy dataset editing and display
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
         
@@ -31,41 +31,46 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/PlotPyStack/guidata/
 Project-URL: Documentation, https://guidata.readthedocs.io/en/latest/
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Software Development :: User Interfaces
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows 7
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Software Development :: Widget Sets
+Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py>=3.0
 Requires-Dist: NumPy>=1.21
 Requires-Dist: QtPy>=1.9
 Requires-Dist: requests
 Requires-Dist: tomli
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: Coverage; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: PyQt5; extra == "doc"
 Requires-Dist: pillow; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
 Requires-Dist: sphinx>6; extra == "doc"
```

### Comparing `guidata-3.4.1/guidata.egg-info/SOURCES.txt` & `guidata-3.5.0/guidata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+conftest.py
 guidata-tests.desktop
 pyproject.toml
+requirements.txt
 doc/basic_example.py
 doc/changelog.rst
 doc/conf.py
 doc/examples.rst
 doc/index.rst
 doc/installation.rst
 doc/overview.rst
 doc/requirements.rst
 doc/update_requirements.py
 doc/widgets.rst
 doc/_static/favicon.ico
+doc/autodoc/autodoc_example.py
+doc/autodoc/index.rst
 doc/dev/contribute.rst
 doc/dev/howto.rst
 doc/dev/index.rst
 doc/dev/platform.rst
 doc/dev/v2_to_v3.csv
 doc/dev/v2_to_v3.rst
 doc/images/basic_example.png
@@ -58,18 +63,21 @@
 guidata.egg-info/PKG-INFO
 guidata.egg-info/SOURCES.txt
 guidata.egg-info/dependency_links.txt
 guidata.egg-info/entry_points.txt
 guidata.egg-info/requires.txt
 guidata.egg-info/top_level.txt
 guidata/dataset/__init__.py
+guidata/dataset/autodoc.py
+guidata/dataset/autodoc_method.py
 guidata/dataset/conv.py
 guidata/dataset/dataitems.py
 guidata/dataset/datatypes.py
 guidata/dataset/io.py
+guidata/dataset/note_directive.py
 guidata/dataset/qtitemwidgets.py
 guidata/dataset/qtwidgets.py
 guidata/dataset/textedit.py
 guidata/external/__init__.py
 guidata/external/darkdetect/__init__.py
 guidata/external/darkdetect/_dummy.py
 guidata/external/darkdetect/_linux_detect.py
@@ -141,15 +149,14 @@
 guidata/io/__init__.py
 guidata/io/base.py
 guidata/io/h5fmt.py
 guidata/io/inifmt.py
 guidata/io/jsonfmt.py
 guidata/locale/fr/LC_MESSAGES/guidata.mo
 guidata/tests/__init__.py
-guidata/tests/conftest.py
 guidata/tests/data/genreqs/pyproject.toml
 guidata/tests/data/genreqs/setup.cfg
 guidata/tests/dataset/__init__.py
 guidata/tests/dataset/test_activable_dataset.py
 guidata/tests/dataset/test_activable_items.py
 guidata/tests/dataset/test_all_features.py
 guidata/tests/dataset/test_all_items.py
```

