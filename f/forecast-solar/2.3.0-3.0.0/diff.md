# Comparing `tmp/forecast_solar-2.3.0.tar.gz` & `tmp/forecast_solar-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecast_solar-2.3.0.tar", last modified: Wed Sep 14 18:34:18 2022, max compression
+gzip compressed data, was "forecast_solar-3.0.0.tar", last modified: Sun Apr 23 18:06:29 2023, max compression
```

## Comparing `forecast_solar-2.3.0.tar` & `forecast_solar-3.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:34:18.944916 forecast_solar-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-09-14 18:34:10.000000 forecast_solar-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6526 2022-09-14 18:34:18.944916 forecast_solar-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5743 2022-09-14 18:34:10.000000 forecast_solar-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:34:18.944916 forecast_solar-2.3.0/forecast_solar/
--rw-r--r--   0 runner    (1001) docker     (121)     5793 2022-09-14 18:34:10.000000 forecast_solar-2.3.0/forecast_solar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-09-14 18:34:10.000000 forecast_solar-2.3.0/forecast_solar/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6566 2022-09-14 18:34:10.000000 forecast_solar-2.3.0/forecast_solar/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:34:18.944916 forecast_solar-2.3.0/forecast_solar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6526 2022-09-14 18:34:18.000000 forecast_solar-2.3.0/forecast_solar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-09-14 18:34:18.000000 forecast_solar-2.3.0/forecast_solar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 18:34:18.000000 forecast_solar-2.3.0/forecast_solar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 18:34:18.000000 forecast_solar-2.3.0/forecast_solar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-14 18:34:18.000000 forecast_solar-2.3.0/forecast_solar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-14 18:34:18.000000 forecast_solar-2.3.0/forecast_solar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-09-14 18:34:18.944916 forecast_solar-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-09-14 18:34:10.000000 forecast_solar-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:06:29.886314 forecast_solar-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-23 18:06:29.886314 forecast_solar-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:06:29.882314 forecast_solar-3.0.0/forecast_solar/
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/forecast_solar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/forecast_solar/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/forecast_solar/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:06:29.886314 forecast_solar-3.0.0/forecast_solar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 18:06:29.000000 forecast_solar-3.0.0/forecast_solar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-23 18:06:29.886314 forecast_solar-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-23 18:06:19.000000 forecast_solar-3.0.0/setup.py
```

### Comparing `forecast_solar-2.3.0/LICENSE` & `forecast_solar-3.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-Copyright (c) 2021-2022 Klaas Schoute
+Copyright (c) 2021-2023 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `forecast_solar-2.3.0/PKG-INFO` & `forecast_solar-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecast_solar
-Version: 2.3.0
+Version: 3.0.0
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/klaasnicolaas/forecast_solar
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 License: MIT license
 Keywords: forecast,solar,power,energy,api,async,client
 Classifier: Framework :: AsyncIO
@@ -51,14 +51,15 @@
 This library returns a lot of different data, based on the API:
 
 ### Energy
 
 - Total Estimated Energy Production - today/tomorrow (kWh)
 - Estimated Energy Production - This Hour (kWh)
 - Estimated Energy Production - Next Hour (kWh)
+- Estimated Energy Production - Remaining today (kWh)
 
 ### Power
 
 - Highest Power Peak Time - Today (datetime)
 - Highest Power Peak Time - Tomorrow (datetime)
 - Estimated Power Production - Now (W)
 - Estimated Power Production - Next Hour (W)
@@ -121,15 +122,15 @@
 
 Thank you for being involved! :heart_eyes:
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2022 Klaas Schoute
+Copyright (c) 2021-2023 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -146,15 +147,15 @@
 SOFTWARE.
 
 <!-- LINKS -->
 [forecast-horizon]: https://doc.forecast.solar/doku.php?id=api#horizon
 [forecast-damping]: https://doc.forecast.solar/doku.php?id=damping
 
 <!-- MARKDOWN LINKS & IMAGES -->
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2022.svg?style=for-the-badge
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge
 [contributors-shield]: https://img.shields.io/github/contributors/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [contributors-url]: https://github.com/home-assistant-libs/forecast_solar/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [forks-url]: https://github.com/home-assistant-libs/forecast_solar/network/members
 [stars-shield]: https://img.shields.io/github/stars/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [stars-url]: https://github.com/home-assistant-libs/forecast_solar/stargazers
 [issues-shield]: https://img.shields.io/github/issues/home-assistant-libs/forecast_solar.svg?style=for-the-badge
```

### Comparing `forecast_solar-2.3.0/README.md` & `forecast_solar-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 This library returns a lot of different data, based on the API:
 
 ### Energy
 
 - Total Estimated Energy Production - today/tomorrow (kWh)
 - Estimated Energy Production - This Hour (kWh)
 - Estimated Energy Production - Next Hour (kWh)
