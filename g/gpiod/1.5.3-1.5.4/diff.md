# Comparing `tmp/gpiod-1.5.3.tar.gz` & `tmp/gpiod-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpiod-1.5.3.tar", last modified: Fri Feb 11 10:14:03 2022, max compression
+gzip compressed data, was "gpiod-1.5.4.tar", last modified: Sun Apr 23 10:20:54 2023, max compression
```

## Comparing `gpiod-1.5.3.tar` & `gpiod-1.5.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:14:03.241308 gpiod-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-02-11 10:13:49.000000 gpiod-1.5.3/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-02-11 10:13:49.000000 gpiod-1.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-02-11 10:13:49.000000 gpiod-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7416 2022-02-11 10:14:03.241308 gpiod-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-02-11 10:13:49.000000 gpiod-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:14:03.237308 gpiod-1.5.3/py_src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:14:03.237308 gpiod-1.5.3/py_src/gpiod/
--rw-r--r--   0 runner    (1001) docker     (121)     2308 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:14:03.241308 gpiod-1.5.3/py_src/gpiod/kernel/
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/kernel/gpio_h.py
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/kernel/ioctl_h.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:14:03.241308 gpiod-1.5.3/py_src/gpiod/libgpiod/
--rw-r--r--   0 runner    (1001) docker     (121)    35951 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/libgpiod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4788 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/libgpiod/gpiod_h.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:14:03.241308 gpiod-1.5.3/py_src/gpiod/libgpiodcxx/
--rw-r--r--   0 runner    (1001) docker     (121)    36851 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/libgpiodcxx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:14:03.241308 gpiod-1.5.3/py_src/gpiod/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/test/blink.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/test/bulk_blink.py
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/test/bulk_button.py
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/test/button.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-02-11 10:13:49.000000 gpiod-1.5.3/py_src/gpiod/test/sequential_blink.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:14:03.241308 gpiod-1.5.3/py_src/gpiod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7416 2022-02-11 10:14:02.000000 gpiod-1.5.3/py_src/gpiod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-02-11 10:14:03.000000 gpiod-1.5.3/py_src/gpiod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 10:14:02.000000 gpiod-1.5.3/py_src/gpiod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 10:14:02.000000 gpiod-1.5.3/py_src/gpiod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-11 10:14:02.000000 gpiod-1.5.3/py_src/gpiod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-02-11 10:14:03.241308 gpiod-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-02-11 10:13:49.000000 gpiod-1.5.3/setup.py
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-04-23 10:20:54.098371 gpiod-1.5.4/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     6198 2023-04-23 10:17:29.000000 gpiod-1.5.4/CHANGELOG
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1093 2023-04-23 09:03:08.000000 gpiod-1.5.4/LICENSE.txt
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)       90 2023-04-23 09:03:08.000000 gpiod-1.5.4/MANIFEST.in
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     7584 2023-04-23 10:20:54.098371 gpiod-1.5.4/PKG-INFO
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      685 2023-04-23 09:03:08.000000 gpiod-1.5.4/README.md
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-04-23 10:20:54.095038 gpiod-1.5.4/py_src/
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-04-23 10:20:54.098371 gpiod-1.5.4/py_src/gpiod/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     2303 2023-04-23 09:40:28.000000 gpiod-1.5.4/py_src/gpiod/__init__.py
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-04-23 10:20:54.098371 gpiod-1.5.4/py_src/gpiod/kernel/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1124 2023-04-23 09:03:08.000000 gpiod-1.5.4/py_src/gpiod/kernel/__init__.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     3905 2023-04-23 09:18:05.000000 gpiod-1.5.4/py_src/gpiod/kernel/gpio_h.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     2108 2023-04-23 09:03:08.000000 gpiod-1.5.4/py_src/gpiod/kernel/ioctl_h.py
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-04-23 10:20:54.098371 gpiod-1.5.4/py_src/gpiod/libgpiod/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)    35757 2023-04-23 10:12:01.000000 gpiod-1.5.4/py_src/gpiod/libgpiod/__init__.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     4788 2023-04-23 09:03:08.000000 gpiod-1.5.4/py_src/gpiod/libgpiod/gpiod_h.py
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-04-23 10:20:54.098371 gpiod-1.5.4/py_src/gpiod/libgpiodcxx/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)    36023 2023-04-23 09:37:15.000000 gpiod-1.5.4/py_src/gpiod/libgpiodcxx/__init__.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)        1 2023-04-23 09:03:08.000000 gpiod-1.5.4/py_src/gpiod/py.typed
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-04-23 10:20:54.098371 gpiod-1.5.4/py_src/gpiod/test/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1102 2023-04-23 09:03:08.000000 gpiod-1.5.4/py_src/gpiod/test/__init__.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     2343 2023-04-23 09:11:06.000000 gpiod-1.5.4/py_src/gpiod/test/blink.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      860 2023-04-23 09:11:06.000000 gpiod-1.5.4/py_src/gpiod/test/bulk_blink.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1514 2023-04-23 09:32:47.000000 gpiod-1.5.4/py_src/gpiod/test/bulk_button.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1406 2023-04-23 09:11:06.000000 gpiod-1.5.4/py_src/gpiod/test/button.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      930 2023-04-23 09:32:57.000000 gpiod-1.5.4/py_src/gpiod/test/sequential_blink.py
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-04-23 10:20:54.098371 gpiod-1.5.4/py_src/gpiod.egg-info/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     7584 2023-04-23 10:20:54.000000 gpiod-1.5.4/py_src/gpiod.egg-info/PKG-INFO
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      688 2023-04-23 10:20:54.000000 gpiod-1.5.4/py_src/gpiod.egg-info/SOURCES.txt
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)        1 2023-04-23 10:20:54.000000 gpiod-1.5.4/py_src/gpiod.egg-info/dependency_links.txt
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)        1 2023-04-23 10:08:18.000000 gpiod-1.5.4/py_src/gpiod.egg-info/not-zip-safe
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)        6 2023-04-23 10:20:54.000000 gpiod-1.5.4/py_src/gpiod.egg-info/top_level.txt
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)    20954 2023-04-23 09:43:25.000000 gpiod-1.5.4/pyproject.toml
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      835 2023-04-23 10:20:54.101704 gpiod-1.5.4/setup.cfg
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1354 2023-04-23 09:03:08.000000 gpiod-1.5.4/setup.py
```

### Comparing `gpiod-1.5.3/CHANGELOG` & `gpiod-1.5.4/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.5.4
+
+- chore: change max-line-length and run black and isort by @hhk7734 in #36
+- Fixed issue when gpio chip has no label by @yacinbm in #35
+- Also build a py3-none-any wheel by @rmelick-muon in #33
+
 ## 1.5.3
 
 - libgpiod: update typing for return values #27
 - libgpiod: update typing for return values #27
 
 ## 1.5.2
