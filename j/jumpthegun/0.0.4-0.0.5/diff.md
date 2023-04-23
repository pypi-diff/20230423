# Comparing `tmp/jumpthegun-0.0.4.tar.gz` & `tmp/jumpthegun-0.0.5.tar.gz`

## Comparing `jumpthegun-0.0.4.tar` & `jumpthegun-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/.flake8
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/test_requirements.txt
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tox.ini
--rwxr-xr-x   0        0        0     3343 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun.sh
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/__version__.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/jumpthegunctl.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/output_redirect.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/project.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/testutils.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/tools.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/LICENSE
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/README.md
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/VERSION
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/__init__.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_api.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_error.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_soft.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_unix.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_util.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/test_jumpthegun.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/test_tools.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/testproj/.flake8
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/testproj/bad.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/testproj/good.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/testproj/pyproject.toml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/LICENSE
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/README.md
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/.flake8
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/test_requirements.txt
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tox.ini
+-rwxr-xr-x   0        0        0     5064 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun.sh
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/__version__.py
+-rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/jumpthegunctl.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/output_redirect.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/testutils.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/tools.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/LICENSE
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/README.md
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/VERSION
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/__init__.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_api.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_error.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_soft.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_unix.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_util.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/test_jumpthegun.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/test_tools.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/testproj/.flake8
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/testproj/bad.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/testproj/good.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/testproj/pyproject.toml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/README.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/PKG-INFO
```

### Comparing `jumpthegun-0.0.4/src/jumpthegun/jumpthegunctl.py` & `jumpthegun-0.0.5/src/jumpthegun/jumpthegunctl.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,39 +10,41 @@
 import subprocess
 import sys
 import tempfile
 import time
 import traceback
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, BinaryIO, Optional, Set, Tuple, cast
-
-from vendor.filelock import FileLock
+from typing import Any, BinaryIO, Optional, Tuple, cast
 
 from .__version__ import __version__
+from ._vendor.filelock import FileLock
 from .output_redirect import SocketOutputRedirector
-from .project import get_tool_names
-from .tools import ToolExceptionBase, UnsupportedTool, get_tool_entrypoint
+from .tools import ToolExceptionBase, get_tool_entrypoint
 from .utils import pid_exists
 
 
 class InvalidCommand(Exception):
     def __init__(self, command: str):
         super().__init__(command)
         self.command = command
 
 
 class DaemonAlreadyExistsError(ToolExceptionBase):
     def __str__(self):
-        return f'Jump the Gun daemon process for tool "{self.tool_name}" already exists.'
+        return (
+            f'Jump the Gun daemon process for tool "{self.tool_name}" already exists.'
+        )
 
 
 class DaemonDoesNotExistError(ToolExceptionBase):
     def __str__(self):
-        return f'Jump the Gun daemon process for tool "{self.tool_name}" does not exist.'
+        return (
+            f'Jump the Gun daemon process for tool "{self.tool_name}" does not exist.'
+        )
 
 
 class StdinWrapper(io.RawIOBase):
     """TODO!"""
 
     def __init__(self, sock: socket.socket) -> None:
         self._sock = sock
@@ -81,18 +83,18 @@
     read = readline
 
     def fileno(self) -> Any:
         return self._sock.fileno()
 
 
 def get_xdg_config_dir() -> Path:
-    env_var = os.environ.get('XDG_CONFIG_HOME')
+    env_var = os.environ.get("XDG_CONFIG_HOME")
     if env_var:
         return Path(env_var)
-    return Path.home() / '.config'
+    return Path.home() / ".config"
 
 
 @dataclass(frozen=True)
 class JumpTheGunConfig:
     idle_timeout_seconds: Optional[int] = 4 * 60 * 60  # 4 hours
 
     def __post_init__(self):
@@ -201,15 +203,16 @@
     # Import the tool and get its entrypoint function.
     #
     # Override sys.stdout and sys.stderr while loading the tool runner,
     # so that any references to them kept during module imports (e.g for
     # setting up logging) already reference the overrides.
     output_redirector = SocketOutputRedirector()
     with output_redirector.override_outputs_for_imports():
