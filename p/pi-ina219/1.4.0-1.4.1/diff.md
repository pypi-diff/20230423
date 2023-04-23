# Comparing `tmp/pi_ina219-1.4.0-py2.py3-none-any.whl.zip` & `tmp/pi_ina219-1.4.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9936 bytes, number of entries: 6
--rw-r--r--  2.0 unx    16651 b- defN 20-Dec-19 01:47 ina219.py
--rw-r--r--  2.0 unx     1064 b- defN 20-Dec-19 01:53 pi_ina219-1.4.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    12608 b- defN 20-Dec-19 01:53 pi_ina219-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-Dec-19 01:53 pi_ina219-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 20-Dec-19 01:53 pi_ina219-1.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      467 b- defN 20-Dec-19 01:53 pi_ina219-1.4.0.dist-info/RECORD
-6 files, 30907 bytes uncompressed, 9096 bytes compressed:  70.6%
+Zip file size: 10125 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    16651 b- defN 23-Apr-18 08:09 ina219.py
+-rw-r--r--  2.0 unx     1064 b- defN 23-Apr-23 02:58 pi_ina219-1.4.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    13385 b- defN 23-Apr-23 02:58 pi_ina219-1.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 02:58 pi_ina219-1.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-23 02:58 pi_ina219-1.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      467 b- defN 23-Apr-23 02:58 pi_ina219-1.4.1.dist-info/RECORD
+6 files, 31684 bytes uncompressed, 9285 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ina219.py
 Comment: 
 
-Filename: pi_ina219-1.4.0.dist-info/LICENSE.md
+Filename: pi_ina219-1.4.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: pi_ina219-1.4.0.dist-info/METADATA
+Filename: pi_ina219-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: pi_ina219-1.4.0.dist-info/WHEEL
+Filename: pi_ina219-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: pi_ina219-1.4.0.dist-info/top_level.txt
+Filename: pi_ina219-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pi_ina219-1.4.0.dist-info/RECORD
+Filename: pi_ina219-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pi_ina219-1.4.0.dist-info/LICENSE.md` & `pi_ina219-1.4.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pi_ina219-1.4.0.dist-info/METADATA` & `pi_ina219-1.4.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-ina219
-Version: 1.4.0
+Version: 1.4.1
 Summary: This Python library for Raspberry Pi makes it easy to leverage the complex functionality of the Texas Instruments INA219 sensor to measure voltage, current and power.
 Home-page: https://github.com/chrisb2/pi_ina219/
 Author: Chris Borrill
 Author-email: chris.borrill@gmail.com
 License: MIT
 Keywords: ina219 raspberrypi
 Platform: UNKNOWN
@@ -20,19 +20,19 @@
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Requires-Dist: Adafruit-GPIO
 Requires-Dist: mock
 
 Raspberry Pi Python Library for Voltage and Current Sensors Using the INA219
 ============================================================================
 
-`Build Status <https://travis-ci.org/chrisb2/pi_ina219>`__
+|Build Status|
 
-`codecov <https://codecov.io/gh/chrisb2/pi_ina219>`__
+|codecov|
 
-`PyPI version <https://badge.fury.io/py/pi-ina219>`__
+|PyPI version|
 
 This Python library supports the
 `INA219 <http://www.ti.com/lit/ds/symlink/ina219.pdf>`__ voltage,
 current and power monitor sensor from Texas Instruments on both Python 2
 and 3. The intent of the library is to make it easy to use the quite
 complex functionality of this sensor.
 
@@ -78,14 +78,34 @@
 *0x40*.
 
 Note that the bus voltage is that on the load side of the shunt
 resistor, if you want the voltage on the supply side then you should add
 the bus voltage and shunt voltage together, or use the
 *supply_voltage()* function.
 
+I2C Bus number
+~~~~~~~~~~~~~~
+
+In most cases this will be determined automatically, however if this
+fails you will see the exception:
+
+::
+
+   Could not determine default I2C bus for platform
+
+In this case just set the bus number in the INA219 constructor, for
+example:
+
+::
+
+   ina = INA219(SHUNT_OHMS, busnum=1)
+
+This is known to be required with Raspberry Pi 4 and the ‘Bullseye’
+(October 2021) Raspberry Pi OS.
+
 Simple - Auto Gain
 ~~~~~~~~~~~~~~~~~~
 
 This mode is great for getting started, as it will provide valid
 readings until the device current capability is exceeded for the value
 of the shunt resistor connected (3.2A for 0.1Ω shunt resistor). It does
 this by automatically adjusting the gain as required until the maximum