```

### Comparing `gpiod-1.5.3/LICENSE.txt` & `gpiod-1.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gpiod-1.5.3/PKG-INFO` & `gpiod-1.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: gpiod
-Version: 1.5.3
-Summary: UNKNOWN
+Version: 1.5.4
 Home-page: https://github.com/hhk7734/python3-gpiod
 Author: Hyeonki Hong
 Author-email: hhk7734@gmail.com
 License: MIT
 Project-URL: Documentation, https://wiki.loliot.net/docs/lang/python/libraries/gpiod/python-gpiod-about
 Project-URL: "Source Code", https://github.com/hhk7734/python3-gpiod
 Keywords: GPIO,gpiod
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Hardware
 Description-Content-Type: text/markdown
@@ -37,14 +35,20 @@
 python3 -m pip install -U --user pip gpiod
 ```
 
 ## Changelog
 
 Ref: CHANGELOG
 
+## 1.5.4
+
+- chore: change max-line-length and run black and isort by @hhk7734 in #36
+- Fixed issue when gpio chip has no label by @yacinbm in #35
+- Also build a py3-none-any wheel by @rmelick-muon in #33
+
 ## 1.5.3
 
 - libgpiod: update typing for return values #27
 - libgpiod: update typing for return values #27
 
 ## 1.5.2
 
@@ -239,9 +243,7 @@
  -- Hyeonki Hong <hhk7734@gmail.com>  Wed, 11 Mar 2020 13:28:45 +0900
 
 python3-gpiod (0.1.0) unstable; urgency=medium
 
   * Add initial setup files
 
  -- Hyeonki Hong <hhk7734@gmail.com>  Tue, 10 Mar 2020 15:40:13 +0900
-
-
```

