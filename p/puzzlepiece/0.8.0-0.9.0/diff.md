# Comparing `tmp/puzzlepiece-0.8.0.tar.gz` & `tmp/puzzlepiece-0.9.0.tar.gz`

## Comparing `puzzlepiece-0.8.0.tar` & `puzzlepiece-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/make.bat
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/requirements.txt
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/conf.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/index.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/modules.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/puzzlepiece.action.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/puzzlepiece.param.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/puzzlepiece.parse.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/puzzlepiece.piece.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/puzzlepiece.puzzle.rst
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/puzzlepiece.rst
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/puzzlepiece.threads.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/_static/README.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/docs/source/_templates/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/examples/basic_example.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/examples/most_basic_example.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/action.py
--rw-r--r--   0        0        0    29402 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/param.py
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/parse.py
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/piece.py
--rw-r--r--   0        0        0    21072 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/puzzle.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/readout.py
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/threads.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/pieces/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/pieces/param_setter.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/pieces/plotter.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/pieces/random_number.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/pieces/scan.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/pieces/scan_value.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/puzzlepiece/pieces/script.py
--rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/tests/test_params.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/LICENSE
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 puzzlepiece-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/index.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/modules.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/puzzlepiece.action.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/puzzlepiece.param.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/puzzlepiece.parse.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/puzzlepiece.piece.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/puzzlepiece.puzzle.rst
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/puzzlepiece.rst
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/puzzlepiece.threads.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/_static/README.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/docs/source/_templates/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/examples/basic_example.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/examples/most_basic_example.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/action.py
+-rw-r--r--   0        0        0    31299 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/param.py
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/parse.py
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/piece.py
+-rw-r--r--   0        0        0    23241 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/puzzle.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/readout.py
+-rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/threads.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/pieces/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/pieces/param_setter.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/pieces/plotter.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/pieces/random_number.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/pieces/scan.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/pieces/scan_value.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/puzzlepiece/pieces/script.py
+-rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/tests/test_params.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 puzzlepiece-0.9.0/PKG-INFO
```

### Comparing `puzzlepiece-0.8.0/.github/workflows/python-publish.yml` & `puzzlepiece-0.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/docs/Makefile` & `puzzlepiece-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/docs/make.bat` & `puzzlepiece-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/docs/source/conf.py` & `puzzlepiece-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/examples/basic_example.py` & `puzzlepiece-0.9.0/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/examples/most_basic_example.py` & `puzzlepiece-0.9.0/examples/most_basic_example.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/puzzlepiece/action.py` & `puzzlepiece-0.9.0/puzzlepiece/action.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/puzzlepiece/param.py` & `puzzlepiece-0.9.0/puzzlepiece/param.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
         if self._setter is not None:
             # Call setter if it exists. It may return a new value.
             new_value = self._setter(value)
             if new_value is None:
                 # If the setter did not return a value, see if there is a getter
                 if self._getter is not None:
                     new_value = self._getter()
+                    new_value = self._type(new_value)
                 else:
                     # Otherwise the new value is just the value we're setting
                     new_value = value
             # Update the value stored to the new value
             self._value = new_value
             # Update the input as well
             self._input_set_value(new_value)
@@ -392,15 +393,17 @@
         """:meta private:"""
         return int(self.input.isChecked())
     
     def _click_handler(self, _):
         try:
             if self._connected_click_handler is not None:
                 self._connected_click_handler()
-            self.set_value()
+            if self._setter is not None:
+                # If there's a setter, we need to explicitly call set_value here
+                self.set_value()
         except Exception as e:
             # Flip back the checkbox if the click resulted in an error
             self.input.setChecked(not(self.input.isChecked()))
             raise e
 
 
 class _PartialAccessor:
@@ -530,14 +533,53 @@
             self.input.setCurrentText(value)
 
         self.input.blockSignals(False)
 
     def _input_get_value(self):
         """:meta private:"""
         return self.input.currentText()
