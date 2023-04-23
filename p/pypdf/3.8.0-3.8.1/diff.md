# Comparing `tmp/pypdf-3.8.0.tar.gz` & `tmp/pypdf-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdf-3.8.0.tar", last modified: Sun Apr 16 19:18:29 2023, max compression
+gzip compressed data, was "pypdf-3.8.1.tar", last modified: Sun Apr 23 13:16:27 2023, max compression
```

## Comparing `pypdf-3.8.0.tar` & `pypdf-3.8.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      488 2022-12-10 23:30:58.176669 pypdf-3.8.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      542 2023-03-29 15:43:03.262713 pypdf-3.8.0/.readthedocs.yaml
--rw-r--r--   0        0        0    35126 2023-04-16 19:18:25.439058 pypdf-3.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     3475 2023-04-16 09:09:24.301502 pypdf-3.8.0/CONTRIBUTORS.md
--rw-r--r--   0        0        0     1605 2022-12-10 23:30:58.184669 pypdf-3.8.0/LICENSE
--rw-r--r--   0        0        0       34 2022-12-10 23:30:58.184669 pypdf-3.8.0/MANIFEST.in
--rw-r--r--   0        0        0     4729 2023-04-09 16:59:02.663368 pypdf-3.8.0/README.md
--rw-r--r--   0        0        0     1234 2023-03-04 08:55:07.145847 pypdf-3.8.0/pypdf/__init__.py
--rw-r--r--   0        0        0    14962 2023-04-16 09:09:24.301502 pypdf-3.8.0/pypdf/_cmap.py
--rw-r--r--   0        0        0     1674 2023-02-28 08:12:53.909178 pypdf-3.8.0/pypdf/_codecs/__init__.py
--rw-r--r--   0        0        0   431492 2022-12-31 10:47:18.999493 pypdf-3.8.0/pypdf/_codecs/adobe_glyphs.py
--rw-r--r--   0        0        0     4269 2022-12-31 10:47:18.999493 pypdf-3.8.0/pypdf/_codecs/pdfdoc.py
--rw-r--r--   0        0        0     2630 2023-02-28 08:12:53.909178 pypdf-3.8.0/pypdf/_codecs/std.py
--rw-r--r--   0        0        0     3734 2022-12-31 10:47:18.999493 pypdf-3.8.0/pypdf/_codecs/symbol.py
--rw-r--r--   0        0        0     3742 2022-12-31 10:47:18.999493 pypdf-3.8.0/pypdf/_codecs/zapfding.py
--rw-r--r--   0        0        0    45635 2023-03-31 16:21:44.806544 pypdf-3.8.0/pypdf/_encryption.py
--rw-r--r--   0        0        0    30706 2023-04-16 16:12:02.507479 pypdf-3.8.0/pypdf/_merger.py
--rw-r--r--   0        0        0    82921 2023-04-16 09:09:24.305502 pypdf-3.8.0/pypdf/_page.py
--rw-r--r--   0        0        0     7186 2023-03-04 08:55:07.145847 pypdf-3.8.0/pypdf/_page_labels.py
--rw-r--r--   0        0        0     1920 2023-04-08 20:27:58.305582 pypdf-3.8.0/pypdf/_protocols.py
--rw-r--r--   0        0        0    86085 2023-04-16 09:09:24.305502 pypdf-3.8.0/pypdf/_reader.py
--rw-r--r--   0        0        0    12788 2023-03-31 16:21:44.806544 pypdf-3.8.0/pypdf/_security.py
--rw-r--r--   0        0        0    10008 2023-03-12 09:43:33.014879 pypdf-3.8.0/pypdf/_text_extraction/__init__.py
--rw-r--r--   0        0        0    14912 2023-04-16 12:58:54.105217 pypdf-3.8.0/pypdf/_utils.py
--rw-r--r--   0        0        0       22 2023-04-16 19:17:18.914887 pypdf-3.8.0/pypdf/_version.py
--rw-r--r--   0        0        0   122863 2023-04-16 09:09:24.305502 pypdf-3.8.0/pypdf/_writer.py
--rw-r--r--   0        0        0    16147 2023-04-09 16:59:02.667368 pypdf-3.8.0/pypdf/constants.py
--rw-r--r--   0        0        0     1631 2023-03-04 08:55:07.149847 pypdf-3.8.0/pypdf/errors.py
--rw-r--r--   0        0        0    25921 2023-04-09 16:59:02.667368 pypdf-3.8.0/pypdf/filters.py
--rw-r--r--   0        0        0     4549 2023-04-09 16:59:02.667368 pypdf-3.8.0/pypdf/generic/__init__.py
--rw-r--r--   0        0        0    17368 2023-04-08 20:27:58.309582 pypdf-3.8.0/pypdf/generic/_annotations.py
--rw-r--r--   0        0        0    24854 2023-04-08 20:27:58.309582 pypdf-3.8.0/pypdf/generic/_base.py
--rw-r--r--   0        0        0    54890 2023-04-10 07:47:24.160491 pypdf-3.8.0/pypdf/generic/_data_structures.py
--rw-r--r--   0        0        0     5427 2023-03-04 08:55:07.149847 pypdf-3.8.0/pypdf/generic/_fit.py
--rw-r--r--   0        0        0     1195 2023-02-28 08:19:03.524706 pypdf-3.8.0/pypdf/generic/_outline.py
--rw-r--r--   0        0        0     8826 2023-03-04 08:55:07.149847 pypdf-3.8.0/pypdf/generic/_rectangle.py
--rw-r--r--   0        0        0     6405 2023-03-04 11:49:14.882511 pypdf-3.8.0/pypdf/generic/_utils.py
--rw-r--r--   0        0        0     6880 2023-03-04 08:55:07.153847 pypdf-3.8.0/pypdf/pagerange.py
--rw-r--r--   0        0        0     1369 2023-02-28 08:12:53.917178 pypdf-3.8.0/pypdf/papersizes.py
--rw-r--r--   0        0        0        0 2022-12-31 10:47:19.003493 pypdf-3.8.0/pypdf/py.typed
--rw-r--r--   0        0        0     2135 2023-03-29 15:43:03.266713 pypdf-3.8.0/pypdf/types.py
--rw-r--r--   0        0        0    17879 2023-03-29 15:43:03.266713 pypdf-3.8.0/pypdf/xmp.py
--rw-r--r--   0        0        0     7425 2023-04-10 18:00:48.219069 pypdf-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     1585 2023-02-05 10:26:02.030123 pypdf-3.8.0/setup.cfg
--rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 pypdf-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0      488 2022-12-10 23:30:58.176669 pypdf-3.8.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      542 2023-03-29 15:43:03.262713 pypdf-3.8.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    35415 2023-04-23 13:15:09.398338 pypdf-3.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3475 2023-04-19 17:12:20.725394 pypdf-3.8.1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     1605 2022-12-10 23:30:58.184669 pypdf-3.8.1/LICENSE
+-rw-r--r--   0        0        0       34 2022-12-10 23:30:58.184669 pypdf-3.8.1/MANIFEST.in
+-rw-r--r--   0        0        0     4729 2023-04-09 16:59:02.663368 pypdf-3.8.1/README.md
+-rw-r--r--   0        0        0     1234 2023-03-04 08:55:07.145847 pypdf-3.8.1/pypdf/__init__.py
+-rw-r--r--   0        0        0    14962 2023-04-19 17:12:20.725394 pypdf-3.8.1/pypdf/_cmap.py
+-rw-r--r--   0        0        0     1674 2023-02-28 08:12:53.909178 pypdf-3.8.1/pypdf/_codecs/__init__.py
+-rw-r--r--   0        0        0   431492 2022-12-31 10:47:18.999493 pypdf-3.8.1/pypdf/_codecs/adobe_glyphs.py
+-rw-r--r--   0        0        0     4269 2022-12-31 10:47:18.999493 pypdf-3.8.1/pypdf/_codecs/pdfdoc.py
+-rw-r--r--   0        0        0     2630 2023-02-28 08:12:53.909178 pypdf-3.8.1/pypdf/_codecs/std.py
+-rw-r--r--   0        0        0     3734 2022-12-31 10:47:18.999493 pypdf-3.8.1/pypdf/_codecs/symbol.py
+-rw-r--r--   0        0        0     3742 2022-12-31 10:47:18.999493 pypdf-3.8.1/pypdf/_codecs/zapfding.py
+-rw-r--r--   0        0        0    45635 2023-03-31 16:21:44.806544 pypdf-3.8.1/pypdf/_encryption.py
+-rw-r--r--   0        0        0    30706 2023-04-19 17:12:20.725394 pypdf-3.8.1/pypdf/_merger.py
+-rw-r--r--   0        0        0    82921 2023-04-19 17:12:20.725394 pypdf-3.8.1/pypdf/_page.py
+-rw-r--r--   0        0        0     7186 2023-03-04 08:55:07.145847 pypdf-3.8.1/pypdf/_page_labels.py
+-rw-r--r--   0        0        0     1920 2023-04-08 20:27:58.305582 pypdf-3.8.1/pypdf/_protocols.py
+-rw-r--r--   0        0        0    86085 2023-04-19 17:12:20.729394 pypdf-3.8.1/pypdf/_reader.py
+-rw-r--r--   0        0        0    12788 2023-03-31 16:21:44.806544 pypdf-3.8.1/pypdf/_security.py
+-rw-r--r--   0        0        0    10008 2023-03-12 09:43:33.014879 pypdf-3.8.1/pypdf/_text_extraction/__init__.py
+-rw-r--r--   0        0        0    14912 2023-04-19 17:12:20.729394 pypdf-3.8.1/pypdf/_utils.py
+-rw-r--r--   0        0        0       22 2023-04-23 13:15:29.250513 pypdf-3.8.1/pypdf/_version.py
+-rw-r--r--   0        0        0   124121 2023-04-22 10:52:03.820548 pypdf-3.8.1/pypdf/_writer.py
+-rw-r--r--   0        0        0    16147 2023-04-09 16:59:02.667368 pypdf-3.8.1/pypdf/constants.py
+-rw-r--r--   0        0        0     1631 2023-03-04 08:55:07.149847 pypdf-3.8.1/pypdf/errors.py
+-rw-r--r--   0        0        0    26830 2023-04-19 17:12:20.729394 pypdf-3.8.1/pypdf/filters.py
+-rw-r--r--   0        0        0     4549 2023-04-09 16:59:02.667368 pypdf-3.8.1/pypdf/generic/__init__.py
+-rw-r--r--   0        0        0    17368 2023-04-08 20:27:58.309582 pypdf-3.8.1/pypdf/generic/_annotations.py
+-rw-r--r--   0        0        0    24854 2023-04-08 20:27:58.309582 pypdf-3.8.1/pypdf/generic/_base.py
+-rw-r--r--   0        0        0    54890 2023-04-10 07:47:24.160491 pypdf-3.8.1/pypdf/generic/_data_structures.py
+-rw-r--r--   0        0        0     5427 2023-03-04 08:55:07.149847 pypdf-3.8.1/pypdf/generic/_fit.py
+-rw-r--r--   0        0        0     1195 2023-02-28 08:19:03.524706 pypdf-3.8.1/pypdf/generic/_outline.py
+-rw-r--r--   0        0        0     8826 2023-03-04 08:55:07.149847 pypdf-3.8.1/pypdf/generic/_rectangle.py
+-rw-r--r--   0        0        0     6405 2023-03-04 11:49:14.882511 pypdf-3.8.1/pypdf/generic/_utils.py
+-rw-r--r--   0        0        0     6880 2023-03-04 08:55:07.153847 pypdf-3.8.1/pypdf/pagerange.py
+-rw-r--r--   0        0        0     1369 2023-02-28 08:12:53.917178 pypdf-3.8.1/pypdf/papersizes.py
+-rw-r--r--   0        0        0        0 2022-12-31 10:47:19.003493 pypdf-3.8.1/pypdf/py.typed
+-rw-r--r--   0        0        0     2135 2023-03-29 15:43:03.266713 pypdf-3.8.1/pypdf/types.py
+-rw-r--r--   0        0        0    17879 2023-03-29 15:43:03.266713 pypdf-3.8.1/pypdf/xmp.py
+-rw-r--r--   0        0        0     7425 2023-04-10 18:00:48.219069 pypdf-3.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1585 2023-02-05 10:26:02.030123 pypdf-3.8.1/setup.cfg
+-rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 pypdf-3.8.1/PKG-INFO
```

### Comparing `pypdf-3.8.0/.readthedocs.yaml` & `pypdf-3.8.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/CHANGELOG.md` & `pypdf-3.8.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 # CHANGELOG
 