### Comparing `gpiod-1.5.3/README.md` & `gpiod-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `gpiod-1.5.3/py_src/gpiod/__init__.py` & `gpiod-1.5.4/py_src/gpiod/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,13 +75,13 @@
     @return New chip iterator object pointing to the first GPIO chip on the
             system.
 
     Usage:
         for c in make_chip_iter():
             print(c.label)
     """
-    return chip_iter().__iter__()
+    return iter(chip_iter())
 
 
 class line_iter(libgpiodcxx.line_iter):
     # pylint: disable=too-few-public-methods
     pass
```

### Comparing `gpiod-1.5.3/py_src/gpiod/kernel/__init__.py` & `gpiod-1.5.4/py_src/gpiod/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `gpiod-1.5.3/py_src/gpiod/kernel/gpio_h.py` & `gpiod-1.5.4/py_src/gpiod/kernel/gpio_h.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from ctypes import c_char, c_uint8, c_uint32, c_uint64, c_int, Structure
+from ctypes import Structure, c_char, c_int, c_uint8, c_uint32, c_uint64
+
 from .ioctl_h import _IOR, _IOWR
 
 # Ref: linux/include/uapi/linux/gpio.h
 # ABI v1
 
 # pylint: disable=too-few-public-methods
 
@@ -99,17 +100,15 @@
 
 GPIOHANDLE_GET_LINE_VALUES_IOCTL = _IOWR(0xB4, 0x08, gpiohandle_data)
 GPIOHANDLE_SET_LINE_VALUES_IOCTL = _IOWR(0xB4, 0x09, gpiohandle_data)
 
 
 GPIOEVENT_REQUEST_RISING_EDGE = 1 << 0
 GPIOEVENT_REQUEST_FALLING_EDGE = 1 << 1
-GPIOEVENT_REQUEST_BOTH_EDGES = (
-    GPIOEVENT_REQUEST_RISING_EDGE | GPIOEVENT_REQUEST_FALLING_EDGE
-)
+GPIOEVENT_REQUEST_BOTH_EDGES = GPIOEVENT_REQUEST_RISING_EDGE | GPIOEVENT_REQUEST_FALLING_EDGE
 
 
 class gpioevent_request(Structure):
     _fields_ = [
         ("lineoffset", c_uint32),
         ("handleflags", c_uint32),
         ("eventflags", c_uint32),
```

### Comparing `gpiod-1.5.3/py_src/gpiod/kernel/ioctl_h.py` & `gpiod-1.5.4/py_src/gpiod/kernel/ioctl_h.py`

 * *Files identical despite different names*

### Comparing `gpiod-1.5.3/py_src/gpiod/libgpiod/__init__.py` & `gpiod-1.5.4/py_src/gpiod/libgpiod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,39 +17,32 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+import select
 from ctypes import memmove, memset, pointer, set_errno, sizeof
 from datetime import datetime, timedelta
 from errno import EBUSY, EINVAL, EIO, ENODEV, ENOENT, ENOTTY, EPERM
 from fcntl import ioctl
-from os import (
-    access,
-    close as os_close,
-    lstat,
-    major,
-    minor,
-    open as os_open,
-    O_CLOEXEC,
-    O_RDWR,
-    read as os_read,
-    R_OK,
-    scandir,
-)
+from os import O_CLOEXEC, O_RDWR, R_OK, access
+from os import close as os_close
+from os import lstat, major, minor
+from os import open as os_open
+from os import read as os_read
+from os import scandir
 from os.path import basename
-import select
 from select import POLLIN, POLLNVAL, POLLPRI
 from stat import S_ISCHR
 from typing import Iterator, List, Optional, Union
 
-from .gpiod_h import *
 from ..kernel import *
+from .gpiod_h import *
 
 # core.c
 
 _LINE_FREE = 0
 _LINE_REQUESTED_VALUES = 1
 _LINE_REQUESTED_EVENTS = 2
 
@@ -67,30 +60,30 @@
         # the same in order to stay compatible with the versions of
         # libgpiod from before the introduction of this routine.
         set_errno(ENOTTY)
         return False
 
     # Do we have a corresponding sysfs attribute?
     name = basename(path)
-    sysfsp = "/sys/bus/gpio/devices/{}/dev".format(name)
+    sysfsp = f"/sys/bus/gpio/devices/{name}/dev"
     if not access(sysfsp, R_OK):
         # This is a character device but not the one we're after.
         # Before the introduction of this function, we'd fail with
         # ENOTTY on the first GPIO ioctl() call for this file
         # descriptor. Let's stay compatible here and keep returning
         # the same error code.
         set_errno(ENOTTY)
         return False
 
     # Make sure the major and minor numbers of the character device
     # correspond to the ones in the dev attribute in sysfs.
-    devstr = "{}:{}".format(major(statbuf.st_rdev), minor(statbuf.st_rdev))
+    devstr = f"{major(statbuf.st_rdev)}:{minor(statbuf.st_rdev)}"
 
     try:
-        with open(sysfsp, "r") as fd:
+        with open(sysfsp, "r", encoding="utf-8") as fd:
             sysfsdev = fd.read(len(devstr))
     except FileNotFoundError:
         return False
 
     if sysfsdev != devstr:
         set_errno(ENODEV)
         return False
@@ -120,22 +113,20 @@
         return None
 
     status = ioctl(fd, GPIO_GET_CHIPINFO_IOCTL, info)
     if status < 0:
         os_close(fd)
         return None
 
-    if info.label[0] == "\0":
+    if not info.label or info.label[0] == "\0":
         label = "unknown"
     else:
         label = info.label.decode()
 
-    return gpiod_chip(
-        num_lines=info.lines, fd=fd, name=info.name.decode(), label=label
-    )
+    return gpiod_chip(num_lines=info.lines, fd=fd, name=info.name.decode(), label=label)
 
 
 def gpiod_chip_close(chip: gpiod_chip) -> None:
     """
     @brief Close a GPIO chip handle and release all allocated resources.
 
     @param chip: The GPIO chip object.
@@ -312,18 +303,18 @@
             set_errno(EBUSY)
             return False
 
     return True
 
 
 def _line_request_direction_is_valid(direction: int) -> bool:
