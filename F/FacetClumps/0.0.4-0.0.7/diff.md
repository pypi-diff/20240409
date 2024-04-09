# Comparing `tmp/FacetClumps-0.0.4.tar.gz` & `tmp/FacetClumps-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FacetClumps-0.0.4.tar", last modified: Fri May  5 16:27:08 2023, max compression
+gzip compressed data, was "dist\FacetClumps-0.0.7.tar", last modified: Tue Apr  9 04:06:39 2024, max compression
```

## Comparing `FacetClumps-0.0.4.tar` & `FacetClumps-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 16:27:08.958453 FacetClumps-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-05 16:27:08.915564 FacetClumps-0.0.4/FacetClumps/
--rw-rw-rw-   0        0        0      743 2023-05-05 15:06:54.000000 FacetClumps-0.0.4/FacetClumps/Detect_FacetClumps.py
--rw-rw-rw-   0        0        0      639 2023-01-28 03:02:47.000000 FacetClumps-0.0.4/FacetClumps/Detect_Files.py
--rw-rw-rw-   0        0        0     9276 2023-05-05 14:27:26.000000 FacetClumps-0.0.4/FacetClumps/Detect_Files_Funs.py
--rw-rw-rw-   0        0        0    21417 2023-05-05 16:26:42.000000 FacetClumps-0.0.4/FacetClumps/FacetClumps_2D_Funs.py
--rw-rw-rw-   0        0        0    26590 2023-05-05 14:32:47.000000 FacetClumps-0.0.4/FacetClumps/FacetClumps_3D_Funs.py
--rw-rw-rw-   0        0        0      105 2022-10-25 13:50:29.000000 FacetClumps-0.0.4/FacetClumps/Test_File.py
--rw-rw-rw-   0        0        0       76 2022-10-25 13:43:03.000000 FacetClumps-0.0.4/FacetClumps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:27:08.945487 FacetClumps-0.0.4/FacetClumps.egg-info/
--rw-rw-rw-   0        0        0      197 2023-05-05 16:27:08.000000 FacetClumps-0.0.4/FacetClumps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-05 16:27:08.000000 FacetClumps-0.0.4/FacetClumps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 16:27:08.000000 FacetClumps-0.0.4/FacetClumps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-05 16:27:08.000000 FacetClumps-0.0.4/FacetClumps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 16:27:08.955462 FacetClumps-0.0.4/FacetClumps_Code/
--rw-rw-rw-   0        0        0      639 2023-01-28 03:02:47.000000 FacetClumps-0.0.4/FacetClumps_Code/Detect_Files.py
--rw-rw-rw-   0        0        0    21494 2023-03-02 01:54:55.000000 FacetClumps-0.0.4/FacetClumps_Code/FacetClumps_2D_Funs.py
--rw-rw-rw-   0        0        0      105 2022-10-25 13:50:29.000000 FacetClumps-0.0.4/FacetClumps_Code/Test_File.py
--rw-rw-rw-   0        0        0       76 2022-10-25 13:43:03.000000 FacetClumps-0.0.4/FacetClumps_Code/__init__.py
--rw-rw-rw-   0        0        0      197 2023-05-05 16:27:08.957455 FacetClumps-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-02-28 04:15:08.000000 FacetClumps-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 16:27:08.958453 FacetClumps-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1329 2023-05-05 14:45:15.000000 FacetClumps-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 04:06:39.094068 FacetClumps-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-04-09 04:06:39.086022 FacetClumps-0.0.7/FacetClumps/
+-rw-rw-rw-   0        0        0      743 2024-04-01 11:59:44.000000 FacetClumps-0.0.7/FacetClumps/Detect_FacetClumps.py
+-rw-rw-rw-   0        0        0      639 2024-04-01 11:59:44.000000 FacetClumps-0.0.7/FacetClumps/Detect_Files.py
+-rw-rw-rw-   0        0        0    11340 2024-03-29 05:58:58.000000 FacetClumps-0.0.7/FacetClumps/Detect_Files_Funs.py
+-rw-rw-rw-   0        0        0    21697 2024-03-28 16:48:07.000000 FacetClumps-0.0.7/FacetClumps/FacetClumps_2D_Funs.py
+-rw-rw-rw-   0        0        0    26301 2024-03-28 14:41:13.000000 FacetClumps-0.0.7/FacetClumps/FacetClumps_3D_Funs.py
+-rw-rw-rw-   0        0        0      105 2022-10-25 13:50:29.000000 FacetClumps-0.0.7/FacetClumps/Test_File.py
+-rw-rw-rw-   0        0        0       76 2022-10-25 13:43:03.000000 FacetClumps-0.0.7/FacetClumps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 04:06:39.094068 FacetClumps-0.0.7/FacetClumps.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-09 04:06:38.000000 FacetClumps-0.0.7/FacetClumps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-09 04:06:38.000000 FacetClumps-0.0.7/FacetClumps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 04:06:38.000000 FacetClumps-0.0.7/FacetClumps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 04:06:38.000000 FacetClumps-0.0.7/FacetClumps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      182 2024-04-09 04:06:39.094068 FacetClumps-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-02-28 04:15:08.000000 FacetClumps-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 04:06:39.094068 FacetClumps-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1314 2024-04-09 04:04:47.000000 FacetClumps-0.0.7/setup.py
```

### Comparing `FacetClumps-0.0.4/FacetClumps/Detect_FacetClumps.py` & `FacetClumps-0.0.7/FacetClumps/Detect_FacetClumps.py`

 * *Files identical despite different names*

### Comparing `FacetClumps-0.0.4/FacetClumps/Detect_Files.py` & `FacetClumps-0.0.7/FacetClumps/Detect_Files.py`

 * *Files identical despite different names*

### Comparing `FacetClumps-0.0.4/FacetClumps/Detect_Files_Funs.py` & `FacetClumps-0.0.7/FacetClumps/Detect_Files_Funs.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,59 +3,91 @@
 import numpy as np
 import astropy.io.fits as fits
 import astropy.wcs as wcs
 from astropy.table import Table
 
 from FacetClumps import Detect_FacetClumps
 