@@ -222,70 +242,78 @@
 
 Note that if you do not wake the device after sleeping, the value
 returned from a read will be the previous value taken before sleeping.
 
 Functions
 ---------
 
--  ``INA219()`` constructs the class. The arguments, are: \_ shunt_ohms:
-   The value of the shunt resistor in Ohms (mandatory). \_
-   max*expected_amps: The maximum expected current in Amps (optional).
+-  ``INA219()`` constructs the class. The arguments, are:
 
+   -  shunt_ohms: The value of the shunt resistor in Ohms (mandatory).
+   -  max_expected_amps: The maximum expected current in Amps
+      (optional).
    -  busnum: The I2C bus number for the device platform, defaults to
       *auto detects 0 or 1 for Raspberry Pi or Beaglebone Black*
       (optional).
    -  address: The I2C address of the INA219, defaults to *0x40*
-      (optional). \* log\ *level: Set to \_logging.INFO\* to see the
-      detailed calibration calculations and \_logging.DEBUG* to see
-      register operations (optional).
+      (optional).
+   -  log_level: Set to *logging.INFO* to see the detailed calibration
+      calculations and *logging.DEBUG* to see register operations
+      (optional).
 
 -  ``configure()`` configures and calibrates how the INA219 will take
-   measurements. The arguments, which are all optional, are: \_
-   voltage_range: The full scale voltage range, this is either 16V or
-   32V, represented by one of the following constants (optional). \_
-   RANGE*16V: Range zero to 16 volts
+   measurements. The arguments, which are all optional, are:
+
+   -  voltage_range: The full scale voltage range, this is either 16V or
+      32V, represented by one of the following constants (optional).
 
-   -  RANGE*32V: Range zero to 32 volts (**default**). **Device only
-      supports up to 26V.**
+      -  RANGE_16V: Range zero to 16 volts
+      -  RANGE_32V: Range zero to 32 volts (**default**). **Device only
+         supports up to 26V.**
 
    -  gain: The gain, which controls the maximum range of the shunt
       voltage, represented by one of the following constants (optional).
-      \_ GAIN_1_40MV: Maximum shunt voltage 40mV \_ GAIN*2_80MV: Maximum
-      shunt voltage 80mV
-   -  GAIN*4_160MV: Maximum shunt voltage 160mV
-   -  GAIN*8_320MV: Maximum shunt voltage 320mV
-   -  GAIN*AUTO: Automatically calculate the gain (**default**)
-   -  bus*adc: The bus ADC resolution (9, 10, 11, or 12-bit), or set the
+
+      -  GAIN_1_40MV: Maximum shunt voltage 40mV
+      -  GAIN_2_80MV: Maximum shunt voltage 80mV
+      -  GAIN_4_160MV: Maximum shunt voltage 160mV
+      -  GAIN_8_320MV: Maximum shunt voltage 320mV
+      -  GAIN_AUTO: Automatically calculate the gain (**default**)
+
+   -  bus_adc: The bus ADC resolution (9, 10, 11, or 12-bit), or set the
       number of samples used when averaging results, represented by one
       of the following constants (optional).
