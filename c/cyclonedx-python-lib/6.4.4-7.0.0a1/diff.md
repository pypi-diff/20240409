# Comparing `tmp/cyclonedx_python_lib-6.4.4.tar.gz` & `tmp/cyclonedx_python_lib-7.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx_python_lib-6.4.4.tar", max compression
+gzip compressed data, was "cyclonedx_python_lib-7.0.0a1.tar", max compression
```

## Comparing `cyclonedx_python_lib-6.4.4.tar` & `cyclonedx_python_lib-7.0.0a1.tar`

### file list

```diff
@@ -1,899 +1,1135 @@
--rw-r--r--   0        0        0   216430 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/LICENSE
--rw-r--r--   0        0        0      147 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/NOTICE
--rw-r--r--   0        0        0     4569 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/README.md
--rw-r--r--   0        0        0      850 2024-03-18 18:13:30.950068 cyclonedx_python_lib-6.4.4/cyclonedx/__init__.py
--rw-r--r--   0        0        0      731 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/_internal/__init__.py
--rw-r--r--   0        0        0     1734 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/_internal/compare.py
--rw-r--r--   0        0        0     1164 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/_internal/hash.py
--rw-r--r--   0        0        0      847 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/_internal/time.py
--rw-r--r--   0        0        0      993 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/__init__.py
--rw-r--r--   0        0        0     1536 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/factory.py
--rw-r--r--   0        0        0     2642 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/model.py
--rw-r--r--   0        0        0     1136 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/output.py
--rw-r--r--   0        0        0     1730 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/serialization.py
--rw-r--r--   0        0        0      680 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/factory/__init__.py
--rw-r--r--   0        0        0     3233 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/factory/license.py
--rw-r--r--   0        0        0    48114 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/__init__.py
--rw-r--r--   0        0        0    23268 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/bom.py
--rw-r--r--   0        0        0     2179 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/bom_ref.py
--rw-r--r--   0        0        0    47132 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/component.py
--rw-r--r--   0        0        0     3766 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/dependency.py
--rw-r--r--   0        0        0     3568 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/impact_analysis.py
--rw-r--r--   0        0        0     7024 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/issue.py
--rw-r--r--   0        0        0     8020 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/license.py
--rw-r--r--   0        0        0     8623 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/release_note.py
--rw-r--r--   0        0        0    12676 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/service.py
--rw-r--r--   0        0        0    43554 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/vulnerability.py
--rw-r--r--   0        0        0     5872 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/output/__init__.py
--rw-r--r--   0        0        0     4060 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/output/json.py
--rw-r--r--   0        0        0     4173 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/output/xml.py
--rw-r--r--   0        0        0      153 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/py.typed
--rw-r--r--   0        0        0     3000 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/__init__.py
--rw-r--r--   0        0        0     1961 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/README.md
--rw-r--r--   0        0        0     2364 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/__init__.py
--rw-r--r--   0        0        0    13604 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd
--rw-r--r--   0        0        0    39716 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd
--rw-r--r--   0        0        0    37194 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    36226 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    76383 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd
--rw-r--r--   0        0        0    40408 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    39348 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    88794 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd
--rw-r--r--   0        0        0    72383 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   133792 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd
--rw-r--r--   0        0        0   164772 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   311805 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd
--rw-r--r--   0        0        0     8058 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    12322 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   144335 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd
--rw-r--r--   0        0        0     2367 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/schema.py
--rw-r--r--   0        0        0     6479 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/serialization/__init__.py
--rw-r--r--   0        0        0     2503 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/spdx.py
--rw-r--r--   0        0        0     3701 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/validation/__init__.py
--rw-r--r--   0        0        0     4817 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/validation/json.py
--rw-r--r--   0        0        0      853 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/validation/model.py
--rw-r--r--   0        0        0     3672 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/validation/xml.py
--rw-r--r--   0        0        0      634 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/Makefile
--rw-r--r--   0        0        0     1524 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/architecture.rst
--rw-r--r--   0        0        0      686 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/changelog.rst
--rw-r--r--   0        0        0     2657 2024-03-18 18:13:30.950068 cyclonedx_python_lib-6.4.4/docs/conf.py
--rw-r--r--   0        0        0       34 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/contributing.rst
--rw-r--r--   0        0        0      895 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/examples.rst
--rw-r--r--   0        0        0     1857 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/index.rst
--rw-r--r--   0        0        0     1499 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/install.rst
--rw-r--r--   0        0        0      800 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/make.bat
--rw-r--r--   0        0        0     3275 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/modelling.rst
--rw-r--r--   0        0        0     2269 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/outputting.rst
--rw-r--r--   0        0        0       81 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/requirements.txt
--rw-r--r--   0        0        0     4961 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/schema-support.rst
--rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/support.rst
--rw-r--r--   0        0        0      176 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/examples/README.md
--rw-r--r--   0        0        0     8164 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/examples/complex_deserialize.py
--rw-r--r--   0        0        0     4046 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/examples/complex_serialize.py
--rw-r--r--   0        0        0     4226 2024-03-18 18:13:30.950068 cyclonedx_python_lib-6.4.4/pyproject.toml
--rw-r--r--   0        0        0     5985 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/__init__.py
--rw-r--r--   0        0        0      704 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/__init__.py
--rw-r--r--   0        0        0    31717 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/models.py
--rw-r--r--   0        0        0       16 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/README.md
--rw-r--r--   0        0        0     1309 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.2/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1309 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.3/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1309 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.4/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     2461 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/xml/1.4/bom_setuptools.xml
--rw-r--r--   0        0        0    98508 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/xml/1.4/webgoat-6.1.xml
--rw-r--r--   0        0        0     3723 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml
--rw-r--r--   0        0        0     1195 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml
--rw-r--r--   0        0        0      559 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml
--rw-r--r--   0        0        0      313 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-component-type-1.1.xml
--rw-r--r--   0        0        0      246 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-empty-component-1.1.xml
--rw-r--r--   0        0        0      830 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml
--rw-r--r--   0        0        0      801 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml
--rw-r--r--   0        0        0      793 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml
--rw-r--r--   0        0        0      769 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml
--rw-r--r--   0        0        0      705 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml
--rw-r--r--   0        0        0     1303 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml
--rw-r--r--   0        0        0    16515 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml
--rw-r--r--   0        0        0    16513 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml
--rw-r--r--   0        0        0     1328 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml
--rw-r--r--   0        0        0     1366 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml
--rw-r--r--   0        0        0      302 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-missing-component-type-1.1.xml
--rw-r--r--   0        0        0    21038 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml
--rw-r--r--   0        0        0      348 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-scope-1.1.xml
--rw-r--r--   0        0        0    21026 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml
--rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml
--rw-r--r--   0        0        0     1217 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml
--rw-r--r--   0        0        0      704 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml
--rw-r--r--   0        0        0      965 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml
--rw-r--r--   0        0        0      186 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-empty-components-1.1.xml
--rw-r--r--   0        0        0    22339 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml
--rw-r--r--   0        0        0     1210 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml
--rw-r--r--   0        0        0     1214 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml
--rw-r--r--   0        0        0     1226 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml
--rw-r--r--   0        0        0      317 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-minimal-viable-1.1.xml
--rw-r--r--   0        0        0    21121 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml
--rw-r--r--   0        0        0    10048 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml
--rw-r--r--   0        0        0      165 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-bomformat-1.2.json
--rw-r--r--   0        0        0      394 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.json
--rw-r--r--   0        0        0      560 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml
--rw-r--r--   0        0        0      385 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.json
--rw-r--r--   0        0        0      433 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.xml
--rw-r--r--   0        0        0      249 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.json
--rw-r--r--   0        0        0      314 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.xml
--rw-r--r--   0        0        0      667 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json
--rw-r--r--   0        0        0      809 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml
--rw-r--r--   0        0        0      247 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-empty-component-1.2.xml
--rw-r--r--   0        0        0      856 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json
--rw-r--r--   0        0        0      831 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml
--rw-r--r--   0        0        0      827 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json
--rw-r--r--   0        0        0      802 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml
--rw-r--r--   0        0        0      819 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json
--rw-r--r--   0        0        0      794 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml
--rw-r--r--   0        0        0      795 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json
--rw-r--r--   0        0        0      770 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml
--rw-r--r--   0        0        0      731 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json
--rw-r--r--   0        0        0      706 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml
--rw-r--r--   0        0        0     1184 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json
--rw-r--r--   0        0        0     1554 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml
--rw-r--r--   0        0        0      515 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json
--rw-r--r--   0        0        0     1304 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml
--rw-r--r--   0        0        0    15788 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json
--rw-r--r--   0        0        0    16516 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml
--rw-r--r--   0        0        0      428 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.json
--rw-r--r--   0        0        0    16514 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml
--rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml
--rw-r--r--   0        0        0     1367 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml
--rw-r--r--   0        0        0      209 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      244 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      303 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-missing-component-type-1.2.xml
--rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml
--rw-r--r--   0        0        0     1185 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json
--rw-r--r--   0        0        0     1555 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml
--rw-r--r--   0        0        0      275 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-scope-1.2.json
--rw-r--r--   0        0        0      349 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-scope-1.2.xml
--rw-r--r--   0        0        0      148 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.json
--rw-r--r--   0        0        0    21027 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.json
--rw-r--r--   0        0        0      416 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.xml
--rw-r--r--   0        0        0      363 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/skip_invalid-empty-component-1.2.json
--rw-r--r--   0        0        0      361 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/skip_invalid-missing-component-type-1.2.json
--rw-r--r--   0        0        0      548 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json
--rw-r--r--   0        0        0      792 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml
--rw-r--r--   0        0        0    20390 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.json
--rw-r--r--   0        0        0    24278 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml
--rw-r--r--   0        0        0     2163 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json
--rw-r--r--   0        0        0     1897 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml
--rw-r--r--   0        0        0      394 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.json
--rw-r--r--   0        0        0      705 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml
--rw-r--r--   0        0        0      456 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.json
--rw-r--r--   0        0        0      492 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.xml
--rw-r--r--   0        0        0     1342 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json
--rw-r--r--   0        0        0     1346 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml
--rw-r--r--   0        0        0      892 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json
--rw-r--r--   0        0        0     1223 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml
--rw-r--r--   0        0        0      693 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json
--rw-r--r--   0        0        0      824 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml
--rw-r--r--   0        0        0      161 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.json
--rw-r--r--   0        0        0      187 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.xml
--rw-r--r--   0        0        0    22340 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml
--rw-r--r--   0        0        0      438 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.json
--rw-r--r--   0        0        0     1211 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-id-1.2.json
--rw-r--r--   0        0        0     1215 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml
--rw-r--r--   0        0        0      440 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-name-1.2.json
--rw-r--r--   0        0        0     1227 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml
--rw-r--r--   0        0        0      333 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.json
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.xml
--rw-r--r--   0        0        0      438 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.json
--rw-r--r--   0        0        0      492 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.xml
--rw-r--r--   0        0        0      417 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.json
--rw-r--r--   0        0        0      468 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.xml
--rw-r--r--   0        0        0      224 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      254 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      605 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json
--rw-r--r--   0        0        0      654 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml
--rw-r--r--   0        0        0      253 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.json
--rw-r--r--   0        0        0      318 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.xml
--rw-r--r--   0        0        0     2465 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.json
--rw-r--r--   0        0        0     3337 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml
--rw-r--r--   0        0        0    21122 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml
--rw-r--r--   0        0        0     2308 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-1.2.json
--rw-r--r--   0        0        0     2693 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-1.2.xml
--rw-r--r--   0        0        0      419 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.json
--rw-r--r--   0        0        0      495 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.xml
--rw-r--r--   0        0        0    11181 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml
--rw-r--r--   0        0        0      165 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-bomformat-1.3.json
--rw-r--r--   0        0        0      394 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.json
--rw-r--r--   0        0        0      560 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml
--rw-r--r--   0        0        0      385 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.json
--rw-r--r--   0        0        0      433 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.xml
--rw-r--r--   0        0        0      249 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.json
--rw-r--r--   0        0        0      314 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.xml
--rw-r--r--   0        0        0      667 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json
--rw-r--r--   0        0        0      809 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml
--rw-r--r--   0        0        0      197 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.json
--rw-r--r--   0        0        0      247 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.xml
--rw-r--r--   0        0        0      856 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json
--rw-r--r--   0        0        0      831 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml
--rw-r--r--   0        0        0      827 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json
--rw-r--r--   0        0        0      802 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml
--rw-r--r--   0        0        0      819 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json
--rw-r--r--   0        0        0      794 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml
--rw-r--r--   0        0        0      795 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json
--rw-r--r--   0        0        0      770 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml
--rw-r--r--   0        0        0      731 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json
--rw-r--r--   0        0        0      706 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml
--rw-r--r--   0        0        0     1184 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json
--rw-r--r--   0        0        0     1554 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml
--rw-r--r--   0        0        0      515 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json
--rw-r--r--   0        0        0     1304 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml
--rw-r--r--   0        0        0    15788 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json
--rw-r--r--   0        0        0    16516 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml
--rw-r--r--   0        0        0      428 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.json
--rw-r--r--   0        0        0    16514 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml
--rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml
--rw-r--r--   0        0        0     1367 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml
--rw-r--r--   0        0        0      277 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.json
--rw-r--r--   0        0        0      319 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      209 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      244 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      228 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.json
--rw-r--r--   0        0        0      303 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.xml
--rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml
--rw-r--r--   0        0        0     1185 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json
--rw-r--r--   0        0        0     1555 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml
--rw-r--r--   0        0        0      275 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-scope-1.3.json
--rw-r--r--   0        0        0      349 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-scope-1.3.xml
--rw-r--r--   0        0        0      148 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.json
--rw-r--r--   0        0        0    21027 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.json
--rw-r--r--   0        0        0      416 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.xml
--rw-r--r--   0        0        0      548 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json
--rw-r--r--   0        0        0      792 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml
--rw-r--r--   0        0        0    20390 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.json
--rw-r--r--   0        0        0    24278 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml
--rw-r--r--   0        0        0     2163 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json
--rw-r--r--   0        0        0     1897 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml
--rw-r--r--   0        0        0      394 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.json
--rw-r--r--   0        0        0      705 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml
--rw-r--r--   0        0        0      456 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.json
--rw-r--r--   0        0        0      492 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.xml
--rw-r--r--   0        0        0     1342 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json
--rw-r--r--   0        0        0     1346 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml
--rw-r--r--   0        0        0      892 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json
--rw-r--r--   0        0        0     1223 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml
--rw-r--r--   0        0        0     1497 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json
--rw-r--r--   0        0        0     1983 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml
--rw-r--r--   0        0        0      693 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json
--rw-r--r--   0        0        0      824 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml
--rw-r--r--   0        0        0      161 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.json
--rw-r--r--   0        0        0      187 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.xml
--rw-r--r--   0        0        0     1384 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json
--rw-r--r--   0        0        0     1596 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml
--rw-r--r--   0        0        0    22340 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml
--rw-r--r--   0        0        0     1117 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json
--rw-r--r--   0        0        0     1324 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml
--rw-r--r--   0        0        0      438 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.json
--rw-r--r--   0        0        0     1211 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-id-1.3.json
--rw-r--r--   0        0        0     1215 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml
--rw-r--r--   0        0        0      440 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-name-1.3.json
--rw-r--r--   0        0        0     1227 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml
--rw-r--r--   0        0        0      333 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.json
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.xml
--rw-r--r--   0        0        0      279 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.json
--rw-r--r--   0        0        0      321 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      438 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.json
--rw-r--r--   0        0        0      492 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.xml
--rw-r--r--   0        0        0      417 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.json
--rw-r--r--   0        0        0      468 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.xml
--rw-r--r--   0        0        0      224 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      254 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      605 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json
--rw-r--r--   0        0        0      654 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml
--rw-r--r--   0        0        0      253 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.json
--rw-r--r--   0        0        0      318 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.xml
--rw-r--r--   0        0        0     2465 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.json
--rw-r--r--   0        0        0     3337 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml
--rw-r--r--   0        0        0      983 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.json
--rw-r--r--   0        0        0     1213 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml
--rw-r--r--   0        0        0    21122 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml
--rw-r--r--   0        0        0     2308 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-1.3.json
--rw-r--r--   0        0        0     2693 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-1.3.xml
--rw-r--r--   0        0        0      419 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.json
--rw-r--r--   0        0        0      495 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.xml
--rw-r--r--   0        0        0    11181 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml
--rw-r--r--   0        0        0      165 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-bomformat-1.4.json
--rw-r--r--   0        0        0      394 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.json
--rw-r--r--   0        0        0      560 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml
--rw-r--r--   0        0        0      385 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.json
--rw-r--r--   0        0        0      433 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.xml
--rw-r--r--   0        0        0      249 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.json
--rw-r--r--   0        0        0      314 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.xml
--rw-r--r--   0        0        0      667 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json
--rw-r--r--   0        0        0      809 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml
--rw-r--r--   0        0        0      197 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.json
--rw-r--r--   0        0        0      247 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.xml
--rw-r--r--   0        0        0      856 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json
--rw-r--r--   0        0        0      831 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml
--rw-r--r--   0        0        0      827 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json
--rw-r--r--   0        0        0      802 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml
--rw-r--r--   0        0        0      819 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json
--rw-r--r--   0        0        0      794 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml
--rw-r--r--   0        0        0      795 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json
--rw-r--r--   0        0        0      770 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml
--rw-r--r--   0        0        0      731 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json
--rw-r--r--   0        0        0      706 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml
--rw-r--r--   0        0        0     1184 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json
--rw-r--r--   0        0        0     1554 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml
--rw-r--r--   0        0        0      515 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json
--rw-r--r--   0        0        0     1304 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml
--rw-r--r--   0        0        0    15788 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json
--rw-r--r--   0        0        0    16516 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml
--rw-r--r--   0        0        0      428 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.json
--rw-r--r--   0        0        0    16514 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml
--rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml
--rw-r--r--   0        0        0     1367 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml
--rw-r--r--   0        0        0      277 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.json
--rw-r--r--   0        0        0      319 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      209 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      244 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      228 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.json
--rw-r--r--   0        0        0      303 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.xml
--rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml
--rw-r--r--   0        0        0     1185 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json
--rw-r--r--   0        0        0     1555 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml
--rw-r--r--   0        0        0      275 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-scope-1.4.json
--rw-r--r--   0        0        0      349 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-scope-1.4.xml
--rw-r--r--   0        0        0      148 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.json
--rw-r--r--   0        0        0    21027 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.json
--rw-r--r--   0        0        0      416 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.xml
--rw-r--r--   0        0        0      548 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json
--rw-r--r--   0        0        0      792 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml
--rw-r--r--   0        0        0    20390 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.json
--rw-r--r--   0        0        0    24278 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml
--rw-r--r--   0        0        0     2163 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json
--rw-r--r--   0        0        0     1897 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml
--rw-r--r--   0        0        0      394 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.json
--rw-r--r--   0        0        0      705 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml
--rw-r--r--   0        0        0      456 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.json
--rw-r--r--   0        0        0      492 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.xml
--rw-r--r--   0        0        0     1342 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json
--rw-r--r--   0        0        0     1346 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml
--rw-r--r--   0        0        0      892 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json
--rw-r--r--   0        0        0     1223 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml
--rw-r--r--   0        0        0     1497 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json
--rw-r--r--   0        0        0     1983 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml
--rw-r--r--   0        0        0      693 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json
--rw-r--r--   0        0        0      824 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml
--rw-r--r--   0        0        0      161 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.json
--rw-r--r--   0        0        0      187 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.xml
--rw-r--r--   0        0        0     1384 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json
--rw-r--r--   0        0        0     1596 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml
--rw-r--r--   0        0        0    22340 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml
--rw-r--r--   0        0        0     1117 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json
--rw-r--r--   0        0        0     1324 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml
--rw-r--r--   0        0        0      438 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.json
--rw-r--r--   0        0        0     1211 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-id-1.4.json
--rw-r--r--   0        0        0     1215 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml
--rw-r--r--   0        0        0      440 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-name-1.4.json
--rw-r--r--   0        0        0     1227 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml
--rw-r--r--   0        0        0      333 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.json
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.xml
--rw-r--r--   0        0        0      279 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.json
--rw-r--r--   0        0        0      321 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      438 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.json
--rw-r--r--   0        0        0      492 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.xml
--rw-r--r--   0        0        0      417 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.json
--rw-r--r--   0        0        0      468 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.xml
--rw-r--r--   0        0        0      224 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      254 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      605 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json
--rw-r--r--   0        0        0      654 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml
--rw-r--r--   0        0        0      227 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.json
--rw-r--r--   0        0        0      281 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.xml
--rw-r--r--   0        0        0     2465 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.json
--rw-r--r--   0        0        0     3337 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml
--rw-r--r--   0        0        0      983 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.json
--rw-r--r--   0        0        0     1213 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml
--rw-r--r--   0        0        0    21122 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml
--rw-r--r--   0        0        0     5338 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json
--rw-r--r--   0        0        0     6828 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml
--rw-r--r--   0        0        0     2312 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-1.4.json
--rw-r--r--   0        0        0     2693 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-1.4.xml
--rw-r--r--   0        0        0      419 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.json
--rw-r--r--   0        0        0      495 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.xml
--rw-r--r--   0        0        0     9733 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json
--rw-r--r--   0        0        0     4274 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json
--rw-r--r--   0        0        0     5987 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml
--rw-r--r--   0        0        0    11181 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml
--rw-r--r--   0        0        0      165 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-bomformat-1.5.json
--rw-r--r--   0        0        0      508 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.json
--rw-r--r--   0        0        0      866 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml
--rw-r--r--   0        0        0      385 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.json
--rw-r--r--   0        0        0      433 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.xml
--rw-r--r--   0        0        0      249 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.json
--rw-r--r--   0        0        0      314 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.xml
--rw-r--r--   0        0        0      746 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json
--rw-r--r--   0        0        0     1086 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml
--rw-r--r--   0        0        0      197 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.json
--rw-r--r--   0        0        0      247 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.xml
--rw-r--r--   0        0        0      856 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json
--rw-r--r--   0        0        0      831 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml
--rw-r--r--   0        0        0      827 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json
--rw-r--r--   0        0        0      802 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml
--rw-r--r--   0        0        0      819 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json
--rw-r--r--   0        0        0      794 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml
--rw-r--r--   0        0        0      795 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json
--rw-r--r--   0        0        0      770 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml
--rw-r--r--   0        0        0      731 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json
--rw-r--r--   0        0        0      706 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml
--rw-r--r--   0        0        0     1184 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json
--rw-r--r--   0        0        0     1554 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml
--rw-r--r--   0        0        0      515 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json
--rw-r--r--   0        0        0     1304 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml
--rw-r--r--   0        0        0    15788 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json
--rw-r--r--   0        0        0    16516 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml
--rw-r--r--   0        0        0      428 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.json
--rw-r--r--   0        0        0    16514 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml
--rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml
--rw-r--r--   0        0        0     1367 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml
--rw-r--r--   0        0        0      277 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.json
--rw-r--r--   0        0        0      319 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      209 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      244 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0      228 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.json
--rw-r--r--   0        0        0      303 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.xml
--rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml
--rw-r--r--   0        0        0     1185 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json
--rw-r--r--   0        0        0     1555 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml
--rw-r--r--   0        0        0      275 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-scope-1.5.json
--rw-r--r--   0        0        0      349 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-scope-1.5.xml
--rw-r--r--   0        0        0      148 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.json
--rw-r--r--   0        0        0    21027 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.json
--rw-r--r--   0        0        0      416 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.xml
--rw-r--r--   0        0        0     2527 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json
--rw-r--r--   0        0        0     3596 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml
--rw-r--r--   0        0        0      548 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json
--rw-r--r--   0        0        0      792 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml
--rw-r--r--   0        0        0    20390 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.json
--rw-r--r--   0        0        0    24278 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml
--rw-r--r--   0        0        0     2163 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json
--rw-r--r--   0        0        0     1897 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml
--rw-r--r--   0        0        0      394 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.json
--rw-r--r--   0        0        0      705 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml
--rw-r--r--   0        0        0      456 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.json
--rw-r--r--   0        0        0      492 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.xml
--rw-r--r--   0        0        0     1342 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json
--rw-r--r--   0        0        0     1346 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml
--rw-r--r--   0        0        0      892 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json
--rw-r--r--   0        0        0     1223 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml
--rw-r--r--   0        0        0     1810 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json
--rw-r--r--   0        0        0     2449 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml
--rw-r--r--   0        0        0      693 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json
--rw-r--r--   0        0        0      824 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml
--rw-r--r--   0        0        0      161 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.json
--rw-r--r--   0        0        0      187 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.xml
--rw-r--r--   0        0        0     3189 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json
--rw-r--r--   0        0        0     4519 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml
--rw-r--r--   0        0        0    22340 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml
--rw-r--r--   0        0        0     1117 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json
--rw-r--r--   0        0        0     1324 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml
--rw-r--r--   0        0        0     7703 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json
--rw-r--r--   0        0        0    11757 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml
--rw-r--r--   0        0        0      473 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.json
--rw-r--r--   0        0        0     1270 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml
--rw-r--r--   0        0        0      467 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-id-1.5.json
--rw-r--r--   0        0        0     1236 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml
--rw-r--r--   0        0        0     1539 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json
--rw-r--r--   0        0        0     2197 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml
--rw-r--r--   0        0        0      477 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-name-1.5.json
--rw-r--r--   0        0        0     1248 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml
--rw-r--r--   0        0        0    98548 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json
--rw-r--r--   0        0        0   100112 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml
--rw-r--r--   0        0        0      333 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.json
--rw-r--r--   0        0        0      430 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.xml
--rw-r--r--   0        0        0      279 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.json
--rw-r--r--   0        0        0      321 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      436 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.json
--rw-r--r--   0        0        0      624 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml
--rw-r--r--   0        0        0      507 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.json
--rw-r--r--   0        0        0      537 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml
--rw-r--r--   0        0        0      482 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.json
--rw-r--r--   0        0        0      509 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.xml
--rw-r--r--   0        0        0      224 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      254 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0     1162 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json
--rw-r--r--   0        0        0     1471 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml
--rw-r--r--   0        0        0      605 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json
--rw-r--r--   0        0        0      654 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml
--rw-r--r--   0        0        0      227 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.json
--rw-r--r--   0        0        0      281 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.xml
--rw-r--r--   0        0        0     2465 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.json
--rw-r--r--   0        0        0     3337 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml
--rw-r--r--   0        0        0     1520 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.json
--rw-r--r--   0        0        0     1660 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml
--rw-r--r--   0        0        0    21122 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml
--rw-r--r--   0        0        0     5338 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json
--rw-r--r--   0        0        0     6828 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml
--rw-r--r--   0        0        0     9412 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json
--rw-r--r--   0        0        0    12249 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml
--rw-r--r--   0        0        0     2312 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-1.5.json
--rw-r--r--   0        0        0     2693 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-1.5.xml
--rw-r--r--   0        0        0      419 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.json
--rw-r--r--   0        0        0      495 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.xml
--rw-r--r--   0        0        0     9733 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json
--rw-r--r--   0        0        0    17746 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json
--rw-r--r--   0        0        0    19794 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml
--rw-r--r--   0        0        0    11181 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml
--rw-r--r--   0        0        0      157 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/README.md
--rwxr-xr-x   0        0        0      739 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/fetch.sh
--rw-r--r--   0        0        0      391 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/README.md
--rw-r--r--   0        0        0      579 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin
--rw-r--r--   0        0        0      649 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin
--rw-r--r--   0        0        0     1050 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin
--rw-r--r--   0        0        0     1055 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin
--rw-r--r--   0        0        0     1050 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin
--rw-r--r--   0        0        0     1055 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin
--rw-r--r--   0        0        0     2128 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin
--rw-r--r--   0        0        0     2211 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin
--rw-r--r--   0        0        0     2128 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin
--rw-r--r--   0        0        0     2211 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin
--rw-r--r--   0        0        0      806 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin
--rw-r--r--   0        0        0      949 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin
--rw-r--r--   0        0        0     1835 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.2.json.bin
--rw-r--r--   0        0        0     1806 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin
--rw-r--r--   0        0        0     1835 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.3.json.bin
--rw-r--r--   0        0        0     1806 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin
--rw-r--r--   0        0        0     2808 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.4.json.bin
--rw-r--r--   0        0        0     2877 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin
--rw-r--r--   0        0        0     3460 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.5.json.bin
--rw-r--r--   0        0        0     3525 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.1.xml.bin
--rw-r--r--   0        0        0      944 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.2.json.bin
--rw-r--r--   0        0        0      865 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin
--rw-r--r--   0        0        0      944 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.3.json.bin
--rw-r--r--   0        0        0      865 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin
--rw-r--r--   0        0        0     2085 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.4.json.bin
--rw-r--r--   0        0        0     2072 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin
--rw-r--r--   0        0        0     2085 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.5.json.bin
--rw-r--r--   0        0        0     2072 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.0.xml.bin
--rw-r--r--   0        0        0      496 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.1.xml.bin
--rw-r--r--   0        0        0      893 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.2.json.bin
--rw-r--r--   0        0        0      812 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.2.xml.bin
--rw-r--r--   0        0        0      893 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.3.json.bin
--rw-r--r--   0        0        0      812 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.3.xml.bin
--rw-r--r--   0        0        0     2013 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.4.json.bin
--rw-r--r--   0        0        0     2002 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.4.xml.bin
--rw-r--r--   0        0        0     2013 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.5.json.bin
--rw-r--r--   0        0        0     2002 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.0.xml.bin
--rw-r--r--   0        0        0     4093 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin
--rw-r--r--   0        0        0     4074 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin
--rw-r--r--   0        0        0     4409 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin
--rw-r--r--   0        0        0     4074 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin
--rw-r--r--   0        0        0     4409 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin
--rw-r--r--   0        0        0     5202 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin
--rw-r--r--   0        0        0     5607 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin
--rw-r--r--   0        0        0     5451 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin
--rw-r--r--   0        0        0     5856 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin
--rw-r--r--   0        0        0      749 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin
--rw-r--r--   0        0        0      793 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin
--rw-r--r--   0        0        0     1894 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin
--rw-r--r--   0        0        0     1461 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin
--rw-r--r--   0        0        0     1894 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin
--rw-r--r--   0        0        0     1461 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin
--rw-r--r--   0        0        0     3014 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin
--rw-r--r--   0        0        0     2651 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin
--rw-r--r--   0        0        0     3014 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin
--rw-r--r--   0        0        0     2651 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.xml.bin
--rw-r--r--   0        0        0     2092 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin
--rw-r--r--   0        0        0     2289 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin
--rw-r--r--   0        0        0     2092 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin
--rw-r--r--   0        0        0     2289 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.xml.bin
--rw-r--r--   0        0        0     3282 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin
--rw-r--r--   0        0        0     3686 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin
--rw-r--r--   0        0        0     3282 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin
--rw-r--r--   0        0        0     3686 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.xml.bin
--rw-r--r--   0        0        0     1827 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin
--rw-r--r--   0        0        0     2023 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin
--rw-r--r--   0        0        0     1827 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin
--rw-r--r--   0        0        0     2023 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.xml.bin
--rw-r--r--   0        0        0     2577 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin
--rw-r--r--   0        0        0     2822 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin
--rw-r--r--   0        0        0     2577 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin
--rw-r--r--   0        0        0     2822 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.1.xml.bin
--rw-r--r--   0        0        0     1081 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin
--rw-r--r--   0        0        0     1083 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin
--rw-r--r--   0        0        0     1081 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin
--rw-r--r--   0        0        0     1083 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2201 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin
--rw-r--r--   0        0        0     2273 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2201 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin
--rw-r--r--   0        0        0     2273 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.1.xml.bin
--rw-r--r--   0        0        0      886 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin
--rw-r--r--   0        0        0      821 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin
--rw-r--r--   0        0        0      886 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin
--rw-r--r--   0        0        0      821 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2006 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin
--rw-r--r--   0        0        0     2011 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2006 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin
--rw-r--r--   0        0        0     2011 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.xml.bin
--rw-r--r--   0        0        0     2014 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin
--rw-r--r--   0        0        0     2243 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin
--rw-r--r--   0        0        0     2014 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin
--rw-r--r--   0        0        0     2243 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.xml.bin
--rw-r--r--   0        0        0     2025 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin
--rw-r--r--   0        0        0     2268 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin
--rw-r--r--   0        0        0     2025 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin
--rw-r--r--   0        0        0     2268 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin
--rw-r--r--   0        0        0      596 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin
--rw-r--r--   0        0        0      695 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin
--rw-r--r--   0        0        0     1561 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin
--rw-r--r--   0        0        0     1597 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin
--rw-r--r--   0        0        0     1561 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin
--rw-r--r--   0        0        0     1597 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin
--rw-r--r--   0        0        0     2702 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin
--rw-r--r--   0        0        0     2804 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin
--rw-r--r--   0        0        0     2702 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin
--rw-r--r--   0        0        0     2804 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin
--rw-r--r--   0        0        0      662 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin
--rw-r--r--   0        0        0      678 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin
--rw-r--r--   0        0        0     1385 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin
--rw-r--r--   0        0        0     1402 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin
--rw-r--r--   0        0        0     1385 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin
--rw-r--r--   0        0        0     1402 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin
--rw-r--r--   0        0        0     2526 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin
--rw-r--r--   0        0        0     2609 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin
--rw-r--r--   0        0        0     2526 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin
--rw-r--r--   0        0        0     2609 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.0.xml.bin
--rw-r--r--   0        0        0      847 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin
--rw-r--r--   0        0        0     1085 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin
--rw-r--r--   0        0        0     1163 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin
--rw-r--r--   0        0        0     1085 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin
--rw-r--r--   0        0        0     1163 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin
--rw-r--r--   0        0        0     2205 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin
--rw-r--r--   0        0        0     2353 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin
--rw-r--r--   0        0        0     2205 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin
--rw-r--r--   0        0        0     2353 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.1.xml.bin
--rw-r--r--   0        0        0     8462 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin
--rw-r--r--   0        0        0     8225 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin
--rw-r--r--   0        0        0    10188 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin
--rw-r--r--   0        0        0     9538 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin
--rw-r--r--   0        0        0    13095 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin
--rw-r--r--   0        0        0    12485 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin
--rw-r--r--   0        0        0    13095 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin
--rw-r--r--   0        0        0    12485 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin
--rw-r--r--   0        0        0      329 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin
--rw-r--r--   0        0        0     2028 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin
--rw-r--r--   0        0        0     2102 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin
--rw-r--r--   0        0        0     2028 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin
--rw-r--r--   0        0        0     2102 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin
--rw-r--r--   0        0        0     1199 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin
--rw-r--r--   0        0        0     4993 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin
--rw-r--r--   0        0        0     7591 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin
--rw-r--r--   0        0        0     7350 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin
--rw-r--r--   0        0        0     8790 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin
--rw-r--r--   0        0        0     8247 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin
--rw-r--r--   0        0        0    11697 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin
--rw-r--r--   0        0        0    11194 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin
--rw-r--r--   0        0        0    11697 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin
--rw-r--r--   0        0        0    11194 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin
--rw-r--r--   0        0        0      307 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.0.xml.bin
--rw-r--r--   0        0        0      477 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.1.xml.bin
--rw-r--r--   0        0        0      860 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin
--rw-r--r--   0        0        0      859 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin
--rw-r--r--   0        0        0      860 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin
--rw-r--r--   0        0        0      859 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin
--rw-r--r--   0        0        0     1980 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin
--rw-r--r--   0        0        0     2049 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin
--rw-r--r--   0        0        0     1980 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin
--rw-r--r--   0        0        0     2049 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin
--rw-r--r--   0        0        0      395 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.0.xml.bin
--rw-r--r--   0        0        0      572 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin
--rw-r--r--   0        0        0      952 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin
--rw-r--r--   0        0        0      961 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin
--rw-r--r--   0        0        0      952 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin
--rw-r--r--   0        0        0      961 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin
--rw-r--r--   0        0        0     2093 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin
--rw-r--r--   0        0        0     2168 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin
--rw-r--r--   0        0        0     2093 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin
--rw-r--r--   0        0        0     2168 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin
--rw-r--r--   0        0        0      329 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin
--rw-r--r--   0        0        0     3848 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin
--rw-r--r--   0        0        0     3888 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin
--rw-r--r--   0        0        0     3848 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin
--rw-r--r--   0        0        0     3888 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin
--rw-r--r--   0        0        0      329 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin
--rw-r--r--   0        0        0     5145 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin
--rw-r--r--   0        0        0     5654 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin
--rw-r--r--   0        0        0     5145 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin
--rw-r--r--   0        0        0     5654 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin
--rw-r--r--   0        0        0      448 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin
--rw-r--r--   0        0        0     1056 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin
--rw-r--r--   0        0        0     1071 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin
--rw-r--r--   0        0        0     1243 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin
--rw-r--r--   0        0        0     1214 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin
--rw-r--r--   0        0        0     2384 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin
--rw-r--r--   0        0        0     2421 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin
--rw-r--r--   0        0        0     2384 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin
--rw-r--r--   0        0        0     2421 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin
--rw-r--r--   0        0        0      655 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin
--rw-r--r--   0        0        0      980 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin
--rw-r--r--   0        0        0     1582 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin
--rw-r--r--   0        0        0     1579 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin
--rw-r--r--   0        0        0     1769 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin
--rw-r--r--   0        0        0     1722 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin
--rw-r--r--   0        0        0     2889 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin
--rw-r--r--   0        0        0     2912 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin
--rw-r--r--   0        0        0     2889 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin
--rw-r--r--   0        0        0     2912 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin
--rw-r--r--   0        0        0      654 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin
--rw-r--r--   0        0        0     1045 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin
--rw-r--r--   0        0        0     1562 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin
--rw-r--r--   0        0        0     1749 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin
--rw-r--r--   0        0        0     2890 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin
--rw-r--r--   0        0        0     2890 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin
--rw-r--r--   0        0        0     2927 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.0.xml.bin
--rw-r--r--   0        0        0      431 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.1.xml.bin
--rw-r--r--   0        0        0      629 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin
--rw-r--r--   0        0        0      666 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin
--rw-r--r--   0        0        0      792 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin
--rw-r--r--   0        0        0      797 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin
--rw-r--r--   0        0        0     1933 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin
--rw-r--r--   0        0        0     2004 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin
--rw-r--r--   0        0        0     1933 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin
--rw-r--r--   0        0        0     2004 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin
--rw-r--r--   0        0        0      516 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin
--rw-r--r--   0        0        0      814 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     2131 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin
--rw-r--r--   0        0        0     2058 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     2231 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin
--rw-r--r--   0        0        0     2149 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     3288 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin
--rw-r--r--   0        0        0     3288 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     3288 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin
--rw-r--r--   0        0        0     3288 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin
--rw-r--r--   0        0        0      448 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin
--rw-r--r--   0        0        0     1575 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin
--rw-r--r--   0        0        0     1762 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin
--rw-r--r--   0        0        0     2903 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin
--rw-r--r--   0        0        0     2903 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin
--rw-r--r--   0        0        0     2927 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin
--rw-r--r--   0        0        0      245 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.0.xml.bin
--rw-r--r--   0        0        0      459 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     1475 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin
--rw-r--r--   0        0        0     1382 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     1649 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin
--rw-r--r--   0        0        0     1533 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     2748 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin
--rw-r--r--   0        0        0     2706 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     2748 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin
--rw-r--r--   0        0        0     2706 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.1.xml.bin
--rw-r--r--   0        0        0     3772 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin
--rw-r--r--   0        0        0     3875 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin
--rw-r--r--   0        0        0     4135 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin
--rw-r--r--   0        0        0     4149 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin
--rw-r--r--   0        0        0     7096 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin
--rw-r--r--   0        0        0     7142 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin
--rw-r--r--   0        0        0     7096 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin
--rw-r--r--   0        0        0     7142 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.1.xml.bin
--rw-r--r--   0        0        0     2066 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin
--rw-r--r--   0        0        0     2150 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin
--rw-r--r--   0        0        0     2429 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin
--rw-r--r--   0        0        0     2424 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin
--rw-r--r--   0        0        0     5390 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin
--rw-r--r--   0        0        0     5417 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin
--rw-r--r--   0        0        0     5390 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin
--rw-r--r--   0        0        0     5417 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.1.xml.bin
--rw-r--r--   0        0        0     1030 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin
--rw-r--r--   0        0        0     1040 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin
--rw-r--r--   0        0        0     1030 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin
--rw-r--r--   0        0        0     1040 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin
--rw-r--r--   0        0        0     2171 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin
--rw-r--r--   0        0        0     2247 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin
--rw-r--r--   0        0        0     2171 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin
--rw-r--r--   0        0        0     2247 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin
--rw-r--r--   0        0        0     2957 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/test_component.py
--rw-r--r--   0        0        0     3283 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/test_deserialize_json.py
--rw-r--r--   0        0        0     1764 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/test_deserialize_xml.py
--rw-r--r--   0        0        0    19038 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/test_enums.py
--rw-r--r--   0        0        0     4389 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_factory_license.py
--rw-r--r--   0        0        0    22571 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model.py
--rw-r--r--   0        0        0    13219 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_bom.py
--rw-r--r--   0        0        0     2782 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_bom_ref.py
--rw-r--r--   0        0        0    18544 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_component.py
--rw-r--r--   0        0        0     1793 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_dependency.py
--rw-r--r--   0        0        0     4064 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_issue.py
--rw-r--r--   0        0        0     4295 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_license.py
--rw-r--r--   0        0        0     2758 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_release_note.py
--rw-r--r--   0        0        0     3390 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_service.py
--rw-r--r--   0        0        0    14370 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_vulnerability.py
--rw-r--r--   0        0        0     3154 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_output.py
--rw-r--r--   0        0        0     4335 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_output_json.py
--rw-r--r--   0        0        0     3663 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_output_xml.py
--rw-r--r--   0        0        0     1307 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_real_world_examples.py
--rw-r--r--   0        0        0     2524 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_schema_SchemaVersion.py
--rw-r--r--   0        0        0     1248 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_schema__res.py
--rw-r--r--   0        0        0     2873 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_spdx.py
--rw-r--r--   0        0        0     1977 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_validation.py
--rw-r--r--   0        0        0     4529 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_validation_json.py
--rw-r--r--   0        0        0     3061 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_validation_xml.py
--rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 cyclonedx_python_lib-6.4.4/PKG-INFO
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

