# Comparing `tmp/webarchiver-0.7.0-py2.py3-none-any.whl.zip` & `tmp/webarchiver-0.8.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5911084 bytes, number of entries: 11
--rw-r--r--  2.0 unx      296 b- defN 23-Feb-21 01:40 webarchiver/__init__.py
--rw-r--r--  2.0 unx      116 b- defN 23-Feb-21 02:58 webarchiver/version.py
--rw-r--r--  2.0 unx    32522 b- defN 23-Feb-21 02:58 webarchiver/webarchiver.py
--rw-r--r--  2.0 unx  2984341 b- defN 23-Feb-21 01:40 webarchiver/lib/uBlock-Origin_v1.27.0.crx
--rw-r--r--  2.0 unx  2984341 b- defN 23-Feb-21 01:40 webarchiver-0.7.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx
--rw-r--r--  2.0 unx     1211 b- defN 23-Feb-21 02:58 webarchiver-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2625 b- defN 23-Feb-21 02:58 webarchiver-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-21 02:58 webarchiver-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 23-Feb-21 02:58 webarchiver-0.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Feb-21 02:58 webarchiver-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      973 b- defN 23-Feb-21 02:58 webarchiver-0.7.0.dist-info/RECORD
-11 files, 6006609 bytes uncompressed, 5909426 bytes compressed:  1.6%
+Zip file size: 5912079 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      296 b- defN 23-Apr-23 06:10 webarchiver/__init__.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Apr-23 06:10 webarchiver/version.py
+-rw-r--r--  2.0 unx    39135 b- defN 23-Apr-23 06:10 webarchiver/webarchiver.py
+-rw-r--r--  2.0 unx  2984341 b- defN 23-Apr-23 06:10 webarchiver/lib/uBlock-Origin_v1.27.0.crx
+-rw-r--r--  2.0 unx  2984341 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx
+-rw-r--r--  2.0 unx     1211 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3295 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      973 b- defN 23-Apr-23 06:10 webarchiver-0.8.0.dist-info/RECORD
+11 files, 6013892 bytes uncompressed, 5910421 bytes compressed:  1.7%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: webarchiver/webarchiver.py
 Comment: 
 
 Filename: webarchiver/lib/uBlock-Origin_v1.27.0.crx
 Comment: 
 
-Filename: webarchiver-0.7.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx
+Filename: webarchiver-0.8.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx
 Comment: 
 
-Filename: webarchiver-0.7.0.dist-info/LICENSE
+Filename: webarchiver-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: webarchiver-0.7.0.dist-info/METADATA
+Filename: webarchiver-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: webarchiver-0.7.0.dist-info/WHEEL
+Filename: webarchiver-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: webarchiver-0.7.0.dist-info/entry_points.txt
+Filename: webarchiver-0.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: webarchiver-0.7.0.dist-info/top_level.txt
+Filename: webarchiver-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: webarchiver-0.7.0.dist-info/RECORD
+Filename: webarchiver-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webarchiver/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.7.0'
+__version__ = '0.8.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## webarchiver/webarchiver.py

