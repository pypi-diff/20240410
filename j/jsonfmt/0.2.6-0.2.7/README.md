# Comparing `tmp/jsonfmt-0.2.6.tar.gz` & `tmp/jsonfmt-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.2.6.tar", last modified: Tue Jun 13 09:59:35 2023, max compression
+gzip compressed data, was "jsonfmt-0.2.7.tar", last modified: Wed Apr 10 07:18:46 2024, max compression
```

## Comparing `jsonfmt-0.2.6.tar` & `jsonfmt-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/jsonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    12198 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/jsonfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:18:46.403048 jsonfmt-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-04-10 07:18:46.403048 jsonfmt-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24214 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:18:46.399048 jsonfmt-0.2.7/jsonfmt/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/jsonfmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/jsonfmt/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14145 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/jsonfmt/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/jsonfmt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/jsonfmt/xml2py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:18:46.403048 jsonfmt-0.2.7/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-04-10 07:18:46.000000 jsonfmt-0.2.7/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-10 07:18:46.000000 jsonfmt-0.2.7/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:18:46.000000 jsonfmt-0.2.7/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 07:18:46.000000 jsonfmt-0.2.7/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 07:18:46.000000 jsonfmt-0.2.7/jsonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 07:18:46.000000 jsonfmt-0.2.7/jsonfmt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:18:46.403048 jsonfmt-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:18:46.403048 jsonfmt-0.2.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/test/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/test/test_jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-10 07:18:37.000000 jsonfmt-0.2.7/test/test_xml2py.py
```

### Comparing `jsonfmt-0.2.6/LICENSE` & `jsonfmt-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.2.6/jsonfmt.py` & `jsonfmt-0.2.7/jsonfmt/jsonfmt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,73 @@
 #!/usr/bin/env python
 '''JSON Formatter'''
 
+import io
 import json
-import re
-import toml
-import yaml
+import os
+import sys
 from argparse import ArgumentParser
 from functools import partial
-from io import TextIOBase
 from pydoc import pager
 from shutil import get_terminal_size
-from sys import stdin, stdout, stderr, exit as sys_exit
-from typing import Any, List, IO, Optional, Sequence, Tuple, Union
+from tempfile import NamedTemporaryFile, _TemporaryFileWrapper
+from typing import IO, Any, Callable, List, Optional, Tuple, Union
 from unittest.mock import patch
 
 import pyperclip
-from jmespath import compile as jcompile
+import toml
+import yaml
+from jmespath import compile as parse_jmespath
 from jmespath.exceptions import JMESPathError
 from jmespath.parser import ParsedResult as JMESPath
 from jsonpath_ng import JSONPath
-from jsonpath_ng import parse as jparse
+from jsonpath_ng import parse as parse_jsonpath
 from jsonpath_ng.exceptions import JSONPathError
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
-from pygments.lexers import JsonLexer, TOMLLexer, YamlLexer
-
-__version__ = '0.2.6'
+from pygments.lexers import JsonLexer, TOMLLexer, XmlLexer, YamlLexer
 
-NUMERIC = re.compile(r'-?\d+$|-?\d+\.\d+$|^-?\d+\.?\d+e-?\d+$')
-DICT_OR_LIST = re.compile(r'^\{.*\}$|^\[.*\]$')
+from . import __version__, utils, xml2py
+from .diff import compare
 
 QueryPath = Union[JMESPath, JSONPath]
-
-
-def print_inf(msg: Any):
-    print(f'\033[1;94mjsonfmt:\033[0m \033[0;94m{msg}\033[0m', file=stderr)
-
-
-def print_err(msg: Any):
-    print(f'\033[1;91mjsonfmt:\033[0m \033[0;91m{msg}\033[0m', file=stderr)
+TEMP_CLIPBOARD = io.StringIO()
 
 
 class FormatError(Exception):
     pass
 
 
 def is_clipboard_available() -> bool:
     '''check if the clipboard available'''
     copy_fn, paste_fn = pyperclip.determine_clipboard()
     return copy_fn.__class__.__name__ != 'ClipboardUnavailable' \
         and paste_fn.__class__.__name__ != 'ClipboardUnavailable'
 
 
+def parse_querypath(querypath: Optional[str], querylang: Optional[str]):
+    '''parse the querypath'''
+    if querypath is None:
+        return None
+    elif querylang is None:
+        parsers = [parse_jmespath, parse_jsonpath]
+    elif querylang in ['jmespath', 'jsonpath']:
+        parsers = [{'jmespath': parse_jmespath, 'jsonpath': parse_jsonpath}[querylang]]
+    else:
+        utils.exit_with_error(f'invalid querylang: "{querylang}"')
+
+    for parse in parsers:
+        try:
+            return parse(querypath)
+        except (JMESPathError, JSONPathError, AttributeError):
+            pass
+
+    utils.exit_with_error(f'invalid querypath expression: "{querypath}"')
+
+
 def extract_elements(qpath: QueryPath, py_obj: Any) -> Any:
     '''find and extract elements via JMESPath or JSONPath'''
     if isinstance(qpath, JMESPath):
         return qpath.search(py_obj)
     else:
         items = [matched.value for matched in qpath.find(py_obj)]
         n_items = len(items)
@@ -66,29 +78,30 @@
         else:
             return items
 
 
 def parse_to_pyobj(text: str, qpath: Optional[QueryPath]) -> Tuple[Any, str]:
     '''read json, toml or yaml from IO and then match sub-element by jmespath'''
     # parse json, toml or yaml to python object
-    loads_methods = {
-        'json': json.loads,
-        'toml': toml.loads,
-        'yaml': partial(yaml.load, Loader=yaml.Loader),
-    }
+    loads_methods: list[tuple[str, Callable]] = [
+        ('json', json.loads),
+        ('toml', toml.loads),
+        ('xml', xml2py.loads),
+        ('yaml', partial(yaml.load, Loader=yaml.Loader)),
+    ]
 
     # try to load the text to be parsed
-    for fmt, fn_loads in loads_methods.items():
+    for fmt, fn_loads in loads_methods:
         try:
             py_obj = fn_loads(text)
             break
         except Exception:
             continue
     else:
-        raise FormatError("no json, toml or yaml found in the text")
+        raise FormatError("no supported format found")
 
     if qpath is None:
         return py_obj, fmt
     else:
         # match sub-elements via jmespath or jsonpath
         return extract_elements(qpath, py_obj), fmt
 
@@ -100,55 +113,44 @@
         return int(key) if isinstance(obj, list) else key
 
     # make sure the keys joined by `.`, and then split
     _keys = keys.replace(']', '').replace('[', '.').split('.')
 
     for k in _keys[:-1]:
         py_obj = py_obj[key_or_idx(py_obj, k)]