+
 def Change_pix2word(data_header, outcat, ndim):
     """
     :param data_wcs: file header.
     :param outcat: table in pixel coordinate.
     :return:
     outcat_wcs: table in WCS coordinate.
     """
     data_header['CTYPE3'] = 'VELO'
     data_wcs = wcs.WCS(data_header)
 
     clump_Peak = outcat['Peak']
     clump_Volume = outcat['Volume']
     clump_Angle = outcat['Angle']
     clump_Edge = outcat['Edge']
-    size1, size2 = np.array([outcat['Size1'] * np.abs(data_header['CDELT1']) * 3600,
-                             outcat['Size2'] * np.abs(data_header['CDELT2']) * 3600])
+    if 'CDELT1' in data_header and 'CDELT2' in data_header:
+        size1, size2 = np.array([outcat['Size1'] * np.abs(data_header['CDELT1']) * 3600,
+                                 outcat['Size2'] * np.abs(data_header['CDELT2']) * 3600])
+    else:
+        size1, size2 = np.array([outcat['Size1'], outcat['Size2']])
+        print('The size has not converted to WCS!')
+        print('You need to transform the WCS table through the Pix table by yourself.')
     if ndim == 2:
-        # 2d result
+        # 2D result
         clump_Sum = outcat['Sum']
-        peak1, peak2 = data_wcs.all_pix2world(outcat['Peak1'], outcat['Peak2'], 1)
+        if data_wcs.world_n_dim == 2:
+            peak1, peak2 = data_wcs.all_pix2world(outcat['Peak1'], outcat['Peak2'], 1)
+            cen1, cen2 = data_wcs.all_pix2world(outcat['Cen1'], outcat['Cen2'], 1)
+        elif data_wcs.world_n_dim == 3:
+            peak1, peak2, temp_value = data_wcs.all_pix2world(outcat['Peak1'], outcat['Peak2'], 1, 1)
+            cen1, cen2, temp_value = data_wcs.all_pix2world(outcat['Cen1'], outcat['Cen2'], 1, 1)
+        else:
+            print('The data_wcs.world_n_dim is unexpected!')
         clump_Peaks = np.column_stack([peak1, peak2])
-        cen1, cen2 = data_wcs.all_pix2world(outcat['Cen1'], outcat['Cen2'], 1)
         clump_Cen = np.column_stack([cen1, cen2])
         clump_Size = np.column_stack([size1, size2])
     elif ndim == 3:
-        # 3d result
+        # 3D result
         if data_wcs.world_n_dim == 3:
             peak1, peak2, peak3 = data_wcs.all_pix2world(outcat['Peak1'], outcat['Peak2'], outcat['Peak3'], 1)
-            clump_Peaks = np.column_stack([peak1, peak2, peak3 / 1000])
             cen1, cen2, cen3 = data_wcs.all_pix2world(outcat['Cen1'], outcat['Cen2'], outcat['Cen3'], 1)
-            clump_Cen = np.column_stack([cen1, cen2, cen3 / 1000])
         elif data_wcs.world_n_dim == 4:
             peak1, peak2, peak3, temp_p = data_wcs.all_pix2world(outcat['Peak1'], outcat['Peak2'], outcat['Peak3'], 1,
                                                                  1)
-            clump_Peaks = np.column_stack([peak1, peak2, peak3 / 1000])
             cen1, cen2, cen3, temp_c = data_wcs.all_pix2world(outcat['Cen1'], outcat['Cen2'], outcat['Cen3'], 1, 1)
-            clump_Cen = np.column_stack([cen1, cen2, cen3 / 1000])
-        clump_Size = np.column_stack([size1, size2, outcat['Size3'] * data_header['CDELT3'] / 1000])
-        clump_Sum = outcat['Sum'] * data_header['CDELT3'] / 1000
+        else:
+            print('The data_wcs.world_n_dim is unexpected!')
+        if 'CDELT3' in data_header:
+            if data_header['CUNIT3'] == 'm/s' or data_header['CUNIT3'] == 'm s-1':
+                clump_Peaks = np.column_stack([peak1, peak2, peak3 / 1000])
+                clump_Cen = np.column_stack([cen1, cen2, cen3 / 1000])
+                clump_Size = np.column_stack([size1, size2, outcat['Size3'] * data_header['CDELT3'] / 1000])
+                clump_Sum = outcat['Sum'] * data_header['CDELT3'] / 1000
+            elif data_header['CUNIT3'] == 'km/s' or data_header['CUNIT3'] == 'km s-1':
+                clump_Peaks = np.column_stack([peak1, peak2, peak3])
+                clump_Cen = np.column_stack([cen1, cen2, cen3])
+                clump_Size = np.column_stack([size1, size2, outcat['Size3'] * data_header['CDELT3']])
+                clump_Sum = outcat['Sum'] * data_header['CDELT3']
+            else:
+                print('Please cheek the unit of the velocity channels (str: km/s, m/s, m s-1, km s-1, or else).')
+                print('You need to transform the WCS table through the Pix table by yourself.')
+                clump_Peaks = np.column_stack([peak1, peak2, peak3])
+                clump_Cen = np.column_stack([cen1, cen2, cen3])
+                clump_Size = np.column_stack([size1, size2, outcat['Size3']])
+                clump_Sum = outcat['Sum']
+        else:
+            print('Please cheek the key world of the velocity channels (CDELT3, or else).')
+            print('You need to transform the WCS table through the Pix table by yourself.')
+            clump_Peaks = np.column_stack([peak1, peak2, peak3])
+            clump_Cen = np.column_stack([cen1, cen2, cen3])
+            clump_Size = np.column_stack([size1, size2, outcat['Size3']])
+            clump_Sum = outcat['Sum']
     id_clumps = np.arange(1, len(clump_Peak) + 1, 1)
     outcat_wcs = np.column_stack((id_clumps, clump_Peaks, clump_Cen, clump_Size, clump_Peak,
                                   clump_Sum, clump_Volume, clump_Angle, clump_Edge))
     return outcat_wcs
 
