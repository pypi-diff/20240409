# Comparing `tmp/commits2pdf-1.1.5.tar.gz` & `tmp/commits2pdf-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commits2pdf-1.1.5.tar", last modified: Sun Apr  7 11:37:24 2024, max compression
+gzip compressed data, was "commits2pdf-1.1.6.tar", last modified: Tue Apr  9 05:56:03 2024, max compression
```

## Comparing `commits2pdf-1.1.5.tar` & `commits2pdf-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 11:37:24.366410 commits2pdf-1.1.5/
--rw-rw-rw-   0        0        0     1086 2024-03-28 09:30:12.000000 commits2pdf-1.1.5/LICENCE.md
--rw-rw-rw-   0        0        0     7912 2024-04-07 11:37:24.365414 commits2pdf-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     7026 2024-04-07 11:27:11.000000 commits2pdf-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 11:37:24.346462 commits2pdf-1.1.5/commits2pdf/
--rw-rw-rw-   0        0        0       21 2024-03-29 18:15:07.000000 commits2pdf-1.1.5/commits2pdf/__init__.py
--rw-rw-rw-   0        0        0    10679 2024-04-07 10:52:13.000000 commits2pdf-1.1.5/commits2pdf/cli.py
--rw-rw-rw-   0        0        0    12788 2024-04-07 09:56:11.000000 commits2pdf-1.1.5/commits2pdf/commits.py
--rw-rw-rw-   0        0        0     3037 2024-04-07 10:09:48.000000 commits2pdf-1.1.5/commits2pdf/constants.py
--rw-rw-rw-   0        0        0      308 2024-04-07 03:56:00.000000 commits2pdf-1.1.5/commits2pdf/logger.py
--rw-rw-rw-   0        0        0     7100 2024-04-07 10:55:21.000000 commits2pdf-1.1.5/commits2pdf/render_cairo.py
--rw-rw-rw-   0        0        0     9646 2024-04-07 11:29:41.000000 commits2pdf-1.1.5/commits2pdf/render_fpdf.py
-drwxrwxrwx   0        0        0        0 2024-04-07 11:37:24.364415 commits2pdf-1.1.5/commits2pdf.egg-info/
--rw-rw-rw-   0        0        0     7912 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 11:37:24.366410 commits2pdf-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1223 2024-04-07 11:37:20.000000 commits2pdf-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:56:03.018548 commits2pdf-1.1.6/
+-rw-rw-rw-   0        0        0     1086 2024-03-28 09:30:12.000000 commits2pdf-1.1.6/LICENCE.md
+-rw-rw-rw-   0        0        0     7987 2024-04-09 05:56:03.017551 commits2pdf-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7101 2024-04-09 05:31:15.000000 commits2pdf-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 05:56:03.008576 commits2pdf-1.1.6/commits2pdf/
+-rw-rw-rw-   0        0        0       21 2024-03-29 18:15:07.000000 commits2pdf-1.1.6/commits2pdf/__init__.py
+-rw-rw-rw-   0        0        0    10749 2024-04-09 05:21:34.000000 commits2pdf-1.1.6/commits2pdf/cli.py
+-rw-rw-rw-   0        0        0    13084 2024-04-09 05:04:37.000000 commits2pdf-1.1.6/commits2pdf/commits.py
+-rw-rw-rw-   0        0        0     3244 2024-04-09 05:38:04.000000 commits2pdf-1.1.6/commits2pdf/constants.py
+-rw-rw-rw-   0        0        0      308 2024-04-07 03:56:00.000000 commits2pdf-1.1.6/commits2pdf/logger.py
+-rw-rw-rw-   0        0        0     7100 2024-04-07 10:55:21.000000 commits2pdf-1.1.6/commits2pdf/render_cairo.py
+-rw-rw-rw-   0        0        0    10136 2024-04-09 05:52:47.000000 commits2pdf-1.1.6/commits2pdf/render_fpdf.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:56:03.016554 commits2pdf-1.1.6/commits2pdf.egg-info/
+-rw-rw-rw-   0        0        0     7987 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 05:56:02.000000 commits2pdf-1.1.6/commits2pdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 05:56:03.019545 commits2pdf-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1223 2024-04-09 05:55:47.000000 commits2pdf-1.1.6/setup.py
```

### Comparing `commits2pdf-1.1.5/LICENCE.md` & `commits2pdf-1.1.6/LICENCE.md`

 * *Files identical despite different names*

### Comparing `commits2pdf-1.1.5/PKG-INFO` & `commits2pdf-1.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commits2pdf
-Version: 1.1.5
+Version: 1.1.6
 Summary: View a filtered commit history in PDF form.
 Home-page: https://github.com/tomasvana10/commits2pdf
 Author: Tomas Vana
 License: MIT
 Platform: any
 Classifier: Topic :: Multimedia
 Classifier: Development Status :: 5 - Production/Stable
