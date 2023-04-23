# Comparing `tmp/bmkg-1.0.1.tar.gz` & `tmp/bmkg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmkg-1.0.1.tar", last modified: Sun Apr 23 17:15:25 2023, max compression
+gzip compressed data, was "bmkg-1.0.2.tar", last modified: Sun Apr 23 17:36:26 2023, max compression
```

## Comparing `bmkg-1.0.1.tar` & `bmkg-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 17:15:25.890121 bmkg-1.0.1/
--rw-rw-rw-   0        0        0     1066 2023-04-23 17:11:27.000000 bmkg-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-23 17:11:27.000000 bmkg-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3635 2023-04-23 17:15:25.888073 bmkg-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2077 2023-04-23 17:11:27.000000 bmkg-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 17:15:25.803928 bmkg-1.0.1/bmkg/
--rw-rw-rw-   0        0        0     1473 2023-04-23 17:13:08.000000 bmkg-1.0.1/bmkg/__init__.py
--rw-rw-rw-   0        0        0     2059 2023-04-23 17:11:27.000000 bmkg-1.0.1/bmkg/base.py
--rw-rw-rw-   0        0        0     9065 2023-04-23 17:11:27.000000 bmkg-1.0.1/bmkg/client.py
--rw-rw-rw-   0        0        0     1431 2023-04-23 17:11:27.000000 bmkg-1.0.1/bmkg/constants.py
--rw-rw-rw-   0        0        0     3914 2023-04-23 17:11:27.000000 bmkg-1.0.1/bmkg/earthquake.py
--rw-rw-rw-   0        0        0     4887 2023-04-23 17:11:27.000000 bmkg-1.0.1/bmkg/enums.py
--rw-rw-rw-   0        0        0     1248 2023-04-23 17:11:27.000000 bmkg-1.0.1/bmkg/errors.py
--rw-rw-rw-   0        0        0     8275 2023-04-23 17:11:27.000000 bmkg-1.0.1/bmkg/forecast.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:15:25.886043 bmkg-1.0.1/bmkg.egg-info/
--rw-rw-rw-   0        0        0     3635 2023-04-23 17:15:25.000000 bmkg-1.0.1/bmkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-04-23 17:15:25.000000 bmkg-1.0.1/bmkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:15:25.000000 bmkg-1.0.1/bmkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-23 17:15:25.000000 bmkg-1.0.1/bmkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 17:15:25.000000 bmkg-1.0.1/bmkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1414 2023-04-23 17:11:48.000000 bmkg-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 17:15:25.890121 bmkg-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 17:36:26.686850 bmkg-1.0.2/
+-rw-rw-rw-   0        0        0     1066 2023-04-23 17:28:59.000000 bmkg-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-23 17:28:59.000000 bmkg-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3635 2023-04-23 17:36:26.684848 bmkg-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2077 2023-04-23 17:28:59.000000 bmkg-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 17:36:26.612796 bmkg-1.0.2/bmkg/
+-rw-rw-rw-   0        0        0     1479 2023-04-23 17:33:35.000000 bmkg-1.0.2/bmkg/__init__.py
+-rw-rw-rw-   0        0        0     2059 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/base.py
+-rw-rw-rw-   0        0        0     9065 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/client.py
+-rw-rw-rw-   0        0        0     1431 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/constants.py
+-rw-rw-rw-   0        0        0     3914 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/earthquake.py
+-rw-rw-rw-   0        0        0     4887 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/enums.py
+-rw-rw-rw-   0        0        0     1248 2023-04-23 17:28:59.000000 bmkg-1.0.2/bmkg/errors.py
+-rw-rw-rw-   0        0        0     8356 2023-04-23 17:32:32.000000 bmkg-1.0.2/bmkg/forecast.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:36:26.681847 bmkg-1.0.2/bmkg.egg-info/
+-rw-rw-rw-   0        0        0     3635 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 17:36:26.000000 bmkg-1.0.2/bmkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1414 2023-04-23 17:33:35.000000 bmkg-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:36:26.687857 bmkg-1.0.2/setup.cfg
```

### Comparing `bmkg-1.0.1/LICENSE` & `bmkg-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.1/PKG-INFO` & `bmkg-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bmkg
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial Python wrapper for the BMKG (Meteorology, Climatology, and Geophysical Agency) API.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/bmkg
-Project-URL: download_url, https://github.com/null8626/bmkg/archive/1.0.1.tar.gz
+Project-URL: download_url, https://github.com/null8626/bmkg/archive/1.0.2.tar.gz
 Keywords: weather,bmkg,indonesia,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `bmkg-1.0.1/README.md` & `bmkg-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.1/bmkg/__init__.py` & `bmkg-1.0.2/bmkg/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 SOFTWARE.
 """
 
 from .enums import AreaKind, Direction, ForecastKind, MMI, Province
 from .constants import METRIC, IMPERIAL
 from .client import Client
 
-__version__ = '1.0.1'
-__all__ = ('AreaKind', 'Client', 'Direction', 'ForecastKind', 'METRIC', 'MMI', 'IMPERIAL', 'Province')
+__version__ = '1.0.2'
+__all__ = (
+  'AreaKind', 'Client', 'Direction', 'ForecastKind', 'METRIC', 'MMI',
+  'IMPERIAL', 'Province'
+)
```

