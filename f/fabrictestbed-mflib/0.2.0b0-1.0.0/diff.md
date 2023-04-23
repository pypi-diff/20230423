# Comparing `tmp/fabrictestbed-mflib-0.2.0b0.tar.gz` & `tmp/fabrictestbed-mflib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-mflib-0.2.0b0.tar", last modified: Thu Apr 20 21:38:11 2023, max compression
+gzip compressed data, was "fabrictestbed-mflib-1.0.0.tar", last modified: Sun Apr 23 02:50:25 2023, max compression
```

## Comparing `fabrictestbed-mflib-0.2.0b0.tar` & `fabrictestbed-mflib-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      647 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.2.0b0/.gitignore
--rw-r--r--   0        0        0      575 2023-03-29 18:17:09.721091 fabrictestbed-mflib-0.2.0b0/.readthedocs.yaml
--rw-r--r--   0        0        0     1071 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.2.0b0/LICENSE
--rw-r--r--   0        0        0       24 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.2.0b0/MANIFEST.in
--rw-r--r--   0        0        0   668002 2023-04-20 20:16:13.194055 fabrictestbed-mflib-0.2.0b0/MFLib.pdf
--rw-r--r--   0        0        0     3974 2023-04-17 18:32:21.683648 fabrictestbed-mflib-0.2.0b0/README.md
--rwxr-xr-x   0        0        0      817 2023-04-17 18:32:21.683648 fabrictestbed-mflib-0.2.0b0/create_html_doc.sh
--rwxr-xr-x   0        0        0      687 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/create_pdf_doc.sh
--rwxr-xr-x   0        0        0      668 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/create_release.sh
--rw-r--r--   0        0        0      638 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/Makefile
--rw-r--r--   0        0        0      804 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/make.bat
--rw-r--r--   0        0        0       55 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/docs/requirements.txt
-lrwxr-xr-x   0        0        0        0 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/source/_static/placeholder
--rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/source/_templates/placeholder
--rw-r--r--   0        0        0     1297 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/docs/source/conf.py
--rw-r--r--   0        0        0      204 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/docs/source/core.rst
--rw-r--r--   0        0        0    42620 2023-04-18 03:41:22.987762 fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes.png
--rw-r--r--   0        0        0    71388 2023-04-18 03:41:22.987762 fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes_add_meas.png
--rw-r--r--   0        0        0   100374 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes_ini.png
--rw-r--r--   0        0        0    70104 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes_inst.png
--rw-r--r--   0        0        0   204495 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/images/keys.png
--rw-r--r--   0        0        0      310 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/index.rst
--rw-r--r--   0        0        0       94 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/mf_timestamp.rst
--rw-r--r--   0        0        0      215 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.2.0b0/docs/source/mflib.rst
--rw-r--r--   0        0        0     6230 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/overview.md
--rw-r--r--   0        0        0       58 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/owl.rst
--rw-r--r--   0        0        0       81 2023-04-18 03:41:22.991762 fabrictestbed-mflib-0.2.0b0/docs/source/owl_data.rst
--rw-r--r--   0        0        0     7308 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.2.0b0/mflib/README.md
--rw-r--r--   0        0        0      539 2023-04-20 20:15:41.833758 fabrictestbed-mflib-0.2.0b0/mflib/__init__.py
--rw-r--r--   0        0        0    47346 2023-04-20 18:51:49.099811 fabrictestbed-mflib-0.2.0b0/mflib/core.py
--rw-r--r--   0        0        0    17118 2023-04-17 18:32:21.683648 fabrictestbed-mflib-0.2.0b0/mflib/mf_timestamp.py
--rw-r--r--   0        0        0    31971 2023-04-18 03:40:43.967413 fabrictestbed-mflib-0.2.0b0/mflib/mflib.py
--rw-r--r--   0        0        0    27967 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.2.0b0/mflib/mfvis.py
--rw-r--r--   0        0        0    15650 2023-04-18 01:21:17.807688 fabrictestbed-mflib-0.2.0b0/mflib/owl.py
--rw-r--r--   0        0        0    11858 2023-04-19 17:56:04.413586 fabrictestbed-mflib-0.2.0b0/mflib/owl_data.py
--rw-r--r--   0        0        0      735 2023-04-17 18:32:21.683648 fabrictestbed-mflib-0.2.0b0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.2.0b0/requirements.txt
--rw-r--r--   0        0        0     4484 1970-01-01 00:00:00.000000 fabrictestbed-mflib-0.2.0b0/PKG-INFO
+-rw-r--r--   0        0        0      647 2023-02-01 16:43:59.704079 fabrictestbed-mflib-1.0.0/.gitignore
+-rw-r--r--   0        0        0      575 2023-03-29 18:17:09.721091 fabrictestbed-mflib-1.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1071 2023-02-01 16:43:59.704079 fabrictestbed-mflib-1.0.0/LICENSE
+-rw-r--r--   0        0        0       24 2023-02-01 16:43:59.704079 fabrictestbed-mflib-1.0.0/MANIFEST.in
+-rw-r--r--   0        0        0   667845 2023-04-23 02:15:54.442310 fabrictestbed-mflib-1.0.0/MFLib.pdf
+-rw-r--r--   0        0        0     3974 2023-04-22 05:12:44.140491 fabrictestbed-mflib-1.0.0/README.md
+-rwxr-xr-x   0        0        0      817 2023-04-17 18:32:21.683648 fabrictestbed-mflib-1.0.0/create_html_doc.sh
+-rwxr-xr-x   0        0        0      687 2023-04-13 17:46:39.734392 fabrictestbed-mflib-1.0.0/create_pdf_doc.sh
+-rwxr-xr-x   0        0        0      668 2023-04-13 17:46:39.734392 fabrictestbed-mflib-1.0.0/create_release.sh
+-rw-r--r--   0        0        0      638 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0       74 2023-04-23 02:13:59.649527 fabrictestbed-mflib-1.0.0/docs/requirements.txt
+lrwxr-xr-x   0        0        0        0 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/source/_static/placeholder
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/source/_templates/placeholder
+-rw-r--r--   0        0        0     1297 2023-04-23 02:12:57.745116 fabrictestbed-mflib-1.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0      204 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/docs/source/core.rst
+-rw-r--r--   0        0        0    42620 2023-04-22 05:12:44.140491 fabrictestbed-mflib-1.0.0/docs/source/images/3nodes.png
+-rw-r--r--   0        0        0    71388 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_add_meas.png
+-rw-r--r--   0        0        0   100374 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_ini.png
+-rw-r--r--   0        0        0    70104 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_inst.png
+-rw-r--r--   0        0        0   204495 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/images/keys.png
+-rw-r--r--   0        0        0      310 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/index.rst
+-rw-r--r--   0        0        0       94 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/mf_timestamp.rst
+-rw-r--r--   0        0        0      215 2023-04-13 17:46:39.734392 fabrictestbed-mflib-1.0.0/docs/source/mflib.rst
+-rw-r--r--   0        0        0     6230 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/overview.md
+-rw-r--r--   0        0        0       58 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/owl.rst
+-rw-r--r--   0        0        0       81 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/docs/source/owl_data.rst
+-rw-r--r--   0        0        0     7308 2023-02-01 16:43:59.708079 fabrictestbed-mflib-1.0.0/mflib/README.md
+-rw-r--r--   0        0        0      539 2023-04-23 02:15:39.926210 fabrictestbed-mflib-1.0.0/mflib/__init__.py
+-rw-r--r--   0        0        0    47374 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.0/mflib/core.py
+-rw-r--r--   0        0        0    17118 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/mflib/mf_timestamp.py
+-rw-r--r--   0        0        0    32687 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.0/mflib/mflib.py
+-rw-r--r--   0        0        0    27981 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.0/mflib/mfvis.py
+-rw-r--r--   0        0        0    15650 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/mflib/owl.py
+-rw-r--r--   0        0        0    11857 2023-04-22 17:59:18.127064 fabrictestbed-mflib-1.0.0/mflib/owl_data.py
+-rw-r--r--   0        0        0      735 2023-04-22 05:12:44.144491 fabrictestbed-mflib-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-04-23 02:13:38.561386 fabrictestbed-mflib-1.0.0/requirements.txt
+-rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 fabrictestbed-mflib-1.0.0/PKG-INFO
```

### Comparing `fabrictestbed-mflib-0.2.0b0/.gitignore` & `fabrictestbed-mflib-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/.readthedocs.yaml` & `fabrictestbed-mflib-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/LICENSE` & `fabrictestbed-mflib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/MFLib.pdf` & `fabrictestbed-mflib-1.0.0/MFLib.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 MFLib
-Release 0.2.0b0
+Release 1.0.0
 
 Fabric UKY Team
 
