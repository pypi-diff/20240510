# Comparing `tmp/dsplus-0.5.1.tar.gz` & `tmp/dsplus-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.5.1.tar", last modified: Fri May 10 00:16:47 2024, max compression
+gzip compressed data, was "dsplus-0.5.2.tar", last modified: Fri May 10 01:21:35 2024, max compression
```

## Comparing `dsplus-0.5.1.tar` & `dsplus-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 00:16:47.527594 dsplus-0.5.1/
--rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.5.1/LICENSE
--rw-rw-rw-   0        0        0      895 2024-05-10 00:16:47.522133 dsplus-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-05-10 00:15:58.000000 dsplus-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 00:16:47.479007 dsplus-0.5.1/dsplus/
--rw-rw-rw-   0        0        0      171 2024-05-10 00:14:12.000000 dsplus-0.5.1/dsplus/__init__.py
--rw-rw-rw-   0        0        0    25485 2024-05-07 12:38:31.000000 dsplus-0.5.1/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    43727 2024-05-07 13:06:53.000000 dsplus-0.5.1/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    57143 2024-05-08 02:06:30.000000 dsplus-0.5.1/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    59122 2024-05-06 04:39:55.000000 dsplus-0.5.1/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:16:47.506667 dsplus-0.5.1/dsplus.egg-info/
--rw-rw-rw-   0        0        0      895 2024-05-10 00:16:47.000000 dsplus-0.5.1/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-10 00:16:47.000000 dsplus-0.5.1/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 00:16:47.000000 dsplus-0.5.1/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-10 00:16:47.000000 dsplus-0.5.1/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 00:16:47.529039 dsplus-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      982 2024-05-10 00:11:27.000000 dsplus-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 00:16:47.511347 dsplus-0.5.1/tests/
--rw-rw-rw-   0        0        0    13083 2024-05-07 12:46:09.000000 dsplus-0.5.1/tests/Test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:21:35.291924 dsplus-0.5.2/
+-rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0      895 2024-05-10 01:21:35.288574 dsplus-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-10 00:15:58.000000 dsplus-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 01:21:35.267385 dsplus-0.5.2/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-05-10 01:21:24.000000 dsplus-0.5.2/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    25485 2024-05-07 12:38:31.000000 dsplus-0.5.2/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    43727 2024-05-07 13:06:53.000000 dsplus-0.5.2/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    57174 2024-05-10 01:20:50.000000 dsplus-0.5.2/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    62215 2024-05-10 01:20:55.000000 dsplus-0.5.2/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:21:35.280987 dsplus-0.5.2/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      895 2024-05-10 01:21:35.000000 dsplus-0.5.2/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-10 01:21:35.000000 dsplus-0.5.2/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 01:21:35.000000 dsplus-0.5.2/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 01:21:35.000000 dsplus-0.5.2/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 01:21:35.291924 dsplus-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      982 2024-05-10 00:11:27.000000 dsplus-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 01:21:35.281983 dsplus-0.5.2/tests/
+-rw-rw-rw-   0        0        0    13083 2024-05-07 12:46:09.000000 dsplus-0.5.2/tests/Test_pandas.py
```

### Comparing `dsplus-0.5.1/LICENSE` & `dsplus-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsplus-0.5.1/PKG-INFO` & `dsplus-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.5.1
+Version: 0.5.2
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.5.1/dsplus/pb_functions_general.py` & `dsplus-0.5.2/dsplus/pb_functions_general.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.5.1/dsplus/pb_functions_pandas.py` & `dsplus-0.5.2/dsplus/pb_functions_pandas.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.5.1/dsplus/pb_functions_plotly.py` & `dsplus-0.5.2/dsplus/pb_functions_plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#region Libraries   
+#region Libraries
 
 #%%
 from typing import Literal, Self, Callable, Any
 
 import pandas as pd
 import numpy as np
 
@@ -35,14 +35,16 @@
         else:
             fig_original = fig
     return fig_original
 
 #endregion -----------------------------------------------------------------------------------------
 #region Class
 