@@ -147,25 +147,25 @@
 ### fpdf (gen2a)
 - **Positives**
   - Fast
   - Scalable
   - Detailed title page
   - Sleek design
   - Hyperlinks
-  - Creates metadata
+  - Saves metadata
 - **Negatives**
-  - Inconsistent page breaks (limitation with fpdf)
-- **Sample use case**: You do not mind if your PDF has large gaps of space, but you want a nice design that can be generated very fast.
+  - Inconsistent page breaks in some cases due to the difficulty of precalculating the height of a commit, a general limitation with this generation method.
+- **Sample use case**: You do not mind if your PDF has occasionally inconsistent spacing, but you want a nice design that can be generated very fast.
 
 ### fpdf (gen2b - Default)
 - **Positives**
-   - **Same as gen2a but with consistent page breaks that do not leave any whitespace**
+   - Same as gen2a but with consistent page breaks that do not leave any whitespace.
 - **Negatives**
-  - Slow (time complexity ranges between `O(n)` to `O(n log n)`)
-- **Sample use case**: You either want to visualise a relatively small amount of commits in a PDF that is sleek and consistently-designed
+  - Slow when generating large 
+- **Sample use case**: You want to visualise a relatively small amount of commits in a PDF that is sleek and consistently-designed.
 <br><br>
 ## Gallery
 **gen1 title page**<br>
 <img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/b243e102-0eda-4750-bbce-027f5738405b" alt="gen1 pdf title page" width=561.12>
 
 **gen2 title page in dark mode**<br>
 <img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/e1f2fe53-1c72-42a6-a89b-44a27c0b06a9" alt="gen2 pdf title page dark" width=561.12>
```

### Comparing `commits2pdf-1.1.5/README.md` & `commits2pdf-1.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -121,25 +121,25 @@
 ### fpdf (gen2a)
 - **Positives**
   - Fast
   - Scalable
   - Detailed title page
   - Sleek design
   - Hyperlinks
-  - Creates metadata
+  - Saves metadata
 - **Negatives**
-  - Inconsistent page breaks (limitation with fpdf)
-- **Sample use case**: You do not mind if your PDF has large gaps of space, but you want a nice design that can be generated very fast.
+  - Inconsistent page breaks in some cases due to the difficulty of precalculating the height of a commit, a general limitation with this generation method.
+- **Sample use case**: You do not mind if your PDF has occasionally inconsistent spacing, but you want a nice design that can be generated very fast.
 
 ### fpdf (gen2b - Default)
 - **Positives**
-   - **Same as gen2a but with consistent page breaks that do not leave any whitespace**
+   - Same as gen2a but with consistent page breaks that do not leave any whitespace.
 - **Negatives**
-  - Slow (time complexity ranges between `O(n)` to `O(n log n)`)
-- **Sample use case**: You either want to visualise a relatively small amount of commits in a PDF that is sleek and consistently-designed
+  - Slow when generating large 
+- **Sample use case**: You want to visualise a relatively small amount of commits in a PDF that is sleek and consistently-designed.
 <br><br>
 ## Gallery
 **gen1 title page**<br>
 <img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/b243e102-0eda-4750-bbce-027f5738405b" alt="gen1 pdf title page" width=561.12>
 
 **gen2 title page in dark mode**<br>
 <img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/e1f2fe53-1c72-42a6-a89b-44a27c0b06a9" alt="gen2 pdf title page dark" width=561.12>
```

### Comparing `commits2pdf-1.1.5/commits2pdf/cli.py` & `commits2pdf-1.1.6/commits2pdf/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,17 @@
     else:
         from .render_fpdf import FPDF_PDF
         cls = FPDF_PDF
         gen_args.append(mode)
         gen_args.append(scaling)
     
     pdf = cls(*gen_args)
