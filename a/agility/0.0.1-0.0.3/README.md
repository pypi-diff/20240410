# Comparing `tmp/agility-0.0.1.tar.gz` & `tmp/agility-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agility-0.0.1.tar", last modified: Thu Dec  2 15:49:06 2021, max compression
+gzip compressed data, was "agility-0.0.3.tar", last modified: Wed Apr 10 13:24:17 2024, max compression
```

## Comparing `agility-0.0.1.tar` & `agility-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-12-02 15:49:06.415314 agility-0.0.1/
--rw-rw-rw-   0        0        0     1076 2021-11-16 17:32:57.000000 agility-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2469 2021-12-02 15:49:06.399688 agility-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1751 2021-12-02 15:33:27.000000 agility-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2021-12-02 15:49:06.399688 agility-0.0.1/agility/
--rw-rw-rw-   0        0        0       37 2021-11-19 13:35:18.000000 agility-0.0.1/agility/__init__.py
--rw-rw-rw-   0        0        0    26436 2021-12-02 15:10:27.000000 agility-0.0.1/agility/analysis.py
--rw-rw-rw-   0        0        0     1132 2021-12-02 15:35:49.000000 agility-0.0.1/agility/minimiser.py
--rw-rw-rw-   0        0        0     2073 2021-11-19 14:05:09.000000 agility-0.0.1/agility/plotting.py
-drwxrwxrwx   0        0        0        0 2021-12-02 15:49:06.399688 agility-0.0.1/agility.egg-info/
--rw-rw-rw-   0        0        0     2469 2021-12-02 15:49:06.000000 agility-0.0.1/agility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2021-12-02 15:49:06.000000 agility-0.0.1/agility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-02 15:49:06.000000 agility-0.0.1/agility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-02 15:49:06.000000 agility-0.0.1/agility.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2021-12-02 15:49:06.000000 agility-0.0.1/agility.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-12-02 15:49:06.000000 agility-0.0.1/agility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      212 2021-11-22 10:17:19.000000 agility-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-12-02 15:49:06.415314 agility-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1457 2021-12-02 15:10:27.000000 agility-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:17.978419 agility-0.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-10 13:24:10.000000 agility-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-10 13:24:17.978419 agility-0.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2327 2024-04-10 13:24:10.000000 agility-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:17.978419 agility-0.0.3/agility/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-10 13:24:10.000000 agility-0.0.3/agility/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44919 2024-04-10 13:24:10.000000 agility-0.0.3/agility/analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-04-10 13:24:10.000000 agility-0.0.3/agility/minimiser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2325 2024-04-10 13:24:10.000000 agility-0.0.3/agility/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:17.978419 agility-0.0.3/agility.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-10 13:24:17.000000 agility-0.0.3/agility.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-10 13:24:17.000000 agility-0.0.3/agility.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:24:17.000000 agility-0.0.3/agility.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 13:24:17.000000 agility-0.0.3/agility.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 13:24:17.000000 agility-0.0.3/agility.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3046 2024-04-10 13:24:10.000000 agility-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:24:17.978419 agility-0.0.3/setup.cfg
```

### Comparing `agility-0.0.1/LICENSE` & `agility-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agility-0.0.1/agility/analysis.py` & `agility-0.0.3/agility/analysis.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # Copyright (c) Alexander Bonkowski
 # Distributed under the terms of the MIT License
 # author: Alexander Bonkowski
 
 """Analysis functions."""
 
-
+import pathlib
+import random
 import sys
+import warnings
+from typing import TYPE_CHECKING, Any, List, Literal, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
+from typing_extensions import Self
 
 from agility.minimiser import mimimise_lmp
 
+if TYPE_CHECKING:
+    pass
+
+available_backends = Literal["ovito", "pymatgen", "babel", "pyiron", "ase", "lammps"]
+# https://github.com/pyiron/pylammpsmpi
+
 
 class GBStructure:
-    """This is the fundamental class of a grain boundary object."""
+    """Fundamental class of a grain boundary object."""
 
-    def __init__(self, backend, filename, **kwargs):
+    def __init__(
+        self,
+        backend: available_backends,
+        filename: Union[str, pathlib.Path],
+        **kwargs,
+    ) -> None:
         """Initialize."""
         self.backend = backend
         self.filename = filename
-        self.data = None
-
-        if self.backend not in [
-            "ovito",
-            "pymatgen",
-            "babel",
-            "pyiron",
-            # https://github.com/pyiron/pylammpsmpi
-            "ase",
-            "lammps",
-        ]:
-            # Put error here
-            pass
+        self.data: Any = None
 
         if self.backend == "lammps":
             # Determine if a jupyter notebook is used
             # Taken from shorturl.at/aikzP
             try:
-                shell = get_ipython().__class__.__name__
+                shell = get_ipython().__class__.__name__  # type: ignore[name-defined]
                 if shell == "ZMQInteractiveShell":
                     ipy = True  # Jupyter notebook or qtconsole
                 elif shell == "TerminalInteractiveShell":
                     ipy = False  # Terminal running IPython
                 else:
                     ipy = False  # Other type (?)
             except NameError:
@@ -56,19 +59,20 @@
                 from lammps import PyLammps
 
                 self.pylmp = PyLammps()
 
         if filename:
             self.read_file(filename, **kwargs)
 
-    def read_file(self, filename, **kwargs):
+    def read_file(self, filename: Union[str, pathlib.Path], **kwargs) -> None:
         """Read structure from file.
 
         Args:
             filename: File to read.
+
         Returns:
             None
         """
         if self.backend == "ovito":
             from ovito.io import import_file
 
             self.pipeline = import_file(str(filename))
@@ -79,26 +83,26 @@
             self.data.structure = Structure.from_file(filename)
 
         if self.backend == "lammps":
             self._init_lmp(filename=filename, **kwargs)
 
     def _init_lmp(
         self,
-        filename,
+        filename: Union[str, pathlib.Path],
         file_type: str = "data",
         pair_style: str = "none",
         kspace_style: str = "none",
-    ):
+    ) -> None:
         """Initialise lammps backend.
 
         Args:
             filename: File to read.
-            file_type: File type (data, dump, restart)
-            pair_style: lammps pair style
-            kspace_style:
+            file_type (str): File type (data, dump, restart)
+            pair_style (str): lammps pair style
+            kspace_style (str): lammps kspace style
         """
         self.pylmp.units("metal")
         self.pylmp.atom_style("charge")
         self.pylmp.atom_modify("map array")
         self.pylmp.pair_style(f"{pair_style}")
         if kspace_style:
             self.pylmp.kspace_style(f"{kspace_style}")