```diff
@@ -15,14 +15,15 @@
 from bs4 import BeautifulSoup
 from pathlib import Path
 from io import BytesIO
 from PIL import Image, ImageChops
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from webdriver_manager.chrome import ChromeDriverManager
+from webdriver_manager.firefox import GeckoDriverManager
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.action_chains import ActionChains
 
 
 class Webarchiver:
@@ -30,71 +31,153 @@
         self.urls = []
         self.file_urls = []
         self.driver = None
         self.home = os.path.expanduser("~")
         self.save_path = os.path.join(self.home, "Downloads")
         self.capabilities = None
         self.chrome_options = webdriver.ChromeOptions()
+        self.firefox_options = webdriver.FirefoxOptions()
         self.image_format = 'PNG'
         self.image_quality = 80
         self.hidden_scroll_bar = 'hidden'
         self.screenshot_success = False
         self.screenshot_success_alt = False
         self.zoom_level = 100
         self.dpi = 1.0
         self.max_scroll_height = 369369
         self.threads = os.cpu_count()
         self.url_filter = None
+        self.url_count = 0
+        self.executor = "Local"
+        self.host = "None"
+        self.browser = "Chrome"
 
     def launch_browser(self):
-        self.capabilities = {
-            'self.browserName': 'chrome',
-            'chromeOptions': {
-                'useAutomationExtension': False,
-                'forceDevToolsScreenshot': True
+        if self.browser.lower() == "chrome" and self.executor.lower() == "local":
+            self.capabilities = {
+                'self.browserName': 'chrome',
+                'chromeOptions': {
+                    'useAutomationExtension': False,
+                    'forceDevToolsScreenshot': True
+                }
             }
-        }
-        # Pass the argument 1 to allow and 2 to block
-        self.chrome_options.add_experimental_option("prefs", {
-            "profile.default_content_setting_values.notifications": 2
-        })
-        # Add Ublock Origin to Chrome
-        parent_dir = os.path.abspath(os.path.dirname(__file__))
-        lib_dir = os.path.join(parent_dir, 'lib')
-        sys.path.append(lib_dir)
-        adblock_path = f'{lib_dir}/uBlock-Origin_v1.27.0.crx'
-        if os.path.isfile(adblock_path):
-            print(f"uBlock Origin Found: {adblock_path}")
-            self.chrome_options.add_extension(adblock_path)
-        elif os.path.isfile(f'{os.curdir}/lib/uBlock-Origin_v1.27.0.crx'):
-            adblock_path = f'{os.curdir}/lib/uBlock-Origin_v1.27.0.crx'
-            print(f"uBlock Origin Found: {adblock_path}")
-            self.chrome_options.add_extension(adblock_path)
-        else:
-            print(f"uBlock Origin was not found")
-        self.chrome_options.add_argument('--disable-gpu')
-        self.chrome_options.add_argument('--start-maximized')
-        self.chrome_options.add_argument('--hide-scrollbars')
-        self.chrome_options.add_argument('--disable-infobars')
-        self.chrome_options.add_argument('--disable-notifications')
-        self.chrome_options.add_argument('--disable-dev-shm-usage')
-        self.chrome_options.add_argument('--dns-prefetch-disable')
-        if self.dpi != 1:
-            self.chrome_options.add_argument(f'--force-device-scale-factor={self.dpi}')
-            self.chrome_options.add_argument(f'--high-dpi-support={self.dpi}')
-        try:
-            self.driver = webdriver.Chrome(executable_path=ChromeDriverManager().install(),
-                                           desired_capabilities=self.capabilities,
-                                           options=self.chrome_options)
-            # Hide the scrollbar
-            scrollbar_js = 'document.documentElement.style.overflow = \"{}\"'.format(self.hidden_scroll_bar)
-            self.driver.execute_script(scrollbar_js)
-        except Exception as e:
-            print("Could not open with Latest Chrome Version. PLEASE ENSURE YOU'RE NOT RUNNING WITH SUDO", e)
-            exit()
+            # Pass the argument 1 to allow and 2 to block
+            self.chrome_options.add_experimental_option("prefs", {
+                "profile.default_content_setting_values.notifications": 2
+            })
+            # Add Ublock Origin to Chrome
+            parent_dir = os.path.abspath(os.path.dirname(__file__))
+            lib_dir = os.path.join(parent_dir, 'lib')
+            sys.path.append(lib_dir)
+            adblock_path = f'{lib_dir}/uBlock-Origin_v1.27.0.crx'
+            if os.path.isfile(adblock_path):
+                print(f"uBlock Origin Found: {adblock_path}")
+                self.chrome_options.add_extension(adblock_path)
+            elif os.path.isfile(f'{os.curdir}/lib/uBlock-Origin_v1.27.0.crx'):
+                adblock_path = f'{os.curdir}/lib/uBlock-Origin_v1.27.0.crx'
+                print(f"uBlock Origin Found: {adblock_path}")
+                self.chrome_options.add_extension(adblock_path)
+            else:
+                print(f"uBlock Origin was not found")
+            self.chrome_options.add_argument('--disable-gpu')
+            self.chrome_options.add_argument('--start-maximized')
+            self.chrome_options.add_argument('--hide-scrollbars')
+            self.chrome_options.add_argument('--disable-infobars')
+            self.chrome_options.add_argument('--disable-notifications')
+            self.chrome_options.add_argument('--disable-dev-shm-usage')
+            self.chrome_options.add_argument('--dns-prefetch-disable')
+            if self.dpi != 1:
+                self.chrome_options.add_argument(f'--force-device-scale-factor={self.dpi}')
+                self.chrome_options.add_argument(f'--high-dpi-support={self.dpi}')
+            try:
+                self.driver = webdriver.Chrome(executable_path=ChromeDriverManager().install(),
+                                               desired_capabilities=self.capabilities,
+                                               options=self.chrome_options)
+                # Hide the scrollbar
+                scrollbar_js = 'document.documentElement.style.overflow = \"{}\"'.format(self.hidden_scroll_bar)
+                self.driver.execute_script(scrollbar_js)
+            except Exception as e:
+                print("Could not open with Latest Chrome Version. PLEASE ENSURE YOU'RE NOT RUNNING WITH SUDO", e)
+                exit()
+        elif self.browser.lower() == "firefox" and self.executor.lower() == "local":
+            options = webdriver.FirefoxOptions()
+            options.headless = True
+            self.driver = webdriver.Firefox(executable_path = GeckoDriverManager().install(), options=options)
+            self.driver.set_window_position(0,0)
+            self.driver.maximize_window()
+        elif self.browser.lower() == "chrome" and self.executor.lower() != "local":
+            browser_name = "Webarchiver"
+            options = webdriver.ChromeOptions()
+            capabilities = {
+                "browserName": "chrome",
+                "browserVersion": "latest",
+                f"{self.host}:options": {
+                    "enableVideo": False,
+                    "enableVNC": True,
+                    "name": browser_name,
+                    "setAcceptInsecureCerts": True,
+                    "acceptSslCerts": True,
+                }
+            }
+            # Add Ublock Origin to Chrome
+            parent_dir = os.path.abspath(os.path.dirname(__file__))
+            lib_dir = os.path.join(parent_dir, 'lib')
+            sys.path.append(lib_dir)
+            adblock_path = f'{lib_dir}/uBlock-Origin_v1.27.0.crx'
+            if os.path.isfile(adblock_path):
+                print(f"uBlock Origin Found: {adblock_path}")
+                self.chrome_options.add_extension(adblock_path)
+            elif os.path.isfile(f'{os.curdir}/lib/uBlock-Origin_v1.27.0.crx'):
+                adblock_path = f'{os.curdir}/lib/uBlock-Origin_v1.27.0.crx'
+                print(f"uBlock Origin Found: {adblock_path}")
+                self.chrome_options.add_extension(adblock_path)
+            else:
+                print(f"uBlock Origin was not found")
+            self.chrome_options.add_argument('--disable-gpu')
+            self.chrome_options.add_argument('--start-maximized')
+            self.chrome_options.add_argument('--hide-scrollbars')
+            self.chrome_options.add_argument('--disable-infobars')
+            self.chrome_options.add_argument('--disable-notifications')
+            self.chrome_options.add_argument('--disable-dev-shm-usage')
+            self.chrome_options.add_argument('--dns-prefetch-disable')
+            self.chrome_options.add_argument('--log-level=3')
+            self.driver = webdriver.Remote(
+                command_executor=self.executor,
+                options=options,
+                desired_capabilities=capabilities
+            )
+            self.driver.maximize_window()
+        elif self.browser.lower() == "firefox" and self.executor.lower() != "local":
+            browser_name = "Webarchiver"
+            options = webdriver.ChromeOptions()
+            capabilities = {
+                "browserName": "firefox",
+                "browserVersion": "latest",
+                f"{self.host}:options": {
+                    "enableVideo": False,
+                    "enableVNC": True,
+                    "name": browser_name,
+                    "setAcceptInsecureCerts": True,
+                    "acceptSslCerts": True,
+                }
+            }
+            self.chrome_options.add_argument('--disable-gpu')
+            self.chrome_options.add_argument('--start-maximized')
+            self.chrome_options.add_argument('--hide-scrollbars')
+            self.chrome_options.add_argument('--disable-infobars')
+            self.chrome_options.add_argument('--disable-notifications')
+            self.chrome_options.add_argument('--disable-dev-shm-usage')
+            self.chrome_options.add_argument('--dns-prefetch-disable')
+            self.chrome_options.add_argument('--log-level=3')
+            self.driver = webdriver.Remote(
+                command_executor=self.executor,
+                options=options,
+                desired_capabilities=capabilities
+            )
+            self.driver.maximize_window()
 
     def open_file(self, file):
         webarchive_urls = open(file, 'r')
         for url in webarchive_urls:
             self.append_link(url)
 
     def append_link(self, url):
@@ -115,14 +198,26 @@
     def get_links(self):
         return self.urls
 
     def reset_links(self):
         print("Links Reset")
         self.urls = []
 
+    def set_executor(self, executor="Local"):
+        self.host = "None"
+        self.executor = executor
+        if executor != "Local":
+            self.host = executor.split('|')[0]
+            self.executor = executor.split('|')[1]
+
+        print(f"HOST: {self.host} EXECUTOR: {self.executor}")
+
+    def set_browser(self, browser="Chrome"):
+        self.browser = browser
+
     def set_zoom_level(self, zoom_percentage=100):
         self.zoom_level = zoom_percentage
 
     def set_dpi_level(self, dpi=1):
         self.dpi = dpi
 
     def read_url(self, url, zoom_percentage):
@@ -596,106 +691,149 @@
                       f"{os.path.normpath(os.path.join(self.save_path, site_folder, file_name))}")
             else:
                 print(f"\tFile {os.path.normpath(os.path.join(self.save_path, site_folder, file_name))} "
                       f"already downloaded")
         except Exception as e:
             pass
 
+    def chunks(self, lst, n):
+        for i in range(0, len(lst), n):
+            return list(lst[i:i + n])
+
+    def screenshot_urls_in_parallel(self, parallel_urls):
+        self.launch_browser()
+        for url in parallel_urls:
+            self.set_zoom_level(self.zoom_level)
+            self.full_page_screenshot(url=f'{url}', zoom_percentage=self.zoom_level)
+            self.url_count = self.url_count + 1
+            percentage = '%.3f' % ((self.url_count / len(self.urls)) * 100)
+            urls_processed = '{0: <25}'.format(f"URLs Processed: {self.url_count}")
+            percentage_display = '{0: <20}'.format(f"Percentage: {percentage}%")
+            total = '{0: <15}'.format(f"Total: {self.url_count}/{len(self.urls)}")
+            print(f"{urls_processed} | {percentage_display} | {total}\n")
+        self.quit_driver()
+        self.url_count = 0
+
 
 def webarchiver(argv):
     filename = "./links.txt"
+    browser = "Chrome"
+    executor = "Local"
     archive = Webarchiver()
     clean_flag = False
     file_flag = False
     zoom_level = 100
     image_archive = False
     scrape_flag = False
     url_filter = None
     threads = os.cpu_count()
 
     try:
-        opts, args = getopt.getopt(argv, "hcd:f:l:i:st:u:z:", ["help", "clean", "directory=", "dpi=", "file=",
-                                                               "links=", "image-type=", "scrape", "threads=",
-                                                               "url-filter=", "zoom="])
+        opts, args = getopt.getopt(argv, "hb:cd:e:f:l:i:st:u:z:", ["help", "browser=", "clean", "directory=", "dpi=",
+                                                                 "file=", "executor=", "links=", "image-type=", "scrape", "threads=",
+                                                                 "url-filter=", "zoom="])
     except getopt.GetoptError:
         usage()
         sys.exit(2)
+
     for opt, arg in opts:
         if opt in ("-h", "--help"):
             usage()
             sys.exit()
+        elif opt in ("-b", "--browser"):
+            browser = arg
         elif opt in ("-c", "--clean"):
             clean_flag = True
         elif opt in ("-d", "--directory"):
             archive.set_save_path(arg)
         elif opt == "--dpi":
             archive.set_dpi_level(int(arg))
         elif opt in ("-f", "--file"):
             file_flag = True
             filename = arg
+        elif opt in ("-e", "--executor"):
+            executor = arg
         elif opt in ("-s", "--scrape"):
             scrape_flag = True
         elif opt in ("-u", "--url-filter"):
             url_filter = arg
         elif opt in ("-l", "--links"):
             url_list = arg.replace(" ", "")
             url_list = url_list.split(",")
             for url in url_list:
                 archive.append_link(url.strip())
         elif opt in ("-i", "--image-type"):
-            if arg == "PNG" or arg == "png" or arg == "JPG" or arg == "jpg" or arg == "JPEG" or arg == "jpeg":
-                archive.image_format = f'{arg}'
+            if arg.lower() == "png" or arg.lower() == "jpg" or arg.lower() == "jpeg":
+                archive.image_format = f'{arg.lower()}'
             image_archive = True
         elif opt in ("-t", "--threads"):
             threads = arg
         elif opt in ("-z", "--zoom"):
             zoom_level = arg
 
     if file_flag:
         archive.open_file(filename)
 
     if clean_flag:
         archive.clean_url()
 
     if image_archive:
+        archive.set_browser(browser=browser)
+        archive.set_executor(executor=executor)
         archive.launch_browser()
         url_count = 0
         for url in archive.urls:
             archive.set_zoom_level(zoom_level)
             archive.full_page_screenshot(url=f'{url}', zoom_percentage=zoom_level)
             url_count = url_count + 1
             percentage = '%.3f' % ((url_count / len(archive.urls)) * 100)
             urls_processed = '{0: <25}'.format(f"URLs Processed: {url_count}")
             percentage_display = '{0: <20}'.format(f"Percentage: {percentage}%")
             total = '{0: <15}'.format(f"Total: {url_count}/{len(archive.urls)}")
             print(f"{urls_processed} | {percentage_display} | {total}\n")
         archive.quit_driver()
 
+        # print("Starting")
+        # archive.set_zoom_level(zoom_level)
+        # archive.set_threads(threads=threads)
+        # archive.set_browser(browser=browser)
+        # archive.set_executor(executor=executor)
+        # parallel_urls = archive.chunks(archive.urls, threads)
+        # pool = Pool(processes=threads)
+        # try:
+        #     pool.map(archive.screenshot_urls_in_parallel, parallel_urls)
+        # finally:
+        #     pool.close()
+        #     pool.join()
+
+
     if scrape_flag:
         archive.set_threads(threads=threads)
         archive.set_url_filter(url_filter=url_filter)
         archive.scrape_urls_in_parallel()
         archive.download_urls_in_parallel()
 
 
 def usage():
     print(f'Usage:\n'
           f'-h | --help       [ See usage ]\n'
+          f'-b | --browser    [ Specify browser: Chrome / Firefox ]\n'
           f'-c | --clean      [ Convert mobile sites to regular site ]\n'
           f'-d | --directory  [ Location where the images will be saved ]\n'
           f'     --dpi        [ DPI for the image ]\n'
+          f'-e | --executor   [ Execution environment: Local / Selenoid Host|Selenoid URL ]\n'
           f'-f | --file       [ Text file to read the URLs from ]\n'
           f'-l | --links      [ Comma separated URLs (No spaces) ]\n'
           f'-i | --image-type [ Save images as PNG or JPEG ]\n'
           f'-t | --threads    [ Number of threads to run scrape and download ]\n'
           f'-u | --url-filter [ Only filter for specific files that contain this string ]\n'
           f'-z | --zoom       [ The zoom to use on the browser ]\n'
           f'\n'
           f'webarchiver -c -f <links_file.txt> '
-          '-l "<URL1, URL2, URL3>" -t <JPEG/PNG> -d "~/Downloads" -z 100 --dpi 1\n')
+          '-l "<URL1, URL2, URL3>" -t <JPEG/PNG> -d "~/Downloads" -z 100 --dpi 1 --browser "Chrome" --executor "selenoid|http://selenoid.com/wd/hub"\n')
 
 
 def main():
     if len(sys.argv) < 2:
         usage()
         sys.exit(2)
     webarchiver(sys.argv[1:])
```

