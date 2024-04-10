# Comparing `tmp/gallia-1.6.0.tar.gz` & `tmp/gallia-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gallia-1.6.0.tar", max compression
+gzip compressed data, was "gallia-1.7.0.tar", max compression
```

## Comparing `gallia-1.6.0.tar` & `gallia-1.7.0.tar`

### file list

```diff
@@ -1,90 +1,93 @@
--rw-r--r--   0        0        0    10280 2024-02-23 10:52:55.788652 gallia-1.6.0/LICENSE
-drwxr-xr-x   0        0        0        0 2024-02-23 10:52:55.788652 gallia-1.6.0/LICENSES/
--rw-r--r--   0        0        0     2995 2024-02-23 10:52:55.788652 gallia-1.6.0/README.md
--rw-r--r--   0        0        0     2752 2024-02-23 10:52:55.788652 gallia-1.6.0/pyproject.toml
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.788652 gallia-1.6.0/src/cursed_hr/__init__.py
--rw-r--r--   0        0        0    54826 2024-02-23 10:52:55.788652 gallia-1.6.0/src/cursed_hr/cursed_hr.py
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.788652 gallia-1.6.0/src/gallia/__init__.py
--rw-r--r--   0        0        0    11585 2024-02-23 10:52:55.788652 gallia-1.6.0/src/gallia/cli.py
--rw-r--r--   0        0        0      353 2024-02-23 10:52:55.788652 gallia-1.6.0/src/gallia/command/__init__.py
--rw-r--r--   0        0        0    20676 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/command/base.py
--rw-r--r--   0        0        0     8403 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/command/uds.py
--rw-r--r--   0        0        0     2222 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/__init__.py
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/discover/__init__.py
--rw-r--r--   0        0        0    21189 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/discover/doip.py
--rw-r--r--   0        0        0     9830 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/discover/find_xcp.py
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/discover/uds/__init__.py
--rw-r--r--   0        0        0     9470 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/discover/uds/isotp.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/fuzz/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/fuzz/uds/__init__.py
--rw-r--r--   0        0        0     7523 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/fuzz/uds/pdu.py
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/generic/__init__.py
--rw-r--r--   0        0        0      686 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/generic/pdu.py
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/__init__.py
--rw-r--r--   0        0        0     8302 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/dtc.py
--rw-r--r--   0        0        0     1998 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/ecu_reset.py
--rw-r--r--   0        0        0     4285 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/iocbi.py
--rw-r--r--   0        0        0     2366 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/pdu.py
--rw-r--r--   0        0        0     1734 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/ping.py
--rw-r--r--   0        0        0     1586 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/rdbi.py
--rw-r--r--   0        0        0     1748 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/rmba.py
--rw-r--r--   0        0        0     5449 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/rtcl.py
--rw-r--r--   0        0        0      777 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/vin.py
--rw-r--r--   0        0        0     2232 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/wdbi.py
--rw-r--r--   0        0        0     2080 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/wmba.py
--rw-r--r--   0        0        0     1886 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/primitive/uds/xcp.py
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/scan/__init__.py
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/scan/uds/__init__.py
--rw-r--r--   0        0        0     8796 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/scan/uds/identifiers.py
--rw-r--r--   0        0        0     4250 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/scan/uds/memory.py
--rw-r--r--   0        0        0     6907 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/scan/uds/reset.py
--rw-r--r--   0        0        0     7766 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/scan/uds/sa_dump_seeds.py
--rw-r--r--   0        0        0     6612 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/scan/uds/services.py
--rw-r--r--   0        0        0    10873 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/scan/uds/sessions.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/script/__init__.py
--rw-r--r--   0        0        0     3767 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/commands/script/vecu.py
--rw-r--r--   0        0        0     2062 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/config.py
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/db/__init__.py
--rw-r--r--   0        0        0    16637 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/db/handler.py
--rw-r--r--   0        0        0      232 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/db/log.py
--rw-r--r--   0        0        0     6415 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/dumpcap.py
--rw-r--r--   0        0        0    26654 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/log.py
--rw-r--r--   0        0        0     4761 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/plugins.py
--rw-r--r--   0        0        0     2782 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/powersupply.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/py.typed
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/__init__.py
--rw-r--r--   0        0        0      702 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/__init__.py
--rw-r--r--   0        0        0       88 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/core/__init__.py
--rw-r--r--   0        0        0    48477 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/core/client.py
--rw-r--r--   0        0        0     8181 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/core/constants.py
--rw-r--r--   0        0        0    13673 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/core/exception.py
--rw-r--r--   0        0        0   111398 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/core/service.py
--rw-r--r--   0        0        0     7754 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/core/utils.py
--rw-r--r--   0        0        0    18714 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/ecu.py
--rw-r--r--   0        0        0     3531 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/helpers.py
--rw-r--r--   0        0        0     5112 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/nrv.py
--rw-r--r--   0        0        0    32114 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/uds/server.py
--rw-r--r--   0        0        0     3746 2024-02-23 10:52:55.792652 gallia-1.6.0/src/gallia/services/xcp/__init__.py
--rw-r--r--   0        0        0    22613 2024-02-23 10:52:55.796652 gallia-1.6.0/src/gallia/services/xcp/types.py
--rw-r--r--   0        0        0      832 2024-02-23 10:52:55.796652 gallia-1.6.0/src/gallia/transports/__init__.py
--rw-r--r--   0        0        0     8091 2024-02-23 10:52:55.796652 gallia-1.6.0/src/gallia/transports/base.py
--rw-r--r--   0        0        0     7571 2024-02-23 10:52:55.796652 gallia-1.6.0/src/gallia/transports/can.py
--rw-r--r--   0        0        0    21151 2024-02-23 10:52:55.796652 gallia-1.6.0/src/gallia/transports/doip.py
--rw-r--r--   0        0        0     6023 2024-02-23 10:52:55.796652 gallia-1.6.0/src/gallia/transports/isotp.py
--rw-r--r--   0        0        0     2118 2024-02-23 10:52:55.796652 gallia-1.6.0/src/gallia/transports/tcp.py
--rw-r--r--   0        0        0     2027 2024-02-23 10:52:55.796652 gallia-1.6.0/src/gallia/transports/unix.py
--rw-r--r--   0        0        0     7247 2024-02-23 10:52:55.796652 gallia-1.6.0/src/gallia/utils.py
--rw-r--r--   0        0        0     2617 2024-02-23 10:52:55.796652 gallia-1.6.0/src/hr/__init__.py
--rw-r--r--   0        0        0      306 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/__init__.py
--rw-r--r--   0        0        0     3327 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/cli.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/devices/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/devices/http/__init__.py
--rw-r--r--   0        0        0     3621 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/devices/http/client.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/devices/rnd/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/devices/rs/__init__.py
--rw-r--r--   0        0        0     4297 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/devices/rs/hmc804.py
--rw-r--r--   0        0        0      144 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/exceptions.py
--rw-r--r--   0        0        0     3099 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/netzteil.py
--rw-r--r--   0        0        0        0 2024-02-23 10:52:55.796652 gallia-1.6.0/src/opennetzteil/py.typed
--rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 gallia-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10280 2024-04-10 14:27:43.138481 gallia-1.7.0/LICENSE
+drwxr-xr-x   0        0        0        0 2024-04-10 14:27:43.138481 gallia-1.7.0/LICENSES/
+-rw-r--r--   0        0        0    10280 2024-04-10 14:27:43.138481 gallia-1.7.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0     7048 2024-04-10 14:27:43.138481 gallia-1.7.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    42098 2024-04-10 14:27:43.138481 gallia-1.7.0/LICENSES/LGPL-3.0-only.txt
+-rw-r--r--   0        0        0     3110 2024-04-10 14:27:43.138481 gallia-1.7.0/README.md
+-rw-r--r--   0        0        0     2765 2024-04-10 14:27:43.138481 gallia-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/cursed_hr/__init__.py
+-rw-r--r--   0        0        0    54826 2024-04-10 14:27:43.142481 gallia-1.7.0/src/cursed_hr/cursed_hr.py
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/__init__.py
+-rw-r--r--   0        0        0    11585 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/cli.py
+-rw-r--r--   0        0        0      353 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/command/__init__.py
+-rw-r--r--   0        0        0    20604 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/command/base.py
+-rw-r--r--   0        0        0     8403 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/command/uds.py
+-rw-r--r--   0        0        0     2222 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/discover/__init__.py
+-rw-r--r--   0        0        0    23703 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/discover/doip.py
+-rw-r--r--   0        0        0     9803 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/discover/find_xcp.py
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/discover/uds/__init__.py
+-rw-r--r--   0        0        0     9454 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/discover/uds/isotp.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/fuzz/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/fuzz/uds/__init__.py
+-rw-r--r--   0        0        0     7537 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/fuzz/uds/pdu.py
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/generic/__init__.py
+-rw-r--r--   0        0        0      686 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/generic/pdu.py
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/__init__.py
+-rw-r--r--   0        0        0     8302 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/dtc.py
+-rw-r--r--   0        0        0     1990 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/ecu_reset.py
+-rw-r--r--   0        0        0     4285 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/iocbi.py
+-rw-r--r--   0        0        0     2366 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/pdu.py
+-rw-r--r--   0        0        0     1734 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/ping.py
+-rw-r--r--   0        0        0     1586 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/rdbi.py
+-rw-r--r--   0        0        0     1748 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/rmba.py
+-rw-r--r--   0        0        0     5449 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/rtcl.py
+-rw-r--r--   0        0        0      777 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/vin.py
+-rw-r--r--   0        0        0     2232 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/wdbi.py
+-rw-r--r--   0        0        0     2080 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/wmba.py
+-rw-r--r--   0        0        0     1886 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/primitive/uds/xcp.py
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/scan/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/scan/uds/__init__.py
+-rw-r--r--   0        0        0     8803 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/scan/uds/identifiers.py
+-rw-r--r--   0        0        0     4227 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/scan/uds/memory.py
+-rw-r--r--   0        0        0     6928 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/scan/uds/reset.py
+-rw-r--r--   0        0        0     7761 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/scan/uds/sa_dump_seeds.py
+-rw-r--r--   0        0        0     6619 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/scan/uds/services.py
+-rw-r--r--   0        0        0    10857 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/scan/uds/sessions.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/script/__init__.py
+-rw-r--r--   0        0        0     3767 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/commands/script/vecu.py
+-rw-r--r--   0        0        0     2062 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/config.py
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/db/__init__.py
+-rw-r--r--   0        0        0    16637 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/db/handler.py
+-rw-r--r--   0        0        0      232 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/db/log.py
+-rw-r--r--   0        0        0     6415 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/dumpcap.py
+-rw-r--r--   0        0        0    26654 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/log.py
+-rw-r--r--   0        0        0     4761 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/plugins.py
+-rw-r--r--   0        0        0     2782 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/powersupply.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/py.typed
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/services/__init__.py
+-rw-r--r--   0        0        0      702 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/services/uds/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/services/uds/core/__init__.py
+-rw-r--r--   0        0        0    48245 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/services/uds/core/client.py
+-rw-r--r--   0        0        0     8181 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/services/uds/core/constants.py
+-rw-r--r--   0        0        0    13673 2024-04-10 14:27:43.142481 gallia-1.7.0/src/gallia/services/uds/core/exception.py
+-rw-r--r--   0        0        0   111398 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/services/uds/core/service.py
+-rw-r--r--   0        0        0     7754 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/services/uds/core/utils.py
+-rw-r--r--   0        0        0    18674 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/services/uds/ecu.py
+-rw-r--r--   0        0        0     3531 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/services/uds/helpers.py
+-rw-r--r--   0        0        0     5112 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/services/uds/nrv.py
+-rw-r--r--   0        0        0    32090 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/services/uds/server.py
+-rw-r--r--   0        0        0     3746 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/services/xcp/__init__.py
+-rw-r--r--   0        0        0    22613 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/services/xcp/types.py
+-rw-r--r--   0        0        0      832 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/transports/__init__.py
+-rw-r--r--   0        0        0     8091 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/transports/base.py
+-rw-r--r--   0        0        0     7563 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/transports/can.py
+-rw-r--r--   0        0        0    27169 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/transports/doip.py
+-rw-r--r--   0        0        0     6023 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/transports/isotp.py
+-rw-r--r--   0        0        0     2118 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/transports/tcp.py
+-rw-r--r--   0        0        0     2027 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/transports/unix.py
+-rw-r--r--   0        0        0     7247 2024-04-10 14:27:43.146481 gallia-1.7.0/src/gallia/utils.py
+-rw-r--r--   0        0        0     2617 2024-04-10 14:27:43.146481 gallia-1.7.0/src/hr/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/__init__.py
+-rw-r--r--   0        0        0     3327 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/cli.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/devices/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/devices/http/__init__.py
+-rw-r--r--   0        0        0     3621 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/devices/http/client.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/devices/rnd/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/devices/rs/__init__.py
+-rw-r--r--   0        0        0     4297 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/devices/rs/hmc804.py
+-rw-r--r--   0        0        0      144 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/exceptions.py
+-rw-r--r--   0        0        0     3091 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/netzteil.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:27:43.146481 gallia-1.7.0/src/opennetzteil/py.typed
+-rw-r--r--   0        0        0     4499 1970-01-01 00:00:00.000000 gallia-1.7.0/PKG-INFO
```

### Comparing `gallia-1.6.0/LICENSE` & `gallia-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/README.md` & `gallia-1.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Gallia
 
 [![docs](https://img.shields.io/badge/-docs-green)](https://fraunhofer-aisec.github.io/gallia)
 [![docs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://gallia.readthedocs.io/en/latest)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gallia)](https://pypi.python.org/pypi/gallia/)
 [![PyPI - License](https://img.shields.io/pypi/l/gallia)](https://www.apache.org/licenses/LICENSE-2.0.html)
 [![PyPI](https://img.shields.io/pypi/v/gallia)](https://pypi.python.org/pypi/gallia/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10696368.svg)](https://zenodo.org/doi/10.5281/zenodo.10696368)
 
 [![Packaging status](https://repology.org/badge/vertical-allrepos/gallia.svg)](https://repology.org/project/gallia/versions)
 
 Gallia is an extendable pentesting framework with the focus on the automotive domain.
 The scope of the toolchain is conducting penetration tests from a single ECU up to whole cars.
 Currently, the main focus lies on the [UDS](https://www.iso.org/standard/72439.html) interface.
 Acting as a generic interface, the logging functionality implements reproducible tests and enables post-processing tasks.
```

### Comparing `gallia-1.6.0/pyproject.toml` & `gallia-1.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "gallia"
-version = "1.6.0"
+version = "1.7.0"
 description = "Extendable Pentesting Framework"
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://fraunhofer-aisec.github.io/gallia"
 repository = "https://github.com/Fraunhofer-AISEC/gallia"
 authors = ["AISEC Pentesting Team"]
 maintainers = [
@@ -43,33 +43,33 @@
 construct = "^2.10"
 msgspec = ">=0.11,<0.19"
 pydantic = "^2.0"
 pygit2 = "^1.10"
 platformdirs = ">=2.6,<5.0"
 exitcode = "^0.1.0"
 psutil = "^5.9.4"
-httpx = {extras = ["http2"], version = "^0.26.0"}
+httpx = {extras = ["http2"], version = ">=0.26,<0.28"}
 
 [tool.poetry.group.dev.dependencies]
 Sphinx = ">=5.2,<8.0"
 mypy = "^1.0"
 pylsp-mypy = "^0.6"
 pylsp-rope = "^0.1"
-pytest = "^7.1"
-pytest-asyncio = ">=0.20,<0.22"
+pytest = ">=7.1,<9.0"
+pytest-asyncio = ">=0.20,<0.24"
 python-lsp-server = "^1.5"
 types-aiofiles = "^23.1"
 types-psutil = "^5.9.5.10"
 types-tabulate = "^0.9"
 myst-parser = ">=0.18,<2.1"
 sphinx-rtd-theme = ">=1,<3"
-reuse = ">=1,<3"
+reuse = ">=1,<4"
 construct-typing = ">=0.5.2,<0.7.0"
-pytest-cov = "^4.0"
-ruff = "^0.1.0"
+pytest-cov = ">=4,<6"
+ruff = "^0.3.0"
 python-lsp-ruff = ">=1.6,<3.0"
 
 [tool.poetry.scripts]
 "gallia" = "gallia.cli:main"
 "netzteil" = "opennetzteil.cli:main"
 "cursed-hr" = "cursed_hr.cursed_hr:main"
 "hr" = "hr:main"
```

### Comparing `gallia-1.6.0/src/cursed_hr/cursed_hr.py` & `gallia-1.7.0/src/cursed_hr/cursed_hr.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/cli.py` & `gallia-1.7.0/src/gallia/cli.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/command/base.py` & `gallia-1.7.0/src/gallia/command/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,16 +126,15 @@
         self._lock_file_fd: int | None = None
         self.db_handler: DBHandler | None = None
         self.configure_class_parser()
         self.configure_parser()
         self.log_file_handlers = []
 
     @abstractmethod
-    def run(self, args: Namespace) -> int:
-        ...
+    def run(self, args: Namespace) -> int: ...
 
     def run_hook(
         self,
         variant: HookVariant,
         args: Namespace,
         exit_code: int | None = None,
     ) -> None:
@@ -255,16 +254,15 @@
                     Path(gettempdir()).joinpath("gallia"),
                 ),
                 type=Path,
                 metavar="DIR",
                 help="Base directory for artifacts",
             )
 
-    def configure_parser(self) -> None:
-        ...
+    def configure_parser(self) -> None: ...
 
     async def _db_insert_run_meta(self, args: Namespace) -> None:
         if args.db is not None:
             self.db_handler = DBHandler(args.db)
             await self.db_handler.connect()
 
             await self.db_handler.insert_run_meta(
@@ -444,23 +442,20 @@
 class Script(BaseCommand, ABC):
     """Script is a base class for a synchronous gallia command.
     To implement a script, create a subclass and implement the
     .main() method."""
 
     GROUP = "script"
 
-    def setup(self, args: Namespace) -> None:
-        ...
+    def setup(self, args: Namespace) -> None: ...
 
     @abstractmethod
-    def main(self, args: Namespace) -> None:
-        ...
+    def main(self, args: Namespace) -> None: ...
 
-    def teardown(self, args: Namespace) -> None:
-        ...
+    def teardown(self, args: Namespace) -> None: ...
 
     def run(self, args: Namespace) -> int:
         self.setup(args)
         try:
             self.main(args)
         finally:
             self.teardown(args)
@@ -471,23 +466,20 @@
 class AsyncScript(BaseCommand, ABC):
     """AsyncScript is a base class for a asynchronous gallia command.
     To implement an async script, create a subclass and implement
     the .main() method."""
 
     GROUP = "script"
 
-    async def setup(self, args: Namespace) -> None:
-        ...
+    async def setup(self, args: Namespace) -> None: ...
 
     @abstractmethod
-    async def main(self, args: Namespace) -> None:
-        ...
+    async def main(self, args: Namespace) -> None: ...
 
-    async def teardown(self, args: Namespace) -> None:
-        ...
+    async def teardown(self, args: Namespace) -> None: ...
 
     async def _run(self, args: Namespace) -> None:
         await self.setup(args)
         try:
             await self.main(args)
         finally:
             await self.teardown(args)
@@ -524,16 +516,15 @@
     def __init__(self, parser: ArgumentParser, config: Config = Config()) -> None:
         super().__init__(parser, config)
         self.power_supply: PowerSupply | None = None
         self.transport: BaseTransport
         self.dumpcap: Dumpcap | None = None
 
     @abstractmethod
-    async def main(self, args: Namespace) -> None:
-        ...
+    async def main(self, args: Namespace) -> None: ...
 
     async def setup(self, args: Namespace) -> None:
         if args.target is None:
             self.parser.error("--target is required")
 
         if args.power_supply is not None:
             self.power_supply = await PowerSupply.connect(args.power_supply)
```

### Comparing `gallia-1.6.0/src/gallia/command/uds.py` & `gallia-1.7.0/src/gallia/command/uds.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/__init__.py` & `gallia-1.7.0/src/gallia/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/discover/doip.py` & `gallia-1.7.0/src/gallia/commands/discover/doip.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import asyncio
 import socket
 from argparse import Namespace
 from collections.abc import Iterable
-from itertools import chain, product
+from itertools import product
 from urllib.parse import parse_qs, urlparse
 
 import aiofiles
 import psutil
 
 from gallia.command import AsyncScript
 from gallia.log import get_logger
@@ -18,49 +18,56 @@
     TesterPresentRequest,
     TesterPresentResponse,
 )
 from gallia.transports.doip import (
     DiagnosticMessage,
     DiagnosticMessageNegativeAckCodes,
     DoIPConnection,
+    DoIPEntityStatusResponse,
     DoIPNegativeAckError,
     DoIPRoutingActivationDeniedError,
+    GenericHeader,
+    PayloadTypes,
+    ProtocolVersions,
     RoutingActivationRequestTypes,
     RoutingActivationResponseCodes,
     TimingAndCommunicationParameters,
+    VehicleAnnouncementMessage,
 )
 
 logger = get_logger("gallia.discover.doip")
 
 
 class DoIPDiscoverer(AsyncScript):
     """This script scans for active DoIP endpoints and automatically enumerates allowed
     RoutingActivationTypes and known SourceAddresses. Once valid endpoints are acquired,
     the script continues to discover valid TargetAddresses that are accepted and respond
-    to UDS DiagnosticSessionControl requests."""
+    to UDS TesterPresent requests."""
 
     GROUP = "discover"
     COMMAND = "doip"
     SHORT_HELP = "zero-knowledge DoIP enumeration scanner"
     HAS_ARTIFACTS_DIR = True
 
+    protocol_version = ProtocolVersions.ISO_13400_2_2019.value
+
     def configure_parser(self) -> None:
         self.parser.add_argument(
             "--start",
             metavar="INT",
             type=lambda x: int(x, 0),
             default=0x00,
-            help="set start address of TargetAddress search range",
+            help="Set start address of TargetAddress search range",
         )
         self.parser.add_argument(
             "--stop",
             metavar="INT",
             type=lambda x: int(x, 0),
             default=0xFFFF,
-            help="set stop address of TargetAddress search range",
+            help="Set stop address of TargetAddress search range",
         )
         self.parser.add_argument(
             "--target",
             metavar="<DoIP URL target string>",
             type=str,
             default=None,
             help="The more you give, the more automatic detection will be skipped: IP, Port, RoutingActivationType, SourceAddress",
@@ -68,14 +75,24 @@
         self.parser.add_argument(
             "--timeout",
             metavar="SECONDS (FLOAT)",
             type=float,
             default=None,
             help="This flag overrides the default timeout of DiagnosticMessages, which can be used to fine-tune classification of unresponsive ECUs or broadcast detection",
         )
+        self.parser.add_argument(
+            "--tcp-connect-delay",
+            metavar="SECONDS (FLOAT)",
+            type=float,
+            default=0.0,
+            help=(
+                "This flag delays subsequent TCP connect attempts during all enumerations. "
+                "Useful if the DoIP entity requires some time before accepting new TCP requests."
+            ),
+        )
 
     # This is an ugly hack to circumvent AsyncScript's shortcomings regarding return codes
     def run(self, args: Namespace) -> int:
         return asyncio.run(self.main2(args))
 
     async def main(self, args: Namespace) -> None:
         pass
@@ -90,14 +107,17 @@
 
         if self.db_handler is not None:
             try:
                 await self.db_handler.insert_discovery_run("doip")
             except Exception as e:
                 logger.warning(f"Could not write the discovery run to the database: {e!r}")
 
+        # Set TCP connect delay for RoutingActivationType and SourceAddress enumeration
+        tcp_connect_delay: float = args.tcp_connect_delay
+
         # Discover Hostname and Port
         tgt_hostname: str
         tgt_port: int
         if target is not None and target.hostname is not None and target.port is not None:
             logger.notice("[📋] Skipping host/port discovery because given by --target")
             tgt_hostname = target.hostname
             tgt_port = target.port
@@ -108,59 +128,64 @@
 
             if len(hosts) != 1:
                 logger.error("[🍃] Can only continue with a single DoIP host! Give me a --target!")
                 return 11
 
             tgt_hostname, tgt_port = hosts[0]
 
-        # Find correct RoutingActivationType
-        rat_success: list[int] = []
-        rat_wrong_source: list[int] = []
+        # Politely ask for more details via UDP
+        await self.gather_doip_details(tgt_hostname, tgt_port)
+
+        # Enumerate all valid RoutingActivationType/Source Address tuples, but only if required
+        rat_not_unsupported: Iterable[int]
+        rat_not_unknown: Iterable[int]
         if target is not None and "activation_type" in parse_qs(target.query):
             logger.notice("[📋] Skipping RoutingActivationType discovery because given by --target")
-            rat_success = [int(parse_qs(target.query)["activation_type"][0], 0)]
+            rat_not_unsupported = [int(parse_qs(target.query)["activation_type"][0], 0)]
         else:
-            logger.notice("[🔍] Enumerating all RoutingActivationTypes")
-
-            (
-                rat_success,
-                rat_wrong_source,
-            ) = await self.enumerate_routing_activation_types(
-                tgt_hostname,
-                tgt_port,
-                int(parse_qs(target.query)["src_addr"][0], 0)
-                if target is not None and "src_addr" in parse_qs(target.query)
-                else 0xE00,
-            )
-
-        if len(rat_success) == 0 and len(rat_wrong_source) == 0:
-            logger.error(
-                "[🥾] Damn son, didn't find a single routing activation type with unknown source?! OUTTA HERE!"
-            )
-            return 10
-
-        # Discovering correct source address for suitable RoutingActivationRequests
+            rat_not_unsupported = range(0x100)
         if target is not None and "src_addr" in parse_qs(target.query):
             logger.notice("[📋] Skipping SourceAddress discovery because given by --target")
-            targets = [
-                f"doip://{tgt_hostname}:{tgt_port}?activation_type={rat:#x}&src_addr={parse_qs(target.query)['src_addr'][0]}"
-                for rat in rat_success
-            ]
-
+            rat_not_unknown = [int(parse_qs(target.query)["src_addr"][0], 0)]
         else:
-            logger.notice("[🔍] Enumerating all SourceAddresses")
-            targets = await self.enumerate_source_addresses(
-                tgt_hostname,
-                tgt_port,
-                chain(rat_success, rat_wrong_source),
+            rat_not_unknown = range(0x10000)
+
+        # We need to know whether the DoIP entity checks for RoutingActivationTypes or SourceAddresses first
+        # By requesting a RoutingActivation with reserved RAT and reserved SrcAddr, we see it based on the error
+        a, _, _ = await self.enumerate_routing_activation_requests(
+            tgt_hostname, tgt_port, [0x02], [0x00], tcp_connect_delay
+        )
+        routing_activation_types_first = len(a) == 0
+
+        if routing_activation_types_first is True and len(rat_not_unsupported) != 1:
+            logger.notice("[🔍] Enumerating RoutingActivationTypes")
+            rat_not_unsupported, _, _ = await self.enumerate_routing_activation_requests(
+                tgt_hostname, tgt_port, range(0x100), [0x00], tcp_connect_delay
+            )
+            logger.notice(
+                f"[💎] Look what promising RoutingActivationTypes I've found: {', '.join([f'{x:#x}' for x in rat_not_unsupported])}"
+            )
+        elif routing_activation_types_first is False and len(rat_not_unknown) != 1:
+            logger.notice("[🔍] Enumerating SourceAddresses")
+            _, rat_not_unknown, _ = await self.enumerate_routing_activation_requests(
+                tgt_hostname, tgt_port, [0x02], range(0x10000), tcp_connect_delay
             )
+            logger.notice(
+                f"[💎] Look what promising SourceAddresses I've found: {', '.join([f'{x:#x}' for x in rat_not_unknown])}"
+            )
+
+        logger.notice("[🔍] Enumerating valid RoutingActivationType/SourceAddress tuples")
+        _, _, targets = await self.enumerate_routing_activation_requests(
+            tgt_hostname, tgt_port, rat_not_unsupported, rat_not_unknown, tcp_connect_delay
+        )
 
         if len(targets) != 1:
             logger.error(
-                f"[💣] I found {len(targets)} valid RoutingActivationType/SourceAddress combos, but can only continue with exactly one; choose your weapon with --target!"
+                f"[💣] I found {len(targets)} valid RoutingActivationType/SourceAddress tuples, "
+                "but can only continue with exactly one; choose your weapon with --target!"
             )
             return 20
 
         # Enumerate valid TargetAddresses
         if target is not None and "target_addr" in parse_qs(target.query):
             logger.error(
                 "[😵] Why do you give me a target_addr in --target? Am I useless to you??? GOODBYE!"
@@ -178,86 +203,158 @@
         await self.enumerate_target_addresses(
             tgt_hostname,
             tgt_port,
             tgt_rat,
             tgt_src,
             args.start,
             args.stop,
+            tcp_connect_delay,
             args.timeout,
         )
 
         logger.notice("[🛩️] All done, thanks for flying with us!")
         return 0
 
-    async def enumerate_routing_activation_types(
+    async def gather_doip_details(
         self,
         tgt_hostname: str,
         tgt_port: int,
-        src_addr: int,
-    ) -> tuple[list[int], list[int]]:
+    ) -> None:
+        sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+        sock.setblocking(False)
+        sock.bind(("0.0.0.0", 0))
+        loop = asyncio.get_running_loop()
+
+        # We send two packets: a VehicleIdentificationRequest and a DoIPEntityStatusRequest that
+        # only differ in their response, so let's reuse code...
+        for req_type in [
+            PayloadTypes.VehicleIdentificationRequestMessage,
+            PayloadTypes.DoIPEntityStatusRequest,
+        ]:
+            logger.info(f"[🥚] Sending {req_type.name}...")
+
+            hdr = GenericHeader(
+                ProtocolVersion=self.protocol_version
+                if req_type == PayloadTypes.DoIPEntityStatusRequest
+                else 0xFF,
+                PayloadType=req_type,
+                PayloadLength=0,
+            )
+            await loop.sock_sendto(sock, hdr.pack(), (tgt_hostname, tgt_port))
+
+            try:
+                data, _ = await asyncio.wait_for(loop.sock_recvfrom(sock, 1024), 2)
+            except TimeoutError:
+                logger.info("[🐣] No response!")
+                continue
+
+            hdr = GenericHeader.unpack(data[:8])
+
+            if hdr.PayloadType == PayloadTypes.VehicleAnnouncementMessage:
+                logger.notice(
+                    f"[👮] Identification please: {VehicleAnnouncementMessage.unpack(data[8:])}"
+                )
+                logger.info(f"[🎯] Setting protocol version to {hdr.ProtocolVersion}")
+                self.protocol_version = hdr.ProtocolVersion
+            elif hdr.PayloadType == PayloadTypes.DoIPEntityStatusResponse:
+                status = DoIPEntityStatusResponse.unpack(data[8:])
+                logger.notice(
+                    f"[👏] This DoIP entity is a {status.NodeType.name} with "
+                    f"{status.CurrentlyOpenTCP_DATASockets}/{status.MaximumConcurrentTCP_DATASockets} "
+                    f"concurrent TCP sockets currently open and a maximum data size of {status.MaximumDataSize}."
+                )
+
+        sock.close()
+
+    async def enumerate_routing_activation_requests(  # noqa: PLR0913
+        self,
+        tgt_hostname: str,
+        tgt_port: int,
+        routing_activation_types: Iterable[int],
+        source_addresses: Iterable[int],
+        tcp_connect_delay: float,
+    ) -> tuple[list[int], list[int], list[str]]:
         rat_not_unsupported: list[int] = []
-        rat_success: list[int] = []
-        rat_wrong_source: list[int] = []
-        for routing_activation_type in range(0x100):
+        rat_not_unknown: list[int] = []
+        targets: list[str] = []
+
+        for routing_activation_type, source_address in product(
+            routing_activation_types, source_addresses
+        ):
             try:
                 conn = await DoIPConnection.connect(
                     tgt_hostname,
                     tgt_port,
-                    src_addr,
-                    0xAFFE,
+                    source_address,
+                    0xAFFE,  # Dummy target address, never actually used
+                    so_linger=True,  # Ensure that connections do not remain in TIME_WAIT
+                    protocol_version=self.protocol_version,
                 )
             except OSError as e:
-                logger.error(f"[🚨] Mr. Stark I don't feel so good: {e}")
-                return rat_success, rat_wrong_source
+                logger.warning(
+                    f"[🚨] J.A.R.V.I.S., recheck rat {routing_activation_type:#x} and src_addr {source_address:#x}; they failed with {e!r}"
+                )
+                continue
 
             try:
                 await conn.write_routing_activation_request(routing_activation_type)
-                rat_success.append(routing_activation_type)
+            except DoIPRoutingActivationDeniedError as e:
                 logger.info(
-                    f"[🤯] Holy moly, it actually worked for activation_type {routing_activation_type:#x} and src_addr {src_addr:#x}!!!"
+                    f"[🌟] Brilliant, RoutingActivationType {routing_activation_type:#x} and SourceAddress {source_address:#x} yields {e.rac_code.name}"
                 )
-            except DoIPRoutingActivationDeniedError as e:
-                logger.info(f"[🌟] splendid, {routing_activation_type:#x} yields {e.rac_code.name}")
 
                 if e.rac_code != RoutingActivationResponseCodes.UnsupportedActivationType:
                     rat_not_unsupported.append(routing_activation_type)
-
-                if e.rac_code == RoutingActivationResponseCodes.UnknownSourceAddress:
-                    rat_wrong_source.append(routing_activation_type)
+                if e.rac_code != RoutingActivationResponseCodes.UnknownSourceAddress:
+                    rat_not_unknown.append(source_address)
+                continue
 
             finally:
                 await conn.close()
+                await asyncio.sleep(tcp_connect_delay)
 
-        logger.notice(
-            f"[💎] Look what RoutingActivationTypes I've found that are not 'unsupported': {', '.join([f'{x:#x}' for x in rat_not_unsupported])}"
-        )
-        return rat_success, rat_wrong_source
+            targets.append(
+                f"doip://{tgt_hostname}:{tgt_port}?protocol_version={self.protocol_version}&activation_type={routing_activation_type:#x}&src_addr={source_address:#x}"
+            )
+            logger.notice(f"[🤯] Holy moly, it actually worked: {targets[-1]}")
+            async with aiofiles.open(
+                self.artifacts_dir.joinpath("1_valid_routing_activation_requests.txt"), "a"
+            ) as f:
+                await f.write(f"{targets[-1]}\n")
+
+        if len(targets) > 0:
+            logger.notice("[⚔️] It's dangerous to test alone, take one of these:")
+            for item in targets:
+                logger.notice(item)
+
+        return rat_not_unsupported, rat_not_unknown, targets
 
     async def enumerate_target_addresses(  # noqa: PLR0913
         self,
         tgt_hostname: str,
         tgt_port: int,
         correct_rat: int,
         correct_src: int,
         start: int,
         stop: int,
+        tcp_connect_delay: float,
         timeout: None | float = None,
     ) -> None:
         known_targets = []
         unreachable_targets = []
         responsive_targets = []
         search_space = range(start, stop + 1)
 
         conn = await self.create_DoIP_conn(tgt_hostname, tgt_port, correct_rat, correct_src, 0xAFFE)
 
         for target_addr in search_space:
             logger.debug(f"[🚧] Attempting connection to {target_addr:#x}")
 
             conn.target_addr = target_addr
-            current_target = f"doip://{tgt_hostname}:{tgt_port}?activation_type={correct_rat:#x}&src_addr={correct_src:#x}&target_addr={target_addr:#x}"
+            current_target = f"doip://{tgt_hostname}:{tgt_port}?protocol_version={self.protocol_version}&activation_type={correct_rat:#x}&src_addr={correct_src:#x}&target_addr={target_addr:#x}"
 
             try:
                 req = TesterPresentRequest(suppress_response=False)
                 await conn.write_diag_request(req.pdu)
 
                 # If we reach this, the request was not denied due to unknown TargetAddress
                 known_targets.append(current_target)
@@ -317,37 +414,40 @@
                     )
                     async with aiofiles.open(
                         self.artifacts_dir.joinpath("7_targets_with_errors.txt"), "a"
                     ) as f:
                         await f.write(f"{target_addr:#x}: {e.nack_code.name}\n")
                     continue
 
-            except asyncio.TimeoutError:  # This triggers when DoIP ACK but no UDS reply
+            except TimeoutError:  # This triggers when DoIP ACK but no UDS reply
                 logger.info(f"[🙊] Presumably no active ECU on target address {target_addr:#x}")
                 async with aiofiles.open(
                     self.artifacts_dir.joinpath("5_unresponsive_targets.txt"), "a"
                 ) as f:
                     await f.write(f"{current_target}\n")
                 continue
 
-            except (ConnectionError, ConnectionResetError) as e:
+            except ConnectionError as e:
                 # Whenever this triggers, but sometimes connections are closed not by us
-                logger.warn(f"[🫦] Sexy, but unexpected: {target_addr:#x} triggered {e}")
+                logger.warn(f"[🫦] Sexy, but unexpected: {target_addr:#x} triggered {e!r}")
                 async with aiofiles.open(
                     self.artifacts_dir.joinpath("7_targets_with_errors.txt"), "a"
                 ) as f:
                     await f.write(f"{target_addr:#x}: {e}\n")
                 # Re-establish DoIP connection
                 await conn.close()
+                await asyncio.sleep(tcp_connect_delay)
+
                 conn = await self.create_DoIP_conn(
                     tgt_hostname, tgt_port, correct_rat, correct_src, 0xAFFE
                 )
                 continue
 
         await conn.close()
+        await asyncio.sleep(tcp_connect_delay)
 
         logger.notice(
             f"[⚔️] It's dangerous to test alone, take one of these {len(known_targets)} known targets:"
         )
         for item in known_targets:
             logger.notice(item)
 
@@ -378,22 +478,24 @@
         while True:
             try:
                 conn = await DoIPConnection.connect(
                     hostname,
                     port,
                     src_addr,
                     target_addr,
+                    so_linger=True,  # Ensure that connections do not remain in TIME_WAIT
+                    protocol_version=self.protocol_version,
                 )
                 logger.info("[📫] Sending RoutingActivationRequest")
                 await conn.write_routing_activation_request(
                     RoutingActivationRequestTypes(routing_activation_type)
                 )
             except Exception as e:  # TODO this probably is too broad
                 logger.warning(
-                    f"[🫨] Got me some good errors when it should be working (dis an infinite loop): {e}"
+                    f"[🫨] Got me some good errors when it should be working (dis an infinite loop): {e!r}"
                 )
                 continue
             return conn
 
     async def read_diag_request_custom(self, conn: DoIPConnection) -> tuple[int | None, bytes]:
         while True:
             hdr, payload = await conn.read_frame()
@@ -405,116 +507,55 @@
             if payload.TargetAddress != conn.src_addr:
                 logger.warning(
                     f"[🤌] You talking to me?! Unexpected DoIP target address: {payload.TargetAddress:#04x}"
                 )
                 continue
             return None, payload.UserData
 
-    async def enumerate_source_addresses(
-        self,
-        tgt_hostname: str,
-        tgt_port: int,
-        valid_routing_activation_types: Iterable[int],
-    ) -> list[str]:
-        known_sourceAddresses: list[int] = []
-        denied_sourceAddresses: list[int] = []
-        targets: list[str] = []
-        for routing_activation_type, source_address in product(
-            valid_routing_activation_types, range(0x0000, 0x10000)
-        ):
-            try:
-                conn = await DoIPConnection.connect(
-                    tgt_hostname,
-                    tgt_port,
-                    source_address,
-                    0xAFFE,
-                )
-            except OSError as e:
-                logger.error(f"[🚨] Mr. Stark I don't feel so good: {e}")
-                return []
-
-            try:
-                await conn.write_routing_activation_request(routing_activation_type)
-            except DoIPRoutingActivationDeniedError as e:
-                logger.info(f"[🌟] splendid, {source_address:#x} yields {e.rac_code.name}")
-
-                if e.rac_code != RoutingActivationResponseCodes.UnknownSourceAddress:
-                    denied_sourceAddresses.append(source_address)
-                    async with aiofiles.open(
-                        self.artifacts_dir.joinpath("2_denied_src_addresses.txt"), "a"
-                    ) as f:
-                        await f.write(
-                            f"activation_type={routing_activation_type:#x},src_addr={source_address:#x}: {e.rac_code.name}\n"
-                        )
-
-                continue
-
-            finally:
-                await conn.close()
-
-            logger.info(
-                f"[🤯] Holy moly, it actually worked for activation_type {routing_activation_type:#x} and src_addr {source_address:#x}!!!"
-            )
-            known_sourceAddresses.append(source_address)
-            targets.append(
-                f"doip://{tgt_hostname}:{tgt_port}?activation_type={routing_activation_type:#x}&src_addr={source_address:#x}"
-            )
-            async with aiofiles.open(
-                self.artifacts_dir.joinpath("1_valid_src_addresses.txt"), "a"
-            ) as f:
-                await f.write(f"{targets[-1]}\n")
-
-        # Print valid SourceAddresses and suitable target string for config
-        logger.notice(
-            f"[💀] Look what SourceAddresses got denied: {', '.join([f'{x:#x}' for x in denied_sourceAddresses])}"
-        )
-        logger.notice(
-            f"[💎] Look what valid SourceAddresses I've found: {', '.join([f'{x:#x}' for x in known_sourceAddresses])}"
-        )
-        logger.notice("[⚔️] It's dangerous to test alone, take one of these:")
-        for item in targets:
-            logger.notice(item)
-        return targets
-
     async def run_udp_discovery(self) -> list[tuple[str, int]]:
         all_ips = []
         found = []
 
         for iface in psutil.net_if_addrs().values():
             for ip in iface:
                 # we only work with broadcastable IPv4
                 if ip.family != socket.AF_INET or ip.broadcast is None:
                     continue
                 all_ips.append(ip)
 
         for ip in all_ips:
             logger.info(f"[💌] Sending DoIP VehicleIdentificationRequest to {ip.broadcast}")
             sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+            sock.setblocking(False)
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-            sock.settimeout(2)
             sock.bind((ip.address, 0))
+            loop = asyncio.get_running_loop()
 
-            sock.sendto(b"\xff\x00\x00\x01\x00\x00\x00\x00", (ip.broadcast, 13400))
+            hdr = GenericHeader(0xFF, PayloadTypes.VehicleIdentificationRequestMessage, 0x00)
+            await loop.sock_sendto(sock, hdr.pack(), (ip.broadcast, 13400))
             try:
-                data, addr = sock.recvfrom(1024)
+                while True:
+                    data, addr = await asyncio.wait_for(loop.sock_recvfrom(sock, 1024), 2)
+                    info = VehicleAnnouncementMessage.unpack(data[8:])
+                    logger.notice(f"[💝]: {addr} responded: {info}")
+                    found.append(addr)
             except TimeoutError:
-                logger.info("[💔] no response")
+                logger.info("[💔] Reached timeout...")
                 continue
             finally:
                 sock.close()
 
-            # Hardcoded slices
-            vin = data[8 : 8 + 17]
-            target_addr = int.from_bytes(data[25:27], "big")
+        if len(found) > 0:
+            logger.notice("[💎] Look what valid hosts I've found:")
+            for item in found:
+                url = f"doip://{item[0]}:{item[1]}"
+                logger.notice(url)
+                async with aiofiles.open(
+                    self.artifacts_dir.joinpath("0_valid_hosts.txt"), "a"
+                ) as f:
+                    await f.write(f"{url}\n")
+        else:
             logger.notice(
-                f"[💝]: {addr} responded with VIN {vin.decode('ascii')} and target_addr {target_addr:#x}"
+                "[👸] Your princess is in another castle: no DoIP endpoints here it seems..."
             )
-            found.append(addr)
-
-        logger.notice("[💎] Look what valid hosts I've found:")
-        for item in found:
-            url = f"doip://{item[0]}:{item[1]}"
-            logger.notice(url)
-            async with aiofiles.open(self.artifacts_dir.joinpath("0_valid_hosts.txt"), "a") as f:
-                await f.write(f"{url}\n")
 
         return found
```

### Comparing `gallia-1.6.0/src/gallia/commands/discover/find_xcp.py` & `gallia-1.7.0/src/gallia/commands/discover/find_xcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import asyncio
 import socket
 import struct
 from argparse import ArgumentParser, Namespace
 
 from gallia.command import AsyncScript
 from gallia.config import Config
 from gallia.log import get_logger
@@ -184,15 +183,15 @@
                 logger.info(f"Receive data on TCP port {port}: {ret}")
                 if len(data_ret) > 0 and data_ret[0] == 0xFF:
                     logger.result(f"XCP Slave on UDP port {port}, data: {ret}")
                     endpoints.append(port)
                 else:
                     logger.info(f"UDP port {port} is no XCP slave, data: {ret}")
 
-            except socket.timeout:
+            except TimeoutError:
                 logger.info(f"Timeout on UDP port {port}")
 
             self.xcp_disconnect(server)
             self.socket.close()
 
         logger.result(f"Finished; Found {len(endpoints)} XCP endpoints via UDP")
 
@@ -228,15 +227,15 @@
                         logger.result(msg)
                         endpoints.append((can_id, master))
                     else:
                         logger.info(
                             f"Received non XCP answer for CAN-ID {can_id_repr(can_id)}: {can_id_repr(master)}:"
                             f"{bytes_repr(data)}"
                         )
-            except asyncio.TimeoutError:
+            except TimeoutError:
                 pass
 
         logger.result(f"Finished; Found {len(endpoints)} XCP endpoints via CAN")
 
     def test_eth_broadcast(self, args: Namespace) -> None:
         # TODO: rewrite as async
 
@@ -263,11 +262,11 @@
             while True:
                 data, slave = self.socket.recvfrom(16)
                 if not data:
                     break
 
                 logger.result(f"Found XCP slave: {slave} {bytes_repr(data)}")
                 endpoints.append(slave)
-        except socket.timeout:
+        except TimeoutError:
             logger.info("Timeout")
 
         logger.result(f"Finished; Found {len(endpoints)} XCP endpoints via multicast group")
```

### Comparing `gallia-1.6.0/src/gallia/commands/discover/uds/isotp.py` & `gallia-1.7.0/src/gallia/commands/discover/uds/isotp.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
             await transport.sendto(pdu, timeout=0.1, dst=dst_addr)
             try:
                 addr, payload = await transport.recvfrom(timeout=0.1)
                 if addr == ID:
                     logger.info(f"The same CAN ID {can_id_repr(ID)} answered. Skipping…")
                     continue
-            except asyncio.TimeoutError:
+            except TimeoutError:
                 continue
 
             while True:
                 # The recv buffer needs to be flushed to avoid
                 # wrong results...
                 try:
                     new_addr, _ = await transport.recvfrom(timeout=0.1)
@@ -196,15 +196,15 @@
                             f"seems that broadcast was triggered on CAN ID {can_id_repr(ID)}, "
                             f"got answer from {can_id_repr(new_addr)}"
                         )
                     else:
                         logger.info(
                             f"seems like a large ISO-TP packet was received on CAN ID {can_id_repr(ID)}"
                         )
-                except asyncio.TimeoutError:
+                except TimeoutError:
                     if is_broadcast:
                         logger.result(
                             f"seems that broadcast was triggered on CAN ID {can_id_repr(ID)}, "
                             f"got answer from {can_id_repr(addr)}"
                         )
                     else:
                         logger.result(
```

### Comparing `gallia-1.6.0/src/gallia/commands/fuzz/uds/pdu.py` & `gallia-1.7.0/src/gallia/commands/fuzz/uds/pdu.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                     if can_id in can_msgs:
                         if msg != can_msgs[can_id]:
                             logger.result(f"Message for {can_id:03x} changed to {msg.hex()}")
                             can_msgs[can_id] = msg
                     else:
                         can_msgs[can_id] = msg
                         logger.result(f"Observed new message from {can_id:03x}: {msg.hex()}")
-                except asyncio.TimeoutError:
+                except TimeoutError:
                     continue
 
         except asyncio.CancelledError:
             logger.debug("Can message observer task cancelled")
 
     async def main(self, args: Namespace) -> None:
         if args.observe_can_ids:
@@ -157,15 +157,15 @@
                                 negative_responses[resp.response_code] += 1
                             else:
                                 negative_responses[resp.response_code] = 1
                         else:
                             logger.result(f"0x{did:0x}: {resp}")
                             positive_DIDs += 1
 
-                    except asyncio.TimeoutError:
+                    except TimeoutError:
                         logger.warning(f"0x{did :0x}: Retries exceeded")
                         timeout_DIDs += 1
                     except IllegalResponse as e:
                         logger.warning(f"{repr(e)}")
                         illegal_resp += 1
                     # Temporary patch: Exception handler is deleted when it goes productive
                     except ConnectionError:
@@ -181,12 +181,12 @@
                 logger.result(f"Positive replies: {positive_DIDs}")
 
                 logger.result(f"Timeouts: {timeout_DIDs}")
                 logger.result(f"Illegal replies: {illegal_resp}")
                 logger.result(f"Flow control frames missing: {flow_control_miss}")
 
                 logger.info(f"Leaving session 0x{session:02x} via hook")
-                await self.ecu.leave_session(session)
+                await self.ecu.leave_session(session, sleep=args.power_cycle_sleep)
 
         if args.observe_can_ids:
             recv_task.cancel()
             await recv_task
```

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/generic/pdu.py` & `gallia-1.7.0/src/gallia/commands/primitive/generic/pdu.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/dtc.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/dtc.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/ecu_reset.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/ecu_reset.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,14 @@
             logger.info(f"try sub-func: {g_repr(args.subfunc)}")
             resp = await self.ecu.ecu_reset(args.subfunc)
             if isinstance(resp, NegativeResponse):
                 msg = f"ECU Reset {g_repr(args.subfunc)} failed in session: {g_repr(args.session)}: {resp}"
                 logger.error(msg)
             else:
                 logger.result(f"ECU Reset {g_repr(args.subfunc)} succeeded")
-        except asyncio.TimeoutError:
+        except TimeoutError:
             logger.error("Timeout")
             await asyncio.sleep(10)
         except ConnectionError:
             msg = f"Lost connection to ECU, session: {g_repr(args.session)} subFunc: {g_repr(args.subfunc)}"
             logger.error(msg)
             return
```

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/iocbi.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/iocbi.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/pdu.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/pdu.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/ping.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/ping.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/rdbi.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/rdbi.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/rmba.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/rmba.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/rtcl.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/rtcl.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/vin.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/vin.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/wdbi.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/wdbi.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/wmba.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/wmba.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/primitive/uds/xcp.py` & `gallia-1.7.0/src/gallia/commands/primitive/uds/xcp.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/commands/scan/uds/identifiers.py` & `gallia-1.7.0/src/gallia/commands/scan/uds/identifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import asyncio
 import binascii
 import reprlib
 from argparse import Namespace
 from itertools import product
 
 from gallia.command import UDSScanner
 from gallia.log import get_logger
@@ -126,15 +125,15 @@
 
                 logger.result(f"Starting scan in session: {g_repr(session)}")
 
                 await self.perform_scan(args, session)
 
                 logger.result(f"Scan in session {g_repr(session)} is complete!")
                 logger.info(f"Leaving session {g_repr(session)} via hook")
-                await self.ecu.leave_session(session)
+                await self.ecu.leave_session(session, sleep=args.power_cycle_sleep)
 
     async def perform_scan(self, args: Namespace, session: None | int = None) -> None:
         positive_DIDs = 0
         abnormal_DIDs = 0
         timeout_DIDs = 0
         sub_functions = [0x00]
 
@@ -188,15 +187,15 @@
             if args.payload:
                 pdu += args.payload
 
             try:
                 resp = await self.ecu.send_raw(
                     pdu, config=UDSRequestConfig(tags=["ANALYZE"], max_retry=3)
                 )
-            except asyncio.TimeoutError:
+            except TimeoutError:
                 logger.result(f"{g_repr(DID)}: Retries exceeded")
                 timeout_DIDs += 1
                 continue
             except IllegalResponse as e:
                 logger.warning(g_repr(e))
                 continue
```

### Comparing `gallia-1.6.0/src/gallia/commands/scan/uds/memory.py` & `gallia-1.7.0/src/gallia/commands/scan/uds/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import asyncio
 import sys
 from argparse import Namespace
 from binascii import unhexlify
 
 from gallia.command import UDSScanner
 from gallia.log import get_logger
 from gallia.services.uds import NegativeResponse, UDSErrorCodes, UDSRequestConfig
@@ -94,15 +93,15 @@
                         f"Aborting scan on session {g_repr(args.session)}; "
                         + f"current memory address was {g_repr(addr)}"
                     )
                     sys.exit(1)
 
             try:
                 resp = await self.ecu.send_raw(pdu, config=UDSRequestConfig(tags=["ANALYZE"]))
-            except asyncio.TimeoutError:
+            except TimeoutError:
                 logger.result(f"Address {g_repr(addr)}: timeout")
                 continue
 
             if isinstance(resp, NegativeResponse):
                 if resp.response_code is UDSErrorCodes.requestOutOfRange:
                     logger.info(f"Address {g_repr(addr)}: {resp}")
                 else:
```

### Comparing `gallia-1.6.0/src/gallia/commands/scan/uds/reset.py` & `gallia-1.7.0/src/gallia/commands/scan/uds/reset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import asyncio
 import reprlib
 import sys
 from argparse import Namespace
 from typing import Any
 
 from gallia.command import UDSScanner
 from gallia.log import get_logger
@@ -75,15 +74,15 @@
                 if isinstance(resp, NegativeResponse):
                     logger.warning(f"Switching to session {g_repr(session)} failed: {resp}")
                     continue
 
                 logger.result(f"Scanning in session: {g_repr(session)}")
                 await self.perform_scan(args, session)
 
-                await self.ecu.leave_session(session)
+                await self.ecu.leave_session(session, sleep=args.power_cycle_sleep)
 
     async def perform_scan(self, args: Namespace, session: None | int = None) -> None:
         l_ok: list[int] = []
         l_timeout: list[int] = []
         l_error: list[Any] = []
 
         for sub_func in range(0x01, 0x80):
@@ -125,27 +124,27 @@
                 if isinstance(resp, NegativeResponse):
                     logger.warning(
                         f"Could not reboot ECU after testing reset level {g_repr(sub_func)}"
                     )
                 else:
                     await self.ecu.wait_for_ecu()
 
-            except asyncio.TimeoutError:
+            except TimeoutError:
                 l_timeout.append(sub_func)
                 if not args.power_cycle:
                     logger.error(f"ECU did not respond after reset level {g_repr(sub_func)}; exit")
                     sys.exit(1)
 
                 logger.warning(
                     f"ECU did not respond after reset level {g_repr(sub_func)}; try power cycle…"
                 )
                 try:
-                    await self.ecu.power_cycle()
+                    await self.ecu.power_cycle(args.power_cycle_sleep)
                     await self.ecu.wait_for_ecu()
-                except (ConnectionError, asyncio.TimeoutError) as e:
+                except (TimeoutError, ConnectionError) as e:
                     logger.error(f"Failed to recover ECU: {g_repr(e)}; exit")
                     sys.exit(1)
             except ConnectionError:
                 msg = f"{g_repr(sub_func)}: lost connection to ECU (post), current session: {g_repr(session)}"
                 logger.warning(msg)
                 await self.ecu.reconnect()
                 continue
```

### Comparing `gallia-1.6.0/src/gallia/commands/scan/uds/sa_dump_seeds.py` & `gallia-1.7.0/src/gallia/commands/scan/uds/sa_dump_seeds.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import asyncio
 import binascii
 import sys
 import time
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 
 import aiofiles
@@ -69,18 +68,18 @@
             const=1,
             default=None,
             type=int,
             help="Attempt to fool brute force protection by resetting the ECU after every nth requested seed.",
         )
         self.parser.add_argument(
             "--duration",
-            default=12 * 60,
+            default=0,
             type=float,
             metavar="FLOAT",
-            help="Run script for N minutes; zero or negative for infinite runtime",
+            help="Run script for N minutes; zero or negative for infinite runtime (default)",
         )
         self.parser.add_argument(
             "--data-record",
             metavar="HEXSTRING",
             type=binascii.unhexlify,
             default=b"",
             help="Append an optional data record to each seed request",
@@ -154,15 +153,15 @@
                     logger.error(f"ECU persistently lost session {g_repr(args.session)}")
                     sys.exit(1)
 
             reset = False
 
             try:
                 seed = await self.request_seed(args.level, args.data_record)
-            except asyncio.TimeoutError:
+            except TimeoutError:
                 logger.error("Timeout while requesting seed")
                 continue
             except Exception as e:
                 logger.critical(f"Error while requesting seed: {g_repr(e)}")
                 sys.exit(1)
 
             if seed is None:
@@ -175,15 +174,15 @@
 
             last_seed = seed
 
             if args.send_zero_key > 0:
                 try:
                     if await self.send_key(args.level, bytes(args.send_zero_key)):
                         break
-                except asyncio.TimeoutError:
+                except TimeoutError:
                     logger.warning("Timeout while sending key")
                     continue
                 except Exception as e:
                     logger.critical(f"Error while sending key: {g_repr(e)}")
                     sys.exit(1)
 
             runs_since_last_reset += 1
@@ -193,23 +192,23 @@
                 runs_since_last_reset = 0
 
                 try:
                     logger.info("Resetting the ECU")
                     await self.ecu.ecu_reset(0x01)
                     logger.info("Waiting for the ECU to recover…")
                     await self.ecu.wait_for_ecu()
-                except asyncio.TimeoutError:
+                except TimeoutError:
                     logger.error("ECU did not respond after reset; exiting…")
                     sys.exit(1)
                 except ConnectionError:
                     logger.warning(
                         "Lost connection to the ECU after performing a reset. "
                         "Attempting to reconnect…"
                     )
                     await self.ecu.reconnect()
 
                 # Re-enter session. Checking/logging will be done at the beginning of next iteration
                 await self.ecu.set_session(session)
 
         await file.close()
         self.log_size(seeds_file, time.time() - start_time)
-        await self.ecu.leave_session(session)
+        await self.ecu.leave_session(session, sleep=args.power_cycle_sleep)
```

### Comparing `gallia-1.6.0/src/gallia/commands/scan/uds/services.py` & `gallia-1.7.0/src/gallia/commands/scan/uds/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
-import asyncio
 import reprlib
 from argparse import BooleanOptionalAction, Namespace
 from typing import Any
 
 from gallia.command import UDSScanner
 from gallia.log import get_logger
 from gallia.services.uds import (
@@ -109,15 +108,15 @@
                     )
                     continue
 
                 logger.result(f"scanning in session {g_repr(session)}")
 
                 found[session] = await self.perform_scan(args, session)
 
-                await self.ecu.leave_session(session)
+                await self.ecu.leave_session(session, sleep=args.power_cycle_sleep)
 
         for key, value in found.items():
             logger.result(f"findings in session 0x{key:02X}:")
             for sid, data in value.items():
                 self.result.append((key, sid))
                 try:
                     logger.result(f"  [{g_repr(sid)}] {UDSIsoServices(sid).name}: {data}")
@@ -145,15 +144,15 @@
                     )
                     break
 
             for length_payload in [1, 2, 3, 5]:
                 pdu = bytes([sid]) + bytes(length_payload)
                 try:
                     resp = await self.ecu.send_raw(pdu, config=UDSRequestConfig(tags=["ANALYZE"]))
-                except asyncio.TimeoutError:
+                except TimeoutError:
                     logger.info(f"{g_repr(sid)}: timeout")
                     continue
                 except MalformedResponse as e:
                     logger.warning(f"{g_repr(sid)}: {e!r} occurred, this needs to be investigated!")
                     continue
 
                 if isinstance(resp, NegativeResponse) and resp.response_code in [
```

### Comparing `gallia-1.6.0/src/gallia/commands/scan/uds/sessions.py` & `gallia-1.7.0/src/gallia/commands/scan/uds/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                                 logger.warning(
                                     f"Could not reset ECU with {EcuResetSubFuncs(args.reset).name if args.reset in iter(EcuResetSubFuncs) else args.reset}: {resp}"
                                     f"; continuing without reset"
                                 )
                             else:
                                 logger.info("Waiting for the ECU to recover…")
                                 await self.ecu.wait_for_ecu(timeout=args.timeout)
-                        except (asyncio.TimeoutError, ConnectionError):
+                        except (TimeoutError, ConnectionError):
                             logger.warning(
                                 "Lost connection to the ECU after performing a reset. "
                                 "Attempting to reconnect…"
                             )
                             await self.ecu.reconnect()
 
                     try:
@@ -218,15 +218,15 @@
                                 {
                                     "session": session,
                                     "stack": stack,
                                     "error": resp.response_code,
                                 }
                             )
 
-                    except asyncio.TimeoutError:
+                    except TimeoutError:
                         logger.warning(f"Could not change to session {g_repr(session)}: Timeout")
                         continue
                     except Exception as e:
                         logger.warning(f"Mamma mia: {repr(e)}")
 
         logger.result("Scan finished; Found the following sessions:")
         previous_session = 0
```

### Comparing `gallia-1.6.0/src/gallia/commands/script/vecu.py` & `gallia-1.7.0/src/gallia/commands/script/vecu.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/config.py` & `gallia-1.7.0/src/gallia/config.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/db/handler.py` & `gallia-1.7.0/src/gallia/db/handler.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/dumpcap.py` & `gallia-1.7.0/src/gallia/dumpcap.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/log.py` & `gallia-1.7.0/src/gallia/log.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/plugins.py` & `gallia-1.7.0/src/gallia/plugins.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/powersupply.py` & `gallia-1.7.0/src/gallia/powersupply.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/services/uds/__init__.py` & `gallia-1.7.0/src/gallia/services/uds/__init__.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/services/uds/core/client.py` & `gallia-1.7.0/src/gallia/services/uds/core/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             if i > 0:
                 logger.info(f"Requesting UDS PDU failed; retrying: {i} from {max_retry}…")
             try:
                 logger.debug(request.pdu.hex(), extra={"tags": ["write", "uds"] + tags})
                 raw_resp = await self.transport.request_unsafe(request.pdu, timeout, config.tags)
                 if raw_resp == b"":
                     raise BrokenPipeError("connection to target lost")
-            except asyncio.TimeoutError as e:
+            except TimeoutError as e:
                 logger.debug(f"{request} failed with: {repr(e)}")
                 last_exception = MissingResponse(request, str(e))
                 await asyncio.sleep(wait_time)
                 continue
 
             logger.debug(raw_resp.hex(), extra={"tags": ["read", "uds"] + tags})
             resp = parse_pdu(raw_resp, request)
@@ -113,15 +113,15 @@
                     + f"waiting for next message: {n_timeout}/{int(max_n_timeout)}s"
                 )
                 try:
                     raw_resp = await self._read(timeout=waiting_time, tags=config.tags)
                     if raw_resp == b"":
                         raise BrokenPipeError("connection to target lost")
                     logger.debug(raw_resp.hex(), extra={"tags": ["read", "uds"] + tags})
-                except asyncio.TimeoutError as e:
+                except TimeoutError as e:
                     # Send a tester present to indicate that
                     # we are still there.
                     # TODO Is this really necessary?
                     await self._tester_present(suppress_resp=True)
                     n_timeout += 1
                     if n_timeout >= max_n_timeout:
                         last_exception = MissingResponse(request, str(e))
@@ -878,224 +878,197 @@
             service.RequestTransferExitRequest(transfer_request_parameter_record),
             config,
         )
 
     @overload
     async def request(
         self, request: service.RawRequest, config: UDSRequestConfig | None = None
-    ) -> service.NegativeResponse | service.PositiveResponse:
-        ...
+    ) -> service.NegativeResponse | service.PositiveResponse: ...
 
     @overload
     async def request(
         self,
         request: service.DiagnosticSessionControlRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.DiagnosticSessionControlResponse:
-        ...
+    ) -> service.NegativeResponse | service.DiagnosticSessionControlResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ECUResetRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ECUResetResponse:
-        ...
+    ) -> service.NegativeResponse | service.ECUResetResponse: ...
 
     @overload
     async def request(
         self,
         request: service.RequestSeedRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.SecurityAccessResponse:
-        ...
+    ) -> service.NegativeResponse | service.SecurityAccessResponse: ...
 
     @overload
     async def request(
         self, request: service.SendKeyRequest, config: UDSRequestConfig | None = None
-    ) -> service.NegativeResponse | service.SecurityAccessResponse:
-        ...
+    ) -> service.NegativeResponse | service.SecurityAccessResponse: ...
 
     @overload
     async def request(
         self,
         request: service.CommunicationControlRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.CommunicationControlResponse:
-        ...
+    ) -> service.NegativeResponse | service.CommunicationControlResponse: ...
 
     @overload
     async def request(
         self,
         request: service.TesterPresentRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.TesterPresentResponse:
-        ...
+    ) -> service.NegativeResponse | service.TesterPresentResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ControlDTCSettingRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ControlDTCSettingResponse:
-        ...
+    ) -> service.NegativeResponse | service.ControlDTCSettingResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ReadDataByIdentifierRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ReadDataByIdentifierResponse:
-        ...
+    ) -> service.NegativeResponse | service.ReadDataByIdentifierResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ReadMemoryByAddressRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ReadMemoryByAddressResponse:
-        ...
+    ) -> service.NegativeResponse | service.ReadMemoryByAddressResponse: ...
 
     @overload
     async def request(
         self,
         request: service.WriteDataByIdentifierRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.WriteDataByIdentifierResponse:
-        ...
+    ) -> service.NegativeResponse | service.WriteDataByIdentifierResponse: ...
 
     @overload
     async def request(
         self,
         request: service.WriteMemoryByAddressRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.WriteMemoryByAddressResponse:
-        ...
+    ) -> service.NegativeResponse | service.WriteMemoryByAddressResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ClearDiagnosticInformationRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ClearDiagnosticInformationResponse:
-        ...
+    ) -> service.NegativeResponse | service.ClearDiagnosticInformationResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ReportNumberOfDTCByStatusMaskRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ReportNumberOfDTCByStatusMaskResponse:
-        ...
+    ) -> service.NegativeResponse | service.ReportNumberOfDTCByStatusMaskResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ReportDTCByStatusMaskRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ReportDTCByStatusMaskResponse:
-        ...
+    ) -> service.NegativeResponse | service.ReportDTCByStatusMaskResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ReportMirrorMemoryDTCByStatusMaskRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ReportMirrorMemoryDTCByStatusMaskResponse:
-        ...
+    ) -> service.NegativeResponse | service.ReportMirrorMemoryDTCByStatusMaskResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ReportNumberOfMirrorMemoryDTCByStatusMaskRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ReportNumberOfMirrorMemoryDTCByStatusMaskResponse:
-        ...
+    ) -> service.NegativeResponse | service.ReportNumberOfMirrorMemoryDTCByStatusMaskResponse: ...
 
     @overload
     async def request(
         self,
         request: service.ReportNumberOfEmissionsRelatedOBDDTCByStatusMaskRequest,
         config: UDSRequestConfig | None = None,
     ) -> (
         service.NegativeResponse | service.ReportNumberOfEmissionsRelatedOBDDTCByStatusMaskResponse
-    ):
-        ...
+    ): ...
 
     @overload
     async def request(
         self,
         request: service.ReportEmissionsRelatedOBDDTCByStatusMaskRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.ReportEmissionsRelatedOBDDTCByStatusMaskResponse:
-        ...
+    ) -> service.NegativeResponse | service.ReportEmissionsRelatedOBDDTCByStatusMaskResponse: ...
 
     @overload
     async def request(
         self,
         request: service.InputOutputControlByIdentifierRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.InputOutputControlByIdentifierResponse:
-        ...
+    ) -> service.NegativeResponse | service.InputOutputControlByIdentifierResponse: ...
 
     @overload
     async def request(
         self,
         request: service.StartRoutineRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.StartRoutineResponse:
-        ...
+    ) -> service.NegativeResponse | service.StartRoutineResponse: ...
 
     @overload
     async def request(
         self,
         request: service.StopRoutineRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.StopRoutineResponse:
-        ...
+    ) -> service.NegativeResponse | service.StopRoutineResponse: ...
 
     @overload
     async def request(
         self,
         request: service.RequestRoutineResultsRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.RequestRoutineResultsResponse:
-        ...
+    ) -> service.NegativeResponse | service.RequestRoutineResultsResponse: ...
 
     @overload
     async def request(
         self,
         request: service.RequestDownloadRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.RequestDownloadResponse:
-        ...
+    ) -> service.NegativeResponse | service.RequestDownloadResponse: ...
 
     @overload
     async def request(
         self,
         request: service.RequestUploadRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.RequestUploadResponse:
-        ...
+    ) -> service.NegativeResponse | service.RequestUploadResponse: ...
 
     @overload
     async def request(
         self,
         request: service.TransferDataRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.TransferDataResponse:
-        ...
+    ) -> service.NegativeResponse | service.TransferDataResponse: ...
 
     @overload
     async def request(
         self,
         request: service.RequestTransferExitRequest,
         config: UDSRequestConfig | None = None,
-    ) -> service.NegativeResponse | service.RequestTransferExitResponse:
-        ...
+    ) -> service.NegativeResponse | service.RequestTransferExitResponse: ...
 
     async def request(
         self, request: service.UDSRequest, config: UDSRequestConfig | None = None
     ) -> service.UDSResponse:
         """Sends a raw UDS request and returns the response.
         Network errors are handled via exponential backoff.
         Pending errors, triggered by the ECU are resolved as well.
```

### Comparing `gallia-1.6.0/src/gallia/services/uds/core/constants.py` & `gallia-1.7.0/src/gallia/services/uds/core/constants.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/services/uds/core/exception.py` & `gallia-1.7.0/src/gallia/services/uds/core/exception.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/services/uds/core/service.py` & `gallia-1.7.0/src/gallia/services/uds/core/service.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/services/uds/core/utils.py` & `gallia-1.7.0/src/gallia/services/uds/core/utils.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/services/uds/ecu.py` & `gallia-1.7.0/src/gallia/services/uds/ecu.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,16 +68,15 @@
         self.tester_present_task: Task[None] | None = None
         self.tester_present_interval: float | None = None
         self.power_supply = power_supply
         self.state = ECUState()
         self.db_handler: DBHandler | None = None
         self.implicit_logging = True
 
-    async def connect(self) -> None:
-        ...
+    async def connect(self) -> None: ...
 
     async def properties(
         self, fresh: bool = False, config: UDSRequestConfig | None = None
     ) -> dict[str, Any]:
         return {}
 
     async def ping(
@@ -150,15 +149,15 @@
         except UnexpectedNegativeResponse as e:
             if suggests_identifier_not_supported(e.RESPONSE_CODE):
                 logger.info(
                     f"Read current session not supported: {e.RESPONSE_CODE.name}, skipping check_session"
                 )
                 return True
             raise e
-        except asyncio.TimeoutError:
+        except TimeoutError:
             logger.warning("Reading current session timed out, skipping check_session")
             return True
 
         logger.debug(f"Current session is {g_repr(current_session)}")
         if current_session == expected_session:
             return True
 
@@ -185,15 +184,15 @@
             except UnexpectedNegativeResponse as e:
                 if suggests_identifier_not_supported(e.RESPONSE_CODE):
                     logger.info(
                         f"Read current session not supported: {e.RESPONSE_CODE.name}, skipping check_session"
                     )
                     return True
                 raise e
-            except asyncio.TimeoutError:
+            except TimeoutError:
                 logger.warning("Reading current session timed out, skipping check_session")
                 return True
 
         logger.warning(
             f"Failed to switch to session {g_repr(expected_session)} after {retries} attempts"
         )
         return False
@@ -206,35 +205,39 @@
         async def callback() -> None:
             await self.wait_for_ecu()
 
         await self.power_supply.power_cycle(sleep, callback)
         self.state.reset()
         return True
 
-    async def leave_session(self, level: int, config: UDSRequestConfig | None = None) -> bool:
+    async def leave_session(
+        self,
+        level: int,
+        config: UDSRequestConfig | None = None,
+        sleep: int | None = None,
+    ) -> bool:
         """leave_session() is a hook which can be called explicitly by a
         scanner when a session is to be disabled. Use this hook if resetting
         the ECU is required, e.g. when disabling the programming session.
-
-        Args:
-            uds: The UDSClient class where this hook is embedded. The caller typically
-                 calls this function with `self` as the first argument.
-            session: The desired session identifier.
-        Returns:
-            True on success, False on error.
         """
         resp: service.UDSResponse = await self.ecu_reset(0x01)
         if isinstance(resp, service.NegativeResponse):
-            await self.power_cycle()
+            if sleep is not None:
+                await self.power_cycle(sleep=sleep)
+            else:
+                await self.power_cycle()
             await self.reconnect()
         await self.wait_for_ecu()
 
         resp = await self.set_session(0x01, config=config)
         if isinstance(resp, service.NegativeResponse):
-            await self.power_cycle()
+            if sleep is not None:
+                await self.power_cycle(sleep=sleep)
+            else:
+                await self.power_cycle()
             await self.reconnect()
         return True
 
     async def set_session(
         self,
         level: int,
         config: UDSRequestConfig | None = None,
@@ -335,15 +338,15 @@
         if self.tester_present_task and self.tester_present_interval:
             await self.stop_cyclic_tester_present()
 
         t = timeout if timeout is not None else self.timeout
         try:
             await asyncio.wait_for(self._wait_for_ecu(0.5), timeout=t)
             return True
-        except asyncio.TimeoutError:
+        except TimeoutError:
             logger.critical("Timeout while waiting for ECU!")
             return False
         finally:
             if self.tester_present_task and self.tester_present_interval:
                 await self.start_cyclic_tester_present(self.tester_present_interval)
 
     async def _tester_present_worker(self, interval: float) -> None:
```

### Comparing `gallia-1.6.0/src/gallia/services/uds/helpers.py` & `gallia-1.7.0/src/gallia/services/uds/helpers.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/services/uds/nrv.py` & `gallia-1.7.0/src/gallia/services/uds/nrv.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/services/uds/server.py` & `gallia-1.7.0/src/gallia/services/uds/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,15 @@
         self.use_default_response_if_none = True
         self.use_default_response_if_suppress = True
 
     @property
     @abstractmethod
     def supported_services(
         self,
-    ) -> dict[int, dict[UDSIsoServices, list[int] | None]]:
-        ...
+    ) -> dict[int, dict[UDSIsoServices, list[int] | None]]: ...
 
     def default_response_if_service_not_supported(
         self, request: service.UDSRequest
     ) -> service.NegativeResponse | None:
         assert self.state.session in self.supported_services, "Virtual ECU in unsupported session"
 
         if request.service_id not in self.supported_services[self.state.session]:
@@ -287,16 +286,15 @@
                 return self.default_response_if_suppress(request, response)
 
         return response
 
     @abstractmethod
     async def respond_after_default(
         self, request: service.UDSRequest
-    ) -> service.UDSResponse | None:
-        ...
+    ) -> service.UDSResponse | None: ...
 
 
 class RNG(random.Random):
     def __init__(self, *args: Any):
         super().__init__()
 
         self.seeds: list[Any] = []
@@ -754,16 +752,15 @@
 
 class UDSServerTransport:
     def __init__(self, server: UDSServer, target: TargetURI):
         self.server = server
         self.target = target
         self.last_time_active = time()
 
-    async def run(self) -> None:
-        ...
+    async def run(self) -> None: ...
 
     async def handle_request(self, request_pdu: bytes) -> tuple[bytes | None, float]:
         start = time()
 
         if start - self.last_time_active > 10:
             logger.info("Server state reset due to inactivity")
             self.server.state.reset()
```

### Comparing `gallia-1.6.0/src/gallia/services/xcp/__init__.py` & `gallia-1.7.0/src/gallia/services/xcp/__init__.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/services/xcp/types.py` & `gallia-1.7.0/src/gallia/services/xcp/types.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/transports/__init__.py` & `gallia-1.7.0/src/gallia/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/transports/base.py` & `gallia-1.7.0/src/gallia/transports/base.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/transports/can.py` & `gallia-1.7.0/src/gallia/transports/can.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,11 +215,11 @@
         t1 = time.time()
         while time.time() - t1 < sniff_time:
             try:
                 addr, _ = await self.recvfrom(timeout=1)
                 if addr not in addr_idle:
                     logger.info(f"Received a message from {addr:03x}")
                     addr_idle.append(addr)
-            except asyncio.TimeoutError:
+            except TimeoutError:
                 continue
         addr_idle.sort()
         return addr_idle
```

### Comparing `gallia-1.6.0/src/gallia/transports/doip.py` & `gallia-1.7.0/src/gallia/transports/doip.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import asyncio
+import socket
 import struct
 from dataclasses import dataclass
 from enum import IntEnum, unique
 from typing import Any
 
 from pydantic import BaseModel, field_validator
 
@@ -19,102 +20,131 @@
 logger = get_logger("gallia.transport.doip")
 
 
 @unique
 class ProtocolVersions(IntEnum):
     ISO_13400_2_2010 = 0x01
     ISO_13400_2_2012 = 0x02
+    ISO_13400_2_2019 = 0x03
 
 
 @unique
 class RoutingActivationRequestTypes(IntEnum):
+    RESERVED = 0xFF
+    ManufacturerSpecific = 0xFE
     Default = 0x00
     WWH_OBD = 0x01
     CentralSecurity = 0xE0
 
+    @classmethod
+    def _missing_(cls, value: Any) -> RoutingActivationRequestTypes:
+        if value in range(0xE1, 0x100):
+            return cls.ManufacturerSpecific
+        return cls.RESERVED
+
 
 @unique
 class RoutingActivationResponseCodes(IntEnum):
-    UNDEFINED = -0x01
+    RESERVED = 0xFF
+    ManufacturerSpecific = 0xFE
     UnknownSourceAddress = 0x00
     NoResources = 0x01
     InvalidConnectionEntry = 0x02
     AlreadyActive = 0x03
     AuthenticationMissing = 0x04
     ConfirmationRejected = 0x05
     UnsupportedActivationType = 0x06
+    TLSRequired = 0x07
     Success = 0x10
     SuccessConfirmationRequired = 0x11
 
     @classmethod
     def _missing_(cls, value: Any) -> RoutingActivationResponseCodes:
-        return cls.UNDEFINED
+        if value in range(0xE0, 0xFF):
+            return cls.ManufacturerSpecific
+        return cls.RESERVED
 
 
 class DoIPRoutingActivationDeniedError(ConnectionAbortedError):
     rac_code: RoutingActivationResponseCodes
 
     def __init__(self, rac_code: int):
         self.rac_code = RoutingActivationResponseCodes(rac_code)
         super().__init__(f"DoIP routing activation denied: {self.rac_code.name} ({rac_code})")
 
 
 @unique
 class PayloadTypes(IntEnum):
-    NegativeAcknowledge = 0x0000
-    VehicleIdentificationRequestMessage = 0x0002
-    VehicleIdentificationRequestMessageWithEID = 0x0003
-    VehicleIdentificationRequestMessageWithVIN = 0x0004
+    GenericDoIPHeaderNACK = 0x0000
+    VehicleIdentificationRequestMessage = 0x0001
+    VehicleIdentificationRequestMessageWithEID = 0x0002
+    VehicleIdentificationRequestMessageWithVIN = 0x0003
+    VehicleAnnouncementMessage = 0x004
     RoutingActivationRequest = 0x0005
     RoutingActivationResponse = 0x0006
     AliveCheckRequest = 0x0007
     AliveCheckResponse = 0x0008
     DoIPEntityStatusRequest = 0x4001
     DoIPEntityStatusResponse = 0x4002
+    DiagnosticPowerModeInformationRequest = 0x4003
+    DiagnosticPowerModeInformationResponse = 0x4004
     DiagnosticMessage = 0x8001
     DiagnosticMessagePositiveAcknowledgement = 0x8002
     DiagnosticMessageNegativeAcknowledgement = 0x8003
 
 
 @unique
 class DiagnosticMessagePositiveAckCodes(IntEnum):
     Success = 0x00
 
 
 @unique
 class DiagnosticMessageNegativeAckCodes(IntEnum):
-    UNDEFINED = -0x01
+    RESERVED = 0xFF
     InvalidSourceAddress = 0x02
     UnknownTargetAddress = 0x03
     DiagnosticMessageTooLarge = 0x04
     OutOfMemory = 0x05
     TargetUnreachable = 0x06
     UnknownNetwork = 0x07
     TransportProtocolError = 0x08
 
     @classmethod
     def _missing_(cls, value: Any) -> DiagnosticMessageNegativeAckCodes:
-        return cls.UNDEFINED
+        return cls.RESERVED
 
 
 class DoIPNegativeAckError(BrokenPipeError):
     nack_code: DiagnosticMessageNegativeAckCodes
 
     def __init__(self, negative_ack_code: int):
         self.nack_code = DiagnosticMessageNegativeAckCodes(negative_ack_code)
         super().__init__(f"DoIP negative ACK received: {self.nack_code.name} ({negative_ack_code})")
 
 
 @unique
-class GenericHeaderNACKCodes(IntEnum):
-    IncorrectPatternFormat = 0x01
-    UnknownPayloadType = 0x02
-    MessageTooLarge = 0x03
-    OutOfMemory = 0x04
-    InvalidPayloadLength = 0x05
+class GenericDoIPHeaderNACKCodes(IntEnum):
+    RESERVED = 0xFF
+    IncorrectPatternFormat = 0x00
+    UnknownPayloadType = 0x01
+    MessageTooLarge = 0x02
+    OutOfMemory = 0x03
+    InvalidPayloadLength = 0x04
+
+    @classmethod
+    def _missing_(cls, value: Any) -> GenericDoIPHeaderNACKCodes:
+        return cls.RESERVED
+
+
+class DoIPGenericHeaderNACKError(ConnectionAbortedError):
+    nack_code: GenericDoIPHeaderNACKCodes
+
+    def __init__(self, nack_code: int):
+        self.nack_code = GenericDoIPHeaderNACKCodes(nack_code)
+        super().__init__(f"DoIP generic header negative ACK: {self.nack_code.name} ({nack_code})")
 
 
 class TimingAndCommunicationParameters(IntEnum):
     CtrlTimeout = 2000
     AnnounceWait = 500
     AnnounceInterval = 500
     AnnounceNum = 3
@@ -157,16 +187,135 @@
             protocol_version,
             payload_type,
             payload_length,
         )
 
 
 @dataclass
-class GenericHeaderNegativeAcknowledge:
-    GenericHeaderNACKCode: GenericHeaderNACKCodes
+class GenericDoIPHeaderNACK:
+    GenericHeaderNACKCode: GenericDoIPHeaderNACKCodes
+
+    def pack(self) -> bytes:
+        return struct.pack(
+            "!B",
+            self.GenericHeaderNACKCode,
+        )
+
+    @classmethod
+    def unpack(cls, data: bytes) -> GenericDoIPHeaderNACK:
+        (generic_header_NACK_code,) = struct.unpack("!B", data)
+        return cls(
+            GenericDoIPHeaderNACKCodes(generic_header_NACK_code),
+        )
+
+
+@dataclass
+class VehicleIdentificationRequestMessage:
+    def pack(self) -> bytes:
+        return b""
+
+
+@dataclass
+class VehicleAnnouncementMessage:
+    VIN: bytes
+    LogicalAddress: int
+    EID: bytes
+    GID: bytes
+    FurtherActionRequired: FurtherActionCodes
+    VINGIDSyncStatus: SynchronisationStatusCodes | None
+
+    @classmethod
+    def unpack(cls, data: bytes) -> VehicleAnnouncementMessage:
+        if len(data) == 32:
+            # VINGIDSyncStatus is optional
+            (vin, logical_address, eid, gid, further_action_required) = struct.unpack(
+                "!17sH6s6sB", data
+            )
+            vin_gid_sync_status = None
+        else:
+            (
+                vin,
+                logical_address,
+                eid,
+                gid,
+                further_action_required,
+                vin_gid_sync_status,
+            ) = struct.unpack("!17sH6s6sBB", data)
+
+        return cls(
+            vin,
+            logical_address,
+            eid,
+            gid,
+            FurtherActionCodes(further_action_required),
+            SynchronisationStatusCodes(vin_gid_sync_status)
+            if vin_gid_sync_status is not None
+            else None,
+        )
+
+
+@unique
+class FurtherActionCodes(IntEnum):
+    RESERVED = 0x0F
+    ManufacturerSpecific = 0xFF
+    NoFurtherActionRequired = 0x00
+    RoutingActivationRequiredToInitiateCentralSecurity = 0x10
+
+    @classmethod
+    def _missing_(cls, value: Any) -> FurtherActionCodes:
+        if value in range(0x11, 0x100):
+            return cls.ManufacturerSpecific
+        return cls.RESERVED
+
+
+@unique
+class SynchronisationStatusCodes(IntEnum):
+    RESERVED = 0xFF
+    VINGIDSynchronized = 0x00
+    IncompleteVINGIDNotSynchronized = 0x10
+
+    @classmethod
+    def _missing_(cls, value: Any) -> SynchronisationStatusCodes:
+        return cls.RESERVED
+
+
+@dataclass
+class DoIPEntityStatusRequest:
+    def pack(self) -> bytes:
+        return b""
+
+
+@dataclass
+class DoIPEntityStatusResponse:
+    NodeType: NodeTypes
+    MaximumConcurrentTCP_DATASockets: int
+    CurrentlyOpenTCP_DATASockets: int
+    MaximumDataSize: int | None
+
+    @classmethod
+    def unpack(cls, data: bytes) -> DoIPEntityStatusResponse:
+        if len(data) == 3:
+            # MaximumDataSize is optional
+            (nt, mcts, ncts) = struct.unpack("!BBB", data)
+            mds = None
+        else:
+            (nt, mcts, ncts, mds) = struct.unpack("!BBBI", data)
+
+        return cls(NodeTypes(nt), mcts, ncts, mds)
+
+
+@unique
+class NodeTypes(IntEnum):
+    RESERVED = 0xFF
+    Gateway = 0x00
+    Node = 0x01
+
+    @classmethod
+    def _missing_(cls, value: Any) -> NodeTypes:
+        return cls.RESERVED
 
 
 @dataclass
 class RoutingActivationRequest:
     SourceAddress: int
     ActivationType: int
     Reserved: int = 0x00000000  # Not used, default value.
@@ -287,15 +436,16 @@
 
     def pack(self) -> bytes:
         return struct.pack("!H", self.SourceAddress)
 
 
 # Messages expected to be sent by the DoIP gateway.
 DoIPInData = (
-    RoutingActivationResponse
+    GenericDoIPHeaderNACK
+    | RoutingActivationResponse
     | DiagnosticMessage
     | DiagnosticMessagePositiveAcknowledgement
     | DiagnosticMessageNegativeAcknowledgement
     | AliveCheckRequest
 )
 
 # Messages expected to be sent by us.
@@ -305,79 +455,107 @@
     GenericHeader,
     DoIPInData | DoIPOutData,
 ]
 DoIPDiagFrame = tuple[GenericHeader, DiagnosticMessage]
 
 
 class DoIPConnection:
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         reader: asyncio.StreamReader,
         writer: asyncio.StreamWriter,
         src_addr: int,
         target_addr: int,
+        protocol_version: int,
     ):
         self.reader = reader
         self.writer = writer
         self.src_addr = src_addr
         self.target_addr = target_addr
+        self.protocol_version = protocol_version
         self._read_queue: asyncio.Queue[DoIPFrame] = asyncio.Queue()
         self._read_task = asyncio.create_task(self._read_worker())
         self._is_closed = False
         self._mutex = asyncio.Lock()
 
     @classmethod
-    async def connect(
+    async def connect(  # noqa: PLR0913
         cls,
         host: str,
         port: int,
         src_addr: int,
         target_addr: int,
+        so_linger: bool = False,
+        protocol_version: int = ProtocolVersions.ISO_13400_2_2019,
     ) -> DoIPConnection:
         reader, writer = await asyncio.open_connection(host, port)
-        return cls(reader, writer, src_addr, target_addr)
 
-    async def _read_frame(self) -> DoIPFrame:
+        if so_linger is True:
+            # Depending on who will close the connection in the end, one party's socket
+            # will remain in a TIME_WAIT state, which occupies resources until enough
+            # time has passed. Setting the LINGER socket option tells our kernel to
+            # close the connection with a RST, which brings the TCP connection to an
+            # error state and thus avoids TIME_WAIT and instantly forces LISTEN or CLOSED
+            # For more info, see e.g. Note 3 of :
+            # https://www.ietf.org/rfc/rfc9293.html#name-state-machine-overview
+            sock = writer.get_extra_info("socket")
+            sock.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER, struct.pack("ii", 1, 0))
+
+        return cls(reader, writer, src_addr, target_addr, protocol_version)
+
+    async def _read_frame(self) -> DoIPFrame | tuple[None, None]:
         # Header is fixed size 8 byte.
         hdr_buf = await self.reader.readexactly(8)
         hdr = GenericHeader.unpack(hdr_buf)
 
         payload_buf = await self.reader.readexactly(hdr.PayloadLength)
         payload: DoIPInData
         match hdr.PayloadType:
+            case PayloadTypes.GenericDoIPHeaderNACK:
+                payload = GenericDoIPHeaderNACK.unpack(payload_buf)
             case PayloadTypes.RoutingActivationResponse:
                 payload = RoutingActivationResponse.unpack(payload_buf)
             case PayloadTypes.DiagnosticMessagePositiveAcknowledgement:
                 payload = DiagnosticMessagePositiveAcknowledgement.unpack(payload_buf)
             case PayloadTypes.DiagnosticMessageNegativeAcknowledgement:
                 payload = DiagnosticMessageNegativeAcknowledgement.unpack(payload_buf)
             case PayloadTypes.DiagnosticMessage:
                 payload = DiagnosticMessage.unpack(payload_buf)
             case PayloadTypes.AliveCheckRequest:
                 payload = AliveCheckRequest()
             case _:
-                raise BrokenPipeError(f"unexpected DoIP message: {hdr} {payload_buf.hex()}")
+                logger.warning(
+                    f"DoIP message with unhandled PayloadType: {hdr} {payload_buf.hex()}"
+                )
+                return None, None
+        logger.trace("Received DoIP message: %s, %s", hdr, payload)
         return hdr, payload
 
     async def _read_worker(self) -> None:
         try:
             while True:
                 hdr, data = await self._read_frame()
+                if hdr is None or data is None:
+                    continue
                 if hdr.PayloadType == PayloadTypes.DiagnosticMessage and isinstance(
                     data, AliveCheckRequest
                 ):
                     await self.write_alive_check_response()
                     continue
                 await self._read_queue.put((hdr, data))
         except asyncio.CancelledError:
             logger.debug("read worker cancelled")
         except asyncio.IncompleteReadError as e:
             logger.debug(f"read worker received EOF: {e}")
         except Exception as e:
             logger.critical(f"read worker died with {type(e)}: {e}")
+        finally:
+            logger.debug("Feeding EOF to reader and requesting a close")
+            self.reader.feed_eof()
+            await self.close()
 
     async def read_frame_unsafe(self) -> DoIPFrame:
         # Avoid waiting on the queue forever when
         # the connection has been terminated.
         if self._is_closed:
             raise ConnectionError()
         return await self._read_queue.get()
@@ -428,15 +606,16 @@
                     f"DoIP-ACK: unexpected addresses (src:dst); expected {self.src_addr:#04x}:{self.target_addr:#04x} "
                     + f"but got: {payload.SourceAddress:#04x}:{payload.TargetAddress:#04x}"
                 )
                 unexpected_packets.append((hdr, payload))
                 continue
             if (
                 len(payload.PreviousDiagnosticMessageData) > 0
-                and prev_data != payload.PreviousDiagnosticMessageData
+                and payload.PreviousDiagnosticMessageData
+                != prev_data[: len(payload.PreviousDiagnosticMessageData)]
             ):
                 logger.warning("ack: previous data differs from request")
                 logger.warning(
                     f"DoIP-ACK: got: {payload.PreviousDiagnosticMessageData.hex()} expected {prev_data.hex()}"
                 )
                 unexpected_packets.append((hdr, payload))
                 continue
@@ -472,15 +651,15 @@
         async with self._mutex:
             buf = b""
             buf += hdr.pack()
             buf += payload.pack()
             self.writer.write(buf)
             await self.writer.drain()
 
-            logger.trace(f"hdr: {hdr}, payload: {payload}")
+            logger.trace("Sent DoIP message: hdr: %s, payload: %s", hdr, payload)
 
             try:
                 match payload:
                     case DiagnosticMessage():
                         # Now an ACK message is expected.
                         await asyncio.wait_for(
                             self._read_ack(payload.UserData),
@@ -489,21 +668,21 @@
                         )
                     case RoutingActivationRequest():
                         await asyncio.wait_for(
                             self._read_routing_activation_response(),
                             TimingAndCommunicationParameters.RoutingActivationResponseTimeout
                             / 1000,
                         )
-            except asyncio.TimeoutError as e:
+            except TimeoutError as e:
                 await self.close()
                 raise BrokenPipeError("Timeout while waiting for DoIP ACK message") from e
 
     async def write_diag_request(self, data: bytes) -> None:
         hdr = GenericHeader(
-            ProtocolVersion=ProtocolVersions.ISO_13400_2_2012,
+            ProtocolVersion=self.protocol_version,
             PayloadType=PayloadTypes.DiagnosticMessage,
             PayloadLength=len(data) + 4,
         )
         payload = DiagnosticMessage(
             SourceAddress=self.src_addr,
             TargetAddress=self.target_addr,
             UserData=data,
@@ -511,54 +690,60 @@
         await self.write_request_raw(hdr, payload)
 
     async def write_routing_activation_request(
         self,
         activation_type: int,
     ) -> None:
         hdr = GenericHeader(
-            ProtocolVersion=ProtocolVersions.ISO_13400_2_2012,
+            ProtocolVersion=self.protocol_version,
             PayloadType=PayloadTypes.RoutingActivationRequest,
             PayloadLength=7,
         )
         payload = RoutingActivationRequest(
             SourceAddress=self.src_addr,
             ActivationType=activation_type,
             Reserved=0x00,
         )
         await self.write_request_raw(hdr, payload)
 
     async def write_alive_check_response(self) -> None:
         hdr = GenericHeader(
-            ProtocolVersion=ProtocolVersions.ISO_13400_2_2012,
+            ProtocolVersion=self.protocol_version,
             PayloadType=PayloadTypes.AliveCheckResponse,
             PayloadLength=2,
         )
         payload = AliveCheckResponse(
             SourceAddress=self.src_addr,
         )
         await self.write_request_raw(hdr, payload)
 
     async def close(self) -> None:
+        logger.debug("Closing DoIP connection...")
         if self._is_closed:
+            logger.debug("Already closed!")
             return
         self._is_closed = True
+        logger.debug("Cancelling read worker")
         self._read_task.cancel()
         self.writer.close()
+        logger.debug("Awaiting confirmation of closed writer")
         await self.writer.wait_closed()
 
 
 class DoIPConfig(BaseModel):
     src_addr: int
     target_addr: int
     activation_type: int = RoutingActivationRequestTypes.WWH_OBD.value
+    protocol_version: int = ProtocolVersions.ISO_13400_2_2019
 
     @field_validator(
         "src_addr",
         "target_addr",
         "activation_type",
+        "protocol_version",
         mode="before",
     )
     def auto_int(cls, v: str) -> int:
         return auto_int(v)
 
 
 class DoIPTransport(BaseTransport, scheme="doip"):
@@ -572,26 +757,28 @@
         super().__init__(target)
         self.port = port
         self.config = config
         self._conn = conn
         self._is_closed = False
 
     @staticmethod
-    async def _connect(
+    async def _connect(  # noqa: PLR0913
         hostname: str,
         port: int,
         src_addr: int,
         target_addr: int,
         activation_type: int,
+        protocol_version: int,
     ) -> DoIPConnection:
         conn = await DoIPConnection.connect(
             hostname,
             port,
             src_addr,
             target_addr,
+            protocol_version=protocol_version,
         )
         await conn.write_routing_activation_request(RoutingActivationRequestTypes(activation_type))
         return conn
 
     @classmethod
     async def connect(
         cls,
@@ -609,14 +796,15 @@
         conn = await asyncio.wait_for(
             cls._connect(
                 t.hostname,
                 port,
                 config.src_addr,
                 config.target_addr,
                 config.activation_type,
+                config.protocol_version,
             ),
             timeout,
         )
         return cls(t, port, config, conn)
 
     async def close(self) -> None:
         if self._is_closed:
```

### Comparing `gallia-1.6.0/src/gallia/transports/isotp.py` & `gallia-1.7.0/src/gallia/transports/isotp.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/transports/tcp.py` & `gallia-1.7.0/src/gallia/transports/tcp.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/transports/unix.py` & `gallia-1.7.0/src/gallia/transports/unix.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/gallia/utils.py` & `gallia-1.7.0/src/gallia/utils.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/hr/__init__.py` & `gallia-1.7.0/src/hr/__init__.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/opennetzteil/cli.py` & `gallia-1.7.0/src/opennetzteil/cli.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/opennetzteil/devices/http/client.py` & `gallia-1.7.0/src/opennetzteil/devices/http/client.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/opennetzteil/devices/rs/hmc804.py` & `gallia-1.7.0/src/opennetzteil/devices/rs/hmc804.py`

 * *Files identical despite different names*

### Comparing `gallia-1.6.0/src/opennetzteil/netzteil.py` & `gallia-1.7.0/src/opennetzteil/netzteil.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,15 @@
         """Checks for connectivity. The default implementation
         reads out the version number and model string by calling
         :meth:`get_ident()`.
         """
         self.ident = await self.get_ident()
 
     @abstractmethod
-    async def status(self) -> dict[str, Any]:
-        ...
+    async def status(self) -> dict[str, Any]: ...
 
     @abstractmethod
     async def get_ident(self) -> str:
         """Reads the version number and model string."""
 
     @abstractmethod
     async def get_master(self) -> bool:
```

### Comparing `gallia-1.6.0/PKG-INFO` & `gallia-1.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gallia
-Version: 1.6.0
+Version: 1.7.0
 Summary: Extendable Pentesting Framework
 Home-page: https://github.com/Fraunhofer-AISEC/gallia
 License: Apache-2.0
 Keywords: pentesting,automotive,uds
 Author: AISEC Pentesting Team
 Maintainer: Stefan Tatschner
 Maintainer-email: stefan.tatschner@aisec.fraunhofer.de
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=22.1,<24.0)
 Requires-Dist: aiosqlite (>=0.18)
 Requires-Dist: argcomplete (>=2,<4)
 Requires-Dist: construct (>=2.10,<3.0)
 Requires-Dist: exitcode (>=0.1.0,<0.2.0)
-Requires-Dist: httpx[http2] (>=0.26.0,<0.27.0)
+Requires-Dist: httpx[http2] (>=0.26,<0.28)
 Requires-Dist: msgspec (>=0.11,<0.19)
 Requires-Dist: platformdirs (>=2.6,<5.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pygit2 (>=1.10,<2.0)
 Requires-Dist: python-can (>=4.2,<5.0)
 Requires-Dist: tabulate (>=0.9)
@@ -43,14 +43,15 @@
 # Gallia
 
 [![docs](https://img.shields.io/badge/-docs-green)](https://fraunhofer-aisec.github.io/gallia)
 [![docs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://gallia.readthedocs.io/en/latest)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gallia)](https://pypi.python.org/pypi/gallia/)
 [![PyPI - License](https://img.shields.io/pypi/l/gallia)](https://www.apache.org/licenses/LICENSE-2.0.html)
 [![PyPI](https://img.shields.io/pypi/v/gallia)](https://pypi.python.org/pypi/gallia/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10696368.svg)](https://zenodo.org/doi/10.5281/zenodo.10696368)
 
 [![Packaging status](https://repology.org/badge/vertical-allrepos/gallia.svg)](https://repology.org/project/gallia/versions)
 
 Gallia is an extendable pentesting framework with the focus on the automotive domain.
 The scope of the toolchain is conducting penetration tests from a single ECU up to whole cars.
 Currently, the main focus lies on the [UDS](https://www.iso.org/standard/72439.html) interface.
 Acting as a generic interface, the logging functionality implements reproducible tests and enables post-processing tasks.
```