-    if (
-        direction == GPIOD_LINE_REQUEST_DIRECTION_AS_IS
-        or direction == GPIOD_LINE_REQUEST_DIRECTION_INPUT
-        or direction == GPIOD_LINE_REQUEST_DIRECTION_OUTPUT
+    if direction in (
+        GPIOD_LINE_REQUEST_DIRECTION_AS_IS,
+        GPIOD_LINE_REQUEST_DIRECTION_INPUT,
+        GPIOD_LINE_REQUEST_DIRECTION_OUTPUT,
     ):
         return True
 
     set_errno(EINVAL)
     return False
 
 
@@ -357,19 +348,15 @@
 
 def _line_request_values(
     bulk: gpiod_line_bulk,
     config: gpiod_line_request_config,
     default_vals: List[int],
 ) -> int:
     if config.request_type != GPIOD_LINE_REQUEST_DIRECTION_OUTPUT and (
-        config.flags
-        & (
-            GPIOD_LINE_REQUEST_FLAG_OPEN_DRAIN
-            | GPIOD_LINE_REQUEST_FLAG_OPEN_SOURCE
-        )
+        config.flags & (GPIOD_LINE_REQUEST_FLAG_OPEN_DRAIN | GPIOD_LINE_REQUEST_FLAG_OPEN_SOURCE)
     ):
         set_errno(EINVAL)
         return -1
 
     if (config.flags & GPIOD_LINE_REQUEST_FLAG_OPEN_DRAIN) and (
         config.flags & GPIOD_LINE_REQUEST_FLAG_OPEN_SOURCE
     ):
@@ -385,18 +372,15 @@
     if config.request_type == GPIOD_LINE_REQUEST_DIRECTION_INPUT:
         req.flags |= GPIOHANDLE_REQUEST_INPUT
     elif config.request_type == GPIOD_LINE_REQUEST_DIRECTION_OUTPUT:
         req.flags |= GPIOHANDLE_REQUEST_OUTPUT
 
     for i in range(bulk.num_lines):
         req.lineoffsets[i] = bulk[i].offset
-        if (
-            config.request_type == GPIOD_LINE_REQUEST_DIRECTION_OUTPUT
-            and default_vals
-        ):
+        if config.request_type == GPIOD_LINE_REQUEST_DIRECTION_OUTPUT and default_vals:
             req.default_values[i] = 1 if default_vals[i] else 0
 
     if config.consumer:
         req.consumer_label = config.consumer[:32].encode()
 
     fd = bulk[0].chip.fd
 
@@ -419,17 +403,15 @@
         if rv:
             gpiod_line_release_bulk(bulk)
             return rv
 
     return 0
 
 
-def _line_request_event_single(
-    line: gpiod_line, config: gpiod_line_request_config
-) -> int:
+def _line_request_event_single(line: gpiod_line, config: gpiod_line_request_config) -> int:
     # pylint: disable=no-member
     req = gpioevent_request()
     if config.consumer:
         req.consumer_label = config.consumer[:32].encode()
 
     req.lineoffset = line.offset
     req.handleflags = _line_request_flag_to_gpio_handleflag(config.flags)
@@ -457,17 +439,15 @@
     if rv:
         gpiod_line_release(line)
         return rv
 
     return 0
 
 
-def _line_request_events(
-    bulk: gpiod_line_bulk, config: gpiod_line_request_config
-) -> int:
+def _line_request_events(bulk: gpiod_line_bulk, config: gpiod_line_request_config) -> int:
     for i in range(bulk.num_lines):
         status = _line_request_event_single(bulk[i], config)
         if status < 0:
             for j in range(i):
                 gpiod_line_release(bulk[j])
 
             return -1
@@ -579,18 +559,15 @@
     """
     @brief Check if the calling user has ownership of this line.
 
     @param line: GPIO line object.
 
     @return True if given line was requested, false otherwise.
     """
-    return (
-        line.state == _LINE_REQUESTED_VALUES
-        or line.state == _LINE_REQUESTED_EVENTS
-    )
+    return line.state in (_LINE_REQUESTED_VALUES, _LINE_REQUESTED_EVENTS)
 
 
 def gpiod_line_is_free(line: gpiod_line) -> bool:
     """
     @brief Check if the calling user has neither requested ownership of this
            line nor configured any event notifications.
 
@@ -666,17 +643,15 @@
     bulk = gpiod_line_bulk()
 
     bulk.add(line)
 
     return gpiod_line_set_value_bulk(bulk, [value])
 
 
-def gpiod_line_set_value_bulk(
-    bulk: gpiod_line_bulk, values: Optional[List[int]] = None
-) -> int:
+def gpiod_line_set_value_bulk(bulk: gpiod_line_bulk, values: Optional[List[int]] = None) -> int:
     """
     @brief Set the values of a set of GPIO lines.
 
     @param bulk:   Set of GPIO lines to reserve.
     @param values: An array holding line_bulk->num_lines new values for lines.
 
     @return 0 is the operation succeeds. In case of an error this routine
@@ -704,17 +679,15 @@
 
     for i, line in enumerate(bulk):
         line.output_value = data.values[i]
 
     return 0
 
 
-def gpiod_line_set_config(
-    line: gpiod_line, direction: int, flags: int, value: int
-) -> int:
+def gpiod_line_set_config(line: gpiod_line, direction: int, flags: int, value: int) -> int:
     """
     @brief Update the configuration of a single GPIO line.
 
     @param line:      GPIO line object.
     @param direction: Updated direction which may be one of
                       GPIOD_LINE_REQUEST_DIRECTION_AS_IS,
                       GPIOD_LINE_REQUEST_DIRECTION_INPUT, or
@@ -844,17 +817,15 @@
     @brief Set the direction of a single GPIO line to input.
 
     @param line: GPIO line object.
 
     @return 0 is the operation succeeds. In case of an error this routine
             returns -1 and sets the last error number.
     """
-    return gpiod_line_set_config(
-        line, GPIOD_LINE_REQUEST_DIRECTION_INPUT, line.req_flags, 0
-    )
+    return gpiod_line_set_config(line, GPIOD_LINE_REQUEST_DIRECTION_INPUT, line.req_flags, 0)
 
 
 def gpiod_line_set_direction_input_bulk(bulk: gpiod_line_bulk) -> int:
     """
     @brief Set the direction of a set of GPIO lines to input.
 
     @param bulk: Set of GPIO lines.
@@ -878,22 +849,18 @@
 
     @param line:  GPIO line object.
     @param value: The logical value output on the line.
 
     @return 0 is the operation succeeds. In case of an error this routine
             returns -1 and sets the last error number.
     """
-    return gpiod_line_set_config(
-        line, GPIOD_LINE_REQUEST_DIRECTION_OUTPUT, line.req_flags, value
-    )
+    return gpiod_line_set_config(line, GPIOD_LINE_REQUEST_DIRECTION_OUTPUT, line.req_flags, value)
 
 
-def gpiod_line_set_direction_output_bulk(
-    bulk: gpiod_line_bulk, values: Optional[List[int]]
-) -> int:
+def gpiod_line_set_direction_output_bulk(bulk: gpiod_line_bulk, values: Optional[List[int]]) -> int:
     """
     @brief Set the direction of a set of GPIO lines to output.
 
     @param bulk:   Set of GPIO lines.
     @param values: An array holding line_bulk->num_lines new logical values
                 for lines.  A NULL pointer is interpreted as a logical low
                 for all lines.
@@ -950,17 +917,15 @@
     fd_to_line = {}
 
     for it in bulk:
         poll.register(it.fd_handle.fd, POLLIN | POLLPRI)
         fd_to_line[it.fd_handle.fd] = it
 
     timeout_ms = (
-        (timeout.days * 86_400_000)
-        + (timeout.seconds * 1_000)
-        + (timeout.microseconds / 1000.0)
+        (timeout.days * 86_400_000) + (timeout.seconds * 1_000) + (timeout.microseconds / 1000.0)
     )
 
     revents = poll.poll(timeout_ms)
 
     if revents is None:
         return -1
     if len(revents) == 0:
```

### Comparing `gpiod-1.5.3/py_src/gpiod/libgpiod/gpiod_h.py` & `gpiod-1.5.4/py_src/gpiod/libgpiod/gpiod_h.py`

 * *Files identical despite different names*

### Comparing `gpiod-1.5.3/py_src/gpiod/libgpiodcxx/__init__.py` & `gpiod-1.5.4/py_src/gpiod/libgpiodcxx/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,17 +58,15 @@
 def chip_deleter(chip_struct: libgpiod.gpiod_chip) -> None:
     # pylint: disable=missing-function-docstring
     libgpiod.gpiod_chip_close(chip_struct)
 
 
 class shared_chip:
     # pylint: disable=missing-function-docstring
-    def __init__(
-        self, chip_struct: Optional[libgpiod.gpiod_chip] = None
-    ) -> None:
+    def __init__(self, chip_struct: Optional[libgpiod.gpiod_chip] = None) -> None:
         self._chip_struct = chip_struct
 
     def get(self) -> Optional[libgpiod.gpiod_chip]:
         return self._chip_struct
 
     def __del__(self) -> None:
         if self._chip_struct is not None:
@@ -110,17 +108,15 @@
         """
         @brief Destructor
 
         Usage:
             del chip
         """
 
-    def open(
-        self, device: Union[int, str], how: int = _CHIP_OPEN_LOOKUP
-    ) -> None:
+    def open(self, device: Union[int, str], how: int = _CHIP_OPEN_LOOKUP) -> None:
         """
         @brief Open a GPIO chip.
 
         @param device: String or int describing the GPIO chip.
         @param how:    Indicates how the chip should be opened.
 
         If the object already holds a reference to an open chip, it will be
@@ -135,15 +131,15 @@
 
         chip_struct = func(device)
         if chip_struct is None:
             errno = get_errno()
             raise OSError(
                 errno,
                 strerror(errno),
-                "cannot open GPIO device {}".format(device),
+                f"cannot open GPIO device {device}",
             )
 
         self._m_chip = shared_chip(chip_struct)
 
     def reset(self) -> None:
         """
         @brief Reset the internal smart pointer owned by this object.
@@ -200,44 +196,36 @@
 
         Usage:
             l = chip.get_line(0)
         """
         if offset >= self.num_lines or offset < 0:
             raise IndexError("line offset out of range")
 
-        line_struct = libgpiod.gpiod_chip_get_line(
-            self._throw_if_noref_and_get_m_chip(), offset
-        )
+        line_struct = libgpiod.gpiod_chip_get_line(self._throw_if_noref_and_get_m_chip(), offset)
         if line_struct is None:
             errno = get_errno()
-            raise OSError(
-                errno, strerror(errno), "error getting GPIO line from chip"
-            )
+            raise OSError(errno, strerror(errno), "error getting GPIO line from chip")
 
         return line(line_struct, copy(self))
 
     def find_line(self, name: str) -> line:
         """
         @brief Get the line exposed by this chip by name.
 
         @param name: Line name.
 
         @return Line object.
 
         Usage:
             l = chip.find_line("PIN_0")
         """
-        line_struct = libgpiod.gpiod_chip_find_line(
-            self._throw_if_noref_and_get_m_chip(), name
-        )
+        line_struct = libgpiod.gpiod_chip_find_line(self._throw_if_noref_and_get_m_chip(), name)
         errno = get_errno()
         if line_struct is None and errno != ENOENT:
-            raise OSError(
-                errno, strerror(errno), "error looking up GPIO line by name"
-            )
+            raise OSError(errno, strerror(errno), "error looking up GPIO line by name")
 
         return line(line_struct, copy(self)) if bool(line_struct) else line()
 
     def get_lines(self, offsets: List[int]) -> line_bulk:
         """
         @brief Get a set of lines exposed by this chip at given offsets.
 
@@ -465,16 +453,15 @@
         @return Current direction setting.
 
         Usage:
             print(line.direction == line.DIRECTION_INPUT)
         """
         return (
             self.DIRECTION_INPUT
-            if self._throw_if_null_and_get_m_line().direction
-            == libgpiod.GPIOD_LINE_DIRECTION_INPUT
+            if self._throw_if_null_and_get_m_line().direction == libgpiod.GPIOD_LINE_DIRECTION_INPUT
             else self.DIRECTION_OUTPUT
         )
 
     @property
     def active_state(self) -> int:
         """
         @brief Get current active state of this line.
@@ -497,17 +484,15 @@
         @brief Get current bias of this line.
 
         @return Current bias setting.
 
         Usage:
             print(line.bias == line.BIAS_PULL_UP)
         """
-        return bias_mapping[
-            libgpiod.gpiod_line_bias(self._throw_if_null_and_get_m_line())
-        ]
+        return bias_mapping[libgpiod.gpiod_line_bias(self._throw_if_null_and_get_m_line())]
 
     def is_used(self) -> bool:
         """
         @brief Check if this line is used by the kernel or other user space
                process.
 
         @return True if this line is in use, false otherwise.
@@ -522,30 +507,26 @@
         @brief Check if this line represents an open-drain GPIO.
 
         @return True if the line is an open-drain GPIO, false otherwise.
 
         Usage:
             print(line.is_open_drain())
         """
-        return libgpiod.gpiod_line_is_open_drain(
-            self._throw_if_null_and_get_m_line()
-        )
+        return libgpiod.gpiod_line_is_open_drain(self._throw_if_null_and_get_m_line())
 
     def is_open_source(self) -> bool:
         """
         @brief Check if this line represents an open-source GPIO.
 
         @return True if the line is an open-source GPIO, false otherwise.
 
         Usage:
             print(line.is_open_source())
         """
-        return libgpiod.gpiod_line_is_open_source(
-            self._throw_if_null_and_get_m_line()
-        )
+        return libgpiod.gpiod_line_is_open_source(self._throw_if_null_and_get_m_line())
 
     def request(self, config: line_request, default_val: int = 0) -> None:
         """
         @brief Request this line.
 
         @param config:      Request config (see gpiod.line_request).
         @param default_val: Default value - only matters for OUTPUT direction.
@@ -588,53 +569,45 @@
         @brief Check if this user has ownership of this line.
 
         @return True if the user has ownership of this line, false otherwise.
 
         Usage:
             print(line.is_requested())
         """
-        return libgpiod.gpiod_line_is_requested(
-            self._throw_if_null_and_get_m_line()
-        )
+        return libgpiod.gpiod_line_is_requested(self._throw_if_null_and_get_m_line())
 
     def get_value(self) -> int:
         """
         @brief Read the line value.
 
         @return Current value (0 or 1).
 
         Usage:
             val = line.get_value()
         """
         rv = libgpiod.gpiod_line_get_value(self._throw_if_null_and_get_m_line())
         if rv == -1:
             errno = get_errno()
-            raise OSError(
-                errno, strerror(errno), "error reading GPIO line value"
-            )
+            raise OSError(errno, strerror(errno), "error reading GPIO line value")
 
         return rv
 
     def set_value(self, val: int) -> None:
         """
         @brief Set the value of this line.
 
         @param val: New value (0 or 1).
 
         Usage:
             line.set_value(1)
         """
-        rv = libgpiod.gpiod_line_set_value(
-            self._throw_if_null_and_get_m_line(), val
-        )
+        rv = libgpiod.gpiod_line_set_value(self._throw_if_null_and_get_m_line(), val)
         if rv:
             errno = get_errno()
-            raise OSError(
-                errno, strerror(errno), "error setting GPIO line value"
-            )
+            raise OSError(errno, strerror(errno), "error setting GPIO line value")
 
     def set_config(self, direction: int, flags: int, value: int = 0) -> None:
         """
         @brief Set configuration of this line.
 
         @param direction: New direction.
         @param flags:     Replacement flags.
@@ -692,17 +665,15 @@
 
         Usage:
             if line.event_wait(timedelta(seconds=10)):
                 print("An event occurred")
             else:
                 print("Timeout")
         """
-        rv = libgpiod.gpiod_line_event_wait(
-            self._throw_if_null_and_get_m_line(), timeout
-        )
+        rv = libgpiod.gpiod_line_event_wait(self._throw_if_null_and_get_m_line(), timeout)
         if rv < 0:
             errno = get_errno()
             raise OSError(errno, strerror(errno), "error polling for events")
 
         return bool(rv)
 
     def event_read(self) -> line_event:
@@ -745,17 +716,15 @@
         @brief Get the event file descriptor associated with this line.
 
         @return File descriptor number
 
         Usage:
             fd = line.event_get_fd()
         """
-        ret = libgpiod.gpiod_line_event_get_fd(
-            self._throw_if_null_and_get_m_line()
-        )
+        ret = libgpiod.gpiod_line_event_get_fd(self._throw_if_null_and_get_m_line())
 
         if ret < 0:
             errno = get_errno()
             raise OSError(
                 errno,
                 strerror(errno),
                 "unable to get the line event file descriptor",
@@ -781,17 +750,15 @@
         Usage:
             line.update()
         """
         ret = libgpiod.gpiod_line_update(self._throw_if_null_and_get_m_line())
 
         if ret < 0:
             errno = get_errno()
-            raise OSError(
-                errno, strerror(errno), "unable to update the line info"
-            )
+            raise OSError(errno, strerror(errno), "unable to update the line info")
 
     def reset(self) -> None:
         """
         @brief Reset the state of this object.
 
         This is useful when the user needs to e.g. keep the line_event object
         but wants to drop the reference to the GPIO chip indirectly held by
@@ -913,21 +880,16 @@
         """
         if not new_line:
             raise ValueError("line_bulk cannot hold empty line objects")
 
         if len(self._m_bulk) >= self.MAX_LINES:
             raise IndexError("maximum number of lines reached")
 
-        if (
-            len(self._m_bulk) >= 1
-            and self._m_bulk[0].get_chip() != new_line.get_chip()
-        ):
-            raise ValueError(
-                "line_bulk cannot hold GPIO lines from different chips"
-            )
+        if len(self._m_bulk) >= 1 and self._m_bulk[0].get_chip() != new_line.get_chip():
+            raise ValueError("line_bulk cannot hold GPIO lines from different chips")
 
         self._m_bulk.append(new_line)
 
     def get(self, offset: int) -> line:
         """
         @brief Get the line at given offset.
 
@@ -993,17 +955,15 @@
         @brief Remove all lines from this object.
 
         Usage:
             bulk.clear()
         """
         self._m_bulk.clear()
 
-    def request(
-        self, config: line_request, default_vals: Optional[List[int]] = None
-    ) -> None:
+    def request(self, config: line_request, default_vals: Optional[List[int]] = None) -> None:
         """
         @brief Request all lines held by this object.
 
         @param config:       Request config (see gpiod::line_request).
         @param default_vals: List of default values. Only relevant for output
                              direction requests.
 
@@ -1017,18 +977,15 @@
         """
         self._throw_if_empty()
 
         if default_vals is None:
             default_vals = [0] * self.size
 
         if self.size != len(default_vals):
-            raise ValueError(
-                "the number of default values must correspond "
-                "to the number of lines"
-            )
+            raise ValueError("the number of default values must correspond to the number of lines")
 
         try:
             for i in range(self.size):
                 self._m_bulk[i].request(config, default_vals[i])
         except OSError as error:
             self.release()
             raise error
@@ -1072,61 +1029,49 @@
 
         Usage:
             bulk.set)_blaues([1] * bulk.size)
         """
         self._throw_if_empty()
 
         if self.size != len(values):
-            raise ValueError(
-                "the size of values array must correspond to "
-                "the number of lines"
-            )
+            raise ValueError("the size of values array must correspond to the number of lines")
 
         for i in range(self.size):
             self._m_bulk[i].set_value(values[i])
 
-    def set_config(
-        self, direction: int, flags: int, values: Optional[List[int]] = None
-    ) -> None:
+    def set_config(self, direction: int, flags: int, values: Optional[List[int]] = None) -> None:
         """
         @brief Set configuration of all lines held by this object.
 
         @param direction: New direction.
         @param flags:     Replacement flags.
 
         @param List of values to set. Must be the same size as the number of
                lines held by this line_bulk.
                Only relevant for output direction requests.
         """
         self._throw_if_empty()
 
         if values is not None and self.size != len(values):
-            raise ValueError(
-                "the size of values array must correspond to "
-                "the number of lines"
-            )
+            raise ValueError("the size of values array must correspond to the number of lines")
 
         gflags = 0
 
         for first, second in reqflag_mapping.items():
             if first & flags:
                 gflags |= second
 
         bulk = libgpiod.gpiod_line_bulk()
 
         self._to_line_bulk(bulk)
 
-        rv = libgpiod.gpiod_line_set_config_bulk(
-            bulk, direction, gflags, values
-        )
+        rv = libgpiod.gpiod_line_set_config_bulk(bulk, direction, gflags, values)
         if rv < 0:
             errno = get_errno()
-            raise OSError(
-                errno, strerror(errno), "error setting GPIO line config"
-            )
+            raise OSError(errno, strerror(errno), "error setting GPIO line config")
 
     def set_flags(self, flags: int) -> None:
         """
         @brief Set configuration flags of all lines held by this object.
 
         @param flags: Replacement flags.
         """
@@ -1141,17 +1086,15 @@
         for first, second in reqflag_mapping.items():
             if first & flags:
                 gflags |= second
 
         rv = libgpiod.gpiod_line_set_flags_bulk(bulk, gflags)
         if rv < 0:
             errno = get_errno()
-            raise OSError(
-                errno, strerror(errno), "error setting GPIO line flags"
-            )
+            raise OSError(errno, strerror(errno), "error setting GPIO line flags")
 
     def set_direction_input(self) -> None:
         """
         @brief Change the direction all lines held by this object to input.
         """
         self._throw_if_empty()
 
@@ -1174,18 +1117,15 @@
 
         @param values: Vector of values to set. Must be the same size as the
                        number of lines held by this line_bulk.
         """
         self._throw_if_empty()
 
         if values is not None and self.size != len(values):