-## Version 3.7.2, 2023-04-16
+## Version 3.8.1, 2023-04-23
+
+### Bug Fixes (BUG)
+-  Convert color space before saving (#1802)
+
+### Documentation (DOC)
+-  PDF/A (#1807)
+-  Use append instead of add_page
+-  Document core mechanics of pypdf (#1783)
+
+[Full Changelog](https://github.com/py-pdf/pypdf/compare/3.8.0...3.8.1)
+
+## Version 3.8.0, 2023-04-16
 
 ### New Features (ENH)
 -  Add transform method to Transformation class (#1765)
 -  Cope with UC2 fonts in text_extraction (#1785)
 
 ### Robustness (ROB)
 -  Invalid startxref pointing 1 char before (#1784)
 
 ### Maintenance (MAINT)
 -  Mark code handling old parameters as deprecated (#1798)
 
-[Full Changelog](https://github.com/py-pdf/pypdf/compare/3.7.1...3.7.2)
+[Full Changelog](https://github.com/py-pdf/pypdf/compare/3.7.1...3.8.0)
 
 
 ## Version 3.7.1, 2023-04-09
 
 ### Security (SEC)
 -  Warn about PDF encryption security (#1755)
```

### Comparing `pypdf-3.8.0/CONTRIBUTORS.md` & `pypdf-3.8.1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/LICENSE` & `pypdf-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/README.md` & `pypdf-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/__init__.py` & `pypdf-3.8.1/pypdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_cmap.py` & `pypdf-3.8.1/pypdf/_cmap.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_codecs/__init__.py` & `pypdf-3.8.1/pypdf/_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_codecs/adobe_glyphs.py` & `pypdf-3.8.1/pypdf/_codecs/adobe_glyphs.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_codecs/pdfdoc.py` & `pypdf-3.8.1/pypdf/_codecs/pdfdoc.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_codecs/std.py` & `pypdf-3.8.1/pypdf/_codecs/std.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_codecs/symbol.py` & `pypdf-3.8.1/pypdf/_codecs/symbol.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_codecs/zapfding.py` & `pypdf-3.8.1/pypdf/_codecs/zapfding.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_encryption.py` & `pypdf-3.8.1/pypdf/_encryption.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_merger.py` & `pypdf-3.8.1/pypdf/_merger.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_page.py` & `pypdf-3.8.1/pypdf/_page.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_page_labels.py` & `pypdf-3.8.1/pypdf/_page_labels.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_protocols.py` & `pypdf-3.8.1/pypdf/_protocols.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_reader.py` & `pypdf-3.8.1/pypdf/_reader.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_security.py` & `pypdf-3.8.1/pypdf/_security.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_text_extraction/__init__.py` & `pypdf-3.8.1/pypdf/_text_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_utils.py` & `pypdf-3.8.1/pypdf/_utils.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/_writer.py` & `pypdf-3.8.1/pypdf/_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,21 @@
 
     def __init__(
         self,
         fileobj: StrByteType = "",
         clone_from: Union[None, PdfReader, StrByteType, Path] = None,
     ) -> None:
         self._header = b"%PDF-1.3"
-        self._objects: List[PdfObject] = []  # array of indirect objects
+
+        self._objects: List[PdfObject] = []
+        """The indirect objects in the PDF."""
+
         self._idnum_hash: Dict[bytes, IndirectObject] = {}
+        """Maps hash values of indirect objects to their IndirectObject instances."""
+
         self._id_translated: Dict[int, Dict[int, int]] = {}
 
         # The root of our page tree node.
         pages = DictionaryObject()
         pages.update(
             {
                 NameObject(PA.TYPE): NameObject("/Pages"),
@@ -194,14 +199,15 @@
         self._root_object.update(
             {
                 NameObject(PA.TYPE): NameObject(CO.CATALOG),
                 NameObject(CO.PAGES): self._pages,
             }
         )
         self._root = self._add_object(self._root_object)
+
         if clone_from is not None:
             if not isinstance(clone_from, PdfReader):
                 clone_from = PdfReader(clone_from)
             self.clone_document_from_reader(clone_from)
         self.fileobj = fileobj
         self.with_as_usage = False
 
@@ -1131,28 +1137,19 @@
                 "It may not be written to correctly.",
                 __name__,
             )
 
         if not self._root:
             self._root = self._add_object(self._root_object)
 
-        # PDF objects sometimes have circular references to their /Page objects
-        # inside their object tree (for example, annotations).  Those will be
-        # indirect references to objects that we've recreated in this PDF.  To
-        # address this problem, PageObject's store their original object
-        # reference number, and we add it to the external reference map before
-        # we sweep for indirect references.  This forces self-page-referencing
-        # trees to reference the correct new object location, rather than
-        # copying in a new copy of the page object.
         self._sweep_indirect_references(self._root)
 
         object_positions = self._write_pdf_structure(stream)
         xref_location = self._write_xref_table(stream, object_positions)
-        self._write_trailer(stream)
-        stream.write(b_(f"\nstartxref\n{xref_location}\n%%EOF\n"))  # eof
+        self._write_trailer(stream, xref_location)
 
     def write(self, stream: Union[Path, StrByteType]) -> Tuple[bool, IO]:
         """
         Write the collection of pages added to this object out as a PDF file.
 
         Args:
             stream: An object to write the file to.  The object can support
@@ -1208,29 +1205,37 @@
         stream.write(b"xref\n")
         stream.write(b_(f"0 {len(self._objects) + 1}\n"))
         stream.write(b_(f"{0:0>10} {65535:0>5} f \n"))
         for offset in object_positions:
             stream.write(b_(f"{offset:0>10} {0:0>5} n \n"))
         return xref_location
 
-    def _write_trailer(self, stream: StreamType) -> None:
+    def _write_trailer(self, stream: StreamType, xref_location: int) -> None:
+        """
+        Write the PDF trailer to the stream.
+
+        To quote the PDF specification:
+            [The] trailer [gives] the location of the cross-reference table and
+            of certain special objects within the body of the file.
+        """
         stream.write(b"trailer\n")
         trailer = DictionaryObject()
         trailer.update(
             {
                 NameObject(TK.SIZE): NumberObject(len(self._objects) + 1),
                 NameObject(TK.ROOT): self._root,
                 NameObject(TK.INFO): self._info,
             }
         )
         if hasattr(self, "_ID"):
             trailer[NameObject(TK.ID)] = self._ID
         if hasattr(self, "_encrypt"):
             trailer[NameObject(TK.ENCRYPT)] = self._encrypt
         trailer.write_to_stream(stream, None)
+        stream.write(b_(f"\nstartxref\n{xref_location}\n%%EOF\n"))  # eof
 
     def add_metadata(self, infos: Dict[str, Any]) -> None:
         """
         Add custom metadata to the output.
 
         Args:
             infos: a Python dictionary where each key is a field
@@ -1261,14 +1266,29 @@
             NameObject,
             PdfObject,
             NumberObject,
             TextStringObject,
             NullObject,
         ],
     ) -> None:
+        """
+        Resolving any circular references to Page objects.
+
+        Circular references to Page objects can arise when objects such as
+        annotations refer to their associated page. If these references are not
+        properly handled, the PDF file will contain multiple copies of the same
+        Page object. To address this problem, Page objects store their original
+        object reference number. This method adds the reference number of any
+        circularly referenced Page objects to an external reference map. This
+        ensures that self-referencing trees reference the correct new object
+        location, rather than copying in a new copy of the Page object.
+
+        Args:
+            root: The root of the PDF object tree to sweep.
+        """
         stack: Deque[
             Tuple[
                 Any,
                 Optional[Any],
                 Any,
                 List[PdfObject],
             ]
@@ -1329,24 +1349,36 @@
                         if indirect_reference_obj is not None:
                             self._idnum_hash[
                                 indirect_reference_obj.hash_value()
                             ] = indirect_reference
 
     def _resolve_indirect_object(self, data: IndirectObject) -> IndirectObject:
         """
-        Resolves indirect object to this pdf indirect objects.
+        Resolves an indirect object to an indirect object in this PDF file.
 
-        If it is a new object then it is added to self._objects
-        and new idnum is given and generation is always 0.
+        If the input indirect object already belongs to this PDF file, it is
+        returned directly. Otherwise, the object is retrieved from the input
+        object's PDF file using the object's ID number and generation number. If
+        the object cannot be found, a warning is logged and a `NullObject` is
+        returned.
+
+        If the object is not already in this PDF file, it is added to the file's
+        list of objects and assigned a new ID number and generation number of 0.
+        The hash value of the object is then added to the `_idnum_hash`
+        dictionary, with the corresponding `IndirectObject` reference as the
+        value.
 
         Args:
-            data:
+            data: The `IndirectObject` to resolve.
 
         Returns:
-            The resolved indirect object
+            The resolved `IndirectObject` in this PDF file.
+
+        Raises:
+            ValueError: If the input stream is closed.
         """
         if hasattr(data.pdf, "stream") and data.pdf.stream.closed:
             raise ValueError(f"I/O operation on closed file: {data.pdf.stream.name}")
 
         if data.pdf == self:
             return data
```

### Comparing `pypdf-3.8.0/pypdf/constants.py` & `pypdf-3.8.1/pypdf/constants.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/errors.py` & `pypdf-3.8.1/pypdf/errors.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/filters.py` & `pypdf-3.8.1/pypdf/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -648,15 +648,15 @@
     size = (x_object_obj[IA.WIDTH], x_object_obj[IA.HEIGHT])
     data = x_object_obj.get_data()  # type: ignore
     if (
         IA.COLOR_SPACE in x_object_obj
         and x_object_obj[IA.COLOR_SPACE] == ColorSpaces.DEVICE_RGB
     ):
         # https://pillow.readthedocs.io/en/stable/handbook/concepts.html#modes
-        mode: Literal["RGB", "P"] = "RGB"
+        mode: Literal["RGB", "P", "L", "RGBA"] = "RGB"
     else:
         mode = "P"
     extension = None
     if SA.FILTER in x_object_obj:
         if x_object_obj[SA.FILTER] == FT.FLATE_DECODE:
             extension = ".png"  # mime_type = "image/png"
             color_space = None
@@ -679,19 +679,37 @@
                         lookup = b"".join(
                             [lookup[i : i + 1] * 3 for i in range(len(lookup))]
                         )
                     img.putpalette(lookup)
                 else:
                     img.putpalette(lookup.get_data())
                 img = img.convert("L" if base == ColorSpaces.DEVICE_GRAY else "RGB")
+            elif color_space is not None and color_space[0] == "/ICCBased":
+                # see Table 66 - Additional Entries Specific to an ICC Profile
+                # Stream Dictionary
+                icc_profile = color_space[1].get_object()
+                color_components = cast(int, icc_profile["/N"])
+                alternate_colorspace = icc_profile["/Alternate"]
+                color_space = alternate_colorspace
+                mode_map = {
+                    "/DeviceGray": "L",
+                    "/DeviceRGB": "RGB",
+                    "/DeviceCMYK": "RGBA",
+                }
+                mode = (
+                    mode_map.get(color_space)  # type: ignore
+                    or {1: "L", 3: "RGB", 4: "RGBA"}.get(color_components)
+                    or mode
+                )  # type: ignore
+                img = Image.frombytes(mode, size, data)
             if G.S_MASK in x_object_obj:  # add alpha channel
                 alpha = Image.frombytes("L", size, x_object_obj[G.S_MASK].get_data())
                 img.putalpha(alpha)
             img_byte_arr = BytesIO()
-            img.save(img_byte_arr, format="PNG")
+            img.convert("RGBA").save(img_byte_arr, format="PNG")
             data = img_byte_arr.getvalue()
         elif x_object_obj[SA.FILTER] in (
             [FT.LZW_DECODE],
             [FT.ASCII_85_DECODE],
             [FT.CCITT_FAX_DECODE],
         ):
             # I'm not sure if the following logic is correct.
```

### Comparing `pypdf-3.8.0/pypdf/generic/__init__.py` & `pypdf-3.8.1/pypdf/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/generic/_annotations.py` & `pypdf-3.8.1/pypdf/generic/_annotations.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/generic/_base.py` & `pypdf-3.8.1/pypdf/generic/_base.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/generic/_data_structures.py` & `pypdf-3.8.1/pypdf/generic/_data_structures.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/generic/_fit.py` & `pypdf-3.8.1/pypdf/generic/_fit.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/generic/_outline.py` & `pypdf-3.8.1/pypdf/generic/_outline.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/generic/_rectangle.py` & `pypdf-3.8.1/pypdf/generic/_rectangle.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/generic/_utils.py` & `pypdf-3.8.1/pypdf/generic/_utils.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/pagerange.py` & `pypdf-3.8.1/pypdf/pagerange.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/papersizes.py` & `pypdf-3.8.1/pypdf/papersizes.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/types.py` & `pypdf-3.8.1/pypdf/types.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pypdf/xmp.py` & `pypdf-3.8.1/pypdf/xmp.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/pyproject.toml` & `pypdf-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/setup.cfg` & `pypdf-3.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pypdf-3.8.0/PKG-INFO` & `pypdf-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdf
-Version: 3.8.0
+Version: 3.8.1
 Summary: A pure-python PDF library capable of splitting, merging, cropping, and transforming PDF files
 Author-email: Mathieu Fenniak <biziqe@mathieu.fenniak.net>
 Maintainer-email: Martin Thoma <info@martin-thoma.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

