# Comparing `tmp/fprime-gds-3.4.3.tar.gz` & `tmp/fprime-gds-3.4.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fprime-gds-3.4.3.tar", last modified: Fri Feb 16 04:11:59 2024, max compression
+gzip compressed data, was "fprime-gds-3.4.4a1.tar", last modified: Tue Apr  9 17:47:55 2024, max compression
```

## Comparing `fprime-gds-3.4.3.tar` & `fprime-gds-3.4.4a1.tar`

### file list

```diff
@@ -1,347 +1,354 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/ISSUE_TEMPLATE/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.503810 fprime-gds-3.4.3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/.github/actions/codeql/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/actions/codeql/security-pack.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/.github/actions/spelling/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/actions/spelling/excludes.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/actions/spelling/expect.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/actions/spelling/patterns.txt
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/.github/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    87604 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/resources/RefTopologyAppDictionary.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/workflows/codeql-security-scan.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/workflows/fprime-gds-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/workflows/gds-cli-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.github/workflows/spelling.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)   106207 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24742 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.507810 fprime-gds-3.4.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/docs/_static/css/rtd_width.css
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/docs/gendoc.bash
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/examples/simple_sequence.bin
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/examples/simple_sequence.seq
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.515810 fprime-gds-3.4.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fastentrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.519810 fprime-gds-3.4.3/src/fprime_gds/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.519810 fprime-gds-3.4.3/src/fprime_gds/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.519810 fprime-gds-3.4.3/src/fprime_gds/common/communication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/communication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.519810 fprime-gds-3.4.3/src/fprime_gds/common/communication/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/communication/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/communication/adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/communication/adapters/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/communication/adapters/uart.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/communication/checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/communication/framing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/communication/ground.py
--rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/communication/updown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.519810 fprime-gds-3.4.3/src/fprime_gds/common/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.523810 fprime-gds-3.4.3/src/fprime_gds/common/data_types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/data_types/ch_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/data_types/cmd_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/data_types/event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/data_types/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/data_types/file_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/data_types/pkt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/data_types/sys_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.523810 fprime-gds-3.4.3/src/fprime_gds/common/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/decoders/ch_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/decoders/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/decoders/event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/decoders/file_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/decoders/pkt_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.523810 fprime-gds-3.4.3/src/fprime_gds/common/distributor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/distributor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/distributor/distributor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.523810 fprime-gds-3.4.3/src/fprime_gds/common/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/encoders/ch_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/encoders/cmd_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/encoders/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/encoders/event_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/encoders/file_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/encoders/pkt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/encoders/seq_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.523810 fprime-gds-3.4.3/src/fprime_gds/common/files/
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/files/File Decoder Documentation.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/files/downlinker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/files/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/files/uplinker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.527810 fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/base_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/command_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/filtering_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.527810 fprime-gds-3.4.3/src/fprime_gds/common/history/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/history/chrono.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/history/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/history/ram.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/history/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.527810 fprime-gds-3.4.3/src/fprime_gds/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/ch_py_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/ch_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/cmd_py_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/cmd_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/dict_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/event_py_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/event_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/pkt_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/python_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    14121 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/loaders/xml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.527810 fprime-gds-3.4.3/src/fprime_gds/common/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/logger/data_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/logger/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.527810 fprime-gds-3.4.3/src/fprime_gds/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.527810 fprime-gds-3.4.3/src/fprime_gds/common/models/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/models/common/channel_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/models/common/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/models/common/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.531810 fprime-gds-3.4.3/src/fprime_gds/common/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/parsers/seq_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.531810 fprime-gds-3.4.3/src/fprime_gds/common/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/pipeline/dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/pipeline/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/pipeline/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/pipeline/histories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/pipeline/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/pipeline/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.531810 fprime-gds-3.4.3/src/fprime_gds/common/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/templates/ch_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/templates/cmd_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/templates/data_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/templates/event_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/templates/pkt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.531810 fprime-gds-3.4.3/src/fprime_gds/common/testing_fw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/testing_fw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60566 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/testing_fw/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18371 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/testing_fw/predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/testing_fw/pytest_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.531810 fprime-gds-3.4.3/src/fprime_gds/common/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/tools/seqgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.531810 fprime-gds-3.4.3/src/fprime_gds/common/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/utils/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/utils/data_desc_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/utils/event_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/utils/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/common/zmq_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.535810 fprime-gds-3.4.3/src/fprime_gds/executables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/executables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31127 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/executables/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/executables/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/executables/fprime_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/executables/run_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/executables/tcpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/executables/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.535810 fprime-gds-3.4.3/src/fprime_gds/flask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.535810 fprime-gds-3.4.3/src/fprime_gds/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.535810 fprime-gds-3.4.3/src/fprime_gds/flask/static/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/.idea/static.iml
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/.idea/vcs.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.539810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.539810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/advanced-settings/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/advanced-settings/addon-templates.js
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/advanced-settings/addon.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.539810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/channel-render/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/channel-render/addon.js
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/channel-render/channel-render-template.js
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/channel-render/channel-render.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.539810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/addon-templates.js
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/addon.js
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.539810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    30243 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-streaming.js
--rw-r--r--   0 runner    (1001) docker     (127)    29512 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-zoom.js
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/flat.js
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/sibling.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.539810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)   184059 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/vendor/chart.js
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/vendor/chartjs-adapter-luxon.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20727 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/vendor/hammer.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.543810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/addon.js
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/argument-templates.js
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/arguments.js
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-history-template.js
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-history.js
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-input-template.js
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-input.js
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-string-template.js
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-string.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.543810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/dictionary/addon-templates.js
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/dictionary/addon.js
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/enabled.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.543810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/image-display/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/image-display/addon.js
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/image-display/dashboard.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.543810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/addon-templates.js
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/addon.js
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/autocomplete.js
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/lint.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.543810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/
--rw-r--r--   0 runner    (1001) docker     (127)   813045 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/code-mirror.es.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.543810 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/rollup/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/rollup/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/rollup/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/rollup/language.grammer
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/rollup/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/rollup/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.543810 fprime-gds-3.4.3/src/fprime_gds/flask/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)   180390 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/css/fprime.css
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/css/fpstyle.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.547810 fprime-gds-3.4.3/src/fprime_gds/flask/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/img/error.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/img/success.svg
--rw-r--r--   0 runner    (1001) docker     (127)    26087 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.547810 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/config.js
--rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/datastore.js
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/gds.js
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/loader.js
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/performance.js
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/uploader.js
--rw-r--r--   0 runner    (1001) docker     (127)    13046 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/validate.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.547810 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/channel.js
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/dashboard-box.js
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/dashboard-row.js
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/downlink.js
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/event.js
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/fp-row.js
--rw-r--r--   0 runner    (1001) docker     (127)    18646 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/fptable.js
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/log.js
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/tabetc.js
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/uplink.js
--rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.511810 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.551810 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/css/
--rw-r--r--   0 runner    (1001) docker     (127)    59305 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   161364 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/css/vue-select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.551810 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/
--rw-r--r--   0 runner    (1001) docker     (127)    72827 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/luxon.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    16877 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/sorttable.js
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/v-runtime-template.js
--rw-r--r--   0 runner    (1001) docker     (127)    16999 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/vue-select.js
--rw-r--r--   0 runner    (1001) docker     (127)    93675 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/vue.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.555810 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   134294 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   747927 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   133988 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    89988 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    76736 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34034 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144714 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    33736 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   203030 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   918991 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   202744 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   101648 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    78268 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/flask/updown.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/src/fprime_gds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/src/fprime_gds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24742 2024-02-16 04:11:59.000000 fprime-gds-3.4.3/src/fprime_gds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-02-16 04:11:59.000000 fprime-gds-3.4.3/src/fprime_gds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 04:11:59.000000 fprime-gds-3.4.3/src/fprime_gds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-16 04:11:59.000000 fprime-gds-3.4.3/src/fprime_gds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-16 04:11:59.000000 fprime-gds-3.4.3/src/fprime_gds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 04:11:59.000000 fprime-gds-3.4.3/src/fprime_gds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.511810 fprime-gds-3.4.3/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.511810 fprime-gds-3.4.3/test/fprime_gds/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.511810 fprime-gds-3.4.3/test/fprime_gds/common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.555810 fprime-gds-3.4.3/test/fprime_gds/common/distributor/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/distributor/test_distributor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.555810 fprime-gds-3.4.3/test/fprime_gds/common/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/encoders/test_ch_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/encoders/test_event_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/encoders/test_pkt_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/test/fprime_gds/common/gds_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/gds_cli/filtering_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/gds_cli/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/test/fprime_gds/common/history/
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/history/chronohistory_unit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/history/testhistory_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/test/fprime_gds/common/testing_fw/
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/testing_fw/UnitTestDictionary.xml
--rw-r--r--   0 runner    (1001) docker     (127)    39899 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/testing_fw/api_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/test/fprime_gds/common/testing_fw/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/testing_fw/logs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/testing_fw/predicate_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/test/fprime_gds/common/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/tools/seqgen_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/test/fprime_gds/common/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/common/utils/test_string_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/test/fprime_gds/executables/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/executables/test_run_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/fprime_gds/executables/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 04:11:59.559810 fprime-gds-3.4.3/test/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-02-16 04:11:51.000000 fprime-gds-3.4.3/test/gui/GUI_Test_Procedure.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.581724 fprime-gds-3.4.4a1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.525724 fprime-gds-3.4.4a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.525724 fprime-gds-3.4.4a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/ISSUE_TEMPLATE/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.517724 fprime-gds-3.4.4a1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.525724 fprime-gds-3.4.4a1/.github/actions/codeql/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/actions/codeql/security-pack.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.525724 fprime-gds-3.4.4a1/.github/actions/spelling/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/actions/spelling/excludes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/actions/spelling/expect.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/actions/spelling/patterns.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.525724 fprime-gds-3.4.4a1/.github/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    87604 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/resources/RefTopologyAppDictionary.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.529724 fprime-gds-3.4.4a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/workflows/codeql-security-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/workflows/fprime-gds-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/workflows/gds-cli-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.github/workflows/spelling.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)   106207 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-04-09 17:47:55.581724 fprime-gds-3.4.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.529724 fprime-gds-3.4.4a1/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.529724 fprime-gds-3.4.4a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.517724 fprime-gds-3.4.4a1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.529724 fprime-gds-3.4.4a1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/docs/_static/css/rtd_width.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/docs/gendoc.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.529724 fprime-gds-3.4.4a1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/examples/simple_sequence.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/examples/simple_sequence.seq
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:47:55.581724 fprime-gds-3.4.4a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.529724 fprime-gds-3.4.4a1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fastentrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.529724 fprime-gds-3.4.4a1/src/fprime_gds/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.533724 fprime-gds-3.4.4a1/src/fprime_gds/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.533724 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.533724 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17074 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/adapters/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/adapters/uart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/framing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/ground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/communication/updown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.533724 fprime-gds-3.4.4a1/src/fprime_gds/common/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.533724 fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/ch_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/cmd_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/pkt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/sys_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.537724 fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/ch_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/file_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/pkt_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.537724 fprime-gds-3.4.4a1/src/fprime_gds/common/distributor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/distributor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/distributor/distributor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.537724 fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/ch_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/cmd_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/event_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/file_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/pkt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/seq_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.537724 fprime-gds-3.4.4a1/src/fprime_gds/common/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/files/File Decoder Documentation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/files/downlinker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/files/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/files/uplinker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.541724 fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/base_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/command_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/filtering_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.541724 fprime-gds-3.4.4a1/src/fprime_gds/common/history/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/history/chrono.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/history/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/history/ram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/history/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.541724 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/ch_py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/ch_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/cmd_py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/cmd_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/dict_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/event_py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/event_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/pkt_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/python_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14121 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/xml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.541724 fprime-gds-3.4.4a1/src/fprime_gds/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/logger/data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/logger/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.541724 fprime-gds-3.4.4a1/src/fprime_gds/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.545724 fprime-gds-3.4.4a1/src/fprime_gds/common/models/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/models/common/channel_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/models/common/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/models/common/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.545724 fprime-gds-3.4.4a1/src/fprime_gds/common/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/parsers/seq_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.545724 fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.545724 fprime-gds-3.4.4a1/src/fprime_gds/common/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/templates/ch_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/templates/cmd_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/templates/data_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/templates/event_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/templates/pkt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.545724 fprime-gds-3.4.4a1/src/fprime_gds/common/testing_fw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/testing_fw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60566 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/testing_fw/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18371 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/testing_fw/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/testing_fw/pytest_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.545724 fprime-gds-3.4.4a1/src/fprime_gds/common/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/tools/seqgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.549724 fprime-gds-3.4.4a1/src/fprime_gds/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/utils/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/utils/data_desc_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/utils/event_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/utils/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/common/zmq_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.549724 fprime-gds-3.4.4a1/src/fprime_gds/executables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/executables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/executables/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36942 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/executables/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/executables/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/executables/fprime_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/executables/run_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/executables/tcpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/executables/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.553724 fprime-gds-3.4.4a1/src/fprime_gds/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.553724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.553724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 17:47:46.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/.idea/static.iml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/.idea/vcs.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.553724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.553724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/advanced-settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/advanced-settings/addon-templates.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/advanced-settings/addon.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.553724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/channel-render/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/channel-render/addon.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/channel-render/channel-render-template.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/channel-render/channel-render.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.553724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/addon-templates.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/addon.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.557724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    30243 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-streaming.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29512 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-zoom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/flat.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/sibling.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.557724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)   184059 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/vendor/chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/vendor/chartjs-adapter-luxon.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20727 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/vendor/hammer.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.557724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/addon.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/argument-templates.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/arguments.js
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-history-template.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-history.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-input-template.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-input.js
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-string-template.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-string.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.557724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/dictionary/addon-templates.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/dictionary/addon.js
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/enabled.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.557724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/image-display/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/image-display/addon.js
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/image-display/dashboard.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.561724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/addon-templates.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/addon.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/autocomplete.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/lint.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.561724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/
+-rw-r--r--   0 runner    (1001) docker     (127)   813045 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/code-mirror.es.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.561724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/language.grammer
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.561724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   180390 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/css/fprime.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/css/fpstyle.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.561724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/img/error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/img/success.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26087 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.565724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/datastore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/gds.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/performance.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/uploader.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13046 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/validate.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.565724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/channel.js
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/dashboard-box.js
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/dashboard-row.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/downlink.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/event.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/fp-row.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18646 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/fptable.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/log.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/tabetc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/uplink.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.521724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.565724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    59305 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   161364 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/css/vue-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.569724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    72827 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/luxon.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16877 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/sorttable.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/v-runtime-template.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16999 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/vue-select.js
+-rw-r--r--   0 runner    (1001) docker     (127)    93675 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/vue.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   134294 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   747927 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   133988 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    89988 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76736 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34034 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144714 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    33736 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   203030 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   918991 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   202744 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   101648 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    78268 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/flask/updown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/src/fprime_gds/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/plugin/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/plugin/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/src/fprime_gds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.581724 fprime-gds-3.4.4a1/src/fprime_gds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-04-09 17:47:55.000000 fprime-gds-3.4.4a1/src/fprime_gds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-04-09 17:47:55.000000 fprime-gds-3.4.4a1/src/fprime_gds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:47:55.000000 fprime-gds-3.4.4a1/src/fprime_gds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 17:47:55.000000 fprime-gds-3.4.4a1/src/fprime_gds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 17:47:55.000000 fprime-gds-3.4.4a1/src/fprime_gds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 17:47:55.000000 fprime-gds-3.4.4a1/src/fprime_gds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.525724 fprime-gds-3.4.4a1/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.525724 fprime-gds-3.4.4a1/test/fprime_gds/common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/common/distributor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/distributor/test_distributor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/common/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/encoders/test_ch_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/encoders/test_event_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/encoders/test_pkt_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/common/gds_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/gds_cli/filtering_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/gds_cli/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/common/history/
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/history/chronohistory_unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/history/testhistory_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/common/testing_fw/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/testing_fw/UnitTestDictionary.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    39899 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/testing_fw/api_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/common/testing_fw/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/testing_fw/logs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/testing_fw/predicate_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/common/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/tools/seqgen_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/common/utils/test_string_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/executables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/executables/test_run_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/executables/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.577724 fprime-gds-3.4.4a1/test/fprime_gds/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)   104503 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/sample/dictionary.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/fprime_gds/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:47:55.581724 fprime-gds-3.4.4a1/test/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-09 17:47:47.000000 fprime-gds-3.4.4a1/test/gui/GUI_Test_Procedure.md
```

### Comparing `fprime-gds-3.4.3/.github/actions/spelling/expect.txt` & `fprime-gds-3.4.4a1/.github/actions/spelling/expect.txt`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,16 @@
 hhc
 hhk
 hhp
 hidecallergraph
 hidecallgraph
 hideinitializer
 hlp
+Hookimpl
+hookspec
 hostname
 hpaulson
 hpp
 href
 htags
 htm
 html
@@ -309,14 +311,15 @@
 instanceof
 intersphinx
 intlimits
 ints
 ip
 ipc
 ipp
+isabstract
 isalnum
 isclass
 isdir
 isfile
 isinstance
 isroutine
 issubclass
```

