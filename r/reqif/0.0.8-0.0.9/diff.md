# Comparing `tmp/reqif-0.0.8.tar.gz` & `tmp/reqif-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqif-0.0.8.tar", last modified: Mon Jan 10 20:02:09 2022, max compression
+gzip compressed data, was "reqif-0.0.9.tar", last modified: Thu Jan 13 19:31:37 2022, max compression
```

## Comparing `reqif-0.0.8.tar` & `reqif-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    11357 2022-01-07 16:58:59.487007 reqif-0.0.8/LICENSE
--rw-r--r--   0        0        0     5469 2022-01-07 16:58:59.487811 reqif-0.0.8/README.md
--rw-r--r--   0        0        0     1198 2022-01-10 20:01:05.781186 reqif-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-14 20:20:04.545461 reqif-0.0.8/reqif/__init__.py
--rw-r--r--   0        0        0        0 2021-12-11 15:37:21.481426 reqif-0.0.8/reqif/cli/__init__.py
--rw-r--r--   0        0        0     5030 2022-01-08 17:07:57.690623 reqif-0.0.8/reqif/cli/cli_arg_parser.py
--rw-r--r--   0        0        0     1642 2022-01-08 17:07:57.691122 reqif-0.0.8/reqif/cli/main.py
--rw-r--r--   0        0        0        0 2022-01-07 16:58:59.491666 reqif-0.0.8/reqif/commands/__init__.py
--rw-r--r--   0        0        0        0 2022-01-08 17:07:57.691243 reqif-0.0.8/reqif/commands/anonymize/__init__.py
--rw-r--r--   0        0        0     3244 2022-01-08 17:07:57.691947 reqif-0.0.8/reqif/commands/anonymize/anonymize.py
--rw-r--r--   0        0        0        0 2022-01-07 16:58:59.492101 reqif-0.0.8/reqif/commands/dump/__init__.py
--rw-r--r--   0        0        0      740 2022-01-07 16:58:59.492724 reqif-0.0.8/reqif/commands/dump/dump.py
--rw-r--r--   0        0        0     3353 2022-01-07 16:58:59.493608 reqif-0.0.8/reqif/commands/dump/templates/index.jinja.html
--rw-r--r--   0        0        0        0 2022-01-07 16:58:59.493764 reqif-0.0.8/reqif/commands/format/__init__.py
--rw-r--r--   0        0        0      438 2022-01-07 16:58:59.496092 reqif-0.0.8/reqif/commands/format/format.py
--rw-r--r--   0        0        0        0 2022-01-07 16:58:59.496227 reqif-0.0.8/reqif/commands/passthrough/__init__.py
--rw-r--r--   0        0        0     1694 2022-01-08 17:07:57.692490 reqif-0.0.8/reqif/commands/passthrough/passthrough.py
--rw-r--r--   0        0        0        0 2022-01-07 16:58:59.497041 reqif-0.0.8/reqif/commands/validate/__init__.py
--rw-r--r--   0        0        0     5829 2022-01-09 20:54:32.491386 reqif-0.0.8/reqif/commands/validate/validate.py
--rw-r--r--   0        0        0        0 2021-12-11 14:11:14.918540 reqif-0.0.8/reqif/helpers/__init__.py
--rw-r--r--   0        0        0      765 2022-01-09 19:46:24.572110 reqif-0.0.8/reqif/helpers/lxml.py
--rw-r--r--   0        0        0        0 2021-11-14 20:20:04.545552 reqif-0.0.8/reqif/models/__init__.py
--rw-r--r--   0        0        0     2141 2022-01-09 20:54:32.491905 reqif-0.0.8/reqif/models/error_handling.py
--rw-r--r--   0        0        0      391 2022-01-07 16:58:59.500475 reqif-0.0.8/reqif/models/reqif_core_content.py
--rw-r--r--   0        0        0     2905 2022-01-08 17:07:57.695647 reqif-0.0.8/reqif/models/reqif_data_type.py
--rw-r--r--   0        0        0     2157 2022-01-08 17:07:57.696613 reqif-0.0.8/reqif/models/reqif_namespace_info.py
--rw-r--r--   0        0        0     1141 2022-01-07 16:58:59.503528 reqif-0.0.8/reqif/models/reqif_req_if_content.py
--rw-r--r--   0        0        0      905 2022-01-07 16:58:59.504027 reqif-0.0.8/reqif/models/reqif_reqif_header.py
--rw-r--r--   0        0        0     2563 2022-01-09 20:54:32.492386 reqif-0.0.8/reqif/models/reqif_spec_hierarchy.py
--rw-r--r--   0        0        0     1948 2022-01-07 16:58:59.505590 reqif-0.0.8/reqif/models/reqif_spec_object.py
--rw-r--r--   0        0        0     3165 2022-01-08 17:07:57.698287 reqif-0.0.8/reqif/models/reqif_spec_object_type.py
--rw-r--r--   0        0        0      961 2022-01-08 19:38:55.833475 reqif-0.0.8/reqif/models/reqif_spec_relation.py
--rw-r--r--   0        0        0      528 2022-01-07 16:58:59.509204 reqif-0.0.8/reqif/models/reqif_spec_relation_type.py
--rw-r--r--   0        0        0     1538 2022-01-09 20:54:32.492968 reqif-0.0.8/reqif/models/reqif_specification.py
--rw-r--r--   0        0        0     1069 2022-01-07 16:58:59.511394 reqif-0.0.8/reqif/models/reqif_specification_type.py
--rw-r--r--   0        0        0      913 2022-01-07 16:58:59.512208 reqif-0.0.8/reqif/models/reqif_types.py
--rw-r--r--   0        0        0     1329 2022-01-09 20:54:51.614986 reqif-0.0.8/reqif/object_lookup.py
--rw-r--r--   0        0        0    11842 2022-01-09 20:54:51.615357 reqif-0.0.8/reqif/parser.py
--rw-r--r--   0        0        0        0 2021-11-14 20:20:04.550711 reqif-0.0.8/reqif/parsers/__init__.py
--rw-r--r--   0        0        0    10136 2022-01-08 17:07:57.701713 reqif-0.0.8/reqif/parsers/data_type_parser.py
--rw-r--r--   0        0        0     4015 2022-01-07 16:58:59.515462 reqif-0.0.8/reqif/parsers/header_parser.py
--rw-r--r--   0        0        0     3997 2022-01-09 20:54:32.493478 reqif-0.0.8/reqif/parsers/spec_hierarchy_parser.py
--rw-r--r--   0        0        0    10355 2022-01-08 17:07:57.703532 reqif-0.0.8/reqif/parsers/spec_object_parser.py
--rw-r--r--   0        0        0     5521 2022-01-08 19:38:55.834562 reqif-0.0.8/reqif/parsers/spec_relation_parser.py
--rw-r--r--   0        0        0    12485 2022-01-08 17:07:57.704818 reqif-0.0.8/reqif/parsers/spec_types/spec_object_type_parser.py
--rw-r--r--   0        0        0     2050 2022-01-07 16:58:59.520120 reqif-0.0.8/reqif/parsers/spec_types/spec_relation_type_parser.py
--rw-r--r--   0        0        0     8409 2022-01-08 17:07:57.705296 reqif-0.0.8/reqif/parsers/spec_types/specification_type_parser.py
--rw-r--r--   0        0        0     7983 2022-01-09 20:54:32.493996 reqif-0.0.8/reqif/parsers/specification_parser.py
--rw-r--r--   0        0        0     2642 2022-01-09 20:54:32.494444 reqif-0.0.8/reqif/reqif_bundle.py
--rw-r--r--   0        0        0      520 2022-01-07 16:58:59.523757 reqif-0.0.8/reqif/specification_iterator.py
--rw-r--r--   0        0        0     6208 2022-01-08 17:07:57.707055 reqif-0.0.8/reqif/unparser.py
--rw-r--r--   0        0        0     6806 2022-01-10 20:02:09.777975 reqif-0.0.8/setup.py
--rw-r--r--   0        0        0     6441 2022-01-10 20:02:09.778839 reqif-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-01-07 16:58:59.487007 reqif-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5483 2022-01-13 19:29:37.633570 reqif-0.0.9/README.md
+-rw-r--r--   0        0        0     1198 2022-01-13 19:29:47.886798 reqif-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-14 20:20:04.545461 reqif-0.0.9/reqif/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-11 15:37:21.481426 reqif-0.0.9/reqif/cli/__init__.py
+-rw-r--r--   0        0        0     5030 2022-01-08 17:07:57.690623 reqif-0.0.9/reqif/cli/cli_arg_parser.py
+-rw-r--r--   0        0        0     1642 2022-01-08 17:07:57.691122 reqif-0.0.9/reqif/cli/main.py
+-rw-r--r--   0        0        0        0 2022-01-07 16:58:59.491666 reqif-0.0.9/reqif/commands/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-08 17:07:57.691243 reqif-0.0.9/reqif/commands/anonymize/__init__.py
+-rw-r--r--   0        0        0     3242 2022-01-13 19:29:37.667358 reqif-0.0.9/reqif/commands/anonymize/anonymize.py
+-rw-r--r--   0        0        0        0 2022-01-07 16:58:59.492101 reqif-0.0.9/reqif/commands/dump/__init__.py
+-rw-r--r--   0        0        0      740 2022-01-07 16:58:59.492724 reqif-0.0.9/reqif/commands/dump/dump.py
+-rw-r--r--   0        0        0     3363 2022-01-13 19:29:37.667510 reqif-0.0.9/reqif/commands/dump/templates/index.jinja.html
+-rw-r--r--   0        0        0        0 2022-01-07 16:58:59.493764 reqif-0.0.9/reqif/commands/format/__init__.py
+-rw-r--r--   0        0        0      438 2022-01-07 16:58:59.496092 reqif-0.0.9/reqif/commands/format/format.py
+-rw-r--r--   0        0        0        0 2022-01-07 16:58:59.496227 reqif-0.0.9/reqif/commands/passthrough/__init__.py
+-rw-r--r--   0        0        0     1694 2022-01-08 17:07:57.692490 reqif-0.0.9/reqif/commands/passthrough/passthrough.py
+-rw-r--r--   0        0        0        0 2022-01-07 16:58:59.497041 reqif-0.0.9/reqif/commands/validate/__init__.py
+-rw-r--r--   0        0        0     5829 2022-01-09 20:54:32.491386 reqif-0.0.9/reqif/commands/validate/validate.py
+-rw-r--r--   0        0        0        0 2021-12-11 14:11:14.918540 reqif-0.0.9/reqif/helpers/__init__.py
+-rw-r--r--   0        0        0      765 2022-01-09 19:46:24.572110 reqif-0.0.9/reqif/helpers/lxml.py
+-rw-r--r--   0        0        0        0 2021-11-14 20:20:04.545552 reqif-0.0.9/reqif/models/__init__.py
+-rw-r--r--   0        0        0     2141 2022-01-09 20:54:32.491905 reqif-0.0.9/reqif/models/error_handling.py
+-rw-r--r--   0        0        0      391 2022-01-07 16:58:59.500475 reqif-0.0.9/reqif/models/reqif_core_content.py
+-rw-r--r--   0        0        0     2905 2022-01-08 17:07:57.695647 reqif-0.0.9/reqif/models/reqif_data_type.py
+-rw-r--r--   0        0        0     2157 2022-01-08 17:07:57.696613 reqif-0.0.9/reqif/models/reqif_namespace_info.py
+-rw-r--r--   0        0        0     1141 2022-01-07 16:58:59.503528 reqif-0.0.9/reqif/models/reqif_req_if_content.py
+-rw-r--r--   0        0        0      905 2022-01-07 16:58:59.504027 reqif-0.0.9/reqif/models/reqif_reqif_header.py
+-rw-r--r--   0        0        0     2563 2022-01-09 20:54:32.492386 reqif-0.0.9/reqif/models/reqif_spec_hierarchy.py
+-rw-r--r--   0        0        0     2274 2022-01-13 19:29:37.667661 reqif-0.0.9/reqif/models/reqif_spec_object.py
+-rw-r--r--   0        0        0     3165 2022-01-08 17:07:57.698287 reqif-0.0.9/reqif/models/reqif_spec_object_type.py
+-rw-r--r--   0        0        0      961 2022-01-08 19:38:55.833475 reqif-0.0.9/reqif/models/reqif_spec_relation.py
+-rw-r--r--   0        0        0      528 2022-01-07 16:58:59.509204 reqif-0.0.9/reqif/models/reqif_spec_relation_type.py
+-rw-r--r--   0        0        0     1538 2022-01-09 20:54:32.492968 reqif-0.0.9/reqif/models/reqif_specification.py
+-rw-r--r--   0        0        0     1069 2022-01-07 16:58:59.511394 reqif-0.0.9/reqif/models/reqif_specification_type.py
+-rw-r--r--   0        0        0      913 2022-01-07 16:58:59.512208 reqif-0.0.9/reqif/models/reqif_types.py
+-rw-r--r--   0        0        0     1329 2022-01-10 20:03:41.105630 reqif-0.0.9/reqif/object_lookup.py
+-rw-r--r--   0        0        0    11842 2022-01-10 20:03:41.105908 reqif-0.0.9/reqif/parser.py
+-rw-r--r--   0        0        0        0 2021-11-14 20:20:04.550711 reqif-0.0.9/reqif/parsers/__init__.py
+-rw-r--r--   0        0        0    10136 2022-01-08 17:07:57.701713 reqif-0.0.9/reqif/parsers/data_type_parser.py
+-rw-r--r--   0        0        0     4015 2022-01-07 16:58:59.515462 reqif-0.0.9/reqif/parsers/header_parser.py
+-rw-r--r--   0        0        0     3997 2022-01-09 20:54:32.493478 reqif-0.0.9/reqif/parsers/spec_hierarchy_parser.py
+-rw-r--r--   0        0        0    10618 2022-01-13 19:29:37.667803 reqif-0.0.9/reqif/parsers/spec_object_parser.py
+-rw-r--r--   0        0        0     5566 2022-01-13 19:29:37.667927 reqif-0.0.9/reqif/parsers/spec_relation_parser.py
+-rw-r--r--   0        0        0    12485 2022-01-08 17:07:57.704818 reqif-0.0.9/reqif/parsers/spec_types/spec_object_type_parser.py
+-rw-r--r--   0        0        0     2050 2022-01-07 16:58:59.520120 reqif-0.0.9/reqif/parsers/spec_types/spec_relation_type_parser.py
+-rw-r--r--   0        0        0     8409 2022-01-08 17:07:57.705296 reqif-0.0.9/reqif/parsers/spec_types/specification_type_parser.py
+-rw-r--r--   0        0        0     8003 2022-01-13 19:29:37.668043 reqif-0.0.9/reqif/parsers/specification_parser.py
+-rw-r--r--   0        0        0     2642 2022-01-09 20:54:32.494444 reqif-0.0.9/reqif/reqif_bundle.py
+-rw-r--r--   0        0        0      520 2022-01-07 16:58:59.523757 reqif-0.0.9/reqif/specification_iterator.py
+-rw-r--r--   0        0        0     6208 2022-01-08 17:07:57.707055 reqif-0.0.9/reqif/unparser.py
+-rw-r--r--   0        0        0     6820 2022-01-13 19:31:37.760136 reqif-0.0.9/setup.py
+-rw-r--r--   0        0        0     6455 2022-01-13 19:31:37.760688 reqif-0.0.9/PKG-INFO
```

### Comparing `reqif-0.0.8/LICENSE` & `reqif-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/README.md` & `reqif-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -143,8 +143,8 @@
 ### [RD01] ReqIF standard
 
 The latest version is 1.2:
 [Requirements Interchange Format](https://www.omg.org/spec/ReqIF)
 
 ### [RD02] ReqIF Implementation Guide 
 
-[ReqIF Implementation Guide](https://www.prostep.org/fileadmin/downloads/PSI_ImplementationGuide_ReqIF_V1-7.pdf)
+[ReqIF Implementation Guide v1.8](https://www.prostep.org/fileadmin/downloads/prostep-ivip_ImplementationGuide_ReqIF_V1-8.pdf)
```

### Comparing `reqif-0.0.8/pyproject.toml` & `reqif-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reqif"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python library for ReqIF format. ReqIF parsing and unparsing."
 authors = ["Stanislav Pankevich <s.pankevich@gmail.com>"]
 maintainers = ["Stanislav Pankevich <s.pankevich@gmail.com>"]
 license = "Apache 2"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/strictdoc-project/reqif"
```

### Comparing `reqif-0.0.8/reqif/cli/cli_arg_parser.py` & `reqif-0.0.9/reqif/cli/cli_arg_parser.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/cli/main.py` & `reqif-0.0.9/reqif/cli/main.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/commands/anonymize/anonymize.py` & `reqif-0.0.9/reqif/commands/anonymize/anonymize.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,11 +73,11 @@
                     AnonymizeCommand._anonymize_attribute(value)
 
     @staticmethod
     def _anonymize_attribute(attribute):
         assert isinstance(attribute, SpecObjectAttribute), f"{attribute}"
         if attribute.attribute_type == SpecObjectAttributeType.STRING:
             attribute.value = ANONYMIZED
-        elif attribute.attribute_type == (SpecObjectAttributeType.XHTML):
+        elif attribute.attribute_type == SpecObjectAttributeType.XHTML:
             attribute.value = (
                 "                " f"<xhtml:div>{ANONYMIZED}</xhtml:div>"
             )
```

### Comparing `reqif-0.0.8/reqif/commands/dump/dump.py` & `reqif-0.0.9/reqif/commands/dump/dump.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/commands/dump/templates/index.jinja.html` & `reqif-0.0.9/reqif/commands/dump/templates/index.jinja.html`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,15 @@
       <tr>
         <td style="text-align: center;" colspan="2">
           &lt;VALUES&gt;
         </td>
       </tr>
     {% for attribute in spec_object.attributes %}
       <tr>
-        <td>{{attribute.name}}</td>
+        <td>{{attribute.definition_ref}}</td>
         <td>{{attribute.value}}</td>
       </tr>
     {% endfor %}
     </table>
   {% endfor %}
 {% endfor %}
```

#### html2text {}

```diff
@@ -32,12 +32,12 @@
 reqif_bundle.core_content.req_if_content %} {% for specification in
 reqif_bundle.core_content.req_if_content.specifications %}
 ****** {{ specification.long_name }} ******
 {% for current_hierarchy in reqif_bundle.iterate_specification_hierarchy
 (specification) %} {% set spec_object = reqif_bundle.get_spec_object_by_ref
 (current_hierarchy.spec_object) %}
 <SPEC-OBJECT>
-<SPEC-OBJECT-TYPE> {{ spec_object.spec_object_type }}
-IDENTIFIER         {{ spec_object.identifier }}
+<SPEC-OBJECT-TYPE>           {{ spec_object.spec_object_type }}
+IDENTIFIER                   {{ spec_object.identifier }}
 <VALUES>
-{{attribute.name}} {{attribute.value}}
+{{attribute.definition_ref}} {{attribute.value}}
 {% endfor %} {% endfor %} {% endif %} {% endif %}
```

### Comparing `reqif-0.0.8/reqif/commands/passthrough/passthrough.py` & `reqif-0.0.9/reqif/commands/passthrough/passthrough.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/commands/validate/validate.py` & `reqif-0.0.9/reqif/commands/validate/validate.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/helpers/lxml.py` & `reqif-0.0.9/reqif/helpers/lxml.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/error_handling.py` & `reqif-0.0.9/reqif/models/error_handling.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_data_type.py` & `reqif-0.0.9/reqif/models/reqif_data_type.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_namespace_info.py` & `reqif-0.0.9/reqif/models/reqif_namespace_info.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_req_if_content.py` & `reqif-0.0.9/reqif/models/reqif_req_if_content.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_reqif_header.py` & `reqif-0.0.9/reqif/models/reqif_reqif_header.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_spec_hierarchy.py` & `reqif-0.0.9/reqif/models/reqif_spec_hierarchy.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_spec_object.py` & `reqif-0.0.9/reqif/models/reqif_spec_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,37 @@
 from reqif.models.reqif_types import SpecObjectAttributeType
 
 
 class SpecObjectAttribute:
     def __init__(
         self,
         attribute_type: SpecObjectAttributeType,
-        name: str,
+        definition_ref: str,
         value: str,
         enum_values_then_definition_order: Optional[bool],
     ):
         self.attribute_type: SpecObjectAttributeType = attribute_type
-        self.name: str = name
+        self.definition_ref: str = definition_ref
         self.value: str = value
         self.enum_values_then_definition_order: Optional[
             bool
         ] = enum_values_then_definition_order
 
+    def __str__(self) -> str:
+        return (
+            f"SpecObjectAttribute("
+            f"attribute_type: {self.attribute_type}"
+            ", "
+            f"definition_ref: {self.definition_ref}"
+            f")"
+        )
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
 
 class ReqIFSpecObject:  # pylint: disable=too-many-instance-attributes
     def __init__(  # pylint: disable=too-many-arguments
         self,
         description: Optional[str],
         identifier: str,
         last_change: Optional[str],
```

### Comparing `reqif-0.0.8/reqif/models/reqif_spec_object_type.py` & `reqif-0.0.9/reqif/models/reqif_spec_object_type.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_spec_relation.py` & `reqif-0.0.9/reqif/models/reqif_spec_relation.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_spec_relation_type.py` & `reqif-0.0.9/reqif/models/reqif_spec_relation_type.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_specification.py` & `reqif-0.0.9/reqif/models/reqif_specification.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_specification_type.py` & `reqif-0.0.9/reqif/models/reqif_specification_type.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/models/reqif_types.py` & `reqif-0.0.9/reqif/models/reqif_types.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/object_lookup.py` & `reqif-0.0.9/reqif/object_lookup.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/parser.py` & `reqif-0.0.9/reqif/parser.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/parsers/data_type_parser.py` & `reqif-0.0.9/reqif/parsers/data_type_parser.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/parsers/header_parser.py` & `reqif-0.0.9/reqif/parsers/header_parser.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/parsers/spec_hierarchy_parser.py` & `reqif-0.0.9/reqif/parsers/spec_hierarchy_parser.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/parsers/spec_object_parser.py` & `reqif-0.0.9/reqif/parsers/spec_object_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,52 +9,52 @@
     SpecObjectAttribute,
     SpecObjectAttributeType,
 )
 
 ATTRIBUTE_STRING_TEMPLATE = """\
             <ATTRIBUTE-VALUE-STRING THE-VALUE="{value}">
               <DEFINITION>
-                <ATTRIBUTE-DEFINITION-STRING-REF>{name}</ATTRIBUTE-DEFINITION-STRING-REF>
+                <ATTRIBUTE-DEFINITION-STRING-REF>{definition_ref}</ATTRIBUTE-DEFINITION-STRING-REF>
               </DEFINITION>
             </ATTRIBUTE-VALUE-STRING>
 """
 
 ATTRIBUTE_INTEGER_TEMPLATE = """\
             <ATTRIBUTE-VALUE-INTEGER THE-VALUE="{value}">
               <DEFINITION>
-                <ATTRIBUTE-DEFINITION-INTEGER-REF>{name}</ATTRIBUTE-DEFINITION-INTEGER-REF>
+                <ATTRIBUTE-DEFINITION-INTEGER-REF>{definition_ref}</ATTRIBUTE-DEFINITION-INTEGER-REF>
               </DEFINITION>
             </ATTRIBUTE-VALUE-INTEGER>
 """
 
 ATTRIBUTE_ENUMERATION_TEMPLATE = """\
             <ATTRIBUTE-VALUE-ENUMERATION>
               <VALUES>
                 <ENUM-VALUE-REF>{value}</ENUM-VALUE-REF>
               </VALUES>
               <DEFINITION>
-                <ATTRIBUTE-DEFINITION-ENUMERATION-REF>{name}</ATTRIBUTE-DEFINITION-ENUMERATION-REF>
+                <ATTRIBUTE-DEFINITION-ENUMERATION-REF>{definition_ref}</ATTRIBUTE-DEFINITION-ENUMERATION-REF>
               </DEFINITION>
             </ATTRIBUTE-VALUE-ENUMERATION>
 """
 ATTRIBUTE_ENUMERATION_TEMPLATE_REVERSE = """\
             <ATTRIBUTE-VALUE-ENUMERATION>
               <DEFINITION>
-                <ATTRIBUTE-DEFINITION-ENUMERATION-REF>{name}</ATTRIBUTE-DEFINITION-ENUMERATION-REF>
+                <ATTRIBUTE-DEFINITION-ENUMERATION-REF>{definition_ref}</ATTRIBUTE-DEFINITION-ENUMERATION-REF>
               </DEFINITION>
               <VALUES>
                 <ENUM-VALUE-REF>{value}</ENUM-VALUE-REF>
               </VALUES>
             </ATTRIBUTE-VALUE-ENUMERATION>
 """
 
 ATTRIBUTE_XHTML_TEMPLATE = """\
             <ATTRIBUTE-VALUE-XHTML>
               <DEFINITION>
-                <ATTRIBUTE-DEFINITION-XHTML-REF>{name}</ATTRIBUTE-DEFINITION-XHTML-REF>
+                <ATTRIBUTE-DEFINITION-XHTML-REF>{definition_ref}</ATTRIBUTE-DEFINITION-XHTML-REF>
               </DEFINITION>
               <THE-VALUE>
 {value}
               </THE-VALUE>
             </ATTRIBUTE-VALUE-XHTML>
 """
 
@@ -240,32 +240,37 @@
     def _unparse_spec_values(spec_object: ReqIFSpecObject):
         output = ""
         output += "          <VALUES>\n"
         for attribute in spec_object.attributes:
             attribute_value = html.escape(attribute.value)
             if attribute.attribute_type == SpecObjectAttributeType.STRING:
                 output += ATTRIBUTE_STRING_TEMPLATE.format(
-                    name=attribute.name, value=attribute_value
+                    definition_ref=attribute.definition_ref,
+                    value=attribute_value,
                 )
             elif attribute.attribute_type == SpecObjectAttributeType.INTEGER:
                 output += ATTRIBUTE_INTEGER_TEMPLATE.format(
-                    name=attribute.name, value=attribute.value
+                    definition_ref=attribute.definition_ref,
+                    value=attribute.value,
                 )
             elif (
                 attribute.attribute_type == SpecObjectAttributeType.ENUMERATION
             ):
                 assert attribute.enum_values_then_definition_order is not None
                 if attribute.enum_values_then_definition_order:
                     output += ATTRIBUTE_ENUMERATION_TEMPLATE.format(
-                        name=attribute.name, value=attribute.value
+                        definition_ref=attribute.definition_ref,
+                        value=attribute.value,
                     )
                 else:
                     output += ATTRIBUTE_ENUMERATION_TEMPLATE_REVERSE.format(
-                        name=attribute.name, value=attribute.value
+                        definition_ref=attribute.definition_ref,
+                        value=attribute.value,
                     )
             elif attribute.attribute_type == SpecObjectAttributeType.XHTML:
                 output += ATTRIBUTE_XHTML_TEMPLATE.format(
-                    name=attribute.name, value=attribute.value
+                    definition_ref=attribute.definition_ref,
+                    value=attribute.value,
                 )
 
         output += "          </VALUES>\n"
         return output
```

### Comparing `reqif-0.0.8/reqif/parsers/spec_relation_parser.py` & `reqif-0.0.9/reqif/parsers/spec_relation_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,16 @@
                     spec_relation
                 )
             elif tag == "VALUES":
                 values_attribute = spec_relation.values_attribute
                 if values_attribute is not None:
                     output += "          <VALUES>\n"
                     output += ATTRIBUTE_STRING_TEMPLATE.format(
-                        name=values_attribute.name, value=values_attribute.value
+                        definition_ref=values_attribute.definition_ref,
+                        value=values_attribute.value,
                     )
                     output += "          </VALUES>\n"
                 else:
                     raise NotImplementedError
             else:
                 raise NotImplementedError(tag)
```

### Comparing `reqif-0.0.8/reqif/parsers/spec_types/spec_object_type_parser.py` & `reqif-0.0.9/reqif/parsers/spec_types/spec_object_type_parser.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/parsers/spec_types/spec_relation_type_parser.py` & `reqif-0.0.9/reqif/parsers/spec_types/spec_relation_type_parser.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/parsers/spec_types/specification_type_parser.py` & `reqif-0.0.9/reqif/parsers/spec_types/specification_type_parser.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/parsers/specification_parser.py` & `reqif-0.0.9/reqif/parsers/specification_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
                         output += "          <VALUES>\n"
                         for xml_attribute in xml_values_attributes:
                             if (
                                 xml_attribute.attribute_type
                                 == SpecObjectAttributeType.XHTML
                             ):
                                 output += ATTRIBUTE_XHTML_TEMPLATE.format(
-                                    name=xml_attribute.name,
+                                    definition_ref=xml_attribute.definition_ref,
                                     value=xml_attribute.value,
                                 )
                             else:
                                 raise NotImplementedError
                         output += "          </VALUES>\n"
                 else:
                     raise NotImplementedError
```

### Comparing `reqif-0.0.8/reqif/reqif_bundle.py` & `reqif-0.0.9/reqif/reqif_bundle.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/specification_iterator.py` & `reqif-0.0.9/reqif/specification_iterator.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/reqif/unparser.py` & `reqif-0.0.9/reqif/unparser.py`

 * *Files identical despite different names*

### Comparing `reqif-0.0.8/setup.py` & `reqif-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 ['beautifulsoup4>=4.9.3,<5.0.0', 'jinja2>=2.11.2,<3.0.0', 'lxml>=4.6.2,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['reqif = reqif.cli.main:main']}
 
 setup_kwargs = {
     'name': 'reqif',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Python library for ReqIF format. ReqIF parsing and unparsing.',
-    'long_description': '# ReqIF\n\nReqIF is a Python library for working with ReqIF format.\n\n**The project is under construction.**\n\n## Supported features\n\n- Parsing/unparsing ReqIF\n- Formatting (pretty-printing) ReqIF\n\nTo be implemented:\n\n- Validating ReqIF\n- Converting from/to Excel and other formats\n\n## Getting started\n\n```bash\npip install reqif\n```\n\n## Using ReqIF as a library\n\n### Parsing ReqIF\n\n```py\nreqif_bundle = ReqIFParser.parse(input_file_path)\nfor specification in reqif_bundle.core_content.req_if_content.specifications\n    print(specification.long_name)\n\n    for current_hierarchy in reqif_bundle.iterate_specification_hierarchy(specification):\n        print(current_hierarchy)\n```\n\n### Unparsing ReqIF\n\n```py\nreqif_bundle = ReqIFParser.parse(input_file_path)\nreqif_xml_output = ReqIFUnparser.unparse(reqif_bundle)\nwith open(output_file_path, "w", encoding="UTF-8") as output_file:\n    output_file.write(reqif_xml_output)\n```\n\nThe contents of `reqif_xml_output` should be the same as the contents of the \n`input_file`.\n\n## Using ReqIF as a command-line tool\n\n### Passthrough command\n\nBefore using the ReqIF library, it is useful to check if it fully understands a\nparticular ReqIF file format that a user has in hand. The `passthrough` command\nfirst parses the ReqIF XML into in-memory Python objects and then unparses\nthese Python objects back to an output ReqIF file.\n\nIf everything goes fine, the output of the passthrough command should be\nidentical to the contents of the input file.\n\n`tests/integration/examples` contains samples of ReqIF files found on the \ninternet. The integration tests ensure that for these samples, the passthrough\ncommand always produces outputs that are identical to inputs. \n\n### Formatting ReqIF\n\nThe `format` command is similar to `clang-format` for C/C++ files or \n`cmake-format` for CMake files. The input file is parsed and then pretty-printed\nback to an output file.\n\nThis command is useful when dealing with ReqIF files that are hand-written or\nReqIF files produced by the ReqIF tools that do not generate a well-formed XML\nwith consistent indentation.  \n\nThe `tests/integration/commands/format` contains typical examples of\nincorrectly formatted ReqIF files. The integration tests ensure that the\n`format` command fixes these issues.\n\n## Implementation details\n\nThe core of the library is a **ReqIF first-stage parser** that only transforms\nthe contents of a ReqIF XML file into a ReqIF in-memory representation. The\nin-memory representation is a tree of Python objects that map directly to the \nobjects of the ReqIF XML file structure (e.g, Spec Objects, Spec Types, Data\nTypes, Specifications, etc.).\n\n### Parsing: Converting from ReqIF to other formats\n\nThe first-stage parser (implemented by the class `ReqIFParser`) can be used by\nuser\'s second-stage parser/converter scripts that convert the ReqIF in-memory\nstructure into a desired format such as Excel, HTML or other formats. The\ntwo-stage process allows the first stage parsing to focus solely on creating an\nin-memory ReqIF object tree, while the second stage parsing can further parse\nthe ReqIF object tree according to the logical structure of user\'s documents as\nencoded in the ReqIF XML file that was produced by user\'s requirements\nmanagement tool.\n\n### Unparsing: Converting from other formats to ReqIF\n\nThe reverse process is also possible. A user\'s script converts another format\'s\ncontents into a ReqIF in-memory representation. The ReqIF un-parser\n(implemented by the class `ReqIFUnparser`) can be used to render the in-memory\nobjects to the ReqIF XML file.\n\n### Tolerance\n\nThe first-stage parser is made tolerant against possible issues in ReqIF.\nIt should be possible to parse a ReqIF file even if it is missing important\ninformation. A separate validation command shall be used to confirm the validity\nof the ReqIF contents.\n\n### A bottom-up overview of the ReqIF format\n\n- ReqIF is a standard. See reference document [RD01](#rd01-reqif-standard).\n- ReqIF has a fixed structure (see "What is common for all ReqIF documents" \nbelow)\n- ReqIF standard does not define a document structure for every documents so\na ReqIF tool implementor is free to choose between several implementation \napproaches. There is a\n[ReqIF Implementation Guide](#rd02-reqif-implementation-guide)\nthat attempts to harmonize ReqIF tool developments. See also\n"What is left open by the ReqIF standard" below.\n- ReqIF files produced by various tool often have incomplete schemas. \n\n### What is common for all ReqIF documents\n\n- All documents have ReqIF tags:\n  - Document metadata is stored inside tags of `REQ-IF-HEADER` tag.\n  - Requirements are stored as `<SPEC-OBJECT>`s\n  - Requirements types are stored as `<SPEC-TYPE>`s\n  - Supported data types are stored as `<DATATYPE>`\n  - Relationships such as \'Parent-Child\' as stored as `<SPEC-RELATIONS>`\n\n### What is left open by the ReqIF standard\n \n- How to distinguish requirements from headers/sections?\n  - One way: create separate `SPEC-TYPES`: one or more for requirements and\n    one for sections.\n  - Another way: have one spec type but have it provide a `TYPE` field that can\n  be used to distinguish between `REQUIREMENT` or `SECTION`.\n\n## Reference documents\n\n### [RD01] ReqIF standard\n\nThe latest version is 1.2:\n[Requirements Interchange Format](https://www.omg.org/spec/ReqIF)\n\n### [RD02] ReqIF Implementation Guide \n\n[ReqIF Implementation Guide](https://www.prostep.org/fileadmin/downloads/PSI_ImplementationGuide_ReqIF_V1-7.pdf)\n',
+    'long_description': '# ReqIF\n\nReqIF is a Python library for working with ReqIF format.\n\n**The project is under construction.**\n\n## Supported features\n\n- Parsing/unparsing ReqIF\n- Formatting (pretty-printing) ReqIF\n\nTo be implemented:\n\n- Validating ReqIF\n- Converting from/to Excel and other formats\n\n## Getting started\n\n```bash\npip install reqif\n```\n\n## Using ReqIF as a library\n\n### Parsing ReqIF\n\n```py\nreqif_bundle = ReqIFParser.parse(input_file_path)\nfor specification in reqif_bundle.core_content.req_if_content.specifications\n    print(specification.long_name)\n\n    for current_hierarchy in reqif_bundle.iterate_specification_hierarchy(specification):\n        print(current_hierarchy)\n```\n\n### Unparsing ReqIF\n\n```py\nreqif_bundle = ReqIFParser.parse(input_file_path)\nreqif_xml_output = ReqIFUnparser.unparse(reqif_bundle)\nwith open(output_file_path, "w", encoding="UTF-8") as output_file:\n    output_file.write(reqif_xml_output)\n```\n\nThe contents of `reqif_xml_output` should be the same as the contents of the \n`input_file`.\n\n## Using ReqIF as a command-line tool\n\n### Passthrough command\n\nBefore using the ReqIF library, it is useful to check if it fully understands a\nparticular ReqIF file format that a user has in hand. The `passthrough` command\nfirst parses the ReqIF XML into in-memory Python objects and then unparses\nthese Python objects back to an output ReqIF file.\n\nIf everything goes fine, the output of the passthrough command should be\nidentical to the contents of the input file.\n\n`tests/integration/examples` contains samples of ReqIF files found on the \ninternet. The integration tests ensure that for these samples, the passthrough\ncommand always produces outputs that are identical to inputs. \n\n### Formatting ReqIF\n\nThe `format` command is similar to `clang-format` for C/C++ files or \n`cmake-format` for CMake files. The input file is parsed and then pretty-printed\nback to an output file.\n\nThis command is useful when dealing with ReqIF files that are hand-written or\nReqIF files produced by the ReqIF tools that do not generate a well-formed XML\nwith consistent indentation.  \n\nThe `tests/integration/commands/format` contains typical examples of\nincorrectly formatted ReqIF files. The integration tests ensure that the\n`format` command fixes these issues.\n\n## Implementation details\n\nThe core of the library is a **ReqIF first-stage parser** that only transforms\nthe contents of a ReqIF XML file into a ReqIF in-memory representation. The\nin-memory representation is a tree of Python objects that map directly to the \nobjects of the ReqIF XML file structure (e.g, Spec Objects, Spec Types, Data\nTypes, Specifications, etc.).\n\n### Parsing: Converting from ReqIF to other formats\n\nThe first-stage parser (implemented by the class `ReqIFParser`) can be used by\nuser\'s second-stage parser/converter scripts that convert the ReqIF in-memory\nstructure into a desired format such as Excel, HTML or other formats. The\ntwo-stage process allows the first stage parsing to focus solely on creating an\nin-memory ReqIF object tree, while the second stage parsing can further parse\nthe ReqIF object tree according to the logical structure of user\'s documents as\nencoded in the ReqIF XML file that was produced by user\'s requirements\nmanagement tool.\n\n### Unparsing: Converting from other formats to ReqIF\n\nThe reverse process is also possible. A user\'s script converts another format\'s\ncontents into a ReqIF in-memory representation. The ReqIF un-parser\n(implemented by the class `ReqIFUnparser`) can be used to render the in-memory\nobjects to the ReqIF XML file.\n\n### Tolerance\n\nThe first-stage parser is made tolerant against possible issues in ReqIF.\nIt should be possible to parse a ReqIF file even if it is missing important\ninformation. A separate validation command shall be used to confirm the validity\nof the ReqIF contents.\n\n### A bottom-up overview of the ReqIF format\n\n- ReqIF is a standard. See reference document [RD01](#rd01-reqif-standard).\n- ReqIF has a fixed structure (see "What is common for all ReqIF documents" \nbelow)\n- ReqIF standard does not define a document structure for every documents so\na ReqIF tool implementor is free to choose between several implementation \napproaches. There is a\n[ReqIF Implementation Guide](#rd02-reqif-implementation-guide)\nthat attempts to harmonize ReqIF tool developments. See also\n"What is left open by the ReqIF standard" below.\n- ReqIF files produced by various tool often have incomplete schemas. \n\n### What is common for all ReqIF documents\n\n- All documents have ReqIF tags:\n  - Document metadata is stored inside tags of `REQ-IF-HEADER` tag.\n  - Requirements are stored as `<SPEC-OBJECT>`s\n  - Requirements types are stored as `<SPEC-TYPE>`s\n  - Supported data types are stored as `<DATATYPE>`\n  - Relationships such as \'Parent-Child\' as stored as `<SPEC-RELATIONS>`\n\n### What is left open by the ReqIF standard\n \n- How to distinguish requirements from headers/sections?\n  - One way: create separate `SPEC-TYPES`: one or more for requirements and\n    one for sections.\n  - Another way: have one spec type but have it provide a `TYPE` field that can\n  be used to distinguish between `REQUIREMENT` or `SECTION`.\n\n## Reference documents\n\n### [RD01] ReqIF standard\n\nThe latest version is 1.2:\n[Requirements Interchange Format](https://www.omg.org/spec/ReqIF)\n\n### [RD02] ReqIF Implementation Guide \n\n[ReqIF Implementation Guide v1.8](https://www.prostep.org/fileadmin/downloads/prostep-ivip_ImplementationGuide_ReqIF_V1-8.pdf)\n',
     'author': 'Stanislav Pankevich',
     'author_email': 's.pankevich@gmail.com',
     'maintainer': 'Stanislav Pankevich',
     'maintainer_email': 's.pankevich@gmail.com',
     'url': 'https://github.com/strictdoc-project/reqif',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `reqif-0.0.8/PKG-INFO` & `reqif-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reqif
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python library for ReqIF format. ReqIF parsing and unparsing.
 Home-page: https://github.com/strictdoc-project/reqif
 License: Apache 2
 Keywords: ReqIF,Requirements,Requirements management
 Author: Stanislav Pankevich
 Author-email: s.pankevich@gmail.com
 Maintainer: Stanislav Pankevich
@@ -167,9 +167,9 @@
 ### [RD01] ReqIF standard
 
 The latest version is 1.2:
 [Requirements Interchange Format](https://www.omg.org/spec/ReqIF)
 
 ### [RD02] ReqIF Implementation Guide 
 
-[ReqIF Implementation Guide](https://www.prostep.org/fileadmin/downloads/PSI_ImplementationGuide_ReqIF_V1-7.pdf)
+[ReqIF Implementation Guide v1.8](https://www.prostep.org/fileadmin/downloads/prostep-ivip_ImplementationGuide_ReqIF_V1-8.pdf)
```

