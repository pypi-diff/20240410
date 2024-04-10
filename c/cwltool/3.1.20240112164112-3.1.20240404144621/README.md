# Comparing `tmp/cwltool-3.1.20240112164112.tar.gz` & `tmp/cwltool-3.1.20240404144621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwltool-3.1.20240112164112.tar", last modified: Mon Jan 15 14:34:42 2024, max compression
+gzip compressed data, was "cwltool-3.1.20240404144621.tar", last modified: Wed Apr 10 13:22:11 2024, max compression
```

## Comparing `cwltool-3.1.20240112164112.tar` & `cwltool-3.1.20240404144621.tar`

### file list

```diff
@@ -1,1066 +1,1068 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.250373 cwltool-3.1.20240112164112/
--rw-r--r--   0 michael   (1000) michael   (1000)       40 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.codecov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.coveragerc
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.dockerignore
--rw-r--r--   0 michael   (1000) michael   (1000)      224 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.flake8
--rw-r--r--   0 michael   (1000) michael   (1000)      203 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.git-blame-ignore-revs
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.gitattributes
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.118372 cwltool-3.1.20240112164112/.github/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.118372 cwltool-3.1.20240112164112/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 michael   (1000) michael   (1000)      143 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 michael   (1000) michael   (1000)      643 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.github/dependabot.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.118372 cwltool-3.1.20240112164112/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)     8971 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.github/workflows/ci-tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      699 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2030 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.github/workflows/quay-publish.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      593 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)      734 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.mergify.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      512 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.readthedocs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      385 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/.snyk
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     4343 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     3181 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     7511 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)    40543 2024-01-15 14:34:42.250373 cwltool-3.1.20240112164112/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    38143 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/README.rst
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1084 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/build-cwltool-docker.sh
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6501 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/conformance-test.sh
--rwxr-xr-x   0 michael   (1000) michael   (1000)      280 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwl-docker.sh
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.118372 cwltool-3.1.20240112164112/cwlref-runner/
--rw-r--r--   0 michael   (1000) michael   (1000)      223 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwlref-runner/README
--rw-r--r--   0 michael   (1000) michael   (1000)      771 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwlref-runner/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.122372 cwltool-3.1.20240112164112/cwltool/
--rw-r--r--   0 michael   (1000) michael   (1000)      280 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)       81 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-01-15 14:34:41.000000 cwltool-3.1.20240112164112/cwltool/_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30839 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/argparser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29615 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/builder.py
--rw-r--r--   0 michael   (1000) michael   (1000)    21295 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/checker.py
--rw-r--r--   0 michael   (1000) michael   (1000)    66095 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/command_line_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9183 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/context.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2341 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/cuda.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.126372 cwltool-3.1.20240112164112/cwltool/cwlprov/
--rw-r--r--   0 michael   (1000) michael   (1000)     5140 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/cwlprov/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1887 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/cwlprov/provenance_constants.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32956 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/cwlprov/provenance_profile.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23846 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/cwlprov/ro.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10899 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/cwlprov/writablebagfile.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6398 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/cwlrdf.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7317 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/cwlviewer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    18416 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/docker.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4283 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/docker_id.py
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/env_to_stdout.py
--rw-r--r--   0 michael   (1000) michael   (1000)      346 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)    20002 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/executors.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3587 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/extensions-v1.1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     7992 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/extensions-v1.2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     6788 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/extensions.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2402 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/factory.py
--rw-r--r--   0 michael   (1000) michael   (1000)      704 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/flatten.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4127 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/hello.simg
--rw-r--r--   0 michael   (1000) michael   (1000)    40577 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.126372 cwltool-3.1.20240112164112/cwltool/jshint/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  1286196 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/jshint/jshint.js
--rw-r--r--   0 michael   (1000) michael   (1000)     1240 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/jshint/jshint_wrapper.js
--rw-r--r--   0 michael   (1000) michael   (1000)    24252 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/load_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1611 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/loghandler.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    53707 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2612 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/mpi.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3221 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/mutation.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11058 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/pack.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8975 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/pathmapper.py
--rw-r--r--   0 michael   (1000) michael   (1000)    51764 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/process.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4655 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/procgenerator.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/py.typed
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.126372 cwltool-3.1.20240112164112/cwltool/rdfqueries/
--rw-r--r--   0 michael   (1000) michael   (1000)     2722 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/rdfqueries/get_inner_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2149 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/rdfqueries/get_input_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2134 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/rdfqueries/get_output_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2146 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/rdfqueries/get_root.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     3507 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/resolver.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3679 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/run_job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.126372 cwltool-3.1.20240112164112/cwltool/schemas/
--rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/CITATION
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)    20024 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.130372 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)       53 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    35108 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    33209 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      856 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       83 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/UserGuide.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    21941 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    18072 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)    42373 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/conformance_test_v1.0.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      985 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      884 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     7889 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.130372 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     3781 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.106371 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.134372 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10104 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3696 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.0/userguide-intro.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.138372 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CITATION
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)      904 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    47777 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)    36571 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      416 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    25923 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    24688 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)    93742 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/conformance_tests.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      769 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1349 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2402 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      891 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8140 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.142372 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.106371 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.146372 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10277 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.138372 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/
--rw-r--r--   0 michael   (1000) michael   (1000)       53 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    47285 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    36569 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      423 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    25411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    24564 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)      769 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      891 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8140 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.138372 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.106371 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.142372 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10277 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.150372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51493 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40072 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29004 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    29634 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1746 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2459 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.190373 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.150372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    43403 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    36600 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      293 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    26814 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.150372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.106371 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.154372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12977 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      882 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.158372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    45433 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    38245 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      293 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    27116 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1688 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.158372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.166372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.166372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    45578 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    39141 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    27124 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1688 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.166372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.170372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.174372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/
--rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CITATION
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51543 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40042 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29054 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    26611 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)    95333 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/conformance_tests.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)     1245 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.174372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.178372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.182372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/
--rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CITATION
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51543 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40064 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29054 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    29634 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)    96242 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/conformance_tests.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)     1737 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/cwl-runner.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.182372 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.186373 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2375 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/secrets.py
--rw-r--r--   0 michael   (1000) michael   (1000)    22138 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/singularity.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1094 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/singularity_utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6506 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/software_requirements.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1775 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/stdfsaccess.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9751 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/subgraph.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3669 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/task_queue.py
--rw-r--r--   0 michael   (1000) michael   (1000)      614 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/udocker.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11158 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/update.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15912 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8506 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/validate_js.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19161 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/workflow.py
--rw-r--r--   0 michael   (1000) michael   (1000)    41287 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool/workflow_job.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      613 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool-in-docker.sh
--rw-r--r--   0 michael   (1000) michael   (1000)     1366 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool.Dockerfile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.250373 cwltool-3.1.20240112164112/cwltool.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)    40543 2024-01-15 14:34:41.000000 cwltool-3.1.20240112164112/cwltool.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    41901 2024-01-15 14:34:42.000000 cwltool-3.1.20240112164112/cwltool.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-01-15 14:34:41.000000 cwltool-3.1.20240112164112/cwltool.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2024-01-15 14:34:41.000000 cwltool-3.1.20240112164112/cwltool.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-01-15 14:34:41.000000 cwltool-3.1.20240112164112/cwltool.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-01-15 14:34:41.000000 cwltool-3.1.20240112164112/cwltool.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-01-15 14:21:53.000000 cwltool-3.1.20240112164112/cwltool.egg-info/zip-safe
--rwxr-xr-x   0 michael   (1000) michael   (1000)      335 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/cwltool.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.194373 cwltool-3.1.20240112164112/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)    18134 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/CWLProv.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/Makefile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.194373 cwltool-3.1.20240112164112/docs/_static/
--rw-r--r--   0 michael   (1000) michael   (1000)    15086 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/_static/favicon.ico
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/cli.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3569 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      248 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     6674 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/loop.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/make.bat
--rw-r--r--   0 michael   (1000) michael   (1000)     7683 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/processgen.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     2510 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/pythonversions.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/docs/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       44 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/lint-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.194373 cwltool-3.1.20240112164112/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.194373 cwltool-3.1.20240112164112/mypy-stubs/arcp/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/arcp/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      788 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/arcp/parse.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1736 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/bagit.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.194373 cwltool-3.1.20240112164112/mypy-stubs/black/
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/black/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.194373 cwltool-3.1.20240112164112/mypy-stubs/coloredlogs/
--rw-r--r--   0 michael   (1000) michael   (1000)      196 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/coloredlogs/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     7565 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/mistune.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.194373 cwltool-3.1.20240112164112/mypy-stubs/prov/
--rw-r--r--   0 michael   (1000) michael   (1000)      170 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     6855 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/constants.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1721 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/dot.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1498 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/graph.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1060 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/identifier.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    15085 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/model.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.194373 cwltool-3.1.20240112164112/mypy-stubs/prov/serializers/
--rw-r--r--   0 michael   (1000) michael   (1000)     1405 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/serializers/provjson.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/serializers/provn.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     3009 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/serializers/provrdf.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      767 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/prov/serializers/provxml.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     5310 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/pydot.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.194373 cwltool-3.1.20240112164112/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8337 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.198373 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      325 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.198373 cwltool-3.1.20240112164112/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.198373 cwltool-3.1.20240112164112/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1370 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/rdflib/term.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.198373 cwltool-3.1.20240112164112/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/ruamel/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.198373 cwltool-3.1.20240112164112/mypy-stubs/shellescape/
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/shellescape/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      104 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/shellescape/main.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/mypy-stubs/spython/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.198373 cwltool-3.1.20240112164112/mypy-stubs/spython/main/
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/spython/main/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.198373 cwltool-3.1.20240112164112/mypy-stubs/spython/main/base/
--rw-r--r--   0 michael   (1000) michael   (1000)       84 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/spython/main/base/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      732 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/spython/main/build.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.198373 cwltool-3.1.20240112164112/mypy-stubs/spython/main/parse/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.198373 cwltool-3.1.20240112164112/mypy-stubs/spython/main/parse/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      363 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/spython/main/parse/parsers/base.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/spython/main/parse/parsers/docker.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      496 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/spython/main/parse/recipe.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.202373 cwltool-3.1.20240112164112/mypy-stubs/spython/main/parse/writers/
--rw-r--r--   0 michael   (1000) michael   (1000)      236 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/spython/main/parse/writers/base.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      342 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy-stubs/spython/main/parse/writers/singularity.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      258 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)      535 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/pyproject.toml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3174 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/release-test.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:34:42.250373 cwltool-3.1.20240112164112/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     6286 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)      234 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/test-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.214373 cwltool-3.1.20240112164112/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)      671 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/2.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/2.fastq
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      340 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/arg-empty-prefix-separate-false.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     3735 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/bundle-context.jsonld
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.214373 cwltool-3.1.20240112164112/tests/checker_wf/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1358 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/broken-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1350 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/broken-wf2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      776 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/broken-wf3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      255 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/broken-wf4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      196 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/cat-a.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      188 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/cat.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      543 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/circ-dep-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/circ-dep-wf2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/echo.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1283 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/functional-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      185 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/ls.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      359 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/optional_array_mismatch.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/test.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      257 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/checker_wf/wc.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.218373 cwltool-3.1.20240112164112/tests/cwl-conformance/
--rw-r--r--   0 michael   (1000) michael   (1000)     1063 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/cwl-conformance/cwltool-conftest.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      205 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/debian_image_id.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/debian_image_id2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      339 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/default_values_list.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      517 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/echo-badposition-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/echo-job.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)       14 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/echo-position-expr-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/echo-position-expr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      313 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/echo-stderr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/echo-stdout-log-dir.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      297 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/echo.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      167 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/echo_broken_outputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      280 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      285 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/env2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/env3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      360 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/env4.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      157 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/env_with_software_req.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.218373 cwltool-3.1.20240112164112/tests/input_deps/
--rw-r--r--   0 michael   (1000) michael   (1000)      202 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/input_deps/docker-array-secondaryfiles-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1081 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/input_deps/docker-array-secondaryfiles.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)    12010 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/input_deps/ref.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/input_deps/ref.fasta.fai
--rw-r--r--   0 michael   (1000) michael   (1000)    12010 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/input_deps/ref2.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/input_deps/ref2.fasta.fai
--rw-r--r--   0 michael   (1000) michael   (1000)      510 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/iwdr_bad_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      506 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/iwdr_dir_literal_real_file.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/listing-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/listing2-job.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.222373 cwltool-3.1.20240112164112/tests/loop/
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/all-output-loop-no-iteration.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      591 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/all-output-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1038 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/default-value-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      558 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-loop-command-line-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      409 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-loop-expression-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      584 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-loop-hint.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      725 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-loop-scatter.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      733 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-loop-when.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      695 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-loop-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1518 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-multi-source-loop-no-requirement.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      669 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-no-loopWhen.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      700 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-non-boolean-loopWhen.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/invalid-value-from-loop-no-requirement.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1311 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/loop-inside-loop-all.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1246 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/loop-inside-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/loop-inside-scatter-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1076 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/loop-inside-scatter.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1556 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/multi-source-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1052 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/scatter-inside-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/single-var-loop-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/single-var-loop-no-iteration.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      591 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/single-var-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      637 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/two-vars-loop-2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       11 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/two-vars-loop-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      691 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/two-vars-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      711 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/loop/value-from-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      175 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/nested-array.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      371 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/non_portable.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      406 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/non_portable2.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.222373 cwltool-3.1.20240112164112/tests/override/
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/echo-job-ov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      144 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/echo-job-ov2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/echo-job.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      211 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/echo-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      427 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/env-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      133 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/env-tool_cwl-requirement_override.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      168 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/env-tool_cwl-requirement_override_default.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      187 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/env-tool_cwl-requirement_override_default_wrongver.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      213 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/env-tool_v1.1.0-dev1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/env-tool_v1.1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      116 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/ov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      127 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/ov2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      119 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/override/ov3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      413 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/portable.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      530 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/random_lines.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      100 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/random_lines_job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/random_lines_mapping.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.222373 cwltool-3.1.20240112164112/tests/reloc/
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/reloc/test.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1063 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/scatter_numbers.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/secondary-files-bad.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/secondary-files-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      336 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/secondary-files-required-container.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      336 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/secondary-files-required-missing-container.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      369 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/secondary-files-string-v1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      609 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/secondary-files.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      430 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/seqtk_seq.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       69 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/seqtk_seq_job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      504 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/seqtk_seq_with_docker.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      539 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/seqtk_seq_wrong_name.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/sing_pullfolder_test.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.226373 cwltool-3.1.20240112164112/tests/subgraph/
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/1432.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      946 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/count-lines1-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4722 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/count-lines17-wf.cwl.json
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)      260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-tool2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-tool2_no_env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-tool2_req.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      298 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-wf2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      291 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-wf2_hint_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      295 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-wf2_hint_req_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      307 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-wf2_long.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      315 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-wf2_only_hint.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      302 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-wf2_req_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     3679 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-wf2_subwf-packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      340 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-wf2_subwf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/env-wf2_subwf_b.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1181 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_count_output.json
--rw-r--r--   0 michael   (1000) michael   (1000)     2623 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_file1.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_file2.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_file3.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_output3.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1232 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_output4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_output5.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1788 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_step1.json
--rw-r--r--   0 michael   (1000) michael   (1000)      810 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_step2.json
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_step2_1432.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_step3.json
--rw-r--r--   0 michael   (1000) michael   (1000)      861 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_step4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/extract_step5.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/parseInt-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1162 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/single_step1.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1189 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/single_step2.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1230 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/single_step3.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1245 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/single_step4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1584 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/single_step5.json
--rw-r--r--   0 michael   (1000) michael   (1000)      538 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/steplevel-resreq.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      803 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/timelimit2-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/subgraph/wc-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5329 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_anon_types.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      558 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_bad_outputs_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      376 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_check.py
--rw-r--r--   0 michael   (1000) michael   (1000)      563 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_conditionals.py
--rw-r--r--   0 michael   (1000) michael   (1000)      794 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_content_type.py
--rw-r--r--   0 michael   (1000) michael   (1000)      820 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_context.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9278 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_cuda.py
--rw-r--r--   0 michael   (1000) michael   (1000)      369 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_cwl_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)      562 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_default_path.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5625 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_dependencies.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/tests/test_deps_env/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/tests/test_deps_env/modulefiles/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.226373 cwltool-3.1.20240112164112/tests/test_deps_env/modulefiles/random-lines/
--rw-r--r--   0 michael   (1000) michael   (1000)      523 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_deps_env/modulefiles/random-lines/1.0
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/tests/test_deps_env/random-lines/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.226373 cwltool-3.1.20240112164112/tests/test_deps_env/random-lines/1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)      355 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_deps_env/random-lines/1.0/env.sh
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.230373 cwltool-3.1.20240112164112/tests/test_deps_env/random-lines/1.0/scripts/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2300 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_deps_env/random-lines/1.0/scripts/random-lines
--rw-r--r--   0 michael   (1000) michael   (1000)       55 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_deps_env_modules_resolvers_conf.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_deps_env_resolvers_conf.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_deps_env_resolvers_conf_rewrite.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      101 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_deps_mapping.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     7703 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_docker.py
--rw-r--r--   0 michael   (1000) michael   (1000)      414 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_docker_info.py
--rw-r--r--   0 michael   (1000) michael   (1000)      845 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_docker_paths_with_colons.py
--rw-r--r--   0 michael   (1000) michael   (1000)      513 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_empty_input.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8325 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_environment.py
--rw-r--r--   0 michael   (1000) michael   (1000)    64197 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_examples.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7610 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_ext.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2533 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_fetch.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2487 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_http_input.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4335 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_input_deps.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10931 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_iwdr.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4459 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_js_sandbox.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6990 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_load_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9408 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_loop.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1302 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_main_parsed_args.py
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_make_template.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2761 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_misc_cli.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11904 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_mpi.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3979 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_override.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7708 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_pack.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1126 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_parallel.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6158 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_path_checks.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2682 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_pathmapper.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1382 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_procgenerator.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28315 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_provenance.py
--rw-r--r--   0 michael   (1000) michael   (1000)      589 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_rdfprint.py
--rw-r--r--   0 michael   (1000) michael   (1000)      526 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_recursive_validation.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_relocate.py
--rw-r--r--   0 michael   (1000) michael   (1000)      319 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_schemadef.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3034 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_secrets.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4596 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_singularity.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4457 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_singularity_versions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1870 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_stdout_stderr_log_dir.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2725 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_streaming.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2289 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_subclass_mypyc.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11067 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_subgraph.py
--rw-r--r--   0 michael   (1000) michael   (1000)      936 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_target.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11937 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_tmpdir.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5693 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_toolargparse.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4342 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_trs.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3579 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_udocker.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1881 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_validate.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2170 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_validate_js.py
--rw-r--r--   0 michael   (1000) michael   (1000)      867 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/test_windows_warning.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/tests/tmp1/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/tests/tmp1/tmp2/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.230373 cwltool-3.1.20240112164112/tests/tmp1/tmp2/tmp3/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/tmp1/tmp2/tmp3/.gitkeep
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.110371 cwltool-3.1.20240112164112/tests/tmp4/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.230373 cwltool-3.1.20240112164112/tests/tmp4/alpha/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/tmp4/alpha/baker
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/tmp4/alpha/charlie
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/tmp4/alpha/delta
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/tmp4/alpha/echo
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/tmp4/alpha/foxtrot
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.230373 cwltool-3.1.20240112164112/tests/trs/
--rw-r--r--   0 michael   (1000) michael   (1000)     1505 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/trs/Dockstore.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/trs/md5sum-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/trs/md5sum-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/utf_doc_example.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/util.py
--rw-r--r--   0 michael   (1000) michael   (1000)      236 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wc-tool-bad-hints.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wc-tool-bad-reqs.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.250373 cwltool-3.1.20240112164112/tests/wf/
--rw-r--r--   0 michael   (1000) michael   (1000)      286 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/1496.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      468 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/1590.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      373 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/1st-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       51 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/1st-workflow_bad_inputs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      181 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/811-12.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/811.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       26 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/811_inputs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      212 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/816_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/816_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      650 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/910.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/arguments.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      254 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/bad-stderr-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      225 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/bad-stdin-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/bad-stdout-expr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      523 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/bad_formattest.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/bad_formattest2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      222 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/bad_networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/bad_timelimit.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/badout1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      304 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/badout2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/badout3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      272 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/cache_test_workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/cat-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      130 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/cat.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/conditional_step_no_inputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      577 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/conflict.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      266 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/cores_float.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      388 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/count-lines1-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      409 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/default-dir5.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/default-wf5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      212 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/default_path.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      210 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/dir_deps.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1479 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/directory.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1420 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/double-nested.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/empty.ttl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/empty2.ttl
--rw-r--r--   0 michael   (1000) michael   (1000)      922 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/expect_iwd-passthrough1_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4397 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/expect_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4564 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/expect_revsort_datetime_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4574 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/expect_trick_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1262 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/extract_region_specs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      619 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/floats_small_and_large.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      120 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/formattest-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      412 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/formattest.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.250373 cwltool-3.1.20240112164112/tests/wf/generator/
--rw-r--r--   0 michael   (1000) michael   (1000)      710 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/generator/pytoolgen.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      275 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/generator/zing.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      672 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/hello-workflow-badhints.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      673 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/hello-workflow-badhints2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      657 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/hello-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/hello.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/hello_single_tool.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.250373 cwltool-3.1.20240112164112/tests/wf/indir/
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/indir/hello2.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      213 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/input_named_id.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       37 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/input_named_id.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      580 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/iwd-passthrough1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      230 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/iwdr-empty.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      414 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/iwdr-entry.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1775 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/iwdr-passthrough-successive.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2268 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/iwdr_permutations.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/iwdr_permutations_inplace.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1016 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/iwdr_permutations_nocontainer.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      284 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/js_output.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      364 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/js_output_workflow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      291 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/listing_deep.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      276 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/listing_none.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/listing_shallow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      158 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/listing_v1_0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/literalfile-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/literalfile.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/malformed_outputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/missing-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      548 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/missing_cwlVersion.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      249 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/mpi_env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      645 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/mpi_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/mpi_expr.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      401 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/mpi_line_count.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      471 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/mpi_simple.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      640 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/mpi_simple_wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/mut.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/mut2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      281 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/mut3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1107 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/nested.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/networkaccess-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      425 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/no-parameters-echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/nvidia-smi-cc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      434 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/nvidia-smi-container.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/nvidia-smi-max.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      408 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/nvidia-smi-range.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      429 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/nvidia-smi.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-01-15 14:34:42.250373 cwltool-3.1.20240112164112/tests/wf/operation/
--rw-r--r--   0 michael   (1000) michael   (1000)      442 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/operation/abstract-cosifer.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5209 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/operation/expect_operation-single_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      969 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/operation/operation-single.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      337 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/optional-numerical-output-0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      174 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/optional_src_mandatory_sink.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      221 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/override-no-secrets.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1921 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/packed-with-loadlisting.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1056 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/packed_no_main.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      786 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/paramref_arguments_roundtrip.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      877 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/paramref_arguments_self.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/parseInt-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      984 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/record_outputeval.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/resreq_expr_float_v1_0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/resreq_expr_float_v1_2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      181 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/revsort-job-shortcut.json
--rw-r--r--   0 michael   (1000) michael   (1000)      152 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/revsort-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2331 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/revsort.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2447 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/revsort_datetime.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2317 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/revsort_step_bad_schema.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1367 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/revtool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1471 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/revtool_bad_schema.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       62 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/scatter-job2.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      927 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/scatter-wf4.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2999 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/scatter-wf4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1563 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/scatter2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1805 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/scatter2_subwf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      703 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/scatterfail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)    94112 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/schemadef-bug-1473.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/schemadef-tool-12.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/schemadef-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      158 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/schemadef-type.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      163 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/sec-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      948 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/sec-wf-out.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      214 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/sec-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      403 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/secret_job.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      380 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/secret_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      363 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/separate_without_prefix.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1101 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/sorttool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      391 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/storage_float.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/tar-param.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1124 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/three_step_color.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      222 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/timelimit-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      277 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/timelimit.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      304 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/touch_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      278 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/trick_defaults.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      260 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/trick_defaults2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2400 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/trick_revsort.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      318 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/updatedir.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      431 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/updatedir_inplace.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      488 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/updateval.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      102 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/updateval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      603 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/updateval_inplace.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/vf-concat.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/wc-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/wc-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      639 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/wffail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1111 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/whale.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      329 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/workreuse-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      392 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/workreuse.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      565 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/wf/wrong_cwlVersion.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      150 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/with_doc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tests/without_doc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2074 2024-01-15 14:21:15.000000 cwltool-3.1.20240112164112/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/
+-rw-r--r--   0 michael   (1000) michael   (1000)       40 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.codecov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.coveragerc
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.dockerignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      224 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.flake8
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.git-blame-ignore-revs
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.gitattributes
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.524123 cwltool-3.1.20240404144621/.github/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.524123 cwltool-3.1.20240404144621/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 michael   (1000) michael   (1000)      143 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      643 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/dependabot.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.528123 cwltool-3.1.20240404144621/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     9031 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/workflows/ci-tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      699 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2030 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.github/workflows/quay-publish.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      593 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      734 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.mergify.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      512 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.readthedocs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      385 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/.snyk
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     4343 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3181 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     7313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)    40543 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    38143 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/README.rst
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1084 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/build-cwltool-docker.sh
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6535 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/conformance-test.sh
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      280 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwl-docker.sh
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.528123 cwltool-3.1.20240404144621/cwlref-runner/
+-rw-r--r--   0 michael   (1000) michael   (1000)      223 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwlref-runner/README
+-rw-r--r--   0 michael   (1000) michael   (1000)      771 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwlref-runner/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.532123 cwltool-3.1.20240404144621/cwltool/
+-rw-r--r--   0 michael   (1000) michael   (1000)      280 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       81 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool/_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30804 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/argparser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29616 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/builder.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    21296 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/checker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    66095 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/command_line_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9184 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2341 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cuda.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/cwlprov/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5140 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1887 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/provenance_constants.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    32949 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/provenance_profile.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23846 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/ro.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10899 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlprov/writablebagfile.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6398 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlrdf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7318 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/cwlviewer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    18656 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/docker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4283 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/docker_id.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/env_to_stdout.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      346 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    20003 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/executors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4161 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/extensions-v1.1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     8565 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/extensions-v1.2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     7404 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/extensions.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2402 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/factory.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      704 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/flatten.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4127 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/hello.simg
+-rw-r--r--   0 michael   (1000) michael   (1000)    40577 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/jshint/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  1286196 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/jshint/jshint.js
+-rw-r--r--   0 michael   (1000) michael   (1000)     1240 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/jshint/jshint_wrapper.js
+-rw-r--r--   0 michael   (1000) michael   (1000)    24252 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/load_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1612 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/loghandler.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    54334 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2613 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/mpi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3221 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/mutation.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11058 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/pack.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8975 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/pathmapper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    51808 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/process.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4655 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/procgenerator.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/py.typed
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/rdfqueries/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2722 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/rdfqueries/get_inner_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2149 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/rdfqueries/get_input_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2134 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/rdfqueries/get_output_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2146 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/rdfqueries/get_root.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     3507 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/resolver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3680 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/run_job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/schemas/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/CITATION
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)    20024 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.536123 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    35108 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    33209 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      856 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       83 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/UserGuide.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    21941 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    18072 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    42373 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/conformance_test_v1.0.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      985 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      884 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     7889 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.540123 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3781 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.540123 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10104 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3696 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.0/userguide-intro.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.544123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CITATION
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      904 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    47777 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)    36571 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      416 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    25923 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    24688 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    93742 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/conformance_tests.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      769 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1349 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2402 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      891 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8140 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.548123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.552124 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10277 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.544123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    47285 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    36569 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      423 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    25411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    24564 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      769 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      891 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8140 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.544123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.548123 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10277 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.552124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40072 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29004 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    29634 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1746 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2459 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.584124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.556124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    43403 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    36600 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      293 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    26814 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.556124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.560124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12977 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      882 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.560124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    45433 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    38245 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      293 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    27116 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1688 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.560124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.564124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.564124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    45578 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    39141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    27124 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1688 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.564124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.568124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.572124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CITATION
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51543 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40042 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29054 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    26611 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    95333 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/conformance_tests.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1245 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.572124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.576124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.576124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1141 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CITATION
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51543 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40064 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29054 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    29634 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    96242 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/conformance_tests.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1737 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1356 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/cwl-runner.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.576124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.516123 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.580124 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2376 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/secrets.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    22137 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/singularity.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1094 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/singularity_utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6506 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/software_requirements.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1775 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/stdfsaccess.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9751 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/subgraph.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3695 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/task_queue.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      614 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/udocker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11158 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/update.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15913 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8506 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/validate_js.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19161 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/workflow.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    41287 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool/workflow_job.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      613 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool-in-docker.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)     1366 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool.Dockerfile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/cwltool.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    40543 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    41948 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       45 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-04-10 13:22:11.000000 cwltool-3.1.20240404144621/cwltool.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 13:21:18.000000 cwltool-3.1.20240404144621/cwltool.egg-info/zip-safe
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      335 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/cwltool.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)    18134 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/CWLProv.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/Makefile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/docs/_static/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15086 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/_static/favicon.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/cli.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3569 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      248 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     6674 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/loop.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/make.bat
+-rw-r--r--   0 michael   (1000) michael   (1000)     7683 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/processgen.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     2510 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/pythonversions.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/docs/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/lint-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/arcp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/arcp/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      788 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/arcp/parse.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1736 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/bagit.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/black/
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/black/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/coloredlogs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      196 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/coloredlogs/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     7565 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/mistune.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/prov/
+-rw-r--r--   0 michael   (1000) michael   (1000)      170 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     6855 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/constants.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1721 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/dot.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1498 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/graph.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1060 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/identifier.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    15085 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/model.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.588124 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1405 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provjson.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provn.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     3009 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provrdf.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      767 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provxml.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     5310 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/pydot.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8337 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      325 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1370 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/rdflib/term.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/ruamel/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/shellescape/
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/shellescape/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/shellescape/main.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/mypy-stubs/spython/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/spython/main/
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/spython/main/base/
+-rw-r--r--   0 michael   (1000) michael   (1000)       84 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/base/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      732 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/build.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.592124 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.596125 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      363 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/parsers/base.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/parsers/docker.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      496 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/recipe.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.596125 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/writers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      236 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/writers/base.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      342 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy-stubs/spython/main/parse/writers/singularity.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      258 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)      535 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/pyproject.toml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3178 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/release-test.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     6934 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      359 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/test-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.608125 cwltool-3.1.20240404144621/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)      671 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/2.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/2.fastq
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      340 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/arg-empty-prefix-separate-false.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     3735 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/bundle-context.jsonld
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.608125 cwltool-3.1.20240404144621/tests/checker_wf/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1358 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/broken-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1350 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/broken-wf2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      776 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/broken-wf3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      255 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/broken-wf4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      196 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/cat-a.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      188 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/cat.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      543 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/circ-dep-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/circ-dep-wf2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/echo.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1283 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/functional-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      185 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/ls.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      359 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/optional_array_mismatch.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/test.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      257 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/checker_wf/wc.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.608125 cwltool-3.1.20240404144621/tests/cwl-conformance/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1064 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/cwl-conformance/cwltool-conftest.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      205 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/debian_image_id.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/debian_image_id2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      339 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/default_values_list.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      517 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-badposition-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-job.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)       14 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-position-expr-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-position-expr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      313 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-stderr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo-stdout-log-dir.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      297 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      167 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/echo_broken_outputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      280 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      285 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      360 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env4.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      157 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/env_with_software_req.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.608125 cwltool-3.1.20240404144621/tests/input_deps/
+-rw-r--r--   0 michael   (1000) michael   (1000)      202 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/docker-array-secondaryfiles-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1081 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/docker-array-secondaryfiles.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)    12010 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/ref.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/ref.fasta.fai
+-rw-r--r--   0 michael   (1000) michael   (1000)    12010 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/ref2.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/input_deps/ref2.fasta.fai
+-rw-r--r--   0 michael   (1000) michael   (1000)      510 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/iwdr_bad_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      506 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/iwdr_dir_literal_real_file.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/listing-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/listing2-job.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.612125 cwltool-3.1.20240404144621/tests/loop/
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/all-output-loop-no-iteration.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      591 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/all-output-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1038 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/default-value-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      558 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-command-line-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      409 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-expression-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-hint.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      725 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-scatter.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      733 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-when.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      695 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-loop-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1518 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-multi-source-loop-no-requirement.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      669 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-no-loopWhen.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      700 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-non-boolean-loopWhen.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/invalid-value-from-loop-no-requirement.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1311 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/loop-inside-loop-all.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1246 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/loop-inside-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/loop-inside-scatter-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1076 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/loop-inside-scatter.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1556 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/multi-source-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1052 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/scatter-inside-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/single-var-loop-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/single-var-loop-no-iteration.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      591 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/single-var-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      637 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/two-vars-loop-2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       11 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/two-vars-loop-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      691 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/two-vars-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      711 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/loop/value-from-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      175 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/nested-array.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      371 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/non_portable.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      406 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/non_portable2.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.616125 cwltool-3.1.20240404144621/tests/override/
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo-job-ov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      144 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo-job-ov2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo-job.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      211 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      427 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      133 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_cwl-requirement_override.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      168 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_cwl-requirement_override_default.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      187 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_cwl-requirement_override_default_wrongver.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      213 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_v1.1.0-dev1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/env-tool_v1.1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      116 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/ov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      127 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/ov2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      119 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/override/ov3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      413 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/portable.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      530 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/random_lines.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      100 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/random_lines_job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/random_lines_mapping.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.616125 cwltool-3.1.20240404144621/tests/reloc/
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/reloc/test.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1063 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/scatter_numbers.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-bad.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       45 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      336 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-required-container.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      336 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-required-missing-container.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      369 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files-string-v1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      609 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/secondary-files.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      432 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/seqtk_seq.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       69 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/seqtk_seq_job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      513 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/seqtk_seq_with_docker.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      539 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/seqtk_seq_wrong_name.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/sing_pullfolder_test.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/subgraph/
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/1432.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      946 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/count-lines1-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4722 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/count-lines17-wf.cwl.json
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-tool2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-tool2_no_env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-tool2_req.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      298 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      291 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_hint_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      295 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_hint_req_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      307 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_long.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      315 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_only_hint.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      302 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_req_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     3679 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_subwf-packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      340 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_subwf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/env-wf2_subwf_b.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1181 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_count_output.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     2623 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_file1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_file2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_file3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_output3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_output4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_output5.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1788 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      810 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step2_1432.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      861 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/extract_step5.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/parseInt-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1162 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1189 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1230 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1245 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1584 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/single_step5.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/steplevel-resreq.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      803 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/timelimit2-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/subgraph/wc-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5329 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_anon_types.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      558 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_bad_outputs_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_check.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_conditionals.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      794 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_content_type.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      820 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9278 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_cuda.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      369 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_cwl_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      562 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_default_path.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5684 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_dependencies.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/test_deps_env/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/test_deps_env/modulefiles/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/test_deps_env/modulefiles/random-lines/
+-rw-r--r--   0 michael   (1000) michael   (1000)      523 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env/modulefiles/random-lines/1.0
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)      355 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/env.sh
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/scripts/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2300 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/scripts/random-lines
+-rw-r--r--   0 michael   (1000) michael   (1000)       55 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env_modules_resolvers_conf.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env_resolvers_conf.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_env_resolvers_conf_rewrite.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      101 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_deps_mapping.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     8162 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_docker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      414 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_docker_info.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      845 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_docker_paths_with_colons.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      513 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_empty_input.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8326 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_environment.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    64197 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_examples.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7610 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_ext.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2533 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_fetch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2487 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_http_input.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4335 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_input_deps.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10932 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_iwdr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4466 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_js_sandbox.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6991 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_load_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9409 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_loop.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1302 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_main_parsed_args.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_make_template.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2761 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_misc_cli.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11905 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_mpi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3979 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_override.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7708 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_pack.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1126 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_parallel.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6158 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_path_checks.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2682 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_pathmapper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1382 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_procgenerator.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28315 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_provenance.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      589 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_rdfprint.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      527 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_recursive_validation.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_relocate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      319 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_schemadef.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3034 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_secrets.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4597 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_singularity.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4458 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_singularity_versions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1870 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_stdout_stderr_log_dir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2726 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_streaming.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_subclass_mypyc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11067 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_subgraph.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      936 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_target.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11938 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_tmpdir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5693 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_toolargparse.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4342 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_trs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3580 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_udocker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      746 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_user_agent.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1882 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_validate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2170 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_validate_js.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      867 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/test_windows_warning.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/tmp1/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/tmp1/tmp2/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/tmp1/tmp2/tmp3/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp1/tmp2/tmp3/.gitkeep
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.520123 cwltool-3.1.20240404144621/tests/tmp4/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/tmp4/alpha/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/baker
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/charlie
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/delta
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/echo
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/tmp4/alpha/foxtrot
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.620125 cwltool-3.1.20240404144621/tests/trs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1505 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/trs/Dockstore.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/trs/md5sum-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/trs/md5sum-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/utf_doc_example.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5261 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/util.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      236 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wc-tool-bad-hints.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wc-tool-bad-reqs.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/tests/wf/
+-rw-r--r--   0 michael   (1000) michael   (1000)      286 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/1496.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      468 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/1590.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      373 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/1st-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       51 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/1st-workflow_bad_inputs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      181 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/811-12.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/811.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       26 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/811_inputs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      212 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/816_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/816_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      650 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/910.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/arguments.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      254 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad-stderr-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      225 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad-stdin-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad-stdout-expr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      523 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad_formattest.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad_formattest2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      222 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad_networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/bad_timelimit.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/badout1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      304 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/badout2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/badout3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      272 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/cache_test_workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/cat-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      130 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/cat.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/conditional_step_no_inputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      577 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/conflict.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      266 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/cores_float.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      388 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/count-lines1-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      409 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/default-dir5.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/default-wf5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      212 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/default_path.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      210 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/dir_deps.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1479 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/directory.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1420 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/double-nested.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/empty.ttl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/empty2.ttl
+-rw-r--r--   0 michael   (1000) michael   (1000)      922 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/expect_iwd-passthrough1_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4397 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/expect_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4564 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/expect_revsort_datetime_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4574 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/expect_trick_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1262 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/extract_region_specs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      619 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/floats_small_and_large.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      120 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/formattest-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      412 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/formattest.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/tests/wf/generator/
+-rw-r--r--   0 michael   (1000) michael   (1000)      710 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/generator/pytoolgen.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      275 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/generator/zing.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      672 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello-workflow-badhints.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      673 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello-workflow-badhints2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      657 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/hello_single_tool.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/tests/wf/indir/
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/indir/hello2.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      213 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/input_named_id.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       37 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/input_named_id.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      580 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwd-passthrough1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      230 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr-empty.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      414 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr-entry.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1775 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr-passthrough-successive.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2268 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr_permutations.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr_permutations_inplace.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1016 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/iwdr_permutations_nocontainer.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      284 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/js_output.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      364 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/js_output_workflow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      291 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/listing_deep.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      276 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/listing_none.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/listing_shallow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      158 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/listing_v1_0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/literalfile-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/literalfile.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/malformed_outputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/missing-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      548 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/missing_cwlVersion.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      249 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      645 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_expr.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      401 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_line_count.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      471 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_simple.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      640 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mpi_simple_wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mut.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mut2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      281 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/mut3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1107 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nested.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/networkaccess-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      425 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/no-parameters-echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi-cc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      434 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi-container.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi-max.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      408 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi-range.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      429 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/nvidia-smi.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:22:11.640125 cwltool-3.1.20240404144621/tests/wf/operation/
+-rw-r--r--   0 michael   (1000) michael   (1000)      442 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/operation/abstract-cosifer.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5209 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/operation/expect_operation-single_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      969 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/operation/operation-single.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      337 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/optional-numerical-output-0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      174 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/optional_src_mandatory_sink.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      221 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/override-no-secrets.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1921 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/packed-with-loadlisting.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1056 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/packed_no_main.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      786 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/paramref_arguments_roundtrip.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      877 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/paramref_arguments_self.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/parseInt-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      984 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/record_outputeval.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/resreq_expr_float_v1_0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/resreq_expr_float_v1_2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      181 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort-job-shortcut.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      152 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2331 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2447 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort_datetime.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2317 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revsort_step_bad_schema.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1367 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revtool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1471 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/revtool_bad_schema.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       62 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter-job2.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      927 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter-wf4.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2999 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter-wf4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1563 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1805 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatter2_subwf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      703 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/scatterfail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)    94112 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/schemadef-bug-1473.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/schemadef-tool-12.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/schemadef-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      158 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/schemadef-type.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      163 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/sec-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      948 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/sec-wf-out.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      214 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/sec-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      403 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/secret_job.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      380 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/secret_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      363 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/separate_without_prefix.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      233 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/shm_size.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1101 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/sorttool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      391 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/storage_float.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/tar-param.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1124 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/three_step_color.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      222 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/timelimit-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      277 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/timelimit.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      304 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/touch_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      278 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/trick_defaults.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      260 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/trick_defaults2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2400 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/trick_revsort.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      318 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updatedir.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      431 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updatedir_inplace.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      488 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updateval.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      102 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updateval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      603 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/updateval_inplace.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/vf-concat.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/wc-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/wc-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      639 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/wffail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1111 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/whale.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      329 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/workreuse-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      392 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/workreuse.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      565 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/wf/wrong_cwlVersion.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      150 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/with_doc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tests/without_doc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2094 2024-04-10 13:20:47.000000 cwltool-3.1.20240404144621/tox.ini
```

### Comparing `cwltool-3.1.20240112164112/.github/ISSUE_TEMPLATE.md` & `cwltool-3.1.20240404144621/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/.github/dependabot.yml` & `cwltool-3.1.20240404144621/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/.github/workflows/ci-tests.yml` & `cwltool-3.1.20240404144621/.github/workflows/ci-tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -67,28 +67,29 @@
       - name: Upgrade setuptools and install tox
         run: |
           pip install -U pip setuptools wheel
           pip install "tox<4" "tox-gh-actions<3"
 
       - name: MyPy cache
         if: ${{ matrix.step == 'mypy' }}
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: .mypy_cache/${{ env.py-semver }}
           key: mypy-${{ env.py-semver }}
 
       - name: Test with tox
         run: APPTAINER_TMPDIR=${RUNNER_TEMP} tox
 
       - name: Upload coverage to Codecov
         if: ${{ matrix.step == 'unit' }}
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
-          fail_ci_if_error: false
-          token: ${{ secrets.CODECOV_TOKEN }}
+          fail_ci_if_error: true
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
 
   tox-style:
     name: Linters
     runs-on: ubuntu-20.04
 
     strategy:
       matrix:
@@ -180,15 +181,15 @@
         if: ${{ matrix.container == 'singularity' }}
         run: |
           wget --no-verbose https://github.com/sylabs/singularity/releases/download/v3.10.4/singularity-ce_3.10.4-jammy_amd64.deb
           sudo apt-get install -y ./singularity-ce_3.10.4-jammy_amd64.deb
 
       - name: Singularity cache
         if: ${{ matrix.container == 'singularity' }}
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: sifcache
           key: singularity
 
       - name: Set up Podman
         if: ${{ matrix.container == 'podman' }}
         run: sudo rm -f /usr/bin/docker ; sudo apt-get install -y podman
@@ -209,18 +210,19 @@
       - name: Archive test results
         uses: actions/upload-artifact@v4
         with:
           name: cwl-${{ matrix.cwl-version }}-${{ matrix.container }}${{ matrix.extras }}-conformance-results
           path: |
             **/cwltool_conf*.xml
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
-          fail_ci_if_error: false
-          token: ${{ secrets.CODECOV_TOKEN }}
+          fail_ci_if_error: true
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
   release_test:
     name: cwltool release test
     runs-on: ubuntu-22.04
 
     steps:
       - uses: actions/checkout@v4
 
@@ -281,23 +283,24 @@
             tox.ini
       - name: Upgrade setuptools and install tox
         run: |
           pip install -U pip setuptools wheel
           pip install "tox<4" "tox-gh-actions<3"
       # # docker for mac install is not currently stable
       # - name: 'SETUP MacOS: load Homebrew cache'
