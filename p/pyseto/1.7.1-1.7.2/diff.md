# Comparing `tmp/pyseto-1.7.1.tar.gz` & `tmp/pyseto-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyseto-1.7.1.tar", max compression
+gzip compressed data, was "pyseto-1.7.2.tar", max compression
```

## Comparing `pyseto-1.7.1.tar` & `pyseto-1.7.2.tar`

### file list

```diff
@@ -1,115 +1,114 @@
--rw-r--r--   0        0        0    12479 2023-01-20 20:03:11.094544 pyseto-1.7.1/CHANGES.rst
--rw-r--r--   0        0        0     1077 2023-01-20 20:03:11.094544 pyseto-1.7.1/LICENSE
--rw-r--r--   0        0        0    16316 2023-01-20 20:03:11.094544 pyseto-1.7.1/README.md
--rw-r--r--   0        0        0      634 2023-01-20 20:03:11.094544 pyseto-1.7.1/docs/Makefile
--rw-r--r--   0        0        0      363 2023-01-20 20:03:11.094544 pyseto-1.7.1/docs/api.rst
--rw-r--r--   0        0        0       28 2023-01-20 20:03:11.094544 pyseto-1.7.1/docs/changes.rst
--rw-r--r--   0        0        0     2880 2023-01-20 20:03:11.094544 pyseto-1.7.1/docs/conf.py
--rw-r--r--   0        0        0     4062 2023-01-20 20:03:11.094544 pyseto-1.7.1/docs/index.rst
--rw-r--r--   0        0        0      111 2023-01-20 20:03:11.094544 pyseto-1.7.1/docs/installation.rst
--rw-r--r--   0        0        0     7741 2023-01-20 20:03:11.094544 pyseto-1.7.1/docs/paserk_usage.rst
--rw-r--r--   0        0        0    12353 2023-01-20 20:03:11.094544 pyseto-1.7.1/docs/paseto_usage.rst
--rw-r--r--   0        0        0    83796 2023-01-20 20:03:11.094544 pyseto-1.7.1/poetry.lock
--rw-r--r--   0        0        0     1076 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyproject.toml
--rw-r--r--   0        0        0      856 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyseto/__init__.py
--rw-r--r--   0        0        0      719 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyseto/exceptions.py
--rw-r--r--   0        0        0     9423 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyseto/key.py
--rw-r--r--   0        0        0     8198 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyseto/key_interface.py
--rw-r--r--   0        0        0     9912 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyseto/key_nist.py
--rw-r--r--   0        0        0    14328 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyseto/key_sodium.py
--rw-r--r--   0        0        0    10577 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyseto/paseto.py
--rw-r--r--   0        0        0        0 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyseto/py.typed
--rw-r--r--   0        0        0     3329 2023-01-20 20:03:11.094544 pyseto-1.7.1/pyseto/pyseto.py
--rw-r--r--   0        0        0     2337 2023-01-20 20:03:11.098544 pyseto-1.7.1/pyseto/token.py
--rw-r--r--   0        0        0     1576 2023-01-20 20:03:11.098544 pyseto-1.7.1/pyseto/utils.py
--rw-r--r--   0        0        0        0 2023-01-20 20:03:11.098544 pyseto-1.7.1/pyseto/versions/__init__.py
--rw-r--r--   0        0        0     9552 2023-01-20 20:03:11.098544 pyseto-1.7.1/pyseto/versions/v1.py
--rw-r--r--   0        0        0     5319 2023-01-20 20:03:11.098544 pyseto-1.7.1/pyseto/versions/v2.py
--rw-r--r--   0        0        0    10898 2023-01-20 20:03:11.098544 pyseto-1.7.1/pyseto/versions/v3.py
--rw-r--r--   0        0        0     5083 2023-01-20 20:03:11.098544 pyseto-1.7.1/pyseto/versions/v4.py
--rw-r--r--   0        0        0        0 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/__init__.py
--rw-r--r--   0        0        0      312 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_ecdsa_p384.json
--rw-r--r--   0        0        0      288 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_ecdsa_p384.pem
--rw-r--r--   0        0        0      288 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_ecdsa_p384_2.pem
--rw-r--r--   0        0        0      198 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_ed25519.json
--rw-r--r--   0        0        0      119 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_ed25519.pem
--rw-r--r--   0        0        0      119 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_ed25519_2.pem
--rw-r--r--   0        0        0     1732 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_rsa.json
--rw-r--r--   0        0        0     1704 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_rsa.pem
--rw-r--r--   0        0        0     1679 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_rsa_2.pem
--rw-r--r--   0        0        0      119 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_x25519.pem
--rw-r--r--   0        0        0      119 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/private_key_x25519_2.pem
--rw-r--r--   0        0        0      255 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_ecdsa_p384.json
--rw-r--r--   0        0        0      215 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_ecdsa_p384.pem
--rw-r--r--   0        0        0      215 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_ecdsa_p384_2.pem
--rw-r--r--   0        0        0      162 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_ed25519.json
--rw-r--r--   0        0        0      113 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_ed25519.pem
--rw-r--r--   0        0        0      113 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_ed25519_2.pem
--rw-r--r--   0        0        0      454 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_rsa.json
--rw-r--r--   0        0        0      451 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_rsa.pem
--rw-r--r--   0        0        0      451 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_rsa_2.pem
--rw-r--r--   0        0        0      113 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_x25519.pem
--rw-r--r--   0        0        0      113 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/keys/public_key_x25519_2.pem
--rw-r--r--   0        0        0    16775 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_key.py
--rw-r--r--   0        0        0     2117 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_key_interface.py
--rw-r--r--   0        0        0    17139 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_pyseto.py
--rw-r--r--   0        0        0    21072 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_sample.py
--rw-r--r--   0        0        0     2886 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_token.py
--rw-r--r--   0        0        0      829 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_utils.py
--rw-r--r--   0        0        0     7242 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_v1.py
--rw-r--r--   0        0        0     9653 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_v2.py
--rw-r--r--   0        0        0     8531 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_v3.py
--rw-r--r--   0        0        0     4464 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_v4.py
--rw-r--r--   0        0        0    20683 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/test_with_test_vectors.py
--rw-r--r--   0        0        0      751 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/utils.py
--rw-r--r--   0        0        0      630 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.lid.json
--rw-r--r--   0        0        0      922 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.local-pw.json
--rw-r--r--   0        0        0      898 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.local-wrap.pie.json
--rw-r--r--   0        0        0      641 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.local.json
--rw-r--r--   0        0        0      645 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.pid.json
--rw-r--r--   0        0        0     1002 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.public.json
--rw-r--r--   0        0        0    10283 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.seal.json
--rw-r--r--   0        0        0     7289 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.secret-pw.json
--rw-r--r--   0        0        0     7265 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.secret-wrap.pie.json
--rw-r--r--   0        0        0     3921 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.secret.json
--rw-r--r--   0        0        0     1886 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k1.sid.json
--rw-r--r--   0        0        0      630 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.lid.json
--rw-r--r--   0        0        0      922 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.local-pw.json
--rw-r--r--   0        0        0      854 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.local-wrap.pie.json
--rw-r--r--   0        0        0      641 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.local.json
--rw-r--r--   0        0        0      630 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.pid.json
--rw-r--r--   0        0        0      648 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.public.json
--rw-r--r--   0        0        0     1135 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.seal.json
--rw-r--r--   0        0        0     1141 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.secret-pw.json
--rw-r--r--   0        0        0     1073 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.secret-wrap.pie.json
--rw-r--r--   0        0        0     1512 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.secret.json
--rw-r--r--   0        0        0     1068 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k2.sid.json
--rw-r--r--   0        0        0      630 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.lid.json
--rw-r--r--   0        0        0      922 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.local-pw.json
--rw-r--r--   0        0        0      898 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.local-wrap.pie.json
--rw-r--r--   0        0        0      641 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.local.json
--rw-r--r--   0        0        0      508 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.pid.json
--rw-r--r--   0        0        0      567 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.public.json
--rw-r--r--   0        0        0     1859 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.seal.json
--rw-r--r--   0        0        0     1937 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.secret-pw.json
--rw-r--r--   0        0        0     1913 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.secret-wrap.pie.json
--rw-r--r--   0        0        0     2163 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.secret.json
--rw-r--r--   0        0        0     2082 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k3.sid.json
--rw-r--r--   0        0        0      630 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.lid.json
--rw-r--r--   0        0        0      922 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.local-pw.json
--rw-r--r--   0        0        0      854 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.local-wrap.pie.json
--rw-r--r--   0        0        0      641 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.local.json
--rw-r--r--   0        0        0      630 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.pid.json
--rw-r--r--   0        0        0      648 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.public.json
--rw-r--r--   0        0        0     1135 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.seal.json
--rw-r--r--   0        0        0     1141 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.secret-pw.json
--rw-r--r--   0        0        0     1073 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.secret-wrap.pie.json
--rw-r--r--   0        0        0     1512 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.secret.json
--rw-r--r--   0        0        0     1068 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/PASERK/k4.sid.json
--rw-r--r--   0        0        0    18232 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/v1.json
--rw-r--r--   0        0        0    11135 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/v2.json
--rw-r--r--   0        0        0    12741 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/v3.json
--rw-r--r--   0        0        0    11643 2023-01-20 20:03:11.098544 pyseto-1.7.1/tests/vectors/v4.json
--rw-r--r--   0        0        0     1134 2023-01-20 20:03:11.098544 pyseto-1.7.1/tox.ini
--rw-r--r--   0        0        0    17735 1970-01-01 00:00:00.000000 pyseto-1.7.1/setup.py
--rw-r--r--   0        0        0    17417 1970-01-01 00:00:00.000000 pyseto-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    13519 2023-04-22 22:58:49.088261 pyseto-1.7.2/CHANGES.rst
+-rw-r--r--   0        0        0     1077 2023-04-22 22:58:49.088261 pyseto-1.7.2/LICENSE
+-rw-r--r--   0        0        0    16316 2023-04-22 22:58:49.088261 pyseto-1.7.2/README.md
+-rw-r--r--   0        0        0      634 2023-04-22 22:58:49.088261 pyseto-1.7.2/docs/Makefile
+-rw-r--r--   0        0        0      363 2023-04-22 22:58:49.088261 pyseto-1.7.2/docs/api.rst
+-rw-r--r--   0        0        0       28 2023-04-22 22:58:49.088261 pyseto-1.7.2/docs/changes.rst
+-rw-r--r--   0        0        0     2880 2023-04-22 22:58:49.088261 pyseto-1.7.2/docs/conf.py
+-rw-r--r--   0        0        0     4062 2023-04-22 22:58:49.088261 pyseto-1.7.2/docs/index.rst
+-rw-r--r--   0        0        0      111 2023-04-22 22:58:49.088261 pyseto-1.7.2/docs/installation.rst
+-rw-r--r--   0        0        0     7741 2023-04-22 22:58:49.088261 pyseto-1.7.2/docs/paserk_usage.rst
+-rw-r--r--   0        0        0    12353 2023-04-22 22:58:49.088261 pyseto-1.7.2/docs/paseto_usage.rst
+-rw-r--r--   0        0        0    84271 2023-04-22 22:58:49.092261 pyseto-1.7.2/poetry.lock
+-rw-r--r--   0        0        0     1077 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0      856 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/__init__.py
+-rw-r--r--   0        0        0      719 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/exceptions.py
+-rw-r--r--   0        0        0     9420 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/key.py
+-rw-r--r--   0        0        0     8198 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/key_interface.py
+-rw-r--r--   0        0        0     9904 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/key_nist.py
+-rw-r--r--   0        0        0    14315 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/key_sodium.py
+-rw-r--r--   0        0        0    10573 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/paseto.py
+-rw-r--r--   0        0        0        0 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/py.typed
+-rw-r--r--   0        0        0     3327 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/pyseto.py
+-rw-r--r--   0        0        0     2337 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/token.py
+-rw-r--r--   0        0        0     1575 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/utils.py
+-rw-r--r--   0        0        0        0 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/versions/__init__.py
+-rw-r--r--   0        0        0     9544 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/versions/v1.py
+-rw-r--r--   0        0        0     5312 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/versions/v2.py
+-rw-r--r--   0        0        0    10887 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/versions/v3.py
+-rw-r--r--   0        0        0     5077 2023-04-22 22:58:49.092261 pyseto-1.7.2/pyseto/versions/v4.py
+-rw-r--r--   0        0        0        0 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/__init__.py
+-rw-r--r--   0        0        0      312 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_ecdsa_p384.json
+-rw-r--r--   0        0        0      288 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_ecdsa_p384.pem
+-rw-r--r--   0        0        0      288 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_ecdsa_p384_2.pem
+-rw-r--r--   0        0        0      198 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_ed25519.json
+-rw-r--r--   0        0        0      119 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_ed25519.pem
+-rw-r--r--   0        0        0      119 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_ed25519_2.pem
+-rw-r--r--   0        0        0     1732 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_rsa.json
+-rw-r--r--   0        0        0     1704 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_rsa.pem
+-rw-r--r--   0        0        0     1679 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_rsa_2.pem
+-rw-r--r--   0        0        0      119 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_x25519.pem
+-rw-r--r--   0        0        0      119 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/private_key_x25519_2.pem
+-rw-r--r--   0        0        0      255 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_ecdsa_p384.json
+-rw-r--r--   0        0        0      215 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_ecdsa_p384.pem
+-rw-r--r--   0        0        0      215 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_ecdsa_p384_2.pem
+-rw-r--r--   0        0        0      162 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_ed25519.json
+-rw-r--r--   0        0        0      113 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_ed25519.pem
+-rw-r--r--   0        0        0      113 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_ed25519_2.pem
+-rw-r--r--   0        0        0      454 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_rsa.json
+-rw-r--r--   0        0        0      451 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_rsa.pem
+-rw-r--r--   0        0        0      451 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_rsa_2.pem
+-rw-r--r--   0        0        0      113 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_x25519.pem
+-rw-r--r--   0        0        0      113 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/keys/public_key_x25519_2.pem
+-rw-r--r--   0        0        0    16770 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_key.py
+-rw-r--r--   0        0        0     2117 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_key_interface.py
+-rw-r--r--   0        0        0    17132 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_pyseto.py
+-rw-r--r--   0        0        0    21047 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_sample.py
+-rw-r--r--   0        0        0     2886 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_token.py
+-rw-r--r--   0        0        0      829 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_utils.py
+-rw-r--r--   0        0        0     7238 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_v1.py
+-rw-r--r--   0        0        0     9647 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_v2.py
+-rw-r--r--   0        0        0     8525 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_v3.py
+-rw-r--r--   0        0        0     4462 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_v4.py
+-rw-r--r--   0        0        0    20667 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/test_with_test_vectors.py
+-rw-r--r--   0        0        0      751 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/utils.py
+-rw-r--r--   0        0        0      630 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.lid.json
+-rw-r--r--   0        0        0      922 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.local-pw.json
+-rw-r--r--   0        0        0      898 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.local-wrap.pie.json
+-rw-r--r--   0        0        0      641 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.local.json
+-rw-r--r--   0        0        0      645 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.pid.json
+-rw-r--r--   0        0        0     1002 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.public.json
+-rw-r--r--   0        0        0    10283 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.seal.json
+-rw-r--r--   0        0        0     7289 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.secret-pw.json
+-rw-r--r--   0        0        0     7265 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.secret-wrap.pie.json
+-rw-r--r--   0        0        0     3921 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.secret.json
+-rw-r--r--   0        0        0     1886 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k1.sid.json
+-rw-r--r--   0        0        0      630 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.lid.json
+-rw-r--r--   0        0        0      922 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.local-pw.json
+-rw-r--r--   0        0        0      854 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.local-wrap.pie.json
+-rw-r--r--   0        0        0      641 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.local.json
+-rw-r--r--   0        0        0      630 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.pid.json
+-rw-r--r--   0        0        0      648 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.public.json
+-rw-r--r--   0        0        0     1135 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.seal.json
+-rw-r--r--   0        0        0     1141 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.secret-pw.json
+-rw-r--r--   0        0        0     1073 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.secret-wrap.pie.json
+-rw-r--r--   0        0        0     1512 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.secret.json
+-rw-r--r--   0        0        0     1068 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k2.sid.json
+-rw-r--r--   0        0        0      630 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.lid.json
+-rw-r--r--   0        0        0      922 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.local-pw.json
+-rw-r--r--   0        0        0      898 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.local-wrap.pie.json
+-rw-r--r--   0        0        0      641 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.local.json
+-rw-r--r--   0        0        0      508 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.pid.json
+-rw-r--r--   0        0        0      567 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.public.json
+-rw-r--r--   0        0        0     1859 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.seal.json
+-rw-r--r--   0        0        0     1937 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.secret-pw.json
+-rw-r--r--   0        0        0     1913 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.secret-wrap.pie.json
+-rw-r--r--   0        0        0     2163 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.secret.json
+-rw-r--r--   0        0        0     2082 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k3.sid.json
+-rw-r--r--   0        0        0      630 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.lid.json
+-rw-r--r--   0        0        0      922 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.local-pw.json
+-rw-r--r--   0        0        0      854 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.local-wrap.pie.json
+-rw-r--r--   0        0        0      641 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.local.json
+-rw-r--r--   0        0        0      630 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.pid.json
+-rw-r--r--   0        0        0      648 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.public.json
+-rw-r--r--   0        0        0     1135 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.seal.json
+-rw-r--r--   0        0        0     1141 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.secret-pw.json
+-rw-r--r--   0        0        0     1073 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.secret-wrap.pie.json
+-rw-r--r--   0        0        0     1512 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.secret.json
+-rw-r--r--   0        0        0     1068 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/PASERK/k4.sid.json
+-rw-r--r--   0        0        0    18232 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/v1.json
+-rw-r--r--   0        0        0    11135 2023-04-22 22:58:49.092261 pyseto-1.7.2/tests/vectors/v2.json
+-rw-r--r--   0        0        0    12741 2023-04-22 22:58:49.096261 pyseto-1.7.2/tests/vectors/v3.json
+-rw-r--r--   0        0        0    11643 2023-04-22 22:58:49.096261 pyseto-1.7.2/tests/vectors/v4.json
+-rw-r--r--   0        0        0     1134 2023-04-22 22:58:49.096261 pyseto-1.7.2/tox.ini
+-rw-r--r--   0        0        0    17417 1970-01-01 00:00:00.000000 pyseto-1.7.2/PKG-INFO
```

### Comparing `pyseto-1.7.1/CHANGES.rst` & `pyseto-1.7.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 Changes
 =======
 
 Unreleased
 ----------
 
-Version 1.7.0
+Version 1.7.2
 -------------
 
-Released 2022-01-21
+Released 2023-04-23
+
+- Update SECURITY.md. `#245 <https://github.com/dajiaji/pyseto/pull/245>`__
+- Add SECURITY.md. `#244 <https://github.com/dajiaji/pyseto/pull/244>`__
+- Fix CHANGES. `#233 <https://github.com/dajiaji/pyseto/pull/233>`__
+- Update dependencies.
+    - Bump cryptography to 40.0.2. `#262 <https://github.com/dajiaji/pyseto/pull/262>`__
+- Update dev dependencies.
+    - Bump pytest to 7.3.1. `#263 <https://github.com/dajiaji/pyseto/pull/263>`__
+    - Bump tox to 4.4.12. `#261 <https://github.com/dajiaji/pyseto/pull/261>`__
+    - Bump pre-commit/mirrors-mypy to 1.2.0. `#260 <https://github.com/dajiaji/pyseto/pull/260>`__
+    - Bump pre-commit/black to 23.3.0. `#256 <https://github.com/dajiaji/pyseto/pull/256>`__
+    - Bump sphinx-rtd-theme to 1.2.0. `#243 <https://github.com/dajiaji/pyseto/pull/243>`__
+    - Bump pre-commit/black to 23.1.0. `#240 <https://github.com/dajiaji/pyseto/pull/240>`__
+    - Bump pre-commit/isort to 5.12.0. `#237 <https://github.com/dajiaji/pyseto/pull/237>`__
+
+Version 1.7.1
+-------------
+
+Released 2023-01-21
 
 - Use allowlist_externals on tox. `#208 <https://github.com/dajiaji/pyseto/pull/208>`__
 
 - Update dependencies.
     - Bump cryptography to 39.0.0. `#212 <https://github.com/dajiaji/pyseto/pull/212>`__
 - Update dev dependencies.
     - Bump tox to 4.3.5. `#230 <https://github.com/dajiaji/pyseto/pull/230>`__