+#TODO Documentation for add_*.
+
 #%%
 class px_Plot():
     '''An interface for declaratively creating plotly plots.
 
     Following are the main methods:
         - facet(): Add faceting.
         - marginal(): Add marginal plots.
```

### Comparing `dsplus-0.5.1/dsplus/pb_functions_spatial.py` & `dsplus-0.5.2/dsplus/pb_functions_spatial.py`

 * *Files 2% similar despite different names*

```diff
@@ -588,275 +588,113 @@
                 df_values = df_values.pipe(pd_concat_rows, temp_df_values)
 
             return (df_values)
 
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: Plotly
 
-#TODO Documentation
+#TODO Documentation for add_*.
 
 #%%
-def px_sp_create_map(sp = None, center_lon=-95.7129, center_lat=37.0902, zoom=2.5, **kwargs):
-    if sp is not None:
-        if sp.crs.to_epsg() != Options_epsg.wgs84.value:
-            sp = sp.to_crs(Options_epsg.wgs84.value)
-
-        temp_centroid = gpd.GeoDataFrame(geometry=sp.centroid)
-        center_lon = temp_centroid.geometry.x.mean()
-        center_lat = temp_centroid.geometry.y.mean()
-        # temp_bounds = sp.bounds
-        # temp_del_x = temp_bounds['maxx'].max() - temp_bounds['minx'].min()
-        # temp_del_y = temp_bounds['maxy'].max() - temp_bounds['miny'].min()
-        # zoom_x = 360/temp_del_x
-        # zoom_y = 180/temp_del_y
-    fig = px.choropleth_mapbox(center=dict(lon=center_lon,
-                                           lat=center_lat),
-                               zoom=zoom,
-                               **kwargs)
-    return fig
-
-#%%
-def px_add_trace_data(fig_original, *figs):
-    # TODO not working (only takes first fig)
-    for fig in figs:
-        for i in range(len(fig.data)):
-            fig_original.add_trace(fig.data[i])
-        return fig_original
-
-#%%
-def px_sp_basemap(fig, basemap):
-    if pd.Series(dir(Options_px_tiles)).str.contains(basemap).any():
-        fig.update_layout(
-            mapbox_style="white-bg",
-            mapbox_layers=[
-                {
-                    "below": "traces",
-                    "sourcetype": "raster",
-                    # "sourceattribution": "United States Geological Survey",
-                    "source": [Options_px_tiles[basemap].value],
-                }
-            ],
-        )
-    else:
-        fig.update_layout(mapbox_style=basemap)
-
-#%%
-def px_sp_points(sp_points,
-                 color_value = None,
-                 size_value = None,
-                 symbol_value = None,
-                 legend_name = None,
-                 hover_skip = False,
-                 update_crs = True,
-                 **kwargs):
-    if update_crs:
-        if sp_points.crs.to_epsg() != Options_epsg.wgs84.value:
-            sp_points = sp_points.to_crs(Options_epsg.wgs84.value)
-    fig = px.scatter_mapbox(sp_points,
-                            lon=sp_points.geometry.x,
-                            lat=sp_points.geometry.y,
-                            **kwargs)
-    if color_value is not None:
-        fig = fig\
-            .update_traces(marker=dict(color=color_value))
-    if size_value is not None:
-        fig = fig\
-            .update_traces(marker=dict(size=size_value))
-    if symbol_value is not None:
-        fig = fig\
-            .update_traces(marker=dict(symbol=symbol_value))
-    if legend_name is not None:
-        if ('color' not in kwargs) and ('size' not in kwargs):
-            fig = fig\
-                .update_traces(name=legend_name,
-                               showlegend=True)
-        else:
-            fig = fig\
-                .update_traces(legendgroup=legend_name,
-                               legendgrouptitle_text=legend_name,
-                               showlegend=True)
-    if hover_skip:
-        fig = fig\
-            .update_traces(hoverinfo='skip',
-                           hovertemplate=None)
-    return fig
-
-#%%
-def px_sp_polylines(sp_lines,
-                    color_value = None,
-                    width_value = None,
-                    dash_value = None,
-                    legend_name = None,
-                    hover_skip = False,
-                    update_crs = True,
-                    **kwargs):
-    if update_crs:
-        if sp_lines.crs.to_epsg() != Options_epsg.wgs84.value:
-            sp_lines = sp_lines.to_crs(Options_epsg.wgs84.value)
-    df_lines_xy = sp_to_df_xy(sp_lines, cols_keep_all=True)
-    fig = px.line_mapbox(df_lines_xy,
-                         lon=df_lines_xy['x'],
-                         lat=df_lines_xy['y'],
-                         line_group=df_lines_xy['id_geom'],
-                         **kwargs)
-    if color_value is not None:
-        fig = fig\
-            .update_traces(line=dict(color=color_value))
-    if width_value is not None:
-        fig = fig\
-            .update_traces(line=dict(width=width_value))
-    if dash_value is not None:
-        fig = fig\
-            .update_traces(line=dict(dash=dash_value))
-    if legend_name is not None:
-        if 'color' not in kwargs:
-            fig = fig\
-                .update_traces(name=legend_name,
-                               legendgroup=legend_name,
-                               showlegend=True)
-        else:
-            fig = fig\
-                .update_traces(legendgroup=legend_name,
-                               legendgrouptitle_text=legend_name,
-                               showlegend=True)
-    if 'color' not in kwargs:
-        for i in range(len(fig.data)):
-            if i == 0:
-                fig.data[i].showlegend = True
-            else:
-                fig.data[i].showlegend = False
-    if hover_skip:
-        fig = fig\
-            .update_traces(hoverinfo='skip',
-                           hovertemplate=None)
-    return fig
+class px_Map(px_Plot):
+    '''An interface for declaratively creating plotly maps.
 