-    else:
-        return py_obj, key_or_idx(py_obj, _keys[-1])
 
-
-def load_value(value: str):
-    if NUMERIC.match(value):
-        return eval(value)
-    elif DICT_OR_LIST.match(value):
-        try:
-            return eval(value)
-        except Exception:
-            return value
-    else:
-        return value
+    return py_obj, key_or_idx(py_obj, _keys[-1])
 
 
 def modify_pyobj(py_obj: Any, sets: List[str], pops: List[str]):
     '''add, modify or pop items for PyObj'''
     for kv in sets:
         try:
             keys, value = kv.split('=')
             bottom, last_k = traverse_to_bottom(py_obj, keys)
             if isinstance(bottom, list) and len(bottom) <= last_k:  # type: ignore
-                bottom.append(load_value(value))
+                bottom.append(utils.safe_eval(value))
             else:
-                bottom[last_k] = load_value(value)  # type: ignore
+                bottom[last_k] = utils.safe_eval(value)  # type: ignore
         except (IndexError, KeyError, ValueError, TypeError):
-            print_err(f'invalid key path: {kv}')
+            utils.print_err(f'invalid key path: {kv}')
             continue
 
     for keys in pops:
         try:
             bottom, last_k = traverse_to_bottom(py_obj, keys)
             bottom.pop(last_k)
         except (IndexError, KeyError):
-            print_err(f'invalid key path: {keys}')
+            utils.print_err(f'invalid key path: {keys}')
             continue
 
 
-def get_overview(py_obj: Any):
-    def clip(value: Any):
+def get_overview(py_obj: Any) -> Any:
+    '''extract the structure of the data'''
+    def clip(value: Any) -> Any:
         if isinstance(value, str):
             return '...'
         elif isinstance(value, (list, tuple)):
             return []
         elif isinstance(value, dict):
             return {k: clip(v) for k, v in value.items()}
         else:
@@ -158,187 +160,211 @@
         return [clip(py_obj[0])]
     else:
         return clip(py_obj)
 
 
 def format_to_text(py_obj: Any, fmt: str, *,
                    compact: bool, escape: bool,
-                   indent: Union[int, str], sort_keys: bool) -> str:
+                   indent: str, sort_keys: bool) -> str:
     '''format the py_obj to text'''
     if fmt == 'json':
         if compact:
-            return json.dumps(py_obj, ensure_ascii=escape, sort_keys=sort_keys,
-                              separators=(',', ':')) + '\n'
+            result = json.dumps(py_obj, ensure_ascii=escape, sort_keys=sort_keys,
+                                separators=(',', ':'))
         else:
-            return json.dumps(py_obj, ensure_ascii=escape, sort_keys=sort_keys,
-                              indent=indent) + '\n'
-
+            result = json.dumps(py_obj, ensure_ascii=escape, sort_keys=sort_keys,
+                                indent='\t' if indent == 't' else int(indent))
     elif fmt == 'toml':
         if not isinstance(py_obj, dict):
             msg = 'the pyobj must be a Mapping when format to toml'
             raise FormatError(msg)
-        return toml.dumps(py_obj)
-
+        result = toml.dumps(utils.sort_dict(py_obj) if sort_keys else py_obj)
+    elif fmt == 'xml':
+        result = xml2py.dumps(py_obj, indent, compact, sort_keys)
     elif fmt == 'yaml':
-        _indent = None if indent == '\t' else int(indent)
-        return yaml.safe_dump(py_obj, allow_unicode=not escape, indent=_indent,
-                              sort_keys=sort_keys)
-
+        _indent = None if indent == 't' else int(indent)
+        result = yaml.safe_dump(py_obj, allow_unicode=not escape, indent=_indent,
+                                sort_keys=sort_keys)
     else:
         raise FormatError('Unknow format')
 
+    return result.strip() + '\n'
+
 
-def output(output_fp: IO, text: str, fmt: str, cp2clip: bool):
-    # copy the result to clipboard
+def get_output_fp(input_file: IO, cp2clip: bool, diff: bool,
+                  overview: bool, overwrite: bool) -> IO:
     if cp2clip:
-        pyperclip.copy(text)
-        print_inf('result copied to clipboard')
-        return
-    elif output_fp.isatty():
-        # highlight the text when output to TTY divice
-        Lexer = {'json': JsonLexer, 'toml': TOMLLexer, 'yaml': YamlLexer}[fmt]
-        colored_text = highlight(text, Lexer(), TerminalFormatter())
-        win_w, win_h = get_terminal_size()
-        # use pager when line-hight > screen hight or
-        if text.count('\n') >= win_h or len(text) > win_w * (win_h - 1):
-            with patch("sys.stdin.isatty", lambda *_: True):
-                pager(colored_text)
-        else:
-            output_fp.write(colored_text)
+        return TEMP_CLIPBOARD
+    elif diff:
+        name = f"_{os.path.basename(input_file.name)}"
+        return NamedTemporaryFile(mode='w+', prefix='jf-', suffix=name, delete=False)
+    elif input_file is sys.stdin or overview:
+        return sys.stdout
+    elif overwrite:
+        return input_file
     else:
-        if output_fp.fileno() > 2:
-            output_fp.seek(0)
-            output_fp.truncate()
+        return sys.stdout
 
-        output_fp.write(text)
 
-        if output_fp.fileno() > 2:
-            print_inf(f'result written to {output_fp.name}')
+def output(output_fp: IO, text: str, fmt: str):
+    if hasattr(output_fp, 'name') and output_fp.name == '<stdout>':
+        if output_fp.isatty():
+            # highlight the text when output to TTY divice
+            Lexer = {'json': JsonLexer, 'toml': TOMLLexer,
+                     'xml': XmlLexer, 'yaml': YamlLexer}[fmt]
+            colored_text = highlight(text, Lexer(), TerminalFormatter())
+            win_w, win_h = get_terminal_size()
+            # use pager when line-hight > screen hight or
+            if text.count('\n') >= win_h or len(text) > win_w * (win_h - 1):
+                with patch("sys.stdin.isatty", lambda *_: True):
+                    pager(colored_text)
+            else:
+                output_fp.write(colored_text)
+        else:
+            output_fp.write(text)
+    elif isinstance(output_fp, (io.TextIOWrapper, _TemporaryFileWrapper)):
+        # For regular files, changes the position to the beginning
+        # and truncates the file to zero length before overwriting
+        output_fp.seek(0)
+        output_fp.truncate()
+        output_fp.write(text)
+    elif output_fp is TEMP_CLIPBOARD and TEMP_CLIPBOARD.tell() != 0:
+        output_fp.write('\n\n')
+        output_fp.write(text)
+    else:
+        output_fp.write(text)
+    output_fp.flush()
 
 
-def process(input_fp: IO, qpath: Optional[QueryPath], to_fmt: Optional[str],
-            *, compact: bool, cp2clip: bool, escape: bool, indent: Union[int, str],
-            overview: bool, overwrite: bool, sort_keys: bool,
-            sets: Optional[list], pops: Optional[list]):
+def process(input_fp: IO, qpath: Optional[QueryPath], to_fmt: Optional[str], *,
+            compact: bool, escape: bool, indent: str, overview: bool,
+            sort_keys: bool, sets: Optional[list], pops: Optional[list]):
     # parse and format
     input_text = input_fp.read()
     py_obj, fmt = parse_to_pyobj(input_text, qpath)
 
     if sets or pops:
         modify_pyobj(py_obj, sets, pops)  # type: ignore
 
     if overview:
         py_obj = get_overview(py_obj)
 
     to_fmt = to_fmt or fmt
     formated_text = format_to_text(py_obj, to_fmt,
                                    compact=compact, escape=escape,
                                    indent=indent, sort_keys=sort_keys)
