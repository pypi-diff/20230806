# Comparing `tmp/mypy_upgrade-0.0.1a3.tar.gz` & `tmp/mypy_upgrade-0.0.1a4.tar.gz`

## Comparing `mypy_upgrade-0.0.1a3.tar` & `mypy_upgrade-0.0.1a4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/__main__.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/cli.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/editing.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/filter.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/py.typed
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/silence.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/mypy_upgrade/utils.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/.gitignore
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/AUTHORS.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/LICENSE.txt
--rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/README.md
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/__main__.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/cli.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/editing.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/filter.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/py.typed
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/silence.py
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/utils.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/.gitignore
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/AUTHORS.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/LICENSE.txt
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/README.md
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/PKG-INFO
```

### Comparing `mypy_upgrade-0.0.1a3/mypy_upgrade/cli.py` & `mypy_upgrade-0.0.1a4/mypy_upgrade/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,45 +50,54 @@
 """,
     )
     parser.add_argument(
         "-m",
         "--module",
         default=[],
         dest="modules",
+        metavar="MODULE",
         action="append",
         help="Silence errors from the provided (importable) module. "
         "This flag may be repeated multiple times.",
     )
     parser.add_argument(
         "-p",
         "--package",
         default=[],
         dest="packages",
+        metavar="PACKAGE",
         action="append",
         help="Silence errors from the provided (importable) package. "
         "This flag may be repeated multiple times.",
     )
     parser.add_argument(
         "-r",
         "--report",
         type=pathlib.Path,
         help="""
         The path to a text file containing a mypy type checking report. If not
-        specified, input is read from stdin.
+        specified, input is read from standard input.
         """,
     )
     parser.add_argument(
         "-d",
-        "--with-descriptions",
-        action="store_const",
-        const="description",
-        dest="suffix",
+        "--description-style",
+        default="none",
+        choices=["full", "none"],
         help="""
-        Use this flag to include the mypy error descriptions in the error
-        suppression comment.
+        Specify the style in which mypy error descriptions are expressed in the
+        error suppression comment.
+        """,
+    )
+    parser.add_argument(
+        "--fix-me",
+        default="FIX ME",
+        help="""
+        Specify a custom 'Fix Me' message to be placed after the error
+        suppression comment. Pass " " to omit a 'Fix Me' message altogether.
         """,
     )
     parser.add_argument(
         "-v",
         "--verbose",
         action="append_const",
         const=True,
@@ -105,74 +114,91 @@
 
 
 def mypy_upgrade(
     report: pathlib.Path | None,
     packages: list[str],
     modules: list[str],
     files: list[str],
-    suffix: Literal["description"] | None,
+    description_style: Literal["full", "none"],
+    fix_me: str,
 ) -> tuple[list[MypyError], list[str]]:
     """Main logic for application.
 
     Args:
         report: a text file object representing the mypy error report.
         packages: a list of string representing the packages in which to
             silence errors.
         modules: a list of string representing the modules in which to
             silence errors.
         files: a list of string representing the files in which to
             silence errors.
-        suffix: an optional string specifying the type of suffix.
+        description_style: a string specifying the style of error descriptions
+            appended to the end of error suppression comments.
+        fix_me: a string specifying the 'Fix Me' message in type error
+            suppresion comments. Pass " " to omit a 'Fix Me' message
+            altogether.
 
     Returns:
