# Comparing `tmp/mypy_json_report-1.1.0.tar.gz` & `tmp/mypy_json_report-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_json_report-1.1.0.tar", max compression
+gzip compressed data, was "mypy_json_report-1.2.0.tar", max compression
```

## Comparing `mypy_json_report-1.1.0.tar` & `mypy_json_report-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0    10702 2024-01-03 15:27:10.283623 mypy_json_report-1.1.0/LICENSE
--rw-r--r--   0        0        0     2331 2024-01-03 15:27:10.283623 mypy_json_report-1.1.0/README.md
--rw-r--r--   0        0        0    13217 2024-01-03 15:27:10.283623 mypy_json_report-1.1.0/mypy_json_report.py
--rw-r--r--   0        0        0     1530 2024-01-03 15:27:10.283623 mypy_json_report-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3296 1970-01-01 00:00:00.000000 mypy_json_report-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10702 2024-04-09 07:36:52.072417 mypy_json_report-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2331 2024-04-09 07:36:52.072417 mypy_json_report-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 07:36:52.072417 mypy_json_report-1.2.0/mypy_json_report/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-09 07:36:52.072417 mypy_json_report-1.2.0/mypy_json_report/__main__.py
+-rw-r--r--   0        0        0     3998 2024-04-09 07:36:52.072417 mypy_json_report-1.2.0/mypy_json_report/cli.py
+-rw-r--r--   0        0        0      834 2024-04-09 07:36:52.072417 mypy_json_report-1.2.0/mypy_json_report/exit_codes.py
+-rw-r--r--   0        0        0    11006 2024-04-09 07:36:52.072417 mypy_json_report-1.2.0/mypy_json_report/parse.py
+-rw-r--r--   0        0        0     1557 2024-04-09 07:36:52.076417 mypy_json_report-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3296 1970-01-01 00:00:00.000000 mypy_json_report-1.2.0/PKG-INFO
```

### Comparing `mypy_json_report-1.1.0/LICENSE` & `mypy_json_report-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_json_report-1.1.0/README.md` & `mypy_json_report-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mypy_json_report-1.1.0/mypy_json_report.py` & `mypy_json_report-1.2.0/mypy_json_report/parse.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,165 +8,75 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import argparse
-import enum
 import itertools
 import json
 import operator
-import pathlib
 import sys
-import textwrap
 from collections import Counter, defaultdict
 from dataclasses import dataclass
 from typing import (
     Any,
     Callable,
     Counter as CounterType,
     Dict,
     Iterable,
     Iterator,
     List,
-    Optional,
     Protocol,
-    Union,
-    cast,
 )
 
+from mypy_json_report.exit_codes import ExitCode
 
-class ErrorCodes(enum.IntEnum):
-    # 1 is returned when an uncaught exception is raised.
-    # Argparse returns 2 when bad args are passed.
-    ERROR_DIFF = 3
-    DEPRECATED = 4
 
-
-def main() -> None:
-    """
-    The primary entrypoint of the program.
-
-    Parses the CLI flags, and delegates to other functions as appropriate.
-    For details of how to invoke the program, call it with `--help`.
-    """
-    parser = argparse.ArgumentParser()
-    subparsers = parser.add_subparsers(title="subcommand")
-
-    parser.set_defaults(func=_no_command)
-
-    parse_parser = subparsers.add_parser(
-        "parse", help="Transform Mypy output into JSON."
-    )
-    parse_parser.add_argument(
-        "-i",
-        "--indentation",
-        type=int,
-        default=2,
-        help="Number of spaces to indent JSON output.",
-    )
-    parse_parser.add_argument(
-        "-o",
-        "--output-file",
-        type=pathlib.Path,
-        help="The file to write the JSON report to. If omitted, the report will be written to STDOUT.",
-    )
-    parse_parser.add_argument(
-        "-d",
-        "--diff-old-report",
-        default=None,
-        type=pathlib.Path,
-        help=textwrap.dedent(
-            f"""\
-            An old report to compare against. We will compare the errors in there to the new report.
-            Fail with return code {ErrorCodes.ERROR_DIFF} if we discover any new errors.
-            New errors will be printed to stderr.
-            Similar errors from the same file will also be printed
-            (because we don't know which error is the new one).
-            For completeness other hints and errors on the same lines are also printed.
-            """
-        ),
-    )
-    parse_parser.add_argument(
-        "-c",
-        "--color",
-        "--colour",
-        action="store_true",
-        help="Whether to colorize the diff-report output. Defaults to False.",
-    )
-
-    parse_parser.set_defaults(func=_parse_command)
-
-    parsed = parser.parse_args()
-    parsed.func(parsed)
+ErrorSummary = Dict[str, Dict[str, int]]
 
 
-ErrorSummary = Dict[str, Dict[str, int]]
+class MessageProcessor(Protocol):
+    def process_messages(self, filename: str, messages: List["MypyMessage"]) -> None:
+        ...
 
