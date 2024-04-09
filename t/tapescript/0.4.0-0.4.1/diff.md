# Comparing `tmp/tapescript-0.4.0.tar.gz` & `tmp/tapescript-0.4.1.tar.gz`

## Comparing `tapescript-0.4.0.tar` & `tapescript-0.4.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tapescript-0.4.0/changelog.md
--rw-r--r--   0        0        0    25963 2020-02-02 00:00:00.000000 tapescript-0.4.0/docs.md
--rw-r--r--   0        0        0    28025 2020-02-02 00:00:00.000000 tapescript-0.4.0/language_spec.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tapescript-0.4.0/license
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tapescript-0.4.0/requirements.txt
--rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 tapescript-0.4.0/script_examples.md
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 tapescript-0.4.0/tapescript/AMHL.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 tapescript-0.4.0/tapescript/__init__.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 tapescript-0.4.0/tapescript/classes.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tapescript-0.4.0/tapescript/errors.py
--rw-r--r--   0        0        0    71862 2020-02-02 00:00:00.000000 tapescript-0.4.0/tapescript/functions.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 tapescript-0.4.0/tapescript/interfaces.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 tapescript-0.4.0/tapescript/notes.md
--rw-r--r--   0        0        0    49796 2020-02-02 00:00:00.000000 tapescript-0.4.0/tapescript/parsing.py
--rw-r--r--   0        0        0    34258 2020-02-02 00:00:00.000000 tapescript-0.4.0/tapescript/tools.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/context.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/debug.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/test_classes.py
--rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/test_e2e_eltoo.py
--rw-r--r--   0        0        0   107136 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/test_functions.py
--rw-r--r--   0        0        0    26900 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/test_parsing.py
--rw-r--r--   0        0        0    36207 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/test_tools.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/1.hex
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/1.src
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/2.hex
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/2.src
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/2_decompiled.src
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/3.hex
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/3.src
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/3_decompiled.src
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/4.hex
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/4.src
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/4_decompiled.src
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/5.hex
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/5.src
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/5_decompiled.src
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/6.hex
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/6.src
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/6_decompiled.src
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/branching_e2e.hex
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/branching_e2e.src
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/branching_e2e_decompiled.src
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_committed_script.hex
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_committed_script.src
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_committed_script_decompiled.src
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_locking_script.hex
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_locking_script.src
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_locking_script_decompiled.src
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_unlocking_script1.hex
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_unlocking_script1.src
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_unlocking_script1_decompiled.src
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_unlocking_script2.hex
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_unlocking_script2.src
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_unlocking_script2_decompiled.src
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_unlocking_script3.hex
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_unlocking_script3.src
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/cds_unlocking_script3_decompiled.src
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_committed_script.hex
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_committed_script.src
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_committed_script_decompiled.src
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_locking_script.hex
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_locking_script.src
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_locking_script_decompiled.src
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_unlocking_script1.hex
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_unlocking_script1.src
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_unlocking_script1_decompiled.src
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_unlocking_script2.hex
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_unlocking_script2.src
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/correspondent_unlocking_script2_decompiled.src
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/macros_and_variables.hex
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/macros_and_variables.src
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/macros_and_variables_decompiled.src
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_a.hex
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_a.src
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_a_decompiled.src
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_b.hex
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_b.src
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_ba.hex
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_ba.src
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_ba_decompiled.src
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_bb.hex
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_bb.src
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_committed_script_bb_decompiled.src
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_locking_script.hex
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_locking_script.src
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_unlocking_script_a.hex
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_unlocking_script_a.src
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_unlocking_script_a_decompiled.src
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_unlocking_script_ba.hex
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_unlocking_script_ba.src
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_unlocking_script_ba_decompiled.src
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_unlocking_script_bb.hex
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_unlocking_script_bb.src
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/merkleval_unlocking_script_bb_decompiled.src
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/new_if_hoist_syntax_0.4.0.hex
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/new_if_hoist_syntax_0.4.0.src
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/new_if_hoist_syntax_0.4.0_decompiled.src
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/new_ops_0.4.0.hex
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/new_ops_0.4.0.src
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/new_ops_0.4.0_decompiled.src
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/omega_e2e.hex
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/omega_e2e.src
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/omega_e2e_aliases.src
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/omega_e2e_decompiled.src
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2pk_locking_script.hex
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2pk_locking_script.src
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2pk_locking_script_decompiled.src
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2pk_unlocking_script1.hex
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2pk_unlocking_script1.src
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2pk_unlocking_script1_decompiled.src
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2pk_unlocking_script2.hex
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2pk_unlocking_script2.src
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2pk_unlocking_script2_decompiled.src
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2sh_committed_script.hex
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2sh_committed_script.src
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2sh_committed_script_decompiled.src
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2sh_locking_script.hex
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2sh_locking_script.src
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2sh_locking_script_decompiled.src
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2sh_unlocking_script.hex
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2sh_unlocking_script.src
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/p2sh_unlocking_script_decompiled.src
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/try_in_if.hex
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/try_in_if.src
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/trydef.hex
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.0/tests/vectors/trydef.src
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tapescript-0.4.0/.gitignore
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 tapescript-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    17501 2020-02-02 00:00:00.000000 tapescript-0.4.0/readme.md
--rw-r--r--   0        0        0    18183 2020-02-02 00:00:00.000000 tapescript-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 tapescript-0.4.1/changelog.md
+-rw-r--r--   0        0        0    25982 2020-02-02 00:00:00.000000 tapescript-0.4.1/docs.md
+-rw-r--r--   0        0        0    28025 2020-02-02 00:00:00.000000 tapescript-0.4.1/language_spec.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tapescript-0.4.1/license
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tapescript-0.4.1/requirements.txt
+-rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 tapescript-0.4.1/script_examples.md
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/AMHL.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/__init__.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/classes.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/errors.py
+-rw-r--r--   0        0        0    72141 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/functions.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/interfaces.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/notes.md
+-rw-r--r--   0        0        0    50537 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/parsing.py
+-rw-r--r--   0        0        0    34258 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/tools.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/context.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/debug.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_classes.py
+-rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_e2e_eltoo.py
+-rw-r--r--   0        0        0   108069 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_functions.py
+-rw-r--r--   0        0        0    26875 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_parsing.py
+-rw-r--r--   0        0        0    36207 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_tools.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/1.hex
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/1.src
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/2.hex
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/2.src
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/2_decompiled.src
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/3.hex
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/3.src
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/3_decompiled.src
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/4.hex
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/4.src
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/4_decompiled.src
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/5.hex
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/5.src
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/5_decompiled.src
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/6.hex
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/6.src
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/6_decompiled.src
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/branching_e2e.hex
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/branching_e2e.src
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/branching_e2e_decompiled.src
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_committed_script.hex
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_committed_script.src
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_committed_script_decompiled.src
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_locking_script.hex
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_locking_script.src
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_locking_script_decompiled.src
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script1.hex
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script1.src
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script1_decompiled.src
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script2.hex
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script2.src
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script2_decompiled.src
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script3.hex
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script3.src
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script3_decompiled.src
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_committed_script.hex
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_committed_script.src
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_committed_script_decompiled.src
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_locking_script.hex
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_locking_script.src
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_locking_script_decompiled.src
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script1.hex
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script1.src
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script1_decompiled.src
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2.hex
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2.src
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2_decompiled.src
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/macros_and_variables.hex
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/macros_and_variables.src
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/macros_and_variables_decompiled.src
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_a.hex
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_a.src
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_a_decompiled.src
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_b.hex
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_b.src
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_ba.hex
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_ba.src
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_ba_decompiled.src
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_bb.hex
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_bb.src
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_bb_decompiled.src
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_locking_script.hex
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_locking_script.src
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_a.hex
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_a.src
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_a_decompiled.src
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_ba.hex
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_ba.src
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_ba_decompiled.src
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_bb.hex
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_bb.src
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_bb_decompiled.src
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_if_hoist_syntax_0.4.0.hex
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_if_hoist_syntax_0.4.0.src
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_if_hoist_syntax_0.4.0_decompiled.src
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_ops_0.4.0.hex
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_ops_0.4.0.src
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_ops_0.4.0_decompiled.src
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/omega_e2e.hex
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/omega_e2e.src
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/omega_e2e_aliases.src
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/omega_e2e_decompiled.src
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_locking_script.hex
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_locking_script.src
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_locking_script_decompiled.src
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script1.hex
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script1.src
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script1_decompiled.src
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script2.hex
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script2.src
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script2_decompiled.src
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_committed_script.hex
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_committed_script.src
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_committed_script_decompiled.src
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_locking_script.hex
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_locking_script.src
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_locking_script_decompiled.src
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_unlocking_script.hex
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_unlocking_script.src
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_unlocking_script_decompiled.src
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/try_in_if.hex
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/try_in_if.src
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/trydef.hex
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/trydef.src
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tapescript-0.4.1/.gitignore
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 tapescript-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 tapescript-0.4.1/readme.md
+-rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 tapescript-0.4.1/PKG-INFO
```

### Comparing `tapescript-0.4.0/changelog.md` & `tapescript-0.4.1/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 0.4.1
+
+- Fixed `OP_NOT` to do a proper bitwise `NOT` operation.
+- Switched the `true` value from `0x01` to `0xff` for compatibility with `FALSE NOT`
+- Fixed compiler to handle negative ints.
+- Added 32-bit float type to arg parsing forsome args: preface the value with `f`.
+
 ## 0.4.0
 
 - Changed `OP_CHECK_TRANSFER` to pull the `count` parameter from the queue.
 - Added `OP_LESS`: pulls ints value1 and value2 from the queue and puts
 `value1<value2` onto the queue.
 - Added `OP_LESS_OR_EQUAL` (alias `OP_LEQ`): pulls ints value1 and value2 from
 the queue and puts `value1<=value2` onto the queue.
```

### Comparing `tapescript-0.4.0/docs.md` & `tapescript-0.4.1/docs.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Puts a null byte onto the queue.
 
 Aliases:
 - FALSE
 
 ## OP_TRUE - 1 - x01
 
-Puts a 0x01 byte onto the queue.
+Puts a 0xFF byte onto the queue.
 
 Aliases:
 - TRUE
 
 ## OP_PUSH0 - 2 - x02
 
 Read the next byte from the tape; put it onto the queue.