```

### Comparing `pyseto-1.7.1/LICENSE` & `pyseto-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/README.md` & `pyseto-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/docs/Makefile` & `pyseto-1.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/docs/conf.py` & `pyseto-1.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/docs/index.rst` & `pyseto-1.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/docs/paserk_usage.rst` & `pyseto-1.7.2/docs/paserk_usage.rst`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/docs/paseto_usage.rst` & `pyseto-1.7.2/docs/paseto_usage.rst`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/poetry.lock` & `pyseto-1.7.2/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -68,32 +68,14 @@
 cffi = ">=1.0.1"
 
 [package.extras]
 dev = ["cogapp", "pre-commit", "pytest", "wheel"]
 tests = ["pytest"]
 
 [[package]]
-name = "attrs"
-version = "21.4.0"
-description = "Classes Without Boilerplate"
-category = "dev"
-optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
-files = [
-    {file = "attrs-21.4.0-py2.py3-none-any.whl", hash = "sha256:2d27e3784d7a565d36ab851fe94887c5eccd6a463168875832a1be79c82828b4"},
-    {file = "attrs-21.4.0.tar.gz", hash = "sha256:626ba8234211db98e869df76230a137c4c40a12d72445c45d5f5b716f076e2fd"},
-]
-
-[package.extras]
-dev = ["cloudpickle", "coverage[toml] (>=5.0.2)", "furo", "hypothesis", "mypy", "pre-commit", "pympler", "pytest (>=4.3.0)", "pytest-mypy-plugins", "six", "sphinx", "sphinx-notfound-page", "zope.interface"]
-docs = ["furo", "sphinx", "sphinx-notfound-page", "zope.interface"]
-tests = ["cloudpickle", "coverage[toml] (>=5.0.2)", "hypothesis", "mypy", "pympler", "pytest (>=4.3.0)", "pytest-mypy-plugins", "six", "zope.interface"]
-tests-no-zope = ["cloudpickle", "coverage[toml] (>=5.0.2)", "hypothesis", "mypy", "pympler", "pytest (>=4.3.0)", "pytest-mypy-plugins", "six"]
-
-[[package]]
 name = "babel"
 version = "2.9.1"
 description = "Internationalization utilities"
 category = "main"
 optional = true
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 files = [
@@ -121,22 +103,22 @@
 
 [package.extras]
 html5lib = ["html5lib"]
 lxml = ["lxml"]
 
 [[package]]
 name = "cachetools"
-version = "5.2.1"
+version = "5.3.0"
 description = "Extensible memoizing collections and decorators"
 category = "dev"
 optional = false
 python-versions = "~=3.7"
 files = [
-    {file = "cachetools-5.2.1-py3-none-any.whl", hash = "sha256:8462eebf3a6c15d25430a8c27c56ac61340b2ecf60c9ce57afc2b97e450e47da"},
-    {file = "cachetools-5.2.1.tar.gz", hash = "sha256:5991bc0e08a1319bb618d3195ca5b6bc76646a49c21d55962977197b301cc1fe"},
+    {file = "cachetools-5.3.0-py3-none-any.whl", hash = "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"},
+    {file = "cachetools-5.3.0.tar.gz", hash = "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14"},
 ]
 
 [[package]]
 name = "certifi"
 version = "2022.12.7"
 description = "Python package for providing Mozilla's CA Bundle."
 category = "main"
@@ -325,55 +307,53 @@
 tomli = {version = "*", optional = true, markers = "python_full_version <= \"3.11.0a6\" and extra == \"toml\""}
 
 [package.extras]
 toml = ["tomli"]
 
 [[package]]
 name = "cryptography"
-version = "39.0.0"
+version = "40.0.2"
 description = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
 category = "main"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "cryptography-39.0.0-cp36-abi3-macosx_10_12_universal2.whl", hash = "sha256:c52a1a6f81e738d07f43dab57831c29e57d21c81a942f4602fac7ee21b27f288"},
-    {file = "cryptography-39.0.0-cp36-abi3-macosx_10_12_x86_64.whl", hash = "sha256:80ee674c08aaef194bc4627b7f2956e5ba7ef29c3cc3ca488cf15854838a8f72"},
-    {file = "cryptography-39.0.0-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:887cbc1ea60786e534b00ba8b04d1095f4272d380ebd5f7a7eb4cc274710fad9"},
-    {file = "cryptography-39.0.0-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6f97109336df5c178ee7c9c711b264c502b905c2d2a29ace99ed761533a3460f"},
-    {file = "cryptography-39.0.0-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1a6915075c6d3a5e1215eab5d99bcec0da26036ff2102a1038401d6ef5bef25b"},
-    {file = "cryptography-39.0.0-cp36-abi3-manylinux_2_24_x86_64.whl", hash = "sha256:76c24dd4fd196a80f9f2f5405a778a8ca132f16b10af113474005635fe7e066c"},
-    {file = "cryptography-39.0.0-cp36-abi3-manylinux_2_28_aarch64.whl", hash = "sha256:bae6c7f4a36a25291b619ad064a30a07110a805d08dc89984f4f441f6c1f3f96"},
-    {file = "cryptography-39.0.0-cp36-abi3-manylinux_2_28_x86_64.whl", hash = "sha256:875aea1039d78557c7c6b4db2fe0e9d2413439f4676310a5f269dd342ca7a717"},
-    {file = "cryptography-39.0.0-cp36-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:f6c0db08d81ead9576c4d94bbb27aed8d7a430fa27890f39084c2d0e2ec6b0df"},
-    {file = "cryptography-39.0.0-cp36-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:f3ed2d864a2fa1666e749fe52fb8e23d8e06b8012e8bd8147c73797c506e86f1"},
-    {file = "cryptography-39.0.0-cp36-abi3-win32.whl", hash = "sha256:f671c1bb0d6088e94d61d80c606d65baacc0d374e67bf895148883461cd848de"},
-    {file = "cryptography-39.0.0-cp36-abi3-win_amd64.whl", hash = "sha256:e324de6972b151f99dc078defe8fb1b0a82c6498e37bff335f5bc6b1e3ab5a1e"},
-    {file = "cryptography-39.0.0-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:754978da4d0457e7ca176f58c57b1f9de6556591c19b25b8bcce3c77d314f5eb"},
-    {file = "cryptography-39.0.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1ee1fd0de9851ff32dbbb9362a4d833b579b4a6cc96883e8e6d2ff2a6bc7104f"},
-    {file = "cryptography-39.0.0-pp38-pypy38_pp73-manylinux_2_24_x86_64.whl", hash = "sha256:fec8b932f51ae245121c4671b4bbc030880f363354b2f0e0bd1366017d891458"},
-    {file = "cryptography-39.0.0-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:407cec680e811b4fc829de966f88a7c62a596faa250fc1a4b520a0355b9bc190"},
-    {file = "cryptography-39.0.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:7dacfdeee048814563eaaec7c4743c8aea529fe3dd53127313a792f0dadc1773"},
-    {file = "cryptography-39.0.0-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:ad04f413436b0781f20c52a661660f1e23bcd89a0e9bb1d6d20822d048cf2856"},
-    {file = "cryptography-39.0.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50386acb40fbabbceeb2986332f0287f50f29ccf1497bae31cf5c3e7b4f4b34f"},
-    {file = "cryptography-39.0.0-pp39-pypy39_pp73-manylinux_2_24_x86_64.whl", hash = "sha256:e5d71c5d5bd5b5c3eebcf7c5c2bb332d62ec68921a8c593bea8c394911a005ce"},
-    {file = "cryptography-39.0.0-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:844ad4d7c3850081dffba91cdd91950038ee4ac525c575509a42d3fc806b83c8"},
-    {file = "cryptography-39.0.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:e0a05aee6a82d944f9b4edd6a001178787d1546ec7c6223ee9a848a7ade92e39"},
-    {file = "cryptography-39.0.0.tar.gz", hash = "sha256:f964c7dcf7802d133e8dbd1565914fa0194f9d683d82411989889ecd701e8adf"},
+    {file = "cryptography-40.0.2-cp36-abi3-macosx_10_12_universal2.whl", hash = "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b"},
+    {file = "cryptography-40.0.2-cp36-abi3-macosx_10_12_x86_64.whl", hash = "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440"},
+    {file = "cryptography-40.0.2-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d"},
+    {file = "cryptography-40.0.2-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288"},
+    {file = "cryptography-40.0.2-cp36-abi3-manylinux_2_28_aarch64.whl", hash = "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2"},
+    {file = "cryptography-40.0.2-cp36-abi3-manylinux_2_28_x86_64.whl", hash = "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b"},
+    {file = "cryptography-40.0.2-cp36-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"},
+    {file = "cryptography-40.0.2-cp36-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c"},
+    {file = "cryptography-40.0.2-cp36-abi3-win32.whl", hash = "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9"},
+    {file = "cryptography-40.0.2-cp36-abi3-win_amd64.whl", hash = "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b"},
+    {file = "cryptography-40.0.2-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b"},
+    {file = "cryptography-40.0.2-pp38-pypy38_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e"},
+    {file = "cryptography-40.0.2-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a"},
+    {file = "cryptography-40.0.2-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958"},
+    {file = "cryptography-40.0.2-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b"},
+    {file = "cryptography-40.0.2-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636"},
+    {file = "cryptography-40.0.2-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e"},
+    {file = "cryptography-40.0.2-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404"},
+    {file = "cryptography-40.0.2.tar.gz", hash = "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99"},
 ]
 
 [package.dependencies]
 cffi = ">=1.12"
 
 [package.extras]
-docs = ["sphinx (>=1.6.5,!=1.8.0,!=3.1.0,!=3.1.1,!=5.2.0,!=5.2.0.post0)", "sphinx-rtd-theme"]
+docs = ["sphinx (>=5.3.0)", "sphinx-rtd-theme (>=1.1.1)"]
 docstest = ["pyenchant (>=1.6.11)", "sphinxcontrib-spelling (>=4.0.1)", "twine (>=1.12.0)"]
-pep8test = ["black", "ruff"]
+pep8test = ["black", "check-manifest", "mypy", "ruff"]
 sdist = ["setuptools-rust (>=0.11.4)"]
 ssh = ["bcrypt (>=3.1.5)"]
-test = ["hypothesis (>=1.11.4,!=3.79.2)", "iso8601", "pretend", "pytest (>=6.2.0)", "pytest-benchmark", "pytest-cov", "pytest-subtests", "pytest-xdist", "pytz"]
+test = ["iso8601", "pretend", "pytest (>=6.2.0)", "pytest-benchmark", "pytest-cov", "pytest-shard (>=0.1.2)", "pytest-subtests", "pytest-xdist"]
+test-randomorder = ["pytest-randomly"]
+tox = ["tox"]
 
 [[package]]
 name = "distlib"
 version = "0.3.6"
 description = "Distribution utilities"
 category = "dev"
 optional = false
@@ -408,27 +388,27 @@
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "filelock"
-version = "3.9.0"
+version = "3.11.0"
 description = "A platform independent file lock."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "filelock-3.9.0-py3-none-any.whl", hash = "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"},
-    {file = "filelock-3.9.0.tar.gz", hash = "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de"},
+    {file = "filelock-3.11.0-py3-none-any.whl", hash = "sha256:f08a52314748335c6460fc8fe40cd5638b85001225db78c2aa01c8c0db83b318"},
+    {file = "filelock-3.11.0.tar.gz", hash = "sha256:3618c0da67adcc0506b015fd11ef7faf1b493f0b40d87728e19986b536890c37"},
 ]
 
 [package.extras]
-docs = ["furo (>=2022.12.7)", "sphinx (>=5.3)", "sphinx-autodoc-typehints (>=1.19.5)"]
-testing = ["covdefaults (>=2.2.2)", "coverage (>=7.0.1)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-timeout (>=2.1)"]
+docs = ["furo (>=2023.3.27)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
+testing = ["covdefaults (>=2.3)", "coverage (>=7.2.2)", "diff-cover (>=7.5)", "pytest (>=7.2.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)", "pytest-timeout (>=2.1)"]
 
 [[package]]
 name = "freezegun"
 version = "1.2.2"
 description = "Let your Python tests travel through time"
 category = "dev"
 optional = false
@@ -496,22 +476,22 @@
 files = [
     {file = "imagesize-1.3.0-py2.py3-none-any.whl", hash = "sha256:1db2f82529e53c3e929e8926a1fa9235aa82d0bd0c580359c67ec31b2fddaa8c"},
     {file = "imagesize-1.3.0.tar.gz", hash = "sha256:cd1750d452385ca327479d45b64d9c7729ecf0b3969a58148298c77092261f9d"},
 ]
 
 [[package]]
 name = "importlib-metadata"
-version = "6.0.0"
+version = "6.3.0"
 description = "Read metadata from Python packages"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "importlib_metadata-6.0.0-py3-none-any.whl", hash = "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad"},
-    {file = "importlib_metadata-6.0.0.tar.gz", hash = "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"},
+    {file = "importlib_metadata-6.3.0-py3-none-any.whl", hash = "sha256:8f8bd2af397cf33bd344d35cfe7f489219b7d14fc79a3f854b75b8417e9226b0"},
+    {file = "importlib_metadata-6.3.0.tar.gz", hash = "sha256:23c2bcae4762dfb0bbe072d358faec24957901d75b6c4ab11172c0c982532402"},
 ]
 
 [package.dependencies]
 typing-extensions = {version = ">=3.6.4", markers = "python_version < \"3.8\""}
 zipp = ">=0.5"
 
 [package.extras]
@@ -683,30 +663,30 @@
 argon2 = ["argon2-cffi (>=18.2.0)"]
 bcrypt = ["bcrypt (>=3.1.0)"]
 build-docs = ["cloud-sptheme (>=1.10.1)", "sphinx (>=1.6)", "sphinxcontrib-fulltoc (>=1.2.0)"]
 totp = ["cryptography"]
 
 [[package]]
 name = "platformdirs"
-version = "2.6.2"
+version = "3.2.0"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-2.6.2-py3-none-any.whl", hash = "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490"},
-    {file = "platformdirs-2.6.2.tar.gz", hash = "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"},
+    {file = "platformdirs-3.2.0-py3-none-any.whl", hash = "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"},
+    {file = "platformdirs-3.2.0.tar.gz", hash = "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08"},
 ]
 
 [package.dependencies]
-typing-extensions = {version = ">=4.4", markers = "python_version < \"3.8\""}
+typing-extensions = {version = ">=4.5", markers = "python_version < \"3.8\""}
 
 [package.extras]
-docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=5.3)", "sphinx-autodoc-typehints (>=1.19.5)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.2.2)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
+docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.2.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 description = "plugin and hook calling mechanisms for python"
 category = "dev"
 optional = false
@@ -805,56 +785,55 @@
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
 name = "pyproject-api"
-version = "1.5.0"
+version = "1.5.1"
 description = "API to interact with the python pyproject.toml based projects"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pyproject_api-1.5.0-py3-none-any.whl", hash = "sha256:4c111277dfb96bcd562c6245428f27250b794bfe3e210b8714c4f893952f2c17"},
-    {file = "pyproject_api-1.5.0.tar.gz", hash = "sha256:0962df21f3e633b8ddb9567c011e6c1b3dcdfc31b7860c0ede7e24c5a1200fbe"},
+    {file = "pyproject_api-1.5.1-py3-none-any.whl", hash = "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"},
+    {file = "pyproject_api-1.5.1.tar.gz", hash = "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9"},
 ]
 
 [package.dependencies]
-packaging = ">=21.3"
+packaging = ">=23"
 tomli = {version = ">=2.0.1", markers = "python_version < \"3.11\""}
 
 [package.extras]
-docs = ["furo (>=2022.9.29)", "sphinx (>=5.3)", "sphinx-autodoc-typehints (>=1.19.5)"]
-testing = ["covdefaults (>=2.2.2)", "importlib-metadata (>=5.1)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)", "virtualenv (>=20.17)", "wheel (>=0.38.4)"]
+docs = ["furo (>=2022.12.7)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
+testing = ["covdefaults (>=2.2.2)", "importlib-metadata (>=6)", "pytest (>=7.2.1)", "pytest-cov (>=4)", "pytest-mock (>=3.10)", "virtualenv (>=20.17.1)", "wheel (>=0.38.4)"]
 
 [[package]]
 name = "pytest"
-version = "7.2.1"
+version = "7.3.1"
 description = "pytest: simple powerful testing with Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pytest-7.2.1-py3-none-any.whl", hash = "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5"},
-    {file = "pytest-7.2.1.tar.gz", hash = "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"},
+    {file = "pytest-7.3.1-py3-none-any.whl", hash = "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362"},
+    {file = "pytest-7.3.1.tar.gz", hash = "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"},
 ]
 
 [package.dependencies]
-attrs = ">=19.2.0"
 colorama = {version = "*", markers = "sys_platform == \"win32\""}
 exceptiongroup = {version = ">=1.0.0rc8", markers = "python_version < \"3.11\""}
 importlib-metadata = {version = ">=0.12", markers = "python_version < \"3.8\""}
 iniconfig = "*"
 packaging = "*"
 pluggy = ">=0.12,<2.0"
 tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
 
 [package.extras]
-testing = ["argcomplete", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "xmlschema"]
+testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "xmlschema"]
 
 [[package]]
 name = "pytest-cov"
 version = "4.0.0"
 description = "Pytest plugin for measuring coverage."
 category = "dev"
 optional = false
@@ -967,14 +946,31 @@
 urllib3 = ">=1.21.1,<1.27"
 
 [package.extras]
 socks = ["PySocks (>=1.5.6,!=1.5.7)", "win-inet-pton"]
 use-chardet-on-py3 = ["chardet (>=3.0.2,<5)"]
 
 [[package]]
+name = "setuptools"
+version = "67.2.0"
+description = "Easily download, build, install, upgrade, and uninstall Python packages"
+category = "main"
+optional = true
+python-versions = ">=3.7"
+files = [
+    {file = "setuptools-67.2.0-py3-none-any.whl", hash = "sha256:16ccf598aab3b506593c17378473978908a2734d7336755a8769b480906bec1c"},
+    {file = "setuptools-67.2.0.tar.gz", hash = "sha256:b440ee5f7e607bb8c9de15259dba2583dd41a38879a7abc1d43a71c59524da48"},
+]
+
+[package.extras]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-lint", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
+testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
+testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
+
+[[package]]
 name = "six"
 version = "1.16.0"
 description = "Python 2 and 3 compatibility utilities"
 category = "dev"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 files = [
@@ -1100,27 +1096,28 @@
 sphinx = ">=4.0"
 
 [package.extras]
 docs = ["furo", "ipython", "myst-parser", "sphinx-copybutton", "sphinx-inline-tabs"]
 
 [[package]]
 name = "sphinx-rtd-theme"
-version = "1.1.1"
+version = "1.2.0"
 description = "Read the Docs theme for Sphinx"
 category = "main"
 optional = true
-python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,>=2.7"
+python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7"
 files = [
-    {file = "sphinx_rtd_theme-1.1.1-py2.py3-none-any.whl", hash = "sha256:31faa07d3e97c8955637fc3f1423a5ab2c44b74b8cc558a51498c202ce5cbda7"},
-    {file = "sphinx_rtd_theme-1.1.1.tar.gz", hash = "sha256:6146c845f1e1947b3c3dd4432c28998a1693ccc742b4f9ad7c63129f0757c103"},
+    {file = "sphinx_rtd_theme-1.2.0-py2.py3-none-any.whl", hash = "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"},
+    {file = "sphinx_rtd_theme-1.2.0.tar.gz", hash = "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8"},
 ]
 
 [package.dependencies]
-docutils = "<0.18"
-sphinx = ">=1.6,<6"
+docutils = "<0.19"
+sphinx = ">=1.6,<7"
+sphinxcontrib-jquery = {version = ">=2.0.0,<3.0.0 || >3.0.0", markers = "python_version > \"3\""}
 
 [package.extras]
 dev = ["bump2version", "sphinxcontrib-httpdomain", "transifex-client", "wheel"]
 
 [[package]]
 name = "sphinxcontrib-applehelp"
 version = "1.0.2"
@@ -1166,14 +1163,29 @@
 ]
 
 [package.extras]
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["html5lib", "pytest"]
 
 [[package]]
