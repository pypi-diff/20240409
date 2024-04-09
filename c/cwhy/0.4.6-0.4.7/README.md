# Comparing `tmp/cwhy-0.4.6.tar.gz` & `tmp/cwhy-0.4.7.tar.gz`

## Comparing `cwhy-0.4.6.tar` & `cwhy-0.4.7.tar`

### file list

```diff
@@ -1,117 +1,137 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cwhy-0.4.6/.clang-format
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 cwhy-0.4.6/.github/workflows/regression-check.yml
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 cwhy-0.4.6/.github/workflows/regression-generate.yml
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 cwhy-0.4.6/.github/workflows/release.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 cwhy-0.4.6/.github/workflows/sanity.yml
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cwhy-0.4.6/mutations/.gitignore
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 cwhy-0.4.6/mutations/CMakeLists.txt
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cwhy-0.4.6/mutations/README.md
--rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 cwhy-0.4.6/mutations/src/main.cpp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.6/src/cwhy/__init__.py
--rwxr-xr-x   0        0        0     6281 2020-02-02 00:00:00.000000 cwhy-0.4.6/src/cwhy/__main__.py
--rwxr-xr-x   0        0        0     7037 2020-02-02 00:00:00.000000 cwhy-0.4.6/src/cwhy/cwhy.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 cwhy-0.4.6/src/cwhy/print_debug.py
--rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 cwhy-0.4.6/src/cwhy/prompts.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 cwhy-0.4.6/src/cwhy/conversation/__init__.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 cwhy-0.4.6/src/cwhy/conversation/diff_functions.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 cwhy-0.4.6/src/cwhy/conversation/explain_functions.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cwhy-0.4.6/src/cwhy/conversation/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/__init__.py
--rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/anonymizer.py
--rwxr-xr-x   0        0        0     1462 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/apply_diff.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/manifest.yml
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/prepare.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/regression.py
--rwxr-xr-x   0        0        0     3845 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/runner-diff.py
--rwxr-xr-x   0        0        0     4165 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/cpp20-feature.cpp
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/ctre-test.cpp
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/include-header-typo.cpp
--rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/missing-hash.cpp
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/missing-ostream-operator.cpp
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/missing-struct-semicolon.cpp
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/overload-resolution-failure-transform-missing-argument.cpp
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/push-back-pointer.cpp
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/redeclared-function.cpp
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/redeclared-variable-deduction-order.cpp
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/redefined-function.cpp
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/reverse-iterator.cpp
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/sfinae-ambiguous.cpp
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/sfinae-trailing-return-type-conditional-noexcept.cpp
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/sfinae-trailing-return-type.cpp
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/macos/clang++/template-recursion.cpp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/cpp20-feature.cpp
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/ctre-test.cpp
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/include-header-typo.cpp
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/missing-hash.cpp
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/missing-ostream-operator.cpp
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/missing-struct-semicolon.cpp
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/overload-resolution-failure-transform-missing-argument.cpp
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/push-back-pointer.cpp
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/redeclared-function.cpp
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/redeclared-variable-deduction-order.cpp
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/redefined-function.cpp
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/reverse-iterator.cpp
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/sfinae-ambiguous.cpp
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/sfinae-trailing-return-type-conditional-noexcept.cpp
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/sfinae-trailing-return-type.cpp
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/clang++/template-recursion.cpp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/cpp20-feature.cpp
--rw-r--r--   0        0        0    12529 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/ctre-test.cpp
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/include-header-typo.cpp
--rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/missing-hash.cpp
--rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/missing-ostream-operator.cpp
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/missing-struct-semicolon.cpp
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/overload-resolution-failure-transform-missing-argument.cpp
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/push-back-pointer.cpp
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/redeclared-function.cpp
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/redeclared-variable-deduction-order.cpp
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/redefined-function.cpp
--rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/reverse-iterator.cpp
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/sfinae-ambiguous.cpp
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/sfinae-trailing-return-type-conditional-noexcept.cpp
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/sfinae-trailing-return-type.cpp
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/.regression/ubuntu/g++/template-recursion.cpp
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/Haskell/README.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/Haskell/testme-fixed.hs
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/Haskell/testme.hs
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c#/testme.cs
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c#/testme.cs.out
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/blank-header.hpp
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/cpp20-feature.cpp
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/ctre-test.cpp
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/include-header-typo.cpp
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/manifest.yml
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/missing-hash.cpp
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/missing-ostream-operator.cpp
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/missing-struct-semicolon.cpp
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/overload-resolution-failure-transform-missing-argument.cpp
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/push-back-pointer.cpp
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/redeclared-function.cpp
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/redeclared-variable-deduction-order.cpp
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/redefined-function.cpp
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/reverse-iterator.cpp
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/sfinae-ambiguous.cpp
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/sfinae-trailing-return-type-conditional-noexcept.cpp
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/sfinae-trailing-return-type.cpp
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/c++/template-recursion.cpp
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/go/testme.go
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/go/testme.go.out
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/kotlin/README.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/kotlin/testme.kt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/php/testme.php
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/python/concatenate-str-to-int.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/ruby/testme.rb
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/rust/testme.rs
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/swift/README.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 cwhy-0.4.6/tests/swift/testme.swift
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cwhy-0.4.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 cwhy-0.4.6/LICENSE
--rw-r--r--   0        0        0    13591 2020-02-02 00:00:00.000000 cwhy-0.4.6/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 cwhy-0.4.6/pyproject.toml
--rw-r--r--   0        0        0    14499 2020-02-02 00:00:00.000000 cwhy-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cwhy-0.4.7/.clang-format
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 cwhy-0.4.7/.github/workflows/regression-check.yml
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 cwhy-0.4.7/.github/workflows/regression-generate.yml
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 cwhy-0.4.7/.github/workflows/release.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 cwhy-0.4.7/.github/workflows/sanity.yml
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cwhy-0.4.7/mutations/.gitignore
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 cwhy-0.4.7/mutations/CMakeLists.txt
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cwhy-0.4.7/mutations/README.md
+-rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 cwhy-0.4.7/mutations/src/main.cpp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.7/src/cwhy/__init__.py
+-rwxr-xr-x   0        0        0     6284 2020-02-02 00:00:00.000000 cwhy-0.4.7/src/cwhy/__main__.py
+-rwxr-xr-x   0        0        0     7013 2020-02-02 00:00:00.000000 cwhy-0.4.7/src/cwhy/cwhy.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 cwhy-0.4.7/src/cwhy/print_debug.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 cwhy-0.4.7/src/cwhy/prompts.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 cwhy-0.4.7/src/cwhy/conversation/__init__.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 cwhy-0.4.7/src/cwhy/conversation/diff_functions.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 cwhy-0.4.7/src/cwhy/conversation/explain_functions.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cwhy-0.4.7/src/cwhy/conversation/utils.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_1.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_10.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_11.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_12.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_13.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_14.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_15.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_16.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_17.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_18.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_19.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_2.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_20.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_3.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_4.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_5.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_6.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_7.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_8.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 cwhy-0.4.7/test/test_coverup_openai_9.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/__init__.py
+-rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/anonymizer.py
+-rwxr-xr-x   0        0        0     1462 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/apply_diff.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/manifest.yml
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/prepare.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/regression.py
+-rwxr-xr-x   0        0        0     3845 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/runner-diff.py
+-rwxr-xr-x   0        0        0     4165 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/cpp20-feature.cpp
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/ctre-test.cpp
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/include-header-typo.cpp
+-rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/missing-hash.cpp
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/missing-ostream-operator.cpp
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/missing-struct-semicolon.cpp
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/overload-resolution-failure-transform-missing-argument.cpp
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/push-back-pointer.cpp
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/redeclared-function.cpp
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/redeclared-variable-deduction-order.cpp
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/redefined-function.cpp
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/reverse-iterator.cpp
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/sfinae-ambiguous.cpp
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/sfinae-trailing-return-type-conditional-noexcept.cpp
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/sfinae-trailing-return-type.cpp
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/macos/clang++/template-recursion.cpp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/cpp20-feature.cpp
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/ctre-test.cpp
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/include-header-typo.cpp
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/missing-hash.cpp
+-rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/missing-ostream-operator.cpp
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/missing-struct-semicolon.cpp
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/overload-resolution-failure-transform-missing-argument.cpp
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/push-back-pointer.cpp
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/redeclared-function.cpp
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/redeclared-variable-deduction-order.cpp
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/redefined-function.cpp
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/reverse-iterator.cpp
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/sfinae-ambiguous.cpp
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/sfinae-trailing-return-type-conditional-noexcept.cpp
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/sfinae-trailing-return-type.cpp
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/clang++/template-recursion.cpp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/cpp20-feature.cpp
+-rw-r--r--   0        0        0    12529 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/ctre-test.cpp
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/include-header-typo.cpp
+-rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/missing-hash.cpp
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/missing-ostream-operator.cpp
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/missing-struct-semicolon.cpp
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/overload-resolution-failure-transform-missing-argument.cpp
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/push-back-pointer.cpp
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/redeclared-function.cpp
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/redeclared-variable-deduction-order.cpp
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/redefined-function.cpp
+-rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/reverse-iterator.cpp
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/sfinae-ambiguous.cpp
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/sfinae-trailing-return-type-conditional-noexcept.cpp
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/sfinae-trailing-return-type.cpp
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/.regression/ubuntu/g++/template-recursion.cpp
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/Haskell/README.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/Haskell/testme-fixed.hs
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/Haskell/testme.hs
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c#/testme.cs
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c#/testme.cs.out
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/blank-header.hpp
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/cpp20-feature.cpp
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/ctre-test.cpp
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/include-header-typo.cpp
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/manifest.yml
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/missing-hash.cpp
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/missing-ostream-operator.cpp
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/missing-struct-semicolon.cpp
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/overload-resolution-failure-transform-missing-argument.cpp
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/push-back-pointer.cpp
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/redeclared-function.cpp
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/redeclared-variable-deduction-order.cpp
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/redefined-function.cpp
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/reverse-iterator.cpp
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/sfinae-ambiguous.cpp
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/sfinae-trailing-return-type-conditional-noexcept.cpp
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/sfinae-trailing-return-type.cpp
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/c++/template-recursion.cpp
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/go/testme.go
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/go/testme.go.out
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/kotlin/README.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/kotlin/testme.kt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/php/testme.php
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/python/concatenate-str-to-int.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/ruby/testme.rb
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/rust/testme.rs
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/swift/README.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 cwhy-0.4.7/tests/swift/testme.swift
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cwhy-0.4.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 cwhy-0.4.7/LICENSE
+-rw-r--r--   0        0        0    13591 2020-02-02 00:00:00.000000 cwhy-0.4.7/README.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 cwhy-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0    14499 2020-02-02 00:00:00.000000 cwhy-0.4.7/PKG-INFO
```

