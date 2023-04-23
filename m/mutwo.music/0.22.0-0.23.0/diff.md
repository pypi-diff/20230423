# Comparing `tmp/mutwo.music-0.22.0.tar.gz` & `tmp/mutwo.music-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.music-0.22.0.tar", last modified: Sat Dec 31 13:48:04 2022, max compression
+gzip compressed data, was "mutwo.music-0.23.0.tar", last modified: Sun Apr 23 21:39:10 2023, max compression
```

## Comparing `mutwo.music-0.22.0.tar` & `mutwo.music-0.23.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.051304 mutwo.music-0.22.0/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.055304 mutwo.music-0.22.0/mutwo/music_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      718 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4313 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11105 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/grace_notes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      821 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/loudness.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4877 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/metricities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12039 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13851 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/pitches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26328 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/playing_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3443 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_converters/spectrals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.055304 mutwo.music-0.22.0/mutwo/music_events/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_events/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5777 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_events/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9011 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_events/music.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.055304 mutwo.music-0.22.0/mutwo/music_generators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_generators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6877 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_generators/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8628 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_generators/wilson.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.059304 mutwo.music-0.22.0/mutwo/music_parameters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    52754 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/ambituses.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2154 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/commas.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.059304 mutwo.music-0.22.0/mutwo/music_parameters/configurations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/configurations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6706 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/configurations/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/configurations/lyrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1079 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/configurations/pitch_intervals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2818 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/configurations/pitches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/configurations/volumes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.059304 mutwo.music-0.22.0/mutwo/music_parameters/constants/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/constants/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      589 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/constants/body_parts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10201 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/constants/diatonic_pitch_classes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/constants/instruments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5911 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/constants/pitch_intervals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7580 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/constants/pitches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/constants/playing_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/constants/volumes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/mutwo/music_parameters/instruments/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/instruments/Bassoon.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/instruments/BfClarinet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7811 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/instruments/CelticHarp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/instruments/EfClarinet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/instruments/Flute.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/instruments/Oboe.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/instruments/Piccolo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/instruments/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22347 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/instruments/general.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/mutwo/music_parameters/lyrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/lyrics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/lyrics/text_based_lyrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3582 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/notation_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23435 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/pitch_intervals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/mutwo/music_parameters/pitches/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2451 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/pitches/CommonHarmonic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1352 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/pitches/DirectPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9091 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42919 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/pitches/JustIntonationPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/pitches/MidiPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22576 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/pitches/WesternPitch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1267 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/pitches/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10257 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/playing_indicators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15132 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/scales.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8333 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_parameters/volumes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/mutwo/music_utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_utilities/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/mutwo/music_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo/music_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.055304 mutwo.music-0.22.0/mutwo.music.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2022-12-31 13:48:04.000000 mutwo.music-0.22.0/mutwo.music.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2932 2022-12-31 13:48:04.000000 mutwo.music-0.22.0/mutwo.music.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-12-31 13:48:04.000000 mutwo.music-0.22.0/mutwo.music.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2022-12-31 13:48:04.000000 mutwo.music-0.22.0/mutwo.music.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2022-12-31 13:48:04.000000 mutwo.music-0.22.0/mutwo.music.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.051304 mutwo.music-0.22.0/mutwo_third_party/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/mutwo_third_party/pydsm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo_third_party/pydsm/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/mutwo_third_party/pydsm/pydsm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo_third_party/pydsm/pydsm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13041 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/mutwo_third_party/pydsm/pydsm/iso226.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2022-12-31 13:48:04.063304 mutwo.music-0.22.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2022-12-31 13:47:55.000000 mutwo.music-0.22.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.484223 mutwo.music-0.23.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2023-04-23 21:39:10.484223 mutwo.music-0.23.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.468223 mutwo.music-0.23.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.472223 mutwo.music-0.23.0/mutwo/music_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      718 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4313 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11105 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/grace_notes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      821 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/loudness.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4877 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/metricities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12039 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13851 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/pitches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26225 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/playing_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3443 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_converters/spectrals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.472223 mutwo.music-0.23.0/mutwo/music_events/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_events/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5777 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_events/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9011 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_events/music.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.472223 mutwo.music-0.23.0/mutwo/music_generators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_generators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6877 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_generators/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8628 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_generators/wilson.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.476224 mutwo.music-0.23.0/mutwo/music_parameters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    52754 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/ambituses.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2154 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/commas.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.476224 mutwo.music-0.23.0/mutwo/music_parameters/configurations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/configurations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6706 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/configurations/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/configurations/lyrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1079 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/configurations/pitch_intervals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2818 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/configurations/pitches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/configurations/volumes.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.480224 mutwo.music-0.23.0/mutwo/music_parameters/constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/constants/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      589 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/constants/body_parts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10201 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/constants/diatonic_pitch_classes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/constants/instruments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5911 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/constants/pitch_intervals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7580 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/constants/pitches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/constants/playing_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/constants/volumes.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.480224 mutwo.music-0.23.0/mutwo/music_parameters/instruments/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/instruments/Bassoon.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/instruments/BfClarinet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7811 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/instruments/CelticHarp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/instruments/EfClarinet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      298 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/instruments/Flute.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      296 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/instruments/Oboe.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/instruments/Piccolo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/instruments/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22682 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/instruments/general.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.480224 mutwo.music-0.23.0/mutwo/music_parameters/lyrics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/lyrics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/lyrics/text_based_lyrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3582 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/notation_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23435 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/pitch_intervals.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.484223 mutwo.music-0.23.0/mutwo/music_parameters/pitches/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2451 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/pitches/CommonHarmonic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1352 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/pitches/DirectPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9091 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42913 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/pitches/JustIntonationPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/pitches/MidiPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24678 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/pitches/WesternPitch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1267 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/pitches/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10260 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/playing_indicators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15132 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/scales.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8333 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_parameters/volumes.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.484223 mutwo.music-0.23.0/mutwo/music_utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_utilities/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.484223 mutwo.music-0.23.0/mutwo/music_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo/music_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.468223 mutwo.music-0.23.0/mutwo.music.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2023-04-23 21:39:10.000000 mutwo.music-0.23.0/mutwo.music.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2932 2023-04-23 21:39:10.000000 mutwo.music-0.23.0/mutwo.music.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-23 21:39:10.000000 mutwo.music-0.23.0/mutwo.music.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2023-04-23 21:39:10.000000 mutwo.music-0.23.0/mutwo.music.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-23 21:39:10.000000 mutwo.music-0.23.0/mutwo.music.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.468223 mutwo.music-0.23.0/mutwo_third_party/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.484223 mutwo.music-0.23.0/mutwo_third_party/pydsm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo_third_party/pydsm/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-23 21:39:10.484223 mutwo.music-0.23.0/mutwo_third_party/pydsm/pydsm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo_third_party/pydsm/pydsm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13041 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/mutwo_third_party/pydsm/pydsm/iso226.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-23 21:39:10.484223 mutwo.music-0.23.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-04-23 21:38:56.000000 mutwo.music-0.23.0/setup.py
```

### Comparing `mutwo.music-0.22.0/LICENSE` & `mutwo.music-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/PKG-INFO` & `mutwo.music-0.23.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.music
-Version: 0.22.0
+Version: 0.23.0
 Summary: music extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.ext-music
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
 Requires-Python: >=3.10, <4