-
 def Table_Interface(did_table, data_header, ndim):
     """
     ['ID', 'Peak1', 'Peak2', 'Peak3', 'Cen1', 'Cen2', 'Cen3', 'Size1', 'Size2', 'Size3', 'Peak', 'Sum', 'Volume', 'Angle', 'Edge'] -->3d
     ['ID', 'Peak1', 'Peak2', 'Cen1', 'Cen2',  'Size1', 'Size2', 'Peak', 'Sum', 'Volume', 'Angle', 'Edge']-->2d
     """
     Peak = did_table['peak_value']
     Sum = did_table['clump_sum']
@@ -141,15 +173,15 @@
         did_table = Detect_FacetClumps.Detect_FacetClumps_2D(RMS, Threshold, SWindow, KBins, SRecursionLB, origin_data)
     elif ndim == 3:
         did_table = Detect_FacetClumps.Detect_FacetClumps_3D(RMS, Threshold, SWindow, KBins, FwhmBeam, VeloRes,
                                                              SRecursionLBV, origin_data)
     else:
         raise Exception('Please check the dimensionality of the data!')
     if len(did_table['peak_value']) != 0:
-        np.savez(outcat_name[:-4] + '_FacetClumps_npz', did_FacetClumps=did_table)
+        # np.savez(outcat_name[:-4] + '_FacetClumps_npz', did_FacetClumps=did_table)
         regions_data = did_table['regions_data']
         fits.writeto(mask_name, regions_data, overwrite=True)
         data_header = fits.getheader(file_name)
         td_outcat, td_outcat_wcs = Table_Interface(did_table, data_header, ndim)
         td_outcat.write(outcat_name, overwrite=True)
         td_outcat_wcs.write(outcat_wcs_name, overwrite=True)
         end_1 = time.time()
```

### Comparing `FacetClumps-0.0.4/FacetClumps/FacetClumps_2D_Funs.py` & `FacetClumps-0.0.7/FacetClumps/FacetClumps_2D_Funs.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,23 +19,23 @@
         threshold = filters.threshold_otsu(origin_data)
     else:
         threshold = threshold
     open_data = morphology.opening(origin_data > threshold,morphology.disk(kopen_radius))
     if temp_array.ndim != 2:
         dilation_data = morphology.dilation(open_data,morphology.disk(kopen_radius))
         dilation_data = dilation_data*(origin_data > threshold)
-#         dilation_label = measure.label(dilation_data,connectivity=1)
+        dilation_label = measure.label(dilation_data,connectivity=1)
     elif temp_array.ndim == 2:
         dilation_data = morphology.dilation(temp_array>0,morphology.disk(kopen_radius))
         dilation_data = dilation_data*(origin_data > RMS)
         xor_data = np.logical_xor(temp_array>0, dilation_data)
         and_data = np.logical_and(origin_data < threshold, xor_data)
         dilation_data = np.logical_or(temp_array,and_data)
 #     dilation_data_1 = ndimage.binary_fill_holes(dilation_data_1)
-    dilation_label = measure.label(dilation_data,connectivity=1)
+        dilation_label = measure.label(dilation_data,connectivity=2)
     regions = measure.regionprops(dilation_label)
     regions_array = dilation_label
     return regions,regions_array
 
 def Convolve(origin_data,SWindow):
     s = SWindow/2
     t = 17/5
@@ -147,30 +147,31 @@
     for final_region in regions_record:
         if len(final_region[:,0])> label_area_min:
             x_region = final_region[:,0]
             y_region = final_region[:,1]
             od_mass = origin_data[x_region,y_region]
             center_of_mass.append(np.around((np.c_[od_mass,od_mass]*final_region).sum(0)\
                 /od_mass.sum(),3).tolist())
-    center_of_mass = np.array(center_of_mass)
     return center_of_mass
 
 def Get_Total_COM(origin_data,regions,convs,kbins,SRecursionLB):
     keig_bins = -1
     recursion_time = 0
     regions_record = []
     for i in tqdm(range(len(regions))):
         coords = regions[i].coords
         region = np.c_[coords[:,0],coords[:,1]]
-        lnV = np.int(np.log(len(coords)))
+        lnV = np.int64(np.log(len(coords)))
         logV = np.log10(len(coords))
         bins = kbins*lnV
         eigenvalue = Calculate_Eig(origin_data,convs,region)
         regions_record = Recursion_Lable(origin_data,convs,region,regions_record,eigenvalue,lnV,logV,bins,keig_bins,SRecursionLB,recursion_time)
     com = Get_COM(origin_data,regions_record)
