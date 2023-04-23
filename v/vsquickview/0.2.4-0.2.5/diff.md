# Comparing `tmp/vsquickview-0.2.4.tar.gz` & `tmp/vsquickview-0.2.5.tar.gz`

## Comparing `vsquickview-0.2.4.tar` & `vsquickview-0.2.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 vsquickview-0.2.4/vsquickview/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 vsquickview-0.2.4/vsquickview/colourbars.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 vsquickview-0.2.4/vsquickview/fakevsquickview.py
--rw-r--r--   0        0        0    14002 2020-02-02 00:00:00.000000 vsquickview-0.2.4/vsquickview/vsquickview.py
--rw-r--r--   0        0        0    14037 2020-02-02 00:00:00.000000 vsquickview-0.2.4/vsquickview/vsquickview.qml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vsquickview-0.2.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 vsquickview-0.2.4/LICENSE
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 vsquickview-0.2.4/README.md
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 vsquickview-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 vsquickview-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/colourbars.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/fakevsquickview.py
+-rw-r--r--   0        0        0    14623 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/vsquickview.py
+-rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/vsquickview.qml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vsquickview-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 vsquickview-0.2.5/LICENSE
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 vsquickview-0.2.5/README.md
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 vsquickview-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 vsquickview-0.2.5/PKG-INFO
```

### Comparing `vsquickview-0.2.4/vsquickview/__init__.py` & `vsquickview-0.2.5/vsquickview/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,12 +21,28 @@
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ---------------------------------------------------------------------
 
 import __main__
 if not __main__.__name__ == "__vapoursynth__":
-    from .vsquickview import View, RemoveView, SetFrame, SetIndex, SetPreviewGroup, ClearPreviewGroup, Show, Hide
+    from .vsquickview import View, \
+                             RemoveView, \
+                             SetFrame, \
+                             SetIndex, \
+                             SetPreviewGroup, \
+                             ClearPreviewGroup, \
+                             PreviewGroup, \
+                             Show, \
+                             Hide
 else:
-    from .fakevsquickview import View, RemoveView, SetFrame, SetIndex, SetPreviewGroup, ClearPreviewGroup, Show, Hide
+    from .fakevsquickview import View, \
+                                 RemoveView, \
+                                 SetFrame, \
+                                 SetIndex, \
+                                 SetPreviewGroup, \
+                                 ClearPreviewGroup, \
+                                 PreviewGroup, \
+                                 Show, \
+                                 Hide
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
```

### Comparing `vsquickview-0.2.4/vsquickview/colourbars.py` & `vsquickview-0.2.5/vsquickview/colourbars.py`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.4/vsquickview/fakevsquickview.py` & `vsquickview-0.2.5/vsquickview/fakevsquickview.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,11 +31,13 @@
     pass
 def SetIndex(*_, **__):
     pass
 def SetPreviewGroup(*_, **__):
     pass
 def ClearPreviewGroup(*_, **__):
     pass
+def PreviewGroup(*_, **__):
+    pass
 def Show(*_, **__):
     pass
 def Hide(*_, **__):
     pass
```

### Comparing `vsquickview-0.2.4/vsquickview/vsquickview.py` & `vsquickview-0.2.5/vsquickview/vsquickview.py`

 * *Files 3% similar despite different names*