### Comparing `cyclonedx_python_lib-6.4.4/CHANGELOG.md` & `cyclonedx_python_lib-7.0.0a1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,103 @@
 # CHANGELOG
 
 
 
+## v6.4.4 (2024-03-18)
+
+### Chore
+
+* chore(deps-dev): update coverage requirement from 7.4.3 to 7.4.4 (#570)
+
+Updates the requirements on [coverage](https://github.com/nedbat/coveragepy) to permit the latest version.
+- [Release notes](https://github.com/nedbat/coveragepy/releases)
+- [Changelog](https://github.com/nedbat/coveragepy/blob/master/CHANGES.rst)
+- [Commits](https://github.com/nedbat/coveragepy/compare/7.4.3...7.4.4)
+
+---
+updated-dependencies:
+- dependency-name: coverage
+  dependency-type: direct:development
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
+Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`3a2e427`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/3a2e427ba9967f11c15cd1a47c59a933b699c87b))
+
+* chore(deps): bump python-semantic-release/python-semantic-release (#564)
+
+Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 8.5.1 to 9.1.1.
+- [Release notes](https://github.com/python-semantic-release/python-semantic-release/releases)
+- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/python-semantic-release/python-semantic-release/compare/v8.5.1...v9.1.1)
+
+---
+updated-dependencies:
+- dependency-name: python-semantic-release/python-semantic-release
+  dependency-type: direct:production
+  update-type: version-update:semver-major
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
+Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`d20a590`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/d20a5902582facab0636e9ff8a261edcaf886a3e))
+
+* chore(deps-dev): update tox requirement from 4.13.0 to 4.14.1 (#567)
+
+Updates the requirements on [tox](https://github.com/tox-dev/tox) to permit the latest version.
+- [Release notes](https://github.com/tox-dev/tox/releases)
+- [Changelog](https://github.com/tox-dev/tox/blob/main/docs/changelog.rst)
+- [Commits](https://github.com/tox-dev/tox/compare/4.13.0...4.14.1)
+
+---
+updated-dependencies:
+- dependency-name: tox
+  dependency-type: direct:development
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
+Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`2dcc60e`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/2dcc60e53ec66d642c728596ff25fed4df5659a0))
+
+* chore(deps-dev): update bandit requirement from 1.7.7 to 1.7.8 (#566)
+
+Updates the requirements on [bandit](https://github.com/PyCQA/bandit) to permit the latest version.
+- [Release notes](https://github.com/PyCQA/bandit/releases)
+- [Commits](https://github.com/PyCQA/bandit/compare/1.7.7...1.7.8)
+
+---
+updated-dependencies:
+- dependency-name: bandit
+  dependency-type: direct:development
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
+Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`eb1a252`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/eb1a2525c09e0dd10f11ff83b451a4db4fb00d9b))
+
+* chore(deps-dev): update mypy requirement from 1.8.0 to 1.9.0 (#565)
+
+Updates the requirements on [mypy](https://github.com/python/mypy) to permit the latest version.
+- [Changelog](https://github.com/python/mypy/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/python/mypy/compare/v1.8.0...1.9.0)
+
+---
+updated-dependencies:
+- dependency-name: mypy
+  dependency-type: direct:development
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
+Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`3ce0f3a`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/3ce0f3a373d9f1b07af50d9b707f766ea446e518))
+
+### Fix
+
+* fix: wrong extra name for xml validation (#571)
+
+
+
+Signed-off-by: Christoph Reiter &lt;reiter.christoph@gmail.com&gt; ([`10e38e2`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/10e38e25095de4b2dafbfcd1fd81dce7a9c0f124))
+
+
 ## v6.4.3 (2024-03-04)
 
 ### Chore
 
 * chore(deps-dev): update ddt requirement from 1.7.1 to 1.7.2 (#563)
 
 Updates the requirements on [ddt](https://github.com/datadriventests/ddt) to permit the latest version.
@@ -1497,40 +1589,15 @@
 
 Signed-off-by: Michael Schlenker &lt;michael.schlenker@contact-software.com&gt;
 Co-authored-by: Michael Schlenker &lt;michael.schlenker@contact-software.com&gt; ([`dad0d28`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/dad0d28ceb7381d1b503e5b29776fc01513f8b04))
 
 
 ## v4.0.0 (2023-03-20)
 
-### Chore
-
-* chore(deps): bump relekang/python-semantic-release from 7.31.2 to 7.33.1 (#345)
-
-Bumps [relekang/python-semantic-release](https://github.com/relekang/python-semantic-release) from 7.31.2 to 7.33.1.
-- [Release notes](https://github.com/relekang/python-semantic-release/releases)
-- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
-- [Commits](https://github.com/relekang/python-semantic-release/compare/v7.31.2...v7.33.1)
-
----
-updated-dependencies:
-- dependency-name: relekang/python-semantic-release
-  dependency-type: direct:production
-  update-type: version-update:semver-minor
-...
-
-Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
-Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`a011d89`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/a011d89ce6cee9e56bcfcc9a9338fa1e559721f7))
-
-* chore: package manifest fix link to homepage and documentation (#291)
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt;
-
-Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`f2350b4`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/f2350b4e2b0fb7668ca987e523c53acb6ac6fefb))
-
-### Feature
+### Breaking
 
 * feat: Release 4.0.0 #341)
 
 Highlights of this release include:
 * Support for De-serialization from JSON and XML to this Pythonic Model
 * Deprecation of Python 3.6 support
 * Support for Python 3.11
@@ -1644,14 +1711,39 @@
 Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt;
 Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt;
 Signed-off-by: Hakan Dilek &lt;hakandilek@gmail.com&gt;
 Co-authored-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt;
 Co-authored-by: Hakan Dilek &lt;hakandilek@gmail.com&gt;
 Co-authored-by: Hakan Dilek &lt;hakandilek@users.noreply.github.com&gt; ([`8fb1b14`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/8fb1b14f5e04e85f21e654c44fa6b9b774867757))
 
+### Chore
+
+* chore(deps): bump relekang/python-semantic-release from 7.31.2 to 7.33.1 (#345)
+
+Bumps [relekang/python-semantic-release](https://github.com/relekang/python-semantic-release) from 7.31.2 to 7.33.1.
+- [Release notes](https://github.com/relekang/python-semantic-release/releases)
+- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/relekang/python-semantic-release/compare/v7.31.2...v7.33.1)
+
+---
+updated-dependencies:
+- dependency-name: relekang/python-semantic-release
+  dependency-type: direct:production
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
+Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`a011d89`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/a011d89ce6cee9e56bcfcc9a9338fa1e559721f7))
+
+* chore: package manifest fix link to homepage and documentation (#291)
+
+Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt;
+
+Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`f2350b4`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/f2350b4e2b0fb7668ca987e523c53acb6ac6fefb))
+
 ### Unknown
 
 * 4.0.0
 
 Automatically generated by python-semantic-release ([`40fbfda`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/40fbfda428cfa71b16fd6e5e8d5f49cea4b5438b))
```

### Comparing `cyclonedx_python_lib-6.4.4/LICENSE` & `cyclonedx_python_lib-7.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/README.md` & `cyclonedx_python_lib-7.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
 """
 Python library for CycloneDX
 """
 
 # !! version is managed by semantic_release
 # do not use typing here, or else `semantic_release` might have issues finding the variable
-__version__ = "6.4.4"  # noqa:Q000
+__version__ = "7.0.0-alpha.1"  # noqa:Q000
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/_internal/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/_internal/compare.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/compare.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/_internal/hash.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/hash.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/_internal/time.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/_internal/time.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/exception/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/exception/factory.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/factory.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/exception/model.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -41,14 +41,46 @@
 
     The language code MUST be lowercase. If the country code is specified, the country code MUST be upper case.
     The language code and country code MUST be separated by a minus sign.
     """
     pass
 
 
+class InvalidNistQuantumSecurityLevelException(CycloneDxModelException):
+    """
+    Raised when an invalid value is provided for an NIST Quantum Security Level
+    as defined at https://csrc.nist.gov/projects/post-quantum-cryptography/post-quantum-cryptography-standardization/
+    evaluation-criteria/security-(evaluation-criteria).
+    """
+    pass
+
+
+class InvalidOmniBorIdException(CycloneDxModelException):
+    """
+    Raised when a supplied value for an OmniBOR ID does not meet the format requirements
+    as defined at https://www.iana.org/assignments/uri-schemes/prov/gitoid.
+    """
+    pass
+
+
+class InvalidRelatedCryptoMaterialSizeException(CycloneDxModelException):
+    """
+    Raised when the supplied size of a Related Crypto Material is negative.
+    """
+    pass
+
+
+class InvalidSwhidException(CycloneDxModelException):
+    """
+    Raised when a supplied value for an Swhid does not meet the format requirements
+    as defined at https://docs.softwareheritage.org/devel/swh-model/persistent-identifiers.html.
+    """
+    pass
+
+
 class InvalidUriException(CycloneDxModelException):
     """
     Raised when a `str` is provided that needs to be a valid URI, but isn't.
     """
     pass
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/exception/output.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/exception/serialization.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/exception/serialization.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/factory/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/factory/license.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/factory/license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from ..schema.schema import (
     SchemaVersion1Dot0,
     SchemaVersion1Dot1,
     SchemaVersion1Dot2,
     SchemaVersion1Dot3,
     SchemaVersion1Dot4,
     SchemaVersion1Dot5,
+    SchemaVersion1Dot6,
 )
 
 
 @serializable.serializable_enum
 class DataFlow(str, Enum):
     """
     This is our internal representation of the dataFlowType simple type within the CycloneDX standard.
@@ -283,14 +284,15 @@
         HashAlgorithm.BLAKE2B_512,
         HashAlgorithm.BLAKE3,
         HashAlgorithm.SHA3_384,
     }
     __CASES[SchemaVersion1Dot3] = __CASES[SchemaVersion1Dot2]
     __CASES[SchemaVersion1Dot4] = __CASES[SchemaVersion1Dot3]
     __CASES[SchemaVersion1Dot5] = __CASES[SchemaVersion1Dot4]
+    __CASES[SchemaVersion1Dot6] = __CASES[SchemaVersion1Dot5]
 
     @classmethod
     def __prep(cls, hts: Iterable['HashType'], view: Type[serializable.ViewType]) -> Generator['HashType', None, None]:
         cases = cls.__CASES.get(view, ())
         for ht in hts:
             if ht.alg in cases:
                 yield ht
@@ -504,36 +506,40 @@
     BUILD_META = 'build-meta'
     BUILD_SYSTEM = 'build-system'
     CERTIFICATION_REPORT = 'certification-report'  # Only supported in >= 1.5
     CHAT = 'chat'
     CODIFIED_INFRASTRUCTURE = 'codified-infrastructure'  # Only supported in >= 1.5
     COMPONENT_ANALYSIS_REPORT = 'component-analysis-report'  # Only supported in >= 1.5
     CONFIGURATION = 'configuration'  # Only supported in >= 1.5
+    DIGITAL_SIGNATURE = 'digital-signature'  # Only supported in >= 1.6
     DISTRIBUTION = 'distribution'
     DISTRIBUTION_INTAKE = 'distribution-intake'  # Only supported in >= 1.5
     DOCUMENTATION = 'documentation'
     DYNAMIC_ANALYSIS_REPORT = 'dynamic-analysis-report'  # Only supported in >= 1.5
+    ELECTRONIC_SIGNATURE = 'electronic-signature'  # Only supported in >= 1.6
     EVIDENCE = 'evidence'  # Only supported in >= 1.5
     EXPLOITABILITY_STATEMENT = 'exploitability-statement'  # Only supported in >= 1.5
     FORMULATION = 'formulation'  # Only supported in >= 1.5
     ISSUE_TRACKER = 'issue-tracker'
     LICENSE = 'license'
     LOG = 'log'  # Only supported in >= 1.5
     MAILING_LIST = 'mailing-list'
     MATURITY_REPORT = 'maturity-report'  # Only supported in >= 1.5
     MODEL_CARD = 'model-card'  # Only supported in >= 1.5
     PENTEST_REPORT = 'pentest-report'  # Only supported in >= 1.5
     POAM = 'poam'  # Only supported in >= 1.5
     QUALITY_METRICS = 'quality-metrics'  # Only supported in >= 1.5
     RELEASE_NOTES = 'release-notes'  # Only supported in >= 1.4
+    RFC_9166 = 'rfc-9116'  # Only supported in >= 1.6
     RISK_ASSESSMENT = 'risk-assessment'  # Only supported in >= 1.5
     RUNTIME_ANALYSIS_REPORT = 'runtime-analysis-report'  # Only supported in >= 1.5
     SECURITY_CONTACT = 'security-contact'  # Only supported in >= 1.5
     STATIC_ANALYSIS_REPORT = 'static-analysis-report'  # Only supported in >= 1.5
     SOCIAL = 'social'
+    SOURCE_DISTRIBUTION = 'source-distribution'  # Only supported in >= 1.6
     SCM = 'vcs'
     SUPPORT = 'support'
     THREAT_MODEL = 'threat-model'  # Only supported in >= 1.5
     VCS = 'vcs'
     VULNERABILITY_ASSERTION = 'vulnerability-assertion'  # Only supported in >= 1.5
     WEBSITE = 'website'
     # --
@@ -587,14 +593,20 @@
         ExternalReferenceType.COMPONENT_ANALYSIS_REPORT,
         ExternalReferenceType.MATURITY_REPORT,
         ExternalReferenceType.CERTIFICATION_REPORT,
         ExternalReferenceType.QUALITY_METRICS,
         ExternalReferenceType.CODIFIED_INFRASTRUCTURE,
         ExternalReferenceType.POAM,
     }
+    __CASES[SchemaVersion1Dot6] = __CASES[SchemaVersion1Dot5] | {
+        ExternalReferenceType.SOURCE_DISTRIBUTION,
+        ExternalReferenceType.ELECTRONIC_SIGNATURE,
+        ExternalReferenceType.DIGITAL_SIGNATURE,
+        ExternalReferenceType.RFC_9166,
+    }
 
     @classmethod
     def __normalize(cls, extref: ExternalReferenceType, view: Type[serializable.ViewType]) -> str:
         return (
             extref
             if extref in cls.__CASES.get(view, ())
             else ExternalReferenceType.OTHER
@@ -778,14 +790,15 @@
     def type(self, type: ExternalReferenceType) -> None:
         self._type = type
 
     @property
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.type_mapping(_HashTypeRepositorySerializationHelper)
     def hashes(self) -> 'SortedSet[HashType]':
         """
         The hashes of the external reference (if applicable).
 
         Returns:
             Set of `HashType`
@@ -1053,185 +1066,14 @@
         return hash((self.text, self.locale))
 
     def __repr__(self) -> str:
         return f'<Note id={id(self)}, locale={self.locale}>'
 
 
 @serializable.serializable_class
-class OrganizationalContact:
-    """
-    This is our internal representation of the `organizationalContact` complex type that can be used in multiple places
-    within a CycloneDX BOM document.
-
-    .. note::
-        See the CycloneDX Schema definition: https://cyclonedx.org/docs/1.4/xml/#type_organizationalContact
-    """
-
-    def __init__(self, *, name: Optional[str] = None, phone: Optional[str] = None, email: Optional[str] = None) -> None:
-        if not name and not phone and not email:
-            raise NoPropertiesProvidedException(
-                'One of name, email or phone must be supplied for an OrganizationalContact - none supplied.'
-            )
-        self.name = name
-        self.email = email
-        self.phone = phone
-
-    @property
-    @serializable.xml_sequence(1)
-    def name(self) -> Optional[str]:
-        """
-        Get the name of the contact.
-
-        Returns:
-            `str` if set else `None`
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name: Optional[str]) -> None:
-        self._name = name
-
-    @property
-    @serializable.xml_sequence(2)
-    def email(self) -> Optional[str]:
-        """
-        Get the email of the contact.
-
-        Returns:
-            `str` if set else `None`
-        """
-        return self._email
-
-    @email.setter
-    def email(self, email: Optional[str]) -> None:
-        self._email = email
-
-    @property
-    @serializable.xml_sequence(3)
-    def phone(self) -> Optional[str]:
-        """
-        Get the phone of the contact.
-
-        Returns:
-            `str` if set else `None`
-        """
-        return self._phone
-
-    @phone.setter
-    def phone(self, phone: Optional[str]) -> None:
-        self._phone = phone
-
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, OrganizationalContact):
-            return hash(other) == hash(self)
-        return False
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, OrganizationalContact):
-            return _ComparableTuple((
-                self.name, self.email, self.phone
-            )) < _ComparableTuple((
-                other.name, other.email, other.phone
-            ))
-        return NotImplemented
-
-    def __hash__(self) -> int:
-        return hash((self.name, self.phone, self.email))
-
-    def __repr__(self) -> str:
-        return f'<OrganizationalContact name={self.name}, email={self.email}, phone={self.phone}>'
-
-
-@serializable.serializable_class
-class OrganizationalEntity:
-    """
-    This is our internal representation of the `organizationalEntity` complex type that can be used in multiple places
-    within a CycloneDX BOM document.
-
-    .. note::
-        See the CycloneDX Schema definition: https://cyclonedx.org/docs/1.4/xml/#type_organizationalEntity
-    """
-
-    def __init__(self, *, name: Optional[str] = None, urls: Optional[Iterable[XsUri]] = None,
-                 contacts: Optional[Iterable[OrganizationalContact]] = None) -> None:
-        if not name and not urls and not contacts:
-            raise NoPropertiesProvidedException(
-                'One of name, urls or contacts must be supplied for an OrganizationalEntity - none supplied.'
-            )
-        self.name = name
-        self.urls = urls or []  # type:ignore[assignment]
-        self.contacts = contacts or []  # type:ignore[assignment]
-
-    @property
-    @serializable.xml_sequence(1)
-    def name(self) -> Optional[str]:
-        """
-        Get the name of the organization.
-
-        Returns:
-            `str` if set else `None`
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name: Optional[str]) -> None:
-        self._name = name
-
-    @property
-    @serializable.json_name('url')
-    @serializable.xml_array(serializable.XmlArraySerializationType.FLAT, 'url')
-    @serializable.xml_sequence(2)
-    def urls(self) -> 'SortedSet[XsUri]':
-        """
-        Get a list of URLs of the organization. Multiple URLs are allowed.
-
-        Returns:
-            Set of `XsUri`
-        """
-        return self._urls
-
-    @urls.setter
-    def urls(self, urls: Iterable[XsUri]) -> None:
-        self._urls = SortedSet(urls)
-
-    @property
-    @serializable.json_name('contact')
-    @serializable.xml_array(serializable.XmlArraySerializationType.FLAT, 'contact')
-    @serializable.xml_sequence(3)
-    def contacts(self) -> 'SortedSet[OrganizationalContact]':
-        """
-        Get a list of contact person at the organization. Multiple contacts are allowed.
-
-        Returns:
-            Set of `OrganizationalContact`
-        """
-        return self._contacts
-
-    @contacts.setter
-    def contacts(self, contacts: Iterable[OrganizationalContact]) -> None:
-        self._contacts = SortedSet(contacts)
-
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, OrganizationalEntity):
-            return hash(other) == hash(self)
-        return False
-
-    def __lt__(self, other: Any) -> bool:
-        if isinstance(other, OrganizationalEntity):
-            return hash(self) < hash(other)
-        return NotImplemented
-
-    def __hash__(self) -> int:
-        return hash((self.name, tuple(self.urls), tuple(self.contacts)))
-
-    def __repr__(self) -> str:
-        return f'<OrganizationalEntity name={self.name}>'
-
-
-@serializable.serializable_class
 class Tool:
     """
     This is our internal representation of the `toolType` complex type within the CycloneDX standard.
 
     Tool(s) are the things used in the creation of the CycloneDX document.
 
     Tool might be deprecated since CycloneDX 1.5, but it is not deprecated in this library.
@@ -1310,19 +1152,20 @@
     @hashes.setter
     def hashes(self, hashes: Iterable[HashType]) -> None:
         self._hashes = SortedSet(hashes)
 
     @property
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'reference')
     @serializable.xml_sequence(5)
     def external_references(self) -> 'SortedSet[ExternalReference]':
         """
-        External References provide a way to document systems, sites, and information that may be relevant but which
+        External References provides a way to document systems, sites, and information that may be relevant but which
         are not included with the BOM.
 
         Returns:
             Set of `ExternalReference`
         """
         return self._external_references
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/bom.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/bom.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 from ..schema.schema import (
     SchemaVersion1Dot0,
     SchemaVersion1Dot1,
     SchemaVersion1Dot2,
     SchemaVersion1Dot3,
     SchemaVersion1Dot4,
     SchemaVersion1Dot5,
+    SchemaVersion1Dot6,
 )
 from ..serialization import LicenseRepositoryHelper, UrnUuidHelper
-from . import ExternalReference, OrganizationalContact, OrganizationalEntity, Property, ThisTool, Tool
+from . import ExternalReference, Property, ThisTool, Tool
 from .bom_ref import BomRef
 from .component import Component
+from .contact import OrganizationalContact, OrganizationalEntity
 from .dependency import Dependable, Dependency
 from .license import License, LicenseExpression, LicenseRepository
 from .service import Service
 from .vulnerability import Vulnerability
 
 if TYPE_CHECKING:  # pragma: no cover
     from packageurl import PackageURL
@@ -55,27 +57,36 @@
 
     .. note::
         See the CycloneDX Schema for Bom metadata: https://cyclonedx.org/docs/1.5/#type_metadata
     """
 
     def __init__(self, *, tools: Optional[Iterable[Tool]] = None,
                  authors: Optional[Iterable[OrganizationalContact]] = None, component: Optional[Component] = None,
-                 manufacture: Optional[OrganizationalEntity] = None,
                  supplier: Optional[OrganizationalEntity] = None,
                  licenses: Optional[Iterable[License]] = None,
                  properties: Optional[Iterable[Property]] = None,
-                 timestamp: Optional[datetime] = None) -> None:
+                 timestamp: Optional[datetime] = None,
+                 manufacturer: Optional[OrganizationalEntity] = None,
+                 # Deprecated as of v1.6
+                 manufacture: Optional[OrganizationalEntity] = None) -> None:
         self.timestamp = timestamp or _get_now_utc()
         self.tools = tools or []  # type:ignore[assignment]
         self.authors = authors or []  # type:ignore[assignment]
         self.component = component
-        self.manufacture = manufacture
         self.supplier = supplier
         self.licenses = licenses or []  # type:ignore[assignment]
         self.properties = properties or []  # type:ignore[assignment]
+        self.manufacturer = manufacturer
+
+        self.manufacture = manufacture
+        if manufacture:
+            warn(
+                '`bom.metadata.manufacture` is deprecated from CycloneDX v1.6 onwards. '
+                'Please use `bom.metadata.component.manufacturer` instead.',
+                DeprecationWarning)
 
         if not tools:
             self.tools.add(ThisTool)
 
     @property
     @serializable.type_mapping(serializable.helpers.XsdDateTime)
     @serializable.xml_sequence(1)
@@ -163,30 +174,57 @@
 
         Returns:
             None
         """
         self._component = component
 
     @property
+    @serializable.view(SchemaVersion1Dot2)
+    @serializable.view(SchemaVersion1Dot3)
+    @serializable.view(SchemaVersion1Dot4)
+    @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_sequence(6)
     def manufacture(self) -> Optional[OrganizationalEntity]:
         """
         The organization that manufactured the component that the BOM describes.
 
         Returns:
             `OrganizationalEntity` if set else `None`
         """
         return self._manufacture
 
     @manufacture.setter
     def manufacture(self, manufacture: Optional[OrganizationalEntity]) -> None:
+        """
+        @todo Based on https://github.com/CycloneDX/specification/issues/346,
+              we should set this data on `.component.manufacturer`.
+        """
         self._manufacture = manufacture
 
     @property
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_sequence(7)
+    def manufacturer(self) -> Optional[OrganizationalEntity]:
+        """
+        The organization that created the BOM.
+        Manufacturer is common in BOMs created through automated processes. BOMs created through manual means may have
+        `@.authors` instead.
+
+        Returns:
+            `OrganizationalEntity` if set else `None`
+        """
+        return self._manufacturer
+
+    @manufacturer.setter
+    def manufacturer(self, manufacturer: Optional[OrganizationalEntity]) -> None:
+        self._manufacturer = manufacturer
+
+    @property
+    @serializable.xml_sequence(8)
     def supplier(self) -> Optional[OrganizationalEntity]:
         """
         The organization that supplied the component that the BOM describes.
 
         The supplier may often be the manufacturer, but may also be a distributor or repackager.
 
         Returns:
@@ -198,16 +236,17 @@
     def supplier(self, supplier: Optional[OrganizationalEntity]) -> None:
         self._supplier = supplier
 
     @property
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.type_mapping(LicenseRepositoryHelper)
-    @serializable.xml_sequence(8)
+    @serializable.xml_sequence(9)
     def licenses(self) -> LicenseRepository:
         """
         A optional list of statements about how this BOM is licensed.
 
         Returns:
             Set of `LicenseChoice`
         """
@@ -217,16 +256,17 @@
     def licenses(self, licenses: Iterable[License]) -> None:
         self._licenses = LicenseRepository(licenses)
 
     @property
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'property')
-    @serializable.xml_sequence(9)
+    @serializable.xml_sequence(10)
     def properties(self) -> 'SortedSet[Property]':
         """
         Provides the ability to document properties in a key/value store. This provides flexibility to include data not
         officially supported in the standard without having to use additional namespaces or create extensions.
 
         Property names of interest to the general public are encouraged to be registered in the CycloneDX Property
         Taxonomy - https://github.com/CycloneDX/cyclonedx-property-taxonomy. Formal registration is OPTIONAL.
@@ -244,15 +284,15 @@
         if isinstance(other, BomMetaData):
             return hash(other) == hash(self)
         return False
 
     def __hash__(self) -> int:
         return hash((
             tuple(self.authors), self.component, tuple(self.licenses), self.manufacture, tuple(self.properties),
-            self.supplier, self.timestamp, tuple(self.tools)
+            self.supplier, self.timestamp, tuple(self.tools), self.manufacturer,
         ))
 
     def __repr__(self) -> str:
         return f'<BomMetaData timestamp={self.timestamp}, component={self.component}>'
 
 
 @serializable.serializable_class(ignore_during_deserialization=['$schema', 'bom_format', 'spec_version'])
@@ -289,14 +329,15 @@
     @property
     @serializable.type_mapping(UrnUuidHelper)
     @serializable.view(SchemaVersion1Dot1)
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_attribute()
     def serial_number(self) -> UUID:
         """
         Unique UUID for this BOM
 
         Returns:
             `UUID` instance
@@ -318,14 +359,15 @@
         self._version = version
 
     @property
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_sequence(1)
     def metadata(self) -> BomMetaData:
         """
         Get our internal metadata object for this Bom.
 
         Returns:
             Metadata object instance for this Bom.
@@ -358,14 +400,15 @@
         self._components = SortedSet(components)
 
     @property
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'service')
     @serializable.xml_sequence(3)
     def services(self) -> 'SortedSet[Service]':
         """
         Get all the Services currently in this Bom.
 
         Returns:
@@ -379,14 +422,15 @@
 
     @property
     @serializable.view(SchemaVersion1Dot1)
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'reference')
     @serializable.xml_sequence(4)
     def external_references(self) -> 'SortedSet[ExternalReference]':
         """
         Provides the ability to document external references related to the BOM or to the project the BOM describes.
 
         Returns:
@@ -399,14 +443,15 @@
         self._external_references = SortedSet(external_references)
 
     @property
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'dependency')
     @serializable.xml_sequence(5)
     def dependencies(self) -> 'SortedSet[Dependency]':
         return self._dependencies
 
     @dependencies.setter
     def dependencies(self, dependencies: Iterable[Dependency]) -> None:
@@ -437,14 +482,15 @@
     # @properties.setter
     # def properties(self, ...) -> None:
     #     ...  # TODO Since CDX 1.3
 
     @property
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'vulnerability')
     @serializable.xml_sequence(8)
     def vulnerabilities(self) -> 'SortedSet[Vulnerability]':
         """
         Get all the Vulnerabilities in this BOM.
 
         Returns:
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/bom_ref.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/component.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/component.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,51 +10,57 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright (c) OWASP Foundation. All Rights Reserved.
-
-
+import re
 from enum import Enum
 from os.path import exists
 from typing import Any, Dict, FrozenSet, Iterable, Optional, Set, Type, Union
+from warnings import warn
 
 # See https://github.com/package-url/packageurl-python/issues/65
 import serializable
 from packageurl import PackageURL
 from sortedcontainers import SortedSet
 
 from .._internal.compare import ComparableTuple as _ComparableTuple
 from .._internal.hash import file_sha1sum as _file_sha1sum
-from ..exception.model import NoPropertiesProvidedException
-from ..exception.serialization import SerializationOfUnsupportedComponentTypeException
+from ..exception.model import InvalidOmniBorIdException, InvalidSwhidException, NoPropertiesProvidedException
+from ..exception.serialization import (
+    CycloneDxDeserializationException,
+    SerializationOfUnexpectedValueException,
+    SerializationOfUnsupportedComponentTypeException,
+)
 from ..schema.schema import (
     SchemaVersion1Dot0,
     SchemaVersion1Dot1,
     SchemaVersion1Dot2,
     SchemaVersion1Dot3,
     SchemaVersion1Dot4,
     SchemaVersion1Dot5,
+    SchemaVersion1Dot6,
 )
 from ..serialization import BomRefHelper, LicenseRepositoryHelper, PackageUrl
 from . import (
     AttachedText,
     Copyright,
     ExternalReference,
     HashAlgorithm,
     HashType,
     IdentifiableAction,
-    OrganizationalEntity,
     Property,
     XsUri,
     _HashTypeRepositorySerializationHelper,
 )
 from .bom_ref import BomRef
+from .contact import OrganizationalContact, OrganizationalEntity
+from .crypto import CryptoProperties
 from .dependency import Dependable
 from .issue import IssueType
 from .license import License, LicenseRepository
 from .release_note import ReleaseNotes
 
 
 @serializable.serializable_class
@@ -300,14 +306,15 @@
     __CASES[SchemaVersion1Dot1] = __CASES[SchemaVersion1Dot0] | {
         ComponentScope.EXCLUDED,
     }
     __CASES[SchemaVersion1Dot2] = __CASES[SchemaVersion1Dot1]
     __CASES[SchemaVersion1Dot3] = __CASES[SchemaVersion1Dot2]
     __CASES[SchemaVersion1Dot4] = __CASES[SchemaVersion1Dot3]
     __CASES[SchemaVersion1Dot5] = __CASES[SchemaVersion1Dot4]
+    __CASES[SchemaVersion1Dot6] = __CASES[SchemaVersion1Dot5]
 
     @classmethod
     def __normalize(cls, cs: ComponentScope, view: Type[serializable.ViewType]) -> Optional[str]:
         return cs.value \
             if cs in cls.__CASES.get(view, ()) \
             else None
 
@@ -337,14 +344,15 @@
 
     .. note::
         See the CycloneDX Schema definition: https://cyclonedx.org/docs/1.3/#type_classification
     """
     # see `_ComponentTypeSerializationHelper.__CASES` for view/case map
     APPLICATION = 'application'
     CONTAINER = 'container'  # Only supported in >= 1.2
+    CRYPTOGRAPHIC_ASSET = 'cryptographic-asset'  # Only supported in >= 1.6
     DATA = 'data'  # Only supported in >= 1.5
     DEVICE = 'device'
     DEVICE_DRIVER = 'device-driver'  # Only supported in >= 1.5
     FILE = 'file'  # Only supported in >= 1.1
     FIRMWARE = 'firmware'  # Only supported in >= 1.2
     FRAMEWORK = 'framework'
     LIBRARY = 'library'
@@ -375,14 +383,17 @@
     __CASES[SchemaVersion1Dot4] = __CASES[SchemaVersion1Dot3]
     __CASES[SchemaVersion1Dot5] = __CASES[SchemaVersion1Dot4] | {
         ComponentType.DATA,
         ComponentType.DEVICE_DRIVER,
         ComponentType.MACHINE_LEARNING_MODEL,
         ComponentType.PLATFORM,
     }
+    __CASES[SchemaVersion1Dot6] = __CASES[SchemaVersion1Dot5] | {
+        ComponentType.CRYPTOGRAPHIC_ASSET,
+    }
 
     @classmethod
     def __normalize(cls, ct: ComponentType, view: Type[serializable.ViewType]) -> Optional[str]:
         if ct in cls.__CASES.get(view, ()):
             return ct.value
         raise SerializationOfUnsupportedComponentTypeException(f'unsupported {ct!r} for view {view!r}')
 
@@ -676,14 +687,15 @@
         self._commits = SortedSet(commits)
 
     @property
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'patch')
     @serializable.xml_sequence(5)
     def patches(self) -> 'SortedSet[Patch]':
         """
         A list of zero or more patches describing how the component deviates from an ancestor, descendant, or variant.
         Patches may be complimentary to commits or may be used in place of commits.
 
@@ -858,14 +870,132 @@
         return hash((self.tag_id, self.name, self.version, self.tag_version, self.patch, self.text, self.url))
 
     def __repr__(self) -> str:
         return f'<Swid tagId={self.tag_id}, name={self.name}, version={self.version}>'
 
 
 @serializable.serializable_class
+class OmniborId(serializable.helpers.BaseHelper):
+    """
+    Helper class that allows us to perform validation on data strings that must conform to
+    https://www.iana.org/assignments/uri-schemes/prov/gitoid.
+
+    """
+
+    _VALID_OMNIBOR_ID_REGEX = re.compile(r'^gitoid:(blob|tree|commit|tag):sha(1|256):([a-z0-9]+)$')
+
+    def __init__(self, id: str) -> None:
+        if OmniborId._VALID_OMNIBOR_ID_REGEX.match(id) is None:
+            raise InvalidOmniBorIdException(
+                f'Supplied value "{id} does not meet format specification.'
+            )
+        self._id = id
+
+    @property
+    @serializable.json_name('.')
+    @serializable.xml_name('.')
+    def id(self) -> str:
+        return self._id
+
+    @classmethod
+    def serialize(cls, o: Any) -> str:
+        if isinstance(o, OmniborId):
+            return str(o)
+        raise SerializationOfUnexpectedValueException(
+            f'Attempt to serialize a non-OmniBorId: {o!r}')
+
+    @classmethod
+    def deserialize(cls, o: Any) -> 'OmniborId':
+        try:
+            return OmniborId(id=str(o))
+        except ValueError as err:
+            raise CycloneDxDeserializationException(
+                f'OmniBorId string supplied does not parse: {o!r}'
+            ) from err
+
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, OmniborId):
+            return hash(other) == hash(self)
+        return False
+
+    def __lt__(self, other: Any) -> bool:
+        if isinstance(other, OmniborId):
+            return self._id < other._id
+        return NotImplemented
+
+    def __hash__(self) -> int:
+        return hash(self._id)
+
+    def __repr__(self) -> str:
+        return f'<OmniBorId {self._id}>'
+
+    def __str__(self) -> str:
+        return self._id
+
+
+@serializable.serializable_class
+class Swhid(serializable.helpers.BaseHelper):
+    """
+    Helper class that allows us to perform validation on data strings that must conform to
+    https://docs.softwareheritage.org/devel/swh-model/persistent-identifiers.html.
+
+    """
+
+    _VALID_SWHID_REGEX = re.compile(r'^swh:1:(cnp|rel|rev|dir|cnt):([0-9a-z]{40})(.*)?$')
+
+    def __init__(self, id: str) -> None:
+        if Swhid._VALID_SWHID_REGEX.match(id) is None:
+            raise InvalidSwhidException(
+                f'Supplied value "{id} does not meet format specification.'
+            )
+        self._id = id
+
+    @property
+    @serializable.json_name('.')
+    @serializable.xml_name('.')
+    def id(self) -> str:
+        return self._id
+
+    @classmethod
+    def serialize(cls, o: Any) -> str:
+        if isinstance(o, Swhid):
+            return str(o)
+        raise SerializationOfUnexpectedValueException(
+            f'Attempt to serialize a non-Swhid: {o!r}')
+
+    @classmethod
+    def deserialize(cls, o: Any) -> 'Swhid':
+        try:
+            return Swhid(id=str(o))
+        except ValueError as err:
+            raise CycloneDxDeserializationException(
+                f'Swhid string supplied does not parse: {o!r}'
+            ) from err
+
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, Swhid):
+            return hash(other) == hash(self)
+        return False
+
+    def __lt__(self, other: Any) -> bool:
+        if isinstance(other, Swhid):
+            return self._id < other._id
+        return NotImplemented
+
+    def __hash__(self) -> int:
+        return hash(self._id)
+
+    def __repr__(self) -> str:
+        return f'<Swhid {self._id}>'
+
+    def __str__(self) -> str:
+        return self._id
+
+
+@serializable.serializable_class
 class Component(Dependable):
     """
     This is our internal representation of a Component within a Bom.
 
     .. note::
         See the CycloneDX Schema definition: https://cyclonedx.org/docs/1.3/#type_component
     """
@@ -899,52 +1029,70 @@
                 version=f'0.0.0-{sha1_hash[0:12]}'
             )
         )
 
     def __init__(self, *,
                  name: str, type: ComponentType = ComponentType.LIBRARY,
                  mime_type: Optional[str] = None, bom_ref: Optional[Union[str, BomRef]] = None,
-                 supplier: Optional[OrganizationalEntity] = None, author: Optional[str] = None,
+                 supplier: Optional[OrganizationalEntity] = None,
                  publisher: Optional[str] = None, group: Optional[str] = None, version: Optional[str] = None,
                  description: Optional[str] = None, scope: Optional[ComponentScope] = None,
                  hashes: Optional[Iterable[HashType]] = None, licenses: Optional[Iterable[License]] = None,
                  copyright: Optional[str] = None, purl: Optional[PackageURL] = None,
                  external_references: Optional[Iterable[ExternalReference]] = None,
                  properties: Optional[Iterable[Property]] = None, release_notes: Optional[ReleaseNotes] = None,
                  cpe: Optional[str] = None, swid: Optional[Swid] = None, pedigree: Optional[Pedigree] = None,
                  components: Optional[Iterable['Component']] = None, evidence: Optional[ComponentEvidence] = None,
-                 modified: bool = False
+                 modified: bool = False, manufacturer: Optional[OrganizationalEntity] = None,
+                 authors: Optional[Iterable[OrganizationalContact]] = None,
+                 omnibor_ids: Optional[Iterable[OmniborId]] = None, swhids: Optional[Iterable[Swhid]] = None,
+                 crypto_properties: Optional[CryptoProperties] = None, tags: Optional[Iterable[str]] = None,
+                 # Deprecated in v1.6
+                 author: Optional[str] = None,
                  ) -> None:
         self.type = type
         self.mime_type = mime_type
         if isinstance(bom_ref, BomRef):
             self._bom_ref = bom_ref
         else:
             self._bom_ref = BomRef(value=str(bom_ref) if bom_ref else None)
         self.supplier = supplier
+        self.manufacturer = manufacturer
+        self.authors = authors or []  # type:ignore[assignment]
         self.author = author
         self.publisher = publisher
         self.group = group
         self.name = name
         self.version = version
         self.description = description
         self.scope = scope
         self.hashes = hashes or []  # type:ignore[assignment]
         self.licenses = licenses or []  # type:ignore[assignment]
         self.copyright = copyright
         self.cpe = cpe
         self.purl = purl
+        self.omnibor_ids = omnibor_ids or []  # type:ignore[assignment]
+        self.swhids = swhids or []  # type:ignore[assignment]
         self.swid = swid
         self.modified = modified
         self.pedigree = pedigree
         self.external_references = external_references or []  # type:ignore[assignment]
         self.properties = properties or []  # type:ignore[assignment]
         self.components = components or []  # type:ignore[assignment]
         self.evidence = evidence
         self.release_notes = release_notes
+        self.crypto_properties = crypto_properties
+        self.tags = tags or []  # type:ignore[assignment]
+
+        if modified:
+            warn('`.component.modified` is deprecated from CycloneDX v1.3 onwards. '
+                 'Please use `@.pedigree` instead.', DeprecationWarning)
+        if author:
+            warn('`.component.author` is deprecated from CycloneDX v1.6 onwards. '
+                 'Please use `@.authors` or `@.manufacturer` instead.', DeprecationWarning)
 
     @property
     @serializable.type_mapping(_ComponentTypeSerializationHelper)
     @serializable.xml_attribute()
     def type(self) -> ComponentType:
         """
         Get the type of this Component.
@@ -980,14 +1128,15 @@
     @serializable.json_name('bom-ref')
     @serializable.type_mapping(BomRefHelper)
     @serializable.view(SchemaVersion1Dot1)
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_attribute()
     @serializable.xml_name('bom-ref')
     def bom_ref(self) -> BomRef:
         """
         An optional identifier which can be used to reference the component elsewhere in the BOM. Every bom-ref MUST be
         unique within the BOM.
 
@@ -999,14 +1148,15 @@
         return self._bom_ref
 
     @property
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_sequence(1)
     def supplier(self) -> Optional[OrganizationalEntity]:
         """
         The organization that supplied the component. The supplier may often be the manufacture, but may also be a
         distributor or repackager.
 
         Returns:
@@ -1015,49 +1165,87 @@
         return self._supplier
 
     @supplier.setter
     def supplier(self, supplier: Optional[OrganizationalEntity]) -> None:
         self._supplier = supplier
 
     @property
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_sequence(2)
+    def manufacturer(self) -> Optional[OrganizationalEntity]:
+        """
+        The organization that created the component.
+        Manufacturer is common in components created through automated processes.
+        Components created through manual means may have `@.authors` instead.
+
+        Returns:
+            `OrganizationalEntity` if set else `None`
+        """
+        return self._manufacturer
+
+    @manufacturer.setter
+    def manufacturer(self, manufacturer: Optional[OrganizationalEntity]) -> None:
+        self._manufacturer = manufacturer
+
+    @property
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'author')
+    @serializable.xml_sequence(3)
+    def authors(self) -> 'SortedSet[OrganizationalContact]':
+        """
+        The person(s) who created the component.
+        Authors are common in components created through manual processes.
+        Components created through automated means may have `@.manufacturer` instead.
+
+        Returns:
+            `Iterable[OrganizationalContact]` if set else `None`
+        """
+        return self._authors
+
+    @authors.setter
+    def authors(self, authors: Iterable[OrganizationalContact]) -> None:
+        self._authors = SortedSet(authors)
+
+    @property
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
-    @serializable.xml_sequence(2)
+    @serializable.view(SchemaVersion1Dot6)  # todo: this is deprecated in v1.6?
+    @serializable.xml_sequence(4)
     def author(self) -> Optional[str]:
         """
         The person(s) or organization(s) that authored the component.
 
         Returns:
             `str` if set else `None`
         """
         return self._author
 
     @author.setter
     def author(self, author: Optional[str]) -> None:
         self._author = author
 
     @property
-    @serializable.xml_sequence(3)
+    @serializable.xml_sequence(5)
     def publisher(self) -> Optional[str]:
         """
         The person(s) or organization(s) that published the component
 
         Returns:
             `str` if set else `None`
         """
         return self._publisher
 
     @publisher.setter
     def publisher(self, publisher: Optional[str]) -> None:
         self._publisher = publisher
 
     @property
-    @serializable.xml_sequence(4)
+    @serializable.xml_sequence(6)
     def group(self) -> Optional[str]:
         """
         The grouping name or identifier. This will often be a shortened, single name of the company or project that
         produced the component, or the source package or domain name. Whitespace and special characters should be
         avoided.
 
         Examples include: `apache`, `org.apache.commons`, and `apache.org`.
@@ -1068,15 +1256,15 @@
         return self._group
 
     @group.setter
     def group(self, group: Optional[str]) -> None:
         self._group = group
 
     @property
-    @serializable.xml_sequence(5)
+    @serializable.xml_sequence(7)
     def name(self) -> str:
         """
         The name of the component.
 
         This will often be a shortened, single name of the component.
 
         Examples: `commons-lang3` and `jquery`.
@@ -1091,33 +1279,35 @@
         self._name = name
 
     @property
     @serializable.include_none(SchemaVersion1Dot0, '')
     @serializable.include_none(SchemaVersion1Dot1, '')
     @serializable.include_none(SchemaVersion1Dot2, '')
     @serializable.include_none(SchemaVersion1Dot3, '')
-    @serializable.xml_sequence(6)
+    @serializable.xml_sequence(8)
     def version(self) -> Optional[str]:
         """
         The component version. The version should ideally comply with semantic versioning but is not enforced.
 
         This is NOT optional for CycloneDX Schema Version < 1.4 but was agreed to default to an empty string where a
         version was not supplied for schema versions < 1.4
 
         Returns:
             Declared version of this Component as `str` or `None`
         """
         return self._version
 
     @version.setter
     def version(self, version: Optional[str]) -> None:
+        if version and len(version) > 1024:
+            warn('`.component.version`has a maximum length of 1024 from CycloneDX v1.6 onwards.', UserWarning)
         self._version = version
 
     @property
-    @serializable.xml_sequence(7)
+    @serializable.xml_sequence(9)
     def description(self) -> Optional[str]:
         """
         Get the description of this Component.
 
         Returns:
             `str` if set, else `None`.
         """
@@ -1125,15 +1315,15 @@
 
     @description.setter
     def description(self, description: Optional[str]) -> None:
         self._description = description
 
     @property
     @serializable.type_mapping(_ComponentScopeSerializationHelper)
-    @serializable.xml_sequence(8)
+    @serializable.xml_sequence(10)
     def scope(self) -> Optional[ComponentScope]:
         """
         Specifies the scope of the component.
 
         If scope is not specified, 'required' scope should be assumed by the consumer of the BOM.
 
         Returns:
@@ -1143,15 +1333,15 @@
 
     @scope.setter
     def scope(self, scope: Optional[ComponentScope]) -> None:
         self._scope = scope
 
     @property
     @serializable.type_mapping(_HashTypeRepositorySerializationHelper)
-    @serializable.xml_sequence(9)
+    @serializable.xml_sequence(11)
     def hashes(self) -> 'SortedSet[HashType]':
         """
         Optional list of hashes that help specify the integrity of this Component.
 
         Returns:
              Set of `HashType`
         """
@@ -1163,31 +1353,32 @@
 
     @property
     @serializable.view(SchemaVersion1Dot1)
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.type_mapping(LicenseRepositoryHelper)
-    @serializable.xml_sequence(10)
+    @serializable.xml_sequence(12)
     def licenses(self) -> LicenseRepository:
         """
         A optional list of statements about how this Component is licensed.
 
         Returns:
             Set of `LicenseChoice`
         """
         return self._licenses
 
     @licenses.setter
     def licenses(self, licenses: Iterable[License]) -> None:
         self._licenses = LicenseRepository(licenses)
 
     @property
-    @serializable.xml_sequence(11)
+    @serializable.xml_sequence(13)
     def copyright(self) -> Optional[str]:
         """
         An optional copyright notice informing users of the underlying claims to copyright ownership in a published
         work.
 
         Returns:
             `str` or `None`
@@ -1195,15 +1386,15 @@
         return self._copyright
 
     @copyright.setter
     def copyright(self, copyright: Optional[str]) -> None:
         self._copyright = copyright
 
     @property
-    @serializable.xml_sequence(12)
+    @serializable.xml_sequence(14)
     def cpe(self) -> Optional[str]:
         """
         Specifies a well-formed CPE name that conforms to the CPE 2.2 or 2.3 specification.
         See https://nvd.nist.gov/products/cpe
 
         Returns:
             `str` if set else `None`
@@ -1212,15 +1403,15 @@
 
     @cpe.setter
     def cpe(self, cpe: Optional[str]) -> None:
         self._cpe = cpe
 
     @property
     @serializable.type_mapping(PackageUrl)
-    @serializable.xml_sequence(13)
+    @serializable.xml_sequence(15)
     def purl(self) -> Optional[PackageURL]:
         """
         Specifies the package-url (PURL).
 
         The purl, if specified, must be valid and conform to the specification defined at:
         https://github.com/package-url/purl-spec
 
@@ -1230,49 +1421,91 @@
         return self._purl
 
     @purl.setter
     def purl(self, purl: Optional[PackageURL]) -> None:
         self._purl = purl
 
     @property
+    @serializable.json_name('omniborId')
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_array(serializable.XmlArraySerializationType.FLAT, child_name='omniborId')
+    @serializable.xml_sequence(16)
+    def omnibor_ids(self) -> 'SortedSet[OmniborId]':
+        """
+        Specifies the OmniBOR Artifact ID. The OmniBOR, if specified, MUST be valid and conform to the specification
+        defined at: https://www.iana.org/assignments/uri-schemes/prov/gitoid
+
+        Returns:
+            `Iterable[str]` or `None`
+        """
+
+        return self._omnibor_ids
+
+    @omnibor_ids.setter
+    def omnibor_ids(self, omnibor_ids: Iterable[OmniborId]) -> None:
+        self._omnibor_ids = SortedSet(omnibor_ids)
+
+    @property
+    @serializable.json_name('swhid')
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_array(serializable.XmlArraySerializationType.FLAT, child_name='swhid')
+    @serializable.xml_sequence(17)
+    def swhids(self) -> 'SortedSet[Swhid]':
+        """
+        Specifies the Software Heritage persistent identifier (SWHID). The SWHID, if specified, MUST be valid and
+        conform to the specification defined at:
+        https://docs.softwareheritage.org/devel/swh-model/persistent-identifiers.html
+
+        Returns:
+            `Iterable[Swhid]` if set else `None`
+        """
+        return self._swhids
+
+    @swhids.setter
+    def swhids(self, swhids: Iterable[Swhid]) -> None:
+        self._swhids = SortedSet(swhids)
+
+    @property
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
-    @serializable.xml_sequence(14)
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_sequence(18)
     def swid(self) -> Optional[Swid]:
         """
         Specifies metadata and content for ISO-IEC 19770-2 Software Identification (SWID) Tags.
 
         Returns:
             `Swid` if set else `None`
         """
         return self._swid
 
     @swid.setter
     def swid(self, swid: Optional[Swid]) -> None:
         self._swid = swid
 
     @property
-    @serializable.view(SchemaVersion1Dot0)
-    @serializable.xml_sequence(18)
+    @serializable.view(SchemaVersion1Dot0)  # todo: Deprecated in v1.3
+    @serializable.xml_sequence(19)
     def modified(self) -> bool:
         return self._modified
 
     @modified.setter
     def modified(self, modified: bool) -> None:
         self._modified = modified
 
     @property
     @serializable.view(SchemaVersion1Dot1)
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
-    @serializable.xml_sequence(16)
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_sequence(20)
     def pedigree(self) -> Optional[Pedigree]:
         """
         Component pedigree is a way to document complex supply chain scenarios where components are created,
         distributed, modified, redistributed, combined with other components, etc.
 
         Returns:
             `Pedigree` if set else `None`
@@ -1285,16 +1518,17 @@
 
     @property
     @serializable.view(SchemaVersion1Dot1)
     @serializable.view(SchemaVersion1Dot2)
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'reference')
-    @serializable.xml_sequence(17)
+    @serializable.xml_sequence(21)
     def external_references(self) -> 'SortedSet[ExternalReference]':
         """
         Provides the ability to document external references related to the component or to the project the component
         describes.
 
         Returns:
             Set of `ExternalReference`
@@ -1305,16 +1539,17 @@
     def external_references(self, external_references: Iterable[ExternalReference]) -> None:
         self._external_references = SortedSet(external_references)
 
     @property
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'property')
-    @serializable.xml_sequence(18)
+    @serializable.xml_sequence(22)
     def properties(self) -> 'SortedSet[Property]':
         """
         Provides the ability to document properties in a key/value store. This provides flexibility to include data not
         officially supported in the standard without having to use additional namespaces or create extensions.
 
         Return:
             Set of `Property`
@@ -1323,15 +1558,15 @@
 
     @properties.setter
     def properties(self, properties: Iterable[Property]) -> None:
         self._properties = SortedSet(properties)
 
     @property
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'component')
-    @serializable.xml_sequence(19)
+    @serializable.xml_sequence(23)
     def components(self) -> "SortedSet['Component']":
         """
         A list of software and hardware components included in the parent component. This is not a dependency tree. It
         provides a way to specify a hierarchical representation of component assemblies, similar to system -> subsystem
         -> parts assembly in physical supply chains.
 
         Returns:
@@ -1343,15 +1578,16 @@
     def components(self, components: Iterable['Component']) -> None:
         self._components = SortedSet(components)
 
     @property
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
-    @serializable.xml_sequence(20)
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_sequence(24)
     def evidence(self) -> Optional[ComponentEvidence]:
         """
         Provides the ability to document evidence collected through various forms of extraction or analysis.
 
         Returns:
             `ComponentEvidence` if set else `None`
         """
@@ -1360,15 +1596,16 @@
     @evidence.setter
     def evidence(self, evidence: Optional[ComponentEvidence]) -> None:
         self._evidence = evidence
 
     @property
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
-    @serializable.xml_sequence(21)
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_sequence(25)
     def release_notes(self) -> Optional[ReleaseNotes]:
         """
         Specifies optional release notes.
 
         Returns:
             `ReleaseNotes` or `None`
         """
@@ -1396,14 +1633,52 @@
     # def data(self) -> ...:
     #     ...  # TODO since CDX1.5
     #
     # @data.setter
     # def data(self, ...) -> None:
     #     ...  # TODO since CDX1.5
 
+    @property
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_sequence(30)
+    def crypto_properties(self) -> Optional[CryptoProperties]:
+        """
+        Cryptographic assets have properties that uniquely define them and that make them actionable for further
+        reasoning. As an example, it makes a difference if one knows the algorithm family (e.g. AES) or the specific
+        variant or instantiation (e.g. AES-128-GCM). This is because the security level and the algorithm primitive
+        (authenticated encryption) is only defined by the definition of the algorithm variant. The presence of a weak
+        cryptographic algorithm like SHA1 vs. HMAC-SHA1 also makes a difference.
+
+        Returns:
+            `CryptoProperties` or `None`
+        """
+        return self._crypto_properties
+
+    @crypto_properties.setter
+    def crypto_properties(self, crypto_properties: Optional[CryptoProperties]) -> None:
+        self._crypto_properties = crypto_properties
+
+    @property
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'tag')
+    @serializable.xml_sequence(31)
+    def tags(self) -> 'SortedSet[str]':
+        """
+        Textual strings that aid in discovery, search, and retrieval of the associated object.
+        Tags often serve as a way to group or categorize similar or related objects by various attributes.
+
+        Returns:
+            `Iterable[str]`
+        """
+        return self._tags
+
+    @tags.setter
+    def tags(self, tags: Iterable[str]) -> None:
+        self._tags = SortedSet(tags)
+
     def get_all_nested_components(self, include_self: bool = False) -> Set['Component']:
         components = set()
         if include_self:
             components.add(self)
 
         for c in self.components:
             components.update(c.get_all_nested_components(include_self=True))
