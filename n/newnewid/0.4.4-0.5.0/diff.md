# Comparing `tmp/newnewid-0.4.4.tar.gz` & `tmp/newnewid-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newnewid-0.4.4.tar", max compression
+gzip compressed data, was "newnewid-0.5.0.tar", max compression
```

## Comparing `newnewid-0.4.4.tar` & `newnewid-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1062 2023-04-16 07:35:23.533595 newnewid-0.4.4/LICENSE
--rw-r--r--   0        0        0    30709 2023-04-16 07:35:23.533595 newnewid-0.4.4/README.md
--rw-r--r--   0        0        0     1046 2023-04-16 07:35:23.533595 newnewid-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2586 2023-04-16 07:35:23.533595 newnewid-0.4.4/src/newnewid/__init__.py
--rw-r--r--   0        0        0     5901 2023-04-16 07:35:23.533595 newnewid-0.4.4/src/newnewid/cli.py
--rw-r--r--   0        0        0     5439 2023-04-16 07:35:23.533595 newnewid-0.4.4/src/newnewid/clock/uuid_clock.py
--rw-r--r--   0        0        0     3212 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/counter/counter.py
--rw-r--r--   0        0        0     2586 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_ietf_uuidrev_rfc4122bis_00/__init__.py
--rw-r--r--   0        0        0      704 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_ietf_uuidrev_rfc4122bis_00/nil_uuid_generator.py
--rw-r--r--   0        0        0     2586 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_ietf_uuidrev_rfc4122bis_01/__init__.py
--rw-r--r--   0        0        0     2586 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_ietf_uuidrev_rfc4122bis_02/__init__.py
--rw-r--r--   0        0        0     1075 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/__init__.py
--rw-r--r--   0        0        0     3831 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid6_generator.py
--rw-r--r--   0        0        0    12099 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid7_generator.py
--rw-r--r--   0        0        0     3880 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid8_generator.py
--rw-r--r--   0        0        0     1075 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_02/__init__.py
--rw-r--r--   0        0        0     1773 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/__init__.py
--rw-r--r--   0        0        0      704 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/max_uuid_generator.py
--rw-r--r--   0        0        0    11624 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/uuid7_generator.py
--rw-r--r--   0        0        0     2746 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/uuid8_generator.py
--rw-r--r--   0        0        0     1665 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_04/__init__.py
--rw-r--r--   0        0        0      488 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/exception/backward_uuid_exception.py
--rw-r--r--   0        0        0     8440 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/parser/uuid_parser.py
--rw-r--r--   0        0        0      952 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/random/pseudo_random_binary_generator.py
--rw-r--r--   0        0        0      482 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/random/pseudo_random_generator.py
--rw-r--r--   0        0        0      153 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/util/nodoc.py
--rw-r--r--   0        0        0     1738 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/util/specloader.py
--rw-r--r--   0        0        0     3077 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/uuidgenerator/clock_based_uuid_generator.py
--rw-r--r--   0        0        0     4099 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/uuidgenerator/gregorian_based_uuid_generator.py
--rw-r--r--   0        0        0      963 2023-04-16 07:35:23.537595 newnewid-0.4.4/src/newnewid/uuidgenerator/uuid_generator.py
--rw-r--r--   0        0        0    31113 1970-01-01 00:00:00.000000 newnewid-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-23 13:31:07.416880 newnewid-0.5.0/LICENSE
+-rw-r--r--   0        0        0    40282 2023-04-23 13:31:07.416880 newnewid-0.5.0/README.md
+-rw-r--r--   0        0        0     1069 2023-04-23 13:31:07.416880 newnewid-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2988 2023-04-23 13:31:07.416880 newnewid-0.5.0/src/newnewid/__init__.py
+-rw-r--r--   0        0        0     9129 2023-04-23 13:31:07.416880 newnewid-0.5.0/src/newnewid/cli.py
+-rw-r--r--   0        0        0     5527 2023-04-23 13:31:07.416880 newnewid-0.5.0/src/newnewid/clock/uuid_clock.py
+-rw-r--r--   0        0        0     3420 2023-04-23 13:31:07.416880 newnewid-0.5.0/src/newnewid/counter/counter.py
+-rw-r--r--   0        0        0     2524 2023-04-23 13:31:07.416880 newnewid-0.5.0/src/newnewid/draft_ietf_uuidrev_rfc4122bis_00/__init__.py
+-rw-r--r--   0        0        0      704 2023-04-23 13:31:07.416880 newnewid-0.5.0/src/newnewid/draft_ietf_uuidrev_rfc4122bis_00/nil_uuid_generator.py
+-rw-r--r--   0        0        0     2524 2023-04-23 13:31:07.416880 newnewid-0.5.0/src/newnewid/draft_ietf_uuidrev_rfc4122bis_01/__init__.py
+-rw-r--r--   0        0        0     2524 2023-04-23 13:31:07.416880 newnewid-0.5.0/src/newnewid/draft_ietf_uuidrev_rfc4122bis_02/__init__.py
+-rw-r--r--   0        0        0     2988 2023-04-23 13:31:07.416880 newnewid-0.5.0/src/newnewid/draft_ietf_uuidrev_rfc4122bis_03/__init__.py
+-rw-r--r--   0        0        0     1013 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/__init__.py
+-rw-r--r--   0        0        0     3831 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid6_generator.py
+-rw-r--r--   0        0        0    12107 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid7_generator.py
+-rw-r--r--   0        0        0     3880 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid8_generator.py
+-rw-r--r--   0        0        0     1013 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_02/__init__.py
+-rw-r--r--   0        0        0     1711 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/__init__.py
+-rw-r--r--   0        0        0      704 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/max_uuid_generator.py
+-rw-r--r--   0        0        0    18877 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/uuid7_generator.py
+-rw-r--r--   0        0        0     2746 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/uuid8_generator.py
+-rw-r--r--   0        0        0     1711 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_04/__init__.py
+-rw-r--r--   0        0        0      488 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/exception/backward_uuid_exception.py
+-rw-r--r--   0        0        0     8420 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/parser/uuid_parser.py
+-rw-r--r--   0        0        0     1695 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/random/pseudo_random_binary_generator.py
+-rw-r--r--   0        0        0      482 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/random/pseudo_random_generator.py
+-rw-r--r--   0        0        0      153 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/util/nodoc.py
+-rw-r--r--   0        0        0      825 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/util/specloader.py
+-rw-r--r--   0        0        0     3077 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/uuidgenerator/clock_based_uuid_generator.py
+-rw-r--r--   0        0        0     4107 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/uuidgenerator/gregorian_based_uuid_generator.py
+-rw-r--r--   0        0        0      963 2023-04-23 13:31:07.420880 newnewid-0.5.0/src/newnewid/uuidgenerator/uuid_generator.py
+-rw-r--r--   0        0        0    40686 1970-01-01 00:00:00.000000 newnewid-0.5.0/PKG-INFO
```

### Comparing `newnewid-0.4.4/LICENSE` & `newnewid-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `newnewid-0.4.4/pyproject.toml` & `newnewid-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 
 [tool.poetry]
 authors = ["quwac <53551867+quwac@users.noreply.github.com>"]
 description = ""
 name = "newnewid"
 packages = [{from = "src", include = "newnewid"}]
 readme = "README.md"
-version = "0.4.4"
+version = "0.5.0"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8-docstrings = "^1.7.0"
 pre-commit = "^3.2.2"
 pyproject-flake8 = "^6.0.0.post1"
 pytest = "^7.2.2"
+pytest-html = "^3.2.0"
 
 [tool.poetry.scripts]
 newnewid = "newnewid.cli:cli"
```