-
-    # output the result
-    if input_fp.name == '<stdin>' or not overwrite:
-        output_fp = stdout
-    else:
-        # truncate file to zero length before overwrite
-        output_fp = input_fp
-    output(output_fp, formated_text, to_fmt, cp2clip)
+    return formated_text, to_fmt
 
 
-def parse_cmdline_args(args: Optional[Sequence[str]] = None):
+def parse_cmdline_args() -> ArgumentParser:
     parser = ArgumentParser('jsonfmt')
+
+    mode = parser.add_mutually_exclusive_group()
+    mode.add_argument('-C', dest='cp2clip', action='store_true',
+                      help='CopyMode, which will copy the processing result to the clipboard')
+    mode.add_argument('-d', dest='diff', action='store_true',
+                      help='DiffMode, which compares the difference between the two input data')
+    mode.add_argument('-D', dest='difftool', type=str,
+                      help='DifftoolMode, similar to "DiffMode". You can specify a tool to perform diff comparisons')
+    mode.add_argument('-o', dest='overview', action='store_true',
+                      help='OverviewMode, which can display an overview of the structure of the data')
+    mode.add_argument('-O', dest='overwrite', action='store_true',
+                      help='OverwriteMode, which will overwrite the original file with the formated text')
+
     parser.add_argument('-c', dest='compact', action='store_true',
-                        help='suppress all whitespace separation')
-    parser.add_argument('-C', dest='cp2clip', action='store_true',
-                        help='copy the result to clipboard')
+                        help='Suppress all whitespace separation (most compact), only valid for JSON')
     parser.add_argument('-e', dest='escape', action='store_true',
                         help='escape non-ASCII characters')
-    parser.add_argument('-f', dest='format', choices=['json', 'toml', 'yaml'],
+    parser.add_argument('-f', dest='format', choices=['json', 'toml', 'xml', 'yaml'],
                         help='the format to output (default: same as input)')
-    parser.add_argument('-i', dest='indent', metavar='{0-8,t}',
+    parser.add_argument('-i', dest='indent', metavar='{0-8 or t}',
                         choices='012345678t', default='2',
                         help='number of spaces for indentation (default: %(default)s)')
-    parser.add_argument('-o', dest='overview', action='store_true',
-                        help='show data structure overview')
-    parser.add_argument('-O', dest='overwrite', action='store_true',
-                        help='overwrite the formated text to original file')
-    parser.add_argument('-l', dest='querylang', default='jmespath',
-                        choices=['jmespath', 'jsonpath'],
-                        help='the language for querying (default: %(default)s)')
+    parser.add_argument('-l', dest='querylang', choices=['jmespath', 'jsonpath'],
+                        help='query language for extracting data (default: auto-detect)')
     parser.add_argument('-p', dest='querypath', type=str,
                         help='the path for querying')
     parser.add_argument('-s', dest='sort_keys', action='store_true',
-                        help='sort keys of objects on output')
+                        help='sort the output of dictionaries alphabetically by key')
     parser.add_argument('--set', metavar="'foo.k1=v1;k2[i]=v2'",
-                        help='set the keys to values (seperated by `;`)')
+                        help='key-value pairs to add or modify (seperated by `;`)')
     parser.add_argument('--pop', metavar="'k1;foo.k2;k3[i]'",
-                        help='pop the specified keys (seperated by `;`)')
+                        help='key-value pairs to delete (seperated by `;`)')
     parser.add_argument(dest='files', nargs='*',
                         help='the files that will be processed')
     parser.add_argument('-v', dest='version', action='version',
                         version=__version__, help="show the version")
-    return parser.parse_args(args)
+    return parser
 
 
 def main():
-    args = parse_cmdline_args()
+    parser = parse_cmdline_args()
+    args = parser.parse_args()
 
-    if args.querypath is None:
-        querypath = None
-    else:
-        parse_path = {'jmespath': jcompile, 'jsonpath': jparse}[args.querylang]
-        try:
-            querypath = parse_path(args.querypath)
-        except (JMESPathError, JSONPathError, AttributeError):
-            print_err(f'invalid querypath expression: "{args.querypath}"')
-            sys_exit(1)
+    # check and parse the querypath
+    querypath = parse_querypath(args.querypath, args.querylang)
 
     # check if the clipboard is available
-    cp2clip = args.cp2clip and is_clipboard_available()
-    if args.cp2clip and not cp2clip:
-        print_err('clipboard unavailable')
-
-    # check the indent
-    indent = '\t' if args.indent == 't' else int(args.indent)
+    if args.cp2clip and not is_clipboard_available():
+        utils.exit_with_error('clipboard unavailable')
 
-    # the overwrite will be forced to close when showing overview
-    overwrite = False if args.overview else args.overwrite
+    # check the input files
+    files = args.files or [sys.stdin]
+    n_files = len(files)
+
+    # check the diff mode
+    diff_mode: bool = args.diff or args.difftool
+    if diff_mode and len(files) != 2:
+        utils.exit_with_error('less than two files')
+    sort_keys = True if diff_mode else args.sort_keys
 
     # get sets and pops
     sets = [k.strip() for k in args.set.split(';')] if args.set else []
     pops = [k.strip() for k in args.pop.split(';')] if args.pop else []
 
-    files = args.files or [stdin]
-    files_cnt = len(files)
+    output_title = n_files > 1 and not (diff_mode or args.cp2clip or args.overwrite)
+
+    diff_files = []
+    for idx, file in enumerate(files, start=1):
+        if output_title:
+            title = f'{idx}. {file}' if idx == 1 else f'\n{idx}. {file}'
+            print(f'\033[37m{title}\033[0m')
 
