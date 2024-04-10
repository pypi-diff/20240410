# Comparing `tmp/DLMS_SPODES_client-0.7.2.tar.gz` & `tmp/DLMS_SPODES_client-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.7.2.tar", last modified: Mon Apr  8 13:08:37 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.7.3.tar", last modified: Tue Apr  9 13:20:02 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.7.2.tar` & `DLMS_SPODES_client-0.7.3.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.610556 DLMS_SPODES_client-0.7.2/
--rw-rw-rw-   0        0        0      526 2024-04-08 13:08:37.609585 DLMS_SPODES_client-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.2/README.md
--rw-rw-rw-   0        0        0      836 2024-04-08 13:05:41.000000 DLMS_SPODES_client-0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 13:08:37.610556 DLMS_SPODES_client-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.461585 DLMS_SPODES_client-0.7.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.478553 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   122792 2024-04-08 06:55:11.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/client.py
--rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.415332 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.497553 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.546552 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      294 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/ConnectionState.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0    10908 2024-01-22 08:39:08.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3438 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.602556 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.604554 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     5634 2024-04-05 09:00:03.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0    35025 2024-04-05 11:00:00.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.492569 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-08 13:08:37.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3206 2024-04-08 13:08:37.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 13:08:37.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-08 13:08:37.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-08 13:08:37.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-08 13:08:37.000000 DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:08:37.607556 DLMS_SPODES_client-0.7.2/test/
--rw-rw-rw-   0        0        0     7036 2024-04-08 07:21:09.000000 DLMS_SPODES_client-0.7.2/test/test_Client.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:02.011498 DLMS_SPODES_client-0.7.3/
+-rw-rw-rw-   0        0        0      526 2024-04-09 13:20:02.010496 DLMS_SPODES_client-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.3/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-09 13:18:34.000000 DLMS_SPODES_client-0.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 13:20:02.011498 DLMS_SPODES_client-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:01.851514 DLMS_SPODES_client-0.7.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:01.868494 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   122734 2024-04-09 11:08:43.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/client.py
+-rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:01.805526 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:01.888495 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:01.942500 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      294 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/ConnectionState.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0    10908 2024-01-22 08:39:08.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3438 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:02.001496 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:02.003497 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     5634 2024-04-05 09:00:03.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0     3150 2024-04-09 07:47:34.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/services.py
+-rw-rw-rw-   0        0        0    34836 2024-04-09 12:26:31.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:01.883496 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-09 13:20:01.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3263 2024-04-09 13:20:01.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 13:20:01.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-09 13:20:01.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-09 13:20:01.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-09 13:20:01.000000 DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:20:02.008498 DLMS_SPODES_client-0.7.3/test/
+-rw-rw-rw-   0        0        0     7036 2024-04-08 07:21:09.000000 DLMS_SPODES_client-0.7.3/test/test_Client.py
+-rw-rw-rw-   0        0        0      251 2024-04-09 08:34:38.000000 DLMS_SPODES_client-0.7.3/test/test_services.py
```

### Comparing `DLMS_SPODES_client-0.7.2/PKG-INFO` & `DLMS_SPODES_client-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.7.2
+Version: 0.7.3
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.2/pyproject.toml` & `DLMS_SPODES_client-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
     "DLMS-SPODES == 0.69.4",
     "DLMS-SPODES-communications >= 1.2.3",
     "pycryptodomex>=3.15"
```

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,17 +196,14 @@
         self.current_obj = None
         """ current transferring object. For progress bar now """
 
         # from Gurux Client
         self.use_protected_release = False
         """  Gurux Client: If protected release is used release is including a ciphered xDLMS Initiate request. """
 
-        self.locker_name = ""
-        """name of locker"""
-
     def log(self, level: logL, msg: str):
         """use logger with level and extra=LDN"""
         if not self.logging_disable:
             logger.log(level=level,
                        msg=msg,
                        extra={"id": self.objects.LDN.value.to_str() if (self.objects and self.objects.LDN.value) else F"#{self.__id}"})
 
@@ -2114,15 +2111,15 @@
                 break
             else:
                 control = frame.Control(self.settings.getNextSend(False))
         self.send_frames.extend(new_frames)
 
     def __str__(self):
         if not self.objects or not self.objects.LDN.value:
-            return self.__id
+            return str(self.__id)
         else:
             return self.objects.LDN.value.to_str()
 
     def get_serial_number(self) -> str:
         """ return serial number as text. If serial object is absence return 'недоступен' """
         if self.objects is None:
             return "нет типа"
```

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/logger.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/logger.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/servers.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/servers.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client/task.py` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,17 @@
             # dev.write_attr(obj, 2)
             # logger.info(F'Write attribute: 2 success')
             c.errors[Transmit.OK] = 'Запись времени'
         except Exception as e:
             # logger.info(F'ERROR: write Clock: attribute 2 {e}')
             c.errors[Transmit.WRITE_ERROR] = F"write time: {e}"
 
+# @dataclass
+# class UpdateResponse:
+#     result:
 
 @dataclass
 class UpdateFirmware(ExTask):
     """only for KPZ now"""
     # firmwares: field(default=dict)
 
     async def exchange(self, c: Client) -> bool:
@@ -476,27 +479,21 @@
                     c.log(logL.INFO, F"start block: {obj.current_block_transfer} transferred")
                     try:
                         obj.set_next_block()
                     except StopIteration:
                         c.log(logL.INFO, "All blocks transferred")
                         break
                 # c.execute_method(obj.get_meth_descriptor(3))  # Start Verify Transfer. todo: removed Verification because don't work with change to 1.3
-                is_activating = True
                 await c.execute_method(obj.get_meth_descriptor(4))
                 c.log(logL.INFO, "Start Activate Transfer")
-                is_activating = False
                 c.set_error(Application.OK, F'Activated')
                 return True
             except Exception as e:
                 c.set_error(Transmit.EXECUTE_ERROR, F'unhandled update error. {e.args[0]}')
                 return False
-            finally:
-                if is_activating:
-                    c.set_error(Transmit.EXECUTE_ERROR, 'Activating')
-                c.current_obj = None
         else:
             return True
 
     async def __is_updated_image_2(self, c: Client, obj: collection.ImageTransfer, with_abort: bool = True) -> bool:
         """ update image if blocks is fulls ver 2"""
         if obj.is_image_exist:
             is_activating: bool = False
```

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.7.2
+Version: 0.7.3
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.2/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.7.3/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/__init__.py
 src/DLMS_SPODES_client/FCS16.py
 src/DLMS_SPODES_client/__init__.py
 src/DLMS_SPODES_client/client.py
 src/DLMS_SPODES_client/enums.py
 src/DLMS_SPODES_client/logger.py
 src/DLMS_SPODES_client/servers.py
+src/DLMS_SPODES_client/services.py
 src/DLMS_SPODES_client/task.py
 src/DLMS_SPODES_client.egg-info/PKG-INFO
 src/DLMS_SPODES_client.egg-info/SOURCES.txt
 src/DLMS_SPODES_client.egg-info/dependency_links.txt
 src/DLMS_SPODES_client.egg-info/entry_points.txt
 src/DLMS_SPODES_client.egg-info/requires.txt
 src/DLMS_SPODES_client.egg-info/top_level.txt
@@ -60,8 +61,9 @@
 src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
 src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
 src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
 src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
 src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
 src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
 src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
-test/test_Client.py
+test/test_Client.py
+test/test_services.py
```

### Comparing `DLMS_SPODES_client-0.7.2/test/test_Client.py` & `DLMS_SPODES_client-0.7.3/test/test_Client.py`

 * *Files identical despite different names*