### Comparing `newnewid-0.4.4/src/newnewid/__init__.py` & `newnewid-0.5.0/src/newnewid/draft_ietf_uuidrev_rfc4122bis_00/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 from newnewid.draft_peabody_dispatch_new_uuid_format_03.uuid8_generator import (
     UUID8Generator,
     uuid8,
 )
 from newnewid.exception.backward_uuid_exception import BackwardUUIDException
 from newnewid.random.pseudo_random_binary_generator import PseudoRandomBinaryGenerator
 from newnewid.random.pseudo_random_generator import PseudoRandomGenerator
-from newnewid.util.specloader import UUIDSpec
 from newnewid.uuidgenerator.gregorian_based_uuid_generator import MacAddressGenerator
 from newnewid.uuidgenerator.uuid_generator import UUIDGenerator
 
 __all__ = [
     # Compatibility
     "NAMESPACE_DNS",
     "NAMESPACE_OID",
@@ -89,10 +88,9 @@
     "uuid8",
     "UUID8Generator",
     "BackwardUUIDException",
     "PseudoRandomBinaryGenerator",
     "Counter",
     "UUIDClock",
     "PseudoRandomGenerator",
-    "UUIDSpec",
     "MacAddressGenerator",
 ]
```

### Comparing `newnewid-0.4.4/src/newnewid/clock/uuid_clock.py` & `newnewid-0.5.0/src/newnewid/clock/uuid_clock.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,91 +4,91 @@
 
 
 class UUIDClock:
     """Clock for UUID."""
 
     GREGORIAN_OFFSET = 0x1B2_1DD_213_814_000
 
