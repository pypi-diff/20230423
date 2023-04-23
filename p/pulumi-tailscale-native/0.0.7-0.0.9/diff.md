# Comparing `tmp/pulumi_tailscale_native-0.0.7.tar.gz` & `tmp/pulumi_tailscale_native-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_tailscale_native-0.0.7.tar", last modified: Mon Apr  3 04:56:34 2023, max compression
+gzip compressed data, was "pulumi_tailscale_native-0.0.9.tar", last modified: Mon Apr 17 00:25:24 2023, max compression
```

## Comparing `pulumi_tailscale_native-0.0.7.tar` & `pulumi_tailscale_native-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:56:34.038681 pulumi_tailscale_native-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-03 04:56:34.038681 pulumi_tailscale_native-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:56:34.034681 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:56:34.034681 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/config/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:56:34.034681 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/authorize_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/get_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/get_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/key_expiry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:56:34.038681 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/dns_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/get_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/get_dns_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/get_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/get_name_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/list_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/list_search_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/name_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/replace_search_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:56:34.034681 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-03 04:56:34.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-03 04:56:34.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 04:56:34.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 04:56:34.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-03 04:56:34.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-03 04:56:34.000000 pulumi_tailscale_native-0.0.7/pulumi_tailscale_native.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 04:56:34.038681 pulumi_tailscale_native-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-03 04:56:33.000000 pulumi_tailscale_native-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:25:24.087089 pulumi_tailscale_native-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-17 00:25:24.087089 pulumi_tailscale_native-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:25:24.083089 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:25:24.083089 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:25:24.083089 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/authorize_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/get_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/key_expiry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:25:24.087089 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/dns_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/get_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/get_dns_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/get_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/get_name_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/list_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/list_search_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/name_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/replace_search_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:25:24.083089 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-17 00:25:24.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-17 00:25:24.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:25:24.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:25:24.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 00:25:24.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 00:25:24.000000 pulumi_tailscale_native-0.0.9/pulumi_tailscale_native.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 00:25:24.087089 pulumi_tailscale_native-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-17 00:25:23.000000 pulumi_tailscale_native-0.0.9/setup.py
```

### Comparing `pulumi_tailscale_native-0.0.7/PKG-INFO` & `pulumi_tailscale_native-0.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pulumi_tailscale_native
-Version: 0.0.7
-Summary: A native Pulumi package for creating and managing Tailscale resources.
-Home-page: https://cloudysky.software
-License: Apache-2.0
-Project-URL: Repository, https://github.com/cloudy-sky-software/pulumi-tailscale-native
-Keywords: pulumi tailscale-native category/cloud kind/native
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Pulumi Native Provider for Tailscale (Preview)
 
 [Tailscale](https://tailscale.com/) connects your team's devices and development environments for easy access to remote resources.
 
 :information_source: This provider uses Tailscale's API directly.
 
 > This provider was generated using [`pulschema`](https://github.com/cloudy-sky-software/pulschema) and [`pulumi-provider-framework`](https://github.com/cloudy-sky-software/pulumi-provider-framework).
@@ -27,14 +15,31 @@
 - Node.js: https://www.npmjs.com/package/@cloudyskysoftware/pulumi-tailscale-native
 - Python: https://pypi.org/project/pulumi_tailscale_native/
 - .NET: https://www.nuget.org/packages/Pulumi.TailscaleNative
 - Go: `import github.com/cloudy-sky-software/pulumi-tailscale-native/sdk/go/tailscale`
 
 ## Using The Provider
 
+### OAuth2 Client
+
+A quote from Tailscale's own docs:
+
+> OAuth clients provide a framework for delegated and scoped access to the Tailscale API. An OAuth client creates access tokens for scoped API access, instead of using a fully-permitted access token which expires after 90 days (or less if the fully-permitted access token has a shorter expiry). OAuth clients support the principle of least privilege by allowing fine-grained control on the access granted to the client using scopes, unlike a fully-permitted access token which grants full access to the Tailscale API.
+
+- Create an OAuth client on https://login.tailscale.com/admin/settings/oauth.
+- Grant the appropriate scopes (permissions) to the client.
+- Copy the client ID and secret.
+- Set the client ID with `pulumi config set tailscale:clientId <clientID>`.
+- Set the client secret with `pulumi config set --secret tailscale:clientSecret <clientSecret>`.
+- Optional: Remove the API key config `tailscale:apiKey` from your stack config if you previously used that method of auth.
+
+Read the full official docs at https://tailscale.com/kb/1215/oauth-clients/.
+
+### API Key
+
 You'll need an API access token (aka API key). Follow Tailscale's [docs](https://tailscale.com/kb/1101/api/?q=API%20access#authentication) for creating one or head straight to your tailnet [admin console](https://login.tailscale.com/admin/settings/keys) to create one.
 Then set the API key as a secret with `pulumi config set --secret tailscale-native:apiKey`.
 
 ## Releasing A New Version
 
 :info: Switch to the `main` branch first and get the latest `git pull origin main && git fetch`. Check what the last release tag was.
 
@@ -49,9 +54,7 @@
    ```
 
 1. Push the tags.
 
    ```bash
    git push --tags
    ```
-
-
```

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/__init__.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/_utilities.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/authorize_device.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/authorize_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/get_device.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/get_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/get_routes.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/get_routes.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/key_expiry.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/key_expiry.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/outputs.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/routes.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/routes.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/device/tags.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/device/tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/provider.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/replace_search_paths.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,94 +3,123 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
-__all__ = ['ProviderArgs', 'Provider']
+__all__ = ['ReplaceSearchPathsArgs', 'ReplaceSearchPaths']
 
 @pulumi.input_type
-class ProviderArgs:
+class ReplaceSearchPathsArgs:
     def __init__(__self__, *,
-                 api_key: Optional[pulumi.Input[str]] = None):
+                 search_paths: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 tailnet: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Provider resource.
-        :param pulumi.Input[str] api_key: The Tailscale API key.
+        The set of arguments for constructing a ReplaceSearchPaths resource.
         """
-        if api_key is None:
-            api_key = _utilities.get_env('TAILSCALE_NATIVE_APIKEY', 'TAILSCALE_APIKEY')
-        if api_key is not None:
-            pulumi.set(__self__, "api_key", api_key)
+        pulumi.set(__self__, "search_paths", search_paths)
+        if tailnet is not None:
+            pulumi.set(__self__, "tailnet", tailnet)
 
     @property
-    @pulumi.getter(name="apiKey")
-    def api_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Tailscale API key.
-        """
-        return pulumi.get(self, "api_key")
+    @pulumi.getter(name="searchPaths")
+    def search_paths(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        return pulumi.get(self, "search_paths")
+
+    @search_paths.setter
+    def search_paths(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "search_paths", value)
+
+    @property
+    @pulumi.getter
+    def tailnet(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "tailnet")
 
-    @api_key.setter
-    def api_key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "api_key", value)
+    @tailnet.setter
+    def tailnet(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "tailnet", value)
 
 
-class Provider(pulumi.ProviderResource):
+class ReplaceSearchPaths(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 api_key: Optional[pulumi.Input[str]] = None,
+                 search_paths: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 tailnet: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The provider type for the Tailscale package.
-
+        Create a ReplaceSearchPaths resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] api_key: The Tailscale API key.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ProviderArgs] = None,
+                 args: ReplaceSearchPathsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The provider type for the Tailscale package.
-
+        Create a ReplaceSearchPaths resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param ProviderArgs args: The arguments to use to populate this resource's properties.
+        :param ReplaceSearchPathsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ProviderArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ReplaceSearchPathsArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 api_key: Optional[pulumi.Input[str]] = None,
+                 search_paths: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 tailnet: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ProviderArgs.__new__(ProviderArgs)
+            __props__ = ReplaceSearchPathsArgs.__new__(ReplaceSearchPathsArgs)
 
-            if api_key is None:
-                api_key = _utilities.get_env('TAILSCALE_NATIVE_APIKEY', 'TAILSCALE_APIKEY')
-            __props__.__dict__["api_key"] = None if api_key is None else pulumi.Output.secret(api_key)
-        super(Provider, __self__).__init__(
-            'tailscale-native',
+            if search_paths is None and not opts.urn:
+                raise TypeError("Missing required property 'search_paths'")
+            __props__.__dict__["search_paths"] = search_paths
+            __props__.__dict__["tailnet"] = tailnet
+        super(ReplaceSearchPaths, __self__).__init__(
+            'tailscale-native:tailnet:replaceSearchPaths',
             resource_name,
             __props__,
             opts)
 
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'ReplaceSearchPaths':
+        """
+        Get an existing ReplaceSearchPaths resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = ReplaceSearchPathsArgs.__new__(ReplaceSearchPathsArgs)
+
+        __props__.__dict__["search_paths"] = None
+        return ReplaceSearchPaths(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter(name="searchPaths")
+    def search_paths(self) -> pulumi.Output[Sequence[str]]:
+        return pulumi.get(self, "search_paths")
+
```

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/__init__.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/_inputs.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/acl.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/dns_preferences.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/dns_preferences.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/get_acl.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/get_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/get_dns_preferences.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/get_dns_preferences.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/get_key.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/get_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/get_name_servers.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/get_name_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/key.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/list_devices.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/list_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/list_keys.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/list_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/list_search_paths.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/list_search_paths.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/name_servers.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/name_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/outputs.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/tailnet/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native/tailnet/replace_search_paths.py` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native/provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,123 +3,142 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
-__all__ = ['ReplaceSearchPathsArgs', 'ReplaceSearchPaths']
+__all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
-class ReplaceSearchPathsArgs:
+class ProviderArgs:
     def __init__(__self__, *,
-                 search_paths: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 tailnet: Optional[pulumi.Input[str]] = None):
+                 api_key: Optional[pulumi.Input[str]] = None,
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 client_secret: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] api_key: The Tailscale API key.
+        :param pulumi.Input[str] client_id: The Tailscale OAuth client ID.
+        :param pulumi.Input[str] client_secret: The Tailscale OAuth client secret.
+        """
+        if api_key is None:
+            api_key = _utilities.get_env('TAILSCALE_NATIVE_APIKEY', 'TAILSCALE_APIKEY')
+        if api_key is not None:
+            pulumi.set(__self__, "api_key", api_key)
+        if client_id is None:
+            client_id = _utilities.get_env('TAILSCALE_NATIVE_CLIENT_ID', 'TAILSCALE_CLIENT_ID')
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if client_secret is None:
+            client_secret = _utilities.get_env('TAILSCALE_NATIVE_CLIENT_SECRET', 'TAILSCALE_CLIENT_SECRET')
+        if client_secret is not None:
+            pulumi.set(__self__, "client_secret", client_secret)
+
+    @property
+    @pulumi.getter(name="apiKey")
+    def api_key(self) -> Optional[pulumi.Input[str]]:
         """
-        The set of arguments for constructing a ReplaceSearchPaths resource.
+        The Tailscale API key.
         """
-        pulumi.set(__self__, "search_paths", search_paths)
-        if tailnet is not None:
-            pulumi.set(__self__, "tailnet", tailnet)
+        return pulumi.get(self, "api_key")
+
+    @api_key.setter
+    def api_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "api_key", value)
 
     @property
-    @pulumi.getter(name="searchPaths")
-    def search_paths(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "search_paths")
-
-    @search_paths.setter
-    def search_paths(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "search_paths", value)
+    @pulumi.getter(name="clientId")
+    def client_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The Tailscale OAuth client ID.
+        """
+        return pulumi.get(self, "client_id")
+
+    @client_id.setter
+    def client_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "client_id", value)
 
     @property
-    @pulumi.getter
-    def tailnet(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "tailnet")
+    @pulumi.getter(name="clientSecret")
+    def client_secret(self) -> Optional[pulumi.Input[str]]:
+        """
+        The Tailscale OAuth client secret.
+        """
+        return pulumi.get(self, "client_secret")
 
-    @tailnet.setter
-    def tailnet(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tailnet", value)
+    @client_secret.setter
+    def client_secret(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "client_secret", value)
 
 
-class ReplaceSearchPaths(pulumi.CustomResource):
+class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 search_paths: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 tailnet: Optional[pulumi.Input[str]] = None,
+                 api_key: Optional[pulumi.Input[str]] = None,
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 client_secret: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a ReplaceSearchPaths resource with the given unique name, props, and options.
+        The provider type for the Tailscale package.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] api_key: The Tailscale API key.
+        :param pulumi.Input[str] client_id: The Tailscale OAuth client ID.
+        :param pulumi.Input[str] client_secret: The Tailscale OAuth client secret.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ReplaceSearchPathsArgs,
+                 args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a ReplaceSearchPaths resource with the given unique name, props, and options.
+        The provider type for the Tailscale package.
+
         :param str resource_name: The name of the resource.
-        :param ReplaceSearchPathsArgs args: The arguments to use to populate this resource's properties.
+        :param ProviderArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ReplaceSearchPathsArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProviderArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 search_paths: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 tailnet: Optional[pulumi.Input[str]] = None,
+                 api_key: Optional[pulumi.Input[str]] = None,
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 client_secret: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ReplaceSearchPathsArgs.__new__(ReplaceSearchPathsArgs)
+            __props__ = ProviderArgs.__new__(ProviderArgs)
 
-            if search_paths is None and not opts.urn:
-                raise TypeError("Missing required property 'search_paths'")
-            __props__.__dict__["search_paths"] = search_paths
-            __props__.__dict__["tailnet"] = tailnet
-        super(ReplaceSearchPaths, __self__).__init__(
-            'tailscale-native:tailnet:replaceSearchPaths',
+            if api_key is None:
+                api_key = _utilities.get_env('TAILSCALE_NATIVE_APIKEY', 'TAILSCALE_APIKEY')
+            __props__.__dict__["api_key"] = None if api_key is None else pulumi.Output.secret(api_key)
+            if client_id is None:
+                client_id = _utilities.get_env('TAILSCALE_NATIVE_CLIENT_ID', 'TAILSCALE_CLIENT_ID')
+            __props__.__dict__["client_id"] = client_id
+            if client_secret is None:
+                client_secret = _utilities.get_env('TAILSCALE_NATIVE_CLIENT_SECRET', 'TAILSCALE_CLIENT_SECRET')
+            __props__.__dict__["client_secret"] = None if client_secret is None else pulumi.Output.secret(client_secret)
+        super(Provider, __self__).__init__(
+            'tailscale-native',
             resource_name,
             __props__,
             opts)
 
-    @staticmethod
-    def get(resource_name: str,
-            id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'ReplaceSearchPaths':
-        """
-        Get an existing ReplaceSearchPaths resource's state with the given name, id, and optional extra
-        properties used to qualify the lookup.
-
-        :param str resource_name: The unique name of the resulting resource.
-        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
-        :param pulumi.ResourceOptions opts: Options for the resource.
-        """
-        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
-
-        __props__ = ReplaceSearchPathsArgs.__new__(ReplaceSearchPathsArgs)
-
-        __props__.__dict__["search_paths"] = None
-        return ReplaceSearchPaths(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="searchPaths")
-    def search_paths(self) -> pulumi.Output[Sequence[str]]:
-        return pulumi.get(self, "search_paths")
-
```

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native.egg-info/PKG-INFO` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-tailscale-native
-Version: 0.0.7
+Version: 0.0.9
 Summary: A native Pulumi package for creating and managing Tailscale resources.
 Home-page: https://cloudysky.software
 License: Apache-2.0
 Project-URL: Repository, https://github.com/cloudy-sky-software/pulumi-tailscale-native
 Keywords: pulumi tailscale-native category/cloud kind/native
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -27,14 +27,31 @@
 - Node.js: https://www.npmjs.com/package/@cloudyskysoftware/pulumi-tailscale-native
 - Python: https://pypi.org/project/pulumi_tailscale_native/
 - .NET: https://www.nuget.org/packages/Pulumi.TailscaleNative
 - Go: `import github.com/cloudy-sky-software/pulumi-tailscale-native/sdk/go/tailscale`
 
 ## Using The Provider
 
+### OAuth2 Client
+
+A quote from Tailscale's own docs:
+
+> OAuth clients provide a framework for delegated and scoped access to the Tailscale API. An OAuth client creates access tokens for scoped API access, instead of using a fully-permitted access token which expires after 90 days (or less if the fully-permitted access token has a shorter expiry). OAuth clients support the principle of least privilege by allowing fine-grained control on the access granted to the client using scopes, unlike a fully-permitted access token which grants full access to the Tailscale API.
+
+- Create an OAuth client on https://login.tailscale.com/admin/settings/oauth.
+- Grant the appropriate scopes (permissions) to the client.
+- Copy the client ID and secret.
+- Set the client ID with `pulumi config set tailscale:clientId <clientID>`.
+- Set the client secret with `pulumi config set --secret tailscale:clientSecret <clientSecret>`.
+- Optional: Remove the API key config `tailscale:apiKey` from your stack config if you previously used that method of auth.
+
+Read the full official docs at https://tailscale.com/kb/1215/oauth-clients/.
+
+### API Key
+
 You'll need an API access token (aka API key). Follow Tailscale's [docs](https://tailscale.com/kb/1101/api/?q=API%20access#authentication) for creating one or head straight to your tailnet [admin console](https://login.tailscale.com/admin/settings/keys) to create one.
 Then set the API key as a secret with `pulumi config set --secret tailscale-native:apiKey`.
 
 ## Releasing A New Version
 
 :info: Switch to the `main` branch first and get the latest `git pull origin main && git fetch`. Check what the last release tag was.
```

### Comparing `pulumi_tailscale_native-0.0.7/pulumi_tailscale_native.egg-info/SOURCES.txt` & `pulumi_tailscale_native-0.0.9/pulumi_tailscale_native.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_tailscale_native-0.0.7/setup.py` & `pulumi_tailscale_native-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.7"
-PLUGIN_VERSION = "0.0.7"
+VERSION = "0.0.9"
+PLUGIN_VERSION = "0.0.9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'tailscale-native', PLUGIN_VERSION, '--server', 'github://api.github.com/cloudy-sky-software/pulumi-tailscale-native'])
         except OSError as error:
```

