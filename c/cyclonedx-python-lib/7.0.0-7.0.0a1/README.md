# Comparing `tmp/cyclonedx_python_lib-7.0.0.tar.gz` & `tmp/cyclonedx_python_lib-7.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx_python_lib-7.0.0.tar", max compression
+gzip compressed data, was "cyclonedx_python_lib-7.0.0a1.tar", max compression
```

## Comparing `cyclonedx_python_lib-7.0.0.tar` & `cyclonedx_python_lib-7.0.0a1.tar`

### file list

```diff
@@ -1,1135 +1,1135 @@
--rw-r--r--   0        0        0   229011 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/LICENSE
--rw-r--r--   0        0        0      147 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/NOTICE
--rw-r--r--   0        0        0     4569 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/README.md
--rw-r--r--   0        0        0      850 2024-04-09 15:24:42.710933 cyclonedx_python_lib-7.0.0/cyclonedx/__init__.py
--rw-r--r--   0        0        0      731 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/_internal/__init__.py
--rw-r--r--   0        0        0     1734 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/_internal/compare.py
--rw-r--r--   0        0        0     1164 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/_internal/hash.py
--rw-r--r--   0        0        0      847 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/_internal/time.py
--rw-r--r--   0        0        0      993 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/exception/__init__.py
--rw-r--r--   0        0        0     1536 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/exception/factory.py
--rw-r--r--   0        0        0     3685 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/exception/model.py
--rw-r--r--   0        0        0     1136 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/exception/output.py
--rw-r--r--   0        0        0     1730 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/exception/serialization.py
--rw-r--r--   0        0        0      680 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/factory/__init__.py
--rw-r--r--   0        0        0     3233 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/factory/license.py
--rw-r--r--   0        0        0    43540 2024-04-09 15:24:21.982841 cyclonedx_python_lib-7.0.0/cyclonedx/model/__init__.py
--rw-r--r--   0        0        0    25088 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/bom.py
--rw-r--r--   0        0        0     2179 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/bom_ref.py
--rw-r--r--   0        0        0    57519 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/component.py
--rw-r--r--   0        0        0    11789 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/contact.py
--rw-r--r--   0        0        0    48270 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/crypto.py
--rw-r--r--   0        0        0     3766 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/dependency.py
--rw-r--r--   0        0        0     3568 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/impact_analysis.py
--rw-r--r--   0        0        0     7024 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/issue.py
--rw-r--r--   0        0        0    10127 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/license.py
--rw-r--r--   0        0        0     8623 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/release_note.py
--rw-r--r--   0        0        0    12798 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/service.py
--rw-r--r--   0        0        0    43655 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/model/vulnerability.py
--rw-r--r--   0        0        0     5872 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/output/__init__.py
--rw-r--r--   0        0        0     4270 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/output/json.py
--rw-r--r--   0        0        0     4285 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/output/xml.py
--rw-r--r--   0        0        0      153 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/py.typed
--rw-r--r--   0        0        0     3018 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/__init__.py
--rw-r--r--   0        0        0     2127 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/README.md
--rw-r--r--   0        0        0     2493 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/__init__.py
--rw-r--r--   0        0        0    13604 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd
--rw-r--r--   0        0        0    39716 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd
--rw-r--r--   0        0        0    37194 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    36226 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    76383 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd
--rw-r--r--   0        0        0    40408 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    39348 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    88794 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd
--rw-r--r--   0        0        0    72383 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   133792 2024-04-09 15:24:21.986841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd
--rw-r--r--   0        0        0   164772 2024-04-09 15:24:21.990841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   311805 2024-04-09 15:24:21.990841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd
--rw-r--r--   0        0        0   252643 2024-04-09 15:24:21.990841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   492947 2024-04-09 15:24:21.990841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd
--rw-r--r--   0        0        0     8058 2024-04-09 15:24:21.990841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    14269 2024-04-09 15:24:21.990841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   165694 2024-04-09 15:24:21.990841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd
--rw-r--r--   0        0        0     2573 2024-04-09 15:24:21.990841 cyclonedx_python_lib-7.0.0/cyclonedx/schema/schema.py
--rw-r--r--   0        0        0     6576 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/cyclonedx/serialization/__init__.py
--rw-r--r--   0        0        0     2503 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/cyclonedx/spdx.py
--rw-r--r--   0        0        0     3701 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/cyclonedx/validation/__init__.py
--rw-r--r--   0        0        0     4817 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/cyclonedx/validation/json.py
--rw-r--r--   0        0        0      853 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/cyclonedx/validation/model.py
--rw-r--r--   0        0        0     3672 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/cyclonedx/validation/xml.py
--rw-r--r--   0        0        0      634 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/Makefile
--rw-r--r--   0        0        0     1524 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/architecture.rst
--rw-r--r--   0        0        0      686 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/changelog.rst
--rw-r--r--   0        0        0     2657 2024-04-09 15:24:42.710933 cyclonedx_python_lib-7.0.0/docs/conf.py
--rw-r--r--   0        0        0       34 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/contributing.rst
--rw-r--r--   0        0        0      895 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/examples.rst
--rw-r--r--   0        0        0     1857 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/index.rst
--rw-r--r--   0        0        0     1499 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/install.rst
--rw-r--r--   0        0        0      800 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/make.bat
--rw-r--r--   0        0        0     3275 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/modelling.rst
--rw-r--r--   0        0        0     2269 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/outputting.rst
--rw-r--r--   0        0        0       81 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     4961 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/schema-support.rst
--rw-r--r--   0        0        0     1329 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/docs/support.rst
--rw-r--r--   0        0        0      176 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/examples/README.md
--rw-r--r--   0        0        0     8164 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/examples/complex_deserialize.py
--rw-r--r--   0        0        0     4081 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/examples/complex_serialize.py
--rw-r--r--   0        0        0     4227 2024-04-09 15:24:42.710933 cyclonedx_python_lib-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     6717 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/__init__.py
--rw-r--r--   0        0        0      704 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/__init__.py
--rw-r--r--   0        0        0    42334 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/models.py
--rw-r--r--   0        0        0       16 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/own/README.md
--rw-r--r--   0        0        0     1309 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/own/json/1.2/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1309 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/own/json/1.3/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1309 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/own/json/1.4/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     2461 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/own/xml/1.4/bom_setuptools.xml
--rw-r--r--   0        0        0    98508 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/own/xml/1.4/webgoat-6.1.xml
--rw-r--r--   0        0        0     3723 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml
--rw-r--r--   0        0        0     1195 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml
--rw-r--r--   0        0        0      559 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml
--rw-r--r--   0        0        0      313 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-component-type-1.1.xml
--rw-r--r--   0        0        0      246 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-empty-component-1.1.xml
--rw-r--r--   0        0        0      830 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml
--rw-r--r--   0        0        0      801 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml
--rw-r--r--   0        0        0      793 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml
--rw-r--r--   0        0        0      769 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml
--rw-r--r--   0        0        0      705 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml
--rw-r--r--   0        0        0     1303 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml
--rw-r--r--   0        0        0    16515 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml
--rw-r--r--   0        0        0    16513 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml
--rw-r--r--   0        0        0     1328 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml
--rw-r--r--   0        0        0     1366 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml
--rw-r--r--   0        0        0      302 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-missing-component-type-1.1.xml
--rw-r--r--   0        0        0    21038 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml
--rw-r--r--   0        0        0      348 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-scope-1.1.xml
--rw-r--r--   0        0        0    21026 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml
--rw-r--r--   0        0        0    21039 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml
--rw-r--r--   0        0        0     1217 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml
--rw-r--r--   0        0        0      704 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml
--rw-r--r--   0        0        0      965 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml
--rw-r--r--   0        0        0      186 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-empty-components-1.1.xml
--rw-r--r--   0        0        0    22339 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml
--rw-r--r--   0        0        0     1210 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml
--rw-r--r--   0        0        0     1214 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml
--rw-r--r--   0        0        0     1226 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml
--rw-r--r--   0        0        0      317 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-minimal-viable-1.1.xml
--rw-r--r--   0        0        0    21121 2024-04-09 15:24:21.994841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml
--rw-r--r--   0        0        0    10048 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml
--rw-r--r--   0        0        0      165 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-bomformat-1.2.json
--rw-r--r--   0        0        0      394 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.json
--rw-r--r--   0        0        0      560 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml
--rw-r--r--   0        0        0      385 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.json
--rw-r--r--   0        0        0      433 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.xml
--rw-r--r--   0        0        0      249 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.json
--rw-r--r--   0        0        0      314 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.xml
--rw-r--r--   0        0        0      667 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json
--rw-r--r--   0        0        0      809 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml
--rw-r--r--   0        0        0      247 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-empty-component-1.2.xml
--rw-r--r--   0        0        0      856 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json
--rw-r--r--   0        0        0      831 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml
--rw-r--r--   0        0        0      827 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json
--rw-r--r--   0        0        0      802 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml
--rw-r--r--   0        0        0      819 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json
--rw-r--r--   0        0        0      794 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml
--rw-r--r--   0        0        0      795 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json
--rw-r--r--   0        0        0      770 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml
--rw-r--r--   0        0        0      731 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json
--rw-r--r--   0        0        0      706 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml
--rw-r--r--   0        0        0     1184 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json
--rw-r--r--   0        0        0     1554 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml
--rw-r--r--   0        0        0      515 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json
--rw-r--r--   0        0        0     1304 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml
--rw-r--r--   0        0        0    15788 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json
--rw-r--r--   0        0        0    16516 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml
--rw-r--r--   0        0        0      428 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.json
--rw-r--r--   0        0        0    16514 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml
--rw-r--r--   0        0        0     1329 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml
--rw-r--r--   0        0        0     1367 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml
--rw-r--r--   0        0        0      209 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      244 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      303 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-missing-component-type-1.2.xml
--rw-r--r--   0        0        0    21039 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml
--rw-r--r--   0        0        0     1185 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json
--rw-r--r--   0        0        0     1555 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml
--rw-r--r--   0        0        0      275 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-scope-1.2.json
--rw-r--r--   0        0        0      349 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-scope-1.2.xml
--rw-r--r--   0        0        0      148 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.json
--rw-r--r--   0        0        0    21027 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml
--rw-r--r--   0        0        0      430 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.json
--rw-r--r--   0        0        0      416 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.xml
--rw-r--r--   0        0        0      363 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/skip_invalid-empty-component-1.2.json
--rw-r--r--   0        0        0      361 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/skip_invalid-missing-component-type-1.2.json
--rw-r--r--   0        0        0      548 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json
--rw-r--r--   0        0        0      792 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml
--rw-r--r--   0        0        0    20390 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.json
--rw-r--r--   0        0        0    24278 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml
--rw-r--r--   0        0        0     2163 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json
--rw-r--r--   0        0        0     1897 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml
--rw-r--r--   0        0        0      394 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.json
--rw-r--r--   0        0        0      705 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml
--rw-r--r--   0        0        0      456 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.json
--rw-r--r--   0        0        0      492 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.xml
--rw-r--r--   0        0        0     1342 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json
--rw-r--r--   0        0        0     1346 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml
--rw-r--r--   0        0        0      892 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json
--rw-r--r--   0        0        0     1223 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml
--rw-r--r--   0        0        0      693 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json
--rw-r--r--   0        0        0      824 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml
--rw-r--r--   0        0        0      161 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.json
--rw-r--r--   0        0        0      187 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.xml
--rw-r--r--   0        0        0    22340 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml
--rw-r--r--   0        0        0      438 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.json
--rw-r--r--   0        0        0     1211 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml
--rw-r--r--   0        0        0      430 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.json
--rw-r--r--   0        0        0     1215 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml
--rw-r--r--   0        0        0      440 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.json
--rw-r--r--   0        0        0     1227 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml
--rw-r--r--   0        0        0      333 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.json
--rw-r--r--   0        0        0      430 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.xml
--rw-r--r--   0        0        0      438 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.json
--rw-r--r--   0        0        0      492 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.xml
--rw-r--r--   0        0        0      417 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.json
--rw-r--r--   0        0        0      468 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.xml
--rw-r--r--   0        0        0      224 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      254 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      605 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json
--rw-r--r--   0        0        0      654 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml
--rw-r--r--   0        0        0      253 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.json
--rw-r--r--   0        0        0      318 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.xml
--rw-r--r--   0        0        0     2465 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.json
--rw-r--r--   0        0        0     3337 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml
--rw-r--r--   0        0        0    21122 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml
--rw-r--r--   0        0        0     2308 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-service-1.2.json
--rw-r--r--   0        0        0     2693 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-service-1.2.xml
--rw-r--r--   0        0        0      419 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.json
--rw-r--r--   0        0        0      495 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.xml
--rw-r--r--   0        0        0    11181 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml
--rw-r--r--   0        0        0      165 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-bomformat-1.3.json
--rw-r--r--   0        0        0      394 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.json
--rw-r--r--   0        0        0      560 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml
--rw-r--r--   0        0        0      385 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.json
--rw-r--r--   0        0        0      433 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.xml
--rw-r--r--   0        0        0      249 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.json
--rw-r--r--   0        0        0      314 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.xml
--rw-r--r--   0        0        0      667 2024-04-09 15:24:21.998841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json
--rw-r--r--   0        0        0      809 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml
--rw-r--r--   0        0        0      197 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.json
--rw-r--r--   0        0        0      247 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.xml
--rw-r--r--   0        0        0      856 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json
--rw-r--r--   0        0        0      831 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml
--rw-r--r--   0        0        0      827 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json
--rw-r--r--   0        0        0      802 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml
--rw-r--r--   0        0        0      819 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json
--rw-r--r--   0        0        0      794 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml
--rw-r--r--   0        0        0      795 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json
--rw-r--r--   0        0        0      770 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml
--rw-r--r--   0        0        0      731 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json
--rw-r--r--   0        0        0      706 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml
--rw-r--r--   0        0        0     1184 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json
--rw-r--r--   0        0        0     1554 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml
--rw-r--r--   0        0        0      515 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json
--rw-r--r--   0        0        0     1304 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml
--rw-r--r--   0        0        0    15788 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json
--rw-r--r--   0        0        0    16516 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml
--rw-r--r--   0        0        0      428 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.json
--rw-r--r--   0        0        0    16514 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml
--rw-r--r--   0        0        0     1329 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml
--rw-r--r--   0        0        0     1367 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml
--rw-r--r--   0        0        0      277 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.json
--rw-r--r--   0        0        0      319 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      209 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      244 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      228 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.json
--rw-r--r--   0        0        0      303 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.xml
--rw-r--r--   0        0        0    21039 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml
--rw-r--r--   0        0        0     1185 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json
--rw-r--r--   0        0        0     1555 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml
--rw-r--r--   0        0        0      275 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-scope-1.3.json
--rw-r--r--   0        0        0      349 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-scope-1.3.xml
--rw-r--r--   0        0        0      148 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.json
--rw-r--r--   0        0        0    21027 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.json
--rw-r--r--   0        0        0      416 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.xml
--rw-r--r--   0        0        0      548 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json
--rw-r--r--   0        0        0      792 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml
--rw-r--r--   0        0        0    20390 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.json
--rw-r--r--   0        0        0    24278 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml
--rw-r--r--   0        0        0     2163 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json
--rw-r--r--   0        0        0     1897 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml
--rw-r--r--   0        0        0      394 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.json
--rw-r--r--   0        0        0      705 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml
--rw-r--r--   0        0        0      456 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.json
--rw-r--r--   0        0        0      492 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.xml
--rw-r--r--   0        0        0     1342 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json
--rw-r--r--   0        0        0     1346 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml
--rw-r--r--   0        0        0      892 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json
--rw-r--r--   0        0        0     1223 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml
--rw-r--r--   0        0        0     1497 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json
--rw-r--r--   0        0        0     1983 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml
--rw-r--r--   0        0        0      693 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json
--rw-r--r--   0        0        0      824 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml
--rw-r--r--   0        0        0      161 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.json
--rw-r--r--   0        0        0      187 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.xml
--rw-r--r--   0        0        0     1384 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json
--rw-r--r--   0        0        0     1596 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml
--rw-r--r--   0        0        0    22340 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml
--rw-r--r--   0        0        0     1117 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json
--rw-r--r--   0        0        0     1324 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml
--rw-r--r--   0        0        0      438 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.json
--rw-r--r--   0        0        0     1211 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.json
--rw-r--r--   0        0        0     1215 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml
--rw-r--r--   0        0        0      440 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.json
--rw-r--r--   0        0        0     1227 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml
--rw-r--r--   0        0        0      333 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.json
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.xml
--rw-r--r--   0        0        0      279 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.json
--rw-r--r--   0        0        0      321 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      438 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.json
--rw-r--r--   0        0        0      492 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.xml
--rw-r--r--   0        0        0      417 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.json
--rw-r--r--   0        0        0      468 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.xml
--rw-r--r--   0        0        0      224 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      254 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      605 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json
--rw-r--r--   0        0        0      654 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml
--rw-r--r--   0        0        0      253 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.json
--rw-r--r--   0        0        0      318 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.xml
--rw-r--r--   0        0        0     2465 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.json
--rw-r--r--   0        0        0     3337 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml
--rw-r--r--   0        0        0      983 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.json
--rw-r--r--   0        0        0     1213 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml
--rw-r--r--   0        0        0    21122 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml
--rw-r--r--   0        0        0     2308 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-service-1.3.json
--rw-r--r--   0        0        0     2693 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-service-1.3.xml
--rw-r--r--   0        0        0      419 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.json
--rw-r--r--   0        0        0      495 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.xml
--rw-r--r--   0        0        0    11181 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml
--rw-r--r--   0        0        0      165 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-bomformat-1.4.json
--rw-r--r--   0        0        0      394 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.json
--rw-r--r--   0        0        0      560 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml
--rw-r--r--   0        0        0      385 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.json
--rw-r--r--   0        0        0      433 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.xml
--rw-r--r--   0        0        0      249 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.json
--rw-r--r--   0        0        0      314 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.xml
--rw-r--r--   0        0        0      667 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json
--rw-r--r--   0        0        0      809 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml
--rw-r--r--   0        0        0      197 2024-04-09 15:24:22.002841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.json
--rw-r--r--   0        0        0      247 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.xml
--rw-r--r--   0        0        0      856 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json
--rw-r--r--   0        0        0      831 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml
--rw-r--r--   0        0        0      827 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json
--rw-r--r--   0        0        0      802 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml
--rw-r--r--   0        0        0      819 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json
--rw-r--r--   0        0        0      794 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml
--rw-r--r--   0        0        0      795 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json
--rw-r--r--   0        0        0      770 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml
--rw-r--r--   0        0        0      731 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json
--rw-r--r--   0        0        0      706 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml
--rw-r--r--   0        0        0     1184 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json
--rw-r--r--   0        0        0     1554 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml
--rw-r--r--   0        0        0      515 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json
--rw-r--r--   0        0        0     1304 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml
--rw-r--r--   0        0        0    15788 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json
--rw-r--r--   0        0        0    16516 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml
--rw-r--r--   0        0        0      428 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.json
--rw-r--r--   0        0        0    16514 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml
--rw-r--r--   0        0        0     1329 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml
--rw-r--r--   0        0        0     1367 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml
--rw-r--r--   0        0        0      277 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.json
--rw-r--r--   0        0        0      319 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      209 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      244 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      228 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.json
--rw-r--r--   0        0        0      303 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.xml
--rw-r--r--   0        0        0    21039 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml
--rw-r--r--   0        0        0     1185 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json
--rw-r--r--   0        0        0     1555 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml
--rw-r--r--   0        0        0      275 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-scope-1.4.json
--rw-r--r--   0        0        0      349 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-scope-1.4.xml
--rw-r--r--   0        0        0      148 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.json
--rw-r--r--   0        0        0    21027 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.json
--rw-r--r--   0        0        0      416 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.xml
--rw-r--r--   0        0        0      548 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json
--rw-r--r--   0        0        0      792 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml
--rw-r--r--   0        0        0    20390 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.json
--rw-r--r--   0        0        0    24278 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml
--rw-r--r--   0        0        0     2163 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json
--rw-r--r--   0        0        0     1897 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml
--rw-r--r--   0        0        0      394 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.json
--rw-r--r--   0        0        0      705 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml
--rw-r--r--   0        0        0      456 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.json
--rw-r--r--   0        0        0      492 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.xml
--rw-r--r--   0        0        0     1342 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json
--rw-r--r--   0        0        0     1346 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml
--rw-r--r--   0        0        0      892 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json
--rw-r--r--   0        0        0     1223 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml
--rw-r--r--   0        0        0     1497 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json
--rw-r--r--   0        0        0     1983 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml
--rw-r--r--   0        0        0      693 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json
--rw-r--r--   0        0        0      824 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml
--rw-r--r--   0        0        0      161 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.json
--rw-r--r--   0        0        0      187 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.xml
--rw-r--r--   0        0        0     1384 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json
--rw-r--r--   0        0        0     1596 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml
--rw-r--r--   0        0        0    22340 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml
--rw-r--r--   0        0        0     1117 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json
--rw-r--r--   0        0        0     1324 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml
--rw-r--r--   0        0        0      438 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.json
--rw-r--r--   0        0        0     1211 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.json
--rw-r--r--   0        0        0     1215 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml
--rw-r--r--   0        0        0      440 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.json
--rw-r--r--   0        0        0     1227 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml
--rw-r--r--   0        0        0      333 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.json
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.xml
--rw-r--r--   0        0        0      279 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.json
--rw-r--r--   0        0        0      321 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      438 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.json
--rw-r--r--   0        0        0      492 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.xml
--rw-r--r--   0        0        0      417 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.json
--rw-r--r--   0        0        0      468 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.xml
--rw-r--r--   0        0        0      224 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      254 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      605 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json
--rw-r--r--   0        0        0      654 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml
--rw-r--r--   0        0        0      227 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.json
--rw-r--r--   0        0        0      281 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.xml
--rw-r--r--   0        0        0     2465 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.json
--rw-r--r--   0        0        0     3337 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml
--rw-r--r--   0        0        0      983 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.json
--rw-r--r--   0        0        0     1213 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml
--rw-r--r--   0        0        0    21122 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml
--rw-r--r--   0        0        0     5338 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json
--rw-r--r--   0        0        0     6828 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml
--rw-r--r--   0        0        0     2312 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-service-1.4.json
--rw-r--r--   0        0        0     2693 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-service-1.4.xml
--rw-r--r--   0        0        0      419 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.json
--rw-r--r--   0        0        0      495 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.xml
--rw-r--r--   0        0        0     9733 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json
--rw-r--r--   0        0        0     4274 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json
--rw-r--r--   0        0        0     5987 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml
--rw-r--r--   0        0        0    11181 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml
--rw-r--r--   0        0        0      165 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-bomformat-1.5.json
--rw-r--r--   0        0        0      508 2024-04-09 15:24:22.006842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.json
--rw-r--r--   0        0        0      866 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml
--rw-r--r--   0        0        0      385 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.json
--rw-r--r--   0        0        0      433 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.xml
--rw-r--r--   0        0        0      249 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.json
--rw-r--r--   0        0        0      314 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.xml
--rw-r--r--   0        0        0      746 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json
--rw-r--r--   0        0        0     1086 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml
--rw-r--r--   0        0        0      197 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.json
--rw-r--r--   0        0        0      247 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.xml
--rw-r--r--   0        0        0      856 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json
--rw-r--r--   0        0        0      831 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml
--rw-r--r--   0        0        0      827 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json
--rw-r--r--   0        0        0      802 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml
--rw-r--r--   0        0        0      819 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json
--rw-r--r--   0        0        0      794 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml
--rw-r--r--   0        0        0      795 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json
--rw-r--r--   0        0        0      770 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml
--rw-r--r--   0        0        0      731 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json
--rw-r--r--   0        0        0      706 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml
--rw-r--r--   0        0        0     1184 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json
--rw-r--r--   0        0        0     1554 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml
--rw-r--r--   0        0        0      515 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json
--rw-r--r--   0        0        0     1304 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml
--rw-r--r--   0        0        0    15788 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json
--rw-r--r--   0        0        0    16516 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml
--rw-r--r--   0        0        0      428 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.json
--rw-r--r--   0        0        0    16514 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml
--rw-r--r--   0        0        0     1329 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml
--rw-r--r--   0        0        0     1367 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml
--rw-r--r--   0        0        0      277 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.json
--rw-r--r--   0        0        0      319 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      209 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      244 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0      228 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.json
--rw-r--r--   0        0        0      303 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.xml
--rw-r--r--   0        0        0    21039 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml
--rw-r--r--   0        0        0     1185 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json
--rw-r--r--   0        0        0     1555 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml
--rw-r--r--   0        0        0      275 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-scope-1.5.json
--rw-r--r--   0        0        0      349 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-scope-1.5.xml
--rw-r--r--   0        0        0      148 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.json
--rw-r--r--   0        0        0    21027 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.json
--rw-r--r--   0        0        0      416 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.xml
--rw-r--r--   0        0        0     2527 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json
--rw-r--r--   0        0        0     3596 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml
--rw-r--r--   0        0        0      548 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json
--rw-r--r--   0        0        0      792 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml
--rw-r--r--   0        0        0    20390 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.json
--rw-r--r--   0        0        0    24278 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml
--rw-r--r--   0        0        0     2163 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json
--rw-r--r--   0        0        0     1897 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml
--rw-r--r--   0        0        0      394 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.json
--rw-r--r--   0        0        0      705 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml
--rw-r--r--   0        0        0      456 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.json
--rw-r--r--   0        0        0      492 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.xml
--rw-r--r--   0        0        0     1342 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json
--rw-r--r--   0        0        0     1346 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml
--rw-r--r--   0        0        0      892 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json
--rw-r--r--   0        0        0     1223 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml
--rw-r--r--   0        0        0     1810 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json
--rw-r--r--   0        0        0     2449 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml
--rw-r--r--   0        0        0      693 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json
--rw-r--r--   0        0        0      824 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml
--rw-r--r--   0        0        0      161 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.json
--rw-r--r--   0        0        0      187 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.xml
--rw-r--r--   0        0        0     3189 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json
--rw-r--r--   0        0        0     4519 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml
--rw-r--r--   0        0        0    22340 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml
--rw-r--r--   0        0        0     1117 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json
--rw-r--r--   0        0        0     1324 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml
--rw-r--r--   0        0        0     7703 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json
--rw-r--r--   0        0        0    11757 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml
--rw-r--r--   0        0        0      473 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.json
--rw-r--r--   0        0        0     1270 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml
--rw-r--r--   0        0        0      467 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.json
--rw-r--r--   0        0        0     1236 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml
--rw-r--r--   0        0        0     1539 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json
--rw-r--r--   0        0        0     2197 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml
--rw-r--r--   0        0        0      477 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.json
--rw-r--r--   0        0        0     1248 2024-04-09 15:24:22.010841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml
--rw-r--r--   0        0        0    98548 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json
--rw-r--r--   0        0        0   100112 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml
--rw-r--r--   0        0        0      333 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.json
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.xml
--rw-r--r--   0        0        0      279 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.json
--rw-r--r--   0        0        0      321 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      436 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.json
--rw-r--r--   0        0        0      624 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml
--rw-r--r--   0        0        0      507 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.json
--rw-r--r--   0        0        0      537 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml
--rw-r--r--   0        0        0      482 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.json
--rw-r--r--   0        0        0      509 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.xml
--rw-r--r--   0        0        0      224 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      254 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0     1162 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json
--rw-r--r--   0        0        0     1471 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml
--rw-r--r--   0        0        0      605 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json
--rw-r--r--   0        0        0      654 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml
--rw-r--r--   0        0        0      227 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.json
--rw-r--r--   0        0        0      281 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.xml
--rw-r--r--   0        0        0     2465 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.json
--rw-r--r--   0        0        0     3337 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml
--rw-r--r--   0        0        0     1520 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.json
--rw-r--r--   0        0        0     1660 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml
--rw-r--r--   0        0        0    21122 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml
--rw-r--r--   0        0        0     5338 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json
--rw-r--r--   0        0        0     6828 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml
--rw-r--r--   0        0        0     9412 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json
--rw-r--r--   0        0        0    12249 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml
--rw-r--r--   0        0        0     2312 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-service-1.5.json
--rw-r--r--   0        0        0     2693 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-service-1.5.xml
--rw-r--r--   0        0        0      419 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.json
--rw-r--r--   0        0        0      495 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.xml
--rw-r--r--   0        0        0     9733 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json
--rw-r--r--   0        0        0    17746 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json
--rw-r--r--   0        0        0    19794 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml
--rw-r--r--   0        0        0    11181 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml
--rw-r--r--   0        0        0      165 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-bomformat-1.6.json
--rw-r--r--   0        0        0      508 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.json
--rw-r--r--   0        0        0      866 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml
--rw-r--r--   0        0        0      385 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.json
--rw-r--r--   0        0        0      433 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.xml
--rw-r--r--   0        0        0      249 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.json
--rw-r--r--   0        0        0      314 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.xml
--rw-r--r--   0        0        0      746 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json
--rw-r--r--   0        0        0     1086 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml
--rw-r--r--   0        0        0      197 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.json
--rw-r--r--   0        0        0      247 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.xml
--rw-r--r--   0        0        0      856 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json
--rw-r--r--   0        0        0      831 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml
--rw-r--r--   0        0        0      827 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json
--rw-r--r--   0        0        0      802 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml
--rw-r--r--   0        0        0      819 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json
--rw-r--r--   0        0        0      794 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml
--rw-r--r--   0        0        0      795 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json
--rw-r--r--   0        0        0      770 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml
--rw-r--r--   0        0        0      731 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json
--rw-r--r--   0        0        0      706 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml
--rw-r--r--   0        0        0     1184 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json
--rw-r--r--   0        0        0     1554 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml
--rw-r--r--   0        0        0      515 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json
--rw-r--r--   0        0        0     1304 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml
--rw-r--r--   0        0        0    15788 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json
--rw-r--r--   0        0        0    16516 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml
--rw-r--r--   0        0        0      428 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.json
--rw-r--r--   0        0        0    16514 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml
--rw-r--r--   0        0        0     1329 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml
--rw-r--r--   0        0        0      360 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.json
--rw-r--r--   0        0        0      466 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.xml
--rw-r--r--   0        0        0     1367 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml
--rw-r--r--   0        0        0      277 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.json
--rw-r--r--   0        0        0      319 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.xml
--rw-r--r--   0        0        0      209 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.json
--rw-r--r--   0        0        0      244 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.xml
--rw-r--r--   0        0        0      228 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.json
--rw-r--r--   0        0        0      303 2024-04-09 15:24:22.014841 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.xml
--rw-r--r--   0        0        0    21039 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml
--rw-r--r--   0        0        0     1185 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json
--rw-r--r--   0        0        0     1555 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml
--rw-r--r--   0        0        0     1290 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json
--rw-r--r--   0        0        0     1504 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml
--rw-r--r--   0        0        0      275 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-scope-1.6.json
--rw-r--r--   0        0        0      349 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-scope-1.6.xml
--rw-r--r--   0        0        0      148 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.json
--rw-r--r--   0        0        0    21027 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.json
--rw-r--r--   0        0        0      416 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.xml
--rw-r--r--   0        0        0     2527 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json
--rw-r--r--   0        0        0     3596 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml
--rw-r--r--   0        0        0      548 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json
--rw-r--r--   0        0        0      792 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml
--rw-r--r--   0        0        0     5654 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json
--rw-r--r--   0        0        0     7084 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml
--rw-r--r--   0        0        0     6538 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.json
--rw-r--r--   0        0        0    24921 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml
--rw-r--r--   0        0        0     2163 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json
--rw-r--r--   0        0        0     1897 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml
--rw-r--r--   0        0        0      750 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json
--rw-r--r--   0        0        0      865 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml
--rw-r--r--   0        0        0      394 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.json
--rw-r--r--   0        0        0      705 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml
--rw-r--r--   0        0        0      456 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.json
--rw-r--r--   0        0        0      492 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.xml
--rw-r--r--   0        0        0     1342 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json
--rw-r--r--   0        0        0     1346 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml
--rw-r--r--   0        0        0      892 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json
--rw-r--r--   0        0        0     1223 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml
--rw-r--r--   0        0        0     1810 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json
--rw-r--r--   0        0        0     2449 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml
--rw-r--r--   0        0        0     2978 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json
--rw-r--r--   0        0        0     4629 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml
--rw-r--r--   0        0        0     1459 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json
--rw-r--r--   0        0        0     2217 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml
--rw-r--r--   0        0        0      693 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json
--rw-r--r--   0        0        0      824 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml
--rw-r--r--   0        0        0      161 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.json
--rw-r--r--   0        0        0      187 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.xml
--rw-r--r--   0        0        0     4432 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json
--rw-r--r--   0        0        0     6383 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml
--rw-r--r--   0        0        0    22340 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml
--rw-r--r--   0        0        0     1117 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json
--rw-r--r--   0        0        0     1324 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml
--rw-r--r--   0        0        0     7703 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json
--rw-r--r--   0        0        0    11757 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml
--rw-r--r--   0        0        0      514 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json
--rw-r--r--   0        0        0     1297 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml
--rw-r--r--   0        0        0      510 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.json
--rw-r--r--   0        0        0     1263 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml
--rw-r--r--   0        0        0     1539 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json
--rw-r--r--   0        0        0     2197 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml
--rw-r--r--   0        0        0      477 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.json
--rw-r--r--   0        0        0     1248 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml
--rw-r--r--   0        0        0    98548 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json
--rw-r--r--   0        0        0   100112 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml
--rw-r--r--   0        0        0     1835 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json
--rw-r--r--   0        0        0     2811 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml
--rw-r--r--   0        0        0      333 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.json
--rw-r--r--   0        0        0      430 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.xml
--rw-r--r--   0        0        0      432 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.json
--rw-r--r--   0        0        0      456 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.xml
--rw-r--r--   0        0        0      436 2024-04-09 15:24:22.018842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.json
--rw-r--r--   0        0        0      624 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml
--rw-r--r--   0        0        0      521 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json
--rw-r--r--   0        0        0      551 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml
--rw-r--r--   0        0        0      508 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.json
--rw-r--r--   0        0        0      539 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml
--rw-r--r--   0        0        0      482 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.json
--rw-r--r--   0        0        0      509 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.xml
--rw-r--r--   0        0        0      224 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.json
--rw-r--r--   0        0        0      254 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.xml
--rw-r--r--   0        0        0     1162 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json
--rw-r--r--   0        0        0     1471 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml
--rw-r--r--   0        0        0      605 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json
--rw-r--r--   0        0        0      654 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml
--rw-r--r--   0        0        0      227 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.json
--rw-r--r--   0        0        0      281 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.xml
--rw-r--r--   0        0        0     2465 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.json
--rw-r--r--   0        0        0     3337 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml
--rw-r--r--   0        0        0     1894 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.json
--rw-r--r--   0        0        0     1872 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml
--rw-r--r--   0        0        0    21122 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml
--rw-r--r--   0        0        0     5338 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json
--rw-r--r--   0        0        0     6828 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml
--rw-r--r--   0        0        0     9412 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json
--rw-r--r--   0        0        0    12249 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml
--rw-r--r--   0        0        0     2312 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-service-1.6.json
--rw-r--r--   0        0        0     2693 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-service-1.6.xml
--rw-r--r--   0        0        0      419 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.json
--rw-r--r--   0        0        0      495 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.xml
--rw-r--r--   0        0        0     9733 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json
--rw-r--r--   0        0        0     1902 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.json
--rw-r--r--   0        0        0     2747 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml
--rw-r--r--   0        0        0      491 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.json
--rw-r--r--   0        0        0      870 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml
--rw-r--r--   0        0        0    17746 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json
--rw-r--r--   0        0        0    19794 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml
--rw-r--r--   0        0        0    11181 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml
--rw-r--r--   0        0        0      157 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/README.md
--rwxr-xr-x   0        0        0      745 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/fetch.sh
--rw-r--r--   0        0        0      391 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/README.md
--rw-r--r--   0        0        0      579 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin
--rw-r--r--   0        0        0      649 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin
--rw-r--r--   0        0        0     1050 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin
--rw-r--r--   0        0        0     1055 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin
--rw-r--r--   0        0        0     1050 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin
--rw-r--r--   0        0        0     1055 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin
--rw-r--r--   0        0        0     2128 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin
--rw-r--r--   0        0        0     2211 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin
--rw-r--r--   0        0        0     2128 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin
--rw-r--r--   0        0        0     2211 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin
--rw-r--r--   0        0        0     2128 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin
--rw-r--r--   0        0        0     2211 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin
--rw-r--r--   0        0        0      806 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin
--rw-r--r--   0        0        0      949 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin
--rw-r--r--   0        0        0     1835 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.2.json.bin
--rw-r--r--   0        0        0     1806 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin
--rw-r--r--   0        0        0     1835 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.3.json.bin
--rw-r--r--   0        0        0     1806 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin
--rw-r--r--   0        0        0     2808 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.4.json.bin
--rw-r--r--   0        0        0     2877 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin
--rw-r--r--   0        0        0     3460 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.5.json.bin
--rw-r--r--   0        0        0     3525 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin
--rw-r--r--   0        0        0     3652 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.6.json.bin
--rw-r--r--   0        0        0     3716 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.1.xml.bin
--rw-r--r--   0        0        0      944 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.2.json.bin
--rw-r--r--   0        0        0      865 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin
--rw-r--r--   0        0        0      944 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.3.json.bin
--rw-r--r--   0        0        0      865 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin
--rw-r--r--   0        0        0     2085 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.4.json.bin
--rw-r--r--   0        0        0     2072 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin
--rw-r--r--   0        0        0     2085 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.5.json.bin
--rw-r--r--   0        0        0     2072 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin
--rw-r--r--   0        0        0     2085 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.6.json.bin
--rw-r--r--   0        0        0     2072 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.0.xml.bin
--rw-r--r--   0        0        0      496 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.1.xml.bin
--rw-r--r--   0        0        0      893 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.2.json.bin
--rw-r--r--   0        0        0      812 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.2.xml.bin
--rw-r--r--   0        0        0      893 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.3.json.bin
--rw-r--r--   0        0        0      812 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.3.xml.bin
--rw-r--r--   0        0        0     2013 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.4.json.bin
--rw-r--r--   0        0        0     2002 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.4.xml.bin
--rw-r--r--   0        0        0     2013 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.5.json.bin
--rw-r--r--   0        0        0     2002 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.5.xml.bin
--rw-r--r--   0        0        0     2013 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.6.json.bin
--rw-r--r--   0        0        0     2002 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.0.xml.bin
--rw-r--r--   0        0        0     4485 2024-04-09 15:24:22.022842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin
--rw-r--r--   0        0        0     4434 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin
--rw-r--r--   0        0        0     4801 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin
--rw-r--r--   0        0        0     4434 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin
--rw-r--r--   0        0        0     4801 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin
--rw-r--r--   0        0        0     5562 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin
--rw-r--r--   0        0        0     5999 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin
--rw-r--r--   0        0        0     5811 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin
--rw-r--r--   0        0        0     6248 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin
--rw-r--r--   0        0        0     5855 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin
--rw-r--r--   0        0        0     6292 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin
--rw-r--r--   0        0        0      749 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin
--rw-r--r--   0        0        0      793 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin
--rw-r--r--   0        0        0     1894 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin
--rw-r--r--   0        0        0     1461 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin
--rw-r--r--   0        0        0     1894 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin
--rw-r--r--   0        0        0     1461 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin
--rw-r--r--   0        0        0     3014 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin
--rw-r--r--   0        0        0     2651 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin
--rw-r--r--   0        0        0     3014 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin
--rw-r--r--   0        0        0     2651 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin
--rw-r--r--   0        0        0     3014 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin
--rw-r--r--   0        0        0     2651 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.xml.bin
--rw-r--r--   0        0        0     2092 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin
--rw-r--r--   0        0        0     2289 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin
--rw-r--r--   0        0        0     2092 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin
--rw-r--r--   0        0        0     2289 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin
--rw-r--r--   0        0        0     2092 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin
--rw-r--r--   0        0        0     2289 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.xml.bin
--rw-r--r--   0        0        0     3282 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin
--rw-r--r--   0        0        0     3686 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin
--rw-r--r--   0        0        0     3282 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin
--rw-r--r--   0        0        0     3686 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin
--rw-r--r--   0        0        0     3282 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin
--rw-r--r--   0        0        0     3686 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.xml.bin
--rw-r--r--   0        0        0     1827 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin
--rw-r--r--   0        0        0     2023 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin
--rw-r--r--   0        0        0     1827 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin
--rw-r--r--   0        0        0     2023 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin
--rw-r--r--   0        0        0     1827 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin
--rw-r--r--   0        0        0     2023 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.xml.bin
--rw-r--r--   0        0        0     2577 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin
--rw-r--r--   0        0        0     2822 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin
--rw-r--r--   0        0        0     2577 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin
--rw-r--r--   0        0        0     2822 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin
--rw-r--r--   0        0        0     2577 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin
--rw-r--r--   0        0        0     2822 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.1.xml.bin
--rw-r--r--   0        0        0     1081 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin
--rw-r--r--   0        0        0     1083 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin
--rw-r--r--   0        0        0     1081 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin
--rw-r--r--   0        0        0     1083 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2201 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin
--rw-r--r--   0        0        0     2273 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2201 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin
--rw-r--r--   0        0        0     2273 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin
--rw-r--r--   0        0        0     2201 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin
--rw-r--r--   0        0        0     2273 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.1.xml.bin
--rw-r--r--   0        0        0      886 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin
--rw-r--r--   0        0        0      821 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin
--rw-r--r--   0        0        0      886 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin
--rw-r--r--   0        0        0      821 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2006 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin
--rw-r--r--   0        0        0     2011 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2006 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin
--rw-r--r--   0        0        0     2011 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin
--rw-r--r--   0        0        0     2006 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin
--rw-r--r--   0        0        0     2011 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.xml.bin
--rw-r--r--   0        0        0     2014 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin
--rw-r--r--   0        0        0     2243 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin
--rw-r--r--   0        0        0     2014 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin
--rw-r--r--   0        0        0     2243 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin
--rw-r--r--   0        0        0     2014 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin
--rw-r--r--   0        0        0     2243 2024-04-09 15:24:22.026841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.xml.bin
--rw-r--r--   0        0        0     2025 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin
--rw-r--r--   0        0        0     2268 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin
--rw-r--r--   0        0        0     2025 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin
--rw-r--r--   0        0        0     2268 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin
--rw-r--r--   0        0        0     2025 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin
--rw-r--r--   0        0        0     2268 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin
--rw-r--r--   0        0        0      596 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin
--rw-r--r--   0        0        0      695 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin
--rw-r--r--   0        0        0     1561 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin
--rw-r--r--   0        0        0     1597 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin
--rw-r--r--   0        0        0     1561 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin
--rw-r--r--   0        0        0     1597 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin
--rw-r--r--   0        0        0     2702 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin
--rw-r--r--   0        0        0     2804 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin
--rw-r--r--   0        0        0     2702 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin
--rw-r--r--   0        0        0     2804 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin
--rw-r--r--   0        0        0     2702 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin
--rw-r--r--   0        0        0     2804 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin
--rw-r--r--   0        0        0      662 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin
--rw-r--r--   0        0        0      678 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin
--rw-r--r--   0        0        0     1385 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin
--rw-r--r--   0        0        0     1402 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin
--rw-r--r--   0        0        0     1385 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin
--rw-r--r--   0        0        0     1402 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin
--rw-r--r--   0        0        0     2526 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin
--rw-r--r--   0        0        0     2609 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin
--rw-r--r--   0        0        0     2526 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin
--rw-r--r--   0        0        0     2609 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin
--rw-r--r--   0        0        0     2526 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin
--rw-r--r--   0        0        0     2609 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.0.xml.bin
--rw-r--r--   0        0        0      847 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin
--rw-r--r--   0        0        0     1085 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin
--rw-r--r--   0        0        0     1163 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin
--rw-r--r--   0        0        0     1085 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin
--rw-r--r--   0        0        0     1163 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin
--rw-r--r--   0        0        0     2205 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin
--rw-r--r--   0        0        0     2353 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin
--rw-r--r--   0        0        0     2205 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin
--rw-r--r--   0        0        0     2353 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin
--rw-r--r--   0        0        0     2205 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin
--rw-r--r--   0        0        0     2353 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.1.xml.bin
--rw-r--r--   0        0        0     8540 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin
--rw-r--r--   0        0        0     8315 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin
--rw-r--r--   0        0        0    10266 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin
--rw-r--r--   0        0        0     9628 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin
--rw-r--r--   0        0        0    13173 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin
--rw-r--r--   0        0        0    12575 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin
--rw-r--r--   0        0        0    13173 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin
--rw-r--r--   0        0        0    12575 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin
--rw-r--r--   0        0        0    14338 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin
--rw-r--r--   0        0        0    13889 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin
--rw-r--r--   0        0        0     2950 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin
--rw-r--r--   0        0        0     3403 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin
--rw-r--r--   0        0        0     2603 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin
--rw-r--r--   0        0        0     2993 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin
--rw-r--r--   0        0        0     2313 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin
--rw-r--r--   0        0        0     2521 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin
--rw-r--r--   0        0        0     2950 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin
--rw-r--r--   0        0        0     3403 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin
--rw-r--r--   0        0        0     2498 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin
--rw-r--r--   0        0        0     2716 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin
--rw-r--r--   0        0        0     2028 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin
--rw-r--r--   0        0        0     2102 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin
--rw-r--r--   0        0        0     2028 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin
--rw-r--r--   0        0        0     2102 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin
--rw-r--r--   0        0        0     2028 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin
--rw-r--r--   0        0        0     2102 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin
--rw-r--r--   0        0        0     1199 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin
--rw-r--r--   0        0        0     4993 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin
--rw-r--r--   0        0        0     7631 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin
--rw-r--r--   0        0        0     7396 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin
--rw-r--r--   0        0        0     8830 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin
--rw-r--r--   0        0        0     8293 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin
--rw-r--r--   0        0        0    11737 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin
--rw-r--r--   0        0        0    11240 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin
--rw-r--r--   0        0        0    11737 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin
--rw-r--r--   0        0        0    11240 2024-04-09 15:24:22.030841 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin
--rw-r--r--   0        0        0    11906 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin
--rw-r--r--   0        0        0    11441 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin
--rw-r--r--   0        0        0      307 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.0.xml.bin
--rw-r--r--   0        0        0      477 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.1.xml.bin
--rw-r--r--   0        0        0      860 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin
--rw-r--r--   0        0        0      859 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin
--rw-r--r--   0        0        0      860 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin
--rw-r--r--   0        0        0      859 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin
--rw-r--r--   0        0        0     1980 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin
--rw-r--r--   0        0        0     2049 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin
--rw-r--r--   0        0        0     1980 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin
--rw-r--r--   0        0        0     2049 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin
--rw-r--r--   0        0        0     1980 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin
--rw-r--r--   0        0        0     2049 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin
--rw-r--r--   0        0        0      395 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.0.xml.bin
--rw-r--r--   0        0        0      572 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin
--rw-r--r--   0        0        0      952 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin
--rw-r--r--   0        0        0      961 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin
--rw-r--r--   0        0        0      952 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin
--rw-r--r--   0        0        0      961 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin
--rw-r--r--   0        0        0     2093 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin
--rw-r--r--   0        0        0     2168 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin
--rw-r--r--   0        0        0     2093 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin
--rw-r--r--   0        0        0     2168 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin
--rw-r--r--   0        0        0     2093 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin
--rw-r--r--   0        0        0     2168 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin
--rw-r--r--   0        0        0     3848 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin
--rw-r--r--   0        0        0     3888 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin
--rw-r--r--   0        0        0     3848 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin
--rw-r--r--   0        0        0     3888 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin
--rw-r--r--   0        0        0     3848 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin
--rw-r--r--   0        0        0     3888 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin
--rw-r--r--   0        0        0     2028 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin
--rw-r--r--   0        0        0     2102 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin
--rw-r--r--   0        0        0     2028 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin
--rw-r--r--   0        0        0     2102 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin
--rw-r--r--   0        0        0     3782 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin
--rw-r--r--   0        0        0     3937 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin
--rw-r--r--   0        0        0     5189 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin
--rw-r--r--   0        0        0     5704 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin
--rw-r--r--   0        0        0     5189 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin
--rw-r--r--   0        0        0     5704 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin
--rw-r--r--   0        0        0     5382 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin
--rw-r--r--   0        0        0     5929 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin
--rw-r--r--   0        0        0      448 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin
--rw-r--r--   0        0        0     1056 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin
--rw-r--r--   0        0        0     1071 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin
--rw-r--r--   0        0        0     1243 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin
--rw-r--r--   0        0        0     1214 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin
--rw-r--r--   0        0        0     2384 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin
--rw-r--r--   0        0        0     2421 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin
--rw-r--r--   0        0        0     2384 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin
--rw-r--r--   0        0        0     2421 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin
--rw-r--r--   0        0        0     2384 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin
--rw-r--r--   0        0        0     2421 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin
--rw-r--r--   0        0        0     2950 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin
--rw-r--r--   0        0        0     3403 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin
--rw-r--r--   0        0        0      655 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin
--rw-r--r--   0        0        0      980 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin
--rw-r--r--   0        0        0     1582 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin
--rw-r--r--   0        0        0     1579 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin
--rw-r--r--   0        0        0     1769 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin
--rw-r--r--   0        0        0     1722 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin
--rw-r--r--   0        0        0     2889 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin
--rw-r--r--   0        0        0     2912 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin
--rw-r--r--   0        0        0     2889 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin
--rw-r--r--   0        0        0     2912 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin
--rw-r--r--   0        0        0     2889 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin
--rw-r--r--   0        0        0     2912 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin
--rw-r--r--   0        0        0      654 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin
--rw-r--r--   0        0        0     1045 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin
--rw-r--r--   0        0        0     1562 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin
--rw-r--r--   0        0        0     1749 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin
--rw-r--r--   0        0        0     2890 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin
--rw-r--r--   0        0        0     2890 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin
--rw-r--r--   0        0        0     2927 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin
--rw-r--r--   0        0        0     2890 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin
--rw-r--r--   0        0        0     2927 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.0.xml.bin
--rw-r--r--   0        0        0      431 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.1.xml.bin
--rw-r--r--   0        0        0      629 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin
--rw-r--r--   0        0        0      666 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin
--rw-r--r--   0        0        0      792 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin
--rw-r--r--   0        0        0      797 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin
--rw-r--r--   0        0        0     1933 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin
--rw-r--r--   0        0        0     2004 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin
--rw-r--r--   0        0        0     1933 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin
--rw-r--r--   0        0        0     2004 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin
--rw-r--r--   0        0        0     1933 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin
--rw-r--r--   0        0        0     2004 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin
--rw-r--r--   0        0        0      516 2024-04-09 15:24:22.034842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin
--rw-r--r--   0        0        0      814 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     2131 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin
--rw-r--r--   0        0        0     2058 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     2231 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin
--rw-r--r--   0        0        0     2149 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     3288 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin
--rw-r--r--   0        0        0     3288 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     3288 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin
--rw-r--r--   0        0        0     3288 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin
--rw-r--r--   0        0        0     3371 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin
--rw-r--r--   0        0        0     3343 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin
--rw-r--r--   0        0        0      448 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin
--rw-r--r--   0        0        0     1575 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin
--rw-r--r--   0        0        0     1762 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin
--rw-r--r--   0        0        0     2903 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin
--rw-r--r--   0        0        0     2903 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin
--rw-r--r--   0        0        0     2927 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin
--rw-r--r--   0        0        0     2903 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin
--rw-r--r--   0        0        0     2927 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin
--rw-r--r--   0        0        0      245 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.0.xml.bin
--rw-r--r--   0        0        0      459 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     1475 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin
--rw-r--r--   0        0        0     1382 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     1649 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin
--rw-r--r--   0        0        0     1533 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     2748 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin
--rw-r--r--   0        0        0     2706 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     2748 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin
--rw-r--r--   0        0        0     2706 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin
--rw-r--r--   0        0        0     2748 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin
--rw-r--r--   0        0        0     2706 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.1.xml.bin
--rw-r--r--   0        0        0     3900 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin
--rw-r--r--   0        0        0     4021 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin
--rw-r--r--   0        0        0     4263 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin
--rw-r--r--   0        0        0     4295 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin
--rw-r--r--   0        0        0     7224 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin
--rw-r--r--   0        0        0     7288 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin
--rw-r--r--   0        0        0     7224 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin
--rw-r--r--   0        0        0     7288 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin
--rw-r--r--   0        0        0     7779 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin
--rw-r--r--   0        0        0     7939 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.1.xml.bin
--rw-r--r--   0        0        0     2106 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin
--rw-r--r--   0        0        0     2196 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin
--rw-r--r--   0        0        0     2469 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin
--rw-r--r--   0        0        0     2470 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin
--rw-r--r--   0        0        0     5430 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin
--rw-r--r--   0        0        0     5463 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin
--rw-r--r--   0        0        0     5430 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin
--rw-r--r--   0        0        0     5463 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin
--rw-r--r--   0        0        0     5599 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin
--rw-r--r--   0        0        0     5664 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.1.xml.bin
--rw-r--r--   0        0        0     1030 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin
--rw-r--r--   0        0        0     1040 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin
--rw-r--r--   0        0        0     1030 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin
--rw-r--r--   0        0        0     1040 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin
--rw-r--r--   0        0        0     2171 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin
--rw-r--r--   0        0        0     2247 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin
--rw-r--r--   0        0        0     2171 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin
--rw-r--r--   0        0        0     2247 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin
--rw-r--r--   0        0        0     2171 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin
--rw-r--r--   0        0        0     2247 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin
--rw-r--r--   0        0        0     2957 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_component.py
--rw-r--r--   0        0        0     3283 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_deserialize_json.py
--rw-r--r--   0        0        0     1764 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_deserialize_xml.py
--rw-r--r--   0        0        0    19038 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_enums.py
--rw-r--r--   0        0        0     4389 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_factory_license.py
--rw-r--r--   0        0        0    22602 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model.py
--rw-r--r--   0        0        0    13254 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model_bom.py
--rw-r--r--   0        0        0     2782 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model_bom_ref.py
--rw-r--r--   0        0        0    18544 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model_component.py
--rw-r--r--   0        0        0     1793 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model_dependency.py
--rw-r--r--   0        0        0     4064 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model_issue.py
--rw-r--r--   0        0        0     4295 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model_license.py
--rw-r--r--   0        0        0     2758 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model_release_note.py
--rw-r--r--   0        0        0     3390 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model_service.py
--rw-r--r--   0        0        0    14370 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_model_vulnerability.py
--rw-r--r--   0        0        0     3154 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_output.py
--rw-r--r--   0        0        0     4587 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_output_json.py
--rw-r--r--   0        0        0     4029 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_output_xml.py
--rw-r--r--   0        0        0     1307 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_real_world_examples.py
--rw-r--r--   0        0        0     2509 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_schema_SchemaVersion.py
--rw-r--r--   0        0        0     1248 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_schema__res.py
--rw-r--r--   0        0        0     2873 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_spdx.py
--rw-r--r--   0        0        0     1977 2024-04-09 15:24:22.038842 cyclonedx_python_lib-7.0.0/tests/test_validation.py
--rw-r--r--   0        0        0     4529 2024-04-09 15:24:22.042842 cyclonedx_python_lib-7.0.0/tests/test_validation_json.py
--rw-r--r--   0        0        0     3061 2024-04-09 15:24:22.042842 cyclonedx_python_lib-7.0.0/tests/test_validation_xml.py
--rw-r--r--   0        0        0     6661 1970-01-01 00:00:00.000000 cyclonedx_python_lib-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0   220539 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/LICENSE
+-rw-r--r--   0        0        0      147 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/NOTICE
+-rw-r--r--   0        0        0     4569 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/README.md
+-rw-r--r--   0        0        0      858 2024-04-09 15:17:58.421851 cyclonedx_python_lib-7.0.0a1/cyclonedx/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/__init__.py
+-rw-r--r--   0        0        0     1734 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/compare.py
+-rw-r--r--   0        0        0     1164 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/hash.py
+-rw-r--r--   0        0        0      847 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/time.py
+-rw-r--r--   0        0        0      993 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/__init__.py
+-rw-r--r--   0        0        0     1536 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/factory.py
+-rw-r--r--   0        0        0     3685 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/model.py
+-rw-r--r--   0        0        0     1136 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/output.py
+-rw-r--r--   0        0        0     1730 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/serialization.py
+-rw-r--r--   0        0        0      680 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/factory/__init__.py
+-rw-r--r--   0        0        0     3233 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/factory/license.py
+-rw-r--r--   0        0        0    43540 2024-04-09 15:17:34.773742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/__init__.py
+-rw-r--r--   0        0        0    25088 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/bom.py
+-rw-r--r--   0        0        0     2179 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/bom_ref.py
+-rw-r--r--   0        0        0    57519 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/component.py
+-rw-r--r--   0        0        0    11789 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/contact.py
+-rw-r--r--   0        0        0    48270 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/crypto.py
+-rw-r--r--   0        0        0     3766 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/dependency.py
+-rw-r--r--   0        0        0     3568 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/impact_analysis.py
+-rw-r--r--   0        0        0     7024 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/issue.py
+-rw-r--r--   0        0        0    10127 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/license.py
+-rw-r--r--   0        0        0     8623 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/release_note.py
+-rw-r--r--   0        0        0    12798 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/service.py
+-rw-r--r--   0        0        0    43655 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/model/vulnerability.py
+-rw-r--r--   0        0        0     5872 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/output/__init__.py
+-rw-r--r--   0        0        0     4270 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/output/json.py
+-rw-r--r--   0        0        0     4285 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/output/xml.py
+-rw-r--r--   0        0        0      153 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/py.typed
+-rw-r--r--   0        0        0     3018 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/__init__.py
+-rw-r--r--   0        0        0     2127 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/README.md
+-rw-r--r--   0        0        0     2493 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/__init__.py
+-rw-r--r--   0        0        0    13604 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    39716 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    37194 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    36226 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    76383 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    40408 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    39348 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    88794 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    72383 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   133792 2024-04-09 15:17:34.777742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd
+-rw-r--r--   0        0        0   164772 2024-04-09 15:17:34.781742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   311805 2024-04-09 15:17:34.781742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd
+-rw-r--r--   0        0        0   252643 2024-04-09 15:17:34.781742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   492947 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd
+-rw-r--r--   0        0        0     8058 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    14269 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   165694 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd
+-rw-r--r--   0        0        0     2573 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/schema.py
+-rw-r--r--   0        0        0     6576 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/serialization/__init__.py
+-rw-r--r--   0        0        0     2503 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/spdx.py
+-rw-r--r--   0        0        0     3701 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/__init__.py
+-rw-r--r--   0        0        0     4817 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/json.py
+-rw-r--r--   0        0        0      853 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/model.py
+-rw-r--r--   0        0        0     3672 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/xml.py
+-rw-r--r--   0        0        0      634 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/Makefile
+-rw-r--r--   0        0        0     1524 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/architecture.rst
+-rw-r--r--   0        0        0      686 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/changelog.rst
+-rw-r--r--   0        0        0     2665 2024-04-09 15:17:58.421851 cyclonedx_python_lib-7.0.0a1/docs/conf.py
+-rw-r--r--   0        0        0       34 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/contributing.rst
+-rw-r--r--   0        0        0      895 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/examples.rst
+-rw-r--r--   0        0        0     1857 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/index.rst
+-rw-r--r--   0        0        0     1499 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/install.rst
+-rw-r--r--   0        0        0      800 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/make.bat
+-rw-r--r--   0        0        0     3275 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/modelling.rst
+-rw-r--r--   0        0        0     2269 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/outputting.rst
+-rw-r--r--   0        0        0       81 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/requirements.txt
+-rw-r--r--   0        0        0     4961 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/schema-support.rst
+-rw-r--r--   0        0        0     1329 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/docs/support.rst
+-rw-r--r--   0        0        0      176 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/examples/README.md
+-rw-r--r--   0        0        0     8164 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/examples/complex_deserialize.py
+-rw-r--r--   0        0        0     4081 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/examples/complex_serialize.py
+-rw-r--r--   0        0        0     4235 2024-04-09 15:17:58.421851 cyclonedx_python_lib-7.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     6717 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/__init__.py
+-rw-r--r--   0        0        0      704 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/__init__.py
+-rw-r--r--   0        0        0    42334 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/models.py
+-rw-r--r--   0        0        0       16 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/own/README.md
+-rw-r--r--   0        0        0     1309 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/own/json/1.2/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     1309 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/own/json/1.3/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     1309 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/own/json/1.4/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     2461 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/own/xml/1.4/bom_setuptools.xml
+-rw-r--r--   0        0        0    98508 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/own/xml/1.4/webgoat-6.1.xml
+-rw-r--r--   0        0        0     3723 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml
+-rw-r--r--   0        0        0     1195 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml
+-rw-r--r--   0        0        0      559 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml
+-rw-r--r--   0        0        0      313 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-component-type-1.1.xml
+-rw-r--r--   0        0        0      246 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-empty-component-1.1.xml
+-rw-r--r--   0        0        0      830 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml
+-rw-r--r--   0        0        0      801 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml
+-rw-r--r--   0        0        0      793 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml
+-rw-r--r--   0        0        0      769 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml
+-rw-r--r--   0        0        0      705 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml
+-rw-r--r--   0        0        0     1303 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml
+-rw-r--r--   0        0        0    16515 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml
+-rw-r--r--   0        0        0    16513 2024-04-09 15:17:34.785742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml
+-rw-r--r--   0        0        0     1328 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml
+-rw-r--r--   0        0        0     1366 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml
+-rw-r--r--   0        0        0      302 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-missing-component-type-1.1.xml
+-rw-r--r--   0        0        0    21038 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml
+-rw-r--r--   0        0        0      348 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-scope-1.1.xml
+-rw-r--r--   0        0        0    21026 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml
+-rw-r--r--   0        0        0    21039 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml
+-rw-r--r--   0        0        0     1217 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml
+-rw-r--r--   0        0        0      704 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml
+-rw-r--r--   0        0        0      965 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml
+-rw-r--r--   0        0        0      186 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-empty-components-1.1.xml
+-rw-r--r--   0        0        0    22339 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml
+-rw-r--r--   0        0        0     1210 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml
+-rw-r--r--   0        0        0     1214 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml
+-rw-r--r--   0        0        0     1226 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml
+-rw-r--r--   0        0        0      317 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-minimal-viable-1.1.xml
+-rw-r--r--   0        0        0    21121 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml
+-rw-r--r--   0        0        0    10048 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml
+-rw-r--r--   0        0        0      165 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-bomformat-1.2.json
+-rw-r--r--   0        0        0      394 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.json
+-rw-r--r--   0        0        0      560 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml
+-rw-r--r--   0        0        0      385 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.json
+-rw-r--r--   0        0        0      433 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.xml
+-rw-r--r--   0        0        0      249 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.json
+-rw-r--r--   0        0        0      314 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.xml
+-rw-r--r--   0        0        0      667 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json
+-rw-r--r--   0        0        0      809 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml
+-rw-r--r--   0        0        0      247 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-empty-component-1.2.xml
+-rw-r--r--   0        0        0      856 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json
+-rw-r--r--   0        0        0      831 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml
+-rw-r--r--   0        0        0      827 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json
+-rw-r--r--   0        0        0      802 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml
+-rw-r--r--   0        0        0      819 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json
+-rw-r--r--   0        0        0      794 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml
+-rw-r--r--   0        0        0      795 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json
+-rw-r--r--   0        0        0      770 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml
+-rw-r--r--   0        0        0      731 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json
+-rw-r--r--   0        0        0      706 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml
+-rw-r--r--   0        0        0     1184 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json
+-rw-r--r--   0        0        0     1554 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml
+-rw-r--r--   0        0        0      515 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json
+-rw-r--r--   0        0        0     1304 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml
+-rw-r--r--   0        0        0    15788 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json
+-rw-r--r--   0        0        0    16516 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml
+-rw-r--r--   0        0        0      428 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.json
+-rw-r--r--   0        0        0    16514 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml
+-rw-r--r--   0        0        0     1329 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml
+-rw-r--r--   0        0        0     1367 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml
+-rw-r--r--   0        0        0      209 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.json
+-rw-r--r--   0        0        0      244 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.xml
+-rw-r--r--   0        0        0      303 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-missing-component-type-1.2.xml
+-rw-r--r--   0        0        0    21039 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml
+-rw-r--r--   0        0        0     1185 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json
+-rw-r--r--   0        0        0     1555 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml
+-rw-r--r--   0        0        0      275 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-scope-1.2.json
+-rw-r--r--   0        0        0      349 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-scope-1.2.xml
+-rw-r--r--   0        0        0      148 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.json
+-rw-r--r--   0        0        0    21027 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.json
+-rw-r--r--   0        0        0      416 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.xml
+-rw-r--r--   0        0        0      363 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/skip_invalid-empty-component-1.2.json
+-rw-r--r--   0        0        0      361 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/skip_invalid-missing-component-type-1.2.json
+-rw-r--r--   0        0        0      548 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json
+-rw-r--r--   0        0        0      792 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml
+-rw-r--r--   0        0        0    20390 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-bom-1.2.json
+-rw-r--r--   0        0        0    24278 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml
+-rw-r--r--   0        0        0     2163 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json
+-rw-r--r--   0        0        0     1897 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml
+-rw-r--r--   0        0        0      394 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.json
+-rw-r--r--   0        0        0      705 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml
+-rw-r--r--   0        0        0      456 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.json
+-rw-r--r--   0        0        0      492 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.xml
+-rw-r--r--   0        0        0     1342 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json
+-rw-r--r--   0        0        0     1346 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml
+-rw-r--r--   0        0        0      892 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json
+-rw-r--r--   0        0        0     1223 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml
+-rw-r--r--   0        0        0      693 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json
+-rw-r--r--   0        0        0      824 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml
+-rw-r--r--   0        0        0      161 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.json
+-rw-r--r--   0        0        0      187 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.xml
+-rw-r--r--   0        0        0    22340 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml
+-rw-r--r--   0        0        0      438 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.json
+-rw-r--r--   0        0        0     1211 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-id-1.2.json
+-rw-r--r--   0        0        0     1215 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml
+-rw-r--r--   0        0        0      440 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-name-1.2.json
+-rw-r--r--   0        0        0     1227 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml
+-rw-r--r--   0        0        0      333 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.json
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.xml
+-rw-r--r--   0        0        0      438 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.json
+-rw-r--r--   0        0        0      492 2024-04-09 15:17:34.789742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.xml
+-rw-r--r--   0        0        0      417 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.json
+-rw-r--r--   0        0        0      468 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.xml
+-rw-r--r--   0        0        0      224 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.json
+-rw-r--r--   0        0        0      254 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.xml
+-rw-r--r--   0        0        0      605 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json
+-rw-r--r--   0        0        0      654 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml
+-rw-r--r--   0        0        0      253 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.json
+-rw-r--r--   0        0        0      318 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.xml
+-rw-r--r--   0        0        0     2465 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-patch-1.2.json
+-rw-r--r--   0        0        0     3337 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml
+-rw-r--r--   0        0        0    21122 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml
+-rw-r--r--   0        0        0     2308 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-service-1.2.json
+-rw-r--r--   0        0        0     2693 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-service-1.2.xml
+-rw-r--r--   0        0        0      419 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.json
+-rw-r--r--   0        0        0      495 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.xml
+-rw-r--r--   0        0        0    11181 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml
+-rw-r--r--   0        0        0      165 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-bomformat-1.3.json
+-rw-r--r--   0        0        0      394 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.json
+-rw-r--r--   0        0        0      560 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml
+-rw-r--r--   0        0        0      385 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.json
+-rw-r--r--   0        0        0      433 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.xml
+-rw-r--r--   0        0        0      249 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.json
+-rw-r--r--   0        0        0      314 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.xml
+-rw-r--r--   0        0        0      667 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json
+-rw-r--r--   0        0        0      809 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml
+-rw-r--r--   0        0        0      197 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.json
+-rw-r--r--   0        0        0      247 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.xml
+-rw-r--r--   0        0        0      856 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json
+-rw-r--r--   0        0        0      831 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml
+-rw-r--r--   0        0        0      827 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json
+-rw-r--r--   0        0        0      802 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml
+-rw-r--r--   0        0        0      819 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json
+-rw-r--r--   0        0        0      794 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml
+-rw-r--r--   0        0        0      795 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json
+-rw-r--r--   0        0        0      770 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml
+-rw-r--r--   0        0        0      731 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json
+-rw-r--r--   0        0        0      706 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml
+-rw-r--r--   0        0        0     1184 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json
+-rw-r--r--   0        0        0     1554 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml
+-rw-r--r--   0        0        0      515 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json
+-rw-r--r--   0        0        0     1304 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml
+-rw-r--r--   0        0        0    15788 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json
+-rw-r--r--   0        0        0    16516 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml
+-rw-r--r--   0        0        0      428 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.json
+-rw-r--r--   0        0        0    16514 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml
+-rw-r--r--   0        0        0     1329 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml
+-rw-r--r--   0        0        0     1367 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml
+-rw-r--r--   0        0        0      277 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.json
+-rw-r--r--   0        0        0      319 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.xml
+-rw-r--r--   0        0        0      209 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.json
+-rw-r--r--   0        0        0      244 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.xml
+-rw-r--r--   0        0        0      228 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.json
+-rw-r--r--   0        0        0      303 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.xml
+-rw-r--r--   0        0        0    21039 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml
+-rw-r--r--   0        0        0     1185 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json
+-rw-r--r--   0        0        0     1555 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml
+-rw-r--r--   0        0        0      275 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-scope-1.3.json
+-rw-r--r--   0        0        0      349 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-scope-1.3.xml
+-rw-r--r--   0        0        0      148 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.json
+-rw-r--r--   0        0        0    21027 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.json
+-rw-r--r--   0        0        0      416 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.xml
+-rw-r--r--   0        0        0      548 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json
+-rw-r--r--   0        0        0      792 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml
+-rw-r--r--   0        0        0    20390 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-bom-1.3.json
+-rw-r--r--   0        0        0    24278 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml
+-rw-r--r--   0        0        0     2163 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json
+-rw-r--r--   0        0        0     1897 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml
+-rw-r--r--   0        0        0      394 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.json
+-rw-r--r--   0        0        0      705 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml
+-rw-r--r--   0        0        0      456 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.json
+-rw-r--r--   0        0        0      492 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.xml
+-rw-r--r--   0        0        0     1342 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json
+-rw-r--r--   0        0        0     1346 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml
+-rw-r--r--   0        0        0      892 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json
+-rw-r--r--   0        0        0     1223 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml
+-rw-r--r--   0        0        0     1497 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json
+-rw-r--r--   0        0        0     1983 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml
+-rw-r--r--   0        0        0      693 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json
+-rw-r--r--   0        0        0      824 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml
+-rw-r--r--   0        0        0      161 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.json
+-rw-r--r--   0        0        0      187 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.xml
+-rw-r--r--   0        0        0     1384 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json
+-rw-r--r--   0        0        0     1596 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml
+-rw-r--r--   0        0        0    22340 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml
+-rw-r--r--   0        0        0     1117 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json
+-rw-r--r--   0        0        0     1324 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml
+-rw-r--r--   0        0        0      438 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.json
+-rw-r--r--   0        0        0     1211 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-id-1.3.json
+-rw-r--r--   0        0        0     1215 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml
+-rw-r--r--   0        0        0      440 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-name-1.3.json
+-rw-r--r--   0        0        0     1227 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml
+-rw-r--r--   0        0        0      333 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.json
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.xml
+-rw-r--r--   0        0        0      279 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.json
+-rw-r--r--   0        0        0      321 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.xml
+-rw-r--r--   0        0        0      438 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.json
+-rw-r--r--   0        0        0      492 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.xml
+-rw-r--r--   0        0        0      417 2024-04-09 15:17:34.793742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.json
+-rw-r--r--   0        0        0      468 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.xml
+-rw-r--r--   0        0        0      224 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.json
+-rw-r--r--   0        0        0      254 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.xml
+-rw-r--r--   0        0        0      605 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json
+-rw-r--r--   0        0        0      654 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml
+-rw-r--r--   0        0        0      253 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.json
+-rw-r--r--   0        0        0      318 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.xml
+-rw-r--r--   0        0        0     2465 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-patch-1.3.json
+-rw-r--r--   0        0        0     3337 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml
+-rw-r--r--   0        0        0      983 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-properties-1.3.json
+-rw-r--r--   0        0        0     1213 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml
+-rw-r--r--   0        0        0    21122 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml
+-rw-r--r--   0        0        0     2308 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-service-1.3.json
+-rw-r--r--   0        0        0     2693 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-service-1.3.xml
+-rw-r--r--   0        0        0      419 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.json
+-rw-r--r--   0        0        0      495 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.xml
+-rw-r--r--   0        0        0    11181 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml
+-rw-r--r--   0        0        0      165 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-bomformat-1.4.json
+-rw-r--r--   0        0        0      394 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.json
+-rw-r--r--   0        0        0      560 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml
+-rw-r--r--   0        0        0      385 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.json
+-rw-r--r--   0        0        0      433 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.xml
+-rw-r--r--   0        0        0      249 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.json
+-rw-r--r--   0        0        0      314 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.xml
+-rw-r--r--   0        0        0      667 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json
+-rw-r--r--   0        0        0      809 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml
+-rw-r--r--   0        0        0      197 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.json
+-rw-r--r--   0        0        0      247 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.xml
+-rw-r--r--   0        0        0      856 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json
+-rw-r--r--   0        0        0      831 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml
+-rw-r--r--   0        0        0      827 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json
+-rw-r--r--   0        0        0      802 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml
+-rw-r--r--   0        0        0      819 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json
+-rw-r--r--   0        0        0      794 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml
+-rw-r--r--   0        0        0      795 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json
+-rw-r--r--   0        0        0      770 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml
+-rw-r--r--   0        0        0      731 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json
+-rw-r--r--   0        0        0      706 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml
+-rw-r--r--   0        0        0     1184 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json
+-rw-r--r--   0        0        0     1554 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml
+-rw-r--r--   0        0        0      515 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json
+-rw-r--r--   0        0        0     1304 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml
+-rw-r--r--   0        0        0    15788 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json
+-rw-r--r--   0        0        0    16516 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml
+-rw-r--r--   0        0        0      428 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.json
+-rw-r--r--   0        0        0    16514 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml
+-rw-r--r--   0        0        0     1329 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml
+-rw-r--r--   0        0        0     1367 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml
+-rw-r--r--   0        0        0      277 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.json
+-rw-r--r--   0        0        0      319 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.xml
+-rw-r--r--   0        0        0      209 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.json
+-rw-r--r--   0        0        0      244 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.xml
+-rw-r--r--   0        0        0      228 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.json
+-rw-r--r--   0        0        0      303 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.xml
+-rw-r--r--   0        0        0    21039 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml
+-rw-r--r--   0        0        0     1185 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json
+-rw-r--r--   0        0        0     1555 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml
+-rw-r--r--   0        0        0      275 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-scope-1.4.json
+-rw-r--r--   0        0        0      349 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-scope-1.4.xml
+-rw-r--r--   0        0        0      148 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.json
+-rw-r--r--   0        0        0    21027 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.json
+-rw-r--r--   0        0        0      416 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.xml
+-rw-r--r--   0        0        0      548 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json
+-rw-r--r--   0        0        0      792 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml
+-rw-r--r--   0        0        0    20390 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-bom-1.4.json
+-rw-r--r--   0        0        0    24278 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml
+-rw-r--r--   0        0        0     2163 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json
+-rw-r--r--   0        0        0     1897 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml
+-rw-r--r--   0        0        0      394 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.json
+-rw-r--r--   0        0        0      705 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml
+-rw-r--r--   0        0        0      456 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.json
+-rw-r--r--   0        0        0      492 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.xml
+-rw-r--r--   0        0        0     1342 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json
+-rw-r--r--   0        0        0     1346 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml
+-rw-r--r--   0        0        0      892 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json
+-rw-r--r--   0        0        0     1223 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml
+-rw-r--r--   0        0        0     1497 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json
+-rw-r--r--   0        0        0     1983 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml
+-rw-r--r--   0        0        0      693 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json
+-rw-r--r--   0        0        0      824 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml
+-rw-r--r--   0        0        0      161 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.json
+-rw-r--r--   0        0        0      187 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.xml
+-rw-r--r--   0        0        0     1384 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json
+-rw-r--r--   0        0        0     1596 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml
+-rw-r--r--   0        0        0    22340 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml
+-rw-r--r--   0        0        0     1117 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json
+-rw-r--r--   0        0        0     1324 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml
+-rw-r--r--   0        0        0      438 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.json
+-rw-r--r--   0        0        0     1211 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-id-1.4.json
+-rw-r--r--   0        0        0     1215 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml
+-rw-r--r--   0        0        0      440 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-name-1.4.json
+-rw-r--r--   0        0        0     1227 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml
+-rw-r--r--   0        0        0      333 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.json
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.xml
+-rw-r--r--   0        0        0      279 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.json
+-rw-r--r--   0        0        0      321 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.xml
+-rw-r--r--   0        0        0      438 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.json
+-rw-r--r--   0        0        0      492 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.xml
+-rw-r--r--   0        0        0      417 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.json
+-rw-r--r--   0        0        0      468 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.xml
+-rw-r--r--   0        0        0      224 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.json
+-rw-r--r--   0        0        0      254 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.xml
+-rw-r--r--   0        0        0      605 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json
+-rw-r--r--   0        0        0      654 2024-04-09 15:17:34.797742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml
+-rw-r--r--   0        0        0      227 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.json
+-rw-r--r--   0        0        0      281 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.xml
+-rw-r--r--   0        0        0     2465 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-patch-1.4.json
+-rw-r--r--   0        0        0     3337 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml
+-rw-r--r--   0        0        0      983 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-properties-1.4.json
+-rw-r--r--   0        0        0     1213 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml
+-rw-r--r--   0        0        0    21122 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml
+-rw-r--r--   0        0        0     5338 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json
+-rw-r--r--   0        0        0     6828 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml
+-rw-r--r--   0        0        0     2312 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-service-1.4.json
+-rw-r--r--   0        0        0     2693 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-service-1.4.xml
+-rw-r--r--   0        0        0      419 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.json
+-rw-r--r--   0        0        0      495 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.xml
+-rw-r--r--   0        0        0     9733 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json
+-rw-r--r--   0        0        0     4274 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json
+-rw-r--r--   0        0        0     5987 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml
+-rw-r--r--   0        0        0    11181 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml
+-rw-r--r--   0        0        0      165 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-bomformat-1.5.json
+-rw-r--r--   0        0        0      508 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.json
+-rw-r--r--   0        0        0      866 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml
+-rw-r--r--   0        0        0      385 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.json
+-rw-r--r--   0        0        0      433 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.xml
+-rw-r--r--   0        0        0      249 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.json
+-rw-r--r--   0        0        0      314 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.xml
+-rw-r--r--   0        0        0      746 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json
+-rw-r--r--   0        0        0     1086 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml
+-rw-r--r--   0        0        0      197 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.json
+-rw-r--r--   0        0        0      247 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.xml
+-rw-r--r--   0        0        0      856 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json
+-rw-r--r--   0        0        0      831 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml
+-rw-r--r--   0        0        0      827 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json
+-rw-r--r--   0        0        0      802 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml
+-rw-r--r--   0        0        0      819 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json
+-rw-r--r--   0        0        0      794 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml
+-rw-r--r--   0        0        0      795 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json
+-rw-r--r--   0        0        0      770 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml
+-rw-r--r--   0        0        0      731 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json
+-rw-r--r--   0        0        0      706 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml
+-rw-r--r--   0        0        0     1184 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json
+-rw-r--r--   0        0        0     1554 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml
+-rw-r--r--   0        0        0      515 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json
+-rw-r--r--   0        0        0     1304 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml
+-rw-r--r--   0        0        0    15788 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json
+-rw-r--r--   0        0        0    16516 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml
+-rw-r--r--   0        0        0      428 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.json
+-rw-r--r--   0        0        0    16514 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml
+-rw-r--r--   0        0        0     1329 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml
+-rw-r--r--   0        0        0     1367 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml
+-rw-r--r--   0        0        0      277 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.json
+-rw-r--r--   0        0        0      319 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.xml
+-rw-r--r--   0        0        0      209 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.json
+-rw-r--r--   0        0        0      244 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.xml
+-rw-r--r--   0        0        0      228 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.json
+-rw-r--r--   0        0        0      303 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.xml
+-rw-r--r--   0        0        0    21039 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml
+-rw-r--r--   0        0        0     1185 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json
+-rw-r--r--   0        0        0     1555 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml
+-rw-r--r--   0        0        0      275 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-scope-1.5.json
+-rw-r--r--   0        0        0      349 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-scope-1.5.xml
+-rw-r--r--   0        0        0      148 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.json
+-rw-r--r--   0        0        0    21027 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.json
+-rw-r--r--   0        0        0      416 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.xml
+-rw-r--r--   0        0        0     2527 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json
+-rw-r--r--   0        0        0     3596 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml
+-rw-r--r--   0        0        0      548 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json
+-rw-r--r--   0        0        0      792 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml
+-rw-r--r--   0        0        0    20390 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-bom-1.5.json
+-rw-r--r--   0        0        0    24278 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml
+-rw-r--r--   0        0        0     2163 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json
+-rw-r--r--   0        0        0     1897 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml
+-rw-r--r--   0        0        0      394 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.json
+-rw-r--r--   0        0        0      705 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml
+-rw-r--r--   0        0        0      456 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.json
+-rw-r--r--   0        0        0      492 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.xml
+-rw-r--r--   0        0        0     1342 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json
+-rw-r--r--   0        0        0     1346 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml
+-rw-r--r--   0        0        0      892 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json
+-rw-r--r--   0        0        0     1223 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml
+-rw-r--r--   0        0        0     1810 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json
+-rw-r--r--   0        0        0     2449 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml
+-rw-r--r--   0        0        0      693 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json
+-rw-r--r--   0        0        0      824 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml
+-rw-r--r--   0        0        0      161 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.json
+-rw-r--r--   0        0        0      187 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.xml
+-rw-r--r--   0        0        0     3189 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json
+-rw-r--r--   0        0        0     4519 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml
+-rw-r--r--   0        0        0    22340 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml
+-rw-r--r--   0        0        0     1117 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json
+-rw-r--r--   0        0        0     1324 2024-04-09 15:17:34.801742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml
+-rw-r--r--   0        0        0     7703 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json
+-rw-r--r--   0        0        0    11757 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml
+-rw-r--r--   0        0        0      473 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.json
+-rw-r--r--   0        0        0     1270 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml
+-rw-r--r--   0        0        0      467 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-id-1.5.json
+-rw-r--r--   0        0        0     1236 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml
+-rw-r--r--   0        0        0     1539 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json
+-rw-r--r--   0        0        0     2197 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml
+-rw-r--r--   0        0        0      477 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-name-1.5.json
+-rw-r--r--   0        0        0     1248 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml
+-rw-r--r--   0        0        0    98548 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json
+-rw-r--r--   0        0        0   100112 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml
+-rw-r--r--   0        0        0      333 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.json
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.xml
+-rw-r--r--   0        0        0      279 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.json
+-rw-r--r--   0        0        0      321 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.xml
+-rw-r--r--   0        0        0      436 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.json
+-rw-r--r--   0        0        0      624 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml
+-rw-r--r--   0        0        0      507 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.json
+-rw-r--r--   0        0        0      537 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml
+-rw-r--r--   0        0        0      482 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.json
+-rw-r--r--   0        0        0      509 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.xml
+-rw-r--r--   0        0        0      224 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.json
+-rw-r--r--   0        0        0      254 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.xml
+-rw-r--r--   0        0        0     1162 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json
+-rw-r--r--   0        0        0     1471 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml
+-rw-r--r--   0        0        0      605 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json
+-rw-r--r--   0        0        0      654 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml
+-rw-r--r--   0        0        0      227 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.json
+-rw-r--r--   0        0        0      281 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.xml
+-rw-r--r--   0        0        0     2465 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-patch-1.5.json
+-rw-r--r--   0        0        0     3337 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml
+-rw-r--r--   0        0        0     1520 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-properties-1.5.json
+-rw-r--r--   0        0        0     1660 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml
+-rw-r--r--   0        0        0    21122 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml
+-rw-r--r--   0        0        0     5338 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json
+-rw-r--r--   0        0        0     6828 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml
+-rw-r--r--   0        0        0     9412 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json
+-rw-r--r--   0        0        0    12249 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml
+-rw-r--r--   0        0        0     2312 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-service-1.5.json
+-rw-r--r--   0        0        0     2693 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-service-1.5.xml
+-rw-r--r--   0        0        0      419 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.json
+-rw-r--r--   0        0        0      495 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.xml
+-rw-r--r--   0        0        0     9733 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json
+-rw-r--r--   0        0        0    17746 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json
+-rw-r--r--   0        0        0    19794 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml
+-rw-r--r--   0        0        0    11181 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml
+-rw-r--r--   0        0        0      165 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-bomformat-1.6.json
+-rw-r--r--   0        0        0      508 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.json
+-rw-r--r--   0        0        0      866 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml
+-rw-r--r--   0        0        0      385 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.json
+-rw-r--r--   0        0        0      433 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.xml
+-rw-r--r--   0        0        0      249 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.json
+-rw-r--r--   0        0        0      314 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.xml
+-rw-r--r--   0        0        0      746 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json
+-rw-r--r--   0        0        0     1086 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml
+-rw-r--r--   0        0        0      197 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.json
+-rw-r--r--   0        0        0      247 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.xml
+-rw-r--r--   0        0        0      856 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json
+-rw-r--r--   0        0        0      831 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml
+-rw-r--r--   0        0        0      827 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json
+-rw-r--r--   0        0        0      802 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml
+-rw-r--r--   0        0        0      819 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json
+-rw-r--r--   0        0        0      794 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml
+-rw-r--r--   0        0        0      795 2024-04-09 15:17:34.805742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json
+-rw-r--r--   0        0        0      770 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml
+-rw-r--r--   0        0        0      731 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json
+-rw-r--r--   0        0        0      706 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml
+-rw-r--r--   0        0        0     1184 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json
+-rw-r--r--   0        0        0     1554 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml
+-rw-r--r--   0        0        0      515 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json
+-rw-r--r--   0        0        0     1304 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml
+-rw-r--r--   0        0        0    15788 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json
+-rw-r--r--   0        0        0    16516 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml
+-rw-r--r--   0        0        0      428 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.json
+-rw-r--r--   0        0        0    16514 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml
+-rw-r--r--   0        0        0     1329 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml
+-rw-r--r--   0        0        0      360 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.json
+-rw-r--r--   0        0        0      466 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.xml
+-rw-r--r--   0        0        0     1367 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml
+-rw-r--r--   0        0        0      277 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.json
+-rw-r--r--   0        0        0      319 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.xml
+-rw-r--r--   0        0        0      209 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.json
+-rw-r--r--   0        0        0      244 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.xml
+-rw-r--r--   0        0        0      228 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.json
+-rw-r--r--   0        0        0      303 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.xml
+-rw-r--r--   0        0        0    21039 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml
+-rw-r--r--   0        0        0     1185 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json
+-rw-r--r--   0        0        0     1555 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml
+-rw-r--r--   0        0        0     1290 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json
+-rw-r--r--   0        0        0     1504 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml
+-rw-r--r--   0        0        0      275 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-scope-1.6.json
+-rw-r--r--   0        0        0      349 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-scope-1.6.xml
+-rw-r--r--   0        0        0      148 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.json
+-rw-r--r--   0        0        0    21027 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.json
+-rw-r--r--   0        0        0      416 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.xml
+-rw-r--r--   0        0        0     2527 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json
+-rw-r--r--   0        0        0     3596 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml
+-rw-r--r--   0        0        0      548 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json
+-rw-r--r--   0        0        0      792 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml
+-rw-r--r--   0        0        0     5654 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json
+-rw-r--r--   0        0        0     7084 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml
+-rw-r--r--   0        0        0     6538 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-bom-1.6.json
+-rw-r--r--   0        0        0    24921 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml
+-rw-r--r--   0        0        0     2163 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json
+-rw-r--r--   0        0        0     1897 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml
+-rw-r--r--   0        0        0      750 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json
+-rw-r--r--   0        0        0      865 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml
+-rw-r--r--   0        0        0      394 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.json
+-rw-r--r--   0        0        0      705 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml
+-rw-r--r--   0        0        0      456 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.json
+-rw-r--r--   0        0        0      492 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.xml
+-rw-r--r--   0        0        0     1342 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json
+-rw-r--r--   0        0        0     1346 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml
+-rw-r--r--   0        0        0      892 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json
+-rw-r--r--   0        0        0     1223 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml
+-rw-r--r--   0        0        0     1810 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json
+-rw-r--r--   0        0        0     2449 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml
+-rw-r--r--   0        0        0     2978 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json
+-rw-r--r--   0        0        0     4629 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml
+-rw-r--r--   0        0        0     1459 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json
+-rw-r--r--   0        0        0     2217 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml
+-rw-r--r--   0        0        0      693 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json
+-rw-r--r--   0        0        0      824 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml
+-rw-r--r--   0        0        0      161 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.json
+-rw-r--r--   0        0        0      187 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.xml
+-rw-r--r--   0        0        0     4432 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json
+-rw-r--r--   0        0        0     6383 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml
+-rw-r--r--   0        0        0    22340 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml
+-rw-r--r--   0        0        0     1117 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json
+-rw-r--r--   0        0        0     1324 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml
+-rw-r--r--   0        0        0     7703 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json
+-rw-r--r--   0        0        0    11757 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml
+-rw-r--r--   0        0        0      514 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json
+-rw-r--r--   0        0        0     1297 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml
+-rw-r--r--   0        0        0      510 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-id-1.6.json
+-rw-r--r--   0        0        0     1263 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml
+-rw-r--r--   0        0        0     1539 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json
+-rw-r--r--   0        0        0     2197 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml
+-rw-r--r--   0        0        0      477 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-name-1.6.json
+-rw-r--r--   0        0        0     1248 2024-04-09 15:17:34.809742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml
+-rw-r--r--   0        0        0    98548 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json
+-rw-r--r--   0        0        0   100112 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml
+-rw-r--r--   0        0        0     1835 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json
+-rw-r--r--   0        0        0     2811 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml
+-rw-r--r--   0        0        0      333 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.json
+-rw-r--r--   0        0        0      430 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.xml
+-rw-r--r--   0        0        0      432 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.json
+-rw-r--r--   0        0        0      456 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.xml
+-rw-r--r--   0        0        0      436 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.json
+-rw-r--r--   0        0        0      624 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml
+-rw-r--r--   0        0        0      521 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json
+-rw-r--r--   0        0        0      551 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml
+-rw-r--r--   0        0        0      508 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.json
+-rw-r--r--   0        0        0      539 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml
+-rw-r--r--   0        0        0      482 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.json
+-rw-r--r--   0        0        0      509 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.xml
+-rw-r--r--   0        0        0      224 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.json
+-rw-r--r--   0        0        0      254 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.xml
+-rw-r--r--   0        0        0     1162 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json
+-rw-r--r--   0        0        0     1471 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml
+-rw-r--r--   0        0        0      605 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json
+-rw-r--r--   0        0        0      654 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml
+-rw-r--r--   0        0        0      227 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.json
+-rw-r--r--   0        0        0      281 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.xml
+-rw-r--r--   0        0        0     2465 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-patch-1.6.json
+-rw-r--r--   0        0        0     3337 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml
+-rw-r--r--   0        0        0     1894 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-properties-1.6.json
+-rw-r--r--   0        0        0     1872 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml
+-rw-r--r--   0        0        0    21122 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml
+-rw-r--r--   0        0        0     5338 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json
+-rw-r--r--   0        0        0     6828 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml
+-rw-r--r--   0        0        0     9412 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json
+-rw-r--r--   0        0        0    12249 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml
+-rw-r--r--   0        0        0     2312 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-service-1.6.json
+-rw-r--r--   0        0        0     2693 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-service-1.6.xml
+-rw-r--r--   0        0        0      419 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.json
+-rw-r--r--   0        0        0      495 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.xml
+-rw-r--r--   0        0        0     9733 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json
+-rw-r--r--   0        0        0     1902 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-standard-1.6.json
+-rw-r--r--   0        0        0     2747 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml
+-rw-r--r--   0        0        0      491 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-tags-1.6.json
+-rw-r--r--   0        0        0      870 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml
+-rw-r--r--   0        0        0    17746 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json
+-rw-r--r--   0        0        0    19794 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml
+-rw-r--r--   0        0        0    11181 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml
+-rw-r--r--   0        0        0      157 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/README.md
+-rwxr-xr-x   0        0        0      745 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/fetch.sh
+-rw-r--r--   0        0        0      391 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/README.md
+-rw-r--r--   0        0        0      579 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin
+-rw-r--r--   0        0        0      649 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin
+-rw-r--r--   0        0        0     1050 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin
+-rw-r--r--   0        0        0     1055 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin
+-rw-r--r--   0        0        0     1050 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin
+-rw-r--r--   0        0        0     1055 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin
+-rw-r--r--   0        0        0     2128 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin
+-rw-r--r--   0        0        0     2211 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin
+-rw-r--r--   0        0        0     2128 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin
+-rw-r--r--   0        0        0     2211 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin
+-rw-r--r--   0        0        0     2128 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin
+-rw-r--r--   0        0        0     2211 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin
+-rw-r--r--   0        0        0      806 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin
+-rw-r--r--   0        0        0      949 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin
+-rw-r--r--   0        0        0     1835 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.2.json.bin
+-rw-r--r--   0        0        0     1806 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin
+-rw-r--r--   0        0        0     1835 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.3.json.bin
+-rw-r--r--   0        0        0     1806 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin
+-rw-r--r--   0        0        0     2808 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.4.json.bin
+-rw-r--r--   0        0        0     2877 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin
+-rw-r--r--   0        0        0     3460 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.5.json.bin
+-rw-r--r--   0        0        0     3525 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin
+-rw-r--r--   0        0        0     3652 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.6.json.bin
+-rw-r--r--   0        0        0     3716 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.1.xml.bin
+-rw-r--r--   0        0        0      944 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.2.json.bin
+-rw-r--r--   0        0        0      865 2024-04-09 15:17:34.813742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin
+-rw-r--r--   0        0        0      944 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.3.json.bin
+-rw-r--r--   0        0        0      865 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin
+-rw-r--r--   0        0        0     2085 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.4.json.bin
+-rw-r--r--   0        0        0     2072 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin
+-rw-r--r--   0        0        0     2085 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.5.json.bin
+-rw-r--r--   0        0        0     2072 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin
+-rw-r--r--   0        0        0     2085 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.6.json.bin
+-rw-r--r--   0        0        0     2072 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.0.xml.bin
+-rw-r--r--   0        0        0      496 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.1.xml.bin
+-rw-r--r--   0        0        0      893 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.2.json.bin
+-rw-r--r--   0        0        0      812 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.2.xml.bin
+-rw-r--r--   0        0        0      893 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.3.json.bin
+-rw-r--r--   0        0        0      812 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.3.xml.bin
+-rw-r--r--   0        0        0     2013 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.4.json.bin
+-rw-r--r--   0        0        0     2002 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.4.xml.bin
+-rw-r--r--   0        0        0     2013 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.5.json.bin
+-rw-r--r--   0        0        0     2002 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.5.xml.bin
+-rw-r--r--   0        0        0     2013 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.6.json.bin
+-rw-r--r--   0        0        0     2002 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.0.xml.bin
+-rw-r--r--   0        0        0     4485 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin
+-rw-r--r--   0        0        0     4434 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin
+-rw-r--r--   0        0        0     4801 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin
+-rw-r--r--   0        0        0     4434 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin
+-rw-r--r--   0        0        0     4801 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin
+-rw-r--r--   0        0        0     5562 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin
+-rw-r--r--   0        0        0     5999 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin
+-rw-r--r--   0        0        0     5811 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin
+-rw-r--r--   0        0        0     6248 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin
+-rw-r--r--   0        0        0     5855 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin
+-rw-r--r--   0        0        0     6292 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin
+-rw-r--r--   0        0        0      749 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin
+-rw-r--r--   0        0        0      793 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin
+-rw-r--r--   0        0        0     1894 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin
+-rw-r--r--   0        0        0     1461 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin
+-rw-r--r--   0        0        0     1894 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin
+-rw-r--r--   0        0        0     1461 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin
+-rw-r--r--   0        0        0     3014 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin
+-rw-r--r--   0        0        0     2651 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin
+-rw-r--r--   0        0        0     3014 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin
+-rw-r--r--   0        0        0     2651 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin
+-rw-r--r--   0        0        0     3014 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin
+-rw-r--r--   0        0        0     2651 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.xml.bin
+-rw-r--r--   0        0        0     2092 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin
+-rw-r--r--   0        0        0     2289 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin
+-rw-r--r--   0        0        0     2092 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin
+-rw-r--r--   0        0        0     2289 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin
+-rw-r--r--   0        0        0     2092 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin
+-rw-r--r--   0        0        0     2289 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.xml.bin
+-rw-r--r--   0        0        0     3282 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin
+-rw-r--r--   0        0        0     3686 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin
+-rw-r--r--   0        0        0     3282 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin
+-rw-r--r--   0        0        0     3686 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin
+-rw-r--r--   0        0        0     3282 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin
+-rw-r--r--   0        0        0     3686 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.xml.bin
+-rw-r--r--   0        0        0     1827 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin
+-rw-r--r--   0        0        0     2023 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin
+-rw-r--r--   0        0        0     1827 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin
+-rw-r--r--   0        0        0     2023 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin
+-rw-r--r--   0        0        0     1827 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin
+-rw-r--r--   0        0        0     2023 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.xml.bin
+-rw-r--r--   0        0        0     2577 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin
+-rw-r--r--   0        0        0     2822 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin
+-rw-r--r--   0        0        0     2577 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin
+-rw-r--r--   0        0        0     2822 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin
+-rw-r--r--   0        0        0     2577 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin
+-rw-r--r--   0        0        0     2822 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.0.xml.bin
+-rw-r--r--   0        0        0      308 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.1.xml.bin
+-rw-r--r--   0        0        0     1081 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin
+-rw-r--r--   0        0        0     1083 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin
+-rw-r--r--   0        0        0     1081 2024-04-09 15:17:34.817742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin
+-rw-r--r--   0        0        0     1083 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin
+-rw-r--r--   0        0        0     2201 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin
+-rw-r--r--   0        0        0     2273 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin
+-rw-r--r--   0        0        0     2201 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin
+-rw-r--r--   0        0        0     2273 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin
+-rw-r--r--   0        0        0     2201 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin
+-rw-r--r--   0        0        0     2273 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.0.xml.bin
+-rw-r--r--   0        0        0      308 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.1.xml.bin
+-rw-r--r--   0        0        0      886 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin
+-rw-r--r--   0        0        0      821 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin
+-rw-r--r--   0        0        0      886 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin
+-rw-r--r--   0        0        0      821 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin
+-rw-r--r--   0        0        0     2006 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin
+-rw-r--r--   0        0        0     2011 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin
+-rw-r--r--   0        0        0     2006 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin
+-rw-r--r--   0        0        0     2011 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin
+-rw-r--r--   0        0        0     2006 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin
+-rw-r--r--   0        0        0     2011 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.xml.bin
+-rw-r--r--   0        0        0     2014 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin
+-rw-r--r--   0        0        0     2243 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin
+-rw-r--r--   0        0        0     2014 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin
+-rw-r--r--   0        0        0     2243 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin
+-rw-r--r--   0        0        0     2014 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin
+-rw-r--r--   0        0        0     2243 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.xml.bin
+-rw-r--r--   0        0        0     2025 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin
+-rw-r--r--   0        0        0     2268 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin
+-rw-r--r--   0        0        0     2025 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin
+-rw-r--r--   0        0        0     2268 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin
+-rw-r--r--   0        0        0     2025 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin
+-rw-r--r--   0        0        0     2268 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin
+-rw-r--r--   0        0        0      596 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin
+-rw-r--r--   0        0        0      695 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin
+-rw-r--r--   0        0        0     1561 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin
+-rw-r--r--   0        0        0     1597 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin
+-rw-r--r--   0        0        0     1561 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin
+-rw-r--r--   0        0        0     1597 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin
+-rw-r--r--   0        0        0     2702 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin
+-rw-r--r--   0        0        0     2804 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin
+-rw-r--r--   0        0        0     2702 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin
+-rw-r--r--   0        0        0     2804 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin
+-rw-r--r--   0        0        0     2702 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin
+-rw-r--r--   0        0        0     2804 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin
+-rw-r--r--   0        0        0      662 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin
+-rw-r--r--   0        0        0      678 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin
+-rw-r--r--   0        0        0     1385 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin
+-rw-r--r--   0        0        0     1402 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin
+-rw-r--r--   0        0        0     1385 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin
+-rw-r--r--   0        0        0     1402 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin
+-rw-r--r--   0        0        0     2526 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin
+-rw-r--r--   0        0        0     2609 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin
+-rw-r--r--   0        0        0     2526 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin
+-rw-r--r--   0        0        0     2609 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin
+-rw-r--r--   0        0        0     2526 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin
+-rw-r--r--   0        0        0     2609 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.0.xml.bin
+-rw-r--r--   0        0        0      847 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin
+-rw-r--r--   0        0        0     1085 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin
+-rw-r--r--   0        0        0     1163 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin
+-rw-r--r--   0        0        0     1085 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin
+-rw-r--r--   0        0        0     1163 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin
+-rw-r--r--   0        0        0     2205 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin
+-rw-r--r--   0        0        0     2353 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin
+-rw-r--r--   0        0        0     2205 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin
+-rw-r--r--   0        0        0     2353 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin
+-rw-r--r--   0        0        0     2205 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin
+-rw-r--r--   0        0        0     2353 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.1.xml.bin
+-rw-r--r--   0        0        0     8540 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin
+-rw-r--r--   0        0        0     8315 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin
+-rw-r--r--   0        0        0    10266 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin
+-rw-r--r--   0        0        0     9628 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin
+-rw-r--r--   0        0        0    13173 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin
+-rw-r--r--   0        0        0    12575 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin
+-rw-r--r--   0        0        0    13173 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin
+-rw-r--r--   0        0        0    12575 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin
+-rw-r--r--   0        0        0    14338 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin
+-rw-r--r--   0        0        0    13889 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin
+-rw-r--r--   0        0        0     2950 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin
+-rw-r--r--   0        0        0     3403 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin
+-rw-r--r--   0        0        0     2603 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin
+-rw-r--r--   0        0        0     2993 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin
+-rw-r--r--   0        0        0     2313 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin
+-rw-r--r--   0        0        0     2521 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin
+-rw-r--r--   0        0        0     2950 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin
+-rw-r--r--   0        0        0     3403 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin
+-rw-r--r--   0        0        0     2498 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin
+-rw-r--r--   0        0        0     2716 2024-04-09 15:17:34.821742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin
+-rw-r--r--   0        0        0     2028 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin
+-rw-r--r--   0        0        0     2102 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin
+-rw-r--r--   0        0        0     2028 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin
+-rw-r--r--   0        0        0     2102 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin
+-rw-r--r--   0        0        0     2028 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin
+-rw-r--r--   0        0        0     2102 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin
+-rw-r--r--   0        0        0     1199 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin
+-rw-r--r--   0        0        0     4993 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin
+-rw-r--r--   0        0        0     7631 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin
+-rw-r--r--   0        0        0     7396 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin
+-rw-r--r--   0        0        0     8830 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin
+-rw-r--r--   0        0        0     8293 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin
+-rw-r--r--   0        0        0    11737 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin
+-rw-r--r--   0        0        0    11240 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin
+-rw-r--r--   0        0        0    11737 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin
+-rw-r--r--   0        0        0    11240 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin
+-rw-r--r--   0        0        0    11906 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin
+-rw-r--r--   0        0        0    11441 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin
+-rw-r--r--   0        0        0      307 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.0.xml.bin
+-rw-r--r--   0        0        0      477 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.1.xml.bin
+-rw-r--r--   0        0        0      860 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin
+-rw-r--r--   0        0        0      859 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin
+-rw-r--r--   0        0        0      860 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin
+-rw-r--r--   0        0        0      859 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin
+-rw-r--r--   0        0        0     1980 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin
+-rw-r--r--   0        0        0     2049 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin
+-rw-r--r--   0        0        0     1980 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin
+-rw-r--r--   0        0        0     2049 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin
+-rw-r--r--   0        0        0     1980 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin
+-rw-r--r--   0        0        0     2049 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin
+-rw-r--r--   0        0        0      395 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.0.xml.bin
+-rw-r--r--   0        0        0      572 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin
+-rw-r--r--   0        0        0      952 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin
+-rw-r--r--   0        0        0      961 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin
+-rw-r--r--   0        0        0      952 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin
+-rw-r--r--   0        0        0      961 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin
+-rw-r--r--   0        0        0     2093 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin
+-rw-r--r--   0        0        0     2168 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin
+-rw-r--r--   0        0        0     2093 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin
+-rw-r--r--   0        0        0     2168 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin
+-rw-r--r--   0        0        0     2093 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin
+-rw-r--r--   0        0        0     2168 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin
+-rw-r--r--   0        0        0     3848 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin
+-rw-r--r--   0        0        0     3888 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin
+-rw-r--r--   0        0        0     3848 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin
+-rw-r--r--   0        0        0     3888 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin
+-rw-r--r--   0        0        0     3848 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin
+-rw-r--r--   0        0        0     3888 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin
+-rw-r--r--   0        0        0     2028 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin
+-rw-r--r--   0        0        0     2102 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin
+-rw-r--r--   0        0        0     2028 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin
+-rw-r--r--   0        0        0     2102 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin
+-rw-r--r--   0        0        0     3782 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin
+-rw-r--r--   0        0        0     3937 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin
+-rw-r--r--   0        0        0     5189 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin
+-rw-r--r--   0        0        0     5704 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin
+-rw-r--r--   0        0        0     5189 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin
+-rw-r--r--   0        0        0     5704 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin
+-rw-r--r--   0        0        0     5382 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin
+-rw-r--r--   0        0        0     5929 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin
+-rw-r--r--   0        0        0      448 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.0.xml.bin
+-rw-r--r--   0        0        0      723 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin
+-rw-r--r--   0        0        0     1056 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin
+-rw-r--r--   0        0        0     1071 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin
+-rw-r--r--   0        0        0     1243 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin
+-rw-r--r--   0        0        0     1214 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin
+-rw-r--r--   0        0        0     2384 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin
+-rw-r--r--   0        0        0     2421 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin
+-rw-r--r--   0        0        0     2384 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin
+-rw-r--r--   0        0        0     2421 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin
+-rw-r--r--   0        0        0     2384 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin
+-rw-r--r--   0        0        0     2421 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin
+-rw-r--r--   0        0        0     2950 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin
+-rw-r--r--   0        0        0     3403 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin
+-rw-r--r--   0        0        0      655 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin
+-rw-r--r--   0        0        0      980 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin
+-rw-r--r--   0        0        0     1582 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin
+-rw-r--r--   0        0        0     1579 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin
+-rw-r--r--   0        0        0     1769 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin
+-rw-r--r--   0        0        0     1722 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin
+-rw-r--r--   0        0        0     2889 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin
+-rw-r--r--   0        0        0     2912 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin
+-rw-r--r--   0        0        0     2889 2024-04-09 15:17:34.825742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin
+-rw-r--r--   0        0        0     2912 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin
+-rw-r--r--   0        0        0     2889 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin
+-rw-r--r--   0        0        0     2912 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin
+-rw-r--r--   0        0        0      654 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin
+-rw-r--r--   0        0        0     1045 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin
+-rw-r--r--   0        0        0     1562 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin
+-rw-r--r--   0        0        0     1577 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin
+-rw-r--r--   0        0        0     1749 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin
+-rw-r--r--   0        0        0     1720 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin
+-rw-r--r--   0        0        0     2890 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin
+-rw-r--r--   0        0        0     2927 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin
+-rw-r--r--   0        0        0     2890 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin
+-rw-r--r--   0        0        0     2927 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin
+-rw-r--r--   0        0        0     2890 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin
+-rw-r--r--   0        0        0     2927 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.0.xml.bin
+-rw-r--r--   0        0        0      431 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.1.xml.bin
+-rw-r--r--   0        0        0      629 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin
+-rw-r--r--   0        0        0      666 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin
+-rw-r--r--   0        0        0      792 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin
+-rw-r--r--   0        0        0      797 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin
+-rw-r--r--   0        0        0     1933 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin
+-rw-r--r--   0        0        0     2004 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin
+-rw-r--r--   0        0        0     1933 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin
+-rw-r--r--   0        0        0     2004 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin
+-rw-r--r--   0        0        0     1933 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin
+-rw-r--r--   0        0        0     2004 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin
+-rw-r--r--   0        0        0      516 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin
+-rw-r--r--   0        0        0      814 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin
+-rw-r--r--   0        0        0     2131 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin
+-rw-r--r--   0        0        0     2058 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin
+-rw-r--r--   0        0        0     2231 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin
+-rw-r--r--   0        0        0     2149 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin
+-rw-r--r--   0        0        0     3288 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin
+-rw-r--r--   0        0        0     3288 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin
+-rw-r--r--   0        0        0     3288 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin
+-rw-r--r--   0        0        0     3288 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin
+-rw-r--r--   0        0        0     3371 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin
+-rw-r--r--   0        0        0     3343 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin
+-rw-r--r--   0        0        0      448 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.0.xml.bin
+-rw-r--r--   0        0        0      723 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin
+-rw-r--r--   0        0        0     1575 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin
+-rw-r--r--   0        0        0     1577 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin
+-rw-r--r--   0        0        0     1762 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin
+-rw-r--r--   0        0        0     1720 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin
+-rw-r--r--   0        0        0     2903 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin
+-rw-r--r--   0        0        0     2927 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin
+-rw-r--r--   0        0        0     2903 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin
+-rw-r--r--   0        0        0     2927 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin
+-rw-r--r--   0        0        0     2903 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin
+-rw-r--r--   0        0        0     2927 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin
+-rw-r--r--   0        0        0      245 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.0.xml.bin
+-rw-r--r--   0        0        0      459 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.1.xml.bin
+-rw-r--r--   0        0        0     1475 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin
+-rw-r--r--   0        0        0     1382 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin
+-rw-r--r--   0        0        0     1649 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin
+-rw-r--r--   0        0        0     1533 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin
+-rw-r--r--   0        0        0     2748 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin
+-rw-r--r--   0        0        0     2706 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin
+-rw-r--r--   0        0        0     2748 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin
+-rw-r--r--   0        0        0     2706 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin
+-rw-r--r--   0        0        0     2748 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin
+-rw-r--r--   0        0        0     2706 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.1.xml.bin
+-rw-r--r--   0        0        0     3900 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin
+-rw-r--r--   0        0        0     4021 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin
+-rw-r--r--   0        0        0     4263 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin
+-rw-r--r--   0        0        0     4295 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin
+-rw-r--r--   0        0        0     7224 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin
+-rw-r--r--   0        0        0     7288 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin
+-rw-r--r--   0        0        0     7224 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin
+-rw-r--r--   0        0        0     7288 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin
+-rw-r--r--   0        0        0     7779 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin
+-rw-r--r--   0        0        0     7939 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.1.xml.bin
+-rw-r--r--   0        0        0     2106 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin
+-rw-r--r--   0        0        0     2196 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin
+-rw-r--r--   0        0        0     2469 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin
+-rw-r--r--   0        0        0     2470 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin
+-rw-r--r--   0        0        0     5430 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin
+-rw-r--r--   0        0        0     5463 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin
+-rw-r--r--   0        0        0     5430 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin
+-rw-r--r--   0        0        0     5463 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin
+-rw-r--r--   0        0        0     5599 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin
+-rw-r--r--   0        0        0     5664 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.1.xml.bin
+-rw-r--r--   0        0        0     1030 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin
+-rw-r--r--   0        0        0     1040 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin
+-rw-r--r--   0        0        0     1030 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin
+-rw-r--r--   0        0        0     1040 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin
+-rw-r--r--   0        0        0     2171 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin
+-rw-r--r--   0        0        0     2247 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin
+-rw-r--r--   0        0        0     2171 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin
+-rw-r--r--   0        0        0     2247 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin
+-rw-r--r--   0        0        0     2171 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin
+-rw-r--r--   0        0        0     2247 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin
+-rw-r--r--   0        0        0     2957 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/test_component.py
+-rw-r--r--   0        0        0     3283 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/test_deserialize_json.py
+-rw-r--r--   0        0        0     1764 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/test_deserialize_xml.py
+-rw-r--r--   0        0        0    19038 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/test_enums.py
+-rw-r--r--   0        0        0     4389 2024-04-09 15:17:34.829742 cyclonedx_python_lib-7.0.0a1/tests/test_factory_license.py
+-rw-r--r--   0        0        0    22602 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model.py
+-rw-r--r--   0        0        0    13254 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model_bom.py
+-rw-r--r--   0        0        0     2782 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model_bom_ref.py
+-rw-r--r--   0        0        0    18544 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model_component.py
+-rw-r--r--   0        0        0     1793 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model_dependency.py
+-rw-r--r--   0        0        0     4064 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model_issue.py
+-rw-r--r--   0        0        0     4295 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model_license.py
+-rw-r--r--   0        0        0     2758 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model_release_note.py
+-rw-r--r--   0        0        0     3390 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model_service.py
+-rw-r--r--   0        0        0    14370 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_model_vulnerability.py
+-rw-r--r--   0        0        0     3154 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_output.py
+-rw-r--r--   0        0        0     4587 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_output_json.py
+-rw-r--r--   0        0        0     4029 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_output_xml.py
+-rw-r--r--   0        0        0     1307 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_real_world_examples.py
+-rw-r--r--   0        0        0     2509 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_schema_SchemaVersion.py
+-rw-r--r--   0        0        0     1248 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_schema__res.py
+-rw-r--r--   0        0        0     2873 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_spdx.py
+-rw-r--r--   0        0        0     1977 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_validation.py
+-rw-r--r--   0        0        0     4529 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_validation_json.py
+-rw-r--r--   0        0        0     3061 2024-04-09 15:17:34.833742 cyclonedx_python_lib-7.0.0a1/tests/test_validation_xml.py
+-rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 cyclonedx_python_lib-7.0.0a1/PKG-INFO
```

### Comparing `cyclonedx_python_lib-7.0.0/CHANGELOG.md` & `cyclonedx_python_lib-7.0.0a1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,182 +1,11 @@
 # CHANGELOG
 
 
 
