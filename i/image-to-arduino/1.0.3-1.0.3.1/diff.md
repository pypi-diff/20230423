# Comparing `tmp/image_to_arduino-1.0.3.tar.gz` & `tmp/image_to_arduino-1.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_to_arduino-1.0.3.tar", last modified: Sat Apr 22 13:24:03 2023, max compression
+gzip compressed data, was "image_to_arduino-1.0.3.1.tar", last modified: Sun Apr 23 08:22:43 2023, max compression
```

## Comparing `image_to_arduino-1.0.3.tar` & `image_to_arduino-1.0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1967 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      696 2023-04-22 13:23:36.000000 image_to_arduino-1.0.3/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3/src/__init__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     6690 2023-04-22 13:00:58.000000 image_to_arduino-1.0.3/src/image_to_arduino.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-23 08:22:43.871574 image_to_arduino-1.0.3.1/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3.1/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-04-23 08:22:43.867574 image_to_arduino-1.0.3.1/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1967 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3.1/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-23 08:22:43.867574 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-23 08:22:43.871574 image_to_arduino-1.0.3.1/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      698 2023-04-23 08:21:38.000000 image_to_arduino-1.0.3.1/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-23 08:22:43.867574 image_to_arduino-1.0.3.1/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3.1/src/__init__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     6688 2023-04-23 08:18:45.000000 image_to_arduino-1.0.3.1/src/image_to_arduino.py
```

### Comparing `image_to_arduino-1.0.3/LICENSE` & `image_to_arduino-1.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_to_arduino-1.0.3/README.md` & `image_to_arduino-1.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `image_to_arduino-1.0.3/setup.py` & `image_to_arduino-1.0.3.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 REQUIREMENTS = [i.strip() for i in open("/home/wiktor/Image_Converter_App/requirements.txt").readlines()]
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 setup(
    name='image_to_arduino',
-   version='1.0.3',
+   version='1.0.3.1',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
```

### Comparing `image_to_arduino-1.0.3/src/image_to_arduino.py` & `image_to_arduino-1.0.3.1/src/image_to_arduino.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,22 +108,22 @@
 
 def clear_all():
     # Clear output text and image preview
     output_text.delete(1.0, tk.END)
     image_preview_label.config(image="")
 
 customtkinter.set_appearance_mode("System")  
-customtkinter.set_default_color_theme("dark-blue")  
+customtkinter.set_default_color_theme("blue")  
 
 # Create customtkinter window
 root = customtkinter.CTk() 
-root.title("Image Converter v1.0")
+root.title("Image to arduino")
 
 # Set window size
-root.geometry("320x530") # Set width and height as desired
+root.geometry("330x550") # Set width and height as desired
 
 # Label for displaying selected file path
 file_label =  customtkinter.CTkLabel(root, text="No file selected")
 file_label.grid(row=0, column=0, padx=10, columnspan=1, sticky="nsew", pady=5)
 
 # "Open File" button
 open_file_button = customtkinter.CTkButton(root, text="Open Image File", command=open_file)
@@ -146,23 +146,23 @@
 copied_all_label.grid(row=4, column=1, pady=5,columnspan=3, sticky="nsew")
 
 # Preview text lael
 preview_text_label = customtkinter.CTkLabel(root, text="Preview")
 preview_text_label.grid(row=5, column=0, pady=5, padx=10)
 
 # Label to display the image
-image_preview_label = tk.Label(root, bg='#1c1c1c')
+image_preview_label = tk.Label(root)
 image_preview_label.grid(row=6, column=0, columnspan=1, padx=10)
 
 # Switch label
 switch = customtkinter.CTkSwitch(root, text="Reverse colors", command=toggle_switch)
 switch.grid(row=1, column=0, padx=10, sticky="nsew")
-# Switch label right
-switch_right = customtkinter.CTkSwitch(root, text="Full arduino code", command=toggle_switch)
-switch_right.grid(row=1, column=1, padx=10, sticky="nsew")
+# Switch label right not ready to use
+# switch_right = customtkinter.CTkSwitch(root, text="Full arduino code", command=toggle_switch)
+# switch_right.grid(row=1, column=1, padx=10, sticky="nsew")
 
 # "Clear all" button 
 clear_all_button = customtkinter.CTkButton(root, text="Clear All", command=clear_all)
 clear_all_button.grid(row=4, column=0, pady=5, padx=10, columnspan=1, sticky="nsew")  
 
 # Configure the window to not be resizable
 root.resizable(False, False)
```

