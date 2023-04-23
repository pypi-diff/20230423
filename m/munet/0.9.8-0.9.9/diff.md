# Comparing `tmp/munet-0.9.8.tar.gz` & `tmp/munet-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "munet-0.9.8.tar", max compression
+gzip compressed data, was "munet-0.9.9.tar", max compression
```

## Comparing `munet-0.9.8.tar` & `munet-0.9.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    17895 2022-09-19 20:34:15.137746 munet-0.9.8/LICENSE.md
--rw-r--r--   0        0        0    19776 2022-09-19 20:34:15.137746 munet-0.9.8/README.org
--rw-r--r--   0        0        0     1549 2022-09-19 20:34:15.149747 munet-0.9.8/munet/__init__.py
--rw-r--r--   0        0        0     6203 2022-09-19 20:34:15.149747 munet-0.9.8/munet/__main__.py
--rw-r--r--   0        0        0    73501 2022-09-19 20:34:15.149747 munet-0.9.8/munet/base.py
--rw-r--r--   0        0        0     4087 2022-09-19 20:34:15.149747 munet-0.9.8/munet/cleanup.py
--rw-r--r--   0        0        0    26455 2022-09-19 20:34:15.149747 munet-0.9.8/munet/cli.py
--rw-r--r--   0        0        0     3967 2022-09-19 20:34:15.149747 munet-0.9.8/munet/config.py
--rw-r--r--   0        0        0     2074 2022-09-19 20:34:15.149747 munet-0.9.8/munet/kinds.yaml
--rw-r--r--   0        0        0      557 2022-09-19 20:34:15.149747 munet-0.9.8/munet/logconf.yaml
--rw-r--r--   0        0        0     3020 2022-09-19 20:34:15.149747 munet-0.9.8/munet/mucmd.py
--rw-r--r--   0        0        0     5558 2022-09-19 20:34:15.149747 munet-0.9.8/munet/munet-schema.yaml
--rw-r--r--   0        0        0    77119 2022-09-19 20:34:15.149747 munet-0.9.8/munet/native.py
--rw-r--r--   0        0        0     7791 2022-09-19 20:34:15.149747 munet-0.9.8/munet/parser.py
--rw-r--r--   0        0        0        0 2022-09-19 20:34:15.149747 munet-0.9.8/munet/testing/__init__.py
--rw-r--r--   0        0        0     8411 2022-09-19 20:34:15.149747 munet-0.9.8/munet/testing/fixtures.py
--rw-r--r--   0        0        0     6930 2022-09-19 20:34:15.149747 munet-0.9.8/munet/testing/hooks.py
--rw-r--r--   0        0        0     4332 2022-09-19 20:34:15.149747 munet-0.9.8/munet/testing/util.py
--rw-r--r--   0        0        0     4155 2022-09-19 20:34:15.149747 munet-0.9.8/munet/unshare.py
--rw-r--r--   0        0        0     3403 2022-09-19 20:34:15.149747 munet-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    21727 1970-01-01 00:00:00.000000 munet-0.9.8/setup.py
--rw-r--r--   0        0        0    21130 1970-01-01 00:00:00.000000 munet-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    17895 2022-09-22 17:11:32.695851 munet-0.9.9/LICENSE.md
+-rw-r--r--   0        0        0    19776 2022-09-22 17:11:32.695851 munet-0.9.9/README.org
+-rw-r--r--   0        0        0     1549 2022-09-22 17:11:32.703852 munet-0.9.9/munet/__init__.py
+-rw-r--r--   0        0        0     6203 2022-09-22 17:11:32.703852 munet-0.9.9/munet/__main__.py
+-rw-r--r--   0        0        0    73805 2022-09-22 17:11:32.703852 munet-0.9.9/munet/base.py
+-rw-r--r--   0        0        0     4087 2022-09-22 17:11:32.703852 munet-0.9.9/munet/cleanup.py
+-rw-r--r--   0        0        0    26455 2022-09-22 17:11:32.703852 munet-0.9.9/munet/cli.py
+-rw-r--r--   0        0        0     3967 2022-09-22 17:11:32.703852 munet-0.9.9/munet/config.py
+-rw-r--r--   0        0        0     2074 2022-09-22 17:11:32.703852 munet-0.9.9/munet/kinds.yaml
+-rw-r--r--   0        0        0      557 2022-09-22 17:11:32.703852 munet-0.9.9/munet/logconf.yaml
+-rw-r--r--   0        0        0     3020 2022-09-22 17:11:32.703852 munet-0.9.9/munet/mucmd.py
+-rw-r--r--   0        0        0     5558 2022-09-22 17:11:32.703852 munet-0.9.9/munet/munet-schema.yaml
+-rw-r--r--   0        0        0    77137 2022-09-22 17:11:32.703852 munet-0.9.9/munet/native.py
+-rw-r--r--   0        0        0     7791 2022-09-22 17:11:32.703852 munet-0.9.9/munet/parser.py
+-rw-r--r--   0        0        0        0 2022-09-22 17:11:32.703852 munet-0.9.9/munet/testing/__init__.py
+-rw-r--r--   0        0        0     8411 2022-09-22 17:11:32.703852 munet-0.9.9/munet/testing/fixtures.py
+-rw-r--r--   0        0        0     6930 2022-09-22 17:11:32.703852 munet-0.9.9/munet/testing/hooks.py
+-rw-r--r--   0        0        0     4332 2022-09-22 17:11:32.703852 munet-0.9.9/munet/testing/util.py
+-rw-r--r--   0        0        0     4155 2022-09-22 17:11:32.703852 munet-0.9.9/munet/unshare.py
+-rw-r--r--   0        0        0     3403 2022-09-22 17:11:32.703852 munet-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    21727 1970-01-01 00:00:00.000000 munet-0.9.9/setup.py
+-rw-r--r--   0        0        0    21130 1970-01-01 00:00:00.000000 munet-0.9.9/PKG-INFO
```

### Comparing `munet-0.9.8/LICENSE.md` & `munet-0.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/README.org` & `munet-0.9.9/README.org`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/__init__.py` & `munet-0.9.9/munet/__init__.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/__main__.py` & `munet-0.9.9/munet/__main__.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/base.py` & `munet-0.9.9/munet/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1989,17 +1989,27 @@
 
     class ShellWrapper(REPLWrapper):
         """
         REPLWrapper - a read-execute-print-loop interface
         """
 
         def __init__(
-            self, cmd_or_spawn, orig_prompt, prompt_change, will_echo=False, **kwargs
+            self,
+            cmd_or_spawn,
+            orig_prompt,
+            prompt_change,
+            will_echo=False,
+            escape_ansi=False,
+            **kwargs,
         ):
             self.echo = will_echo
+            self.escape = (
+                re.compile(r"(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]") if escape_ansi else None
+            )
+
             # REPLWrapper expect a non-echoing child or will create one if given a
             # command string
             super().__init__(cmd_or_spawn, orig_prompt, prompt_change, **kwargs)
 
         def cmd_nostatus(self, cmd, timeout=-1):
             """Execute a shell command
 
@@ -2016,14 +2026,16 @@
                         cmd,
                         output,
                     )
                 else:
                     # Remove up to and including the command from the output stream
                     output = output[idx + len(cmd) :]
 
+            if self.escape:
+                output = self.escape.sub("", output)
             return output.replace("\r", "").strip()
 
         def cmd_status(self, cmd, timeout=-1):
             """Execute a shell command
 
             Returns status and (strip/cleaned \r) output
             """
```

