# Comparing `tmp/protokolo-0.3.0.tar.gz` & `tmp/protokolo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protokolo-0.3.0.tar", max compression
+gzip compressed data, was "protokolo-1.0.0.tar", max compression
```

## Comparing `protokolo-0.3.0.tar` & `protokolo-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1451 2024-04-07 11:37:00.007312 protokolo-0.3.0/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-0.3.0/LICENSES/
--rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-0.3.0/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-0.3.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-0.3.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     5698 2024-04-07 10:36:42.970478 protokolo-0.3.0/README.md
--rw-r--r--   0        0        0     2452 2024-04-07 11:36:14.630847 protokolo-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      177 2024-04-07 11:36:14.630847 protokolo-0.3.0/src/protokolo/__init__.py
--rw-r--r--   0        0        0      290 2024-04-07 10:30:16.712348 protokolo-0.3.0/src/protokolo/__main__.py
--rw-r--r--   0        0        0     3874 2024-03-08 18:49:41.103198 protokolo-0.3.0/src/protokolo/_formatter.py
--rw-r--r--   0        0        0     1435 2024-03-08 18:20:59.913097 protokolo-0.3.0/src/protokolo/_util.py
--rw-r--r--   0        0        0     7950 2024-04-07 10:30:16.712348 protokolo-0.3.0/src/protokolo/cli.py
--rw-r--r--   0        0        0     9904 2024-04-07 08:08:13.113594 protokolo-0.3.0/src/protokolo/compile.py
--rw-r--r--   0        0        0    11710 2024-04-06 19:36:36.296945 protokolo-0.3.0/src/protokolo/config.py
--rw-r--r--   0        0        0     3171 2023-11-07 12:34:47.189029 protokolo-0.3.0/src/protokolo/exceptions.py
--rw-r--r--   0        0        0     3778 2024-03-29 20:30:44.665888 protokolo-0.3.0/src/protokolo/initialise.py
--rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-0.3.0/src/protokolo/py.typed
--rw-r--r--   0        0        0      890 2023-11-01 17:19:54.550000 protokolo-0.3.0/src/protokolo/replace.py
--rw-r--r--   0        0        0      930 2024-03-29 19:44:07.379769 protokolo-0.3.0/src/protokolo/types.py
--rw-r--r--   0        0        0     2224 2024-04-06 17:40:55.028923 protokolo-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0    18254 2024-04-07 10:30:16.712348 protokolo-0.3.0/tests/test_cli.py
--rw-r--r--   0        0        0    14236 2024-04-07 08:08:13.113594 protokolo-0.3.0/tests/test_compile.py
--rw-r--r--   0        0        0    11411 2024-03-29 19:44:07.383769 protokolo-0.3.0/tests/test_config.py
--rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-0.3.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     6089 2023-11-07 12:32:33.427701 protokolo-0.3.0/tests/test_formatter.py
--rw-r--r--   0        0        0     3279 2023-11-01 17:52:44.244904 protokolo-0.3.0/tests/test_replace.py
--rw-r--r--   0        0        0     6706 1970-01-01 00:00:00.000000 protokolo-0.3.0/setup.py
--rw-r--r--   0        0        0     6281 1970-01-01 00:00:00.000000 protokolo-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2147 2024-04-09 10:54:02.994443 protokolo-1.0.0/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-1.0.0/LICENSES/
+-rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-1.0.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-1.0.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-1.0.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     6944 2024-04-09 10:45:20.520978 protokolo-1.0.0/README.md
+-rw-r--r--   0        0        0     2770 2024-04-09 10:53:06.853855 protokolo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      177 2024-04-09 10:53:06.853855 protokolo-1.0.0/src/protokolo/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-07 10:30:16.712348 protokolo-1.0.0/src/protokolo/__main__.py
+-rw-r--r--   0        0        0     3825 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/_formatter.py
+-rw-r--r--   0        0        0     1435 2024-03-08 18:20:59.913097 protokolo-1.0.0/src/protokolo/_util.py
+-rw-r--r--   0        0        0     7982 2024-04-09 07:14:59.883614 protokolo-1.0.0/src/protokolo/cli.py
+-rw-r--r--   0        0        0    10126 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/compile.py
+-rw-r--r--   0        0        0    11712 2024-04-08 09:03:05.349473 protokolo-1.0.0/src/protokolo/config.py
+-rw-r--r--   0        0        0     3245 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/exceptions.py
+-rw-r--r--   0        0        0     3773 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/initialise.py
+-rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-1.0.0/src/protokolo/py.typed
+-rw-r--r--   0        0        0     1520 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/replace.py
+-rw-r--r--   0        0        0      931 2024-04-09 10:25:50.336818 protokolo-1.0.0/src/protokolo/types.py
+-rw-r--r--   0        0        0     2231 2024-04-09 10:25:50.336818 protokolo-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0    18278 2024-04-09 10:25:50.336818 protokolo-1.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0    15949 2024-04-09 07:02:10.527188 protokolo-1.0.0/tests/test_compile.py
+-rw-r--r--   0        0        0    11411 2024-03-29 19:44:07.383769 protokolo-1.0.0/tests/test_config.py
+-rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-1.0.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6053 2024-04-09 10:25:50.336818 protokolo-1.0.0/tests/test_formatter.py
+-rw-r--r--   0        0        0     4040 2024-04-09 07:02:10.527188 protokolo-1.0.0/tests/test_replace.py
+-rw-r--r--   0        0        0     8018 1970-01-01 00:00:00.000000 protokolo-1.0.0/setup.py
+-rw-r--r--   0        0        0     7914 1970-01-01 00:00:00.000000 protokolo-1.0.0/PKG-INFO
```

### Comparing `protokolo-0.3.0/CHANGELOG.md` & `protokolo-1.0.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,22 +12,40 @@
 - `Added` for new features.
 - `Changed` for changes in existing functionality.
 - `Deprecated` for soon-to-be removed features.
 - `Removed` for now removed features.
 - `Fixed` for any bug fixes.
 - `Security` in case of vulnerabilities.
 
