# Comparing `tmp/cyclonedx_python_lib-6.4.3.tar.gz` & `tmp/cyclonedx_python_lib-6.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx_python_lib-6.4.3.tar", max compression
+gzip compressed data, was "cyclonedx_python_lib-6.4.4.tar", max compression
```

## Comparing `cyclonedx_python_lib-6.4.3.tar` & `cyclonedx_python_lib-6.4.4.tar`

### file list

```diff
@@ -1,899 +1,899 @@
--rw-r--r--   0        0        0   215304 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/LICENSE
--rw-r--r--   0        0        0      147 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/NOTICE
--rw-r--r--   0        0        0     4569 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/README.md
--rw-r--r--   0        0        0      850 2024-03-04 12:10:52.524222 cyclonedx_python_lib-6.4.3/cyclonedx/__init__.py
--rw-r--r--   0        0        0      731 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/_internal/__init__.py
--rw-r--r--   0        0        0     1734 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/_internal/compare.py
--rw-r--r--   0        0        0     1164 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/_internal/hash.py
--rw-r--r--   0        0        0      847 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/_internal/time.py
--rw-r--r--   0        0        0      993 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/exception/__init__.py
--rw-r--r--   0        0        0     1536 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/exception/factory.py
--rw-r--r--   0        0        0     2642 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/exception/model.py
--rw-r--r--   0        0        0     1136 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/exception/output.py
--rw-r--r--   0        0        0     1730 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/exception/serialization.py
--rw-r--r--   0        0        0      680 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/factory/__init__.py
--rw-r--r--   0        0        0     3233 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/factory/license.py
--rw-r--r--   0        0        0    48114 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/model/__init__.py
--rw-r--r--   0        0        0    23268 2024-03-04 12:10:32.507575 cyclonedx_python_lib-6.4.3/cyclonedx/model/bom.py
--rw-r--r--   0        0        0     2179 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/model/bom_ref.py
--rw-r--r--   0        0        0    47132 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/model/component.py
--rw-r--r--   0        0        0     3766 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/model/dependency.py
--rw-r--r--   0        0        0     3568 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/model/impact_analysis.py
--rw-r--r--   0        0        0     7024 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/model/issue.py
--rw-r--r--   0        0        0     8020 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/model/license.py
--rw-r--r--   0        0        0     8623 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/model/release_note.py
--rw-r--r--   0        0        0    12676 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/model/service.py
--rw-r--r--   0        0        0    43554 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/model/vulnerability.py
--rw-r--r--   0        0        0     5872 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/output/__init__.py
--rw-r--r--   0        0        0     4060 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/output/json.py
--rw-r--r--   0        0        0     4173 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/output/xml.py
--rw-r--r--   0        0        0      153 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/py.typed
--rw-r--r--   0        0        0     3000 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/__init__.py
--rw-r--r--   0        0        0     1961 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/README.md
--rw-r--r--   0        0        0     2364 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/__init__.py
--rw-r--r--   0        0        0    13604 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd
--rw-r--r--   0        0        0    39716 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd
--rw-r--r--   0        0        0    37194 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    36226 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    76383 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd
--rw-r--r--   0        0        0    40408 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    39348 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    88794 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd
--rw-r--r--   0        0        0    72383 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   133792 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd
--rw-r--r--   0        0        0   164772 2024-03-04 12:10:32.511575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   311805 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd
--rw-r--r--   0        0        0     8058 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    12322 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   144335 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd
--rw-r--r--   0        0        0     2367 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/schema/schema.py
--rw-r--r--   0        0        0     6479 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/serialization/__init__.py
--rw-r--r--   0        0        0     2503 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/spdx.py
--rw-r--r--   0        0        0     3701 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/validation/__init__.py
--rw-r--r--   0        0        0     4817 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/validation/json.py
--rw-r--r--   0        0        0      853 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/validation/model.py
--rw-r--r--   0        0        0     3673 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/cyclonedx/validation/xml.py
--rw-r--r--   0        0        0      634 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/Makefile
--rw-r--r--   0        0        0     1524 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/architecture.rst
--rw-r--r--   0        0        0      686 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/changelog.rst
--rw-r--r--   0        0        0     2657 2024-03-04 12:10:52.524222 cyclonedx_python_lib-6.4.3/docs/conf.py
--rw-r--r--   0        0        0       34 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/contributing.rst
--rw-r--r--   0        0        0      895 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/examples.rst
--rw-r--r--   0        0        0     1857 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/index.rst
--rw-r--r--   0        0        0     1499 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/install.rst
--rw-r--r--   0        0        0      800 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/make.bat
--rw-r--r--   0        0        0     3275 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/modelling.rst
--rw-r--r--   0        0        0     2269 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/outputting.rst
--rw-r--r--   0        0        0       81 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/requirements.txt
--rw-r--r--   0        0        0     4961 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/schema-support.rst
--rw-r--r--   0        0        0     1329 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/docs/support.rst
--rw-r--r--   0        0        0      176 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/examples/README.md
--rw-r--r--   0        0        0     8164 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/examples/complex_deserialize.py
--rw-r--r--   0        0        0     4046 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/examples/complex_serialize.py
--rw-r--r--   0        0        0     4226 2024-03-04 12:10:52.524222 cyclonedx_python_lib-6.4.3/pyproject.toml
--rw-r--r--   0        0        0     5985 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/tests/__init__.py
--rw-r--r--   0        0        0      704 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/tests/_data/__init__.py
--rw-r--r--   0        0        0    31717 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/tests/_data/models.py
--rw-r--r--   0        0        0       16 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/tests/_data/own/README.md
--rw-r--r--   0        0        0     1309 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/tests/_data/own/json/1.2/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1309 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/tests/_data/own/json/1.3/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1309 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/tests/_data/own/json/1.4/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     2461 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/tests/_data/own/xml/1.4/bom_setuptools.xml
--rw-r--r--   0        0        0    98508 2024-03-04 12:10:32.515575 cyclonedx_python_lib-6.4.3/tests/_data/own/xml/1.4/webgoat-6.1.xml
--rw-r--r--   0        0        0     3723 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml
--rw-r--r--   0        0        0     1195 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml
--rw-r--r--   0        0        0      559 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml
--rw-r--r--   0        0        0      313 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-component-type-1.1.xml
--rw-r--r--   0        0        0      246 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-empty-component-1.1.xml
--rw-r--r--   0        0        0      830 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml
--rw-r--r--   0        0        0      801 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml
--rw-r--r--   0        0        0      793 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml
--rw-r--r--   0        0        0      769 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml
--rw-r--r--   0        0        0      705 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml
--rw-r--r--   0        0        0     1303 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml
--rw-r--r--   0        0        0    16515 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml
--rw-r--r--   0        0        0    16513 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml
--rw-r--r--   0        0        0     1328 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml
--rw-r--r--   0        0        0     1366 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml
--rw-r--r--   0        0        0      302 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-missing-component-type-1.1.xml
--rw-r--r--   0        0        0    21038 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml
--rw-r--r--   0        0        0      348 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-scope-1.1.xml
--rw-r--r--   0        0        0    21026 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml
--rw-r--r--   0        0        0    21039 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml
--rw-r--r--   0        0        0     1217 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml
--rw-r--r--   0        0        0      704 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml
--rw-r--r--   0        0        0      965 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml
--rw-r--r--   0        0        0      186 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-empty-components-1.1.xml
--rw-r--r--   0        0        0    22339 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml
--rw-r--r--   0        0        0     1210 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml
--rw-r--r--   0        0        0     1214 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml
--rw-r--r--   0        0        0     1226 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml
--rw-r--r--   0        0        0      317 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-minimal-viable-1.1.xml
--rw-r--r--   0        0        0    21121 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml
--rw-r--r--   0        0        0    10048 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml
--rw-r--r--   0        0        0      165 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-bomformat-1.2.json
--rw-r--r--   0        0        0      394 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.json
--rw-r--r--   0        0        0      560 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml
--rw-r--r--   0        0        0      385 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.json
--rw-r--r--   0        0        0      433 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.xml
--rw-r--r--   0        0        0      249 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.json
--rw-r--r--   0        0        0      314 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.xml
--rw-r--r--   0        0        0      667 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json
--rw-r--r--   0        0        0      809 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml
--rw-r--r--   0        0        0      247 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-empty-component-1.2.xml
--rw-r--r--   0        0        0      856 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json
--rw-r--r--   0        0        0      831 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml
--rw-r--r--   0        0        0      827 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json
--rw-r--r--   0        0        0      802 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml
--rw-r--r--   0        0        0      819 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json
--rw-r--r--   0        0        0      794 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml
--rw-r--r--   0        0        0      795 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json
--rw-r--r--   0        0        0      770 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml
--rw-r--r--   0        0        0      731 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json
--rw-r--r--   0        0        0      706 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml
--rw-r--r--   0        0        0     1184 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json
--rw-r--r--   0        0        0     1554 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml
--rw-r--r--   0        0        0      515 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json
--rw-r--r--   0        0        0     1304 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml
--rw-r--r--   0        0        0    15788 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json
--rw-r--r--   0        0        0    16516 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml
--rw-r--r--   0        0        0      428 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.json
--rw-r--r--   0        0        0    16514 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml
--rw-r--r--   0        0        0     1329 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml
--rw-r--r--   0        0        0     1367 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml
--rw-r--r--   0        0        0      209 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      244 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      303 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-missing-component-type-1.2.xml
--rw-r--r--   0        0        0    21039 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml
--rw-r--r--   0        0        0     1185 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json
--rw-r--r--   0        0        0     1555 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml
--rw-r--r--   0        0        0      275 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-scope-1.2.json
--rw-r--r--   0        0        0      349 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-scope-1.2.xml
--rw-r--r--   0        0        0      148 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.json
--rw-r--r--   0        0        0    21027 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.json
--rw-r--r--   0        0        0      416 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.xml
--rw-r--r--   0        0        0      363 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/skip_invalid-empty-component-1.2.json
--rw-r--r--   0        0        0      361 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/skip_invalid-missing-component-type-1.2.json
--rw-r--r--   0        0        0      548 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json
--rw-r--r--   0        0        0      792 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml
--rw-r--r--   0        0        0    20390 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-bom-1.2.json
--rw-r--r--   0        0        0    24278 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml
--rw-r--r--   0        0        0     2163 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json
--rw-r--r--   0        0        0     1897 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml
--rw-r--r--   0        0        0      394 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.json
--rw-r--r--   0        0        0      705 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml
--rw-r--r--   0        0        0      456 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.json
--rw-r--r--   0        0        0      492 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.xml
--rw-r--r--   0        0        0     1342 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json
--rw-r--r--   0        0        0     1346 2024-03-04 12:10:32.519575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml
--rw-r--r--   0        0        0      892 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json
--rw-r--r--   0        0        0     1223 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml
--rw-r--r--   0        0        0      693 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json
--rw-r--r--   0        0        0      824 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml
--rw-r--r--   0        0        0      161 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.json
--rw-r--r--   0        0        0      187 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.xml
--rw-r--r--   0        0        0    22340 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml
--rw-r--r--   0        0        0      438 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.json
--rw-r--r--   0        0        0     1211 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-license-id-1.2.json
--rw-r--r--   0        0        0     1215 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml
--rw-r--r--   0        0        0      440 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-license-name-1.2.json
--rw-r--r--   0        0        0     1227 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml
--rw-r--r--   0        0        0      333 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.json
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.xml
--rw-r--r--   0        0        0      438 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.json
--rw-r--r--   0        0        0      492 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.xml
--rw-r--r--   0        0        0      417 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.json
--rw-r--r--   0        0        0      468 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.xml
--rw-r--r--   0        0        0      224 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      254 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      605 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json
--rw-r--r--   0        0        0      654 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml
--rw-r--r--   0        0        0      253 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.json
--rw-r--r--   0        0        0      318 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.xml
--rw-r--r--   0        0        0     2465 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-patch-1.2.json
--rw-r--r--   0        0        0     3337 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml
--rw-r--r--   0        0        0    21122 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml
--rw-r--r--   0        0        0     2308 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-service-1.2.json
--rw-r--r--   0        0        0     2693 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-service-1.2.xml
--rw-r--r--   0        0        0      419 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.json
--rw-r--r--   0        0        0      495 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.xml
--rw-r--r--   0        0        0    11181 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml
--rw-r--r--   0        0        0      165 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-bomformat-1.3.json
--rw-r--r--   0        0        0      394 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.json
--rw-r--r--   0        0        0      560 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml
--rw-r--r--   0        0        0      385 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.json
--rw-r--r--   0        0        0      433 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.xml
--rw-r--r--   0        0        0      249 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.json
--rw-r--r--   0        0        0      314 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.xml
--rw-r--r--   0        0        0      667 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json
--rw-r--r--   0        0        0      809 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml
--rw-r--r--   0        0        0      197 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.json
--rw-r--r--   0        0        0      247 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.xml
--rw-r--r--   0        0        0      856 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json
--rw-r--r--   0        0        0      831 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml
--rw-r--r--   0        0        0      827 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json
--rw-r--r--   0        0        0      802 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml
--rw-r--r--   0        0        0      819 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json
--rw-r--r--   0        0        0      794 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml
--rw-r--r--   0        0        0      795 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json
--rw-r--r--   0        0        0      770 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml
--rw-r--r--   0        0        0      731 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json
--rw-r--r--   0        0        0      706 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml
--rw-r--r--   0        0        0     1184 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json
--rw-r--r--   0        0        0     1554 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml
--rw-r--r--   0        0        0      515 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json
--rw-r--r--   0        0        0     1304 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml
--rw-r--r--   0        0        0    15788 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json
--rw-r--r--   0        0        0    16516 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml
--rw-r--r--   0        0        0      428 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.json
--rw-r--r--   0        0        0    16514 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml
--rw-r--r--   0        0        0     1329 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml
--rw-r--r--   0        0        0     1367 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml
--rw-r--r--   0        0        0      277 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.json
--rw-r--r--   0        0        0      319 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      209 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      244 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      228 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.json
--rw-r--r--   0        0        0      303 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.xml
--rw-r--r--   0        0        0    21039 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml
--rw-r--r--   0        0        0     1185 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json
--rw-r--r--   0        0        0     1555 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml
--rw-r--r--   0        0        0      275 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-scope-1.3.json
--rw-r--r--   0        0        0      349 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-scope-1.3.xml
--rw-r--r--   0        0        0      148 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.json
--rw-r--r--   0        0        0    21027 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.json
--rw-r--r--   0        0        0      416 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.xml
--rw-r--r--   0        0        0      548 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json
--rw-r--r--   0        0        0      792 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml
--rw-r--r--   0        0        0    20390 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-bom-1.3.json
--rw-r--r--   0        0        0    24278 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml
--rw-r--r--   0        0        0     2163 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json
--rw-r--r--   0        0        0     1897 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml
--rw-r--r--   0        0        0      394 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.json
--rw-r--r--   0        0        0      705 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml
--rw-r--r--   0        0        0      456 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.json
--rw-r--r--   0        0        0      492 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.xml
--rw-r--r--   0        0        0     1342 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json
--rw-r--r--   0        0        0     1346 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml
--rw-r--r--   0        0        0      892 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json
--rw-r--r--   0        0        0     1223 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml
--rw-r--r--   0        0        0     1497 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json
--rw-r--r--   0        0        0     1983 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml
--rw-r--r--   0        0        0      693 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json
--rw-r--r--   0        0        0      824 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml
--rw-r--r--   0        0        0      161 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.json
--rw-r--r--   0        0        0      187 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.xml
--rw-r--r--   0        0        0     1384 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json
--rw-r--r--   0        0        0     1596 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml
--rw-r--r--   0        0        0    22340 2024-03-04 12:10:32.523575 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml
--rw-r--r--   0        0        0     1117 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json
--rw-r--r--   0        0        0     1324 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml
--rw-r--r--   0        0        0      438 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.json
--rw-r--r--   0        0        0     1211 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-license-id-1.3.json
--rw-r--r--   0        0        0     1215 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml
--rw-r--r--   0        0        0      440 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-license-name-1.3.json
--rw-r--r--   0        0        0     1227 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml
--rw-r--r--   0        0        0      333 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.json
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.xml
--rw-r--r--   0        0        0      279 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.json
--rw-r--r--   0        0        0      321 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      438 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.json
--rw-r--r--   0        0        0      492 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.xml
--rw-r--r--   0        0        0      417 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.json
--rw-r--r--   0        0        0      468 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.xml
--rw-r--r--   0        0        0      224 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      254 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      605 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json
--rw-r--r--   0        0        0      654 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml
--rw-r--r--   0        0        0      253 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.json
--rw-r--r--   0        0        0      318 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.xml
--rw-r--r--   0        0        0     2465 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-patch-1.3.json
--rw-r--r--   0        0        0     3337 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml
--rw-r--r--   0        0        0      983 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-properties-1.3.json
--rw-r--r--   0        0        0     1213 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml
--rw-r--r--   0        0        0    21122 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml
--rw-r--r--   0        0        0     2308 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-service-1.3.json
--rw-r--r--   0        0        0     2693 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-service-1.3.xml
--rw-r--r--   0        0        0      419 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.json
--rw-r--r--   0        0        0      495 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.xml
--rw-r--r--   0        0        0    11181 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml
--rw-r--r--   0        0        0      165 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-bomformat-1.4.json
--rw-r--r--   0        0        0      394 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.json
--rw-r--r--   0        0        0      560 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml
--rw-r--r--   0        0        0      385 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.json
--rw-r--r--   0        0        0      433 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.xml
--rw-r--r--   0        0        0      249 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.json
--rw-r--r--   0        0        0      314 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.xml
--rw-r--r--   0        0        0      667 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json
--rw-r--r--   0        0        0      809 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml
--rw-r--r--   0        0        0      197 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.json
--rw-r--r--   0        0        0      247 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.xml
--rw-r--r--   0        0        0      856 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json
--rw-r--r--   0        0        0      831 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml
--rw-r--r--   0        0        0      827 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json
--rw-r--r--   0        0        0      802 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml
--rw-r--r--   0        0        0      819 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json
--rw-r--r--   0        0        0      794 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml
--rw-r--r--   0        0        0      795 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json
--rw-r--r--   0        0        0      770 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml
--rw-r--r--   0        0        0      731 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json
--rw-r--r--   0        0        0      706 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml
--rw-r--r--   0        0        0     1184 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json
--rw-r--r--   0        0        0     1554 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml
--rw-r--r--   0        0        0      515 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json
--rw-r--r--   0        0        0     1304 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml
--rw-r--r--   0        0        0    15788 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json
--rw-r--r--   0        0        0    16516 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml
--rw-r--r--   0        0        0      428 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.json
--rw-r--r--   0        0        0    16514 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml
--rw-r--r--   0        0        0     1329 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml
--rw-r--r--   0        0        0     1367 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml
--rw-r--r--   0        0        0      277 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.json
--rw-r--r--   0        0        0      319 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      209 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      244 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      228 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.json
--rw-r--r--   0        0        0      303 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.xml
--rw-r--r--   0        0        0    21039 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml
--rw-r--r--   0        0        0     1185 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json
--rw-r--r--   0        0        0     1555 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml
--rw-r--r--   0        0        0      275 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-scope-1.4.json
--rw-r--r--   0        0        0      349 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-scope-1.4.xml
--rw-r--r--   0        0        0      148 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.json
--rw-r--r--   0        0        0    21027 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.json
--rw-r--r--   0        0        0      416 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.xml
--rw-r--r--   0        0        0      548 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json
--rw-r--r--   0        0        0      792 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml
--rw-r--r--   0        0        0    20390 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-bom-1.4.json
--rw-r--r--   0        0        0    24278 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml
--rw-r--r--   0        0        0     2163 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json
--rw-r--r--   0        0        0     1897 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml
--rw-r--r--   0        0        0      394 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.json
--rw-r--r--   0        0        0      705 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml
--rw-r--r--   0        0        0      456 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.json
--rw-r--r--   0        0        0      492 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.xml
--rw-r--r--   0        0        0     1342 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json
--rw-r--r--   0        0        0     1346 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml
--rw-r--r--   0        0        0      892 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json
--rw-r--r--   0        0        0     1223 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml
--rw-r--r--   0        0        0     1497 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json
--rw-r--r--   0        0        0     1983 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml
--rw-r--r--   0        0        0      693 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json
--rw-r--r--   0        0        0      824 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml
--rw-r--r--   0        0        0      161 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.json
--rw-r--r--   0        0        0      187 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.xml
--rw-r--r--   0        0        0     1384 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json
--rw-r--r--   0        0        0     1596 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml
--rw-r--r--   0        0        0    22340 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml
--rw-r--r--   0        0        0     1117 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json
--rw-r--r--   0        0        0     1324 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml
--rw-r--r--   0        0        0      438 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.json
--rw-r--r--   0        0        0     1211 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-license-id-1.4.json
--rw-r--r--   0        0        0     1215 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml
--rw-r--r--   0        0        0      440 2024-03-04 12:10:32.527576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-license-name-1.4.json
--rw-r--r--   0        0        0     1227 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml
--rw-r--r--   0        0        0      333 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.json
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.xml
--rw-r--r--   0        0        0      279 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.json
--rw-r--r--   0        0        0      321 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      438 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.json
--rw-r--r--   0        0        0      492 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.xml
--rw-r--r--   0        0        0      417 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.json
--rw-r--r--   0        0        0      468 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.xml
--rw-r--r--   0        0        0      224 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      254 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      605 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json
--rw-r--r--   0        0        0      654 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml
--rw-r--r--   0        0        0      227 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.json
--rw-r--r--   0        0        0      281 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.xml
--rw-r--r--   0        0        0     2465 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-patch-1.4.json
--rw-r--r--   0        0        0     3337 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml
--rw-r--r--   0        0        0      983 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-properties-1.4.json
--rw-r--r--   0        0        0     1213 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml
--rw-r--r--   0        0        0    21122 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml
--rw-r--r--   0        0        0     5338 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json
--rw-r--r--   0        0        0     6828 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml
--rw-r--r--   0        0        0     2312 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-service-1.4.json
--rw-r--r--   0        0        0     2693 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-service-1.4.xml
--rw-r--r--   0        0        0      419 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.json
--rw-r--r--   0        0        0      495 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.xml
--rw-r--r--   0        0        0     9733 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json
--rw-r--r--   0        0        0     4274 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json
--rw-r--r--   0        0        0     5987 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml
--rw-r--r--   0        0        0    11181 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml
--rw-r--r--   0        0        0      165 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-bomformat-1.5.json
--rw-r--r--   0        0        0      508 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.json
--rw-r--r--   0        0        0      866 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml
--rw-r--r--   0        0        0      385 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.json
--rw-r--r--   0        0        0      433 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.xml
--rw-r--r--   0        0        0      249 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.json
--rw-r--r--   0        0        0      314 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.xml
--rw-r--r--   0        0        0      746 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json
--rw-r--r--   0        0        0     1086 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml
--rw-r--r--   0        0        0      197 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.json
--rw-r--r--   0        0        0      247 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.xml
--rw-r--r--   0        0        0      856 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json
--rw-r--r--   0        0        0      831 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml
--rw-r--r--   0        0        0      827 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json
--rw-r--r--   0        0        0      802 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml
--rw-r--r--   0        0        0      819 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json
--rw-r--r--   0        0        0      794 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml
--rw-r--r--   0        0        0      795 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json
--rw-r--r--   0        0        0      770 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml
--rw-r--r--   0        0        0      731 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json
--rw-r--r--   0        0        0      706 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml
--rw-r--r--   0        0        0     1184 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json
--rw-r--r--   0        0        0     1554 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml
--rw-r--r--   0        0        0      515 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json
--rw-r--r--   0        0        0     1304 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml
--rw-r--r--   0        0        0    15788 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json
--rw-r--r--   0        0        0    16516 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml
--rw-r--r--   0        0        0      428 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.json
--rw-r--r--   0        0        0    16514 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml
--rw-r--r--   0        0        0     1329 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml
--rw-r--r--   0        0        0     1367 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml
--rw-r--r--   0        0        0      277 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.json
--rw-r--r--   0        0        0      319 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      209 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      244 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0      228 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.json
--rw-r--r--   0        0        0      303 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.xml
--rw-r--r--   0        0        0    21039 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml
--rw-r--r--   0        0        0     1185 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json
--rw-r--r--   0        0        0     1555 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml
--rw-r--r--   0        0        0      275 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-scope-1.5.json
--rw-r--r--   0        0        0      349 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-scope-1.5.xml
--rw-r--r--   0        0        0      148 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.json
--rw-r--r--   0        0        0    21027 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.json
--rw-r--r--   0        0        0      416 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.xml
--rw-r--r--   0        0        0     2527 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json
--rw-r--r--   0        0        0     3596 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml
--rw-r--r--   0        0        0      548 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json
--rw-r--r--   0        0        0      792 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml
--rw-r--r--   0        0        0    20390 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-bom-1.5.json
--rw-r--r--   0        0        0    24278 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml
--rw-r--r--   0        0        0     2163 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json
--rw-r--r--   0        0        0     1897 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml
--rw-r--r--   0        0        0      394 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.json
--rw-r--r--   0        0        0      705 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml
--rw-r--r--   0        0        0      456 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.json
--rw-r--r--   0        0        0      492 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.xml
--rw-r--r--   0        0        0     1342 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json
--rw-r--r--   0        0        0     1346 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml
--rw-r--r--   0        0        0      892 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json
--rw-r--r--   0        0        0     1223 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml
--rw-r--r--   0        0        0     1810 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json
--rw-r--r--   0        0        0     2449 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml
--rw-r--r--   0        0        0      693 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json
--rw-r--r--   0        0        0      824 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml
--rw-r--r--   0        0        0      161 2024-03-04 12:10:32.531576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.json
--rw-r--r--   0        0        0      187 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.xml
--rw-r--r--   0        0        0     3189 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json
--rw-r--r--   0        0        0     4519 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml
--rw-r--r--   0        0        0    22340 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml
--rw-r--r--   0        0        0     1117 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json
--rw-r--r--   0        0        0     1324 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml
--rw-r--r--   0        0        0     7703 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json
--rw-r--r--   0        0        0    11757 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml
--rw-r--r--   0        0        0      473 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.json
--rw-r--r--   0        0        0     1270 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml
--rw-r--r--   0        0        0      467 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-id-1.5.json
--rw-r--r--   0        0        0     1236 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml
--rw-r--r--   0        0        0     1539 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json
--rw-r--r--   0        0        0     2197 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml
--rw-r--r--   0        0        0      477 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-name-1.5.json
--rw-r--r--   0        0        0     1248 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml
--rw-r--r--   0        0        0    98548 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json
--rw-r--r--   0        0        0   100112 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml
--rw-r--r--   0        0        0      333 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.json
--rw-r--r--   0        0        0      430 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.xml
--rw-r--r--   0        0        0      279 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.json
--rw-r--r--   0        0        0      321 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      436 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.json
--rw-r--r--   0        0        0      624 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml
--rw-r--r--   0        0        0      507 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.json
--rw-r--r--   0        0        0      537 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml
--rw-r--r--   0        0        0      482 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.json
--rw-r--r--   0        0        0      509 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.xml
--rw-r--r--   0        0        0      224 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      254 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0     1162 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json
--rw-r--r--   0        0        0     1471 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml
--rw-r--r--   0        0        0      605 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json
--rw-r--r--   0        0        0      654 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml
--rw-r--r--   0        0        0      227 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.json
--rw-r--r--   0        0        0      281 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.xml
--rw-r--r--   0        0        0     2465 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-patch-1.5.json
--rw-r--r--   0        0        0     3337 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml
--rw-r--r--   0        0        0     1520 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-properties-1.5.json
--rw-r--r--   0        0        0     1660 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml
--rw-r--r--   0        0        0    21122 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml
--rw-r--r--   0        0        0     5338 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json
--rw-r--r--   0        0        0     6828 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml
--rw-r--r--   0        0        0     9412 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json
--rw-r--r--   0        0        0    12249 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml
--rw-r--r--   0        0        0     2312 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-service-1.5.json
--rw-r--r--   0        0        0     2693 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-service-1.5.xml
--rw-r--r--   0        0        0      419 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.json
--rw-r--r--   0        0        0      495 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.xml
--rw-r--r--   0        0        0     9733 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json
--rw-r--r--   0        0        0    17746 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json
--rw-r--r--   0        0        0    19794 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml
--rw-r--r--   0        0        0    11181 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml
--rw-r--r--   0        0        0      157 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/README.md
--rwxr-xr-x   0        0        0      739 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/fetch.sh
--rw-r--r--   0        0        0      391 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/README.md
--rw-r--r--   0        0        0      579 2024-03-04 12:10:32.535576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin
--rw-r--r--   0        0        0      649 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin
--rw-r--r--   0        0        0     1050 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin
--rw-r--r--   0        0        0     1055 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin
--rw-r--r--   0        0        0     1050 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin
--rw-r--r--   0        0        0     1055 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin
--rw-r--r--   0        0        0     2128 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin
--rw-r--r--   0        0        0     2211 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin
--rw-r--r--   0        0        0     2128 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin
--rw-r--r--   0        0        0     2211 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin
--rw-r--r--   0        0        0      806 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin
--rw-r--r--   0        0        0      949 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin
--rw-r--r--   0        0        0     1835 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.2.json.bin
--rw-r--r--   0        0        0     1806 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin
--rw-r--r--   0        0        0     1835 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.3.json.bin
--rw-r--r--   0        0        0     1806 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin
--rw-r--r--   0        0        0     2808 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.4.json.bin
--rw-r--r--   0        0        0     2877 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin
--rw-r--r--   0        0        0     3460 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.5.json.bin
--rw-r--r--   0        0        0     3525 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.1.xml.bin
--rw-r--r--   0        0        0      944 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.2.json.bin
--rw-r--r--   0        0        0      865 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin
--rw-r--r--   0        0        0      944 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.3.json.bin
--rw-r--r--   0        0        0      865 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin
--rw-r--r--   0        0        0     2085 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.4.json.bin
--rw-r--r--   0        0        0     2072 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin
--rw-r--r--   0        0        0     2085 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.5.json.bin
--rw-r--r--   0        0        0     2072 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.0.xml.bin
--rw-r--r--   0        0        0      496 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.1.xml.bin
--rw-r--r--   0        0        0      893 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.2.json.bin
--rw-r--r--   0        0        0      812 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.2.xml.bin
--rw-r--r--   0        0        0      893 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.3.json.bin
--rw-r--r--   0        0        0      812 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.3.xml.bin
--rw-r--r--   0        0        0     2013 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.4.json.bin
--rw-r--r--   0        0        0     2002 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.4.xml.bin
--rw-r--r--   0        0        0     2013 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.5.json.bin
--rw-r--r--   0        0        0     2002 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.0.xml.bin
--rw-r--r--   0        0        0     4093 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin
--rw-r--r--   0        0        0     4074 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin
--rw-r--r--   0        0        0     4409 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin
--rw-r--r--   0        0        0     4074 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin
--rw-r--r--   0        0        0     4409 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin
--rw-r--r--   0        0        0     5202 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin
--rw-r--r--   0        0        0     5607 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin
--rw-r--r--   0        0        0     5451 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin
--rw-r--r--   0        0        0     5856 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin
--rw-r--r--   0        0        0      749 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin
--rw-r--r--   0        0        0      793 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin
--rw-r--r--   0        0        0     1894 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin
--rw-r--r--   0        0        0     1461 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin
--rw-r--r--   0        0        0     1894 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin
--rw-r--r--   0        0        0     1461 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin
--rw-r--r--   0        0        0     3014 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin
--rw-r--r--   0        0        0     2651 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin
--rw-r--r--   0        0        0     3014 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin
--rw-r--r--   0        0        0     2651 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.xml.bin
--rw-r--r--   0        0        0     2092 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin
--rw-r--r--   0        0        0     2289 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin
--rw-r--r--   0        0        0     2092 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin
--rw-r--r--   0        0        0     2289 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.xml.bin
--rw-r--r--   0        0        0     3282 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin
--rw-r--r--   0        0        0     3686 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin
--rw-r--r--   0        0        0     3282 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin
--rw-r--r--   0        0        0     3686 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.xml.bin
--rw-r--r--   0        0        0     1827 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin
--rw-r--r--   0        0        0     2023 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin
--rw-r--r--   0        0        0     1827 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin
--rw-r--r--   0        0        0     2023 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.xml.bin
--rw-r--r--   0        0        0     2577 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin
--rw-r--r--   0        0        0     2822 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin
--rw-r--r--   0        0        0     2577 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin
--rw-r--r--   0        0        0     2822 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.1.xml.bin
--rw-r--r--   0        0        0     1081 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin
--rw-r--r--   0        0        0     1083 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin
--rw-r--r--   0        0        0     1081 2024-03-04 12:10:32.539576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin
--rw-r--r--   0        0        0     1083 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2201 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin
--rw-r--r--   0        0        0     2273 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2201 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin
--rw-r--r--   0        0        0     2273 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.1.xml.bin
--rw-r--r--   0        0        0      886 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin
--rw-r--r--   0        0        0      821 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin
--rw-r--r--   0        0        0      886 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin
--rw-r--r--   0        0        0      821 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2006 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin
--rw-r--r--   0        0        0     2011 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2006 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin
--rw-r--r--   0        0        0     2011 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.xml.bin
--rw-r--r--   0        0        0     2014 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin
--rw-r--r--   0        0        0     2243 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin
--rw-r--r--   0        0        0     2014 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin
--rw-r--r--   0        0        0     2243 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.xml.bin
--rw-r--r--   0        0        0     2025 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin
--rw-r--r--   0        0        0     2268 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin
--rw-r--r--   0        0        0     2025 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin
--rw-r--r--   0        0        0     2268 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin
--rw-r--r--   0        0        0      596 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin
--rw-r--r--   0        0        0      695 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin
--rw-r--r--   0        0        0     1561 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin
--rw-r--r--   0        0        0     1597 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin
--rw-r--r--   0        0        0     1561 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin
--rw-r--r--   0        0        0     1597 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin
--rw-r--r--   0        0        0     2702 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin
--rw-r--r--   0        0        0     2804 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin
--rw-r--r--   0        0        0     2702 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin
--rw-r--r--   0        0        0     2804 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin
--rw-r--r--   0        0        0      662 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin
--rw-r--r--   0        0        0      678 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin
--rw-r--r--   0        0        0     1385 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin
--rw-r--r--   0        0        0     1402 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin
--rw-r--r--   0        0        0     1385 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin
--rw-r--r--   0        0        0     1402 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin
--rw-r--r--   0        0        0     2526 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin
--rw-r--r--   0        0        0     2609 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin
--rw-r--r--   0        0        0     2526 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin
--rw-r--r--   0        0        0     2609 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin
--rw-r--r--   0        0        0      246 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.0.xml.bin
--rw-r--r--   0        0        0      847 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin
--rw-r--r--   0        0        0     1085 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin
--rw-r--r--   0        0        0     1163 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin
--rw-r--r--   0        0        0     1085 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin
--rw-r--r--   0        0        0     1163 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin
--rw-r--r--   0        0        0     2205 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin
--rw-r--r--   0        0        0     2353 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin
--rw-r--r--   0        0        0     2205 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin
--rw-r--r--   0        0        0     2353 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.1.xml.bin
--rw-r--r--   0        0        0     8462 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin
--rw-r--r--   0        0        0     8225 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin
--rw-r--r--   0        0        0    10188 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin
--rw-r--r--   0        0        0     9538 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin
--rw-r--r--   0        0        0    13095 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin
--rw-r--r--   0        0        0    12485 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin
--rw-r--r--   0        0        0    13095 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin
--rw-r--r--   0        0        0    12485 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin
--rw-r--r--   0        0        0      329 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin
--rw-r--r--   0        0        0     2028 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin
--rw-r--r--   0        0        0     2102 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin
--rw-r--r--   0        0        0     2028 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin
--rw-r--r--   0        0        0     2102 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin
--rw-r--r--   0        0        0     1199 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin
--rw-r--r--   0        0        0     4993 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin
--rw-r--r--   0        0        0     7591 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin
--rw-r--r--   0        0        0     7350 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin
--rw-r--r--   0        0        0     8790 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin
--rw-r--r--   0        0        0     8247 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin
--rw-r--r--   0        0        0    11697 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin
--rw-r--r--   0        0        0    11194 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin
--rw-r--r--   0        0        0    11697 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin
--rw-r--r--   0        0        0    11194 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin
--rw-r--r--   0        0        0      307 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.0.xml.bin
--rw-r--r--   0        0        0      477 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.1.xml.bin
--rw-r--r--   0        0        0      860 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin
--rw-r--r--   0        0        0      859 2024-03-04 12:10:32.543576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin
--rw-r--r--   0        0        0      860 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin
--rw-r--r--   0        0        0      859 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin
--rw-r--r--   0        0        0     1980 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin
--rw-r--r--   0        0        0     2049 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin
--rw-r--r--   0        0        0     1980 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin
--rw-r--r--   0        0        0     2049 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin
--rw-r--r--   0        0        0      395 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.0.xml.bin
--rw-r--r--   0        0        0      572 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin
--rw-r--r--   0        0        0      952 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin
--rw-r--r--   0        0        0      961 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin
--rw-r--r--   0        0        0      952 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin
--rw-r--r--   0        0        0      961 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin
--rw-r--r--   0        0        0     2093 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin
--rw-r--r--   0        0        0     2168 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin
--rw-r--r--   0        0        0     2093 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin
--rw-r--r--   0        0        0     2168 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin
--rw-r--r--   0        0        0      329 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin
--rw-r--r--   0        0        0     3848 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin
--rw-r--r--   0        0        0     3888 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin
--rw-r--r--   0        0        0     3848 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin
--rw-r--r--   0        0        0     3888 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin
--rw-r--r--   0        0        0      329 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin
--rw-r--r--   0        0        0     5145 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin
--rw-r--r--   0        0        0     5654 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin
--rw-r--r--   0        0        0     5145 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin
--rw-r--r--   0        0        0     5654 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin
--rw-r--r--   0        0        0      448 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin
--rw-r--r--   0        0        0     1056 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin
--rw-r--r--   0        0        0     1071 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin
--rw-r--r--   0        0        0     1243 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin
--rw-r--r--   0        0        0     1214 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin
--rw-r--r--   0        0        0     2384 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin
--rw-r--r--   0        0        0     2421 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin
--rw-r--r--   0        0        0     2384 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin
--rw-r--r--   0        0        0     2421 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin
--rw-r--r--   0        0        0      655 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin
--rw-r--r--   0        0        0      980 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin
--rw-r--r--   0        0        0     1582 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin
--rw-r--r--   0        0        0     1579 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin
--rw-r--r--   0        0        0     1769 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin
--rw-r--r--   0        0        0     1722 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin
--rw-r--r--   0        0        0     2889 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin
--rw-r--r--   0        0        0     2912 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin
--rw-r--r--   0        0        0     2889 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin
--rw-r--r--   0        0        0     2912 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin
--rw-r--r--   0        0        0      654 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin
--rw-r--r--   0        0        0     1045 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin
--rw-r--r--   0        0        0     1562 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin
--rw-r--r--   0        0        0     1749 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin
--rw-r--r--   0        0        0     2890 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin
--rw-r--r--   0        0        0     2890 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin
--rw-r--r--   0        0        0     2927 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.0.xml.bin
--rw-r--r--   0        0        0      431 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.1.xml.bin
--rw-r--r--   0        0        0      629 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin
--rw-r--r--   0        0        0      666 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin
--rw-r--r--   0        0        0      792 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin
--rw-r--r--   0        0        0      797 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin
--rw-r--r--   0        0        0     1933 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin
--rw-r--r--   0        0        0     2004 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin
--rw-r--r--   0        0        0     1933 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin
--rw-r--r--   0        0        0     2004 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin
--rw-r--r--   0        0        0      516 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin
--rw-r--r--   0        0        0      814 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     2131 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin
--rw-r--r--   0        0        0     2058 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     2231 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin
--rw-r--r--   0        0        0     2149 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     3288 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin
--rw-r--r--   0        0        0     3288 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     3288 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin
--rw-r--r--   0        0        0     3288 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin
--rw-r--r--   0        0        0      448 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin
--rw-r--r--   0        0        0     1575 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin
--rw-r--r--   0        0        0     1762 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin
--rw-r--r--   0        0        0     2903 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin
--rw-r--r--   0        0        0     2903 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin
--rw-r--r--   0        0        0     2927 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin
--rw-r--r--   0        0        0      245 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.0.xml.bin
--rw-r--r--   0        0        0      459 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     1475 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin
--rw-r--r--   0        0        0     1382 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     1649 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin
--rw-r--r--   0        0        0     1533 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     2748 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin
--rw-r--r--   0        0        0     2706 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     2748 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin
--rw-r--r--   0        0        0     2706 2024-03-04 12:10:32.547576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.1.xml.bin
--rw-r--r--   0        0        0     3772 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin
--rw-r--r--   0        0        0     3875 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin
--rw-r--r--   0        0        0     4135 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin
--rw-r--r--   0        0        0     4149 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin
--rw-r--r--   0        0        0     7096 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin
--rw-r--r--   0        0        0     7142 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin
--rw-r--r--   0        0        0     7096 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin
--rw-r--r--   0        0        0     7142 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.1.xml.bin
--rw-r--r--   0        0        0     2066 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin
--rw-r--r--   0        0        0     2150 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin
--rw-r--r--   0        0        0     2429 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin
--rw-r--r--   0        0        0     2424 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin
--rw-r--r--   0        0        0     5390 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin
--rw-r--r--   0        0        0     5417 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin
--rw-r--r--   0        0        0     5390 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin
--rw-r--r--   0        0        0     5417 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin
--rw-r--r--   0        0        0      108 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.1.xml.bin
--rw-r--r--   0        0        0     1030 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin
--rw-r--r--   0        0        0     1040 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin
--rw-r--r--   0        0        0     1030 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin
--rw-r--r--   0        0        0     1040 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin
--rw-r--r--   0        0        0     2171 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin
--rw-r--r--   0        0        0     2247 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin
--rw-r--r--   0        0        0     2171 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin
--rw-r--r--   0        0        0     2247 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin
--rw-r--r--   0        0        0     2957 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_component.py
--rw-r--r--   0        0        0     3283 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_deserialize_json.py
--rw-r--r--   0        0        0     1764 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_deserialize_xml.py
--rw-r--r--   0        0        0    19038 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_enums.py
--rw-r--r--   0        0        0     4389 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_factory_license.py
--rw-r--r--   0        0        0    22571 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model.py
--rw-r--r--   0        0        0    13219 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model_bom.py
--rw-r--r--   0        0        0     2782 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model_bom_ref.py
--rw-r--r--   0        0        0    18544 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model_component.py
--rw-r--r--   0        0        0     1793 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model_dependency.py
--rw-r--r--   0        0        0     4064 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model_issue.py
--rw-r--r--   0        0        0     4295 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model_license.py
--rw-r--r--   0        0        0     2758 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model_release_note.py
--rw-r--r--   0        0        0     3390 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model_service.py
--rw-r--r--   0        0        0    14370 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_model_vulnerability.py
--rw-r--r--   0        0        0     3154 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_output.py
--rw-r--r--   0        0        0     4335 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_output_json.py
--rw-r--r--   0        0        0     3663 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_output_xml.py
--rw-r--r--   0        0        0     1307 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_real_world_examples.py
--rw-r--r--   0        0        0     2524 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_schema_SchemaVersion.py
--rw-r--r--   0        0        0     1248 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_schema__res.py
--rw-r--r--   0        0        0     2873 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_spdx.py
--rw-r--r--   0        0        0     1977 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_validation.py
--rw-r--r--   0        0        0     4529 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_validation_json.py
--rw-r--r--   0        0        0     3061 2024-03-04 12:10:32.551576 cyclonedx_python_lib-6.4.3/tests/test_validation_xml.py
--rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 cyclonedx_python_lib-6.4.3/PKG-INFO
+-rw-r--r--   0        0        0   216430 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/LICENSE
+-rw-r--r--   0        0        0      147 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/NOTICE
+-rw-r--r--   0        0        0     4569 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/README.md
+-rw-r--r--   0        0        0      850 2024-03-18 18:13:30.950068 cyclonedx_python_lib-6.4.4/cyclonedx/__init__.py
+-rw-r--r--   0        0        0      731 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/_internal/__init__.py
+-rw-r--r--   0        0        0     1734 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/_internal/compare.py
+-rw-r--r--   0        0        0     1164 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/_internal/hash.py
+-rw-r--r--   0        0        0      847 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/_internal/time.py
+-rw-r--r--   0        0        0      993 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/__init__.py
+-rw-r--r--   0        0        0     1536 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/factory.py
+-rw-r--r--   0        0        0     2642 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/model.py
+-rw-r--r--   0        0        0     1136 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/output.py
+-rw-r--r--   0        0        0     1730 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/exception/serialization.py
+-rw-r--r--   0        0        0      680 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/factory/__init__.py
+-rw-r--r--   0        0        0     3233 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/factory/license.py
+-rw-r--r--   0        0        0    48114 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/__init__.py
+-rw-r--r--   0        0        0    23268 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/bom.py
+-rw-r--r--   0        0        0     2179 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/bom_ref.py
+-rw-r--r--   0        0        0    47132 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/component.py
+-rw-r--r--   0        0        0     3766 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/dependency.py
+-rw-r--r--   0        0        0     3568 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/impact_analysis.py
+-rw-r--r--   0        0        0     7024 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/issue.py
+-rw-r--r--   0        0        0     8020 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/license.py
+-rw-r--r--   0        0        0     8623 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/release_note.py
+-rw-r--r--   0        0        0    12676 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/service.py
+-rw-r--r--   0        0        0    43554 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/model/vulnerability.py
+-rw-r--r--   0        0        0     5872 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/output/__init__.py
+-rw-r--r--   0        0        0     4060 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/output/json.py
+-rw-r--r--   0        0        0     4173 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/output/xml.py
+-rw-r--r--   0        0        0      153 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/py.typed
+-rw-r--r--   0        0        0     3000 2024-03-18 18:13:08.146144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/__init__.py
+-rw-r--r--   0        0        0     1961 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/README.md
+-rw-r--r--   0        0        0     2364 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/__init__.py
+-rw-r--r--   0        0        0    13604 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    39716 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    37194 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    36226 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    76383 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    40408 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    39348 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    88794 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    72383 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   133792 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd
+-rw-r--r--   0        0        0   164772 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   311805 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd
+-rw-r--r--   0        0        0     8058 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    12322 2024-03-18 18:13:08.150144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   144335 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd
+-rw-r--r--   0        0        0     2367 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/schema/schema.py
+-rw-r--r--   0        0        0     6479 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/serialization/__init__.py
+-rw-r--r--   0        0        0     2503 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/spdx.py
+-rw-r--r--   0        0        0     3701 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/validation/__init__.py
+-rw-r--r--   0        0        0     4817 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/validation/json.py
+-rw-r--r--   0        0        0      853 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/validation/model.py
+-rw-r--r--   0        0        0     3672 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/cyclonedx/validation/xml.py
+-rw-r--r--   0        0        0      634 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/Makefile
+-rw-r--r--   0        0        0     1524 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/architecture.rst
+-rw-r--r--   0        0        0      686 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/changelog.rst
+-rw-r--r--   0        0        0     2657 2024-03-18 18:13:30.950068 cyclonedx_python_lib-6.4.4/docs/conf.py
+-rw-r--r--   0        0        0       34 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/contributing.rst
+-rw-r--r--   0        0        0      895 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/examples.rst
+-rw-r--r--   0        0        0     1857 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/index.rst
+-rw-r--r--   0        0        0     1499 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/install.rst
+-rw-r--r--   0        0        0      800 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/make.bat
+-rw-r--r--   0        0        0     3275 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/modelling.rst
+-rw-r--r--   0        0        0     2269 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/outputting.rst
+-rw-r--r--   0        0        0       81 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/requirements.txt
+-rw-r--r--   0        0        0     4961 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/schema-support.rst
+-rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/docs/support.rst
+-rw-r--r--   0        0        0      176 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/examples/README.md
+-rw-r--r--   0        0        0     8164 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/examples/complex_deserialize.py
+-rw-r--r--   0        0        0     4046 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/examples/complex_serialize.py
+-rw-r--r--   0        0        0     4226 2024-03-18 18:13:30.950068 cyclonedx_python_lib-6.4.4/pyproject.toml
+-rw-r--r--   0        0        0     5985 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/__init__.py
+-rw-r--r--   0        0        0      704 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/__init__.py
+-rw-r--r--   0        0        0    31717 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/models.py
+-rw-r--r--   0        0        0       16 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/README.md
+-rw-r--r--   0        0        0     1309 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.2/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     1309 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.3/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     1309 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.4/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     2461 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/xml/1.4/bom_setuptools.xml
+-rw-r--r--   0        0        0    98508 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/own/xml/1.4/webgoat-6.1.xml
+-rw-r--r--   0        0        0     3723 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml
+-rw-r--r--   0        0        0     1195 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml
+-rw-r--r--   0        0        0      559 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml
+-rw-r--r--   0        0        0      313 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-component-type-1.1.xml
+-rw-r--r--   0        0        0      246 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-empty-component-1.1.xml
+-rw-r--r--   0        0        0      830 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml
+-rw-r--r--   0        0        0      801 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml
+-rw-r--r--   0        0        0      793 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml
+-rw-r--r--   0        0        0      769 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml
+-rw-r--r--   0        0        0      705 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml
+-rw-r--r--   0        0        0     1303 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml
+-rw-r--r--   0        0        0    16515 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml
+-rw-r--r--   0        0        0    16513 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml
+-rw-r--r--   0        0        0     1328 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml
+-rw-r--r--   0        0        0     1366 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml
+-rw-r--r--   0        0        0      302 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-missing-component-type-1.1.xml
+-rw-r--r--   0        0        0    21038 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml
+-rw-r--r--   0        0        0      348 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-scope-1.1.xml
+-rw-r--r--   0        0        0    21026 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml
+-rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml
+-rw-r--r--   0        0        0     1217 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml
+-rw-r--r--   0        0        0      704 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml
+-rw-r--r--   0        0        0      965 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml
+-rw-r--r--   0        0        0      186 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-empty-components-1.1.xml
+-rw-r--r--   0        0        0    22339 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml
+-rw-r--r--   0        0        0     1210 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml
+-rw-r--r--   0        0        0     1214 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml
+-rw-r--r--   0        0        0     1226 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml
+-rw-r--r--   0        0        0      317 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-minimal-viable-1.1.xml
+-rw-r--r--   0        0        0    21121 2024-03-18 18:13:08.154144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml
+-rw-r--r--   0        0        0    10048 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml
+-rw-r--r--   0        0        0      165 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-bomformat-1.2.json
+-rw-r--r--   0        0        0      394 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.json
+-rw-r--r--   0        0        0      560 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml
+-rw-r--r--   0        0        0      385 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.json
+-rw-r--r--   0        0        0      433 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.xml
+-rw-r--r--   0        0        0      249 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.json
+-rw-r--r--   0        0        0      314 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.xml
+-rw-r--r--   0        0        0      667 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json
+-rw-r--r--   0        0        0      809 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml
+-rw-r--r--   0        0        0      247 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-empty-component-1.2.xml
+-rw-r--r--   0        0        0      856 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json
+-rw-r--r--   0        0        0      831 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml
+-rw-r--r--   0        0        0      827 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json
+-rw-r--r--   0        0        0      802 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml
+-rw-r--r--   0        0        0      819 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json
+-rw-r--r--   0        0        0      794 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml
+-rw-r--r--   0        0        0      795 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json
+-rw-r--r--   0        0        0      770 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml
+-rw-r--r--   0        0        0      731 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json
+-rw-r--r--   0        0        0      706 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml
+-rw-r--r--   0        0        0     1184 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json
+-rw-r--r--   0        0        0     1554 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml
+-rw-r--r--   0        0        0      515 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json
+-rw-r--r--   0        0        0     1304 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml
+-rw-r--r--   0        0        0    15788 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json
+-rw-r--r--   0        0        0    16516 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml
+-rw-r--r--   0        0        0      428 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.json
+-rw-r--r--   0        0        0    16514 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml
+-rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml
+-rw-r--r--   0        0        0     1367 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml
+-rw-r--r--   0        0        0      209 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.json
+-rw-r--r--   0        0        0      244 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.xml
+-rw-r--r--   0        0        0      303 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-missing-component-type-1.2.xml
+-rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml
+-rw-r--r--   0        0        0     1185 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json
+-rw-r--r--   0        0        0     1555 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml
+-rw-r--r--   0        0        0      275 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-scope-1.2.json
+-rw-r--r--   0        0        0      349 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-scope-1.2.xml
+-rw-r--r--   0        0        0      148 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.json
+-rw-r--r--   0        0        0    21027 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.json
+-rw-r--r--   0        0        0      416 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.xml
+-rw-r--r--   0        0        0      363 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/skip_invalid-empty-component-1.2.json
+-rw-r--r--   0        0        0      361 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/skip_invalid-missing-component-type-1.2.json
+-rw-r--r--   0        0        0      548 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json
+-rw-r--r--   0        0        0      792 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml
+-rw-r--r--   0        0        0    20390 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.json
+-rw-r--r--   0        0        0    24278 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml
+-rw-r--r--   0        0        0     2163 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json
+-rw-r--r--   0        0        0     1897 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml
+-rw-r--r--   0        0        0      394 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.json
+-rw-r--r--   0        0        0      705 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml
+-rw-r--r--   0        0        0      456 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.json
+-rw-r--r--   0        0        0      492 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.xml
+-rw-r--r--   0        0        0     1342 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json
+-rw-r--r--   0        0        0     1346 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml
+-rw-r--r--   0        0        0      892 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json
+-rw-r--r--   0        0        0     1223 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml
+-rw-r--r--   0        0        0      693 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json
+-rw-r--r--   0        0        0      824 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml
+-rw-r--r--   0        0        0      161 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.json
+-rw-r--r--   0        0        0      187 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.xml
+-rw-r--r--   0        0        0    22340 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml
+-rw-r--r--   0        0        0      438 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.json
+-rw-r--r--   0        0        0     1211 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-id-1.2.json
+-rw-r--r--   0        0        0     1215 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml
+-rw-r--r--   0        0        0      440 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-name-1.2.json
+-rw-r--r--   0        0        0     1227 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml
+-rw-r--r--   0        0        0      333 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.json
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.xml
+-rw-r--r--   0        0        0      438 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.json
+-rw-r--r--   0        0        0      492 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.xml
+-rw-r--r--   0        0        0      417 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.json
+-rw-r--r--   0        0        0      468 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.xml
+-rw-r--r--   0        0        0      224 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.json
+-rw-r--r--   0        0        0      254 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.xml
+-rw-r--r--   0        0        0      605 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json
+-rw-r--r--   0        0        0      654 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml
+-rw-r--r--   0        0        0      253 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.json
+-rw-r--r--   0        0        0      318 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.xml
+-rw-r--r--   0        0        0     2465 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.json
+-rw-r--r--   0        0        0     3337 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml
+-rw-r--r--   0        0        0    21122 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml
+-rw-r--r--   0        0        0     2308 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-1.2.json
+-rw-r--r--   0        0        0     2693 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-1.2.xml
+-rw-r--r--   0        0        0      419 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.json
+-rw-r--r--   0        0        0      495 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.xml
+-rw-r--r--   0        0        0    11181 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml
+-rw-r--r--   0        0        0      165 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-bomformat-1.3.json
+-rw-r--r--   0        0        0      394 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.json
+-rw-r--r--   0        0        0      560 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml
+-rw-r--r--   0        0        0      385 2024-03-18 18:13:08.158144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.json
+-rw-r--r--   0        0        0      433 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.xml
+-rw-r--r--   0        0        0      249 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.json
+-rw-r--r--   0        0        0      314 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.xml
+-rw-r--r--   0        0        0      667 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json
+-rw-r--r--   0        0        0      809 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml
+-rw-r--r--   0        0        0      197 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.json
+-rw-r--r--   0        0        0      247 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.xml
+-rw-r--r--   0        0        0      856 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json
+-rw-r--r--   0        0        0      831 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml
+-rw-r--r--   0        0        0      827 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json
+-rw-r--r--   0        0        0      802 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml
+-rw-r--r--   0        0        0      819 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json
+-rw-r--r--   0        0        0      794 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml
+-rw-r--r--   0        0        0      795 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json
+-rw-r--r--   0        0        0      770 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml
+-rw-r--r--   0        0        0      731 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json
+-rw-r--r--   0        0        0      706 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml
+-rw-r--r--   0        0        0     1184 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json
+-rw-r--r--   0        0        0     1554 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml
+-rw-r--r--   0        0        0      515 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json
+-rw-r--r--   0        0        0     1304 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml
+-rw-r--r--   0        0        0    15788 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json
+-rw-r--r--   0        0        0    16516 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml
+-rw-r--r--   0        0        0      428 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.json
+-rw-r--r--   0        0        0    16514 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml
+-rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml
+-rw-r--r--   0        0        0     1367 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml
+-rw-r--r--   0        0        0      277 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.json
+-rw-r--r--   0        0        0      319 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.xml
+-rw-r--r--   0        0        0      209 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.json
+-rw-r--r--   0        0        0      244 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.xml
+-rw-r--r--   0        0        0      228 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.json
+-rw-r--r--   0        0        0      303 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.xml
+-rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml
+-rw-r--r--   0        0        0     1185 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json
+-rw-r--r--   0        0        0     1555 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml
+-rw-r--r--   0        0        0      275 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-scope-1.3.json
+-rw-r--r--   0        0        0      349 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-scope-1.3.xml
+-rw-r--r--   0        0        0      148 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.json
+-rw-r--r--   0        0        0    21027 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.json
+-rw-r--r--   0        0        0      416 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.xml
+-rw-r--r--   0        0        0      548 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json
+-rw-r--r--   0        0        0      792 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml
+-rw-r--r--   0        0        0    20390 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.json
+-rw-r--r--   0        0        0    24278 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml
+-rw-r--r--   0        0        0     2163 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json
+-rw-r--r--   0        0        0     1897 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml
+-rw-r--r--   0        0        0      394 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.json
+-rw-r--r--   0        0        0      705 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml
+-rw-r--r--   0        0        0      456 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.json
+-rw-r--r--   0        0        0      492 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.xml
+-rw-r--r--   0        0        0     1342 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json
+-rw-r--r--   0        0        0     1346 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml
+-rw-r--r--   0        0        0      892 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json
+-rw-r--r--   0        0        0     1223 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml
+-rw-r--r--   0        0        0     1497 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json
+-rw-r--r--   0        0        0     1983 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml
+-rw-r--r--   0        0        0      693 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json
+-rw-r--r--   0        0        0      824 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml
+-rw-r--r--   0        0        0      161 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.json
+-rw-r--r--   0        0        0      187 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.xml
+-rw-r--r--   0        0        0     1384 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json
+-rw-r--r--   0        0        0     1596 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml
+-rw-r--r--   0        0        0    22340 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml
+-rw-r--r--   0        0        0     1117 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json
+-rw-r--r--   0        0        0     1324 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml
+-rw-r--r--   0        0        0      438 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.json
+-rw-r--r--   0        0        0     1211 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-id-1.3.json
+-rw-r--r--   0        0        0     1215 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml
+-rw-r--r--   0        0        0      440 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-name-1.3.json
+-rw-r--r--   0        0        0     1227 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml
+-rw-r--r--   0        0        0      333 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.json
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.xml
+-rw-r--r--   0        0        0      279 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.json
+-rw-r--r--   0        0        0      321 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.xml
+-rw-r--r--   0        0        0      438 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.json
+-rw-r--r--   0        0        0      492 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.xml
+-rw-r--r--   0        0        0      417 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.json
+-rw-r--r--   0        0        0      468 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.xml
+-rw-r--r--   0        0        0      224 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.json
+-rw-r--r--   0        0        0      254 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.xml
+-rw-r--r--   0        0        0      605 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json
+-rw-r--r--   0        0        0      654 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml
+-rw-r--r--   0        0        0      253 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.json
+-rw-r--r--   0        0        0      318 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.xml
+-rw-r--r--   0        0        0     2465 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.json
+-rw-r--r--   0        0        0     3337 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml
+-rw-r--r--   0        0        0      983 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.json
+-rw-r--r--   0        0        0     1213 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml
+-rw-r--r--   0        0        0    21122 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml
+-rw-r--r--   0        0        0     2308 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-1.3.json
+-rw-r--r--   0        0        0     2693 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-1.3.xml
+-rw-r--r--   0        0        0      419 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.json
+-rw-r--r--   0        0        0      495 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.xml
+-rw-r--r--   0        0        0    11181 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml
+-rw-r--r--   0        0        0      165 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-bomformat-1.4.json
+-rw-r--r--   0        0        0      394 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.json
+-rw-r--r--   0        0        0      560 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml
+-rw-r--r--   0        0        0      385 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.json
+-rw-r--r--   0        0        0      433 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.xml
+-rw-r--r--   0        0        0      249 2024-03-18 18:13:08.162144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.json
+-rw-r--r--   0        0        0      314 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.xml
+-rw-r--r--   0        0        0      667 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json
+-rw-r--r--   0        0        0      809 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml
+-rw-r--r--   0        0        0      197 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.json
+-rw-r--r--   0        0        0      247 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.xml
+-rw-r--r--   0        0        0      856 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json
+-rw-r--r--   0        0        0      831 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml
+-rw-r--r--   0        0        0      827 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json
+-rw-r--r--   0        0        0      802 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml
+-rw-r--r--   0        0        0      819 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json
+-rw-r--r--   0        0        0      794 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml
+-rw-r--r--   0        0        0      795 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json
+-rw-r--r--   0        0        0      770 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml
+-rw-r--r--   0        0        0      731 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json
+-rw-r--r--   0        0        0      706 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml
+-rw-r--r--   0        0        0     1184 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json
+-rw-r--r--   0        0        0     1554 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml
+-rw-r--r--   0        0        0      515 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json
+-rw-r--r--   0        0        0     1304 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml
+-rw-r--r--   0        0        0    15788 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json
+-rw-r--r--   0        0        0    16516 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml
+-rw-r--r--   0        0        0      428 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.json
+-rw-r--r--   0        0        0    16514 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml
+-rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml
+-rw-r--r--   0        0        0     1367 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml
+-rw-r--r--   0        0        0      277 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.json
+-rw-r--r--   0        0        0      319 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.xml
+-rw-r--r--   0        0        0      209 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.json
+-rw-r--r--   0        0        0      244 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.xml
+-rw-r--r--   0        0        0      228 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.json
+-rw-r--r--   0        0        0      303 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.xml
+-rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml
+-rw-r--r--   0        0        0     1185 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json
+-rw-r--r--   0        0        0     1555 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml
+-rw-r--r--   0        0        0      275 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-scope-1.4.json
+-rw-r--r--   0        0        0      349 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-scope-1.4.xml
+-rw-r--r--   0        0        0      148 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.json
+-rw-r--r--   0        0        0    21027 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.json
+-rw-r--r--   0        0        0      416 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.xml
+-rw-r--r--   0        0        0      548 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json
+-rw-r--r--   0        0        0      792 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml
+-rw-r--r--   0        0        0    20390 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.json
+-rw-r--r--   0        0        0    24278 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml
+-rw-r--r--   0        0        0     2163 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json
+-rw-r--r--   0        0        0     1897 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml
+-rw-r--r--   0        0        0      394 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.json
+-rw-r--r--   0        0        0      705 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml
+-rw-r--r--   0        0        0      456 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.json
+-rw-r--r--   0        0        0      492 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.xml
+-rw-r--r--   0        0        0     1342 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json
+-rw-r--r--   0        0        0     1346 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml
+-rw-r--r--   0        0        0      892 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json
+-rw-r--r--   0        0        0     1223 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml
+-rw-r--r--   0        0        0     1497 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json
+-rw-r--r--   0        0        0     1983 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml
+-rw-r--r--   0        0        0      693 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json
+-rw-r--r--   0        0        0      824 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml
+-rw-r--r--   0        0        0      161 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.json
+-rw-r--r--   0        0        0      187 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.xml
+-rw-r--r--   0        0        0     1384 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json
+-rw-r--r--   0        0        0     1596 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml
+-rw-r--r--   0        0        0    22340 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml
+-rw-r--r--   0        0        0     1117 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json
+-rw-r--r--   0        0        0     1324 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml
+-rw-r--r--   0        0        0      438 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.json
+-rw-r--r--   0        0        0     1211 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-id-1.4.json
+-rw-r--r--   0        0        0     1215 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml
+-rw-r--r--   0        0        0      440 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-name-1.4.json
+-rw-r--r--   0        0        0     1227 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml
+-rw-r--r--   0        0        0      333 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.json
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.xml
+-rw-r--r--   0        0        0      279 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.json
+-rw-r--r--   0        0        0      321 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.xml
+-rw-r--r--   0        0        0      438 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.json
+-rw-r--r--   0        0        0      492 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.xml
+-rw-r--r--   0        0        0      417 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.json
+-rw-r--r--   0        0        0      468 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.xml
+-rw-r--r--   0        0        0      224 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.json
+-rw-r--r--   0        0        0      254 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.xml
+-rw-r--r--   0        0        0      605 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json
+-rw-r--r--   0        0        0      654 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml
+-rw-r--r--   0        0        0      227 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.json
+-rw-r--r--   0        0        0      281 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.xml
+-rw-r--r--   0        0        0     2465 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.json
+-rw-r--r--   0        0        0     3337 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml
+-rw-r--r--   0        0        0      983 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.json
+-rw-r--r--   0        0        0     1213 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml
+-rw-r--r--   0        0        0    21122 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml
+-rw-r--r--   0        0        0     5338 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json
+-rw-r--r--   0        0        0     6828 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml
+-rw-r--r--   0        0        0     2312 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-1.4.json
+-rw-r--r--   0        0        0     2693 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-1.4.xml
+-rw-r--r--   0        0        0      419 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.json
+-rw-r--r--   0        0        0      495 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.xml
+-rw-r--r--   0        0        0     9733 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json
+-rw-r--r--   0        0        0     4274 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json
+-rw-r--r--   0        0        0     5987 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml
+-rw-r--r--   0        0        0    11181 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml
+-rw-r--r--   0        0        0      165 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-bomformat-1.5.json
+-rw-r--r--   0        0        0      508 2024-03-18 18:13:08.166144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.json
+-rw-r--r--   0        0        0      866 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml
+-rw-r--r--   0        0        0      385 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.json
+-rw-r--r--   0        0        0      433 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.xml
+-rw-r--r--   0        0        0      249 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.json
+-rw-r--r--   0        0        0      314 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.xml
+-rw-r--r--   0        0        0      746 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json
+-rw-r--r--   0        0        0     1086 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml
+-rw-r--r--   0        0        0      197 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.json
+-rw-r--r--   0        0        0      247 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.xml
+-rw-r--r--   0        0        0      856 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json
+-rw-r--r--   0        0        0      831 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml
+-rw-r--r--   0        0        0      827 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json
+-rw-r--r--   0        0        0      802 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml
+-rw-r--r--   0        0        0      819 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json
+-rw-r--r--   0        0        0      794 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml
+-rw-r--r--   0        0        0      795 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json
+-rw-r--r--   0        0        0      770 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml
+-rw-r--r--   0        0        0      731 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json
+-rw-r--r--   0        0        0      706 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml
+-rw-r--r--   0        0        0     1184 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json
+-rw-r--r--   0        0        0     1554 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml
+-rw-r--r--   0        0        0      515 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json
+-rw-r--r--   0        0        0     1304 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml
+-rw-r--r--   0        0        0    15788 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json
+-rw-r--r--   0        0        0    16516 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml
+-rw-r--r--   0        0        0      428 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.json
+-rw-r--r--   0        0        0    16514 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml
+-rw-r--r--   0        0        0     1329 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml
+-rw-r--r--   0        0        0     1367 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml
+-rw-r--r--   0        0        0      277 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.json
+-rw-r--r--   0        0        0      319 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.xml
+-rw-r--r--   0        0        0      209 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.json
+-rw-r--r--   0        0        0      244 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.xml
+-rw-r--r--   0        0        0      228 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.json
+-rw-r--r--   0        0        0      303 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.xml
+-rw-r--r--   0        0        0    21039 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml
+-rw-r--r--   0        0        0     1185 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json
+-rw-r--r--   0        0        0     1555 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml
+-rw-r--r--   0        0        0      275 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-scope-1.5.json
+-rw-r--r--   0        0        0      349 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-scope-1.5.xml
+-rw-r--r--   0        0        0      148 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.json
+-rw-r--r--   0        0        0    21027 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.json
+-rw-r--r--   0        0        0      416 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.xml
+-rw-r--r--   0        0        0     2527 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json
+-rw-r--r--   0        0        0     3596 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml
+-rw-r--r--   0        0        0      548 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json
+-rw-r--r--   0        0        0      792 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml
+-rw-r--r--   0        0        0    20390 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.json
+-rw-r--r--   0        0        0    24278 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml
+-rw-r--r--   0        0        0     2163 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json
+-rw-r--r--   0        0        0     1897 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml
+-rw-r--r--   0        0        0      394 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.json
+-rw-r--r--   0        0        0      705 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml
+-rw-r--r--   0        0        0      456 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.json
+-rw-r--r--   0        0        0      492 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.xml
+-rw-r--r--   0        0        0     1342 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json
+-rw-r--r--   0        0        0     1346 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml
+-rw-r--r--   0        0        0      892 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json
+-rw-r--r--   0        0        0     1223 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml
+-rw-r--r--   0        0        0     1810 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json
+-rw-r--r--   0        0        0     2449 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml
+-rw-r--r--   0        0        0      693 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json
+-rw-r--r--   0        0        0      824 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml
+-rw-r--r--   0        0        0      161 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.json
+-rw-r--r--   0        0        0      187 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.xml
+-rw-r--r--   0        0        0     3189 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json
+-rw-r--r--   0        0        0     4519 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml
+-rw-r--r--   0        0        0    22340 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml
+-rw-r--r--   0        0        0     1117 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json
+-rw-r--r--   0        0        0     1324 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml
+-rw-r--r--   0        0        0     7703 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json
+-rw-r--r--   0        0        0    11757 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml
+-rw-r--r--   0        0        0      473 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.json
+-rw-r--r--   0        0        0     1270 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml
+-rw-r--r--   0        0        0      467 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-id-1.5.json
+-rw-r--r--   0        0        0     1236 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml
+-rw-r--r--   0        0        0     1539 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json
+-rw-r--r--   0        0        0     2197 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml
+-rw-r--r--   0        0        0      477 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-name-1.5.json
+-rw-r--r--   0        0        0     1248 2024-03-18 18:13:08.170144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml
+-rw-r--r--   0        0        0    98548 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json
+-rw-r--r--   0        0        0   100112 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml
+-rw-r--r--   0        0        0      333 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.json
+-rw-r--r--   0        0        0      430 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.xml
+-rw-r--r--   0        0        0      279 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.json
+-rw-r--r--   0        0        0      321 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.xml
+-rw-r--r--   0        0        0      436 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.json
+-rw-r--r--   0        0        0      624 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml
+-rw-r--r--   0        0        0      507 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.json
+-rw-r--r--   0        0        0      537 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml
+-rw-r--r--   0        0        0      482 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.json
+-rw-r--r--   0        0        0      509 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.xml
+-rw-r--r--   0        0        0      224 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.json
+-rw-r--r--   0        0        0      254 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.xml
+-rw-r--r--   0        0        0     1162 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json
+-rw-r--r--   0        0        0     1471 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml
+-rw-r--r--   0        0        0      605 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json
+-rw-r--r--   0        0        0      654 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml
+-rw-r--r--   0        0        0      227 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.json
+-rw-r--r--   0        0        0      281 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.xml
+-rw-r--r--   0        0        0     2465 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.json
+-rw-r--r--   0        0        0     3337 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml
+-rw-r--r--   0        0        0     1520 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.json
+-rw-r--r--   0        0        0     1660 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml
+-rw-r--r--   0        0        0    21122 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml
+-rw-r--r--   0        0        0     5338 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json
+-rw-r--r--   0        0        0     6828 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml
+-rw-r--r--   0        0        0     9412 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json
+-rw-r--r--   0        0        0    12249 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml
+-rw-r--r--   0        0        0     2312 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-1.5.json
+-rw-r--r--   0        0        0     2693 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-1.5.xml
+-rw-r--r--   0        0        0      419 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.json
+-rw-r--r--   0        0        0      495 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.xml
+-rw-r--r--   0        0        0     9733 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json
+-rw-r--r--   0        0        0    17746 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json
+-rw-r--r--   0        0        0    19794 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml
+-rw-r--r--   0        0        0    11181 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml
+-rw-r--r--   0        0        0      157 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/README.md
+-rwxr-xr-x   0        0        0      739 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/fetch.sh
+-rw-r--r--   0        0        0      391 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/README.md
+-rw-r--r--   0        0        0      579 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin
+-rw-r--r--   0        0        0      649 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin
+-rw-r--r--   0        0        0     1050 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin
+-rw-r--r--   0        0        0     1055 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin
+-rw-r--r--   0        0        0     1050 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin
+-rw-r--r--   0        0        0     1055 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin
+-rw-r--r--   0        0        0     2128 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin
+-rw-r--r--   0        0        0     2211 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin
+-rw-r--r--   0        0        0     2128 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin
+-rw-r--r--   0        0        0     2211 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin
+-rw-r--r--   0        0        0      806 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin
+-rw-r--r--   0        0        0      949 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin
+-rw-r--r--   0        0        0     1835 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.2.json.bin
+-rw-r--r--   0        0        0     1806 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin
+-rw-r--r--   0        0        0     1835 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.3.json.bin
+-rw-r--r--   0        0        0     1806 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin
+-rw-r--r--   0        0        0     2808 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.4.json.bin
+-rw-r--r--   0        0        0     2877 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin
+-rw-r--r--   0        0        0     3460 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.5.json.bin
+-rw-r--r--   0        0        0     3525 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.1.xml.bin
+-rw-r--r--   0        0        0      944 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.2.json.bin
+-rw-r--r--   0        0        0      865 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin
+-rw-r--r--   0        0        0      944 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.3.json.bin
+-rw-r--r--   0        0        0      865 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin
+-rw-r--r--   0        0        0     2085 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.4.json.bin
+-rw-r--r--   0        0        0     2072 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin
+-rw-r--r--   0        0        0     2085 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.5.json.bin
+-rw-r--r--   0        0        0     2072 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin
+-rw-r--r--   0        0        0      246 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.0.xml.bin
+-rw-r--r--   0        0        0      496 2024-03-18 18:13:08.174144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.1.xml.bin
+-rw-r--r--   0        0        0      893 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.2.json.bin
+-rw-r--r--   0        0        0      812 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.2.xml.bin
+-rw-r--r--   0        0        0      893 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.3.json.bin
+-rw-r--r--   0        0        0      812 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.3.xml.bin
+-rw-r--r--   0        0        0     2013 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.4.json.bin
+-rw-r--r--   0        0        0     2002 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.4.xml.bin
+-rw-r--r--   0        0        0     2013 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.5.json.bin
+-rw-r--r--   0        0        0     2002 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.5.xml.bin
+-rw-r--r--   0        0        0      246 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.0.xml.bin
+-rw-r--r--   0        0        0     4093 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin
+-rw-r--r--   0        0        0     4074 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin
+-rw-r--r--   0        0        0     4409 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin
+-rw-r--r--   0        0        0     4074 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin
+-rw-r--r--   0        0        0     4409 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin
+-rw-r--r--   0        0        0     5202 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin
+-rw-r--r--   0        0        0     5607 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin
+-rw-r--r--   0        0        0     5451 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin
+-rw-r--r--   0        0        0     5856 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin
+-rw-r--r--   0        0        0      749 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin
+-rw-r--r--   0        0        0      793 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin
+-rw-r--r--   0        0        0     1894 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin
+-rw-r--r--   0        0        0     1461 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin
+-rw-r--r--   0        0        0     1894 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin
+-rw-r--r--   0        0        0     1461 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin
+-rw-r--r--   0        0        0     3014 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin
+-rw-r--r--   0        0        0     2651 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin
+-rw-r--r--   0        0        0     3014 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin
+-rw-r--r--   0        0        0     2651 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.xml.bin
+-rw-r--r--   0        0        0     2092 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin
+-rw-r--r--   0        0        0     2289 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin
+-rw-r--r--   0        0        0     2092 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin
+-rw-r--r--   0        0        0     2289 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.xml.bin
+-rw-r--r--   0        0        0     3282 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin
+-rw-r--r--   0        0        0     3686 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin
+-rw-r--r--   0        0        0     3282 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin
+-rw-r--r--   0        0        0     3686 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.xml.bin
+-rw-r--r--   0        0        0     1827 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin
+-rw-r--r--   0        0        0     2023 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin
+-rw-r--r--   0        0        0     1827 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin
+-rw-r--r--   0        0        0     2023 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.xml.bin
+-rw-r--r--   0        0        0     2577 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin
+-rw-r--r--   0        0        0     2822 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin
+-rw-r--r--   0        0        0     2577 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin
+-rw-r--r--   0        0        0     2822 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin
+-rw-r--r--   0        0        0      246 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.0.xml.bin
+-rw-r--r--   0        0        0      308 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.1.xml.bin
+-rw-r--r--   0        0        0     1081 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin
+-rw-r--r--   0        0        0     1083 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin
+-rw-r--r--   0        0        0     1081 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin
+-rw-r--r--   0        0        0     1083 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin
+-rw-r--r--   0        0        0     2201 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin
+-rw-r--r--   0        0        0     2273 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin
+-rw-r--r--   0        0        0     2201 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin
+-rw-r--r--   0        0        0     2273 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin
+-rw-r--r--   0        0        0      246 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.0.xml.bin
+-rw-r--r--   0        0        0      308 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.1.xml.bin
+-rw-r--r--   0        0        0      886 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin
+-rw-r--r--   0        0        0      821 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin
+-rw-r--r--   0        0        0      886 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin
+-rw-r--r--   0        0        0      821 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin
+-rw-r--r--   0        0        0     2006 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin
+-rw-r--r--   0        0        0     2011 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin
+-rw-r--r--   0        0        0     2006 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin
+-rw-r--r--   0        0        0     2011 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.xml.bin
+-rw-r--r--   0        0        0     2014 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin
+-rw-r--r--   0        0        0     2243 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin
+-rw-r--r--   0        0        0     2014 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin
+-rw-r--r--   0        0        0     2243 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.xml.bin
+-rw-r--r--   0        0        0     2025 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin
+-rw-r--r--   0        0        0     2268 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin
+-rw-r--r--   0        0        0     2025 2024-03-18 18:13:08.178144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin
+-rw-r--r--   0        0        0     2268 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin
+-rw-r--r--   0        0        0      596 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin
+-rw-r--r--   0        0        0      695 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin
+-rw-r--r--   0        0        0     1561 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin
+-rw-r--r--   0        0        0     1597 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin
+-rw-r--r--   0        0        0     1561 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin
+-rw-r--r--   0        0        0     1597 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin
+-rw-r--r--   0        0        0     2702 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin
+-rw-r--r--   0        0        0     2804 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin
+-rw-r--r--   0        0        0     2702 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin
+-rw-r--r--   0        0        0     2804 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin
+-rw-r--r--   0        0        0      662 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin
+-rw-r--r--   0        0        0      678 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin
+-rw-r--r--   0        0        0     1385 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin
+-rw-r--r--   0        0        0     1402 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin
+-rw-r--r--   0        0        0     1385 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin
+-rw-r--r--   0        0        0     1402 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin
+-rw-r--r--   0        0        0     2526 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin
+-rw-r--r--   0        0        0     2609 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin
+-rw-r--r--   0        0        0     2526 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin
+-rw-r--r--   0        0        0     2609 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin
+-rw-r--r--   0        0        0      246 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.0.xml.bin
+-rw-r--r--   0        0        0      847 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin
+-rw-r--r--   0        0        0     1085 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin
+-rw-r--r--   0        0        0     1163 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin
+-rw-r--r--   0        0        0     1085 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin
+-rw-r--r--   0        0        0     1163 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin
+-rw-r--r--   0        0        0     2205 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin
+-rw-r--r--   0        0        0     2353 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin
+-rw-r--r--   0        0        0     2205 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin
+-rw-r--r--   0        0        0     2353 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.1.xml.bin
+-rw-r--r--   0        0        0     8462 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin
+-rw-r--r--   0        0        0     8225 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin
+-rw-r--r--   0        0        0    10188 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin
+-rw-r--r--   0        0        0     9538 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin
+-rw-r--r--   0        0        0    13095 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin
+-rw-r--r--   0        0        0    12485 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin
+-rw-r--r--   0        0        0    13095 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin
+-rw-r--r--   0        0        0    12485 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin
+-rw-r--r--   0        0        0      329 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin
+-rw-r--r--   0        0        0     2028 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin
+-rw-r--r--   0        0        0     2102 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin
+-rw-r--r--   0        0        0     2028 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin
+-rw-r--r--   0        0        0     2102 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin
+-rw-r--r--   0        0        0     1199 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin
+-rw-r--r--   0        0        0     4993 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin
+-rw-r--r--   0        0        0     7591 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin
+-rw-r--r--   0        0        0     7350 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin
+-rw-r--r--   0        0        0     8790 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin
+-rw-r--r--   0        0        0     8247 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin
+-rw-r--r--   0        0        0    11697 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin
+-rw-r--r--   0        0        0    11194 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin
+-rw-r--r--   0        0        0    11697 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin
+-rw-r--r--   0        0        0    11194 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin
+-rw-r--r--   0        0        0      307 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.0.xml.bin
+-rw-r--r--   0        0        0      477 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.1.xml.bin
+-rw-r--r--   0        0        0      860 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin
+-rw-r--r--   0        0        0      859 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin
+-rw-r--r--   0        0        0      860 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin
+-rw-r--r--   0        0        0      859 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin
+-rw-r--r--   0        0        0     1980 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin
+-rw-r--r--   0        0        0     2049 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin
+-rw-r--r--   0        0        0     1980 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin
+-rw-r--r--   0        0        0     2049 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin
+-rw-r--r--   0        0        0      395 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.0.xml.bin
+-rw-r--r--   0        0        0      572 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin
+-rw-r--r--   0        0        0      952 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin
+-rw-r--r--   0        0        0      961 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin
+-rw-r--r--   0        0        0      952 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin
+-rw-r--r--   0        0        0      961 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin
+-rw-r--r--   0        0        0     2093 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin
+-rw-r--r--   0        0        0     2168 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin
+-rw-r--r--   0        0        0     2093 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin
+-rw-r--r--   0        0        0     2168 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin
+-rw-r--r--   0        0        0      329 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin
+-rw-r--r--   0        0        0     3848 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin
+-rw-r--r--   0        0        0     3888 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin
+-rw-r--r--   0        0        0     3848 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin
+-rw-r--r--   0        0        0     3888 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin
+-rw-r--r--   0        0        0      329 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin
+-rw-r--r--   0        0        0     5145 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin
+-rw-r--r--   0        0        0     5654 2024-03-18 18:13:08.182144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin
+-rw-r--r--   0        0        0     5145 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin
+-rw-r--r--   0        0        0     5654 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin
+-rw-r--r--   0        0        0      448 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.0.xml.bin
+-rw-r--r--   0        0        0      723 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin
+-rw-r--r--   0        0        0     1056 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin
+-rw-r--r--   0        0        0     1071 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin
+-rw-r--r--   0        0        0     1243 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin
+-rw-r--r--   0        0        0     1214 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin
+-rw-r--r--   0        0        0     2384 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin
+-rw-r--r--   0        0        0     2421 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin
+-rw-r--r--   0        0        0     2384 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin
+-rw-r--r--   0        0        0     2421 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin
+-rw-r--r--   0        0        0      655 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin
+-rw-r--r--   0        0        0      980 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin
+-rw-r--r--   0        0        0     1582 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin
+-rw-r--r--   0        0        0     1579 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin
+-rw-r--r--   0        0        0     1769 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin
+-rw-r--r--   0        0        0     1722 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin
+-rw-r--r--   0        0        0     2889 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin
+-rw-r--r--   0        0        0     2912 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin
+-rw-r--r--   0        0        0     2889 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin
+-rw-r--r--   0        0        0     2912 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin
+-rw-r--r--   0        0        0      654 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin
+-rw-r--r--   0        0        0     1045 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin
+-rw-r--r--   0        0        0     1562 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin
+-rw-r--r--   0        0        0     1577 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin
+-rw-r--r--   0        0        0     1749 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin
+-rw-r--r--   0        0        0     1720 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin
+-rw-r--r--   0        0        0     2890 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin
+-rw-r--r--   0        0        0     2927 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin
+-rw-r--r--   0        0        0     2890 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin
+-rw-r--r--   0        0        0     2927 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.0.xml.bin
+-rw-r--r--   0        0        0      431 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.1.xml.bin
+-rw-r--r--   0        0        0      629 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin
+-rw-r--r--   0        0        0      666 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin
+-rw-r--r--   0        0        0      792 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin
+-rw-r--r--   0        0        0      797 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin
+-rw-r--r--   0        0        0     1933 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin
+-rw-r--r--   0        0        0     2004 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin
+-rw-r--r--   0        0        0     1933 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin
+-rw-r--r--   0        0        0     2004 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin
+-rw-r--r--   0        0        0      516 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin
+-rw-r--r--   0        0        0      814 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin
+-rw-r--r--   0        0        0     2131 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin
+-rw-r--r--   0        0        0     2058 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin
+-rw-r--r--   0        0        0     2231 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin
+-rw-r--r--   0        0        0     2149 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin
+-rw-r--r--   0        0        0     3288 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin
+-rw-r--r--   0        0        0     3288 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin
+-rw-r--r--   0        0        0     3288 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin
+-rw-r--r--   0        0        0     3288 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin
+-rw-r--r--   0        0        0      448 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.0.xml.bin
+-rw-r--r--   0        0        0      723 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin
+-rw-r--r--   0        0        0     1575 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin
+-rw-r--r--   0        0        0     1577 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin
+-rw-r--r--   0        0        0     1762 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin
+-rw-r--r--   0        0        0     1720 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin
+-rw-r--r--   0        0        0     2903 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin
+-rw-r--r--   0        0        0     2927 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin
+-rw-r--r--   0        0        0     2903 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin
+-rw-r--r--   0        0        0     2927 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin
+-rw-r--r--   0        0        0      245 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.0.xml.bin
+-rw-r--r--   0        0        0      459 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.1.xml.bin
+-rw-r--r--   0        0        0     1475 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin
+-rw-r--r--   0        0        0     1382 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin
+-rw-r--r--   0        0        0     1649 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin
+-rw-r--r--   0        0        0     1533 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin
+-rw-r--r--   0        0        0     2748 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin
+-rw-r--r--   0        0        0     2706 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin
+-rw-r--r--   0        0        0     2748 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin
+-rw-r--r--   0        0        0     2706 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.1.xml.bin
+-rw-r--r--   0        0        0     3772 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin
+-rw-r--r--   0        0        0     3875 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin
+-rw-r--r--   0        0        0     4135 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin
+-rw-r--r--   0        0        0     4149 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin
+-rw-r--r--   0        0        0     7096 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin
+-rw-r--r--   0        0        0     7142 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin
+-rw-r--r--   0        0        0     7096 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin
+-rw-r--r--   0        0        0     7142 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.1.xml.bin
+-rw-r--r--   0        0        0     2066 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin
+-rw-r--r--   0        0        0     2150 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin
+-rw-r--r--   0        0        0     2429 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin
+-rw-r--r--   0        0        0     2424 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin
+-rw-r--r--   0        0        0     5390 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin
+-rw-r--r--   0        0        0     5417 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin
+-rw-r--r--   0        0        0     5390 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin
+-rw-r--r--   0        0        0     5417 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin
+-rw-r--r--   0        0        0      108 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.1.xml.bin
+-rw-r--r--   0        0        0     1030 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin
+-rw-r--r--   0        0        0     1040 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin
+-rw-r--r--   0        0        0     1030 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin
+-rw-r--r--   0        0        0     1040 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin
+-rw-r--r--   0        0        0     2171 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin
+-rw-r--r--   0        0        0     2247 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin
+-rw-r--r--   0        0        0     2171 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin
+-rw-r--r--   0        0        0     2247 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin
+-rw-r--r--   0        0        0     2957 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/test_component.py
+-rw-r--r--   0        0        0     3283 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/test_deserialize_json.py
+-rw-r--r--   0        0        0     1764 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/test_deserialize_xml.py
+-rw-r--r--   0        0        0    19038 2024-03-18 18:13:08.186144 cyclonedx_python_lib-6.4.4/tests/test_enums.py
+-rw-r--r--   0        0        0     4389 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_factory_license.py
+-rw-r--r--   0        0        0    22571 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model.py
+-rw-r--r--   0        0        0    13219 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_bom.py
+-rw-r--r--   0        0        0     2782 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_bom_ref.py
+-rw-r--r--   0        0        0    18544 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_component.py
+-rw-r--r--   0        0        0     1793 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_dependency.py
+-rw-r--r--   0        0        0     4064 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_issue.py
+-rw-r--r--   0        0        0     4295 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_license.py
+-rw-r--r--   0        0        0     2758 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_release_note.py
+-rw-r--r--   0        0        0     3390 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_service.py
+-rw-r--r--   0        0        0    14370 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_model_vulnerability.py
+-rw-r--r--   0        0        0     3154 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_output.py
+-rw-r--r--   0        0        0     4335 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_output_json.py
+-rw-r--r--   0        0        0     3663 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_output_xml.py
+-rw-r--r--   0        0        0     1307 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_real_world_examples.py
+-rw-r--r--   0        0        0     2524 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_schema_SchemaVersion.py
+-rw-r--r--   0        0        0     1248 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_schema__res.py
+-rw-r--r--   0        0        0     2873 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_spdx.py
+-rw-r--r--   0        0        0     1977 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_validation.py
+-rw-r--r--   0        0        0     4529 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_validation_json.py
+-rw-r--r--   0        0        0     3061 2024-03-18 18:13:08.190144 cyclonedx_python_lib-6.4.4/tests/test_validation_xml.py
+-rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 cyclonedx_python_lib-6.4.4/PKG-INFO
```

### Comparing `cyclonedx_python_lib-6.4.3/CHANGELOG.md` & `cyclonedx_python_lib-6.4.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,43 @@
 # CHANGELOG
 
 
 