```diff
@@ -278,14 +278,27 @@
             self.frame = self.preview_group[bisect.bisect_left(self.preview_group, self.frame + 1)]
         else:
             self.nextFrame()
     @pyqtSlot(int)
     def switchFrame(self, frame):
         self.frame = frame
 
+    previewGroupChanged = pyqtSignal()
+    @pyqtSlot(result=bool)
+    def frameInPreviewGroup(self):
+        return self.frame in self.preview_group
+    @pyqtSlot()
+    def toggleFrameInPreviewGroup(self):
+        if self.frame in self.preview_group:
+            self.preview_group.remove(self.frame)
+        else:
+            self.preview_group.append(self.frame)
+            self.preview_group.sort()
+        self.previewGroupChanged.emit()
+
     @pyqtSlot()
     def manageCache(self):
         cancelPreviousWorks(self.index)
 
         cacheFrames(self.index, self.frame, True)
         for index in range(10):
             cacheFrames(index, self.frame, False)
@@ -386,25 +399,28 @@
         index = clip
     assert(type(index) == int and 0 <= index < 10)
 
     backend.switchIndex(index)
 def SetPreviewGroup(clip: Union[vs.VideoNode, int, None]=None, group: Optional[list]=None):
     if group == None:
         group = clip
-    assert(type(group) == list and all([type(item) == int for item in group]))
+    assert(type(group) == list and all([type(item) == int and item >= 0 for item in group]))
 
     group = list(set(group))
     group.sort()
 
     backend.preview_group = group
 
+    backend.previewGroupChanged.emit()
     backend.cacheUpdateTrigger.emit()
 def ClearPreviewGroup(clip: Optional[vs.VideoNode]=None):
     backend.preview_group = []
     
+    backend.previewGroupChanged.emit()
     backend.cacheUpdateTrigger.emit()
+def PreviewGroup(clip: Optional[vs.VideoNode]=None):
+    return backend.preview_group
 
 def Show(clip: Optional[vs.VideoNode]=None):
     window_control.show.emit()
-
 def Hide(clip: Optional[vs.VideoNode]=None):
     window_control.hide.emit()
```

### Comparing `vsquickview-0.2.4/vsquickview/vsquickview.qml` & `vsquickview-0.2.5/vsquickview/vsquickview.qml`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     property bool showLabelText: false
     property string extraLabelText: ""
     function updateLabelText() {
         if(extraLabelText) {
             label.text = extraLabelText
         }
         else if(showLabelText) {
-            label.text = "Index " + backend.index.toString() + (backend.name ? ": " + backend.name : "") + " / Frame " + backend.frame.toString()
+            label.text = "Index " + backend.index.toString() + (backend.name ? ": " + backend.name : "") + " / Frame " + backend.frame.toString() + (backend.frameInPreviewGroup() ? " (Preview Group)" : "")
         }
         else {
             label.text = ""
         }
     }
     Connections {
         target: window
@@ -110,14 +110,20 @@
     }
     Connections {
         target: backend
         function onNameChanged() {
             updateLabelText()
         }
     }
