# Comparing `tmp/image_to_arduino-1.0.3.1.tar.gz` & `tmp/image-to-arduino-1.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_to_arduino-1.0.3.1.tar", last modified: Sun Apr 23 08:22:43 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.3.2.tar", last modified: Sun Apr 23 17:56:50 2023, max compression
```

## Comparing `image_to_arduino-1.0.3.1.tar` & `image-to-arduino-1.0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-23 08:22:43.871574 image_to_arduino-1.0.3.1/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3.1/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-04-23 08:22:43.867574 image_to_arduino-1.0.3.1/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1967 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3.1/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-23 08:22:43.867574 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-04-23 08:22:43.000000 image_to_arduino-1.0.3.1/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-23 08:22:43.871574 image_to_arduino-1.0.3.1/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      698 2023-04-23 08:21:38.000000 image_to_arduino-1.0.3.1/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-23 08:22:43.867574 image_to_arduino-1.0.3.1/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3.1/src/__init__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     6688 2023-04-23 08:18:45.000000 image_to_arduino-1.0.3.1/src/image_to_arduino.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-23 17:56:50.247417 image-to-arduino-1.0.3.2/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.2/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-04-23 17:56:50.247417 image-to-arduino-1.0.3.2/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.3.2/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-23 17:56:50.243417 image-to-arduino-1.0.3.2/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-04-23 17:56:50.000000 image-to-arduino-1.0.3.2/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-04-23 17:56:50.000000 image-to-arduino-1.0.3.2/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-23 17:56:50.000000 image-to-arduino-1.0.3.2/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-04-23 17:56:50.000000 image-to-arduino-1.0.3.2/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-04-23 17:56:50.000000 image-to-arduino-1.0.3.2/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-23 17:56:50.247417 image-to-arduino-1.0.3.2/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      698 2023-04-23 17:56:27.000000 image-to-arduino-1.0.3.2/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-23 17:56:50.243417 image-to-arduino-1.0.3.2/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.2/src/__init__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     7724 2023-04-23 17:50:58.000000 image-to-arduino-1.0.3.2/src/image-to-arduino.py
```

### Comparing `image_to_arduino-1.0.3.1/LICENSE` & `image-to-arduino-1.0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image_to_arduino-1.0.3.1/setup.py` & `image-to-arduino-1.0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 REQUIREMENTS = [i.strip() for i in open("/home/wiktor/Image_Converter_App/requirements.txt").readlines()]
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 setup(
-   name='image_to_arduino',
-   version='1.0.3.1',
+   name='image-to-arduino',
+   version='1.0.3.2',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
```

### Comparing `image_to_arduino-1.0.3.1/src/image_to_arduino.py` & `image-to-arduino-1.0.3.2/src/image-to-arduino.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import os
 
 # To check extenxion
 import imghdr
 
 file_path = ''
 image_tk = ''
-switch_state = False
+left_switch_state = False
+right_switch_state = False
 
 def open_file():
     global file_path
     file_path = filedialog.askopenfilename()
     if file_path:
         # If file name len is greater than 15: return ... + extension
         file_label.configure(text="File: " + (os.path.basename(file_path) if len(os.path.basename(file_path)) < 15 else "..." + imghdr.what(file_path)))
@@ -39,28 +40,28 @@
                 
                 # Convert RGB image to grayscale
                 grayscale_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
                 
                 # Convert the image to a PIL Image object
                 image_pre = Image.fromarray(cv2.threshold(grayscale_image, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1])
 
-                if switch_state == True:
+                if left_switch_state == True:
                     # Reverse the colors of the image
                     image_pre = ImageOps.invert(image_pre)
                 
                 # Convert the PIL Image to a PhotoImage object
                 image_pre = ImageTk.PhotoImage(image_pre)
                 
                 # Update the label's image
                 image_preview_label.config(image=image_pre)
                 image_preview_label.image = image_pre
             
                 _, thresholded_image = cv2.threshold(grayscale_image, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
 
-                if switch_state == True:
+                if left_switch_state == True:
                     # Convert the thresholded image to a binary array (0s and 1s)
                     binary_array = np.where(thresholded_image > 0, 0, 1)
                 else:
                     # Convert the thresholded image to a binary array (0s and 1s)
                     binary_array = np.where(thresholded_image > 0, 1, 0)
 
             # Convert the binary array to a 1D array
@@ -74,16 +75,37 @@
 
             cpp_array = ', '.join(hex_byte_arrays)
             # Insert newline after every 10 hexadecimal numbers
             cpp_array = [cpp_array[i:i+2] for i in range(0, len(cpp_array), 2)]  # Split into pairs of hexadecimal numbers
             cpp_array = [''.join(cpp_array[i:i+30]) for i in range(0, len(cpp_array), 30)]  # Join pairs with space, and group every 10 pairs
             cpp_array = '\n'.join(cpp_array)  # Join groups with newline character
 
-            # Generate C++ array
-            cpp_array = 'unsigned char my_array[] = {\n' + cpp_array + '\n};'
+            if right_switch_state == False:
+                # Generate C++ array
+                cpp_array = 'const unsigned char PROGMEM ' + os.path.splitext(os.path.basename(file_path))[0] + ' [] = {\n' + cpp_array + '\n};' 
+            elif right_switch_state == True:
+                # Generate full code ready to use 
+                cpp_array = '''#include <Adafruit_SSD1306.h>
+#include <Adafruit_GFX.h>
+#define OLED_RESET 4
+Adafruit_SSD1306 display(OLED_RESET);
+const unsigned char PROGMEM ''' + os.path.splitext(os.path.basename(file_path))[0] + '''[] = {''' +  cpp_array + ''' };
+void setup() 
+{
+    display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
+    display.display();
+    delay(2000);
+    display.clearDisplay();}
+void loop() 
+{
+    display.drawBitmap(0, 0, ''' + os.path.splitext(os.path.basename(file_path))[0] + ''', 128, 64, 1); 
+    display.display();
+    delay(5000);
+    display.clearDisplay();
+    delay(5000);}'''        
 
             output_text.delete(1.0, tk.END)
             output_text.insert(tk.END, cpp_array)
         
         # In case of error or invalid extension 
         except:
             output_text.delete(1.0, tk.END)
@@ -98,25 +120,29 @@
         copied_all_label.configure(text="No text to copy")
         return
 
     root.clipboard_clear()
     root.clipboard_append(output_text.get(1.0, tk.END))
     copied_all_label.configure(text="✓ Copied")
 
-def toggle_switch():
-    global switch_state
-    switch_state = not switch_state
+def toggle_left_switch():
+    global left_switch_state
+    left_switch_state = not left_switch_state
+
+def toggle_right_switch():
+    global right_switch_state
+    right_switch_state = not right_switch_state
 
 def clear_all():
     # Clear output text and image preview
     output_text.delete(1.0, tk.END)
     image_preview_label.config(image="")
 
-customtkinter.set_appearance_mode("System")  
-customtkinter.set_default_color_theme("blue")  
+customtkinter.set_appearance_mode("dark")  
+customtkinter.set_default_color_theme("dark-blue")  
 
 # Create customtkinter window
 root = customtkinter.CTk() 
 root.title("Image to arduino")
 
 # Set window size
 root.geometry("330x550") # Set width and height as desired
@@ -146,23 +172,24 @@
 copied_all_label.grid(row=4, column=1, pady=5,columnspan=3, sticky="nsew")
 
 # Preview text lael
 preview_text_label = customtkinter.CTkLabel(root, text="Preview")
 preview_text_label.grid(row=5, column=0, pady=5, padx=10)
 
 # Label to display the image
-image_preview_label = tk.Label(root)
+image_preview_label = tk.Label(root, bg="#1b1a1b")
 image_preview_label.grid(row=6, column=0, columnspan=1, padx=10)
 
-# Switch label
-switch = customtkinter.CTkSwitch(root, text="Reverse colors", command=toggle_switch)
+# Switch label left
+switch = customtkinter.CTkSwitch(root, text="Reverse colors", command=toggle_left_switch)
 switch.grid(row=1, column=0, padx=10, sticky="nsew")
-# Switch label right not ready to use
-# switch_right = customtkinter.CTkSwitch(root, text="Full arduino code", command=toggle_switch)
-# switch_right.grid(row=1, column=1, padx=10, sticky="nsew")
+
+# Switch label right 
+switch_right = customtkinter.CTkSwitch(root, text="Full arduino code", command=toggle_right_switch)
+switch_right.grid(row=1, column=1, padx=10, sticky="nsew")
 
 # "Clear all" button 
 clear_all_button = customtkinter.CTkButton(root, text="Clear All", command=clear_all)
 clear_all_button.grid(row=4, column=0, pady=5, padx=10, columnspan=1, sticky="nsew")  
 
 # Configure the window to not be resizable
 root.resizable(False, False)
```