@@ -107,132 +111,166 @@
         elif file_type == "dump":
             self.pylmp.read_dump(filename)
         elif file_type == "restart":
             self.pylmp.read_restart(filename)
         else:
             print("Please specify the type of lammps file to read.")
 
-    def save_structure(self, filename: str = None, file_type: str = None, **kwargs):
+    def save_structure(self, filename: str, file_type: str, **kwargs) -> None:
         """Save structure to disc.
 
         Args:
             filename:
             file_type:
-
         """
         if self.backend == "ovito":
             from ovito.io import export_file
 
             export_file(self.pipeline, filename, file_type, **kwargs)
 
         if self.backend == "lammps":
             if file_type == "data":
                 self.pylmp.write_data(filename)
             elif file_type == "dump":
                 self.pylmp.write_dump(filename)
             elif file_type == "restart":
                 self.pylmp.write_restart(filename)
 
-    def minimise(self, *args, **kwargs):
-        """Minimise structure.
-
-        Returns:
-        """
+    def minimise(self, *args, **kwargs) -> None:
+        """Minimise structure."""
         if self.backend == "ovito":
             print(f"The {self.backend} backend does not support minimisation.")
             sys.exit(1)
         elif self.backend == "lammps":
             self.pylmp = mimimise_lmp(self.pylmp, *args, **kwargs)
 
-    def delete_particles(self, particle_type):
+    def delete_particles(self, particle_type: set) -> None:
         """Delete a specific type of particles from a structure.
 
         This can be particularly useful if
         there is a mobile type in the structure. Note that for ovito structures you need to make
         sure that type information is included.
+
+        Args:
+            particle_type: Particle type to delete.
+
+        """
+        if self.backend == "ovito":
+            from ovito.modifiers import DeleteSelectedModifier
+
+            self.select_particles_by_type(particle_type)
+            self.pipeline.modifiers.append(DeleteSelectedModifier())
+
+        elif self.backend == "lammps":
+            self.pylmp.group(f"delete type {particle_type}")
+            self.pylmp.delete_atoms("group delete compress no")
+
+        elif self.backend == "pymatgen":
+            self.data.structure.remove_species(particle_type)
+
+        elif self.backend == "babel":
+            pass
+
+    #    def assign_particles_types(self, particle_types: list):
+    #        """Assign
+    #
+    #        """
+    #        if self.backend == "ovito":
+    #            def setup_atom_types(frame, data):
+    #                types = self.data.particles_.particle_types_
+    #                for i, particle_type in enumerate(particle_types):
+    #                    types.type_by_id_(i+1).name = particle_type
+    #            self.pipeline.modifiers.append(setup_atom_types)
+    #            self.set_analysis()
+
+    def select_particles_by_type(self, particle_type: set) -> None:
+        """Select a specific type of particles from a structure.
+
+        Text.
+
         Args:
             particle_type:
         Returns:
         """
         if self.backend == "ovito":
             # from ovito.plugins.StdModPython import (
             #     SelectTypeModifier,
             #     DeleteSelectedModifier,
             # )
-            from ovito.modifiers import DeleteSelectedModifier, SelectTypeModifier
+            from ovito.modifiers import SelectTypeModifier
 
-            def assign_particle_types(frame, data):  # pylint: disable=W0613
+            def assign_particle_types(  # noqa: ANN202
+                frame,  # noqa: ANN001
+                data,  # noqa: ANN001
+            ):  # pylint: disable=W0613
                 atom_types = data.particles_.particle_types_  # pylint: disable=W0612
 
             self.pipeline.modifiers.append(assign_particle_types)
 
             # Select atoms and delete them
             self.pipeline.modifiers.append(
-                SelectTypeModifier(
+                SelectTypeModifier(  # type: ignore[call-arg]
                     operate_on="particles",
                     property="Particle Type",
-                    types={particle_type},
+                    types=particle_type,
                 )
             )
 
-            self.pipeline.modifiers.append(DeleteSelectedModifier())
-        elif self.backend == "lammps":
-            self.pylmp.group(f"delete type {particle_type}")
-            self.pylmp.delete_atoms("group delete compress no")
-
-        elif self.backend == "pymatgen":
-            self.data.structure.remove_species(particle_type)
-
-        elif self.backend == "babel":
-            pass
-
     def select_particles(
         self,
-        list_ids,
-        invert=True,
-        delete=True,
-        expand=False,
-        expand_cutoff=3.2,
-        nearest_neighbors=None,
-        iterations=1,
-    ):
+        list_ids: list,
+        list_ids_type: Literal["Identifier", "Indices"] = "Identifier",
+        invert: bool = True,
+        delete: bool = True,
+        expand_cutoff: Optional[float] = None,
+        expand_nearest_neighbors: Optional[int] = None,
+        iterations: int = 1,
+    ) -> None:
         """Select particles by ID.
 
         Args:
-            nearest_neighbors:
-            delete:
+            list_ids (list): List of IDs to select.
+            list_ids_type (str): "Indices" or "Identifier"
+            expand_nearest_neighbors (int): Number of nearest neighbors. Default 1.
+            invert (bool): Invert selection.
+            delete (bool): Delete selection.
             iterations:
-            expand_cutoff:
-            expand:
-            invert:
-            list_ids:
+            expand_cutoff (float): Expansion cutoff. Default 3.2.
 
         Returns:
             None
         """
         if self.backend == "ovito":
+            if np.where(self.data.particles.selection != 0)[0].size > 0:
+                self._clear_selection()
+                warnings.warn("Selection currently not empty. Clearing selection.", stacklevel=2)
 
-            def modify(frame, data):  # pylint: disable=W0613
+            def modify(frame, data):  # noqa: ANN001,ANN202  # pylint: disable=W0613
                 # Specify the IDs of all atoms that are to remain here