-    def time_ns(self) -> int:
-        """Get time in nanoseconds.
-
-        Returns:
-            int: Epoch time in nanoseconds.
-        """
-        return time.time_ns()
-
     # ----------------------------
     # epoch_*_seconds
     # ----------------------------
 
     def epoch_seconds(self) -> int:
         """Get time in seconds.
 
         Returns:
             int: Epoch time in seconds.
         """
-        return self.time_ns() // 1_000_000_000
+        return self.epoch_nano_seconds() // 1_000_000_000
 
     def epoch_milli_seconds(self) -> int:
         """Get time in milliseconds.
 
         Returns:
             int: Epoch time in milliseconds.
         """
-        return self.time_ns() // 1_000_000
+        return self.epoch_nano_seconds() // 1_000_000
+
+    def epoch_nano_seconds(self) -> int:
+        """Get time in nanoseconds.
+
+        Returns:
+            int: Epoch time in nanoseconds.
+        """
+        return time.time_ns()
 
     def epoch_100_nano_seconds(self) -> int:
         """Get time in 100 nanoseconds.
 
         Returns:
             int: Epoch time in 100 nanoseconds.
         """
-        return self.time_ns() // 100
+        return self.epoch_nano_seconds() // 100
 
     # ----------------------------
     # gregorian
     # ----------------------------
 
     def gregorian_100_nano_seconds(self) -> int:
         """Get time in 100 nanoseconds since Gregorian epoch.
 
         Returns:
             int: Time in 100 nanoseconds since Gregorian epoch.
         """
-        return self.time_ns() // 100 + self.GREGORIAN_OFFSET
+        return self.epoch_nano_seconds() // 100 + self.GREGORIAN_OFFSET
 
     # ----------------------------
     # epoch_36_bits_seconds_with_*_bits_*_seconds
     # ----------------------------
 
     def epoch_36_bits_seconds_with_12_bits_milli_seconds(self) -> int:
         """Get time in 12 bits milliseconds since epoch.
 
         Returns:
             int: Time in 12 bits milliseconds since epoch.
         """