@@ -419,16 +419,16 @@
 tape.definitions; it also has access to all loaded contracts.
 
 Aliases:
 - EVAL
 
 ## OP_NOT - 46 - x2E
 
-Pulls a value from the queue, interpreting as a bool; performs logical NOT
-operation; puts that value onto the queue.
+Pulls a value from the queue; performs bitwise NOT operation; puts result onto
+the queue.
 
 Aliases:
 - NOT
 
 ## OP_RANDOM - 47 - x2F
 
 Read the next byte from the tape, interpreting as an unsigned int; put that many
@@ -838,17 +838,18 @@
 Aliases:
 - GET_MESSAGE
 - OP_MSG
 - MSG
 
 ## NOP Codes - 90-255 (x5A-FF)
 
-Codes in 90-255 (x5A-FF) Read the next byte from the tape, interpreting as an
-unsigned int and pull that many values from the queue. Does nothing with the
-values. Useful for later soft-forks by redefining byte codes.
+Codes in 90-255 (x5A-FF) Read the next byte from the tape, interpreting as a
+signed int and pull that many values from the queue. Does nothing with the
+values. Useful for later soft-forks by redefining byte codes. Raises
+ScriptExecutionError if count is negative.
 
 
 # Other interpreter functions
 
 ## `run_script(script: bytes, cache_vals: dict = {}, contracts: dict = {}, additional_flags: dict = {}): -> tuple[Tape, LifoQueue, dict]`
 
 Run the given script byte code. Returns a tape, queue, and dict.
@@ -856,15 +857,15 @@
 ## `run_tape(tape: Tape, queue: LifoQueue, cache: dict, additional_flags: dict = {}): -> None`
 
 Run the given tape using the queue and cache.
 
 ## `run_auth_script(script: bytes, cache_vals: dict = {}, contracts: dict = {}): -> bool`
 
 Run the given auth script byte code. Returns True iff the queue has a single
-\x01 value after script execution and no errors were raised; otherwise, returns
+\xff value after script execution and no errors were raised; otherwise, returns
 False.
 
 ## `add_opcode(code: int, name: str, function: Callable): -> None`
 
 Adds an OP implementation with the code, name, and function.
 
 ## `add_contract(contract_id: bytes, contract: object): -> None`
```

### Comparing `tapescript-0.4.0/language_spec.md` & `tapescript-0.4.1/language_spec.md`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/license` & `tapescript-0.4.1/license`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/script_examples.md` & `tapescript-0.4.1/script_examples.md`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tapescript/AMHL.py` & `tapescript-0.4.1/tapescript/AMHL.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tapescript/__init__.py` & `tapescript-0.4.1/tapescript/__init__.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tapescript/classes.py` & `tapescript-0.4.1/tapescript/classes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tapescript/errors.py` & `tapescript-0.4.1/tapescript/errors.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tapescript/functions.py` & `tapescript-0.4.1/tapescript/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,21 @@
     # compute the sum
     sum = scalars[0]
     for i in range(1, len(scalars)):
         sum = nacl.bindings.crypto_core_ed25519_scalar_add(sum, scalars[i])
 
     return sum
 
+def not_bytes(b1: bytes) -> bytes:
+    """Perform a bitwise NOT operation. Implementation is specific to
+        the Python memory model.
+    """
+    n_bits = len(b1)*8
+    return ((1 << n_bits) - 1 - int.from_bytes(b1, 'big')).to_bytes(n_bits//8, 'big')
+
 def xor(b1: bytes, b2: bytes) -> bytes:
     """XOR two equal-length byte strings together."""
     b3 = bytearray()
     for i in range(len(b1)):
         b3.append(b1[i] ^ b2[i])
 
     return bytes(b3)
@@ -165,16 +172,16 @@
 
 
 def OP_FALSE(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Puts a null byte onto the queue."""
     queue.put(b'\x00')
 
 def OP_TRUE(tape: Tape, queue: LifoQueue, cache: dict) -> None:
-    """Puts a 0x01 byte onto the queue."""
-    queue.put(b'\x01')
+    """Puts a 0xFF byte onto the queue."""
+    queue.put(b'\xff')
 
 def OP_PUSH0(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Read the next byte from the tape; put it onto the queue.
     """
     queue.put(tape.read(1))
 
 def OP_PUSH1(tape: Tape, queue: LifoQueue, cache: dict) -> None:
@@ -546,15 +553,15 @@
     sert(bytes_to_bool(queue.get(False)), 'OP_VERIFY check failed')
 
 def OP_EQUAL(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Pull 2 items from the queue; compare them; put the bool result
         onto the queue.
     """
     item1, item2 = queue.get(False), queue.get(False)
-    queue.put(b'\x01' if bytes_are_same(item1, item2) else b'\x00')
+    queue.put(b'\xff' if bytes_are_same(item1, item2) else b'\x00')
 
 def OP_EQUAL_VERIFY(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Runs OP_EQUAL then OP_VERIFY."""
     OP_EQUAL(tape, queue, cache)
     OP_VERIFY(tape, queue, cache)
 
 def OP_CHECK_SIG(tape: Tape, queue: LifoQueue, cache: dict) -> None:
@@ -625,15 +632,15 @@
     if 'sigfield7' in cache and not sig_flag7:
         message += cache['sigfield7']
     if 'sigfield8' in cache and not sig_flag8:
         message += cache['sigfield8']
 
     try:
         vkey.verify(message, sig)
-        queue.put(b'\x01')
+        queue.put(b'\xff')
     except BadSignatureError:
         queue.put(b'\x00')
 
 def OP_CHECK_SIG_VERIFY(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Runs OP_CHECK_SIG, then OP_VERIFY."""
     OP_CHECK_SIG(tape, queue, cache)
     OP_VERIFY(tape, queue, cache)
@@ -664,15 +671,15 @@
     difference = cache['timestamp'] - int(time())
     if cache['timestamp'] < constraint:
         queue.put(b'\x00')
     elif difference >= tape.flags['ts_threshold'] and \
         tape.flags['ts_threshold'] > 0:
         queue.put(b'\x00')
     else:
-        queue.put(b'\x01')
+        queue.put(b'\xff')
 
 def OP_CHECK_TIMESTAMP_VERIFY(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Runs OP_CHECK_TIMESTAMP, then OP_VERIFY."""
     OP_CHECK_TIMESTAMP(tape, queue, cache)
     OP_VERIFY(tape, queue, cache)
 
 def OP_CHECK_EPOCH(tape: Tape, queue: LifoQueue, cache: dict) -> None:
@@ -692,15 +699,15 @@
         'OP_CHECK_EPOCH malformed epoch_threshold flag')
     sert(tape.flags['epoch_threshold'] >= 0,
         'OP_CHECK_EPOCH malformed epoch_threshold flag')
 
     if constraint - int(time()) >= tape.flags['epoch_threshold']:
         queue.put(b'\x00')
     else:
-        queue.put(b'\x01')
+        queue.put(b'\xff')
 
 def OP_CHECK_EPOCH_VERIFY(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Runs OP_CHECK_EPOCH, then OP_VERIFY."""
     OP_CHECK_EPOCH(tape, queue, cache)
     OP_VERIFY(tape, queue, cache)
 
 def OP_DEF(tape: Tape, queue: LifoQueue, cache: dict) -> None:
@@ -815,19 +822,19 @@
     if 'returned' in cache:
         if 'eval_return' in tape.flags and tape.flags['eval_return']:
             OP_RETURN(tape, queue, cache)
         else:
             del cache['returned']
 
 def OP_NOT(tape: Tape, queue: LifoQueue, cache: dict) -> None:
-    """Pulls a value from the queue, interpreting as a bool; performs
-        logical NOT operation; puts that value onto the queue.
+    """Pulls a value from the queue; performs bitwise NOT operation;
+        puts result onto the queue.
     """
     item = queue.get(False)
-    queue.put(b'\x01' if item == b'\x00' else b'\x00')
+    queue.put(not_bytes(item))
 
 def OP_RANDOM(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Read the next byte from the tape, interpreting as an unsigned int;
         put that many random bytes onto the queue.
     """
     size = int.from_bytes(tape.read(1), 'big')
     queue.put(token_bytes(size), False)
@@ -992,15 +999,15 @@
             all_proofs_valid = False
         if len(constraint) and not verify_txn_constraint(txn_proofs[i], constraint):
             all_proofs_valid = False
 
     # calculate aggregate
     aggregate = calc_txn_aggregates(txn_proofs, scope=destination)[destination]
 
-    queue.put(b'\x01' if all_proofs_valid and amount <= aggregate else b'\x00')
+    queue.put(b'\xff' if all_proofs_valid and amount <= aggregate else b'\x00')
 
 def OP_MERKLEVAL(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Read 32 bytes from the tape as the root digest; pull a bool from
         the queue; call OP_DUP then OP_SHA256; call OP_SWAP 1 2; if not
         bool, call OP_SWAP2; call OP_CONCAT; call OP_SHA256; push root
         hash onto the queue; call OP_EQUAL_VERIFY; call OP_EVAL.
     """
@@ -1059,23 +1066,23 @@
 
 def OP_LESS(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Pull two signed ints val1 and val2 from queue; put (v1<v2) onto
         queue.
     """
     val1 = bytes_to_int(queue.get(False))
     val2 = bytes_to_int(queue.get(False))
-    queue.put(b'\x01' if val1 < val2 else b'\x00')
+    queue.put(b'\xff' if val1 < val2 else b'\x00')
 
 def OP_LESS_OR_EQUAL(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Pull two signed ints val1 and val2 from queue; put (v1<=v2) onto
         queue.
     """
     val1 = bytes_to_int(queue.get(False))
     val2 = bytes_to_int(queue.get(False))
-    queue.put(b'\x01' if val1 <= val2 else b'\x00')
+    queue.put(b'\xff' if val1 <= val2 else b'\x00')
 
 def OP_GET_VALUE(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Read one byte from the tape as uint size; read size bytes from
         the tape, interpreting as utf-8 string; put the read-only cache
         value(s) at that cache key onto the queue, serialized as bytes.
     """
     size = tape.read(1)[0]
@@ -1092,21 +1099,21 @@
         elif type(val) is float:
             queue.put(float_to_bytes(val))
 
 def OP_FLOAT_LESS(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Pull two floats val1 and val2 from queue; put (v1<v2) onto queue."""
     val1 = bytes_to_float(queue.get(False))
     val2 = bytes_to_float(queue.get(False))
-    queue.put(b'\x01' if val1 < val2 else b'\x00')
+    queue.put(b'\xff' if val1 < val2 else b'\x00')
 
 def OP_FLOAT_LESS_OR_EQUAL(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Pull two floats val1 and val2 from queue; put (v1<=v2) onto queue."""
     val1 = bytes_to_float(queue.get(False))
     val2 = bytes_to_float(queue.get(False))
-    queue.put(b'\x01' if val1 <= val2 else b'\x00')
+    queue.put(b'\xff' if val1 <= val2 else b'\x00')
 
 def OP_INT_TO_FLOAT(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Pull a signed int from the queue and put it back as a float."""
     value = bytes_to_int(queue.get(False))
     queue.put(float_to_bytes(1.0 * value))
 
 def OP_FLOAT_TO_INT(tape: Tape, queue: LifoQueue, cache: dict) -> None:
@@ -1166,15 +1173,15 @@
             result = bytes_to_bool(queue.get(False))
             if result:
                 vkeys.remove(vkey)
                 confirmed.add(sig)
                 break
 
     if len(confirmed) == len(sigs):
-        queue.put(b'\x01')
+        queue.put(b'\xff')
     else:
         queue.put(b'\x00')
 
 def OP_CHECK_MULTISIG_VERIFY(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Runs OP_CHECK_MULTISIG then OP_VERIFY."""
     OP_CHECK_MULTISIG(tape, queue, cache)
     OP_VERIFY(tape, queue, cache)
@@ -1421,15 +1428,15 @@
     R = queue.get(False)
     sa = queue.get(False)
     sa_G = nacl.bindings.crypto_scalarmult_ed25519_base_noclamp(sa) # sa_G = G^sa
     RT = aggregate_points((R, T)) # R + T
     ca = clamp_scalar(H_small(RT, X, m)) # H(R + T || X || m)
     caX = nacl.bindings.crypto_scalarmult_ed25519_noclamp(ca, X) # X^H(R + T || X || m)
     RcaX = aggregate_points((R, caX)) # R + X^H(R + T || X || m)
-    queue.put(b'\x01' if bytes_are_same(sa_G, RcaX) else b'\x00')
+    queue.put(b'\xff' if bytes_are_same(sa_G, RcaX) else b'\x00')
 
 def OP_DECRYPT_ADAPTER_SIG(tape: Tape, queue: LifoQueue, cache: dict) -> None:
     """Takes tweak scalar t, nonce point R, and signature adapter sa
         from queue; calculates nonce RT; decrypts signature s from sa;
         puts s onto queue; puts RT onto the queue; sets cache keys b's'
         to s if tape.flags[9] and b'RT' to RT if tape.flags[7] (can be
         used in code with @s and @RT).
@@ -1553,21 +1560,23 @@
         message += cache['sigfield7']
     if 'sigfield8' in cache and not sig_flag8:
         message += cache['sigfield8']
 
     queue.put(message)
 
 def NOP(tape: Tape, queue: LifoQueue, cache: dict) -> None:
-    """Read the next byte from the tape, interpreting as an unsigned int
+    """Read the next byte from the tape, interpreting as a signed int
         and pull that many values from the queue. Does nothing with the
         values. Useful for later soft-forks by redefining byte codes.
+        Raises ScriptExecutionError if count is negative.
     """
-    size = int.from_bytes(tape.read(1), 'big')
+    count = bytes_to_int(tape.read(1))
+    sert(count >= 0, 'NOP count must not be negative')
 
-    for _ in range(size):
+    for _ in range(count):
         queue.get(False)
 
 
 opcodes = [
     ('OP_FALSE', OP_FALSE),
     ('OP_TRUE', OP_TRUE),
     ('OP_PUSH0', OP_PUSH0),
@@ -1854,20 +1863,19 @@
             op = opcodes[op_code][1]
         else:
             op = nopcodes[op_code][1]
         op(tape, queue, cache)
 
 def run_auth_script(script: bytes, cache_vals: dict = {}, contracts: dict = {}) -> bool:
     """Run the given auth script byte code. Returns True iff the queue
-        has a single \\x01 value after script execution and no errors were
+        has a single \\xff value after script execution and no errors were
         raised; otherwise, returns False.
     """
     try:
         tape, queue, cache = run_script(script, cache_vals, contracts)
         assert tape.has_terminated()
-        assert not queue.empty()
+        assert queue.qsize() == 1
         item = queue.get(False)
-        assert item == b'\x01'
-        assert queue.empty()
+        assert item == b'\xff'
         return True
     except BaseException as e:
         return False
```

