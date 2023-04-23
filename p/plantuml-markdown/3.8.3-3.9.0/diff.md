# Comparing `tmp/plantuml_markdown-3.8.3-py3-none-any.whl.zip` & `tmp/plantuml_markdown-3.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16756 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    29396 b- defN 23-Apr-12 16:52 plantuml_markdown.py
--rw-rw-r--  2.0 unx     1299 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx    16363 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      515 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/RECORD
-6 files, 47683 bytes uncompressed, 15820 bytes compressed:  66.8%
+Zip file size: 17410 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    30751 b- defN 23-Apr-23 18:07 plantuml_markdown.py
+-rw-rw-r--  2.0 unx     1299 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    17482 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      515 b- defN 23-Apr-23 18:11 plantuml_markdown-3.9.0.dist-info/RECORD
+6 files, 50157 bytes uncompressed, 16474 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: plantuml_markdown.py
 Comment: 
 
-Filename: plantuml_markdown-3.8.3.dist-info/LICENSE
+Filename: plantuml_markdown-3.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: plantuml_markdown-3.8.3.dist-info/METADATA
+Filename: plantuml_markdown-3.9.0.dist-info/METADATA
 Comment: 
 
-Filename: plantuml_markdown-3.8.3.dist-info/WHEEL
+Filename: plantuml_markdown-3.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: plantuml_markdown-3.8.3.dist-info/top_level.txt
+Filename: plantuml_markdown-3.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: plantuml_markdown-3.8.3.dist-info/RECORD
+Filename: plantuml_markdown-3.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## plantuml_markdown.py