+    Connections {
+        target: backend
+        function onPreviewGroupChanged() {
+            updateLabelText()
+        }
+    }
 
     Label {
         id: label
         font.pixelSize: 35
         color: "#B0FFFFFF"
         antialiasing: true
         anchors.bottom: parent.bottom
@@ -416,14 +422,18 @@
             else if(event.key === Qt.Key_8) {
                 backend.switchIndex(8)
             }
             else if(event.key === Qt.Key_9) {
                 backend.switchIndex(9)
             }
 
+            else if(event.key === Qt.Key_R) {
+                backend.toggleFrameInPreviewGroup()
+            }
+
             else {
                 event.accepted = false
             }
         }
         Keys.onReleased: (event) => {
             if(altPressed && event.key === Qt.Key_Alt) {
                 window.showLabelText = !window.showLabelText
```

### Comparing `vsquickview-0.2.4/LICENSE` & `vsquickview-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.4/README.md` & `vsquickview-0.2.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <h1 align="center">vsquickview</h1>
 
 vsquickview is a frame-by-frame VapourSynth preview script designed to be used together with Jupyter Notebook with these advantages:  
 
-* Less waiting. vsquickview will run alongside Jupyter Notebook. Everytimes you make an adjustment, you can switch to the vsquickview window to see the updated result immediately.  
+* Less waiting. vsquickview will run alongside Jupyter Notebook. Everytimes you make an adjustment, you can switch to the vsquickview window to view the result immediately.  
 * Easier comparing between two clips with a right click. Blind comparing is also possible.  
 
 *Thanks to*  
 
 * Setsugen no ao for helping with VapourSynth magics.  
 * witchymary and others for helping with the UX.  
 
@@ -97,7 +97,27 @@
 * `G`: Press `G` key and type the frame number followed by `Enter` key to go to a specific frame.  
 * `Left` Key or `Right` Key: Go to the previous or the next frame.  
 * `Ctrl` and `Left` Key or `Right` Key: Jump 12 frames backwards or forwards.  
 * `Up` Key or `Down` Key: Go to the next or previous clip, but not cycling the clips.  
 * `F` or `F11`: Toggle fullscreen.  
 
 vsquickview will be closed when you terminate or restart the Jupyter Notebook section. If you close the vsquickview window by accident, you can reopen it by calling function `vsquickview.Show()`.  
+
+### Using preview group
+
+Additionally, you can also create preview group for a selecteds list of frames you want to compare.  
+
+Set preview group using the `vsquickview.SetPreviewGroup()` function:  
+```py
+vsqv.SetPreviewGroup([1934, 6849, 13226, 21647, 25374, 26811, 28499, 29111])
+```
+
+In the vsquickview GUI, use `Shift` Key and `Left` Key or `Right` Key to go to the previous or next frame in the set preview group.  
+
+You can also add frame to or remove frame from the preview group using `R` Key from GUI. Afterwards, you can retrieve the current preview group using the `vsquickview.PreviewGroup()` function.  
+
+Here is a short list of functions and their definitions for preview group:  
+```py
+SetPreviewGroup(clip: Union[vs.VideoNode, int, None]=None, group: Optional[list]=None)
+ClearPreviewGroup(clip: Optional[vs.VideoNode]=None)
+PreviewGroup(clip: Optional[vs.VideoNode]=None)
+```
```

### Comparing `vsquickview-0.2.4/pyproject.toml` & `vsquickview-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.4/PKG-INFO` & `vsquickview-0.2.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsquickview
-Version: 0.2.4
+Version: 0.2.5
 Summary: VapourSynth preview script
 Project-URL: Documentation, https://github.com/Akatmks/vsquickview
 Project-URL: Issues, https://github.com/Akatmks/vsquickview/issues
 Project-URL: Source, https://github.com/Akatmks/vsquickview
 Author-email: Akatsumekusa <Akatsumekusa@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -21,15 +21,15 @@
 Requires-Dist: pyqt5
 Description-Content-Type: text/markdown
 
 <h1 align="center">vsquickview</h1>
 
 vsquickview is a frame-by-frame VapourSynth preview script designed to be used together with Jupyter Notebook with these advantages:  
 
-* Less waiting. vsquickview will run alongside Jupyter Notebook. Everytimes you make an adjustment, you can switch to the vsquickview window to see the updated result immediately.  
+* Less waiting. vsquickview will run alongside Jupyter Notebook. Everytimes you make an adjustment, you can switch to the vsquickview window to view the result immediately.  
 * Easier comparing between two clips with a right click. Blind comparing is also possible.  
 
 *Thanks to*  
 
 * Setsugen no ao for helping with VapourSynth magics.  
 * witchymary and others for helping with the UX.  
 
@@ -120,7 +120,27 @@
 * `G`: Press `G` key and type the frame number followed by `Enter` key to go to a specific frame.  
 * `Left` Key or `Right` Key: Go to the previous or the next frame.  
 * `Ctrl` and `Left` Key or `Right` Key: Jump 12 frames backwards or forwards.  
 * `Up` Key or `Down` Key: Go to the next or previous clip, but not cycling the clips.  
 * `F` or `F11`: Toggle fullscreen.  
 
 vsquickview will be closed when you terminate or restart the Jupyter Notebook section. If you close the vsquickview window by accident, you can reopen it by calling function `vsquickview.Show()`.  
+
+### Using preview group
+
+Additionally, you can also create preview group for a selecteds list of frames you want to compare.  
+
+Set preview group using the `vsquickview.SetPreviewGroup()` function:  
+```py
+vsqv.SetPreviewGroup([1934, 6849, 13226, 21647, 25374, 26811, 28499, 29111])
+```
+
+In the vsquickview GUI, use `Shift` Key and `Left` Key or `Right` Key to go to the previous or next frame in the set preview group.  
+
+You can also add frame to or remove frame from the preview group using `R` Key from GUI. Afterwards, you can retrieve the current preview group using the `vsquickview.PreviewGroup()` function.  
+
+Here is a short list of functions and their definitions for preview group:  
+```py
+SetPreviewGroup(clip: Union[vs.VideoNode, int, None]=None, group: Optional[list]=None)
+ClearPreviewGroup(clip: Optional[vs.VideoNode]=None)
+PreviewGroup(clip: Optional[vs.VideoNode]=None)
+```
```