-                ids = data.particles["Particle Identifier"]
+                if list_ids_type == "Identifier":
+                    ids = data.particles["Particle Identifier"]
+                elif list_ids_type == "Indices":
+                    ids = list(np.where(self.data.particles["Structure Type"] != 10000)[0])
+                else:
+                    raise NameError("Only Indices and Identifier are possible as list id types.")
                 l_ids = np.in1d(ids, list_ids, assume_unique=True, invert=False)
-                selection = data.particles_.create_property(
+                selection = data.particles_.create_property(  # pylint: disable=W0612
                     "Selection", data=l_ids
-                )  # pylint: disable=W0612
+                )
 
             self.pipeline.modifiers.append(modify)
 
-            if expand:
+            if expand_nearest_neighbors or expand_cutoff:
                 from ovito.plugins.ParticlesPython import ExpandSelectionModifier
 
-                if nearest_neighbors:
+                if expand_nearest_neighbors:
                     self.pipeline.modifiers.append(
                         ExpandSelectionModifier(
                             mode=ExpandSelectionModifier.ExpansionMode.Nearest,
-                            num_neighbors=nearest_neighbors,
+                            num_neighbors=expand_nearest_neighbors,
                             iterations=iterations,
                         )
                     )
                 else:
                     self.pipeline.modifiers.append(
                         ExpandSelectionModifier(
                             cutoff=expand_cutoff,
@@ -241,84 +279,132 @@
                         )
                     )
             if invert:
                 self._invert_selection()  # for bulk ions
             if delete:
                 self._delete_selection()
 
-    def _invert_selection(self):
-
+    def _invert_selection(self) -> None:
         if self.backend == "ovito":
-            from ovito.plugins.StdModPython import InvertSelectionModifier
+            from ovito.modifiers import InvertSelectionModifier
 
             self.pipeline.modifiers.append(InvertSelectionModifier())
 
         if self.backend == "pymatgen":
             # Todo: Look which ids are in the list and invert by self.structure
             pass
 
-    def _delete_selection(self):
-
+    def _delete_selection(self) -> None:
         if self.backend == "ovito":
-            from ovito.plugins.StdModPython import DeleteSelectedModifier
+            from ovito.modifiers import DeleteSelectedModifier
 
             self.pipeline.modifiers.append(DeleteSelectedModifier())
 
-    def perform_cna(self, mode: str = "IntervalCutoff", cutoff: float = 3.2, compute: bool = True):
+    def _clear_selection(self) -> None:
+        if self.backend == "ovito":
+            from ovito.modifiers import ClearSelectionModifier
+
+            self.pipeline.modifiers.append(ClearSelectionModifier())
+
+    def perform_cna(
+        self,
+        mode: str = "IntervalCutoff",
+        enabled: Sequence[str] = ("fcc", "hpc", "bcc"),
+        cutoff: float = 3.2,
+        color_by_type: bool = True,
+        only_selected: bool = False,
+        compute: bool = True,
+    ) -> None:
         """Perform Common neighbor analysis.
 
         Args:
             mode: Mode of common neighbor analysis. The lammps backend uses "FixedCutoff".
+            enabled: Enabled structures for identifier.
             cutoff: Cutoff for the FixedCutoff mode.
+            color_by_type: Color by structure type.
+            only_selected: Only selected particles.
             compute: Compute results.
+
         Returns:
             None
         """
         if self.backend == "ovito":
-            # TODO: Enable/diable structure types
-            from ovito.plugins.ParticlesPython import CommonNeighborAnalysisModifier
+            # TODO: Enable/disable structure types
+            from ovito.modifiers import CommonNeighborAnalysisModifier as CNA
 
             if mode == "IntervalCutoff":
-                cna_mode = CommonNeighborAnalysisModifier.Mode.IntervalCutoff
+                cna_mode = CNA.Mode.IntervalCutoff
             elif mode == "AdaptiveCutoff":
-                cna_mode = CommonNeighborAnalysisModifier.Mode.AdaptiveCutoff
+                cna_mode = CNA.Mode.AdaptiveCutoff
             elif mode == "FixedCutoff":
-                cna_mode = CommonNeighborAnalysisModifier.Mode.FixedCutoff
+                cna_mode = CNA.Mode.FixedCutoff
             elif mode == "BondBased":
-                cna_mode = CommonNeighborAnalysisModifier.Mode.BondBased
+                cna_mode = CNA.Mode.BondBased
             else:
                 print(f'Selected CNA mode "{mode}" unknown.')
                 sys.exit(1)
-            cna = CommonNeighborAnalysisModifier(mode=cna_mode, cutoff=cutoff)
+
+            cna = CNA(  # type: ignore[call-arg]
+                mode=cna_mode,
+                cutoff=cutoff,
+                color_by_type=color_by_type,
+                only_selected=only_selected,
+            )
+            # Enabled by default: FCC, HCP, BCC
+            if "fcc" not in enabled:
+                cna.structures[
+                    CNA.Type.FCC  # type: ignore[attr-defined]
+                ].enabled = False  # type: ignore[misc]
+            if "hcp" not in enabled:
+                cna.structures[
+                    CNA.Type.HCP  # type: ignore[attr-defined]
+                ].enabled = False  # type: ignore[misc]
+            if "bcc" not in enabled:
+                cna.structures[
+                    CNA.Type.BCC  # type: ignore[attr-defined]
+                ].enabled = False  # type: ignore[misc]
+            if "ico" not in enabled:
+                cna.structures[
+                    CNA.Type.ICO  # type: ignore[attr-defined]
+                ].enabled = False  # type: ignore[misc]
+
             self.pipeline.modifiers.append(cna)
 
         elif self.backend == "lammps":
             # https://docs.lammps.org/compute_cna_atom.html
             n_compute = len([i["style"] for i in self.pylmp.computes if i["style"] == "cna/atom"])
             self.pylmp.compute(f"cna_{n_compute} all cna/atom {cutoff}")
 
         else:
-            raise NotImplementedError(f"The backend {self.backend} doesn't support this function.")
+            raise not_implemented(self.backend)
 
+        if only_selected:
+            warnings.warn(
+                "Evaluating only the selected atoms. Be aware that non-selected atoms may be "
+                "assigned to the wrong category.",
+                stacklevel=2,
+            )
         if compute:
             self.set_analysis()
 