+    
+class ParamProgress(BaseParam):
+    """
+    A param with a progress bar. See the :func:`~puzzlepiece.param.progress` decorator below
+    for how to use this in your Piece.
+    """
+    _type = float
+
+    def _make_input(self, value=None, connect=None):
+        """:meta private:"""
+        input = QtWidgets.QProgressBar()
+        input.setMinimum(0)
+        input.setMaximum(1000)
+        if value is not None:
+            input.setValue(value)
+        return input, True
+
+    def _input_set_value(self, value):
+        """:meta private:"""
+        if value < 0:
+            self.input.setMaximum(0)
+        else:
+            self.input.setMaximum(1000)
+            self.input.setValue(int(value*1000))
+
+    def _input_get_value(self):
+        """:meta private:"""
+        return self.input.value()
+    
+    def iter(self, iterable):
+        if hasattr(iterable, '__len__'):
+            length = len(iterable)
+        else:
+            length = -1
+
+        for i, value in enumerate(iterable):
+            self.set_value(i/length)
+            yield value
+        self.set_value(1)
 
 def wrap_setter(piece, setter):
     """
     We wrap the setter function such that it can be called without passing
     a reference to the Piece as the first argument
 
     :meta private:
@@ -754,8 +796,23 @@
 
     def decorator(values):
         if callable(values):
             # `values` can be a function that returns a list of values
             values = values(piece)
         piece.params[name] = ParamDropdown(name, value, values, None, None, visible)
         return piece.params[name]
+    return decorator
+
+def progress(piece, name, visible=True):
+    """
+    A decorator generator for registering a :class:`~puzzlepiece.param.ParamProgress` in a Piece's
+    :func:`~puzzlepiece.piece.Piece.define_params` method with a given **getter**.
+
+    This will display the current progress value on a scale of 0 to 1 with no option to edit it.
+
+    See :func:`~puzzlepiece.param.base_param` for more details.
+    """
+    def decorator(getter):
+        wrapper = wrap_getter(piece, getter)
+        piece.params[name] = ParamProgress(name, None, setter=None, getter=wrapper, visible=visible)
+        return piece.params[name]
     return decorator
```

### Comparing `puzzlepiece-0.8.0/puzzlepiece/parse.py` & `puzzlepiece-0.9.0/puzzlepiece/parse.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/puzzlepiece/piece.py` & `puzzlepiece-0.9.0/puzzlepiece/piece.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import math
 
 class Piece(QtWidgets.QGroupBox):
     """
     A single `Piece` object is an unit of automation - an object that is meant to represent a single
     physical instrument (like a laser) or a particular functionality (like a plotter or a parameter scan).
 
-    Pieces can be assembled into a :class:`~puzzlepiece.puzzle.Puzzle`.
+    Pieces can be assembled into a :class:`~puzzlepiece.puzzle.Puzzle` using the Puzzle's
+    :func:`~puzzlepiece.puzzle.Puzzle.add_piece` method.
 
     :param puzzle: The parent :class:`~puzzlepiece.puzzle.Puzzle`.
-    :param custom_horizontal: A bool flat, the custom layout is displayed to the right of the main controls
-                                if True.
+    :param custom_horizontal: A bool, the custom layout is displayed to the right of the main controls
+                              if True.
     """
     def __init__(self, puzzle, custom_horizontal=False, *args, **kwargs):
         super().__init__()
         #: Reference to the parent :class:`~puzzlepiece.puzzle.Puzzle`.
         self.puzzle = puzzle
         #: Boolean flag. See :func:`~puzzlepiece.piece.Piece.call_stop`
         self.stop = False
@@ -68,15 +69,15 @@
             layout.addWidget(self.params[key], i%numrows, i//numrows)
         return layout
 
     def action_layout(self, wrap=2):
         """
         Genereates a `QGridLayout` for the actions. Override to set a different wrapping.
 
-        :param wrap: the number of columns the actions are displayed in .
+        :param wrap: the number of columns the actions are displayed in.
         :rtype: QtWidgets.QGridLayout
         """
         layout = QtWidgets.QGridLayout()
         visible_actions = [key for key in self.actions if self.actions[key].visible]
         for i, key in enumerate(visible_actions):
             button = QtWidgets.QPushButton(key)
             button.clicked.connect(lambda x=False, _key=key: self.actions[_key]())
@@ -114,28 +115,57 @@
     def setup(self):
         """
         Only called if the :class:`~puzzlepiece.puzzle.Puzzle` debug flag is False.
         Override to set up necessary hardware libraries.
         """
         pass
 
+    def open_popup(self, popup):
+        """
+        Open a popup window for this Piece. A popup is a :class:`puzzlepiece.piece.Popup`
+        object, which is like a Piece but floats in a separate window attached to the main
+        :class:`~puzzlepiece.puzzle.Puzzle`. This can be used for handling additional tasks
+        that you don't want to clutter the main Piece. See :class:`puzzlepiece.piece.Popup`
+        for details on implementing a Popup.
+
+        :param popup: a :class:`puzzlepiece.piece.Popup` _class_ to instantiate
+        :rtype: puzzlepiece.piece.Popup
+        """
+        # Instantiate the popup
+        if isinstance(popup, type):
+            popup = popup(self, self.puzzle)
+        popup.setStyleSheet("QGroupBox {border:0;}")
+
+        # Make a dialog window for the popup to live in
+        dialog = _QDialog(self, popup)
+        layout = QtWidgets.QVBoxLayout()
+        dialog.setLayout(layout)
+        layout.addWidget(popup)
+
+        # Display the dialog
+        dialog.show()
+        dialog.raise_()
+        dialog.activateWindow()
+
+        return popup
+
     def call_stop(self):
         """
         This method is called by the parent Puzzle when a global stop is called.
 
         By default, it sets the stop flag to True. Detect the flag in you code to stop processes.
 
         Alternatively, this can be overriden to support more complex actions.
         """
         self.stop = True
 
     def handle_close(self, event):
         """