+name = "sphinxcontrib-jquery"
+version = "2.0.0"
+description = "Extension to include jQuery on newer Sphinx releases"
+category = "main"
+optional = true
+python-versions = ">=2.7"
+files = [
+    {file = "sphinxcontrib-jquery-2.0.0.tar.gz", hash = "sha256:8fb65f6dba84bf7bcd1aea1f02ab3955ac34611d838bcc95d4983b805b234daa"},
+    {file = "sphinxcontrib_jquery-2.0.0-py3-none-any.whl", hash = "sha256:ed47fa425c338ffebe3c37e1cdb56e30eb806116b85f01055b158c7057fdb995"},
+]
+
+[package.dependencies]
+setuptools = "*"
+
+[[package]]
 name = "sphinxcontrib-jsmath"
 version = "1.0.1"
 description = "A sphinx extension which renders display math in HTML via JavaScript"
 category = "main"
 optional = true
 python-versions = ">=3.5"
 files = [
@@ -1257,52 +1269,52 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tox"
-version = "4.3.5"
+version = "4.4.12"
 description = "tox is a generic virtualenv management and test command line tool"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "tox-4.3.5-py3-none-any.whl", hash = "sha256:6dddc4c69718b65aacbef0921ffa8af065b0f63ff0b24ffc403477975853c918"},
-    {file = "tox-4.3.5.tar.gz", hash = "sha256:307993257d792a12a63ff86a0b67a71a5ab2d4a2cc12bbae947115224d4ac3fb"},
+    {file = "tox-4.4.12-py3-none-any.whl", hash = "sha256:d4be558809d86fad13f4553976b0500352630a8fbfa39ea4b1ce3bd945ba680b"},
+    {file = "tox-4.4.12.tar.gz", hash = "sha256:740f5209d0dec19451b951ee5b1cce4a207acdc7357af84dbc8ec35bcf2c454e"},
 ]
 
 [package.dependencies]
-cachetools = ">=5.2.1"
+cachetools = ">=5.3"
 chardet = ">=5.1"
 colorama = ">=0.4.6"
-filelock = ">=3.9"
-importlib-metadata = {version = ">=6", markers = "python_version < \"3.8\""}
+filelock = ">=3.11"
+importlib-metadata = {version = ">=6.2", markers = "python_version < \"3.8\""}
 packaging = ">=23"
-platformdirs = ">=2.6.2"
+platformdirs = ">=3.2"
 pluggy = ">=1"
-pyproject-api = ">=1.5"
+pyproject-api = ">=1.5.1"
 tomli = {version = ">=2.0.1", markers = "python_version < \"3.11\""}
-typing-extensions = {version = ">=4.4", markers = "python_version < \"3.8\""}
-virtualenv = ">=20.17.1"
+typing-extensions = {version = ">=4.5", markers = "python_version < \"3.8\""}
+virtualenv = ">=20.21"
 
 [package.extras]
-docs = ["furo (>=2022.12.7)", "sphinx (>=6.1.3)", "sphinx-argparse-cli (>=1.11)", "sphinx-autodoc-typehints (>=1.20.1)", "sphinx-copybutton (>=0.5.1)", "sphinx-inline-tabs (>=2022.1.2b11)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=22.12)"]
-testing = ["build[virtualenv] (>=0.9)", "covdefaults (>=2.2.2)", "devpi-process (>=0.3)", "diff-cover (>=7.3)", "distlib (>=0.3.6)", "flaky (>=3.7)", "hatch-vcs (>=0.3)", "hatchling (>=1.12.2)", "psutil (>=5.9.4)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)", "pytest-xdist (>=3.1)", "re-assert (>=1.1)", "time-machine (>=2.8.2)", "wheel (>=0.38.4)"]
+docs = ["furo (>=2023.3.27)", "sphinx (>=6.1.3)", "sphinx-argparse-cli (>=1.11)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)", "sphinx-copybutton (>=0.5.1)", "sphinx-inline-tabs (>=2022.1.2b11)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=22.12)"]
+testing = ["build[virtualenv] (>=0.10)", "covdefaults (>=2.3)", "devpi-process (>=0.3)", "diff-cover (>=7.5)", "distlib (>=0.3.6)", "flaky (>=3.7)", "hatch-vcs (>=0.3)", "hatchling (>=1.14)", "psutil (>=5.9.4)", "pytest (>=7.2.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)", "pytest-xdist (>=3.2.1)", "re-assert (>=1.1)", "time-machine (>=2.9)", "wheel (>=0.40)"]
 
 [[package]]
 name = "typing-extensions"
-version = "4.4.0"
+version = "4.5.0"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "typing_extensions-4.4.0-py3-none-any.whl", hash = "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"},
-    {file = "typing_extensions-4.4.0.tar.gz", hash = "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa"},
+    {file = "typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
+    {file = "typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
 ]
 
 [[package]]
 name = "urllib3"
 version = "1.26.8"
 description = "HTTP library with thread-safe connection pooling, file post, and more."
 category = "main"
@@ -1316,33 +1328,33 @@
 [package.extras]
 brotli = ["brotlipy (>=0.6.0)"]
 secure = ["certifi", "cryptography (>=1.3.4)", "idna (>=2.0.0)", "ipaddress", "pyOpenSSL (>=0.14)"]
 socks = ["PySocks (>=1.5.6,!=1.5.7,<2.0)"]
 
 [[package]]
 name = "virtualenv"
-version = "20.17.1"
+version = "20.21.0"
 description = "Virtual Python Environment builder"
 category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "virtualenv-20.17.1-py3-none-any.whl", hash = "sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4"},
-    {file = "virtualenv-20.17.1.tar.gz", hash = "sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058"},
+    {file = "virtualenv-20.21.0-py3-none-any.whl", hash = "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc"},
+    {file = "virtualenv-20.21.0.tar.gz", hash = "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"},
 ]
 
 [package.dependencies]
 distlib = ">=0.3.6,<1"
 filelock = ">=3.4.1,<4"
 importlib-metadata = {version = ">=4.8.3", markers = "python_version < \"3.8\""}
-platformdirs = ">=2.4,<3"
+platformdirs = ">=2.4,<4"
 
 [package.extras]
-docs = ["proselint (>=0.13)", "sphinx (>=5.3)", "sphinx-argparse (>=0.3.2)", "sphinx-rtd-theme (>=1)", "towncrier (>=22.8)"]
-testing = ["coverage (>=6.2)", "coverage-enable-subprocess (>=1)", "flaky (>=3.7)", "packaging (>=21.3)", "pytest (>=7.0.1)", "pytest-env (>=0.6.2)", "pytest-freezegun (>=0.4.2)", "pytest-mock (>=3.6.1)", "pytest-randomly (>=3.10.3)", "pytest-timeout (>=2.1)"]
+docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-argparse (>=0.4)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=22.12)"]
+test = ["covdefaults (>=2.2.2)", "coverage (>=7.1)", "coverage-enable-subprocess (>=1)", "flaky (>=3.7)", "packaging (>=23)", "pytest (>=7.2.1)", "pytest-env (>=0.8.1)", "pytest-freezegun (>=0.4.2)", "pytest-mock (>=3.10)", "pytest-randomly (>=3.12)", "pytest-timeout (>=2.1)"]
 
 [[package]]
 name = "zipp"
 version = "3.6.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
 category = "main"
 optional = false