-    def perfom_cnp(self, cutoff: float = 3.20, compute: bool = False):
+    def perform_cnp(self, cutoff: float = 3.20, compute: bool = False) -> None:
         """Perform Common Neighborhood Parameter calculation.
 
+        Please cite https://doi.org/10.1016/j.cpc.2007.05.018
+
         Returns:
             None
         """
         if self.backend == "lammps":
             self.pylmp.compute(f"compute 1 all cnp/atom {cutoff}")
 
         if compute:
             self.set_analysis()
 
-    def perform_voroni_analysis(self, compute: bool = False):
+    def perform_voronoi_analysis(self, compute: bool = False) -> None:
         """Perform Voronoi analysis.
 
         Args:
             ovito:
                 bonds_vis = False
                 edge_threshold = 0.0
                 face_threshold = 0.0
@@ -362,27 +448,27 @@
             self.set_analysis()
 
         # https://tess.readthedocs.io/en/stable/
         # https://github.com/materialsproject/pymatgen/blob/v2022.0.14/pymatgen/analysis/structure_analyzer.py#L61-L174
 
     def perform_ptm(
         self,
-        *args,
-        enabled: list = ["fcc", "hpc", "bcc"],
+        enabled: Sequence[str] = ("fcc", "hpc", "bcc"),
         rmsd_threshold: float = 0.1,
+        only_selected: bool = False,
         compute: bool = True,
         **kwargs,
-    ):
+    ) -> None:
         """Perform Polyhedral template matching.
 
         https://dx.doi.org/10.1088/0965-0393/24/5/055007
         https://github.com/pmla/polyhedral-template-matching.
 
         Args:
-            enabled (list): List of strings for enabled structure types. Possible values:
+            enabled (tuple): List of strings for enabled structure types. Possible values:
                 fcc-hcp-bcc-ico-sc-dcub-dhex-graphene
             for ovito:
                 output_deformation_gradient = False
                 output_interatomic_distance = False
                 output_ordering = False
                 output_orientation = False
                 output_rmsd = False
@@ -396,54 +482,70 @@
         Returns:
             None
         """
         for i in enabled:
             if i not in ["fcc", "hcp", "bcc", "ico", "sc", "dcub", "dhex", "graphene"]:
                 print(f"Enabled structure type {i} unknown")
         if self.backend == "ovito":
+            from ovito.modifiers import PolyhedralTemplateMatchingModifier as PTM
 
-            from ovito.plugins.ParticlesPython import PolyhedralTemplateMatchingModifier
-
-            ptm = PolyhedralTemplateMatchingModifier(*args, rmsd_cutoff=rmsd_threshold, **kwargs)
+            ptm = PTM(  # type: ignore[call-arg]
+                rmsd_cutoff=rmsd_threshold, only_selected=only_selected, **kwargs
+            )
 
             # Enabled by default: FCC, HCP, BCC
             if "fcc" not in enabled:
-                ptm.structures[PolyhedralTemplateMatchingModifier.Type.FCC].enabled = False
+                ptm.structures[
+                    PTM.Type.FCC  # type: ignore[attr-defined]
+                ].enabled = False  # type: ignore[misc]
             if "hcp" not in enabled:
-                ptm.structures[PolyhedralTemplateMatchingModifier.Type.HCP].enabled = False
+                ptm.structures[
+                    PTM.Type.HCP  # type: ignore[attr-defined]
+                ].enabled = False  # type: ignore[misc]
             if "bcc" not in enabled:
-                ptm.structures[PolyhedralTemplateMatchingModifier.Type.BCC].enabled = False
+                ptm.structures[
+                    PTM.Type.BCC  # type: ignore[attr-defined]
+                ].enabled = False  # type: ignore[misc]
             if "ico" in enabled:
-                ptm.structures[PolyhedralTemplateMatchingModifier.Type.ICO].enabled = True
+                ptm.structures[
+                    PTM.Type.ICO  # type: ignore[attr-defined]
+                ].enabled = True  # type: ignore[misc]
             if "sc" in enabled:
-                ptm.structures[PolyhedralTemplateMatchingModifier.Type.SC].enabled = True
+                ptm.structures[
+                    PTM.Type.SC  # type: ignore[attr-defined]
+                ].enabled = True  # type: ignore[misc]
             if "dcub" in enabled:
-                ptm.structures[PolyhedralTemplateMatchingModifier.Type.CUBIC_DIAMOND].enabled = True
+                ptm.structures[
+                    PTM.Type.CUBIC_DIAMOND  # type: ignore[attr-defined]
+                ].enabled = True  # type: ignore[misc]
             if "dhex" in enabled:
-                ptm.structures[PolyhedralTemplateMatchingModifier.Type.HEX_DIAMOND].enabled = True
+                ptm.structures[
+                    PTM.Type.HEX_DIAMOND  # type: ignore[attr-defined]
+                ].enabled = True  # type: ignore[misc]
             if "graphene" in enabled:
-                ptm.structures[PolyhedralTemplateMatchingModifier.Type.GRAPHENE].enabled = True
+                ptm.structures[
+                    PTM.Type.GRAPHENE  # type: ignore[attr-defined]
+                ].enabled = True  # type: ignore[misc]
 
             self.pipeline.modifiers.append(ptm)
 
         elif self.backend == "lammps":
             # https://docs.lammps.org/compute_ptm_atom.html
             n_compute = len([i["style"] for i in self.pylmp.computes if i["style"] == "ptm/atom"])
             enabled_structures = " ".join(enabled)
             self.pylmp.compute(
                 f"ptm_{n_compute} all ptm/atom {enabled_structures} {rmsd_threshold}"
             )
         else:
-            # print error
-            pass
+            raise not_implemented(self.backend)
 
         if compute:
             self.set_analysis()
 
-    def perform_ajm(self, compute: bool = True):
+    def perform_ajm(self, compute: bool = True) -> None:
         """Ackland-Jones analysis.
 
         https://doi.org/10.1103/PhysRevB.73.054104
         Returns:
         """
         if self.backend == "ovito":
             from ovito.plugins.ParticlesPython import AcklandJonesModifier
@@ -462,15 +564,15 @@
 
         else:
             pass
 
         if compute:
             self.set_analysis()
 
-    def perform_csp(self, num_neighbors: int = 12, compute: bool = True):
+    def perform_csp(self, num_neighbors: int = 12, compute: bool = True) -> None:
         """Centrosymmetric parameter.
 
         Use 12 for fcc and 8 for bcc, respectively
         Returns:
         """
         if self.backend == "ovito":
             from ovito.plugins.ParticlesPython import CentroSymmetryModifier
@@ -486,15 +588,15 @@
             self.pylmp.compute(f"centro_{n_compute} all centro/atom {num_neighbors}")
 
         if compute:
             self.set_analysis()
 
     def get_distinct_grains(
         self, *args, algorithm: str = "GraphClusteringAuto", compute: bool = True, **kwargs
-    ):
+    ) -> None:
         """Get distinct grains from the structure.
 
         Args:
             ovito:
                     algorithm = GrainSegmentationModifier.Algorithm.GraphClusteringAuto
                     color_particles = True
                     handle_stacking_faults = True