-            raise ValueError(
-                "the size of values array must correspond to "
-                "the number of lines"
-            )
+            raise ValueError("the size of values array must correspond to the number of lines")
 
         bulk = libgpiod.gpiod_line_bulk()
 
         self._to_line_bulk(bulk)
 
         rv = libgpiod.gpiod_line_set_direction_output_bulk(bulk, values)
         if rv < 0:
@@ -1281,17 +1221,15 @@
     def __init__(self) -> None:
         self._iter = None
 
     def __iter__(self: CI) -> CI:
         self._iter = libgpiod.gpiod_chip_iter().__iter__()
         if self._iter is None:
             errno = get_errno()
-            raise OSError(
-                errno, strerror(errno), "error creating GPIO chip iterator"
-            )
+            raise OSError(errno, strerror(errno), "error creating GPIO chip iterator")
 
         return self
 
     def __next__(self) -> chip:
         _next = self._iter.next_noclose()
         return chip(chip_shared=shared_chip(_next))
 
@@ -1315,17 +1253,15 @@
 
         self._iter = None
 
     def __iter__(self: LI) -> LI:
         self._iter = iter(libgpiod.gpiod_line_iter(self._chip._m_chip.get()))
         if self._iter is None:
             errno = get_errno()
-            raise OSError(
-                errno, strerror(errno), "error creating GPIO line iterator"
-            )
+            raise OSError(errno, strerror(errno), "error creating GPIO line iterator")
 
         return self
 
     def __next__(self) -> line:
         if self._iter is not None:
             return line(next(self._iter), self._chip)