+    sorted_id_com = sorted(range(len(com)), key=lambda k: com[k], reverse=False)
+    com = (np.array(com)[sorted_id_com])
     return com
 
 def GNC_FacetClumps(core_data,cores_coordinate):
     xres,yres = core_data.shape
     x_center = cores_coordinate[0]+1
     y_center = cores_coordinate[1]+1
     x_arange = np.arange(max(0,x_center-1),min(xres,x_center+2))
@@ -189,15 +190,15 @@
     i_record = []
     temp_rc_dict = {}
     rc_dict = {}
     new_regions = []
     temp_regions_array = np.zeros_like(regions_array)
     for i in range(1,np.int(regions_array.max()+1)):
         temp_rc_dict[i] = []
-    center = np.array(com,dtype = 'uint16')
+    center = np.array(np.around(com),dtype = 'uint16')
     for cent in center:
         if regions_array[cent[0],cent[1]] != 0 :
             temp_rc_dict[regions_array[cent[0],cent[1]]].append(com[k1])
             i_record.append(regions_array[cent[0],cent[1]])
         k1 += 1
     for i in range(1,np.int(regions_array.max())+1):
         if i in i_record:
@@ -270,97 +271,107 @@
     box_data = np.zeros([x_max-x_min+2,y_max-y_min+2])
     box_data[i_region[:,0]-x_min,i_region[:,1]-y_min] = 1
     box_data[j_region[:,0]-x_min,j_region[:,1]-y_min] = 1
     box_label = measure.label(box_data,connectivity=2)
     box_region = measure.regionprops(box_label)
     return len(box_region)
 
-def Delect(new_peak_dict,new_core_dict,peak_dict_center,core_dict_center,key_peak_record,near_k_2,origin_data):
+def Delect(new_peak_dict,new_core_dict,com_dict,core_dict_center,key_peak_record,near_k_2,origin_data):
     for key_peak in key_peak_record:
-        dist = Dists_Array([new_peak_dict[key_peak]], list(peak_dict_center.values()))
+        dist = Dists_Array([new_peak_dict[key_peak]], list(com_dict.values()))
         dist_index_sort = np.argsort(dist[0])
-        pdc_sort = np.array(list(peak_dict_center.keys()))[dist_index_sort]
+        pdc_sort = np.array(list(com_dict.keys()))[dist_index_sort]
         i_num = key_peak
         for key_center in pdc_sort[:near_k_2]:
             j_num = key_center
             connectivity_1 = Connectivity_FacetClumps(new_core_dict,core_dict_center,i_num,j_num)
             if connectivity_1 == 1:
                 core_dict_center[key_center] += new_core_dict[key_peak]
                 del new_core_dict[key_peak]
                 del new_peak_dict[key_peak]
                 break
 
-def Update_CP_Dict_FacetClumps(new_peak_dict,peak_dict_center,new_core_dict,mountain_array,origin_data):
-    peak_dict_temp = {}
+
+def Update_CP_Dict_FacetClumps(new_peak_dict, com_dict, new_core_dict, mountain_array, origin_data):
+    com_dict_temp = {}
     core_dict_center = {}
     key_mountain_record = []
     center_mountain = {}
     new_peak_dict_2 = {}
     for key in new_peak_dict.keys():
         new_peak_dict_2[key] = new_peak_dict[key]
-    for key_center in peak_dict_center.keys():
-        peak_coord = peak_dict_center[key_center]
-        peak_coord = np.array(np.around(peak_coord,0),dtype = 'uint16')
-        if mountain_array[peak_coord[0],peak_coord[1]]!=0:
-            key_mountain = mountain_array[peak_coord[0],peak_coord[1]]
+    for key_center in com_dict.keys():
+        peak_coord = com_dict[key_center]
+        peak_coord = np.array(np.around(peak_coord, 0), dtype='uint16')
+        if mountain_array[peak_coord[0], peak_coord[1]] != 0:
+            key_mountain = mountain_array[peak_coord[0], peak_coord[1]]
         if key_mountain not in key_mountain_record:
-            peak_dict_temp[key_center] = peak_dict_center[key_center]
+            com_dict_temp[key_center] = com_dict[key_center]
             core_dict_center[key_center] = new_core_dict[key_mountain]
             center_mountain[key_mountain] = key_center
             key_mountain_record.append(key_mountain)
             del new_core_dict[key_mountain]
             del new_peak_dict[key_mountain]
         else:
-            old_center = peak_dict_temp[center_mountain[key_mountain]]
-            new_center = peak_dict_center[key_center]
+            old_center = com_dict_temp[center_mountain[key_mountain]]
+            new_center = com_dict[key_center]
             dist_1 = Dists_Array([old_center], [new_peak_dict_2[key_mountain]])[0][0]
             dist_2 = Dists_Array([new_center], [new_peak_dict_2[key_mountain]])[0][0]
-            if dist_2<dist_1:
-                peak_dict_temp[center_mountain[key_mountain]] = peak_dict_center[key_center]
-    peak_dict_center = peak_dict_temp
+            if dist_2 < dist_1:
+                com_dict_temp[center_mountain[key_mountain]] = com_dict[key_center]
+    com_dict = com_dict_temp
     near_k_1 = 1
     near_k_2 = 1