### Comparing `fprime-gds-3.4.3/.github/actions/spelling/patterns.txt` & `fprime-gds-3.4.4a1/.github/actions/spelling/patterns.txt`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/.github/pull_request_template.md` & `fprime-gds-3.4.4a1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/.github/resources/RefTopologyAppDictionary.xml` & `fprime-gds-3.4.4a1/.github/resources/RefTopologyAppDictionary.xml`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/.github/workflows/codeql-security-scan.yml` & `fprime-gds-3.4.4a1/.github/workflows/codeql-security-scan.yml`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/.github/workflows/fprime-gds-tests.yml` & `fprime-gds-3.4.4a1/.github/workflows/fprime-gds-tests.yml`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/.github/workflows/gds-cli-tests.yml` & `fprime-gds-3.4.4a1/.github/workflows/gds-cli-tests.yml`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/.github/workflows/publish.yml` & `fprime-gds-3.4.4a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/.github/workflows/spelling.yml` & `fprime-gds-3.4.4a1/.github/workflows/spelling.yml`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/.gitignore` & `fprime-gds-3.4.4a1/.gitignore`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/Doxyfile` & `fprime-gds-3.4.4a1/Doxyfile`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/LICENSE.txt` & `fprime-gds-3.4.4a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/NOTICE.txt` & `fprime-gds-3.4.4a1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/PKG-INFO` & `fprime-gds-3.4.4a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime-gds
-Version: 3.4.3
+Version: 3.4.4a1
 Summary: F Prime Flight Software Ground Data System layer
 Author-email: Michael Starch <Michael.D.Starch@jpl.nasa.gov>, Thomas Boyer-Chammard <Thomas.Boyer.Chammard@jpl.nasa.gov>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `fprime-gds-3.4.3/README.md` & `fprime-gds-3.4.4a1/README.md`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/docs/README.md` & `fprime-gds-3.4.4a1/docs/README.md`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/docs/_static/css/rtd_width.css` & `fprime-gds-3.4.4a1/docs/_static/css/rtd_width.css`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/docs/conf.py` & `fprime-gds-3.4.4a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/docs/index.rst` & `fprime-gds-3.4.4a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/examples/simple_sequence.seq` & `fprime-gds-3.4.4a1/examples/simple_sequence.seq`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/pyproject.toml` & `fprime-gds-3.4.4a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -81,7 +81,11 @@
 # - package_data: included by default, and setuptools_scm will automatically include all files tracked by git
 # - package discovery (src/): setuptools will automatically discover all packages as we use the src-layout
 #
 # Reference:
 # - https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # - https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout
 ####
+[tool.pytest.ini_options]
+markers =[
+  "gds_cli"
+]
```