+The versions follow [semantic versioning](https://semver.org) for the
+`protokolo` CLI command and its behaviour. There are no guarantees of stability
+for the `protokolo` Python library.
+
 <!-- protokolo-section-tag -->
 
+## 1.0.0 - 2024-04-09
+
+### Changed
+
+- Renamed the concept of 'entry' to 'fragment'.
+- Changed the way newlines are handled for fragments. Newlines surrounding
+  fragments are now significant when concatenation of fragments happens.
+  However, a _lack_ of final is considered an error, and one is always added.
+  The foremost consequence of this change is that list items now concatenate
+  without a blank line between them.
+
+### Fixed
+
+- Newline at the end of CHANGELOG is retained after `protokolo compile`.
+
 ## 0.3.0 - 2024-04-07
 
 ### Added
 
 - Added `--dry-run` to `compile`.
-
 - Added `--format` to `compile`. This is primarily useful for doing something
   like `protokolo compile --format version 1.0.0` to format the correct version
   into the section heading.
 
 ### Changed
 
 - Re-wrote the internals to use the `attrs` library for easier validation.
```

### Comparing `protokolo-0.3.0/LICENSES/CC-BY-SA-4.0.txt` & `protokolo-1.0.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-0.3.0/LICENSES/CC0-1.0.txt` & `protokolo-1.0.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-0.3.0/LICENSES/GPL-3.0-or-later.txt` & `protokolo-1.0.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `protokolo-0.3.0/README.md` & `protokolo-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 [![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
 [![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
 Protokolo is a change log generator.
 
-Protokolo allows you to maintain your change log entries in separate files, and
-then finally aggregate them into a new section in CHANGELOG just before release.
+Protokolo allows you to maintain your change log fragments in separate files,
+and then finally aggregate them into a new section in CHANGELOG just before
+release.
 
-## Table of Contents
+## Table of contents
 
 - [Background](#background)
 - [Install](#install)
 - [Usage](#usage)
 - [Maintainers](#maintainers)
 - [Contributing](#contributing)
 - [License](#license)
@@ -31,35 +32,62 @@
 Unfortunately, they are also a bit of a pain when combined with version control:
 
 - If two pull requests edit CHANGELOG, there is a non-zero chance that you'll
   need to resolve a conflict when trying to merge them both.
 - Just after you make a release, you need to create a new section in CHANGELOG
   for your next release. If you forget this busywork, new feature branches will
   need to create this section, which increases the chance of merge conflicts.
-- If a feature branch adds a change log entry to the section for the next v1.2.3
-  release, and v1.2.3 subsequently releases without merging that feature branch,
+- If a feature branch adds a change log entry to the section for the next v2.0
+  release, and v2.0 subsequently releases without merging that feature branch,
   then merging that feature branch afterwards would still add the change log
-  entry to the v1.2.3 section, even though it should now go to the v1.3.0
+  entry to the v2.0 section, even though it should now go to the unreleased v3.0
   section.
 
 Life would be a lot easier if you didn't have to deal with these problems.
 
-Enter Protokolo. The idea is very simple: For every change log entry, create a
-new file. Finally, just before release, compile the contents of those files into
-a new section in CHANGELOG, and delete the files.
+Enter Protokolo
+([Esperanto for 'report' or 'minutes'](https://vortaro.net/#protokolo)). The
+idea is very simple: for every change log entry, create a new file. Finally,
+just before release, compile the contents of those files into a new section in
+CHANGELOG, and delete the files.
+
+### See also
+
+[Towncrier](https://github.com/twisted/towncrier) is an older and more widely
+used implementation of the same idea. Protokolo is distinct in that it uses a
+directory hierarchy instead of putting all metadata in the file name of each
+change log fragment. Furthermore, Protokolo does no fancy formatting of
+fragments---what you write is what you get.
+
+There are three main problems I encountered in Towncrier that Protokolo attempts
+to address:
+
+- When using Towncrier, I would always forget which fragment types are available
+  to me and had to look them up. These fragment types can also differ per
+  repository. In Protokolo, the types are always visible because they are
+  directories.
+- Towncrier fragments are sorted by their ID, which is typically an issue or PR
+  number. This isn't always what I want.
+- Because (some) Towncrier workflows put the PR number in the file name as
+  metadata, I would have to open the PR before I could create the change log
+  fragment.
+
+A much younger version of me also tried her hand at writing a program like this
+in [changelogdir](https://pypi.org/project/changelogdir/).
 
 ## Install
 
 Protokolo is a regular Python package. You can install it using
 `pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`
 with `pipx ensurepath`.
 
 ## Usage
 
-For full documentation and options, read the documentation at TODO.
+For full documentation and options, read the documentation at
+<https://protokolo.readthedocs.io>.
 
 ### Initial set-up
 
 To set up your project for use with Protokolo, run `protokolo init`. This will
 create a `CHANGELOG.md` file (if one did not already exist) and a directory
 structure under `changelog.d`. The directory structure uses the
 [Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking
@@ -82,56 +110,55 @@
 │   │   └── .protokolo.toml
 │   └── .protokolo.toml
 ├── CHANGELOG.md
 └── .protokolo.toml
 ```
 
 The `.protokolo.toml` files in `changelog.d` contain metadata for their
-respective sections; the section title, heading level, and order. Their
+respective sections: the section title, heading level, and order. Their
 inclusion is mandatory.
 
 The `.protokolo.toml` file in the root of the project contains configurations
 for Protokolo that reduce the amount of typing you need to do when running
 commands.
 
 If a `CHANGELOG.md` file already existed, make sure to add a line containing
 `<!-- protokolo-section-tag -->` just before the heading of the latest release.
 
-### Adding entries
+### Adding fragments
 
-To add a change log entry, create the file `changelog.d/added/my_feature.md`,
+To add a change log fragment, create the file `changelog.d/added/my_feature.md`,
 and write something like:
 
 ```markdown
 - Added `--my-new-feature` option.
 ```
 
-Note the item dash at the start; Protokolo does not add them for you. What you
+Note the item dash at the start---Protokolo does not add them for you. What you
 write is exactly what you get.
 
-You can add more files. Change log entries in the same section (read: directory)
-are sorted alphabetically by their file name. If you want to make certain that
-some change log entries go first or last, prefix the file with `000_` or `zzz_`.
-For example, you can create `changelog.d/added/000_important_feature.md` to make
-it appear first.
+You can add more files. Change log fragments in the same section (read:
+directory) are sorted alphabetically by their file name. If you want to make
+certain that some change log fragments go first or last, prefix the file with
+`000_` or `zzz_`. For example, you can create
+`changelog.d/added/000_important_feature.md` to make it appear first.
 
 ### Compiling your change log
 
 You compile your change log with `protokolo compile`. This will take all change
-log entries from `changelog.d` and put them in your `CHANGELOG.md`. If we run it
-now, the following section is added after the `<!-- protokolo-section-tag -->`
-comment:
+log fragments from `changelog.d` and put them in your `CHANGELOG.md`. If we run
+it now, the following section is added after the
+`<!-- protokolo-section-tag -->` comment:
 
 ```markdown
 ## ${version} - 2023-11-08
 
 ### Added
 
 - Added important feature.
-
 - Added `--my-new-feature` option.
 ```
 
 The Markdown files in `changelog.d/added/` are deleted. You can manually replace
 `${version}` with a release version, or you can pass the option
 `--format version 1.0.0` to `protokolo compile` to format the heading at compile
 time.
```

### Comparing `protokolo-0.3.0/pyproject.toml` & `protokolo-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "protokolo"
-version = "0.3.0"
+version = "1.0.0"
 description = "Protokolo is a change log generator."
 authors = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
 maintainers = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
 license = "GPL-3.0-or-later"
 readme = "README.md"
+homepage = "https://codeberg.org/carmenbianca/protokolo"
+repository = "https://codeberg.org/carmenbianca/protokolo"
+documentation = "https://protokolo.readthedocs.io"
+keywords = ["changelog", "history", "news"]
+classifiers = [
+    "Intended Audience :: Developers",
+    "Topic :: Documentation",
+    "Topic :: Software Development :: Documentation",
+    "Topic :: Utilities"
+]
 
 packages = [
     { include = "protokolo", from = "src" }
 ]
 include = [
     { path = "tests", format = "sdist" },
     { path = "README.md", format = "sdist" },
@@ -65,38 +75,33 @@
 pyls-isort = "*"
 python-lsp-black = "*"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.protokolo]
-changelog = "CHANGELOG.md"
-markup = "markdown"
-directory = "changelog.d"
-
 [bumpver]
-current_version = "0.3.0"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message = "Bump version to {new_version}"
+current_version = "v1.0.0"
+version_pattern = "vMAJOR.MINOR.PATCH"
+commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
 tag = false
 push = false
 
 [bumpver.file_patterns]
 "pyproject.toml" = [
-    '^version = "{version}"$',
+    '^version = "{pep440_version}"$',
     '^current_version = "{version}"$',
 ]
 "src/protokolo/__init__.py" = [
-    '^__version__ = "{version}"$',
+    '^__version__ = "{pep440_version}"$',
 ]
 
 [tool.black]
 line-length = 80
 
 [tool.isort]
 multi_line_output = 3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `protokolo-0.3.0/src/protokolo/_formatter.py` & `protokolo-1.0.0/src/protokolo/_formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,21 +82,22 @@
 class ReStructuredTextFormatter(MarkupFormatter):
     """A reStructuredText formatter."""
 
     # TODO: Honestly this should be more flexible, but the amount of engineering
     # it would take to achieve that is beyond the scope of what I want to do.
     # What were the designers of reST thinking when they didn't define the
     # heading hierarchy?
+    #
+    # These are borrowed from Pandoc.
     _levels = {
-        1: "=",  # Special case.
-        2: "=",
-        3: "-",
-        4: "~",
-        5: "^",
-        6: "'",
+        1: "=",
+        2: "-",
+        3: "~",
+        4: "^",
+        5: "'",
     }
 
     @classmethod
     def _validate(cls, attrs: SectionAttributes) -> None:
         super()._validate(attrs)
         if attrs.level > len(cls._levels):
             raise HeadingFormatError(
@@ -105,23 +106,22 @@
 
     @classmethod
     def _format_section(cls, title: str, attrs: SectionAttributes) -> str:
         sign = cls._levels[attrs.level]
         length = len(title)
         return cleandoc(
             f"""
-            {sign * length if attrs.level == 1 else ''}
             {title}
             {sign * length}
             """
         )
 
 
 MARKUP_FORMATTER_MAPPING = {
     "markdown": MarkdownFormatter,
     "restructuredtext": ReStructuredTextFormatter,
 }
 
 MARKUP_EXTENSION_MAPPING = {
-    "markdown": {".md", ".markdown", ""},
+    "markdown": {".md", ".markdown"},
     "restructuredtext": {".rst"},
 }
```

### Comparing `protokolo-0.3.0/src/protokolo/_util.py` & `protokolo-1.0.0/src/protokolo/_util.py`

 * *Files identical despite different names*

### Comparing `protokolo-0.3.0/src/protokolo/cli.py` & `protokolo-1.0.0/src/protokolo/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 def compile_(
     changelog: click.File,
     markup: SupportedMarkup,
     format_: tuple[tuple[str, str], ...],
     dry_run: bool,
     directory: Path,
 ) -> None:
-    """Aggregate all change log entries from files in a directory into a
+    """Aggregate all change log fragments from files in a directory into a
     CHANGELOG file.
 
     A change log directory should contain a '.protokolo.toml' file that defines
     some attributes of the section. This is an example file:
 
     \b
     [protokolo.section]
@@ -121,15 +121,15 @@
     level = 2
 
     When the section is compiled, it looks a little like this:
 
     ## 1.0.0 - 2023-11-08
 
     The heading is followed by the contents of files in the section's directory.
-    If a section is empty (no change log entries), it is not compiled.
+    If a section is empty (no change log fragments), it is not compiled.
 
     The CHANGELOG file should contain the following comment, which is the
     location in the file after which the compiled section will be pasted:
 
     \b
     <!-- protokolo-section-tag -->
 
@@ -155,15 +155,15 @@
     # Compile Section
     try:
         new_section = section.compile()
     except HeadingFormatError as error:
         raise click.UsageError(str(error)) from error
 
     if not new_section:
-        click.echo("There are no change log entries to compile.")
+        click.echo("There are no change log fragments to compile.")
         return
 
     # Write to CHANGELOG
     try:
         fp: TextIOWrapper
         with changelog.open() as fp:  # type: ignore
             # TODO: use buffer reading, probably
@@ -181,17 +181,17 @@
             else:
                 fp.seek(0)
                 fp.write(new_contents)
                 fp.truncate()
     except OSError as error:
         # TODO: This is a little tricky to test. click already exits early if
         # changelog isn't readable/writable.
-        raise click.UsageError(str(error))
+        raise click.UsageError(str(error)) from error
 
-    # Delete change log entries
+    # Delete change log fragments
     if not dry_run:
         for dirpath, _, filenames in os.walk(directory):
             for filename in filenames:
                 path = Path(dirpath) / filename
                 if path.suffix in _MARKUP_EXTENSION_MAPPING[markup]:
                     path.unlink()
 
@@ -210,15 +210,15 @@
     show_default="determined by config, or changelog.d",
     type=click.Path(
         file_okay=False,
         dir_okay=True,
         readable=True,
         path_type=Path,
     ),