-    while len(new_core_dict)>0:
-        if len(new_core_dict)>len(peak_dict_center.keys()):
-            for key_center in peak_dict_center.keys():
-                if len(new_core_dict)>0:
-                    distance = Dists_Array([peak_dict_center[key_center]], list(new_peak_dict.values()))
+    flag = 0
+    while len(new_core_dict) > 0:
+        remaining_len = len(new_core_dict)
+        if len(new_core_dict) > len(com_dict.keys()):
+            for key_center in com_dict.keys():
+                if len(new_core_dict) > 0:
+                    distance = Dists_Array([com_dict[key_center]], list(new_peak_dict.values()))
                     distance_index_sort = np.argsort(distance[0])
                     npd_sort = np.array(list(new_peak_dict.keys()))[distance_index_sort]
                     key_peak_record = npd_sort[:near_k_2]
-                    Delect(new_peak_dict,new_core_dict,peak_dict_center,core_dict_center,key_peak_record,near_k_2,origin_data)
+                    Delect(new_peak_dict, new_core_dict, com_dict, core_dict_center, key_peak_record, near_k_2,
+                           origin_data)
         else:
             key_peak_record = np.array(list(new_peak_dict.keys()))
-            Delect(new_peak_dict,new_core_dict,peak_dict_center,core_dict_center,key_peak_record,near_k_1,origin_data)
+            Delect(new_peak_dict, new_core_dict, com_dict, core_dict_center, key_peak_record, near_k_1, origin_data)
+
+        if remaining_len == len(new_core_dict):
+            if remaining_len == remaining_len:
+                #                 print('Remaining Length:',remaining_len)
+                break
+            flag = remaining_len
         temp_near_k = near_k_2
         near_k_2 = near_k_1
         near_k_1 += temp_near_k
-    return peak_dict_temp,core_dict_center
+    return com_dict_temp, core_dict_center
 
 def Get_CP_Dict(rc_dict,mountain_array,mountain_dict,peak_dict,region_mp_dict,origin_data):
     core_id = 0
-    peak_dict_record = {}
+    com_dict_record = {}
     core_dict_record = {}
     for key in tqdm(rc_dict.keys()):
         new_peak_dict = {}
-        peak_dict_center = {}
+        com_dict = {}
         new_core_dict = {}
         mountain_keys = region_mp_dict[key]
         com_FacetClumpss = rc_dict[key]
         for mountain_key in mountain_keys:
             new_peak_dict[mountain_key] = peak_dict[mountain_key][0]
             new_core_dict[mountain_key] = mountain_dict[mountain_key]
         for com_FacetClumps in com_FacetClumpss:
-            peak_dict_center[core_id] = com_FacetClumps.tolist()
+            com_dict[core_id] = com_FacetClumps.tolist()
             core_id += 1
-        peak_dict_temp,core_dict_center = Update_CP_Dict_FacetClumps(new_peak_dict,peak_dict_center,new_core_dict,mountain_array,origin_data)
+        com_dict_temp,core_dict_center = Update_CP_Dict_FacetClumps(new_peak_dict,com_dict,new_core_dict,mountain_array,origin_data)
         for key_center in core_dict_center.keys():
-            peak_dict_record[key_center] = peak_dict_temp[key_center]
+            com_dict_record[key_center] = com_dict_temp[key_center]
             core_dict_record[key_center] = core_dict_center[key_center]
-    return peak_dict_record,core_dict_record
+    return com_dict_record,core_dict_record
 
 def Get_DV(box_data,box_center):
     #2D
     box_region = np.where(box_data!= 0)
     A11 = np.sum((box_region[0]-box_center[0])**2*\
         box_data[box_region])
     A12 = -np.sum((box_region[0]-box_center[0])*\
@@ -391,23 +402,24 @@
     clump_volume = []
     clump_angle = []
     clump_regions = []
     clump_edge = []
     detect_infor_dict = {}
     k = 0
     regions_data = np.zeros_like(origin_data)
+    data_size = origin_data.shape
     for key in center_dict.keys():
-        k += 1
         core_x = np.array(core_dict[key])[:,0]
         core_y = np.array(core_dict[key])[:,1]
         core_x_min = core_x.min()
         core_x_max = core_x.max()
         core_y_min = core_y.min()
         core_y_max = core_y.max()
         if len(core_dict[key])>SRecursionLB:
+            k += 1
             temp_core = np.zeros((core_x_max-core_x_min+1,core_y_max-core_y_min+1))
             temp_core[core_x-core_x_min,core_y-core_y_min]=origin_data[core_x,core_y]
             temp_center = [center_dict[key][0]-core_x_min,center_dict[key][1]-core_y_min]
             D,V,size_ratio,angle = Get_DV(temp_core,temp_center)
             peak_coord = np.where(temp_core == temp_core.max())
             peak_coord = [(peak_coord[0]+core_x_min)[0],(peak_coord[1]+core_y_min)[0]]
             peak_value.append(origin_data[peak_coord[0],peak_coord[1]])
@@ -422,15 +434,14 @@
                            ((mass_array*np.array(core_dict[key])).sum(0)/od_mass.sum())**2)
             clump_size.append(size.tolist())
             clump_sum.append(origin_data[core_x,core_y].sum())
             clump_volume.append(len(core_dict[key]))
             clump_angle.append(angle)
             regions_data[core_x,core_y] = k
             clump_regions.append([np.array(core_dict[key])[:,0],np.array(core_dict[key])[:,1]])
-            data_size = origin_data.shape
             if core_x_min == 0 or core_y_min == 0 or \
                 core_x_max+1 == data_size[0] or core_y_max+1 == data_size[1]:
                 clump_edge.append(1)
             else:
                 clump_edge.append(0)
     detect_infor_dict['peak_value'] = np.around(peak_value,3).tolist()
     detect_infor_dict['peak_location'] = peak_location