+    def write_report(self) -> ExitCode:
+        ...
 
-def _load_json_file(filepath: pathlib.Path) -> Any:
-    with filepath.open() as json_file:
-        return json.load(json_file)
-
-
-def _parse_command(args: argparse.Namespace) -> None:
-    """Handle the `parse` command."""
-    if args.output_file:
-        report_writer = args.output_file.write_text
-    else:
-        report_writer = sys.stdout.write
-    processors: List[Union[ErrorCounter, ChangeTracker]] = [
-        ErrorCounter(report_writer=report_writer, indentation=args.indentation)
-    ]
-
-    # If we have access to an old report, add the ChangeTracker processor.
-    tracker = None
-    if args.diff_old_report is not None:
-        old_report = cast(ErrorSummary, _load_json_file(args.diff_old_report))
-        change_report_writer: _ChangeReportWriter
-        if args.color:
-            change_report_writer = ColorChangeReportWriter()
-        else:
-            change_report_writer = DefaultChangeReportWriter()
-        tracker = ChangeTracker(old_report, report_writer=change_report_writer)
-        processors.append(tracker)
 
-    messages = MypyMessage.from_lines(sys.stdin)
+def parse_message_lines(
+    processors: List[MessageProcessor], lines: Iterable[str]
+) -> ExitCode:
+    messages = MypyMessage.from_lines(lines)
 
     # Sort the lines by the filename otherwise itertools.groupby() will make
     # multiple groups for the same file name if the lines are out of order.
     messages_sorted = sorted(messages, key=operator.attrgetter("filename"))
 
     for filename, messages in itertools.groupby(
         messages_sorted, key=operator.attrgetter("filename")
     ):
         # Send each line of the Mypy report to each processor.
         message_group = list(messages)
         for processor in processors:
             processor.process_messages(filename, message_group)
 
     for processor in processors:
-        error_code = processor.write_report()
-        if error_code is not None:
-            sys.exit(error_code)
+        exit_code = processor.write_report()
+        if exit_code is not ExitCode.SUCCESS:
+            return exit_code
 
+    return ExitCode.SUCCESS
 
-def _no_command(args: argparse.Namespace) -> None:
-    """
-    Handle the lack of an explicit command.
 
-    This will be hit when the program is called without arguments.
-    """
-    print("A subcommand is required. Pass --help for usage info.", file=sys.stderr)
-    sys.exit(ErrorCodes.DEPRECATED)
+class FilenameWithoutLineNumberError(Exception):
+    pass
 
 
-class ParseError(Exception):
+class SkipLineError(Exception):
     pass
 
 
 @dataclass(frozen=True)
 class MypyMessage:
     filename: str
     line_number: int
@@ -176,26 +86,40 @@
 
     @classmethod
     def from_lines(cls, lines: Iterable[str]) -> Iterator["MypyMessage"]:
         """Given lines from mypy's output, yield a series of MypyMessage objects."""
         for line in lines:
             try:
                 yield MypyMessage.from_line(line)
-            except ParseError:
+            except SkipLineError:
                 continue
 
     @classmethod
     def from_line(cls, line: str) -> "MypyMessage":
         try:
             location, message_type, message = line.strip().split(": ", 2)
         except ValueError as e:
             # Expected to happen on summary lines.
             # We could avoid this by requiring --no-error-summary