+## v6.4.3 (2024-03-04)
+
+### Chore
+
+* chore(deps-dev): update ddt requirement from 1.7.1 to 1.7.2 (#563)
+
+Updates the requirements on [ddt](https://github.com/datadriventests/ddt) to permit the latest version.
+- [Release notes](https://github.com/datadriventests/ddt/releases)
+- [Commits](https://github.com/datadriventests/ddt/compare/1.7.1...1.7.2)
+
+---
+updated-dependencies:
+- dependency-name: ddt
+  dependency-type: direct:development
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt;
+Co-authored-by: dependabot[bot] &lt;49699333+dependabot[bot]@users.noreply.github.com&gt; ([`53cb8a9`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/53cb8a9aa2630e992467525ff246a0f6e6759100))
+
+### Fix
+
+* fix: serialization of `model.component.Diff` (#557)
+
+Fixes #556 
+
+---------
+
+Signed-off-by: rcross-lc &lt;151086351+rcross-lc@users.noreply.github.com&gt;
+Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt;
+Co-authored-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`22fa873`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/22fa8734bf1a3a8789ad7578bfa0c86cf0a49d4a))
+
+
 ## v6.4.2 (2024-03-01)
 
 ### Build
 
 * build: use poetry v1.8.1 (#560)
 
 Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`6f81dfa`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/6f81dfaed32b76f251647f6291791e714ab158a3))
```

### Comparing `cyclonedx_python_lib-6.4.3/LICENSE` & `cyclonedx_python_lib-6.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/README.md` & `cyclonedx_python_lib-6.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
 """
 Python library for CycloneDX
 """
 
 # !! version is managed by semantic_release
 # do not use typing here, or else `semantic_release` might have issues finding the variable
-__version__ = "6.4.3"  # noqa:Q000
+__version__ = "6.4.4"  # noqa:Q000
```

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/_internal/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/_internal/compare.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/_internal/compare.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/_internal/hash.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/_internal/hash.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/_internal/time.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/_internal/time.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/exception/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/exception/factory.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/exception/factory.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/exception/model.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/exception/model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/exception/output.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/exception/output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/exception/serialization.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/exception/serialization.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/factory/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/factory/license.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/factory/license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/bom.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/bom_ref.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/component.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/dependency.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/impact_analysis.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/impact_analysis.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/issue.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/license.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/release_note.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/service.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/service.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/model/vulnerability.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/model/vulnerability.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/output/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/output/json.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/output/json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/output/xml.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/output/xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/README.md` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/README.md`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/schema/schema.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/serialization/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/spdx.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/validation/__init__.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/validation/json.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/validation/json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/validation/model.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/validation/model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/cyclonedx/validation/xml.py` & `cyclonedx_python_lib-6.4.4/cyclonedx/validation/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         XMLParser,
         XMLSchema,
         fromstring as xml_fromstring,
     )
 except ImportError as err:
     _missing_deps_error = MissingOptionalDependencyException(
         'This functionality requires optional dependencies.\n'
-        'Please install `cyclonedx-python-lib` with the extra "json-validation".\n'
+        'Please install `cyclonedx-python-lib` with the extra "xml-validation".\n'
     ), err
 
 
 class _BaseXmlValidator(BaseSchemabasedValidator, ABC):
 
     @property
     def output_format(self) -> Literal[OutputFormat.XML]:
```

### Comparing `cyclonedx_python_lib-6.4.3/docs/Makefile` & `cyclonedx_python_lib-6.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/architecture.rst` & `cyclonedx_python_lib-6.4.4/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/changelog.rst` & `cyclonedx_python_lib-6.4.4/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/conf.py` & `cyclonedx_python_lib-6.4.4/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 project = 'CycloneDX Python Library'
 copyright = '2022, Copyright (c) OWASP Foundation'
 author = 'Paul Horton, Jan Kowalleck, Steve Springett, Patrick Dwyer'
 
 # The full version, including alpha/beta/rc tags
 # !! version is managed by semantic_release
-release = '6.4.3'
+release = '6.4.4'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `cyclonedx_python_lib-6.4.3/docs/examples.rst` & `cyclonedx_python_lib-6.4.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/index.rst` & `cyclonedx_python_lib-6.4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/install.rst` & `cyclonedx_python_lib-6.4.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/make.bat` & `cyclonedx_python_lib-6.4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/modelling.rst` & `cyclonedx_python_lib-6.4.4/docs/modelling.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/outputting.rst` & `cyclonedx_python_lib-6.4.4/docs/outputting.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/schema-support.rst` & `cyclonedx_python_lib-6.4.4/docs/schema-support.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/docs/support.rst` & `cyclonedx_python_lib-6.4.4/docs/support.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/examples/complex_deserialize.py` & `cyclonedx_python_lib-6.4.4/examples/complex_deserialize.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/examples/complex_serialize.py` & `cyclonedx_python_lib-6.4.4/examples/complex_serialize.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/pyproject.toml` & `cyclonedx_python_lib-6.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cyclonedx-python-lib"
 # !! version is managed by semantic_release
-version = "6.4.3"
+version = "6.4.4"
 description = "Python library for CycloneDX"
 authors = [
   "Paul Horton <phorton@sonatype.com>",
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
 ]
 maintainers = [
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
@@ -78,28 +78,28 @@
 [tool.poetry.extras]
 validation = ["jsonschema", "lxml"]
 json-validation = ["jsonschema"]
 xml-validation = ["lxml"]
 
 [tool.poetry.group.dev.dependencies]
 ddt = "1.7.2"
-coverage = "7.4.3"
+coverage = "7.4.4"
 flake8 = { version="7.0.0", python=">=3.8.1" }
 flake8-annotations = { version="3.0.1", python=">=3.8.1" }
 flake8-bugbear = { version="24.2.6", python=">=3.8.1" }
 flake8-isort = "6.1.1"
 flake8-quotes = "3.4.0"
 flake8-use-fstring = "1.4"
 pep8-naming = "0.13.3"
 isort = "5.13.2"
 autopep8 = "2.0.4"
-mypy = "1.8.0"
-tox = "4.13.0"
+mypy = "1.9.0"
+tox = "4.14.1"
 xmldiff = "2.6.3"
-bandit = "1.7.7"
+bandit = "1.7.8"
 
 [tool.semantic_release]
 # see https://python-semantic-release.readthedocs.io/en/latest/configuration.html
 commit_author = "semantic-release <semantic-release>"
 commit_message = "chore(release): {version}\n\nAutomatically generated by python-semantic-release\n\nSigned-off-by: semantic-release <semantic-release>"
 upload_to_vcs_release = true
 build_command = "pip install poetry && poetry build"
```

### Comparing `cyclonedx_python_lib-6.4.3/tests/__init__.py` & `cyclonedx_python_lib-6.4.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/__init__.py` & `cyclonedx_python_lib-6.4.4/tests/_data/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/models.py` & `cyclonedx_python_lib-6.4.4/tests/_data/models.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/own/json/1.2/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.2/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/own/json/1.3/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.3/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/own/json/1.4/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-6.4.4/tests/_data/own/json/1.4/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/own/xml/1.4/bom_setuptools.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/own/xml/1.4/bom_setuptools.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/own/xml/1.4/webgoat-6.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/own/xml/1.4/webgoat-6.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-bom-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-patch-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-service-1.2.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-service-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-service-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-bom-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-patch-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-properties-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-service-1.3.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-service-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-service-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-bom-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-patch-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-properties-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-service-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-service-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-service-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-bom-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-patch-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-properties-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-service-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-service-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-service-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/schemaTestData/fetch.sh` & `cyclonedx_python_lib-6.4.4/tests/_data/schemaTestData/fetch.sh`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_Encoding-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_Encoding-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin` & `cyclonedx_python_lib-6.4.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_component.py` & `cyclonedx_python_lib-6.4.4/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_deserialize_json.py` & `cyclonedx_python_lib-6.4.4/tests/test_deserialize_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_deserialize_xml.py` & `cyclonedx_python_lib-6.4.4/tests/test_deserialize_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_enums.py` & `cyclonedx_python_lib-6.4.4/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_factory_license.py` & `cyclonedx_python_lib-6.4.4/tests/test_factory_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model.py` & `cyclonedx_python_lib-6.4.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model_bom.py` & `cyclonedx_python_lib-6.4.4/tests/test_model_bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model_bom_ref.py` & `cyclonedx_python_lib-6.4.4/tests/test_model_bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model_component.py` & `cyclonedx_python_lib-6.4.4/tests/test_model_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model_dependency.py` & `cyclonedx_python_lib-6.4.4/tests/test_model_dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model_issue.py` & `cyclonedx_python_lib-6.4.4/tests/test_model_issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model_license.py` & `cyclonedx_python_lib-6.4.4/tests/test_model_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model_release_note.py` & `cyclonedx_python_lib-6.4.4/tests/test_model_release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model_service.py` & `cyclonedx_python_lib-6.4.4/tests/test_model_service.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_model_vulnerability.py` & `cyclonedx_python_lib-6.4.4/tests/test_model_vulnerability.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_output.py` & `cyclonedx_python_lib-6.4.4/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_output_json.py` & `cyclonedx_python_lib-6.4.4/tests/test_output_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_output_xml.py` & `cyclonedx_python_lib-6.4.4/tests/test_output_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_real_world_examples.py` & `cyclonedx_python_lib-6.4.4/tests/test_real_world_examples.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_schema_SchemaVersion.py` & `cyclonedx_python_lib-6.4.4/tests/test_schema_SchemaVersion.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_schema__res.py` & `cyclonedx_python_lib-6.4.4/tests/test_schema__res.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_spdx.py` & `cyclonedx_python_lib-6.4.4/tests/test_spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_validation.py` & `cyclonedx_python_lib-6.4.4/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_validation_json.py` & `cyclonedx_python_lib-6.4.4/tests/test_validation_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/tests/test_validation_xml.py` & `cyclonedx_python_lib-6.4.4/tests/test_validation_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-6.4.3/PKG-INFO` & `cyclonedx_python_lib-6.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclonedx-python-lib
-Version: 6.4.3
+Version: 6.4.4
 Summary: Python library for CycloneDX
 Home-page: https://github.com/CycloneDX/cyclonedx-python-lib/#readme
 License: Apache-2.0
 Keywords: CycloneDX,library,OWASP,SCA,Software Bill of Materials,Bill of Materials,BOM,SBOM,VEX,VDR,OBOM,MBOM,SaaSBOM,SPDX,PackageURL,PURL
 Author: Paul Horton
 Author-email: phorton@sonatype.com
 Maintainer: Jan Kowalleck
```