@@ -1358,8 +1370,8 @@
 
 [extras]
 docs = ["Sphinx", "sphinx-rtd-theme", "sphinx-autodoc-typehints"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.7"
-content-hash = "9e5191e7fbbe013d10975bdf69133de78b3b60719d0b2356e860a90a25d60842"
+content-hash = "16b5abf1b8d07bfb925b2e72732df5aae28368a89b6c1d014c26d5084a25463e"
```

### Comparing `pyseto-1.7.1/pyproject.toml` & `pyseto-1.7.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyseto"
-version = "1.7.1"
+version = "1.7.2"
 description = "A Python implementation of PASETO/PASERK."
 authors = ["Ajitomi Daisuke <dajiaji@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dajiaji/pyseto"
 
 include = [
@@ -21,15 +21,15 @@
 
 exclude = [
   "docs/_build",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-cryptography = ">=36,<40"
+cryptography = ">=36,<41"
 pycryptodomex = "^3.12.0"
 passlib = {extras = ["argon2"], version = "^1.7.4"}
 iso8601 = "^1.0.2"
 Sphinx = {version = ">=4.3.2,<6.0.0", optional = true, extras = ["docs"]}
 sphinx-autodoc-typehints = {version = "1.21.0", optional = true, extras = ["docs"]}
 sphinx-rtd-theme = {version = "^1.0.0", optional = true, extras = ["docs"]}
 
@@ -37,12 +37,12 @@
 docs = [
   "Sphinx",
   "sphinx-rtd-theme",
   "sphinx-autodoc-typehints",
 ]
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2"
+pytest = "^7.3"
 pytest-cov = "^4.0.0"
-tox = "^4.3.5"
+tox = "^4.4.12"
 pre-commit = "^2.20.0"
 freezegun = "^1.2.2"
```

### Comparing `pyseto-1.7.1/pyseto/__init__.py` & `pyseto-1.7.2/pyseto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 )
 from .key import Key
 from .key_interface import KeyInterface
 from .paseto import Paseto
 from .pyseto import decode, encode
 from .token import Token
 
-__version__ = "1.7.1"
+__version__ = "1.7.2"
 __title__ = "PySETO"
 __description__ = "A Python implementation of PASETO/PASERK."
 __url__ = "https://pyseto.readthedocs.io"
 __uri__ = __url__
 __doc__ = __description__ + " <" + __uri__ + ">"
 __author__ = "AJITOMI Daisuke"
 __email__ = "ajitomi@gmail.com"
```

### Comparing `pyseto-1.7.1/pyseto/exceptions.py` & `pyseto-1.7.2/pyseto/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/pyseto/key.py` & `pyseto-1.7.2/pyseto/key.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         "secret-wrap",
         "local-pw",
         "secret-pw",
     ]
 
     @classmethod
     def new(cls, version: int, purpose: str, key: Union[bytes, str] = b"") -> KeyInterface:
-
         """
         Constructor of a PASETO key object which has
         :class:`KeyInterface <pyseto.key_interface.KeyInterface>`.
 
         Args:
             version(int): The version of the key. It will be ``1``,
                 ``2``, ``3`` or ``4``.
@@ -75,15 +74,14 @@
     def from_paserk(
         cls,
         paserk: str,
         wrapping_key: Union[bytes, str] = b"",
         password: Union[bytes, str] = b"",
         unsealing_key: Union[bytes, str] = b"",
     ) -> KeyInterface:
-
         """
         Generates a PASETO key object which has
         :class:`KeyInterface <pyseto.key_interface.KeyInterface>` from PASERK.
 
         Args:
             paserk (str): A PASERK string.
             wrapping_key (Union[bytes, str]): A wrapping key. If the
@@ -141,15 +139,14 @@
     #         return V3Public.from_public_bytes(key)
     #     if version == 4:
     #         return V4Public.from_public_bytes(key)
     #     raise ValueError(f"Invalid version: {version}.")
 
     @staticmethod
     def from_asymmetric_key_params(version: int, x: bytes = b"", y: bytes = b"", d: bytes = b"") -> KeyInterface:
-
         """
         Constructor of a PASETO key object which has
         :class:`KeyInterface <pyseto.key_interface.KeyInterface>` wth
         asymmetric key parameters (x-coordinate, y-coordinate, and/or private
         key). This is intended to be used to generate keys for PASETO from JWK
         and other sources.
```

### Comparing `pyseto-1.7.1/pyseto/key_interface.py` & `pyseto-1.7.2/pyseto/key_interface.py`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/pyseto/key_nist.py` & `pyseto-1.7.2/pyseto/key_nist.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,27 +22,25 @@
     NIST (v1, v3) PASETO key.
     """
 
     # _VERSION = 1 or 3
     # _TYPE = "local", "public" or "secret"
 
     def __init__(self, key: Any):
-
         super().__init__(self._VERSION, self._TYPE, key)
         return
 
     @classmethod
     def from_paserk(
         cls,
         paserk: str,
         wrapping_key: bytes = b"",
         password: bytes = b"",
         unsealing_key: bytes = b"",
     ) -> KeyInterface:
-
         if wrapping_key and password:
             raise ValueError("Only one of wrapping_key or password should be specified.")
 
         frags = paserk.split(".")
         if frags[0] != f"k{cls._VERSION}":
             raise ValueError(f"Invalid PASERK version: {frags[0]}.")
 
@@ -91,15 +89,14 @@
         password: Union[bytes, str] = b"",
         sealing_key: Union[bytes, str] = b"",
         iteration: int = 100000,
         memory_cost: int = 15 * 1024,
         time_cost: int = 2,
         parallelism: int = 1,
     ) -> str:
-
         if wrapping_key and password:
             raise ValueError("Only one of wrapping_key or password should be specified.")
 
         # local-wrap
         if wrapping_key:
             bkey = wrapping_key if isinstance(wrapping_key, bytes) else wrapping_key.encode("utf-8")
             h = f"k{self.version}.local-wrap.pie."
@@ -123,28 +120,26 @@
 
         # local
         h = f"k{self.version}.local."
         return h + base64url_encode(self._key).decode("utf-8")
 
     @classmethod
     def _encode_pie(cls, header: str, wrapping_key: bytes, ptk: bytes) -> str:
-
         h = header.encode("utf-8")
         n = token_bytes(32)
         x = cls._generate_hash(wrapping_key, b"\x80" + n)
         ek = x[0:32]
         n2 = x[32:]
         ak = cls._generate_hash(wrapping_key, b"\x81" + n, 32)
         c = cls._encrypt(ek, n2, ptk)
         t = cls._generate_hash(ak, h + n + c, 48)
         return base64url_encode(t + n + c).decode("utf-8")
 
     @classmethod
     def _decode_pie(cls, header: str, wrapping_key: bytes, data: str) -> bytes:
-
         h = header.encode("utf-8")
         d = base64url_decode(data)
         t = d[0:48]
         n = d[48:80]
         c = d[80:]
         ak = cls._generate_hash(wrapping_key, b"\x81" + n, 32)
         t2 = cls._generate_hash(ak, h + n + c, 48)
@@ -153,15 +148,14 @@
         x = cls._generate_hash(wrapping_key, b"\x80" + n)
         ek = x[0:32]
         n2 = x[32:]
         return cls._decrypt(ek, n2, c)
 
     @classmethod
     def _encode_pbkw(cls, header: str, password: bytes, ptk: bytes, iteration: int = 100000) -> str:
-
         h = header.encode("utf-8")
 
         s = token_bytes(32)
         k = PBKDF2HMAC(
             algorithm=hashes.SHA384(),
             length=32,
             salt=s,
@@ -173,15 +167,14 @@
         edk = cls._encrypt(ek, n, ptk)
         bi = iteration.to_bytes(4, byteorder="big")
         t = cls._generate_hash(ak, h + s + bi + n + edk, 48)
         return base64url_encode(s + bi + n + edk + t).decode("utf-8")
 
     @classmethod
     def _decode_pbkw(cls, header: str, password: bytes, data: str) -> bytes:
-
         h = header.encode("utf-8")
         d = base64url_decode(data)
 
         s = d[0:32]
         bi = d[32:36]
         n = d[36:52]
         edk = d[52 : len(d) - 48]
@@ -259,15 +252,14 @@
     #     tmp = cls._digest(b"\x01" + h + xk + epk + pk)
     #     ek = tmp[0:32]
     #     n = tmp[32:]
     #     return cls._decrypt(ek, n, edk)
 
     @staticmethod
     def _generate_hash(key: bytes, msg: bytes, size: int = 0) -> bytes:
-
         try:
             d = hmac.new(key, msg, hashlib.sha384).digest()
             return d[0:size] if size > 0 else d
         except Exception as err:
             raise EncryptError("Failed to generate hash.") from err
 
     @staticmethod
```

### Comparing `pyseto-1.7.1/pyseto/key_sodium.py` & `pyseto-1.7.2/pyseto/key_sodium.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,25 @@
     Sodium (v2, v4) PASETO key.
     """
 
     # _VERSION = 2 or 4
     # _TYPE = "local", "public" or "secret"
 
     def __init__(self, key: Any):
-
         super().__init__(self._VERSION, self._TYPE, key)
         return
 
     @classmethod
     def from_paserk(
         cls,
         paserk: str,
         wrapping_key: bytes = b"",
         password: bytes = b"",
         unsealing_key: bytes = b"",
     ) -> KeyInterface:
-
         if wrapping_key and password:
             raise ValueError("Only one of wrapping_key or password should be specified.")
 
         frags = paserk.split(".")
         if frags[0] != f"k{cls._VERSION}":
             raise ValueError(f"Invalid PASERK version: {frags[0]}.")
 
@@ -130,15 +128,14 @@
         password: Union[bytes, str] = b"",
         sealing_key: Union[bytes, str] = b"",
         iteration: int = 100000,
         memory_cost: int = 15 * 1024,
         time_cost: int = 2,
         parallelism: int = 1,
     ) -> str:
-
         if wrapping_key and password:
             raise ValueError("Only one of wrapping_key or password should be specified.")
 
         if wrapping_key:
             # local-wrap
             bkey = wrapping_key if isinstance(wrapping_key, bytes) else wrapping_key.encode("utf-8")
             if self.purpose == "local":
@@ -225,28 +222,26 @@
             encoding=serialization.Encoding.Raw,
             format=serialization.PublicFormat.Raw,
         )
         return h + base64url_encode(priv + pub).decode("utf-8")
 
     @classmethod
     def _encode_pie(cls, header: str, wrapping_key: bytes, ptk: bytes) -> str:
-
         h = header.encode("utf-8")
         n = token_bytes(32)
         x = cls._generate_hash(wrapping_key, b"\x80" + n, 56)
         ek = x[0:32]
         n2 = x[32:]
         ak = cls._generate_hash(wrapping_key, b"\x81" + n, 32)
         c = cls._encrypt(ek, n2, ptk)
         t = cls._generate_hash(ak, h + n + c, 32)
         return base64url_encode(t + n + c).decode("utf-8")
 
     @classmethod
     def _decode_pie(cls, header: str, wrapping_key: bytes, data: str) -> bytes:
-
         h = header.encode("utf-8")
         d = base64url_decode(data)
         t = d[0:32]
         n = d[32:64]
         c = d[64:]
         ak = cls._generate_hash(wrapping_key, b"\x81" + n, 32)
 
@@ -265,15 +260,14 @@
         header: str,
         password: bytes,
         ptk: bytes,
         memory_cost: int,
         time_cost: int,
         parallelism: int,
     ) -> str:
-
         h = header.encode("utf-8")
         s = token_bytes(16)
         argon2_k = argon2.using(
             salt=s,
             memory_cost=memory_cost,
             time_cost=time_cost,
             parallelism=parallelism,
@@ -289,15 +283,14 @@
         time = time_cost.to_bytes(4, byteorder="big")
         para = parallelism.to_bytes(4, byteorder="big")
         t = cls._generate_hash(ak, h + s + mem + time + para + n + edk, 32)
         return base64url_encode(s + mem + time + para + n + edk + t).decode("utf-8")
 
     @classmethod
     def _decode_pbkw(cls, header: str, password: bytes, data: str) -> bytes:
-
         h = header.encode("utf-8")
         d = base64url_decode(data)
 
         s = d[0:16]
         mem = d[16:24]
         time = d[24:28]
         para = d[28:32]
@@ -327,15 +320,14 @@
     @classmethod
     def _encode_pke(
         cls,
         header: str,
         sealing_key: bytes,
         ptk: bytes,
     ) -> str:
-
         h = header.encode("utf-8")
 
         xpk = X25519PublicKey.from_public_bytes(sealing_key)
         esk = X25519PrivateKey.generate()
         epk = esk.public_key().public_bytes(Encoding.Raw, PublicFormat.Raw)
         xk = esk.exchange(xpk)
 
@@ -345,15 +337,14 @@
 
         edk = cls._encrypt(ek, n, ptk)
         t = cls._generate_hash(ak, h + epk + edk, 32)
         return base64url_encode(t + epk + edk).decode("utf-8")
 
     @classmethod
     def _decode_pke(cls, header: str, unsealing_key: bytes, data: str) -> bytes:
-
         h = header.encode("utf-8")
         d = base64url_decode(data)
 
         t = d[0:32]
         epk = d[32:64]
         edk = d[64:]
 
@@ -368,39 +359,35 @@
 
         ek = cls._digest(b"\x01" + h + xk + epk + xpk, 32)
         n = cls._digest(epk + xpk, 24)
         return cls._decrypt(ek, n, edk)
 
     @staticmethod
     def _generate_hash(key: bytes, msg: bytes, size: int) -> bytes:
-
         try:
             h = hashlib.blake2b(key=key, digest_size=size)
             h.update(msg)
             return h.digest()
         except Exception as err:
             raise EncryptError("Failed to generate hash.") from err
 
     @staticmethod
     def _digest(msg: bytes, size: int) -> bytes:
-
         h = hashlib.blake2b(digest_size=size)
         h.update(msg)
         return h.digest()
 
     @staticmethod
     def _encrypt(key: bytes, nonce: bytes, msg: bytes) -> bytes:
-
         try:
             cipher = ChaCha20.new(key=key, nonce=nonce)
             return cipher.encrypt(msg)
         except Exception as err:
             raise EncryptError("Failed to encrypt.") from err
 
     @staticmethod
     def _decrypt(key: bytes, nonce: bytes, msg: bytes) -> bytes:
-
         try:
             cipher = ChaCha20.new(key=key, nonce=nonce)
             return cipher.decrypt(msg)
         except Exception as err:
             raise DecryptError("Failed to decrypt.") from err
```

### Comparing `pyseto-1.7.1/pyseto/paseto.py` & `pyseto-1.7.2/pyseto/paseto.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         payload: Union[bytes, str, dict],
         footer: Union[bytes, str, dict] = b"",
         implicit_assertion: Union[bytes, str] = b"",
         nonce: bytes = b"",
         serializer: Any = json,
         exp: int = 0,
     ) -> bytes:
-
         """
         Encodes a message to a PASETO token with a key for encryption or signing.
 
         Args:
             key (KeyInterface): A key for encryption or signing.
             payload (Union[bytes, str, dict]): A message to be encrypted or signed.
             footer (Union[bytes, str, dict]): A footer.
@@ -152,15 +151,14 @@
         self,
         keys: Union[KeyInterface, List[KeyInterface]],
         token: Union[bytes, str],
         implicit_assertion: Union[bytes, str] = b"",
         deserializer: Optional[Any] = None,
         aud: str = "",
     ) -> Token:
-
         """
         Decodes a PASETO token with a key for decryption and/or verifying.
 
         Args:
             keys (KeyInterface): A key for decryption or verifying the signature in the token.
             token (Union[bytes, str]): A PASETO token to be decrypted or verified.
             implicit_assertion (Union[bytes, str]): An implicit assertion. It is
@@ -219,28 +217,26 @@
             except Exception as err:
                 failed = err
         if failed:
             raise failed
         raise ValueError("key is not found for verifying the token.")
 
     def _set_registered_claims(self, claims: dict, exp: int) -> dict:
-
         now = datetime.now(tz=timezone.utc)
         # exp
         if exp > 0:
             claims["exp"] = (now + timedelta(seconds=exp)).isoformat(timespec="seconds")
         elif self._exp > 0:
             claims["exp"] = (now + timedelta(seconds=self._exp)).isoformat(timespec="seconds")
         # iat
         if self._include_iat:
             claims["iat"] = now.isoformat(timespec="seconds")
         return claims
 
     def _verify_registered_claims(self, claims: dict, aud: str):
-
         now = iso8601.parse_date(datetime.now(tz=timezone.utc).isoformat(timespec="seconds"))
         # In Python 3.7 or later, the following code can be used:
         # now = datetime.fromisoformat(
         #     datetime.now(tz=timezone.utc).isoformat(timespec="seconds")
         # )
         if "exp" in claims:
             try:
```

### Comparing `pyseto-1.7.1/pyseto/pyseto.py` & `pyseto-1.7.2/pyseto/pyseto.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     payload: Union[bytes, str, dict],
     footer: Union[bytes, str] = b"",
     implicit_assertion: Union[bytes, str] = b"",
     nonce: bytes = b"",
     serializer: Any = json,
     exp: int = 0,
 ) -> bytes:
-
     """
     Encodes a message to a PASETO token with a key for encryption or signing.
 
     Args:
         key (KeyInterface): A key for encryption or signing.
         payload (Union[bytes, str, dict]): A message to be encrypted or signed.
         footer (Union[bytes, str]): A footer.
@@ -52,15 +51,14 @@
 def decode(
     keys: Union[KeyInterface, List[KeyInterface]],
     token: Union[bytes, str],
     implicit_assertion: Union[bytes, str] = b"",
     deserializer: Optional[Any] = None,
     aud: str = "",
 ) -> Token:
-
     """
     Decodes a PASETO token with a key for decryption and/or verifying.
 
     Args:
         keys (KeyInterface): A key for decryption or verifying the signature in the token.
         token (Union[bytes, str]): A PASETO token to be decrypted or verified.
         implicit_assertion (Union[bytes, str]): An implicit assertion. It is
```

### Comparing `pyseto-1.7.1/pyseto/token.py` & `pyseto-1.7.2/pyseto/token.py`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/pyseto/utils.py` & `pyseto-1.7.2/pyseto/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,13 +56,12 @@
     for i in range(len(pieces)):
         output += _le64(len(pieces[i]))
         output += pieces[i]
     return output
 
 
 def ec_public_key_compress(x: int, y: int) -> bytes:
-
     bx = x.to_bytes(48, byteorder="big")
     by = y.to_bytes((y.bit_length() + 7) // 8, byteorder="big")
     s = bytearray(1)
     s[0] = 0x02 + (by[len(by) - 1] & 1)
     return bytes(s) + bx
```

### Comparing `pyseto-1.7.1/pyseto/versions/v1.py` & `pyseto-1.7.2/pyseto/versions/v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     The key object for v1.local.
     """
 
     _VERSION = 1
     _TYPE = "local"
 
     def __init__(self, key: Union[str, bytes]):
-
         super().__init__(key)
         return
 
     def to_paserk_id(self) -> str:
         h = "k1.lid."
         p = self.to_paserk()
         digest = hashes.Hash(hashes.SHA384())
@@ -42,15 +41,14 @@
     def encrypt(
         self,
         payload: bytes,
         footer: bytes = b"",
         implicit_assertion: bytes = b"",
         nonce: bytes = b"",
     ) -> bytes:
-
         if nonce:
             if len(nonce) != 32:
                 raise ValueError("nonce must be 32 bytes long.")
         else:
             nonce = token_bytes(32)
 
         n = self._generate_hash(nonce, payload, 32)
@@ -74,15 +72,14 @@
         t = hmac.new(ak, pre_auth, hashlib.sha384).digest()
         token = self._header + base64url_encode(n + c + t)
         if footer:
             token += b"." + base64url_encode(footer)
         return token
 
     def decrypt(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b"") -> bytes:
-
         n = payload[0:32]
         t = payload[-48:]
         c = payload[32 : len(payload) - 48]
         e = HKDF(
             algorithm=hashes.SHA384(),
             length=32,
             salt=n[0:16],
@@ -109,15 +106,14 @@
     The key object for v1.public.
     """
 
     _VERSION = 1
     _TYPE = "public"
 
     def __init__(self, key: Any):
-
         super().__init__(key)
 
         self._sig_size = 256
         if not isinstance(self._key, (RSAPublicKey, RSAPrivateKey)):
             raise ValueError("The key is not RSA key.")
 
         if isinstance(self._key, RSAPublicKey):
@@ -130,15 +126,14 @@
     def from_paserk(
         cls,
         paserk: str,
         wrapping_key: bytes = b"",
         password: bytes = b"",
         unsealing_key: bytes = b"",
     ) -> KeyInterface:
-
         if wrapping_key and password:
             raise ValueError("Only one of wrapping_key or password should be specified.")
 
         frags = paserk.split(".")
         if frags[0] != "k1":
             raise ValueError(f"Invalid PASERK version: {frags[0]}.")
 
@@ -179,15 +174,14 @@
         password: Union[bytes, str] = b"",
         sealing_key: Union[bytes, str] = b"",
         iteration: int = 100000,
         memory_cost: int = 15 * 1024,
         time_cost: int = 2,
         parallelism: int = 1,
     ) -> str:
-
         if wrapping_key and password:
             raise ValueError("Only one of wrapping_key or password should be specified.")
 
         if wrapping_key:
             # secret-wrap
             if not isinstance(self._key, RSAPrivateKey):
                 raise ValueError("Public key cannot be wrapped.")
@@ -252,25 +246,23 @@
         h = "k1.pid."
         digest = hashes.Hash(hashes.SHA384())
         digest.update((h + p).encode("utf-8"))
         d = digest.finalize()
         return h + base64url_encode(d[0:33]).decode("utf-8")
 
     def sign(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b"") -> bytes:
-
         if isinstance(self._key, RSAPublicKey):
             raise ValueError("A public key cannot be used for signing.")
         m2 = pae([self.header, payload, footer])
         try:
             return self._key.sign(m2, self._padding, hashes.SHA384())
         except Exception as err:
             raise SignError("Failed to sign.") from err
 
     def verify(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b""):
-
         if len(payload) <= self._sig_size:
             raise ValueError("Invalid payload.")
 
         sig = payload[-self._sig_size :]
         m = payload[: len(payload) - self._sig_size]
         k = self._key if isinstance(self._key, RSAPublicKey) else self._key.public_key()
         m2 = pae([self.header, m, footer])
```

### Comparing `pyseto-1.7.1/pyseto/versions/v2.py` & `pyseto-1.7.2/pyseto/versions/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     The key object for v2.local.
     """
 
     _VERSION = 2
     _TYPE = "local"
 
     def __init__(self, key: Union[str, bytes]):
-
         super().__init__(key)
         if len(self._key) != 32:
             raise ValueError("key must be 32 bytes long.")
         return
 
     def to_paserk_id(self) -> str:
         h = "k2.lid."
@@ -41,15 +40,14 @@
     def encrypt(
         self,
         payload: bytes,
         footer: bytes = b"",
         implicit_assertion: bytes = b"",
         nonce: bytes = b"",
     ) -> bytes:
-
         n = self._generate_nonce(nonce, payload)
         pre_auth = pae([self.header, n, footer])
 
         try:
             cipher = ChaCha20_Poly1305.new(key=self._key, nonce=n)
             cipher.update(pre_auth)
             c, tag = cipher.encrypt_and_digest(payload)
@@ -57,30 +55,28 @@
             if footer:
                 token += b"." + base64url_encode(footer)
             return token
         except Exception as err:
             raise EncryptError("Failed to encrypt.") from err
 
     def decrypt(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b"") -> bytes:
-
         n = payload[0:24]
         c = payload[24 : len(payload) - 16]
         tag = payload[-16:]
         pre_auth = pae([self.header, n, footer])
 
         try:
             cipher = ChaCha20_Poly1305.new(key=self._key, nonce=n)
             cipher.update(pre_auth)
             return cipher.decrypt_and_verify(c, tag)
         except Exception as err:
             raise DecryptError("Failed to decrypt.") from err
 
     @staticmethod
     def _generate_nonce(key: bytes, msg: bytes) -> bytes:
-
         if key:
             if len(key) != 24:
                 raise ValueError("nonce must be 24 bytes long.")
         else:
             key = token_bytes(24)
 
         try:
@@ -96,15 +92,14 @@
     The key object for v2.public.
     """
 
     _VERSION = 2
     _TYPE = "public"
 
     def __init__(self, key: Any):
-
         super().__init__(key)
         self._sig_size = 64
 
         if not isinstance(self._key, (Ed25519PublicKey, Ed25519PrivateKey)):
             raise ValueError("The key is not Ed25519 key.")
 
         if isinstance(self._key, Ed25519PublicKey):
@@ -141,25 +136,23 @@
     #     try:
     #         k = Ed25519PublicKey.from_public_bytes(key)
     #     except Exception as err:
     #         raise ValueError("Invalid bytes for the key.") from err
     #     return cls(k)
 
     def sign(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b"") -> bytes:
-
         if isinstance(self._key, Ed25519PublicKey):
             raise ValueError("A public key cannot be used for signing.")
         m2 = pae([self.header, payload, footer])
         try:
             return self._key.sign(m2)
         except Exception as err:
             raise SignError("Failed to sign.") from err
 
     def verify(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b""):
-
         if len(payload) <= self._sig_size:
             raise ValueError("Invalid payload.")
 
         sig = payload[-self._sig_size :]
         m = payload[: len(payload) - self._sig_size]
         k = self._key if isinstance(self._key, Ed25519PublicKey) else self._key.public_key()
         m2 = pae([self.header, m, footer])
```

### Comparing `pyseto-1.7.1/pyseto/versions/v3.py` & `pyseto-1.7.2/pyseto/versions/v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,26 +33,24 @@
     The key object for v3.local.
     """
 
     _VERSION = 3
     _TYPE = "local"
 
     def __init__(self, key: Union[str, bytes]):
-
         super().__init__(key)
         return
 
     def encrypt(
         self,
         payload: bytes,
         footer: bytes = b"",
         implicit_assertion: bytes = b"",
         nonce: bytes = b"",
     ) -> bytes:
-
         if nonce:
             if len(nonce) != 32:
                 raise ValueError("nonce must be 32 bytes long.")
         else:
             nonce = token_bytes(32)
         e = HKDF(
             algorithm=hashes.SHA384(),
@@ -79,15 +77,14 @@
         t = hmac.new(ak, pre_auth, hashlib.sha384).digest()
         token = self._header + base64url_encode(nonce + c + t)
         if footer:
             token += b"." + base64url_encode(footer)
         return token
 
     def decrypt(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b"") -> bytes:
-
         n = payload[0:32]
         c = payload[32 : len(payload) - 48]
         t = payload[-48:]
         e = HKDF(
             algorithm=hashes.SHA384(),
             length=48,
             salt=None,
@@ -110,15 +107,14 @@
         pre_auth = pae([self.header, n, c, footer, implicit_assertion])
         t2 = hmac.new(ak, pre_auth, hashlib.sha384).digest()
         if not hmac.compare_digest(t, t2):
             raise DecryptError("Failed to decrypt.")
         return self._decrypt(ek, n2, c)
 
     def to_paserk_id(self) -> str:
-
         h = "k3.lid."
         p = self.to_paserk()
         digest = hashes.Hash(hashes.SHA384())
         digest.update((h + p).encode("utf-8"))
         d = digest.finalize()
         return h + base64url_encode(d[0:33]).decode("utf-8")
 
@@ -128,15 +124,14 @@
     The key object for v3.public.
     """
 
     _VERSION = 3
     _TYPE = "public"
 
     def __init__(self, key: Any):
-
         super().__init__(key)
 
         self._sig_size = 96
         if not isinstance(self._key, (EllipticCurvePublicKey, EllipticCurvePrivateKey)):
             raise ValueError("The key is not ECDSA key.")
 
         if isinstance(self._key, EllipticCurvePublicKey):
@@ -155,15 +150,14 @@
     def from_paserk(
         cls,
         paserk: str,
         wrapping_key: bytes = b"",
         password: bytes = b"",
         unsealing_key: bytes = b"",
     ) -> KeyInterface:
-
         if wrapping_key and password:
             raise ValueError("Only one of wrapping_key or password should be specified.")
 
         frags = paserk.split(".")
         if frags[0] != "k3":
             raise ValueError(f"Invalid PASERK version: {frags[0]}.")
 
@@ -213,15 +207,14 @@
         password: Union[bytes, str] = b"",
         sealing_key: Union[bytes, str] = b"",
         iteration: int = 100000,
         memory_cost: int = 15 * 1024,
         time_cost: int = 2,
         parallelism: int = 1,
     ) -> str:
-
         if wrapping_key and password:
             raise ValueError("Only one of wrapping_key or password should be specified.")
 
         if wrapping_key:
             # secret-wrap
             if not isinstance(self._key, EllipticCurvePrivateKey):
                 raise ValueError("Public key cannot be wrapped.")
@@ -269,30 +262,28 @@
         h = "k3.pid."
         digest = hashes.Hash(hashes.SHA384())
         digest.update((h + p).encode("utf-8"))
         d = digest.finalize()
         return h + base64url_encode(d[0:33]).decode("utf-8")
 
     def sign(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b"") -> bytes:
-
         if isinstance(self._key, EllipticCurvePublicKey):
             raise ValueError("A public key cannot be used for signing.")
         pk = ec_public_key_compress(
             self._key.private_numbers().public_numbers.x,
             self._key.private_numbers().public_numbers.y,
         )
         m2 = pae([pk, self.header, payload, footer, implicit_assertion])
         try:
             sig = self._key.sign(m2, ec.ECDSA(hashes.SHA384()))
             return self._der_to_os(self._key.curve.key_size, sig)
         except Exception as err:
             raise SignError("Failed to sign.") from err
 
     def verify(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b""):
-
         if len(payload) <= self._sig_size:
             raise ValueError("Invalid payload.")
 
         sig = payload[-self._sig_size :]
         m = payload[: len(payload) - self._sig_size]
         k = self._key if isinstance(self._key, EllipticCurvePublicKey) else self._key.public_key()
         pk = ec_public_key_compress(k.public_numbers().x, k.public_numbers().y)
@@ -301,20 +292,18 @@
             der_sig = self._os_to_der(self._key.curve.key_size, sig)
             k.verify(der_sig, m2, ec.ECDSA(hashes.SHA384()))
         except Exception as err:
             raise VerifyError("Failed to verify.") from err
         return m
 
     def _der_to_os(self, key_size: int, sig: bytes) -> bytes:
-
         num_bytes = (key_size + 7) // 8
         r, s = decode_dss_signature(sig)
         return i2osp(r, num_bytes) + i2osp(s, num_bytes)
 
     def _os_to_der(self, key_size: int, sig: bytes) -> bytes:
-
         num_bytes = (key_size + 7) // 8
         if len(sig) != 2 * num_bytes:
             raise ValueError("Invalid signature.")
         r = os2ip(sig[:num_bytes])
         s = os2ip(sig[num_bytes:])
         return encode_dss_signature(r, s)
```

### Comparing `pyseto-1.7.1/pyseto/versions/v4.py` & `pyseto-1.7.2/pyseto/versions/v4.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     The key object for v4.local.
     """
 
     _VERSION = 4
     _TYPE = "local"
 
     def __init__(self, key: Union[str, bytes]):
-
         super().__init__(key)
         if len(self._key) > 64:
             raise ValueError("key length must be up to 64 bytes.")
         return
 
     def to_paserk_id(self) -> str:
         h = "k4.lid."
@@ -40,15 +39,14 @@
     def encrypt(
         self,
         payload: bytes,
         footer: bytes = b"",
         implicit_assertion: bytes = b"",
         nonce: bytes = b"",
     ) -> bytes:
-
         if nonce:
             if len(nonce) != 32:
                 raise ValueError("nonce must be 32 bytes long.")
         else:
             nonce = token_bytes(32)
         tmp = self._generate_hash(self._key, b"paseto-encryption-key" + nonce, 56)
         ek = tmp[0:32]
@@ -60,15 +58,14 @@
         t = self._generate_hash(ak, pre_auth, 32)
         token = self._header + base64url_encode(nonce + c + t)
         if footer:
             token += b"." + base64url_encode(footer)
         return token
 
     def decrypt(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b"") -> bytes:
-
         n = payload[0:32]
         c = payload[32 : len(payload) - 32]
         t = payload[-32:]
         tmp = self._generate_hash(self._key, b"paseto-encryption-key" + n, 56)
         ek = tmp[0:32]
         n2 = tmp[32:]
         ak = self._generate_hash(self._key, b"paseto-auth-key-for-aead" + n, 32)
@@ -84,15 +81,14 @@
     The key object for v4.public.
     """
 
     _VERSION = 4
     _TYPE = "public"
 
     def __init__(self, key: Any):
-
         super().__init__(key)
         self._sig_size = 64
 
         if not isinstance(self._key, (Ed25519PublicKey, Ed25519PrivateKey)):
             raise ValueError("The key is not Ed25519 key.")
 
         if isinstance(self._key, Ed25519PublicKey):
@@ -129,26 +125,24 @@
         h2 = "k4.pid."
         b = hashlib.blake2b(digest_size=33)
         b.update((h2 + p).encode("utf-8"))
         d = b.digest()
         return h2 + base64url_encode(d).decode("utf-8")
 
     def sign(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b"") -> bytes:
-
         if isinstance(self._key, Ed25519PublicKey):
             raise ValueError("A public key cannot be used for signing.")
 
         m2 = pae([self.header, payload, footer, implicit_assertion])
         try:
             return self._key.sign(m2)
         except Exception as err:
             raise SignError("Failed to sign.") from err
 
     def verify(self, payload: bytes, footer: bytes = b"", implicit_assertion: bytes = b""):
-
         if len(payload) <= self._sig_size:
             raise ValueError("Invalid payload.")
 
         sig = payload[-self._sig_size :]
         m = payload[: len(payload) - self._sig_size]
         k = self._key if isinstance(self._key, Ed25519PublicKey) else self._key.public_key()
         m2 = pae([self.header, m, footer, implicit_assertion])
```

### Comparing `pyseto-1.7.1/tests/keys/private_key_rsa.json` & `pyseto-1.7.2/tests/keys/private_key_rsa.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/keys/private_key_rsa.pem` & `pyseto-1.7.2/tests/keys/private_key_rsa.pem`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/keys/private_key_rsa_2.pem` & `pyseto-1.7.2/tests/keys/private_key_rsa_2.pem`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/test_key.py` & `pyseto-1.7.2/tests/test_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,14 @@
             (3, load_jwk("keys/private_key_ecdsa_p384.json")),
             (3, load_jwk("keys/public_key_ecdsa_p384.json")),
             (4, load_jwk("keys/private_key_ed25519.json")),
             (4, load_jwk("keys/public_key_ed25519.json")),
         ],
     )
     def test_key_from_asymmetric_params(self, version, key):
-
         k = Key.from_asymmetric_key_params(version, x=key["x"], y=key["y"], d=key["d"])
         assert isinstance(k, KeyInterface)
         assert k.version == version
         assert k.purpose == "public"
 
     @pytest.mark.parametrize(
         "paserk",
@@ -187,15 +186,14 @@
             "k3.local.AAAAAAAAAAAAAAAA",
             "k3.public.AAAAAAAAAAAAAAAA",
             "k4.local.AAAAAAAAAAAAAAAA",
             "k4.public.AAAAAAAAAAAAAAAA",
         ],
     )
     def test_key_from_paserk_with_wrapping_key_and_password(self, paserk):
-
         with pytest.raises(ValueError) as err:
             Key.from_paserk(paserk, wrapping_key="xxx", password="yyy")
             pytest.fail("Key.from_paserk should fail.")
         assert "Only one of wrapping_key or password should be specified." in str(err.value)
 
     @pytest.mark.parametrize(
         "paserk, msg",
@@ -207,30 +205,28 @@
             ("k3.local.AAAAAAAAAAAAAAAA", "Invalid PASERK type: local."),
             ("k3.public.AAAAAAAAAAAAAAAA", "Invalid PASERK type: public."),
             ("k4.local.AAAAAAAAAAAAAAAA", "Invalid PASERK type: local."),
             ("k4.public.AAAAAAAAAAAAAAAA", "Invalid PASERK type: public."),
         ],
     )
     def test_key_from_paserk_with_password_for_wrong_paserk(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             Key.from_paserk(paserk, password="yyy")
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     @pytest.mark.parametrize(
         "paserk, msg",
         [
             ("v1.local.AAAAAAAAAAAAAAAA", "Invalid PASERK version: v1."),
             ("*.local.AAAAAAAAAAAAAAAA", "Invalid PASERK version: *."),
             ("k1.xxx.AAAAAAAAAAAAAAAA", "Invalid PASERK key type: xxx."),
         ],
     )
     def test_key_from_paserk_with_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             Key.from_paserk(paserk)
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     @pytest.mark.parametrize(
         "version",
@@ -376,15 +372,14 @@
                 4,
                 {"x": b"", "y": b"", "d": b""},
                 "x or d should be set for v4.public.",
             ),
         ],
     )
     def test_key_from_asymmetric_params_with_invalid_arg(self, version, key, msg):
-
         with pytest.raises(ValueError) as err:
             Key.from_asymmetric_key_params(version, x=key["x"], y=key["y"], d=key["d"])
             pytest.fail("Key.from_asymmetric_key_params() should fail.")
         assert msg in str(err.value)
 
     @pytest.mark.parametrize(
         "version, purpose, key",
```

### Comparing `pyseto-1.7.1/tests/test_key_interface.py` & `pyseto-1.7.2/tests/test_key_interface.py`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/test_pyseto.py` & `pyseto-1.7.2/tests/test_pyseto.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,14 @@
         )
         public_key = Key.new(version=4, purpose="public", key=public_key_pem)
         decoded = pyseto.decode(public_key, token, deserializer=json)
         assert isinstance(decoded.footer, bytes)
         assert decoded.footer == b"This is a footer."
 
     def test_decode_object_payload_with_invalid_exp(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
             {"data": "this is a signed message", "exp": "xxxxx"},
@@ -267,15 +266,14 @@
         public_key = Key.new(version=4, purpose="public", key=public_key_pem)
         with pytest.raises(VerifyError) as err:
             pyseto.decode(public_key, token, deserializer=json)
             pytest.fail("pyseto.decode() should fail.")
         assert "Invalid exp." in str(err.value)
 
     def test_decode_object_payload_with_expired_exp(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
             {"data": "this is a signed message"},
@@ -285,29 +283,27 @@
         public_key = Key.new(version=4, purpose="public", key=public_key_pem)
         with pytest.raises(VerifyError) as err:
             pyseto.decode(public_key, token, deserializer=json)
             pytest.fail("pyseto.decode() should fail.")
         assert "Token expired." in str(err.value)
 
     def test_decode_object_payload_with_aud(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
             {"data": "this is a signed message", "aud": "12345"},
         )
         public_key = Key.new(version=4, purpose="public", key=public_key_pem)
         decoded = pyseto.decode(public_key, token, deserializer=json, aud="12345")
         assert decoded.payload["aud"] == "12345"
 
     def test_decode_object_payload_without_aud(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
             {"data": "this is a signed message"},
@@ -315,15 +311,14 @@
         public_key = Key.new(version=4, purpose="public", key=public_key_pem)
         with pytest.raises(VerifyError) as err:
             pyseto.decode(public_key, token, deserializer=json, aud="12345")
             pytest.fail("pyseto.decode() should fail.")
         assert "aud verification failed." in str(err.value)
 
     def test_decode_object_payload_with_invalid_aud(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
             {"data": "this is a signed message", "aud": "12345"},
@@ -331,15 +326,14 @@
         public_key = Key.new(version=4, purpose="public", key=public_key_pem)
         with pytest.raises(VerifyError) as err:
             pyseto.decode(public_key, token, deserializer=json, aud="1234x")
             pytest.fail("pyseto.decode() should fail.")
         assert "aud verification failed." in str(err.value)
 
     def test_decode_object_payload_with_invalid_nbf(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
             {"data": "this is a signed message", "nbf": "xxxxx"},
@@ -347,15 +341,14 @@
         public_key = Key.new(version=4, purpose="public", key=public_key_pem)
         with pytest.raises(VerifyError) as err:
             pyseto.decode(public_key, token, deserializer=json)
             pytest.fail("pyseto.decode() should fail.")
         assert "Invalid nbf." in str(err.value)
 
     def test_decode_object_payload_with_future_nbf(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         now = datetime.now(tz=timezone.utc)
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
```

### Comparing `pyseto-1.7.1/tests/test_sample.py` & `pyseto-1.7.2/tests/test_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,24 @@
 
 class TestSample:
     """
     Tests for sample code.
     """
 
     def test_sample_v4_local_old(self):
-
         key = Key.new(4, "local", b"our-secret")
         token = pyseto.encode(
             key,
             b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
         )
 
         decoded = pyseto.decode(key, token)
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
 
     def test_sample_v4_public_old(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         private_key = Key.new(4, "public", private_key_pem)
         token = pyseto.encode(
             private_key,
             b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
@@ -44,26 +42,24 @@
         assert (
             token
             == b"v4.public.eyJkYXRhIjogInRoaXMgaXMgYSBzaWduZWQgbWVzc2FnZSIsICJleHAiOiAiMjAyMi0wMS0wMVQwMDowMDowMCswMDowMCJ9l1YiKei2FESvHBSGPkn70eFO1hv3tXH0jph1IfZyEfgm3t1DjkYqD5r4aHWZm1eZs_3_bZ9pBQlZGp0DPSdzDg"
         )
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
 
     def test_sample_v4_local(self):
-
         key = Key.new(version=4, purpose="local", key=b"our-secret")
         token = pyseto.encode(
             key,
             b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
         )
 
         decoded = pyseto.decode(key, token)
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
 
     def test_sample_v4_public(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
             b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
@@ -75,15 +71,14 @@
             token
             == b"v4.public.eyJkYXRhIjogInRoaXMgaXMgYSBzaWduZWQgbWVzc2FnZSIsICJleHAiOiAiMjAyMi0wMS0wMVQwMDowMDowMCswMDowMCJ9l1YiKei2FESvHBSGPkn70eFO1hv3tXH0jph1IfZyEfgm3t1DjkYqD5r4aHWZm1eZs_3_bZ9pBQlZGp0DPSdzDg"
         )
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
 
     @freezegun.freeze_time("2021-01-01")
     def test_sample_v4_public_with_serializer(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
             {"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"},
@@ -95,25 +90,23 @@
             token
             == b"v4.public.eyJkYXRhIjogInRoaXMgaXMgYSBzaWduZWQgbWVzc2FnZSIsICJleHAiOiAiMjAyMi0wMS0wMVQwMDowMDowMCswMDowMCJ9l1YiKei2FESvHBSGPkn70eFO1hv3tXH0jph1IfZyEfgm3t1DjkYqD5r4aHWZm1eZs_3_bZ9pBQlZGp0DPSdzDg"
         )
         assert decoded.payload["data"] == "this is a signed message"
         assert decoded.payload["exp"] == "2022-01-01T00:00:00+00:00"
 
     def test_sample_v4_local_with_serializer(self):
-
         key = Key.new(version=4, purpose="local", key=b"out-secret")
         token = pyseto.encode(
             key,
             {"data": "this is a signed message"},
         )
         decoded = pyseto.decode(key, token, deserializer=json)
         assert decoded.payload["data"] == "this is a signed message"
 
     def test_sample_v4_public_with_serializer_and_exp(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
         now = datetime.now(tz=timezone.utc)
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         token = pyseto.encode(
             private_key,
@@ -123,15 +116,14 @@
         public_key = Key.new(version=4, purpose="public", key=public_key_pem)
         decoded = pyseto.decode(public_key, token, deserializer=json)
 
         assert decoded.payload["data"] == "this is a signed message"
         assert iso8601.parse_date(decoded.payload["exp"]) >= now + timedelta(seconds=3600 - 1)
 
     def test_sample_v4_public_with_paseto_class(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
         now = datetime.now(tz=timezone.utc)
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         paseto = Paseto.new(exp=3600, include_iat=True)
         token = paseto.encode(
@@ -143,15 +135,14 @@
 
         assert decoded.payload["data"] == "this is a signed message"
         assert "iat" in decoded.payload
         assert "exp" in decoded.payload
         assert iso8601.parse_date(decoded.payload["exp"]) >= now + timedelta(seconds=3600 - 1)
 
     def test_sample_v4_public_with_paseto_class_and_leeway(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
         now = datetime.now(tz=timezone.utc)
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         paseto = Paseto.new(exp=1, include_iat=True, leeway=1)
         token = paseto.encode(
@@ -164,15 +155,14 @@
 
         assert decoded.payload["data"] == "this is a signed message"
         assert "iat" in decoded.payload
         assert "exp" in decoded.payload
         assert iso8601.parse_date(decoded.payload["exp"]) >= now
 
     def test_sample_v4_public_with_kid(self):
-
         private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
         public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
         now = datetime.now(tz=timezone.utc)
 
         private_key = Key.new(version=4, purpose="public", key=private_key_pem)
         public_key = Key.new(version=4, purpose="public", key=public_key_pem)
         paseto = Paseto.new(exp=3600, include_iat=True)
@@ -190,15 +180,14 @@
         assert "iat" in decoded.payload
         assert "exp" in decoded.payload
         assert "kid" in decoded.footer
         assert decoded.footer["kid"] == "k4.pid.yh4-bJYjOYAG6CWy0zsfPmpKylxS7uAWrxqVmBN2KAiJ"
         assert iso8601.parse_date(decoded.payload["exp"]) >= now
 
     def test_sample_paserk(self):
-
         symmetric_key = Key.new(version=4, purpose="local", key=b"our-secret")
         private_key = Key.from_paserk(
             "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"
         )
         public_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")
 
         token = pyseto.encode(
@@ -212,27 +201,25 @@
         assert (
             private_key.to_paserk()
             == "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"
         )
         assert public_key.to_paserk() == "k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI"
 
     def test_sample_paserk_id(self):
-
         symmetric_key = Key.new(version=4, purpose="local", key=b"our-secret")
         private_key = Key.from_paserk(
             "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"
         )
         public_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")
 
         assert symmetric_key.to_paserk_id() == "k4.lid._D6kgTzxgiPGk35gMj9bukgj4En2H94u22wVX9zaoh05"
         assert private_key.to_paserk_id() == "k4.sid.9gZFsAQuXhu9lif2pV3rCDjOewsMF4qb4RHGhc0zUklt"
         assert public_key.to_paserk_id() == "k4.pid.yh4-bJYjOYAG6CWy0zsfPmpKylxS7uAWrxqVmBN2KAiJ"
 
     def test_sample_paserk_key_wrapping_local(self):
-
         raw_key = Key.new(version=4, purpose="local", key=b"our-secret")
         wrapping_key = token_bytes(32)
         wpk = raw_key.to_paserk(wrapping_key=wrapping_key)
 
         # assert wpk == "k4.local-wrap.pie.TNKEwC4K1xBcgJ_GiwWAoRlQFE33HJO3oN9DHEZ05pieSCd-W7bgAL64VG9TZ_pBkuNBFHNrfOGHtnfnhYGdbz5-x3CxShhPJxg"
 
         unwrapped_key = Key.from_paserk(wpk, wrapping_key=wrapping_key)
@@ -240,15 +227,14 @@
             raw_key,
             b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
         )
         decoded = pyseto.decode(unwrapped_key, token)
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
 
     def test_sample_paserk_key_wrapping_public(self):
-
         raw_private_key = Key.from_paserk(
             "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"
         )
         public_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")
         wrapping_key = token_bytes(32)
         wpk = raw_private_key.to_paserk(wrapping_key=wrapping_key)
 
@@ -259,30 +245,28 @@
             unwrapped_private_key,
             b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
         )
         decoded = pyseto.decode(public_key, token)
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
 
     def test_sample_paserk_password_local(self):
-
         raw_key = Key.new(version=4, purpose="local", key=b"our-secret")
         wpk = raw_key.to_paserk(password="our-secret")
 
         # assert wpk == "k4.local-pw.HrCs9Pu-2LB0l7jkHB-x2gAAAAAA8AAAAAAAAgAAAAGttW0IHZjQCHJdg-Vc3tqO_GSLR4vzLl-yrKk2I-l8YHj6jWpC0lQB2Z7uzTtVyV1rd_EZQPzHdw5VOtyucP0FkCU"
 
         unwrapped_key = Key.from_paserk(wpk, password="our-secret")
         token = pyseto.encode(
             raw_key,
             b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
         )
         decoded = pyseto.decode(unwrapped_key, token)
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
 
     def test_sample_paserk_password_public(self):
-
         raw_private_key = Key.from_paserk(
             "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"
         )
         public_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")
         wpk = raw_private_key.to_paserk(password="our-secret")
 
         # assert wpk == "k4.secret-pw.MEMW4K1MaD5nWigCLyEyFAAAAAAA8AAAAAAAAgAAAAFU-tArtryNVjS2n2hCYiM11V6tOyuIog69Bjb0yNZanrLJ3afGclb3kPzQ6IhK8ob9E4QgRdEALGWCizZ0RCPFF_M95IQDfmdYKC0Er656UgKUK4UKG9JlxP4o81UwoJoZYz_D1zTlltipEa5RiNvUtNU8vLKoGSY"
@@ -292,30 +276,28 @@
             unwrapped_private_key,
             b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
         )
         decoded = pyseto.decode(public_key, token)
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
 
     def test_sample_paserk_seal(self):
-
         raw_key = Key.new(version=4, purpose="local", key=b"our-secret")
         token = pyseto.encode(
             raw_key,
             b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
         )
         with open(get_path("keys/public_key_x25519.pem")) as key_file:
             sealed_key = raw_key.to_paserk(sealing_key=key_file.read())
 
         with open(get_path("keys/private_key_x25519.pem")) as key_file:
             unsealed_key = Key.from_paserk(sealed_key, unsealing_key=key_file.read())
         decoded = pyseto.decode(unsealed_key, token)
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
 
     def test_sample_rtd_v4_public(self):
-
         with open(get_path("keys/private_key_ed25519.pem")) as key_file:
             private_key = Key.new(4, "public", key_file.read())
         token = pyseto.encode(
             private_key,
             payload=b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
             footer=b"This is a footer",  # Optional
             implicit_assertion=b"xyz",  # Optional
@@ -327,15 +309,14 @@
 
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
         assert decoded.footer == b"This is a footer"
         assert decoded.version == "v4"
         assert decoded.purpose == "public"
 
     def test_sample_rtd_v4_local(self):
-
         key = Key.new(version=4, purpose="local", key=b"our-secret")
         token = pyseto.encode(
             key,
             payload=b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
             footer=b"This is a footer",  # Optional
             implicit_assertion=b"xyz",  # Optional
         )
@@ -344,15 +325,14 @@
 
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
         assert decoded.footer == b"This is a footer"
         assert decoded.version == "v4"
         assert decoded.purpose == "local"
 
     def test_sample_rtd_v3_public(self):
-
         with open(get_path("keys/private_key_ecdsa_p384.pem")) as key_file:
             private_key = Key.new(3, "public", key_file.read())
         token = pyseto.encode(
             private_key,
             payload=b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
             footer=b"This is a footer",  # Optional
             implicit_assertion=b"xyz",  # Optional
@@ -364,15 +344,14 @@
 
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
         assert decoded.footer == b"This is a footer"
         assert decoded.version == "v3"
         assert decoded.purpose == "public"
 
     def test_sample_rtd_v3_local(self):
-
         key = Key.new(version=3, purpose="local", key=b"our-secret")
         token = pyseto.encode(
             key,
             payload=b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
             footer=b"This is a footer",  # Optional
             implicit_assertion=b"xyz",  # Optional
         )
@@ -381,15 +360,14 @@
 
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
         assert decoded.footer == b"This is a footer"
         assert decoded.version == "v3"
         assert decoded.purpose == "local"
 
     def test_sample_rtd_v2_public(self):
-
         with open(get_path("keys/private_key_ed25519.pem")) as key_file:
             private_key = Key.new(2, "public", key_file.read())
         token = pyseto.encode(
             private_key,
             payload=b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
             footer=b"This is a footer",  # Optional
         )
@@ -400,15 +378,14 @@
 
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
         assert decoded.footer == b"This is a footer"
         assert decoded.version == "v2"
         assert decoded.purpose == "public"
 
     def test_sample_rtd_v2_local(self):
-
         key = Key.new(version=2, purpose="local", key=token_bytes(32))
         token = pyseto.encode(
             key,
             payload=b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
             footer=b"This is a footer",  # Optional
         )
 
@@ -416,15 +393,14 @@
 
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
         assert decoded.footer == b"This is a footer"
         assert decoded.version == "v2"
         assert decoded.purpose == "local"
 
     def test_sample_rtd_v1_public(self):
-
         with open(get_path("keys/private_key_rsa.pem")) as key_file:
             private_key = Key.new(1, "public", key_file.read())
         token = pyseto.encode(
             private_key,
             payload=b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
             footer=b"This is a footer",  # Optional
         )
@@ -435,15 +411,14 @@
 
         assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
         assert decoded.footer == b"This is a footer"
         assert decoded.version == "v1"
         assert decoded.purpose == "public"
 
     def test_sample_rtd_v1_local(self):
-
         key = Key.new(version=1, purpose="local", key=b"our-secret")
         token = pyseto.encode(
             key,
             payload=b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
             footer=b"This is a footer",  # Optional
         )
```

### Comparing `pyseto-1.7.1/tests/test_token.py` & `pyseto-1.7.2/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/test_utils.py` & `pyseto-1.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/test_v1.py` & `pyseto-1.7.2/tests/test_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,14 @@
             (
                 "k1.local-pw.AAAAAAAAAAAAAAAA",
                 "local-pw needs password.",
             ),
         ],
     )
     def test_vl_local_from_paserk_with_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V1Local.from_paserk(paserk)
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     @pytest.mark.parametrize(
         "paserk, msg",
@@ -121,15 +120,14 @@
             ("xx.local-wrap.AAAAAAAAAAAAAAAA", "Invalid PASERK version: xx."),
             ("k1.local-wrap.AAAAAAAAAAAAAAAA", "Invalid PASERK format."),
             ("k1.local-wrap.xxx.AAAAAAAAAAAAAAAA", "Unknown wrapping algorithm: xxx."),
             ("k1.xxx.pie.AAAAAAAAAAAAAAAA", "Invalid PASERK type: xxx."),
         ],
     )
     def test_v1_local_from_paserk_with_wrapping_key_and_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V1Local.from_paserk(paserk, wrapping_key=token_bytes(32))
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     def test_v1_local_to_peer_paserk_id(self):
         k = Key.new(1, "local", b"our-secret")
@@ -172,15 +170,14 @@
             (
                 "k1.secret-wrap.AAAAAAAAAAAAAAAA",
                 "secret-wrap needs wrapping_key.",
             ),
         ],
     )
     def test_vl_public_from_paserk_with_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V1Public.from_paserk(paserk)
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     @pytest.mark.parametrize(
         "paserk, msg",
@@ -188,12 +185,11 @@
             ("xx.secret-wrap.pie.AAAAAAAAAAAAAAAA", "Invalid PASERK version: xx."),
             ("k1.secret-wrap.AAAAAAAAAAAAAAAA", "Invalid PASERK format."),
             ("k1.secret-wrap.xxx.AAAAAAAAAAAAAAAA", "Unknown wrapping algorithm: xxx."),
             ("k1.xxx.pie.AAAAAAAAAAAAAAAA", "Invalid PASERK type: xxx."),
         ],
     )
     def test_v1_public_from_paserk_with_wrapping_key_and_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V1Public.from_paserk(paserk, wrapping_key=token_bytes(32))
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
```

### Comparing `pyseto-1.7.1/tests/test_v2.py` & `pyseto-1.7.2/tests/test_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
             (
                 "k2.seal.AAAAAAAAAAAAAAAA",
                 "seal needs unsealing_key.",
             ),
         ],
     )
     def test_v2_local_from_paserk_with_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V2Local.from_paserk(paserk)
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     @pytest.mark.parametrize(
         "paserk, msg",
@@ -131,44 +130,40 @@
             ("xx.local-wrap.AAAAAAAAAAAAAAAA", "Invalid PASERK version: xx."),
             ("k2.local-wrap.AAAAAAAAAAAAAAAA", "Invalid PASERK format."),
             ("k2.local-wrap.xxx.AAAAAAAAAAAAAAAA", "Unknown wrapping algorithm: xxx."),
             ("k2.xxx.pie.AAAAAAAAAAAAAAAA", "Invalid PASERK type: xxx."),
         ],
     )
     def test_v2_local_from_paserk_with_wrapping_key_and_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V2Local.from_paserk(paserk, wrapping_key=token_bytes(32))
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     @pytest.mark.parametrize(
         "paserk, msg",
         [
             ("k2.xxx.AAAAAAAAAAAAAAAA", "Invalid PASERK type: xxx."),
             ("k2.seal.AAAAAAAAAAAAAAAA", "Invalid or unsupported PEM format."),
         ],
     )
     def test_v2_local_from_paserk_with_unsealing_key_and_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V2Local.from_paserk(paserk, unsealing_key=token_bytes(32))
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     def test_v2_local_to_paserk_with_invalid_sealing_key(self):
-
         k = Key.new(2, "local", token_bytes(32))
         with pytest.raises(ValueError) as err:
             k.to_paserk(sealing_key=b"not-PEM-formatted-key")
             pytest.fail("Key.from_paserk should fail.")
         assert "Invalid or unsupported PEM format." in str(err.value)
 
     def test_v2_local_from_paserk_with_wrong_unsealing_key(self):
-
         k = Key.new(2, "local", token_bytes(32))
         with open(get_path("keys/public_key_x25519.pem")) as key_file:
             sealed_key = k.to_paserk(sealing_key=key_file.read())
 
         with open(get_path("keys/private_key_x25519_2.pem")) as key_file:
             unsealing_key = key_file.read()
 
@@ -240,12 +235,11 @@
             (
                 "k2.secret-pw.AAAAAAAAAAAAAAAA",
                 "secret-pw needs password.",
             ),
         ],
     )
     def test_v2_public_from_paserk_with_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V2Public.from_paserk(paserk)
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
```

### Comparing `pyseto-1.7.1/tests/test_v3.py` & `pyseto-1.7.2/tests/test_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,14 @@
             (
                 "k3.local-pw.AAAAAAAAAAAAAAAA",
                 "local-pw needs password.",
             ),
         ],
     )
     def test_v3_local_from_paserk_with_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V3Local.from_paserk(paserk)
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     @pytest.mark.parametrize(
         "paserk, msg",
@@ -95,15 +94,14 @@
             ("xx.local-wrap.AAAAAAAAAAAAAAAA", "Invalid PASERK version: xx."),
             ("k3.local-wrap.AAAAAAAAAAAAAAAA", "Invalid PASERK format."),
             ("k3.local-wrap.xxx.AAAAAAAAAAAAAAAA", "Unknown wrapping algorithm: xxx."),
             ("k3.xxx.pie.AAAAAAAAAAAAAAAA", "Invalid PASERK type: xxx."),
         ],
     )
     def test_v3_local_from_paserk_with_wrapping_key_and_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V3Local.from_paserk(paserk, wrapping_key=token_bytes(32))
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     def test_v3_local_to_peer_paserk_id(self):
         k = Key.new(3, "local", b"our-secret")
@@ -175,15 +173,14 @@
             (
                 "k3.secret-wrap.AAAAAAAAAAAAAAAA",
                 "secret-wrap needs wrapping_key.",
             ),
         ],
     )
     def test_v3_public_from_paserk_with_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V3Public.from_paserk(paserk)
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     @pytest.mark.parametrize(
         "paserk, msg",
@@ -191,29 +188,26 @@
             ("xx.secret-wrap.pie.AAAAAAAAAAAAAAAA", "Invalid PASERK version: xx."),
             ("k3.secret-wrap.AAAAAAAAAAAAAAAA", "Invalid PASERK format."),
             ("k3.secret-wrap.xxx.AAAAAAAAAAAAAAAA", "Unknown wrapping algorithm: xxx."),
             ("k3.xxx.pie.AAAAAAAAAAAAAAAA", "Invalid PASERK type: xxx."),
         ],
     )
     def test_v3_public_from_paserk_with_wrapping_key_and_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V3Public.from_paserk(paserk, wrapping_key=token_bytes(32))
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     def test_v3_public_from_public_bytes_with_invalid_args(self):
-
         with pytest.raises(ValueError) as err:
             V3Public.from_public_bytes(b"xxx")
             pytest.fail("Key.from_paserk should fail.")
         assert "Invalid bytes for the key." in str(err.value)
 
     def test_v3_public_sign_via_encode_with_invalid_key(self):
-
         k = Key.from_paserk(
             "k3.secret-pw.mXsR2qVqmcDxmSWeQCnCwNeIxe5RDQ3ehnQvdXFj-YgAAAPoFI8eRXCL8PFpVW_CWOvGHnvMPy0BkMlKF1AtmBYGKold9i-ALC2oflkemYdbncrHbiKGd8zfjTQu2tTo2ayOMHybk_-hhopwJ2IUallYfLfUzPuqvtOQfVxXLtUBPnmR75dhRiPDgzdIO1OMbqa3Z1LDevvzbrcPyhHqmJSZioeJ7j1Mu8DJOvrIK0pWHmjDq_eg4YFnaOgz7I3Tkxx89A",
             password="correct horse battery staple".encode("utf-8").hex(),
         )
         with pytest.raises(SignError) as err:
             pyseto.encode(k, b"Hello world!")
             pytest.fail("pyseto.sign() should fail.")
```

### Comparing `pyseto-1.7.1/tests/test_v4.py` & `pyseto-1.7.2/tests/test_v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
             ("k4.local.xxx.AAAAAAAAAAAAAAAA", "Invalid PASERK format."),
             ("k4.public.xxx.AAAAAAAAAAAAAAAA", "Invalid PASERK format."),
             ("k4.xxx.AAAAAAAAAAAAAAAA", "Invalid PASERK type: xxx."),
             ("k4.public.AAAAAAAAAAAAAAAA", "Invalid PASERK type: public."),
         ],
     )
     def test_v4_local_from_paserk_with_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V4Local.from_paserk(paserk)
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
 
     def test_v4_local_to_peer_paserk_id(self):
         k = Key.new(4, "local", b"our-secret")
@@ -111,12 +110,11 @@
             ("k4.public.xxx.AAAAAAAAAAAAAAAA", "Invalid PASERK format."),
             ("k4.local.xxx.AAAAAAAAAAAAAAAA", "Invalid PASERK format."),
             ("k4.xxx.AAAAAAAAAAAAAAAA", "Invalid PASERK type: xxx."),
             ("k4.local.AAAAAAAAAAAAAAAA", "Invalid PASERK type: local."),
         ],
     )
     def test_v4_public_from_paserk_with_invalid_args(self, paserk, msg):
-
         with pytest.raises(ValueError) as err:
             V4Public.from_paserk(paserk)
             pytest.fail("Key.from_paserk should fail.")
         assert msg in str(err.value)
```

### Comparing `pyseto-1.7.1/tests/test_with_test_vectors.py` & `pyseto-1.7.2/tests/test_with_test_vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,42 +15,38 @@
 from pyseto import Key
 from pyseto.versions.v3 import V3Public
 
 from .utils import get_path
 
 
 def _load_tests(paths: list) -> list:
-
     tests: list = []
     for path in paths:
         with open(get_path(path)) as tv_file:
             tv = json.loads(tv_file.read())
         tests += tv["tests"]
     return tests
 
 
 def _name_to_version(name: str) -> int:
-
     v = name.split(".")[0]
     if len(v) != 2:
         raise ValueError("Invalid PASERK test name.")
     return int(v[1:])
 
 
 def _public_key_compress(x: int, y: int) -> bytes:
-
     bx = x.to_bytes(48, byteorder="big")
     by = y.to_bytes((y.bit_length() + 7) // 8, byteorder="big")
     s = bytearray(1)
     s[0] = 0x02 + (by[len(by) - 1] & 1)
     return bytes(s) + bx
 
 
 def _from_Ed25519PrivateKey_to_X25519PrivateKey(data: bytes) -> X25519PrivateKey:
-
     hasher = hashes.Hash(hashes.SHA512())
     hasher.update(data)
     h = bytearray(hasher.finalize())
 
     # curve25519 clamping
     h[0] &= 248
     h[31] &= 127
@@ -71,15 +67,14 @@
                 "vectors/v2.json",
                 "vectors/v3.json",
                 "vectors/v4.json",
             ]
         ),
     )
     def test_with_test_vectors(self, v):
-
         token = v["token"].encode("utf-8")
         payload = v["payload"]
         footer = v["footer"].encode("utf-8")
         implicit_assertion = v["implicit-assertion"].encode("utf-8")
 
         version = int(v["name"].split("-")[0])
         purpose = v["name"].split("-")[1]
@@ -156,15 +151,14 @@
                 "vectors/PASERK/k2.public.json",
                 "vectors/PASERK/k3.public.json",
                 "vectors/PASERK/k4.public.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_public(self, v):
-
         version = _name_to_version(v["name"])
         if version == 1:
             k = Key.new(version, "public", v["key"])
         elif version == 2 or version == 4:
             k = Key.from_asymmetric_key_params(version, x=bytes.fromhex(v["key"]))
         elif version == 3:
             k = V3Public.from_public_bytes(bytes.fromhex(v["key"]))
@@ -182,15 +176,14 @@
                 "vectors/PASERK/k2.secret.json",
                 "vectors/PASERK/k3.secret.json",
                 "vectors/PASERK/k4.secret.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_secret(self, v):
-
         version = _name_to_version(v["name"])
         if version == 1:
             k = Key.new(version, "public", v["key"])
         elif version == 2 or version == 4:
             k = Key.from_asymmetric_key_params(version, d=bytes.fromhex(v["secret-key-seed"]))
         elif version == 3:
             pub_k = Key.new(version, "public", bytes.fromhex(v["public-key"]))
@@ -211,15 +204,14 @@
                 "vectors/PASERK/k2.local.json",
                 "vectors/PASERK/k3.local.json",
                 "vectors/PASERK/k4.local.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_local(self, v):
-
         version = _name_to_version(v["name"])
         k = Key.new(version, "local", bytes.fromhex(v["key"]))
         k2 = Key.from_paserk(v["paserk"])
         assert k.to_paserk() == v["paserk"]
         assert k2.to_paserk() == v["paserk"]
 
     @pytest.mark.parametrize(
@@ -230,15 +222,14 @@
                 "vectors/PASERK/k2.pid.json",
                 "vectors/PASERK/k3.pid.json",
                 "vectors/PASERK/k4.pid.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_pid(self, v):
-
         version = _name_to_version(v["name"])
         if version == 1:
             k = Key.new(version, "public", v["key"])
         elif version == 2 or version == 4:
             k = Key.from_asymmetric_key_params(version, x=bytes.fromhex(v["key"]))
         elif version == 3:
             k = V3Public.from_public_bytes(bytes.fromhex(v["key"]))
@@ -254,15 +245,14 @@
                 "vectors/PASERK/k2.sid.json",
                 "vectors/PASERK/k3.sid.json",
                 "vectors/PASERK/k4.sid.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_sid(self, v):
-
         version = _name_to_version(v["name"])
         if version == 1:
             k = Key.new(version, "public", v["key"])
         elif version == 2 or version == 4:
             k = Key.from_asymmetric_key_params(version, d=bytes.fromhex(v["seed"]))
         elif version == 3:
             pub_k = Key.new(version, "public", bytes.fromhex(v["public-key"]))
@@ -281,15 +271,14 @@
                 "vectors/PASERK/k2.lid.json",
                 "vectors/PASERK/k3.lid.json",
                 "vectors/PASERK/k4.lid.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_lid(self, v):
-
         version = _name_to_version(v["name"])
         k = Key.new(version, "local", bytes.fromhex(v["key"]))
         assert k.to_paserk_id() == v["paserk"]
 
     @pytest.mark.parametrize(
         "v",
         _load_tests(
@@ -298,15 +287,14 @@
                 "vectors/PASERK/k2.local-wrap.pie.json",
                 "vectors/PASERK/k3.local-wrap.pie.json",
                 "vectors/PASERK/k4.local-wrap.pie.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_local_wrap_pie(self, v):
-
         version = _name_to_version(v["name"])
         k = Key.from_paserk(v["paserk"], wrapping_key=bytes.fromhex(v["wrapping-key"]))
 
         k1 = Key.new(version, "local", bytes.fromhex(v["unwrapped"]))
         wpk = k1.to_paserk(wrapping_key=bytes.fromhex(v["wrapping-key"]))
         k2 = Key.from_paserk(wpk, wrapping_key=bytes.fromhex(v["wrapping-key"]))
 
@@ -332,15 +320,14 @@
                 "vectors/PASERK/k2.secret-wrap.pie.json",
                 "vectors/PASERK/k3.secret-wrap.pie.json",
                 "vectors/PASERK/k4.secret-wrap.pie.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_secret_wrap_pie(self, v):
-
         version = _name_to_version(v["name"])
 
         k = Key.from_paserk(v["paserk"], wrapping_key=bytes.fromhex(v["wrapping-key"]))
 
         if version == 1:
             k1 = Key.new(version, "public", v["unwrapped"])
         elif version == 2 or version == 4:
@@ -378,15 +365,14 @@
                 "vectors/PASERK/k2.local-pw.json",
                 "vectors/PASERK/k3.local-pw.json",
                 "vectors/PASERK/k4.local-pw.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_local_pw(self, v):
-
         version = _name_to_version(v["name"])
 
         k = Key.from_paserk(v["paserk"], password=v["password"])
 
         k1 = Key.new(version, "local", bytes.fromhex(v["unwrapped"]))
         if version in [1, 3]:
             wpk = k1.to_paserk(password=v["password"], iteration=v["options"]["iterations"])
@@ -425,15 +411,14 @@
                 "vectors/PASERK/k2.secret-pw.json",
                 "vectors/PASERK/k3.secret-pw.json",
                 "vectors/PASERK/k4.secret-pw.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_secret_pw(self, v):
-
         version = _name_to_version(v["name"])
 
         k = Key.from_paserk(v["paserk"], password=v["password"])
 
         if version == 1:
             k1 = Key.new(version, "public", v["unwrapped"])
         elif version == 2 or version == 4:
@@ -479,15 +464,14 @@
             [
                 "vectors/PASERK/k2.seal.json",
                 "vectors/PASERK/k4.seal.json",
             ]
         ),
     )
     def test_with_test_vectors_paserk_seal_v2_v4(self, v):
-
         version = _name_to_version(v["name"])
 
         if version == 1:
             raise NotImplementedError("Not implemented.")
         elif version in [2, 4]:
             sk_ed25519 = bytes.fromhex(v["sealing-secret-key"])[0:32]
             tmp_key = _from_Ed25519PrivateKey_to_X25519PrivateKey(sk_ed25519)
```

### Comparing `pyseto-1.7.1/tests/utils.py` & `pyseto-1.7.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.lid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.lid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.local-pw.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.local-pw.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.local-wrap.pie.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.local-wrap.pie.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.local.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.local.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.pid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.pid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.public.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.public.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.seal.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.seal.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.secret-pw.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.secret-pw.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.secret-wrap.pie.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.secret-wrap.pie.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.secret.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.secret.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k1.sid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k1.sid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.lid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.lid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.local-pw.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.local-pw.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.local-wrap.pie.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.local-wrap.pie.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.local.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.local.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.pid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.pid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.public.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.public.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.seal.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.seal.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.secret-pw.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.secret-pw.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.secret-wrap.pie.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.secret-wrap.pie.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.secret.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.secret.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k2.sid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k2.sid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.lid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.lid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.local-pw.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.local-pw.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.local-wrap.pie.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.local-wrap.pie.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.local.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.local.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.public.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.public.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.seal.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.seal.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.secret-pw.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.secret-pw.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.secret-wrap.pie.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.secret-wrap.pie.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.secret.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.secret.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k3.sid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k3.sid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.lid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.lid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.local-pw.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.local-pw.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.local-wrap.pie.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.local-wrap.pie.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.local.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.local.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.pid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.pid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.public.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.public.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.seal.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.seal.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.secret-pw.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.secret-pw.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.secret-wrap.pie.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.secret-wrap.pie.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.secret.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.secret.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/PASERK/k4.sid.json` & `pyseto-1.7.2/tests/vectors/PASERK/k4.sid.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/v1.json` & `pyseto-1.7.2/tests/vectors/v1.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/v2.json` & `pyseto-1.7.2/tests/vectors/v2.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/v3.json` & `pyseto-1.7.2/tests/vectors/v3.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tests/vectors/v4.json` & `pyseto-1.7.2/tests/vectors/v4.json`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/tox.ini` & `pyseto-1.7.2/tox.ini`

 * *Files identical despite different names*

### Comparing `pyseto-1.7.1/setup.py` & `pyseto-1.7.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,418 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyseto
+Version: 1.7.2
+Summary: A Python implementation of PASETO/PASERK.
+Home-page: https://github.com/dajiaji/pyseto
+License: MIT
+Author: Ajitomi Daisuke
+Author-email: dajiaji@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: docs
+Requires-Dist: Sphinx[docs] (>=4.3.2,<6.0.0) ; extra == "docs"
+Requires-Dist: cryptography (>=36,<41)
+Requires-Dist: iso8601 (>=1.0.2,<2.0.0)
+Requires-Dist: passlib[argon2] (>=1.7.4,<2.0.0)
+Requires-Dist: pycryptodomex (>=3.12.0,<4.0.0)
+Requires-Dist: sphinx-autodoc-typehints[docs] (==1.21.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0) ; extra == "docs"
+Project-URL: Repository, https://github.com/dajiaji/pyseto
+Description-Content-Type: text/markdown
 
-packages = \
-['pyseto', 'pyseto.versions']
+# PySETO - A Python implementation of PASETO/PASERK
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/pyseto.svg)](https://badge.fury.io/py/pyseto)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyseto)
+[![Documentation Status](https://readthedocs.org/projects/pyseto/badge/?version=latest)](https://pyseto.readthedocs.io/en/latest/?badge=latest)
+![Github CI](https://github.com/dajiaji/pyseto/actions/workflows/python-package.yml/badge.svg)
+[![codecov](https://codecov.io/gh/dajiaji/pyseto/branch/main/graph/badge.svg?token=QN8GXEYEP3)](https://codecov.io/gh/dajiaji/pyseto)
 
-install_requires = \
-['cryptography>=36,<40',
- 'iso8601>=1.0.2,<2.0.0',
- 'passlib[argon2]>=1.7.4,<2.0.0',
- 'pycryptodomex>=3.12.0,<4.0.0']
-
-extras_require = \
-{'docs': ['Sphinx[docs]>=4.3.2,<6.0.0',
-          'sphinx-autodoc-typehints[docs]==1.21.0',
-          'sphinx-rtd-theme[docs]>=1.0.0,<2.0.0']}
-
-setup_kwargs = {
-    'name': 'pyseto',
-    'version': '1.7.1',
-    'description': 'A Python implementation of PASETO/PASERK.',
-    'long_description': '# PySETO - A Python implementation of PASETO/PASERK\n\n[![PyPI version](https://badge.fury.io/py/pyseto.svg)](https://badge.fury.io/py/pyseto)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyseto)\n[![Documentation Status](https://readthedocs.org/projects/pyseto/badge/?version=latest)](https://pyseto.readthedocs.io/en/latest/?badge=latest)\n![Github CI](https://github.com/dajiaji/pyseto/actions/workflows/python-package.yml/badge.svg)\n[![codecov](https://codecov.io/gh/dajiaji/pyseto/branch/main/graph/badge.svg?token=QN8GXEYEP3)](https://codecov.io/gh/dajiaji/pyseto)\n\n\nPySETO is a [PASETO (Platform-Agnostic SEcurity TOkens)](https://paseto.io/)/[PASERK (Platform-Agnostic Serialized Keys)](https://github.com/paseto-standard/paserk) implementation written in Python\nwhich supports all of the versions ([v1](https://github.com/paseto-standard/paseto-spec/blob/master/docs/01-Protocol-Versions/Version1.md),\n[v2](https://github.com/paseto-standard/paseto-spec/blob/master/docs/01-Protocol-Versions/Version2.md),\n[v3](https://github.com/paseto-standard/paseto-spec/blob/master/docs/01-Protocol-Versions/Version3.md) and\n[v4](https://github.com/paseto-standard/paseto-spec/blob/master/docs/01-Protocol-Versions/Version4.md)) and purposes (`public` and `local`)\nand has passed all of [the official tests](https://github.com/paseto-standard/test-vectors).\n\nYou can install PySETO with pip:\n\n```sh\n$ pip install pyseto\n```\n\nPySETO can be used in ease as follows (in case of `v4.public`):\n\n```py\nimport pyseto\nfrom pyseto import Key\n\nprivate_key_pem = b"-----BEGIN PRIVATE KEY-----\\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\\n-----END PRIVATE KEY-----"\npublic_key_pem = b"-----BEGIN PUBLIC KEY-----\\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\\n-----END PUBLIC KEY-----"\n\n\n# Create a PASETO token.\nprivate_key = Key.new(version=4, purpose="public", key=private_key_pem)\ntoken = pyseto.encode(private_key, b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\')\n\n# Decode and verify a PASETO token.\npublic_key = Key.new(version=4, purpose="public", key=public_key_pem)\ndecoded = pyseto.decode(public_key, token)\n\nassert token == b\'v4.public.eyJkYXRhIjogInRoaXMgaXMgYSBzaWduZWQgbWVzc2FnZSIsICJleHAiOiAiMjAyMi0wMS0wMVQwMDowMDowMCswMDowMCJ9l1YiKei2FESvHBSGPkn70eFO1hv3tXH0jph1IfZyEfgm3t1DjkYqD5r4aHWZm1eZs_3_bZ9pBQlZGp0DPSdzDg\'\nassert decoded.payload == b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\'\n```\n\nSee following contents or [Documentation](https://pyseto.readthedocs.io/en/stable/) for details.\n\n## Index\n\n- [Installation](#installation)\n- [Supported PASETO Versions](#supported-paseto-versions)\n- [Supported PASERK Types](#supported-paserk-types)\n- [PASETO Usage](#paseto-usage)\n    - [Basic usage: v4.public](#basic-usage-v4public)\n    - [Basic usage: v4.local](#basic-usage-v4local)\n    - [Using serializer/deserializer for payload and footer](#using-serializerdeserializer-for-payload-and-footer)\n    - [Using Paseto class for handling registered claims](#using-paseto-class-for-handling-registered-claims)\n- [PASERK Usage](#paserk-usage)\n    - [Serializing/Deserializing PASERK](#serializingdeserializing-paserk)\n    - [Serializing PASERK ID](#serializing-paserk-id)\n    - [Key Wrapping](#key-wrapping)\n    - [Password-based Key Encryption](#password-based-key-encryption)\n    - [Asymmetric Encryption](#asymmetric-encryption)\n- [API Reference](#api-reference)\n- [Tests](#tests)\n- [Contributing](#contributing)\n\n## Installation\n\nYou can install PySETO with pip:\n\n```sh\n$ pip install pyseto\n```\n\n## Supported PASETO Versions\n\nPySETO supports all of PASETO versions and purposes below:\n\n\n|          |  v4  |  v3  |  v2  |  v1  |\n| ---------| ---- | ---- | ---- | ---- |\n| `local`  |  ✅  |  ✅  |  ✅  |  ✅  |\n| `public` |  ✅  |  ✅  |  ✅  |  ✅  |\n\n\n## Supported PASERK Types\n\nPySETO also supports [PASERK (Platform-Agnostic Serialized Keys)](https://github.com/paseto-standard/paserk).\nCurrently, following PASERK types are supported:\n\n\n|               |  v4  |  v3  |  v2  |  v1  |\n| ------------- | ---- | ---- | ---- | ---- |\n| `lid`         |  ✅  |  ✅  |  ✅  |  ✅  |\n| `sid`         |  ✅  |  ✅  |  ✅  |  ✅  |\n| `pid`         |  ✅  |  ✅  |  ✅  |  ✅  |\n| `local`       |  ✅  |  ✅  |  ✅  |  ✅  |\n| `secret`      |  ✅  |  ✅  |  ✅  |  ✅  |\n| `public`      |  ✅  |  ✅  |  ✅  |  ✅  |\n| `seal`        |  ✅  |      |  ✅  |      |\n| `local-wrap`  |  ✅  |  ✅  |  ✅  |  ✅  |\n| `secret-wrap` |  ✅  |  ✅  |  ✅  |  ✅  |\n| `local-pw`    |  ✅  |  ✅  |  ✅  |  ✅  |\n| `secret-pw`   |  ✅  |  ✅  |  ✅  |  ✅  |\n\n\n## PASETO Usage\n\nBy using this PySETO, you can easily create, decode and verify PASETO tokens. Here are sample codes that handle version 4 PySETO tokens.\n\nPlease refer to [the Documentation](https://pyseto.readthedocs.io/en/stable/) for all usage examples including other versions.\n\n### Basic usage: v4.public\n\n`v4.public` is one of current PASETO versions to be used for asymmetric authentication (public key signatures).\n\n```py\nimport pyseto\nfrom pyseto import Key\n\nprivate_key_pem = b"-----BEGIN PRIVATE KEY-----\\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\\n-----END PRIVATE KEY-----"\npublic_key_pem = b"-----BEGIN PUBLIC KEY-----\\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\\n-----END PUBLIC KEY-----"\n\nprivate_key = Key.new(version=4, purpose="public", key=private_key_pem)\ntoken = pyseto.encode(private_key, b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\')\n\npublic_key = Key.new(version=4, purpose="public", key=public_key_pem)\ndecoded = pyseto.decode(public_key, token)\n\nassert token == b\'v4.public.eyJkYXRhIjogInRoaXMgaXMgYSBzaWduZWQgbWVzc2FnZSIsICJleHAiOiAiMjAyMi0wMS0wMVQwMDowMDowMCswMDowMCJ9l1YiKei2FESvHBSGPkn70eFO1hv3tXH0jph1IfZyEfgm3t1DjkYqD5r4aHWZm1eZs_3_bZ9pBQlZGp0DPSdzDg\'\nassert decoded.payload == b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\'\n```\n\n### Basic usage: v4.local\n\n`v4.local` is one of current PASETO versions to be used for symmetric authenticated encryption.\n\n```py\nimport pyseto\nfrom pyseto import Key\n\nkey = Key.new(version=4, purpose="local", key=b"our-secret")\ntoken = pyseto.encode(key, b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\')\n\ndecoded = pyseto.decode(key, token)\n\nassert decoded.payload == b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\'\n```\n\n### Using serializer/deserializer for payload and footer\n\nBy using `serializer` and `deserializer`, you can encode/decode a dict-typed payload and footer included in PASETO tokens into an arbitrary format.\nThe following example shows that the payload and the footer in a PASETO token are encoded/decoded as JSON formatted data.\nWhen specifing dict-typed payload, exp parameter can be used to set the expiration time (seconds) of the token.\n\n```py\nimport json\nimport pyseto\nfrom pyseto import Key\n\nprivate_key_pem = b"-----BEGIN PRIVATE KEY-----\\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\\n-----END PRIVATE KEY-----"\npublic_key_pem = b"-----BEGIN PUBLIC KEY-----\\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\\n-----END PUBLIC KEY-----"\n\nprivate_key = Key.new(version=4, purpose="public", key=private_key_pem)\npublic_key = Key.new(version=4, purpose="public", key=public_key_pem)\ntoken = pyseto.encode(\n    private_key,\n    {"data": "this is a signed message"},\n    footer={"kid": public_key.to_paserk_id()},\n    serializer=json,\n    exp=3600,\n)\n\ndecoded = pyseto.decode(public_key, token, deserializer=json)\n\nassert decoded.payload["data"] == "this is a signed message"\nassert decoded.payload["exp"] == "2021-11-11T00:00:00+00:00"\nassert decoded.footer["kid"] == "k4.pid.yh4-bJYjOYAG6CWy0zsfPmpKylxS7uAWrxqVmBN2KAiJ"\n```\n\n### Using `Paseto` class for handling registered claims\n\nBy using `Paseto` class, you can change the default value of `exp` (the expiration date ot tokens), whether to include an `iat` claim, and other settings.\n\nNote that `pyseto.encode()` and `pyseto.decode()` are aliases to the `encode()` and `decode()` of the global "Paseto" class instance created with the default settings.\n\n```py\nimport json\nimport pyseto\nfrom pyseto import Key, Paseto\n\nprivate_key_pem = b"-----BEGIN PRIVATE KEY-----\\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\\n-----END PRIVATE KEY-----"\npublic_key_pem = b"-----BEGIN PUBLIC KEY-----\\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\\n-----END PUBLIC KEY-----"\n\nprivate_key = Key.new(version=4, purpose="public", key=private_key_pem)\npaseto = Paseto.new(exp=3600, include_iat=True) # Default values are exp=0(not specified) and including_iat=False\ntoken = paseto.encode(\n    private_key,\n    {"data": "this is a signed message"},\n    serializer=json,\n)\n\npublic_key = Key.new(version=4, purpose="public", key=public_key_pem)\ndecoded = pyseto.decode(public_key, token, deserializer=json)\n\nassert decoded.payload["data"] == "this is a signed message"\nassert decoded.payload["iat"] == "2021-11-11T00:00:00+00:00"\nassert decoded.payload["exp"] == "2021-11-11T01:00:00+00:00"\n```\n\n## PASERK Usage\n\n[PASERK (Platform-Agnostic Serialized Keys)](https://github.com/paseto-standard/paserk) is an extension to PASETO that provides key-wrapping and serialization.\n\n### Serializing/Deserializing PASERK\n\nAs shown in the examples above, the `pyseto.Key` used for encryption and signature can be generated from PASERK or converted to PASERK as follows:\n\n```py\nimport pyseto\nfrom pyseto import Key\n\n# pyseto.Key can be generated from PASERK.\nsymmetric_key = Key.new(version=4, purpose="local", key=b"our-secret")\nprivate_key = Key.from_paserk("k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog")\npublic_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")\n\ntoken = pyseto.encode(private_key, b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\')\ndecoded = pyseto.decode(public_key, token)\n\nassert decoded.payload == b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\'\n\n# PASERK can be derived from pyseto.Key.\nassert symmetric_key.to_paserk() == "k4.local.b3VyLXNlY3JldA"\nassert private_key.to_paserk() == "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"\nassert public_key.to_paserk() == "k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI"\n```\n\n### Serializing PASERK ID\n\n`pyseto.Key` can also be converted to PASERK ID as follows:\n\n```py\nimport pyseto\nfrom pyseto import Key\n\n# pyseto.Key can be generated from PASERK.\nsymmetric_key = Key.new(version=4, purpose="local", key=b"our-secret")\nprivate_key = Key.from_paserk("k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog")\npublic_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")\n\n# PASERK ID can be derived from pyseto.Key.\nassert symmetric_key.to_paserk_id() == "k4.lid._D6kgTzxgiPGk35gMj9bukgj4En2H94u22wVX9zaoh05"\nassert private_key.to_paserk() == "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"\nassert public_key.to_paserk_id() == "k4.pid.yh4-bJYjOYAG6CWy0zsfPmpKylxS7uAWrxqVmBN2KAiJ"\n```\n\n### Key Wrapping\n\nIf you call `to_paserk` with `wrapping_key`, you can get a wrapped (encrypted) PASERK with the wrapping key.\nThe wrapped PASERK can be decrypted by calling `from_paserk` with `wrapping key`.\n\nIn case of `local-wrap.pie`:\n\n```py\nimport pyseto\nfrom pyseto import Key\n\nraw_key = Key.new(version=4, purpose="local", key=b"our-secret")\nwrapping_key = token_bytes(32)\nwpk = raw_key.to_paserk(wrapping_key=wrapping_key)\ntoken = pyseto.encode(raw_key, b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\')\n\nunwrapped_key = Key.from_paserk(wpk, wrapping_key=wrapping_key)\ndecoded = pyseto.decode(unwrapped_key, token)\n\n# assert wpk == "k4.local-wrap.pie.TNKEwC4K1xBcgJ_GiwWAoRlQFE33HJO3oN9DHEZ05pieSCd-W7bgAL64VG9TZ_pBkuNBFHNrfOGHtnfnhYGdbz5-x3CxShhPJxg"\nassert decoded.payload == b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\'\n```\n\nIn case of `secret-wrap.pie`:\n\n```py\nimport pyseto\nfrom pyseto import Key\n\nraw_private_key = Key.from_paserk(\n    "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"\n)\nwrapping_key = token_bytes(32)\nwpk = raw_private_key.to_paserk(wrapping_key=wrapping_key)\nunwrapped_private_key = Key.from_paserk(wpk, wrapping_key=wrapping_key)\ntoken = pyseto.encode(unwrapped_private_key, b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\')\n\npublic_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")\ndecoded = pyseto.decode(public_key, token)\n\n# assert wpk == "k4.secret-wrap.pie.excv7V4-NaECy5hpji-tkSkMvyjsAgNxA-mGALgdjyvGNyDlTb89bJ35R1e3tILgbMpEW5WXMXzySe2T-sBz-ZAcs1j7rbD3ZWvsBTM6K5N9wWfAxbR4ppCXH_H5__9yY-kBaF2NimyAJyduhOhSmqLm6TTSucpAOakEJOXePW8"\nassert decoded.payload == b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\'\n```\n\n### Password-based Key Encryption\n\nIf you call `to_paserk` with `password`, you can get a wrapped (encrypted) PASERK with the password.\nThe wrapped PASERK can be decrypted by calling `from_paserk` with `passwrod`.\n\nIn case of `local-pw`:\n\n```py\nimport pyseto\nfrom pyseto import Key\n\nraw_key = Key.new(version=4, purpose="local", key=b"our-secret")\ntoken = pyseto.encode(raw_key, b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\')\n\nwpk = raw_key.to_paserk(password="our-secret")\nunwrapped_key = Key.from_paserk(wpk, password="our-secret")\ndecoded = pyseto.decode(unwrapped_key, token)\n\n# assert wpk == "k4.local-pw.HrCs9Pu-2LB0l7jkHB-x2gAAAAAA8AAAAAAAAgAAAAGttW0IHZjQCHJdg-Vc3tqO_GSLR4vzLl-yrKk2I-l8YHj6jWpC0lQB2Z7uzTtVyV1rd_EZQPzHdw5VOtyucP0FkCU"\nassert decoded.payload == b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\'\n```\n\nIn case of `secret-pw`:\n\n```py\nimport pyseto\nfrom pyseto import Key\n\nraw_private_key = Key.from_paserk(\n    "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"\n)\nwpk = raw_private_key.to_paserk(password="our-secret")\nunwrapped_private_key = Key.from_paserk(wpk, password="our-secret")\ntoken = pyseto.encode(unwrapped_private_key, b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\')\n\npublic_key = Key.from_paserk(\n    "k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI"\n)\ndecoded = pyseto.decode(public_key, token)\n\n# assert wpk == "k4.secret-pw.MEMW4K1MaD5nWigCLyEyFAAAAAAA8AAAAAAAAgAAAAFU-tArtryNVjS2n2hCYiM11V6tOyuIog69Bjb0yNZanrLJ3afGclb3kPzQ6IhK8ob9E4QgRdEALGWCizZ0RCPFF_M95IQDfmdYKC0Er656UgKUK4UKG9JlxP4o81UwoJoZYz_D1zTlltipEa5RiNvUtNU8vLKoGSY"\nassert decoded.payload == b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\'\n```\n\n### Asymmetric Encryption\n\nAt this time, PySETO supports asymmetric encryption (key sealing) for `v2` and `v4`.\n\n```py\nimport pyseto\nfrom pyseto import Key\n\nprivate_key_pem = b"-----BEGIN PRIVATE KEY-----\\nMC4CAQAwBQYDK2VuBCIEIFAF7jSCZHFgWvC8hUkXr55Az6Pot2g4zOAUxck0/6x8\\n-----END PRIVATE KEY-----"\npublic_key_pem = b"-----BEGIN PUBLIC KEY-----\\nMCowBQYDK2VuAyEAFv8IXsICYj0paznDK/99GyCsFOIGnfY87ayyNSIvSB4=\\n-----END PUBLIC KEY-----"\n\nraw_key = Key.new(version=4, purpose="local", key=b"our-secret")\ntoken = pyseto.encode(\n    raw_key,\n    b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\',\n)\n\nsealed_key = raw_key.to_paserk(sealing_key=public_key_pem)\nunsealed_key = Key.from_paserk(sealed_key, unsealing_key=private_key_pem)\ndecoded = pyseto.decode(unsealed_key, token)\n\nassert (\n    decoded.payload\n    == b\'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}\'\n)\n```\n\nKey searing for `v1` and `v3` have not been supported yet.\n\n\n## API Reference\n\nSee [Documentation](https://pyseto.readthedocs.io/en/stable/api.html).\n\n## Tests\n\nYou can run tests from the project root after cloning with:\n\n```sh\n$ tox\n```\n\n## Contributing\n\nWe welcome all kind of contributions, filing issues, suggesting new features or sending PRs.\n',
-    'author': 'Ajitomi Daisuke',
-    'author_email': 'dajiaji@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dajiaji/pyseto',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
 
+PySETO is a [PASETO (Platform-Agnostic SEcurity TOkens)](https://paseto.io/)/[PASERK (Platform-Agnostic Serialized Keys)](https://github.com/paseto-standard/paserk) implementation written in Python
+which supports all of the versions ([v1](https://github.com/paseto-standard/paseto-spec/blob/master/docs/01-Protocol-Versions/Version1.md),
+[v2](https://github.com/paseto-standard/paseto-spec/blob/master/docs/01-Protocol-Versions/Version2.md),
+[v3](https://github.com/paseto-standard/paseto-spec/blob/master/docs/01-Protocol-Versions/Version3.md) and
+[v4](https://github.com/paseto-standard/paseto-spec/blob/master/docs/01-Protocol-Versions/Version4.md)) and purposes (`public` and `local`)
+and has passed all of [the official tests](https://github.com/paseto-standard/test-vectors).
+
+You can install PySETO with pip:
+
+```sh
+$ pip install pyseto
+```
+
+PySETO can be used in ease as follows (in case of `v4.public`):
+
+```py
+import pyseto
+from pyseto import Key
+
+private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
+public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
+
+
+# Create a PASETO token.
+private_key = Key.new(version=4, purpose="public", key=private_key_pem)
+token = pyseto.encode(private_key, b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}')
+
+# Decode and verify a PASETO token.
+public_key = Key.new(version=4, purpose="public", key=public_key_pem)
+decoded = pyseto.decode(public_key, token)
+
+assert token == b'v4.public.eyJkYXRhIjogInRoaXMgaXMgYSBzaWduZWQgbWVzc2FnZSIsICJleHAiOiAiMjAyMi0wMS0wMVQwMDowMDowMCswMDowMCJ9l1YiKei2FESvHBSGPkn70eFO1hv3tXH0jph1IfZyEfgm3t1DjkYqD5r4aHWZm1eZs_3_bZ9pBQlZGp0DPSdzDg'
+assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
+```
+
+See following contents or [Documentation](https://pyseto.readthedocs.io/en/stable/) for details.
+
+## Index
+
+- [Installation](#installation)
+- [Supported PASETO Versions](#supported-paseto-versions)
+- [Supported PASERK Types](#supported-paserk-types)
+- [PASETO Usage](#paseto-usage)
+    - [Basic usage: v4.public](#basic-usage-v4public)
+    - [Basic usage: v4.local](#basic-usage-v4local)
+    - [Using serializer/deserializer for payload and footer](#using-serializerdeserializer-for-payload-and-footer)
+    - [Using Paseto class for handling registered claims](#using-paseto-class-for-handling-registered-claims)
+- [PASERK Usage](#paserk-usage)
+    - [Serializing/Deserializing PASERK](#serializingdeserializing-paserk)
+    - [Serializing PASERK ID](#serializing-paserk-id)
+    - [Key Wrapping](#key-wrapping)
+    - [Password-based Key Encryption](#password-based-key-encryption)
+    - [Asymmetric Encryption](#asymmetric-encryption)
+- [API Reference](#api-reference)
+- [Tests](#tests)
+- [Contributing](#contributing)
+
+## Installation
+
+You can install PySETO with pip:
+
+```sh
+$ pip install pyseto
+```
+
+## Supported PASETO Versions
+
+PySETO supports all of PASETO versions and purposes below:
+
+
+|          |  v4  |  v3  |  v2  |  v1  |
+| ---------| ---- | ---- | ---- | ---- |
+| `local`  |  ✅  |  ✅  |  ✅  |  ✅  |
+| `public` |  ✅  |  ✅  |  ✅  |  ✅  |
+
+
+## Supported PASERK Types
+
+PySETO also supports [PASERK (Platform-Agnostic Serialized Keys)](https://github.com/paseto-standard/paserk).
+Currently, following PASERK types are supported:
+
+
+|               |  v4  |  v3  |  v2  |  v1  |
+| ------------- | ---- | ---- | ---- | ---- |
+| `lid`         |  ✅  |  ✅  |  ✅  |  ✅  |
+| `sid`         |  ✅  |  ✅  |  ✅  |  ✅  |
+| `pid`         |  ✅  |  ✅  |  ✅  |  ✅  |
+| `local`       |  ✅  |  ✅  |  ✅  |  ✅  |
+| `secret`      |  ✅  |  ✅  |  ✅  |  ✅  |
+| `public`      |  ✅  |  ✅  |  ✅  |  ✅  |
+| `seal`        |  ✅  |      |  ✅  |      |
+| `local-wrap`  |  ✅  |  ✅  |  ✅  |  ✅  |
+| `secret-wrap` |  ✅  |  ✅  |  ✅  |  ✅  |
+| `local-pw`    |  ✅  |  ✅  |  ✅  |  ✅  |
+| `secret-pw`   |  ✅  |  ✅  |  ✅  |  ✅  |
+
+
+## PASETO Usage
+
+By using this PySETO, you can easily create, decode and verify PASETO tokens. Here are sample codes that handle version 4 PySETO tokens.
+
+Please refer to [the Documentation](https://pyseto.readthedocs.io/en/stable/) for all usage examples including other versions.
+
+### Basic usage: v4.public
+
+`v4.public` is one of current PASETO versions to be used for asymmetric authentication (public key signatures).
+
+```py
+import pyseto
+from pyseto import Key
+
+private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
+public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
+
+private_key = Key.new(version=4, purpose="public", key=private_key_pem)
+token = pyseto.encode(private_key, b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}')
+
+public_key = Key.new(version=4, purpose="public", key=public_key_pem)
+decoded = pyseto.decode(public_key, token)
+
+assert token == b'v4.public.eyJkYXRhIjogInRoaXMgaXMgYSBzaWduZWQgbWVzc2FnZSIsICJleHAiOiAiMjAyMi0wMS0wMVQwMDowMDowMCswMDowMCJ9l1YiKei2FESvHBSGPkn70eFO1hv3tXH0jph1IfZyEfgm3t1DjkYqD5r4aHWZm1eZs_3_bZ9pBQlZGp0DPSdzDg'
+assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
+```
+
+### Basic usage: v4.local
+
+`v4.local` is one of current PASETO versions to be used for symmetric authenticated encryption.
+
+```py
+import pyseto
+from pyseto import Key
+
+key = Key.new(version=4, purpose="local", key=b"our-secret")
+token = pyseto.encode(key, b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}')
+
+decoded = pyseto.decode(key, token)
+
+assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
+```
+
+### Using serializer/deserializer for payload and footer
+
+By using `serializer` and `deserializer`, you can encode/decode a dict-typed payload and footer included in PASETO tokens into an arbitrary format.
+The following example shows that the payload and the footer in a PASETO token are encoded/decoded as JSON formatted data.
+When specifing dict-typed payload, exp parameter can be used to set the expiration time (seconds) of the token.
+
+```py
+import json
+import pyseto
+from pyseto import Key
+
+private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
+public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
+
+private_key = Key.new(version=4, purpose="public", key=private_key_pem)
+public_key = Key.new(version=4, purpose="public", key=public_key_pem)
+token = pyseto.encode(
+    private_key,
+    {"data": "this is a signed message"},
+    footer={"kid": public_key.to_paserk_id()},
+    serializer=json,
+    exp=3600,
+)
+
+decoded = pyseto.decode(public_key, token, deserializer=json)
+
+assert decoded.payload["data"] == "this is a signed message"
+assert decoded.payload["exp"] == "2021-11-11T00:00:00+00:00"
+assert decoded.footer["kid"] == "k4.pid.yh4-bJYjOYAG6CWy0zsfPmpKylxS7uAWrxqVmBN2KAiJ"
+```
+
+### Using `Paseto` class for handling registered claims
+
+By using `Paseto` class, you can change the default value of `exp` (the expiration date ot tokens), whether to include an `iat` claim, and other settings.
+
+Note that `pyseto.encode()` and `pyseto.decode()` are aliases to the `encode()` and `decode()` of the global "Paseto" class instance created with the default settings.
+
+```py
+import json
+import pyseto
+from pyseto import Key, Paseto
+
+private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VwBCIEILTL+0PfTOIQcn2VPkpxMwf6Gbt9n4UEFDjZ4RuUKjd0\n-----END PRIVATE KEY-----"
+public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VwAyEAHrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI=\n-----END PUBLIC KEY-----"
+
+private_key = Key.new(version=4, purpose="public", key=private_key_pem)
+paseto = Paseto.new(exp=3600, include_iat=True) # Default values are exp=0(not specified) and including_iat=False
+token = paseto.encode(
+    private_key,
+    {"data": "this is a signed message"},
+    serializer=json,
+)
+
+public_key = Key.new(version=4, purpose="public", key=public_key_pem)
+decoded = pyseto.decode(public_key, token, deserializer=json)
+
+assert decoded.payload["data"] == "this is a signed message"
+assert decoded.payload["iat"] == "2021-11-11T00:00:00+00:00"
+assert decoded.payload["exp"] == "2021-11-11T01:00:00+00:00"
+```
+
+## PASERK Usage
+
+[PASERK (Platform-Agnostic Serialized Keys)](https://github.com/paseto-standard/paserk) is an extension to PASETO that provides key-wrapping and serialization.
+
+### Serializing/Deserializing PASERK
+
+As shown in the examples above, the `pyseto.Key` used for encryption and signature can be generated from PASERK or converted to PASERK as follows:
+
+```py
+import pyseto
+from pyseto import Key
+
+# pyseto.Key can be generated from PASERK.
+symmetric_key = Key.new(version=4, purpose="local", key=b"our-secret")
+private_key = Key.from_paserk("k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog")
+public_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")
+
+token = pyseto.encode(private_key, b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}')
+decoded = pyseto.decode(public_key, token)
+
+assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
+
+# PASERK can be derived from pyseto.Key.
+assert symmetric_key.to_paserk() == "k4.local.b3VyLXNlY3JldA"
+assert private_key.to_paserk() == "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"
+assert public_key.to_paserk() == "k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI"
+```
+
+### Serializing PASERK ID
+
+`pyseto.Key` can also be converted to PASERK ID as follows:
+
+```py
+import pyseto
+from pyseto import Key
+
+# pyseto.Key can be generated from PASERK.
+symmetric_key = Key.new(version=4, purpose="local", key=b"our-secret")
+private_key = Key.from_paserk("k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog")
+public_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")
+
+# PASERK ID can be derived from pyseto.Key.
+assert symmetric_key.to_paserk_id() == "k4.lid._D6kgTzxgiPGk35gMj9bukgj4En2H94u22wVX9zaoh05"
+assert private_key.to_paserk() == "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"
+assert public_key.to_paserk_id() == "k4.pid.yh4-bJYjOYAG6CWy0zsfPmpKylxS7uAWrxqVmBN2KAiJ"
+```
+
+### Key Wrapping
+
+If you call `to_paserk` with `wrapping_key`, you can get a wrapped (encrypted) PASERK with the wrapping key.
+The wrapped PASERK can be decrypted by calling `from_paserk` with `wrapping key`.
+
+In case of `local-wrap.pie`:
+
+```py
+import pyseto
+from pyseto import Key
+
+raw_key = Key.new(version=4, purpose="local", key=b"our-secret")
+wrapping_key = token_bytes(32)
+wpk = raw_key.to_paserk(wrapping_key=wrapping_key)
+token = pyseto.encode(raw_key, b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}')
+
+unwrapped_key = Key.from_paserk(wpk, wrapping_key=wrapping_key)
+decoded = pyseto.decode(unwrapped_key, token)
+
+# assert wpk == "k4.local-wrap.pie.TNKEwC4K1xBcgJ_GiwWAoRlQFE33HJO3oN9DHEZ05pieSCd-W7bgAL64VG9TZ_pBkuNBFHNrfOGHtnfnhYGdbz5-x3CxShhPJxg"
+assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
+```
+
+In case of `secret-wrap.pie`:
+
+```py
+import pyseto
+from pyseto import Key
+
+raw_private_key = Key.from_paserk(
+    "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"
+)
+wrapping_key = token_bytes(32)
+wpk = raw_private_key.to_paserk(wrapping_key=wrapping_key)
+unwrapped_private_key = Key.from_paserk(wpk, wrapping_key=wrapping_key)
+token = pyseto.encode(unwrapped_private_key, b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}')
+
+public_key = Key.from_paserk("k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI")
+decoded = pyseto.decode(public_key, token)
+
+# assert wpk == "k4.secret-wrap.pie.excv7V4-NaECy5hpji-tkSkMvyjsAgNxA-mGALgdjyvGNyDlTb89bJ35R1e3tILgbMpEW5WXMXzySe2T-sBz-ZAcs1j7rbD3ZWvsBTM6K5N9wWfAxbR4ppCXH_H5__9yY-kBaF2NimyAJyduhOhSmqLm6TTSucpAOakEJOXePW8"
+assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
+```
+
+### Password-based Key Encryption
+
+If you call `to_paserk` with `password`, you can get a wrapped (encrypted) PASERK with the password.
+The wrapped PASERK can be decrypted by calling `from_paserk` with `passwrod`.
+
+In case of `local-pw`:
+
+```py
+import pyseto
+from pyseto import Key
+
+raw_key = Key.new(version=4, purpose="local", key=b"our-secret")
+token = pyseto.encode(raw_key, b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}')
+
+wpk = raw_key.to_paserk(password="our-secret")
+unwrapped_key = Key.from_paserk(wpk, password="our-secret")
+decoded = pyseto.decode(unwrapped_key, token)
+
+# assert wpk == "k4.local-pw.HrCs9Pu-2LB0l7jkHB-x2gAAAAAA8AAAAAAAAgAAAAGttW0IHZjQCHJdg-Vc3tqO_GSLR4vzLl-yrKk2I-l8YHj6jWpC0lQB2Z7uzTtVyV1rd_EZQPzHdw5VOtyucP0FkCU"
+assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
+```
+
+In case of `secret-pw`:
+
+```py
+import pyseto
+from pyseto import Key
+
+raw_private_key = Key.from_paserk(
+    "k4.secret.tMv7Q99M4hByfZU-SnEzB_oZu32fhQQUONnhG5QqN3Qeudu7vAR8A_1wYE4AcfCYfhayi3VyJcEfAEFdDiCxog"
+)
+wpk = raw_private_key.to_paserk(password="our-secret")
+unwrapped_private_key = Key.from_paserk(wpk, password="our-secret")
+token = pyseto.encode(unwrapped_private_key, b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}')
+
+public_key = Key.from_paserk(
+    "k4.public.Hrnbu7wEfAP9cGBOAHHwmH4Wsot1ciXBHwBBXQ4gsaI"
+)
+decoded = pyseto.decode(public_key, token)
+
+# assert wpk == "k4.secret-pw.MEMW4K1MaD5nWigCLyEyFAAAAAAA8AAAAAAAAgAAAAFU-tArtryNVjS2n2hCYiM11V6tOyuIog69Bjb0yNZanrLJ3afGclb3kPzQ6IhK8ob9E4QgRdEALGWCizZ0RCPFF_M95IQDfmdYKC0Er656UgKUK4UKG9JlxP4o81UwoJoZYz_D1zTlltipEa5RiNvUtNU8vLKoGSY"
+assert decoded.payload == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
+```
+
+### Asymmetric Encryption
+
+At this time, PySETO supports asymmetric encryption (key sealing) for `v2` and `v4`.
+
+```py
+import pyseto
+from pyseto import Key
+
+private_key_pem = b"-----BEGIN PRIVATE KEY-----\nMC4CAQAwBQYDK2VuBCIEIFAF7jSCZHFgWvC8hUkXr55Az6Pot2g4zOAUxck0/6x8\n-----END PRIVATE KEY-----"
+public_key_pem = b"-----BEGIN PUBLIC KEY-----\nMCowBQYDK2VuAyEAFv8IXsICYj0paznDK/99GyCsFOIGnfY87ayyNSIvSB4=\n-----END PUBLIC KEY-----"
+
+raw_key = Key.new(version=4, purpose="local", key=b"our-secret")
+token = pyseto.encode(
+    raw_key,
+    b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}',
+)
+
+sealed_key = raw_key.to_paserk(sealing_key=public_key_pem)
+unsealed_key = Key.from_paserk(sealed_key, unsealing_key=private_key_pem)
+decoded = pyseto.decode(unsealed_key, token)
+
+assert (
+    decoded.payload
+    == b'{"data": "this is a signed message", "exp": "2022-01-01T00:00:00+00:00"}'
+)
+```
+
+Key searing for `v1` and `v3` have not been supported yet.
+
+
+## API Reference
+
+See [Documentation](https://pyseto.readthedocs.io/en/stable/api.html).
+
+## Tests
+
+You can run tests from the project root after cloning with:
+
+```sh
+$ tox
+```
+
+## Contributing
+
+We welcome all kind of contributions, filing issues, suggesting new features or sending PRs.
 
-setup(**setup_kwargs)
```