```

### Comparing `gpiod-1.5.3/py_src/gpiod/test/__init__.py` & `gpiod-1.5.4/py_src/gpiod/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gpiod-1.5.3/py_src/gpiod/test/blink.py` & `gpiod-1.5.4/py_src/gpiod/test/blink.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=missing-docstring
 import sys
 import time
+
 from .. import chip, line, line_request
 
 try:
     if len(sys.argv) > 2:
         LED_CHIP = sys.argv[1]
         LED_LINE_OFFSET = int(sys.argv[2])
     else:
```

### Comparing `gpiod-1.5.3/py_src/gpiod/test/bulk_blink.py` & `gpiod-1.5.4/py_src/gpiod/test/bulk_blink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=missing-docstring
 import sys
 import time
+
 from .. import chip, line_request
 
 try:
     if len(sys.argv) > 2:
         LED_CHIP = sys.argv[1]
         LED_LINE_OFFSETS = []
         for i in range(len(sys.argv) - 2):
```

### Comparing `gpiod-1.5.3/py_src/gpiod/test/bulk_button.py` & `gpiod-1.5.4/py_src/gpiod/test/bulk_button.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=missing-docstring
 import sys
 from datetime import timedelta
-from .. import chip, line_request, line_event
+
+from .. import chip, line_event, line_request
 
 try:
     if len(sys.argv) > 3:
         BUTTON_CHIP = sys.argv[1]
         BUTTON_LINE_OFFSETS = []
         for i in range(len(sys.argv) - 3):
             BUTTON_LINE_OFFSETS.append(int(sys.argv[i + 2]))
