# Comparing `tmp/gplugins-0.9.8.tar.gz` & `tmp/gplugins-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gplugins-0.9.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gplugins-0.9.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gplugins-0.9.8.tar` & `gplugins-0.9.9.tar`

### file list

```diff
@@ -1,227 +1,228 @@
--rw-r--r--   0        0        0     1077 2023-12-11 16:57:12.109730 gplugins-0.9.8/LICENSE
--rw-r--r--   0        0        0     2993 2023-12-11 16:57:12.109730 gplugins-0.9.8/README.md
--rw-r--r--   0        0        0      258 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/__init__.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/__init__.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/base_models/__init__.py
--rw-r--r--   0        0        0     7201 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/base_models/component.py
--rw-r--r--   0        0        0     2126 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/base_models/simulation.py
--rw-r--r--   0        0        0      716 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/config.py
--rw-r--r--   0        0        0      571 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/types.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/__init__.py
--rw-r--r--   0        0        0     4275 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/add_simulation_markers.py
--rw-r--r--   0        0        0     4487 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/async_helpers.py
--rw-r--r--   0        0        0     1216 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/cache.py
--rw-r--r--   0        0        0     3276 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/convert_sparameters.py
--rw-r--r--   0        0        0      251 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/disable_print.py
--rw-r--r--   0        0        0     2857 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/get_capacitance.py
--rw-r--r--   0        0        0     3921 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/get_component_with_net_layers.py
--rw-r--r--   0        0        0     3407 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/get_effective_indices.py
--rw-r--r--   0        0        0     2821 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/get_scattering.py
--rw-r--r--   0        0        0     2946 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/get_sparameters_path.py
--rw-r--r--   0        0        0     1484 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/optical_constants.py
--rw-r--r--   0        0        0     3880 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/parse_layer_stack.py
--rw-r--r--   0        0        0     6046 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/plot.py
--rw-r--r--   0        0        0     2439 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/plot_csv.py
--rw-r--r--   0        0        0      613 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/port_symmetries.py
--rw-r--r--   0        0        0     1573 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/common/utils/tests/test_get_component_with_new_port_layers.py
--rw-r--r--   0        0        0       28 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/dagster/Makefile
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/dagster/__init__.py
--rw-r--r--   0        0        0      933 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/dagster/workflow.py
--rw-r--r--   0        0        0      571 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/devsim/__init__.py
--rw-r--r--   0        0        0     2504 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/devsim/doping.py
--rw-r--r--   0        0        0    11856 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/devsim/get_simulation.py
--rw-r--r--   0        0        0    28231 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19702 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/devsim/get_solver.py
--rw-r--r--   0        0        0     1530 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/devsim/test_devsim.py
--rw-r--r--   0        0        0      129 2023-12-11 16:57:12.113730 gplugins-0.9.8/gplugins/elmer/__init__.py
--rw-r--r--   0        0        0     4701 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/elmer/electrostatic.sif.j2
--rw-r--r--   0        0        0    10177 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/elmer/get_capacitance.py
--rw-r--r--   0        0        0     4070 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/elmer/tests/test_elmer.py
--rw-r--r--   0        0        0      664 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/fdtdz/__init__.py
--rw-r--r--   0        0        0     8549 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/fdtdz/get_epsilon_fdtdz.py
--rw-r--r--   0        0        0     7146 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/fdtdz/get_ports_fdtdz.py
--rw-r--r--   0        0        0     5473 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/fdtdz/get_sparameters_fdtdz.py
--rw-r--r--   0        0        0      196 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/femwell/__init__.py
--rw-r--r--   0        0        0     8465 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/femwell/mode_solver.py
--rw-r--r--   0        0        0     3168 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/femwell/solve_thermal.py
--rw-r--r--   0        0        0     1353 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/femwell/test_mode_solver.py
--rw-r--r--   0        0        0     1926 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/__init__.py
--rw-r--r--   0        0        0     3853 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/get_material.py
--rw-r--r--   0        0        0     6308 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6028 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    11392 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15878 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    18123 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12263 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11862 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0     2000 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6146 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    13921 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    23177 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8095 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9551 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0      850 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/__init__.py
--rw-r--r--   0        0        0     1360 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/define_polysurfaces.py
--rw-r--r--   0        0        0     5481 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/get_mesh.py
--rw-r--r--   0        0        0     7758 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/parse_component.py
--rw-r--r--   0        0        0     3844 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/parse_gds.py
--rw-r--r--   0        0        0    10756 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     2686 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/tests/test_custom_names.py
--rw-r--r--   0        0        0     1952 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/tests/test_meshing_2D.py
--rw-r--r--   0        0        0     1612 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/tests/test_meshing_3D.py
--rw-r--r--   0        0        0    17653 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     9533 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0    14087 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/klayout/__init__.py
--rw-r--r--   0        0        0      312 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/klayout/dataprep/__init__.py
--rw-r--r--   0        0        0     6898 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/klayout/dataprep/regions.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.117730 gplugins-0.9.8/gplugins/klayout/drc/__init__.py
--rw-r--r--   0        0        0      532 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/drc/check_duplicated_cells.py
--rw-r--r--   0        0        0     2684 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/drc/check_exclusion.py
--rw-r--r--   0        0        0     2794 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/drc/check_inclusion.py
--rw-r--r--   0        0        0     3550 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/drc/check_space.py
--rw-r--r--   0        0        0     1813 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/drc/check_width.py
--rw-r--r--   0        0        0     3580 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/drc/write_connectivity.py
--rw-r--r--   0        0        0    14201 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/drc/write_drc.py
--rw-r--r--   0        0        0     3879 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/get_netlist.py
--rw-r--r--   0        0        0      566 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/netlist_spice_reader.py
--rw-r--r--   0        0        0     6782 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/plot_nets.py
--rw-r--r--   0        0        0     2546 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/tests/test_dataprep_regions.py
--rw-r--r--   0        0        0      951 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/tests/test_drc_exclusion.py
--rw-r--r--   0        0        0     1149 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/tests/test_drc_inclusion.py
--rw-r--r--   0        0        0      619 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/tests/test_drc_space.py
--rw-r--r--   0        0        0     1281 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/tests/test_drc_width.py
--rw-r--r--   0        0        0     2495 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/tests/test_geometry_write_connectivity.py
--rw-r--r--   0        0        0      725 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/tests/test_netlist_spice_reader.py
--rw-r--r--   0        0        0     1952 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/klayout/tests/test_plot_nets.py
--rw-r--r--   0        0        0      536 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/lumerical/__init__.py
--rw-r--r--   0        0        0    16025 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/lumerical/interconnect.py
--rw-r--r--   0        0        0     4236 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/lumerical/settings.py
--rw-r--r--   0        0        0     2360 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/lumerical/tests/test_lumerical_read_sparameters.py
--rw-r--r--   0        0        0    19828 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     2534 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/materials/__init__.py
--rw-r--r--   0        0        0     1776 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/materials/inorganic.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/materials/optical/__init__.py
--rw-r--r--   0        0        0     1847 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/materials/optical/optical_mat.py
--rw-r--r--   0        0        0    23894 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/materials/optical/refractive_index_info.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/materials/semiconductor/__init__.py
--rw-r--r--   0        0        0      273 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/materials/semiconductor/semiconductor_mat.py
--rw-r--r--   0        0        0       67 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/meow/__init__.py
--rw-r--r--   0        0        0    16624 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/meow/meow_eme.py
--rw-r--r--   0        0        0     2269 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/meow/test_meow_simulation.py
--rw-r--r--   0        0        0      854 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/__init__.py
--rw-r--r--   0        0        0     1580 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/coupler.py
--rw-r--r--   0        0        0     4153 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2734 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     9309 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/find_modes.py
--rwxr-xr-x   0        0        0     7031 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4506 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2715 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     7083 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4407 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5372 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     7965 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2381 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/overlap.py
--rw-r--r--   0        0        0      410 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0       83 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/tests/test_dw_dh/test_dw_dh.obtained.csv
--rw-r--r--   0        0        0      548 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1129 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      641 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      346 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0      112 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.obtained.csv
--rw-r--r--   0        0        0    16700 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/types.py
--rw-r--r--   0        0        0     1140 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/modes/waveguide.py
--rw-r--r--   0        0        0      248 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/palace/__init__.py
--rw-r--r--   0        0        0     1076 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/palace/driven.json
--rw-r--r--   0        0        0      982 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/palace/electrostatic.json
--rw-r--r--   0        0        0    11386 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/palace/get_capacitance.py
--rw-r--r--   0        0        0    18664 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/palace/get_scattering.py
--rw-r--r--   0        0        0     7214 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/palace/tests/test_palace.py
--rw-r--r--   0        0        0      132 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/path_length_analysis/__init__.py
--rw-r--r--   0        0        0    19671 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/path_length_analysis/path_length_analysis.py
--rw-r--r--   0        0        0     6072 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/path_length_analysis/test_pathlength_extraction.py
--rw-r--r--   0        0        0     2013 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-12-11 16:57:12.121730 gplugins-0.9.8/gplugins/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3009 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/process/__init__.py
--rw-r--r--   0        0        0     4623 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/process/diffusion.py
--rw-r--r--   0        0        0     5318 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/process/implant_tables.py
--rw-r--r--   0        0        0     6879 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      165 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/__init__.py
--rw-r--r--   0        0        0    14727 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/build_model.py
--rw-r--r--   0        0        0        0 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/integrations/__init__.py
--rw-r--r--   0        0        0     7432 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/integrations/femwell_waveguide_model.py
--rw-r--r--   0        0        0     6726 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/integrations/meep_FDTD_model.py
--rw-r--r--   0        0        0     4453 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/integrations/meow_eme_model.py
--rw-r--r--   0        0        0     1546 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/interpolators.py
--rw-r--r--   0        0        0     5613 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/mlp.py
--rw-r--r--   0        0        0     7337 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/models.py
--rw-r--r--   0        0        0    13851 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/parameter.py
--rwxr-xr-x   0        0        0     2223 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/plot_model.py
--rw-r--r--   0        0        0     6591 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/read.py
--rw-r--r--   0        0        0     1349 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2311 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0       76 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.obtained.yml
--rw-r--r--   0        0        0       50 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.yml
--rw-r--r--   0        0        0     1469 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/sax/tests/test_parameters.py
--rw-r--r--   0        0        0      102 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/schematic_editor/__init__.py
--rw-r--r--   0        0        0    16197 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/schematic_editor/circuitviz.py
--rw-r--r--   0        0        0    17770 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/schematic_editor/schematic_editor.py
--rw-r--r--   0        0        0      763 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/__init__.py
--rw-r--r--   0        0        0    31432 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/component.py
--rw-r--r--   0        0        0     4449 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/get_results.py
--rw-r--r--   0        0        0    21177 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     3327 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/materials.py
--rw-r--r--   0        0        0    38999 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/modes.py
--rw-r--r--   0        0        0     1106 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/test_component_modeler.py
--rw-r--r--   0        0        0     1968 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/test_materials.py
--rw-r--r--   0        0        0      262 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      260 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/test_modes/test_sweep_width.obtained.csv
--rw-r--r--   0        0        0      544 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/test_modes_coupler.py
--rw-r--r--   0        0        0      738 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/test_modes_waveguide.py
--rw-r--r--   0        0        0      943 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/test_plot_simulation_grating_coupler.py
--rw-r--r--   0        0        0      532 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/test_write_sparameters.py
--rw-r--r--   0        0        0     9587 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml
--rw-r--r--   0        0        0     1561 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py
--rw-r--r--   0        0        0      938 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py
--rw-r--r--   0        0        0     1898 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0      862 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/types.py
--rw-r--r--   0        0        0     3002 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/util.py
--rw-r--r--   0        0        0    10221 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/tidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0      111 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/vlsir/__init__.py
--rw-r--r--   0        0        0     7047 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/vlsir/export_netlist.py
--rw-r--r--   0        0        0      941 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/vlsir/tests/resources/pads_correct.cir
--rw-r--r--   0        0        0     1262 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/vlsir/tests/resources/pads_correct.scs
--rw-r--r--   0        0        0      932 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/vlsir/tests/resources/pads_correct.sp
--rw-r--r--   0        0        0     1590 2023-12-11 16:57:12.125730 gplugins-0.9.8/gplugins/vlsir/tests/test_vlsir.py
--rw-r--r--   0        0        0     5024 2023-12-11 16:57:12.125730 gplugins-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     5920 1970-01-01 00:00:00.000000 gplugins-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-12-19 00:00:03.746982 gplugins-0.9.9/LICENSE
+-rw-r--r--   0        0        0     2993 2023-12-19 00:00:03.746982 gplugins-0.9.9/README.md
+-rw-r--r--   0        0        0      258 2023-12-19 00:00:03.750982 gplugins-0.9.9/gplugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.750982 gplugins-0.9.9/gplugins/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.750982 gplugins-0.9.9/gplugins/common/base_models/__init__.py
+-rw-r--r--   0        0        0     7201 2023-12-19 00:00:03.750982 gplugins-0.9.9/gplugins/common/base_models/component.py
+-rw-r--r--   0        0        0     2126 2023-12-19 00:00:03.750982 gplugins-0.9.9/gplugins/common/base_models/simulation.py
+-rw-r--r--   0        0        0      716 2023-12-19 00:00:03.750982 gplugins-0.9.9/gplugins/common/config.py
+-rw-r--r--   0        0        0      571 2023-12-19 00:00:03.750982 gplugins-0.9.9/gplugins/common/types.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.750982 gplugins-0.9.9/gplugins/common/utils/__init__.py
+-rw-r--r--   0        0        0     4275 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/add_simulation_markers.py
+-rw-r--r--   0        0        0     4487 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/async_helpers.py
+-rw-r--r--   0        0        0     1216 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/cache.py
+-rw-r--r--   0        0        0     3276 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/convert_sparameters.py
+-rw-r--r--   0        0        0      251 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/disable_print.py
+-rw-r--r--   0        0        0     2857 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/get_capacitance.py
+-rw-r--r--   0        0        0     3921 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/get_component_with_net_layers.py
+-rw-r--r--   0        0        0     3407 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/get_effective_indices.py
+-rw-r--r--   0        0        0     2821 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/get_scattering.py
+-rw-r--r--   0        0        0     2946 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/get_sparameters_path.py
+-rw-r--r--   0        0        0     1484 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/optical_constants.py
+-rw-r--r--   0        0        0     3880 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/parse_layer_stack.py
+-rw-r--r--   0        0        0     6046 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/plot.py
+-rw-r--r--   0        0        0     2439 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/plot_csv.py
+-rw-r--r--   0        0        0      613 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/port_symmetries.py
+-rw-r--r--   0        0        0     1573 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/common/utils/tests/test_get_component_with_new_port_layers.py
+-rw-r--r--   0        0        0       28 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/dagster/Makefile
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/dagster/__init__.py
+-rw-r--r--   0        0        0      933 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/dagster/workflow.py
+-rw-r--r--   0        0        0      571 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/devsim/__init__.py
+-rw-r--r--   0        0        0     2504 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/devsim/doping.py
+-rw-r--r--   0        0        0    11856 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/devsim/get_simulation.py
+-rw-r--r--   0        0        0    28231 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19702 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/devsim/get_solver.py
+-rw-r--r--   0        0        0     1530 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/devsim/test_devsim.py
+-rw-r--r--   0        0        0      129 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/elmer/__init__.py
+-rw-r--r--   0        0        0     4701 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/elmer/electrostatic.sif.j2
+-rw-r--r--   0        0        0    10177 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/elmer/get_capacitance.py
+-rw-r--r--   0        0        0     4070 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/elmer/tests/test_elmer.py
+-rw-r--r--   0        0        0      664 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/fdtdz/__init__.py
+-rw-r--r--   0        0        0     8549 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/fdtdz/get_epsilon_fdtdz.py
+-rw-r--r--   0        0        0     7146 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/fdtdz/get_ports_fdtdz.py
+-rw-r--r--   0        0        0     5473 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/fdtdz/get_sparameters_fdtdz.py
+-rw-r--r--   0        0        0      196 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/femwell/__init__.py
+-rw-r--r--   0        0        0     8465 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/femwell/mode_solver.py
+-rw-r--r--   0        0        0     3168 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/femwell/solve_thermal.py
+-rw-r--r--   0        0        0     1353 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/femwell/test_mode_solver.py
+-rw-r--r--   0        0        0     1926 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/__init__.py
+-rw-r--r--   0        0        0     3853 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/get_material.py
+-rw-r--r--   0        0        0     6308 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6028 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    11392 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15878 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    18139 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12263 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11862 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0     2000 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6146 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    13921 2023-12-19 00:00:03.754982 gplugins-0.9.9/gplugins/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    23177 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8095 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9551 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0      850 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/__init__.py
+-rw-r--r--   0        0        0     1360 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/define_polysurfaces.py
+-rw-r--r--   0        0        0     5481 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/get_mesh.py
+-rw-r--r--   0        0        0     7758 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3844 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/parse_gds.py
+-rw-r--r--   0        0        0    10756 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     2686 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/tests/test_custom_names.py
+-rw-r--r--   0        0        0     1952 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/tests/test_meshing_2D.py
+-rw-r--r--   0        0        0     1612 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/tests/test_meshing_3D.py
+-rw-r--r--   0        0        0    17653 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     9533 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0    14087 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/__init__.py
+-rw-r--r--   0        0        0      312 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/dataprep/__init__.py
+-rw-r--r--   0        0        0     6898 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/dataprep/regions.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/drc/__init__.py
+-rw-r--r--   0        0        0      532 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/drc/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2684 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/drc/check_exclusion.py
+-rw-r--r--   0        0        0     2794 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/drc/check_inclusion.py
+-rw-r--r--   0        0        0     3550 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/drc/check_space.py
+-rw-r--r--   0        0        0     1813 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/drc/check_width.py
+-rw-r--r--   0        0        0     2659 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/drc/count_drc.py
+-rw-r--r--   0        0        0     3580 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/drc/write_connectivity.py
+-rw-r--r--   0        0        0    14201 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/drc/write_drc.py
+-rw-r--r--   0        0        0     3879 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/get_netlist.py
+-rw-r--r--   0        0        0      566 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/netlist_spice_reader.py
+-rw-r--r--   0        0        0     6782 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/plot_nets.py
+-rw-r--r--   0        0        0     2546 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/tests/test_dataprep_regions.py
+-rw-r--r--   0        0        0      951 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/tests/test_drc_exclusion.py
+-rw-r--r--   0        0        0     1149 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/tests/test_drc_inclusion.py
+-rw-r--r--   0        0        0      619 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/tests/test_drc_space.py
+-rw-r--r--   0        0        0     1281 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/tests/test_drc_width.py
+-rw-r--r--   0        0        0     2495 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/tests/test_geometry_write_connectivity.py
+-rw-r--r--   0        0        0      725 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/tests/test_netlist_spice_reader.py
+-rw-r--r--   0        0        0     1952 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/klayout/tests/test_plot_nets.py
+-rw-r--r--   0        0        0      536 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/lumerical/__init__.py
+-rw-r--r--   0        0        0    16025 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4236 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/lumerical/settings.py
+-rw-r--r--   0        0        0     2360 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/lumerical/tests/test_lumerical_read_sparameters.py
+-rw-r--r--   0        0        0    19828 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     2534 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/materials/__init__.py
+-rw-r--r--   0        0        0     1776 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/materials/inorganic.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/materials/optical/__init__.py
+-rw-r--r--   0        0        0     1847 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/materials/optical/optical_mat.py
+-rw-r--r--   0        0        0    23894 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/materials/optical/refractive_index_info.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/materials/semiconductor/__init__.py
+-rw-r--r--   0        0        0      273 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/materials/semiconductor/semiconductor_mat.py
+-rw-r--r--   0        0        0       67 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/meow/__init__.py
+-rw-r--r--   0        0        0    16624 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/meow/meow_eme.py
+-rw-r--r--   0        0        0     2269 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/meow/test_meow_simulation.py
+-rw-r--r--   0        0        0      854 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/__init__.py
+-rw-r--r--   0        0        0     1580 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/coupler.py
+-rw-r--r--   0        0        0     4153 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2734 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     9309 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/find_modes.py
+-rwxr-xr-x   0        0        0     7031 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4506 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2715 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     7083 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4407 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5372 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     7965 2023-12-19 00:00:03.758982 gplugins-0.9.9/gplugins/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2381 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/overlap.py
+-rw-r--r--   0        0        0      410 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0       83 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/tests/test_dw_dh/test_dw_dh.obtained.csv
+-rw-r--r--   0        0        0      548 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1129 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      641 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      346 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0      112 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.obtained.csv
+-rw-r--r--   0        0        0    16700 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/types.py
+-rw-r--r--   0        0        0     1140 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/modes/waveguide.py
+-rw-r--r--   0        0        0      248 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/palace/__init__.py
+-rw-r--r--   0        0        0     1076 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/palace/driven.json
+-rw-r--r--   0        0        0      982 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/palace/electrostatic.json
+-rw-r--r--   0        0        0    11386 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/palace/get_capacitance.py
+-rw-r--r--   0        0        0    18664 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/palace/get_scattering.py
+-rw-r--r--   0        0        0     7214 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/palace/tests/test_palace.py
+-rw-r--r--   0        0        0      132 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/path_length_analysis/__init__.py
+-rw-r--r--   0        0        0    19671 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/path_length_analysis/path_length_analysis.py
+-rw-r--r--   0        0        0     6072 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/path_length_analysis/test_pathlength_extraction.py
+-rw-r--r--   0        0        0     2013 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3009 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/process/__init__.py
+-rw-r--r--   0        0        0     4623 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/process/diffusion.py
+-rw-r--r--   0        0        0     5318 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/process/implant_tables.py
+-rw-r--r--   0        0        0     6879 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      165 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/__init__.py
+-rw-r--r--   0        0        0    14727 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/build_model.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/integrations/__init__.py
+-rw-r--r--   0        0        0     7432 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/integrations/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     6726 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/integrations/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4453 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/integrations/meow_eme_model.py
+-rw-r--r--   0        0        0     1546 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/interpolators.py
+-rw-r--r--   0        0        0     5613 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/mlp.py
+-rw-r--r--   0        0        0     7337 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/models.py
+-rw-r--r--   0        0        0    13851 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/parameter.py
+-rwxr-xr-x   0        0        0     2223 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/plot_model.py
+-rw-r--r--   0        0        0     6591 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/read.py
+-rw-r--r--   0        0        0     1349 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2311 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0       76 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.obtained.yml
+-rw-r--r--   0        0        0       50 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.yml
+-rw-r--r--   0        0        0     1469 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0      102 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/schematic_editor/__init__.py
+-rw-r--r--   0        0        0    16197 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/schematic_editor/circuitviz.py
+-rw-r--r--   0        0        0    17770 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/schematic_editor/schematic_editor.py
+-rw-r--r--   0        0        0      763 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/__init__.py
+-rw-r--r--   0        0        0    31432 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/component.py
+-rw-r--r--   0        0        0     4449 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/get_results.py
+-rw-r--r--   0        0        0    21177 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     3327 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/materials.py
+-rw-r--r--   0        0        0    38999 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/modes.py
+-rw-r--r--   0        0        0     1106 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/tests/test_component_modeler.py
+-rw-r--r--   0        0        0     1968 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/tests/test_materials.py
+-rw-r--r--   0        0        0      262 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      260 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/tests/test_modes/test_sweep_width.obtained.csv
+-rw-r--r--   0        0        0      544 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/tests/test_modes_coupler.py
+-rw-r--r--   0        0        0      738 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/tests/test_modes_waveguide.py
+-rw-r--r--   0        0        0      943 2023-12-19 00:00:03.762982 gplugins-0.9.9/gplugins/tidy3d/tests/test_plot_simulation_grating_coupler.py
+-rw-r--r--   0        0        0      532 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/tidy3d/tests/test_write_sparameters.py
+-rw-r--r--   0        0        0     9587 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml
+-rw-r--r--   0        0        0     1561 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py
+-rw-r--r--   0        0        0      938 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py
+-rw-r--r--   0        0        0     1898 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0      862 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/tidy3d/types.py
+-rw-r--r--   0        0        0     3002 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/tidy3d/util.py
+-rw-r--r--   0        0        0    10221 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/tidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0      111 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/vlsir/__init__.py
+-rw-r--r--   0        0        0     7047 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/vlsir/export_netlist.py
+-rw-r--r--   0        0        0      941 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/vlsir/tests/resources/pads_correct.cir
+-rw-r--r--   0        0        0     1262 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/vlsir/tests/resources/pads_correct.scs
+-rw-r--r--   0        0        0      932 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/vlsir/tests/resources/pads_correct.sp
+-rw-r--r--   0        0        0     1590 2023-12-19 00:00:03.766982 gplugins-0.9.9/gplugins/vlsir/tests/test_vlsir.py
+-rw-r--r--   0        0        0     5015 2023-12-19 00:00:03.766982 gplugins-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     5911 1970-01-01 00:00:00.000000 gplugins-0.9.9/PKG-INFO
```