-    for num, file in enumerate(files, start=1):
         try:
-            # read from file
+            # process the input data file
             input_fp = open(file, 'r+') if isinstance(file, str) else file
-            process(input_fp,
-                    querypath,
-                    args.format,
-                    compact=args.compact,
-                    cp2clip=cp2clip,
-                    escape=args.escape,
-                    indent=indent,
-                    overview=args.overview,
-                    overwrite=overwrite,
-                    sort_keys=args.sort_keys,
-                    sets=sets,
-                    pops=pops)
-            # output a line to separate multiple results
-            if num < files_cnt:
-                print('----------------', file=stdout)
-        except (FormatError, JMESPathError, JSONPathError) as err:
-            print_err(err)
-        except FileNotFoundError:
-            print_err(f'no such file: {file}')
-        except PermissionError:
-            print_err(f'permission denied: {file}')
+            formated, fmt = process(input_fp, querypath, args.format,
+                                    compact=args.compact, escape=args.escape,
+                                    indent=args.indent, overview=args.overview,
+                                    sort_keys=sort_keys, sets=sets, pops=pops)
+            # output the result
+            output_fp = get_output_fp(input_fp, args.cp2clip, diff_mode,
+                                      args.overview, args.overwrite)
+            output(output_fp, formated, fmt)
+
+            if diff_mode:
+                diff_files.append(output_fp.name)
+            elif args.overwrite:
+                utils.print_inf(f'result written to {os.path.basename(output_fp.name)}')
+
+        except (FormatError, JMESPathError, JSONPathError, OSError) as err:
+            utils.print_err(err)
+        except KeyboardInterrupt:
+            utils.exit_with_error('user canceled')
         finally:
             input_fp = locals().get('input_fp')
-            if isinstance(input_fp, TextIOBase):
+            if isinstance(input_fp, io.TextIOBase):
                 input_fp.close()
 
+    if args.cp2clip:
+        TEMP_CLIPBOARD.seek(0)
+        pyperclip.copy(TEMP_CLIPBOARD.read())
+        utils.print_inf('result copied to clipboard')
+    elif diff_mode:
+        try:
+            compare(diff_files[0], diff_files[1], args.difftool)
+        except (OSError, ValueError, IndexError) as err:
+            utils.exit_with_error(err)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `jsonfmt-0.2.6/pyproject.toml` & `jsonfmt-0.2.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsonfmt"
 dynamic = ["dependencies", "version"]
 requires-python = ">=3.6"
-license = {text = "MIT License"}
-description = "A simple tool for formatting JSON object."
+license = { text = "MIT License" }
+description = "A powerful tool for pretty-printing, querying and conversion JSON documents."
 readme = "README.md"
 keywords = ["json", "formatter", "pretty-print", "highlight", "jmespath"]
-authors = [{name = "Seamile", email = "lanhuermao@gmail.com"}]
+authors = [{ name = "Seamile", email = "lanhuermao@gmail.com" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
@@ -29,13 +29,16 @@
 ]
 
 [project.urls]
 homepage = "https://github.com/seamile/jsonfmt"
 repository = "https://github.com/seamile/jsonfmt"
 documentation = "https://seamile.github.io/jsonfmt/"
 
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
-version = {attr = "jsonfmt.__version__" }
-
 [project.scripts]
-jsonfmt = "jsonfmt:main"
+jf = "jsonfmt.jsonfmt:main"
+
+[tool.setuptools]
+packages = ["jsonfmt"]
+
+[tool.setuptools.dynamic]
+dependencies = { file = ["requirements.txt"] }
+version = { attr = "jsonfmt.__version__" }
```

### Comparing `jsonfmt-0.2.6/test/test.py` & `jsonfmt-0.2.7/test/test_jsonfmt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 import json
 import os
 import sys
 import tempfile
 import unittest
-import pyperclip
 from argparse import Namespace
+from contextlib import contextmanager
 from copy import deepcopy
 from functools import partial
 from io import StringIO
+from unittest.mock import patch
+
+import pyperclip
 from jmespath import compile as jcompile
 from jsonpath_ng import parse as jparse
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
-from pygments.lexers import JsonLexer, YamlLexer, TOMLLexer
-from unittest.mock import patch
+from pygments.lexers import JsonLexer, TOMLLexer, XmlLexer, YamlLexer
 
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 sys.path.insert(0, BASE_DIR)
-import jsonfmt
+from jsonfmt import jsonfmt
 
 JSON_FILE = f'{BASE_DIR}/test/example.json'
 with open(JSON_FILE) as json_fp:
     JSON_TEXT = json_fp.read()
 
 TOML_FILE = f'{BASE_DIR}/test/example.toml'
 with open(TOML_FILE) as toml_fp:
     TOML_TEXT = toml_fp.read()
 
+XML_FILE = f'{BASE_DIR}/test/example.xml'
+with open(XML_FILE) as xml_fp:
+    XML_TEXT = xml_fp.read()
+
 YAML_FILE = f'{BASE_DIR}/test/example.yaml'
 with open(YAML_FILE) as yaml_fp:
     YAML_TEXT = yaml_fp.read()
 
 
-def color(text, format):
-    fn = {
-        'json': partial(highlight,
-                        lexer=JsonLexer(),
-                        formatter=TerminalFormatter()),
-        'toml': partial(highlight,
-                        lexer=TOMLLexer(),
-                        formatter=TerminalFormatter()),
-        'yaml': partial(highlight,
-                        lexer=YamlLexer(),
-                        formatter=TerminalFormatter()),
-    }[format]
+def color(text, fmt):
+    functions = {
+        'json': partial(highlight, lexer=JsonLexer(), formatter=TerminalFormatter()),
+        'toml': partial(highlight, lexer=TOMLLexer(), formatter=TerminalFormatter()),
+        'xml': partial(highlight, lexer=XmlLexer(), formatter=TerminalFormatter()),
+        'yaml': partial(highlight, lexer=YamlLexer(), formatter=TerminalFormatter()),
+    }
+    fn = functions[fmt]
     return fn(text)
 
 
-class FakeStdStream(StringIO):
+class FakeStream(StringIO):
 
     def __init__(self, initial_value='', newline='\n', tty=True):
         super().__init__(initial_value, newline)
         self._istty = tty
 
     def isatty(self):
         return self._istty
@@ -61,67 +63,94 @@
         content = super().read()
 
         self.seek(0)
         self.truncate()
         return content
 
 