-        Only called if the :class:`~puzzlepiece.puzzle.Puzzle` debug flag is False.
-        Override to disconnect hardware etc when the main window closes.
+        Only called if the :class:`~puzzlepiece.puzzle.Puzzle` :attr:`~puzzlepiece.puzzle.Puzzle.debug`
+        flag is False. Override to disconnect hardware etc when the main window closes.
         """
         pass
 
     def handle_shortcut(self, event):
         """
         Calls an Action if a keyboard shortcut has been registered.
 
@@ -214,8 +244,69 @@
                 try:
                     ensure_function(self)
                 except:
                     return False
                 return True
             else:
                 ensure_function(self)
-    return ensure_decorator
+    return ensure_decorator
+
+class _QDialog(QtWidgets.QDialog):
+    """
+    A variant of the QDialog specifically for popups, handles closing them
+    with a custom function.
+    """
+    def __init__(self, parent, popup, *args, **kwargs):
+        self.popup = popup
+        super().__init__(parent, *args, **kwargs)
+    
+    def closeEvent(self, event):
+        self.popup.handle_close()
+        super().closeEvent(event)
+
+class Popup(Piece):
+    """
+    A Popup is similar to a Piece, but floats in a separate window attached to the main
+    :class:`~puzzlepiece.puzzle.Puzzle`. This can be used for handling additional tasks
+    that you don't want to clutter the main Piece. For example you can have a camera
+    Piece which can open a Popup to set the camera's region of interest with an interactive
+    plot window.
+
+    A Popup can be created and displayed by calling :func:`puzzlepiece.piece.Piece.open_popup`.
+
+    A Popup is attached to a specific Piece and knows it through its 
+    :attr:`~puzzlepiece.piece.Popup.parent_piece` attribute, but it can also access other
+    Pieces through the Puzzle, which it knows through its :attr:`~puzzlepiece.piece.Piece.puzzle`
+    attribute.
+
+    A Popup can have params, actions, and custom layouts just like a normal Piece, and are created by
+    overriding :func:`~puzzlepiece.piece.Piece.define_params`, :func:`~puzzlepiece.piece.Piece.define_actions`,
+    and :func:`~puzzlepiece.piece.Piece.custom_layout` like for a Piece.
+
+    :param puzzle: The parent :class:`~puzzlepiece.puzzle.Puzzle`.
+    :param parent_piece: The parent :class:`~puzzlepiece.piece.Piece`.
+    :param custom_horizontal: A bool, the custom layout is displayed to the right of the main controls
+                              if True.
+    """
+    def __init__(self, parent_piece, puzzle, custom_horizontal=False, *args, **kwargs):
+        self._parent_piece = parent_piece
+        super().__init__(puzzle, custom_horizontal, *args, **kwargs)
+        self.layout.setContentsMargins(0,0,0,0)
+
+    @property
+    def parent_piece(self):
+        """
+        A reference to this Popup's parent :class:`~puzzlepiece.piece.Piece`,
+        the one that created it through :func:`puzzlepiece.piece.Piece.open_popup`.
+        """
+        return self._parent_piece
+    
+    def handle_close(self):
+        """
+        Called when the Popup is closed. Override to perform actions when the user
+        closes this Popup - for example delete related plot elements.
+
+        In contrast to :func:`puzzlepiece.piece.Piece.handle_close`, this is called even
+        if the :class:`~puzzlepiece.puzzle.Puzzle` :attr:`~puzzlepiece.puzzle.Puzzle.debug`
+        flag is True.
+        """
+        pass
```

### Comparing `puzzlepiece-0.8.0/puzzlepiece/puzzle.py` & `puzzlepiece-0.9.0/puzzlepiece/puzzle.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,47 @@
         self.setLayout(self.wrapper_layout)
 
         self.layout = QtWidgets.QGridLayout()
         self.wrapper_layout.addLayout(self.layout, 0, 0)
 
         self.wrapper_layout.addLayout(self._button_layout(), 1, 0)
 