@@ -511,66 +613,219 @@
             if algorithm == "GraphClusteringAuto":
                 gsm_mode = GrainSegmentationModifier.Algorithm.GraphClusteringAuto
             elif algorithm == "GraphClusteringManual":
                 gsm_mode = GrainSegmentationModifier.Algorithm.GraphClusteringManual
             elif algorithm == "MinimumSpanningTree":
                 gsm_mode = GrainSegmentationModifier.Algorithm.MinimumSpanningTree
             else:
-                print("Incorrenct Grain Segmentation algorithm specified.")
+                print("Incorrect Grain Segmentation algorithm specified.")
                 sys.exit(1)
 
             gsm = GrainSegmentationModifier(*args, algorithm=gsm_mode, **kwargs)
             self.pipeline.modifiers.append(gsm)
             if compute:
-                self.data = self.pipeline.compute()
+                self.set_analysis()
             # TODO: Get misorientation plot
 
-    def set_analysis(self):
+    def set_analysis(self) -> None:
         """Compute results.
 
         Important function for the ovito backend. The lammps backend can access compute results
         without evaluation of this function.
+
         Returns:
             None
         """
         if self.backend == "ovito":
             self.data = self.pipeline.compute()
 
         elif self.backend == "lammps":
             self.pylmp.run(1)
 
         elif self.backend == "pymatgen":
             print("The pymatgen backend does not require setting the analysis.")
 
-    def get_gb_atoms(self, mode: str = "cna"):
+    def expand_to_non_selected(
+        self,
+        nearest_n: Optional[int] = None,
+        cutoff: Optional[float] = None,
+        expansion_base: Optional[list] = None,
+        return_type: str = "Identifier",
+        return_random: bool = False,
+        invert: bool = False,
+    ) -> List[int]:
+        """Useful method if only_selected was chosen for structural analysis.
+
+        Args:
+            nearest_n: Number of nearest neighbors to consider.
+            cutoff: Cutoff distance to consider.
+            expansion_base: List of atoms to expand from. Must be Indices.
+            return_type: Either Identifier or Indices.
+            return_random: If True, return a random selection of the non-selected atoms.
+            invert: If True, invert the selection.
+
+        Returns:
+        gb_non_selected: list of GB atoms that were not in the previously selected group.
+        """
+        if nearest_n and cutoff:
+            raise ValueError("Only one of nearest_n and cutoff can be specified.")
+        if self.backend == "ovito":
+            if return_type not in ["Identifier", "Indices"]:
+                raise NameError("Only Indices and Identifier are possible as return types.")
+
+            self._invert_selection()
+            self.set_analysis()
+
+            finder = get_finder(self.data, cutoff=cutoff, nearest_n=nearest_n)
+            if nearest_n:
+                from ovito.data import NearestNeighborFinder
+
+            gb_non_selected = []
+            # edge = []
+            # Obtain a set of bulk (=crystalline) cations
+            bulk_atoms = expansion_base or self.get_crystalline_atoms(return_type="Indices")
+            bulk_atoms_set = set(bulk_atoms)
+            # These are the atoms that haven't been analysed in the structure analysis, i.e. anions
+            non_selected = set(np.where(self.data.particles.selection == 1)[0])
+
+            for index in non_selected:
+                neighbors = {neigh.index for neigh in finder.find(index)}
+                # The following is the neighbors w/o the atoms excluded from structural analysis
+                neighbors_no_selected = neighbors - non_selected
+                # If NN, correct for non-selected atoms
+                if nearest_n:
+                    nearest_n_added = nearest_n
+                    while len(neighbors_no_selected) < nearest_n:
+                        finder = NearestNeighborFinder(nearest_n_added, self.data)
+                        neighbors = {neigh.index for neigh in finder.find(index)}
+                        neighbors_no_selected = neighbors - non_selected
+                        nearest_n_added += 1
+                if len(neighbors_no_selected) == 0:
+                    raise ValueError("Cutoff radius too small.")
+                if len(neighbors_no_selected) <= 2:
+                    warnings.warn(
+                        "At least one atoms has only two other atoms to assign. "
+                        "Consider increasing the cutoff value.",
+                        stacklevel=2,
+                    )
+                bulk_neighbors = bulk_atoms_set.intersection(neighbors_no_selected)
+                bulk_fraction = len(bulk_neighbors) / len(neighbors_no_selected)
+                if bulk_fraction < 0.5:
+                    gb_non_selected.append(index)
+                if return_random and bulk_fraction == 0.5 and random.random() < 0.5:
+                    gb_non_selected.append(index)
+
+            self._invert_selection()
+
+            if invert:
+                gb_non_selected = list(set(non_selected) - set(gb_non_selected))
+            if return_type == "Identifier":
+                gb_non_selected = [
+                    self.data.particles["Particle Identifier"][i] for i in gb_non_selected
+                ]
+        else:
+            raise not_implemented(self.backend)
+
+        return gb_non_selected
+
+    def expand_to_non_selected_groups(
+        self,
+        groups: list,
+        cutoff: float = 4.5,
+        return_type: str = "Identifier",
+        return_random: bool = False,
+    ) -> list:
+        """Useful method if only_selected was chosen for structural analysis.
+
+        Args:
+            groups: list of lists containing the groups (as indices).
+            cutoff (float): Cutoff (in Angstrom) for the neighbour finder.
+            return_type (str): return either identifiers or indices.
+            return_random (bool): Some particles will have the same (maximum) neighbours in
+                multiple groups. If true, returns a random group from that pool.
+
+        Returns:
+        groups_non_selected (list): atoms that were not in the previously selected group.
+        """
+        if self.backend == "ovito":
+            if return_type not in ["Identifier", "Indices"]:
+                raise NameError("Only Indices and Identifier are possible as return types.")
+
+            self._invert_selection()
+            self.set_analysis()
+
+            finder = get_finder(self.data, cutoff=cutoff)
+
+            groups_non_selected = [[] for _ in range(len(groups))]  # type: list[list]
+            # Obtain sets of bulk (=crystalline) cations
+            group_sets = [set(i) for i in groups]
+            # These are the atoms that haven't been analysed in the structure analysis, most likely
+            # anions
+            non_selected = set(np.where(self.data.particles.selection == 1)[0])
+
+            for index in non_selected:
+                neighbors = {neigh.index for neigh in finder.find(index)}
+                # The following is the neighbors w/o the atoms excluded from structural analysis
+                neighbors_no_selected = neighbors - non_selected
+                if len(neighbors_no_selected) < 3:
+                    warnings.warn(
+                        "At least one atoms has only two other atoms to assign.", stacklevel=2
+                    )
+                group_neighbors = [len(i.intersection(neighbors_no_selected)) for i in group_sets]
+                indices_max = np.where(group_neighbors == np.amax(group_neighbors))[0]
+                if len(indices_max) > 1 and return_random:
+                    groups_non_selected[random.choice(indices_max)].append(index)
+                else:
+                    group_maximum_interception = np.argmax(group_neighbors)
+                    groups_non_selected[group_maximum_interception].append(index)
+
+            self._invert_selection()
+
+            if return_type == "Identifier":
+                groups_non_selected = [
+                    self.data.particles["Particle Identifier"][i] for i in groups_non_selected
+                ]
+
+        else:
+            raise not_implemented(self.backend)
+
+        return groups_non_selected
+
+    # TODO: Rename to particles
+    def get_non_crystalline_atoms(self, mode: str = "cna", return_type: str = "Identifier") -> list:
         """Get the atoms at the grain boundary.
 
-        For this to work, some sort of stuctural analysis has to be performed.
+        For this to work, some sort of structural analysis has to be performed.
 
         Args:
             mode: Mode for selection of grain boundary atoms.
+            return_type:
         Returns:
-            None
+            List of non-crystalline particles.
         """
         if self.backend == "ovito":
             if "Structure Type" in self.data.particles.keys():