-Apr 20, 2023
+Apr 22, 2023
 
 CONTENTS
 
 1
 
 Documentation Resources
 1.1 Example Jupyter Notebooks . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
@@ -83,17 +83,17 @@
 
 Index
 
 23
 
 i
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
-docs passing
+docs failing
 
 Welcome to the FABRIC Measurement Framework Library. MFLib makes it easy to install monitoring systems to a
 FABRIC experimenter’s slice. The monitoring system makes extensive use of industry standards such as Prometheus,
 Grafana, Elastic Search and Kibana while adding customized monitoring tools and dashboards for quick setup and
 visualization.
 
 CONTENTS
@@ -167,15 +167,15 @@
 
 Run the bash script to create the MFLIB.pdf documentation. MFLIB.pdf will be placed in the root directory of the
 repository.
 ./create_pdf_doc.sh
 
 4
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 3.2 Distribution Package
 MFLib package is created using Flit Be sure to create and commit the PDF documentation to GitHub before building
 and publishing to PyPi. The MFLib.pdf is included in the distributition.
 To build python package for PyPi run
 ./create_release.sh
 
@@ -216,15 +216,15 @@
 MFLib().addMeasNode(slice) where slice is a fabric slice that has been specified but not yet submitted. This example
 has 3 ndoes and an experimental network.
 
 The MFLib().addMeasNode(slice) adds an extra node called the Measurement Node (meas_node) and an measure-
 
 6
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 ment network.
 
 4.1.2 Init & Instrumentize
 MFlib works on an existing slice to which MFLib must first add some software and services.
 MFLib(slice_name) mf = MFLib(slice_name, local_storage_directory="/tmp/mflib") First you must
 create the MFLib object by passing the slice name to MFLib() . You can optionally pass a string for where you would