-class FakeStdIn(FakeStdStream):
+class StdIn(FakeStream):
     name = '<stdin>'
 
     def fileno(self) -> int:
         return 0
 
 
-class FakeStdOut(FakeStdStream):
+class StdOut(FakeStream):
     name = '<stdout>'
 
     def fileno(self) -> int:
         return 1
 
 
-class FakeStdErr(FakeStdStream):
+class StdErr(FakeStream):
     name = '<stderr>'
 
     def fileno(self) -> int:
         return 2
 
 
 class JSONFormatToolTestCase(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         self.py_obj = json.loads(JSON_TEXT)
 
+    @contextmanager
+    def assertNotRaises(self, exc_type):
+        try:
+            yield None
+        except exc_type:
+            raise self.failureException('{} raised'.format(exc_type.__name__))
+
     def test_is_clipboard_available(self):
         available = jsonfmt.is_clipboard_available()
         self.assertIsInstance(available, bool)
 
+    def test_parse_querypath(self):
+        jmespath, jsonpath = 'actions.name', '$..name'
+        # test parse jmespath
+        res1 = jsonfmt.parse_querypath(jmespath, None)
+        res2 = jsonfmt.parse_querypath(jmespath, 'jmespath')
+
+        self.assertEqual(res1, res2)
+        # test parse jsonpath
+        res3 = jsonfmt.parse_querypath(jsonpath, None)
+        res4 = jsonfmt.parse_querypath(jsonpath, 'jsonpath')
+        self.assertEqual(res3, res4)
+
+        # test wrong args
+        self.assertEqual(jsonfmt.parse_querypath(None, None), None)
+        with self.assertRaises(SystemExit):
+            jsonfmt.parse_querypath('as*df', None)
+
+        with self.assertRaises(SystemExit):
+            jsonfmt.parse_querypath(jsonpath, 'wrong')
+
     def test_parse_to_pyobj_with_jmespath(self):
         # normal parameters test
         matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, jcompile("actions[:].calorie"))
-        self.assertEqual(matched_obj, ([294.9, -375], 'json'))
+        self.assertEqual(matched_obj, ([1294.9, -2375, -420.5], 'json'))
         matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jcompile("actions[*].name"))
-        self.assertEqual(matched_obj, (['eat', 'sport'], 'toml'))
+        self.assertEqual(matched_obj, (['eating', 'sporting', 'sleeping'], 'toml'))
         matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jcompile("actions[*].date"))
-        self.assertEqual(matched_obj, (['2021-03-02', '2023-04-27'], 'yaml'))
+        self.assertEqual(matched_obj, (['2021-03-02', '2023-04-27', '2023-05-15'], 'yaml'))
         # test not exists key
         matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jcompile("not_exist_key"))
         self.assertEqual(matched_obj, (None, 'toml'))
         # test index out of range
         matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jcompile('actions[7]'))
         self.assertEqual(matched_obj, (None, 'yaml'))
 
     def test_parse_to_pyobj_with_jsonpath(self):
         # normal parameters test
         matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, jparse("age"))
         self.assertEqual(matched_obj, (23, 'json'))
         matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jparse("$..name"))
-        self.assertEqual(matched_obj, (['Bob', 'eat', 'sport'], 'toml'))
+        self.assertEqual(matched_obj, (['Bob', 'eating', 'sporting', 'sleeping'], 'toml'))
         matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jparse("actions[*].date"))
-        self.assertEqual(matched_obj, (['2021-03-02', '2023-04-27'], 'yaml'))
+        self.assertEqual(matched_obj, (['2021-03-02', '2023-04-27', '2023-05-15'], 'yaml'))
         # test not exists key
         matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jparse("not_exist_key"))
         self.assertEqual(matched_obj, (None, 'toml'))
         # test index out of range
         matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jparse('actions[7]'))
         self.assertEqual(matched_obj, (None, 'yaml'))
 
@@ -137,20 +166,20 @@
 
         # test add new value
         obj = deepcopy(self.py_obj)
         # add single value to dict
         jsonfmt.modify_pyobj(obj, ['new=value'], [])
         self.assertEqual(obj['new'], 'value')
         # add single value to list
-        jsonfmt.modify_pyobj(obj, ['actions[20]={"K":"V"}'], [])
-        self.assertEqual(obj['actions'][2], {"K": "V"})
+        jsonfmt.modify_pyobj(obj, ['actions[10]={"A":"B"}'], [])
+        self.assertEqual(obj['actions'][-1], {"A": "B"})
         # add multiple values at once
-        jsonfmt.modify_pyobj(obj, ['new=[1,2,3]', 'actions[50]={"K":"V"}'], [])
+        jsonfmt.modify_pyobj(obj, ['new=[1,2,3]', 'actions[11]={"X":"Y"}'], [])
         self.assertEqual(obj['new'], [1, 2, 3])
-        self.assertEqual(obj['actions'][2], {"K": "V"})
+        self.assertEqual(obj['actions'][-1], {"X": "Y"})
 
     def test_modify_pyobj_for_modifying(self):
         # test modify values
         obj = deepcopy(self.py_obj)
         # modify single value
         jsonfmt.modify_pyobj(obj, ['name=Alex'], [])
         self.assertEqual(obj['name'], 'Alex')
@@ -158,43 +187,44 @@
         jsonfmt.modify_pyobj(obj, ['gender=[male]', 'actions[0].calorie=0'], [])
         self.assertEqual(obj['gender'], '[male]')
         self.assertEqual(obj['actions'][0]['calorie'], 0)
 
     def test_modify_pyobj_for_popping(self):
         # test pop values
         obj = deepcopy(self.py_obj)
+        n_actions = len(obj['actions'])
         # pop single value
         jsonfmt.modify_pyobj(obj, [], ['age'])
         self.assertNotIn('age', obj)
         # pop multiple values at once
         jsonfmt.modify_pyobj(obj, [], ['money', 'actions[1]', 'actions.0.date'])
         self.assertNotIn('money', obj)
         self.assertNotIn('date', obj['actions'][0])
-        self.assertEqual(1, len(obj['actions']))
+        self.assertEqual(n_actions - 1, len(obj['actions']))
 
     def test_modify_pyobj_for_all(self):
         # test adding, popping and modifying simultaneously
         obj = deepcopy(self.py_obj)
         jsonfmt.modify_pyobj(obj,
                              ['new=abc', 'actions.0=[]'],  # add and modify
                              ['actions.1.name', 'age'])  # pop
         self.assertEqual(obj['new'], 'abc')
         self.assertEqual(obj['actions'][0], [])
         self.assertNotIn('name', obj['actions'][1])
         self.assertNotIn('age', obj)
 
         # test exceptions
         obj = deepcopy(self.py_obj)
