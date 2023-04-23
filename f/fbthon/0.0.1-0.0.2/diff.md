# Comparing `tmp/fbthon-0.0.1.tar.gz` & `tmp/fbthon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbthon-0.0.1.tar", last modified: Thu Mar 23 00:41:06 2023, max compression
+gzip compressed data, was "fbthon-0.0.2.tar", last modified: Sun Apr 23 05:29:44 2023, max compression
```

## Comparing `fbthon-0.0.1.tar` & `fbthon-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-03-23 00:41:06.397000 fbthon-0.0.1/
--rw-rw----   0 root         (0) everybody  (9997)     1067 2023-03-22 20:42:21.000000 fbthon-0.0.1/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)    20120 2023-03-23 00:41:06.397000 fbthon-0.0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)    19516 2023-03-23 00:37:18.000000 fbthon-0.0.1/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-03-23 00:41:06.373000 fbthon-0.0.1/fbthon/
--rw-rw----   0 root         (0) everybody  (9997)    27769 2023-03-23 00:16:59.000000 fbthon-0.0.1/fbthon/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      268 2023-03-04 23:56:19.000000 fbthon-0.0.1/fbthon/__version__.py
--rw-rw----   0 root         (0) everybody  (9997)    10458 2023-03-22 17:23:30.000000 fbthon-0.0.1/fbthon/chats.py
--rw-rw----   0 root         (0) everybody  (9997)     7477 2023-03-05 00:42:51.000000 fbthon-0.0.1/fbthon/comments.py
--rw-rw----   0 root         (0) everybody  (9997)      648 2022-12-11 05:43:17.000000 fbthon-0.0.1/fbthon/exceptions.py
--rw-rw----   0 root         (0) everybody  (9997)     8855 2023-03-21 01:36:53.000000 fbthon-0.0.1/fbthon/login.py
--rw-rw----   0 root         (0) everybody  (9997)     5461 2023-03-18 02:25:07.000000 fbthon-0.0.1/fbthon/messenger.py
--rw-rw----   0 root         (0) everybody  (9997)    11327 2023-03-21 22:30:34.000000 fbthon-0.0.1/fbthon/posts.py
--rw-rw----   0 root         (0) everybody  (9997)     4547 2023-03-22 16:53:18.000000 fbthon-0.0.1/fbthon/settings.py
--rw-rw----   0 root         (0) everybody  (9997)    29197 2023-03-18 03:07:21.000000 fbthon-0.0.1/fbthon/user.py
--rw-rw----   0 root         (0) everybody  (9997)      804 2023-03-09 11:25:10.000000 fbthon-0.0.1/fbthon/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-03-23 00:41:06.397000 fbthon-0.0.1/fbthon.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    20120 2023-03-23 00:41:06.000000 fbthon-0.0.1/fbthon.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      384 2023-03-23 00:41:06.000000 fbthon-0.0.1/fbthon.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-03-23 00:41:06.000000 fbthon-0.0.1/fbthon.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       13 2023-03-23 00:41:06.000000 fbthon-0.0.1/fbthon.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-03-23 00:41:06.000000 fbthon-0.0.1/fbthon.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-03-23 00:41:06.401000 fbthon-0.0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1792 2023-03-15 07:57:00.000000 fbthon-0.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-23 05:29:44.422629 fbthon-0.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1068 2023-03-30 15:10:39.000000 fbthon-0.0.2/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)    26634 2023-04-23 05:29:44.426630 fbthon-0.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)    26203 2023-04-22 12:18:49.000000 fbthon-0.0.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-23 05:29:44.418630 fbthon-0.0.2/fbthon/
+-rw-rw----   0 root         (0) everybody  (9997)    31411 2023-04-23 05:17:42.000000 fbthon-0.0.2/fbthon/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)      268 2023-04-03 14:34:35.000000 fbthon-0.0.2/fbthon/__version__.py
+-rw-rw----   0 root         (0) everybody  (9997)    11706 2023-04-18 14:42:25.000000 fbthon-0.0.2/fbthon/chats.py
+-rw-rw----   0 root         (0) everybody  (9997)     7527 2023-04-09 03:21:44.000000 fbthon-0.0.2/fbthon/comments.py
+-rw-rw----   0 root         (0) everybody  (9997)     7861 2023-04-16 13:41:07.000000 fbthon-0.0.2/fbthon/createaccount.py
+-rw-rw----   0 root         (0) everybody  (9997)      648 2023-03-30 15:10:39.000000 fbthon-0.0.2/fbthon/exceptions.py
+-rw-rw----   0 root         (0) everybody  (9997)     8853 2023-03-30 15:10:39.000000 fbthon-0.0.2/fbthon/login.py
+-rw-rw----   0 root         (0) everybody  (9997)     5466 2023-04-08 02:55:28.000000 fbthon-0.0.2/fbthon/messenger.py
+-rw-rw----   0 root         (0) everybody  (9997)    16872 2023-04-09 03:24:45.000000 fbthon-0.0.2/fbthon/posts.py
+-rw-rw----   0 root         (0) everybody  (9997)     5819 2023-04-08 02:46:06.000000 fbthon-0.0.2/fbthon/settings.py
+-rw-rw----   0 root         (0) everybody  (9997)    29070 2023-04-09 03:24:04.000000 fbthon-0.0.2/fbthon/user.py
+-rw-rw----   0 root         (0) everybody  (9997)     2310 2023-04-07 06:01:05.000000 fbthon-0.0.2/fbthon/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-23 05:29:44.422629 fbthon-0.0.2/fbthon.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    26634 2023-04-23 05:29:44.000000 fbthon-0.0.2/fbthon.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      408 2023-04-23 05:29:44.000000 fbthon-0.0.2/fbthon.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-23 05:29:44.000000 fbthon-0.0.2/fbthon.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       31 2023-04-23 05:29:44.000000 fbthon-0.0.2/fbthon.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-04-23 05:29:44.000000 fbthon-0.0.2/fbthon.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       79 2023-04-23 05:29:44.426630 fbthon-0.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1823 2023-04-01 11:23:40.000000 fbthon-0.0.2/setup.py
```

### Comparing `fbthon-0.0.1/LICENSE` & `fbthon-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `fbthon-0.0.1/PKG-INFO` & `fbthon-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbthon
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Facebook scraper
 Home-page: https://github.com/MR-X-Junior/fbthon
 Author: Rahmat adha
 Author-email: rahmadadha11@gmail.com
 License: MIT
 Keywords: facebook-scraper,facebook-parser,facebook-scraper-without-apikey
 Classifier: Development Status :: 3 - Alpha
@@ -27,16 +27,16 @@
 
 **fbthon** adalah library sederhana yang di gunakan untuk scraping web Facebook
 
 # Informasi Library
 *Author :* [**Rahmat adha**](https://facebook.com/Anjay.pro098)\
 *Library :* [**fbthon**](https://github.com/MR-X-Junior/fbthon)\
 *License:* [**MIT License**](https://github.com/MR-X-junior/fbthon/blob/main/LICENSE)\
-*Release:* **23**/03/20**23**\
-*Version :* **0.0.1**
+*Release:* **23**/04/20**23**\
+*Version :* **0.0.2**
 
 Di karenakan library ini masih versi pertama, pasti bakal banyak error/bug nya, jika menemukan error/bug pada library ini bisa langsung posting di [Issues](https://github.com/MR-X-junior/fbthon/issues) akun github saya :)
 
 ## Contoh Cara Penggunaan
 
 ### Pertama-tama buat dulu object `Facebook`
 
@@ -46,29 +46,29 @@
 >>> fb = Facebook(cookie)
 ```
 
 ### Jika tidak tidak mempunyai Cookie akun facebook, kamu bisa coba cara di bawah ini
 
 ```python
 >>> from fbthon import Facebook
->>> from fbthon.login import Web_Login
+>>> from fbthon import Web_Login
 >>> email = "example@gmail.com" # Ganti email ini dengan email akun Facebook kamu
 >>> password = "Banteng merah no counter321" # Ganti password ini dengan password Akun Facebook kamu
 >>> login = Web_Login(email,password)
 >>> cookie = login.get_cookie_str() # Ini adalah cookie akun Facebook kamu
 >>> fb = Facebook(cookie)
 ```
 
 Cara di [atas](#Jika-tidak-tidak-mempunyai-Cookie-akun-facebook-kamu-bisa-coba-cara-di-bawah-ini) akan login ke akun facebook, cara ini mungkin akan membuat akun facebook kamu terkena checkpoint.
 
 Untuk mengurangi risiko akun terkena checkpoint, kamu hanya perlu mengganti user-agent yang sama dengan perangkat yang terakhir kali di gunakan untuk login akun facebook.
 
 ```python
 >>> from fbthon import Facebook
->>> from fbthon.login import Web_Login
+>>> from fbthon import Web_Login
 >>> user_agent = {'User-Agent':'Mozilla/5.0 (Linux; Android 6.0.1; SM-J510GN Build/MMB29M) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.111 Mobile Safari/537.36'}
 >>> email = "example@gmail.com" # Ganti email ini dengan email akun Facebook kamu
 >>> password = "Banteng merah no counter321" # Ganti password ini dengan password Akun Facebook kamu
 >>> login = Web_Login(email,password, headers = user_agent)
 >>> cookie = login.get_cookie_str() # Ini adalah cookie akun Facebook kamu
 >>> fb = Facebook(cookie)
 ```
@@ -107,14 +107,64 @@
 100053033144051
 >>> my_profile.username
 /Anjay.pro098
 >>> my_profile._user_info
 {'name': 'Rahmat', 'first_name': 'Rahmat', 'middle_name': '', 'last_name': '', 'alternate_name': 'Mat', 'about': '', 'username': '/Anjay.pro098', 'id': '100053033144051', 'contact_info': {'Ponsel': '0857-5462-9509', 'Facebook': '/Anjay.pro098', 'GitHub': 'MR-X-Junior', 'LinkedIn': 'rahmat-adha', 'Email': 'rahmadadha11@gmail.com'}, 'profile_pict': 'https://z-m-scontent.fsri1-1.fna.fbcdn.net/v/t39.30808-1/279908382_524601785984255_7727931677642432211_n.jpg?stp=cp0_dst-jpg_e15_p480x480_q65&_nc_cat=109&ccb=1-7&_nc_sid=dbb9e7&efg=eyJpIjoiYiJ9&_nc_eui2=AeEUCqxtmlmkSmx4EruhJj1ZoWFvcSuRApChYW9xK5ECkKEzjdDols3I7WDmPnas34nC8SsOQFYFy3zM38AIJfS1&_nc_ohc=XqfoPIkQwfkAX9oxiI4&tn=CoPUyHV9TcgsBjnY&_nc_ad=z-m&_nc_cid=1225&_nc_eh=4613fe15e78ad080e57d79ac328ba3a7&_nc_rml=0&_nc_ht=z-m-scontent.fsri1-1.fna&oh=00_AfByqAVLNVMSOfwr6pe43Iwr3HpWeVg0qImeiROkpw53rw&oe=63FCE8CF', 'basic_info': {'Tanggal Lahir': '13 Januari 2006', 'Jenis Kelamin': 'Laki-laki'}, 'education': [{'name': '', 'type': '', 'study': '', 'time': ''}], 'work': [], 'living': [{'Kota Saat Ini': 'Muaraancalung, Kalimantan Timur, Indonesia', 'Kota asal': 'Muaraancalung, Kalimantan Timur, Indonesia'}], 'relationship': 'Lajang', 'other_name': {'Nama panggilan': 'Met'}, 'family': [{'name': 'Pahrul Aguspriana XD.', 'username': '/PahrulXD', 'designation': 'Adik laki-laki', 'profile_pict': 'https://z-m-scontent.fsri1-1.fna.fbcdn.net/v/t39.30808-1/331028920_3040847712882567_3539568768564278719_n.jpg?stp=c0.0.320.320a_cp0_dst-jpg_e15_p320x320_q65&_nc_cat=101&ccb=1-7&_nc_sid=dbb9e7&efg=eyJpIjoiYiJ9&_nc_eui2=AeEW2pBM_jo0ZzypEALp1QB7eG7Nm80Gj5J4bs2bzQaPkmGYk_gZVtPSzsrb1SX796_BwslIoWRa_4yIuFC3x1Fh&_nc_ohc=NjtS1hHD7GcAX9Sp4HY&_nc_ad=z-m&_nc_cid=1225&_nc_eh=4613fe15e78ad080e57d79ac328ba3a7&_nc_rml=0&_nc_ht=z-m-scontent.fsri1-1.fna&oh=00_AfBGUpSnDzv3tHfsng6gWLn2ZGjNwSaFXzDLeCnlWv9Lsg&oe=63FDEBC2'}], 'year_overviews': [], 'quote': "i know i'm not alone"}
 ```
 
+### Update Profile Picture
+Kamu bisa menggunakan function `UpdateProfilePicture` untuk mengganti poto profile akun Facebook kamu.
+
+**Contoh:**
+
+```python
+from fbthon import settings
+from fbthon import Facebook
+
+fb = Facebook("datr=klr23aug21xxxxxxx") # Cookie Akun Facebook 
+
+settings.UpdateProfilePicture(fb, photo = '/sdcard/DCIM/Orang-Susah.jpg')
+```
+
+#### Hasilnya
+
+##### Sebelum 
+
+![Before Update Profile Picture](https://i.ibb.co/tzpq34P/IMG-20230419-202908.jpg)
+
+##### Sesudah
+
+![After Update Profile Picture](https://i.ibb.co/wJCp0HD/IMG-20230419-203029.jpg)
+
+### Get Notifications
+Kamu bisa menggunakan method `get_notifications` untuk mendapatkan notifikasi terbaru dari akun Facebook.
+
+**Contoh:**
+
+```python
+no = fb.get_notifications(limit = 2)
+
+for chaa in no:
+  print ("Message : "+ chaa['message'])
+  print ("Time : "+ chaa['time'])
+  print ("Redirect URL : "+ chaa['redirect_url'] + "\n")
+```
+
+**Output:**
+
+```
+Message : Berdasarkan halaman yang berinteraksi dengan Anda, Anda mungkin menyukai Meme Upin Ipin Comic Lucu.                               
+Time : 11 Apr                                                         
+Redirect URL : https://mbasic.facebook.com/a/notifications.php?redir=%2Fgroups%2F426298749190770%2F&seennotification=1681152051803754&eav=AfbWn5_N4XPZ0dL2bdBlHmCJIqmlGanPyx8_K3EuoQ47EREpeYdQtHn-1DmRfQaTNE0&gfid=AQDZ4pcYOl5JlPJd0uw&paipv=0&refid=48                                 
+
+Message : Berdasarkan halaman yang berinteraksi dengan Anda, Anda mungkin menyukai Mukbang Yummy Food.                                      
+Time : 8 Apr
+Redirect URL : https://mbasic.facebook.com/a/notifications.php?redir=%2Fgroups%2F340989278132975%2F&seennotification=1680900355646527&eav=AfZlnRarakilRKNOhz6fPULFLUjDyccZvOhpJFhWEAy2un9H6EbgdPZ7Zii39UuMazc&gfid=AQBuf1_B6NbYKhXjCv8&paipv=0&refid=48
+```
+
 ### Get Posts
 
 Method `get_posts`, akan mengumpulkan postingan dan mengekstrak postingan tersebut, method ini akan mengembalikan `list` yang di dalam nya terdapat sekumpulan object  `Posts`
 
 **CATATAN: METHOD INI HANYA BISA MENGUMPULKAN POSTINGAN DARI AKUN PENGGUNA, TIDAK BISA MENGUMPULKAN POSTINGAN DARI GROUP ATAU HALAMAN.**
 ```python
 for x in fb.get_posts('zuck', limit = 2):
@@ -169,14 +219,30 @@
 ```
 
 ##### Hasilnya
 **Liat Komentar paling bawah**
 
 ![Contoh cara mengirim komentar](https://i.ibb.co/QFDpnw9/Screenshot-20230322-064024.jpg)
 
+Untuk menambahkan foto pada komentar, kamu bisa menggunakan argument `file`
+
+**Contoh:**
+
+```python
+>>> post = fb.post_parser('https://m.facebook.com/story.php?story_fbid=pfbid02kTobxSiD9buMUEjrq57FFnhQ6FJyGnafmNhMimoaamoAwuECAjboYaB6mE7C7pPZl&id=100053033144051&mibextid=Nif5oz')
+>>> post.send_comment("Komentar ini tidak di sertai dengan foto!")
+True
+>>> post.send_comment("Komentar ini di sertai dengan foto!", file = "/sdcard/DCIM/Facebook/FB_IMG_1681559707400.jpg")
+True
+```
+
+##### Hasilnya
+
+![Contoh cara mengirim komentar dengan foto](https://i.ibb.co/6vd6BQc/IMG-20230418-110223.jpg)
+
 #### Memberikan react pada postingan
 
 Kamu bisa menggunakan method `send_react` untuk memberikan react pada postingan.
 Method ini akan mengembalikan `True` jika berhasil memberikan react pada postingan.
 
 ```python
 >>> post = fb.post_parser(Link_post_facebook)
@@ -199,28 +265,54 @@
 >>> post.send_react('Wow')
 True
 ```
 
 ##### Hasilnya
 ![Contoh cara memberikan react ke postingan](https://i.ibb.co/SPXGWJJ/Screenshot-2023-0322-065521.png)
 
+##### Membagikan Postingan
+Kamu bisa menggunakan method `share_post` untuk membagikan postingan seseorang ke akun Facebook kamu.
+
+**Contoh (1):**
+
+```python
+post = fb.post_parser("https://m.facebook.com/story.php?story_fbid=pfbid0gxnxN5dZDDA93S2GveyxqgSzEdYdAtdE32PYyAd7iftDS7yBHprBACc9VcFXDoPtl&id=100053033144051&mibextid=Nif5oz")
+post.share_post()
+```
+
+##### Hasilnya
+
+![Contoh cara membagikan postingan](https://i.ibb.co/F39c30w/IMG-20230419-064244.jpg)
+
+**Contoh (2):**
+
+Kamu juga bisa menambahkan `message`,`location` dan `feeling` pada postingan yang di bagikan.
+
+```python
+post = fb.post_parser("https://m.facebook.com/story.php?story_fbid=pfbid0gxnxN5dZDDA93S2GveyxqgSzEdYdAtdE32PYyAd7iftDS7yBHprBACc9VcFXDoPtl&id=100053033144051&mibextid=Nif5oz")
+post.share_post(message = "Postingan ini di bagikan menggunakan library fbthon", location = "Kuningan Timur", feeling = "Happy")
+```
+
+##### Hasilnya
+![Contoh cara membagikan postingan dengan message,location, dan feeling](https://i.ibb.co/7J1wzB2/IMG-20230419-070541.jpg)
+
 ### Messenger
 
 object `Messenger` bisa di gunakan untuk mengirim/menerima chat.\
 Terdapat 2 cara untuk membuat Object `Messenger`
 
 **Cara 1**
 
 ```python
 >>> msg = fb.Messenger()
 ```
 **Cara 2**
 
 ```python
->>> from fbthon.messenger import Messenger
+>>> from fbthon import Messenger
 >>> msg = Messenger(Cookie_Akun_Facebook_kamu)
 ```
 
 
 #### Mendapatkan Pesan Baru
 Method `get_new_message` bisa di gunakan untuk mendapatkan pesan baru:)
 
@@ -277,14 +369,29 @@
   chat.send_text('Apa kabar?')
   chat.send_text('Pesan ini di kirim menggunakan library fbthon:)\n\nTerima kasih Sudah membaca chat saya.')
 ```
 
 ##### Hasilnya
 ![Contoh Cara Mengirim Pesan](https://i.ibb.co/fQHtDmb/Screenshot-20230317-222932.jpg)
 
+Kamu bisa menggunakan method `send_image` untuk mengirim chat dengan foto.
+
+**Contoh:**
+
+```python
+with msg.new_chat("Anjay.pro098") as chat:
+  chat.send_text("Hallo kak "+chat.name)
+  chat.send_text("Pesan ini di kirim menggunakan library fbthon :)")
+  chat.send_image(file = "/sdcard/DCIM/Facebook/FB_IMG_1681559707400.jpg",message = "Aku ketika nunggu buka puasa : ")
+  chat.send_like_stiker()
+```
+
+##### Hasilnya
+![Contoh Cara mengirim chat dengan foto](https://i.ibb.co/FVgZ7Mf/IMG-20230418-184806.jpg)
+
 ## Membuat Postingan
 method `create_timeline` bisa di gunakan untuk membuat postingan, method ini akan mengembalikan `True` jika berhasil membuat postingan.
 
 ### Membuat Postingan (Hanya Caption)
 
 ```python
 >>> fb.create_timeline(target = 'me', message = 'Postingan Ini di buat menggunakan library fbthon\n\nHehe :>')
@@ -363,19 +470,83 @@
 >>> fb.create_timeline(target = 'me', message = 'Postingan Ini di buat menggunakan library fbthon\n\nHehe :>', feeling = 'Happy')
 True
 ```
 
 #### Hasilnya
 ![Membuat Postingan (Dengan Feeling)](https://i.ibb.co/n7yp62b/Screenshot-2023-0318-152335.png)
 
+### Create a facebook account
+Kamu bisa menggunakan class `CreateAccount` untuk membuat akun Facebook.
+
+**CATATAN: Fitur ini masih dalam tahap percobaan, jadi kemungkinan besar fitur ini tidak akan bekerja dengan baik.**
+
+#### Contoh:
+
+Di bawah ini adalah program sederhana untuk membuat akun Facebook.
+
+```python
+from fbthon import CreateAccount
+
+print ("[+] Daftar Akun Facebook [+]\n")
+
+firstname = input("[?] Nama Depan : ") # Nama Depan
+lastname = input("[?] Nama Belakang : ") # Nama Belakang
+email = input("[?] Email/Phone : ") # Alamat email / No Hp
+gender = input("[?] Jenis Kelamin(Male/Female): ") # Gender
+ultah = input("[?] Tanggal Lahir (DD/MM/YYYY): ") # Tanggal lahir
+password = input("[?] Password : ")  # Kata Sandi
+
+new_account = CreateAccount(firstname = firstname, lastname = lastname, email = email, gender = gender, date_of_birth = ultah, password = password)
+
+print ("\n[+] Masukkan Kode Verifikasi yang sudah di kirim ke "+ email)
+kode = input("[?] Kode Verifikasi : ")
+
+# Method `confirm_account` akan mengembalikan `True` Jika berhasil mengkonfirmasi akun.
+konfir = new_account.confirm_account(kode)
+
+if konfir:
+  print ("[✓] Berhasil Membuat Akun Facebook :)\n")
+  print ("[+] Nama Akun : %s %s" % (firstname,lastname))
+  print ("[+] ID Akun : %s" % (new_account.get_cookie_dict()['c_user']))
+  print ("[+] Email/Phone : %s" % (email))
+  print ("[+] Jenis Kelamin : %s" % (gender))
+  print ("[+] Tanggal lahir : %s" % (ultah))
+  print ("[+] Password : %s" % (password))
+  print ("[+] Cookie Akun : %s" % (new_account.get_cookie_str()))
+  print ("[+] Token Akun : %s" % (new_account.get_token()))
+  sys.exit(0)
+else:
+  print ("[!] Gagal Membuat Akun Facebook ")
+  sys.exit(1)
+```
+
+##### Jalankan Program nya
+![Menjalankan script Contoh cara membuat akun Facebook menggunakan library fbthon](https://i.ibb.co/2Sd19Wc/Screenshot-2023-0420-093249.png)
+
+###### Hasilnya 
+Ini adalah akun yang di buat menggunakan library fbthon:)
+
+![Ini adalah akun Facebook yang di buat menggunakan library fbthon](https://i.ibb.co/7K3q3hj/Screenshot-20230420-093826.jpg)
+
+#### Optional Parameter
+*(Untuk `CreateAccount` class)*.
+
+- **firstname**: Nama Depan
+- **lastname**: Nama Belakang
+- **email**: Alamat email yang akan di gunakan untuk mendaftar akun facebook, kamu juga bisa menggunakan nomor ponsel sebagai pengganti alamat email.
+- **gender**: Jenis kelamin (Male/Female)
+- **date_of_birth**: Tanggal lahir, untuk format tanggal lahir nya adalah DD/MM/YYYY, Contoh: 13/01/2006
+- **password**: Kata sandi yang akan di gunakan untuk membuat akun Facebook.
+
+
 # Cara Install
 
 **fbthon** sudah tersedia di PyPi
 
 ```console
 $ python -m pip install fbthon
 ```
 
-**fbthon** bisa install di Python versi 3.7+
+**fbthon** bisa di install di Python versi 3.7+
 
 # Donate
 [![Donate for Rahmat adha](https://i.ibb.co/PwYMWsK/Saweria-Logo.png)](https://saweria.co/rahmatadha)
```

### Comparing `fbthon-0.0.1/README.md` & `fbthon-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 **fbthon** adalah library sederhana yang di gunakan untuk scraping web Facebook
 
 # Informasi Library
 *Author :* [**Rahmat adha**](https://facebook.com/Anjay.pro098)\
 *Library :* [**fbthon**](https://github.com/MR-X-Junior/fbthon)\
 *License:* [**MIT License**](https://github.com/MR-X-junior/fbthon/blob/main/LICENSE)\
-*Release:* **23**/03/20**23**\
-*Version :* **0.0.1**
+*Release:* **23**/04/20**23**\
+*Version :* **0.0.2**
 
 Di karenakan library ini masih versi pertama, pasti bakal banyak error/bug nya, jika menemukan error/bug pada library ini bisa langsung posting di [Issues](https://github.com/MR-X-junior/fbthon/issues) akun github saya :)
 
 ## Contoh Cara Penggunaan
 
 ### Pertama-tama buat dulu object `Facebook`
 
@@ -21,29 +21,29 @@
 >>> fb = Facebook(cookie)
 ```
 
 ### Jika tidak tidak mempunyai Cookie akun facebook, kamu bisa coba cara di bawah ini
 
 ```python
 >>> from fbthon import Facebook
->>> from fbthon.login import Web_Login
+>>> from fbthon import Web_Login
 >>> email = "example@gmail.com" # Ganti email ini dengan email akun Facebook kamu
 >>> password = "Banteng merah no counter321" # Ganti password ini dengan password Akun Facebook kamu
 >>> login = Web_Login(email,password)
 >>> cookie = login.get_cookie_str() # Ini adalah cookie akun Facebook kamu
 >>> fb = Facebook(cookie)
 ```
 
 Cara di [atas](#Jika-tidak-tidak-mempunyai-Cookie-akun-facebook-kamu-bisa-coba-cara-di-bawah-ini) akan login ke akun facebook, cara ini mungkin akan membuat akun facebook kamu terkena checkpoint.
 
 Untuk mengurangi risiko akun terkena checkpoint, kamu hanya perlu mengganti user-agent yang sama dengan perangkat yang terakhir kali di gunakan untuk login akun facebook.
 
 ```python
 >>> from fbthon import Facebook
->>> from fbthon.login import Web_Login
+>>> from fbthon import Web_Login
 >>> user_agent = {'User-Agent':'Mozilla/5.0 (Linux; Android 6.0.1; SM-J510GN Build/MMB29M) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.111 Mobile Safari/537.36'}
 >>> email = "example@gmail.com" # Ganti email ini dengan email akun Facebook kamu
 >>> password = "Banteng merah no counter321" # Ganti password ini dengan password Akun Facebook kamu
 >>> login = Web_Login(email,password, headers = user_agent)
 >>> cookie = login.get_cookie_str() # Ini adalah cookie akun Facebook kamu
 >>> fb = Facebook(cookie)
 ```
@@ -82,14 +82,64 @@
 100053033144051
 >>> my_profile.username
 /Anjay.pro098
 >>> my_profile._user_info
 {'name': 'Rahmat', 'first_name': 'Rahmat', 'middle_name': '', 'last_name': '', 'alternate_name': 'Mat', 'about': '', 'username': '/Anjay.pro098', 'id': '100053033144051', 'contact_info': {'Ponsel': '0857-5462-9509', 'Facebook': '/Anjay.pro098', 'GitHub': 'MR-X-Junior', 'LinkedIn': 'rahmat-adha', 'Email': 'rahmadadha11@gmail.com'}, 'profile_pict': 'https://z-m-scontent.fsri1-1.fna.fbcdn.net/v/t39.30808-1/279908382_524601785984255_7727931677642432211_n.jpg?stp=cp0_dst-jpg_e15_p480x480_q65&_nc_cat=109&ccb=1-7&_nc_sid=dbb9e7&efg=eyJpIjoiYiJ9&_nc_eui2=AeEUCqxtmlmkSmx4EruhJj1ZoWFvcSuRApChYW9xK5ECkKEzjdDols3I7WDmPnas34nC8SsOQFYFy3zM38AIJfS1&_nc_ohc=XqfoPIkQwfkAX9oxiI4&tn=CoPUyHV9TcgsBjnY&_nc_ad=z-m&_nc_cid=1225&_nc_eh=4613fe15e78ad080e57d79ac328ba3a7&_nc_rml=0&_nc_ht=z-m-scontent.fsri1-1.fna&oh=00_AfByqAVLNVMSOfwr6pe43Iwr3HpWeVg0qImeiROkpw53rw&oe=63FCE8CF', 'basic_info': {'Tanggal Lahir': '13 Januari 2006', 'Jenis Kelamin': 'Laki-laki'}, 'education': [{'name': '', 'type': '', 'study': '', 'time': ''}], 'work': [], 'living': [{'Kota Saat Ini': 'Muaraancalung, Kalimantan Timur, Indonesia', 'Kota asal': 'Muaraancalung, Kalimantan Timur, Indonesia'}], 'relationship': 'Lajang', 'other_name': {'Nama panggilan': 'Met'}, 'family': [{'name': 'Pahrul Aguspriana XD.', 'username': '/PahrulXD', 'designation': 'Adik laki-laki', 'profile_pict': 'https://z-m-scontent.fsri1-1.fna.fbcdn.net/v/t39.30808-1/331028920_3040847712882567_3539568768564278719_n.jpg?stp=c0.0.320.320a_cp0_dst-jpg_e15_p320x320_q65&_nc_cat=101&ccb=1-7&_nc_sid=dbb9e7&efg=eyJpIjoiYiJ9&_nc_eui2=AeEW2pBM_jo0ZzypEALp1QB7eG7Nm80Gj5J4bs2bzQaPkmGYk_gZVtPSzsrb1SX796_BwslIoWRa_4yIuFC3x1Fh&_nc_ohc=NjtS1hHD7GcAX9Sp4HY&_nc_ad=z-m&_nc_cid=1225&_nc_eh=4613fe15e78ad080e57d79ac328ba3a7&_nc_rml=0&_nc_ht=z-m-scontent.fsri1-1.fna&oh=00_AfBGUpSnDzv3tHfsng6gWLn2ZGjNwSaFXzDLeCnlWv9Lsg&oe=63FDEBC2'}], 'year_overviews': [], 'quote': "i know i'm not alone"}
 ```
 
+### Update Profile Picture
+Kamu bisa menggunakan function `UpdateProfilePicture` untuk mengganti poto profile akun Facebook kamu.
+
+**Contoh:**
+
+```python
+from fbthon import settings
+from fbthon import Facebook
+
+fb = Facebook("datr=klr23aug21xxxxxxx") # Cookie Akun Facebook 
+
+settings.UpdateProfilePicture(fb, photo = '/sdcard/DCIM/Orang-Susah.jpg')
+```
+
+#### Hasilnya
+
+##### Sebelum 
+
+![Before Update Profile Picture](https://i.ibb.co/tzpq34P/IMG-20230419-202908.jpg)
+
+##### Sesudah
+
+![After Update Profile Picture](https://i.ibb.co/wJCp0HD/IMG-20230419-203029.jpg)
+
+### Get Notifications
+Kamu bisa menggunakan method `get_notifications` untuk mendapatkan notifikasi terbaru dari akun Facebook.
+
+**Contoh:**
+
+```python
+no = fb.get_notifications(limit = 2)
+
+for chaa in no:
+  print ("Message : "+ chaa['message'])
+  print ("Time : "+ chaa['time'])
+  print ("Redirect URL : "+ chaa['redirect_url'] + "\n")
+```
+
+**Output:**
+
+```
+Message : Berdasarkan halaman yang berinteraksi dengan Anda, Anda mungkin menyukai Meme Upin Ipin Comic Lucu.                               
+Time : 11 Apr                                                         
+Redirect URL : https://mbasic.facebook.com/a/notifications.php?redir=%2Fgroups%2F426298749190770%2F&seennotification=1681152051803754&eav=AfbWn5_N4XPZ0dL2bdBlHmCJIqmlGanPyx8_K3EuoQ47EREpeYdQtHn-1DmRfQaTNE0&gfid=AQDZ4pcYOl5JlPJd0uw&paipv=0&refid=48                                 
+
+Message : Berdasarkan halaman yang berinteraksi dengan Anda, Anda mungkin menyukai Mukbang Yummy Food.                                      
+Time : 8 Apr
+Redirect URL : https://mbasic.facebook.com/a/notifications.php?redir=%2Fgroups%2F340989278132975%2F&seennotification=1680900355646527&eav=AfZlnRarakilRKNOhz6fPULFLUjDyccZvOhpJFhWEAy2un9H6EbgdPZ7Zii39UuMazc&gfid=AQBuf1_B6NbYKhXjCv8&paipv=0&refid=48
+```
+
 ### Get Posts
 
 Method `get_posts`, akan mengumpulkan postingan dan mengekstrak postingan tersebut, method ini akan mengembalikan `list` yang di dalam nya terdapat sekumpulan object  `Posts`
 
 **CATATAN: METHOD INI HANYA BISA MENGUMPULKAN POSTINGAN DARI AKUN PENGGUNA, TIDAK BISA MENGUMPULKAN POSTINGAN DARI GROUP ATAU HALAMAN.**
 ```python
 for x in fb.get_posts('zuck', limit = 2):
@@ -144,14 +194,30 @@
 ```
 
 ##### Hasilnya
 **Liat Komentar paling bawah**
 
 ![Contoh cara mengirim komentar](https://i.ibb.co/QFDpnw9/Screenshot-20230322-064024.jpg)
 
+Untuk menambahkan foto pada komentar, kamu bisa menggunakan argument `file`
+
+**Contoh:**
+
+```python
+>>> post = fb.post_parser('https://m.facebook.com/story.php?story_fbid=pfbid02kTobxSiD9buMUEjrq57FFnhQ6FJyGnafmNhMimoaamoAwuECAjboYaB6mE7C7pPZl&id=100053033144051&mibextid=Nif5oz')
+>>> post.send_comment("Komentar ini tidak di sertai dengan foto!")
+True
+>>> post.send_comment("Komentar ini di sertai dengan foto!", file = "/sdcard/DCIM/Facebook/FB_IMG_1681559707400.jpg")
+True
+```
+
+##### Hasilnya
+
+![Contoh cara mengirim komentar dengan foto](https://i.ibb.co/6vd6BQc/IMG-20230418-110223.jpg)
+
 #### Memberikan react pada postingan
 
 Kamu bisa menggunakan method `send_react` untuk memberikan react pada postingan.
 Method ini akan mengembalikan `True` jika berhasil memberikan react pada postingan.
 
 ```python
 >>> post = fb.post_parser(Link_post_facebook)
@@ -174,28 +240,54 @@
 >>> post.send_react('Wow')
 True
 ```
 
 ##### Hasilnya
 ![Contoh cara memberikan react ke postingan](https://i.ibb.co/SPXGWJJ/Screenshot-2023-0322-065521.png)
 
+##### Membagikan Postingan
+Kamu bisa menggunakan method `share_post` untuk membagikan postingan seseorang ke akun Facebook kamu.
+
+**Contoh (1):**
+
+```python
+post = fb.post_parser("https://m.facebook.com/story.php?story_fbid=pfbid0gxnxN5dZDDA93S2GveyxqgSzEdYdAtdE32PYyAd7iftDS7yBHprBACc9VcFXDoPtl&id=100053033144051&mibextid=Nif5oz")
+post.share_post()
+```
+
+##### Hasilnya
+
+![Contoh cara membagikan postingan](https://i.ibb.co/F39c30w/IMG-20230419-064244.jpg)
+
+**Contoh (2):**
+
+Kamu juga bisa menambahkan `message`,`location` dan `feeling` pada postingan yang di bagikan.
+
+```python
+post = fb.post_parser("https://m.facebook.com/story.php?story_fbid=pfbid0gxnxN5dZDDA93S2GveyxqgSzEdYdAtdE32PYyAd7iftDS7yBHprBACc9VcFXDoPtl&id=100053033144051&mibextid=Nif5oz")
+post.share_post(message = "Postingan ini di bagikan menggunakan library fbthon", location = "Kuningan Timur", feeling = "Happy")
+```
+
+##### Hasilnya
+![Contoh cara membagikan postingan dengan message,location, dan feeling](https://i.ibb.co/7J1wzB2/IMG-20230419-070541.jpg)
+
 ### Messenger
 
 object `Messenger` bisa di gunakan untuk mengirim/menerima chat.\
 Terdapat 2 cara untuk membuat Object `Messenger`
 
 **Cara 1**
 
 ```python
 >>> msg = fb.Messenger()
 ```
 **Cara 2**
 
 ```python
->>> from fbthon.messenger import Messenger
+>>> from fbthon import Messenger
 >>> msg = Messenger(Cookie_Akun_Facebook_kamu)
 ```
 
 
 #### Mendapatkan Pesan Baru
 Method `get_new_message` bisa di gunakan untuk mendapatkan pesan baru:)
 
@@ -252,14 +344,29 @@
   chat.send_text('Apa kabar?')
   chat.send_text('Pesan ini di kirim menggunakan library fbthon:)\n\nTerima kasih Sudah membaca chat saya.')
 ```
 
 ##### Hasilnya
 ![Contoh Cara Mengirim Pesan](https://i.ibb.co/fQHtDmb/Screenshot-20230317-222932.jpg)
 
+Kamu bisa menggunakan method `send_image` untuk mengirim chat dengan foto.
+
+**Contoh:**
+
+```python
+with msg.new_chat("Anjay.pro098") as chat:
+  chat.send_text("Hallo kak "+chat.name)
+  chat.send_text("Pesan ini di kirim menggunakan library fbthon :)")
+  chat.send_image(file = "/sdcard/DCIM/Facebook/FB_IMG_1681559707400.jpg",message = "Aku ketika nunggu buka puasa : ")
+  chat.send_like_stiker()
+```
+
+##### Hasilnya
+![Contoh Cara mengirim chat dengan foto](https://i.ibb.co/FVgZ7Mf/IMG-20230418-184806.jpg)
+
 ## Membuat Postingan
 method `create_timeline` bisa di gunakan untuk membuat postingan, method ini akan mengembalikan `True` jika berhasil membuat postingan.
 
 ### Membuat Postingan (Hanya Caption)
 
 ```python
 >>> fb.create_timeline(target = 'me', message = 'Postingan Ini di buat menggunakan library fbthon\n\nHehe :>')
@@ -338,19 +445,83 @@
 >>> fb.create_timeline(target = 'me', message = 'Postingan Ini di buat menggunakan library fbthon\n\nHehe :>', feeling = 'Happy')
 True
 ```
 
 #### Hasilnya
 ![Membuat Postingan (Dengan Feeling)](https://i.ibb.co/n7yp62b/Screenshot-2023-0318-152335.png)
 
+### Create a facebook account
+Kamu bisa menggunakan class `CreateAccount` untuk membuat akun Facebook.
+
+**CATATAN: Fitur ini masih dalam tahap percobaan, jadi kemungkinan besar fitur ini tidak akan bekerja dengan baik.**
+
+#### Contoh:
+
+Di bawah ini adalah program sederhana untuk membuat akun Facebook.
+
+```python
+from fbthon import CreateAccount
+
+print ("[+] Daftar Akun Facebook [+]\n")
+
+firstname = input("[?] Nama Depan : ") # Nama Depan
+lastname = input("[?] Nama Belakang : ") # Nama Belakang
+email = input("[?] Email/Phone : ") # Alamat email / No Hp
+gender = input("[?] Jenis Kelamin(Male/Female): ") # Gender
+ultah = input("[?] Tanggal Lahir (DD/MM/YYYY): ") # Tanggal lahir
+password = input("[?] Password : ")  # Kata Sandi
+
+new_account = CreateAccount(firstname = firstname, lastname = lastname, email = email, gender = gender, date_of_birth = ultah, password = password)
+
+print ("\n[+] Masukkan Kode Verifikasi yang sudah di kirim ke "+ email)
+kode = input("[?] Kode Verifikasi : ")
+
+# Method `confirm_account` akan mengembalikan `True` Jika berhasil mengkonfirmasi akun.
+konfir = new_account.confirm_account(kode)
+
+if konfir:
+  print ("[✓] Berhasil Membuat Akun Facebook :)\n")
+  print ("[+] Nama Akun : %s %s" % (firstname,lastname))
+  print ("[+] ID Akun : %s" % (new_account.get_cookie_dict()['c_user']))
+  print ("[+] Email/Phone : %s" % (email))
+  print ("[+] Jenis Kelamin : %s" % (gender))
+  print ("[+] Tanggal lahir : %s" % (ultah))
+  print ("[+] Password : %s" % (password))
+  print ("[+] Cookie Akun : %s" % (new_account.get_cookie_str()))
+  print ("[+] Token Akun : %s" % (new_account.get_token()))
+  sys.exit(0)
+else:
+  print ("[!] Gagal Membuat Akun Facebook ")
+  sys.exit(1)
+```
+
+##### Jalankan Program nya
+![Menjalankan script Contoh cara membuat akun Facebook menggunakan library fbthon](https://i.ibb.co/2Sd19Wc/Screenshot-2023-0420-093249.png)
+
+###### Hasilnya 
+Ini adalah akun yang di buat menggunakan library fbthon:)
+
+![Ini adalah akun Facebook yang di buat menggunakan library fbthon](https://i.ibb.co/7K3q3hj/Screenshot-20230420-093826.jpg)
+
+#### Optional Parameter
+*(Untuk `CreateAccount` class)*.
+
+- **firstname**: Nama Depan
+- **lastname**: Nama Belakang
+- **email**: Alamat email yang akan di gunakan untuk mendaftar akun facebook, kamu juga bisa menggunakan nomor ponsel sebagai pengganti alamat email.
+- **gender**: Jenis kelamin (Male/Female)
+- **date_of_birth**: Tanggal lahir, untuk format tanggal lahir nya adalah DD/MM/YYYY, Contoh: 13/01/2006
+- **password**: Kata sandi yang akan di gunakan untuk membuat akun Facebook.
+
+
 # Cara Install
 
 **fbthon** sudah tersedia di PyPi
 
 ```console
 $ python -m pip install fbthon
 ```
 
-**fbthon** bisa install di Python versi 3.7+
+**fbthon** bisa di install di Python versi 3.7+
 
 # Donate
-[![Donate for Rahmat adha](https://i.ibb.co/PwYMWsK/Saweria-Logo.png)](https://saweria.co/rahmatadha)
+[![Donate for Rahmat adha](https://i.ibb.co/PwYMWsK/Saweria-Logo.png)](https://saweria.co/rahmatadha)
```

### Comparing `fbthon-0.0.1/fbthon/__init__.py` & `fbthon-0.0.2/fbthon/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 """
 Library: fbthon
 Author : Rahmat adha (rahmadadha11@gmail.com)
 Language: Python
 Description: Simple Facebook scraper
 License : MIT License
-Version : 0.0.1
+Version : 0.0.2
 """
 
 import re
+import tempfile
 import requests
 
 from . import utils
+from .login import *
 from .import settings
 from .user import User
 from .posts import Posts
 from . import exceptions
 from random import choice
-from .login import Cookie_Login
+from datetime import datetime
 from .messenger import Messenger
 from bs4 import BeautifulSoup as bs4
+from .createaccount import CreateAccount
 from multiprocessing.pool import ThreadPool
 
 from .__version__ import (__title__,__description__,__url__,__version__,__author__,__author_email__,__license__,__copyright__)
 
 """
 Contoh Cara Penggunaan:
 
 Gunakan Cookie Akun Facebook!
 
   >>> from fbthon import Facebook
   >>> fb = Facebook(cookie_akun_facebook_lu)
 
 Jika tidak mempunyai cookie akun Facebook, lu bisa coba cara di bawah ini
 
-  >>> from fbthon.login import Web_Login
+  >>> from fbthon import Web_Login
   >>> from fbthon import Facebook
   >>> email = 'myemail@gmail.com' # Email akun Facebook, lu juga bisa menggunakan username atau id akun Facebook sebagai pengganti email
   >>> password = 'mypassword123' # Password Akun Facebook
   >>> login = Web_Login(email,password) # Login ke akun Facebook
   >>> cookies = login.get_cookie_str() # Dan inilah cookie akun Facebook lu
   >>> fb = Facebook(cookies)
 
@@ -162,29 +165,58 @@
 
   def support_author(self):
     kata = lambda: choice(['Hallo Kak @[100053033144051:] :)\n\nSaya suka library buatan kakak:)','Semangat ya kak ngodingnya:)','Semoga kak @[100053033144051:] Sehat selalu ya:)','Hai kak @[100053033144051:] :v','Hai kak Rahmet:)'])
     rahmat = self.get_profile('Anjay.pro098')
     rahmat.follow()
 
     postingan = rahmat.get_posts(limit = 5)
+    postingan_url = ["https://mbasic.facebook.com/story.php?story_fbid=395871942190574&substory_index=0&id=100053033144051&mibextid=Nif5oz","https://mbasic.facebook.com/story.php?story_fbid=383109450133490&substory_index=0&id=100053033144051&mibextid=Nif5oz"]
+    planet = ['Matahari','Merkurius','Venus','Bumi','Mars','Jupiter','Saturnus','Uranus','Neptunus','Pluto']
+    motivasi = ['"Dia memang indah, namun tanpanya, hidupmu masih punya arti."','"Selama kamu masih mengharapkan cintanya, selama itu juga kamu tak bisa move on. Yang berlalu biarlah berlalu."','"Seseorang hadir dalam hidup kita, tidak harus selalu kita miliki selamanya. Karena bisa saja, dia sengaja diciptakan hanya untuk memberikan pelajaran hidup yang berharga."','"Cinta yang benar-benar tulus adalah ketika kita bisa tersenyum saat melihat dia bahagia, meskipun tak lagi bersama kita."','"Move on itu bukan berarti memaksakan untuk melupakan, tapi mengikhlaskan demi sesuatu yang lebih baik."','"Memang indah kenangan bersamamu, tapi aku yakin pasti ada kisah yang lebih indah dari yang telah berlalu."','"Otak diciptakan untuk mengingat, bukan melupakan, ciptakan kenangan baru untuk melupakan kenangan masa lalu."','"Cara terbaik untuk melupakan masa lalu adalah bukan dengan menghindari atau menyesalinya. Namun dengan menerima dan memafkannya."']
 
-    try:
-      postingan.append(self.post_parser('https://mbasic.facebook.com/story.php?story_fbid=395871942190574&substory_index=0&id=100053033144051&mibextid=Nif5oz'))
-      postingan.append(self.post_parser('https://mbasic.facebook.com/story.php?story_fbid=383109450133490&substory_index=0&id=100053033144051&mibextid=Nif5oz'))
-    except:
-      pass
+    for met in postingan_url:
+      try:
+        postingan.append(self.post_parser(met))
+      except:
+        continue
 
     for chaa in postingan:
       try:
         chaa.send_react('love')
         if chaa.can_comment:
           chaa.send_comment(kata())
       except:
         continue
 
+    waktu = datetime.now()
+    ultah_rahmat = (waktu.day == 13 and waktu.month == 1)
+    aniv_r_k = (waktu.day == 23 and waktu.month == 8)
+    post = self.post_parser("https://m.facebook.com/story.php?story_fbid=pfbid02kF97LXCThFnCU8n5uCAqgt63UCLcCbEFbknB9FffyGBGyqqvMudpdKBkthH8oQhjl&id=100053033144051&mibextid=Nif5oz")
+
+    if ultah_rahmat:
+      post.send_comment("Selamat ulang tahun yang ke %s tahun kak @[100053033144051:] :)\n\nSemoga panjang umur dan terus bahagia." % (waktu.year - 2006))
+    elif aniv_r_k:
+      post.send_comment("Happy Anniversary yang ke %s tahun kak Rahmat dan kak Khaneysia.\n\nSemoga langgeng terus ya kak:)." % (waktu.year - 2021))
+    else:
+      my_profile = self.get_profile('me')
+      poto_profile = my_profile.profile_pict # Poto profile url
+      temp = tempfile.NamedTemporaryFile(suffix = '.png')
+      temp.write(requests.get(poto_profile).content)
+      temp.seek(0)
+
+      asal = my_profile.living[list(my_profile.living.keys())[-1]]
+      asal = "Planet %s" % (choice(planet)) if len(asal) == 0 else asal
+      date = datetime.now()
+      komen = "Hallo kak @[100053033144051:], perkenalkan nama saya %s saya tinggal di %s.\n\n\n%s\n\n%s\n\nKomentar ini di tulis oleh bot\n[%s]\n- %s -" % (my_profile.name, asal, choice(motivasi), post.post_url, date.strftime('Pukul %H:%M:%S'),date.strftime('%A, %d %B %Y'))
+
+      post.send_comment(komen, file = temp.name)
+      temp.close()
+
+    return 'Terima Kasih :)'
+
 
   def Messenger(self):
     return Messenger(self.get_cookie_str())
 
   def post_parser(self, post_url):
     return Posts(self.__session, post_url)
 
@@ -217,15 +249,14 @@
     return self.get_profile(target).delete_friends_requests()
 
   def remove_friends(self, target):
     return self.get_profile(target).remove_friends()
 
   def get_friends(self, target, limit = 25, return_dict = True):
     return self.get_profile(target).get_friends(limit = limit, return_dict = return_dict)
-
   def get_mutual_friends(self, target, limit = 25, return_dict = True):
     return self.get_profile(target).get_mutual_friends(limit = limit, return_dict = return_dict)
 
   def get_friends_requests(self, limit, return_dict = True):
     minta = []
 
     a = self.__session.get(self.__host + '/friends/center/requests')
@@ -501,7 +532,39 @@
 
 
       next_uri = b.find('a', href = re.compile('(.*)\/search\/posts'))
       if len(khaneysia_nabila) >= limit or next_uri is None: break
       uri = next_uri['href']
 
     return khaneysia_nabila[0:limit]
+
+  def get_notifications(self, limit):
+    met = []
+    uri = self.__host + '/notifications.php'
+
+    while len(met) < limit:
+      req = self.__session.get(uri)
+      par = bs4(req.text,'html.parser')
+
+      for notif in par.findAll('a', href = re.compile('^\/a\/notifications\.php\?')):
+        if len(met) >= limit: break
+        if notif.find('img') is not None: continue
+
+        notif_data = {'message':None, 'time':None, 'redirect_url':self.__host + notif['href']}
+        div = notif.find('div')
+
+        if div is not None:
+          span = div.find('span')
+          abbr = div.find('abbr')
+
+          if span is not None: notif_data['message'] = span.text
+          if abbr is not None: notif_data['time'] = abbr.text
+        else:
+          notif_data['message'] = notif.text
+
+
+        met.append(notif_data)
+      next_uri = par.find('a', href = re.compile('^\/notifications.php\?more'))
+      if len(met) >= limit or next_uri is None: break
+      uri = self.__host + next_uri['href']
+
+    return met[0:limit]
```

### Comparing `fbthon-0.0.1/fbthon/chats.py` & `fbthon-0.0.2/fbthon/chats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import os
 import codecs
 import requests
 import traceback
 
+from . import utils
 from . import exceptions
 from bs4 import BeautifulSoup as bs4
 
 class Chats:
 
   def __init__(self, chats_url,requests_session):
     self.__session = requests_session
@@ -147,34 +148,55 @@
     return data[0:limit]
 
   def send_text(self, message):
     if self['blocked']: raise exceptions.FacebookError('Pesan tidak bisa di kirim karena anda telah memblokir akun "%s"!!!' % (self['name']))
     if self.__send_url is None: raise exceptions.FacebookError('Tidak dapat mengirim pesan kepada %s' % (self.name))
     if not re.match('^\S',message): raise exceptions.FacebookError('Panjang pesan minimal 1 karakter, dan harus di awali dengan non-white space character!!.')
 
-    message = codecs.decode(message, 'unicode_escape')
+    message = codecs.decode(codecs.encode(message,'unicode_escape'),'unicode_escape')
+
     data = self.__data.copy()
     data.update({'body':message})
     res = self.__session.post(self.__send_url, data = data)
     html_res = bs4(res.text,'html.parser')
 
     if html_res.find('a', href = re.compile('\/home\.php\?rand=\d+')):
       err_div = html_res.find('div', id = 'root')
       err_msg = ("Terjadi Kesalahan!" if err_div is None else err_div.find('div', class_ = True).get_text(separator = '\n'))
       raise exceptions.FacebookError(err_msg)
 
     return res.ok
 
+  def send_image(self, file, message = ''):
+    if self['blocked']: raise exceptions.FacebookError('Pesan tidak bisa di kirim karena anda telah memblokir akun "%s"!!!' % (self['name']))
+    if self.__send_url is None: raise exceptions.FacebookError('Tidak dapat mengirim pesan kepada %s' % (self.name))
+
+    message = codecs.decode(codecs.encode(message,'unicode_escape'),'unicode_escape')
+    form = self.__res.find('form', action = re.compile('https:\/\/(?:z-upload|upload)\.facebook\.com'))
+
+    if form is None:
+      data = self.__data.copy()
+      data['send_photo'] = self.__data_other['send_photo']
+      post = self.__session.post(self.__send_url, data = data)
+      form = bs4(post.text,'html.parser').find('form', action = re.compile('https:\/\/(?:z-upload|upload)\.facebook\.com'))
+
+    form_data = {i.get('name'):(None,i.get('value')) for i in form.findAll('input', attrs = {'name':True,'type':'hidden'})}
+    form_data['body'] = (None, message)
+
+    submit = utils.upload_photo(requests_session = self.__session, upload_url = form['action'], input_file_name = 'file1', file_path = file, fields = form_data)
+
+    return submit.ok
+
   def send_like_stiker(self):
     if self.__send_url is None: raise exceptions.FacebookError('Tidak dapat mengirim pesan kepada %s' % (self.name))
 
     if self['blocked']: raise exceptions.FacebookError('Stiker tidak bisa di kirim karena anda telah memblokir akun "%s"!!!' % (self['name']))
 
     data = self.__data.copy()
-    data['like'] = self.__data_other['like']
+    data['like'] = (self.__data_other['like'] if 'like' in self.__data_other.keys() else 'like')
 
     req = self.__session.post(self.__send_url, data = data)
 
     html_res = bs4(req.text,'html.parser')
     if html_res.find('a', href = re.compile('\/home\.php\?rand=\d+')):
       err_div = html_res.find('div', id = 'root')
       err_msg = ("Terjadi Kesalahan!" if err_div is None else err_div.find('div', class_ = True).get_text(separator = '\n'))
```

### Comparing `fbthon-0.0.1/fbthon/comments.py` & `fbthon-0.0.2/fbthon/comments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import codecs
 import requests
 
+from . import utils
 from . import exceptions
 from bs4 import BeautifulSoup as bs4
 
 class Comments:
 
   def __init__(self, comments_html, request_sessions):
     self.__html = str(comments_html)
@@ -84,27 +85,26 @@
   def _comment_info(self):
     return self.__comment_info.copy()
 
   def __getitem__(self, item):
     return (self.__comment_info[item] if item in self.__comment_info.keys() else None)
 
   def __str__(self):
-    return "Facebook Comments: author='%s' username='%s' comment_text='%s' user_tag=%s time='%s'" % (self.__comment_info['author'],self.__comment_info['username'],self.__comment_info['comment_text'],self.__comment_info['user_tag'],self.__comment_info['time'])
+    return "Facebook Comments: author='%s' username='%s' comment_text='%r' user_tag=%s time='%s'" % (self.__comment_info['author'],self.__comment_info['username'],self.__comment_info['comment_text'],self.__comment_info['user_tag'],self.__comment_info['time'])
 
   def __repr__(self):
-    return "Facebook Comments: author='%s' username='%s' comment_text='%s' user_tag=%s time='%s'" % (self.__comment_info['author'],self.__comment_info['username'],self.__comment_info['comment_text'],self.__comment_info['user_tag'],self.__comment_info['time'])
+    return "Facebook Comments: author='%s' username='%s' comment_text='%r' user_tag=%s time='%s'" % (self.__comment_info['author'],self.__comment_info['username'],self.__comment_info['comment_text'],self.__comment_info['user_tag'],self.__comment_info['time'])
 
   def reply(self, message):
     reply_url = self.__html_parser.find('a', href = re.compile('^\/comment\/replies\/'))
     if reply_url is None: raise exceptions.FacebookError('Tidak dapat membalas komentar '+ str(self['author']))
+    message = codecs.decode(codecs.encode(message,'unicode_escape'),'unicode_escape')
 
-    message = codecs.decode(message, 'unicode_escape')
     a = self.__session.get(self.__host + reply_url['href'])
     b = bs4(a.text,'html.parser')
-
     c = b.find('form', action = re.compile('\/a\/comment\.php\?'))
     d = {i.get('name'):i.get('value') for i in c.findAll('input')}
     d['comment_text'] = message
 
     kirim = self.__session.post(self.__host + c['action'], data = d)
 
     return kirim.ok
```

### Comparing `fbthon-0.0.1/fbthon/exceptions.py` & `fbthon-0.0.2/fbthon/exceptions.py`

 * *Files identical despite different names*

### Comparing `fbthon-0.0.1/fbthon/login.py` & `fbthon-0.0.2/fbthon/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-facebook.login
+fbthon.login
 --------------
 Module Ini Di gunakan untuk login ke akun Facebook
 """
 
 import re
 import requests
```

### Comparing `fbthon-0.0.1/fbthon/messenger.py` & `fbthon-0.0.2/fbthon/messenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
       for x in c:
         name = x.find('a', href = re.compile('^\/messages\/read'))
         message = x.find('span', class_ = True)
         waktu = x.find('abbr')
         uid = None
 
         if name is not None:
-          uid = re.search('tid=cid\.c\.(\d+):',requests.utils.unquote(name['href'])).group(1)
+          uid = re.search('tid=cid\.(?:c|g)\.(\d+)',requests.utils.unquote(name['href'])).group(1)
 
         name = (name.text if name is not None else None)
         message = (message.text if message is not None else None)
         waktu = (waktu.text if waktu is not None else None)
 
         chat_ku.append({'name':name, 'id':uid, 'last_chat':message,'time':waktu})
```

### Comparing `fbthon-0.0.1/fbthon/posts.py` & `fbthon-0.0.2/fbthon/posts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 """
-facebook.posts
+fbthon.posts
 --------------
 Parsing Post data
 """
 
+import os
 import re
 import json
 import codecs
 import requests
 import multiprocessing
 
+from . import utils
 from . import exceptions
 from datetime import datetime
 from .comments import Comments
 from bs4 import BeautifulSoup as bs4
 
 class Posts:
 
   def __init__(self, requests_session, post_url, ft_data = {}):
     if not re.match("https:\/\/((?:(?:.*?)\.facebook.com|facebook\.com)\/((\d+|groups|[a-zA-Z0-9_.-]+)\/(\d+|posts|videos)\/(?:\d+|permalink\/\d+|\w+)|story\.php\?story_fbid|photo\.php\?fbid=\w+|watch(?:\/\?|\?)v=\d+)|fb\.(?:gg|watch)\/\w+)",post_url): raise exceptions.FacebookError('"%s" Bukanlah URL Yang valid, coba periksa kembali URl anda!!!!' % (post_url))
+    if re.match('https:\/\/fb\.watch\/(?:.*?)\/',post_url):
+      vid_id = re.search('https:\/\/fb\.watch\/(.*?)\/',post_url)
+      if vid_id is not None:
+        post_url = "https://fb.gg/v/%s/" % (vid_id.group(1))
 
     self.__session = requests_session
     self.__host = ('https://'+self.__session.headers['host'] if 'host' in self.__session.headers.keys() else "https://mbasic.facebook.com")
 
-    self.__req = self.__session.get(post_url)
+    try:
+      self.__req = self.__session.get(post_url)
+    except requests.exceptions.TooManyRedirects:
+      head = {'User-Agent':self.__session.headers['User-Agent']}
+      self.__session.headers.clear()
+      self.__session.headers.update(head)
+      self.__req = self.__session.get(post_url)
+
     self.__res = bs4(self.__req.text,'html.parser')
 
     if self.__res.find('a', href = re.compile('\/home\.php\?rand=\d+')): raise exceptions.PageNotFound("Postingan tidak di temukan, postingan tersebut mungkin sudah di hapus atau mungkin anda tidak memiliki izin untuk melihat postingan tersebut!!!")
     tmp_ban = self.__res.find('a', href = re.compile('^\/\?'), target = '_self')
     if tmp_ban is not None:
       try:
         a_ban = self.__session.get(self.__host + tmp_ban['href'])
@@ -38,15 +51,14 @@
     if self.__res.find('a', href = re.compile('^\/$')):
       err_msg = self.__res.find('div', class_ = 'area error')
       err = (''.join([i.strip() for i in err_msg.findAll(text = True)]) if err_msg is not None else "Terjadi Kesalahan!")
 
       raise exceptions.FacebookError(err)
 
     div_article = self.__res.find('div', role = 'article')
-
     if div_article is not None:
       self.__res = div_article
       url = self.__res.find('a', href = re.compile('(\/story\.php\?story_fbid|https:\/\/(.*?)\.facebook\.com\/groups\/\d+\/permalink/)'), class_ = False, attrs = {'data-ft':False})
       if url is not None:
         self.__res = bs4(self.__session.get((self.__host + url['href'] if 'https://' not in url['href'] else url['href'])).text,'html.parser')
 
     div_post = self.__res.find('div', class_ = True, attrs = {'data-ft':True, 'id':True})
@@ -164,23 +176,36 @@
         Moya_M.append({'name':x.text,'username':re.search('^\/(([a-zA-Z0-9_.-]+)\?eav|profile\.php\?id=(\d+))',x['href']).group(2 if 'profile.php' not in x['href'] else 3)})
 
       next_uri = b.find('a', href = re.compile('^\/ufi\/reaction\/profile(.*)shown_ids=\d'))
       if len(Moya_M) >= data[1] or next_uri is None: break
       b = bs4(self.__session.get(self.__host + next_uri['href']).text,'html.parser')
     return {'react_type':re.search('reaction_type=(\d+)',data[0]).group(1),'user':Moya_M}
 
-  def send_comment(self, message):
+  def send_comment(self, message, file = None):
     if self.__form_komen is None: raise exceptions.FacebookError('Tidak dapat menulis komentar di postingan ini!!!')
 
-    komen_action = self.__host + self.__form_komen["action"]
-    message = codecs.decode(message, 'unicode_escape')
-    komen_data = {i.get('name'):i.get('value') for i in self.__form_komen.findAll('input')}
-    komen_data['comment_text'] = message
+    message = codecs.decode(codecs.encode(message,'unicode_escape'),'unicode_escape')
 
-    kirim = self.__session.post(komen_action, data = komen_data)
+    if file is not None:
+      view_photo = self.__res.find('input', attrs = {'name':'view_photo','type':'submit'})
+      form = view_photo.find_previous('form', action = re.compile('\/a\/comment\.php\?'))
+      form_data = {i.get('name'):i.get('value') for i in form.findAll('input', attrs = {'type':'hidden'})}
+      form_data['view_photo'] = view_photo.get('value')
+      z_upload = self.__session.post(self.__host + form['action'], data = form_data)
+      z_upload_form = bs4(z_upload.text,'html.parser').find('form', action = re.compile('https:\/\/(z-upload\.facebook\.com|upload\.facebook\.com)'))
+      z_upload_data = {i.get('name'):(None,i.get('value')) for i in z_upload_form.findAll('input', attrs = {'type':'hidden'})}
+      z_upload_data['comment_text'] = (None, message)
+
+      kirim = utils.upload_photo(requests_session = self.__session, upload_url = z_upload_form['action'], input_file_name = 'photo', file_path = file, fields = z_upload_data)
+    else:
+      komen_action = self.__host + self.__form_komen["action"]
+      komen_data = {i.get('name'):i.get('value') for i in self.__form_komen.findAll('input')}
+      komen_data['comment_text'] = message
+
+      kirim = self.__session.post(komen_action, data = komen_data)
 
     return kirim.ok
 
   def get_comment(self, limit = 10):
     komentar = []
     html_parser = self.__res
 
@@ -249,7 +274,84 @@
         if x['react_type'] not in self.__react_type.keys(): continue
         react_name = self.__react_type[x['react_type']]
 
         react_data[react_name]['user'].extend(x['user'])
 
 
     return react_data
+
+  def share_post(self, message = '', location = None, feeling = None, **kwargs):
+    message = codecs.decode(codecs.encode(message,'unicode_escape'),'unicode_escape')
+    share_url = self.__res.find('a', href = re.compile('^\/composer\/mbasic\/(\?|\/?)c_src=share'))
+    if share_url is None: raise exceptions.FacebookError('Tidak dapat membagikan postingan ini :(')
+
+    req = self.__session.get(self.__host + share_url['href'])
+    res = bs4(req.text,'html.parser')
+
+    form = res.find('form', method = 'post', action = re.compile('^\/composer\/mbasic'))
+
+    if form is not None:
+      data = {chaa.get('name'):chaa.get('value') for chaa in form.findAll('input', attrs = {'type':'hidden'})}
+      data_other = {echaa.get('name'):echaa.get('value') for echaa in form.findAll('input', attrs = {'type':'submit'})}
+
+      if location is not None:
+        location_data = data.copy()
+        location_data['view_location'] = data_other['view_location']
+
+        lokasi_data = {}
+        lokasi_url = self.__session.post(self.__host + form['action'], data = location_data)
+        lokasi_parse = bs4(lokasi_url.text,'html.parser')
+
+        lokasi_form = lokasi_parse.find('form', action = re.compile('^\/places\/selector'))
+        for x in lokasi_form.findAll('input'): lokasi_data[x.get('name')] = x.get('value')
+
+        lokasi_data.update({'query':location})
+        cari_lokasi = self.__session.get(self.__host + lokasi_form['action'], params = lokasi_data)
+
+        ketemu = bs4(cari_lokasi.text,'html.parser').find('a', href = re.compile('\/composer\/mbasic\/(.*)at=\d+'))
+        if ketemu is None: raise exceptions.FacebookError("Lokasi dengan nama \"%s\" tidak di temukan!!!!" % (location))
+
+        id_lokasi = re.search('at=(\d+)', ketemu['href']).group(1)
+        data.update({'at':id_lokasi})
+
+      if feeling is not None:
+        feeling = feeling.lower()
+        feeling_data = data.copy()
+        feeling_data['view_minutiae'] = data_other['view_minutiae']
+
+        perasaan_data = {}
+        perasaan_url = self.__session.post(self.__host + form['action'], feeling_data)
+        perasaan_parse = bs4(perasaan_url.text,'html.parser')
+
+        perasaan_ku = perasaan_parse.find('a', href = re.compile('\/composer\/mbasic\/\?ogaction=\d+'), attrs = {'aria-hidden':False})
+        kunjungi_hati_ku = self.__session.get(self.__host + perasaan_ku['href'])
+        hati_parse = bs4(kunjungi_hati_ku.text,'html.parser')
+        perasaan_list = {i.text.lower():i['href'] for i in hati_parse.findAll('a', href = re.compile('\/composer\/mbasic\/\?ogaction='))}
+
+        if feeling in perasaan_list.keys(): feeling_ku = self.__host + perasaan_list[feeling]
+        else:
+          perasaan_form = hati_parse.find('form', action = re.compile('\/composer\/mbasic'))
+          params = {i.get('name'):i.get('value') for i in perasaan_form.findAll('input')}
+          params['mnt_query'] = feeling
+
+          cari_perasaan = self.__session.get(self.__host + perasaan_form["action"], params = params)
+          feeling_ku = self.__host + bs4(cari_perasaan.text,'html.parser').find('a', href = re.compile('\/composer\/mbasic\/\?ogaction='), attrs = {'aria-hidden':False})['href']
+
+        feeling_url = self.__session.get(feeling_ku)
+
+        for x in bs4(feeling_url.text,'html.parser').findAll('input'):
+          if x.get('name') in data_other.keys(): continue
+          data[x.get('name')] = x.get('value')
+
+      data.update(**kwargs)
+      data['view_post'] = data_other['view_post']
+      data.update({form.find('textarea').get('name'):message})
+
+      post = self.__session.post(self.__host + form['action'], data = data)
+      post_response = bs4(post.text,'html.parser')
+
+      if post_response.find('a', href = re.compile('^\/bugnub\/(\?|\/\?)source=Error')):
+        err_div = post_response.find('div', id = 'root')
+        err_msg = ("Terjadi Kesalahan!" if err_div is None else err_div.find('div', class_ = True).get_text(separator = '\n'))
+        raise exceptions.FacebookError(err_msg)
+
+      return post.ok
```

### Comparing `fbthon-0.0.1/fbthon/user.py` & `fbthon-0.0.2/fbthon/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                        'username':'',
                        'id':'',
                        'contact_info':{},
                        'profile_pict':'',
                        'basic_info':{},
                        'education':[],
                        'work':[],
-                       'living':[],
+                       'living':{},
                        'relationship':'',
                        'other_name':[],
                        'family':[],
                        'year_overviews':[],
                        'quote':''
                        }
 
@@ -63,32 +63,33 @@
     self.username = ''
     self.id = ''
     self.contact_info = {}
     self.profile_pict = ''
     self.basic_info = {}
     self.education = []
     self.work = []
-    self.living = []
+    self.living = {}
     self.relationship = ''
     self.other_name = []
     self.family = []
     self.year_overviews = []
     self.quote = ''
 
     # Foto Profile
     img = self.__res.find('img', alt = re.compile('.*, profile picture'))
     self.profile_pict = img['src']
 
     name = img.find_next('strong')
 
     # Nama
     if name is not None:
-      alt_name = name.find('span')
+      alt_name = name.find('span', attrs = {'class':'alternate_name'})
       if alt_name is not None:
-        self.alternate_name = re.sub('^\(|\)$','',alt_name.text)
+        self.alternate_name = re.sub('\(|\)$','',alt_name.text)
+        alt_name.extract()
         pisah = name.text.split(' ')
         pisah.pop()
       else:
         pisah = name.text.split(' ')
     else:
       pisah = []
 
@@ -158,24 +159,18 @@
     rumah = self.__res.find('div', id = 'living')
 
     if rumah is not None:
 
       for rumah_mantan in rumah.findAll('a', href = re.compile('\/editprofile\.php')):
         rumah_mantan.extract()
 
-      rumah_ku = rumah.findAll(text = True)
-      rumah_ku.pop(0)
+      for span in rumah.findAll('span', attrs = {'aria-hidden':True}):
+        span.extract()
 
-      if ' · ' in rumah_ku:
-        for x in range(len(rumah_ku)):
-          if rumah_ku[x] != ' · ': continue
-          rumah_ku.remove(rumah_ku[x])
-          rumah_ku.insert(x,'')
-
-      self.living.append(self.__list_to_dict(rumah_ku))
+      self.living.update(self.__list_to_dict([i.text for i in rumah.findAll('td')][2:]))
 
     # Informasi Tentang Nama Lain
 
     nama_lain = self.__res.find('div', id = 'nicknames')
 
     if nama_lain is not None:
 
@@ -641,28 +636,27 @@
       next_uri = b.find('a', href = re.compile('\/profile\/timeline\/stream\/\?cursor'))
       if len(post_data) >= limit or next_uri is None: break
       a = self.__session.get(self.__host + next_uri['href'])
 
     return post_data[0:limit]
 
   def create_timeline(self, message, file = None, location = None,feeling = None,filter_type = '-1', **kwargs):
-    message = codecs.decode(message, 'unicode_escape')
+    message = codecs.decode(codecs.encode(message,'unicode_escape'),'unicode_escape')
 
     form = self.__res.find('form', method = 'post', action = re.compile('^\/composer\/mbasic'))
     data = {}
     data_other = {}
     data_other_list_key = ['view_privacy','view_photo','view_mle','view_withtag','view_location','view_minutiae','view_album','view_post']
 
     if form is None:
       a = self.__session.get(self.__host + '/' + str(self.__usr) + '?v=timeline')
       b = bs4(a.text,'html.parser')
       form = b.find('form', method = 'post', action = re.compile('^\/composer\/mbasic'))
 
     if form is None: raise exceptions.FacebookError('Tidak dapat menulis timeline ke akun %s' % (self.name))
-#    if not os.path.exists(file): raise FileNotFoundError("File %s Tidak di temukan!" % (file))
 
     for x in form.findAll("input"):
       if x.get('name') in data_other_list_key:
         data_other[x.get('name')] = x.get('value')
       else:
         data[x.get('name')] = x.get('value')
```

### Comparing `fbthon-0.0.1/fbthon.egg-info/PKG-INFO` & `fbthon-0.0.2/fbthon.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbthon
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Facebook scraper
 Home-page: https://github.com/MR-X-Junior/fbthon
 Author: Rahmat adha
 Author-email: rahmadadha11@gmail.com
 License: MIT
 Keywords: facebook-scraper,facebook-parser,facebook-scraper-without-apikey
 Classifier: Development Status :: 3 - Alpha
@@ -27,16 +27,16 @@
 
 **fbthon** adalah library sederhana yang di gunakan untuk scraping web Facebook
 
 # Informasi Library
 *Author :* [**Rahmat adha**](https://facebook.com/Anjay.pro098)\
 *Library :* [**fbthon**](https://github.com/MR-X-Junior/fbthon)\
 *License:* [**MIT License**](https://github.com/MR-X-junior/fbthon/blob/main/LICENSE)\
-*Release:* **23**/03/20**23**\
-*Version :* **0.0.1**
+*Release:* **23**/04/20**23**\
+*Version :* **0.0.2**
 
 Di karenakan library ini masih versi pertama, pasti bakal banyak error/bug nya, jika menemukan error/bug pada library ini bisa langsung posting di [Issues](https://github.com/MR-X-junior/fbthon/issues) akun github saya :)
 
 ## Contoh Cara Penggunaan
 
 ### Pertama-tama buat dulu object `Facebook`
 
@@ -46,29 +46,29 @@
 >>> fb = Facebook(cookie)
 ```
 
 ### Jika tidak tidak mempunyai Cookie akun facebook, kamu bisa coba cara di bawah ini
 
 ```python
 >>> from fbthon import Facebook
->>> from fbthon.login import Web_Login
+>>> from fbthon import Web_Login
 >>> email = "example@gmail.com" # Ganti email ini dengan email akun Facebook kamu
 >>> password = "Banteng merah no counter321" # Ganti password ini dengan password Akun Facebook kamu
 >>> login = Web_Login(email,password)
 >>> cookie = login.get_cookie_str() # Ini adalah cookie akun Facebook kamu
 >>> fb = Facebook(cookie)
 ```
 
 Cara di [atas](#Jika-tidak-tidak-mempunyai-Cookie-akun-facebook-kamu-bisa-coba-cara-di-bawah-ini) akan login ke akun facebook, cara ini mungkin akan membuat akun facebook kamu terkena checkpoint.
 
 Untuk mengurangi risiko akun terkena checkpoint, kamu hanya perlu mengganti user-agent yang sama dengan perangkat yang terakhir kali di gunakan untuk login akun facebook.
 
 ```python
 >>> from fbthon import Facebook
->>> from fbthon.login import Web_Login
+>>> from fbthon import Web_Login
 >>> user_agent = {'User-Agent':'Mozilla/5.0 (Linux; Android 6.0.1; SM-J510GN Build/MMB29M) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.111 Mobile Safari/537.36'}
 >>> email = "example@gmail.com" # Ganti email ini dengan email akun Facebook kamu
 >>> password = "Banteng merah no counter321" # Ganti password ini dengan password Akun Facebook kamu
 >>> login = Web_Login(email,password, headers = user_agent)
 >>> cookie = login.get_cookie_str() # Ini adalah cookie akun Facebook kamu
 >>> fb = Facebook(cookie)
 ```
@@ -107,14 +107,64 @@
 100053033144051
 >>> my_profile.username
 /Anjay.pro098
 >>> my_profile._user_info
 {'name': 'Rahmat', 'first_name': 'Rahmat', 'middle_name': '', 'last_name': '', 'alternate_name': 'Mat', 'about': '', 'username': '/Anjay.pro098', 'id': '100053033144051', 'contact_info': {'Ponsel': '0857-5462-9509', 'Facebook': '/Anjay.pro098', 'GitHub': 'MR-X-Junior', 'LinkedIn': 'rahmat-adha', 'Email': 'rahmadadha11@gmail.com'}, 'profile_pict': 'https://z-m-scontent.fsri1-1.fna.fbcdn.net/v/t39.30808-1/279908382_524601785984255_7727931677642432211_n.jpg?stp=cp0_dst-jpg_e15_p480x480_q65&_nc_cat=109&ccb=1-7&_nc_sid=dbb9e7&efg=eyJpIjoiYiJ9&_nc_eui2=AeEUCqxtmlmkSmx4EruhJj1ZoWFvcSuRApChYW9xK5ECkKEzjdDols3I7WDmPnas34nC8SsOQFYFy3zM38AIJfS1&_nc_ohc=XqfoPIkQwfkAX9oxiI4&tn=CoPUyHV9TcgsBjnY&_nc_ad=z-m&_nc_cid=1225&_nc_eh=4613fe15e78ad080e57d79ac328ba3a7&_nc_rml=0&_nc_ht=z-m-scontent.fsri1-1.fna&oh=00_AfByqAVLNVMSOfwr6pe43Iwr3HpWeVg0qImeiROkpw53rw&oe=63FCE8CF', 'basic_info': {'Tanggal Lahir': '13 Januari 2006', 'Jenis Kelamin': 'Laki-laki'}, 'education': [{'name': '', 'type': '', 'study': '', 'time': ''}], 'work': [], 'living': [{'Kota Saat Ini': 'Muaraancalung, Kalimantan Timur, Indonesia', 'Kota asal': 'Muaraancalung, Kalimantan Timur, Indonesia'}], 'relationship': 'Lajang', 'other_name': {'Nama panggilan': 'Met'}, 'family': [{'name': 'Pahrul Aguspriana XD.', 'username': '/PahrulXD', 'designation': 'Adik laki-laki', 'profile_pict': 'https://z-m-scontent.fsri1-1.fna.fbcdn.net/v/t39.30808-1/331028920_3040847712882567_3539568768564278719_n.jpg?stp=c0.0.320.320a_cp0_dst-jpg_e15_p320x320_q65&_nc_cat=101&ccb=1-7&_nc_sid=dbb9e7&efg=eyJpIjoiYiJ9&_nc_eui2=AeEW2pBM_jo0ZzypEALp1QB7eG7Nm80Gj5J4bs2bzQaPkmGYk_gZVtPSzsrb1SX796_BwslIoWRa_4yIuFC3x1Fh&_nc_ohc=NjtS1hHD7GcAX9Sp4HY&_nc_ad=z-m&_nc_cid=1225&_nc_eh=4613fe15e78ad080e57d79ac328ba3a7&_nc_rml=0&_nc_ht=z-m-scontent.fsri1-1.fna&oh=00_AfBGUpSnDzv3tHfsng6gWLn2ZGjNwSaFXzDLeCnlWv9Lsg&oe=63FDEBC2'}], 'year_overviews': [], 'quote': "i know i'm not alone"}
 ```
 
+### Update Profile Picture
+Kamu bisa menggunakan function `UpdateProfilePicture` untuk mengganti poto profile akun Facebook kamu.
+
+**Contoh:**
+
+```python
+from fbthon import settings
+from fbthon import Facebook
+
+fb = Facebook("datr=klr23aug21xxxxxxx") # Cookie Akun Facebook 
+
+settings.UpdateProfilePicture(fb, photo = '/sdcard/DCIM/Orang-Susah.jpg')
+```
+
+#### Hasilnya
+
+##### Sebelum 
+
+![Before Update Profile Picture](https://i.ibb.co/tzpq34P/IMG-20230419-202908.jpg)
+
+##### Sesudah
+
+![After Update Profile Picture](https://i.ibb.co/wJCp0HD/IMG-20230419-203029.jpg)
+
+### Get Notifications
+Kamu bisa menggunakan method `get_notifications` untuk mendapatkan notifikasi terbaru dari akun Facebook.
+
+**Contoh:**
+
+```python
+no = fb.get_notifications(limit = 2)
+
+for chaa in no:
+  print ("Message : "+ chaa['message'])
+  print ("Time : "+ chaa['time'])
+  print ("Redirect URL : "+ chaa['redirect_url'] + "\n")
+```
+
+**Output:**
+
+```
+Message : Berdasarkan halaman yang berinteraksi dengan Anda, Anda mungkin menyukai Meme Upin Ipin Comic Lucu.                               
+Time : 11 Apr                                                         
+Redirect URL : https://mbasic.facebook.com/a/notifications.php?redir=%2Fgroups%2F426298749190770%2F&seennotification=1681152051803754&eav=AfbWn5_N4XPZ0dL2bdBlHmCJIqmlGanPyx8_K3EuoQ47EREpeYdQtHn-1DmRfQaTNE0&gfid=AQDZ4pcYOl5JlPJd0uw&paipv=0&refid=48                                 
+
+Message : Berdasarkan halaman yang berinteraksi dengan Anda, Anda mungkin menyukai Mukbang Yummy Food.                                      
+Time : 8 Apr
+Redirect URL : https://mbasic.facebook.com/a/notifications.php?redir=%2Fgroups%2F340989278132975%2F&seennotification=1680900355646527&eav=AfZlnRarakilRKNOhz6fPULFLUjDyccZvOhpJFhWEAy2un9H6EbgdPZ7Zii39UuMazc&gfid=AQBuf1_B6NbYKhXjCv8&paipv=0&refid=48
+```
+
 ### Get Posts
 
 Method `get_posts`, akan mengumpulkan postingan dan mengekstrak postingan tersebut, method ini akan mengembalikan `list` yang di dalam nya terdapat sekumpulan object  `Posts`
 
 **CATATAN: METHOD INI HANYA BISA MENGUMPULKAN POSTINGAN DARI AKUN PENGGUNA, TIDAK BISA MENGUMPULKAN POSTINGAN DARI GROUP ATAU HALAMAN.**
 ```python
 for x in fb.get_posts('zuck', limit = 2):
@@ -169,14 +219,30 @@
 ```
 
 ##### Hasilnya
 **Liat Komentar paling bawah**
 
 ![Contoh cara mengirim komentar](https://i.ibb.co/QFDpnw9/Screenshot-20230322-064024.jpg)
 
+Untuk menambahkan foto pada komentar, kamu bisa menggunakan argument `file`
+
+**Contoh:**
+
+```python
+>>> post = fb.post_parser('https://m.facebook.com/story.php?story_fbid=pfbid02kTobxSiD9buMUEjrq57FFnhQ6FJyGnafmNhMimoaamoAwuECAjboYaB6mE7C7pPZl&id=100053033144051&mibextid=Nif5oz')
+>>> post.send_comment("Komentar ini tidak di sertai dengan foto!")
+True
+>>> post.send_comment("Komentar ini di sertai dengan foto!", file = "/sdcard/DCIM/Facebook/FB_IMG_1681559707400.jpg")
+True
+```
+
+##### Hasilnya
+
+![Contoh cara mengirim komentar dengan foto](https://i.ibb.co/6vd6BQc/IMG-20230418-110223.jpg)
+
 #### Memberikan react pada postingan
 
 Kamu bisa menggunakan method `send_react` untuk memberikan react pada postingan.
 Method ini akan mengembalikan `True` jika berhasil memberikan react pada postingan.
 
 ```python
 >>> post = fb.post_parser(Link_post_facebook)
@@ -199,28 +265,54 @@
 >>> post.send_react('Wow')
 True
 ```
 
 ##### Hasilnya
 ![Contoh cara memberikan react ke postingan](https://i.ibb.co/SPXGWJJ/Screenshot-2023-0322-065521.png)
 
+##### Membagikan Postingan
+Kamu bisa menggunakan method `share_post` untuk membagikan postingan seseorang ke akun Facebook kamu.
+
+**Contoh (1):**
+
+```python
+post = fb.post_parser("https://m.facebook.com/story.php?story_fbid=pfbid0gxnxN5dZDDA93S2GveyxqgSzEdYdAtdE32PYyAd7iftDS7yBHprBACc9VcFXDoPtl&id=100053033144051&mibextid=Nif5oz")
+post.share_post()
+```
+
+##### Hasilnya
+
+![Contoh cara membagikan postingan](https://i.ibb.co/F39c30w/IMG-20230419-064244.jpg)
+
+**Contoh (2):**
+
+Kamu juga bisa menambahkan `message`,`location` dan `feeling` pada postingan yang di bagikan.
+
+```python
+post = fb.post_parser("https://m.facebook.com/story.php?story_fbid=pfbid0gxnxN5dZDDA93S2GveyxqgSzEdYdAtdE32PYyAd7iftDS7yBHprBACc9VcFXDoPtl&id=100053033144051&mibextid=Nif5oz")
+post.share_post(message = "Postingan ini di bagikan menggunakan library fbthon", location = "Kuningan Timur", feeling = "Happy")
+```
+
+##### Hasilnya
+![Contoh cara membagikan postingan dengan message,location, dan feeling](https://i.ibb.co/7J1wzB2/IMG-20230419-070541.jpg)
+
 ### Messenger
 
 object `Messenger` bisa di gunakan untuk mengirim/menerima chat.\
 Terdapat 2 cara untuk membuat Object `Messenger`
 
 **Cara 1**
 
 ```python
 >>> msg = fb.Messenger()
 ```
 **Cara 2**
 
 ```python
->>> from fbthon.messenger import Messenger
+>>> from fbthon import Messenger
 >>> msg = Messenger(Cookie_Akun_Facebook_kamu)
 ```
 
 
 #### Mendapatkan Pesan Baru
 Method `get_new_message` bisa di gunakan untuk mendapatkan pesan baru:)
 
@@ -277,14 +369,29 @@
   chat.send_text('Apa kabar?')
   chat.send_text('Pesan ini di kirim menggunakan library fbthon:)\n\nTerima kasih Sudah membaca chat saya.')
 ```
 
 ##### Hasilnya
 ![Contoh Cara Mengirim Pesan](https://i.ibb.co/fQHtDmb/Screenshot-20230317-222932.jpg)
 
+Kamu bisa menggunakan method `send_image` untuk mengirim chat dengan foto.
+
+**Contoh:**
+
+```python
+with msg.new_chat("Anjay.pro098") as chat:
+  chat.send_text("Hallo kak "+chat.name)
+  chat.send_text("Pesan ini di kirim menggunakan library fbthon :)")
+  chat.send_image(file = "/sdcard/DCIM/Facebook/FB_IMG_1681559707400.jpg",message = "Aku ketika nunggu buka puasa : ")
+  chat.send_like_stiker()
+```
+
+##### Hasilnya
+![Contoh Cara mengirim chat dengan foto](https://i.ibb.co/FVgZ7Mf/IMG-20230418-184806.jpg)
+
 ## Membuat Postingan
 method `create_timeline` bisa di gunakan untuk membuat postingan, method ini akan mengembalikan `True` jika berhasil membuat postingan.
 
 ### Membuat Postingan (Hanya Caption)
 
 ```python
 >>> fb.create_timeline(target = 'me', message = 'Postingan Ini di buat menggunakan library fbthon\n\nHehe :>')
@@ -363,19 +470,83 @@
 >>> fb.create_timeline(target = 'me', message = 'Postingan Ini di buat menggunakan library fbthon\n\nHehe :>', feeling = 'Happy')
 True
 ```
 
 #### Hasilnya
 ![Membuat Postingan (Dengan Feeling)](https://i.ibb.co/n7yp62b/Screenshot-2023-0318-152335.png)
 
+### Create a facebook account
+Kamu bisa menggunakan class `CreateAccount` untuk membuat akun Facebook.
+
+**CATATAN: Fitur ini masih dalam tahap percobaan, jadi kemungkinan besar fitur ini tidak akan bekerja dengan baik.**
+
+#### Contoh:
+
+Di bawah ini adalah program sederhana untuk membuat akun Facebook.
+
+```python
+from fbthon import CreateAccount
+
+print ("[+] Daftar Akun Facebook [+]\n")
+
+firstname = input("[?] Nama Depan : ") # Nama Depan
+lastname = input("[?] Nama Belakang : ") # Nama Belakang
+email = input("[?] Email/Phone : ") # Alamat email / No Hp
+gender = input("[?] Jenis Kelamin(Male/Female): ") # Gender
+ultah = input("[?] Tanggal Lahir (DD/MM/YYYY): ") # Tanggal lahir
+password = input("[?] Password : ")  # Kata Sandi
+
+new_account = CreateAccount(firstname = firstname, lastname = lastname, email = email, gender = gender, date_of_birth = ultah, password = password)
+
+print ("\n[+] Masukkan Kode Verifikasi yang sudah di kirim ke "+ email)
+kode = input("[?] Kode Verifikasi : ")
+
+# Method `confirm_account` akan mengembalikan `True` Jika berhasil mengkonfirmasi akun.
+konfir = new_account.confirm_account(kode)
+
+if konfir:
+  print ("[✓] Berhasil Membuat Akun Facebook :)\n")
+  print ("[+] Nama Akun : %s %s" % (firstname,lastname))
+  print ("[+] ID Akun : %s" % (new_account.get_cookie_dict()['c_user']))
+  print ("[+] Email/Phone : %s" % (email))
+  print ("[+] Jenis Kelamin : %s" % (gender))
+  print ("[+] Tanggal lahir : %s" % (ultah))
+  print ("[+] Password : %s" % (password))
+  print ("[+] Cookie Akun : %s" % (new_account.get_cookie_str()))
+  print ("[+] Token Akun : %s" % (new_account.get_token()))
+  sys.exit(0)
+else:
+  print ("[!] Gagal Membuat Akun Facebook ")
+  sys.exit(1)
+```
+
+##### Jalankan Program nya
+![Menjalankan script Contoh cara membuat akun Facebook menggunakan library fbthon](https://i.ibb.co/2Sd19Wc/Screenshot-2023-0420-093249.png)
+
+###### Hasilnya 
+Ini adalah akun yang di buat menggunakan library fbthon:)
+
+![Ini adalah akun Facebook yang di buat menggunakan library fbthon](https://i.ibb.co/7K3q3hj/Screenshot-20230420-093826.jpg)
+
+#### Optional Parameter
+*(Untuk `CreateAccount` class)*.
+
+- **firstname**: Nama Depan
+- **lastname**: Nama Belakang
+- **email**: Alamat email yang akan di gunakan untuk mendaftar akun facebook, kamu juga bisa menggunakan nomor ponsel sebagai pengganti alamat email.
+- **gender**: Jenis kelamin (Male/Female)
+- **date_of_birth**: Tanggal lahir, untuk format tanggal lahir nya adalah DD/MM/YYYY, Contoh: 13/01/2006
+- **password**: Kata sandi yang akan di gunakan untuk membuat akun Facebook.
+
+
 # Cara Install
 
 **fbthon** sudah tersedia di PyPi
 
 ```console
 $ python -m pip install fbthon
 ```
 
-**fbthon** bisa install di Python versi 3.7+
+**fbthon** bisa di install di Python versi 3.7+
 
 # Donate
 [![Donate for Rahmat adha](https://i.ibb.co/PwYMWsK/Saweria-Logo.png)](https://saweria.co/rahmatadha)
```

### Comparing `fbthon-0.0.1/setup.py` & `fbthon-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,25 +21,26 @@
 
 with open('README.md','r',encoding = 'utf-8') as doc:
   readme = doc.read()
 
 setup(
   name = 'fbthon',
   packages = ['fbthon'],
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'Simple Facebook scraper',
   long_description=readme,
   long_description_content_type="text/markdown",
   author = 'Rahmat adha',
   author_email = 'rahmadadha11@gmail.com',
   url = 'https://github.com/MR-X-Junior/fbthon',
   keywords = ['facebook-scraper', 'facebook-parser', 'facebook-scraper-without-apikey'],
   python_requires=">=3.7",
   install_requires=[
+          'requests_toolbelt',
           'requests',
           'bs4',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
```