@@ -248,15 +248,15 @@
 – Prometheus & Grafana
 – ELK with Kibana
 
 4.1. MFLib Methods
 
 7
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 4.1.3 Service Methods
 Measurement Framework has “services” which are installed on the measurement node. The MFLib.instrumentize()
 method installs Prometheus, Grafana, and ELK.. MFLib is built on top of MFLib.Core(). MFLib uses Core methods to
 interact with services using several basic methods: create, info, update, start, stop and remove. Each of these methods
 require the service name. Most can also take an optional dictionary and an optional list of files to be uploaded. All will
 return a json object with at least a “success” and “msg” values.
@@ -285,15 +285,15 @@
 mflib.download_common_hosts mf.download_common_hosts() retrieves an ansible hosts.ini file for the slice. The
 hosts file will contain 2 groups: Experiment_nodes and Measurement_node
 
 4.1. MFLib Methods
 
 8
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 mflib.download_log_file mf.download_log_file(service, method) retrieves the log files for runs of the given
 service’s method: create, info, update. . . etc. This can be useful for debugging.
 
 4.1.4 Accessing Experiment Nodes via Bastion Host
 Many of the services set up by MFLib run web accessible user interfaces on the Measurement Node. Since experimental
 resources are secured by the FABRIC Bastion host, a tunnel must be created to access the web pages.
@@ -339,15 +339,15 @@
 Parameters
 slice_name (str) – The name of the slice to be monitored.
 Returns
 False if no Measure Node found or a init process fails. True otherwise.
 
 10
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 Return type
 Bool
 instrumentize(services=['prometheus', 'elk'])
 Instrumentize the slice. This is a convenience method that sets up & starts the monitoring of the slice. Sets
 up Prometheus, ELK & Grafana.
 Parameters
@@ -420,15 +420,15 @@
 Parameters
 • service (String) – The name of the service.
 • data (JSON serializable object) –
 • files (List of Strings) – List of filepaths to be uploaded.
 
 12
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 Returns
 Dictionary of creation results.
 Return type
 dict
 download_log_file(service, method)
 Download the log file for the given service and method. Downloaded file will be stored locally for future
@@ -468,15 +468,15 @@
 Return type
 String
 property grafana_tunnel_local_port
 If a tunnel is used for grafana, this value must be set for the port. :returns: port number :rtype: String
 
 13
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 info(service, data=None)
 Gets inormation from an existing service. Strictly gets information, does not change how the service is
 running.
 Parameters
 • service (String) – The name of the service.
 • data (JSON Serializable Object) – Data to be passed to a JSON file place in the