## Comparing `webarchiver-0.7.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx` & `webarchiver-0.8.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx`

 * *Files identical despite different names*

## Comparing `webarchiver-0.7.0.dist-info/LICENSE` & `webarchiver-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webarchiver-0.7.0.dist-info/METADATA` & `webarchiver-0.8.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webarchiver
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python tool that allows you to take multiple full page screenshots of web pages without ads.
 Home-page: https://github.com/Knuckles-Team/webarchiver
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,43 +20,54 @@
 Requires-Dist: Pillow (>=9.3.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2)
 Requires-Dist: piexif (>=1.1.3)
 Requires-Dist: selenium (>=4.7.2)
 Requires-Dist: webdriver-manager (>=3.8.5)
 
 # Webarchiver
-*Version: 0.7.0*
+*Version: 0.8.0*
 
 Python tool that allows you to take full page screenshots of pages without ads
 
 Supports batching by adding multiple links in a text file, or my adding links to command line separated by commas.
 
 ### Requirements:
-- Chrome/Chomium browser
+
+One of the following browsers:
+
+- Chrome/Chromium browser
+- Firefox
+- Selenoid Server
 
 ### Usage:
-| Short Flag | Long Flag    | Description                             |
-|------------|--------------|-----------------------------------------|
-| -h         | --help       | See Usage                               |
-| -c         | --clean      | Convert mobile sites to regular site    |
-| -d         | --directory  | Location where the images will be saved |
-|            | --dpi        | DPI for the image                       |
-| -f         | --file       | Text file to read the URLs from         |
-| -l         | --links      | Comma separated URLs (No spaces)        |
-| -i         | --image-type | Save images as PNG or JPEG              |
-| -t         | --threads    | Number of threads to run concurrently   |
-| -u         | --url-filter | Filter URLs that contain this string    |
-| -z         | --zoom       | The zoom to use on the browser          |
+| Short Flag | Long Flag    | Description                                                 |
+|------------|--------------|-------------------------------------------------------------|
+| -h         | --help       | See Usage                                                   |
+| -b         | --browser    | Specify browser: Chrome / Firefox / Selenoid                |
+| -c         | --clean      | Convert mobile sites to regular site                        |
+| -d         | --directory  | Location where the images will be saved                     |
+|            | --dpi        | DPI for the image                                           |
+| -e         | --executor   | Execution environmment: Local / Selenoid Host\|Selenoid URL |
+| -f         | --file       | Text file to read the URLs from                             |
+| -l         | --links      | Comma separated URLs (No spaces)                            |
+| -i         | --image-type | Save images as PNG or JPEG                                  |
+| -t         | --threads    | Number of threads to run concurrently                       |
+| -u         | --url-filter | Filter URLs that contain this string                        |
+| -z         | --zoom       | The zoom to use on the browser                              |
 
 
 ### Example:
 ```bash
 webarchiver -c -f <links_file.txt> -l "<URL1,URL2,URL3>" -t <JPEG/PNG> -d "~/Downloads" -z 100 --dpi 1
 ```
 
