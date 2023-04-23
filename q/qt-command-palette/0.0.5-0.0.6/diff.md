# Comparing `tmp/qt_command_palette-0.0.5.tar.gz` & `tmp/qt_command_palette-0.0.6.tar.gz`

## Comparing `qt_command_palette-0.0.5.tar` & `qt_command_palette-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/codecov.yml
--rw-r--r--   0        0        0   201915 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/example.gif
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/launch.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/setup.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/qt_command_palette/__about__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/qt_command_palette/__init__.py
--rw-r--r--   0        0        0     8917 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/qt_command_palette/_api.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/qt_command_palette/_commands.py
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/qt_command_palette/_list.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/qt_command_palette/_storage.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/qt_command_palette/_widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/tests/_file_0.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/tests/_file_1.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/tests/test_register.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/tests/test_storage.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/.gitignore
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/README.md
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 qt_command_palette-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/codecov.yml
+-rw-r--r--   0        0        0   201915 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/example.gif
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/launch.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/setup.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/__about__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/__init__.py
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_api.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_commands.py
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_list.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_storage.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/_file_0.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/_file_1.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/test_register.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/test_storage.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/README.md
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/PKG-INFO
```

### Comparing `qt_command_palette-0.0.5/.pre-commit-config.yaml` & `qt_command_palette-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.5/example.gif` & `qt_command_palette-0.0.6/example.gif`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.5/launch.py` & `qt_command_palette-0.0.6/launch.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     main = QtW.QWidget()
     main.setMinimumSize(400, 300)
 
     main.setLayout(QtW.QVBoxLayout())
     _checkbox = QtW.QCheckBox("Check")
     main.layout().addWidget(_checkbox)
 
-    palette = get_palette(name=__name__)
+    palette = get_palette(name=__name__, alignment="screen")
     storage = get_storage(name=__name__)
 
     @storage.mark_getter("widget")
     def get_widget():
         return main
 
     group_0 = palette.add_group("Example")
```

### Comparing `qt_command_palette-0.0.5/qt_command_palette/_api.py` & `qt_command_palette-0.0.6/qt_command_palette/_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from __future__ import annotations
+
+from enum import Enum
 from functools import wraps
 from typing import Any, Callable, TypeVar, overload, TYPE_CHECKING
 import weakref
 import inspect
 from ._commands import Command
 from ._storage import Storage
 
@@ -36,22 +38,37 @@
     desc: str | None = None,
     tooltip: str | None = None,
     when: Callable[[], bool] = _always_true,
 ):
     """Template function to provide signature to register() without 'func' argument."""
 
 
+class Alignment(Enum):
+    """Alignment flag of the palette."""
+
+    parent = "parent"  # align to the parent widget
+    screen = "screen"  # align to the screen
+
+
 class CommandPalette:
     """The command palette interface."""
 
-    def __init__(self, name: str) -> None:
+    def __init__(
+        self, name: str, *, alignment: str | Alignment = Alignment.parent
+    ) -> None:
         self._commands: list[Command] = []
         self._parent_to_palette_map: dict[int, QCommandPalette] = {}
         self._palette_to_parent_map: WVDict = weakref.WeakValueDictionary()
         self._name = name
+        self._alignment = Alignment(alignment)
+
+    @property
+    def alignment(self) -> Alignment:
+        """Alignment flag of the palette."""
+        return self._alignment
 
     @property
     def commands(self) -> list[Command]:
         """List of all the commands."""
         return self._commands.copy()
 
     @overload
@@ -83,18 +100,18 @@
             bound = register_without_func.bind(*args, **kwargs)
 
         bound.apply_defaults()
         bound_args = bound.arguments
         func = bound_args.pop("func", None)
 
         # update defaults
-        title = bound_args["title"]
-        desc = bound_args["desc"]
-        tooltip = bound_args["tooltip"]
-        when = bound_args["when"]
+        title: str | None = bound_args["title"]
+        desc: str | None = bound_args["desc"]
+        tooltip: str | None = bound_args["tooltip"]
+        when: Callable[..., bool] = bound_args["when"]
 
         if title is None:
             title = ""
 
         def wrapper(func: _F) -> _F:
             nonlocal title, desc, tooltip
             if desc is None:
@@ -131,15 +148,18 @@
             widget.extend_command(self._commands)
             self._parent_to_palette_map[_id] = widget
             self._palette_to_parent_map[id(widget)] = parent
         return widget
 
     def show_widget(self, parent: Any = __default) -> None:
         """Show command palette widget."""