-#%%
-def px_sp_polygons(sp_polygons,
-                   color_value = None,
-                   line_color = None,
-                   line_width = None,
-                   line_dash = None,
-                   legend_name = None,
-                   hover_skip = False,
-                   update_crs = True,
-                   **kwargs):
-    if update_crs:
-        if sp_polygons.crs.to_epsg() != Options_epsg.wgs84.value:
-            sp_polygons = sp_polygons.to_crs(Options_epsg.wgs84.value)
-    if color_value is not None:
-        kwargs['color_discrete_sequence'] = [color_value, color_value]
-    fig = px.choropleth_mapbox(sp_polygons,
-                               locations=sp_polygons.index,
-                               geojson=sp_polygons.geometry,
-                               **kwargs)
-    if line_color is not None:
-        fig = fig\
-            .update_traces(marker=dict(line=dict(color=line_color)))
-    if line_width is not None:
-        fig = fig\
-            .update_traces(marker=dict(line=dict(width=line_width)))
-    if line_dash is not None:
-        fig = fig\
-            .update_traces(marker=dict(line=dict(dash=line_dash)))
-    if legend_name is not None:
-        if 'color' not in kwargs:
-            fig = fig\
-                .update_traces(name=legend_name,
-                               legendgroup=legend_name,
-                               showlegend=True)
-        else:
-            fig = fig\
-                .update_traces(legendgroup=legend_name,
-                               legendgrouptitle_text=legend_name,
-                               showlegend=True)
-    if hover_skip:
-        fig = fig\
-            .update_traces(hoverinfo='skip',
-                           hovertemplate=None)
-    return fig
+    Following are the main methods:
+        - add_*(): Add different traces. Not all traces have been implemented. Main ones are:
+            - add_sp_points(): Add points geodataframe.
+            - add_sp_polylines(): Add polylines geodataframe.
+            - add_sp_polygons(): Add polygons geodataframe.
+            - add_sp_poygon_borders(): Add polygons geodataframe as borders.
+            - add_sp_basemap(): Add basemap.
+        - add(): Add traces directly from plotly trace objects.
+        - label(): Add x and y labels and plot title.
+        - legend(): Update legend properties.
+        - colorbar(): Update colorbar legend properties.
+        - size(): Update plot size.
+        - layout(): Update layout properties.
+        - show(): Show plot.
+        - get_fig(): Get figure object.
 