@@ -514,15 +514,15 @@
 property log_directory
 The full path for the log directory.
 Returns
 The full path to the log directory.
 
 14
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 Return type
 String
 property meas_node
 The fablib node object for the Measurement Node in the slice.
 Returns
 The fablib node object for the Measurement Node in the slice.
@@ -561,15 +561,15 @@
 start(services=[])
 Restarts a stopped service using existing configs on meas node.
 Parameters
 services (List of Strings) – The name of the services to be restarted.
 
 15
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 Returns
 List of start result dictionaries.
 Return type
 List
 stop(services=[])
 Stops a service, does not remove the service, just stops it from using resources.
@@ -651,15 +651,15 @@
 • pcap_int (int) – time interval (sec) at which tcpdump will start a new pcap file.
 generate_local_links_file(links)
 Create a local copy of links.json file.
 Parameters
 links ([(str, str)]) – list of endpoint pairs [(‘src_ip’, ‘dst_ip’)]
 18
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 get_local_service_file_paths()
 Get paths for owl.conf and links.json files.
 Returns
 owl.conf path, links.json path
 Return type
 [str, str]
@@ -696,15 +696,15 @@
 remove_owl_docker_image(node, name='fabric-owl')
 Remove container with the name given and OWL Docker image saved on the node.
 Parameters
 • node (fablib.Node) – remote node
 
 19
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 • name (str) – container name
 start_owl_receiver(dst_node, receiving_ip, name='fabric-owl', pcap_time_limit=360, duration=180)
 Start Docker container to run OWL receiver.
 Parameters
 • dst_node (fablib.Node) – OWL destination node
 • receiving_ip (str) – IPv4 address of dst node where OWL packets are expected.
@@ -834,15 +834,15 @@
 13
 get_local_service_file_paths() (mflib.owl.Owl mflib.owl
 module, 18
 method), 19
 mflib.owl_data.OwlDataAnalyzer
 23
 
-MFLib, Release 0.2.0b0
+MFLib, Release 1.0.0
 
 module, 21
 mflib_class_version (mflib.mflib.MFLib attribute),
 11
 module
 mflib.core, 12
 mflib.mf_timestamp.mf_timestamp, 17
```

### Comparing `fabrictestbed-mflib-0.2.0b0/README.md` & `fabrictestbed-mflib-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/create_html_doc.sh` & `fabrictestbed-mflib-1.0.0/create_html_doc.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/create_pdf_doc.sh` & `fabrictestbed-mflib-1.0.0/create_pdf_doc.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/create_release.sh` & `fabrictestbed-mflib-1.0.0/create_release.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/docs/Makefile` & `fabrictestbed-mflib-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/docs/make.bat` & `fabrictestbed-mflib-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/docs/source/conf.py` & `fabrictestbed-mflib-1.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes.png` & `fabrictestbed-mflib-1.0.0/docs/source/images/3nodes.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes_add_meas.png` & `fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_add_meas.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes_ini.png` & `fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_ini.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/docs/source/images/3nodes_inst.png` & `fabrictestbed-mflib-1.0.0/docs/source/images/3nodes_inst.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/docs/source/images/keys.png` & `fabrictestbed-mflib-1.0.0/docs/source/images/keys.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/docs/source/overview.md` & `fabrictestbed-mflib-1.0.0/docs/source/overview.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/mflib/README.md` & `fabrictestbed-mflib-1.0.0/mflib/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/mflib/__init__.py` & `fabrictestbed-mflib-1.0.0/mflib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
 """
 # release level is a alpha, b beta, rc candidate, dev development, post post,  or f final
 # (major, minor, micro, release level, release build)
-__version_info__ = [0, 2, 0, "b", 0]
+__version_info__ = [1, 0, 0, "f", 0]
 
 __version__ = f"{__version_info__[0]}.{__version_info__[1]}.{__version_info__[2]}"
 
 if __version_info__[3] != 'f':
     __version__ = f"{__version__}{__version_info__[3]}{__version_info__[4]}"
```

### Comparing `fabrictestbed-mflib-0.2.0b0/mflib/core.py` & `fabrictestbed-mflib-1.0.0/mflib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         # The slice object
         self.slice = None
         # The meas_node object
         self._meas_node = None
 
         # The following are normally constant values
         # Name given to the meas node
-        self.measurement_node_name = "_meas_node"
+        self.measurement_node_name = "meas-node"
         # Services directory on meas node
         self.services_directory = os.path.join("/", "home", "mfuser", "services")
         # Base names for keys
         self.mfuser_private_key_filename = "mfuser_private_key"
         self.mfuser_public_key_filename = "mfuser_public_key"
 
     # User Methods
@@ -857,15 +857,15 @@
         # TODO figure out how to name/where to put file locally
         try:
             # local_file_path = os.path.join(self.local_slice_directory, service, filename)
             remote_file_path = os.path.join(self.services_directory, service, filename)
             file_attributes = self.meas_node.download_file(
                 local_file_path, remote_file_path
             )  # , retry=3, retry_interval=10):
-            return {"success": True, "message": "uploaded " + filename + " successfully."}
+            return {"success": True, "filename": local_file_path, "message": "uploaded " + filename + " successfully."}
         except Exception as e:
             self.core_logger.exception()
             return {"success": False, "message": f"Download service file Fail: {e}"}
 
     def _clone_mf_repo(self):
         """
         Clones the MeasurementFramework  git repository to /home/mfuser/mf_git on the meas node.