-## v7.0.0-alpha.1 (2024-04-09)
-
-### Chore
-
-* chore(deps): bump `py-serializable` to &gt;=1.0.3 to resolve issues with deserialization to XML
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`0398051`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/039805174f76f2b228e4436e01752ec7893df30f))
-
-* chore(deps-dev): update autopep8 requirement from 2.0.4 to 2.1.0 (#573)
-
-Updates the requirements on [autopep8](https://github.com/hhatto/autopep8) to permit the latest version.
-- [Release notes](https://github.com/hhatto/autopep8/releases)
-- [Commits](https://github.com/hhatto/autopep8/compare/v2.0.4...v2.1.0)
-
----
-updated-dependencies:
-- dependency-name: autopep8
-  dependency-type: direct:development
-...
-
-Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
-Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`35749c6`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/35749c6cd18ebb8911b7cefac8a381d2ee57177a))
-
-* chore(deps-dev): update tox requirement from 4.14.1 to 4.14.2 (#574)
-
-Updates the requirements on [tox](https://github.com/tox-dev/tox) to permit the latest version.
-- [Release notes](https://github.com/tox-dev/tox/releases)
-- [Changelog](https://github.com/tox-dev/tox/blob/main/docs/changelog.rst)
-- [Commits](https://github.com/tox-dev/tox/compare/4.14.1...4.14.2)
-
----
-updated-dependencies:
-- dependency-name: tox
-  dependency-type: direct:development
-...
-
-Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
-Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`d60f457`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/d60f4570621246ce3d68e7f2e7f1aa831fb818f0))
-
-### Unknown
-
-* docs
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`42c6f25`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/42c6f253f0ee4a26230d7c119d622154f34d9795))
-
-* refactor
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`b4a133a`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/b4a133ab916ce66a2a955ff1c9bc8596234a8b30))
-
-* style
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`0843234`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/084323425fed612331c8f519e0a9ea7dfc4db636))
-
-* refactor
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`62c1d9a`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/62c1d9a18c0e0a2efb8f215e68a46057177733a0))
-
-* reformat
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`e10ffee`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/e10ffee9c8cd4a2fcfe9f06fce5a1e5d4c8157fe))
-
-* reformat
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`e0184cc`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/e0184cc4f098634076d11234b3cb949c5fba5bd9))
-
-* fetch test data for CDX 1.6
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`618a292`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/618a29258d576e96163be51511710232de16fe53))
-
-* fetch schema 1.6 JSON
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`289e81a`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/289e81a7e65e39d3960a9e57e9e75079966f2db1))
-
-* update schema to published versions
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`0449de2`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/0449de2e87b6907e8712a504d1fb7a5ebf14fbc2))
-
-* more proper way to filter test cases
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`0a2ca2c`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/0a2ca2cfe42fd7306b69ea7c5df3d603bca5c43d))
-
-* add `acknowledgement` to `LicenseExpression` (#582)
-
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`ddd7847`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/ddd7847c9a70faa353000e0cfeeb710d8df5bb93))
-
-* coding standards and typing
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`5c97c2d`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/5c97c2d22595479ae4b464baf04da9113c40a549))
-
-* raise `UserWarning` in `.component.version` has length &gt; 1024
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`abebd4f`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/abebd4f63d23d95b1a126c710dabf924689a8695))
-
-* Added `address` to `organizationalEntity`
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`1327558`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/1327558454b5f30f478783ae6cbbe4de73f1e011))
-
-* Added `address` to `organizationalEntity`
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`318d723`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/318d7238cab1805a3524413b6d10314065284cb7))
-
-* coding standards
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`d294620`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/d294620e44d8498025fa98e99e65f3366eb66fc2))
-
-* corrected CryptoMode enum
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`71e4bc6`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/71e4bc6fdc70c75187baf51a0e45fb21afe62d79))
-
-* additional tests to increase code coverage
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`f504daa`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/f504daadbb633a1e46ab474f97f76717c3358f0b))
-
-* coding standards
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`a3e09d1`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/a3e09d1bf0fde331e4e7e4685db4ed391c16d765))
-
-* test filtering
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`14f699f`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/14f699fe3d9ea282c47e5a6947d783a6ca0304c5))
-
-* coding standards
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`b23df1f`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/b23df1fcbe9af2657e47a436d00409e75bfd6b18))
-
-* typing and bandit ignores
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`96a6dc9`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/96a6dc9d5684589951dd3541b5cfa24160689b41))
-
-* add `.component.cryptoProperties` - with test failures for SchemaVersion &lt; 1.6
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`1e71dc3`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/1e71dc3da931500e1c332034cb244bf8230a7360))
-
-* properly added `.component.swhid`
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`ee80ea3`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/ee80ea32a91941349e0a81c1b4345a9fa73d6943))
-
-* imports tidied
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`875a338`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/875a338337a77fca3f51f41f65136dc5ec1ccdb9))
-
-* work to get deserialization tests passing
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`fdece59`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/fdece595c5ffec1f47b0fe5f1fc57aad06677107))
-
-* work to add `.component.omniborid` - but tests deserialisation tests fail due to schema differences (`.component.author` not in 1.6)
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`af7b92b`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/af7b92b0b4736610806504f73784333920592a45))
-
-* Deprecated `.component.author`. Added `.component.authors` and `.component.manufacturer`
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`6227c08`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/6227c08af50c4c612baaedc64976652cd53e3a1b))
-
-* work on `bom.metadata` for v1.6
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`6192ed8`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/6192ed886faec9b51f080db628659d4246ebae70))
-
-* note `bom.metadata.manufacture` as deprecated
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`240dfaa`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/240dfaa00a74c66e71d8d65864bf492b67d5310a))
-
-* re-generated test snapshots for v1.6
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`8132c3e`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/8132c3ec59084e84156eb815e9da9277541e2afd))
-
-* added draft v1.6 schemas and boilerplate for v1.6
-
-Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`41ca1e0`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/41ca1e007c73692d5ada6af6318b0c5ff42fa11d))
-
-
 ## v6.4.4 (2024-03-18)
 
 ### Chore
 
 * chore(deps-dev): update coverage requirement from 7.4.3 to 7.4.4 (#570)
 
 Updates the requirements on [coverage](https://github.com/nedbat/coveragepy) to permit the latest version.
```

### Comparing `cyclonedx_python_lib-7.0.0/LICENSE` & `cyclonedx_python_lib-7.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/README.md` & `cyclonedx_python_lib-7.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
 """
 Python library for CycloneDX
 """
 
 # !! version is managed by semantic_release
 # do not use typing here, or else `semantic_release` might have issues finding the variable
-__version__ = "7.0.0"  # noqa:Q000
+__version__ = "7.0.0-alpha.1"  # noqa:Q000
```

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/_internal/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/_internal/compare.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/compare.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/_internal/hash.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/hash.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/_internal/time.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/time.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/exception/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/exception/factory.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/factory.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/exception/model.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/exception/output.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/exception/serialization.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/serialization.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/factory/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/factory/license.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/factory/license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/bom.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/bom_ref.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/component.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/contact.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/contact.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/crypto.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/crypto.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/dependency.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/impact_analysis.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/impact_analysis.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/issue.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/license.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/release_note.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/service.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/service.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/model/vulnerability.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/vulnerability.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/output/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/output/json.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/output/json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/output/xml.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/output/xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/README.md` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/README.md`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/schema/schema.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/serialization/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/spdx.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/validation/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/validation/json.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/validation/model.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/cyclonedx/validation/xml.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/Makefile` & `cyclonedx_python_lib-7.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/architecture.rst` & `cyclonedx_python_lib-7.0.0a1/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/changelog.rst` & `cyclonedx_python_lib-7.0.0a1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/conf.py` & `cyclonedx_python_lib-7.0.0a1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 project = 'CycloneDX Python Library'
 copyright = '2022, Copyright (c) OWASP Foundation'
 author = 'Paul Horton, Jan Kowalleck, Steve Springett, Patrick Dwyer'
 
 # The full version, including alpha/beta/rc tags
 # !! version is managed by semantic_release
-release = '7.0.0'
+release = '7.0.0-alpha.1'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `cyclonedx_python_lib-7.0.0/docs/examples.rst` & `cyclonedx_python_lib-7.0.0a1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/index.rst` & `cyclonedx_python_lib-7.0.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/install.rst` & `cyclonedx_python_lib-7.0.0a1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/make.bat` & `cyclonedx_python_lib-7.0.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/modelling.rst` & `cyclonedx_python_lib-7.0.0a1/docs/modelling.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/outputting.rst` & `cyclonedx_python_lib-7.0.0a1/docs/outputting.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/schema-support.rst` & `cyclonedx_python_lib-7.0.0a1/docs/schema-support.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/docs/support.rst` & `cyclonedx_python_lib-7.0.0a1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/examples/complex_deserialize.py` & `cyclonedx_python_lib-7.0.0a1/examples/complex_deserialize.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/examples/complex_serialize.py` & `cyclonedx_python_lib-7.0.0a1/examples/complex_serialize.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/pyproject.toml` & `cyclonedx_python_lib-7.0.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cyclonedx-python-lib"
 # !! version is managed by semantic_release
-version = "7.0.0"
+version = "7.0.0-alpha.1"
 description = "Python library for CycloneDX"
 authors = [
   "Paul Horton <phorton@sonatype.com>",
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
 ]
 maintainers = [
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
```

### Comparing `cyclonedx_python_lib-7.0.0/tests/__init__.py` & `cyclonedx_python_lib-7.0.0a1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/__init__.py` & `cyclonedx_python_lib-7.0.0a1/tests/_data/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/models.py` & `cyclonedx_python_lib-7.0.0a1/tests/_data/models.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/own/json/1.2/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/json/1.2/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/own/json/1.3/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/json/1.3/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/own/json/1.4/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/json/1.4/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/own/xml/1.4/bom_setuptools.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/xml/1.4/bom_setuptools.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/own/xml/1.4/webgoat-6.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/xml/1.4/webgoat-6.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-bom-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-patch-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-service-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-service-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-service-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-service-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-bom-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-patch-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-properties-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-service-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-service-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-service-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-service-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-bom-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-patch-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-properties-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-service-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-service-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-service-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-service-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-bom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-patch-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-properties-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-service-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-service-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-service-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-service-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-bom-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-patch-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-properties-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-service-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-service-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-service-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-service-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-standard-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/schemaTestData/fetch.sh` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/fetch.sh`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_Encoding-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_component.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_deserialize_json.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_deserialize_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_deserialize_xml.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_deserialize_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_enums.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_factory_license.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_factory_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model_bom.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model_bom_ref.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model_component.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model_dependency.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model_issue.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model_license.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model_release_note.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model_service.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_service.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_model_vulnerability.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_vulnerability.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_output.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_output_json.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_output_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_output_xml.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_output_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_real_world_examples.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_real_world_examples.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_schema_SchemaVersion.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_schema_SchemaVersion.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_schema__res.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_schema__res.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_spdx.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_validation.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_validation_json.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_validation_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/tests/test_validation_xml.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_validation_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.0.0/PKG-INFO` & `cyclonedx_python_lib-7.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclonedx-python-lib
-Version: 7.0.0
+Version: 7.0.0a1
 Summary: Python library for CycloneDX
 Home-page: https://github.com/CycloneDX/cyclonedx-python-lib/#readme
 License: Apache-2.0
 Keywords: CycloneDX,library,OWASP,SCA,Software Bill of Materials,Bill of Materials,BOM,SBOM,VEX,VDR,OBOM,MBOM,SaaSBOM,SPDX,PackageURL,PURL
 Author: Paul Horton
 Author-email: phorton@sonatype.com
 Maintainer: Jan Kowalleck
```

