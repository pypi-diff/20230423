# Comparing `tmp/thu_learn_downloader-0.1.8.tar.gz` & `tmp/thu_learn_downloader-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thu_learn_downloader-0.1.8.tar", max compression
+gzip compressed data, was "thu_learn_downloader-0.1.9.tar", max compression
```

## Comparing `thu_learn_downloader-0.1.8.tar` & `thu_learn_downloader-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-03-10 08:46:06.433145 thu_learn_downloader-0.1.8/LICENSE
--rw-r--r--   0        0        0     1381 2023-03-10 08:46:06.433145 thu_learn_downloader-0.1.8/README.md
--rw-r--r--   0        0        0      757 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/__init__.py
--rw-r--r--   0        0        0     2067 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/__main__.py
--rw-r--r--   0        0        0      968 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/constants.py
--rw-r--r--   0        0        0     5298 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/downloader.py
--rw-r--r--   0        0        0     4903 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/helper.py
--rw-r--r--   0        0        0     4346 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/parser.py
--rw-r--r--   0        0        0     8031 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/sync.py
--rw-r--r--   0        0        0     2083 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/typing.py
--rw-r--r--   0        0        0     4208 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/urls.py
--rw-r--r--   0        0        0     1813 2023-03-10 08:46:06.437145 thu_learn_downloader-0.1.8/thu_learn_downloader/utils.py
--rw-r--r--   0        0        0     2087 1970-01-01 00:00:00.000000 thu_learn_downloader-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1753 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/README.md
+-rw-r--r--   0        0        0      818 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/__init__.py
+-rw-r--r--   0        0        0     2588 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/__main__.py
+-rw-r--r--   0        0        0      400 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/config.py
+-rw-r--r--   0        0        0      887 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/constants.py
+-rw-r--r--   0        0        0     5298 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/downloader.py
+-rw-r--r--   0        0        0     4903 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/helper.py
+-rw-r--r--   0        0        0     4346 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/parser.py
+-rw-r--r--   0        0        0     7665 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/sync.py
+-rw-r--r--   0        0        0     2083 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/typing.py
+-rw-r--r--   0        0        0     4208 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/urls.py
+-rw-r--r--   0        0        0     1813 2023-03-22 15:28:07.324505 thu_learn_downloader-0.1.9/thu_learn_downloader/utils.py
+-rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 thu_learn_downloader-0.1.9/PKG-INFO
```

### Comparing `thu_learn_downloader-0.1.8/LICENSE` & `thu_learn_downloader-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thu_learn_downloader-0.1.8/thu_learn_downloader/__main__.py` & `thu_learn_downloader-0.1.9/thu_learn_downloader/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,47 @@
-import os
+import sys
+from pathlib import Path
 
-import hydra
-from omegaconf import DictConfig
+import typer
 from rich.console import Group
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import (
     BarColumn,
     MofNCompleteColumn,
     Progress,
     TextColumn,
     TimeElapsedColumn,
 )
 
 from . import sync
+from .config import Config
 from .constants import MAX_ACTIVE_TASKS, SUCCESS_PREFIX
 from .downloader import Downloader
 from .helper import Helper
 
 