```

### Comparing `fabrictestbed-mflib-0.2.0b0/mflib/mf_timestamp.py` & `fabrictestbed-mflib-1.0.0/mflib/mf_timestamp.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/mflib/mflib.py` & `fabrictestbed-mflib-1.0.0/mflib/mflib.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,17 @@
                 interfaces[this_site] = []
             this_nodename = node.get_name()
             this_interface = node.add_component(
                 model="NIC_Basic", name=(f"meas_nic_{this_nodename}_{this_site}")
             ).get_interfaces()[0]
             (interfaces[this_site]).append(this_interface)
 
-        meas_nodename = "_meas_node"
+        # Note this is also defined in self.measurement_node_name but we are in a static method
+        meas_nodename = "meas-node" 
+
         meas_image = image
         meas = slice.add_node(name=meas_nodename, site=site)
 
         meas.set_capacities(cores=cores, ram=ram, disk=disk)
         meas.set_image(meas_image)
         if site not in interfaces.keys():
             interfaces[site] = []
@@ -551,16 +553,15 @@
         hosts = []
         mfuser = "mfuser"
         if set_ip:
             msg = f"Configuring Measurement Network..."
             print(msg)
             self.mflib_logger.info(msg)
 
-        meas_nodename = "_meas_node"
-        meas_node = self.slice.get_node(name=meas_nodename)
+        meas_node = self.slice.get_node(name=self.measurement_node_name)
         meas_site = meas_node.get_site()
         meas_network = self.slice.get_network(name=f"l3_meas_net_{meas_site}")
         meas_net_subnet = meas_network.get_subnet()
         networks = self.slice.get_networks()
 
         for network in networks:
             network_name = network.get_name()
@@ -615,15 +616,15 @@
 [workers:children]
 Experiment_Nodes
 """
 
         experiment_nodes = "[Experiment_Nodes]\n"
         e_experiment_nodes = "[workers]\n"
         for host in hosts:
-            if "_meas_node" in host:
+            if self.measurement_node_name in host:
                 hosts_txt += "[Meas_Node]\n"
                 hosts_txt += host + "\n\n"
             else:  # It is an experimenters node
                 experiment_nodes += host + "\n"
 
         hosts_txt += experiment_nodes
         hosts_txt += hosts_tail
@@ -733,31 +734,36 @@
             commands = """
             sudo echo -n "127.0.0.1 " | sudo cat - /etc/hostname  | sudo tee -a /etc/hosts;
             sudo echo -n "2a01:4f9:c010:3f02:64:0:8c52:7103       github.com\n"|sudo tee -a /etc/hosts;
             sudo echo -n "2a01:4f9:c010:3f02:64:0:8c52:7009       codeload.github.com\n"|sudo tee -a /etc/hosts;
             sudo echo -n "2a01:4f9:c010:3f02:64:0:b9c7:6e85       objects.githubusercontent.com\n"|sudo tee -a /etc/hosts;
             sudo echo -n "2600:1fa0:80b4:db49:34d9:6d1e::         ansible-galaxy.s3.amazonaws.com\n"|sudo tee -a /etc/hosts;
             sudo echo -n "2a01:4f9:c010:3f02:64:0:3455:9777       packages.confluent.io\n"|sudo tee -a /etc/hosts;
