# Comparing `tmp/bacteria-0.1.0.tar.gz` & `tmp/bacteria-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.1.0.tar", last modified: Fri Apr 21 15:41:20 2023, max compression
+gzip compressed data, was "bacteria-0.1.1.tar", last modified: Sun Apr 23 13:19:08 2023, max compression
```

## Comparing `bacteria-0.1.0.tar` & `bacteria-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 15:41:20.137000 bacteria-0.1.0/
--rw-rw-rw-   0        0        0      603 2023-04-21 15:41:20.050000 bacteria-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-04-21 15:20:04.000000 bacteria-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 15:41:19.255000 bacteria-0.1.0/bacteria/
--rw-rw-rw-   0        0        0      721 2023-04-21 11:26:10.000000 bacteria-0.1.0/bacteria/__init__.py
--rw-rw-rw-   0        0        0   140140 2023-04-21 14:40:24.000000 bacteria-0.1.0/bacteria/functions.py
--rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.0/bacteria/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:41:19.995000 bacteria-0.1.0/bacteria.egg-info/
--rw-rw-rw-   0        0        0      603 2023-04-21 15:41:17.000000 bacteria-0.1.0/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-04-21 15:41:18.000000 bacteria-0.1.0/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 15:41:17.000000 bacteria-0.1.0/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-21 15:41:17.000000 bacteria-0.1.0/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 15:41:17.000000 bacteria-0.1.0/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 15:41:20.099000 bacteria-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-04-21 15:41:14.000000 bacteria-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:19:08.626000 bacteria-0.1.1/
+-rw-rw-rw-   0        0        0      603 2023-04-23 13:19:08.399000 bacteria-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2023-04-21 18:30:09.000000 bacteria-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-23 13:19:06.999000 bacteria-0.1.1/bacteria/
+-rw-rw-rw-   0        0        0       67 2023-04-23 10:02:48.000000 bacteria-0.1.1/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   147713 2023-04-23 13:08:05.000000 bacteria-0.1.1/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.1/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:19:08.107000 bacteria-0.1.1/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-04-23 13:19:02.000000 bacteria-0.1.1/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-04-23 13:19:03.000000 bacteria-0.1.1/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 13:19:02.000000 bacteria-0.1.1/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-23 13:19:02.000000 bacteria-0.1.1/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 13:19:03.000000 bacteria-0.1.1/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 13:19:08.498000 bacteria-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2023-04-23 13:18:26.000000 bacteria-0.1.1/setup.py
```

### Comparing `bacteria-0.1.0/PKG-INFO` & `bacteria-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.0
+Version: 0.1.1
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.0/bacteria/functions.py` & `bacteria-0.1.1/bacteria/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 import graphviz
 import scipy.io
 # import matlab.engine
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
-from IPython import display
+# from IPython import display
 from scipy.stats import sem
 from natsort import natsorted # pip install natsort
-from tqdm.notebook import tqdm
 from datetime import date,timedelta
 from matplotlib.lines import Line2D
 from sklearn import preprocessing as pre
 from sklearn.linear_model import LinearRegression
 from scipy.signal import savgol_filter, argrelextrema
 from anytree import Node, RenderTree, PostOrderIter # pip install anytree
 
@@ -222,37 +221,37 @@
         if None good_cells = df['Cell ID'].values
         
     Returns
     --------------
     df : pandas DataFrame
         df with the F/V column
     """
-    cell_cycle = []
+    cell_cycles = []
 
     if good_cells is None: good_cells = natsorted(set(df['Cell ID'].values)) 
 
     for cell in good_cells:
         time_frames = df[(df['Cell ID'] == cell) & (df['Time (fps)'])]['Time (fps)'].values
-        cell_cycle.extend(pre.MinMaxScaler((0,1)).fit_transform(np.arange(0,len(time_frames),1).reshape(-1, 1)).flatten())
+        cell_cycles.extend(pre.MinMaxScaler((0,1)).fit_transform(np.arange(0,len(time_frames),1).reshape(-1, 1)).flatten())
 
-    df['Cell Cycle'] = cell_cycle
+    df['Cell Cycle'] = cell_cycles
 
     return df
 
-def df_data3d(data, fps = 3, filter = True, comp = False):
+def df_data3d(data, fps = 3, filters = True, comp = False):
     """
     Create a pandas DataFrame of the 2D data using the headers pre-determined. 
     
     Parameters
     --------------
     data : clist.mat
         Supersegger clist already loaded
     fps : int (optional)
         Frames per second used in the experiment, usual 3
-    filter : bool (optional)
+    filters : bool (optional)
         Filter data based on data2d['stat0'] = 2 and non NaN's
     comp : bool
         Input data are the compiled clists (clist for all xy/fovs)
         
     Returns
     --------------
     df : pandas DataFrame
@@ -264,15 +263,15 @@
     gc = _good_cells(data, comp = comp)
 
     # creating the header of the dataframe removing the Focus and Fluor2 columns
     header_3d = {idx:column[0] for idx,column in enumerate(data['def3D'][0]) if column[0][:5] != 'Focus' and column[0][:6] != 'Fluor2'} 
     df_temp = []
     # for each cell take the time vector data (for each frames)
     for cell in range(data['data3D'].shape[0]):
-        if filter:
+        if filters:
             if cell in gc:
                 temp = {}
                 for column in header_3d:
                     temp[header_3d[column]] = data['data3D'][cell,column]
                     temp['Cell ID'] = cell # using the same numbers than matlab - done in gc
                 # add the time vector in fps
                 temp['Time (fps)'] = temp['Time (Frames)'] * fps
@@ -285,15 +284,15 @@
                 temp['Cell ID'] = cell+1 # using the same numbers than matlab
             # add the time vector in fps
             temp['Time (fps)'] = temp['Time (Frames)'] * fps
             temp['Age (fps)'] = temp['Age (Frames)'] * fps
             df_temp.append(pd.DataFrame(temp))
 
     df = pd.concat(df_temp)
-    if filter:
+    if filters:
         # remove the NaN values
         df = df[df['Age (Frames)'].isna()== False]
     # remove trailing space
     df.columns = df.columns.str.rstrip()
 
     df = _volume(df)
     
@@ -376,25 +375,25 @@
     data2d = df_data2d(data,fps,comp)
     
     # vector of good cells
     good_cells = data2d[data2d['stat0']==2]['Cell ID'].values
 
     return good_cells
 
-def concatenate_clist(path, fps = 3, filter = True, save_mat = False, path2save = None , direct = False):
+def concatenate_clist(path, fps = 3, filters = True, save_mat = False, path2save = None , direct = False):
     """
     Concatenate all c_list.mat from one experiment in DataFrames.
     
     Parameters
     --------------
     path : str
         Experiment path
     fps : int (optional)
         Frames per second used in the experiment, usual 3
-    filter : bool (optional)
+    filters : bool (optional)
         Filter data based on data2d['stat0'] = 2 and is.nan()
     save_mat : bool (optional)
         save the dataframes in .mat format.
     path2save : str (optional)
         If false, the data will be saved into the current directory
         else, should pass a path to save.
     direct : bool
@@ -445,15 +444,15 @@
         data2D.loc[int2d[idx][0]:int2d[idx][1]-1,'Daughter2 ID'] = [i+off2d[int2d[idx][1]] for i in data2D.iloc[int2d[idx][0]:int2d[idx][1]]['Daughter2 ID']]
         data2D.loc[int2d[idx][0]:int2d[idx][1]-1,'Mother ID'] = [i+off2d[int2d[idx][1]] if i != 0 else i for i in data2D.iloc[int2d[idx][0]:int2d[idx][1]]['Mother ID']]
 
     for idx in range(len(int3d)):
         data3D.loc[int3d[idx][0]:int3d[idx][1]-1,'Cell ID'] = [i+off3d[int3d[idx][1]] for i in data3D.iloc[int3d[idx][0]:int3d[idx][1]]['Cell ID']]
 
     gc = data2D[data2D['stat0']==2]['Cell ID'].values
-    if filter:
+    if filters:
         data2D = data2D[data2D['stat0']==2]
         data3D = data3D[data3D['Cell ID'].isin(gc)]
         data3D = data3D[data3D['Age (Frames)'].isna() == False]
         # test
         data2D['Time Division'] = data2D['Cell birth time'].values + data2D['Cell age'].values
          
         data3D = fluor_volume_ratio(data3D)
@@ -479,165 +478,161 @@
             # save matlab file
             scipy.io.savemat(path2save + os.sep +'2d_clist', mat_data2D)
             scipy.io.savemat(path2save + os.sep +'3d_clist', mat_data3D)
 
     return data2D,data3D,gc
 
 def combined_filters(df_2d, df_3d, std = 1, daughter = True, lentgh = True, plot=False):
-	"""
-	Plot the mean fluo for the lineage for the entire experiment.
-	Check also fluor_lineage().
-
-	Parameters
-	--------------
-	df_2d : DataFrame
-		DataFrame of 2D data
-	df_3d : DataFrame
-		DataFrame of 3D data
-	std : int (optional)
-		Number of standard deviations desired to use as 
-		reference for the cell size filter
+    """
+    Plot the mean fluo for the lineage for the entire experiment.
+    Check also fluor_lineage().
+
+    Parameters
+    --------------
+    df_2d : DataFrame
+        DataFrame of 2D data
+    df_3d : DataFrame
+        DataFrame of 3D data
+    std : int (optional)
+        Number of standard deviations desired to use as 
+        reference for the cell size filter
     daughter : bool (optional)
         If True the daughter filter will be used. If True
         alongised with 'lentgh' the two filters will be used
     lentgh : bool (optional)
         If True the lentgh filter will be used. If True
         alongised with 'daughter' the two filters will be used
-	plot : bool (optional)
-		Plot the histogram pre and pos filter the data
-		
-	Returns
-	--------------
-	df_2d : DataFrame
-		Filtered DataFrame of 2D data
-	df_3d : DataFrame
-		Filtered DataFrame of 3D data
-	gc_filter : nd.array
-		Array with good cells ID after filter
-	"""
-	gc = df_2d[df_2d['stat0'] == 2]['Cell ID'].values
-	wm_cell = [cell for cell in gc if df_2d[df_2d['Cell ID']==cell]['Mother ID'].values in gc]
-	good_daughters = []
-	good_cells_d = []
-
-	gc_mean_d = np.mean(df_2d['Area death'].values)
-	gc_std_d = np.std(df_2d['Area death'].values)
-	size_ref_d = gc_mean_d + gc_std_d*std
-
-	# daughter filter
-	for cell in wm_cell:
-		mae = df_2d[df_2d['Cell ID']==cell]['Mother ID'].values[0]
-		mae_d = df_2d[df_2d['Cell ID']==mae]['Area death'].values[0]
-		filha_b = df_2d[df_2d['Cell ID']==cell]['Area birth'].values[0]
-		if filha_b > .4*mae_d and filha_b < .6*mae_d:
-			good_daughters.append(cell)
-
-	# lentgh filter
-	for cell in df_2d['Cell ID'].values:
-		if (df_2d[df_2d['Cell ID']==cell]['Area death'].values) < size_ref_d:
-			good_cells_d.append(cell)
-			
-	# combined filters
-	gc_filter = natsorted(list(set(good_cells_d) & set(good_daughters)))
-
-	if plot:
-		fig,ax = plt.subplots(2,2, figsize = (12,8),sharex=True, sharey= True)
-		yx = ax[0][0].hist(df_2d['Area death'], bins=20, range = [0,1000],label = 'Pre-Filter',
-						histtype='stepfilled', facecolor='blue', edgecolor='k');
-		ax[0][0].set_title('Stat0 == 2 - '+ str(len(df_2d['Cell ID'])) + " Cells", fontsize = 17)
-		ax[0][0].axvline(size_ref_d, linestyle='-', color='red',label = 'Size ref')
-		ax[0][0].axvline(gc_mean_d, linestyle='-', color='k',label = 'Pre-Filter Mean')
-		ax[0][0].fill_between(np.arange(gc_mean_d-gc_std_d,gc_mean_d+gc_std_d,20),max(yx[0]),
-							linestyle='--', color='k',label = 'Pre-Filter Std', alpha = .1)
-		ax[0][0].legend(loc='upper right')
-		
-		ax[0][1].hist(df_2d[df_2d['Cell ID'].isin(gc_filter)]['Area death'], bins=20, range = [0,1000],label = "Combined Filters",
-					histtype='stepfilled', facecolor='yellow', edgecolor='k');
-		ax[0][1].set_title("Combined Filters - "+ str(len(gc_filter)) + " Cells", fontsize = 17)
-		ax[0][1].axvline(size_ref_d, linestyle='-', color='red',label = 'Size ref')
-		ax[0][1].axvline(gc_mean_d, linestyle='-', color='k',label = 'Pre-Filter Mean')
-		ax[0][1].fill_between(np.arange(gc_mean_d-gc_std_d,gc_mean_d+gc_std_d,20),max(yx[0]),
-							linestyle='--', color='k',label = 'Pre-Filter Std', alpha = .1)
-		ax[0][1].legend(loc='upper right')
-
-		ax[1][0].hist(df_2d[df_2d['Cell ID'].isin(good_daughters)]['Area death'], bins=20, range = [0,1000],label = "Daughters Filter",
-					histtype='stepfilled', facecolor='green', edgecolor='k');
-		ax[1][0].set_title("Daughters Filter - " + str(len(good_daughters)) + " Cells", fontsize = 17)
-		ax[1][0].axvline(size_ref_d, linestyle='-', color='red',label = 'Size ref')
-		ax[1][0].axvline(gc_mean_d, linestyle='-', color='k',label = 'Pre-Filter Mean')
-		ax[1][0].fill_between(np.arange(gc_mean_d-gc_std_d,gc_mean_d+gc_std_d,20),max(yx[0]),
-							linestyle='--', color='k',label = 'Pre-Filter Std', alpha = .1)
-		ax[1][0].legend(loc='upper right')
-
-		ax[1][1].hist(df_2d[df_2d['Cell ID'].isin(good_cells_d)]['Area death'], bins=20, range = [0,1000],label = "Length Filter",
-					histtype='stepfilled', facecolor='orange', edgecolor='k');
-		ax[1][1].set_title('Length Filter - '+ str(len(good_cells_d)) + " Cells", fontsize = 17)
-		ax[1][1].axvline(size_ref_d, linestyle='-', color='red',label = 'Size ref')
-		ax[1][1].axvline(gc_mean_d, linestyle='-', color='k',label = 'Pre-Filter Mean')
-		ax[1][1].fill_between(np.arange(gc_mean_d-gc_std_d,gc_mean_d+gc_std_d,20),max(yx[0]),
-							linestyle='--', color='k',label = 'Pre-Filter Std', alpha = .1)
-		ax[1][1].legend(loc='upper right')
-
-		fig.supxlabel('Division size (px)', fontsize = 15)
-		fig.supylabel('Number of cells', fontsize = 15)
-		plt.tight_layout()
-
-	# Filters
-	if daughter == True and lentgh == True:
-		gc_filter = natsorted(list(set(good_cells_d) & set(good_daughters)))
-	elif daughter == True and lentgh == False:
-		gc_filter = natsorted(set(good_daughters))
-	elif lentgh == False and lentgh == True:
-		gc_filter = natsorted(set(good_cells_d))
-		
-	df_3d = df_3d[df_3d['Cell ID'].isin(gc_filter)]
-	df_2d = df_2d[df_2d['Cell ID'].isin(gc_filter)]
+    plot : bool (optional)
+        Plot the histogram pre and pos filter the data
+        
+    Returns
+    --------------
+    df_2d : DataFrame
+        Filtered DataFrame of 2D data
+    df_3d : DataFrame
+        Filtered DataFrame of 3D data
+    gc_filter : nd.array
+        Array with good cells ID after filter
+    """
+    gc = df_2d[df_2d['stat0'] == 2]['Cell ID'].values
+    wm_cell = [cell for cell in gc if df_2d[df_2d['Cell ID']==cell]['Mother ID'].values in gc]
+    good_daughters = []
+    good_cells_d = []
+
+    gc_mean_d = np.mean(df_2d['Area death'].values)
+    gc_std_d = np.std(df_2d['Area death'].values)
+    size_ref_d = gc_mean_d + gc_std_d*std
+
+    # daughter filter
+    for cell in wm_cell:
+        mae = df_2d[df_2d['Cell ID']==cell]['Mother ID'].values[0]
+        mae_d = df_2d[df_2d['Cell ID']==mae]['Area death'].values[0]
+        filha_b = df_2d[df_2d['Cell ID']==cell]['Area birth'].values[0]
+        if filha_b > .4*mae_d and filha_b < .6*mae_d:
+            good_daughters.append(cell)
+
+    # lentgh filter
+    for cell in df_2d['Cell ID'].values:
+        if (df_2d[df_2d['Cell ID']==cell]['Area death'].values) < size_ref_d:
+            good_cells_d.append(cell)
+
+    # combined filters
+    gc_filter = natsorted(list(set(good_cells_d) & set(good_daughters)))
 
-	return df_2d,df_3d,np.asarray(gc_filter)
+    if plot:
+        fig,ax = plt.subplots(2,2, figsize = (12,8),sharex=True, sharey= True)
+        yx = ax[0][0].hist(df_2d['Area death'], bins=20, range = [0,1000],label = 'Pre-Filter',histtype='stepfilled', facecolor='blue', edgecolor='k')
+        ax[0][0].set_title('Stat0 == 2 - '+ str(len(df_2d['Cell ID'])) + " Cells", fontsize = 17)
+        ax[0][0].axvline(size_ref_d, linestyle='-', color='red',label = 'Size ref')
+        ax[0][0].axvline(gc_mean_d, linestyle='-', color='k',label = 'Pre-Filter Mean')
+        ax[0][0].fill_between(np.arange(gc_mean_d-gc_std_d,gc_mean_d+gc_std_d,20),max(yx[0]),
+                            linestyle='--', color='k',label = 'Pre-Filter Std', alpha = .1)
+        ax[0][0].legend(loc='upper right')
+
+        ax[0][1].hist(df_2d[df_2d['Cell ID'].isin(gc_filter)]['Area death'], bins=20, range = [0,1000],label = "Combined Filters",histtype='stepfilled', facecolor='yellow', edgecolor='k')
+        ax[0][1].set_title("Combined Filters - "+ str(len(gc_filter)) + " Cells", fontsize = 17)
+        ax[0][1].axvline(size_ref_d, linestyle='-', color='red',label = 'Size ref')
+        ax[0][1].axvline(gc_mean_d, linestyle='-', color='k',label = 'Pre-Filter Mean')
+        ax[0][1].fill_between(np.arange(gc_mean_d-gc_std_d,gc_mean_d+gc_std_d,20),max(yx[0]),
+                            linestyle='--', color='k',label = 'Pre-Filter Std', alpha = .1)
+        ax[0][1].legend(loc='upper right')
+
+        ax[1][0].hist(df_2d[df_2d['Cell ID'].isin(good_daughters)]['Area death'], bins=20, range = [0,1000],label = "Daughters Filter",histtype='stepfilled', facecolor='green', edgecolor='k')
+        ax[1][0].set_title("Daughters Filter - " + str(len(good_daughters)) + " Cells", fontsize = 17)
+        ax[1][0].axvline(size_ref_d, linestyle='-', color='red',label = 'Size ref')
+        ax[1][0].axvline(gc_mean_d, linestyle='-', color='k',label = 'Pre-Filter Mean')
+        ax[1][0].fill_between(np.arange(gc_mean_d-gc_std_d,gc_mean_d+gc_std_d,20),max(yx[0]),
+                            linestyle='--', color='k',label = 'Pre-Filter Std', alpha = .1)
+        ax[1][0].legend(loc='upper right')
+
+        ax[1][1].hist(df_2d[df_2d['Cell ID'].isin(good_cells_d)]['Area death'], bins=20, range = [0,1000],label = "Length Filter",histtype='stepfilled', facecolor='orange', edgecolor='k')
+        ax[1][1].set_title('Length Filter - '+ str(len(good_cells_d)) + " Cells", fontsize = 17)
+        ax[1][1].axvline(size_ref_d, linestyle='-', color='red',label = 'Size ref')
+        ax[1][1].axvline(gc_mean_d, linestyle='-', color='k',label = 'Pre-Filter Mean')
+        ax[1][1].fill_between(np.arange(gc_mean_d-gc_std_d,gc_mean_d+gc_std_d,20),max(yx[0]),
+                            linestyle='--', color='k',label = 'Pre-Filter Std', alpha = .1)
+        ax[1][1].legend(loc='upper right')
+
+        fig.supxlabel('Division size (px)', fontsize = 15)
+        fig.supylabel('Number of cells', fontsize = 15)
+        plt.tight_layout()
+
+    # Filters
+    if daughter == True and lentgh == True:
+        gc_filter = natsorted(list(set(good_cells_d) & set(good_daughters)))
+    elif daughter == True and lentgh == False:
+        gc_filter = natsorted(set(good_daughters))
+    elif lentgh == False and lentgh == True:
+        gc_filter = natsorted(set(good_cells_d))
+
+    df_3d = df_3d[df_3d['Cell ID'].isin(gc_filter)]
+    df_2d = df_2d[df_2d['Cell ID'].isin(gc_filter)]
+
+    return df_2d,df_3d,np.asarray(gc_filter)
 
 def plot_2d_data(df_2d):
-	"""
-	Plot The Growth Rate, Cell Age and
-	Long axis (L) death by 'Birth Time +
-	Age'.
-
-	Parameters
-	--------------
-	df_3d : DataFrame
-		DataFrame of 3D data
-	reverse_lineage : dict
-		Dict with the lineage Cell ID's as key,
-		output from 'lineages()'
-	shift : int
-		The time value of the shift
-			
-	Returns
-	--------------
-	None
-	"""	
-	df_2d['Cell birth time + age'] = df_2d['Cell birth time'].values + df_2d['Cell age'].values
-	_,ax = plt.subplots(1,3, figsize =(18,4))
-	df = pd.melt(df_2d, id_vars=['Cell ID','Cell birth time + age'], value_vars=['Growth Rate']).sort_values(by=['Cell birth time + age'])
-	ax[0].plot(df['Cell birth time + age'],df.value.rolling(150).mean())
-	ax[0].set_ylabel('Growth Rate', fontsize = 15)
-	ax[0].set_xlabel('Cell birth time + age', fontsize = 15)
-	ax[0].set_title('Growth Rate by Birth Time + Age', fontsize = 17)
-
-	df = pd.melt(df_2d, id_vars=['Cell ID','Cell birth time + age'], value_vars=['Cell age']).sort_values(by=['Cell birth time + age'])
-	ax[1].plot(df['Cell birth time + age'],df.value.rolling(150).mean())
-	ax[1].set_ylabel('Cell age', fontsize = 15)
-	ax[1].set_xlabel('Cell birth time + age', fontsize = 15)
-	ax[1].set_title('Cell Age by Birth Time + Age', fontsize = 17)
-
-	df = pd.melt(df_2d, id_vars=['Cell ID','Cell birth time + age'], value_vars=['Long axis (L) death']).sort_values(by=['Cell birth time + age'])
-	ax[2].plot(df['Cell birth time + age'],df.value.rolling(150).mean())
-	ax[2].set_ylabel('Long axis (L) death', fontsize = 15)
-	ax[2].set_xlabel('Cell birth time + age', fontsize = 15)
-	ax[2].set_title('Long axis (L) death by Birth Time + Age', fontsize = 17)
-	plt.show()
+    """
+    Plot The Growth Rate, Cell Age and
+    Long axis (L) death by 'Birth Time +
+    Age'.
+
+    Parameters
+    --------------
+    df_3d : DataFrame
+        DataFrame of 3D data
+    reverse_lineage : dict
+        Dict with the lineage Cell ID's as key,
+        output from 'lineages()'
+    shift : int
+        The time value of the shift
+            
+    Returns
+    --------------
+    None
+    """	
+    df_2d['Cell birth time + age'] = df_2d['Cell birth time'].values + df_2d['Cell age'].values
+    _,ax = plt.subplots(1,3, figsize =(18,4))
+    df = pd.melt(df_2d, id_vars=['Cell ID','Cell birth time + age'], value_vars=['Growth Rate']).sort_values(by=['Cell birth time + age'])
+    ax[0].plot(df['Cell birth time + age'],df.value.rolling(150).mean())
+    ax[0].set_ylabel('Growth Rate', fontsize = 15)
+    ax[0].set_xlabel('Cell birth time + age', fontsize = 15)
+    ax[0].set_title('Growth Rate by Birth Time + Age', fontsize = 17)
+
+    df = pd.melt(df_2d, id_vars=['Cell ID','Cell birth time + age'], value_vars=['Cell age']).sort_values(by=['Cell birth time + age'])
+    ax[1].plot(df['Cell birth time + age'],df.value.rolling(150).mean())
+    ax[1].set_ylabel('Cell age', fontsize = 15)
+    ax[1].set_xlabel('Cell birth time + age', fontsize = 15)
+    ax[1].set_title('Cell Age by Birth Time + Age', fontsize = 17)
+    
+    df = pd.melt(df_2d, id_vars=['Cell ID','Cell birth time + age'], value_vars=['Long axis (L) death']).sort_values(by=['Cell birth time + age'])
+    ax[2].plot(df['Cell birth time + age'],df.value.rolling(150).mean())
+    ax[2].set_ylabel('Long axis (L) death', fontsize = 15)
+    ax[2].set_xlabel('Cell birth time + age', fontsize = 15)
+    ax[2].set_title('Long axis (L) death by Birth Time + Age', fontsize = 17)
+    plt.show()
 
 def roll_mean_plot2D(ax, df, y, x = 'Cell birth time', window = 50, fsize = 15):
     """
     A helper function to make a roll mean plot for 2D data
 
     Parameters
     ----------