### Comparing `cwhy-0.4.6/.github/workflows/regression-check.yml` & `cwhy-0.4.7/.github/workflows/regression-check.yml`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/.github/workflows/regression-generate.yml` & `cwhy-0.4.7/.github/workflows/regression-generate.yml`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/.github/workflows/release.yml` & `cwhy-0.4.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/.github/workflows/sanity.yml` & `cwhy-0.4.7/.github/workflows/sanity.yml`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/mutations/CMakeLists.txt` & `cwhy-0.4.7/mutations/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/mutations/README.md` & `cwhy-0.4.7/mutations/README.md`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/mutations/src/main.cpp` & `cwhy-0.4.7/mutations/src/main.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/src/cwhy/__main__.py` & `cwhy-0.4.7/src/cwhy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,17 +114,17 @@
         nargs="?",
         default="explain",
         choices=["explain", "diff", "converse", "diff-converse"],
         metavar="subcommand",
         help=textwrap.dedent(
             """
                 explain:       explain the diagnostic (default)
-                diff:          \[experimental] generate a diff to fix the diagnostic
-                converse:      \[experimental] interactively converse with CWhy
-                diff-converse: \[experimental] interactively fix errors with CWhy
+                diff:          \\[experimental] generate a diff to fix the diagnostic
+                converse:      \\[experimental] interactively converse with CWhy
+                diff-converse: \\[experimental] interactively fix errors with CWhy
             """
         ).strip(),
     )
 
     parser.add_argument(
         "--llm",
         type=str,
```

### Comparing `cwhy-0.4.6/src/cwhy/cwhy.py` & `cwhy-0.4.7/src/cwhy/cwhy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import argparse
 import os
 import subprocess
 import sys
-import logging
+import warnings
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    import litellm  # type: ignore
 
-import litellm  # type: ignore
 import llm_utils
 from openai import (
     NotFoundError,
     RateLimitError,
     APITimeoutError,
     OpenAIError,
     BadRequestError,
 )
 
 from . import conversation, prompts
 from .print_debug import dprint, enable_debug_printing
 
 
-# Turn off most logging
-litellm.set_verbose = False
-logging.getLogger().setLevel(logging.ERROR)
-
-
 def print_key_info():
     dprint("You need a key (or keys) from an AI service to use CWhy.")
     dprint()
     dprint("OpenAI:")
     dprint("  You can get a key here: https://platform.openai.com/api-keys")
     dprint("  Set the environment variable OPENAI_API_KEY to your key value:")
     dprint("    export OPENAI_API_KEY=<your key>")
```

### Comparing `cwhy-0.4.6/src/cwhy/print_debug.py` & `cwhy-0.4.7/src/cwhy/print_debug.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/src/cwhy/prompts.py` & `cwhy-0.4.7/src/cwhy/prompts.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/src/cwhy/conversation/__init__.py` & `cwhy-0.4.7/src/cwhy/conversation/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import json
 import textwrap
+import warnings
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    import litellm  # type: ignore
 
-import litellm  # type: ignore
 import llm_utils
 
 from . import utils
 from .diff_functions import DiffFunctions
 from .explain_functions import ExplainFunctions
 from ..print_debug import dprint
```

### Comparing `cwhy-0.4.6/src/cwhy/conversation/diff_functions.py` & `cwhy-0.4.7/src/cwhy/conversation/diff_functions.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/src/cwhy/conversation/explain_functions.py` & `cwhy-0.4.7/src/cwhy/conversation/explain_functions.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/src/cwhy/conversation/utils.py` & `cwhy-0.4.7/src/cwhy/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/anonymizer.py` & `cwhy-0.4.7/tests/anonymizer.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/apply_diff.py` & `cwhy-0.4.7/tests/apply_diff.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/prepare.py` & `cwhy-0.4.7/tests/prepare.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/regression.py` & `cwhy-0.4.7/tests/regression.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/runner-diff.py` & `cwhy-0.4.7/tests/runner-diff.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/runner.py` & `cwhy-0.4.7/tests/runner.py`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/ctre-test.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/ctre-test.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/include-header-typo.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/include-header-typo.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/missing-hash.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/missing-hash.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/missing-ostream-operator.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/missing-ostream-operator.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/missing-struct-semicolon.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/missing-struct-semicolon.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/overload-resolution-failure-transform-missing-argument.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/overload-resolution-failure-transform-missing-argument.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/push-back-pointer.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/push-back-pointer.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/redeclared-function.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/redeclared-function.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/redeclared-variable-deduction-order.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/redeclared-variable-deduction-order.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/redefined-function.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/redefined-function.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/reverse-iterator.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/reverse-iterator.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/sfinae-ambiguous.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/sfinae-ambiguous.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/sfinae-trailing-return-type-conditional-noexcept.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/sfinae-trailing-return-type-conditional-noexcept.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/sfinae-trailing-return-type.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/sfinae-trailing-return-type.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/macos/clang++/template-recursion.cpp` & `cwhy-0.4.7/tests/.regression/macos/clang++/template-recursion.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/ctre-test.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/ctre-test.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/include-header-typo.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/include-header-typo.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/missing-hash.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/missing-hash.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/missing-ostream-operator.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/missing-ostream-operator.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/missing-struct-semicolon.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/missing-struct-semicolon.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/overload-resolution-failure-transform-missing-argument.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/overload-resolution-failure-transform-missing-argument.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/push-back-pointer.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/push-back-pointer.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/redeclared-function.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/redeclared-function.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/redeclared-variable-deduction-order.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/redeclared-variable-deduction-order.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/redefined-function.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/redefined-function.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/reverse-iterator.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/reverse-iterator.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/sfinae-ambiguous.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/sfinae-ambiguous.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/sfinae-trailing-return-type-conditional-noexcept.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/sfinae-trailing-return-type-conditional-noexcept.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/sfinae-trailing-return-type.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/sfinae-trailing-return-type.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/clang++/template-recursion.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/clang++/template-recursion.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/ctre-test.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/ctre-test.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/include-header-typo.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/include-header-typo.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/missing-hash.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/missing-hash.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/missing-ostream-operator.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/missing-ostream-operator.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/missing-struct-semicolon.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/missing-struct-semicolon.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/overload-resolution-failure-transform-missing-argument.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/overload-resolution-failure-transform-missing-argument.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/push-back-pointer.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/push-back-pointer.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/redeclared-function.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/redeclared-function.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/redeclared-variable-deduction-order.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/redeclared-variable-deduction-order.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/redefined-function.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/redefined-function.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/reverse-iterator.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/reverse-iterator.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/sfinae-ambiguous.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/sfinae-ambiguous.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/sfinae-trailing-return-type-conditional-noexcept.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/sfinae-trailing-return-type-conditional-noexcept.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/sfinae-trailing-return-type.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/sfinae-trailing-return-type.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/.regression/ubuntu/g++/template-recursion.cpp` & `cwhy-0.4.7/tests/.regression/ubuntu/g++/template-recursion.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/ctre-test.cpp` & `cwhy-0.4.7/tests/c++/ctre-test.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/missing-hash.cpp` & `cwhy-0.4.7/tests/c++/missing-hash.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/missing-ostream-operator.cpp` & `cwhy-0.4.7/tests/c++/missing-ostream-operator.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp` & `cwhy-0.4.7/tests/c++/overload-resolution-failure-bind-const-ref-to-non-const-ref.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/overload-resolution-failure-transform-missing-argument.cpp` & `cwhy-0.4.7/tests/c++/overload-resolution-failure-transform-missing-argument.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/push-back-pointer.cpp` & `cwhy-0.4.7/tests/c++/push-back-pointer.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/redeclared-function.cpp` & `cwhy-0.4.7/tests/c++/redeclared-function.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/redefined-function.cpp` & `cwhy-0.4.7/tests/c++/redefined-function.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/reverse-iterator.cpp` & `cwhy-0.4.7/tests/c++/reverse-iterator.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/c++/template-recursion.cpp` & `cwhy-0.4.7/tests/c++/template-recursion.cpp`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/tests/kotlin/testme.kt` & `cwhy-0.4.7/tests/kotlin/testme.kt`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/.gitignore` & `cwhy-0.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/LICENSE` & `cwhy-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/README.md` & `cwhy-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `cwhy-0.4.6/pyproject.toml` & `cwhy-0.4.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cwhy"
-version = "0.4.6"
+version = "0.4.7"
 authors = [
   { name="Emery Berger", email="emery.berger@gmail.com" },
   { name="Nicolas van Kempen", email="nvankemp@gmail.com" },
   { name="Bryce Adelstein Lelbach", email="brycelelbach@gmail.com" }
 ]
 
 dependencies = [
```

### Comparing `cwhy-0.4.6/PKG-INFO` & `cwhy-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: cwhy
-Version: 0.4.6
+Version: 0.4.7
 Summary: Explains and proposes fixes for compile-time errors for many programming languages.
 Project-URL: Homepage, https://github.com/plasma-umass/cwhy
 Project-URL: Bug Tracker, https://github.com/plasma-umass/cwhy/issues
 Author-email: Emery Berger <emery.berger@gmail.com>, Nicolas van Kempen <nvankemp@gmail.com>, Bryce Adelstein Lelbach <brycelelbach@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

