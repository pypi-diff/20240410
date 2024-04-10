# Comparing `tmp/electrode_visualizer-1.0.0.tar.gz` & `tmp/electrode_visualizer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrode_visualizer-1.0.0.tar", max compression
+gzip compressed data, was "electrode_visualizer-1.0.1.tar", max compression
```

## Comparing `electrode_visualizer-1.0.0.tar` & `electrode_visualizer-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-04-02 14:24:00.426502 electrode_visualizer-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-02 14:23:35.676501 electrode_visualizer-1.0.0/README.md
--rw-r--r--   0        0        0    19709 2024-04-02 14:24:43.096501 electrode_visualizer-1.0.0/electrode_visualizer/Application.py
--rw-r--r--   0        0        0     7704 2024-04-02 14:33:58.606497 electrode_visualizer-1.0.0/electrode_visualizer/Parser.py
--rw-r--r--   0        0        0        0 2024-04-02 14:24:43.096501 electrode_visualizer-1.0.0/electrode_visualizer/__init__.py
--rw-r--r--   0        0        0      125 2024-04-02 14:24:43.096501 electrode_visualizer-1.0.0/electrode_visualizer/__main__.py
--rw-r--r--   0        0        0      336 2024-04-02 22:26:46.356499 electrode_visualizer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 electrode_visualizer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-04-10 15:19:49.357010 electrode_visualizer-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4464 2024-04-10 15:19:49.357010 electrode_visualizer-1.0.1/README.md
+-rw-r--r--   0        0        0    19767 2024-04-10 15:19:49.357010 electrode_visualizer-1.0.1/electrode_visualizer/Application.py
+-rw-r--r--   0        0        0     7704 2024-04-10 15:19:49.357010 electrode_visualizer-1.0.1/electrode_visualizer/Parser.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:19:49.357010 electrode_visualizer-1.0.1/electrode_visualizer/__init__.py
+-rw-r--r--   0        0        0      125 2024-04-10 15:19:49.357010 electrode_visualizer-1.0.1/electrode_visualizer/__main__.py
+-rw-r--r--   0        0        0      505 2024-04-10 15:53:42.227007 electrode_visualizer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5232 1970-01-01 00:00:00.000000 electrode_visualizer-1.0.1/PKG-INFO
```

### Comparing `electrode_visualizer-1.0.0/LICENSE` & `electrode_visualizer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `electrode_visualizer-1.0.0/electrode_visualizer/Application.py` & `electrode_visualizer-1.0.1/electrode_visualizer/Application.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,26 +327,26 @@
       A partir de los datos leídos se crea una vista agradable para el usuario
     """
     self.end_time = self.max_time
     with dpg.child_window(parent="graphs", height=-110):
       # Se separan los datos por su locación/electrodo
       for location, frequencies in self.data.hierarchy.items():
         with dpg.tree_node(label=location, default_open=True):
-          with dpg.plot(width=-1,no_menus=True, tag=location):
-            
+          with dpg.plot(width=-1, no_menus=True, anti_aliased=True, tag=location):
+            dpg.add_plot_legend()
             # Añadir tag del eje para actualizarlo al hacer zoom o desplazar el zoom
             self.time_axis.append(dpg.add_plot_axis(dpg.mvXAxis, label="segundos"))
             with dpg.plot_axis(dpg.mvYAxis, label="value"):
               # Marca la parte mas alta de los datos para el electrodo
               ceiling: float = self.data.data[f"{location} {frequencies[0]}"].max()
               # Marca la parte mas baja de los datos para el electrodo
               ground: float = self.data.data[f"{location} {frequencies[0]}"].min()
               for frequency in frequencies:
                 # Añadir datos para cada frecuencia
-                dpg.add_line_series(self.data.data.index.to_list(), self.data.data[f"{location} {frequency}"].to_list())
+                dpg.add_line_series(self.data.data.index.to_list(), self.data.data[f"{location} {frequency}"].to_list(), label=frequency)
                 if self.data.data[f"{location} {frequency}"].max() > ceiling:
                   ceiling: float = self.data.data[f"{location} {frequency}"].max()
                 if self.data.data[f"{location} {frequency}"].min() < ground:
                   ground: float = self.data.data[f"{location} {frequency}"].min()
               # Marcar puntos donde se supero el umbral
               for start, end in self.data.aceptable:
                 dpg.add_area_series([start,start,end,end], [ground,ceiling,ceiling,ground], fill=[0,255,0,100] if self.data.parsed["reached"] else [255,0,0,100])
```

### Comparing `electrode_visualizer-1.0.0/electrode_visualizer/Parser.py` & `electrode_visualizer-1.0.1/electrode_visualizer/Parser.py`

 * *Files identical despite different names*