+    try:
+        if pdf.recursion_err_flag: return
+    except: ...
     p = path.abspath(args.output)
     logger.info(f"{commits.rname}-commits_report.pdf successfully generated in {p}")
 
     if not args.prevent_open: _open_pdf(args, p)
     
 def _open_pdf(args, p) -> None:
     """Open the PDF in the user's file system, unless the user has prevent open
```

### Comparing `commits2pdf-1.1.5/commits2pdf/commits.py` & `commits2pdf-1.1.6/commits2pdf/commits.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,17 +234,20 @@
 
         self["info"] = f"{self['hexsha_short']} | Branch: {self['branch']} | " \
                        f"By {self['author_name']} ({self['author_email']}) | " \
                        f"At {self['date'].strftime('%Y-%m-%d')}"
          
         # Extract the message from the title
         msg = commit.message.split("\n")
-        self["title"] = msg[0]
+        self["title"] = msg[0].encode("latin-1", errors="replace")\
+                                                            .decode("latin-1")
         if len(msg) > 1:
-            self["description"] = "\n".join(msg[1:])
+            self["description"] = "\n".join(msg[1:]).encode("latin-1", 
+                                                            errors="replace")\
+                                                            .decode("latin-1")
         else:
             self["description"] = ""
     
     def __str__(self): 
         """View the commit in the terminal."""
         return \
             "=============================\n" \
```

### Comparing `commits2pdf-1.1.5/commits2pdf/constants.py` & `commits2pdf-1.1.6/commits2pdf/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 INVALID_ARG_WARNING = "Invalid {} format. Run commits2pdf -h for more information."
 CANNOT_USE_SCALE_WARNING = "You cannot set scaling when using the gen1 PDF " \
                              "generator."
 
 
 """Handling the processing of the repository"""
 REPO_ALREADY_EXISTS_WARNING = "The repository you are cloning from already "\
-                              "exists, the repo will be accessed normally."
+                              "exists, so it will be accessed normally."
 DETACHED_BRANCH_ERROR = "The repository you are cloning from already exists, "\
                         "but the branch you specified ({}) is detached."
 BRANCH_ALREADY_EXISTS_WARNING = "The branch you specified ({}) does not exist. " \
                                 "Selecting the active branch ({}) instead."
 INVALID_REPO_ERROR = "The repository {} does not exist or is invalid. " \
                      "Attempting to delete tree..."
 INVALID_REPO_ERROR_2 = "Invalid git repository. Exiting..."
@@ -47,19 +47,22 @@
 """For the pycairo PDF implementation"""
 WIDTH = 612
 HEIGHT = 792
 MARGIN = 50
 
 
 """For the fpdf PDF implementation"""
+RECURSION_ERROR = "An error occured when using the gen2b renderer. Please try " \
+                  "adding the -gen2a flag to your console command and try again."
 TITLE_FONT = ["Arial", "B", 36]
 SUBTITLE_FONT = ["Arial", "", 30]
 MARGIN_FONT = ["Arial", "I", 8]
 SMALL_TEXT_FONT = ["Arial", "", 12]
 MEDIUM_TEXT_FONT = ["Arial", "", 16]
+TITLE_PAGE_INFO_FONT = ["Courier", "", 15]
 MEDIUM_TEXT_FONT_BOLD = ["Arial", "B", 16]
 INFO_TEXT_FONT = ["Courier", "", 12]
 MARGIN_LR = 25.4
 MARGIN_TB = 25.4
 
 
 """Appearances"""
```

### Comparing `commits2pdf-1.1.5/commits2pdf/render_cairo.py` & `commits2pdf-1.1.6/commits2pdf/render_cairo.py`

 * *Files identical despite different names*

### Comparing `commits2pdf-1.1.5/commits2pdf/render_fpdf.py` & `commits2pdf-1.1.6/commits2pdf/render_fpdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from time import time
 from datetime import datetime
 from os import path
 from pickle import loads, dumps
 from typing import List, Dict, Union
+from pickle import loads, dumps
 
 from fpdf import FPDF
 
 from .constants import (
     TITLE_FONT, SUBTITLE_FONT, MARGIN_FONT, SMALL_TEXT_FONT, MEDIUM_TEXT_FONT,
-    MEDIUM_TEXT_FONT_BOLD, INFO_TEXT_FONT, MARGIN_LR, MARGIN_TB
+    MEDIUM_TEXT_FONT_BOLD, INFO_TEXT_FONT, MARGIN_LR, MARGIN_TB, RECURSION_ERROR,
+    TITLE_PAGE_INFO_FONT
 )
+from .logger import logger
 
 
 class FPDF_PDF(FPDF):
     def __init__(self, 
                  commits: object, 
                  output: str, 
                  filename: str, 
@@ -22,35 +25,37 @@
                  scaling: str
                  ) -> None:
         """Assign attributes for use across the instance and configure the 
         settings of the ``FPDF`` class.
         """
         super().__init__() # portrait; millimetres; a4
         FPDF_PDF._set_scaling(scaling)
+        self.recursion_err_flag = False
         self.timestamp = datetime.fromtimestamp(
             int(time())).strftime('%Y-%m-%d %H:%M:%S')
         self._commits, self._output, self._filename, self._ap, self._mode = \
             commits, output, filename, appearance, mode
-        if self._mode == "unstable":
-            self.do_pre_vis = True 
-            self.set_auto_page_break(auto=False)
-        else:
-            self.do_pre_vis = False
-            self.set_auto_page_break(auto=True)
-
+    
         self.set_fill_color(*self._ap["background"])
         self.set_creator("commits2pdf")
         self.set_title(f"Commits Report - {self._commits.rname}")
         self.set_author(f"{self._commits.owner}")
         self.set_subject("Git Commit Report")
         self.set_keywords("git;repo;repository;report;documentation;cli;python")
         self.set_margins(MARGIN_LR, MARGIN_TB)
+        
         self.add_page()
         self._draw_page_bg()
         self._draw_title_page()
+        self.set_auto_page_break(auto=True)
+        if self._mode == "unstable":
+            self.do_pre_vis = True 
+            self.set_auto_page_break(auto=False)
+        else:
+            self.do_pre_vis = False
         
         if len(self._commits.filtered_commits) > 0: self._draw_commits()
         self._write()
     
     @staticmethod
     def _set_scaling(scaling: float) -> None:
         """Scale the fonts based on the user-selected scaling. Set to 1.0 by