+- Estimated Energy Production - Remaining today (kWh)
 
 ### Power
 
 - Highest Power Peak Time - Today (datetime)
 - Highest Power Peak Time - Tomorrow (datetime)
 - Estimated Power Production - Now (W)
 - Estimated Power Production - Next Hour (W)
@@ -101,15 +102,15 @@
 
 Thank you for being involved! :heart_eyes:
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2022 Klaas Schoute
+Copyright (c) 2021-2023 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -126,15 +127,15 @@
 SOFTWARE.
 
 <!-- LINKS -->
 [forecast-horizon]: https://doc.forecast.solar/doku.php?id=api#horizon
 [forecast-damping]: https://doc.forecast.solar/doku.php?id=damping
 
 <!-- MARKDOWN LINKS & IMAGES -->
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2022.svg?style=for-the-badge
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge
 [contributors-shield]: https://img.shields.io/github/contributors/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [contributors-url]: https://github.com/home-assistant-libs/forecast_solar/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [forks-url]: https://github.com/home-assistant-libs/forecast_solar/network/members
 [stars-shield]: https://img.shields.io/github/stars/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [stars-url]: https://github.com/home-assistant-libs/forecast_solar/stargazers
 [issues-shield]: https://img.shields.io/github/issues/home-assistant-libs/forecast_solar.svg?style=for-the-badge
```

### Comparing `forecast_solar-2.3.0/forecast_solar/__init__.py` & `forecast_solar-3.0.0/forecast_solar/__init__.py`

 * *Files identical despite different names*

### Comparing `forecast_solar-2.3.0/forecast_solar/exceptions.py` & `forecast_solar-3.0.0/forecast_solar/exceptions.py`

 * *Files identical despite different names*

### Comparing `forecast_solar-2.3.0/forecast_solar/models.py` & `forecast_solar-3.0.0/forecast_solar/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,35 +22,55 @@
         if timestamp > at:
             return value
         value = cur_value
 
     return None
 
 
+def _interval_value_sum(
+    interval_begin: datetime, interval_end: datetime, data: dict[datetime, int]
+) -> int:
+    """Return the sum of values in interval."""
+
+    total = 0
+
+    for timestamp, wh in data.items():
+        # Skip all until this hour
+        if timestamp < interval_begin:
+            continue
+
+        if timestamp >= interval_end:
+            break
+
+        total += wh
+
+    return total
+
+
 class AccountType(str, Enum):
     """Enumeration representing the Forecast.Solar account type."""
 
     PUBLIC = "public"
     PERSONAL = "personal"
     PROFESSIONAL = "professional"
 
 
 @dataclass
 class Estimate:
     """Object holding estimate forecast results from Forecast.Solar.
 
     Attributes:
+        watts: Estimated solar power output per time period.
+        wh_period: Estimated solar energy production differences per hour.
         wh_days: Estimated solar energy production per day.
-        wh_hours: Estimated solar energy production per hour.
-        watts: Estimated solar power output per hour.
     """
 
-    wh_days: dict[datetime, int]
-    wh_hours: dict[datetime, int]
     watts: dict[datetime, int]
+    wh_period: dict[datetime, int]
+    wh_days: dict[datetime, int]
     api_rate_limit: int
     api_timezone: str
 
     @property
     def timezone(self) -> str:
         """Return API timezone information."""
         return self.api_timezone
@@ -71,14 +91,24 @@
 
     @property
     def energy_production_tomorrow(self) -> int:
         """Return estimated energy produced today."""
         return self.day_production(self.now().date() + timedelta(days=1))
 
     @property
+    def energy_production_today_remaining(self) -> int:
+        """Return estimated energy produced in rest of today."""
+        return _interval_value_sum(
+            self.now(),
+            self.now().replace(hour=0, minute=0, second=0, microsecond=0)
+            + timedelta(days=1),
+            self.wh_period,
+        )
+
+    @property
     def power_production_now(self) -> int:
         """Return estimated power production right now."""
         return self.power_production_at_time(self.now())
 
     @property
     def power_highest_peak_time_today(self) -> datetime:
         """Return datetime with highest power production moment today."""
@@ -88,15 +118,19 @@
     def power_highest_peak_time_tomorrow(self) -> datetime:
         """Return datetime with highest power production moment tomorrow."""
         return self.peak_production_time(self.now().date() + timedelta(days=1))
 
     @property
     def energy_current_hour(self) -> int:
         """Return the estimated energy production for the current hour."""