### Comparing `bmkg-1.0.1/bmkg/base.py` & `bmkg-1.0.2/bmkg/base.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.1/bmkg/client.py` & `bmkg-1.0.2/bmkg/client.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.1/bmkg/constants.py` & `bmkg-1.0.2/bmkg/constants.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.1/bmkg/earthquake.py` & `bmkg-1.0.2/bmkg/earthquake.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.1/bmkg/enums.py` & `bmkg-1.0.2/bmkg/enums.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.1/bmkg/errors.py` & `bmkg-1.0.2/bmkg/errors.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.1/bmkg/forecast.py` & `bmkg-1.0.2/bmkg/forecast.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 from enum import auto
 
 from .enums import AreaKind, Direction, ForecastKind
 from .constants import METRIC, XML_NAMESPACES
 from .base import CustomizableUnit
 
 Humidity = namedtuple('Humidity', 'date value')
-MinHumidity = namedtuple('MinHumidity', 'date value')
-MaxHumidity = namedtuple('MaxHumidity', 'date value')
+LowestHumidity = namedtuple('LowestHumidity', 'date value')
+HighestHumidity = namedtuple('HighestHumidity', 'date value')
 Temperature = namedtuple('Temperature', 'date value')
-MinTemperature = namedtuple('MinTemperature', 'date value')
-MaxTemperature = namedtuple('MaxTemperature', 'date value')
+LowestTemperature = namedtuple('LowestTemperature', 'date value')
+HighestTemperature = namedtuple('HighestTemperature', 'date value')
 HourlyForecast = namedtuple('HourlyForecast', 'date kind')
 WindDirection = namedtuple('WindDirection', 'date degrees direction')
 WindSpeed = namedtuple('WindSpeed', 'date knots value')
 
 class Forecast(CustomizableUnit):
   """Represents a single weather forecast for a given location."""
   
@@ -89,31 +89,31 @@
       Humidity(
         datetime.strptime(child.attrib['datetime'], '%Y%m%d%H%M'),
         int(child.find('value').text)
       ) for child in self.__inner.iterfind('./parameter[@id="hu"]/timerange')
     )
   
   @property
