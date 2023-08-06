# Comparing `tmp/gplugins-0.0.3.tar.gz` & `tmp/gplugins-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gplugins-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gplugins-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gplugins-0.0.3.tar` & `gplugins-0.1.0.tar`

### file list

```diff
@@ -1,205 +1,208 @@
--rw-r--r--   0        0        0     1077 2023-08-03 23:24:20.872192 gplugins-0.0.3/LICENSE
--rw-r--r--   0        0        0     2217 2023-08-03 23:24:20.872192 gplugins-0.0.3/README.md
--rw-r--r--   0        0        0      244 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/__init__.py
--rw-r--r--   0        0        0      603 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/config.py
--rw-r--r--   0        0        0       28 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/dagster/Makefile
--rw-r--r--   0        0        0        0 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/dagster/__init__.py
--rw-r--r--   0        0        0      933 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/dagster/workflow.py
--rw-r--r--   0        0        0      566 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/database/README.md
--rw-r--r--   0        0        0        0 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/database/__init__.py
--rw-r--r--   0        0        0     6142 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/database/db_upload.py
--rw-r--r--   0        0        0    16141 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/database/models.py
--rw-r--r--   0        0        0      571 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/__init__.py
--rw-r--r--   0        0        0     2569 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/doping.py
--rw-r--r--   0        0        0    11898 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/get_simulation.py
--rw-r--r--   0        0        0    28843 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19679 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/get_solver.py
--rw-r--r--   0        0        0     1598 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/test_devsim.py
--rw-r--r--   0        0        0      198 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/eme/__init__.py
--rw-r--r--   0        0        0      207 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/fem/__init__.py
--rw-r--r--   0        0        0      107 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/femwell/__init__.py
--rw-r--r--   0        0        0     8557 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/femwell/mode_solver.py
--rw-r--r--   0        0        0     7772 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/femwell/solve_thermal.py
--rw-r--r--   0        0        0     1414 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/femwell/test_mode_solver.py
--rw-r--r--   0        0        0     1906 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/__init__.py
--rw-r--r--   0        0        0     1311 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/async_utils.py
--rw-r--r--   0        0        0     3151 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_material.py
--rw-r--r--   0        0        0     6037 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6028 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    10937 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15892 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    18153 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12263 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11862 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0      820 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6189 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    13928 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    21199 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8081 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9528 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0     1168 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/__init__.py
--rw-r--r--   0        0        0     6640 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/break_geometry.py
--rw-r--r--   0        0        0    11103 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/mesh.py
--rw-r--r--   0        0        0    11769 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/meshtracker.py
--rw-r--r--   0        0        0     7714 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/parse_component.py
--rw-r--r--   0        0        0     3644 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/parse_gds.py
--rw-r--r--   0        0        0     3619 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/parse_layerstack.py
--rw-r--r--   0        0        0     2990 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/refine.py
--rw-r--r--   0        0        0    10756 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     1997 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/tests/test_meshing.py
--rw-r--r--   0        0        0    14029 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     7281 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0     9145 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0      220 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gtidy3d/__init__.py
--rw-r--r--   0        0        0      536 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/__init__.py
--rw-r--r--   0        0        0    16025 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/interconnect.py
--rw-r--r--   0        0        0     4229 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/settings.py
--rw-r--r--   0        0        0     2353 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/tests/test_lumerical_read_sparameters.py
--rw-r--r--   0        0        0    19826 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     1459 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0       67 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/meow/__init__.py
--rw-r--r--   0        0        0    16461 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/meow/meow_eme.py
--rw-r--r--   0        0        0     1802 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/meow/test_meow_simulation.py
--rw-r--r--   0        0        0      854 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/__init__.py
--rw-r--r--   0        0        0     1580 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/coupler.py
--rw-r--r--   0        0        0     4153 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2734 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     8811 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_modes.py
--rwxr-xr-x   0        0        0     6968 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4445 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2715 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     7088 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4410 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5377 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     7965 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2443 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/overlap.py
--rw-r--r--   0        0        0      405 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0       83 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_dw_dh/test_dw_dh.obtained.csv
--rw-r--r--   0        0        0      548 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1124 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      636 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      341 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0      112 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.obtained.csv
--rw-r--r--   0        0        0    15453 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/types.py
--rw-r--r--   0        0        0     1140 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/waveguide.py
--rw-r--r--   0        0        0      132 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/path_length_analysis/__init__.py
--rw-r--r--   0        0        0    19360 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/path_length_analysis/path_length_analysis.py
--rw-r--r--   0        0        0     5948 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/path_length_analysis/test_pathlength_extraction.py
--rw-r--r--   0        0        0     2013 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3009 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0        0 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/__init__.py
--rw-r--r--   0        0        0     4623 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/diffusion.py
--rw-r--r--   0        0        0     5318 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/implant_tables.py
--rw-r--r--   0        0        0     6901 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      165 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/__init__.py
--rw-r--r--   0        0        0    14710 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/build_model.py
--rw-r--r--   0        0        0        0 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/integrations/__init__.py
--rw-r--r--   0        0        0     7415 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/integrations/femwell_waveguide_model.py
--rw-r--r--   0        0        0     6725 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/integrations/meep_FDTD_model.py
--rw-r--r--   0        0        0     4492 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/integrations/meow_eme_model.py
--rw-r--r--   0        0        0     1546 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/interpolators.py
--rw-r--r--   0        0        0     5613 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/mlp.py
--rw-r--r--   0        0        0     7345 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/models.py
--rw-r--r--   0        0        0    13837 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/parameter.py
--rwxr-xr-x   0        0        0     2173 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/plot_model.py
--rw-r--r--   0        0        0     6672 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/read.py
--rw-r--r--   0        0        0     1349 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2255 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0       76 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.obtained.yml
--rw-r--r--   0        0        0       76 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.yml
--rw-r--r--   0        0        0     1393 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_parameters.py
--rw-r--r--   0        0        0      102 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/schematic_editor/__init__.py
--rw-r--r--   0        0        0    16197 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/schematic_editor/circuitviz.py
--rw-r--r--   0        0        0    17770 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/schematic_editor/schematic_editor.py
--rw-r--r--   0        0        0     1541 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/__init__.py
--rw-r--r--   0        0        0     4448 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/get_results.py
--rw-r--r--   0        0        0    20040 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/get_simulation.py
--rw-r--r--   0        0        0    21258 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     3462 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/materials.py
--rw-r--r--   0        0        0    37241 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/modes.py
--rw-r--r--   0        0        0     9326 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/sim_ref.yaml
--rw-r--r--   0        0        0      730 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_modes.py
--rw-r--r--   0        0        0      262 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      260 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_modes/test_sweep_width.obtained.csv
--rw-r--r--   0        0        0      852 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_results.py
--rw-r--r--   0        0        0     1562 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_simulation.py
--rw-r--r--   0        0        0     1709 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py
--rw-r--r--   0        0        0     1891 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0     1192 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/utils.py
--rw-r--r--   0        0        0    11050 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/write_sparameters.py
--rw-r--r--   0        0        0     8567 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0        0 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/__init__.py
--rw-r--r--   0        0        0     4262 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/add_simulation_markers.py
--rw-r--r--   0        0        0     3276 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/convert_sparameters.py
--rw-r--r--   0        0        0      251 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/disable_print.py
--rw-r--r--   0        0        0     3407 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/get_effective_indices.py
--rw-r--r--   0        0        0     2893 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/get_sparameters_path.py
--rw-r--r--   0        0        0     5951 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/plot.py
--rw-r--r--   0        0        0     2439 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/plot_csv.py
--rw-r--r--   0        0        0      613 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/port_symmetries.py
--rw-r--r--   0        0        0       32 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/Makefile
--rw-r--r--   0        0        0       23 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/__init__.py
--rw-r--r--   0        0        0      212 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/C.gds
--rw-r--r--   0        0        0      220 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/C_width20.gds
--rw-r--r--   0        0        0      218 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/C_width5.gds
--rw-r--r--   0        0        0    14536 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_rx_dual_pol.gds
--rw-r--r--   0        0        0    13550 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol.gds
--rw-r--r--   0        0        0    13564 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds
--rw-r--r--   0        0        0    13564 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds
--rw-r--r--   0        0        0    10292 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_tx_dual_pol.gds
--rw-r--r--   0        0        0     1498 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/crossing_arm.gds
--rw-r--r--   0        0        0     7406 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/dbr_cavity.gds
--rw-r--r--   0        0        0      440 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/die_bbox_frame.gds
--rw-r--r--   0        0        0    27548 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/loss_deembedding_ch14_23.gds
--rw-r--r--   0        0        0      872 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/pad_array_add_fiducials.gds
--rw-r--r--   0        0        0    39252 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds
--rw-r--r--   0        0        0      182 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/wg.gds
--rw-r--r--   0        0        0     8606 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/main.py
--rw-r--r--   0        0        0     1998 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/middleware.py
--rwxr-xr-x   0        0        0     7546 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/server.py
--rwxr-xr-x   0        0        0      636 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/server_jupyter.py
--rw-r--r--   0        0        0     1299 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/static/client.css
--rw-r--r--   0        0        0     9598 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/static/client.js
--rw-r--r--   0        0        0      840 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/client.html.j2
--rw-r--r--   0        0        0      481 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/file_browser.html.j2
--rw-r--r--   0        0        0     1999 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/filewatcher.html.j2
--rw-r--r--   0        0        0      236 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/footer.html.j2
--rw-r--r--   0        0        0      242 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/gds_history.html.j2
--rw-r--r--   0        0        0      578 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/header.html.j2
--rw-r--r--   0        0        0      376 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/index.html.j2
--rw-r--r--   0        0        0      995 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/navbar.html.j2
--rw-r--r--   0        0        0      272 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/pdk.html.j2
--rw-r--r--   0        0        0     1871 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/viewer.html.j2
--rw-r--r--   0        0        0       87 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/widget/__init__.py
--rw-r--r--   0        0        0    14936 2023-08-03 23:24:20.888192 gplugins-0.0.3/gplugins/widget/interactive.py
--rw-r--r--   0        0        0     3132 2023-08-03 23:24:20.888192 gplugins-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 gplugins-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-06 18:26:48.063156 gplugins-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2235 2023-08-06 18:26:48.063156 gplugins-0.1.0/README.md
+-rw-r--r--   0        0        0      244 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/__init__.py
+-rw-r--r--   0        0        0      603 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/config.py
+-rw-r--r--   0        0        0       28 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/dagster/Makefile
+-rw-r--r--   0        0        0        0 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/dagster/__init__.py
+-rw-r--r--   0        0        0      933 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/dagster/workflow.py
+-rw-r--r--   0        0        0      566 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/database/README.md
+-rw-r--r--   0        0        0        0 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/database/__init__.py
+-rw-r--r--   0        0        0     6142 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/database/db_upload.py
+-rw-r--r--   0        0        0    16141 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/database/models.py
+-rw-r--r--   0        0        0      571 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/__init__.py
+-rw-r--r--   0        0        0     2569 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/doping.py
+-rw-r--r--   0        0        0    11898 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/get_simulation.py
+-rw-r--r--   0        0        0    28255 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19679 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/get_solver.py
+-rw-r--r--   0        0        0     1598 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/test_devsim.py
+-rw-r--r--   0        0        0      198 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/eme/__init__.py
+-rw-r--r--   0        0        0      207 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/fem/__init__.py
+-rw-r--r--   0        0        0      107 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/femwell/__init__.py
+-rw-r--r--   0        0        0     8522 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/femwell/mode_solver.py
+-rw-r--r--   0        0        0     7772 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/femwell/solve_thermal.py
+-rw-r--r--   0        0        0     1414 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/femwell/test_mode_solver.py
+-rw-r--r--   0        0        0     1906 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/__init__.py
+-rw-r--r--   0        0        0     1311 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/async_utils.py
+-rw-r--r--   0        0        0     3151 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_material.py
+-rw-r--r--   0        0        0     6037 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6028 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    10937 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15892 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    18153 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12263 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11862 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0      820 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6189 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    13921 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    21199 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8081 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9528 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0     1168 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/__init__.py
+-rw-r--r--   0        0        0     6640 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/break_geometry.py
+-rw-r--r--   0        0        0    11103 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/mesh.py
+-rw-r--r--   0        0        0    11769 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/meshtracker.py
+-rw-r--r--   0        0        0     7714 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3644 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/parse_gds.py
+-rw-r--r--   0        0        0     3619 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/parse_layerstack.py
+-rw-r--r--   0        0        0     2990 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/refine.py
+-rw-r--r--   0        0        0    10756 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     1997 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/tests/test_meshing.py
+-rw-r--r--   0        0        0    14029 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     7281 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0     9109 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0      220 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gtidy3d/__init__.py
+-rw-r--r--   0        0        0      536 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/__init__.py
+-rw-r--r--   0        0        0    16025 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4229 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/settings.py
+-rw-r--r--   0        0        0     2353 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/tests/test_lumerical_read_sparameters.py
+-rw-r--r--   0        0        0    19821 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     1459 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0       67 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/meow/__init__.py
+-rw-r--r--   0        0        0    16461 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/meow/meow_eme.py
+-rw-r--r--   0        0        0     2301 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/meow/test_meow_simulation.py
+-rw-r--r--   0        0        0      854 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/__init__.py
+-rw-r--r--   0        0        0     1580 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/coupler.py
+-rw-r--r--   0        0        0     4153 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2734 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     8811 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_modes.py
+-rwxr-xr-x   0        0        0     6968 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4445 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2715 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     7088 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4410 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5377 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     7965 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2443 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/overlap.py
+-rw-r--r--   0        0        0      405 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0       83 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_dw_dh/test_dw_dh.obtained.csv
+-rw-r--r--   0        0        0      548 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1124 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      636 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      341 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0      112 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.obtained.csv
+-rw-r--r--   0        0        0    15422 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/types.py
+-rw-r--r--   0        0        0     1140 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/waveguide.py
+-rw-r--r--   0        0        0      132 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/path_length_analysis/__init__.py
+-rw-r--r--   0        0        0    19221 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/path_length_analysis/path_length_analysis.py
+-rw-r--r--   0        0        0     5948 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/path_length_analysis/test_pathlength_extraction.py
+-rw-r--r--   0        0        0     2013 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3009 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0        0 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/__init__.py
+-rw-r--r--   0        0        0     4623 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/diffusion.py
+-rw-r--r--   0        0        0     5318 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/implant_tables.py
+-rw-r--r--   0        0        0     6879 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      165 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/__init__.py
+-rw-r--r--   0        0        0    14710 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/build_model.py
+-rw-r--r--   0        0        0        0 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/integrations/__init__.py
+-rw-r--r--   0        0        0     7415 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/integrations/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     6720 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/integrations/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4492 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/integrations/meow_eme_model.py
+-rw-r--r--   0        0        0     1546 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/interpolators.py
+-rw-r--r--   0        0        0     5613 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/mlp.py
+-rw-r--r--   0        0        0     7345 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/models.py
+-rw-r--r--   0        0        0    13837 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/parameter.py
+-rwxr-xr-x   0        0        0     2222 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/plot_model.py
+-rw-r--r--   0        0        0     6672 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/read.py
+-rw-r--r--   0        0        0     1349 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2255 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0       76 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.obtained.yml
+-rw-r--r--   0        0        0       76 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.yml
+-rw-r--r--   0        0        0     1393 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0      102 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/schematic_editor/__init__.py
+-rw-r--r--   0        0        0    16197 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/schematic_editor/circuitviz.py
+-rw-r--r--   0        0        0    17770 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/schematic_editor/schematic_editor.py
+-rw-r--r--   0        0        0     1541 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/__init__.py
+-rw-r--r--   0        0        0     4448 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/get_results.py
+-rw-r--r--   0        0        0    19950 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/get_simulation.py
+-rw-r--r--   0        0        0    21096 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     3263 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/materials.py
+-rw-r--r--   0        0        0    37811 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/modes.py
+-rw-r--r--   0        0        0     1943 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_materials.py
+-rw-r--r--   0        0        0      730 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_modes.py
+-rw-r--r--   0        0        0      262 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      260 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_modes/test_sweep_width.obtained.csv
+-rw-r--r--   0        0        0      700 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_plot_simulation.py
+-rw-r--r--   0        0        0      936 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_plot_simulation_grating_coupler.py
+-rw-r--r--   0        0        0      852 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_results.py
+-rw-r--r--   0        0        0     9326 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml
+-rw-r--r--   0        0        0     1562 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py
+-rw-r--r--   0        0        0     1709 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py
+-rw-r--r--   0        0        0     1891 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0     1192 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/utils.py
+-rw-r--r--   0        0        0    11050 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/write_sparameters.py
+-rw-r--r--   0        0        0     8567 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0        0 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/__init__.py
+-rw-r--r--   0        0        0     4262 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/add_simulation_markers.py
+-rw-r--r--   0        0        0     3276 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/convert_sparameters.py
+-rw-r--r--   0        0        0      251 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/disable_print.py
+-rw-r--r--   0        0        0     3407 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/get_effective_indices.py
+-rw-r--r--   0        0        0     2893 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/get_sparameters_path.py
+-rw-r--r--   0        0        0     5951 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/plot.py
+-rw-r--r--   0        0        0     2439 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/plot_csv.py
+-rw-r--r--   0        0        0      613 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/port_symmetries.py
+-rw-r--r--   0        0        0       32 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/Makefile
+-rw-r--r--   0        0        0       23 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/__init__.py
+-rw-r--r--   0        0        0      212 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/C.gds
+-rw-r--r--   0        0        0      220 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/C_width20.gds
+-rw-r--r--   0        0        0      218 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/C_width5.gds
+-rw-r--r--   0        0        0    14536 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_rx_dual_pol.gds
+-rw-r--r--   0        0        0    13550 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol.gds
+-rw-r--r--   0        0        0    13564 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds
+-rw-r--r--   0        0        0    13564 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds
+-rw-r--r--   0        0        0    10292 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_tx_dual_pol.gds
+-rw-r--r--   0        0        0     1498 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/crossing_arm.gds
+-rw-r--r--   0        0        0     7406 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/dbr_cavity.gds
+-rw-r--r--   0        0        0      440 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/die_bbox_frame.gds
+-rw-r--r--   0        0        0    27548 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/loss_deembedding_ch14_23.gds
+-rw-r--r--   0        0        0      872 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/pad_array_add_fiducials.gds
+-rw-r--r--   0        0        0    39252 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds
+-rw-r--r--   0        0        0      182 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/wg.gds
+-rw-r--r--   0        0        0     8606 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/main.py
+-rw-r--r--   0        0        0     1942 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/middleware.py
+-rwxr-xr-x   0        0        0     7445 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/server.py
+-rwxr-xr-x   0        0        0      636 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/server_jupyter.py
+-rw-r--r--   0        0        0     1299 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/static/client.css
+-rw-r--r--   0        0        0     9598 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/static/client.js
+-rw-r--r--   0        0        0      840 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/client.html.j2
+-rw-r--r--   0        0        0      481 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/file_browser.html.j2
+-rw-r--r--   0        0        0     1999 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/filewatcher.html.j2
+-rw-r--r--   0        0        0      236 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/footer.html.j2
+-rw-r--r--   0        0        0      242 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/gds_history.html.j2
+-rw-r--r--   0        0        0      578 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/header.html.j2
+-rw-r--r--   0        0        0      376 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/index.html.j2
+-rw-r--r--   0        0        0      995 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/navbar.html.j2
+-rw-r--r--   0        0        0      272 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/pdk.html.j2
+-rw-r--r--   0        0        0     1871 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/viewer.html.j2
+-rw-r--r--   0        0        0       87 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/widget/__init__.py
+-rw-r--r--   0        0        0    14936 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/widget/interactive.py
+-rw-r--r--   0        0        0     3174 2023-08-06 18:26:48.079156 gplugins-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4987 1970-01-01 00:00:00.000000 gplugins-0.1.0/PKG-INFO
```