-        self.get_widget(parent).show()
+        if self.alignment is Alignment.parent:
+            self.get_widget(parent).show()
+        else:
+            self.get_widget(parent).show_center()
         return None
 
     def install(self, parent: QtW.QWidget, keys: str | None = None) -> None:
         """
         Install command palette on a Qt widget.
 
         Parameters
@@ -163,14 +183,26 @@
             return None
         _id = id(parent)
         widget = self._parent_to_palette_map[_id]
         widget.clear_commands()
         widget.extend_command(self._commands)
         return None
 
+    def sort(
+        self, rule: Callable[[Command], Any] | None = None, reverse: bool = False
+    ) -> None:
+        """Sort the command palette."""
+        if rule is None:
+
+            def rule(cmd: Command):
+                return cmd.title + cmd.desc
+
+        self._commands.sort(key=rule, reverse=reverse)
+        return None
+
 
 class CommandGroup:
     def __init__(self, title: str, parent: CommandPalette) -> None:
         self._palette_ref = weakref.ref(parent)
         self._title = title
 
     def __repr__(self) -> str:
@@ -235,15 +267,19 @@
     return None
 
 
 _GLOBAL_PALETTES: dict[str, CommandPalette] = {}
 _DEFAULT_PALETTE = CommandPalette(name="default")
 
 
-def get_palette(name: str | None = None) -> CommandPalette:
+def get_palette(
+    name: str | None = None,
+    *,
+    alignment: str | Alignment = Alignment.parent,
+) -> CommandPalette:
     """
     Get the global command palette object.
 
     Examples
     --------
     >>> palette = get_palette()  # get the default palette
     >>> palette = get_palette("my_module")  # get a palette for specific app
@@ -251,15 +287,19 @@
     global _GLOBAL_PALETTES
 
     if name is None:
         return _DEFAULT_PALETTE
     if not isinstance(name, str):
         raise TypeError(f"Expected str, got {type(name).__name__}")
     if (palette := _GLOBAL_PALETTES.get(name, None)) is None:
-        palette = _GLOBAL_PALETTES[name] = CommandPalette(name=name)
+        palette = _GLOBAL_PALETTES[name] = CommandPalette(
+            name=name, alignment=alignment
+        )
+    else:
+        palette._alignment = alignment
     return palette
 
 
 def add_group(title: str) -> CommandGroup:
     """
     Add a command group to the global command palette.
```

### Comparing `qt_command_palette-0.0.5/qt_command_palette/_commands.py` & `qt_command_palette-0.0.6/qt_command_palette/_commands.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.5/qt_command_palette/_list.py` & `qt_command_palette-0.0.6/qt_command_palette/_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import Any, TYPE_CHECKING, Iterator
 import logging
 import re
 
-from qtpy import QtWidgets as QtW, QtCore
-from qtpy.QtCore import Qt, Signal
+from qtpy import QtWidgets as QtW, QtCore, QtGui
+from qtpy.QtCore import Qt, Signal, Property
 
 from ._commands import Command
 
 logger = logging.getLogger(__name__)
 MATCH_COLOR = "blue"
 DISABLED_COLOR = "gray"
 
@@ -23,15 +23,15 @@
 
 class QCommandMatchModel(QtCore.QAbstractListModel):
     """A list model for the command palette."""
 
     def __init__(self, parent: QtW.QWidget = None):
         super().__init__(parent)
         self._commands: list[Command] = []
-        self._max_matches = 24
+        self._max_matches = 80
 
     def rowCount(self, parent: QtCore.QModelIndex = None) -> int:
         return self._max_matches
 
     def data(self, index: QtCore.QModelIndex, role: int = ...) -> Any:
         return QtCore.QVariant()
 
@@ -106,20 +106,22 @@
         self._current_max_index = 0
         for i in range(self.model()._max_matches):
             lw = QCommandLabel()
             self._label_widgets.append(lw)
             self.setIndexWidget(self.model().index(i), lw)
         self.pressed.connect(self._on_clicked)
 
-        self._match_color = "#468cc6"
+        self._match_color = QtGui.QColor("#468cc6")
 
-    def match_color(self) -> str:
+    @Property(QtGui.QColor)
+    def matchColor(self) -> QtGui.QColor:
         return self._match_color
 
-    def set_match_color(self, color: str):
+    @matchColor.setter
+    def matchColor(self, color: QtGui.QColor):
         self._match_color = color
 
     def _on_clicked(self, index: QtCore.QModelIndex) -> None:
         if index.isValid():
             self.commandClicked.emit(index.row())
             return None
 
@@ -191,15 +193,15 @@
         row = 0
         for cmd in self.all_commands:
             if cmd.matches(input_text):
                 self.setRowHidden(row, False)
                 lw = self.indexWidget(self.model().index(row))
                 lw.set_command(cmd)
                 if cmd.enabled():
-                    lw.set_text_colors(input_text, color=self._match_color)
+                    lw.set_text_colors(input_text, color=self.matchColor.name())
                 else:
                     lw.set_disabled()
                 row += 1
 
                 if row >= max_matches:
                     self._current_max_index = max_matches
                     break
```

### Comparing `qt_command_palette-0.0.5/qt_command_palette/_storage.py` & `qt_command_palette-0.0.6/qt_command_palette/_storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 from __future__ import annotations
-from typing import Any, Callable, TypeVar
+from typing import Any, Callable, TypeVar, overload
 import inspect
 
 _R = TypeVar("_R")
 
 
 class Storage:
     """The variable storage."""
 
     _INSTANCES: dict[str, Storage] = {}
 
     def __init__(self):
-        self._varmap: dict[str, Callable[[], Any]] = {}
+        self._varmap: dict[str, Callable[..., Any]] = {}
+
+    @overload
+    def mark_getter(self, func: Callable[..., Any]) -> Callable[..., Any]:
+        ...
+
+    @overload
+    def mark_getter(
+        self, name: str
+    ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
+        ...
+
+    def mark_getter(self, name, func=None):
+        if callable(name) and func is None:
+            func = name
+            name = func.__name__
+        elif isinstance(name, str):
+            pass
+        else:
+            raise TypeError(f"Invalid type for name: {type(name)}")
 
-    def mark_getter(self, name: str, func: Callable[[], Any] | None = None):
         def wrapper(f: Callable[[], Any]):
             self._varmap[name] = f
             return f
 
         return wrapper if func is None else wrapper(func)
 
     def mark_constant(self, name: str, value: Any):
@@ -28,19 +46,20 @@
         if name not in cls._INSTANCES:
             cls._INSTANCES[name] = Storage()
         return cls._INSTANCES[name]
 
     def call(self, func: Callable[..., _R], parent=None) -> _R:
         """Call a function with variables from the storage."""
         args = []
-        for v in inspect.signature(func).parameters.keys():
+
+        for v in inspect.getargs(func.__code__).args:
             if v == "self" and parent is not None:
                 args.append(parent)
             elif getter := self._varmap.get(v, None):
-                args.append(getter())
+                args.append(self.call(getter, parent=parent))
             else:
                 raise ValueError(f"Variable {v} not found in storage")
         return func(*args)
 
 
 def get_storage(name: str = "") -> Storage:
     """Get the name specific storage instance."""
```

### Comparing `qt_command_palette-0.0.5/qt_command_palette/_widget.py` & `qt_command_palette-0.0.6/qt_command_palette/_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,19 +60,19 @@
 
         self._line.textChanged.connect(self._on_text_changed)
         self._list.commandClicked.connect(self._on_command_clicked)
         self._line.editingFinished.connect(self.hide)
 
     def match_color(self) -> str:
         """The color used for the matched characters."""
-        return self._list.match_color()
+        return self._list.matchColor
 
-    def set_match_color(self, color: str):
+    def set_match_color(self, color):
         """Set the color used for the matched characters."""
-        return self._list.set_match_color(color)
+        self._list.matchColor = QtGui.QColor(color)
 
     def add_command(self, cmd: Command):
         self._list.add_command(cmd)
         return None
 
     def extend_command(self, list_of_commands: list[Command]):
         self._list.extend_command(list_of_commands)
@@ -113,10 +113,26 @@
             self.move(topleft)
             self.resize(w, self_size.height())
 
         self.raise_()
         self._line.setFocus()
         return None
 
+    def show_center(self):
+        """Show command palette widget in the center of the screen."""
+        self._line.setText("")
+        self._list.update_for_text("")
+        self.setWindowFlags(Qt.WindowType.Dialog | Qt.WindowType.FramelessWindowHint)
+        super().show()
+
+        screen_rect = QtGui.QGuiApplication.primaryScreen().geometry()
+        self.resize(screen_rect.width() * 0.5, screen_rect.height() * 0.5)
+        point = screen_rect.center() - self.rect().center()
+        self.move(point)
+
+        self.raise_()
+        self._line.setFocus()
+        return None
+
     def hide(self):
         self.hidden.emit()
         return super().hide()
```

### Comparing `qt_command_palette-0.0.5/tests/test_register.py` & `qt_command_palette-0.0.6/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.5/.gitignore` & `qt_command_palette-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.5/LICENSE.txt` & `qt_command_palette-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.5/README.md` & `qt_command_palette-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.5/pyproject.toml` & `qt_command_palette-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.5/PKG-INFO` & `qt_command_palette-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-command-palette
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command palette widget for Qt applications
 Project-URL: Documentation, https://github.com/unknown/qt-command-palette#readme
 Project-URL: Issues, https://github.com/unknown/qt-command-palette/issues
 Project-URL: Source, https://github.com/unknown/qt-command-palette
 Author-email: Hanjin Liu <hanjin.liu@bs.s.u-tokyo.ac.jp>
 License: MIT License
```