@@ -450,13 +461,13 @@
     regions_1,regions_array_1 = Get_Regions_FacetClumps(origin_data,RMS,Threshold,np.array([0]))
     convs,hook_face = Convolve(origin_data*regions_array_1,SWindow)
     com = Get_Total_COM(hook_face,regions_1,convs,KBins,SRecursionLB)
     new_regions_1,regions_array_1,rc_dict = Build_RC_Dict(com,regions_array_1,regions_1)
     regions_2,regions_array_2 = Get_Regions_FacetClumps(origin_data,RMS,Threshold,regions_array_1)
     new_regions_2,regions_array_2,rc_dict = Build_RC_Dict(com,regions_array_2,regions_2)
     mountain_array,mountain_dict,peak_dict,region_mp_dict = Build_MPR_Dict(origin_data,new_regions_2)
-    peak_dict_record,core_dict_record = Get_CP_Dict(rc_dict,mountain_array,mountain_dict,peak_dict,region_mp_dict,origin_data)
-    detect_infor_dict = DID_FacetClumps(SRecursionLB,peak_dict_record,core_dict_record,origin_data)
+    com_dict_record,core_dict_record = Get_CP_Dict(rc_dict,mountain_array,mountain_dict,peak_dict,region_mp_dict,origin_data)
+    detect_infor_dict = DID_FacetClumps(SRecursionLB,com_dict_record,core_dict_record,origin_data)
     return detect_infor_dict
```

### Comparing `FacetClumps-0.0.4/FacetClumps/FacetClumps_3D_Funs.py` & `FacetClumps-0.0.7/FacetClumps/FacetClumps_3D_Funs.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 #         dilation_data_1 = ndimage.binary_fill_holes(dilation_data_1)
         dilation_label = measure.label(dilation_data,connectivity=3)
     regions = measure.regionprops(dilation_label)
     regions_array = dilation_label
     return regions,regions_array
 
 def Convolve(origin_data,SWindow):
-    s = np.int(SWindow/2)
+    s = np.int64(SWindow/2)
     L = 0
     xres, yres, zres = np.mgrid[0:SWindow:1,0:SWindow:1,0:SWindow:1]
     xyz = np.column_stack([xres.flat, yres.flat, zres.flat])
     sigma = np.array([s,s,s])
     covariance = np.diag(sigma**2)
     center = [s,s,s]
     prob_density = multivariate_normal.pdf(xyz, mean=center, cov=covariance)
@@ -212,15 +212,15 @@
 def Get_Total_COM(origin_data,regions,convs,kbins,SRecursionLBV):
     keig_bins = -1
     recursion_time = 0
     regions_record = []
     for i in tqdm(range(len(regions))):
         coords = regions[i].coords
         region = np.c_[coords[:,0],coords[:,1],coords[:,2]]
-        lnV = np.int(np.log(len(coords)))
+        lnV = np.int64(np.log(len(coords)))
         logV = np.log10(len(coords))
         bins = kbins*lnV
         eigenvalue = Calculate_Eig(origin_data,convs,region)
         regions_record = Recursion_Lable(origin_data,convs,region,regions_record,eigenvalue,lnV,logV,bins,keig_bins,SRecursionLBV,recursion_time)
     com = Get_COM(origin_data,regions_record)
     return com
 
@@ -244,23 +244,23 @@
     k1 = 0
     k2 = 0
     i_record = []
     temp_rc_dict = {}
     rc_dict = {}
     new_regions = []
     temp_regions_array = np.zeros_like(regions_array)
-    for i in range(1,np.int(regions_array.max()+1)):
+    for i in range(1,np.int64(regions_array.max()+1)):
         temp_rc_dict[i] = []
     center = np.array(np.around(com,0),dtype = 'uint16')
     for cent in center:
         if regions_array[cent[0],cent[1],cent[2]] != 0 :
             temp_rc_dict[regions_array[cent[0],cent[1],cent[2]]].append(com[k1])
             i_record.append(regions_array[cent[0],cent[1],cent[2]])
         k1 += 1
-    for i in range(1,np.int(regions_array.max())+1):
+    for i in range(1,np.int64(regions_array.max())+1):
         if i in i_record:
             coordinates = regions_first[i-1].coords
             temp_regions_array[(coordinates[:,0],coordinates[:,1],coordinates[:,2])] = 1
             new_regions.append(regions_first[i-1])
             rc_dict[k2] = temp_rc_dict[i]
             k2 += 1
     return new_regions,temp_regions_array,rc_dict
@@ -340,98 +340,98 @@
     box_data = np.zeros([x_max-x_min+2,y_max-y_min+2,z_max-z_min+2])
     box_data[i_region[:,0]-x_min,i_region[:,1]-y_min,i_region[:,2]-z_min] = 1
     box_data[j_region[:,0]-x_min,j_region[:,1]-y_min,j_region[:,2]-z_min] = 1
     box_label = measure.label(box_data,connectivity=3)
     box_region = measure.regionprops(box_label)
     return len(box_region)
 
-def Delect(FwhmBeam,VeloRes,new_peak_dict,new_core_dict,peak_dict_center,core_dict_center,key_peak_record,near_k_2,origin_data):
+def Delect(FwhmBeam,VeloRes,new_peak_dict,new_core_dict,com_dict,core_dict_center,key_peak_record,near_k_2,origin_data):
     for key_peak in key_peak_record:
-        dist = Dists_Array_Weighted(FwhmBeam,VeloRes,[new_peak_dict[key_peak]], list(peak_dict_center.values()))
+        dist = Dists_Array_Weighted(FwhmBeam,VeloRes,[new_peak_dict[key_peak]], list(com_dict.values()))
         dist_index_sort = np.argsort(dist[0])