-  def min_humidity(self) -> Iterable[MinHumidity]:
-    """Iterable[:class:`MinHumidity`]: This weather forecast's minimum humidity values across various timeframes."""
+  def lowest_humidity(self) -> Iterable[LowestHumidity]:
+    """Iterable[:class:`LowestHumidity`]: This weather forecast's lowest humidity values across various timeframes."""
     
     return (
-      MinHumidity(
+      LowestHumidity(
         datetime.strptime(child.attrib['datetime'], '%Y%m%d%H%M'),
         int(child.find('value').text)
       )
       for child in self.__inner.iterfind('./parameter[@id="humin"]/timerange')
     )
   
   @property
-  def max_humidity(self) -> Iterable[MaxHumidity]:
-    """Iterable[:class:`MaxHumidity`]: This weather forecast's maximum humidity values across various timeframes."""
+  def highest_humidity(self) -> Iterable[HighestHumidity]:
+    """Iterable[:class:`HighestHumidity`]: This weather forecast's highest humidity values across various timeframes."""
     
     return (
-      MaxHumidity(
+      HighestHumidity(
         datetime.strptime(child.attrib['datetime'], '%Y%m%d%H%M'),
         int(child.find('value').text)
       )
       for child in self.__inner.iterfind('./parameter[@id="humax"]/timerange')
     )
   
   @property
@@ -126,34 +126,34 @@
       Temperature(
         datetime.strptime(child.attrib['datetime'], '%Y%m%d%H%M'),
         float(child.find(f'./value[@unit="{unit}"]').text)
       ) for child in self.__inner.iterfind('./parameter[@id="t"]/timerange')
     )
   
   @property
-  def min_temperature(self) -> Iterable[MinTemperature]:
-    """Iterable[:class:`MinTemperature`]: This weather forecast's minimum temperature across various timeframes."""
+  def lowest_temperature(self) -> Iterable[LowestTemperature]:
+    """Iterable[:class:`LowestTemperature`]: This weather forecast's lowest temperature across various timeframes."""
     
     unit = 'C' if self._CustomizableUnit__unit == METRIC else 'F'
     
     return (
-      MinTemperature(
+      LowestTemperature(
         datetime.strptime(child.attrib['datetime'], '%Y%m%d%H%M'),
         float(child.find(f'./value[@unit="{unit}"]').text)
       ) for child in self.__inner.iterfind('./parameter[@id="tmin"]/timerange')
     )
   
   @property
-  def max_temperature(self) -> Iterable[MaxTemperature]:
-    """Iterable[:class:`MinTemperature`]: This weather forecast's maximum temperature across various timeframes."""
+  def highest_temperature(self) -> Iterable[HighestTemperature]:
+    """Iterable[:class:`LowestTemperature`]: This weather forecast's highest temperature across various timeframes."""
     
     unit = 'C' if self._CustomizableUnit__unit == METRIC else 'F'
     
     return (
-      MaxTemperature(
+      HighestTemperature(
         datetime.strptime(child.attrib['datetime'], '%Y%m%d%H%M'),
         float(child.find(f'./value[@unit="{unit}"]').text)
       ) for child in self.__inner.iterfind('./parameter[@id="tmax"]/timerange')
     )
   
   @property
   def hourly(self) -> Iterable[HourlyForecast]:
```

### Comparing `bmkg-1.0.1/bmkg.egg-info/PKG-INFO` & `bmkg-1.0.2/bmkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bmkg
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial Python wrapper for the BMKG (Meteorology, Climatology, and Geophysical Agency) API.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/bmkg
-Project-URL: download_url, https://github.com/null8626/bmkg/archive/1.0.1.tar.gz
+Project-URL: download_url, https://github.com/null8626/bmkg/archive/1.0.2.tar.gz
 Keywords: weather,bmkg,indonesia,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `bmkg-1.0.1/pyproject.toml` & `bmkg-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "bmkg"
-version = "1.0.1"
+version = "1.0.2"
 description = "Unofficial Python wrapper for the BMKG (Meteorology, Climatology, and Geophysical Agency) API."
 readme = "README.md"
 license = { text = "MIT" }
 authors = [{ name = "null8626" }]
 keywords = ["weather", "bmkg", "indonesia", "wrapper"]
 dependencies = ["aiohttp>=3.0.0"]
 classifiers = [
@@ -34,8 +34,8 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12"
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 repository = "https://github.com/null8626/bmkg"
-download_url = "https://github.com/null8626/bmkg/archive/1.0.1.tar.gz"
+download_url = "https://github.com/null8626/bmkg/archive/1.0.2.tar.gz"
```