-        seconds, milli_part = divmod(self.time_ns() // 1_000_000, 1_000)
+        seconds, milli_part = divmod(self.epoch_nano_seconds() // 1_000_000, 1_000)
         return ((seconds & 0x000F_FFFF_FFFF) << 12) | milli_part
 
     def epoch_36_bits_seconds_with_24_bits_micro_seconds(self) -> int:
         """Get time in 24 bits microseconds since epoch.
 
         Returns:
             int: Time in 24 bits microseconds since epoch.
         """
-        seconds, micro_part = divmod(self.time_ns() // 1_000, 1_000_000)
+        seconds, micro_part = divmod(self.epoch_nano_seconds() // 1_000, 1_000_000)
         return ((seconds & 0x000F_FFFF_FFFF) << 24) | micro_part
 
     def epoch_36_bits_seconds_with_38_bits_nano_seconds(self) -> int:
         """Get time in 38 bits nanoseconds since epoch.
 
         Returns:
             int: Time in 38 bits nanoseconds since epoch.
         """
-        seconds, nano_part = divmod(self.time_ns(), 1_000_000_000)
+        seconds, nano_part = divmod(self.epoch_nano_seconds(), 1_000_000_000)
         return ((seconds & 0x000F_FFFF_FFFF) << 38) | nano_part
 
     # ----------------------------
     # converter
     # ----------------------------
 
     @classmethod
```

### Comparing `newnewid-0.4.4/src/newnewid/counter/counter.py` & `newnewid-0.5.0/src/newnewid/counter/counter.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,77 +9,81 @@
     This class manages a counter.
 
     The counter is incremented when the same timestamp is given and reset when the timestamp is changed.
     """
 
     def __init__(
         self,
-        bits_length: int,
+        counter_bits_length: int,
         max_increment_bits_length: Optional[int],
         pseudo_random_generator: PseudoRandomGenerator,
         initial_timestamp: Optional[int],
         initial_counter: Optional[int],
     ) -> None:
         """Create counter.
 
         Args:
-            bits_length (int): Number of bits of the counter.
+            counter_bits_length (int): Number of bits of the counter.
             max_increment_bits_length (Optional[int]): Maximum number of bits of the increment. Maximum value is 2^max_increment_bits_length - 1.
             pseudo_random_generator (PseudoRandomGenerator): Pseudo random generator.
             initial_last_timestamp (Optional[int]): Initial timestamp.
             initial_counter (Optional[int]): Initial counter value.
         """
-        if bits_length > 0:
-            assert max_increment_bits_length is not None, "increment_bits_length must be specified"
+        if counter_bits_length > 0:
             assert (
-                bits_length >= max_increment_bits_length
-            ), f"mask_bits_length must be greater than or equal to increment_bits_length, not {bits_length} < {max_increment_bits_length}"
+                max_increment_bits_length is not None
+            ), "max_increment_bits_length must be specified"
+            assert (
+                counter_bits_length >= max_increment_bits_length
+            ), f"counter_bits_length must be greater than or equal to max_increment_bits_length, not {counter_bits_length} < {max_increment_bits_length}"
             assert (
                 max_increment_bits_length >= 1
-            ), f"increment_bits_length must be greater than or equal to 1, not {max_increment_bits_length}"
+            ), f"max_increment_bits_length must be greater than or equal to 1, not {max_increment_bits_length}"
 
-        self.bits_length = bits_length
-        self.mask: int = (1 << bits_length) - 1
+        self.counter_bits_length = counter_bits_length
+        self.mask: int = (1 << counter_bits_length) - 1
         self.max_increment_bits_length = max_increment_bits_length
         self._pseudo_random_generator = pseudo_random_generator
 
         self.last_timestamp = initial_timestamp
         if initial_counter is None:
-            if bits_length > 0:
-                self.counter = self._get_counter_reset_value()
+            if counter_bits_length > 0:
+                self.counter = None
             else:
                 self.counter = 0
         else:
             self.counter = initial_counter
 
     def _get_counter_reset_value(self) -> int:
-        return self._pseudo_random_generator.generate(self.bits_length - 1, "counter-reset")
+        return self._pseudo_random_generator.generate(self.counter_bits_length - 1, "counter-reset")
 
     def get_next(self, timestamp: int) -> int:
         """Ge next counter value.
 
         Args:
             timestamp (int): Current timestamp.
 
         Returns:
             int: counter value.
         """
-        if self.bits_length == 0:
+        if self.counter_bits_length == 0:
             return 0
 
         if self.last_timestamp is not None and timestamp <= self.last_timestamp:
+            if self.counter is None:
+                self.counter = self._get_counter_reset_value()
+
             if self.max_increment_bits_length == 1:
                 increment = 1
             else:
                 assert self.max_increment_bits_length is not None
                 increment = 0
                 while increment <= 0:
                     increment = self._pseudo_random_generator.generate(
                         self.max_increment_bits_length, "counter-increment"
                     )
-
             new_counter_raw = self.counter + increment
         else:
             new_counter_raw = self._get_counter_reset_value()
         self.counter = new_counter_raw & self.mask
         self.last_timestamp = timestamp
         return self.counter
```

### Comparing `newnewid-0.4.4/src/newnewid/draft_ietf_uuidrev_rfc4122bis_00/__init__.py` & `newnewid-0.5.0/src/newnewid/draft_ietf_uuidrev_rfc4122bis_01/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 from newnewid.draft_peabody_dispatch_new_uuid_format_03.uuid8_generator import (
     UUID8Generator,
     uuid8,
 )
 from newnewid.exception.backward_uuid_exception import BackwardUUIDException
 from newnewid.random.pseudo_random_binary_generator import PseudoRandomBinaryGenerator
 from newnewid.random.pseudo_random_generator import PseudoRandomGenerator
-from newnewid.util.specloader import UUIDSpec
 from newnewid.uuidgenerator.gregorian_based_uuid_generator import MacAddressGenerator
 from newnewid.uuidgenerator.uuid_generator import UUIDGenerator
 
 __all__ = [
     # Compatibility
     "NAMESPACE_DNS",
     "NAMESPACE_OID",
@@ -89,10 +88,9 @@
     "uuid8",
     "UUID8Generator",
     "BackwardUUIDException",
     "PseudoRandomBinaryGenerator",
     "Counter",
     "UUIDClock",
     "PseudoRandomGenerator",
-    "UUIDSpec",
     "MacAddressGenerator",
 ]
```

### Comparing `newnewid-0.4.4/src/newnewid/draft_ietf_uuidrev_rfc4122bis_00/nil_uuid_generator.py` & `newnewid-0.5.0/src/newnewid/draft_ietf_uuidrev_rfc4122bis_00/nil_uuid_generator.py`

 * *Files identical despite different names*

### Comparing `newnewid-0.4.4/src/newnewid/draft_ietf_uuidrev_rfc4122bis_01/__init__.py` & `newnewid-0.5.0/src/newnewid/draft_ietf_uuidrev_rfc4122bis_02/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 from newnewid.draft_peabody_dispatch_new_uuid_format_03.uuid8_generator import (
     UUID8Generator,
     uuid8,
 )
 from newnewid.exception.backward_uuid_exception import BackwardUUIDException
 from newnewid.random.pseudo_random_binary_generator import PseudoRandomBinaryGenerator
 from newnewid.random.pseudo_random_generator import PseudoRandomGenerator
-from newnewid.util.specloader import UUIDSpec
 from newnewid.uuidgenerator.gregorian_based_uuid_generator import MacAddressGenerator
 from newnewid.uuidgenerator.uuid_generator import UUIDGenerator
 
 __all__ = [
     # Compatibility
     "NAMESPACE_DNS",
     "NAMESPACE_OID",
@@ -89,10 +88,9 @@
     "uuid8",
     "UUID8Generator",
     "BackwardUUIDException",
     "PseudoRandomBinaryGenerator",
     "Counter",
     "UUIDClock",
     "PseudoRandomGenerator",
-    "UUIDSpec",
     "MacAddressGenerator",
 ]
```

### Comparing `newnewid-0.4.4/src/newnewid/draft_ietf_uuidrev_rfc4122bis_02/__init__.py` & `newnewid-0.5.0/src/newnewid/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,27 +32,29 @@
 )
 from newnewid.draft_peabody_dispatch_new_uuid_format_03.uuid7_generator import (
     METHOD_0_NO_COUNTER,
     METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_12,
     METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_26,
     METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_42,
     METHOD_2_MONOTONIC_RANDOM_62_BITS,
+    METHOD_3_RERANDOMIZE_UNTIL_MONOTONIC,
+    METHOD_4_REPLACE_LEFT_MOST_RANDOM_BITS_WITH_INCREASED_CLOCK_PRECISION_12_BITS,
+    METHOD_4_REPLACE_LEFT_MOST_RANDOM_BITS_WITH_INCREASED_CLOCK_PRECISION_12_BITS_WITH_COUNTER_14_BITS,
     UUID7Generator,
     UUID7Option,
     ulid_compatible,
     uuid7,
 )
 from newnewid.draft_peabody_dispatch_new_uuid_format_03.uuid8_generator import (
     UUID8Generator,
     uuid8,
 )
 from newnewid.exception.backward_uuid_exception import BackwardUUIDException
 from newnewid.random.pseudo_random_binary_generator import PseudoRandomBinaryGenerator
 from newnewid.random.pseudo_random_generator import PseudoRandomGenerator
-from newnewid.util.specloader import UUIDSpec
 from newnewid.uuidgenerator.gregorian_based_uuid_generator import MacAddressGenerator
 from newnewid.uuidgenerator.uuid_generator import UUIDGenerator
 
 __all__ = [
     # Compatibility
     "NAMESPACE_DNS",
     "NAMESPACE_OID",
@@ -78,21 +80,23 @@
     "uuid6",
     "UUID6Generator",
     "METHOD_0_NO_COUNTER",
     "METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_12",
     "METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_26",
     "METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_42",
     "METHOD_2_MONOTONIC_RANDOM_62_BITS",
+    "METHOD_3_RERANDOMIZE_UNTIL_MONOTONIC",
+    "METHOD_4_REPLACE_LEFT_MOST_RANDOM_BITS_WITH_INCREASED_CLOCK_PRECISION_12_BITS",
+    "METHOD_4_REPLACE_LEFT_MOST_RANDOM_BITS_WITH_INCREASED_CLOCK_PRECISION_12_BITS_WITH_COUNTER_14_BITS",
     "UUID7Generator",
     "UUID7Option",
     "ulid_compatible",
     "uuid7",
     "uuid8",
     "UUID8Generator",
     "BackwardUUIDException",
     "PseudoRandomBinaryGenerator",
     "Counter",
     "UUIDClock",
     "PseudoRandomGenerator",
-    "UUIDSpec",
     "MacAddressGenerator",
 ]
```

### Comparing `newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/__init__.py` & `newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 )
 from newnewid.draft_peabody_dispatch_new_uuid_format_01.uuid8_generator import (
     UUID8Generator,
     uuid8,
 )
 from newnewid.exception.backward_uuid_exception import BackwardUUIDException
 from newnewid.random.pseudo_random_binary_generator import PseudoRandomBinaryGenerator
-from newnewid.util.specloader import UUIDSpec
 from newnewid.uuidgenerator.gregorian_based_uuid_generator import MacAddressGenerator
 from newnewid.uuidgenerator.uuid_generator import UUIDGenerator
 
 __all__ = [
     "UUIDGenerator",
     "uuid6",
     "UUID6Generator",
@@ -26,10 +25,9 @@
     "UUID7Generator",
     "uuid8",
     "UUID8Generator",
     "BackwardUUIDException",
     "PseudoRandomBinaryGenerator",
     "Counter",
     "UUIDClock",
-    "UUIDSpec",
     "MacAddressGenerator",
 ]
```

### Comparing `newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid6_generator.py` & `newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid6_generator.py`

 * *Files identical despite different names*

### Comparing `newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid7_generator.py` & `newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid7_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         last_timestamp: Optional[int] = None
         last_counter: Optional[int] = None
         if last_uuid:
             assert last_uuid.version == 7, f"last_uuid must be version 7, not {last_uuid.version}"
             (last_timestamp, last_counter) = self.__class__._parse_last_uuid(last_uuid, precision)
 
         self._counter = Counter(
-            bits_length=self.cbl,
+            counter_bits_length=self.cbl,
             max_increment_bits_length=1,
             pseudo_random_generator=self._pseudo_random_generator,
             initial_timestamp=last_timestamp,
             initial_counter=last_counter,
         )
         self._pseudo_random_binary_generator = PseudoRandomBinaryGenerator(
             self.random_bits, self._pseudo_random_generator
```

### Comparing `newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid8_generator.py` & `newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_01/uuid8_generator.py`

 * *Files identical despite different names*

### Comparing `newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_02/__init__.py` & `newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_02/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 )
 from newnewid.draft_peabody_dispatch_new_uuid_format_01.uuid8_generator import (
     UUID8Generator,
     uuid8,
 )
 from newnewid.exception.backward_uuid_exception import BackwardUUIDException
 from newnewid.random.pseudo_random_binary_generator import PseudoRandomBinaryGenerator
-from newnewid.util.specloader import UUIDSpec
 from newnewid.uuidgenerator.gregorian_based_uuid_generator import MacAddressGenerator
 from newnewid.uuidgenerator.uuid_generator import UUIDGenerator
 
 __all__ = [
     "UUIDGenerator",
     "uuid6",
     "UUID6Generator",
@@ -26,10 +25,9 @@
     "UUID7Generator",
     "uuid8",
     "UUID8Generator",
     "BackwardUUIDException",
     "PseudoRandomBinaryGenerator",
     "Counter",
     "UUIDClock",
-    "UUIDSpec",
     "MacAddressGenerator",
 ]
```

### Comparing `newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/__init__.py` & `newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 )
 from newnewid.draft_peabody_dispatch_new_uuid_format_03.uuid8_generator import (
     UUID8Generator,
     uuid8,
 )
 from newnewid.exception.backward_uuid_exception import BackwardUUIDException
 from newnewid.random.pseudo_random_binary_generator import PseudoRandomBinaryGenerator
-from newnewid.util.specloader import UUIDSpec
 from newnewid.uuidgenerator.gregorian_based_uuid_generator import MacAddressGenerator
 from newnewid.uuidgenerator.uuid_generator import UUIDGenerator
 
 __all__ = [
     "BackwardUUIDException",
     "Counter",
     "MacAddressGenerator",
@@ -47,9 +46,8 @@
     "uuid7",
     "UUID7Generator",
     "UUID7Option",
     "uuid8",
     "UUID8Generator",
     "UUIDClock",
     "UUIDGenerator",
-    "UUIDSpec",
 ]
```

### Comparing `newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/max_uuid_generator.py` & `newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/max_uuid_generator.py`

 * *Files identical despite different names*

### Comparing `newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/uuid8_generator.py` & `newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_03/uuid8_generator.py`

 * *Files identical despite different names*

### Comparing `newnewid-0.4.4/src/newnewid/draft_peabody_dispatch_new_uuid_format_04/__init__.py` & `newnewid-0.5.0/src/newnewid/draft_peabody_dispatch_new_uuid_format_04/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,47 +7,47 @@
 from newnewid.draft_peabody_dispatch_new_uuid_format_03.max_uuid_generator import (
     MaxUUIDGenerator,
     max_uuid,
 )
 from newnewid.draft_peabody_dispatch_new_uuid_format_03.uuid7_generator import (
     METHOD_0_NO_COUNTER,
     METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_12,
+    METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_26,
     METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_42,
     METHOD_2_MONOTONIC_RANDOM_62_BITS,
     UUID7Generator,
     UUID7Option,
     ulid_compatible,
     uuid7,
 )
 from newnewid.draft_peabody_dispatch_new_uuid_format_03.uuid8_generator import (
     UUID8Generator,
     uuid8,
 )
 from newnewid.exception.backward_uuid_exception import BackwardUUIDException
 from newnewid.random.pseudo_random_binary_generator import PseudoRandomBinaryGenerator
-from newnewid.util.specloader import UUIDSpec
 from newnewid.uuidgenerator.gregorian_based_uuid_generator import MacAddressGenerator
 from newnewid.uuidgenerator.uuid_generator import UUIDGenerator
 
 __all__ = [
     "BackwardUUIDException",
     "Counter",
     "MacAddressGenerator",
     "max_uuid",
     "MaxUUIDGenerator",
     "METHOD_0_NO_COUNTER",
     "METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_12",
+    "METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_26",
     "METHOD_1_FIXED_LENGTH_DEDICATED_COUNTER_BITS_42",
     "METHOD_2_MONOTONIC_RANDOM_62_BITS",
     "PseudoRandomBinaryGenerator",
     "ulid_compatible",
     "uuid6",
     "UUID6Generator",
     "uuid7",
     "UUID7Generator",
     "UUID7Option",
     "uuid8",
     "UUID8Generator",
     "UUIDClock",
     "UUIDGenerator",
-    "UUIDSpec",
 ]
```

### Comparing `newnewid-0.4.4/src/newnewid/parser/uuid_parser.py` & `newnewid-0.5.0/src/newnewid/parser/uuid_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict
 from uuid import UUID
 
 from newnewid.clock.uuid_clock import UUIDClock
-from newnewid.util.specloader import UUIDSpec, load_modules
+from newnewid.util.specloader import load_modules
 from newnewid.uuidgenerator.uuid_generator import UUIDGenerator
 
 
 class _OtherUUIDParser:
     @classmethod
     def parse_uuid1(cls, uuid: UUID, **kwargs: Any) -> Dict[str, Any]:
         """Parse UUIDv1."""
@@ -157,20 +157,20 @@
             "sha1_mid": sha1_mid,
             "var": var,
             "sha1_low": sha1_low,
             "sha1": sha1,
         }
 
 
-def parse(uuid: UUID, spec: UUIDSpec = "latest", **kwargs) -> Dict[str, Any]:
+def parse(uuid: UUID, spec: str = "latest", **kwargs) -> Dict[str, Any]:
     """Parse UUID.
 
     Args:
         uuid (UUID): UUID.
-        spec (UUIDSpec, optional): UUID spec. Defaults to "latest".
+        spec (str, optional): UUID spec. Defaults to "latest".
 
     Returns:
         Dict[str, Any]: Parsed UUID.
     """
     uuid_int = uuid.int
     version = UUIDGenerator.get_version(uuid)
```

### Comparing `newnewid-0.4.4/src/newnewid/uuidgenerator/clock_based_uuid_generator.py` & `newnewid-0.5.0/src/newnewid/uuidgenerator/clock_based_uuid_generator.py`

 * *Files identical despite different names*

### Comparing `newnewid-0.4.4/src/newnewid/uuidgenerator/gregorian_based_uuid_generator.py` & `newnewid-0.5.0/src/newnewid/uuidgenerator/gregorian_based_uuid_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 parsed["time_low"],
             )
 
             last_timestamp = time_high << 20 | time_mid << 4 | time_low
             last_counter = parsed["clock_seq"]
 
         self._counter = Counter(
-            bits_length=14,
+            counter_bits_length=14,
             max_increment_bits_length=1,
             pseudo_random_generator=self._pseudo_random_generator,
             initial_timestamp=last_timestamp,
             initial_counter=last_counter,
         )
         if uses_mac_address:
             self._pseudo_random_binary_generator = MacAddressGenerator()
```

### Comparing `newnewid-0.4.4/src/newnewid/uuidgenerator/uuid_generator.py` & `newnewid-0.5.0/src/newnewid/uuidgenerator/uuid_generator.py`

 * *Files identical despite different names*