-        with patch('jsonfmt.stderr', FakeStdErr()):
+        with patch('sys.stderr', StdErr()):
             # modifying
             jsonfmt.modify_pyobj(obj, ['aa.bb=empty'], [])
-            self.assertIn('invalid key path', jsonfmt.stderr.read())
+            self.assertIn('invalid key path', sys.stderr.read())
             # popping
             jsonfmt.modify_pyobj(obj, [], ['actions[3]'])
-            self.assertIn('invalid key path', jsonfmt.stderr.read())
+            self.assertIn('invalid key path', sys.stderr.read())
 
     def test_get_overview(self):
         # test dict obj
         obj = deepcopy(self.py_obj)
         obj['dict'] = {"a": 7758, "b": [1, 2, 3]}
         expected_1 = {
             'actions': [],
@@ -210,258 +240,280 @@
         overview = jsonfmt.get_overview(obj)
         self.assertEqual(overview, expected_1)
 
         # test list obj
         obj = deepcopy(self.py_obj['actions'])
         expected_2 = [
             {
-                "calorie": 294.9,
-                "date": "...",
-                "name": "..."
+                "name": "...",
+                "calorie": 1294.9,
+                "date": "..."
             }
         ]
         overview = jsonfmt.get_overview(obj)
         self.assertEqual(overview, expected_2)
 
     def test_format_to_text(self):
         py_obj = {"name": "约翰", "age": 30}
         # format to json (compacted)
         j_compacted = jsonfmt.format_to_text(py_obj, 'json',
                                              compact=True, escape=True,
-                                             indent=4, sort_keys=False)
+                                             indent='4', sort_keys=False)
         self.assertEqual(j_compacted.strip(), '{"name":"\\u7ea6\\u7ff0","age":30}')
 
         # format to json (indentation)
         j_indented = jsonfmt.format_to_text(py_obj, 'json',
                                             compact=False, escape=False,
-                                            indent=4, sort_keys=True)
-        self.assertEqual(j_indented.strip(), '{\n    "age": 30,\n    "name": "约翰"\n}')
+                                            indent='t', sort_keys=True)
+        self.assertEqual(j_indented.strip(), '{\n\t"age": 30,\n\t"name": "约翰"\n}')
 
         # format to toml
         toml_text = jsonfmt.format_to_text(self.py_obj, 'toml',
                                            compact=False, escape=False,
-                                           indent=4, sort_keys=False)
+                                           indent='4', sort_keys=False)
         self.assertEqual(toml_text.strip(), TOML_TEXT.strip())
 
+        # format to xml
+        xml_text = jsonfmt.format_to_text(py_obj, 'xml',
+                                          compact=True, escape=False,
+                                          indent='t', sort_keys=True)
+        result = '<root><age>30</age><name>约翰</name></root>'
+        self.assertEqual(xml_text.strip(), result)
+
         # format to yaml
         yaml_text = jsonfmt.format_to_text(self.py_obj, 'yaml',
                                            compact=False, escape=False,
-                                           indent=2, sort_keys=True)
+                                           indent='2', sort_keys=False)
         self.assertEqual(yaml_text.strip(), YAML_TEXT.strip())
 
         # test exceptions
         with self.assertRaises(jsonfmt.FormatError):
             jsonfmt.format_to_text([1, 2, 3], 'toml',
                                    compact=False, escape=False,
-                                   indent=4, sort_keys=False)
+                                   indent='4', sort_keys=False)
 
         with self.assertRaises(jsonfmt.FormatError):
-            jsonfmt.format_to_text(py_obj, 'xml',
+            jsonfmt.format_to_text(py_obj, 'unknow',
                                    compact=False, escape=False,
-                                   indent=4, sort_keys=False)
+                                   indent='4', sort_keys=False)
 
     def test_output(self):
         # output JSON to clipboard
-        if jsonfmt.is_clipboard_available():
-            with patch('jsonfmt.stdout', FakeStdOut()):
-                jsonfmt.output(jsonfmt.stdout, JSON_TEXT, 'json', True)
-                self.assertEqual(pyperclip.paste(), JSON_TEXT)
+        jsonfmt.TEMP_CLIPBOARD.seek(0)
+        jsonfmt.TEMP_CLIPBOARD.truncate()
+        jsonfmt.output(jsonfmt.TEMP_CLIPBOARD, JSON_TEXT, 'json')
+        jsonfmt.output(jsonfmt.TEMP_CLIPBOARD, XML_TEXT, 'xml')
+        jsonfmt.TEMP_CLIPBOARD.seek(0)
+        self.assertEqual(jsonfmt.TEMP_CLIPBOARD.read(),
+                         JSON_TEXT + '\n\n' + XML_TEXT)
 
         # output TOML to file (temp file)
         with tempfile.NamedTemporaryFile(mode='r+') as tmpfile:
-            jsonfmt.output(tmpfile, TOML_TEXT, 'toml', False)
+            jsonfmt.output(tmpfile, TOML_TEXT, 'toml')
             tmpfile.seek(0)
             self.assertEqual(tmpfile.read(), TOML_TEXT)
 
         # output YAML to stdout (mock)
-        with patch('jsonfmt.stdout', FakeStdOut()):
-            jsonfmt.output(jsonfmt.stdout, YAML_TEXT, 'yaml', False)
-            self.assertEqual(jsonfmt.stdout.read(), color(YAML_TEXT, 'yaml'))
+        with patch('sys.stdout', StdOut()):
+            jsonfmt.output(sys.stdout, YAML_TEXT, 'yaml')
+            self.assertEqual(sys.stdout.read(), color(YAML_TEXT, 'yaml'))
 
         # output unknow format
-        with self.assertRaises(KeyError), patch('jsonfmt.stdout', FakeStdOut()):
-            jsonfmt.output(jsonfmt.stdout, YAML_TEXT, 'xml', False)
+        with self.assertRaises(KeyError), patch('sys.stdout', StdOut()):
+            jsonfmt.output(sys.stdout, YAML_TEXT, 'null')
 
     def test_parse_cmdline_args(self):
         # test default parameters
         default_args = Namespace(
-            compact=False,
             cp2clip=False,
+            diff=False,
+            difftool=None,
+            overview=False,
+            overwrite=False,
+            compact=False,
             escape=False,
             format=None,
             indent='2',
-            overview=False,
-            overwrite=False,
-            querylang='jmespath',
+            querylang=None,
             querypath=None,
             sort_keys=False,
             set=None,
             pop=None,
             files=[]
         )