-   -  ADC*9BIT: 9 bit, conversion time 84us.
-   -  ADC*10BIT: 10 bit, conversion time 148us.
-   -  ADC*11BIT: 11 bit, conversion time 276us.
-   -  ADC*12BIT: 12 bit, conversion time 532us (**default**).
-   -  ADC*2SAMP: 2 samples at 12 bit, conversion time 1.06ms.
-   -  ADC*4SAMP: 4 samples at 12 bit, conversion time 2.13ms.
-   -  ADC*8SAMP: 8 samples at 12 bit, conversion time 4.26ms.
-   -  ADC*16SAMP: 16 samples at 12 bit, conversion time 8.51ms
-   -  ADC*32SAMP: 32 samples at 12 bit, conversion time 17.02ms.
-   -  ADC*64SAMP: 64 samples at 12 bit, conversion time 34.05ms.
-   -  ADC*128SAMP: 128 samples at 12 bit, conversion time 68.10ms.
-   -  shunt*adc: The shunt ADC resolution (9, 10, 11, or 12-bit), or set
+
+      -  ADC_9BIT: 9 bit, conversion time 84us.
+      -  ADC_10BIT: 10 bit, conversion time 148us.
+      -  ADC_11BIT: 11 bit, conversion time 276us.
+      -  ADC_12BIT: 12 bit, conversion time 532us (**default**).
+      -  ADC_2SAMP: 2 samples at 12 bit, conversion time 1.06ms.
+      -  ADC_4SAMP: 4 samples at 12 bit, conversion time 2.13ms.
+      -  ADC_8SAMP: 8 samples at 12 bit, conversion time 4.26ms.
+      -  ADC_16SAMP: 16 samples at 12 bit, conversion time 8.51ms
+      -  ADC_32SAMP: 32 samples at 12 bit, conversion time 17.02ms.
+      -  ADC_64SAMP: 64 samples at 12 bit, conversion time 34.05ms.
+      -  ADC_128SAMP: 128 samples at 12 bit, conversion time 68.10ms.
+
+   -  shunt_adc: The shunt ADC resolution (9, 10, 11, or 12-bit), or set
       the number of samples used when averaging results, represented by
       one of the following constants (optional).
-   -  ADC*9BIT: 9 bit, conversion time 84us.
-   -  ADC*10BIT: 10 bit, conversion time 148us.
-   -  ADC*11BIT: 11 bit, conversion time 276us.
-   -  ADC*12BIT: 12 bit, conversion time 532us (**default**).
-   -  ADC*2SAMP: 2 samples at 12 bit, conversion time 1.06ms.
-   -  ADC*4SAMP: 4 samples at 12 bit, conversion time 2.13ms.
-   -  ADC*8SAMP: 8 samples at 12 bit, conversion time 4.26ms.
-   -  ADC*16SAMP: 16 samples at 12 bit, conversion time 8.51ms
-   -  ADC*32SAMP: 32 samples at 12 bit, conversion time 17.02ms.
-   -  ADC_64SAMP: 64 samples at 12 bit, conversion time 34.05ms. \*
-      ADC_128SAMP: 128 samples at 12 bit, conversion time 68.10ms.
+
+      -  ADC_9BIT: 9 bit, conversion time 84us.
+      -  ADC_10BIT: 10 bit, conversion time 148us.
+      -  ADC_11BIT: 11 bit, conversion time 276us.
+      -  ADC_12BIT: 12 bit, conversion time 532us (**default**).
+      -  ADC_2SAMP: 2 samples at 12 bit, conversion time 1.06ms.
+      -  ADC_4SAMP: 4 samples at 12 bit, conversion time 2.13ms.
+      -  ADC_8SAMP: 8 samples at 12 bit, conversion time 4.26ms.
+      -  ADC_16SAMP: 16 samples at 12 bit, conversion time 8.51ms
+      -  ADC_32SAMP: 32 samples at 12 bit, conversion time 17.02ms.
+      -  ADC_64SAMP: 64 samples at 12 bit, conversion time 34.05ms.
+      -  ADC_128SAMP: 128 samples at 12 bit, conversion time 68.10ms.
 
 -  ``voltage()`` Returns the bus voltage in volts (V).
 -  ``supply_voltage()`` Returns the bus supply voltage in volts (V).
    This is the sum of the bus voltage and shunt voltage. A
    *DeviceRangeError* exception is thrown if current overflow occurs.
 -  ``current()`` Returns the bus current in milliamps (mA). A
    *DeviceRangeError* exception is thrown if current overflow occurs.
@@ -354,8 +382,15 @@
 
 Coding Standard
 ---------------
 
 This library adheres to the *PEP8* standard and follows the *idiomatic*
 style described in the book *Writing Idiomatic Python* by *Jeff Knupp*.
 
+.. |Build Status| image:: https://travis-ci.com/chrisb2/pi_ina219.svg?branch=master
+   :target: https://travis-ci.com/chrisb2/pi_ina219
+.. |codecov| image:: https://codecov.io/gh/chrisb2/pi_ina219/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/chrisb2/pi_ina219
+.. |PyPI version| image:: https://badge.fury.io/py/pi-ina219.svg
+   :target: https://badge.fury.io/py/pi-ina219
+
```