### Comparing `munet-0.9.8/munet/cleanup.py` & `munet-0.9.9/munet/cleanup.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/cli.py` & `munet-0.9.9/munet/cli.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/config.py` & `munet-0.9.9/munet/config.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/kinds.yaml` & `munet-0.9.9/munet/kinds.yaml`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/logconf.yaml` & `munet-0.9.9/munet/logconf.yaml`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/mucmd.py` & `munet-0.9.9/munet/mucmd.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/munet-schema.yaml` & `munet-0.9.9/munet/munet-schema.yaml`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/native.py` & `munet-0.9.9/munet/native.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
         p = self.spawn(sock, prompt, logfile=logfile, logfile_read=logfile_read)
         from .base import ShellWrapper  # pylint: disable=C0415
 
         # ShellWrapper (REPLWrapper) unfortunately uses string match not regex
         # for the prompt
         p.send("\n")
         prompt = "(qemu) "
-        return ShellWrapper(p, prompt, None, will_echo=True)
+        return ShellWrapper(p, prompt, None, will_echo=True, escape_ansi=True)
 
     def mount_volumes(self):
         for m in self.config.get("volumes", []):
             if isinstance(m, str):
                 s = m.split(":", 1)
                 if len(s) == 1:
                     self.tmpfs_mount(s[0])