### Comparing `fprime-gds-3.4.3/src/fastentrypoints.py` & `fprime-gds-3.4.4a1/src/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/communication/adapters/base.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/communication/adapters/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 with various wire formats as they are supported by the F prime comm-layer. This file defines a single abstract base
 class representing the core features of the adapter class that must be implemented by every implementation of the
 adapter for use with the comm-layer.
 
 @author lestarch
 """
 import abc
+from typing import Type
+from fprime_gds.plugin.definitions import gds_plugin_implementation, gds_plugin_specification
 
 
 class BaseAdapter(abc.ABC):
     """
     Base adapter for adapting the communications layer. This essentially breaks down to providing the ability to read
     data from, and write to the necessary wire-format. The children of this class must at least implement the 'read' and
     'write' functions to ensure that data can be read and written. 'open' and 'close' are also provided as a helper to
@@ -43,75 +45,45 @@
         Write to the interface. Must be overridden by the child adapter. Throw no fatal errors, reconnect instead.
 
         :param frame: framed data to uplink
         :return: True if data sent through adapter, False otherwise
         """
 
     @classmethod
-    @abc.abstractmethod
-    def get_arguments(cls):
-        """
-        Returns a set of arguments consumed by this adapter. This will be consumed by the CLI layer in order to provide
-        command line arguments to the user. Note: these should be globally unique args, e.g. --ip-address
+    @gds_plugin_specification
+    def register_communication_plugin(cls) -> Type["BaseAdapter"]:
+        """Register a communications adapter
 
-        :return: dictionary, keys of tuple of arg flags and value of list of other arguments to argparse's add_argument
-        """
+        Plugin hook for registering a plugin that supplies an adapter to the communications interface (radio, uart, i2c,
+        etc). This interface is expected to read and write bytes from a wire and will be provided to the framing system.
 
-    @classmethod
-    @abc.abstractmethod
-    def check_arguments(cls, args):
-        """
-        Code that should check arguments of this adapter. If there is a problem with this code, then a "ValueError"
-        should be raised describing the problem with these arguments.
+        Note: users should return the class, not an instance of the class. Needed arguments for instantiation are
+        determined from class methods, solicited via the command line, and provided at construction time to the chosen
+        instantiation.
 
-        :param args: arguments as dictionary
+        Returns:
+            BaseAdapter subclass
         """
+        raise NotImplementedError()
 
-    @classmethod
-    def get_adapters(cls):
-        """
-        Get all known adapters of this base class. These must be imported into the comm-layer to be available to the
-        system, however; they only need to be imported. Once imported this function will find them and make them
-        available to the comm-layer in the standard way.
 
-        :return: list of all imported comm adapters.
-        """
-        adapter_map = {}
-        for adapter in cls.__subclasses__():
-            # Get two versions of names
-            adapter_name = adapter.__module__
-            adapter_short = adapter_name.split(".")[-1]
-            # Check to use long or short name
-            if adapter_short not in adapter_map:
-                adapter_name = adapter_short
-            adapter_map[adapter_name] = adapter
-        return adapter_map
+class NoneAdapter(BaseAdapter):
+    """ None adapter used to turn off the comm script """
 
-    @staticmethod
-    def process_arguments(clazz, args):
-        """
-        Process arguments incoming from the command line and construct a dictionary of kwargs to supply to the chosen
-        adapter at creation time. This will allow the user to choose any imported adapters at runtime.
+    @classmethod
+    def get_name(cls):
+        """ Get name of the non-adapter """
+        return "none"
 
-        :param args: arguments to process
-        :return: dictionary of constructor keyword arguments
-        """
-        return {
-            value["dest"]: getattr(args, value["dest"])
-            for value in clazz.get_arguments().values()
-        }
+    def read(self, timeout=0.500):
+        """ Raise exception if this is called"""
+        raise NotImplementedError()
+
+    def write(self, frame):
+        """ Raise exception if this is called"""
+        raise NotImplementedError()
 
     @classmethod
-    def construct_adapter(cls, adapter_name, args):
-        """
-        Constructs a new adapter, from the given adapter name and the given namespace of argument inputs. This is a
-        wrapper of "get_adapters" and "process_arguments" to help build a new, fully configured, adapter. This is a
-        factory method.
-
-        :param adapter_name: name of the adapter to build
-        :param args: namespace of arg value to help build an adapter
-        :return: newly constructed adapter
-        """
-        if adapter_name == "none":
-            return None
-        adapter = cls.get_adapters()[adapter_name]
-        return adapter(**cls.process_arguments(adapter, args))
+    @gds_plugin_implementation
+    def register_communication_plugin(cls):
+        """ Register this as a plugin """
+        return cls
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/communication/adapters/ip.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/communication/adapters/ip.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import socket
 import threading
 import time
 
 import fprime_gds.common.communication.adapters.base
 import fprime_gds.common.logger
 
+from fprime_gds.plugin.definitions import gds_plugin_implementation
+
 LOGGER = logging.getLogger("ip_adapter")
 
 
 def check_port(address, port):
     """
     Checks a given address and port to ensure that it is available. If not available, a ValueError is raised. Note: this
     is done by binding to an address. It does not call "listen"
@@ -110,15 +112,15 @@
         handler.open()
         while not self.stop:
             self.data_chunks.put(handler.read())
         handler.close()
 
     def write(self, frame):
         """
-        Send a given framed bit of data by sending it out the serial interface. It will attempt to reconnect if there is
+        Send a given framed bit of data by sending it out the serial interface. It will attempt to reconnect if there
         was a problem previously. This function will return true on success, or false on error.
 
         :param frame: framed data packet to send out
         :return: True, when data was sent through the UART. False otherwise.
         """
         if self.tcp.connected == IpHandler.CONNECTED:
             return self.tcp.write(frame)
@@ -148,52 +150,68 @@
         given client.
         """
         while not self.stop:
             self.write(IpAdapter.KEEPALIVE_DATA)
             time.sleep(interval)
 
     @classmethod
+    def get_name(cls):
+        """ Get the name of this adapter  """
+        return "ip"
+
+    @classmethod
     def get_arguments(cls):
         """
         Returns a dictionary of flag to argparse-argument dictionaries for use with argparse to setup arguments.
 
         :return: dictionary of flag to argparse arguments for use with argparse
         """
         return {
             ("--ip-address",): {
                 "dest": "address",
                 "type": str,
                 "default": "0.0.0.0",
-                "help": "Address of the IP adapter server. Default: %(default)s",
+                "help": "Address of the IP adapter server.",
             },
             ("--ip-port",): {
                 "dest": "port",
                 "type": int,
                 "default": 50000,
-                "help": "Port of the IP adapter server. Default: %(default)s",
+                "help": "Port of the IP adapter server.",
             },
             ("--ip-client",): {
                 # dest is "server" since it is handled in BaseAdapter.construct_adapter and passed with the same
                 # name to the IpAdapter constructor. Default to server=True, meaning IpAdapter is the TCP server
                 "dest": "server",
                 "action": "store_false",
                 "default": True,
                 "help": "Run the IP adapter as the client (connects to FSW running TcpServer)",
             },
         }
 
     @classmethod
-    def check_arguments(cls, args):
+    @gds_plugin_implementation
+    def register_communication_plugin(cls):
+        """ Register this as a communication plugin """
+        return cls
+
+    @classmethod
+    def check_arguments(cls, address, port, server=True):
         """
         Code that should check arguments of this adapter. If there is a problem with this code, then a "ValueError"
         should be raised describing the problem with these arguments.
 
         :param args: arguments as dictionary
         """
-        check_port(args["address"], args["port"])
+        try:
+            if server:
+                check_port(address, port)
+        except OSError as os_error:
+            raise ValueError(f"{os_error}")
+
 
 
 class IpHandler(abc.ABC):
     """
     Base handler for IP types. This will provide the basic methods, and synchronization for reading/writing to multiple
     child implementations, namely: UDP and TCP. These child objects can then be instantiated individually.
     """
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/communication/adapters/uart.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/communication/adapters/uart.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import logging
 
 import serial
 from serial.tools import list_ports
 
 import fprime_gds.common.communication.adapters.base
 
+from fprime_gds.plugin.definitions import gds_plugin_implementation
+
 LOGGER = logging.getLogger("serial_adapter")
 
 
 class SerialAdapter(fprime_gds.common.communication.adapters.base.BaseAdapter):
     """
     Supplies a data source adapter that is pulling data off from a UART wire using PySerial. This is setup using a
     device handle and a baudrate for the given serial device.
@@ -147,43 +149,54 @@
         )
         default = available[-1] if available else "/dev/ttyACM0"
         return {
             ("--uart-device",): {
                 "dest": "device",
                 "type": str,
                 "default": default,
-                "help": "UART device representing the FSW. Default: %(default)s",
+                "help": "UART device representing the FSW.",
             },
             ("--uart-baud",): {
                 "dest": "baud",
                 "type": int,
                 "default": 9600,
-                "help": "Baud rate of the serial device. Default: %(default)s",
+                "help": "Baud rate of the serial device.",
             },
         }
 
     @classmethod
-    def check_arguments(cls, args):
+    def get_name(cls):
+        """ Get name of the adapter """
+        return "uart"
+
+    @classmethod
+    @gds_plugin_implementation
+    def register_communication_plugin(cls):
+        """ Register this as a communication plugin """
+        return cls
+
+    @classmethod
+    def check_arguments(cls, device, baud):
         """
         Code that should check arguments of this adapter. If there is a problem with this code, then a "ValueError"
         should be raised describing the problem with these arguments.
 
         :param args: arguments as dictionary
         """
         ports = map(lambda info: info.device, list_ports.comports(include_links=True))
-        if args["device"] not in ports:
-            msg = f"Serial port '{args['device']}' not valid. Available ports: {ports}"
+        if device not in ports:
+            msg = f"Serial port '{device}' not valid. Available ports: {ports}"
             raise ValueError(
                 msg
             )
         # Note: baud rate may not *always* work. These are a superset
         try:
-            baud = int(args["baud"])
+            baud = int(baud)
         except ValueError:
-            msg = f"Serial baud rate '{args['baud']}' not integer. Use one of: {SerialAdapter.BAUDS}"
+            msg = f"Serial baud rate '{baud}' not integer. Use one of: {SerialAdapter.BAUDS}"
             raise ValueError(
                 msg
             )
         if baud not in SerialAdapter.BAUDS:
             msg = f"Serial baud rate '{baud}' not supported. Use one of: {SerialAdapter.BAUDS}"
             raise ValueError(
                 msg
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/communication/checksum.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/communication/checksum.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,18 @@
 
 
 def crc_calculation(data: bytes):
     """Initial checksum implementation for FpFramerDeframer."""
     return zlib.crc32(data) & 0xFFFFFFFF
 
 
-CHECKSUM_SELECTION = "crc32"
 CHECKSUM_MAPPING = {
     "fixed": lambda data: 0xCAFECAFE,
     "crc32": crc_calculation,
     "default": crc_calculation,
 }
 
 
-def calculate_checksum(data: bytes):
+def calculate_checksum(data: bytes, selected_checksum: str):
     """Calculates the checksum of bytes"""
-    selected_checksum = CHECKSUM_SELECTION
     hash_fn = CHECKSUM_MAPPING.get(selected_checksum, CHECKSUM_MAPPING.get("default"))
     return hash_fn(data)
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/communication/framing.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/communication/framing.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 
 @author lestarch
 """
 import abc
 import copy
 import struct
 import sys