-@hydra.main(config_path=os.getcwd(), config_name="config.yaml", version_base="1.3")
-def main(config: DictConfig) -> None:
+def main(
+    username: str = typer.Option("liqin20", "-u", "--username"),
+    password: str = typer.Option(
+        None, "-p", "--password", prompt=True, hide_input=True
+    ),
+    semester: list[str] = typer.Option(["2022-2023-2"], "-s", "--semester"),
+    course: list[str] = typer.Option([], "-c", "--course"),
+    prefix: Path = typer.Option(Path.home() / "Desktop" / "thu-learn", "--prefix"),
+    size_limit: int = typer.Option(sys.maxsize, "-s", "--size-limit"),
+) -> None:
+    config = Config(
+        username=username,
+        password=password,
+        semesters=semester,
+        courses=course,
+        prefix=prefix,
+        size_limit=size_limit,
+    )
     helper = Helper()
     downloader = Downloader()
     overall_progress = Progress(
         TextColumn("{task.description}", style="bold bright_blue"),
         BarColumn(),
         MofNCompleteColumn(),
         TimeElapsedColumn(),
@@ -32,16 +49,14 @@
     semesters_task_id = overall_progress.add_task(description="Semesters")
     courses_task_id = overall_progress.add_task(description="Courses")
     progress_group = Group(
         Panel(downloader.progress, height=MAX_ACTIVE_TASKS + 2),
         Panel(overall_progress),
     )
 
-    username: str = config.get("username")
-    password: str = config.get("password")
     with Live(progress_group) as live:
         with downloader.pool:
             try:
                 helper.login(username=username, password=password)
             except:
                 live.console.log(
                     f"Login as {username} FAILED",
@@ -60,9 +75,13 @@
                     console=live.console,
                     overall_progress=overall_progress,
                     semesters_task_id=semesters_task_id,
                     courses_task_id=courses_task_id,
                 )
 
 
+def run() -> None:
+    typer.run(main)
+
+
 if __name__ == "__main__":
-    main()
+    run()
```

### Comparing `thu_learn_downloader-0.1.8/thu_learn_downloader/constants.py` & `thu_learn_downloader-0.1.9/thu_learn_downloader/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from pathlib import Path
-
 from rich.style import Style
 
 from . import typing as t
 
 BS_FEATURES = "html.parser"
 CHUNK_SIZE = 1024 * 1024
-DEFAULT_PREFIX = Path.home() / "Desktop" / "thu-learn"
 MAX_ACTIVE_TASKS = 16
 
 
 FAILURE_PREFIX = "[reverse] FAILURE [/]"
 RETRY_PREFIX = "[reverse] RETRY [/]"
 SKIPPED_PREFIX = "[reverse] SKIPPED [/]"
 SUCCESS_PREFIX = "[reverse] SUCCESS [/]"
```

### Comparing `thu_learn_downloader-0.1.8/thu_learn_downloader/downloader.py` & `thu_learn_downloader-0.1.9/thu_learn_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `thu_learn_downloader-0.1.8/thu_learn_downloader/helper.py` & `thu_learn_downloader-0.1.9/thu_learn_downloader/helper.py`

 * *Files identical despite different names*

### Comparing `thu_learn_downloader-0.1.8/thu_learn_downloader/parser.py` & `thu_learn_downloader-0.1.9/thu_learn_downloader/parser.py`

 * *Files identical despite different names*

### Comparing `thu_learn_downloader-0.1.8/thu_learn_downloader/sync.py` & `thu_learn_downloader-0.1.9/thu_learn_downloader/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 import os
 import shutil
 import subprocess
-import sys
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
-from omegaconf import DictConfig
 from rich.console import Console
 from rich.progress import Progress, TaskID
 
 from . import typing as t
 from . import utils
-from .constants import (
-    DEFAULT_PREFIX,
-    DOCUMENT_STYLE,
-    HOMEWORK_STYLE,
-    SKIPPED_PREFIX,
-    SUCCESS_PREFIX,
-)
+from .config import Config
+from .constants import DOCUMENT_STYLE, HOMEWORK_STYLE, SKIPPED_PREFIX, SUCCESS_PREFIX
 from .downloader import Downloader
 from .helper import Helper
 
 
 def sync_all(
     helper: Helper,
     downloader: Downloader,
-    config: DictConfig,
+    config: Config,
     *,
     console: Console = Console(),
     overall_progress: Progress = Progress(),
     semesters_task_id: TaskID = TaskID(0),
     courses_task_id: TaskID = TaskID(1),
 ) -> None:
-    semesters = config.get("semesters") or helper.get_semester_id_list()
+    semesters = config.semesters or helper.get_semester_id_list()
 
     for semester in overall_progress.track(
         semesters, task_id=semesters_task_id, description="Semesters"
     ):
         sync_semester(
             helper=helper,
             downloader=downloader,
@@ -48,29 +41,29 @@
             courses_task_id=courses_task_id,
         )
 
 
 def sync_semester(
     helper: Helper,
     downloader: Downloader,
-    config: DictConfig,
+    config: Config,
     semester_id: str,
     *,
     console: Console = Console(),
     overall_progress: Progress = Progress(),
     courses_task_id: TaskID = TaskID(1),
 ) -> None:
     courses: list[t.CourseInfo] = helper.get_course_list(semester_id=semester_id)
 
-    if config.get("courses"):
+    if config.courses:
         courses = [
             course
             for course in courses
-            if course.name in config["courses"]
-            or course.english_name in config["courses"]
+            if (course.name in config.courses)
+            or (course.english_name in config.courses)
         ]
 
     overall_progress.update(
         task_id=courses_task_id, description=utils.format_semester_id(semester_id)
     )
     for course in overall_progress.track(courses, task_id=courses_task_id):
         sync_course(
@@ -81,15 +74,15 @@
             console=console,
         )
 
 
 def sync_course(
     helper: Helper,
     downloader: Downloader,
-    config: DictConfig,
+    config: Config,
     course: t.CourseInfo,
     *,
     console: Console = Console(),
 ) -> None:
     sync_files(
         helper=helper,
         downloader=downloader,
@@ -105,23 +98,21 @@
         console=console,
     )
 
 
 def sync_files(
     helper: Helper,
     downloader: Downloader,
-    config: DictConfig,
+    config: Config,
     course: t.CourseInfo,
     *,
     console: Console = Console(),
 ) -> None:
-    prefix: Path = Path(
-        config.get(key="prefix", default_value=DEFAULT_PREFIX)
-    ).expanduser()
-    size_limit: int = config.get(key="size_limit", default_value=sys.maxsize)
+    prefix: Path = config.prefix
+    size_limit: int = config.size_limit
 
     files: list[t.File] = helper.get_file_list(course_id=course.id)
     files: list[t.File] = sorted(files, key=lambda f: f.id)
 
     for i, f in enumerate(files):
         filename: str = utils.format_doc_filename(title=f.title, file_type=f.file_type)
         filename: str = f"{i:02d}-{filename}"
@@ -149,15 +140,15 @@
             ),
         )
 
 
 def sync_homeworks(
     helper: Helper,
     downloader: Downloader,
-    config: DictConfig,
+    config: Config,
     course: t.CourseInfo,
     *,
     console: Console = Console(),
 ) -> None:
     homeworks = helper.get_homework_list(course_id=course.id)
 
     for hw in homeworks:
@@ -178,23 +169,21 @@
             console=console,
         )
 
 
 def sync_homework_detail(
     helper: Helper,
     downloader: Downloader,
-    config: DictConfig,
+    config: Config,
     course: t.CourseInfo,
     hw: t.Homework,
     *,
     console: Console = Console(),
 ) -> None:
-    prefix: Path = Path(
-        config.get(key="prefix", default_value=DEFAULT_PREFIX)
-    ).expanduser()
+    prefix: Path = config.prefix
     title: str = f"{hw.number:02d}-{hw.title}"
     filepath: Path = prefix / course.english_name / "work" / title / "README.md"
     os.makedirs(filepath.parent, exist_ok=True)
     with open(file=filepath, mode="w") as fp:
         fp.write(utils.format_homework_readme(hw=hw))
         fp.flush()
     if shutil.which("prettier"):
@@ -207,15 +196,15 @@
         style=HOMEWORK_STYLE,
     )
 
 
 def sync_homework_attachments(
     helper: Helper,
     downloader: Downloader,
-    config: DictConfig,
+    config: Config,
     course: t.CourseInfo,
     hw: t.Homework,
     *,
     console: Console = Console(),
 ) -> None:
     sync_homework_attachment(
         helper=helper,
@@ -258,27 +247,25 @@
         console=console,
     )
 
 
 def sync_homework_attachment(
     helper: Helper,
     downloader: Downloader,
-    config: DictConfig,
+    config: Config,
     course: t.CourseInfo,
     hw: t.Homework,
     attach: Optional[t.RemoteFile],
     attach_type: str,
     *,
     console: Console = Console(),
 ) -> None:
     if not attach:
         return