### Comparing `tapescript-0.4.0/tapescript/interfaces.py` & `tapescript-0.4.1/tapescript/interfaces.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tapescript/notes.md` & `tapescript-0.4.1/tapescript/notes.md`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tapescript/parsing.py` & `tapescript-0.4.1/tapescript/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,22 +194,18 @@
     symbols_to_advance += 1
     val = symbols[0]
     yert(val[0].lower() in ('d', 'x', 's'),
         'values for OP_PUSH must be prefaced with d, x, or s')
 
     match val[0].lower():
         case 'd':
-            vert(val[1:].isnumeric(),
+            vert(val[1:].isnumeric() or (val[1] == '-' and val[2:].isnumeric()),
                 'value prefaced by d must be decimal int')
-            if '.' in val:
-                val = int(val[1:].split('.')[0])
-            else:
-                val = int(val[1:])
-            size = ceil(log2(val+1)/8) or 1
-            val = val.to_bytes(size, 'big')
+            val = int(val[1:].split('.')[0])
+            val = int_to_bytes(val)
         case 'x':
             val = bytes.fromhex(val[1:])
         case 's':
             if val[1] == '"' and '"' in val[2:]:
                 last_idx = val[2:].index('"')
                 val = bytes(val[2:last_idx+2], 'utf-8')
             elif val[1] == "'" and "'" in val[2:]:
@@ -290,20 +286,19 @@
     symbols_to_advance += 1
     val = symbols[0]
     yert(val[0].lower() in ('d', 'x'),
         f'{opname} - numeric args must be prefaced with d or x; {val} is invalid - symbol {symbol_index}')
 
     match val[0].lower():
         case 'd':
-            vert(val[1:].isnumeric(),
+            vert(val[1:].lstrip('+-').isnumeric(),
                 f'{opname} - value prefaced by d must be decimal int; {val} is invalid - symbol {symbol_index}')
-            if '.' in val:
-                args.append(int(val[1:].split('.')[0]).to_bytes(1, 'big'))
-            else:
-                args.append(int(val[1:]).to_bytes(1, 'big'))
+            val = int_to_bytes(int(val[1:].split('.')[0]))
+            assert len(val) == 1, 'value overflow'
+            args.append(val)
         case 'x':
             vert(len(val[1:]) <= 2,
                 f'{opname} - value must be at most 1 byte long; {val} is invalid - symbol {symbol_index}')
             val = bytes.fromhex(val[1:])
             args.append(val if len(val) == 1 else b'\x00')
     return (symbols_to_advance, args)
 
@@ -324,27 +319,31 @@
             symbols_to_advance += 1
             val = symbols[0]
     else:
         # human-readable syntax of OP_[whatever] [key]
         symbols_to_advance += 1
         val = symbols[0]
 
-    yert(val[0].lower() in ('d', 'x', 's'),
-        f'values for {opname} must be prefaced with d, x, or s; {val} is invalid - symbol {symbol_index}')
+    yert(val[0].lower() in ('d', 'f', 'x', 's'),
+        f'values for {opname} must be prefaced with d, x, or s; {val} is invalid'
+        f' - symbol {symbol_index}')
     match val[0].lower():
         case 'd':
-            vert(val[1:].lstrip('+-').isnumeric(),
-                f'{opname} - value prefaced by d must be decimal int or float; {val} is invalid - symbol {symbol_index}')
-            if '.' in val:
-                args.append((4).to_bytes(1, 'big'))
-                args.append(struct.pack('!f', float(val[1:])))
-            else:
-                val = int_to_bytes(int(val[1:]))
-                args.append(len(val).to_bytes(1, 'big'))
-                args.append(val)
+            vert(val[1:].lstrip('+-').replace('.','').isnumeric(),
+                f'{opname} - value prefaced by d must be decimal int; '
+                f'{val} is invalid - symbol {symbol_index}')
+            val = int_to_bytes(int(val[1:].split('.')[0]))
+            args.append(len(val).to_bytes(1, 'big'))
+            args.append(val)
+        case 'f':
+            vert(val[1:].lstrip('+-').replace('.','').isnumeric(),
+                f'{opname} - value prefaced by f must be decimal float; '
+                f'{val} is invalid - symbol {symbol_index}')
+            args.append((4).to_bytes(1, 'big'))
+            args.append(struct.pack('!f', float(val[1:])))
         case 'x':
             val = bytes.fromhex(val[1:])
             args.append(len(val).to_bytes(1, 'big'))
             args.append(val)
         case 's':
             if val[1] == '"' and '"' in val[2:]:
                 last_idx = val[2:].index('"')
@@ -376,39 +375,46 @@
             symbols_to_advance += 1
             val = symbols[0]
     else:
         # human-readable syntax of OP_[whatever] [key]
         symbols_to_advance += 1
         val = symbols[0]
 
-    yert(val[0].lower() in ('d', 'x', 's'),
-        f'{opname} - values for OP_PUSH2 must be prefaced with d, x, or s; {val} is invalid - symbol {symbol_index}')
+    yert(val[0].lower() in ('d', 'f', 'x', 's'),
+        f'{opname} - values for OP_PUSH2 must be prefaced with d, f, x, or s; '
+        f'{val} is invalid - symbol {symbol_index}')
 
     match val[0].lower():
         case 's':
             if val[1] == '"' and '"' in val[2:]:
                 last_idx = val[2:].index('"')
                 val = bytes(val[2:last_idx+2], 'utf-8')
             elif val[1] == "'" and "'" in val[2:]:
                 last_idx = val[2:].index("'")
                 val = bytes(val[2:last_idx+2], 'utf-8')
             else:
                 val = bytes(val[1:], 'utf-8')
         case 'd':
             vert(val[1:].lstrip('+-').isnumeric(),
-                f'{opname} - value prefaced by d must be decimal int; {val} is invalid - symbol {symbol_index}')
-            if '.' in val:
-                val = int_to_bytes(int(val[1:].split('.')[0]))
-            else:
-                val = int_to_bytes(int(val[1:]))
-            vert(len(val) < 65_536, f'OP_PUSH2 value overflow; {val} is invalid - symbol {symbol_index}')
+                f'{opname} - value prefaced by d must be decimal int; {val} is '
+                f'invalid - symbol {symbol_index}')
+            val = int_to_bytes(int(val[1:].split('.')[0]))
+            vert(len(val) < 65_536, f'OP_PUSH2 value overflow; {bytes_to_int(val)}'
+                 f' is invalid - symbol {symbol_index}')
+        case 'f':
+            vert(val[1:].lstrip('+-').replace('.','').isnumeric(),
+                f'{opname} - value prefaced by f must be decimal float; '
+                f'{val} is invalid - symbol {symbol_index}')
+            args.append((4).to_bytes(1, 'big'))
+            args.append(struct.pack('!f', float(val[1:])))
         case 'x':
             val = bytes.fromhex(val[1:])
             vert(len(val) < 65_536,
-                f'x-value for OP_PUSH2 must be at most 65_535 bytes long - symbol {symbol_index}')
+                f'x-value for OP_PUSH2 must be at most 65_535 bytes long - '
+                f'symbol {symbol_index}')
     args.append(len(val).to_bytes(2, 'big'))
     args.append(val)
     return (symbols_to_advance, args)
 
 def _get_OP_PUSH4_args(
         opname: str, symbols: list[str], symbols_to_advance: int,
         symbol_index: int
@@ -448,14 +454,20 @@
         case 'd':
             vert(val[1:].lstrip('+-').isnumeric(),
                 f'{opname} - value prefaced by d must be decimal int - symbol {symbol_index}')
             if '.' in val:
                 val = int_to_bytes(int(val[1:].split('.')[0]))
             else:
                 val = int_to_bytes(int(val[1:]))
+        case 'f':
+            vert(val[1:].lstrip('+-').replace('.','').isnumeric(),
+                f'{opname} - value prefaced by f must be decimal float; '
+                f'{val} is invalid - symbol {symbol_index}')
+            args.append((4).to_bytes(1, 'big'))
+            args.append(struct.pack('!f', float(val[1:])))
         case 'x':
             val = bytes.fromhex(val[1:])
             vert(len(val) < 2**32,
                 f'x-value for {opname} must be at most 4_294_967_295 bytes long - symbol {symbol_index}')
     args.append(len(val).to_bytes(4, 'big'))
     args.append(val)
     return (symbols_to_advance, args)
@@ -463,21 +475,21 @@
 def _get_OP_DIV_FLOAT_args(
         opname: str, symbols: list[str], symbols_to_advance: int,
         symbol_index: int
     ) -> tuple[int, tuple[bytes]]:
     args = []
     symbols_to_advance += 1
     val = symbols[0]
-    yert(val[0].lower() in ('d', 'x'),
-        f'{opname} - numeric args must be prefaced with d or x; {val} is invalid - symbol {symbol_index}')
+    yert(val[0].lower() in ('f', 'x'),
+        f'{opname} - numeric args must be prefaced with f or x; {val} is invalid - symbol {symbol_index}')
 
     match val[0].lower():
-        case 'd':
+        case 'f':
             vert(val[1:].lstrip('+-').isnumeric(),
-                f'{opname} - value prefaced by d must be decimal float; {val} is invalid - symbol {symbol_index}')
+                f'{opname} - value prefaced by f must be decimal float; {val} is invalid - symbol {symbol_index}')
             args.append(struct.pack('!f', float(val[1:])))
         case 'x':
             vert(len(val[1:]) == 8,
                 f'{opname} - value prefaced by x must be 8 long (4 bytes); {val} is invalid - symbol {symbol_index}')
             args.append(bytes.fromhex(val[1:]))
     return (symbols_to_advance, args)
 