+```bash
+webarchiver -c -f <links_file.txt> -l "<URL1,URL2,URL3>" -t <JPEG/PNG> -d "~/Downloads" -z 100 --dpi 1 --executor "selenoid|http://selenoid.com/wd/hub" --browser "Chrome"
+```
+
 #### Install Instructions
 Install Python Package
 
 ```bash
 python -m pip install webarchiver
 ```
```

## Comparing `webarchiver-0.7.0.dist-info/RECORD` & `webarchiver-0.8.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 webarchiver/__init__.py,sha256=4vtajcsU1T7GG8ZNK4h0c2RSdccz4LDEnNDcOyVwyRc,296
-webarchiver/version.py,sha256=DEpmsreHKLkk1HePeizyVrVAnG3OvqvP-AFKZPao1lc,116
-webarchiver/webarchiver.py,sha256=hM2I4Xu5DBW4hDUiMiaq4jJXXioh3KhNK1W6HLMEIGw,32522
+webarchiver/version.py,sha256=tDDkCMChiJvcYngqfjlW_EaRz0JpbXA3z7tYvqWYe8M,116
+webarchiver/webarchiver.py,sha256=KlhCDiMXstntgr7pRrn3euAPYidCyCTKVmMa9UsVOCE,39135
 webarchiver/lib/uBlock-Origin_v1.27.0.crx,sha256=Zgb-gLVb4PTPguapI8G7Tm7v6PwPWgCPrAaTakFAsgg,2984341