-#%%
-def px_sp_polygon_borders(sp_polygons,
-                          line_color = None,
-                          line_width = None,
-                          line_dash = None,
-                          legend_name = None,
-                          hover_skip = True,
-                          update_crs = True,
-                          **kwargs):
-    if update_crs:
-        if sp_polygons.crs.to_epsg() != Options_epsg.wgs84.value:
-            sp_polygons = sp_polygons.to_crs(Options_epsg.wgs84.value)
-    df_polygons_xy = sp_to_df_xy(sp_polygons, cols_keep_all=True)
-    fig = px.line_mapbox(df_polygons_xy,
-                         lon=df_polygons_xy['x'],
-                         lat=df_polygons_xy['y'],
-                         line_group=df_polygons_xy['id_geom'])
-    if line_color is not None:
-        fig = fig\
-            .update_traces(line=dict(color=line_color))
-    if line_width is not None:
-        fig = fig\
-            .update_traces(line=dict(width=line_width))
-    if line_dash is not None:
-        fig = fig\
-            .update_traces(line=dict(dash=line_dash))
-    if legend_name is not None:
-        if 'color' not in kwargs:
-            fig = fig\
-                .update_traces(name=legend_name,
-                               legendgroup=legend_name,
-                               showlegend=True)
-        else:
-            fig = fig\
-                .update_traces(legendgroup=legend_name,
-                               legendgrouptitle_text=legend_name,
-                               showlegend=True)
-    if 'color' not in kwargs:
-        for i in range(len(fig.data)):
-            if i == 0:
-                fig.data[i].showlegend = True
-            else:
-                fig.data[i].showlegend = False
-    if hover_skip:
-        fig = fig\
-            .update_traces(hoverinfo='skip',
-                           hovertemplate=None)
-    return fig
-
-#%%
-class px_Map(px_Plot):
+    Examples:
+        >>> (ds.px_Map(sp=sp_states, zoom=2.5)
+                .add_sp_polygons(sp_states,
+                                color='water_prop',
+                                legend_name='States',
+                                hover_skip=True)
+                .add_sp_polylines(sp_roads,
+                                color_value='red',
+                                width_value=3,
+                                legend_name='Roads',
+                                hover_name='FULLNAME',
+                                hover_data=dict(x=False,
+                                                y=False,
+                                                id_geom=False,
+                                                LINEARID=True))
+                .add_sp_points(sp_capitals,
+                               color_value='green',
+                               size_value=8,
+                               legend_name='Capitals',
+                               hover_name='name',
+                               hover_data=['state'])
+                .add_sp_polygon_borders(sp_states,
+                                        line_color='black',
+                                        line_width=2,
+                                        legend_name='States Boundary')
+                .add_sp_basemap(ds.Options_px_basemap.carto_darkmatter.value)
+                .legend(x_anchor='right',
+                        y_anchor='bottom',
+                        x=1,
+                        y=0.1)
+                .colorbar(title='Water%',
+                        orientation='h',
+                        x_anchor='left',
+                        y_anchor='bottom',
+                        x=0,
+                        y=0,
+                        thickness=10,
+                        len=0.5)
+                .layout(margins=[0,0,0,0])
+                .show()
+            )
+    '''
     fig = None
 
     def __init__(self,
                  sp=None,
-                 center_lon=-95.7129, 
-                 center_lat=37.0902, 
-                 zoom=2.5, 
+                 center_lon=-95.7129,
+                 center_lat=37.0902,
+                 zoom=2.5,
                  **kwargs) -> None:
         if sp is not None:
             if sp.crs.to_epsg() != Options_epsg.wgs84.value:
                 sp = sp.to_crs(Options_epsg.wgs84.value)
-        
+
             temp_centroid = gpd.GeoDataFrame(geometry=sp.centroid)
             center_lon = temp_centroid.geometry.x.mean()
             center_lat = temp_centroid.geometry.y.mean()
         fig = px.choropleth_mapbox(center=dict(lon=center_lon,
                                                lat=center_lat),
                                    zoom=zoom,
                                    **kwargs)
-        
+
         self.fig = fig
 
         self.add_sp_basemap(Options_px_basemap.none.value)
-        
-    def add_sp_basemap(self, basemap):
+
+    def add_sp_basemap(self, basemap: str) -> Self:
+        '''Add basemap.
+
+        Args:
+            basemap (str): Use `Options_px_basemap`. Or see 'Base Maps in layout.mapbox.style' in https://plotly.com/python/mapbox-layers/.
+
+        Returns:
+            Self: Self object.
+        '''
         fig = self.fig
-        
+
         if pd.Series(dir(Options_px_tiles)).str.contains(basemap).any():
             fig.update_layout(
                 mapbox_style="white-bg",
                 mapbox_layers=[
                     {
                         "below": "traces",
                         "sourcetype": "raster",
@@ -865,48 +703,52 @@
                     }
                 ],
             )
         else:
             fig.update_layout(mapbox_style=basemap)
 
         return self
-        
+
     def _dec_add_sp():
+        '''Decorator to make the following updates:
+            - Geodataframe coordiantes.
+            - Hover arguemnts
+        '''
         def inner(func):
             def wrapper(self, *args, **kwargs):
                 kwargs = combine_arguments(func, [0, *args], kwargs)
                 kwargs.pop('self')
 
                 update_crs = kwargs['update_crs']
-                
+
                 if update_crs:
                     sp = kwargs['sp']
 
                     if sp.crs.to_epsg() != Options_epsg.wgs84.value:
                         sp = sp.to_crs(Options_epsg.wgs84.value)
 
                     kwargs['sp'] = sp
-                
+
                 trace = func(self, **kwargs)
 
                 hover_skip_check = kwargs['hover_skip']
 
                 if hover_skip_check:
                     trace = \
                     (trace
                         .update_traces(hoverinfo='skip',
                                        hovertemplate=None)
-                    )                
+                    )
 
                 self.add(trace)
 
                 return self
             return wrapper
         return inner
-    
+
     @_dec_add_sp()
     def add_sp_points(self,
                       sp,
                       color_value = None,
                       size_value = None,
                       symbol_value = None,
                       legend_name = None,
@@ -942,17 +784,17 @@
             else:
                 trace = \
                 (trace
                     .update_traces(legendgroup=legend_name,
                                    legendgrouptitle_text=legend_name,
                                    showlegend=True)
                 )
-            
+
         return trace
-    
+
     @_dec_add_sp()
     def add_sp_polylines(self,
                          sp,
                          color_value = None,
                          width_value = None,
                          dash_value = None,
                          legend_name = None,
@@ -997,15 +839,15 @@
                 )
         if 'color' not in kwargs:
             for i in range(len(trace.data)):
                 if i == 0:
                     trace.data[i].showlegend = True
                 else:
                     trace.data[i].showlegend = False
-            
+
         return trace
 
     @_dec_add_sp()
     def add_sp_polygons(self,
                         sp,
                         color_value = None,
                         line_color = None,
@@ -1047,15 +889,15 @@
             else:
                 trace = \
                 (trace
                     .update_traces(legendgroup=legend_name,
                                    legendgrouptitle_text=legend_name,
                                    showlegend=True)
                 )
-            
+
         return trace
 
     @_dec_add_sp()
     def add_sp_polygon_borders(self,
                                sp,
                                line_color = None,
                                line_width = None,
@@ -1204,14 +1046,244 @@
     '''
     return (gpd.GeoDataFrame.from_features(gpd.GeoSeries([sp.geometry.iloc[0].offset_curve(distance, join_style=join_style)])))
 
 #endregion -----------------------------------------------------------------------------------------
 #region Archive
 
 #%%