-            raise ParseError from e
-        filename, line_number, *_ = location.split(":")
+            raise SkipLineError from e
+
+        try:
+            filename, line_number, *_ = location.split(":")
+        except ValueError:
+            # This happens if the line contains a filename but no line number.
+            # We don't have any good way of handling those error messages right now,
+            # and in most cases it's probably an indicator of mypy warning about a problem with the file as a whole.
+            # In these cases we want the parsing to stop and emit the line that couldn't be parsed.
+            raise FilenameWithoutLineNumberError(
+                "Error message from mypy contains a filename but no line number. "
+                "This is normally an indication of a file-level issue reported by mypy. "
+                "Please correct this and try again. The error emitted from mypy is:\n\n"
+                f"    {line.strip()}"
+            )
+
         return MypyMessage(
             filename=filename,
             line_number=int(line_number),
             message=message,
             message_type=message_type,
             raw=line.rstrip(),
         )
@@ -224,18 +148,19 @@
 
     def process_messages(self, filename: str, messages: List[MypyMessage]) -> None:
         error_strings = (m.message for m in messages if m.message_type == "error")
         counted_errors = Counter(error_strings)
         if counted_errors:
             self.grouped_errors[filename] = counted_errors
 
-    def write_report(self) -> None:
+    def write_report(self) -> ExitCode:
         errors = self.grouped_errors
         error_json = json.dumps(errors, sort_keys=True, indent=self.indentation)
         self.report_writer(error_json + "\n")
+        return ExitCode.SUCCESS
 
 
 @dataclass(frozen=True)
 class DiffReport:
     error_lines: List[str]
     total_errors: int
     num_new_errors: int
@@ -389,18 +314,14 @@
         return DiffReport(
             error_lines=self.error_lines,
             total_errors=self.num_errors,
             num_new_errors=self.num_new_errors,
             num_fixed_errors=self.num_fixed_errors + unseen_errors,
         )
 
-    def write_report(self) -> Optional[ErrorCodes]:
+    def write_report(self) -> ExitCode:
         diff = self.diff_report()
         self.report_writer.write_report(diff)
 
         if diff.num_new_errors or diff.num_fixed_errors:
-            return ErrorCodes.ERROR_DIFF
-        return None
-
-
-if __name__ == "__main__":
-    main()
+            return ExitCode.ERROR_DIFF
+        return ExitCode.SUCCESS
```

### Comparing `mypy_json_report-1.1.0/pyproject.toml` & `mypy_json_report-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mypy-json-report"
-version = "1.1.0"
+version = "1.2.0"
 description = "Generate a JSON report from your mypy output"
 authors = ["Charlie Denton <charlie@meshy.co.uk>"]
 license = "Apache-2.0"
 repository = "https://github.com/memrise/mypy-json-report"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
@@ -30,33 +30,35 @@
 [tool.poetry.group.dev.dependencies]
 mypy = "*"
 pytest = "*"
 tox = "*"
 tox-gh-actions = "*"
 
 [tool.poetry.scripts]
-mypy-json-report = "mypy_json_report:main"
+mypy-json-report = "mypy_json_report.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py38"
+
+[tool.ruff.lint]
 select = [
     "E",  # pycodestyle
     "F",  # Pyflakes
     "I",  # isort
     "PL",  # Pylint
     "UP",  # pyupgrade
 ]
 ignore = [
     "E501",  # Line too long
 ]
 
-[tool.ruff.format]
-skip-magic-trailing-comma = true
-
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 lines-after-imports = 2
 split-on-trailing-comma = false
+
+[tool.ruff.format]
+skip-magic-trailing-comma = true
```

### Comparing `mypy_json_report-1.1.0/PKG-INFO` & `mypy_json_report-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-json-report
-Version: 1.1.0
+Version: 1.2.0
 Summary: Generate a JSON report from your mypy output
 Home-page: https://github.com/memrise/mypy-json-report
 License: Apache-2.0
 Author: Charlie Denton
 Author-email: charlie@meshy.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