-      #   uses: actions/cache@v3
+      #   uses: actions/cache@v4
       #   if: runner.os == 'macOS'
       #   with:
       #      path: |
       #        ~/Library/Caches/Homebrew/downloads/*--Docker.dmg
       #      key: brew-actions-setup-docker-1.0.11
       #      restore-keys: brew-actions-setup-docker-
       # - name: setup docker on macos (default stable version)
       #   uses: docker-practice/actions-setup-docker@master
       - name: Test with tox
         run: tox
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
-          fail_ci_if_error: false
-          token: ${{ secrets.CODECOV_TOKEN }}
+          fail_ci_if_error: true
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `cwltool-3.1.20240112164112/.github/workflows/codeql-analysis.yml` & `cwltool-3.1.20240404144621/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/.github/workflows/quay-publish.yml` & `cwltool-3.1.20240404144621/.github/workflows/quay-publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           pip install setuptools_scm[toml] wheel
           python setup.py --version
       - name: Set up QEMU
         uses: docker/setup-qemu-action@v3
       - name: Set up Docker Buildx
         uses: docker/setup-buildx-action@v3
       - name: Cache Docker layers
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: /tmp/.buildx-cache
           key: ${{ runner.os }}-multi-buildx-${{ github.sha }}
           restore-keys: |
             ${{ runner.os }}-multi-buildx
       - name: Login to Quay.io
         uses: docker/login-action@v3
```