-    prefix: Path = Path(
-        config.get(key="prefix", default_value=DEFAULT_PREFIX)
-    ).expanduser()
+    prefix: Path = config.prefix
     title: str = f"{hw.number:02d}-{hw.title}"
     filename: str = utils.remove_attachment_prefix(attach.name)
     filename: str = f"{attach_type}-{filename}"
     filepath: Path = prefix / course.english_name / "work" / title / filename
     upload_time: Optional[datetime] = None
     match attach_type:
         case "attach":
```

### Comparing `thu_learn_downloader-0.1.8/thu_learn_downloader/typing.py` & `thu_learn_downloader-0.1.9/thu_learn_downloader/typing.py`

 * *Files identical despite different names*

### Comparing `thu_learn_downloader-0.1.8/thu_learn_downloader/urls.py` & `thu_learn_downloader-0.1.9/thu_learn_downloader/urls.py`

 * *Files identical despite different names*

### Comparing `thu_learn_downloader-0.1.8/thu_learn_downloader/utils.py` & `thu_learn_downloader-0.1.9/thu_learn_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `thu_learn_downloader-0.1.8/PKG-INFO` & `thu_learn_downloader-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: thu-learn-downloader
-Version: 0.1.8
+Version: 0.1.9
 Summary: Download everything from Web Learning of Tsinghua University
 Home-page: https://github.com/liblaf/thu-learn-downloader
 Author: Qin Li
 Author-email: liblaf@outlook.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
-Requires-Dist: hydra-core (>=1.3.1,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: rich (>=13.3.1,<14.0.0)
+Requires-Dist: rich (>=12.0.0,<13.0.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/liblaf/thu-learn-downloader
 Description-Content-Type: text/markdown
 
 # thu-learn-downloader
 
 Download everything from Web Learning of Tsinghua University
 
 ## Demo
 
-![Demo](https://res.cloudinary.com/liblaf/image/upload/v1677213088/2023/02/24/20230224-1677213085.gif)
+![Demo](https://res.cloudinary.com/liblaf/image/upload/v1679497703/2023/03/22/20230322-1679497699.gif)
 
 The resulting file structure looks like:
 
 ```
 thu-learn
 └── Quantum Mechanics(1)
    ├── docs
@@ -36,23 +36,42 @@
    └── work
       └── 01-第一周作业
          ├── attach-第一周作业.pdf
          ├── submit-第一周作业.pdf
          └── README.md
 ```
 
+## Usage
+
+**Usage**:
+
+```shell-session
+$ tld [OPTIONS]
+```
+
+**Options**:
+
+- `-u, --username TEXT`: [default: liqin20]
+- `-p, --password TEXT`
+- `-s, --semester TEXT`: [default: 2022-2023-2]
+- `-c, --course TEXT`
+- `--prefix PATH`: [default: /home/liblaf/Desktop/thu-learn]
+- `-s, --size-limit INTEGER`: [default: 9223372036854775807]
+- `--install-completion`: Install completion for the current shell.
+- `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
+- `--help`: Show this message and exit.
+
 ## Features
 
 - fast concurrent download
 - pretty TUI powered by [rich](https://github.com/Textualize/rich)
 - auto set `mtime` of downloaded files according to timestamp of remote file
 - auto skip download when local file is newer
 - dump homework details into `README.md` in each homework folder
 - pretty markdown files powered by [prettier](https://prettier.io) (require `prettier` installed)
 
-## Usage
-
-Download pre-built binary from [releases](https://github.com/liblaf/thu-learn-downloader/releases) or install from PyPI by executing `pip install thu-learn-downloader`.
+## Installation
 
-1. Prepare a `config.yaml` like [config.yaml](https://github.com/liblaf/thu-learn-downloader/blob/main/config.yaml).
-2. Run `thu-learn-downloader password="***"` and wait for the sync to finish.
+- download pre-built binary form [GitHub Releases](https://github.com/liblaf/thu-learn-downloader/releases)
+- `pip install thu-learn-downloader`
+- `pipx install thu-learn-downloader`
```