```diff
@@ -128,24 +128,26 @@
         self._cachedir: Optional[str] = None
         self._plantuml_server: Optional[str] = None
         self._kroki_server: Optional[str] = None
         self._base_dir: Optional[str] = None
         self._encoding: str = 'utf-8'
         self._http_method: str = 'GET'
         self._fallback_to_get: bool = True
+        self._config_path: Optional[str] = None
 
     def run(self, lines: List[str]) -> List[str]:
         # extract some configurations, to simplify code
         self._cachedir = self.config['cachedir']
         self._plantuml_server = self.config['server']
         self._kroki_server = self.config['kroki_server']
         self._base_dir = self.config['base_dir']
         self._encoding = self.config['encoding'] or self._encoding
         self._http_method = self.config['http_method'].strip()
         self._fallback_to_get = bool(self.config['fallback_to_get'])
+        self._config_path = self.config['config']
 
         text = '\n'.join(lines)
         idx = 0
 
         # loop until all text is parsed
         while idx < len(text):
             text1, idx1 = self._replace_block(text[idx:])
@@ -322,15 +324,15 @@
         img.attrib['alt'] = options['alt']
         img.attrib['title'] = options['title']
 
         if options['id']:
             img.attrib['id'] = options['id']
 
     @staticmethod
-    def _render_error(self, msg: str) -> str:
+    def _render_error(msg: str) -> str:
         return f'<div style="color: red">{msg}</div>'
 
     def _render_diagram(self, code: str, requested_format: str) -> Tuple[Optional[bytes], Optional[str]]:
         cached_diagram_file = None
         diagram = None
 
         if self._cachedir:
@@ -417,18 +419,22 @@
                 code = startuml + "!theme " + theme + "\n" + code_nostartuml
             elif theme_wont_err:
                 # if no @startuml tag found just add it to the beginning
                 code = "\n!theme " + theme + "\n" + code
 
         return code
 
-    @staticmethod
-    def _render_local_uml_image(plantuml_code: str, img_format: str) -> Tuple[Optional[bytes], Optional[str]]:
+    def _render_local_uml_image(self, plantuml_code: str, img_format: str) -> Tuple[Optional[bytes], Optional[str]]:
         plantuml_code = plantuml_code.encode('utf8')
-        cmdline = ['plantuml', '-pipemap' if img_format == 'map' else '-p', "-t" + img_format, '-charset', 'UTF-8']
+        cmdline = self.config['plantuml_cmd'].split(' ')
+        cmdline.extend(['-pipemap' if img_format == 'map' else '-p', "-t" + img_format, '-charset', 'UTF-8'])
+
+        if self._config_path:
+            full_path = os.path.join(self._base_dir, self._config_path) if self._base_dir else self._config_path
+            cmdline.extend(['-config', full_path])
 
         try:
             # On Windows run batch files through a shell so the extension can be resolved
             p = Popen(cmdline, stdin=PIPE, stdout=PIPE, stderr=PIPE, shell=(os.name == 'nt'))
             out, err = p.communicate(input=plantuml_code)
         except Exception as exc:
             raise Exception(f'Failed to run plantuml: {exc}')
@@ -438,14 +444,18 @@
                 logger.error(f'Error in "uml" directive: {err}')
 
             return out, None
 
     def _render_remote_uml_image(
             self, plantuml_code: str, img_format: str, session: requests.Session
         ) -> Tuple[Optional[bytes], Optional[str]]:
+        if self._config_path:
+            # insert an include directive for the config file as the first statement
+            plantuml_code = re.sub(r'^\s*(@start\w+\n)?', r'\1!include '+self._config_path+'\n', plantuml_code)
+
         # build the whole source diagram, executing include directives
         temp_file = PlantUMLIncluder(self._lang, not not self._kroki_server,
                                      self.config['server_include_whitelist'],
                                      False).readFile(plantuml_code, self._base_dir)
 
         # Use GET if preferred, use POST with GET as fallback if POST fails
         if self._http_method == "POST":
@@ -501,21 +511,22 @@
         self._dark_mode = dark_mode
         self._light_theme = light_theme
         self._dark_theme = dark_theme
         self._definitions: Dict[str, str] = {}
         self._lang = lang
         self._kroki = kroki
         self._white_lists = white_lists
+        self._diagram_type = 'uml'
 
     # Given a PlantUML source, replace any "!include" directive with the included code, recursively
     def readFile(self, plantuml_code: str, directory: str) -> str:
         lines = plantuml_code.splitlines()
         # Wrap the whole combined text between startuml and enduml tags as recursive processing would have removed them
         # This is necessary for it to work correctly with plamtuml POST processing
-        return "@startuml\n" + "\n".join(self._readFileRec(lines, directory)) + "\n@enduml\n"
+        return "@start"+self._diagram_type+"\n" + "\n".join(self._readFileRec(lines, directory)) + "\n@end"+self._diagram_type+"\n"
 
     # Reads the file recursively
     def _readFileRec(self, lines: List[str], directory: str) -> List[str]:
         result: List[str] = []
 
         for line in lines:
             line_striped = line.strip()
@@ -529,15 +540,20 @@
 
             if match:
                 # variable definition, save the mapping as the value can be used in !include directives
                 self._definitions[match.group('varname')] = match.group('value')
                 result.append(line)
             elif line_striped.startswith("!include"):
                 result.append(self._readInclLine(line_striped, directory))
-            elif line_striped.startswith("@startuml") or line_striped.startswith("@enduml"):
+            elif line_striped.startswith("@start"):
+                # remove startuml as plantuml POST method doesn't like it in include files
+                # we will wrap the whole combined text between start and end tags at the end
+                self._diagram_type = line_striped[len("@start"):]  # save the type of plantuml diagram
+                continue
+            elif line_striped.startswith("@end"):
                 # remove startuml and enduml tags as plantuml POST method doesn't like it in include files
                 # we will wrap the whole combined text between start and end tags at the end
                 continue
             else:
                 result.append(line)
 
         return result
@@ -598,14 +614,16 @@
     def __init__(self, **kwargs):
         self.config = {
             'classes': ["uml", "Space separated list of classes for the generated image. Defaults to 'uml'."],
             'alt': ["uml diagram", "Text to show when image is not available. Defaults to 'uml diagram'"],
             'format': ["png", "Format of image to generate (png, svg or txt). Defaults to 'png'."],
             'remove_inline_svg_size': [True, "Remove the width and height attributes of inline_svg diagrams", "Defaults to True"],
             'title': ["", "Tooltip for the diagram"],
+            'config': ["", "Path for a PlantUML configuration file (relative to base_dir), included before every "
+                           "diagram", "Defaults to blank, no config file"],
             'server': ["", "PlantUML server url, for remote rendering. Defaults to '', use local command."],
             'kroki_server': ["", "Kroki server url, as alternative to 'server' for remote rendering (image maps must "
                                  "be disabled manually). Defaults to '', use PlantUML server if defined"],
             'server_include_whitelist': [[r'^[Cc]4.*$'],
                                          "List of regular expressions defining which include files are supported by "
                                          "the server. Defaults to [r'^c4.*$']"],
             'insecure': [False, "Disable SSL certificates verification; set to True if you server uses self-signed certificates. Defaults to False"],
@@ -623,15 +641,17 @@
                                      'version', 
                                      'listfonts', 
                                      'stdlib', 
                                      'license'
                                      ], 
                                      "theme will not be set if listed commands present (default list),",
                                      "Defaults to the before mentioned list"
-                                    ]
+                                    ],
+            "plantuml_cmd": ["plantuml", "Command executed when using local plantuml (ex: 'java -Dplantuml.include.path="
+                                         ". -jar plantuml.jar')", "Defaults to 'plantuml'."]
         }
 
         # Fix to make links navigable in SVG diagrams
         etree.register_namespace('xlink', 'http://www.w3.org/1999/xlink')
 
         super(PlantUMLMarkdownExtension, self).__init__(**kwargs)
```