+from typing import Type
 
-from .checksum import calculate_checksum
+from .checksum import calculate_checksum, CHECKSUM_MAPPING
+from fprime_gds.plugin.definitions import gds_plugin_implementation, gds_plugin_specification
 
 
 class FramerDeframer(abc.ABC):
     """
     Abstract base class of the Framer/Deframer variety. Framers and Deframers have to define two methods, one for
     framing a set of bytes and one for deframing a set of bytes into packets.
     """
@@ -66,14 +68,32 @@
             # Deframe and return only on None
             (packet, data, discarded) = self.deframe(data, no_copy=True)
             discarded_aggregate += discarded
             if packet is None:
                 return packets, data, discarded_aggregate
             packets.append(packet)
 
+    @classmethod
+    @gds_plugin_specification
+    def register_framing_plugin(cls) -> Type["FramerDeframer"]:
+        """Register a plugin to provide framing capabilities
+
+        Plugin hook for registering a plugin that supplies a FramerDeframer implementation. Implementors of this hook must
+        return a non-abstract subclass of FramerDeframer. This class will be provided as a framing implementation option
+        that users may select via command line arguments.
+
+        Note: users should return the class, not an instance of the class. Needed arguments for instantiation are
+        determined from class methods, solicited via the command line, and provided at construction time to the chosen
+        instantiation.
+
+        Returns:
+            FramerDeframer subclass
+        """
+        raise NotImplementedError()
+
 
 class FpFramerDeframer(FramerDeframer):
     """
     Framing object used to read/write in the standard F prime format. This format is compatible with the standard ground
     system. It contains the following format for data:
 
     | token: start word |
@@ -93,18 +113,19 @@
     MAXIMUM_DATA_SIZE = 4096
 
     # Filled by set_constants()
     TOKEN_TYPE = None
     HEADER_FORMAT = None
     START_TOKEN = None
 
-    def __init__(self):
+    def __init__(self, checksum_type):
         """Sets constants on construction."""
         # Setup the constants as soon as possible.
         FpFramerDeframer.set_constants()
+        self.checksum = checksum_type
 
     @classmethod
     def set_constants(cls):
         """
         Setup the constants for the various token sizes. This will ensure that the system can read the tokens properly.
         This can be changed to make the framing more efficient.
         """
@@ -130,15 +151,15 @@
         :param data: bytes to frame
         :return: array of raw bytes representing a framed packet. Should be ready for uplink.
         """
         framed = struct.pack(
             FpFramerDeframer.HEADER_FORMAT, FpFramerDeframer.START_TOKEN, len(data)
         )
         framed += data
