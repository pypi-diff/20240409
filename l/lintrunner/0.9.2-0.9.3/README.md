# Comparing `tmp/lintrunner-0.9.2.tar.gz` & `tmp/lintrunner-0.9.3.tar.gz`

## Comparing `lintrunner-0.9.2.tar` & `lintrunner-0.9.3.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 lintrunner-0.9.2/Cargo.toml
--rw-r--r--   0     1001      121     1892 2022-05-11 18:58:59.000000 lintrunner-0.9.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      121     1074 2022-05-11 18:58:59.000000 lintrunner-0.9.2/.gitignore
--rw-r--r--   0     1001      121     3877 2022-05-11 18:58:59.000000 lintrunner-0.9.2/CHANGELOG.md
--rw-r--r--   0        0        0    26048 2022-05-11 19:00:32.000000 lintrunner-0.9.2/Cargo.lock
--rw-r--r--   0     1001      121     1068 2022-05-11 18:58:59.000000 lintrunner-0.9.2/LICENSE
--rw-r--r--   0     1001      121     5335 2022-05-11 18:58:59.000000 lintrunner-0.9.2/README.md
--rw-r--r--   0     1001      121     2234 2022-05-11 18:58:59.000000 lintrunner-0.9.2/cliff.toml
--rw-r--r--   0     1001      121      368 2022-05-11 18:58:59.000000 lintrunner-0.9.2/examples/config_example.toml
--rw-r--r--   0     1001      121    11283 2022-05-11 18:58:59.000000 lintrunner-0.9.2/examples/flake8_linter.py
--rw-r--r--   0     1001      121     6991 2022-05-11 18:58:59.000000 lintrunner-0.9.2/examples/rustfmt_linter.py
--rw-r--r--   0     1001      121      352 2022-05-11 18:58:59.000000 lintrunner-0.9.2/pyproject.toml
--rwxr-xr-x   0     1001      121      691 2022-05-11 18:59:23.000000 lintrunner-0.9.2/run-maturin-action.sh
--rw-r--r--   0     1001      121      165 2022-05-11 18:58:59.000000 lintrunner-0.9.2/rustfmt.toml
--rw-r--r--   0     1001      121    12860 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/git.rs
--rw-r--r--   0     1001      121     1569 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/init.rs
--rw-r--r--   0     1001      121     9186 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/lib.rs
--rw-r--r--   0     1001      121     7960 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/lint_config.rs
--rw-r--r--   0     1001      121     2044 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/lint_message.rs
--rw-r--r--   0     1001      121     7545 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/linter.rs
--rw-r--r--   0     1001      121     3467 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/log_utils.rs
--rw-r--r--   0     1001      121    10370 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/main.rs
--rw-r--r--   0     1001      121     4251 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/path.rs
--rw-r--r--   0     1001      121     9963 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/persistent_data.rs
--rw-r--r--   0     1001      121     1719 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/rage.rs
--rw-r--r--   0     1001      121    12475 2022-05-11 18:58:59.000000 lintrunner-0.9.2/src/render.rs
--rw-r--r--   0     1001      121     1090 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/fixtures/fake_source_file.rs
--rw-r--r--   0     1001      121    19825 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/integration_test.rs
--rw-r--r--   0     1001      121      253 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__changed_init_causes_warning_1.snap
--rw-r--r--   0     1001      121      238 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__changed_init_causes_warning_2.snap
--rw-r--r--   0     1001      121      191 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__duplicate_code_fails.snap
--rw-r--r--   0     1001      121      191 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__empty_command_fails.snap
--rw-r--r--   0     1001      121      209 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__excluding_dryrun_fails.snap
--rw-r--r--   0     1001      121      307 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__format_command_doesnt_use_nonformat_linter.snap
--rw-r--r--   0     1001      121     1262 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__git_head_files.snap
--rw-r--r--   0     1001      121     1165 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__git_no_changes.snap
--rw-r--r--   0     1001      121      124 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__init_suppresses_warning.snap
--rw-r--r--   0     1001      121      297 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__invalid_args.snap
--rw-r--r--   0     1001      121      221 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__invalid_config_fails.snap
--rw-r--r--   0     1001      121      317 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__invalid_paths_cmd_and_from.snap
--rw-r--r--   0     1001      121      302 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__invalid_paths_cmd_and_specified_paths.snap
--rw-r--r--   0     1001      121      553 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__linter_hard_failure_is_caught.snap
--rw-r--r--   0     1001      121      506 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__linter_nonexistent_command.snap
--rw-r--r--   0     1001      121      483 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__linter_providing_nonexistent_path_degrades_gracefully.snap
--rw-r--r--   0     1001      121      253 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__no_op_config_succeeds.snap
--rw-r--r--   0     1001      121      299 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__rage_command_output.snap
--rw-r--r--   0     1001      121      696 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__simple_linter.snap
--rw-r--r--   0     1001      121      361 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__simple_linter_fails_on_nonexistent_file.snap
--rw-r--r--   0     1001      121      313 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__simple_linter_oneline.snap
--rw-r--r--   0     1001      121      774 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__simple_linter_replacement_message.snap
--rw-r--r--   0     1001      121      214 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__skip_nonexistent_linter.snap
--rw-r--r--   0     1001      121      214 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__take_nonexistent_linter.snap
--rw-r--r--   0     1001      121      225 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__tee_json.snap
--rw-r--r--   0     1001      121      239 2022-05-11 18:58:59.000000 lintrunner-0.9.2/tests/snapshots/integration_test__unknown_config_fails.snap
--rw-r--r--   0        0        0     5824 1970-01-01 00:00:00.000000 lintrunner-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 lintrunner-0.9.3/Cargo.toml
+-rw-r--r--   0     1001      121     2194 2022-09-23 05:49:22.000000 lintrunner-0.9.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      121     1074 2022-09-23 05:49:22.000000 lintrunner-0.9.3/.gitignore
+-rw-r--r--   0     1001      121     4340 2022-09-23 05:49:22.000000 lintrunner-0.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0    29915 2022-09-23 05:51:08.000000 lintrunner-0.9.3/Cargo.lock
+-rw-r--r--   0     1001      121     1068 2022-09-23 05:49:22.000000 lintrunner-0.9.3/LICENSE
+-rw-r--r--   0     1001      121     5335 2022-09-23 05:49:22.000000 lintrunner-0.9.3/README.md
+-rw-r--r--   0     1001      121     2234 2022-09-23 05:49:22.000000 lintrunner-0.9.3/cliff.toml
+-rw-r--r--   0     1001      121      368 2022-09-23 05:49:22.000000 lintrunner-0.9.3/examples/config_example.toml
+-rw-r--r--   0     1001      121    11283 2022-09-23 05:49:22.000000 lintrunner-0.9.3/examples/flake8_linter.py
+-rw-r--r--   0     1001      121     6991 2022-09-23 05:49:22.000000 lintrunner-0.9.3/examples/rustfmt_linter.py
+-rw-r--r--   0     1001      121      352 2022-09-23 05:49:22.000000 lintrunner-0.9.3/pyproject.toml
+-rwxr-xr-x   0     1001      121      741 2022-09-23 05:50:12.000000 lintrunner-0.9.3/run-maturin-action.sh
+-rw-r--r--   0     1001      121      165 2022-09-23 05:49:22.000000 lintrunner-0.9.3/rustfmt.toml
+-rw-r--r--   0     1001      121    14180 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/git.rs
+-rw-r--r--   0     1001      121     1569 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/init.rs
+-rw-r--r--   0     1001      121     9186 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/lib.rs
+-rw-r--r--   0     1001      121     7960 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/lint_config.rs
+-rw-r--r--   0     1001      121     2044 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/lint_message.rs
+-rw-r--r--   0     1001      121     7545 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/linter.rs
+-rw-r--r--   0     1001      121     3467 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/log_utils.rs
+-rw-r--r--   0     1001      121    10370 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/main.rs
+-rw-r--r--   0     1001      121     4251 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/path.rs
+-rw-r--r--   0     1001      121     9963 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/persistent_data.rs
+-rw-r--r--   0     1001      121     1719 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/rage.rs
+-rw-r--r--   0     1001      121    12475 2022-09-23 05:49:22.000000 lintrunner-0.9.3/src/render.rs
+-rw-r--r--   0     1001      121     1090 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/fixtures/fake_source_file.rs
+-rw-r--r--   0     1001      121    21149 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/integration_test.rs
+-rw-r--r--   0     1001      121      253 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__changed_init_causes_warning_1.snap
+-rw-r--r--   0     1001      121      238 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__changed_init_causes_warning_2.snap
+-rw-r--r--   0     1001      121      191 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__duplicate_code_fails.snap
+-rw-r--r--   0     1001      121      191 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__empty_command_fails.snap
+-rw-r--r--   0     1001      121      209 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__excluding_dryrun_fails.snap
+-rw-r--r--   0     1001      121      307 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__format_command_doesnt_use_nonformat_linter.snap
+-rw-r--r--   0     1001      121     1262 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__git_head_files.snap
+-rw-r--r--   0     1001      121     1165 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__git_no_changes.snap
+-rw-r--r--   0     1001      121      124 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__init_suppresses_warning.snap
+-rw-r--r--   0     1001      121      297 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__invalid_args.snap
+-rw-r--r--   0     1001      121      221 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__invalid_config_fails.snap
+-rw-r--r--   0     1001      121      317 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__invalid_paths_cmd_and_from.snap
+-rw-r--r--   0     1001      121      302 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__invalid_paths_cmd_and_specified_paths.snap
+-rw-r--r--   0     1001      121      553 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__linter_hard_failure_is_caught.snap
+-rw-r--r--   0     1001      121      506 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__linter_nonexistent_command.snap
+-rw-r--r--   0     1001      121      483 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__linter_providing_nonexistent_path_degrades_gracefully.snap
+-rw-r--r--   0     1001      121     1584 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__linter_replacement_trailing_newlines.snap
+-rw-r--r--   0     1001      121      253 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__no_op_config_succeeds.snap
+-rw-r--r--   0     1001      121      299 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__rage_command_output.snap
+-rw-r--r--   0     1001      121      696 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__simple_linter.snap
+-rw-r--r--   0     1001      121      361 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__simple_linter_fails_on_nonexistent_file.snap
+-rw-r--r--   0     1001      121      313 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__simple_linter_oneline.snap
+-rw-r--r--   0     1001      121      774 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__simple_linter_replacement_message.snap
+-rw-r--r--   0     1001      121      214 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__skip_nonexistent_linter.snap
+-rw-r--r--   0     1001      121      214 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__take_nonexistent_linter.snap
+-rw-r--r--   0     1001      121      225 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__tee_json.snap
+-rw-r--r--   0     1001      121      239 2022-09-23 05:49:22.000000 lintrunner-0.9.3/tests/snapshots/integration_test__unknown_config_fails.snap
+-rw-r--r--   0        0        0     5824 1970-01-01 00:00:00.000000 lintrunner-0.9.3/PKG-INFO
```

### Comparing `lintrunner-0.9.2/Cargo.toml` & `lintrunner-0.9.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lintrunner"
-version = "0.9.2"
+version = "0.9.3"
 authors = ["Michael Suo <suo@fb.com>"]
 edition = "2021"
 description = "A lint running tool and framework."
 license = "BSD-3-Clause"
 
 [dependencies]
 clap = { version = "3.1.9", features = ["derive"] }