-        sys.excepthook = self._excepthook
+        try:
+            # If this doesn't raise a NameError, we're in IPython
+            shell = get_ipython()
+            # _orig_sys_module_state stores the original IPKernelApp excepthook,
+            # irrespective of possible modifications in other cells
+            self._old_excepthook = shell._orig_sys_module_state['excepthook']
+
+            # The following hack allows us to handle exceptions through the Puzzle in IPython.
+            # Normally when a cell is executed in an IPython InteractiveShell,
+            # sys.excepthook is overwritten with shell.excepthook, and then restored
+            # to sys.excepthook after the cell run finishes. Any changes we make to
+            # sys.excepthook in here directly will thus be overwritten as soon as the
+            # cell that defines the Puzzle finishes running.
+                
+            # Instead, we schedule set_excepthook on a QTimer, meaning that it will
+            # execute in the Qt loop rather than in a cell, so it can modify
+            # sys.excepthook without risk of the changes being immediately overwritten,
+                
+            # For bonus points, we could set _old_excepthook to shell.excepthook,
+            # which would result in all tracebacks appearing in the Notebook rather
+            # than the console, but I think that is not desireable.
+            def set_excepthook():
+                sys.excepthook = self._excepthook
+            QtCore.QTimer.singleShot(0, set_excepthook)
+        except NameError:
+            # In normal Python (not IPython) this is comparatively easy.
+            # We use the original system hook here instead of sys.excepthook
+            # to avoid unexpected behaviour if multiple things try to override
+            # the hook in various ways.
+            # If you need to implement custom exception handling, please assign
+            # a value to your Puzzle's ``custom_excepthook`` method.
+            self._old_excepthook = sys.__excepthook__
+            sys.excepthook = self._excepthook
 
     @property
     def pieces(self):
         """
         A :class:`~puzzlepiece.puzzle.PieceDict`, effectively a dictionary of
         :class:`~puzzlepiece.piece.Piece` objects. Can be used to access Pieces from within other Pieces.
         """
@@ -126,15 +158,18 @@
         if hasattr(worker, 'stop'):
             # This signal is emitted when the application is shutting down,
             # so we're telling the LiveWorker to stop
             self._shutdown_threads.connect(worker.stop)
         self._threadpool.start(worker)
 
     def _excepthook(self, exctype, value, traceback):
-        sys.__excepthook__(exctype, value, traceback)
+        self._old_excepthook(exctype, value, traceback)
+
+        # Stop any threads that may be running
+        self._shutdown_threads.emit()
 
         # Only do custom exception handling in the main thread, otherwise the messagebox
         # or other such things are likely to break things.
         if QtCore.QThread.currentThread() == self.app.thread():
             self.custom_excepthook(exctype, value, traceback)
 
             box = QtWidgets.QMessageBox()
@@ -334,14 +369,17 @@
         :meta private:
         """
         self._shutdown_threads.emit()
         
         if not self.debug:
             for piece_name in self.pieces:
                 self.pieces[piece_name].handle_close(event)
+
+        # Reinstate the original excepthook
+        sys.excepthook = self._old_excepthook
         super().closeEvent(event)
 
 
 QApp = QtWidgets.QApplication
 """A QApplication has to be constructed before any Qt objects
 (including the Puzzle and the Pieces), so this is a convenient shortcut to
 the QApplication class (see https://doc.qt.io/qt-6/qapplication.html).
```

### Comparing `puzzlepiece-0.8.0/puzzlepiece/threads.py` & `puzzlepiece-0.9.0/puzzlepiece/threads.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/puzzlepiece/pieces/param_setter.py` & `puzzlepiece-0.9.0/puzzlepiece/pieces/param_setter.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/puzzlepiece/pieces/plotter.py` & `puzzlepiece-0.9.0/puzzlepiece/pieces/plotter.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/puzzlepiece/pieces/random_number.py` & `puzzlepiece-0.9.0/puzzlepiece/pieces/random_number.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/puzzlepiece/pieces/scan.py` & `puzzlepiece-0.9.0/puzzlepiece/pieces/scan.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/puzzlepiece/pieces/scan_value.py` & `puzzlepiece-0.9.0/puzzlepiece/pieces/scan_value.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/puzzlepiece/pieces/script.py` & `puzzlepiece-0.9.0/puzzlepiece/pieces/script.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/tests/test_params.py` & `puzzlepiece-0.9.0/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/.gitignore` & `puzzlepiece-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/LICENSE` & `puzzlepiece-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/README.md` & `puzzlepiece-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `puzzlepiece-0.8.0/pyproject.toml` & `puzzlepiece-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "puzzlepiece"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
   { name="Jakub Dranczewski", email="jakub.dranczewski@gmail.com" },
 ]
 description = "A GUI-forward Python framework for automating experimental setups."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `puzzlepiece-0.8.0/PKG-INFO` & `puzzlepiece-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puzzlepiece
-Version: 0.8.0
+Version: 0.9.0
 Summary: A GUI-forward Python framework for automating experimental setups.
 Project-URL: Homepage, https://github.com/jdranczewski/puzzlepiece
 Project-URL: Documentation, https://puzzlepiece.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/jdranczewski/puzzlepiece/issues
 Author-email: Jakub Dranczewski <jakub.dranczewski@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