### Comparing `cwltool-3.1.20240112164112/.gitignore` & `cwltool-3.1.20240404144621/.gitignore`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/.mergify.yml` & `cwltool-3.1.20240404144621/.mergify.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/.readthedocs.yml` & `cwltool-3.1.20240404144621/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240404144621/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/CONTRIBUTING.md` & `cwltool-3.1.20240404144621/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/LICENSE.txt` & `cwltool-3.1.20240404144621/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/MANIFEST.in` & `cwltool-3.1.20240404144621/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/Makefile` & `cwltool-3.1.20240404144621/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -68,30 +68,26 @@
 dev: install-dep
 	pip install -e .[deps]
 
 
 ## dist                   : create a module package for distribution
 dist: dist/${MODULE}-$(VERSION).tar.gz
 
-check-python3:
-# Check that the default python version is python 3
-	python --version 2>&1 | grep "Python 3"
-
-dist/${MODULE}-$(VERSION).tar.gz: check-python3 $(SOURCES)
-	python -m build
+dist/${MODULE}-$(VERSION).tar.gz: $(SOURCES)
+	python3 -m build
 
 ## docs                   : make the docs
 docs: FORCE
 	cd docs && $(MAKE) html
 
 ## clean                  : clean up all temporary / machine-generated files
-clean: check-python3 FORCE
+clean: FORCE
 	rm -f ${MODULE}/*.pyc tests/*.pyc *.so ${MODULE}/*.so cwltool/cwlprov/*.so
 	rm -Rf ${MODULE}/__pycache__/
-	python setup.py clean --all || true
+	rm -Rf build
 	rm -Rf .coverage
 	rm -f diff-cover.html
 
 # Linting and code style related targets
 ## sort_import            : sorting imports using isort: https://github.com/timothycrosley/isort
 sort_imports: $(PYSOURCES) mypy-stubs
 	isort $^
@@ -159,20 +155,20 @@
 diff-cover: coverage.xml
 	diff-cover --compare-branch=main $^
 
 diff-cover.html: coverage.xml
 	diff-cover --compare-branch=main $^ --html-report $@
 
 ## test                   : run the cwltool test suite
-test: check-python3 $(PYSOURCES)
-	python -m pytest -rs ${PYTEST_EXTRA}
+test: $(PYSOURCES)
+	python3 -m pytest -rs ${PYTEST_EXTRA}
 
 ## testcov                : run the cwltool test suite and collect coverage
-testcov: check-python3 $(PYSOURCES)
-	python -m pytest -rs --cov --cov-config=.coveragerc --cov-report= ${PYTEST_EXTRA}
+testcov: $(PYSOURCES)
+	python3 -m pytest -rs --cov --cov-config=.coveragerc --cov-report= ${PYTEST_EXTRA}
 
 sloccount.sc: $(PYSOURCES) Makefile
 	sloccount --duplicates --wide --details $^ > $@
 
 ## sloccount              : count lines of code
 sloccount: $(PYSOURCES) Makefile
 	sloccount $^
@@ -193,24 +189,24 @@
 	shellcheck build-cwltool-docker.sh cwl-docker.sh release-test.sh conformance-test.sh \
 		cwltool-in-docker.sh
 
 pyupgrade: $(PYSOURCES)
 	pyupgrade --exit-zero-even-if-changed --py38-plus $^
 	auto-walrus $^
 
-release-test: check-python3 FORCE
+release-test: FORCE
 	git diff-index --quiet HEAD -- || ( echo You have uncommitted changes, please commit them and try again; false )
 	./release-test.sh
 
 release:
 	export SETUPTOOLS_SCM_PRETEND_VERSION_FOR_CWLTOOL=${VERSION} && \
 	./release-test.sh && \
 	. testenv2/bin/activate && \
 		pip install build && \
-		python -m build testenv2/src/${MODULE} && \
+		python3 -m build testenv2/src/${MODULE} && \
 		pip install twine && \
 		twine upload testenv2/src/${MODULE}/dist/* && \
 		git tag ${VERSION} && git push --tags
 
 flake8: $(PYSOURCES)
 	flake8 $^
```

### Comparing `cwltool-3.1.20240112164112/PKG-INFO` & `cwltool-3.1.20240404144621/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltool
-Version: 3.1.20240112164112
+Version: 3.1.20240404144621
 Summary: Common workflow language reference implementation
 Home-page: https://github.com/common-workflow-language/cwltool
 Download-URL: https://github.com/common-workflow-language/cwltool
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -46,16 +46,16 @@
 Requires-Dist: coloredlogs
 Requires-Dist: pydot>=1.4.1
 Requires-Dist: argcomplete
 Requires-Dist: pyparsing!=3.0.2
 Requires-Dist: cwl-utils>=0.32
 Requires-Dist: spython>=0.3.0
 Provides-Extra: deps
-Requires-Dist: galaxy-tool-util!=23.0.1,!=23.0.2,!=23.0.3,!=23.0.4,!=23.0.5,<23.2,>=22.1.2; extra == "deps"
-Requires-Dist: galaxy-util<23.2; extra == "deps"
+Requires-Dist: galaxy-tool-util!=23.0.1,!=23.0.2,!=23.0.3,!=23.0.4,!=23.0.5,<24.1,>=22.1.2; extra == "deps"
+Requires-Dist: galaxy-util<24.1; extra == "deps"
 
 #############################################################################################
 ``cwltool``: The reference reference implementation of the Common Workflow Language standards
 #############################################################################################
 
 |Linux Status| |Coverage Status| |Docs Status|
```

### Comparing `cwltool-3.1.20240112164112/README.rst` & `cwltool-3.1.20240404144621/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/build-cwltool-docker.sh` & `cwltool-3.1.20240404144621/build-cwltool-docker.sh`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/conformance-test.sh` & `cwltool-3.1.20240404144621/conformance-test.sh`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
    echo 'Skip installing dependencies; cwltool & cwltest must already be installed'
 else
 	venv "${TMP_DIR}/cwl-conformance-venv"
 	pip install -U setuptools wheel pip
 	pip uninstall -y cwltool
 	pip install -r"${SCRIPT_DIRECTORY}/mypy-requirements.txt"
 	CWLTOOL_USE_MYPYC=1 MYPYPATH="${SCRIPT_DIRECTORY}/mypy-stubs" pip install "${SCRIPT_DIRECTORY}" -r"${SCRIPT_DIRECTORY}/requirements.txt"
-	pip install 'cwltest>=2.3' pytest-cov pytest-xdist
+	pip install 'cwltest>=2.5' pytest-cov pytest-xdist>=3.2.0 psutil
 fi
 
 # Set conformance test filename
 if [[ "${VERSION}" = "v1.0" ]] ; then
   CONFORMANCE_TEST="${TMP_DIR}/${REPO}-${GIT_TARGET}/${VERSION}/conformance_test_v1.0.yaml"
 else
   CONFORMANCE_TEST="${TMP_DIR}/${REPO}-${GIT_TARGET}/conformance_tests.yaml"
@@ -117,15 +117,15 @@
     EXCLUDE="${EXCLUDE},"
 fi
 if (( "${#exclusions[*]}" > 0 )); then
     EXCLUDE=${EXCLUDE}$(IFS=,; echo "${exclusions[*]}")
 fi
 
 # Build command
-TEST_COMMAND="python -m pytest ${CONFORMANCE_TEST} -n auto -rs --junit-xml=${TMP_DIR}/cwltool_conf_${VERSION}_${GIT_TARGET}_${CONTAINER}.xml -o junit_suite_name=cwltool_$(echo "${CWLTOOL_OPTIONS}" | tr "[:blank:]-" _)"
+TEST_COMMAND="python -m pytest ${CONFORMANCE_TEST} -n logical --dist worksteal -rs --junit-xml=${TMP_DIR}/cwltool_conf_${VERSION}_${GIT_TARGET}_${CONTAINER}.xml -o junit_suite_name=cwltool_$(echo "${CWLTOOL_OPTIONS}" | tr "[:blank:]-" _)"
 if [[ -n "${EXCLUDE}" ]] ; then
   TEST_COMMAND="${TEST_COMMAND} --cwl-exclude ${EXCLUDE}"
 fi
 if [ -v SKIP_COV ] ; then
 	echo Skipping gathering of coverage information
 else
 	TEST_COMMAND="${TEST_COMMAND} --cov --cov-config ${SCRIPT_DIRECTORY}/.coveragerc --cov-report= ${PYTEST_EXTRA}"
```

### Comparing `cwltool-3.1.20240112164112/cwlref-runner/setup.py` & `cwltool-3.1.20240404144621/cwlref-runner/setup.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/argparser.py` & `cwltool-3.1.20240404144621/cwltool/argparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         "respective fields or capture it as an output",
     )
 
     parser.add_argument(
         "--parallel",
         action="store_true",
         default=False,
-        help="[experimental] Run jobs in parallel. ",
+        help="Run jobs in parallel. ",
     )
     envgroup = parser.add_mutually_exclusive_group()
     envgroup.add_argument(
         "--preserve-environment",
         type=str,
         action="append",
         help="Preserve specific environment variable when running "
@@ -444,25 +444,25 @@
         dest="user_space_docker_cmd",
     )
 
     dockergroup.add_argument(
         "--singularity",
         action="store_true",
         default=False,
-        help="[experimental] Use "
-        "Singularity runtime for running containers. "
+        help="Use "
+        "Singularity or Apptainer runtime for running containers. "
         "Requires Singularity v2.6.1+ and Linux with kernel "
         "version v3.18+ or with overlayfs support "
         "backported.",
     )
     dockergroup.add_argument(
         "--podman",
         action="store_true",
         default=False,
-        help="[experimental] Use " "Podman runtime for running containers. ",
+        help="Use Podman runtime for running containers. ",
     )
     dockergroup.add_argument(
         "--no-container",
         action="store_false",
         default=True,
         help="Do not execute jobs in a "
         "Docker container, even when `DockerRequirement` "
```

### Comparing `cwltool-3.1.20240112164112/cwltool/builder.py` & `cwltool-3.1.20240404144621/cwltool/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command line builder."""
+
 import copy
 import logging
 import math
 from decimal import Decimal
 from typing import (
     IO,
     TYPE_CHECKING,
```

### Comparing `cwltool-3.1.20240112164112/cwltool/checker.py` & `cwltool-3.1.20240404144621/cwltool/checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Static checking of CWL workflow connectivity."""
+
 from collections import namedtuple
 from typing import (
     Any,
     Dict,
     Iterator,
     List,
     Literal,
```

### Comparing `cwltool-3.1.20240112164112/cwltool/command_line_tool.py` & `cwltool-3.1.20240404144621/cwltool/command_line_tool.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/context.py` & `cwltool-3.1.20240404144621/cwltool/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Shared context objects that replace use of kwargs."""
+
 import copy
 import os
 import shutil
 import tempfile
 import threading
 from typing import (
     IO,
```

### Comparing `cwltool-3.1.20240112164112/cwltool/cuda.py` & `cwltool-3.1.20240404144621/cwltool/cuda.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/cwlprov/__init__.py` & `cwltool-3.1.20240404144621/cwltool/cwlprov/__init__.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/cwlprov/provenance_constants.py` & `cwltool-3.1.20240404144621/cwltool/cwlprov/provenance_constants.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/cwlprov/provenance_profile.py` & `cwltool-3.1.20240404144621/cwltool/cwlprov/provenance_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
             # FIXME: Make consistent hash URIs for these
             # that somehow include the type
             # (so "1" != 1 != "1.0" != true)
             entity = self.document.entity(uuid.uuid4().urn, {PROV_VALUE: value})
             self.research_object.add_uri(entity.identifier.uri)
             return entity
 
-        if isinstance(value, (str, str)):
+        if isinstance(value, str):
             (entity, _) = self.declare_string(value)
             return entity
 
         if isinstance(value, bytes):
             # If we got here then we must be in Python 3
             byte_s = BytesIO(value)
             data_file = self.research_object.add_data_file(byte_s)
```

### Comparing `cwltool-3.1.20240112164112/cwltool/cwlprov/ro.py` & `cwltool-3.1.20240404144621/cwltool/cwlprov/ro.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/cwlprov/writablebagfile.py` & `cwltool-3.1.20240404144621/cwltool/cwlprov/writablebagfile.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/cwlrdf.py` & `cwltool-3.1.20240404144621/cwltool/cwlrdf.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/cwlviewer.py` & `cwltool-3.1.20240404144621/cwltool/cwlviewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Visualize a CWL workflow."""
+
 from pathlib import Path
 from typing import Iterator, List, cast
 from urllib.parse import urlparse
 
 import pydot
 import rdflib
```

### Comparing `cwltool-3.1.20240112164112/cwltool/docker.py` & `cwltool-3.1.20240404144621/cwltool/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,15 +425,18 @@
                     "[job %s] Skipping Docker software container '--cpus' limit "
                     "despite presence of ResourceRequirement with coresMin "
                     "and/or coresMax setting. Consider running with "
                     "--strict-cpu-limit for increased portability "
                     "assurance.",
                     self.name,
                 )
-
+        shm_size_od, shm_bool = self.builder.get_requirement("http://commonwl.org/cwltool#ShmSize")
+        if shm_bool:
+            shm_size = cast(CWLObjectType, shm_size_od)["shmSize"]
+            runtime.append(f"--shm-size={shm_size}")
         return runtime, cidfile_path
 
 
 class PodmanCommandLineJob(DockerCommandLineJob):
     """Runs a :py:class:`~cwltool.job.CommandLineJob` in a software container using the podman engine."""
 
     def __init__(
```

### Comparing `cwltool-3.1.20240112164112/cwltool/docker_id.py` & `cwltool-3.1.20240404144621/cwltool/docker_id.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/env_to_stdout.py` & `cwltool-3.1.20240404144621/cwltool/env_to_stdout.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/executors.py` & `cwltool-3.1.20240404144621/cwltool/executors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Single and multi-threaded executors."""
+
 import datetime
 import functools
 import logging
 import math
 import os
 import threading
 from abc import ABCMeta, abstractmethod
```

### Comparing `cwltool-3.1.20240112164112/cwltool/extensions-v1.1.yml` & `cwltool-3.1.20240404144621/cwltool/extensions-v1.1.yml`

 * *Files 8% similar despite different names*

```diff
@@ -116,7 +116,25 @@
         same as `cudaDeviceCountMax`.  If neither are specified,
         default 1.
     cudaDeviceCountMax:
       type: ['null', int, cwl:Expression]
       doc: |
         Maximum number of GPU devices to request.  If not specified,
         same as `cudaDeviceCountMin`.
+- name: ShmSize
+  type: record
+  extends: cwl:ProcessRequirement
+  inVocab: false
+  fields:
+    class:
+      type: string
+      doc: 'cwltool:ShmSize'
+      jsonldPredicate:
+        "_id": "@type"
+        "_type": "@vocab"
+    shmSize:
+      type: string
+      doc: |
+        Size of /dev/shm. The format is `<number><unit>`. <number> must be greater
+        than 0. Unit is optional and can be `b` (bytes), `k` (kilobytes), `m`
+        (megabytes), or `g` (gigabytes). If you omit the unit, the default is
+        bytes. If you omit the size entirely, the value is `64m`."
```

### Comparing `cwltool-3.1.20240112164112/cwltool/extensions-v1.2.yml` & `cwltool-3.1.20240404144621/cwltool/extensions-v1.2.yml`

 * *Files 4% similar despite different names*

```diff
@@ -236,8 +236,25 @@
         name: LoopOutputModes
         symbols: [ last, all ]
       default: last
       doc:
         - Specify the desired method of dealing with loop outputs
         - Default. Propagates only the last computed element to the subsequent steps when the loop terminates.
         - Propagates a single array with all output values to the subsequent steps when the loop terminates.
-
+- name: ShmSize
+  type: record
+  extends: cwl:ProcessRequirement
+  inVocab: false
+  fields:
+    class:
+      type: string
+      doc: 'cwltool:ShmSize'
+      jsonldPredicate:
+        "_id": "@type"
+        "_type": "@vocab"
+    shmSize:
+      type: string
+      doc: |
+        Size of /dev/shm. The format is `<number><unit>`. <number> must be greater
+        than 0. Unit is optional and can be `b` (bytes), `k` (kilobytes), `m`
+        (megabytes), or `g` (gigabytes). If you omit the unit, the default is
+        bytes. If you omit the size entirely, the value is `64m`."
```

### Comparing `cwltool-3.1.20240112164112/cwltool/extensions.yml` & `cwltool-3.1.20240404144621/cwltool/extensions.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 $base: http://commonwl.org/cwltool#
 $namespaces:
   cwl: "https://w3id.org/cwl/cwl#"
+  cwltool: "http://commonwl.org/cwltool#"
 $graph:
 - $import: https://w3id.org/cwl/CommonWorkflowLanguage.yml
 
 - name: LoadListingRequirement
   type: record
   extends: cwl:ProcessRequirement
   inVocab: false
@@ -225,7 +226,25 @@
         same as `cudaDeviceCountMax`.  If neither are specified,
         default 1.
     cudaDeviceCountMax:
       type: ['null', int, cwl:Expression]
       doc: |
         Maximum number of GPU devices to request.  If not specified,
         same as `cudaDeviceCountMin`.
+- name: ShmSize
+  type: record
+  extends: cwl:ProcessRequirement
+  inVocab: false
+  fields:
+    class:
+      type: string
+      doc: 'cwltool:ShmSize'
+      jsonldPredicate:
+        "_id": "@type"
+        "_type": "@vocab"
+    shmSize:
+      type: string
+      doc: |
+        Size of /dev/shm. The format is `<number><unit>`. <number> must be greater
+        than 0. Unit is optional and can be `b` (bytes), `k` (kilobytes), `m`
+        (megabytes), or `g` (gigabytes). If you omit the unit, the default is
+        bytes. If you omit the size entirely, the value is `64m`."
```

### Comparing `cwltool-3.1.20240112164112/cwltool/factory.py` & `cwltool-3.1.20240404144621/cwltool/factory.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/flatten.py` & `cwltool-3.1.20240404144621/cwltool/flatten.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/hello.simg` & `cwltool-3.1.20240404144621/cwltool/hello.simg`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/job.py` & `cwltool-3.1.20240404144621/cwltool/job.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/jshint/jshint.js` & `cwltool-3.1.20240404144621/cwltool/jshint/jshint.js`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/jshint/jshint_wrapper.js` & `cwltool-3.1.20240404144621/cwltool/jshint/jshint_wrapper.js`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/load_tool.py` & `cwltool-3.1.20240404144621/cwltool/load_tool.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/loghandler.py` & `cwltool-3.1.20240404144621/cwltool/loghandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Shared logger for cwltool."""
+
 import logging
 
 import coloredlogs
 
 _logger = logging.getLogger("cwltool")  # pylint: disable=invalid-name
 defaultStreamHandler = logging.StreamHandler()  # pylint: disable=invalid-name
 _logger.addHandler(defaultStreamHandler)
```

### Comparing `cwltool-3.1.20240112164112/cwltool/main.py` & `cwltool-3.1.20240404144621/cwltool/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     Tuple,
     Union,
     cast,
 )
 
 import argcomplete
 import coloredlogs
+import requests
 import ruamel.yaml
 from ruamel.yaml.comments import CommentedMap, CommentedSeq
 from ruamel.yaml.main import YAML
 from schema_salad.exceptions import ValidationException
 from schema_salad.ref_resolver import Loader, file_uri, uri_file_path
 from schema_salad.sourceline import cmap, strip_dup_lineno
 from schema_salad.utils import (
@@ -169,14 +170,22 @@
 
     Refer to the docstring for _terminate_processes() for other caveats.
     """
     _terminate_processes()
     sys.exit(signum)
 
 
+def append_word_to_default_user_agent(word: str) -> None:
+    """Append the specified word to the requests http user agent string if it's not already there."""
+    original_function = requests.utils.default_user_agent
+    suffix = f" {word}"
+    if not original_function().endswith(suffix):
+        requests.utils.default_user_agent = lambda *args: original_function(*args) + suffix
+
+
 def generate_example_input(
     inptype: Optional[CWLOutputType],
     default: Optional[CWLOutputType],
 ) -> Tuple[Any, str]:
     """Convert a single input schema into an example."""
     example = None
     comment = ""
@@ -975,14 +984,20 @@
         _logger.addHandler(stderr_handler)
     else:
         coloredlogs.install(logger=_logger, stream=stderr)
         stderr_handler = _logger.handlers[-1]
     workflowobj = None
     prov_log_handler: Optional[logging.StreamHandler[ProvOut]] = None
     global docker_exe
+
+    user_agent = "cwltool"
+    if user_agent not in (progname := os.path.basename(sys.argv[0])):
+        user_agent += f" {progname}"  # append the real program name as well
+    append_word_to_default_user_agent(user_agent)
+
     try:
         if args is None:
             if argsl is None:
                 argsl = sys.argv[1:]
             addl = []  # type: List[str]
             if "CWLTOOL_OPTIONS" in os.environ:
                 c_opts = os.environ["CWLTOOL_OPTIONS"].split(" ")
```

### Comparing `cwltool-3.1.20240112164112/cwltool/mpi.py` & `cwltool-3.1.20240404144621/cwltool/mpi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Experimental support for MPI."""
+
 import inspect
 import os
 import re
 from typing import List, Mapping, MutableMapping, Optional, Type, TypeVar, Union
 
 from schema_salad.utils import yaml_no_ts
```

### Comparing `cwltool-3.1.20240112164112/cwltool/mutation.py` & `cwltool-3.1.20240404144621/cwltool/mutation.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/pack.py` & `cwltool-3.1.20240404144621/cwltool/pack.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/pathmapper.py` & `cwltool-3.1.20240404144621/cwltool/pathmapper.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/process.py` & `cwltool-3.1.20240404144621/cwltool/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes and methods relevant for all CWL Process types."""
+
 import abc
 import copy
 import functools
 import hashlib
 import json
 import logging
 import math
@@ -116,14 +117,15 @@
     MPIRequirementName,
     "http://commonwl.org/cwltool#TimeLimit",
     "http://commonwl.org/cwltool#WorkReuse",
     "http://commonwl.org/cwltool#NetworkAccess",
     "http://commonwl.org/cwltool#LoadListingRequirement",
     "http://commonwl.org/cwltool#InplaceUpdateRequirement",
     "http://commonwl.org/cwltool#CUDARequirement",
+    "http://commonwl.org/cwltool#ShmSize",
 ]
 
 cwl_files = (
     "Workflow.yml",
     "CommandLineTool.yml",
     "CommonWorkflowLanguage.yml",
     "Process.yml",
```

### Comparing `cwltool-3.1.20240112164112/cwltool/procgenerator.py` & `cwltool-3.1.20240404144621/cwltool/procgenerator.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/rdfqueries/get_inner_edges.sparql` & `cwltool-3.1.20240404144621/cwltool/rdfqueries/get_inner_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/rdfqueries/get_input_edges.sparql` & `cwltool-3.1.20240404144621/cwltool/rdfqueries/get_input_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/rdfqueries/get_output_edges.sparql` & `cwltool-3.1.20240404144621/cwltool/rdfqueries/get_output_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/rdfqueries/get_root.sparql` & `cwltool-3.1.20240404144621/cwltool/rdfqueries/get_root.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/resolver.py` & `cwltool-3.1.20240404144621/cwltool/resolver.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/run_job.py` & `cwltool-3.1.20240404144621/cwltool/run_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Only used when there is a job script or CWLTOOL_FORCE_SHELL_POPEN=1."""
+
 import json
 import os
 import subprocess  # nosec
 import sys
 from typing import BinaryIO, Dict, List, Optional, TextIO, Union
```

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/CITATION` & `cwltool-3.1.20240404144621/cwltool/schemas/CITATION`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240404144621/cwltool/schemas/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/README.md` & `cwltool-3.1.20240404144621/cwltool/schemas/README.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/CommandLineTool.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/Process.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/README.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/README.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/Workflow.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/concepts.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/conformance_test_v1.0.yaml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/conformance_test_v1.0.yaml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/contrib.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/intro.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/invocation.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/README.rst` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CITATION` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CITATION`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/CommandLineTool.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/Process.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/Workflow.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/concepts.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/conformance_tests.yaml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/conformance_tests.yaml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/contrib.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/cwl-runner.cwl` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/index.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/intro.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/invocation.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/README.rst` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/Process.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/Workflow.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/concepts.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/contrib.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/cwl-runner.cwl` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/intro.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/invocation.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/README.rst` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/CommandLineTool.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/Operation.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/Process.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/Workflow.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/concepts.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/contrib.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/index.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/intro.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/invocation.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/CommandLineTool.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/Process.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/Workflow.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/concepts.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/contrib.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/cwl-runner.cwl` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/intro.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/invocation.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/README.rst` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/Operation.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/Process.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/Workflow.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/concepts.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/contrib.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/cwl-runner.cwl` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/intro.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/invocation.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/README.rst` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/Operation.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/Process.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/Workflow.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/concepts.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/contrib.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/cwl-runner.cwl` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/index.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/intro.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/invocation.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/README.rst` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CITATION` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CITATION`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/Operation.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/Process.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/Workflow.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/concepts.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/conformance_tests.yaml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/conformance_tests.yaml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/contrib.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/cwl-runner.cwl` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/index.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/intro.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/invocation.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/README.rst` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CITATION` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CITATION`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/Operation.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/Process.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/Workflow.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/concepts.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/conformance_tests.yaml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/conformance_tests.yaml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/contrib.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/cwl-runner.cwl` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/cwl-runner.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/index.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/intro.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/invocation.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/LICENSE.txt` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/README.rst` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20240404144621/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/secrets.py` & `cwltool-3.1.20240404144621/cwltool/secrets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Minimal in memory storage of secrets."""
+
 import uuid
 from typing import Dict, List, MutableMapping, MutableSequence, Optional, cast
 
 from .utils import CWLObjectType, CWLOutputType
 
 
 class SecretStore:
```

### Comparing `cwltool-3.1.20240112164112/cwltool/singularity.py` & `cwltool-3.1.20240404144621/cwltool/singularity.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         tmpdir_prefix: str,
     ) -> None:
         if host_outdir_tgt is not None and not is_version_3_4_or_newer():
             # workaround for lack of overlapping mounts in Singularity <3.4
             if self.inplace_update:
                 try:
                     os.link(os.path.realpath(volume.resolved), host_outdir_tgt)
-                except os.error:
+                except OSError:
                     shutil.copy(volume.resolved, host_outdir_tgt)
             else:
                 shutil.copy(volume.resolved, host_outdir_tgt)
             ensure_writable(host_outdir_tgt)
         elif self.inplace_update:
             self.append_volume(runtime, volume.resolved, volume.target, writable=True)
             ensure_writable(volume.resolved)
```

### Comparing `cwltool-3.1.20240112164112/cwltool/singularity_utils.py` & `cwltool-3.1.20240404144621/cwltool/singularity_utils.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/software_requirements.py` & `cwltool-3.1.20240404144621/cwltool/software_requirements.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/stdfsaccess.py` & `cwltool-3.1.20240404144621/cwltool/stdfsaccess.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/subgraph.py` & `cwltool-3.1.20240404144621/cwltool/subgraph.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/task_queue.py` & `cwltool-3.1.20240404144621/cwltool/task_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     def _task_queue_func(self) -> None:
         while True:
             task = self.task_queue.get()
             if task is None:
                 return
             try:
                 task()
-            except BaseException as e:
-                _logger.exception("Unhandled exception running task")
+            except BaseException as e:  # noqa: B036
+                _logger.exception("Unhandled exception running task", exc_info=e)
                 self.error = e
             finally:
                 with self.lock:
                     self.in_flight -= 1
 
     def add(
         self,
```

### Comparing `cwltool-3.1.20240112164112/cwltool/udocker.py` & `cwltool-3.1.20240404144621/cwltool/udocker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/update.py` & `cwltool-3.1.20240404144621/cwltool/update.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/utils.py` & `cwltool-3.1.20240404144621/cwltool/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Shared functions and other definitions."""
+
 import collections
 
 try:
     import fcntl
 except ImportError:
     # Guard against `from .utils import ...` on windows.
     # See windows_check() in main.py
```

### Comparing `cwltool-3.1.20240112164112/cwltool/validate_js.py` & `cwltool-3.1.20240404144621/cwltool/validate_js.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/workflow.py` & `cwltool-3.1.20240404144621/cwltool/workflow.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool/workflow_job.py` & `cwltool-3.1.20240404144621/cwltool/workflow_job.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool-in-docker.sh` & `cwltool-3.1.20240404144621/cwltool-in-docker.sh`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool.Dockerfile` & `cwltool-3.1.20240404144621/cwltool.Dockerfile`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/cwltool.egg-info/PKG-INFO` & `cwltool-3.1.20240404144621/cwltool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltool
-Version: 3.1.20240112164112
+Version: 3.1.20240404144621
 Summary: Common workflow language reference implementation
 Home-page: https://github.com/common-workflow-language/cwltool
 Download-URL: https://github.com/common-workflow-language/cwltool
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -46,16 +46,16 @@
 Requires-Dist: coloredlogs
 Requires-Dist: pydot>=1.4.1
 Requires-Dist: argcomplete
 Requires-Dist: pyparsing!=3.0.2
 Requires-Dist: cwl-utils>=0.32
 Requires-Dist: spython>=0.3.0
 Provides-Extra: deps
-Requires-Dist: galaxy-tool-util!=23.0.1,!=23.0.2,!=23.0.3,!=23.0.4,!=23.0.5,<23.2,>=22.1.2; extra == "deps"
-Requires-Dist: galaxy-util<23.2; extra == "deps"
+Requires-Dist: galaxy-tool-util!=23.0.1,!=23.0.2,!=23.0.3,!=23.0.4,!=23.0.5,<24.1,>=22.1.2; extra == "deps"
+Requires-Dist: galaxy-util<24.1; extra == "deps"
 
 #############################################################################################
 ``cwltool``: The reference reference implementation of the Common Workflow Language standards
 #############################################################################################
 
 |Linux Status| |Coverage Status| |Docs Status|
```

### Comparing `cwltool-3.1.20240112164112/cwltool.egg-info/SOURCES.txt` & `cwltool-3.1.20240404144621/cwltool.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -696,14 +696,15 @@
 tests/test_subclass_mypyc.py
 tests/test_subgraph.py
 tests/test_target.py
 tests/test_tmpdir.py
 tests/test_toolargparse.py
 tests/test_trs.py
 tests/test_udocker.py
+tests/test_user_agent.py
 tests/test_validate.py
 tests/test_validate_js.py
 tests/test_windows_warning.py
 tests/utf_doc_example.cwl
 tests/util.py
 tests/wc-tool-bad-hints.cwl
 tests/wc-tool-bad-reqs.cwl
@@ -939,14 +940,15 @@
 tests/wf/schemadef-type.yml
 tests/wf/sec-tool.cwl
 tests/wf/sec-wf-out.cwl
 tests/wf/sec-wf.cwl
 tests/wf/secret_job.cwl
 tests/wf/secret_wf.cwl
 tests/wf/separate_without_prefix.cwl
+tests/wf/shm_size.cwl
 tests/wf/sorttool.cwl
 tests/wf/storage_float.cwl
 tests/wf/tar-param.cwl
 tests/wf/three_step_color.cwl
 tests/wf/timelimit-fail.cwl
 tests/wf/timelimit.cwl
 tests/wf/touch_tool.cwl
```

### Comparing `cwltool-3.1.20240112164112/docs/CWLProv.rst` & `cwltool-3.1.20240404144621/docs/CWLProv.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/docs/Makefile` & `cwltool-3.1.20240404144621/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/docs/_static/favicon.ico` & `cwltool-3.1.20240404144621/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/docs/conf.py` & `cwltool-3.1.20240404144621/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/docs/loop.rst` & `cwltool-3.1.20240404144621/docs/loop.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/docs/make.bat` & `cwltool-3.1.20240404144621/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/docs/processgen.rst` & `cwltool-3.1.20240404144621/docs/processgen.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/docs/pythonversions.rst` & `cwltool-3.1.20240404144621/docs/pythonversions.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/arcp/parse.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/arcp/parse.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/bagit.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/bagit.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/mistune.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/mistune.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/prov/constants.py` & `cwltool-3.1.20240404144621/mypy-stubs/prov/constants.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/prov/dot.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/prov/dot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/prov/graph.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/prov/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/prov/identifier.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/prov/identifier.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/prov/model.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/prov/model.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -219,18 +219,17 @@
     ) -> Namespace: ...
     def get_registered_namespaces(self) -> Iterable[Namespace]: ...
     def valid_qualified_name(
         self, identifier: QualifiedName | Tuple[str, Identifier]
     ) -> QualifiedName | None: ...
     def get_records(
         self,
-        class_or_type_or_tuple: type
-        | type[int | str]
-        | Tuple[type | type[int | str] | Tuple[Any, ...], ...]
-        | None = ...,
+        class_or_type_or_tuple: (
+            type | type[int | str] | Tuple[type | type[int | str] | Tuple[Any, ...], ...] | None
+        ) = ...,
     ) -> List[ProvRecord]: ...
     def get_record(self, identifier: Identifier | None) -> ProvRecord | List[ProvRecord] | None: ...
     def is_document(self) -> bool: ...
     def is_bundle(self) -> bool: ...
     def has_bundles(self) -> bool: ...
     @property
     def bundles(self) -> Iterable[ProvBundle]: ...
```

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/prov/serializers/provjson.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provjson.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/prov/serializers/provrdf.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provrdf.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/prov/serializers/provxml.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/prov/serializers/provxml.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/pydot.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/pydot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/__init__.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/collection.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/graph.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_ORG.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_OWL.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_PROV.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_QB.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_RDF.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SDO.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SH.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_SSN.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_TIME.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_VOID.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/_XSD.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/namespace/__init__.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/paths.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/query.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/resource.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/rdflib/term.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/mypy-stubs/spython/main/build.pyi` & `cwltool-3.1.20240404144621/mypy-stubs/spython/main/build.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/pyproject.toml` & `cwltool-3.1.20240404144621/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
     "setuptools>=45",
     "setuptools_scm[toml]>=8.0.4,<9",
-    "mypy==1.8.0",  # also update mypy-requirements.txt
+    "mypy==1.9.0",  # also update mypy-requirements.txt
     "types-requests",
     "types-psutil",
     "importlib_resources>=1.4;python_version<'3.9'",
     "ruamel.yaml>=0.16.0,<0.18",
     "schema-salad>=8.4.20230426093816,<9",
     "cwl-utils>=0.32",
     "toml",
```

### Comparing `cwltool-3.1.20240112164112/release-test.sh` & `cwltool-3.1.20240404144621/release-test.sh`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 fi
 test_prefix=""
 run_tests() {
 	local mod_loc
 	mod_loc=$(pip show ${package} |
 		grep ^Location | awk '{print $2}')/${module}
 	"${test_prefix}"bin/py.test "--ignore=${mod_loc}/schemas/" \
-		--pyargs -x ${module} -n auto --dist=loadfile
+		--pyargs -x ${module} -n logical --dist=worksteal
 }
 pipver=23.1  # minimum required version of pip for Python 3.12
 setuptoolsver=67.6.1  # required for Python 3.12
 DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null && pwd )"
 
 rm -Rf testenv? || /bin/true
```

### Comparing `cwltool-3.1.20240112164112/setup.py` & `cwltool-3.1.20240404144621/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -91,15 +91,37 @@
     author="Common workflow language working group",
     author_email="common-workflow-language@googlegroups.com",
     url="https://github.com/common-workflow-language/cwltool",
     download_url="https://github.com/common-workflow-language/cwltool",
     ext_modules=ext_modules,
     # platforms='',  # empty as is conveyed by the classifier below
     # license='',  # empty as is conveyed by the classifier below
-    packages=["cwltool", "cwltool.tests", "cwltool.cwlprov"],
+    packages=[
+        "cwltool",
+        "cwltool.cwlprov",
+        "cwltool.jshint",
+        "cwltool.rdfqueries",
+        "cwltool.schemas",
+        "cwltool.tests",
+        "cwltool.tests.checker_wf",
+        "cwltool.tests.input_deps",
+        "cwltool.tests.loop",
+        "cwltool.tests.override",
+        "cwltool.tests.reloc",
+        "cwltool.tests.subgraph",
+        "cwltool.tests.test_deps_env",
+        "cwltool.tests.test_deps_env.modulefiles",
+        "cwltool.tests.tmp1.tmp2.tmp3",
+        "cwltool.tests.tmp4.alpha",
+        "cwltool.tests.trs",
+        "cwltool.tests.wf",
+        "cwltool.tests.wf.generator",
+        "cwltool.tests.wf.indir",
+        "cwltool.tests.wf.operation",
+    ],
     package_dir={"cwltool.tests": "tests"},
     include_package_data=True,
     install_requires=[
         "setuptools",
         "requests >= 2.6.1",  # >= 2.6.1 to workaround
         # https://github.com/ionrock/cachecontrol/issues/137
         "ruamel.yaml >= 0.16, < 0.19",
@@ -115,25 +137,25 @@
         "argcomplete",
         "pyparsing != 3.0.2",  # breaks --print-dot (pydot) https://github.com/pyparsing/pyparsing/issues/319
         "cwl-utils >= 0.32",
         "spython >= 0.3.0",
     ],
     extras_require={
         "deps": [
-            "galaxy-tool-util>=22.1.2,<23.2,!=23.0.1,!=23.0.2,!=23.0.3,!=23.0.4,!=23.0.5",
-            "galaxy-util <23.2",
+            "galaxy-tool-util>=22.1.2,!=23.0.1,!=23.0.2,!=23.0.3,!=23.0.4,!=23.0.5,<24.1",
+            "galaxy-util <24.1",
         ],
     },
     python_requires=">=3.8, <4",
     use_scm_version=True,
     setup_requires=PYTEST_RUNNER + ["setuptools_scm>=8.0.4,<9"],
     test_suite="tests",
     tests_require=[
         "bagit >= 1.6.4, < 1.9",
-        "pytest >= 6.2, < 7.5",
+        "pytest >= 6.2, < 8.2",
         "mock >= 2.0.0",
         "pytest-mock >= 1.10.0",
         "pytest-httpserver",
         "arcp >= 0.2.0",
     ],
     entry_points={"console_scripts": ["cwltool=cwltool.main:run"]},
     zip_safe=True,
```

### Comparing `cwltool-3.1.20240112164112/tests/2.fasta` & `cwltool-3.1.20240404144621/tests/2.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/bundle-context.jsonld` & `cwltool-3.1.20240404144621/tests/bundle-context.jsonld`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/checker_wf/broken-wf.cwl` & `cwltool-3.1.20240404144621/tests/checker_wf/broken-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/checker_wf/broken-wf2.cwl` & `cwltool-3.1.20240404144621/tests/checker_wf/broken-wf2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/checker_wf/broken-wf3.cwl` & `cwltool-3.1.20240404144621/tests/checker_wf/broken-wf3.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/checker_wf/circ-dep-wf.cwl` & `cwltool-3.1.20240404144621/tests/checker_wf/circ-dep-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/checker_wf/circ-dep-wf2.cwl` & `cwltool-3.1.20240404144621/tests/checker_wf/circ-dep-wf2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/checker_wf/functional-wf.cwl` & `cwltool-3.1.20240404144621/tests/checker_wf/functional-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/cwl-conformance/cwltool-conftest.py` & `cwltool-3.1.20240404144621/tests/cwl-conformance/cwltool-conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Example configuration for pytest + cwltest plugin using cwltool directly.
 
 Calls cwltool via Python, instead of a subprocess via `--cwl-runner cwltool`.
 """
+
 import json
 from io import StringIO
 from typing import Any, Dict, List, Optional, Tuple
 
 from cwltest import utils
```

### Comparing `cwltool-3.1.20240112164112/tests/echo-badposition-expr.cwl` & `cwltool-3.1.20240404144621/tests/echo-badposition-expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/echo-position-expr.cwl` & `cwltool-3.1.20240404144621/tests/echo-position-expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/input_deps/docker-array-secondaryfiles.cwl` & `cwltool-3.1.20240404144621/tests/input_deps/docker-array-secondaryfiles.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/input_deps/ref.fasta` & `cwltool-3.1.20240404144621/tests/input_deps/ref.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/input_deps/ref2.fasta` & `cwltool-3.1.20240404144621/tests/input_deps/ref2.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/all-output-loop-no-iteration.cwl` & `cwltool-3.1.20240404144621/tests/loop/all-output-loop-no-iteration.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/all-output-loop.cwl` & `cwltool-3.1.20240404144621/tests/loop/all-output-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/default-value-loop.cwl` & `cwltool-3.1.20240404144621/tests/loop/default-value-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/invalid-loop-command-line-tool.cwl` & `cwltool-3.1.20240404144621/tests/loop/invalid-loop-command-line-tool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/invalid-loop-hint.cwl` & `cwltool-3.1.20240404144621/tests/loop/invalid-loop-hint.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/invalid-loop-scatter.cwl` & `cwltool-3.1.20240404144621/tests/loop/invalid-loop-scatter.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/invalid-loop-when.cwl` & `cwltool-3.1.20240404144621/tests/loop/invalid-loop-when.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/invalid-loop-workflow.cwl` & `cwltool-3.1.20240404144621/tests/loop/invalid-loop-workflow.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/invalid-multi-source-loop-no-requirement.cwl` & `cwltool-3.1.20240404144621/tests/loop/invalid-multi-source-loop-no-requirement.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/invalid-no-loopWhen.cwl` & `cwltool-3.1.20240404144621/tests/loop/invalid-no-loopWhen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/invalid-non-boolean-loopWhen.cwl` & `cwltool-3.1.20240404144621/tests/loop/invalid-non-boolean-loopWhen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/invalid-value-from-loop-no-requirement.cwl` & `cwltool-3.1.20240404144621/tests/loop/invalid-value-from-loop-no-requirement.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/loop-inside-loop-all.cwl` & `cwltool-3.1.20240404144621/tests/loop/loop-inside-loop-all.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/loop-inside-loop.cwl` & `cwltool-3.1.20240404144621/tests/loop/loop-inside-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/loop-inside-scatter.cwl` & `cwltool-3.1.20240404144621/tests/loop/loop-inside-scatter.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/multi-source-loop.cwl` & `cwltool-3.1.20240404144621/tests/loop/multi-source-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/scatter-inside-loop.cwl` & `cwltool-3.1.20240404144621/tests/loop/scatter-inside-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/single-var-loop-no-iteration.cwl` & `cwltool-3.1.20240404144621/tests/loop/single-var-loop-no-iteration.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/single-var-loop.cwl` & `cwltool-3.1.20240404144621/tests/loop/single-var-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/two-vars-loop-2.cwl` & `cwltool-3.1.20240404144621/tests/loop/two-vars-loop-2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/two-vars-loop.cwl` & `cwltool-3.1.20240404144621/tests/loop/two-vars-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/loop/value-from-loop.cwl` & `cwltool-3.1.20240404144621/tests/loop/value-from-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/random_lines.cwl` & `cwltool-3.1.20240404144621/tests/random_lines.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/random_lines_mapping.cwl` & `cwltool-3.1.20240404144621/tests/random_lines_mapping.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/scatter_numbers.cwl` & `cwltool-3.1.20240404144621/tests/scatter_numbers.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/secondary-files-bad.cwl` & `cwltool-3.1.20240404144621/tests/secondary-files-bad.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/secondary-files.cwl` & `cwltool-3.1.20240404144621/tests/secondary-files.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/seqtk_seq_wrong_name.cwl` & `cwltool-3.1.20240404144621/tests/seqtk_seq_wrong_name.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/count-lines1-wf.cwl` & `cwltool-3.1.20240404144621/tests/subgraph/count-lines1-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/count-lines17-wf.cwl.json` & `cwltool-3.1.20240404144621/tests/subgraph/count-lines17-wf.cwl.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/env-wf2_subwf-packed.cwl` & `cwltool-3.1.20240404144621/tests/subgraph/env-wf2_subwf-packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_count_output.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_count_output.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_file1.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_file1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_file2.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_file2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_file3.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_file3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_output3.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_output3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_output4.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_output4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_output5.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_output5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_step1.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_step1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_step2.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_step2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_step2_1432.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_step2_1432.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_step3.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_step3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_step4.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_step4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/extract_step5.json` & `cwltool-3.1.20240404144621/tests/subgraph/extract_step5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/single_step1.json` & `cwltool-3.1.20240404144621/tests/subgraph/single_step1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/single_step2.json` & `cwltool-3.1.20240404144621/tests/subgraph/single_step2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/single_step3.json` & `cwltool-3.1.20240404144621/tests/subgraph/single_step3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/single_step4.json` & `cwltool-3.1.20240404144621/tests/subgraph/single_step4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/single_step5.json` & `cwltool-3.1.20240404144621/tests/subgraph/single_step5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/steplevel-resreq.cwl` & `cwltool-3.1.20240404144621/tests/subgraph/steplevel-resreq.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/subgraph/timelimit2-wf.cwl` & `cwltool-3.1.20240404144621/tests/subgraph/timelimit2-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_anon_types.py` & `cwltool-3.1.20240404144621/tests/test_anon_types.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_bad_outputs_wf.cwl` & `cwltool-3.1.20240404144621/tests/test_bad_outputs_wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_conditionals.py` & `cwltool-3.1.20240404144621/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_content_type.py` & `cwltool-3.1.20240404144621/tests/test_content_type.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_context.py` & `cwltool-3.1.20240404144621/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_cuda.py` & `cwltool-3.1.20240404144621/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_default_path.py` & `cwltool-3.1.20240404144621/tests/test_default_path.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_dependencies.py` & `cwltool-3.1.20240404144621/tests/test_dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests of satisfying SoftwareRequirement via dependencies."""
+
 import os
 import tempfile
 from getpass import getuser
 from pathlib import Path
 from shutil import which
 from types import ModuleType
 from typing import Optional, Tuple
@@ -20,14 +21,15 @@
     from galaxy.tool_util import deps
 except ImportError:
     pass
 
 
 @needs_docker
 @pytest.mark.skipif(not deps, reason="galaxy-tool-util is not installed")
+@pytest.mark.flaky(retries=3)
 def test_biocontainers(tmp_path: Path) -> None:
     wflow = get_data("tests/seqtk_seq.cwl")
     job = get_data("tests/seqtk_seq_job.json")
     error_code, _, _ = get_main_output(
         [
             "--outdir",
             str(tmp_path / "out"),
@@ -43,20 +45,18 @@
 
 
 @needs_docker
 @pytest.mark.skipif(not deps, reason="galaxy-tool-util is not installed")
 def test_biocontainers_resolution(tmp_path: Path) -> None:
     """Confirm expected container name for --beta-use-biocontainers."""
     tool = load_tool(get_data("tests/seqtk_seq.cwl"), LoadingContext())
-    assert (
-        get_container_from_software_requirements(
-            True, tool, container_image_cache_path=str(tmp_path)
-        )
-        == "quay.io/biocontainers/seqtk:r93--0"
+    container = get_container_from_software_requirements(
+        True, tool, container_image_cache_path=str(tmp_path)
     )
+    assert container is not None and container.startswith("quay.io/biocontainers/seqtk:1.4--")
 
 
 @pytest.fixture(scope="session")
 def bioconda_setup(request: pytest.FixtureRequest) -> Tuple[Optional[int], str]:
     """
     Caches the conda environment created for seqtk_seq.cwl.
```

### Comparing `cwltool-3.1.20240112164112/tests/test_deps_env/modulefiles/random-lines/1.0` & `cwltool-3.1.20240404144621/tests/test_deps_env/modulefiles/random-lines/1.0`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_deps_env/random-lines/1.0/scripts/random-lines` & `cwltool-3.1.20240404144621/tests/test_deps_env/random-lines/1.0/scripts/random-lines`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_docker.py` & `cwltool-3.1.20240404144621/tests/test_docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for docker engine."""
+
 import json
 import re
 from pathlib import Path
 from shutil import which
 
 import pytest
 
@@ -259,7 +260,24 @@
     stderr = re.sub(r"\s\s+", " ", stderr)
     assert "Job error:" in stderr
     assert "Error collecting output for parameter 'output'" in stderr
     assert (
         "tests/secondary-files-required-missing-container.cwl:16:5: Missing required secondary file"
     )
     assert "file.ext3" in stderr
+
+
+@needs_docker
+def test_docker_shm_size(tmp_path: Path) -> None:
+    result_code, stdout, stderr = get_main_output(
+        [
+            "--enable-ext",
+            "--default-container",
+            "docker.io/debian:stable-slim",
+            "--outdir",
+            str(tmp_path),
+            get_data("tests/wf/shm_size.cwl"),
+        ]
+    )
+    stderr = re.sub(r"\s\s+", " ", stderr)
+    assert result_code == 0
+    assert "--shm-size=128m" in stderr
```

### Comparing `cwltool-3.1.20240112164112/tests/test_docker_paths_with_colons.py` & `cwltool-3.1.20240404144621/tests/test_docker_paths_with_colons.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_empty_input.py` & `cwltool-3.1.20240404144621/tests/test_empty_input.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_environment.py` & `cwltool-3.1.20240404144621/tests/test_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test passing of environment variables to tools."""
+
 import os
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Mapping, Union
 
 import pytest
```

### Comparing `cwltool-3.1.20240112164112/tests/test_examples.py` & `cwltool-3.1.20240404144621/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_ext.py` & `cwltool-3.1.20240404144621/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_fetch.py` & `cwltool-3.1.20240404144621/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_http_input.py` & `cwltool-3.1.20240404144621/tests/test_http_input.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_input_deps.py` & `cwltool-3.1.20240404144621/tests/test_input_deps.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_iwdr.py` & `cwltool-3.1.20240404144621/tests/test_iwdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """InitialWorkDirRequirement related tests."""
+
 import json
 import re
 from pathlib import Path
 from stat import S_IWGRP, S_IWOTH, S_IWRITE
 from typing import Any
 
 import pytest
```

### Comparing `cwltool-3.1.20240112164112/tests/test_js_sandbox.py` & `cwltool-3.1.20240404144621/tests/test_js_sandbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test sandboxjs.py and related code."""
+
 import logging
 import os
 import shutil
 import threading
 from pathlib import Path
 from typing import Any, List
 
@@ -60,15 +61,15 @@
             new_dir = temp_dir / os.path.basename(dirname)
             new_dir.mkdir()
             for entry in os.listdir(dirname):
                 if entry not in ("nodejs", "node"):
                     os.symlink(os.path.join(dirname, entry), new_dir / entry)
             paths.append(str(new_dir))
             dirname_path = Path(dirname)
-            for path in paths:
+            for path in list(paths):
                 if Path(path).resolve() == dirname_path:
                     paths.remove(path)
     return ":".join(paths)
 
 
 @needs_podman
 def test_value_from_two_concatenated_expressions_podman(
```

### Comparing `cwltool-3.1.20240112164112/tests/test_load_tool.py` & `cwltool-3.1.20240404144621/tests/test_load_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for cwltool.load_tool."""
+
 import logging
 import urllib.parse
 from pathlib import Path
 
 import pytest
 from schema_salad.exceptions import ValidationException
```

### Comparing `cwltool-3.1.20240112164112/tests/test_loop.py` & `cwltool-3.1.20240404144621/tests/test_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the prototype loop extension."""
+
 import json
 from io import StringIO
 from typing import MutableMapping, MutableSequence
 
 from cwltool.main import main
 
 from .util import get_data
```

### Comparing `cwltool-3.1.20240112164112/tests/test_main_parsed_args.py` & `cwltool-3.1.20240404144621/tests/test_main_parsed_args.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_make_template.py` & `cwltool-3.1.20240404144621/tests/test_make_template.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_misc_cli.py` & `cwltool-3.1.20240404144621/tests/test_misc_cli.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_mpi.py` & `cwltool-3.1.20240404144621/tests/test_mpi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests of the experimental MPI extension."""
+
 import json
 import os.path
 import sys
 from io import StringIO
 from pathlib import Path
 from typing import Any, Generator, List, MutableMapping, Optional, Tuple
```

### Comparing `cwltool-3.1.20240112164112/tests/test_override.py` & `cwltool-3.1.20240404144621/tests/test_override.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_pack.py` & `cwltool-3.1.20240404144621/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_parallel.py` & `cwltool-3.1.20240404144621/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_path_checks.py` & `cwltool-3.1.20240404144621/tests/test_path_checks.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_pathmapper.py` & `cwltool-3.1.20240404144621/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_procgenerator.py` & `cwltool-3.1.20240404144621/tests/test_procgenerator.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_provenance.py` & `cwltool-3.1.20240404144621/tests/test_provenance.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_rdfprint.py` & `cwltool-3.1.20240404144621/tests/test_rdfprint.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_recursive_validation.py` & `cwltool-3.1.20240404144621/tests/test_recursive_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the recursive validation feature (validate document and try to build tool)."""
+
 from cwltool.load_tool import fetch_document, recursive_resolve_and_validate_document
 
 from .util import get_data
 
 
 def test_recursive_validation() -> None:
     """Test the recursive_resolve_and_validate_document function."""
```

### Comparing `cwltool-3.1.20240112164112/tests/test_relocate.py` & `cwltool-3.1.20240404144621/tests/test_relocate.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_secrets.py` & `cwltool-3.1.20240404144621/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_singularity.py` & `cwltool-3.1.20240404144621/tests/test_singularity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests to find local Singularity image."""
+
 import shutil
 from pathlib import Path
 from typing import Any
 
 import pytest
 
 from cwltool.main import main
```

### Comparing `cwltool-3.1.20240112164112/tests/test_singularity_versions.py` & `cwltool-3.1.20240404144621/tests/test_singularity_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test singularity{,-ce} & apptainer versions."""
+
 from subprocess import check_output  # nosec
 
 import cwltool.singularity
 from cwltool.singularity import (
     get_version,
     is_apptainer_1_or_newer,
     is_version_2_6,
```

### Comparing `cwltool-3.1.20240112164112/tests/test_stdout_stderr_log_dir.py` & `cwltool-3.1.20240404144621/tests/test_stdout_stderr_log_dir.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_streaming.py` & `cwltool-3.1.20240404144621/tests/test_streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test that files marked as 'streamable' when 'streaming_allowed' can be named pipes."""
+
 import os
 from pathlib import Path
 from typing import cast
 
 import pytest
 from ruamel.yaml.comments import CommentedMap
 from schema_salad.sourceline import cmap
```

### Comparing `cwltool-3.1.20240112164112/tests/test_subclass_mypyc.py` & `cwltool-3.1.20240404144621/tests/test_subclass_mypyc.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_subgraph.py` & `cwltool-3.1.20240404144621/tests/test_subgraph.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_target.py` & `cwltool-3.1.20240404144621/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_tmpdir.py` & `cwltool-3.1.20240404144621/tests/test_tmpdir.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test that all temporary directories respect the --tmpdir-prefix and --tmp-outdir-prefix options."""
+
 import os
 import re
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 from typing import List, cast
```

### Comparing `cwltool-3.1.20240112164112/tests/test_toolargparse.py` & `cwltool-3.1.20240404144621/tests/test_toolargparse.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_trs.py` & `cwltool-3.1.20240404144621/tests/test_trs.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_udocker.py` & `cwltool-3.1.20240404144621/tests/test_udocker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test optional udocker feature."""
+
 import copy
 import os
 import subprocess
 import sys
 from pathlib import Path
 
 import pytest
```

### Comparing `cwltool-3.1.20240112164112/tests/test_validate.py` & `cwltool-3.1.20240404144621/tests/test_validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests --validation."""
+
 import re
 
 from .util import get_data, get_main_output
 
 
 def test_validate_graph_with_no_default() -> None:
     """Ensure that --validate works on $graph docs that lack a main/#main."""
```

### Comparing `cwltool-3.1.20240112164112/tests/test_validate_js.py` & `cwltool-3.1.20240404144621/tests/test_validate_js.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/test_windows_warning.py` & `cwltool-3.1.20240404144621/tests/test_windows_warning.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/trs/Dockstore.cwl` & `cwltool-3.1.20240404144621/tests/trs/Dockstore.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/trs/md5sum-tool.cwl` & `cwltool-3.1.20240404144621/tests/trs/md5sum-tool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/utf_doc_example.cwl` & `cwltool-3.1.20240404144621/tests/utf_doc_example.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/util.py` & `cwltool-3.1.20240404144621/tests/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test functions."""
+
 import atexit
 import contextlib
 import io
 import json
 import os
 import shutil
 import subprocess
```

### Comparing `cwltool-3.1.20240112164112/tests/wf/910.cwl` & `cwltool-3.1.20240404144621/tests/wf/910.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/bad_formattest.cwl` & `cwltool-3.1.20240404144621/tests/wf/bad_formattest.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/bad_formattest2.cwl` & `cwltool-3.1.20240404144621/tests/wf/bad_formattest2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/conflict.cwl` & `cwltool-3.1.20240404144621/tests/wf/conflict.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/directory.cwl` & `cwltool-3.1.20240404144621/tests/wf/directory.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/double-nested.cwl` & `cwltool-3.1.20240404144621/tests/wf/double-nested.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/echo.cwl` & `cwltool-3.1.20240404144621/tests/wf/echo.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/expect_iwd-passthrough1_packed.cwl` & `cwltool-3.1.20240404144621/tests/wf/expect_iwd-passthrough1_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/expect_packed.cwl` & `cwltool-3.1.20240404144621/tests/wf/expect_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/expect_revsort_datetime_packed.cwl` & `cwltool-3.1.20240404144621/tests/wf/expect_revsort_datetime_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/expect_trick_packed.cwl` & `cwltool-3.1.20240404144621/tests/wf/expect_trick_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/extract_region_specs.cwl` & `cwltool-3.1.20240404144621/tests/wf/extract_region_specs.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/floats_small_and_large.cwl` & `cwltool-3.1.20240404144621/tests/wf/floats_small_and_large.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/generator/pytoolgen.cwl` & `cwltool-3.1.20240404144621/tests/wf/generator/pytoolgen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/hello-workflow-badhints.cwl` & `cwltool-3.1.20240404144621/tests/wf/hello-workflow-badhints.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/hello-workflow-badhints2.cwl` & `cwltool-3.1.20240404144621/tests/wf/hello-workflow-badhints2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/hello-workflow.cwl` & `cwltool-3.1.20240404144621/tests/wf/hello-workflow.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/iwd-passthrough1.cwl` & `cwltool-3.1.20240404144621/tests/wf/iwd-passthrough1.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/iwdr-passthrough-successive.cwl` & `cwltool-3.1.20240404144621/tests/wf/iwdr-passthrough-successive.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/iwdr_permutations.cwl` & `cwltool-3.1.20240404144621/tests/wf/iwdr_permutations.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/iwdr_permutations_nocontainer.cwl` & `cwltool-3.1.20240404144621/tests/wf/iwdr_permutations_nocontainer.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/missing_cwlVersion.cwl` & `cwltool-3.1.20240404144621/tests/wf/missing_cwlVersion.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/mpi_expr.cwl` & `cwltool-3.1.20240404144621/tests/wf/mpi_expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/mpi_simple_wf.cwl` & `cwltool-3.1.20240404144621/tests/wf/mpi_simple_wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/nested.cwl` & `cwltool-3.1.20240404144621/tests/wf/nested.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/operation/expect_operation-single_packed.cwl` & `cwltool-3.1.20240404144621/tests/wf/operation/expect_operation-single_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/operation/operation-single.cwl` & `cwltool-3.1.20240404144621/tests/wf/operation/operation-single.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/packed-with-loadlisting.cwl` & `cwltool-3.1.20240404144621/tests/wf/packed-with-loadlisting.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/packed_no_main.cwl` & `cwltool-3.1.20240404144621/tests/wf/packed_no_main.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/paramref_arguments_roundtrip.cwl` & `cwltool-3.1.20240404144621/tests/wf/paramref_arguments_roundtrip.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/paramref_arguments_self.cwl` & `cwltool-3.1.20240404144621/tests/wf/paramref_arguments_self.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/record_outputeval.cwl` & `cwltool-3.1.20240404144621/tests/wf/record_outputeval.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/revsort.cwl` & `cwltool-3.1.20240404144621/tests/wf/revsort.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/revsort_datetime.cwl` & `cwltool-3.1.20240404144621/tests/wf/revsort_datetime.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/revsort_step_bad_schema.cwl` & `cwltool-3.1.20240404144621/tests/wf/revsort_step_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/revtool.cwl` & `cwltool-3.1.20240404144621/tests/wf/revtool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/revtool_bad_schema.cwl` & `cwltool-3.1.20240404144621/tests/wf/revtool_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/scatter-wf4.cwl` & `cwltool-3.1.20240404144621/tests/wf/scatter-wf4.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/scatter-wf4.json` & `cwltool-3.1.20240404144621/tests/wf/scatter-wf4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/scatter2.cwl` & `cwltool-3.1.20240404144621/tests/wf/scatter2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/scatter2_subwf.cwl` & `cwltool-3.1.20240404144621/tests/wf/scatter2_subwf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/scatterfail.cwl` & `cwltool-3.1.20240404144621/tests/wf/scatterfail.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/schemadef-bug-1473.cwl` & `cwltool-3.1.20240404144621/tests/wf/schemadef-bug-1473.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/sec-wf-out.cwl` & `cwltool-3.1.20240404144621/tests/wf/sec-wf-out.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/sorttool.cwl` & `cwltool-3.1.20240404144621/tests/wf/sorttool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/three_step_color.cwl` & `cwltool-3.1.20240404144621/tests/wf/three_step_color.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/trick_revsort.cwl` & `cwltool-3.1.20240404144621/tests/wf/trick_revsort.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/updateval_inplace.cwl` & `cwltool-3.1.20240404144621/tests/wf/updateval_inplace.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/wffail.cwl` & `cwltool-3.1.20240404144621/tests/wf/wffail.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/whale.txt` & `cwltool-3.1.20240404144621/tests/wf/whale.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tests/wf/wrong_cwlVersion.cwl` & `cwltool-3.1.20240404144621/tests/wf/wrong_cwlVersion.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20240112164112/tox.ini` & `cwltool-3.1.20240404144621/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   py312-lintreadme
   py312-shellcheck
   py312-pydocstyle
 
 skip_missing_interpreters = True
 
 [pytest]
-addopts=--ignore cwltool/schemas -n auto
+addopts=--ignore cwltool/schemas -n logical --dist worksteal
 testpaths = tests
 
 [gh-actions]
 python =
   3.8: py38
   3.9: py39
   3.10: py310
```