-        pdc_sort = np.array(list(peak_dict_center.keys()))[dist_index_sort]
+        pdc_sort = np.array(list(com_dict.keys()))[dist_index_sort]
         i_num = key_peak
         for key_center in pdc_sort[:near_k_2]:
             j_num = key_center
             connectivity_1 = Connectivity_FacetClumps(new_core_dict,core_dict_center,i_num,j_num)
             if connectivity_1 == 1:
                 core_dict_center[key_center] += new_core_dict[key_peak]
                 del new_core_dict[key_peak]
                 del new_peak_dict[key_peak]
                 break
 
-def Update_CP_Dict_FacetClumps(FwhmBeam,VeloRes,new_peak_dict,peak_dict_center,new_core_dict,mountain_array,origin_data):
-    peak_dict_temp = {}
+def Update_CP_Dict_FacetClumps(FwhmBeam,VeloRes,new_peak_dict,com_dict,new_core_dict,mountain_array,origin_data):
+    com_dict_temp = {}
     core_dict_center = {}
     key_mountain_record = []
     center_mountain = {}
     new_peak_dict_2 = {}
     for key in new_peak_dict.keys():
         new_peak_dict_2[key] = new_peak_dict[key]
-    for key_center in peak_dict_center.keys():
-        peak_coord = peak_dict_center[key_center]
-        peak_coord = np.array(np.around(peak_coord,0),dtype = 'uint16')
-        if mountain_array[peak_coord[0],peak_coord[1],peak_coord[2]]!=0:
-            key_mountain = mountain_array[peak_coord[0],peak_coord[1],peak_coord[2]]
+    for key_center in com_dict.keys():
+        com_coord = com_dict[key_center]
+        com_coord = np.array(np.around(com_coord,0),dtype = 'uint16')
+        if mountain_array[com_coord[0],com_coord[1],com_coord[2]]!=0:
+            key_mountain = mountain_array[com_coord[0],com_coord[1],com_coord[2]]
         if key_mountain not in key_mountain_record:
-            peak_dict_temp[key_center] = peak_dict_center[key_center]
+            com_dict_temp[key_center] = com_dict[key_center]
             core_dict_center[key_center] = new_core_dict[key_mountain]
             center_mountain[key_mountain] = key_center
             key_mountain_record.append(key_mountain)
             del new_core_dict[key_mountain]
             del new_peak_dict[key_mountain]
         else:
-            old_center = peak_dict_temp[center_mountain[key_mountain]]
-            new_center = peak_dict_center[key_center]
+            old_center = com_dict_temp[center_mountain[key_mountain]]
+            new_center = com_dict[key_center]
             dist_1 = Dists_Array_Weighted(FwhmBeam,VeloRes,[old_center], [new_peak_dict_2[key_mountain]])[0][0]
             dist_2 = Dists_Array_Weighted(FwhmBeam,VeloRes,[new_center], [new_peak_dict_2[key_mountain]])[0][0]
             if dist_2<dist_1:
-                peak_dict_temp[center_mountain[key_mountain]] = peak_dict_center[key_center]
-    peak_dict_center = peak_dict_temp
+                com_dict_temp[center_mountain[key_mountain]] = com_dict[key_center]
+    com_dict = com_dict_temp
     near_k_1 = 1
     near_k_2 = 1
     while len(new_core_dict)>0:
-        if len(new_core_dict)>len(peak_dict_center.keys()):
-            for key_center in peak_dict_center.keys():
+        if len(new_core_dict)>len(com_dict.keys()):
+            for key_center in com_dict.keys():
                 if len(new_core_dict)>0:
-                    distance = Dists_Array_Weighted(FwhmBeam,VeloRes,[peak_dict_center[key_center]], list(new_peak_dict.values()))
+                    distance = Dists_Array_Weighted(FwhmBeam,VeloRes,[com_dict[key_center]], list(new_peak_dict.values()))
                     distance_index_sort = np.argsort(distance[0])
                     npd_sort = np.array(list(new_peak_dict.keys()))[distance_index_sort]
                     key_peak_record = npd_sort[:near_k_2]
-                    Delect(FwhmBeam,VeloRes,new_peak_dict,new_core_dict,peak_dict_center,core_dict_center,key_peak_record,near_k_2,origin_data)
+                    Delect(FwhmBeam,VeloRes,new_peak_dict,new_core_dict,com_dict,core_dict_center,key_peak_record,near_k_2,origin_data)
         else:
             key_peak_record = np.array(list(new_peak_dict.keys()))
-            Delect(FwhmBeam,VeloRes,new_peak_dict,new_core_dict,peak_dict_center,core_dict_center,key_peak_record,near_k_1,origin_data)
+            Delect(FwhmBeam,VeloRes,new_peak_dict,new_core_dict,com_dict,core_dict_center,key_peak_record,near_k_1,origin_data)
         temp_near_k = near_k_2
         near_k_2 = near_k_1
         near_k_1 += temp_near_k
-    return peak_dict_temp,core_dict_center
+    return com_dict_temp,core_dict_center
 
 def Get_CP_Dict(FwhmBeam,VeloRes,rc_dict,mountain_array,mountain_dict,peak_dict,region_mp_dict,origin_data):
     core_id = 0