-                df_temp = pd.DataFrame(
-                    list(
-                        zip(
+                if return_type == "Identifier":
+                    gb_list = [
+                        i[0]
+                        for i in zip(
                             self.data.particles["Particle Identifier"],
                             self.data.particles["Structure Type"],
                         )
-                    ),
-                    columns=["Particle Identifier", "Structure Type"],
-                )
-                df_gb = df_temp[df_temp["Structure Type"] == 0]
-                return list(df_gb["Particle Identifier"])
+                        if i[1] == 0
+                    ]
+                elif return_type == "Indices":
+                    gb_list = list(np.where(self.data.particles["Structure Type"] == 0)[0])
+                else:
+                    raise NameError("Only Indices and Identifier are possible as return types.")
+            elif "Centrosymmetry" in self.data.particles.keys():
+                print("Implementation in progress.")
+                gb_list = []
             else:
-                print("No Structure analysis performed.")
-                sys.exit(1)
+                raise not_implemented(self.backend)
         elif self.backend == "lammps":
             # Supported analysis methods: cna, ptm,
             from lammps import LMP_STYLE_ATOM, LMP_TYPE_VECTOR
 
             # ids = []
             # for i in range(len(self.pylmp.atoms)):
             #     ids.append(self.pylmp.atoms[i].id)
@@ -587,155 +842,316 @@
                     )
                 ),
                 columns=["Particle Identifier", "Structure Type"],
             )
             # TDOD: This is only cna, what about others?
             if mode == "cna":
                 df_gb = df_temp[df_temp["Structure Type"] == 5]
-            elif mode == "ptm" or mode == "ackland":
+            elif mode in ("ptm", "ackland"):
                 df_gb = df_temp[df_temp["Structure Type"] == 0]
-            elif mode == "voronoi" or mode == "centro":
-                print("Method not implemented.")
+            elif mode in ("voronoi", "centro"):
+                raise NotImplementedError(f"Mode {mode} currently not implemented")
+            else:
+                print(f"Incorrect mode {mode} specified")
                 sys.exit(1)
-            return list(df_gb["Particle Identifier"])
+            gb_list = list(df_gb["Particle Identifier"])
         else:
-            print("Method not implemented.")
-            return None
+            raise not_implemented(self.backend)
+        return gb_list
 
-    def get_bulk_atoms(self):
+    # TODO: Rename to particles
+    def get_crystalline_atoms(self, return_type: str = "Identifier") -> list:
         """Get the atoms in the bulk, as determined by structural analysis.
 
         Returns:
-            None
+            List of crystalline particles.
         """
         if self.backend == "ovito":
             if "Structure Type" in self.data.particles.keys():