@@ -115,41 +120,50 @@
                      commit: Dict[str, str], 
                      pre_vis: bool = False, 
                      no_divider: bool = False
                      ) -> Union[str, None]:
         """Draw all the parts of a commit to the current ``FPDF`` instance
         or a copy of it as part of the ``gen2b`` generation implementation.
         """
-        p = self if not pre_vis or not self.do_pre_vis else loads(dumps(self))
+        if not pre_vis or not self.do_pre_vis:
+            p = self
+        else:
+            try:
+                p = loads(dumps(self))
+            except RecursionError: # Why this happen bruh?!
+                logger.error(RECURSION_ERROR)
+                self.recursion_err_flag = True
+                exit(1)
+            
         
         y: int = p.get_y()
         p.set_text_color(*self._ap["text"])
         p._set_font(*INFO_TEXT_FONT)
         p.multi_cell(w=0, h=p.font_size * 1.25, align="C", txt=commit["info"])
         p.ln(p.font_size * 0.75)
         # Tells the driver code that it must add a page
         if self.do_pre_vis and pre_vis and p.get_y() > p.h * 0.95: return "new"
         
         p._set_font(*MEDIUM_TEXT_FONT_BOLD)
         p.multi_cell(w=0, h=p.font_size * 1.25, align="L", txt=commit["title"])
         p.ln(-1 * p.font_size * 0.5)
         if self.do_pre_vis and pre_vis and p.get_y() > p.h * 0.95: return "new"
-
+            
         p._set_font(*SMALL_TEXT_FONT)
         p.multi_cell(w=0, h=p.font_size * 1.5, align="L", 
                      txt=commit["description"])
         p.ln()
-        if self.do_pre_vis and pre_vis and p.get_y() > p.h * 0.95: return "new" 
-
+        if self.do_pre_vis and pre_vis and p.get_y() > p.h * 0.95: return "new"
+            
         p.set_text_color(*self._ap["diff_url"])
         p._set_font(*SMALL_TEXT_FONT)
         p.write(p.font_size * 1.5, "View diff on GitHub", commit["diff_url"])
         p.ln(p.font_size * 4.75) 
-        if self.do_pre_vis and pre_vis and p.get_y() > p.h * 0.95: return "new" 
-
+        if self.do_pre_vis and pre_vis and p.get_y() > p.h * 0.95: return "new"
+            
         if pre_vis or not no_divider or not self.do_pre_vis:
             div_y = p.get_y() - p.font_size * 3.25 / 2
             self.set_draw_color(*self._ap["text"])
             p.line(p.l_margin, div_y, p.w - p.r_margin, div_y)
             self.set_draw_color(*self._ap["background"])
             if self.do_pre_vis and pre_vis and p.get_y() > p.h * 0.97: \
                 return "no_divider" 
