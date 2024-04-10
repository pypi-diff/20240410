# Comparing `tmp/musify-0.8.1.tar.gz` & `tmp/musify-0.9.0.tar.gz`

## Comparing `musify-0.8.1.tar` & `musify-0.9.0.tar`

### file list

```diff
@@ -1,89 +1,97 @@
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 musify-0.8.1/musify/__init__.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 musify-0.8.1/musify/report.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/base.py
--rw-r--r--   0        0        0    22168 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/collection.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/exception.py
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/file.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/library/__init__.py
--rw-r--r--   0        0        0    18144 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/library/library.py
--rw-r--r--   0        0        0    24520 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/library/musicbee.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/playlist/__init__.py
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/playlist/base.py
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/playlist/m3u.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/playlist/utils.py
--rw-r--r--   0        0        0     8894 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/playlist/xautopf.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/__init__.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/field.py
--rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/flac.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/m4a.py
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/mp3.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/utils.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/wma.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/base/__init__.py
--rw-r--r--   0        0        0    18665 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/base/reader.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/base/track.py
--rw-r--r--   0        0        0    18687 2020-02-02 00:00:00.000000 musify-0.8.1/musify/local/track/base/writer.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/__init__.py
--rw-r--r--   0        0        0     9626 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/base.py
--rw-r--r--   0        0        0    13327 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/compare.py
--rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/download.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/exception.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/filter.py
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/filter_matcher.py
--rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/limit.py
--rw-r--r--   0        0        0    21355 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/match.py
--rw-r--r--   0        0        0     9419 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/sort.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 musify-0.8.1/musify/processors/time.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/__init__.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/exception.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/field.py
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/handlers.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/logger.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/types.py
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/utils.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/api/__init__.py
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/api/authorise.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/api/exception.py
--rw-r--r--   0        0        0     9916 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/api/request.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/core/__init__.py
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/core/base.py
--rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/core/collection.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/core/enum.py
--rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/core/misc.py
--rw-r--r--   0        0        0    23655 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/core/object.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/_base.py
--rw-r--r--   0        0        0    18232 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/api.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/base.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/config.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/enum.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/exception.py
--rw-r--r--   0        0        0    21558 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/library.py
--rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/object.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/types.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/processors/__init__.py
--rw-r--r--   0        0        0    21720 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/processors/check.py
--rw-r--r--   0        0        0    13240 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/processors/search.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 musify-0.8.1/musify/shared/remote/processors/wrangle.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/__init__.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/_base.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/base.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/config.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/exception.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/library.py
--rw-r--r--   0        0        0    26146 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/object.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/api/__init__.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/api/api.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/api/base.py
--rw-r--r--   0        0        0    27452 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/api/item.py
--rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/api/misc.py
--rw-r--r--   0        0        0     9672 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/api/playlist.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/processors/__init__.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/processors/processors.py
--rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 musify-0.8.1/musify/spotify/processors/wrangle.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 musify-0.8.1/.gitignore
--rw-r--r--   0        0        0    35184 2020-02-02 00:00:00.000000 musify-0.8.1/LICENSE
--rw-r--r--   0        0        0    14786 2020-02-02 00:00:00.000000 musify-0.8.1/README.md
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 musify-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    17005 2020-02-02 00:00:00.000000 musify-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 musify-0.9.0/musify/__init__.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 musify-0.9.0/musify/exception.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 musify-0.9.0/musify/field.py
+-rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 musify-0.9.0/musify/report.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 musify-0.9.0/musify/types.py
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 musify-0.9.0/musify/utils.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 musify-0.9.0/musify/api/__init__.py
+-rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 musify-0.9.0/musify/api/authorise.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 musify-0.9.0/musify/api/exception.py
+-rw-r--r--   0        0        0    10229 2020-02-02 00:00:00.000000 musify-0.9.0/musify/api/request.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/base.py
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/enum.py
+-rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/printer.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/result.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/__init__.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/base.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/exception.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/image.py
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/path_mapper.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/__init__.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/collection.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/core/__init__.py
+-rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/core/collection.py
+-rw-r--r--   0        0        0    23292 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/core/object.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/__init__.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/base.py
+-rw-r--r--   0        0        0    19985 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/collection.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/exception.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/library/__init__.py
+-rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/library/library.py
+-rw-r--r--   0        0        0    24639 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/library/musicbee.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/__init__.py
+-rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/base.py
+-rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/m3u.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/utils.py
+-rw-r--r--   0        0        0    28389 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/xautopf.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/__init__.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/field.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/flac.py
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/m4a.py
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/mp3.py
+-rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/track.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/utils.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/wma.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/tags/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/tags/base.py
+-rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/tags/reader.py
+-rw-r--r--   0        0        0    32439 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/tags/writer.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/__init__.py
+-rw-r--r--   0        0        0    21411 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/api.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/base.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/enum.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/exception.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/factory.py
+-rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/library.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/object.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/response.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/types.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/processors/__init__.py
+-rw-r--r--   0        0        0    23087 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/processors/check.py
+-rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/processors/search.py
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/processors/wrangle.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/base.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/exception.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/factory.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/library.py
+-rw-r--r--   0        0        0    31359 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/object.py
+-rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/processors.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/__init__.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/api.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/base.py
+-rw-r--r--   0        0        0    29516 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/item.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/misc.py
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/playlist.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 musify-0.9.0/musify/log/__init__.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 musify-0.9.0/musify/log/filter.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 musify-0.9.0/musify/log/handlers.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 musify-0.9.0/musify/log/logger.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/__init__.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/base.py
+-rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/compare.py
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/download.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/exception.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/filter.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/filter_matcher.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/limit.py
+-rw-r--r--   0        0        0    21695 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/match.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/sort.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/time.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 musify-0.9.0/.gitignore
+-rw-r--r--   0        0        0    35184 2020-02-02 00:00:00.000000 musify-0.9.0/LICENSE
+-rw-r--r--   0        0        0    15052 2020-02-02 00:00:00.000000 musify-0.9.0/README.md
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 musify-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    17340 2020-02-02 00:00:00.000000 musify-0.9.0/PKG-INFO
```

### Comparing `musify-0.8.1/musify/report.py` & `musify-0.9.0/musify/report.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
 Meta-functions for providing reports to the user based on comparisons between objects implemented in this package.
 """
-
 import logging
 from collections.abc import Iterable
 
-from musify.local.library import LocalLibrary
-from musify.shared.core.base import Item
-from musify.shared.core.collection import ItemCollection
-from musify.shared.core.enum import TagField, Fields, ALL_FIELDS, TagFields
-from musify.shared.core.object import Library, Playlist
-from musify.shared.logger import MusifyLogger, REPORT
-from musify.shared.types import UnitIterable
-from musify.shared.utils import align_string, get_max_width, to_collection
+from musify.core.base import MusifyItem
+from musify.core.enum import TagField, Fields, ALL_FIELDS, TagFields
+from musify.libraries.core.collection import MusifyCollection
+from musify.libraries.core.object import Library, Playlist
+from musify.libraries.local.library import LocalLibrary
+from musify.log import REPORT
+from musify.log.logger import MusifyLogger
+from musify.types import UnitIterable
+from musify.utils import align_string, get_max_width, to_collection
 
 
 def report_playlist_differences(
         source: Library | Iterable[Playlist], reference: Library | Iterable[Playlist]
-) -> dict[str, dict[str, tuple[Item, ...]]]:
+) -> dict[str, dict[str, tuple[MusifyItem, ...]]]:
     """
     Generate a report on the differences between two library's playlists.
 
     :param source: A source library object containing the source playlists, or a collection of playlists .
     :param reference: A comparative library object or collection of playlists
         containing the playlists to compare to the source's playlists.
     :return: Report on extra, missing, and unavailable tracks for the reference library.
     """
     # noinspection PyTypeChecker
     logger: MusifyLogger = logging.getLogger(__name__)
     logger.debug("Report library differences: START")
 
-    extra: dict[str, tuple[Item, ...]] = {}
-    missing: dict[str, tuple[Item, ...]] = {}
-    unavailable: dict[str, tuple[Item, ...]] = {}
+    extra: dict[str, tuple[MusifyItem, ...]] = {}
+    missing: dict[str, tuple[MusifyItem, ...]] = {}
+    unavailable: dict[str, tuple[MusifyItem, ...]] = {}
 
     source = source.playlists if isinstance(source, Library) else {pl.name: pl for pl in source}
     reference = reference.playlists if isinstance(reference, Library) else {pl.name: pl for pl in reference}
     max_width = get_max_width(source.keys())
 
     logger.info("\33[1;95m ->\33[1;97m Reporting on differences between libraries \33[0m")
     logger.print()
@@ -57,15 +57,15 @@
             f"\33[97m{align_string(name, max_width=max_width)} \33[0m|"
             f"\33[92m{len(reference_extra):>6} extra \33[0m|"
             f"\33[91m{len(source_extra):>6} missing \33[0m|"
             f"\33[93m{len(source_no_uri) + len(reference_no_uri):>6} unavailable \33[0m|"
             f"\33[94m{len(pl_source):>6} in source \33[0m"
         )
 
-    report: dict[str, dict[str, tuple[Item, ...]]] = {
+    report: dict[str, dict[str, tuple[MusifyItem, ...]]] = {
         "Source ✗ | Compare ✓": extra,
         "Source ✓ | Compare ✗": missing,
         "Items unavailable (no URI)": unavailable
     }
 
     logger.report(
         f"\33[1;96m{'TOTALS':<{max_width}} \33[0m|"
@@ -76,56 +76,41 @@
     )
     logger.print(REPORT)
     logger.debug("Report library differences: DONE\n")
     return report
 
 
 def report_missing_tags(
-        collections: LocalLibrary | Iterable[ItemCollection],
+        collections: LocalLibrary | Iterable[MusifyCollection],
         tags: UnitIterable[TagField] = TagFields.ALL,
         match_all: bool = False
-) -> dict[str, dict[Item, tuple[str, ...]]]:
+) -> dict[str, dict[MusifyItem, tuple[str, ...]]]:
     """
     Generate a report on the items with a set of collections that have missing tags.
 
     :param collections: A collection of item collections to report on.
         If a local library is given, use the albums of the library as the collections to report on.
     :param tags: List of tags to consider missing.
     :param match_all: When True, item counts as missing tags if item is missing ``all`` of the given tags.
         When False, item counts as missing tags when missing only one of the given tags.
     :return: Report on collections by name which have items with missing tags.
     """
     # noinspection PyTypeChecker
     logger: MusifyLogger = logging.getLogger(__name__)
     logger.debug("Report missing tags: START")
 
-    tags = to_collection(tags, set)
-    tag_order = [field.name.lower() for field in ALL_FIELDS]
-    # noinspection PyTypeChecker
-    tag_names = set(TagField.__tags__) if Fields.ALL in tags else TagField.to_tags(tags)
-    tag_names: list[str] = list(sorted(tag_names, key=lambda x: tag_order.index(x)))
-
     if isinstance(collections, LocalLibrary):
         collections = collections.albums
-    items_total = sum(len(collection) for collection in collections)
 
-    logger.info(
-        f"\33[1;95m ->\33[1;97m "
-        f"Checking {items_total} items for {'all' if match_all else 'any'} missing tags: \n"
-        f"    \33[90m{', '.join(tag_names)}\33[0m"
-    )
-
-    if Fields.URI in tags or Fields.ALL in tags:
-        tag_names[tag_names.index(Fields.URI.name.lower())] = "has_uri"
-    if Fields.IMAGES in tags or Fields.ALL in tags:
-        tag_names[tag_names.index(Fields.IMAGES.name.lower())] = "has_image"
+    item_total = sum(len(collection) for collection in collections)
+    tag_names = _get_tag_names(logger=logger, tags=tags, item_total=item_total, match_all=match_all)
 
-    missing: dict[str, dict[Item, tuple[str, ...]]] = {}
+    missing: dict[str, dict[MusifyItem, tuple[str, ...]]] = {}
     for collection in collections:
-        missing_collection: dict[Item, tuple[str, ...]] = {}
+        missing_collection: dict[MusifyItem, tuple[str, ...]] = {}
         for item in collection.items:
             missing_tags: list[str] = [tag for tag in tag_names if item[tag] is None]
             if "has_uri" in missing_tags:
                 missing_tags[missing_tags.index("has_uri")] = Fields.URI.name.lower()
             if "has_image" in missing_tags:
                 missing_tags[missing_tags.index("has_image")] = Fields.IMAGES.name.lower()
             if all(tag in missing_tags for tag in tag_names) if match_all else missing_tags:
@@ -134,30 +119,57 @@
         if missing_collection:
             missing[collection.name] = missing_collection
 
     if not missing:
         logger.debug("Report missing tags: DONE\n")
         return missing
 
+    _log_missing_tags(logger=logger, missing=missing)
+
+    missing_tags_all = {tag for items in missing.values() for tags in items.values() for tag in tags}
+    tag_order = [field.name.lower() for field in ALL_FIELDS]
+    logger.info(
+        f"    \33[94mFound {len({item for items in missing.values() for item in items})} items with "
+        f"{'all' if match_all else 'any'} missing tags\33[0m: \n"
+        f"    \33[90m{', '.join(sorted(missing_tags_all, key=lambda x: tag_order.index(x)))}\33[0m"
+    )
+    logger.print()
+    logger.debug("Report missing tags: DONE\n")
+    return missing
+
+
+def _get_tag_names(logger: MusifyLogger, tags: UnitIterable[TagField], item_total: int, match_all: bool) -> list[str]:
+    tags = to_collection(tags, set)
+    tag_order = [field.name.lower() for field in ALL_FIELDS]
+    # noinspection PyTypeChecker
+    tag_names_set = set(TagField.__tags__) if Fields.ALL in tags else TagField.to_tags(tags)
+    tag_names: list[str] = list(sorted(tag_names_set, key=lambda x: tag_order.index(x)))
+
+    logger.info(
+        f"\33[1;95m ->\33[1;97m "
+        f"Checking {item_total} items for {'all' if match_all else 'any'} missing tags: \n"
+        f"    \33[90m{', '.join(tag_names)}\33[0m"
+    )
+
+    # switch out tag names with expected attribute names to check on
+    if Fields.URI in tags or Fields.ALL in tags:
+        tag_names[tag_names.index(Fields.URI.name.lower())] = "has_uri"
+    if Fields.IMAGES in tags or Fields.ALL in tags:
+        tag_names[tag_names.index(Fields.IMAGES.name.lower())] = "has_image"
+
+    return tag_names
+
+
+def _log_missing_tags(logger: MusifyLogger, missing: dict[str, dict[MusifyItem, tuple[str, ...]]]) -> None:
     all_keys = {item.name for items in missing.values() for item in items}
     max_width = get_max_width(all_keys)
 
-    # log the report
     logger.print(REPORT)
     logger.report("\33[1;94mFound the following missing items by collection: \33[0m")
     logger.print(REPORT)
+
     for name, result in missing.items():
         logger.report(f"\33[1;91m -> {name} \33[0m")
         for item, tags in result.items():
             n = align_string(item.name, max_width=max_width)
             logger.report(f"\33[96m{n} \33[0m| \33[93m{', '.join(tags)} \33[0m")
         logger.print(REPORT)
-
-    missing_tags_all = {tag for items in missing.values() for tags in items.values() for tag in tags}
-    logger.info(
-        f"    \33[94mFound {len(all_keys)} items with "
-        f"{'all' if match_all else 'any'} missing tags\33[0m: \n"
-        f"    \33[90m{', '.join(sorted(missing_tags_all, key=lambda x: tag_order.index(x)))}\33[0m"
-    )
-    logger.print()
-    logger.debug("Report missing tags: DONE\n")
-    return missing
```

### Comparing `musify-0.8.1/musify/local/collection.py` & `musify-0.9.0/musify/libraries/local/collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 """
 Implements all collection types for a local library.
 """
-
 from __future__ import annotations
 
 import logging
 import sys
 from abc import ABCMeta, abstractmethod
 from collections.abc import Mapping, Collection, Iterable, Container
+from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from glob import glob
 from os.path import splitext, join, basename, exists, isdir
 from typing import Any
 
-from musify.local.base import LocalItem
-from musify.local.exception import LocalCollectionError
-from musify.local.track import LocalTrack, SyncResultTrack, load_track, TRACK_FILETYPES
-from musify.local.track.field import LocalTrackField
-from musify.shared.core.base import Item
-from musify.shared.core.collection import ItemCollection
-from musify.shared.core.enum import Fields, TagField, TagFields
-from musify.shared.core.object import Track, Library, Folder, Album, Artist, Genre
-from musify.shared.exception import MusifyKeyError
-from musify.shared.logger import MusifyLogger
-from musify.shared.remote.enum import RemoteIDType
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
-from musify.shared.types import UnitCollection
-from musify.shared.types import UnitIterable
-from musify.shared.utils import get_most_common_values, to_collection, align_string, get_max_width
+from musify.core.enum import Fields, TagField, TagFields
+from musify.libraries.core.collection import MusifyCollection
+from musify.libraries.core.object import Track, Library, Folder, Album, Artist, Genre
+from musify.libraries.local.base import LocalItem
+from musify.libraries.local.exception import LocalCollectionError
+from musify.libraries.local.track import LocalTrack, SyncResultTrack, load_track, TRACK_FILETYPES
+from musify.libraries.local.track.field import LocalTrackField
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
+from musify.log.logger import MusifyLogger
+from musify.types import UnitCollection, UnitIterable
+from musify.utils import get_most_common_values, to_collection, align_string, get_max_width
 
 _max_str = "z" * 50
 
 
-class LocalCollection[T: LocalTrack](ItemCollection[T], metaclass=ABCMeta):
+class LocalCollection[T: LocalTrack](MusifyCollection[T], metaclass=ABCMeta):
     """
     Generic class for storing a collection of local tracks.
 
     :param remote_wrangler: Optionally, provide a RemoteDataWrangler object for processing URIs on items.
         If given, the wrangler can be used when calling __get_item__ to get an item from the collection from its URI.
     """
 
@@ -57,36 +53,19 @@
     @property
     @abstractmethod
     def tracks(self) -> list[T]:
         """The tracks in this collection"""
         raise NotImplementedError
 
     @property
-    def artists(self) -> list[str]:
-        """List of artists ordered by frequency of appearance on the tracks in this collection"""
-        return get_most_common_values(track.artist for track in self.tracks if track.artist)
-
-    @property
     def track_total(self) -> int:
         """The total number of tracks in this collection"""
         return len(self)
 
     @property
-    def genres(self) -> list[str]:
-        """List of genres ordered by frequency of appearance on the tracks in this collection"""
-        genres = (genre for track in self.tracks for genre in (track.genres if track.genres else []))
-        return get_most_common_values(genres)
-
-    @property
-    def length(self) -> float | None:
-        """Total duration of all tracks in this collection in seconds"""
-        lengths = {track.length for track in self.tracks}
-        return sum(lengths) if lengths else None
-
-    @property
     def last_modified(self) -> datetime:
         """Timestamp of the last modified track in this collection"""
         sort = sorted(filter(lambda t: t.date_modified, self.tracks), key=lambda t: t.date_modified, reverse=True)
         # None condition will only be returned when using dummy tracks in tests therefore not included in typing
         return sort[0].date_modified if sort else None
 
     @property
@@ -102,47 +81,45 @@
         return sort[0].last_played if sort else None
 
     @property
     def play_count(self) -> int:
         """Total number of plays of all tracks in this collection"""
         return sum(track.play_count for track in self.tracks if track.play_count)
 
-    @property
-    def track_paths(self) -> set[str]:
-        """Set of all unique track paths in this collection"""
-        return {track.path for track in self.tracks}
-
     def __init__(self, remote_wrangler: RemoteDataWrangler = None):
-        super().__init__()
+        super().__init__(remote_wrangler=remote_wrangler)
 
         # noinspection PyTypeChecker
         #: The :py:class:`MusifyLogger` for this  object
         self.logger: MusifyLogger = logging.getLogger(__name__)
-        #: A :py:class:`RemoteDataWrangler` object for processing URIs
-        self.remote_wrangler = remote_wrangler
 
     def save_tracks(
             self,
             tags: UnitIterable[LocalTrackField] = LocalTrackField.ALL,
             replace: bool = False,
             dry_run: bool = True
     ) -> dict[LocalTrack, SyncResultTrack]:
         """
         Saves the tags of all tracks in this collection. Use arguments from :py:func:`LocalTrack.save`
 
         :param tags: Tags to be updated.
         :param replace: Destructively replace tags in each file.
-        :param dry_run: Run function, but do not modify file at all.
+        :param dry_run: Run function, but do not modify the file on the disk.
         :return: A map of the :py:class:`LocalTrack` saved to its result as a :py:class:`SyncResultTrack` object
         """
-        bar = self.logger.get_progress_bar(iterable=self.tracks, desc="Updating tracks", unit="tracks")
-        results = {track: track.save(tags=tags, replace=replace, dry_run=dry_run) for track in bar}
-        return {track: result for track, result in results.items() if result.updated}
+        with ThreadPoolExecutor(thread_name_prefix="track-saver") as executor:
+            futures = {
+                track: executor.submit(track.save, tags=tags, replace=replace, dry_run=dry_run)
+                for track in self.tracks
+            }
+            bar = self.logger.get_progress_bar(futures.items(), desc="Updating tracks", unit="tracks")
+
+            return {track: future.result() for track, future in bar if future.result().updated}
 
-    def log_sync_result(self, results: Mapping[LocalTrack, SyncResultTrack]) -> None:
+    def log_save_tracks_result(self, results: Mapping[LocalTrack, SyncResultTrack]) -> None:
         """Log stats from the results of a ``save_tracks`` operation"""
         if not results:
             return
 
         max_width = get_max_width([track.path for track in results], max_width=80)
 
         self.logger.stat("\33[1;96mSaved tags to the following tracks: \33[0m")
@@ -154,15 +131,15 @@
             )
 
     def merge_tracks(self, tracks: Collection[Track], tags: UnitIterable[TagField] = Fields.ALL) -> None:
         """
         Merge this collection with another collection or list of items
         by performing an inner join on a given set of tags
 
-        :param tracks: List of items or ItemCollection to merge with
+        :param tracks: List of items or :py:class:`MusifyCollection` to merge with
         :param tags: List of tags to merge on.
         """
         # noinspection PyTypeChecker
         tag_names = set(TagField.__tags__) if tags == Fields.ALL else set(TagField.to_tags(tags))
         tag_order = [tag for field in TagFields.all(only_tags=True) for tag in field.to_tag()]
         tag_names = sorted(tag_names, key=lambda x: tag_order.index(x))
 
@@ -186,47 +163,14 @@
             for tag in tag_names:  # merge on each tag
                 if hasattr(track, tag):
                     track_in_collection[tag] = track[tag]
 
         if isinstance(self, Library):
             self.logger.print()
 
-    def __getitem__(self, __key: str | int | slice | Item) -> T | list[T] | list[T, None, None]:
-        """
-        Returns the item in this collection by matching on a given path/index/URI.
-        If an item is given, the URI or path is extracted from this item
-        and the matching Item from this collection is returned.
-        """
-        if isinstance(__key, int) or isinstance(__key, slice):  # simply index the list or items
-            return self.items[__key]
-        elif isinstance(__key, LocalTrack):  # take the path
-            __key = __key.path
-        elif isinstance(__key, Item):  # take the URI
-            if not __key.has_uri:
-                raise MusifyKeyError(f"Given item does not have a URI associated to use as a key: {__key.name}")
-            __key = __key.uri
-
-        if self.remote_wrangler is None or not self.remote_wrangler.validate_id_type(__key, kind=RemoteIDType.URI):
-            # string is not a URI, assume it is a path or name
-            if __key in self.track_paths:  # path is valid
-                try:
-                    return next(track for track in self.tracks if track.path == __key)
-                except StopIteration:
-                    raise MusifyKeyError(f"No matching item found for path: '{__key}'")
-
-            try:  # last try, assume given string is a name
-                return next(item for item in self.items if item.name == __key)
-            except StopIteration:
-                raise MusifyKeyError(f"No matching item found for name/path: '{__key}'")
-
-        try:  # string is a URI
-            return next(item for item in self.items if item.uri == __key)
-        except StopIteration:
-            raise MusifyKeyError(f"No matching item found for URI: '{__key}'")
-
 
 class LocalCollectionFiltered[T: LocalItem](LocalCollection[T], metaclass=ABCMeta):
     """
     Generic class for storing and filtering on a collection of local tracks
     with methods for enriching the attributes of this object from the attributes of the collection of tracks
 
     :param tracks: A list of loaded tracks.
@@ -244,14 +188,25 @@
         """The name of the key property of this collection"""
         return self._name
 
     @property
     def tracks(self):
         return self._tracks
 
+    @property
+    def artists(self) -> list[str]:
+        """List of artists ordered by frequency of appearance on the tracks in this collection"""
+        return get_most_common_values(track.artist for track in self.tracks if track.artist)
+
+    @property
+    def genres(self) -> list[str]:
+        """List of genres ordered by frequency of appearance on the tracks in this collection"""
+        genres = (genre for track in self.tracks for genre in (track.genres if track.genres else []))
+        return get_most_common_values(genres)
+
     def __init__(
             self, tracks: Collection[LocalTrack], name: str | None = None, remote_wrangler: RemoteDataWrangler = None
     ):
         super().__init__(remote_wrangler=remote_wrangler)
         if len(tracks) == 0:
             raise LocalCollectionError("No tracks were given")
```

### Comparing `musify-0.8.1/musify/local/exception.py` & `musify-0.9.0/musify/libraries/local/exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Exceptions relating to local operations.
 """
-
-from musify.shared.exception import MusifyError
+from musify.exception import MusifyError
 
 
 class LocalError(MusifyError):
     """
     Exception raised for local errors.
 
     :param message: Explanation of the error.
@@ -40,66 +39,19 @@
     def __init__(self, message: str | None = None, kind: str | None = None):
         self.message = message
         self.kind = kind
         formatted = f"{kind} | {message}" if kind else message
         super().__init__(formatted)
 
 
-class LocalProcessorError(LocalError):
-    """Exception raised for errors related to track processors."""
-
-
 ###########################################################################
-## File errors
+## Track errors
 ###########################################################################
-class FileError(LocalError):
-    """
-    Exception raised for file errors.
-
-    :param file: The file type that caused the error.
-    :param message: Explanation of the error.
-    """
-
-    def __init__(self, file: str | None = None, message: str | None = None):
-        self.file = file
-        self.message = message
-        formatted = f"{file} | {message}" if file else message
-        super().__init__(formatted)
-
-
-class InvalidFileType(FileError):
-    """
-    Exception raised for unrecognised file types.
-
-    :param filetype: The file type that caused the error.
-    :param message: Explanation of the error.
-    """
-
-    def __init__(self, filetype: str, message: str = "File type not recognised"):
-        self.filetype = filetype
-        self.message = message
-        super().__init__(file=filetype, message=message)
-
-
-class FileDoesNotExistError(FileError, FileNotFoundError):
-    """
-    Exception raised when a file cannot be found.
-
-    :param path: The path that caused the error.
-    :param message: Explanation of the error.
-    """
-
-    def __init__(self, path: str, message: str = "File cannot be found"):
-        self.path = path
-        self.message = message
-        super().__init__(file=path, message=message)
-
-
-class ImageLoadError(FileError):
-    """Exception raised for errors in loading an image."""
+class TagError(LocalError):
+    """Exception raised for errors related to track tag errors."""
 
 
 ###########################################################################
 ## Library errors
 ###########################################################################
 class LocalLibraryError(LocalError):
     """Exception raised for errors related to :py:class:`LocalLibrary` logic."""
```

### Comparing `musify-0.8.1/musify/local/library/library.py` & `musify-0.9.0/musify/libraries/local/library/library.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 The core, basic library implementation which is just a simple set of folders.
 """
 import itertools
-from collections.abc import Collection, Mapping, Iterable
+from collections.abc import Collection, Mapping
+from concurrent.futures import ThreadPoolExecutor
 from functools import reduce
 from os.path import splitext, join, exists, basename, dirname
 from typing import Any
 
-from musify.local.collection import LocalCollection, LocalFolder, LocalAlbum, LocalArtist, LocalGenres
-from musify.local.file import PathMapper, PathStemMapper
-from musify.local.playlist import LocalPlaylist, load_playlist, PLAYLIST_CLASSES
-from musify.local.track import TRACK_CLASSES, LocalTrack, load_track
-from musify.local.track.field import LocalTrackField
+from musify.core.result import Result
+from musify.exception import MusifyError
+from musify.file.path_mapper import PathMapper, PathStemMapper
+from musify.libraries.core.object import Library
+from musify.libraries.local.collection import LocalCollection, LocalFolder, LocalAlbum, LocalArtist, LocalGenres
+from musify.libraries.local.playlist import PLAYLIST_CLASSES, LocalPlaylist, load_playlist
+from musify.libraries.local.track import TRACK_CLASSES, LocalTrack, load_track
+from musify.libraries.local.track.field import LocalTrackField
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
+from musify.log import STAT
 from musify.processors.base import Filter
 from musify.processors.filter import FilterDefinedList
 from musify.processors.sort import ItemSorter
-from musify.shared.core.misc import Result
-from musify.shared.core.object import Playlist, Library
-from musify.shared.exception import MusifyError
-from musify.shared.logger import STAT
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
-from musify.shared.types import UnitCollection, UnitIterable
-from musify.shared.utils import align_string, get_max_width, to_collection
+from musify.types import UnitCollection, UnitIterable
+from musify.utils import align_string, get_max_width, to_collection
 
 
 class LocalLibrary(LocalCollection[LocalTrack], Library[LocalTrack]):
     """
     Represents a local library, providing various methods for manipulating
     tracks and playlists across an entire local library collection.
 
@@ -54,21 +55,22 @@
         "path_mapper",
         "_playlist_paths",
         "_playlists",
         "_track_paths",
         "_tracks",
     )
     __attributes_classes__ = (Library, LocalCollection)
+    __attributes_ignore__ = ("tracks_in_playlists",)
 
-    # noinspection PyTypeChecker,PyPropertyDefinition
+    # noinspection PyPropertyDefinition
     @classmethod
     @property
     def name(cls) -> str:
         """The type of library loaded"""
-        return cls.source
+        return str(cls.source)
 
     # noinspection PyPropertyDefinition
     @classmethod
     @property
     def source(cls) -> str:
         """The type of local library loaded"""
         return cls.__name__.replace("Library", "")
@@ -270,35 +272,45 @@
             self.logger.warning(f"\33[97m{message}: \33[0m\n\t- {"\n\t- ".join(errors)} ")
             self.logger.print()
         self.errors.clear()
 
     ###########################################################################
     ## Tracks
     ###########################################################################
+    def load_track(self, path: str) -> LocalTrack | None:
+        """
+        Wrapper for :py:func:`load_track` which automatically loads the track at the given ``path``
+        and assigns optional arguments using this library's attributes.
+
+        Handles exceptions by logging paths which produce errors to internal list of ``errors``.
+        """
+        try:
+            return load_track(path=path, remote_wrangler=self.remote_wrangler)
+        except MusifyError as ex:
+            self.logger.debug(f"Load error for track: {path} - {ex}")
+            self.errors.append(path)
+
     def load_tracks(self) -> None:
         """Load all tracks from all the valid paths in this library, replacing currently loaded tracks."""
+        if not self._track_paths:
+            return
+
         self.logger.debug(f"Load {self.name} tracks: START")
         self.logger.info(
             f"\33[1;95m  >\33[1;97m Extracting metadata and properties for {len(self._track_paths)} tracks \33[0m"
         )
 
-        tracks: list[LocalTrack] = []
-        bar: Iterable[str] = self.logger.get_progress_bar(
-            iterable=self._track_paths, desc="Loading tracks", unit="tracks"
-        )
-        for path in bar:
-            try:
-                tracks.append(load_track(path=path, remote_wrangler=self.remote_wrangler))
-            except MusifyError as ex:
-                self.logger.debug(f"Load error: {path} - {ex}")
-                self.errors.append(path)
-                continue
+        with ThreadPoolExecutor(thread_name_prefix="track-loader") as executor:
+            tasks = executor.map(self.load_track, self._track_paths)
+            bar = self.logger.get_progress_bar(
+                tasks, desc="Loading tracks", unit="tracks", total=len(self._track_paths)
+            )
+            self._tracks = list(bar)
 
-        self._tracks = tracks
-        self._log_errors()
+        self._log_errors("Could not load the following tracks")
         self.logger.debug(f"Load {self.name} tracks: DONE\n")
 
     def log_tracks(self) -> None:
         width = get_max_width(self._playlist_paths) if self._playlist_paths else 20
         self.logger.stat(
             f"\33[1;96m{'LIBRARY URIS':<{width}}\33[1;0m |"
             f"\33[92m{sum([track.has_uri is True for track in self.tracks]):>6} available \33[0m|"
@@ -306,14 +318,29 @@
             f"\33[93m{sum([track.has_uri is False for track in self.tracks]):>6} unavailable \33[0m|"
             f"\33[1;94m{len(self.tracks):>6} total \33[0m"
         )
 
     ###########################################################################
     ## Playlists
     ###########################################################################
+    def load_playlist(self, path: str) -> LocalPlaylist:
+        """
+        Wrapper for :py:func:`load_playlist` which automatically loads the playlist at the given ``path``
+        and assigns optional arguments using this library's attributes.
+
+        Handles exceptions by logging paths which produce errors to internal list of ``errors``.
+        """
+        try:
+            return load_playlist(
+                path=path, tracks=self.tracks, path_mapper=self.path_mapper, remote_wrangler=self.remote_wrangler,
+            )
+        except MusifyError as ex:
+            self.logger.debug(f"Load error for playlist: {path} - {ex}")
+            self.errors.append(path)
+
     def load_playlists(self) -> None:
         """
         Load all playlists found in this library's ``playlist_folder``,
         filtered down using the ``playlist_filter`` if given, replacing currently loaded playlists.
 
         :return: The loaded playlists.
         :raise LocalCollectionError: If a given playlist name cannot be found.
@@ -322,23 +349,22 @@
             return
 
         self.logger.debug(f"Load {self.name} playlist data: START")
         self.logger.info(
             f"\33[1;95m  >\33[1;97m Loading playlist data for {len(self._playlist_paths)} playlists \33[0m"
         )
 
-        iterable = self._playlist_paths.items()
-        bar = self.logger.get_progress_bar(iterable=iterable, desc="Loading playlists", unit="playlists")
-        playlists: list[LocalPlaylist] = [
-            load_playlist(
-                path=path, tracks=self.tracks, path_mapper=self.path_mapper, remote_wrangler=self.remote_wrangler,
-            ) for name, path in bar
-        ]
+        with ThreadPoolExecutor(thread_name_prefix="playlist-loader") as executor:
+            tasks = executor.map(self.load_playlist, self._playlist_paths.values())
+            bar = self.logger.get_progress_bar(
+                tasks, desc="Loading playlists", unit="playlists", total=len(self._playlist_paths)
+            )
+            self._playlists = {pl.name: pl for pl in sorted(bar, key=lambda x: x.name.casefold())}
 
-        self._playlists = {pl.name: pl for pl in sorted(playlists, key=lambda x: x.name.casefold())}
+        self._log_errors("Could not load the following playlists")
         self.logger.debug(f"Load {self.name} playlists: DONE\n")
 
     def log_playlists(self) -> None:
         max_width = get_max_width(self.playlists)
 
         self.logger.stat(f"\33[1;96m{self.name.upper()} PLAYLISTS: \33[0m")
         for name, playlist in self.playlists.items():
@@ -350,23 +376,22 @@
                 f"\33[1;94m{len(playlist):>6} total \33[0m"
             )
 
     def save_playlists(self, dry_run: bool = True) -> dict[str, Result]:
         """
         For each Playlist in this Library, saves its associate tracks and its settings (if applicable) to file.
 
-        :param dry_run: Run function, but do not modify file at all.
+        :param dry_run: Run function, but do not modify the file on the disk.
         :return: A map of the playlist name to the results of its sync as a :py:class:`Result` object.
         """
-        return {name: pl.save(dry_run=dry_run) for name, pl in self.playlists.items()}
+        with ThreadPoolExecutor(thread_name_prefix="playlist-saver") as executor:
+            futures = {name: executor.submit(pl.save, dry_run=dry_run) for name, pl in self.playlists.items()}
+            bar = self.logger.get_progress_bar(futures.items(), desc="Updating playlists", unit="playlists")
 
-    def merge_playlists(
-            self, playlists: Library[LocalTrack] | Collection[Playlist[LocalTrack]] | Mapping[Any, Playlist[LocalTrack]]
-    ) -> None:
-        raise NotImplementedError
+            return dict(bar)
 
     ###########################################################################
     ## Backup/restore
     ###########################################################################
     def restore_tracks(
             self, backup: Mapping[str, Mapping[str, Any]], tags: UnitIterable[LocalTrackField] = LocalTrackField.ALL
     ) -> int:
@@ -392,7 +417,41 @@
             count += 1
 
         return count
 
     def _get_attributes(self) -> dict[str, Any]:
         attributes_extra = {"remote_source": self.remote_wrangler.source if self.remote_wrangler else None}
         return super()._get_attributes() | attributes_extra
+
+    def json(self):
+        self.logger.info(
+            f"\33[1;95m ->\33[1;97m Extracting JSON data for library of "
+            f"{len(self.tracks)} tracks and {len(self.playlists)} playlists\n"
+        )
+
+        attributes = self._get_attributes()
+
+        playlists: dict[str, LocalPlaylist] | None = None
+        if "playlists" in attributes and "tracks" in attributes:
+            playlists = attributes["playlists"]
+            attributes["playlists"] = {}
+
+        self_json = self._to_json(attributes, pool=True)
+
+        if playlists is not None:
+            tracks: Mapping[str, Mapping[str, Any]] = {track["path"]: track for track in self_json["tracks"]}
+
+            def _get_playlist_json(pl: LocalPlaylist) -> tuple[str, dict[str, Any]]:
+                pl_attributes = pl._get_attributes()
+                pl_attributes["tracks"] = []
+
+                pl_json = pl._to_json(pl_attributes, pool=True)
+                pl_json["tracks"] = [tracks.get(track.path) for track in pl]
+
+                return pl.name, pl_json
+
+            with ThreadPoolExecutor(thread_name_prefix="to-json-playlists") as executor:
+                tasks = executor.map(_get_playlist_json, playlists.values())
+
+            self_json["playlists"] = dict(sorted(tasks, key=lambda x: x[0]))
+
+        return self_json
```

### Comparing `musify-0.8.1/musify/local/library/musicbee.py` & `musify-0.9.0/musify/libraries/local/library/musicbee.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
 An implementation of :py:class:`LocalLibrary` for the MusicBee library manager.
 Reads library/settings files from MusicBee to load and enrich playlist/track etc. data.
 """
-
 import hashlib
 import re
 import urllib.parse
 from collections.abc import Iterable, Mapping, Sequence, Collection, Iterator
 from datetime import datetime
 from os.path import join, exists, normpath
 from typing import Any
 
 import xmltodict
 from lxml import etree
 from lxml.etree import iterparse
 
-from musify.local.exception import MusicBeeIDError, XMLReaderError, FileDoesNotExistError
-from musify.local.file import File, PathMapper, PathStemMapper
-from musify.local.library.library import LocalLibrary
-from musify.local.playlist import LocalPlaylist
-from musify.local.track import LocalTrack
+from musify.file.base import File
+from musify.file.exception import FileDoesNotExistError
+from musify.file.path_mapper import PathMapper, PathStemMapper
+from musify.libraries.local.exception import MusicBeeIDError, XMLReaderError
+from musify.libraries.local.library.library import LocalLibrary
+from musify.libraries.local.playlist import LocalPlaylist
+from musify.libraries.local.track import LocalTrack
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
 from musify.processors.base import Filter
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
-from musify.shared.types import Number
-from musify.shared.utils import to_collection
+from musify.types import Number
+from musify.utils import to_collection
 
 
 class MusicBee(LocalLibrary, File):
     """
     Represents a local MusicBee library, providing various methods for manipulating
     tracks and playlists across an entire local library collection.
 
@@ -146,15 +147,15 @@
         self._log_errors("Could not find a loaded track for these paths from the MusicBee library file")
         self.logger.debug(f"Enrich {self.name} tracks: DONE\n")
 
     def save(self, dry_run: bool = True, *_, **__) -> dict[str, Any]:
         """
         Generate and save the XML library file for this MusicBee library.
 
-        :param dry_run: Run function, but do not modify file at all.
+        :param dry_run: Run function, but do not modify the file on the disk.
         :return: Map representation of the saved XML file.
         """
         self.logger.debug(f"Save {self.name} library file: START")
         # need to remove library folders to allow match to be os agnostic
         track_map = {
             track.path.removeprefix(folder).casefold(): track
             for folder in self.library_folders for track in self.tracks
@@ -265,15 +266,15 @@
             "Total Time": int(track.length * 1000),  # in milliseconds
             "Rating": track.rating,
             # "Composer": track.composer,  # currently not supported by this program
             # "Conductor": track.conductor,  # currently not supported by this program
             # "Publisher": track.publisher,  # currently not supported by this program
             # "Encoder": track.encoder,  # currently not supported by this program
             "Size": track.size,
-            "Kind": track.kind,
+            "Kind": track.type,
             # "": track.channels,  # unknown MusicBee mapping
             "Bit Rate": int(track.bit_rate),
             # "": track.bit_depth,  # unknown MusicBee mapping
             "Sample Rate": int(track.sample_rate * 1000),  # in Hz
             "Date Modified": track.date_modified,
             "Date Added": track.date_added,
             "Play Date UTC": track.last_played,
@@ -504,15 +505,15 @@
                 raise XMLReaderError(f"Unexpected value type: {value} ({type(value)})")
 
     def unparse(self, data: Mapping[str, Any], dry_run: bool = True) -> None:
         """
         Un-parse a map of XML data to XML and save to file.
 
         :param data: Map of XML data to export.
-        :param dry_run: Run function, but do not modify file at all.
+        :param dry_run: Run function, but do not modify the file on the disk.
         """
         et: etree._ElementTree = etree.parse(self.path)
         parsed: dict[str, Any] = xmltodict.parse(etree.tostring(et.getroot(), encoding='utf-8', method='xml'))
 
         root: etree.Element = etree.Element(et.docinfo.root_name)
         root.set("version", parsed[et.docinfo.root_name]["@version"])
```

### Comparing `musify-0.8.1/musify/local/playlist/base.py` & `musify-0.9.0/musify/libraries/local/playlist/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Base implementation for the functionality of a local playlist.
 """
-
 from abc import ABCMeta, abstractmethod
 from collections.abc import Collection
 from datetime import datetime
 from os.path import dirname, join, getmtime, getctime, exists
 
-from musify.local.collection import LocalCollection
-from musify.local.file import File, PathMapper
-from musify.local.track import LocalTrack
+from musify.core.result import Result
+from musify.file.base import File
+from musify.file.path_mapper import PathMapper
+from musify.libraries.core.object import Playlist
+from musify.libraries.local.collection import LocalCollection
+from musify.libraries.local.track import LocalTrack
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
 from musify.processors.base import Filter
 from musify.processors.limit import ItemLimiter
 from musify.processors.sort import ItemSorter
-from musify.shared.core.misc import Result
-from musify.shared.core.object import Playlist
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
 
 
 class LocalPlaylist[T: Filter[LocalTrack]](LocalCollection[LocalTrack], Playlist[LocalTrack], File, metaclass=ABCMeta):
     """
     Generic class for loading and manipulating local playlists.
 
     :param path: Absolute path of the playlist.
@@ -99,32 +99,29 @@
         #: Maps paths stored in the playlist file.
         self.path_mapper = path_mapper
 
         self._tracks: list[LocalTrack] = []
         self._original: list[LocalTrack] = []
 
     def _match(self, tracks: Collection[LocalTrack] = (), reference: LocalTrack | None = None) -> None:
-        """Wrapper for matcher operations"""
         if self.matcher is None or not tracks:
             return
 
         if not self.matcher.ready:  # just return the tracks given if matcher has no settings applied
             self.tracks: list[LocalTrack] = list(tracks)
         else:  # run matcher
             self.tracks: list[LocalTrack] = list(self.matcher(values=tracks, reference=reference))
 
     def _limit(self, ignore: Collection[str | LocalTrack]) -> None:
-        """Wrapper for limiter operations"""
         if self.limiter is not None and self.tracks is not None:
             track_path_map = {track.path: track for track in self.tracks}
             ignore: set[LocalTrack] = {i if isinstance(i, LocalTrack) else track_path_map.get(i) for i in ignore}
             self.limiter(items=self.tracks, ignore=ignore)
 
     def _sort(self) -> None:
-        """Wrapper for sorter operations"""
         if self.sorter is not None and self.tracks is not None:
             self.sorter(items=self.tracks)
 
     @abstractmethod
     def load(self, tracks: Collection[LocalTrack] = ()) -> list[LocalTrack]:
         """
         Read the playlist file and update the tracks in this playlist instance.
@@ -135,14 +132,11 @@
         raise NotImplementedError
 
     @abstractmethod
     def save(self, dry_run: bool = True, *args, **kwargs) -> Result:
         """
         Write the tracks in this Playlist and its settings (if applicable) to file.
 
-        :param dry_run: Run function, but do not modify file at all.
+        :param dry_run: Run function, but do not modify the file on the disk.
         :return: :py:class:`Result` object with stats on the changes to the playlist.
         """
         raise NotImplementedError
-
-    def merge(self, playlist: Playlist[LocalTrack]) -> None:
-        raise NotImplementedError
```

### Comparing `musify-0.8.1/musify/local/playlist/m3u.py` & `musify-0.9.0/musify/libraries/local/playlist/m3u.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 The M3U implementation of a :py:class:`LocalPlaylist`.
 """
-
 import os
 from collections.abc import Collection
 from dataclasses import dataclass
 from os.path import exists, dirname
 
-from musify.local.file import PathMapper, File
-from musify.local.playlist.base import LocalPlaylist
-from musify.local.track import LocalTrack, load_track
+from musify.core.result import Result
+from musify.file.base import File
+from musify.file.path_mapper import PathMapper
+from musify.libraries.local.playlist.base import LocalPlaylist
+from musify.libraries.local.track import LocalTrack, load_track
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
 from musify.processors.filter import FilterDefinedList
-from musify.shared.core.misc import Result
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
 
 
 @dataclass(frozen=True)
 class SyncResultM3U(Result):
     """Stores the results of a sync with a local M3U playlist"""
     #: The total number of tracks in the playlist before the sync.
     start: int
@@ -110,15 +110,15 @@
         self._original = self.tracks.copy() if exists(self._path) else []
         return self.tracks
 
     def save(self, dry_run: bool = True, *_, **__) -> SyncResultM3U:
         """
         Write the tracks in this Playlist and its settings (if applicable) to file.
 
-        :param dry_run: Run function, but do not modify file at all.
+        :param dry_run: Run function, but do not modify the file on the disk.
         :return: The results of the sync as a :py:class:`SyncResultM3U` object.
         """
         start_paths = {path.casefold() for path in self.path_mapper.unmap_many(self._original, check_existence=False)}
         os.makedirs(dirname(self.path), exist_ok=True)
 
         if not dry_run:
             with open(self.path, "w", encoding="utf-8") as file:
```

### Comparing `musify-0.8.1/musify/local/playlist/utils.py` & `musify-0.9.0/musify/libraries/local/playlist/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 Utilities for operations on :py:class:`LocalPlaylist` types.
 
 Generally, this will contain global variables representing all supported playlist file types
 and a utility function for loading the appropriate :py:class:`LocalPlaylist` type for a path based on its extension.
 """
-
 from collections.abc import Collection
 from os.path import splitext
 
-from musify.local.exception import InvalidFileType
-from musify.local.file import PathMapper
-from musify.local.playlist.base import LocalPlaylist
-from musify.local.playlist.m3u import M3U
-from musify.local.playlist.xautopf import XAutoPF
-from musify.local.track import LocalTrack
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
+from musify.file.exception import InvalidFileType
+from musify.file.path_mapper import PathMapper
+from musify.libraries.local.playlist.base import LocalPlaylist
+from musify.libraries.local.playlist.m3u import M3U
+from musify.libraries.local.playlist.xautopf import XAutoPF
+from musify.libraries.local.track import LocalTrack
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
 
 PLAYLIST_CLASSES = frozenset({M3U, XAutoPF})
 PLAYLIST_FILETYPES = frozenset(filetype for c in PLAYLIST_CLASSES for filetype in c.valid_extensions)
 
 
 def load_playlist(
         path: str,
@@ -41,14 +40,12 @@
         If given, the wrangler can be used when calling __get_item__ to get an item from the collection from its URI.
         The wrangler is also used when loading tracks to allow them to process URI tags.
         For more info on this, see :py:class:`LocalTrack`.
     :return: Loaded :py:class:`LocalPlaylist` object
     :raise InvalidFileType: If the file type is not supported.
     """
     ext = splitext(path)[1].casefold()
+    if ext not in PLAYLIST_FILETYPES:
+        raise InvalidFileType(ext, f"Not an accepted extension. Use only: {', '.join(PLAYLIST_FILETYPES)}")
 
-    if ext in M3U.valid_extensions:
-        return M3U(path=path, tracks=tracks, path_mapper=path_mapper, remote_wrangler=remote_wrangler)
-    elif ext in XAutoPF.valid_extensions:
-        return XAutoPF(path=path, tracks=tracks, path_mapper=path_mapper)
-
-    raise InvalidFileType(ext, f"Not an accepted extension. Use only: {', '.join(PLAYLIST_FILETYPES)}")
+    cls = next(cls for cls in PLAYLIST_CLASSES if ext in cls.valid_extensions)
+    return cls(path=path, tracks=tracks, path_mapper=path_mapper, remote_wrangler=remote_wrangler)
```

### Comparing `musify-0.8.1/musify/local/track/field.py` & `musify-0.9.0/musify/libraries/local/track/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 The core Field enum for a :py:class:`LocalTrack` representing all possible tags/metadata/properties.
 """
-
-from musify.shared.core.enum import TagFields
-from musify.shared.field import TrackFieldMixin
+from musify.core.enum import TagFields
+from musify.field import TrackFieldMixin
 
 
 class LocalTrackField(TrackFieldMixin):
-    """Represent all currently supported fields for objects of type :py:class:`LocalTrack`"""
+    """Represents all currently supported fields for objects of type :py:class:`LocalTrack`"""
     ALL = TagFields.ALL.value
 
     TITLE = TagFields.TITLE.value
     ARTIST = TagFields.ARTIST.value
     ALBUM = TagFields.ALBUM.value
     ALBUM_ARTIST = TagFields.ALBUM_ARTIST.value
     TRACK = TagFields.TRACK_NUMBER.value + 500
@@ -35,15 +34,15 @@
 
     # file properties
     PATH = TagFields.PATH.value
     FOLDER = TagFields.FOLDER.value
     FILENAME = TagFields.FILENAME.value
     EXT = TagFields.EXT.value
     SIZE = TagFields.SIZE.value
-    KIND = TagFields.KIND.value
+    TYPE = TagFields.TYPE.value
     CHANNELS = TagFields.CHANNELS.value
     BIT_RATE = TagFields.BIT_RATE.value
     BIT_DEPTH = TagFields.BIT_DEPTH.value
     SAMPLE_RATE = TagFields.SAMPLE_RATE.value
 
     # date properties
     DATE_MODIFIED = TagFields.DATE_MODIFIED.value
```

### Comparing `musify-0.8.1/musify/local/track/flac.py` & `musify-0.9.0/musify/libraries/local/track/flac.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,121 @@
 """
 The FLAC implementation of a :py:class:`LocalTrack`.
 """
-
 from io import BytesIO
 from typing import Any
 
 import mutagen
 import mutagen.flac
 import mutagen.id3
 from PIL import Image
 
-from musify.local.file import open_image, get_image_bytes
-from musify.local.track.base.track import LocalTrack
-from musify.local.track.field import LocalTrackField
-from musify.shared.core.enum import TagMap
+from musify.core.enum import TagMap
+from musify.file.image import open_image, get_image_bytes
+from musify.libraries.local.track.field import LocalTrackField
+from musify.libraries.local.track.tags.reader import TagReader
+from musify.libraries.local.track.tags.writer import TagWriter
+from musify.libraries.local.track.track import LocalTrack
 
 
-class FLAC(LocalTrack[mutagen.flac.FLAC]):
+class FLACTagReader(TagReader[mutagen.flac.FLAC]):
 
-    valid_extensions = frozenset({".flac"})
+    def read_images(self) -> list[Image.Image] | None:
+        values = self.file.pictures
+        return [Image.open(BytesIO(value.data)) for value in values] if len(values) > 0 else None
 
-    # noinspection SpellCheckingInspection
-    #: Map of human-friendly tag name to ID3 tag ids for a given file type
-    tag_map = TagMap(
-        title=["title"],
-        artist=["artist"],
-        album=["album"],
-        album_artist=["albumartist"],
-        track_number=["tracknumber", "track"],
-        track_total=["tracktotal"],
-        genres=["genre"],
-        date=["date", "year"],
-        year=["year"],
-        bpm=["bpm"],
-        key=["initialkey"],
-        disc_number=["discnumber"],
-        disc_total=["disctotal"],
-        compilation=["compilation"],
-        comments=["comment", "description"],
-    )
+    def check_for_images(self) -> bool:
+        return len(self.file.pictures) > 0
 
-    def _read_images(self) -> list[Image.Image] | None:
-        values = self._file.pictures
-        return [Image.open(BytesIO(value.data)) for value in values] if len(values) > 0 else None
 
-    def _check_for_images(self) -> bool:
-        return len(self._file.pictures) > 0
+class FLACTagWriter(TagWriter[mutagen.flac.FLAC]):
 
-    def _write_tag(self, tag_id: str | None, tag_value: Any, dry_run: bool = True) -> bool:
-        result = super()._write_tag(tag_id=tag_id, tag_value=tag_value, dry_run=dry_run)
+    def write_tag(self, tag_id: str | None, tag_value: Any, dry_run: bool = True) -> bool:
+        result = super().write_tag(tag_id=tag_id, tag_value=tag_value, dry_run=dry_run)
         if result is not None:
             return result
 
         if not dry_run:
             if isinstance(tag_value, (list, set, tuple)):
-                self._file[tag_id] = list(map(str, tag_value))
+                self.file[tag_id] = list(map(str, tag_value))
             else:
-                self._file[tag_id] = str(tag_value)
+                self.file[tag_id] = str(tag_value)
         return True
 
-    def _write_images(self, dry_run: bool = True) -> bool:
+    def _write_images(self, track: LocalTrack, dry_run: bool = True) -> bool:
         updated = False
-        for image_kind, image_link in self.image_links.items():
+        for image_kind, image_link in track.image_links.items():
             image = open_image(image_link)
             image_kind_attr = image_kind.upper().replace(" ", "_")
 
             picture = mutagen.flac.Picture()
             picture.type = getattr(mutagen.id3.PictureType, image_kind_attr)
             picture.mime = Image.MIME[image.format]
             picture.data = get_image_bytes(image)
 
             if not dry_run:
                 # clear all images, adding back those that don't match the new image's type
-                pictures_current = self._file.pictures.copy()
-                self._file.clear_pictures()
+                pictures_current = self.file.pictures.copy()
+                self.file.clear_pictures()
                 for pic in pictures_current:
                     if pic.type != picture.type:
-                        self._file.add_picture(pic)
+                        self.file.add_picture(pic)
 
-                self._file.add_picture(picture)
+                self.file.add_picture(picture)
 
             image.close()
-            self.has_image = True
+            track.has_image = True
             updated = True
 
         return updated
 
     def delete_tag(self, tag_name: str, dry_run: bool = True) -> bool:
         if tag_name == LocalTrackField.IMAGES.name.lower():
-            self._file.clear_pictures()
+            self.file.clear_pictures()
             return True
 
         removed = False
 
         tag_ids = self.tag_map[tag_name]
         if tag_ids is None or len(tag_ids) is None:
             return removed
 
         for tag_id in tag_ids:
-            if tag_id in self._file and self._file[tag_id]:
+            if tag_id in self.file and self.file[tag_id]:
                 if not dry_run:
-                    del self._file[tag_id]
+                    del self.file[tag_id]
                 removed = True
 
         return removed
+
+
+class FLAC(LocalTrack[mutagen.flac.FLAC, FLACTagReader, FLACTagWriter]):
+
+    valid_extensions = frozenset({".flac"})
+
+    # noinspection SpellCheckingInspection
+    #: Map of human-friendly tag name to ID3 tag ids for a given file type
+    tag_map = TagMap(
+        title=["title"],
+        artist=["artist"],
+        album=["album"],
+        album_artist=["albumartist"],
+        track_number=["tracknumber", "track"],
+        track_total=["tracktotal"],
+        genres=["genre"],
+        date=["date", "year"],
+        year=["year"],
+        bpm=["bpm"],
+        key=["initialkey"],
+        disc_number=["discnumber"],
+        disc_total=["disctotal"],
+        compilation=["compilation"],
+        comments=["comment", "description"],
+    )
+
+    @staticmethod
+    def _create_reader(*args, **kwargs):
+        return FLACTagReader(*args, **kwargs)
+
+    @staticmethod
+    def _create_writer(*args, **kwargs):
+        return FLACTagWriter(*args, **kwargs)
```

### Comparing `musify-0.8.1/musify/local/track/m4a.py` & `musify-0.9.0/musify/libraries/local/track/m4a.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,29 @@
 """
 The M4A implementation of a :py:class:`LocalTrack`.
 """
-
 from collections.abc import Iterable
 from io import BytesIO
 from typing import Any
 
 import mutagen
 import mutagen.mp4
 from PIL import Image
 
-from musify.local.file import open_image, get_image_bytes
-from musify.local.track.base.track import LocalTrack
-from musify.shared.core.enum import TagMap
-from musify.shared.utils import to_collection
-
+from musify.core.enum import TagMap
+from musify.file.image import open_image, get_image_bytes
+from musify.libraries.local.track.tags.reader import TagReader
+from musify.libraries.local.track.tags.writer import TagWriter
+from musify.libraries.local.track.track import LocalTrack
+from musify.utils import to_collection
 
-class M4A(LocalTrack[mutagen.mp4.MP4]):
 
-    valid_extensions = frozenset({".m4a"})
+class M4ATagReader(TagReader[mutagen.mp4.MP4]):
 
-    # noinspection SpellCheckingInspection
-    #: Map of human-friendly tag name to ID3 tag ids for a given file type
-    tag_map = TagMap(
-        title=["©nam"],
-        artist=["©ART"],
-        album=["©alb"],
-        album_artist=["aART"],
-        track_number=["trkn"],
-        track_total=["trkn"],
-        genres=["----:com.apple.iTunes:GENRE", "©gen", "gnre"],
-        date=["©day"],
-        bpm=["tmpo"],
-        key=["----:com.apple.iTunes:INITIALKEY"],
-        disc_number=["disk"],
-        disc_total=["disk"],
-        compilation=["cpil"],
-        comments=["©cmt"],
-        images=["covr"],
-    )
-
-    def _read_tag(self, tag_ids: Iterable[str]) -> list[Any] | None:
+    def read_tag(self, tag_ids: Iterable[str]) -> list[Any] | None:
         """Extract all tag values for a given list of tag IDs"""
         values = []
         for tag_id in tag_ids:
             value = self.file.get(tag_id)
             if value is None or (isinstance(value, str) and len(value.strip()) == 0):
                 # skip null or empty/blank strings
                 continue
@@ -54,100 +33,136 @@
             elif isinstance(value, bytes):
                 value = value.decode("utf-8").split('\x00')
 
             values.extend(value) if isinstance(value, (list, set, tuple)) else values.append(value)
 
         return values if len(values) > 0 else None
 
-    def _read_track_number(self) -> int | None:
-        values = self._read_tag(self.tag_map.track_number)
+    def read_track_number(self) -> int | None:
+        values = self.read_tag(self.tag_map.track_number)
         return int(values[0][0]) if values is not None else None
 
-    def _read_track_total(self) -> int | None:
-        values = self._read_tag(self.tag_map.track_total)
+    def read_track_total(self) -> int | None:
+        values = self.read_tag(self.tag_map.track_total)
         return int(values[0][1]) if values is not None else None
 
-    def _read_key(self) -> str | None:
-        values = self._read_tag(self.tag_map.key)
+    def read_key(self) -> str | None:
+        values = self.read_tag(self.tag_map.key)
         return str(values[0][:]) if values is not None else None
 
-    def _read_disc_number(self) -> int | None:
-        values = self._read_tag(self.tag_map.disc_number)
+    def read_disc_number(self) -> int | None:
+        values = self.read_tag(self.tag_map.disc_number)
         return int(values[0][0]) if values is not None else None
 
-    def _read_disc_total(self) -> int | None:
-        values = self._read_tag(self.tag_map.disc_total)
+    def read_disc_total(self) -> int | None:
+        values = self.read_tag(self.tag_map.disc_total)
         return int(values[0][1]) if values is not None else None
 
-    def _read_images(self) -> list[Image.Image] | None:
-        values = self._read_tag(self.tag_map.images)
+    def read_images(self) -> list[Image.Image] | None:
+        values = self.read_tag(self.tag_map.images)
         return [Image.open(BytesIO(bytes(value))) for value in values] if values is not None else None
 
-    def _write_tag(self, tag_id: str | None, tag_value: Any, dry_run: bool = True) -> bool:
-        result = super()._write_tag(tag_id=tag_id, tag_value=tag_value, dry_run=dry_run)
+
+class M4ATagWriter(TagWriter[mutagen.mp4.MP4]):
+
+    def write_tag(self, tag_id: str | None, tag_value: Any, dry_run: bool = True) -> bool:
+        result = super().write_tag(tag_id=tag_id, tag_value=tag_value, dry_run=dry_run)
         if result is not None:
             return result
 
         if not dry_run:
             if tag_id.startswith("----:com.apple.iTunes"):
-                self._file[tag_id] = [
+                self.file[tag_id] = [
                     mutagen.mp4.MP4FreeForm(str(v).encode("utf-8"), 1) for v in to_collection(tag_value)
                 ]
             elif isinstance(tag_value, bool):
-                self._file[tag_id] = tag_value
+                self.file[tag_id] = tag_value
             elif isinstance(tag_value, tuple):
-                self._file[tag_id] = [tag_value]
+                self.file[tag_id] = [tag_value]
             else:
-                self._file[tag_id] = to_collection(tag_value, list)
+                self.file[tag_id] = to_collection(tag_value, list)
         return True
 
-    def _write_track(self, dry_run: bool = True) -> bool:
+    def _write_track(self, track: LocalTrack, dry_run: bool = True) -> bool:
         tag_id = next(iter(self.tag_map.track_number), None)
-        tag_value = (self.track_number, self.track_total)
-        return self._write_tag(tag_id, tag_value, dry_run)
+        tag_value = (track.track_number, track.track_total)
+        return self.write_tag(tag_id, tag_value, dry_run)
 
-    def _write_date(self, dry_run: bool = True) -> tuple[bool, bool, bool, bool]:
-        date_str = self.date.strftime(self.date_format) if self.date else None
+    def _write_date(self, track: LocalTrack, dry_run: bool = True) -> tuple[bool, bool, bool, bool]:
+        date_str = track.date.strftime(self.date_format) if track.date else None
         if not date_str:
-            date_str = f"{self.year}-{str(self.month).zfill(2)}" if self.month else str(self.year)
-        date = self._write_tag(next(iter(self.tag_map.date), None), date_str, dry_run)
+            date_str = f"{track.year}-{str(track.month).zfill(2)}" if track.month else str(track.year)
+        date = self.write_tag(next(iter(self.tag_map.date), None), date_str, dry_run)
         if date:
             return date, False, False, False
 
-        year = self._write_tag(next(iter(self.tag_map.year), None), str(self.year) if self.year else None, dry_run)
-        month = self._write_tag(next(iter(self.tag_map.month), None), str(self.month) if self.month else None, dry_run)
-        day = self._write_tag(next(iter(self.tag_map.day), None), str(self.day) if self.day else None, dry_run)
+        year = self.write_tag(next(iter(self.tag_map.year), None), str(track.year) if track.year else None, dry_run)
+        month = self.write_tag(next(iter(self.tag_map.month), None), str(track.month) if track.month else None, dry_run)
+        day = self.write_tag(next(iter(self.tag_map.day), None), str(track.day) if track.day else None, dry_run)
 
         return date, year, month, day
 
-    def _write_bpm(self, dry_run: bool = True) -> bool:
-        return self._write_tag(next(iter(self.tag_map.bpm), None), int(self.bpm), dry_run)
+    def _write_bpm(self, track: LocalTrack, dry_run: bool = True) -> bool:
+        return self.write_tag(next(iter(self.tag_map.bpm), None), int(track.bpm), dry_run)
 
-    def _write_disc(self, dry_run: bool = True) -> bool:
+    def _write_disc(self, track: LocalTrack, dry_run: bool = True) -> bool:
         tag_id = next(iter(self.tag_map.disc_number), None)
-        tag_value = (self.disc_number, self.disc_total)
-        return self._write_tag(tag_id, tag_value, dry_run)
+        tag_value = (track.disc_number, track.disc_total)
+        return self.write_tag(tag_id, tag_value, dry_run)
 
-    def _write_compilation(self, dry_run: bool = True) -> bool:
-        return self._write_tag(next(iter(self.tag_map.compilation), None), self.compilation, dry_run)
+    def _write_compilation(self, track: LocalTrack, dry_run: bool = True) -> bool:
+        return self.write_tag(next(iter(self.tag_map.compilation), None), track.compilation, dry_run)
 
-    def _write_images(self, dry_run: bool = True) -> bool:
+    def _write_images(self, track: LocalTrack, dry_run: bool = True) -> bool:
         tag_id = next(iter(self.tag_map.images), None)
 
         updated = False
         tag_value = []
-        for image_link in self.image_links.values():
+        for image_link in track.image_links.values():
             image = open_image(image_link)
 
             if image.format == "PNG":
                 image_format = mutagen.mp4.MP4Cover.FORMAT_PNG
             else:
                 image_format = mutagen.mp4.MP4Cover.FORMAT_JPEG
 
             tag_value.append(mutagen.mp4.MP4Cover(get_image_bytes(image), imageformat=image_format))
             image.close()
 
         if len(tag_value) > 0:
-            updated = self._write_tag(tag_id, tag_value, dry_run)
+            updated = self.write_tag(tag_id, tag_value, dry_run)
 
-        self.has_image = updated or self.has_image
+        track.has_image = updated or track.has_image
         return updated
+
+
+class M4A(LocalTrack[mutagen.mp4.MP4, M4ATagReader, M4ATagWriter]):
+
+    valid_extensions = frozenset({".m4a"})
+
+    # noinspection SpellCheckingInspection
+    #: Map of human-friendly tag name to ID3 tag ids for a given file type
+    tag_map = TagMap(
+        title=["©nam"],
+        artist=["©ART"],
+        album=["©alb"],
+        album_artist=["aART"],
+        track_number=["trkn"],
+        track_total=["trkn"],
+        genres=["----:com.apple.iTunes:GENRE", "©gen", "gnre"],
+        date=["©day"],
+        bpm=["tmpo"],
+        key=["----:com.apple.iTunes:INITIALKEY"],
+        disc_number=["disk"],
+        disc_total=["disk"],
+        compilation=["cpil"],
+        comments=["©cmt"],
+        images=["covr"],
+    )
+
+    @staticmethod
+    def _create_reader(*args, **kwargs):
+        return M4ATagReader(*args, **kwargs)
+
+    @staticmethod
+    def _create_writer(*args, **kwargs):
+        return M4ATagWriter(*args, **kwargs)
```

### Comparing `musify-0.8.1/musify/local/track/mp3.py` & `musify-0.9.0/musify/libraries/local/track/mp3.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,169 +1,186 @@
 """
 The MP3 implementation of a :py:class:`LocalTrack`.
 """
-
 from collections.abc import Iterable
 from io import BytesIO
 from typing import Any
 
 import mutagen
 import mutagen.id3
 import mutagen.mp3
 from PIL import Image
 
-from musify.local.file import open_image, get_image_bytes
-from musify.local.track.base.track import LocalTrack
-from musify.local.track.field import LocalTrackField
-from musify.shared.core.enum import TagMap
-
+from musify.core.enum import TagMap
+from musify.file.image import open_image, get_image_bytes
+from musify.libraries.local.exception import TagError
+from musify.libraries.local.track.field import LocalTrackField
+from musify.libraries.local.track.tags.reader import TagReader
+from musify.libraries.local.track.tags.writer import TagWriter
+from musify.libraries.local.track.track import LocalTrack
 
-class MP3(LocalTrack[mutagen.mp3.MP3]):
 
-    valid_extensions = frozenset({".mp3"})
-
-    # noinspection SpellCheckingInspection
-    #: Map of human-friendly tag name to ID3 tag ids for a given file type
-    tag_map = TagMap(
-        title=["TIT2"],
-        artist=["TPE1"],
-        album=["TALB"],
-        album_artist=["TPE2"],
-        track_number=["TRCK"],
-        track_total=["TRCK"],
-        genres=["TCON"],
-        date=["TDRC", "TDAT", "TDOR"],
-        year=["TYER", "TORY"],
-        bpm=["TBPM"],
-        key=["TKEY"],
-        disc_number=["TPOS"],
-        disc_total=["TPOS"],
-        compilation=["TCMP"],
-        comments=["COMM"],
-        images=["APIC"],
-    )
+class MP3TagReader(TagReader[mutagen.mp3.MP3]):
 
-    def _read_tag(self, tag_ids: Iterable[str]) -> list[Any] | None:
+    def read_tag(self, tag_ids: Iterable[str]) -> list[Any] | None:
         # MP3 tag ids come in parts separated by : i.e. 'COMM:ID3v1 Comment:eng'
         # need to search all actual MP3 tag ids to check if the first part equals any of the given base tag ids
-        tag_ids = tuple(mp3_id for mp3_id in self._file.keys() for tag_id in tag_ids if mp3_id.split(":")[0] == tag_id)
+        tag_ids = tuple(mp3_id for mp3_id in self.file.keys() for tag_id in tag_ids if mp3_id.split(":")[0] == tag_id)
 
         values = []
         for tag_id in tag_ids:
-            value = self._file.get(tag_id)
+            value = self.file.get(tag_id)
             if value is None:
                 continue
 
             # convert id3 object to python types, causes downstream if not
             if isinstance(value, mutagen.id3.TextFrame):
                 values.extend(str(value).split('\x00'))
             elif isinstance(value, mutagen.id3.APIC):
                 values.append(value)
             else:
-                raise NotImplementedError(f"Unrecognised id3 type: {value} ({type(value)})")
+                raise TagError(f"Unrecognised id3 type: {value} ({type(value)})")
 
         return values if len(values) > 0 else None
 
-    def _read_genres(self) -> list[str] | None:
+    def read_genres(self) -> list[str] | None:
         """Extract metadata from file for genre"""
-        values = self._read_tag(self.tag_map.genres)
+        values = self.read_tag(self.tag_map.genres)
         if values is None:
             return
         return [genre for value in values for genre in value.split(";")]
 
-    def _read_images(self) -> list[Image.Image] | None:
-        values = self._read_tag(self.tag_map.images)
+    def read_images(self) -> list[Image.Image] | None:
+        values = self.read_tag(self.tag_map.images)
         return [Image.open(BytesIO(value.data)) for value in values] if values is not None else None
 
-    def _write_tag(self, tag_id: str | None, tag_value: Any, dry_run: bool = True) -> bool:
-        result = super()._write_tag(tag_id=tag_id, tag_value=tag_value, dry_run=dry_run)
+
+class MP3TagWriter(TagWriter[mutagen.mp3.MP3]):
+
+    def delete_tag(self, tag_name: str, dry_run: bool = True) -> bool:
+        removed = False
+
+        tag_ids = self.tag_map[tag_name]
+        if tag_ids is None or len(tag_ids) is None:
+            return removed
+
+        for tag_id_prefix in tag_ids:
+            for mp3_id in list(self.file.keys()).copy():
+                if mp3_id.split(":")[0] == tag_id_prefix and self.file[mp3_id]:
+                    if not dry_run:
+                        del self.file[mp3_id]
+                    removed = True
+
+        return removed
+
+    def write_tag(self, tag_id: str | None, tag_value: Any, dry_run: bool = True) -> bool:
+        result = super().write_tag(tag_id=tag_id, tag_value=tag_value, dry_run=dry_run)
         if result is not None:
             return result
 
         if not dry_run:
-            self._file[tag_id] = getattr(mutagen.id3, tag_id)(3, text=str(tag_value))
+            self.file[tag_id] = getattr(mutagen.id3, tag_id)(3, text=str(tag_value))
         return True
 
-    def _write_genres(self, dry_run: bool = True) -> bool:
-        values = ";".join(self.genres or [])
-        return self._write_tag(next(iter(self.tag_map.genres), None), values, dry_run)
+    def _write_genres(self, track: LocalTrack, dry_run: bool = True) -> bool:
+        values = ";".join(track.genres or [])
+        return self.write_tag(next(iter(self.tag_map.genres), None), values, dry_run)
 
-    def _write_images(self, dry_run: bool = True) -> bool:
+    def _write_images(self, track: LocalTrack, dry_run: bool = True) -> bool:
         tag_id_prefix = next(iter(self.tag_map.images), None)
 
         updated = False
-        for image_kind, image_link in self.image_links.items():
+        for image_kind, image_link in track.image_links.items():
             image = open_image(image_link)
 
             if not dry_run and tag_id_prefix is not None:
                 image_kind_attr = image_kind.upper().replace(" ", "_")
                 image_type: mutagen.id3.PictureType = getattr(mutagen.id3.PictureType, image_kind_attr)
                 tag_id = f"{tag_id_prefix}:{image_kind}"
 
                 # noinspection PyUnresolvedReferences
-                self._file[tag_id] = mutagen.id3.APIC(
+                self.file[tag_id] = mutagen.id3.APIC(
                     encoding=mutagen.id3.Encoding.UTF8,
                     # desc=image_kind,
                     mime=Image.MIME[image.format],
                     type=image_type,
                     data=get_image_bytes(image)
                 )
 
             image.close()
-            self.has_image = tag_id_prefix is not None or self.has_image
+            track.has_image = tag_id_prefix is not None or track.has_image
             updated = tag_id_prefix is not None
+
         return updated
 
-    def _write_comments(self, dry_run: bool = True) -> bool:
+    def _write_comments(self, track: LocalTrack, dry_run: bool = True) -> bool:
         tag_id_prefix = next(iter(self.tag_map.comments), None)
         self.delete_tags(tags=LocalTrackField.COMMENTS, dry_run=dry_run)
 
-        for comment in self.comments:
+        for comment in track.comments:
             # noinspection PyUnresolvedReferences
             comm = mutagen.id3.COMM(
                 encoding=mutagen.id3.Encoding.UTF8, desc="ID3v1 Comment", lang="eng", text=[comment]
             )
             # noinspection PyUnresolvedReferences
             tag_id = f"{tag_id_prefix}:{comm.desc}:{comm.lang}"
             if not dry_run and tag_id is not None:
-                self._file[tag_id] = comm
+                self.file[tag_id] = comm
 
         return tag_id_prefix is not None
 
-    def _write_uri(self, dry_run: bool = True) -> bool:
+    def _write_uri(self, track: LocalTrack, dry_run: bool = True) -> bool:
         if not self.remote_wrangler:
             return False
 
-        tag_value = self.remote_wrangler.unavailable_uri_dummy if not self.has_uri else self.uri
+        tag_value = self.remote_wrangler.unavailable_uri_dummy if not track.has_uri else track.uri
 
         # if applying URI as comment, clear comments and add manually with custom description
         if self.uri_tag == LocalTrackField.COMMENTS:
             tag_id_prefix = next(iter(self.tag_map.comments), None)
             self.delete_tags(tags=self.uri_tag, dry_run=dry_run)
 
             # noinspection PyUnresolvedReferences
             comm = mutagen.id3.COMM(encoding=mutagen.id3.Encoding.UTF8, lang="eng", desc="URI", text=[tag_value])
             # noinspection PyUnresolvedReferences
             tag_id = f"{tag_id_prefix}:{comm.desc}:{comm.lang}"
             if not dry_run and tag_id is not None:
-                self._file[tag_id] = comm
+                self.file[tag_id] = comm
 
             return tag_id is not None
         else:
             tag_id = next(iter(self.tag_map[self.uri_tag.name.lower()]), None)
-            return self._write_tag(tag_id, tag_value, dry_run)
+            return self.write_tag(tag_id, tag_value, dry_run)
 
-    def delete_tag(self, tag_name: str, dry_run: bool = True) -> bool:
-        removed = False
 
-        tag_ids = self.tag_map[tag_name]
-        if tag_ids is None or len(tag_ids) is None:
-            return removed
+class MP3(LocalTrack[mutagen.mp3.MP3, MP3TagReader, MP3TagWriter]):
 
-        for tag_id_prefix in tag_ids:
-            for mp3_id in list(self._file.keys()).copy():
-                if mp3_id.split(":")[0] == tag_id_prefix and self._file[mp3_id]:
-                    if not dry_run:
-                        del self._file[mp3_id]
-                    removed = True
+    valid_extensions = frozenset({".mp3"})
 
-        return removed
+    # noinspection SpellCheckingInspection
+    #: Map of human-friendly tag name to ID3 tag ids for a given file type
+    tag_map = TagMap(
+        title=["TIT2"],
+        artist=["TPE1"],
+        album=["TALB"],
+        album_artist=["TPE2"],
+        track_number=["TRCK"],
+        track_total=["TRCK"],
+        genres=["TCON"],
+        date=["TDRC", "TDAT", "TDOR"],
+        year=["TYER", "TORY"],
+        bpm=["TBPM"],
+        key=["TKEY"],
+        disc_number=["TPOS"],
+        disc_total=["TPOS"],
+        compilation=["TCMP"],
+        comments=["COMM"],
+        images=["APIC"],
+    )
+
+    @staticmethod
+    def _create_reader(*args, **kwargs):
+        return MP3TagReader(*args, **kwargs)
+
+    @staticmethod
+    def _create_writer(*args, **kwargs):
+        return MP3TagWriter(*args, **kwargs)
```

### Comparing `musify-0.8.1/musify/local/track/utils.py` & `musify-0.9.0/musify/libraries/local/track/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Utilities for operations on :py:class:`LocalTrack` types.
 
 Generally, this will contain global variables representing all supported audio file types
 and a utility function for loading the appropriate :py:class:`LocalTrack` type for a path based on its extension.
 """
-
 from os.path import splitext
 
-from musify.local.exception import InvalidFileType
-from musify.local.track import LocalTrack
-from musify.local.track.flac import FLAC
-from musify.local.track.m4a import M4A
-from musify.local.track.mp3 import MP3
-from musify.local.track.wma import WMA
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
+from musify.file.exception import InvalidFileType
+from musify.libraries.local.track import LocalTrack
+from musify.libraries.local.track.flac import FLAC
+from musify.libraries.local.track.m4a import M4A
+from musify.libraries.local.track.mp3 import MP3
+from musify.libraries.local.track.wma import WMA
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
 
 TRACK_CLASSES = frozenset({FLAC, MP3, M4A, WMA})
 TRACK_FILETYPES = frozenset(filetype for c in TRACK_CLASSES for filetype in c.valid_extensions)
 
 
 def load_track(path: str, remote_wrangler: RemoteDataWrangler = None) -> LocalTrack:
     """
@@ -28,20 +27,12 @@
         This object will be used to check for and validate a URI tag on the file.
         The tag that is used for reading and writing is set by the ``uri_tag`` class attribute on the track object.
         If no ``remote_wrangler`` is given, no URI processing will occur.
     :return: Loaded :py:class:`LocalTrack` object
     :raise InvalidFileType: If the file type is not supported.
     """
     ext = splitext(path)[1].casefold()
+    if ext not in TRACK_FILETYPES:
+        raise InvalidFileType(ext, f"Not an accepted extension. Use only: {', '.join(TRACK_FILETYPES)}")
 
-    if ext in FLAC.valid_extensions:
-        return FLAC(file=path, remote_wrangler=remote_wrangler)
-    elif ext in MP3.valid_extensions:
-        return MP3(file=path, remote_wrangler=remote_wrangler)
-    elif ext in M4A.valid_extensions:
-        return M4A(file=path, remote_wrangler=remote_wrangler)
-    elif ext in WMA.valid_extensions:
-        return WMA(file=path, remote_wrangler=remote_wrangler)
-
-    raise InvalidFileType(
-        ext, f"Not an accepted extension. Use only: {', '.join(TRACK_FILETYPES)}"
-    )
+    cls = next(cls for cls in TRACK_CLASSES if ext in cls.valid_extensions)
+    return cls(file=path, remote_wrangler=remote_wrangler)
```

### Comparing `musify-0.8.1/musify/local/track/wma.py` & `musify-0.9.0/musify/libraries/local/track/wma.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,44 @@
 """
 The WMA implementation of a :py:class:`LocalTrack`.
 """
-
 import struct
 from collections.abc import Collection, Iterable
 from io import BytesIO
 from typing import Any
 
 import mutagen
 import mutagen.asf
 import mutagen.id3
 from PIL import Image, UnidentifiedImageError
 
-from musify.local.file import open_image, get_image_bytes
-from musify.local.track.base.track import LocalTrack
-from musify.shared.core.enum import TagMap
-
-
-class WMA(LocalTrack[mutagen.asf.ASF]):
+from musify.core.enum import TagMap
+from musify.file.image import open_image, get_image_bytes
+from musify.libraries.local.track.tags.reader import TagReader
+from musify.libraries.local.track.tags.writer import TagWriter
+from musify.libraries.local.track.track import LocalTrack
 
-    valid_extensions = frozenset({".wma"})
 
-    #: Map of human-friendly tag name to ID3 tag ids for a given file type
-    tag_map = TagMap(
-        title=["Title"],
-        artist=["Author"],
-        album=["WM/AlbumTitle"],
-        album_artist=["WM/AlbumArtist"],
-        track_number=["WM/TrackNumber"],
-        track_total=["TotalTracks", "WM/TrackNumber"],
-        genres=["WM/Genre"],
-        year=["WM/Year", "WM/OriginalReleaseYear"],
-        bpm=["WM/BeatsPerMinute"],
-        key=["WM/InitialKey"],
-        disc_number=["WM/PartOfSet"],
-        disc_total=["WM/PartOfSet"],
-        compilation=["COMPILATION"],
-        comments=["Description", "WM/Comments"],
-        images=["WM/Picture"],
-    )
+class WMATagReader(TagReader[mutagen.asf.ASF]):
 
-    def _read_tag(self, tag_ids: Iterable[str]) -> list[Any] | None:
+    def read_tag(self, tag_ids: Iterable[str]) -> list[Any] | None:
         # WMA tag values are returned as mutagen.asf._attrs.ASFUnicodeAttribute
         values = []
         for tag_id in tag_ids:
-            value: Collection[mutagen.asf.ASFBaseAttribute] = self._file.get(tag_id)
+            value: Collection[mutagen.asf.ASFBaseAttribute] = self.file.get(tag_id)
             if value is None:
                 # skip null or empty/blank strings
                 continue
 
             values.extend([v.value for v in value if not (isinstance(value, str) and len(value.strip()) == 0)])
 
         return values if len(values) > 0 else None
 
-    def _read_images(self) -> list[Image.Image] | None:
-        values = self._read_tag(self.tag_map.images)
+    def read_images(self) -> list[Image.Image] | None:
+        values = self.read_tag(self.tag_map.images)
         if values is None:
             return
 
         images: list[Image.Image] = []
         for i, value in enumerate(values):
             try:
                 # first attempt to open image from bytes; assumes bytes value refer only to the image data
@@ -86,46 +66,81 @@
             pos += 2
 
             image_data: bytes = value[pos:pos + v_size]
             images.append(Image.open(BytesIO(image_data)))
 
         return images
 
-    def _write_tag(self, tag_id: str | None, tag_value: Any, dry_run: bool = True) -> bool:
-        result = super()._write_tag(tag_id=tag_id, tag_value=tag_value, dry_run=dry_run)
+
+class WMATagWriter(TagWriter[mutagen.asf.ASF]):
+
+    def write_tag(self, tag_id: str | None, tag_value: Any, dry_run: bool = True) -> bool:
+        result = super().write_tag(tag_id=tag_id, tag_value=tag_value, dry_run=dry_run)
         if result is not None:
             return result
 
         if not dry_run:
             if isinstance(tag_value, (list, set, tuple)):
                 if all(isinstance(v, mutagen.asf.ASFByteArrayAttribute) for v in tag_value):
-                    self._file[tag_id] = tag_value
+                    self.file[tag_id] = tag_value
                 else:
-                    self._file[tag_id] = [mutagen.asf.ASFUnicodeAttribute(str(v)) for v in tag_value]
+                    self.file[tag_id] = [mutagen.asf.ASFUnicodeAttribute(str(v)) for v in tag_value]
             else:
-                self._file[tag_id] = mutagen.asf.ASFUnicodeAttribute(str(tag_value))
+                self.file[tag_id] = mutagen.asf.ASFUnicodeAttribute(str(tag_value))
         return True
 
-    def _write_images(self, dry_run: bool = True) -> bool:
+    def _write_images(self, track: LocalTrack, dry_run: bool = True) -> bool:
         tag_id = next(iter(self.tag_map.images), None)
 
         updated = False
         tag_value = []
-        for image_kind, image_link in self.image_links.items():
+        for image_kind, image_link in track.image_links.items():
             image_kind_attr = image_kind.upper().replace(" ", "_")
             image_type: mutagen.id3.PictureType = getattr(mutagen.id3.PictureType, image_kind_attr)
 
             image = open_image(image_link)
             data = get_image_bytes(image)
             tag_data = struct.pack("<bi", image_type, len(data))
             tag_data += Image.MIME[image.format].encode("utf-16") + b"\x00\x00"  # mime
             tag_data += "".encode("utf-16") + b"\x00\x00"  # description
             tag_data += data
 
             tag_value.append(mutagen.asf.ASFByteArrayAttribute(tag_data))
             image.close()
 
         if len(tag_value) > 0:
-            updated = self._write_tag(tag_id, tag_value, dry_run)
+            updated = self.write_tag(tag_id, tag_value, dry_run)
 
-        self.has_image = updated or self.has_image
+        track.has_image = updated or track.has_image
         return updated
+
+
+class WMA(LocalTrack[mutagen.asf.ASF, WMATagReader, WMATagWriter]):
+
+    valid_extensions = frozenset({".wma"})
+
+    #: Map of human-friendly tag name to ID3 tag ids for a given file type
+    tag_map = TagMap(
+        title=["Title"],
+        artist=["Author"],
+        album=["WM/AlbumTitle"],
+        album_artist=["WM/AlbumArtist"],
+        track_number=["WM/TrackNumber"],
+        track_total=["TotalTracks", "WM/TrackNumber"],
+        genres=["WM/Genre"],
+        year=["WM/Year", "WM/OriginalReleaseYear"],
+        bpm=["WM/BeatsPerMinute"],
+        key=["WM/InitialKey"],
+        disc_number=["WM/PartOfSet"],
+        disc_total=["WM/PartOfSet"],
+        compilation=["COMPILATION"],
+        comments=["Description", "WM/Comments"],
+        images=["WM/Picture"],
+    )
+
+    @staticmethod
+    def _create_reader(*args, **kwargs):
+        return WMATagReader(*args, **kwargs)
+
+    @staticmethod
+    def _create_writer(*args, **kwargs):
+        return WMATagWriter(*args, **kwargs)
```

### Comparing `musify-0.8.1/musify/processors/base.py` & `musify-0.9.0/musify/processors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Base classes for all processors in this module. Also contains decorators for use in implementations.
 """
-
 import logging
 from abc import ABCMeta, abstractmethod
 from collections.abc import Mapping, Callable, Collection, Iterable, MutableSequence
 from functools import partial, update_wrapper
-from typing import Any, Self, Optional
+from typing import Any, Optional
 
+from musify.core.printer import PrettyPrinter
+from musify.log.logger import MusifyLogger
 from musify.processors.exception import ProcessorLookupError
-from musify.shared.core.misc import PrettyPrinter
-from musify.shared.logger import MusifyLogger
-from musify.shared.utils import get_user_input, get_max_width, align_string
+from musify.utils import get_user_input, get_max_width, align_string
 
 
 class Processor(PrettyPrinter, metaclass=ABCMeta):
     """Generic base class for processors"""
 
 
 class InputProcessor(Processor, metaclass=ABCMeta):
@@ -46,42 +45,14 @@
         help_text.extend(
             f"\33[1m{align_string(k, max_width=max_width)}\33[0m{': ' + v or ''}" for k, v in options.items()
         )
 
         return "\n\t".join(help_text) + '\n'
 
 
-class ItemProcessor(Processor, metaclass=ABCMeta):
-    """Base object for processing :py:class:`Item` objects"""
-
-
-class MusicBeeProcessor(ItemProcessor):
-    """Base object for processing :py:class:`Item` objects on MusicBee settings"""
-
-    @classmethod
-    def _processor_method_fmt(cls, name: str) -> str:
-        """A custom formatter to apply to the dynamic processor name"""
-        return "_" + cls._pascal_to_snake(name)
-
-    @classmethod
-    @abstractmethod
-    def from_xml(cls, xml: Mapping[str, Any], **kwargs) -> Self:
-        """
-        Initialise object from XML playlist data.
-
-        :param xml: The loaded XML object for this playlist.
-        """
-        raise NotImplementedError
-
-    @abstractmethod
-    def to_xml(self, **kwargs) -> Mapping[str, Any]:
-        """Export this object's settings to a map ready for export to an XML playlist file."""
-        raise NotImplementedError
-
-
 # noinspection PyPep8Naming,SpellCheckingInspection
 class dynamicprocessormethod:
     """
     Decorator for methods on a class decorated with the :py:func:`processor` decorator
 
     This assigns the method a processor method which can be dynamically called by the processor class.
     Optionally, provide a list of alternative names from which this processor method can also be called.
@@ -127,14 +98,19 @@
     __processormethods__: frozenset[str] = frozenset()
 
     @property
     def processor_methods(self) -> frozenset[str]:
         """String representation of the current processor name of this object"""
         return frozenset(self._processor_method_fmt(name) for name in self.__processormethods__)
 
+    @classmethod
+    def _processor_method_fmt(cls, name: str) -> str:
+        """A custom formatter to apply to the dynamic processor name"""
+        return name
+
     def __new__(cls, *_, **__):
         processor_methods = list(cls.__processormethods__)
 
         for method in cls.__dict__.copy().values():
             if not isinstance(method, dynamicprocessormethod):
                 continue
 
@@ -150,19 +126,14 @@
 
         cls.__processormethods__ = frozenset(processor_methods)
         return super().__new__(cls)
 
     def __init__(self):
         self._processor_name: str | None = None
 
-    @classmethod
-    def _processor_method_fmt(cls, name: str) -> str:
-        """A custom formatter to apply to the dynamic processor name"""
-        return name
-
     def _set_processor_name(self, value: str | None, fail_on_empty: bool = True):
         """Verifies and sets the condition name"""
         if value is None:
             if not fail_on_empty:
                 self._processor_name = None
                 return
             raise ProcessorLookupError("No condition given")
@@ -199,15 +170,15 @@
         """Apply this filter's settings to the given values"""
         raise NotImplementedError
 
     @property
     def transform(self) -> Callable[[Any], Any]:
         """
         Transform the input ``value`` to the value that should be used when comparing against this filter's settings
-        Simply returns the given ``value`` at baseline unless overriden.
+        Simply returns the given ``value`` at baseline unless overridden.
         """
         return self._transform
 
     @transform.setter
     def transform(self, transformer: Callable[[Any], Any]):
         self._transform = transformer
```

### Comparing `musify-0.8.1/musify/processors/download.py` & `musify-0.9.0/musify/processors/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+"""
+Processor that helps user download songs from collections based on given configuration.
+"""
 import re
 from collections.abc import Iterable, Collection
 from itertools import batched
 from typing import Any
 from webbrowser import open as webopen
 
-from musify.processors.base import InputProcessor, ItemProcessor
-from musify.shared.core.base import Item
-from musify.shared.core.collection import ItemCollection
-from musify.shared.core.enum import Field, Fields
-from musify.shared.exception import MusifyEnumError
-from musify.shared.types import UnitIterable
-from musify.shared.utils import to_collection
+from musify.core.base import MusifyItem
+from musify.core.enum import Field, Fields
+from musify.exception import MusifyEnumError
+from musify.libraries.core.collection import MusifyCollection
+from musify.processors.base import InputProcessor
+from musify.types import UnitIterable
+from musify.utils import to_collection
 
 
-class ItemDownloadHelper(InputProcessor, ItemProcessor):
+class ItemDownloadHelper(InputProcessor):
     """
     Runs operations for helping the user to download items from given collections.
 
     :param urls: The template URLs for websites to open queries for.
         The given sites should contain exactly 1 '{}' placeholder into which the processor can place
         a query for the item being searched. e.g. *bandcamp.com/search?q={}&item_type=t*
     :param fields: The default fields to take from an item for use as the query string when initially opening sites.
@@ -29,43 +32,43 @@
 
         self.urls: list[str] = to_collection(urls, list)
         if fields == Fields.ALL or Fields.ALL in to_collection(fields, set):
             fields = Fields.all()
         self.fields: list[Field] = to_collection(fields, list)
         self.interval = interval
 
-    def __call__(self, collections: UnitIterable[ItemCollection]) -> None:
-        self.open_sites(collections=collections)
+    def __call__(self, *args, **kwargs) -> None:
+        return self.open_sites(*args, **kwargs)
 
-    def open_sites(self, collections: UnitIterable[ItemCollection]) -> None:
+    def open_sites(self, collections: UnitIterable[MusifyCollection]) -> None:
         """
         Run the download helper.
 
         Opens the formatted ``urls`` for each item in all given collections in the user's browser.
         """
-        if isinstance(collections, ItemCollection):
+        if isinstance(collections, MusifyCollection):
             items = collections.items
         else:
             items = [item for coll in collections for item in coll]
 
         pages_total = (len(items) // self.interval) + (len(items) % self.interval > 0)
         for page, items in enumerate(batched(items, self.interval), 1):
             not_queried = self._open_sites_for_items(items=items, fields=self.fields)
             self._pause(items=items, not_queried=not_queried, page=page, total=pages_total)
 
-    def _open_sites_for_items(self, items: Iterable[Item], fields: Iterable[Field]) -> list[Item]:
+    def _open_sites_for_items(self, items: Iterable[MusifyItem], fields: Iterable[Field]) -> list[MusifyItem]:
         not_queried = []
         for item in items:
             queried = self._open_sites_for_item(item=item, fields=fields)
             if not queried:
                 not_queried.append(item)
 
         return not_queried
 
-    def _open_sites_for_item(self, item: Item, fields: Iterable[Field]) -> bool:
+    def _open_sites_for_item(self, item: MusifyItem, fields: Iterable[Field]) -> bool:
         query_parts = []
         for field in fields:
             field_name = field.name.lower()
             if not hasattr(item, field_name) or getattr(item, field_name) is None:
                 continue
 
             value = getattr(item, field_name)
@@ -80,15 +83,15 @@
 
         self.logger.debug(f"Opening {len(self.urls)} URLs with query: {query}")
         for url in self.urls:
             webopen(url.format(query))
 
         return True
 
-    def _pause(self, items: Iterable[Item], not_queried: Collection[Item], page: int, total: int):
+    def _pause(self, items: Iterable[MusifyItem], not_queried: Collection[MusifyItem], page: int, total: int):
         opened = len(self.urls) * (self.interval - len(not_queried))
         not_opened = f" - Could not open sites for {len(not_queried)} items. " if not_queried else ". "
         valid_fields = [
             field.name.lower() for field in Fields.all()
             if any(
                 hasattr(item, field.name.lower()) and getattr(item, field.name.lower()) is not None for item in items
             )
```

### Comparing `musify-0.8.1/musify/processors/exception.py` & `musify-0.9.0/musify/processors/exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,39 @@
 """
 Exceptions relating to processor operations.
 """
-
-from musify.shared.exception import MusifyError
+from musify.exception import MusifyError
 
 
 class ProcessorError(MusifyError):
     """Exception raised for errors related to processors."""
 
 
 class ProcessorLookupError(ProcessorError):
     """Exception raised when processor name given is not valid."""
 
 
 class ComparerError(ProcessorError):
     """Exception raised for errors related to :py:class:`Comparer` settings."""
 
 
+class LimiterProcessorError(ProcessorError):
+    """Exception raised for errors related to :py:class:`ItemLimiter` logic."""
+
+
+class MatcherProcessorError(ProcessorError):
+    """Exception raised for errors related to :py:class:`ItemMatcher` logic."""
+
+
+class SorterProcessorError(ProcessorError):
+    """Exception raised for errors related to :py:class:`ItemSorter` logic."""
+
+
 class TimeMapperError(ProcessorError):
     """Exception raised for errors related to :py:class:`TimeMapper` logic."""
 
 
 ###########################################################################
 ## Filter errors
 ###########################################################################
 class FilterError(ProcessorError):
     """Exception raised for errors related to :py:class:`Filter` logic."""
-
-
-###########################################################################
-## Item processor errors
-###########################################################################
-class ItemProcessorError(ProcessorError):
-    """Exception raised for errors related to :py:class:`ItemProcessor` logic."""
-
-
-class ItemLimiterError(ItemProcessorError):
-    """Exception raised for errors related to :py:class:`ItemLimiter` logic."""
-
-
-class ItemMatcherError(ItemProcessorError):
-    """Exception raised for errors related to :py:class:`ItemMatcher` logic."""
-
-
-class ItemSorterError(ItemProcessorError):
-    """Exception raised for errors related to :py:class:`ItemSorter` logic."""
```

### Comparing `musify-0.8.1/musify/processors/filter.py` & `musify-0.9.0/musify/processors/filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """
 Processors that filter down objects and data types based on some given configuration.
 """
-
 from __future__ import annotations
 
 from collections.abc import Collection, Sequence, Mapping
 from typing import Any, Self
 
+from musify.core.base import MusifyObject
 from musify.processors.base import Filter, FilterComposite
 from musify.processors.compare import Comparer
-from musify.shared.core.base import Nameable
 
 
-class FilterDefinedList[T: str | Nameable](Filter[T], Collection[T]):
+class FilterDefinedList[T: str | MusifyObject](Filter[T], Collection[T]):
 
     __slots__ = ("values",)
 
     @property
     def ready(self):
         return len(self.values) > 0
 
     def __init__(self, values: Collection[T] = (), *_, **__):
         super().__init__()
         #: The values to include when processing for this filter
         self.values: Collection[T] = values
 
-    def __call__(self, values: Collection[T] | None = None, *_, **__) -> Collection[T]:
-        return self.process(values=values)
+    def __call__(self, *args, **kwargs) -> Collection[T]:
+        return self.process(*args, **kwargs)
 
     def process(self, values: Collection[T] | None = None, *_, **__) -> Collection[T]:
         """Returns all ``values`` that match this filter's settings"""
         if self.ready:
             matches = [value for value in values if self.transform(value) in self.values]
             if isinstance(self.values, Sequence):
                 matches = sorted((self.values.index(self.transform(match)), match) for match in matches)
@@ -47,15 +46,15 @@
     def __len__(self):
         return len(self.values)
 
     def __contains__(self, item: Any):
         return item in self.values
 
 
-class FilterComparers[T: str | Nameable](Filter[T]):
+class FilterComparers[T: str | MusifyObject](Filter[T]):
 
     __slots__ = ("comparers", "match_all")
 
     @property
     def ready(self):
         return len(self.comparers) > 0
 
@@ -73,16 +72,16 @@
         #: The comparers to use when processing for this filter
         #: When a mapping with other :py:class:`FilterComparers` is given,
         #: will apply this sub-filter to all parent filters when processing
         self.comparers: Mapping[Comparer, tuple[bool, Self]] = comparers
         #: When true, only include those items that match on all comparers
         self.match_all: bool = match_all
 
-    def __call__(self, values: Collection[T], reference: T | None = None, *_, **__) -> Collection[T]:
-        return self.process(values=values, reference=reference)
+    def __call__(self, *args, **kwargs) -> Collection[T]:
+        return self.process(*args, **kwargs)
 
     def process(self, values: Collection[T], reference: T | None = None, *_, **__) -> Collection[T]:
         if not self.ready:
             return values
 
         def run_comparer(c: Comparer, v: T) -> bool:
             """Run the comparer ``c`` for the given value ``v``"""
@@ -126,16 +125,16 @@
     def __init__(self, include: U, exclude: V, *_, **__):
         super().__init__(include, exclude)
         #: The filter that, when processed, returns items to include
         self.include: U = include
         #: The filter that, when processed, returns items to exclude
         self.exclude: V = exclude
 
-    def __call__(self, values: Collection[T], *_, **__) -> list[T]:
-        return self.process(values=values)
+    def __call__(self, *args, **kwargs) -> list[T]:
+        return self.process(*args, **kwargs)
 
     def process(self, values: Collection[T], *_, **__) -> list[T]:
         """Filter down ``values`` that match this filter's settings from"""
         values = self.include.process(values) if self.include.ready else values
         exclude = self.exclude.process(values) if self.exclude.ready else ()
         return [v for v in values if v not in exclude]
```

### Comparing `musify-0.8.1/musify/processors/limit.py` & `musify-0.9.0/musify/processors/limit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 Processor that limits the items in a given collection of items
 """
-
-from collections.abc import Collection, Mapping
+from collections.abc import Collection, MutableSequence
 from functools import reduce
 from operator import mul
 from random import shuffle
-from typing import Any, Self
 
-from musify.local.file import File
-from musify.processors.base import DynamicProcessor, MusicBeeProcessor, dynamicprocessormethod
-from musify.processors.exception import ItemLimiterError
+from musify.core.base import MusifyItem
+from musify.core.enum import MusifyEnum, Fields
+from musify.file.base import File
+from musify.libraries.core.object import Track
+from musify.processors.base import DynamicProcessor, dynamicprocessormethod
+from musify.processors.exception import LimiterProcessorError
 from musify.processors.sort import ItemSorter
-from musify.shared.core.base import Item
-from musify.shared.core.enum import MusifyEnum, Fields
-from musify.shared.core.object import Track
 
 
 class LimitType(MusifyEnum):
     """Represents the possible limit types to apply when filtering a playlist."""
     ITEMS = 0
     ALBUMS = 1
 
@@ -31,15 +29,15 @@
     BYTES = 20
     KILOBYTES = 21
     MEGABYTES = 22
     GIGABYTES = 23
     TERABYTES = 24
 
 
-class ItemLimiter(MusicBeeProcessor, DynamicProcessor):
+class ItemLimiter(DynamicProcessor):
     """
     Sort items in-place based on given conditions.
 
     :param limit: The number of items to limit to. A value of 0 applies no limiting.
     :param on: The type to limit on e.g. items, albums, minutes.
     :param sorted_by: When limiting, sort the collection of items by this function first.
     :param allowance: When limiting on bytes or length, add this extra allowance factor to
@@ -50,37 +48,23 @@
         However, with an allowance of say 1.33 it will as the max limit for this comparison becomes 30 * 1.33 = 40.
         Now, with 32 minutes worth of songs in the final playlist, the limit is >30 minutes and the limiter stops
         processing.
     """
 
     __slots__ = ("limit_max", "kind", "allowance")
 
+    @classmethod
+    def _processor_method_fmt(cls, name: str) -> str:
+        return "_" + cls._pascal_to_snake(name)
+
     @property
     def limit_sort(self) -> str | None:
         """String representation of the sorting method to use before limiting"""
         return self._processor_name.lstrip("_")
 
-    @classmethod
-    def from_xml(cls, xml: Mapping[str, Any], **__) -> Self | None:
-        conditions: Mapping[str, str] = xml["SmartPlaylist"]["Source"]["Limit"]
-        if conditions["@Enabled"] != "True":
-            return
-        # filter_duplicates = conditions["@FilterDuplicates"] == "True"
-
-        # MusicBee appears to have some extra allowance on time and byte limits of ~1.25
-        return cls(
-            limit=int(conditions["@Count"]),
-            on=LimitType.from_name(conditions["@Type"])[0],
-            sorted_by=conditions["@SelectedBy"],
-            allowance=1.25
-        )
-
-    def to_xml(self, **kwargs) -> Mapping[str, Any]:
-        raise NotImplementedError
-
     def __init__(
             self,
             limit: int = 0,
             on: LimitType = LimitType.ITEMS,
             sorted_by: str | None = None,
             allowance: float = 1.0,
     ):
@@ -92,18 +76,18 @@
         self.kind = on
         #: When limiting on bytes or length, add this extra allowance factor to
         #: the max size limit on comparison.
         self.allowance = allowance
 
         self._set_processor_name(sorted_by, fail_on_empty=False)
 
-    def __call__[T: Item](self, items: list[T], ignore: Collection[T] = ()) -> None:
-        return self.limit(items=items, ignore=ignore)
+    def __call__(self, *args, **kwargs) -> None:
+        return self.limit(*args, **kwargs)
 
-    def limit[T: Item](self, items: list[T], ignore: Collection[T] = ()) -> None:
+    def limit[T: MusifyItem](self, items: list[T], ignore: Collection[T] = ()) -> None:
         """
         Limit ``items`` in-place based on set conditions.
 
         :param items: The list of items to limit.
         :param ignore: list of items to ignore when limiting. i.e. keep them in the list regardless.
         """
         if len(items) == 0 or self.limit_max == 0:
@@ -117,95 +101,109 @@
             items_ignore = [item for item in items if item in ignore]
             items.clear()
             items.extend(items_ignore)
         else:  # make a copy of the given items and clear the original list
             items_limit = [t for t in items]
             items.clear()
 
-        if self.kind == LimitType.ITEMS:  # limit on items
+        if self.kind == LimitType.ITEMS:
             items.extend(items_limit[:self.limit_max])
-        elif self.kind == LimitType.ALBUMS:  # limit on albums
-            seen_albums = []
-            for item in items_limit:
-                if not isinstance(item, Track):
-                    ItemLimiterError("In order to limit on Album, all items must be of type 'Track'")
-
-                if len(seen_albums) < self.limit_max and item.album not in seen_albums:
-                    # album limit not yet reached
-                    seen_albums.append(item.album)
-                if item.album in seen_albums:
-                    items.append(item)
-        else:  # limit on duration or size
-            count = 0
-            for item in items_limit:
-                value = self._convert(item)
-                if count + value <= self.limit_max * self.allowance:  # limit not yet reached
-                    items.append(item)
-                    count += value
-                if count > self.limit_max:  # limit reached
-                    break
+        elif self.kind == LimitType.ALBUMS:
+            items.extend(self._limit_on_albums(items_limit))
+        else:
+            items.extend(self._limit_on_numeric(items_limit))
+
+    def _limit_on_albums[T: MusifyItem](self, items: MutableSequence[T]) -> list[T]:
+        seen_albums = []
+        result = []
+
+        for item in items:
+            if not isinstance(item, Track):
+                LimiterProcessorError("In order to limit on Album, all items must be of type 'Track'")
+
+            if len(seen_albums) < self.limit_max and item.album not in seen_albums:
+                # album limit not yet reached
+                seen_albums.append(item.album)
+            if item.album in seen_albums:
+                result.append(item)
+
+        return result
+
+    def _limit_on_numeric[T: MusifyItem](self, items: MutableSequence[T]) -> list[T]:
+        count = 0
+        result = []
+
+        for item in items:
+            value = self._convert(item)
+            if count + value <= self.limit_max * self.allowance:  # limit not yet reached
+                result.append(item)
+                count += value
+            if count > self.limit_max:  # limit reached
+                break
+
+        return result
 
-    def _convert(self, item: Item) -> float:
+    def _convert(self, item: MusifyItem) -> float:
         """
         Convert units for item length or size and return the value.
 
         :raise ItemLimiterError: When the given limit type cannot be found
         """
         if 10 < self.kind.value < 20:
-            if not hasattr(item, "length"):
-                raise ItemLimiterError("The given item cannot be limited on length as it does not have a length.")
+            if getattr(item, "length", None) is None:  # TODO: there should be a better way of handling this...
+                raise LimiterProcessorError("The given item cannot be limited on length as it does not have a length.")
 
             factors = (1, 60, 60, 24, 7)[:self.kind.value % 10]
             # noinspection PyUnresolvedReferences
             return item.length / reduce(mul, factors, 1)
 
         elif 20 <= self.kind.value < 30:
             if not isinstance(item, File):
-                raise ItemLimiterError("The given item cannot be limited on bytes as it is not a file.")
+                raise LimiterProcessorError("The given item cannot be limited on bytes as it is not a file.")
 
             bytes_scale = 1000
             return item.size / (bytes_scale ** (self.kind.value % 10))
 
         else:
-            raise ItemLimiterError(f"Unrecognised LimitType: {self.kind}")
+            raise LimiterProcessorError(f"Unrecognised LimitType: {self.kind}")
 
     @dynamicprocessormethod
-    def _random(self, items: list[Item]) -> None:
+    def _random(self, items: MutableSequence[MusifyItem]) -> None:
         shuffle(items)
 
     @dynamicprocessormethod
-    def _highest_rating(self, items: list[Item]) -> None:
+    def _highest_rating(self, items: list[MusifyItem]) -> None:
         ItemSorter.sort_by_field(items, Fields.RATING, reverse=True)
 
     @dynamicprocessormethod
-    def _lowest_rating(self, items: list[Item]) -> None:
+    def _lowest_rating(self, items: list[MusifyItem]) -> None:
         ItemSorter.sort_by_field(items, Fields.RATING)
 
     @dynamicprocessormethod
-    def _most_recently_played(self, items: list[Item]) -> None:
+    def _most_recently_played(self, items: list[MusifyItem]) -> None:
         ItemSorter.sort_by_field(items, Fields.LAST_PLAYED, reverse=True)
 
     @dynamicprocessormethod
-    def _least_recently_played(self, items: list[Item]) -> None:
+    def _least_recently_played(self, items: list[MusifyItem]) -> None:
         ItemSorter.sort_by_field(items, Fields.LAST_PLAYED)
 
     @dynamicprocessormethod
-    def _most_often_played(self, items: list[Item]) -> None:
+    def _most_often_played(self, items: list[MusifyItem]) -> None:
         ItemSorter.sort_by_field(items, Fields.PLAY_COUNT, reverse=True)
 
     @dynamicprocessormethod
-    def _least_often_played(self, items: list[Item]) -> None:
+    def _least_often_played(self, items: list[MusifyItem]) -> None:
         ItemSorter.sort_by_field(items, Fields.PLAY_COUNT)
 
     @dynamicprocessormethod
-    def _most_recently_added(self, items: list[Item]) -> None:
+    def _most_recently_added(self, items: list[MusifyItem]) -> None:
         ItemSorter.sort_by_field(items, Fields.DATE_ADDED, reverse=True)
 
     @dynamicprocessormethod
-    def _least_recently_added(self, items: list[Item]) -> None:
+    def _least_recently_added(self, items: list[MusifyItem]) -> None:
         ItemSorter.sort_by_field(items, Fields.DATE_ADDED)
 
     def as_dict(self):
         return {
             "on": self.kind,
             "limit": self.limit_max,
             "sorted_by": self.limit_sort,
```

### Comparing `musify-0.8.1/musify/processors/match.py` & `musify-0.9.0/musify/processors/match.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
 Processor that matches objects and data types based on given configuration.
 """
-
 import inspect
 import logging
 import re
 from collections.abc import Iterable, Callable, MutableSequence
+from concurrent.futures import ThreadPoolExecutor, Future, Executor
 from dataclasses import dataclass, field
 from typing import Any
 
-from musify.processors.base import ItemProcessor
-from musify.shared.core.base import Nameable, NameableTaggableMixin, Taggable
-from musify.shared.core.collection import ItemCollection
-from musify.shared.core.enum import TagField, TagFields as Tag, ALL_TAG_FIELDS
-from musify.shared.core.misc import PrettyPrinter
-from musify.shared.core.object import Track, Album
-from musify.shared.logger import MusifyLogger
-from musify.shared.types import UnitIterable
-from musify.shared.utils import limit_value, to_collection
+from musify.core.base import MusifyObject
+from musify.core.enum import TagField, TagFields as Tag, ALL_TAG_FIELDS
+from musify.core.printer import PrettyPrinter
+from musify.libraries.core.collection import MusifyCollection
+from musify.log.logger import MusifyLogger
+from musify.processors.base import Processor
+from musify.types import UnitIterable
+from musify.utils import limit_value, to_collection
 
 
 @dataclass
 class CleanTagConfig(PrettyPrinter):
     """Config for processing string-type tag values before matching with :py:class:`ItemMatcher`"""
     #: The name of the tag to clean.
     tag: TagField
@@ -37,15 +36,15 @@
             "tag": self.tag.name.lower(),
             "remove": [value for value in self.remove],
             "split": [value for value in self.split],
             "preprocess": self.preprocess is not None,
         }
 
 
-class ItemMatcher(ItemProcessor):
+class ItemMatcher(Processor):
     """Matches source items/collections to given result(s)."""
 
     __slots__ = ("logger",)
 
     #: A set of words to search for in tag values that identify the item as being a karaoke item.
     karaoke_tags = {"karaoke", "backing", "instrumental"}
     #: A difference in years of this value gives a score of 0 for the :py:meth:`match_year` algorithm.
@@ -67,60 +66,63 @@
         CleanTagConfig(tag=Tag.ALBUM, remove={"ep"}, preprocess=lambda x: x.split('-')[0])
     )
 
     # config for name score reduction
     #: A set of words to check for when applying name score reduction logic.
     #:
     #: If a word from this list is present in the name of the result to score against
-    #: but not in the source :py:class:`Item`, apply the ``reduce_name_score_factor`` to reduce its score.
+    #: but not in the source :py:class:`MusifyObject`, apply the ``reduce_name_score_factor`` to reduce its score.
     #: This set is always combined with the ``karaoke_tags``.
     reduce_name_score_on = {"live", "demo", "acoustic"}
     #: The factor to apply to a name score when a word from ``reduce_name_score_on``
-    #: is found in the result but not in the source :py:class:`Item`.
+    #: is found in the result but not in the source :py:class:`MusifyObject`.
     reduce_name_score_factor = 0.5
 
     def __init__(self):
         super().__init__()
 
         # noinspection PyTypeChecker
         #: The :py:class:`MusifyLogger` for this  object
         self.logger: MusifyLogger = logging.getLogger(__name__)
 
-    def _log_padded(self, log: MutableSequence[str], pad: str = ' ') -> None:
-        """Wrapper for logging lists in a correctly aligned format"""
-        log[0] = pad * 3 + ' ' + (log[0] if log[0] else "unknown")
-        self.logger.debug(" | ".join(log))
+    def log_messages(self, messages: MutableSequence[str], pad: str = ' ') -> None:
+        """
+        Log lists of ``messages`` in a uniform aligned format with a given ``pad`` character.
 
-    def _log_algorithm(self, source: Nameable, extra: Iterable[str] = ()) -> None:
-        """Wrapper for initially logging an algorithm in a correctly aligned format"""
+        Convenience function for ensuring consistent log format for results of operations of this class
+        and any other classes which use this class.
+        """
+        messages[0] = pad * 3 + ' ' + (messages[0] if messages[0] else "unknown")
+        self.logger.debug(" | ".join(messages))
+
+    def _log_algorithm(self, source: MusifyObject, extra: Iterable[str] = ()) -> None:
+        """Wrapper for initially logging an algorithm in a uniform aligned format"""
         algorithm = inspect.stack()[1][0].f_code.co_name.upper().lstrip("_").replace("_", " ")
         log = [source.name, algorithm]
         if extra:
             log.extend(extra)
-        self._log_padded(log, pad='>')
+        self.log_messages(log, pad='>')
 
-    def _log_test[T: (Track, Album)](
-            self, source: Nameable, result: T, test: Any, extra: Iterable[str] = ()
-    ) -> None:
-        """Wrapper for initially logging a test result in a correctly aligned format"""
+    def _log_test[T: MusifyObject](self, source: T, result: T, test: Any, extra: Iterable[str] = ()) -> None:
+        """Wrapper for initially logging a test result in a uniform aligned format"""
         algorithm = inspect.stack()[1][0].f_code.co_name.replace("match", "").upper().lstrip("_").replace("_", " ")
         log_result = f"> Testing URI: {result.uri}" if hasattr(result, "uri") else "> Test failed"
         log = [source.name, log_result, f"{algorithm:<10}={test:<5}"]
         if extra:
             log.extend(extra)
-        self._log_padded(log)
+        self.log_messages(log)
 
-    def _log_match[T: (Track, Album)](self, source: Nameable, result: T, extra: Iterable[str] = ()) -> None:
+    def _log_match[T: MusifyObject](self, source: T, result: T, extra: Iterable[str] = ()) -> None:
         """Wrapper for initially logging a match in a correctly aligned format"""
         log = [source.name, f"< Matched URI: {result.uri}"]
         if extra:
             log.extend(extra)
-        self._log_padded(log, pad='<')
+        self.log_messages(log, pad='<')
 
-    def clean_tags(self, source: NameableTaggableMixin) -> None:
+    def clean_tags(self, source: MusifyObject) -> None:
         """
         Clean tags on the input item and assign to its ``clean_tags`` attribute. Used for better matching/searching.
         Clean by removing words, and only taking phrases before a certain word e.g. 'featuring', 'part'.
         Cleaning config for string-type tags is set in ``_clean_tags_config``.
 
         :param source: The base object with tags to clean.
         """
@@ -156,136 +158,122 @@
 
         source.clean_tags[Tag.LENGTH] = getattr(source, Tag.LENGTH.name.lower(), None)
         source.clean_tags[Tag.YEAR] = getattr(source, Tag.YEAR.name.lower(), None)
 
     ###########################################################################
     ## Conditions
     ###########################################################################
-    def match_not_karaoke[T: (Track, Album)](self, source: T, result: T) -> int:
+    def match_not_karaoke[T: MusifyObject](self, source: T, result: T) -> int:
         """Checks if a result is not a karaoke item that is either 0 when item is karaoke or 1 when not karaoke."""
         def is_karaoke(*values: str) -> bool:
             """Check if the words in the given ``values`` match any word in ``karaoke_tags``"""
             values = {v for value in values for v in value.casefold().split()}
             karaoke = any(word.casefold() in values for word in self.karaoke_tags)
             self._log_test(source=source, result=result, test=karaoke, extra=[f"{self.karaoke_tags} -> {values}"])
             return karaoke
 
-        if is_karaoke(result.name):  # title/album name
+        if is_karaoke(result.name):
             return 0
-        if is_karaoke(result.artist):  # artists
+        if is_karaoke(result.artist):
             return 0
-        if is_karaoke(result.album):  # album
+        if is_karaoke(result.album):
             return 0
         return 1
 
-    def match_name[T: (Track, Album)](self, source: T, result: T) -> float:
+    def match_name[T: MusifyObject](self, source: T, result: T) -> float:
         """Match on names and return a score between 0-1. Score=0 when either value is None."""
         score = 0
-        source_val = source.clean_tags[Tag.NAME]
-        result_val = result.clean_tags[Tag.NAME]
+        source_val = source.clean_tags.get(Tag.NAME)
+        result_val = result.clean_tags.get(Tag.NAME)
 
         if source_val and result_val:
             score = sum(word in result_val for word in source_val.split()) / len(source_val.split())
 
             # reduce a score if certain keywords are present in result and not source
             reduce_on = self.reduce_name_score_on | self.karaoke_tags
             reduce_on = {word.casefold() for word in reduce_on}
             if any(word in result.name.casefold() and word not in source.name.casefold() for word in reduce_on):
                 score = max(score * self.reduce_name_score_factor, 0)
 
         self._log_test(source=source, result=result, test=round(score, 2), extra=[f"{source_val} -> {result_val}"])
         return score
 
-    def match_artist[T: (Track, Album)](self, source: T, result: T) -> float:
+    def match_artist[T: MusifyObject](self, source: T, result: T) -> float:
         """
         Match on artists and return a score between 0-1. Score=0 when either value is None.
         When many artists are present, a scale factor is applied to the score of matches on subsequent artists.
         i.e. match on artist 1 is scaled by 1, match on artist 2 is scaled by 1/2,
         match on artist 3 is scaled by 1/3 etc.
         """
         score = 0
-        source_val = source.clean_tags[Tag.ARTIST]
-        result_val = result.clean_tags[Tag.ARTIST]
+        source_val = source.clean_tags.get(Tag.ARTIST)
+        result_val = result.clean_tags.get(Tag.ARTIST)
 
         if not source_val or not result_val:
             self._log_test(source=source, result=result, test=score, extra=[f"{source_val} -> {result_val}"])
             return score
 
-        artists_source = source_val.replace(Taggable.tag_sep, " ")
-        artists_result = result_val.split(Taggable.tag_sep)
+        artists_source = source_val.replace(MusifyObject.tag_sep, " ")
+        artists_result = result_val.split(MusifyObject.tag_sep)
 
         for i, artist in enumerate(artists_result, 1):
             score += (sum(word in artists_source for word in artist.split()) / len(artists_source.split())) * (1 / i)
         self._log_test(source=source, result=result, test=round(score, 2), extra=[f"{source_val} -> {result_val}"])
         return score
 
-    def match_album[T: (Track, Album)](self, source: T, result: T) -> float:
+    def match_album[T: MusifyObject](self, source: T, result: T) -> float:
         """Match on album and return a score between 0-1. Score=0 when either value is None."""
         score = 0
-        source_val = source.clean_tags[Tag.ALBUM]
-        result_val = result.clean_tags[Tag.ALBUM]
+
+        source_val = source.clean_tags.get(Tag.ALBUM)
+        result_val = result.clean_tags.get(Tag.ALBUM)
 
         if source_val and result_val:
             score = sum(word in result_val for word in source_val.split()) / len(source_val.split())
 
         self._log_test(source=source, result=result, test=round(score, 2), extra=[f"{source_val} -> {result_val}"])
         return score
 
-    def match_length[T: (Track, Album)](self, source: T, result: T) -> float:
+    def match_length[T: MusifyObject](self, source: T, result: T) -> float:
         """Match on length and return a score between 0-1. Score=0 when either value is None."""
         score = 0
-        source_val = source.clean_tags[Tag.LENGTH]
-        result_val = result.clean_tags[Tag.LENGTH]
+        source_val = source.clean_tags.get(Tag.LENGTH)
+        result_val = result.clean_tags.get(Tag.LENGTH)
 
         if source_val and result_val:
             score = max((source_val - abs(source_val - result_val)), 0) / source_val
 
         extra = [f"{round(source_val, 2) if source_val else None} -> {round(result_val, 2) if result_val else None}"]
         self._log_test(source=source, result=result, test=round(score, 2), extra=extra)
         return score
 
-    def match_year[T: (Track, Album)](self, source: T, result: T) -> float:
+    def match_year[T: MusifyObject](self, source: T, result: T) -> float:
         """
         Match on year and return a score between 0-1. Score=0 when either value is None.
         Matches within ``year_range`` years on a 0-1 scale where 1 is the exact same year
         and 0 is a difference in year greater that ``year_range``.
         User may modify this max range via the ``year_range`` class attribute.
         """
         score = 0
-        source_val = source.clean_tags[Tag.YEAR]
-        result_val = result.clean_tags[Tag.YEAR]
+        source_val = source.clean_tags.get(Tag.YEAR)
+        result_val = result.clean_tags.get(Tag.YEAR)
 
         if source_val and result_val:
             score = max((self.year_range - abs(source_val - result_val)), 0) / self.year_range
 
         self._log_test(source=source, result=result, test=round(score, 2), extra=[f"{source_val} -> {result_val}"])
         return score
 
     ###########################################################################
     ## Score match
     ###########################################################################
-    def __call__[T: (Track, Album)](
-            self,
-            source: T,
-            results: Iterable[T],
-            min_score: float = 0.1,
-            max_score: float = 0.8,
-            match_on: UnitIterable[TagField] = ALL_TAG_FIELDS,
-            allow_karaoke: bool = False,
-    ) -> T | None:
-        return self.match(
-            source=source,
-            results=results,
-            min_score=min_score,
-            max_score=max_score,
-            match_on=match_on,
-            allow_karaoke=allow_karaoke
-        )
+    def __call__[T: MusifyObject](self, *args, **kwargs) -> T | None:
+        return self.match(*args, **kwargs)
 
-    def match[T: (Track, Album)](
+    def match[T: MusifyObject](
             self,
             source: T,
             results: Iterable[T],
             min_score: float = 0.1,
             max_score: float = 0.8,
             match_on: UnitIterable[TagField] = ALL_TAG_FIELDS,
             allow_karaoke: bool = False,
@@ -312,127 +300,141 @@
         match_on_filtered = set()
         for match_field in to_collection(match_on, set):
             if match_field == Tag.ALL:
                 match_on_filtered.update(match_field.all())
             else:
                 match_on_filtered.add(match_field)
 
-        score, result = self._score(
-            source=source, results=results, max_score=max_score, match_on=match_on_filtered, allow_karaoke=allow_karaoke
-        )
+        max_score = limit_value(max_score, floor=0.01, ceil=1.0)
+        self._log_algorithm(source=source, extra=[f"max_score={max_score}"])
+
+        with ThreadPoolExecutor(thread_name_prefix="matcher") as executor:
+            scores = self._score(
+                source=source,
+                results=results,
+                executor=executor,
+                match_on=match_on_filtered,
+                allow_karaoke=allow_karaoke
+            )
+
+        result = None
+        best_score = 0
+
+        def sum_nested_scores(futures: list[list[Future[float]]]) -> float:
+            """Sum the scores from a given list of nested Futures"""
+            scores_summed = [sum(score.result() for score in nested) / len(nested) for nested in futures]
+            return sum(scores_summed) / len(scores_summed)
+
+        for result, result_scores in scores:
+            result_scores = [
+                sum_nested_scores(score) if isinstance(score, list) else score.result()
+                for score in result_scores.values()
+            ]
+            best_score = sum(result_scores) / len(result_scores)
+            if best_score > max_score:
+                break
 
         min_score = limit_value(min_score, floor=0.01, ceil=1.0)
-        if score > min_score:
+        if best_score > min_score:
             extra = [
-                f"best score: {'%.2f' % round(score, 2)} > {'%.2f' % round(min_score, 2)}"
-                if score < max_score else
-                f"max score reached: {'%.2f' % round(score, 2)} > {'%.2f' % round(max_score, 2)}"
+                f"best score: {'%.2f' % round(best_score, 2)} > {'%.2f' % round(min_score, 2)}"
+                if best_score < max_score else
+                f"max score reached: {'%.2f' % round(best_score, 2)} > {'%.2f' % round(max_score, 2)}"
             ]
             self._log_match(source=source, result=result, extra=extra)
             return result
         else:
-            self._log_test(source=source, result=result, test=score, extra=[f"NO MATCH: {score}<{min_score}"])
+            self._log_test(source=source, result=result, test=best_score, extra=[f"NO MATCH: {best_score}<{min_score}"])
 
-    def _score[T: (Track, Album)](
+    def _score[T: MusifyObject](
             self,
             source: T,
             results: Iterable[T],
-            max_score: float = 0.8,
+            executor: Executor,
             match_on: set[TagField] = ALL_TAG_FIELDS,
             allow_karaoke: bool = False,
-    ) -> tuple[float, T | None]:
+    ) -> list[tuple[T, dict[TagField, Future[float] | list[list[Future[float]]]]]]:
         """
-        Gets the score and result from a cleaned source and a given list of results.
+        Gets the scores for all given ``results`` against a cleaned ``source``.
 
         :param source: Source item to compare against and find a match for with assigned ``clean_tags``.
         :param results: Result items for comparisons.
-        :param max_score: Stop matching once this score has been reached.
-            Value will be limited to between 0.01 and 1.0.
+        :param executor: The executor to submit tasks to.
         :param match_on: List of tags to match on. Currently only the following fields are supported:
             ``title``, ``artist``, ``album``, ``year``, ``length``.
         :param allow_karaoke: When True, items determined to be karaoke are allowed when matching added items.
             Skip karaoke results otherwise. Karaoke items are identified using the ``karaoke_tags`` attribute.
         :return: Tuple of (the score between 0-1, the item that had the best score)
         """
+        scores: list[tuple[T, dict[TagField, Future[float] | list[Future[float]]]]] = []
         if not results:
             self._log_algorithm(source=source, extra=["NO RESULTS GIVEN, SKIPPING"])
-            return 0, None
-        max_score = limit_value(max_score, floor=0.01, ceil=1.0)
-        self._log_algorithm(source=source, extra=[f"max_score={max_score}"])
-
-        best_score = 0
-        best_result = None
+            return scores
 
-        for current_result in results:
-            self.clean_tags(current_result)
-            scores = self._get_scores(
-                source=source, result=current_result, match_on=match_on, allow_karaoke=allow_karaoke
+        for result in results:
+            self.clean_tags(result)
+            result_scores = self._get_scores(
+                source=source, result=result, executor=executor, match_on=match_on, allow_karaoke=allow_karaoke
             )
-            if not scores:
+            if not result_scores:
                 continue
+            scores.append((result, result_scores))
 
-            current_score = sum(scores.values()) / len(scores)
-            log_extra = [f"BEST={round(best_score, 2)}"]
-            self._log_test(source=source, result=current_result, test=round(current_score, 2), extra=log_extra)
-
-            if current_score > best_score:
-                best_result = current_result
-                best_score = sum(scores.values()) / len(scores)
-            if best_score >= max_score:  # max threshold reached, match found
-                break
-
-        return best_score, best_result
+        return scores
 
-    def _get_scores[T: (Track, Album)](
-            self, source: T, result: T, match_on: set[TagField] = ALL_TAG_FIELDS, allow_karaoke: bool = False
-    ) -> dict[TagField, float]:
+    def _get_scores[T: MusifyObject](
+            self,
+            source: T,
+            result: T,
+            executor: Executor,
+            match_on: set[TagField] = ALL_TAG_FIELDS,
+            allow_karaoke: bool = False,
+    ) -> dict[TagField, Future[float] | list[list[Future[float]]]]:
         """
         Gets the scores from a cleaned source and result to match on.
-        When an ItemCollection is given to match on, scores are also calculated for each of the items in the collection.
+        When an MusifyCollection is given to match on,
+        scores are also calculated for each of the items in the collection.
         Scores are always between 0-1.
 
         :param source: Source item to compare against and find a match for with assigned ``clean_tags``.
         :param result: Result item to compare against with assigned ``clean_tags``.
+        :param executor: The executor to submit tasks to.
         :param match_on: List of tags to match on. Currently only the following fields are supported:
             ``title``, ``artist``, ``album``, ``year``, ``length``.
         :param allow_karaoke: When True, items determined to be karaoke are allowed when matching added items.
             Skip karaoke results otherwise. Karaoke items are identified using the ``karaoke_tags`` attribute.
         :return: Map of score type name to score.
         """
+        scores: dict[TagField, Future[float] | list[list[Future[float]]]] = {}
         if not allow_karaoke and self.match_not_karaoke(source, result) < 1:
-            return {}
-
-        scores_current: dict[TagField, float] = {}
+            return scores
 
         if Tag.TITLE in match_on:
-            scores_current[Tag.TITLE] = self.match_name(source=source, result=result)
+            scores[Tag.TITLE] = executor.submit(self.match_name, source=source, result=result)
         if Tag.ARTIST in match_on:
-            scores_current[Tag.ARTIST] = self.match_artist(source=source, result=result)
+            scores[Tag.ARTIST] = executor.submit(self.match_artist, source=source, result=result)
         if Tag.ALBUM in match_on:
-            scores_current[Tag.ALBUM] = self.match_album(source=source, result=result)
+            scores[Tag.ALBUM] = executor.submit(self.match_album, source=source, result=result)
         if Tag.LENGTH in match_on:
-            scores_current[Tag.LENGTH] = self.match_length(source=source, result=result)
+            scores[Tag.LENGTH] = executor.submit(self.match_length, source=source, result=result)
         if Tag.YEAR in match_on:
-            scores_current[Tag.YEAR] = self.match_year(source=source, result=result)
-
-        if isinstance(source, ItemCollection) and isinstance(result, ItemCollection):
-            # skip this if not a collection of items
-            if not all(isinstance(i, Track) for i in source.items):
-                return scores_current
-            if not all(isinstance(i, Track) for i in result.items):
-                return scores_current
+            scores[Tag.YEAR] = executor.submit(self.match_year, source=source, result=result)
 
+        if isinstance(source, MusifyCollection) and isinstance(result, MusifyCollection):
             # also score all the items individually in the collection
-            scores_current[Tag.ALL] = 0
+            scores[Tag.ALL] = []
             for item in source.items:
                 self.clean_tags(item)
-                score, _ = self._score(source=item, results=result.items, match_on=match_on)
-                scores_current[Tag.ALL] += score / len(source.items)
+                item_scores = self._score(
+                    source=item, results=result.items, match_on=match_on, allow_karaoke=allow_karaoke, executor=executor
+                )
+                for _, item_score in item_scores:
+                    scores[Tag.ALL].append([score for score in item_score.values() if not isinstance(score, list)])
 
-        return scores_current
+        return scores
 
     def as_dict(self) -> dict[str, Any]:
         return {
             "clean_tags": {
                 "remove_all": self.clean_tags_remove_all,
                 "split_all": self.clean_tags_split_all,
                 "config": self.clean_tags_config,
```

### Comparing `musify-0.8.1/musify/processors/sort.py` & `musify-0.9.0/musify/processors/sort.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,65 @@
 """
 Processor that sorts the given collection of items based on given configuration.
 """
-
-from collections.abc import Callable, Mapping, MutableMapping, Sequence, MutableSequence, Iterable
+import random
+from collections.abc import Callable, Mapping, MutableMapping, Sequence, Iterable
 from copy import copy
 from datetime import datetime
 from random import shuffle
-from typing import Any, Self
+from typing import Any
 
-from musify.processors.base import MusicBeeProcessor
-from musify.shared.core.base import Item
-from musify.shared.core.enum import MusifyEnum, Field, Fields
-from musify.shared.types import UnitSequence, UnitIterable
-from musify.shared.utils import flatten_nested, strip_ignore_words, to_collection, limit_value
+from musify.core.base import MusifyItem
+from musify.core.enum import MusifyEnum, Field
+from musify.processors.base import Processor
+from musify.processors.exception import SorterProcessorError
+from musify.types import UnitSequence, UnitIterable, Number
+from musify.utils import flatten_nested, strip_ignore_words, to_collection, limit_value
 
 
 class ShuffleMode(MusifyEnum):
-    """Represents the possible shuffle modes to use when shuffling items in a playlist."""
-    NONE = 0
-    RANDOM = 1
-    HIGHER_RATING = 2
-    RECENT_ADDED = 3
+    """Represents the possible shuffle modes to use when shuffling items using :py:class:`ItemSorter`."""
+    RANDOM = 0
+    HIGHER_RATING = 1
+    RECENT_ADDED = 2
     DIFFERENT_ARTIST = 3
 
 
-class ShuffleBy(MusifyEnum):
-    """Represents the possible items/properties to shuffle by when shuffling items in a playlist."""
-    TRACK = 0
-    ALBUM = 1
-    ARTIST = 2
-
-
-class ItemSorter(MusicBeeProcessor):
+class ItemSorter(Processor):
     """
     Sort items in-place based on given conditions.
 
-    :param fields:
-        * When None and ShuffleMode is RANDOM, shuffle the items. Otherwise, do nothing.
+    ``fields`` may be:
         * List of tags/properties to sort by.
         * Map of ``{<tag/property>: <reversed>}``. If reversed is true, sort the ``tag/property`` in reverse.
-    :param shuffle_mode: The mode to use for shuffling.
-    :param shuffle_by: The field to shuffle by when shuffling.
-    :param shuffle_weight: The weights (between -1 and 1) to apply to shuffling modes that can use it.
-        This value will automatically be limited to within the accepted range 0 and 1.
-    """
 
-    __slots__ = ("sort_fields", "shuffle_mode", "shuffle_by", "shuffle_weight")
+    When ``shuffle_mode`` == ``HIGHER_RATING`` or ``RECENT_ADDED``:
+        * A ``shuffle_weight`` of 0 will sort the tracks in order according to the desired ``shuffle_mode``.
+        * A positive ``shuffle_weight`` shuffles according to the desired ``shuffle_mode``.
+          The ``shuffle_weight`` will determine how much randomness is applied to lower ranking items.
+        * A negative ``shuffle_weight`` works as above but reverses the final sort order.
+
+    When ``shuffle_mode`` == ``DIFFERENT_ARTIST``:
+        * A ``shuffle_weight`` of 1 will group the tracks by artist, shuffling artists randomly.
+        * A ``shuffle_weight`` of -1 will shuffle the items randomly.
+
+    :param fields: Fields to sort by. If defined, this value will always take priority over any shuffle settings
+        i.e. shuffle settings will be ignored.
+    :param shuffle_mode: The mode to use for shuffling. Only used when no ``fields`` are given.
+        WARNING: Currently only ``RANDOM`` shuffle mode has been implemented.
+        Any other given value will default to ``RANDOM`` shuffling.
+    :param shuffle_weight: The weights (between -1 and 1) to apply to certain shuffling modes.
+        This value will automatically be limited to within the valid range -1 and 1.
+        Only used when no ``fields`` are given and shuffle_mode is not None or ``RANDOM``.
+    """
 
-    #: Settings for custom sort codes.
-    _custom_sort: dict[int, Mapping[Field, bool]] = {
-        6: {
-            Fields.ALBUM: False,
-            Fields.DISC_NUMBER: False,
-            Fields.TRACK_NUMBER: False,
-            Fields.FILENAME: False
-        }
-    }
-    # TODO: implement field_code 78 - manual order according to MusicBee library file.
-    #  This is a workaround
-    _custom_sort[78] = _custom_sort[6]
+    __slots__ = ("sort_fields", "shuffle_mode", "shuffle_weight")
 
     @classmethod
-    def sort_by_field(cls, items: list[Item], field: Field | None = None, reverse: bool = False) -> None:
+    def sort_by_field(cls, items: list[MusifyItem], field: Field | None = None, reverse: bool = False) -> None:
         """
         Sort items by the values of a given field.
 
         :param items: List of items to sort
         :param field: Tag or property to sort on. If None and reverse is True, reverse the order of the list.
         :param reverse: If true, reverse the order of the sort.
         """
@@ -84,27 +78,27 @@
                 break
         if example_value is None:
             # if no example value found, all values are None and so no sort can happen safely. Skip
             return
 
         # get sort key based on value type
         if isinstance(example_value, datetime):  # key converts datetime to floats
-            def sort_key(t: Item) -> float:
+            def sort_key(t: MusifyItem) -> float:
                 """Get the sort key for timestamp tags from the given ``t``"""
                 value = t[tag_name]
                 return value.timestamp() if value is not None else 0.0
         elif isinstance(example_value, str):  # key strips ignore words from string
-            sort_key: Callable[[Item], (bool, str)] = lambda t: strip_ignore_words(t[tag_name])
+            sort_key: Callable[[MusifyItem], (bool, str)] = lambda t: strip_ignore_words(t[tag_name])
         else:
-            sort_key: Callable[[Item], object] = lambda t: t[tag_name] if t[tag_name] else 0
+            sort_key: Callable[[MusifyItem], object] = lambda t: t[tag_name] if t[tag_name] else 0
 
         items.sort(key=sort_key, reverse=reverse)
 
     @classmethod
-    def group_by_field[T: Item](cls, items: UnitIterable[T], field: Field | None = None) -> dict[Any, list[T]]:
+    def group_by_field[T: MusifyItem](cls, items: UnitIterable[T], field: Field | None = None) -> dict[Any, list[T]]:
         """
         Group items by the values of a given field.
 
         :param items: List of items to sort.
         :param field: Tag or property to group by. None returns map of ``{None: <items>}``.
         :return: Map of grouped items.
         """
@@ -126,89 +120,101 @@
                 for val in value:
                     group(val)
             else:
                 group(value)
 
         return grouped
 
-    @classmethod
-    def from_xml(cls, xml: Mapping[str, Any], **__) -> Self:
-        fields: Sequence[Field] | Mapping[Field | bool]
-        source = xml["SmartPlaylist"]["Source"]
-
-        if "SortBy" in source:
-            field_code = int(source["SortBy"].get("@Field", 0))
-        elif "DefinedSort" in source:
-            field_code = int(source["DefinedSort"]["@Id"])
-        else:
-            return
-
-        if field_code in cls._custom_sort:
-            fields = cls._custom_sort[field_code]
-            return cls(fields=fields)
-        else:
-            field = Fields.from_value(field_code)[0]
-
-        if field is None:
-            return cls()
-        elif "SortBy" in source:
-            fields = {field: source["SortBy"]["@Order"] == "Descending"}
-        elif "DefinedSort" in source:
-            fields = [field]
-        else:
-            raise NotImplementedError("Sort type in XML not recognised")
-
-        shuffle_mode = ShuffleMode.from_name(cls._pascal_to_snake(xml["SmartPlaylist"]["@ShuffleMode"]))[0]
-        shuffle_by = ShuffleBy.from_name(cls._pascal_to_snake(xml["SmartPlaylist"]["@GroupBy"]))[0]
-        shuffle_weight = float(xml["SmartPlaylist"].get("@ShuffleSameArtistWeight", 1))
-
-        return cls(fields=fields, shuffle_mode=shuffle_mode, shuffle_by=shuffle_by, shuffle_weight=shuffle_weight)
-
-    def to_xml(self, **kwargs) -> Mapping[str, Any]:
-        raise NotImplementedError
-
     def __init__(
             self,
             fields: UnitSequence[Field | None] | Mapping[Field | None, bool] = (),
-            shuffle_mode: ShuffleMode = ShuffleMode.NONE,
-            shuffle_by: ShuffleBy = ShuffleBy.TRACK,
-            shuffle_weight: float = 1.0
+            shuffle_mode: ShuffleMode | None = None,
+            shuffle_weight: float = 0.0
     ):
         super().__init__()
         fields = to_collection(fields, list) if isinstance(fields, Field) else fields
-        self.sort_fields: Mapping[Field | None, bool]
-        self.sort_fields = {field: False for field in fields} if isinstance(fields, Sequence) else fields
+        self.sort_fields: dict[Field | None, bool] = {field: False for field in fields} \
+            if isinstance(fields, Sequence) else fields
 
-        self.shuffle_mode: ShuffleMode | None
-        self.shuffle_mode = shuffle_mode if shuffle_mode in [ShuffleMode.NONE, ShuffleMode.RANDOM] else ShuffleMode.NONE
-        self.shuffle_by: ShuffleBy | None = shuffle_by
+        self.shuffle_mode = shuffle_mode
         self.shuffle_weight = limit_value(shuffle_weight, floor=-1, ceil=1)
 
-    def __call__(self, items: MutableSequence[Item]) -> None:
-        return self.sort(items=items)
+    def __call__(self, *args, **kwargs) -> None:
+        return self.sort(*args, **kwargs)
 
-    def sort(self, items: MutableSequence[Item]) -> None:
+    def sort(self, items: list[MusifyItem]) -> None:
         """Sorts a list of ``items`` in-place."""
         if len(items) == 0:
             return
 
-        if self.shuffle_mode == ShuffleMode.RANDOM:  # random
-            shuffle(items)
-        elif self.shuffle_mode == ShuffleMode.NONE and self.sort_fields:  # sort by fields
+        if self.sort_fields:
             items_nested = self._sort_by_fields({None: items}, fields=self.sort_fields)
             items.clear()
             items.extend(flatten_nested(items_nested))
-        elif not self.sort_fields:  # no sort
-            return
-        else:
-            # TODO: implement all shuffle modes
-            raise NotImplementedError(f"Shuffle mode not yet implemented: {self.shuffle_mode}")
+        elif self.shuffle_mode == ShuffleMode.RANDOM:
+            shuffle(items)
+        elif self.shuffle_mode == ShuffleMode.HIGHER_RATING:
+            self._shuffle_on_rating(items)
+        elif self.shuffle_mode == ShuffleMode.RECENT_ADDED:
+            self._shuffle_on_date_added(items)
+        elif self.shuffle_mode == ShuffleMode.DIFFERENT_ARTIST:
+            self._shuffle_on_artist(items)
+
+    def _get_weighted_shuffle_value(self, value: Number, max_value: Number) -> float:
+        weight_factor = random.uniform(-1, 1) * self.shuffle_weight
+        return abs(value - weight_factor * (value - max_value))
+
+    # noinspection PyUnresolvedReferences
+    def _shuffle_on_rating(self, items: list[MusifyItem]) -> None:
+        if not all(hasattr(item, "rating") for item in items):
+            raise SorterProcessorError(
+                "Cannot shuffle sort on rating as the given items do not all have a 'rating' property"
+            )
+
+        max_value: float = max(item.rating for item in items)
+        items.sort(
+            key=lambda item: self._get_weighted_shuffle_value(item.rating, max_value),
+            reverse=self.shuffle_weight >= 0
+        )
+
+    # noinspection PyUnresolvedReferences
+    def _shuffle_on_date_added(self, items: list[MusifyItem]) -> None:
+        if not all(hasattr(item, "date_added") for item in items):
+            raise SorterProcessorError(
+                "Cannot shuffle sort on date added as the given items do not all have a 'date_added' property"
+            )
+
+        max_value: float = max(item.date_added.timestamp() for item in items)
+        items.sort(
+            key=lambda item: self._get_weighted_shuffle_value(item.date_added.timestamp(), max_value),
+            reverse=self.shuffle_weight >= 0
+        )
+
+    # noinspection PyUnresolvedReferences
+    def _shuffle_on_artist(self, items: list[MusifyItem]) -> None:
+        if not all(hasattr(item, "artist") for item in items):
+            raise SorterProcessorError(
+                "Cannot shuffle sort on artist as the given items do not all have an 'artist' property"
+            )
+
+        shuffle_weight = (self.shuffle_weight + 1) / 2
+        artists: list[str] = list({item.artist for item in items})
+        shuffle(artists)
+
+        def sort_key(artist: str) -> int:
+            """Get sort key for a given ``artist``"""
+            return artists.index(artist) if random.random() <= shuffle_weight else random.randrange(0, len(artists))
+
+        shuffle(items)
+        items.sort(key=lambda item: sort_key(item.artist))
 
     @classmethod
-    def _sort_by_fields(cls, items_grouped: MutableMapping, fields: MutableMapping[Field, bool]) -> MutableMapping:
+    def _sort_by_fields(
+            cls, items_grouped: MutableMapping, fields: MutableMapping[Field | None, bool]
+    ) -> MutableMapping:
         """
         Sort items by the given fields recursively in the order given.
 
         :param items_grouped: Map of items grouped by the last sort value.
         :param fields: Map of ``{<tag/property>: <reversed>}``.
             If reversed is True, sort the ``tag/property`` in reverse.
         :return: Map of grouped and sorted items.
@@ -231,9 +237,9 @@
         fields = None
         if isinstance(self.sort_fields, Mapping):
             fields = {field.name: "desc" if r else "asc" for field, r in self.sort_fields.items()}
 
         return {
             "sort_fields": fields,
             "shuffle_mode": self.shuffle_mode,
-            "shuffle_by": self.shuffle_by
+            "shuffle_weight": self.shuffle_weight
         }
```

### Comparing `musify-0.8.1/musify/processors/time.py` & `musify-0.9.0/musify/processors/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """
 Processor that converts representations of time units to python time objects.
 """
-
 from datetime import timedelta
 from typing import Any
 
 from dateutil.relativedelta import relativedelta
 
+from musify.core.printer import PrettyPrinter
 from musify.processors.base import DynamicProcessor, dynamicprocessormethod
-from musify.shared.core.misc import PrettyPrinter
 
 
 class TimeMapper(DynamicProcessor, PrettyPrinter):
     """Map of time character representation to it unit conversion from seconds"""
 
     @classmethod
     def _processor_method_fmt(cls, name: str) -> str:
         return name.casefold().strip()[0] if not name.startswith("min") else name
 
     def __init__(self, func: str):
         super().__init__()
         self._set_processor_name(func)
 
-    def __call__(self, value: Any):
-        return self.map(value)
+    def __call__(self, *args, **kwargs):
+        return self.map(*args, **kwargs)
 
     def map(self, value: Any):
         """Run the mapping function"""
         return super().__call__(value)
 
     @dynamicprocessormethod
     def seconds(self, value: Any) -> timedelta:
```

### Comparing `musify-0.8.1/musify/shared/exception.py` & `musify-0.9.0/musify/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Core exceptions for the entire package.
 """
-
 from typing import Any
 
 
 class MusifyError(Exception):
     """Generic base class for all Musify-related errors"""
```

### Comparing `musify-0.8.1/musify/shared/field.py` & `musify-0.9.0/musify/field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,31 @@
 """
 All core :py:class:`Field` implementations relating to
-core :py:class:`Item` and :py:class`ItemCollection` implementations.
+core :py:class:`MusifyItem` and :py:class`MusifyCollection` implementations.
 """
-
 from typing import Self
 
-from musify.shared.core.enum import Field, Fields, TagField, TagFields
+from musify.core.enum import Field, Fields, TagField, TagFields
 
 
 class TrackFieldMixin(TagField):
     """Applies extra functionality to the TagField enum for TagField types relating to :py:class:`Track` types"""
 
     # noinspection PyUnresolvedReferences
     @classmethod
     def map(cls, enum: Self) -> list[Self]:
-        """
-        Mapper to apply to the enum found during :py:meth:`from_name` and :py:meth:`from_value` calls,
-        or from :py:meth:`to_tag` and :py:meth:`to_tags` calls
-
-        Applies the following mapping:
-            * ``TRACK`` returns both ``TRACK_NUMBER`` and ``TRACK_TOTAL`` enums
-            * ``DISC`` returns both ``DISC_NUMBER`` and ``DISC_TOTAL`` enums
-            * all other enums return the enum in a unit list
-        """
         if enum == cls.TRACK:
             return [cls.TRACK_NUMBER, cls.TRACK_TOTAL]
         elif enum == cls.DISC:
             return [cls.DISC_NUMBER, cls.DISC_TOTAL]
         return [enum]
 
 
 class TrackField(TrackFieldMixin):
-    """Represent all currently supported fields for objects of type :py:class:`Track`"""
+    """Represents all currently supported fields for objects of type :py:class:`Track`"""
     ALL = TagFields.ALL.value
 
     TITLE = TagFields.TITLE.value
     ARTIST = TagFields.ARTIST.value
     ALBUM = TagFields.ALBUM.value
     ALBUM_ARTIST = TagFields.ALBUM_ARTIST.value
     TRACK = TagFields.TRACK_NUMBER.value + 500
@@ -55,15 +45,15 @@
     RATING = TagFields.RATING.value
 
     # remote properties
     URI = TagFields.URI.value
 
 
 class PlaylistField(Field):
-    """Represent all currently supported fields for objects of type :py:class:`Playlist`"""
+    """Represents all currently supported fields for objects of type :py:class:`Playlist`"""
     ALL = Fields.ALL.value
 
     # tags/core properties
     TRACK_TOTAL = Fields.TRACK_TOTAL.value
     IMAGES = Fields.IMAGES.value
     LENGTH = Fields.LENGTH.value
 
@@ -72,30 +62,30 @@
     DATE_MODIFIED = Fields.DATE_MODIFIED.value
 
     # miscellaneous properties
     DESCRIPTION = Fields.DESCRIPTION.value
 
 
 class FolderField(Field):
-    """Represent all currently supported fields for objects of type :py:class:`Folder`"""
+    """Represents all currently supported fields for objects of type :py:class:`Folder`"""
     ALL = Fields.ALL.value
 
     # tags/core properties
     TRACK_TOTAL = Fields.TRACK_TOTAL.value
     GENRES = Fields.GENRES.value
     IMAGES = Fields.IMAGES.value
     COMPILATION = Fields.COMPILATION.value
     LENGTH = Fields.LENGTH.value
 
     # file properties
     FOLDER = Fields.FOLDER.value
 
 
 class AlbumField(Field):
-    """Represent all currently supported fields for objects of type :py:class:`Album`"""
+    """Represents all currently supported fields for objects of type :py:class:`Album`"""
     ALL = Fields.ALL.value
 
     # tags/core properties
     ARTIST = Fields.ARTIST.value
     ALBUM = Fields.ALBUM.value
     ALBUM_ARTIST = Fields.ALBUM_ARTIST.value
     TRACK_TOTAL = Fields.TRACK_TOTAL.value
@@ -108,15 +98,15 @@
     COMPILATION = Fields.COMPILATION.value
     IMAGES = Fields.IMAGES.value
     LENGTH = Fields.LENGTH.value
     RATING = Fields.RATING.value
 
 
 class ArtistField(Field):
-    """Represent all currently supported fields for objects of type :py:class:`Artist`"""
+    """Represents all currently supported fields for objects of type :py:class:`Artist`"""
     ALL = Fields.ALL.value
 
     # tags/core properties
     ARTIST = Fields.ARTIST.value
     TRACK_TOTAL = Fields.TRACK_TOTAL.value
     GENRES = Fields.GENRES.value
     IMAGES = Fields.IMAGES.value
```

### Comparing `musify-0.8.1/musify/shared/handlers.py` & `musify-0.9.0/musify/log/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """
 All logging handlers specific to this package.
 """
-
 import logging.handlers
 import os
 import shutil
 from datetime import datetime
 from glob import glob
 from os.path import join, dirname, isfile, sep, isdir
 
+from musify.log import LOGGING_DT_FORMAT
 from musify.processors.time import TimeMapper
-from musify.shared.logger import LOGGING_DT_FORMAT
 
 
-###########################################################################
-## Logging handlers
-###########################################################################
 class CurrentTimeRotatingFileHandler(logging.handlers.BaseRotatingHandler):
     """
     Handles log file and directory rotation based on log file/folder name.
 
     :param filename: The full path to the log file.
         Optionally, include a '{}' part in the path to format in the current datetime.
         When None, defaults to '{}.log'
```

### Comparing `musify-0.8.1/musify/shared/utils.py` & `musify-0.9.0/musify/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Generic utility functions and classes which can be used throughout the entire package.
 """
-
 import re
 from collections import Counter
 from collections.abc import Iterable, Collection, MutableSequence, Mapping, MutableMapping
 from typing import Any
 
 import unicodedata
 
-from musify.shared.exception import MusifyTypeError
-from musify.shared.types import Number
+from musify.exception import MusifyTypeError
+from musify.types import Number
 
 
 class SafeDict(dict):
     """Extends dict to ignore missing keys when using format_map operations"""
     def __missing__(self, key):
         return "{" + key + "}"
```

### Comparing `musify-0.8.1/musify/shared/api/authorise.py` & `musify-0.9.0/musify/api/authorise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Handle API authorisation for requesting access tokens to an API.
 """
-
 import json
 import logging
 import os
 import socket
 from collections.abc import Callable, Mapping, Sequence, MutableMapping
 from datetime import datetime
 from typing import Any
 from urllib.parse import urlparse, parse_qs
 from webbrowser import open as webopen
 
 import requests
 
 from musify import PROGRAM_NAME
-from musify.shared.api.exception import APIError
-from musify.shared.logger import MusifyLogger
+from musify.api.exception import APIError
+from musify.log.logger import MusifyLogger
 
 
 class APIAuthoriser:
+    # noinspection GrazieInspection
     """
     Authorises and validates an API token for given input parameters.
     Functions for returning formatted headers for future, authorised requests.
 
     Any ``..._args`` parameters must be provided as a dictionary of parameters to be passed directly
     to the :py:class:`requests` module e.g.
 
@@ -39,26 +39,29 @@
             },
             "auth": ('user', 'pass'),
             "headers": {},
             "json": {},
         }
 
     :param name: The name of the API service being accessed.
-    :param auth_args: The parameters to be passed to the requests.post() function for initial token authorisation.
-        See description for possible example values.
-    :param user_args: Parameters to be passed to the requests.post() function
-        for requesting user authorised access to API services.
+    :param auth_args: The parameters to be passed to the
+        `requests.post() <https://requests.readthedocs.io/en/latest/api/#requests.post>`_
+        function for initial token authorisation. See description for possible example values.
+    :param user_args: The parameters to be passed to the
+        `requests.post() <https://requests.readthedocs.io/en/latest/api/#requests.post>`_
+        function for requesting user authorised access to API services.
         The code response from this request is then added to the authorisation request args
-        to grant user authorisation to the API.
-        See description for possible example values.
-    :param refresh_args: Parameters to be passed to the requests.post() function
-        for refreshing an expired token when a refresh_token is present.
+        to grant user authorisation to the API. See description for possible example values.
+    :param refresh_args: The parameters to be passed to the
+        `requests.post() <https://requests.readthedocs.io/en/latest/api/#requests.post>`_
+        function for refreshing an expired token when a refresh_token is present.
         See description for possible example values.
-    :param test_args: Parameters to be passed to the requests.get() function for testing validity of the token.
-        Must be set in conjunction with test_condition to work.
+    :param test_args: The parameters to be passed to the
+        `requests.get() <https://requests.readthedocs.io/en/latest/api/#requests.get>`_
+        function for testing validity of the token. Must be set in conjunction with test_condition to work.
         See description for possible example values.
     :param test_condition: Callable function for testing the response from the given
         test_args. e.g. ``lambda r: "error" not in r``
     :param test_expiry: The time allowance in seconds left until the token is due to expire to use when testing.
         Useful for ensuring the token will be valid for long enough to run your operations e.g.
 
         - a token has 600 second total expiry time,
```

### Comparing `musify-0.8.1/musify/shared/api/exception.py` & `musify-0.9.0/musify/api/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Exceptions relating to API operations.
 """
-
 from requests import Response
 
-from musify.shared.exception import MusifyError
+from musify.exception import MusifyError
 
 
 class APIError(MusifyError):
     """
     Exception raised for API errors.
 
     :param message: Explanation of the error.
```

### Comparing `musify-0.8.1/musify/shared/api/request.py` & `musify-0.9.0/musify/api/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
 All operations relating to handling of requests to an API.
 """
-
 import json
 from collections.abc import Mapping, Iterable
-from datetime import datetime as dt
-from datetime import timedelta
+from datetime import datetime, timedelta
 from http import HTTPStatus
 from time import sleep
 from typing import Any
 
 import requests
 from requests import Response, Session
-from requests_cache import CachedSession
+from requests_cache import CachedSession, ExpirationTime
 
-from musify.shared.api.authorise import APIAuthoriser
-from musify.shared.api.exception import APIError
+from musify.api.authorise import APIAuthoriser
+from musify.api.exception import APIError
 
 
 class RequestHandler(APIAuthoriser):
     """
     Generic API request handler using cached responses for GET requests only.
     Caches GET responses for a maximum of 4 weeks by default.
     Handles error responses and backoff on failed requests.
@@ -51,15 +49,15 @@
     def timeout(self) -> int:
         """
         When the response gives a time to wait until (i.e. retry-after),
         the program will exit if this time is above this timeout (in seconds)
         """
         return sum(self.backoff_start * self.backoff_factor ** i for i in range(self.backoff_count + 1))
 
-    def __init__(self, cache_path: str | None = None, cache_expiry=timedelta(weeks=4), **auth_kwargs):
+    def __init__(self, cache_path: str | None = None, cache_expiry: ExpirationTime = timedelta(weeks=4), **auth_kwargs):
         super().__init__(**auth_kwargs)
 
         #: The :py:class:`Session` or :py:class:`CachedSession` object
         self.session: CachedSession | Session
         if cache_path:
             self.logger.debug(f"Setting up requests cache: {cache_path}")
             self.session = CachedSession(cache_path, expire_after=cache_expiry, allowable_methods=["GET"])
@@ -67,14 +65,18 @@
             self.session = Session()
 
     def authorise(self, force_load: bool = False, force_new: bool = False) -> dict[str, str]:
         headers = super().authorise(force_load=force_load, force_new=force_new)
         self.session.headers.update(headers)
         return headers
 
+    def close(self) -> None:
+        """Close the current session. No more requests will be possible once this has been called."""
+        self.session.close()
+
     def request(self, method: str, url: str, *args, **kwargs) -> dict[str, Any]:
         """
         Generic method for handling API requests with back-off on failed requests.
         See :py:func:`request` for more arguments.
 
         :param method: method for the new :class:`Request` object:
             ``GET``, ``OPTIONS``, ``HEAD``, ``POST``, ``PUT``, ``PATCH``, or ``DELETE``.
@@ -170,15 +172,15 @@
 
     def _handle_wait_time(self, response: Response) -> bool:
         """Handle when a wait time is included in the response headers."""
         if "retry-after" not in response.headers:
             return False
 
         wait_time = int(response.headers["retry-after"])
-        wait_str = (dt.now() + timedelta(seconds=wait_time)).strftime("%Y-%m-%d %H:%M:%S")
+        wait_str = (datetime.now() + timedelta(seconds=wait_time)).strftime("%Y-%m-%d %H:%M:%S")
         self.logger.info(f"\33[91mRate limit exceeded. Retrying again at {wait_str}\33[0m")
 
         if wait_time > self.timeout:  # exception if too long
             raise APIError(f"Rate limit exceeded and wait time is greater than timeout of {self.timeout} seconds")
 
         # wait if time is short
         sleep(wait_time)
@@ -231,7 +233,14 @@
     def __copy__(self):
         """Do not copy handler"""
         return self
 
     def __deepcopy__(self, _: dict = None):
         """Do not copy handler"""
         return self
+
+    def __enter__(self):
+        self.authorise()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
```

### Comparing `musify-0.8.1/musify/shared/core/collection.py` & `musify-0.9.0/musify/libraries/core/collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,144 @@
 """
 The fundamental core collection classes for the entire package.
 """
-
 from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
+from abc import ABCMeta, abstractmethod, ABC
 from collections.abc import MutableSequence, Iterable, Mapping, Collection
+from dataclasses import dataclass
 from typing import Any, SupportsIndex, Self
 
-from musify.processors.sort import ShuffleMode, ShuffleBy, ItemSorter
-from musify.shared.core.base import Nameable, NameableTaggableMixin, AttributePrinter, Item
-from musify.shared.core.enum import Field
-from musify.shared.exception import MusifyTypeError, MusifyKeyError
-from musify.shared.types import UnitSequence
+from musify.core.base import MusifyObject, MusifyItem
+from musify.core.enum import Field
+from musify.exception import MusifyTypeError, MusifyKeyError, MusifyAttributeError
+from musify.file.base import File
+from musify.libraries.remote.core import RemoteResponse
+from musify.libraries.remote.core.base import RemoteObject
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
+from musify.processors.sort import ShuffleMode, ItemSorter
+from musify.types import UnitSequence
+
+
+@dataclass
+class ItemGetterStrategy(ABC):
+    """Abstract base class for strategies relating to __getitem__ operations on a :py:class:`MusifyCollection`"""
+
+    key: str
+
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        """The name of the name to assign to this ItemGetter when logging"""
+        raise NotImplementedError
+
+    @abstractmethod
+    def get_value_from_item(self, item: MusifyItem) -> str:
+        """Retrieve the appropriate value from a given ``item`` for this ItemGetter type"""
+        raise NotImplementedError
+
+    def get_item[T](self, collection: MusifyCollection[T]) -> T:
+        """Run this strategy and return the matched item from the given ``collection``"""
+        try:
+            return next(item for item in collection.items if str(self.get_value_from_item(item)) == self.key)
+        except AttributeError:
+            raise MusifyAttributeError(f"Items in collection do not have the attribute '{self.name}'")
+        except StopIteration:
+            raise MusifyKeyError(f"No matching item found for {self.name}: {self.key}")
+
+
+class NameGetter(ItemGetterStrategy):
+    """Get an item via its name for a :py:class:`MusifyCollection`"""
+    def name(self) -> str:
+        return "name"
+
+    def get_value_from_item(self, item: MusifyObject) -> str:
+        return item.name
+
+
+class PathGetter(ItemGetterStrategy):
+    """Get an item via its path for a :py:class:`MusifyCollection`"""
+    def name(self) -> str:
+        return "path"
+
+    def get_value_from_item(self, item: File) -> str:
+        return item.path
+
+
+class RemoteIDGetter(ItemGetterStrategy):
+    """Get an item via its remote ID for a :py:class:`MusifyCollection`"""
+    def name(self) -> str:
+        return "remote ID"
+
+    def get_value_from_item(self, item: RemoteResponse) -> str:
+        return item.id
+
+
+class RemoteURIGetter(ItemGetterStrategy):
+    """Get an item via its remote URI for a :py:class:`MusifyCollection`"""
+    def name(self) -> str:
+        return "URI"
+
+    def get_value_from_item(self, item: MusifyItem | RemoteResponse) -> str:
+        return item.uri
 
 
-class ItemCollection[T: Item](AttributePrinter, NameableTaggableMixin, MutableSequence[T], metaclass=ABCMeta):
-    """Generic class for storing a collection of items."""
+class RemoteURLAPIGetter(ItemGetterStrategy):
+    """Get an item via its remote API URL for a :py:class:`MusifyCollection`"""
+    def name(self) -> str:
+        return "API URL"
+
+    def get_value_from_item(self, item: RemoteObject) -> str:
+        return item.url
+
+
+class RemoteURLEXTGetter(ItemGetterStrategy):
+    """Get an item via its remote external URL for a :py:class:`MusifyCollection`"""
+    def name(self) -> str:
+        return "external URL"
+
+    def get_value_from_item(self, item: RemoteObject) -> str:
+        return item.url_ext
+
+
+class MusifyCollection[T: MusifyItem](MusifyObject, MutableSequence[T], metaclass=ABCMeta):
+    """Generic class for storing a collection of musify items."""
 
     @property
     @abstractmethod
     def items(self) -> list[T]:
         """The items in this collection"""
         raise NotImplementedError
 
+    @property
+    @abstractmethod
+    def length(self) -> float | None:
+        """Total duration of all items in this collection in seconds"""
+        raise NotImplementedError
+
     @staticmethod
     @abstractmethod
     def _validate_item_type(items: Any | Iterable[Any]) -> bool:
         """
-        Validate the given :py:class:`Item` by ensuring it matches the allowed item type for this collection.
-        Used to validate input :py:class:`Item` types given to functions that
+        Validate the given :py:class:`MusifyItem` by ensuring it matches the allowed item type for this collection.
+        Used to validate input :py:class:`MusifyItem` types given to functions that
         modify the stored items in this collection.
 
         :param items: The item or items to validate
         :return: True if valid, False if not.
         """
         raise NotImplementedError
 
+    def __init__(self, remote_wrangler: RemoteDataWrangler | None = None):
+        super().__init__()
+        #: A :py:class:`RemoteDataWrangler` object for processing remote data
+        self.remote_wrangler = remote_wrangler
+
     def count(self, __item: T) -> int:
-        """Return the number of occurrences of the given :py:class:`Item` in this collection"""
+        """Return the number of occurrences of the given :py:class:`MusifyItem` in this collection"""
         if not self._validate_item_type(__item):
             raise MusifyTypeError(type(__item).__name__)
         return self.items.count(__item)
 
     def index(self, __item: T, __start: SupportsIndex = None, __stop: SupportsIndex = None) -> int:
         """
         Return first index of item from items in this collection.
@@ -65,24 +161,24 @@
         if allow_duplicates or __item not in self.items:
             self.items.append(__item)
 
     def extend(self, __items: Iterable[T], allow_duplicates: bool = True) -> None:
         """Append many items to the items in this collection"""
         if not self._validate_item_type(__items):
             raise MusifyTypeError([type(i).__name__ for i in __items])
-        if isinstance(__items, ItemCollection):
+        if isinstance(__items, MusifyCollection):
             __items = __items.items
 
         if allow_duplicates:
             self.items.extend(__items)
         else:
             self.items.extend(item for item in __items if item not in self.items)
 
     def insert(self, __index: int, __item: T, allow_duplicates: bool = True) -> None:
-        """Insert given :py:class:`Item` before the given index"""
+        """Insert given :py:class:`MusifyItem` before the given index"""
         if not self._validate_item_type(__item):
             raise MusifyTypeError(type(__item))
         if allow_duplicates or __item not in self.items:
             self.items.insert(__index, __item)
 
     def remove(self, __item: T) -> None:
         """Remove one item from the items in this collection"""
@@ -101,73 +197,85 @@
     def clear(self) -> None:
         """Remove all items from this collection"""
         self.items.clear()
 
     def sort(
             self,
             fields: UnitSequence[Field | None] | Mapping[Field | None, bool] = (),
-            shuffle_mode: ShuffleMode = ShuffleMode.NONE,
-            shuffle_by: ShuffleBy = ShuffleBy.TRACK,
+            shuffle_mode: ShuffleMode | None = None,
             shuffle_weight: float = 1.0,
             key: Field | None = None,
             reverse: bool = False,
     ) -> None:
         """
         Sort items in this collection in-place based on given conditions.
         If key is given,
 
         :param fields:
             * When None and ShuffleMode is RANDOM, shuffle the tracks. Otherwise, do nothing.
             * List of tags/properties to sort by.
             * Map of `{<tag/property>: <reversed>}`. If reversed is true, sort the ``tag/property`` in reverse.
         :param shuffle_mode: The mode to use for shuffling.
-        :param shuffle_by: The field to shuffle by when shuffling.
         :param shuffle_weight: The weights (between 0 and 1) to apply to shuffling modes that can use it.
             This value will automatically be limited to within the accepted range 0 and 1.
         :param key: Tag or property to sort on. Can be given instead of ``fields`` for a simple sort.
             If set, all other fields apart from ``reverse`` are ignored.
             If None, ``fields``, ``shuffle_mode``, ``shuffle_by``, and ``shuffle_weight`` are used to apply sorting.
         :param reverse: If true, reverse the order of the sort at the end.
         """
         if key is not None:
             ItemSorter.sort_by_field(self.items, field=key)
         else:
-            ItemSorter(
-                fields=fields, shuffle_mode=shuffle_mode, shuffle_by=shuffle_by, shuffle_weight=shuffle_weight
-            )(self.items)
+            ItemSorter(fields=fields, shuffle_mode=shuffle_mode, shuffle_weight=shuffle_weight)(self.items)
 
         if reverse:
             self.items.reverse()
 
+    def difference(self, other: Iterable[T]) -> list[T]:
+        """
+        Return the difference between the items in this collection and an ``other`` collection as a new list.
+
+        (i.e. all items that are in this collection but not the ``other`` collection).
+        """
+        return [item for item in other if item not in self]
+
+    def intersection(self, other: Iterable[T]) -> list[T]:
+        """
+        Return the difference between the items in this collection and an ``other`` collection as a new list.
+
+        (i.e. all items that are in both this collection and the ``other`` collection).
+        """
+        return [item for item in other if item in self]
+
     @staticmethod
     def _condense_attributes(attributes: dict[str, Any]) -> dict[str, Any]:
         """Condense the attributes of the given map for cleaner attribute displaying"""
         def condense(key: str, value: Any) -> tuple[str, Any]:
             """Decide whether this key-value pair should be condensed and condense them."""
             if isinstance(value, Collection) and not isinstance(value, str):
-                if any(isinstance(v, Nameable) for v in value) or len(value) > 20 or len(value) == 0:
+                if any(isinstance(v, MusifyObject) for v in value) or len(value) > 20 or len(value) == 0:
                     return f"{key.rstrip("s")}_count", len(value)
             return key, value
 
         return dict(condense(k, v) for k, v in attributes.items())
 
     def as_dict(self):
         return self._condense_attributes(self._get_attributes())
 
-    def json(self):
-        return self._to_json(self._get_attributes())
+    def _json_attributes(self):
+        return self._get_attributes()
 
-    def __eq__(self, __collection: ItemCollection | Iterable[T]):
+    def __eq__(self, __collection: MusifyCollection | Iterable[T]):
         """Names equal and all items equal in order"""
-        name = self.name == __collection.name if isinstance(__collection, ItemCollection) else True
+        name = self.name == __collection.name if isinstance(__collection, MusifyCollection) else True
         length = len(self) == len(__collection)
         items = all(x == y for x, y in zip(self, __collection))
         return name and length and items
 
-    def __ne__(self, __collection: ItemCollection | Iterable[T]):
+    def __ne__(self, __collection: MusifyCollection | Iterable[T]):
         return not self.__eq__(__collection)
 
     def __len__(self):
         return len(self.items)
 
     def __iter__(self):
         return iter(self.items)
@@ -175,15 +283,15 @@
     def __reversed__(self):
         return reversed(self.items)
 
     def __contains__(self, __item: T):
         return any(__item == i for i in self.items)
 
     def __add__(self, __items: list[T] | Self):
-        if isinstance(__items, ItemCollection):
+        if isinstance(__items, MusifyCollection):
             return self.items + __items.items
         return self.items + __items
 
     def __iadd__(self, __items: Iterable[T]):
         self.extend(__items)
         return self
 
@@ -194,22 +302,63 @@
         return items
 
     def __isub__(self, __items: Iterable[T]):
         for item in __items:
             self.remove(item)
         return self
 
-    @abstractmethod
-    def __getitem__(self, __key: str | int | slice | Item) -> T | list[T] | list[T, None, None]:
+    def __getitem__(
+            self, __key: str | int | slice | MusifyItem | File | RemoteResponse
+    ) -> T | list[T] | list[T, None, None]:
         """
-        Returns the item in this collection by matching on a given index/Item/URI.
-        If an item is given, the URI is extracted from this item
+        Returns the item in this collection by matching on a given index/Item/URI/ID/URL.
+        If an :py:class:`MusifyItem` is given, the URI is extracted from this item
         and the matching Item from this collection is returned.
+        If a :py:class:`RemoteObject` is given, the ID is extracted from this object
+        and the matching RemoteObject from this collection is returned.
         """
-        raise NotImplementedError
+        if isinstance(__key, int) or isinstance(__key, slice):  # simply index the list or items
+            return self.items[__key]
+
+        getters = self.__get_item_getters(__key)
+        if not getters:
+            raise MusifyKeyError(f"Unrecognised key type | {__key=} | type={type(__key).__name__}")
+
+        caught_exceptions = []
+        for getter in getters:
+            try:
+                return getter.get_item(self)
+            except (MusifyAttributeError, MusifyKeyError) as ex:
+                caught_exceptions.append(ex)
+
+        raise MusifyKeyError(
+            f"Key is invalid. The following errors were thrown: {[str(ex) for ex in caught_exceptions]}"
+        )
+
+    def __get_item_getters(self, __key: str | MusifyItem | File | RemoteResponse) -> list[ItemGetterStrategy]:
+        getters = []
+        if isinstance(__key, File):
+            getters.append(PathGetter(__key.path))
+        if isinstance(__key, RemoteResponse) and self.remote_wrangler:
+            getters.append(RemoteIDGetter(__key.id))
+        if isinstance(__key, MusifyItem) and __key.has_uri:
+            getters.append(RemoteURIGetter(__key.uri))
+        if isinstance(__key, MusifyObject):
+            getters.append(NameGetter(__key.name))
+        if isinstance(__key, str):
+            getters.extend([
+                RemoteIDGetter(__key),
+                RemoteURIGetter(__key),
+                RemoteURLAPIGetter(__key),
+                RemoteURLEXTGetter(__key),
+                PathGetter(__key),
+                NameGetter(__key),
+            ])
+
+        return getters
 
     def __setitem__(self, __key: str | int | T, __value: T):
         """Replace the item at a given ``__key`` with the given ``__value``."""
         try:
             item = self[__key]
         except KeyError:
             raise MusifyKeyError(f"Given index is out of range: {__key}")
```

### Comparing `musify-0.8.1/musify/shared/core/enum.py` & `musify-0.9.0/musify/core/enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 The fundamental core enum classes for the entire package.
 """
-
 from collections.abc import Sequence
 from dataclasses import dataclass, field
 from enum import IntEnum
 from typing import Self
 
-from musify.shared.exception import MusifyEnumError
-from musify.shared.types import UnitIterable
-from musify.shared.utils import unique_list
+from musify.exception import MusifyEnumError
+from musify.types import UnitIterable
+from musify.utils import unique_list
 
 
 class MusifyEnum(IntEnum):
     """Generic class for :py:class:`IntEnum` implementations for the entire package."""
 
     @classmethod
     def map(cls, enum: Self) -> list[Self]:
         """
-        "Optional mapper to apply to the enum found during :py:meth:`all`, :py:meth:`from_name`,
+        Optional mapper to apply to the enum found during :py:meth:`all`, :py:meth:`from_name`,
         and :py:meth:`from_value` calls
         """
         return [enum]
 
     @classmethod
     def all(cls) -> list[Self]:
         """Get all enums for this enum."""
@@ -124,15 +123,15 @@
 
     # file properties
     PATH = 106
     FOLDER = 179
     FILENAME = 3
     EXT = 100
     SIZE = 7
-    KIND = 4
+    TYPE = 4
     CHANNELS = 8
     BIT_RATE = 10
     BIT_DEPTH = 183
     SAMPLE_RATE = 9
 
     # date properties
     DATE_CREATED = 921  # no MusicBee mapping
@@ -259,15 +258,15 @@
 
     # file properties
     PATH = Fields.PATH.value
     FOLDER = Fields.FOLDER.value
     FILENAME = Fields.FILENAME.value
     EXT = Fields.EXT.value
     SIZE = Fields.SIZE.value
-    KIND = Fields.KIND.value
+    TYPE = Fields.TYPE.value
     CHANNELS = Fields.CHANNELS.value
     BIT_RATE = Fields.BIT_RATE.value
     BIT_DEPTH = Fields.BIT_DEPTH.value
     SAMPLE_RATE = Fields.SAMPLE_RATE.value
 
     # date properties
     DATE_CREATED = Fields.DATE_CREATED.value
```

### Comparing `musify-0.8.1/musify/shared/core/object.py` & `musify-0.9.0/musify/libraries/core/object.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 """
-The core implementations of :py:class:`Item` and :py:class:`ItemCollection` classes.
+The core abstract implementations of :py:class:`MusifyItem` and :py:class:`MusifyCollection` classes.
 """
-
 from __future__ import annotations
 
 import datetime
 import logging
 from abc import ABCMeta, abstractmethod
-from collections.abc import Iterable, Collection, Mapping
+from collections.abc import Collection, Mapping, Iterable
 from copy import deepcopy
-from typing import Any, Self
+from typing import Self
 
-from musify.processors.base import Filter
-from musify.processors.filter import FilterDefinedList
-from musify.shared.core.base import Item
-from musify.shared.core.collection import ItemCollection
-from musify.shared.exception import MusifyKeyError, MusifyTypeError
-from musify.shared.logger import MusifyLogger
-from musify.shared.utils import to_collection, align_string, get_max_width
+from musify.core.base import MusifyItem
+from musify.exception import MusifyTypeError
+from musify.libraries.core.collection import MusifyCollection
+from musify.libraries.remote.core.enum import RemoteObjectType
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
+from musify.log.logger import MusifyLogger
 
 
-class Track(Item, metaclass=ABCMeta):
+class Track(MusifyItem, metaclass=ABCMeta):
     """Represents a track including its metadata/tags/properties."""
 
     __attributes_ignore__ = "name"
 
+    # noinspection PyPropertyDefinition
+    @classmethod
+    @property
+    def kind(cls) -> RemoteObjectType:
+        """The type of remote object associated with this class"""
+        return RemoteObjectType.TRACK
+
     @property
     def name(self) -> str:
         """This track's title"""
         return self.title
 
     @property
     @abstractmethod
@@ -149,85 +154,38 @@
     @property
     def has_image(self) -> bool:
         """Does the album this track is associated with have an image"""
         return len(self.image_links) > 0
 
     @property
     @abstractmethod
-    def length(self) -> float:
+    def length(self) -> float | None:
         """Total duration of this track in seconds"""
         raise NotImplementedError
 
     @property
     @abstractmethod
     def rating(self) -> float | None:
         """The rating for this track"""
         raise NotImplementedError
 
 
-class BasicCollection[T: Item](ItemCollection[T]):
-    """
-    A basic implementation of ItemCollection for storing ``items`` with a given ``name``.
-
-    :param name: The name of this collection.
-    :param items: The items in this collection
-    """
-
-    __slots__ = ("_name", "_items")
-
-    @staticmethod
-    def _validate_item_type(items: Any | Iterable[Any]) -> bool:
-        if isinstance(items, Iterable):
-            return all(isinstance(item, Item) for item in items)
-        return isinstance(items, Item)
-
-    @property
-    def name(self):
-        """The name of this collection"""
-        return self._name
-
-    @property
-    def items(self) -> list[T]:
-        return self._items
-
-    def __init__(self, name: str, items: Collection[T]):
-        super().__init__()
-        self._name = name
-        self._items = to_collection(items, list)
-
-    def __getitem__(self, __key: str | int | slice | Item) -> T | list[T] | list[T, None, None]:
-        """
-        Returns the item in this collection by matching on a given index/Item/URI.
-        If an item is given, the URI is extracted from this item
-        and the matching Item from this collection is returned.
-        """
-        if isinstance(__key, int) or isinstance(__key, slice):  # simply index the list or items
-            return self.items[__key]
-        elif isinstance(__key, Item):  # take the URI
-            if not __key.has_uri:
-                raise MusifyKeyError(f"Given item does not have a URI associated: {__key.name}")
-            __key = __key.uri
-        else:  # assume the string is a name
-            try:
-                return next(item for item in self.items if item.name == __key)
-            except StopIteration:
-                raise MusifyKeyError(f"No matching item found for name: '{__key}'")
-
-        try:  # string is a URI
-            return next(item for item in self.items if item.uri == __key)
-        except StopIteration:
-            raise MusifyKeyError(f"No matching item found for URI: '{__key}'")
-
-
-class Playlist[T: Track](ItemCollection[T], metaclass=ABCMeta):
+class Playlist[T: Track](MusifyCollection[T], metaclass=ABCMeta):
     """A playlist of items and their derived properties/objects."""
 
-    __attributes_classes__ = ItemCollection
+    __attributes_classes__ = MusifyCollection
     __attributes_ignore__ = "items"
 
+    # noinspection PyPropertyDefinition
+    @classmethod
+    @property
+    def kind(cls) -> RemoteObjectType:
+        """The type of remote object associated with this class"""
+        return RemoteObjectType.PLAYLIST
+
     @property
     @abstractmethod
     def name(self):
         """The name of this playlist"""
         raise NotImplementedError
 
     @property
@@ -260,15 +218,15 @@
 
     @property
     def has_image(self) -> bool:
         """Does this playlist have an image"""
         return len(self.image_links) > 0
 
     @property
-    def length(self) -> float | None:
+    def length(self):
         """Total duration of all tracks in this playlist in seconds"""
         lengths = {track.length for track in self.tracks}
         return sum(lengths) if lengths else None
 
     @property
     @abstractmethod
     def date_created(self) -> datetime.datetime | None:
@@ -277,61 +235,88 @@
 
     @property
     @abstractmethod
     def date_modified(self) -> datetime.datetime | None:
         """:py:class:`datetime.datetime` object representing when the playlist was last modified"""
         raise NotImplementedError
 
-    @abstractmethod
-    def merge(self, playlist: Playlist[T]) -> None:
+    def merge(self, other: Iterable[T], reference: Self | None = None) -> None:
         """
-        **WARNING: NOT IMPLEMENTED YET**
-        Merge tracks in this playlist with another playlist synchronising tracks between the two.
+        Merge tracks in this playlist with another collection, synchronising tracks between the two.
         Only modifies this playlist.
-        """
-        # TODO: merge playlists adding/removing tracks as needed.
-        raise NotImplementedError
 
-    # noinspection PyTypeChecker
+        Sort order is not preserved when merging.
+        Any items that need to be added to this playlist will be added at the end of the playlist.
+        Duplicates that are present in the ``other`` collection are filtered out by default.
+
+        :param other: The collection of items to merge onto this playlist.
+        :param reference: Optionally, provide a reference playlist to compare both the current playlist
+            and the ``other`` items to. The function will determine tracks to remove from
+            this playlist based on the reference. Useful for using this function as a synchronizer
+            where the reference refers to the playlist at the previous sync.
+        """
+        if not self._validate_item_type(other):
+            raise MusifyTypeError([type(i).__name__ for i in other])
+
+        if reference is None:
+            self.extend(self.difference(other), allow_duplicates=False)
+            return
+
+        for item in reference:
+            if item not in other and item in self:
+                self.remove(item)
+
+        self.extend(reference.difference(other), allow_duplicates=False)
+
     def __or__(self, other: Playlist[T]) -> Self:
         if not isinstance(other, self.__class__):
             raise MusifyTypeError(
                 f"Incorrect item given. Cannot merge with {other.__class__.__name__} "
                 f"as it is not a {self.__class__.__name__}"
             )
-        raise NotImplementedError
 
-    # noinspection PyTypeChecker
+        self_copy = deepcopy(self)
+        self_copy.merge(other)
+        return self_copy
+
     def __ior__(self, other: Playlist[T]) -> Self:
         if not isinstance(other, self.__class__):
             raise MusifyTypeError(
                 f"Incorrect item given. Cannot merge with {other.__class__.__name__} "
                 f"as it is not a {self.__class__.__name__}"
             )
-        raise NotImplementedError
 
+        self.merge(other)
+        return self
 
-class Library[T: Track](ItemCollection[T], metaclass=ABCMeta):
+
+class Library[T: Track](MusifyCollection[T], metaclass=ABCMeta):
     """A library of items and playlists and other object types."""
 
-    __attributes_classes__ = ItemCollection
+    __attributes_classes__ = MusifyCollection
     __attributes_ignore__ = "items"
 
     @property
     @abstractmethod
     def name(self):
         """The library name"""
         raise NotImplementedError
 
     @property
     def items(self):
         """The tracks in this collection"""
         return self.tracks
 
     @property
+    def length(self):
+        """Total duration of all tracks in this library in seconds"""
+        lengths = {track.length for track in self.tracks}
+        return sum(lengths) if lengths else None
+
+    @property
     @abstractmethod
     def tracks(self) -> list[T]:
         """The tracks in this library"""
         raise NotImplementedError
 
     @property
     def track_total(self) -> int:
@@ -345,68 +330,21 @@
 
     @property
     @abstractmethod
     def playlists(self) -> dict[str, Playlist[T]]:
         """The playlists in this library"""
         raise NotImplementedError
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, remote_wrangler: RemoteDataWrangler()):
+        super().__init__(remote_wrangler=remote_wrangler)
 
         # noinspection PyTypeChecker
         #: The :py:class:`MusifyLogger` for this  object
         self.logger: MusifyLogger = logging.getLogger(__name__)
 
-    def get_filtered_playlists(
-            self, playlist_filter: Collection[str] | Filter[str] = (), **tag_filter: dict[str, tuple[str, ...]]
-    ) -> dict[str, Playlist[T]]:
-        """
-        Returns a filtered set of playlists in this library.
-        The playlists returned are deep copies of the playlists in the library.
-
-        :param playlist_filter: An optional :py:class:`Filter` to apply or collection of playlist names.
-            Playlist names will be passed to this filter to limit which playlists are processed.
-        :param tag_filter: Provide optional kwargs of the tags and values of items to filter out of every playlist.
-            Parse a tag name as a parameter, any item matching the values given for this tag will be filtered out.
-            NOTE: Only `string` value types are currently supported.
-        :return: Filtered playlists.
-        """
-        self.logger.info(
-            f"\33[1;95m ->\33[1;97m Filtering playlists and tracks from {len(self.playlists)} playlists\n"
-            f"\33[0;90m    Filter out tags: {tag_filter} \33[0m"
-        )
-
-        if not isinstance(playlist_filter, Filter):
-            playlist_filter = FilterDefinedList(playlist_filter)
-        pl_filtered = [
-            pl for name, pl in self.playlists.items() if not playlist_filter or name in playlist_filter(self.playlists)
-        ]
-
-        max_width = get_max_width(self.playlists)
-        filtered: dict[str, Playlist[T]] = {}
-        for pl in self.logger.get_progress_bar(iterable=pl_filtered, desc="Filtering playlists", unit="playlists"):
-            filtered[pl.name] = deepcopy(pl)
-            for track in pl.tracks:
-                for tag, values in tag_filter.items():
-                    item_val = track[tag]
-                    if not isinstance(item_val, str):
-                        continue
-
-                    if any(v.strip().casefold() in item_val.strip().casefold() for v in values):
-                        filtered[pl.name].remove(track)
-                        break
-
-            self.logger.debug(
-                f"{align_string(pl.name, max_width=max_width)} | "
-                f"Filtered out {len(pl) - len(filtered[pl.name]):>3} items"
-            )
-
-        self.logger.print()
-        return filtered
-
     @abstractmethod
     def load(self):
         """Implementations of this function should load all data for this library and log results."""
         raise NotImplementedError
 
     @abstractmethod
     def load_tracks(self) -> None:
@@ -430,31 +368,60 @@
         raise NotImplementedError
 
     @abstractmethod
     def log_playlists(self) -> None:
         """Log stats on currently loaded playlists"""
         raise NotImplementedError
 
-    @abstractmethod
-    def merge_playlists(self, playlists: Library[T] | Collection[Playlist[T]] | Mapping[Any, Playlist[T]]) -> None:
-        """
-        **WARNING: NOT IMPLEMENTED YET**
-        Merge playlists from given list/map/library to this library
-        """
-        # TODO: merge playlists adding/removing tracks as needed.
-        #  Most likely will need to implement some method on playlist class too
-        raise NotImplementedError
+    def merge_playlists(
+            self,
+            playlists: Library[T] | Collection[Playlist[T]] | Mapping[str, Playlist[T]],
+            reference: Library[T] | Collection[Playlist[T]] | Mapping[str, Playlist[T]] | None = None,
+    ) -> None:
+        """
+        Merge playlists from given list/map/library to this library.
+
+        See :py:meth:`.Playlist.merge` for more info.
+
+        :param playlists: The playlists to merge onto this library's playlists.
+            If a given playlist is not found in this library, simply add the playlist to this library.
+        :param reference: Optionally, provide a reference playlist to compare both the current playlist
+            and the ``other`` items to. The function will determine tracks to remove from
+            this playlist based on the reference. Useful for using this function as a synchronizer
+            where the reference refers to the playlist at the previous sync.
+        """
+        def get_playlists_map(
+                value: Library[T] | Collection[Playlist[T]] | Mapping[str, Playlist[T]]
+        ) -> Mapping[str, Playlist[T]]:
+            """Reformat the input playlist values to map"""
+            if isinstance(value, Mapping):
+                return value
+            elif isinstance(value, Library):
+                return value.playlists
+            elif isinstance(value, Collection):
+                return {pl.name: pl for pl in value}
+            raise MusifyTypeError(f"Unrecognised input type: {value.__class__.__name__}")
+
+        playlists = get_playlists_map(playlists)
+        reference = get_playlists_map(reference) if reference is not None else {}
+
+        for name, playlist in playlists.items():
+            if name not in self.playlists:
+                self.playlists[name] = playlist
+                continue
+
+            self.playlists[name].merge(playlist, reference=reference.get(name))
 
 
-class Folder[T: Track](ItemCollection[T], metaclass=ABCMeta):
+class Folder[T: Track](MusifyCollection[T], metaclass=ABCMeta):
     """
     A folder of items and their derived properties/objects
     """
 
-    __attributes_classes__ = ItemCollection
+    __attributes_classes__ = MusifyCollection
     __attributes_ignore__ = ("name", "items")
 
     @property
     @abstractmethod
     def name(self):
         """The folder name"""
         raise NotImplementedError
@@ -501,26 +468,33 @@
     @property
     @abstractmethod
     def compilation(self) -> bool:
         """Is this folder a compilation"""
         raise NotImplementedError
 
     @property
-    @abstractmethod
-    def length(self) -> float | None:
-        """Total duration of all tracks in this folder"""
-        raise NotImplementedError
+    def length(self):
+        """Total duration of all tracks in this folder in seconds"""
+        lengths = {track.length for track in self.tracks}
+        return sum(lengths) if lengths else None
 
 
-class Album[T: Track](ItemCollection[T], metaclass=ABCMeta):
+class Album[T: Track](MusifyCollection[T], metaclass=ABCMeta):
     """An album of items and their derived properties/objects."""
 
-    __attributes_classes__ = ItemCollection
+    __attributes_classes__ = MusifyCollection
     __attributes_ignore__ = ("name", "items")
 
+    # noinspection PyPropertyDefinition
+    @classmethod
+    @property
+    def kind(cls) -> RemoteObjectType:
+        """The type of remote object associated with this class"""
+        return RemoteObjectType.ALBUM
+
     @property
     @abstractmethod
     def name(self) -> str:
         """The album name"""
         raise NotImplementedError
 
     @property
@@ -611,32 +585,39 @@
 
     @property
     def has_image(self) -> bool:
         """Does this album have an image"""
         return len(self.image_links) > 0
 
     @property
-    @abstractmethod
-    def length(self) -> float | None:
+    def length(self):
         """Total duration of all tracks on this album in seconds"""
-        raise NotImplementedError
+        lengths = {track.length for track in self.tracks}
+        return sum(lengths) if lengths else None
 
     @property
     @abstractmethod
     def rating(self) -> float | None:
         """Rating of this album"""
         raise NotImplementedError
 
 
-class Artist[T: Track](ItemCollection[T], metaclass=ABCMeta):
+class Artist[T: (Track, Album)](MusifyCollection[T], metaclass=ABCMeta):
     """An artist of items and their derived properties/objects."""
 
-    __attributes_classes__ = ItemCollection
+    __attributes_classes__ = MusifyCollection
     __attributes_ignore__ = ("name", "items")
 
+    # noinspection PyPropertyDefinition
+    @classmethod
+    @property
+    def kind(cls) -> RemoteObjectType:
+        """The type of remote object associated with this class"""
+        return RemoteObjectType.ARTIST
+
     @property
     @abstractmethod
     def name(self):
         """The artist name"""
         raise NotImplementedError
 
     @property
@@ -675,30 +656,30 @@
     @property
     @abstractmethod
     def genres(self) -> list[str]:
         """List of genres for this artist"""
         raise NotImplementedError
 
     @property
-    @abstractmethod
-    def length(self) -> float | None:
-        """Total duration of all tracks by this artist"""
-        raise NotImplementedError
+    def length(self):
+        """Total duration of all tracks by this artist in seconds"""
+        lengths = {track.length for track in self.tracks}
+        return sum(lengths) if lengths else None
 
     @property
     @abstractmethod
     def rating(self) -> int | None:
         """The popularity of this artist"""
         raise NotImplementedError
 
 
-class Genre[T: Track](ItemCollection[T], metaclass=ABCMeta):
+class Genre[T: Track](MusifyCollection[T], metaclass=ABCMeta):
     """A genre of items and their derived properties/objects."""
 
-    __attributes_classes__ = ItemCollection
+    __attributes_classes__ = MusifyCollection
     __attributes_ignore__ = ("name", "items")
 
     @property
     @abstractmethod
     def name(self):
         """The genre"""
         raise NotImplementedError
@@ -732,7 +713,13 @@
         raise NotImplementedError
 
     @property
     @abstractmethod
     def genres(self) -> list[str]:
         """List of genres ordered by frequency of appearance on the tracks for this genre"""
         raise NotImplementedError
+
+    @property
+    def length(self):
+        """Total duration of all tracks with this genre in seconds"""
+        lengths = {track.length for track in self.tracks}
+        return sum(lengths) if lengths else None
```

### Comparing `musify-0.8.1/musify/shared/remote/api.py` & `musify-0.9.0/musify/libraries/remote/core/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,89 @@
 """
 The framework for interacting with a remote API.
 
 All methods that interact with the API should return raw, unprocessed responses.
 """
-
 import logging
-from abc import ABCMeta, abstractmethod
-from collections.abc import Collection, MutableMapping, Mapping
+from abc import ABC, abstractmethod
+from collections.abc import Collection, MutableMapping, Mapping, Sequence
 from typing import Any, Self
 
-from musify.shared.api.request import RequestHandler
-from musify.shared.logger import MusifyLogger
-from musify.shared.remote.enum import RemoteIDType, RemoteObjectType
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
-from musify.shared.remote.types import APIMethodInputType
-from musify.shared.utils import align_string
+from musify.api.request import RequestHandler
+from musify.libraries.remote.core import RemoteResponse
+from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
+from musify.libraries.remote.core.types import APIInputValue
+from musify.log.logger import MusifyLogger
+from musify.types import UnitSequence, JSON, UnitList
+from musify.utils import align_string, to_collection
 
 
-class RemoteAPI(RemoteDataWrangler, metaclass=ABCMeta):
+class RemoteAPI(ABC):
     """
     Collection of endpoints for a remote API.
     See :py:class:`RequestHandler` and :py:class:`APIAuthoriser`
     for more info on which params to pass to authorise and execute requests.
 
     :param handler_kwargs: The authorisation kwargs to be passed to :py:class:`APIAuthoriser`.
     """
 
-    __slots__ = ("logger", "handler", "user_data")
+    __slots__ = ("logger", "handler", "user_data", "wrangler")
 
     #: Map of :py:class:`RemoteObjectType` for remote collections
     #: to the  :py:class:`RemoteObjectType` of the items they hold
     collection_item_map = {
         RemoteObjectType.PLAYLIST: RemoteObjectType.TRACK,
         RemoteObjectType.ALBUM: RemoteObjectType.TRACK,
         RemoteObjectType.AUDIOBOOK: RemoteObjectType.CHAPTER,
         RemoteObjectType.SHOW: RemoteObjectType.EPISODE,
     }
     #: A set of possible saved item types that can be retrieved for the currently authenticated user
     user_item_types = (
             set(collection_item_map) | {RemoteObjectType.TRACK, RemoteObjectType.ARTIST, RemoteObjectType.EPISODE}
     )
-
-    @property
-    @abstractmethod
-    def api_url_base(self) -> str:
-        """The base URL for making calls to the remote API"""
-        raise NotImplementedError
+    #: The key to use when getting an ID from a response
+    id_key = "id"
 
     @property
     @abstractmethod
     def user_id(self) -> str | None:
         """ID of the currently authorised user"""
         raise NotImplementedError
 
     @property
     @abstractmethod
     def user_name(self) -> str | None:
         """Name of the currently authorised user"""
         raise NotImplementedError
 
-    def __init__(self, **handler_kwargs):
+    @property
+    def url(self) -> str:
+        """The base URL of the API"""
+        return self.wrangler.url_api
+
+    @property
+    def source(self) -> str:
+        """The name of the API service"""
+        return self.wrangler.source
+
+    def __init__(self, wrangler: RemoteDataWrangler, **handler_kwargs):
+        super().__init__()
+        #: A :py:class:`RemoteDataWrangler` object for processing URIs
+        self.wrangler = wrangler
+
         # noinspection PyTypeChecker
         #: The :py:class:`MusifyLogger` for this  object
         self.logger: MusifyLogger = logging.getLogger(__name__)
 
-        handler_kwargs = {k: v for k, v in handler_kwargs.items() if k != "name"}
         #: The :py:class:`RequestHandler` for handling authorised requests to the API
-        self.handler = RequestHandler(name=self.source, **handler_kwargs)
+        self.handler = RequestHandler(
+            name=self.wrangler.source, **{k: v for k, v in handler_kwargs.items() if k != "name"}
+        )
+
         #: Stores the loaded user data for the currently authorised user
         self.user_data: dict[str, Any] = {}
 
     def authorise(self, force_load: bool = False, force_new: bool = False) -> Self:
         """
         Main method for authorisation, tests/refreshes/reauthorises as needed
 
@@ -79,72 +92,99 @@
         :param force_new: Ignore saved/loaded token and generate new token.
         :return: Self.
         :raise APIError: If the token cannot be validated.
         """
         self.handler.authorise(force_load=force_load, force_new=force_new)
         return self
 
+    def close(self) -> None:
+        """Close the current session. No more requests will be possible once this has been called."""
+        self.handler.close()
+
     ###########################################################################
     ## Misc helpers
     ###########################################################################
     def load_user_data(self) -> None:
         """Load and store user data in this API object for the currently authorised user"""
         self.user_data = self.get_self()
 
     @staticmethod
+    def _merge_results_to_input_mapping(
+            original: MutableMapping[str, Any], response: Mapping[str, Any], clear: bool = True,
+    ) -> None:
+        if clear:
+            original.clear()
+        original |= response
+
     def _merge_results_to_input(
-            original: APIMethodInputType, results: list[dict[str, Any]], ordered: bool = True, clear: bool = True,
+            self,
+            original: UnitSequence[JSON] | UnitSequence[RemoteResponse],
+            responses: UnitList[JSON],
+            ordered: bool = True,
+            clear: bool = True,
     ) -> None:
         """
         If API response type given on input, update with new results.
         Assumes on a one-to-one relationship between ``original`` and the list of ``results``.
 
         :param original: The original values given to the function.
-        :param results: The new results from the API.
+        :param responses: The new results from the API.
         :param ordered: When True, function assumes the order of items in ``original`` and ``results`` is the same.
             When False, the function will attempt to match each input value to each result by matching on
             the ``id`` key of each dictionary.
         :param ordered: When True, clear the original value before merging, completely replacing all original data.
         """
-        id_key = "id"
-
-        if isinstance(original, MutableMapping):
-            if not len(results) == 1:
-                return
-
-            if clear:
-                original.clear()
-            original |= results[0]
-            return
-        elif not isinstance(original, Collection):
+        if isinstance(original, str) or not isinstance(original, Collection | RemoteResponse):
             return
 
-        # process as lists
-        valid_input_types = all(isinstance(item, MutableMapping) for item in original)
-        valid_lengths = len(original) == len(results)
-        if not valid_input_types or not valid_lengths:
+        if isinstance(original, RemoteResponse):
+            original = [original]
+        elif not isinstance(original, Sequence):
+            original = to_collection(original)
+        if not isinstance(responses, Sequence):
+            responses = to_collection(responses, list)
+
+        original = [item.response if isinstance(item, RemoteResponse) else item for item in original]
+
+        valid_types_input = all(isinstance(item, MutableMapping) for item in original)
+        valid_types_responses = all(isinstance(item, MutableMapping) for item in responses)
+        valid_lengths = len(original) == len(responses)
+        if not all((valid_types_input, valid_types_responses, valid_lengths)):
+            self.logger.debug(
+                "Could not merge responses to given user input | "
+                "Reason: assertions failed | "
+                f"{valid_types_input=} {valid_types_responses=} {valid_lengths=} | "
+            )
             return
 
-        if ordered:
-            for item, res in zip(original, results):
-                if clear:
-                    item.clear()
-                item |= res
-            return
+        if not ordered:
+            expected_keys_input = all(self.id_key in item for item in original)
+            expected_keys_responses = all(self.id_key in item for item in responses)
+            if not all((expected_keys_input, expected_keys_responses)):
+                self.logger.debug(
+                    "Could not merge responses to given user input | "
+                    f"Reason: unordered and cannot order on {self.id_key=} | "
+                    f"{expected_keys_input=} {expected_keys_responses=}"
+                )
+                return
 
-        valid_keys_values = all(id_key in item for item in original)
-        valid_keys_results = all(id_key in item for item in results)
-        if not valid_keys_values or not valid_keys_results:
-            return
+            id_ordered = [response[self.id_key] for response in original]
+            responses.sort(key=lambda response: id_ordered.index(response[self.id_key]))
 
-        result_mapped = {result[id_key]: result for result in results if result}
-        for item in original:
-            if clear:
-                item.clear()
-            item |= result_mapped[item[id_key]]
+        for item, response in zip(original, responses):
+            self._merge_results_to_input_mapping(original=item, response=response, clear=clear)
+
+    @staticmethod
+    def _refresh_responses(responses: Any, skip_checks: bool = False) -> None:
+        if isinstance(responses, RemoteResponse):
+            responses = [responses]
+
+        for response in responses:
+            if isinstance(response, RemoteResponse):
+                response.refresh(skip_checks=skip_checks)
 
     def print_item(
             self, i: int, name: str, uri: str, length: float = 0, total: int = 1, max_width: int = 50
     ) -> None:
         """
         Pretty print item data for displaying to the user.
         Format = ``<i> - <name> | <length> | <URI> - <URL>``.
@@ -157,44 +197,45 @@
         :param max_width: The maximum width to print names as. Any name lengths longer than this will be truncated.
         """
         print(
             f"\t\33[92m{str(i).zfill(len(str(total)))} \33[0m- "
             f"\33[97m{align_string(name, max_width=max_width)} \33[0m| "
             f"\33[91m{str(int(length // 60)).zfill(2)}:{str(round(length % 60)).zfill(2)} \33[0m| "
             f"\33[93m{uri} \33[0m- "
-            f"{self.convert(uri, type_in=RemoteIDType.URI, type_out=RemoteIDType.URL_EXT)}"
+            f"{self.wrangler.convert(uri, type_in=RemoteIDType.URI, type_out=RemoteIDType.URL_EXT)}"
         )
 
     @abstractmethod
     def print_collection(
             self,
-            value: str | Mapping[str, Any] | None = None,
+            value: str | Mapping[str, Any] | RemoteResponse | None = None,
             kind: RemoteIDType | None = None,
             limit: int = 20,
             use_cache: bool = True
     ) -> None:
         """
         Pretty print collection data for displaying to the user.
         Runs :py:meth:`print_item()` for each item in the collection.
 
         ``value`` may be:
             * A string representing a URL/URI/ID.
             * A remote API JSON response for a collection with a valid ID value under an ``id`` key.
+            * A RemoteResponse representing some remote collection of items.
 
         :param value: The value representing some remote collection. See description for allowed value types.
         :param kind: When an ID is provided, give the kind of ID this is here.
             If None and ID is given, user will be prompted to give the kind anyway.
         :param limit: The number of results to call per request and,
             therefore, the number of items in each printed block.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def get_playlist_url(self, playlist: str, use_cache: bool = True) -> str:
+    def get_playlist_url(self, playlist: str | Mapping[str, Any] | RemoteResponse, use_cache: bool = True) -> str:
         """
         Determine the type of the given ``playlist`` and return its API URL.
         If type cannot be determined, attempt to find the playlist in the
         list of the currently authenticated user's playlists.
 
         :param playlist: In URL/URI/ID form, or the name of one of the currently authenticated user's playlists.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
@@ -232,53 +273,61 @@
 
     ###########################################################################
     ## Item - GET endpoints
     ###########################################################################
     @abstractmethod
     def extend_items(
             self,
-            items_block: MutableMapping[str, Any],
+            response: MutableMapping[str, Any] | RemoteResponse,
             kind: RemoteObjectType | str | None = None,
             key: RemoteObjectType | None = None,
             use_cache: bool = True,
     ) -> list[dict[str, Any]]:
         """
-        Extend the items for a given ``items_block`` API response.
+        Extend the items for a given API ``response``.
         The function requests each page of the collection returning a list of all items
         found across all pages for this URL.
 
         Updates the value of the ``items`` key in-place by extending the value of the ``items`` key with new results.
 
-        :param items_block: A remote API JSON response for an items type endpoint.
+        If a :py:class:`RemoteResponse`, this function will not refresh itself with the new response.
+        The user must call `refresh` manually after execution.
+
+        :param response: A remote API JSON response for an items type endpoint.
         :param kind: The type of response being extended. Optional, used only for logging.
         :param key: The type of response of the child objects.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         :return: API JSON responses for each item
         """
         raise NotImplementedError
 
     @abstractmethod
     def get_items(
             self,
-            values: APIMethodInputType,
+            values: APIInputValue,
             kind: RemoteObjectType | None = None,
             limit: int = 50,
             extend: bool = True,
             use_cache: bool = True,
     ) -> list[dict[str, Any]]:
         """
-        ``GET: /{kind}s`` - Get information for given ``values``.
+        ``GET`` - Get information for given ``values``.
 
         ``values`` may be:
             * A string representing a URL/URI/ID.
             * A MutableSequence of strings representing URLs/URIs/IDs of the same type.
             * A remote API JSON response for a collection.
             * A MutableSequence of remote API JSON responses for a collection.
+            * A RemoteResponse of the appropriate type for this RemoteAPI which holds a valid API JSON response
+              as described above.
+            * A Sequence of RemoteResponses as above.
+
+        If JSON response(s) given, this updates each response given by merging with the new response.
 
-        If JSON response(s) given, this update each response given by merging with the new response.
+        If :py:class:`RemoteResponse` values are given, this function will call `refresh` on them.
 
         :param values: The values representing some remote objects. See description for allowed value types.
             These items must all be of the same type of item i.e. all tracks OR all artists etc.
         :param kind: Item type if given string is ID.
         :param limit: When requests can be batched, size of batches to request.
             This value will be limited to be between ``1`` and ``50``.
         :param extend: When True and the given ``kind`` is a collection of items,
@@ -288,15 +337,15 @@
         :raise RemoteObjectTypeError: Raised when the function cannot determine the item type
             of the input ``values``. Or when it does not recognise the type of the input ``values`` parameter.
         """
         raise NotImplementedError
 
     @abstractmethod
     def get_tracks(
-            self, values: APIMethodInputType, limit: int = 50, use_cache: bool = True, *args, **kwargs,
+            self, values: APIInputValue, limit: int = 50, use_cache: bool = True, *args, **kwargs,
     ) -> list[dict[str, Any]]:
         """
         Wrapper for :py:meth:`get_items` which only returns Track type responses.
         See :py:meth:`get_items` for more info.
         """
         raise NotImplementedError
 
@@ -333,23 +382,28 @@
         :param name: Name of playlist to create.
         :return: API URL for playlist.
         """
         raise NotImplementedError
 
     @abstractmethod
     def add_to_playlist(
-            self, playlist: str | Mapping[str, Any], items: Collection[str], limit: int = 50, skip_dupes: bool = True
+            self,
+            playlist: str | Mapping[str, Any] | RemoteResponse,
+            items: Collection[str],
+            limit: int = 50,
+            skip_dupes: bool = True
     ) -> int:
         """
         ``POST`` - Add list of tracks to a given playlist.
 
         :param playlist: One of the following to identify the playlist to clear:
             - playlist URL/URI/ID,
             - the name of the playlist in the current user's playlists,
             - the API response of a playlist.
+            - a RemoteResponse object representing a remote playlist.
         :param items: List of URLs/URIs/IDs of the tracks to add.
         :param limit: Size of each batch of IDs to add. This value will be limited to be between ``1`` and ``50``.
         :param skip_dupes: Skip duplicates.
         :return: The number of tracks added to the playlist.
         :raise RemoteIDTypeError: Raised when the input ``playlist`` does not represent
             a playlist URL/URI/ID.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``items``
@@ -357,42 +411,53 @@
         """
         raise NotImplementedError
 
     ###########################################################################
     ## Collection - DELETE endpoints
     ###########################################################################
     @abstractmethod
-    def delete_playlist(self, playlist: str | Mapping[str, Any]) -> str:
+    def delete_playlist(self, playlist: str | Mapping[str, Any] | RemoteResponse) -> str:
         """
         ``DELETE`` - Unfollow/delete a given playlist.
         WARNING: This function will destructively modify your remote playlists.
 
         :param playlist: One of the following to identify the playlist to clear:
             - playlist URL/URI/ID,
             - the name of the playlist in the current user's playlists,
             - the API response of a playlist.
+            - a RemoteResponse object representing a remote playlist.
         :return: API URL for playlist.
         """
         raise NotImplementedError
 
     @abstractmethod
     def clear_from_playlist(
-            self, playlist: str | Mapping[str, Any], items: Collection[str] | None = None, limit: int = 100
+            self,
+            playlist: str | Mapping[str, Any] | RemoteResponse,
+            items: Collection[str] | None = None,
+            limit: int = 100
     ) -> int:
         """
         ``DELETE`` - Clear tracks from a given playlist.
         WARNING: This function can destructively modify your remote playlists.
 
         :param playlist: One of the following to identify the playlist to clear:
             - playlist URL/URI/ID,
             - the name of the playlist in the current user's playlists,
             - the API response of a playlist.
+            - a RemoteResponse object representing a remote playlist.
         :param items: List of URLs/URIs/IDs of the tracks to remove. If None, clear all songs from the playlist.
         :param limit: Size of each batch of IDs to clear in a single request.
             This value will be limited to be between ``1`` and ``100``.
         :return: The number of tracks cleared from the playlist.
-        :raise RemoteIDTypeError: Raised when the input ``playlist`` does not represent
-            a playlist URL/URI/ID.
+        :raise RemoteIDTypeError: Raised when the input ``playlist`` does not represent a playlist URL/URI/ID.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``items``
             are not all tracks or IDs.
         """
         raise NotImplementedError
+
+    def __enter__(self):
+        self.handler.__enter__()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.handler.__exit__(exc_type, exc_val, exc_tb)
```

### Comparing `musify-0.8.1/musify/shared/remote/base.py` & `musify-0.9.0/musify/libraries/remote/core/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 """
 Core abstract classes for the :py:mod:`Remote` module.
 
 These define the foundations of any remote object or item.
 """
-
 from abc import ABCMeta, abstractmethod
+from collections.abc import Mapping
 from typing import Any, Self
 
-from musify.shared.api.exception import APIError
-from musify.shared.core.base import AttributePrinter, NameableTaggableMixin, Item
-from musify.shared.remote import Remote
-from musify.shared.remote.api import RemoteAPI
+from musify.api.exception import APIError
+from musify.core.base import MusifyItem
+from musify.libraries.remote.core import RemoteResponse
+from musify.libraries.remote.core.api import RemoteAPI
 
 
-class RemoteObject(AttributePrinter, NameableTaggableMixin, Remote, metaclass=ABCMeta):
+class RemoteObject[T: (RemoteAPI | None)](RemoteResponse, metaclass=ABCMeta):
     """
     Generic base class for remote objects. Extracts key data from a remote API JSON response.
 
     :param response: The remote API JSON response
     :param api: The instantiated and authorised API object for this source type.
     """
 
     __slots__ = ("_response", "api")
-    __attributes_ignore__ = ("api", "response")
+    __attributes_ignore__ = ("response", "api")
 
     _url_pad = 71
 
     @property
     @abstractmethod
-    def id(self) -> str:
-        """The ID of this item/collection."""
-        raise NotImplementedError
-
-    @property
-    @abstractmethod
     def uri(self) -> str:
         """The URI of this item/collection."""
         raise NotImplementedError
 
     @property
     @abstractmethod
     def has_uri(self) -> bool:
@@ -57,33 +51,25 @@
         raise NotImplementedError
 
     @property
     def response(self) -> dict[str, Any]:
         """The API response for this object"""
         return self._response
 
-    def __init__(self, response: dict[str, Any], api: RemoteAPI | None = None, skip_checks: bool = False):
+    def __init__(self, response: dict[str, Any], api: T = None, skip_checks: bool = False):
         super().__init__()
         self._response = response
 
         #: The :py:class:`RemoteAPI` to call when reloading
         self.api = api
 
         self._check_type()
         self.refresh(skip_checks=skip_checks)
 
     @abstractmethod
-    def refresh(self, skip_checks: bool = False) -> None:
-        """
-        Refresh this object by updating from the stored API response.
-        Useful for updating stored variables after making changes to the stored API response manually.
-        """
-        raise NotImplementedError
-
-    @abstractmethod
     def _check_type(self) -> None:
         """
         Checks the given response is compatible with this object type, raises an exception if not.
 
         :raise RemoteObjectTypeError: When the response type is not compatible with this object.
         """
         raise NotImplementedError
@@ -95,41 +81,50 @@
         :raise APIError: When the API has not been set for this instance.
         """
         if self.api is None:
             raise APIError("API is not set. Assign an API to this instance first.")
 
     @classmethod
     @abstractmethod
-    def load(cls, value: str | dict[str, Any], api: RemoteAPI, use_cache: bool = True, *args, **kwargs) -> Self:
+    def load(
+            cls,
+            value: str | Mapping[str, Any] | RemoteResponse,
+            api: RemoteAPI,
+            use_cache: bool = True,
+            *args,
+            **kwargs
+    ) -> Self:
         """
         Generate a new object of this class,
         calling all required endpoints to get a complete set of data for this item type.
 
         ``value`` may be:
             * A string representing a URL/URI/ID.
             * A remote API JSON response for a collection with a valid ID value under an ``id`` key.
+            * An object of the same type as this collection.
+              The remote API JSON response will be used to load a new object.
 
         :param value: The value representing some remote object. See description for allowed value types.
         :param api: An authorised API object to load the object from.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         """
         raise NotImplementedError
 
     @abstractmethod
     def reload(self, use_cache: bool = True, *args, **kwargs) -> None:
         """
         Reload this object from the API, calling all required endpoints
-        to get a complete set of data for this item type
+        to get a complete set of data for this item type.
 
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         """
         raise NotImplementedError
 
     def __hash__(self):
         """Uniqueness of a remote object is its URI"""
         return hash(self.uri)
 
 
-class RemoteItem(RemoteObject, Item, metaclass=ABCMeta):
+class RemoteItem(RemoteObject, MusifyItem, metaclass=ABCMeta):
     """Generic base class for remote items. Extracts key data from a remote API JSON response."""
 
-    __attributes_classes__ = (RemoteObject, Item)
+    __attributes_classes__ = (RemoteObject, MusifyItem)
```

### Comparing `musify-0.8.1/musify/shared/remote/enum.py` & `musify-0.9.0/musify/libraries/remote/core/enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 The fundamental core enum classes for the :py:mod:`Remote` module.
 
 Represents ID and item types.
 """
-
-from musify.shared.core.enum import MusifyEnum
+from musify.core.enum import MusifyEnum
 
 
 class RemoteIDType(MusifyEnum):
     """Represents remote ID types"""
     ALL: int = 0
 
     #: Value is the expected length of ID string
```

### Comparing `musify-0.8.1/musify/shared/remote/exception.py` & `musify-0.9.0/musify/libraries/remote/core/exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Exceptions relating to remote operations.
 """
-
 from typing import Any
 
-from musify.shared.exception import MusifyError
-from musify.shared.remote.enum import RemoteIDType, RemoteObjectType
+from musify.exception import MusifyError
+from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
 
 
 class RemoteError(MusifyError):
     """Exception raised for remote errors"""
 
 
 ###########################################################################
```

### Comparing `musify-0.8.1/musify/shared/remote/library.py` & `musify-0.9.0/musify/libraries/remote/core/library.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,183 +1,184 @@
 """
 Functionality relating to a generic remote library.
 """
-
 from abc import ABCMeta, abstractmethod
 from collections.abc import Collection, Mapping, Iterable
 from typing import Any, Literal
 
+from musify.core.base import MusifyItem
+from musify.libraries.core.object import Track, Library, Playlist
+from musify.libraries.remote.core.api import RemoteAPI
+from musify.libraries.remote.core.enum import RemoteObjectType
+from musify.libraries.remote.core.factory import RemoteObjectFactory
+from musify.libraries.remote.core.object import RemoteCollection, SyncResultRemotePlaylist
+from musify.libraries.remote.core.object import RemoteTrack, RemotePlaylist, RemoteArtist, RemoteAlbum
+from musify.log import STAT
 from musify.processors.base import Filter
 from musify.processors.filter import FilterDefinedList
-from musify.shared.core.base import Item
-from musify.shared.core.object import Track, Library, Playlist
-from musify.shared.logger import STAT
-from musify.shared.remote.api import RemoteAPI
-from musify.shared.remote.config import RemoteObjectClasses
-from musify.shared.remote.enum import RemoteObjectType
-from musify.shared.remote.object import RemoteTrack, RemoteCollection, RemotePlaylist, SyncResultRemotePlaylist, \
-    RemoteArtist, RemoteAlbum
-from musify.shared.utils import align_string, get_max_width
+from musify.utils import align_string, get_max_width
 
 
-class RemoteLibrary[T: RemoteTrack](Library[T], RemoteCollection[T], metaclass=ABCMeta):
+class RemoteLibrary[
+    A: RemoteAPI, PL: RemotePlaylist, TR: RemoteTrack, AL: RemoteAlbum, AR: RemoteArtist
+](RemoteCollection[TR], Library[TR], metaclass=ABCMeta):
     """
     Represents a remote library, providing various methods for manipulating
     tracks and playlists across an entire remote library collection.
 
-    :param api: An authorised API object for the authenticated user you wish to load the library from.
+    :param api: The instantiated and authorised API object for this source type.
     :param playlist_filter: An optional :py:class:`Filter` to apply or collection of playlist names to include when
         loading playlists. Playlist names will be passed to this filter to limit which playlists are loaded.
     :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
     """
 
-    __slots__ = ("_api", "_tracks", "_playlists", "playlist_filter", "use_cache")
+    __slots__ = ("_factory", "_tracks", "_playlists", "playlist_filter")
     __attributes_classes__ = (Library, RemoteCollection)
-    __attributes_ignore__ = ("api", "_object_cls")
+    __attributes_ignore__ = ("api", "factory")
 
     @property
+    def factory(self) -> RemoteObjectFactory[A, PL, TR, AL, AR]:
+        """Stores the key object classes for a remote source."""
+        return self._factory
+
     @abstractmethod
-    def _object_cls(self) -> RemoteObjectClasses:
+    def _create_factory(self, api: A) -> RemoteObjectFactory[A, PL, TR, AL, AR]:
         """Stores the key object classes for a remote source."""
         raise NotImplementedError
 
     @property
+    def api(self):
+        """Authorised API object for making authenticated calls to a user's library"""
+        return self.factory.api
+
+    @property
     def name(self):
         """The username associated with this library"""
         return self.api.user_name
 
     @property
     def id(self):
         """The user ID associated with this library"""
         return self.api.user_id
 
     @property
-    def playlists(self) -> dict[str, RemotePlaylist[T]]:
+    def playlists(self) -> dict[str, PL]:
         return self._playlists
 
     @property
-    def tracks(self) -> list[T]:
+    def tracks(self) -> list[TR]:
         """All user's saved tracks"""
         return self._tracks
 
     @property
-    def artists(self) -> list[RemoteArtist[T]]:
+    def artists(self) -> list[AR]:
         """All user's saved artists"""
         return self._artists
 
     @property
-    def albums(self) -> list[RemoteAlbum[T]]:
+    def albums(self) -> list[AL]:
         """All user's saved albums"""
         return self._albums
 
-    @property
-    def api(self) -> RemoteAPI:
-        """Authorised API object for making authenticated calls to a user's library"""
-        return self._api
-
-    def __init__(
-            self,
-            api: RemoteAPI,
-            use_cache: bool = True,
-            playlist_filter: Collection[str] | Filter[str] = (),
-    ):
-        super().__init__()
+    def __init__(self, api: A, use_cache: bool = True, playlist_filter: Collection[str] | Filter[str] = ()):
+        super().__init__(remote_wrangler=api.wrangler)
 
-        self._api = api
         #: When true, use the cache when calling the API endpoint
         self.use_cache = use_cache
 
         if not isinstance(playlist_filter, Filter):
             playlist_filter = FilterDefinedList(playlist_filter)
         #: :py:class:`Filter` to filter out the playlists loaded by name.
         self.playlist_filter: Filter[str] = playlist_filter
 
-        self._playlists: dict[str, RemotePlaylist[T]] = {}
-        self._tracks: list[T] = []
-        self._albums: list[RemoteAlbum[T]] = []
-        self._artists: list[RemoteArtist[T]] = []
+        self._factory = self._create_factory(api=api)
+        self._playlists: dict[str, PL] = {}
+        self._tracks: list[TR] = []
+        self._albums: list[AL] = []
+        self._artists: list[AR] = []
 
-    def extend(self, __items: Iterable[Item], allow_duplicates: bool = True) -> None:
-        self.logger.debug(f"Extend {self.source} tracks data: START")
+    def extend(self, __items: Iterable[MusifyItem], allow_duplicates: bool = True) -> None:
+        self.logger.debug(f"Extend {self.api.source} tracks data: START")
         if not allow_duplicates:
             self.logger.info(
                 "\33[1;95m ->\33[1;97m Extending library: "
                 "checking if the given items are already in this library \33[0m"
             )
 
         load_uris = []
         bar = self.logger.get_progress_bar(iterable=__items, desc="Checking items", unit="items")
         for item in bar:
             if not allow_duplicates and item in self.items:
                 continue
-            elif isinstance(item, self._object_cls.track):
+            elif isinstance(item, RemoteTrack):
                 self.items.append(item)
             elif item.has_uri:
                 load_uris.append(item.uri)
 
         if not load_uris:
             return
 
         self.logger.info(
-            f"\33[1;95m  >\33[1;97m Extending {self.source} library with {len(load_uris)} additional tracks \33[0m"
+            f"\33[1;95m  >\33[1;97m Extending {self.api.source} library "
+            f"with {len(load_uris)} additional tracks \33[0m"
         )
 
         load_tracks = self.api.get_tracks(load_uris, features=True, use_cache=self.use_cache)
-        self.items.extend(self._object_cls.track(response=response, api=self.api) for response in load_tracks)
+        self.items.extend(self.factory.track(response=response) for response in load_tracks)
 
         self.logger.print()
         self.log_tracks()
-        self.logger.debug(f"Extend {self.source} tracks data: DONE\n")
+        self.logger.debug(f"Extend {self.api.source} tracks data: DONE\n")
 
     def load(self) -> None:
         """Loads all data from the remote API for this library and log results."""
-        self.logger.debug(f"Load {self.source} library: START")
-        self.logger.info(f"\33[1;95m ->\33[1;97m Loading {self.source} library \33[0m")
+        self.logger.debug(f"Load {self.api.source} library: START")
+        self.logger.info(f"\33[1;95m ->\33[1;97m Loading {self.api.source} library \33[0m")
 
         self.load_playlists()
         self.load_tracks()
         self.load_saved_albums()
         self.load_saved_artists()
 
         self.logger.print(STAT)
         self.log_playlists()
         self.log_tracks()
         self.log_albums()
         self.log_artists()
 
         self.logger.print()
-        self.logger.debug(f"Load {self.source} library: DONE\n")
+        self.logger.debug(f"Load {self.api.source} library: DONE\n")
 
     ###########################################################################
     ## Load - playlists
     ###########################################################################
     def load_playlists(self) -> None:
         """
         Load all playlists from the API that match the filter rules in this library. Also loads all their tracks.
         WARNING: Overwrites any currently loaded playlists.
         """
-        self.logger.debug(f"Load {self.source} playlists: START")
+        self.logger.debug(f"Load {self.api.source} playlists: START")
         self.api.load_user_data()
 
         responses = self.api.get_user_items(kind=RemoteObjectType.PLAYLIST, use_cache=self.use_cache)
         responses = self._filter_playlists(responses)
 
         self.logger.info(
             f"\33[1;95m  >\33[1;97m Getting {self._get_total_tracks(responses=responses)} "
-            f"{self.source} tracks from {len(responses)} playlists \33[0m"
+            f"{self.api.source} tracks from {len(responses)} playlists \33[0m"
         )
         self.api.get_items(responses, kind=RemoteObjectType.PLAYLIST, use_cache=self.use_cache)
 
         playlists = [
-            self._object_cls.playlist(response=r, api=self.api, skip_checks=False)
+            self.factory.playlist(response=r, skip_checks=False)
             for r in self.logger.get_progress_bar(iterable=responses, desc="Processing playlists", unit="playlists")
         ]
 
         self._playlists = {pl.name: pl for pl in sorted(playlists, key=lambda x: x.name.casefold())}
-        self.logger.debug(f"Load {self.source} playlists: DONE")
+        self.logger.debug(f"Load {self.api.source} playlists: DONE")
 
     def _filter_playlists(self, responses: list[dict[str, Any]]) -> list[dict[str, Any]]:
         """
         Filter API responses from all playlists according to filter rules in this library.
 
         :return: Filtered API responses.
         """
@@ -190,45 +191,45 @@
         :return: Total track count.
         """
         raise NotImplementedError
 
     def log_playlists(self) -> None:
         max_width = get_max_width(self.playlists)
 
-        self.logger.stat(f"\33[1;96m{self.source} PLAYLISTS: \33[0m")
+        self.logger.stat(f"\33[1;96m{self.api.source.upper()} PLAYLISTS: \33[0m")
         for name, playlist in self.playlists.items():
             name = align_string(playlist.name, max_width=max_width)
             self.logger.stat(f"\33[97m{name} \33[0m| \33[92m{len(playlist):>6} total tracks \33[0m")
 
     ###########################################################################
     ## Load - tracks
     ###########################################################################
     def load_tracks(self) -> None:
         """
         Load all user's saved tracks from the API.
         Updates currently loaded tracks in-place or appends if not already loaded.
         """
-        self.logger.debug(f"Load user's saved {self.source} tracks: START")
+        self.logger.debug(f"Load user's saved {self.api.source} tracks: START")
         self.api.load_user_data()
 
         responses = self.api.get_user_items(kind=RemoteObjectType.TRACK, use_cache=self.use_cache)
         for response in self.logger.get_progress_bar(iterable=responses, desc="Processing tracks", unit="tracks"):
-            track = self._object_cls.track(response=response, api=self.api, skip_checks=True)
+            track = self.factory.track(response=response, skip_checks=True)
 
             if not track.has_uri:  # skip any invalid non-remote responses
                 continue
 
             current = next((item for item in self._tracks if item == track), None)
             if current is None:
                 self._tracks.append(track)
             else:
                 current._response = track.response
-                current.refresh()
+                current.refresh(skip_checks=False)
 
-        self.logger.debug(f"Load user's saved {self.source} tracks: DONE")
+        self.logger.debug(f"Load user's saved {self.api.source} tracks: DONE")
 
     def enrich_tracks(self, *_, **__) -> None:
         """
         Call API to enrich elements of track objects improving metadata coverage.
         This is an optionally implementable method. Defaults to doing nothing.
         """
         self.logger.debug("Enrich tracks not implemented for this library, skipping...")
@@ -237,101 +238,101 @@
         playlist_tracks = [track.uri for tracks in self.playlists.values() for track in tracks]
         in_playlists = len([track for track in self.tracks if track.uri in playlist_tracks])
         album_tracks = [track.uri for tracks in self.albums for track in tracks]
         in_albums = len([track for track in self.tracks if track.uri in album_tracks])
 
         width = get_max_width(self.playlists)
         self.logger.stat(
-            f"\33[1;96m{"USER'S " + self.source.upper() + " TRACKS":<{width}}\33[1;0m |"
+            f"\33[1;96m{"USER'S " + self.api.source.upper() + " TRACKS":<{width}}\33[1;0m |"
             f"\33[92m{in_playlists:>7} in playlists  \33[0m|"
             f"\33[92m{in_albums:>7} in saved albums \33[0m|"
             f"\33[1;94m{len(self.tracks):>7} total tracks \33[0m"
         )
 
     ###########################################################################
     ## Load - albums
     ###########################################################################
     def load_saved_albums(self) -> None:
         """
         Load all user's saved albums from the API.
         Updates currently loaded albums in-place or appends if not already loaded.
         """
-        self.logger.debug(f"Load user's saved {self.source} albums: START")
+        self.logger.debug(f"Load user's saved {self.api.source} albums: START")
         self.api.load_user_data()
 
         responses = self.api.get_user_items(kind=RemoteObjectType.ALBUM, use_cache=self.use_cache)
         for response in self.logger.get_progress_bar(iterable=responses, desc="Processing albums", unit="albums"):
-            album = self._object_cls.album(response=response, api=self.api, skip_checks=True)
+            album = self.factory.album(response=response, skip_checks=True)
 
             current = next((item for item in self._albums if item == album), None)
             if current is None:
                 self._albums.append(album)
             else:
                 current._response = album.response
                 current.refresh(skip_checks=True)
 
             for track in album.tracks:  # add tracks from this album to the user's saved tracks
                 if track not in self.tracks:
                     self._tracks.append(track)
 
-        self.logger.debug(f"Load user's saved {self.source} albums: DONE")
+        self.logger.debug(f"Load user's saved {self.api.source} albums: DONE")
 
     def enrich_saved_albums(self, *_, **__) -> None:
         """
         Call API to enrich elements of user's saved album objects improving metadata coverage.
         This is an optionally implementable method. Defaults to doing nothing.
         """
         self.logger.debug("Enrich albums not implemented for this library, skipping...")
 
     def log_albums(self) -> None:
         """Log stats on currently loaded albums"""
         width = get_max_width(self.playlists)
         self.logger.stat(
-            f"\33[1;96m{"USER'S " + self.source.upper() + " ALBUMS":<{width}}\33[1;0m |"
+            f"\33[1;96m{"USER'S " + self.api.source.upper() + " ALBUMS":<{width}}\33[1;0m |"
             f"\33[92m{sum(len(album.tracks) for album in self.albums):>7} album tracks  \33[0m|"
             f"\33[92m{sum(len(album.artists) for album in self.albums):>7} album artists   \33[0m|"
             f"\33[1;94m{len(self.artists):>7} total albums \33[0m"
         )
 
     ###########################################################################
     ## Load - artists
     ###########################################################################
     def load_saved_artists(self) -> None:
         """
         Load all user's saved artists from the API.
         Updates currently loaded artists in-place or appends if not already loaded.
         """
-        self.logger.debug(f"Load user's saved {self.source} artists: START")
+        self.logger.debug(f"Load user's saved {self.api.source} artists: START")
         self.api.load_user_data()
 
         responses = self.api.get_user_items(kind=RemoteObjectType.ARTIST, use_cache=self.use_cache)
         for response in self.logger.get_progress_bar(iterable=responses, desc="Processing artists", unit="artists"):
-            artist = self._object_cls.artist(response=response, api=self.api, skip_checks=True)
+            artist = self.factory.artist(response=response, skip_checks=True)
 
             current = next((item for item in self._artists if item == artist), None)
             if current is None:
                 self._artists.append(artist)
             else:
                 current._response = artist.response
                 current.refresh(skip_checks=True)
 
-        self.logger.debug(f"Load user's saved {self.source} artists: DONE")
+        self.logger.debug(f"Load user's saved {self.api.source} artists: DONE")
 
     def enrich_saved_artists(self, *_, **__) -> None:
         """
         Call API to enrich elements of user's saved artist objects improving metadata coverage.
         This is an optionally implementable method. Defaults to doing nothing.
         """
         self.logger.debug("Enrich artists not implemented for this library, skipping...")
 
     def log_artists(self) -> None:
         """Log stats on currently loaded artists"""
         width = get_max_width(self.playlists)
         self.logger.stat(
-            f"\33[1;96m{"USER'S " + self.source.upper() + " ARTISTS":<{width}}\33[1;0m |"
+            f"\33[1;96m{"USER'S " + self.api.source.upper() + " ARTISTS":<{width}}\33[1;0m |"
             f"\33[92m{sum(len(artist.tracks) for artist in self.artists):>7} artist tracks \33[0m|"
             f"\33[92m{sum(len(artist.albums) for artist in self.artists):>7} artist albums   \33[0m|"
             f"\33[1;94m{len(self.artists):>7} total artists \33[0m"
         )
 
     ###########################################################################
     ## Backup/Restore/Sync
@@ -356,46 +357,49 @@
         When ``dry_run`` is False, this function does create new playlists on the remote library for playlists
         given that do not exist in this Library.
 
         :param playlists: Values that represent the playlists to restore from.
         :param dry_run: When True, do not create playlists
             and just skip any playlists that are not already currently loaded.
         """
-        # TODO: expand this function to support all RemoteItem types + update input type
         if isinstance(playlists, Library):  # get URIs from playlists in library
             playlists = {name: [track.uri for track in pl] for name, pl in playlists.playlists.items()}
-        elif isinstance(playlists, Mapping) and all(isinstance(v, Item) for vals in playlists.values() for v in vals):
+        elif (
+                isinstance(playlists, Mapping)
+                and all(isinstance(v, MusifyItem) for vals in playlists.values() for v in vals)
+        ):
             # get URIs from playlists in map values
             playlists = {name: [item.uri for item in pl] for name, pl in playlists.items()}
         elif not isinstance(playlists, Mapping) and isinstance(playlists, Collection):
             # get URIs from playlists in collection
             playlists = {pl.name: [track.uri for track in pl] for pl in playlists}
         playlists: Mapping[str, Iterable[str]]
 
         uri_tracks = {track.uri: track for track in self.tracks}
         uri_get = [uri for uri_list in playlists.values() for uri in uri_list if uri not in uri_tracks]
 
         if uri_get:
             tracks_data = self.api.get_tracks(uri_get, features=False, use_cache=self.use_cache)
-            tracks = list(map(lambda response: self._object_cls.track(api=self.api, response=response), tracks_data))
+            tracks = list(map(self.factory.track, tracks_data))
             uri_tracks |= {track.uri: track for track in tracks}
 
         for name, uri_list in playlists.items():
             playlist = self.playlists.get(name)
             if not playlist and dry_run:  # skip on dry run
                 continue
             if not playlist:  # new playlist given, create it on remote first
-                playlist = self._object_cls.playlist.create(name=name, api=self.api)
+                # noinspection PyArgumentList
+                playlist = self.factory.playlist.create(name=name)
 
             playlist._tracks = [uri_tracks.get(uri) for uri in uri_list]
             self.playlists[name] = playlist
 
     def sync(
             self,
-            playlists: Library | Mapping[str, Iterable[Item]] | Collection[Playlist] | None = None,
+            playlists: Library | Mapping[str, Iterable[MusifyItem]] | Collection[Playlist] | None = None,
             kind: Literal["new", "refresh", "sync"] = "new",
             reload: bool = True,
             dry_run: bool = True
     ) -> dict[str, SyncResultRemotePlaylist]:
         """
         Synchronise this playlist object with the remote playlist it is associated with.
 
@@ -411,57 +415,64 @@
             Use the currently loaded ``playlists`` in this object if not given.
         :param kind: Sync option for the remote playlist. See description.
         :param reload: When True, once synchronisation is complete, reload this RemotePlaylist object
             to reflect the changes on the remote playlist if enabled. Skip if False.
         :param dry_run: Run function, but do not modify the remote playlists at all.
         :return: Map of playlist name to the results of the sync as a :py:class:`SyncResultRemotePlaylist` object.
         """
-        self.logger.debug(f"Sync {self.source} playlists: START")
+        self.logger.debug(f"Sync {self.api.source} playlists: START")
 
         if not playlists:  # use the playlists as stored in this library object
             playlists = self.playlists
         elif isinstance(playlists, Library):  # get map of playlists from the given library
             playlists = playlists.playlists
         elif isinstance(playlists, Collection) and all(isinstance(pl, Playlist) for pl in playlists):
             # reformat list to map
             playlists = {pl.name: pl for pl in playlists}
-        playlists: Mapping[str, Iterable[Item]]
+        playlists: Mapping[str, Iterable[MusifyItem]]
 
         log_kind = "adding new items only"
         if kind != "new":
             log_kind = 'all' if kind == 'refresh' else 'extra'
-            log_kind = f"clearing {log_kind} items from {self.source} playlist first"
+            log_kind = f"clearing {log_kind} items from {self.api.source} playlist first"
         self.logger.info(
-            f"\33[1;95m ->\33[1;97m Synchronising {len(playlists)} {self.source} playlists: {log_kind}"
+            f"\33[1;95m ->\33[1;97m Synchronising {len(playlists)} {self.api.source} playlists: {log_kind}"
             f"{f' and reloading stored playlists' if reload else ''} \33[0m"
         )
 
         bar = self.logger.get_progress_bar(
-            iterable=playlists.items(), desc=f"Synchronising {self.source}", unit="playlists"
+            iterable=playlists.items(), desc=f"Synchronising {self.api.source}", unit="playlists"
         )
         results = {}
         for name, pl in bar:  # synchronise playlists
             if name not in self.playlists:  # new playlist given, create it on remote first
-                self.playlists[name] = self._object_cls.playlist.create(name=name, api=self.api)
+                if dry_run:
+                    results[name] = SyncResultRemotePlaylist(
+                        start=0, added=len(pl), removed=0, unchanged=0, difference=len(pl), final=len(pl)
+                    )
+                    continue
+
+                # noinspection PyArgumentList
+                self.playlists[name] = self.factory.playlist.create(name=name)
             results[name] = self.playlists[name].sync(items=pl, kind=kind, reload=reload, dry_run=dry_run)
 
         self.logger.print()
-        self.logger.debug(f"Sync {self.source} playlists: DONE\n")
+        self.logger.debug(f"Sync {self.api.source} playlists: DONE\n")
         return results
 
     def log_sync(self, results: SyncResultRemotePlaylist | Mapping[str, SyncResultRemotePlaylist]) -> None:
         """Log stats from the results of a ``sync`` operation"""
         if not results:
             return
         if not isinstance(results, Mapping):
             results = {"": results}
 
-        max_width = get_max_width(self.playlists)
+        max_width = get_max_width(results)
 
-        self.logger.stat(f"\33[1;96mSync {self.source} playlists' stats: \33[0m")
+        self.logger.stat(f"\33[1;96mSync {self.api.source} playlists' stats: \33[0m")
         for name, result in results.items():
             self.logger.stat(
                 f"\33[97m{align_string(name, max_width=max_width)} \33[0m|"
                 f"\33[96m{result.start:>6} initial \33[0m|"
                 f"\33[92m{result.added:>6} added \33[0m|"
                 f"\33[91m{result.removed:>6} removed \33[0m|"
                 f"\33[93m{result.unchanged:>6} unchanged \33[0m|"
```

### Comparing `musify-0.8.1/musify/shared/remote/object.py` & `musify-0.9.0/musify/libraries/remote/core/object.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,83 @@
 """
 Functionality relating to generic remote objects.
 
-Implements core :py:class:`Item` and :py:class:`ItemCollection` classes for remote object types.
+Implements core :py:class:`MusifyItem` and :py:class:`MusifyCollection` classes for remote object types.
 """
-
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from collections.abc import Iterable, Mapping
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Self, Literal, Any
 
-from musify.shared.api.exception import APIError
-from musify.shared.core.base import Item
-from musify.shared.core.collection import ItemCollection
-from musify.shared.core.misc import Result
-from musify.shared.core.object import Track, Album, Playlist, Artist
-from musify.shared.exception import MusifyKeyError
-from musify.shared.remote.api import RemoteAPI
-from musify.shared.remote.base import RemoteObject, RemoteItem
-from musify.shared.remote.enum import RemoteIDType
-from musify.shared.remote.exception import RemoteIDTypeError, RemoteError
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
-from musify.shared.utils import get_most_common_values
-
-
-class RemoteItemWranglerMixin[T: RemoteObject](RemoteItem, RemoteDataWrangler, metaclass=ABCMeta):
-    """Mixin for :py:class:`RemoteItem` and :py:class:`RemoteDataWrangler`"""
-    pass
+from musify.api.exception import APIError
+from musify.core.base import MusifyItem
+from musify.core.result import Result
+from musify.libraries.core.collection import MusifyCollection
+from musify.libraries.core.object import Track, Album, Playlist, Artist
+from musify.libraries.remote.core.api import RemoteAPI
+from musify.libraries.remote.core.base import RemoteObject, RemoteItem
+from musify.libraries.remote.core.exception import RemoteError
+from musify.utils import get_most_common_values
 
 
-class RemoteTrack(RemoteItemWranglerMixin, Track, metaclass=ABCMeta):
+class RemoteTrack(Track, RemoteItem, metaclass=ABCMeta):
     """Extracts key ``track`` data from a remote API JSON response."""
 
     __attributes_classes__ = (Track, RemoteItem)
 
 
-class RemoteCollection[T: RemoteObject](ItemCollection[T], RemoteDataWrangler, metaclass=ABCMeta):
+class RemoteCollection[T: RemoteObject](MusifyCollection[T], metaclass=ABCMeta):
     """Generic class for storing a collection of remote objects."""
 
-    __attributes_classes__ = ItemCollection
-    __attributes_ignore__ = ("items", "track_total", "_total")
-
-    def __getitem__(self, __key: str | int | slice | Item | RemoteObject) -> T | list[T] | list[T, None, None]:
-        """
-        Returns the item in this collection by matching on a given index/Item/URI/ID/URL.
-        If an :py:class:`Item` is given, the URI is extracted from this item
-        and the matching Item from this collection is returned.
-        If a :py:class:`RemoteObject` is given, the ID is extracted from this object
-        and the matching RemoteObject from this collection is returned.
-        """
-        if isinstance(__key, int) or isinstance(__key, slice):  # simply index the list or items
-            return self.items[__key]
-        elif isinstance(__key, Item):  # take the URI
-            if not __key.has_uri:
-                raise MusifyKeyError(f"Given item does not have a URI associated: {__key.name}")
-            __key = __key.uri
-            key_type = RemoteIDType.URI
-        elif isinstance(__key, RemoteObject):
-            __key = __key.id
-            key_type = RemoteIDType.ID
-        else:  # determine the ID type
-            try:
-                return next(item for item in self.items if item.name == __key)
-            except StopIteration:
-                try:
-                    key_type = self.get_id_type(__key)
-                except RemoteIDTypeError:
-                    raise MusifyKeyError(f"ID Type not recognised: '{__key}'")
-
-        try:  # get the item based on the ID type
-            if key_type == RemoteIDType.URI:
-                return next(item for item in self.items if item.uri == __key)
-            elif key_type == RemoteIDType.ID:
-                return next(item for item in self.items if item.uri.split(":")[2] == __key)
-            elif key_type == RemoteIDType.URL:
-                __key = self.convert(__key, type_in=RemoteIDType.URL, type_out=RemoteIDType.URI)
-                return next(item for item in self.items if item.uri == __key)
-            elif key_type == RemoteIDType.URL_EXT:
-                __key = self.convert(__key, type_in=RemoteIDType.URL_EXT, type_out=RemoteIDType.URI)
-                return next(item for item in self.items if item.uri == __key)
-            else:
-                raise MusifyKeyError(f"ID Type not recognised: '{__key}'")
-        except StopIteration:
-            raise MusifyKeyError(f"No matching {key_type.name} found: '{__key}'")
+    __attributes_classes__ = MusifyCollection
+    __attributes_ignore__ = ("items", "track_total")
 
 
 class RemoteCollectionLoader[T: RemoteObject](RemoteObject, RemoteCollection[T], metaclass=ABCMeta):
     """Generic class for storing a collection of remote objects that can be loaded from an API response."""
 
     __attributes_classes__ = (RemoteObject, RemoteCollection)
+    __attributes_ignore__ = "_total"
 
-    def __eq__(self, __collection: RemoteObject | ItemCollection | Iterable[T]):
+    def __eq__(self, __collection: RemoteObject | MusifyCollection | Iterable[T]):
         if isinstance(__collection, RemoteObject):
             return self.uri == __collection.uri
         return super().__eq__(__collection)
 
     @property
     @abstractmethod
     def _total(self) -> int:
         """The total expected items for this collection"""
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def load(
             cls,
-            value: str | Mapping[str, Any],
+            value: str | Mapping[str, Any] | Self,
             api: RemoteAPI,
             use_cache: bool = True,
             items: Iterable[T] = (),
             *args,
             **kwargs
     ) -> Self:
         """
         Generate a new object, calling all required endpoints to get a complete set of data for this item type.
 
         ``value`` may be:
             * A string representing a URL/URI/ID.
             * A remote API JSON response for a collection with a valid ID value under an ``id`` key.
+            * An object of the same type as this collection.
+              The remote API JSON response will be used to load a new object.
+
+        You may also provide a set of kwargs relating that will extend aspects of the response
+        before using it to initialise a new object. See :py:meth:`reload` for possible extensions.
 
         :param value: The value representing some remote collection. See description for allowed value types.
         :param api: An authorised API object to load the object from.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         :param items: Optionally, give a list of available items to build a response for this collection.
             In doing so, the method will first try to find the API responses for the items of this collection
             in the given list before calling the API for any items not found there.
@@ -228,15 +182,15 @@
         self._check_for_api()
 
         self.api.delete_playlist(self.url)
         self.response.clear()
 
     def sync(
             self,
-            items: Iterable[Item] = (),
+            items: Iterable[MusifyItem] = (),
             kind: PLAYLIST_SYNC_KINDS = "new",
             reload: bool = True,
             dry_run: bool = True,
     ) -> SyncResultRemotePlaylist:
         """
         Synchronise this playlist object's items with the remote playlist it is associated with.
 
@@ -276,15 +230,15 @@
             removed = self.api.clear_from_playlist(self.url, items=uri_clear) if not dry_run else len(uri_clear)
             uri_unchanged = [uri for uri in uri_remote if uri in uri_initial]
 
         added = len(uri_add)
         if not dry_run:
             added = self.api.add_to_playlist(self.url, items=uri_add, skip_dupes=kind != "refresh")
             if reload:  # reload the current playlist object from remote
-                self.reload(use_cache=False)
+                self.reload(use_cache=False, extend_tracks=True)
 
         return SyncResultRemotePlaylist(
             start=len(uri_remote),
             added=added,
             removed=removed,
             unchanged=len(uri_unchanged),
             difference=len(self.tracks) - len(uri_remote) if not dry_run and reload else added - removed,
@@ -295,17 +249,14 @@
     def _get_track_uris_from_api_response(self) -> list[str]:
         """
         Returns a list of URIs from the API response stored for this playlist
         Implementation of this method is needed for the :py:func:`sync` function.
         """
         raise NotImplementedError
 
-    def merge(self, playlist: Playlist[T]) -> None:
-        raise NotImplementedError
-
 
 class RemoteAlbum[T: RemoteTrack](Album[T], RemoteCollectionLoader[T], metaclass=ABCMeta):
     """Extracts key ``album`` data from a remote API JSON response."""
 
     __attributes_classes__ = (Album, RemoteCollectionLoader)
 
     @property
@@ -314,15 +265,15 @@
 
     @property
     @abstractmethod
     def artists(self) -> list[RemoteArtist[T]]:
         raise NotImplementedError
 
 
-class RemoteArtist[T: RemoteTrack](Artist[T], RemoteCollectionLoader[T], metaclass=ABCMeta):
+class RemoteArtist[T: (RemoteTrack, RemoteAlbum)](Artist[T], RemoteCollectionLoader[T], metaclass=ABCMeta):
     """Extracts key ``artist`` data from a remote API JSON response."""
 
     __attributes_classes__ = (Artist, RemoteCollectionLoader)
 
     @property
     def _total(self):
         return 0
```

### Comparing `musify-0.8.1/musify/shared/remote/processors/check.py` & `musify-0.9.0/musify/libraries/remote/core/processors/check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,130 +1,144 @@
 """
 Processor operations that help a user to check whether the currently matched ID is valid for given items.
 
 Provides the user the ability to modify associated IDs using a Remote player as an interface for
 reviewing matches through temporary playlist creation.
 """
-
-import traceback
-from abc import ABCMeta, abstractmethod
+import logging
 from collections import Counter
-from collections.abc import Sequence, Collection
+from collections.abc import Sequence, Collection, Iterator
+from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass, field
+from typing import Any
 
 from musify import PROGRAM_NAME
+from musify.core.base import MusifyItemSettable
+from musify.core.enum import Fields
+from musify.core.result import Result
+from musify.libraries.core.collection import MusifyCollection
+from musify.libraries.remote.core.api import RemoteAPI
+from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
+from musify.libraries.remote.core.factory import RemoteObjectFactory
+from musify.libraries.remote.core.processors.search import RemoteItemSearcher
+from musify.log import REPORT
+from musify.log.logger import MusifyLogger
 from musify.processors.base import InputProcessor
 from musify.processors.match import ItemMatcher
-from musify.shared.core.base import Item
-from musify.shared.core.collection import ItemCollection
-from musify.shared.core.enum import Fields
-from musify.shared.core.misc import Result
-from musify.shared.core.object import Track
-from musify.shared.logger import REPORT
-from musify.shared.remote.api import RemoteAPI
-from musify.shared.remote.config import RemoteObjectClasses
-from musify.shared.remote.enum import RemoteObjectType, RemoteIDType
-from musify.shared.remote.processors.search import RemoteItemSearcher
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
-from musify.shared.utils import get_max_width, align_string
+from musify.utils import get_max_width, align_string
 
-ALLOW_KARAOKE_DEFAULT = RemoteItemSearcher.settings_items.allow_karaoke
+ALLOW_KARAOKE_DEFAULT = RemoteItemSearcher.search_settings[RemoteObjectType.TRACK].allow_karaoke
 
 
 @dataclass(frozen=True)
-class ItemCheckResult(Result):
+class ItemCheckResult[T: MusifyItemSettable](Result):
     """Stores the results of the checking process."""
     #: Sequence of Items that had URIs switched during the check.
-    switched: Sequence[Item] = field(default=tuple())
+    switched: Sequence[T] = field(default=tuple())
     #: Sequence of Items that were marked as unavailable.
-    unavailable: Sequence[Item] = field(default=tuple())
+    unavailable: Sequence[T] = field(default=tuple())
     #: Sequence of Items that were skipped from the check.
-    skipped: Sequence[Item] = field(default=tuple())
+    skipped: Sequence[T] = field(default=tuple())
 
 
-class RemoteItemChecker(RemoteDataWrangler, ItemMatcher, InputProcessor, metaclass=ABCMeta):
+class RemoteItemChecker(InputProcessor):
     """
     Runs operations for checking the URIs associated with a collection of items.
 
     When running :py:func:`check`, the object will do the following:
         * Make temporary playlists for each collection up to a ``interval`` limit of playlists.
           At which point, playlist creation pauses.
         * User can then check and modify the temporary playlists to match items to correct items or otherwise.
         * When operations resume at the user's behest, the program will search each playlist to find changes
           and attempt to match any new items to a source item.
         * If no matches are found for certain items, the program will prompt the user
           to determine how they wish to deal with these items.
         * Operation completes once user exists or all items have an associated URI.
 
-    :param api: An API object with authorised access to a remote User to create playlists for.
+    :param matcher: The :py:class:`ItemMatcher` to use when comparing any changes made by the user in remote playlists
+        during the checking operation
+    :param object_factory: The :py:class:`RemoteObjectFactory` to use when creating new remote objects.
+        This must have a :py:class:`RemoteAPI` assigned for this processor to work as expected.
     :param interval: Stop creating playlists after this many playlists have been created and pause for user input.
     :param allow_karaoke: When True, items determined to be karaoke are allowed when matching switched items.
         Skip karaoke results otherwise. Karaoke items are identified using the ``karaoke_tags`` attribute.
     """
 
     __slots__ = (
         "interval",
         "allow_karaoke",
-        "api",
+        "factory",
         "_playlist_name_urls",
         "_playlist_name_collection",
         "_skip",
         "_quit",
         "_remaining",
         "_switched",
         "_final_switched",
         "_final_unavailable",
         "_final_skipped",
     )
 
     @property
-    @abstractmethod
-    def _object_cls(self) -> RemoteObjectClasses:
-        """Stores the key object classes for a remote source."""
-        raise NotImplementedError
-
-    def __init__(self, api: RemoteAPI, interval: int = 10, allow_karaoke: bool = ALLOW_KARAOKE_DEFAULT):
+    def api(self) -> RemoteAPI:
+        """The :py:class:`RemoteAPI` to call"""
+        return self.factory.api
+
+    def __init__(
+            self,
+            matcher: ItemMatcher,
+            object_factory: RemoteObjectFactory,
+            interval: int = 10,
+            allow_karaoke: bool = ALLOW_KARAOKE_DEFAULT
+    ):
         super().__init__()
 
+        # noinspection PyTypeChecker
+        #: The :py:class:`MusifyLogger` for this  object
+        self.logger: MusifyLogger = logging.getLogger(__name__)
+
+        #: The :py:class:`ItemMatcher` to use when comparing any changes made by the user in remote playlists
+        #: during the checking operation
+        self.matcher = matcher
+        #: The :py:class:`RemoteObjectFactory` to use when creating new remote objects.
+        self.factory = object_factory
         #: Stop creating playlists after this many playlists have been created and pause for user input
         self.interval = interval
         #: Allow karaoke items when matching on switched items
         self.allow_karaoke = allow_karaoke
 
-        #: The :py:class:`RemoteAPI` to call
-        self.api = api
         #: Map of playlist names to their URLs for created temporary playlists
         self._playlist_name_urls = {}
         #: Map of playlist names to the collection of items added for created temporary playlists
         self._playlist_name_collection = {}
 
         #: When true, skip the current loop and eventually safely quit check
         self._skip = False
         #: When true, safely quit check
         self._quit = False
 
         #: The currently remaining items that the user needs to manually check
-        self._remaining: list[Track] = []
+        self._remaining: list[MusifyItemSettable] = []
         #: The list of items with switched URIs currently processed by the checker
-        self._switched: list[Track] = []
+        self._switched: list[MusifyItemSettable] = []
 
         #: The final list of items with switched URIs as processed by the checker
-        self._final_switched: list[Track] = []
+        self._final_switched: list[MusifyItemSettable] = []
         #: The final list of items marked as unavailable for this remote source
-        self._final_unavailable: list[Track] = []
+        self._final_unavailable: list[MusifyItemSettable] = []
         #: The final list of items skipped by the checker
-        self._final_skipped: list[Track] = []
+        self._final_skipped: list[MusifyItemSettable] = []
 
     def _check_api(self):
         """Check if the API token has expired and refresh as necessary"""
         if not self.api.handler.test_token():  # check if token has expired
             self.logger.info_extra("\33[93mAPI token has expired, re-authorising... \33[0m")
             self.api.authorise()
 
-    def _create_playlist(self, collection: ItemCollection) -> None:
+    def _create_playlist(self, collection: MusifyCollection[MusifyItemSettable]) -> None:
         """Create a temporary playlist, store its URL for later unfollowing, and add all given URIs."""
         self._check_api()
 
         uris = [item.uri for item in collection if item.has_uri]
         if not uris:
             return
 
@@ -141,65 +155,60 @@
         self.logger.info_extra(f"\33[93mDeleting {len(self._playlist_name_urls)} temporary playlists... \33[0m")
         for url in self._playlist_name_urls.values():  # delete playlists
             self.api.delete_playlist(url)
 
         self._playlist_name_urls.clear()
         self._playlist_name_collection.clear()
 
-    # noinspection PyMethodOverriding
-    def __call__(self, collections: Collection[ItemCollection]) -> ItemCheckResult | None:
-        return self.check(collections=collections)
+    def __call__(self, *args, **kwargs) -> ItemCheckResult | None:
+        return self.check(*args, **kwargs)
 
-    def check(self, collections: Collection[ItemCollection]) -> ItemCheckResult | None:
+    def check[T: MusifyItemSettable](self, collections: Collection[MusifyCollection[T]]) -> ItemCheckResult[T] | None:
         """
         Run the checker for the given ``collections``.
 
         :param collections: A list of collections to check.
         :return: A :py:class:`ItemCheckResult` object containing the remapped items created during the check.
             Return None when the user opted to quit (not skip) the checker before completion.
         """
         if len(collections) == 0 or all(not collection.items for collection in collections):
             self.logger.debug("\33[93mNo items to check. \33[0m")
             return
 
         self.logger.debug("Checking items: START")
         self.logger.info(
-            f"\33[1;95m ->\33[1;97m Checking items by creating temporary {self.source} playlists "
+            f"\33[1;95m ->\33[1;97m Checking items by creating temporary {self.api.source} playlists "
             f"for the current user: {self.api.user_name} \33[0m"
         )
 
         total = len(collections)
         pages_total = (total // self.interval) + (total % self.interval > 0)
         bar = self.logger.get_progress_bar(total=total, desc="Creating temp playlists", unit="playlists")
 
         self._skip = False
         self._quit = False
 
         collections_iter = (collection for collection in collections)
         for page in range(1, pages_total + 1):
-            # noinspection PyBroadException
             try:
                 for count, collection in enumerate(collections_iter, 1):
                     self._create_playlist(collection=collection)
                     bar.update(1)
                     if count >= self.interval:
                         break
 
                 self._pause(page=page, total=pages_total)
                 if not self._quit:  # still run if skip is True
                     self._check_uri()
             except KeyboardInterrupt:
                 self.logger.error("User triggered exit with KeyboardInterrupt")
                 self._quit = True
-            except BaseException as ex:  # delete playlists first before raising error
-                self.logger.error(traceback.format_exc())
+            finally:
                 self._delete_playlists()
-                raise ex
 
-            self._delete_playlists()
             if self._quit or self._skip:  # quit check
                 break
 
         bar.close()
         result = self._finalise() if not self._quit else None
         self.logger.debug("Checking items: DONE\n")
         return result
@@ -235,21 +244,21 @@
         """
         Initial pause after the ``interval`` limit of playlists have been created.
 
         :param page: The current page number i.e. the current number of pauses that have happened so far.
         :param total: The total number of pages (pauses) that will occur in this run.
         """
         header = [
-            f"\t\33[1;94mTemporary playlists created on {self.source}.",
-            f"You may now check the songs in each playlist on {self.source}. \33[0m"
+            f"\t\33[1;94mTemporary playlists created on {self.api.source}.",
+            f"You may now check the songs in each playlist on {self.api.source}. \33[0m"
         ]
         options = {
             "<Name of playlist>":
                 "Print position, item name, URI, and URL from given link of items as originally added to temp playlist",
-            f"<{self.source} URL/URI>":
+            f"<{self.api.source} URL/URI>":
                 "Print position, item name, URI, and URL from given link (useful to check current status of playlist)",
             "<Return/Enter>":
                 "Once you have checked all playlist's items, continue on and check for any switches by the user",
             "s": "Check for changes on current playlists, but skip any remaining checks",
             "q": "Delete current temporary playlists and quit check",
             "h": "Show this dialogue again",
         }
@@ -281,43 +290,43 @@
                 for i, item in enumerate(items, 1):
                     length = getattr(item, "length", 0)
                     self.api.print_item(
                         i=i, name=item.name, uri=item.uri, length=length, total=len(items), max_width=max_width
                     )
                 print()
 
-            elif self.validate_id_type(current_input):  # print URL/URI/ID result
+            elif self.api.wrangler.validate_id_type(current_input):  # print URL/URI/ID result
                 self._check_api()
                 self.api.print_collection(current_input)
 
             elif current_input != "":
                 self.logger.warning("Input not recognised.")
 
     ###########################################################################
     ## Match items user has added or removed
     ###########################################################################
     def _check_uri(self) -> None:
         """Run operations to check that URIs are assigned to all the items in the current list of collections."""
         skip_hold = self._skip
         self._skip = False
         for name, collection in self._playlist_name_collection.items():
-            self._log_padded([name, f"{len(collection):>6} total items"], pad='>')
+            self.matcher.log_messages([name, f"{len(collection):>6} total items"], pad='>')
 
             while True:
                 self._match_to_remote(name=name)
                 self._match_to_input(name=name)
                 if not self._remaining:
                     break
 
             unavailable = tuple(item for item in collection if item.has_uri is False)
             skipped = tuple(item for item in collection if item.has_uri is None)
 
-            self._log_padded([name, f"{len(self._switched):>6} items switched"], pad='<')
-            self._log_padded([name, f"{len(unavailable):>6} items unavailable"])
-            self._log_padded([name, f"{len(skipped):>6} items skipped"])
+            self.matcher.log_messages([name, f"{len(self._switched):>6} items switched"], pad='<')
+            self.matcher.log_messages([name, f"{len(unavailable):>6} items unavailable"])
+            self.matcher.log_messages([name, f"{len(skipped):>6} items skipped"])
 
             self._final_switched += self._switched
             self._final_unavailable += unavailable
             self._final_skipped += skipped
             self._switched.clear()
 
             if self._quit or self._skip:
@@ -330,136 +339,155 @@
         Check the current temporary playlist given by ``name`` and attempt to match the source list of items
         to any modifications the user has made.
         """
         self._check_api()
 
         self.logger.info(
             "\33[1;95m ->\33[1;97m Checking for changes to items in "
-            f"{self.source} playlist: \33[94m{name}\33[0m..."
+            f"{self.api.source} playlist: \33[94m{name}\33[0m..."
         )
 
         source = self._playlist_name_collection[name]
         source_valid = [item for item in source if item.has_uri]
 
         remote_response = self.api.get_items(self._playlist_name_urls[name], extend=True, use_cache=False)[0]
-        remote = self._object_cls.playlist(response=remote_response, api=self.api).tracks
+        remote = self.factory.playlist(response=remote_response).items
         remote_valid = [item for item in remote if item.has_uri]
 
         added = [item for item in remote_valid if item not in source]
         removed = [item for item in source_valid if item not in remote] if not self._remaining else []
         missing = self._remaining or [item for item in source if item.has_uri is None]
 
         if len(added) + len(removed) + len(missing) == 0:
             if len(source_valid) == len(remote_valid):
-                self._log_padded([name, "Playlist unchanged and no missing URIs, skipping match"])
+                self.matcher.log_messages([name, "Playlist unchanged and no missing URIs, skipping match"])
                 return
 
             # if item collection originally contained duplicate URIS and one or more of the duplicates were removed,
             # find missing items by looking for changes in counts
             remote_counts = Counter(item.uri for item in remote_valid)
             for uri, count in Counter(item.uri for item in source_valid).items():
                 if remote_counts.get(uri) != count:
                     missing.extend([item for item in source_valid if item.uri == uri])
 
-        self._log_padded([name, f"{len(added):>6} items added"])
-        self._log_padded([name, f"{len(removed):>6} items removed"])
-        self._log_padded([name, f"{len(missing):>6} items in source missing URI"])
-        self._log_padded([name, f"{len(source_valid) - len(remote_valid):>6} total difference"])
+        self.matcher.log_messages([name, f"{len(added):>6} items added"])
+        self.matcher.log_messages([name, f"{len(removed):>6} items removed"])
+        self.matcher.log_messages([name, f"{len(missing):>6} items in source missing URI"])
+        self.matcher.log_messages([name, f"{len(source_valid) - len(remote_valid):>6} total difference"])
 
         remaining = removed + missing
         count_start = len(remaining)
-        for item in remaining:
-            if not added:
-                break
+        with ThreadPoolExecutor(thread_name_prefix="checker") as executor:
+            tasks: Iterator[tuple[MusifyItemSettable, MusifyItemSettable | None]] = executor.map(
+                lambda item: (
+                    item, self.matcher(item, results=added, match_on=[Fields.TITLE], allow_karaoke=self.allow_karaoke)
+                ),
+                remaining if added else ()
+            )
 
-            result = self.match(item, results=added, match_on=[Fields.TITLE], allow_karaoke=self.allow_karaoke)
-            if not result:
+        for item, match in tasks:
+            if not match:
                 continue
 
-            item.uri = result.uri
+            item.uri = match.uri
 
-            added.remove(result)
+            added.remove(match)
             removed.remove(item) if item in removed else missing.remove(item)
-            self._switched.append(result)
+            self._switched.append(match)
 
         self._remaining = removed + missing
         count_final = len(self._remaining)
-        self._log_padded([name, f"{count_start - count_final:>6} items switched"])
-        self._log_padded([name, f"{count_final:>6} items still not found"])
+        self.matcher.log_messages([name, f"{count_start - count_final:>6} items switched"])
+        self.matcher.log_messages([name, f"{count_final:>6} items still not found"])
 
     def _match_to_input(self, name: str) -> None:
         """
         Get the user's input for any items in the ``remaining`` list that are still missing URIs.
         Provide a ``name`` to use for logging only.
         """
         if not self._remaining:
             return
 
         header = [f"\t\33[1;94m{name}:\33[91m The following items were removed and/or matches were not found. \33[0m"]
         options = {
-            "u": f"Mark item as 'Unavailable on {self.source}'",
+            "u": f"Mark item as 'Unavailable on {self.api.source}'",
             "n": f"Leave item with no URI. ({PROGRAM_NAME} will still attempt to find this item at the next run)",
             "a": "Add in addition to 'u' or 'n' options to apply this setting to all items in this playlist",
-            "r": "Recheck playlist for all items in the album",
+            "r": "Recheck playlist for all items in the collection",
             "p": "Print the local path of the current item if available",
             "s": "Skip checking process for all current playlists",
             "q": "Skip checking process for all current playlists and quit check",
             "h": "Show this dialogue again",
         }
 
         current_input = ""
         help_text = self._format_help_text(options=options, header=header)
         help_text += "OR enter a custom URI/URL/ID for this item\n"
 
-        self._log_padded([name, f"Getting user input for {len(self._remaining)} items"])
+        self.matcher.log_messages([name, f"Getting user input for {len(self._remaining)} items"])
         max_width = get_max_width({item.name for item in self._remaining})
 
         print("\n" + help_text)
         for item in self._remaining.copy():
-            while item in self._remaining:  # while item not matched or skipped
-                self._log_padded([name, f"{len(self._remaining):>6} remaining items"])
+            while current_input is not None and item in self._remaining:  # while item not matched or skipped
+                self.matcher.log_messages([name, f"{len(self._remaining):>6} remaining items"])
                 if 'a' not in current_input:
                     current_input = self._get_user_input(align_string(item.name, max_width=max_width))
 
                 if current_input.casefold() == 'h':  # print help
                     print("\n" + help_text)
+                else:
+                    current_input = self._match_item_to_input(name=name, item=item, current_input=current_input)
 
-                elif current_input.casefold() == 's' or current_input.casefold() == 'q':  # quit/skip
-                    self._log_padded([name, "Skipping all loops"], pad="<")
-                    self._quit = current_input.casefold() == 'q' or self._quit
-                    self._skip = current_input.casefold() == 's' or self._skip
-                    self._remaining.clear()
-                    return
-
-                elif current_input.casefold().replace('a', '') == 'u':  # mark item as unavailable
-                    self._log_padded([name, "Marking as unavailable"], pad="<")
-                    item.uri = self.unavailable_uri_dummy
-                    self._remaining.remove(item)
-
-                elif current_input.casefold().replace('a', '') == 'n':  # leave item without URI and unprocessed
-                    self._log_padded([name, "Skipping"], pad="<")
-                    item.uri = None
-                    self._remaining.remove(item)
-
-                elif current_input.casefold() == 'r':  # return to former 'while' loop
-                    self._log_padded([name, "Refreshing playlist metadata and restarting loop"])
-                    return
-
-                elif current_input.casefold() == 'p' and hasattr(item, "path"):  # print item path
-                    print(f"\33[96m{item.path}\33[0m")
-
-                elif self.validate_id_type(current_input):  # update URI and add item to switched list
-                    uri = self.convert(current_input, kind=RemoteObjectType.TRACK, type_out=RemoteIDType.URI)
-
-                    self._log_padded([name, f"Updating URI: {item.uri} -> {uri}"], pad="<")
-                    item.uri = uri
-
-                    self._switched.append(item)
-                    self._remaining.remove(item)
-                    current_input = ""
-
-                elif current_input:  # invalid input
-                    self.logger.warning("Input not recognised.")
-                    current_input = ""
-
-            if not self._remaining:
+            if current_input is None or not self._remaining:
                 break
+
+    def _match_item_to_input(self, name: str, item: MusifyItemSettable, current_input: str) -> str | None:
+        if current_input.casefold() == 's' or current_input.casefold() == 'q':  # quit/skip
+            self.matcher.log_messages([name, "Skipping all loops"], pad="<")
+            self._quit = current_input.casefold() == 'q' or self._quit
+            self._skip = current_input.casefold() == 's' or self._skip
+            self._remaining.clear()
+            return
+
+        elif current_input.casefold().replace('a', '') == 'u':  # mark item as unavailable
+            self.matcher.log_messages([name, "Marking as unavailable"], pad="<")
+            item.uri = self.api.wrangler.unavailable_uri_dummy
+            self._remaining.remove(item)
+
+        elif current_input.casefold().replace('a', '') == 'n':  # leave item without URI and unprocessed
+            self.matcher.log_messages([name, "Skipping"], pad="<")
+            item.uri = None
+            self._remaining.remove(item)
+
+        elif current_input.casefold() == 'r':  # return to former 'while' loop
+            self.matcher.log_messages([name, "Refreshing playlist metadata and restarting loop"])
+            return
+
+        elif current_input.casefold() == 'p' and hasattr(item, "path"):  # print item path
+            print(f"\33[96m{item.path}\33[0m")
+
+        elif self.api.wrangler.validate_id_type(current_input):  # update URI and add item to switched list
+            uri = self.api.wrangler.convert(
+                current_input, kind=RemoteObjectType.TRACK, type_out=RemoteIDType.URI
+            )
+
+            self.matcher.log_messages([name, f"Updating URI: {item.uri} -> {uri}"], pad="<")
+            item.uri = uri
+
+            self._switched.append(item)
+            self._remaining.remove(item)
+            current_input = ""
+
+        elif current_input:  # invalid input
+            self.logger.warning("Input not recognised.")
+            current_input = ""
+
+        return current_input
+
+    def as_dict(self) -> dict[str, Any]:
+        return {
+            "matcher": self.matcher,
+            "remote_source": self.factory.api.source,
+            "interval": self.interval,
+            "allow_karaoke": self.allow_karaoke,
+        }
```

### Comparing `musify-0.8.1/musify/shared/remote/processors/search.py` & `musify-0.9.0/musify/libraries/remote/core/processors/search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,150 @@
 """
 Processor operations that search for and match given items with remote items.
 
 Searches for matches on remote APIs, matches the item to the best matching result from the query,
 and assigns the ID of the matched object back to the item.
 """
-
-from abc import ABCMeta, abstractmethod
+import logging
 from collections.abc import Mapping, Sequence, Iterable, Collection
+from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass, field
 from typing import Any
 
+from musify.core.base import MusifyObject, MusifyItemSettable
+from musify.core.enum import TagField, TagFields as Tag
+from musify.core.result import Result
+from musify.exception import MusifyAttributeError
+from musify.libraries.core.collection import MusifyCollection
+from musify.libraries.remote.core.api import RemoteAPI
+from musify.libraries.remote.core.enum import RemoteObjectType
+from musify.libraries.remote.core.factory import RemoteObjectFactory
+from musify.log import REPORT
+from musify.log.logger import MusifyLogger
+from musify.processors.base import Processor
 from musify.processors.match import ItemMatcher
-from musify.shared.core.base import NameableTaggableMixin, Item
-from musify.shared.core.collection import ItemCollection
-from musify.shared.core.enum import TagField, TagFields as Tag
-from musify.shared.core.misc import Result
-from musify.shared.core.object import Track
-from musify.shared.logger import REPORT
-from musify.shared.remote import Remote
-from musify.shared.remote.api import RemoteAPI
-from musify.shared.remote.config import RemoteObjectClasses
-from musify.shared.remote.enum import RemoteObjectType
-from musify.shared.utils import align_string, get_max_width
+from musify.types import UnitIterable
+from musify.utils import align_string, get_max_width
 
 
 @dataclass(frozen=True)
-class ItemSearchResult(Result):
+class ItemSearchResult[T: MusifyItemSettable](Result):
     """Stores the results of the searching process."""
     #: Sequence of Items for which matches were found from the search.
-    matched: Sequence[Item] = field(default=tuple())
+    matched: Sequence[T] = field(default=tuple())
     #: Sequence of Items for which matches were not found from the search.
-    unmatched: Sequence[Item] = field(default=tuple())
+    unmatched: Sequence[T] = field(default=tuple())
     #: Sequence of Items which were skipped during the search.
-    skipped: Sequence[Item] = field(default=tuple())
+    skipped: Sequence[T] = field(default=tuple())
 
 
 @dataclass(frozen=True)
-class SearchSettings:
+class SearchConfig:
     """Key settings related to a search algorithm."""
-    #: A sequence of the tag names to use as search fields in the 1st pass.
-    search_fields_1: Sequence[TagField]
     #: The fields to match results on.
     match_fields: TagField | Iterable[TagField]
-    #: The number of the results to request when querying the API.
-    result_count: int
-    #: When True, items determined to be karaoke are allowed when matching added items.
-    #: Skip karaoke results otherwise.
-    allow_karaoke: bool = False
-
-    #: The minimum acceptable score for an item to be considered a match.
-    min_score: float = 0.1
-    #: The maximum score for an item to be considered a perfect match.
-    #: After this score is reached by an item, any other items are disregarded as potential matches.
-    max_score: float = 0.8
-
+    #: A sequence of the tag names to use as search fields in the 1st pass.
+    search_fields_1: Sequence[TagField] = (Tag.NAME,)
     #: If no results are found from the tag names in ``search_fields_1`` on the 1st pass,
     #: an optional sequence of the tag names to use as search fields in the 2nd pass.
     search_fields_2: Iterable[TagField] = ()
     #: If no results are found from the tag names in ``search_fields_2`` on the 2nd pass,
     #: an optional sequence of the tag names to use as search fields in the 3rd pass.
     search_fields_3: Iterable[TagField] = ()
 
+    #: The number of the results to request when querying the API.
+    result_count: int = 10
+    #: The minimum acceptable score for an item to be considered a match.
+    min_score: float = 0.1
+    #: The maximum score for an item to be considered a perfect match.
+    #: After this score is reached by an item, any other items are disregarded as potential matches.
+    max_score: float = 0.8
+    #: When True, items determined to be karaoke are allowed when matching added items.
+    #: Skip karaoke results otherwise.
+    allow_karaoke: bool = False
 
-class RemoteItemSearcher(Remote, ItemMatcher, metaclass=ABCMeta):
+
+class RemoteItemSearcher(Processor):
     """
     Searches for remote matches for a list of item collections.
 
-    :param api: An API object for calling the remote query endpoint.
+    :param matcher: The :py:class:`ItemMatcher` to use when comparing any changes made by the user in remote playlists
+        during the checking operation
+    :param object_factory: The :py:class:`RemoteObjectFactory` to use when creating new remote objects.
+        This must have a :py:class:`RemoteAPI` assigned for this processor to work as expected.
     :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
     """
 
-    __slots__ = ("api", "use_cache")
+    __slots__ = ("factory", "use_cache")
 
-    #: The :py:class:`SearchSettings` to use when running item searches
-    settings_items = SearchSettings(
-        search_fields_1=[Tag.NAME, Tag.ARTIST],
-        search_fields_2=[Tag.NAME, Tag.ALBUM],
-        search_fields_3=[Tag.NAME],
-        match_fields={Tag.TITLE, Tag.ARTIST, Tag.ALBUM, Tag.LENGTH},
-        result_count=10,
-        allow_karaoke=False,
-        min_score=0.1,
-        max_score=0.8
-    )
-    #: The :py:class:`SearchSettings` to use when running album searches
-    settings_albums = SearchSettings(
-        search_fields_1=[Tag.NAME, Tag.ARTIST],
-        search_fields_2=[Tag.NAME],
-        match_fields={Tag.ARTIST, Tag.ALBUM, Tag.LENGTH},
-        result_count=5,
-        allow_karaoke=False,
-        min_score=0.1,
-        max_score=0.7
-    )
+    #: The :py:class:`SearchSettings` for each :py:class:`RemoteObjectType`
+    search_settings: dict[RemoteObjectType, SearchConfig] = {
+        RemoteObjectType.TRACK: SearchConfig(
+            match_fields={Tag.TITLE, Tag.ARTIST, Tag.ALBUM, Tag.LENGTH},
+            search_fields_1=[Tag.NAME, Tag.ARTIST],
+            search_fields_2=[Tag.NAME, Tag.ALBUM],
+            search_fields_3=[Tag.NAME],
+            result_count=10,
+            min_score=0.1,
+            max_score=0.8,
+            allow_karaoke=False,
+        ),
+        RemoteObjectType.ALBUM: SearchConfig(
+            match_fields={Tag.ARTIST, Tag.ALBUM, Tag.LENGTH},
+            search_fields_1=[Tag.NAME, Tag.ARTIST],
+            search_fields_2=[Tag.NAME],
+            result_count=5,
+            min_score=0.1,
+            max_score=0.7,
+            allow_karaoke=False,
+        )
+    }
 
     @property
-    @abstractmethod
-    def _object_cls(self) -> RemoteObjectClasses:
-        """Stores the key object classes for a remote source."""
-        raise NotImplementedError
+    def api(self) -> RemoteAPI:
+        """The :py:class:`RemoteAPI` to call"""
+        return self.factory.api
 
-    def __init__(self, api: RemoteAPI, use_cache: bool = False):
+    def __init__(self, matcher: ItemMatcher, object_factory: RemoteObjectFactory, use_cache: bool = False):
         super().__init__()
 
-        #: The :py:class:`RemoteAPI` to call
-        self.api = api
+        # noinspection PyTypeChecker
+        #: The :py:class:`MusifyLogger` for this  object
+        self.logger: MusifyLogger = logging.getLogger(__name__)
+
+        #: The :py:class:`ItemMatcher` to use when comparing any changes made by the user in remote playlists
+        #: during the checking operation
+        self.matcher = matcher
+        #: The :py:class:`RemoteObjectFactory` to use when creating new remote objects.
+        self.factory = object_factory
         #: When true, use the cache when calling the API endpoint
         self.use_cache = use_cache
 
     def _get_results(
-            self, item: NameableTaggableMixin, kind: RemoteObjectType, settings: SearchSettings
+            self, item: MusifyObject, kind: RemoteObjectType, settings: SearchConfig
     ) -> list[dict[str, Any]] | None:
         """Query the API to get results for the current item based on algorithm settings"""
-        self.clean_tags(item)
+        self.matcher.clean_tags(item)
 
         def execute_query(keys: Iterable[TagField]) -> tuple[list[dict[str, Any]], str]:
             """Generate and execute the query against the API for the given item's cleaned ``keys``"""
             attributes = [item.clean_tags.get(key) for key in keys]
             q = " ".join(str(attr) for attr in attributes if attr)
             return self.api.query(q, kind=kind, limit=settings.result_count), q
 
         results, query = execute_query(settings.search_fields_1)
         if not results and settings.search_fields_2:
             results, query = execute_query(settings.search_fields_2)
         if not results and settings.search_fields_3:
             results, query = execute_query(settings.search_fields_3)
 
         if results:
-            self._log_padded([item.name, f"Query: {query}", f"{len(results)} results"])
+            self.matcher.log_messages([item.name, f"Query: {query}", f"{len(results)} results"])
             return results
-        self._log_padded([item.name, f"Query: {query}", "Match failed: No results."], pad="<")
+        self.matcher.log_messages([item.name, f"Query: {query}", "Match failed: No results."], pad="<")
 
     def _log_results(self, results: Mapping[str, ItemSearchResult]) -> None:
         """Logs the final results of the ItemSearcher"""
         if not results:
             return
 
         max_width = get_max_width(results)
@@ -171,130 +182,151 @@
             f"\33[92m{total_matched:>6} matched \33[0m| "
             f"\33[91m{total_unmatched:>6} unmatched \33[0m| "
             f"\33[93m{total_skipped:>6} skipped \33[0m| "
             f"\33[97m{total_all:>6} total \33[0m"
         )
         self.logger.print(REPORT)
 
-    # noinspection PyMethodOverriding
-    def __call__(self, collections: Collection[ItemCollection]) -> dict[str, ItemSearchResult]:
-        return self.search(collections=collections)
-
-    def search(self, collections: Collection[ItemCollection]) -> dict[str, ItemSearchResult]:
+    @staticmethod
+    def _determine_remote_object_type(obj: MusifyObject) -> RemoteObjectType:
+        if hasattr(obj, "kind"):
+            return obj.kind
+        raise MusifyAttributeError(f"Given object does not specify a RemoteObjectType: {obj.__class__.__name__}")
+
+    def __call__(self, *args, **kwargs) -> dict[str, ItemSearchResult]:
+        return self.search(*args, **kwargs)
+
+    def search[T: MusifyItemSettable](
+            self, collections: Collection[MusifyCollection[T]]
+    ) -> dict[str, ItemSearchResult[T]]:
         """
         Searches for remote matches for the given list of item collections.
 
         :return: Map of the collection's name to its :py:class:`ItemSearchResult` object.
         """
         self.logger.debug("Searching: START")
         if not [item for c in collections for item in c.items if item.has_uri is None]:
             self.logger.debug("\33[93mNo items to search. \33[0m")
             return {}
 
         kinds = {coll.__class__.__name__ for coll in collections}
         kind = kinds.pop() if len(kinds) == 1 else "collection"
         self.logger.info(
             f"\33[1;95m ->\33[1;97m "
-            f"Searching for matches on {self.source} for {len(collections)} {kind}s\33[0m"
+            f"Searching for matches on {self.api.source} for {len(collections)} {kind}s\33[0m"
         )
 
         bar = self.logger.get_progress_bar(iterable=collections, desc="Searching", unit=f"{kind}s")
-        search_results = {coll.name: self._search_collection(collection=coll) for coll in bar}
+        with ThreadPoolExecutor(thread_name_prefix="searcher-main") as executor:
+            search_results = dict(executor.map(lambda coll: (coll.name, self._search_collection(coll)), bar))
 
         self.logger.print()
         self._log_results(search_results)
         self.logger.debug("Searching: DONE\n")
         return search_results
 
-    def _search_collection(self, collection: ItemCollection) -> ItemSearchResult:
+    def _search_collection[T: MusifyItemSettable](self, collection: MusifyCollection) -> ItemSearchResult[T]:
         kind = collection.__class__.__name__
 
         skipped = tuple(item for item in collection if item.has_uri is not None)
         if len(skipped) == len(collection):
-            self._log_padded([collection.name, "Skipping search, no tracks to search"], pad='<')
+            self.matcher.log_messages([collection.name, "Skipping search, no items to search"], pad='<')
 
         if getattr(collection, "compilation", True) is False:
-            self._log_padded([collection.name, "Searching with album algorithm"], pad='>')
-            self._search_album(collection=collection)
+            self.matcher.log_messages([collection.name, "Searching for collection as a unit"], pad='>')
+            self._search_collection_unit(collection=collection)
 
             missing = [item for item in collection.items if item.has_uri is None]
             if missing:
-                self._log_padded([collection.name, f"Searching for {len(missing)} unmatched items in this {kind}"])
+                self.matcher.log_messages(
+                    [collection.name, f"Searching for {len(missing)} unmatched items in this {kind}"]
+                )
                 self._search_items(collection=collection)
         else:
-            self._log_padded([collection.name, "Searching with item algorithm"], pad='>')
+            self.matcher.log_messages([collection.name, "Searching for distinct items in collection"], pad='>')
             self._search_items(collection=collection)
 
         return ItemSearchResult(
             matched=tuple(item for item in collection if item.has_uri and item not in skipped),
             unmatched=tuple(item for item in collection if item.has_uri is None and item not in skipped),
             skipped=skipped
         )
 
-    def _search_items(self, collection: Iterable[Item]) -> None:
-        """Search for matches on individual items in an item collection that have ``None`` on ``has_uri`` attribute"""
-        for item in filter(lambda i: i.has_uri is None, collection):
-            if not isinstance(item, Track):
-                # TODO: expand search logic to include all item types (low priority)
-                raise NotImplementedError(
-                    f"Currently only able to search for Track items, not {item.__class__.__name__}"
-                )
+    def _get_item_match[T: MusifyItemSettable](
+            self, item: T, match_on: UnitIterable[TagField] | None = None, results: Iterable[T] = None
+    ) -> tuple[T, T | None]:
+        kind = self._determine_remote_object_type(item)
+        search_config = self.search_settings[kind]
+
+        if results is None:
+            responses = self._get_results(item, kind=kind, settings=search_config)
+            # noinspection PyTypeChecker
+            results: Iterable[T] = map(self.factory[kind], responses or ())
+
+        result = self.matcher(
+            item,
+            results=results,
+            match_on=match_on if match_on is not None else search_config.match_fields,
+            min_score=search_config.min_score,
+            max_score=search_config.max_score,
+            allow_karaoke=search_config.allow_karaoke,
+        ) if results else None
 
-            results = self._get_results(item, kind=RemoteObjectType.TRACK, settings=self.settings_items)
-            if not results:
-                continue
-
-            result = self.match(
-                item,
-                results=map(lambda response: self._object_cls.track(api=self.api, response=response), results),
-                match_on=self.settings_items.match_fields,
-                min_score=self.settings_items.min_score,
-                max_score=self.settings_items.max_score,
-                allow_karaoke=self.settings_items.allow_karaoke,
-            )
+        return item, result
 
-            if result and result.has_uri:
-                item.uri = result.uri
+    def _search_items[T: MusifyItemSettable](self, collection: Iterable[T]) -> None:
+        """Search for matches on individual items in an item collection that have ``None`` on ``has_uri`` attribute"""
+        with ThreadPoolExecutor(thread_name_prefix="searcher-items") as executor:
+            matches = executor.map(self._get_item_match, filter(lambda i: i.has_uri is None, collection))
 
-    def _search_album(self, collection: ItemCollection) -> None:
-        """Search for matches on an entire album"""
+        for item, match in matches:
+            if match and match.has_uri:
+                item.uri = match.uri
+
+    def _search_collection_unit[T: MusifyItemSettable](self, collection: MusifyCollection[T]) -> None:
+        """
+        Search for matches on an entire collection as a whole
+        i.e. search for just the collection and not its distinct items.
+        """
         if all(item.has_uri for item in collection):
             return
 
-        results = self._get_results(collection, kind=RemoteObjectType.ALBUM, settings=self.settings_albums)
+        kind = self._determine_remote_object_type(collection)
+        search_config = self.search_settings[kind]
 
-        # convert to RemoteAlbum objects and extend items on each response
-        albums = list(map(
-            lambda response: self._object_cls.album(api=self.api, response=response, skip_checks=True), results
-        ))
-        kind = RemoteObjectType.ALBUM
+        responses = self._get_results(collection, kind=kind, settings=search_config)
         key = self.api.collection_item_map[kind]
-        for album in albums:  # extend album's tracks
-            self.api.extend_items(album.response, kind=kind, key=key, use_cache=self.use_cache)
+        for response in responses:
+            self.api.extend_items(response, kind=kind, key=key, use_cache=self.use_cache)
 
+        # noinspection PyProtectedMember,PyTypeChecker
         # order to prioritise results that are closer to the item count of the input collection
-        albums.sort(key=lambda x: abs(x.track_total - len(collection)))
-        # noinspection PyTypeChecker
-        result = self.match(
+        results: list[T] = sorted(map(self.factory[kind], responses), key=lambda x: abs(x._total - len(collection)))
+
+        result = self.matcher(
             collection,
-            results=albums,
-            match_on=self.settings_albums.match_fields,
-            min_score=self.settings_albums.min_score,
-            max_score=self.settings_albums.max_score,
-            allow_karaoke=self.settings_albums.allow_karaoke,
+            results=results,
+            match_on=search_config.match_fields,
+            min_score=search_config.min_score,
+            max_score=search_config.max_score,
+            allow_karaoke=search_config.allow_karaoke,
         )
 
         if not result:
             return
 
-        for item in filter(lambda i: i.has_uri is None, collection):
-            # match items back onto the result to discern which URI matches which
-            item_result = self.match(
-                item,
-                results=result.items,
-                match_on=[Tag.TITLE],
-                min_score=self.settings_items.min_score,
-                max_score=self.settings_items.max_score,
-                allow_karaoke=self.settings_items.allow_karaoke,
+        with ThreadPoolExecutor(thread_name_prefix="searcher-collection") as executor:
+            matches = executor.map(
+                lambda item: self._get_item_match(item, match_on=[Tag.TITLE], results=result.items),
+                filter(lambda i: i.has_uri is None, collection)
             )
-            if item_result:
-                item.uri = item_result.uri
+
+        for item, match in matches:
+            if match and match.has_uri:
+                item.uri = match.uri
+
+    def as_dict(self) -> dict[str, Any]:
+        return {
+            "matcher": self.matcher,
+            "remote_source": self.factory.api.source,
+            "interval": self.use_cache,
+        }
```

### Comparing `musify-0.8.1/musify/shared/remote/processors/wrangle.py` & `musify-0.9.0/musify/libraries/remote/core/processors/wrangle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,50 @@
 """
 Convert and validate remote ID and item types according to specific remote implementations.
 """
-
-from abc import ABCMeta, abstractmethod
+from abc import ABC, abstractmethod
 from collections.abc import Mapping
 from typing import Any
 
-from musify.shared.remote import Remote
-from musify.shared.remote.enum import RemoteIDType, RemoteObjectType
-from musify.shared.remote.exception import RemoteObjectTypeError
-from musify.shared.remote.types import APIMethodInputType
+from musify.libraries.remote.core import RemoteResponse
+from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
+from musify.libraries.remote.core.exception import RemoteObjectTypeError
+from musify.libraries.remote.core.types import APIInputValue
 
 
-class RemoteDataWrangler(Remote, metaclass=ABCMeta):
+class RemoteDataWrangler(ABC):
+    """Convert and validate remote ID and item types according to specific remote implementations."""
+
+    @property
+    @abstractmethod
+    def source(self) -> str:
+        """The name of the service for which data can be processed by this wrangler"""
+        raise NotImplementedError
 
     @property
     @abstractmethod
     def unavailable_uri_dummy(self) -> str:
         """
         The value to use as a URI for an item which does not have an associated remote object.
         An item that has this URI value will be excluded from most remote logic.
         """
         raise NotImplementedError
 
+    @property
+    @abstractmethod
+    def url_api(self) -> str:
+        """The base URL of the API for this remote source"""
+        raise NotImplementedError
+
+    @property
+    @abstractmethod
+    def url_ext(self) -> str:
+        """The base URL of external links for this remote source"""
+        raise NotImplementedError
+
     @staticmethod
     @abstractmethod
     def get_id_type(value: str, kind: RemoteObjectType | None = None) -> RemoteIDType:
         """
         Determine the remote ID type of the given ``value`` and return its type.
 
         :param value: URL/URI/ID to check.
@@ -40,33 +58,36 @@
     @classmethod
     @abstractmethod
     def validate_id_type(cls, value: str, kind: RemoteIDType = RemoteIDType.ALL) -> bool:
         """Check that the given ``value`` is a type of remote ID given by ``kind``"""
         raise NotImplementedError
 
     @classmethod
-    def get_item_type(cls, values: APIMethodInputType, kind: RemoteObjectType | None = None) -> RemoteObjectType:
+    def get_item_type(cls, values: APIInputValue, kind: RemoteObjectType | None = None) -> RemoteObjectType:
         """
         Determine the remote object type of ``values``.
 
         ``values`` may be:
             * A string representing a URL/URI/ID.
             * A MutableSequence of strings representing URLs/URIs/IDs of the same type.
             * A remote API JSON response for a collection including a valid item type value under a ``type`` key.
             * A MutableSequence of remote API JSON responses for a collection including the same structure as above.
+            * A RemoteResponse of the appropriate type for this RemoteAPI which holds a valid API JSON response
+              as described above.
+            * A Sequence of RemoteResponses as above.
 
         :param values: The values representing some remote objects. See description for allowed value types.
             These items must all be of the same type of item to pass i.e. all tracks OR all artists etc.
-        :param kind: The :py:class:`RemoteObjectType` if the value is found to be an ID.
+        :param kind: The :py:class:`RemoteObjectType` to use as backup if the value is found to be an ID.
         :return: The :py:class:`RemoteObjectType`
         :raise RemoteObjectTypeError: Raised when the function cannot determine the item type
             of the input ``values``.
             Or when the list contains strings representing many differing remote object types or only IDs.
         """
-        if isinstance(values, str) or isinstance(values, Mapping):
+        if isinstance(values, str | Mapping | RemoteResponse):
             return cls._get_item_type(value=values, kind=kind)
 
         if len(values) == 0:
             raise RemoteObjectTypeError("No values given: collection is empty")
 
         kinds = {cls._get_item_type(value=value, kind=kind) for value in values if value is not None}
         kinds.discard(None)
@@ -75,42 +96,48 @@
         if len(kinds) != 1:
             value = [kind.name for kind in kinds]
             raise RemoteObjectTypeError("Ensure all the given items are of the same type! Found", value=value)
         return kinds.pop()
 
     @staticmethod
     @abstractmethod
-    def _get_item_type(value: str | Mapping[str, Any], kind: RemoteObjectType) -> RemoteObjectType | None:
+    def _get_item_type(
+            value: str | Mapping[str, Any] | RemoteResponse, kind: RemoteObjectType | None = None
+    ) -> RemoteObjectType | None:
         """
         Determine the remote object type of the given ``value`` and return its type.
 
         ``value`` may be:
             * A string representing a URL/URI/ID.
             * A remote API JSON response for a collection with a valid ID value under an ``id`` key.
+            * A RemoteResponse containing a remote API JSON response with the same structure as above.
 
         :param value: The value representing some remote collection. See description for allowed value types.
-        :param kind: The :py:class:`RemoteObjectType` if the value is found to be an ID.
+        :param kind: The :py:class:`RemoteObjectType` to use as backup if the value is found to be an ID.
         :return: The :py:class:`RemoteObjectType`. If the given value is determined to be an ID, returns None.
         :raise RemoteObjectTypeError: Raised when the function cannot determine the item type
             of the input ``values``.
         :raise EnumNotFoundError: Raised when the item type of the given ``value`` is not
             a valid remote object type.
         """
         raise NotImplementedError
 
     @classmethod
-    def validate_item_type(cls, values: APIMethodInputType, kind: RemoteObjectType) -> None:
+    def validate_item_type(cls, values: APIInputValue, kind: RemoteObjectType) -> None:
         """
         Check that the given ``values`` are a type of item given by ``kind`` or a simple ID.
 
         ``values`` may be:
             * A string representing a URL/URI/ID.
             * A MutableSequence of strings representing URLs/URIs/IDs of the same type.
             * A remote API JSON response for a collection including a valid item type value under a ``type`` key.
             * A MutableSequence of remote API JSON responses for a collection including the same structure as above.
+            * A RemoteResponse of the appropriate type for this RemoteAPI which holds a valid API JSON response
+              as described above.
+            * A Sequence of RemoteResponses as above.
 
         :param values: The values representing some remote objects. See description for allowed value types.
             These items must all be of the same type of item to pass i.e. all tracks OR all artists etc.
         :param kind: The remote object type to check for.
         :raise RemoteObjectTypeError: Raised when the function cannot validate the item type
             of the input ``values`` is of type ``kind`` or a simple ID.
         """
@@ -140,25 +167,28 @@
         :raise RemoteIDTypeError: Raised when the function cannot determine the item type
             of the input ``value``.
         """
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
-    def extract_ids(cls, values: APIMethodInputType, kind: RemoteObjectType | None = None) -> list[str]:
+    def extract_ids(cls, values: APIInputValue, kind: RemoteObjectType | None = None) -> list[str]:
         """
         Extract a list of IDs from input ``values``.
 
         ``values`` may be:
             * A string representing a URL/URI/ID.
             * A MutableSequence of strings representing URLs/URIs/IDs of the same type.
             * A remote API JSON response for a collection including:
                 - a valid ID value under an ``id`` key,
                 - a valid item type value under a ``type`` key if ``kind`` is None.
             * A MutableSequence of remote API JSON responses for a collection including the same structure as above.
+            * A RemoteResponse of the appropriate type for this RemoteAPI which holds a valid API JSON response
+              as described above.
+            * A Sequence of RemoteResponses as above.
 
         :param values: The values representing some remote objects. See description for allowed value types.
             These items may be of mixed item types e.g. some tracks AND some artists.
         :param kind: Optionally, give the item type of the input ``value`` to skip some checks.
             This is required when the given ``value`` is an ID.
         :return: List of IDs.
         :raise RemoteError: Raised when the function cannot determine the item type of the input ``values``.
```

### Comparing `musify-0.8.1/musify/spotify/base.py` & `musify-0.9.0/musify/libraries/remote/spotify/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,48 @@
 """
 Core abstract classes for the :py:mod:`Spotify` module.
 
 These define the foundations of any Spotify object or item.
 """
-
 from abc import ABCMeta
 from typing import Any
 
-from musify.shared.remote.base import RemoteObject, RemoteItem
-from musify.shared.remote.enum import RemoteObjectType
-from musify.shared.remote.exception import RemoteObjectTypeError, RemoteError
-from musify.spotify import SpotifyRemote
-from musify.spotify.api import SpotifyAPI
-
-
-class SpotifyObjectMixin(RemoteObject, SpotifyRemote, metaclass=ABCMeta):
-    """Mixin for :py:class:`RemoteObject` and :py:class:`SpotifyRemote`"""
-    pass
+from musify.libraries.remote.core.base import RemoteObject, RemoteItem
+from musify.libraries.remote.core.enum import RemoteObjectType
+from musify.libraries.remote.core.exception import RemoteObjectTypeError, RemoteError
+from musify.libraries.remote.spotify.api import SpotifyAPI
 
 
-class SpotifyObject(SpotifyObjectMixin, metaclass=ABCMeta):
+class SpotifyObject(RemoteObject[SpotifyAPI], metaclass=ABCMeta):
     """Generic base class for Spotify-stored objects. Extracts key data from a Spotify API JSON response."""
 
     _url_pad = 71
 
     @property
-    def id(self) -> str:
-        """The ID of this item/collection."""
+    def id(self):
         return self.response["id"]
 
     @property
-    def uri(self) -> str:
-        """The URI of this item/collection."""
+    def uri(self):
         return self.response["uri"]
 
     @property
-    def has_uri(self) -> bool:
-        """Does this item/collection have a valid URI that is not a local URI."""
+    def has_uri(self):
         return not self.response.get("is_local", False)
 
     @property
-    def url(self) -> str:
-        """The API URL of this item/collection."""
+    def url(self):
         return self.response["href"]
 
     @property
-    def url_ext(self) -> str | None:
-        """The external URL of this item/collection."""
+    def url_ext(self):
         return self.response["external_urls"].get("spotify")
 
     def __init__(self, response: dict[str, Any], api: SpotifyAPI | None = None, skip_checks: bool = False):
         super().__init__(response=response, api=api, skip_checks=skip_checks)
-        # noinspection PyTypeChecker
-        self.api: SpotifyAPI = self.api
 
     def _check_type(self) -> None:
         """
         Checks the given response is compatible with this object type, raises an exception if not.
 
         :raise RemoteObjectTypeError: When the response type is not compatible with this object.
         """
@@ -67,10 +53,10 @@
 
         kind = self.__class__.__name__.removeprefix("Spotify").lower()
         if self.response.get("type") != kind:
             kind = RemoteObjectType.from_name(kind)[0]
             raise RemoteObjectTypeError("Response type invalid", kind=kind, value=self.response.get("type"))
 
 
-class SpotifyItem(RemoteItem, SpotifyObject, metaclass=ABCMeta):
+class SpotifyItem(SpotifyObject, RemoteItem, metaclass=ABCMeta):
     """Generic base class for Spotify-stored items. Extracts key data from a Spotify API JSON response."""
     pass
```

### Comparing `musify-0.8.1/musify/spotify/exception.py` & `musify-0.9.0/musify/libraries/remote/spotify/exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Exceptions relating to Spotify operations.
 """
-
-from musify.shared.remote.exception import RemoteError
+from musify.libraries.remote.core.exception import RemoteError
 
 
 class SpotifyError(RemoteError):
     """
     Exception raised for Spotify ID errors.
 
     :param message: Explanation of the error.
```

### Comparing `musify-0.8.1/musify/spotify/library.py` & `musify-0.9.0/musify/libraries/remote/spotify/library.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,44 @@
 """
 Implements a :py:class:`RemoteLibrary` for Spotify.
 """
-
-from collections.abc import Collection, Mapping, Iterable
+from collections.abc import Collection, Iterable
 from typing import Any
 
-from musify.shared.core.object import Playlist, Library
-from musify.shared.remote.config import RemoteObjectClasses
-from musify.shared.remote.enum import RemoteObjectType
-from musify.shared.remote.library import RemoteLibrary
-from musify.shared.remote.object import RemoteTrack
-from musify.spotify.api import SpotifyAPI
-from musify.spotify.config import SPOTIFY_OBJECT_CLASSES
-from musify.spotify.object import SpotifyTrack, SpotifyCollection, SpotifyPlaylist, SpotifyAlbum, SpotifyArtist
+from musify.libraries.remote.core.enum import RemoteObjectType
+from musify.libraries.remote.core.library import RemoteLibrary
+from musify.libraries.remote.spotify.api import SpotifyAPI
+from musify.libraries.remote.spotify.factory import SpotifyObjectFactory
+from musify.libraries.remote.spotify.object import SpotifyTrack, SpotifyAlbum, SpotifyArtist, SpotifyPlaylist
 
 
-class SpotifyLibrary(RemoteLibrary[SpotifyTrack], SpotifyCollection[SpotifyTrack]):
+class SpotifyLibrary(RemoteLibrary[SpotifyAPI, SpotifyPlaylist, SpotifyTrack, SpotifyAlbum, SpotifyArtist]):
     """
     Represents a Spotify library. Provides various methods for manipulating
     tracks and playlists across an entire Spotify library collection.
     """
     __attributes_classes__ = RemoteLibrary
 
     @staticmethod
     def _validate_item_type(items: Any | Iterable[Any]) -> bool:
         if isinstance(items, Iterable):
             return all(isinstance(item, SpotifyTrack) for item in items)
         return isinstance(items, SpotifyTrack)
 
-    @property
-    def _object_cls(self) -> RemoteObjectClasses:
-        return SPOTIFY_OBJECT_CLASSES
-
-    # noinspection PyTypeChecker
-    @property
-    def playlists(self) -> dict[str, SpotifyPlaylist]:
-        return self._playlists
-
-    # noinspection PyTypeChecker
-    @property
-    def albums(self) -> list[SpotifyAlbum]:
-        return self._albums
-
-    # noinspection PyTypeChecker
-    @property
-    def artists(self) -> list[SpotifyArtist]:
-        return self._artists
-
-    # noinspection PyTypeChecker
-    @property
-    def api(self) -> SpotifyAPI:
-        return self._api
+    def _create_factory(self, api: SpotifyAPI) -> SpotifyObjectFactory:
+        return SpotifyObjectFactory(api=api)
 
     def _filter_playlists(self, responses: list[dict[str, Any]]) -> list[dict[str, Any]]:
         pl_total = len(responses)
         pl_names_filtered = self.playlist_filter({response["name"] for response in responses})
         responses = [response for response in responses if response["name"] in pl_names_filtered]
 
         self.logger.debug(
-            f"Filtered out {pl_total - len(responses)} playlists from {pl_total} {self.source} available playlists"
+            f"Filtered out {pl_total - len(responses)} playlists from "
+            f"{pl_total} {self.api.source} available playlists"
             if (pl_total - len(responses)) > 0 else f"{len(responses)} playlists found"
         )
 
         return responses
 
     def _get_total_tracks(self, responses: list[dict[str, Any]]) -> int:
         return sum(pl["tracks"]["total"] for pl in responses)
@@ -77,19 +53,21 @@
         :param analysis: Load all audio analyses (technical audio data).
             WARNING: can be very slow as calls to this endpoint cannot be batched i.e. one call per track.
         :param albums: Reload albums for all tracks, adding extra album data e.g. genres, popularity
         :param artists: Reload artists for all tracks, adding extra artist data e.g. genres, popularity, followers
         """
         if not self.tracks or not any((features, analysis, albums, artists)):
             return
-        self.logger.debug(f"Enrich {self.source} tracks: START")
-        self.logger.info(f"\33[1;95m  >\33[1;97m Enriching {len(self.tracks)} {self.source} tracks \33[0m")
+        self.logger.debug(f"Enrich {self.api.source} tracks: START")
+        self.logger.info(
+            f"\33[1;95m  >\33[1;97m Enriching {len(self.tracks)} {self.api.source} tracks \33[0m"
+        )
 
-        responses = [track.response for track in self.tracks if track.has_uri]
-        self.api.get_tracks_extra(responses, features=features, analysis=analysis, use_cache=self.use_cache)
+        tracks = [track for track in self.tracks if track.has_uri]
+        self.api.extend_tracks(tracks, features=features, analysis=analysis, use_cache=self.use_cache)
 
         # enrich on list of URIs to avoid duplicate calls for same items
         if albums:
             album_uris: set[str] = {track.response["album"]["uri"] for track in self.tracks}
             album_responses = self.api.get_items(
                 album_uris, kind=RemoteObjectType.ALBUM, extend=False, use_cache=self.use_cache
             )
@@ -107,72 +85,61 @@
             )
 
             artists = {response["uri"]: response for response in artist_responses}
             for track in self.tracks:
                 track.response["artists"] = [artists[artist["uri"]] for artist in track.response["artists"]]
 
         for track in self.tracks:
-            track.refresh(skip_checks=False)  # tracks are popped from albums so checks will skip by default
+            track.refresh(skip_checks=False)  # tracks are popped from albums so checks should skip by default anyway
 
-        self.logger.debug(f"Enrich {self.source} tracks: DONE\n")
+        self.logger.debug(f"Enrich {self.api.source} tracks: DONE\n")
 
     def enrich_saved_albums(self) -> None:
         """Extends the tracks data for currently loaded albums, getting all available tracks data for each album"""
         if not self.albums or all(len(album) == album.track_total for album in self.albums):
             return
-        self.logger.debug(f"Enrich {self.source} artists: START")
-        self.logger.info(f"\33[1;95m  >\33[1;97m Enriching {len(self.albums)} {self.source} albums \33[0m")
+        self.logger.debug(f"Enrich {self.api.source} artists: START")
+        self.logger.info(
+            f"\33[1;95m  >\33[1;97m Enriching {len(self.albums)} {self.api.source} albums \33[0m"
+        )
 
         kind = RemoteObjectType.ALBUM
         key = self.api.collection_item_map[kind]
-        responses = [album.response for album in self.albums]
-        for response in responses:
-            self.api.extend_items(response, kind=kind, key=key, use_cache=self.use_cache)
 
         for album in self.albums:
-            album.refresh(skip_checks=False)  # tracks are extended so checks should pass
+            self.api.extend_items(album, kind=kind, key=key, use_cache=self.use_cache)
+            album.refresh(skip_checks=False)
 
             for track in album.tracks:  # add tracks from this album to the user's saved tracks
                 if track not in self.tracks:
                     self._tracks.append(track)
 
-        self.logger.debug(f"Enrich {self.source} artists: DONE\n")
+        self.logger.debug(f"Enrich {self.api.source} artists: DONE\n")
 
     def enrich_saved_artists(self, tracks: bool = False, types: Collection[str] = ()) -> None:
         """
         Gets all albums for current loaded following artists.
 
         :param tracks: When True, also get all tracks for each album.
         :param types: Provide a list of albums types to get to limit the types of albums loaded.
             Select from ``{"album", "single", "compilation", "appears_on"}``.
         """
         if not self.artists:
             return
-        self.logger.debug(f"Enrich {self.source} artists: START")
-        self.logger.info(f"\33[1;95m  >\33[1;97m Enriching {len(self.artists)} {self.source} artists \33[0m")
-
-        responses = [artist.response for artist in self.artists]
-        self.api.get_artist_albums(responses, types=types, use_cache=self.use_cache)
+        self.logger.debug(f"Enrich {self.api.source} artists: START")
+        self.logger.info(
+            f"\33[1;95m  >\33[1;97m Enriching {len(self.artists)} {self.api.source} artists \33[0m"
+        )
 
-        for artist in self.artists:
-            artist.refresh(skip_checks=True)  # album tracks extended in next step if required
+        self.api.get_artist_albums(self.artists, types=types, use_cache=self.use_cache)
 
         if tracks:
             kind = RemoteObjectType.ALBUM
             key = self.api.collection_item_map[kind]
 
-            responses_albums = [album.response for artist in self.artists for album in artist.albums]
+            responses_albums = [album for artist in self.artists for album in artist.albums]
             bar = self.logger.get_progress_bar(iterable=responses_albums, desc="Getting album tracks", unit="albums")
             for album in bar:
                 self.api.extend_items(album, kind=kind, key=key, use_cache=self.use_cache)
+                album.refresh(skip_checks=False)
 
-            for artist in self.artists:
-                for album in artist.albums:
-                    album.refresh(skip_checks=False)
-
-        self.logger.debug(f"Enrich {self.source} artists: DONE\n")
-
-    def merge_playlists(
-            self,
-            playlists: Library[RemoteTrack] | Collection[Playlist[RemoteTrack]] | Mapping[Any, Playlist[RemoteTrack]]
-    ) -> None:
-        raise NotImplementedError
+        self.logger.debug(f"Enrich {self.api.source} artists: DONE\n")
```

### Comparing `musify-0.8.1/musify/spotify/object.py` & `musify-0.9.0/musify/libraries/remote/spotify/object.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 """
 Implements all :py:mod:`Remote` object types for Spotify.
 """
-
 from __future__ import annotations
 
-from abc import ABCMeta
-from collections.abc import Iterable, MutableMapping, Mapping
+from abc import ABCMeta, abstractmethod
+from collections.abc import Iterable, MutableMapping, Mapping, Collection
 from copy import copy, deepcopy
 from datetime import datetime
 from typing import Any, Self
 
-from musify.shared.remote.enum import RemoteObjectType, RemoteIDType
-from musify.shared.remote.object import RemoteCollection, RemoteCollectionLoader, RemoteTrack
-from musify.shared.remote.object import RemotePlaylist, RemoteAlbum, RemoteArtist
-from musify.shared.types import UnitCollection
-from musify.shared.utils import to_collection
-from musify.spotify.api import SpotifyAPI
-from musify.spotify.base import SpotifyObject, SpotifyItem
-from musify.spotify.exception import SpotifyCollectionError
-from musify.spotify.processors.wrangle import SpotifyDataWrangler
-
-
-class SpotifyItemWranglerMixin(SpotifyItem, SpotifyDataWrangler, metaclass=ABCMeta):
-    """Mixin for :py:class:`SpotifyItem` and :py:class:`SpotifyDataWrangler`"""
-    pass
+from musify.libraries.remote.core import RemoteResponse
+from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
+from musify.libraries.remote.core.object import RemoteCollectionLoader, RemoteTrack
+from musify.libraries.remote.core.object import RemotePlaylist, RemoteAlbum, RemoteArtist
+from musify.libraries.remote.spotify.api import SpotifyAPI
+from musify.libraries.remote.spotify.base import SpotifyObject, SpotifyItem
+from musify.libraries.remote.spotify.exception import SpotifyCollectionError
+from musify.types import UnitCollection
+from musify.utils import to_collection
 
 
-class SpotifyTrack(SpotifyItemWranglerMixin, RemoteTrack):
+class SpotifyTrack(SpotifyItem, RemoteTrack):
     """
     Extracts key ``track`` data from a Spotify API JSON response.
 
     :param response: The Spotify API JSON response.
     """
 
     __slots__ = ("_artists", "_disc_total", "_comments")
@@ -207,165 +201,201 @@
             SpotifyArtist(artist, api=self.api, skip_checks=skip_checks)
             for artist in self._response.get("artists", {})
         ]
 
     @classmethod
     def load(
             cls,
-            value: str | dict[str, Any],
+            value: str | Mapping[str, Any] | RemoteResponse,
             api: SpotifyAPI,
             features: bool = False,
             analysis: bool = False,
             extend_album: bool = False,
             extend_artists: bool = False,
             use_cache: bool = True,
             *_,
             **__
     ) -> Self:
-        obj = cls.__new__(cls)
-        obj.api = api
+        self = cls.__new__(cls)
+        self.api = api
 
         # set a mock response with URL to load from
-        id_ = cls.extract_ids(value)[0]
-        obj._response = {
-            "href": cls.convert(id_, kind=RemoteObjectType.TRACK, type_in=RemoteIDType.ID, type_out=RemoteIDType.URL)
+        id_ = api.wrangler.extract_ids(value)[0]
+        self._response = {
+            "href": api.wrangler.convert(
+                id_, kind=RemoteObjectType.TRACK, type_in=RemoteIDType.ID, type_out=RemoteIDType.URL
+            )
         }
-        obj.reload(
+        self.reload(
             features=features,
             analysis=analysis,
             extend_album=extend_album,
             extend_artists=extend_artists,
             use_cache=use_cache
         )
-        return obj
+        return self
 
     def reload(
             self,
+            use_cache: bool = True,
             features: bool = False,
             analysis: bool = False,
             extend_album: bool = False,
             extend_artists: bool = False,
-            use_cache: bool = True,
             *_,
             **__
     ) -> None:
         self._check_for_api()
 
         # reload with enriched data
         response = self.api.handler.get(self.url, use_cache=use_cache, log_pad=self._url_pad)
         if extend_album:
             self.api.get_items(response["album"], kind=RemoteObjectType.ALBUM, extend=False, use_cache=use_cache)
         if extend_artists:
             self.api.get_items(response["artists"], kind=RemoteObjectType.ARTIST, use_cache=use_cache)
         if features or analysis:
-            self.api.get_tracks_extra(response, features=features, analysis=analysis, use_cache=use_cache)
+            self.api.extend_tracks(response, features=features, analysis=analysis, use_cache=use_cache)
 
         self.__init__(response=response, api=self.api)
 
 
-class SpotifyCollection[T: SpotifyItem](RemoteCollection[T], SpotifyDataWrangler, metaclass=ABCMeta):
-    """Generic class for storing a collection of Spotify objects."""
+class SpotifyCollectionLoader[T: SpotifyObject](RemoteCollectionLoader[T], SpotifyObject, metaclass=ABCMeta):
+    """Generic class for storing a collection of Spotify objects that can be loaded from an API response."""
 
+    @classmethod
+    def _get_item_kind(cls, api: SpotifyAPI) -> RemoteObjectType:
+        """Returns the :py:class:`RemoteObjectType` for the items in this collection"""
+        return api.collection_item_map[cls.kind]
 
-class SpotifyObjectLoaderMixin[T: SpotifyItem](RemoteCollectionLoader[T], SpotifyObject, metaclass=ABCMeta):
-    """Mixin for :py:class:`RemoteCollectionLoader` and :py:class:`SpotifyObject`"""
-    pass
+    @classmethod
+    @abstractmethod
+    def _get_items(
+            cls, items: Collection[str] | MutableMapping[str, Any], api: SpotifyAPI, use_cache: bool = True
+    ) -> list[dict[str, Any]]:
+        """Call the ``api`` to get values for the given ``items`` URIs"""
+        raise NotImplementedError
 
+    @classmethod
+    def _filter_items(cls, items: Iterable[T], response: Mapping[str, Any]) -> Iterable[T]:
+        """
+        Filter down and return only ``items`` associated with the given ``response``.
+        The default implementation of this will just return the given ``items``.
+        Override for object-specific filtering.
+        """
+        return items
 
-class SpotifyCollectionLoader[T: SpotifyItem](SpotifyObjectLoaderMixin[T], SpotifyCollection[T], metaclass=ABCMeta):
-    """Generic class for storing a collection of Spotify objects that can be loaded from an API response."""
+    @classmethod
+    def _extend_response(
+            cls, response: MutableMapping[str, Any], api: SpotifyAPI, use_cache: bool = True, *_, **__
+    ) -> bool:
+        """
+        Apply extensions to specific aspects of the given ``response``.
+        Does nothing by default. Override to implement object-specific extensions.
+
+        :return: True if checks should be skipped when initialising the object.
+        """
+        pass
+
+    @classmethod
+    def _merge_items_to_response(
+            cls,
+            items: Iterable[T | Mapping[str, Any]],
+            response: Iterable[MutableMapping[str, Any]],
+            skip: Collection[str] = ()
+    ) -> tuple[set[str], set[str]]:
+        """
+        Find items in the ``response`` that match from the given ``items`` and replace them in the response.
+        Optionally, provide a list of URIs to ``skip``.
+
+        :return: Two sets of URIs for items that could and could not be found in response.
+        """
+        items_mapped: dict[str, T | Mapping[str, Any]] = {
+            item.uri if isinstance(item, SpotifyObject) else item["uri"]: item for item in items
+        }
+        uri_matched: set[str] = set()
+        uri_missing: set[str] = set()
+
+        # find items in the response that match from the given items
+        for source_item in response:
+            if cls.kind == RemoteObjectType.PLAYLIST:
+                source_item = source_item["track"]
+
+            if source_item["uri"] in skip:
+                continue
+            elif source_item["uri"] in items_mapped:
+                # replace the skeleton response with the response from the given items
+                replacement_item = items_mapped.pop(source_item["uri"])
+                if isinstance(replacement_item, SpotifyObject):
+                    replacement_item = replacement_item.response
+
+                source_item.clear()
+                source_item |= replacement_item
+                uri_matched.add(source_item["uri"])
+            elif not source_item.get("is_local"):  # add to missing list
+                uri_missing.add(source_item["uri"])
+
+        return uri_matched, uri_missing
+
+    @classmethod
+    def _load_new(cls, value: str | Mapping[str, Any] | RemoteResponse, api: SpotifyAPI, *args, **kwargs) -> Self:
+        """
+        Sets up a new object of the current class for the given ``value`` by calling ``__new__``
+        and adding just enough attributes to the object to get :py:meth:`reload` to run.
+        """
+        # noinspection PyTypeChecker
+        id_ = next(iter(api.wrangler.extract_ids(values=value, kind=cls.kind)))
+        # noinspection PyTypeChecker
+        url = api.wrangler.convert(id_, kind=cls.kind, type_in=RemoteIDType.ID, type_out=RemoteIDType.URL)
+
+        self = cls.__new__(cls)
+        self.api = api
+        self._response = {"href": url}
+
+        self.reload(*args, **kwargs)
+        return self
 
     @classmethod
     def load(
             cls,
-            value: str | MutableMapping[str, Any],
+            value: str | Mapping[str, Any] | RemoteResponse,
             api: SpotifyAPI,
-            items: Iterable[SpotifyTrack] = (),
-            extend_tracks: bool = False,
             use_cache: bool = True,
+            items: Iterable[T] = (),
             leave_bar: bool = True,
             *args,
             **kwargs
     ) -> Self:
-        unit = cls.__name__.removeprefix("Spotify").lower()
-        kind = RemoteObjectType.from_name(unit)[0]
-        key = api.collection_item_map[kind].name.lower() + "s"
+        item_kind = cls._get_item_kind(api=api)
+        item_key = item_kind.name.lower() + "s"
+
+        if isinstance(value, RemoteResponse):
+            value = value.response
 
         # no items given, regenerate API response from the URL
-        if not items or (isinstance(value, Mapping) and (key not in value or api.items_key not in value[key])):
-            if kind == RemoteObjectType.PLAYLIST:
-                value = api.get_playlist_url(value)
-
-            obj = cls.__new__(cls)
-            obj.api = api
-            obj._response = {"href": value}
-            obj.reload(*args, **kwargs, extend_tracks=extend_tracks, use_cache=use_cache)
-            return obj
+        if any({not items, isinstance(value, Mapping) and api.items_key not in value.get(item_key, [])}):
+            return cls._load_new(value=value, api=api, use_cache=use_cache, *args, **kwargs)
 
-        # get response
-        if isinstance(value, MutableMapping) and cls.get_item_type(value) == kind:
+        if isinstance(value, MutableMapping) and api.wrangler.get_item_type(value) == cls.kind:  # input is response
             response = deepcopy(value)
-        else:  # reload response from the API
-            response = cls.api.get_items(value, kind=kind, use_cache=use_cache)[0]
+        else:  # load fresh response from the API
+            response = cls.api.get_items(value, kind=cls.kind, use_cache=use_cache)[0]
 
-        # attempt to find items for this track collection in the given items
-        if kind == RemoteObjectType.ALBUM:
-            uri_tracks_input: dict[str, SpotifyTrack] = {
-                track.uri: track for track in items if track.response.get("album", {}).get("id") == response["id"]
-            }
-        else:
-            uri_tracks_input: dict[str, SpotifyTrack] = {track.uri: track for track in items}
-        uri_get: list[str] = []
+        # filter down input items to those that match the response
+        items = cls._filter_items(items=items, response=response)
+        matched, missing = cls._merge_items_to_response(items=items, response=response[item_key][api.items_key])
 
-        # loop through the skeleton response for this album, find items that match from the given items
-        for track_response in response[key][api.items_key]:
-            if kind == RemoteObjectType.PLAYLIST:
-                track_response = track_response["track"]
-
-            if track_response["uri"] in uri_tracks_input:
-                # replace the skeleton response with the response from the track
-                track = uri_tracks_input.pop(track_response["uri"])
-                track_response.clear()
-                track_response |= track.response
-            elif not track_response["is_local"]:  # add to get from API list
-                uri_get.append(track_response["uri"])
-
-        if len(uri_get) > 0:  # get remaining items from API
-            uri_tracks_get = {r["uri"]: r for r in api.get_tracks(uri_get, features=True, use_cache=use_cache)}
-
-            for track_response in response[key][api.items_key]:
-                if kind == RemoteObjectType.PLAYLIST:
-                    track_response = track_response["track"]
-
-                track_new: dict[str, Any] = uri_tracks_get.pop(track_response["uri"], None)
-                if track_new:  # replace the skeleton response with the new response
-                    track_response.clear()
-                    track_response |= track_new
-
-        if kind == RemoteObjectType.ALBUM:
-            if len(response[key][api.items_key]) < response["total_tracks"]:
-                response[key][api.items_key].extend([track.response for track in uri_tracks_input.values()])
-            response[key][api.items_key].sort(key=lambda x: x["track_number"])
-
-        extend_response = api.extend_items(
-            response[key],
-            kind=kind,
-            key=api.collection_item_map[kind],
-            use_cache=use_cache,
-            leave_bar=leave_bar
-        )
-        if extend_tracks:
-            if kind == RemoteObjectType.PLAYLIST:
-                extend_response = [item["track"] for item in extend_response]
-            api.get_tracks_extra(extend_response, limit=response[key]["limit"], features=True, use_cache=use_cache)
+        if missing:
+            items_missing = cls._get_items(items=missing, api=api, use_cache=use_cache)
+            cls._merge_items_to_response(items=items_missing, response=response[item_key][api.items_key], skip=matched)
 
-        return cls(response=response, api=api, skip_checks=False)
+        skip_checks = cls._extend_response(response=response, api=api, use_cache=use_cache, *args, **kwargs)
+        return cls(response=response, api=api, skip_checks=skip_checks)
 
 
-class SpotifyPlaylist(RemotePlaylist[SpotifyTrack], SpotifyCollectionLoader[SpotifyTrack]):
+class SpotifyPlaylist(SpotifyCollectionLoader[SpotifyTrack], RemotePlaylist[SpotifyTrack]):
     """
     Extracts key ``playlist`` data from a Spotify API JSON response.
 
     :param response: The Spotify API JSON response
     """
 
     __slots__ = ("_tracks",)
@@ -469,23 +499,65 @@
         self._tracks = [
             SpotifyTrack(track, api=self.api, skip_checks=skip_checks)
             for track in self._response.get("tracks", {}).get("items", [])
         ]
         if not skip_checks:
             self._check_total()
 
-    def reload(self, extend_tracks: bool = False, use_cache: bool = True, *_, **__) -> None:
-        self._check_for_api()
+    @classmethod
+    def _get_items(
+            cls, items: Collection[str] | MutableMapping[str, Any], api: SpotifyAPI, use_cache: bool = True
+    ) -> list[dict[str, Any]]:
+        return api.get_tracks(items, use_cache=use_cache)
+
+    @classmethod
+    def _extend_response(
+            cls,
+            response: MutableMapping[str, Any],
+            api: SpotifyAPI,
+            use_cache: bool = True,
+            leave_bar: bool = True,
+            extend_tracks: bool = False,
+            extend_features: bool = False,
+            *_,
+            **__
+    ) -> bool:
+        item_kind = api.collection_item_map[cls.kind]
 
-        response = self.api.get_items(self.url, kind=RemoteObjectType.PLAYLIST, use_cache=use_cache)[0]
         if extend_tracks:
-            tracks = [track["track"] for track in response["tracks"]["items"]]
-            self.api.get_tracks_extra(tracks, limit=response["tracks"]["limit"], features=True, use_cache=use_cache)
+            # noinspection PyTypeChecker
+            api.extend_items(response, kind=cls.kind, key=item_kind, use_cache=use_cache, leave_bar=leave_bar)
+
+        item_key = item_kind.name.lower() + "s"
+        tracks = [item["track"] for item in response.get(item_key, {}).get(api.items_key, [])]
+        if tracks and extend_features:
+            api.extend_tracks(tracks, limit=response[item_key]["limit"], features=True, use_cache=use_cache)
+
+        return not extend_tracks
+
+    def reload(
+            self,
+            use_cache: bool = True,
+            extend_tracks: bool = False,
+            extend_features: bool = False,
+            *_,
+            **__
+    ) -> None:
+        self._check_for_api()
+        response = self.api.get_items(self.url, kind=RemoteObjectType.PLAYLIST, extend=False, use_cache=use_cache)[0]
+
+        skip_checks = self._extend_response(
+            response=response,
+            api=self.api,
+            use_cache=use_cache,
+            extend_tracks=extend_tracks,
+            extend_features=extend_features
+        )
 
-        self.__init__(response=response, api=self.api, skip_checks=not extend_tracks)
+        self.__init__(response=response, api=self.api, skip_checks=skip_checks)
 
     def _get_track_uris_from_api_response(self) -> list[str]:
         return [track["track"]["uri"] for track in self.response["tracks"]["items"]]
 
 
 class SpotifyAlbum(RemoteAlbum[SpotifyTrack], SpotifyCollectionLoader[SpotifyTrack]):
     """
@@ -564,19 +636,14 @@
         return {"cover_front": url for height, url in images.items() if height == max(images)}
 
     @property
     def has_image(self):
         return len(self.response["images"]) > 0
 
     @property
-    def length(self):
-        lengths = {track.length for track in self.tracks}
-        return sum(lengths) if lengths else None
-
-    @property
     def rating(self):
         return self.response.get("popularity")
 
     def __init__(self, response: dict[str, Any], api: SpotifyAPI | None = None, skip_checks: bool = False):
         self._artists: list[SpotifyArtist] | None = None
         self._tracks: list[SpotifyTrack] | None = None
 
@@ -598,27 +665,76 @@
         ]
         if not skip_checks:
             self._check_total()
 
         for track in self.tracks:
             track.disc_total = self.disc_total
 
+    @classmethod
+    def _get_items(
+            cls, items: Collection[str] | MutableMapping[str, Any], api: SpotifyAPI, use_cache: bool = True
+    ) -> list[dict[str, Any]]:
+        return api.get_tracks(items, use_cache=use_cache)
+
+    @classmethod
+    def _filter_items(cls, items: Iterable[SpotifyTrack], response: Mapping[str, Any]) -> Iterable[SpotifyTrack]:
+        """Filter down and return only ``items`` the items associated with the given ``response``"""
+        return [item for item in items if item.response.get("album", {}).get("id") == response["id"]]
+
+    @classmethod
+    def _extend_response(
+            cls,
+            response: MutableMapping[str, Any],
+            api: SpotifyAPI,
+            use_cache: bool = True,
+            leave_bar: bool = True,
+            extend_tracks: bool = False,
+            extend_artists: bool = False,
+            extend_features: bool = False,
+            *_,
+            **__
+    ) -> bool:
+        item_kind = api.collection_item_map[cls.kind]
+
+        if extend_artists:
+            api.get_items(response["artists"], kind=RemoteObjectType.ARTIST, use_cache=use_cache)
+
+        if extend_tracks:
+            # noinspection PyTypeChecker
+            api.extend_items(response, kind=cls.kind, key=item_kind, use_cache=use_cache, leave_bar=leave_bar)
+
+        item_key = item_kind.name.lower() + "s"
+        tracks = response.get(item_key, {}).get(api.items_key)
+        if tracks and extend_features:
+            api.extend_tracks(tracks, limit=response[item_key]["limit"], features=True, use_cache=use_cache)
+
+        return not extend_tracks
+
     def reload(
-            self, extend_artists: bool = True, extend_tracks: bool = True, use_cache: bool = True, *_, **__
+            self,
+            use_cache: bool = True,
+            extend_artists: bool = False,
+            extend_tracks: bool = False,
+            extend_features: bool = False,
+            *_,
+            **__
     ) -> None:
         self._check_for_api()
+        response = self.api.get_items(self.url, kind=RemoteObjectType.ALBUM, extend=False, use_cache=use_cache)[0]
 
-        response = self.api.get_items(self.url, kind=RemoteObjectType.ALBUM, use_cache=use_cache)[0]
-        if extend_artists:
-            self.api.get_items(response["artists"], kind=RemoteObjectType.ARTIST, use_cache=use_cache)
-        if extend_tracks:
-            tracks = response["tracks"]
-            self.api.get_tracks_extra(tracks["items"], limit=tracks["limit"], features=True, use_cache=use_cache)
+        skip_checks = self._extend_response(
+            response=response,
+            api=self.api,
+            use_cache=use_cache,
+            extend_tracks=extend_tracks,
+            extend_artists=extend_artists,
+            extend_features=extend_features,
+        )
 
-        self.__init__(response=response, api=self.api, skip_checks=not extend_tracks)
+        self.__init__(response=response, api=self.api, skip_checks=skip_checks)
 
 
 class SpotifyArtist(RemoteArtist[SpotifyAlbum], SpotifyCollectionLoader[SpotifyAlbum]):
     """Extracts key ``artist`` data from a Spotify API JSON response."""
 
     __slots__ = ("_albums",)
 
@@ -675,46 +791,82 @@
 
     def refresh(self, skip_checks: bool = False) -> None:
         self._albums = [
             SpotifyAlbum(album, api=self.api, skip_checks=skip_checks)
             for album in self.response.get("albums", {}).get("items", [])
         ]
 
-    # TODO: this currently overrides parent loader because parent loader is too 'tracks' specific
-    #  see if this can be modified to take advantage of the item filtering logic in the parent loader
     @classmethod
-    def load(
+    def _get_item_kind(cls, api: SpotifyAPI) -> RemoteObjectType:
+        return RemoteObjectType.ALBUM
+
+    @classmethod
+    def _get_items(
+            cls, items: Collection[str] | MutableMapping[str, Any], api: SpotifyAPI, use_cache: bool = True
+    ) -> list[dict[str, Any]]:
+        return api.get_items(items, extend=False, use_cache=use_cache)
+
+    @classmethod
+    def _filter_items(cls, items: Iterable[SpotifyAlbum], response: dict[str, Any]) -> Iterable[SpotifyAlbum]:
+        """Filter down and return only ``items`` the items associated with the given ``response``"""
+        return [
+            item for item in items
+            if any(artist["id"] == response["id"] for artist in item.response.get("artists", []))
+        ]
+
+    @classmethod
+    def _extend_response(
             cls,
-            value: str | dict[str, Any],
+            response: MutableMapping[str, Any],
             api: SpotifyAPI,
+            use_cache: bool = True,
+            leave_bar: bool = True,
             extend_albums: bool = False,
             extend_tracks: bool = False,
-            use_cache: bool = True,
+            extend_features: bool = False,
             *_,
             **__
-    ) -> Self:
-        obj = cls.__new__(cls)
-        obj.api = api
+    ) -> bool:
+        item_kind = RemoteObjectType.ALBUM
+        item_key = item_kind.name.lower() + "s"
+
+        response_items = response.get(item_key, {})
+        has_all_albums = item_key in response and len(response_items[api.items_key]) == response_items["total"]
+        if extend_albums and not has_all_albums:
+            api.get_artist_albums(response, limit=response.get(item_key, {}).get("limit", 50), use_cache=use_cache)
+
+        album_item_kind = api.collection_item_map[item_kind]
+        album_item_key = album_item_kind.name.lower() + "s"
+        albums = response.get(item_key, {}).get(api.items_key)
+
+        if albums and extend_tracks:
+            for album in albums:
+                api.extend_items(album[album_item_key], kind=item_kind, key=album_item_kind, use_cache=use_cache)
+
+        if albums and extend_features:
+            tracks = [track for album in albums for track in album[album_item_key]["items"]]
+            api.extend_tracks(tracks, limit=response[item_key]["limit"], features=True, use_cache=use_cache)
 
-        # set a mock response with URL to load from
-        id_ = cls.extract_ids(value)[0]
-        obj._response = {
-            "href": cls.convert(id_, kind=RemoteObjectType.ARTIST, type_in=RemoteIDType.ID, type_out=RemoteIDType.URL)
-        }
-        obj.reload(extend_albums=extend_albums, extend_tracks=extend_tracks, use_cache=use_cache)
-        return obj
+        return not extend_albums or not extend_tracks
 
     def reload(
-            self, extend_albums: bool = False, extend_tracks: bool = False, use_cache: bool = True, *_, **__
+            self,
+            use_cache: bool = True,
+            extend_albums: bool = False,
+            extend_tracks: bool = False,
+            extend_features: bool = False,
+            *_,
+            **__
     ) -> None:
         self._check_for_api()
-
         response = self.api.handler.get(url=self.url, use_cache=use_cache, log_pad=self._url_pad)
-        if extend_albums:
-            self.api.get_artist_albums(response, use_cache=use_cache)
-        if extend_albums and extend_tracks:
-            kind = RemoteObjectType.ALBUM
-            key = self.api.collection_item_map[kind]
-            for album in response["albums"]["items"]:
-                self.api.extend_items(album["tracks"], kind=kind, key=key, use_cache=use_cache)
 
-        self.__init__(response=response, api=self.api, skip_checks=extend_albums and not extend_tracks)
+        skip_checks = self._extend_response(
+            response=response,
+            api=self.api,
+            use_cache=use_cache,
+            extend_albums=extend_albums,
+            extend_tracks=extend_tracks,
+            extend_features=extend_features,
+        )
+
+        self.__init__(response=response, api=self.api, skip_checks=skip_checks)
```

### Comparing `musify-0.8.1/musify/spotify/api/api.py` & `musify-0.9.0/musify/libraries/remote/spotify/api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Mixin for all implementations of :py:class:`RemoteAPI` for the Spotify API.
 
 Also includes the default arguments to be used when requesting authorisation from the Spotify API.
 """
-
 import base64
 from collections.abc import Iterable
 from copy import deepcopy
 
 from musify import PROGRAM_NAME
-from musify.shared.api.exception import APIError
-from musify.shared.utils import safe_format_map
-from musify.spotify import URL_API, URL_AUTH
-from musify.spotify.api.item import SpotifyAPIItems
-from musify.spotify.api.misc import SpotifyAPIMisc
-from musify.spotify.api.playlist import SpotifyAPIPlaylists
+from musify.api.exception import APIError
+from musify.libraries.remote.spotify.api.item import SpotifyAPIItems
+from musify.libraries.remote.spotify.api.misc import SpotifyAPIMisc
+from musify.libraries.remote.spotify.api.playlist import SpotifyAPIPlaylists
+from musify.libraries.remote.spotify.processors import SpotifyDataWrangler
+from musify.utils import safe_format_map
+
+URL_AUTH = "https://accounts.spotify.com"
 
 # user authenticated access with scopes
 SPOTIFY_API_AUTH_ARGS = {
     "auth_args": {
         "url": f"{URL_AUTH}/api/token",
         "data": {
             "grant_type": "authorization_code",
@@ -48,15 +49,15 @@
             "refresh_token": None,
         },
         "headers": {
             "content-type": "application/x-www-form-urlencoded",
             "Authorization": "Basic {client_base64}"
         },
     },
-    "test_args": {"url": f"{URL_API}/me"},
+    "test_args": {"url": "{url}/me"},
     "test_condition": lambda r: "href" in r and "display_name" in r,
     "test_expiry": 600,
     "token_key_path": ["access_token"],
     "header_extra": {"Accept": "application/json", "Content-Type": "application/json"},
 }
 
 
@@ -65,20 +66,14 @@
     Collection of endpoints for the Spotify API.
 
     :param client_id: The client ID to use when authorising requests.
     :param client_secret: The client secret to use when authorising requests.
     :param scopes: The scopes to request access to.
     """
 
-    items_key = "items"
-
-    @property
-    def api_url_base(self) -> str:
-        return URL_API
-
     @property
     def user_id(self) -> str | None:
         """ID of the currently authenticated user"""
         if not self.user_data:
             try:
                 self.user_data = self.get_self()
             except APIError:
@@ -98,16 +93,18 @@
     def __init__(
             self,
             client_id: str | None = None,
             client_secret: str | None = None,
             scopes: Iterable[str] = (),
             **kwargs,
     ):
+        wrangler = SpotifyDataWrangler()
         format_map = {
             "client_id": client_id,
             "client_base64": base64.b64encode(f"{client_id}:{client_secret}".encode()).decode(),
             "scopes": " ".join(scopes),
+            "url": wrangler.url_api
         }
         auth_kwargs = deepcopy(SPOTIFY_API_AUTH_ARGS)
         safe_format_map(auth_kwargs, format_map=format_map)
 
-        super().__init__(**auth_kwargs, **kwargs)
+        super().__init__(wrangler=wrangler, **auth_kwargs, **kwargs)
```

### Comparing `musify-0.8.1/musify/spotify/api/base.py` & `musify-0.9.0/musify/libraries/remote/spotify/api/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 Base functionality to be shared by all classes that implement :py:class:`RemoteAPI` functionality for Spotify.
 """
-
 from abc import ABCMeta
 from typing import Any
 from urllib.parse import parse_qs, urlparse, urlencode, quote, urlunparse
 
-from musify.shared.remote.api import RemoteAPI
-from musify.spotify.processors.wrangle import SpotifyDataWrangler
+from musify.libraries.remote.core.api import RemoteAPI
 
 
-class SpotifyAPIBase(RemoteAPI, SpotifyDataWrangler, metaclass=ABCMeta):
+class SpotifyAPIBase(RemoteAPI, metaclass=ABCMeta):
     """Base functionality required for all endpoint functions for the Spotify API"""
 
     #: The key to reference when extracting items from a collection
     items_key = "items"
 
     @staticmethod
     def format_next_url(url: str, offset: int = 0, limit: int = 20) -> str:
```

### Comparing `musify-0.8.1/musify/spotify/api/item.py` & `musify-0.9.0/musify/libraries/remote/spotify/api/item.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Implements endpoints for getting items from the Spotify API.
 """
-
 import re
 from abc import ABCMeta
 from collections.abc import Collection, Mapping, MutableMapping
 from itertools import batched
 from typing import Any
 from urllib.parse import parse_qs, urlparse
 
-from musify.shared.api.exception import APIError
-from musify.shared.remote.api import APIMethodInputType
-from musify.shared.remote.enum import RemoteObjectType, RemoteIDType
-from musify.shared.remote.exception import RemoteObjectTypeError
-from musify.shared.utils import limit_value
-from musify.spotify.api.base import SpotifyAPIBase
+from musify.api.exception import APIError
+from musify.libraries.remote.core import RemoteResponse
+from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
+from musify.libraries.remote.core.exception import RemoteObjectTypeError
+from musify.libraries.remote.core.types import APIInputValue
+from musify.libraries.remote.spotify.api.base import SpotifyAPIBase
+from musify.utils import limit_value
+
+ARTIST_ALBUM_TYPES = {"album", "single", "compilation", "appears_on"}
 
 
 class SpotifyAPIItems(SpotifyAPIBase, metaclass=ABCMeta):
 
     _bar_threshold = 5
 
     def _get_unit(self, key: str | None = None, kind: str | None = None) -> str:
@@ -131,84 +133,97 @@
         return results
 
     ###########################################################################
     ## GET endpoints
     ###########################################################################
     def extend_items(
             self,
-            items_block: MutableMapping[str, Any],
+            response: MutableMapping[str, Any] | RemoteResponse,
             kind: RemoteObjectType | str | None = None,
             key: RemoteObjectType | None = None,
             use_cache: bool = True,
             leave_bar: bool | None = None,
     ) -> list[dict[str, Any]]:
         """
-        Extend the items for a given ``items_block`` API response.
+        Extend the items for a given API ``response``.
         The function requests each page of the collection returning a list of all items
         found across all pages for this URL.
 
         Updates the value of the ``items`` key in-place by extending the value of the ``items`` key with new results.
 
-        :param items_block: A remote API JSON response for an items type endpoint which includes required keys:
+        If a :py:class:`RemoteResponse`, this function will not refresh itself with the new response.
+        The user must call `refresh` manually after execution.
+
+        :param response: A remote API JSON response for an items type endpoint
+            or a RemoteResponse which contains this response.
+            Must include required keys:
             ``total`` and either ``next`` or ``href``, plus optional keys ``previous``, ``limit``, ``items`` etc.
         :param kind: The type of response being extended. Optional, used only for logging.
         :param key: The type of response of the child objects. Used when selecting nested data for certain responses
             (e.g. user's followed artists).
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         :param leave_bar: When a progress bar is displayed,
             toggle whether this bar should continue to be displayed after the operation is finished.
             When None, allow the logger to decide this setting.
         :return: API JSON responses for each item
         """
+        if isinstance(response, RemoteResponse):
+            response = response.response
+
         key = key.name.lower() + "s" if key else None
-        if key and key in items_block:
-            items_block = items_block[key]
-        if self.items_key not in items_block:
-            items_block[self.items_key] = []
+        if key and key in response:
+            response = response[key]
+        if self.items_key not in response:
+            response[self.items_key] = []
+
+        if len(response[self.items_key]) == response["total"]:  # skip on fully extended response
+            url = response["href"].split("?")[0]
+            self.logger.debug(f"{'SKIP':<7}: {url:<43} | Response already extended")
+            return response[self.items_key]
 
         # this usually happens on the items block of a current user's playlist
-        if "next" not in items_block:
-            items_block["next"] = items_block["href"]
-        if "previous" not in items_block:
-            items_block["previous"] = None
-        if "limit" not in items_block:
-            items_block["limit"] = int(parse_qs(urlparse(items_block["next"]).query).get("limit", [50])[0])
+        if "next" not in response:
+            response["next"] = response["href"]
+        if "previous" not in response:
+            response["previous"] = None
+        if "limit" not in response:
+            response["limit"] = int(parse_qs(urlparse(response["next"]).query).get("limit", [50])[0])
 
         kind = kind.name.lower() + "s" if isinstance(kind, RemoteObjectType) else kind or self.items_key
-        pages = (items_block["total"] - len(items_block[self.items_key])) / (items_block["limit"] or 1)
+        pages = (response["total"] - len(response[self.items_key])) / (response["limit"] or 1)
         bar = self.logger.get_progress_bar(
-            initial=len(items_block[self.items_key]),
-            total=items_block["total"],
+            initial=len(response[self.items_key]),
+            total=response["total"],
             desc=f"Extending {kind}".rstrip("s") if kind[0].islower() else kind,
             unit=key or self.items_key,
             leave=leave_bar,
             disable=pages < self._bar_threshold,
         )
 
-        while items_block.get("next"):  # loop through each page
-            log_count = min(len(items_block[self.items_key]) + items_block["limit"], items_block["total"])
-            log = [f"{log_count:>6}/{items_block["total"]:<6} {key or self.items_key}"]
-
-            response = self.handler.get(items_block["next"], use_cache=use_cache, log_pad=95, log_extra=log)
-            if key and key in response:
-                response = response[key]
-
-            items_block[self.items_key].extend(response[self.items_key])
-            items_block["href"] = response["href"]
-            items_block["next"] = response.get("next")
-            items_block["previous"] = response.get("previous")
+        while response.get("next"):  # loop through each page
+            log_count = min(len(response[self.items_key]) + response["limit"], response["total"])
+            log = [f"{log_count:>6}/{response["total"]:<6} {key or self.items_key}"]
+
+            response_next = self.handler.get(response["next"], use_cache=use_cache, log_pad=95, log_extra=log)
+            if key and key in response_next:
+                response_next = response_next[key]
+
+            response[self.items_key].extend(response_next[self.items_key])
+            response["href"] = response_next["href"]
+            response["next"] = response_next.get("next")
+            response["previous"] = response_next.get("previous")
 
-            bar.update(len(response[self.items_key]))
+            bar.update(len(response_next[self.items_key]))
 
         bar.close()
-        return items_block[self.items_key]
+        return response[self.items_key]
 
     def get_items(
             self,
-            values: APIMethodInputType,
+            values: APIInputValue,
             kind: RemoteObjectType | None = None,
             limit: int = 50,
             extend: bool = True,
             use_cache: bool = True,
     ) -> list[dict[str, Any]]:
         """
         ``GET: /{kind}s`` - Get information for given ``values``.
@@ -217,66 +232,74 @@
             * A string representing a URL/URI/ID.
             * A MutableSequence of strings representing URLs/URIs/IDs of the same type.
             * A remote API JSON response for a collection including:
                 - some items under an ``items`` key,
                 - a valid ID value under an ``id`` key,
                 - a valid item type value under a ``type`` key if ``kind`` is None.
             * A MutableSequence of remote API JSON responses for a collection including the same structure as above.
+            * A RemoteResponse of the appropriate type for this RemoteAPI which holds a valid API JSON response
+              as described above.
+            * A Sequence of RemoteResponses as above.
 
         If JSON response(s) given, this update each response given by merging with the new response
         and replacing the ``items`` with the new results.
 
+        If :py:class:`RemoteResponse` values are given, this function will call `refresh` on them.
+
         :param values: The values representing some remote objects. See description for allowed value types.
             These items must all be of the same type of item i.e. all tracks OR all artists etc.
         :param kind: Item type if given string is ID.
         :param limit: When requests can be batched, size of batches to request.
             This value will be limited to be between ``1`` and ``50`` or ``20`` if getting albums.
         :param extend: When True and the given ``kind`` is a collection of items,
             extend the response to include all items in this collection.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         :return: API JSON responses for each item.
         :raise RemoteObjectTypeError: Raised when the function cannot determine the item type
             of the input ``values``. Or when it does not recognise the type of the input ``values`` parameter.
         """
         # input validation
-        if not values:  # skip on empty
-            self.logger.debug(f"{'SKIP':<7}: {self.api_url_base:<43} | No data given")
+        if not isinstance(values, RemoteResponse) and not values:  # skip on empty
+            url = f"{self.url}/{kind.name.lower() + "s"}" if kind else self.url
+            self.logger.debug(f"{'SKIP':<7}: {url:<43} | No data given")
             return []
         if kind is None:  # determine the item type
-            kind = self.get_item_type(values)
+            kind = self.wrangler.get_item_type(values)
         else:
-            self.validate_item_type(values, kind=kind)
+            self.wrangler.validate_item_type(values, kind=kind)
 
         unit = kind.name.lower() + "s"
-        url = f"{self.api_url_base}/{unit}"
-        id_list = self.extract_ids(values, kind=kind)
+        url = f"{self.url}/{unit}"
+        id_list = self.wrangler.extract_ids(values, kind=kind)
 
         if kind in {RemoteObjectType.USER, RemoteObjectType.PLAYLIST} or len(id_list) <= 1:
             results = self._get_items_multi(url=url, id_list=id_list, kind=unit, use_cache=use_cache)
         else:
             if kind == RemoteObjectType.ALBUM:
                 limit = limit_value(limit, floor=1, ceil=20)
             results = self._get_items_batched(url=url, id_list=id_list, key=unit, use_cache=use_cache, limit=limit)
 
         key = self.collection_item_map.get(kind, kind)
         key_name = key.name.lower() + "s"
         if len(results) == 0 or any(key_name not in result for result in results) or not extend:
-            self._merge_results_to_input(original=values, results=results, ordered=True)
+            self._merge_results_to_input(original=values, responses=results, ordered=True)
+            self._refresh_responses(responses=values, skip_checks=False)
             self.logger.debug(f"{'DONE':<7}: {url:<43} | Retrieved {len(results):>6} {unit}")
             return results
 
         bar = self.logger.get_progress_bar(
             iterable=results, desc=f"Extending {unit}", unit=unit, disable=len(id_list) < self._bar_threshold
         )
 
         for result in bar:
             if result[key_name].get("next") or ("next" not in result[key_name] and result[key_name].get("href")):
                 self.extend_items(result[key_name], kind=kind, key=key, use_cache=use_cache, leave_bar=False)
 
-        self._merge_results_to_input(original=values, results=results, ordered=True)
+        self._merge_results_to_input(original=values, responses=results, ordered=True)
+        self._refresh_responses(responses=values, skip_checks=False)
 
         item_count = sum(len(result[key_name][self.items_key]) for result in results)
         self.logger.debug(
             f"{'DONE':<7}: {url:<71} | Retrieved {item_count:>6} {key_name} across {len(results):>5} {unit}"
         )
 
         return results
@@ -309,138 +332,152 @@
             raise RemoteObjectTypeError(
                 f"Only able to retrieve {kind.name.lower()}s from the currently authenticated user",
                 kind=kind
             )
 
         params = {"limit": limit_value(limit, floor=1, ceil=50)}
         if user is not None:
-            url = f"{self.convert(user, kind=RemoteObjectType.USER, type_out=RemoteIDType.URL)}/{kind.name.lower()}s"
+            url = self.wrangler.convert(user, kind=RemoteObjectType.USER, type_out=RemoteIDType.URL)
+            url = f"{url}/{kind.name.lower()}s"
             desc_qualifier = "user's"
         elif kind == RemoteObjectType.ARTIST:
-            url = f"{self.api_url_base}/me/following"
+            url = f"{self.url}/me/following"
             desc_qualifier = "current user's followed"
             params["type"] = "artist"
         else:
-            url = f"{self.api_url_base}/me/{kind.name.lower()}s"
+            url = f"{self.url}/me/{kind.name.lower()}s"
             desc_qualifier = "current user's" if kind == RemoteObjectType.PLAYLIST else "current user's saved"
 
         desc = f"Getting {desc_qualifier} {kind.name.lower()}s"
         initial = self.handler.get(url, params=params, use_cache=use_cache, log_pad=71)
         results = self.extend_items(initial, kind=desc, key=kind, use_cache=use_cache)
 
         self.logger.debug(f"{'DONE':<7}: {url:<43} | Retrieved {len(results):>6} {kind.name.lower()}s")
 
         return results
 
-    def get_tracks_extra(
+    def extend_tracks(
             self,
-            values: APIMethodInputType,
+            values: APIInputValue,
             features: bool = False,
             analysis: bool = False,
             limit: int = 50,
             use_cache: bool = True,
-    ) -> dict[str, list[dict[str, Any]]]:
+    ) -> list[dict[str, Any]]:
         """
         ``GET: /audio-features`` and/or ``GET: /audio-analysis`` - Get audio features/analysis for given track/s.
 
         ``values`` may be:
             * A string representing a URL/URI/ID of type 'track'.
             * A MutableSequence of strings representing URLs/URIs/IDs of the type 'track'.
             * A remote API JSON response for a track including:
                 - some items under an ``items`` key,
                 - a valid ID value under an ``id`` key.
             * A MutableSequence of remote API JSON responses for a set of tracks including the same structure as above.
+            * A RemoteResponse of the appropriate type for this RemoteAPI which holds a valid API JSON response
+              as described above.
+            * A Sequence of RemoteResponses as above.
 
         If JSON response(s) given, this updates each response given by adding the results
         under the ``audio_features`` and ``audio_analysis`` keys as appropriate.
 
+        If :py:class:`RemoteResponse` values are given, this function will call `refresh` on them.
+
         :param values: The values representing some remote track/s. See description for allowed value types.
         :param features: When True, get audio features.
         :param analysis: When True, get audio analysis.
         :param limit: Size of batches to request when getting audio features.
             This value will be limited to be between ``1`` and ``50``.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         :return: API JSON responses for each item.
             Mapped to ``audio_features`` and ``audio_analysis`` keys as appropriate.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``values`` are not all tracks or IDs.
         """
         # input validation
         if not features and not analysis:  # skip on all False
-            return {}
+            return []
         if not values:  # skip on empty
-            self.logger.debug(f"{'SKIP':<7}: {self.api_url_base:<43} | No data given")
-            return {}
-        self.validate_item_type(values, kind=RemoteObjectType.TRACK)
+            self.logger.debug(f"{'SKIP':<7}: {self.url:<43} | No data given")
+            return []
+        self.wrangler.validate_item_type(values, kind=RemoteObjectType.TRACK)
 
-        id_list = self.extract_ids(values, kind=RemoteObjectType.TRACK)
+        id_list = self.wrangler.extract_ids(values, kind=RemoteObjectType.TRACK)
 
         # value list takes the form [URL, key, batched]
         config: dict[str, tuple[str, str, bool]] = {}
         if features:
-            config["features"] = (f"{self.api_url_base}/audio-features", "audio_features", True)
+            config["features"] = (f"{self.url}/audio-features", "audio_features", True)
         if analysis:
-            config["analysis"] = (f"{self.api_url_base}/audio-analysis", "audio_analysis", False)
+            config["analysis"] = (f"{self.url}/audio-analysis", "audio_analysis", False)
 
-        results: dict[str, list[dict[str, Any]]] = {}
+        results: list[dict[str, Any]]
         if len(id_list) == 1:
             id_ = id_list[0]
+            id_map = {self.id_key: id_}
+
+            result = id_map.copy()
             for (url, key, _) in config.values():
-                results[key] = [self.handler.get(f"{url}/{id_}", use_cache=use_cache, log_pad=43) | {"id": id_}]
+                result[key] = self.handler.get(f"{url}/{id_}", use_cache=use_cache, log_pad=43) | id_map.copy()
+            results = [result]
         else:
+            results = []
             for kind, (url, key, batch) in config.items():
                 method = self._get_items_batched if batch else self._get_items_multi
-                results[key] = method(
+                responses = method(
                     url=url, id_list=id_list, kind=kind, key=key if batch else None, limit=limit, use_cache=use_cache
                 )
+                responses.sort(key=lambda response: id_list.index(response[self.id_key]))
+                responses = [{self.id_key: response[self.id_key], key: response} for response in responses]
+
+                if not results:
+                    results = responses
+                else:
+                    results = [result | response for result, response in zip(results, responses)]
 
-        # re-map results and extend original input if required
-        if isinstance(values, MutableMapping) or (isinstance(values, Collection) and not isinstance(values, str)):
-            results_id_mapped = {}
-            for k, v in results.items():
-                for result in v:
-                    results_id_mapped[result["id"]] = results_id_mapped.get(result["id"], {"id": result["id"]})
-                    results_id_mapped[result["id"]][k] = result
-            results_remapped = list(results_id_mapped.values())
-            self._merge_results_to_input(original=values, results=results_remapped, ordered=False, clear=False)
+        self._merge_results_to_input(original=values, responses=results, ordered=False, clear=False)
+        self._refresh_responses(responses=values, skip_checks=False)
 
         def map_key(value: str) -> str:
             """Map the given ``value`` to logging appropriate string"""
             return value.replace("_", " ").replace("analysis", "analyses")
 
-        url_suffix = "+".join(c[0].split("/")[-1] for c in config.values())
+        log_url = f"{self.url}/{"+".join(c[0].split("/")[-1] for c in config.values())}"
         self.logger.debug(
-            f"{'DONE':<7}: {f"{self.api_url_base}/{url_suffix}":<71} | Retrieved "
-            f"{" and ".join(map_key(k) for k in results)} for {len(id_list):>5} tracks"
+            f"{'DONE':<7}: {log_url:<71} | "
+            f"Retrieved {" and ".join(map_key(key) for _, key, _ in config.values())} for {len(id_list):>5} tracks"
         )
 
         return results
 
     def get_tracks(
             self,
-            values: APIMethodInputType,
+            values: APIInputValue,
             features: bool = False,
             analysis: bool = False,
             limit: int = 50,
             use_cache: bool = True,
             *_,
             **__,
     ) -> list[dict[str, Any]]:
         """
         ``GET: /{kind}s`` + ``GET: /audio-features`` and/or ``GET: /audio-analysis``
 
         Get track(s) info and any audio features/analysis.
-        Mostly just a wrapper for ``get_items`` and ``get_tracks_extra`` functions.
+        Mostly just a wrapper for ``get_items`` and ``extend_tracks`` functions.
 
         ``values`` may be:
             * A string representing a URL/URI/ID of type 'track'.
             * A MutableSequence of strings representing URLs/URIs/IDs of the type 'track'.
             * A remote API JSON response for a track including:
                 - some items under an ``items`` key,
                 - a valid ID value under an ``id`` key.
             * A MutableSequence of remote API JSON responses for a set of tracks including the same structure as above.
+            * A RemoteResponse of the appropriate type for this RemoteAPI which holds a valid API JSON response
+              as described above.
+            * A Sequence of RemoteResponses as above.
 
         If JSON response(s) given, this updates each response given by adding the results
         under the ``audio_features`` and ``audio_analysis`` keys as appropriate.
 
         :param values: The values representing some remote track/s. See description for allowed value types.
         :param features: When True, get audio features.
         :param analysis: When True, get audio analysis.
@@ -449,83 +486,90 @@
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         :return: API JSON responses for each item, or the original response if the input ``values`` are API responses.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``values`` are not all tracks or IDs.
         """
         tracks = self.get_items(values=values, kind=RemoteObjectType.TRACK, limit=limit, use_cache=use_cache)
 
         # ensure that response are being assigned back to the original values if API response(s) given
-        if isinstance(values, Mapping):
+        if isinstance(values, Mapping | RemoteResponse):
             tracks = [values]
-        elif isinstance(values, Collection) and all(isinstance(v, Mapping) for v in values):
+        elif isinstance(values, Collection) and all(isinstance(v, Mapping | RemoteResponse) for v in values):
             tracks = values
 
-        self.get_tracks_extra(values=tracks, features=features, analysis=analysis, limit=limit, use_cache=use_cache)
+        self.extend_tracks(values=tracks, features=features, analysis=analysis, limit=limit, use_cache=use_cache)
         return tracks
 
     def get_artist_albums(
             self,
-            values: APIMethodInputType,
+            values: APIInputValue,
             types: Collection[str] = (),
             limit: int = 50,
             use_cache: bool = True,
     ) -> dict[str, list[dict[str, Any]]]:
         """
         ``GET: /artists/{ID}/albums`` - Get all albums associated with the given artist/s.
 
         ``values`` may be:
             * A string representing a URL/URI/ID of type 'artist'.
             * A MutableSequence of strings representing URLs/URIs/IDs of the type 'artist'.
             * A remote API JSON response for an artist including a valid ID value under an ``id`` key.
             * A MutableSequence of remote API JSON responses for a set of artists including the same structure as above.
+            * A RemoteResponse of the appropriate type for this RemoteAPI which holds a valid API JSON response
+              as described above.
+            * A Sequence of RemoteResponses as above.
 
         If JSON response(s) given, this updates each response given by adding the results under the ``albums`` key.
 
+        If :py:class:`RemoteResponse` values are given, this function will call `refresh` on them.
+
         :param values: The values representing some remote artist/s. See description for allowed value types.
         :param types: The types of albums to return. Select from ``{"album", "single", "compilation", "appears_on"}``.
         :param limit: Size of batches to request.
             This value will be limited to be between ``1`` and ``50``.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         :return: A map of the Artist ID to a list of the API JSON responses for each album.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``values`` are not all artists or IDs.
         """
+        url = f"{self.url}/artists/{{id}}/albums"
+
         # input validation
-        if not values:  # skip on empty
-            self.logger.debug(f"{'SKIP':<7}: {self.api_url_base:<43} | No data given")
+        if not isinstance(values, RemoteResponse) and not values:  # skip on empty
+            self.logger.debug(f"{'SKIP':<7}: {url:<43} | No data given")
             return {}
-        valid_types = {"album", "single", "compilation", "appears_on"}
-        if types and not all(t in valid_types for t in types):
-            raise APIError(f"Given types not recognised, must be one or many of the following: {valid_types} ({types})")
-        self.validate_item_type(values, kind=RemoteObjectType.ARTIST)
 
-        id_list = self.extract_ids(values, kind=RemoteObjectType.ARTIST)
+        if types and not all(t in ARTIST_ALBUM_TYPES for t in types):
+            raise APIError(
+                f"Given types not recognised, must be one or many of the following: {ARTIST_ALBUM_TYPES} ({types})"
+            )
+        self.wrangler.validate_item_type(values, kind=RemoteObjectType.ARTIST)
+
+        id_list = self.wrangler.extract_ids(values, kind=RemoteObjectType.ARTIST)
         bar = self.logger.get_progress_bar(
             iterable=id_list, desc="Getting artist albums", unit="artist", disable=len(id_list) < self._bar_threshold
         )
 
         params = {"limit": limit_value(limit, floor=1, ceil=50)}
         if types:
             params["include_groups"] = ",".join(set(types))
 
         key = RemoteObjectType.ALBUM
-        url = self.api_url_base + "/artists/{id}/albums"
         results: dict[str, dict[str, Any]] = {}
         for id_ in bar:
             results[id_] = self.handler.get(url=url.format(id=id_), params=params, use_cache=use_cache)
             self.extend_items(results[id_], kind="artist albums", key=key, use_cache=use_cache, leave_bar=False)
 
             for album in results[id_]["items"]:  # add skeleton items block to album responses
                 album["tracks"] = {
                     "href": self.format_next_url(url=album["href"].split("?")[0] + "/tracks", offset=0, limit=50),
                     "total": album["total_tracks"]
                 }
 
-        # re-map results and extend original input if required
-        if isinstance(values, MutableMapping) or (isinstance(values, Collection) and not isinstance(values, str)):
-            results_remapped = [{"id": id_, "albums": result} for id_, result in results.items()]
-            self._merge_results_to_input(original=values, results=results_remapped, ordered=False, clear=False)
+        results_remapped = [{"id": id_, "albums": result} for id_, result in results.items()]
+        self._merge_results_to_input(original=values, responses=results_remapped, ordered=False, clear=False)
+        self._refresh_responses(responses=values, skip_checks=True)
 
         item_count = sum(len(result) for result in results.values())
         self.logger.debug(
             f"{'DONE':<7}: {url.format(id="..."):<71} | "
             f"Retrieved {item_count:>6} albums across {len(results):>5} artists"
         )
```

### Comparing `musify-0.8.1/musify/spotify/api/misc.py` & `musify-0.9.0/musify/libraries/remote/spotify/api/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 """
 Implements all required non-items and non-playlist endpoints from the Spotify API.
 """
-
 from abc import ABCMeta
 from collections.abc import MutableMapping
 from typing import Any
 
-from musify.shared.remote.enum import RemoteIDType, RemoteObjectType
-from musify.shared.types import Number
-from musify.shared.utils import limit_value
-from musify.spotify.api.base import SpotifyAPIBase
+from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
+from musify.libraries.remote.spotify.api.base import SpotifyAPIBase
+from musify.types import Number
+from musify.utils import limit_value
 
 
 class SpotifyAPIMisc(SpotifyAPIBase, metaclass=ABCMeta):
 
     def print_collection(
             self,
             value: str | MutableMapping[str, Any] | None = None,
             kind: RemoteIDType | None = None,
             limit: int = 20,
             use_cache: bool = True
     ) -> None:
         if not value:  # get user to paste in URL/URI
             value = input("\33[1mEnter URL/URI/ID: \33[0m")
         if not kind:
-            kind = self.get_item_type(value)
+            kind = self.wrangler.get_item_type(value)
         key = self.collection_item_map[kind].name.lower()
 
         while kind is None:  # get user to input ID type
             kind = RemoteObjectType.from_name(input("\33[1mEnter ID type: \33[0m"))[0]
 
-        id_ = self.extract_ids(values=value, kind=kind)[0]
-        url = self.convert(id_, kind=kind, type_in=RemoteIDType.ID, type_out=RemoteIDType.URL)
+        id_ = self.wrangler.extract_ids(values=value, kind=kind)[0]
+        url = self.wrangler.convert(id_, kind=kind, type_in=RemoteIDType.ID, type_out=RemoteIDType.URL)
         limit = limit_value(limit, floor=1, ceil=50)
 
         name = self.handler.get(url, params={"limit": limit}, log_pad=43)["name"]
         response = self.handler.get(f"{url}/{key}s", params={"limit": limit}, log_pad=43)
 
         i = 0
         while response.get("next") or i < response["total"]:  # loop through each page, printing data in blocks of 20
             if response.get("offset", 0) == 0:  # first page, show header
-                url_ext = self.convert(id_, kind=kind, type_in=RemoteIDType.ID, type_out=RemoteIDType.URL_EXT)
+                url_ext = self.wrangler.convert(id_, kind=kind, type_in=RemoteIDType.ID, type_out=RemoteIDType.URL_EXT)
                 print(
                     f"\n\t\33[96mShowing tracks for {kind.name.lower()}\33[0m: "
                     f"\33[94m{name} \33[97m- {url_ext} \33[0m\n"
                 )
 
             tracks = [item[key] if key in item else item for item in response[self.items_key]]
             for i, track in enumerate(tracks, i + 1):  # print each item in this page
@@ -63,15 +62,15 @@
     ###########################################################################
     def get_self(self, update_user_data: bool = True) -> dict[str, Any]:
         """
         ``GET: /me`` - Get API response for information on current user.
 
         :param update_user_data: When True, update the ``_user_data`` stored in this API object.
         """
-        r = self.handler.get(url=f"{self.api_url_base}/me", use_cache=True, log_pad=71)
+        r = self.handler.get(url=f"{self.url}/me", use_cache=True, log_pad=71)
         if update_user_data:
             self.user_data = r
         return r
 
     def query(
             self, query: str | None, kind: RemoteObjectType, limit: int = 10, use_cache: bool = True
     ) -> list[dict[str, Any]]:
@@ -83,15 +82,15 @@
         :param limit: Number of results to get and return.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         :return: The response from the endpoint.
         """
         if not query or len(query) > 150:  # query is too short or too long, skip
             return []
 
-        url = f"{self.api_url_base}/search"
+        url = f"{self.url}/search"
         params = {'q': query, "type": kind.name.lower(), "limit": limit_value(limit, floor=1, ceil=50)}
         response = self.handler.get(url, params=params, use_cache=use_cache)
 
         if "error" in response:
             self.logger.error(f"{'ERROR':<7}: {url:<43} | Query: {query} | {response['error']}")
             return []
```

### Comparing `musify-0.8.1/musify/spotify/api/playlist.py` & `musify-0.9.0/musify/libraries/remote/spotify/api/playlist.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 """
 Implements endpoints for manipulating playlists with the Spotify API.
 """
-
 from abc import ABCMeta
 from collections.abc import Collection, Mapping
 from itertools import batched
 from typing import Any
 
 from musify import PROGRAM_NAME, PROGRAM_URL
-from musify.shared.remote.enum import RemoteIDType, RemoteObjectType
-from musify.shared.remote.exception import RemoteIDTypeError
-from musify.shared.utils import limit_value
-from musify.spotify.api.base import SpotifyAPIBase
+from musify.libraries.remote.core import RemoteResponse
+from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
+from musify.libraries.remote.core.exception import RemoteIDTypeError
+from musify.libraries.remote.spotify.api.base import SpotifyAPIBase
+from musify.utils import limit_value
 
 
 class SpotifyAPIPlaylists(SpotifyAPIBase, metaclass=ABCMeta):
     """API endpoints for processing collections i.e. playlists, albums, shows, and audiobooks"""
 
-    def get_playlist_url(self, playlist: str | Mapping[str, Any], use_cache: bool = True) -> str:
+    def get_playlist_url(self, playlist: str | Mapping[str, Any] | RemoteResponse, use_cache: bool = True) -> str:
         """
         Determine the type of the given ``playlist`` and return its API URL.
         If type cannot be determined, attempt to find the playlist in the
         list of the currently authorised user's playlists.
 
         :param playlist: One of the following to identify the playlist URL:
             - playlist URL/URI/ID,
             - the name of the playlist in the current user's playlists,
             - the API response of a playlist.
+            - a RemoteResponse object representing a remote playlist.
         :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
         :return: The playlist URL.
         :raise RemoteIDTypeError: Raised when the function cannot determine the item type of
             the input ``playlist``. Or when it does not recognise the type of the input ``playlist`` parameter.
         """
+        if isinstance(playlist, RemoteResponse):
+            playlist = playlist.response
+
         if isinstance(playlist, Mapping):
             if "href" in playlist:
                 return playlist["href"]
             elif "id" in playlist:
-                return self.convert(
+                return self.wrangler.convert(
                     playlist["id"], kind=RemoteObjectType.PLAYLIST, type_in=RemoteIDType.ID, type_out=RemoteIDType.URL
                 )
             elif "uri" in playlist:
-                return self.convert(
+                return self.wrangler.convert(
                     playlist["uri"], kind=RemoteObjectType.PLAYLIST, type_in=RemoteIDType.URI, type_out=RemoteIDType.URL
                 )
+
         try:
-            return self.convert(playlist, kind=RemoteObjectType.PLAYLIST, type_out=RemoteIDType.URL)
+            return self.wrangler.convert(playlist, kind=RemoteObjectType.PLAYLIST, type_out=RemoteIDType.URL)
         except RemoteIDTypeError:
             playlists = self.get_user_items(kind=RemoteObjectType.PLAYLIST, use_cache=use_cache)
             playlists = {pl["name"]: pl["href"] for pl in playlists}
             if playlist not in playlists:
                 raise RemoteIDTypeError(
                     "Given playlist is not a valid URL/URI/ID and name not found in user's playlists",
                     value=playlist
@@ -63,37 +68,42 @@
         ``POST: /users/{user_id}/playlists`` - Create an empty playlist for the current user with the given name.
 
         :param name: Name of playlist to create.
         :param public: Set playlist availability as `public` if True and `private` if False.
         :param collaborative: Set playlist to collaborative i.e. other users may edit the playlist.
         :return: API URL for playlist.
         """
-        url = f"{self.api_url_base}/users/{self.user_id}/playlists"
+        url = f"{self.url}/users/{self.user_id}/playlists"
 
         body = {
             "name": name,
             "description": f"Generated using {PROGRAM_NAME}: {PROGRAM_URL}",
             "public": public,
             "collaborative": collaborative,
         }
         pl_url = self.handler.post(url, json=body, log_pad=71)["href"]
 
         self.logger.debug(f"{'DONE':<7}: {url:<71} | Created playlist: '{name}' -> {pl_url}")
         return pl_url
 
     def add_to_playlist(
-            self, playlist: str | Mapping[str, Any], items: Collection[str], limit: int = 100, skip_dupes: bool = True
+            self,
+            playlist: str | Mapping[str, Any] | RemoteResponse,
+            items: Collection[str],
+            limit: int = 100,
+            skip_dupes: bool = True
     ) -> int:
         """
         ``POST: /playlists/{playlist_id}/tracks`` - Add list of tracks to a given playlist.
 
-        :param playlist: One of the following to identify the playlist to clear:
+        :param playlist: One of the following to identify the playlist to add to:
             - playlist URL/URI/ID,
             - the name of the playlist in the current user's playlists,
             - the API response of a playlist.
+            - a RemoteResponse object representing a remote playlist.
         :param items: List of URLs/URIs/IDs of the tracks to add.
         :param limit: Size of each batch of IDs to add. This value will be limited to be between ``1`` and ``100``.
         :param skip_dupes: Skip duplicates.
         :return: The number of tracks added to the playlist.
         :raise RemoteIDTypeError: Raised when the input ``playlist`` does not represent
             a playlist URL/URI/ID.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``items``
@@ -101,17 +111,19 @@
         """
         url = f"{self.get_playlist_url(playlist, use_cache=False)}/tracks"
 
         if len(items) == 0:
             self.logger.debug(f"{'SKIP':<7}: {url:<43} | No data given")
             return 0
 
-        self.validate_item_type(items, kind=RemoteObjectType.TRACK)
+        self.wrangler.validate_item_type(items, kind=RemoteObjectType.TRACK)
 
-        uri_list = [self.convert(item, kind=RemoteObjectType.TRACK, type_out=RemoteIDType.URI) for item in items]
+        uri_list = [
+            self.wrangler.convert(item, kind=RemoteObjectType.TRACK, type_out=RemoteIDType.URI) for item in items
+        ]
         if skip_dupes:  # skip tracks currently in playlist
             pl_current = self.get_items(url, kind=RemoteObjectType.PLAYLIST, use_cache=False)[0]
             tracks_key = self.collection_item_map[RemoteObjectType.PLAYLIST].name.lower() + "s"
             tracks = pl_current[tracks_key][self.items_key]
 
             uri_current = [track["track"]["uri"] for track in tracks]
             uri_list = [uri for uri in uri_list if uri not in uri_current]
@@ -123,37 +135,45 @@
 
         self.logger.debug(f"{'DONE':<7}: {url:<71} | Added {len(uri_list):>6} items to playlist: {url}")
         return len(uri_list)
 
     ###########################################################################
     ## DELETE endpoints
     ###########################################################################
-    def delete_playlist(self, playlist: str | Mapping[str, Any]) -> str:
+    def delete_playlist(self, playlist: str | Mapping[str, Any] | RemoteResponse) -> str:
         """
         ``DELETE: /playlists/{playlist_id}/followers`` - Unfollow a given playlist.
         WARNING: This function will destructively modify your remote playlists.
 
-        :param playlist: Playlist URL/URI/ID to unfollow OR the name of the playlist in the current user's playlists.
+        :param playlist: One of the following to identify the playlist to delete:
+            - playlist URL/URI/ID,
+            - the name of the playlist in the current user's playlists,
+            - the API response of a playlist.
+            - a RemoteResponse object representing a remote playlist.
         :return: API URL for playlist.
         """
         url = f"{self.get_playlist_url(playlist, use_cache=False)}/followers"
         self.handler.delete(url, log_pad=43)
         return url
 
     def clear_from_playlist(
-            self, playlist: str | Mapping[str, Any], items: Collection[str] | None = None, limit: int = 100
+            self,
+            playlist: str | Mapping[str, Any] | RemoteResponse,
+            items: Collection[str] | None = None,
+            limit: int = 100
     ) -> int:
         """
         ``DELETE: /playlists/{playlist_id}/tracks`` - Clear tracks from a given playlist.
         WARNING: This function can destructively modify your remote playlists.
 
-        :param playlist: One of the following to identify the playlist to clear:
+        :param playlist: One of the following to identify the playlist to clear from :
             - playlist URL/URI/ID,
             - the name of the playlist in the current user's playlists,
             - the API response of a playlist.
+            - a RemoteResponse object representing a remote playlist.
         :param items: List of URLs/URIs/IDs of the tracks to remove. If None, clear all songs from the playlist.
         :param limit: Size of each batch of IDs to clear in a single request.
             This value will be limited to be between ``1`` and ``100``.
         :return: The number of tracks cleared from the playlist.
         :raise RemoteIDTypeError: Raised when the input ``playlist`` does not represent
             a playlist URL/URI/ID.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``items``
@@ -167,16 +187,18 @@
         if items is None:  # clear everything
             pl_current = self.get_items(url, kind=RemoteObjectType.PLAYLIST, extend=True, use_cache=False)[0]
 
             tracks_key = self.collection_item_map[RemoteObjectType.PLAYLIST].name.lower() + "s"
             tracks = pl_current[tracks_key][self.items_key]
             uri_list = [track[tracks_key.rstrip("s")]["uri"] for track in tracks]
         else:  # clear only the items given
-            self.validate_item_type(items, kind=RemoteObjectType.TRACK)
-            uri_list = [self.convert(item, kind=RemoteObjectType.TRACK, type_out=RemoteIDType.URI) for item in items]
+            self.wrangler.validate_item_type(items, kind=RemoteObjectType.TRACK)
+            uri_list = [
+                self.wrangler.convert(item, kind=RemoteObjectType.TRACK, type_out=RemoteIDType.URI) for item in items
+            ]
 
         if not uri_list:  # skip when nothing to clear
             self.logger.debug(f"{'SKIP':<7}: {url:<43} | No tracks to clear")
             return 0
 
         limit = limit_value(limit, floor=1, ceil=100)
         for uris in batched(uri_list, limit):  # clear in batches
```

### Comparing `musify-0.8.1/musify/spotify/processors/wrangle.py` & `musify-0.9.0/musify/libraries/remote/spotify/processors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """
 Convert and validate Spotify ID and item types.
 """
-
-from collections.abc import Mapping, Collection
+from collections.abc import Mapping
 from typing import Any
 from urllib.parse import urlparse
 
-from musify.shared.exception import MusifyEnumError
-from musify.shared.remote.api import APIMethodInputType
-from musify.shared.remote.enum import RemoteIDType, RemoteObjectType
-from musify.shared.remote.exception import RemoteError, RemoteIDTypeError, RemoteObjectTypeError
-from musify.shared.remote.processors.wrangle import RemoteDataWrangler
-from musify.spotify import URL_API, URL_EXT, SPOTIFY_UNAVAILABLE_URI, SpotifyRemote
-
-
-class SpotifyDataWrangler(RemoteDataWrangler, SpotifyRemote):
-
-    unavailable_uri_dummy = SPOTIFY_UNAVAILABLE_URI
+from musify.exception import MusifyEnumError
+from musify.libraries.core.collection import MusifyCollection
+from musify.libraries.remote.core import RemoteResponse
+from musify.libraries.remote.core.api import APIInputValue
+from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
+from musify.libraries.remote.core.exception import RemoteError, RemoteIDTypeError, RemoteObjectTypeError
+from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
+from musify.utils import to_collection
+
+
+class SpotifyDataWrangler(RemoteDataWrangler):
+
+    source = "Spotify"
+    unavailable_uri_dummy = "spotify:track:unavailable"
+    url_api = "https://api.spotify.com/v1"
+    url_ext = "https://open.spotify.com"
 
-    @staticmethod
-    def get_id_type(value: str, kind: RemoteObjectType | None = None) -> RemoteIDType:
+    @classmethod
+    def get_id_type(cls, value: str, kind: RemoteObjectType | None = None) -> RemoteIDType:
         value = value.strip().casefold()
         uri_split = value.split(':')
 
-        if value.startswith(URL_API):
+        if value.startswith(cls.url_api):
             return RemoteIDType.URL
-        elif value.startswith(URL_EXT):
+        elif value.startswith(cls.url_ext):
             return RemoteIDType.URL_EXT
         elif len(uri_split) == RemoteIDType.URI.value and uri_split[0] == "spotify":  # URI
             if uri_split[1] == "user":
                 return RemoteIDType.URI
             elif uri_split[1] != "user" and len(uri_split[2]) == RemoteIDType.ID.value:
                 return RemoteIDType.URI
         elif len(value) == RemoteIDType.ID.value or kind == RemoteObjectType.USER:
@@ -37,17 +41,17 @@
         raise RemoteIDTypeError(f"Could not determine ID type of given value: {value}")
 
     @classmethod
     def validate_id_type(cls, value: str, kind: RemoteIDType = RemoteIDType.ALL) -> bool:
         value = value.strip().casefold()
 
         if kind == RemoteIDType.URL:
-            return value.startswith(URL_API)
+            return value.startswith(cls.url_api)
         elif kind == RemoteIDType.URL_EXT:
-            return value.startswith(URL_EXT)
+            return value.startswith(cls.url_ext)
         elif kind == RemoteIDType.URI:
             uri_split = value.split(':')
             if len(uri_split) != RemoteIDType.URI.value or uri_split[0] != "spotify":
                 return False
             return uri_split[1] == "user" or (uri_split[1] != "user" and len(uri_split[2]) == RemoteIDType.ID.value)
         elif kind == RemoteIDType.ID:
             return len(value) == RemoteIDType.ID.value
@@ -55,105 +59,131 @@
             try:
                 cls.get_id_type(value)
                 return True
             except RemoteIDTypeError:
                 pass
         return False
 
-    @staticmethod
-    def _get_item_type(value: str | Mapping[str, Any], kind: RemoteObjectType) -> RemoteObjectType | None:
+    @classmethod
+    def _get_item_type(
+            cls, value: str | Mapping[str, Any] | RemoteResponse, kind: RemoteObjectType | None = None
+    ) -> RemoteObjectType | None:
+        if isinstance(value, RemoteResponse):
+            return cls._get_item_type_from_response(value)
         if isinstance(value, Mapping):
-            if value.get("is_local", False):
-                raise RemoteObjectTypeError("Cannot process local items")
-            if "type" not in value:
-                raise RemoteObjectTypeError(f"Given map does not contain a 'type' key: {value}")
-            return RemoteObjectType.from_name(value["type"].casefold().rstrip('s'))[0]
+            return cls._get_item_type_from_mapping(value)
 
         value = value.strip()
         uri_check = value.split(':')
 
-        if value.startswith(URL_API) or value.startswith(URL_EXT):  # open/API URL
-            value = value.removeprefix(URL_API) if value.startswith(URL_API) else value.removeprefix(URL_EXT)
+        if value.startswith(cls.url_api) or value.startswith(cls.url_ext):  # open/API URL
+            value = value.removeprefix(cls.url_api if value.startswith(cls.url_api) else cls.url_ext)
             url_path = urlparse(value).path.split("/")
             for chunk in url_path:
                 try:
                     return RemoteObjectType.from_name(chunk.casefold().rstrip('s'))[0]
                 except MusifyEnumError:
                     continue
         elif len(uri_check) == RemoteIDType.URI.value and uri_check[0].casefold() == "spotify":
             return RemoteObjectType.from_name(uri_check[1])[0]
         elif len(value) == RemoteIDType.ID.value or kind == RemoteObjectType.USER:
+            # in these cases, we have to go on faith...
             return kind
         raise RemoteObjectTypeError(f"Could not determine item type of given value: {value}")
 
     @classmethod
+    def _get_item_type_from_response(cls, value: RemoteResponse) -> RemoteObjectType:
+        response_kind = cls._get_item_type_from_mapping(value.response)
+        if value.kind != response_kind:
+            raise RemoteObjectTypeError(
+                f"RemoteResponse kind != actual response kind: {value.kind} != {response_kind}"
+            )
+        return value.kind
+
+    @classmethod
+    def _get_item_type_from_mapping(cls, value: Mapping[str, Any]) -> RemoteObjectType:
+        if value.get("is_local", False):
+            raise RemoteObjectTypeError("Cannot process local items")
+        if "type" not in value:
+            raise RemoteObjectTypeError(f"Given map does not contain a 'type' key: {value}")
+        return RemoteObjectType.from_name(value["type"].casefold().rstrip('s'))[0]
+
+    @classmethod
     def convert(
             cls,
             value: str,
             kind: RemoteObjectType | None = None,
             type_in: RemoteIDType = RemoteIDType.ALL,
             type_out: RemoteIDType = RemoteIDType.ID
     ) -> str:
         if cls.validate_id_type(value, kind=type_out):
             return value
         if type_in == RemoteIDType.ALL or not cls.validate_id_type(value, kind=type_in):
             type_in = cls.get_id_type(value, kind=kind)
 
         value = value.strip()
 
-        if type_in == RemoteIDType.URL_EXT or type_in == RemoteIDType.URL:  # open/API URL
-            url_path = urlparse(value).path.split("/")
-            for chunk in url_path:
-                try:
-                    kind = RemoteObjectType.from_name(chunk.rstrip('s'))[0]
-                    break
-                except MusifyEnumError:
-                    continue
-
-            if kind == RemoteObjectType.USER:
-                name = kind.name.lower()
-                try:
-                    id_ = url_path[url_path.index(name) + 1]
-                except ValueError:
-                    id_ = url_path[url_path.index(name + "s") + 1]
-            else:
-                id_ = next(p for p in url_path if len(p) == RemoteIDType.ID.value)
-
+        if type_in == RemoteIDType.URL_EXT or type_in == RemoteIDType.URL:
+            kind, id_ = cls._get_id_from_url(value=value, kind=kind)
         elif type_in == RemoteIDType.URI:
-            uri_split = value.split(':')
-            kind = RemoteObjectType.from_name(uri_split[1])[0]
-            id_ = uri_split[2]
-
+            kind, id_ = cls._get_id_from_uri(value=value)
         elif type_in == RemoteIDType.ID:
             if kind is None:
                 raise RemoteIDTypeError("Input value is an ID and no defined 'kind' has been given.", RemoteIDType.ID)
             id_ = value
-
         else:
             raise RemoteIDTypeError(f"Could not determine item type: {value}")
 
         # reformat
         item = kind.name.lower().rstrip('s')
         if type_out == RemoteIDType.URL:
-            return f'{URL_API}/{item}s/{id_}'
+            return f'{cls.url_api}/{item}s/{id_}'
         elif type_out == RemoteIDType.URL_EXT:
-            return f'{URL_EXT}/{item}/{id_}'
+            return f'{cls.url_ext}/{item}/{id_}'
         elif type_out == RemoteIDType.URI:
             return f"spotify:{item}:{id_}"
         else:
             return id_
 
     @classmethod
-    def extract_ids(cls, values: APIMethodInputType, kind: RemoteObjectType | None = None) -> list[str]:
-        if isinstance(values, str):
-            return [cls.convert(values, kind=kind, type_out=RemoteIDType.ID)]
-        elif isinstance(values, Mapping) and "id" in values:  # is a raw API response from Spotify
-            return [values["id"]]
-        elif isinstance(values, Collection):
-            if len(values) == 0:
-                return []
-            elif all(isinstance(d, str) for d in values):
-                return [cls.convert(d, kind=kind, type_out=RemoteIDType.ID) for d in values]
-            elif all(isinstance(d, Mapping) and "id" in d for d in values):
-                return [track["id"] for track in values]
+    def _get_id_from_url(cls, value: str, kind: RemoteObjectType | None = None) -> tuple[RemoteObjectType, str]:
+        url_path = urlparse(value).path.split("/")
+        for chunk in url_path:
+            try:
+                kind = RemoteObjectType.from_name(chunk.rstrip('s'))[0]
+                break
+            except MusifyEnumError:
+                continue
+
+        if kind == RemoteObjectType.USER:
+            name = kind.name.lower()
+            try:
+                id_ = url_path[url_path.index(name) + 1]
+            except ValueError:
+                id_ = url_path[url_path.index(name + "s") + 1]
+        else:
+            id_ = next(p for p in url_path if len(p) == RemoteIDType.ID.value)
+
+        return kind, id_
+
+    @classmethod
+    def _get_id_from_uri(cls, value: str) -> tuple[RemoteObjectType, str]:
+        uri_split = value.split(':')
+        kind = RemoteObjectType.from_name(uri_split[1])[0]
+        id_ = uri_split[2]
+        return kind, id_
+
+    @classmethod
+    def extract_ids(cls, values: APIInputValue, kind: RemoteObjectType | None = None) -> list[str]:
+        def extract_id(value: str | Mapping[str, Any] | RemoteResponse) -> str:
+            """Extract an ID from a given ``value``"""
+            if isinstance(value, str):
+                return cls.convert(value, kind=kind, type_out=RemoteIDType.ID)
+            elif isinstance(value, Mapping) and "id" in value:
+                return value["id"]
+            elif isinstance(value, RemoteResponse):
+                return value.id
+
+            raise RemoteError(f"Could not extract ID. Input data not recognised: {type(value)}")
 
-        raise RemoteError(f"Could not extract IDs. Input data not recognised: {type(values)}")
+        values = to_collection(values) if not isinstance(values, MusifyCollection) else [values]
+        return [extract_id(value=value) for value in to_collection(values)]
```

### Comparing `musify-0.8.1/.gitignore` & `musify-0.9.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -64,25 +64,21 @@
 # Flask stuff:
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
-# Sphinx/other documentation
-docs/_build/
-docs/musify*.rst
-.grip/
-
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 jupyter/
+notebooks/
 .ipynb_checkpoints
 
 # IPython
 profile_default/
 ipython_config.py
 
 # pdm
@@ -138,7 +134,19 @@
 # binary/cache files
 **.sql*
 **cache*
 
 # large data & log folders
 _data/
 _logs/
+
+# Sphinx/other documentation
+docs/_build/
+docs/musify*.rst
+.grip/
+
+# Jekyll
+_site
+.sass-cache
+.jekyll-cache
+.jekyll-metadata
+vendor
```

### Comparing `musify-0.8.1/LICENSE` & `musify-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `musify-0.8.1/README.md` & `musify-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [![Documentation](https://img.shields.io/badge/Documentation-red.svg)](https://geo-martino.github.io/musify/)
 </br>
 [![PyPI Downloads](https://img.shields.io/pypi/dm/musify?label=Downloads)](https://pypi.org/project/musify/)
 [![Code Size](https://img.shields.io/github/languages/code-size/geo-martino/musify?label=Code%20Size)](https://github.com/geo-martino/musify)
 [![Contributors](https://img.shields.io/github/contributors/geo-martino/musify?logo=github&label=Contributors)](https://github.com/geo-martino/musify/graphs/contributors)
 [![License](https://img.shields.io/github/license/geo-martino/musify?label=License)](https://github.com/geo-martino/musify/blob/master/LICENSE)
 </br>
+[![GitHub - Validate](https://github.com/geo-martino/musify/actions/workflows/validate.yml/badge.svg?branch=master)](https://github.com/geo-martino/musify/actions/workflows/validate.yml)
 [![GitHub - Deployment](https://github.com/geo-martino/musify/actions/workflows/deploy.yml/badge.svg?event=release)](https://github.com/geo-martino/musify/actions/workflows/deploy.yml)
 [![GitHub - Documentation](https://github.com/geo-martino/musify/actions/workflows/docs_publish.yml/badge.svg)](https://github.com/geo-martino/musify/actions/workflows/docs_publish.yml)
 
 ### A Swiss Army knife for music library management
 Supporting local and music streaming service (remote) libraries.
 - Extract data for all item types from remote libraries, including following/saved items, such as:
 **playlists, tracks, albums, artists, users, podcasts, audiobooks**
@@ -29,15 +30,15 @@
   * [Local](#local)
 * [Currently Supported](#currently-supported)
 * [Release History](#release-history)
 * [Contributing](#contributing)
 * [Motivation & Aims](#aims)
 * [Author Notes](#notes)
 
-> [!NOTE]  
+> **NOTE:**  
 > This readme provides a brief overview of the program. 
 > [Read the docs](https://geo-martino.github.io/musify/) for full reference documentation.
 
 
 ## Installation
 Install through pip using one of the following commands:
 
@@ -49,20 +50,21 @@
 ```
 
 ## Quick Guides
 
 These quick guides will help you get set up and going with Musify in just a few minutes.
 For more detailed guides, check out the [documentation](https://geo-martino.github.io/musify/).
 
-> [!TIP]
+> **TIP:**
 > Set up logging to ensure you can see all info reported by the later operations.
 > Libraries log info about loaded objects to the custom `STAT` level.
 > ```python
 > import logging
-> from musify.shared.logger import STAT
+> from musify.log import STAT
+> 
 > logging.basicConfig(format="%(message)s", level=STAT)
 > ```
 
 ### Spotify
 
 > In this example, you will: 
 > - Authorise access to the [Spotify Web API](https://developer.spotify.com/documentation/web-api)
@@ -75,15 +77,15 @@
    Select "Web API" when asked which APIs you are planning on using. 
    To use this program, you will only need to take note of the **client ID** and **client secret**.
 3. Create a `SpotifyAPI` object and authorise the program access to Spotify data as follows:
    
    > The scopes listed in this example will allow access to read your library data and write to your playlists.
    > See Spotify Web API documentation for more information about [scopes](https://developer.spotify.com/documentation/web-api/concepts/scopes)
    ```python
-   from musify.spotify.api import SpotifyAPI
+   from musify.libraries.remote.spotify.api import SpotifyAPI
    
    api = SpotifyAPI(
        client_id="<YOUR CLIENT ID>",
        client_secret="<YOUR CLIENT SECRET>",
        scopes=[
            "user-library-read",
            "user-follow-read",
@@ -98,15 +100,15 @@
    )
    
    # authorise the program to access your Spotify data in your web browser
    api.authorise()
    ```
 4. Create a `SpotifyLibrary` object and load your library data as follows:
    ```python
-   from musify.spotify.library import SpotifyLibrary
+   from musify.libraries.remote.spotify.library import SpotifyLibrary
    
    library = SpotifyLibrary(api=api)
    
    # if you have a very large library, this will take some time...
    library.load()
    
    # ...or you may also just load distinct sections of your library
@@ -128,15 +130,15 @@
    library.log_artists()
    
    # pretty print an overview of your library
    print(library)
    ```
 5. Load some Spotify objects using any of the supported identifiers as follows:
    ```python
-   from musify.spotify.object import SpotifyTrack, SpotifyAlbum, SpotifyPlaylist, SpotifyArtist
+   from musify.libraries.remote.spotify.object import SpotifyTrack, SpotifyAlbum, SpotifyPlaylist, SpotifyArtist
    
    # load by ID
    track1 = SpotifyTrack.load("6fWoFduMpBem73DMLCOh1Z", api=api)
    # load by URI
    track2 = SpotifyTrack.load("spotify:track:4npv0xZO9fVLBmDS2XP9Bw", api=api)
    # load by open/external style URL
    track3 = SpotifyTrack.load("https://open.spotify.com/track/1TjVbzJUAuOvas1bL00TiH", api=api)
@@ -176,25 +178,25 @@
 > - Modify the tags of some local tracks and save them
 > - Modify a local playlist and save it
 
 1. Create one of the following supported `LocalLibrary` objects:
 
    #### Generic local library
    ```python
-   from musify.local.library import LocalLibrary
+   from musify.libraries.local.library import LocalLibrary
    
    library = LocalLibrary(
        library_folders=["<PATH TO YOUR LIBRARY FOLDER>", ...],
        playlist_folder="<PATH TO YOUR PLAYLIST FOLDER",
    )
    ```
    
    #### MusicBee
    ```python
-   from musify.local.library import MusicBee
+   from musify.libraries.local.library import MusicBee
    
    library = MusicBee(musicbee_folder="<PATH TO YOUR MUSICBEE FOLDER>")
    ```
 
 2. Load your library:
    ```python
    # if you have a very large library, this will take some time...
@@ -223,15 +225,16 @@
    # pretty print information about the loaded objects
    print(playlist, album, artist, folder, genre, sep="\n")
    ```
 
 4. Get a track from your library using any of the following identifiers:
    ```python
    # get a track via its title
-   track = library["<TRACK TITLE>"]  # if multiple tracks have the same title, the first matching one if returned
+   # if multiple tracks have the same title, the first matching one if returned
+   track = library["<TRACK TITLE>"]
    
    # get a track via its path
    track = library["<PATH TO YOUR TRACK>"]  # must be an absolute path
    
    # get a track according to a specific tag
    track = next(track for track in library if track.artist == "<ARTIST NAME>")
    track = next(track for track in library if "<GENRE>" in (track.genres or []))
@@ -260,15 +263,15 @@
    
    # see the updated information
    print(track)
    ```
 
 6. Save the tags to the file:
    ```python
-   from musify.local.track.field import LocalTrackField
+   from musify.libraries.local.track.field import LocalTrackField
    
    # you don't have to save all the tags you just modified
    # select which you wish to save first like so
    tags = [
         LocalTrackField.TITLE,
         LocalTrackField.GENRES,
         LocalTrackField.KEY,
@@ -334,15 +337,15 @@
 **With this functionality, user's should then have the freedom to**:
 
 - Switch between music streaming services with a few simple commands
 - Share local playlists and other local library data with friends over music streaming services 
 without ever having to use them personally
 - Easily maintain a high-quality local library with complete metadata
 
-**User's should have the freedom to choose how and where they want to listen to their favourite artists.**
+**Users should have the freedom to choose how and where they want to listen to their favourite artists.**
 
 Given the near non-existence of income these services provide to artists, user's should have the choice to 
 compensate their favourite artists fairly for their work, choosing to switch to other services that do and/or choosing 
 not to use music streaming services altogether because of this. Hopefully, by reintroducing this choice to users, 
 the music industry will be forced to re-evaluate their complete devaluing of creative work in the rush to chase profits, 
 and instead return to a culture of nurturing talent by providing artists with a basic income to survive 
 on the work of their craft. One can dream.
```

### Comparing `musify-0.8.1/pyproject.toml` & `musify-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling", "hatch-vcs"]
+requires = ["hatchling", "versioningit"]
 build-backend = "hatchling.build"
 
 [project]
 dynamic = ["version"]
 name = "musify"
 authors = [
   { name="George Martin Marino", email="gm.engineer+musify@pm.me" },
@@ -14,40 +14,41 @@
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
 ]
 dependencies = [
     "mutagen~=1.47",
-    "pyyaml~=6.0",
     "requests~=2.31",
     "requests-cache~=1.1",
     "Pillow~=10.1",
     "python-dateutil>=2.8.2,<2.10.0",
     "xmltodict~=0.13",
     "lxml~=5.1",
     "tqdm~=4.66",
 ]
 
 [project.optional-dependencies]
 build = [
     "hatch",
-    "hatch-vcs",
+    "versioningit",
 ]
 test = [
     "pytest~=8.0",
+    "pytest-xdist~=3.5",
     "pytest-mock~=3.12",
     "requests-mock~=1.11",
+    "pyyaml~=6.0",
     "pycountry~=23.12",
 ]
 docs = [
     "musify[build]",
     "sphinx~=7.2",
     "renku_sphinx_theme",
     "graphviz~=0.20",
@@ -65,16 +66,23 @@
 "Documentation" = "https://geo-martino.github.io/musify/"
 "Release Notes" = "https://geo-martino.github.io/musify/release-history.html"
 "Contribute" = "https://geo-martino.github.io/musify/contributing.html"
 "Source code" = "https://github.com/geo-martino/musify"
 Issues = "https://github.com/geo-martino/musify/issues"
 
 [tool.hatch.version]
-source = "vcs"
-fallback-version = "0.0.0"
+source = "versioningit"
+
+[tool.versioningit.format]
+# WORKAROUND: commits for actual production releases keep getting identified as dirty and/or with distance
+#  Delete this config when fixed. It should be the commented lines below each (i.e. the default formats)
+dirty = "{base_version}"
+#dirty = "{base_version}+d{build_date:%Y%m%d}"
+distance-dirty = "{base_version}"
+#distance-dirty = "{next_version}.dev{distance}+{vcs}{rev}.d{build_date:%Y%m%d}"
 
 [tool.hatch.build.targets.sdist]
 include = ["musify"]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 testpaths = ["tests"]
```

### Comparing `musify-0.8.1/PKG-INFO` & `musify-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: musify
-Version: 0.8.1
+Version: 0.9.0
 Summary: Synchronise your music library to local or remote libraries
 Project-URL: Documentation, https://geo-martino.github.io/musify/
 Project-URL: Release Notes, https://geo-martino.github.io/musify/release-history.html
 Project-URL: Contribute, https://geo-martino.github.io/musify/contributing.html
 Project-URL: Source code, https://github.com/geo-martino/musify
 Project-URL: Issues, https://github.com/geo-martino/musify/issues
 Author-email: George Martin Marino <gm.engineer+musify@pm.me>
 License-File: LICENSE
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Requires-Dist: lxml~=5.1
 Requires-Dist: mutagen~=1.47
 Requires-Dist: pillow~=10.1
 Requires-Dist: python-dateutil<2.10.0,>=2.8.2
-Requires-Dist: pyyaml~=6.0
 Requires-Dist: requests-cache~=1.1
 Requires-Dist: requests~=2.31
 Requires-Dist: tqdm~=4.66
 Requires-Dist: xmltodict~=0.13
 Provides-Extra: build
 Requires-Dist: hatch; extra == 'build'
-Requires-Dist: hatch-vcs; extra == 'build'
+Requires-Dist: versioningit; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: grip~=4.6; extra == 'dev'
 Requires-Dist: musify[build,docs,test]; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm~=0.2; extra == 'docs'
 Requires-Dist: graphviz~=0.20; extra == 'docs'
@@ -42,29 +41,32 @@
 Requires-Dist: renku-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints<3.0,>=1.25; extra == 'docs'
 Requires-Dist: sphinxext-opengraph~=0.9; extra == 'docs'
 Requires-Dist: sphinx~=7.2; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pycountry~=23.12; extra == 'test'
 Requires-Dist: pytest-mock~=3.12; extra == 'test'
+Requires-Dist: pytest-xdist~=3.5; extra == 'test'
 Requires-Dist: pytest~=8.0; extra == 'test'
+Requires-Dist: pyyaml~=6.0; extra == 'test'
 Requires-Dist: requests-mock~=1.11; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Musify
 
 [![PyPI Version](https://img.shields.io/pypi/v/musify?logo=pypi&label=Latest%20Version)](https://pypi.org/project/musify)
 [![Python Version](https://img.shields.io/pypi/pyversions/musify.svg?logo=python&label=Supported%20Python%20Versions)](https://pypi.org/project/musify/)
 [![Documentation](https://img.shields.io/badge/Documentation-red.svg)](https://geo-martino.github.io/musify/)
 </br>
 [![PyPI Downloads](https://img.shields.io/pypi/dm/musify?label=Downloads)](https://pypi.org/project/musify/)
 [![Code Size](https://img.shields.io/github/languages/code-size/geo-martino/musify?label=Code%20Size)](https://github.com/geo-martino/musify)
 [![Contributors](https://img.shields.io/github/contributors/geo-martino/musify?logo=github&label=Contributors)](https://github.com/geo-martino/musify/graphs/contributors)
 [![License](https://img.shields.io/github/license/geo-martino/musify?label=License)](https://github.com/geo-martino/musify/blob/master/LICENSE)
 </br>
+[![GitHub - Validate](https://github.com/geo-martino/musify/actions/workflows/validate.yml/badge.svg?branch=master)](https://github.com/geo-martino/musify/actions/workflows/validate.yml)
 [![GitHub - Deployment](https://github.com/geo-martino/musify/actions/workflows/deploy.yml/badge.svg?event=release)](https://github.com/geo-martino/musify/actions/workflows/deploy.yml)
 [![GitHub - Documentation](https://github.com/geo-martino/musify/actions/workflows/docs_publish.yml/badge.svg)](https://github.com/geo-martino/musify/actions/workflows/docs_publish.yml)
 
 ### A Swiss Army knife for music library management
 Supporting local and music streaming service (remote) libraries.
 - Extract data for all item types from remote libraries, including following/saved items, such as:
 **playlists, tracks, albums, artists, users, podcasts, audiobooks**
@@ -81,15 +83,15 @@
   * [Local](#local)
 * [Currently Supported](#currently-supported)
 * [Release History](#release-history)
 * [Contributing](#contributing)
 * [Motivation & Aims](#aims)
 * [Author Notes](#notes)
 
-> [!NOTE]  
+> **NOTE:**  
 > This readme provides a brief overview of the program. 
 > [Read the docs](https://geo-martino.github.io/musify/) for full reference documentation.
 
 
 ## Installation
 Install through pip using one of the following commands:
 
@@ -101,20 +103,21 @@
 ```
 
 ## Quick Guides
 
 These quick guides will help you get set up and going with Musify in just a few minutes.
 For more detailed guides, check out the [documentation](https://geo-martino.github.io/musify/).
 
-> [!TIP]
+> **TIP:**
 > Set up logging to ensure you can see all info reported by the later operations.
 > Libraries log info about loaded objects to the custom `STAT` level.
 > ```python
 > import logging
-> from musify.shared.logger import STAT
+> from musify.log import STAT
+> 
 > logging.basicConfig(format="%(message)s", level=STAT)
 > ```
 
 ### Spotify
 
 > In this example, you will: 
 > - Authorise access to the [Spotify Web API](https://developer.spotify.com/documentation/web-api)
@@ -127,15 +130,15 @@
    Select "Web API" when asked which APIs you are planning on using. 
    To use this program, you will only need to take note of the **client ID** and **client secret**.
 3. Create a `SpotifyAPI` object and authorise the program access to Spotify data as follows:
    
    > The scopes listed in this example will allow access to read your library data and write to your playlists.
    > See Spotify Web API documentation for more information about [scopes](https://developer.spotify.com/documentation/web-api/concepts/scopes)
    ```python
-   from musify.spotify.api import SpotifyAPI
+   from musify.libraries.remote.spotify.api import SpotifyAPI
    
    api = SpotifyAPI(
        client_id="<YOUR CLIENT ID>",
        client_secret="<YOUR CLIENT SECRET>",
        scopes=[
            "user-library-read",
            "user-follow-read",
@@ -150,15 +153,15 @@
    )
    
    # authorise the program to access your Spotify data in your web browser
    api.authorise()
    ```
 4. Create a `SpotifyLibrary` object and load your library data as follows:
    ```python
-   from musify.spotify.library import SpotifyLibrary
+   from musify.libraries.remote.spotify.library import SpotifyLibrary
    
    library = SpotifyLibrary(api=api)
    
    # if you have a very large library, this will take some time...
    library.load()
    
    # ...or you may also just load distinct sections of your library
@@ -180,15 +183,15 @@
    library.log_artists()
    
    # pretty print an overview of your library
    print(library)
    ```
 5. Load some Spotify objects using any of the supported identifiers as follows:
    ```python
-   from musify.spotify.object import SpotifyTrack, SpotifyAlbum, SpotifyPlaylist, SpotifyArtist
+   from musify.libraries.remote.spotify.object import SpotifyTrack, SpotifyAlbum, SpotifyPlaylist, SpotifyArtist
    
    # load by ID
    track1 = SpotifyTrack.load("6fWoFduMpBem73DMLCOh1Z", api=api)
    # load by URI
    track2 = SpotifyTrack.load("spotify:track:4npv0xZO9fVLBmDS2XP9Bw", api=api)
    # load by open/external style URL
    track3 = SpotifyTrack.load("https://open.spotify.com/track/1TjVbzJUAuOvas1bL00TiH", api=api)
@@ -228,25 +231,25 @@
 > - Modify the tags of some local tracks and save them
 > - Modify a local playlist and save it
 
 1. Create one of the following supported `LocalLibrary` objects:
 
    #### Generic local library
    ```python
-   from musify.local.library import LocalLibrary
+   from musify.libraries.local.library import LocalLibrary
    
    library = LocalLibrary(
        library_folders=["<PATH TO YOUR LIBRARY FOLDER>", ...],
        playlist_folder="<PATH TO YOUR PLAYLIST FOLDER",
    )
    ```
    
    #### MusicBee
    ```python
-   from musify.local.library import MusicBee
+   from musify.libraries.local.library import MusicBee
    
    library = MusicBee(musicbee_folder="<PATH TO YOUR MUSICBEE FOLDER>")
    ```
 
 2. Load your library:
    ```python
    # if you have a very large library, this will take some time...
@@ -275,15 +278,16 @@
    # pretty print information about the loaded objects
    print(playlist, album, artist, folder, genre, sep="\n")
    ```
 
 4. Get a track from your library using any of the following identifiers:
    ```python
    # get a track via its title
-   track = library["<TRACK TITLE>"]  # if multiple tracks have the same title, the first matching one if returned
+   # if multiple tracks have the same title, the first matching one if returned
+   track = library["<TRACK TITLE>"]
    
    # get a track via its path
    track = library["<PATH TO YOUR TRACK>"]  # must be an absolute path
    
    # get a track according to a specific tag
    track = next(track for track in library if track.artist == "<ARTIST NAME>")
    track = next(track for track in library if "<GENRE>" in (track.genres or []))
@@ -312,15 +316,15 @@
    
    # see the updated information
    print(track)
    ```
 
 6. Save the tags to the file:
    ```python
-   from musify.local.track.field import LocalTrackField
+   from musify.libraries.local.track.field import LocalTrackField
    
    # you don't have to save all the tags you just modified
    # select which you wish to save first like so
    tags = [
         LocalTrackField.TITLE,
         LocalTrackField.GENRES,
         LocalTrackField.KEY,
@@ -386,15 +390,15 @@
 **With this functionality, user's should then have the freedom to**:
 
 - Switch between music streaming services with a few simple commands
 - Share local playlists and other local library data with friends over music streaming services 
 without ever having to use them personally
 - Easily maintain a high-quality local library with complete metadata
 
-**User's should have the freedom to choose how and where they want to listen to their favourite artists.**
+**Users should have the freedom to choose how and where they want to listen to their favourite artists.**
 
 Given the near non-existence of income these services provide to artists, user's should have the choice to 
 compensate their favourite artists fairly for their work, choosing to switch to other services that do and/or choosing 
 not to use music streaming services altogether because of this. Hopefully, by reintroducing this choice to users, 
 the music industry will be forced to re-evaluate their complete devaluing of creative work in the rush to chase profits, 
 and instead return to a culture of nurturing talent by providing artists with a basic income to survive 
 on the work of their craft. One can dream.
```