@@ -817,30 +812,30 @@
 
     # Plot daughters fluorescence:
     color_add = 0
     if ax is None:
         for cell in df_2d[df_2d['Mother ID'] == cell_id]['Cell ID']:
             color_add += 1
             color_array = np.array([.2,.2,.2]) * color_add
-            df_2d[df_2d['Mother ID'] == cell_id]
+            # df_2d[df_2d['Mother ID'] == cell_id]
             t_daughter = pre.MinMaxScaler((1,2)).fit_transform(df_3d[df_3d['Cell ID'] == cell]['Time (Frames)'].values.reshape(-1, 1))
             plt.plot(t_daughter,df_3d[df_3d['Cell ID'] == cell]['Fluor1 mean'],color=color_array, label ='Daughter ' + str(int(cell)))
 
         plt.xlabel('Cell cycle',fontsize = 15)
         plt.ylabel('[GFP]',fontsize = 15)
         plt.title('Fluor mean - Cell ' + str(int(cell_id)),fontsize = 17)
         plt.legend()
         plt.show()
     
     else:
         out = []
         for cell in df_2d[df_2d['Mother ID'] == cell_id]['Cell ID']:
             color_add += 1
             color_array = np.array([.2,.2,.2]) * color_add
-            df_2d[df_2d['Mother ID'] == cell_id]
+            # df_2d[df_2d['Mother ID'] == cell_id]
             t_daughter = pre.MinMaxScaler((1,2)).fit_transform(df_3d[df_3d['Cell ID'] == cell]['Time (Frames)'].values.reshape(-1, 1))
             out.append(ax.plot(t_daughter,df_3d[df_3d['Cell ID'] == cell]['Fluor1 mean'],color=color_array, label ='Daughter ' + str(int(cell))))
 
             return out
         
 def _bin_vector(df_3d,t_cell,d_cell):
     """
@@ -880,15 +875,15 @@
     
     return mean_vector,bins
 
 def fluor_lineage(df_2d,df_3d,limit_inf,limit_sup):
     """
     Calculate the fluor mean for every mother cell and daugther.
     The bins here were not made using pandas.
-    
+
     Parameters
     --------------
     df_2d : DataFrame
         DataFrame of 2D data
     df_3d : DataFrame
         DataFrame of 3D data
     limit_inf : int
@@ -924,17 +919,17 @@
             temp_vector_m,bins_m = _bin_vector(df_3d,t_mother,mother_cells[mother])
             mean_m.append(temp_vector_m)
 
             # daughter cells
             daughter_cells = df_2d[df_2d['Mother ID'] == mother_cells[mother]]['Cell ID']
             daughter_cells = natsorted(list(set(daughter_cells) & set(cells_stats)))
             for daughter in daughter_cells:   
-                    t_daughter = pre.MinMaxScaler((0.95,2.05)).fit_transform(df_3d[df_3d['Cell ID'] == daughter]['Time (Frames)'].values.reshape(-1, 1))
-                    temp_vector_d,bins_d = _bin_vector(df_3d,t_daughter,daughter)
-                    mean_d.append(temp_vector_d)
+                t_daughter = pre.MinMaxScaler((0.95,2.05)).fit_transform(df_3d[df_3d['Cell ID'] == daughter]['Time (Frames)'].values.reshape(-1, 1))
+                temp_vector_d,bins_d = _bin_vector(df_3d,t_daughter,daughter)
+                mean_d.append(temp_vector_d)
 
         else:
             cells_removed.append(mother_cells[mother])
 
     mean_m = np.array([np.array(vector) for vector in mean_m]) # transform list to vector
     mean_d = np.array([np.array(vector) for vector in mean_d]) # transform list to vector
 
@@ -1138,23 +1133,24 @@
     Returns
     --------------
     time :  nd.array
         time array using column_x
     vector : nd.array
         mean of the vector from column_y
     """
-    if good_cells is None: good_cells = list(set(df['Cell ID'].values))    
-    time = np.arange(df[column_x].min(),df[column_x].max()+fps,fps)
-    vector = np.zeros((len(good_cells),len(time)))
+    if good_cells is None: 
+        good_cells = list(set(df['Cell ID'].values))    
+    times = np.arange(df[column_x].min(),df[column_x].max()+fps,fps)
+    vector = np.zeros((len(good_cells),len(times)))
 
     for idx,cell in enumerate(good_cells):
         for _,data in enumerate(zip(df[df['Cell ID']==cell][column_x],df[df['Cell ID']==cell][column_y])):
-            vector[idx,np.where(time==data[0])[0][0]] = data[1]
+            vector[idx,np.where(times==data[0])[0][0]] = data[1]
 
-    return time, np.mean(vector,0)
+    return times, np.mean(vector,0)
 
 def mean_vector_df(df,id_vars = 'Time (fps)', value_vars = 'F/V', conf = 0.95, method = np.mean,fps = 3):
     """
     Calculate the mean vector for a column in time or volume
     using pd.melt.
     
     Parameters
@@ -1183,27 +1179,27 @@
     ci : nd.array
         matrix with CI low and high (ci[:,0] = low, ci[:,1] = high)
     """
     
     df_ratio = pd.melt(df, id_vars=[id_vars], value_vars=[value_vars]).sort_values(by=[id_vars])
     time_frames = list(set(df_ratio['Time (fps)'].values))
     mean_list = []
-    time = []
+    times = []
     ci = np.zeros((len(range(1,len(time_frames)-2)),2))
 
     for i in range(1,len(time_frames)-2):
         mean_list.append(np.mean(df_ratio[df_ratio['Time (fps)'].isin(time_frames[i-1:i+2])]['value'].values))
-        time.append(time_frames[i])
+        times.append(time_frames[i])
         ci[i-1,:] = ci_bootstrap(df_ratio[df_ratio['Time (fps)'].isin(time_frames[i-1:i+2])]['value'].values,
                                  conf = conf, method = method, plot = False)
 
     mean_list = np.asarray(mean_list)
-    time = np.asarray(time)
+    times = np.asarray(times)
 
-    return time,mean_list,ci
+    return times,mean_list,ci
 
 def plot_mean_vector_df(df, id_vars = 'Time (fps)', value_vars = 'F/V', conf = 0.95, method = np.mean, fps = 3, ax = None):
     """
     Plot the mean vector for the entire experiment.
     Check also mean_vector_df().
     
     Parameters
@@ -1226,27 +1222,27 @@
         the ax position to plot
         
     Returns
     --------------
     None
     """
 
-    time,mean_vector,ci = mean_vector_df(df,id_vars=id_vars,value_vars=value_vars,conf=conf,method=method,fps=fps)
+    times,mean_vector,ci = mean_vector_df(df,id_vars=id_vars,value_vars=value_vars,conf=conf,method=method,fps=fps)
 
     if ax is None:
-        plt.plot(time,mean_vector)
-        plt.fill_between(time,ci[:,0],ci[:,1], alpha=.3)
+        plt.plot(times,mean_vector)
+        plt.fill_between(times,ci[:,0],ci[:,1], alpha=.3)
         plt.title(value_vars + ' mean', fontsize = 17)
         plt.xlabel(id_vars, fontsize = 15)
         plt.ylabel(value_vars + ' (a.u.)', fontsize = 15)
         plt.show()
 
     else:
-        out = ax.plot(time,mean_vector),\
-              ax.fill_between(time,ci[:,0],ci[:,1], alpha=.3),\
+        out = ax.plot(times,mean_vector),\
+              ax.fill_between(times,ci[:,0],ci[:,1], alpha=.3),\
               ax.set_xlabel(id_vars, fontsize = 15),\
               ax.set_ylabel(value_vars + ' (a.u.)', fontsize = 15),\
               ax.set_title(value_vars + ' mean', fontsize = 17)
         
         return out
 
 def instantaneous_measuraments(df,good_cells, column, fps = 3, minus = 1, plus = 2):
@@ -1296,22 +1292,22 @@
                 y_temp = y[i-minus:i+plus]
                 model.fit(x_temp.reshape(len(x_temp), 1), y_temp.reshape(len(y_temp)))
             gr_temp.append(model.coef_[0])
             t_temp.append(x[i])
         gr_inst[cell] = np.array(gr_temp)
         time_dict[cell] = np.array(t_temp)
 
-    time = np.arange(df['Time (fps)'].min(),df['Time (fps)'].max()+fps,fps)
-    im = np.zeros((len(gr_inst),len(time)))
+    times = np.arange(df['Time (fps)'].min(),df['Time (fps)'].max()+fps,fps)
+    im = np.zeros((len(gr_inst),len(times)))
 
     for idx,cell in enumerate(good_cells):
         for _,data in enumerate(zip(time_dict[cell],gr_inst[cell])):
-            im[idx,np.where(time==data[0])[0][0]] = data[1]
+            im[idx,np.where(times==data[0])[0][0]] = data[1]
 
-    return im,time
+    return im,times
 
 def simple_bootstrap(arr, conf = 0.95,times = 10000):
     """
     Calculate the confidence interval (CI).By default 
     the bootstrap is done for 10000 times. 
     
     Parameters
@@ -1376,15 +1372,15 @@
 
 def derivative(df_3d, column = 'Fluor1 sum',minus = 1, plus = 2, bar = True):
     """
     Calculate the derivatine of the fluor sum using
     a 3 slide window. Return a dataframe with the
     derivative, derivative normalized by volume,
     logrith
-    
+
     Parameters
     --------------
     df_3d : DataFrame
         DataFrame of 3D data
     column : str
         column to calculate the derivative
     minus : int (optional)
@@ -1402,19 +1398,24 @@
         DataFrame with the deravtives data alongside with 
         the time and volume 
     dict_derivative : dict
         A dict with other dicts that contains the 
         [volume,fluor,time,F/V and all derivatives] 
         of each cell at the slide window (cell number = key).
     """
+    import sys
+    if 'tqdm' in sys.modules:
+        from tqdm.notebook import tqdm
+    else:
+        bar = False
     if column == 'Volume':
         df_dev = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','F/V'], value_vars=[column]).sort_values(by=['Cell ID','Time (fps)'])
     else:
         df_dev = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','F/V','Volume'], value_vars=[column]).sort_values(by=['Cell ID','Time (fps)'])
-    
+
     dict_derivative,vol_dict,time_dict,bin_dict,ratio_dict = {},{},{},{},{}
     dev_dict,dev_dict_norm,dev_dict_log,dev_dict_log_norm = {},{},{},{}
 
     cells = natsorted(set(df_dev['Cell ID']))
     count = 0
 
     if bar:
@@ -1423,33 +1424,32 @@
             count += 1
             time_frames = df_dev[(df_dev['Cell ID'] == cell) & (df_dev['Time (fps)'])]['Time (fps)'].values
             vol,deriv,deriv_log,deriv_norm,deriv_log_norm,time,ratio = [],[],[],[],[],[],[]
             model_deriv = LinearRegression()
             model_deriv_log = LinearRegression()
 
             for i in range(minus,len(time_frames)-plus):