-        actual_args = jsonfmt.parse_cmdline_args(args=[])
-        self.assertEqual(actual_args, default_args)
+
+        with patch('sys.argv', ['jf']):
+            actual_args = jsonfmt.parse_cmdline_args().parse_args()
+            self.assertEqual(actual_args, default_args)
 
         # test specified parameters
-        args = [
-            '-c',
-            '-C',
-            '-e',
-            '-f', 'toml',
-            '-i', '4',
-            '-o',
-            '-O',
-            '-l', 'jsonpath',
-            '-p', 'path.to.json',
-            '--set', 'a; b',
-            '--pop', 'c; d',
-            '-s',
-            'file1.json',
-            'file2.json'
-        ]
         expected_args = Namespace(
+            cp2clip=False,
+            diff=True,
+            difftool=None,
+            overview=False,
+            overwrite=False,
             compact=True,
-            cp2clip=True,
             escape=True,
             format='toml',
             indent='4',
-            overview=True,
-            overwrite=True,
             querylang='jsonpath',
             querypath='path.to.json',
             sort_keys=True,
             set='a; b',
             pop='c; d',
             files=['file1.json', 'file2.json']
         )
-
-        actual_args = jsonfmt.parse_cmdline_args(args=args)
-        self.assertEqual(actual_args, expected_args)
+        with patch('sys.argv', ['jf', '-d', '-c', '-e', '-f', 'toml', '-i', '4',
+                                '-l', 'jsonpath', '-p', 'path.to.json', '-s',
+                                '--set', 'a; b', '--pop', 'c; d',
+                                'file1.json', 'file2.json']):
+            actual_args = jsonfmt.parse_cmdline_args().parse_args()
+            self.assertEqual(actual_args, expected_args)
 
     ############################################################################
     #                                 main test                                #
     ############################################################################
 