@@ -171,36 +185,36 @@
                       // self.w
 
         height = (info_lines * INFO_TEXT_FONT[2]) \
                          + (title_lines * MEDIUM_TEXT_FONT_BOLD[2]) \
                          + (desc_lines * SMALL_TEXT_FONT[2]) \
                          + (diff_lines * SMALL_TEXT_FONT[2])
 
-        return height > self.h - self.get_y()
+        return height * 1.2 > self.h - self.get_y()
 
     def _draw_title_page(self) -> None:
         """Draw the title, repository name, and filtering information on the
         first page of the PDF.
         """
         self._set_font(*TITLE_FONT)
         self.set_text_color(*self._ap["text"])
         self.cell(w=0, h=self.font_size * 1.5, txt="Commits Report", align="C")
         self.ln()
         
         self._set_font(*SUBTITLE_FONT)
-        self.cell(w=0, h=self.font_size * 3, 
+        self.multi_cell(w=0, h=self.font_size * 1.25, 
                   txt=f"Repository: {self._commits.rname}", align="C")
-        self.ln()
+        self.ln(self.font_size)
 
-        self._set_font(*MEDIUM_TEXT_FONT)
+        self._set_font(*TITLE_PAGE_INFO_FONT)
         self.multi_cell(0, self.font_size * 1.5, 
             txt=f"Owner: {self._commits.owner}", align="C")
         self.ln()
         self.multi_cell(0, self.font_size * 1.5, align="C",
-            txt=f"Authors: "
+            txt=f"Selected authors: "
                 f"{', '.join(self._commits.authors.split(',')) if self._commits.authors else 'All'}")
         self.ln()
         self.multi_cell(0, self.font_size * 1.5, align="C",
             txt=f"Start date: "
                 f"{self._commits.start_date.strftime('%Y-%m-%d') if self._commits.start_date else 'N/A'} "
                 f"| End date: {self._commits.end_date.strftime('%Y-%m-%d') if self._commits.end_date else 'N/A'}")
         self.ln()
```

### Comparing `commits2pdf-1.1.5/commits2pdf.egg-info/PKG-INFO` & `commits2pdf-1.1.6/commits2pdf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commits2pdf
-Version: 1.1.5
+Version: 1.1.6
 Summary: View a filtered commit history in PDF form.
 Home-page: https://github.com/tomasvana10/commits2pdf
 Author: Tomas Vana
 License: MIT
 Platform: any
 Classifier: Topic :: Multimedia
 Classifier: Development Status :: 5 - Production/Stable
@@ -147,25 +147,25 @@
 ### fpdf (gen2a)
 - **Positives**
   - Fast
   - Scalable
   - Detailed title page
   - Sleek design
   - Hyperlinks
-  - Creates metadata
+  - Saves metadata
 - **Negatives**
-  - Inconsistent page breaks (limitation with fpdf)
-- **Sample use case**: You do not mind if your PDF has large gaps of space, but you want a nice design that can be generated very fast.
+  - Inconsistent page breaks in some cases due to the difficulty of precalculating the height of a commit, a general limitation with this generation method.
+- **Sample use case**: You do not mind if your PDF has occasionally inconsistent spacing, but you want a nice design that can be generated very fast.
 
 ### fpdf (gen2b - Default)
 - **Positives**
-   - **Same as gen2a but with consistent page breaks that do not leave any whitespace**
+   - Same as gen2a but with consistent page breaks that do not leave any whitespace.
 - **Negatives**
-  - Slow (time complexity ranges between `O(n)` to `O(n log n)`)
-- **Sample use case**: You either want to visualise a relatively small amount of commits in a PDF that is sleek and consistently-designed
+  - Slow when generating large 
+- **Sample use case**: You want to visualise a relatively small amount of commits in a PDF that is sleek and consistently-designed.
 <br><br>
 ## Gallery
 **gen1 title page**<br>
 <img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/b243e102-0eda-4750-bbce-027f5738405b" alt="gen1 pdf title page" width=561.12>
 
 **gen2 title page in dark mode**<br>
 <img src="https://github.com/tomasvana10/commits2pdf/assets/124552709/e1f2fe53-1c72-42a6-a89b-44a27c0b06a9" alt="gen2 pdf title page dark" width=561.12>
```

### Comparing `commits2pdf-1.1.5/setup.py` & `commits2pdf-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="commits2pdf",
-    version="1.1.5",
+    version="1.1.6",
     author="Tomas Vana",
     url="https://github.com/tomasvana10/commits2pdf",
     description="View a filtered commit history in PDF form.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     license="MIT",
```