@@ -1431,13 +1706,14 @@
         return NotImplemented
 
     def __hash__(self) -> int:
         return hash((
             self.type, self.mime_type, self.supplier, self.author, self.publisher, self.group, self.name,
             self.version, self.description, self.scope, tuple(self.hashes), tuple(self.licenses), self.copyright,
             self.cpe, self.purl, self.swid, self.pedigree, tuple(self.external_references), tuple(self.properties),
-            tuple(self.components), self.evidence, self.release_notes, self.modified
+            tuple(self.components), self.evidence, self.release_notes, self.modified, tuple(self.authors),
+            tuple(self.omnibor_ids),
         ))
 
     def __repr__(self) -> str:
         return f'<Component bom-ref={self.bom_ref!r}, group={self.group}, name={self.name}, ' \
                f'version={self.version}, type={self.type}>'
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/dependency.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/impact_analysis.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/impact_analysis.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/issue.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/license.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/license.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 # Copyright (c) OWASP Foundation. All Rights Reserved.
 
 
 """
 License related things
 """
 
-
+from enum import Enum
 from typing import TYPE_CHECKING, Any, Optional, Union
 from warnings import warn
 
 import serializable
 from sortedcontainers import SortedSet
 
 from .._internal.compare import ComparableTuple as _ComparableTuple
 from ..exception.model import MutuallyExclusivePropertiesException
+from ..schema.schema import SchemaVersion1Dot6
 from . import AttachedText, XsUri
 
 
 @serializable.serializable_class(name='license')
 class DisjunctiveLicense:
     """
     This is our internal representation of `licenseType` complex type that can be used in multiple places within
@@ -155,27 +156,72 @@
     def __hash__(self) -> int:
         return hash((self._id, self._name, self._text, self._url))
 
     def __repr__(self) -> str:
         return f'<License id={self._id!r}, name={self._name!r}>'
 
 
+@serializable.serializable_enum
+class LicenseExpressionAcknowledgement(str, Enum):
+    """
+    This is our internal representation of the `type_licenseAcknowledgementEnumerationType` ENUM type
+    within the CycloneDX standard.
+
+    .. note::
+        Introduced in CycloneDX v1.6
+
+    .. note::
+        See the CycloneDX Schema for hashType:
+        https://cyclonedx.org/docs/1.6/#type_licenseAcknowledgementEnumerationType
+    """
+
+    CONCLUDED = 'concluded'
+    DECLARED = 'declared'
+
+
 @serializable.serializable_class(name='expression')
 class LicenseExpression:
     """
     This is our internal representation of `licenseType`'s  expression type that can be used in multiple places within
     a CycloneDX BOM document.
 
     .. note::
         See the CycloneDX Schema definition:
         https://cyclonedx.org/docs/1.4/json/#components_items_licenses_items_expression
     """
 
-    def __init__(self, value: str) -> None:
+    def __init__(self, value: str,
+                 acknowledgement: Optional[LicenseExpressionAcknowledgement] = None) -> None:
         self._value = value
+        self.acknowledgement = acknowledgement
+
+    @property
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_attribute()
+    def acknowledgement(self) -> Optional[LicenseExpressionAcknowledgement]:
+        """
+        Declared licenses and concluded licenses represent two different stages in the licensing process within
+        software development.
+
+        Declared licenses refer to the initial intention of the software authors regarding the
+        licensing terms under which their code is released. On the other hand, concluded licenses are the result of a
+        comprehensive analysis of the project's codebase to identify and confirm the actual licenses of the components
+        used, which may differ from the initially declared licenses. While declared licenses provide an upfront
+        indication of the licensing intentions, concluded licenses offer a more thorough understanding of the actual
+        licensing within a project, facilitating proper compliance and risk management. Observed licenses are defined
+        in evidence.licenses. Observed licenses form the evidence necessary to substantiate a concluded license.
+
+        Returns:
+            `LicenseExpressionAcknowledgement` or `None`
+        """
+        return self._acknowledgement
+
+    @acknowledgement.setter
+    def acknowledgement(self, acknowledgement: Optional[LicenseExpressionAcknowledgement]) -> None:
+        self._acknowledgement = acknowledgement
 
     @property
     @serializable.xml_name('.')
     @serializable.json_name('expression')
     def value(self) -> str:
         """
         Value of this LicenseExpression.
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/release_note.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/service.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,18 @@
 
 import serializable
 from sortedcontainers import SortedSet
 
 from cyclonedx.serialization import BomRefHelper, LicenseRepositoryHelper
 
 from .._internal.compare import ComparableTuple as _ComparableTuple
-from ..schema.schema import SchemaVersion1Dot3, SchemaVersion1Dot4, SchemaVersion1Dot5
-from . import DataClassification, ExternalReference, OrganizationalEntity, Property, XsUri
+from ..schema.schema import SchemaVersion1Dot3, SchemaVersion1Dot4, SchemaVersion1Dot5, SchemaVersion1Dot6
+from . import DataClassification, ExternalReference, Property, XsUri
 from .bom_ref import BomRef
+from .contact import OrganizationalEntity
 from .dependency import Dependable
 from .license import License, LicenseRepository
 from .release_note import ReleaseNotes
 
 
 @serializable.serializable_class
 class Service(Dependable):
@@ -94,15 +95,15 @@
         """
         return self._bom_ref
 
     @property
     @serializable.xml_sequence(1)
     def provider(self) -> Optional[OrganizationalEntity]:
         """
-        Get the The organization that provides the service.
+        Get the organization that provides the service.
 
         Returns:
             `OrganizationalEntity` if set else `None`
         """
         return self._provider
 
     @provider.setter
@@ -285,14 +286,15 @@
     def external_references(self, external_references: Iterable[ExternalReference]) -> None:
         self._external_references = SortedSet(external_references)
 
     @property
     @serializable.view(SchemaVersion1Dot3)
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_array(serializable.XmlArraySerializationType.NESTED, 'property')
     @serializable.xml_sequence(13)
     def properties(self) -> 'SortedSet[Property]':
         """
         Provides the ability to document properties in a key/value store. This provides flexibility to include data not
         officially supported in the standard without having to use additional namespaces or create extensions.
 
@@ -324,14 +326,15 @@
     @services.setter
     def services(self, services: Iterable['Service']) -> None:
         self._services = SortedSet(services)
 
     @property
     @serializable.view(SchemaVersion1Dot4)
     @serializable.view(SchemaVersion1Dot5)
+    @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_sequence(15)
     def release_notes(self) -> Optional[ReleaseNotes]:
         """
         Specifies optional release notes.
 
         Returns:
             `ReleaseNotes` or `None`
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/model/vulnerability.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/model/vulnerability.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,18 +36,19 @@
 from typing import Any, Dict, FrozenSet, Iterable, Optional, Tuple, Type, Union
 
 import serializable
 from sortedcontainers import SortedSet
 
 from .._internal.compare import ComparableTuple as _ComparableTuple
 from ..exception.model import MutuallyExclusivePropertiesException, NoPropertiesProvidedException
-from ..schema.schema import SchemaVersion1Dot4, SchemaVersion1Dot5
+from ..schema.schema import SchemaVersion1Dot4, SchemaVersion1Dot5, SchemaVersion1Dot6
 from ..serialization import BomRefHelper
-from . import OrganizationalContact, OrganizationalEntity, Property, Tool, XsUri
+from . import Property, Tool, XsUri
 from .bom_ref import BomRef
+from .contact import OrganizationalContact, OrganizationalEntity
 from .impact_analysis import (
     ImpactAnalysisAffectedStatus,
     ImpactAnalysisJustification,
     ImpactAnalysisResponse,
     ImpactAnalysisState,
 )
 
@@ -601,14 +602,15 @@
         VulnerabilityScoreSource.OWASP,
         VulnerabilityScoreSource.OTHER,
     })
     __CASES[SchemaVersion1Dot5] = __CASES[SchemaVersion1Dot4] | {
         VulnerabilityScoreSource.CVSS_V4,
         VulnerabilityScoreSource.SSVC
     }
+    __CASES[SchemaVersion1Dot6] = __CASES[SchemaVersion1Dot5]
 
     @classmethod
     def __normalize(cls, vss: VulnerabilityScoreSource, view: Type[serializable.ViewType]) -> str:
         return (
             vss
             if vss in cls.__CASES.get(view, ())
             else VulnerabilityScoreSource.OTHER
@@ -693,15 +695,15 @@
     1.4 - see https://github.com/CycloneDX/specification/blob/master/schema/ext/vulnerability-1.0.xsd.
 
     .. note::
         See `ratingType` in https://cyclonedx.org/docs/1.4/#ratingType
 
     .. warning::
         As part of implementing support for CycloneDX schema version 1.4, the three score types defined in the schema
-        externsion used prior to 1.4 have been deprecated. The deprecated `score_base` should loosely be equivalent to
+        extension used prior to 1.4 have been deprecated. The deprecated `score_base` should loosely be equivalent to
         the new `score` in 1.4 schema. Both `score_impact` and `score_exploitability` are deprecated and removed as
         they are redundant if you have the vector (the vector allows you to calculate the scores).
     """
 
     def __init__(self, *,
                  source: Optional[VulnerabilitySource] = None, score: Optional[Decimal] = None,
                  severity: Optional[VulnerabilitySeverity] = None,
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/output/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/output/json.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/output/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     BaseSchemaVersion,
     SchemaVersion1Dot0,
     SchemaVersion1Dot1,
     SchemaVersion1Dot2,
     SchemaVersion1Dot3,
     SchemaVersion1Dot4,
     SchemaVersion1Dot5,
+    SchemaVersion1Dot6,
 )
 from . import BaseOutput, BomRefDiscriminator
 
 if TYPE_CHECKING:  # pragma: no cover
     from ..model.bom import Bom
 
 
@@ -120,15 +121,22 @@
 
 class JsonV1Dot5(Json, SchemaVersion1Dot5):
 
     def _get_schema_uri(self) -> str:
         return 'http://cyclonedx.org/schema/bom-1.5.schema.json'
 
 
+class JsonV1Dot6(Json, SchemaVersion1Dot6):
+
+    def _get_schema_uri(self) -> str:
+        return 'http://cyclonedx.org/schema/bom-1.6.schema.json'
+
+
 BY_SCHEMA_VERSION: Dict[SchemaVersion, Type[Json]] = {
+    SchemaVersion.V1_6: JsonV1Dot6,
     SchemaVersion.V1_5: JsonV1Dot5,
     SchemaVersion.V1_4: JsonV1Dot4,
     SchemaVersion.V1_3: JsonV1Dot3,
     SchemaVersion.V1_2: JsonV1Dot2,
     SchemaVersion.V1_1: JsonV1Dot1,
     SchemaVersion.V1_0: JsonV1Dot0,
 }
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/output/xml.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/output/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     BaseSchemaVersion,
     SchemaVersion1Dot0,
     SchemaVersion1Dot1,
     SchemaVersion1Dot2,
     SchemaVersion1Dot3,
     SchemaVersion1Dot4,
     SchemaVersion1Dot5,
+    SchemaVersion1Dot6,
 )
 from . import BaseOutput, BomRefDiscriminator
 
 if TYPE_CHECKING:  # pragma: no cover
     from ..model.bom import Bom
 
 
@@ -115,15 +116,20 @@
     pass
 
 
 class XmlV1Dot5(Xml, SchemaVersion1Dot5):
     pass
 
 