-        A two-tuple whose first element is a list of MypyErrors that were
+        A 2-tuple whose first element is a list of MypyErrors that were
         silenced and whose second element is the list of modules in which
         errors were silenced.
     """
     if report is not None:
         with pathlib.Path(report).open(encoding="utf-8") as file:
             errors = parse_mypy_report(file)
     else:
         errors = parse_mypy_report(sys.stdin)
 
     filtered_errors = filter_mypy_errors(errors, packages, modules, files)
 
     edited_files = []
+    excluded = []  # Do something with these
+    silenced_errors = []
     for filename, filename_grouped_errors in itertools.groupby(
         filtered_errors, key=lambda error: error.filename
     ):
         with pathlib.Path(filename).open(encoding="utf-8") as f:
-            line_number_corrected_errors, lines = correct_line_numbers(
+            safe_to_suppress, to_exclude = correct_line_numbers(
                 f, filename_grouped_errors
             )
+            f.seek(0)
+            lines = f.readlines()
+
+        excluded.extend(to_exclude)
 
         for line_number, line_grouped_errors in itertools.groupby(
-            line_number_corrected_errors, key=lambda error: error.line_no
+            safe_to_suppress, key=lambda error: error.line_no
         ):
             lines[line_number - 1] = silence_errors(
-                lines[line_number - 1], line_grouped_errors, suffix
+                lines[line_number - 1],
+                line_grouped_errors,
+                description_style,
+                fix_me.strip(),
             )
 
         with pathlib.Path(filename).open(mode="w", encoding="utf-8") as f:
             _ = f.write("".join(lines))
 
-        edited_files.append(filename)
+        if safe_to_suppress:
+            edited_files.append(filename)
+            silenced_errors.extend(safe_to_suppress)
 
-    return filtered_errors, edited_files
+    return silenced_errors, edited_files
 
 
 def main() -> None:
     """Logic for CLI."""
     parser = _create_argument_parser()
     args = parser.parse_args()
     errors, modules = mypy_upgrade(
         args.report,
         args.packages,
         args.modules,
         args.files,
-        args.suffix,
+        args.description_style,
+        args.fix_me.strip(),
     )
 
     if len(args.verbose) > 0:
         print(  # noqa: T201
             f"{len(errors)} errors silenced across {len(modules)} modules."
         )
```

### Comparing `mypy_upgrade-0.0.1a3/mypy_upgrade/editing.py` & `mypy_upgrade-0.0.1a4/mypy_upgrade/editing.py`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a3/mypy_upgrade/filter.py` & `mypy_upgrade-0.0.1a4/mypy_upgrade/filter.py`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a3/mypy_upgrade/parsing.py` & `mypy_upgrade-0.0.1a4/mypy_upgrade/parsing.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 import re
 from typing import NamedTuple, TextIO
 
 
 class MypyError(NamedTuple):
     filename: str
+    col_offset: int | None
     line_no: int
-    description: str
+    message: str
     error_code: str
 
     @staticmethod
     def filename_and_line_number(error: MypyError) -> tuple[str, int]:
         return error.filename, error.line_no
 
 
@@ -27,30 +28,41 @@
         A sorted list of MypyErrors. Elements are sorted by their filename
         and line_no attributes.
 
         Example::
 
             >> report = pathlib.Path('mypy_report.txt').open(encoding='utf-8')
             >> errors = parse_report(report)
-            >> module, line_no, description , error_code= errors[0]
+            >> module, col_offset, line_no, message , error_code= errors[0]
     """
     info = re.compile(
-        r"^(?P<filename>[^:]+):(?P<line_no>\d+): error: (?P<description>.+)\s+(\[(?P<error_code>.+)\])?"  # noqa: E501
+        r"^(?P<filename>[^:]+):(?P<line_no>\d+)(:(?P<col_offset>\d+))?"
+        r"(:\d+:\d+)?: error: (?P<message>.+)\s+(\[(?P<error_code>.+)\])?"
     )
     errors = []
 
     for line in report:
         error = info.match(line.strip())
         if error:
-            filename, description, error_code = error.group(
-                "filename", "description", "error_code"
-            )
+            error_code = error.group("error_code") or ""
+            filename, message = error.group("filename", "message")
             line_no = int(error.group("line_no"))