@@ -594,15 +606,15 @@
         case 'OP_PUSH0' | 'OP_POP1' | 'OP_ADD_INTS' | 'OP_SUBTRACT_INTS' | \
             'OP_MULT_INTS' | 'OP_ADD_FLOATS' | \
             'OP_SUBTRACT_FLOATS' | 'OP_ADD_POINTS' | 'OP_CALL' | \
             'OP_COPY' | 'OP_SHAKE256' | 'OP_RANDOM' | 'OP_REVERSE' | \
             'OP_SPLIT' | 'OP_SPLIT_STR' | 'OP_CHECK_SIG' | 'OP_SIGN' | \
             'OP_CHECK_SIG_VERIFY' | 'OP_CLAMP_SCALAR' | 'OP_ADD_SCALARS' | \
             'OP_SUBTRACT_SCALARS' | 'OP_SUBTRACT_POINTS' | 'OP_GET_MESSAGE':
-            # ops that have tape argument of form [0-255]
+            # ops that have tape argument of form [-128 to 127]
             # human-readable syntax of OP_[whatever] [int]
             return _get_OP_PUSH0_type_args(opname, symbols, symbols_to_advance, symbol_index)
         case 'OP_PUSH2':
             # ops that have tape argument of form [0-65535] [val]
             # human-readable syntax of simply OP_PUSH2 [val]
             return _get_OP_PUSH2_args(opname, symbols, symbols_to_advance, symbol_index)
         case 'OP_PUSH4':
@@ -1154,31 +1166,31 @@
                 'OP_MULT_INTS' | 'OP_ADD_FLOATS' | \
                 'OP_SUBTRACT_FLOATS' | 'OP_ADD_POINTS' | 'OP_CALL' | \
                 'OP_COPY' | 'OP_SHAKE256' | 'OP_RANDOM' | 'OP_REVERSE' | \
                 'OP_SPLIT' | 'OP_SPLIT_STR' | 'OP_CLAMP_SCALAR' | \
                 'OP_ADD_SCALARS' | 'OP_SUBTRACT_SCALARS' | 'OP_SUBTRACT_POINTS':
                 # ops that have tape argument of form [0-255]
                 # human-readable syntax of OP_[whatever] [int]
-                val = tape.read(1)[0]
+                val = bytes_to_int(tape.read(1))
                 add_line(f'{op_name} d{val}')
             case 'OP_CHECK_SIG' | 'OP_CHECK_SIG_VERIFY' | 'OP_SIGN' | 'OP_GET_MESSAGE':
                 # ops that have tape argument of form x[00-ff]
                 # human-readable syntax of OP_[whatever] x[00-ff]
                 val = tape.read(1)
                 add_line(f'{op_name} x{val.hex()}')
             case 'OP_PUSH2':
                 # ops that have tape argument of form [0-65535] [val]
                 # human-readable syntax of simply OP_PUSH2 [val]
-                size = int.from_bytes(tape.read(2), 'big')
+                size = bytes_to_int(tape.read(2))
                 val = tape.read(size)
                 add_line(f'{op_name} d{size} x{val.hex()}')
             case 'OP_PUSH4':
                 # ops that have tape argument of form [0-4_294_967_295] [val]
                 # human-readable syntax of simply OP_PUSH4 [val]
-                size = int.from_bytes(tape.read(4), 'big')
+                size = bytes_to_int(tape.read(4))
                 val = tape.read(size)
                 add_line(f'{op_name} d{size} x{val.hex()}')
             case 'OP_DIV_FLOAT' | 'OP_MOD_FLOAT':
                 # ops that have tape argument of form [4-byte float]
                 # human-readable syntax of OP_[DIV|MOD]_FLOAT [val]
                 val = tape.read(4)
                 add_line(f'{op_name} x{val.hex()}')