+            sudo echo -n "2a01:4f9:c010:3f02:64:0:12d7:8a3a	      registry-1.docker.io\n"|sudo tee -a /etc/hosts;
+            sudo echo -n "2a01:4f9:c010:3f02:64:0:12d7:8a3a	      auth.docker.io\n"|sudo tee -a /etc/hosts;
             """
             stdout, stderr = node.execute(commands, quiet=True)
             self.mflib_logger.info(f"STDOUT: {stdout}")
             if stderr:
                 self.mflib_logger.error(f"STDERR: {stderr}")
 
     def restore_DNS(self, node):
         return
 
     def _set_all_hosts_file(self):
         meas_node_meas_net_ip = None
         for interface in self.meas_node.get_interfaces():
-            if "_meas_node-meas_nic" in interface.get_name():
+            if "meas-node-meas_nic" in interface.get_name():
                 meas_node_meas_net_ip = interface.get_ip_addr()
         if meas_node_meas_net_ip:
             execute_threads = {}
-            cmd = f'sudo echo -n "{meas_node_meas_net_ip} {self.measurement_node_name}" | sudo tee -a /etc/hosts;'
+            #cmd = f'sudo echo -n "{meas_node_meas_net_ip} {self.measurement_node_name}" | sudo tee -a /etc/hosts;'
+            #TODO WARNING hardcoded _meas_node name here to match existing docker container needs. Need to update
+            #cmd = f'sudo echo -n "{meas_node_meas_net_ip} _meas_node" | sudo tee -a /etc/hosts;'
+            cmd = f'sudo echo -n "{meas_node_meas_net_ip} {self.measurement_node_name}\n" | sudo tee -a /etc/hosts; sudo echo -n "{meas_node_meas_net_ip} _meas_node\n" | sudo tee -a /etc/hosts;'
             for node in self.slice.get_nodes():
                 execute_threads[node] = node.execute_thread(cmd)
             for node, thread in execute_threads.items():
                 self.mflib_logger.info(
                     f"Waiting for result from node {node.get_name()}"
                 )
                 stdout, stderr = thread.result()
```

### Comparing `fabrictestbed-mflib-0.2.0b0/mflib/mfvis.py` & `fabrictestbed-mflib-1.0.0/mflib/mfvis.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     def get_node_and_interface_names(self):
         """
         Uses fablib to get all the interface names of all the experiment nodes 
         """
         try:
             slice = self.slice
             for node in slice.get_nodes():
-                if node.get_name() != "_meas_node":
+                if node.get_name() != self.measurement_node_name:
                     self.slice_node_info[node.get_name()]=[]
                     os_interface = []
                     interface_matching = {}
                     for interface in node.get_interfaces():
                         os_interface.append(interface.get_os_interface())
                         interface_matching[interface.get_os_interface()]=interface.get_name()
                     self.slice_node_info[node.get_name()].append(os_interface)
```

### Comparing `fabrictestbed-mflib-0.2.0b0/mflib/owl.py` & `fabrictestbed-mflib-1.0.0/mflib/owl.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/mflib/owl_data.py` & `fabrictestbed-mflib-1.0.0/mflib/owl_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         fablib = fablib_manager()
         r = fablib.get_resources()
         
         df = pd.DataFrame(columns = ['node_name', 'site_name', 'lon', 'lat', 'exp_ip'])
         for node in nodes:
             node_name = node.get_name()
             
-            if node_name == "_meas_node":
+            if node_name == "meas-node":
                 pass
             else: 
                 site_name = node.get_site()
                 lat, lon = r.get_location_lat_long(site_name)
                 node_ip = self.list_experiment_ip_addrs(node)[0]
 
                 new_row = pd.DataFrame([{
```

### Comparing `fabrictestbed-mflib-0.2.0b0/pyproject.toml` & `fabrictestbed-mflib-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.2.0b0/PKG-INFO` & `fabrictestbed-mflib-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-mflib
-Version: 0.2.0b0
+Version: 1.0.0
 Summary: FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
 Author: Song, Pinyi, Hussam
 Author-email: Carpenter <csacarp0@g.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