### Comparing `gplugins-0.0.3/LICENSE` & `gplugins-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/README.md` & `gplugins-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gplugins 0.0.3
+# gplugins 0.1.0
 
 [![docs](https://github.com/gdsfactory/gplugins/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gplugins/)
 [![PyPI](https://img.shields.io/pypi/v/gplugins)](https://pypi.org/project/gplugins/)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gplugins.svg)](https://pypi.python.org/pypi/gplugins)
 [![MIT](https://img.shields.io/github/license/gdsfactory/gplugins)](https://choosealicense.com/licenses/mit/)
 [![codecov](https://img.shields.io/codecov/c/github/gdsfactory/gplugins)](https://codecov.io/gh/gdsfactory/gdsfactory/tree/main/gplugins)
 
@@ -27,15 +27,15 @@
 
 You can install all plugins with:
 
 ```
 pip install "gplugins[database,devsim,femwell,gmsh,schematic,meow,meshwell,ray,sax,tidy3d]" --upgrade
 ```
 
-Or Install only the plugins you need `pip install gplugins[database,devsim]` from the available plugins:
+Or Install only the plugins you need `pip install gplugins[schematic,femwell,meow,sax,tidy3d]` from the available plugins:
 
 Separate installation (not using pip):
 
 - For Meep and MPB you need to use `conda` or `mamba` on MacOS, Linux or [Windows WSL (Windows Subsystem for Linux)](https://learn.microsoft.com/en-us/windows/wsl/install) with `conda install pymeep=*=mpi_mpich_* -c conda-forge -y`
 
 ## Getting started
```

### Comparing `gplugins-0.0.3/gplugins/config.py` & `gplugins-0.1.0/gplugins/config.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/dagster/workflow.py` & `gplugins-0.1.0/gplugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/database/README.md` & `gplugins-0.1.0/gplugins/database/README.md`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/database/db_upload.py` & `gplugins-0.1.0/gplugins/database/db_upload.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/database/models.py` & `gplugins-0.1.0/gplugins/database/models.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/devsim/__init__.py` & `gplugins-0.1.0/gplugins/devsim/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/devsim/doping.py` & `gplugins-0.1.0/gplugins/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/devsim/get_simulation.py` & `gplugins-0.1.0/gplugins/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/devsim/get_simulation_xsection.py` & `gplugins-0.1.0/gplugins/devsim/get_simulation_xsection.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,172 +517,15 @@
             cache: True uses file cache from PDK.modes_path. False skips cache.
             precision: single or double.
 
         Returns:
             A tidy3d Waveguide object.
 
         """
-        if perturb:
-            # Create temporary Waveguide to get the X, Y, Z positions
-            temp_Waveguide = Waveguide(
-                wavelength=wavelength,
-                core_width=self.core_width / um,
-                core_thickness=self.core_thickness / um,
-                slab_thickness=self.slab_thickness / um,
-                box_thickness=box_thickness,
-                clad_thickness=clad_thickness,
-                side_margin=max(
-                    self.ppp_offset + self.xmargin, self.npp_offset + self.xmargin
-                )
-                / um,
-                grid_resolution=grid_resolution,
-                precision=precision,
-                core_material=core_material,
-                clad_material=clad_material,
-                cache=False,
-            )
-
-            # Create index perturbation
-            x_fem = []
-            y_fem = []
-            dN_fem = []
-            dP_fem = []
-
-            mat_dtype = np.float64 if precision == "double" else np.float32
-
-            for region_name in ["core", "slab"]:
-                x_fem.append(
-                    np.array(self.get_field(region_name=region_name, field_name="x"))
-                )
-                y_fem.append(
-                    np.array(self.get_field(region_name=region_name, field_name="y"))
-                )
-                dN_fem.append(
-                    np.array(
-                        self.get_field(region_name=region_name, field_name="Electrons"),
-                        dtype=mat_dtype,
-                    )
-                )
-                dP_fem.append(
-                    np.array(
-                        self.get_field(region_name=region_name, field_name="Holes"),
-                        dtype=mat_dtype,
-                    )
-                )
-
-            x_fem = np.concatenate(x_fem)
-            y_fem = np.concatenate(y_fem)
-            dN_fem = np.concatenate(dN_fem)
-            dP_fem = np.concatenate(dP_fem)
-
-            dn_fem = dn_carriers(wavelength, dN_fem, dP_fem)
-            dk_fem = alpha_to_k(dalpha_carriers(wavelength, dN_fem, dP_fem), wavelength)
-
-            # Interpolate the index perturbation onto the Waveguide grid
-            temp_grid = temp_Waveguide.waveguide.mode_solver.simulation.grid
-            X = temp_grid.centers.x
-            Y = temp_grid.centers.y
-            Z = temp_grid.centers.z
-
-            freq0 = td.C_0 / wavelength
-            freqs = [freq0]
-
-            x_mesh, y_mesh, z_mesh, freq_mesh = np.meshgrid(
-                X, Y, Z, freqs, indexing="ij"
-            )
-            x_mesh_2D = x_mesh[:, :, 0, 0]
-            y_mesh_2D = y_mesh[:, :, 0, 0]
-
-            dn_grid = np.nan_to_num(
-                griddata(
-                    (x_fem * cm / um, y_fem * cm / um),
-                    dn_fem,
-                    (x_mesh_2D, y_mesh_2D),
-                    DEVSIM_INTERPOLATION_METHOD,
-                )
-            )
-            dk_grid = np.nan_to_num(
-                griddata(
-                    (x_fem * cm / um, y_fem * cm / um),
-                    dk_fem,
-                    (x_mesh_2D, y_mesh_2D),
-                    DEVSIM_INTERPOLATION_METHOD,
-                )
-            )
-
-            # Extend to 3D (Nx, Ny,) -> (Nx, Ny, Nz,)
-            dn_grid_3D = np.stack([dn_grid] * Z.size, axis=-1)
-            dk_grid_3D = np.stack([dk_grid] * Z.size, axis=-1)
-
-            # Extend to 4D (Nx, Ny, Nz,) -> (Nx, Ny, Nz, Nf)
-            dn_grid_td = np.stack([dn_grid_3D] * len(freqs), axis=-1)
-            dk_grid_td = np.stack([dk_grid_3D] * len(freqs), axis=-1)
-
-            n_core, k_core = get_nk(core_material)
-            n_dataset = td.ScalarFieldDataArray(
-                n_core + dn_grid_td, coords=dict(x=X, y=Y, z=Z, f=freqs)
-            )
-            k_dataset = td.ScalarFieldDataArray(
-                k_core + dk_grid_td, coords=dict(x=X, y=Y, z=Z, f=freqs)
-            )
-
-            # core_material_pertub = td.CustomMedium.from_nk(
-            #     n=n_dataset,
-            #     k=k_dataset,
-            #     interp_method="linear",
-            # )
-            if isinstance(core_material, str):
-                name_material = core_material + "_with_carriers"
-            else:
-                name_material = "core_material_with_carriers"
-
-            eps_real = n_dataset**2 - k_dataset**2
-            eps_imag = 2 * n_dataset * k_dataset
-            eps_diag_data = td.ScalarFieldDataArray(
-                eps_real + 1.0j * eps_imag, coords=dict(x=X, y=Y, z=Z, f=freqs)
-            )
-
-            eps_perturb = td.PermittivityDataset(
-                eps_xx=eps_diag_data, eps_yy=eps_diag_data, eps_zz=eps_diag_data
-            )
-            core_material_pertub = td.CustomMedium(
-                name=name_material,
-                eps_dataset=eps_perturb,
-                frequency_range=[0.99 * freq0, 1.01 * freq0],
-            )
-
-            # dn_dict = (
-            #     {
-            #         "x": x_fem * cm / um,
-            #         "y": y_fem * cm / um + box_thickness,
-            #         "dn": dn_fem + 1j * dk_fem,
-            #     }
-            #     if perturb
-            #     else None
-            # )
-
-            # Create perturbed waveguide, handle like regular mode
-            return Waveguide(
-                wavelength=wavelength,
-                core_width=self.core_width / um,
-                core_thickness=self.core_thickness / um,
-                slab_thickness=self.slab_thickness / um,
-                box_thickness=box_thickness,
-                clad_thickness=clad_thickness,
-                side_margin=max(
-                    self.ppp_offset + self.xmargin, self.npp_offset + self.xmargin
-                )
-                / um,
-                grid_resolution=grid_resolution,
-                precision=precision,
-                core_material=core_material_pertub,
-                clad_material=clad_material,
-                cache=cache,
-            )
-        else:
+        if not perturb:
             # Create simple waveguide, handle like regular mode
             return Waveguide(
                 wavelength=wavelength,
                 core_width=self.core_width / um,
                 core_thickness=self.core_thickness / um,
                 slab_thickness=self.slab_thickness / um,
                 box_thickness=box_thickness,
@@ -693,14 +536,168 @@
                 / um,
                 grid_resolution=grid_resolution,
                 precision=precision,
                 core_material=core_material,
                 clad_material=clad_material,
                 cache=cache,
             )
+        # Create temporary Waveguide to get the X, Y, Z positions
+        temp_Waveguide = Waveguide(
+            wavelength=wavelength,
+            core_width=self.core_width / um,
+            core_thickness=self.core_thickness / um,
+            slab_thickness=self.slab_thickness / um,
+            box_thickness=box_thickness,
+            clad_thickness=clad_thickness,
+            side_margin=max(
+                self.ppp_offset + self.xmargin, self.npp_offset + self.xmargin
+            )
+            / um,
+            grid_resolution=grid_resolution,
+            precision=precision,
+            core_material=core_material,
+            clad_material=clad_material,
+            cache=False,
+        )
+
+        # Create index perturbation
+        x_fem = []
+        y_fem = []
+        dN_fem = []
+        dP_fem = []
+
+        mat_dtype = np.float64 if precision == "double" else np.float32
+
+        for region_name in ["core", "slab"]:
+            x_fem.append(
+                np.array(self.get_field(region_name=region_name, field_name="x"))
+            )
+            y_fem.append(
+                np.array(self.get_field(region_name=region_name, field_name="y"))
+            )
+            dN_fem.append(
+                np.array(
+                    self.get_field(region_name=region_name, field_name="Electrons"),
+                    dtype=mat_dtype,
+                )
+            )
+            dP_fem.append(
+                np.array(
+                    self.get_field(region_name=region_name, field_name="Holes"),
+                    dtype=mat_dtype,
+                )
+            )
+
+        x_fem = np.concatenate(x_fem)
+        y_fem = np.concatenate(y_fem)
+        dN_fem = np.concatenate(dN_fem)
+        dP_fem = np.concatenate(dP_fem)
+
+        dn_fem = dn_carriers(wavelength, dN_fem, dP_fem)
+        dk_fem = alpha_to_k(dalpha_carriers(wavelength, dN_fem, dP_fem), wavelength)
+
+        # Interpolate the index perturbation onto the Waveguide grid
+        temp_grid = temp_Waveguide.waveguide.mode_solver.simulation.grid
+        X = temp_grid.centers.x
+        Y = temp_grid.centers.y
+        Z = temp_grid.centers.z
+
+        freq0 = td.C_0 / wavelength
+        freqs = [freq0]
+
+        x_mesh, y_mesh, z_mesh, freq_mesh = np.meshgrid(X, Y, Z, freqs, indexing="ij")
+        x_mesh_2D = x_mesh[:, :, 0, 0]
+        y_mesh_2D = y_mesh[:, :, 0, 0]
+
+        dn_grid = np.nan_to_num(
+            griddata(
+                (x_fem * cm / um, y_fem * cm / um),
+                dn_fem,
+                (x_mesh_2D, y_mesh_2D),
+                DEVSIM_INTERPOLATION_METHOD,
+            )
+        )
+        dk_grid = np.nan_to_num(
+            griddata(
+                (x_fem * cm / um, y_fem * cm / um),
+                dk_fem,
+                (x_mesh_2D, y_mesh_2D),
+                DEVSIM_INTERPOLATION_METHOD,
+            )
+        )
+
+        # Extend to 3D (Nx, Ny,) -> (Nx, Ny, Nz,)
+        dn_grid_3D = np.stack([dn_grid] * Z.size, axis=-1)
+        dk_grid_3D = np.stack([dk_grid] * Z.size, axis=-1)
+
+        # Extend to 4D (Nx, Ny, Nz,) -> (Nx, Ny, Nz, Nf)
+        dn_grid_td = np.stack([dn_grid_3D] * len(freqs), axis=-1)
+        dk_grid_td = np.stack([dk_grid_3D] * len(freqs), axis=-1)
+
+        n_core, k_core = get_nk(core_material)
+        n_dataset = td.ScalarFieldDataArray(
+            n_core + dn_grid_td, coords=dict(x=X, y=Y, z=Z, f=freqs)
+        )
+        k_dataset = td.ScalarFieldDataArray(
+            k_core + dk_grid_td, coords=dict(x=X, y=Y, z=Z, f=freqs)
+        )
+
+        # core_material_pertub = td.CustomMedium.from_nk(
+        #     n=n_dataset,
+        #     k=k_dataset,
+        #     interp_method="linear",
+        # )
+        if isinstance(core_material, str):
+            name_material = f"{core_material}_with_carriers"
+        else:
+            name_material = "core_material_with_carriers"
+
+        eps_real = n_dataset**2 - k_dataset**2
+        eps_imag = 2 * n_dataset * k_dataset
+        eps_diag_data = td.ScalarFieldDataArray(
+            eps_real + 1.0j * eps_imag, coords=dict(x=X, y=Y, z=Z, f=freqs)
+        )
+
+        eps_perturb = td.PermittivityDataset(
+            eps_xx=eps_diag_data, eps_yy=eps_diag_data, eps_zz=eps_diag_data
+        )
+        core_material_pertub = td.CustomMedium(
+            name=name_material,
+            eps_dataset=eps_perturb,
+            frequency_range=[0.99 * freq0, 1.01 * freq0],
+        )
+
+        # dn_dict = (
+        #     {
+        #         "x": x_fem * cm / um,
+        #         "y": y_fem * cm / um + box_thickness,
+        #         "dn": dn_fem + 1j * dk_fem,
+        #     }
+        #     if perturb
+        #     else None
+        # )
+
+        # Create perturbed waveguide, handle like regular mode
+        return Waveguide(
+            wavelength=wavelength,
+            core_width=self.core_width / um,
+            core_thickness=self.core_thickness / um,
+            slab_thickness=self.slab_thickness / um,
+            box_thickness=box_thickness,
+            clad_thickness=clad_thickness,
+            side_margin=max(
+                self.ppp_offset + self.xmargin, self.npp_offset + self.xmargin
+            )
+            / um,
+            grid_resolution=grid_resolution,
+            precision=precision,
+            core_material=core_material_pertub,
+            clad_material=clad_material,
+            cache=cache,
+        )
 
 
 def clear_devsim_cache() -> None:
     try:
         devsim.delete_mesh(mesh="dio")
     except devsim.error:
         warnings.warn("No mesh to delete.")
```

### Comparing `gplugins-0.0.3/gplugins/devsim/get_solver.py` & `gplugins-0.1.0/gplugins/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/devsim/test_devsim.py` & `gplugins-0.1.0/gplugins/devsim/test_devsim.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/femwell/mode_solver.py` & `gplugins-0.1.0/gplugins/femwell/mode_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,26 +145,24 @@
                 get_material_index(layer.material, wavelength) ** 2
             )
         if "background_tag" in kwargs:
             epsilon[basis0.get_dofs(elements=kwargs["background_tag"])] = (
                 get_material_index(kwargs["background_tag"], wavelength) ** 2
             )
 
-    # Mode solve
-    modes = compute_modes(
+    return compute_modes(
         basis0,
         epsilon,
         wavelength=wavelength,
         mu_r=1,
         num_modes=num_modes,
         order=order,
         radius=radius,
         solver=solver,
     )
-    return modes
 
 
 if __name__ == "__main__":
     import matplotlib.pyplot as plt
 
     PDK = gf.get_generic_pdk()
     PDK.activate()
```

### Comparing `gplugins-0.0.3/gplugins/femwell/solve_thermal.py` & `gplugins-0.1.0/gplugins/femwell/solve_thermal.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/femwell/test_mode_solver.py` & `gplugins-0.1.0/gplugins/femwell/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/__init__.py` & `gplugins-0.1.0/gplugins/gmeep/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/async_utils.py` & `gplugins-0.1.0/gplugins/gmeep/async_utils.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/get_material.py` & `gplugins-0.1.0/gplugins/gmeep/get_material.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/get_meep_geometry.py` & `gplugins-0.1.0/gplugins/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/get_port_eigenmode.py` & `gplugins-0.1.0/gplugins/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/get_simulation.py` & `gplugins-0.1.0/gplugins/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/get_simulation_grating_farfield.py` & `gplugins-0.1.0/gplugins/gmeep/get_simulation_grating_farfield.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/get_simulation_grating_fiber.py` & `gplugins-0.1.0/gplugins/gmeep/get_simulation_grating_fiber.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/meep_adjoint_optimization.py` & `gplugins-0.1.0/gplugins/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_eigenmode.py` & `gplugins-0.1.0/gplugins/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_materials.py` & `gplugins-0.1.0/gplugins/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gplugins-0.1.0/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gplugins-0.1.0/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep.py` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/write_sparameters_grating.py` & `gplugins-0.1.0/gplugins/gmeep/write_sparameters_grating.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
 
     # Write execution file
     script_lines = [
         "from gplugins.gmeep.write_sparameters_grating import write_sparameters_grating\n\n",
         'if __name__ == "__main__":\n\n',
         "\twrite_sparameters_grating(\n",
     ]
-    script_lines.extend(f"\t\t{key} = {instance[key]!r},\n" for key in instance.keys())
+    script_lines.extend(f"\t\t{key} = {instance[key]!r},\n" for key in instance)
     script_lines.append("\t)")
     script_file = filepath.with_suffix(".py")
     with open(script_file, "w") as script_file_obj:
         script_file_obj.writelines(script_lines)
     # Exec string
     command = f"mpirun -np {cores} {_python()} {script_file}"
```

### Comparing `gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep.py` & `gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep_batch.py` & `gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep_batch.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep_mpi.py` & `gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep_mpi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/__init__.py` & `gplugins-0.1.0/gplugins/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/break_geometry.py` & `gplugins-0.1.0/gplugins/gmsh/break_geometry.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/mesh.py` & `gplugins-0.1.0/gplugins/gmsh/mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/meshtracker.py` & `gplugins-0.1.0/gplugins/gmsh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/parse_component.py` & `gplugins-0.1.0/gplugins/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/parse_gds.py` & `gplugins-0.1.0/gplugins/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/parse_layerstack.py` & `gplugins-0.1.0/gplugins/gmsh/parse_layerstack.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/refine.py` & `gplugins-0.1.0/gplugins/gmsh/refine.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/scratch/mesh3D.py` & `gplugins-0.1.0/gplugins/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/tests/test_meshing.py` & `gplugins-0.1.0/gplugins/gmsh/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/uz_xsection_mesh.py` & `gplugins-0.1.0/gplugins/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/xy_xsection_mesh.py` & `gplugins-0.1.0/gplugins/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/gmsh/xyz_mesh.py` & `gplugins-0.1.0/gplugins/gmsh/xyz_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,29 +170,26 @@
 
     resolutions = copy.deepcopy(resolutions)
 
     if resolutions:
         for r in resolutions.values():
             r["resolution"] *= global_scaling_premesh
 
-    # Mesh
-    mesh_out = model.mesh(
+    return model.mesh(
         entities_dict=prisms_dict,
         resolutions=resolutions,
         default_characteristic_length=default_characteristic_length,
         global_scaling=global_scaling,
         global_2D_algorithm=global_2D_algorithm,
         global_3D_algorithm=global_3D_algorithm,
         gmsh_version=gmsh_version,
         filename=filename,
         verbosity=verbosity,
     )
 
-    return mesh_out
-
 
 if __name__ == "__main__":
     import gdsfactory as gf
     from gdsfactory.generic_tech import LAYER
     from gdsfactory.pdk import get_layer_stack
 
     # Choose some component
```

### Comparing `gplugins-0.0.3/gplugins/lumerical/__init__.py` & `gplugins-0.1.0/gplugins/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/lumerical/interconnect.py` & `gplugins-0.1.0/gplugins/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/lumerical/read.py` & `gplugins-0.1.0/gplugins/lumerical/read.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/lumerical/settings.py` & `gplugins-0.1.0/gplugins/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/lumerical/tests/test_lumerical_read_sparameters.py` & `gplugins-0.1.0/gplugins/lumerical/tests/test_lumerical_read_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/lumerical/write_sparameters_lumerical.py` & `gplugins-0.1.0/gplugins/lumerical/write_sparameters_lumerical.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     layer_stack = layer_stack or get_layer_stack()
 
     layer_to_thickness = layer_stack.get_layer_to_thickness()
     layer_to_zmin = layer_stack.get_layer_to_zmin()
     layer_to_material = layer_stack.get_layer_to_material()
 
     if hasattr(component.info, "simulation_settings"):
-        sim_settings.update(component.info.simulation_settings)
+        sim_settings |= component.info.simulation_settings
         logger.info(
             f"Updating {component.name!r} sim settings {component.simulation_settings}"
         )
     for setting in settings:
         if setting not in sim_settings:
             raise ValueError(
                 f"Invalid setting {setting!r} not in ({list(sim_settings.keys())})"
```

### Comparing `gplugins-0.0.3/gplugins/lumerical/write_sparameters_lumerical_components.py` & `gplugins-0.1.0/gplugins/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/meow/meow_eme.py` & `gplugins-0.1.0/gplugins/meow/meow_eme.py`

 * *Files identical despite different names*

```diff
@@ -297,15 +297,15 @@
             cell_length: in um.
         """
         zs = np.linspace(self.z_min, self.z_max, self.num_cells - 1)
 
         # add two cells without length:
         zs = np.concatenate([[self.z_min], zs, [self.z_max]])
 
-        mesh = mw.Mesh2d(
+        mesh = mw.Mesh2D(
             x=np.linspace(
                 self.center_x - self.span_x / 2,
                 self.center_x + self.span_x / 2,
                 self.resolution_x,
             ),
             y=np.linspace(
                 self.center_y - self.span_y / 2,
```

### Comparing `gplugins-0.0.3/gplugins/meow/test_meow_simulation.py` & `gplugins-0.1.0/gplugins/meow/test_meow_simulation.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,18 +32,22 @@
 
     for key in sp.keys():
         if key == "wavelengths":
             continue
         entry1, entry2 = key.split(",")
         port1, mode1 = entry1.split("@")
         port2, mode2 = entry2.split("@")
+
+        # Transmission larger than 90%
         if port1 != port2 and mode1 == "0" and mode2 == "0":
-            assert np.abs(sp[key]) ** 2 > 0.9
-        elif port1 != port2 and mode1 == "1" and mode2 == "1":
-            assert np.abs(sp[key]) ** 2 > 0.2
+            assert np.abs(sp[key]) ** 2 > 0.90
+
+    # Reflection smaller than 5%
+    assert abs(sp["o1@0,o1@0"]) < 0.05
+    assert abs(sp["o2@0,o2@0"]) < 0.05
 
 
 def test_cells() -> None:
     layerstack = LayerStack(
         layers={
             k: get_layer_stack().layers[k]
             for k in (
@@ -62,8 +66,27 @@
     c = gf.components.taper(length=1, width2=2)
     m = MEOW(component=c, layerstack=layerstack, wavelength=1.55, cell_length=1)
     assert len(m.cells) == 4, len(m.cells)
 
 
 if __name__ == "__main__":
     # test_cells()
-    test_meow_defaults()
+    # test_meow_defaults()
+    c = gf.components.taper_cross_section_linear()
+    filtered_layerstack = LayerStack(
+        layers={
+            k: get_layer_stack().layers[k]
+            for k in (
+                "slab90",
+                "core",
+                "box",
+                "clad",
+            )
+        }
+    )
+
+    sp = MEOW(
+        component=c,
+        layerstack=filtered_layerstack,
+        wavelength=1.55,
+        overwrite=True,
+    ).compute_sparameters()
```

### Comparing `gplugins-0.0.3/gplugins/modes/__init__.py` & `gplugins-0.1.0/gplugins/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/coupler.py` & `gplugins-0.1.0/gplugins/modes/coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/find_coupling_vs_gap.py` & `gplugins-0.1.0/gplugins/modes/find_coupling_vs_gap.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/find_mode_dispersion.py` & `gplugins-0.1.0/gplugins/modes/find_mode_dispersion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/find_modes.py` & `gplugins-0.1.0/gplugins/modes/find_modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/find_modes_cross_section.py` & `gplugins-0.1.0/gplugins/modes/find_modes_cross_section.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/find_neff_ng_dw_dh.py` & `gplugins-0.1.0/gplugins/modes/find_neff_ng_dw_dh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/find_neff_vs_width.py` & `gplugins-0.1.0/gplugins/modes/find_neff_vs_width.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/get_mode_solver_coupler.py` & `gplugins-0.1.0/gplugins/modes/get_mode_solver_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/get_mode_solver_cross_section.py` & `gplugins-0.1.0/gplugins/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/get_mode_solver_rib.py` & `gplugins-0.1.0/gplugins/modes/get_mode_solver_rib.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_nitride.csv` & `gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_rib.csv` & `gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_strip.csv` & `gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/neff_convergence_test.py` & `gplugins-0.1.0/gplugins/modes/neff_convergence_test.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/overlap.py` & `gplugins-0.1.0/gplugins/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gplugins-0.1.0/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/tests/test_find_modes.py` & `gplugins-0.1.0/gplugins/modes/tests/test_find_modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/tests/test_find_modes_dispersion.py` & `gplugins-0.1.0/gplugins/modes/tests/test_find_modes_dispersion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/modes/types.py` & `gplugins-0.1.0/gplugins/modes/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from collections.abc import Callable
-from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from gdsfactory.typings import Array
 from meep import mpb
 from pydantic import BaseModel
 from scipy.interpolate import RectBivariateSpline
@@ -461,15 +460,15 @@
 class WavelengthSweep(BaseModel):
     wavelength: list[float]
     neff: dict[int, list[float]]
     ng: dict[int, list[float]]
 
 
 ModeSolverFactory = Callable[..., mpb.ModeSolver]
-ModeSolverOrFactory = Union[mpb.ModeSolver, ModeSolverFactory]
+ModeSolverOrFactory = mpb.ModeSolver | ModeSolverFactory
 
 
 if __name__ == "__main__":
     import gplugins.modes as gm
 
     m = gm.find_modes_waveguide()
     # m[1].plot_e_all(operation=np.abs)
```

### Comparing `gplugins-0.0.3/gplugins/modes/waveguide.py` & `gplugins-0.1.0/gplugins/modes/waveguide.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/path_length_analysis/path_length_analysis.py` & `gplugins-0.1.0/gplugins/path_length_analysis/path_length_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,15 @@
         return None
 
 
 def _get_link_name(component: Component):
     ports = sorted(component.ports.keys())
     if len(ports) != 2:
         raise ValueError("routing components must have two ports")
-    link = ":".join(ports)
-    return link
+    return ":".join(ports)
 
 
 def _node_to_inst_port(node: str):
     ip = node.split(",")
     if len(ip) == 2:
         inst, port = ip
     elif len(ip) == 1:
@@ -66,15 +65,15 @@
         raise ValueError(
             f"did not expect a connection name with more than one comma: {node}"
         )
     return inst, port
 
 
 def _is_scalar(val):
-    return isinstance(val, float) or isinstance(val, int)
+    return isinstance(val, float | int)
 
 
 def _expand_bbox(bbox):
     if len(bbox) == 2:
         bbox = [bbox[0], (bbox[0][0], bbox[1][1]), bbox[1], (bbox[1][0], bbox[0][1])]
     return bbox
 
@@ -171,28 +170,25 @@
                         continue
                     edges = pathlength_graph.edges(nbunch=path, data=True)
                     edge_data = [e[2] for e in edges if e[2]]
                     summed_route_attrs = sum_route_attrs(edge_data)
                     if "weight" in summed_route_attrs:
                         summed_route_attrs.pop("weight")
                     if summed_route_attrs:
-                        record.update(summed_route_attrs)
+                        record |= summed_route_attrs
                         route_records.append(record)
                     record["edges"] = edges
                     record["nodes"] = path
     return route_records
 
 
 def _get_subinst_node_name(node_name, inst_name):
-    if "," in node_name:
-        new_node_name = f"{inst_name}.{node_name}"
-    else:
-        # for top-level ports
-        new_node_name = f"{inst_name},{node_name}"
-    return new_node_name
+    return (
+        f"{inst_name}.{node_name}" if "," in node_name else f"{inst_name},{node_name}"
+    )
 
 
 def idealized_mxn_connectivity(inst_name: str, ref: ComponentReference, g: nx.Graph):
     """
     Connects all input ports to all output ports of m x n components, with idealized routes
 
     Args:
@@ -266,16 +262,16 @@
                 sub_graph = _get_edge_based_route_attr_graph(
                     sub_inst.parent,
                     recursive=True,
                     component_connectivity=component_connectivity,
                     netlist=sub_netlist,
                     netlists=netlists,
                 )
-                sub_edges = []
                 sub_nodes = []
+                sub_edges = []
                 for edge in sub_graph.edges(data=True):
                     s, e, d = edge
                     new_edge = []
                     for node_name in [s, e]:
                         new_node_name = _get_subinst_node_name(node_name, inst_name)
                         new_edge.append(new_node_name)
                     new_edge.append(d)
@@ -293,21 +289,20 @@
                     )
                     d["x"] = new_pt[0]
                     d["y"] = new_pt[1]
                     new_node = (new_name, d)
                     sub_nodes.append(new_node)
                 g.add_nodes_from(sub_nodes)
                 g.add_edges_from(sub_edges)
+            elif component_connectivity:
+                component_connectivity(inst_name, sub_inst, g)
             else:
-                if component_connectivity:
-                    component_connectivity(inst_name, sub_inst, g)
-                else:
-                    warnings.warn(
-                        f"ignoring any links in {inst_name} ({sub_inst.parent.name})"
-                    )
+                warnings.warn(
+                    f"ignoring any links in {inst_name} ({sub_inst.parent.name})"
+                )
 
     # connect all top level ports
     if top_level_ports:
         edges = []
         for port, sub_port in top_level_ports.items():
             p_attrs = dict(node_attrs[sub_port])
             e_attrs = {"weight": 0.0001}
@@ -337,18 +332,21 @@
     if recursive:
         netlists = get_netlist_recursive(pic, component_suffix="", full_settings=True)
         netlist = netlists[pic.name]
     else:
         netlist = get_netlist(pic, full_settings=True)
         netlists = None
 
-    graph = _get_edge_based_route_attr_graph(
-        pic, recursive, component_connectivity, netlist=netlist, netlists=netlists
+    return _get_edge_based_route_attr_graph(
+        pic,
+        recursive,
+        component_connectivity,
+        netlist=netlist,
+        netlists=netlists,
     )
-    return graph
 
 
 def get_pathlength_widgets(
     pic: Component,
     G: nx.Graph,
     paths: list[dict[str, Any]],
     cs_colors: dict[str, str] | None = None,
@@ -439,17 +437,17 @@
             for n in pp:
                 n_data = G.nodes[n]
                 xs.append(n_data["x"])
                 ys.append(n_data["y"])
             path_data["xs"].append(xs)
             path_data["ys"].append(ys)
             path_data["color"].append(Category10[10][i % 10])
-            for key in path_data:
+            for key, value in path_data.items():
                 if key not in ["xs", "ys", "color"]:
-                    path_data[key].append(path.get(key, 0.0))
+                    value.append(path.get(key, 0.0))
 
     inst_patches = {"xs": [], "ys": [], "names": [], "xl": [], "yt": []}
     for inst_name, inst_info in inst_infos.items():
         bbox = np.array(_expand_bbox(inst_info["bbox"]))
         xs = bbox[:, 0]
         ys = bbox[:, 1]
         inst_patches["xs"].append(xs)
@@ -483,16 +481,17 @@
         TableColumn(field="color", title="Key", formatter=formatter, width=2),
         TableColumn(field="src_inst", title="Source"),
         TableColumn(field="src_port", title="Port"),
         TableColumn(field="dst_inst", title="Dest"),
         TableColumn(field="dst_port", title="Port"),
         TableColumn(field="length", title="Length"),
     ]
-    for cs_name in cs_colors:
-        columns.append(TableColumn(field=f"{cs_name}_length", title=cs_name))
+    columns.extend(
+        TableColumn(field=f"{cs_name}_length", title=cs_name) for cs_name in cs_colors
+    )
     columns.append(TableColumn(field="n_bend_90", title="# bend90"))
     table = DataTable(
         source=paths_ds,
         columns=columns,
         sizing_mode="stretch_height",
         selectable="checkbox",
     )
```

### Comparing `gplugins-0.0.3/gplugins/path_length_analysis/test_pathlength_extraction.py` & `gplugins-0.1.0/gplugins/path_length_analysis/test_pathlength_extraction.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/photonic_circuit_models/__init__.py` & `gplugins-0.1.0/gplugins/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/photonic_circuit_models/coupler.py` & `gplugins-0.1.0/gplugins/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/photonic_circuit_models/mzi.py` & `gplugins-0.1.0/gplugins/photonic_circuit_models/mzi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/photonic_circuit_models/ring.py` & `gplugins-0.1.0/gplugins/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/process/diffusion.py` & `gplugins-0.1.0/gplugins/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/process/implant_tables.py` & `gplugins-0.1.0/gplugins/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/process/pysrim.py` & `gplugins-0.1.0/gplugins/process/pysrim.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 
 
 def fragment(step, total):
     remaining = total
     while remaining > 0:
         if step > remaining:
             return remaining
-        else:
-            remaining -= step
-            yield step
+        remaining -= step
+        yield step
 
 
 def find_folder(directory):
     for i in count():
         path = Path(directory) / str(i)
         if not path.is_dir():
             return str(path.absolute())
```

### Comparing `gplugins-0.0.3/gplugins/process/silicon.py` & `gplugins-0.1.0/gplugins/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/process/skew/antimony_si_skew.csv` & `gplugins-0.1.0/gplugins/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/process/skew/arsenic_si_skew.csv` & `gplugins-0.1.0/gplugins/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/process/skew/boron_si_skew.csv` & `gplugins-0.1.0/gplugins/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/process/skew/phosphorus_si_skew.csv` & `gplugins-0.1.0/gplugins/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/build_model.py` & `gplugins-0.1.0/gplugins/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/integrations/femwell_waveguide_model.py` & `gplugins-0.1.0/gplugins/sax/integrations/femwell_waveguide_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/integrations/meep_FDTD_model.py` & `gplugins-0.1.0/gplugins/sax/integrations/meep_FDTD_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         # Define function input given parameter values and transformed layerstack/component
         function_input = dict(
             input_component_file=input_component_file,
             cores=self.num_cpus_per_task,
             output_vector_labels=self.output_vector_labels,
         )
-        function_input.update(sim_settings)
+        function_input |= sim_settings
         # Assign the task to a worker
         return remote_function.remote(**function_input)
 
 
 if __name__ == "__main__":
     import gdsfactory as gf
     from gdsfactory.technology import LayerStack
```

### Comparing `gplugins-0.0.3/gplugins/sax/integrations/meow_eme_model.py` & `gplugins-0.1.0/gplugins/sax/integrations/meow_eme_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/interpolators.py` & `gplugins-0.1.0/gplugins/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/mlp.py` & `gplugins-0.1.0/gplugins/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/models.py` & `gplugins-0.1.0/gplugins/sax/models.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/parameter.py` & `gplugins-0.1.0/gplugins/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/plot_model.py` & `gplugins-0.1.0/gplugins/sax/plot_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,10 +70,11 @@
     ax.set_xlabel("wavelength (nm)")
     ax.set_ylabel(ylabel)
     plt.legend()
     return ax
 
 
 if __name__ == "__main__":
-    import sax
+    import gplugins.sax as gs
 
-    plot_model(sax.models.straight, phase=True, port1="in2")
+    plot_model(gs.models.straight, phase=True, port1="o1", ports2=("o1", "o2"))
+    plt.show()
```

### Comparing `gplugins-0.0.3/gplugins/sax/read.py` & `gplugins-0.1.0/gplugins/sax/read.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/tests/test_mzi.py` & `gplugins-0.1.0/gplugins/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/tests/test_mzi_lattice.py` & `gplugins-0.1.0/gplugins/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/sax/tests/test_parameters.py` & `gplugins-0.1.0/gplugins/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/schematic_editor/circuitviz.py` & `gplugins-0.1.0/gplugins/schematic_editor/circuitviz.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/schematic_editor/schematic_editor.py` & `gplugins-0.1.0/gplugins/schematic_editor/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/__init__.py` & `gplugins-0.1.0/gplugins/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/get_results.py` & `gplugins-0.1.0/gplugins/tidy3d/get_results.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/get_simulation.py` & `gplugins-0.1.0/gplugins/tidy3d/get_simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,26 +238,26 @@
     component_ref = component_padding.ref()
     component_ref.x = 0
     component_ref.y = 0
 
     material_name_to_tidy3d = material_name_to_tidy3d or {}
 
     if material_name_to_tidy3d:
-        clad_material_name_or_index = material_name_to_tidy3d[clad_material]
+        clad_material_spec = material_name_to_tidy3d[clad_material]
     else:
-        clad_material_name_or_index = (
+        clad_material_spec = (
             clad_material(wavelength) if callable(clad_material) else clad_material
         )
 
     clad = td.Structure(
         geometry=td.Box(
             size=(td.inf, td.inf, td.inf),
             center=(0, 0, 0),
         ),
-        medium=get_medium(name_or_index=clad_material_name_or_index),
+        medium=get_medium(spec=clad_material_spec),
     )
     structures = [clad]
 
     if len(layer_to_thickness) < 1:
         raise ValueError(f"{component.get_layers()} not in {layer_to_thickness.keys()}")
 
     t_core = max(layer_to_thickness.values())
@@ -277,19 +277,19 @@
         if layer in layer_to_material and layer in component_layers:
             zmin = layer_to_zmin[layer] if is_3d else 0
             zmax = zmin + thickness if is_3d else 0
 
             material_name = layer_to_material[layer]
 
             if material_name in material_name_to_tidy3d:
-                name_or_index = material_name_to_tidy3d[material_name]
-                medium = get_medium(name_or_index=name_or_index)
-                index = get_index(name_or_index=name_or_index)
+                spec = material_name_to_tidy3d[material_name]
+                medium = get_medium(spec=spec)
+                index = get_index(spec=spec)
                 logger.debug(
-                    f"Add {layer}, {name_or_index!r}, index = {index:.3f}, "
+                    f"Add {layer}, {spec!r}, index = {index:.3f}, "
                     f"thickness = {thickness}, zmin = {zmin}, zmax = {zmax}"
                 )
             else:
                 material_index = (
                     material_name(wavelength)
                     if callable(material_name)
                     else material_name
```

### Comparing `gplugins-0.0.3/gplugins/tidy3d/get_simulation_grating_coupler.py` & `gplugins-0.1.0/gplugins/tidy3d/get_simulation_grating_coupler.py`

 * *Files 4% similar despite different names*

```diff
@@ -298,70 +298,70 @@
         sim_xsize,
         sim_ysize,
         sim_zsize,
     ]
     material_name_to_tidy3d = material_name_to_tidy3d or {}
 
     if material_name_to_tidy3d:
-        clad_material_name_or_index = material_name_to_tidy3d[clad_material]
-        box_material_name_or_index = material_name_to_tidy3d[box_material]
-        substrate_material_name_or_index = material_name_to_tidy3d[substrate_material]
+        clad_material_spec = material_name_to_tidy3d[clad_material]
+        box_material_spec = material_name_to_tidy3d[box_material]
+        substrate_material_spec = material_name_to_tidy3d[substrate_material]
     else:
-        clad_material_name_or_index = (
+        clad_material_spec = (
             clad_material(wavelength) if callable(clad_material) else clad_material
         )
-        box_material_name_or_index = (
+        box_material_spec = (
             box_material(wavelength) if callable(box_material) else box_material
         )
-        substrate_material_name_or_index = (
+        substrate_material_spec = (
             substrate_material(wavelength)
             if callable(substrate_material)
             else substrate_material
         )
 
     clad = td.Structure(
         geometry=td.Box(
             size=(td.inf, td.inf, sim_zsize),
             center=(0, 0, sim_zsize / 2),
         ),
-        medium=get_medium(name_or_index=clad_material_name_or_index),
+        medium=get_medium(spec=clad_material_spec),
     )
     box = td.Structure(
         geometry=td.Box(
             size=(td.inf, td.inf, box_thickness),
             center=(0, 0, -box_thickness / 2),
         ),
-        medium=get_medium(name_or_index=box_material_name_or_index),
+        medium=get_medium(spec=box_material_spec),
     )
 
     substrate_thickness = 10
     substrate = td.Structure(
         geometry=td.Box(
             size=(td.inf, td.inf, substrate_thickness),
             center=(0, 0, -box_thickness - substrate_thickness / 2),
         ),
-        medium=get_medium(name_or_index=substrate_material_name_or_index),
+        medium=get_medium(spec=substrate_material_spec),
     )
 
     structures = [substrate, box, clad]
 
     component_layers = component_with_booleans.get_layers()
 
     for layer, thickness in layer_to_thickness.items():
         if layer in layer_to_material and layer in component_layers:
             zmin = layer_to_zmin[layer]
             zmax = zmin + thickness
             material_name = layer_to_material[layer]
 
             if material_name in material_name_to_tidy3d:
-                name_or_index = material_name_to_tidy3d[material_name]
-                medium = get_medium(name_or_index=name_or_index)
-                index = get_index(name_or_index=name_or_index)
+                spec = material_name_to_tidy3d[material_name]
+                medium = get_medium(spec=spec)
+                index = get_index(spec=spec)
                 logger.debug(
-                    f"Add {layer}, {name_or_index!r}, index = {index:.3f}, "
+                    f"Add {layer}, {spec!r}, index = {index:.3f}, "
                     f"thickness = {thickness}, zmin = {zmin}, zmax = {zmax}"
                 )
 
             else:
                 material_index = (
                     material_name(wavelength)
                     if callable(material_name)
```

### Comparing `gplugins-0.0.3/gplugins/tidy3d/modes.py` & `gplugins-0.1.0/gplugins/tidy3d/modes.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 from typing import Any, Literal
 
 import numpy as np
 import pydantic
 import tidy3d as td
 import xarray
 from gdsfactory.config import logger
-from gdsfactory.pdk import MaterialSpec, get_modes_path
+from gdsfactory.pdk import get_modes_path
 from gdsfactory.serialization import clean_value_name
 from gdsfactory.typings import PathType
 from tidy3d.plugins import waveguide
 from tqdm.auto import tqdm
 
-from gplugins.tidy3d.materials import get_medium
+from gplugins.tidy3d.materials import MaterialSpecTidy3d, get_medium
 
 Precision = Literal["single", "double"]
 nm = 1e-3
 
 
 class Waveguide(pydantic.BaseModel):
     """Waveguide Model.
@@ -43,14 +43,15 @@
         wavelength: wavelength in free space.
         core_width: waveguide core width.
         core_thickness: waveguide core thickness (height).
         core_material: core material. One of:
             - string: material name.
             - float: refractive index.
             - float, float: refractive index real and imaginary part.
+            - td.Medium: tidy3d medium.
             - function: function of wavelength.
         clad_material: top cladding material.
         box_material: bottom cladding material.
         slab_thickness: thickness of the slab region in a rib waveguide.
         clad_thickness: thickness of the top cladding.
         box_thickness: thickness of the bottom cladding.
         side_margin: domain extension to the side of the waveguide core.
@@ -103,17 +104,17 @@
                                v
         ________________________________________________
     """
 
     wavelength: float | Sequence[float] | Any
     core_width: float
     core_thickness: float
-    core_material: MaterialSpec | td.CustomMedium
-    clad_material: MaterialSpec
-    box_material: MaterialSpec | None = None
+    core_material: MaterialSpecTidy3d
+    clad_material: MaterialSpecTidy3d
+    box_material: MaterialSpecTidy3d | None = None
     slab_thickness: float = 0.0
     clad_thickness: float | None = None
     box_thickness: float | None = None
     side_margin: float | None = None
     sidewall_angle: float = 0.0
     sidewall_thickness: float = 0.0
     sidewall_k: float = 0.0
@@ -165,20 +166,31 @@
     @property
     def waveguide(self):
         """Tidy3D waveguide used by this instance."""
         # if (not hasattr(self, "_waveguide")
         #         or isinstance(self.core_material, td.CustomMedium)):
         if not hasattr(self, "_waveguide"):
             # To include a dn -> custom medium
-            if isinstance(self.core_material, td.CustomMedium):
+            if isinstance(self.core_material, td.CustomMedium | td.Medium):
                 core_medium = self.core_material
             else:
                 core_medium = get_medium(self.core_material)
-            clad_medium = get_medium(self.clad_material)
-            box_medium = get_medium(self.box_material) if self.box_material else None
+
+            if isinstance(self.clad_material, td.CustomMedium | td.Medium):
+                clad_medium = self.clad_material
+            else:
+                clad_medium = get_medium(self.clad_material)
+
+            if self.box_material:
+                if isinstance(self.box_material, td.CustomMedium | td.Medium):
+                    box_medium = self.box_material
+                else:
+                    box_medium = get_medium(self.box_material)
+            else:
+                box_medium = None
 
             freq0 = td.C_0 / np.mean(self.wavelength)
             n_core = core_medium.eps_model(freq0) ** 0.5
             n_clad = clad_medium.eps_model(freq0) ** 0.5
 
             sidewall_medium = (
                 td.Medium.from_nk(
@@ -961,26 +973,31 @@
     #     core_thickness=0.22,
     #     core_material="si",
     #     clad_material="sio2",
     #     num_modes=2,
     #     overwrite=True
     # )
 
+    import matplotlib.pyplot as plt
+
     strip = Waveguide(
         wavelength=1.55,
         core_width=1.0,
         slab_thickness=0.0,
-        core_material="si",
+        # core_material="si",
+        core_material=td.material_library["cSi"]["Li1993_293K"],
         clad_material="sio2",
         core_thickness=220 * nm,
         num_modes=4,
     )
-    w = np.linspace(400 * nm, 1000 * nm, 7)
-    n_eff = sweep_n_eff(strip, core_width=w)
-    fraction_te = sweep_fraction_te(strip, core_width=w)
+    strip.plot_index()
+    plt.show()
+    # w = np.linspace(400 * nm, 1000 * nm, 7)
+    # n_eff = sweep_n_eff(strip, core_width=w)
+    # fraction_te = sweep_fraction_te(strip, core_width=w)
 
     # t = np.linspace(0.2, 0.25, 6)
     # w = np.linspace(0.4, 0.6, 5)
     # n_eff = sweep_n_eff(wg, core_width=w, core_thickness=t)
 
     # fig, ax = pyplot.subplots(1, 2, tight_layout=True, figsize=(9, 4))
     # n_eff.sel(mode_index=0).real.plot(ax=ax[0])
```

### Comparing `gplugins-0.0.3/gplugins/tidy3d/tests/sim_ref.yaml` & `gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/tests/test_modes.py` & `gplugins-0.1.0/gplugins/tidy3d/tests/test_modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/tests/test_results.py` & `gplugins-0.1.0/gplugins/tidy3d/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/tests/test_simulation.py` & `gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py` & `gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py` & `gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/utils.py` & `gplugins-0.1.0/gplugins/tidy3d/utils.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/write_sparameters.py` & `gplugins-0.1.0/gplugins/tidy3d/write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/tidy3d/write_sparameters_grating_coupler.py` & `gplugins-0.1.0/gplugins/tidy3d/write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/utils/add_simulation_markers.py` & `gplugins-0.1.0/gplugins/utils/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/utils/convert_sparameters.py` & `gplugins-0.1.0/gplugins/utils/convert_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/utils/get_effective_indices.py` & `gplugins-0.1.0/gplugins/utils/get_effective_indices.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/utils/get_sparameters_path.py` & `gplugins-0.1.0/gplugins/utils/get_sparameters_path.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/utils/plot.py` & `gplugins-0.1.0/gplugins/utils/plot.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/utils/plot_csv.py` & `gplugins-0.1.0/gplugins/utils/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/utils/port_symmetries.py` & `gplugins-0.1.0/gplugins/utils/port_symmetries.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/coh_rx_dual_pol.gds` & `gplugins-0.1.0/gplugins/web/gds_files/coh_rx_dual_pol.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol.gds` & `gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds` & `gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds` & `gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/coh_tx_dual_pol.gds` & `gplugins-0.1.0/gplugins/web/gds_files/coh_tx_dual_pol.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/crossing_arm.gds` & `gplugins-0.1.0/gplugins/web/gds_files/crossing_arm.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/dbr_cavity.gds` & `gplugins-0.1.0/gplugins/web/gds_files/dbr_cavity.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/loss_deembedding_ch14_23.gds` & `gplugins-0.1.0/gplugins/web/gds_files/loss_deembedding_ch14_23.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/pad_array_add_fiducials.gds` & `gplugins-0.1.0/gplugins/web/gds_files/pad_array_add_fiducials.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds` & `gplugins-0.1.0/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/main.py` & `gplugins-0.1.0/gplugins/web/main.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/middleware.py` & `gplugins-0.1.0/gplugins/web/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,15 @@
         )
 
         source = dict(source)
         if upgrade:  # resolve conflict with priority of upgrade
             source[b"connection"] = b"upgrade"
 
         if b"x-forwarded-host" in source:
-            source.update({b"host": source[b"x-forwarded-host"]})
+            source[b"host"] = source[b"x-forwarded-host"]
             source.pop(b"x-forwarded-host")
 
         if b"x-forwarded-prefix" in source:
-            source.update({b"host": source[b"host"] + source[b"x-forwarded-prefix"]})
+            source[b"host"] = source[b"host"] + source[b"x-forwarded-prefix"]
             source.pop(b"x-forwarded-prefix")
 
-        source = [(k, v) for k, v in source.items()]
-
-        return source
+        return list(source.items())
```

### Comparing `gplugins-0.0.3/gplugins/web/server.py` & `gplugins-0.1.0/gplugins/web/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,34 +64,32 @@
     def mode_dump(self):
         return self.layout_view.mode_names()
 
     def annotation_dump(self):
         return [d[1] for d in self.layout_view.annotation_templates()]
 
     def layer_dump(self):
-        js = []
-        for layer in self.layout_view.each_layer():
-            js.append(
-                {
-                    "dp": layer.eff_dither_pattern(),
-                    "ls": layer.eff_line_style(),
-                    "c": layer.eff_fill_color(),
-                    "fc": layer.eff_frame_color(),
-                    "m": layer.marked,
-                    "s": layer.source,
-                    "t": layer.transparent,
-                    "va": layer.valid,
-                    "v": layer.visible,
-                    "w": layer.width,
-                    "x": layer.xfill,
-                    "name": layer.name,
-                    "id": layer.id(),
-                }
-            )
-        return js
+        return [
+            {
+                "dp": layer.eff_dither_pattern(),
+                "ls": layer.eff_line_style(),
+                "c": layer.eff_fill_color(),
+                "fc": layer.eff_frame_color(),
+                "m": layer.marked,
+                "s": layer.source,
+                "t": layer.transparent,
+                "va": layer.valid,
+                "v": layer.visible,
+                "w": layer.width,
+                "x": layer.xfill,
+                "name": layer.name,
+                "id": layer.id(),
+            }
+            for layer in self.layout_view.each_layer()
+        ]
 
     async def connection(self, websocket: WebSocket, path: str | None = None) -> None:
         self.layout_view = lay.LayoutView()
         url = self.url
         self.layout_view.load_layout(url)
         if self.layer_props is not None:
             self.layout_view.load_layer_props(str(self.layer_props))
```

### Comparing `gplugins-0.0.3/gplugins/web/server_jupyter.py` & `gplugins-0.1.0/gplugins/web/server_jupyter.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/static/client.css` & `gplugins-0.1.0/gplugins/web/static/client.css`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/static/client.js` & `gplugins-0.1.0/gplugins/web/static/client.js`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/templates/client.html.j2` & `gplugins-0.1.0/gplugins/web/templates/client.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/templates/filewatcher.html.j2` & `gplugins-0.1.0/gplugins/web/templates/filewatcher.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/templates/header.html.j2` & `gplugins-0.1.0/gplugins/web/templates/header.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/templates/navbar.html.j2` & `gplugins-0.1.0/gplugins/web/templates/navbar.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/web/templates/viewer.html.j2` & `gplugins-0.1.0/gplugins/web/templates/viewer.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/gplugins/widget/interactive.py` & `gplugins-0.1.0/gplugins/widget/interactive.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.3/pyproject.toml` & `gplugins-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 description = "gdsfactory plugins"
 keywords = ["python"]
 license = {file = "LICENSE"}
 name = "gplugins"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.0.3"
+version = "0.1.0"
 
 [project.optional-dependencies]
 database = [
   "sqlalchemy",
   "sqlalchemy-utils",
   "dagster",
   "dagit",
@@ -54,43 +54,43 @@
 docs = [
   "jupytext",
   "autodoc_pydantic",
   "matplotlib",
   "jupyter-book==0.15.1"
 ]
 femwell = [
-  "femwell==0.1.6"
+  "femwell>=0.1.6,<0.2.0"
 ]
 gmsh = [
   "gmsh",
   "h5py",
   "mapbox_earcut",
   "meshio",
   "pygmsh",
   "pyvista",
   "trimesh",
   "shapely",
-  "meshwell==0.0.9"
+  "meshwell>=0.0.9,<0.1.0"
 ]
 meow = [
-  "meow-sim==0.7.1",
-  "tidy3d==2.3.3"
+  "meow-sim>=0.7.1,<0.8.0",
+  "tidy3d>=2.3.3,<2.4.0"
 ]
 sax = [
-  "sax==0.8.8",
+  "sax>=0.8.8,<0.9.0",
   "jaxlib",
   "jax",
   "scikit-learn"
 ]
 schematic = [
-  'bokeh',
+  "bokeh",
   "natsort"
 ]
 tidy3d = [
-  "tidy3d==2.3.3"
+  "tidy3d>=2.3.3,<2.4.0"
 ]
 web = [
   "jinja2",
   "python-multipart",
   "fastapi",
   "uvicorn[standard]"
 ]
```

### Comparing `gplugins-0.0.3/PKG-INFO` & `gplugins-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gplugins
-Version: 0.0.3
+Version: 0.1.0
 Summary: gdsfactory plugins
 Keywords: python
 Author-email: gdsfactory <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,33 +30,33 @@
 Requires-Dist: devsim ; extra == "devsim"
 Requires-Dist: pyvista ; extra == "devsim"
 Requires-Dist: tidy3d ; extra == "devsim"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: autodoc_pydantic ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "docs"
 Requires-Dist: jupyter-book==0.15.1 ; extra == "docs"
-Requires-Dist: femwell==0.1.6 ; extra == "femwell"
+Requires-Dist: femwell>=0.1.6,<0.2.0 ; extra == "femwell"
 Requires-Dist: gmsh ; extra == "gmsh"
 Requires-Dist: h5py ; extra == "gmsh"
 Requires-Dist: mapbox_earcut ; extra == "gmsh"
 Requires-Dist: meshio ; extra == "gmsh"
 Requires-Dist: pygmsh ; extra == "gmsh"
 Requires-Dist: pyvista ; extra == "gmsh"
 Requires-Dist: trimesh ; extra == "gmsh"
 Requires-Dist: shapely ; extra == "gmsh"
-Requires-Dist: meshwell==0.0.9 ; extra == "gmsh"
-Requires-Dist: meow-sim==0.7.1 ; extra == "meow"
-Requires-Dist: tidy3d==2.3.3 ; extra == "meow"
-Requires-Dist: sax==0.8.8 ; extra == "sax"
+Requires-Dist: meshwell>=0.0.9,<0.1.0 ; extra == "gmsh"
+Requires-Dist: meow-sim>=0.7.1,<0.8.0 ; extra == "meow"
+Requires-Dist: tidy3d>=2.3.3,<2.4.0 ; extra == "meow"
+Requires-Dist: sax>=0.8.8,<0.9.0 ; extra == "sax"
 Requires-Dist: jaxlib ; extra == "sax"
 Requires-Dist: jax ; extra == "sax"
 Requires-Dist: scikit-learn ; extra == "sax"
 Requires-Dist: bokeh ; extra == "schematic"
 Requires-Dist: natsort ; extra == "schematic"
-Requires-Dist: tidy3d==2.3.3 ; extra == "tidy3d"
+Requires-Dist: tidy3d>=2.3.3,<2.4.0 ; extra == "tidy3d"
 Requires-Dist: jinja2 ; extra == "web"
 Requires-Dist: python-multipart ; extra == "web"
 Requires-Dist: fastapi ; extra == "web"
 Requires-Dist: uvicorn[standard] ; extra == "web"
 Provides-Extra: database
 Provides-Extra: dev
 Provides-Extra: devsim
@@ -65,15 +65,15 @@
 Provides-Extra: gmsh
 Provides-Extra: meow
 Provides-Extra: sax
 Provides-Extra: schematic
 Provides-Extra: tidy3d
 Provides-Extra: web
 
-# gplugins 0.0.3
+# gplugins 0.1.0
 
 [![docs](https://github.com/gdsfactory/gplugins/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gplugins/)
 [![PyPI](https://img.shields.io/pypi/v/gplugins)](https://pypi.org/project/gplugins/)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gplugins.svg)](https://pypi.python.org/pypi/gplugins)
 [![MIT](https://img.shields.io/github/license/gdsfactory/gplugins)](https://choosealicense.com/licenses/mit/)
 [![codecov](https://img.shields.io/codecov/c/github/gdsfactory/gplugins)](https://codecov.io/gh/gdsfactory/gdsfactory/tree/main/gplugins)
 
@@ -98,15 +98,15 @@
 
 You can install all plugins with:
 
 ```
 pip install "gplugins[database,devsim,femwell,gmsh,schematic,meow,meshwell,ray,sax,tidy3d]" --upgrade
 ```
 
-Or Install only the plugins you need `pip install gplugins[database,devsim]` from the available plugins:
+Or Install only the plugins you need `pip install gplugins[schematic,femwell,meow,sax,tidy3d]` from the available plugins:
 
 Separate installation (not using pip):
 
 - For Meep and MPB you need to use `conda` or `mamba` on MacOS, Linux or [Windows WSL (Windows Subsystem for Linux)](https://learn.microsoft.com/en-us/windows/wsl/install) with `conda install pymeep=*=mpi_mpich_* -c conda-forge -y`
 
 ## Getting started
```