## Comparing `plantuml_markdown-3.8.3.dist-info/LICENSE` & `plantuml_markdown-3.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plantuml_markdown-3.8.3.dist-info/METADATA` & `plantuml_markdown-3.9.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantuml-markdown
-Version: 3.8.3
+Version: 3.9.0
 Summary: A PlantUML plugin for Markdown
 Home-page: https://github.com/mikitex70/plantuml-markdown
 Author: Michele Tessaro
 Author-email: michele.tessaro@email.it
 Keywords: Markdown,typesetting,include,plugin,extension
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -202,14 +202,15 @@
 ```yaml
 plantuml_markdown:
   server: http://www.plantuml.com/plantuml  # PlantUML server, for remote rendering
   # other global options
   insecure: False                           # set to True if the server uses self-signed certificates
   cachedir: /tmp                            # set a non-empty value to enable caching
   base_dir: .                               # where to search for diagrams to include
+  config:                                   # PlantUML config file, relative to base_dir (a PlantUML file included in every diagram)
   format: png                               # default diagram image format
   classes: class1,class2                    # default diagram classes
   encoding: utf-8                           # character encoding for external files (default utf-8)
   title: UML diagram                        # default title (tooltip) for diagram images
   alt: UML diagram image                    # default `alt` attribute for diagram images
   image_maps: True                          # generate image maps when the format is png and there are hyperlinks
   priority: 30                              # plugin priority; the higher, the sooner will be applied (default 30)
@@ -248,39 +249,50 @@
 * otherwise, it is assumed that the file is local and that the `include` statement is replaced with the contents of the 
   file before sending it to the remote server. This behavior can be changed by declaring an appropriate regular
   expression in `server_include_whitelist` or by adding a comment to the line:
     * if the comment begins with `local`, include is forced local; e.g. `!include C4/C4_Container.puml ' local file`
       will search and read the local file `C4/C4_Container.puml`
     * if the comment begins with `remote`, include is treated as a server side include;
       for example `!include my_configuration.puml 'server-side include`
+* includes are resolved recursively, as when used with a local PlantUML.
+
+If using a local PlantUML installation includes works out of the box only if includes are in the current directory. If 
+they are in other directories there are two possibilities:
+* use the directory in includes (ex: `!include includes/my-defs.puml`)
+* set the `base_dir` option in the plugin configuration (ex: `base_dir: includes`) **AND** change the default plantuml
+  command in something like `plantuml_cmd: java -Dplantuml.include.path=includes -jar path/to/plantuml.jar` 
 
 Plugin options
 --------------
 
 The plugin has several configuration option:
 
 * `alt`: text to show when image is not available. Defaults to `uml diagram`
 * `base_dir`: path where to search for external diagrams files
 * `cachedir`: directory for caching of diagrams. Defaults to `''`, no caching
 * `classes`: space separated list of classes for the generated image. Defaults to `uml`
+* `config`: PlantUML config file, relative to `base_dir` (a PlantUML file included before every diagram, see
+  [PlantUML documentation](https://plantuml.com/command-line)). Defaults to `None`
 * `encoding`: character encoding for external files (see `source` parameter); default encoding is `utf-8`. Please note 
   that on Windows text files may use the `cp1252` as default encoding, so setting `encoding: cp1252` may fix incorrect 
   characters rendering.
 * `fallback_to_get`: Fallback to `GET` if `POST` fails. Defaults to True
 * `format`: format of image to generate (`png`, `svg`, `svg_object`, `svg_inline` or `txt`). Defaults to `png` (See 
   example section above for further explanations of the values for `format`)
 * `remove_inline_svg_size`: When `format` is `svg_inline`, remove the `width` and `height` attributes of the generated
-  SVG. Defaults to True
+  SVG. Defaults to `True`
 * `http_method`: Http Method for server - `GET` or `POST`. "Defaults to `GET`
 * `image_maps`: generate image maps if format is `png` and the diagram has hyperlinks; `true`, `on`, `yes` or `1`
-  activates image maps, everything else disables it. Defaults to `true`
+  activates image maps, everything else disables it. Defaults to `True`
 * `insecure`: if `True` do not validate SSL certificate of the PlantUML server; set to `True` when using a custom 
   PlantUML installation with self-signed certificates. Defaults to `False`
 * `kroki_server`: Kroki server url, as alternative to `server` for remote rendering (image maps mus be disabled 
   manually). Defaults to `''`, use PlantUML server if defined
+* `plantuml_cmd`: command to run for executing PlantUML locally; for example, if you need to set the include directory
+  the value can be `java -Dplantuml.include.path=includes -jar plantuml.jar`. Defaults to `plantuml` (the system script)
 * `priority`: extension priority. Higher values means the extension is applied sooner than others. Defaults to `30`
 * `puml_notheme_cmdlist`: theme will not be set if listed commands present. Default list is
   `['version', 'listfonts', 'stdlib', 'license']`. **If modifying please copy the default list provided and append**
 * `server`: PlantUML server url, for remote rendering. Defaults to `''`, use local command
 * `server_include_whitelist`: List of regular expressions defining which include files are supported by the server. 
   Defaults to `[r'^c4.*$']` (all files starting with `c4`). **See [Inclusion Management](#inclusion-management) for 
   details**
```