### Comparing `gplugins-0.9.8/LICENSE` & `gplugins-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/README.md` & `gplugins-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gplugins 0.9.8
+# gplugins 0.9.9
 
 [![docs](https://github.com/gdsfactory/gplugins/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gplugins/)
 [![PyPI](https://img.shields.io/pypi/v/gplugins)](https://pypi.org/project/gplugins/)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gplugins.svg)](https://pypi.python.org/pypi/gplugins)
 [![MIT](https://img.shields.io/github/license/gdsfactory/gplugins)](https://choosealicense.com/licenses/mit/)
 [![codecov](https://img.shields.io/codecov/c/github/gdsfactory/gplugins)](https://codecov.io/gh/gdsfactory/gdsfactory/tree/main/gplugins)
```

### Comparing `gplugins-0.9.8/gplugins/common/base_models/component.py` & `gplugins-0.9.9/gplugins/common/base_models/component.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/base_models/simulation.py` & `gplugins-0.9.9/gplugins/common/base_models/simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/config.py` & `gplugins-0.9.9/gplugins/common/config.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/types.py` & `gplugins-0.9.9/gplugins/common/types.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/add_simulation_markers.py` & `gplugins-0.9.9/gplugins/common/utils/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/async_helpers.py` & `gplugins-0.9.9/gplugins/common/utils/async_helpers.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/cache.py` & `gplugins-0.9.9/gplugins/common/utils/cache.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/convert_sparameters.py` & `gplugins-0.9.9/gplugins/common/utils/convert_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/get_capacitance.py` & `gplugins-0.9.9/gplugins/common/utils/get_capacitance.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/get_component_with_net_layers.py` & `gplugins-0.9.9/gplugins/common/utils/get_component_with_net_layers.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/get_effective_indices.py` & `gplugins-0.9.9/gplugins/common/utils/get_effective_indices.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/get_scattering.py` & `gplugins-0.9.9/gplugins/common/utils/get_scattering.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/get_sparameters_path.py` & `gplugins-0.9.9/gplugins/common/utils/get_sparameters_path.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/optical_constants.py` & `gplugins-0.9.9/gplugins/common/utils/optical_constants.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/parse_layer_stack.py` & `gplugins-0.9.9/gplugins/common/utils/parse_layer_stack.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/plot.py` & `gplugins-0.9.9/gplugins/common/utils/plot.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/plot_csv.py` & `gplugins-0.9.9/gplugins/common/utils/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/port_symmetries.py` & `gplugins-0.9.9/gplugins/common/utils/port_symmetries.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/common/utils/tests/test_get_component_with_new_port_layers.py` & `gplugins-0.9.9/gplugins/common/utils/tests/test_get_component_with_new_port_layers.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/dagster/workflow.py` & `gplugins-0.9.9/gplugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/devsim/__init__.py` & `gplugins-0.9.9/gplugins/devsim/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/devsim/doping.py` & `gplugins-0.9.9/gplugins/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/devsim/get_simulation.py` & `gplugins-0.9.9/gplugins/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/devsim/get_simulation_xsection.py` & `gplugins-0.9.9/gplugins/devsim/get_simulation_xsection.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/devsim/get_solver.py` & `gplugins-0.9.9/gplugins/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/devsim/test_devsim.py` & `gplugins-0.9.9/gplugins/devsim/test_devsim.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/elmer/electrostatic.sif.j2` & `gplugins-0.9.9/gplugins/elmer/electrostatic.sif.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/elmer/get_capacitance.py` & `gplugins-0.9.9/gplugins/elmer/get_capacitance.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/elmer/tests/test_elmer.py` & `gplugins-0.9.9/gplugins/elmer/tests/test_elmer.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/fdtdz/__init__.py` & `gplugins-0.9.9/gplugins/fdtdz/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/fdtdz/get_epsilon_fdtdz.py` & `gplugins-0.9.9/gplugins/fdtdz/get_epsilon_fdtdz.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/fdtdz/get_ports_fdtdz.py` & `gplugins-0.9.9/gplugins/fdtdz/get_ports_fdtdz.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/fdtdz/get_sparameters_fdtdz.py` & `gplugins-0.9.9/gplugins/fdtdz/get_sparameters_fdtdz.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/femwell/mode_solver.py` & `gplugins-0.9.9/gplugins/femwell/mode_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/femwell/solve_thermal.py` & `gplugins-0.9.9/gplugins/femwell/solve_thermal.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/femwell/test_mode_solver.py` & `gplugins-0.9.9/gplugins/femwell/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/__init__.py` & `gplugins-0.9.9/gplugins/gmeep/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/get_material.py` & `gplugins-0.9.9/gplugins/gmeep/get_material.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/get_meep_geometry.py` & `gplugins-0.9.9/gplugins/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/get_port_eigenmode.py` & `gplugins-0.9.9/gplugins/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/get_simulation.py` & `gplugins-0.9.9/gplugins/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/get_simulation_grating_farfield.py` & `gplugins-0.9.9/gplugins/gmeep/get_simulation_grating_farfield.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/get_simulation_grating_fiber.py` & `gplugins-0.9.9/gplugins/gmeep/get_simulation_grating_fiber.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,17 @@
     top_clad_material = mp.Medium(index=clad_material)
     bottom_clad_material = mp.Medium(index=nbox)
     fiber_core_material = (fiber_numerical_aperture**2 + fiber_clad_material**2) ** 0.5
     fiber_clad_material = mp.Medium(index=fiber_clad_material)
     fiber_core_material = mp.Medium(index=fiber_core_material)
 
     # Useful reference point
-    grating_start = -fiber_xposition  # Since fiber dominates, keep it centered and offset the grating
+    grating_start = (
+        -fiber_xposition
+    )  # Since fiber dominates, keep it centered and offset the grating
 
     # Initialize domain x-z plane simulation
     cell_size = mp.Vector3(sxy, sz)
 
     # Ports (position, sizes, directions)
     fiber_port_y = -sz / 2 + (
         +pml_thickness
```

### Comparing `gplugins-0.9.8/gplugins/gmeep/meep_adjoint_optimization.py` & `gplugins-0.9.9/gplugins/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_eigenmode.py` & `gplugins-0.9.9/gplugins/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_materials.py` & `gplugins-0.9.9/gplugins/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gplugins-0.9.9/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gplugins-0.9.9/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep.py` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gplugins-0.9.9/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/write_sparameters_grating.py` & `gplugins-0.9.9/gplugins/gmeep/write_sparameters_grating.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/write_sparameters_meep.py` & `gplugins-0.9.9/gplugins/gmeep/write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/write_sparameters_meep_batch.py` & `gplugins-0.9.9/gplugins/gmeep/write_sparameters_meep_batch.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmeep/write_sparameters_meep_mpi.py` & `gplugins-0.9.9/gplugins/gmeep/write_sparameters_meep_mpi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/__init__.py` & `gplugins-0.9.9/gplugins/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/define_polysurfaces.py` & `gplugins-0.9.9/gplugins/gmsh/define_polysurfaces.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/get_mesh.py` & `gplugins-0.9.9/gplugins/gmsh/get_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/parse_component.py` & `gplugins-0.9.9/gplugins/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/parse_gds.py` & `gplugins-0.9.9/gplugins/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/scratch/mesh3D.py` & `gplugins-0.9.9/gplugins/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/tests/test_custom_names.py` & `gplugins-0.9.9/gplugins/gmsh/tests/test_custom_names.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/tests/test_meshing_2D.py` & `gplugins-0.9.9/gplugins/gmsh/tests/test_meshing_2D.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/tests/test_meshing_3D.py` & `gplugins-0.9.9/gplugins/gmsh/tests/test_meshing_3D.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/uz_xsection_mesh.py` & `gplugins-0.9.9/gplugins/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/xy_xsection_mesh.py` & `gplugins-0.9.9/gplugins/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/gmsh/xyz_mesh.py` & `gplugins-0.9.9/gplugins/gmsh/xyz_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/dataprep/regions.py` & `gplugins-0.9.9/gplugins/klayout/dataprep/regions.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/drc/check_duplicated_cells.py` & `gplugins-0.9.9/gplugins/klayout/drc/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/drc/check_exclusion.py` & `gplugins-0.9.9/gplugins/klayout/drc/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/drc/check_inclusion.py` & `gplugins-0.9.9/gplugins/klayout/drc/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/drc/check_space.py` & `gplugins-0.9.9/gplugins/klayout/drc/check_space.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/drc/check_width.py` & `gplugins-0.9.9/gplugins/klayout/drc/check_width.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/drc/write_connectivity.py` & `gplugins-0.9.9/gplugins/klayout/drc/write_connectivity.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/drc/write_drc.py` & `gplugins-0.9.9/gplugins/klayout/drc/write_drc.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/get_netlist.py` & `gplugins-0.9.9/gplugins/klayout/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/netlist_spice_reader.py` & `gplugins-0.9.9/gplugins/klayout/netlist_spice_reader.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/plot_nets.py` & `gplugins-0.9.9/gplugins/klayout/plot_nets.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/tests/test_dataprep_regions.py` & `gplugins-0.9.9/gplugins/klayout/tests/test_dataprep_regions.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/tests/test_drc_exclusion.py` & `gplugins-0.9.9/gplugins/klayout/tests/test_drc_exclusion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/tests/test_drc_inclusion.py` & `gplugins-0.9.9/gplugins/klayout/tests/test_drc_inclusion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/tests/test_drc_space.py` & `gplugins-0.9.9/gplugins/klayout/tests/test_drc_space.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/tests/test_drc_width.py` & `gplugins-0.9.9/gplugins/klayout/tests/test_drc_width.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/tests/test_geometry_write_connectivity.py` & `gplugins-0.9.9/gplugins/klayout/tests/test_geometry_write_connectivity.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/tests/test_netlist_spice_reader.py` & `gplugins-0.9.9/gplugins/klayout/tests/test_netlist_spice_reader.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/klayout/tests/test_plot_nets.py` & `gplugins-0.9.9/gplugins/klayout/tests/test_plot_nets.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/lumerical/__init__.py` & `gplugins-0.9.9/gplugins/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/lumerical/interconnect.py` & `gplugins-0.9.9/gplugins/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/lumerical/read.py` & `gplugins-0.9.9/gplugins/lumerical/read.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/lumerical/settings.py` & `gplugins-0.9.9/gplugins/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/lumerical/tests/test_lumerical_read_sparameters.py` & `gplugins-0.9.9/gplugins/lumerical/tests/test_lumerical_read_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/lumerical/write_sparameters_lumerical.py` & `gplugins-0.9.9/gplugins/lumerical/write_sparameters_lumerical.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/lumerical/write_sparameters_lumerical_components.py` & `gplugins-0.9.9/gplugins/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/materials/inorganic.py` & `gplugins-0.9.9/gplugins/materials/inorganic.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/materials/optical/optical_mat.py` & `gplugins-0.9.9/gplugins/materials/optical/optical_mat.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/materials/optical/refractive_index_info.py` & `gplugins-0.9.9/gplugins/materials/optical/refractive_index_info.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/meow/meow_eme.py` & `gplugins-0.9.9/gplugins/meow/meow_eme.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/meow/test_meow_simulation.py` & `gplugins-0.9.9/gplugins/meow/test_meow_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/__init__.py` & `gplugins-0.9.9/gplugins/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/coupler.py` & `gplugins-0.9.9/gplugins/modes/coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/find_coupling_vs_gap.py` & `gplugins-0.9.9/gplugins/modes/find_coupling_vs_gap.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/find_mode_dispersion.py` & `gplugins-0.9.9/gplugins/modes/find_mode_dispersion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/find_modes.py` & `gplugins-0.9.9/gplugins/modes/find_modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/find_modes_cross_section.py` & `gplugins-0.9.9/gplugins/modes/find_modes_cross_section.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/find_neff_ng_dw_dh.py` & `gplugins-0.9.9/gplugins/modes/find_neff_ng_dw_dh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/find_neff_vs_width.py` & `gplugins-0.9.9/gplugins/modes/find_neff_vs_width.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/get_mode_solver_coupler.py` & `gplugins-0.9.9/gplugins/modes/get_mode_solver_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/get_mode_solver_cross_section.py` & `gplugins-0.9.9/gplugins/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/get_mode_solver_rib.py` & `gplugins-0.9.9/gplugins/modes/get_mode_solver_rib.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/modes/neff_vs_width_nitride.csv` & `gplugins-0.9.9/gplugins/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/modes/neff_vs_width_rib.csv` & `gplugins-0.9.9/gplugins/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/modes/neff_vs_width_strip.csv` & `gplugins-0.9.9/gplugins/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/neff_convergence_test.py` & `gplugins-0.9.9/gplugins/modes/neff_convergence_test.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/overlap.py` & `gplugins-0.9.9/gplugins/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gplugins-0.9.9/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/tests/test_find_modes.py` & `gplugins-0.9.9/gplugins/modes/tests/test_find_modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/tests/test_find_modes_dispersion.py` & `gplugins-0.9.9/gplugins/modes/tests/test_find_modes_dispersion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/types.py` & `gplugins-0.9.9/gplugins/modes/types.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/modes/waveguide.py` & `gplugins-0.9.9/gplugins/modes/waveguide.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/palace/driven.json` & `gplugins-0.9.9/gplugins/palace/driven.json`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/palace/electrostatic.json` & `gplugins-0.9.9/gplugins/palace/electrostatic.json`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/palace/get_capacitance.py` & `gplugins-0.9.9/gplugins/palace/get_capacitance.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/palace/get_scattering.py` & `gplugins-0.9.9/gplugins/palace/get_scattering.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/palace/tests/test_palace.py` & `gplugins-0.9.9/gplugins/palace/tests/test_palace.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/path_length_analysis/path_length_analysis.py` & `gplugins-0.9.9/gplugins/path_length_analysis/path_length_analysis.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/path_length_analysis/test_pathlength_extraction.py` & `gplugins-0.9.9/gplugins/path_length_analysis/test_pathlength_extraction.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/photonic_circuit_models/__init__.py` & `gplugins-0.9.9/gplugins/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/photonic_circuit_models/coupler.py` & `gplugins-0.9.9/gplugins/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/photonic_circuit_models/mzi.py` & `gplugins-0.9.9/gplugins/photonic_circuit_models/mzi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/photonic_circuit_models/ring.py` & `gplugins-0.9.9/gplugins/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/process/diffusion.py` & `gplugins-0.9.9/gplugins/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/process/implant_tables.py` & `gplugins-0.9.9/gplugins/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/process/pysrim.py` & `gplugins-0.9.9/gplugins/process/pysrim.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/process/silicon.py` & `gplugins-0.9.9/gplugins/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/process/skew/antimony_si_skew.csv` & `gplugins-0.9.9/gplugins/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/process/skew/arsenic_si_skew.csv` & `gplugins-0.9.9/gplugins/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/process/skew/boron_si_skew.csv` & `gplugins-0.9.9/gplugins/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/process/skew/phosphorus_si_skew.csv` & `gplugins-0.9.9/gplugins/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/build_model.py` & `gplugins-0.9.9/gplugins/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/integrations/femwell_waveguide_model.py` & `gplugins-0.9.9/gplugins/sax/integrations/femwell_waveguide_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/integrations/meep_FDTD_model.py` & `gplugins-0.9.9/gplugins/sax/integrations/meep_FDTD_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/integrations/meow_eme_model.py` & `gplugins-0.9.9/gplugins/sax/integrations/meow_eme_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/interpolators.py` & `gplugins-0.9.9/gplugins/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/mlp.py` & `gplugins-0.9.9/gplugins/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/models.py` & `gplugins-0.9.9/gplugins/sax/models.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/parameter.py` & `gplugins-0.9.9/gplugins/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/plot_model.py` & `gplugins-0.9.9/gplugins/sax/plot_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/read.py` & `gplugins-0.9.9/gplugins/sax/read.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/tests/test_mzi.py` & `gplugins-0.9.9/gplugins/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/tests/test_mzi_lattice.py` & `gplugins-0.9.9/gplugins/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/sax/tests/test_parameters.py` & `gplugins-0.9.9/gplugins/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/schematic_editor/circuitviz.py` & `gplugins-0.9.9/gplugins/schematic_editor/circuitviz.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/schematic_editor/schematic_editor.py` & `gplugins-0.9.9/gplugins/schematic_editor/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/__init__.py` & `gplugins-0.9.9/gplugins/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/component.py` & `gplugins-0.9.9/gplugins/tidy3d/component.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/get_results.py` & `gplugins-0.9.9/gplugins/tidy3d/get_results.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/get_simulation_grating_coupler.py` & `gplugins-0.9.9/gplugins/tidy3d/get_simulation_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/materials.py` & `gplugins-0.9.9/gplugins/tidy3d/materials.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/modes.py` & `gplugins-0.9.9/gplugins/tidy3d/modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/test_component_modeler.py` & `gplugins-0.9.9/gplugins/tidy3d/tests/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/test_materials.py` & `gplugins-0.9.9/gplugins/tidy3d/tests/test_materials.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/test_modes_coupler.py` & `gplugins-0.9.9/gplugins/tidy3d/tests/test_modes_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/test_modes_waveguide.py` & `gplugins-0.9.9/gplugins/tidy3d/tests/test_modes_waveguide.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/test_plot_simulation_grating_coupler.py` & `gplugins-0.9.9/gplugins/tidy3d/tests/test_plot_simulation_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/test_write_sparameters.py` & `gplugins-0.9.9/gplugins/tidy3d/tests/test_write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml` & `gplugins-0.9.9/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py` & `gplugins-0.9.9/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py` & `gplugins-0.9.9/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py` & `gplugins-0.9.9/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/types.py` & `gplugins-0.9.9/gplugins/tidy3d/types.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/util.py` & `gplugins-0.9.9/gplugins/tidy3d/util.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/tidy3d/write_sparameters_grating_coupler.py` & `gplugins-0.9.9/gplugins/tidy3d/write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/vlsir/export_netlist.py` & `gplugins-0.9.9/gplugins/vlsir/export_netlist.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/vlsir/tests/resources/pads_correct.cir` & `gplugins-0.9.9/gplugins/vlsir/tests/resources/pads_correct.cir`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/vlsir/tests/resources/pads_correct.scs` & `gplugins-0.9.9/gplugins/vlsir/tests/resources/pads_correct.scs`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/vlsir/tests/resources/pads_correct.sp` & `gplugins-0.9.9/gplugins/vlsir/tests/resources/pads_correct.sp`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/gplugins/vlsir/tests/test_vlsir.py` & `gplugins-0.9.9/gplugins/vlsir/tests/test_vlsir.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.9.8/pyproject.toml` & `gplugins-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 description = "gdsfactory plugins"
 keywords = ["python"]
 license = {file = "LICENSE"}
 name = "gplugins"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.9.8"
+version = "0.9.9"
 
 [project.optional-dependencies]
 dagster = ["dagster", "dagit"]
 dev = [
   "pre-commit",
   "pytest",
   "pytest-cov",
@@ -40,15 +40,15 @@
   "tbump",
   "towncrier",
   "ray"
 ]
 devsim = [
   "devsim",
   "pyvista<=0.40",
-  "tidy3d==2.5.0rc3"
+  "tidy3d==2.5.0"
 ]
 docs = [
   "jupytext",
   "matplotlib",
   "jupyter-book==0.15.1",
   "pyvista[jupyter]<=0.40"
 ]
@@ -71,28 +71,28 @@
   "kfactory[git,ipy]>=0.9.3,<0.11",
   "pyvis<=0.3.1"
 ]
 meow = [
   "jaxlib",
   "jax",
   "meow-sim>0.8,<0.9",
-  "tidy3d==2.5.0rc3"
+  "tidy3d==2.5.0"
 ]
 sax = [
   "jaxlib",
   "jax",
   "sax>=0.10.3,<0.11.0",
   "scikit-learn"
 ]
 schematic = [
   "bokeh",
   "natsort"
 ]
 tidy3d = [
-  "tidy3d==2.5.0rc3",
+  "tidy3d==2.5.0",
   "meshio",
   "meshwell>=1.0.0,<1.1"
 ]
 vlsir = [
   "vlsir>=4.0.0,<6.0.0",
   "vlsirtools>=4.0.0,<6.0.0"
 ]
@@ -203,15 +203,15 @@
 src = "gplugins/__init__.py"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.tbump.version]
-current = "0.9.8"
+current = "0.9.9"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
```

### Comparing `gplugins-0.9.8/PKG-INFO` & `gplugins-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gplugins
-Version: 0.9.8
+Version: 0.9.9
 Summary: gdsfactory plugins
 Keywords: python
 Author-email: gdsfactory <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,15 @@
 Requires-Dist: autograd ; extra == "dev"
 Requires-Dist: hyperopt ; extra == "dev"
 Requires-Dist: tbump ; extra == "dev"
 Requires-Dist: towncrier ; extra == "dev"
 Requires-Dist: ray ; extra == "dev"
 Requires-Dist: devsim ; extra == "devsim"
 Requires-Dist: pyvista<=0.40 ; extra == "devsim"
-Requires-Dist: tidy3d==2.5.0rc3 ; extra == "devsim"
+Requires-Dist: tidy3d==2.5.0 ; extra == "devsim"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "docs"
 Requires-Dist: jupyter-book==0.15.1 ; extra == "docs"
 Requires-Dist: pyvista[jupyter]<=0.40 ; extra == "docs"
 Requires-Dist: femwell>=0.1.6,<0.2 ; extra == "femwell"
 Requires-Dist: meshwell>=1.0.0,<1.1 ; extra == "femwell"
 Requires-Dist: gmsh ; extra == "gmsh"
@@ -44,22 +44,22 @@
 Requires-Dist: shapely ; extra == "gmsh"
 Requires-Dist: meshwell>=1.0.0,<1.1.0 ; extra == "gmsh"
 Requires-Dist: kfactory[git,ipy]>=0.9.3,<0.11 ; extra == "klayout"
 Requires-Dist: pyvis<=0.3.1 ; extra == "klayout"
 Requires-Dist: jaxlib ; extra == "meow"
 Requires-Dist: jax ; extra == "meow"
 Requires-Dist: meow-sim>0.8,<0.9 ; extra == "meow"
-Requires-Dist: tidy3d==2.5.0rc3 ; extra == "meow"
+Requires-Dist: tidy3d==2.5.0 ; extra == "meow"
 Requires-Dist: jaxlib ; extra == "sax"
 Requires-Dist: jax ; extra == "sax"
 Requires-Dist: sax>=0.10.3,<0.11.0 ; extra == "sax"
 Requires-Dist: scikit-learn ; extra == "sax"
 Requires-Dist: bokeh ; extra == "schematic"
 Requires-Dist: natsort ; extra == "schematic"
-Requires-Dist: tidy3d==2.5.0rc3 ; extra == "tidy3d"
+Requires-Dist: tidy3d==2.5.0 ; extra == "tidy3d"
 Requires-Dist: meshio ; extra == "tidy3d"
 Requires-Dist: meshwell>=1.0.0,<1.1 ; extra == "tidy3d"
 Requires-Dist: vlsir>=4.0.0,<6.0.0 ; extra == "vlsir"
 Requires-Dist: vlsirtools>=4.0.0,<6.0.0 ; extra == "vlsir"
 Provides-Extra: dagster
 Provides-Extra: dev
 Provides-Extra: devsim
@@ -69,15 +69,15 @@
 Provides-Extra: klayout
 Provides-Extra: meow
 Provides-Extra: sax
 Provides-Extra: schematic
 Provides-Extra: tidy3d
 Provides-Extra: vlsir
 
-# gplugins 0.9.8
+# gplugins 0.9.9
 
 [![docs](https://github.com/gdsfactory/gplugins/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gplugins/)
 [![PyPI](https://img.shields.io/pypi/v/gplugins)](https://pypi.org/project/gplugins/)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gplugins.svg)](https://pypi.python.org/pypi/gplugins)
 [![MIT](https://img.shields.io/github/license/gdsfactory/gplugins)](https://choosealicense.com/licenses/mit/)
 [![codecov](https://img.shields.io/codecov/c/github/gdsfactory/gplugins)](https://codecov.io/gh/gdsfactory/gdsfactory/tree/main/gplugins)
```