@@ -31,15 +32,15 @@
 c = chip(BUTTON_CHIP)
 buttons = c.get_lines(BUTTON_LINE_OFFSETS)
 
 config = line_request()
 config.request_type = BUTTON_EDGE
 
 for i in range(buttons.size):
-    config.consumer = "Button {}".format(i)
+    config.consumer = f"Button {i}"
     buttons[i].request(config)
 
 
 while True:
     lines = buttons.event_wait(timedelta(seconds=10))
     if not lines.empty:
         for it in lines:
```

### Comparing `gpiod-1.5.3/py_src/gpiod/test/button.py` & `gpiod-1.5.4/py_src/gpiod/test/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=missing-docstring
 import sys
 from datetime import timedelta
-from .. import chip, line_request, line_event
+
+from .. import chip, line_event, line_request
 
 try:
     if len(sys.argv) > 2:
         BUTTON_CHIP = sys.argv[1]
         BUTTON_LINE_OFFSET = int(sys.argv[2])
         if len(sys.argv) > 3:
             edge = sys.argv[3]
```

### Comparing `gpiod-1.5.3/py_src/gpiod/test/sequential_blink.py` & `gpiod-1.5.4/py_src/gpiod/test/sequential_blink.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=missing-docstring
 import sys
 import time
+
 from .. import chip, line_request
 
 try:
     if len(sys.argv) > 2:
         LED_CHIP = sys.argv[1]
         LED_LINE_OFFSETS = []
         for i in range(len(sys.argv) - 2):