+            if error.group("col_offset"):
+                col_offset = int(error.group("col_offset"))
+            else:
+                col_offset = None
+
             errors.append(
-                MypyError(filename, line_no, description.strip(), error_code)
+                MypyError(
+                    filename,
+                    col_offset,
+                    line_no,
+                    message.strip(),
+                    error_code,
+                )
             )
 
     return sorted(errors, key=MypyError.filename_and_line_number)
 
 
 def description_to_type_ignore(description: str) -> tuple[str, ...]:
     type_ignore_re = re.compile(
```

### Comparing `mypy_upgrade-0.0.1a3/mypy_upgrade/silence.py` & `mypy_upgrade-0.0.1a4/mypy_upgrade/silence.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,39 +17,43 @@
 from mypy_upgrade.parsing import MypyError, description_to_type_ignore
 from mypy_upgrade.utils import split_code_and_comment
 
 
 def silence_errors(
     line: str,
     errors: Iterable[MypyError],
-    suffix: Literal["description"] | None,
+    description_style: Literal["full", "none"],
+    fix_me: str,
 ) -> str:
     """Silences the given error on a line with an error code-specific comment.
 
     Args:
         line: a string containing the line.
-        error_code: a string representing the mypy error code.
-        description: a string representing a description of the error.
+        error: an `Iterable` of `MypyError`s to be silenced.
+        description_style: a string specifying the style of the description of
+            errors.
+        fix_me: a string specifying a "fix me" message to be appended after the
+            silencing comment.
     Returns:
         The line with a type error suppression comment.
     """
     unused_ignore = None
     error_codes = []
     descriptions = []
     for error in errors:
         if error.error_code == "unused-ignore":
             unused_ignore = error  # there should only be one
         else:
             error_codes.append(error.error_code)
-            descriptions.append(error.description)
+            descriptions.append(error.message)
 
     python_code, comment = split_code_and_comment(line.rstrip())
 
     if unused_ignore:
-        codes_to_remove = description_to_type_ignore(unused_ignore.description)
+        codes_to_remove = description_to_type_ignore(unused_ignore.message)
         pruned_comment = remove_unused_type_ignore(comment, codes_to_remove)
         cleaned_comment = format_type_ignore_comment(pruned_comment)
     else:
         cleaned_comment = comment
 
     if error_codes:
         final_comment = add_type_ignore_comment(
@@ -57,11 +61,14 @@
             error_codes,
         )
     else:
         final_comment = cleaned_comment
 
     updated_line = f"{python_code}  {final_comment}".rstrip()
 
-    if suffix == "description" and descriptions:
+    if fix_me:
+        updated_line += f" # {fix_me.strip()}"
+
+    if description_style == "full" and descriptions:
         updated_line += f" # {', '.join(descriptions)}"
 
     return updated_line + "\n"
```

### Comparing `mypy_upgrade-0.0.1a3/.gitignore` & `mypy_upgrade-0.0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a3/LICENSE.txt` & `mypy_upgrade-0.0.1a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a3/README.md` & `mypy_upgrade-0.0.1a4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -11,39 +11,37 @@
 -----
 
 **Table of Contents**
 
 - [What is `mypy-upgrade`?](#what-is-mypy-upgrade)
 - [Features](#features)
 - [Basic Usage](#basic-usage)
+- [Recommended Mypy Flags](#recommended-mypy-flags)
 - [Command-Line Options](#command-line-options)
 - [Quick Start](#quick-start)
-- [Known Bugs](#known-bugs)
+- [Known Limitations](#known-limitations)
 - [Similar Projects](#similar-projects)
 
 ## What is `mypy-upgrade`?
 
 `mypy-upgrade` is a command-line utility that provides automatic error
 suppression for [`mypy`](http://mypy.readthedocs.io/) (analogous to [`pyre-upgrade`](https://pyre-check.org/docs/types-in-python/#upgrade) and [`pylint-silent`](https://github.com/udifuchs/pylint-silent/)).
 
-Given a type checking report from `mypy`,
-`mypy-upgrade` will silence the listed errors using error suppression
-comments. For example, with the following output from mypy:
+Given a type checking report from `mypy`, `mypy-upgrade` will silence
+the listed errors using error suppression comments. For example, with
+the following output from mypy:
 
     package/subpackage/module.py:13: error: Incompatible default for argument "filename" (default has type "None", argument has type "str") [assignment]
 
-`mypy-upgrade` will place a `# type: ignore[assignment]` comment at the
+`mypy-upgrade` will place a `# type: ignore[assignment] # FIX ME` comment at the
 end of line 13 in `package/subpackage/module.py`. If error codes are not
 present in the `mypy` report (e.g., the `hide-error-codes` flag is set when
-`mypy` was invoked), then a non-specific `# type: ignore` comment will be
+`mypy` was invoked), then a non-specific `# type: ignore # FIX ME` comment will be
 added instead.
 
-> :warning: **Warning:** `mypy-check` **must** be run in the same directory
-> that `mypy` was run.
-
 ## Features
 
 * Removal of unused `type: ignore` comments
 
 * Optional inclusion of `mypy` error description messages
 
 * Support for suppressing multiple mypy errors per-line
@@ -66,57 +64,93 @@
 
         mypy --strict -p my_package > mypy_report.txt
 
     and then pass the file to `mypy-upgrade`
 
         mypy-upgrade --report mypy_report.txt
 
-> :memo: **Note:** To ensure desired behaviour, packages and modules must be
-passed using their fully qualified names (e.g., `my_package.my_module`).
-
 ## Command-Line Options
 
-You may want to include the error descriptions provided by `mypy` in the
+You may want to include the error messages provided by `mypy` in the
 suppression comments so that you can fix them later. You can do so using
-the `-d` (or `--with-descriptions`) option
+the `-d` (or `--description-style`) option
+
+    mypy-upgrade --report mypy_report.txt -d full -p package
 
-    mypy-upgrade --report mypy_report.txt -d -p MY_PACKAGE
+You also customize the "fix me" message placed after the error suppression
+comment using the `--fix-me` option
+
+    mypy-upgrade --report mypy_report.txt --fix-me "FIX THIS" -p package
 
 To selectively silence errors in packages and modules, use the `-p`
-(`--package`) and `-m` (`--module`) options, respectively:
+(`--package`) and `-m` (`--module`) options along with the fully qualified
+module/package name, respectively:
+
+    mypy-upgrade --report mypy_report.txt -p package1 -p package2 -m package1.module1 -m package2.module2
 
 Similarly, to selectively silence errors in files and directories,
 pass them in as positional arguments:
 
     mypy-upgrade --report mypy_report.txt path/to/my_package/ path/to/a/module.py
 
 For a full list of all options and their descriptions, run
 
     mypy-upgrade --help
 
+## Recommended Mypy Flags
+
+To enable all checks utilized by `mypy-upgrade` to silence as many errors as possible, the
+following flags should be set when creating the type checking report to pass to `mypy-upgrade`:
+
+* `--show-absolute-path`
+
+    * Required if running `mypy-upgrade` in a separate directory than `mypy`
+
+* `--strict`
+
+    * This will ensure that `mypy-upgrade` will attempt to silence all possible mypy errors
+
+* `--show-column-numbers`
+
+    * This allows for more precise treatment of certain type error edge cases (e.g. type checking
+    errors before the start of multiline strings)
+
+* `--show-error-codes`
+
+    * This ensures that error-code specific comments are added instead of blanket `type: ignore`
+    comments
+
 ## Quick Start
 
 `mypy-upgrade` can be installed via `pip`.
 
     python3 -m pip install mypy-upgrade
 
 If you want to run the latest version of the code, you can install from the
 repo directly:
 
     python3 -m pip install -U git+https://github.com/ugognw/mypy-upgrade.git
     # or if you don't have 'git' installed
     python3 -m pip install -U https://github.com/ugognw/mypy-upgrade/tree/development
 
-## Known Bugs
+## Known Limitations
+
+The following limitations derive mainly from Python syntax issues and are unable to be handled
+by `mypy-upgrade`. If you can't resolve the error directly, please consider refactoring to permit
+error suppression.
+
+* Type errors on lines ending in line continuation characters or within multiline f-strings
+
+    * Comments are not permitted within multiline strings or following line continuation characters
+    and Mypy only recognizes inline `type: ignore` comments (see
+    [#3448](https://github.com/python/mypy/issues/3448))
 
-This utility is unable to silence mypy errors which occur on lines ending in
-line continuation characters since any non-whitespace following such a
-character is a syntax error. Pre-formatting your code with a PEP8 adherent
-formatter (e.g., [`black`](http://black.readthedocs.io)) to replace such lines with parentheses
-is recommended.
+    * Pre-formatting your code with a PEP8 adherent formatter
+    (e.g., [`black`](http://black.readthedocs.io)) to replace such lines with parentheses is
+    recommended.
 
 ## Similar Projects
 
 If this doesn't fit your use-case, maybe one of these other projects will!
 
 * [`geo7/mypy_clean_slate`](https://github.com/geo7/mypy_clean_slate/tree/main): `mypy` reports are generated internally in `--strict` mode; includes
 support for suppressing multiple errors on a single line; an inspiration for
```

### Comparing `mypy_upgrade-0.0.1a3/pyproject.toml` & `mypy_upgrade-0.0.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a3/PKG-INFO` & `mypy_upgrade-0.0.1a4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-upgrade
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: automatic error suppression for mypy
 Project-URL: Documentation, https://github.com/ugognw/mypy-upgrade#readme
 Project-URL: Issues, https://github.com/ugognw/mypy-upgrade/issues
 Project-URL: Source, https://github.com/ugognw/mypy-upgrade
 Author-email: Ugochukwu Nwosu <ugognw@gmail.com>
 License-Expression: MIT
 License-File: AUTHORS.md
@@ -37,39 +37,37 @@
 -----
 
 **Table of Contents**
 
 - [What is `mypy-upgrade`?](#what-is-mypy-upgrade)
 - [Features](#features)
 - [Basic Usage](#basic-usage)
+- [Recommended Mypy Flags](#recommended-mypy-flags)
 - [Command-Line Options](#command-line-options)
 - [Quick Start](#quick-start)
-- [Known Bugs](#known-bugs)
+- [Known Limitations](#known-limitations)
 - [Similar Projects](#similar-projects)
 
 ## What is `mypy-upgrade`?
 
 `mypy-upgrade` is a command-line utility that provides automatic error
 suppression for [`mypy`](http://mypy.readthedocs.io/) (analogous to [`pyre-upgrade`](https://pyre-check.org/docs/types-in-python/#upgrade) and [`pylint-silent`](https://github.com/udifuchs/pylint-silent/)).
 
-Given a type checking report from `mypy`,
-`mypy-upgrade` will silence the listed errors using error suppression
-comments. For example, with the following output from mypy:
+Given a type checking report from `mypy`, `mypy-upgrade` will silence
+the listed errors using error suppression comments. For example, with
+the following output from mypy:
 
     package/subpackage/module.py:13: error: Incompatible default for argument "filename" (default has type "None", argument has type "str") [assignment]
 
-`mypy-upgrade` will place a `# type: ignore[assignment]` comment at the
+`mypy-upgrade` will place a `# type: ignore[assignment] # FIX ME` comment at the
 end of line 13 in `package/subpackage/module.py`. If error codes are not
 present in the `mypy` report (e.g., the `hide-error-codes` flag is set when
-`mypy` was invoked), then a non-specific `# type: ignore` comment will be
+`mypy` was invoked), then a non-specific `# type: ignore # FIX ME` comment will be
 added instead.
 
-> :warning: **Warning:** `mypy-check` **must** be run in the same directory
-> that `mypy` was run.
-
 ## Features
 
 * Removal of unused `type: ignore` comments
 
 * Optional inclusion of `mypy` error description messages
 
 * Support for suppressing multiple mypy errors per-line
@@ -92,57 +90,93 @@
 
         mypy --strict -p my_package > mypy_report.txt
 
     and then pass the file to `mypy-upgrade`
 
         mypy-upgrade --report mypy_report.txt
 
-> :memo: **Note:** To ensure desired behaviour, packages and modules must be
-passed using their fully qualified names (e.g., `my_package.my_module`).
-
 ## Command-Line Options
 
-You may want to include the error descriptions provided by `mypy` in the
+You may want to include the error messages provided by `mypy` in the
 suppression comments so that you can fix them later. You can do so using
-the `-d` (or `--with-descriptions`) option
+the `-d` (or `--description-style`) option
+
+    mypy-upgrade --report mypy_report.txt -d full -p package
 
-    mypy-upgrade --report mypy_report.txt -d -p MY_PACKAGE
+You also customize the "fix me" message placed after the error suppression
+comment using the `--fix-me` option
+
+    mypy-upgrade --report mypy_report.txt --fix-me "FIX THIS" -p package
 
 To selectively silence errors in packages and modules, use the `-p`
-(`--package`) and `-m` (`--module`) options, respectively:
+(`--package`) and `-m` (`--module`) options along with the fully qualified
+module/package name, respectively:
+
+    mypy-upgrade --report mypy_report.txt -p package1 -p package2 -m package1.module1 -m package2.module2
 
 Similarly, to selectively silence errors in files and directories,
 pass them in as positional arguments:
 
     mypy-upgrade --report mypy_report.txt path/to/my_package/ path/to/a/module.py
 
 For a full list of all options and their descriptions, run
 
     mypy-upgrade --help
 
+## Recommended Mypy Flags
+
+To enable all checks utilized by `mypy-upgrade` to silence as many errors as possible, the
+following flags should be set when creating the type checking report to pass to `mypy-upgrade`:
+
+* `--show-absolute-path`
+
+    * Required if running `mypy-upgrade` in a separate directory than `mypy`
+
+* `--strict`
+
+    * This will ensure that `mypy-upgrade` will attempt to silence all possible mypy errors
+
+* `--show-column-numbers`
+
+    * This allows for more precise treatment of certain type error edge cases (e.g. type checking
+    errors before the start of multiline strings)
+
+* `--show-error-codes`
+
+    * This ensures that error-code specific comments are added instead of blanket `type: ignore`
+    comments
+
 ## Quick Start
 
 `mypy-upgrade` can be installed via `pip`.
 
     python3 -m pip install mypy-upgrade
 
 If you want to run the latest version of the code, you can install from the
 repo directly:
 
     python3 -m pip install -U git+https://github.com/ugognw/mypy-upgrade.git
     # or if you don't have 'git' installed
     python3 -m pip install -U https://github.com/ugognw/mypy-upgrade/tree/development
 
-## Known Bugs
+## Known Limitations
+
+The following limitations derive mainly from Python syntax issues and are unable to be handled
+by `mypy-upgrade`. If you can't resolve the error directly, please consider refactoring to permit
+error suppression.
+
+* Type errors on lines ending in line continuation characters or within multiline f-strings
+
+    * Comments are not permitted within multiline strings or following line continuation characters
+    and Mypy only recognizes inline `type: ignore` comments (see
+    [#3448](https://github.com/python/mypy/issues/3448))
 
-This utility is unable to silence mypy errors which occur on lines ending in
-line continuation characters since any non-whitespace following such a
-character is a syntax error. Pre-formatting your code with a PEP8 adherent
-formatter (e.g., [`black`](http://black.readthedocs.io)) to replace such lines with parentheses
-is recommended.
+    * Pre-formatting your code with a PEP8 adherent formatter
+    (e.g., [`black`](http://black.readthedocs.io)) to replace such lines with parentheses is
+    recommended.
 
 ## Similar Projects
 
 If this doesn't fit your use-case, maybe one of these other projects will!
 
 * [`geo7/mypy_clean_slate`](https://github.com/geo7/mypy_clean_slate/tree/main): `mypy` reports are generated internally in `--strict` mode; includes
 support for suppressing multiple errors on a single line; an inspiration for
```

