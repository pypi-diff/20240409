# Comparing `tmp/warmth-0.0.1.tar.gz` & `tmp/warmth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warmth-0.0.1.tar", max compression
+gzip compressed data, was "warmth-0.0.2.tar", max compression
```

## Comparing `warmth-0.0.1.tar` & `warmth-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     7652 2023-12-12 12:34:10.844993 warmth-0.0.1/LICENSE.md
--rw-r--r--   0        0        0     1286 2023-12-12 12:34:10.844993 warmth-0.0.1/README.md
--rw-r--r--   0        0        0      798 2023-12-12 12:34:10.884993 warmth-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       87 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/__init__.py
--rw-r--r--   0        0        0    33866 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/build.py
--rw-r--r--   0        0        0    44794 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/data/haq87.json
--rw-r--r--   0        0        0    39680 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/data.py
--rw-r--r--   0        0        0    78638 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/forward_modelling.py
--rw-r--r--   0        0        0      284 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/logging.py
--rw-r--r--   0        0        0    68063 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/mesh_model.py
--rw-r--r--   0        0        0     7951 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/mesh_utils.py
--rw-r--r--   0        0        0     1991 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/model.py
--rw-r--r--   0        0        0    10952 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/parameters.py
--rw-r--r--   0        0        0    14074 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/postprocessing.py
--rw-r--r--   0        0        0    20666 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/resqpy_helpers.py
--rw-r--r--   0        0        0     8290 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/simulator.py
--rw-r--r--   0        0        0     4255 2023-12-12 12:34:10.896993 warmth-0.0.1/warmth/utils.py
--rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 warmth-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-04-09 10:10:23.254884 warmth-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1286 2024-04-09 10:10:23.254884 warmth-0.0.2/README.md
+-rw-r--r--   0        0        0      837 2024-04-09 10:10:52.983189 warmth-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/__init__.py
+-rw-r--r--   0        0        0    33895 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/build.py
+-rw-r--r--   0        0        0    44794 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/data/haq87.json
+-rw-r--r--   0        0        0    39680 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/data.py
+-rw-r--r--   0        0        0    78689 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/forward_modelling.py
+-rw-r--r--   0        0        0      284 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/logging.py
+-rw-r--r--   0        0        0    78829 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/mesh_model.py
+-rw-r--r--   0        0        0     8296 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/mesh_utils.py
+-rw-r--r--   0        0        0     1991 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/model.py
+-rw-r--r--   0        0        0    10952 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/parameters.py
+-rw-r--r--   0        0        0    19686 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/postprocessing.py
+-rw-r--r--   0        0        0    25882 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/resqpy_helpers.py
+-rw-r--r--   0        0        0    10027 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/simulator.py
+-rw-r--r--   0        0        0     4255 2024-04-09 10:10:23.314884 warmth-0.0.2/warmth/utils.py
+-rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 warmth-0.0.2/PKG-INFO
```

### Comparing `warmth-0.0.1/LICENSE.md` & `warmth-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `warmth-0.0.1/README.md` & `warmth-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `warmth-0.0.1/pyproject.toml` & `warmth-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "warmth"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Adam Cheng <52572642+adamchengtkc@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 xtgeo = "^3.4.0"
 numpy = "^1.26.0"
 pandas = "<2.0"
 scipy = "^1.11.3"
 progress = "^1.6"
 urllib3 = "^2.0.6"
 meshio = {extras = ["all"], version = "^5.3.4"}
 resqpy = "^4.12.1"
+pillow = "^10.3.0"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.25.2"
 notebook = "^7.0.4"
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 flake8 = "^6.1.0"
@@ -26,12 +27,13 @@
 sphinx-rtd-theme = "^1.3.0"
 sphinx-toolbox = "^3.5.0"
 myst-parser = "^2.0.0"
 matplotlib = "^3.8.0"
 ipywidgets = "^8.1.1"
 widgetsnbextension = "^4.0.9"
 nbsphinx = "^0.9.3"
+pytest-mpi = "^0.6"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `warmth-0.0.1/warmth/build.py` & `warmth-0.0.2/warmth/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -716,19 +716,18 @@
                         inputRef= np.append(inputRef,hor.horizon_index)
 
         
                     df = pd.DataFrame({'top': top, 'topage': topage, 'k_cond': k_cond,
                                                 'rhp': rhp, 'phi': phi, 'decay': decay, 'solidus': solidus, 'liquidus': liquidus,'strat':strat,'horizonIndex':inputRef})
                     df = df.sort_values(by=["topage"],ignore_index=True)
 
-    
+                    # print(df)
                     #df.reset_index(drop=True,inplace=True)
-                    df.at[2, 'top'] = np.nan
-            
-                    df.at[3, 'top'] = np.nan
+                    # df.at[2, 'top'] = np.nan            
+                    # df.at[3, 'top'] = np.nan
                     checker = self._check_nan_sed(df)
 
                     if checker is False:
                         self.nodes[index[0]][index[1]] = False
                     else:
                         df = self._fix_nan_sed(df)
                         n = single_node()
```

### Comparing `warmth-0.0.1/warmth/data/haq87.json` & `warmth-0.0.2/warmth/data/haq87.json`

 * *Files identical despite different names*

### Comparing `warmth-0.0.1/warmth/data.py` & `warmth-0.0.2/warmth/data.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.1/warmth/forward_modelling.py` & `warmth-0.0.2/warmth/forward_modelling.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,16 @@
                 if upper_idx.size == 0:
                     raise Exception
                 else:
                     upper_idx = upper_idx[-1][0]
 
                 lower_idx = np.argwhere(coord_new > key_depth)
                 if lower_idx.size == 0:
-                    raise Exception
+                    # raise Exception
+                    lower_idx = len(coord_new)-1
                 else:
                     lower_idx = lower_idx[0][0]
 
                 upper_diff = key_depth - coord_new[upper_idx]
                 lower_diff = coord_new[lower_idx] - key_depth
                 differences = np.array([upper_diff, lower_diff])
                 if np.any(differences < margin):
```

### Comparing `warmth-0.0.1/warmth/mesh_model.py` & `warmth-0.0.2/warmth/mesh_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import ufl
 from scipy.interpolate import LinearNDInterpolator
 from progress.bar import Bar
 from warmth.build import single_node, Builder
 from .parameters import Parameters
 from warmth.logging import logger
 from .mesh_utils import  top_crust,top_sed,thick_crust,  top_lith, top_asth, top_sed_id, bottom_sed_id,interpolateNode, interpolate_all_nodes
-from .resqpy_helpers import write_tetra_grid_with_properties, write_hexa_grid_with_properties,read_mesh_resqml_hexa
+from .resqpy_helpers import write_tetra_grid_with_properties, write_hexa_grid_with_timeseries, write_hexa_grid_with_properties,read_mesh_resqml_hexa
 def tic():
     #Homemade version of matlab tic and toc functions
     import time
     global startTime_for_tictoc
     startTime_for_tictoc = time.time()
 
 def toc(msg=""):
@@ -45,21 +45,26 @@
         self.mesh = None
 
         self.modelName = self._parameters.name
         self.Temp0 = 5
         self.TempBase = 1369
         self.verbose = True
         self.minimumCellThick = 0.05
+        self.averageLABdepth = 260000
         
         self.runSedimentsOnly = sedimentsOnly
-
-        self.numElemPerSediment = 4
-        self.numElemInCrust = 0 if self.runSedimentsOnly else 8    # split crust hexahedron into pieces
+        self.posarr = []
+        self.Tarr = []
+        self.time_indices = []
+
+        # 2 6 6 6
+        self.numElemPerSediment = 2
+        self.numElemInCrust = 0 if self.runSedimentsOnly else 4    # split crust hexahedron into pieces
         self.numElemInLith = 0 if self.runSedimentsOnly else 4  # split lith hexahedron into pieces
-        self.numElemInAsth = 0 if self.runSedimentsOnly else 2  # split asth hexahedron into pieces
+        self.numElemInAsth = 0 if self.runSedimentsOnly else 4  # split asth hexahedron into pieces
 
         self.num_nodes_x = self._builder.grid.num_nodes_x
         self.num_nodes_y = self._builder.grid.num_nodes_y
 
         nodes_padded = []
         self.padX = padding_num_nodes
         for j in range(-self.padX,self.num_nodes_y+self.padX):
@@ -134,15 +139,15 @@
             # discard aesth and lith (layer IDs -2, -3)
             #
             if (lid0>=-1) and (lid0<100):
                 tet_to_keep.append(t)
                 lid_to_keep.append(lid0)
                 cell_id_to_keep.append(self.node_index[i])
                 if abs(self.node_index[i].Y-minY)>1:
-                    print("unusual Y coordinate:", minY, self.node1D[self.node_index[i]].Y, i, self.node_index[i], self.node1D[self.node_index[i]])
+                    logger.warning( f"unusual Y coordinate:, {minY}, {self.node1D[self.node_index[i]].Y}, {i}, {self.node_index[i]}, {self.node1D[self.node_index[i]]}")
                 for ti in t:
                     p_to_keep.add(ti)
         poro0_per_cell = np.array( [ self.getSedimentPropForLayerID('phi', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ] )
         decay_per_cell = np.array( [ self.getSedimentPropForLayerID('decay', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
         density_per_cell = np.array( [ self.getSedimentPropForLayerID('solidus', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
         cond_per_cell = np.array( [ self.getSedimentPropForLayerID('k_cond', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
         rhp_per_cell = np.array( [ self.getSedimentPropForLayerID('rhp', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
@@ -162,107 +167,207 @@
         from os import path
         filename = path.join(out_path, self.modelName+'_'+str(self.tti)+'.epc')
         write_tetra_grid_with_properties(filename, np.array(points_cached), tet_renumbered, "tetramesh",
             np.array(T_per_vertex), np.array(age_per_vertex), poro0_per_cell, decay_per_cell, density_per_cell,
             cond_per_cell, rhp_per_cell, lid_per_cell)
         return filename
 
+    # def send_mpi_messages(self):
+    #     comm = MPI.COMM_WORLD
+    #     comm.send(mm2.mesh.topology.index_map(0).local_to_global(list(range(mm2.mesh.geometry.x.shape[0]))) , dest=0, tag=((comm.rank-1)*10)+21)
+    #     comm.send(mm2.mesh_reindex, dest=0, tag=((comm.rank-1)*10)+23)
+    #     comm.send(mm2.mesh_vertices_age, dest=0, tag=((comm.rank-1)*10)+25)
+    #     comm.send(self.posarr, dest=0, tag=( (comm.rank-1)*10)+20)
+    #     comm.send(self.Tarr, dest=0, tag=( (comm.rank-1)*10)+24)
+
+    def receive_mpi_messages(self):
+        comm = MPI.COMM_WORLD
+        import time
+        st = time.time()
+
+        self.sub_posarr_s = [self.posarr]
+        self.sub_Tarr_s = [self.Tarr]
+
+        self.index_map_s = [self.mesh.topology.index_map(0).local_to_global(list(range(self.mesh.geometry.x.shape[0])))]
+        self.mesh_reindex_s = [self.mesh_reindex]
+        self.mesh_vertices_age_s = [self.mesh_vertices_age]
+
+        for i in range(1,comm.size):
+            self.index_map_s.append(comm.recv(source=i, tag=((i-1)*10)+21))
+            self.mesh_reindex_s.append(comm.recv(source=i, tag=((i-1)*10)+23))
+            self.mesh_vertices_age_s.append(comm.recv(source=i, tag=((i-1)*10)+25))
+            self.sub_posarr_s.append(comm.recv(source=i, tag=((i-1)*10)+20))
+            self.sub_Tarr_s.append(comm.recv(source=i, tag=((i-1)*10)+24))
+
+        nv = np.amax(np.array( [np.amax(index_map) for index_map in self.index_map_s ] )) + 1   # no. vertices/nodes
+        mri = np.arange( nv, dtype=np.int32)
+
+        self.x_original_order = [ (np.ones( [nv,3], dtype= np.float32) * -1) for _ in range(len(self.posarr)) ]
+        self.T_per_vertex = [ (np.ones( nv, dtype= np.float32) * -1) for _ in range(len(self.Tarr)) ]
+        self.age_per_vertex = np.ones( nv, dtype= np.int32) * -1
+
+        for k in range(len(self.mesh_reindex_s)):
+            for ind,val in enumerate(self.mesh_reindex_s[k]):
+                for i in range(len(self.posarr)):
+                    self.x_original_order[i][val,:] = self.sub_posarr_s[k][i][ind,:] 
+                    self.T_per_vertex[i][val] = self.sub_Tarr_s[k][i][ind]
+                self.age_per_vertex[val] = self.mesh_vertices_age_s[k][ind]
+
+        delta = time.time() - st
+        logger.debug( f"receive_mpi_messages delta: {delta}")
+
+    def get_node_pos_and_temp(self, tti=-1):
+        #
+        # This function can only be called after all MPI compute processes have finished and receive_mpi_messages has been called.
+        #
+        start_time = self.time_indices[0]
+        end_time = self.time_indices[-1]
+        ind = start_time - ( tti if (tti>=0) else end_time)
+        if (ind >= len(self.x_original_order)):
+            return None,None
+        if (ind < 0):
+            return None,None
+        return self.x_original_order[ind], self.T_per_vertex[ind]
 
-    def write_hexa_mesh_resqml( self, out_path):
+    def write_hexa_mesh_resqml( self, out_path, tti):
         """Prepares arrays and calls the RESQML output helper function for hexa meshes:  the lith and aesth are removed, and the remaining
            vertices and cells are renumbered;  the sediment properties are prepared for output.
 
            out_path: string: path to write the resqml model to (.epc and .h5 files)
 
            returns the filename (of the .epc file) that was written 
         """            
-        x_original_order = self.mesh.geometry.x[:].copy()
-        reverse_reindex_order = np.arange( self.mesh_vertices.shape[0] )
-        for ind,val in enumerate(self.mesh_reindex):
-            x_original_order[val,:] = self.mesh.geometry.x[ind,:]
-            reverse_reindex_order[val] = ind
+        comm = MPI.COMM_WORLD
+        nv = np.amax(np.array([np.amax(index_map) for index_map in self.index_map_s])) +1  # no. vertices/nodes
         hexaHedra, hex_data_layerID, hex_data_nodeID = self.buildHexahedra(keep_padding=False)
 
         hexa_to_keep = []
         p_to_keep = set()
         lid_to_keep = []
         cond_per_cell = []
         cell_id_to_keep = []
+        x_original_order, T_per_vertex = self.get_node_pos_and_temp(tti)
         for i,h in enumerate(hexaHedra):
             lid0 = hex_data_layerID[i]
             # 
             # discard aesth and lith (layer IDs -2, -3)
             #
             if (lid0>=-1) and (lid0<100):
                 hexa_to_keep.append(h)
                 lid_to_keep.append(lid0)
                 # cell_id_to_keep.append(self.node_index[i])
                 cell_id_to_keep.append(hex_data_nodeID[i])
                 minY = np.amin(np.array ( [x_original_order[hi,1] for hi in h] ))
                 if abs( self.node1D[hex_data_nodeID[i]].Y - minY)>1:
-                    print("weird Y:", minY, self.node1D[hex_data_nodeID[i]].Y, abs( self.node1D[hex_data_nodeID[i]].Y - minY), i, hex_data_nodeID[i])
+                    logger.warning( f"weird Y:  {minY}, {self.node1D[hex_data_nodeID[i]].Y}, {abs( self.node1D[hex_data_nodeID[i]].Y - minY)}, {i}, {hex_data_nodeID[i]}" )
                     breakpoint()
-                # if (minY>40000):
-                #     pp = self.getSedimentPropForLayerID('phi', lid0, hex_data_nodeID[i])
-                #     if (pp<0.7) and lid0>=0:
-                #         print("weird phi: ", pp, minY, self.node1D[hex_data_nodeID[i]].Y, abs( self.node1D[hex_data_nodeID[i]].Y - minY), i, hex_data_nodeID[i])
-                #         breakpoint()
-                k_cond_mean = []
                 for hi in h:
                     p_to_keep.add(hi)
-                    k_cond_mean.append(self.thermalCond.x.array[hi])
-                cond_per_cell.append( np.mean(np.array(k_cond_mean)))
+                    # k_cond_mean.append(self.thermalCond.x.array[hi])   # the actual, Sekiguchi-derived conductivitues
+                # cond_per_cell.append( np.mean(np.array(k_cond_mean)))
 
         poro0_per_cell = np.array( [ self.getSedimentPropForLayerID('phi', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ] )
         decay_per_cell = np.array( [ self.getSedimentPropForLayerID('decay', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
         density_per_cell = np.array( [ self.getSedimentPropForLayerID('solidus', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
         cond_per_cell = np.array( [ self.getSedimentPropForLayerID('k_cond', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
         rhp_per_cell = np.array( [ self.getSedimentPropForLayerID('rhp', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
         lid_per_cell = np.array(lid_to_keep)
 
         points_cached = []
-        point_original_to_cached = np.ones(self.mesh.geometry.x.shape[0], dtype = np.int32)  * (-1)
-        for i in range(self.mesh.geometry.x.shape[0]):
+        point_original_to_cached = np.ones(nv, dtype = np.int32)  * (-1)
+        for i in range(nv):
             if (i in p_to_keep):
                 point_original_to_cached[i] = len(points_cached)
                 points_cached.append(x_original_order[i,:])
         hexa_renumbered = [ [point_original_to_cached[i] for i in hexa] for hexa in hexa_to_keep ]
         
-        for i,h in enumerate(hexa_renumbered):
-            minY = np.amin(np.array ( [np.array(points_cached)[hi,1] for hi in h] ))
-            poro0 = poro0_per_cell[i]
-            lid0  = lid_to_keep[i]
-            # if (minY>40000) and poro0 < 0.8 and lid0>=0:
-            #     print("problem A", minY, poro0, i, h)
-            #     breakpoint()
-            # if (minY<40000) and poro0 > 0.8:
-            #     print("problem B", minY, poro0, i, h)
-            #     breakpoint()
-
+        # for i,h in enumerate(hexa_renumbered):
+        #     minY = np.amin(np.array ( [np.array(points_cached)[hi][1] for hi in h] ))
+        #     poro0 = poro0_per_cell[i]
+        #     lid0  = lid_to_keep[i]
 
-        T_per_vertex = [ self.uh.x.array[reverse_reindex_order[i]] for i in range(self.mesh.geometry.x.shape[0]) if i in p_to_keep  ]
-        age_per_vertex = [ self.mesh_vertices_age[reverse_reindex_order[i]] for i in range(self.mesh.geometry.x.shape[0]) if i in p_to_keep  ]
+        T_per_vertex_keep = [ T_per_vertex[i] for i in range(nv) if i in p_to_keep ]
+        age_per_vertex_keep = [ self.age_per_vertex[i] for i in range(nv) if i in p_to_keep ]
 
         from os import path
-        filename_hex = path.join(out_path, self.modelName+'_hexa_'+str(self.tti)+'.epc')
+        filename_hex = path.join(out_path, self.modelName+'_hexa_'+str(tti)+'.epc')
         write_hexa_grid_with_properties(filename_hex, np.array(points_cached), hexa_renumbered, "hexamesh",
-            np.array(T_per_vertex), np.array(age_per_vertex), poro0_per_cell, decay_per_cell, density_per_cell,
+            np.array(T_per_vertex_keep), np.array(age_per_vertex_keep), poro0_per_cell, decay_per_cell, density_per_cell,
             cond_per_cell, rhp_per_cell, lid_per_cell)
         return filename_hex
 
+
+    def write_hexa_mesh_timeseries( self, out_path):
+        """Prepares arrays and calls the RESQML output helper function for hexa meshes:  the lith and aesth are removed, and the remaining
+           vertices and cells are renumbered;  the sediment properties are prepared for output.
+
+           out_path: string: path to write the resqml model to (.epc and .h5 files)
+
+           returns the filename (of the .epc file) that was written 
+        """            
+        hexaHedra, hex_data_layerID, hex_data_nodeID = self.buildHexahedra(keep_padding=False)
+
+        hexa_to_keep = []
+        p_to_keep = set()
+        lid_to_keep = []
+        cond_per_cell = []
+        cell_id_to_keep = []
+        for i,h in enumerate(hexaHedra):
+            lid0 = hex_data_layerID[i]
+            # 
+            # discard aesth and lith (layer IDs -2, -3)
+            #
+            if (lid0>=-1) and (lid0<100):
+                hexa_to_keep.append(h)
+                lid_to_keep.append(lid0)
+                cell_id_to_keep.append(hex_data_nodeID[i])
+                # k_cond_mean = []
+                for hi in h:
+                    p_to_keep.add(hi)
+                #     k_cond_mean.append(self.thermalCond.x.array[hi])
+                # cond_per_cell.append( np.mean(np.array(k_cond_mean)))
+
+        # poro0_per_cell = np.array( [ self.getSedimentPropForLayerID('phi', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ] )
+        # decay_per_cell = np.array( [ self.getSedimentPropForLayerID('decay', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
+        # density_per_cell = np.array( [ self.getSedimentPropForLayerID('solidus', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
+        # cond_per_cell = np.array( [ self.getSedimentPropForLayerID('k_cond', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
+        # rhp_per_cell = np.array( [ self.getSedimentPropForLayerID('rhp', lid,cid) for lid,cid in zip(lid_to_keep,cell_id_to_keep) ])
+        # lid_per_cell = np.array(lid_to_keep)
+
+        points_cached_series = []
+        Temp_per_vertex_series = []
+
+        for tti in self.time_indices:
+            x_original_order, T_per_vertex = self.get_node_pos_and_temp(tti)
+            T_per_vertex_filt = [ T_per_vertex[i] for i in range(x_original_order.shape[0]) if i in p_to_keep  ]
+            Temp_per_vertex_series.append(np.array(T_per_vertex_filt))
+            points_cached = []
+            point_original_to_cached = np.ones(x_original_order.shape[0], dtype = np.int32)  * (-1)
+            for i in range(x_original_order.shape[0]):
+                if (i in p_to_keep):
+                    point_original_to_cached[i] = len(points_cached)
+                    points_cached.append(x_original_order[i,:])
+            points_cached_series.append(np.array(points_cached))
+        hexa_renumbered = [ [point_original_to_cached[i] for i in hexa] for hexa in hexa_to_keep ]
+
+        from os import path
+        filename_hex = path.join(out_path, self.modelName+'_hexa_ts_'+str(self.tti)+'.epc')
+        write_hexa_grid_with_timeseries(filename_hex, points_cached_series, hexa_renumbered, "hexamesh",
+            Temp_per_vertex_series )
+        return filename_hex
+
     def heatflow_at_crust_sed_boundary(self):
         hf_array = np.zeros([self.num_nodes_x-2*self.padX, self.num_nodes_y-2*self.padX])
         for hy in range(self.padX, self.num_nodes_y-self.padX):
             for hx in range(self.padX, self.num_nodes_x-self.padX):
                 v_per_n = int(self.mesh_vertices.shape[0]/(self.num_nodes_y*self.num_nodes_x))
                 ind_base_of_sed = v_per_n - self.numElemInAsth - self.numElemInLith - self.numElemInCrust -1
                 # first_ind_in_crust = v_per_n - self.numElemInAsth - self.numElemInLith - self.numElemInCrust
 
                 node_ind = hy*self.num_nodes_x + hx
-                # nn = model.builder.nodes[hy][hx]
                 nn = self.node1D[node_ind]
                 temp_3d_ind = np.array([ np.where([self.mesh_reindex==i])[1][0] for i in range(node_ind*v_per_n+ind_base_of_sed, node_ind*v_per_n+ind_base_of_sed+2 ) ] )
                 dd = self.mesh.geometry.x[temp_3d_ind,2]
                 tt = self.u_n.x.array[temp_3d_ind]
                 hf = nn.kCrust*(tt[1]-tt[0])/(dd[1]-dd[0])
 
                 hx_unpad = hx - self.padX            
@@ -307,25 +412,16 @@
 
     #
     def getSedimentPropForLayerID(self, property, layer_id:int, node_index:int) ->float:
         """
         """           
         assert property in ['k_cond', 'rhp', 'phi', 'decay', 'solidus', 'liquidus'], "Unknown property " + property
         if (layer_id>=0) and (layer_id<self.numberOfSediments):
-            # node_index = ind2 // (self.numberOfSediments+6)  # +6 because crust, lith, aest are each cut into two
             node = self.node1D[node_index]
             prop = node.sediments[property][layer_id]
-            # if (property=='phi') and phi>0.7 and node.Y<40000:
-            #     print("phi", property, phi, node_index, node)
-            #     breakpoint()
-            # if (property=='phi') and phi<0.7 and node.Y>40000:
-            #     print("phi", property, phi, node_index, node)
-            #     breakpoint()
-            # phi = self.globalSediments[property][layer_id]
-            # assert abs(phi-phi0)<1e-6
             return prop
         if (layer_id<=-1) and (layer_id>=-3):
             lid = -layer_id -1
             node = self.node1D[node_index]
             if (property=='k_cond'):
                 return [node.kCrust, node.kLith, node.kAsth][lid]
             if (property=='rhp'):
@@ -340,19 +436,19 @@
                 return [node.crustliquid,node.lithliquid,node.asthliquid][lid]   # liquid density for crust, lith, aest
         return np.nan
 
     def porosity0ForLayerID(self, layer_id:int, node_index:int)->Tuple[float, float]:
         """Porosity (at surface) conductivity value for the given layer index
         """           
         if (layer_id==-1):
-            return 0.0,0.0 # porosity (at surface) of crust
+            return 0.0,1e8 # porosity (at surface) of crust
         if (layer_id==-2):
-            return 0.0,0.0 # porosity (at surface) of lith
+            return 0.0,1e8 # porosity (at surface) of lith
         if (layer_id==-3):
-            return 0.0,0.0  # porosity (at surface) of aesth
+            return 0.0,1e8  # porosity (at surface) of aesth
         if (layer_id>=0) and (layer_id<self.numberOfSediments):
             # assert (node_index < len(self.node1D)) and node_index > 0
             node = self.node1D[node_index]
             phi = node.sediments.phi[layer_id]
             decay = node.sediments.decay[layer_id]
             return phi, decay
         return 0.0, 0.0
@@ -400,115 +496,157 @@
             node = self.node1D[node_index]
             kc = node.sediments.rhp[ss]
             return kc
         else:
             return 0
 
 
-    def buildVertices(self, time_index=0, useFakeEncodedZ=False):
+    def buildVertices(self, time_index=0, optimized=False):
         """Determine vertex positions, node-by-node.
            For every node, the same number of vertices is added (one per sediment, one per crust, lith, asth, and one at the bottom)
            Degenerate vertices (e.g. at nodes where sediment is yet to be deposited or has been eroded) are avoided by a small shift, kept in self.sed_diff_z
-           
-           When the option useFakeEncodedZ is set, the z-values are repurposed to encode the index of the vertex in the original, deterministic indexing.
-           This is necessary because dolfinx will re-index the vertices upon mesh generation. 
         """           
         tti = time_index
         self.tti = time_index
+        import time
+
+        compare = False
+        if (optimized) and hasattr(self, 'mesh_vertices'):            
+            compare = True
+            xxT = self.top_sed_at_nodes[:,tti]
+            bc = self.base_crust_at_nodes[:,tti]
+            bl = self.base_lith_at_nodes[:,tti]
+            ba = bl.copy()+130000
+            aa = np.array([self.top_sed_at_nodes[:,tti]])
 
-        self.mesh_vertices_0 = []
-        self.sed_diff_z = []
-        self.mesh_vertices_age_unsorted = []
-        if not self.runSedimentsOnly:
-            mean_top_of_lith = np.mean( np.array( [ self.getTopOfLithAtNode(tti, node) for node in self.node1D ] ) )
-            mean_top_of_asth = np.mean( np.array( [ self.getTopOfAsthAtNode(tti, node) for node in self.node1D ] ) )
-            logger.info(f'Time {tti}: mean top of lith: {mean_top_of_lith:.1f}; of asth: {mean_top_of_asth:.1f} ')
-
-        for node in self.node1D:
-            top_of_sediments = top_sed(node, tti)
-            self.mesh_vertices_0.append( [ node.X, node.Y, top_of_sediments - 0.0*(self.numberOfSedimentCells+1) ] )
-            self.sed_diff_z.append(-self.minimumCellThick*(self.numberOfSedimentCells+1))
-            self.mesh_vertices_age_unsorted.append(node.sediments.topage[0])  # append top age of top sediment
             for ss in range(self.numberOfSediments):
                 for j in range(self.numElemPerSediment):
-                    base_of_prev_sediments = bottom_sed_id(node, ss-1, tti) if (ss>0) else top_of_sediments
-                    base_of_current_sediments = bottom_sed_id(node, ss, tti)
+                    base_of_prev_sediments = self.bottom_sed_id_at_nodes[ss-1][:,tti] if (ss>0) else (self.bottom_sed_id_at_nodes[ss][:,tti]*0)
+                    base_of_current_sediments = self.bottom_sed_id_at_nodes[ss][:,tti]
                     base_of_current_sediments = base_of_prev_sediments + (base_of_current_sediments-base_of_prev_sediments)* (j+1) / self.numElemPerSediment
                     if self.runSedimentsOnly:
                         zpos = base_of_current_sediments
+                        aa = np.concatenate([aa,np.array([zpos])])
                     else:
-                        zpos = top_of_sediments + base_of_current_sediments
-                    vert = np.array([ node.X, node.Y, zpos ])
-                    self.mesh_vertices_0.append( vert )
-                    self.sed_diff_z.append(-self.minimumCellThick*(self.numberOfSedimentCells - (ss*self.numElemPerSediment+j) ))
-                    age_of_previous = node.sediments.baseage[ss-1] if (ss>0) else 0.0
-                    self.mesh_vertices_age_unsorted.append( age_of_previous + ((j+1) / self.numElemPerSediment) * (node.sediments.baseage[ss]-age_of_previous) )  # append interpolatedbase age of current sediment
-
-            if not self.runSedimentsOnly:
-                base_of_last_sediments = bottom_sed_id(node, self.numberOfSediments-1, tti) if (self.numberOfSediments>0) else top_of_sediments
-                base_crust = mean_top_of_lith
-                for i in range(1,self.numElemInCrust+1):
-                    self.mesh_vertices_0.append( [ node.X, node.Y, base_of_last_sediments+ (base_crust-base_of_last_sediments)*(i/self.numElemInCrust) ] )
-                    self.sed_diff_z.append(0.0)
-                    self.mesh_vertices_age_unsorted.append(1000)
-
-                base_lith = mean_top_of_asth
-                for i in range(1,self.numElemInLith+1):
-                    self.mesh_vertices_0.append( [ node.X, node.Y, base_crust+ (base_lith-base_crust)*(i/self.numElemInLith) ] )
-                    self.sed_diff_z.append(0.0)
-                    self.mesh_vertices_age_unsorted.append(1000)
-
-                base_aest = base_lith+130000 # 260000
-                for i in range(1,self.numElemInAsth+1):
-                    self.mesh_vertices_0.append( [ node.X, node.Y, base_lith+(base_aest-base_lith)*(i/self.numElemInAsth) ] )
-                    self.sed_diff_z.append(0.0)
-                    self.mesh_vertices_age_unsorted.append(1000)
-
-        assert len(self.mesh_vertices_0) % self.num_nodes ==0
-        self.mesh_vertices_0 = np.array(self.mesh_vertices_0)
-        self.sed_diff_z = np.array(self.sed_diff_z)
-        self.mesh_vertices = self.mesh_vertices_0.copy()
+                        zpos = xxT + base_of_current_sediments
+                        aa = np.concatenate([aa,np.array([zpos])])
+
+            base_of_last_sediments = (xxT+self.bottom_sed_id_at_nodes[-1][:,tti]) if (len(self.bottom_sed_id_at_nodes)>0) else xxT
+
+            for i in range(1,self.numElemInCrust+1):
+                zp = base_of_last_sediments+ (bc-base_of_last_sediments)*(i/self.numElemInCrust) 
+                aa = np.concatenate([aa,np.array([zp])])
+
+            for i in range(1,self.numElemInLith+1):
+                zp = bc+ (bl-bc)*(i/self.numElemInLith) 
+                aa = np.concatenate([aa,np.array([zp])])
+            for i in range(1,self.numElemInAsth+1):
+                zp = bl+ (ba-bl)*(i/self.numElemInLith) 
+                aa = np.concatenate([aa,np.array([zp])])
+
+            new_z_pos_0 = np.transpose(aa).flatten()
+            mm0 = self.mesh_vertices.copy()
+            mm0[:,2] = new_z_pos_0
+            self.mesh_vertices_0 = mm0
+        else:
+            self.mesh_vertices_0 = []
+            self.sed_diff_z = []
+            self.mesh_vertices_age_unsorted = []
+
+            for ind,node in enumerate(self.node1D):
+                top_of_sediments = top_sed(node, tti)
+                self.mesh_vertices_0.append( [ node.X, node.Y, top_of_sediments - 0.0*(self.numberOfSedimentCells+1) ] )
+                self.sed_diff_z.append(-self.minimumCellThick*(self.numberOfSedimentCells+1))
+                self.mesh_vertices_age_unsorted.append(node.sediments.topage[0])  # append top age of top sediment
+                if (ind==0):
+                    st = time.time()
+                for ss in range(self.numberOfSediments):
+                    for j in range(self.numElemPerSediment):
+                        base_of_prev_sediments = bottom_sed_id(node, ss-1, tti) if (ss>0) else top_of_sediments
+                        base_of_current_sediments = bottom_sed_id(node, ss, tti)
+                        base_of_current_sediments = base_of_prev_sediments + (base_of_current_sediments-base_of_prev_sediments)* (j+1) / self.numElemPerSediment
+                        if self.runSedimentsOnly:
+                            zpos = base_of_current_sediments
+                        else:
+                            zpos = top_of_sediments + base_of_current_sediments
+                        vert = np.array([ node.X, node.Y, zpos ])
+                        self.mesh_vertices_0.append( vert )
+                        self.sed_diff_z.append(-self.minimumCellThick*(self.numberOfSedimentCells - (ss*self.numElemPerSediment+j) ))
+                        age_of_previous = node.sediments.baseage[ss-1] if (ss>0) else 0.0
+                        self.mesh_vertices_age_unsorted.append( age_of_previous + ((j+1) / self.numElemPerSediment) * (node.sediments.baseage[ss]-age_of_previous) )  # append interpolatedbase age of current sediment
+                if (ind==0):
+                    delta = time.time() - st
+                    logger.debug(f"delta 2: {delta}")
+                    st = time.time()
+                if not self.runSedimentsOnly:
+                    base_of_last_sediments = bottom_sed_id(node, self.numberOfSediments-1, tti) if (self.numberOfSediments>0) else top_of_sediments
+                    base_crust = node.subsidence[tti] + node.sed_thickness_ls[tti] + node.crust_ls[tti]
+
+                    for i in range(1,self.numElemInCrust+1):
+                        self.mesh_vertices_0.append( [ node.X, node.Y, base_of_last_sediments+ (base_crust-base_of_last_sediments)*(i/self.numElemInCrust) ] )
+                        self.sed_diff_z.append(0.0)
+                        self.mesh_vertices_age_unsorted.append(1000)
+
+                    base_lith = node.crust_ls[tti]+node.lith_ls[tti]+node.subsidence[tti]+node.sed_thickness_ls[tti]
+                    for i in range(1,self.numElemInLith+1):
+                        self.mesh_vertices_0.append( [ node.X, node.Y, base_crust+ (base_lith-base_crust)*(i/self.numElemInLith) ] )
+                        self.sed_diff_z.append(0.0)
+                        self.mesh_vertices_age_unsorted.append(1000)
+
+                    base_aest = base_lith+130000
+                    for i in range(1,self.numElemInAsth+1):
+                        self.mesh_vertices_0.append( [ node.X, node.Y, base_lith+(base_aest-base_lith)*(i/self.numElemInAsth) ] )
+                        self.sed_diff_z.append(0.0)
+                        self.mesh_vertices_age_unsorted.append(1000)
+                if (ind==0):
+                    delta = time.time() - st
+                    logger.debug(f"delta 3: {delta}")
+
+            assert len(self.mesh_vertices_0) % self.num_nodes ==0
+            self.mesh_vertices_0 = np.array(self.mesh_vertices_0)
+            self.sed_diff_z = np.array(self.sed_diff_z)
+            self.mesh_vertices = self.mesh_vertices_0.copy()
         self.mesh_vertices[:,2] = self.mesh_vertices_0[:,2] + self.sed_diff_z
-        if (useFakeEncodedZ):
-            self.mesh_vertices[:,2] = np.ceil(self.mesh_vertices[:,2])*1000 + np.array(list(range(self.mesh_vertices.shape[0])))*0.01
-            # zz = self.mesh_vertices[:,2].copy()
-            # zz2=np.mod(zz,1000)
-            # # mesh_reindex = (1e-4+zz2*10).astype(np.int32)
 
     def updateVertices(self):
         """Update the mesh vertex positions using the values in self.mesh_vertices, and using the known dolfinx-induded reindexing
         """        
         self.mesh.geometry.x[:] = self.mesh_vertices[self.mesh_reindex].copy()
         self.mesh_vertices_age = np.array(self.mesh_vertices_age_unsorted)[self.mesh_reindex].copy()
         self.mesh0_geometry_x = self.mesh.geometry.x.copy()      
         self.mesh_vertices[:,2] = self.mesh_vertices_0[:,2] - self.sed_diff_z
-        self.updateTopVertexMap()
+        
+        if hasattr(self, 'top_sed_at_nodes'):         
+            self.updateTopVertexMap()
         if self.runSedimentsOnly or (self.useBaseFlux): 
             self.updateBottomVertexMap()
         self.mesh_vertices[:,2] = self.mesh_vertices_0[:,2] + self.sed_diff_z
 
     def buildMesh(self,tti:int):
         """Construct a new mesh at the given time index tti, and determine the vertex re-indexing induced by dolfinx
         """        
         self.tti = tti
-        self.buildVertices(time_index=tti, useFakeEncodedZ=True)
+        self.buildVertices(time_index=tti)
         logger.info("Built vertices")
         self.constructMesh()
         logger.info("Built mesh")
         self.updateMesh(tti)
         logger.info("Updated vertices")
      
 
-    def updateMesh(self,tti:int):
+    def updateMesh(self,tti:int, optimized=False):
         """Construct the mesh positions at the given time index tti, and update the existing mesh with the new values
         """   
+        import time
         assert self.mesh is not None
-        self.tti = tti
-        self.buildVertices(time_index=tti, useFakeEncodedZ=False)
+        self.tti = tti        
+        self.buildVertices(time_index=tti, optimized=optimized)
         self.updateVertices()        
+        self.posarr.append(self.mesh.geometry.x.copy())
+        self.time_indices.append(self.tti)
 
     def buildHexahedra(self, keep_padding=True):
         xpnum = self.num_nodes_x
         ypnum = self.num_nodes_y
         # xpnum = self.num_nodes_x - 2* self.padX
         # ypnum = self.num_nodes_y - 2* self.padX
 
@@ -558,14 +696,16 @@
 
            The meshio library is used to write the mesh to file, from which dolfinx reads it.
         """   
         self.thermalCond = None
         v_per_n = int(len(self.mesh_vertices) / self.num_nodes)
         hexaHedra, hex_data_layerID, hex_data_nodeID = self.buildHexahedra()
 
+        comm = MPI.COMM_WORLD
+
 
         # https://www.baumanneduard.ch/Splitting%20a%20cube%20in%20tetrahedras2.htm
         tetsplit1 = [ [1,2,4,8], [1,2,5,8], [4,8,2,3], [2,3,7,8], [2,5,6,8], [2,6,7,8] ]
         tetsplit0 = [ [ p-1 for p in v ] for v in tetsplit1 ]
         lid_per_node = [100]
         for i in range(self.numberOfSedimentCells):
             lid_per_node.append(i)
@@ -581,128 +721,123 @@
         cells = []
         cell_data_layerID = []
         node_index = []
         c_count = 0
         for h,lid,nid in zip(hexaHedra, hex_data_layerID, hex_data_nodeID):
             for t in tetsplit0:
                 candidate_tet_ind = [ h[k] for k in t ]
-                # candidate_tet_pos = np.array(self.mesh_vertices[candidate_tet_ind,:] )
                 cells.append(candidate_tet_ind)
                 cell_data_layerID.append(lid)
                 node_index.append(nid)
             c_count = c_count + 1
 
         points = self.mesh_vertices.copy()
 
         mesh = meshio.Mesh(
             points,
             [ ("tetra", cells ) ],
             # Only one cell-spefific data array can be recovered by dolfinx (using read_meshtags), so we can write only one!
             cell_data={"layer": [ (np.array(cell_data_layerID, dtype=np.float64)+3)*1e7 + np.array(node_index, dtype=np.float64) ] },
         )
         
-        p = self._parameters.output_path/ 'mesh'
-        p.mkdir(parents=True, exist_ok=True)
-        fn = p/(self.modelName+"_mesh.xdmf")
- 
-        mesh.write( fn )
-        logger.info(f"saved mesh to {fn}")             
+        def mpi_print(s):
+            logger.info(f"Rank {comm.rank}: {s}")
+
+        fn = self.modelName+"_mesh.xdmf"
+        if comm.rank==0:
+            mesh.write( fn )
+            logger.info(f"saved mesh to {fn}")             
+        comm.Barrier()
         enc = dolfinx.io.XDMFFile.Encoding.HDF5
-        with dolfinx.io.XDMFFile(MPI.COMM_SELF, fn, "r", encoding=enc) as file:
-            self.mesh = file.read_mesh(name="Grid" )
-            aa=file.read_meshtags(self.mesh, name="Grid")
+        with dolfinx.io.XDMFFile(MPI.COMM_WORLD, fn, "r", encoding=enc) as file:   # MPI.COMM_SELF
+            self.mesh = file.read_mesh(name="Grid", ghost_mode=dolfinx.cpp.mesh.GhostMode.shared_facet)
+            aa = file.read_meshtags(self.mesh, name="Grid")
             self.cell_data_layerID = np.floor(aa.values.copy()*1e-7)-3
             self.node_index = np.mod(aa.values.copy(),1e7).astype(np.int32)
-        #
-        # obtain original vertex order as encoded in z-pos digits
+        self.mesh.topology.create_connectivity(3,0)  # create_connectivity_all()
+        mpi_print(f"Number of local cells: {self.mesh.topology.index_map(3).size_local}")
+        mpi_print(f"Number of global cells: {self.mesh.topology.index_map(3).size_global}")
+        mpi_print(f"Number of local vertices: {self.mesh.topology.index_map(0).size_local}")
+        mpi_print(f"Ghost cells (global numbering): {self.mesh.topology.index_map(3).ghosts}")
+        mpi_print(f"Ghost nodes (global numbering): {self.mesh.topology.index_map(0).ghosts}")
+
+        mpi_print(f"Dir local cells: {type(self.mesh.topology.index_map(3))} {dir(self.mesh.topology.index_map(3))}")
+        mpi_print(f"Dir local verts: {dir(self.mesh.topology.index_map(0))}")  # local_to_global ! ?
+        mpi_print(f"Type local verts: {type(self.mesh.topology.index_map(0))}")
 
-        zz  = self.mesh.geometry.x[:,2].copy()
-        zz2 = np.mod(zz,1000)
-        self.mesh_reindex = (1e-4+zz2*100).astype(np.int32)
+        # store original vertex order 
+        self.mesh_reindex = np.array(self.mesh.geometry.input_global_indices).astype(np.int32)
         self.mesh0_geometry_x = self.mesh.geometry.x.copy()
 
 
-
     def TemperatureGradient(self, x):
         self.averageLABdepth = np.mean(np.array([ top_asth(n, self.tti) for n in self.node1D]))
-        Zmin, Zmax = np.amin(x[2,:]), np.amax(x[2,:])
-        nz = (x[2,:] - Zmin) / (self.averageLABdepth - Zmin)
+
+        nz = (x[2,:] - self.Zmin) / (self.averageLABdepth - self.Zmin)
         nz[nz>1.0] = 1.0
         res = nz * (self.TempBase-self.Temp0) + self.Temp0
         for i in range(x.shape[1]):
             p = x[:,i]
             fkey = self.floatKey2D(p+[2e-2, 2e-2,0.0])
             dz = UniformNodeGridFixedSizeMeshModel.point_top_vertex_map.get(fkey, 1e10)
-            Zmin0 = dz if (dz<1e9) else np.amin(x[2,:])
+            Zmin0 = dz if (dz<1e9) else self.Zmin 
             nz0 = (p[2] - Zmin0) / (self.averageLABdepth - Zmin0)
             nz0 = min(nz0, 1.0)
             res[i] = nz0 * (self.TempBase-self.Temp0) + self.Temp0
-            if (p[2]>250000):
+            if (p[2] > self.averageLABdepth):
                 res[i] =  1330 + (p[2]-self.averageLABdepth)*0.0003  # 1369
-
-            # Zmax = np.amax(x[2,:])
-        # res[x[2,:]<self.Zmin] = self.Temp0 + (( x[2,:][x[2,:]<self.Zmin] - self.Zmin)/1000)*12
         return res
 
 
     def floatKey2D(self, xp):
         """Returns a tuple of integers from the input xy-point.  This is useful as a dict key for fast lookups. 
         """   
         return( int(xp[0]*10), int(xp[1]*10) )
 
 
-    def sedimentsConductivitySekiguchi(self): #mean_porosity, conductivity, temperature_C):
+    def sedimentsConductivitySekiguchi(self):
         """Scale surface conductivity of sediments to effective conductivity of sediments at depth. Scaler of 0.6 based on Allen & Allen p345. porosity dependent conductivity
         Args:
             mean_porosity (npt.NDArray[np.float64]): Mean porosity of sediments at depth
             conductivity (npt.NDArray[np.float64]): Conductivity of sediments at 20C
         Returns:
             npt.NDArray[np.float64]: Effective conductivity of sediments
         """
+        import time
         def boundary(x):
             return np.full(x.shape[1], True)
         entities = dolfinx.mesh.locate_entities(self.mesh, 3, boundary )
         tet = dolfinx.cpp.mesh.entities_to_geometry(self.mesh, 3, entities, False)
         self.layer_id_per_vertex = [ [] for _ in range(self.mesh.geometry.x.shape[0]) ]
-        ## TODO vectorize and use function from Forward model
-        for i,t in enumerate(tet):
-            lidval = int(self.layerIDsFcn.x.array[i])
-            if (lidval<0):
-                # only relevant for sediment
-                self.mean_porosity.x.array[i] = 0.0
-                continue
-            zpos = [ self.mesh.geometry.x[ti,2] for ti in t]
-            xpos = [ self.mesh.geometry.x[ti,0] for ti in t]
-            ypos = [ self.mesh.geometry.x[ti,1] for ti in t]
-            fkey = self.floatKey2D([xpos[0]+2e-2, ypos[0]+2e-2])
-            meshZmin = UniformNodeGridFixedSizeMeshModel.point_top_vertex_map.get(fkey, 1e10)
-            if (meshZmin < 1e9):
-                zpos = [ (zp-meshZmin) for zp in zpos ]
-            top_km = np.amin(zpos) / 1e3
-            bottom_km = np.amax(zpos) / 1e3
-            poro0 = self.porosity0.x.array[i]
-            decay = self.porosityDecay.x.array[i]
-            f1 = poro0 / (decay * (bottom_km-top_km))
-            f2 = np.exp(-1 * decay * top_km) - np.exp(-1 * decay * bottom_km)
-            mean_porosity = f1*f2
-            self.porosityAtDepth.x.array[i] = mean_porosity
-            
-            cond_local = self.kForLayerID(lidval, self.node_index[i])
-            temperature_C = np.mean(np.array([ self.uh.x.array[ti] for ti in t]))
+        ## 
 
-            temperature_K = 273.15 + temperature_C
-            conductivity_effective = 1.84 + 358 * ( (1.0227*cond_local)-1.882) * ((1/temperature_K)-0.00068)
-            conductivity_effective = conductivity_effective * (1.0-mean_porosity) # * np.sqrt(1-mean_porosity)
-
-            self.thermalCond.x.array[i] = conductivity_effective
-            self.mean_porosity.x.array[i] = mean_porosity
-            self.c_rho.x.array[i] = self._parameters.cp*((self.c_rho0.x.array[i]/self._parameters.cp) * (1-mean_porosity) + mean_porosity*self._parameters.rhowater)
-
-        # self.rhpFcn.x.array[:] = np.multiply( self.rhp0.x.array[:], (1.0-self.mean_porosity.x.array[:]) )
-        self.rhpFcn.x.array[:] = np.multiply( self.rhp0.x.array[:], 1.0 )
+        top_km = (np.min(self.mesh.geometry.x[tet,2], 1)-self.subsidence_at_nodes[:,self.tti]) * 1e-3
+        bottom_km = (np.max(self.mesh.geometry.x[tet,2], 1)-self.subsidence_at_nodes[:,self.tti]) * 1e-3
+        poro0 = self.porosity0.x.array[:]
+        decay = self.porosityDecay.x.array[:]
+        ii = np.where(top_km<0.0)
+
+        diff_z = np.amin(top_km)
+        top_km[top_km<0.0] = top_km[top_km<0.0]+0.0002-diff_z
+        bottom_km[bottom_km<0.0] = bottom_km[bottom_km<0.0]+0.0002-diff_z
+        f1 = np.divide( self.porosity0.x.array[:], np.multiply( self.porosityDecay.x.array[:], bottom_km-top_km ) )
+        f2 = np.exp(-1 * np.multiply(decay, top_km)) - np.exp(-1 * np.multiply(decay, bottom_km))
+        mean_porosity = np.multiply(f1,f2)
+
+        # temperature_C is the mean temperature in the cells
+        temperature_C = np.mean(self.uh.x.array[tet[:,:]],1)
+        temperature_K_inv = np.reciprocal(273.15 + temperature_C)
+        conductivity_effective = 1.84 + 358 * np.multiply( ( (1.0227*self.thermalCond0)-1.882) , ((temperature_K_inv)-0.00068) )
+        conductivity_effective = conductivity_effective * (1.0-mean_porosity) # * np.sqrt(1-mean_porosity)
+        self.thermalCond.x.array[self.layerIDsFcn.x.array[:]>=0] = conductivity_effective[self.layerIDsFcn.x.array[:]>=0]
+        self.mean_porosity.x.array[self.layerIDsFcn.x.array[:]>=0] = mean_porosity[self.layerIDsFcn.x.array[:]>=0]
+
+        newrho = self._parameters.cp * np.multiply( \
+            ((self.c_rho0.x.array[:]/self._parameters.cp)), (1-mean_porosity)) + mean_porosity*self._parameters.rhowater
+        self.c_rho.x.array[self.layerIDsFcn.x.array[:]>=0] = newrho[self.layerIDsFcn.x.array[:]>=0] 
 
     def getCellMidpoints(self):  
         def boundary(x):
             return np.full(x.shape[1], True)
         entities = dolfinx.mesh.locate_entities(self.mesh, 3, boundary )
         tet = dolfinx.cpp.mesh.entities_to_geometry(self.mesh, 3, entities, False)
         self.layer_id_per_vertex = [ [] for _ in range(self.mesh.geometry.x.shape[0]) ]
@@ -750,24 +885,24 @@
         midp = np.sum(p0,1)*0.25   # midpoints of tetrahedra
 
         ls = self.cell_data_layerID.copy()
         lid.x.array[:] = np.array(ls, dtype=PETSc.ScalarType).flatten()
 
         ks = [ self.kForLayerID(lid,self.node_index[i]) for i,lid in enumerate(ls)]
         thermalCond.x.array[:] = np.array(ks, dtype=PETSc.ScalarType).flatten()
+        self.thermalCond0 = np.array(ks, dtype=PETSc.ScalarType).flatten()
 
         rhps = [ self.rhpForLayerID(lid,self.node_index[i]) for i,lid in enumerate(ls)]
         rhp.x.array[:] = np.array(rhps, dtype=PETSc.ScalarType).flatten()
         self.rhp0.x.array[:] = np.array(rhps, dtype=PETSc.ScalarType).flatten()
 
         crs = [ self.cRhoForLayerID(lid,self.node_index[i]) for i,lid in enumerate(ls)]
         c_rho.x.array[:] = np.array(crs, dtype=PETSc.ScalarType).flatten()
         self.c_rho0.x.array[:] = np.array(crs, dtype=PETSc.ScalarType).flatten()
 
-        # self.node_index[i]
         poro = [ self.porosity0ForLayerID(lid, self.node_index[i])[0] for i,lid in enumerate(ls)]
         self.porosity0.x.array[:] = np.array(poro, dtype=PETSc.ScalarType).flatten()
         self.porosityAtDepth.x.array[:] = np.array(poro, dtype=PETSc.ScalarType).flatten()
 
         decay = [ self.porosity0ForLayerID(lid, self.node_index[i])[1] for i,lid in enumerate(ls)]
         self.porosityDecay.x.array[:] = np.array(decay, dtype=PETSc.ScalarType).flatten()
 
@@ -797,28 +932,25 @@
         self.updateTopVertexMap()
         if self.runSedimentsOnly:
             self.updateBottomVertexMap()
         return thermalCond, c_rho, lid, rhp
 
     def updateTopVertexMap(self):
         """ Updates the point_top_vertex_map, used for fast lookup of subsidence values.
-            (to be re-designed?)
         """ 
         UniformNodeGridFixedSizeMeshModel.point_top_vertex_map = {}
         v_per_n = int(len(self.mesh_vertices) / self.num_nodes)
-        if not self.runSedimentsOnly:
-            indices = np.where( np.mod(self.mesh_reindex,v_per_n)==0)[0]
-        else:
-            indices = range(self.mesh.geometry.x.shape[0])
-        for i in indices:
-            p = self.mesh.geometry.x[i,:]
-            fkey = self.floatKey2D(p+[2e-2, 2e-2,0.0])
-            dz = UniformNodeGridFixedSizeMeshModel.point_top_vertex_map.get(fkey, 1e10)
-            if p[2]<dz:
-                UniformNodeGridFixedSizeMeshModel.point_top_vertex_map[fkey] = p[2]
+        for i,n in enumerate(self.node1D):
+            aa = self.top_sed_at_nodes[i, self.tti] + (-self.minimumCellThick*(self.numberOfSedimentCells+1))
+            fkey = self.floatKey2D( np.array([n.X,n.Y,0.0]) + [2e-2, 2e-2,0.0])
+            UniformNodeGridFixedSizeMeshModel.point_top_vertex_map[fkey] = aa
+            fkey = self.floatKey2D( np.array([n.X,n.Y,0.0]) - [2e-2, 2e-2,0.0])
+            UniformNodeGridFixedSizeMeshModel.point_top_vertex_map[fkey] = aa
+            fkey = self.floatKey2D( np.array([n.X,n.Y,0.0]) + [0e-2, 0e-2,0.0])
+            UniformNodeGridFixedSizeMeshModel.point_top_vertex_map[fkey] = aa
 
     def updateBottomVertexMap(self):
         """ Updates the point_bottom_vertex_map, used for fast lookup of subsidence values.
             (to be re-designed?)
         """ 
         UniformNodeGridFixedSizeMeshModel.point_bottom_vertex_map = {}
         #v_per_n = int(len(self.mesh_vertices) / self.num_nodes)
@@ -829,39 +961,60 @@
             if p[2]>dz:
                 UniformNodeGridFixedSizeMeshModel.point_bottom_vertex_map[fkey] = p[2]
 
     def updateDirichletBaseTemperature(self):
         assert False, "to be re-implemented"
 
 
+    def updateDBC(self):
+        self.averageLABdepth = np.mean(np.array([ top_asth(n, self.tti) for n in self.node1D]))
+        logger.debug(f"self.averageLABdepth: {self.averageLABdepth}")
+        ii = np.where(self.mesh.geometry.x[:,2]>250000)
+        self.bc.value.x.array[ii] = 1330+(self.mesh.geometry.x[ii,2]-self.averageLABdepth)*0.0003
+
+
     def buildDirichletBC(self):
         """ Generate a dolfinx Dirichlet Boundary condition that applies at the top and bottom vertices.
             The values at the edges are those in function self.TemperatureStep
         """ 
-        # Dirichlet BC at top and bottom
-        self.Zmax = np.amax(self.mesh.geometry.x[:,2])
-        self.averageLABdepth = np.mean(np.array([ top_sed(n, self.tti) for n in self.node1D]))
+        import time
+        comm = MPI.COMM_WORLD          
+
+        st = time.time()
+        self.averageLABdepth = np.mean(np.array([ top_asth(n, self.tti) for n in self.node1D]))
+        self.Zmax = self.averageLABdepth + 130000
+        logger.debug(f"buildDirichletBC delta 1: {time.time()-st}")
+
         def boundary_D_top_bottom(x):
             subs0 = self.getSubsidenceAtMultiplePos(x[0,:], x[1,:])
-            xx = np.logical_or( np.abs(x[2]-subs0)<5, np.isclose(x[2], self.Zmax) )
+            xx = np.logical_or( np.abs(x[2]-subs0) < 0.9*self.minimumCellThick, np.abs(x[2]-self.Zmax)<10000 )
+            return xx
+        def boundary_D_bottom(x):
+            subs0 = self.getSubsidenceAtMultiplePos(x[0,:], x[1,:])
+            xx = np.logical_or( np.abs(x[2]-self.Zmax)<10000, np.abs(x[2]-self.Zmax)<10000 )
             return xx
         def boundary_D_top(x):
             subs0 = self.getSubsidenceAtMultiplePos(x[0,:], x[1,:])
-            # print("subs0", self.tti, subs0.shape, subs0[np.abs(subs0)>1].shape, subs0[np.abs(subs0)>1] )
-            #print("subs0", self.tti, subs0.shape, subs0[np.abs(subs0)>1].shape, subs0[np.abs(subs0)>1] )
-            xx = np.logical_or( np.abs(x[2]-subs0)<5, np.isclose(x[2], 1e6*self.Zmax) )            
+            xx = np.logical_or( np.abs(x[2]-subs0) < 0.9*self.minimumCellThick, np.isclose(x[2], 1e6*self.Zmax) )            
             return xx
             
         if (self.useBaseFlux):
+            st = time.time()
             dofs_D = dolfinx.fem.locate_dofs_geometrical(self.V, boundary_D_top)
-            print("dofs_D", self.tti, dofs_D.shape)
+            logger.debug(f"buildDirichletBC delta 2: {time.time()-st}")
         else:
+            st = time.time()
             dofs_D = dolfinx.fem.locate_dofs_geometrical(self.V, boundary_D_top_bottom)
+            # dofs_D2 = dolfinx.fem.locate_dofs_geometrical(self.V, boundary_D_bottom)
+            # dofs_D3 = dolfinx.fem.locate_dofs_geometrical(self.V, boundary_D_top)
+            logger.debug(f"buildDirichletBC delta 3: {time.time()-st}")
         u_bc = dolfinx.fem.Function(self.V)
+        st = time.time()
         u_bc.interpolate(self.TemperatureGradient)
+        logger.debug(f"buildDirichletBC delta 4: {time.time()-st}")
         bc = dolfinx.fem.dirichletbc(u_bc, dofs_D)
         return bc
 
 
     def resetMesh(self):
         self.mesh.geometry.x[:,2] = self.mesh0_geometry_x.copy()[:,2]
 
@@ -893,86 +1046,136 @@
             #
         """         
         xdmf = dolfinx.io.XDMFFile(MPI.COMM_WORLD, outfilename, "w")
         xdmf.write_mesh(self.mesh)
         xdmf.write_function(self.layerIDsFcn, tti)
         xdmf.write_function(self.u_n, tti)
 
-    def setupSolverAndSolve(self, n_steps:int=100, time_step:int=-1, skip_setup:bool = False, initial_state_model = None):
+    def setupSolver(self, initial_state_model = None):
+        comm = MPI.COMM_WORLD          
+        def mpi_print(s):
+            print(f"Rank {comm.rank}: {s}")
+
+        self.resetMesh()
+        self.Zmin = np.min(self.mesh_vertices, axis=0)[2]
+        self.Zmax = np.max(self.mesh_vertices, axis=0)[2]
+        # mpi_print(f"Number of local cells: {self.mesh.topology.index_map(3).size_local}")
+        # mpi_print(f"Number of global cells: {self.mesh.topology.index_map(3).size_global}")
+        # mpi_print(f"Number of local vertices: {self.mesh.topology.index_map(0).size_local}")
+
+        #
+        # define function space
+        self.FE = ufl.FiniteElement("CG", self.mesh.ufl_cell(), self.CGorder)
+        self.V = dolfinx.fem.FunctionSpace(self.mesh, self.FE)
+
+        # Define solution variable uh
+        self.uh = dolfinx.fem.Function(self.V)
+        self.uh.name = "uh"
+
+        # u_n: solution at previous time step
+        self.u_n = dolfinx.fem.Function(self.V)
+        self.u_n.name = "u_n"
+
+        import time
+
+        st = time.time()
+        nn = self.node1D[self.node_index[0]]
+        
+        self.subsidence_at_nodes = np.zeros([ len(self.cell_data_layerID), nn.subsidence.shape[0] ])
+        
+        for i in range(len(self.node1D)):
+            nn = self.node1D[i]
+            iix = np.where(self.node_index==i)
+            self.subsidence_at_nodes[iix,:] = nn.subsidence
+        logger.debug(f"setup delay 1.3: {time.time()-st}")
+
+        st = time.time()
+        top_of_sediments = self.subsidence_at_nodes
+        self.bottom_sed_id_at_nodes = [] 
+        self.top_sed_at_nodes = np.zeros([self.num_nodes, nn.subsidence.shape[0] ])
+        self.base_crust_at_nodes = np.zeros([self.num_nodes, nn.subsidence.shape[0] ])
+        self.base_lith_at_nodes = np.zeros([self.num_nodes, nn.subsidence.shape[0] ])
+        for k in range(0,self.numberOfSediments):
+            bottom_sed_id_at_nodes = np.zeros([self.num_nodes, nn.subsidence.shape[0] ])
+            for i in range(len(self.node1D)):
+                nn = self.node1D[i]
+                bottom_sed_id_at_nodes[i, :] = nn.sed[k,1,:]
+            self.bottom_sed_id_at_nodes.append(bottom_sed_id_at_nodes)
+        for i in range(len(self.node1D)):
+            nn = self.node1D[i]
+            self.top_sed_at_nodes[i,:] = nn.subsidence
+            self.base_crust_at_nodes[i,:] = nn.subsidence + nn.sed_thickness_ls + nn.crust_ls
+            self.base_lith_at_nodes[i,:]  = self.base_crust_at_nodes[i,:] + nn.lith_ls
+        logger.debug(f"setup delay 1.4: {time.time()-st}")
+
+        st = time.time()
+        self.thermalCond, self.c_rho, self.layerIDsFcn, self.rhpFcn = self.buildKappaAndLayerIDs()
+        assert not np.any(np.isnan(self.thermalCond.x.array))
+        logger.debug(f"setup delay 1: {time.time()-st}")
+
+        st = time.time()
+        # initialise both with initial condition: either a step function, or the solution from another Model instance
+        if (initial_state_model is None):
+            self.u_n.interpolate(self.TemperatureGradient)
+        else:
+            self.u_n.x.array[:] = initial_state_model.uh.x.array[:].copy()
+        self.uh.x.array[:] = self.u_n.x.array[:].copy()
+        logger.debug(f"setup delay 1.5: {time.time()-st}")
+
+    def setupSolverAndSolve(self, n_steps:int=100, time_step:int=-1, skip_setup:bool = False, initial_state_model = None, update_bc=False):
         """ Sets up the function spaces, output functions, input function (kappa values), boundary conditions, initial conditions.
             Sets up the heat equation in dolfinx, and solves the system in time for the given number of steps.
             
             Use skip_setup = True to continue a computation (e.g. after deforming the mesh), instead of starting one from scratch 
-        """     
-        if (not skip_setup):
-            self.resetMesh()
-            self.Zmin = np.min(self.mesh_vertices, axis=0)[2]
-            self.Zmax = np.max(self.mesh_vertices, axis=0)[2]
-        
-        # Time-dependent heat problem:
-        #   time-discretized variational form with backwards Euler,
-        #   see: https://fenicsproject.org/pub/tutorial/html/._ftut1006.html
+        """   
+        comm = MPI.COMM_WORLD          
+        def mpi_print(s):
+            logger.debug(f"Rank {comm.rank}: {s}")
     
         if (not skip_setup):
-            #
-            # define function space
-            self.FE = ufl.FiniteElement("CG", self.mesh.ufl_cell(), self.CGorder)
-            self.V = dolfinx.fem.FunctionSpace(self.mesh, self.FE)
-
-            # Define solution variable uh
-            self.uh = dolfinx.fem.Function(self.V)
-            self.uh.name = "uh"
-
-            # u_n: solution at previous time step
-            self.u_n = dolfinx.fem.Function(self.V)
-            self.u_n.name = "u_n"
-
-            # initialise both with initial condition: either a step function, or the solution from another Model instance
-            if (initial_state_model is None):
-                # self.u_n.interpolate(self.TemperatureStep)
-                self.u_n.interpolate(self.TemperatureGradient)
-                # self.u_n.interpolate(self.TemperatureFromNode)
-            else:
-                self.u_n.x.array[:] = initial_state_model.uh.x.array[:].copy()
-            self.uh.x.array[:] = self.u_n.x.array[:].copy()
+            self.setupSolver(initial_state_model)
 
+        if (not skip_setup) or update_bc:
+            self.bc = self.buildDirichletBC()
 
-        self.thermalCond, self.c_rho, self.layerIDsFcn, self.rhpFcn = self.buildKappaAndLayerIDs()
-        assert not np.any(np.isnan(self.thermalCond.x.array))
-        
+        import time
+        st = time.time()
         self.sedimentsConductivitySekiguchi()
-
-        self.bc = self.buildDirichletBC()
+        logger.debug(f"solve delay 2: {time.time()-st}")
 
         t=0
         dt = time_step if (time_step>0) else  3600*24*365 * 5000000
         num_steps = n_steps
 
         #
+        # Time-dependent heat problem:
+        #   time-discretized variational form with backwards Euler,
+        #   see: https://fenicsproject.org/pub/tutorial/html/._ftut1006.html
+        #
         #  solver setup, see:
         #  https://jorgensd.github.io/dolfinx-tutorial/chapter2/diffusion_code.html
         #
 
         u = ufl.TrialFunction(self.V)
         v = ufl.TestFunction(self.V)
 
         a = self.c_rho*u*v*ufl.dx + dt*ufl.dot(self.thermalCond*ufl.grad(u), ufl.grad(v)) * ufl.dx
         f = self.rhpFcn 
         logger.info(f"mean RHP {np.mean(self.rhpFcn.x.array[:])}")
 
-
         if ( self.useBaseFlux ):
-            # baseFlux = 0.03 if (self.tti>50) else 0.03 
             baseFlux = self.baseFluxMagnitude
             # define Neumann condition: constant flux at base
             # expression g defines values of Neumann BC (heat flux at base)
-            #x = ufl.SpatialCoordinate(self.mesh)
             domain_c = dolfinx.fem.Function(self.V)
             domain_c.x.array[ : ] = 0.0
             if (self.CGorder>1):
+                #
+                # NOTE: CGorder>1 is under development, not functional
+                #
                 def marker(x):
                     print(x.shape, x)
                     return x[2,:]>3990
                 facets = dolfinx.mesh.locate_entities_boundary(self.mesh, dim=(self.mesh.topology.dim - 2),
                                         marker=marker )
                 #print(type(facets), facets.shape)
                 dofs = dolfinx.fem.locate_dofs_topological(V=self.V, entity_dim=1, entities=facets)
@@ -997,38 +1200,38 @@
                 # domain_c.x.array[  np.logical_and( self.mesh.geometry.x[:,0] < xmin+1, self.mesh.geometry.x[:,1] > ymax-1) ] = 0
                 # domain_c.x.array[  np.logical_and( self.mesh.geometry.x[:,0] > xmax-1, self.mesh.geometry.x[:,1] < ymin+1) ] = 0
                 # domain_c.x.array[  np.logical_and( self.mesh.geometry.x[:,0] > xmax-1, self.mesh.geometry.x[:,1] > ymax-1) ] = 0
 
             domain_zero = dolfinx.fem.Function(self.V)
             toppos = self.getSubsidenceAtMultiplePos(self.mesh.geometry.x[:,0], self.mesh.geometry.x[:,1])
             domain_zero.x.array[  self.mesh.geometry.x[:,2] < toppos+0.01 ] = 1
-            print("Neumann conditions: ", self.tti, np.count_nonzero(domain_c.x.array), np.count_nonzero(domain_zero.x.array))
+            logger.debug(f"Neumann conditions: , {self.tti}, {np.count_nonzero(domain_c.x.array)}, {np.count_nonzero(domain_zero.x.array)}")
 
             g = (-1.0*baseFlux) * ufl.conditional( domain_c > 0, 1.0, 0.0 )
             L = (self.c_rho*self.u_n + dt*f)*v*ufl.dx - dt * g * v * ufl.ds    # last term reflects Neumann BC 
         else:
             L = (self.c_rho*self.u_n + dt*f)*v*ufl.dx   # no Neumann BC 
 
         bilinear_form = dolfinx.fem.form(a)
         linear_form = dolfinx.fem.form(L)
 
         A = dolfinx.fem.petsc.assemble_matrix(bilinear_form, bcs=[self.bc])
         A.assemble()
         b = dolfinx.fem.petsc.create_vector(linear_form)
 
-        from petsc4py import PETSc
+        comm = MPI.COMM_WORLD
         solver = PETSc.KSP().create(self.mesh.comm)
 
         solver.setOperators(A)
         solver.setType(PETSc.KSP.Type.PREONLY)
         solver.getPC().setType(PETSc.PC.Type.LU)
-        
+
+        import time
         for i in range(num_steps):
             t += dt
-
             # Update the right hand side reusing the initial vector
             with b.localForm() as loc_b:
                 loc_b.set(0)
             dolfinx.fem.petsc.assemble_vector(b, linear_form)
 
             # TODO: update Dirichlet BC at every time step:
             #       the temperature at the base of Asth is set such that it reaches Tm at the current depth of the LAB (using the slope adiab=0.0003)
@@ -1043,14 +1246,17 @@
             # Solve linear problem
             solver.solve(b, self.uh.vector)
             self.uh.x.scatter_forward()
 
             # Update solution at previous time step (u_n)
             # diffnorm = np.sum(np.abs(self.u_n.x.array - self.uh.x.array)) / self.u_n.x.array.shape[0]
             self.u_n.x.array[:] = self.uh.x.array
+            # comm.Barrier()
+        self.Tarr.append(self.uh.x.array[:].copy())
+        # print("latest Tarr", self.Tarr[-1], np.mean(self.Tarr[-1]))
 
 
 
 
     #
     # =====================================
     #     Helper functions, not used by the main workflow
@@ -1067,15 +1273,14 @@
         if (np.isnan(res)):
             manyres = np.array( [ interp([pos_x-epsilon, pos_y-epsilon])[0], \
                 interp([pos_x+epsilon, pos_y-epsilon])[0],\
                 interp([pos_x-epsilon, pos_y+epsilon])[0],\
                 interp([pos_x+epsilon, pos_y+epsilon])[0]])
             res = np.nanmean(manyres)
         if (np.isnan(res)):
-            # print(pos_x, pos_y, interp([pos_x, pos_y]), interp([0,0])[0] )
             logger.warning(f'NaN encounered in safeInterpolation pos_x {pos_x}:  pos_y: {pos_y};  {interp([pos_x, pos_y])} {interp([0,0])[0]} ')
         # assert not np.isnan(res), "interpolation is nan in safeInterpolation"
         return res
 
     def getThickOfCrustAtPos(self, tti, pos_x, pos_y):
         interp = self.getInterpolator(tti, "thick_crust")
         thick_crust_1 = self.safeInterpolation(interp, pos_x, pos_y)        
@@ -1307,112 +1512,109 @@
                 #points_cells.append(cell_candidates.links(i)[0])
                 for bb in cell_candidates.links(i):
                     val = self.uh.eval(point, [bb])
                     if (not np.isnan(val)):
                         break
                 res.append( val )
             else:
-                print("need to extrapolate cell for point", i, point)
+                logger.debug(f"need to extrapolate cell for point {i}, {point}")
                 if (point[2]>200000):
                     try:
                         points_cells.append(cell_candidates.links(i)[0])
                         points_on_proc.append(point)
                     except IndexError:
-                        print("IndexError", point, cell_candidates.links(i) )
+                        logger.warning(f"IndexError, {point}, {cell_candidates.links(i)}" )
                         breakpoint()
                         raise
                 else:
-                    print("PING V", point)
+                    logger.debug(f"PING V, {point}")
                     if len(cell_candidates.links(i))==0:
-                        print("PING V V", point)
+                        logger.debug(f"PING V V, {point}")
                         def boundary(x):
                             return np.full(x.shape[1], True)
                         #entities = dolfinx.mesh.locate_entities(self.mesh, 3, boundary )
                         breakpoint()
                     points_on_proc.append(point)
                     points_cells.append(cell_candidates.links(i)[0])
         res = np.array(res)
         aa = np.any(np.isnan(res))
         bb = np.any(np.isnan(self.uh.x.array))
         if aa or bb:
-            print(aa,bb)
+            logger.debug(f"aa {aa},  bb {bb}")
             breakpoint()
 
         if transpose:
             assert res.flatten().shape[0] == x.shape[1]
         else:
             assert res.flatten().shape[0] == x.shape[0]
         return res.flatten()
 
-    # def nodeIsOnDomainEdge(self, node0):
-    #     return any([ e[0]==node0 or e[1]==node0 for e in self.convexHullEdges])
-
-    # def pointIsOnDomainEdge(self, pt, node0, node1, weight):
-    #     if (abs(weight)<0.01):
-    #         return self.nodeIsOnDomainEdge(node0)
-    #     if (abs(weight-1.0)<0.01):
-    #         return self.nodeIsOnDomainEdge(node1)
-    #     b0 = [node0, node1] in self.convexHullEdges
-    #     b1 = [node1, node0] in self.convexHullEdges
-    #     if b0 or b1:
-    #         return True
-    #     return False
-
 
 def run_3d( builder:Builder, parameters:Parameters,  start_time=182, end_time=0, pad_num_nodes=0,
-            sedimentsOnly=False, writeout=True, base_flux=None):
+            out_dir = "out-mapA/",sedimentsOnly=False, writeout=True, base_flux=None):
+    logger.setLevel(10)  # numeric level equals DEBUG
+    comm = MPI.COMM_WORLD
     builder=interpolate_all_nodes(builder)
     nums = 4
     dt = parameters.myr2s / nums # time step is 1/4 of 1Ma
     mms2 = []
     mms_tti = []
     tti = 0
     # base_flux = 0.0033
-    out_dir = parameters.output_path / 'results3d'/'layers'
-    out_dir.mkdir(parents=True, exist_ok=True)
+    writeout_final = True
     time_solve = 0.0    
     with Bar('Processing...',check_tty=False, max=(start_time-end_time)) as bar:
         for tti in range(start_time, end_time-1,-1): #start from oldest
             rebuild_mesh = (tti==start_time)
             if rebuild_mesh:
                 logger.info(f"Rebuild/reload mesh at {tti}")          
                 mm2 = UniformNodeGridFixedSizeMeshModel(builder, parameters,sedimentsOnly, padding_num_nodes=pad_num_nodes)
                 mm2.buildMesh(tti)
                 if (base_flux is not None):
                     mm2.baseFluxMagnitude = base_flux
             else:
                 logger.info(f"Re-generating mesh vertices at {tti}")
-                mm2.updateMesh(tti)
+                tic()
+                mm2.updateMesh(tti, optimized=True)
+                toc(msg="update mesh")
             logger.info(f"Solving {tti}")
-
             mm2.useBaseFlux = (base_flux is not None)
             mm2.baseFluxMagnitude = base_flux
 
             if ( len(mms2) == 0):
                 tic()
                 mm2.useBaseFlux = False
                 mm2.setupSolverAndSolve(n_steps=40, time_step = 314712e8 * 2e2, skip_setup=False)   
                 time_solve = time_solve + toc(msg="setup solver and solve")
-            else:
+            else:    
                 mm2.useBaseFlux = (base_flux is not None)
                 tic()
-                mm2.setupSolverAndSolve( n_steps=nums, time_step=dt, skip_setup=(not rebuild_mesh))
+                mm2.setupSolverAndSolve( n_steps=nums, time_step=dt, skip_setup=(not rebuild_mesh), update_bc = mm2.useBaseFlux and (len(mms2) == 1))
                 time_solve = time_solve + toc(msg="setup solver and solve")
             if (writeout):
                 tic()
-                mm2.writeLayerIDFunction(out_dir/f"LayerID-{str(tti)}.xdmf", tti=tti)
-                mm2.writeTemperatureFunction(out_dir+f"Temperature-{str(tti)}.xdmf", tti=tti)
+                mm2.writeLayerIDFunction(out_dir+"LayerID-"+str(tti)+".xdmf", tti=tti)
+                mm2.writeTemperatureFunction(out_dir+"Temperature-"+str(tti)+".xdmf", tti=tti)
                 # mm2.writeOutputFunctions(out_dir+"test4-"+str(tti)+".xdmf", tti=tti)
                 toc(msg="write function")
             
             mms2.append(mm2)
             mms_tti.append(tti)
             logger.info(f"Simulated time step {tti}")
             bar.next()
-    print("total time solve: " , time_solve)
-    if (writeout):
-        resqml_path= parameters.output_path / 'results3d'/'mesh'
-        resqml_path.mkdir(parents=True, exist_ok=True)
-        EPCfilename = mm2.write_hexa_mesh_resqml(resqml_path)
-        print("RESQML model written to: " , EPCfilename)
-        read_mesh_resqml_hexa(EPCfilename)  # test reading of the .epc file
-    return mm2
+    logger.info(f"total time solve 3D: {time_solve}")
+    if (writeout_final):
+        comm.Barrier()
+        if comm.rank>=1:
+            comm.send(mm2.mesh.topology.index_map(0).local_to_global(list(range(mm2.mesh.geometry.x.shape[0]))) , dest=0, tag=((comm.rank-1)*10)+21)
+            comm.send(mm2.mesh_reindex, dest=0, tag=((comm.rank-1)*10)+23)
+            comm.send(mm2.mesh_vertices_age, dest=0, tag=((comm.rank-1)*10)+25)
+            comm.send(mm2.posarr, dest=0, tag=((comm.rank-1)*10)+20)
+            comm.send(mm2.Tarr, dest=0, tag=((comm.rank-1)*10)+24)
+        if comm.rank==0:
+            mm2.receive_mpi_messages()
+            EPCfilename = mm2.write_hexa_mesh_resqml("temp/", end_time)
+            logger.info(f"RESQML model written to: {EPCfilename}")
+            EPCfilename_ts = mm2.write_hexa_mesh_timeseries("temp/")
+            logger.info(f"RESQML partial model with timeseries written to: {EPCfilename_ts}")
+            read_mesh_resqml_hexa(EPCfilename)  # test reading of the .epc file
+    return mm2
```

### Comparing `warmth-0.0.1/warmth/mesh_utils.py` & `warmth-0.0.2/warmth/mesh_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,14 +109,26 @@
     import numpy as np
     ad = points[0]-points[3]
     bd = points[1]-points[3]
     cd = points[2]-points[3]
     bdcd = np.cross(bd,cd)
     return np.linalg.norm(np.dot(ad,bdcd))/6
 
+
+def volumeOfHex(points):
+    """ Computes the volume of a hexahedron, given as eight 3D-points
+    """ 
+    import numpy as np
+    tetsplit1 = [ [1,2,4,8], [1,2,5,8], [4,8,2,3], [2,3,7,8], [2,5,6,8], [2,6,7,8] ]
+    vol = 0.0
+    for f in tetsplit1:
+        tet = points[[p-1 for p in f],:]
+        vol = vol + volumeOfTet(tet)
+    return vol
+
 def interpolateNode(interpolationNodes: List[single_node], interpolationWeights=None) -> single_node:
     assert len(interpolationNodes)>0
     if interpolationWeights is None:
         interpolationWeights = np.ones([len(interpolationNodes),1])
     assert len(interpolationNodes)==len(interpolationWeights)
     wsum = np.sum(np.array(interpolationWeights))
     iWeightNorm = [ w/wsum for w in interpolationWeights]
```

### Comparing `warmth-0.0.1/warmth/model.py` & `warmth-0.0.2/warmth/model.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.1/warmth/parameters.py` & `warmth-0.0.2/warmth/parameters.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.1/warmth/resqpy_helpers.py` & `warmth-0.0.2/warmth/resqpy_helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import numpy as np
 
 import resqpy.property as rqp
 import resqpy.crs as rqc
 import resqpy.model as rq
 import resqpy.olio.uuid as bu
 import resqpy.unstructured as rug
-
+import resqpy.time_series as rts
 
 #
-#  Our example resqml model can be read using the read_mesh_resqml function below.. 
-#  read_mesh_resqml("/path/mapA-961-nodes-182_0.epc")
 # 
 #
 
 def read_mesh_resqml(epcfilename, meshTitle = 'tetramesh'):
     """Example code how to read the .epc file written by the write_tetra_grid_with_properties function.
        Extracts arrays of node positions and of tetrahedra indices.
        Extracts arrays of properties (per-cell and per-node)
@@ -26,47 +24,44 @@
     #
     # read mesh:  vertex positions and cell/tetrahedra definitions
     #
     tetra_uuid = model.uuid(obj_type = 'UnstructuredGridRepresentation', title = meshTitle)
     assert tetra_uuid is not None
     tetra = rug.TetraGrid(model, uuid = tetra_uuid)
     assert tetra is not None
-    print(tetra.title, tetra.node_count, tetra.cell_count, tetra.cell_shape)
+    print(f"Mesh {tetra.title}: {tetra.node_count} nodes, {tetra.cell_count} cells, {tetra.cell_shape} cell shape")
     assert tetra.cell_shape == 'tetrahedral'
     
-    print( tetra.points_ref().shape )   # numpy array of vertex positions
     cells = np.array( [ tetra.distinct_node_indices_for_cell(i) for i in range(tetra.cell_count) ]  ) # cell indices are read using this function(?)
-    print( cells.shape )   # numpy array of vertex positions
     
     tetra.check_tetra()
 
     #
     # read properties
     #
 
     temp_uuid = model.uuid(title = 'Temperature')
     assert temp_uuid is not None
     temp_prop = rqp.Property(model, uuid = temp_uuid)
     assert temp_prop.uom() == 'degC'
     assert temp_prop.indexable_element() == 'nodes'   # properties are defined either on nodes or on cells
-    print( temp_prop.array_ref().shape, temp_prop.array_ref()[0:10] )  # .array_ref() exposes the values as numpy array
 
     layerID_uuid = model.uuid(title = 'LayerID')
     assert layerID_uuid is not None
     layerID_prop = rqp.Property(model, uuid = layerID_uuid)
     # assert layerID_prop.uom() == 'Euc'
     assert layerID_prop.is_continuous() == False
     assert layerID_prop.indexable_element() == 'cells'
-    print( layerID_prop.array_ref().shape, layerID_prop.array_ref()[0:10] )  # .array_ref() exposes the values as numpy array
+    # print( layerID_prop.array_ref().shape, layerID_prop.array_ref()[0:10] )  # .array_ref() exposes the values as numpy array
  
     titles=['Temperature', 'Age', 'LayerID', 'Porosity_initial', 'Porosity_decay', 'Density_solid', 'insulance_thermal', 'Radiogenic_heat_production']
     for title in titles:
         prop_uuid = model.uuid(title = title)
         prop = rqp.Property(model, uuid = prop_uuid)
-        print(title, prop.indexable_element(), prop.uom(), prop.array_ref()[0:10] )
+        print(f"Property {title}: defined on {prop.indexable_element()}, unit {prop.uom()}, first values: {prop.array_ref()[0:10]}")
     
 def write_tetra_grid_with_properties(filename, nodes, cells, modelTitle = "tetramesh",
     Temp_per_vertex=None, age_per_vertex=None, poro0_per_cell=None, decay_per_cell=None, density_per_cell=None,
     cond_per_cell=None, rhp_per_cell=None, lid_per_cell=None ):
     """Writes the given tetrahedral mesh, defined by arrays of nodes and cell indices, into a RESQML .epc file
        Given SubsHeat properties are optionally written.
        NOTE: writing properties that are defines per-node (have 'nodes' as indexable element) requires a patched version of resqpy!
@@ -340,14 +335,18 @@
     face_count = int(len(nodes_per_face)/4)
 
 
     model = rq.new_model(filename)
     crs = rqc.Crs(model)
     crs.create_xml()
 
+    # gts = rts.GeologicTimeSeries(model, title="warmth simulation")
+    # gts.create_time_index(182)
+    # gts.create_xml()
+
     # create an empty HexaGrid
     hexa = rug.HexaGrid(model, title = modelTitle)
     assert hexa.cell_shape == 'hexahedral'
 
     # hand craft all attribute data
     hexa.crs_uuid = model.uuid(obj_type = 'LocalDepth3dCrs')
     assert hexa.crs_uuid is not None
@@ -374,25 +373,25 @@
 
     # write arrays, create xml and store model
     hexa.write_hdf5()
     hexa.create_xml()
 
     if Temp_per_vertex is not None:
         _ = rqp.Property.from_array(model,
-                                    Temp_per_vertex,
+                                    Temp_per_vertex.astype(np.float32),
                                     source_info = 'SubsHeat',
                                     keyword = 'Temperature',
                                     support_uuid = hexa.uuid,
                                     property_kind = 'thermodynamic temperature',
                                     indexable_element = 'nodes',
                                     uom = 'degC')
 
     if age_per_vertex is not None:
         _ = rqp.Property.from_array(model,
-                                    age_per_vertex,
+                                    age_per_vertex.astype(np.float32),
                                     source_info = 'SubsHeat',
                                     keyword = 'Age',
                                     support_uuid = hexa.uuid,
                                     property_kind = 'geological age',
                                     indexable_element = 'nodes',
                                     uom = 'y')
 
@@ -405,56 +404,183 @@
                                     property_kind = 'layer ID',
                                     indexable_element = 'cells',
                                     uom = 'Euc',
                                     discrete=True)
          
     if poro0_per_cell is not None:
         _ = rqp.Property.from_array(model,
-                                    poro0_per_cell,
+                                    poro0_per_cell.astype(np.float32),
                                     source_info = 'SubsHeat',
                                     keyword = 'Porosity_initial',
                                     support_uuid = hexa.uuid,
                                     property_kind = 'porosity',
                                     indexable_element = 'cells',
                                     uom = 'm3/m3')
     if decay_per_cell is not None:
         _ = rqp.Property.from_array(model,
-                                    decay_per_cell,
+                                    decay_per_cell.astype(np.float32),
                                     source_info = 'SubsHeat',
                                     keyword = 'Porosity_decay',
                                     support_uuid = hexa.uuid,
                                     property_kind = 'porosity decay',
                                     indexable_element = 'cells',
                                     uom = 'Euc')
     if density_per_cell is not None:
         _ = rqp.Property.from_array(model,
-                                    density_per_cell,
+                                    density_per_cell.astype(np.float32),
                                     source_info = 'SubsHeat',
                                     keyword = 'Density_solid',
                                     support_uuid = hexa.uuid,
                                     property_kind = 'density',
                                     indexable_element = 'cells',
                                     uom = 'kg/m3')
     if cond_per_cell is not None:
         #
         # we write thermal conductivity as its inverse, the thermal insulance
         #
         _ = rqp.Property.from_array(model,
-                                    np.reciprocal(cond_per_cell),
+                                    np.reciprocal(cond_per_cell).astype(np.float32),
                                     source_info = 'SubsHeat',
                                     keyword = 'insulance_thermal',
                                     support_uuid = hexa.uuid,
                                     property_kind = 'thermal insulance',
                                     indexable_element = 'cells',
                                     uom = 'deltaK.m2/W')
     if rhp_per_cell is not None:
         _ = rqp.Property.from_array(model,
-                                    rhp_per_cell,
+                                    rhp_per_cell.astype(np.float32),
                                     source_info = 'SubsHeat',
                                     keyword = 'Radiogenic_heat_production',
                                     support_uuid = hexa.uuid,
                                     property_kind = 'heat',
                                     indexable_element = 'cells',
                                     uom = 'W/m3')
 
     model.store_epc()
 
+
+def write_hexa_grid_with_timeseries(filename, nodes_series, cells, modelTitle = "hexamesh",
+    Temp_per_vertex_series=None ):
+    """Writes the given hexahedral mesh, defined by arrays of nodes and cell indices, into a RESQML .epc file
+       Given SubsHeat properties are optionally written.
+ 
+       cells is an array of 8-arrays in which the nodes are ordered:     
+               7------6
+              /      /|
+             /      / |
+            4------5  |
+            |         |
+            |  3------2
+            | /      /
+            |/      /
+            0------1
+
+       NOTE: writing properties that are defines per-node (have 'nodes' as indexable element) requires a patched version of resqpy!
+    """
+
+    nodes = nodes_series[0]
+    node_count = len(nodes)
+    faces_per_cell = []
+    nodes_per_face = []
+    faces_dict = {}
+    faces_repeat = np.zeros(node_count*100, dtype = bool)
+
+    cell_face_is_right_handed = np.zeros( len(cells)*6, dtype = bool)
+    for ih,hexa in enumerate(cells):
+        faces= [[0,3,2,1], [0,1,5,4], [1,2,6,5], [2,3,7,6], [3,0,4,7], [4,5,6,7]]
+        for iq,quad in enumerate(faces):
+            face0 = [hexa[x] for x in quad ]
+            assert -1 not in face0
+            fkey0 = ( x for x in sorted(face0) )
+            #
+            # keep track of which faces are encountered once vs. more than once
+            # faces that are encountered the second time will need to use the reverse handedness
+            #
+            face_is_repeated = False
+            if (fkey0 not in faces_dict):
+                faces_dict[fkey0] = len(nodes_per_face)
+                nodes_per_face.extend(face0)
+                cell_face_is_right_handed[(ih*6 + iq)] = False
+            else:
+                face_is_repeated = True
+                cell_face_is_right_handed[(ih*6 + iq)] = True
+            fidx0 = faces_dict.get(fkey0)            
+            faces_per_cell.append(fidx0/4)
+            faces_repeat[int(fidx0/4)] = face_is_repeated
+    
+    set_cell_count = int(len(faces_per_cell)/6)
+    face_count = int(len(nodes_per_face)/4)
+
+
+    model = rq.new_model(filename)
+    crs = rqc.Crs(model)
+    crs.create_xml()
+
+    times_in_years = [ max(int(t*1e6),1) for t in list(range(len(nodes_series)-1,-1,-1))]
+    gts = rts.GeologicTimeSeries.from_year_list(model, times_in_years, title="warmth simulation")
+    gts.create_xml()
+    rts.timeframe_for_time_series_uuid(model, gts.uuid)
+
+    # create an empty HexaGrid
+    hexa = rug.HexaGrid(model, title = modelTitle)
+    assert hexa.cell_shape == 'hexahedral'
+
+    # hand craft all attribute data
+    hexa.crs_uuid = model.uuid(obj_type = 'LocalDepth3dCrs')
+    assert hexa.crs_uuid is not None
+    assert bu.matching_uuids(hexa.crs_uuid, crs.uuid)
+    hexa.set_cell_count(set_cell_count)
+    # faces
+    hexa.face_count = face_count
+    hexa.faces_per_cell_cl = np.arange(6, 6 * set_cell_count + 1, 6, dtype = int)
+    hexa.faces_per_cell = np.array(faces_per_cell)
+
+    # nodes
+    hexa.node_count = node_count
+    hexa.nodes_per_face_cl = np.arange(4, 4 * face_count + 1, 4, dtype = int)
+    hexa.nodes_per_face = np.array(nodes_per_face)
+
+    # face handedness
+    hexa.cell_face_is_right_handed = cell_face_is_right_handed  # False for all faces for external cells
+
+    # points
+    hexa.points_cached = nodes
+
+    # basic validity check
+    hexa.check_hexahedral()
+
+    hexa.create_xml()
+    hexa.write_hdf5()
+
+    if hexa.property_collection is None:
+        hexa.property_collection = rqp.PropertyCollection(support = hexa)
+    pc = hexa.property_collection
+
+    # nodes0 = nodes.copy()
+    for time_index in range(len(nodes_series)-1,-1,-1):
+        # nodes2 = nodes0 + [0,0,time_index*10]
+        nodes2 = nodes_series[time_index].astype(np.float32)
+        pc.add_cached_array_to_imported_list(nodes2,
+                                                'dynamic nodes',
+                                                'points',
+                                                uom = 'm',
+                                                property_kind = 'length',
+                                                realization = 0,
+                                                time_index = time_index,
+                                                indexable_element = 'nodes',
+                                                points = True)
+        # active_array = np.ones([2160], dtype = bool)
+        tt = Temp_per_vertex_series[time_index].astype(np.float32)
+        pc.add_cached_array_to_imported_list(tt,
+                                                'Temperature',
+                                                'Temperature',
+                                                uom = 'degC',
+                                                property_kind = 'thermodynamic temperature',
+                                                realization = 0,
+                                                time_index = time_index,
+                                                indexable_element = 'nodes')
+                                                # points = True)
+    pc.write_hdf5_for_imported_list()
+    pc.create_xml_for_imported_list_and_add_parts_to_model(time_series_uuid = gts.uuid)
+
+    model.store_epc()
+
```

### Comparing `warmth-0.0.1/warmth/simulator.py` & `warmth-0.0.2/warmth/simulator.py`

 * *Files 11% similar despite different names*

```diff
@@ -107,41 +107,53 @@
     def dump_input_nodes(self, node: single_node):
         filename = node._name + '.pickle'
         p = self._nodes_path / filename
 
         node._dump(p)
         return p
 
-    def dump_input_data(self):
+    def dump_input_data(self, use_mpi=False):
         p = []
         parameter_data_path = self._parameters_path
-        self._builder.parameters.dump(self._parameters_path)
-        if isinstance(self._builder.grid,type(None)) is False:
-            self._builder.grid.dump(self._grid_path)
-        with concurrent.futures.ThreadPoolExecutor(max_workers=10) as th:
-            futures = [th.submit(self.dump_input_nodes,  i)
-                       for i in self._builder.iter_node() if i is not False]
-            for future in concurrent.futures.as_completed(futures):
-                p.append([parameter_data_path, future.result()])
+
+        from mpi4py import MPI
+        comm = MPI.COMM_WORLD        
+        if (comm.rank==0):
+            self._builder.parameters.dump(self._parameters_path)
+            if isinstance(self._builder.grid,type(None)) is False:
+                self._builder.grid.dump(self._grid_path)                
+            if use_mpi:
+                from mpi4py.futures import MPIPoolExecutor
+                with MPIPoolExecutor(max_workers=10) as th:
+                    futures = [th.submit(self.dump_input_nodes,  i)
+                            for i in self._builder.iter_node() if i is not False]
+                    for future in concurrent.futures.as_completed(futures):
+                        p.append([parameter_data_path, future.result()])
+            else:
+                with concurrent.futures.ThreadPoolExecutor(max_workers=10) as th:
+                    futures = [th.submit(self.dump_input_nodes,  i)
+                            for i in self._builder.iter_node() if i is not False]
+                    for future in concurrent.futures.as_completed(futures):
+                        p.append([parameter_data_path, future.result()])
         return p
 
     def setup_directory(self, purge=False):
         if self._builder.parameters.output_path.exists():
             if purge:
                 from shutil import rmtree
                 rmtree(self._builder.parameters.output_path)
             else:
                 raise Exception(
                     f'Output directory {self._builder.parameters.output_path} already exist. Use purge=True to delete existing data')
         self._nodes_path.mkdir(parents=True, exist_ok=True)
         return
 
-    def run(self, save=False,purge=False,parallel=True):
+    def run(self, save=False,purge=False,parallel=True,use_mpi=True):
         if parallel:
-            self._parellel_run(save,purge)
+            self._parellel_run(save,purge,use_mpi=use_mpi)
         else:
             if self.simulate_every != 1:
                 logger.warning("Serial simulation will run full simulation on all nodes")
             for i in self._builder.iter_node():
                 self.forward_modelling.current_node=i
                 self.forward_modelling.simulate_single_node()
         return
@@ -173,47 +185,69 @@
                     if isinstance(self._builder.nodes[index[0]][index[1]],bool) is False:
                         self._builder.nodes[index[0]][index[1]]._full_simulation = False
                         count+=1
 
         if count >0:
             logger.info(f"Setting {count} nodes to partial simulation")
         return count
-    def _parellel_run(self, save,purge):
+
+
+    def _parellel_run(self, save, purge, use_mpi=False):
         filtered = self._filter_full_sim()
-        self.setup_directory(purge)
-        p = self.dump_input_data()
-        #self._builder.nodes=self._builder.grid.make_grid_arr()
-        with concurrent.futures.ProcessPoolExecutor(mp_context=get_context('spawn')) as executor:
-            results = [executor.submit(runWorker, i) for i in p]
-            with Bar('Processing...',check_tty=False, max=len(p)) as bar:
-                for future in concurrent.futures.as_completed(results):
-                    bar.next()
-                    try:
-                        path_result = future.result()
-                        n= load_node(path_result) # numerical model error should still resovle
-                        if save==False:
-                            path_result.unlink()
-                        self.put_node_to_grid(n)
-                    except Exception as e:
-                        logger.error(e)
+        from mpi4py import MPI
+        comm = MPI.COMM_WORLD        
+        if (comm.rank==0):
+            self.setup_directory(purge)
+        p = self.dump_input_data(use_mpi=use_mpi)
+
+        if use_mpi:
+            from mpi4py.futures import MPIPoolExecutor
+            with MPIPoolExecutor(max_workers=20) as executor:
+                results = [executor.submit(runWorker, i) for i in p]
+                with Bar('Processing...',check_tty=False, max=len(p)) as bar:
+                    for future in concurrent.futures.as_completed(results):
+                        bar.next()
+                        try:
+                            path_result = future.result()
+                            n= load_node(path_result) # numerical model error should still resovle
+                            if save==False:
+                                path_result.unlink()
+                            self.put_node_to_grid(n)
+                        except Exception as e:
+                            logger.error(e)
+        else:
+            with concurrent.futures.ProcessPoolExecutor(mp_context=get_context('spawn')) as executor:
+                results = [executor.submit(runWorker, i) for i in p]
+                with Bar('Processing...',check_tty=False, max=len(p)) as bar:
+                    for future in concurrent.futures.as_completed(results):
+                        bar.next()
+                        try:
+                            path_result = future.result()
+                            n= load_node(path_result) # numerical model error should still resovle
+                            if save==False:
+                                path_result.unlink()
+                            self.put_node_to_grid(n)
+                        except Exception as e:
+                            logger.error(e)
         # pick up node with no results (failed)
-        for node_path in self._nodes_path.iterdir():
-            str_f = str(node_path)
-            if str_f.endswith(".pickle"):
-                n=load_node(node_path)
-                if save==False:
-                    node_path.unlink()
-                self.put_node_to_grid(n)
-                logger.warning(f"No result file for node X:{n.X}, Y:{n.Y}")
-        if save==False:
-            from shutil import rmtree
-            rmtree(self._builder.parameters.output_path)
-        if filtered >0:
-            logger.info(f"Interpolating results back to {filtered} partial simulated nodes")
-            interp_res= Results_interpolator(self._builder,len(p)-filtered)
-            interp_res.run()
+        if comm.rank==0:                            
+            for node_path in self._nodes_path.iterdir():
+                str_f = str(node_path)
+                if str_f.endswith(".pickle"):
+                    n=load_node(node_path)
+                    if save==False:
+                        node_path.unlink()
+                    self.put_node_to_grid(n)
+                    logger.warning(f"No result file for node X:{n.X}, Y:{n.Y}")
+            if save==False:
+                from shutil import rmtree
+                rmtree(self._builder.parameters.output_path)
+            if filtered >0:
+                logger.info(f"Interpolating results back to {filtered} partial simulated nodes")
+                interp_res= Results_interpolator(self._builder,len(p)-filtered)
+                interp_res.run()
         return
     def put_node_to_grid(self,node:single_node):
         self._builder.nodes[node.indexer[0]][node.indexer[1]]=node
         return
```

### Comparing `warmth-0.0.1/warmth/utils.py` & `warmth-0.0.2/warmth/utils.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.1/PKG-INFO` & `warmth-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: warmth
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Adam Cheng
 Author-email: 52572642+adamchengtkc@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: meshio[all] (>=5.3.4,<6.0.0)
 Requires-Dist: numpy (>=1.26.0,<2.0.0)
 Requires-Dist: pandas (<2.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: progress (>=1.6,<2.0)
 Requires-Dist: resqpy (>=4.12.1,<5.0.0)
 Requires-Dist: scipy (>=1.11.3,<2.0.0)
 Requires-Dist: urllib3 (>=2.0.6,<3.0.0)
 Requires-Dist: xtgeo (>=3.4.0,<4.0.0)
 Description-Content-Type: text/markdown
```