-    help="Directory of change log sections and entries.",
+    help="Directory of change log sections and fragments.",
 )
 @click.option(
     "--markup",
     default="markdown",
     show_default="determined by config, or markdown",
     type=click.Choice(SupportedMarkup.__args__),  # type: ignore
     help="Markup language.",
@@ -256,8 +256,8 @@
     .protokolo.toml file, which is always (re-)generated.
     """
     try:
         create_changelog(changelog.name, markup)
         create_keep_a_changelog(directory)
         create_root_toml(changelog.name, markup, directory)
     except OSError as error:
-        raise click.UsageError(str(error))
+        raise click.UsageError(str(error)) from error
```

### Comparing `protokolo-0.3.0/src/protokolo/compile.py` & `protokolo-1.0.0/src/protokolo/compile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-"""Code to combine the files in protokolo/ into a single text block."""
+"""Code to combine the files in ``changelog.d/`` into a single text block."""
 
 import errno
 import tomllib
 from io import StringIO
 from itertools import chain
 from operator import attrgetter
 from os import strerror
@@ -27,36 +27,38 @@
 )
 from .types import StrPath, SupportedMarkup
 
 # pylint: disable=too-few-public-methods
 
 
 @attrs_.define(frozen=True)
-class Entry:
-    """An entry, analogous to a file."""
+class Fragment:
+    """A fragment, analogous to a file."""
 
     text: str
     source: Path | None = attrs_.field(default=None, converter=optional(Path))
 
     def compile(self) -> str:
-        """Compile the entry. For the time being, this just means stripping the
-        newline characters around the text.
+        """Compile the fragment. For the time being, this just means adding a
+        newline at the end if one does not exist.
         """
-        return self.text.strip("\n")
+        if not self.text.endswith("\n"):
+            return f"{self.text}\n"
+        return self.text
 
 
 @attrs_.define(eq=False)
 class Section:
     """A section, analogous to a directory."""
 
     attrs: SectionAttributes = attrs_.field(factory=SectionAttributes)
     markup: SupportedMarkup = "markdown"
     source: Path | None = attrs_.field(default=None, converter=optional(Path))
 
-    entries: set[Entry] = attrs_.field(factory=set, init=False)
+    fragments: set[Fragment] = attrs_.field(factory=set, init=False)
     subsections: set[Self] = attrs_.field(factory=set, init=False)
 
     @classmethod
     def from_directory(
         cls,
         directory: StrPath,
         level: int = 1,
@@ -86,15 +88,15 @@
         if section_format_pairs is None:
             section_format_pairs = {}
 
         directory = Path(directory)
         section = cls(markup=markup, source=directory)
 
         section._load_section_attributes(directory, level, section_format_pairs)
-        section._load_subsections_and_entries(
+        section._load_subsections_and_fragments(
             directory, section.attrs.level, section_format_pairs
         )
 
         return section
 
     def _load_section_attributes(
         self, directory: Path, level: int, section_format_pairs: dict[str, str]
@@ -134,31 +136,31 @@
         # in the toml, second by the level value.
         level = values.get("level") or level
         attrs.level = level
         for key, val in section_format_pairs.items():
             attrs[key] = val
         self.attrs = attrs
 
-    def _load_subsections_and_entries(
+    def _load_subsections_and_fragments(
         self, directory: Path, level: int, section_format_pairs: dict[str, str]
     ) -> None:
-        """Locate subsections and entries. Load entries onto self, and
+        """Locate subsections and fragments. Load fragments onto self, and
         recursively create subsections to also load them onto self.
 
         Raises:
             OSError: input/output error.
             ProtokoloTOMLNotFoundError: ``.protokolo.toml`` doesn't exist.
             ProtokoloTOMLIsADirectoryError: ``.protokolo.toml`` is not a file.
             tomllib.TOMLDecodeError: ``.protokolo.toml`` couldn't be parsed.
             DictTypeError: ``.protokolo.toml`` fields have the wrong type.
             AttributeNotPositiveError: value in ``.protokolo.toml`` should be a
                 positive integer.
         """
         subsections = set()
-        entries = set()
+        fragments = set()
         for path in directory.iterdir():
             if path.is_dir():
                 subsections.add(
                     self.from_directory(
                         path,
                         level=level + 1,
                         markup=self.markup,
@@ -167,21 +169,21 @@
                 )
             elif (
                 path.is_file()
                 and path.suffix in _MARKUP_EXTENSION_MAPPING[self.markup]
             ):
                 with path.open("r", encoding="utf-8") as fp_:
                     content = fp_.read()
-                    entries.add(Entry(text=content, source=path))
+                    fragments.add(Fragment(text=content, source=path))
         self.subsections = cast(set[Self], subsections)
-        self.entries = entries
+        self.fragments = fragments
 
     def compile(self) -> str:
-        """Compile the entire section recursively, first printing the entries in
-        order, then the subsections.
+        """Compile the entire section recursively, first printing the fragments
+        in order, then the subsections.
 
         Empty sections are not compiled.
 
         Raises:
             HeadingFormatError: could not format heading of section.
         """
         buffer = self.write_to_buffer()
@@ -205,52 +207,56 @@
             )
         except HeadingFormatError as error:
             raise HeadingFormatError(
                 f"Failed to format section heading of {repr(str(self.source))}:"
                 f" {str(error)}"
             ) from error
         buffer.write(heading)
+        buffer.write("\n")
 
-        for entry in self.sorted_entries():
-            buffer.write("\n\n")
-            buffer.write(entry.compile())
+        if self.fragments:
+            buffer.write("\n")
+        for fragment in self.sorted_fragments():
+            buffer.write(fragment.compile())
 
         for subsection in self.sorted_subsections():
             if not subsection.is_empty():
-                buffer.write("\n\n")
+                buffer.write("\n")
             subsection.write_to_buffer(buffer=buffer)
 
         return buffer
 
     def is_empty(self) -> bool:
-        """A :class:`Section` is empty if it contains neither entries nor
-        subsections. If it contains no entries, and its subsections are empty,
+        """A :class:`Section` is empty if it contains neither fragments nor
+        subsections. If it contains no fragments, and its subsections are empty,
         then it is also considered empty.
         """
-        if self.entries:
+        if self.fragments:
             return False
         if not self.subsections:
             return True
         for subsection in self.subsections:
             if not subsection.is_empty():
                 return False
         return True
 
-    def sorted_entries(self) -> Iterator[Entry]:
-        """Yield the entries, ordered by their source. Entries that do not have
-        a source are sorted afterwards by their text.
+    def sorted_fragments(self) -> Iterator[Fragment]:
+        """Yield the fragments, ordered by their source. Fragments that do not
+        have a source are sorted afterwards by their text.
         """
         with_source = {
-            entry for entry in self.entries if entry.source is not None
+            fragment
+            for fragment in self.fragments
+            if fragment.source is not None
         }
         source_sorted = sorted(
-            with_source, key=lambda entry: cast(Path, entry.source).name
+            with_source, key=lambda fragment: cast(Path, fragment.source).name
         )
         alphabetical_sorted = sorted(
-            self.entries - with_source, key=attrgetter("text")
+            self.fragments - with_source, key=attrgetter("text")
         )
         return chain(source_sorted, alphabetical_sorted)
 
     def sorted_subsections(self) -> Iterator[Self]:
         """Yield the subsections, first ordered by their order value, then the
         remainder sorted alphabetically.
         """
```

### Comparing `protokolo-0.3.0/src/protokolo/config.py` & `protokolo-1.0.0/src/protokolo/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,13 +337,13 @@
 
     @markup.setter
     def markup(self, value: str | None) -> None:
         self["markup"] = value
 
     @property
     def directory(self) -> str | None:
-        """The directory where the change log entries are stored."""
+        """The directory where the change log fragments are stored."""
         return cast(str | None, self["directory"])
 
     @directory.setter
     def directory(self, value: str | None) -> None:
         self["directory"] = value
```

### Comparing `protokolo-0.3.0/src/protokolo/exceptions.py` & `protokolo-1.0.0/src/protokolo/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 """Exception classes."""
 
 from operator import attrgetter
 from typing import Any
 
 
 class ProtokoloError(Exception):
-    """Common exception class for all custom errors raised by protokolo."""
+    """Common exception class for all custom errors raised by the
+    :mod:`protokolo` module.
+    """
 
 
 class DictTypeError(TypeError, ProtokoloError):
     """Expected a value of a different type for a given key."""
 
     def __init__(self, *args: Any):
         if (args_count := len(args)) > 4:
@@ -68,33 +70,35 @@
         try:
             return args[index]
         except IndexError:
             return default
 
 
 class DictTypeListError(DictTypeError):
-    """Like DictTypeError, but the item is in a list (inside of a dictionary)
-    instead of in a dictionary.
+    """Like :class:`DictTypeError`, but the item is in a list (inside of a
+    dictionary) instead of in a dictionary.
     """
 
     def _key_text(self) -> str:
         return f"List {repr(self.key)} contains an element with the wrong type."
 
 
 class ProtokoloTOMLError(ProtokoloError):
-    """An exception that pertains to .protokolo.toml."""
+    """An exception that pertains to ``.protokolo.toml.``"""
 
 
 class AttributeNotPositiveError(ValueError, ProtokoloTOMLError):
-    """A value in AttributeSections is expected to be a positive integer."""
+    """A value in :class:`.config.SectionAttributes` is expected to be a
+    positive integer.
+    """
 
 
 class ProtokoloTOMLNotFoundError(FileNotFoundError, ProtokoloTOMLError):
-    """Couldn't find a .protokolo.toml file."""
+    """Couldn't find a ``.protokolo.toml`` file."""
 
 
 class ProtokoloTOMLIsADirectoryError(IsADirectoryError, ProtokoloTOMLError):
-    """.protokolo.toml is not a file."""
+    """``.protokolo.toml`` is not a file."""
 
 
 class HeadingFormatError(ValueError, ProtokoloError):
     """Could not create heading."""
```

### Comparing `protokolo-0.3.0/src/protokolo/initialise.py` & `protokolo-1.0.0/src/protokolo/initialise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-"""Code related to `protokolo init`."""
+"""Code related to ``protokolo init``."""
 
 from pathlib import Path
 
 from ._util import cleandoc
 from .types import StrPath, SupportedMarkup
 
 CHANGELOG_MD = """# Change log
@@ -19,16 +19,15 @@
 - `Deprecated` for soon-to-be removed features.
 - `Removed` for now removed features.
 - `Fixed` for any bug fixes.
 - `Security` in case of vulnerabilities.
 
 <!-- protokolo-section-tag -->
 """
-CHANGELOG_RST = """==========
-Change log
+CHANGELOG_RST = """Change log
 ==========
 
 This change log follows the `Keep a Changelog <http://keepachangelog.com/>`_
 recommendations. Every release contains the following sections:
 
 - ``Added`` for new features.
 - ``Changed`` for changes in existing functionality.
@@ -95,15 +94,15 @@
                 encoding="utf-8",
             )
 
 
 def create_root_toml(
     changelog: StrPath, markup: SupportedMarkup | None, directory: StrPath
 ) -> None:
-    """Create a .protokolo.toml file in the current working directory."""
+    """Create a ``.protokolo.toml`` file in the current working directory."""
     if markup is None:
         markup = "markdown"
 
     Path(".protokolo.toml").write_text(
         cleandoc(
             """
             [protokolo]
```

### Comparing `protokolo-0.3.0/src/protokolo/types.py` & `protokolo-1.0.0/src/protokolo/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,11 +27,11 @@
     | bool
     | datetime
     | date
     | None
     | TOMLType
     | list["TOMLType"]
 )
-#: Like :ref:`TOMLValue`, but using only Python primitives.
+#: Like :data:`TOMLValue`, but using only Python primitives.
 TOMLValueType: UnionType = (
     str | int | float | bool | datetime | date | None | dict | list
 )
```

### Comparing `protokolo-0.3.0/tests/conftest.py` & `protokolo-1.0.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,33 +28,34 @@
             <!-- protokolo-section-tag -->
 
             ## 0.1.0 - 2020-01-01
 
             First release.
             """
         )
+        + "\n"
     )
     (directory / "CHANGELOG.rst").write_text(
         cleandoc(
             """
-            ==========
             Change log
             ==========
 
             Lorem ipsum.
 
             ..
                 protokolo-section-tag
 
             0.1.0 - 2020-01-01
-            ==================
+            ------------------
 
             First release.
             """
         )
+        + "\n"
     )
 
     changelog_d = directory / "changelog.d"
     changelog_d.mkdir()
     (changelog_d / ".protokolo.toml").write_text(
         cleandoc(
             """
```

### Comparing `protokolo-0.3.0/tests/test_cli.py` & `protokolo-1.0.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
                 Foo
 
                 ## 0.1.0 - 2020-01-01
                 """
             )
             in changelog
         )
+        assert changelog.endswith("\n")
         assert not Path("changelog.d/foo.md").exists()
 
     @freeze_time("2023-11-08")
     def test_with_format(self, runner):
         """The simple case, but using --format."""
         Path("changelog.d/foo.md").write_text("Foo")
         result = runner.invoke(
@@ -317,29 +318,31 @@
         assert result.exit_code != 0
         assert (
             "Error: Failed to format section heading of 'changelog.d': Heading"
             " level 10 is too deep." in result.output
         )
 
     def test_nothing_to_compile(self, runner):
-        """There are no change log entries."""
+        """There are no change log fragments."""
         changelog = Path("CHANGELOG.md").read_text()
         result = runner.invoke(
             main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
             ],
         )
         assert result.exit_code == 0
-        assert result.output == "There are no change log entries to compile.\n"
+        assert (
+            result.output == "There are no change log fragments to compile.\n"
+        )
         assert Path("CHANGELOG.md").read_text() == changelog
 
     def test_no_replacement_tag(self, runner):
         """There is no protokolo-section-tag in CHANGELOG."""
         Path("CHANGELOG.md").write_text("Hello, world!")
         Path("changelog.d/foo.md").write_text("Foo")
         result = runner.invoke(
@@ -356,16 +359,16 @@
         assert result.exit_code != 0
         assert (
             "Error: There is no 'protokolo-section-tag' in 'CHANGELOG.md'"
             in result.output
         )
 
     @freeze_time("2023-11-08")
-    def test_nested_entries_deleted(self, runner):
-        """Entries in nested sections are also deleted, but other files are
+    def test_nested_fragments_deleted(self, runner):
+        """Fragments in nested sections are also deleted, but other files are
         not.
         """
         Path("changelog.d/feature/foo.md").write_text("Foo")
         Path("changelog.d/feature/bar.txt").write_text("Bar")
         result = runner.invoke(
             main,
             [
@@ -425,25 +428,25 @@
                 """
                 Lorem ipsum.
 
                 ..
                     protokolo-section-tag
 
                 ${version} - 2023-11-08
-                =======================
+                -----------------------
 
                 Foo
 
                 Features
-                --------
+                ~~~~~~~~
 
                 Bar
 
                 0.1.0 - 2020-01-01
-                ==================
+                ------------------
                 """
             )
             in changelog
         )
         assert not Path("changelog.d/feature/bar.rst").exists()
         assert not Path("changelog.d/foo.rst").exists()
 
@@ -542,18 +545,15 @@
 
     def test_markup_option(self, empty_runner):
         """Use with --markup option."""
         result = empty_runner.invoke(
             main, ["init", "--markup", "restructuredtext"]
         )
         assert result.exit_code == 0
-        assert (
-            "==========\nChange log\n=========="
-            in Path("CHANGELOG.md").read_text()
-        )
+        assert "Change log\n==========" in Path("CHANGELOG.md").read_text()
         assert (
             'markup = "restructuredtext"' in Path(".protokolo.toml").read_text()
         )
 
     def test_directory_option(self, empty_runner):
         """Use with --directory option."""
         result = empty_runner.invoke(main, ["init", "--directory", "foo"])
```

### Comparing `protokolo-0.3.0/tests/test_compile.py` & `protokolo-1.0.0/tests/test_compile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-"""Test the compilation of change log sections and entries."""
+"""Test the compilation of change log sections and fragments."""
 
 import random
 import tomllib
 from inspect import cleandoc
 
 import pytest
 
-from protokolo.compile import Entry, Section
+from protokolo.compile import Fragment, Section
 from protokolo.config import SectionAttributes
 from protokolo.exceptions import (
     AttributeNotPositiveError,
     DictTypeError,
     ProtokoloTOMLIsADirectoryError,
     ProtokoloTOMLNotFoundError,
 )
@@ -22,40 +22,78 @@
 # pylint: disable=too-many-public-methods
 
 
 class TestSection:
     """Collect all tests for Section."""
 
     def test_compile_simple(self):
-        """Test the compilation of a very simple section with one entry and one
-        subsection.
+        """Test the compilation of a very simple section with one fragment and
+        one subsection.
         """
         subsection = Section(
             attrs=SectionAttributes(title="Subsection", level=2)
         )
-        subsection.entries.add(Entry("- world"))
+        subsection.fragments.add(Fragment("- world"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
-        section.entries.add(Entry("- hello"))
+        section.fragments.add(Fragment("- hello"))
         section.subsections.add(subsection)
 
-        expected = cleandoc(
-            """
-            # Section
+        expected = (
+            cleandoc(
+                """
+                # Section
+
+                - hello
+
+                ## Subsection
+
+                - world
+                """
+            )
+            + "\n"
+        )
+        assert section.compile() == expected
+
+    def test_compile_multiple_fragments(self):
+        """Test the compilation of a single section with multiple fragments.
+
+        In this test, there are three types of newline configurations for
+        fragments:
 
-            - hello
+        - None
+        - One newline
+        - More newlines
+        """
+        section = Section(attrs=SectionAttributes(title="Section", level=1))
+        section.fragments.add(Fragment("- A", source="a"))
+        section.fragments.add(Fragment("- B\n", source="b"))
+        section.fragments.add(Fragment("- C\n\n", source="c"))
+        section.fragments.add(Fragment("- D", source="d"))
+        section.fragments.add(Fragment("\n- E", source="e"))
+
+        expected = (
+            cleandoc(
+                """
+                # Section
+
+                - A
+                - B
+                - C
 
-            ## Subsection
+                - D
 
-            - world
-            """
+                - E
+                """
+            )
+            + "\n"
         )
         assert section.compile() == expected
 
     def test_compile_empty(self):
-        """A section that contains neither entries nor subsections doesn't
+        """A section that contains neither fragments nor subsections doesn't
         compile to anything.
         """
         section = Section()
         assert section.compile() == ""
 
     def test_compile_empty_subsections(self):
         """A section that only contains empty subsections doesn't compile to
@@ -69,236 +107,255 @@
     def test_compile_one_empty_subsection(self):
         """If one subsection is empty, and the other is not, the empty
         subsection should not be compiled.
         """
         subsection_1 = Section(
             attrs=SectionAttributes(title="Subsection Foo", level=2, order=1)
         )
-        subsection_1.entries.add(Entry("Foo"))
+        subsection_1.fragments.add(Fragment("Foo"))
         subsection_2 = Section(
             attrs=SectionAttributes(title="Subsection Bar", level=2, order=2)
         )
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.add(subsection_1)
         section.subsections.add(subsection_2)
 
-        expected = cleandoc(
-            """
-            # Section
+        expected = (
+            cleandoc(
+                """
+                # Section
 
-            ## Subsection Foo
+                ## Subsection Foo
 
-            Foo
-            """
+                Foo
+                """
+            )
+            + "\n"
         )
         assert section.compile() == expected
 
     def test_compile_order_specified(self):
         """Respect the order specified on the subsection."""
         subsection_1 = Section(
             attrs=SectionAttributes(title="Subsection Foo", level=2, order=1)
         )
-        subsection_1.entries.add(Entry("Foo"))
+        subsection_1.fragments.add(Fragment("Foo"))
         subsection_2 = Section(
             attrs=SectionAttributes(title="Subsection Bar", level=2, order=2)
         )
-        subsection_2.entries.add(Entry("Bar"))
+        subsection_2.fragments.add(Fragment("Bar"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.add(subsection_1)
         section.subsections.add(subsection_2)
 
-        expected = cleandoc(
-            """
-            # Section
+        expected = (
+            cleandoc(
+                """
+                # Section
 
-            ## Subsection Foo
+                ## Subsection Foo
 
-            Foo
+                Foo
 
-            ## Subsection Bar
+                ## Subsection Bar
 
-            Bar
-            """
+                Bar
+                """
+            )
+            + "\n"
         )
         assert section.compile() == expected
 
     def test_compile_order_alphabetic(self):
         """If no orders are specified, sort subsections alphabetically."""
         subsection_1 = Section(
             attrs=SectionAttributes(title="Subsection Foo", level=2)
         )
-        subsection_1.entries.add(Entry("Foo"))
+        subsection_1.fragments.add(Fragment("Foo"))
         subsection_2 = Section(
             attrs=SectionAttributes(title="Subsection Bar", level=2)
         )
-        subsection_2.entries.add(Entry("Bar"))
+        subsection_2.fragments.add(Fragment("Bar"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.add(subsection_1)
         section.subsections.add(subsection_2)
 
-        expected = cleandoc(
-            """
-            # Section
+        expected = (
+            cleandoc(
+                """
+                # Section
 
-            ## Subsection Bar
+                ## Subsection Bar
 
-            Bar
+                Bar
 
-            ## Subsection Foo
+                ## Subsection Foo
 
-            Foo
-            """
+                Foo
+                """
+            )
+            + "\n"
         )
         assert section.compile() == expected
 
     def test_compile_order_mixed(self):
         """Ordered subsections are sorted first, and all subsections with
         unspecified order are sorted afterwards, alphabetically.
         """
         subsection_1 = Section(
             attrs=SectionAttributes(title="Subsection Foo", level=2, order=1)
         )
-        subsection_1.entries.add(Entry("Foo"))
+        subsection_1.fragments.add(Fragment("Foo"))
         subsection_2 = Section(
             attrs=SectionAttributes(title="Subsection Bar", level=2, order=2)
         )
-        subsection_2.entries.add(Entry("Bar"))
+        subsection_2.fragments.add(Fragment("Bar"))
         subsection_3 = Section(
             attrs=SectionAttributes(title="Subsection Baz", level=2)
         )
-        subsection_3.entries.add(Entry("Baz"))
+        subsection_3.fragments.add(Fragment("Baz"))
         subsection_4 = Section(
             attrs=SectionAttributes(title="Subsection Quz", level=2)
         )
-        subsection_4.entries.add(Entry("Quz"))
+        subsection_4.fragments.add(Fragment("Quz"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.update(
             {subsection_1, subsection_2, subsection_3, subsection_4}
         )
-        expected = cleandoc(
-            """
-            # Section
+        expected = (
+            cleandoc(
+                """
+                # Section
 
-            ## Subsection Foo
+                ## Subsection Foo
 
-            Foo
+                Foo
 
-            ## Subsection Bar
+                ## Subsection Bar
 
-            Bar
+                Bar
 
-            ## Subsection Baz
+                ## Subsection Baz
 
-            Baz
+                Baz
 
-            ## Subsection Quz
+                ## Subsection Quz
 
-            Quz
-            """
+                Quz
+                """
+            )
+            + "\n"
         )
         assert section.compile() == expected
 
     def test_compile_order_same_order(self):
         """If two sections have the same order number, sort alphabetically."""
         subsection_1 = Section(
             attrs=SectionAttributes(title="Subsection Foo", level=2, order=1)
         )
-        subsection_1.entries.add(Entry("Foo"))
+        subsection_1.fragments.add(Fragment("Foo"))
         subsection_2 = Section(
             attrs=SectionAttributes(title="Subsection Bar", level=2, order=1)
         )
-        subsection_2.entries.add(Entry("Bar"))
+        subsection_2.fragments.add(Fragment("Bar"))
         section = Section(attrs=SectionAttributes(title="Section", level=1))
         section.subsections.add(subsection_1)
         section.subsections.add(subsection_2)
 
-        expected = cleandoc(
-            """
-            # Section
+        expected = (
+            cleandoc(
+                """
+                # Section
 
-            ## Subsection Bar
+                ## Subsection Bar
 
-            Bar
+                Bar
 
-            ## Subsection Foo
+                ## Subsection Foo
 
-            Foo
-            """
+                Foo
+                """
+            )
+            + "\n"
         )
         assert section.compile() == expected
 
-    def test_compile_entries_sorted_by_source(self):
-        """Compiled entries are sorted by their source."""
+    def test_compile_fragments_sorted_by_source(self):
+        """Compiled fragments are sorted by their source."""
         section = Section(attrs=SectionAttributes(title="Section"))
-        entries = {
+        fragments = {
             f"{source_nr}.md": str(random.randint(1, 10_000))
             for source_nr in range(10)
         }
-        for source, text in entries.items():
-            section.entries.add(Entry(text, source=source))
+        for source, text in fragments.items():
+            section.fragments.add(Fragment(text, source=source))
 
-        expected = "# Section\n\n" + "\n\n".join(
-            item[1] for item in sorted(entries.items())
+        expected = (
+            "# Section\n\n"
+            + "\n".join(item[1] for item in sorted(fragments.items()))
+            + "\n"
         )
         assert section.compile() == expected
 
-    def test_compile_entries_sorted_by_text(self):
-        """Compiled entries are sorted alphabetically by their text if they have
-        no source.
+    def test_compile_fragments_sorted_by_text(self):
+        """Compiled fragments are sorted alphabetically by their text if they
+        have no source.
         """
         section = Section(attrs=SectionAttributes(title="Section"))
-        entries = {str(random.randint(1, 10_000)) for _ in range(10)}
-        for text in entries:
-            section.entries.add(Entry(text))
+        fragments = {str(random.randint(1, 10_000)) for _ in range(10)}
+        for text in fragments:
+            section.fragments.add(Fragment(text))
 
-        expected = "# Section\n\n" + "\n\n".join(sorted(entries))
+        expected = "# Section\n\n" + "\n".join(sorted(fragments)) + "\n"
         assert section.compile() == expected
 
-    def test_compile_entries_sorted_mixed(self):
-        """Compiled entries that have a source are sorted before ones that
+    def test_compile_fragments_sorted_mixed(self):
+        """Compiled fragments that have a source are sorted before ones that
         don't.
         """
         section = Section(attrs=SectionAttributes(title="Section"))
-        section.entries.add(Entry("Foo", source="foo.md"))
-        section.entries.add(Entry("Bar"))
+        section.fragments.add(Fragment("- Foo", source="foo.md"))
+        section.fragments.add(Fragment("- Bar"))
 
-        expected = cleandoc(
-            """
-            # Section
-
-            Foo
+        expected = (
+            cleandoc(
+                """
+                # Section
 
-            Bar
-            """
+                - Foo
+                - Bar
+                """
+            )
+            + "\n"
         )
         assert section.compile() == expected
 
     def test_is_empty_simple(self):
-        """A section with neither entries nor subsections is empty."""
+        """A section with neither fragments nor subsections is empty."""
         section = Section()
         assert section.is_empty()
 
-    def test_is_empty_contains_entries(self):
-        """A section with entries is not empty."""
+    def test_is_empty_contains_fragments(self):
+        """A section with fragments is not empty."""
         section = Section()
-        section.entries.add(Entry("Foo"))
+        section.fragments.add(Fragment("Foo"))
         assert not section.is_empty()
 
     def test_is_empty_with_empty_subsections(self):
         """A section with empty subsections is empty."""
         subsection = Section()
         section = Section()
         section.subsections.add(subsection)
         assert subsection.is_empty()
         assert section.is_empty()
 
     def test_is_empty_with_nonempty_subsections(self):
         """A section with non-empty subsections is not empty."""
         subsection = Section()
-        subsection.entries.add(Entry("Hello"))
+        subsection.fragments.add(Fragment("Hello"))
         section = Section()
         section.subsections.add(subsection)
         assert not subsection.is_empty()
         assert not section.is_empty()
 
     def test_from_directory(self, project_dir):
         """A very simple case of generating a Section from a directory."""
@@ -311,26 +368,26 @@
         section = Section.from_directory(project_dir / "changelog.d")
         assert section.attrs.level == 2
         assert (
             # Strange pylint false positive here.
             section.attrs.title  # pylint: disable=no-member
             == "${version} - ${date}"
         )
-        assert len(section.entries) == 1
-        announcement = next(iter(section.entries))
+        assert len(section.fragments) == 1
+        announcement = next(iter(section.fragments))
         assert announcement.text == "Hello, world!"
         assert (
             announcement.source == project_dir / "changelog.d/announcement.md"
         )
         assert len(section.subsections) == 1
         subsection = next(iter(section.subsections))
         assert subsection.attrs.level == 3
         assert subsection.attrs.title == "Features"
-        assert len(subsection.entries) == 1
-        feature = next(iter(subsection.entries))
+        assert len(subsection.fragments) == 1
+        feature = next(iter(subsection.fragments))
         assert feature.text == "- Added feature."
         assert (
             feature.source == project_dir / "changelog.d/feature/feature_1.md"
         )
 
     def test_from_directory_additional_format_pairs(self, project_dir):
         """Provide additional section format pairs to Section, and make sure
@@ -415,19 +472,19 @@
             Section.from_directory(project_dir / "changelog.d")
         error = exc_info.value
         assert error.filename == str(
             project_dir / "changelog.d/.protokolo.toml"
         )
 
 
-class TestEntry:
-    """Collect all tests for Entry."""
+class TestFragment:
+    """Collect all tests for Fragment."""
 
     def test_compile_simple(self):
-        """Compile a simple entry."""
-        entry = Entry("Hello, world!")
-        assert entry.compile() == "Hello, world!"
-
-    def test_compile_newlines(self):
-        """Strip newlines from entry."""
-        entry = Entry("\n\n\nFoo\n\n\n\n\n")
-        assert entry.compile() == "Foo"
+        """Compile a simple fragment."""
+        fragment = Fragment("Hello, world!\n")
+        assert fragment.compile() == "Hello, world!\n"
+
+    def test_compile_no_newline_at_end(self):
+        """Add missing newline to fragment."""
+        fragment = Fragment("Foo")
+        assert fragment.compile() == "Foo\n"
```

### Comparing `protokolo-0.3.0/tests/test_config.py` & `protokolo-1.0.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `protokolo-0.3.0/tests/test_exceptions.py` & `protokolo-1.0.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-0.3.0/tests/test_formatter.py` & `protokolo-1.0.0/tests/test_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,39 +145,38 @@
 
     def test_format_section_one_level(self):
         """Format an h1 section."""
         assert ReStructuredTextFormatter.format_section(
             SectionAttributes(title="Foo", level=1)
         ) == cleandoc(
             """
-            ===
             Foo
             ===
             """
         )
 
     def test_format_section_two_levels(self):
         """Format an h2 section."""
         assert ReStructuredTextFormatter.format_section(
             SectionAttributes(title="Foo Bar Baz", level=2)
         ) == cleandoc(
             """
             Foo Bar Baz
-            ===========
+            -----------
             """
         )
 
     def test_format_section_three_levels(self):
         """Format an h3 section."""
         assert ReStructuredTextFormatter.format_section(
             SectionAttributes(title="Hello, world", level=3)
         ) == cleandoc(
             """
             Hello, world
-            ------------
+            ~~~~~~~~~~~~
             """
         )
 
     def test_format_section_level_too_deep(self):
         """Very deep sections are not supported."""
         with pytest.raises(HeadingFormatError):
             ReStructuredTextFormatter.format_section(
@@ -186,12 +185,11 @@
 
     def test_format_with_replacement(self):
         """The length of the section symbols adjusts to the rendered text."""
         assert ReStructuredTextFormatter.format_section(
             SectionAttributes(title="Foo $bar", level=1, values={"bar": "bar"})
         ) == cleandoc(
             """
-            =======
             Foo bar
             =======
             """
         )
```

### Comparing `protokolo-0.3.0/tests/test_replace.py` & `protokolo-1.0.0/tests/test_replace.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,16 @@
             """
             Line 1
             Line 2
             Foo
             Line 3
             """
         )
+        # The newline is implicit.
+        assert insert_into_str("Foo\n", target, 2) == expected
         assert insert_into_str("Foo", target, 2) == expected
 
     def test_insert_into_str_multiple_lines(self):
         """Insert multiple lines into a string."""
         target = cleandoc(
             """
             Line 1
@@ -60,15 +62,15 @@
             )
             == expected
         )
 
     def test_insert_into_str_target_empty(self):
         """Insert into an empty target."""
         target = ""
-        expected = "Foo"
+        expected = "Foo\n"
         assert insert_into_str("Foo", target, 0) == expected
 
     def test_insert_into_str_text_empty(self):
         """Insert empty string into target."""
         target = cleandoc(
             """
             Line 1
@@ -82,22 +84,26 @@
         """Insert at the end of the target."""
         target = cleandoc(
             """
             Line 1
             Line 2
             """
         )
-        expected = cleandoc(
-            """
-            Line 1
-            Line 2
-            Foo
-            """
+        expected = (
+            cleandoc(
+                """
+                Line 1
+                Line 2
+                Foo
+                """
+            )
+            + "\n"
         )
         assert insert_into_str("Foo", target, 2) == expected
+        assert insert_into_str("Foo\n", target, 2) == expected
 
     def test_insert_into_str_start(self):
         """Insert at the start of the target."""
         target = cleandoc(
             """
             Line 1
             Line 2
@@ -108,14 +114,37 @@
             Foo
             Line 1
             Line 2
             """
         )
         assert insert_into_str("Foo", target, 0) == expected
 
+    def test_insert_into_str_keep_newline_at_end(self):
+        """The newline at the end is preserved."""
+        target = (
+            cleandoc(
+                """
+                Line 1
+                Line 2
+                """
+            )
+            + "\n"
+        )
+        expected = (
+            cleandoc(
+                """
+                Foo
+                Line 1
+                Line 2
+                """
+            )
+            + "\n"
+        )
+        assert insert_into_str("Foo", target, 0) == expected
+
 
 class TestFindFirstOccurrence:
     """Collect all tests for find_first_occurrence."""
 
     def test_find_first_occurrence_simple(self):
         """Simple case."""
         source = cleandoc(
```

### Comparing `protokolo-0.3.0/PKG-INFO` & `protokolo-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: protokolo
-Version: 0.3.0
+Version: 1.0.0
 Summary: Protokolo is a change log generator.
+Home-page: https://codeberg.org/carmenbianca/protokolo
 License: GPL-3.0-or-later
+Keywords: changelog,history,news
 Author: Carmen Bianca BAKKER
 Author-email: carmen@carmenbianca.eu
 Maintainer: Carmen Bianca BAKKER
 Maintainer-email: carmen@carmenbianca.eu
 Requires-Python: >=3.11,<4.0
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Utilities
 Requires-Dist: attrs (>=22.1.0)
 Requires-Dist: click (>=8.0)
+Project-URL: Documentation, https://protokolo.readthedocs.io
+Project-URL: Repository, https://codeberg.org/carmenbianca/protokolo
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 
 SPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later
 -->
@@ -26,18 +34,19 @@
 [![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
 [![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 
 Protokolo is a change log generator.
 
-Protokolo allows you to maintain your change log entries in separate files, and
-then finally aggregate them into a new section in CHANGELOG just before release.
+Protokolo allows you to maintain your change log fragments in separate files,
+and then finally aggregate them into a new section in CHANGELOG just before
+release.
 
-## Table of Contents
+## Table of contents
 
 - [Background](#background)
 - [Install](#install)
 - [Usage](#usage)
 - [Maintainers](#maintainers)
 - [Contributing](#contributing)
 - [License](#license)
@@ -48,35 +57,62 @@
 Unfortunately, they are also a bit of a pain when combined with version control:
 
 - If two pull requests edit CHANGELOG, there is a non-zero chance that you'll
   need to resolve a conflict when trying to merge them both.
 - Just after you make a release, you need to create a new section in CHANGELOG
   for your next release. If you forget this busywork, new feature branches will
   need to create this section, which increases the chance of merge conflicts.
-- If a feature branch adds a change log entry to the section for the next v1.2.3
-  release, and v1.2.3 subsequently releases without merging that feature branch,
+- If a feature branch adds a change log entry to the section for the next v2.0
+  release, and v2.0 subsequently releases without merging that feature branch,
   then merging that feature branch afterwards would still add the change log
-  entry to the v1.2.3 section, even though it should now go to the v1.3.0
+  entry to the v2.0 section, even though it should now go to the unreleased v3.0
   section.
 
 Life would be a lot easier if you didn't have to deal with these problems.
 
-Enter Protokolo. The idea is very simple: For every change log entry, create a
-new file. Finally, just before release, compile the contents of those files into
-a new section in CHANGELOG, and delete the files.
+Enter Protokolo
+([Esperanto for 'report' or 'minutes'](https://vortaro.net/#protokolo)). The
+idea is very simple: for every change log entry, create a new file. Finally,
+just before release, compile the contents of those files into a new section in
+CHANGELOG, and delete the files.
+
+### See also
+
+[Towncrier](https://github.com/twisted/towncrier) is an older and more widely
+used implementation of the same idea. Protokolo is distinct in that it uses a
+directory hierarchy instead of putting all metadata in the file name of each
+change log fragment. Furthermore, Protokolo does no fancy formatting of
+fragments---what you write is what you get.
+
+There are three main problems I encountered in Towncrier that Protokolo attempts
+to address:
+
+- When using Towncrier, I would always forget which fragment types are available
+  to me and had to look them up. These fragment types can also differ per
+  repository. In Protokolo, the types are always visible because they are
+  directories.
+- Towncrier fragments are sorted by their ID, which is typically an issue or PR
+  number. This isn't always what I want.
+- Because (some) Towncrier workflows put the PR number in the file name as
+  metadata, I would have to open the PR before I could create the change log
+  fragment.
+
+A much younger version of me also tried her hand at writing a program like this
+in [changelogdir](https://pypi.org/project/changelogdir/).
 
 ## Install
 
 Protokolo is a regular Python package. You can install it using
 `pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`
 with `pipx ensurepath`.
 
 ## Usage
 
-For full documentation and options, read the documentation at TODO.
+For full documentation and options, read the documentation at
+<https://protokolo.readthedocs.io>.
 
 ### Initial set-up
 
 To set up your project for use with Protokolo, run `protokolo init`. This will
 create a `CHANGELOG.md` file (if one did not already exist) and a directory
 structure under `changelog.d`. The directory structure uses the
 [Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking
@@ -99,56 +135,55 @@
 │   │   └── .protokolo.toml
 │   └── .protokolo.toml
 ├── CHANGELOG.md
 └── .protokolo.toml
 ```
 
 The `.protokolo.toml` files in `changelog.d` contain metadata for their
-respective sections; the section title, heading level, and order. Their
+respective sections: the section title, heading level, and order. Their
 inclusion is mandatory.
 
 The `.protokolo.toml` file in the root of the project contains configurations
 for Protokolo that reduce the amount of typing you need to do when running
 commands.
 
 If a `CHANGELOG.md` file already existed, make sure to add a line containing
 `<!-- protokolo-section-tag -->` just before the heading of the latest release.
 
-### Adding entries
+### Adding fragments
 
-To add a change log entry, create the file `changelog.d/added/my_feature.md`,
+To add a change log fragment, create the file `changelog.d/added/my_feature.md`,
 and write something like:
 
 ```markdown
 - Added `--my-new-feature` option.
 ```
 
-Note the item dash at the start; Protokolo does not add them for you. What you
+Note the item dash at the start---Protokolo does not add them for you. What you
 write is exactly what you get.
 
-You can add more files. Change log entries in the same section (read: directory)
-are sorted alphabetically by their file name. If you want to make certain that
-some change log entries go first or last, prefix the file with `000_` or `zzz_`.
-For example, you can create `changelog.d/added/000_important_feature.md` to make
-it appear first.
+You can add more files. Change log fragments in the same section (read:
+directory) are sorted alphabetically by their file name. If you want to make
+certain that some change log fragments go first or last, prefix the file with
+`000_` or `zzz_`. For example, you can create
+`changelog.d/added/000_important_feature.md` to make it appear first.
 
 ### Compiling your change log
 
 You compile your change log with `protokolo compile`. This will take all change
-log entries from `changelog.d` and put them in your `CHANGELOG.md`. If we run it
-now, the following section is added after the `<!-- protokolo-section-tag -->`
-comment:
+log fragments from `changelog.d` and put them in your `CHANGELOG.md`. If we run
+it now, the following section is added after the
+`<!-- protokolo-section-tag -->` comment:
 
 ```markdown
 ## ${version} - 2023-11-08
 
 ### Added
 
 - Added important feature.
-
 - Added `--my-new-feature` option.
 ```
 
 The Markdown files in `changelog.d/added/` are deleted. You can manually replace
 `${version}` with a release version, or you can pass the option
 `--format version 1.0.0` to `protokolo compile` to format the heading at compile
 time.
```