@@ -23,15 +24,15 @@
 c = chip(LED_CHIP)
 leds = c.get_lines(LED_LINE_OFFSETS)
 
 config = line_request()
 config.request_type = line_request.DIRECTION_OUTPUT
 
 for i in range(leds.size):
-    config.consumer = "Blink{}".format(i)
+    config.consumer = f"Blink {i}"
     leds.get(i).request(config)
     print("line: ", leds[i].offset, ", consumer: ", leds[i].consumer)
 
 while True:
     for led in leds:
         led.set_value(1)
         time.sleep(0.2)
```

### Comparing `gpiod-1.5.3/py_src/gpiod.egg-info/PKG-INFO` & `gpiod-1.5.4/py_src/gpiod.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: gpiod
-Version: 1.5.3
-Summary: UNKNOWN
+Version: 1.5.4
 Home-page: https://github.com/hhk7734/python3-gpiod
 Author: Hyeonki Hong
 Author-email: hhk7734@gmail.com
 License: MIT
 Project-URL: Documentation, https://wiki.loliot.net/docs/lang/python/libraries/gpiod/python-gpiod-about
 Project-URL: "Source Code", https://github.com/hhk7734/python3-gpiod
 Keywords: GPIO,gpiod
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Hardware
 Description-Content-Type: text/markdown
@@ -37,14 +35,20 @@
 python3 -m pip install -U --user pip gpiod
 ```
 
 ## Changelog
 
 Ref: CHANGELOG
 
+## 1.5.4
+
+- chore: change max-line-length and run black and isort by @hhk7734 in #36
+- Fixed issue when gpio chip has no label by @yacinbm in #35
+- Also build a py3-none-any wheel by @rmelick-muon in #33
+
 ## 1.5.3
 
 - libgpiod: update typing for return values #27
 - libgpiod: update typing for return values #27
 
 ## 1.5.2
 
@@ -239,9 +243,7 @@
  -- Hyeonki Hong <hhk7734@gmail.com>  Wed, 11 Mar 2020 13:28:45 +0900
 
 python3-gpiod (0.1.0) unstable; urgency=medium
 
   * Add initial setup files
 
  -- Hyeonki Hong <hhk7734@gmail.com>  Tue, 10 Mar 2020 15:40:13 +0900
-
-
```

### Comparing `gpiod-1.5.3/py_src/gpiod.egg-info/SOURCES.txt` & `gpiod-1.5.4/py_src/gpiod.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGELOG
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 py_src/gpiod/__init__.py
 py_src/gpiod/py.typed
 py_src/gpiod.egg-info/PKG-INFO
 py_src/gpiod.egg-info/SOURCES.txt
 py_src/gpiod.egg-info/dependency_links.txt
```

### Comparing `gpiod-1.5.3/setup.cfg` & `gpiod-1.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `gpiod-1.5.3/setup.py` & `gpiod-1.5.4/setup.py`

 * *Files identical despite different names*