-webarchiver-0.7.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx,sha256=Zgb-gLVb4PTPguapI8G7Tm7v6PwPWgCPrAaTakFAsgg,2984341
-webarchiver-0.7.0.dist-info/LICENSE,sha256=awOCsWJ58m_2kBQwBUGWejVqZm6wuRtCL2hi9rfa0X4,1211
-webarchiver-0.7.0.dist-info/METADATA,sha256=kdFK63-jv0-Ry9DLesB5FOcI4dkRDhDvRR_2toqXfS8,2625
-webarchiver-0.7.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-webarchiver-0.7.0.dist-info/entry_points.txt,sha256=wQykdZtGZ3VxOnateyqCvbK47KNgFNrmh6d2Pyw6i64,62
-webarchiver-0.7.0.dist-info/top_level.txt,sha256=MUnVdeIutFBKKfK08DiNEpZhyb8UbmnX8jhFa49vPUA,12
-webarchiver-0.7.0.dist-info/RECORD,,
+webarchiver-0.8.0.data/data/webarchiver/uBlock-Origin_v1.27.0.crx,sha256=Zgb-gLVb4PTPguapI8G7Tm7v6PwPWgCPrAaTakFAsgg,2984341
+webarchiver-0.8.0.dist-info/LICENSE,sha256=awOCsWJ58m_2kBQwBUGWejVqZm6wuRtCL2hi9rfa0X4,1211
+webarchiver-0.8.0.dist-info/METADATA,sha256=XoztwwPH49gViiOTt5zRLwjtn6XXWjjvXr1uGydDXEE,3295
+webarchiver-0.8.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+webarchiver-0.8.0.dist-info/entry_points.txt,sha256=wQykdZtGZ3VxOnateyqCvbK47KNgFNrmh6d2Pyw6i64,62
+webarchiver-0.8.0.dist-info/top_level.txt,sha256=MUnVdeIutFBKKfK08DiNEpZhyb8UbmnX8jhFa49vPUA,12
+webarchiver-0.8.0.dist-info/RECORD,,
```