+class XmlV1Dot6(Xml, SchemaVersion1Dot6):
+    pass
+
+
 BY_SCHEMA_VERSION: Dict[SchemaVersion, Type[Xml]] = {
+    SchemaVersion.V1_6: XmlV1Dot6,
     SchemaVersion.V1_5: XmlV1Dot5,
     SchemaVersion.V1_4: XmlV1Dot4,
     SchemaVersion.V1_3: XmlV1Dot3,
     SchemaVersion.V1_2: XmlV1Dot2,
     SchemaVersion.V1_1: XmlV1Dot1,
     SchemaVersion.V1_0: XmlV1Dot0,
 }
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     Cases are hashable.
     Cases are comparable(!=,>=,>,==,<,<=)
 
     Do not rely on the actual/literal values, just use enum cases, like so:
         my_sv = SchemaVersion.V1_3
     """
 
+    V1_6 = (1, 6)
     V1_5 = (1, 5)
     V1_4 = (1, 4)
     V1_3 = (1, 3)
     V1_2 = (1, 2)
     V1_1 = (1, 1)
     V1_0 = (1, 0)
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/README.md` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # Resources: Schema files
 
 some schema for offline use as download via [script](../../../tools/schema-downloader.py).
 original sources: <https://github.com/CycloneDX/specification/tree/master/schema>
 
 Currently using version
-[299209abd9531d808e0cc4235e77a7c4b1b53d96](https://github.com/CycloneDX/specification/commit/299209abd9531d808e0cc4235e77a7c4b1b53d96)
+[55343ba19dee1785acf1ce9191540d5fd7b590db](https://github.com/CycloneDX/specification/commit/55343ba19dee1785acf1ce9191540d5fd7b590db)
 
 | file | note |
 |------|------|
 | [`bom-1.0.SNAPSHOT.xsd`](bom-1.0.SNAPSHOT.xsd) | applied changes: 1 |
 | [`bom-1.1.SNAPSHOT.xsd`](bom-1.1.SNAPSHOT.xsd) | applied changes: 1 |
 | [`bom-1.2.SNAPSHOT.xsd`](bom-1.2.SNAPSHOT.xsd) | applied changes: 1 |
 | [`bom-1.3.SNAPSHOT.xsd`](bom-1.3.SNAPSHOT.xsd) | applied changes: 1 |
 | [`bom-1.4.SNAPSHOT.xsd`](bom-1.4.SNAPSHOT.xsd) | applied changes: 1 |
 | [`bom-1.5.SNAPSHOT.xsd`](bom-1.5.SNAPSHOT.xsd) | applied changes: 1 |
+| [`bom-1.6.SNAPSHOT.xsd`](bom-1.6.SNAPSHOT.xsd) | applied changes: 1 |
 | [`bom-1.2.SNAPSHOT.schema.json`](bom-1.2.SNAPSHOT.schema.json) | applied changes: 2,3,4,5 |
 | [`bom-1.3.SNAPSHOT.schema.json`](bom-1.3.SNAPSHOT.schema.json) | applied changes: 2,3,4,5 |
 | [`bom-1.4.SNAPSHOT.schema.json`](bom-1.4.SNAPSHOT.schema.json) | applied changes: 2,3,4,5 |
 | [`bom-1.5.SNAPSHOT.schema.json`](bom-1.5.SNAPSHOT.schema.json) | applied changes: 2,3,4,5 |
+| [`bom-1.6.SNAPSHOT.schema.json`](bom-1.6.SNAPSHOT.schema.json) | applied changes: 2,3,4,5 |
 | [`bom-1.2-strict.SNAPSHOT.schema.json`](bom-1.2-strict.SNAPSHOT.schema.json) | applied changes: 2,3,4,5 |
 | [`bom-1.3-strict.SNAPSHOT.schema.json`](bom-1.3-strict.SNAPSHOT.schema.json) | applied changes: 2,3,4,5 |
 | [`spdx.SNAPSHOT.xsd`](spdx.SNAPSHOT.xsd) | |
 | [`spdx.SNAPSHOT.schema.json`](spdx.SNAPSHOT.schema.json) | |
 | [`jsf-0.82.SNAPSHOT.schema.json`](jsf-0.82.SNAPSHOT.schema.json) | |
 
 changes:
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,34 +24,36 @@
 from typing import Dict, Optional
 
 from .. import SchemaVersion
 
 __DIR = dirname(__file__)
 
 BOM_XML: Dict[SchemaVersion, Optional[str]] = {
+    SchemaVersion.V1_6: join(__DIR, 'bom-1.6.SNAPSHOT.xsd'),
     SchemaVersion.V1_5: join(__DIR, 'bom-1.5.SNAPSHOT.xsd'),
     SchemaVersion.V1_4: join(__DIR, 'bom-1.4.SNAPSHOT.xsd'),
     SchemaVersion.V1_3: join(__DIR, 'bom-1.3.SNAPSHOT.xsd'),
     SchemaVersion.V1_2: join(__DIR, 'bom-1.2.SNAPSHOT.xsd'),
     SchemaVersion.V1_1: join(__DIR, 'bom-1.1.SNAPSHOT.xsd'),
     SchemaVersion.V1_0: join(__DIR, 'bom-1.0.SNAPSHOT.xsd'),
 }
 
 BOM_JSON: Dict[SchemaVersion, Optional[str]] = {
+    SchemaVersion.V1_6: join(__DIR, 'bom-1.6.SNAPSHOT.schema.json'),
     SchemaVersion.V1_5: join(__DIR, 'bom-1.5.SNAPSHOT.schema.json'),
     SchemaVersion.V1_4: join(__DIR, 'bom-1.4.SNAPSHOT.schema.json'),
     SchemaVersion.V1_3: join(__DIR, 'bom-1.3.SNAPSHOT.schema.json'),
     SchemaVersion.V1_2: join(__DIR, 'bom-1.2.SNAPSHOT.schema.json'),
     # <= v1.1 is not defined in JSON
     SchemaVersion.V1_1: None,
     SchemaVersion.V1_0: None,
 }
 
 BOM_JSON_STRICT: Dict[SchemaVersion, Optional[str]] = {
-    # >= v1.4 is already strict - no special file here
+    SchemaVersion.V1_6: BOM_JSON[SchemaVersion.V1_6],
     SchemaVersion.V1_5: BOM_JSON[SchemaVersion.V1_5],
     SchemaVersion.V1_4: BOM_JSON[SchemaVersion.V1_4],
     # <= 1.3 need special files
     SchemaVersion.V1_3: join(__DIR, 'bom-1.3-strict.SNAPSHOT.schema.json'),
     SchemaVersion.V1_2: join(__DIR, 'bom-1.2-strict.SNAPSHOT.schema.json'),
     # <= v1.1 is not defined in JSON
     SchemaVersion.V1_1: None,
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8870738636363636%*

 * *Differences: {"'$comment'": "'v1.0-3.23'",*

 * * "'enum'": "{insert: [(5, 'Adobe-Display-PostScript'), (7, 'Adobe-Utopia'), (24, 'AML-glslang'), "*

 * *           "(48, 'bcrypt-Solar-Designer'), (58, 'Brian-Gladman-2-Clause'), (62, "*

 * *           "'BSD-2-Clause-Darwin'), (68, 'BSD-3-Clause-acpica'), (71, 'BSD-3-Clause-flex'), (72, "*

 * *           "'BSD-3-Clause-HP'), (80, 'BSD-3-Clause-Sun'), (88, 'BSD-Inferno-Nettverk'), (90, "*

 * *           "'BSD-Source-beginning-file'), (92, 'BSD-Systemics'), (93, 'BSD-Systemics-W3Works'), "*

 * *          […]*

```diff
@@ -1,18 +1,20 @@
 {
-    "$comment": "v1.0-3.21",
+    "$comment": "v1.0-3.23",
     "$id": "http://cyclonedx.org/schema/spdx.schema.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "enum": [
         "0BSD",
         "AAL",
         "Abstyles",
         "AdaCore-doc",
         "Adobe-2006",
+        "Adobe-Display-PostScript",
         "Adobe-Glyph",
+        "Adobe-Utopia",
         "ADSL",
         "AFL-1.1",
         "AFL-1.2",
         "AFL-2.0",
         "AFL-2.1",
         "AFL-3.0",
         "Afmparse",
@@ -21,14 +23,15 @@
         "AGPL-1.0-or-later",
         "AGPL-3.0",
         "AGPL-3.0-only",
         "AGPL-3.0-or-later",
         "Aladdin",
         "AMDPLPA",
         "AML",
+        "AML-glslang",
         "AMPAS",
         "ANTLR-PD",
         "ANTLR-PD-fallback",
         "Apache-1.0",
         "Apache-1.1",
         "Apache-2.0",
         "APAFML",
@@ -44,64 +47,77 @@
         "Artistic-1.0-Perl",
         "Artistic-2.0",
         "ASWF-Digital-Assets-1.0",
         "ASWF-Digital-Assets-1.1",
         "Baekmuk",
         "Bahyph",
         "Barr",
+        "bcrypt-Solar-Designer",
         "Beerware",
         "Bitstream-Charter",
         "Bitstream-Vera",
         "BitTorrent-1.0",
         "BitTorrent-1.1",
         "blessing",
         "BlueOak-1.0.0",
         "Boehm-GC",
         "Borceux",
+        "Brian-Gladman-2-Clause",
         "Brian-Gladman-3-Clause",
         "BSD-1-Clause",
         "BSD-2-Clause",
+        "BSD-2-Clause-Darwin",
         "BSD-2-Clause-FreeBSD",
         "BSD-2-Clause-NetBSD",
         "BSD-2-Clause-Patent",
         "BSD-2-Clause-Views",
         "BSD-3-Clause",
+        "BSD-3-Clause-acpica",
         "BSD-3-Clause-Attribution",
         "BSD-3-Clause-Clear",
+        "BSD-3-Clause-flex",
+        "BSD-3-Clause-HP",
         "BSD-3-Clause-LBNL",
         "BSD-3-Clause-Modification",
         "BSD-3-Clause-No-Military-License",
         "BSD-3-Clause-No-Nuclear-License",
         "BSD-3-Clause-No-Nuclear-License-2014",
         "BSD-3-Clause-No-Nuclear-Warranty",
         "BSD-3-Clause-Open-MPI",
+        "BSD-3-Clause-Sun",
         "BSD-4-Clause",
         "BSD-4-Clause-Shortened",
         "BSD-4-Clause-UC",
         "BSD-4.3RENO",
         "BSD-4.3TAHOE",
         "BSD-Advertising-Acknowledgement",
         "BSD-Attribution-HPND-disclaimer",
+        "BSD-Inferno-Nettverk",
         "BSD-Protection",
+        "BSD-Source-beginning-file",
         "BSD-Source-Code",
+        "BSD-Systemics",
+        "BSD-Systemics-W3Works",
         "BSL-1.0",
         "BUSL-1.1",
         "bzip2-1.0.5",
         "bzip2-1.0.6",
         "C-UDA-1.0",
         "CAL-1.0",
         "CAL-1.0-Combined-Work-Exception",
         "Caldera",
+        "Caldera-no-preamble",
         "CATOSL-1.1",
         "CC-BY-1.0",
         "CC-BY-2.0",
         "CC-BY-2.5",
         "CC-BY-2.5-AU",
         "CC-BY-3.0",
         "CC-BY-3.0-AT",
+        "CC-BY-3.0-AU",
         "CC-BY-3.0-DE",
         "CC-BY-3.0-IGO",
         "CC-BY-3.0-NL",
         "CC-BY-3.0-US",
         "CC-BY-4.0",
         "CC-BY-NC-1.0",
         "CC-BY-NC-2.0",
@@ -158,41 +174,47 @@
         "CECILL-C",
         "CERN-OHL-1.1",
         "CERN-OHL-1.2",
         "CERN-OHL-P-2.0",
         "CERN-OHL-S-2.0",
         "CERN-OHL-W-2.0",
         "CFITSIO",
+        "check-cvs",
         "checkmk",
         "ClArtistic",
         "Clips",
         "CMU-Mach",
+        "CMU-Mach-nodoc",
         "CNRI-Jython",
         "CNRI-Python",
         "CNRI-Python-GPL-Compatible",
         "COIL-1.0",
         "Community-Spec-1.0",
         "Condor-1.1",
         "copyleft-next-0.3.0",
         "copyleft-next-0.3.1",
         "Cornell-Lossless-JPEG",
         "CPAL-1.0",
         "CPL-1.0",
         "CPOL-1.02",
+        "Cronyx",
         "Crossword",
         "CrystalStacker",
         "CUA-OPL-1.0",
         "Cube",
         "curl",
         "D-FSL-1.0",
+        "DEC-3-Clause",
         "diffmark",
         "DL-DE-BY-2.0",
+        "DL-DE-ZERO-2.0",
         "DOC",
         "Dotseqn",
         "DRL-1.0",
+        "DRL-1.1",
         "DSDP",
         "dtoa",
         "dvipdfm",
         "ECL-1.0",
         "ECL-2.0",
         "eCos-2.0",
         "EFL-1.0",
@@ -207,23 +229,29 @@
         "etalab-2.0",
         "EUDatagrid",
         "EUPL-1.0",
         "EUPL-1.1",
         "EUPL-1.2",
         "Eurosym",
         "Fair",
+        "FBM",
         "FDK-AAC",
+        "Ferguson-Twofish",
         "Frameworx-1.0",
         "FreeBSD-DOC",
         "FreeImage",
         "FSFAP",
+        "FSFAP-no-warranty-disclaimer",
         "FSFUL",
         "FSFULLR",
         "FSFULLRWD",
         "FTL",
+        "Furuseth",
+        "fwlw",
+        "GCR-docs",
         "GD",
         "GFDL-1.1",
         "GFDL-1.1-invariants-only",
         "GFDL-1.1-invariants-or-later",
         "GFDL-1.1-no-invariants-only",
         "GFDL-1.1-no-invariants-or-later",
         "GFDL-1.1-only",
@@ -265,22 +293,37 @@
         "GPL-3.0+",
         "GPL-3.0-only",
         "GPL-3.0-or-later",
         "GPL-3.0-with-autoconf-exception",
         "GPL-3.0-with-GCC-exception",
         "Graphics-Gems",
         "gSOAP-1.3b",
+        "gtkbook",
         "HaskellReport",
+        "hdparm",
         "Hippocratic-2.1",
         "HP-1986",
+        "HP-1989",
         "HPND",
+        "HPND-DEC",
+        "HPND-doc",
+        "HPND-doc-sell",
         "HPND-export-US",
+        "HPND-export-US-modify",
+        "HPND-Fenneberg-Livingston",
+        "HPND-INRIA-IMAG",
+        "HPND-Kevlin-Henney",
         "HPND-Markus-Kuhn",
+        "HPND-MIT-disclaimer",
+        "HPND-Pbmplus",
+        "HPND-sell-MIT-disclaimer-xserver",
+        "HPND-sell-regexpr",
         "HPND-sell-variant",
         "HPND-sell-variant-MIT-disclaimer",
+        "HPND-UC",
         "HTMLTIDY",
         "IBM-pibs",
         "ICU",
         "IEC-Code-Components-EULA",
         "IJG",
         "IJG-short",
         "ImageMagick",
@@ -290,19 +333,21 @@
         "Inner-Net-2.0",
         "Intel",
         "Intel-ACPI",
         "Interbase-1.0",
         "IPA",
         "IPL-1.0",
         "ISC",
+        "ISC-Veillard",
         "Jam",
         "JasPer-2.0",
         "JPL-image",
         "JPNIC",
         "JSON",
+        "Kastrup",
         "Kazlib",
         "Knuth-CTAN",
         "LAL-1.2",
         "LAL-1.3",
         "Latex2e",
         "Latex2e-translated-notice",
         "Leptonica",
@@ -329,40 +374,51 @@
         "LiLiQ-Rplus-1.1",
         "Linux-man-pages-1-para",
         "Linux-man-pages-copyleft",
         "Linux-man-pages-copyleft-2-para",
         "Linux-man-pages-copyleft-var",
         "Linux-OpenIB",
         "LOOP",
+        "LPD-document",
         "LPL-1.0",
         "LPL-1.02",
         "LPPL-1.0",
         "LPPL-1.1",
         "LPPL-1.2",
         "LPPL-1.3a",
         "LPPL-1.3c",
+        "lsof",
+        "Lucida-Bitmap-Fonts",
         "LZMA-SDK-9.11-to-9.20",
         "LZMA-SDK-9.22",
+        "Mackerras-3-Clause",
+        "Mackerras-3-Clause-acknowledgment",
+        "magaz",
+        "mailprio",
         "MakeIndex",
         "Martin-Birgmeier",
+        "McPhee-slideshow",
         "metamail",
         "Minpack",
         "MirOS",
         "MIT",
         "MIT-0",
         "MIT-advertising",
         "MIT-CMU",
         "MIT-enna",
         "MIT-feh",
         "MIT-Festival",
         "MIT-Modern-Variant",
         "MIT-open-group",
+        "MIT-testregex",
         "MIT-Wu",
         "MITNFA",
+        "MMIXware",
         "Motosoto",
+        "MPEG-SSG",
         "mpi-permissive",
         "mpich2",
         "MPL-1.0",
         "MPL-1.1",
         "MPL-2.0",
         "MPL-2.0-no-copyleft-exception",
         "mplus",
@@ -436,100 +492,122 @@
         "OLDAP-2.6",
         "OLDAP-2.7",
         "OLDAP-2.8",
         "OLFL-1.3",
         "OML",
         "OpenPBS-2.3",
         "OpenSSL",
+        "OpenSSL-standalone",
+        "OpenVision",
         "OPL-1.0",
         "OPL-UK-3.0",
         "OPUBL-1.0",
         "OSET-PL-2.1",
         "OSL-1.0",
         "OSL-1.1",
         "OSL-2.0",
         "OSL-2.1",
         "OSL-3.0",
+        "PADL",
         "Parity-6.0.0",
         "Parity-7.0.0",
         "PDDL-1.0",
         "PHP-3.0",
         "PHP-3.01",
+        "Pixar",
         "Plexus",
+        "pnmstitch",
         "PolyForm-Noncommercial-1.0.0",
         "PolyForm-Small-Business-1.0.0",
         "PostgreSQL",
         "PSF-2.0",
         "psfrag",
         "psutils",
         "Python-2.0",
         "Python-2.0.1",
+        "python-ldap",
         "Qhull",
         "QPL-1.0",
         "QPL-1.0-INRIA-2004",
+        "radvd",
         "Rdisc",
         "RHeCos-1.1",
         "RPL-1.1",
         "RPL-1.5",
         "RPSL-1.0",
         "RSA-MD",
         "RSCPL",
         "Ruby",
         "SAX-PD",
+        "SAX-PD-2.0",
         "Saxpath",
         "SCEA",
         "SchemeReport",
         "Sendmail",
         "Sendmail-8.23",
         "SGI-B-1.0",
         "SGI-B-1.1",
         "SGI-B-2.0",
+        "SGI-OpenGL",
         "SGP4",
         "SHL-0.5",
         "SHL-0.51",
         "SimPL-2.0",
         "SISSL",
         "SISSL-1.2",
+        "SL",
         "Sleepycat",
         "SMLNJ",
         "SMPPL",
         "SNIA",
         "snprintf",
+        "softSurfer",
+        "Soundex",
         "Spencer-86",
         "Spencer-94",
         "Spencer-99",
         "SPL-1.0",
+        "ssh-keyscan",
         "SSH-OpenSSH",
         "SSH-short",
+        "SSLeay-standalone",
         "SSPL-1.0",
         "StandardML-NJ",
         "SugarCRM-1.1.3",
+        "Sun-PPP",
         "SunPro",
         "SWL",
+        "swrule",
         "Symlinks",
         "TAPR-OHL-1.0",
         "TCL",
         "TCP-wrappers",
         "TermReadKey",
+        "TGPPL-1.0",
         "TMate",
         "TORQUE-1.1",
         "TOSL",
         "TPDL",
         "TPL-1.0",
         "TTWL",
+        "TTYP0",
         "TU-Berlin-1.0",
         "TU-Berlin-2.0",
         "UCAR",
         "UCL-1.0",
+        "ulem",
+        "UMich-Merit",
+        "Unicode-3.0",
         "Unicode-DFS-2015",
         "Unicode-DFS-2016",
         "Unicode-TOU",
         "UnixCrypt",
         "Unlicense",
         "UPL-1.0",
+        "URT-RLE",
         "Vim",
         "VOSTROM",
         "VSL-1.0",
         "W3C",
         "W3C-19980720",
         "W3C-20150513",
         "w3m",
@@ -541,49 +619,58 @@
         "X11",
         "X11-distribute-modifications-variant",
         "Xdebug-1.03",
         "Xerox",
         "Xfig",
         "XFree86-1.1",
         "xinetd",
+        "xkeyboard-config-Zinoviev",
         "xlock",
         "Xnet",
         "xpp",
         "XSkat",
         "YPL-1.0",
         "YPL-1.1",
         "Zed",
+        "Zeeff",
         "Zend-2.0",
         "Zimbra-1.3",
         "Zimbra-1.4",
         "Zlib",
         "zlib-acknowledgement",
         "ZPL-1.1",
         "ZPL-2.0",
         "ZPL-2.1",
         "389-exception",
         "Asterisk-exception",
         "Autoconf-exception-2.0",
         "Autoconf-exception-3.0",
         "Autoconf-exception-generic",
+        "Autoconf-exception-generic-3.0",
         "Autoconf-exception-macro",
+        "Bison-exception-1.24",
         "Bison-exception-2.2",
         "Bootloader-exception",
         "Classpath-exception-2.0",
         "CLISP-exception-2.0",
         "cryptsetup-OpenSSL-exception",
         "DigiRule-FOSS-exception",
         "eCos-exception-2.0",
         "Fawkes-Runtime-exception",
         "FLTK-exception",
+        "fmt-exception",
         "Font-exception-2.0",
         "freertos-exception-2.0",
         "GCC-exception-2.0",
+        "GCC-exception-2.0-note",
         "GCC-exception-3.1",
+        "Gmsh-exception",
         "GNAT-exception",
+        "GNOME-examples-exception",
+        "GNU-compiler-exception",
         "gnu-javamail-exception",
         "GPL-3.0-interface-exception",
         "GPL-3.0-linking-exception",
         "GPL-3.0-linking-source-exception",
         "GPL-CC-1.0",
         "GStreamer-exception-2005",
         "GStreamer-exception-2008",
@@ -603,19 +690,23 @@
         "OpenJDK-assembly-exception-1.0",
         "openvpn-openssl-exception",
         "PS-or-PDF-font-exception-20170817",
         "QPL-1.0-INRIA-2004-exception",
         "Qt-GPL-exception-1.0",
         "Qt-LGPL-exception-1.1",
         "Qwt-exception-1.0",
+        "SANE-exception",
         "SHL-2.0",
         "SHL-2.1",
+        "stunnel-exception",
         "SWI-exception",
         "Swift-exception",
+        "Texinfo-exception",
         "u-boot-exception-2.0",
+        "UBDL-exception",
         "Universal-FOSS-exception-1.0",
         "vsftpd-openssl-exception",
         "WxWindows-exception-3.1",
         "x11vnc-openssl-exception"
     ],
     "type": "string"
 }
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd`

 * *Files 1% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" elementFormDefault="qualified" targetNamespace="http://cyclonedx.org/schema/spdx" version="1.0-3.21">
+<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" elementFormDefault="qualified" targetNamespace="http://cyclonedx.org/schema/spdx" version="1.0-3.23">
   <xs:simpleType name="licenseId">
     <xs:restriction base="xs:string">
       <!-- Licenses -->
       <xs:enumeration value="0BSD">
         <xs:annotation>
           <xs:documentation>BSD Zero Clause License</xs:documentation>
         </xs:annotation>
@@ -24,19 +24,29 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Adobe-2006">
         <xs:annotation>
           <xs:documentation>Adobe Systems Incorporated Source Code License Agreement</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Adobe-Display-PostScript">
+        <xs:annotation>
+          <xs:documentation>Adobe Display PostScript License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Adobe-Glyph">
         <xs:annotation>
           <xs:documentation>Adobe Glyph List License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Adobe-Utopia">
+        <xs:annotation>
+          <xs:documentation>Adobe Utopia Font License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="ADSL">
         <xs:annotation>
           <xs:documentation>Amazon Digital Services License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="AFL-1.1">
         <xs:annotation>
@@ -109,14 +119,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="AML">
         <xs:annotation>
           <xs:documentation>Apple MIT License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="AML-glslang">
+        <xs:annotation>
+          <xs:documentation>AML glslang variant License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="AMPAS">
         <xs:annotation>
           <xs:documentation>Academy of Motion Picture Arts and Sciences BSD</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="ANTLR-PD">
         <xs:annotation>
@@ -224,14 +239,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Barr">
         <xs:annotation>
           <xs:documentation>Barr License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="bcrypt-Solar-Designer">
+        <xs:annotation>
+          <xs:documentation>bcrypt Solar Designer License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Beerware">
         <xs:annotation>
           <xs:documentation>Beerware License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Bitstream-Charter">
         <xs:annotation>
@@ -269,14 +289,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Borceux">
         <xs:annotation>
           <xs:documentation>Borceux license</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Brian-Gladman-2-Clause">
+        <xs:annotation>
+          <xs:documentation>Brian Gladman 2-Clause License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Brian-Gladman-3-Clause">
         <xs:annotation>
           <xs:documentation>Brian Gladman 3-Clause License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-1-Clause">
         <xs:annotation>
@@ -284,14 +309,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-2-Clause">
         <xs:annotation>
           <xs:documentation>BSD 2-Clause &quot;Simplified&quot; License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="BSD-2-Clause-Darwin">
+        <xs:annotation>
+          <xs:documentation>BSD 2-Clause - Ian Darwin variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="BSD-2-Clause-FreeBSD">
         <xs:annotation>
           <xs:documentation>BSD 2-Clause FreeBSD License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-2-Clause-NetBSD">
         <xs:annotation>
@@ -309,24 +339,39 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-3-Clause">
         <xs:annotation>
           <xs:documentation>BSD 3-Clause &quot;New&quot; or &quot;Revised&quot; License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="BSD-3-Clause-acpica">
+        <xs:annotation>
+          <xs:documentation>BSD 3-Clause acpica variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="BSD-3-Clause-Attribution">
         <xs:annotation>
           <xs:documentation>BSD with attribution</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-3-Clause-Clear">
         <xs:annotation>
           <xs:documentation>BSD 3-Clause Clear License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="BSD-3-Clause-flex">
+        <xs:annotation>
+          <xs:documentation>BSD 3-Clause Flex variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="BSD-3-Clause-HP">
+        <xs:annotation>
+          <xs:documentation>Hewlett-Packard BSD variant license</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="BSD-3-Clause-LBNL">
         <xs:annotation>
           <xs:documentation>Lawrence Berkeley National Labs BSD variant license</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-3-Clause-Modification">
         <xs:annotation>
@@ -354,14 +399,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-3-Clause-Open-MPI">
         <xs:annotation>
           <xs:documentation>BSD 3-Clause Open MPI variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="BSD-3-Clause-Sun">
+        <xs:annotation>
+          <xs:documentation>BSD 3-Clause Sun Microsystems</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="BSD-4-Clause">
         <xs:annotation>
           <xs:documentation>BSD 4-Clause &quot;Original&quot; or &quot;Old&quot; License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-4-Clause-Shortened">
         <xs:annotation>
@@ -389,24 +439,44 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-Attribution-HPND-disclaimer">
         <xs:annotation>
           <xs:documentation>BSD with Attribution and HPND disclaimer</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="BSD-Inferno-Nettverk">
+        <xs:annotation>
+          <xs:documentation>BSD-Inferno-Nettverk</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="BSD-Protection">
         <xs:annotation>
           <xs:documentation>BSD Protection License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="BSD-Source-beginning-file">
+        <xs:annotation>
+          <xs:documentation>BSD Source Code Attribution - beginning of file variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="BSD-Source-Code">
         <xs:annotation>
           <xs:documentation>BSD Source Code Attribution</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="BSD-Systemics">
+        <xs:annotation>
+          <xs:documentation>Systemics BSD variant license</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="BSD-Systemics-W3Works">
+        <xs:annotation>
+          <xs:documentation>Systemics W3Works BSD variant license</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="BSL-1.0">
         <xs:annotation>
           <xs:documentation>Boost Software License 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BUSL-1.1">
         <xs:annotation>
@@ -439,14 +509,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Caldera">
         <xs:annotation>
           <xs:documentation>Caldera License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Caldera-no-preamble">
+        <xs:annotation>
+          <xs:documentation>Caldera License (without preamble)</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="CATOSL-1.1">
         <xs:annotation>
           <xs:documentation>Computer Associates Trusted Open Source License 1.1</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="CC-BY-1.0">
         <xs:annotation>
@@ -474,14 +549,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="CC-BY-3.0-AT">
         <xs:annotation>
           <xs:documentation>Creative Commons Attribution 3.0 Austria</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="CC-BY-3.0-AU">
+        <xs:annotation>
+          <xs:documentation>Creative Commons Attribution 3.0 Australia</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="CC-BY-3.0-DE">
         <xs:annotation>
           <xs:documentation>Creative Commons Attribution 3.0 Germany</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="CC-BY-3.0-IGO">
         <xs:annotation>
@@ -794,14 +874,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="CFITSIO">
         <xs:annotation>
           <xs:documentation>CFITSIO License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="check-cvs">
+        <xs:annotation>
+          <xs:documentation>check-cvs License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="checkmk">
         <xs:annotation>
           <xs:documentation>Checkmk License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="ClArtistic">
         <xs:annotation>
@@ -814,14 +899,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="CMU-Mach">
         <xs:annotation>
           <xs:documentation>CMU Mach License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="CMU-Mach-nodoc">
+        <xs:annotation>
+          <xs:documentation>CMU    Mach - no notices-in-documentation variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="CNRI-Jython">
         <xs:annotation>
           <xs:documentation>CNRI Jython License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="CNRI-Python">
         <xs:annotation>
@@ -874,14 +964,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="CPOL-1.02">
         <xs:annotation>
           <xs:documentation>Code Project Open License 1.02</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Cronyx">
+        <xs:annotation>
+          <xs:documentation>Cronyx License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Crossword">
         <xs:annotation>
           <xs:documentation>Crossword License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="CrystalStacker">
         <xs:annotation>
@@ -904,24 +999,34 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="D-FSL-1.0">
         <xs:annotation>
           <xs:documentation>Deutsche Freie Software Lizenz</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="DEC-3-Clause">
+        <xs:annotation>
+          <xs:documentation>DEC 3-Clause License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="diffmark">
         <xs:annotation>
           <xs:documentation>diffmark license</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="DL-DE-BY-2.0">
         <xs:annotation>
           <xs:documentation>Data licence Germany – attribution – version 2.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="DL-DE-ZERO-2.0">
+        <xs:annotation>
+          <xs:documentation>Data licence Germany – zero – version 2.0</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="DOC">
         <xs:annotation>
           <xs:documentation>DOC License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Dotseqn">
         <xs:annotation>
@@ -929,14 +1034,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="DRL-1.0">
         <xs:annotation>
           <xs:documentation>Detection Rule License 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="DRL-1.1">
+        <xs:annotation>
+          <xs:documentation>Detection Rule License 1.1</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="DSDP">
         <xs:annotation>
           <xs:documentation>DSDP License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="dtoa">
         <xs:annotation>
@@ -1039,19 +1149,29 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Fair">
         <xs:annotation>
           <xs:documentation>Fair License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="FBM">
+        <xs:annotation>
+          <xs:documentation>Fuzzy Bitmap License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="FDK-AAC">
         <xs:annotation>
           <xs:documentation>Fraunhofer FDK AAC Codec Library</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Ferguson-Twofish">
+        <xs:annotation>
+          <xs:documentation>Ferguson Twofish License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Frameworx-1.0">
         <xs:annotation>
           <xs:documentation>Frameworx Open License 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="FreeBSD-DOC">
         <xs:annotation>
@@ -1064,14 +1184,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="FSFAP">
         <xs:annotation>
           <xs:documentation>FSF All Permissive License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="FSFAP-no-warranty-disclaimer">
+        <xs:annotation>
+          <xs:documentation>FSF All Permissive License (without Warranty)</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="FSFUL">
         <xs:annotation>
           <xs:documentation>FSF Unlimited License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="FSFULLR">
         <xs:annotation>
@@ -1084,14 +1209,29 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="FTL">
         <xs:annotation>
           <xs:documentation>Freetype Project License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Furuseth">
+        <xs:annotation>
+          <xs:documentation>Furuseth License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="fwlw">
+        <xs:annotation>
+          <xs:documentation>fwlw License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="GCR-docs">
+        <xs:annotation>
+          <xs:documentation>Gnome GCR Documentation License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="GD">
         <xs:annotation>
           <xs:documentation>GD License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="GFDL-1.1">
         <xs:annotation>
@@ -1329,54 +1469,129 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="gSOAP-1.3b">
         <xs:annotation>
           <xs:documentation>gSOAP Public License v1.3b</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="gtkbook">
+        <xs:annotation>
+          <xs:documentation>gtkbook License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HaskellReport">
         <xs:annotation>
           <xs:documentation>Haskell Language Report License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="hdparm">
+        <xs:annotation>
+          <xs:documentation>hdparm License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Hippocratic-2.1">
         <xs:annotation>
           <xs:documentation>Hippocratic License 2.1</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="HP-1986">
         <xs:annotation>
           <xs:documentation>Hewlett-Packard 1986 License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HP-1989">
+        <xs:annotation>
+          <xs:documentation>Hewlett-Packard 1989 License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HPND">
         <xs:annotation>
           <xs:documentation>Historical Permission Notice and Disclaimer</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-DEC">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - DEC variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="HPND-doc">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - documentation variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="HPND-doc-sell">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - documentation sell variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HPND-export-US">
         <xs:annotation>
           <xs:documentation>HPND with US Government export control warning</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-export-US-modify">
+        <xs:annotation>
+          <xs:documentation>HPND with US Government export control warning and modification rqmt</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="HPND-Fenneberg-Livingston">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - Fenneberg-Livingston variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="HPND-INRIA-IMAG">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer    - INRIA-IMAG variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="HPND-Kevlin-Henney">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - Kevlin Henney variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HPND-Markus-Kuhn">
         <xs:annotation>
           <xs:documentation>Historical Permission Notice and Disclaimer - Markus Kuhn variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-MIT-disclaimer">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer with MIT disclaimer</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="HPND-Pbmplus">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - Pbmplus variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="HPND-sell-MIT-disclaimer-xserver">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - sell xserver variant with MIT disclaimer</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="HPND-sell-regexpr">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - sell regexpr variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HPND-sell-variant">
         <xs:annotation>
           <xs:documentation>Historical Permission Notice and Disclaimer - sell variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="HPND-sell-variant-MIT-disclaimer">
         <xs:annotation>
           <xs:documentation>HPND sell variant with MIT disclaimer</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-UC">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - University of California variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HTMLTIDY">
         <xs:annotation>
           <xs:documentation>HTML Tidy License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="IBM-pibs">
         <xs:annotation>
@@ -1454,14 +1669,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="ISC">
         <xs:annotation>
           <xs:documentation>ISC License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="ISC-Veillard">
+        <xs:annotation>
+          <xs:documentation>ISC Veillard variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Jam">
         <xs:annotation>
           <xs:documentation>Jam License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="JasPer-2.0">
         <xs:annotation>
@@ -1479,14 +1699,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="JSON">
         <xs:annotation>
           <xs:documentation>JSON License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Kastrup">
+        <xs:annotation>
+          <xs:documentation>Kastrup License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Kazlib">
         <xs:annotation>
           <xs:documentation>Kazlib License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Knuth-CTAN">
         <xs:annotation>
@@ -1649,14 +1874,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="LOOP">
         <xs:annotation>
           <xs:documentation>Common Lisp LOOP License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="LPD-document">
+        <xs:annotation>
+          <xs:documentation>LPD Documentation License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="LPL-1.0">
         <xs:annotation>
           <xs:documentation>Lucent Public License Version 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="LPL-1.02">
         <xs:annotation>
@@ -1684,34 +1914,69 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="LPPL-1.3c">
         <xs:annotation>
           <xs:documentation>LaTeX Project Public License v1.3c</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="lsof">
+        <xs:annotation>
+          <xs:documentation>lsof License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="Lucida-Bitmap-Fonts">
+        <xs:annotation>
+          <xs:documentation>Lucida Bitmap Fonts License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="LZMA-SDK-9.11-to-9.20">
         <xs:annotation>
           <xs:documentation>LZMA SDK License (versions 9.11 to 9.20)</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="LZMA-SDK-9.22">
         <xs:annotation>
           <xs:documentation>LZMA SDK License (versions 9.22 and beyond)</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Mackerras-3-Clause">
+        <xs:annotation>
+          <xs:documentation>Mackerras 3-Clause License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="Mackerras-3-Clause-acknowledgment">
+        <xs:annotation>
+          <xs:documentation>Mackerras 3-Clause - acknowledgment variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="magaz">
+        <xs:annotation>
+          <xs:documentation>magaz License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="mailprio">
+        <xs:annotation>
+          <xs:documentation>mailprio License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="MakeIndex">
         <xs:annotation>
           <xs:documentation>MakeIndex License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Martin-Birgmeier">
         <xs:annotation>
           <xs:documentation>Martin Birgmeier License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="McPhee-slideshow">
+        <xs:annotation>
+          <xs:documentation>McPhee Slideshow License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="metamail">
         <xs:annotation>
           <xs:documentation>metamail License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Minpack">
         <xs:annotation>
@@ -1764,29 +2029,44 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="MIT-open-group">
         <xs:annotation>
           <xs:documentation>MIT Open Group variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="MIT-testregex">
+        <xs:annotation>
+          <xs:documentation>MIT testregex Variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="MIT-Wu">
         <xs:annotation>
           <xs:documentation>MIT Tom Wu Variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="MITNFA">
         <xs:annotation>
           <xs:documentation>MIT +no-false-attribs license</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="MMIXware">
+        <xs:annotation>
+          <xs:documentation>MMIXware License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Motosoto">
         <xs:annotation>
           <xs:documentation>Motosoto License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="MPEG-SSG">
+        <xs:annotation>
+          <xs:documentation>MPEG Software Simulation</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="mpi-permissive">
         <xs:annotation>
           <xs:documentation>mpi Permissive License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="mpich2">
         <xs:annotation>
@@ -2184,14 +2464,24 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="OpenSSL">
         <xs:annotation>
           <xs:documentation>OpenSSL License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="OpenSSL-standalone">
+        <xs:annotation>
+          <xs:documentation>OpenSSL License - standalone</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="OpenVision">
+        <xs:annotation>
+          <xs:documentation>OpenVision License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="OPL-1.0">
         <xs:annotation>
           <xs:documentation>Open Public License v1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="OPL-UK-3.0">
         <xs:annotation>
@@ -2229,14 +2519,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="OSL-3.0">
         <xs:annotation>
           <xs:documentation>Open Software License 3.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="PADL">
+        <xs:annotation>
+          <xs:documentation>PADL License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Parity-6.0.0">
         <xs:annotation>
           <xs:documentation>The Parity Public License 6.0.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Parity-7.0.0">
         <xs:annotation>
@@ -2254,19 +2549,29 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="PHP-3.01">
         <xs:annotation>
           <xs:documentation>PHP License v3.01</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Pixar">
+        <xs:annotation>
+          <xs:documentation>Pixar License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Plexus">
         <xs:annotation>
           <xs:documentation>Plexus Classworlds License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="pnmstitch">
+        <xs:annotation>
+          <xs:documentation>pnmstitch License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="PolyForm-Noncommercial-1.0.0">
         <xs:annotation>
           <xs:documentation>PolyForm Noncommercial License 1.0.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="PolyForm-Small-Business-1.0.0">
         <xs:annotation>
@@ -2299,14 +2604,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Python-2.0.1">
         <xs:annotation>
           <xs:documentation>Python License 2.0.1</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="python-ldap">
+        <xs:annotation>
+          <xs:documentation>Python ldap License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Qhull">
         <xs:annotation>
           <xs:documentation>Qhull License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="QPL-1.0">
         <xs:annotation>
@@ -2314,14 +2624,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="QPL-1.0-INRIA-2004">
         <xs:annotation>
           <xs:documentation>Q Public License 1.0 - INRIA 2004 variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="radvd">
+        <xs:annotation>
+          <xs:documentation>radvd License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Rdisc">
         <xs:annotation>
           <xs:documentation>Rdisc License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="RHeCos-1.1">
         <xs:annotation>
@@ -2359,14 +2674,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SAX-PD">
         <xs:annotation>
           <xs:documentation>Sax Public Domain Notice</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="SAX-PD-2.0">
+        <xs:annotation>
+          <xs:documentation>Sax Public Domain Notice 2.0</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Saxpath">
         <xs:annotation>
           <xs:documentation>Saxpath License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SCEA">
         <xs:annotation>
@@ -2399,14 +2719,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SGI-B-2.0">
         <xs:annotation>
           <xs:documentation>SGI Free Software License B v2.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="SGI-OpenGL">
+        <xs:annotation>
+          <xs:documentation>SGI OpenGL License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="SGP4">
         <xs:annotation>
           <xs:documentation>SGP4 Permission Notice</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SHL-0.5">
         <xs:annotation>
@@ -2429,14 +2754,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SISSL-1.2">
         <xs:annotation>
           <xs:documentation>Sun Industry Standards Source License v1.2</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="SL">
+        <xs:annotation>
+          <xs:documentation>SL License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Sleepycat">
         <xs:annotation>
           <xs:documentation>Sleepycat License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SMLNJ">
         <xs:annotation>
@@ -2454,14 +2784,24 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="snprintf">
         <xs:annotation>
           <xs:documentation>snprintf License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="softSurfer">
+        <xs:annotation>
+          <xs:documentation>softSurfer License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="Soundex">
+        <xs:annotation>
+          <xs:documentation>Soundex License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Spencer-86">
         <xs:annotation>
           <xs:documentation>Spencer License 86</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Spencer-94">
         <xs:annotation>
@@ -2474,24 +2814,34 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SPL-1.0">
         <xs:annotation>
           <xs:documentation>Sun Public License v1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="ssh-keyscan">
+        <xs:annotation>
+          <xs:documentation>ssh-keyscan License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="SSH-OpenSSH">
         <xs:annotation>
           <xs:documentation>SSH OpenSSH license</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SSH-short">
         <xs:annotation>
           <xs:documentation>SSH short notice</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="SSLeay-standalone">
+        <xs:annotation>
+          <xs:documentation>SSLeay License - standalone</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="SSPL-1.0">
         <xs:annotation>
           <xs:documentation>Server Side Public License, v 1</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="StandardML-NJ">
         <xs:annotation>
@@ -2499,24 +2849,34 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SugarCRM-1.1.3">
         <xs:annotation>
           <xs:documentation>SugarCRM Public License v1.1.3</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Sun-PPP">
+        <xs:annotation>
+          <xs:documentation>Sun PPP License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="SunPro">
         <xs:annotation>
           <xs:documentation>SunPro License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SWL">
         <xs:annotation>
           <xs:documentation>Scheme Widget Library (SWL) Software License Agreement</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="swrule">
+        <xs:annotation>
+          <xs:documentation>swrule License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Symlinks">
         <xs:annotation>
           <xs:documentation>Symlinks License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="TAPR-OHL-1.0">
         <xs:annotation>
@@ -2534,14 +2894,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="TermReadKey">
         <xs:annotation>
           <xs:documentation>TermReadKey License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="TGPPL-1.0">
+        <xs:annotation>
+          <xs:documentation>Transitive Grace Period Public Licence 1.0</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="TMate">
         <xs:annotation>
           <xs:documentation>TMate Open Source License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="TORQUE-1.1">
         <xs:annotation>
@@ -2564,14 +2929,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="TTWL">
         <xs:annotation>
           <xs:documentation>Text-Tabs+Wrap License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="TTYP0">
+        <xs:annotation>
+          <xs:documentation>TTYP0 License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="TU-Berlin-1.0">
         <xs:annotation>
           <xs:documentation>Technische Universitaet Berlin License 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="TU-Berlin-2.0">
         <xs:annotation>
@@ -2584,14 +2954,29 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="UCL-1.0">
         <xs:annotation>
           <xs:documentation>Upstream Compatibility License v1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="ulem">
+        <xs:annotation>
+          <xs:documentation>ulem License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="UMich-Merit">
+        <xs:annotation>
+          <xs:documentation>Michigan/Merit Networks License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="Unicode-3.0">
+        <xs:annotation>
+          <xs:documentation>Unicode License v3</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Unicode-DFS-2015">
         <xs:annotation>
           <xs:documentation>Unicode License Agreement - Data Files and Software (2015)</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Unicode-DFS-2016">
         <xs:annotation>
@@ -2614,14 +2999,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="UPL-1.0">
         <xs:annotation>
           <xs:documentation>Universal Permissive License v1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="URT-RLE">
+        <xs:annotation>
+          <xs:documentation>Utah Raster Toolkit Run Length Encoded License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Vim">
         <xs:annotation>
           <xs:documentation>Vim License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="VOSTROM">
         <xs:annotation>
@@ -2709,14 +3099,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="xinetd">
         <xs:annotation>
           <xs:documentation>xinetd License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="xkeyboard-config-Zinoviev">
+        <xs:annotation>
+          <xs:documentation>xkeyboard-config Zinoviev License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="xlock">
         <xs:annotation>
           <xs:documentation>xlock License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Xnet">
         <xs:annotation>
@@ -2744,14 +3139,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Zed">
         <xs:annotation>
           <xs:documentation>Zed License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Zeeff">
+        <xs:annotation>
+          <xs:documentation>Zeeff License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Zend-2.0">
         <xs:annotation>
           <xs:documentation>Zend License v2.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Zimbra-1.3">
         <xs:annotation>
@@ -2810,19 +3210,29 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Autoconf-exception-generic">
         <xs:annotation>
           <xs:documentation>Autoconf generic exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Autoconf-exception-generic-3.0">
+        <xs:annotation>
+          <xs:documentation>Autoconf generic exception for GPL-3.0</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Autoconf-exception-macro">
         <xs:annotation>
           <xs:documentation>Autoconf macro exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Bison-exception-1.24">
+        <xs:annotation>
+          <xs:documentation>Bison exception 1.24</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Bison-exception-2.2">
         <xs:annotation>
           <xs:documentation>Bison exception 2.2</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Bootloader-exception">
         <xs:annotation>
@@ -2860,14 +3270,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="FLTK-exception">
         <xs:annotation>
           <xs:documentation>FLTK exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="fmt-exception">
+        <xs:annotation>
+          <xs:documentation>fmt exception</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Font-exception-2.0">
         <xs:annotation>
           <xs:documentation>Font exception 2.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="freertos-exception-2.0">
         <xs:annotation>
@@ -2875,24 +3290,44 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="GCC-exception-2.0">
         <xs:annotation>
           <xs:documentation>GCC Runtime Library exception 2.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="GCC-exception-2.0-note">
+        <xs:annotation>
+          <xs:documentation>GCC    Runtime Library exception 2.0 - note variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="GCC-exception-3.1">
         <xs:annotation>
           <xs:documentation>GCC Runtime Library exception 3.1</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Gmsh-exception">
+        <xs:annotation>
+          <xs:documentation>Gmsh exception&gt;</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="GNAT-exception">
         <xs:annotation>
           <xs:documentation>GNAT exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="GNOME-examples-exception">
+        <xs:annotation>
+          <xs:documentation>GNOME examples exception</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="GNU-compiler-exception">
+        <xs:annotation>
+          <xs:documentation>GNU Compiler Exception</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="gnu-javamail-exception">
         <xs:annotation>
           <xs:documentation>GNU JavaMail exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="GPL-3.0-interface-exception">
         <xs:annotation>
@@ -3020,39 +3455,59 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Qwt-exception-1.0">
         <xs:annotation>
           <xs:documentation>Qwt exception 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="SANE-exception">
+        <xs:annotation>
+          <xs:documentation>SANE Exception</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="SHL-2.0">
         <xs:annotation>
           <xs:documentation>Solderpad Hardware License v2.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SHL-2.1">
         <xs:annotation>
           <xs:documentation>Solderpad Hardware License v2.1</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="stunnel-exception">
+        <xs:annotation>
+          <xs:documentation>stunnel Exception</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="SWI-exception">
         <xs:annotation>
           <xs:documentation>SWI exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Swift-exception">
         <xs:annotation>
           <xs:documentation>Swift Exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Texinfo-exception">
+        <xs:annotation>
+          <xs:documentation>Texinfo exception</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="u-boot-exception-2.0">
         <xs:annotation>
           <xs:documentation>U-Boot exception 2.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="UBDL-exception">
+        <xs:annotation>
+          <xs:documentation>Unmodified Binary Distribution exception</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Universal-FOSS-exception-1.0">
         <xs:annotation>
           <xs:documentation>Universal FOSS Exception, Version 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="vsftpd-openssl-exception">
         <xs:annotation>
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/schema/schema.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/schema/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,21 @@
     def schema_version_enum(self) -> SchemaVersion:
         ...
 
     def get_schema_version(self) -> str:
         return self.schema_version_enum.to_version()
 
 
+class SchemaVersion1Dot6(BaseSchemaVersion):
+
+    @property
+    def schema_version_enum(self) -> Literal[SchemaVersion.V1_6]:
+        return SchemaVersion.V1_6
+
+
 class SchemaVersion1Dot5(BaseSchemaVersion):
 
     @property
     def schema_version_enum(self) -> Literal[SchemaVersion.V1_5]:
         return SchemaVersion.V1_5
 
 
@@ -73,14 +80,15 @@
 
     @property
     def schema_version_enum(self) -> Literal[SchemaVersion.V1_0]:
         return SchemaVersion.V1_0
 
 
 SCHEMA_VERSIONS: Dict[SchemaVersion, Type[BaseSchemaVersion]] = {
+    SchemaVersion.V1_6: SchemaVersion1Dot6,
     SchemaVersion.V1_5: SchemaVersion1Dot5,
     SchemaVersion.V1_4: SchemaVersion1Dot4,
     SchemaVersion.V1_3: SchemaVersion1Dot3,
     SchemaVersion.V1_2: SchemaVersion1Dot2,
     SchemaVersion.V1_1: SchemaVersion1Dot1,
     SchemaVersion.V1_0: SchemaVersion1Dot0,
 }
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/serialization/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/serialization/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         if len(o) == 0:
             return None
         expression = next((li for li in o if isinstance(li, LicenseExpression)), None)
         if expression:
             # mixed license expression and license? this is an invalid constellation according to schema!
             # see https://github.com/CycloneDX/specification/pull/205
             # but models need to allow it for backwards compatibility with JSON CDX < 1.5
-            return [{'expression': str(expression.value)}]
+            return [json_loads(expression.as_json(view_=view))]  # type:ignore[attr-defined]
         return [
             {'license': json_loads(
                 li.as_json(  # type:ignore[attr-defined]
                     view_=view)
             )}
             for li in o
             if isinstance(li, DisjunctiveLicense)
@@ -119,15 +119,17 @@
                          **__: Any) -> LicenseRepository:
         repo = LicenseRepository()
         for li in o:
             if 'license' in li:
                 repo.add(DisjunctiveLicense.from_json(  # type:ignore[attr-defined]
                     li['license']))
             elif 'expression' in li:
-                repo.add(LicenseExpression(li['expression']))
+                repo.add(LicenseExpression.from_json(  # type:ignore[attr-defined]
+                    li
+                ))
             else:
                 raise CycloneDxDeserializationException(f'unexpected: {li!r}')
         return repo
 
     @classmethod
     def xml_normalize(cls, o: LicenseRepository, *,
                       element_name: str,
```

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/spdx.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/validation/__init__.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/validation/json.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/validation/model.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/cyclonedx/validation/xml.py` & `cyclonedx_python_lib-7.0.0a1/cyclonedx/validation/xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/Makefile` & `cyclonedx_python_lib-7.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/architecture.rst` & `cyclonedx_python_lib-7.0.0a1/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/changelog.rst` & `cyclonedx_python_lib-7.0.0a1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/conf.py` & `cyclonedx_python_lib-7.0.0a1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 project = 'CycloneDX Python Library'
 copyright = '2022, Copyright (c) OWASP Foundation'
 author = 'Paul Horton, Jan Kowalleck, Steve Springett, Patrick Dwyer'
 
 # The full version, including alpha/beta/rc tags
 # !! version is managed by semantic_release
-release = '6.4.4'
+release = '7.0.0-alpha.1'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `cyclonedx_python_lib-6.4.4/docs/examples.rst` & `cyclonedx_python_lib-7.0.0a1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/index.rst` & `cyclonedx_python_lib-7.0.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/install.rst` & `cyclonedx_python_lib-7.0.0a1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/make.bat` & `cyclonedx_python_lib-7.0.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/modelling.rst` & `cyclonedx_python_lib-7.0.0a1/docs/modelling.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/outputting.rst` & `cyclonedx_python_lib-7.0.0a1/docs/outputting.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/schema-support.rst` & `cyclonedx_python_lib-7.0.0a1/docs/schema-support.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/docs/support.rst` & `cyclonedx_python_lib-7.0.0a1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/examples/complex_deserialize.py` & `cyclonedx_python_lib-7.0.0a1/examples/complex_deserialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 if TYPE_CHECKING:
     from cyclonedx.validation.xml import XmlValidator
 
 # region JSON
 
 json_data = """{
-  "$schema": "http://cyclonedx.org/schema/bom-1.5.schema.json",
+  "$schema": "http://cyclonedx.org/schema/bom-1.6.schema.json",
   "bomFormat": "CycloneDX",
-  "specVersion": "1.5",
+  "specVersion": "1.6",
   "serialNumber": "urn:uuid:88fabcfa-7529-4ba2-8256-29bec0c03900",
   "version": 1,
   "metadata": {
     "timestamp": "2024-02-10T21:38:53.313120+00:00",
     "tools": [
       {
         "vendor": "CycloneDX",
@@ -141,15 +141,15 @@
       "dependsOn": [
         "some-lib"
       ],
       "ref": "myComponent@1.33.7-beta.1"
     }
   ]
 }"""
-my_json_validator = JsonStrictValidator(SchemaVersion.V1_5)
+my_json_validator = JsonStrictValidator(SchemaVersion.V1_6)
 try:
     validation_errors = my_json_validator.validate_str(json_data)
     if validation_errors:
         print('JSON invalid', 'ValidationError:', repr(validation_errors), sep='\n', file=sys.stderr)
         sys.exit(2)
     print('JSON valid')
 except MissingOptionalDependencyException as error:
@@ -161,15 +161,15 @@
 # endregion JSON
 
 print('', '=' * 30, '', sep='\n')
 
 # endregion XML
 
 xml_data = """<?xml version="1.0" ?>
-<bom xmlns="http://cyclonedx.org/schema/bom/1.5"
+<bom xmlns="http://cyclonedx.org/schema/bom/1.6"
   serialNumber="urn:uuid:88fabcfa-7529-4ba2-8256-29bec0c03900"
   version="1"
 >
   <metadata>
     <timestamp>2024-02-10T21:38:53.313120+00:00</timestamp>
     <tools>
       <tool>
@@ -242,15 +242,15 @@
       <dependency ref="myComponent@1.33.7-beta.1"/>
     </dependency>
     <dependency ref="myComponent@1.33.7-beta.1">
       <dependency ref="some-lib"/>
     </dependency>
   </dependencies>
 </bom>"""
-my_xml_validator: 'XmlValidator' = make_schemabased_validator(OutputFormat.XML, SchemaVersion.V1_5)
+my_xml_validator: 'XmlValidator' = make_schemabased_validator(OutputFormat.XML, SchemaVersion.V1_6)
 try:
     validation_errors = my_xml_validator.validate_str(xml_data)
     if validation_errors:
         print('XML invalid', 'ValidationError:', repr(validation_errors), sep='\n', file=sys.stderr)
         sys.exit(2)
     print('XML valid')
 except MissingOptionalDependencyException as error:
```

### Comparing `cyclonedx_python_lib-6.4.4/examples/complex_serialize.py` & `cyclonedx_python_lib-7.0.0a1/examples/complex_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 import sys
 from typing import TYPE_CHECKING
 
 from packageurl import PackageURL
 
 from cyclonedx.exception import MissingOptionalDependencyException
 from cyclonedx.factory.license import LicenseFactory
-from cyclonedx.model import OrganizationalEntity, XsUri
+from cyclonedx.model import XsUri
 from cyclonedx.model.bom import Bom
 from cyclonedx.model.component import Component, ComponentType
+from cyclonedx.model.contact import OrganizationalEntity
 from cyclonedx.output import make_outputter
 from cyclonedx.output.json import JsonV1Dot5
 from cyclonedx.schema import OutputFormat, SchemaVersion
 from cyclonedx.validation import make_schemabased_validator
 from cyclonedx.validation.json import JsonStrictValidator
 
 if TYPE_CHECKING:
@@ -77,15 +78,15 @@
 
 # region JSON
 """demo with explicit instructions for SchemaVersion, outputter and validator"""
 
 my_json_outputter: 'JsonOutputter' = JsonV1Dot5(bom)
 serialized_json = my_json_outputter.output_as_string(indent=2)
 print(serialized_json)
-my_json_validator = JsonStrictValidator(SchemaVersion.V1_5)
+my_json_validator = JsonStrictValidator(SchemaVersion.V1_6)
 try:
     validation_errors = my_json_validator.validate_str(serialized_json)
     if validation_errors:
         print('JSON invalid', 'ValidationError:', repr(validation_errors), sep='\n', file=sys.stderr)
         sys.exit(2)
     print('JSON valid')
 except MissingOptionalDependencyException as error:
@@ -94,15 +95,15 @@
 # endregion JSON
 
 print('', '=' * 30, '', sep='\n')
 
 # region XML
 """demo with implicit instructions for SchemaVersion, outputter and validator. TypeCheckers will catch errors."""
 
-my_xml_outputter: 'XmlOutputter' = make_outputter(bom, OutputFormat.XML, SchemaVersion.V1_5)
+my_xml_outputter: 'XmlOutputter' = make_outputter(bom, OutputFormat.XML, SchemaVersion.V1_6)
 serialized_xml = my_xml_outputter.output_as_string(indent=2)
 print(serialized_xml)
 my_xml_validator: 'XmlValidator' = make_schemabased_validator(
     my_xml_outputter.output_format, my_xml_outputter.schema_version)
 try:
     validation_errors = my_xml_validator.validate_str(serialized_xml)
     if validation_errors:
```

### Comparing `cyclonedx_python_lib-6.4.4/pyproject.toml` & `cyclonedx_python_lib-7.0.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cyclonedx-python-lib"
 # !! version is managed by semantic_release
-version = "6.4.4"
+version = "7.0.0-alpha.1"
 description = "Python library for CycloneDX"
 authors = [
   "Paul Horton <phorton@sonatype.com>",
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
 ]
 maintainers = [
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
@@ -65,15 +65,15 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/CycloneDX/cyclonedx-python-lib/issues"
 "Funding" = "https://owasp.org/donate/?reponame=www-project-cyclonedx&title=OWASP+CycloneDX"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 packageurl-python = ">=0.11, <2"
-py-serializable =  ">=0.16, <2"
+py-serializable =  ">=1.0.3, <2"
 sortedcontainers = "^2.4.0"
 license-expression = "^30"
 jsonschema = { version = "^4.18", extras=['format'], optional=true }
 lxml = { version=">=4,<6", optional=true }
 
 [tool.poetry.extras]
 validation = ["jsonschema", "lxml"]
@@ -87,17 +87,17 @@
 flake8-annotations = { version="3.0.1", python=">=3.8.1" }
 flake8-bugbear = { version="24.2.6", python=">=3.8.1" }
 flake8-isort = "6.1.1"
 flake8-quotes = "3.4.0"
 flake8-use-fstring = "1.4"
 pep8-naming = "0.13.3"
 isort = "5.13.2"
-autopep8 = "2.0.4"
+autopep8 = "2.1.0"
 mypy = "1.9.0"
-tox = "4.14.1"
+tox = "4.14.2"
 xmldiff = "2.6.3"
 bandit = "1.7.8"
 
 [tool.semantic_release]
 # see https://python-semantic-release.readthedocs.io/en/latest/configuration.html
 commit_author = "semantic-release <semantic-release>"
 commit_message = "chore(release): {version}\n\nAutomatically generated by python-semantic-release\n\nSigned-off-by: semantic-release <semantic-release>"
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/__init__.py` & `cyclonedx_python_lib-7.0.0a1/tests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright (c) OWASP Foundation. All Rights Reserved.
-
+import re
 from os import getenv, path
 from os.path import join
 from typing import TYPE_CHECKING, Any, Generator, Iterable, List, Optional, TypeVar, Union
 from unittest import TestCase
 from uuid import UUID
 
 from sortedcontainers import SortedSet
@@ -155,11 +155,31 @@
 
 
 _SNAME_EXT = {
     OutputFormat.JSON: 'json',
     OutputFormat.XML: 'xml',
 }
 
+_LIMIT_GET_BOM_BY_VERSION_REGEX = re.compile(r'^get_bom_(?P<sv>v(?P<major_version>1)_(?P<minor_version>[0-6]))?(.*)$')
+
+
+def _get_purpose_as_str(purpose: Union[Any]) -> str:
+    return purpose if isinstance(purpose, str) else purpose.__name__
+
+
+def is_valid_for_schema_version(purpose: Union[Any], sv: SchemaVersion) -> bool:
+    restrict_to_schema = _LIMIT_GET_BOM_BY_VERSION_REGEX.match(_get_purpose_as_str(purpose))
+
+    if restrict_to_schema:
+        mg = restrict_to_schema.groupdict()
+        if mg.get('sv') is not None:
+            restricted_to_sv = SchemaVersion.from_version(f'{mg.get("major_version")}.{mg.get("minor_version")}')
+            if sv >= restricted_to_sv:
+                return True
+            else:
+                return False
+
+    return True
+
 
 def mksname(purpose: Union[Any], sv: SchemaVersion, f: OutputFormat) -> str:
-    purpose = purpose if isinstance(purpose, str) else purpose.__name__
-    return f'{purpose}-{sv.to_version()}.{_SNAME_EXT[f]}'
+    return f'{_get_purpose_as_str(purpose)}-{sv.to_version()}.{_SNAME_EXT[f]}'
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/__init__.py` & `cyclonedx_python_lib-7.0.0a1/tests/_data/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/models.py` & `cyclonedx_python_lib-7.0.0a1/tests/_data/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,43 +33,64 @@
     DataFlow,
     Encoding,
     ExternalReference,
     ExternalReferenceType,
     HashType,
     Note,
     NoteText,
-    OrganizationalContact,
-    OrganizationalEntity,
     Property,
     Tool,
     XsUri,
 )
 from cyclonedx.model.bom import Bom, BomMetaData
 from cyclonedx.model.bom_ref import BomRef
 from cyclonedx.model.component import (
     Commit,
     Component,
     ComponentEvidence,
     ComponentScope,
     ComponentType,
     Diff,
+    OmniborId,
     Patch,
     PatchClassification,
     Pedigree,
+    Swhid,
     Swid,
 )
+from cyclonedx.model.contact import OrganizationalContact, OrganizationalEntity, PostalAddress
+from cyclonedx.model.crypto import (
+    AlgorithmProperties,
+    CertificateProperties,
+    CryptoAssetType,
+    CryptoCertificationLevel,
+    CryptoExecutionEnvironment,
+    CryptoFunction,
+    CryptoImplementationPlatform,
+    CryptoMode,
+    CryptoPadding,
+    CryptoPrimitive,
+    CryptoProperties,
+    ProtocolProperties,
+    ProtocolPropertiesCipherSuite,
+    ProtocolPropertiesType,
+    RelatedCryptoMaterialProperties,
+    RelatedCryptoMaterialSecuredBy,
+    RelatedCryptoMaterialState,
+    RelatedCryptoMaterialType,
+)
 from cyclonedx.model.dependency import Dependency
 from cyclonedx.model.impact_analysis import (
     ImpactAnalysisAffectedStatus,
     ImpactAnalysisJustification,
     ImpactAnalysisResponse,
     ImpactAnalysisState,
 )
 from cyclonedx.model.issue import IssueClassification, IssueType, IssueTypeSource
-from cyclonedx.model.license import DisjunctiveLicense, License, LicenseExpression
+from cyclonedx.model.license import DisjunctiveLicense, License, LicenseExpression, LicenseExpressionAcknowledgement
 from cyclonedx.model.release_note import ReleaseNotes
 from cyclonedx.model.service import Service
 from cyclonedx.model.vulnerability import (
     BomTarget,
     BomTargetVersionRange,
     Vulnerability,
     VulnerabilityAdvisory,
@@ -121,14 +142,248 @@
 
 def get_bom_with_component_setuptools_with_cpe() -> Bom:
     component = get_component_setuptools_simple()
     component.cpe = 'cpe:2.3:a:python:setuptools:50.3.2:*:*:*:*:*:*:*'
     return _make_bom(components=[component])
 
 
+def get_crypto_properties_algorithm() -> CryptoProperties:
+    return CryptoProperties(
+        asset_type=CryptoAssetType.ALGORITHM,
+        algorithm_properties=AlgorithmProperties(
+            primitive=CryptoPrimitive.KEM,
+            parameter_set_identifier='a-parameter-set-id',
+            curve='9n8y2oxty3ao83n8qc2g2x3qcw4jt4wj',
+            execution_environment=CryptoExecutionEnvironment.SOFTWARE_PLAIN_RAM,
+            implementation_platform=CryptoImplementationPlatform.GENERIC,
+            certification_levels=[
+                CryptoCertificationLevel.FIPS140_1_L1,
+                CryptoCertificationLevel.FIPS140_2_L3,
+                CryptoCertificationLevel.OTHER
+            ],
+            mode=CryptoMode.ECB,
+            padding=CryptoPadding.PKCS7,
+            crypto_functions=[
+                CryptoFunction.SIGN,
+                CryptoFunction.UNKNOWN
+            ],
+            classical_security_level=2,
+            nist_quantum_security_level=2
+        ),
+        oid='an-oid-here'
+    )
+
+
+def get_crypto_properties_certificate() -> CryptoProperties:
+    return CryptoProperties(
+        asset_type=CryptoAssetType.CERTIFICATE,
+        certificate_properties=CertificateProperties(
+            subject_name='cyclonedx.org',
+            issuer_name='Cloudflare Inc ECC CA-3',
+            not_valid_before=datetime(year=2023, month=5, day=19, hour=1, minute=0, second=0, microsecond=0,
+                                      tzinfo=timezone.utc),
+            not_valid_after=datetime(year=2024, month=5, day=19, hour=0, minute=59, second=59, microsecond=999999,
+                                     tzinfo=timezone.utc),
+            signature_algorithm_ref=None,
+            subject_public_key_ref=None,
+            certificate_format='pem',
+            certificate_extension='csr'
+        ),
+        oid='an-oid-here'
+    )
+
+
+def get_crypto_properties_protocol() -> CryptoProperties:
+    return CryptoProperties(
+        asset_type=CryptoAssetType.PROTOCOL,
+        protocol_properties=ProtocolProperties(
+            type=ProtocolPropertiesType.TLS,
+            version='1.3',
+            cipher_suites=[
+                ProtocolPropertiesCipherSuite(
+                    name='TLS_AES_128_GCM_SHA256',
+                    algorithms=None,
+                    identifiers=[
+                        'TLS_AES_128_GCM_SHA256'
+                    ]
+                ),
+                ProtocolPropertiesCipherSuite(
+                    name='TLS_AES_256_GCM_SHA384',
+                    algorithms=None,
+                    identifiers=[
+                        'TLS_AES_256_GCM_SHA384'
+                    ]
+                ),
+                ProtocolPropertiesCipherSuite(
+                    name='TLS_CHACHA20_POLY1305_SHA256',
+                    algorithms=None,
+                    identifiers=[
+                        'TLS_CHACHA20_POLY1305_SHA256'
+                    ]
+                ),
+                ProtocolPropertiesCipherSuite(
+                    name='TLS_AES_128_CCM_SHA256',
+                    algorithms=None,
+                    identifiers=[
+                        'TLS_AES_128_CCM_SHA256'
+                    ]
+                ),
+                ProtocolPropertiesCipherSuite(
+                    name='TLS_AES_128_CCM_8_SHA256',
+                    algorithms=None,
+                    identifiers=[
+                        'TLS_AES_128_CCM_8_SHA256'
+                    ]
+                )
+            ],
+        ),
+        oid='an-oid-here'
+    )
+
+
+def get_crypto_properties_related_material() -> CryptoProperties:
+    return CryptoProperties(
+        asset_type=CryptoAssetType.RELATED_CRYPTO_MATERIAL,
+        related_crypto_material_properties=RelatedCryptoMaterialProperties(
+            type=RelatedCryptoMaterialType.DIGEST,
+            id='some-identifier',
+            state=RelatedCryptoMaterialState.ACTIVE,
+            algorithm_ref=None,
+            creation_date=datetime(year=2023, month=5, day=19, hour=1, minute=0, second=0, microsecond=0,
+                                   tzinfo=timezone.utc),
+            activation_date=datetime(year=2023, month=5, day=19, hour=1, minute=0, second=0, microsecond=0,
+                                     tzinfo=timezone.utc),
+            update_date=None,
+            expiration_date=datetime(year=2024, month=5, day=19, hour=0, minute=59, second=59, microsecond=999999,
+                                     tzinfo=timezone.utc),
+            value='some-random-value',
+            size=32,
+            format='a-format',
+            secured_by=RelatedCryptoMaterialSecuredBy(
+                mechanism='hard-work',
+                algorithm_ref=None
+            )
+        ),
+        oid='an-oid-here'
+    )
+
+
+def get_bom_with_component_setuptools_with_v16_fields() -> Bom:
+    component = get_component_setuptools_simple()
+    component.manufacturer = get_org_entity_1()
+    component.authors = [get_org_contact_1(), get_org_contact_2()]
+    component.omnibor_ids = [OmniborId('gitoid:blob:sha1:261eeb9e9f8b2b4b0d119366dda99c6fd7d35c64')]
+    component.swhids = [
+        Swhid('swh:1:cnt:94a9ed024d3859793618152ea559a168bbcbb5e2'),
+        Swhid('swh:1:rel:22ece559cc7cc2364edc5e5593d63ae8bd229f9f'),
+        Swhid('swh:1:cnt:4d99d2d18326621ccdd70f5ea66c2e2ac236ad8b;'
+              'origin=https://gitorious.org/ocamlp3l/ocamlp3l_cvs.git;'
+              'visit=swh:1:snp:d7f1b9eb7ccb596c2622c4780febaa02549830f9;'
+              'anchor=swh:1:rev:2db189928c94d62a3b4757b3eec68f0a4d4113f0;'
+              'path=/Examples/SimpleFarm/simplefarm.ml;lines=9-15'),
+        Swhid('swh:1:cnt:f10371aa7b8ccabca8479196d6cd640676fd4a04;origin=https://github.com/web-platform-tests/wpt;'
+              'visit=swh:1:snp:b37d435721bbd450624165f334724e3585346499;'
+              'anchor=swh:1:rev:259d0612af038d14f2cd889a14a3adb6c9e96d96;'
+              'path=/html/semantics/document-metadata/the-meta-element/pragma-directives/attr-meta-http-equiv-refresh/'
+              'support/x%3Burl=foo/')
+    ]
+    return _make_bom(components=[component])
+
+
+def get_bom_with_component_setuptools_with_v16_fields_omnibor_id_invalid() -> Bom:
+    component = get_component_setuptools_simple()
+    component.manufacturer = get_org_entity_1()
+    component.authors = [get_org_contact_1(), get_org_contact_2()]
+    component.omnibor_ids = [OmniborId('gitoid:stuff:sha1:261eeb9e9f8b2b4b0d119366dda99c6fd7d35c64')]
+    return _make_bom(components=[component])
+
+
+def get_bom_with_component_setuptools_with_v16_fields_swhid_invalid() -> Bom:
+    component = get_component_setuptools_simple()
+    component.manufacturer = get_org_entity_1()
+    component.authors = [get_org_contact_1(), get_org_contact_2()]
+    component.omnibor_ids = [OmniborId('gitoid:blob:sha1:261eeb9e9f8b2b4b0d119366dda99c6fd7d35c64')]
+    component.swhids = [
+        Swhid('swh:1:cntp:94a9ed024d3859793618152ea559a168bbcbb5e2'),
+    ]
+    return _make_bom(components=[component])
+
+
+def get_component_crypto_asset_algorithm(
+    bom_ref: Optional[str] = '8182921e-0588-472e-b8f9-9c527c68f067'
+) -> Component:
+    return Component(
+        name='My Algorithm', version='1.0', type=ComponentType.CRYPTOGRAPHIC_ASSET,
+        bom_ref=bom_ref,
+        crypto_properties=get_crypto_properties_algorithm(),
+        tags=['algorithm']
+    )
+
+
+def get_component_crypto_asset_certificate(
+    bom_ref: Optional[str] = '1f4ed1e4-582a-4fa0-8c38-1b4facc16972'
+) -> Component:
+    return Component(
+        name='My Certificate', version='1.0', type=ComponentType.CRYPTOGRAPHIC_ASSET,
+        bom_ref=bom_ref,
+        crypto_properties=get_crypto_properties_certificate(),
+        tags=['certificate']
+    )
+
+
+def get_component_crypto_asset_protocol_tls_v13(
+    bom_ref: Optional[str] = '26b1ce0f-bec6-4bfe-9db1-03b75a4ed1ec'
+) -> Component:
+    return Component(
+        name='TLS', version='v1.3', type=ComponentType.CRYPTOGRAPHIC_ASSET,
+        bom_ref=bom_ref,
+        crypto_properties=get_crypto_properties_protocol(),
+        tags=['protocl', 'tls']
+    )
+
+
+def get_component_crypto_asset_related_material(
+    bom_ref: Optional[str] = '332b3cee-078c-4789-ab15-887565b6fac5'
+) -> Component:
+    return Component(
+        name='My Encrypted Thing', version='1.0', type=ComponentType.CRYPTOGRAPHIC_ASSET,
+        bom_ref=bom_ref,
+        crypto_properties=get_crypto_properties_related_material(),
+        tags=['encrypted', 'data']
+    )
+
+
+def get_bom_v1_6_with_crypto_algorithm() -> Bom:
+    c = get_component_crypto_asset_algorithm()
+    b = _make_bom(components=[c])
+    b.register_dependency(c)
+    return b
+
+
+def get_bom_v1_6_with_crypto_certificate() -> Bom:
+    c = get_component_crypto_asset_certificate()
+    b = _make_bom(components=[c])
+    b.register_dependency(c)
+    return b
+
+
+def get_bom_v1_6_with_crypto_protocol() -> Bom:
+    c = get_component_crypto_asset_protocol_tls_v13()
+    b = _make_bom(components=[c])
+    b.register_dependency(c)
+    return b
+
+
+def get_bom_v1_6_with_crypto_related_material() -> Bom:
+    c = get_component_crypto_asset_related_material()
+    b = _make_bom(components=[c])
+    b.register_dependency(c)
+    return b
+
+
 def get_bom_with_component_setuptools_no_component_version() -> Bom:
     return _make_bom(components=[get_component_setuptools_simple_no_version()])
 
 
 def get_bom_with_component_setuptools_with_release_notes() -> Bom:
     component = get_component_setuptools_simple()
     component.release_notes = get_release_notes()
@@ -262,15 +517,16 @@
     return _make_bom(components=[get_component_toml_with_hashes_with_references()])
 
 
 def get_bom_just_complete_metadata() -> Bom:
     bom = _make_bom()
     bom.metadata.authors = [get_org_contact_1(), get_org_contact_2()]
     bom.metadata.component = get_component_setuptools_complete()
-    bom.metadata.manufacture = get_org_entity_1()
+    bom.metadata.component.manufacturer = get_org_entity_1()
+    bom.metadata.manufacture = get_org_entity_1()  # Deprecated from v1.6 onwards
     bom.metadata.supplier = get_org_entity_2()
     bom.metadata.licenses = [DisjunctiveLicense(
         id='Apache-2.0',
         url=XsUri('https://www.apache.org/licenses/LICENSE-2.0.txt'),
         text=AttachedText(
             encoding=Encoding.BASE_64,
             content='VGVzdCBjb250ZW50IC0gdGhpcyBpcyBub3QgdGhlIEFwYWNoZSAyLjAgbGljZW5zZSE='
@@ -556,23 +812,34 @@
     return OrganizationalContact(name='Paul Horton', email='paul.horton@owasp.org')
 
 
 def get_org_contact_2() -> OrganizationalContact:
     return OrganizationalContact(name='A N Other', email='someone@somewhere.tld', phone='+44 (0)1234 567890')
 
 
+def get_postal_address_1() -> PostalAddress:
+    return PostalAddress(country='GB', region='England', locality='Cheshire', street_address='100 Main Street')
+
+
+def get_postal_address_2() -> PostalAddress:
+    return PostalAddress(country='US', region='Texas', locality='Austin', street_address='100 Yee-Ha Street',
+                         postal_code='12345', post_office_box_number='105a')
+
+
 def get_org_entity_1() -> OrganizationalEntity:
     return OrganizationalEntity(
-        name='CycloneDX', urls=[XsUri('https://cyclonedx.org')], contacts=[get_org_contact_1(), get_org_contact_2()]
+        name='CycloneDX', urls=[XsUri('https://cyclonedx.org'), XsUri('https://cyclonedx.org/docs')],
+        contacts=[get_org_contact_1(), get_org_contact_2()], address=get_postal_address_1()
     )
 
 
 def get_org_entity_2() -> OrganizationalEntity:
     return OrganizationalEntity(
-        name='Cyclone DX', urls=[XsUri('https://cyclonedx.org/')], contacts=[get_org_contact_2()]
+        name='Cyclone DX', urls=[XsUri('https://cyclonedx.org/')], contacts=[get_org_contact_2()],
+        address=get_postal_address_2()
     )
 
 
 def get_pedigree_1() -> Pedigree:
     return Pedigree(
         ancestors=[
             get_component_setuptools_simple(bom_ref='ccc8d7ee-4b9c-4750-aee0-a72585152291'),
@@ -675,23 +942,25 @@
         metadata=BomMetaData(
             licenses=[DisjunctiveLicense(id='CC-BY-1.0')],
             component=Component(name='app', type=ComponentType.APPLICATION, bom_ref='my-app',
                                 licenses=[DisjunctiveLicense(name='proprietary')])
         ),
         components=[
             Component(name='c-with-expression', type=ComponentType.LIBRARY, bom_ref='C1',
-                      licenses=[LicenseExpression(value='Apache-2.0 OR MIT')]),
+                      licenses=[LicenseExpression(value='Apache-2.0 OR MIT',
+                                                  acknowledgement=LicenseExpressionAcknowledgement.CONCLUDED)]),
             Component(name='c-with-SPDX', type=ComponentType.LIBRARY, bom_ref='C2',
                       licenses=[DisjunctiveLicense(id='Apache-2.0')]),
             Component(name='c-with-name', type=ComponentType.LIBRARY, bom_ref='C3',
                       licenses=[DisjunctiveLicense(name='(c) ACME Inc.')]),
         ],
         services=[
             Service(name='s-with-expression', bom_ref='S1',
-                    licenses=[LicenseExpression(value='Apache-2.0 OR MIT')]),
+                    licenses=[LicenseExpression(value='Apache-2.0 OR MIT',
+                                                acknowledgement=LicenseExpressionAcknowledgement.DECLARED)]),
             Service(name='s-with-SPDX', bom_ref='S2',
                     licenses=[DisjunctiveLicense(id='Apache-2.0')]),
             Service(name='s-with-name', bom_ref='S3',
                     licenses=[DisjunctiveLicense(name='(c) ACME Inc.')]),
         ])
 
 
@@ -833,8 +1102,9 @@
     get_bom_with_metadata_component_and_dependencies,
     get_bom_with_nested_services,
     get_bom_with_services_complex,
     get_bom_with_services_simple,
     get_bom_with_licenses,
     get_bom_with_multiple_licenses,
     get_bom_for_issue_497_urls,
+    get_bom_with_component_setuptools_with_v16_fields,
 }
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.2/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/json/1.2/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.3/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/json/1.3/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.4/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/json/1.4/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/own/xml/1.4/bom_setuptools.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/xml/1.4/bom_setuptools.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/own/xml/1.4/webgoat-6.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/own/xml/1.4/webgoat-6.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-bom-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-patch-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-1.2.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-service-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-service-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-bom-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-patch-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-properties-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-1.3.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-service-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-service-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-bom-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-patch-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-properties-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-service-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-service-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-bom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-patch-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-properties-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-service-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-service-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/fetch.sh` & `cyclonedx_python_lib-7.0.0a1/tests/_data/schemaTestData/fetch.sh`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 SOURCE_DIR='specification-master/tools/src/test/resources'
 
 THIS_DIR="$(dirname "$0")"
 TEMP_DIR="$(mktemp -d)"
 LOCAL_PACKAGE="$TEMP_DIR/source_package.zip"
 
 wget -O "$LOCAL_PACKAGE" "$SOURCE_PACKAGE"
-for SCHEMA_VERSION in '1.5' '1.4' '1.3' '1.2' '1.1' '1.0'
+for SCHEMA_VERSION in '1.6' '1.5' '1.4' '1.3' '1.2' '1.1' '1.0'
 do
   unzip -d "$TEMP_DIR" "$LOCAL_PACKAGE" "$SOURCE_DIR/$SCHEMA_VERSION/*"
   rm -rf "${THIS_DIR:?}/$SCHEMA_VERSION"
   mkdir -p "$THIS_DIR/$SCHEMA_VERSION"
   cp -rf "$TEMP_DIR/$SOURCE_DIR/$SCHEMA_VERSION/"*.xml "$THIS_DIR/$SCHEMA_VERSION/"
   cp -rf "$TEMP_DIR/$SOURCE_DIR/$SCHEMA_VERSION/"*.json "$THIS_DIR/$SCHEMA_VERSION/" || true
 done
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_Encoding-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin`

 * *Files 4% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin`

```diff
@@ -34,27 +34,33 @@
         </reference>
         <reference type="other">
           <url>tests/COMPONENT_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
           <url>tests/CONFIGURATION</url>
         </reference>
+        <reference type="other">
+          <url>tests/DIGITAL_SIGNATURE</url>
+        </reference>
         <reference type="distribution">
           <url>tests/DISTRIBUTION</url>
         </reference>
         <reference type="other">
           <url>tests/DISTRIBUTION_INTAKE</url>
         </reference>
         <reference type="documentation">
           <url>tests/DOCUMENTATION</url>
         </reference>
         <reference type="other">
           <url>tests/DYNAMIC_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
+          <url>tests/ELECTRONIC_SIGNATURE</url>
+        </reference>
+        <reference type="other">
           <url>tests/EVIDENCE</url>
         </reference>
         <reference type="other">
           <url>tests/EXPLOITABILITY_STATEMENT</url>
         </reference>
         <reference type="other">
           <url>tests/FORMULATION</url>
@@ -89,26 +95,32 @@
         <reference type="other">
           <url>tests/QUALITY_METRICS</url>
         </reference>
         <reference type="other">
           <url>tests/RELEASE_NOTES</url>
         </reference>
         <reference type="other">
+          <url>tests/RFC_9166</url>
+        </reference>
+        <reference type="other">
           <url>tests/RISK_ASSESSMENT</url>
         </reference>
         <reference type="other">
           <url>tests/RUNTIME_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
           <url>tests/SECURITY_CONTACT</url>
         </reference>
         <reference type="social">
           <url>tests/SOCIAL</url>
         </reference>
         <reference type="other">
+          <url>tests/SOURCE_DISTRIBUTION</url>
+        </reference>
+        <reference type="other">
           <url>tests/STATIC_ANALYSIS_REPORT</url>
         </reference>
         <reference type="support">
           <url>tests/SUPPORT</url>
         </reference>
         <reference type="other">
           <url>tests/THREAT_MODEL</url>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8744186046511628%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.3a.schema.json'",*

 * * "'components'": "{0: {'externalReferences': {insert: [(11, OrderedDict([('type', 'other'), "*

 * *                 "('url', 'tests/DIGITAL_SIGNATURE')])), (16, OrderedDict([('type', 'other'), "*

 * *                 "('url', 'tests/ELECTRONIC_SIGNATURE')])), (31, OrderedDict([('type', 'other'), "*

 * *                 "('url', 'tests/RFC_9166')])), (36, OrderedDict([('type', 'other'), ('url', "*

 * *                 "'tests/SOURCE_DISTRIBUTION')]))]}}}",*

 * * "'s […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.2b.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.3a.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "dummy",
             "externalReferences": [
                 {
                     "type": "other",
@@ -46,14 +46,18 @@
                     "url": "tests/COMPONENT_ANALYSIS_REPORT"
                 },
                 {
                     "type": "other",
                     "url": "tests/CONFIGURATION"
                 },
                 {
+                    "type": "other",
+                    "url": "tests/DIGITAL_SIGNATURE"
+                },
+                {
                     "type": "distribution",
                     "url": "tests/DISTRIBUTION"
                 },
                 {
                     "type": "other",
                     "url": "tests/DISTRIBUTION_INTAKE"
                 },
@@ -63,14 +67,18 @@
                 },
                 {
                     "type": "other",
                     "url": "tests/DYNAMIC_ANALYSIS_REPORT"
                 },
                 {
                     "type": "other",
+                    "url": "tests/ELECTRONIC_SIGNATURE"
+                },
+                {
+                    "type": "other",
                     "url": "tests/EVIDENCE"
                 },
                 {
                     "type": "other",
                     "url": "tests/EXPLOITABILITY_STATEMENT"
                 },
                 {
@@ -119,14 +127,18 @@
                 },
                 {
                     "type": "other",
                     "url": "tests/RELEASE_NOTES"
                 },
                 {
                     "type": "other",
+                    "url": "tests/RFC_9166"
+                },
+                {
+                    "type": "other",
                     "url": "tests/RISK_ASSESSMENT"
                 },
                 {
                     "type": "other",
                     "url": "tests/RUNTIME_ANALYSIS_REPORT"
                 },
                 {
@@ -135,14 +147,18 @@
                 },
                 {
                     "type": "social",
                     "url": "tests/SOCIAL"
                 },
                 {
                     "type": "other",
+                    "url": "tests/SOURCE_DISTRIBUTION"
+                },
+                {
+                    "type": "other",
                     "url": "tests/STATIC_ANALYSIS_REPORT"
                 },
                 {
                     "type": "support",
                     "url": "tests/SUPPORT"
                 },
                 {
@@ -179,10 +195,10 @@
                 "name": "cyclonedx-python-lib",
                 "vendor": "CycloneDX",
                 "version": "TESTING"
             }
         ]
     },
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
-    "specVersion": "1.2",
+    "specVersion": "1.3",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin`

 * *Files 2% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin`

```diff
@@ -44,27 +44,33 @@
         </reference>
         <reference type="other">
           <url>tests/COMPONENT_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
           <url>tests/CONFIGURATION</url>
         </reference>
+        <reference type="other">
+          <url>tests/DIGITAL_SIGNATURE</url>
+        </reference>
         <reference type="distribution">
           <url>tests/DISTRIBUTION</url>
         </reference>
         <reference type="other">
           <url>tests/DISTRIBUTION_INTAKE</url>
         </reference>
         <reference type="documentation">
           <url>tests/DOCUMENTATION</url>
         </reference>
         <reference type="other">
           <url>tests/DYNAMIC_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
+          <url>tests/ELECTRONIC_SIGNATURE</url>
+        </reference>
+        <reference type="other">
           <url>tests/EVIDENCE</url>
         </reference>
         <reference type="other">
           <url>tests/EXPLOITABILITY_STATEMENT</url>
         </reference>
         <reference type="other">
           <url>tests/FORMULATION</url>
@@ -99,26 +105,32 @@
         <reference type="other">
           <url>tests/QUALITY_METRICS</url>
         </reference>
         <reference type="other">
           <url>tests/RELEASE_NOTES</url>
         </reference>
         <reference type="other">
+          <url>tests/RFC_9166</url>
+        </reference>
+        <reference type="other">
           <url>tests/RISK_ASSESSMENT</url>
         </reference>
         <reference type="other">
           <url>tests/RUNTIME_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
           <url>tests/SECURITY_CONTACT</url>
         </reference>
         <reference type="social">
           <url>tests/SOCIAL</url>
         </reference>
         <reference type="other">
+          <url>tests/SOURCE_DISTRIBUTION</url>
+        </reference>
+        <reference type="other">
           <url>tests/STATIC_ANALYSIS_REPORT</url>
         </reference>
         <reference type="support">
           <url>tests/SUPPORT</url>
         </reference>
         <reference type="other">
           <url>tests/THREAT_MODEL</url>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8744186046511628%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.2b.schema.json'",*

 * * "'components'": "{0: {'externalReferences': {insert: [(11, OrderedDict([('type', 'other'), "*

 * *                 "('url', 'tests/DIGITAL_SIGNATURE')])), (16, OrderedDict([('type', 'other'), "*

 * *                 "('url', 'tests/ELECTRONIC_SIGNATURE')])), (31, OrderedDict([('type', 'other'), "*

 * *                 "('url', 'tests/RFC_9166')])), (36, OrderedDict([('type', 'other'), ('url', "*

 * *                 "'tests/SOURCE_DISTRIBUTION')]))]}}}",*

 * * "'s […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.3a.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.2b.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "dummy",
             "externalReferences": [
                 {
                     "type": "other",
@@ -46,14 +46,18 @@
                     "url": "tests/COMPONENT_ANALYSIS_REPORT"
                 },
                 {
                     "type": "other",
                     "url": "tests/CONFIGURATION"
                 },
                 {
+                    "type": "other",
+                    "url": "tests/DIGITAL_SIGNATURE"
+                },
+                {
                     "type": "distribution",
                     "url": "tests/DISTRIBUTION"
                 },
                 {
                     "type": "other",
                     "url": "tests/DISTRIBUTION_INTAKE"
                 },
@@ -63,14 +67,18 @@
                 },
                 {
                     "type": "other",
                     "url": "tests/DYNAMIC_ANALYSIS_REPORT"
                 },
                 {
                     "type": "other",
+                    "url": "tests/ELECTRONIC_SIGNATURE"
+                },
+                {
+                    "type": "other",
                     "url": "tests/EVIDENCE"
                 },
                 {
                     "type": "other",
                     "url": "tests/EXPLOITABILITY_STATEMENT"
                 },
                 {
@@ -119,14 +127,18 @@
                 },
                 {
                     "type": "other",
                     "url": "tests/RELEASE_NOTES"
                 },
                 {
                     "type": "other",
+                    "url": "tests/RFC_9166"
+                },
+                {
+                    "type": "other",
                     "url": "tests/RISK_ASSESSMENT"
                 },
                 {
                     "type": "other",
                     "url": "tests/RUNTIME_ANALYSIS_REPORT"
                 },
                 {
@@ -135,14 +147,18 @@
                 },
                 {
                     "type": "social",
                     "url": "tests/SOCIAL"
                 },
                 {
                     "type": "other",
+                    "url": "tests/SOURCE_DISTRIBUTION"
+                },
+                {
+                    "type": "other",
                     "url": "tests/STATIC_ANALYSIS_REPORT"
                 },
                 {
                     "type": "support",
                     "url": "tests/SUPPORT"
                 },
                 {
@@ -179,10 +195,10 @@
                 "name": "cyclonedx-python-lib",
                 "vendor": "CycloneDX",
                 "version": "TESTING"
             }
         ]
     },
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
-    "specVersion": "1.3",
+    "specVersion": "1.2",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin`

 * *Files 2% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin`

```diff
@@ -44,27 +44,33 @@
         </reference>
         <reference type="other">
           <url>tests/COMPONENT_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
           <url>tests/CONFIGURATION</url>
         </reference>
+        <reference type="other">
+          <url>tests/DIGITAL_SIGNATURE</url>
+        </reference>
         <reference type="distribution">
           <url>tests/DISTRIBUTION</url>
         </reference>
         <reference type="other">
           <url>tests/DISTRIBUTION_INTAKE</url>
         </reference>
         <reference type="documentation">
           <url>tests/DOCUMENTATION</url>
         </reference>
         <reference type="other">
           <url>tests/DYNAMIC_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
+          <url>tests/ELECTRONIC_SIGNATURE</url>
+        </reference>
+        <reference type="other">
           <url>tests/EVIDENCE</url>
         </reference>
         <reference type="other">
           <url>tests/EXPLOITABILITY_STATEMENT</url>
         </reference>
         <reference type="other">
           <url>tests/FORMULATION</url>
@@ -99,26 +105,32 @@
         <reference type="other">
           <url>tests/QUALITY_METRICS</url>
         </reference>
         <reference type="other">
           <url>tests/RELEASE_NOTES</url>
         </reference>
         <reference type="other">
+          <url>tests/RFC_9166</url>
+        </reference>
+        <reference type="other">
           <url>tests/RISK_ASSESSMENT</url>
         </reference>
         <reference type="other">
           <url>tests/RUNTIME_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
           <url>tests/SECURITY_CONTACT</url>
         </reference>
         <reference type="social">
           <url>tests/SOCIAL</url>
         </reference>
         <reference type="other">
+          <url>tests/SOURCE_DISTRIBUTION</url>
+        </reference>
+        <reference type="other">
           <url>tests/STATIC_ANALYSIS_REPORT</url>
         </reference>
         <reference type="support">
           <url>tests/SUPPORT</url>
         </reference>
         <reference type="other">
           <url>tests/THREAT_MODEL</url>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992732558139534%*

 * *Differences: {"'components'": "{0: {'externalReferences': {insert: [(11, OrderedDict([('type', 'other'), "*

 * *                 "('url', 'tests/DIGITAL_SIGNATURE')])), (16, OrderedDict([('type', 'other'), "*

 * *                 "('url', 'tests/ELECTRONIC_SIGNATURE')])), (31, OrderedDict([('type', 'other'), "*

 * *                 "('url', 'tests/RFC_9166')])), (36, OrderedDict([('type', 'other'), ('url', "*

 * *                 "'tests/SOURCE_DISTRIBUTION')]))]}}}"}*

```diff
@@ -46,14 +46,18 @@
                     "url": "tests/COMPONENT_ANALYSIS_REPORT"
                 },
                 {
                     "type": "other",
                     "url": "tests/CONFIGURATION"
                 },
                 {
+                    "type": "other",
+                    "url": "tests/DIGITAL_SIGNATURE"
+                },
+                {
                     "type": "distribution",
                     "url": "tests/DISTRIBUTION"
                 },
                 {
                     "type": "other",
                     "url": "tests/DISTRIBUTION_INTAKE"
                 },
@@ -63,14 +67,18 @@
                 },
                 {
                     "type": "other",
                     "url": "tests/DYNAMIC_ANALYSIS_REPORT"
                 },
                 {
                     "type": "other",
+                    "url": "tests/ELECTRONIC_SIGNATURE"
+                },
+                {
+                    "type": "other",
                     "url": "tests/EVIDENCE"
                 },
                 {
                     "type": "other",
                     "url": "tests/EXPLOITABILITY_STATEMENT"
                 },
                 {
@@ -119,14 +127,18 @@
                 },
                 {
                     "type": "release-notes",
                     "url": "tests/RELEASE_NOTES"
                 },
                 {
                     "type": "other",
+                    "url": "tests/RFC_9166"
+                },
+                {
+                    "type": "other",
                     "url": "tests/RISK_ASSESSMENT"
                 },
                 {
                     "type": "other",
                     "url": "tests/RUNTIME_ANALYSIS_REPORT"
                 },
                 {
@@ -135,14 +147,18 @@
                 },
                 {
                     "type": "social",
                     "url": "tests/SOCIAL"
                 },
                 {
                     "type": "other",
+                    "url": "tests/SOURCE_DISTRIBUTION"
+                },
+                {
+                    "type": "other",
                     "url": "tests/STATIC_ANALYSIS_REPORT"
                 },
                 {
                     "type": "support",
                     "url": "tests/SUPPORT"
                 },
                 {
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin`

 * *Files 1% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin`

```diff
@@ -69,27 +69,33 @@
         </reference>
         <reference type="other">
           <url>tests/COMPONENT_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
           <url>tests/CONFIGURATION</url>
         </reference>
+        <reference type="other">
+          <url>tests/DIGITAL_SIGNATURE</url>
+        </reference>
         <reference type="distribution">
           <url>tests/DISTRIBUTION</url>
         </reference>
         <reference type="other">
           <url>tests/DISTRIBUTION_INTAKE</url>
         </reference>
         <reference type="documentation">
           <url>tests/DOCUMENTATION</url>
         </reference>
         <reference type="other">
           <url>tests/DYNAMIC_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
+          <url>tests/ELECTRONIC_SIGNATURE</url>
+        </reference>
+        <reference type="other">
           <url>tests/EVIDENCE</url>
         </reference>
         <reference type="other">
           <url>tests/EXPLOITABILITY_STATEMENT</url>
         </reference>
         <reference type="other">
           <url>tests/FORMULATION</url>
@@ -124,26 +130,32 @@
         <reference type="other">
           <url>tests/QUALITY_METRICS</url>
         </reference>
         <reference type="release-notes">
           <url>tests/RELEASE_NOTES</url>
         </reference>
         <reference type="other">
+          <url>tests/RFC_9166</url>
+        </reference>
+        <reference type="other">
           <url>tests/RISK_ASSESSMENT</url>
         </reference>
         <reference type="other">
           <url>tests/RUNTIME_ANALYSIS_REPORT</url>
         </reference>
         <reference type="other">
           <url>tests/SECURITY_CONTACT</url>
         </reference>
         <reference type="social">
           <url>tests/SOCIAL</url>
         </reference>
         <reference type="other">
+          <url>tests/SOURCE_DISTRIBUTION</url>
+        </reference>
+        <reference type="other">
           <url>tests/STATIC_ANALYSIS_REPORT</url>
         </reference>
         <reference type="support">
           <url>tests/SUPPORT</url>
         </reference>
         <reference type="other">
           <url>tests/THREAT_MODEL</url>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8742732558139534%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.6.schema.json'",*

 * * "'components'": "{0: {'externalReferences': {insert: [(11, OrderedDict([('type', "*

 * *                 "'digital-signature'), ('url', 'tests/DIGITAL_SIGNATURE')])), (16, "*

 * *                 "OrderedDict([('type', 'electronic-signature'), ('url', "*

 * *                 "'tests/ELECTRONIC_SIGNATURE')])), (31, OrderedDict([('type', 'rfc-9116'), "*

 * *                 "('url', 'tests/RFC_9166')])), (36, OrderedDict([('type', 'source-distribution'), "*

 * *      […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.5.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.6.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "dummy",
             "externalReferences": [
                 {
                     "type": "adversary-model",
@@ -46,14 +46,18 @@
                     "url": "tests/COMPONENT_ANALYSIS_REPORT"
                 },
                 {
                     "type": "configuration",
                     "url": "tests/CONFIGURATION"
                 },
                 {
+                    "type": "digital-signature",
+                    "url": "tests/DIGITAL_SIGNATURE"
+                },
+                {
                     "type": "distribution",
                     "url": "tests/DISTRIBUTION"
                 },
                 {
                     "type": "distribution-intake",
                     "url": "tests/DISTRIBUTION_INTAKE"
                 },
@@ -62,14 +66,18 @@
                     "url": "tests/DOCUMENTATION"
                 },
                 {
                     "type": "dynamic-analysis-report",
                     "url": "tests/DYNAMIC_ANALYSIS_REPORT"
                 },
                 {
+                    "type": "electronic-signature",
+                    "url": "tests/ELECTRONIC_SIGNATURE"
+                },
+                {
                     "type": "evidence",
                     "url": "tests/EVIDENCE"
                 },
                 {
                     "type": "exploitability-statement",
                     "url": "tests/EXPLOITABILITY_STATEMENT"
                 },
@@ -118,14 +126,18 @@
                     "url": "tests/QUALITY_METRICS"
                 },
                 {
                     "type": "release-notes",
                     "url": "tests/RELEASE_NOTES"
                 },
                 {
+                    "type": "rfc-9116",
+                    "url": "tests/RFC_9166"
+                },
+                {
                     "type": "risk-assessment",
                     "url": "tests/RISK_ASSESSMENT"
                 },
                 {
                     "type": "runtime-analysis-report",
                     "url": "tests/RUNTIME_ANALYSIS_REPORT"
                 },
@@ -134,14 +146,18 @@
                     "url": "tests/SECURITY_CONTACT"
                 },
                 {
                     "type": "social",
                     "url": "tests/SOCIAL"
                 },
                 {
+                    "type": "source-distribution",
+                    "url": "tests/SOURCE_DISTRIBUTION"
+                },
+                {
                     "type": "static-analysis-report",
                     "url": "tests/STATIC_ANALYSIS_REPORT"
                 },
                 {
                     "type": "support",
                     "url": "tests/SUPPORT"
                 },
@@ -212,10 +228,10 @@
                 "name": "cyclonedx-python-lib",
                 "vendor": "CycloneDX",
                 "version": "TESTING"
             }
         ]
     },
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
-    "specVersion": "1.5",
+    "specVersion": "1.6",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin`

 * *Files 2% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin`

```diff
@@ -69,26 +69,32 @@
         </reference>
         <reference type="component-analysis-report">
           <url>tests/COMPONENT_ANALYSIS_REPORT</url>
         </reference>
         <reference type="configuration">
           <url>tests/CONFIGURATION</url>
         </reference>
+        <reference type="other">
+          <url>tests/DIGITAL_SIGNATURE</url>
+        </reference>
         <reference type="distribution">
           <url>tests/DISTRIBUTION</url>
         </reference>
         <reference type="distribution-intake">
           <url>tests/DISTRIBUTION_INTAKE</url>
         </reference>
         <reference type="documentation">
           <url>tests/DOCUMENTATION</url>
         </reference>
         <reference type="dynamic-analysis-report">
           <url>tests/DYNAMIC_ANALYSIS_REPORT</url>
         </reference>
+        <reference type="other">
+          <url>tests/ELECTRONIC_SIGNATURE</url>
+        </reference>
         <reference type="evidence">
           <url>tests/EVIDENCE</url>
         </reference>
         <reference type="exploitability-statement">
           <url>tests/EXPLOITABILITY_STATEMENT</url>
         </reference>
         <reference type="formulation">
@@ -123,26 +129,32 @@
         </reference>
         <reference type="quality-metrics">
           <url>tests/QUALITY_METRICS</url>
         </reference>
         <reference type="release-notes">
           <url>tests/RELEASE_NOTES</url>
         </reference>
+        <reference type="other">
+          <url>tests/RFC_9166</url>
+        </reference>
         <reference type="risk-assessment">
           <url>tests/RISK_ASSESSMENT</url>
         </reference>
         <reference type="runtime-analysis-report">
           <url>tests/RUNTIME_ANALYSIS_REPORT</url>
         </reference>
         <reference type="security-contact">
           <url>tests/SECURITY_CONTACT</url>
         </reference>
         <reference type="social">
           <url>tests/SOCIAL</url>
         </reference>
+        <reference type="other">
+          <url>tests/SOURCE_DISTRIBUTION</url>
+        </reference>
         <reference type="static-analysis-report">
           <url>tests/STATIC_ANALYSIS_REPORT</url>
         </reference>
         <reference type="support">
           <url>tests/SUPPORT</url>
         </reference>
         <reference type="threat-model">
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994893790849674%*

 * *Differences: {"'metadata'": "{'component': {'supplier': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}, 'manufacture': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}"}*

```diff
@@ -217,15 +217,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "swid": {
                 "name": "Test Application",
                 "tagId": "swidgen-242eb18a-503e-ca37-393b-cf156ef09691_9.1.1",
                 "text": {
                     "content": "PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiID8+CjxTb2Z0d2FyZUlkZW50aXR5IHhtbDpsYW5nPSJFTiIgbmFtZT0iQWNtZSBBcHBsaWNhdGlvbiIgdmVyc2lvbj0iOS4xLjEiIAogdmVyc2lvblNjaGVtZT0ibXVsdGlwYXJ0bnVtZXJpYyIgCiB0YWdJZD0ic3dpZGdlbi1iNTk1MWFjOS00MmMwLWYzODItM2YxZS1iYzdhMmE0NDk3Y2JfOS4xLjEiIAogeG1sbnM9Imh0dHA6Ly9zdGFuZGFyZHMuaXNvLm9yZy9pc28vMTk3NzAvLTIvMjAxNS9zY2hlbWEueHNkIj4gCiB4bWxuczp4c2k9Imh0dHA6Ly93d3cudzMub3JnLzIwMDEvWE1MU2NoZW1hLWluc3RhbmNlIiAKIHhzaTpzY2hlbWFMb2NhdGlvbj0iaHR0cDovL3N0YW5kYXJkcy5pc28ub3JnL2lzby8xOTc3MC8tMi8yMDE1LWN1cnJlbnQvc2NoZW1hLnhzZCBzY2hlbWEueHNkIiA+CiAgPE1ldGEgZ2VuZXJhdG9yPSJTV0lEIFRhZyBPbmxpbmUgR2VuZXJhdG9yIHYwLjEiIC8+IAogIDxFbnRpdHkgbmFtZT0iQWNtZSwgSW5jLiIgcmVnaWQ9ImV4YW1wbGUuY29tIiByb2xlPSJ0YWdDcmVhdG9yIiAvPiAKPC9Tb2Z0d2FyZUlkZW50aXR5Pg==",
@@ -247,15 +248,16 @@
                 {
                     "email": "paul.horton@owasp.org",
                     "name": "Paul Horton"
                 }
             ],
             "name": "CycloneDX",
             "url": [
-                "https://cyclonedx.org"
+                "https://cyclonedx.org",
+                "https://cyclonedx.org/docs"
             ]
         },
         "supplier": {
             "contact": [
                 {
                     "email": "someone@somewhere.tld",
                     "name": "A N Other",
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin`

 * *Files 1% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin`

```diff
@@ -20,14 +20,15 @@
         <email>paul.horton@owasp.org</email>
       </author>
     </authors>
     <component type="library" bom-ref="my-specific-bom-ref-for-dings">
       <supplier>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
@@ -179,14 +180,15 @@
           </externalReferences>
         </component>
       </components>
     </component>
     <manufacture>
       <name>CycloneDX</name>
       <url>https://cyclonedx.org</url>
+      <url>https://cyclonedx.org/docs</url>
       <contact>
         <name>A N Other</name>
         <email>someone@somewhere.tld</email>
         <phone>+44 (0)1234 567890</phone>
       </contact>
       <contact>
         <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996181860902256%*

 * *Differences: {"'metadata'": "{'component': {'supplier': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}, 'manufacture': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}"}*

```diff
@@ -261,15 +261,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "swid": {
                 "name": "Test Application",
                 "tagId": "swidgen-242eb18a-503e-ca37-393b-cf156ef09691_9.1.1",
                 "text": {
                     "content": "PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiID8+CjxTb2Z0d2FyZUlkZW50aXR5IHhtbDpsYW5nPSJFTiIgbmFtZT0iQWNtZSBBcHBsaWNhdGlvbiIgdmVyc2lvbj0iOS4xLjEiIAogdmVyc2lvblNjaGVtZT0ibXVsdGlwYXJ0bnVtZXJpYyIgCiB0YWdJZD0ic3dpZGdlbi1iNTk1MWFjOS00MmMwLWYzODItM2YxZS1iYzdhMmE0NDk3Y2JfOS4xLjEiIAogeG1sbnM9Imh0dHA6Ly9zdGFuZGFyZHMuaXNvLm9yZy9pc28vMTk3NzAvLTIvMjAxNS9zY2hlbWEueHNkIj4gCiB4bWxuczp4c2k9Imh0dHA6Ly93d3cudzMub3JnLzIwMDEvWE1MU2NoZW1hLWluc3RhbmNlIiAKIHhzaTpzY2hlbWFMb2NhdGlvbj0iaHR0cDovL3N0YW5kYXJkcy5pc28ub3JnL2lzby8xOTc3MC8tMi8yMDE1LWN1cnJlbnQvc2NoZW1hLnhzZCBzY2hlbWEueHNkIiA+CiAgPE1ldGEgZ2VuZXJhdG9yPSJTV0lEIFRhZyBPbmxpbmUgR2VuZXJhdG9yIHYwLjEiIC8+IAogIDxFbnRpdHkgbmFtZT0iQWNtZSwgSW5jLiIgcmVnaWQ9ImV4YW1wbGUuY29tIiByb2xlPSJ0YWdDcmVhdG9yIiAvPiAKPC9Tb2Z0d2FyZUlkZW50aXR5Pg==",
@@ -304,15 +305,16 @@
                 {
                     "email": "paul.horton@owasp.org",
                     "name": "Paul Horton"
                 }
             ],
             "name": "CycloneDX",
             "url": [
-                "https://cyclonedx.org"
+                "https://cyclonedx.org",
+                "https://cyclonedx.org/docs"
             ]
         },
         "properties": [
             {
                 "name": "key1",
                 "value": "val1"
             },
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin`

 * *Files 2% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin`

```diff
@@ -20,14 +20,15 @@
         <email>paul.horton@owasp.org</email>
       </author>
     </authors>
     <component type="library" bom-ref="my-specific-bom-ref-for-dings">
       <supplier>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
@@ -201,14 +202,15 @@
           <text>Commercial 2</text>
         </copyright>
       </evidence>
     </component>
     <manufacture>
       <name>CycloneDX</name>
       <url>https://cyclonedx.org</url>
+      <url>https://cyclonedx.org/docs</url>
       <contact>
         <name>A N Other</name>
         <email>someone@somewhere.tld</email>
         <phone>+44 (0)1234 567890</phone>
       </contact>
       <contact>
         <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996186755952381%*

 * *Differences: {"'metadata'": "{'component': {'supplier': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}, 'manufacture': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}"}*

```diff
@@ -318,15 +318,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "swid": {
                 "name": "Test Application",
                 "tagId": "swidgen-242eb18a-503e-ca37-393b-cf156ef09691_9.1.1",
                 "text": {
                     "content": "PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiID8+CjxTb2Z0d2FyZUlkZW50aXR5IHhtbDpsYW5nPSJFTiIgbmFtZT0iQWNtZSBBcHBsaWNhdGlvbiIgdmVyc2lvbj0iOS4xLjEiIAogdmVyc2lvblNjaGVtZT0ibXVsdGlwYXJ0bnVtZXJpYyIgCiB0YWdJZD0ic3dpZGdlbi1iNTk1MWFjOS00MmMwLWYzODItM2YxZS1iYzdhMmE0NDk3Y2JfOS4xLjEiIAogeG1sbnM9Imh0dHA6Ly9zdGFuZGFyZHMuaXNvLm9yZy9pc28vMTk3NzAvLTIvMjAxNS9zY2hlbWEueHNkIj4gCiB4bWxuczp4c2k9Imh0dHA6Ly93d3cudzMub3JnLzIwMDEvWE1MU2NoZW1hLWluc3RhbmNlIiAKIHhzaTpzY2hlbWFMb2NhdGlvbj0iaHR0cDovL3N0YW5kYXJkcy5pc28ub3JnL2lzby8xOTc3MC8tMi8yMDE1LWN1cnJlbnQvc2NoZW1hLnhzZCBzY2hlbWEueHNkIiA+CiAgPE1ldGEgZ2VuZXJhdG9yPSJTV0lEIFRhZyBPbmxpbmUgR2VuZXJhdG9yIHYwLjEiIC8+IAogIDxFbnRpdHkgbmFtZT0iQWNtZSwgSW5jLiIgcmVnaWQ9ImV4YW1wbGUuY29tIiByb2xlPSJ0YWdDcmVhdG9yIiAvPiAKPC9Tb2Z0d2FyZUlkZW50aXR5Pg==",
@@ -361,15 +362,16 @@
                 {
                     "email": "paul.horton@owasp.org",
                     "name": "Paul Horton"
                 }
             ],
             "name": "CycloneDX",
             "url": [
-                "https://cyclonedx.org"
+                "https://cyclonedx.org",
+                "https://cyclonedx.org/docs"
             ]
         },
         "properties": [
             {
                 "name": "key1",
                 "value": "val1"
             },
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin`

 * *Files 0% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin`

```diff
@@ -46,14 +46,15 @@
         <email>paul.horton@owasp.org</email>
       </author>
     </authors>
     <component type="library" bom-ref="my-specific-bom-ref-for-dings">
       <supplier>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
@@ -269,14 +270,15 @@
           <property name="key2">val2</property>
         </properties>
       </releaseNotes>
     </component>
     <manufacture>
       <name>CycloneDX</name>
       <url>https://cyclonedx.org</url>
+      <url>https://cyclonedx.org/docs</url>
       <contact>
         <name>A N Other</name>
         <email>someone@somewhere.tld</email>
         <phone>+44 (0)1234 567890</phone>
       </contact>
       <contact>
         <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996186755952381%*

 * *Differences: {"'metadata'": "{'component': {'supplier': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}, 'manufacture': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}"}*

```diff
@@ -318,15 +318,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "swid": {
                 "name": "Test Application",
                 "tagId": "swidgen-242eb18a-503e-ca37-393b-cf156ef09691_9.1.1",
                 "text": {
                     "content": "PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiID8+CjxTb2Z0d2FyZUlkZW50aXR5IHhtbDpsYW5nPSJFTiIgbmFtZT0iQWNtZSBBcHBsaWNhdGlvbiIgdmVyc2lvbj0iOS4xLjEiIAogdmVyc2lvblNjaGVtZT0ibXVsdGlwYXJ0bnVtZXJpYyIgCiB0YWdJZD0ic3dpZGdlbi1iNTk1MWFjOS00MmMwLWYzODItM2YxZS1iYzdhMmE0NDk3Y2JfOS4xLjEiIAogeG1sbnM9Imh0dHA6Ly9zdGFuZGFyZHMuaXNvLm9yZy9pc28vMTk3NzAvLTIvMjAxNS9zY2hlbWEueHNkIj4gCiB4bWxuczp4c2k9Imh0dHA6Ly93d3cudzMub3JnLzIwMDEvWE1MU2NoZW1hLWluc3RhbmNlIiAKIHhzaTpzY2hlbWFMb2NhdGlvbj0iaHR0cDovL3N0YW5kYXJkcy5pc28ub3JnL2lzby8xOTc3MC8tMi8yMDE1LWN1cnJlbnQvc2NoZW1hLnhzZCBzY2hlbWEueHNkIiA+CiAgPE1ldGEgZ2VuZXJhdG9yPSJTV0lEIFRhZyBPbmxpbmUgR2VuZXJhdG9yIHYwLjEiIC8+IAogIDxFbnRpdHkgbmFtZT0iQWNtZSwgSW5jLiIgcmVnaWQ9ImV4YW1wbGUuY29tIiByb2xlPSJ0YWdDcmVhdG9yIiAvPiAKPC9Tb2Z0d2FyZUlkZW50aXR5Pg==",
@@ -361,15 +362,16 @@
                 {
                     "email": "paul.horton@owasp.org",
                     "name": "Paul Horton"
                 }
             ],
             "name": "CycloneDX",
             "url": [
-                "https://cyclonedx.org"
+                "https://cyclonedx.org",
+                "https://cyclonedx.org/docs"
             ]
         },
         "properties": [
             {
                 "name": "key1",
                 "value": "val1"
             },
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin`

 * *Files 0% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin`

```diff
@@ -46,14 +46,15 @@
         <email>paul.horton@owasp.org</email>
       </author>
     </authors>
     <component type="library" bom-ref="my-specific-bom-ref-for-dings">
       <supplier>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
@@ -269,14 +270,15 @@
           <property name="key2">val2</property>
         </properties>
       </releaseNotes>
     </component>
     <manufacture>
       <name>CycloneDX</name>
       <url>https://cyclonedx.org</url>
+      <url>https://cyclonedx.org/docs</url>
       <contact>
         <name>A N Other</name>
         <email>someone@somewhere.tld</email>
         <phone>+44 (0)1234 567890</phone>
       </contact>
       <contact>
         <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998468137254902%*

 * *Differences: {"'components'": "{0: {'supplier': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}}}"}*

```diff
@@ -201,15 +201,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "swid": {
                 "name": "Test Application",
                 "tagId": "swidgen-242eb18a-503e-ca37-393b-cf156ef09691_9.1.1",
                 "text": {
                     "content": "PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiID8+CjxTb2Z0d2FyZUlkZW50aXR5IHhtbDpsYW5nPSJFTiIgbmFtZT0iQWNtZSBBcHBsaWNhdGlvbiIgdmVyc2lvbj0iOS4xLjEiIAogdmVyc2lvblNjaGVtZT0ibXVsdGlwYXJ0bnVtZXJpYyIgCiB0YWdJZD0ic3dpZGdlbi1iNTk1MWFjOS00MmMwLWYzODItM2YxZS1iYzdhMmE0NDk3Y2JfOS4xLjEiIAogeG1sbnM9Imh0dHA6Ly9zdGFuZGFyZHMuaXNvLm9yZy9pc28vMTk3NzAvLTIvMjAxNS9zY2hlbWEueHNkIj4gCiB4bWxuczp4c2k9Imh0dHA6Ly93d3cudzMub3JnLzIwMDEvWE1MU2NoZW1hLWluc3RhbmNlIiAKIHhzaTpzY2hlbWFMb2NhdGlvbj0iaHR0cDovL3N0YW5kYXJkcy5pc28ub3JnL2lzby8xOTc3MC8tMi8yMDE1LWN1cnJlbnQvc2NoZW1hLnhzZCBzY2hlbWEueHNkIiA+CiAgPE1ldGEgZ2VuZXJhdG9yPSJTV0lEIFRhZyBPbmxpbmUgR2VuZXJhdG9yIHYwLjEiIC8+IAogIDxFbnRpdHkgbmFtZT0iQWNtZSwgSW5jLiIgcmVnaWQ9ImV4YW1wbGUuY29tIiByb2xlPSJ0YWdDcmVhdG9yIiAvPiAKPC9Tb2Z0d2FyZUlkZW50aXR5Pg==",
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin`

 * *Files 1% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin`

```diff
@@ -11,14 +11,15 @@
     </tools>
   </metadata>
   <components>
     <component type="library" bom-ref="my-specific-bom-ref-for-dings">
       <supplier>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998629385964912%*

 * *Differences: {"'components'": "{0: {'supplier': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}}}"}*

```diff
@@ -245,15 +245,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "swid": {
                 "name": "Test Application",
                 "tagId": "swidgen-242eb18a-503e-ca37-393b-cf156ef09691_9.1.1",
                 "text": {
                     "content": "PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiID8+CjxTb2Z0d2FyZUlkZW50aXR5IHhtbDpsYW5nPSJFTiIgbmFtZT0iQWNtZSBBcHBsaWNhdGlvbiIgdmVyc2lvbj0iOS4xLjEiIAogdmVyc2lvblNjaGVtZT0ibXVsdGlwYXJ0bnVtZXJpYyIgCiB0YWdJZD0ic3dpZGdlbi1iNTk1MWFjOS00MmMwLWYzODItM2YxZS1iYzdhMmE0NDk3Y2JfOS4xLjEiIAogeG1sbnM9Imh0dHA6Ly9zdGFuZGFyZHMuaXNvLm9yZy9pc28vMTk3NzAvLTIvMjAxNS9zY2hlbWEueHNkIj4gCiB4bWxuczp4c2k9Imh0dHA6Ly93d3cudzMub3JnLzIwMDEvWE1MU2NoZW1hLWluc3RhbmNlIiAKIHhzaTpzY2hlbWFMb2NhdGlvbj0iaHR0cDovL3N0YW5kYXJkcy5pc28ub3JnL2lzby8xOTc3MC8tMi8yMDE1LWN1cnJlbnQvc2NoZW1hLnhzZCBzY2hlbWEueHNkIiA+CiAgPE1ldGEgZ2VuZXJhdG9yPSJTV0lEIFRhZyBPbmxpbmUgR2VuZXJhdG9yIHYwLjEiIC8+IAogIDxFbnRpdHkgbmFtZT0iQWNtZSwgSW5jLiIgcmVnaWQ9ImV4YW1wbGUuY29tIiByb2xlPSJ0YWdDcmVhdG9yIiAvPiAKPC9Tb2Z0d2FyZUlkZW50aXR5Pg==",
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin`

 * *Files 2% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin`

```diff
@@ -11,14 +11,15 @@
     </tools>
   </metadata>
   <components>
     <component type="library" bom-ref="my-specific-bom-ref-for-dings">
       <supplier>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998697916666667%*

 * *Differences: {"'components'": "{0: {'supplier': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}}}"}*

```diff
@@ -302,15 +302,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "swid": {
                 "name": "Test Application",
                 "tagId": "swidgen-242eb18a-503e-ca37-393b-cf156ef09691_9.1.1",
                 "text": {
                     "content": "PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiID8+CjxTb2Z0d2FyZUlkZW50aXR5IHhtbDpsYW5nPSJFTiIgbmFtZT0iQWNtZSBBcHBsaWNhdGlvbiIgdmVyc2lvbj0iOS4xLjEiIAogdmVyc2lvblNjaGVtZT0ibXVsdGlwYXJ0bnVtZXJpYyIgCiB0YWdJZD0ic3dpZGdlbi1iNTk1MWFjOS00MmMwLWYzODItM2YxZS1iYzdhMmE0NDk3Y2JfOS4xLjEiIAogeG1sbnM9Imh0dHA6Ly9zdGFuZGFyZHMuaXNvLm9yZy9pc28vMTk3NzAvLTIvMjAxNS9zY2hlbWEueHNkIj4gCiB4bWxuczp4c2k9Imh0dHA6Ly93d3cudzMub3JnLzIwMDEvWE1MU2NoZW1hLWluc3RhbmNlIiAKIHhzaTpzY2hlbWFMb2NhdGlvbj0iaHR0cDovL3N0YW5kYXJkcy5pc28ub3JnL2lzby8xOTc3MC8tMi8yMDE1LWN1cnJlbnQvc2NoZW1hLnhzZCBzY2hlbWEueHNkIiA+CiAgPE1ldGEgZ2VuZXJhdG9yPSJTV0lEIFRhZyBPbmxpbmUgR2VuZXJhdG9yIHYwLjEiIC8+IAogIDxFbnRpdHkgbmFtZT0iQWNtZSwgSW5jLiIgcmVnaWQ9ImV4YW1wbGUuY29tIiByb2xlPSJ0YWdDcmVhdG9yIiAvPiAKPC9Tb2Z0d2FyZUlkZW50aXR5Pg==",
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin`

 * *Files 0% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<bom xmlns="http://cyclonedx.org/schema/bom/1.4" serialNumber="urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac" version="1">
+<bom xmlns="http://cyclonedx.org/schema/bom/1.5" serialNumber="urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac" version="1">
   <metadata>
     <timestamp>2023-01-07T13:44:32.312678+00:00</timestamp>
     <tools>
       <tool>
         <vendor>CycloneDX</vendor>
         <name>cyclonedx-python-lib</name>
         <version>TESTING</version>
@@ -37,14 +37,15 @@
     </tools>
   </metadata>
   <components>
     <component type="library" bom-ref="my-specific-bom-ref-for-dings">
       <supplier>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998697916666667%*

 * *Differences: {"'components'": "{0: {'supplier': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}}}"}*

```diff
@@ -302,15 +302,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "swid": {
                 "name": "Test Application",
                 "tagId": "swidgen-242eb18a-503e-ca37-393b-cf156ef09691_9.1.1",
                 "text": {
                     "content": "PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiID8+CjxTb2Z0d2FyZUlkZW50aXR5IHhtbDpsYW5nPSJFTiIgbmFtZT0iQWNtZSBBcHBsaWNhdGlvbiIgdmVyc2lvbj0iOS4xLjEiIAogdmVyc2lvblNjaGVtZT0ibXVsdGlwYXJ0bnVtZXJpYyIgCiB0YWdJZD0ic3dpZGdlbi1iNTk1MWFjOS00MmMwLWYzODItM2YxZS1iYzdhMmE0NDk3Y2JfOS4xLjEiIAogeG1sbnM9Imh0dHA6Ly9zdGFuZGFyZHMuaXNvLm9yZy9pc28vMTk3NzAvLTIvMjAxNS9zY2hlbWEueHNkIj4gCiB4bWxuczp4c2k9Imh0dHA6Ly93d3cudzMub3JnLzIwMDEvWE1MU2NoZW1hLWluc3RhbmNlIiAKIHhzaTpzY2hlbWFMb2NhdGlvbj0iaHR0cDovL3N0YW5kYXJkcy5pc28ub3JnL2lzby8xOTc3MC8tMi8yMDE1LWN1cnJlbnQvc2NoZW1hLnhzZCBzY2hlbWEueHNkIiA+CiAgPE1ldGEgZ2VuZXJhdG9yPSJTV0lEIFRhZyBPbmxpbmUgR2VuZXJhdG9yIHYwLjEiIC8+IAogIDxFbnRpdHkgbmFtZT0iQWNtZSwgSW5jLiIgcmVnaWQ9ImV4YW1wbGUuY29tIiByb2xlPSJ0YWdDcmVhdG9yIiAvPiAKPC9Tb2Z0d2FyZUlkZW50aXR5Pg==",
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin`

 * *Files 1% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<bom xmlns="http://cyclonedx.org/schema/bom/1.5" serialNumber="urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac" version="1">
+<bom xmlns="http://cyclonedx.org/schema/bom/1.4" serialNumber="urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac" version="1">
   <metadata>
     <timestamp>2023-01-07T13:44:32.312678+00:00</timestamp>
     <tools>
       <tool>
         <vendor>CycloneDX</vendor>
         <name>cyclonedx-python-lib</name>
         <version>TESTING</version>
@@ -37,14 +37,15 @@
     </tools>
   </metadata>
   <components>
     <component type="library" bom-ref="my-specific-bom-ref-for-dings">
       <supplier>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999678497942388%*

 * *Differences: {"'vulnerabilities'": "{0: {'credits': {'organizations': {0: {'url': {insert: [(1, "*

 * *                      "'https://cyclonedx.org/docs')]}}}}}}"}*

```diff
@@ -120,15 +120,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     }
                 ]
             },
             "cwes": [
                 22,
                 33
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin`

 * *Files 1% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<bom xmlns="http://cyclonedx.org/schema/bom/1.4" serialNumber="urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac" version="1">
+<bom xmlns="http://cyclonedx.org/schema/bom/1.5" serialNumber="urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac" version="1">
   <metadata>
     <timestamp>2023-01-07T13:44:32.312678+00:00</timestamp>
     <tools>
       <tool>
         <vendor>CycloneDX</vendor>
         <name>cyclonedx-python-lib</name>
         <version>TESTING</version>
@@ -111,14 +111,15 @@
       <published>2021-09-02T10:50:42.051979+00:00</published>
       <updated>2021-09-03T10:50:42.051979+00:00</updated>
       <credits>
         <organizations>
           <organization>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999678497942388%*

 * *Differences: {"'vulnerabilities'": "{0: {'credits': {'organizations': {0: {'url': {insert: [(1, "*

 * *                      "'https://cyclonedx.org/docs')]}}}}}}"}*

```diff
@@ -120,15 +120,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     }
                 ]
             },
             "cwes": [
                 22,
                 33
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin`

 * *Files 1% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<bom xmlns="http://cyclonedx.org/schema/bom/1.5" serialNumber="urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac" version="1">
+<bom xmlns="http://cyclonedx.org/schema/bom/1.4" serialNumber="urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac" version="1">
   <metadata>
     <timestamp>2023-01-07T13:44:32.312678+00:00</timestamp>
     <tools>
       <tool>
         <vendor>CycloneDX</vendor>
         <name>cyclonedx-python-lib</name>
         <version>TESTING</version>
@@ -111,14 +111,15 @@
       <published>2021-09-02T10:50:42.051979+00:00</published>
       <updated>2021-09-03T10:50:42.051979+00:00</updated>
       <credits>
         <organizations>
           <organization>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998745612026863%*

 * *Differences: {"'services'": "{0: {'provider': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}, "*

 * *               "'services': {0: {'provider': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}}}, 1: {'services': {0: {'provider': {'url': "*

 * *               "{insert: [(1, 'https://cyclonedx.org/docs')]}}}}}}"}*

```diff
@@ -70,15 +70,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "services": [
                 {
                     "authenticated": true,
                     "bom-ref": "my-specific-bom-ref-for-second-nested-service",
                     "group": "no-group",
@@ -93,15 +94,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     },
                     "version": "3.2.1",
                     "x-trust-boundary": false
                 },
                 {
                     "bom-ref": "my-specific-bom-ref-for-first-nested-service",
@@ -129,15 +131,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     },
                     "version": "6.5.4"
                 },
                 {
                     "bom-ref": "my-specific-bom-ref-for-another-nested-service",
                     "name": "another-nested-service"
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin`

 * *Files 6% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin`

```diff
@@ -15,14 +15,15 @@
     </component>
   </metadata>
   <services>
     <service bom-ref="my-specific-bom-ref-for-my-first-service">
       <provider>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
@@ -54,14 +55,15 @@
         </reference>
       </externalReferences>
       <services>
         <service bom-ref="my-specific-bom-ref-for-second-nested-service">
           <provider>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
@@ -82,14 +84,15 @@
     <service bom-ref="my-specific-bom-ref-for-my-second-service">
       <name>my-second-service</name>
       <services>
         <service bom-ref="yet-another-nested-service">
           <provider>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998819710175737%*

 * *Differences: {"'services'": "{0: {'provider': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}, "*

 * *               "'services': {0: {'provider': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}}}, 1: {'services': {0: {'provider': {'url': "*

 * *               "{insert: [(1, 'https://cyclonedx.org/docs')]}}}}}}"}*

```diff
@@ -86,15 +86,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "services": [
                 {
                     "authenticated": true,
                     "bom-ref": "my-specific-bom-ref-for-second-nested-service",
                     "group": "no-group",
@@ -109,15 +110,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     },
                     "version": "3.2.1",
                     "x-trust-boundary": false
                 },
                 {
                     "bom-ref": "my-specific-bom-ref-for-first-nested-service",
@@ -145,15 +147,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     },
                     "version": "6.5.4"
                 },
                 {
                     "bom-ref": "my-specific-bom-ref-for-another-nested-service",
                     "name": "another-nested-service"
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin`

 * *Files 4% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin`

```diff
@@ -15,14 +15,15 @@
     </component>
   </metadata>
   <services>
     <service bom-ref="my-specific-bom-ref-for-my-first-service">
       <provider>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
@@ -61,14 +62,15 @@
         <property name="key2">val2</property>
       </properties>
       <services>
         <service bom-ref="my-specific-bom-ref-for-second-nested-service">
           <provider>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
@@ -89,14 +91,15 @@
     <service bom-ref="my-specific-bom-ref-for-my-second-service">
       <name>my-second-service</name>
       <services>
         <service bom-ref="yet-another-nested-service">
           <provider>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998883928571429%*

 * *Differences: {"'services'": "{0: {'provider': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}, "*

 * *               "'services': {0: {'provider': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}}}, 1: {'services': {0: {'provider': {'url': "*

 * *               "{insert: [(1, 'https://cyclonedx.org/docs')]}}}}}}"}*

```diff
@@ -120,15 +120,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "releaseNotes": {
                 "aliases": [
                     "First Test Release"
                 ],
                 "description": "This release is a test release",
@@ -202,15 +203,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     },
                     "version": "3.2.1",
                     "x-trust-boundary": false
                 },
                 {
                     "bom-ref": "my-specific-bom-ref-for-first-nested-service",
@@ -238,15 +240,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     },
                     "version": "6.5.4"
                 },
                 {
                     "bom-ref": "my-specific-bom-ref-for-another-nested-service",
                     "name": "another-nested-service"
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin`

 * *Files 2% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin`

```diff
@@ -41,14 +41,15 @@
     </component>
   </metadata>
   <services>
     <service bom-ref="my-specific-bom-ref-for-my-first-service">
       <provider>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
@@ -87,14 +88,15 @@
         <property name="key2">val2</property>
       </properties>
       <services>
         <service bom-ref="my-specific-bom-ref-for-second-nested-service">
           <provider>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
@@ -159,14 +161,15 @@
     <service bom-ref="my-specific-bom-ref-for-my-second-service">
       <name>my-second-service</name>
       <services>
         <service bom-ref="yet-another-nested-service">
           <provider>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998883928571429%*

 * *Differences: {"'services'": "{0: {'provider': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}, "*

 * *               "'services': {0: {'provider': {'url': {insert: [(1, "*

 * *               "'https://cyclonedx.org/docs')]}}}}}, 1: {'services': {0: {'provider': {'url': "*

 * *               "{insert: [(1, 'https://cyclonedx.org/docs')]}}}}}}"}*

```diff
@@ -120,15 +120,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "releaseNotes": {
                 "aliases": [
                     "First Test Release"
                 ],
                 "description": "This release is a test release",
@@ -202,15 +203,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     },
                     "version": "3.2.1",
                     "x-trust-boundary": false
                 },
                 {
                     "bom-ref": "my-specific-bom-ref-for-first-nested-service",
@@ -238,15 +240,16 @@
                             {
                                 "email": "paul.horton@owasp.org",
                                 "name": "Paul Horton"
                             }
                         ],
                         "name": "CycloneDX",
                         "url": [
-                            "https://cyclonedx.org"
+                            "https://cyclonedx.org",
+                            "https://cyclonedx.org/docs"
                         ]
                     },
                     "version": "6.5.4"
                 },
                 {
                     "bom-ref": "my-specific-bom-ref-for-another-nested-service",
                     "name": "another-nested-service"
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin`

 * *Files 2% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin`

```diff
@@ -41,14 +41,15 @@
     </component>
   </metadata>
   <services>
     <service bom-ref="my-specific-bom-ref-for-my-first-service">
       <provider>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
@@ -87,14 +88,15 @@
         <property name="key2">val2</property>
       </properties>
       <services>
         <service bom-ref="my-specific-bom-ref-for-second-nested-service">
           <provider>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
@@ -159,14 +161,15 @@
     <service bom-ref="my-specific-bom-ref-for-my-second-service">
       <name>my-second-service</name>
       <services>
         <service bom-ref="yet-another-nested-service">
           <provider>
             <name>CycloneDX</name>
             <url>https://cyclonedx.org</url>
+            <url>https://cyclonedx.org/docs</url>
             <contact>
               <name>A N Other</name>
               <email>someone@somewhere.tld</email>
               <phone>+44 (0)1234 567890</phone>
             </contact>
             <contact>
               <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998914930555556%*

 * *Differences: {"'services'": "{0: {'provider': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}}}"}*

```diff
@@ -70,15 +70,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "version": "1.2.3",
             "x-trust-boundary": true
         },
         {
             "bom-ref": "my-specific-bom-ref-for-my-second-service",
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin`

 * *Files 9% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin`

```diff
@@ -15,14 +15,15 @@
     </component>
   </metadata>
   <services>
     <service bom-ref="my-specific-bom-ref-for-my-first-service">
       <provider>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998998397435898%*

 * *Differences: {"'services'": "{0: {'provider': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}}}"}*

```diff
@@ -86,15 +86,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "version": "1.2.3",
             "x-trust-boundary": true
         },
         {
             "bom-ref": "my-specific-bom-ref-for-my-second-service",
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin`

 * *Files 3% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin`

```diff
@@ -15,14 +15,15 @@
     </component>
   </metadata>
   <services>
     <service bom-ref="my-specific-bom-ref-for-my-first-service">
       <provider>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999069940476191%*

 * *Differences: {"'services'": "{0: {'provider': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}}}"}*

```diff
@@ -120,15 +120,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "releaseNotes": {
                 "aliases": [
                     "First Test Release"
                 ],
                 "description": "This release is a test release",
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin`

 * *Files 0% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin`

```diff
@@ -41,14 +41,15 @@
     </component>
   </metadata>
   <services>
     <service bom-ref="my-specific-bom-ref-for-my-first-service">
       <provider>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999069940476191%*

 * *Differences: {"'services'": "{0: {'provider': {'url': {insert: [(1, 'https://cyclonedx.org/docs')]}}}}"}*

```diff
@@ -120,15 +120,16 @@
                     {
                         "email": "paul.horton@owasp.org",
                         "name": "Paul Horton"
                     }
                 ],
                 "name": "CycloneDX",
                 "url": [
-                    "https://cyclonedx.org"
+                    "https://cyclonedx.org",
+                    "https://cyclonedx.org/docs"
                 ]
             },
             "releaseNotes": {
                 "aliases": [
                     "First Test Release"
                 ],
                 "description": "This release is a test release",
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin`

 * *Files 0% similar despite different names*

#### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin`

```diff
@@ -41,14 +41,15 @@
     </component>
   </metadata>
   <services>
     <service bom-ref="my-specific-bom-ref-for-my-first-service">
       <provider>
         <name>CycloneDX</name>
         <url>https://cyclonedx.org</url>
+        <url>https://cyclonedx.org/docs</url>
         <contact>
           <name>A N Other</name>
           <email>someone@somewhere.tld</email>
           <phone>+44 (0)1234 567890</phone>
         </contact>
         <contact>
           <name>Paul Horton</name>
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin` & `cyclonedx_python_lib-7.0.0a1/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_component.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_deserialize_json.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_deserialize_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 @ddt
 class TestDeserializeJson(TestCase, SnapshotMixin, DeepCompareMixin):
 
     @named_data(*all_get_bom_funct_valid_immut)
     @patch('cyclonedx.model.ThisTool._version', 'TESTING')
     def test_prepared(self, get_bom: Callable[[], Bom], *_: Any, **__: Any) -> None:
         # only latest schema will have all data populated in serialized form
-        snapshot_name = mksname(get_bom, SchemaVersion.V1_5, OutputFormat.JSON)
+        snapshot_name = mksname(get_bom, SchemaVersion.V1_6, OutputFormat.JSON)
         expected = get_bom()
         json = json_loads(self.readSnapshot(snapshot_name))
         bom = Bom.from_json(json)
         self.assertBomDeepEqual(expected, bom,
                                 fuzzy_deps=get_bom in all_get_bom_funct_with_incomplete_deps)
 
     @data(SchemaVersion.V1_4, SchemaVersion.V1_3, SchemaVersion.V1_2)
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_deserialize_xml.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_deserialize_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 @ddt
 class TestDeserializeXml(TestCase, SnapshotMixin, DeepCompareMixin):
 
     @named_data(*all_get_bom_funct_valid_immut)
     @patch('cyclonedx.model.ThisTool._version', 'TESTING')
     def test_prepared(self, get_bom: Callable[[], Bom], *_: Any, **__: Any) -> None:
         # only latest schema will have all data populated in serialized form
-        snapshot_name = mksname(get_bom, SchemaVersion.V1_5, OutputFormat.XML)
+        snapshot_name = mksname(get_bom, SchemaVersion.V1_6, OutputFormat.XML)
         expected = get_bom()
         with open(self.getSnapshotFile(snapshot_name), 'r') as s:
             bom = Bom.from_xml(s)
         self.assertBomDeepEqual(expected, bom,
                                 fuzzy_deps=get_bom in all_get_bom_funct_with_incomplete_deps)
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_enums.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_factory_license.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_factory_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,19 +35,19 @@
     ExternalReference,
     ExternalReferenceType,
     HashAlgorithm,
     HashType,
     IdentifiableAction,
     Note,
     NoteText,
-    OrganizationalContact,
     Property,
     Tool,
     XsUri,
 )
+from cyclonedx.model.contact import OrganizationalContact
 from cyclonedx.model.issue import IssueClassification, IssueType, IssueTypeSource
 from tests import reorder
 
 
 class DummyStringEnum(str, Enum):
     FIRST = 'first'
     SECOND = 'second'
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model_bom.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_bom.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 from typing import Callable, Tuple
 from unittest import TestCase
 from uuid import uuid4
 
 from ddt import ddt, named_data
 
 from cyclonedx.exception.model import LicenseExpressionAlongWithOthersException
-from cyclonedx.model import OrganizationalContact, OrganizationalEntity, Property, ThisTool, Tool
+from cyclonedx.model import Property, ThisTool, Tool
 from cyclonedx.model.bom import Bom, BomMetaData
 from cyclonedx.model.bom_ref import BomRef
 from cyclonedx.model.component import Component, ComponentType
+from cyclonedx.model.contact import OrganizationalContact, OrganizationalEntity
 from cyclonedx.model.license import DisjunctiveLicense
 from tests._data.models import (
     get_bom_component_licenses_invalid,
     get_bom_component_nested_licenses_invalid,
     get_bom_for_issue_275_components,
     get_bom_metadata_component_licenses_invalid,
     get_bom_metadata_component_nested_licenses_invalid,
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model_bom_ref.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model_component.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model_dependency.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model_issue.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model_license.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model_release_note.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model_service.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_service.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_model_vulnerability.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_model_vulnerability.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_output.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_output_json.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_output_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,26 @@
 from unittest import TestCase
 from unittest.mock import Mock, patch
 from warnings import warn
 
 from ddt import data, ddt, idata, named_data, unpack
 
 from cyclonedx.exception import CycloneDxException, MissingOptionalDependencyException
-from cyclonedx.exception.model import LicenseExpressionAlongWithOthersException, UnknownComponentDependencyException
+from cyclonedx.exception.model import (
+    InvalidOmniBorIdException,
+    InvalidSwhidException,
+    LicenseExpressionAlongWithOthersException,
+    UnknownComponentDependencyException,
+)
 from cyclonedx.exception.output import FormatNotSupportedException
 from cyclonedx.model.bom import Bom
 from cyclonedx.output.json import BY_SCHEMA_VERSION, Json
 from cyclonedx.schema import OutputFormat, SchemaVersion
 from cyclonedx.validation.json import JsonStrictValidator
-from tests import SnapshotMixin, mksname
+from tests import SnapshotMixin, is_valid_for_schema_version, mksname
 from tests._data.models import all_get_bom_funct_invalid, all_get_bom_funct_valid, bom_all_same_bomref
 
 UNSUPPORTED_SV = frozenset((SchemaVersion.V1_1, SchemaVersion.V1_0,))
 
 
 @ddt
 class TestOutputJson(TestCase, SnapshotMixin):
@@ -44,45 +49,53 @@
     def test_unsupported_schema_raises(self, sv: SchemaVersion) -> None:
         outputter_class = BY_SCHEMA_VERSION[sv]
         self.assertTrue(issubclass(outputter_class, Json))
         outputter = outputter_class(Mock(spec=Bom))
         with self.assertRaises(FormatNotSupportedException):
             outputter.output_as_string()
 
-    @named_data(*((f'{n}-{sv.to_version()}', gb, sv)
-                  for n, gb in all_get_bom_funct_valid
-                  for sv in SchemaVersion
-                  if sv not in UNSUPPORTED_SV))
+    @named_data(*(
+        (f'{n}-{sv.to_version()}', gb, sv)
+        for n, gb in all_get_bom_funct_valid
+        for sv in SchemaVersion
+        if sv not in UNSUPPORTED_SV
+        and is_valid_for_schema_version(gb, sv)
+    ))
     @unpack
     @patch('cyclonedx.model.ThisTool._version', 'TESTING')
     def test_valid(self, get_bom: Callable[[], Bom], sv: SchemaVersion, *_: Any, **__: Any) -> None:
         snapshot_name = mksname(get_bom, sv, OutputFormat.JSON)
         bom = get_bom()
         json = BY_SCHEMA_VERSION[sv](bom).output_as_string(indent=2)
         try:
             errors = JsonStrictValidator(sv).validate_str(json)
         except MissingOptionalDependencyException:
             warn('!!! skipped schema validation',
                  category=UserWarning, stacklevel=0)
         else:
-            self.assertIsNone(errors)
+            self.assertIsNone(errors, json)
         self.assertEqualSnapshot(json, snapshot_name)
 
-    @named_data(*((f'{n}-{sv.to_version()}', gb, sv)
-                  for n, gb in all_get_bom_funct_invalid
-                  for sv in SchemaVersion
-                  if sv not in UNSUPPORTED_SV))
+    @named_data(*(
+        (f'{n}-{sv.to_version()}', gb, sv)
+        for n, gb in all_get_bom_funct_invalid
+        for sv in SchemaVersion
+        if sv not in UNSUPPORTED_SV
+        and is_valid_for_schema_version(gb, sv)
+    ))
     @unpack
     def test_invalid(self, get_bom: Callable[[], Bom], sv: SchemaVersion) -> None:
-        bom = get_bom()
-        outputter = BY_SCHEMA_VERSION[sv](bom)
         with self.assertRaises(CycloneDxException) as error:
+            bom = get_bom()
+            outputter = BY_SCHEMA_VERSION[sv](bom)
             outputter.output_as_string()
         if isinstance(error.exception, (
             LicenseExpressionAlongWithOthersException,
+            InvalidOmniBorIdException,
+            InvalidSwhidException,
             UnknownComponentDependencyException,
         )):
             return None  # expected
         raise error.exception
 
     def test_bomref_not_duplicate(self) -> None:
         bom, nr_bomrefs = bom_all_same_bomref()
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_output_xml.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_output_xml.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,55 +20,70 @@
 from unittest import TestCase
 from unittest.mock import Mock, patch
 from warnings import warn
 
 from ddt import ddt, idata, named_data, unpack
 
 from cyclonedx.exception import CycloneDxException, MissingOptionalDependencyException
-from cyclonedx.exception.model import LicenseExpressionAlongWithOthersException, UnknownComponentDependencyException
+from cyclonedx.exception.model import (
+    InvalidOmniBorIdException,
+    InvalidSwhidException,
+    LicenseExpressionAlongWithOthersException,
+    UnknownComponentDependencyException,
+)
 from cyclonedx.model.bom import Bom
 from cyclonedx.output.xml import BY_SCHEMA_VERSION, Xml
 from cyclonedx.schema import OutputFormat, SchemaVersion
 from cyclonedx.validation.xml import XmlValidator
-from tests import SnapshotMixin, mksname
+from tests import SnapshotMixin, is_valid_for_schema_version, mksname
 from tests._data.models import all_get_bom_funct_invalid, all_get_bom_funct_valid, bom_all_same_bomref
 
 
 @ddt
 class TestOutputXml(TestCase, SnapshotMixin):
 
     @named_data(*(
-        (f'{n}-{sv.to_version()}', gb, sv) for n, gb in all_get_bom_funct_valid for sv in SchemaVersion
+        (f'{n}-{sv.to_version()}', gb, sv)
+        for n, gb in all_get_bom_funct_valid
+        for sv in SchemaVersion
+        if is_valid_for_schema_version(gb, sv)
     ))
     @unpack
     @patch('cyclonedx.model.ThisTool._version', 'TESTING')
     def test_valid(self, get_bom: Callable[[], Bom], sv: SchemaVersion, *_: Any, **__: Any) -> None:
         snapshot_name = mksname(get_bom, sv, OutputFormat.XML)
+        if snapshot_name is None:
+            return
         bom = get_bom()
         xml = BY_SCHEMA_VERSION[sv](bom).output_as_string(indent=2)
         try:
             errors = XmlValidator(sv).validate_str(xml)
         except MissingOptionalDependencyException:
             warn('!!! skipped schema validation',
                  category=UserWarning, stacklevel=0)
         else:
-            self.assertIsNone(errors)
+            self.assertIsNone(errors, xml)
         self.assertEqualSnapshot(xml, snapshot_name)
 
     @named_data(*(
-        (f'{n}-{sv.to_version()}', gb, sv) for n, gb in all_get_bom_funct_invalid for sv in SchemaVersion
+        (f'{n}-{sv.to_version()}', gb, sv)
+        for n, gb in all_get_bom_funct_invalid
+        for sv in SchemaVersion
+        if is_valid_for_schema_version(gb, sv)
     ))
     @unpack
     def test_invalid(self, get_bom: Callable[[], Bom], sv: SchemaVersion) -> None:
-        bom = get_bom()
-        outputter = BY_SCHEMA_VERSION[sv](bom)
         with self.assertRaises(CycloneDxException) as error:
+            bom = get_bom()
+            outputter = BY_SCHEMA_VERSION[sv](bom)
             outputter.output_as_string()
         if isinstance(error.exception, (
             LicenseExpressionAlongWithOthersException,
+            InvalidOmniBorIdException,
+            InvalidSwhidException,
             UnknownComponentDependencyException,
         )):
             return None  # expected
         raise error.exception
 
     def test_bomref_not_duplicate(self) -> None:
         bom, nr_bomrefs = bom_all_same_bomref()
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_real_world_examples.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_real_world_examples.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_schema_SchemaVersion.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_schema_SchemaVersion.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,20 +17,23 @@
 
 from unittest import TestCase
 
 from ddt import ddt, idata, unpack
 
 from cyclonedx.schema import SchemaVersion
 
-SORTED_SV = (SchemaVersion.V1_5,
-             SchemaVersion.V1_4,
-             SchemaVersion.V1_3,
-             SchemaVersion.V1_2,
-             SchemaVersion.V1_1,
-             SchemaVersion.V1_0)
+SORTED_SV = (
+    SchemaVersion.V1_6,
+    SchemaVersion.V1_5,
+    SchemaVersion.V1_4,
+    SchemaVersion.V1_3,
+    SchemaVersion.V1_2,
+    SchemaVersion.V1_1,
+    SchemaVersion.V1_0
+)
 
 # do not use any value-comparisons or implicit hash-functions here !
 # just work with the position in tuple SORTED_SCHEMA_VERSIONS
 td_gt = tuple((a, b) for i, a in enumerate(SORTED_SV) for b in SORTED_SV[i + 1:])
 td_ge = tuple((a, b) for i, a in enumerate(SORTED_SV) for b in SORTED_SV[i:])
 td_eq = tuple((v, v) for v in SORTED_SV)
 td_le = tuple((b, a) for a, b in td_ge)
```

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_schema__res.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_schema__res.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_spdx.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_validation.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_validation_json.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_validation_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/tests/test_validation_xml.py` & `cyclonedx_python_lib-7.0.0a1/tests/test_validation_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.4/PKG-INFO` & `cyclonedx_python_lib-7.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclonedx-python-lib
-Version: 6.4.4
+Version: 7.0.0a1
 Summary: Python library for CycloneDX
 Home-page: https://github.com/CycloneDX/cyclonedx-python-lib/#readme
 License: Apache-2.0
 Keywords: CycloneDX,library,OWASP,SCA,Software Bill of Materials,Bill of Materials,BOM,SBOM,VEX,VDR,OBOM,MBOM,SaaSBOM,SPDX,PackageURL,PURL
 Author: Paul Horton
 Author-email: phorton@sonatype.com
 Maintainer: Jan Kowalleck
@@ -29,15 +29,15 @@
 Provides-Extra: json-validation
 Provides-Extra: validation
 Provides-Extra: xml-validation
 Requires-Dist: jsonschema[format] (>=4.18,<5.0) ; extra == "validation" or extra == "json-validation"
 Requires-Dist: license-expression (>=30,<31)
 Requires-Dist: lxml (>=4,<6) ; extra == "validation" or extra == "xml-validation"
 Requires-Dist: packageurl-python (>=0.11,<2)
-Requires-Dist: py-serializable (>=0.16,<2)
+Requires-Dist: py-serializable (>=1.0.3,<2)
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/CycloneDX/cyclonedx-python-lib/issues
 Project-URL: Documentation, https://cyclonedx-python-library.readthedocs.io/
 Project-URL: Funding, https://owasp.org/donate/?reponame=www-project-cyclonedx&title=OWASP+CycloneDX
 Project-URL: Repository, https://github.com/CycloneDX/cyclonedx-python-lib
 Description-Content-Type: text/markdown
```