@@ -25,8 +25,8 @@
 blake3 = "1.3.1"
 fern = { version = "0.6.1", features = ["colored"] }
 chrono = "0.4.19"
 dialoguer = "0.10.1"
 
 [dev-dependencies]
 assert_cmd = "2.0.4"
-insta = { version = "1.14.0", features = ["redactions"] }
+insta = { version = "1.20.0", features = ["redactions", "yaml"] }
```

### Comparing `lintrunner-0.9.2/.gitignore` & `lintrunner-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/CHANGELOG.md` & `lintrunner-0.9.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.9.3] - 2022-09-23
+
+### Bug Fixes
+
+- Don't check files that were deleted/moved in working tree ([0fbb2f3](https://github.com/suo/lintrunner/commit/0fbb2f3d01a08088606ee6650e98d9db9b0b7b3a))
+
+### Testing
+
+- Add unit test for trailing whitespace ([bbbcffd](https://github.com/suo/lintrunner/commit/bbbcffd7d095b16fc831fe48c163b4805e6a9aa0))
+- Add missing snapshot ([9fda576](https://github.com/suo/lintrunner/commit/9fda576f330392c244527defb6e80250663744c6))
+
 ## [0.9.2] - 2022-05-11
 
 ### Bug Fixes
 
 - Add more runtime info to logs ([80e78de](https://github.com/suo/lintrunner/commit/80e78dee128f834f4f696c652bcec32a4f0e0d1c))
 
 ### Features
```

### Comparing `lintrunner-0.9.2/Cargo.lock` & `lintrunner-0.9.3/Cargo.lock`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,45 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "ahash"
+version = "0.7.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
+dependencies = [
+ "getrandom",
+ "once_cell",
+ "version_check",
+]
+
+[[package]]
 name = "aho-corasick"
-version = "0.7.18"
+version = "0.7.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e37cfd5e7657ada45f742d6e99ca5788580b5c529dc78faf11ece6dc702656f"
+checksum = "b4f55bd91a0978cbfd91c457a164bab8b4001c833b7f323132c0a4e1922dd44e"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "anyhow"
-version = "1.0.57"
+version = "1.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08f9b8508dccb7687a1d6c4ce66b2b0ecef467c94667de27d8d7fe1f8d2a9cdc"
+checksum = "98161a4e3e2184da77bb14f02184cdd111e83bbbcc9979dfee3c44b9a85f5602"
 
 [[package]]
 name = "arrayref"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4c527152e37cf757a3f78aae5a06fbeefdb07ccc535c980a3208ee3060dd544"
 
@@ -73,69 +93,42 @@
 checksum = "a08e53fc5a564bb15bfe6fae56bd71522205f1f91893f9c0116edad6496c183f"
 dependencies = [
  "arrayref",
  "arrayvec",
  "cc",
  "cfg-if",
  "constant_time_eq",
- "digest 0.10.3",
+ "digest",
 ]
 
 [[package]]
 name = "block-buffer"
-version = "0.7.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0940dc441f31689269e10ac70eb1002a3a1d3ad1390e030043662eb7fe4688b"
-dependencies = [
- "block-padding",
- "byte-tools",
- "byteorder",
- "generic-array 0.12.4",
-]
-
-[[package]]
-name = "block-buffer"
-version = "0.10.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bf7fe51849ea569fd452f37822f606a5cabb684dc918707a0193fd4664ff324"
-dependencies = [
- "generic-array 0.14.5",
-]
-
-[[package]]
-name = "block-padding"
-version = "0.1.5"
+version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa79dedbb091f449f1f39e53edf88d5dbe95f895dae6135a8d7b881fb5af73f5"
+checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
 dependencies = [
- "byte-tools",
+ "generic-array",
 ]
 
 [[package]]
 name = "bstr"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
 dependencies = [
  "lazy_static",
  "memchr",
  "regex-automata",
 ]
 
 [[package]]
-name = "byte-tools"
-version = "0.3.1"
+name = "bumpalo"
+version = "3.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b5ca7a04898ad4bcd41c90c5285445ff5b791899bb1b0abdd2a2aa791211d7"
-
-[[package]]
-name = "byteorder"
-version = "1.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+checksum = "c1ad822118d20d2c234f427000d5acc36eabe1e29a348c89b63dd60b13f28e5d"
 
 [[package]]
 name = "cc"
 version = "1.0.73"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2fff2a6927b3bb87f9595d67196a70493f627687a71d87a0d692242c33f58c11"
 
@@ -143,60 +136,62 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.19"
+version = "0.4.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "670ad68c9088c2a963aaa298cb369688cf3f9465ce5e2d4ca10e6e0098a1ce73"
+checksum = "bfd4d1b31faaa3a89d7934dbded3111da0d2ef28e3ebccdb4f0179f5929d1ef1"
 dependencies = [
- "libc",
+ "iana-time-zone",
+ "js-sys",
  "num-integer",
  "num-traits",
  "time",
+ "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "clap"
-version = "3.1.18"
+version = "3.2.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2dbdf4bdacb33466e854ce889eee8dfd5729abf7ccd7664d0a2d60cd384440b"
+checksum = "86447ad904c7fb335a790c9d7fe3d0d971dc523b8ccd1561a520de9a85302750"
 dependencies = [
  "atty",
  "bitflags",
  "clap_derive",
  "clap_lex",
  "indexmap",
- "lazy_static",
+ "once_cell",
  "strsim",
  "termcolor",
  "textwrap",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "3.1.18"
+version = "3.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25320346e922cffe59c0bbc5410c8d8784509efb321488971081313cb1e1a33c"
+checksum = "ea0c8bce528c4be4da13ea6fead8965e95b6073585a2f05204bd8f4119f82a65"
 dependencies = [
  "heck",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.2.0"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a37c35f1112dad5e6e0b1adaff798507497a18fceeb30cceb3bae7d1427b9213"
+checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
 name = "colored"
 version = "1.9.3"
@@ -206,76 +201,81 @@
  "atty",
  "lazy_static",
  "winapi",
 ]
 
 [[package]]
 name = "console"
-version = "0.15.0"
+version = "0.15.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28b32d32ca44b70c3e4acd7db1babf555fa026e385fb95f18028f88848b3c31"
+checksum = "89eab4d20ce20cea182308bca13088fecea9c05f6776cf287205d41a0ed3c847"
 dependencies = [
  "encode_unicode",
  "libc",
  "once_cell",
- "regex",
- "terminal_size",
+ "terminal_size 0.1.17",
  "unicode-width",
  "winapi",
 ]
 
 [[package]]
 name = "constant_time_eq"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "245097e9a4535ee1e3e3931fcfcd55a796a44c643e8596ff6566d68f09b87bbc"
 
 [[package]]
+name = "core-foundation-sys"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+
+[[package]]
+name = "cpufeatures"
+version = "0.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "crypto-common"
-version = "0.1.3"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57952ca27b5e3606ff4dd79b0020231aaf9d6aa76dc05fd30137538c50bd3ce8"
+checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
- "generic-array 0.14.5",
+ "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "dialoguer"
-version = "0.10.1"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8c8ae48e400addc32a8710c8d62d55cb84249a7d58ac4cd959daecfbaddc545"
+checksum = "a92e7e37ecef6857fdc0c0c5d42fd5b0938e46590c2183cc92dd310a6d078eb1"
 dependencies = [
  "console",
  "tempfile",
  "zeroize",
 ]
 
 [[package]]
 name = "difflib"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6184e33543162437515c2e2b48714794e37845ec9851711914eec9d308f6ebe8"
 
 [[package]]
 name = "digest"
-version = "0.8.1"
+version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3d0c8c8752312f9713efd397ff63acb9f85585afbf179282e720e7704954dd5"
+checksum = "adfbc57365a37acbd2ebf2b64d7e69bb766e2fea813521ed536f5d0520dcf86c"
 dependencies = [
- "generic-array 0.12.4",
-]
-
-[[package]]
-name = "digest"
-version = "0.10.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2fb860ca6fafa5552fb6d0e816a69c8e49f0908bf524e30a90d97c85892d506"
-dependencies = [
- "block-buffer 0.10.2",
+ "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "directories"
 version = "4.0.1"
@@ -300,35 +300,50 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "either"
-version = "1.6.1"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e78d4f1cc4ae33bbfc157ed5d5a5ef3bc29227303d595861deb238fcec4e9457"
+checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
 
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
 [[package]]
-name = "fake-simd"
+name = "errno"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "winapi",
+]
+
+[[package]]
+name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88a8acf291dafb59c2d96e8f59828f3838bb1a70398823ade51a84de6a6deed"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
 
 [[package]]
 name = "fastrand"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3fcf0cee53519c866c09b5de1f6c56ff9d647101f81c1964fa632e148896cdf"
+checksum = "a7a407cfaa3385c4ae6b23e84623d48c2798d06e3e6a1878f7f59f17b3f86499"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "fern"
 version = "0.6.1"
@@ -337,53 +352,47 @@
 dependencies = [
  "colored",
  "log",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.12.4"
+version = "0.14.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffdf9f34f1447443d37393cc6c2b8313aebddcd96906caf34e54c68d8e57d7bd"
-dependencies = [
- "typenum",
-]
-
-[[package]]
-name = "generic-array"
-version = "0.14.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd48d33ec7f05fbfa152300fdad764757cbded343c1aa1cff2fbaf4134851803"
+checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9be70c98951c83b8d2f8f60d7065fa6d5146873094452a1008da8c2f1e4205ad"
+checksum = "4eb1a864a501629691edf6c15a593b7a51eebaa1e8468e9ddc623de7c9b58ec6"
 dependencies = [
  "cfg-if",
  "libc",
- "wasi",
+ "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "glob"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b919933a397b79c37e33b77bb2aa3dc8eb6e165ad809e58ff75bc7db2e34574"
 
 [[package]]
 name = "hashbrown"
-version = "0.11.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab5ef0d4909ef3724cc8cce6ccc8572c5c817592e9285f5464f8e86f8bd3726e"
+checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+dependencies = [
+ "ahash",
+]
 
 [[package]]
 name = "heck"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2540771e65fc8cb83cd6e8a237f70c319bd5c29f78ed1084ba5d50eeac86f7f9"
 
@@ -393,18 +402,31 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "iana-time-zone"
+version = "0.1.49"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3bbaead50122b06e9a973ac20bc7445074d99ad9a0a0654934876908a9cec82c"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "js-sys",
+ "wasm-bindgen",
+ "winapi",
+]
+
+[[package]]
 name = "indexmap"
-version = "1.8.1"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f647032dfaa1f8b6dc29bd3edb7bbef4861b8b8007ebb118d6db284fd59f6ee"
+checksum = "10a35a97730320ffe8e2d410b5d3b69279b98d2c14bdb8b70ea89ecf7888d41e"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indicatif"
@@ -416,73 +438,88 @@
  "lazy_static",
  "number_prefix",
  "regex",
 ]
 
 [[package]]
 name = "insta"
-version = "1.14.0"
+version = "1.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "689960f187c43c01650c805fb6bc6f55ab944499d86d4ffe9474ad78991d8e94"
+checksum = "58a931b01c76064c5be919faa2ef0dc570e9a889dcd1e5fef08a8ca6eb4d6c0b"
 dependencies = [
  "console",
+ "linked-hash-map",
  "once_cell",
  "pest",
  "pest_derive",
  "serde",
- "serde_json",
- "serde_yaml",
  "similar",
+ "yaml-rust",
 ]
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "io-lifetimes"
+version = "0.7.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1ea37f355c05dde75b84bba2d767906ad522e97cd9e2eef2be7a4ab7fb442c06"
+
+[[package]]
 name = "itertools"
-version = "0.10.3"
+version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9a9d19fa1e79b6215ff29b9d6880b706147f16e9b1dbb1e4e5947b5b02bc5e3"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.1"
+version = "1.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c8af84674fe1f223a982c933a0ee1086ac4d4052aa0fb8060c12c6ad838e754"
+
+[[package]]
+name = "js-sys"
+version = "0.3.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1aab8fc367588b89dcee83ab0fd66b72b50b72fa1904d7095045ace2b0c81c35"
+checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+dependencies = [
+ "wasm-bindgen",
+]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.125"
+version = "0.2.133"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5916d2ae698f6de9bfb891ad7a8d65c09d232dc58cc4ac433c7da3b2fd84bc2b"
+checksum = "c0f80d65747a3e43d1596c7c5492d95d5edddaabd45a7fcdb02b95f644164966"
 
 [[package]]
 name = "linked-hash-map"
-version = "0.5.4"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fb9b38af92608140b86b693604b9ffcc5824240a484d1ecd4795bacb2fe88f3"
+checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "lintrunner"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "blake3",
  "chrono",
  "clap",
  "console",
@@ -500,29 +537,29 @@
  "similar",
  "tempfile",
  "textwrap",
  "toml",
 ]
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.0.46"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d4d2456c373231a208ad294c33dc5bff30051eafd954cd4caae83a712b12854d"
+
+[[package]]
 name = "log"
 version = "0.4.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "maplit"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e2e65a1a2e43cfcb47a895c4c8b10d1f4a61097f9f254f183aee60cad9c651d"
-
-[[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "num-integer"
@@ -547,71 +584,66 @@
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
 name = "once_cell"
-version = "1.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87f3e037eac156d1775da914196f0f37741a274155e34a0b7e427c35d2a2ecb9"
-
-[[package]]
-name = "opaque-debug"
-version = "0.2.3"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2839e79665f131bdb5782e51f2c6c9599c133c6098982a54c794358bf432529c"
+checksum = "e82dad04139b71a90c080c8463fe0dc7902db5192d939bd0950f074d014339e1"
 
 [[package]]
 name = "os_str_bytes"
-version = "6.0.0"
+version = "6.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e22443d1643a904602595ba1cd8f7d896afe56d26712531c5ff73a15b2fbf64"
+checksum = "9ff7415e9ae3fff1225851df9e0d9e4e5479f947619774677a63572e55e80eff"
 
 [[package]]
 name = "pest"
-version = "2.1.3"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10f4872ae94d7b90ae48754df22fd42ad52ce740b8f370b03da4835417403e53"
+checksum = "cb779fcf4bb850fbbb0edc96ff6cf34fd90c4b1a112ce042653280d9a7364048"
 dependencies = [
+ "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.1.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "833d1ae558dc601e9a60366421196a8d94bc0ac980476d0b67e1d0988d72b2d0"
+checksum = "502b62a6d0245378b04ffe0a7fb4f4419a4815fce813bd8a0ec89a56e07d67b1"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.1.3"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99b8db626e31e5b81787b9783425769681b347011cc59471e33ea46d2ea0cf55"
+checksum = "451e629bf49b750254da26132f1a5a9d11fd8a95a3df51d15c4abd1ba154cb6c"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.1.3"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54be6e404f5317079812fc8f9f5279de376d8856929e21c184ecf6bbd692a11d"
+checksum = "bcec162c71c45e269dfc3fc2916eaeb97feab22993a21bcce4721d08cd7801a6"
 dependencies = [
- "maplit",
+ "once_cell",
  "pest",
- "sha-1",
+ "sha1",
 ]
 
 [[package]]
 name = "predicates"
 version = "2.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5aab5be6e4732b473071984b3164dbbfb7a3674d30ea5ff44410b6bcd960c3c"
@@ -659,35 +691,35 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.38"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9027b48e9d4c9175fa2218adf3557f91c1137021739951d4932f5f8268ac48aa"
+checksum = "0a2ca2c61bc9f3d74d2886294ab7b9853abd9c1ad903a3ac7815c58989bb7bab"
 dependencies = [
- "unicode-xid",
+ "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.18"
+version = "1.0.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1feb54ed693b93a84e14094943b84b7c4eae204c512b7ccb95ab0c66d278ad1"
+checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.13"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62f25bc4c7e55e0b0b7a1d43fb893f4fa1361d0abe38b9ce4f323c2adfe6ef42"
+checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "redox_users"
 version = "0.4.3"
@@ -697,110 +729,111 @@
  "getrandom",
  "redox_syscall",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.5.5"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a11647b6b25ff05a515cb92c365cec08801e83423a235b51e231e1808747286"
+checksum = "4c4eb3267174b8c6c2f654116623910a0fef09c4753f8dd83db29c48a0df988b"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.25"
+version = "0.6.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f497285884f3fcff424ffc933e56d7cbca511def0c9831a7f9b5f6153e3cc89b"
+checksum = "a3f87b73ce11b1619a3c6332f45341e0047173771e8b8b73f87bfeefb7b56244"
 
 [[package]]
 name = "remove_dir_all"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
+name = "rustix"
+version = "0.35.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af895b90e5c071badc3136fc10ff0bcfc98747eadbaf43ed8f214e07ba8f8477"
+dependencies = [
+ "bitflags",
+ "errno",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys",
+]
+
+[[package]]
 name = "ryu"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73b4b750c782965c211b42f022f59af1fbceabdd026623714f104152f1ec149f"
+checksum = "4501abdff3ae82a1c1b477a17252eb69cee9e66eb915c1abaa4f44d873df9f09"
 
 [[package]]
 name = "serde"
-version = "1.0.137"
+version = "1.0.145"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61ea8d54c77f8315140a05f4c7237403bf38b72704d031543aa1d16abbf517d1"
+checksum = "728eb6351430bccb993660dfffc5a72f91ccc1295abaa8ce19b27ebe4f75568b"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.137"
+version = "1.0.145"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f26faba0c3959972377d3b2d306ee9f71faee9714294e41bb777f83f88578be"
+checksum = "81fa1584d3d1bcacd84c277a0dfe21f5b0f6accf4a23d04d4c6d61f1af522b4c"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.81"
+version = "1.0.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7ce2b32a1aed03c558dc61a5cd328f15aff2dbc17daad8fb8af04d2100e15c"
+checksum = "e55a28e3aaef9d5ce0506d0a14dbba8054ddc7e499ef522dd8b26859ec9d4a44"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
-name = "serde_yaml"
-version = "0.8.24"
+name = "sha1"
+version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "707d15895415db6628332b737c838b88c598522e4dc70647e59b72312924aebc"
+checksum = "f04293dc80c3993519f2d7f6f511707ee7094fe0c6d3406feb330cdb3540eba3"
 dependencies = [
- "indexmap",
- "ryu",
- "serde",
- "yaml-rust",
-]
-
-[[package]]
-name = "sha-1"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7d94d0bede923b3cea61f3f1ff57ff8cdfd77b400fb8f9998949e0cf04163df"
-dependencies = [
- "block-buffer 0.7.3",
- "digest 0.8.1",
- "fake-simd",
- "opaque-debug",
+ "cfg-if",
+ "cpufeatures",
+ "digest",
 ]
 
 [[package]]
 name = "similar"
-version = "2.1.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e24979f63a11545f5f2c60141afe249d4f19f84581ea2138065e400941d83d3"
+checksum = "62ac7f900db32bf3fd12e0117dd3dc4da74bc52ebaac97f39668446d89694803"
 
 [[package]]
 name = "smawk"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f67ad224767faa3c7d8b6d91985b78e70a1324408abcb1cfcc2be4c06bc06043"
 
@@ -814,21 +847,21 @@
 name = "subtle"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
 
 [[package]]
 name = "syn"
-version = "1.0.93"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04066589568b72ec65f42d65a1a52436e954b168773148893c020269563decf2"
+checksum = "52205623b1b0f064a4e71182c3b18ae902267282930c6d5462c91b859668426e"
 dependencies = [
  "proc-macro2",
  "quote",
- "unicode-xid",
+ "unicode-ident",
 ]
 
 [[package]]
 name = "tempfile"
 version = "3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cdb1ef4eaeeaddc8fbd371e5017057064af0911902ef36b39801f67cc6d79e4"
@@ -857,59 +890,69 @@
 checksum = "633c1a546cee861a1a6d0dc69ebeca693bf4296661ba7852b9d21d159e0506df"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "terminal_size"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8440c860cf79def6164e4a0a983bcc2305d82419177a0e0c71930d049e3ac5a1"
+dependencies = [
+ "rustix",
+ "windows-sys",
+]
+
+[[package]]
 name = "termtree"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "507e9898683b6c43a9aa55b64259b721b52ba226e0f3779137e50ad114a4c90b"
 
 [[package]]
 name = "textwrap"
-version = "0.15.0"
+version = "0.15.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1141d4d61095b28419e22cb0bbf02755f5e54e0526f97f1e3d1d160e60885fb"
+checksum = "949517c0cf1bf4ee812e2e07e08ab448e3ae0d23472aee8a06c985f0c8815b16"
 dependencies = [
  "smawk",
- "terminal_size",
+ "terminal_size 0.2.1",
  "unicode-linebreak",
  "unicode-width",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.31"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd829fe32373d27f76265620b5309d0340cb8550f523c1dda251d6298069069a"
+checksum = "c53f98874615aea268107765aa1ed8f6116782501d18e53d08b471733bea6c85"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.31"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0396bc89e626244658bef819e22d0cc459e795a5ebe878e6ec336d1674a8d79a"
+checksum = "f8b463991b4eab2d801e724172285ec4195c650e8ec79b149e6c2a8e6dd3f783"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6db9e6914ab8b1ae1c260a4ae7a49b6c5611b40328a735b21862567685e73255"
 dependencies = [
  "libc",
- "wasi",
+ "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "toml"
 version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -922,38 +965,39 @@
 name = "typenum"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dcf81ac59edc17cc8697ff311e8f5ef2d99fcbd9817b34cec66f90b6c3dfd987"
 
 [[package]]
 name = "ucd-trie"
-version = "0.1.3"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56dee185309b50d1f11bfedef0fe6d036842e3fb77413abef29f8f8d1c5d4c1c"
+checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
+
+[[package]]
+name = "unicode-ident"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dcc811dc4066ac62f84f11307873c4850cb653bfa9b1719cee2bd2204a4bc5dd"
 
 [[package]]
 name = "unicode-linebreak"
-version = "0.1.2"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a52dcaab0c48d931f7cc8ef826fa51690a08e1ea55117ef26f89864f532383f"
+checksum = "ba853b89cad55680dd3cf06f2798cb1ad8d483f0e2dfa14138d7e789ecee5c4e"
 dependencies = [
+ "hashbrown",
  "regex",
 ]
 
 [[package]]
 name = "unicode-width"
-version = "0.1.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ed742d4ea2bd1176e236172c8429aaf54486e7ac098db29ffe6529e0ce50973"
-
-[[package]]
-name = "unicode-xid"
-version = "0.2.3"
+version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "957e51f3646910546462e67d5f7599b9e4fb8acdd304b087a6494730f9eebf04"
+checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
@@ -969,14 +1013,74 @@
 [[package]]
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
 
 [[package]]
+name = "wasi"
+version = "0.11.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
+
+[[package]]
+name = "wasm-bindgen"
+version = "0.2.83"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen-macro",
+]
+
+[[package]]
+name = "wasm-bindgen-backend"
+version = "0.2.83"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+dependencies = [
+ "bumpalo",
+ "log",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-macro"
+version = "0.2.83"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+dependencies = [
+ "quote",
+ "wasm-bindgen-macro-support",
+]
+
+[[package]]
+name = "wasm-bindgen-macro-support"
+version = "0.2.83"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+ "wasm-bindgen-backend",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-shared"
+version = "0.2.83"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -1000,20 +1104,63 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows-sys"
+version = "0.36.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
+dependencies = [
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_msvc",
+]
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.36.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.36.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.36.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.36.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.36.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
+
+[[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.5.5"
+version = "1.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94693807d016b2f2d2e14420eb3bfcca689311ff775dcf113d74ea624b7cdf07"
+checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
```

### Comparing `lintrunner-0.9.2/LICENSE` & `lintrunner-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/README.md` & `lintrunner-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/cliff.toml` & `lintrunner-0.9.3/cliff.toml`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/examples/flake8_linter.py` & `lintrunner-0.9.3/examples/flake8_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/examples/rustfmt_linter.py` & `lintrunner-0.9.3/examples/rustfmt_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/run-maturin-action.sh` & `lintrunner-0.9.3/run-maturin-action.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/bin/bash
 set -e
 echo "::group::Install Rust"
 which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain stable
 export PATH="$HOME/.cargo/bin:$PATH"
 rustup override set stable
+rustup component add llvm-tools-preview || true
 echo "::endgroup::"
 export PATH="$PATH:/opt/python/cp36-cp36m/bin:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin"
 echo "::group::Install maturin"
-curl -L https://github.com/PyO3/maturin/releases/latest/download/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
+curl -L https://github.com/PyO3/maturin/releases/download/v0.12.20/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
 echo "::endgroup::"
 maturin build --release -o dist
```

### Comparing `lintrunner-0.9.2/src/git.rs` & `lintrunner-0.9.3/src/git.rs`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,15 @@
     path::AbsPath,
 };
 use anyhow::{ensure, Context, Result};
 use log::debug;
 use regex::Regex;
 
 pub fn get_head() -> Result<String> {
-    let output = Command::new("git")
-        .arg("rev-parse")
-        .arg("HEAD")
-        .output()?;
+    let output = Command::new("git").arg("rev-parse").arg("HEAD").output()?;
     ensure_output("git rev-parse", &output)?;
     let head = std::str::from_utf8(&output.stdout)?.trim();
     Ok(head.to_string())
 }
 
 pub fn get_paths_from_cmd(paths_cmd: &str) -> Result<Vec<AbsPath>> {
     debug!("Running paths_cmd: {}", paths_cmd);
@@ -114,17 +111,35 @@
         .filter(|line| !line.starts_with('D'))
         // Strip the status prefix.
         .map(|line| re.replace(line, "").to_string())
         .collect();
 
     log_files("Linting working tree diff files: ", &working_tree_files);
 
-    working_tree_files
+    let deleted_working_tree_files: HashSet<String> = working_tree_files_str
+        .lines()
+        .filter(|line| !line.is_empty())
+        // Filter IN deleted files.
+        .filter(|line| line.starts_with('D'))
+        // Strip the status prefix.
+        .map(|line| re.replace(line, "").to_string())
+        .collect();
+
+    log_files(
+        "These files were deleted in the working tree and won't be checked: ",
+        &working_tree_files,
+    );
+
+    let all_files = working_tree_files
         .union(&commit_files)
-        .into_iter()
+        .map(|s| s.to_string())
+        .collect::<HashSet<_>>();
+
+    all_files
+        .difference(&deleted_working_tree_files)
         // Git reports files relative to the root of git root directory, so retrieve
         // that and prepend it to the file paths.
         .map(|f| format!("{}/{}", git_root.display(), f))
         .map(|f| {
             AbsPath::try_from(&f).with_context(|| {
                 format!("Failed to find file while gathering files to lint: {}", f)
             })
@@ -278,14 +293,38 @@
         git.rm_file("test_2.txt")?;
 
         let files = git.changed_files(None)?;
         assert_eq!(files.len(), 0);
         Ok(())
     }
 
+    // Files that were deleted/moved in the working tree should not be checked,
+    // since obviously they are gone.
+    #[test]
+    fn moved_files_working_tree() -> Result<()> {
+        let git = GitCheckout::new()?;
+        git.write_file("test_1.txt", "Initial commit")?;
+        git.add(".")?;
+        git.commit("commit 1")?;
+
+        git.write_file("test_2.txt", "foo")?;
+        git.add(".")?;
+        git.commit("commit 2")?;
+
+        let output = Command::new("git")
+            .args(&["mv", "test_2.txt", "new.txt"])
+            .current_dir(git.root.path())
+            .output()?;
+        assert!(output.status.success());
+
+        let files = git.changed_files(None)?;
+        assert!(files.contains(&"new.txt".to_string()));
+        Ok(())
+    }
+
     #[test]
     fn relative_revision() -> Result<()> {
         let git = GitCheckout::new()?;
         git.write_file("test_1.txt", "Initial commit")?;
         git.write_file("test_2.txt", "Initial commit")?;
         git.write_file("test_3.txt", "Initial commit")?;
```

### Comparing `lintrunner-0.9.2/src/init.rs` & `lintrunner-0.9.3/src/init.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/lib.rs` & `lintrunner-0.9.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/lint_config.rs` & `lintrunner-0.9.3/src/lint_config.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/lint_message.rs` & `lintrunner-0.9.3/src/lint_message.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/linter.rs` & `lintrunner-0.9.3/src/linter.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/log_utils.rs` & `lintrunner-0.9.3/src/log_utils.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/main.rs` & `lintrunner-0.9.3/src/main.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/path.rs` & `lintrunner-0.9.3/src/path.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/persistent_data.rs` & `lintrunner-0.9.3/src/persistent_data.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/rage.rs` & `lintrunner-0.9.3/src/rage.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/src/render.rs` & `lintrunner-0.9.3/src/render.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/tests/fixtures/fake_source_file.rs` & `lintrunner-0.9.3/tests/fixtures/fake_source_file.rs`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/tests/integration_test.rs` & `lintrunner-0.9.3/tests/integration_test.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use anyhow::Result;
 use assert_cmd::Command;
-use insta::{assert_yaml_snapshot, assert_snapshot};
+use insta::{assert_snapshot, assert_yaml_snapshot};
 use lintrunner::lint_message::{LintMessage, LintSeverity};
 use regex::Regex;
 use serde_json;
 use std::io::Write;
 
 fn assert_output_snapshot(name: &str, cmd: &mut Command) -> Result<()> {
     let re = Regex::new("'.*test-lintrunner-config.*toml'").unwrap();
@@ -699,7 +699,54 @@
 
     let tee_json = std::fs::read_to_string(data_path.path().join("foo.json"))?;
 
     assert_snapshot!("tee_json", tee_json);
 
     Ok(())
 }
+
+#[test]
+fn linter_replacement_trailing_newlines() -> Result<()> {
+    let data_path = tempfile::tempdir()?;
+    let lint_message = LintMessage {
+        path: Some("tests/fixtures/fake_source_file.rs".to_string()),
+        line: Some(9),
+        char: Some(1),
+        code: "DUMMY".to_string(),
+        name: "dummy failure".to_string(),
+        severity: LintSeverity::Advice,
+        original: Some(
+            "\
+            foo       \n\
+            bar     \n\
+            baz    \n\
+            foo       \n\
+        "
+            .to_string(),
+        ),
+        replacement: Some(
+            "\
+            foo\n\
+            bar\n\
+            baz\n\
+            foo\n\
+        "
+            .to_string(),
+        ),
+        description: Some("A dummy linter failure".to_string()),
+    };
+    let config = temp_config_returning_msg(lint_message)?;
+
+    let mut cmd = Command::cargo_bin("lintrunner")?;
+    cmd.arg(format!("--config={}", config.path().to_str().unwrap()));
+    cmd.arg(format!(
+        "--data-path={}",
+        data_path.path().to_str().unwrap()
+    ));
+    cmd.arg(format!("--force-color"));
+    // Run on a file to ensure that the linter is run.
+    cmd.arg("README.md");
+    cmd.assert().failure();
+    assert_output_snapshot("linter_replacement_trailing_newlines", &mut cmd)?;
+
+    Ok(())
+}
```

### Comparing `lintrunner-0.9.2/tests/snapshots/integration_test__git_head_files.snap` & `lintrunner-0.9.3/tests/snapshots/integration_test__git_head_files.snap`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/tests/snapshots/integration_test__git_no_changes.snap` & `lintrunner-0.9.3/tests/snapshots/integration_test__git_no_changes.snap`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/tests/snapshots/integration_test__linter_hard_failure_is_caught.snap` & `lintrunner-0.9.3/tests/snapshots/integration_test__linter_hard_failure_is_caught.snap`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/tests/snapshots/integration_test__simple_linter.snap` & `lintrunner-0.9.3/tests/snapshots/integration_test__simple_linter.snap`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/tests/snapshots/integration_test__simple_linter_replacement_message.snap` & `lintrunner-0.9.3/tests/snapshots/integration_test__simple_linter_replacement_message.snap`

 * *Files identical despite different names*

### Comparing `lintrunner-0.9.2/PKG-INFO` & `lintrunner-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintrunner
-Version: 0.9.2
+Version: 0.9.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: A lint running tool and framework.
 Author: Michael Suo <suo@fb.com>
 Author-email: Michael Suo <suo@fb.com>
```

