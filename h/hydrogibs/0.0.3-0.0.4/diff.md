# Comparing `tmp/hydrogibs-0.0.3.tar.gz` & `tmp/hydrogibs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.0.3.tar", last modified: Sun Apr 23 14:19:37 2023, max compression
+gzip compressed data, was "hydrogibs-0.0.4.tar", last modified: Sun Apr 23 15:00:51 2023, max compression
```

## Comparing `hydrogibs-0.0.3.tar` & `hydrogibs-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.3/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.3/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/hydrogibs/
--rw-rw-r--   0 axel      (1000) axel      (1000)       13 2023-04-23 13:28:00.000000 hydrogibs-0.0.3/hydrogibs/__init_.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       42 2023-04-23 13:53:43.000000 hydrogibs-0.0.3/hydrogibs/example.py
--rw-rw-r--   0 axel      (1000) axel      (1000)    24140 2023-04-23 13:17:14.000000 hydrogibs-0.0.3/hydrogibs/floods.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-23 14:19:37.000000 hydrogibs-0.0.3/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      226 2023-04-23 14:19:37.000000 hydrogibs-0.0.3/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-23 14:19:37.000000 hydrogibs-0.0.3/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-23 14:19:37.000000 hydrogibs-0.0.3/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-23 14:17:46.000000 hydrogibs-0.0.3/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-23 14:19:37.689379 hydrogibs-0.0.3/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 15:00:51.610881 hydrogibs-0.0.4/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.4/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-23 15:00:51.610881 hydrogibs-0.0.4/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.4/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 15:00:51.606881 hydrogibs-0.0.4/hydrogibs/
+-rw-rw-r--   0 axel      (1000) axel      (1000)       13 2023-04-23 13:28:00.000000 hydrogibs-0.0.4/hydrogibs/__init_.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       42 2023-04-23 13:53:43.000000 hydrogibs-0.0.4/hydrogibs/example.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)    24378 2023-04-23 15:00:15.000000 hydrogibs-0.0.4/hydrogibs/floods.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-23 15:00:51.610881 hydrogibs-0.0.4/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-23 15:00:51.000000 hydrogibs-0.0.4/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      226 2023-04-23 15:00:51.000000 hydrogibs-0.0.4/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-23 15:00:51.000000 hydrogibs-0.0.4/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-23 15:00:51.000000 hydrogibs-0.0.4/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-23 15:00:37.000000 hydrogibs-0.0.4/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-23 15:00:51.610881 hydrogibs-0.0.4/setup.cfg
```

### Comparing `hydrogibs-0.0.3/LICENSE` & `hydrogibs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.3/PKG-INFO` & `hydrogibs-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.0.3/hydrogibs/floods.py` & `hydrogibs-0.0.4/hydrogibs/floods.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,51 +458,58 @@
 
         ctk.set_appearance_mode(appearance)
         ctk.set_default_color_theme(color_theme)
 
         self.root = ctk.CTk()
         self.root.title("Génie Rural 4")
         self.root.bind('<Return>', self.entries_update)
-        self.ww = self.root.winfo_screenwidth()
-        self.wh = self.root.winfo_screenheight()
-        self.root.geometry(f"{self.ww*0.8:.0f}x{self.wh*0.5:.0f}")
+        # self.ww = self.root.winfo_screenwidth()
+        # self.wh = self.root.winfo_screenheight()
+        # self.root.geometry(f"{self.ww*0.8:.0f}x{self.wh*0.5:.0f}")
 
         self.dframe = ctk.CTkFrame(master=self.root)
-        self.dframe.pack(side=ctk.RIGHT, fill="x", pady=0)
+        self.dframe.grid(row=0, column=1, sticky="NSEW")
         self.draw_diagram()
 
-        entryframe = ctk.CTkLabel(text="GR4 method", master=self.root)
-        entryframe.pack(side=ctk.TOP)
+        self.pframe = ctk.CTkFrame(master=self.root)
+        self.pframe.grid(column=0, row=0, sticky="NSEW")
+
+        entryframe = ctk.CTkLabel(text="GR4 parameters",
+                                  master=self.pframe,
+                                  font=("monospace", 24))
+        entryframe.grid(row=0, column=0,
+                        sticky="NSEW",
+                        ipadx=5, ipady=10)
 
         self.entries = dict()
         self.define_entry("X1", "-", self.gr4.X1)
         self.define_entry("X2", "mm", self.gr4.X2)
         self.define_entry("X3", "1/h", self.gr4.X3)
         self.define_entry("X4", "h", self.gr4.X4)
         self.root.mainloop()
 
     def define_entry(self, key: str, unit, value):
 
-        entryframe = ctk.CTkFrame(master=self.root)
-        entryframe.pack(side=ctk.TOP)
+        entryframe = ctk.CTkFrame(master=self.pframe)
+        entryframe.grid(sticky="NSEW")
         unit_str = f"[{unit}]"
         label = ctk.CTkLabel(master=entryframe,
-                             text=f"{key:>5} {unit_str:>5}",
-                             font=("monospace", 12))
-        label.pack(pady=10, padx=20, fill="x", side=ctk.LEFT)
+                             text=f"{key:>5} {unit_str:>5} ",
+                             font=("monospace", 14))
+        label.grid(row=0, column=0, sticky="EW", ipady=5)
 
         input = ctk.CTkEntry(master=entryframe)
         input.insert(0, value)
-        input.pack(pady=10, padx=20, fill="both", side=ctk.LEFT)
+        input.grid(row=0, column=1, sticky="EW")
 
         slider = ctk.CTkSlider(master=entryframe,
                                from_=0, to=2*value,
                                number_of_steps=999,
                                command=lambda _: self.slider_update(key))
-        slider.pack(pady=10, padx=20, fill="x", side=ctk.RIGHT)
+        slider.grid(row=0, column=2, sticky="EW")
 
         self.entries[key] = dict(
             label=label,
             input=input,
             slider=slider
         )
 
@@ -526,17 +533,17 @@
         self.fig, axes, lines = self.gr4.diagram(show=False)
         self.ax1, self.ax2, self.ax3 = axes
         self.rain, self.disch, self.dischp, self.dischv, self.wflow = lines
 
         self.canvas = FigureCanvasTkAgg(self.fig, master=self.dframe)
         toolbar = NavigationToolbar2Tk(self.canvas)
         toolbar.update()
-        self.canvas._tkcanvas.pack(side=ctk.TOP, fill="x")
+        self.canvas._tkcanvas.pack()
         self.canvas.draw()
-        self.canvas.get_tk_widget().pack(fill="x")
+        self.canvas.get_tk_widget().pack()
         self.canvas.mpl_connect('key_press_event',
                                 lambda arg: key_press_handler(
                                     arg, self.canvas, toolbar
                                 ))
         self.root.update()
 
     def update_canvas(self):
```

### Comparing `hydrogibs-0.0.3/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.0.4/hydrogibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

