# Comparing `tmp/kerykeion-4.0a4.tar.gz` & `tmp/kerykeion-4.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerykeion-4.0a4.tar", max compression
+gzip compressed data, was "kerykeion-4.0a5.tar", max compression
```

## Comparing `kerykeion-4.0a4.tar` & `kerykeion-4.0a5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     6519 2023-01-08 19:46:40.441366 kerykeion-4.0a4/README.md
--rw-r--r--   0        0        0     3746 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/__init__.py
--rw-r--r--   0        0        0      316 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/aspects/__init__.py
--rw-r--r--   0        0        0      230 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/aspects/aspects_settings.py
--rw-r--r--   0        0        0     2982 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/aspects/composite_aspects.py
--rw-r--r--   0        0        0    10625 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/aspects/natal_aspects.py
--rw-r--r--   0        0        0      127 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/charts/__init__.py
--rwxr-xr-x   0        0        0    67889 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/charts/charts_svg.py
--rwxr-xr-x   0        0        0    56546 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    56733 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/charts/templates/extended.xml
--rw-r--r--   0        0        0     4690 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/fetch_geonames.py
--rw-r--r--   0        0        0    11423 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/kr.config.json
--rw-r--r--   0        0        0    21131 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/kr_instance.py
--rw-r--r--   0        0        0      104 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/kr_types/__init__.py
--rw-r--r--   0        0        0      337 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/kr_types/kerykeion_exception.py
--rw-r--r--   0        0        0     1027 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/kr_types/kr_literals.py
--rw-r--r--   0        0        0     3857 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/kr_types/kr_models.py
--rw-r--r--   0        0        0     7592 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/relationship_score.py
--rw-r--r--   0        0        0     2455 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/report.py
--rw-r--r--   0        0        0     6673 2023-01-08 19:46:40.445366 kerykeion-4.0a4/kerykeion/utilities.py
--rw-r--r--   0        0        0     2229 2023-01-08 19:46:40.445366 kerykeion-4.0a4/pyproject.toml
--rw-r--r--   0        0        0     7877 1970-01-01 00:00:00.000000 kerykeion-4.0a4/setup.py
--rw-r--r--   0        0        0     8294 1970-01-01 00:00:00.000000 kerykeion-4.0a4/PKG-INFO
+-rw-r--r--   0        0        0    18091 2023-01-08 19:26:15.413715 kerykeion-4.0a5/LICENSE
+-rw-r--r--   0        0        0     6519 2023-02-15 21:33:35.198498 kerykeion-4.0a5/README.md
+-rw-r--r--   0        0        0     3746 2023-02-15 21:33:35.199155 kerykeion-4.0a5/kerykeion/__init__.py
+-rw-r--r--   0        0        0      316 2023-02-15 21:33:35.199279 kerykeion-4.0a5/kerykeion/aspects/__init__.py
+-rw-r--r--   0        0        0      230 2023-02-15 21:33:35.199380 kerykeion-4.0a5/kerykeion/aspects/aspects_settings.py
+-rw-r--r--   0        0        0     2982 2023-02-15 21:33:35.199557 kerykeion-4.0a5/kerykeion/aspects/composite_aspects.py
+-rw-r--r--   0        0        0    10625 2023-02-15 21:33:35.199665 kerykeion-4.0a5/kerykeion/aspects/natal_aspects.py
+-rw-r--r--   0        0        0      127 2023-02-15 21:33:35.199813 kerykeion-4.0a5/kerykeion/charts/__init__.py
+-rwxr-xr-x   0        0        0    67889 2023-02-15 21:33:35.200435 kerykeion-4.0a5/kerykeion/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    56546 2023-01-08 19:26:15.412083 kerykeion-4.0a5/kerykeion/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    56733 2023-01-08 19:26:15.412582 kerykeion-4.0a5/kerykeion/charts/templates/extended.xml
+-rw-r--r--   0        0        0     4690 2023-02-15 21:33:35.200689 kerykeion-4.0a5/kerykeion/fetch_geonames.py
+-rw-r--r--   0        0        0    12446 2023-02-15 21:33:35.200979 kerykeion-4.0a5/kerykeion/kr.config.json
+-rw-r--r--   0        0        0    21131 2023-02-15 21:33:35.201333 kerykeion-4.0a5/kerykeion/kr_instance.py
+-rw-r--r--   0        0        0      104 2023-02-15 21:33:35.201474 kerykeion-4.0a5/kerykeion/kr_types/__init__.py
+-rw-r--r--   0        0        0      337 2023-02-15 21:33:35.201619 kerykeion-4.0a5/kerykeion/kr_types/kerykeion_exception.py
+-rw-r--r--   0        0        0     1027 2023-02-15 21:33:35.201725 kerykeion-4.0a5/kerykeion/kr_types/kr_literals.py
+-rw-r--r--   0        0        0     3857 2023-02-15 21:33:35.201812 kerykeion-4.0a5/kerykeion/kr_types/kr_models.py
+-rw-r--r--   0        0        0     7592 2023-02-15 21:33:35.202022 kerykeion-4.0a5/kerykeion/relationship_score.py
+-rw-r--r--   0        0        0     2455 2023-02-15 21:33:35.202207 kerykeion-4.0a5/kerykeion/report.py
+-rw-r--r--   0        0        0     6673 2023-02-15 21:33:35.202442 kerykeion-4.0a5/kerykeion/utilities.py
+-rw-r--r--   0        0        0     2229 2023-02-15 21:34:49.315701 kerykeion-4.0a5/pyproject.toml
+-rw-r--r--   0        0        0     7877 1970-01-01 00:00:00.000000 kerykeion-4.0a5/setup.py
+-rw-r--r--   0        0        0     8294 1970-01-01 00:00:00.000000 kerykeion-4.0a5/PKG-INFO
```

### Comparing `kerykeion-4.0a4/README.md` & `kerykeion-4.0a5/README.md`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/__init__.py` & `kerykeion-4.0a5/kerykeion/__init__.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/aspects/composite_aspects.py` & `kerykeion-4.0a5/kerykeion/aspects/composite_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/aspects/natal_aspects.py` & `kerykeion-4.0a5/kerykeion/aspects/natal_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/charts/charts_svg.py` & `kerykeion-4.0a5/kerykeion/charts/charts_svg.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/charts/templates/basic.xml` & `kerykeion-4.0a5/kerykeion/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/charts/templates/extended.xml` & `kerykeion-4.0a5/kerykeion/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/fetch_geonames.py` & `kerykeion-4.0a5/kerykeion/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/kr.config.json` & `kerykeion-4.0a5/kerykeion/kr.config.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9800000000000001%*

 * *Differences: {"'language_settings'": "{'CN': OrderedDict([('info', '命盤資訊'), ('cusp', '宮'), ('longitude', '經度'), "*

 * *                        "('latitude', '緯度'), ('north', '北'), ('east', '東'), ('south', '南'), "*

 * *                        "('west', '西'), ('fire', '火'), ('earth', '土'), ('air', '風'), ('water', "*

 * *                        "'水'), ('&', '與'), ('transits', '流年合盤'), ('type', '盤型'), ('aspects', "*

 * *                        "'相位'), ('planets_and_house', '行星 與 宫位'), ('transit_name', '流年星相'), "*

 * *                        "('luna […]*

```diff
@@ -327,14 +327,54 @@
         "zodiac_radix_ring_2": "#ff0000",
         "zodiac_transit_ring_0": "#ff0000",
         "zodiac_transit_ring_1": "#ff0000",
         "zodiac_transit_ring_2": "#0000ff",
         "zodiac_transit_ring_3": "#0000ff"
     },
     "language_settings": {
+        "CN": {
+            "&": "\u8207",
+            "air": "\u98a8",
+            "aspects": "\u76f8\u4f4d",
+            "celestial_points": {
+                "Asc": "\u4e0a\u5347\u9ede",
+                "Dsc": "\u4e0b\u964d\u9ede",
+                "Ic": "\u4e0b\u4e2d\u5929",
+                "Jupiter": "\u6728\u661f",
+                "Mars": "\u706b\u661f",
+                "Mc": "\u4e0a\u4e2d\u5929",
+                "Mean_Node": "\u5e73\u4ea4\u9ede",
+                "Mercury": "\u6c34\u661f",
+                "Moon": "\u6708\u4eae",
+                "Neptune": "\u6d77\u738b\u661f",
+                "North_Node": "\u5317\u4ea4\u9ede",
+                "Pluto": "\u51a5\u738b\u661f",
+                "Saturn": "\u571f\u661f",
+                "Sun": "\u592a\u967d",
+                "Uranus": "\u5929\u738b\u661f",
+                "Venus": "\u91d1\u661f"
+            },
+            "cusp": "\u5bae",
+            "day": "\u65e5",
+            "earth": "\u571f",
+            "east": "\u6771",
+            "fire": "\u706b",
+            "info": "\u547d\u76e4\u8cc7\u8a0a",
+            "latitude": "\u7def\u5ea6",
+            "longitude": "\u7d93\u5ea6",
+            "lunar_phase": "\u6708\u76f8",
+            "north": "\u5317",
+            "planets_and_house": "\u884c\u661f \u8207 \u5bab\u4f4d",
+            "south": "\u5357",
+            "transit_name": "\u6d41\u5e74\u661f\u76f8",
+            "transits": "\u6d41\u5e74\u5408\u76e4",
+            "type": "\u76e4\u578b",
+            "water": "\u6c34",
+            "west": "\u897f"
+        },
         "EN": {
             "&": "and",
             "air": "Air",
             "aspects": "Couple aspects",
             "celestial_points": {
                 "Asc": "Asc",
                 "Dsc": "Dsc",
```

### Comparing `kerykeion-4.0a4/kerykeion/kr_instance.py` & `kerykeion-4.0a5/kerykeion/kr_instance.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/kr_types/kr_literals.py` & `kerykeion-4.0a5/kerykeion/kr_types/kr_literals.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/kr_types/kr_models.py` & `kerykeion-4.0a5/kerykeion/kr_types/kr_models.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/relationship_score.py` & `kerykeion-4.0a5/kerykeion/relationship_score.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/report.py` & `kerykeion-4.0a5/kerykeion/report.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/kerykeion/utilities.py` & `kerykeion-4.0a5/kerykeion/utilities.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.0a4/pyproject.toml` & `kerykeion-4.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kerykeion"
-version = "4.0a4"
+version = "4.0a5"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>"]
 description = "A python library for astrology."
 license = "GPL-2.0"
 homepage = "https://github.com/g-battaglia/kerykeion"
 repository = "https://github.com/g-battaglia/kerykeion"
 keywords = [
     "astrology",
```

### Comparing `kerykeion-4.0a4/setup.py` & `kerykeion-4.0a5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'terminaltables>=3.1.10,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['create-docs = scripts.docs:main']}
 
 setup_kwargs = {
     'name': 'kerykeion',
-    'version': '4.0a4',
+    'version': '4.0a5',
     'description': 'A python library for astrology.',
     'long_description': '<h1 align=center>Kerykeion</h1>\n<div align="center">\n    <a href="#">\n        <img src="https://img.shields.io/github/contributors/g-battaglia/kerykeion?color=blue&logo=github" alt="contributors">\n    </a>\n    <a href="#">\n        <img src="https://img.shields.io/github/stars/g-battaglia/kerykeion.svg?logo=github" alt="stars">\n    </a>\n    <a href="#">\n        <img src="https://img.shields.io/github/forks/g-battaglia/kerykeion.svg?logo=github" alt="forks">\n    </a>\n    <a href="https://pypi.org/project/kerykeion" target="_blank">\n        <img src="https://visitor-badge.laobi.icu/badge?page_id=g-battaglia.kerykeion" alt="visitors"/>\n    </a>    \n    <a href="https://pypi.org/project/kerykeion" target="_blank">\n        <img src="https://img.shields.io/pypi/v/kerykeion?label=pypi%20package" alt="Package version">\n    </a>\n    <a href="https://pypi.org/project/kerykeion" target="_blank">\n        <img src="https://img.shields.io/pypi/pyversions/kerykeion.svg" alt="Supported Python versions">\n    </a>\n</div>\n\n&nbsp;\n\nKerykeion is a python library for Astrology.\nIt can calculate all the planet and house position,\nalso it can calculate the aspects of a single persone or between two, you can set how many planets you\nneed in the settings in the utility module.\nIt also can generate an SVG of a birthchart, a composite chart or a transit chart.\n\n## Installation\n\nKerykeion is a *Python 3.9* package, make sure you have *Python 3.9* or above installed on your system.\n\n```bash\npip3 install kerykeion\n```\n\n## Usage\n\nHere some examples:\n\n```python\n\n# Import the main class for creating a kerykeion instance:\nfrom kerykeion import KrInstance\n\n# Create a kerykeion instance:\n# Args: Name, year, month, day, hour, minuts, city, nation(optional)\nkanye = KrInstance("Kanye", 1977, 6, 8, 8, 45, "Atlanta")\n\n# Get the information about the sun in the chart:\n# (The position of the planets always starts at 0)\nkanye.sun\n\n#> {\'name\': \'Sun\', \'quality\': \'Mutable\', \'element\': \'Air\', \'sign\': \'Gem\', \'sign_num\': 2, \'pos\': 17.598992059774275, \'abs_pos\': 77.59899205977428, \'emoji\': \'♊️\', \'house\': \'12th House\', \'retrograde\': False}\n\n# Get informations about the first house:\nkanye.first_house\n\n#> {\'name\': \'First House\', \'quality\': \'Cardinal\', \'element\': \'Water\', \'sign\': \'Can\', \'sign_num\': 3, \'pos\': 17.995779673209114, \'abs_pos\': 107.99577967320911, \'emoji\': \'♋️\'}\n\n# Get element of the moon sign:\nkanye.moon.get("element")\n\n#> \'Water\'\n\n```\n\n**To avoid connecting to GeoNames (eg. avoiding hourly limit or no internet connection) you should instance kerykeion like this:**\n\n```python\nkanye = KrInstance(\n    "Kanye", 1977, 6, 8, 8, 45,\n    lng=50, lat=50, tz_str="Europe/Rome"\n    )\n```\n\n## Generate a SVG Chart:\n\n```python\nfrom kerykeion import KrInstance, MakeSvgInstance\n\nfirst = KrInstance("Jack", 1990, 6, 15, 15, 15, "Roma")\nsecond = KrInstance("Jane", 1991, 10, 25, 21, 00, "Roma")\n\n# Set the type, it can be Natal, Composite or Transit\n\nname = MakeSvgInstance(first, chart_type="Composite", second_obj=second)\nname.makeSVG()\nprint(len(name.aspects_list))\n\n#> Generating kerykeion object for Jack...\n#> Generating kerykeion object for Jane...\n#> Jack birth location: Roma, 41.89193, 12.51133\n#> SVG Generated Correctly\n#> 38\n\n```\n\n![alt text](http://centuryboy.altervista.org/JackComposite_Chart.svg)\n\n\n# Report\n\nTo print a report of all the data:\n\n```python\nfrom kerykeion import Report, KrInstance\n\nkanye = KrInstance("Kanye", 1977, 6, 8, 8, 45, "Atlanta")\nreport = Report(kanye)\nreport.print_report()\n\n```\n\nReturns:\n\n```\n+- Kerykeion report for Kanye -+\n+----------+------+-------------+-----------+----------+\n| Date     | Time | Location    | Longitude | Latitude |\n+----------+------+-------------+-----------+----------+\n| 8/6/1977 | 8:45 | Atlanta, US | -84.38798 | 33.749   |\n+----------+------+-------------+-----------+----------+\n+-----------+------+-------+------+----------------+\n| Planet    | Sign | Pos.  | Ret. | House          |\n+-----------+------+-------+------+----------------+\n| Sun       | Gem  | 17.6  | -    | Twelfth House  |\n| Moon      | Pis  | 16.43 | -    | Ninth House    |\n| Mercury   | Tau  | 26.29 | -    | Eleventh House |\n| Venus     | Tau  | 2.03  | -    | Tenth House    |\n| Mars      | Tau  | 1.79  | -    | Tenth House    |\n| Jupiter   | Gem  | 14.61 | -    | Eleventh House |\n| Saturn    | Leo  | 12.8  | -    | Second House   |\n| Uranus    | Sco  | 8.27  | R    | Fourth House   |\n| Neptune   | Sag  | 14.69 | R    | Fifth House    |\n| Pluto     | Lib  | 11.45 | R    | Fourth House   |\n| Mean_Node | Lib  | 21.49 | R    | Fourth House   |\n| True_Node | Lib  | 22.82 | R    | Fourth House   |\n+-----------+------+-------+------+----------------+\n+----------------+------+----------+\n| House          | Sign | Position |\n+----------------+------+----------+\n| First House    | Can  | 18.0     |\n| Second House   | Leo  | 9.51     |\n| Third House    | Vir  | 4.02     |\n| Fourth House   | Lib  | 3.98     |\n| Fifth House    | Sco  | 9.39     |\n| Sixth House    | Sag  | 15.68    |\n| Seventh House  | Cap  | 18.0     |\n| Eighth House   | Aqu  | 9.51     |\n| Ninth House    | Pis  | 4.02     |\n| Tenth House    | Ari  | 3.98     |\n| Eleventh House | Tau  | 9.39     |\n| Twelfth House  | Gem  | 15.68    |\n+----------------+------+----------+\n\n```\n\nAnd if you want to export it to a file:\n\n```bash\n$ python3 your_script_name.py > file.txt \n```\n\n## Other exeples of possibles usecase\n\n```python\n# Get all aspects between two persons:\n\nfrom kerykeion import CompositeAspects, KrInstance\nfirst = KrInstance("Jack", 1990, 6, 15, 15, 15, "Roma")\nsecond = KrInstance("Jane", 1991, 10, 25, 21, 00, "Roma")\n\nname = CompositeAspects(first, second)\naspect_list = name.get_relevant_aspects()\nprint(aspect_list[0])\n\n#> Generating kerykeion object for Jack...\n#> Generating kerykeion object for Jane...\n#> {\'p1_name\': \'Sun\', \'p1_abs_pos\': 84.17867971515636, \'p2_name\': \'Sun\', \'p2_abs_pos\': 211.90472999502984, \'aspect\': \'trine\', \'orbit\': 7.726050279873476, \'aspect_degrees\': 120, \'color\': \'#36d100\', \'aid\': 6, \'diff\': 127.72605027987348, \'p1\': 0, \'p2\': 0}\n\n```\n\n## Documentation\n\nMost of the functions and the classes are self documented by the types and have docstrings.\nAn auto-generated documentation [is available here](https://g-battaglia.github.io/kerykeion).\n\nSooner or later I\'ll try to write an extensive documentation.\n\n## Development\n\nYou can clone this repository or download a zip file using the right side buttons.\n\n## Contributing\n\nFeel free to contribute to the code!\n',
     'author': 'Giacomo Battaglia',
     'author_email': 'battaglia.giacomo@yahoo.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/g-battaglia/kerykeion',
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'kerykeion.aspects', 'kerykeion.charts', 'kerykeion.kr_types'] package_data = \
 {'': ['*'], 'kerykeion.charts': ['templates/*']} install_requires = \
 ['jsonpickle>=3.0.1,<4.0.0', 'pydantic>=1.10.4,<2.0.0',
 'pyswisseph>=2.10.3.1,<3.0.0.0', 'pytz>=2022.7,<2023.0', 'requests-
 cache>=0.9.7,<0.10.0', 'requests>=2.28.1,<3.0.0',
 'terminaltables>=3.1.10,<4.0.0'] entry_points = \ {'console_scripts': ['create-
 docs = scripts.docs:main']} setup_kwargs = { 'name': 'kerykeion', 'version':
-'4.0a4', 'description': 'A python library for astrology.', 'long_description':
+'4.0a5', 'description': 'A python library for astrology.', 'long_description':
 '
                             ****** Kerykeion ******
 \n
  \n \n_[contributors]\n\n \n_[stars]\n\n \n_[forks]\n\n \n_[visitors]\n \n \n_
            [Package_version]\n\n \n_[Supported_Python_versions]\n\n
 \n\n \n\nKerykeion is a python library for Astrology.\nIt can calculate all the
 planet and house position,\nalso it can calculate the aspects of a single
```

### Comparing `kerykeion-4.0a4/PKG-INFO` & `kerykeion-4.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerykeion
-Version: 4.0a4
+Version: 4.0a5
 Summary: A python library for astrology.
 Home-page: https://github.com/g-battaglia/kerykeion
 License: GPL-2.0
 Keywords: astrology,ephemeris,astrology library,birtchart,svg,zodiac,zodiac-sing,astronomical-algorithms,synastry,astrology-calculator
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kerykeion Version: 4.0a4 Summary: A python library
+Metadata-Version: 2.1 Name: kerykeion Version: 4.0a5 Summary: A python library
 for astrology. Home-page: https://github.com/g-battaglia/kerykeion License:
 GPL-2.0 Keywords: astrology,ephemeris,astrology
 library,birtchart,svg,zodiac,zodiac-sing,astronomical-
 algorithms,synastry,astrology-calculator Author: Giacomo Battaglia Author-
 email: battaglia.giacomo@yahoo.it Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
```