```

### Comparing `mutwo.music-0.22.0/README.md` & `mutwo.music-0.23.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/__init__.py` & `mutwo.music-0.23.0/mutwo/music_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/configurations.py` & `mutwo.music-0.23.0/mutwo/music_converters/configurations.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/grace_notes.py` & `mutwo.music-0.23.0/mutwo/music_converters/grace_notes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/instruments.py` & `mutwo.music-0.23.0/mutwo/music_converters/instruments.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/loudness.py` & `mutwo.music-0.23.0/mutwo/music_converters/loudness.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/metricities.py` & `mutwo.music-0.23.0/mutwo/music_converters/metricities.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/parsers.py` & `mutwo.music-0.23.0/mutwo/music_converters/parsers.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/pitches.py` & `mutwo.music-0.23.0/mutwo/music_converters/pitches.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/playing_indicators.py` & `mutwo.music-0.23.0/mutwo/music_converters/playing_indicators.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 class PlayingIndicatorConverter(core_converters.abc.Converter):
     """Abstract base class to apply :class:`~mutwo.music_parameters.abc.PlayingIndicator` on a :class:`~mutwo.core_events.SimpleEvent`.
 
     :param simple_event_to_playing_indicator_collection: Function to extract from a
         :class:`mutwo.core_events.SimpleEvent` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
-        :attr:`~mutwo.ext.events.music.NoteLike.playing_indicator_collection`
-        attribute (because by default :class:`mutwo.ext.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
+        attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
-        When using different Event classes than :class:`~mutwo.ext.events.music.NoteLike`
+        When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
     :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection], optional
 
@@ -124,42 +124,42 @@
     :param duration_for_each_attack: Set how long each attack of the
         Arpeggio lasts. Default to 0.1.
     :type duration_for_each_attack: constants.DurationType
     :param simple_event_to_pitch_list: Function to extract from a
         :class:`mutwo.core_events.SimpleEvent` a tuple that contains pitch objects
         (objects that inherit from :class:`mutwo.music_parameters.abc.Pitch`).
         By default it asks the Event for its
-        :attr:`~mutwo.ext.events.music.NoteLike.pitch_list` attribute
-        (because by default :class:`mutwo.ext.events.music.NoteLike` objects are expected).
-        When using different Event classes than :class:`~mutwo.ext.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.pitch_list` attribute
+        (because by default :class:`mutwo.music_events.NoteLike` objects are expected).
+        When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their pitch property, this argument
         should be overridden.
         If the function call raises an :obj:`AttributeError` (e.g. if no pitch can be
         extracted), mutwo will assume an event without any pitches.
     :type simple_event_to_pitch_list: typing.Callable[[core_events.SimpleEvent], music_parameters.abc.Pitch], optional
     :param simple_event_to_playing_indicator_collection: Function to extract from a
         :class:`mutwo.core_events.SimpleEvent` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
-        :attr:`~mutwo.ext.events.music.NoteLike.playing_indicator_collection`
-        attribute (because by default :class:`mutwo.ext.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
+        attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
-        When using different Event classes than :class:`~mutwo.ext.events.music.NoteLike`
+        When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
     :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
     :param set_pitch_list_for_simple_event: Function which assigns
         a list of :class:`~mutwo.music_parameters.abc.Pitch` objects to a
         :class:`~mutwo.core_events.SimpleEvent`. By default the
         function assigns the passed pitches to the
-        :attr:`~mutwo.ext.events.music.NoteLike.pitch_list` attribute
-        (because by default :class:`mutwo.ext.events.music.NoteLike` objects
+        :attr:`~mutwo.music_events.NoteLike.pitch_list` attribute
+        (because by default :class:`mutwo.music_events.NoteLike` objects
         are expected).
     :type set_pitch_list_for_simple_event: typing.Callable[[core_events.SimpleEvent, list[music_parameters.abc.Pitch]], None]
     """
 
     def __init__(
         self,
         duration_for_each_attack: core_constants.DurationType = 0.1,
@@ -236,18 +236,18 @@
 
     :param factor:
     :param allowed_articulation_name_sequence:
     :param simple_event_to_playing_indicator_collection: Function to extract from a
         :class:`mutwo.core_events.SimpleEvent` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
-        :attr:`~mutwo.ext.events.music.NoteLike.playing_indicator_collection`
-        attribute (because by default :class:`mutwo.ext.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
+        attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
-        When using different Event classes than :class:`~mutwo.ext.events.music.NoteLike`
+        When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
     :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
     """
@@ -295,18 +295,18 @@
 
     :param articulation_name_tuple_to_playing_indicator_converter:
     :type articulation_name_tuple_to_playing_indicator_converter: dict[tuple[str, ...], PlayingIndicatorConverter]
     :param simple_event_to_playing_indicator_collection: Function to extract from a
         :class:`mutwo.core_events.SimpleEvent` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
-        :attr:`~mutwo.ext.events.music.NoteLike.playing_indicator_collection`
-        attribute (because by default :class:`mutwo.ext.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
+        attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
-        When using different Event classes than :class:`~mutwo.ext.events.music.NoteLike`
+        When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
     :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
     """
@@ -374,30 +374,30 @@
 
     :param trill_size:
     :type trill_size: constants.DurationType
     :param simple_event_to_pitch_list: Function to extract from a
         :class:`mutwo.core_events.SimpleEvent` a tuple that contains pitch objects
         (objects that inherit from :class:`mutwo.music_parameters.abc.Pitch`).
         By default it asks the Event for its
-        :attr:`~mutwo.ext.events.music.NoteLike.pitch_list` attribute
-        (because by default :class:`mutwo.ext.events.music.NoteLike` objects are expected).
-        When using different Event classes than :class:`~mutwo.ext.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.pitch_list` attribute
+        (because by default :class:`mutwo.music_events.NoteLike` objects are expected).
+        When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their pitch property, this argument
         should be overridden.
         If the function call raises an :obj:`AttributeError` (e.g. if no pitch can be
         extracted), mutwo will assume an event without any pitches.
     :type simple_event_to_pitch_list: typing.Callable[[core_events.SimpleEvent], music_parameters.abc.Pitch], optional
     :param simple_event_to_playing_indicator_collection: Function to extract from a
         :class:`mutwo.core_events.SimpleEvent` a
-        :class:`mutwo.ext.parameters.playing_indicators.PlayingIndicatorCollection`
+        :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
-        :attr:`~mutwo.ext.events.music.NoteLike.playing_indicator_collection`
-        attribute (because by default :class:`mutwo.ext.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
+        attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
-        When using different Event classes than :class:`~mutwo.ext.events.music.NoteLike`
+        When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
     :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
     """
@@ -407,15 +407,15 @@
         trill_size: core_constants.DurationType = fractions.Fraction(1, 16),
         simple_event_to_pitch_list: typing.Callable[
             [core_events.SimpleEvent], list[music_parameters.abc.Pitch]
         ] = music_converters.SimpleEventToPitchList(),
         simple_event_to_playing_indicator_collection: typing.Callable[
             [core_events.SimpleEvent],
             music_parameters.PlayingIndicatorCollection,
-        ] = music_converters.SimpleEventToPitchList(),
+        ] = music_converters.SimpleEventToPlayingIndicatorCollection(),
     ):
         self._trill_size = trill_size
         self._simple_event_to_pitch_list = simple_event_to_pitch_list
         super().__init__(simple_event_to_playing_indicator_collection)
 
     def _apply_trill(
         self,
@@ -471,18 +471,18 @@
         and returns a new `SimpleEvent` with the same duration which represents a rest.
         By default, `mutwo` simply creates a `SimpleEvent` with the same duration.
     :type make_rest: typing.Callable[[core_events.SimpleEvent], core_events.SimpleEvent]
     :param simple_event_to_playing_indicator_collection: Function to extract from a
         :class:`mutwo.core_events.SimpleEvent` a
         :class:`mutwo.music_parameters.PlayingIndicatorCollection`
         object. By default it asks the Event for its
-        :attr:`~mutwo.ext.events.music.NoteLike.playing_indicator_collection`
-        attribute (because by default :class:`mutwo.ext.events.music.NoteLike`
+        :attr:`~mutwo.music_events.NoteLike.playing_indicator_collection`
+        attribute (because by default :class:`mutwo.music_events.NoteLike`
         objects are expected).
-        When using different Event classes than :class:`~mutwo.ext.events.music.NoteLike`
+        When using different Event classes than :class:`~mutwo.music_events.NoteLike`
         with a different name for their playing_indicator_collection property, this argument
         should be overridden. If the
         function call raises an :obj:`AttributeError` (e.g. if no playing indicator
         collection can be extracted), mutwo will build a playing indicator collection
         from :const:`~mutwo.music_events.configurations.DEFAULT_PLAYING_INDICATORS_COLLECTION_CLASS`.
     :type simple_event_to_playing_indicator_collection: typing.Callable[[core_events.SimpleEvent], music_parameters.PlayingIndicatorCollection,], optional
     """
@@ -523,15 +523,15 @@
 
     @property
     def default_playing_indicator(self) -> music_parameters.abc.PlayingIndicator:
         return music_parameters.abc.ExplicitPlayingIndicator()
 
 
 class PlayingIndicatorsConverter(core_converters.abc.SymmetricalEventConverter):
-    """Apply :class:`~mutwo.ext.parameters.abc.PlayingIndicator` on any :class:`~mutwo.core_events.abc.Event`.
+    """Apply :class:`mutwo.music_parameters.abc.PlayingIndicator` on any :class:`~mutwo.core_events.abc.Event`.
 
     :param playing_indicator_converter_sequence: A sequence of :class:`PlayingIndicatorConverter` which shall
         be applied on each :class:`~mutwo.core_events.SimpleEvent`.
     :type playing_indicator_converter_sequence: typing.Sequence[PlayingIndicatorConverter]
     """
 
     def __init__(
```

### Comparing `mutwo.music-0.22.0/mutwo/music_converters/spectrals.py` & `mutwo.music-0.23.0/mutwo/music_converters/spectrals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_events/configurations.py` & `mutwo.music-0.23.0/mutwo/music_events/configurations.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_events/music.py` & `mutwo.music-0.23.0/mutwo/music_events/music.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_generators/constants.py` & `mutwo.music-0.23.0/mutwo/music_generators/constants.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_generators/wilson.py` & `mutwo.music-0.23.0/mutwo/music_generators/wilson.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/__init__.py` & `mutwo.music-0.23.0/mutwo/music_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/abc.py` & `mutwo.music-0.23.0/mutwo/music_parameters/abc.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/commas.py` & `mutwo.music-0.23.0/mutwo/music_parameters/commas.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/configurations/instruments.py` & `mutwo.music-0.23.0/mutwo/music_parameters/configurations/instruments.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/configurations/pitch_intervals.py` & `mutwo.music-0.23.0/mutwo/music_parameters/configurations/pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/configurations/pitches.py` & `mutwo.music-0.23.0/mutwo/music_parameters/configurations/pitches.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/configurations/volumes.py` & `mutwo.music-0.23.0/mutwo/music_parameters/configurations/volumes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/constants/body_parts.py` & `mutwo.music-0.23.0/mutwo/music_parameters/constants/body_parts.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/constants/diatonic_pitch_classes.py` & `mutwo.music-0.23.0/mutwo/music_parameters/constants/diatonic_pitch_classes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/constants/instruments.py` & `mutwo.music-0.23.0/mutwo/music_parameters/constants/instruments.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/constants/pitch_intervals.py` & `mutwo.music-0.23.0/mutwo/music_parameters/constants/pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/constants/pitches.py` & `mutwo.music-0.23.0/mutwo/music_parameters/constants/pitches.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/constants/playing_indicators.py` & `mutwo.music-0.23.0/mutwo/music_parameters/constants/playing_indicators.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/constants/volumes.py` & `mutwo.music-0.23.0/mutwo/music_parameters/constants/volumes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/instruments/CelticHarp.py` & `mutwo.music-0.23.0/mutwo/music_parameters/instruments/CelticHarp.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/instruments/__init__.py` & `mutwo.music-0.23.0/mutwo/music_parameters/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/instruments/general.py` & `mutwo.music-0.23.0/mutwo/music_parameters/instruments/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     @functools.cached_property
     def pitch(self) -> music_parameters.JustIntonationPitch:
         """The resulting sounding pitch of a :class:`NaturalHarmonic`.
 
         **Example:**
 
         >>> from mutwo import music_parameters
-        >>> string = music_parameters.String(music_parameters.WesternPitch("g", 3))
+        >>> string = music_parameters.String(0, music_parameters.WesternPitch("g", 3))
         >>> natural_harmonic = music_parameters.NaturalHarmonic(3, string)
         >>> natural_harmonic.pitch
         WesternPitch('d', 5)
         """
         return self.string.tuning + self.interval
 
     @functools.cached_property
@@ -89,18 +89,18 @@
         """Find all :class:`NaturalHarmonic.Node` on which harmonic is playable.
 
         **Example:**
 
         >>> from mutwo import music_parameters
         >>> natural_harmonic = music_parameters.NaturalHarmonic(
         ...     2,
-        ...     music_parameters.String(music_parameters.WesternPitch('g', 3)),
+        ...     music_parameters.String(0, music_parameters.WesternPitch('g', 3)),
         ... )
         >>> natural_harmonic.node_tuple
-        (NaturalHarmonic.Node(interval=JustIntonationPitch('2/1'), natural_harmonic=NaturalHarmonic(index=2, tonality=True), string=String(WesternPitch('g', 3))),)
+        (NaturalHarmonic.Node(interval=JustIntonationPitch('2/1'), natural_harmonic=NaturalHarmonic(index=2, tonality=True), string=String(0, WesternPitch('g', 3))),)
         """
         node_list = []
         for node_index in range(1, self.index):
             ratio = fractions.Fraction(self.index, node_index)
             if ratio.numerator == self.index:
                 node_list.append(
                     self.Node(
@@ -110,14 +110,18 @@
         return tuple(reversed(node_list))
 
 
 @dataclasses.dataclass(frozen=True)
 class String(object):
     """:class:`String` represents a string of an instrument.
 
+    :param index: The index of a :class:`String`. This is important
+        in order to differentiate how far two strings are from
+        each other.
+    :type index: int
     :param tuning: The pitch to which the string is tuned to.
     :type tuning: music_parameters.abc.Pitch
     :param tuning_original: If the standard tuning of a string
         differs from its current tuning (e.g. if a scordatura
         is used) this parameter can be set to the standard tuning.
         This is useful in case one wants to notate the fingering
         of a harmonic and not the sounding result. The ``pitch``
@@ -136,25 +140,27 @@
         infinitely high :class:`NaturalHarmonic` of a :class:`String`
         with its ``index_to_natural_harmonic`` method. Default to 6.
     :type max_natural_harmonic_index: int
 
     **Example:**
 
     >>> from mutwo import music_parameters
-    >>> g_string = music_parameters.String(music_parameters.WesternPitch('g', 3))
+    >>> g_string = music_parameters.String(0, music_parameters.WesternPitch('g', 3))
     >>> g_string
     String(WesternPitch('g', 3))
     >>> retuned_g_string = music_parameters.String(
+    ...     0,
     ...     music_parameters.WesternPitch('g', 3),
     ...     tuning_original=music_parameters.JustIntonationPitch('8/11'),
     ... )
     >>> retuned_g_string
     String(WesternPitch('g', 3))
     """
 
+    index: int
     tuning: music_parameters.abc.Pitch
     tuning_original: typing.Optional[music_parameters.abc.Pitch] = None
     max_natural_harmonic_index: int = 6
 
     def __post_init__(self):
         object.__setattr__(self, "tuning_original", self.tuning_original or self.tuning)
         object.__setattr__(self, "_index_to_natural_harmonic", {})
@@ -180,15 +186,15 @@
             plus fifth), etc.
         :type natural_harmonic_index: int
 
         **Example:**
 
         >>> from mutwo import music_parameters
         >>> g_string = music_parameters.String(
-        ...     music_parameters.WesternPitch('g', 3)
+        ...     0, music_parameters.WesternPitch('g', 3)
         ... )
         >>> g_string.index_to_natural_harmonic(5)
         NaturalHarmonic(index=5, tonality=True)
         """
         try:
             return self._index_to_natural_harmonic[natural_harmonic_index]
         except KeyError:
@@ -244,15 +250,15 @@
                     pitch_list.append(p)
         return tuple(sorted(pitch_list))
 
     @functools.cached_property
     def harmonic_pitch_ambitus(self) -> music_parameters.abc.PitchAmbitus:
         """Get flageolet :class:`music_parameters.abc.PitchAmbitus`."""
         hp_tuple = self.harmonic_pitch_tuple
-        return music_parameters.OctaveAmbitus(hp_tuple[0], hp_tuple[1])
+        return music_parameters.OctaveAmbitus(hp_tuple[0], hp_tuple[-1])
 
     def get_harmonic_pitch_variant_tuple(
         self,
         pitch: music_parameters.abc.Pitch,
         period: typing.Optional[music_parameters.abc.PitchInterval] = None,
         tolerance: music_parameters.abc.PitchInterval = music_parameters.DirectPitchInterval(
             2
@@ -542,17 +548,19 @@
     >>> music_parameters.Orchestration(
     ...   oboe0=music_parameters.Oboe(),
     ...   oboe1=music_parameters.Oboe(),
     ... )
     Orchestration(oboe0=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=DirectPitchInterval(interval = 0)), oboe1=Oboe(name='oboe', short_name='ob.', pitch_count_range=Range[1, 2), transposition_pitch_interval=DirectPitchInterval(interval = 0)))
     """
 
-    instrument_name_tuple, instrument_tuple = zip(
-        *instrument_name_to_instrument.items()
-    )
+    instrument_name_tuple, instrument_tuple = tuple([]), tuple([])
+    if instrument_name_to_instrument:
+        instrument_name_tuple, instrument_tuple = zip(
+            *instrument_name_to_instrument.items()
+        )
 
     return type(
         "Orchestration",
         (
             collections.namedtuple("Orchestration", instrument_name_tuple),
             OrchestrationMixin,
         ),
```

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/lyrics/__init__.py` & `mutwo.music-0.23.0/mutwo/music_parameters/lyrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/lyrics/text_based_lyrics.py` & `mutwo.music-0.23.0/mutwo/music_parameters/lyrics/text_based_lyrics.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/notation_indicators.py` & `mutwo.music-0.23.0/mutwo/music_parameters/notation_indicators.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/pitch_intervals.py` & `mutwo.music-0.23.0/mutwo/music_parameters/pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/pitches/CommonHarmonic.py` & `mutwo.music-0.23.0/mutwo/music_parameters/pitches/CommonHarmonic.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/pitches/DirectPitch.py` & `mutwo.music-0.23.0/mutwo/music_parameters/pitches/DirectPitch.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py` & `mutwo.music-0.23.0/mutwo/music_parameters/pitches/EqualDividedOctavePitch.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/pitches/JustIntonationPitch.py` & `mutwo.music-0.23.0/mutwo/music_parameters/pitches/JustIntonationPitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
                 return super().__eq__(other)
 
     def __lt__(self, other: typing.Any) -> bool:
         match other:
             case music_parameters.abc.PitchInterval():
                 return self.interval < other.interval
             case _:  # pitch test
-                return super().__lt__(self, other)
+                return super().__lt__(other)
 
     def __float__(self) -> float:
         """Return the float of a JustIntonationPitch - object.
 
         These are the same:
             float(myJustIntonationPitch.ratio) == float(myJustIntonationPitch).
         Note the difference that the second version might be slightly
```

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/pitches/MidiPitch.py` & `mutwo.music-0.23.0/mutwo/music_parameters/pitches/MidiPitch.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/pitches/WesternPitch.py` & `mutwo.music-0.23.0/mutwo/music_parameters/pitches/WesternPitch.py`

 * *Files 4% similar despite different names*

```diff
@@ -563,7 +563,53 @@
                 pitch_interval = pitch_to_compare._get_western_pitch_interval(self)
                 pitch_interval.inverse()
             else:
                 pitch_interval = self._get_western_pitch_interval(pitch_to_compare)
             return pitch_interval
         else:
             return super().get_pitch_interval(pitch_to_compare)
+
+    @core_utilities.add_copy_option
+    def round_to(
+        self,
+        allowed_division_sequence: typing.Sequence[fractions.Fraction] = (
+            fractions.Fraction(1, 1),
+        ),
+    ) -> WesternPitch:
+        """Round to closest accidental (helpful to avoid microtones).
+
+        param allowed_division_sequence: Only accidentals are allowed which
+            pitch class modification are dividable by any of the provided
+            numbers. So for instance if only chromatic pitches should be
+            allowed this should be ``[fractions.Fraction(1, 1)]``. But if
+            both chromatic and quartertone pitches are allowed this must be
+            ``[fractions.Fraction(1, 1), fractions.Fraction(1, 2)]``. Default
+            to ``(fractions.Fraction(1, 1),)`` (only chromatic pitches are
+            allowed).
+        type allowed_division_sequence: typing.Sequence[fractions.Fraction]
+        """
+
+        allowed_accidental_to_pitch_class_modification = {
+            a: pmod
+            for a, pmod in music_parameters.constants.ACCIDENTAL_NAME_TO_PITCH_CLASS_MODIFICATION_DICT.items()
+            if any([pmod % d == 0 for d in allowed_division_sequence])
+        }
+        pitch_modifiation = (
+            music_parameters.constants.ACCIDENTAL_NAME_TO_PITCH_CLASS_MODIFICATION_DICT[
+                self.accidental_name
+            ]
+        )
+        if pitch_modifiation not in allowed_accidental_to_pitch_class_modification:
+            pitch_class_modification_to_accidental = {
+                v: k for k, v in allowed_accidental_to_pitch_class_modification.items()
+            }
+            allowed_pitch_class_modification_tuple = tuple(
+                sorted(allowed_accidental_to_pitch_class_modification.values())
+            )
+            new_accidental = pitch_class_modification_to_accidental[
+                core_utilities.find_closest_item(
+                    pitch_modifiation, allowed_pitch_class_modification_tuple
+                )
+            ]
+            self.pitch_class_name = f"{self.pitch_class_name[0]}{new_accidental}"
+
+        return self
```

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/pitches/__init__.py` & `mutwo.music-0.23.0/mutwo/music_parameters/pitches/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/playing_indicators.py` & `mutwo.music-0.23.0/mutwo/music_parameters/playing_indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     >>> from mutwo import music_events, music_parameters
     >>> n = music_events.NoteLike('c', 4)
     >>> n.playing_indicator_collection.natural_harmonic_node_list.is_active
     False
     >>> n.playing_indicator_collection.natural_harmonic_node_list.append(
     ...     music_parameters.NaturalHarmonic(
     ...         2,
-    ...         music_parameters.String(music_parameters.WesternPitch('c', 3))
+    ...         music_parameters.String(0, music_parameters.WesternPitch('c', 3))
     ...     ).node_tuple[0]
     ... )
     >>> n.playing_indicator_collection.natural_harmonic_node_list.is_active
     True
     """
 
     def __new__(
```

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/scales.py` & `mutwo.music-0.23.0/mutwo/music_parameters/scales.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_parameters/volumes.py` & `mutwo.music-0.23.0/mutwo/music_parameters/volumes.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo/music_utilities/exceptions.py` & `mutwo.music-0.23.0/mutwo/music_utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo.music.egg-info/PKG-INFO` & `mutwo.music-0.23.0/mutwo.music.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.music
-Version: 0.22.0
+Version: 0.23.0
 Summary: music extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.ext-music
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
 Requires-Python: >=3.10, <4
```

### Comparing `mutwo.music-0.22.0/mutwo.music.egg-info/SOURCES.txt` & `mutwo.music-0.23.0/mutwo.music.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/mutwo_third_party/pydsm/pydsm/iso226.py` & `mutwo.music-0.23.0/mutwo_third_party/pydsm/pydsm/iso226.py`

 * *Files identical despite different names*

### Comparing `mutwo.music-0.22.0/setup.py` & `mutwo.music-0.23.0/setup.py`

 * *Files identical despite different names*