-                    x_temp = time_frames[i-minus:i+plus]
-                    y_temp = df_dev[(df_dev['Cell ID'] == cell) & (df_dev['Time (fps)'].isin(x_temp))].value.values
-                    y_temp_log = np.log(y_temp)
-                    model_deriv.fit(x_temp.reshape(len(x_temp), 1), y_temp.reshape(len(y_temp)))
-                    model_deriv_log.fit(x_temp.reshape(len(x_temp), 1), y_temp_log.reshape(len(y_temp_log)))
-                    
-                    if column == 'Volume':
-                        deriv_norm.append(model_deriv.coef_[0]/df_dev[df_dev['Cell ID'] == cell].value.values[i])
-                        deriv_log_norm.append(model_deriv_log.coef_[0]/df_dev[df_dev['Cell ID'] == cell].value.values[i])
-                        vol.append(df_dev[df_dev['Cell ID'] == cell].value.values[i])
-                    else:
-                        deriv_norm.append(model_deriv.coef_[0]/df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
-                        deriv_log_norm.append(model_deriv_log.coef_[0]/df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
-                        vol.append(df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
-
-                    deriv.append(model_deriv.coef_[0])
-                    deriv_log.append(model_deriv_log.coef_[0])
-                    time.append(time_frames[i])
-                    ratio.append(df_dev[df_dev['Cell ID'] == cell]['F/V'].values[i])
+                x_temp = time_frames[i-minus:i+plus]
+                y_temp = df_dev[(df_dev['Cell ID'] == cell) & (df_dev['Time (fps)'].isin(x_temp))].value.values
+                y_temp_log = np.log(y_temp)
+                model_deriv.fit(x_temp.reshape(len(x_temp), 1), y_temp.reshape(len(y_temp)))
+                model_deriv_log.fit(x_temp.reshape(len(x_temp), 1), y_temp_log.reshape(len(y_temp_log)))
+                if column == 'Volume':
+                    deriv_norm.append(model_deriv.coef_[0]/df_dev[df_dev['Cell ID'] == cell].value.values[i])
+                    deriv_log_norm.append(model_deriv_log.coef_[0]/df_dev[df_dev['Cell ID'] == cell].value.values[i])
+                    vol.append(df_dev[df_dev['Cell ID'] == cell].value.values[i])
+                else:
+                    deriv_norm.append(model_deriv.coef_[0]/df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
+                    deriv_log_norm.append(model_deriv_log.coef_[0]/df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
+                    vol.append(df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
+
+                deriv.append(model_deriv.coef_[0])
+                deriv_log.append(model_deriv_log.coef_[0])
+                time.append(time_frames[i])
+                ratio.append(df_dev[df_dev['Cell ID'] == cell]['F/V'].values[i])
             
             vol_dict[cell] = np.array(vol)
             dev_dict[cell] = np.array(deriv)
             dev_dict_norm[cell] = np.array(deriv_norm) 
             dev_dict_log[cell] = np.array(deriv_log)
             dev_dict_log_norm[cell] = np.array(deriv_log_norm)
             time_dict[cell] = np.array(time)
@@ -1461,110 +1461,157 @@
             count += 1
             time_frames = df_dev[(df_dev['Cell ID'] == cell) & (df_dev['Time (fps)'])]['Time (fps)'].values
             vol,deriv,deriv_log,deriv_norm,deriv_log_norm,time,ratio = [],[],[],[],[],[],[]
             model_deriv = LinearRegression()
             model_deriv_log = LinearRegression()
 
             for i in range(minus,len(time_frames)-plus):
-                    x_temp = time_frames[i-minus:i+plus]
-                    y_temp = df_dev[(df_dev['Cell ID'] == cell) & (df_dev['Time (fps)'].isin(x_temp))].value.values
-                    y_temp_log = np.log(y_temp)
-                    model_deriv.fit(x_temp.reshape(len(x_temp), 1), y_temp.reshape(len(y_temp)))
-                    model_deriv_log.fit(x_temp.reshape(len(x_temp), 1), y_temp_log.reshape(len(y_temp_log)))
-                    
-                    if column == 'Volume':
-                        deriv_norm.append(model_deriv.coef_[0]/df_dev[df_dev['Cell ID'] == cell].value.values[i])
-                        deriv_log_norm.append(model_deriv_log.coef_[0]/df_dev[df_dev['Cell ID'] == cell].value.values[i])
-                        vol.append(df_dev[df_dev['Cell ID'] == cell].value.values[i])
-                    else:
-                        deriv_norm.append(model_deriv.coef_[0]/df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
-                        deriv_log_norm.append(model_deriv_log.coef_[0]/df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
-                        vol.append(df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
-
-                    deriv.append(model_deriv.coef_[0])
-                    deriv_log.append(model_deriv_log.coef_[0])
-                    time.append(time_frames[i])
-                    ratio.append(df_dev[df_dev['Cell ID'] == cell]['F/V'].values[i])
-            
+                x_temp = time_frames[i-minus:i+plus]
+                y_temp = df_dev[(df_dev['Cell ID'] == cell) & (df_dev['Time (fps)'].isin(x_temp))].value.values
+                y_temp_log = np.log(y_temp)
+                model_deriv.fit(x_temp.reshape(len(x_temp), 1), y_temp.reshape(len(y_temp)))
+                model_deriv_log.fit(x_temp.reshape(len(x_temp), 1), y_temp_log.reshape(len(y_temp_log)))
+
+                if column == 'Volume':
+                    deriv_norm.append(model_deriv.coef_[0]/df_dev[df_dev['Cell ID'] == cell].value.values[i])
+                    deriv_log_norm.append(model_deriv_log.coef_[0]/df_dev[df_dev['Cell ID'] == cell].value.values[i])
+                    vol.append(df_dev[df_dev['Cell ID'] == cell].value.values[i])
+                else:
+                    deriv_norm.append(model_deriv.coef_[0]/df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
+                    deriv_log_norm.append(model_deriv_log.coef_[0]/df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
+                    vol.append(df_dev[df_dev['Cell ID'] == cell]['Volume'].values[i])
+
+                deriv.append(model_deriv.coef_[0])
+                deriv_log.append(model_deriv_log.coef_[0])
+                time.append(time_frames[i])
+                ratio.append(df_dev[df_dev['Cell ID'] == cell]['F/V'].values[i])
+
             vol_dict[cell] = np.array(vol)
             dev_dict[cell] = np.array(deriv)
             dev_dict_norm[cell] = np.array(deriv_norm) 
             dev_dict_log[cell] = np.array(deriv_log)
             dev_dict_log_norm[cell] = np.array(deriv_log_norm)
             time_dict[cell] = np.array(time)
             ratio_dict[cell] = np.asarray(ratio)
             bin_dict[cell] = pre.MinMaxScaler((0,1)).fit_transform(np.arange(0,len(time),1).reshape(-1, 1)).flatten()
 
     df_temp = []
     for cell in vol_dict.keys():
         ref_list = [cell]*len(vol_dict[cell])
         df_temp.append(pd.DataFrame(list(zip(ref_list,time_dict[cell],ratio_dict[cell],vol_dict[cell],dev_dict[cell],dev_dict_norm[cell],dev_dict_log[cell], dev_dict_log_norm[cell],bin_dict[cell])),
                                     columns=['Cell ID','Time (fps)','F/V','Volume','Derivative','Derivative/V','Derivative Log','Derivative Log/V','Cell Cycle']))
-        
+             
     df_derivative = pd.concat(df_temp, ignore_index=True)
     dict_derivative['Volume'],dict_derivative['Time (fps)'],dict_derivative['F/V'] = vol_dict,time_dict,ratio_dict
     dict_derivative['Cell Cycle'],dict_derivative['Derivative'],dict_derivative['Derivative/V'] = bin_dict,dev_dict,dev_dict_norm
     dict_derivative['Derivative Log'], dict_derivative['Derivative Log/V'] = dev_dict_log,dev_dict_log_norm
 
     return df_derivative,dict_derivative
 
 def column_mean(df,column,conf = .95, method = np.mean, plot_hist = False):
-	"""
-	Estimate the column mean for all cells using
-	the 'pd.melt()' method, sorting by time.
-
-	Parameters
-	--------------
-	df : DataFrame
-		DataFrame with the deravtive data alongside 
-		with the time and volume or the 3D df
+    """
+    Estimate the column mean for all cells using
+    the 'pd.melt()' method, sorting by time.
+
+    Parameters
+    --------------
+    df : DataFrame
+        DataFrame with the deravtive data alongside 
+        with the time and volume or the 3D df
     column : str
         column to calculate the mean   
-	conf : float (optional)
-		confidence interval desired for bootstrap,
-		default - 0.95
-	method : function (optional)
-		Method to use as basis for the boostrap,
-		default its np.mean. Other options are np.std
-		and stats.sem.
-	plot_hist: bool (optional)
-		Plot a histogram with the data distribution
-		
-	Returns
-	--------------
-	time : nd.array
-		1D time vector with the uniques time points (fps)
-	mean : nd.array
-		1D time vector with the mean for 
-		each time point
-	ci : nd.array
-		array(2,bins) with inferior Confidence
-		Interval in the first column and the 
-	"""
-	len_data = []
-	time = natsorted(set(df['Time (fps)'].values))
-	mean = np.zeros((len(time),))
-	ci = np.zeros((len(time),2))
-
-	for idx,ts in enumerate(time):
-		temp = df[df['Time (fps)']==ts][column].values
-		mean[idx] = np.mean(temp)
-		len_data.append(len(df[df['Time (fps)']==ts][column].values))
-		if len(temp) > 1:
-			ci[idx,:] = ci_bootstrap(temp,conf = conf, method = method, plot = False)
-		else:
-			ci[idx,:] = [-temp[0],+temp[0]]
-
-	if plot_hist:
-		plt.hist(len_data)
-		plt.ylabel('Amount of time points')
-		plt.xlabel('len(derivative)')
-		plt.show()
+    conf : float (optional)
+        confidence interval desired for bootstrap,
+        default - 0.95
+    method : function (optional)
+        Method to use as basis for the boostrap,
+        default its np.mean. Other options are np.std
+        and stats.sem.
+    plot_hist: bool (optional)
+        Plot a histogram with the data distribution
+        
+    Returns
+    --------------
+    time : nd.array
+        1D time vector with the uniques time points (fps)
+    mean : nd.array
+        1D time vector with the mean for 
+        each time point
+    ci : nd.array
+        array(2,bins) with inferior Confidence
+        Interval in the first column and the 
+    """
+    len_data = []
+    time = natsorted(set(df['Time (fps)'].values))
+    mean = np.zeros((len(time),))
+    ci = np.zeros((len(time),2))
+
+    for idx,ts in enumerate(time):
+        temp = df[df['Time (fps)']==ts][column].values
+        mean[idx] = np.mean(temp)
+        len_data.append(len(df[df['Time (fps)']==ts][column].values))
+        if len(temp) > 1:
+            ci[idx,:] = ci_bootstrap(temp,conf = conf, method = method, plot = False)
+        else:
+            ci[idx,:] = [-temp[0],+temp[0]]
+
+    if plot_hist:
+        plt.hist(len_data)
+        plt.ylabel('Amount of time points')
+        plt.xlabel('len(derivative)')
+        plt.show()
 
-	return time,mean,ci
+    return time,mean,ci
+
+def plot_column_mean(time,mean,ci,column,color = 'Orange', ax = None):
+    """
+    Plot the colunm mean for the entire experiment.
+    Check also 'column_mean()'.
+
+    Parameters
+    --------------
+    time : nd.array
+            1D time vector with the uniques time points (fps)
+            output of 'column_mean()'
+    mean : nd.array
+            1D time vector with the mean growth rate for 
+            each time point output of 'column_mean()'
+    ci : nd.array
+            array(2,bins) with inferior Confidence
+            Interval in the first column and the 
+            upper one in the second output of 
+            'column_mean()'
+    column : str
+            DataFrame column to estimate the column_mean,
+            default is 'Volume'
+    color: str (optional)
+            Color to plot the growth rate.
+    ax : nd.array (optional)
+            the ax position to plot
+        
+    Returns
+    --------------
+    None
+    """
+    if ax is None:
+        plt.plot(time,mean, color = color)
+        plt.fill_between(time,ci[:,0],ci[:,1],color=color, alpha = .3)
+        plt.title(column+ ' Mean', fontsize = 17)
+        plt.xlabel('Time (min)', fontsize = 15)
+        plt.ylabel(column, fontsize = 17)
+        plt.show()
+    else:
+        out = []
+        out.append(ax.plot(time,mean, color = color))
+        out.append(ax.fill_between(time,ci[:,0],ci[:,1],color=color, alpha = .3))
+        out.append(ax.set_title(column+ ' Mean', fontsize = 17))
+        out.append(ax.set_xlabel('Time (min)', fontsize = 15))
+        out.append(ax.set_ylabel(column, fontsize = 17))
+        
+        return out
 
 def	derivative_binning(df_deriv, derivative_column = 'Derivative', bins = 10 , plot_params = None, sort_by = 'Cell Cycle', print_bins = True, conf = 0.95, method = np.mean):
     """
     Perform the binning of the derivative of one column.
     Please check 'derivative()'.
     
     Parameters
@@ -1645,88 +1692,88 @@
         bins_mean[i,1] = np.mean(temp)
         if len(temp) > 1:
             ci[i,:] = ci_bootstrap(temp,conf = conf, method = method, plot = False)
 
     return bins_mean,ci
 
 def bin_column(df_3d,column = 'F/V',bins = 10,sort_by = 'Cell Cycle',print_bins = True,conf = .95,method = np.mean):
-	"""
-	Perform the binning of one column.
+    """
+    Perform the binning of one column.
 
-	Parameters
-	--------------
-	df_3d : DataFrame
-		DataFrame with the 3D data
-	column : str
-		DataFrame column to bin
-	bins : int or list (optional)
-		Amount of bins to use, default = 10. This
-		parameter can also receive a list/nd.array
-		with the desired bins intervals. 
-		e.g., [0,500,1000,1500,2000,2500,3000,
-		3500,4000,4500].
-	sort_by : str (optional)
-		The parameter to bin the data (x axis), the 
-		default is 'Cell Cycle', but is also possible 
-		to bin by 'Volume' or 'Time (fps)' columns.
-	print_bins : bool
-		If true will plot a report of bins
-	conf : float (optional)
-		confidence interval desired for bootstrap,
-		default - 0.95
-	method : function (optional)
-		Method to use as basis for the boostrap,
-		default its np.mean. Other options are np.std
-		and stats.sem.
-		
-	Returns
-	--------------
-	bins_mean : nd.array
-		array(2,bins) with bin value in the first
-		column and the mean value in the second
-	ci : dict
-		array(2,bins) with inferior Confidence
-		Interval in the first column and the 
-		upper one in the second
-	"""
-	if sort_by == 'Time (fps)':
-		df_bin = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','Volume','Cell Cycle'], value_vars=[column]).sort_values(by=[sort_by])
-		x = df_bin['Time (fps)'].value_counts(bins = bins, sort = False)
-	elif sort_by == 'Cell Cycle':
-		df_bin = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','Volume','Cell Cycle'], value_vars=[column]).sort_values(by=[sort_by])
-		x = df_bin['Cell Cycle'].value_counts(bins = 10, sort = False)
-	else:
-		df_bin = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','Volume','Cell Cycle'], value_vars=[column]).sort_values(by=[sort_by])
-		x = df_bin['Volume'].value_counts(bins = bins, sort = False)
-		
-	if isinstance(bins, int):
-		bins_array = np.zeros((bins,2))
-	else:
-		bins_array = np.zeros((len(bins)-1,2))
-
-	for idx,interval in enumerate(x.keys()):
-		bins_array[idx][0] = interval.left
-		bins_array[idx][1] = interval.right
-		if print_bins:
-			if sort_by == 'Cell Cycle':
-				print('Bin: {:>2}|Bin Min Value: {:>6}|Bin Max Value: {:>4}|Unique Points: {:>5}'.format((idx+1),float(interval.left),float(interval.right),x.values[idx]))
-			else:
-				print('Bin: {:>2}|Bin Min Value: {:>4}|Bin Max Value: {:>4}|Unique Points: {:>5}'.format((idx+1),int(interval.left),int(interval.right),x.values[idx]))
-	if print_bins:
-		print('\n')
-	bins_mean = np.zeros((len(bins_array),2))
-	ci = np.zeros((len(bins_array),2))
-	for i in range(len(bins_array)):
-		temp = df_bin[df_bin[sort_by].between(bins_array[i][0], bins_array[i][1])].value
-		bins_mean[i,0] = bins_array[i][1]
-		bins_mean[i,1] = np.mean(temp)
-		if len(temp) > 1:
-			ci[i,:] = ci_bootstrap(temp,conf = conf, method = method, plot = False)
-	
-	return bins_mean,ci
+    Parameters
+    --------------
+    df_3d : DataFrame
+        DataFrame with the 3D data
+    column : str
+        DataFrame column to bin
+    bins : int or list (optional)
+        Amount of bins to use, default = 10. This
+        parameter can also receive a list/nd.array
+        with the desired bins intervals. 
+        e.g., [0,500,1000,1500,2000,2500,3000,
+        3500,4000,4500].
+    sort_by : str (optional)
+        The parameter to bin the data (x axis), the 
+        default is 'Cell Cycle', but is also possible 
+        to bin by 'Volume' or 'Time (fps)' columns.
+    print_bins : bool
+        If true will plot a report of bins
+    conf : float (optional)
+        confidence interval desired for bootstrap,
+        default - 0.95
+    method : function (optional)
+        Method to use as basis for the boostrap,
+        default its np.mean. Other options are np.std
+        and stats.sem.
+        
+    Returns
+    --------------
+    bins_mean : nd.array
+        array(2,bins) with bin value in the first
+        column and the mean value in the second
+    ci : dict
+        array(2,bins) with inferior Confidence
+        Interval in the first column and the 
+        upper one in the second
+    """
+    if sort_by == 'Time (fps)':
+        df_bin = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','Volume','Cell Cycle'], value_vars=[column]).sort_values(by=[sort_by])
+        x = df_bin['Time (fps)'].value_counts(bins = bins, sort = False)
+    elif sort_by == 'Cell Cycle':
+        df_bin = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','Volume','Cell Cycle'], value_vars=[column]).sort_values(by=[sort_by])
+        x = df_bin['Cell Cycle'].value_counts(bins = 10, sort = False)
+    else:
+        df_bin = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','Volume','Cell Cycle'], value_vars=[column]).sort_values(by=[sort_by])
+        x = df_bin['Volume'].value_counts(bins = bins, sort = False)
+
+    if isinstance(bins, int):
+        bins_array = np.zeros((bins,2))
+    else:
+        bins_array = np.zeros((len(bins)-1,2))
+
+    for idx,interval in enumerate(x.keys()):
+        bins_array[idx][0] = interval.left
+        bins_array[idx][1] = interval.right
+        if print_bins:
+            if sort_by == 'Cell Cycle':
+                print('Bin: {:>2}|Bin Min Value: {:>6}|Bin Max Value: {:>4}|Unique Points: {:>5}'.format((idx+1),float(interval.left),float(interval.right),x.values[idx]))
+            else:
+                print('Bin: {:>2}|Bin Min Value: {:>4}|Bin Max Value: {:>4}|Unique Points: {:>5}'.format((idx+1),int(interval.left),int(interval.right),x.values[idx]))
+    if print_bins:
+        print('\n')
+    bins_mean = np.zeros((len(bins_array),2))
+    ci = np.zeros((len(bins_array),2))
+    for i in range(len(bins_array)):
+        temp = df_bin[df_bin[sort_by].between(bins_array[i][0], bins_array[i][1])].value
+        bins_mean[i,0] = bins_array[i][1]
+        bins_mean[i,1] = np.mean(temp)
+        if len(temp) > 1:
+            ci[i,:] = ci_bootstrap(temp,conf = conf, method = method, plot = False)
+            
+    return bins_mean,ci
 
 def plot_derivative_mean(time,mean,ci,column = 'Fluor1 sum',derivative_column = 'Derivative',color = 'Orange', ax = None):
     """
     Plot the derivative mean for the entire experiment.
     Check also derivative() and column_mean().
 
     Parameters
@@ -1755,15 +1802,15 @@
         Color to plot the growth rate.
     ax : nd.array (optional)
         the ax position to plot
         
     Returns
     --------------
     None
-	"""
+    """
     if ax is None:
         plt.plot(time,mean, color = color)
         plt.fill_between(time,ci[:,0],ci[:,1],color=color, alpha = .3)
         if column == 'Volume':
             plt.title('{} Derivative'.format(column), fontsize = 17)
         else:
             plt.title('Growth Rate'.format(column), fontsize = 17)
@@ -1783,71 +1830,24 @@
         out.append(ax.fill_between(time,ci[:,0],ci[:,1],color=color, alpha = .3))
         if column == 'Volume':
             out.append(ax.set_title('Growth Rate', fontsize = 17))
         else:
             out.append(ax.set_title('{} Derivative'.format(column), fontsize = 17))
         out.append(ax.set_xlabel('Time (min)', fontsize = 15))
         if derivative_column == 'Log Derivative/V':
-           out.append(ax.set_ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(column), fontsize = 15))
+            out.append(ax.set_ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(column), fontsize = 15))
         elif derivative_column == 'Derivative/V':
-           out.append(ax.set_ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(column), fontsize = 15))
+            out.append(ax.set_ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(column), fontsize = 15))
         elif derivative_column == 'Log Derivative':
             out.append(ax.set_ylabel(r'$\frac{\partial (log(%s))}{\partial t}$'%(column), fontsize = 15))
         elif derivative_column == 'Derivative':
             out.append(ax.set_ylabel(r'$\frac{\partial %s}{\partial t}$'%(column), fontsize = 15))
 
         return out
 
-def plot_column_mean(time,mean,ci,column,color = 'Orange', ax = None):
-	"""
-	Plot the colunm mean for the entire experiment.
-	Check also 'column_mean()'.
-
-	Parameters
-	--------------
-	time : nd.array
-			1D time vector with the uniques time points (fps)
-			output of 'column_mean()'
-	mean : nd.array
-			1D time vector with the mean growth rate for 
-			each time point output of 'column_mean()'
-	ci : nd.array
-			array(2,bins) with inferior Confidence
-			Interval in the first column and the 
-			upper one in the second output of 
-			'column_mean()'
-	column : str
-			DataFrame column to estimate the column_mean,
-			default is 'Volume'
-	color: str (optional)
-			Color to plot the growth rate.
-	ax : nd.array (optional)
-			the ax position to plot
-		
-	Returns
-	--------------
-	None
-	"""
-	if ax is None:
-		plt.plot(time,mean, color = color)
-		plt.fill_between(time,ci[:,0],ci[:,1],color=color, alpha = .3)
-		plt.title(column+ ' Mean', fontsize = 17)
-		plt.xlabel('Time (min)', fontsize = 15)
-		plt.ylabel(column, fontsize = 17)
-		plt.show()
-	else:
-		out = []
-		out.append(ax.plot(time,mean, color = color))
-		out.append(ax.fill_between(time,ci[:,0],ci[:,1],color=color, alpha = .3))
-		out.append(ax.set_title(column+ ' Mean', fontsize = 17))
-		out.append(ax.set_xlabel('Time (min)', fontsize = 15))
-		out.append(ax.set_ylabel(column, fontsize = 17))
-        
-		return out
-
 def plot_bins(arr,ci,column = 'Fluor1 sum',derivative_column = 'Derivative',sort_by = 'Cell Cycle',cmap = 'rainbow',line = 'k',ax =None):
     """
     Plot the bins that are organized into arrays.
 
     Parameters
     --------------
     arr : nd.array
@@ -1901,15 +1901,15 @@
             down = ci[:,0][i]
             left  = bins - (0.30*(interval/2)) / 2
             right = bins + (0.30*(interval/2)) / 2
             data = arr[:,1][i]
             right_fill = bins + interval/2
             left_fill = bins - interval/2
 
-            plt.plot([bins,bins], [up,down],'-',color = line);
+            plt.plot([bins,bins], [up,down],'-',color = line)
             plt.plot([left, right], [up, up], color= line)
             plt.plot([left, right], [down, down], color= line)
             # plt.plot([left_fill,right_fill],[data,data],'-',color = line, alpha = .3,linestyle='--');
             plt.plot(bins,data,'o',color = line)
             if cmap is not None:
                 plt.fill_between([left_fill,right_fill],min_v,max_v, color=c,alpha=.3)
         
@@ -1924,15 +1924,15 @@
         elif derivative_column == 'Derivative/V':
             plt.ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(column), fontsize = 15)
         elif derivative_column == 'Log Derivative':
             plt.ylabel(r'$\frac{\partial (log(%s))}{\partial t}$'%(column), fontsize = 15)
         elif derivative_column == 'Derivative':
             plt.ylabel(r'$\frac{\partial %s}{\partial t}$'%(column), fontsize = 15)
         plt.xticks(list(bins_xthick).insert(0, bins_xthick[0]-bins_xthick[0]))
-			
+            
     else:
         out = []
         out.append(ax.plot(bins_thick,data_line,'-',color = line))
         for i in range(n):
             c = next(color)
 
             bins = arr[:,0][i] - interval/2
@@ -1947,405 +1947,407 @@
             out.append(ax.plot([left, right], [up, up], color= line))
             out.append(ax.plot([left, right], [down, down], color= line))
             out.append(ax.plot(bins,data,'o',color = line))
             if cmap is not None:
                 out.append(ax.fill_between([left_fill,right_fill],min_v,max_v, color=c,alpha=.3))
 
         if sort_by == 'Cell Cycle':
-             out.append(ax.set_xlabel('Cell Cycle', fontsize = 15))
+            out.append(ax.set_xlabel('Cell Cycle', fontsize = 15))
         elif sort_by == 'Time (fps)':
             out.append(ax.set_xlabel('Time (min)', fontsize = 15))
         elif sort_by == 'Volume':
             out.append(ax.set_xlabel(r'Volume [$\mu m^3$]',fontsize = 15))
         if derivative_column == 'Log Derivative/V':
-           out.append(ax.set_ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(column), fontsize = 15))
+            out.append(ax.set_ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(column), fontsize = 15))
         elif derivative_column == 'Derivative/V':
-           out.append(ax.set_ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(column), fontsize = 15))
+            out.append(ax.set_ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(column), fontsize = 15))
         elif derivative_column == 'Log Derivative':
             out.append(ax.set_ylabel(r'$\frac{\partial (log(%s))}{\partial t}$'%(column), fontsize = 15))
         elif derivative_column == 'Derivative':
             out.append(ax.set_ylabel(r'$\frac{\partial %s}{\partial t}$'%(column), fontsize = 15))
         out.append(ax.set_xticks(bins_xthick))
         
-        return out		
+        return out
 
 def lineages(df_2d, nodes_min=5):
-	"""
-	Extract the lineage for the entire dataset using
-	AnyTree lib, data is organized using the node 
-	structure. The output is in dicts and anytree.node
-	types. The last value of reverse lineage is the ID
-	of a cell that we don't have data, cells without 
-	daughters are removed by Stat0 == 2 filter.
-
-	Parameters
-	--------------
-	df_2d : pd.DataFrame
-		2D data
-	nodes_min : int
-		The minimum value of nodes in the lineage 
-		
-	Returns
-	--------------
-	reverse_lineages : dict
-		Key values are the cell id of cells with more than
-		X nodes (nodes_min), and the data values is a 
-		list with the nodes to reach the key cell.
-	large_lineages : dict
-		Key values are the cell id of the root of the lineage,
-		the data values are the all cells ids that are part
-		of this lineage (mother and daughters).
-	large_nodes : dict
-		Key values are the cell id of the root of the lineage,
-		and the values are the Node with all the information
-		about this lineage, structure in anytree.Node dataype
-	all_nodes : dict
-		Key values are all the cell id's in the dataset,
-		and the values are the Node with all the information
-		about this lineage, structure in anytree.Node dataype 
-	"""
-	reverse_lineages = {}
-	large_lineages = {}
-	large_nodes = {}
-	all_nodes = {}
-	
-	for cell in df_2d['Cell ID'].values:
-		if cell not in df_2d['Daughter1 ID'].values and cell not in df_2d['Daughter2 ID'].values:
-			d1 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter1 ID'].values[0])
-			d2 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter2 ID'].values[0])
-
-			vars()["cell"+str(int(cell))] = Node(int(cell))
-			all_nodes[int(cell)] = vars()["cell"+str(int(cell))]
-
-			vars()["cell"+str(d1)] = Node(d1,parent = all_nodes[int(cell)])
-			all_nodes[d1] = vars()["cell"+str(d1)]
-
-			vars()["cell"+str(d2)] = Node(d2,parent = all_nodes[int(cell)])
-			all_nodes[d2] = vars()["cell"+str(d2)]
-
-		elif cell in df_2d['Daughter1 ID'].values:
-			d1 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter1 ID'].values[0])
-			d2 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter2 ID'].values[0])
-			mom = int(df_2d[df_2d['Daughter1 ID'] == cell]['Cell ID'].values[0])
-
-			vars()["cell"+str(int(cell))] = Node(int(cell), parent = all_nodes[mom])
-
-			vars()["cell"+str(d1)] = Node(d1, parent = all_nodes[int(cell)])
-			all_nodes[d1] = vars()["cell"+str(d1)]
-			
-			vars()["cell"+str(d2)] = Node(d2, parent = all_nodes[int(cell)])
-			all_nodes[d2] = vars()["cell"+str(d2)]
-
-		elif cell in df_2d['Daughter2 ID'].values:
-			d1 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter1 ID'].values[0])
-			d2 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter2 ID'].values[0])
-			mom = int(df_2d[df_2d['Daughter2 ID'] == cell]['Cell ID'].values[0])
-
-			vars()["cell"+str(int(cell))] = Node(int(cell), parent = all_nodes[mom])
-
-			vars()["cell"+str(d1)] = Node(d1, parent = all_nodes[int(cell)])
-			all_nodes[d1] = vars()["cell"+str(d1)]
-
-			vars()["cell"+str(d2)] = Node(d2, parent = all_nodes[int(cell)])
-			all_nodes[d2] = vars()["cell"+str(d2)]
-
-	for cell in df_2d['Cell ID'].values:
-		if all_nodes[int(cell)].is_root:
-			if all_nodes[int(cell)].height >= nodes_min:
-				large_lineages[int(cell)] = sorted(list(set([node.name for node in PostOrderIter(all_nodes[int(cell)])])))
-				large_nodes[int(cell)] = all_nodes[int(cell)]
-
-	for cell in df_2d['Cell ID'].values:
-		for node in PostOrderIter(all_nodes[int(cell)]):
-			temp = []
-			if len(node.anchestors) > nodes_min:
-				for name in node.anchestors:
-					temp.append(name.name)
-				reverse_lineages[node.name] = temp
-				reverse_lineages[node.name].extend([node.name])
+    """
+    Extract the lineage for the entire dataset using
+    AnyTree lib, data is organized using the node 
+    structure. The output is in dicts and anytree.node
+    types. The last value of reverse lineage is the ID
+    of a cell that we don't have data, cells without 
+    daughters are removed by Stat0 == 2 filter.
+
+    Parameters
+    --------------
+    df_2d : pd.DataFrame
+        2D data
+    nodes_min : int
+        The minimum value of nodes in the lineage 
+        
+    Returns
+    --------------
+    reverse_lineages : dict
+        Key values are the cell id of cells with more than
+        X nodes (nodes_min), and the data values is a 
+        list with the nodes to reach the key cell.
+    large_lineages : dict
+        Key values are the cell id of the root of the lineage,
+        the data values are the all cells ids that are part
+        of this lineage (mother and daughters).
+    large_nodes : dict
+        Key values are the cell id of the root of the lineage,
+        and the values are the Node with all the information
+        about this lineage, structure in anytree.Node dataype
+    all_nodes : dict
+        Key values are all the cell id's in the dataset,
+        and the values are the Node with all the information
+        about this lineage, structure in anytree.Node dataype 
+    """
+    reverse_lineages = {}
+    large_lineages = {}
+    large_nodes = {}
+    all_nodes = {}
+
+    for cell in df_2d['Cell ID'].values:
+        if cell not in df_2d['Daughter1 ID'].values and cell not in df_2d['Daughter2 ID'].values:
+            d1 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter1 ID'].values[0])
+            d2 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter2 ID'].values[0])
+
+            vars()["cell"+str(int(cell))] = Node(int(cell))
+            all_nodes[int(cell)] = vars()["cell"+str(int(cell))]
+
+            vars()["cell"+str(d1)] = Node(d1,parent = all_nodes[int(cell)])
+            all_nodes[d1] = vars()["cell"+str(d1)]
+
+            vars()["cell"+str(d2)] = Node(d2,parent = all_nodes[int(cell)])
+            all_nodes[d2] = vars()["cell"+str(d2)]
+
+        elif cell in df_2d['Daughter1 ID'].values:
+            d1 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter1 ID'].values[0])
+            d2 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter2 ID'].values[0])
+            mom = int(df_2d[df_2d['Daughter1 ID'] == cell]['Cell ID'].values[0])
+
+            vars()["cell"+str(int(cell))] = Node(int(cell), parent = all_nodes[mom])
+
+            vars()["cell"+str(d1)] = Node(d1, parent = all_nodes[int(cell)])
+            all_nodes[d1] = vars()["cell"+str(d1)]
+            
+            vars()["cell"+str(d2)] = Node(d2, parent = all_nodes[int(cell)])
+            all_nodes[d2] = vars()["cell"+str(d2)]
+
+        elif cell in df_2d['Daughter2 ID'].values:
+            d1 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter1 ID'].values[0])
+            d2 = int(df_2d[df_2d['Cell ID'] == cell]['Daughter2 ID'].values[0])
+            mom = int(df_2d[df_2d['Daughter2 ID'] == cell]['Cell ID'].values[0])
+
+            vars()["cell"+str(int(cell))] = Node(int(cell), parent = all_nodes[mom])
+
+            vars()["cell"+str(d1)] = Node(d1, parent = all_nodes[int(cell)])
+            all_nodes[d1] = vars()["cell"+str(d1)]
+
+            vars()["cell"+str(d2)] = Node(d2, parent = all_nodes[int(cell)])
+            all_nodes[d2] = vars()["cell"+str(d2)]
+
+    for cell in df_2d['Cell ID'].values:
+        if all_nodes[int(cell)].is_root:
+            if all_nodes[int(cell)].height >= nodes_min:
+                large_lineages[int(cell)] = sorted(list(set([node.name for node in PostOrderIter(all_nodes[int(cell)])])))
+                large_nodes[int(cell)] = all_nodes[int(cell)]
+
+    for cell in df_2d['Cell ID'].values:
+        for node in PostOrderIter(all_nodes[int(cell)]):
+            temp = []
+            if len(node.anchestors) > nodes_min:
+                for name in node.anchestors:
+                    temp.append(name.name)
+                reverse_lineages[node.name] = temp
+                reverse_lineages[node.name].extend([node.name])
 
-	return reverse_lineages, large_lineages, large_nodes, all_nodes
+    return reverse_lineages, large_lineages, large_nodes, all_nodes
 
 def plot_reverse_lineages(df_2d, lineage_list, column = 'Long axis (L) death', label = 'Cell Size ',for_ref = 2,return_plot = False):
-	"""
-	Plot the reverse lineage data with one column value.
-	This plot remove the last value, as by the filter 
-	we dont have the data from cells without daughters.
-	This plot is made using graphviz, the variable can
-	be used to save the plot in pdf.
-
-	Parameters
-	--------------
-	df_2d : DataFrame
-		2D data
-	lineage_list : list
-		list with the Cell ID's to plot
-	column : str (optional)
-		column value to plot alongside with the ID's
-	label : str (optional)
-		Label to use alongside with the column value,
-		as usual the column name is to big.
-	for_ref : int (optional)
-		The limit of the for range (in range - for_ref)
-	return_plot : bool (optional)
-		If true return the graphviz variable.
-		
-	Returns
-	--------------
-	None
-	"""
-	graph = graphviz.Digraph('unix', filename='unix.gv',
-						node_attr={'color': 'white', 'style': 'filled'})
-	graph.attr(size='1920,1080',rankdir='LR')
-
-	for i in range(len(lineage_list)-for_ref):
-		a = 'ID '+str(lineage_list[i]) +'\n'+ label + str(int(df_2d[df_2d['Cell ID'] == lineage_list[i]][column].values[0])) 
-		b = 'ID '+str(lineage_list[i+1]) +'\n'+ label + str(int(df_2d[df_2d['Cell ID'] == lineage_list[i+1]][column].values[0])) 
-		graph.edge(a,b)
-	
-	if return_plot:
-		return graph
-	else:
-		display.display_svg(graph)
+    """
+    Plot the reverse lineage data with one column value.
+    This plot remove the last value, as by the filter 
+    we dont have the data from cells without daughters.
+    This plot is made using graphviz, the variable can
+    be used to save the plot in pdf.
+
+    Parameters
+    --------------
+    df_2d : DataFrame
+        2D data
+    lineage_list : list
+        list with the Cell ID's to plot
+    column : str (optional)
+        column value to plot alongside with the ID's
+    label : str (optional)
+        Label to use alongside with the column value,
+        as usual the column name is to big.
+    for_ref : int (optional)
+        The limit of the for range (in range - for_ref)
+    return_plot : bool (optional)
+        If true return the graphviz variable.
+        
+    Returns
+    --------------
+    None
+    """
+    from IPython import display
+    graph = graphviz.Digraph('unix', filename='unix.gv',
+                        node_attr={'color': 'white', 'style': 'filled'})
+    graph.attr(size='1920,1080',rankdir='LR')
+
+    for i in range(len(lineage_list)-for_ref):
+        a = 'ID '+str(lineage_list[i]) +'\n'+ label + str(int(df_2d[df_2d['Cell ID'] == lineage_list[i]][column].values[0])) 
+        b = 'ID '+str(lineage_list[i+1]) +'\n'+ label + str(int(df_2d[df_2d['Cell ID'] == lineage_list[i+1]][column].values[0])) 
+        graph.edge(a,b)
+
+    if return_plot:
+        return graph
+    else:
+        display.display_svg(graph)
+  
+def plot_large_lineages(df_2d, lineage_list, return_plot = False):
+    """
+    Plot the large lineage data without prune the data.
+    This plot is made using graphviz, the variable can
+    be used to save the plot in pdf.
+
+    Parameters
+    --------------
+    df_2d : DataFrame
+        2D data
+    lineage_list : list
+        list with the Cell ID's to plot
+    return_plot : bool (optional)
+        If true return the graphviz variable.
+        
+    Returns
+    --------------
+    None
+    """
+    from IPython import display
+    graph = graphviz.Digraph('unix', filename='unix.gv',
+                        node_attr={'color': 'white', 'style': 'filled'})
+    graph.attr(size='1920,1080',rankdir='LR')
+
+    for i in df_2d[df_2d['Cell ID'].isin(lineage_list)]['Cell ID'].values:
+        id_d1 = int(df_2d[df_2d['Cell ID']==i]['Daughter1 ID'].values[0])
+        id_d2 = int(df_2d[df_2d['Cell ID']==i]['Daughter2 ID'].values[0])
+        parent = 'ID '+ str(int(i)) 
+        d1 = 'ID '+str(id_d1)
+        d2 = 'ID '+str(id_d2)
+        graph.edge(parent, d1)
+        graph.edge(parent, d2)
+
+    if return_plot:
+        return graph
+    else:
+        display.display_svg(graph)
 
 def plot_cell_size_lineage(df_2d,reverse_lineage, ax = None):
-	"""
-	Plot the cell size lineage. X-axis is the Cell ID and the
-	Y-axis is the Cell Size ('Long axis (L) death') in px, 
-	the size of the circle is proportionald to the cell size.
-
-	Parameters
-	--------------
-	df_2d : DataFrame
-		2D data
-	reverse_lineage : list
-		list with the Cell ID's to plot, check 'lineages()'
-	ax : nd.array (optional)
-		Pass the ax for subplot.
-		
-	Returns
-	--------------
-	None
-	"""	
-	dict_values = {value:int(df_2d[df_2d['Cell ID']== value]['Long axis (L) death'].values[0]) for _,value in enumerate(reverse_lineage[:-1])}
-	sizes = [i**1.99 for i in dict_values.values()]
-	
-	if ax is None:
-		sc = plt.scatter(list(dict_values.keys()),list(dict_values.values()),sizes,zorder=2,c = list(dict_values.values()),cmap=plt.get_cmap('rainbow'),edgecolor="k")
-		plt.plot(list(dict_values.keys()),list(dict_values.values()),color = 'k',zorder=1)
-		for i, txt in dict_values.items(): plt.annotate(txt, (i, txt),horizontalalignment='center',verticalalignment='center')
-		plt.xlim(min(dict_values.keys())-50,max(dict_values.keys())+30)
-		plt.ylim(0,max(dict_values.values())+15)
-		plt.ylabel('Cell Size (px)', fontsize = 15)
-		plt.xlabel('Cell ID', fontsize = 15)
-		plt.title('Cell Size Lineage {}-{}'.format(list(dict_values.keys())[0],list(dict_values.keys())[-1]), fontsize = 17)
-		plt.colorbar(sc)
-	else:
-		out = []
-		out.append(ax.scatter(list(dict_values.keys()),list(dict_values.values()),sizes,zorder=2,c = list(dict_values.values()),cmap=plt.get_cmap('rainbow'),edgecolor="k"))
-		out.append(ax.plot(list(dict_values.keys()),list(dict_values.values()),color = 'k',zorder=1))
-		for i, txt in dict_values.items(): out.append(ax.annotate(txt, (i, txt),horizontalalignment='center',verticalalignment='center'))
-		out.append(ax.set_xlim(min(dict_values.keys())-50,max(dict_values.keys())+30))
-		out.append(ax.set_ylim(0,max(dict_values.values())+15))
-		out.append(ax.set_xlabel('Cell ID', fontsize = 15))
-		out.append(ax.set_ylabel('Cell Size (px)', fontsize = 15))
-		out.append(ax.set_title('Cell Size Lineage {}-{}'.format(list(dict_values.keys())[0],list(dict_values.keys())[-1]), fontsize = 17))
-		out.append(plt.colorbar(out[0]))
+    """
+    Plot the cell size lineage. X-axis is the Cell ID and the
+    Y-axis is the Cell Size ('Long axis (L) death') in px, 
+    the size of the circle is proportionald to the cell size.
+
+    Parameters
+    --------------
+    df_2d : DataFrame
+        2D data
+    reverse_lineage : list
+        list with the Cell ID's to plot, check 'lineages()'
+    ax : nd.array (optional)
+        Pass the ax for subplot.
         
-		return out
+    Returns
+    --------------
+    None
+    """	
+    dict_values = {value:int(df_2d[df_2d['Cell ID']== value]['Long axis (L) death'].values[0]) for _,value in enumerate(reverse_lineage[:-1])}
+    sizes = [i**1.99 for i in dict_values.values()]
+
+    if ax is None:
+        sc = plt.scatter(list(dict_values.keys()),list(dict_values.values()),sizes,zorder=2,c = list(dict_values.values()),cmap=plt.get_cmap('rainbow'),edgecolor="k")
+        plt.plot(list(dict_values.keys()),list(dict_values.values()),color = 'k',zorder=1)
+        for i, txt in dict_values.items(): plt.annotate(txt, (i, txt),horizontalalignment='center',verticalalignment='center')
+        plt.xlim(min(dict_values.keys())-50,max(dict_values.keys())+30)
+        plt.ylim(0,max(dict_values.values())+15)
+        plt.ylabel('Cell Size (px)', fontsize = 15)
+        plt.xlabel('Cell ID', fontsize = 15)
+        plt.title('Cell Size Lineage {}-{}'.format(list(dict_values.keys())[0],list(dict_values.keys())[-1]), fontsize = 17)
+        plt.colorbar(sc)
+    else:
+        out = []
+        out.append(ax.scatter(list(dict_values.keys()),list(dict_values.values()),sizes,zorder=2,c = list(dict_values.values()),cmap=plt.get_cmap('rainbow'),edgecolor="k"))
+        out.append(ax.plot(list(dict_values.keys()),list(dict_values.values()),color = 'k',zorder=1))
+        for i, txt in dict_values.items(): out.append(ax.annotate(txt, (i, txt),horizontalalignment='center',verticalalignment='center'))
+        out.append(ax.set_xlim(min(dict_values.keys())-50,max(dict_values.keys())+30))
+        out.append(ax.set_ylim(0,max(dict_values.values())+15))
+        out.append(ax.set_xlabel('Cell ID', fontsize = 15))
+        out.append(ax.set_ylabel('Cell Size (px)', fontsize = 15))
+        out.append(ax.set_title('Cell Size Lineage {}-{}'.format(list(dict_values.keys())[0],list(dict_values.keys())[-1]), fontsize = 17))
+        out.append(plt.colorbar(out[0]))
+        
+        return out
 
 def plot_cell_lineage(df_2d,reverse_lineage,x_axis,y_axis,z_axis,c_axis ,colormap = 'rainbow',ax = None):
-	"""
-	Plot the cell size lineage. It's possible to pick different
-	varibales for each axis. The function is already removing
-	the last value of the reverse_lineage, because the last
-	cell has no daughter and is removed by our filters. 
-
-	Parameters
-	--------------
-	df_2d : DataFrame
-		2D data
-	reverse_lineage : list
-		list with the Cell ID's to plot, check 'lineages()'
-	x_axis : str
-		Data to plot in the X axis, use the df_2d terms.
-	y_axis : str
-		Data to plot in the Y axis, use the df_2d terms.
-	z_axis : str
-		Data to use as Z axis, use the df_2d terms.
-		In this case the Z is the size of each scatter point.
-		It's intrensting to use cell size as parameter, at
-		division or at birth.
-	c_axis : str
-		Data to use in the color of each saccater point and 
-		in the color bar, use the df_2d terms. It's intresting
-		to use fluorescence data.
-	colormap : str (optional)
-		Colormap to use. Check the matplotlib documentation.
+    """
+    Plot the cell size lineage. It's possible to pick different
+    varibales for each axis. The function is already removing
+    the last value of the reverse_lineage, because the last
+    cell has no daughter and is removed by our filters. 
+
+    Parameters
+    --------------
+    df_2d : DataFrame
+        2D data
+    reverse_lineage : list
+        list with the Cell ID's to plot, check 'lineages()'
+    x_axis : str
+        Data to plot in the X axis, use the df_2d terms.
+    y_axis : str
+        Data to plot in the Y axis, use the df_2d terms.
+    z_axis : str
+        Data to use as Z axis, use the df_2d terms.
+        In this case the Z is the size of each scatter point.
+        It's intrensting to use cell size as parameter, at
+        division or at birth.
+    c_axis : str
+        Data to use in the color of each saccater point and 
+        in the color bar, use the df_2d terms. It's intresting
+        to use fluorescence data.
+    colormap : str (optional)
+        Colormap to use. Check the matplotlib documentation.
         Default = rainbow.
-	ax : nd.array (optional)
-		Pass the ax for subplot.
-		
-	Returns
-	--------------
-	None
-	"""	
-	x = [np.round(df_2d[df_2d['Cell ID']== cell][x_axis].values[0],2) for cell in reverse_lineage[:-1]]
-	y = [np.round(df_2d[df_2d['Cell ID']== cell][y_axis].values[0],2) for cell in reverse_lineage[:-1]]
-	z = [df_2d[df_2d['Cell ID']== cell][z_axis].values[0] for cell in reverse_lineage[:-1]]
-	c = [df_2d[df_2d['Cell ID']== cell][c_axis].values[0] for cell in reverse_lineage[:-1]]
-	annotations = {np.round(df_2d[df_2d['Cell ID']==c][x_axis].values[0],2):np.round(df_2d[df_2d['Cell ID']==c][y_axis].values[0],2) for c in reverse_lineage[:-1]}
-	sizes = [i**1.99 for i in z]
-
-	if ax is None:
-		sc = plt.scatter(x,y,sizes,zorder=2,c = c,cmap=plt.get_cmap(colormap),edgecolor="k")
-		plt.plot(x,y,color = 'k',zorder=1)
-		for i, txt in annotations.items(): plt.annotate(txt, (i, txt),horizontalalignment='center',verticalalignment='center')
-		plt.tight_layout()
-		plt.xlim(min(x)-min(x)*.60,max(x)+max(x)*.1)
-		plt.ylim(min(y)-min(y)*.6,max(y)+max(y)*.25)
-		plt.ylabel(y_axis, fontsize = 15)
-		plt.xlabel(x_axis, fontsize = 15)
-		plt.title(y_axis+' Lineage {}-{}'.format(reverse_lineage[0],reverse_lineage[-1]), fontsize = 17)
-		plt.colorbar(sc).set_label(label=c_axis,size=15)
-
-	else:
-		out = []
-		out.append(ax.scatter(x,y,sizes,zorder=2,c = c,cmap=plt.get_cmap(colormap),edgecolor="k"))
-		out.append(ax.plot(x,y,color = 'k',zorder=1))
-		for i, txt in annotations.items(): out.append(ax.annotate(txt, (i, txt),horizontalalignment='center',verticalalignment='center'))
-		out.append(plt.tight_layout())
-		out.append(ax.set_xlim(min(x)-min(x)*.60,max(x)+max(x)*.1))
-		out.append(ax.set_ylim(min(y)-min(y)*.6,max(y)+max(y)*.25))
-		out.append(ax.set_xlabel(x_axis, fontsize = 15))
-		out.append(ax.set_ylabel(y_axis, fontsize = 15))
-		out.append(ax.set_title(y_axis+' Lineage {}-{}'.format(reverse_lineage[0],reverse_lineage[-1]), fontsize = 17))
-		out.append(plt.colorbar(out[0]).set_label(label=c_axis,size=15))
-		
-		return out
+    ax : nd.array (optional)
+        Pass the ax for subplot.
+        
+    Returns
+    --------------
+    None
+    """	
+    x = [np.round(df_2d[df_2d['Cell ID']== cell][x_axis].values[0],2) for cell in reverse_lineage[:-1]]
+    y = [np.round(df_2d[df_2d['Cell ID']== cell][y_axis].values[0],2) for cell in reverse_lineage[:-1]]
+    z = [df_2d[df_2d['Cell ID']== cell][z_axis].values[0] for cell in reverse_lineage[:-1]]
+    c = [df_2d[df_2d['Cell ID']== cell][c_axis].values[0] for cell in reverse_lineage[:-1]]
+    annotations = {np.round(df_2d[df_2d['Cell ID']==c][x_axis].values[0],2):np.round(df_2d[df_2d['Cell ID']==c][y_axis].values[0],2) for c in reverse_lineage[:-1]}
+    sizes = [i**1.99 for i in z]
+
+    if ax is None:
+        sc = plt.scatter(x,y,sizes,zorder=2,c = c,cmap=plt.get_cmap(colormap),edgecolor="k")
+        plt.plot(x,y,color = 'k',zorder=1)
+        for i, txt in annotations.items(): plt.annotate(txt, (i, txt),horizontalalignment='center',verticalalignment='center')
+        plt.tight_layout()
+        plt.xlim(min(x)-min(x)*.60,max(x)+max(x)*.1)
+        plt.ylim(min(y)-min(y)*.6,max(y)+max(y)*.25)
+        plt.ylabel(y_axis, fontsize = 15)
+        plt.xlabel(x_axis, fontsize = 15)
+        plt.title(y_axis+' Lineage {}-{}'.format(reverse_lineage[0],reverse_lineage[-1]), fontsize = 17)
+        plt.colorbar(sc).set_label(label=c_axis,size=15)
+
+    else:
+        out = []
+        out.append(ax.scatter(x,y,sizes,zorder=2,c = c,cmap=plt.get_cmap(colormap),edgecolor="k"))
+        out.append(ax.plot(x,y,color = 'k',zorder=1))
+        for i, txt in annotations.items(): out.append(ax.annotate(txt, (i, txt),horizontalalignment='center',verticalalignment='center'))
+        out.append(plt.tight_layout())
+        out.append(ax.set_xlim(min(x)-min(x)*.60,max(x)+max(x)*.1))
+        out.append(ax.set_ylim(min(y)-min(y)*.6,max(y)+max(y)*.25))
+        out.append(ax.set_xlabel(x_axis, fontsize = 15))
+        out.append(ax.set_ylabel(y_axis, fontsize = 15))
+        out.append(ax.set_title(y_axis+' Lineage {}-{}'.format(reverse_lineage[0],reverse_lineage[-1]), fontsize = 17))
+        out.append(plt.colorbar(out[0]).set_label(label=c_axis,size=15))
+        
+        return out
 
 def plot_lineages_check(df_2d,reverse_lineages,y_axis,colormap = 'rainbow'):
-	"""
-	Plot all lineages using the length as x-axis. It's possible to chose
-	different columns to inspect. The function is already removing
-	the last value of the reverse_lineage, because the last
-	cell has no daughter and is removed by our filters. 
-
-	Parameters
-	--------------
-	df_2d : DataFrame
-		2D data
-	reverse_lineages : dict
-		Dict with all lineages, output from 'lineages()'
-	y_axis : str
-		Data to plot in the Y axis, use the df_2d terms.
-	colormap : str (optional)
-		Colormap to use. Check the matplotlib documentation.
-        Default = rainbow.
-		
-	Returns
-	--------------
-	None
-	"""	
-	import matplotlib
-	parameters = np.linspace(min(reverse_lineages.keys()),max(reverse_lineages.keys()),len(reverse_lineages))
-	colormap = plt.get_cmap(colormap)
-	norm = matplotlib.colors.Normalize(vmin=min(reverse_lineages.keys()),vmax=max(reverse_lineages.keys()))
-	s_m = matplotlib.cm.ScalarMappable(cmap=colormap, norm=norm)
-	s_m.set_array([])
-
-	plt.figure(figsize = (14,9))
-	for idx,lineage in enumerate(reverse_lineages):
-		y = [np.round(df_2d[df_2d['Cell ID']== cell][y_axis].values[0],2) for cell in reverse_lineages[lineage][:-1]]
-		x = np.arange(1,len(y)+1)
-		plt.scatter(x,y,zorder=2,edgecolor="k", color =  s_m.to_rgba(parameters[idx]))
-		plt.plot(x,y,color = s_m.to_rgba(parameters[idx]),zorder=1,label = lineage) 
-
-	plt.ylabel(y_axis, fontsize=15)
-	plt.xlabel('Lineage Length', fontsize=15)
-	plt.title('Lineage Check', fontsize=17)
-	plt.legend(bbox_to_anchor=(0, -.15),loc="upper left", borderaxespad=0.,ncol=11);
-	plt.colorbar(s_m);
-	plt.tight_layout()
-	plt.show()
+    """
+    Plot all lineages using the length as x-axis. It's possible to chose
+    different columns to inspect. The function is already removing
+    the last value of the reverse_lineage, because the last
+    cell has no daughter and is removed by our filters. 
 
-def plot_large_lineages(df_2d, lineage_list, return_plot = False):
-	"""
-	Plot the large lineage data without prune the data.
-	This plot is made using graphviz, the variable can
-	be used to save the plot in pdf.
-
-	Parameters
-	--------------
-	df_2d : DataFrame
-		2D data
-	lineage_list : list
-		list with the Cell ID's to plot
-	return_plot : bool (optional)
-		If true return the graphviz variable.
-		
-	Returns
-	--------------
-	None
-	"""
-	graph = graphviz.Digraph('unix', filename='unix.gv',
-						node_attr={'color': 'white', 'style': 'filled'})
-	graph.attr(size='1920,1080',rankdir='LR')
-
-	for i in df_2d[df_2d['Cell ID'].isin(lineage_list)]['Cell ID'].values:
-		id_d1 = int(df_2d[df_2d['Cell ID']==i]['Daughter1 ID'].values[0])
-		id_d2 = int(df_2d[df_2d['Cell ID']==i]['Daughter2 ID'].values[0])
-		parent = 'ID '+ str(int(i)) 
-		d1 = 'ID '+str(id_d1)
-		d2 = 'ID '+str(id_d2)
-		graph.edge(parent, d1)
-		graph.edge(parent, d2)
-
-	if return_plot:
-		return graph
-	else:
-		display.display_svg(graph)
+    Parameters
+    --------------
+    df_2d : DataFrame
+        2D data
+    reverse_lineages : dict
+        Dict with all lineages, output from 'lineages()'
+    y_axis : str
+        Data to plot in the Y axis, use the df_2d terms.
+    colormap : str (optional)
+        Colormap to use. Check the matplotlib documentation.
+        Default = rainbow.
+        
+    Returns
+    --------------
+    None
+    """	
+    import matplotlib
+    parameters = np.linspace(min(reverse_lineages.keys()),max(reverse_lineages.keys()),len(reverse_lineages))
+    colormap = plt.get_cmap(colormap)
+    norm = matplotlib.colors.Normalize(vmin=min(reverse_lineages.keys()),vmax=max(reverse_lineages.keys()))
+    s_m = matplotlib.cm.ScalarMappable(cmap=colormap, norm=norm)
+    s_m.set_array([])
+
+    plt.figure(figsize = (14,9))
+    for idx,lineage in enumerate(reverse_lineages):
+        y = [np.round(df_2d[df_2d['Cell ID']== cell][y_axis].values[0],2) for cell in reverse_lineages[lineage][:-1]]
+        x = np.arange(1,len(y)+1)
+        plt.scatter(x,y,zorder=2,edgecolor="k", color =  s_m.to_rgba(parameters[idx]))
+        plt.plot(x,y,color = s_m.to_rgba(parameters[idx]),zorder=1,label = lineage) 
+
+    plt.ylabel(y_axis, fontsize=15)
+    plt.xlabel('Lineage Length', fontsize=15)
+    plt.title('Lineage Check', fontsize=17)
+    plt.legend(bbox_to_anchor=(0, -.15),loc="upper left", borderaxespad=0.,ncol=11)
+    plt.colorbar(s_m)
+    plt.tight_layout()
+    plt.show()
 
 def plot_total_fluo_volume(df_3d, reverse_lineage, ax = None):
-	"""
-	Plot the total fluorescence by the volume. 
+    """
+    Plot the total fluorescence by the volume. 
 
-	Parameters
-	--------------
-	df_3d : DataFrame
-		3D data
-	reverse_lineage : list
-		List with the lineage Cell ID's, output 
-		from 'lineages()'
-	ax : nd.array
-		axis to plot
-			
-	Returns
-	--------------
-	None
-	"""	
-	df_oder = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','Volume'], value_vars=['Fluor1 sum']).sort_values(by=['Cell ID','Volume'])
-	if ax is None:
-		for i in reverse_lineage[:-1]:
-			plt.plot(df_oder[df_oder['Cell ID']==i]['Volume'].values,df_oder[df_oder['Cell ID']==i].value.values,'.',label='Cell {}'.format(i))
-		plt.title('Total Fluorescene Lineage {}-{}'.format(reverse_lineage[:-1][0],reverse_lineage[:-1][-1]),fontsize = 17)
-		plt.xlabel(r'Volume [$\mu m^3$]',fontsize = 15)
-		plt.ylabel('Fluor1 sum',fontsize = 15)
-		plt.legend()
-		plt.show()
-	else:
-		out = []
-		for i in reverse_lineage[:-1]:
-			out.append(ax.plot(df_oder[df_oder['Cell ID']==i]['Volume'].values,df_oder[df_oder['Cell ID']==i].value.values,'.',label='Cell {}'.format(i)))
-		out.append(ax.set_title('Total Fluorescene Lineage {}-{}'.format(reverse_lineage[:-1][0],reverse_lineage[:-1][-1]),fontsize = 17))
-		out.append(ax.set_xlabel(r'Volume [$\mu m^3$]',fontsize = 15))
-		out.append(ax.set_ylabel('Fluor1 sum',fontsize = 15))
-		out.append(ax.legend())
+    Parameters
+    --------------
+    df_3d : DataFrame
+        3D data
+    reverse_lineage : list
+        List with the lineage Cell ID's, output 
+        from 'lineages()'
+    ax : nd.array
+        axis to plot
+            
+    Returns
+    --------------
+    None
+    """	
+    df_oder = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','Volume'], value_vars=['Fluor1 sum']).sort_values(by=['Cell ID','Volume'])
+    if ax is None:
+        for i in reverse_lineage[:-1]:
+            plt.plot(df_oder[df_oder['Cell ID']==i]['Volume'].values,df_oder[df_oder['Cell ID']==i].value.values,'.',label='Cell {}'.format(i))
+        plt.title('Total Fluorescene Lineage {}-{}'.format(reverse_lineage[:-1][0],reverse_lineage[:-1][-1]),fontsize = 17)
+        plt.xlabel(r'Volume [$\mu m^3$]',fontsize = 15)
+        plt.ylabel('Fluor1 sum',fontsize = 15)
+        plt.legend()
+        plt.show()
+    else:
+        out = []
+        for i in reverse_lineage[:-1]:
+            out.append(ax.plot(df_oder[df_oder['Cell ID']==i]['Volume'].values,df_oder[df_oder['Cell ID']==i].value.values,'.',label='Cell {}'.format(i)))
+        out.append(ax.set_title('Total Fluorescene Lineage {}-{}'.format(reverse_lineage[:-1][0],reverse_lineage[:-1][-1]),fontsize = 17))
+        out.append(ax.set_xlabel(r'Volume [$\mu m^3$]',fontsize = 15))
+        out.append(ax.set_ylabel('Fluor1 sum',fontsize = 15))
+        out.append(ax.legend())
 
-		return out	
+        return out
 
 def _adjust_order(order,data,perc):
     """
     Function to adapt the order of the smooth
     filter for small data. 
     
     Parameters
@@ -2444,41 +2446,41 @@
     if len(df_3d[df_3d['Cell ID']==reverse_lineage[-1]]) == 0:
         keys = natsorted(reverse_lineage[:-1])
     else:
         keys = natsorted(reverse_lineage)
 
     df_deriv,_ = derivative(df_3d[df_3d['Cell ID'].isin(keys)],column=column,bar = False)
 
-    x_vol_sep,x_vol_order,cell_cycle = {},{},{}
+    x_vol_sep,x_vol_order,cell_cycles = {},{},{}
 
     count = 0
     order_dict = {}
 
     for idx,cell in enumerate(keys):
         if idx == 0:
             temp = df_deriv[df_deriv['Cell ID']==cell]['Volume'].values
             e_order = _adjust_order(order=order,data=temp,perc=perc)
             temp_vol = savgol_filter(temp, int(len(temp)*perc), e_order)
             x_vol_sep[cell] = temp_vol + count
-            cell_cycle[cell] = [x_vol_sep[cell][0],x_vol_sep[cell][-1]]
+            cell_cycles[cell] = [x_vol_sep[cell][0],x_vol_sep[cell][-1]]
             x_vol_order[cell] = e_order
         else:
             temp1 = df_deriv[df_deriv['Cell ID']==cell]['Volume'].values
             temp2 = df_deriv[df_deriv['Cell ID']==keys[idx-1]]['Volume'].values
 
             e_order = _adjust_order(order=order,data=temp1,perc=perc)
             temp_vol = savgol_filter(temp1, int(len(temp1)*perc), e_order)
             x_vol_order[cell] = e_order
             e_order = _adjust_order(order=order,data=temp2,perc=perc)
             temp_fut = savgol_filter(temp2, int(len(temp2)*perc), e_order)
 
             count = temp_fut[-1] - temp_vol[0] + count
             diff = np.mean(np.diff(temp_vol)) + count
             x_vol_sep[cell] = temp_vol+diff
-            cell_cycle[cell] = [x_vol_sep[cell][0],x_vol_sep[cell][-1]]
+            cell_cycles[cell] = [x_vol_sep[cell][0],x_vol_sep[cell][-1]]
             
     order_dict['volume order'] = x_vol_order
     vol_dict,dev_dict,time_dict,ratio_dict = {},{},{},{}
     vol_concat,dev_concat,time_concat,ratio_concat,df_temp = [],[],[],[],[]
 
     for cell in keys:
         temp_vol = df_deriv[df_deriv['Cell ID']==cell][derivative_column].values
@@ -2498,35 +2500,35 @@
         ratio_concat.extend(df_deriv[df_deriv['Cell ID']==cell]['F/V'].values[vol_idx])
 
         ref_list = [cell]*len(vol_dict[cell])
         df_temp.append(pd.DataFrame(list(zip(ref_list,time_dict[cell],ratio_dict[cell],vol_dict[cell],dev_dict[cell])),
                                     columns=['Cell ID','Time (fps)','F/V','Volume','Derivative']))
 
     if window is None:
-            window = int(len(vol_concat)*.2)
+        window = int(len(vol_concat)*.2)
             
     smooth_vol, smooth_dev = savgol_filter((vol_concat,dev_concat), window , order ,mode=mode)
         
     df_lineage = pd.concat(df_temp, ignore_index=True)
     df_lineage['Smoothed Volume'] = smooth_vol
     df_lineage['Smoothed Derivative'] = smooth_dev
-    
+
     local_min = argrelextrema(smooth_dev, np.less) 
     local_max = argrelextrema(smooth_dev, np.greater)
     local_min_dict,local_max_dict = {},{}
 
-    for _, key in enumerate(cell_cycle):
+    for _, key in enumerate(cell_cycles):
         local_min_dict[key] = []
         local_max_dict[key] = []
         for values in local_min[0]:
-            if cell_cycle[key][0] < smooth_vol[values] < cell_cycle[key][1]:
-                    local_min_dict[key] += [values]
+            if cell_cycles[key][0] < smooth_vol[values] < cell_cycles[key][1]:
+                local_min_dict[key] += [values]
         for values in local_max[0]:
-            if cell_cycle[key][0] < smooth_vol[values] < cell_cycle[key][1]:
-                    local_max_dict[key] += [values]
+            if cell_cycles[key][0] < smooth_vol[values] < cell_cycles[key][1]:
+                local_max_dict[key] += [values]
 
     local_min_filt = {key:np.where(smooth_dev == min(smooth_dev[local_min_dict[key]]))[0][0] if len(smooth_dev[local_min_dict[key]])>0 else 0 for key in local_min_dict}
     local_max_filt = {key:np.where(smooth_dev == max(smooth_dev[local_max_dict[key]]))[0][0] if len(smooth_dev[local_max_dict[key]])>0 else 0 for key in local_max_dict}
     peaks = {'minima':local_min_filt,'maxima':local_max_filt}
 
     return df_lineage,peaks,order_dict
 
@@ -2620,154 +2622,154 @@
         first = reverse_lineages[cell][0]
         if df_3d[df_3d['Cell ID']==first]['Time (fps)'].values[0] > shift:
             lineage_filter.append(reverse_lineages[cell])
 
     return natsorted(lineage_filter)
 
 def longer_lineages(df_3d, reverse_lineages, column = 'Fluor1 mean', method = np.var):
-	"""
-	Filter the lineages based on length and return 
-	the variance (default or other method - np.mean, 
-	np.std, stats.sem and others) for one feature (as 
-	default 'Fluor1 mean', but can be used any column 
-	of df_3d). Return a dictionary with the root cell 
-	as a key, each root cell have dictionaries with 
-	the longest lineages and use the last cell ID as key. 
-	The values in the dict is the method applied into 
-	the column choosed. This function is used as support 
-	for other functions.
-
-	Parameters
-	--------------
-	df_3d : DataFrame
-		DataFrame of 3D data
-	reverse_lineage : dict
-		Dict with the lineage Cell ID's as key,
-		output from 'lineages()'
-	column : str (optional)
-		The column to estimate the
+    """
+    Filter the lineages based on length and return 
+    the variance (default or other method - np.mean, 
+    np.std, stats.sem and others) for one feature (as 
+    default 'Fluor1 mean', but can be used any column 
+    of df_3d). Return a dictionary with the root cell 
+    as a key, each root cell have dictionaries with 
+    the longest lineages and use the last cell ID as key. 
+    The values in the dict is the method applied into 
+    the column choosed. This function is used as support 
+    for other functions.
+
+    Parameters
+    --------------
+    df_3d : DataFrame
+        DataFrame of 3D data
+    reverse_lineage : dict
+        Dict with the lineage Cell ID's as key,
+        output from 'lineages()'
+    column : str (optional)
+        The column to estimate the
     method : function (optional)
         Method to use to extract feature of
-		each cell, default its np.mean. Other 
-		options are np.std and stats.sem.
-			
-	Returns
-	--------------
-	root_dict : dict
-		Dict with the mother Cell ID used as a key and
-		inside each mother cell another dict with the
-		longest daughters, the key of this dict is the
-		last cell of the lineage.
-	lineage_array : nd.array
-		Array with all lineages in arrays. Used in plot
-		functions.
-	len_dict : dict
-		Dict with the mother Cell ID used as a key and
-		inside the lenght of the longest lineage.
-	"""	
-	lineage_array = np.array([np.array(lineage) for lineage in list(reverse_lineages.values())],dtype=object)
-	fist_cells = natsorted(set([cell[0] for cell in lineage_array]))
-
-	len_dict = {}
-	for root_cell in fist_cells:
-		temp_len = 0
-		for cell in lineage_array:
-			if cell[0] == root_cell:
-				if len(cell) > temp_len:
-					temp_len = len(cell)
-		len_dict[root_cell] = temp_len
-
-	root_dict = {}
-	for root_cell in fist_cells:
-		count = 0
-		temp_dict = {}
-		for lineage in lineage_array: # other length?
-			if lineage[0] == root_cell and len_dict[root_cell] == len(lineage):
-				temp_list = []
-				for cell in lineage:
-					temp_list.append(method(df_3d[df_3d['Cell ID']==cell][column].values))    
-				temp_dict[cell] = temp_list
-				count += 1
-		root_dict[root_cell] = temp_dict
-	
-	return root_dict, lineage_array, len_dict
+        each cell, default its np.mean. Other 
+        options are np.std and stats.sem.
+            
+    Returns
+    --------------
+    root_dict : dict
+        Dict with the mother Cell ID used as a key and
+        inside each mother cell another dict with the
+        longest daughters, the key of this dict is the
+        last cell of the lineage.
+    lineage_array : nd.array
+        Array with all lineages in arrays. Used in plot
+        functions.
+    len_dict : dict
+        Dict with the mother Cell ID used as a key and
+        inside the lenght of the longest lineage.
+    """	
+    lineage_array = np.array([np.array(lineage) for lineage in list(reverse_lineages.values())],dtype=object)
+    fist_cells = natsorted(set([cell[0] for cell in lineage_array]))
+
+    len_dict = {}
+    for root_cell in fist_cells:
+        temp_len = 0
+        for cell in lineage_array:
+            if cell[0] == root_cell:
+                if len(cell) > temp_len:
+                    temp_len = len(cell)
+        len_dict[root_cell] = temp_len
+
+    root_dict = {}
+    for root_cell in fist_cells:
+        count = 0
+        temp_dict = {}
+        for lineage in lineage_array: # other length?
+            if lineage[0] == root_cell and len_dict[root_cell] == len(lineage):
+                temp_list = []
+                for cell in lineage:
+                    temp_list.append(method(df_3d[df_3d['Cell ID']==cell][column].values))    
+                temp_dict[cell] = temp_list
+                count += 1
+        root_dict[root_cell] = temp_dict
+
+    return root_dict, lineage_array, len_dict
 
 def lineage_corr_filter(df_3d,reverse_lineages,shift = None,threshold = .96,column = 'Fluor1 mean', method = np.var):
-	"""
-	Filter the lineages based on the correlation
-	between the longest lineage of a mother cell.
-	Return the lineages that match the parameters.
-	
-	Parameters
-	--------------
-	df_3d : DataFrame
-		DataFrame of 3D data
-	reverse_lineage : dict
-		Dict with the lineage Cell ID's as key,
-		output from 'lineages()'
-	shift : int (optional)
-		Value to use to extract the lineages that
-		pass through this time point, usually used
-		to get the shift moment. If shift is passed
-		automatically the output will be filtered 
-		for these cells. Default is None.
-	threshold : float (optional)
-		Value to be used as threshold to determine
-		if the lineage must be maintained. If the 
-		correlation between the daughter lineages 
-		is less than the threshold value, the 
-		lineage is maintained. Default '.96'.
-	column : str (optional)
-		The column to extract the feature of
-		the dataset. Default 'Fluor1 mean'.
+    """
+    Filter the lineages based on the correlation
+    between the longest lineage of a mother cell.
+    Return the lineages that match the parameters.
+
+    Parameters
+    --------------
+    df_3d : DataFrame
+        DataFrame of 3D data
+    reverse_lineage : dict
+        Dict with the lineage Cell ID's as key,
+        output from 'lineages()'
+    shift : int (optional)
+        Value to use to extract the lineages that
+        pass through this time point, usually used
+        to get the shift moment. If shift is passed
+        automatically the output will be filtered 
+        for these cells. Default is None.
+    threshold : float (optional)
+        Value to be used as threshold to determine
+        if the lineage must be maintained. If the 
+        correlation between the daughter lineages 
+        is less than the threshold value, the 
+        lineage is maintained. Default '.96'.
+    column : str (optional)
+        The column to extract the feature of
+        the dataset. Default 'Fluor1 mean'.
     method : function (optional)
         Method to use to extract feature of
-		each cell, default its np.mean. Other 
-		options are np.std and stats.sem.	
-			
-	Returns
-	--------------
-	filtered_lineage : list
-		List with the Cell ID for each lineage that
-		match the paramters (threshold and shift).
-		Longest lineages for each mother cell and
-		different from each other in case of more 
-		than one.
-	"""
-	root_dict,_,_ = longer_lineages(df_3d = df_3d,
-			     			        reverse_lineages = reverse_lineages,
-								    column = column, 
-								    method = method)
-	if shift is not None:
-		lineage_filter = lineages_shift(df_3d = df_3d,
-				  						reverse_lineages = reverse_lineages,
-										shift = shift)
-
-	lineages_corr = []
-	for mother_cell in root_dict.keys():
-		keys_lineage = list(root_dict[mother_cell].keys())
-		corr_arr = np.array([np.array(root_dict[mother_cell][i][:-1]) for i in root_dict[mother_cell]]) 
-		corr = np.corrcoef(corr_arr)
-		if len(corr[::2,::2]) == 1:
-			lineages_corr.append(keys_lineage[0])
-		elif len(corr[::2,::2][0]) > 1:
-			for i in range(1,len(corr[::2,::2][0])):
-				if corr[::2,::2][0][i] < threshold:
-					lineages_corr.append(keys_lineage[i])
-
-	filtered_lineage = []
-	for cell in reverse_lineages:
-		if shift is not None:
-			if cell in natsorted(list(set(lineages_corr) & set(lineage_filter))):
-					filtered_lineage.append(reverse_lineages[cell])
-		else:
-			if cell in natsorted(set(lineages_corr)):
-					filtered_lineage.append(reverse_lineages[cell])
-	
-	return filtered_lineage
+        each cell, default its np.mean. Other 
+        options are np.std and stats.sem.	
+            
+    Returns
+    --------------
+    filtered_lineage : list
+        List with the Cell ID for each lineage that
+        match the paramters (threshold and shift).
+        Longest lineages for each mother cell and
+        different from each other in case of more 
+        than one.
+    """
+    root_dict,_,_ = longer_lineages(df_3d = df_3d,
+                                    reverse_lineages = reverse_lineages,
+                                    column = column, 
+                                    method = method)
+    if shift is not None:
+        lineage_filter = lineages_shift(df_3d = df_3d,
+                                        reverse_lineages = reverse_lineages,
+                                        shift = shift)
+
+    lineages_corr = []
+    for mother_cell in root_dict.keys():
+        keys_lineage = list(root_dict[mother_cell].keys())
+        corr_arr = np.array([np.array(root_dict[mother_cell][i][:-1]) for i in root_dict[mother_cell]])
+        corr = np.corrcoef(corr_arr)
+        if len(corr[::2,::2]) == 1:
+            lineages_corr.append(keys_lineage[0])
+        elif len(corr[::2,::2][0]) > 1:
+            for i in range(1,len(corr[::2,::2][0])):
+                if corr[::2,::2][0][i] < threshold:
+                    lineages_corr.append(keys_lineage[i])
+
+    filtered_lineage = []
+    for cell in reverse_lineages:
+        if shift is not None:
+            if cell in natsorted(list(set(lineages_corr) & set(lineage_filter))):
+                filtered_lineage.append(reverse_lineages[cell])
+        else:
+            if cell in natsorted(set(lineages_corr)):
+                filtered_lineage.append(reverse_lineages[cell])
+
+    return filtered_lineage
 
 def plot_lineage_derivative(df_lineage,peaks,column = 'Fluor1 sum',derivative_column = 'Derivative',x_axis = 'Smoothed Volume',ax = None):
     """
     Plot a single lineages derivative with the
     local minima and local maxmia. The input parameters
     are the output of 'lineage_derivative()'. This 
     function can receive both volume ('Smoothed Volume')
@@ -2844,17 +2846,17 @@
         if x_axis == 'Time (fps)':
             out.append(ax.set_xlabel('Time (min)', fontsize = 15))
         elif x_axis == 'Smoothed Volume':
             out.append(ax.set_xlabel(r'Volume [$\mu m^3$]', fontsize = 15))
         else:
             out.append(ax.set_xlabel(x_axis, fontsize = 15))
         if derivative_column == 'Log Derivative/V':
-           out.append(ax.set_ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(column), fontsize = 15))
+            out.append(ax.set_ylabel(r'$\frac{\frac{\partial (log(%s))}{\partial t}}{Volume}$'%(column), fontsize = 15))
         elif derivative_column == 'Derivative/V':
-           out.append(ax.set_ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(column), fontsize = 15))
+            out.append(ax.set_ylabel(r'$\frac{\frac{\partial %s}{\partial t}}{Volume}$'%(column), fontsize = 15))
         elif derivative_column == 'Log Derivative':
             out.append(ax.set_ylabel(r'$\frac{\partial (log(%s))}{\partial t}$'%(column), fontsize = 15))
         elif derivative_column == 'Derivative':
             out.append(ax.set_ylabel(r'$\frac{\partial %s}{\partial t}$'%(column), fontsize = 15))
         out.append(ax.legend(bbox_to_anchor=(1.05, 1),loc="upper left", borderaxespad=0.,ncol=1))
 
         return out
@@ -2925,176 +2927,176 @@
             out.append(ax.set_xlabel(x_axis, fontsize = 15))
         out.append(ax.set_ylabel('F/V', fontsize = 17))        
         out.append(ax.legend(bbox_to_anchor=(1.05, 1),loc="upper left", borderaxespad=0.,ncol=1))
 
         return out
 
 def plot_corr_lineage(df_3d, reverse_lineages, mother_cell, column = 'Fluor1 mean', method = np.var, derivative_plot = False):
-	"""
-	Function to produce three plots. The first
-	one is the correlation between the lineages
-	from the same mother cell (and same size),
-	the second one present the variance of the
-	column for each cell inside the lineages
-	easy to see if the lineages are differents,
-	and the third graph present the dV/dt, dF/dt,
-	Volume and Fluor1 mean of the lineage, and
-	if the 'derivative_plot = True', will plot the
-	lineage oscilations using 'plot_lineage_derivative()'
-
-	Parameters
-	--------------
-	df_3d : DataFrame
-		DataFrame of 3D data
-	reverse_lineage : dict
-		Dict with the lineage Cell ID's as key,
-		output from 'lineages()'
-	mother_cell : int 
-		Mother cell (first cell of the lineage),
-		to plot the lineage
-	column : str (optional)
-		The column to extract the feature of
-		the dataset. Default 'Fluor1 mean'.
-	method : function (optional)
-		Method to use to extract feature of
-		each cell, default its np.mean. Other 
-		options are np.std and stats.sem.
-	derivative_plot : bool (optional)
-		If true beside plot the dV/dt, dF/dt,
-		Volume and Fluor1 mean, will plot the
-		lineage oscilations using 'plot_lineage_derivative()'
-			
-	Returns
-	--------------
-	None
-	"""
-	root_dict, lineage_array, len_dict = longer_lineages(df_3d = df_3d,
-			     			        					 reverse_lineages = reverse_lineages,
-								    					 column = column, 
-								    					 method = method)
-
-	# pearson correlation
-	corr_arr = np.array([np.array(root_dict[mother_cell][i][:-1]) for i in root_dict[mother_cell]]) 
-	corr = np.corrcoef(corr_arr)
-
-	# plot params
-	colors = ['red', 'k', 'purple', 'gray']
-	lines = ['--','--','-.','-.']
-	lines = [Line2D([0], [0], color=colors[i], linewidth=1, linestyle=lines[i]) for i in range(len(colors))]
-	labels = [r'$\frac{dV}{dt}$', r'$\frac{dF}{dt}$', 'Volume', 'Fluor1 mean']
-
-	temp_lineage = []
-	for lineage in lineage_array:
-		if lineage[0] == mother_cell and len_dict[mother_cell] == len(lineage):
-			temp_lineage.append(lineage)
-	plot_labels = [lineage[-1] for lineage in temp_lineage[::2]]
-	lineage_plot_size = int(len(root_dict[mother_cell].keys())/2)
-	corr_plot_size = int(len(root_dict[mother_cell].keys()))
-	len_lineage = len_dict[mother_cell]
-	lineage_plot_labels = ['Cell {}'.format(cell+1) for cell in range(len_lineage)]
-	lineage_plot_keys = list(root_dict[mother_cell].keys())
-
-	# corr heatmap plot
-	fig,ax = plt.subplots(1,2, figsize = (16,5))
-	sns.heatmap(corr[::2,::2],ax=ax[0],xticklabels = plot_labels,yticklabels = plot_labels)
-	ax[0].set_title('Correlation Heatmap',fontsize = 17)
-	ax[0].set_xlabel('Lineages',fontsize = 15)
-	ax[0].set_ylabel('Lineages',fontsize = 15)
-
-	# lineage corr plot
-	ax[1].plot(root_dict[mother_cell][lineage_plot_keys[0]],'x:',color = colors[0],label='Lineage {} \nCorr: {}'.format(plot_labels[0],np.round(corr[:,0][0],2)))
-	if corr_plot_size > 2:
-		ax[1].plot(root_dict[mother_cell][lineage_plot_keys[3]],'o-.',color = colors[1],label='Lineage {} \nCorr: {}'.format(plot_labels[1],np.round(corr[:,0][3],2)))
-	if corr_plot_size > 4:
-		ax[1].plot(root_dict[mother_cell][lineage_plot_keys[5]],'*--',color = colors[2],label='Lineage {} \nCorr: {}'.format(plot_labels[2],np.round(corr[:,0][5],2)))
-	if corr_plot_size > 6:
-		ax[1].plot(root_dict[mother_cell][lineage_plot_keys[7]],'v--',color = colors[3],label='Lineage {} \nCorr: {}'.format(plot_labels[3],np.round(corr[:,0][7],2)))
-	ax[1].set_title(column,fontsize = 17)
-	ax[1].set_xticklabels(lineage_plot_labels,rotation=45)
-	ax[1].set_xticks(range(len(lineage_plot_labels)-1))
-	ax[1].set_ylabel('Fluor1 mean variance',fontsize = 15)
-	ax[1].set_xlabel('Cells',fontsize = 15)
-	ax[1].legend()
-	plt.show()
-
-	# lineage plot
-	if derivative_plot:
-		limit_plot = len(temp_lineage[::2])-1
-		fig,ax = plt.subplots(lineage_plot_size,1, figsize = (12.5,6+lineage_plot_size),constrained_layout = True)
-		fig.suptitle('Lineage of Cell {}'.format(mother_cell),fontsize = 17)
-		for idx,lineage in enumerate(temp_lineage[::2]):
-			if lineage_plot_size != 1:
-				df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Volume',order=4)
-				plot_lineage_derivative(df_lineage,extremes,plot_params,x_axis='Time (fps)',ax=ax[idx]);
-				ax[idx].set_title('')
-				if limit_plot != idx:
-					ax[idx].set_xlabel('')
-					ax[idx].set_xticks([])
-			else:
-				df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Volume',order=4)
-				plot_lineage_derivative(df_lineage,extremes,plot_params,x_axis='Time (fps)',ax=ax);
-				ax.set_title('')
-	else:
-		fig,ax = plt.subplots(lineage_plot_size,1, figsize = (12.5,3+lineage_plot_size),constrained_layout = True)
-		count,temp_min,temp_max = 0,100000,0
-		for idx,lineage in enumerate(temp_lineage[::2]):
-			if temp_max < df_3d[df_3d['Cell ID']==lineage[-2]]['Time (fps)'].values[-1]:
-				temp_max = df_3d[df_3d['Cell ID']==lineage[-2]]['Time (fps)'].values[-1]
-			if df_3d[df_3d['Cell ID']==lineage[0]]['Time (fps)'].values[0] < temp_min:
-				temp_min = df_3d[df_3d['Cell ID']==lineage[0]]['Time (fps)'].values[0]
-
-		for idx,lineage in enumerate(temp_lineage[::2]):
-			if lineage_plot_size != 1:
-				ax2 = ax[count].twinx()
-				df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Volume',order=4)
-				
-				y_axis = pre.MinMaxScaler((0,50)).fit_transform(df_lineage['Smoothed Derivative'].values.reshape(-1, 1))
-				ax[count].plot(df_lineage['Time (fps)'].values, y_axis,'--', color='red')
-				df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Fluor1 sum',order=4)
-				y_axis = pre.MinMaxScaler((0,50)).fit_transform(df_lineage['Smoothed Derivative'].values.reshape(-1, 1))
-
-				ax[count].plot(df_lineage['Time (fps)'].values, y_axis,'--', color='k')
-				ax[count].legend(lines, labels,loc='upper left',ncols = 4)
-			else:
-				ax2 = ax.twinx()
-				df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Volume',order=4)
-				
-				y_axis = pre.MinMaxScaler((0,50)).fit_transform(df_lineage['Smoothed Derivative'].values.reshape(-1, 1))
-				ax.plot(df_lineage['Time (fps)'].values, y_axis,'--', color='red')
-				
-				df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Fluor1 sum',order=4)
-				y_axis = pre.MinMaxScaler((0,50)).fit_transform(df_lineage['Smoothed Derivative'].values.reshape(-1, 1))
-
-				ax.plot(df_lineage['Time (fps)'].values, y_axis,'--', color='k')
-				ax.legend(lines, labels,loc='upper left',ncols = 4)
-
-			temp_x,temp_y,scale_y = [],[],[]
-			for cell in lineage:
-				temp_x.extend(df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values)
-				temp_y.extend(df_3d[df_3d['Cell ID']==cell]['Volume'].values)
-				scale_y.extend(df_3d[df_3d['Cell ID']==cell]['Fluor1 mean'].values)
-				# ax2.plot(df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values,df_3d[df_3d['Cell ID']==cell]['Volume'].values,
-				# 				':',color = 'brown') 
-				ax2.plot(df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values,df_3d[df_3d['Cell ID']==cell]['Fluor1 mean'].values,
-								':',color = 'gray') 
-				if lineage_plot_size != 1 and count != lineage_plot_size-1:
-					ax[count].set_xticks([])
-				ax2.set_xlim(temp_min-15,temp_max+15)
-			ax2.plot(temp_x,pre.MinMaxScaler((min(scale_y),max(scale_y))).fit_transform(np.asarray(temp_y).reshape(-1, 1)),':',color = 'purple')
-			if count != lineage_plot_size-1:
-				count +=1
-				
-		fig.text(-0.035, 0.5, r'$\frac{dV}{dt}\;and\;\frac{dF}{dt}$', va='center', rotation='vertical',fontsize = 15,zorder=2)
-		fig.text(1.02, 0.5, 'Volume and Fluor1 mean', va='center', rotation=-90,fontsize = 15,zorder=2)
-		if lineage_plot_size != 1:
-			ax[count].set_xlabel('Time (min)',fontsize = 15)
-		else:
-			ax.set_xlabel('Time (min)', fontsize = 15)
-		fig.suptitle('Lineage of Cell {}'.format(mother_cell),fontsize = 17)
-		plt.show()
+    """
+    Function to produce three plots. The first
+    one is the correlation between the lineages
+    from the same mother cell (and same size),
+    the second one present the variance of the
+    column for each cell inside the lineages
+    easy to see if the lineages are differents,
+    and the third graph present the dV/dt, dF/dt,
+    Volume and Fluor1 mean of the lineage, and
+    if the 'derivative_plot = True', will plot the
+    lineage oscilations using 'plot_lineage_derivative()'
+
+    Parameters
+    --------------
+    df_3d : DataFrame
+        DataFrame of 3D data
+    reverse_lineage : dict
+        Dict with the lineage Cell ID's as key,
+        output from 'lineages()'
+    mother_cell : int 
+        Mother cell (first cell of the lineage),
+        to plot the lineage
+    column : str (optional)
+        The column to extract the feature of
+        the dataset. Default 'Fluor1 mean'.
+    method : function (optional)
+        Method to use to extract feature of
+        each cell, default its np.mean. Other 
+        options are np.std and stats.sem.
+    derivative_plot : bool (optional)
+        If true beside plot the dV/dt, dF/dt,
+        Volume and Fluor1 mean, will plot the
+        lineage oscilations using 'plot_lineage_derivative()'
+            
+    Returns
+    --------------
+    None
+    """
+    root_dict, lineage_array, len_dict = longer_lineages(df_3d = df_3d,
+                                                            reverse_lineages = reverse_lineages,
+                                                            column = column, 
+                                                            method = method)
+
+    # pearson correlation
+    corr_arr = np.array([np.array(root_dict[mother_cell][i][:-1]) for i in root_dict[mother_cell]]) 
+    corr = np.corrcoef(corr_arr)
+
+    # plot params
+    colors = ['red', 'k', 'purple', 'gray']
+    lines = ['--','--','-.','-.']
+    lines = [Line2D([0], [0], color=colors[i], linewidth=1, linestyle=lines[i]) for i in range(len(colors))]
+    labels = [r'$\frac{dV}{dt}$', r'$\frac{dF}{dt}$', 'Volume', 'Fluor1 mean']
+
+    temp_lineage = []
+    for lineage in lineage_array:
+        if lineage[0] == mother_cell and len_dict[mother_cell] == len(lineage):
+            temp_lineage.append(lineage)
+    plot_labels = [lineage[-1] for lineage in temp_lineage[::2]]
+    lineage_plot_size = int(len(root_dict[mother_cell].keys())/2)
+    corr_plot_size = int(len(root_dict[mother_cell].keys()))
+    len_lineage = len_dict[mother_cell]
+    lineage_plot_labels = ['Cell {}'.format(cell+1) for cell in range(len_lineage)]
+    lineage_plot_keys = list(root_dict[mother_cell].keys())
+
+    # corr heatmap plot
+    fig,ax = plt.subplots(1,2, figsize = (16,5))
+    sns.heatmap(corr[::2,::2],ax=ax[0],xticklabels = plot_labels,yticklabels = plot_labels)
+    ax[0].set_title('Correlation Heatmap',fontsize = 17)
+    ax[0].set_xlabel('Lineages',fontsize = 15)
+    ax[0].set_ylabel('Lineages',fontsize = 15)
+
+    # lineage corr plot
+    ax[1].plot(root_dict[mother_cell][lineage_plot_keys[0]],'x:',color = colors[0],label='Lineage {} \nCorr: {}'.format(plot_labels[0],np.round(corr[:,0][0],2)))
+    if corr_plot_size > 2:
+        ax[1].plot(root_dict[mother_cell][lineage_plot_keys[3]],'o-.',color = colors[1],label='Lineage {} \nCorr: {}'.format(plot_labels[1],np.round(corr[:,0][3],2)))
+    if corr_plot_size > 4:
+        ax[1].plot(root_dict[mother_cell][lineage_plot_keys[5]],'*--',color = colors[2],label='Lineage {} \nCorr: {}'.format(plot_labels[2],np.round(corr[:,0][5],2)))
+    if corr_plot_size > 6:
+        ax[1].plot(root_dict[mother_cell][lineage_plot_keys[7]],'v--',color = colors[3],label='Lineage {} \nCorr: {}'.format(plot_labels[3],np.round(corr[:,0][7],2)))
+    ax[1].set_title(column,fontsize = 17)
+    ax[1].set_xticklabels(lineage_plot_labels,rotation=45)
+    ax[1].set_xticks(range(len(lineage_plot_labels)-1))
+    ax[1].set_ylabel('Fluor1 mean variance',fontsize = 15)
+    ax[1].set_xlabel('Cells',fontsize = 15)
+    ax[1].legend()
+    plt.show()
+
+    # lineage plot
+    if derivative_plot:
+        limit_plot = len(temp_lineage[::2])-1
+        fig,ax = plt.subplots(lineage_plot_size,1, figsize = (12.5,6+lineage_plot_size),constrained_layout = True)
+        fig.suptitle('Lineage of Cell {}'.format(mother_cell),fontsize = 17)
+        for idx,lineage in enumerate(temp_lineage[::2]):
+            if lineage_plot_size != 1:
+                df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Volume',order=4)
+                plot_lineage_derivative(df_lineage,extremes,plot_params,x_axis='Time (fps)',ax=ax[idx])
+                ax[idx].set_title('')
+                if limit_plot != idx:
+                    ax[idx].set_xlabel('')
+                    ax[idx].set_xticks([])
+            else:
+                df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Volume',order=4)
+                plot_lineage_derivative(df_lineage,extremes,plot_params,x_axis='Time (fps)',ax=ax)
+                ax.set_title('')
+    else:
+        fig,ax = plt.subplots(lineage_plot_size,1, figsize = (12.5,3+lineage_plot_size),constrained_layout = True)
+        count,temp_min,temp_max = 0,100000,0
+        for idx,lineage in enumerate(temp_lineage[::2]):
+            if temp_max < df_3d[df_3d['Cell ID']==lineage[-2]]['Time (fps)'].values[-1]:
+                temp_max = df_3d[df_3d['Cell ID']==lineage[-2]]['Time (fps)'].values[-1]
+            if df_3d[df_3d['Cell ID']==lineage[0]]['Time (fps)'].values[0] < temp_min:
+                temp_min = df_3d[df_3d['Cell ID']==lineage[0]]['Time (fps)'].values[0]
+
+        for idx,lineage in enumerate(temp_lineage[::2]):
+            if lineage_plot_size != 1:
+                ax2 = ax[count].twinx()
+                df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Volume',order=4)
+                
+                y_axis = pre.MinMaxScaler((0,50)).fit_transform(df_lineage['Smoothed Derivative'].values.reshape(-1, 1))
+                ax[count].plot(df_lineage['Time (fps)'].values, y_axis,'--', color='red')
+                df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Fluor1 sum',order=4)
+                y_axis = pre.MinMaxScaler((0,50)).fit_transform(df_lineage['Smoothed Derivative'].values.reshape(-1, 1))
+
+                ax[count].plot(df_lineage['Time (fps)'].values, y_axis,'--', color='k')
+                ax[count].legend(lines, labels,loc='upper left',ncols = 4)
+            else:
+                ax2 = ax.twinx()
+                df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Volume',order=4)
+                
+                y_axis = pre.MinMaxScaler((0,50)).fit_transform(df_lineage['Smoothed Derivative'].values.reshape(-1, 1))
+                ax.plot(df_lineage['Time (fps)'].values, y_axis,'--', color='red')
+                
+                df_lineage,extremes,plot_params = lineage_derivative(df_3d,temp_lineage[::2][idx],column='Fluor1 sum',order=4)
+                y_axis = pre.MinMaxScaler((0,50)).fit_transform(df_lineage['Smoothed Derivative'].values.reshape(-1, 1))
+
+                ax.plot(df_lineage['Time (fps)'].values, y_axis,'--', color='k')
+                ax.legend(lines, labels,loc='upper left',ncols = 4)
+
+            temp_x,temp_y,scale_y = [],[],[]
+            for cell in lineage:
+                temp_x.extend(df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values)
+                temp_y.extend(df_3d[df_3d['Cell ID']==cell]['Volume'].values)
+                scale_y.extend(df_3d[df_3d['Cell ID']==cell]['Fluor1 mean'].values)
+                # ax2.plot(df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values,df_3d[df_3d['Cell ID']==cell]['Volume'].values,
+                # 				':',color = 'brown') 
+                ax2.plot(df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values,df_3d[df_3d['Cell ID']==cell]['Fluor1 mean'].values,
+                                ':',color = 'gray') 
+                if lineage_plot_size != 1 and count != lineage_plot_size-1:
+                    ax[count].set_xticks([])
+                ax2.set_xlim(temp_min-15,temp_max+15)
+            ax2.plot(temp_x,pre.MinMaxScaler((min(scale_y),max(scale_y))).fit_transform(np.asarray(temp_y).reshape(-1, 1)),':',color = 'purple')
+            if count != lineage_plot_size-1:
+                count +=1
+                
+        fig.text(-0.035, 0.5, r'$\frac{dV}{dt}\;and\;\frac{dF}{dt}$', va='center', rotation='vertical',fontsize = 15,zorder=2)
+        fig.text(1.02, 0.5, 'Volume and Fluor1 mean', va='center', rotation=-90,fontsize = 15,zorder=2)
+        if lineage_plot_size != 1:
+            ax[count].set_xlabel('Time (min)',fontsize = 15)
+        else:
+            ax.set_xlabel('Time (min)', fontsize = 15)
+        fig.suptitle('Lineage of Cell {}'.format(mother_cell),fontsize = 17)
+        plt.show()
 
 def plot_distance_minima_lineage(df_3d,df_2d,lineages_list,order=9,ax = None):
     """
     Function to plot the distance between the minimas for
     an specifics lineages.
 
     Parameters
@@ -3144,350 +3146,350 @@
         out.append(ax.set_xlabel(r'Volume at birth [$\mu m^3$]',fontsize = 15))
         out.append(ax.set_ylabel(r'Volume minima [$\mu m^3$]',fontsize = 15))
         out.append(ax.legend())
 
         return out
 
 def diff_minima(df_3d,df_2d,order = 3,pre = None,pos = None, adjust = False):
-	"""
-	Function to plot the distance between the minimas of
-	the daughter and mother by the mothe volume. The 'pre' 
-	and 'pos' to be used, both must be different than 'None'.
-	It is possible to use a higher order together with adjust 
-	order for each cell, the higher the order, the higher 
-	the noise acceptance. Higher orders take longer and can 
-	reach 20 minutes to run. The value of the minimum used 
+    """
+    Function to plot the distance between the minimas of
+    the daughter and mother by the mothe volume. The 'pre' 
+    and 'pos' to be used, both must be different than 'None'.
+    It is possible to use a higher order together with adjust 
+    order for each cell, the higher the order, the higher 
+    the noise acceptance. Higher orders take longer and can 
+    reach 20 minutes to run. The value of the minimum used 
     comes from the column 'Smoothed Volume', output of
-	'lineage_derivative()'. Also, plot the histogram of 
+    'lineage_derivative()'. Also, plot the histogram of 
     the diff.
 
-	Parameters
-	--------------
-	df_3d : DataFrame
-		DataFrame of 3D data
-	df_2d : DataFrame
-		DataFrame of 2D data
-	order : int (optional)
-		The order of the polynomial used to fit the 
-		savgol_filter from scipy in 'lineage_derivative()'
-		higher order is better to find more minimas, accept
-		more noise. Default is 3.
-	pre : int (optional)
-		Save the data pre this moment in minutes
-	pos : int (optional)
-		Save the data pos this moment in minutes
-	adjust : bool (optional)
-		If true it's possible to pass a bigger order value
-		and the algorithm will adjust for each cell if 
-		needed and the order used for each cell is stored
-		in the dictionary vol_dict['order']['cell id'].
-		Default false
-	plot : bool (optional)
-		If true will plot the result of the analysis, if
-		'pre' or 'pos' is None will plot just all the data.
-
-	Returns
-	--------------
-	vol_dict : dict
-		Dictionary with the following keys 'all', 'pre',
-		'pos' with subkeys 'diff' and 'minima', 'diff' is 
-		the difference between daughter and mother volume at
-		minima and 'minima' the minima volume of the mother.
-		The key 'order' store the order used for each cell and
-		the value of 'pre' and 'pos' for plot purpose.
-	"""
-	vol_dict = {}
-	vol_dict['all'],vol_dict['pre'],vol_dict['pos'],vol_dict['order'] = {},{},{},{}
-	volume_minima,volume_minima_pos,volume_diff_pos = [],[],[]
-	volume_diff,volume_minima_pre,volume_diff_pre = [],[],[]
-	size_birth,size_birth_pre,size_birth_pos = [],[],[]
-	vol_dict['order']['pre'],vol_dict['order']['pos'] = pre,pos
-	if adjust:
-		for_range = 9
-	else:
-		for_range = 2
-
-	for cell in natsorted(df_2d['Cell ID'].values):
-		temp_order = order
-		daughter_cell1 = df_2d[df_2d['Cell ID']==cell]['Daughter1 ID'].values[0]
-		daughter_cell2 = df_2d[df_2d['Cell ID']==cell]['Daughter2 ID'].values[0]
-		
-		if len(df_3d[df_3d['Cell ID']==daughter_cell1]) > 0:
-			for attempt in range(for_range):
-				try:            
-					df,peaks,_= lineage_derivative(df_3d,[cell,daughter_cell1],order = temp_order)
-					vol_dict['order'][cell] = temp_order
-					if 0 not in list(peaks['minima'].values()):
-						temp = df['Smoothed Volume'].values[list(peaks['minima'].values())]
-						time_pre = df_3d[df_3d['Cell ID']==daughter_cell1]['Time (fps)'].values[-1]
-						time_pos = df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values[0]
-						size_birth.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
-						diff_size = temp[1]-temp[0]
-						volume_minima.append(temp[0])
-						volume_diff.append(diff_size)
-						if pre is not None and pos is not None:
-							if time_pre < pre:
-								volume_minima_pre.append(temp[0])
-								size_birth_pre.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
-								volume_diff_pre.append(diff_size)
-							elif time_pos > pos:
-								volume_minima_pos.append(temp[0])
-								size_birth_pos.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
-								volume_diff_pos.append(diff_size) 
-				except ValueError:
-					if adjust:
-						temp_order = temp_order-1
-					else:
-						continue
-			# else:
-			# 	pass
-
-		elif len(df_3d[df_3d['Cell ID']==daughter_cell2]) > 0:
-			for attempt in range(for_range):
-				try:
-					df,peaks,_= lineage_derivative(df_3d,[cell,daughter_cell2],order = temp_order)
-					vol_dict['order'][cell] = temp_order
-					if 0 not in list(peaks['minima'].values()):
-						temp = df['Smoothed Volume'].values[list(peaks['minima'].values())]
-						time_pre = df_3d[df_3d['Cell ID']==daughter_cell2]['Time (fps)'].values[-1]
-						time_pos = df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values[0]
-						size_birth.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
-						diff_size = temp[1]-temp[0]
-						volume_minima.append(temp[0])
-						volume_diff.append(diff_size)
-						if pre is not None and pos is not None:
-							if time_pre < pre:
-								volume_minima_pre.append(temp[0])
-								size_birth_pre.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
-								volume_diff_pre.append(diff_size)
-							elif time_pos > pos:
-								volume_minima_pos.append(temp[0])
-								size_birth_pos.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
-								volume_diff_pos.append(diff_size) 
-				except ValueError:
-					if adjust:
-						temp_order = temp_order-1
-					else:
-						continue
-			# else:
-			# 	pass
-    
-	vol_dict['all']['diff'],vol_dict['all']['min'],vol_dict['all']['birth'] = volume_diff,volume_minima,size_birth
-	vol_dict['pre']['diff'],vol_dict['pre']['min'],vol_dict['pre']['birth'] = volume_diff_pre,volume_minima_pre,size_birth_pre
-	vol_dict['pos']['diff'],vol_dict['pos']['min'],vol_dict['pos']['birth'] = volume_diff_pos,volume_minima_pos,size_birth_pos
+    Parameters
+    --------------
+    df_3d : DataFrame
+        DataFrame of 3D data
+    df_2d : DataFrame
+        DataFrame of 2D data
+    order : int (optional)
+        The order of the polynomial used to fit the 
+        savgol_filter from scipy in 'lineage_derivative()'
+        higher order is better to find more minimas, accept
+        more noise. Default is 3.
+    pre : int (optional)
+        Save the data pre this moment in minutes
+    pos : int (optional)
+        Save the data pos this moment in minutes
+    adjust : bool (optional)
+        If true it's possible to pass a bigger order value
+        and the algorithm will adjust for each cell if 
+        needed and the order used for each cell is stored
+        in the dictionary vol_dict['order']['cell id'].
+        Default false
+    plot : bool (optional)
+        If true will plot the result of the analysis, if
+        'pre' or 'pos' is None will plot just all the data.
+
+    Returns
+    --------------
+    vol_dict : dict
+        Dictionary with the following keys 'all', 'pre',
+        'pos' with subkeys 'diff' and 'minima', 'diff' is 
+        the difference between daughter and mother volume at
+        minima and 'minima' the minima volume of the mother.
+        The key 'order' store the order used for each cell and
+        the value of 'pre' and 'pos' for plot purpose.
+    """
+    vol_dict = {}
+    vol_dict['all'],vol_dict['pre'],vol_dict['pos'],vol_dict['order'] = {},{},{},{}
+    volume_minima,volume_minima_pos,volume_diff_pos = [],[],[]
+    volume_diff,volume_minima_pre,volume_diff_pre = [],[],[]
+    size_birth,size_birth_pre,size_birth_pos = [],[],[]
+    vol_dict['order']['pre'],vol_dict['order']['pos'] = pre,pos
+    if adjust:
+        for_range = 9
+    else:
+        for_range = 2
+
+    for cell in natsorted(df_2d['Cell ID'].values):
+        temp_order = order
+        daughter_cell1 = df_2d[df_2d['Cell ID']==cell]['Daughter1 ID'].values[0]
+        daughter_cell2 = df_2d[df_2d['Cell ID']==cell]['Daughter2 ID'].values[0]
+        
+        if len(df_3d[df_3d['Cell ID']==daughter_cell1]) > 0:
+            for attempt in range(for_range):
+                try:            
+                    df,peaks,_= lineage_derivative(df_3d,[cell,daughter_cell1],order = temp_order)
+                    vol_dict['order'][cell] = temp_order
+                    if 0 not in list(peaks['minima'].values()):
+                        temp = df['Smoothed Volume'].values[list(peaks['minima'].values())]
+                        time_pre = df_3d[df_3d['Cell ID']==daughter_cell1]['Time (fps)'].values[-1]
+                        time_pos = df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values[0]
+                        size_birth.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
+                        diff_size = temp[1]-temp[0]
+                        volume_minima.append(temp[0])
+                        volume_diff.append(diff_size)
+                        if pre is not None and pos is not None:
+                            if time_pre < pre:
+                                volume_minima_pre.append(temp[0])
+                                size_birth_pre.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
+                                volume_diff_pre.append(diff_size)
+                            elif time_pos > pos:
+                                volume_minima_pos.append(temp[0])
+                                size_birth_pos.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
+                                volume_diff_pos.append(diff_size) 
+                except ValueError:
+                    if adjust:
+                        temp_order = temp_order-1
+                    else:
+                        continue
+            # else:
+            # 	pass
+
+        elif len(df_3d[df_3d['Cell ID']==daughter_cell2]) > 0:
+            for attempt in range(for_range):
+                try:
+                    df,peaks,_= lineage_derivative(df_3d,[cell,daughter_cell2],order = temp_order)
+                    vol_dict['order'][cell] = temp_order
+                    if 0 not in list(peaks['minima'].values()):
+                        temp = df['Smoothed Volume'].values[list(peaks['minima'].values())]
+                        time_pre = df_3d[df_3d['Cell ID']==daughter_cell2]['Time (fps)'].values[-1]
+                        time_pos = df_3d[df_3d['Cell ID']==cell]['Time (fps)'].values[0]
+                        size_birth.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
+                        diff_size = temp[1]-temp[0]
+                        volume_minima.append(temp[0])
+                        volume_diff.append(diff_size)
+                        if pre is not None and pos is not None:
+                            if time_pre < pre:
+                                volume_minima_pre.append(temp[0])
+                                size_birth_pre.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
+                                volume_diff_pre.append(diff_size)
+                            elif time_pos > pos:
+                                volume_minima_pos.append(temp[0])
+                                size_birth_pos.extend(df_2d[df_2d['Cell ID']==cell]['Volume birth'].values)
+                                volume_diff_pos.append(diff_size) 
+                except ValueError:
+                    if adjust:
+                        temp_order = temp_order-1
+                    else:
+                        continue
+            # else:
+            # 	pass
+
+    vol_dict['all']['diff'],vol_dict['all']['min'],vol_dict['all']['birth'] = volume_diff,volume_minima,size_birth
+    vol_dict['pre']['diff'],vol_dict['pre']['min'],vol_dict['pre']['birth'] = volume_diff_pre,volume_minima_pre,size_birth_pre
+    vol_dict['pos']['diff'],vol_dict['pos']['min'],vol_dict['pos']['birth'] = volume_diff_pos,volume_minima_pos,size_birth_pos
 
-	return vol_dict
+    return vol_dict
 
 def plot_diff_minima(vol_dict,key = None, ax = None):
-	"""
-	Function to plot the difference between the minimas.
-	The function will plot the 'pre' and 'pos' moments
-	automatically if present in the dictionary. Also,
-	plot the histogram of the diff. It's possible to 
-	choose the key to plot ('all','pre' or 'pos'), if
-	you pass just the key will plot the cloud and the
-	histogram, if you pass the 'key' and the 'ax' will
-	return just the cloud plot. If the 'pre' os 'pos'
+    """
+    Function to plot the difference between the minimas.
+    The function will plot the 'pre' and 'pos' moments
+    automatically if present in the dictionary. Also,
+    plot the histogram of the diff. It's possible to 
+    choose the key to plot ('all','pre' or 'pos'), if
+    you pass just the key will plot the cloud and the
+    histogram, if you pass the 'key' and the 'ax' will
+    return just the cloud plot. If the 'pre' os 'pos'
     are less than 2, the function will plot just the 
     all data vector, to plot those moments you should
     pass the 'key'.
 
-	Parameters
-	--------------
-	vol_dict : dict
-		Dict with the values of the diff minima, output
-		of 'diff_minima()'.
-	key : str (optional)
-		key used to plot just one moment, 'all', 'pre'
-		or 'por'
+    Parameters
+    --------------
+    vol_dict : dict
+        Dict with the values of the diff minima, output
+        of 'diff_minima()'.
+    key : str (optional)
+        key used to plot just one moment, 'all', 'pre'
+        or 'por'
     ax : nd.array (optional)
         the ax position to plot
-	
-	Returns
-	--------------
-	None
-	"""
-	if key is not None:
-		model = LinearRegression()
-		model.fit(np.asarray(vol_dict[key]['min']).reshape(len(vol_dict[key]['min']), 1),
-					np.asarray(vol_dict[key]['diff']).reshape(len(vol_dict[key]['diff'])))
-		if ax is None:
-			fig,ax = plt.subplots(1,2, figsize = (13,5))
-
-
-			ax[0].plot(vol_dict[key]['min'],vol_dict[key]['diff'],'.')
-			ax[0].plot(vol_dict[key]['min'],model.predict(np.asarray(vol_dict[key]['min']).reshape(len(vol_dict[key]['min']), 1)),
-					'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
-			ax[0].set_title('{} the time'.format(key.capitalize()),fontsize = 17)
-			ax[0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
-			ax[0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-			ax[0].set_ylim(0,5)
-			ax[0].set_xlim(.5,5.5)
-			ax[0].legend()
-			
-			ax[1].hist(vol_dict[key]['diff']);
-			if key == 'all':
-				ax[1].set_title('{} the time'.format(key.capitalize()),fontsize = 17)
-			else:
-				ax[1].set_title('{} {} min'.format(key.capitalize(),vol_dict['order'][key]),fontsize = 17)
-			ax[1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-		else:
-			out = []
-			out.append(ax.plot(vol_dict[key]['min'],vol_dict[key]['diff'],'.'))
-			out.append(ax.plot(vol_dict[key]['min'],model.predict(np.asarray(vol_dict[key]['min']).reshape(len(vol_dict[key]['min']), 1)),
-						'gray',label = 'Coef: ' + str(model.coef_[0])[:5]))
-			out.append(ax.set_title('{} the time'.format(key.capitalize()),fontsize = 17))
-			out.append(ax.set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15))
-			out.append(ax.set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15))
-			out.append(ax.set_ylim(0,5))
-			out.append(ax.set_xlim(.5,5.5))
-			out.append(ax.legend())	
-
-			return out
-	else:	
-		if len(vol_dict['pre']['diff']) < 2 or len(vol_dict['pos']['diff']) < 2:
-			fig,ax = plt.subplots(1,2, figsize = (13,5))
-			model = LinearRegression()
-			model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
-					np.asarray(vol_dict['all']['diff']).reshape(len(vol_dict['all']['diff'])))
-
-			ax[0].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.')
-			ax[0].plot(vol_dict['all']['min'],model.predict(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1)),
-					'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
-			ax[0].set_title('All the time',fontsize = 17)
-			ax[0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
-			ax[0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-			ax[0].set_ylim(0,5)
-			ax[0].set_xlim(.5,5.5)
-			ax[0].legend()
-			
-			ax[1].hist(vol_dict['all']['diff']);
-			ax[1].set_title('All the time Histogram',fontsize = 17)
-			ax[1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)	 
-		else:
-			y_min,y_max = [],[]
-			fig,ax = plt.subplots(2,3, figsize = (17,10))
-
-			model = LinearRegression()
-			model.fit(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1),
-					np.asarray(vol_dict['pre']['diff']).reshape(len(vol_dict['pre']['diff'])))
-
-			ax[0][0].plot(vol_dict['pre']['min'],vol_dict['pre']['diff'],'.',color = 'k')
-			ax[0][0].plot(vol_dict['pre']['min'],model.predict(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1)),
-					'gray',label = 'Pre Coef: ' + str(model.coef_[0])[:5])
-			ax[0][0].set_title('Pre {} min'.format(vol_dict['order']['pre']),fontsize = 17)
-			ax[0][0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-			ax[0][0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
-			ax[0][0].set_ylim(0,5)
-			ax[0][0].set_xlim(.5,5.5)
-			ax[0][0].legend()
-
-			ax[1][0].hist(vol_dict['pre']['diff'],color = 'k');
-			ax[1][0].set_title('Pre {} Histogram'.format(vol_dict['order']['pre']),fontsize = 17)
-			ax[1][0].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-			y_min.append(ax[1][0].get_ylim()[0])
-			y_max.append(ax[1][0].get_ylim()[1])
-
-			model = LinearRegression()
-			model.fit(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1),
-					np.asarray(vol_dict['pos']['diff']).reshape(len(vol_dict['pos']['diff'])))
-
-			ax[0][1].plot(vol_dict['pos']['min'],vol_dict['pos']['diff'],'.',color = 'red')
-			ax[0][1].plot(vol_dict['pos']['min'],model.predict(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1)),
-					'gray',label = 'Pos Coef: ' + str(model.coef_[0])[:5])
-			ax[0][1].set_title('Pos {} min'.format(vol_dict['order']['pos']),fontsize = 17)
-			ax[0][1].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
-			ax[0][1].set_ylim(0,5)
-			ax[0][1].set_xlim(.5,5.5)
-			ax[0][1].legend()
-
-			ax[1][1].hist(vol_dict['pos']['diff'],color = 'red');
-			ax[1][1].set_title('Pos {} Histogram'.format(vol_dict['order']['pos']),fontsize = 17)
-			ax[1][1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-			y_min.append(ax[1][1].get_ylim()[0])
-			y_max.append(ax[1][1].get_ylim()[1])
-
-			model = LinearRegression()
-			model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
-					np.asarray(vol_dict['all']['diff']).reshape(len(vol_dict['all']['diff'])))
-
-			ax[0][2].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.')
-			ax[0][2].plot(vol_dict['all']['min'],model.predict(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1)),
-					'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
-			ax[0][2].set_title('All the time',fontsize = 17)
-			ax[0][2].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
-			ax[0][2].set_ylim(0,5)
-			ax[0][2].set_xlim(.5,5.5)
-			ax[0][2].legend()
-
-			ax[1][2].hist(vol_dict['all']['diff']);
-			ax[1][2].set_title('All the time Histogram',fontsize = 17)
-			ax[1][2].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-			y_min.append(ax[1][2].get_ylim()[0])
-			y_max.append(ax[1][2].get_ylim()[1])
-
-			ax[1][0].set_ylim(min(y_min),max(y_max)+100)
-			ax[1][1].set_ylim(min(y_min),max(y_max)+100)
-			ax[1][2].set_ylim(min(y_min),max(y_max)+100)
-			ax[1][0].set_xlim(0,5.5)
-			ax[1][1].set_xlim(0,5.5)
-			ax[1][2].set_xlim(0,5.5)
 
-			plt.tight_layout()
+    Returns
+    --------------
+    None
+    """
+    if key is not None:
+        model = LinearRegression()
+        model.fit(np.asarray(vol_dict[key]['min']).reshape(len(vol_dict[key]['min']), 1),
+                    np.asarray(vol_dict[key]['diff']).reshape(len(vol_dict[key]['diff'])))
+        if ax is None:
+            fig,ax = plt.subplots(1,2, figsize = (13,5))
+
+
+            ax[0].plot(vol_dict[key]['min'],vol_dict[key]['diff'],'.')
+            ax[0].plot(vol_dict[key]['min'],model.predict(np.asarray(vol_dict[key]['min']).reshape(len(vol_dict[key]['min']), 1)),
+                    'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
+            ax[0].set_title('{} the time'.format(key.capitalize()),fontsize = 17)
+            ax[0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
+            ax[0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
+            ax[0].set_ylim(0,5)
+            ax[0].set_xlim(.5,5.5)
+            ax[0].legend()
+            
+            ax[1].hist(vol_dict[key]['diff'])
+            if key == 'all':
+                ax[1].set_title('{} the time'.format(key.capitalize()),fontsize = 17)
+            else:
+                ax[1].set_title('{} {} min'.format(key.capitalize(),vol_dict['order'][key]),fontsize = 17)
+            ax[1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
+        else:
+            out = []
+            out.append(ax.plot(vol_dict[key]['min'],vol_dict[key]['diff'],'.'))
+            out.append(ax.plot(vol_dict[key]['min'],model.predict(np.asarray(vol_dict[key]['min']).reshape(len(vol_dict[key]['min']), 1)),
+                        'gray',label = 'Coef: ' + str(model.coef_[0])[:5]))
+            out.append(ax.set_title('{} the time'.format(key.capitalize()),fontsize = 17))
+            out.append(ax.set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15))
+            out.append(ax.set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15))
+            out.append(ax.set_ylim(0,5))
+            out.append(ax.set_xlim(.5,5.5))
+            out.append(ax.legend())	
+
+            return out
+    else:	
+        if len(vol_dict['pre']['diff']) < 2 or len(vol_dict['pos']['diff']) < 2:
+            fig,ax = plt.subplots(1,2, figsize = (13,5))
+            model = LinearRegression()
+            model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
+                    np.asarray(vol_dict['all']['diff']).reshape(len(vol_dict['all']['diff'])))
+
+            ax[0].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.')
+            ax[0].plot(vol_dict['all']['min'],model.predict(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1)),
+                    'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
+            ax[0].set_title('All the time',fontsize = 17)
+            ax[0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
+            ax[0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
+            ax[0].set_ylim(0,5)
+            ax[0].set_xlim(.5,5.5)
+            ax[0].legend()
+            
+            ax[1].hist(vol_dict['all']['diff'])
+            ax[1].set_title('All the time Histogram',fontsize = 17)
+            ax[1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)	 
+        else:
+            y_min,y_max = [],[]
+            fig,ax = plt.subplots(2,3, figsize = (17,10))
+
+            model = LinearRegression()
+            model.fit(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1),
+                    np.asarray(vol_dict['pre']['diff']).reshape(len(vol_dict['pre']['diff'])))
+
+            ax[0][0].plot(vol_dict['pre']['min'],vol_dict['pre']['diff'],'.',color = 'k')
+            ax[0][0].plot(vol_dict['pre']['min'],model.predict(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1)),
+                    'gray',label = 'Pre Coef: ' + str(model.coef_[0])[:5])
+            ax[0][0].set_title('Pre {} min'.format(vol_dict['order']['pre']),fontsize = 17)
+            ax[0][0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
+            ax[0][0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
+            ax[0][0].set_ylim(0,5)
+            ax[0][0].set_xlim(.5,5.5)
+            ax[0][0].legend()
+
+            ax[1][0].hist(vol_dict['pre']['diff'],color = 'k')
+            ax[1][0].set_title('Pre {} Histogram'.format(vol_dict['order']['pre']),fontsize = 17)
+            ax[1][0].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
+            y_min.append(ax[1][0].get_ylim()[0])
+            y_max.append(ax[1][0].get_ylim()[1])
+
+            model = LinearRegression()
+            model.fit(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1),
+                    np.asarray(vol_dict['pos']['diff']).reshape(len(vol_dict['pos']['diff'])))
+
+            ax[0][1].plot(vol_dict['pos']['min'],vol_dict['pos']['diff'],'.',color = 'red')
+            ax[0][1].plot(vol_dict['pos']['min'],model.predict(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1)),
+                    'gray',label = 'Pos Coef: ' + str(model.coef_[0])[:5])
+            ax[0][1].set_title('Pos {} min'.format(vol_dict['order']['pos']),fontsize = 17)
+            ax[0][1].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
+            ax[0][1].set_ylim(0,5)
+            ax[0][1].set_xlim(.5,5.5)
+            ax[0][1].legend()
+
+            ax[1][1].hist(vol_dict['pos']['diff'],color = 'red')
+            ax[1][1].set_title('Pos {} Histogram'.format(vol_dict['order']['pos']),fontsize = 17)
+            ax[1][1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
+            y_min.append(ax[1][1].get_ylim()[0])
+            y_max.append(ax[1][1].get_ylim()[1])
+
+            model = LinearRegression()
+            model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
+                    np.asarray(vol_dict['all']['diff']).reshape(len(vol_dict['all']['diff'])))
+
+            ax[0][2].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.')
+            ax[0][2].plot(vol_dict['all']['min'],model.predict(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1)),
+                    'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
+            ax[0][2].set_title('All the time',fontsize = 17)
+            ax[0][2].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
+            ax[0][2].set_ylim(0,5)
+            ax[0][2].set_xlim(.5,5.5)
+            ax[0][2].legend()
+
+            ax[1][2].hist(vol_dict['all']['diff'])
+            ax[1][2].set_title('All the time Histogram',fontsize = 17)
+            ax[1][2].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
+            y_min.append(ax[1][2].get_ylim()[0])
+            y_max.append(ax[1][2].get_ylim()[1])
+
+            ax[1][0].set_ylim(min(y_min),max(y_max)+100)
+            ax[1][1].set_ylim(min(y_min),max(y_max)+100)
+            ax[1][2].set_ylim(min(y_min),max(y_max)+100)
+            ax[1][0].set_xlim(0,5.5)
+            ax[1][1].set_xlim(0,5.5)
+            ax[1][2].set_xlim(0,5.5)
+
+            plt.tight_layout()
 
 def plot_distance_minima(vol_dict,key,color = None,ax=None):
-	"""
-	Function to plot the distance between the minimas.
-	The function will plot the volume minima by the 
-	volume at birth. It's necessary to pass the 'key' 
-	perform the cloud plot ('pre','pos','all').
-
-	Parameters
-	--------------
-	vol_dict : dict
-		Dict with the values of the diff minima, output
-		of 'diff_minima()'.
-	key : str (optional)
-		key used to plot just one moment, 'all', 'pre'
-		or 'por'
-	color : str (optional)
-		Cloud color
+    """
+    Function to plot the distance between the minimas.
+    The function will plot the volume minima by the 
+    volume at birth. It's necessary to pass the 'key' 
+    perform the cloud plot ('pre','pos','all').
+
+    Parameters
+    --------------
+    vol_dict : dict
+        Dict with the values of the diff minima, output
+        of 'diff_minima()'.
+    key : str (optional)
+        key used to plot just one moment, 'all', 'pre'
+        or 'por'
+    color : str (optional)
+        Cloud color
     ax : nd.array (optional)
         the ax position to plot
-	
-	Returns
-	--------------
-	None
-	"""
-	x = np.asarray(vol_dict[key]['birth'])
-	y = np.asarray(vol_dict[key]['min'])
-	model = LinearRegression()
-	model.fit(x.reshape(len(x), 1),y.reshape(len(y)))
-	if ax is None:
-		plt.plot(x,y,'.',color = color)
-		plt.plot(x,model.predict(x.reshape(len(x), 1)),'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
-		plt.xlabel(r'Volume at birth [$\mu m^3$]',fontsize = 15)
-		plt.ylabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
-		if key == 'all':
-			plt.title('{} cells'.format(key.capitalize()),fontsize = 17)
-		else:
-			plt.title('{} {} min cells'.format(key.capitalize(),vol_dict['order'][key]),fontsize = 17)
-		plt.legend()
-	else:
-		out = []
-		out.append(ax.plot(x,y,'.',color = color))
-		out.append(ax.plot(x,model.predict(x.reshape(len(x), 1)),'gray',label = 'Coef: ' + str(model.coef_[0])[:5]))
-		out.append(ax.set_xlabel(r'Volume at birth [$\mu m^3$]',fontsize = 15))
-		out.append(ax.set_ylabel(r'Volume minima [$\mu m^3$]',fontsize = 15))
-		if key == 'all':
-			out.append(ax.set_title('{} cells'.format(key.capitalize()),fontsize = 17))
-		else:
-			out.append(ax.set_title('{} {} min cells'.format(key.capitalize(),vol_dict['order'][key]),fontsize = 17))
-		out.append(ax.legend())
-		return out
+
+    Returns
+    --------------
+    None
+    """
+    x = np.asarray(vol_dict[key]['birth'])
+    y = np.asarray(vol_dict[key]['min'])
+    model = LinearRegression()
+    model.fit(x.reshape(len(x), 1),y.reshape(len(y)))
+    if ax is None:
+        plt.plot(x,y,'.',color = color)
+        plt.plot(x,model.predict(x.reshape(len(x), 1)),'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
+        plt.xlabel(r'Volume at birth [$\mu m^3$]',fontsize = 15)
+        plt.ylabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
+        if key == 'all':
+            plt.title('{} cells'.format(key.capitalize()),fontsize = 17)
+        else:
+            plt.title('{} {} min cells'.format(key.capitalize(),vol_dict['order'][key]),fontsize = 17)
+        plt.legend()
+    else:
+        out = []
+        out.append(ax.plot(x,y,'.',color = color))
+        out.append(ax.plot(x,model.predict(x.reshape(len(x), 1)),'gray',label = 'Coef: ' + str(model.coef_[0])[:5]))
+        out.append(ax.set_xlabel(r'Volume at birth [$\mu m^3$]',fontsize = 15))
+        out.append(ax.set_ylabel(r'Volume minima [$\mu m^3$]',fontsize = 15))
+        if key == 'all':
+            out.append(ax.set_title('{} cells'.format(key.capitalize()),fontsize = 17))
+        else:
+            out.append(ax.set_title('{} {} min cells'.format(key.capitalize(),vol_dict['order'][key]),fontsize = 17))
+        out.append(ax.legend())
+        return out
 
 # !pip install session-info
 # !pip install pipreqs
 # !pip install nbconvert
 # %cd code
 # !jupyter nbconvert --output-dir="./reqs" --to script 200707.ipynb
 # %cd reqs
```

### Comparing `bacteria-0.1.0/bacteria/pipeline.py` & `bacteria-0.1.1/bacteria/pipeline.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.0/bacteria.egg-info/PKG-INFO` & `bacteria-0.1.1/bacteria.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.0
+Version: 0.1.1
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.0/setup.py` & `bacteria-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.rst", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.1.0',      
+    version = '0.1.1',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
     url = 'https://github.com/tuliofalmeida/bacteria',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