-        framed += struct.pack(">I", calculate_checksum(framed))
+        framed += struct.pack(">I", calculate_checksum(framed, self.checksum))
         return framed
 
     def deframe(self, data, no_copy=False):
         """
         Deframes the incoming data from the F prime standard format. Produces exactly one packet, and leftover bytes.
         Users wanting all packets to be deframed should call "deframe_all". If no full packet is available, this method
         returns None. Expects incoming raw bytes to deframe, and returns a deframed packet or None, and the leftover
@@ -172,15 +193,16 @@
             # If the pool is large enough to read the whole frame, then read it
             if len(data) >= total_size:
                 deframed, check = struct.unpack_from(
                     f">{data_size}sI", data, FpFramerDeframer.HEADER_SIZE
                 )
                 # If the checksum is valid, return the packet. Otherwise continue to rotate
                 if check == calculate_checksum(
-                    data[: data_size + FpFramerDeframer.HEADER_SIZE]
+                    data[: data_size + FpFramerDeframer.HEADER_SIZE],
+                    self.checksum
                 ):
                     data = data[total_size:]
                     return deframed, data, discarded
                 print(
                     "[WARNING] Checksum validation failed. Have you correctly set '--comm-checksum-type'",
                     file=sys.stderr,
                 )
@@ -188,14 +210,41 @@
                 discarded += data[0:1]
                 data = data[1:]
                 continue
             # Case of not enough data for a full packet, return hoping for more later
             return None, data, discarded
         return None, data, discarded
 
+    @classmethod
+    def get_name(cls):
+        """ Get the name of this plugin """
+        return "fprime"
+
+    @classmethod
+    def get_arguments(cls):
+        """ Get arguments for the framer/deframer """
+        return {("--comm-checksum-type",): {
+            "dest": "checksum_type",
+            "action": "store",
+            "type": str,
+            "help": "Setup the checksum algorithm. [default: %(default)s]",
+            "choices": [
+                item
+                for item in CHECKSUM_MAPPING.keys()
+                if item != "default"
+            ],
+            "default": "crc32",
+        }}
+
+    @classmethod
+    @gds_plugin_implementation
+    def register_framing_plugin(cls):
+        """ Register a bad plugin """
+        return cls
+
 
 class TcpServerFramerDeframer(FramerDeframer):
     """
     Framing object used to read/write in the Tcp Server format. This format is compatible with the older ground
     system. It contains the following formats for data:
 
     Uplink (command) data:
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/communication/ground.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/communication/ground.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/communication/updown.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/communication/updown.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/data_types/ch_data.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/ch_data.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/data_types/cmd_data.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/cmd_data.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/data_types/event_data.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/event_data.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/data_types/exceptions.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/exceptions.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/data_types/file_data.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/file_data.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/data_types/pkt_data.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/pkt_data.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/data_types/sys_data.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/data_types/sys_data.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/decoders/ch_decoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/ch_decoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/decoders/decoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/decoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/decoders/event_decoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/event_decoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/decoders/file_decoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/file_decoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/decoders/pkt_decoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/decoders/pkt_decoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/distributor/distributor.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/distributor/distributor.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/encoders/ch_encoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/ch_encoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/encoders/cmd_encoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/cmd_encoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/encoders/encoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/encoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/encoders/event_encoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/event_encoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/encoders/file_encoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/file_encoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/encoders/pkt_encoder.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/pkt_encoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/encoders/seq_writer.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/encoders/seq_writer.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/files/File Decoder Documentation.txt` & `fprime-gds-3.4.4a1/src/fprime_gds/common/files/File Decoder Documentation.txt`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/files/downlinker.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/files/downlinker.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/files/helpers.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/files/helpers.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/files/uplinker.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/files/uplinker.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/base_commands.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/base_commands.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/channels.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/channels.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/command_send.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/command_send.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/events.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/events.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/filtering_utils.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/filtering_utils.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/gds_cli/test_api_utils.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/gds_cli/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/handlers.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/handlers.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/history/chrono.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/history/chrono.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/history/history.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/history/history.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/history/ram.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/history/ram.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/history/test.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/history/test.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/ch_py_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/ch_py_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/ch_xml_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/ch_xml_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/cmd_py_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/cmd_py_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/cmd_xml_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/cmd_xml_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/dict_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/dict_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/event_py_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/event_py_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/event_xml_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/event_xml_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/pkt_xml_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/pkt_xml_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/python_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/python_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/loaders/xml_loader.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/loaders/xml_loader.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/logger/__init__.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/logger/data_logger.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/logger/data_logger.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/logger/test_logger.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/logger/test_logger.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/models/common/channel_telemetry.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/models/common/channel_telemetry.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/models/common/command.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/models/common/command.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/models/common/event.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/models/common/event.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/parsers/seq_file_parser.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/parsers/seq_file_parser.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/pipeline/dictionaries.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/dictionaries.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/pipeline/encoding.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/encoding.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/pipeline/files.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/files.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/pipeline/histories.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/histories.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/pipeline/router.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/router.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/pipeline/standard.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/pipeline/standard.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/templates/ch_template.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/templates/ch_template.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/templates/cmd_template.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/templates/cmd_template.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/templates/data_template.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/templates/data_template.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/templates/event_template.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/templates/event_template.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/templates/pkt_template.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/templates/pkt_template.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/testing_fw/api.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/testing_fw/api.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/testing_fw/predicates.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/testing_fw/predicates.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/testing_fw/pytest_integration.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/testing_fw/pytest_integration.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/tools/seqgen.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/tools/seqgen.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/transport.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/transport.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/utils/config_manager.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/utils/data_desc_type.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/utils/data_desc_type.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/utils/string_util.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/common/zmq_transport.py` & `fprime-gds-3.4.4a1/src/fprime_gds/common/zmq_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 1. ZeroMQ is performant and can move 1GB/s/thread
 2. ZeroMQ does not require a separate process and may be used w/o tcp sockets
 3. ZeroMQ will not reorder packets at high data rates
 
 @author lestarch
 """
+
 import logging
 import struct
 from typing import Tuple
 
 import zmq
 
 from fprime_gds.common.communication.ground import GroundHandler
@@ -20,14 +21,15 @@
     RoutingTag,
     ThreadedTransportClient,
     TransportationException,
 )
 
 LOGGER = logging.getLogger("transport")
 
+
 class ZmqWrapper(object):
     """Handler for ZMQ functions for use in other objects"""
 
     def __init__(self):
         """Initialize the ZMQ setup"""
         super().__init__()
         self.context = zmq.Context()
@@ -46,15 +48,17 @@
         the creation of the sockets until the threads exist.
 
         Args:
             transport_url: url of the ZeroMQ network to connect to
             sub_topic: subscription topic used to filter incoming messages
             pub_topic: publication topic supplied for remote subscription filters
         """
-        assert len(transport_url) == 2, f"Must supply a pair of URLs for ZeroMQ not '{transport_url}'"
+        assert (
+            len(transport_url) == 2
+        ), f"Must supply a pair of URLs for ZeroMQ not '{transport_url}'"
         self.pub_topic = pub_topic
         self.sub_topic = sub_topic
         self.transport_url = transport_url
 
     def make_server(self):
         """Makes this wrapper a server
 
@@ -74,40 +78,48 @@
         system. This will connect the ZeroMQ topology and if self.server is set, will bind the outgoing port rather than
         connect it such that this wrapper will act as a host. This only affects outgoing connections as sockets must be
         created on their owning threads.
 
         The connection is made using self.transport_url, and as such, this must be configured before running. This is
         intended to be called on the sending thread.
         """
-        assert self.transport_url is not None and len(self.transport_url) == 2, "Must configure before connecting"
-        assert self.zmq_socket_outgoing is None, "Cannot connect outgoing multiple times"
+        assert (
+            self.transport_url is not None and len(self.transport_url) == 2
+        ), "Must configure before connecting"
+        assert (
+            self.zmq_socket_outgoing is None
+        ), "Cannot connect outgoing multiple times"
         assert self.pub_topic is not None, "Must configure sockets before connecting"
         self.zmq_socket_outgoing = self.context.socket(zmq.PUB)
         self.zmq_socket_outgoing.setsockopt(zmq.SNDHWM, 0)
         # When set to bind sockets, connect via a bind call
         if self.server:
             server_transport = self.transport_url[1].replace("localhost", "127.0.0.1")
             LOGGER.info("Outgoing binding to: %s", (server_transport))
             self.zmq_socket_outgoing.bind(server_transport)
         else:
             LOGGER.info("Outgoing connecting to: %s", (self.transport_url[0]))
             self.zmq_socket_outgoing.connect(self.transport_url[0])
 
     def connect_incoming(self):
-        """ Sets up a ZeroMQ connection for incoming data
+        """Sets up a ZeroMQ connection for incoming data
 
         ZeroMQ allows multiple connections to a single endpoint. This only affects incoming connections as sockets must
         be created on their owning threads. This will connect the ZeroMQ topology and if self.server is set, will bind
         the incoming port rather than connect it such that this wrapper will act as a host.
 
         The connection is made using self.transport_url, and as such, this must be configured before running. This is
         intended to be called on the receiving thread.
         """
-        assert self.transport_url is not None and len(self.transport_url) == 2, "Must configure before connecting"
-        assert self.zmq_socket_incoming is None, "Cannot connect incoming multiple times"
+        assert (
+            self.transport_url is not None and len(self.transport_url) == 2
+        ), "Must configure before connecting"
+        assert (
+            self.zmq_socket_incoming is None
+        ), "Cannot connect incoming multiple times"
         assert self.sub_topic is not None, "Must configure sockets before connecting"
         self.zmq_socket_incoming = self.context.socket(zmq.SUB)
         self.zmq_socket_incoming.setsockopt(zmq.RCVHWM, 0)
         self.zmq_socket_incoming.setsockopt(zmq.SUBSCRIBE, self.sub_topic)
         if self.server:
             server_transport = self.transport_url[0].replace("localhost", "127.0.0.1")
             LOGGER.info("Incoming binding to: %s", (server_transport))
@@ -121,15 +133,15 @@
         self.zmq_socket_outgoing.close()
 
     def disconnect_incoming(self):
         """Disconnect the ZeroMQ sockets"""
         self.zmq_socket_incoming.close()
 
     def terminate(self):
-        """ Terminate the ZeroMQ context"""
+        """Terminate the ZeroMQ context"""
         self.context.term()
 
     def recv(self, timeout=None):
         """Receive single packet from ZMQ"""
         try:
             self.zmq_socket_incoming.setsockopt(
                 zmq.RCVTIMEO, timeout if timeout is not None else -1
@@ -158,38 +170,43 @@
 
     def __init__(self):
         """Create ZMQ wrapper"""
         super().__init__()
         self.zmq = ZmqWrapper()
 
     def connect(
-        self, transport_url: Tuple[str], sub_routing: RoutingTag, pub_routing: RoutingTag
+        self,
+        transport_url: Tuple[str],
+        sub_routing: RoutingTag,
+        pub_routing: RoutingTag,
     ):
         """Connects to the ZeroMQ network"""
         self.zmq.configure(transport_url, sub_routing.value, pub_routing.value)
-        self.zmq.connect_outgoing() # Outgoing socket, for clients, exists on the current thread
+        self.zmq.connect_outgoing()  # Outgoing socket, for clients, exists on the current thread
         super().connect(transport_url, sub_routing, pub_routing)
 
     def disconnect(self):
         """Disconnects from ZeroMQ network"""
         self.zmq.disconnect_outgoing()  # Outgoing is on the current thread
         super().disconnect()
 
     def send(self, data):
         """Send data via ZeroMQ"""
-        if data[:4] == b'ZZZZ':
+        if data[:4] == b"ZZZZ":
             data = data[4:]
-        self.zmq.send(data)  # Must strip out ZZZZ as that is a ThreadedTcpServer only property
+        self.zmq.send(
+            data
+        )  # Must strip out ZZZZ as that is a ThreadedTcpServer only property
 
     def recv(self, timeout=None):
         """Receives data from ZeroMQ"""
         return self.zmq.recv(timeout)
 
     def recv_thread(self):
-        """ Overrides the recv_thread method
+        """Overrides the recv_thread method
 
         Overrides the recv_thread method of the superclass such that the ZeroMQ socket may be created/destroyed
         before/after the main recv loop.
         """
         self.zmq.connect_incoming()
         super().recv_thread()  # Contains a while <event> loop, will only return at end of program
         self.zmq.disconnect_incoming()
@@ -199,28 +216,30 @@
 class ZmqGround(GroundHandler):
     """Ground handler implementation for using ZeroMQ as the transport
 
     This ground handler is built upon the ZmqWrapper subclass an uses zero mq to send data from the communications layer
     to the display and processing layer(s). This effectively acts as the "FSW" side of that interface as it
     frames/deframes packets heading to that layer.
 
-    Since there is likely only one communications client to the FSW users should call make_server() after construction
+    Since there is likely only one communications client to the FSW users should instantiate with server=True
     to ensure that it binds to resources for the network. This is not forced in case of multiple FSW connections.
     """
 
-    def __init__(self, transport_url):
+    def __init__(self, transport_url, server=True):
         """Initialize this interface with the transport_url needed to connect
 
         Args:
             transport_url: transport url passed into the zeromq connection
         """
         super().__init__()
         self.zmq = ZmqWrapper()
         self.transport_url = transport_url
         self.timeout = 10
+        if server:
+            self.zmq.make_server()
 
     def open(self):
         """Open this ground interface. Delegates to the connect method
 
         Opens any needed resources and prepares the system for receiving and sending. This means opening the ZeroMQ
         network and setting up routing to incoming as FSW and outgoing to GUI.
 
@@ -238,18 +257,14 @@
     def close(self):
         """Closes the open adapter"""
         # Don't know what else to do, the governing threads are dead, so attempt to close?
         self.zmq.disconnect_incoming()
         self.zmq.disconnect_outgoing()
         self.zmq.terminate()
 
-    def make_server(self):
-        """Makes it into a server"""
-        self.zmq.make_server()
-
     def receive_all(self):
         """Receive all available packets
 
         Receive all packet available from the ground layer. This will return full ground packets up to the uplinker.
         These packets should be fully-deframed and ready for reframing in the comm-layer specified format. With ZeroMQ
         handling whole messages, there is never any outstanding data.
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds/executables/cli.py` & `fprime-gds-3.4.4a1/src/fprime_gds/executables/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This file sets up the command line interface and argument parsing that is done to support the F prime executable tools
 layer. It is designed to allow users to import standard sets of arguments that applied to the various aspects of the
 code that they are importing.
 
 @author mstarch
 """
+
 import argparse
 import datetime
 import errno
 import getpass
 import itertools
 import os
 import platform
@@ -19,20 +20,21 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Dict, List, Tuple
 
 # Required to set the checksum as a module variable
 import fprime_gds.common.communication.checksum
 import fprime_gds.common.logger
-from fprime_gds.common.communication.adapters.base import BaseAdapter
 from fprime_gds.common.communication.adapters.ip import check_port
 from fprime_gds.common.pipeline.standard import StandardPipeline
 from fprime_gds.common.transport import ThreadedTCPSocketClient
 from fprime_gds.common.utils.config_manager import ConfigManager
 from fprime_gds.executables.utils import find_app, find_dict, get_artifacts_root
+from fprime_gds.plugin.definitions import PluginType
+from fprime_gds.plugin.system import Plugins
 
 # Optional import: ZeroMQ. Requires package: pyzmq
 try:
     import zmq
 
     from fprime_gds.common.zmq_transport import ZmqClient
 except ImportError:
@@ -41,15 +43,14 @@
 
 # Optional import: Serial Adapter. Requires package: SerialAdapter
 try:
     from fprime_gds.common.communication.adapters.uart import SerialAdapter
 except ImportError:
     SerialAdapter = None
 
-
 GUIS = ["none", "html"]
 
 
 class ParserBase(ABC):
     """Base parser for handling fprime command lines
 
     Parsers must define several functions. They must define "get_parser", which will produce a parser to parse the
@@ -81,19 +82,39 @@
 
         Produce a parser that will handle the given arguments. These parsers can be combined for a CLI for a tool by
         assembling them as parent processors to a parser for the given tool.
 
         Return:
             argparse parser for supplied arguments
         """
-        parser = argparse.ArgumentParser(description=self.description, add_help=True)
-        for flags, keywords in self.get_arguments().items():
-            parser.add_argument(*flags, **keywords)
+        parser = argparse.ArgumentParser(
+            description=self.description,
+            add_help=True,
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        )
+        self.fill_parser(parser)
         return parser
 
+    def fill_parser(self, parser):
+        """ Fill supplied parser with arguments
+
+        Fills the supplied parser with the arguments returned via the `get_arguments` method invocation. This
+        implementation add the arguments directly to the parser.
+
+        Args:
+            parser: parser to fill with arguments
+
+        """
+        for flags, keywords in self.get_arguments().items():
+            try:
+                parser.add_argument(*flags, **keywords)
+            except argparse.ArgumentError:
+                # flag has already been added, pass
+                pass
+
     def reproduce_cli_args(self, args_ns):
         """Reproduce the list of arguments needed on the command line"""
 
         def flag_member(flags, argparse_inputs) -> Tuple[str, str]:
             """Get the best CLI flag and namespace member"""
             best_flag = (
                 [flag for flag in flags if flag.startswith("--")] + list(flags)
@@ -172,14 +193,15 @@
             args_ns = composition.handle_arguments(args_ns, **kwargs)
         except ValueError as ver:
             print(f"[ERROR] Failed to parse arguments: {ver}", file=sys.stderr)
             parser.print_help()
             sys.exit(-1)
         except Exception as exc:
             print(f"[ERROR] {exc}", file=sys.stderr)
+            raise
             sys.exit(-1)
         return args_ns, parser
 
     @staticmethod
     def find_in(token, deploy, is_file=True):
         """
         Find token in deploy directory by walking the directory looking for reg-ex. This effectively finds a file in a
@@ -241,27 +263,199 @@
         elif len(child_directories) > 1:
             msg = f"Multiple deployments found in {detected_toolchain}. Choose using: --deployment"
             raise Exception(msg)
         args.deployment = child_directories[0]
         return args
 
 
+class PluginArgumentParser(ParserBase):
+    """Parser for arguments coming from plugins"""
+
+    DESCRIPTION = "Plugin options"
+    FPRIME_CHOICES = {
+        "framing": "fprime",
+        "communication": "ip",
+    }
+
+    def __init__(self):
+        """Initialize the plugin information for this parser"""
+        self._plugin_map = {
+            category: Plugins.system().get_plugins(category)
+            for category in Plugins.system().get_categories()
+        }
+
+    @staticmethod
+    def safe_add_argument(parser, *flags, **keywords):
+        """ Add an argument allowing duplicates
+
+        Add arguments to the parser (passes through *flags and **keywords) to the supplied parser. This method traps
+        errors to prevent duplicates.
+
+        Args:
+            parser: parser or argument group to add arguments to
+            *flags: positional arguments passed to `add_argument`
+            **keywords: key word arguments passed to `add_argument`
+        """
+        try:
+            parser.add_argument(*flags, **keywords)
+        except argparse.ArgumentError:
+            # flag has already been added, pass
+            pass
+
+    def fill_parser(self, parser):
+        """ File supplied parser with grouped arguments
+
+        Fill the supplied parser with arguments from the `get_arguments` method invocation. This implementation groups
+        arguments based on the constituent that sources the argument.
+
+        Args:
+            parser: parser to fill
+        """
+        for category, plugins in self._plugin_map.items():
+            argument_group = parser.add_argument_group(title=f"{category.title()} Plugin Options")
+            for flags, keywords in self.get_category_arguments(category).items():
+                self.safe_add_argument(argument_group, *flags, **keywords)
+
+            for plugin in plugins:
+                argument_group = parser.add_argument_group(title=f"{category.title()} Plugin '{plugin.get_name()}' Options")
+                if plugin.type == PluginType.FEATURE:
+                    self.safe_add_argument(argument_group,
+                                           f"--disable-{plugin.get_name()}",
+                                           action="store_true",
+                                           default=False,
+                                           help=f"Disable the {category} plugin '{plugin.get_name()}'")
+                for flags, keywords in plugin.get_arguments().items():
+                    self.safe_add_argument(argument_group, *flags, **keywords)
+
+    def get_category_arguments(self, category):
+        """ Get arguments for a plugin category """
+        arguments: Dict[Tuple[str, ...], Dict[str, Any]] = {}
+        plugins = self._plugin_map[category]
+        # Add category options: SELECTION plugins add a selection flag
+        plugin_type = Plugins.get_category_plugin_type(category)
+        if plugin_type == PluginType.SELECTION:
+            arguments.update(
+                {
+                    (f"--{category}-selection",): {
+                        "choices": [choice.get_name() for choice in plugins],
+                        "help": f"Select {category} implementer.",
+                        "default": self.FPRIME_CHOICES.get(
+                            category, list(plugins)[0].get_name()
+                        ),
+                    }
+                }
+            )
+        return arguments
+
+    def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
+        """Return arguments to used in plugins"""
+        arguments: Dict[Tuple[str, ...], Dict[str, Any]] = {}
+        for category, plugins in self._plugin_map.items():
+            arguments.update(self.get_category_arguments(category))
+            for plugin in plugins:
+                # Add disable flags for feature type plugins
+                if plugin.type == PluginType.FEATURE:
+                    arguments.update({
+                        (f"--disable-{plugin.get_name()}", ): {
+                            "action": "store_true",
+                            "default": False,
+                            "help": f"Disable the {category} plugin '{plugin.get_name()}'"
+                        }
+                    })
+                arguments.update(plugin.get_arguments())
+        return arguments
+
+    def handle_arguments(self, args, **kwargs):
+        """Handles the arguments"""
+        for category, plugins in self._plugin_map.items():
+            plugin_type = Plugins.get_category_plugin_type(category)
+
+            # Selection plugins choose one plugin and instantiate it
+            if plugin_type == PluginType.SELECTION:
+                selection_string = getattr(args, f"{category}_selection")
+                matching_plugins = [plugin for plugin in plugins if plugin.get_name() == selection_string]
+                assert len(matching_plugins) == 1, "Plugin selection system failed"
+                selection_class = matching_plugins[0].plugin_class
+                filled_arguments = self.extract_plugin_arguments(args, selection_class)
+                selection_instance = selection_class(**filled_arguments)
+                setattr(args, f"{category}_selection_instance", selection_instance)
+            # Feature plugins instantiate all enabled plugins
+            elif plugin_type == PluginType.FEATURE:
+                enabled_plugins = [
+                    plugin for plugin in plugins
+                    if not getattr(args, f"disable_{plugin.get_name().replace('-', '_')}", False)
+                ]
+                plugin_instantiations = [
+                    plugin.plugin_class(**self.extract_plugin_arguments(args, plugin))
+                    for plugin in enabled_plugins
+                ]
+                setattr(args, f"{category}_enabled_instances", plugin_instantiations)
+        return args
+
+    @staticmethod
+    def extract_plugin_arguments(args, plugin) -> Dict[str, Any]:
+        """Extract plugin argument values from the args namespace into a map
+
+        Plugin arguments will be supplied to the `__init__` function of the plugin via a keyword argument dictionary.
+        This function maps from the argument namespace from parsing back into that dictionary.
+
+        Args:
+            args: argument namespace from argparse
+            plugin: plugin to extract arguments for
+        Return:
+            filled arguments dictionary
+        """
+        expected_args = plugin.get_arguments()
+        argument_destinations = [
+            (
+                value["dest"]
+                if "dest" in value
+                else key[0].replace("--", "").replace("-", "_")
+            )
+            for key, value in expected_args.items()
+        ]
+        filled_arguments = {
+            destination: getattr(args, destination)
+            for destination in argument_destinations
+        }
+        # Check arguments or yield a Value error
+        if hasattr(plugin, "check_arguments"):
+            plugin.check_arguments(**filled_arguments)
+        return filled_arguments
+
+
 class CompositeParser(ParserBase):
     """Composite parser handles parsing as a composition of multiple other parsers"""
 
     def __init__(self, constituents, description=None):
         """Construct this parser by instantiating the sub-parsers"""
         self.given = description
         constructed = [constituent() for constituent in constituents]
         flattened = [
             item.constituents if isinstance(item, CompositeParser) else [item]
             for item in constructed
         ]
         self.constituent_parsers = {*itertools.chain.from_iterable(flattened)}
 
+    def fill_parser(self, parser):
+        """ File supplied parser with grouped arguments
+
+        Fill the supplied parser with arguments from the `get_arguments` method invocation. This implementation groups
+        arguments based on the constituent that sources the argument.
+
+        Args:
+            parser: parser to fill
+        """
+        for constituent in sorted(self.constituents, key=lambda x: x.description):
+            if isinstance(constituent, (PluginArgumentParser, CompositeParser)):
+                constituent.fill_parser(parser)
+            else:
+                argument_group = parser.add_argument_group(title=constituent.description)
+                constituent.fill_parser(argument_group)
+
     @property
     def constituents(self):
         """Get constituent"""
         return self.constituent_parsers
 
     @property
     def description(self):
@@ -282,89 +476,46 @@
     def handle_arguments(self, args, **kwargs):
         """Process all constituent arguments"""
         for constituent in self.constituents:
             args = constituent.handle_arguments(args, **kwargs)
         return args
 
 
-class CommAdapterParser(ParserBase):
-    """
-    Handles parsing of all of the comm-layer arguments. This means selecting a comm adapter, and passing the arguments
-    required to setup that comm adapter. In addition, this parser uses the import parser to import modules such that a
-    user may import other adapter implementation files.
-    """
+class CommExtraParser(ParserBase):
+    """Parses extra communication arguments"""
 
-    DESCRIPTION = "Process arguments needed to specify a comm-adapter"
+    DESCRIPTION = "Communications options"
 
     def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
         """Get arguments for the comm-layer parser"""
-        adapter_definition_dictionaries = BaseAdapter.get_adapters()
-        adapter_arguments = {}
-        for name, adapter in adapter_definition_dictionaries.items():
-            adapter_arguments_callable = getattr(adapter, "get_arguments", None)
-            if not callable(adapter_arguments_callable):
-                print(
-                    f"[WARNING] '{name}' does not have 'get_arguments' method, skipping.",
-                    file=sys.stderr,
-                )
-                continue
-            adapter_arguments.update(adapter.get_arguments())
         com_arguments = {
-            ("--comm-adapter",): {
-                "dest": "adapter",
-                "action": "store",
-                "type": str,
-                "help": "Adapter for communicating to flight deployment. [default: %(default)s]",
-                "choices": ["none"] + list(adapter_definition_dictionaries),
-                "default": "ip",
-            },
-            ("--comm-checksum-type",): {
-                "dest": "checksum_type",
-                "action": "store",
-                "type": str,
-                "help": "Setup the checksum algorithm. [default: %(default)s]",
-                "choices": [
-                    item
-                    for item in fprime_gds.common.communication.checksum.CHECKSUM_MAPPING.keys()
-                    if item != "default"
-                ],
-                "default": fprime_gds.common.communication.checksum.CHECKSUM_SELECTION,
-            },
             ("--output-unframed-data",): {
                 "dest": "output_unframed_data",
                 "action": "store",
                 "nargs": "?",
                 "help": "Log unframed data to supplied file relative to log directory. Use '-' for standard out.",
                 "default": None,
                 "const": "unframed.log",
                 "required": False,
             },
         }
-        return {**adapter_arguments, **com_arguments}
+        return com_arguments
 
     def handle_arguments(self, args, **kwargs):
-        """
-        Handle the input arguments for the parser. This will help setup the adapter with its expected arguments.
-
-        :param args: parsed arguments in namespace format
-        :return: namespace with "comm_adapter" value added
-        """
-        args.comm_adapter = BaseAdapter.construct_adapter(args.adapter, args)
-        fprime_gds.common.communication.checksum.CHECKSUM_SELECTION = args.checksum_type
         return args
 
 
 class LogDeployParser(ParserBase):
     """
     A parser that handles log files by reading in a '--logs' directory or a '--deploy' directory to put the logs into
     as a default. This is useful as a parsing fragment for any application that produces log files and needs these logs
     to end up in the proper place.
     """
 
-    DESCRIPTION = "Process arguments needed to specify a logging"
+    DESCRIPTION = "Logging options"
 
     def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
         """Return arguments to parse logging options"""
         return {
             ("-l", "--logs"): {
                 "dest": "logs",
                 "action": "store",
@@ -419,34 +570,28 @@
     """
     Middleware (ThreadedTcpServer, ZMQ) interface that looks for an address and a port. The argument handling will
     attempt to connect to the socket to ensure that it is a valid address/port and report any errors. This is then
     immediately closes the port after use. There is a minor race-condition between this check and the actual usage,
     however; it should be close enough.
     """
 
-    DESCRIPTION = "Process arguments needed to specify a tool using the middleware"
+    DESCRIPTION = "Middleware options"
 
     def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
         """Return arguments necessary to run a and connect to the GDS middleware"""
         # May use ZMQ transportation layer if zmq package is available
         zmq_arguments = {}
         if zmq is not None and ZmqClient is not None:
             zmq_arguments = {
                 ("--zmq",): {
                     "dest": "zmq",
                     "action": "store_true",
                     "help": "Switch to using the ZMQ transportation layer",
                     "default": False,
                 },
-                ("--zmq-server",): {
-                    "dest": "zmq_server",
-                    "action": "store_true",
-                    "help": "Sets the ZMQ connection to be a server. Default: false (client)",
-                    "default": False,
-                },
                 ("--zmq-transport",): {
                     "dest": "zmq_transport",
                     "nargs": 2,
                     "help": "Pair of URls used with --zmq to setup ZeroMQ transportation [default: %(default)s]",
                     "default": [
                         "ipc:///tmp/fprime-server-in",
                         "ipc:///tmp/fprime-server-out",
@@ -497,14 +642,16 @@
             check_port(args.tts_addr, args.tts_port)
         return args
 
 
 class DictionaryParser(DetectionParser):
     """Parser for deployments"""
 
+    DESCRIPTION = "Dictionary options"
+
     def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
         """Arguments to handle deployments"""
         return {
             **super().get_arguments(),
             **{
                 ("--dictionary",): {
                     "dest": "dictionary",
@@ -536,14 +683,16 @@
             args.dictionary = find_dict(args.deployment)
         return args
 
 
 class FileHandlingParser(ParserBase):
     """Parser for deployments"""
 
+    DESCRIPTION = "File handling options"
+
     def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
         """Arguments to handle deployments"""
 
         username = getpass.getuser()
 
         return {
             ("--file-storage-directory",): {
@@ -614,15 +763,20 @@
                 raise
         return pipeline
 
 
 class CommParser(CompositeParser):
     """Comm Executable Parser"""
 
-    CONSTITUENTS = [CommAdapterParser, MiddleWareParser, LogDeployParser]
+    CONSTITUENTS = [
+        CommExtraParser,
+        MiddleWareParser,
+        LogDeployParser,
+        PluginArgumentParser,
+    ]
 
     def __init__(self):
         """Initialization"""
         super().__init__(
             constituents=self.CONSTITUENTS,
             description="Communications bridge application",
         )
@@ -635,15 +789,15 @@
     - dictionary: path to dictionary, either a folder for py_dicts, or a file for XML dicts
     - logs: path to logging path
     - config: configuration for GDS.
 
     Note: deployment can help in setting both dictionary and logs, but isn't strictly required.
     """
 
-    DESCRIPTION = "Process arguments needed to specify a tool using the GDS"
+    DESCRIPTION = "GUI options"
 
     def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
         """Return arguments necessary to run a binary deployment via the GDS"""
         return {
             ("-g", "--gui"): {
                 "choices": GUIS,
                 "dest": "gui",
@@ -682,15 +836,15 @@
 
 class BinaryDeployment(DetectionParser):
     """
     Parsing subclass used to read the arguments of the binary application. This derives functionality from a comm parser
     and represents the flight-side of the equation.
     """
 
-    DESCRIPTION = "Process arguments needed for running F prime binary"
+    DESCRIPTION = "FPrime binary options"
 
     def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
         """Return arguments necessary to run a binary deployment via the GDS"""
         return {
             **super().get_arguments(),
             **{
                 ("-n", "--no-app"): {
@@ -728,15 +882,15 @@
         return args
 
 
 class SearchArgumentsParser(ParserBase):
     """Parser for search arguments"""
 
     DESCRIPTION = (
-        "Process arguments relevant to searching/filtering Channels/Events/Commands"
+        "Searching and filtering options"
     )
 
     def __init__(self, command_name: str) -> None:
         self.command_name = command_name
 
     def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
         """Return arguments necessary to search through channels/events/commands"""
@@ -774,15 +928,15 @@
     def handle_arguments(self, args, **kwargs):
         return args
 
 
 class RetrievalArgumentsParser(ParserBase):
     """Parser for retrieval arguments"""
 
-    DESCRIPTION = "Process arguments relevant to retrieving Channels/Events"
+    DESCRIPTION = "Data retrieval options"
 
     def __init__(self, command_name: str) -> None:
         self.command_name = command_name
 
     def get_arguments(self) -> Dict[Tuple[str, ...], Dict[str, Any]]:
         """Return arguments to retrieve channels/events/commands in specific ways"""
         return {
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds/executables/comm.py` & `fprime-gds-3.4.4a1/src/fprime_gds/executables/comm.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,33 +12,30 @@
 
 Note: assuming the module containing the ground adapter has been imported, then this code should provide it as a CLI
       argument, removing the need to rewrite most of this class to use something different.
 
 @author lestarch
 """
 
-
 import logging
 import signal
 import sys
 
 from pathlib import Path
 
 # Required adapters built on standard tools
 try:
     from fprime_gds.common.zmq_transport import ZmqGround
 except ImportError:
     ZmqGround = None
 import fprime_gds.common.communication.adapters.base
 import fprime_gds.common.communication.adapters.ip
-import fprime_gds.common.communication.checksum
 import fprime_gds.common.communication.ground
 import fprime_gds.common.logger
 import fprime_gds.executables.cli
-from fprime_gds.common.communication.framing import FpFramerDeframer
 from fprime_gds.common.communication.updown import Downlinker, Uplinker
 
 # Uses non-standard PIP package pyserial, so test the waters before getting a hard-import crash
 try:
     import fprime_gds.common.communication.adapters.uart
 except ImportError:
     pass
@@ -54,46 +51,46 @@
     :return: return code
     """
     args, _ = fprime_gds.executables.cli.ParserBase.parse_args(
         [
             fprime_gds.executables.cli.LogDeployParser,
             fprime_gds.executables.cli.MiddleWareParser,
             fprime_gds.executables.cli.CommParser,
+            fprime_gds.executables.cli.PluginArgumentParser,
         ],
         description="F prime communications layer.",
         client=True,
     )
-    fprime_gds.common.communication.checksum = args.checksum_type
-    if args.comm_adapter == "none":
-        print("[ERROR] Comm adapter set to 'none'. Nothing to do but exit.", file=sys.stderr)
+    if args.communication_selection == "none":
+        print(
+            "[ERROR] Comm adapter set to 'none'. Nothing to do but exit.",
+            file=sys.stderr,
+        )
         sys.exit(-1)
 
     # Create the handling components for either side of this script, adapter for hardware, and ground for the GDS side
     if args.zmq and ZmqGround is None:
         print("[ERROR] ZeroMQ is not available. Install pyzmq.", file=sys.stderr)
         sys.exit(-1)
     elif args.zmq:
         ground = fprime_gds.common.zmq_transport.ZmqGround(args.zmq_transport)
-        # Check for need to make this a server
-        if args.zmq_server:
-            ground.make_server()
     else:
         ground = fprime_gds.common.communication.ground.TCPGround(
             args.tts_addr, args.tts_port
         )
 
-    adapter = args.comm_adapter
+    adapter = args.communication_selection_instance
 
     # Set the framing class used and pass it to the uplink and downlink component constructions giving each a separate
     # instantiation
-    framer_class = FpFramerDeframer
+    framer_instance = args.framing_selection_instance
     LOGGER.info(
         "Starting uplinker/downlinker connecting to FSW using %s with %s",
-        adapter,
-        framer_class.__name__,
+        args.communication_selection,
+        args.framing_selection,
     )
     discarded_file_handle = None
     try:
         if args.output_unframed_data == "-":
             discarded_file_handle = sys.stdout.buffer
         elif args.output_unframed_data is not None:
             discarded_file_handle_path = (
@@ -104,29 +101,29 @@
                 LOGGER.info("Logging unframed data to %s", discarded_file_handle_path)
             except OSError:
                 LOGGER.warning(
                     "Failed to open %s. Unframed data will be discarded.",
                     discarded_file_handle_path,
                 )
         downlinker = Downlinker(
-            adapter, ground, framer_class(), discarded=discarded_file_handle
+            adapter, ground, framer_instance, discarded=discarded_file_handle
         )
-        uplinker = Uplinker(adapter, ground, framer_class(), downlinker)
+        uplinker = Uplinker(adapter, ground, framer_instance, downlinker)
 
         # Open resources for the handlers on either side, this prepares the resources needed for reading/writing data
         ground.open()
         adapter.open()
 
         # Finally start the processing of uplink and downlink
         downlinker.start()
         uplinker.start()
         LOGGER.debug("Uplinker and downlinker running")
 
-        # Wait for shutdown event in the form of a KeyboardInterrupt then stop the processing, close resources, and wait for
-        # everything to terminate as expected.
+        # Wait for shutdown event in the form of a KeyboardInterrupt then stop the processing, close resources,
+        # and wait for everything to terminate as expected.
         def shutdown(*_):
             """Shutdown function for signals"""
             uplinker.stop()
             downlinker.stop()
             uplinker.join()
             downlinker.join()
             ground.close()
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds/executables/fprime_cli.py` & `fprime-gds-3.4.4a1/src/fprime_gds/executables/fprime_cli.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/executables/tcpserver.py` & `fprime-gds-3.4.4a1/src/fprime_gds/executables/tcpserver.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/executables/utils.py` & `fprime-gds-3.4.4a1/src/fprime_gds/executables/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             arguments, stdout=file_handler, stderr=subprocess.STDOUT, env=env
         )
         register_process_assassin(child, file_handler)
         # If launch time is specified, then wait for it to be stable
         if launch_time is not None:
             time.sleep(launch_time)
             child.poll()
-            if child.returncode is not None:
+            if child.returncode is not None and child.returncode != 0:
                 raise ProcessNotStableException(
                     arguments[0], child.returncode, launch_time
                 )
         return child
     except Exception as exc:
         msg = f"Failed to run application: {' '.join(arguments)}. Error: {exc}"
         raise AppWrapperException(msg)
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/app.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/app.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/channels.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/channels.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/commands.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/commands.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/components.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/components.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/default_settings.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/default_settings.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/errors.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/errors.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/events.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/events.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/json.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/json.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/logs.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/logs.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/resource.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/resource.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/sequence.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/sequence.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/advanced-settings/addon-templates.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/advanced-settings/addon-templates.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/advanced-settings/addon.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/advanced-settings/addon.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/channel-render/channel-render-template.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/channel-render/channel-render-template.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/channel-render/channel-render.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/channel-render/channel-render.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/addon-templates.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/addon-templates.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/addon.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/addon.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/config.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/config.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-streaming.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-streaming.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-zoom.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/chartjs-plugin-zoom.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/flat.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/modified-vendor/flat.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/sibling.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/sibling.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/vendor/chart.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/vendor/chart.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/vendor/chartjs-adapter-luxon.min.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/vendor/chartjs-adapter-luxon.min.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/chart-display/vendor/hammer.min.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/chart-display/vendor/hammer.min.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/argument-templates.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/argument-templates.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/arguments.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/arguments.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-history-template.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-history-template.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-history.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-history.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-input-template.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-input-template.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-input.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-input.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-string-template.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-string-template.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/commanding/command-string.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/commanding/command-string.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/dictionary/addon-templates.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/dictionary/addon-templates.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/dictionary/addon.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/dictionary/addon.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/image-display/addon.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/image-display/addon.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/README.md` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/README.md`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/addon-templates.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/addon-templates.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/addon.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/addon.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/autocomplete.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/autocomplete.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/lint.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/lint.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/code-mirror.es.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/code-mirror.es.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/rollup/index.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/index.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/rollup/language.grammer` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/language.grammer`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/addons/sequencer/third/rollup/package.json` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/addons/sequencer/third/rollup/package.json`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/css/fprime.css` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/css/fprime.css`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/css/fpstyle.css` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/css/fpstyle.css`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/favicon.ico` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/img/error.svg` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/img/error.svg`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/img/logo.svg` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/img/success.svg` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/img/success.svg`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/index.html` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/index.html`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/config.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/config.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/datastore.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/datastore.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/gds.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/gds.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/loader.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/loader.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/performance.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/performance.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/settings.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/settings.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/uploader.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/uploader.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/validate.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/validate.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/channel.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/channel.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/dashboard-box.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/dashboard-box.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/dashboard.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/dashboard.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/downlink.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/downlink.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/event.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/event.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/fp-row.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/fp-row.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/fptable.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/fptable.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/log.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/log.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/tabetc.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/tabetc.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/uplink.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/uplink.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/js/vue-support/utils.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/js/vue-support/utils.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/css/all.min.css` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/css/all.min.css`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/css/bootstrap.min.css` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/css/vue-select.css` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/css/vue-select.css`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/luxon.min.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/luxon.min.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/sorttable.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/sorttable.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/v-runtime-template.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/v-runtime-template.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/vue-select.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/vue-select.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/js/vue.min.js` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/js/vue.min.js`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.eot` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.svg` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.ttf` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff2` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.eot` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.svg` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.ttf` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff2` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.eot` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.svg` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.ttf` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff2` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/stats.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/stats.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds/flask/updown.py` & `fprime-gds-3.4.4a1/src/fprime_gds/flask/updown.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/src/fprime_gds.egg-info/PKG-INFO` & `fprime-gds-3.4.4a1/src/fprime_gds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime-gds
-Version: 3.4.3
+Version: 3.4.4a1
 Summary: F Prime Flight Software Ground Data System layer
 Author-email: Michael Starch <Michael.D.Starch@jpl.nasa.gov>, Thomas Boyer-Chammard <Thomas.Boyer.Chammard@jpl.nasa.gov>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `fprime-gds-3.4.3/src/fprime_gds.egg-info/SOURCES.txt` & `fprime-gds-3.4.4a1/src/fprime_gds.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitignore
 Doxyfile
 LICENSE.txt
 NOTICE.txt
 README.md
 pyproject.toml
-pytest.ini
 setup.py
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/actions/codeql/security-pack.yml
 .github/actions/spelling/excludes.txt
 .github/actions/spelling/expect.txt
 .github/actions/spelling/patterns.txt
@@ -132,14 +131,15 @@
 src/fprime_gds/common/tools/seqgen.py
 src/fprime_gds/common/utils/__init__.py
 src/fprime_gds/common/utils/config_manager.py
 src/fprime_gds/common/utils/data_desc_type.py
 src/fprime_gds/common/utils/event_severity.py
 src/fprime_gds/common/utils/string_util.py
 src/fprime_gds/executables/__init__.py
+src/fprime_gds/executables/apps.py
 src/fprime_gds/executables/cli.py
 src/fprime_gds/executables/comm.py
 src/fprime_gds/executables/fprime_cli.py
 src/fprime_gds/executables/run_deployment.py
 src/fprime_gds/executables/tcpserver.py
 src/fprime_gds/executables/utils.py
 src/fprime_gds/flask/__init__.py
@@ -248,14 +248,18 @@
 src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff
 src/fprime_gds/flask/static/third-party/webfonts/fa-regular-400.woff2
 src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.eot
 src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.svg
 src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.ttf
 src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff
 src/fprime_gds/flask/static/third-party/webfonts/fa-solid-900.woff2
+src/fprime_gds/plugin/__init__.py
+src/fprime_gds/plugin/definitions.py
+src/fprime_gds/plugin/system.py
+test/fprime_gds/test_plugins.py
 test/fprime_gds/common/distributor/test_distributor.py
 test/fprime_gds/common/encoders/test_ch_encoder.py
 test/fprime_gds/common/encoders/test_event_encoder.py
 test/fprime_gds/common/encoders/test_pkt_encoder.py
 test/fprime_gds/common/gds_cli/filtering_utils_test.py
 test/fprime_gds/common/gds_cli/utils_test.py
 test/fprime_gds/common/history/chronohistory_unit_test.py
@@ -264,8 +268,9 @@
 test/fprime_gds/common/testing_fw/api_unit_test.py
 test/fprime_gds/common/testing_fw/predicate_unit_test.py
 test/fprime_gds/common/testing_fw/logs/.gitignore
 test/fprime_gds/common/tools/seqgen_unit_test.py
 test/fprime_gds/common/utils/test_string_util.py
 test/fprime_gds/executables/test_run_deployment.py
 test/fprime_gds/executables/test_utils.py
+test/fprime_gds/sample/dictionary.xml
 test/gui/GUI_Test_Procedure.md
```

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/distributor/test_distributor.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/distributor/test_distributor.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/encoders/test_ch_encoder.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/encoders/test_ch_encoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/encoders/test_event_encoder.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/encoders/test_event_encoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/encoders/test_pkt_encoder.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/encoders/test_pkt_encoder.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/gds_cli/filtering_utils_test.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/gds_cli/filtering_utils_test.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/gds_cli/utils_test.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/gds_cli/utils_test.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/history/chronohistory_unit_test.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/history/chronohistory_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/history/testhistory_unit_test.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/history/testhistory_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/testing_fw/UnitTestDictionary.xml` & `fprime-gds-3.4.4a1/test/fprime_gds/common/testing_fw/UnitTestDictionary.xml`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/testing_fw/api_unit_test.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/testing_fw/api_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/testing_fw/predicate_unit_test.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/testing_fw/predicate_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/common/utils/test_string_util.py` & `fprime-gds-3.4.4a1/test/fprime_gds/common/utils/test_string_util.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/fprime_gds/executables/test_run_deployment.py` & `fprime-gds-3.4.4a1/test/fprime_gds/executables/test_run_deployment.py`

 * *Files identical despite different names*

### Comparing `fprime-gds-3.4.3/test/gui/GUI_Test_Procedure.md` & `fprime-gds-3.4.4a1/test/gui/GUI_Test_Procedure.md`

 * *Files identical despite different names*