-    peak_dict_record = {}
+    com_dict_record = {}
     core_dict_record = {}
     for key in tqdm(np.array(list(rc_dict.keys()))):
         new_peak_dict = {}
         peak_dict_center = {}
         new_core_dict = {}
         mountain_keys = region_mp_dict[key]
         com_FacetClumpss = rc_dict[key]
         for mountain_key in mountain_keys:
             new_peak_dict[mountain_key] = peak_dict[mountain_key][0]
             new_core_dict[mountain_key] = mountain_dict[mountain_key]
         for com_FacetClumps in com_FacetClumpss:
             peak_dict_center[core_id] = com_FacetClumps.tolist()
             core_id += 1
-        peak_dict_temp,core_dict_center = \
+        com_dict_temp,core_dict_center = \
             Update_CP_Dict_FacetClumps(FwhmBeam,VeloRes,new_peak_dict,peak_dict_center,new_core_dict,mountain_array,origin_data)
         for key_center in core_dict_center.keys():
-            peak_dict_record[key_center] = peak_dict_temp[key_center]
+            com_dict_record[key_center] = com_dict_temp[key_center]
             core_dict_record[key_center] = core_dict_center[key_center]
-    return peak_dict_record,core_dict_record
+    return com_dict_record,core_dict_record
 
 def Get_DV(box_data,box_center):
     box_data_sum = box_data.sum(0)
     box_region = np.where(box_data_sum!= 0)
     A11 = np.sum((box_region[0]-box_center[1])**2*\
         box_data_sum[box_region])
     A12 = -np.sum((box_region[0]-box_center[1])*\
@@ -455,20 +455,20 @@
     peak_value = []
     peak_location = []
     clump_center=[]
     clump_com = []
     clump_size = []
     clump_sum = []
     clump_volume = []
-    clump_regions = []
     clump_edge = []
     clump_angle = []
     detect_infor_dict = {}
     k = 0
     regions_data = np.zeros_like(origin_data)
+    data_size = origin_data.shape
     for key in center_dict.keys():
         core_x = np.array(core_dict[key])[:,0]
         core_y = np.array(core_dict[key])[:,1]
         core_z = np.array(core_dict[key])[:,2]
         coords_range,lb_area,v_delta,box_data = Get_LBV_Table(np.array(core_dict[key]))
         core_x_min, core_x_max = coords_range[0],coords_range[1]
         core_y_min, core_y_max = coords_range[2],coords_range[3]
@@ -492,16 +492,14 @@
             size = np.sqrt((mass_array*(np.array(core_dict[key])**2)).sum(0)/od_mass.sum()-\
                            ((mass_array*np.array(core_dict[key])).sum(0)/od_mass.sum())**2)
             clump_size.append(size.tolist())
             clump_sum.append(origin_data[core_x,core_y,core_z].sum())
             clump_volume.append(len(core_dict[key]))
             clump_angle.append(angle)
             regions_data[core_x,core_y,core_z] = k
-            clump_regions.append([np.array(core_dict[key])[:,0],np.array(core_dict[key])[:,1],np.array(core_dict[key])[:,2]])
-            data_size = origin_data.shape
             if core_x_min == 0 or core_y_min == 0 or core_z_min == 0 or \
                 core_x_max+1 == data_size[0] or core_y_max+1 == data_size[1] or core_z_max+1 == data_size[2]:
                 clump_edge.append(1)
             else:
                 clump_edge.append(0)
     detect_infor_dict['peak_value'] = np.around(peak_value,3).tolist()
     detect_infor_dict['peak_location'] = peak_location
@@ -524,10 +522,12 @@
     convs,hook_face = Convolve(origin_data*regions_array_1,SWindow)
     com = Get_Total_COM(hook_face,regions_1,convs,KBins,SRecursionLBV)
     new_regions_1,regions_array_1,rc_dict = Build_RC_Dict(com,regions_array_1,regions_1)
     regions_2,regions_array_2 = Get_Regions_FacetClumps(origin_data,RMS,Threshold,regions_array_1)
     new_regions_2,regions_array_2,rc_dict = Build_RC_Dict(com,regions_array_2,regions_2)
     mountain_array,mountain_dict,peak_dict,region_mp_dict = Build_MPR_Dict(origin_data,new_regions_2)
     peak_dict = Updata_Peak_Dict(origin_data,mountain_dict,peak_dict)
-    peak_dict_record,core_dict_record = Get_CP_Dict(FwhmBeam,VeloRes,rc_dict,mountain_array,mountain_dict,peak_dict,region_mp_dict,origin_data)
-    detect_infor_dict = DID_FacetClumps(SRecursionLBV,peak_dict_record,core_dict_record,origin_data)
+    com_dict_record,core_dict_record = Get_CP_Dict(FwhmBeam,VeloRes,rc_dict,mountain_array,mountain_dict,peak_dict,region_mp_dict,origin_data)
+    detect_infor_dict = DID_FacetClumps(SRecursionLBV,com_dict_record,core_dict_record,origin_data)
     return detect_infor_dict
+
+
```

### Comparing `FacetClumps-0.0.4/setup.py` & `FacetClumps-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FacetClumps',  # 包名
-    version='0.0.4',  # 版本 0.3, 0.0.3
-    description="FacetClumps: A molecular cloud clump detection algorithm based on Facet model",  # 包简介
+    version='0.0.7',  # 版本 0.3, 0.0.4
+    description="FacetClumps: A Facet-based Molecular Clump Detection Algorithm",  # 包简介
     # long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     # include_package_data=True,  # 是否允许上传资源文件
     author='Jiang Yu',  # 作者
     author_email="yujiang@pmo.ac.cn",  # 作者邮件
     # maintainer='',  # 维护者
     # maintainer_email="yujiang@pmo.ac.cn",  # 维护者邮件
     # license='MIT License',  # 协议
```