-        tool_runner = get_tool_entrypoint(tool_name)
+        tool_entrypoint = get_tool_entrypoint(tool_name)
+        tool_runner = tool_entrypoint.load()
 
     pid_file_path, port_file_path = get_pid_and_port_file_paths(tool_name)
 
     if pid_file_path.exists():
         file_pid = int(pid_file_path.read_text())
         if pid_exists(file_pid):
             raise DaemonAlreadyExistsError(tool_name=tool_name)
@@ -263,27 +266,31 @@
             conn, address = sock.accept()
             print(f"Got connection from: {address}")
             newpid = os.fork()
             if newpid == 0:
                 break
 
             # Avoid "zombie" processes: Reap completed sub-processes.
-            done_subproc_pids = {x for x in subproc_pids if os.waitpid(x, os.WNOHANG)[0] != 0}
+            done_subproc_pids = {
+                x for x in subproc_pids if os.waitpid(x, os.WNOHANG)[0] != 0
+            }
             subproc_pids -= done_subproc_pids
             subproc_pids.add(newpid)
     except BaseException as exc:
         # Server is exiting: Clean up as needed.
         sock.close()
         if pid_file_path.exists():
             file_pid = int(pid_file_path.read_text())
             if file_pid == pid:
                 pid_file_path.unlink(missing_ok=True)
                 port_file_path.unlink(missing_ok=True)
         if isinstance(exc, socket.timeout):
-            print(f"Exiting after receiving no connections for {config.idle_timeout_seconds} seconds.")
+            print(
+                f"Exiting after receiving no connections for {config.idle_timeout_seconds} seconds."
+            )
             return
         raise
 
     # Send pid.
     conn.sendall(b"%d\n" % os.getpid())
 
     rfile = conn.makefile("rb", 0)
@@ -326,15 +333,15 @@
         conn.shutdown(socket.SHUT_WR)
         sys.exit(0)
 
 
 def stop(tool_name: str) -> None:
     try:
         get_tool_entrypoint(tool_name)
-    except UnsupportedTool:
+    except ToolExceptionBase:
         raise DaemonDoesNotExistError(tool_name)
 
     try:
         pid_file_path, _port_file_path = get_pid_and_port_file_paths(tool_name)
         if not pid_file_path.exists():
             raise DaemonDoesNotExistError(tool_name)
 
@@ -389,58 +396,23 @@
         if cmd == "version" or cmd == "--version":
             print(f"jumpthegun v{__version__}")
             sys.exit(0)
     elif len(args) == 2:
         (cmd, tool_name) = args
         tool_name = tool_name.strip().lower()
 
-        if tool_name == "all":
-            tool_names = get_tool_names(Path.cwd())
-            failed_for_tools: Set[str] = set()
-            for _tool_name in tool_names:
-                try:
-                    do_action(tool_name=_tool_name, action=cmd)
-                except ToolExceptionBase:
-                    failed_for_tools.add(_tool_name)
-
-            succeeded_for_tools = set(tool_names) - failed_for_tools
-            if cmd == "restart":
-                if succeeded_for_tools:
-                    print(
-                        "Restarted jumpthegun daemons for tools:",
-                        ", ".join(sorted(succeeded_for_tools)),
-                    )
-                    sys.exit(0)
-                if failed_for_tools:
-                    print(
-                        "Failed to restart jumpthegun daemons for tools:",
-                        ", ".join(sorted(failed_for_tools)),
-                    )
-                    sys.exit(1)
-            elif cmd == "start" or cmd == "stop":
-                if succeeded_for_tools:
-                    action_str = "Stopped" if cmd == "stop" else "Started"
-                    print(
-                        f"{action_str} jumpthegun daemons for tools:",
-                        ", ".join(sorted(succeeded_for_tools)),
-                    )
-                    sys.exit(0)
-                else:
-                    print(f"No tools to {cmd} jumpthegun daemons for.")
-                    sys.exit(0)
+        try:
+            do_action(tool_name=tool_name, action=cmd)
+        except ToolExceptionBase as exc:
+            print(str(exc))
+            sys.exit(1)
+        except InvalidCommand as exc:
+            print(str(exc))
         else:
-            try:
-                do_action(tool_name=tool_name, action=cmd)
-            except ToolExceptionBase as exc:
-                print(str(exc))
-                sys.exit(1)
-            except InvalidCommand as exc:
-                print(str(exc))
-            else:
-                sys.exit(0)
+            sys.exit(0)
 
     print_usage()
     sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jumpthegun-0.0.4/src/jumpthegun/output_redirect.py` & `jumpthegun-0.0.5/src/jumpthegun/output_redirect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import contextlib
 import functools
 import io
 import socket
 import sys
-from typing import Any, BinaryIO, Union, cast
+from typing import Any, BinaryIO, Optional, Union, cast
 
 
 class SocketOutputRedirector:
     """Helper class for redirecting stdout and stderr.
 
     This redirects to a socket, writing in the JumpTheGun protocol.
 
@@ -15,14 +15,15 @@
     temporarily override stdout and stderr, buffering all data written
     to them.
 
     Later, use .set_socket() to set the socket to be written to and
     override stdout and stderr in a final manner.  At this point, any
     buffered data will be written to the socket.
     """
+
     def __init__(self):
         self._stdout_socket_writer = SocketWriter(prefix=b"1")
         self._stdout = io.TextIOWrapper(
             cast(BinaryIO, self._stdout_socket_writer), write_through=True
         )
         self._stderr_socket_writer = SocketWriter(prefix=b"2")
         self._stderr = io.TextIOWrapper(
@@ -34,18 +35,18 @@
 
     @contextlib.contextmanager
     def override_outputs_for_imports(self):
         prev_stdout = sys.stdout
         prev_stderr = sys.stderr
 
         self._override_output_stream_write(
-            self._stdout, self._stdout_socket_writer, self._stdout_buffer,
+            self._stdout, self._stdout_socket_writer, self._stdout_buffer
         )
         self._override_output_stream_write(
-            self._stderr, self._stderr_socket_writer, self._stderr_buffer,
+            self._stderr, self._stderr_socket_writer, self._stderr_buffer
         )
         sys.stdout = self._stdout
         sys.stderr = self._stderr
         try:
             yield
         finally:
             sys.stdout = prev_stdout
@@ -54,15 +55,15 @@
             del self._stderr.write
 
     @classmethod
     def _override_output_stream_write(cls, stream, socket_writer, buffer):
         orig_write = stream.write
 
         @functools.wraps(orig_write)
-        def new_write(data: str, /):
+        def new_write(data: str):
             if not socket_writer.has_socket():
                 buffer.append(data)
                 return len(data)
             else:
                 return orig_write(data)
 
         stream.write = new_write
@@ -84,15 +85,16 @@
 class SocketWriter(io.RawIOBase):
     """Output adapter implementing the file interface.
 
     This writes lines to a socket in the JumpTheGun protocol.
 
     The socket is set after initialization via .set_socket().
     """
-    _sock: socket.socket | None
+
+    _sock: Optional[socket.socket]
 
     def __init__(self, prefix: bytes) -> None:
         self._sock = None
         self._prefix = prefix
 
     def readable(self) -> bool:
         return False
```

### Comparing `jumpthegun-0.0.4/src/jumpthegun/utils.py` & `jumpthegun-0.0.5/src/jumpthegun/utils.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/src/vendor/filelock/LICENSE` & `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/src/vendor/filelock/README.md` & `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/README.md`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/src/vendor/filelock/__init__.py` & `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/__init__.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/src/vendor/filelock/_api.py` & `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_api.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/src/vendor/filelock/_soft.py` & `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_soft.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/src/vendor/filelock/_unix.py` & `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_unix.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/src/vendor/filelock/_util.py` & `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_util.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/src/vendor/filelock/_windows.py` & `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_windows.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/tests/test_jumpthegun.py` & `jumpthegun-0.0.5/tests/test_jumpthegun.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,85 +13,108 @@
 
 def get_bin_path(project_path: Path) -> Path:
     venv_path = project_path.with_name(project_path.name + "_venv")
     bin_dir_name = "Scripts" if sys.platform == "win32" else "bin"
     return venv_path / bin_dir_name
 
 
-# @pytest.fixture(scope="session")
-# def setup_testproj() -> Path:
-#     with tempfile.TemporaryDirectory() as tmp_dir:
-#         proj_dir = Path(tmp_dir) / "testproj"
-#         shutil.copytree(Path(__file__).parent / "testproj", proj_dir)
-#         venv_path = proj_dir / "venv"
-#         subprocess.run([sys.executable, "-mvenv", str(venv_path)])
-#         bin_path = get_bin_path(proj_dir)
-#         subprocess.run([str(bin_path / "pip"), "install", ".", "black", "flake8", "isort"], cwd=str(Path(__file__).parents[1]), check=True)
-#         yield proj_dir
-#
-#
-# @pytest.fixture
-# def testproj(setup_testproj, tmp_path) -> Path:
-#     proj_dir = Path(tmp_path) / "testproj"
-#     shutil.copytree(setup_testproj, proj_dir)
-#     yield proj_dir
+@pytest.fixture
+def testproj(request, testproj_with_jumpthegun, testproj_without_jumpthegun) -> Path:
+    testproj_name = getattr(request, "param", "testproj_without_jumpthegun")
+    if testproj_name == "testproj_with_jumpthegun":
+        return testproj_with_jumpthegun
+    elif testproj_name == "testproj_without_jumpthegun":
+        return testproj_without_jumpthegun
 
 
 @pytest.fixture(scope="session")
-def testproj() -> Path:
+def testproj_with_jumpthegun() -> Path:
+    return _setup_test_project("testproj_with_jumpthegun", with_jumpthegun=True)
+
+
+@pytest.fixture(scope="session")
+def testproj_without_jumpthegun() -> Path:
+    return _setup_test_project("testproj_without_jumpthegun", with_jumpthegun=False)
+
+
+def _setup_test_project(name: str, with_jumpthegun: bool) -> Path:
     root_dir = Path(__file__).parent.parent
     testenvs_dir = root_dir / ".testenvs"
     testenvs_dir.mkdir(exist_ok=True)
     ver_dir = testenvs_dir / sys.version.split()[0]
     ver_dir.mkdir(exist_ok=True)
 
-    proj_dir = ver_dir / "testproj"
+    proj_dir = ver_dir / name
     if not proj_dir.exists():
         sources_dir = Path(__file__).parent / "testproj"
         shutil.copytree(sources_dir, proj_dir)
         venv_path = get_bin_path(proj_dir).parent
-        subprocess.run([sys.executable, "-m", "venv", str(venv_path.resolve())], check=True)
-        bin_path = get_bin_path(proj_dir)
         subprocess.run(
-            [str(bin_path / "pip"), "install", "black", "flake8", "isort"],
-            cwd=str(root_dir),
+            [sys.executable, "-m", "venv", str(venv_path.resolve())],
             check=True,
         )
+        bin_path = get_bin_path(proj_dir)
+        if with_jumpthegun:
+            # Need pip >= 21.3 for editable installation without setup.py.
+            # See: https://pip.pypa.io/en/stable/news/#v21-3
+            subprocess.run(
+                [str(bin_path / "pip"), "install", "--upgrade", "pip >= 21.3"],
+                cwd=str(root_dir),
+                check=True,
+            )
         subprocess.run(
-            [str(bin_path / "pip"), "install", "-e", "."],
+            [str(bin_path / "pip"), "install", "black", "flake8", "isort"],
             cwd=str(root_dir),
             check=True,
         )
-        sleep_and_exit_on_signal_script = textwrap.dedent("""\
+        if with_jumpthegun:
+            subprocess.run(
+                [str(bin_path / "pip"), "install", "-e", "."],
+                cwd=str(root_dir),
+                check=True,
+            )
+        sleep_and_exit_on_signal_script = textwrap.dedent(
+            """\
             #!/usr/bin/env python
             import jumpthegun.testutils
 
             jumpthegun.testutils.sleep_and_exit_on_signal()
-            """)
-        (bin_path / "__test_sleep_and_exit_on_signal").write_text(sleep_and_exit_on_signal_script)
+            """
+        )
+        script_path = bin_path / "__test_sleep_and_exit_on_signal"
+        script_path.write_text(sleep_and_exit_on_signal_script)
+        script_path.chmod(0o755)
 
-    yield proj_dir
+    return proj_dir
 
 
 @pytest.mark.parametrize(
+    "testproj",
+    ["testproj_with_jumpthegun", "testproj_without_jumpthegun"],
+    ids=["testproj_with_jumpthegun", "testproj_without_jumpthegun"],
+    indirect=True,
+)
+@pytest.mark.parametrize(
     "tool_cmd",
     [
         ["black", "--check", "."],
         ["isort", "--check", "."],
         ["flake8"],
     ],
     ids=lambda tool_cmd: tool_cmd[0],
 )
 def test_jumpthegun_start_run_stop(testproj, tool_cmd):
     without_jumpthegun_proc = run(tool_cmd, proj_path=testproj)
     assert without_jumpthegun_proc.returncode != 0
 
     run(["jumpthegun", "start", tool_cmd[0]], proj_path=testproj, check=True)
     try:
-        proc1 = run(["jumpthegun", "run", "--no-autorun", *tool_cmd], proj_path=testproj)
+        proc1 = run(
+            ["jumpthegun", "run", "--no-autorun", *tool_cmd], proj_path=testproj
+        )
         proc2 = run(["jumpthegun", "run", *tool_cmd], proj_path=testproj)
     finally:
         run(["jumpthegun", "stop", tool_cmd[0]], proj_path=testproj, check=True)
 
     assert proc1.stdout == without_jumpthegun_proc.stdout
     assert proc1.stderr == without_jumpthegun_proc.stderr
     assert proc1.returncode == without_jumpthegun_proc.returncode
@@ -104,17 +127,21 @@
 def test_jumpthegun_autorun(testproj):
     tool_cmd = ["flake8"]
 
     without_jumpthegun_proc = run(tool_cmd, proj_path=testproj)
     assert without_jumpthegun_proc.returncode != 0
 
     try:
-        proc1 = run(["jumpthegun", "run", "--no-autorun", *tool_cmd], proj_path=testproj)
+        proc1 = run(
+            ["jumpthegun", "run", "--no-autorun", *tool_cmd], proj_path=testproj
+        )
         proc2 = run(["jumpthegun", "run", *tool_cmd], proj_path=testproj)
-        proc3 = run(["jumpthegun", "run", "--no-autorun", *tool_cmd], proj_path=testproj)
+        proc3 = run(
+            ["jumpthegun", "run", "--no-autorun", *tool_cmd], proj_path=testproj
+        )
     finally:
         run(["jumpthegun", "stop", tool_cmd[0]], proj_path=testproj, check=True)
 
     assert proc1.stdout == without_jumpthegun_proc.stdout
     assert proc1.stderr == without_jumpthegun_proc.stderr
     assert proc1.returncode == without_jumpthegun_proc.returncode
 
@@ -123,37 +150,51 @@
     assert proc2.returncode == without_jumpthegun_proc.returncode
 
     assert proc3.stdout == without_jumpthegun_proc.stdout
     assert proc3.stderr == without_jumpthegun_proc.stderr
     assert proc3.returncode == without_jumpthegun_proc.returncode
 
 
-@pytest.mark.parametrize("signum", [signal.SIGINT, signal.SIGTERM, signal.SIGUSR1, signal.SIGUSR2])
+@pytest.mark.parametrize(
+    "testproj",
+    ["testproj_with_jumpthegun", "testproj_without_jumpthegun"],
+    ids=["testproj_with_jumpthegun", "testproj_without_jumpthegun"],
+    indirect=True,
+)
+@pytest.mark.parametrize(
+    "signum", [signal.SIGINT, signal.SIGTERM, signal.SIGUSR1, signal.SIGUSR2]
+)
 def test_signal_forwarding(testproj, signum):
     subcmd = ["__test_sleep_and_exit_on_signal"]
     run(["jumpthegun", "start", subcmd[0]], proj_path=testproj, check=True)
     try:
-        proc: subprocess.Popen = run(["jumpthegun", "run", "--no-autorun", *subcmd], proj_path=testproj, background=True)
+        proc: subprocess.Popen = run(
+            ["jumpthegun", "run", "--no-autorun", *subcmd],
+            proj_path=testproj,
+            background=True,
+        )
         assert proc.stdout.readline() == b"Sleeping...\n"
         assert proc.poll() is None
         proc.send_signal(signum)
         proc.wait(2)
         assert b"Received signal" in proc.stdout.read()
     finally:
         run(["jumpthegun", "stop", subcmd[0]], proj_path=testproj, check=True)
 
 
-def run(cmd: List[str], proj_path: Path, background: bool = False, check: bool = False) -> Union[subprocess.CompletedProcess, subprocess.Popen]:
+def run(
+    cmd: List[str], proj_path: Path, background: bool = False, check: bool = False
+) -> Union[subprocess.CompletedProcess, subprocess.Popen]:
     if background and check:
         raise ValueError("Must not set both background=True and check=True.")
 
     pass_through_env_vars = {
         key: value
         for key, value in os.environ.items()
-        if re.fullmatch(r"TMPDIR|USER|XDG_.*", key)
+        if re.fullmatch(r"HOME|TMPDIR|USER|XDG_.*", key)
     }
 
     bin_path = get_bin_path(proj_path).resolve()
     proc_kwargs = dict(
         cwd=str(proj_path),
         env={
             **pass_through_env_vars,
```

### Comparing `jumpthegun-0.0.4/.gitignore` & `jumpthegun-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/LICENSE` & `jumpthegun-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.4/README.md` & `jumpthegun-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,21 +16,25 @@
 This is especially significant, for example, when running code linting and
 formatting tools on just a few files in SCM hooks, such as via
 [pre-commit](https://pre-commit.com/).
 
 
 # Installation
 
-Install into the same Python env where you have tools like black or flake8
-installed:
+Install JumpTheGun into any Python environment (Python >= 3.7):
 
 ```shell
 pip install jumpthegun
 ```
 
+Or use [pipx](https://pypa.github.io/pipx/):
+```shell
+pipx install jumpthegun
+```
+
 
 # Usage
 
 Example:
 
 ```shell
 jumpthegun run black --help
```

### Comparing `jumpthegun-0.0.4/pyproject.toml` & `jumpthegun-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-  "tomli>=1.1.0; python_version < '3.11'",
+  "importlib_metadata; python_version < '3.8'",
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
   "pytest>=7,<8",
@@ -63,16 +63,16 @@
 [tool.hatch.build.targets.wheel.shared-data]
 "src/jumpthegun.sh" = "bin/jumpthegun"
 
 [tool.black]
 line-length = 88
 target-version = ["py37", "py38", "py39", "py310", "py311"]
 include = '\.pyi?$'
-extend-exclude = 'vendor|tests/testproj'
+extend-exclude = 'src/jumpthegun/_vendor|tests/testproj'
 
 [tool.isort]
 atomic = true
 profile = "black"
 line_length = 88
 skip_gitignore = true
-extend_skip_glob = ["vendor", "tests/testproj"]
+extend_skip_glob = ["src/jumpthegun/_vendor", "tests/testproj"]
 known_first_party = ["jumpthegun"]
```

### Comparing `jumpthegun-0.0.4/PKG-INFO` & `jumpthegun-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumpthegun
-Version: 0.0.4
+Version: 0.0.5
 Summary: Make Python CLI tools win the speed race, by cheating!
 Project-URL: Homepage, https://github.com/taleinat/jumpthegun
 Author-email: Tal Einat <taleinat@gmail.com>
 License: Apache-2.0
 License-File: LICENSE
 Keywords: cli
 Classifier: Development Status :: 1 - Planning
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
-Requires-Dist: tomli>=1.1.0; python_version < '3.11'
+Requires-Dist: importlib-metadata; python_version < '3.8'
 Provides-Extra: test
 Requires-Dist: pytest<8,>=7; extra == 'test'
 Description-Content-Type: text/markdown
 
 Jump the Gun
 ============
 Make Python CLI tools win the speed race, by cheating!
@@ -45,21 +45,25 @@
 This is especially significant, for example, when running code linting and
 formatting tools on just a few files in SCM hooks, such as via
 [pre-commit](https://pre-commit.com/).
 
 
 # Installation
 
-Install into the same Python env where you have tools like black or flake8
-installed:
+Install JumpTheGun into any Python environment (Python >= 3.7):
 
 ```shell
 pip install jumpthegun
 ```
 
+Or use [pipx](https://pypa.github.io/pipx/):
+```shell
+pipx install jumpthegun
+```
+
 
 # Usage
 
 Example:
 
 ```shell
 jumpthegun run black --help
```

