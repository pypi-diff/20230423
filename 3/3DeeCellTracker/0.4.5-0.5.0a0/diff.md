# Comparing `tmp/3DeeCellTracker-0.4.5.tar.gz` & `tmp/3DeeCellTracker-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3DeeCellTracker-0.4.5.tar", last modified: Mon Jun  6 05:32:00 2022, max compression
+gzip compressed data, was "3DeeCellTracker-0.5.0a0.tar", last modified: Sun Apr 23 06:38:09 2023, max compression
```

## Comparing `3DeeCellTracker-0.4.5.tar` & `3DeeCellTracker-0.5.0a0.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-06-06 05:32:00.773787 3DeeCellTracker-0.4.5/
-drwxrwxrwx   0        0        0        0 2022-06-06 05:32:00.757998 3DeeCellTracker-0.4.5/3DeeCellTracker.egg-info/
--rw-rw-rw-   0        0        0     6327 2022-06-06 05:32:00.000000 3DeeCellTracker-0.4.5/3DeeCellTracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2022-06-06 05:32:00.000000 3DeeCellTracker-0.4.5/3DeeCellTracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-06 05:32:00.000000 3DeeCellTracker-0.4.5/3DeeCellTracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-06-06 05:32:00.000000 3DeeCellTracker-0.4.5/3DeeCellTracker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-06-06 05:32:00.772785 3DeeCellTracker-0.4.5/CellTracker/
--rw-rw-rw-   0        0        0        0 2022-06-03 04:27:27.000000 3DeeCellTracker-0.4.5/CellTracker/__init__.py
--rw-rw-rw-   0        0        0     4710 2022-06-06 05:30:44.000000 3DeeCellTracker-0.4.5/CellTracker/analyses.py
--rw-rw-rw-   0        0        0     5522 2022-06-06 05:29:07.000000 3DeeCellTracker-0.4.5/CellTracker/preprocess.py
--rw-rw-rw-   0        0        0    24004 2022-06-06 05:29:07.000000 3DeeCellTracker-0.4.5/CellTracker/track.py
--rw-rw-rw-   0        0        0    71728 2022-06-06 05:29:07.000000 3DeeCellTracker-0.4.5/CellTracker/tracker.py
--rw-rw-rw-   0        0        0    25362 2022-06-06 05:29:07.000000 3DeeCellTracker-0.4.5/CellTracker/unet3d.py
--rw-rw-rw-   0        0        0     4845 2022-06-06 05:29:07.000000 3DeeCellTracker-0.4.5/CellTracker/watershed.py
--rw-rw-rw-   0        0        0     1089 2022-04-07 05:05:46.000000 3DeeCellTracker-0.4.5/LICENSE
--rw-rw-rw-   0        0        0     6327 2022-06-06 05:32:00.772785 3DeeCellTracker-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     5906 2022-06-06 05:30:44.000000 3DeeCellTracker-0.4.5/README.md
--rw-rw-rw-   0        0        0       42 2022-06-06 05:32:00.773787 3DeeCellTracker-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      656 2022-06-06 05:30:44.000000 3DeeCellTracker-0.4.5/setup.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/
+-rw-rw-r--   0 wen       (1000) wen       (1000)     7899 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/PKG-INFO
+-rw-rw-r--   0 wen       (1000) wen       (1000)      569 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)        1 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)      166 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/requires.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)       12 2023-04-23 06:38:09.000000 3DeeCellTracker-0.5.0a0/3DeeCellTracker.egg-info/top_level.txt
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/CellTracker/
+-rw-rw-r--   0 wen       (1000) wen       (1000)        0 2023-04-07 02:12:11.000000 3DeeCellTracker-0.5.0a0/CellTracker/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4598 2023-04-22 01:33:34.000000 3DeeCellTracker-0.5.0a0/CellTracker/analyses.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    22903 2023-04-22 08:31:03.000000 3DeeCellTracker-0.5.0a0/CellTracker/coord_image_transformer.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    11593 2023-04-22 07:34:57.000000 3DeeCellTracker-0.5.0a0/CellTracker/ffn.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     5332 2023-04-21 05:33:48.000000 3DeeCellTracker-0.5.0a0/CellTracker/preprocess.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    12898 2023-04-18 05:44:06.000000 3DeeCellTracker-0.5.0a0/CellTracker/stardist3dcustom.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13105 2023-04-23 05:04:40.000000 3DeeCellTracker-0.5.0a0/CellTracker/stardistwrapper.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     3302 2023-04-14 05:41:05.000000 3DeeCellTracker-0.5.0a0/CellTracker/synthesize.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    23398 2023-04-21 05:29:47.000000 3DeeCellTracker-0.5.0a0/CellTracker/track.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    70284 2023-04-21 06:12:02.000000 3DeeCellTracker-0.5.0a0/CellTracker/tracker.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    20911 2023-04-22 09:18:38.000000 3DeeCellTracker-0.5.0a0/CellTracker/trackerlite.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    24761 2023-04-07 02:12:11.000000 3DeeCellTracker-0.5.0a0/CellTracker/unet3d.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     5756 2023-04-19 05:03:09.000000 3DeeCellTracker-0.5.0a0/CellTracker/watershed.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1068 2023-04-07 02:12:11.000000 3DeeCellTracker-0.5.0a0/LICENSE
+-rw-rw-r--   0 wen       (1000) wen       (1000)     7899 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/PKG-INFO
+-rw-rw-r--   0 wen       (1000) wen       (1000)     7414 2023-04-23 04:52:37.000000 3DeeCellTracker-0.5.0a0/README.md
+-rw-rw-r--   0 wen       (1000) wen       (1000)      720 2023-04-23 06:38:09.664312 3DeeCellTracker-0.5.0a0/setup.cfg
+-rw-rw-r--   0 wen       (1000) wen       (1000)       38 2023-04-23 06:38:07.000000 3DeeCellTracker-0.5.0a0/setup.py
```

### Comparing `3DeeCellTracker-0.4.5/3DeeCellTracker.egg-info/PKG-INFO` & `3DeeCellTracker-0.5.0a0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,123 @@
-Metadata-Version: 2.1
-Name: 3DeeCellTracker
-Version: 0.4.5
-Summary: A package for tracking cells in 3D time lapse images
-Home-page: https://github.com/WenChentao/3DeeCellTracker
-Author: Chentao Wen
-Author-email: chintou.on@gmail.com
-Classifier: Programming Language :: Python
-Classifier: Environment :: GPU :: NVIDIA CUDA
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# 3DeeCellTracker
-[![PyPI](https://img.shields.io/pypi/v/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![GitHub](https://img.shields.io/github/license/WenChentao/3DeeCellTracker)](https://github.com/WenChentao/3DeeCellTracker/blob/master/LICENSE)
-[![Youtube](https://img.shields.io/badge/YouTube-Demo-red)](https://www.youtube.com/watch?v=ctt6o3DY2bA&list=PLGY0oNQomrHERP08iEj-MsluFW8xQJujP)
-
-**3DeeCellTracker** is a deep-learning based pipeline for tracking cells in 3D time lapse images of deforming/moving organs ([eLife, 2021](https://elifesciences.org/articles/59187)).
-
-## Updates:
-
-**3DeeCellTracker v0.4.5 was released with following issues fixed (2022.06.03)**
-- Solved an activity load bug.
-
-## Installation
-
-* Create a conda environment for a PC with GPU including prerequisite packages using the 3DCT.yml file:
-
-```console
-$ conda env create -f 3DCT.yml
-```
-
-* (NOT RECOMMEND) Users can create a conda environment for a PC with only CPU, but it will be slow and may fail.
-```console
-$ conda env create -f 3DCT-CPU.yml
-```
-
-* Install the 3DeeCellTracker package solely by pip
-
-```console
-$ pip install 3DeeCellTracker
-```
-
-* Update the 3DeeCellTracker package to the latest version
-
-```console
-$ pip install --upgrade 3DeeCellTracker
-```
-
-For detailed instructions, see [here](Doc/Enviroment.md).
-## Quick Start
-To learn how to track cells use 3DeeCellTracker, see following notebooks for examples:
-1. Track cells in deforming organs: 
-    - [**Single mode (clear notebook)**](Examples/single_mode_worm1-clear.ipynb);
-    - [**single mode (results)**](https://wenchentao.github.io//3DeeCellTracker/Examples/single_mode_worm1.html)
-
-
-2. Track cells in freely moving animals: 
-    - [**Ensemble mode (clear notebook)**](Examples/ensemble_mode_worm4-clear.ipynb)
-    - [**Ensemble mode (results)**](https://wenchentao.github.io//3DeeCellTracker/Examples/ensemble_mode_worm4.html)
-
-
-3. Train a new 3D U-Net for segmenting cells in new optical conditions: 
-    - [**Train 3D U-Net (clear notebook)**](Examples/3D_U_Net_training-clear.ipynb).
-    - [**Train 3D U-Net (results)**](https://wenchentao.github.io//3DeeCellTracker/Examples/3D_U_Net_training.html).
-   
-The data and model files for demonstrating above notebooks can be downloaded [**here**](https://osf.io/dt76c/).
-
-**Note**: Codes above were based on the latest version. 
-For old programs used in eLife 2021, please check the "[**Deprecated_programs**](Deprecated_programs)" folder.
-
-## Video Tutorials
-We have made tutorials explaining how to use our software. See links below (videos in Youtube):
-
-[Tutorial 1: Install 3DeeCellTracker and train the 3D U-Net](https://www.youtube.com/watch?v=ctt6o3DY2bA)
-
-[Tutorial 2: Tracking cells by 3DeeCellTracker](https://www.youtube.com/watch?v=KZ03Y8u8UK0)
-
-[Tutorial 3: Annotate cells for training 3D U-Net](https://www.youtube.com/watch?v=ONSOLJQaq28)
-
-[Tutorial 4: Manually correct the cell segmentation](https://www.youtube.com/watch?v=e7xWaccH63o)
-
-## A Text Tutorial 
-We have wrote a tutorial explaining how to install and use 3DeeCellTracker. See [Bio-protocol, 2022](https://bio-protocol.org/e4319)
-
-## How it works
-We designed this pipeline for segmenting and tracking cells in 3D + T images in deforming organs. The methods have been explained in [Wen et al. bioRxiv 2018]( https://doi.org/10.1101/385567) and in [Wen et al. eLife, 2021](https://elifesciences.org/articles/59187).
-
-**Overall procedures of our method** ([Wen et al. eLife, 2021–Figure 1](https://elifesciences.org/articles/59187/figures#content))
-
-<img src="https://iiif.elifesciences.org/lax:59187%2Felife-59187-fig1-v1.tif/full/1500,/0/default.jpg" width="400">
-
-**Examples of tracking results** ([Wen et al. eLife, 2021–Videos](https://elifesciences.org/articles/59187/figures#content))
-
-| [Neurons in a ‘straightened’ <br />freely moving worm](https://static-movie-usa.glencoesoftware.com/mp4/10.7554/5/4ce9eaa4a84bf7847c99c81a13ccafd797b40218/elife-59187-fig6-video1.mp4)| [Cardiac cells in a zebrafish larva](https://static-movie-usa.glencoesoftware.com/mp4/10.7554/5/4ce9eaa4a84bf7847c99c81a13ccafd797b40218/elife-59187-fig7-video2.mp4) | [Cells in a 3D tumor spheriod](https://static-movie-usa.glencoesoftware.com/mp4/10.7554/5/4ce9eaa4a84bf7847c99c81a13ccafd797b40218/elife-59187-fig8-video2.mp4) |
-| ------------- | ------------- | ------------- | 
-| <img src="https://user-images.githubusercontent.com/27986173/115169952-63b4e600-a0fa-11eb-9b85-91292bc9d419.gif" width="340">| <img src="https://user-images.githubusercontent.com/27986173/115170418-90b5c880-a0fb-11eb-9382-13690c3375dc.gif" width="400">| <img src="https://user-images.githubusercontent.com/27986173/115170434-9ad7c700-a0fb-11eb-9004-2e4cff86f7ab.gif" width="200">|
-
-
-## Citation
-
-If you used this package in your research and is interested in citing it here's how you do it:
-
-```
-@article{
-author = {Wen, Chentao and Miura, Takuya and Voleti, Venkatakaushik and Yamaguchi, Kazushi and Tsutsumi, Motosuke and Yamamoto, Kei and Otomo, Kohei and Fujie, Yukako and Teramoto, Takayuki and Ishihara, Takeshi and Aoki, Kazuhiro and Nemoto, Tomomi and Hillman, Elizabeth MC and Kimura, Koutarou D},
-doi = {10.7554/eLife.59187},
-journal = {eLife},
-month = {mar},
-title = {{3DeeCellTracker, a deep learning-based pipeline for segmenting and tracking cells in 3D time lapse images}},
-volume = {10},
-year = {2021}
-}
-```
-
-## Acknowledgements
-We wish to thank **JetBrains** for supporting this project 
-with free open source **Pycharm** license.
-
-[![Pycharm Logo](pictures/jetbrains_small.png)](https://www.jetbrains.com/) 
-[![Pycharm Logo](pictures/icon-pycharm_small.png)](https://www.jetbrains.com/pycharm/)
+# 3DeeCellTracker
+[![PyPI](https://img.shields.io/pypi/v/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/3DeeCellTracker)](https://pypi.org/project/3DeeCellTracker/) [![GitHub](https://img.shields.io/github/license/WenChentao/3DeeCellTracker)](https://github.com/WenChentao/3DeeCellTracker/blob/master/LICENSE)
+[![Youtube](https://img.shields.io/badge/YouTube-Demo-red)](https://www.youtube.com/watch?v=ctt6o3DY2bA&list=PLGY0oNQomrHERP08iEj-MsluFW8xQJujP)
+
+**3DeeCellTracker** is a deep-learning based pipeline for tracking cells in 3D time lapse images of deforming/moving organs ([eLife, 2021](https://elifesciences.org/articles/59187)).
+
+## Updates:
+
+**3DeeCellTracker v0.5.0-alpha will be released soon**
+- Allows you to use [StarDist3D](https://github.com/stardist/stardist) for segmentation
+- Reduces the requirements for fine-tuning parameters
+- Decouples the code to facilitate reuse by third-party developers.
+
+## Installation
+
+To install 3DeeCellTracker, please follow the instructions below:
+
+### Prerequisites
+- A computer with an NVIDIA GPU that supports CUDA.
+- [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://conda.io/miniconda.html) installed.
+
+### Steps
+1. Create a new conda environment and activate it by running the following commands in your terminal:
+
+   ```console
+   $ conda create -n track python=3.8 pip
+   $ conda activate track
+   ```
+   
+2. Install [TensorFlow](https://www.tensorflow.org/install).
+3. Install 3DeeCellTracker by running the following command in your terminal:
+   ```console
+   $ pip install 3DeeCellTracker
+   ```
+   After completing the installation steps, you can start using 3DeeCellTracker for your 3D cell tracking tasks within 
+   the jupyter notebooks we have provided (See below). 
+   If you encounter any issues or have any questions, please refer to the project's documentation 
+   or raise an issue in the GitHub repository.
+
+## Quick Start
+To learn how to track cells using 3DeeCellTracker, please refer to the following notebooks for examples. 
+We recommend using StarDist for segmentation, as we have optimized the StarDist-based tracking programs for more convenient and quick cell tracking.
+1. Train a custom deep neural network for segmenting cells in new optical conditions: 
+    - [**Train 3D StarDist (notebook with results)**](Examples/use_stardist/train_stardist.ipynb)
+    - [**Train 3D U-Net (clear notebook)**](Examples/use_unet/3D_U_Net_training-clear.ipynb).
+    - [**Train 3D U-Net (results)**](https://wenchentao.github.io//3DeeCellTracker/Examples/use_unet/3D_U_Net_training.html).
+ 
+2. Track cells in deforming organs: 
+    - [**Single mode + StarDist (notebook with results)**](Examples/use_stardist/track_worm1_stardist_single_mode.ipynb);
+    - [**Single mode + UNet (clear notebook)**](Examples/use_unet/single_mode_worm1-clear.ipynb);
+    - [**single mode + UNet (results)**](https://wenchentao.github.io//3DeeCellTracker/Examples/use_unet/single_mode_worm1.html)
+
+3. Track cells in freely moving animals: 
+    - [**Ensemble mode + StarDist (notebook with results)**](Examples/use_stardist/track_worm4_stardist_ensemble_mode.ipynb);
+    - [**Ensemble mode + UNet (clear notebook)**](Examples/use_unet/ensemble_mode_worm4-clear.ipynb)
+    - [**Ensemble mode + UNet (results)**](https://wenchentao.github.io//3DeeCellTracker/Examples/use_unet/ensemble_mode_worm4.html)
+
+   
+The data and model files for demonstrating above notebooks can be downloaded here: 
+- [**StarDist-based notebooks**](https://osf.io/pgr95/).
+- [**UNet-based notebooks**](https://osf.io/dt76c/).
+
+
+**Note**: Codes above were based on the latest version. 
+For old programs used in eLife 2021, please check the "[**Deprecated_programs**](Deprecated_programs)" folder.
+
+## Frequently Reported Issue and Solution (for v0.4)
+
+Multiple users have reported encountering a `ValueError` of shape mismatch when running the `tracker.match()` function. 
+After investigation, it was found that the issue resulted from an incorrect setting of `siz_xyz`, 
+which should be set to the dimensions of the 3D image as (height, width, depth). 
+
+
+## Video Tutorials (for v0.4)
+We have made tutorials explaining how to use our software. See links below (videos in Youtube):
+
+[Tutorial 1: Install 3DeeCellTracker and train the 3D U-Net](https://www.youtube.com/watch?v=ctt6o3DY2bA)
+
+[Tutorial 2: Tracking cells by 3DeeCellTracker](https://www.youtube.com/watch?v=KZ03Y8u8UK0)
+
+[Tutorial 3: Annotate cells for training 3D U-Net](https://www.youtube.com/watch?v=ONSOLJQaq28)
+
+[Tutorial 4: Manually correct the cell segmentation](https://www.youtube.com/watch?v=e7xWaccH63o)
+
+## A Text Tutorial (for v0.4)
+We have written a tutorial explaining how to install and use 3DeeCellTracker. See [Bio-protocol, 2022](https://bio-protocol.org/e4319)
+
+## How it works
+We designed this pipeline for segmenting and tracking cells in 3D + T images in deforming organs. The methods have been explained in [Wen et al. bioRxiv 2018]( https://doi.org/10.1101/385567) and in [Wen et al. eLife, 2021](https://elifesciences.org/articles/59187).
+
+**Overall procedures of our method** ([Wen et al. eLife, 2021–Figure 1](https://elifesciences.org/articles/59187/figures#content))
+
+<img src="https://iiif.elifesciences.org/lax:59187%2Felife-59187-fig1-v1.tif/full/1500,/0/default.jpg" width="400">
+
+**Examples of tracking results** ([Wen et al. eLife, 2021–Videos](https://elifesciences.org/articles/59187/figures#content))
+
+| [Neurons in a ‘straightened’ <br />freely moving worm](https://static-movie-usa.glencoesoftware.com/mp4/10.7554/5/4ce9eaa4a84bf7847c99c81a13ccafd797b40218/elife-59187-fig6-video1.mp4)| [Cardiac cells in a zebrafish larva](https://static-movie-usa.glencoesoftware.com/mp4/10.7554/5/4ce9eaa4a84bf7847c99c81a13ccafd797b40218/elife-59187-fig7-video2.mp4) | [Cells in a 3D tumor spheriod](https://static-movie-usa.glencoesoftware.com/mp4/10.7554/5/4ce9eaa4a84bf7847c99c81a13ccafd797b40218/elife-59187-fig8-video2.mp4) |
+| ------------- | ------------- | ------------- | 
+| <img src="https://user-images.githubusercontent.com/27986173/115169952-63b4e600-a0fa-11eb-9b85-91292bc9d419.gif" width="340">| <img src="https://user-images.githubusercontent.com/27986173/115170418-90b5c880-a0fb-11eb-9382-13690c3375dc.gif" width="400">| <img src="https://user-images.githubusercontent.com/27986173/115170434-9ad7c700-a0fb-11eb-9004-2e4cff86f7ab.gif" width="200">|
+
+
+## Citation
+
+If you used this package in your research and is interested in citing it here's how you do it:
+
+```
+@article{
+author = {Wen, Chentao and Miura, Takuya and Voleti, Venkatakaushik and Yamaguchi, Kazushi and Tsutsumi, Motosuke and Yamamoto, Kei and Otomo, Kohei and Fujie, Yukako and Teramoto, Takayuki and Ishihara, Takeshi and Aoki, Kazuhiro and Nemoto, Tomomi and Hillman, Elizabeth MC and Kimura, Koutarou D},
+doi = {10.7554/eLife.59187},
+journal = {eLife},
+month = {mar},
+title = {{3DeeCellTracker, a deep learning-based pipeline for segmenting and tracking cells in 3D time lapse images}},
+volume = {10},
+year = {2021}
+}
+```
+
+## Acknowledgements
+We wish to thank **JetBrains** for supporting this project 
+with free open source **Pycharm** license.
+
+[![Pycharm Logo](pictures/jetbrains_small.png)](https://www.jetbrains.com/) 
+[![Pycharm Logo](pictures/icon-pycharm_small.png)](https://www.jetbrains.com/pycharm/)
```

### Comparing `3DeeCellTracker-0.4.5/CellTracker/analyses.py` & `3DeeCellTracker-0.5.0a0/CellTracker/analyses.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,142 +1,143 @@
-"""
-A module for analyses after tracking
-Author: Chentao Wen
-
-"""
-
-import numpy as np
-import matplotlib.pyplot as plt
-import cv2
-import matplotlib as mpl
-
-mpl.rcParams["axes.spines.right"] = False
-mpl.rcParams["axes.spines.top"] = False
-
-def get_activities(path_raw, path_tracked, volume_num, layer_num):
-    """
-    Get activities of all cells
-
-    Parameters
-    ----------
-    path_raw : str
-        The path of the images for extracting activities
-    path_tracked : str
-        The path of the tracked labels
-    volume_num : int
-        The number of the volumes
-    layer_num : int
-        the number of layers in the raw images and the tracked labels
-
-    Returns
-    -------
-    activities : numpy.ndarray
-        The extracted activities with shape (volume, label)
-    """
-    images_label, images_raw = _read_image(1, layer_num, path_raw, path_tracked)
-    cell_num = np.max(images_label)
-    activities = np.zeros((volume_num, cell_num))
-    discard_ratio = 0.1
-    for frame in range(1, volume_num + 1):
-
-        print("t=%i"%frame, end="\r")
-
-        # read raw images and labels
-        if frame>=2:
-            images_label, images_raw = _read_image(frame, layer_num, path_raw, path_tracked)
-
-        # calculate mean intensities of each cell of top 90% area
-        for label in range(1, cell_num + 1):
-            intensity_label_i = images_raw[images_label==label]
-            threshold = np.floor(np.size(intensity_label_i) * discard_ratio).astype(int)
-            sorted_intensity_idx = np.argsort(intensity_label_i)
-            activities[frame-1, label-1] = np.mean(intensity_label_i[sorted_intensity_idx[threshold:]])
-    return activities
-
-
-def _read_image(frame, layer_num, path_raw, path_tracked):
-    """Read 3D images of raw activities and tracked labels"""
-    images_raw = []
-    images_label = []
-    for z in range(1, layer_num + 1):
-        images_raw.append(cv2.imread(path_raw % (frame, z), -1))
-        images_label.append(cv2.imread(path_tracked % (frame, z), -1))
-    images_raw = np.array(images_raw)
-    images_label = np.array(images_label)
-    return images_label, images_raw
-
-
-def optimize_row_column(duration, n_signals, figsize):
-    """
-    Return the proper number of row, column for visualization
-
-    Parameters
-    ----------
-    duration : int
-        Number of time points for each signal.
-    n_signals : int
-        Number of signals.
-    figsize : tuple
-        size of the figure to show activities
-
-    Returns
-    -------
-    row_n : int
-        Number of row
-    column_n : int
-        Number of column
-
-    Notes
-    -----
-    The row_n and colume_n are designed to make sure the xy_ratio of each subplot propotional with duration.
-
-    Examples
-    --------
-    >>> optimize_row_column(duration=200, n_signals=100, figsize=(40, 20))
-    (14, 8)
-    """
-    width_hight_ratio = figsize[0]/figsize[1]
-    total_length = duration * n_signals
-    row_n = int((total_length / (50 * width_hight_ratio)) ** 0.5)
-    column_n = int(np.ceil(n_signals / row_n))
-    return row_n, column_n
-
-
-def draw_signals(signals, ylim_upper=None, ylim_lower=None, figsize=(40, 20)):
-    """
-    Draw signals in multiple subplots
-
-    Parameters
-    ----------
-    signals : numpy.ndarray
-        N Signals with T time points with shape (T, N)
-    ylim_upper : float
-        ylim upper bound. If None, set it to the highest value.
-    ylim_lower : float
-        ylim lower bound. If None, set it to the lowest value.
-    figsize : tuple
-        Size of the figure
-
-    Returns
-    -------
-    fig : matplotlib.figure
-    axes : array of matplotlib.axes.Axes
-    """
-    row_n, column_n = optimize_row_column(signals.shape[0], signals.shape[1], figsize)
-    fig, axes = plt.subplots(row_n, column_n, figsize=figsize)
-    for row in range(row_n):
-        for column in range(column_n):
-            n = row * column_n + column
-            if n >= signals.shape[1]:
-                break
-            axes[row, column].plot(signals[:, n], lw=2)
-            upper_sig_n, lower_sig_n = np.nanmax(signals[:, n]), np.nanmin(signals[:, n])
-            if ylim_upper is not None:
-                upper_sig_n = ylim_upper
-            if ylim_lower is not None:
-                lower_sig_n = ylim_lower
-            axes[row, column].set_ylim(lower_sig_n, upper_sig_n)
-            axes[row, column].set_title("N%d" % (n + 1), va="top")
-            if row<row_n-1:
-                axes[row, column].get_xaxis().set_visible(False)
-    plt.subplots_adjust(left=0.02, bottom=0.02, right=0.98, top=0.98, wspace=0.2, hspace=0.2)
-    return fig, axes
+"""
+A module for analyses after tracking
+Author: Chentao Wen
+
+"""
+
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+from tifffile import imread
+
+mpl.rcParams["axes.spines.right"] = False
+mpl.rcParams["axes.spines.top"] = False
+
+
+def get_activities(raw_path: str, tracked_labels_path: str, volume_num: int, layer_num: int):
+    """
+    Get activities of all cells
+
+    Parameters
+    ----------
+    raw_path : str
+        The path of the images for extracting activities
+    tracked_labels_path : str
+        The path of the tracked labels
+    volume_num : int
+        The number of the volumes
+    layer_num : int
+        the number of layers in the raw images and the tracked labels
+
+    Returns
+    -------
+    activities : numpy.ndarray
+        The extracted activities with shape (volume, label)
+    """
+    images_label, images_raw = _read_image(1, layer_num, raw_path, tracked_labels_path)
+    cell_num = np.max(images_label)
+    activities = np.zeros((volume_num, cell_num))
+    discard_ratio = 0.1
+    for frame in range(1, volume_num + 1):
+
+        print("t=%i"%frame, end="\r")
+
+        # read raw images and labels
+        if frame>=2:
+            images_label, images_raw = _read_image(frame, layer_num, raw_path, tracked_labels_path)
+
+        # calculate mean intensities of each cell of top 90% area
+        for label in range(1, cell_num + 1):
+            intensity_label_i = images_raw[images_label==label]
+            threshold = np.floor(np.size(intensity_label_i) * discard_ratio).astype(int)
+            sorted_intensity_idx = np.argsort(intensity_label_i)
+            activities[frame-1, label-1] = np.mean(intensity_label_i[sorted_intensity_idx[threshold:]])
+    return activities
+
+
+def _read_image(frame, layer_num, path_raw, path_tracked):
+    """Read 3D images of raw activities and tracked labels"""
+    images_raw = []
+    images_label = []
+    for z in range(1, layer_num + 1):
+        images_raw.append(imread(path_raw % (frame, z)))
+        images_label.append(imread(path_tracked % (frame, z)))
+    images_raw = np.array(images_raw)
+    images_label = np.array(images_label)
+    return images_label, images_raw
+
+
+def optimize_row_column(duration, n_signals, figsize):
+    """
+    Return the proper number of row, column for visualization
+
+    Parameters
+    ----------
+    duration : int
+        Number of time points for each signal.
+    n_signals : int
+        Number of signals.
+    figsize : tuple
+        size of the figure to show activities
+
+    Returns
+    -------
+    row_n : int
+        Number of row
+    column_n : int
+        Number of column
+
+    Notes
+    -----
+    The row_n and colume_n are designed to make sure the xy_ratio of each subplot propotional with duration.
+
+    Examples
+    --------
+    >>> optimize_row_column(duration=200, n_signals=100, figsize=(40, 20))
+    (14, 8)
+    """
+    width_hight_ratio = figsize[0]/figsize[1]
+    total_length = duration * n_signals
+    row_n = int((total_length / (50 * width_hight_ratio)) ** 0.5)
+    column_n = int(np.ceil(n_signals / row_n))
+    return row_n, column_n
+
+
+def draw_signals(signals, ylim_upper=None, ylim_lower=None, figsize=(20, 10)):
+    """
+    Draw signals in multiple subplots
+
+    Parameters
+    ----------
+    signals : numpy.ndarray
+        N Signals with T time points with shape (T, N)
+    ylim_upper : float
+        ylim upper bound. If None, set it to the highest value.
+    ylim_lower : float
+        ylim lower bound. If None, set it to the lowest value.
+    figsize : tuple
+        Size of the figure
+
+    Returns
+    -------
+    fig : matplotlib.figure
+    axes : array of matplotlib.axes.Axes
+    """
+    row_n, column_n = optimize_row_column(signals.shape[0], signals.shape[1], figsize)
+    fig, axes = plt.subplots(row_n, column_n, figsize=figsize)
+    for row in range(row_n):
+        for column in range(column_n):
+            n = row * column_n + column
+            if n >= signals.shape[1]:
+                break
+            axes[row, column].plot(signals[:, n], lw=2)
+            upper_sig_n, lower_sig_n = np.nanmax(signals[:, n]), np.nanmin(signals[:, n])
+            if ylim_upper is not None:
+                upper_sig_n = ylim_upper
+            if ylim_lower is not None:
+                lower_sig_n = ylim_lower
+            axes[row, column].set_ylim(lower_sig_n, upper_sig_n)
+            axes[row, column].set_title("N%d" % (n + 1), va="top")
+            if row<row_n-1:
+                axes[row, column].get_xaxis().set_visible(False)
+    plt.subplots_adjust(left=0.02, bottom=0.02, right=0.98, top=0.98, wspace=0.2, hspace=0.2)
+
```

### Comparing `3DeeCellTracker-0.4.5/CellTracker/preprocess.py` & `3DeeCellTracker-0.5.0a0/CellTracker/preprocess.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,204 +1,205 @@
-"""
-A module for preprocessing of 3D cell images
-Author: Chentao Wen
-
-"""
-import os
-import cv2
-from scipy import ndimage
-import numpy as np
-from tensorflow.keras.models import Model
-from tensorflow.keras.layers import Conv3D, Input
-import tensorflow.keras as keras
-
-
-def _make_folder(path_i, print_=True):
-    """
-    Make a folder
-
-    Parameters
-    ----------
-    path_i : str
-         The folder path
-    print_ : bool, optional
-        If True, print the relative path of the created folder. Default: True
-
-    Returns
-    -------
-    path_i : str
-        The folder path
-    """
-    if not os.path.exists(path_i):
-        os.makedirs(path_i)
-    if print_:
-        print(os.path.relpath(path_i, os.getcwd()))
-    return path_i
-
-
-def _get_files(folder_path):
-    """
-    Get paths of all files in the folder
-
-    Parameters
-    ----------
-    folder_path : str
-        The path of the folder containing images
-
-    Returns
-    -------
-    img_path : list
-        A list of the file paths in the folder
-    """
-    img_path = []
-    for img_filename in sorted(os.listdir(folder_path)):
-        img_path.append(folder_path + "/" + img_filename)
-    return img_path
-
-
-def load_image(folder_path, print_=True):
-    """
-    Load a 3D image from 2D layers (without time information)
-
-    Parameters
-    ----------
-    folder_path : str
-        The path of the folder containing images
-    print_ : int, optional
-        If True, print the shape of the loaded 3D image. Default: True
-
-    Returns
-    -------
-    img_array : numpy.ndarray
-        The 3D array of the loaded image
-    """
-    img_file_path = _get_files(folder_path)
-    img = []
-    for img_path in img_file_path:
-        img.append(cv2.imread(img_path, -1))
-    img_array = np.array(img).transpose((1, 2, 0))
-    if print_:
-        print("Load images with shape:", img_array.shape)
-    return img_array
-
-
-def lcn_cpu(img3d, noise_level, filter_size=(27, 27, 1)):
-    """
-    Local contrast normalization by cpu
-    
-    Parameters
-    ----------
-    img3d : numpy.ndarray
-        The raw 3D image
-    noise_level : float
-        The parameter to suppress the enhancement of the background noises
-    filter_size : tuple, optional
-        the window size to apply the normalization along x, y, and z axis. Default: (27, 27, 1)
-
-    Returns
-    -------
-    norm : numpy.ndarray
-        The normalized 3D image
-
-    Notes
-    -----
-    The normalization in the edge regions used "reflect" padding, which is different with
-    the lcn_gpu function (uses zero padding).
-    """
-    filter = np.ones(filter_size)
-    filter = filter / filter.size
-    avg = ndimage.convolve(img3d, filter, mode='reflect')
-    diff_sqr = np.square(img3d - avg)
-    std = np.sqrt(ndimage.convolve(diff_sqr, filter, mode='reflect'))
-    norm = np.divide(img3d - avg, std + noise_level)
-    return norm
-
-
-def conv3d_keras(filter_size, img3d_siz):
-    """
-    Generate a keras model for applying 3D convolution
-
-    Parameters
-    ----------
-    filter_size : tuple
-    img3d_siz : tuple
-
-    Returns
-    -------
-    keras.Model
-        The keras model to apply 3D convolution
-    """
-    inputs = Input((img3d_siz[0], img3d_siz[1], img3d_siz[2], 1))
-    conv_3d = Conv3D(1, filter_size, kernel_initializer=keras.initializers.Ones(), padding='same')(inputs)
-    return Model(inputs=inputs, outputs=conv_3d)
-
-
-def lcn_gpu(img3d, noise_level=5, filter_size=(27, 27, 1)):
-    """
-    Local contrast normalization by gpu
-
-    Parameters
-    ----------
-    img3d : numpy.ndarray
-        The raw 3D image
-    noise_level : float
-        The parameter to suppress the enhancement of the background noises
-    filter_size : tuple, optional
-        the window size to apply the normalization along x, y, and z axis. Default: (27, 27, 1)
-
-    Returns
-    -------
-    norm : numpy.ndarray
-        The normalized 3D image
-
-    Notes
-    -----
-    The normalization in the edge regions currently used zero padding based on keras.Conv3D function,
-    which is different with the lcn_cpu function (uses "reflect" padding).
-    """
-    img3d_siz = img3d.shape
-    volume = filter_size[0] * filter_size[1] * filter_size[2]
-    conv3d_model = conv3d_keras(filter_size, img3d_siz)
-    img3d = np.expand_dims(img3d, axis=(0,4))
-    avg = conv3d_model.predict(img3d) / volume
-    diff_sqr = np.square(img3d - avg)
-    std = np.sqrt(conv3d_model.predict(diff_sqr) / volume)
-    norm = np.divide(img3d - avg, std + noise_level)
-    return norm[0, :, :, :, 0]
-
-
-def _normalize_image(image, noise_level):
-    """
-    Normalize an 3D image by local contrast normalization
-
-    Parameters
-    ----------
-    image : numpy.ndarray
-        A 3D image to be normalized
-    noise_level : float
-        The parameter to suppress the enhancement of the background noises
-
-    Returns
-    -------
-    numpy.ndarray
-        The normalized image
-    """
-    image_norm = image - np.median(image)
-    image_norm[image_norm < 0] = 0
-    return lcn_gpu(image_norm, noise_level, filter_size=(27, 27, 1))
-
-
-def _normalize_label(label_img):
-    """
-    Transform cell/non-cell image into binary (0/1)
-
-    Parameters
-    ----------
-    label_img : numpy.ndarray
-        Input image of cell/non-cell regions
-
-    Returns
-    -------
-    numpy.ndarray
-        The binarized image
-    """
+"""
+A module for preprocessing of 3D cell images
+Author: Chentao Wen
+
+"""
+import os
+
+import numpy as np
+import tensorflow.keras as keras
+from scipy import ndimage
+from tensorflow.keras.layers import Conv3D, Input
+from tensorflow.keras.models import Model
+from tifffile import imread
+
+
+def _make_folder(path_i, print_=True):
+    """
+    Make a folder
+
+    Parameters
+    ----------
+    path_i : str
+         The folder path
+    print_ : bool, optional
+        If True, print the relative path of the created folder. Default: True
+
+    Returns
+    -------
+    path_i : str
+        The folder path
+    """
+    if not os.path.exists(path_i):
+        os.makedirs(path_i)
+    if print_:
+        print(os.path.relpath(path_i, os.getcwd()))
+    return path_i
+
+
+def _get_files(folder_path):
+    """
+    Get paths of all files in the folder
+
+    Parameters
+    ----------
+    folder_path : str
+        The path of the folder containing images
+
+    Returns
+    -------
+    img_path : list
+        A list of the file paths in the folder
+    """
+    img_path = []
+    for img_filename in sorted(os.listdir(folder_path)):
+        img_path.append(folder_path + "/" + img_filename)
+    return img_path
+
+
+def load_image(folder_path, print_=True):
+    """
+    Load a 3D image from 2D layers (without time information)
+
+    Parameters
+    ----------
+    folder_path : str
+        The path of the folder containing images
+    print_ : int, optional
+        If True, print the shape of the loaded 3D image. Default: True
+
+    Returns
+    -------
+    img_array : numpy.ndarray
+        The 3D array of the loaded image
+    """
+    img_file_path = _get_files(folder_path)
+    img = []
+    for img_path in img_file_path:
+        img.append(imread(img_path))
+    img_array = np.array(img).transpose((1, 2, 0))
+    if print_:
+        print("Load images with shape:", img_array.shape)
+    return img_array
+
+
+def lcn_cpu(img3d, noise_level, filter_size=(27, 27, 1)):
+    """
+    Local contrast normalization by cpu
+    
+    Parameters
+    ----------
+    img3d : numpy.ndarray
+        The raw 3D image
+    noise_level : float
+        The parameter to suppress the enhancement of the background noises
+    filter_size : tuple, optional
+        the window size to apply the normalization along x, y, and z axis. Default: (27, 27, 1)
+
+    Returns
+    -------
+    norm : numpy.ndarray
+        The normalized 3D image
+
+    Notes
+    -----
+    The normalization in the edge regions used "reflect" padding, which is different with
+    the lcn_gpu function (uses zero padding).
+    """
+    filter = np.ones(filter_size)
+    filter = filter / filter.size
+    avg = ndimage.convolve(img3d, filter, mode='reflect')
+    diff_sqr = np.square(img3d - avg)
+    std = np.sqrt(ndimage.convolve(diff_sqr, filter, mode='reflect'))
+    norm = np.divide(img3d - avg, std + noise_level)
+    return norm
+
+
+def conv3d_keras(filter_size, img3d_siz):
+    """
+    Generate a keras model for applying 3D convolution
+
+    Parameters
+    ----------
+    filter_size : tuple
+    img3d_siz : tuple
+
+    Returns
+    -------
+    tf.keras.Model
+        The keras model to apply 3D convolution
+    """
+    inputs = Input((img3d_siz[0], img3d_siz[1], img3d_siz[2], 1))
+    conv_3d = Conv3D(1, filter_size, kernel_initializer=keras.initializers.Ones(), padding='same')(inputs)
+    return Model(inputs=inputs, outputs=conv_3d)
+
+
+def lcn_gpu(img3d, noise_level=5, filter_size=(27, 27, 1)):
+    """
+    Local contrast normalization by gpu
+
+    Parameters
+    ----------
+    img3d : numpy.ndarray
+        The raw 3D image
+    noise_level : float
+        The parameter to suppress the enhancement of the background noises
+    filter_size : tuple, optional
+        the window size to apply the normalization along x, y, and z axis. Default: (27, 27, 1)
+
+    Returns
+    -------
+    norm : numpy.ndarray
+        The normalized 3D image
+
+    Notes
+    -----
+    The normalization in the edge regions currently used zero padding based on keras.Conv3D function,
+    which is different with the lcn_cpu function (uses "reflect" padding).
+    """
+    img3d_siz = img3d.shape
+    volume = filter_size[0] * filter_size[1] * filter_size[2]
+    conv3d_model = conv3d_keras(filter_size, img3d_siz)
+    img3d = np.expand_dims(img3d, axis=(0,4))
+    avg = conv3d_model.predict(img3d) / volume
+    diff_sqr = np.square(img3d - avg)
+    std = np.sqrt(conv3d_model.predict(diff_sqr) / volume)
+    norm = np.divide(img3d - avg, std + noise_level)
+    return norm[0, :, :, :, 0]
+
+
+def _normalize_image(image, noise_level):
+    """
+    Normalize an 3D image by local contrast normalization
+
+    Parameters
+    ----------
+    image : numpy.ndarray
+        A 3D image to be normalized
+    noise_level : float
+        The parameter to suppress the enhancement of the background noises
+
+    Returns
+    -------
+    numpy.ndarray
+        The normalized image
+    """
+    image_norm = image - np.median(image)
+    image_norm[image_norm < 0] = 0
+    return lcn_gpu(image_norm, noise_level, filter_size=(27, 27, 1))
+
+
+def _normalize_label(label_img):
+    """
+    Transform cell/non-cell image into binary (0/1)
+
+    Parameters
+    ----------
+    label_img : numpy.ndarray
+        Input image of cell/non-cell regions
+
+    Returns
+    -------
+    numpy.ndarray
+        The binarized image
+    """
     return (label_img > 0).astype(int)
```

### Comparing `3DeeCellTracker-0.4.5/CellTracker/track.py` & `3DeeCellTracker-0.5.0a0/CellTracker/track.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,612 +1,610 @@
-"""
-A module including functions for tracking cells
-Author: Chentao Wen
-
-"""
-import matplotlib.pyplot as plt
-import numpy as np
-from skimage.filters import gaussian
-from sklearn.neighbors import NearestNeighbors
-
-
-def pr_gls_quick(X, Y, corr, BETA=300, max_iteration=20, LAMBDA=0.1, vol=1E8):
-    """
-    Get coherent movements from the initial matching by PR-GLS algorithm
-
-    Parameters
-    ----------
-    X : numpy.ndarray
-    Y : numpy.ndarray
-        positions of two point sets
-    corr : numpy.ndarray
-        initial matching
-    BETA : float
-    max_iteration : int
-    LAMBDA : float
-    vol : float
-        parameters of PR-GLS
-
-    Returns
-    -------
-    P : numpy.ndarray
-        updated matching
-    T_X : numpy.ndarray
-        transformed positions of X
-    C : numpy.ndarray
-        coefficients for transforming positions other than X.
-    """
-    ############################################################
-    # initiate Gram matrix, C, sigma_square, init_match, T_X, P
-    ############################################################
-    # set parameters
-    gamma = 0.1
-
-    # Gram matrix quick (represents basis functions for transformation)
-    length_X = np.size(X, axis=0)
-    X_tile = np.tile(X, (length_X, 1, 1))
-    Gram_matrix = np.exp(-np.sum(np.square(X_tile - X_tile.transpose(1, 0, 2)), axis=2) / (2 * BETA * BETA))
-
-    # Vector C includes weights for each basis function
-    C = np.zeros((3, length_X))
-
-    # sigma square (quick): relates to the variance of differences between
-    # corresponding points in T_X and Y.
-    length_Y = np.size(Y, axis=0)
-    X_tile = np.tile(X, (length_Y, 1, 1))
-    Y_tile = np.tile(Y, (length_X, 1, 1)).transpose(1, 0, 2)
-    sigma_square = np.sum(np.sum(np.square(X_tile - Y_tile), axis=2)) / (3 * length_X * length_Y)
-
-    # set initial matching
-    # only the most possible pairs are set with probalility of 0.9
-    init_match = np.ones((length_Y, length_X)) / length_X
-    cc_ref_tgt_temp = np.copy(corr)
-    for ptr_num in range(length_X):
-        cc_max = cc_ref_tgt_temp.max()
-        if cc_max < 0.5:
-            break
-        cc_max_idx = np.unravel_index(cc_ref_tgt_temp.argmax(), cc_ref_tgt_temp.shape)
-        init_match[cc_max_idx[0], :] = 0.1 / (length_X - 1)
-        init_match[cc_max_idx[0], cc_max_idx[1]] = 0.9
-        cc_ref_tgt_temp[cc_max_idx[0], :] = 0;
-        cc_ref_tgt_temp[:, cc_max_idx[1]] = 0;
-
-    # initiate T_X, which equals to X+v(X).
-    T_X = X.copy()
-
-    ############################################################################
-    # iteratively update T_X, gamma, sigma_square, and P. Plot and save results
-    ############################################################################
-    for iteration in range(1, max_iteration):
-
-        # calculate P (quick)
-        T_X_tile = np.tile(T_X, (length_Y, 1, 1))
-        Y_tile = np.tile(Y, (length_X, 1, 1)).transpose(1, 0, 2)
-        dist_square = np.sum(np.square(T_X_tile - Y_tile), axis=2)
-        exp_dist_square = np.exp(-dist_square / (2 * sigma_square))
-        P1 = init_match * exp_dist_square
-        denominator = np.sum(P1, axis=1) + gamma * (2 * np.pi * sigma_square) ** 1.5 / ((1 - gamma) * vol)
-        denominator_tile = np.tile(denominator, (length_X, 1)).transpose()
-        P = P1 / denominator_tile
-
-        # solve the linear equations for vector C
-        diag_P = np.diag(np.reshape(np.dot(np.ones((1, length_Y)), P), (length_X)))
-        a = np.dot(Gram_matrix, diag_P) + LAMBDA * sigma_square * np.identity(length_X)
-        b = np.dot(np.matrix.transpose(Y), P) - np.dot(np.matrix.transpose(X), diag_P)
-
-        a = np.matrix.transpose(a)
-        b = np.matrix.transpose(b)
-        C = np.matrix.transpose(np.linalg.solve(a, b))
-
-        # calculate T_X
-        T_X = np.matrix.transpose(np.matrix.transpose(X) + np.dot(C, Gram_matrix))
-
-        # update gamma and sigma square (quick)
-        M_P = np.sum(P)
-        gamma = 1 - M_P / length_Y
-
-        T_X_tile = np.tile(T_X, (length_Y, 1, 1))
-        dist_square = np.sum(np.square(T_X_tile - Y_tile), axis=2)
-        sigma_square = np.sum(P * dist_square) / (3 * M_P)
-
-        # avoid using too small values of sigma_square (the sample error should be >=1 pixel)
-        if sigma_square < 1:
-            sigma_square = 1
-
-    return P, T_X, C
-
-
-def initial_matching_quick(ffn_model, ref, tgt, k_ptrs):
-    """
-    This function compute initial matching between all pairs of points in reference and target points set.
-
-    Parameters
-    ----------
-    ffn_model : keras.Model
-        The pretrained FFN model
-    ref : numpy.ndarray
-        The positions of the cells in the first volume
-    tgt : numpy.ndarray
-        The positions of the cells in the second volume
-    k_ptrs : int
-        The number of neighboring points used for FFN
-
-    Returns
-    -------
-    corr : numpy.ndarray
-        The correspondence matrix between two point sets
-    """
-    nbors_ref = NearestNeighbors(n_neighbors=k_ptrs + 1).fit(ref)
-    nbors_tgt = NearestNeighbors(n_neighbors=k_ptrs + 1).fit(tgt)
-
-    ref_x_flat_batch = np.zeros((ref.shape[0], k_ptrs * 3 + 1), dtype='float32')
-    tgt_x_flat_batch = np.zeros((tgt.shape[0], k_ptrs * 3 + 1), dtype='float32')
-
-    for ref_i in range(ref.shape[0]):
-        # Generate 20 (k_ptrs) points near the specific point
-        # in the ref points set
-
-        distance_ref, indices_ref = nbors_ref.kneighbors(ref[ref_i:ref_i + 1, :],
-                                                         return_distance=True)
-
-        mean_dist_ref = np.mean(distance_ref)
-        ref_x = (ref[indices_ref[0, 1:k_ptrs + 1], :] - ref[indices_ref[0, 0], :]) / mean_dist_ref
-        ref_x_flat = np.zeros(k_ptrs * 3 + 1)
-        ref_x_flat[0:k_ptrs * 3] = ref_x.reshape(k_ptrs * 3)
-        ref_x_flat[k_ptrs * 3] = mean_dist_ref
-
-        ref_x_flat_batch[ref_i, :] = ref_x_flat.reshape(1, k_ptrs * 3 + 1)
-
-    ref_x_flat_batch_meshgrid = np.tile(ref_x_flat_batch, (tgt.shape[0], 1, 1)).reshape(
-        (ref.shape[0] * tgt.shape[0], k_ptrs * 3 + 1))
-
-    for tgt_i in range(tgt.shape[0]):
-        distance_tgt, indices_tgt = nbors_tgt.kneighbors(tgt[tgt_i:tgt_i + 1, :],
-                                                         return_distance=True)
-        mean_dist_tgt = np.mean(distance_tgt)
-        tgt_x = (tgt[indices_tgt[0, 1:k_ptrs + 1], :] - tgt[indices_tgt[0, 0], :]) / mean_dist_tgt
-        tgt_x_flat = np.zeros(k_ptrs * 3 + 1)
-        tgt_x_flat[0:k_ptrs * 3] = tgt_x.reshape(k_ptrs * 3)
-        tgt_x_flat[k_ptrs * 3] = mean_dist_tgt
-
-        tgt_x_flat_batch[tgt_i, :] = tgt_x_flat.reshape(1, k_ptrs * 3 + 1)
-
-    tgt_x_flat_batch_meshgrid = np.tile(tgt_x_flat_batch, (ref.shape[0], 1, 1)).transpose(1, 0, 2).reshape(
-        (ref.shape[0] * tgt.shape[0], k_ptrs * 3 + 1))
-
-    corr = np.reshape(ffn_model.predict([ref_x_flat_batch_meshgrid, tgt_x_flat_batch_meshgrid], batch_size=1024),
-                      (tgt.shape[0], ref.shape[0]))
-
-    return corr
-
-def pr_gls(X,Y,corr,BETA=300, max_iteration=20, LAMBDA=0.1,vol=1E8):
-    """
-    (Deprecated from v0.3) The old version of pr_gls_quick(). Much slower.
-    """
-    ############################################################
-    # initiate Gram matrix, C, sigma_square, init_match, T_X, P
-    ############################################################
-    
-    # set parameters
-    gamma = 0.1
-    
-    # Gram matrix (represents basis functions for transformation)
-    length_X = np.size(X, axis=0)
-    Gram_matrix = np.zeros((length_X,length_X))
-    for idx_i in range(length_X):
-        for idx_j in range(length_X):
-            Gram_matrix[idx_i,idx_j] = np.exp(-np.sum(np.square(X[idx_i,:]-X[idx_j,:]))/
-                       (2*BETA*BETA)) 
-    
-    # Vector C includes weights for each basis function        
-    C = np.zeros((3,length_X))
-    
-    # sigma square: relates to the variance of differences between 
-    # corresponding points in T_X and Y.
-    length_Y = np.size(Y,axis=0)
-    sigma_square=0
-    for idx_X in range(length_X):
-        for idx_Y in range(length_Y):
-            sigma_square = sigma_square + np.sum(np.square(X[idx_X,:]-Y[idx_Y,:]))
-    sigma_square = sigma_square/(3*length_X*length_Y)
-    
-    # set initial matching
-    # only the most possible pairs are set with probalility of 0.9
-    init_match=np.ones((length_Y,length_X))/length_X
-    cc_ref_tgt_temp=np.copy(corr)
-    for ptr_num in range(length_X):
-        cc_max=cc_ref_tgt_temp.max()
-        if cc_max<0.5:
-            break
-        cc_max_idx=np.unravel_index(cc_ref_tgt_temp.argmax(),cc_ref_tgt_temp.shape)
-        init_match[cc_max_idx[0],:]=0.1/(length_X-1)    
-        init_match[cc_max_idx[0],cc_max_idx[1]]=0.9
-        cc_ref_tgt_temp[cc_max_idx[0],:]=0;
-        cc_ref_tgt_temp[:,cc_max_idx[1]]=0;
-    
-    # initiate T_X, which equals to X+v(X).
-    T_X=X.copy()
-    
-    # initiate P 
-    P=np.zeros((length_Y,length_X))
-    
-    ############################################################################
-    # iteratively update T_X, gamma, sigma_square, and P. Plot and save results
-    ############################################################################
-    
-    # loop start
-    
-    for iteration in range(1,max_iteration):
-        
-        # calculate P
-        for idx_Y in range(length_Y):
-            denominator=0
-            for idx_X in range(length_X):
-                P[idx_Y,idx_X]=init_match[idx_Y,idx_X]*np.exp(
-                        -np.sum(np.square(Y[idx_Y,:]-T_X[idx_X,:]))/(2*sigma_square))
-                denominator=denominator+P[idx_Y,idx_X]
-            denominator=denominator+gamma*(2*np.pi*sigma_square)**1.5/((1-gamma)*vol)
-            P[idx_Y,:]=P[idx_Y,:]/denominator
-            
-        # solve the linear equations for vector C
-        diag_P=np.diag(np.reshape(np.dot(np.ones((1,length_Y)),P),(length_X)))
-        a = np.dot(Gram_matrix,diag_P)+LAMBDA*sigma_square*np.identity(length_X)
-        b=np.dot(np.matrix.transpose(Y),P)-np.dot(np.matrix.transpose(X),diag_P)
-        
-        a = np.matrix.transpose(a)
-        b = np.matrix.transpose(b)
-        C = np.matrix.transpose(np.linalg.solve(a, b))
-        
-        # calculate T_X
-        T_X=np.matrix.transpose(np.matrix.transpose(X)+np.dot(C,Gram_matrix))
-        
-        # update gamma and sigma square
-        M_P=np.sum(P)
-        gamma=1-M_P/length_Y
-        
-        sigma_square=0
-        for idx_X in range(length_X):
-            for idx_Y in range(length_Y):
-                sigma_square=sigma_square+P[idx_Y,idx_X]*np.sum(
-                        np.square(Y[idx_Y,:]-T_X[idx_X,:]))
-        sigma_square = sigma_square/(3*M_P)
-        
-        # avoid using too small values of sigma_square (the sample error should be
-                                                        # >=1 pixel)
-        if sigma_square<1:
-            sigma_square=1
-            
-    # loop end
-    
-    return [P, T_X, C]
-
-def initial_matching(fnn_model,ref,tgt,k_ptrs):
-    """
-    (Deprecated from v0.3) The old version of initial_matching_quick(). Much slower.
-    """
-    nbors_ref=NearestNeighbors(n_neighbors=k_ptrs+1).fit(ref)
-    nbors_tgt=NearestNeighbors(n_neighbors=k_ptrs+1).fit(tgt)
-    
-    corr=np.zeros((tgt.shape[0],ref.shape[0]),dtype='float32')
-    
-    for ref_i in range(ref.shape[0]):       
-        
-        ref_x_flat_batch=np.zeros((tgt.shape[0],k_ptrs*3+1),dtype='float32')
-        tgt_x_flat_batch=np.zeros((tgt.shape[0],k_ptrs*3+1),dtype='float32') 
-        
-        # Generate 20 (k_ptrs) points near the specific point 
-        # in the ref points set
-        distance_ref,indices_ref=nbors_ref.kneighbors(ref[ref_i:ref_i+1,:],
-                                 return_distance=True)
-        mean_dist_ref=np.mean(distance_ref)                                  
-        ref_x=(ref[indices_ref[0,1:k_ptrs+1],:]-ref[indices_ref[0,0],:])/mean_dist_ref
-        ref_x_flat=np.zeros(k_ptrs*3+1)
-        ref_x_flat[0:k_ptrs*3]=ref_x.reshape(k_ptrs*3)
-        ref_x_flat[k_ptrs*3]=mean_dist_ref   
-           
-        for tgt_i in range(tgt.shape[0]):     
-            distance_tgt,indices_tgt=nbors_tgt.kneighbors(tgt[tgt_i:tgt_i+1,:],
-                                     return_distance=True)
-            mean_dist_tgt=np.mean(distance_tgt)                                  
-            tgt_x=(tgt[indices_tgt[0,1:k_ptrs+1],:]-tgt[indices_tgt[0,0],:])/mean_dist_tgt
-            tgt_x_flat=np.zeros(k_ptrs*3+1)
-            tgt_x_flat[0:k_ptrs*3]=tgt_x.reshape(k_ptrs*3)
-            tgt_x_flat[k_ptrs*3]=mean_dist_tgt
-            
-            ref_x_flat_batch[tgt_i,:]=ref_x_flat.reshape(1,k_ptrs*3+1)
-            tgt_x_flat_batch[tgt_i,:]=tgt_x_flat.reshape(1,k_ptrs*3+1)
-        
-        corr[:,ref_i]=np.reshape(fnn_model.predict([ref_x_flat_batch, tgt_x_flat_batch],batch_size=32),tgt.shape[0])     
-                   
-    return corr
-
-
-def transform_cells(img3d, vectors3d):
-    """
-    Move individual cells in the label image.
-
-    Parameters
-    ----------
-    img3d : numpy.ndarray
-        Label image, each cell with different labels.
-    vectors3d : numpy.ndarray
-        The movement vectors for each cell, of dtype 'int' (movement from input img to output img)
-
-    Returns
-    -------
-    output : numpy.ndarray
-        Transformed label image
-    mask : numpy.ndarray
-        Overlap between different labels (if value>1)
-    """
-    shape = np.shape(img3d)
-    output = np.zeros((shape),dtype=np.dtype(img3d[0,0,0]))
-    mask = np.zeros((shape),dtype=np.dtype(img3d[0,0,0]))
-    for label in range(1, img3d.max()+1):
-
-        v1 = vectors3d[label-1,0]; v2 = vectors3d[label-1,1]; v3 = vectors3d[label-1,2]; 
-        
-        if v1>=0:
-            idx_1_start=0;idx_1_end=shape[0]-v1
-        else:
-            idx_1_start=-v1;idx_1_end=shape[0]
-        if v2>=0:
-            idx_2_start=0;idx_2_end=shape[1]-v2
-        else:
-            idx_2_start=-v2;idx_2_end=shape[1]
-        if v3>=0:
-            idx_3_start=0;idx_3_end=shape[2]-v3
-        else:
-            idx_3_start=-v3;idx_3_end=shape[2]
-        
-        image_temp = img3d[idx_1_start:idx_1_end, idx_2_start:idx_2_end, idx_3_start:idx_3_end]
-        idx_label = np.where(image_temp==label)
-        output[idx_label[0]+idx_1_start+v1,idx_label[1]+idx_2_start+v2,idx_label[2]+idx_3_start+v3] = image_temp[idx_label]
-        mask[idx_label[0]+idx_1_start+v1,idx_label[1]+idx_2_start+v2,
-             idx_label[2]+idx_3_start+v3] = mask[idx_label[0]+idx_1_start+v1,
-                      idx_label[1]+idx_2_start+v2,idx_label[2]+idx_3_start+v3]+1
-    
-    return output, mask
-
-
-def plot_arrow(ax, x1, y1, x2, y2):
-    """Draw the arrows from (x1, y1) to (x2,y2)"""
-    return ax.annotate("",
-                xy=(x2, y2), xycoords='axes fraction',
-                xytext=(x1, y1), textcoords='axes fraction',
-                arrowprops=dict(arrowstyle="wedge",  color="C0"))
-
-def plot_tracking_2d(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis, sizes):
-    """Draw the tracking process between two point sets with layer-based coordinates"""
-    element = []
-    ax.invert_yaxis()
-    if draw_point:
-        element.append(ax.scatter(ref_ptrs[:, x_axis], ref_ptrs[:, y_axis], facecolors='none', edgecolors='r'))
-        element.append(ax.plot(tgt_ptrs[:, x_axis], tgt_ptrs[:, y_axis], 'bx')[0])
-    length_X = np.size(ref_ptrs, axis=0)
-    for ptr_num in range(length_X):
-        element.append(plot_arrow(ax,
-            x1=ref_ptrs[ptr_num, x_axis]/sizes[0], y1=1-ref_ptrs[ptr_num, y_axis]/sizes[1],
-            x2=T_ref[ptr_num, x_axis]/sizes[0], y2=1-T_ref[ptr_num, y_axis]/sizes[1]))
-    ax.axis('equal')
-    return element
-
-def plot_tracking_2d_realcoord(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis):
-    """Draw the tracking process between two point sets with real-resolution coordinates"""
-    ax.invert_yaxis()
-    element = []
-    if draw_point:
-        element.append(ax.scatter(ref_ptrs[:, x_axis], ref_ptrs[:, y_axis], facecolors='none', edgecolors='r'))
-        element.append(ax.plot(tgt_ptrs[:, x_axis], tgt_ptrs[:, y_axis], 'bx')[0])
-    length_X = np.size(ref_ptrs, axis=0)
-    for ptr_num in range(length_X):
-        element.append(ax.arrow(
-            x=ref_ptrs[ptr_num, x_axis], y=ref_ptrs[ptr_num, y_axis],
-            dx=T_ref[ptr_num, x_axis] - ref_ptrs[ptr_num, x_axis],
-            dy=T_ref[ptr_num, y_axis] - ref_ptrs[ptr_num, y_axis], color="C0", length_includes_head=True,
-            head_length=4, head_width=3))
-    ax.axis('equal')
-    return element
-
-
-def tracking_plot_xy(ax, ref_ptrs, tgt_ptrs, T_ref, yx_sizes, draw_point=True, layercoord=False):
-    """Draw the tracking process between two point sets in x-y plane"""
-    x_axis=1
-    y_axis=0
-    if layercoord:
-        element = plot_tracking_2d(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis, yx_sizes)
-    else:
-        element = plot_tracking_2d_realcoord(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis)
-    return element
-
-
-def tracking_plot_zx(ax, ref_ptrs, tgt_ptrs, T_ref, yz_sizes, draw_point=True, layercoord=True):
-    """Draw the tracking process between two point sets in z-x plane"""
-    x_axis=1
-    y_axis=2
-    if layercoord:
-        element = plot_tracking_2d(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis, yz_sizes)
-    else:
-        element = plot_tracking_2d_realcoord(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis)
-    return element
-
-
-def FFN_matching_plot(ref_ptrs, tgt_ptrs, initial_match_score):
-    """(Deprecated from v0.3) Draw the FFN_matching process"""
-    length_ref_ptrs = np.size(ref_ptrs, axis=0)
-    
-    tgt_ptrs_y_bias = tgt_ptrs.copy()
-    bias = (np.max(tgt_ptrs[:,0])-np.min(tgt_ptrs[:,0]))*2
-    tgt_ptrs_y_bias[:,0] = tgt_ptrs_y_bias[:,0]+bias
-    plt.ion()
-    fig = plt.figure(figsize=(9,9))
-    plt.scatter(ref_ptrs[:,1],-ref_ptrs[:,0],facecolors='none',edgecolors='r')
-    plt.plot(tgt_ptrs_y_bias[:,1],-tgt_ptrs_y_bias[:,0],'x')
-    plt.axis('equal')
-
-    cc_ref_tgt_temp=np.copy(initial_match_score)
-    for ptr_num in range(length_ref_ptrs):
-        cc_max=cc_ref_tgt_temp.max()
-        if cc_max<0.5:
-            break
-        cc_max_idx=np.unravel_index(cc_ref_tgt_temp.argmax(),cc_ref_tgt_temp.shape)
-    
-        plt.plot([ref_ptrs[cc_max_idx[1],1],tgt_ptrs_y_bias[cc_max_idx[0],1]],
-             [-ref_ptrs[cc_max_idx[1],0],-tgt_ptrs_y_bias[cc_max_idx[0],0]],'r-')
-        cc_ref_tgt_temp[cc_max_idx[0],:]=0
-        cc_ref_tgt_temp[:,cc_max_idx[1]]=0  
-    return fig
-
-
-def get_subregions(label_image, num):
-    """
-    Get individual regions of segmented cells
-
-    Parameters
-    ----------
-    label_image : numpy.ndarray
-        Image of segmented cells
-    num : int
-        Number of cells
-
-    Returns
-    -------
-    region_list : list
-        Cropped images of each cell
-    region_width : list
-        Width of each cell in x,y,and z axis
-    region_coord_min : list
-        Minimum coordinates of each element in region list
-    """
-    region_list = []
-    region_width = []
-    region_coord_min = []
-    for label in range(1, num + 1):
-        if label < num:
-            print(f"Calculating subregions... cell: {label}", end="\r")
-        else:
-            print(f"Calculating subregions... cell: {label}")
-        x_max, x_min, y_max, y_min, z_max, z_min = _get_coordinates(label, label_image, get_subregion=False)
-        region_list.append(label_image[x_min:x_max + 1, y_min:y_max + 1, z_min:z_max + 1] == label)
-        region_width.append([x_max + 1 - x_min, y_max + 1 - y_min, z_max + 1 - z_min])
-        region_coord_min.append([x_min, y_min, z_min])
-    return region_list, region_width, region_coord_min
-
-
-def gaussian_filter(img, z_scaling=10, smooth_sigma=5):
-    """
-    Generate smoothed label image of cells
-
-    Parameters
-    ----------
-    img : numpy.ndarray
-        Label image
-    z_scaling : int
-        Factor of interpolations along z axis, should be <10
-    smooth_sigma : float
-        sigma used for making Gaussian blur
-
-    Returns
-    -------
-    output_img : numpy.ndarray
-        Generated smoothed label image
-    mask : numpy.ndarray
-        Mask image indicating the overlapping of multiple cells (0: background; 1: one cell; >1: multiple cells)
-    """
-    img_interp = np.repeat(img, z_scaling, axis=2)
-    shape_interp = img_interp.shape
-    output_img = np.zeros((shape_interp[0] + 10, shape_interp[1] + 10, shape_interp[2] + 10), dtype='int')
-    mask = output_img.copy()
-
-    for label in range(1, np.max(img) + 1):
-        print(f"Interpolating... cell:{label}", end="\r")
-        x_max, x_min, y_max, y_min, z_max, z_min, subregion_pad, voxels = _get_coordinates(label, img_interp)
-
-        percentage = 1 - np.divide(voxels, np.size(subregion_pad), dtype='float')
-
-        img_smooth = gaussian(subregion_pad, sigma=smooth_sigma, mode='constant')
-
-        threshold = np.percentile(img_smooth, percentage * 100)
-
-        cell_region_interp = img_smooth > threshold
-
-        output_img[x_min:x_max + 11, y_min:y_max + 11, z_min:z_max + 11] += cell_region_interp * label
-        mask[x_min:x_max + 11, y_min:y_max + 11, z_min:z_max + 11] += cell_region_interp * 1
-
-    return output_img, mask
-
-
-def _get_coordinates(label, label_image, get_subregion=True):
-    """
-    Get the coordinates of a specific label
-
-    Parameters
-    ----------
-    label : int
-        The number of the cell label
-    label_image :
-        The label image
-    get_subregion : bool
-        If True, return the image of the subregion and its size
-
-    Returns
-    -------
-    x_max : float
-    x_min : float
-    y_max : float
-    y_min : float
-    z_max : float
-    z_min : float
-        Coordinates for the subregion
-    subregion : numpy.ndarray
-        The subregion containing the label
-    np.size(region[0]) : int
-        The size of the subregion
-    """
-    region = np.where(label_image == label)
-    x_max, x_min = np.max(region[0]), np.min(region[0])
-    y_max, y_min = np.max(region[1]), np.min(region[1])
-    z_max, z_min = np.max(region[2]), np.min(region[2])
-    if not get_subregion:
-        return x_max, x_min, y_max, y_min, z_max, z_min
-    else:
-        subregion = np.zeros((x_max-x_min+11,y_max-y_min+11,z_max-z_min+11))
-        subregion[region[0] - x_min + 5, region[1] - y_min + 5, region[2] - z_min + 5] = 0.5
-        return x_max, x_min, y_max, y_min, z_max, z_min, subregion, np.size(region[0])
-
-
-def get_reference_vols(ensemble, vol, adjacent=False):
-    """
-    Get the reference volumes to calculate multiple prediction from which
-
-    Parameters
-    ----------
-    ensemble : int
-        The maximum number of predictions
-    vol : int
-        The current volume number at which the prediction was made
-    adjacent : bool
-        If True, get reference volumes from adjacent previous volumes. If False, from distributed previous volumes
-
-    Returns
-    -------
-    vols_list : list
-        The list of the reference volume numbers
-    """
-    if not ensemble:
-        return [vol - 1]
-    if vol - 1 < ensemble:
-        vols_list = list(range(1, vol))
-    else:
-        if adjacent:
-            vols_list = list(range(vol - ensemble, vol))
-        else:
-            vols_list = get_remote_vols(ensemble, vol)
-    return vols_list
-
-
-def get_remote_vols(ensemble, vol):
-    """Get distributed previous volumes"""
-    interval = (vol - 1) // ensemble
-    start = np.mod(vol - 1, ensemble) + 1
-    vols_list = list(range(start, vol - interval+1, interval))
-    return vols_list
+"""
+A module including functions for tracking cells
+Author: Chentao Wen
+
+"""
+import matplotlib.pyplot as plt
+import numpy as np
+from sklearn.neighbors import NearestNeighbors
+
+
+def pr_gls_quick(X, Y, corr, BETA=300, max_iteration=20, LAMBDA=0.1, vol=1E8):
+    """
+    Get coherent movements from the initial matching by PR-GLS algorithm
+
+    Parameters
+    ----------
+    X : numpy.ndarray
+    Y : numpy.ndarray
+        positions of two point sets
+    corr : numpy.ndarray
+        initial matching
+    BETA : float
+    max_iteration : int
+    LAMBDA : float
+    vol : float
+        parameters of PR-GLS
+
+    Returns
+    -------
+    P : numpy.ndarray
+        updated matching
+    T_X : numpy.ndarray
+        transformed positions of X
+    C : numpy.ndarray
+        coefficients for transforming positions other than X.
+    """
+    ############################################################
+    # initiate Gram matrix, C, sigma_square, init_match, T_X, P
+    ############################################################
+    # set parameters
+    gamma = 0.1
+
+    # Gram matrix quick (represents basis functions for transformation)
+    length_X = np.size(X, axis=0)
+    X_tile = np.tile(X, (length_X, 1, 1))
+    Gram_matrix = np.exp(-np.sum(np.square(X_tile - X_tile.transpose(1, 0, 2)), axis=2) / (2 * BETA * BETA))
+
+    # Vector C includes weights for each basis function
+    C = np.zeros((3, length_X))
+
+    # sigma square (quick): relates to the variance of differences between
+    # corresponding points in T_X and Y.
+    length_Y = np.size(Y, axis=0)
+    X_tile = np.tile(X, (length_Y, 1, 1))
+    Y_tile = np.tile(Y, (length_X, 1, 1)).transpose(1, 0, 2)
+    sigma_square = np.sum(np.sum(np.square(X_tile - Y_tile), axis=2)) / (3 * length_X * length_Y)
+
+    # set initial matching
+    # only the most possible pairs are set with probalility of 0.9
+    init_match = np.ones((length_Y, length_X)) / length_X
+    cc_ref_tgt_temp = np.copy(corr)
+    for ptr_num in range(length_X):
+        cc_max = cc_ref_tgt_temp.max()
+        if cc_max < 0.5:
+            break
+        cc_max_idx = np.unravel_index(cc_ref_tgt_temp.argmax(), cc_ref_tgt_temp.shape)
+        init_match[cc_max_idx[0], :] = 0.1 / (length_X - 1)
+        init_match[cc_max_idx[0], cc_max_idx[1]] = 0.9
+        cc_ref_tgt_temp[cc_max_idx[0], :] = 0;
+        cc_ref_tgt_temp[:, cc_max_idx[1]] = 0;
+
+    # initiate T_X, which equals to X+v(X).
+    T_X = X.copy()
+
+    ############################################################################
+    # iteratively update T_X, gamma, sigma_square, and P. Plot and save results
+    ############################################################################
+    for iteration in range(1, max_iteration):
+
+        # calculate P (quick)
+        T_X_tile = np.tile(T_X, (length_Y, 1, 1))
+        Y_tile = np.tile(Y, (length_X, 1, 1)).transpose(1, 0, 2)
+        dist_square = np.sum(np.square(T_X_tile - Y_tile), axis=2)
+        exp_dist_square = np.exp(-dist_square / (2 * sigma_square))
+        P1 = init_match * exp_dist_square
+        denominator = np.sum(P1, axis=1) + gamma * (2 * np.pi * sigma_square) ** 1.5 / ((1 - gamma) * vol)
+        denominator_tile = np.tile(denominator, (length_X, 1)).transpose()
+        P = P1 / denominator_tile
+
+        # solve the linear equations for vector C
+        diag_P = np.diag(np.reshape(np.dot(np.ones((1, length_Y)), P), (length_X)))
+        a = np.dot(Gram_matrix, diag_P) + LAMBDA * sigma_square * np.identity(length_X)
+        b = np.dot(np.matrix.transpose(Y), P) - np.dot(np.matrix.transpose(X), diag_P)
+
+        a = np.matrix.transpose(a)
+        b = np.matrix.transpose(b)
+        C = np.matrix.transpose(np.linalg.solve(a, b))
+
+        # calculate T_X
+        T_X = np.matrix.transpose(np.matrix.transpose(X) + np.dot(C, Gram_matrix))
+
+        # update gamma and sigma square (quick)
+        M_P = np.sum(P)
+        gamma = 1 - M_P / length_Y
+
+        T_X_tile = np.tile(T_X, (length_Y, 1, 1))
+        dist_square = np.sum(np.square(T_X_tile - Y_tile), axis=2)
+        sigma_square = np.sum(P * dist_square) / (3 * M_P)
+
+        # avoid using too small values of sigma_square (the sample error should be >=1 pixel)
+        if sigma_square < 1:
+            sigma_square = 1
+
+    return P, T_X, C
+
+
+def initial_matching_quick(ffn_model, ref, tgt, k_ptrs):
+    """
+    This function compute initial matching between all pairs of points in reference and target points set.
+
+    Parameters
+    ----------
+    ffn_model : keras.Model
+        The pretrained FFN model
+    ref : numpy.ndarray
+        The positions of the cells in the first volume
+    tgt : numpy.ndarray
+        The positions of the cells in the second volume
+    k_ptrs : int
+        The number of neighboring points used for FFN
+
+    Returns
+    -------
+    corr : numpy.ndarray
+        The correspondence matrix between two point sets
+    """
+    nbors_ref = NearestNeighbors(n_neighbors=k_ptrs + 1).fit(ref)
+    nbors_tgt = NearestNeighbors(n_neighbors=k_ptrs + 1).fit(tgt)
+
+    ref_x_flat_batch = np.zeros((ref.shape[0], k_ptrs * 3 + 1), dtype='float32')
+    tgt_x_flat_batch = np.zeros((tgt.shape[0], k_ptrs * 3 + 1), dtype='float32')
+
+    for ref_i in range(ref.shape[0]):
+        # Generate 20 (k_ptrs) points near the specific point
+        # in the ref points set
+
+        distance_ref, indices_ref = nbors_ref.kneighbors(ref[ref_i:ref_i + 1, :],
+                                                         return_distance=True)
+
+        mean_dist_ref = np.mean(distance_ref)
+        ref_x = (ref[indices_ref[0, 1:k_ptrs + 1], :] - ref[indices_ref[0, 0], :]) / mean_dist_ref
+        ref_x_flat = np.zeros(k_ptrs * 3 + 1)
+        ref_x_flat[0:k_ptrs * 3] = ref_x.reshape(k_ptrs * 3)
+        ref_x_flat[k_ptrs * 3] = mean_dist_ref
+
+        ref_x_flat_batch[ref_i, :] = ref_x_flat.reshape(1, k_ptrs * 3 + 1)
+
+    ref_x_flat_batch_meshgrid = np.tile(ref_x_flat_batch, (tgt.shape[0], 1, 1)).reshape(
+        (ref.shape[0] * tgt.shape[0], k_ptrs * 3 + 1))
+
+    for tgt_i in range(tgt.shape[0]):
+        distance_tgt, indices_tgt = nbors_tgt.kneighbors(tgt[tgt_i:tgt_i + 1, :],
+                                                         return_distance=True)
+        mean_dist_tgt = np.mean(distance_tgt)
+        tgt_x = (tgt[indices_tgt[0, 1:k_ptrs + 1], :] - tgt[indices_tgt[0, 0], :]) / mean_dist_tgt
+        tgt_x_flat = np.zeros(k_ptrs * 3 + 1)
+        tgt_x_flat[0:k_ptrs * 3] = tgt_x.reshape(k_ptrs * 3)
+        tgt_x_flat[k_ptrs * 3] = mean_dist_tgt
+
+        tgt_x_flat_batch[tgt_i, :] = tgt_x_flat.reshape(1, k_ptrs * 3 + 1)
+
+    tgt_x_flat_batch_meshgrid = np.tile(tgt_x_flat_batch, (ref.shape[0], 1, 1)).transpose(1, 0, 2).reshape(
+        (ref.shape[0] * tgt.shape[0], k_ptrs * 3 + 1))
+
+    corr = np.reshape(ffn_model.predict([ref_x_flat_batch_meshgrid, tgt_x_flat_batch_meshgrid], batch_size=1024),
+                      (tgt.shape[0], ref.shape[0]))
+
+    return corr
+
+def pr_gls(X,Y,corr,BETA=300, max_iteration=20, LAMBDA=0.1,vol=1E8):
+    """
+    (Deprecated from v0.3) The old version of pr_gls_quick(). Much slower.
+    """
+    ############################################################
+    # initiate Gram matrix, C, sigma_square, init_match, T_X, P
+    ############################################################
+    
+    # set parameters
+    gamma = 0.1
+    
+    # Gram matrix (represents basis functions for transformation)
+    length_X = np.size(X, axis=0)
+    Gram_matrix = np.zeros((length_X,length_X))
+    for idx_i in range(length_X):
+        for idx_j in range(length_X):
+            Gram_matrix[idx_i,idx_j] = np.exp(-np.sum(np.square(X[idx_i,:]-X[idx_j,:]))/
+                       (2*BETA*BETA)) 
+    
+    # Vector C includes weights for each basis function        
+    C = np.zeros((3,length_X))
+    
+    # sigma square: relates to the variance of differences between 
+    # corresponding points in T_X and Y.
+    length_Y = np.size(Y,axis=0)
+    sigma_square=0
+    for idx_X in range(length_X):
+        for idx_Y in range(length_Y):
+            sigma_square = sigma_square + np.sum(np.square(X[idx_X,:]-Y[idx_Y,:]))
+    sigma_square = sigma_square/(3*length_X*length_Y)
+    
+    # set initial matching
+    # only the most possible pairs are set with probalility of 0.9
+    init_match=np.ones((length_Y,length_X))/length_X
+    cc_ref_tgt_temp=np.copy(corr)
+    for ptr_num in range(length_X):
+        cc_max=cc_ref_tgt_temp.max()
+        if cc_max<0.5:
+            break
+        cc_max_idx=np.unravel_index(cc_ref_tgt_temp.argmax(),cc_ref_tgt_temp.shape)
+        init_match[cc_max_idx[0],:]=0.1/(length_X-1)    
+        init_match[cc_max_idx[0],cc_max_idx[1]]=0.9
+        cc_ref_tgt_temp[cc_max_idx[0],:]=0;
+        cc_ref_tgt_temp[:,cc_max_idx[1]]=0;
+    
+    # initiate T_X, which equals to X+v(X).
+    T_X=X.copy()
+    
+    # initiate P 
+    P=np.zeros((length_Y,length_X))
+    
+    ############################################################################
+    # iteratively update T_X, gamma, sigma_square, and P. Plot and save results
+    ############################################################################
+    
+    # loop start
+    
+    for iteration in range(1,max_iteration):
+        
+        # calculate P
+        for idx_Y in range(length_Y):
+            denominator=0
+            for idx_X in range(length_X):
+                P[idx_Y,idx_X]=init_match[idx_Y,idx_X]*np.exp(
+                        -np.sum(np.square(Y[idx_Y,:]-T_X[idx_X,:]))/(2*sigma_square))
+                denominator=denominator+P[idx_Y,idx_X]
+            denominator=denominator+gamma*(2*np.pi*sigma_square)**1.5/((1-gamma)*vol)
+            P[idx_Y,:]=P[idx_Y,:]/denominator
+            
+        # solve the linear equations for vector C
+        diag_P=np.diag(np.reshape(np.dot(np.ones((1,length_Y)),P),(length_X)))
+        a = np.dot(Gram_matrix,diag_P)+LAMBDA*sigma_square*np.identity(length_X)
+        b=np.dot(np.matrix.transpose(Y),P)-np.dot(np.matrix.transpose(X),diag_P)
+        
+        a = np.matrix.transpose(a)
+        b = np.matrix.transpose(b)
+        C = np.matrix.transpose(np.linalg.solve(a, b))
+        
+        # calculate T_X
+        T_X=np.matrix.transpose(np.matrix.transpose(X)+np.dot(C,Gram_matrix))
+        
+        # update gamma and sigma square
+        M_P=np.sum(P)
+        gamma=1-M_P/length_Y
+        
+        sigma_square=0
+        for idx_X in range(length_X):
+            for idx_Y in range(length_Y):
+                sigma_square=sigma_square+P[idx_Y,idx_X]*np.sum(
+                        np.square(Y[idx_Y,:]-T_X[idx_X,:]))
+        sigma_square = sigma_square/(3*M_P)
+        
+        # avoid using too small values of sigma_square (the sample error should be
+                                                        # >=1 pixel)
+        if sigma_square<1:
+            sigma_square=1
+            
+    # loop end
+    
+    return [P, T_X, C]
+
+def initial_matching(fnn_model,ref,tgt,k_ptrs):
+    """
+    (Deprecated from v0.3) The old version of initial_matching_quick(). Much slower.
+    """
+    nbors_ref=NearestNeighbors(n_neighbors=k_ptrs+1).fit(ref)
+    nbors_tgt=NearestNeighbors(n_neighbors=k_ptrs+1).fit(tgt)
+    
+    corr=np.zeros((tgt.shape[0],ref.shape[0]),dtype='float32')
+    
+    for ref_i in range(ref.shape[0]):       
+        
+        ref_x_flat_batch=np.zeros((tgt.shape[0],k_ptrs*3+1),dtype='float32')
+        tgt_x_flat_batch=np.zeros((tgt.shape[0],k_ptrs*3+1),dtype='float32') 
+        
+        # Generate 20 (k_ptrs) points near the specific point 
+        # in the ref points set
+        distance_ref,indices_ref=nbors_ref.kneighbors(ref[ref_i:ref_i+1,:],
+                                 return_distance=True)
+        mean_dist_ref=np.mean(distance_ref)                                  
+        ref_x=(ref[indices_ref[0,1:k_ptrs+1],:]-ref[indices_ref[0,0],:])/mean_dist_ref
+        ref_x_flat=np.zeros(k_ptrs*3+1)
+        ref_x_flat[0:k_ptrs*3]=ref_x.reshape(k_ptrs*3)
+        ref_x_flat[k_ptrs*3]=mean_dist_ref   
+           
+        for tgt_i in range(tgt.shape[0]):     
+            distance_tgt,indices_tgt=nbors_tgt.kneighbors(tgt[tgt_i:tgt_i+1,:],
+                                     return_distance=True)
+            mean_dist_tgt=np.mean(distance_tgt)                                  
+            tgt_x=(tgt[indices_tgt[0,1:k_ptrs+1],:]-tgt[indices_tgt[0,0],:])/mean_dist_tgt
+            tgt_x_flat=np.zeros(k_ptrs*3+1)
+            tgt_x_flat[0:k_ptrs*3]=tgt_x.reshape(k_ptrs*3)
+            tgt_x_flat[k_ptrs*3]=mean_dist_tgt
+            
+            ref_x_flat_batch[tgt_i,:]=ref_x_flat.reshape(1,k_ptrs*3+1)
+            tgt_x_flat_batch[tgt_i,:]=tgt_x_flat.reshape(1,k_ptrs*3+1)
+        
+        corr[:,ref_i]=np.reshape(fnn_model.predict([ref_x_flat_batch, tgt_x_flat_batch],batch_size=32),tgt.shape[0])     
+                   
+    return corr
+
+
+def gaussian_filter(img, z_scaling=10, smooth_sigma=5):
+    """
+    Generate smoothed label image of cells
+    Parameters
+    ----------
+    img : numpy.ndarray
+        Label image
+    z_scaling : int
+        Factor of interpolations along z axis, should be <10
+    smooth_sigma : float
+        sigma used for making Gaussian blur
+    Returns
+    -------
+    output_img : numpy.ndarray
+        Generated smoothed label image
+    mask : numpy.ndarray
+        Mask image indicating the overlapping of multiple cells (0: background; 1: one cell; >1: multiple cells)
+    """
+    img_interp = np.repeat(img, z_scaling, axis=2)
+    shape_interp = img_interp.shape
+    output_img = np.zeros((shape_interp[0] + 10, shape_interp[1] + 10, shape_interp[2] + 10), dtype='int')
+    mask = output_img.copy()
+
+    for label in range(1, np.max(img) + 1):
+        from skimage.filters import gaussian
+        print(f"Interpolating... cell:{label}", end="\r")
+        x_max, x_min, y_max, y_min, z_max, z_min, subregion_pad, voxels = _get_coordinates(label, img_interp)
+
+        percentage = 1 - np.divide(voxels, np.size(subregion_pad), dtype='float')
+
+        img_smooth = gaussian(subregion_pad, sigma=smooth_sigma, mode='constant')
+
+        threshold = np.percentile(img_smooth, percentage * 100)
+
+        cell_region_interp = img_smooth > threshold
+
+        output_img[x_min:x_max + 11, y_min:y_max + 11, z_min:z_max + 11] += cell_region_interp * label
+        mask[x_min:x_max + 11, y_min:y_max + 11, z_min:z_max + 11] += cell_region_interp * 1
+
+    return output_img, mask
+
+
+def transform_cells(img3d, vectors3d):
+    """
+    Move individual cells in the label image.
+
+    Parameters
+    ----------
+    img3d : numpy.ndarray
+        Label image, each cell with different labels.
+    vectors3d : numpy.ndarray
+        The movement vectors for each cell, of dtype 'int' (movement from input img to output img)
+
+    Returns
+    -------
+    output : numpy.ndarray
+        Transformed label image
+    mask : numpy.ndarray
+        Overlap between different labels (if value>1)
+    """
+    shape = np.shape(img3d)
+    output = np.zeros((shape),dtype=np.dtype(img3d[0,0,0]))
+    mask = np.zeros((shape),dtype=np.dtype(img3d[0,0,0]))
+    for label in range(1, img3d.max()+1):
+
+        v1 = vectors3d[label-1,0]; v2 = vectors3d[label-1,1]; v3 = vectors3d[label-1,2]; 
+        
+        if v1>=0:
+            idx_1_start=0;idx_1_end=shape[0]-v1
+        else:
+            idx_1_start=-v1;idx_1_end=shape[0]
+        if v2>=0:
+            idx_2_start=0;idx_2_end=shape[1]-v2
+        else:
+            idx_2_start=-v2;idx_2_end=shape[1]
+        if v3>=0:
+            idx_3_start=0;idx_3_end=shape[2]-v3
+        else:
+            idx_3_start=-v3;idx_3_end=shape[2]
+        
+        image_temp = img3d[idx_1_start:idx_1_end, idx_2_start:idx_2_end, idx_3_start:idx_3_end]
+        idx_label = np.where(image_temp==label)
+        output[idx_label[0]+idx_1_start+v1,idx_label[1]+idx_2_start+v2,idx_label[2]+idx_3_start+v3] = image_temp[idx_label]
+        mask[idx_label[0]+idx_1_start+v1,idx_label[1]+idx_2_start+v2,
+             idx_label[2]+idx_3_start+v3] = mask[idx_label[0]+idx_1_start+v1,
+                      idx_label[1]+idx_2_start+v2,idx_label[2]+idx_3_start+v3]+1
+    
+    return output, mask
+
+
+def plot_arrow(ax, x1, y1, x2, y2):
+    """Draw the arrows from (x1, y1) to (x2,y2)"""
+    return ax.annotate("",
+                xy=(x2, y2), xycoords='axes fraction',
+                xytext=(x1, y1), textcoords='axes fraction',
+                arrowprops=dict(arrowstyle="wedge",  color="C0"))
+
+def plot_tracking_2d(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis, sizes):
+    """Draw the tracking process between two point sets with layer-based coordinates"""
+    element = []
+    ax.invert_yaxis()
+    if draw_point:
+        element.append(ax.scatter(ref_ptrs[:, x_axis], ref_ptrs[:, y_axis], facecolors='none', edgecolors='r'))
+        element.append(ax.plot(tgt_ptrs[:, x_axis], tgt_ptrs[:, y_axis], 'bx')[0])
+    length_X = np.size(ref_ptrs, axis=0)
+    for ptr_num in range(length_X):
+        element.append(plot_arrow(ax,
+            x1=ref_ptrs[ptr_num, x_axis]/sizes[0], y1=1-ref_ptrs[ptr_num, y_axis]/sizes[1],
+            x2=T_ref[ptr_num, x_axis]/sizes[0], y2=1-T_ref[ptr_num, y_axis]/sizes[1]))
+    ax.axis('equal')
+    return element
+
+def plot_tracking_2d_realcoord(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis):
+    """Draw the tracking process between two point sets with real-resolution coordinates"""
+    ax.invert_yaxis()
+    element = []
+    if draw_point:
+        element.append(ax.scatter(ref_ptrs[:, x_axis], ref_ptrs[:, y_axis], facecolors='none', edgecolors='r'))
+        element.append(ax.plot(tgt_ptrs[:, x_axis], tgt_ptrs[:, y_axis], 'bx')[0])
+    length_X = np.size(ref_ptrs, axis=0)
+    for ptr_num in range(length_X):
+        element.append(ax.arrow(
+            x=ref_ptrs[ptr_num, x_axis], y=ref_ptrs[ptr_num, y_axis],
+            dx=T_ref[ptr_num, x_axis] - ref_ptrs[ptr_num, x_axis],
+            dy=T_ref[ptr_num, y_axis] - ref_ptrs[ptr_num, y_axis], color="C0", length_includes_head=True,
+            head_length=4, head_width=3))
+    ax.axis('equal')
+    return element
+
+
+def tracking_plot_xy(ax, ref_ptrs, tgt_ptrs, T_ref, yx_sizes, draw_point=True, layercoord=False):
+    """Draw the tracking process between two point sets in x-y plane"""
+    x_axis=1
+    y_axis=0
+    if layercoord:
+        element = plot_tracking_2d(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis, yx_sizes)
+    else:
+        element = plot_tracking_2d_realcoord(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis)
+    return element
+
+
+def tracking_plot_zx(ax, ref_ptrs, tgt_ptrs, T_ref, yz_sizes, draw_point=True, layercoord=True):
+    """Draw the tracking process between two point sets in z-x plane"""
+    x_axis=1
+    y_axis=2
+    if layercoord:
+        element = plot_tracking_2d(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis, yz_sizes)
+    else:
+        element = plot_tracking_2d_realcoord(T_ref, ax, draw_point, ref_ptrs, tgt_ptrs, x_axis, y_axis)
+    return element
+
+
+def FFN_matching_plot(ref_ptrs, tgt_ptrs, initial_match_score):
+    """(Deprecated from v0.3) Draw the FFN_matching process"""
+    length_ref_ptrs = np.size(ref_ptrs, axis=0)
+    
+    tgt_ptrs_y_bias = tgt_ptrs.copy()
+    bias = (np.max(tgt_ptrs[:,0])-np.min(tgt_ptrs[:,0]))*2
+    tgt_ptrs_y_bias[:,0] = tgt_ptrs_y_bias[:,0]+bias
+    plt.ion()
+    fig = plt.figure(figsize=(9,9))
+    plt.scatter(ref_ptrs[:,1],-ref_ptrs[:,0],facecolors='none',edgecolors='r')
+    plt.plot(tgt_ptrs_y_bias[:,1],-tgt_ptrs_y_bias[:,0],'x')
+    plt.axis('equal')
+
+    cc_ref_tgt_temp=np.copy(initial_match_score)
+    for ptr_num in range(length_ref_ptrs):
+        cc_max=cc_ref_tgt_temp.max()
+        if cc_max<0.5:
+            break
+        cc_max_idx=np.unravel_index(cc_ref_tgt_temp.argmax(),cc_ref_tgt_temp.shape)
+    
+        plt.plot([ref_ptrs[cc_max_idx[1],1],tgt_ptrs_y_bias[cc_max_idx[0],1]],
+             [-ref_ptrs[cc_max_idx[1],0],-tgt_ptrs_y_bias[cc_max_idx[0],0]],'r-')
+        cc_ref_tgt_temp[cc_max_idx[0],:]=0
+        cc_ref_tgt_temp[:,cc_max_idx[1]]=0  
+    return fig
+
+
+def get_subregions(label_image, num):
+    """
+    Get individual regions of segmented cells
+
+    Parameters
+    ----------
+    label_image : numpy.ndarray
+        Image of segmented cells
+    num : int
+        Number of cells
+
+    Returns
+    -------
+    region_list : list
+        Cropped images of each cell
+    region_width : list
+        Width of each cell in x,y,and z axis
+    region_coord_min : list
+        Minimum coordinates of each element in region list
+    """
+    region_list = []
+    region_width = []
+    region_coord_min = []
+    for label in range(1, num + 1):
+        if label < num:
+            print(f"Calculating subregions... cell: {label}", end="\r")
+        else:
+            print(f"Calculating subregions... cell: {label}")
+        x_max, x_min, y_max, y_min, z_max, z_min = _get_coordinates(label, label_image, get_subregion=False)
+        region_list.append(label_image[x_min:x_max + 1, y_min:y_max + 1, z_min:z_max + 1] == label)
+        region_width.append([x_max + 1 - x_min, y_max + 1 - y_min, z_max + 1 - z_min])
+        region_coord_min.append([x_min, y_min, z_min])
+    return region_list, region_width, region_coord_min
+
+
+def _get_coordinates(label, label_image, get_subregion=True):
+    """
+    Get the coordinates of a specific label
+
+    Parameters
+    ----------
+    label : int
+        The number of the cell label
+    label_image :
+        The label image
+    get_subregion : bool
+        If True, return the image of the subregion and its size
+
+    Returns
+    -------
+    x_max : float
+    x_min : float
+    y_max : float
+    y_min : float
+    z_max : float
+    z_min : float
+        Coordinates for the subregion
+    subregion : numpy.ndarray
+        The subregion containing the label
+    np.size(region[0]) : int
+        The size of the subregion
+    """
+    region = np.where(label_image == label)
+    x_max, x_min = np.max(region[0]), np.min(region[0])
+    y_max, y_min = np.max(region[1]), np.min(region[1])
+    z_max, z_min = np.max(region[2]), np.min(region[2])
+    if not get_subregion:
+        return x_max, x_min, y_max, y_min, z_max, z_min
+    else:
+        subregion = np.zeros((x_max-x_min+11,y_max-y_min+11,z_max-z_min+11))
+        subregion[region[0] - x_min + 5, region[1] - y_min + 5, region[2] - z_min + 5] = 0.5
+        return x_max, x_min, y_max, y_min, z_max, z_min, subregion, np.size(region[0])
+
+
+def get_reference_vols(ensemble, vol, adjacent=False):
+    """
+    Get the reference volumes to calculate multiple prediction from which
+
+    Parameters
+    ----------
+    ensemble : int
+        The maximum number of predictions
+    vol : int
+        The current volume number at which the prediction was made
+    adjacent : bool
+        If True, get reference volumes from adjacent previous volumes. If False, from distributed previous volumes
+
+    Returns
+    -------
+    vols_list : list
+        The list of the reference volume numbers
+    """
+    if not ensemble:
+        return [vol - 1]
+    if vol - 1 < ensemble:
+        vols_list = list(range(1, vol))
+    else:
+        if adjacent:
+            vols_list = list(range(vol - ensemble, vol))
+        else:
+            vols_list = get_remote_vols(ensemble, vol)
+    return vols_list
+
+
+def get_remote_vols(ensemble, vol):
+    """Get distributed previous volumes"""
+    interval = (vol - 1) // ensemble
+    start = np.mod(vol - 1, ensemble) + 1
+    vols_list = list(range(start, vol - interval+1, interval))
+    return vols_list
```

### Comparing `3DeeCellTracker-0.4.5/CellTracker/tracker.py` & `3DeeCellTracker-0.5.0a0/CellTracker/tracker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,1551 +1,1551 @@
-"""
-A module for tracking and monitoring the intermediate results
-Author: Chentao Wen
-
-Notes
------
-To describe the cell positions, 3 different coordinates are used
-    layer-based
-        Use \"l_\" prefix, corresponding to the positions in the raw image
-    interpolated-layer-based
-        Use "i_" prefix, corresponding to the positions in the interpolated image
-    real-resolution
-        Use "r_" prefix, the cell positions along z axis are transformed to correspond the resolution in x-y plane
-"""
-
-import os
-import time
-from functools import reduce
-
-import cv2
-import matplotlib as mpl
-import matplotlib.image as mgimg
-import numpy as np
-import scipy.ndimage.measurements as snm
-from PIL import Image
-from tensorflow.keras.models import load_model
-from tensorflow.keras.preprocessing.image import ImageDataGenerator
-from matplotlib import animation
-from matplotlib import pyplot as plt
-from scipy.stats import trim_mean
-from skimage.measure import label
-from skimage.segmentation import relabel_sequential, find_boundaries
-
-from .preprocess import _make_folder, _normalize_image, _normalize_label, load_image
-from .track import pr_gls_quick, initial_matching_quick, gaussian_filter, \
-    get_reference_vols, get_subregions, tracking_plot_xy, tracking_plot_zx
-from .unet3d import unet3_prediction, _divide_img, _augmentation_generator
-from .watershed import watershed_2d, watershed_3d, watershed_2d_markers
-
-mpl.rcParams['image.interpolation'] = 'none'
-
-TITLE_STYLE = {'fontsize': 16, 'verticalalignment': 'bottom'}
-
-REP_NUM_PRGLS = 5
-REP_NUM_CORRECTION = 20
-BOUNDARY_XY = 6
-ALPHA_BLEND = 0.5
-
-
-def timer(func):
-    """A decorators to display runtime of a function"""
-
-    def wrapper_timer(*args, **kwargs):
-        tic = time.perf_counter()
-        value = func(*args, **kwargs)
-        toc = time.perf_counter()
-        elapsed_time = toc - tic
-        print(f"{func.__name__} took {elapsed_time:0.2f} seconds")
-        return value
-
-    return wrapper_timer
-
-
-def get_random_cmap(num, seed=1):
-    """
-    Generate a random cmap
-
-    Parameters
-    ----------
-    num : int
-        The number of colors to be generated
-    seed : int
-        The same value will lead to the same cmap
-
-    Returns
-    -------
-    cmap : matplotlib.colors.Colormap
-        The generated cmap
-    """
-    vals = np.linspace(0, 1, num + 1)
-    np.random.seed(seed)
-    np.random.shuffle(vals)
-    vals = np.concatenate(([0], vals[1:]))
-    cmap = plt.cm.colors.ListedColormap(plt.cm.rainbow(vals))
-    cmap.colors[0, :3] = 0
-    return cmap
-
-
-def get_tracking_path(adjacent, ensemble, folder_path):
-    """
-    Generate a path for storing tracking results according to tracking mode
-
-    Parameters
-    ----------
-    adjacent : bool
-    ensemble : bool or int
-    folder_path : str
-
-    Returns
-    -------
-    str
-        The generated path
-    """
-    if not ensemble:
-        return os.path.join(folder_path, "track_results_SingleMode/")
-    elif not adjacent:
-        return os.path.join(folder_path, "track_results_EnsembleDstrbtMode/")
-    else:
-        return os.path.join(folder_path, "track_results_EnsembleAdjctMode/")
-
-
-def read_image_ts(vol, path, name, z_range, print_=False):
-    """
-    Read a 3D image at time vol
-
-    Parameters
-    ----------
-    vol : int
-        A specific volume
-    path : str
-        Folder path
-    name : str
-        File name
-    z_range : tuple
-        Range of layers
-    print_ : bool
-        Whether print the image shape or not
-
-    Returns
-    -------
-    img_array : numpy.ndarray
-        An array of the image with shape (row, column, layer)
-    """
-    image_raw = []
-    for z in range(z_range[0], z_range[1]):
-        image_raw.append(cv2.imread(path + name % (vol, z), -1))
-    img_array = np.array(image_raw).transpose((1, 2, 0))
-    if print_:
-        print("Load images with shape:", img_array.shape)
-    return img_array
-
-
-def save_img3(z_siz, img, path, use_8_bit: bool):
-    """
-    Save a 3D image (at t=1) as 2D image sequence
-
-    Parameters
-    ----------
-    z_siz : int
-        The layer number of the 3D image
-    img : numpy.ndarray
-        The 3D image to be saved. Shape: (row, column, layer)
-    path : str
-        The path of the image files to be saved.
-        It should use formatted string to indicate volume number and then layer number, e.g. "xxx_t%04d_z%04i.tif"
-    use_8_bit: bool
-        The array will be transformed to 8-bit or 16-bit before saving as image.
-    """
-    dtype = np.uint8 if use_8_bit else np.uint16
-    for z in range(1, z_siz + 1):
-        img2d = img[:, :, z - 1].astype(dtype)
-        Image.fromarray(img2d).save(path % (1, z))
-
-
-def save_img3ts(z_range, img, path, t, use_8_bit: bool=True):
-    """
-    Save a 3D image at time t as 2D image sequence
-
-    Parameters
-    ----------
-    z_range : range
-        The range of layers to be saved
-    img : numpy.array
-        The 3D image to be saved
-    path : str
-        The path of the image files to be saved.
-        It should use formatted string to indicate volume number and then layer number, e.g. "xxx_t%04d_z%04i.tif"
-    t : int
-        The volume number for the image to be saved
-    use_8_bit: bool
-        The array will be transformed to 8-bit or 16-bit before saving as image.
-    """
-    dtype = np.uint8 if use_8_bit else np.uint16
-    for i, z in enumerate(z_range):
-        img2d = (img[:, :, z]).astype(dtype)
-        Image.fromarray(img2d).save(path % (t, i + 1))
-
-
-class Draw:
-    """
-    Class for drawing figures. Only use its method through Tracker instances.
-    """
-
-    def __init__(self):
-        self.history.r_tracked_coordinates = None
-        self.r_coordinates_tracked_t0 = None
-        self.segresult = None
-        self.vol = None
-        self.x_siz = None
-        self.y_siz = None
-        self.z_siz = None
-        self.cell_num = None
-        self.seg_cells_interpolated_corrected = None
-        self.cell_num_t0 = None
-        self.z_scaling = None
-        self.z_xy_ratio = None
-        self.Z_RANGE_INTERP = None
-        self.tracked_labels = None
-
-    def draw_segresult(self, percentile_high=99.9):
-        """
-        Draw the raw image and the segmentation result in current volume by max-projection and return an animation
-        showing the 3D images as 2D image sequences
-
-        Parameters
-        ----------
-        percentile_high : float
-            A percentile value (0.0-100.0) as the upper limitation of the intensities when showing the raw image
-
-        Returns
-        -------
-        anim : matplotlib.animation.ArtistAnimation
-            The animation including each layer of the raw image and the segmentation results
-            
-        Notes
-        -----
-        The lower limitation of intensities for showing the raw image is set to lower 10% by default.
-        """
-        axs, figs = self._subplots_3()
-        axs[0].set_title(f"Raw image at vol {self.vol}", fontdict=TITLE_STYLE)
-        axs[1].set_title(f"Cell regions at vol {self.vol} by U-Net", fontdict=TITLE_STYLE)
-        axs[2].set_title(f"Auto-_segment at vol {self.vol}", fontdict=TITLE_STYLE)
-        anim_obj = []
-        vmax = np.percentile(self.segresult.image_gcn, percentile_high)
-        vmin = np.percentile(self.segresult.image_gcn, 10)
-        for z in range(self.z_siz):
-            obj1 = axs[0].imshow(self.segresult.image_gcn[:, :, z],
-                                 vmin=vmin, vmax=vmax, cmap="gray")
-            obj2 = axs[1].imshow(self.segresult.image_cell_bg[0, :, :, z, 0] > 0.5, cmap="gray")
-            obj3 = axs[2].imshow(self.segresult.segmentation_auto[:, :, z],
-                                 vmin=0, vmax=self.cell_num, cmap=get_random_cmap(num=self.cell_num))
-            anim_obj.append([obj1, obj2, obj3])
-        anim = animation.ArtistAnimation(figs, anim_obj, interval=200).to_jshtml()
-
-        axs[0].imshow(np.max(self.segresult.image_gcn, axis=2), vmin=vmin, vmax=vmax, cmap="gray")
-        axs[1].imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0] > 0.5, axis=2), cmap="gray")
-        axs[2].imshow(np.max(self.segresult.segmentation_auto, axis=2),
-                      cmap=get_random_cmap(num=self.cell_num))
-        print("Segmentation results (max projection):")
-        return anim
-
-    def draw_manual_seg1(self):
-        """
-        Draw the cell regions and the interpolated/smoothed manual segmentation with max-projection in volume 1
-        """
-        axm, figm = self._subplots_2_horizontal()
-        axm[0].imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=2) > 0.5, cmap="gray")
-        axm[0].set_title(f"Cell regions at vol {self.vol} by U-Net", fontdict=TITLE_STYLE)
-        axm[1].imshow(np.max(self.seg_cells_interpolated_corrected, axis=2),
-                      cmap=get_random_cmap(num=self.cell_num_t0))
-        axm[1].set_title(f"Manual _segment at vol 1", fontdict=TITLE_STYLE)
-
-    def _draw_transformation(self, ax, r_coordinates_predicted_pre, r_coordinates_segmented_post,
-                             r_coordinates_predicted_post, layercoord, draw_point=True):
-        """
-        Draw each iteration of the tracking by FFN + PR-GLS
-        """
-        element1 = tracking_plot_xy(
-            ax[0], r_coordinates_predicted_pre, r_coordinates_segmented_post, r_coordinates_predicted_post,
-            (self.y_siz, self.x_siz), draw_point, layercoord)
-        element2 = tracking_plot_zx(
-            ax[1], r_coordinates_predicted_pre, r_coordinates_segmented_post, r_coordinates_predicted_post,
-            (self.y_siz, self.z_siz), draw_point, layercoord)
-        if layercoord:
-            ax[0].set_aspect('equal', 'box')
-            ax[1].set_aspect('equal', 'box')
-        return element1 + element2
-
-    def draw_correction(self, i_disp_from_vol1_updated, r_coor_predicted):
-        """
-        Draw the accurate correction superimposed on the cell regions
-
-        Parameters
-        ----------
-        i_disp_from_vol1_updated : numpy.ndarray
-            The current displacement of each cell from volume 1. Interpolated coordinates.
-        r_coor_predicted : numpy.ndarray
-            The current coordinates of each cell. Real coordinates
-        """
-        ax, fig = self._subplots_2_horizontal()
-        ax[0].set_title("Accurate Correction (y-x plane)", size=16)
-        ax[1].set_title("Accurate Correction (y-z plane)", size=16)
-        self._draw_correction(ax, r_coor_predicted, i_disp_from_vol1_updated)
-        return None
-
-    def _draw_correction(self, ax, r_coor_predicted, i_disp_from_vol1_updated):
-        """
-        Draw the accurate correction of cell positions after FFN + PR-GLS transformation
-        """
-        _ = self._draw_transformation(
-            [ax[0], ax[1]],
-            self._transform_real_to_layer(r_coor_predicted),
-            self._transform_real_to_layer(self.segresult.r_coordinates_segment),
-            self._transform_real_to_layer(self.r_coordinates_tracked_t0) +
-            self._transform_interpolated_to_layer(i_disp_from_vol1_updated),
-            layercoord=True, draw_point=False)
-        ax[0].imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=2) > 0.5, cmap="gray",
-                     extent=(0, self.y_siz - 1, self.x_siz - 1, 0))
-        ax[1].imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=0).T > 0.5, aspect=self.z_xy_ratio,
-                     cmap="gray", extent=(0, self.y_siz - 1, self.z_siz - 1, 0))
-
-        return None
-
-    def draw_overlapping(self, cells_on_boundary_local, volume2, i_disp_from_vol1_updated):
-        """
-        Draw the overlapping of cell regions (gray) and the labels before/after matching
-
-        Parameters
-        ----------
-        cells_on_boundary_local : numpy.ndarray
-            A 1d array of cells on boundary (1, ignored in tracking) or not (0).
-        volume2 : int
-            The current volume
-        i_disp_from_vol1_updated : numpy.ndarray
-            The displacement of each cell from volume 1. Interpolated coordinates.
-        """
-        self.tracked_labels = self._transform_motion_to_image(cells_on_boundary_local, i_disp_from_vol1_updated)
-        self._draw_matching(volume2)
-        plt.pause(0.1)
-        return None
-
-    def _draw_matching(self, volume2):
-        """Draw the overlapping of cell and labels"""
-        axc, figc = self._subplots_4()
-        self._draw_before_matching(axc[0], axc[1], volume2)
-        self._draw_after_matching(axc[2], axc[3], volume2)
-        plt.tight_layout()
-        return None
-
-    def _draw_matching_6panel(self, target_volume, ax, r_coor_predicted_mean, i_disp_from_vol1_updated):
-        """Draw the tracking process in a specific volume"""
-        for ax_i in ax:
-            ax_i.cla()
-        plt.suptitle(f"Tracking results at vol {target_volume}", size=16)
-
-        _ = self._draw_transformation([ax[0], ax[1]], self.history.r_tracked_coordinates[target_volume - 2],
-                                      self.segresult.r_coordinates_segment, r_coor_predicted_mean, layercoord=False)
-        self._draw_correction([ax[2], ax[3]], r_coor_predicted_mean, i_disp_from_vol1_updated)
-        self._draw_after_matching(ax[4], ax[5], target_volume, legend=False)
-        self._set_layout_anim()
-        for axi in ax:
-            plt.setp(axi.get_xticklabels(), visible=False)
-            plt.setp(axi.get_yticklabels(), visible=False)
-            axi.tick_params(axis='both', which='both', length=0)
-            axi.axis("off")
-        return None
-
-    def _draw_before_matching(self, ax1, ax2, volume2):
-        """Draw overlapping of cells and labels before matching"""
-        ax1.imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=2) > 0.5, cmap="gray")
-        ax1.imshow(np.max(self.seg_cells_interpolated_corrected[:, :, self.Z_RANGE_INTERP], axis=2),
-                   cmap=get_random_cmap(num=self.cell_num_t0), alpha=ALPHA_BLEND)
-
-        ax2.imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=0).T > 0.5, aspect=self.z_xy_ratio,
-                   cmap="gray")
-        ax2.imshow(np.max(self.seg_cells_interpolated_corrected[:, :, self.Z_RANGE_INTERP], axis=0).T,
-                   cmap=get_random_cmap(num=self.cell_num_t0), aspect=self.z_xy_ratio, alpha=ALPHA_BLEND)
-        ax1.set_title(f"Before matching: Cells at vol {volume2} + Labels at vol {self.vol} (y-x plane)",
-                      fontdict=TITLE_STYLE)
-        ax2.set_title(f"Before matching (y-z plane)",
-                      fontdict=TITLE_STYLE)
-
-    def _draw_after_matching(self, ax1, ax2, volume2, legend=True):
-        """Draw overlapping of cells and labels after matching"""
-        ax1.imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=2) > 0.5, cmap="gray")
-        ax1.imshow(np.max(self.tracked_labels, axis=2),
-                   cmap=get_random_cmap(num=self.cell_num_t0), alpha=ALPHA_BLEND)
-
-        ax2.imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=0).T > 0.5, aspect=self.z_xy_ratio,
-                   cmap="gray")
-        ax2.imshow(np.max(self.tracked_labels, axis=0).T, cmap=get_random_cmap(num=self.cell_num_t0),
-                   aspect=self.z_xy_ratio, alpha=ALPHA_BLEND)
-        if legend:
-            ax1.set_title(f"After matching: Cells at vol {volume2} + Labels at vol {volume2} (y-x plane)",
-                          fontdict=TITLE_STYLE)
-            ax2.set_title(f"After matching (y-z plane)",
-                          fontdict=TITLE_STYLE)
-        return None
-
-    def _subplots_ffnprgls_animation(self):
-        """Generate a figure to draw the FFN + PR-GLS transformation"""
-        ax, fig = self._subplots_2_horizontal()
-        ax[0].set_title("Matching by FFN + PR-GLS (y-x plane)", fontdict=TITLE_STYLE)
-        ax[1].set_title("Matching by FFN + PR-GLS (y-z plane)", fontdict=TITLE_STYLE)
-        plt.tight_layout()
-        plt.close(fig)
-        return ax, fig
-
-    def _subplots_2_horizontal(self):
-        """Generate 2 subplots aligned horizontally in a figure"""
-        fig, ax = plt.subplots(1, 2, figsize=(20, int(12 * self.x_siz / self.y_siz)))
-        plt.tight_layout()
-        return ax, fig
-
-    def _subplots_3(self):
-        """
-        Generate 3 subplots in a figure
-
-        Returns
-        -------
-        ax : list of matplotlib.axes.Axes
-            The subplots to show each panel
-        fig : matplotlib.figure.Figure
-            The figure to draw tracking process
-        """
-        fig = plt.figure(figsize=(20, int(24 * self.x_siz / self.y_siz)))
-        ax = plt.subplot(221), plt.subplot(222), plt.subplot(223)
-        plt.tight_layout()
-        return ax, fig
-
-    def _subplots_4(self):
-        """Generate a (2, 2) layout subplots in a figure"""
-        fig, axs = plt.subplots(2, 2, figsize=(20, int(24 * self.x_siz / self.y_siz)))
-        ax = axs[0, 0], axs[0, 1], axs[1, 0], axs[1, 1]
-        plt.tight_layout()
-        return ax, fig
-
-    def subplots_tracking(self):
-        """
-        Generate a (3, 2) layout subplots in a figure
-
-        Returns
-        -------
-        fig : matplotlib.figure.Figure
-            The figure to draw tracking process
-        ax : list of matplotlib.axes.Axes
-            The subplots to show each panel
-        """
-        fig, axs = plt.subplots(3, 2, figsize=(14, int(21 * self.x_siz / self.y_siz)))
-        ax = axs[0, 0], axs[0, 1], axs[1, 0], axs[1, 1], axs[2, 0], axs[2, 1]
-        return fig, ax
-
-    @staticmethod
-    def _set_layout_anim():
-        """set the layout to show the tracking process dynamically in the notebook backend"""
-        plt.tight_layout()
-        plt.subplots_adjust(right=0.9, bottom=0.1)
-
-    def _transform_interpolated_to_layer(self, i_disp_from_vol1_updated):
-        """Overridden in Tracker"""
-        raise NotImplementedError("Must override this method")
-
-    def _transform_motion_to_image(self, cells_on_boundary_local, i_disp_from_vol1_updated):
-        """Overridden in Tracker"""
-        raise NotImplementedError("Must override this method")
-
-    def _transform_real_to_layer(self, r_coor_predicted):
-        """Overridden in Tracker"""
-        raise NotImplementedError("Must override this method")
-
-
-class SegResults:
-    """
-    Class to store the segmentation result.
-
-    Attributes
-    ----------
-    image_cell_bg : numpy.ndarray
-        The cell/non-cell predictions by 3D U-Net
-    l_center_coordinates : list of tuple
-        The detected centers coordinates of the cells, using voxels as the unit
-    segmentation_auto : numpy.ndarray
-        The individual cells predicted by 3D U-Net + watershed
-    image_gcn : numpy.ndarray
-        The raw image divided by 65535
-    r_coordinates_segment : numpy.ndarray
-        Transformed from l_center_coordinates, with the z coordinates corrected by the resolution relative to x-y plane
-    """
-
-    def __init__(self):
-        self.image_cell_bg = None
-        self.l_center_coordinates = None
-        self.segmentation_auto = None
-        self.image_gcn = None
-        self.r_coordinates_segment = None
-
-    def update_results(self, image_cell_bg, l_center_coordinates, segmentation_auto,
-                       image_gcn, r_coordinates_segment):
-        """Update the attributes of a SegResults instance"""
-        self.image_cell_bg = image_cell_bg
-        self.l_center_coordinates = l_center_coordinates
-        self.segmentation_auto = segmentation_auto
-        self.image_gcn = image_gcn
-        self.r_coordinates_segment = r_coordinates_segment
-
-
-class Segmentation:
-    """
-    Class for segmentation. Only use it through the Tracker instance.
-    """
-
-    def __init__(self, volume_num, siz_xyz: tuple, z_xy_ratio, z_scaling, shrink):
-        self.volume_num = volume_num
-        self.x_siz = siz_xyz[0]
-        self.y_siz = siz_xyz[1]
-        self.z_siz = siz_xyz[2]
-        self.z_xy_ratio = z_xy_ratio
-        self.z_scaling = z_scaling
-        self.shrink = shrink
-        self.noise_level = None
-        self.min_size = None
-        self.vol = None
-        self.paths = None
-        self.unet_model = None
-        self.r_coordinates_segment_t0 = None
-        self.segresult = SegResults()
-
-    def set_segmentation(self, noise_level=None, min_size=None, del_cache=False):
-        """
-        Set the segmentation parameters
-        If parameters changed or if reset_=True, delete cached segmentation.
-        
-        Parameters
-        ----------
-        noise_level : float, optional
-            Modify the attribute "noise_level" to this value. If None, no modification occur. Default: None
-        min_size : int, optional
-            Modify the attribute "min_size" to this value. If None, no modification occur. Default: None
-        del_cache : bool, optional
-            If True, delete all cached segmentation files under "/unet" folder. Default: False 
-        """
-        if self.noise_level == noise_level and self.min_size == min_size:
-            print("Segmentation parameters were not modified")
-        elif noise_level == None and min_size == None:
-            print("Segmentation parameters were not modified")
-        else:
-            if noise_level is not None:
-                self.noise_level = noise_level
-            if min_size is not None:
-                self.min_size = min_size
-            print(f"Parameters were modified: noise_level={self.noise_level}, min_size={self.min_size}")
-            for f in os.listdir(self.paths.unet_cache):
-                os.remove(os.path.join(self.paths.unet_cache, f))
-            print(f"All files under /unet folder were deleted")
-        if del_cache:
-            for f in os.listdir(self.paths.unet_cache):
-                os.remove(os.path.join(self.paths.unet_cache, f))
-            print(f"All files under /unet folder were deleted")
-
-    @staticmethod
-    def _transform_disps(disp, factor):
-        """Transform the coordinates with different units along z"""
-        new_disp = np.array(disp).copy()
-        new_disp[:, 2] = new_disp[:, 2] * factor
-        return new_disp
-
-    def _transform_layer_to_real(self, voxel_disp):
-        """Transform the coordinates from layer to real"""
-        return self._transform_disps(voxel_disp, self.z_xy_ratio)
-
-    def _transform_real_to_interpolated(self, r_disp):
-        """Transform the coordinates from real to interpolated"""
-        return np.rint(self._transform_disps(r_disp, self.z_scaling / self.z_xy_ratio)).astype(int)
-
-    def _transform_real_to_layer(self, r_disp):
-        """Transform the coordinates from real to layer"""
-        return np.rint(self._transform_disps(r_disp, 1 / self.z_xy_ratio)).astype(int)
-
-    def _transform_interpolated_to_layer(self, r_disp):
-        """Transform the coordinates from real to layer"""
-        return np.rint(self._transform_disps(r_disp, 1 / self.z_scaling)).astype(int)
-
-    def load_unet(self):
-        """
-        Load the pretrained unet model (keras Model file like "xxx.h5") and save its weights for retraining
-        """
-        self.unet_model = load_model(os.path.join(self.paths.models, self.paths.unet_model_file))
-        self.unet_model.save_weights(os.path.join(self.paths.unet_weights, 'weights_initial.h5'))
-        print("Loaded the 3D U-Net model")
-
-    def segment_vol1(self, method="min_size"):
-        """
-        Segment the volume 1 of the 3D time lapse image and save the segmentation result into "/auto_vol1" folder
-
-        Parameters
-        ----------
-        method : str
-            The method to remove the small regions in watershed. If "min_size", remove cells whose size is smaller than
-            this value. If "cell_num", sort the cells by their sizes and only keep the top "self.cell_num" cells.
-            Default: "min_size"
-
-        """
-        self.vol = 1
-        self.segresult.update_results(*self._segment(self.vol, method=method, print_shape=True))
-        self.r_coordinates_segment_t0 = self.segresult.r_coordinates_segment.copy()
-        use_8_bit = True if self.segresult.segmentation_auto.max() <= 255 else False
-
-        # save the segmented cells of volume #1
-        save_img3(z_siz=self.z_siz, img=self.segresult.segmentation_auto,
-                  path=self.paths.auto_segmentation_vol1 + "auto_t%04i_z%04i.tif", use_8_bit=use_8_bit)
-        print(f"Segmented volume 1 and saved it")
-
-    def _segment(self, vol, method, print_shape=False):
-        """
-        Segment cells from one volume of 3D image
-
-        Parameters
-        ----------
-        vol : int
-            A specific volume
-        method : str
-            "min_size" or "cell_num" used in watershed
-        print_shape : bool
-            If True, print the shape of the raw 3D image
-
-        Returns
-        -------
-        image_cell_bg : numpy.ndarray
-            The cell/non-cell predictions by 3D U-Net
-        l_center_coordinates : list of tuple
-            The detected centers coordinates of the cells, using voxels as the unit
-        segmentation_auto : numpy.ndarray
-            The individual cells predicted by 3D U-Net + watershed
-        image_gcn : numpy.ndarray
-            The raw image divided by 65535
-        r_coordinates_segment : numpy.ndarray
-            Transformed from l_center_coordinates, with the z coordinates corrected by the resolution relative to x-y
-            plane
-        """
-        image_raw = read_image_ts(vol, self.paths.raw_image, self.paths.image_name, (1, self.z_siz + 1),
-                                  print_=print_shape)
-        # image_gcn will be used to correct tracking results
-        image_gcn = (image_raw.copy() / 65536.0)
-        image_cell_bg = self._predict_cellregions(image_raw, vol)
-        if np.max(image_cell_bg) <= 0.5:
-            raise ValueError("No cell was detected by 3D U-Net! Try to reduce the noise_level.")
-
-        # segment connected cell-like regions using _watershed
-        segmentation_auto = self._watershed(image_cell_bg, method)
-        if np.max(segmentation_auto) == 0:
-            raise ValueError("No cell was detected by watershed! Try to reduce the min_size.")
-
-        # calculate coordinates of the centers of each segmented cell
-        l_center_coordinates = snm.center_of_mass(segmentation_auto > 0, segmentation_auto,
-                                                  range(1, segmentation_auto.max() + 1))
-        r_coordinates_segment = self._transform_layer_to_real(l_center_coordinates)
-
-        return image_cell_bg, l_center_coordinates, segmentation_auto, image_gcn, r_coordinates_segment
-
-    def _predict_cellregions(self, image_raw, vol):
-        """
-        Predict cell regions by 3D U-Net and save it if the prediction has not been cached
-        """
-        try:
-            image_cell_bg = np.load(self.paths.unet_cache + "t%04i.npy" % vol, allow_pickle=True)
-        except OSError:
-            image_cell_bg = self._save_unet_regions(image_raw, vol)
-        return image_cell_bg
-
-    def _save_unet_regions(self, image_raw, vol):
-        """Predict the cell regions by 3D U-Net and cache the prediction"""
-        # pre-processing: local contrast normalization
-        image_norm = np.expand_dims(_normalize_image(image_raw, self.noise_level), axis=(0, 4))
-        # predict cell-like regions using 3D U-net
-        image_cell_bg = unet3_prediction(image_norm, self.unet_model, shrink=self.shrink)
-        np.save(self.paths.unet_cache + "t%04i.npy" % vol, np.array(image_cell_bg, dtype="float16"))
-        return image_cell_bg
-
-    def _watershed(self, image_cell_bg, method):
-        """
-        Segment the cell regions by watershed method
-        """
-        image_watershed2d_wo_border, _ = watershed_2d(image_cell_bg[0, :, :, :, 0], z_range=self.z_siz,
-                                                      min_distance=7)
-        _, image_watershed3d_wi_border, min_size, cell_num = watershed_3d(
-            image_watershed2d_wo_border, samplingrate=[1, 1, self.z_xy_ratio], method=method,
-            min_size=self.min_size, cell_num=self.cell_num, min_distance=3)
-        segmentation_auto, fw, inv = relabel_sequential(image_watershed3d_wi_border)
-        self.min_size = min_size
-        if method == "min_size":
-            self.cell_num = cell_num
-        return segmentation_auto
-
-
-class Paths:
-    """
-    Paths for storing data and results used by Tracker instance
-
-    Attributes
-    ----------
-    folder_path : str
-        The path of the folder to store all related data
-        including images, 3D U-Net, FFN models and segmentation/tracking results.
-    models : str
-        The path of the folder to store the pretrained and retrained models
-    unet_cache : str
-        The path of the folder to store the cached cell regions (predicted by 3D U-Net) to accelerate the tracking
-    raw_image : str
-        The path of the folder to store the raw images to be tracked
-    auto_segmentation_vol1 : str
-        The path of the folder to store the automatic segmentation in volume 1 to be used in manual correction
-    manual_segmentation_vol1 : str
-        The path of the folder to store the manually corrected segmentation in volume 1
-    unet_weights : str
-        The path of the folder to store the retrained weights of 3D U-Net
-    track_results :
-        The path of the folder to store the tracking results (in images with labels)
-    track_information : str
-        The path of the folder to store the displacements, coordinates information of segmented and tracked cells
-    anim : str
-        The path of the folder to store the animation of tracking in each volume
-    image_name : str
-        The file names of the raw image files.
-        It should use formatted string to indicate volume number and then layer number, e.g. "xxx_t%04d_z%04i.tif"
-    unet_model_file : str
-        The filename of the pretrained 3D U-Net (keras model such as "xxx.h5")
-    ffn_model_file : str
-        The filename of the pretrained FFN model (keras model such as "xxx.h5")
-    """
-
-    def __init__(self, folder_path, image_name, unet_model_file, ffn_model_file):
-        self.folder = folder_path
-        self.models = None
-        self.unet_cache = None
-        self.raw_image = None
-        self.auto_segmentation_vol1 = None
-        self.manual_segmentation_vol1 = None
-        self.unet_weights = None
-        self.track_results = None
-        self.track_information = None
-        self.anim = None
-        self.image_name = image_name
-        self.unet_model_file = unet_model_file
-        self.ffn_model_file = ffn_model_file
-
-    def make_folders(self, adjacent, ensemble):
-        """
-        Make folders for storing data, models, and results
-        """
-        print("Following folders were made under:", os.getcwd())
-        folder_path = self.folder
-        self.raw_image = _make_folder(os.path.join(folder_path, "data/"))
-        self.auto_segmentation_vol1 = _make_folder(os.path.join(folder_path, "auto_vol1/"))
-        self.manual_segmentation_vol1 = _make_folder(os.path.join(folder_path, "manual_vol1/"))
-        self.track_information = _make_folder(os.path.join(folder_path, "track_information/"))
-        self.models = _make_folder(os.path.join(folder_path, "models/"))
-        self.unet_cache = _make_folder(os.path.join(folder_path, "unet_cache/"))
-        track_results_path = get_tracking_path(adjacent, ensemble, folder_path)
-        self.track_results = _make_folder(track_results_path)
-        self.anim = _make_folder(os.path.join(folder_path, "anim/"))
-        self.unet_weights = _make_folder(os.path.join(self.models, "unet_weights/"))
-
-
-class History:
-    """
-    Storing the tracking histories
-
-    Attributes
-    ----------
-    r_displacements :  list of numpy.ndarray
-        The displacements of each cell in each volume relative to their positions in volume 1. Shape: (cell_num, 3)
-    r_segmented_coordinates : list of numpy.ndarray
-        The positions of each cell segmented by 3D U-Net + watershed in each volume. Shape: (cell_num, 3)
-    r_tracked_coordinates : list of numpy.ndarray
-        The positions of each cell tracked by FFN + PR-GLS + corrections in each volume. Shape: (cell_num, 3)
-    anim : list
-        The images of tracking process in each volume (from volume 2)
-    """
-
-    def __init__(self):
-        self.r_displacements = []
-        self.r_segmented_coordinates = []
-        self.r_tracked_coordinates = []
-        self.anim = []
-
-
-class Tracker(Segmentation, Draw):
-    """
-    Data and methods for tracking cells
-
-    Attributes
-    ----------
-    volume_num :  int
-        The number of volumes (time points) of the 3D + T image to be tracked
-    x_siz : int
-    y_siz : int
-    z_siz : int
-        Size of each 3D image. Obtained from the siz_xyz parameter (tuple) with (x_siz:Height, y_siz:Width, z_siz:Depth)
-    z_xy_ratio : float
-        The resolution (length per voxels) ratio between the z axis and the x-y plane, used in tracking.
-        Does not need to very precise
-    z_scaling : int
-        An integer (>= 1) for interpolating/smoothing images along z direction.
-        z_scaling = 1 makes no interpolation but only smoothing.
-    noise_level : float
-        A threshold to discriminate noise/artifacts from cell regions, used in preprocess._normalize_image function
-    min_size : int
-        A threshold of the minimum cell size (unit: voxels) to remove tiny regions that may be non-cell objects,
-        used in watershed.watershed_3d function
-    beta_tk : float
-        Control coherence by a weighted average of movements from neighbouring cells.
-        A larger BETA will include more cells and thus generates more coherent movements.
-    lambda_tk : float
-        Control coherence by applying a penalty for the incoherence of cell movements.
-        A large LAMBDA will generates more coherent movements.
-    maxiter_tk : int
-        The maximum number of iterations of PR-GLS during once application of FFN + PR-GLS.
-        A large values will generate more accurate tracking but will also increase the runtime.
-    cell_num : int
-        The number of cells to be extracted from watershed. It is used only when segmentation method is "cell_num".
-        Default: 0
-    ensemble : bool or int, optional
-        If False, track cells in single mode. If an integer, track cells in ensemble mode.
-        The integer indicates number of predictions to be averaged. Default: False
-    adjacent : bool, optional
-        Only used in ensemble mode. If True, make predictions of cell positions at t from
-        adjacent previous volumes such as t-1, t-2, t-3,..., t-10 (when ensemble=10).
-        If False, make prediction from distributed previous volumes. For example, predict cells at t=101 from
-        t = 1, 11, 21, ..., 91 (when ensemble=10). Default: False
-    shrink : tuple, optional
-        For padding the images before applying U-Net and for shrinking the cell prediction in the center part
-        of the U-Net output. Each value should be < (x, y, or z size of the U-Net input // 2), Default: (24, 24, 2)
-    miss_frame : list, optional
-        A list of volumes (int) which includes serious problem in the raw images and thus will be skipped for tracking.
-        Default: None
-    cell_num_t0 : int
-        The detected cell numbers in the manually corrected segmentation in volume 1
-    Z_RANGE_INTERP : Range object
-        The sequence of the indexes along z axis in the interpolated image corresponding to the layers in the raw image
-    region_list : list
-        List of the 3D sub-images [array_cell1, array_cell2, ...] with binary values
-        (1: this cell; 0: background or other cells)
-    region_width : list
-        List of the width of [[x_width, y_width, z_width]_cell1, ...] each sub-image in x, y, and z axis
-    region_xyz_min : list
-        List of the minimum coordinates [[x_min, y_min, z_min]_cell1, ...] of each sub-image in the raw image
-    pad_x : int
-    pad_y : int
-    pad_z : int
-        The values for padding a zero array with the raw image size
-    label_padding : numpy.ndarray
-        A 3D array with zero values, used in accurate correction during tracking.
-        Shape: (row + 2 * pad_x, column + 2 * pad_y, layer + 2 * pad_z)
-    segmentation_manual_relabels : numpy.ndarray
-        The relabeled manual segmentation. Shape: (row, column, layer)
-    segresult : SegResults object
-        The results of the segmentation in current volume
-    unet_model : keras.Model
-        The pretrained/retrained 3D U-Net model
-    """
-
-    def __init__(self,
-                 volume_num, siz_xyz: tuple, z_xy_ratio, z_scaling, noise_level, min_size, beta_tk,
-                 lambda_tk, maxiter_tk, folder_path, image_name, unet_model_file,
-                 ffn_model_file, cell_num=0, ensemble=False, adjacent=False,
-                 shrink=(24, 24, 2), miss_frame=None
-                 ):
-        Segmentation.__init__(self, volume_num, siz_xyz, z_xy_ratio, z_scaling, shrink)
-
-        self.miss_frame = [] if not miss_frame else miss_frame
-        self.noise_level = noise_level
-        self.min_size = min_size
-        self.beta_tk = beta_tk
-        self.lambda_tk = lambda_tk
-        self.max_iteration = maxiter_tk
-        self.ensemble = ensemble
-        self.adjacent = adjacent
-        self.cell_num = cell_num
-        self.cell_num_t0 = None
-        self.Z_RANGE_INTERP = None
-        self.region_list = None
-        self.region_width = None
-        self.region_xyz_min = None
-        self.pad_x = None
-        self.pad_y = None
-        self.pad_z = None
-        self.label_padding = None
-        self.segmentation_manual_relabels = None
-        self.cells_on_boundary = None
-        self.ffn_model = None
-        self.val_losses = None
-        self.paths = Paths(folder_path, image_name, unet_model_file, ffn_model_file)
-        self.history = History()
-        self.paths.make_folders(adjacent, ensemble)
-        self.use_8_bit = True
-
-    def set_tracking(self, beta_tk, lambda_tk, maxiter_tk):
-        """
-        Set tracking parameters
-
-        Parameters
-        ----------
-        beta_tk : float
-        lambda_tk : float
-        maxiter_tk : int
-        """
-        if self.beta_tk == beta_tk and self.lambda_tk == lambda_tk and self.max_iteration == maxiter_tk:
-            print("Tracking parameters were not modified")
-        else:
-            self.beta_tk = beta_tk
-            self.lambda_tk = lambda_tk
-            self.max_iteration = maxiter_tk
-            print(f"Parameters were modified: beta_tk={self.beta_tk}, "
-                  f"lambda_tk={self.lambda_tk}, maxiter_tk={self.max_iteration}")
-
-    def load_manual_seg(self):
-        """
-        Load the manually corrected segmentation in the "/manual_vol1" folder
-
-        Notes
-        -----
-        The files to be loaded in "manual_vol1" folder should be 2D images corresponding to cell labels in
-        each layer of the 3D image in volume 1
-        """
-        segmentation_manual = load_image(self.paths.manual_segmentation_vol1, print_=False)
-        print("Loaded manual _segment at vol 1")
-        self.segmentation_manual_relabels, _, _ = relabel_sequential(segmentation_manual)
-        if self.segmentation_manual_relabels.max() > 255:
-            self.use_8_bit = False
-
-    def _retrain_preprocess(self):
-        """
-        Prepare the training data for retraining the unet model
-        """
-        self.image_raw_vol1 = read_image_ts(1, self.paths.raw_image, self.paths.image_name, (1, self.z_siz + 1))
-        self.train_image_norm = _normalize_image(self.image_raw_vol1, self.noise_level)
-        self.label_vol1 = self._remove_2d_boundary(self.segmentation_manual_relabels) > 0
-        self.train_label_norm = _normalize_label(self.label_vol1)
-        print("Images were normalized")
-
-        self.train_subimage = _divide_img(self.train_image_norm, self.unet_model.input_shape[1:4])
-        self.train_subcells = _divide_img(self.train_label_norm, self.unet_model.input_shape[1:4])
-        print("Images were divided")
-
-        image_gen = ImageDataGenerator(rotation_range=90, width_shift_range=0.2, height_shift_range=0.2,
-                                       shear_range=0.2, horizontal_flip=True, fill_mode='reflect')
-
-        self.train_generator = _augmentation_generator(self.train_subimage, self.train_subcells, image_gen, batch_siz=8)
-        self.valid_data = (self.train_subimage, self.train_subcells)
-        print("Data for training 3D U-Net were prepared")
-
-    def _remove_2d_boundary(self, labels3d):
-        """
-        Remove boundaries between touching cells in x-y plane
-
-        Parameters
-        ----------
-        labels3d : numpy.ndarray
-            The 3D image of cell labels
-
-        Returns
-        -------
-        labels_new : numpy.ndarray
-            The new image with the boundaries removed
-        """
-        labels_new = labels3d.copy()
-        for z in range(self.z_siz):
-            labels = labels_new[:, :, z]
-            labels[find_boundaries(labels, mode='outer') == 1] = 0
-        return labels_new
-
-    def retrain_unet(self, iteration=10, weights_name="unet_weights_retrain_"):
-        """
-        Retrain the pretrained self.unet_model using the manually corrected segmentation in volume 1. Here the training
-        data are the randomly augmented sub-images from vol 1 data while the validation data are from the same vol but
-        without augmentation. The ground truth and the updated predictions are displayed after each epoch when the
-        val_loss was reduced.
-
-        Parameters
-        ----------
-        iteration : int, optional
-            The number of epochs to train the unet_model. Default: 10
-        weights_name : str, optional
-            The filename of the unet weights to be saved. Default: "unet_weights_retrain_"
-
-        Notes
-        -----
-        The boundaries (on x-y planes) between touching cells in the manual segmentation are removed to force the model
-        to predict boundaries as non-cell regions.
-
-        See Also
-        --------
-        _retrain_preprocess :  Preprocess of the training data
-        _remove_2d_boundary : Remove the boundaries between cells
-        """
-        self._retrain_preprocess()
-
-        self.unet_model.compile(loss='binary_crossentropy', optimizer="adam")
-        self.unet_model.load_weights(os.path.join(self.paths.unet_weights, 'weights_initial.h5'))
-
-        # evaluate model prediction before retraining
-        val_loss = self.unet_model.evaluate(self.train_subimage, self.train_subcells)
-        print("val_loss before retraining: ", val_loss)
-        self.val_losses = [val_loss]
-        self._draw_retrain(step="before retrain")
-
-        for step in range(1, iteration + 1):
-            self.unet_model.fit_generator(self.train_generator, validation_data=self.valid_data, epochs=1,
-                                          steps_per_epoch=60)
-            loss = self.unet_model.history.history["val_loss"][-1]
-            if loss < min(self.val_losses):
-                print("val_loss updated from ", min(self.val_losses), " to ", loss)
-                self.unet_model.save_weights(os.path.join(self.paths.unet_weights, weights_name + f"step{step}.h5"))
-                self._draw_retrain(step)
-            self.val_losses.append(loss)
-
-    def _draw_retrain(self, step):
-        """Draw the ground truth and the updated predictions during retraining the unet"""
-        train_prediction = np.squeeze(
-            unet3_prediction(np.expand_dims(self.train_image_norm, axis=(0, 4)), self.unet_model))
-        fig, axs = plt.subplots(1, 2, figsize=(20, int(12 * self.x_siz / self.y_siz)))
-        axs[0].imshow(np.max(self.label_vol1, axis=2), cmap="gray")
-        axs[1].imshow(np.max(train_prediction, axis=2) > 0.5, cmap="gray")
-        axs[0].set_title("Cell regions from manual segmentation at vol 1", fontdict=TITLE_STYLE)
-        axs[1].set_title(f"Cell prediction at step {step} at vol 1", fontdict=TITLE_STYLE)
-        plt.tight_layout()
-        plt.pause(0.1)
-
-    def select_unet_weights(self, step, weights_name="unet_weights_retrain_"):
-        """
-        Select a satisfied unet weights to restore it.
-
-        Parameters
-        ----------
-        step : int
-            The step with a satisfied prediction of cell regions in the trained image. If step=0, the initial weights
-            before retraining will be restored.
-        weights_name : str, optional
-            The filename of the unet weights to be saved. Default: "unet_weights_retrain_"
-
-        Raises
-        ------
-        ValueError
-            If step < 0
-        """
-        if step == 0:
-            self.unet_model.load_weights(os.path.join(self.paths.unet_weights, 'weights_initial.h5'))
-        elif step > 0:
-            self.unet_model.load_weights((os.path.join(self.paths.unet_weights, weights_name + f"step{step}.h5")))
-            self.unet_model.save(os.path.join(self.paths.unet_weights, "unet3_retrained.h5"))
-        else:
-            raise ValueError("step should be an interger >= 0")
-
-    def interpolate_seg(self):
-        """
-        Interpolate the images along z axis in volume 1 and save the results in "track_results_xxx" folder
-
-        Notes
-        -----
-        The image was interpolated and smoothed if z_scaling>1, or smoothed if z_scaling=1 by a Gaussian filter.
-        After interpolation/smoothing, the cell boundaries were reassigned by 2d watershed. Then the interpolated cells
-        were re-segmented by 3d connectivity to separate cells incorrectly labelled as the same cell.
-        """
-        # _interpolate layers in z axis
-        self.seg_cells_interpolated_corrected = self._interpolate()
-        self.Z_RANGE_INTERP = range(self.z_scaling // 2, self.seg_cells_interpolated_corrected.shape[2],
-                                    self.z_scaling)
-
-        # re-segmentation
-        self.seg_cells_interpolated_corrected = self._relabel_separated_cells(self.seg_cells_interpolated_corrected)
-        self.segmentation_manual_relabels = self.seg_cells_interpolated_corrected[:, :, self.Z_RANGE_INTERP]
-
-        # save labels in the first volume (interpolated)
-        save_img3ts(range(0, self.z_siz), self.segmentation_manual_relabels,
-                    self.paths.track_results + "track_results_t%04i_z%04i.tif", t=1, use_8_bit=self.use_8_bit)
-
-        # calculate coordinates of cell centers at t=1
-        center_points_t0 = snm.center_of_mass(self.segmentation_manual_relabels > 0,
-                                              self.segmentation_manual_relabels,
-                                              range(1, self.segmentation_manual_relabels.max() + 1))
-        r_coordinates_manual_vol1 = self._transform_layer_to_real(center_points_t0)
-        self.r_coordinates_tracked_t0 = r_coordinates_manual_vol1.copy()
-        self.cell_num_t0 = r_coordinates_manual_vol1.shape[0]
-
-    @staticmethod
-    def _relabel_separated_cells(seg_cells_interpolated):
-        """Relabel the separate cells that were incorrectly labeled as the same one"""
-        num_cells = np.size(np.unique(seg_cells_interpolated)) - 1
-        seg_cells_interpolated_corrected = label(seg_cells_interpolated, connectivity=3)
-        if num_cells != np.max(seg_cells_interpolated_corrected):
-            print(f"WARNING: {num_cells} cells were manually labeled while the program found "
-                  f"{np.max(seg_cells_interpolated_corrected)} separated cells and corrected it")
-        return seg_cells_interpolated_corrected
-
-    def _interpolate(self):
-        """Interpolate/smoothen a 3D image"""
-        seg_cells_interpolated, seg_cell_or_bg = gaussian_filter(
-            self.segmentation_manual_relabels, z_scaling=self.z_scaling, smooth_sigma=2.5)
-        seg_cells_interpolated_corrected = watershed_2d_markers(
-            seg_cells_interpolated, seg_cell_or_bg, z_range=self.z_siz * self.z_scaling + 10)
-        return seg_cells_interpolated_corrected[5:self.x_siz + 5,
-               5:self.y_siz + 5, 5:self.z_siz * self.z_scaling + 5]
-
-    def cal_subregions(self):
-        """
-        Calculate the subregions of cells and the padded images to accelerate the accurate correction in tracking.
-
-        See Also
-        --------
-        _transform_cells_quick
-        """
-        # Compute subregions of each cells for quick "accurate correction"
-        seg_16 = self.seg_cells_interpolated_corrected.astype("int16")
-
-        self.region_list, self.region_width, self.region_xyz_min = get_subregions(seg_16, seg_16.max())
-        self.pad_x, self.pad_y, self.pad_z = np.max(self.region_width, axis=0)
-        self.label_padding = np.pad(seg_16,
-                                    pad_width=((self.pad_x, self.pad_x),
-                                               (self.pad_y, self.pad_y),
-                                               (self.pad_z, self.pad_z)),
-                                    mode='constant') * 0
-
-    def _check_multicells(self):
-        """Test if there are multiple cells marked as a single region"""
-        for i, region in enumerate(self.region_list):
-            assert np.sum(np.unique(label(region))) == 1, f"more than one cell in region {i + 1}"
-
-    def load_ffn(self):
-        """Load the pre-trained FFN model"""
-        self.ffn_model = load_model(os.path.join(self.paths.models, self.paths.ffn_model_file))
-        print("Loaded the FFN model")
-
-    def initiate_tracking(self):
-        """
-        Initiate the lists to store the displacement/coordinates histories from volume 1 (t0)
-        """
-        self.cells_on_boundary = np.zeros(self.cell_num_t0).astype(int)
-        self.history.r_displacements = []
-        self.history.r_displacements.append(np.zeros((self.cell_num_t0, 3)))
-        self.history.r_segmented_coordinates = []
-        self.history.r_segmented_coordinates.append(self.r_coordinates_segment_t0)
-        self.history.r_tracked_coordinates = []
-        self.history.r_tracked_coordinates.append(self.r_coordinates_tracked_t0)
-        self.history.anim = []
-        print("Initiated coordinates for tracking (from vol 1)")
-
-    def match(self, target_volume, method="min_size"):
-        """
-        Match cells in volume 1 with the target_volume
-
-        Parameters
-        ----------
-        target_volume : int
-            The target volume to be matched
-        method : str
-            The method to segment cells.
-
-        Returns
-        -------
-        anim : matplotlib.animation.ArtistAnimation
-            The animation including each iteration of the FFN + PR-GLS predictions
-        [cells_on_boundary_local, target_volume, i_disp_from_vol1_updated, r_coor_predicted] : list
-            The matching results used to draw figures
-        """
-        # skip frames that cannot be tracked
-        if target_volume in self.miss_frame:
-            raise ValueError("target_volume is a miss_frame")
-
-        # generate automatic _segment in current volume
-        self.segresult.update_results(*self._segment(target_volume, method=method))
-
-        # track by fnn + prgls
-        r_coor_predicted, anim = self._predict_pos_once(source_volume=1, draw=True)
-
-        # boundary cells
-        cells_bd = self._get_cells_onBoundary(r_coor_predicted, self.ensemble)
-        cells_on_boundary_local = self.cells_on_boundary.copy()
-        cells_on_boundary_local[cells_bd] = 1
-
-        # accurate correction
-        _, i_disp_from_vol1_updated = \
-            self._accurate_correction(cells_on_boundary_local, r_coor_predicted)
-        print(f"Matching between vol 1 and vol {target_volume} was computed")
-        return anim, [cells_on_boundary_local, target_volume, i_disp_from_vol1_updated, r_coor_predicted]
-
-    def _accurate_correction(self, cells_on_boundary_local, r_coor_predicted):
-        """Correct center positions of cells based on the cell regions detected by unet and intensities in raw image"""
-        r_disp_from_vol1_updated = self.history.r_displacements[-1] + \
-                                   (r_coor_predicted - self.history.r_tracked_coordinates[-1])
-        i_disp_from_vol1_updated = self._transform_real_to_interpolated(r_disp_from_vol1_updated)
-        for i in range(REP_NUM_CORRECTION):
-            # update positions (from vol1) by correction
-            r_disp_from_vol1_updated, i_disp_from_vol1_updated, r_disp_correction = \
-                self._correction_once_interp(i_disp_from_vol1_updated, cells_on_boundary_local)
-
-            # stop the repetition if correction converged
-            stop_flag = self._evaluate_correction(r_disp_correction)
-            if i == REP_NUM_CORRECTION - 1 or stop_flag:
-                break
-        return r_disp_from_vol1_updated, i_disp_from_vol1_updated
-
-    def _predict_pos_once(self, source_volume, draw=False):
-        """
-        Predict cell coordinates using the transformation parameters in all repetitions
-            from fnn_prgls()
-        """
-        # fitting the parameters for transformation
-        C_t, BETA_t, coor_intermediate_list = self._fit_ffn_prgls(
-            REP_NUM_PRGLS, self.history.r_segmented_coordinates[source_volume - 1])
-
-        # Transform the coordinates
-        r_coordinates_predicted = self.history.r_tracked_coordinates[source_volume - 1].copy()
-
-        if draw:
-            ax, fig = self._subplots_ffnprgls_animation()
-            plt_objs = []
-            for i in range(len(C_t)):
-                r_coordinates_predicted, r_coordinates_predicted_pre = self._predict_one_rep(
-                    r_coordinates_predicted, coor_intermediate_list[i], BETA_t[i], C_t[i])
-                plt_obj = self._draw_transformation(
-                    ax, r_coordinates_predicted_pre, self.segresult.r_coordinates_segment,
-                    r_coordinates_predicted, layercoord=False)
-                plt_objs.append(plt_obj)
-            anim = animation.ArtistAnimation(fig, plt_objs, interval=200).to_jshtml()
-        else:
-            for i in range(len(C_t)):
-                r_coordinates_predicted, r_coordinates_predicted_pre = self._predict_one_rep(
-                    r_coordinates_predicted, coor_intermediate_list[i], BETA_t[i], C_t[i])
-            anim = None
-
-        return r_coordinates_predicted, anim
-
-    def _fit_ffn_prgls(self, rep, r_coordinates_segment_pre):
-        """
-        Appliy FFN + PR-GLS from t1 to t2 (multiple times) to get transformation parameters to predict cell coordinates
-
-        Parameters
-        ----------
-        rep : int
-            The number of repetitions of (FFN + max_iteration times of PR-GLS)
-        r_coordinates_segment_pre : numpy.ndarray
-            Coordinates of cells in previous volume. Shape: (cell_num, 3)
-
-        Returns
-        -------
-        C_t : list
-            List of C in each repetition (to predict the transformed coordinates)
-        BETA_t : list
-            List of the parameter beta used in each repetition (to predict coordinates)
-        coor_intermediate_list : list
-            List of the pre-transformed coordinates of automatically segmented cells in each repetition
-            (to predict coordinates)
-        """
-        corr_intermediate = r_coordinates_segment_pre.copy()
-        C_t = []
-        BETA_t = []
-        coor_intermediate_list = []
-        for i in range(rep):
-            coor_intermediate_list.append(corr_intermediate)
-            C, corr_intermediate = self._ffn_prgls_once(i, corr_intermediate)
-            C_t.append(C)
-            BETA_t.append(self.beta_tk * (0.8 ** i))
-        return C_t, BETA_t, coor_intermediate_list
-
-    def _ffn_prgls_once(self, i, r_coordinates_segment_pre):
-        """Apply one iteration of FFN + PR-GLS"""
-        init_match = initial_matching_quick(self.ffn_model, r_coordinates_segment_pre,
-                                            self.segresult.r_coordinates_segment, 20)
-        pre_transformation_pre = r_coordinates_segment_pre.copy()
-        P, r_coordinates_segment_post, C = pr_gls_quick(pre_transformation_pre,
-                                                        self.segresult.r_coordinates_segment,
-                                                        init_match,
-                                                        BETA=self.beta_tk * (0.8 ** i),
-                                                        max_iteration=self.max_iteration,
-                                                        LAMBDA=self.lambda_tk)
-        return C, r_coordinates_segment_post
-
-    def _predict_one_rep(self, r_coordinates_predicted_pre, coor_intermediate_list, BETA_t, C_t):
-        """
-        Predict cell coordinates using one set of the transformation parameters
-            from fnn_prgls()
-        Input:
-            r_coordinates_predicted_pre: the coordinates before transformation
-            coor_intermediate_list, BETA_t, C_t: one set of the transformation parameters
-        Return:
-            r_coordinates_predicted_post: the coordinates after transformation
-        """
-
-        length_auto_segmentation = np.size(coor_intermediate_list, axis=0)
-
-        r_coordinates_predicted_tile = np.tile(r_coordinates_predicted_pre, (length_auto_segmentation, 1, 1))
-        coor_intermediate_tile = np.tile(coor_intermediate_list, (self.cell_num_t0, 1, 1)).transpose((1, 0, 2))
-        Gram_matrix = np.exp(-np.sum(np.square(r_coordinates_predicted_tile - coor_intermediate_tile),
-                                     axis=2) / (2 * BETA_t * BETA_t))
-
-        r_coordinates_predicted_post = r_coordinates_predicted_pre + np.dot(C_t, Gram_matrix).T
-
-        return r_coordinates_predicted_post, r_coordinates_predicted_pre
-
-    def _get_cells_onBoundary(self, r_coordinates_prgls, ensemble):
-        """
-        Get cell near the boundary of the image
-        """
-        if ensemble:
-            boundary_xy = 0
-        else:
-            boundary_xy = BOUNDARY_XY
-        cells_bd = np.where(reduce(
-            np.logical_or,
-            [r_coordinates_prgls[:, 0] < boundary_xy,
-             r_coordinates_prgls[:, 1] < boundary_xy,
-             r_coordinates_prgls[:, 0] > self.x_siz - boundary_xy,
-             r_coordinates_prgls[:, 1] > self.y_siz - boundary_xy,
-             r_coordinates_prgls[:, 2] / self.z_xy_ratio < 0,
-             r_coordinates_prgls[:, 2] / self.z_xy_ratio > self.z_siz])
-        )
-        return cells_bd
-
-    def _correction_once_interp(self, i_displacement_from_vol1, cell_on_bound):
-        """
-        Correct the tracking for once (in interpolated image)
-        """
-        # generate current image of labels from the manually corrected _segment in volume 1
-        i_l_tracked_cells_prgls_0, i_l_overlap_prgls_0 = self._transform_cells_quick(i_displacement_from_vol1)
-        l_tracked_cells_prgls = i_l_tracked_cells_prgls_0[:, :,
-                                self.z_scaling // 2:self.z_siz * self.z_scaling:self.z_scaling]
-        l_overlap_prgls = i_l_overlap_prgls_0[:, :,
-                          self.z_scaling // 2:self.z_siz * self.z_scaling:self.z_scaling]
-
-        # overlapping regions of multiple cells are discarded before correction to avoid cells merging
-        l_tracked_cells_prgls[np.where(l_overlap_prgls > 1)] = 0
-
-        for i in np.where(cell_on_bound == 1)[0]:
-            l_tracked_cells_prgls[l_tracked_cells_prgls == (i + 1)] = 0
-
-        # accurate correction of displacement
-        l_coordinates_prgls_int_move = \
-            self.r_coordinates_tracked_t0 * np.array([1, 1, 1 / self.z_xy_ratio]) + \
-            i_displacement_from_vol1 * np.array([1, 1, 1 / self.z_scaling])
-        l_centers_unet_x_prgls = snm.center_of_mass(
-            self.segresult.image_cell_bg[0, :, :, :, 0] + self.segresult.image_gcn, l_tracked_cells_prgls,
-            range(1, self.seg_cells_interpolated_corrected.max() + 1))
-        l_centers_unet_x_prgls = np.asarray(l_centers_unet_x_prgls)
-        l_centers_prgls = np.asarray(l_coordinates_prgls_int_move)
-
-        lost_cells = np.where(np.isnan(l_centers_unet_x_prgls)[:, 0])
-
-        r_displacement_correction = l_centers_unet_x_prgls - l_centers_prgls
-        r_displacement_correction[lost_cells, :] = 0
-        r_displacement_correction[:, 2] = r_displacement_correction[:, 2] * self.z_xy_ratio
-
-        # calculate the corrected displacement from vol #1
-        r_displacement_from_vol1 = i_displacement_from_vol1 * np.array(
-            [1, 1, self.z_xy_ratio / self.z_scaling]) + r_displacement_correction
-        i_displacement_from_vol1_new = self._transform_real_to_interpolated(r_displacement_from_vol1)
-
-        return r_displacement_from_vol1, i_displacement_from_vol1_new, r_displacement_correction
-
-    def _transform_cells_quick(self, vectors3d):
-        """
-        Generate a image with labels indicating the moved cells.
-
-        Parameters
-        ----------
-        vectors3d : numpy.array
-            Movements of each cell
-
-        Returns
-        -------
-        output : numpy.ndarray
-            The new image with moved cells
-        mask : numpy.ndarray
-            The new image with the
-        """
-        label_moved = self.label_padding.copy()
-        mask = label_moved.copy()
-        for label in range(0, len(self.region_list)):
-            new_x_min = self.region_xyz_min[label][0] + vectors3d[label, 0] + self.pad_x
-            new_y_min = self.region_xyz_min[label][1] + vectors3d[label, 1] + self.pad_y
-            new_z_min = self.region_xyz_min[label][2] + vectors3d[label, 2] + self.pad_z
-            subregion_previous = label_moved[new_x_min:new_x_min + self.region_width[label][0],
-                                 new_y_min:new_y_min + self.region_width[label][1],
-                                 new_z_min:new_z_min + self.region_width[label][2]]
-            if subregion_previous.shape != self.region_list[label].shape:
-                continue
-            subregion_new = subregion_previous * (1 - self.region_list[label]) + \
-                            self.region_list[label] * (label + 1)
-            label_moved[new_x_min:new_x_min + self.region_width[label][0],
-            new_y_min:new_y_min + self.region_width[label][1],
-            new_z_min:new_z_min + self.region_width[label][2]] = subregion_new
-            mask[new_x_min:new_x_min + self.region_width[label][0],
-            new_y_min:new_y_min + self.region_width[label][1],
-            new_z_min:new_z_min + self.region_width[label][2]] += \
-                (self.region_list[label] > 0).astype("int8")
-        output = label_moved[self.pad_x:-self.pad_x, self.pad_y:-self.pad_y, self.pad_z:-self.pad_z]
-        mask = mask[self.pad_x:-self.pad_x, self.pad_y:-self.pad_y, self.pad_z:-self.pad_z]
-
-        return output, mask
-
-    def _transform_motion_to_image(self, cells_on_boundary_local, i_disp_from_vol1_updated):
-        """Transform the predicted movements to the moved labels in 3D image"""
-        i_tracked_cells_corrected, i_overlap_corrected = self._transform_cells_quick(i_disp_from_vol1_updated)
-        # re-calculate boundaries by _watershed
-        i_tracked_cells_corrected[i_overlap_corrected > 1] = 0
-        for i in np.where(cells_on_boundary_local == 1)[0]:
-            i_tracked_cells_corrected[i_tracked_cells_corrected == (i + 1)] = 0
-        tracked_labels = watershed_2d_markers(
-            i_tracked_cells_corrected[:, :, self.Z_RANGE_INTERP], i_overlap_corrected[:, :, self.Z_RANGE_INTERP],
-            z_range=self.z_siz)
-        return tracked_labels
-
-    def _evaluate_correction(self, r_displacement_correction):
-        """
-        evaluate if the accurate correction should be stopped
-        """
-        i_disp_test = r_displacement_correction.copy()
-        i_disp_test[:, 2] *= self.z_scaling / self.z_xy_ratio
-        if np.nanmax(np.abs(i_disp_test)) >= 0.5:
-            # print(np.nanmax(np.abs(i_disp_test)), end=",")
-            return False
-        else:
-            # print(np.nanmax(np.abs(i_disp_test)))
-            return True
-
-    def track(self, fig, ax, from_volume=2):
-        """
-        Track cells from a specific volume
-
-        Parameters
-        ----------
-        fig : matplotlib.figure.Figure
-            The figure to draw tracking results
-        ax : matplotlib.figure.Figure
-            The list of 6 subplots to draw tracking results
-        from_volume : int, optional
-            The volume from which to track the cells. Should be >= 2 and <= last tracked volume + 1. Default: 2
-        """
-        self._reset_tracking_state(from_volume)
-        for vol in range(from_volume, self.volume_num + 1):
-            self.track_one_vol(vol, fig, ax)
-        return None
-
-    def replay_track_animation(self, from_volume=2):
-        """
-        Replay the tracking animation based on the stored tracking process
-
-        Parameters
-        ----------
-        from_volume : int
-            The start volume to show the tracking process. Should be >= 2. Default: 2
-
-        Returns
-        -------
-        track_anim : matplotlib.animation.ArtistAnimation
-            The animation object to be showed
-        """
-        fig, ax = plt.subplots(figsize=(14, int(21 * self.x_siz / self.y_siz)), tight_layout=True)
-        plt.close(fig)
-        ax.axis('off')
-        track_process_images = []
-        for volume in range(from_volume, self.volume_num + 1):
-            try:
-                im = mgimg.imread(self.paths.anim + "track_anim_t%04i.png" % volume)
-            except FileNotFoundError:
-                continue
-            implot = ax.imshow(im)
-            track_process_images.append([implot])
-
-        track_anim = animation.ArtistAnimation(fig, track_process_images, interval=200, repeat=False).to_jshtml()
-        return track_anim
-
-    def _reset_tracking_state(self, from_volume):
-        """Remove the tracking history after a specific volume to re-track from this volume"""
-        assert from_volume >= 2, "from_volume should >= 2"
-        current_vol = len(self.history.r_displacements)
-        del self.history.r_displacements[from_volume - 1:]
-        del self.history.r_segmented_coordinates[from_volume - 1:]
-        del self.history.r_tracked_coordinates[from_volume - 1:]
-        assert len(self.history.r_displacements) == from_volume - 1, \
-            f"Currently data has been tracked until vol {current_vol}, the program cannot start from {from_volume}"
-        # print(f"Currently data has been tracked until vol {current_vol}, start from vol {from_volume}")
-
-    def track_one_vol(self, target_volume, fig, axc6, method="min_size"):
-        """
-        Track one volume of cells and update the coordinates information
-
-        Parameters
-        ----------
-        target_volume : int
-            The target volume to be tracked
-        fig : matplotlib.figure.Figure
-            A figure to draw the updated tracking results
-        axc6 : list of matplotlib.axes.Axes
-            A list of axes to draw each sub-figures of tracking results
-        method : str, optional
-            The method used in segmenting cells. Default: "min_size"
-        """
-        # skip frames that cannot be tracked
-        if target_volume in self.miss_frame:
-            save_img3ts(range(0, self.z_siz), self.tracked_labels,
-                        self.paths.track_results + "track_results_t%04i_z%04i.tif", target_volume, self.use_8_bit)
-            self.history.r_displacements.append(self.history.r_displacements[-1])
-            self.history.r_segmented_coordinates.append(self.segresult.r_coordinates_segment)
-            self.history.r_tracked_coordinates.append(
-                self.r_coordinates_tracked_t0 + self.history.r_displacements[-1])
-            return None
-
-        # make _segment of target volume
-        self.segresult.update_results(*self._segment(target_volume, method=method))
-
-        # FFN + PR-GLS predictions (single or ensemble)
-        source_vols_list = get_reference_vols(self.ensemble, target_volume, adjacent=self.adjacent)
-        list_predictions = []
-        for source_vol in source_vols_list:
-            r_coor_predicted, _ = self._predict_pos_once(source_volume=source_vol, draw=False)
-            list_predictions.append(r_coor_predicted)
-        r_coor_predicted_mean = trim_mean(list_predictions, 0.1, axis=0)
-
-        # remove cells moved to the boundaries of the 3D image
-        cells_bd = self._get_cells_onBoundary(r_coor_predicted_mean, self.ensemble)
-        self.cells_on_boundary[cells_bd] = 1
-
-        # accurate correction to get more accurate positions
-        r_disp_from_vol1_updated, i_disp_from_vol1_updated = \
-            self._accurate_correction(self.cells_on_boundary, r_coor_predicted_mean)
-
-        # transform positions into images
-        self.tracked_labels = self._transform_motion_to_image(self.cells_on_boundary, i_disp_from_vol1_updated)
-
-        # save tracked labels
-        save_img3ts(range(0, self.z_siz), self.tracked_labels,
-                    self.paths.track_results + "track_results_t%04i_z%04i.tif", target_volume, self.use_8_bit)
-
-        self._draw_matching_6panel(target_volume, axc6, r_coor_predicted_mean, i_disp_from_vol1_updated)
-        fig.canvas.draw()
-        plt.savefig(self.paths.anim + "track_anim_t%04i.png" % target_volume, bbox_inches='tight')
-
-        # update and save points locations
-        if self.ensemble:
-            self.cells_on_boundary = \
-                np.zeros(self.cell_num_t0).astype(int)  # in ensemble mode, cells on boundary are not deleted forever
-        self.history.r_displacements.append(r_disp_from_vol1_updated)
-        self.history.r_segmented_coordinates.append(self.segresult.r_coordinates_segment)
-        self.history.r_tracked_coordinates.append(self.r_coordinates_tracked_t0 + r_disp_from_vol1_updated)
-
-        return None
-
-    def save_coordinates(self):
-        """Save 3D coordinates in a csv file under the track_information folder
-
-        Notes
-        -----
-        x,y are coordinates with pixel unit, while z is the interpolated coordinate with the same unit as x and y
-        """
-        coord = np.asarray(self.history.r_tracked_coordinates)
-        t, cell, pos = coord.shape
-        coord_table = np.column_stack(
-            (np.repeat(np.arange(1, t + 1), cell), np.tile(np.arange(1, cell + 1), t), coord.reshape(t * cell, pos)))
-        np.savetxt(os.path.join(self.paths.track_information, "tracked_coordinates.csv"), coord_table, delimiter=',',
-                   header="cell,t,x(row),y(column),z(interpolated)", comments="")
-        print("Cell coordinates were stored in ./track_information/tracked_coordinates.csv")
+"""
+A module for tracking and monitoring the intermediate results
+Author: Chentao Wen
+
+Notes
+-----
+To describe the cell positions, 3 different coordinates are used
+    layer-based
+        Use \"l_\" prefix, corresponding to the positions in the raw image
+    interpolated-layer-based
+        Use "i_" prefix, corresponding to the positions in the interpolated image
+    real-resolution
+        Use "r_" prefix, the cell positions along z axis are transformed to correspond the resolution in x-y plane
+"""
+
+import os
+import time
+from functools import reduce
+from pathlib import Path
+
+import matplotlib as mpl
+import matplotlib.image as mgimg
+import numpy as np
+import scipy.ndimage.measurements as ndm
+from PIL import Image
+from numpy import ndarray
+from tensorflow.keras.models import load_model
+from tensorflow.keras.preprocessing.image import ImageDataGenerator
+from matplotlib import animation
+from matplotlib import pyplot as plt
+from scipy.stats import trim_mean
+from skimage.measure import label
+from skimage.segmentation import relabel_sequential, find_boundaries
+
+from .preprocess import _make_folder, _normalize_image, _normalize_label, load_image
+from .track import pr_gls_quick, initial_matching_quick, get_reference_vols, get_subregions, tracking_plot_xy, \
+    tracking_plot_zx, gaussian_filter
+from .unet3d import unet3_prediction, _divide_img, _augmentation_generator
+from .watershed import watershed_2d, watershed_3d, recalculate_cell_boundaries
+
+mpl.rcParams['image.interpolation'] = 'none'
+
+TITLE_STYLE = {'fontsize': 16, 'verticalalignment': 'bottom'}
+
+REP_NUM_PRGLS = 5
+REP_NUM_CORRECTION = 20
+BOUNDARY_XY = 6
+ALPHA_BLEND = 0.5
+
+
+def timer(func):
+    """A decorators to display runtime of a function"""
+
+    def wrapper_timer(*args, **kwargs):
+        tic = time.perf_counter()
+        value = func(*args, **kwargs)
+        toc = time.perf_counter()
+        elapsed_time = toc - tic
+        print(f"{func.__name__} took {elapsed_time:0.2f} seconds")
+        return value
+
+    return wrapper_timer
+
+
+def get_random_cmap(num, seed=1):
+    """
+    Generate a random cmap
+
+    Parameters
+    ----------
+    num : int
+        The number of colors to be generated
+    seed : int
+        The same value will lead to the same cmap
+
+    Returns
+    -------
+    cmap : matplotlib.colors.Colormap
+        The generated cmap
+    """
+    vals = np.linspace(0, 1, num + 1)
+    np.random.seed(seed)
+    np.random.shuffle(vals)
+    vals = np.concatenate(([0], vals[1:]))
+    cmap = plt.cm.colors.ListedColormap(plt.cm.rainbow(vals))
+    cmap.colors[0, :3] = 0
+    return cmap
+
+
+def get_tracking_path(adjacent, ensemble, folder_path):
+    """
+    Generate a path for storing tracking results according to tracking mode
+
+    Parameters
+    ----------
+    adjacent : bool
+    ensemble : bool or int
+    folder_path : str
+
+    Returns
+    -------
+    str
+        The generated path
+    """
+    if not ensemble:
+        return os.path.join(folder_path, "track_results_SingleMode/")
+    elif not adjacent:
+        return os.path.join(folder_path, "track_results_EnsembleDstrbtMode/")
+    else:
+        return os.path.join(folder_path, "track_results_EnsembleAdjctMode/")
+
+
+def read_image_ts(vol, path, name, z_range, print_=False):
+    """
+    Read a 3D image at time vol
+
+    Parameters
+    ----------
+    vol : int
+        A specific volume
+    path : str
+        Folder path
+    name : str
+        File name
+    z_range : tuple
+        Range of layers
+    print_ : bool
+        Whether print the image shape or not
+
+    Returns
+    -------
+    img_array : numpy.ndarray
+        An array of the image with shape (row, column, layer)
+    """
+    from tifffile import imread
+    image_raw = []
+    for z in range(z_range[0], z_range[1]):
+        image_raw.append(imread(path + name % (vol, z)))
+    img_array = np.array(image_raw).transpose((1, 2, 0))
+    if print_:
+        print("Load images with shape:", img_array.shape)
+    return img_array
+
+
+def save_automatic_segmentation(labels_xyz: ndarray, folder_path, use_8_bit: bool):
+    """
+    Save a 3D image (at t=1) as 2D image sequence
+
+    Parameters
+    ----------
+    z_siz : int
+        The layer number of the 3D image
+    labels_xyz : numpy.ndarray
+        The 3D image to be saved. Shape: (row, column, layer)
+    folder_path : str
+        The path of folder to save the results.
+    use_8_bit: bool
+        The array will be transformed to 8-bit or 16-bit before saving as image.
+    """
+    _seg_path = Path(folder_path)
+    _seg_path.mkdir(parents=True, exist_ok=True)
+    dtype = np.uint8 if use_8_bit else np.uint16
+    for z in range(1, labels_xyz.shape[2] + 1):
+        img2d = labels_xyz[:, :, z - 1].astype(dtype)
+        Image.fromarray(img2d).save(os.path.join(folder_path, "auto_vol1", "auto_vol1_z%04i.tif"%z))
+
+
+def save_img3ts(z_range, img, path, t, use_8_bit: bool=True):
+    """
+    Save a 3D image at time t as 2D image sequence
+    Parameters
+    ----------
+    z_range : range
+        The range of layers to be saved
+    img : numpy.array
+        The 3D image to be saved
+    path : str
+        The path of the image files to be saved.
+        It should use formatted string to indicate volume number and then layer number, e.g. "xxx_t%04d_z%04i.tif"
+    t : int
+        The volume number for the image to be saved
+    use_8_bit: bool
+        The array will be transformed to 8-bit or 16-bit before saving as image.
+    """
+    dtype = np.uint8 if use_8_bit else np.uint16
+    for i, z in enumerate(z_range):
+        img2d = (img[:, :, z]).astype(dtype)
+        Image.fromarray(img2d).save(path % (t, i + 1))
+
+
+class Draw:
+    """
+    Class for drawing figures. Only use its method through Tracker instances.
+    """
+
+    def __init__(self):
+        self.history.r_tracked_coordinates = None
+        self.r_coordinates_tracked_t0 = None
+        self.segresult = None
+        self.vol = None
+        self.x_siz = None
+        self.y_siz = None
+        self.z_siz = None
+        self.cell_num = None
+        self.seg_cells_interpolated_corrected = None
+        self.cell_num_t0 = None
+        self.z_scaling = None
+        self.z_xy_ratio = None
+        self.Z_RANGE_INTERP = None
+        self.tracked_labels = None
+
+    def draw_segresult(self, percentile_high=99.9):
+        """
+        Draw the raw image and the segmentation result in current volume by max-projection and return an animation
+        showing the 3D images as 2D image sequences
+
+        Parameters
+        ----------
+        percentile_high : float
+            A percentile value (0.0-100.0) as the upper limitation of the intensities when showing the raw image
+
+        Returns
+        -------
+        anim : matplotlib.animation.ArtistAnimation
+            The animation including each layer of the raw image and the segmentation results
+            
+        Notes
+        -----
+        The lower limitation of intensities for showing the raw image is set to lower 10% by default.
+        """
+        axs, figs = self._subplots_3()
+        axs[0].set_title(f"Raw image at vol {self.vol}", fontdict=TITLE_STYLE)
+        axs[1].set_title(f"Cell regions at vol {self.vol} by U-Net", fontdict=TITLE_STYLE)
+        axs[2].set_title(f"Auto-_segment at vol {self.vol}", fontdict=TITLE_STYLE)
+        anim_obj = []
+        vmax = np.percentile(self.segresult.image_gcn, percentile_high)
+        vmin = np.percentile(self.segresult.image_gcn, 10)
+        for z in range(self.z_siz):
+            obj1 = axs[0].imshow(self.segresult.image_gcn[:, :, z],
+                                 vmin=vmin, vmax=vmax, cmap="gray")
+            obj2 = axs[1].imshow(self.segresult.image_cell_bg[0, :, :, z, 0] > 0.5, cmap="gray")
+            obj3 = axs[2].imshow(self.segresult.segmentation_auto[:, :, z],
+                                 vmin=0, vmax=self.cell_num, cmap=get_random_cmap(num=self.cell_num))
+            anim_obj.append([obj1, obj2, obj3])
+        anim = animation.ArtistAnimation(figs, anim_obj, interval=200).to_jshtml()
+
+        axs[0].imshow(np.max(self.segresult.image_gcn, axis=2), vmin=vmin, vmax=vmax, cmap="gray")
+        axs[1].imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0] > 0.5, axis=2), cmap="gray")
+        axs[2].imshow(np.max(self.segresult.segmentation_auto, axis=2),
+                      cmap=get_random_cmap(num=self.cell_num))
+        print("Segmentation results (max projection):")
+        return anim
+
+    def draw_manual_seg1(self):
+        """
+        Draw the cell regions and the interpolated/smoothed manual segmentation with max-projection in volume 1
+        """
+        axm, figm = self._subplots_2_horizontal()
+        axm[0].imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=2) > 0.5, cmap="gray")
+        axm[0].set_title(f"Cell regions at vol {self.vol} by U-Net", fontdict=TITLE_STYLE)
+        axm[1].imshow(np.max(self.seg_cells_interpolated_corrected, axis=2),
+                      cmap=get_random_cmap(num=self.cell_num_t0))
+        axm[1].set_title(f"Manual _segment at vol 1", fontdict=TITLE_STYLE)
+
+    def _draw_transformation(self, ax, r_coordinates_predicted_pre, r_coordinates_segmented_post,
+                             r_coordinates_predicted_post, layercoord, draw_point=True):
+        """
+        Draw each iteration of the tracking by FFN + PR-GLS
+        """
+        element1 = tracking_plot_xy(
+            ax[0], r_coordinates_predicted_pre, r_coordinates_segmented_post, r_coordinates_predicted_post,
+            (self.y_siz, self.x_siz), draw_point, layercoord)
+        element2 = tracking_plot_zx(
+            ax[1], r_coordinates_predicted_pre, r_coordinates_segmented_post, r_coordinates_predicted_post,
+            (self.y_siz, self.z_siz), draw_point, layercoord)
+        if layercoord:
+            ax[0].set_aspect('equal', 'box')
+            ax[1].set_aspect('equal', 'box')
+        return element1 + element2
+
+    def draw_correction(self, i_disp_from_vol1_updated, r_coor_predicted):
+        """
+        Draw the accurate correction superimposed on the cell regions
+
+        Parameters
+        ----------
+        i_disp_from_vol1_updated : numpy.ndarray
+            The current displacement of each cell from volume 1. Interpolated coordinates.
+        r_coor_predicted : numpy.ndarray
+            The current coordinates of each cell. Real coordinates
+        """
+        ax, fig = self._subplots_2_horizontal()
+        ax[0].set_title("Accurate Correction (y-x plane)", size=16)
+        ax[1].set_title("Accurate Correction (y-z plane)", size=16)
+        self._draw_correction(ax, r_coor_predicted, i_disp_from_vol1_updated)
+        return None
+
+    def _draw_correction(self, ax, r_coor_predicted, i_disp_from_vol1_updated):
+        """
+        Draw the accurate correction of cell positions after FFN + PR-GLS transformation
+        """
+        _ = self._draw_transformation(
+            [ax[0], ax[1]],
+            self._transform_real_to_layer(r_coor_predicted),
+            self._transform_real_to_layer(self.segresult.r_coordinates_segment),
+            self._transform_real_to_layer(self.r_coordinates_tracked_t0) +
+            self._transform_interpolated_to_layer(i_disp_from_vol1_updated),
+            layercoord=True, draw_point=False)
+        ax[0].imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=2) > 0.5, cmap="gray",
+                     extent=(0, self.y_siz - 1, self.x_siz - 1, 0))
+        ax[1].imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=0).T > 0.5, aspect=self.z_xy_ratio,
+                     cmap="gray", extent=(0, self.y_siz - 1, self.z_siz - 1, 0))
+
+        return None
+
+    def draw_overlapping(self, cells_on_boundary_local, volume2, i_disp_from_vol1_updated):
+        """
+        Draw the overlapping of cell regions (gray) and the labels before/after matching
+
+        Parameters
+        ----------
+        cells_on_boundary_local : numpy.ndarray
+            A 1d array of cells on boundary (1, ignored in tracking) or not (0).
+        volume2 : int
+            The current volume
+        i_disp_from_vol1_updated : numpy.ndarray
+            The displacement of each cell from volume 1. Interpolated coordinates.
+        """
+        self.tracked_labels = self._transform_motion_to_image(cells_on_boundary_local, i_disp_from_vol1_updated)
+        self._draw_matching(volume2)
+        plt.pause(0.1)
+        return None
+
+    def _draw_matching(self, volume2):
+        """Draw the overlapping of cell and labels"""
+        axc, figc = self._subplots_4()
+        self._draw_before_matching(axc[0], axc[1], volume2)
+        self._draw_after_matching(axc[2], axc[3], volume2)
+        plt.tight_layout()
+        return None
+
+    def _draw_matching_6panel(self, target_volume, ax, r_coor_predicted_mean, i_disp_from_vol1_updated):
+        """Draw the tracking process in a specific volume"""
+        for ax_i in ax:
+            ax_i.cla()
+        plt.suptitle(f"Tracking results at vol {target_volume}", size=16)
+
+        _ = self._draw_transformation([ax[0], ax[1]], self.history.r_tracked_coordinates[target_volume - 2],
+                                      self.segresult.r_coordinates_segment, r_coor_predicted_mean, layercoord=False)
+        self._draw_correction([ax[2], ax[3]], r_coor_predicted_mean, i_disp_from_vol1_updated)
+        self._draw_after_matching(ax[4], ax[5], target_volume, legend=False)
+        self._set_layout_anim()
+        for axi in ax:
+            plt.setp(axi.get_xticklabels(), visible=False)
+            plt.setp(axi.get_yticklabels(), visible=False)
+            axi.tick_params(axis='both', which='both', length=0)
+            axi.axis("off")
+        return None
+
+    def _draw_before_matching(self, ax1, ax2, volume2):
+        """Draw overlapping of cells and labels before matching"""
+        ax1.imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=2) > 0.5, cmap="gray")
+        ax1.imshow(np.max(self.seg_cells_interpolated_corrected[:, :, self.Z_RANGE_INTERP], axis=2),
+                   cmap=get_random_cmap(num=self.cell_num_t0), alpha=ALPHA_BLEND)
+
+        ax2.imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=0).T > 0.5, aspect=self.z_xy_ratio,
+                   cmap="gray")
+        ax2.imshow(np.max(self.seg_cells_interpolated_corrected[:, :, self.Z_RANGE_INTERP], axis=0).T,
+                   cmap=get_random_cmap(num=self.cell_num_t0), aspect=self.z_xy_ratio, alpha=ALPHA_BLEND)
+        ax1.set_title(f"Before matching: Cells at vol {volume2} + Labels at vol {self.vol} (y-x plane)",
+                      fontdict=TITLE_STYLE)
+        ax2.set_title(f"Before matching (y-z plane)",
+                      fontdict=TITLE_STYLE)
+
+    def _draw_after_matching(self, ax1, ax2, volume2, legend=True):
+        """Draw overlapping of cells and labels after matching"""
+        ax1.imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=2) > 0.5, cmap="gray")
+        ax1.imshow(np.max(self.tracked_labels, axis=2),
+                   cmap=get_random_cmap(num=self.cell_num_t0), alpha=ALPHA_BLEND)
+
+        ax2.imshow(np.max(self.segresult.image_cell_bg[0, :, :, :, 0], axis=0).T > 0.5, aspect=self.z_xy_ratio,
+                   cmap="gray")
+        ax2.imshow(np.max(self.tracked_labels, axis=0).T, cmap=get_random_cmap(num=self.cell_num_t0),
+                   aspect=self.z_xy_ratio, alpha=ALPHA_BLEND)
+        if legend:
+            ax1.set_title(f"After matching: Cells at vol {volume2} + Labels at vol {volume2} (y-x plane)",
+                          fontdict=TITLE_STYLE)
+            ax2.set_title(f"After matching (y-z plane)",
+                          fontdict=TITLE_STYLE)
+        return None
+
+    def _subplots_ffnprgls_animation(self):
+        """Generate a figure to draw the FFN + PR-GLS transformation"""
+        ax, fig = self._subplots_2_horizontal()
+        ax[0].set_title("Matching by FFN + PR-GLS (y-x plane)", fontdict=TITLE_STYLE)
+        ax[1].set_title("Matching by FFN + PR-GLS (y-z plane)", fontdict=TITLE_STYLE)
+        plt.tight_layout()
+        plt.close(fig)
+        return ax, fig
+
+    def _subplots_2_horizontal(self):
+        """Generate 2 subplots aligned horizontally in a figure"""
+        fig, ax = plt.subplots(1, 2, figsize=(20, int(12 * self.x_siz / self.y_siz)))
+        plt.tight_layout()
+        return ax, fig
+
+    def _subplots_3(self):
+        """
+        Generate 3 subplots in a figure
+
+        Returns
+        -------
+        ax : list of matplotlib.axes.Axes
+            The subplots to show each panel
+        fig : matplotlib.figure.Figure
+            The figure to draw tracking process
+        """
+        fig = plt.figure(figsize=(20, int(24 * self.x_siz / self.y_siz)))
+        ax = plt.subplot(221), plt.subplot(222), plt.subplot(223)
+        plt.tight_layout()
+        return ax, fig
+
+    def _subplots_4(self):
+        """Generate a (2, 2) layout subplots in a figure"""
+        fig, axs = plt.subplots(2, 2, figsize=(20, int(24 * self.x_siz / self.y_siz)))
+        ax = axs[0, 0], axs[0, 1], axs[1, 0], axs[1, 1]
+        plt.tight_layout()
+        return ax, fig
+
+    def subplots_tracking(self):
+        """
+        Generate a (3, 2) layout subplots in a figure
+
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The figure to draw tracking process
+        ax : list of matplotlib.axes.Axes
+            The subplots to show each panel
+        """
+        fig, axs = plt.subplots(3, 2, figsize=(14, int(21 * self.x_siz / self.y_siz)))
+        ax = axs[0, 0], axs[0, 1], axs[1, 0], axs[1, 1], axs[2, 0], axs[2, 1]
+        return fig, ax
+
+    @staticmethod
+    def _set_layout_anim():
+        """set the layout to show the tracking process dynamically in the notebook backend"""
+        plt.tight_layout()
+        plt.subplots_adjust(right=0.9, bottom=0.1)
+
+    def _transform_interpolated_to_layer(self, i_disp_from_vol1_updated):
+        """Overridden in Tracker"""
+        raise NotImplementedError("Must override this method")
+
+    def _transform_motion_to_image(self, cells_on_boundary_local, i_disp_from_vol1_updated):
+        """Overridden in Tracker"""
+        raise NotImplementedError("Must override this method")
+
+    def _transform_real_to_layer(self, r_coor_predicted):
+        """Overridden in Tracker"""
+        raise NotImplementedError("Must override this method")
+
+
+class SegResults:
+    """
+    Class to store the segmentation result.
+
+    Attributes
+    ----------
+    image_cell_bg : numpy.ndarray
+        The cell/non-cell predictions by 3D U-Net
+    l_center_coordinates : list of tuple
+        The detected centers coordinates of the cells, using voxels as the unit
+    segmentation_auto : numpy.ndarray
+        The individual cells predicted by 3D U-Net + watershed
+    image_gcn : numpy.ndarray
+        The raw image divided by 65535
+    r_coordinates_segment : numpy.ndarray
+        Transformed from l_center_coordinates, with the z coordinates corrected by the resolution relative to x-y plane
+    """
+
+    def __init__(self):
+        self.image_cell_bg = None
+        self.l_center_coordinates = None
+        self.segmentation_auto = None
+        self.image_gcn = None
+        self.r_coordinates_segment = None
+
+    def update_results(self, image_cell_bg, l_center_coordinates, segmentation_auto,
+                       image_gcn, r_coordinates_segment):
+        """Update the attributes of a SegResults instance"""
+        self.image_cell_bg = image_cell_bg
+        self.l_center_coordinates = l_center_coordinates
+        self.segmentation_auto = segmentation_auto
+        self.image_gcn = image_gcn
+        self.r_coordinates_segment = r_coordinates_segment
+
+
+class Segmentation:
+    """
+    Class for segmentation. Only use it through the Tracker instance.
+    """
+
+    def __init__(self, volume_num, siz_xyz: tuple, z_xy_ratio, z_scaling, shrink):
+        self.volume_num = volume_num
+        self.x_siz = siz_xyz[0]
+        self.y_siz = siz_xyz[1]
+        self.z_siz = siz_xyz[2]
+        self.z_xy_ratio = z_xy_ratio
+        self.z_scaling = z_scaling
+        self.shrink = shrink
+        self.noise_level = None
+        self.min_size = None
+        self.vol = None
+        self.paths = None
+        self.unet_model = None
+        self.r_coordinates_segment_t0 = None
+        self.segresult = SegResults()
+
+    def set_segmentation(self, noise_level=None, min_size=None, del_cache=False):
+        """
+        Set the segmentation parameters
+        If parameters changed or if reset_=True, delete cached segmentation.
+        
+        Parameters
+        ----------
+        noise_level : float, optional
+            Modify the attribute "noise_level" to this value. If None, no modification occur. Default: None
+        min_size : int, optional
+            Modify the attribute "min_size" to this value. If None, no modification occur. Default: None
+        del_cache : bool, optional
+            If True, delete all cached segmentation files under "/unet" folder. Default: False 
+        """
+        if self.noise_level == noise_level and self.min_size == min_size:
+            print("Segmentation parameters were not modified")
+        elif noise_level == None and min_size == None:
+            print("Segmentation parameters were not modified")
+        else:
+            if noise_level is not None:
+                self.noise_level = noise_level
+            if min_size is not None:
+                self.min_size = min_size
+            print(f"Parameters were modified: noise_level={self.noise_level}, min_size={self.min_size}")
+            for f in os.listdir(self.paths.unet_cache):
+                os.remove(os.path.join(self.paths.unet_cache, f))
+            print(f"All files under /unet folder were deleted")
+        if del_cache:
+            for f in os.listdir(self.paths.unet_cache):
+                os.remove(os.path.join(self.paths.unet_cache, f))
+            print(f"All files under /unet folder were deleted")
+
+    @staticmethod
+    def _transform_disps(disp, factor):
+        """Transform the coordinates with different units along z"""
+        new_disp = np.array(disp).copy()
+        new_disp[:, 2] = new_disp[:, 2] * factor
+        return new_disp
+
+    def _transform_layer_to_real(self, voxel_disp):
+        """Transform the coordinates from layer to real"""
+        return self._transform_disps(voxel_disp, self.z_xy_ratio)
+
+    def _transform_real_to_interpolated(self, r_disp):
+        """Transform the coordinates from real to interpolated"""
+        return np.rint(self._transform_disps(r_disp, self.z_scaling / self.z_xy_ratio)).astype(int)
+
+    def _transform_real_to_layer(self, r_disp):
+        """Transform the coordinates from real to layer"""
+        return np.rint(self._transform_disps(r_disp, 1 / self.z_xy_ratio)).astype(int)
+
+    def _transform_interpolated_to_layer(self, r_disp):
+        """Transform the coordinates from real to layer"""
+        return np.rint(self._transform_disps(r_disp, 1 / self.z_scaling)).astype(int)
+
+    def load_unet(self):
+        """
+        Load the pretrained unet model (keras Model file like "xxx.h5") and save its weights for retraining
+        """
+        self.unet_model = load_model(os.path.join(self.paths.models, self.paths.unet_model_file))
+        self.unet_model.save_weights(os.path.join(self.paths.unet_weights, 'weights_initial.h5'))
+        print("Loaded the 3D U-Net model")
+
+    def segment_vol1(self, method="min_size"):
+        """
+        Segment the volume 1 of the 3D time lapse image and save the segmentation result into "/auto_vol1" folder
+
+        Parameters
+        ----------
+        method : str
+            The method to remove the small regions in watershed. If "min_size", remove cells whose size is smaller than
+            this value. If "cell_num", sort the cells by their sizes and only keep the top "self.cell_num" cells.
+            Default: "min_size"
+
+        """
+        self.vol = 1
+        self.segresult.update_results(*self._segment(self.vol, method=method, print_shape=True))
+        self.r_coordinates_segment_t0 = self.segresult.r_coordinates_segment.copy()
+        use_8_bit = True if self.segresult.segmentation_auto.max() <= 255 else False
+
+        # save the segmented cells of volume #1
+        save_automatic_segmentation(labels_xyz=self.segresult.segmentation_auto,
+                                    folder_path=self.paths.folder, use_8_bit=use_8_bit)
+        print(f"Segmented volume 1 and saved it")
+
+    def _segment(self, vol, method, print_shape=False):
+        """
+        Segment cells from one volume of 3D image
+
+        Parameters
+        ----------
+        vol : int
+            A specific volume
+        method : str
+            "min_size" or "cell_num" used in watershed
+        print_shape : bool
+            If True, print the shape of the raw 3D image
+
+        Returns
+        -------
+        image_cell_bg : numpy.ndarray
+            The cell/non-cell predictions by 3D U-Net
+        l_center_coordinates : list of tuple
+            The detected centers coordinates of the cells, using voxels as the unit
+        segmentation_auto : numpy.ndarray
+            The individual cells predicted by 3D U-Net + watershed
+        image_gcn : numpy.ndarray
+            The raw image divided by 65535
+        r_coordinates_segment : numpy.ndarray
+            Transformed from l_center_coordinates, with the z coordinates corrected by the resolution relative to x-y
+            plane
+        """
+        image_raw = read_image_ts(vol, self.paths.raw_image, self.paths.image_name, (1, self.z_siz + 1),
+                                  print_=print_shape)
+        # image_gcn will be used to correct tracking results
+        image_gcn = (image_raw.copy() / 65536.0)
+        image_cell_bg = self._predict_cellregions(image_raw, vol)
+        if np.max(image_cell_bg) <= 0.5:
+            raise ValueError("No cell was detected by 3D U-Net! Try to reduce the noise_level.")
+
+        # segment connected cell-like regions using _watershed
+        segmentation_auto = self._watershed(image_cell_bg, method)
+        if np.max(segmentation_auto) == 0:
+            raise ValueError("No cell was detected by watershed! Try to reduce the min_size.")
+
+        # calculate coordinates of the centers of each segmented cell
+        l_center_coordinates = ndm.center_of_mass(segmentation_auto > 0, segmentation_auto,
+                                                  range(1, segmentation_auto.max() + 1))
+        r_coordinates_segment = self._transform_layer_to_real(l_center_coordinates)
+
+        return image_cell_bg, l_center_coordinates, segmentation_auto, image_gcn, r_coordinates_segment
+
+    def _predict_cellregions(self, image_raw, vol):
+        """
+        Predict cell regions by 3D U-Net and save it if the prediction has not been cached
+        """
+        try:
+            image_cell_bg = np.load(self.paths.unet_cache + "t%04i.npy" % vol, allow_pickle=True)
+        except OSError:
+            image_cell_bg = self._save_unet_regions(image_raw, vol)
+        return image_cell_bg
+
+    def _save_unet_regions(self, image_raw, vol):
+        """Predict the cell regions by 3D U-Net and cache the prediction"""
+        # pre-processing: local contrast normalization
+        image_norm = np.expand_dims(_normalize_image(image_raw, self.noise_level), axis=(0, 4))
+        # predict cell-like regions using 3D U-net
+        image_cell_bg = unet3_prediction(image_norm, self.unet_model, shrink=self.shrink)
+        np.save(self.paths.unet_cache + "t%04i.npy" % vol, np.array(image_cell_bg, dtype="float16"))
+        return image_cell_bg
+
+    def _watershed(self, image_cell_bg, method):
+        """
+        Segment the cell regions by watershed method
+        """
+        image_watershed2d_wo_border, _ = watershed_2d(image_cell_bg[0, :, :, :, 0], z_range=self.z_siz,
+                                                      min_distance=7)
+        _, image_watershed3d_wi_border, min_size, cell_num = watershed_3d(
+            image_watershed2d_wo_border, samplingrate=[1, 1, self.z_xy_ratio], method=method,
+            min_size=self.min_size, cell_num=self.cell_num, min_distance=3)
+        segmentation_auto, fw, inv = relabel_sequential(image_watershed3d_wi_border)
+        self.min_size = min_size
+        if method == "min_size":
+            self.cell_num = cell_num
+        return segmentation_auto
+
+
+class Paths:
+    """
+    Paths for storing data and results used by Tracker instance
+
+    Attributes
+    ----------
+    folder_path : str
+        The path of the folder to store all related data
+        including images, 3D U-Net, FFN models and segmentation/tracking results.
+    models : str
+        The path of the folder to store the pretrained and retrained models
+    unet_cache : str
+        The path of the folder to store the cached cell regions (predicted by 3D U-Net) to accelerate the tracking
+    raw_image : str
+        The path of the folder to store the raw images to be tracked
+    auto_segmentation_vol1 : str
+        The path of the folder to store the automatic segmentation in volume 1 to be used in manual correction
+    manual_segmentation_vol1 : str
+        The path of the folder to store the manually corrected segmentation in volume 1
+    unet_weights : str
+        The path of the folder to store the retrained weights of 3D U-Net
+    track_results :
+        The path of the folder to store the tracking results (in images with labels)
+    track_information : str
+        The path of the folder to store the displacements, coordinates information of segmented and tracked cells
+    anim : str
+        The path of the folder to store the animation of tracking in each volume
+    image_name : str
+        The file names of the raw image files.
+        It should use formatted string to indicate volume number and then layer number, e.g. "xxx_t%04d_z%04i.tif"
+    unet_model_file : str
+        The filename of the pretrained 3D U-Net (keras model such as "xxx.h5")
+    ffn_model_file : str
+        The filename of the pretrained FFN model (keras model such as "xxx.h5")
+    """
+
+    def __init__(self, folder_path, image_name, unet_model_file, ffn_model_file):
+        self.folder = folder_path
+        self.models = None
+        self.unet_cache = None
+        self.raw_image = None
+        self.auto_segmentation_vol1 = None
+        self.manual_segmentation_vol1 = None
+        self.unet_weights = None
+        self.track_results = None
+        self.track_information = None
+        self.anim = None
+        self.image_name = image_name
+        self.unet_model_file = unet_model_file
+        self.ffn_model_file = ffn_model_file
+
+    def make_folders(self, adjacent, ensemble):
+        """
+        Make folders for storing data, models, and results
+        """
+        print("Following folders were made under:", os.getcwd())
+        folder_path = self.folder
+        self.raw_image = _make_folder(os.path.join(folder_path, "data/"))
+        self.auto_segmentation_vol1 = _make_folder(os.path.join(folder_path, "auto_vol1/"))
+        self.manual_segmentation_vol1 = _make_folder(os.path.join(folder_path, "manual_vol1/"))
+        self.track_information = _make_folder(os.path.join(folder_path, "track_information/"))
+        self.models = _make_folder(os.path.join(folder_path, "models/"))
+        self.unet_cache = _make_folder(os.path.join(folder_path, "unet_cache/"))
+        track_results_path = get_tracking_path(adjacent, ensemble, folder_path)
+        self.track_results = _make_folder(track_results_path)
+        self.anim = _make_folder(os.path.join(folder_path, "anim/"))
+        self.unet_weights = _make_folder(os.path.join(self.models, "unet_weights/"))
+
+
+class History:
+    """
+    Storing the tracking histories
+
+    Attributes
+    ----------
+    r_displacements :  list of numpy.ndarray
+        The displacements of each cell in each volume relative to their positions in volume 1. Shape: (cell_num, 3)
+    r_segmented_coordinates : list of numpy.ndarray
+        The positions of each cell segmented by 3D U-Net + watershed in each volume. Shape: (cell_num, 3)
+    r_tracked_coordinates : list of numpy.ndarray
+        The positions of each cell tracked by FFN + PR-GLS + corrections in each volume. Shape: (cell_num, 3)
+    anim : list
+        The images of tracking process in each volume (from volume 2)
+    """
+
+    def __init__(self):
+        self.r_displacements = []
+        self.r_segmented_coordinates = []
+        self.r_tracked_coordinates = []
+        self.anim = []
+
+
+class Tracker(Segmentation, Draw):
+    """
+    Data and methods for tracking cells
+
+    Attributes
+    ----------
+    volume_num :  int
+        The number of volumes (time points) of the 3D + T image to be tracked
+    x_siz : int
+    y_siz : int
+    z_siz : int
+        Size of each 3D image. Obtained from the siz_xyz parameter (tuple) with (x_siz:Height, y_siz:Width, z_siz:Depth)
+    z_xy_ratio : float
+        The resolution (length per voxels) ratio between the z axis and the x-y plane, used in tracking.
+        Does not need to very precise
+    z_scaling : int
+        An integer (>= 1) for interpolating/smoothing images along z direction.
+        z_scaling = 1 makes no interpolation but only smoothing.
+    noise_level : float
+        A threshold to discriminate noise/artifacts from cell regions, used in preprocess._normalize_image function
+    min_size : int
+        A threshold of the minimum cell size (unit: voxels) to remove tiny regions that may be non-cell objects,
+        used in watershed.watershed_3d function
+    beta_tk : float
+        Control coherence by a weighted average of movements from neighbouring cells.
+        A larger BETA will include more cells and thus generates more coherent movements.
+    lambda_tk : float
+        Control coherence by applying a penalty for the incoherence of cell movements.
+        A large LAMBDA will generates more coherent movements.
+    maxiter_tk : int
+        The maximum number of iterations of PR-GLS during once application of FFN + PR-GLS.
+        A large values will generate more accurate tracking but will also increase the runtime.
+    cell_num : int
+        The number of cells to be extracted from watershed. It is used only when segmentation method is "cell_num".
+        Default: 0
+    ensemble : bool or int, optional
+        If False, track cells in single mode. If an integer, track cells in ensemble mode.
+        The integer indicates number of predictions to be averaged. Default: False
+    adjacent : bool, optional
+        Only used in ensemble mode. If True, make predictions of cell positions at t from
+        adjacent previous volumes such as t-1, t-2, t-3,..., t-10 (when ensemble=10).
+        If False, make prediction from distributed previous volumes. For example, predict cells at t=101 from
+        t = 1, 11, 21, ..., 91 (when ensemble=10). Default: False
+    shrink : tuple, optional
+        For padding the images before applying U-Net and for shrinking the cell prediction in the center part
+        of the U-Net output. Each value should be < (x, y, or z size of the U-Net input // 2), Default: (24, 24, 2)
+    miss_frame : list, optional
+        A list of volumes (int) which includes serious problem in the raw images and thus will be skipped for tracking.
+        Default: None
+    cell_num_t0 : int
+        The detected cell numbers in the manually corrected segmentation in volume 1
+    Z_RANGE_INTERP : Range object
+        The sequence of the indexes along z axis in the interpolated image corresponding to the layers in the raw image
+    region_list : list
+        List of the 3D sub-images [array_cell1, array_cell2, ...] with binary values
+        (1: this cell; 0: background or other cells)
+    region_width : list
+        List of the width of [[x_width, y_width, z_width]_cell1, ...] each sub-image in x, y, and z axis
+    region_xyz_min : list
+        List of the minimum coordinates [[x_min, y_min, z_min]_cell1, ...] of each sub-image in the raw image
+    pad_x : int
+    pad_y : int
+    pad_z : int
+        The values for padding a zero array with the raw image size
+    label_padding : numpy.ndarray
+        A 3D array with zero values, used in accurate correction during tracking.
+        Shape: (row + 2 * pad_x, column + 2 * pad_y, layer + 2 * pad_z)
+    segmentation_manual_relabels : numpy.ndarray
+        The relabeled manual segmentation. Shape: (row, column, layer)
+    segresult : SegResults object
+        The results of the segmentation in current volume
+    unet_model : keras.Model
+        The pretrained/retrained 3D U-Net model
+    """
+
+    def __init__(self,
+                 volume_num, siz_xyz: tuple, z_xy_ratio, z_scaling, noise_level, min_size, beta_tk,
+                 lambda_tk, maxiter_tk, folder_path, image_name, unet_model_file,
+                 ffn_model_file, cell_num=0, ensemble=False, adjacent=False,
+                 shrink=(24, 24, 2), miss_frame=None
+                 ):
+        Segmentation.__init__(self, volume_num, siz_xyz, z_xy_ratio, z_scaling, shrink)
+
+        self.miss_frame = [] if not miss_frame else miss_frame
+        self.noise_level = noise_level
+        self.min_size = min_size
+        self.beta_tk = beta_tk
+        self.lambda_tk = lambda_tk
+        self.max_iteration = maxiter_tk
+        self.ensemble = ensemble
+        self.adjacent = adjacent
+        self.cell_num = cell_num
+        self.cell_num_t0 = None
+        self.Z_RANGE_INTERP = None
+        self.region_list = None
+        self.region_width = None
+        self.region_xyz_min = None
+        self.pad_x = None
+        self.pad_y = None
+        self.pad_z = None
+        self.label_padding = None
+        self.segmentation_manual_relabels = None
+        self.cells_on_boundary = None
+        self.ffn_model = None
+        self.val_losses = None
+        self.paths = Paths(folder_path, image_name, unet_model_file, ffn_model_file)
+        self.history = History()
+        self.paths.make_folders(adjacent, ensemble)
+        self.use_8_bit = True
+
+    def set_tracking(self, beta_tk, lambda_tk, maxiter_tk):
+        """
+        Set tracking parameters
+
+        Parameters
+        ----------
+        beta_tk : float
+        lambda_tk : float
+        maxiter_tk : int
+        """
+        if self.beta_tk == beta_tk and self.lambda_tk == lambda_tk and self.max_iteration == maxiter_tk:
+            print("Tracking parameters were not modified")
+        else:
+            self.beta_tk = beta_tk
+            self.lambda_tk = lambda_tk
+            self.max_iteration = maxiter_tk
+            print(f"Parameters were modified: beta_tk={self.beta_tk}, "
+                  f"lambda_tk={self.lambda_tk}, maxiter_tk={self.max_iteration}")
+
+    def load_manual_seg(self):
+        """
+        Load the manually corrected segmentation in the "/manual_vol1" folder
+
+        Notes
+        -----
+        The files to be loaded in "manual_vol1" folder should be 2D images corresponding to cell labels in
+        each layer of the 3D image in volume 1
+        """
+        segmentation_manual = load_image(self.paths.manual_segmentation_vol1, print_=False)
+        print("Loaded manual _segment at vol 1")
+        self.segmentation_manual_relabels, _, _ = relabel_sequential(segmentation_manual)
+        if self.segmentation_manual_relabels.max() > 255:
+            self.use_8_bit = False
+
+    def _retrain_preprocess(self):
+        """
+        Prepare the training data for retraining the unet model
+        """
+        self.image_raw_vol1 = read_image_ts(1, self.paths.raw_image, self.paths.image_name, (1, self.z_siz + 1))
+        self.train_image_norm = _normalize_image(self.image_raw_vol1, self.noise_level)
+        self.label_vol1 = self._remove_2d_boundary(self.segmentation_manual_relabels) > 0
+        self.train_label_norm = _normalize_label(self.label_vol1)
+        print("Images were normalized")
+
+        self.train_subimage = _divide_img(self.train_image_norm, self.unet_model.input_shape[1:4])
+        self.train_subcells = _divide_img(self.train_label_norm, self.unet_model.input_shape[1:4])
+        print("Images were divided")
+
+        image_gen = ImageDataGenerator(rotation_range=90, width_shift_range=0.2, height_shift_range=0.2,
+                                       shear_range=0.2, horizontal_flip=True, fill_mode='reflect')
+
+        self.train_generator = _augmentation_generator(self.train_subimage, self.train_subcells, image_gen, batch_siz=8)
+        self.valid_data = (self.train_subimage, self.train_subcells)
+        print("Data for training 3D U-Net were prepared")
+
+    def _remove_2d_boundary(self, labels3d):
+        """
+        Remove boundaries between touching cells in x-y plane
+
+        Parameters
+        ----------
+        labels3d : numpy.ndarray
+            The 3D image of cell labels
+
+        Returns
+        -------
+        labels_new : numpy.ndarray
+            The new image with the boundaries removed
+        """
+        labels_new = labels3d.copy()
+        for z in range(self.z_siz):
+            labels = labels_new[:, :, z]
+            labels[find_boundaries(labels, mode='outer') == 1] = 0
+        return labels_new
+
+    def retrain_unet(self, iteration=10, weights_name="unet_weights_retrain_"):
+        """
+        Retrain the pretrained self.unet_model using the manually corrected segmentation in volume 1. Here the training
+        data are the randomly augmented sub-images from vol 1 data while the validation data are from the same vol but
+        without augmentation. The ground truth and the updated predictions are displayed after each epoch when the
+        val_loss was reduced.
+
+        Parameters
+        ----------
+        iteration : int, optional
+            The number of epochs to train the unet_model. Default: 10
+        weights_name : str, optional
+            The filename of the unet weights to be saved. Default: "unet_weights_retrain_"
+
+        Notes
+        -----
+        The boundaries (on x-y planes) between touching cells in the manual segmentation are removed to force the model
+        to predict boundaries as non-cell regions.
+
+        See Also
+        --------
+        _retrain_preprocess :  Preprocess of the training data
+        _remove_2d_boundary : Remove the boundaries between cells
+        """
+        self._retrain_preprocess()
+
+        self.unet_model.compile(loss='binary_crossentropy', optimizer="adam")
+        self.unet_model.load_weights(os.path.join(self.paths.unet_weights, 'weights_initial.h5'))
+
+        # evaluate model prediction before retraining
+        val_loss = self.unet_model.evaluate(self.train_subimage, self.train_subcells)
+        print("val_loss before retraining: ", val_loss)
+        self.val_losses = [val_loss]
+        self._draw_retrain(step="before retrain")
+
+        for step in range(1, iteration + 1):
+            self.unet_model.fit_generator(self.train_generator, validation_data=self.valid_data, epochs=1,
+                                          steps_per_epoch=60)
+            loss = self.unet_model.history.history["val_loss"][-1]
+            if loss < min(self.val_losses):
+                print("val_loss updated from ", min(self.val_losses), " to ", loss)
+                self.unet_model.save_weights(os.path.join(self.paths.unet_weights, weights_name + f"step{step}.h5"))
+                self._draw_retrain(step)
+            self.val_losses.append(loss)
+
+    def _draw_retrain(self, step):
+        """Draw the ground truth and the updated predictions during retraining the unet"""
+        train_prediction = np.squeeze(
+            unet3_prediction(np.expand_dims(self.train_image_norm, axis=(0, 4)), self.unet_model))
+        fig, axs = plt.subplots(1, 2, figsize=(20, int(12 * self.x_siz / self.y_siz)))
+        axs[0].imshow(np.max(self.label_vol1, axis=2), cmap="gray")
+        axs[1].imshow(np.max(train_prediction, axis=2) > 0.5, cmap="gray")
+        axs[0].set_title("Cell regions from manual segmentation at vol 1", fontdict=TITLE_STYLE)
+        axs[1].set_title(f"Cell prediction at step {step} at vol 1", fontdict=TITLE_STYLE)
+        plt.tight_layout()
+        plt.pause(0.1)
+
+    def select_unet_weights(self, step, weights_name="unet_weights_retrain_"):
+        """
+        Select a satisfied unet weights to restore it.
+
+        Parameters
+        ----------
+        step : int
+            The step with a satisfied prediction of cell regions in the trained image. If step=0, the initial weights
+            before retraining will be restored.
+        weights_name : str, optional
+            The filename of the unet weights to be saved. Default: "unet_weights_retrain_"
+
+        Raises
+        ------
+        ValueError
+            If step < 0
+        """
+        if step == 0:
+            self.unet_model.load_weights(os.path.join(self.paths.unet_weights, 'weights_initial.h5'))
+        elif step > 0:
+            self.unet_model.load_weights((os.path.join(self.paths.unet_weights, weights_name + f"step{step}.h5")))
+            self.unet_model.save(os.path.join(self.paths.unet_weights, "unet3_retrained.h5"))
+        else:
+            raise ValueError("step should be an interger >= 0")
+
+    def interpolate_seg(self):
+        """
+        Interpolate the images along z axis in volume 1 and save the results in "track_results_xxx" folder
+
+        Notes
+        -----
+        The image was interpolated and smoothed if z_scaling>1, or smoothed if z_scaling=1 by a Gaussian filter.
+        After interpolation/smoothing, the cell boundaries were reassigned by 2d watershed. Then the interpolated cells
+        were re-segmented by 3d connectivity to separate cells incorrectly labelled as the same cell.
+        """
+        # _interpolate layers in z axis
+        self.seg_cells_interpolated_corrected = self._interpolate()
+        self.Z_RANGE_INTERP = range(self.z_scaling // 2, self.seg_cells_interpolated_corrected.shape[2],
+                                    self.z_scaling)
+
+        # re-segmentation
+        self.seg_cells_interpolated_corrected = self._relabel_separated_cells(self.seg_cells_interpolated_corrected)
+        self.segmentation_manual_relabels = self.seg_cells_interpolated_corrected[:, :, self.Z_RANGE_INTERP]
+
+        # save labels in the first volume (interpolated)
+        save_img3ts(range(0, self.z_siz), self.segmentation_manual_relabels,
+                    self.paths.track_results + "track_results_t%04i_z%04i.tif", t=1, use_8_bit=self.use_8_bit)
+
+        # calculate coordinates of cell centers at t=1
+        center_points_t0 = ndm.center_of_mass(self.segmentation_manual_relabels > 0,
+                                              self.segmentation_manual_relabels,
+                                              range(1, self.segmentation_manual_relabels.max() + 1))
+        r_coordinates_manual_vol1 = self._transform_layer_to_real(center_points_t0)
+        self.r_coordinates_tracked_t0 = r_coordinates_manual_vol1.copy()
+        self.cell_num_t0 = r_coordinates_manual_vol1.shape[0]
+
+    @staticmethod
+    def _relabel_separated_cells(seg_cells_interpolated):
+        """Relabel the separate cells that were incorrectly labeled as the same one"""
+        num_cells = np.size(np.unique(seg_cells_interpolated)) - 1
+        seg_cells_interpolated_corrected = label(seg_cells_interpolated, connectivity=3)
+        if num_cells != np.max(seg_cells_interpolated_corrected):
+            print(f"WARNING: {num_cells} cells were manually labeled while the program found "
+                  f"{np.max(seg_cells_interpolated_corrected)} separated cells and corrected it")
+        return seg_cells_interpolated_corrected
+
+    def _interpolate(self):
+        """Interpolate/smoothen a 3D image"""
+        seg_cells_interpolated, seg_cell_or_bg = gaussian_filter(
+            self.segmentation_manual_relabels, z_scaling=self.z_scaling, smooth_sigma=2.5)
+        seg_cells_interpolated_corrected = recalculate_cell_boundaries(seg_cells_interpolated, seg_cell_or_bg)
+        return seg_cells_interpolated_corrected[5:self.x_siz + 5,
+               5:self.y_siz + 5, 5:self.z_siz * self.z_scaling + 5]
+
+    def cal_subregions(self):
+        """
+        Calculate the subregions of cells and the padded images to accelerate the accurate correction in tracking.
+
+        See Also
+        --------
+        _transform_cells_quick
+        """
+        # Compute subregions of each cells for quick "accurate correction"
+        seg_16 = self.seg_cells_interpolated_corrected.astype("int16")
+
+        self.region_list, self.region_width, self.region_xyz_min = get_subregions(seg_16, seg_16.max())
+        self.pad_x, self.pad_y, self.pad_z = np.max(self.region_width, axis=0)
+        self.label_padding = np.pad(seg_16,
+                                    pad_width=((self.pad_x, self.pad_x),
+                                               (self.pad_y, self.pad_y),
+                                               (self.pad_z, self.pad_z)),
+                                    mode='constant') * 0
+
+    def _check_multicells(self):
+        """Test if there are multiple cells marked as a single region"""
+        for i, region in enumerate(self.region_list):
+            assert np.sum(np.unique(label(region))) == 1, f"more than one cell in region {i + 1}"
+
+    def load_ffn(self):
+        """Load the pre-trained FFN model"""
+        self.ffn_model = load_model(os.path.join(self.paths.models, self.paths.ffn_model_file))
+        print("Loaded the FFN model")
+
+    def initiate_tracking(self):
+        """
+        Initiate the lists to store the displacement/coordinates histories from volume 1 (t0)
+        """
+        self.cells_on_boundary = np.zeros(self.cell_num_t0).astype(int)
+        self.history.r_displacements = []
+        self.history.r_displacements.append(np.zeros((self.cell_num_t0, 3)))
+        self.history.r_segmented_coordinates = []
+        self.history.r_segmented_coordinates.append(self.r_coordinates_segment_t0)
+        self.history.r_tracked_coordinates = []
+        self.history.r_tracked_coordinates.append(self.r_coordinates_tracked_t0)
+        self.history.anim = []
+        print("Initiated coordinates for tracking (from vol 1)")
+
+    def match(self, target_volume, method="min_size"):
+        """
+        Match cells in volume 1 with the target_volume
+
+        Parameters
+        ----------
+        target_volume : int
+            The target volume to be matched
+        method : str
+            The method to segment cells.
+
+        Returns
+        -------
+        anim : matplotlib.animation.ArtistAnimation
+            The animation including each iteration of the FFN + PR-GLS predictions
+        [cells_on_boundary_local, target_volume, i_disp_from_vol1_updated, r_coor_predicted] : list
+            The matching results used to draw figures
+        """
+        # skip frames that cannot be tracked
+        if target_volume in self.miss_frame:
+            raise ValueError("target_volume is a miss_frame")
+
+        # generate automatic _segment in current volume
+        self.segresult.update_results(*self._segment(target_volume, method=method))
+
+        # track by fnn + prgls
+        r_coor_predicted, anim = self._predict_pos_once(source_volume=1, draw=True)
+
+        # boundary cells
+        cells_bd = self._get_cells_onBoundary(r_coor_predicted, self.ensemble)
+        cells_on_boundary_local = self.cells_on_boundary.copy()
+        cells_on_boundary_local[cells_bd] = 1
+
+        # accurate correction
+        _, i_disp_from_vol1_updated = \
+            self._accurate_correction(cells_on_boundary_local, r_coor_predicted)
+        print(f"Matching between vol 1 and vol {target_volume} was computed")
+        return anim, [cells_on_boundary_local, target_volume, i_disp_from_vol1_updated, r_coor_predicted]
+
+    def _accurate_correction(self, cells_on_boundary_local, r_coor_predicted):
+        """Correct center positions of cells based on the cell regions detected by unet and intensities in raw image"""
+        r_disp_from_vol1_updated = self.history.r_displacements[-1] + \
+                                   (r_coor_predicted - self.history.r_tracked_coordinates[-1])
+        i_disp_from_vol1_updated = self._transform_real_to_interpolated(r_disp_from_vol1_updated)
+        for i in range(REP_NUM_CORRECTION):
+            # update positions (from vol1) by correction
+            r_disp_from_vol1_updated, i_disp_from_vol1_updated, r_disp_correction = \
+                self._correction_once_interp(i_disp_from_vol1_updated, cells_on_boundary_local)
+
+            # stop the repetition if correction converged
+            stop_flag = self._evaluate_correction(r_disp_correction)
+            if i == REP_NUM_CORRECTION - 1 or stop_flag:
+                break
+        return r_disp_from_vol1_updated, i_disp_from_vol1_updated
+
+    def _predict_pos_once(self, source_volume, draw=False):
+        """
+        Predict cell coordinates using the transformation parameters in all repetitions
+            from fnn_prgls()
+        """
+        # fitting the parameters for transformation
+        C_t, BETA_t, coor_intermediate_list = self._fit_ffn_prgls(
+            REP_NUM_PRGLS, self.history.r_segmented_coordinates[source_volume - 1])
+
+        # Transform the coordinates
+        r_coordinates_predicted = self.history.r_tracked_coordinates[source_volume - 1].copy()
+
+        if draw:
+            ax, fig = self._subplots_ffnprgls_animation()
+            plt_objs = []
+            for i in range(len(C_t)):
+                r_coordinates_predicted, r_coordinates_predicted_pre = self._predict_one_rep(
+                    r_coordinates_predicted, coor_intermediate_list[i], BETA_t[i], C_t[i])
+                plt_obj = self._draw_transformation(
+                    ax, r_coordinates_predicted_pre, self.segresult.r_coordinates_segment,
+                    r_coordinates_predicted, layercoord=False)
+                plt_objs.append(plt_obj)
+            anim = animation.ArtistAnimation(fig, plt_objs, interval=200).to_jshtml()
+        else:
+            for i in range(len(C_t)):
+                r_coordinates_predicted, r_coordinates_predicted_pre = self._predict_one_rep(
+                    r_coordinates_predicted, coor_intermediate_list[i], BETA_t[i], C_t[i])
+            anim = None
+
+        return r_coordinates_predicted, anim
+
+    def _fit_ffn_prgls(self, rep, r_coordinates_segment_pre):
+        """
+        Appliy FFN + PR-GLS from t1 to t2 (multiple times) to get transformation parameters to predict cell coordinates
+
+        Parameters
+        ----------
+        rep : int
+            The number of repetitions of (FFN + max_iteration times of PR-GLS)
+        r_coordinates_segment_pre : numpy.ndarray
+            Coordinates of cells in previous volume. Shape: (cell_num, 3)
+
+        Returns
+        -------
+        C_t : list
+            List of C in each repetition (to predict the transformed coordinates)
+        BETA_t : list
+            List of the parameter beta used in each repetition (to predict coordinates)
+        coor_intermediate_list : list
+            List of the pre-transformed coordinates of automatically segmented cells in each repetition
+            (to predict coordinates)
+        """
+        corr_intermediate = r_coordinates_segment_pre.copy()
+        C_t = []
+        BETA_t = []
+        coor_intermediate_list = []
+        for i in range(rep):
+            coor_intermediate_list.append(corr_intermediate)
+            C, corr_intermediate = self._ffn_prgls_once(i, corr_intermediate)
+            C_t.append(C)
+            BETA_t.append(self.beta_tk * (0.8 ** i))
+        return C_t, BETA_t, coor_intermediate_list
+
+    def _ffn_prgls_once(self, i, r_coordinates_segment_pre):
+        """Apply one iteration of FFN + PR-GLS"""
+        init_match = initial_matching_quick(self.ffn_model, r_coordinates_segment_pre,
+                                            self.segresult.r_coordinates_segment, 20)
+        pre_transformation_pre = r_coordinates_segment_pre.copy()
+        P, r_coordinates_segment_post, C = pr_gls_quick(pre_transformation_pre,
+                                                        self.segresult.r_coordinates_segment,
+                                                        init_match,
+                                                        BETA=self.beta_tk * (0.8 ** i),
+                                                        max_iteration=self.max_iteration,
+                                                        LAMBDA=self.lambda_tk)
+        return C, r_coordinates_segment_post
+
+    def _predict_one_rep(self, r_coordinates_predicted_pre, coor_intermediate_list, BETA_t, C_t):
+        """
+        Predict cell coordinates using one set of the transformation parameters
+            from fnn_prgls()
+        Input:
+            r_coordinates_predicted_pre: the coordinates before transformation
+            coor_intermediate_list, BETA_t, C_t: one set of the transformation parameters
+        Return:
+            r_coordinates_predicted_post: the coordinates after transformation
+        """
+
+        length_auto_segmentation = np.size(coor_intermediate_list, axis=0)
+
+        r_coordinates_predicted_tile = np.tile(r_coordinates_predicted_pre, (length_auto_segmentation, 1, 1))
+        coor_intermediate_tile = np.tile(coor_intermediate_list, (self.cell_num_t0, 1, 1)).transpose((1, 0, 2))
+        Gram_matrix = np.exp(-np.sum(np.square(r_coordinates_predicted_tile - coor_intermediate_tile),
+                                     axis=2) / (2 * BETA_t * BETA_t))
+
+        r_coordinates_predicted_post = r_coordinates_predicted_pre + np.dot(C_t, Gram_matrix).T
+
+        return r_coordinates_predicted_post, r_coordinates_predicted_pre
+
+    def _get_cells_onBoundary(self, r_coordinates_prgls, ensemble):
+        """
+        Get cell near the boundary of the image
+        """
+        if ensemble:
+            boundary_xy = 0
+        else:
+            boundary_xy = BOUNDARY_XY
+        cells_bd = np.where(reduce(
+            np.logical_or,
+            [r_coordinates_prgls[:, 0] < boundary_xy,
+             r_coordinates_prgls[:, 1] < boundary_xy,
+             r_coordinates_prgls[:, 0] > self.x_siz - boundary_xy,
+             r_coordinates_prgls[:, 1] > self.y_siz - boundary_xy,
+             r_coordinates_prgls[:, 2] / self.z_xy_ratio < 0,
+             r_coordinates_prgls[:, 2] / self.z_xy_ratio > self.z_siz])
+        )
+        return cells_bd
+
+    def _correction_once_interp(self, i_displacement_from_vol1, cell_on_bound):
+        """
+        Correct the tracking for once (in interpolated image)
+        """
+        # generate current image of labels from the manually corrected _segment in volume 1
+        i_l_tracked_cells_prgls_0, i_l_overlap_prgls_0 = self._transform_cells_quick(i_displacement_from_vol1)
+        l_tracked_cells_prgls = i_l_tracked_cells_prgls_0[:, :,
+                                self.z_scaling // 2:self.z_siz * self.z_scaling:self.z_scaling]
+        l_overlap_prgls = i_l_overlap_prgls_0[:, :,
+                          self.z_scaling // 2:self.z_siz * self.z_scaling:self.z_scaling]
+
+        # overlapping regions of multiple cells are discarded before correction to avoid cells merging
+        l_tracked_cells_prgls[np.where(l_overlap_prgls > 1)] = 0
+
+        for i in np.where(cell_on_bound == 1)[0]:
+            l_tracked_cells_prgls[l_tracked_cells_prgls == (i + 1)] = 0
+
+        # accurate correction of displacement
+        l_coordinates_prgls_int_move = \
+            self.r_coordinates_tracked_t0 * np.array([1, 1, 1 / self.z_xy_ratio]) + \
+            i_displacement_from_vol1 * np.array([1, 1, 1 / self.z_scaling])
+        l_centers_unet_x_prgls = ndm.center_of_mass(
+            self.segresult.image_cell_bg[0, :, :, :, 0] + self.segresult.image_gcn, l_tracked_cells_prgls,
+            range(1, self.seg_cells_interpolated_corrected.max() + 1))
+        l_centers_unet_x_prgls = np.asarray(l_centers_unet_x_prgls)
+        l_centers_prgls = np.asarray(l_coordinates_prgls_int_move)
+
+        lost_cells = np.where(np.isnan(l_centers_unet_x_prgls)[:, 0])
+
+        r_displacement_correction = l_centers_unet_x_prgls - l_centers_prgls
+        r_displacement_correction[lost_cells, :] = 0
+        r_displacement_correction[:, 2] = r_displacement_correction[:, 2] * self.z_xy_ratio
+
+        # calculate the corrected displacement from vol #1
+        r_displacement_from_vol1 = i_displacement_from_vol1 * np.array(
+            [1, 1, self.z_xy_ratio / self.z_scaling]) + r_displacement_correction
+        i_displacement_from_vol1_new = self._transform_real_to_interpolated(r_displacement_from_vol1)
+
+        return r_displacement_from_vol1, i_displacement_from_vol1_new, r_displacement_correction
+
+    def _transform_cells_quick(self, vectors3d):
+        """
+        Generate a image with labels indicating the moved cells.
+
+        Parameters
+        ----------
+        vectors3d : numpy.array
+            Movements of each cell
+
+        Returns
+        -------
+        output : numpy.ndarray
+            The new image with moved cells
+        mask : numpy.ndarray
+            The new image with the
+        """
+        label_moved = self.label_padding.copy()
+        mask = label_moved.copy()
+        for label in range(0, len(self.region_list)):
+            new_x_min = self.region_xyz_min[label][0] + vectors3d[label, 0] + self.pad_x
+            new_y_min = self.region_xyz_min[label][1] + vectors3d[label, 1] + self.pad_y
+            new_z_min = self.region_xyz_min[label][2] + vectors3d[label, 2] + self.pad_z
+            subregion_previous = label_moved[new_x_min:new_x_min + self.region_width[label][0],
+                                 new_y_min:new_y_min + self.region_width[label][1],
+                                 new_z_min:new_z_min + self.region_width[label][2]]
+            if subregion_previous.shape != self.region_list[label].shape:
+                continue
+            subregion_new = subregion_previous * (1 - self.region_list[label]) + \
+                            self.region_list[label] * (label + 1)
+            label_moved[new_x_min:new_x_min + self.region_width[label][0],
+            new_y_min:new_y_min + self.region_width[label][1],
+            new_z_min:new_z_min + self.region_width[label][2]] = subregion_new
+            mask[new_x_min:new_x_min + self.region_width[label][0],
+            new_y_min:new_y_min + self.region_width[label][1],
+            new_z_min:new_z_min + self.region_width[label][2]] += \
+                (self.region_list[label] > 0).astype("int8")
+        output = label_moved[self.pad_x:-self.pad_x, self.pad_y:-self.pad_y, self.pad_z:-self.pad_z]
+        mask = mask[self.pad_x:-self.pad_x, self.pad_y:-self.pad_y, self.pad_z:-self.pad_z]
+
+        return output, mask
+
+    def _transform_motion_to_image(self, cells_on_boundary_local, i_disp_from_vol1_updated):
+        """Transform the predicted movements to the moved labels in 3D image"""
+        i_tracked_cells_corrected, i_overlap_corrected = self._transform_cells_quick(i_disp_from_vol1_updated)
+        # re-calculate boundaries by _watershed
+        i_tracked_cells_corrected[i_overlap_corrected > 1] = 0
+        for i in np.where(cells_on_boundary_local == 1)[0]:
+            i_tracked_cells_corrected[i_tracked_cells_corrected == (i + 1)] = 0
+        tracked_labels = recalculate_cell_boundaries(i_tracked_cells_corrected[:, :, self.Z_RANGE_INTERP],
+                                              i_overlap_corrected[:, :, self.Z_RANGE_INTERP])
+        return tracked_labels
+
+    def _evaluate_correction(self, r_displacement_correction):
+        """
+        evaluate if the accurate correction should be stopped
+        """
+        i_disp_test = r_displacement_correction.copy()
+        i_disp_test[:, 2] *= self.z_scaling / self.z_xy_ratio
+        if np.nanmax(np.abs(i_disp_test)) >= 0.5:
+            # print(np.nanmax(np.abs(i_disp_test)), end=",")
+            return False
+        else:
+            # print(np.nanmax(np.abs(i_disp_test)))
+            return True
+
+    def track(self, fig, ax, from_volume=2):
+        """
+        Track cells from a specific volume
+
+        Parameters
+        ----------
+        fig : matplotlib.figure.Figure
+            The figure to draw tracking results
+        ax : matplotlib.figure.Figure
+            The list of 6 subplots to draw tracking results
+        from_volume : int, optional
+            The volume from which to track the cells. Should be >= 2 and <= last tracked volume + 1. Default: 2
+        """
+        self._reset_tracking_state(from_volume)
+        for vol in range(from_volume, self.volume_num + 1):
+            self.track_one_vol(vol, fig, ax)
+        return None
+
+    def replay_track_animation(self, from_volume=2):
+        """
+        Replay the tracking animation based on the stored tracking process
+
+        Parameters
+        ----------
+        from_volume : int
+            The start volume to show the tracking process. Should be >= 2. Default: 2
+
+        Returns
+        -------
+        track_anim : matplotlib.animation.ArtistAnimation
+            The animation object to be showed
+        """
+        fig, ax = plt.subplots(figsize=(14, int(21 * self.x_siz / self.y_siz)), tight_layout=True)
+        plt.close(fig)
+        ax.axis('off')
+        track_process_images = []
+        for volume in range(from_volume, self.volume_num + 1):
+            try:
+                im = mgimg.imread(self.paths.anim + "track_anim_t%04i.png" % volume)
+            except FileNotFoundError:
+                continue
+            implot = ax.imshow(im)
+            track_process_images.append([implot])
+
+        track_anim = animation.ArtistAnimation(fig, track_process_images, interval=200, repeat=False).to_jshtml()
+        return track_anim
+
+    def _reset_tracking_state(self, from_volume):
+        """Remove the tracking history after a specific volume to re-track from this volume"""
+        assert from_volume >= 2, "from_volume should >= 2"
+        current_vol = len(self.history.r_displacements)
+        del self.history.r_displacements[from_volume - 1:]
+        del self.history.r_segmented_coordinates[from_volume - 1:]
+        del self.history.r_tracked_coordinates[from_volume - 1:]
+        assert len(self.history.r_displacements) == from_volume - 1, \
+            f"Currently data has been tracked until vol {current_vol}, the program cannot start from {from_volume}"
+        # print(f"Currently data has been tracked until vol {current_vol}, start from vol {from_volume}")
+
+    def track_one_vol(self, target_volume, fig, axc6, method="min_size"):
+        """
+        Track one volume of cells and update the coordinates information
+
+        Parameters
+        ----------
+        target_volume : int
+            The target volume to be tracked
+        fig : matplotlib.figure.Figure
+            A figure to draw the updated tracking results
+        axc6 : list of matplotlib.axes.Axes
+            A list of axes to draw each sub-figures of tracking results
+        method : str, optional
+            The method used in segmenting cells. Default: "min_size"
+        """
+        # skip frames that cannot be tracked
+        if target_volume in self.miss_frame:
+            save_img3ts(range(0, self.z_siz), self.tracked_labels,
+                        self.paths.track_results + "track_results_t%04i_z%04i.tif", target_volume, self.use_8_bit)
+            self.history.r_displacements.append(self.history.r_displacements[-1])
+            self.history.r_segmented_coordinates.append(self.segresult.r_coordinates_segment)
+            self.history.r_tracked_coordinates.append(
+                self.r_coordinates_tracked_t0 + self.history.r_displacements[-1])
+            return None
+
+        # make _segment of target volume
+        self.segresult.update_results(*self._segment(target_volume, method=method))
+
+        # FFN + PR-GLS predictions (single or ensemble)
+        source_vols_list = get_reference_vols(self.ensemble, target_volume, adjacent=self.adjacent)
+        list_predictions = []
+        for source_vol in source_vols_list:
+            r_coor_predicted, _ = self._predict_pos_once(source_volume=source_vol, draw=False)
+            list_predictions.append(r_coor_predicted)
+        r_coor_predicted_mean = trim_mean(list_predictions, 0.1, axis=0)
+
+        # remove cells moved to the boundaries of the 3D image
+        cells_bd = self._get_cells_onBoundary(r_coor_predicted_mean, self.ensemble)
+        self.cells_on_boundary[cells_bd] = 1
+
+        # accurate correction to get more accurate positions
+        r_disp_from_vol1_updated, i_disp_from_vol1_updated = \
+            self._accurate_correction(self.cells_on_boundary, r_coor_predicted_mean)
+
+        # transform positions into images
+        self.tracked_labels = self._transform_motion_to_image(self.cells_on_boundary, i_disp_from_vol1_updated)
+
+        # save tracked labels
+        save_img3ts(range(0, self.z_siz), self.tracked_labels,
+                    self.paths.track_results + "track_results_t%04i_z%04i.tif", target_volume, self.use_8_bit)
+
+        self._draw_matching_6panel(target_volume, axc6, r_coor_predicted_mean, i_disp_from_vol1_updated)
+        fig.canvas.draw()
+        plt.savefig(self.paths.anim + "track_anim_t%04i.png" % target_volume, bbox_inches='tight')
+
+        # update and save points locations
+        if self.ensemble:
+            self.cells_on_boundary = \
+                np.zeros(self.cell_num_t0).astype(int)  # in ensemble mode, cells on boundary are not deleted forever
+        self.history.r_displacements.append(r_disp_from_vol1_updated)
+        self.history.r_segmented_coordinates.append(self.segresult.r_coordinates_segment)
+        self.history.r_tracked_coordinates.append(self.r_coordinates_tracked_t0 + r_disp_from_vol1_updated)
+
+        return None
+
+    def save_coordinates(self):
+        """Save 3D coordinates in a csv file under the track_information folder
+
+        Notes
+        -----
+        x,y are coordinates with pixel unit, while z is the interpolated coordinate with the same unit as x and y
+        """
+        coord = np.asarray(self.history.r_tracked_coordinates)
+        t, cell, pos = coord.shape
+        coord_table = np.column_stack(
+            (np.repeat(np.arange(1, t + 1), cell), np.tile(np.arange(1, cell + 1), t), coord.reshape(t * cell, pos)))
+        np.savetxt(os.path.join(self.paths.track_information, "tracked_coordinates.csv"), coord_table, delimiter=',',
+                   header="cell,t,x(row),y(column),z(interpolated)", comments="")
+        print("Cell coordinates were stored in ./track_information/tracked_coordinates.csv")
```