-                df_temp = pd.DataFrame(
-                    list(
-                        zip(
+                if return_type == "Identifier":
+                    gb_list = [
+                        i[0]
+                        for i in zip(
                             self.data.particles["Particle Identifier"],
                             self.data.particles["Structure Type"],
                         )
-                    ),
-                    columns=["Particle Identifier", "Structure Type"],
+                        if i[1] != 0
+                    ]
+                elif return_type == "Indices":
+                    gb_list = list(np.where(self.data.particles["Structure Type"] != 0)[0])
+                else:
+                    raise NotImplementedError(
+                        "Indices and Identifier are possible as return types."
+                    )
+                # df_temp = pd.DataFrame(
+                #     list(
+                #         zip(
+                #             self.data.particles["Particle Identifier"],
+                #             self.data.particles["Structure Type"],
+                #         )
+                #     ),
+                #     columns=["Particle Identifier", "Structure Type"],
+                # )
+                # df_gb = df_temp[df_temp["Structure Type"] != 0]
+                # return list(df_gb["Particle Identifier"])
+            else:
+                warnings.warn(
+                    "No structure type information found. Returning empty list.", stacklevel=2
                 )
-                df_gb = df_temp[df_temp["Structure Type"] != 0]
-                return list(df_gb["Particle Identifier"])
+                gb_list = []
+        elif self.backend == "lammps":
+            # TODO
+            raise not_implemented(self.backend)
+        else:
+            raise not_implemented(self.backend)
+        return gb_list
+
+    # TODO: Rename to particles
+    def get_grain_edge_ions(
+        self,
+        nearest_n: int = 12,
+        cutoff: Optional[float] = None,
+        gb_ions: Optional[set] = None,
+        bulk_ions: Optional[list] = None,
+        return_type: str = "Identifier",
+    ) -> list:
+        """Get the atoms at the grain edge, as determined by structural analysis.
+
+        Returns a list of IDs, which were identified as crystalline/bulk atoms, but border at
+        least one non-crystalline/grain boundary atom.
+
+        Args:
+            nearest_n (int): Number of nearest neighbors to consider. Examples: fcc=12, bcc=8
+            cutoff (float):
+            gb_ions (set): Indices of grain boundary ions. Default: non-crystalline ions.
+            bulk_ions (list): Indices of bulk ions. Default: crystalline ions.
+            return_type (str):
+
+        """
+        if self.backend == "ovito":
+            # finder: CutoffNeighborFinder | NearestNeighborFinder
+            from typing import Union
+
+            from ovito.data import CutoffNeighborFinder, NearestNeighborFinder
+
+            finder: Union[CutoffNeighborFinder, NearestNeighborFinder]
+            if cutoff:
+                finder = CutoffNeighborFinder(cutoff, self.data)
+            else:
+                finder = NearestNeighborFinder(nearest_n, self.data)
+            # ptypes = self.data.particles.particle_types
+
+            gb_edge_ions = []
+            gb_ions_set = gb_ions or self.get_non_crystalline_atoms(return_type="Indices")
+            bulk_ions_list = bulk_ions or self.get_crystalline_atoms(return_type="Indices")
+            gb_ions_set = set(gb_ions_set)
+            for index in bulk_ions_list:
+                # print("Nearest neighbors of particle %i:" % index)
+                # for neigh in finder.find(index):
+                #    print(neigh.index, neigh.distance, neigh.delta)
+                #    # The index can be used to access properties of the current neighbor, e.g.
+                #    type_of_neighbor = ptypes[neigh.index]
+                neighbors = [neigh.index for neigh in finder.find(index)]
+                if any(x in gb_ions_set for x in neighbors):
+                    gb_edge_ions.append(index)
+            if return_type == "Identifier":
+                gb_edge_ions = [self.data.particles["Particle Identifier"][i] for i in gb_edge_ions]
         elif self.backend == "lammps":
             # TODO
-            return None
+            raise not_implemented(self.backend)
         else:
-            print("Method not implemented.")
-            return None
+            raise not_implemented(self.backend)
+        return gb_edge_ions
+
+    def set_gb_type(self) -> None:
+        """Set a property for grain boundary/bulk/grain edge atoms."""
+
+    def get_gb_fraction(self, mode: str = "cna") -> float:
+        """Get fraction of grain boundary ions.
+
+        Args:
+            mode:
 
-    def get_type(self, atom_type):
+        Returns:
+            fraction (float): Fraction of grain boundary ions.
+        """
+        if self.backend == "ovito":
+            fraction = len(self.get_non_crystalline_atoms(mode)) / len(
+                self.data.particles["Particle Identifier"]
+            )
+            warnings.warn(
+                "Using all particles with a particle identifier as the base.", stacklevel=2
+            )
+        elif self.backend == "lammps":
+            # TODO
+            raise not_implemented(self.backend)
+        else:
+            raise not_implemented(self.backend)
+        return fraction
+
+    # TODO: Rename to particles
+    def get_type(self, atom_type: int, return_type: str = "Identifier") -> list:
         """Get all atoms by type.
 
         Args:
             atom_type:
+            return_type (str):
 
         Returns:
-            None
+            List of particles of the specified type.
         """
         if self.backend == "ovito":
             # Currently doesn't work!
             # def assign_particle_types(frame, data):
             #     atom_types = data.particles_.particle_types_
             #
             # self.pipeline.modifiers.append(assign_particle_types)
             # self.set_analysis()
-            df_temp = pd.DataFrame(
-                list(
-                    zip(
+            if return_type == "Identifier":
+                atom_list = [
+                    i[0]
+                    for i in zip(
                         self.data.particles["Particle Identifier"],
                         self.data.particles["Particle Type"],
                     )
-                ),
-                columns=["Particle Identifier", "Particle Type"],
-            )
-            df_atom = df_temp[df_temp["Particle Type"].eq(atom_type)]
-            return list(df_atom["Particle Identifier"])
+                    if i[1] == atom_type
+                ]
+            elif return_type == "Indices":
+                atom_list = list(np.where(self.data.particles["Particle Type"] == atom_type)[0])
+            else:
+                raise NameError("Only Indices and Identifier are possible as return types.")
+            # df_temp = pd.DataFrame(
+            #     list(
+            #         zip(
+            #             self.data.particles["Particle Identifier"],
+            #             self.data.particles["Particle Type"],
+            #         )
+            #     ),
+            #     columns=["Particle Identifier", "Particle Type"],
+            # )
+            # df_atom = df_temp[df_temp["Particle Type"].eq(atom_type)]
+            # return list(df_atom["Particle Identifier"])
 
         elif self.backend == "lammps":
             # TODO
-            return None
+            atom_list = []
         else:
-            print("Method not implemented.")
-            return None
+            raise not_implemented(self.backend)
+        return atom_list
 
     # Todo: Verkippungswinkel
     # Todo: Grain Index
 
-    def get_fraction(self, numerator, denominator):
+    def get_fraction(self, numerator: list, denominator: list) -> float:
         """Get fraction of ions/atoms. Helper function.
 
         Args:
-            numerator:
-            denominator:
+            numerator: Particle type(s) in the numerator.
+            denominator: Particle type(s) in the denominator.
 
         Returns:
             None
         """
         if self.backend == "ovito":
             num = sum([len(self.get_type(i)) for i in numerator])
             den = sum([len(self.get_type(i)) for i in denominator])
-            return num / den
-
         else:
-            print("Method not implemented.")
-            return None
+            raise not_implemented(self.backend)
 
-    def save_image(self, filename: str = "image.png"):
+        return num / den
+
+    def save_image(self, filename: str = "image.png") -> None:
         """Save image file.
 
         Args:
             filename: file to be saved.
-
         """
         if self.backend == "ovito":
             # TODO: use render function
             pass
         if self.backend == "lammps":
             # Only works with IPython integration
             self.pylmp.image(filename=filename)
 
-    def convert_backend(self, convert_to: str = None):
+    def convert_backend(self, convert_to: available_backends) -> Self:
         """Convert the current backend.
 
         Args:
             convert_to: Backend to convert to.
         """
         if self.backend == "lammps":
             from datetime import datetime
 
             filename = datetime.now().strftime("%d%m%Y_%H%M%S") + ".lmp"
             self.save_structure("filename", file_type="data")
             if convert_to == "ovito":
-                import pathlib
-                from ovito.io import import_file
-
-                self.backend == convert_to
-                self.pipeline = import_file(str(filename))
-                del self.pylmp
-                tempfile = pathlib.Path(filename)
-                tempfile.unlink()
+                try:
+                    return GBStructure(backend=convert_to, filename=filename)  # type: ignore[return-value]
+                finally:
+                    tempfile = pathlib.Path(filename)
+                    tempfile.unlink()
+            else:
+                raise not_implemented(convert_to)
+        else:
+            raise not_implemented(self.backend)
 
 
 class GBStructureTimeseries(GBStructure):
     """This is a class containing multiple snapshots from a time series."""
 
+    # Todo: enable inheritance
     # Todo: get diffusion data
     # Todo: differentiate between along/across GB
 
-    def remove_timesteps(self, timesteps_to_exclude):
-        """Remove timesteps from the beggining of a simulation.
+    def remove_timesteps(self, timesteps_to_exclude: int) -> None:
+        """Remove timesteps from the beginning of a simulation.
 
         Args:
-            timesteps_to_exclude (:py:class:`int`): Number of timesteps to exclude
+            timesteps_to_exclude (int): Number of timesteps to exclude
+
         Returns:
             new_trajectory (:py:class:`polypy.read.Trajectory`):
             Trajectory object.
         """
-        pass
 
     # Todo: Add differentiation between diffusion along a grain boundary, transverse to the GB,
     # and between grains
+
+
+def get_finder(data, cutoff: Optional[float] = None, nearest_n: Optional[int] = None):  # noqa: ANN001,ANN201
+    """Get neighbor finder.
+
+    Args:
+        data: Data object.
+        cutoff: Cutoff distance.
+        nearest_n: Number of nearest neighbors.
+
+    Returns:
+        finder: Neighbor finder.
+
+    """
+    from ovito.data import CutoffNeighborFinder, NearestNeighborFinder
+
+    finder: Union[CutoffNeighborFinder, NearestNeighborFinder]
+
+    if cutoff:
+        finder = CutoffNeighborFinder(cutoff, data)
+    elif nearest_n:
+        finder = NearestNeighborFinder(nearest_n, data)
+    elif cutoff and nearest_n:
+        raise NameError("Only cutoff or nearest_n can be specified.")
+    else:
+        raise NameError("Either cutoff or nearest_n must be specified.")
+    return finder
+
+
+def not_implemented(backend: available_backends) -> NotImplementedError:
+    """Raise not implemented error.
+
+    Args:
+        backend: Backend currently in use.
+
+    Returns:
+        NotImplementedError
+
+    """
+    return NotImplementedError(f"The backend {backend} doesn't support this function.")
```

### Comparing `agility-0.0.1/agility/plotting.py` & `agility-0.0.3/agility/plotting.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-"""
-Plotting and rendering funtions.
-"""
+"""Plotting and rendering functions."""
 
 # Copyright (c) Alexander Bonkowski
 # Distributed under the terms of the MIT License
 # author: Alexander Bonkowski
 
+from typing import TYPE_CHECKING
+
 import pandas as pd
 import seaborn as sns
 
+if TYPE_CHECKING:
+    from ovito.data import DataCollection
+    from ovito.pipeline import Pipeline
+    from PySide6.QtGui import QImage
+
+
+def render_ovito(pipeline: Pipeline, res_factor: int = 1) -> QImage:
+    """Render an ovito pipeline object.
 
-def render_ovito(pipeline=None, res_factor: int = 1):
-    """
-    Render an ovito pipeline object.
     Args:
         pipeline: The ovito pipeline to be rendered.
-        res_factor: Factor to scale the resolution of the redering. 2=Full HD, 4=4K
+        res_factor: Factor to scale the resolution of the rendering. 2=Full HD, 4=4K.
 
     Returns:
+    -------
         image: Image object. Can be saved via image.save("figure.png")
 
     """
-    from ovito.plugins.PyScript import Viewport
-    from ovito.plugins.TachyonPython import TachyonRenderer
+    from ovito.vis import TachyonRenderer, Viewport
 
     pipeline.add_to_scene()
-    viewport = Viewport(type=Viewport.Type.Ortho)
-    viewport.type = Viewport.Type.Perspective
-    viewport.camera_dir = (-1, 2, -1)
+
+    viewport = Viewport()
+    viewport.type = Viewport.Type.Perspective  # type: ignore[misc]
+    viewport.camera_dir = (-1, 2, -1)  # type: ignore[misc]
     viewport.zoom_all(size=(640, 480))
 
-    tachyon = TachyonRenderer(shadows=False, direct_light_intensity=1.1)
-    image = viewport.render_image(
+    tachyon = TachyonRenderer(shadows=False, direct_light_intensity=1.1)  # type: ignore[call-arg]
+    return viewport.render_image(
         size=(res_factor * 640, res_factor * 480),
         # filename="figure.png",
         background=(1, 1, 1),
         alpha=True,
         renderer=tachyon,
         crop=True,
     )
 
-    return image
 
+def plot_face_order(data: DataCollection, plot_property: str = "Max Face Order") -> sns.FacetGrid:
+    """Plot the histogram of max. face order from ovito data.
 
-def plot_face_order(data=None, plot_property="Max Face Order"):
-    """
-    Plot the histogram of max. face order from ovito data.
     Args:
         data:
+        plot_property:
 
     Returns:
+        Histogram plot.
 
     """
     df_temp = pd.DataFrame(
         list(
             zip(
                 data.particles["Particle Identifier"],
                 data.particles[plot_property],
```