-        return _timed_value(self.now(), self.wh_hours) or 0
+        return _interval_value_sum(
+            self.now().replace(minute=0, second=0, microsecond=0),
+            self.now().replace(minute=0, second=0, microsecond=0) + timedelta(hours=1),
+            self.wh_period,
+        )
 
     def day_production(self, specific_date: date) -> int:
         """Return the day production."""
         for timestamp, production in self.wh_days.items():
             if timestamp.date() == specific_date:
                 return production
 
@@ -121,66 +155,44 @@
 
     def power_production_at_time(self, time: datetime) -> int:
         """Return estimated power production at a specific time."""
         return _timed_value(time, self.watts) or 0
 
     def sum_energy_production(self, period_hours: int) -> int:
         """Return the sum of the energy production."""
-        now = self.now().replace(minute=59, second=59)
+        now = self.now().replace(minute=59, second=59, microsecond=999)
         until = now + timedelta(hours=period_hours)
 
-        total = 0
-
-        for timestamp, wh in self.wh_hours.items():
-            # Skip all dates until this hour
-            if timestamp < now:
-                continue
-
-            if timestamp > until:
-                break
-
-            total += wh
-
-        return total
+        return _interval_value_sum(now, until, self.wh_period)
 
     @classmethod
     def from_dict(cls, data: dict[str, Any]) -> Estimate:
         """Return a Estimate object from a Forecast.Solar API response.
 
         Converts a dictionary, obtained from the Forecast.Solar API into
         a Estimate object.
 
         Args:
             data: The estimate response from the Forecast.Solar API.
 
         Returns:
             An Estimate object.
         """
-        previous_value = 0
-        wh_hours = {}
-
-        for timestamp, energy in data["result"]["watt_hours"].items():
-            timestamp = datetime.fromisoformat(timestamp)
-
-            # If we get a reset
-            if energy < previous_value:
-                previous_value = 0
-
-            wh_hours[timestamp] = energy - previous_value
-            previous_value = energy
-
         return cls(
+            watts={
+                datetime.fromisoformat(d): w for d, w in data["result"]["watts"].items()
+            },
+            wh_period={
+                datetime.fromisoformat(d): e
+                for d, e in data["result"]["watt_hours_period"].items()
+            },
             wh_days={
                 datetime.fromisoformat(d): e
                 for d, e in data["result"]["watt_hours_day"].items()
             },
-            wh_hours=wh_hours,
-            watts={
-                datetime.fromisoformat(d): w for d, w in data["result"]["watts"].items()
-            },
             api_rate_limit=data["message"]["ratelimit"]["limit"],
             api_timezone=data["message"]["info"]["timezone"],
         )
 
 
 @dataclass
 class Ratelimit:
```

### Comparing `forecast_solar-2.3.0/forecast_solar.egg-info/PKG-INFO` & `forecast_solar-3.0.0/forecast_solar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecast-solar
-Version: 2.3.0
+Version: 3.0.0
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/klaasnicolaas/forecast_solar
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 License: MIT license
 Keywords: forecast,solar,power,energy,api,async,client
 Classifier: Framework :: AsyncIO
@@ -51,14 +51,15 @@
 This library returns a lot of different data, based on the API:
 
 ### Energy
 
 - Total Estimated Energy Production - today/tomorrow (kWh)
 - Estimated Energy Production - This Hour (kWh)
 - Estimated Energy Production - Next Hour (kWh)
+- Estimated Energy Production - Remaining today (kWh)
 
 ### Power
 
 - Highest Power Peak Time - Today (datetime)
 - Highest Power Peak Time - Tomorrow (datetime)
 - Estimated Power Production - Now (W)
 - Estimated Power Production - Next Hour (W)
@@ -121,15 +122,15 @@
 
 Thank you for being involved! :heart_eyes:
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2022 Klaas Schoute
+Copyright (c) 2021-2023 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -146,15 +147,15 @@
 SOFTWARE.
 
 <!-- LINKS -->
 [forecast-horizon]: https://doc.forecast.solar/doku.php?id=api#horizon
 [forecast-damping]: https://doc.forecast.solar/doku.php?id=damping
 
 <!-- MARKDOWN LINKS & IMAGES -->
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2022.svg?style=for-the-badge
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge
 [contributors-shield]: https://img.shields.io/github/contributors/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [contributors-url]: https://github.com/home-assistant-libs/forecast_solar/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [forks-url]: https://github.com/home-assistant-libs/forecast_solar/network/members
 [stars-shield]: https://img.shields.io/github/stars/home-assistant-libs/forecast_solar.svg?style=for-the-badge
 [stars-url]: https://github.com/home-assistant-libs/forecast_solar/stargazers
 [issues-shield]: https://img.shields.io/github/issues/home-assistant-libs/forecast_solar.svg?style=for-the-badge
```

### Comparing `forecast_solar-2.3.0/setup.py` & `forecast_solar-3.0.0/setup.py`

 * *Files identical despite different names*