```

### Comparing `tapescript-0.4.0/tapescript/tools.py` & `tapescript-0.4.1/tapescript/tools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/test_classes.py` & `tapescript-0.4.1/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/test_e2e_eltoo.py` & `tapescript-0.4.1/tests/test_e2e_eltoo.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/test_functions.py` & `tapescript-0.4.1/tests/test_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
     def test_OP_TRUE_puts_nonnull_byte_onto_queue(self):
         assert self.queue.empty()
         assert not len(self.cache.keys())
         functions.OP_TRUE(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         assert not len(self.cache.keys())
-        assert self.queue.get() == b'\x01'
+        assert functions.bytes_to_bool(self.queue.get())
 
     def test_OP_PUSH0_puts_next_byte_from_tape_onto_queue(self):
         self.tape = classes.Tape(b'123')
         assert self.queue.empty()
         assert not len(self.cache.keys())
         functions.OP_PUSH0(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
@@ -655,15 +655,15 @@
         self.queue.put(b'12323')
         functions.OP_VERIFY(self.tape, self.queue, self.cache)
 
     def test_OP_EQUAL_compares_two_values_from_queue_and_puts_bool_on_queue(self):
         self.queue.put(b'123')
         self.queue.put(b'123')
         functions.OP_EQUAL(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
 
         self.queue.put(b'321')
         self.queue.put(b'123')
         functions.OP_EQUAL(self.tape, self.queue, self.cache)
         assert self.queue.get(False) == b'\x00'
 
     def test_OP_EQUAL_VERIFY_runs_OP_EQUAL_then_OP_VERIFY(self):
@@ -689,15 +689,15 @@
         self.tape = classes.Tape(b'\x00')
         assert self.queue.empty()
         self.queue.put(sig)
         self.queue.put(bytes(vkey))
         self.cache['sigfield1'] = body
         functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
         assert self.queue.empty()
 
     def test_OP_CHECK_SIG_sigflag_omits_sigfields(self):
         field1 = b'hello'
         field3 = b' '
         field8 = b'world'
         body = field1 + field3 + field8
@@ -717,15 +717,15 @@
         self.cache['sigfield4'] = b'should be ignored'
         self.cache['sigfield5'] = b'should be ignored'
         self.cache['sigfield6'] = b'should be ignored'
         self.cache['sigfield7'] = b'should be ignored'
         self.cache['sigfield8'] = field8
         functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
         assert self.queue.empty()
 
     def test_OP_CHECK_SIG_errors_on_invalid_vkey_or_sig(self):
         self.tape = classes.Tape(b'\x00')
         self.queue.put(b''.join(b'\xff' for _ in range(64)))
         self.queue.put(b'not a valid vkey')
         with self.assertRaises(ValueError) as e:
@@ -825,15 +825,15 @@
     def test_OP_CHECK_TIMESTAMP_compares_top_queue_int_to_cache_timestamp(self):
         assert self.queue.empty()
         self.tape.flags['ts_threshold'] = 10
         self.cache['timestamp'] = int(time())
         self.queue.put(int(time()).to_bytes(4, 'big'))
         functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
 
         assert self.queue.empty()
         self.cache['timestamp'] = int(time())-1
         self.queue.put(int(time()).to_bytes(4, 'big'))
         functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         item = self.queue.get(False)
@@ -850,15 +850,15 @@
         assert self.queue.empty()
         self.tape.flags['ts_threshold'] = 100
         self.cache['timestamp'] = int(time())+12
         self.queue.put(int(time()).to_bytes(4, 'big'))
         functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         item = self.queue.get(False)
-        assert item == b'\x01'
+        assert item == b'\xff'
 
     def test_OP_CHECK_TIMESTAMP_VERIFY_runs_OP_CHECK_TIMESTAMP_then_OP_VERIFY(self):
         assert self.queue.empty()
         self.tape = classes.Tape(b'', flags={'ts_threshold': 10})
         self.cache['timestamp'] = int(time())
         self.queue.put(int(time()).to_bytes(4, 'big'))
         functions.OP_CHECK_TIMESTAMP_VERIFY(self.tape, self.queue, self.cache)
@@ -910,30 +910,30 @@
 
     def test_OP_CHCECK_EPOCH_compares_current_time_to_constraint(self):
         assert self.queue.empty()
         self.tape.flags['epoch_threshold'] = 0
         self.queue.put(int(time()-10).to_bytes(4, 'big'))
         functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
 
         assert self.queue.empty()
         self.queue.put(int(time()+10).to_bytes(4, 'big'))
         functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         item = self.queue.get(False)
         assert item == b'\x00'
 
         assert self.queue.empty()
         self.tape.flags['epoch_threshold'] = 100
         self.queue.put(int(time()+10).to_bytes(4, 'big'))
         functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         item = self.queue.get(False)
-        assert item == b'\x01'
+        assert item == b'\xff'
 
     def test_OP_CHECK_EPOCH_VERIFY_runs_OP_CHECK_EPOCH_then_OP_VERIFY(self):
         assert self.queue.empty()
         self.tape.flags['epoch_threshold'] = 0
         self.queue.put(int(time()-10).to_bytes(4, 'big'))
         functions.OP_CHECK_EPOCH_VERIFY(self.tape, self.queue, self.cache)
         assert self.queue.empty()
@@ -958,26 +958,38 @@
         assert b'\x00' in self.tape.definitions
         assert isinstance(self.tape.definitions[b'\x00'], classes.Tape)
         assert self.tape.definitions[b'\x00'].data == b'hello world'
         assert self.queue.empty()
 
     def test_OP_NOT_inverts_bool_value_of_top_queue_value(self):
         assert self.queue.empty()
-        self.queue.put(b'\x01')
+        self.queue.put(b'\xFF')
         functions.OP_NOT(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         assert self.queue.get(False) == b'\x00'
 
         assert self.queue.empty()
         self.queue.put(b'\x00')
         functions.OP_NOT(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xFF'
         assert self.queue.empty()
 
+    def test_OP_NOT_inverts_bytestring_on_top_of_queue(self):
+        self.queue.put(b'\xf0\x0f')
+        functions.OP_NOT(self.tape, self.queue, self.cache)
+        assert self.queue.get(False) == b'\x0f\xf0'
+
+        data = token_bytes(4)
+        self.queue.put(data)
+        functions.OP_DUP(self.tape, self.queue, self.cache)
+        functions.OP_NOT(self.tape, self.queue, self.cache)
+        functions.OP_XOR(self.tape, self.queue, self.cache)
+        assert self.queue.get(False) == b'\xff\xff\xff\xff'
+
     def test_OP_RANDOM_puts_random_bytes_on_queue(self):
         assert self.queue.empty()
         n_bytes = randint(1, 250)
         self.tape = classes.Tape(n_bytes.to_bytes(1, 'big'))
         functions.OP_RANDOM(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         item = self.queue.get(False)
@@ -1130,24 +1142,29 @@
     def test_OP_SPLIT_STR_raises_ScriptExecutionError_for_str_length_overflow(self):
         self.queue.put(b'sds')
         self.tape = classes.Tape(b'\xff')
         with self.assertRaises(errors.ScriptExecutionError) as e:
             functions.OP_SPLIT_STR(self.tape, self.queue, self.cache)
         assert str(e.exception) == 'OP_SPLIT_STR item len exceeded by index'
 
-    def test_NOP_reads_uint_from_tape_and_pulls_that_many_items_from_queue(self):
+    def test_NOP_reads_int_from_tape_and_pulls_that_many_items_from_queue(self):
         assert self.queue.empty()
         self.queue.put(1)
         self.queue.put(2)
         self.queue.put(3)
-        self.tape = classes.Tape(b'\x02')
+        self.tape = classes.Tape(functions.int_to_bytes(2))
         functions.NOP(self.tape, self.queue, self.cache)
         assert self.queue.get(False) == 1
         assert self.queue.empty()
 
+    def test_NOP_raises_ScriptExecutionError_for_negative_count(self):
+        self.tape = classes.Tape(functions.int_to_bytes(-2))
+        with self.assertRaises(errors.ScriptExecutionError) as e:
+            functions.NOP(self.tape, self.queue, self.cache)
+
     def test_OP_CHECK_TRANSFER_errors_on_missing_or_invalid_contract_or_params(self):
         def setup_transfer():
             self.tape = classes.Tape(b'\x01')
             self.queue.put(b'txn_proof')
             self.queue.put(b'source')
             self.queue.put(b'\x01')
             self.queue.put(b'destination')
@@ -1177,38 +1194,38 @@
             self.queue.put((10).to_bytes(1, 'big')) # amount
             self.queue.put(b'contractid')
 
         amount = 10
         setup_transfer()
         self.tape.contracts[b'contractid'] = ValidContract(amount)
         functions.OP_CHECK_TRANSFER(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
         assert self.queue.empty()
 
         amount = 9
         setup_transfer()
         self.tape.contracts[b'contractid'] = ValidContract(amount)
         functions.OP_CHECK_TRANSFER(self.tape, self.queue, self.cache)
         assert self.queue.get(False) == b'\x00'
         assert self.queue.empty()
 
         amount = 11
         setup_transfer()
         self.tape.contracts[b'contractid'] = ValidContract(amount)
         functions.OP_CHECK_TRANSFER(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
         assert self.queue.empty()
 
     def test_OP_CALL_reads_uint_from_tape_and_runs_that_definition(self):
         self.tape = classes.Tape(b'\x00')
         self.tape.definitions[b'\x00'] = classes.Tape(b'\x01')
         assert self.queue.empty()
         functions.OP_CALL(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
 
     def test_OP_CALL_raises_ScriptExecutionError_when_callstack_limit_exceeded(self):
         self.tape.callstack_limit = -1
         self.tape.callstack_count = 1
         with self.assertRaises(errors.ScriptExecutionError) as e:
             functions.OP_CALL(self.tape, self.queue, self.cache)
         assert str(e.exception) == 'callstack limit exceeded'
@@ -1218,15 +1235,16 @@
         subtape = classes.Tape(b'\x2b\x00\x03\x00\x2a\x00\x02\x03')
         self.tape.definitions[b'\x00'] = subtape
         subtape.definitions = self.tape.definitions
         assert self.queue.empty()
         self.queue.put(b'\x01', False)
         functions.OP_CALL(self.tape, self.queue, self.cache)
         assert self.tape.definitions[b'\x00'].pointer == 0
-        assert not self.queue.empty()
+        assert self.queue.qsize() == 2
+        assert self.queue.get(False) == b'\x03'
         assert self.queue.get(False) == b'\x03'
 
     def test_OP_IF_reads_2uint_length_from_tape_pulls_top_queue_bool_and_executes_if_true(self):
         length = b'\x00\x02'
         op_push0 = b'\x02'
         self.tape = classes.Tape(length + op_push0 + b'X')
         assert self.queue.empty()
@@ -1278,15 +1296,15 @@
         assert b'E' in self.cache
         assert len(self.cache[b'E']) == 1
         exname, exstr = str(self.cache[b'E'][0], 'utf-8').split('|')
         assert exname == 'ScriptExecutionError'
         assert exstr == 'OP_VERIFY check failed'
         assert not self.queue.empty()
         item = self.queue.get(False)
-        assert item == b'\x01'
+        assert functions.bytes_to_bool(item)
 
     def test_OP_EVAL_pulls_value_from_queue_and_runs_as_script(self):
         code = b'\x02F'
         assert self.queue.empty()
         self.queue.put(code)
         functions.OP_EVAL(self.tape, self.queue, self.cache)
         assert self.tape.has_terminated()
@@ -1310,15 +1328,15 @@
         committed_branch_a = b'\x02A'
         committed_branch_b = b'\x02B'
         commitment_a = sha256(committed_branch_a).digest()
         commitment_b = sha256(committed_branch_b).digest()
         commitment_root = sha256(commitment_a + commitment_b).digest()
         self.queue.put(commitment_b)
         self.queue.put(committed_branch_a)
-        self.queue.put(b'\x01')
+        self.queue.put(b'\xff')
         self.tape = classes.Tape(commitment_root)
         functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         assert self.queue.get(False) == b'A'
         assert self.queue.empty()
 
         self.queue.put(commitment_a)
@@ -1340,24 +1358,24 @@
         commitment_b_root = sha256(commitment_ba + commitment_bb).digest()
         committed_branch_b_root = b'\x3c' + commitment_b_root
         commitment_b = sha256(committed_branch_b_root).digest()
 
         commitment_root = sha256(commitment_a + commitment_b).digest()
         self.queue.put(commitment_b)
         self.queue.put(committed_branch_a)
-        self.queue.put(b'\x01')
+        self.queue.put(b'\xff')
         self.tape = classes.Tape(commitment_root)
         functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         assert self.queue.get(False) == b'A'
         assert self.queue.empty()
 
         self.queue.put(commitment_bb)
         self.queue.put(committed_branch_ba)
-        self.queue.put(b'\x01')
+        self.queue.put(b'\xff')
         self.queue.put(commitment_a)
         self.queue.put(committed_branch_b_root)
         self.queue.put(b'\x00')
         self.tape = classes.Tape(commitment_root)
         functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
         assert not self.queue.empty()
         assert self.queue.get(False) == b'BA'
@@ -1379,15 +1397,15 @@
         committed_branch_a = b'\x02A'
         committed_branch_b = b'\x02B'
         commitment_a = sha256(committed_branch_a).digest()
         commitment_b = sha256(committed_branch_b).digest()
         commitment_root = sha256(commitment_a + commitment_b).digest()
         self.queue.put(commitment_b)
         self.queue.put(committed_branch_a + b'uncommitted code')
-        self.queue.put(b'\x01')
+        self.queue.put(b'\xff')
         self.tape = classes.Tape(commitment_root)
 
         with self.assertRaises(errors.ScriptExecutionError) as e:
             functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
         assert str(e.exception) == 'OP_VERIFY check failed'
 
     def test_OP_LESS_pulls_two_ints_from_queue_and_places_bool_on_queue(self):
@@ -1408,15 +1426,15 @@
         assert result == b'\x00'
 
         self.queue.put(val2)
         self.queue.put(val1)
         functions.OP_LESS(self.tape, self.queue, self.cache)
         assert self.queue._qsize() == 1
         result = self.queue.get(False)
-        assert result == b'\x01'
+        assert result == b'\xff'
 
     def test_OP_LESS_OR_EQUAL_pulls_two_ints_from_queue_and_places_bool_on_queue(self):
         val1 = functions.int_to_bytes(123)
         val2 = functions.int_to_bytes(321)
         self.queue.put(val1)
         self.queue.put(val2)
         functions.OP_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
@@ -1425,22 +1443,22 @@
         assert result == b'\x00'
 
         self.queue.put(val1)
         self.queue.put(val1)
         functions.OP_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
         assert self.queue._qsize() == 1
         result = self.queue.get(False)
-        assert result == b'\x01'
+        assert result == b'\xff'
 
         self.queue.put(val2)
         self.queue.put(val1)
         functions.OP_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
         assert self.queue._qsize() == 1
         result = self.queue.get(False)
-        assert result == b'\x01'
+        assert result == b'\xff'
 
     def test_OP_GET_VALUE_pulls_str_from_tape_and_puts_cache_vals_onto_queue(self):
         key = bytes('test', 'utf-8')
         self.cache['test'] = 123
         self.tape.data = functions.int_to_bytes(len(key)) + key
         functions.OP_GET_VALUE(self.tape, self.queue, self.cache)
         assert self.queue.qsize() == 1
@@ -1482,15 +1500,15 @@
         assert result == b'\x00'
 
         self.queue.put(val2)
         self.queue.put(val1)
         functions.OP_FLOAT_LESS(self.tape, self.queue, self.cache)
         assert self.queue._qsize() == 1
         result = self.queue.get(False)
-        assert result == b'\x01'
+        assert result == b'\xff'
 
     def test_OP_FLOAT_LESS_OR_EQUAL_pulls_two_floats_from_queue_and_places_bool_on_queue(self):
         val1 = functions.float_to_bytes(123.0)
         val2 = functions.float_to_bytes(321.0)
         self.queue.put(val1)
         self.queue.put(val2)
         functions.OP_FLOAT_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
@@ -1499,22 +1517,22 @@
         assert result == b'\x00'
 
         self.queue.put(val1)
         self.queue.put(val1)
         functions.OP_FLOAT_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
         assert self.queue._qsize() == 1
         result = self.queue.get(False)
-        assert result == b'\x01'
+        assert result == b'\xff'
 
         self.queue.put(val2)
         self.queue.put(val1)
         functions.OP_FLOAT_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
         assert self.queue._qsize() == 1
         result = self.queue.get(False)
-        assert result == b'\x01'
+        assert result == b'\xff'
 
     def test_OP_INT_TO_FLOAT_works_correctly(self):
         val = functions.int_to_bytes(123)
         self.queue.put(val)
         functions.OP_INT_TO_FLOAT(self.tape, self.queue, self.cache)
         result = self.queue.get(False)
         assert result == functions.float_to_bytes(123 * 1.0)
@@ -1683,15 +1701,15 @@
 
         self.queue.put(sig)
         self.queue.put(bytes(SigningKey(seed).verify_key))
         self.tape.reset()
         functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
         result = self.queue.get(False)
         assert self.queue.qsize() == 0
-        assert result == b'\x01'
+        assert result == b'\xff'
 
     def test_OP_SIGN_raises_error_for_invalid_key(self):
         seed = b'not a valid key length'
         self.tape.data = b'\x00'
         self.queue.put(seed)
         self.cache['sigfield1'] = b'test'
         with self.assertRaises(ValueError) as e:
@@ -1735,15 +1753,15 @@
         sig = skey.sign(msg).signature
 
         self.queue.put(msg)
         self.queue.put(sig)
         self.queue.put(bytes(skey.verify_key))
         functions.OP_CHECK_SIG_QUEUE(self.tape, self.queue, self.cache)
         assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
 
         self.queue.put(msg)
         self.queue.put(sig[1:] + sig[:1])
         self.queue.put(bytes(skey.verify_key))
         functions.OP_CHECK_SIG_QUEUE(self.tape, self.queue, self.cache)
         assert self.queue.qsize() == 1
         assert self.queue.get(False) == b'\x00'
@@ -1859,15 +1877,15 @@
 
         self.tape = classes.Tape(b'\x00')
         self.queue.put(m)
         self.queue.put(sig)
         self.queue.put(X)
         functions.OP_CHECK_SIG_QUEUE(self.tape, self.queue, self.cache)
         assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
 
     def test_OP_SUBTRACT_POINTS_and_OP_SUBTRACT_SCALARS_work_properly(self):
         seed1 = token_bytes(32)
         seed2 = token_bytes(32)
         x1 = functions.derive_key_from_seed(seed1)
         x2 = functions.derive_key_from_seed(seed2)
         x3 = functions.aggregate_scalars([x1, x2])
@@ -1977,15 +1995,15 @@
         self.queue.put(sa)
         self.queue.put(R)
         self.queue.put(m)
         self.queue.put(T)
         self.queue.put(X)
         functions.OP_CHECK_ADAPTER_SIG(self.tape, self.queue, self.cache)
         assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
 
         # negative case
         self.queue.put(sa)
         self.queue.put(R)
         self.queue.put(m + b'qws')
         self.queue.put(T)
         self.queue.put(X)
@@ -2023,15 +2041,15 @@
         self.cache['sigfield1'] = m
         self.tape = classes.Tape(b'\x00')
         functions.set_tape_flags(self.tape)
         self.queue.put(RT + s)
         self.queue.put(X)
         functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
         assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\x01'
+        assert self.queue.get(False) == b'\xff'
 
     # cryptographic proofs
     def test_ed25519_maths_meet_homomorphic_one_way_condition(self):
         """Test if Ed25519 meets the homomorphic one way condition."""
         x1 = functions.clamp_scalar(token_bytes(32))
         x2 = functions.clamp_scalar(token_bytes(32))
         y1 = nacl.bindings.crypto_scalarmult_ed25519_base_noclamp(x1) # G^x1
@@ -2094,15 +2112,17 @@
         self.tape = classes.Tape(code)
         assert self.queue.empty()
         assert not self.cache
         functions.run_tape(self.tape, self.queue, self.cache)
         assert self.tape.has_terminated()
         assert not self.queue.empty()
         item = self.queue.get(False)
-        assert item == b'\x01'
+        assert item == b'\xff'
+        item = self.queue.get(False)
+        assert item == b'\x02'
 
     def test_run_script_returns_tuple_of_tape_queue_and_cache(self):
         code = bytes.fromhex('990099009900990099009900')
         result = functions.run_script(code)
         assert isinstance(result, tuple)
         assert len(result) == 3
         assert isinstance(result[0], classes.Tape)
@@ -2122,22 +2142,22 @@
         assert str(e.exception) == 'callstack limit exceeded'
 
     def test_OP_RETURN_exits_local_context_and_returns_to_outer_context(self):
         # return from def before adding int false to queue
         code = b'\x29\x00\x00\x02\x30\x00\x2a\x00\x01'
         tape, queue, _ = functions.run_script(code)
         assert tape.has_terminated()
-        assert queue.get(False) == b'\x01'
+        assert queue.get(False) == b'\xff'
         assert queue.empty()
 
         # return from def after adding int false to queue
         code = b'\x29\x00\x00\x02\x00\x30\x2a\x00\x01'
         tape, queue, _ = functions.run_script(code)
         assert tape.has_terminated()
-        assert queue.get(False) == b'\x01'
+        assert queue.get(False) == b'\xff'
         assert queue.get(False) == b'\x00'
         assert queue.empty()
 
     def test_OP_RETURN_within_OP_IF_exits_outer_context(self):
         # return from def within OP_IF before adding int false to queue
         code = b'\x29\x00\x00\x06\x2b\x00\x02\x30\x00\x01\x01\x2a\x00\x02\x02'
         tape, queue, _ = functions.run_script(code)
@@ -2226,15 +2246,15 @@
 
         functions.add_opcode(255, 'OP_NONSENSE', lambda tape, queue, cache: queue.put('nonsense'))
         assert self.original_opcodes != functions.opcodes
         assert self.original_opcodes_inverse != functions.opcodes_inverse
 
         tape, queue, cache = functions.run_script(b'\xff\x01')
         assert not queue.empty()
-        assert queue.get(False) == b'\x01'
+        assert queue.get(False) == b'\xff'
         assert queue.get(False) == 'nonsense'
 
     def test_add_contract_raises_error_on_invalid_contract(self):
         assert b'123' not in functions._contracts
         with self.assertRaises(errors.ScriptExecutionError) as e:
             functions.add_contract(b'123', InvalidContract(1))
         assert str(e.exception) == 'contract does not fulfill at least one interface'
@@ -2313,25 +2333,25 @@
             hexdata = ''.join(f.read().split())
             unlocking_script1 = bytes.fromhex(hexdata)
             script = unlocking_script1 + locking_script
             tape, queue, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
             assert not queue.empty()
             item = queue.get(False)
-            assert item == b'\x01'
+            assert item == b'\xff'
 
         with open('tests/vectors/p2pk_unlocking_script2.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script2 = bytes.fromhex(hexdata)
             script = unlocking_script2 + locking_script
             tape, queue, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
             assert not queue.empty()
             item = queue.get(False)
-            assert item == b'\x01'
+            assert item == b'\xff'
 
     def test_p2sh_e2e(self):
         message = b'spending bitcoinz or something'
         original_flags = {**functions.flags}
         # disable additional time check
         functions.flags['ts_threshold'] = 0
         ts = int(time())
@@ -2348,15 +2368,15 @@
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
             tape, queue, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
             assert not queue.empty()
             item = queue.get(False)
-            assert item == b'\x01'
+            assert item == b'\xff'
 
         functions.flags = original_flags
 
     def test_cds_e2e(self):
         original_flags = {**functions.flags}
         # disable additional time check
         functions.flags['ts_threshold'] = 0
@@ -2440,25 +2460,25 @@
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
             tape, queue, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
             assert not queue.empty()
             item = queue.get(False)
-            assert item == b'\x01'
+            assert item == b'\xff'
 
         with open('tests/vectors/correspondent_unlocking_script2.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
             tape, queue, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
             assert not queue.empty()
             item = queue.get(False)
-            assert item == b'\x01'
+            assert item == b'\xff'
 
         functions.flags = original_flags
 
     def test_merkleval_e2e(self):
         message = b'spending some coinz'
         original_flags = {**functions.flags}
         # disable additional time check
@@ -2477,34 +2497,34 @@
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
             tape, queue, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
             assert not queue.empty()
             item = queue.get(False)
-            assert item == b'\x01'
+            assert item == b'\xff'
 
         with open('tests/vectors/merkleval_unlocking_script_ba.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
             tape, queue, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
             assert not queue.empty()
             item = queue.get(False)
-            assert item == b'\x01'
+            assert item == b'\xff'
 
         with open('tests/vectors/merkleval_unlocking_script_bb.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
             tape, queue, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
             assert not queue.empty()
             item = queue.get(False)
-            assert item == b'\x01'
+            assert item == b'\xff'
 
         functions.flags = original_flags
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tapescript-0.4.0/tests/test_parsing.py` & `tapescript-0.4.1/tests/test_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,27 +96,27 @@
 
         with self.assertRaises(errors.SyntaxError) as e:
             parsing.compile_script('OP_DEF 0 { d123 }')
         assert 'unrecognized symbol' in str(e.exception)
 
         with self.assertRaises(errors.SyntaxError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH 123 }')
-        assert str(e.exception) == 'values for OP_PUSH must be prefaced with d, x, or s'
+        assert 'values for OP_PUSH must be prefaced with' in str(e.exception)
 
         with self.assertRaises(ValueError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH dabc }')
         assert str(e.exception) == 'value prefaced by d must be decimal int'
 
         with self.assertRaises(errors.SyntaxError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH1 asd }')
-        assert 'values for OP_PUSH1 must be prefaced with d, x, or s' in str(e.exception)
+        assert 'values for OP_PUSH1 must be prefaced with' in str(e.exception)
 
         with self.assertRaises(ValueError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH1 dnotnumeric }')
-        assert 'value prefaced by d must be decimal int or float' in str(e.exception)
+        assert 'value prefaced by d must be decimal int' in str(e.exception)
 
         with self.assertRaises(errors.SyntaxError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH0 asd }')
         assert 'numeric args must be prefaced with d or x' in str(e.exception)
 
         with self.assertRaises(ValueError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH0 dnotnumeric }')
@@ -124,35 +124,36 @@
 
         with self.assertRaises(ValueError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH0 x1234 }')
         assert 'value must be at most 1 byte long' in str(e.exception)
 
         with self.assertRaises(errors.SyntaxError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH2 asd }')
-        assert 'values for OP_PUSH2 must be prefaced with d, x, or s' in str(e.exception)
+        assert 'values for OP_PUSH2 must be prefaced with' in str(e.exception)
 
         with self.assertRaises(ValueError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH2 dnotnumeric }')
         assert 'value prefaced by d must be decimal int' in str(e.exception)
 
         with self.assertRaises(errors.SyntaxError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH4 asd }')
-        assert 'values for OP_PUSH4 must be prefaced with d, x, or s' in str(e.exception)
+        assert 'values for OP_PUSH4 must be prefaced with' in str(e.exception)
 
         with self.assertRaises(ValueError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH4 dnotnumeric }')
         assert 'value prefaced by d must be decimal int' in str(e.exception)
 
         with self.assertRaises(errors.SyntaxError) as e:
             parsing.compile_script('OP_DEF 0 { OP_DIV_FLOAT asd }')
-        assert 'numeric args must be prefaced with d or x' in str(e.exception)
+        assert 'numeric args must be prefaced with' in str(e.exception)
 
         with self.assertRaises(ValueError) as e:
-            parsing.compile_script('OP_DEF 0 { OP_DIV_FLOAT dnotnumeric }')
-        assert 'value prefaced by d must be decimal float' in str(e.exception)
+            parsing.compile_script('OP_DEF 0 { OP_DIV_FLOAT fnotnumeric }')
+        assert 'value prefaced by' in str(e.exception)
+        assert 'must be decimal float' in str(e.exception)
 
         with self.assertRaises(ValueError) as e:
             parsing.compile_script('OP_DEF 0 { OP_MOD_FLOAT x123456 }')
         assert 'value prefaced by x must be 8 long (4 bytes)' in str(e.exception)
 
         with self.assertRaises(errors.SyntaxError) as e:
             parsing.compile_script('OP_DEF 0 { OP_SWAP asd d123 }')
```

### Comparing `tapescript-0.4.0/tests/test_tools.py` & `tapescript-0.4.1/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_committed_script.hex` & `tapescript-0.4.1/tests/vectors/cds_committed_script.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_committed_script.src` & `tapescript-0.4.1/tests/vectors/cds_committed_script.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_committed_script_decompiled.src` & `tapescript-0.4.1/tests/vectors/cds_committed_script_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_unlocking_script1.hex` & `tapescript-0.4.1/tests/vectors/cds_unlocking_script1.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_unlocking_script1.src` & `tapescript-0.4.1/tests/vectors/cds_unlocking_script1.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_unlocking_script1_decompiled.src` & `tapescript-0.4.1/tests/vectors/cds_unlocking_script1_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_unlocking_script2.hex` & `tapescript-0.4.1/tests/vectors/cds_unlocking_script2.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_unlocking_script2.src` & `tapescript-0.4.1/tests/vectors/cds_unlocking_script2.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_unlocking_script2_decompiled.src` & `tapescript-0.4.1/tests/vectors/cds_unlocking_script2_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_unlocking_script3.hex` & `tapescript-0.4.1/tests/vectors/cds_unlocking_script3.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_unlocking_script3.src` & `tapescript-0.4.1/tests/vectors/cds_unlocking_script3.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/cds_unlocking_script3_decompiled.src` & `tapescript-0.4.1/tests/vectors/cds_unlocking_script3_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/correspondent_unlocking_script2.src` & `tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/correspondent_unlocking_script2_decompiled.src` & `tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/macros_and_variables.src` & `tapescript-0.4.1/tests/vectors/macros_and_variables.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/macros_and_variables_decompiled.src` & `tapescript-0.4.1/tests/vectors/macros_and_variables_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/new_ops_0.4.0_decompiled.src` & `tapescript-0.4.1/tests/vectors/new_ops_0.4.0_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/omega_e2e.hex` & `tapescript-0.4.1/tests/vectors/omega_e2e.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/omega_e2e.src` & `tapescript-0.4.1/tests/vectors/omega_e2e.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/omega_e2e_aliases.src` & `tapescript-0.4.1/tests/vectors/omega_e2e_aliases.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/tests/vectors/omega_e2e_decompiled.src` & `tapescript-0.4.1/tests/vectors/omega_e2e_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.0/pyproject.toml` & `tapescript-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tapescript"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 dependencies = [
   "PyNaCl>=1.5.0"
 ]
 description = "Scripting system for use in distributed systems"
```

### Comparing `tapescript-0.4.0/readme.md` & `tapescript-0.4.1/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Tapescript
 
-Simple script system loosely inspired by Bitcoin script but also hopefully more
+Simple DSL and VM loosely inspired by Bitcoin script but also hopefully more
 useful for other applications. The idea is to programmatically ensure access
-controls in a distributed system.
+controls in a distributed system using cryptography.
 
 ## Status
 
 - [x] OPs
 - [x] Interpreter functions and classes
 - [x] Byte-code compiler
 - [x] Decompiler
@@ -181,17 +181,17 @@
 - `OP_MAKE_ADAPTER_SIG_PUBLIC`
 - `OP_MAKE_ADAPTER_SIG_PRIVATE`
 - `OP_CHECK_ADAPTER_SIG`
 - `OP_DECRYPT_ADAPTER_SIG`
 - `make_adapter_lock_pub`
 - `make_adapter_lock_prv`
 - `make_adapter_locks_pub`
+- `make_adapter_locks_prv`
 - `make_adapter_decrypt`
 - `decrypt_adapter`
-- `make_adapter_locks_prv`
 - `make_adapter_witness`
 - `clamp_scalar`
 - `derive_key_from_seed`
 - `derive_point_from_scalar`
 - `aggregate_points`
 - `aggregate_scalars`
 
@@ -199,16 +199,16 @@
 of related transactions to be constructed in such a way that unlocking one of
 them unlocks all of them through a mathematical cascade. When combined with
 adapter signatures, it allows all links in the chain to be verified before they
 are unlocked. See [the original paper](https://secpriv.wien/fulltext/publik_278436.pdf)
 for a full explanation of the mathematics of the AMHL. Tapescript provides the
 following tools for using AMHLs:
 
-- `tools.setup_amhl`
-- `tools.release_left_amhl_lock`
+- `setup_amhl`
+- `release_left_amhl_lock`
 
 The `setup_amhl` tool constructs adapter signature locking scripts, `check_sig`
 locks, and intermediate values, and it will provide PTLCs in lieu of `check_sig`
 locks for any pubkey for which a corresponding entry is found in the optional
 `refund_pubkeys` argument. The paper authors envision its use with MuSig/MuSig2
 aggregated keys in a "scriptless script" setting, but MuSig and MuSig2 are
 beyond the scope of this project.
@@ -286,21 +286,24 @@
 call `add_contract_interface` and pass a `runtime_checkable` subclass of
 `typing.Protocol` as the argument. To remove an interface, call
 `remove_contract_interface` and pass the interface as the argument.
 
 To add a contract, use `add_contract(contract_id: bytes, contract: object)`. To
 remove a contract, use `remove_contract(contract_id: bytes)`.
 
-Each contract will be checked against each interface when added (it must meet at
-least one) and again at runtime when an op that uses a contract is executed. All
-contracts added via the `add_contract` function will be included in the runtime
-environment of scripts run thereafter. Additionally, contracts can be passed
-into the `run_script` and `run_auth_script` functions, and these will override
-any contracts in the global runtime environment in case of a contract_id
-conflict.
+Each contract will be checked against each interface when added (it must
+implement at least one) and again at runtime when an op that uses a contract is
+executed. All contracts added via the `add_contract` function will be included
+in the runtime environment of scripts run thereafter. Additionally, contracts
+can be passed into the `run_script` and `run_auth_script` functions, and these
+will override any contracts in the global runtime environment in case of a
+contract_id conflict. The contract_id should be a cryptographic hash of the
+contract's source code; it is called a contract rather than a module because the
+users of a system must commit to running the same code, and this forms a
+contractual relationship between users.
 
 To use a contract in a custom op, find it in the `tape.contracts` dict by its
 contract_id.
 
 ### Signature checking
 
 Notes for the `OP_CHECK_SIG` and `OP_CHECK_SIG_VERIFY` operations:
@@ -323,36 +326,38 @@
 A soft fork is a protocol upgrade such that all scripts written under the new
 protocol also validate under the old version -- older versions do not break when
 encountering use of the new feature. Tapescript was designed with soft-fork
 support in mind, and the helper function `add_soft_fork` is included to
 streamline the process and reduce the use of boilerplate.
 
 To enable a soft fork, a NOP code must be replaced with an op that reads the
-next byte as an unsigned int, pulls that many values from the queue, runs any
+next byte as a signed int, pulls that many values from the queue, runs any
 checks on the data, and raises an error in case any check fails. This maintains
 the behavior of the original NOP such that any nodes that did not activate the
 soft fork will not have any errors parsing scripts using the new OP.
 
 Example soft fork:
 
 ```python
 from tapescript import (
     Tape,
     ScriptExecutionError,
-    add_soft_fork
+    add_soft_fork,
+    bytes_to_int,
 )
 from queue import LifoQueue
 
 
 def OP_CHECK_ALL_EQUAL_VERIFY(tape: Tape, queue: LifoQueue, cache: dict) -> None:
-    """Replacement for NOP255: read the next byte as uint count, take
+    """Replacement for NOP255: read the next byte an int count, take
         that many items from queue, run checks, and raise an error if
         any check fails.
     """
-    count = tape.read(1)[0]
+    count = bytes_to_int(tape.read(1))
+    assert count >= 0
     items = []
     for i in range(count):
         items.append(queue.get(False))
 
     compare = items.pop()
     while len(items):
         if items.pop() != compare:
@@ -422,15 +427,15 @@
 python test/test_classes.py
 python test/test_functions.py
 python test/test_parsing.py
 python test/test_tools.py
 python test/test_e2e_eltoo.py
 ```
 
-There are currently 223 tests and 104 test vectors used for validating the
+There are currently 225 tests and 106 test vectors used for validating the
 compiler, decompiler, and script running functions. This includes 3 tests for a
 proof-of-concept implementation of the eltoo payment channel protocol, a test
 proving the one-way homomorphic quality of ed25519, and e2e tests combining the
 anonymous multi-hop lock (AMHL) system with adapter signatures.
 
 ## ISC License
```

### Comparing `tapescript-0.4.0/PKG-INFO` & `tapescript-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tapescript
-Version: 0.4.0
+Version: 0.4.1
 Summary: Scripting system for use in distributed systems
 Project-URL: Homepage, https://github.com/k98kurz/tapescript
 Project-URL: Bug Tracker, https://github.com/k98kurz/tapescript/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -13,17 +13,17 @@
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.10
 Requires-Dist: pynacl>=1.5.0
 Description-Content-Type: text/markdown
 
 # Tapescript
 
-Simple script system loosely inspired by Bitcoin script but also hopefully more
+Simple DSL and VM loosely inspired by Bitcoin script but also hopefully more
 useful for other applications. The idea is to programmatically ensure access
-controls in a distributed system.
+controls in a distributed system using cryptography.
 
 ## Status
 
 - [x] OPs
 - [x] Interpreter functions and classes
 - [x] Byte-code compiler
 - [x] Decompiler
@@ -198,17 +198,17 @@
 - `OP_MAKE_ADAPTER_SIG_PUBLIC`
 - `OP_MAKE_ADAPTER_SIG_PRIVATE`
 - `OP_CHECK_ADAPTER_SIG`
 - `OP_DECRYPT_ADAPTER_SIG`
 - `make_adapter_lock_pub`
 - `make_adapter_lock_prv`
 - `make_adapter_locks_pub`
+- `make_adapter_locks_prv`
 - `make_adapter_decrypt`
 - `decrypt_adapter`
-- `make_adapter_locks_prv`
 - `make_adapter_witness`
 - `clamp_scalar`
 - `derive_key_from_seed`
 - `derive_point_from_scalar`
 - `aggregate_points`
 - `aggregate_scalars`
 
@@ -216,16 +216,16 @@
 of related transactions to be constructed in such a way that unlocking one of
 them unlocks all of them through a mathematical cascade. When combined with
 adapter signatures, it allows all links in the chain to be verified before they
 are unlocked. See [the original paper](https://secpriv.wien/fulltext/publik_278436.pdf)
 for a full explanation of the mathematics of the AMHL. Tapescript provides the
 following tools for using AMHLs:
 
-- `tools.setup_amhl`
-- `tools.release_left_amhl_lock`
+- `setup_amhl`
+- `release_left_amhl_lock`
 
 The `setup_amhl` tool constructs adapter signature locking scripts, `check_sig`
 locks, and intermediate values, and it will provide PTLCs in lieu of `check_sig`
 locks for any pubkey for which a corresponding entry is found in the optional
 `refund_pubkeys` argument. The paper authors envision its use with MuSig/MuSig2
 aggregated keys in a "scriptless script" setting, but MuSig and MuSig2 are
 beyond the scope of this project.
@@ -303,21 +303,24 @@
 call `add_contract_interface` and pass a `runtime_checkable` subclass of
 `typing.Protocol` as the argument. To remove an interface, call
 `remove_contract_interface` and pass the interface as the argument.
 
 To add a contract, use `add_contract(contract_id: bytes, contract: object)`. To
 remove a contract, use `remove_contract(contract_id: bytes)`.
 
-Each contract will be checked against each interface when added (it must meet at
-least one) and again at runtime when an op that uses a contract is executed. All
-contracts added via the `add_contract` function will be included in the runtime
-environment of scripts run thereafter. Additionally, contracts can be passed
-into the `run_script` and `run_auth_script` functions, and these will override
-any contracts in the global runtime environment in case of a contract_id
-conflict.
+Each contract will be checked against each interface when added (it must
+implement at least one) and again at runtime when an op that uses a contract is
+executed. All contracts added via the `add_contract` function will be included
+in the runtime environment of scripts run thereafter. Additionally, contracts
+can be passed into the `run_script` and `run_auth_script` functions, and these
+will override any contracts in the global runtime environment in case of a
+contract_id conflict. The contract_id should be a cryptographic hash of the
+contract's source code; it is called a contract rather than a module because the
+users of a system must commit to running the same code, and this forms a
+contractual relationship between users.
 
 To use a contract in a custom op, find it in the `tape.contracts` dict by its
 contract_id.
 
 ### Signature checking
 
 Notes for the `OP_CHECK_SIG` and `OP_CHECK_SIG_VERIFY` operations:
@@ -340,36 +343,38 @@
 A soft fork is a protocol upgrade such that all scripts written under the new
 protocol also validate under the old version -- older versions do not break when
 encountering use of the new feature. Tapescript was designed with soft-fork
 support in mind, and the helper function `add_soft_fork` is included to
 streamline the process and reduce the use of boilerplate.
 
 To enable a soft fork, a NOP code must be replaced with an op that reads the
-next byte as an unsigned int, pulls that many values from the queue, runs any
+next byte as a signed int, pulls that many values from the queue, runs any
 checks on the data, and raises an error in case any check fails. This maintains
 the behavior of the original NOP such that any nodes that did not activate the
 soft fork will not have any errors parsing scripts using the new OP.
 
 Example soft fork:
 
 ```python
 from tapescript import (
     Tape,
     ScriptExecutionError,
-    add_soft_fork
+    add_soft_fork,
+    bytes_to_int,
 )
 from queue import LifoQueue
 
 
 def OP_CHECK_ALL_EQUAL_VERIFY(tape: Tape, queue: LifoQueue, cache: dict) -> None:
-    """Replacement for NOP255: read the next byte as uint count, take
+    """Replacement for NOP255: read the next byte an int count, take
         that many items from queue, run checks, and raise an error if
         any check fails.
     """
-    count = tape.read(1)[0]
+    count = bytes_to_int(tape.read(1))
+    assert count >= 0
     items = []
     for i in range(count):
         items.append(queue.get(False))
 
     compare = items.pop()
     while len(items):
         if items.pop() != compare:
@@ -439,15 +444,15 @@
 python test/test_classes.py
 python test/test_functions.py
 python test/test_parsing.py
 python test/test_tools.py
 python test/test_e2e_eltoo.py
 ```
 
-There are currently 223 tests and 104 test vectors used for validating the
+There are currently 225 tests and 106 test vectors used for validating the
 compiler, decompiler, and script running functions. This includes 3 tests for a
 proof-of-concept implementation of the eltoo payment channel protocol, a test
 proving the one-way homomorphic quality of ed25519, and e2e tests combining the
 anonymous multi-hop lock (AMHL) system with adapter signatures.
 
 ## ISC License
```

