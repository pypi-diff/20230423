# Comparing `tmp/roadmapper-1.1.1.tar.gz` & `tmp/roadmapper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadmapper-1.1.1.tar", last modified: Sat Apr  1 20:06:03 2023, max compression
+gzip compressed data, was "roadmapper-1.2.0.tar", last modified: Sun Apr 23 20:33:22 2023, max compression
```

## Comparing `roadmapper-1.1.1.tar` & `roadmapper-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 20:06:03.745434 roadmapper-1.1.1/
--rw-rw-rw-   0        0        0     1092 2023-01-07 22:57:29.000000 roadmapper-1.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     4460 2023-04-01 20:06:03.744434 roadmapper-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3904 2023-04-01 20:04:15.000000 roadmapper-1.1.1/README.md
--rw-rw-rw-   0        0        0     1088 2023-01-31 06:22:36.000000 roadmapper-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-01 20:06:03.745434 roadmapper-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-01 20:06:03.708190 roadmapper-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-01 20:06:03.728703 roadmapper-1.1.1/src/roadmapper/
--rw-rw-rw-   0        0        0        0 2023-01-07 22:57:29.000000 roadmapper-1.1.1/src/roadmapper/__init__.py
--rw-rw-rw-   0        0        0    17090 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/colourtheme.py
--rw-rw-rw-   0        0        0     2896 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/footer.py
--rw-rw-rw-   0        0        0     6650 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/group.py
--rw-rw-rw-   0        0        0     4415 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/logo.py
--rw-rw-rw-   0        0        0     5307 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/marker.py
--rw-rw-rw-   0        0        0     3465 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/milestone.py
--rw-rw-rw-   0        0        0    18885 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/painter.py
--rw-rw-rw-   0        0        0    21156 2023-04-01 20:04:15.000000 roadmapper-1.1.1/src/roadmapper/roadmap.py
--rw-rw-rw-   0        0        0     2775 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/subtitle.py
--rw-rw-rw-   0        0        0    21403 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/task.py
--rw-rw-rw-   0        0        0    22091 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/timeline.py
--rw-rw-rw-   0        0        0    13465 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/timelineitem.py
--rw-rw-rw-   0        0        0     3988 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/timelineitemyear.py
--rw-rw-rw-   0        0        0     4653 2023-04-01 20:04:15.000000 roadmapper-1.1.1/src/roadmapper/timelinelocale.py
--rw-rw-rw-   0        0        0     1335 2023-01-07 22:57:29.000000 roadmapper-1.1.1/src/roadmapper/timelinemode.py
--rw-rw-rw-   0        0        0     2986 2023-01-31 06:18:56.000000 roadmapper-1.1.1/src/roadmapper/title.py
--rw-rw-rw-   0        0        0       24 2023-04-01 20:05:20.000000 roadmapper-1.1.1/src/roadmapper/version.py
-drwxrwxrwx   0        0        0        0 2023-04-01 20:06:03.743433 roadmapper-1.1.1/src/roadmapper.egg-info/
--rw-rw-rw-   0        0        0     4460 2023-04-01 20:06:03.000000 roadmapper-1.1.1/src/roadmapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-04-01 20:06:03.000000 roadmapper-1.1.1/src/roadmapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 20:06:03.000000 roadmapper-1.1.1/src/roadmapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-01 20:06:03.000000 roadmapper-1.1.1/src/roadmapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-01 20:06:03.000000 roadmapper-1.1.1/src/roadmapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.247319 roadmapper-1.2.0/
+-rw-rw-rw-   0        0        0     1092 2023-01-07 22:57:29.000000 roadmapper-1.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0     4333 2023-04-23 20:33:22.247319 roadmapper-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3777 2023-04-23 20:25:06.000000 roadmapper-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1088 2023-01-31 06:22:36.000000 roadmapper-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 20:33:22.247319 roadmapper-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.215883 roadmapper-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.233887 roadmapper-1.2.0/src/roadmapper/
+-rw-rw-rw-   0        0        0        0 2023-01-07 22:57:29.000000 roadmapper-1.2.0/src/roadmapper/__init__.py
+-rw-rw-rw-   0        0        0    17086 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/roadmapper/colourtheme.py
+-rw-rw-rw-   0        0        0     2888 2023-04-23 20:31:54.000000 roadmapper-1.2.0/src/roadmapper/footer.py
+-rw-rw-rw-   0        0        0     6811 2023-04-23 20:32:10.000000 roadmapper-1.2.0/src/roadmapper/group.py
+-rw-rw-rw-   0        0        0     4376 2023-04-23 20:32:17.000000 roadmapper-1.2.0/src/roadmapper/logo.py
+-rw-rw-rw-   0        0        0     5253 2023-04-23 20:32:21.000000 roadmapper-1.2.0/src/roadmapper/marker.py
+-rw-rw-rw-   0        0        0     3415 2023-04-23 20:32:23.000000 roadmapper-1.2.0/src/roadmapper/milestone.py
+-rw-rw-rw-   0        0        0    19946 2023-04-23 20:32:26.000000 roadmapper-1.2.0/src/roadmapper/painter.py
+-rw-rw-rw-   0        0        0    17902 2023-04-23 20:32:32.000000 roadmapper-1.2.0/src/roadmapper/roadmap.py
+-rw-rw-rw-   0        0        0     2767 2023-04-23 20:32:35.000000 roadmapper-1.2.0/src/roadmapper/subtitle.py
+-rw-rw-rw-   0        0        0    21541 2023-04-23 20:32:38.000000 roadmapper-1.2.0/src/roadmapper/task.py
+-rw-rw-rw-   0        0        0    22043 2023-04-23 20:32:42.000000 roadmapper-1.2.0/src/roadmapper/timeline.py
+-rw-rw-rw-   0        0        0    13397 2023-04-23 20:32:46.000000 roadmapper-1.2.0/src/roadmapper/timelineitem.py
+-rw-rw-rw-   0        0        0     3846 2023-04-23 20:32:50.000000 roadmapper-1.2.0/src/roadmapper/timelineitemyear.py
+-rw-rw-rw-   0        0        0     4655 2023-04-09 00:51:50.000000 roadmapper-1.2.0/src/roadmapper/timelinelocale.py
+-rw-rw-rw-   0        0        0     1330 2023-04-09 00:51:50.000000 roadmapper-1.2.0/src/roadmapper/timelinemode.py
+-rw-rw-rw-   0        0        0     2978 2023-04-23 20:33:00.000000 roadmapper-1.2.0/src/roadmapper/title.py
+-rw-rw-rw-   0        0        0       24 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/roadmapper/version.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.241888 roadmapper-1.2.0/src/roadmapper.egg-info/
+-rw-rw-rw-   0        0        0     4333 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-23 20:33:22.000000 roadmapper-1.2.0/src/roadmapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 20:33:22.245889 roadmapper-1.2.0/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 00:51:50.000000 roadmapper-1.2.0/src/tests/__init__.py
+-rw-rw-rw-   0        0        0      925 2023-04-09 00:51:50.000000 roadmapper-1.2.0/src/tests/roadmap_draw_test.py
+-rw-rw-rw-   0        0        0    42793 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/tests/test_cases.py
+-rw-rw-rw-   0        0        0     3044 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/tests/test_painter.py
+-rw-rw-rw-   0        0        0    13294 2023-04-23 20:15:33.000000 roadmapper-1.2.0/src/tests/test_roadmapper.py
```

### Comparing `roadmapper-1.1.1/LICENSE.md` & `roadmapper-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roadmapper-1.1.1/PKG-INFO` & `roadmapper-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadmapper
-Version: 1.1.1
+Version: 1.2.0
 Summary: Roadmapper. A Roadmap-as-Code (RaC) python library for generating a roadmap by using python code
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/roadmapper
 Project-URL: Bug Tracker, https://github.com/csgoh/roadmapper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,47 +18,39 @@
 ![release](https://img.shields.io/pypi/v/roadmapper)
 ![Wheel](https://img.shields.io/pypi/wheel/roadmapper?style=plastic)
 ![download count](https://img.shields.io/pypi/dm/roadmapper?style=plastic)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/roadmapper?style=plastic)
 ![commit count](https://img.shields.io/github/commit-activity/m/csgoh/roadmapper?style=plastic)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/roadmapper/badge)](https://www.codefactor.io/repository/github/csgoh/roadmapper)
 ![python version](https://img.shields.io/pypi/pyversions/roadmapper?style=plastic)
+![CI](https://github.com/csgoh/roadmapper/actions/workflows/ci.yaml/badge.svg)
 
 # Roadmaper - a Roadmap as Code (RaC) Tool
 
 ## Purpose
 The purpose of roadmapper python library is used to draw roadmap by using python code. This is the first Roadmap as Code (RaC) library. RaC helps to create and edit roadmap in a more efficient way without having to use any graphical tools that are not always easy to use to create or update a roadmap.
 
 With git repository like GitHub or Bitbucket, roadmaps created using RaC can be version controlled, track changes and can be easily shared with others.
 
 ### Latest version
 ![release](https://img.shields.io/pypi/v/roadmapper)
 
 :book: For usage documentation, how-to guide and code examples, refer to [Roadmapper Wiki](https://github.com/csgoh/roadmap-generator/wiki).
 
-### What's new in the latest version of Roadmapper?
-* Unicode, multilingual support
-* Ability to change timeline locale and labels
-* Ability to add your own custom colour scheme
+View the [Change Logs](https://github.com/csgoh/processpiper/wiki/Change-Logs) to find out the latest updates and additions in the most recent version.
 
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
 * Pillow 9.4.0
 * python-dateutil
 
-## Future plans :bulb:
-* Create roadmap with plain english text like PlantUML
-* GUI and Web frontend for this roadmapper library
-* Visual Studio Code extension to create and edit roadmap
-<br/>
-
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
 ## Installation
 ### Install from PyPI
@@ -84,15 +76,15 @@
 ```python 
 from roadmapper.roadmap import Roadmap
 from roadmapper.timelinemode import TimelineMode
 
 roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
 roadmap.set_title("My Demo Roadmap")
 roadmap.set_subtitle("Matariki Technologies Ltd")
-roadmap.set_timeline(TimelineMode.MONTHLY, "2023-01-01", 12)
+roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=12)
 roadmap.add_logo("matariki-tech-logo.png", "top-right", 50, 50)
 
 group = roadmap.add_group("Core Product Work Stream")
 
 task = group.add_task("Base Functionality", "2023-01-01", "2023-10-31")
 task.add_milestone("v.1.0", "2023-02-15")
 task.add_milestone("v.1.1", "2023-08-01")
```

### Comparing `roadmapper-1.1.1/README.md` & `roadmapper-1.2.0/src/roadmapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,56 @@
+Metadata-Version: 2.1
+Name: roadmapper
+Version: 1.2.0
+Summary: Roadmapper. A Roadmap-as-Code (RaC) python library for generating a roadmap by using python code
+Author: CS Goh
+Project-URL: Homepage, https://github.com/csgoh/roadmapper
+Project-URL: Bug Tracker, https://github.com/csgoh/roadmapper/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 ![Banner](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner.png?raw=true)
 
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 ![release](https://img.shields.io/pypi/v/roadmapper)
 ![Wheel](https://img.shields.io/pypi/wheel/roadmapper?style=plastic)
 ![download count](https://img.shields.io/pypi/dm/roadmapper?style=plastic)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/roadmapper?style=plastic)
 ![commit count](https://img.shields.io/github/commit-activity/m/csgoh/roadmapper?style=plastic)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/roadmapper/badge)](https://www.codefactor.io/repository/github/csgoh/roadmapper)
 ![python version](https://img.shields.io/pypi/pyversions/roadmapper?style=plastic)
+![CI](https://github.com/csgoh/roadmapper/actions/workflows/ci.yaml/badge.svg)
 
 # Roadmaper - a Roadmap as Code (RaC) Tool
 
 ## Purpose
 The purpose of roadmapper python library is used to draw roadmap by using python code. This is the first Roadmap as Code (RaC) library. RaC helps to create and edit roadmap in a more efficient way without having to use any graphical tools that are not always easy to use to create or update a roadmap.
 
 With git repository like GitHub or Bitbucket, roadmaps created using RaC can be version controlled, track changes and can be easily shared with others.
 
 ### Latest version
 ![release](https://img.shields.io/pypi/v/roadmapper)
 
 :book: For usage documentation, how-to guide and code examples, refer to [Roadmapper Wiki](https://github.com/csgoh/roadmap-generator/wiki).
 
-### What's new in the latest version of Roadmapper?
-* Unicode, multilingual support
-* Ability to change timeline locale and labels
-* Ability to add your own custom colour scheme
+View the [Change Logs](https://github.com/csgoh/processpiper/wiki/Change-Logs) to find out the latest updates and additions in the most recent version.
 
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
 * Pillow 9.4.0
 * python-dateutil
 
-## Future plans :bulb:
-* Create roadmap with plain english text like PlantUML
-* GUI and Web frontend for this roadmapper library
-* Visual Studio Code extension to create and edit roadmap
-<br/>
-
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
 ## Installation
 ### Install from PyPI
@@ -70,15 +76,15 @@
 ```python 
 from roadmapper.roadmap import Roadmap
 from roadmapper.timelinemode import TimelineMode
 
 roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
 roadmap.set_title("My Demo Roadmap")
 roadmap.set_subtitle("Matariki Technologies Ltd")
-roadmap.set_timeline(TimelineMode.MONTHLY, "2023-01-01", 12)
+roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=12)
 roadmap.add_logo("matariki-tech-logo.png", "top-right", 50, 50)
 
 group = roadmap.add_group("Core Product Work Stream")
 
 task = group.add_task("Base Functionality", "2023-01-01", "2023-10-31")
 task.add_milestone("v.1.0", "2023-02-15")
 task.add_milestone("v.1.1", "2023-08-01")
```

### Comparing `roadmapper-1.1.1/pyproject.toml` & `roadmapper-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `roadmapper-1.1.1/src/roadmapper/colourtheme.py` & `roadmapper-1.2.0/src/roadmapper/colourtheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # "Segoe UI"
 # "Tahoma"
 # "Microsoft Jhenghei"
 # simhei.ttf
 # "ARIALUNI.TTF"
 # "arial.ttf"
 
-DEFAULT_FONT = "arial.ttf"
+DEFAULT_FONT = "Arial"
 DEFAULT_TITLE_FONT_SIZE = 26
 DEFAULT_SUBTITLE_FONT_SIZE = 18
 DEFAULT_TIMELINE_YEAR_FONT_SIZE = 12
 DEFAULT_TIMELINE_ITEM_FONT_SIZE = 12
 DEFAULT_MARKER_FONT_SIZE = 12
 DEFAULT_GROUP_FONT_SIZE = 12
 DEFAULT_TASK_FONT_SIZE = 12
```

### Comparing `roadmapper-1.1.1/src/roadmapper/footer.py` & `roadmapper-1.2.0/src/roadmapper/footer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 from dataclasses import dataclass, field
-from roadmapper.painter import Painter
+from .painter import Painter
 
 
 @dataclass(kw_only=True)
 class Footer:
     """Roadmap Footer class"""
 
     text: str = field(init=True, default=None)
```

### Comparing `roadmapper-1.1.1/src/roadmapper/group.py` & `roadmapper-1.2.0/src/roadmapper/group.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 from dataclasses import dataclass, field
-from contextlib import contextmanager
 from datetime import datetime
-from roadmapper.painter import Painter
-from roadmapper.timeline import Timeline
-from roadmapper.task import Task
-from roadmapper.milestone import Milestone
+from .painter import Painter
+from .timeline import Timeline
+from .task import Task
 
 
 @dataclass
 class Group:
     """Roadmap Group class"""
 
     text: str = field(init=True, default=None)
@@ -180,7 +179,15 @@
             self.font_size,
             self.font_colour,
         )
 
         # Step 2: draw tasks
         for tasks in self.tasks:
             tasks.draw(painter)
+
+    def __enter__(self):
+        """This method is called when the 'with' statement is used"""
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
+        """This method is called when the 'with' statement is used"""
+        pass
```

### Comparing `roadmapper-1.1.1/src/roadmapper/logo.py` & `roadmapper-1.2.0/src/roadmapper/logo.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from datetime import datetime
+
 from dataclasses import dataclass, field
-from roadmapper.painter import Painter
+from .painter import Painter
 
 
 @dataclass(kw_only=True)
 class Logo:
     """Logo class - used to show the logo on the roadmap"""
 
     image: str = field(init=True, default=None)
```

### Comparing `roadmapper-1.1.1/src/roadmapper/marker.py` & `roadmapper-1.2.0/src/roadmapper/marker.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 from datetime import datetime
 from dataclasses import dataclass, field
-from roadmapper.painter import Painter
-from roadmapper.timeline import Timeline
-from roadmapper.group import Group
+from .painter import Painter
+from .timeline import Timeline
 
 
 @dataclass(kw_only=True)
 class Marker:
     """A marker used to show the "Now" vertical line on the timeline"""
 
     font: str = field(init=True, default=None)
```

### Comparing `roadmapper-1.1.1/src/roadmapper/milestone.py` & `roadmapper-1.2.0/src/roadmapper/milestone.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 from datetime import datetime
 from dataclasses import dataclass, field
-from roadmapper.painter import Painter
-from roadmapper.timeline import Timeline
+from .painter import Painter
 
 
 @dataclass(kw_only=True)
 class Milestone:
     """Roadmap Milestone class"""
 
     text: str = field(init=True, default=None)
```

### Comparing `roadmapper-1.1.1/src/roadmapper/painter.py` & `roadmapper-1.2.0/src/roadmapper/painter.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# import cairo
-# from colour import Color
-from roadmapper.colourtheme import ColourTheme
+import os
+import sys
+from .colourtheme import ColourTheme
 from PIL import Image, ImageDraw, ImageFont, ImageColor
 import textwrap
 
 
 class Painter:
     """A wrapper class for Pillow library"""
 
@@ -179,14 +179,39 @@
         ) = self.colour_theme.get_colour_theme_settings("milestone")
         (
             self.footer_font,
             self.footer_font_size,
             self.footer_font_colour,
         ) = self.colour_theme.get_colour_theme_settings("footer")
 
+    def get_font_path(self, font_name: str) -> str:
+        """Get the path to the font file"""
+        # Check if font_name contained ttf or otf extension
+        if font_name.endswith(".ttf") or font_name.endswith(".otf"):
+            return font_name
+        # Check if font_name contained ttf or otf extension
+        if sys.platform.startswith("win"):  # Windows
+            return os.path.join("C:\\", "Windows", "Fonts", f"{font_name}.ttf")
+        elif sys.platform.startswith("darwin"):  # macOS
+            return os.path.join(
+                "/", "System", "Library", "Fonts", "Supplemental", f"{font_name}.ttf"
+            )
+        elif sys.platform.startswith("linux"):  # Linux
+            return os.path.join(
+                "/",
+                "usr",
+                "share",
+                "fonts",
+                "truetype",
+                "msttcorefonts",
+                f"{font_name}.ttf",
+            )
+        else:
+            raise Exception("Unsupported operating system")
+
     def draw_box(
         self, x: int, y: int, width: int, height: int, box_fill_colour: str
     ) -> None:
         """Draw a rectagle
 
         Args:
             x (int): X coordinate
@@ -255,15 +280,15 @@
         text: str,
         text_alignment: str,
         text_font: str,
         text_font_size: int,
         text_font_colour: str,
         style: str = "rectangle",
     ) -> None:
-        font = ImageFont.truetype(text_font, size=text_font_size)
+        font = ImageFont.truetype(self.get_font_path(text_font), size=text_font_size)
 
         multi_lines = []
         wrap_lines = []
 
         ### Make '\n' work
         multi_lines = text.splitlines()
 
@@ -363,15 +388,15 @@
             x (int): X coordinate
             y (int): Y coordinate
             text (str): Text to draw/display
         """
         self.__cr.text(
             (x, y),
             text,
-            font=ImageFont.truetype(font, font_size),
+            font=ImageFont.truetype(self.get_font_path(font), font_size),
             anchor="la",
             fill=(font_colour),
         )
 
     def set_line_style(self, style: str = "solid") -> None:
         """Set line style
 
@@ -492,15 +517,15 @@
             font (str): Font name
             font_size (int): Font size
 
         Returns:
             (text_width (int), text_height (int)): Text dimension (width, height)
         """
         # Use Pillow's ImageFont module to get the dimensions of the text.
-        image_font = ImageFont.truetype(font, font_size)
+        image_font = ImageFont.truetype(self.get_font_path(font), font_size)
 
         ascent, descent = image_font.getmetrics()
 
         left, _, right, bottom = image_font.getbbox(text)
         font_width = right
         font_height = bottom
```

### Comparing `roadmapper-1.1.1/src/roadmapper/roadmap.py` & `roadmapper-1.2.0/src/roadmapper/roadmap.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,62 +19,59 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from datetime import datetime
 from dataclasses import dataclass, field
 import time
-import importlib.metadata
 
-
-from roadmapper.painter import Painter
-from roadmapper.title import Title
-from roadmapper.subtitle import SubTitle
-from roadmapper.footer import Footer
-from roadmapper.timelinemode import TimelineMode
-from roadmapper.timeline import Timeline
-from roadmapper.group import Group
-from roadmapper.marker import Marker
-from roadmapper.logo import Logo
+from .painter import Painter
+from .title import Title
+from .subtitle import SubTitle
+from .footer import Footer
+from .timelinemode import TimelineMode
+from .timeline import Timeline
+from .group import Group
+from .marker import Marker
+from .logo import Logo
 
 
 @dataclass()
 class Roadmap:
     """The main Roadmap class"""
 
-    width: int = field(default=1200)
-    height: int = field(default=600)
-    auto_height: bool = field(default=True)
-    colour_theme: str = field(default="DEFAULT")
-    show_marker: bool = field(default=True)
-
-    title: Title = field(default=None, init=False)
-    subtitle: SubTitle = field(default=None, init=False)
-    timeline: Timeline = field(default=None, init=False)
-    groups: list[Group] = field(default_factory=list, init=False)
-    footer: Footer = field(default=None, init=False)
-    marker: Marker = field(default=None, init=False)
-    show_generic_dates: bool = field(default=False, init=False)
-
-    logo: Logo = field(default=None, init=False)
+    width: int = field(default=1200, init=True)
+    height: int = field(default=600, init=True)
+    auto_height: bool = field(default=True, init=True)
+    colour_theme: str = field(default="DEFAULT", init=True)
+    show_marker: bool = field(default=True, init=True)
+
+    _title: Title = field(default=None, init=False)
+    _subtitle: SubTitle = field(default=None, init=False)
+    _timeline: Timeline = field(default=None, init=False)
+    _groups: list[Group] = field(default_factory=list, init=False)
+    _footer: Footer = field(default=None, init=False)
+    _marker: Marker = field(default=None, init=False)
+    _show_generic_dates: bool = field(default=False, init=False)
+    _logo: Logo = field(default=None, init=False)
 
     def __post_init__(self):
         """This method is called after __init__() is called"""
         self.start_time = time.time()
-        self.__painter = Painter(self.width, self.height)
-        self.__set_colour_theme(self.colour_theme)
-        self.groups = []
+        self._painter = Painter(self.width, self.height)
+        self._set_colour_theme(self.colour_theme)
+        self._groups = []
         if self.show_marker == True:
-            self.__create_marker()
+            self._create_marker()
 
-    def __set_colour_theme(self, palette: str) -> None:
+    def _set_colour_theme(self, palette: str) -> None:
         """This method sets the colour palette"""
-        self.__painter.set_colour_theme(palette)
+        self._painter.set_colour_theme(palette)
 
-    def __create_marker(
+    def _create_marker(
         self,
         label_text_font: str = "",
         label_text_colour: str = "",
         label_text_size: int = 0,
         line_colour: str = "",
         line_width: int = 2,
         line_style: str = "dashed",
@@ -86,23 +83,23 @@
             label_text_colour (str, optional): Label text colour. Defaults to "Black".
             label_text_size (int, optional): Label text size. Defaults to 10.
             line_colour (str, optional): Line colour. Defaults to "Black".
             line_width (int, optional): Line width. Defaults to 2.
             line_style (str, optional): Line style. Defaults to "solid". Options are "solid", "dashed"
         """
         if label_text_font == "":
-            label_text_font = self.__painter.marker_font
+            label_text_font = self._painter.marker_font
         if label_text_size == 0:
-            label_text_size = self.__painter.marker_font_size
+            label_text_size = self._painter.marker_font_size
         if label_text_colour == "":
-            label_text_colour = self.__painter.marker_font_colour
+            label_text_colour = self._painter.marker_font_colour
         if line_colour == "":
-            line_colour = self.__painter.marker_line_colour
+            line_colour = self._painter.marker_line_colour
 
-        self.marker = Marker(
+        self._marker = Marker(
             font=label_text_font,
             font_size=label_text_size,
             font_colour=label_text_colour,
             line_colour=line_colour,
             line_width=line_width,
             line_style=line_style,
         )
@@ -123,24 +120,24 @@
             label_text_colour (str, optional): Label text colour. Defaults to "Black".
             label_text_size (int, optional): Label text size. Defaults to 10.
             line_colour (str, optional): Line colour. Defaults to "Black".
             line_width (int, optional): Line width. Defaults to 2.
             line_style (str, optional): Line style. Defaults to "solid". Options are "solid", "dashed"
         """
         if label_text_font == "":
-            label_text_font = self.__painter.marker_font
+            label_text_font = self._painter.marker_font
         if label_text_size == 0:
-            label_text_size = self.__painter.marker_font_size
+            label_text_size = self._painter.marker_font_size
         if label_text_colour == "":
-            label_text_colour = self.__painter.marker_font_colour
+            label_text_colour = self._painter.marker_font_colour
         if line_colour == "":
-            line_colour = self.__painter.marker_line_colour
+            line_colour = self._painter.marker_line_colour
 
-        self.marker.font = label_text_font
-        self.marker.font_size = label_text_size
+        self._marker.font = label_text_font
+        self._marker.font_size = label_text_size
         self.font_colour = label_text_colour
         self.line_colour = line_colour
         self.line_width = line_width
         self.line_style = line_style
 
     def set_title(
         self,
@@ -154,26 +151,26 @@
         Args:
             text (str): Title text
             font (str, optional): Title font. Defaults to "Arial".
             font_size (int, optional): Title font size. Defaults to 18.
             font_colour (str, optional): Title font colour. Defaults to "Black".
         """
         if font == "":
-            font = self.__painter.title_font
+            font = self._painter.title_font
         if font_size == 0:
-            font_size = self.__painter.title_font_size
+            font_size = self._painter.title_font_size
         if font_colour == "":
-            font_colour = self.__painter.title_font_colour
+            font_colour = self._painter.title_font_colour
 
-        self.title = Title(
+        self._title = Title(
             text=text, font=font, font_size=font_size, font_colour=font_colour
         )
-        self.title.text = text
+        self._title.text = text
 
-        self.title.set_draw_position(self.__painter)
+        self._title.set_draw_position(self._painter)
 
     def set_subtitle(
         self,
         text: str,
         font: str = "",
         font_size: int = 0,
         font_colour: str = "",
@@ -183,26 +180,26 @@
         Args:
             text (str): Title text
             font (str, optional): Title font. Defaults to "Arial".
             font_size (int, optional): Title font size. Defaults to 18.
             font_colour (str, optional): Title font colour. Defaults to "Black".
         """
         if font == "":
-            font = self.__painter.subtitle_font
+            font = self._painter.subtitle_font
         if font_size == 0:
-            font_size = self.__painter.subtitle_font_size
+            font_size = self._painter.subtitle_font_size
         if font_colour == "":
-            font_colour = self.__painter.subtitle_font_colour
+            font_colour = self._painter.subtitle_font_colour
 
-        self.subtitle = SubTitle(
+        self._subtitle = SubTitle(
             text=text, font=font, font_size=font_size, font_colour=font_colour
         )
-        self.subtitle.text = text
+        self._subtitle.text = text
 
-        self.subtitle.set_draw_position(self.__painter)
+        self._subtitle.set_draw_position(self._painter)
 
     def set_footer(
         self,
         text: str,
         font: str = "",
         font_size: int = 0,
         font_colour: str = "",
@@ -212,28 +209,29 @@
         Args:
             text (str): Footer text
             font (str, optional): Footer font. Defaults to "Arial".
             font_size (int, optional): Footer font size. Defaults to 18.
             font_colour (str, optional): Footer font colour. Defaults to "Black".
         """
         if font == "":
-            font = self.__painter.footer_font
+            font = self._painter.footer_font
         if font_size == 0:
-            font_size = self.__painter.footer_font_size
+            font_size = self._painter.footer_font_size
         if font_colour == "":
-            font_colour = self.__painter.footer_font_colour
+            font_colour = self._painter.footer_font_colour
 
-        self.footer = Footer(
+        self._footer = Footer(
             text=text, font=font, font_size=font_size, font_colour=font_colour
         )
-        self.footer.text = text
+        self._footer.text = text
 
     def set_timeline(
         self,
         mode: TimelineMode = TimelineMode.MONTHLY,
+        *,
         start: datetime = datetime.strptime(
             datetime.strftime(datetime.today(), "%Y-%m-%d"),
             "%Y-%m-%d",
         ),
         number_of_items: int = 12,
         show_generic_dates: bool = False,
         show_first_day_of_week: bool = False,
@@ -264,34 +262,34 @@
             fill_colour (str, optional): Timelinegroup fill colour. Defaults to "DEFAULT" colour theme.
             font (str, optional): Timeline font. Defaults to "DEFAULT" colour theme.
             font_size (int, optional): Timeline font size. Defaults to "DEFAULT" colour theme.
             font_colour (str, optional): Timeline font colour. Defaults to "DEFAULT" colour theme.
             fill_colour (str, optional): Timeline fill colour. Defaults to "DEFAULT" colour theme.
         """
         if year_font == "":
-            year_font = self.__painter.timeline_year_font
+            year_font = self._painter.timeline_year_font
         if year_font_size == 0:
-            year_font_size = self.__painter.timeline_year_font_size
+            year_font_size = self._painter.timeline_year_font_size
         if year_font_colour == "":
-            year_font_colour = self.__painter.timeline_year_font_colour
+            year_font_colour = self._painter.timeline_year_font_colour
         if year_fill_colour == "":
-            year_fill_colour = self.__painter.timeline_year_fill_colour
+            year_fill_colour = self._painter.timeline_year_fill_colour
 
         if item_font == "":
-            item_font = self.__painter.timeline_item_font
+            item_font = self._painter.timeline_item_font
         if item_font_size == 0:
-            item_font_size = self.__painter.timeline_item_font_size
+            item_font_size = self._painter.timeline_item_font_size
         if item_font_colour == "":
-            item_font_colour = self.__painter.timeline_item_font_colour
+            item_font_colour = self._painter.timeline_item_font_colour
         if item_fill_colour == "":
-            item_fill_colour = self.__painter.timeline_item_fill_colour
+            item_fill_colour = self._painter.timeline_item_fill_colour
 
-        self.show_generic_dates = show_generic_dates
+        self._show_generic_dates = show_generic_dates
         start_date = datetime.strptime(start, "%Y-%m-%d")
-        self.timeline = Timeline(
+        self._timeline = Timeline(
             mode=mode,
             start=start_date,
             locale_name=timeline_locale,
             number_of_items=number_of_items,
             show_generic_dates=show_generic_dates,
             show_first_day_of_week=show_first_day_of_week,
             year_font=year_font,
@@ -299,17 +297,17 @@
             year_font_colour=year_font_colour,
             year_fill_colour=year_fill_colour,
             item_font=item_font,
             item_font_size=item_font_size,
             item_font_colour=item_font_colour,
             item_fill_colour=item_fill_colour,
         )
-        self.timeline.set_draw_position(self.__painter)
-        if self.marker != None:
-            self.marker.set_label_draw_position(self.__painter, self.timeline)
+        self._timeline.set_draw_position(self._painter)
+        if self._marker != None:
+            self._marker.set_label_draw_position(self._painter, self._timeline)
 
     def add_logo(
         self,
         image: str,
         position: str = "top-right",
         width: int = 0,
         height: int = 0,
@@ -319,19 +317,19 @@
         Args:
             image (str): Image file path. See this page for supported image formats: https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html
             position (str): Position of the logo. Defaults to "top_right".
                             Options are top_left, top_centre, top_right, bottom_left, bottom_centre, bottom_right
             width (int, optional): Logo width. Defaults to image width.
             height (int, optional): Logo height. Defaults to image height.
         """
-        self.logo = Logo(image=image, position=position, width=width, height=height)
-        if self.logo != None:
+        self._logo = Logo(image=image, position=position, width=width, height=height)
+        if self._logo != None:
             ### If logo is positioned at top-centre, it x, y position has to be calculated first before Title.
-            if self.logo.position[:10] == "top-centre":
-                self.logo.set_draw_position(self.__painter, self.auto_height)
+            if self._logo.position[:10] == "top-centre":
+                self._logo.set_draw_position(self._painter, self.auto_height)
 
     def add_group(
         self,
         text: str,
         font: str = "",
         font_size: int = 0,
         font_colour: str = "",
@@ -348,153 +346,101 @@
             fill_colour (str, optional): Group fill colour. Defaults to "lightgrey".
             text_alignment (str, optional): Group text alignment. Defaults to "centre". Options are "left", "centre", "right"
 
         Return:
             Group: A new group instance. Use this to add taks to the group
         """
         if font == "":
-            font = self.__painter.group_font
+            font = self._painter.group_font
         if font_size == 0:
-            font_size = self.__painter.group_font_size
+            font_size = self._painter.group_font_size
         if font_colour == "":
-            font_colour = self.__painter.group_font_colour
+            font_colour = self._painter.group_font_colour
         if fill_colour == "":
-            fill_colour = self.__painter.group_fill_colour
+            fill_colour = self._painter.group_fill_colour
 
         group = Group(
             text=text,
             font=font,
             font_size=font_size,
             font_colour=font_colour,
             fill_colour=fill_colour,
             text_alignment=text_alignment,
-            painter=self.__painter,
+            painter=self._painter,
         )
-        self.groups.append(group)
+        self._groups.append(group)
         return group
 
     def draw(self) -> None:
         """Draw the roadmap"""
 
         ### Set the surface background colour
-        self.__painter.set_background_colour()
+        self._painter.set_background_colour()
 
         ### Draw the roadmap title
-        if self.title == None:
+        if self._title == None:
             raise ValueError("Title is not set. Please call set_title() to set title.")
-        self.title.draw(self.__painter)
+        self._title.draw(self._painter)
 
         ### Draw the roadmap subtitle
-        if self.subtitle != None:
-            self.subtitle.draw(self.__painter)
+        if self._subtitle != None:
+            self._subtitle.draw(self._painter)
 
         ### Draw the roadmap timeline
-        if self.timeline == None:
+        if self._timeline == None:
             raise ValueError(
                 "Timeline is not set. Please call set_timeline() to set timeline."
             )
-        self.timeline.draw(self.__painter)
+        self._timeline.draw(self._painter)
 
         ### Set the roadmap groups draw position
-        for group in self.groups:
-            group.set_draw_position(self.__painter, self.timeline)
+        for group in self._groups:
+            group.set_draw_position(self._painter, self._timeline)
 
         ### Draw timeline vertical lines on the roadmap
-        self.timeline.draw_vertical_lines(self.__painter)
+        self._timeline.draw_vertical_lines(self._painter)
 
         ### Draw the roadmap groups
-        for group in self.groups:
-            group.draw(self.__painter)
+        for group in self._groups:
+            group.draw(self._painter)
 
         ### Draw the roadmap marker
-        if self.marker != None and self.show_generic_dates == False:
-            self.marker.set_line_draw_position(self.__painter)
-            self.marker.draw(self.__painter)
+        if self._marker != None and self._show_generic_dates == False:
+            self._marker.set_line_draw_position(self._painter)
+            self._marker.draw(self._painter)
 
         ### Draw the roadmap footer
-        if self.footer != None:
-            self.footer.set_draw_position(self.__painter)
-            self.footer.draw(self.__painter)
+        if self._footer != None:
+            self._footer.set_draw_position(self._painter)
+            self._footer.draw(self._painter)
 
         ### Draw logo
 
-        if self.logo != None:
-            if self.logo.position[:10] != "top-centre":
-                self.logo.set_draw_position(self.__painter, self.auto_height)
-            self.logo.draw(self.__painter)
+        if self._logo != None:
+            if self._logo.position[:10] != "top-centre":
+                self._logo.set_draw_position(self._painter, self.auto_height)
+            self._logo.draw(self._painter)
 
         ### Auto adjust the surface height
         if self.auto_height == True:
-            self.__painter.set_surface_size(
-                self.__painter.width, int(self.__painter.next_y_pos)
+            self._painter.set_surface_size(
+                self._painter.width, int(self._painter.next_y_pos)
             )
 
     def save(self, filename: str) -> None:
         """Save surface to PNG file
 
         Args:
             filename (str): PNG file name
         """
-        self.__painter.save_surface(filename)
+        self._painter.save_surface(filename)
 
         elapsed_time = (time.time() - self.start_time) * 1000
         print(f"Took [{elapsed_time:.2f}ms] to generate '{filename}' roadmap")
 
-    def print_roadmap(self, print_area: str = "all") -> None:
-        """Print the content of the roadmap
-
-        Args:
-            print_area (str, optional): Roadmap area to print. Defaults to "all". Options are "all", "title", "timeline", "groups", "footer"
-        """
-        dash = "─"
-        space = " "
-        if print_area == "all" or print_area == "title":
-            print(f"Title={self.title.text}")
-
-        if print_area == "all" or print_area == "timeline":
-            print("Timeline:")
-            for timeline_item in self.timeline.timeline_items:
-                print(
-                    f"└{dash*8}{timeline_item.text}, value={timeline_item.value}, "
-                    f"box_x={round(timeline_item.box_x,2)}, box_y={timeline_item.box_y}, "
-                    f"box_w={round(timeline_item.box_width,2)}, box_h={timeline_item.box_height}, "
-                    f"text_x={round(timeline_item.text_x,2)}, text_y={timeline_item.text_y}"
-                )
-
-        if print_area == "all" or print_area == "groups":
-            for group in self.groups:
-                print(
-                    f"Group: text={group.text}, x={round(group.box_x, 2)}, y={group.box_y},",
-                    f"w={group.box_width}, h={group.box_height}",
-                )
-                for task in group.tasks:
-                    print(
-                        f"└{dash*8}{task.text}, start={task.start}, end={task.end}, "
-                        f"x={round(task.box_x, 2)}, y={task.box_y}, w={round(task.box_width, 2)}, "
-                        f"h={task.box_height}"
-                    )
-                    for milestone in task.milestones:
-                        print(
-                            f"{space*9}├{dash*4}{milestone.text}, date={milestone.date}, x={round(milestone.diamond_x, 2)}, "
-                            f"y={milestone.diamond_y}, w={milestone.diamond_width}, h={milestone.diamond_height}, "
-                            f"font_colour={milestone.font_colour}, fill_colour={milestone.fill_colour}"
-                        )
-                    for parellel_task in task.tasks:
-                        print(
-                            f"{space*9}└{dash*4}Parellel Task: {parellel_task.text}, start={parellel_task.start}, "
-                            f"end={parellel_task.end}, x={round(parellel_task.box_x,2)}, y={round(parellel_task.box_y, 2)}, "
-                            f"w={round(parellel_task.box_width, 2)}, h={round(parellel_task.box_height,2)}"
-                        )
-                        for parellel_task_milestone in parellel_task.milestones:
-                            print(
-                                f"{space*14}├{dash*4}{parellel_task_milestone.text}, "
-                                f"date={parellel_task_milestone.date}, x={round(parellel_task_milestone.diamond_x, 2)}, "
-                                f"y={round(parellel_task_milestone.diamond_y, 2)}, w={parellel_task_milestone.diamond_width}, "
-                                f"h={parellel_task_milestone.diamond_height}"
-                            )
-        if print_area == "all" or print_area == "footer":
-            if self.footer != None:
-                print(
-                    f"Footer: {self.footer.text} x={self.footer.x} "
-                    f"y={self.footer.y} w={self.footer.width} "
-                    f"h={self.footer.height}"
-                )
+    def __enter__(self):
+        """This method is called when the 'with' statement is used"""
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
+        """This method is called when the 'with' statement is used"""
+        pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `roadmapper-1.1.1/src/roadmapper/subtitle.py` & `roadmapper-1.2.0/src/roadmapper/subtitle.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 from dataclasses import dataclass, field
-from roadmapper.painter import Painter
+from .painter import Painter
 
 
 @dataclass(kw_only=True)
 class SubTitle:
     """Roadmap subtitle class"""
 
     text: str = field(init=True, default=None)
```

### Comparing `roadmapper-1.1.1/src/roadmapper/task.py` & `roadmapper-1.2.0/src/roadmapper/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from datetime import datetime, date, timedelta
-from dateutil.relativedelta import relativedelta
+
 from dataclasses import dataclass, field
-from contextlib import contextmanager
+from datetime import datetime
 
-from roadmapper.painter import Painter
-from roadmapper.timeline import Timeline
-from roadmapper.milestone import Milestone
+from .milestone import Milestone
+from .painter import Painter
+from .timeline import Timeline
 
 
 @dataclass(kw_only=True)
 class Task:
     """Roadmap Task class"""
 
     text: str = field(init=True, default=None)
@@ -588,7 +587,15 @@
             )
 
             for task in self.tasks:
                 task.draw(painter)
 
             for milestone in self.milestones:
                 milestone.draw(painter)
+
+    def __enter__(self):
+        """This method is called when the 'with' statement is used"""
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
+        """This method is called when the 'with' statement is used"""
+        pass
```

### Comparing `roadmapper-1.1.1/src/roadmapper/timeline.py` & `roadmapper-1.2.0/src/roadmapper/timeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 from datetime import datetime, date, timedelta
 from dateutil.relativedelta import relativedelta
 from dataclasses import dataclass, field
 import calendar
 
-from roadmapper.painter import Painter
-from roadmapper.timelineitem import TimelineItem
-from roadmapper.timelineitemyear import TimelineYear
-from roadmapper.timelinemode import TimelineMode
-from roadmapper.timelinelocale import TimelineLocale
+from .painter import Painter
+from .timelineitem import TimelineItem
+from .timelineitemyear import TimelineYear
+from .timelinemode import TimelineMode
+from .timelinelocale import TimelineLocale
 
 
 @dataclass(kw_only=True)
 class Timeline:
     """Roadmap Timeline Class"""
 
     mode: str = field(init=True, default=None)
```

### Comparing `roadmapper-1.1.1/src/roadmapper/timelineitem.py` & `roadmapper-1.2.0/src/roadmapper/timelineitem.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from datetime import datetime, date, timedelta
-from dateutil.relativedelta import relativedelta
-from dataclasses import dataclass, field
+
 import calendar
+from dataclasses import dataclass, field
+from datetime import datetime, date, timedelta
 
-from roadmapper.painter import Painter
-from roadmapper.timelinemode import TimelineMode
+from .painter import Painter
+from .timelinemode import TimelineMode
 
 
 @dataclass(kw_only=True)
 class TimelineItem:
     """Roadmap TimelineItem class"""
 
     text: str = field(init=True, default=None)
```

### Comparing `roadmapper-1.1.1/src/roadmapper/timelineitemyear.py` & `roadmapper-1.2.0/src/roadmapper/timelineitemyear.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,19 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from datetime import datetime, date, timedelta
-from dateutil.relativedelta import relativedelta
+
 from dataclasses import dataclass, field
-import calendar
+from datetime import datetime
 
-from roadmapper.painter import Painter
-from roadmapper.timelinemode import TimelineMode
+from .painter import Painter
 
 
 @dataclass(kw_only=True)
 class TimelineYear:
     """Roadmap TimelineYear class"""
 
     text: str = field(init=True, default=None)
```

### Comparing `roadmapper-1.1.1/src/roadmapper/timelinelocale.py` & `roadmapper-1.2.0/src/roadmapper/timelinelocale.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 from dataclasses import dataclass
 import json
 import os
 import locale
 
 default_timeline_locale_settings = {
     "locale": "en_US",
```

### Comparing `roadmapper-1.1.1/src/roadmapper/timelinemode.py` & `roadmapper-1.2.0/src/roadmapper/timelinemode.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from dataclasses import dataclass, field
+
+from dataclasses import dataclass
 
 
 @dataclass
 class TimelineMode:
     """Timeline mode for roadmap"""
 
     WEEKLY = "W"
```

### Comparing `roadmapper-1.1.1/src/roadmapper/title.py` & `roadmapper-1.2.0/src/roadmapper/title.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 from dataclasses import dataclass, field
-from roadmapper.painter import Painter
+from .painter import Painter
 
 
 @dataclass(kw_only=True)
 class Title:
     """Roadmap title class"""
 
     text: str = field(init=True, default=None)
```

### Comparing `roadmapper-1.1.1/src/roadmapper.egg-info/SOURCES.txt` & `roadmapper-1.2.0/src/roadmapper.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,8 +19,13 @@
 src/roadmapper/timelinemode.py
 src/roadmapper/title.py
 src/roadmapper/version.py
 src/roadmapper.egg-info/PKG-INFO
 src/roadmapper.egg-info/SOURCES.txt
 src/roadmapper.egg-info/dependency_links.txt
 src/roadmapper.egg-info/requires.txt
-src/roadmapper.egg-info/top_level.txt
+src/roadmapper.egg-info/top_level.txt
+src/tests/__init__.py
+src/tests/roadmap_draw_test.py
+src/tests/test_cases.py
+src/tests/test_painter.py
+src/tests/test_roadmapper.py
```