+def px_sp_create_map(sp = None, center_lon=-95.7129, center_lat=37.0902, zoom=2.5, **kwargs):
+    if sp is not None:
+        if sp.crs.to_epsg() != Options_epsg.wgs84.value:
+            sp = sp.to_crs(Options_epsg.wgs84.value)
+
+        temp_centroid = gpd.GeoDataFrame(geometry=sp.centroid)
+        center_lon = temp_centroid.geometry.x.mean()
+        center_lat = temp_centroid.geometry.y.mean()
+        # temp_bounds = sp.bounds
+        # temp_del_x = temp_bounds['maxx'].max() - temp_bounds['minx'].min()
+        # temp_del_y = temp_bounds['maxy'].max() - temp_bounds['miny'].min()
+        # zoom_x = 360/temp_del_x
+        # zoom_y = 180/temp_del_y
+    fig = px.choropleth_mapbox(center=dict(lon=center_lon,
+                                           lat=center_lat),
+                               zoom=zoom,
+                               **kwargs)
+    return fig
+
+#%%
+def px_add_trace_data(fig_original, *figs):
+    # TODO not working (only takes first fig)
+    for fig in figs:
+        for i in range(len(fig.data)):
+            fig_original.add_trace(fig.data[i])
+        return fig_original
+
+#%%
+def px_sp_basemap(fig, basemap):
+    if pd.Series(dir(Options_px_tiles)).str.contains(basemap).any():
+        fig.update_layout(
+            mapbox_style="white-bg",
+            mapbox_layers=[
+                {
+                    "below": "traces",
+                    "sourcetype": "raster",
+                    # "sourceattribution": "United States Geological Survey",
+                    "source": [Options_px_tiles[basemap].value],
+                }
+            ],
+        )
+    else:
+        fig.update_layout(mapbox_style=basemap)
+
+#%%
+def px_sp_points(sp_points,
+                 color_value = None,
+                 size_value = None,
+                 symbol_value = None,
+                 legend_name = None,
+                 hover_skip = False,
+                 update_crs = True,
+                 **kwargs):
+    if update_crs:
+        if sp_points.crs.to_epsg() != Options_epsg.wgs84.value:
+            sp_points = sp_points.to_crs(Options_epsg.wgs84.value)
+    fig = px.scatter_mapbox(sp_points,
+                            lon=sp_points.geometry.x,
+                            lat=sp_points.geometry.y,
+                            **kwargs)
+    if color_value is not None:
+        fig = fig\
+            .update_traces(marker=dict(color=color_value))
+    if size_value is not None:
+        fig = fig\
+            .update_traces(marker=dict(size=size_value))
+    if symbol_value is not None:
+        fig = fig\
+            .update_traces(marker=dict(symbol=symbol_value))
+    if legend_name is not None:
+        if ('color' not in kwargs) and ('size' not in kwargs):
+            fig = fig\
+                .update_traces(name=legend_name,
+                               showlegend=True)
+        else:
+            fig = fig\
+                .update_traces(legendgroup=legend_name,
+                               legendgrouptitle_text=legend_name,
+                               showlegend=True)
+    if hover_skip:
+        fig = fig\
+            .update_traces(hoverinfo='skip',
+                           hovertemplate=None)
+    return fig
+
+#%%
+def px_sp_polylines(sp_lines,
+                    color_value = None,
+                    width_value = None,
+                    dash_value = None,
+                    legend_name = None,
+                    hover_skip = False,
+                    update_crs = True,
+                    **kwargs):
+    if update_crs:
+        if sp_lines.crs.to_epsg() != Options_epsg.wgs84.value:
+            sp_lines = sp_lines.to_crs(Options_epsg.wgs84.value)
+    df_lines_xy = sp_to_df_xy(sp_lines, cols_keep_all=True)
+    fig = px.line_mapbox(df_lines_xy,
+                         lon=df_lines_xy['x'],
+                         lat=df_lines_xy['y'],
+                         line_group=df_lines_xy['id_geom'],
+                         **kwargs)
+    if color_value is not None:
+        fig = fig\
+            .update_traces(line=dict(color=color_value))
+    if width_value is not None:
+        fig = fig\
+            .update_traces(line=dict(width=width_value))
+    if dash_value is not None:
+        fig = fig\
+            .update_traces(line=dict(dash=dash_value))
+    if legend_name is not None:
+        if 'color' not in kwargs:
+            fig = fig\
+                .update_traces(name=legend_name,
+                               legendgroup=legend_name,
+                               showlegend=True)
+        else:
+            fig = fig\
+                .update_traces(legendgroup=legend_name,
+                               legendgrouptitle_text=legend_name,
+                               showlegend=True)
+    if 'color' not in kwargs:
+        for i in range(len(fig.data)):
+            if i == 0:
+                fig.data[i].showlegend = True
+            else:
+                fig.data[i].showlegend = False
+    if hover_skip:
+        fig = fig\
+            .update_traces(hoverinfo='skip',
+                           hovertemplate=None)
+    return fig
+
+#%%
+def px_sp_polygons(sp_polygons,
+                   color_value = None,
+                   line_color = None,
+                   line_width = None,
+                   line_dash = None,
+                   legend_name = None,
+                   hover_skip = False,
+                   update_crs = True,
+                   **kwargs):
+    if update_crs:
+        if sp_polygons.crs.to_epsg() != Options_epsg.wgs84.value:
+            sp_polygons = sp_polygons.to_crs(Options_epsg.wgs84.value)
+    if color_value is not None:
+        kwargs['color_discrete_sequence'] = [color_value, color_value]
+    fig = px.choropleth_mapbox(sp_polygons,
+                               locations=sp_polygons.index,
+                               geojson=sp_polygons.geometry,
+                               **kwargs)
+    if line_color is not None:
+        fig = fig\
+            .update_traces(marker=dict(line=dict(color=line_color)))
+    if line_width is not None:
+        fig = fig\
+            .update_traces(marker=dict(line=dict(width=line_width)))
+    if line_dash is not None:
+        fig = fig\
+            .update_traces(marker=dict(line=dict(dash=line_dash)))
+    if legend_name is not None:
+        if 'color' not in kwargs:
+            fig = fig\
+                .update_traces(name=legend_name,
+                               legendgroup=legend_name,
+                               showlegend=True)
+        else:
+            fig = fig\
+                .update_traces(legendgroup=legend_name,
+                               legendgrouptitle_text=legend_name,
+                               showlegend=True)
+    if hover_skip:
+        fig = fig\
+            .update_traces(hoverinfo='skip',
+                           hovertemplate=None)
+    return fig
+
+#%%
+def px_sp_polygon_borders(sp_polygons,
+                          line_color = None,
+                          line_width = None,
+                          line_dash = None,
+                          legend_name = None,
+                          hover_skip = True,
+                          update_crs = True,
+                          **kwargs):
+    if update_crs:
+        if sp_polygons.crs.to_epsg() != Options_epsg.wgs84.value:
+            sp_polygons = sp_polygons.to_crs(Options_epsg.wgs84.value)
+    df_polygons_xy = sp_to_df_xy(sp_polygons, cols_keep_all=True)
+    fig = px.line_mapbox(df_polygons_xy,
+                         lon=df_polygons_xy['x'],
+                         lat=df_polygons_xy['y'],
+                         line_group=df_polygons_xy['id_geom'])
+    if line_color is not None:
+        fig = fig\
+            .update_traces(line=dict(color=line_color))
+    if line_width is not None:
+        fig = fig\
+            .update_traces(line=dict(width=line_width))
+    if line_dash is not None:
+        fig = fig\
+            .update_traces(line=dict(dash=line_dash))
+    if legend_name is not None:
+        if 'color' not in kwargs:
+            fig = fig\
+                .update_traces(name=legend_name,
+                               legendgroup=legend_name,
+                               showlegend=True)
+        else:
+            fig = fig\
+                .update_traces(legendgroup=legend_name,
+                               legendgrouptitle_text=legend_name,
+                               showlegend=True)
+    if 'color' not in kwargs:
+        for i in range(len(fig.data)):
+            if i == 0:
+                fig.data[i].showlegend = True
+            else:
+                fig.data[i].showlegend = False
+    if hover_skip:
+        fig = fig\
+            .update_traces(hoverinfo='skip',
+                           hovertemplate=None)
+    return fig
+
+#%%
 # options_epsg = dict(wgs84 = 4326, nad83_LA_north = 3451, nad83_LA_south = 3452)
 # class Options_epsg:
 #     wgs84 = 4326
 #     nad83_LA_north = 3451
 #     nad83_LA_south = 3452
 
 # #%%
```

### Comparing `dsplus-0.5.1/dsplus.egg-info/PKG-INFO` & `dsplus-0.5.2/dsplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.5.1
+Version: 0.5.2
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.5.1/setup.py` & `dsplus-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.5.1/tests/Test_pandas.py` & `dsplus-0.5.2/tests/Test_pandas.py`

 * *Files identical despite different names*