-    @patch.multiple(sys, argv=['jsonfmt', '-i', 't', '-p', 'actions[*].name',
+    @patch.multiple(sys, argv=['jf', '-i', 't', '-p', 'actions[*].name',
                                JSON_FILE, YAML_FILE])
-    @patch.multiple(jsonfmt, stdout=FakeStdOut())
+    @patch.multiple(sys, stdout=StdOut())
     def test_main_with_file(self):
-        expected_output = color('[\n\t"eat",\n\t"sport"\n]', 'json')
-        expected_output += '----------------\n'
-        expected_output += color('- eat\n- sport', 'yaml')
+        json_output = color('[\n\t"eating",\n\t"sporting",\n\t"sleeping"\n]', 'json')
+        yaml_output = color('- eating\n- sporting\n- sleeping', 'yaml')
         jsonfmt.main()
-        self.assertEqual(jsonfmt.stdout.read(), expected_output)
+        output = sys.stdout.read()
+        self.assertIn(json_output, output)
+        self.assertIn(yaml_output, output)
 
-    @patch.multiple(sys, argv=['jsonfmt', '-f', 'yaml'])
-    @patch.multiple(jsonfmt, stdin=FakeStdIn('["a", "b"]'), stdout=FakeStdOut())
     def test_main_with_stdin(self):
-        expected_output = color('- a\n- b', 'yaml')
-        jsonfmt.main()
-        self.assertEqual(jsonfmt.stdout.read(), expected_output)
+        with patch.multiple(sys, argv=['jf', '-f', 'yaml'],
+                            stdin=StdIn('["a", "b"]'), stdout=StdOut()):
+            expected_output = color('- a\n- b', 'yaml')
+            jsonfmt.main()
+            self.assertEqual(sys.stdout.read(), expected_output)
 
-    @patch.multiple(jsonfmt, stderr=FakeStdErr())
+    @patch.multiple(sys, stderr=StdErr())
     def test_main_invalid_input(self):
         # test not exist file and wrong format
-        with patch.multiple(sys, argv=['jsonfmt', 'not_exist_file.json', __file__]):
+        with patch.multiple(sys, argv=['jf', 'not_exist_file.json', __file__]):
             jsonfmt.main()
-            errmsg = jsonfmt.stderr.read()
-            self.assertIn('no such file: not_exist_file.json', errmsg)
-            self.assertIn('no json, toml or yaml found', errmsg)
+            errmsg = sys.stderr.read()
+            self.assertIn("No such file or directory: 'not_exist_file.json'", errmsg)
+            self.assertIn('no supported format found', errmsg)
 
-    @patch.multiple(jsonfmt, stderr=FakeStdErr())
+        with patch.multiple(sys, argv=['jf']), \
+                patch('sys.stdin.read', side_effect=KeyboardInterrupt), \
+                self.assertRaises(SystemExit):
+            jsonfmt.main()
+        self.assertIn('user canceled', sys.stderr.read())
+
+    @patch.multiple(sys, stderr=StdErr())
     def test_main_querying(self):
         # test empty jmespath
-        with patch('sys.argv', ['jsonfmt', JSON_FILE, '-p', '$.-[=]']),\
+        with patch('sys.argv', ['jf', JSON_FILE, '-p', '$.-[=]']), \
                 self.assertRaises(SystemExit):
             jsonfmt.main()
-        self.assertIn('invalid querypath expression', jsonfmt.stderr.read())
+        self.assertIn('invalid querypath expression', sys.stderr.read())
 
         # test empty jmespath
-        with patch('sys.argv', ['jsonfmt', JSON_FILE, '-l', 'jsonpath', '-p', ' ']),\
+        with patch('sys.argv', ['jf', JSON_FILE, '-l', 'jsonpath', '-p', ' ']), \
                 self.assertRaises(SystemExit):
             jsonfmt.main()
-        self.assertIn('invalid querypath expression', jsonfmt.stderr.read())
+        self.assertIn('invalid querypath expression', sys.stderr.read())
 
-    @patch('jsonfmt.stdout', FakeStdOut())
+    @patch('sys.stdout', StdOut())
     def test_main_convert(self):
         # test json to toml
-        with patch.multiple(sys, argv=['jsonfmt', '-f', 'toml', JSON_FILE]):
-            colored_output = color(TOML_TEXT, 'toml')
+        with patch.multiple(sys, argv=['jf', '-f', 'toml', JSON_FILE]):
             jsonfmt.main()
-            self.assertEqual(jsonfmt.stdout.read(), colored_output)
+            self.assertEqual(sys.stdout.read(), color(TOML_TEXT, 'toml'))
 
-        # test toml to yaml
-        with patch.multiple(sys, argv=['jsonfmt', '-s', '-f', 'yaml', TOML_FILE]):
-            colored_output = color(YAML_TEXT, 'yaml')
+        # test toml to xml
+        with patch.multiple(sys, argv=['jf', '-f', 'xml', TOML_FILE]):
             jsonfmt.main()
-            self.assertEqual(jsonfmt.stdout.read(), colored_output)
+            self.assertEqual(sys.stdout.read(), color(XML_TEXT, 'xml'))
+
+        # test xml to yaml
+        with patch.multiple(sys, argv=['jf', '-f', 'yaml', XML_FILE]):
+            jsonfmt.main()
+            self.assertEqual(sys.stdout.read(), color(YAML_TEXT, 'yaml'))
 
         # test yaml to json
-        with patch.multiple(sys, argv=['jsonfmt', '-c', '-f', 'json', YAML_FILE]):
-            colored_output = color(JSON_TEXT, 'json')
+        with patch.multiple(sys, argv=['jf', '-c', '-f', 'json', YAML_FILE]):
             jsonfmt.main()
-            self.assertEqual(jsonfmt.stdout.read(), colored_output)
+            self.assertEqual(sys.stdout.read(), color(JSON_TEXT, 'json'))
 
-    @patch.multiple(sys, argv=['jsonfmt', '-oc'])
-    @patch.multiple(jsonfmt, stdin=FakeStdIn('{"a": "asfd", "b": [1, 2, 3]}'), stdout=FakeStdOut(tty=False))
+    @patch.multiple(sys, argv=['jf', '-oc'])
+    @patch.multiple(sys,
+                    stdin=StdIn('{"a": "asfd", "b": [1, 2, 3]}'),
+                    stdout=StdOut(tty=False))
     def test_main_overview(self):
         jsonfmt.main()
-        self.assertEqual(jsonfmt.stdout.read().strip(), '{"a":"...","b":[]}')
+        self.assertEqual(sys.stdout.read().strip(), '{"a":"...","b":[]}')
 
-    @patch('sys.argv', ['jsonfmt', '-Ocsf', 'json', TOML_FILE])
+    @patch('sys.argv', ['jf', '-Ocf', 'json', TOML_FILE])
     def test_main_overwrite_to_original_file(self):
         try:
             jsonfmt.main()
             with open(TOML_FILE) as toml_fp:
                 new_content = toml_fp.read().strip()
             self.assertEqual(new_content, JSON_TEXT.strip())
         finally:
             with open(TOML_FILE, 'w') as toml_fp:
                 toml_fp.write(TOML_TEXT)
 
-    @patch.multiple(jsonfmt, stdout=FakeStdOut(), stderr=FakeStdErr())
+    @patch.multiple(sys, argv=['jf', '-Cc', JSON_FILE, TOML_FILE])
     def test_main_copy_to_clipboard(self):
         if jsonfmt.is_clipboard_available():
-            with patch("sys.argv",
-                       ['jsonfmt', '-Ccs', JSON_FILE]):
-                jsonfmt.main()
-                copied_text = pyperclip.paste().strip()
-                self.assertEqual(copied_text, JSON_TEXT.strip())
-
-            with patch("sys.argv",
-                       ['jsonfmt', '-Cs', TOML_FILE]):
-                jsonfmt.main()
-                copied_text = pyperclip.paste().strip()
-                self.assertEqual(copied_text, TOML_TEXT.strip())
-
-            with patch("sys.argv",
-                       ['jsonfmt', '-Cs', YAML_FILE]):
-                jsonfmt.main()
-                copied_text = pyperclip.paste().strip()
-                self.assertEqual(copied_text, YAML_TEXT.strip())
+            pyperclip.copy('')
+            jsonfmt.main()
+            copied_text = pyperclip.paste().strip()
+            self.assertEqual(copied_text, JSON_TEXT.strip() + '\n\n\n' + TOML_TEXT.strip())
 
     @patch.multiple(jsonfmt, is_clipboard_available=lambda: False)
-    @patch.multiple(jsonfmt, stdout=FakeStdOut(), stderr=FakeStdErr())
-    @patch.multiple(sys, argv=['jsonfmt', JSON_FILE, '-cC'])
+    @patch.multiple(sys, stderr=StdErr())
+    @patch.multiple(sys, argv=['jf', JSON_FILE, '-cC'])
     def test_main_clipboard_unavailable(self):
         errmsg = '\033[1;91mjsonfmt:\033[0m \033[0;91mclipboard unavailable\033[0m\n'
-        jsonfmt.main()
-        self.assertEqual(jsonfmt.stderr.read(), errmsg)
-        self.assertEqual(jsonfmt.stdout.read(), color(JSON_TEXT, 'json'))
+        with self.assertRaises(SystemExit):
+            jsonfmt.main()
+        self.assertEqual(sys.stderr.read(), errmsg)
 
-    @patch.multiple(sys, argv=['jsonfmt', '--set', 'age=32; box=[1,2,3]', '--pop', 'money; actions.1'])
-    @patch.multiple(jsonfmt, stdin=FakeStdIn(JSON_TEXT), stdout=FakeStdOut(tty=False))
+    @patch.multiple(sys,
+                    argv=['jf',
+                          '--set', 'age=32; box=[1,2,3]',
+                          '--pop', 'money; actions.1'])
+    @patch.multiple(sys, stdin=StdIn(JSON_TEXT), stdout=StdOut(tty=False))
     def test_main_modify_and_pop(self):
         try:
             jsonfmt.main()
-            py_obj = json.loads(jsonfmt.stdout.read())
+            py_obj = json.loads(sys.stdout.read())
             self.assertEqual(py_obj['age'], 32)
             self.assertEqual(py_obj['box'], [1, 2, 3])
             self.assertNotIn('money', py_obj)
-            self.assertEqual(len(py_obj['actions']), 1)
+            self.assertEqual(len(py_obj['actions']), 2)
         finally:
             with open(JSON_FILE, 'w') as fp:
                 fp.write(JSON_TEXT)
 
+    @patch.multiple(sys, stdout=StdOut(), stderr=StdErr())
+    def test_main_diff_mode(self):
+        # right way
+        with patch.multiple(sys, argv=['jf', '-D', 'diff', JSON_FILE, XML_FILE]), \
+                self.assertNotRaises(SystemExit):
+            jsonfmt.main()
+
+        # wrong args
+        with patch.multiple(sys, argv=['jf', '-D', 'diff', XML_FILE]), \
+                self.assertRaises(SystemExit):
+            jsonfmt.main()
+        self.assertIn('less than two files', sys.stderr.read())
+
+        with patch.multiple(sys, argv=['jf', '-D', 'nothing', XML_FILE, TOML_FILE]), \
+                self.assertRaises(SystemExit):
+            jsonfmt.main()
+        self.assertIn("No such file or directory: 'nothing'", sys.stderr.read())
+
 
 if __name__ == "__main__":
     unittest.main()
```