```

### Comparing `munet-0.9.8/munet/parser.py` & `munet-0.9.9/munet/parser.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/testing/fixtures.py` & `munet-0.9.9/munet/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/testing/hooks.py` & `munet-0.9.9/munet/testing/hooks.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/testing/util.py` & `munet-0.9.9/munet/testing/util.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/munet/unshare.py` & `munet-0.9.9/munet/unshare.py`

 * *Files identical despite different names*

### Comparing `munet-0.9.8/pyproject.toml` & `munet-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "munet"
-version = "0.9.8"
+version = "0.9.9"
 description = "A package to facilitate network simulations"
 authors = ["Christian Hopps <chopps@labn.net>"]
 license = "GPL-2.0-or-later"
 readme = "README.org"
 repository = "https://github.com/LabNConsulting/munet"
 
 include = ["logconf.yaml", "munet-schema.yaml"]
```

### Comparing `munet-0.9.8/setup.py` & `munet-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'validate': ['jsonschema>=4.6.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['mucmd = munet.mucmd:main', 'munet = munet.__main__:main']}
 
 setup_kwargs = {
     'name': 'munet',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'A package to facilitate network simulations',
     'long_description': '* μNET (munet)\n\n[[ci-badge-main][https://github.com/LabNConsulting/munet/actions/workflows/ci.yml/badge.svg?branch=main]] [[https://codecov.io/gh/LabNConsulting/munet][https://codecov.io/gh/LabNConsulting/munet/branch/main/graph/badge.svg?token=FD2O4YGDTT]]\n\nA package for creating network topologies and running programs and containers\nwithin them using linux namepsaces.\n\nMunet can be run in a standalone mode with a configuration file for launching\nlinux shell and container based topologies, as well as be used as a library from\nwithin another application to provide the same functionality.\n\n* Standalone Config\n\nThe standalone config can be provided in a number of formats, limited by the\navailable encode/decode libraries withing the python environment. As JSON is\nbuilt in to python that format is always supported. Additionally YAML and TOML\nare supported if the corresponding packages are available (i.e., ~PyYAML~ and\n~toml~).\n\nThe config itself is defined with a YANG model which is defined in the following\nsections.\n\n** Config Tree\n\n#+NAME: Munet standalone config YANG tree diagram\n#+HEADER: :var module=labn-munet-config\n#+begin_src shell :results output verbatim replace :wrap example :exports results\n  [ -d /yang ] || DOCKER="docker run --net=host -v $(pwd):/work labn/org-rfc"\n  $DOCKER pyang --tree-line-length=69 -f tree ${module} 2> err.out;\n#+end_src\n\n\n#+RESULTS: Munet standalone config YANG tree diagram\n#+begin_example\nmodule: labn-munet-config\n  +--rw cli\n  |  +--rw commands* [name]\n  |     +--rw exec?         string\n  |     +--rw exec-kind* [kind]\n  |     |  +--rw kind    string\n  |     |  +--rw exec?   string\n  |     +--rw format?       string\n  |     +--rw help?         string\n  |     +--rw kinds*        -> ../../../kinds/name\n  |     +--rw name          string\n  |     +--rw new-window?   boolean\n  |     +--rw top-level?    boolean\n  +--rw kinds* [name]\n  |  +--rw merge*         string\n  |  +--rw cap-add*       string\n  |  +--rw cap-remove*    string\n  |  +--rw cmd?           string\n  |  +--rw cleanup_cmd?   string\n  |  +--rw connections* [to]\n  |  |  +--rw to                    string\n  |  |  +--rw ip?                   string\n  |  |  +--rw name?                 string\n  |  |  +--rw hostintf?             string\n  |  |  +--rw physical?             string\n  |  |  +--rw remote-name?          string\n  |  |  +--rw delay?                uint64\n  |  |  +--rw jitter?               uint64\n  |  |  +--rw jitter-correlation?   decimal64\n  |  |  +--rw loss?                 uint64\n  |  |  +--rw loss-correlation?     decimal64\n  |  |  +--rw rate\n  |  |     +--rw rate?    number64\n  |  |     +--rw limit?   number64\n  |  |     +--rw burst?   number64\n  |  +--rw env* [name]\n  |  |  +--rw name     string\n  |  |  +--rw value?   string\n  |  +--rw image?         string\n  |  +--rw init?          union\n  |  +--rw mounts* [destination]\n  |  |  +--rw destination    string\n  |  |  +--rw source?        string\n  |  |  +--rw tmpfs-size?    string\n  |  |  +--rw type?          string\n  |  +--rw name           string\n  |  +--rw podman\n  |  |  +--rw extra-args*   string\n  |  +--rw privileged?    boolean\n  |  +--rw shell?         union\n  |  +--rw volumes*       string\n  +--rw topology\n  |  +--rw ipv6-enable?           boolean\n  |  +--rw networks-autonumber?   boolean\n  |  +--rw networks* [name]\n  |  |  +--rw name    string\n  |  |  +--rw ip?     string\n  |  +--rw nodes* [name]\n  |     +--rw id?            uint32\n  |     +--rw kind?          -> ../../../kinds/name\n  |     +--rw cap-add*       string\n  |     +--rw cap-remove*    string\n  |     +--rw cmd?           string\n  |     +--rw cleanup_cmd?   string\n  |     +--rw connections* [to]\n  |     |  +--rw to                    string\n  |     |  +--rw ip?                   string\n  |     |  +--rw name?                 string\n  |     |  +--rw hostintf?             string\n  |     |  +--rw physical?             string\n  |     |  +--rw remote-name?          string\n  |     |  +--rw delay?                uint64\n  |     |  +--rw jitter?               uint64\n  |     |  +--rw jitter-correlation?   decimal64\n  |     |  +--rw loss?                 uint64\n  |     |  +--rw loss-correlation?     decimal64\n  |     |  +--rw rate\n  |     |     +--rw rate?    number64\n  |     |     +--rw limit?   number64\n  |     |     +--rw burst?   number64\n  |     +--rw env* [name]\n  |     |  +--rw name     string\n  |     |  +--rw value?   string\n  |     +--rw image?         string\n  |     +--rw init?          union\n  |     +--rw mounts* [destination]\n  |     |  +--rw destination    string\n  |     |  +--rw source?        string\n  |     |  +--rw tmpfs-size?    string\n  |     |  +--rw type?          string\n  |     +--rw name           string\n  |     +--rw podman\n  |     |  +--rw extra-args*   string\n  |     +--rw privileged?    boolean\n  |     +--rw shell?         union\n  |     +--rw volumes*       string\n  +--rw version?    uint32\n#+end_example\n\n\n** Config Model\n\n#+NAME: test-validate-module\n#+begin_src emacs-lisp :exports none\n  (org-sbe "validate-module" (module labn-munet-config))\n#+end_src\n\n#+RESULTS: test-validate-module\n\n#+NAME: labn-munet-config\n#+HEADER: :var dep1=dep-babel :var dep2=fetch-yang-files\n#+HEADER: :file labn-munet-config.yang :results output file silent :cache yes\n#+begin_src yang :exports code\n  module labn-munet-config {\n    yang-version 1.1;\n    namespace "urn:labn:yang:labn-munet-config";\n    prefix c;\n\n    organization\n      "LabN Consulting, L.L.C.";\n\n    contact\n      "Author: Christian Hopps\n               <mailto:chopps@labn.net>";\n\n    description\n      "This module defines the configuration state for munet.";\n\n    revision 2021-12-18 {\n      description "Initial Revision";\n      reference "https://github.com/LabNConsulting/munet/blob/main/README.md";\n    }\n\n    typedef number64 {\n      type union {\n        type uint64;\n        type string {\n          pattern \'[0-9]+([KMGTPE]i?)?\';\n        }\n      }\n      description\n        "A number with optional suffix, where suffix means:\n           K -> value*10^3, Ki -> value*2^10,\n           M -> value*10^6, Mi -> value*2^20,\n           G -> value*10^9, Gi -> value*2^30,\n           T -> value*10^12, Gi -> value*2^40,\n           P -> value*10^15, Gi -> value*2^50,\n           E -> value*10^18, Gi -> value*2^60";\n    }\n\n    grouping intf-constraints {\n      description "traffic control based interface constraints";\n      leaf delay {\n        type uint64;\n        description "number of microseconds of delay";\n      }\n      leaf jitter {\n        type uint64;\n        must "../delay";\n        description "number of microseconds of possible jitter";\n      }\n      leaf jitter-correlation {\n        type decimal64 {\n          fraction-digits 16;\n          range "0..100";\n        }\n        must "../jitter";\n        description "percent correlation between consecutive jitter values";\n      }\n      leaf loss {\n        type uint64;\n        must "../delay";\n        description "number of microseconds of possible jitter";\n      }\n      leaf loss-correlation {\n        type decimal64 {\n          fraction-digits 16;\n          range "0..100";\n        }\n        must "../loss";\n        description "percent correlation between consecutive loss values";\n      }\n      container rate {\n        description "bits per second maximum rate with possible limit and burst";\n        leaf rate {\n          type number64;\n          description "bits per second maximum rate";\n        }\n        leaf limit {\n          type number64;\n          must "../rate";\n          description "bits per second maximum rate";\n        }\n        leaf burst {\n          type number64;\n          must "../rate";\n          description "bits per second maximum rate";\n        }\n      }\n    }\n\n    grouping common-node {\n      description "Common node properties";\n      leaf-list cap-add {\n        type string;\n        description "Capabilities to add to a container.";\n        reference "https://man7.org/linux/man-pages/man7/capabilities.7.html";\n      }\n      leaf-list cap-remove {\n        type string;\n        description "Capabilities to remove from a container.";\n        reference "https://man7.org/linux/man-pages/man7/capabilities.7.html";\n      }\n      leaf cmd {\n        type string;\n        description "Shell command[s] to execute when creating the node.";\n      }\n      leaf cleanup_cmd {\n        type string;\n        description\n          "Shell command[s] to execute when deleting the node.\n\n           NOTE: With container nodes, the cleanup_cmd will be run\n           prior to the `cmd` being killed, so that the container is\n           present. For Qemu/VM nodes the cleanup command is run prior\n           to the VM being brought down.";\n      }\n      leaf image {\n        type string;\n        description "Container image specification.";\n      }\n      container qemu {\n        description "Specify parameters for Qemu VM node";\n        leaf kerenel {\n          type string;\n          description "path to kernel image (e.g,. bzImage) to boot";\n        }\n        leaf initrd {\n          type string;\n          description "path to initrd image (e.g,. rootfs.ext2) to boot";\n        }\n        leaf kvm {\n          type boolean;\n          default true;\n          description "Run with HW acceleration";\n        }\n        leaf ncpu {\n          type uint32;\n          default 1;\n          description "Number of cores";\n        }\n        leaf memory {\n          type string;\n          default "512M";\n          description "ammount of memory for VM.";\n        }\n        leaf root {\n          type string;\n          default "/dev/ram0";\n          description "root file system passed in cmdline as root=<value>";\n        }\n        leaf cmdline-extra {\n          type string;\n          description "string to add to the kernel cmdline (qemu -append)";\n        }\n        leaf extra-args {\n          type string;\n          description "extra qemu args passed when launching";\n        }\n      }\n      list connections {\n        key to;\n        description "Connections to other networks or nodes from this node";\n\n        leaf to {\n          type string;\n          description "The target of this connection.";\n        }\n        leaf ip {\n          type string;\n          description "IP address for the connection (interface).";\n        }\n        leaf name {\n          type string;\n          description "Name for the connection (interface name).";\n        }\n        leaf hostintf {\n          type string;\n          description "Host interface name for wired connections";\n        }\n        leaf physical {\n          type string;\n          description "Physical interface name for wired connections";\n        }\n        leaf remote-name {\n          type string;\n          description\n            "The remote name of a p2p connection. This is used for disambiguation\n             when there are multiple point-to-point connections to the same\n             remote node.";\n        }\n        uses intf-constraints;\n      }\n      list env {\n        key name;\n        description\n          "List of environment variable to add to the `cmd` execution\n           environment";\n        leaf name {\n          type string;\n          description "Environment variable name.";\n        }\n        leaf value {\n          type string;\n          description "Environment variable value.";\n        }\n      }\n      leaf init {\n        type union {\n          type boolean;\n          type string;\n        }\n        description "Controls use of an init process.";\n      }\n      list mounts {\n        key destination;\n        description\n          "Mounts to be made inside the namespace. Currently only supported for\n           container based nodes.";\n\n        leaf destination {\n          type string;\n          description\n            "The inner mount point. If no source is given this will be a tmpfs\n             mount, otherwise the it is a bind mount from the `source`.";\n        }\n        leaf source {\n          type string;\n          description "The source of the bind mount.";\n        }\n        leaf tmpfs-size {\n          type string;\n          description "The size of the tmpfs.";\n        }\n        leaf type {\n          type string;\n          description "The type of the mount (currently bind or tmpfs).";\n        }\n      }\n      leaf name {\n        type string;\n        description "Name of this node or kind.";\n      }\n      container podman {\n        description "Configuration related to podman containers.";\n        leaf-list extra-args {\n          type string;\n          description "list of CLI arguments to add to the podman run command.";\n        }\n      }\n      leaf privileged {\n        type boolean;\n        description "Controls running the container in privileged mode.";\n      }\n      leaf shell {\n        type union {\n          type boolean;\n          type string;\n        }\n        description\n          "Controls use of an shell process for `cmd` execution. If \'false\' then\n           `cmd` will be run directly with exec(1), otherwise a shell will be\n           used. If this value is `true` then the default shell will be used,\n           otherwise it is a string which specifies the path to the shell to\n           use.";\n      }\n      leaf-list volumes {\n        type string;\n        description\n          "Bind or tmpfs mounts. For bind mounts the format of the string is\n           <outer>:<inner>, for tmpfs it\'s simply the inner mount path.";\n      }\n    }\n\n    container cli {\n      description "CLI additions.";\n      list commands {\n        key name;\n        description "A command to add to the CLI.";\n\n        leaf exec {\n          type string;\n          description\n            "Command to execute when the CLI command is given. The string is\n             evaluated as a python f-string with `{host}` set to the current\n             host object (or None) `{unet}` set to the Munet object, and\n             `{user_input}` to any user input that follows the command (or \'\' if\n             none specified).";\n        }\n        list exec-kind {\n          key kind;\n          description "A kind specific execution formats.";\n\n          leaf kind {\n            type string;\n            description "Kind for which this command format should be used.";\n          }\n          leaf exec {\n            type string;\n            description\n              "Command to execute when the CLI command is given. The string is\n               evaluated as a python f-string with `{host}` set to the current\n               host object (or None) `{unet}` set to the Munet object, and\n               `{user_input}` to any user input that follows the command (or \'\'\n               if none specified).";\n          }\n        }\n        leaf format {\n          type string;\n          description\n            "The format of the command. Used to print help string for user.";\n        }\n        leaf help {\n          type string;\n          description\n            "The description of the command. Used to print help string for\n             user.";\n        }\n        leaf-list kinds {\n          type leafref {\n            path "../../../kinds/name";\n          }\n          description\n            "List of kinds for which this command should be restricted to running\n             on.";\n        }\n        leaf name {\n          type string;\n          description "CLI command name.";\n        }\n        leaf new-window {\n          type boolean;\n          description\n            "Controls if the command runs in the CLI window or opens a new\n             terminal window to run the command in.";\n        }\n        leaf top-level {\n          type boolean;\n          default false;\n          description\n            "If true the command is run in the top-level containing namespace. This is the\n             namespace from which each of the hosts allocated sub-namespaces from.\n             or a host namespace.";\n        }\n      }\n    }\n\n    list kinds {\n      key name;\n      description\n        "List of kinds used to group and share common node properities.";\n\n      leaf-list merge {\n        type string;\n        description\n          "List of properties which should be merged with their node specific\n           values, rather than being replaced by the node specific version.";\n      }\n      uses common-node;\n    }\n\n    container topology {\n      description "The topology munet should create.";\n\n      leaf dns-network {\n        type leafref {\n          path "../networks/name";\n        }\n        description "network used for DNS addresses of hosts in hosts files.";\n      }\n\n      leaf ipv6-enable {\n        type boolean;\n        default false;\n        description\n          "Controls if IPv6 is enabled or disabled.";\n      }\n\n      leaf networks-autonumber {\n        type boolean;\n        description\n          "Controls if networks and node connections are given IP addresses if\n           not explicitly configured.";\n      }\n\n      list networks {\n        key name;\n        description "List of networks to create.";\n\n        leaf name {\n          type string {\n            length "1..11";\n            pattern "[-a-zA-Z0-9_]+";\n          }\n          description "Name of the network";\n        }\n        leaf ip {\n          type string;\n          description\n            "IP prefix for the network. If host bit\'s are set then the linux\n             bridge will be assigned that IP.";\n        }\n      }\n\n      list nodes {\n        key name;\n        description "Nodes in the topology.";\n\n        leaf id {\n          type uint32;\n          description "Explicitly set the ID for the node.";\n        }\n        leaf kind {\n          type leafref {\n            path "../../../kinds/name";\n          }\n          description\n            "Indicate the kind of this node, which pulls in the properies of that\n             `kind` for this node.";\n        }\n        uses common-node;\n      }\n    }\n    leaf version {\n      type uint32;\n      description "version of this config";\n    }\n  }\n#+end_src\n\n#+name: dep-babel\n#+begin_src emacs-lisp :results none :exports none\n    (org-babel-do-load-languages \'org-babel-load-languages \'((shell . t)))\n    (setq fill-column 69)\n    (setq org-confirm-babel-evaluate nil)\n#+end_src\n\n#+name: fetch-yang-files\n#+begin_src shell :results none silent :exports none\n      curl -O https://raw.githubusercontent.com/YangModels/yang/master/standard/ietf/RFC/ietf-routing-types@2017-12-04.yang\n      curl -O https://raw.githubusercontent.com/YangModels/yang/master/standard/ietf/RFC/ietf-routing@2018-03-13.yang\n#+end_src\n\n#+NAME: generate-tree\n#+HEADER: :var dep1=dep-babel\n#+begin_src shell :results output verbatim replace :wrap example :exports results\n  [ -d /yang ] || DOCKER="docker run --net=host -v $(pwd):/work labn/org-rfc"\n  $DOCKER pyang --tree-line-length=69 -f tree ${module} 2> err.out;\n#+end_src\n\n#+NAME: validate-module\n#+HEADER: :var dep1=dep-babel\n#+begin_src bash :results output verbatim replace :wrap comment :exports none\n  [ -d /yang ] || DOCKER="docker run --net=host -v $(pwd):/work labn/org-rfc"\n  if ! $DOCKER pyang --lax-quote-checks -Werror --lint $module 2>&1; then echo FAIL; fi\n#+end_src\n\n#+NAME: validate-config\n#+HEADER: :var dep1=dep-babel\n#+begin_src bash :results output verbatim replace :wrap comment :exports none\n  [ -d /yang ] || DOCKER="docker run --net=host -v $(pwd):/work labn/org-rfc"\n  LINT="$DOCKER yanglint -p /yang-drafts -p /yang --strict -t config"\n  $LINT $extra $module ${file} 2>&1 || echo FAIL\n#+end_src\n\n#+NAME: validate-data\n#+HEADER: :var dep1=dep-babel\n#+begin_src bash :results output verbatim replace :wrap comment :exports none\n  [ -d /yang ] || DOCKER="docker run --net=host -v $(pwd):/work labn/org-rfc"\n  LINT="$DOCKER yanglint -p /yang-drafts -p /yang --strict -t data"\n  $LINT $extra $module ${file} 2>&1 || echo FAIL\n#+end_src\n',
     'author': 'Christian Hopps',
     'author_email': 'chopps@labn.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/LabNConsulting/munet',
```

### Comparing `munet-0.9.8/PKG-INFO` & `munet-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: munet
-Version: 0.9.8
+Version: 0.9.9
 Summary: A package to facilitate network simulations
 Home-page: https://github.com/LabNConsulting/munet
 License: GPL-2.0-or-later
 Author: Christian Hopps
 Author-email: chopps@labn.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

