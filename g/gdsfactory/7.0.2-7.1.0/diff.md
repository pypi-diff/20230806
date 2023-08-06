# Comparing `tmp/gdsfactory-7.0.2.tar.gz` & `tmp/gdsfactory-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsfactory-7.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gdsfactory-7.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gdsfactory-7.0.2.tar` & `gdsfactory-7.1.0.tar`

### file list

```diff
@@ -1,525 +1,526 @@
--rw-r--r--   0        0        0     1072 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/LICENSE
--rw-r--r--   0        0        0     9454 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/README.md
--rw-r--r--   0        0        0     3417 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/__init__.py
--rw-r--r--   0        0        0     1870 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/add_keepout.py
--rw-r--r--   0        0        0    12537 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/add_labels.py
--rw-r--r--   0        0        0     3682 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/add_loopback.py
--rw-r--r--   0        0        0     5016 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/add_padding.py
--rw-r--r--   0        0        0    16012 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/add_pins.py
--rw-r--r--   0        0        0    14682 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/add_ports.py
--rw-r--r--   0        0        0     2864 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/add_tapers.py
--rw-r--r--   0        0        0     2253 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/add_tapers_cross_section.py
--rw-r--r--   0        0        0     1791 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/add_termination.py
--rw-r--r--   0        0        0     1856 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/asserts.py
--rw-r--r--   0        0        0    14884 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/cell.py
--rw-r--r--   0        0        0     5959 2023-08-03 14:49:49.382499 gdsfactory-7.0.2/gdsfactory/cli.py
--rw-r--r--   0        0        0   102115 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/component.py
--rw-r--r--   0        0        0    24269 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/component_layout.py
--rw-r--r--   0        0        0    30803 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/component_reference.py
--rw-r--r--   0        0        0     1179 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/C.py
--rw-r--r--   0        0        0     1105 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/L.py
--rw-r--r--   0        0        0    21495 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/__init__.py
--rw-r--r--   0        0        0     2599 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/add_fiducials.py
--rw-r--r--   0        0        0    13939 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/add_grating_couplers.py
--rw-r--r--   0        0        0     2014 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/add_trenches.py
--rw-r--r--   0        0        0     3168 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/align.py
--rw-r--r--   0        0        0     2528 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/array_component.py
--rw-r--r--   0        0        0     4664 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/array_with_fanout.py
--rw-r--r--   0        0        0     4319 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/array_with_via.py
--rw-r--r--   0        0        0     4042 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/awg.py
--rw-r--r--   0        0        0     1636 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/bbox.py
--rw-r--r--   0        0        0     3048 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/bend_circular.py
--rw-r--r--   0        0        0     2614 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/bend_circular_heater.py
--rw-r--r--   0        0        0     8029 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/bend_euler.py
--rw-r--r--   0        0        0     2663 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/bend_port.py
--rw-r--r--   0        0        0     3807 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/bend_s.py
--rw-r--r--   0        0        0     5338 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/bezier.py
--rw-r--r--   0        0        0     1605 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/cavity.py
--rw-r--r--   0        0        0     5740 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/cdc.py
--rw-r--r--   0        0        0     2888 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/cdsem_all.py
--rw-r--r--   0        0        0     1788 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/cdsem_bend180.py
--rw-r--r--   0        0        0     1593 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/cdsem_coupler.py
--rw-r--r--   0        0        0     1374 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/cdsem_straight.py
--rw-r--r--   0        0        0     1552 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/cdsem_straight_density.py
--rw-r--r--   0        0        0      793 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/circle.py
--rw-r--r--   0        0        0     5933 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coh_rx_dual_pol.py
--rw-r--r--   0        0        0     8880 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coh_rx_single_pol.py
--rw-r--r--   0        0        0     5005 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coh_tx_dual_pol.py
--rw-r--r--   0        0        0     6080 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coh_tx_single_pol.py
--rw-r--r--   0        0        0     2514 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/compass.py
--rw-r--r--   0        0        0     9898 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/component_lattice.py
--rw-r--r--   0        0        0    11731 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/component_lattice_generic.py
--rw-r--r--   0        0        0     7130 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/component_sequence.py
--rw-r--r--   0        0        0      812 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/copy_layers.py
--rw-r--r--   0        0        0     3460 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler.py
--rw-r--r--   0        0        0     2128 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler90.py
--rw-r--r--   0        0        0     1802 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler90bend.py
--rw-r--r--   0        0        0     4666 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler_adiabatic.py
--rw-r--r--   0        0        0     1909 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler_asymmetric.py
--rw-r--r--   0        0        0     4667 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler_bent.py
--rw-r--r--   0        0        0     3970 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler_full.py
--rw-r--r--   0        0        0     5829 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler_ring.py
--rw-r--r--   0        0        0     1060 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler_straight.py
--rw-r--r--   0        0        0     1164 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler_straight_asymmetric.py
--rw-r--r--   0        0        0     2192 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/coupler_symmetric.py
--rw-r--r--   0        0        0     1816 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/cross.py
--rw-r--r--   0        0        0    13157 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/crossing_waveguide.py
--rw-r--r--   0        0        0      500 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
--rw-r--r--   0        0        0     1014 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
--rw-r--r--   0        0        0    19749 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
--rw-r--r--   0        0        0    19751 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
--rw-r--r--   0        0        0    19749 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
--rw-r--r--   0        0        0    19751 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
--rw-r--r--   0        0        0    19775 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
--rw-r--r--   0        0        0     3143 2023-08-03 14:49:49.386499 gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
--rw-r--r--   0        0        0     5256 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/cutback_2x2.py
--rw-r--r--   0        0        0     6743 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/cutback_bend.py
--rw-r--r--   0        0        0     3759 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/cutback_component.py
--rw-r--r--   0        0        0     2708 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/cutback_splitter.py
--rw-r--r--   0        0        0     2971 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/dbr.py
--rw-r--r--   0        0        0     4262 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/dbr_tapered.py
--rw-r--r--   0        0        0     2481 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/delay_snake.py
--rw-r--r--   0        0        0     3176 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/delay_snake2.py
--rw-r--r--   0        0        0     3245 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/delay_snake3.py
--rw-r--r--   0        0        0     4313 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/delay_snake_sbend.py
--rw-r--r--   0        0        0     1254 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/dicing_lane.py
--rw-r--r--   0        0        0     3578 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/die.py
--rw-r--r--   0        0        0     2968 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/die_bbox.py
--rw-r--r--   0        0        0     2816 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/die_bbox_frame.py
--rw-r--r--   0        0        0     7984 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/disk.py
--rw-r--r--   0        0        0     4121 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/edge_coupler_array.py
--rw-r--r--   0        0        0     1188 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/ellipse.py
--rw-r--r--   0        0        0     1756 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/extend_ports_list.py
--rw-r--r--   0        0        0     7046 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/extension.py
--rw-r--r--   0        0        0      981 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/fiber.py
--rw-r--r--   0        0        0     1432 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/fiber_array.py
--rw-r--r--   0        0        0      722 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/fiducial_squares.py
--rw-r--r--   0        0        0     3225 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/ge_detector_straight_si_contacts.py
--rw-r--r--   0        0        0     2458 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_array.py
--rw-r--r--   0        0        0     4651 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_dual_pol.py
--rw-r--r--   0        0        0     7137 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_elliptical.py
--rw-r--r--   0        0        0     7209 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
--rw-r--r--   0        0        0     4942 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_elliptical_lumerical.py
--rw-r--r--   0        0        0     4694 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_elliptical_trenches.py
--rw-r--r--   0        0        0     1747 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_functions.py
--rw-r--r--   0        0        0     9054 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_loss.py
--rw-r--r--   0        0        0     1814 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_loss_fiber_single.py
--rw-r--r--   0        0        0     4110 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_rectangular.py
--rw-r--r--   0        0        0     4650 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
--rw-r--r--   0        0        0     3855 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
--rw-r--r--   0        0        0     1579 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/grating_coupler_tree.py
--rw-r--r--   0        0        0     8722 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/greek_cross.py
--rw-r--r--   0        0        0     1019 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/hline.py
--rw-r--r--   0        0        0     3643 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/interdigital_capacitor.py
--rw-r--r--   0        0        0     1799 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/litho_calipers.py
--rw-r--r--   0        0        0     1218 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/litho_ruler.py
--rw-r--r--   0        0        0     1278 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/litho_steps.py
--rw-r--r--   0        0        0      650 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/logo.py
--rw-r--r--   0        0        0     1679 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/loop_mirror.py
--rw-r--r--   0        0        0     5005 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mmi.py
--rw-r--r--   0        0        0     3978 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mmi1x2.py
--rw-r--r--   0        0        0     2769 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mmi1x2_with_sbend.py
--rw-r--r--   0        0        0     3801 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mmi2x2.py
--rw-r--r--   0        0        0     3192 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mmi2x2_with_sbend.py
--rw-r--r--   0        0        0     4944 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mmi_90degree_hybrid.py
--rw-r--r--   0        0        0     3293 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mode_converter.py
--rw-r--r--   0        0        0     7610 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mzi.py
--rw-r--r--   0        0        0     2464 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mzi_arm.py
--rw-r--r--   0        0        0     5822 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mzi_arms.py
--rw-r--r--   0        0        0    12188 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mzi_lattice.py
--rw-r--r--   0        0        0     4020 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mzi_pads_center.py
--rw-r--r--   0        0        0     1264 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mzi_phase_shifter.py
--rw-r--r--   0        0        0     6310 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mzit.py
--rw-r--r--   0        0        0     3476 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mzit_lattice.py
--rw-r--r--   0        0        0     6016 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/mzm.py
--rw-r--r--   0        0        0     3518 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/nxn.py
--rw-r--r--   0        0        0     1940 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/optimal_90deg.py
--rw-r--r--   0        0        0     3876 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/optimal_hairpin.py
--rw-r--r--   0        0        0     6131 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/optimal_step.py
--rw-r--r--   0        0        0     6289 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/pack_doe.py
--rw-r--r--   0        0        0     3833 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/pad.py
--rw-r--r--   0        0        0     1915 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/pad_gsg.py
--rw-r--r--   0        0        0     1157 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/pads_shorted.py
--rw-r--r--   0        0        0     3799 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/polarization_splitter_rotator.py
--rw-r--r--   0        0        0     1115 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/ramp.py
--rw-r--r--   0        0        0     1475 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/rectangle.py
--rw-r--r--   0        0        0     2933 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/rectangle_with_slits.py
--rw-r--r--   0        0        0     1059 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/rectangular_ring.py
--rw-r--r--   0        0        0     1476 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/regular_polygon.py
--rw-r--r--   0        0        0     3276 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/resistance_meander.py
--rw-r--r--   0        0        0     2629 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/resistance_sheet.py
--rw-r--r--   0        0        0     1260 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/ring.py
--rw-r--r--   0        0        0     4118 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/ring_crow.py
--rw-r--r--   0        0        0     3247 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/ring_crow_couplers.py
--rw-r--r--   0        0        0     2348 2023-08-03 14:49:49.390499 gdsfactory-7.0.2/gdsfactory/components/ring_double.py
--rw-r--r--   0        0        0     2846 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_double_bend_coupler.py
--rw-r--r--   0        0        0     5102 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_double_heater.py
--rw-r--r--   0        0        0     7747 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_double_pn.py
--rw-r--r--   0        0        0    12046 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_section_based.py
--rw-r--r--   0        0        0     2909 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_single.py
--rw-r--r--   0        0        0     1923 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_single_array.py
--rw-r--r--   0        0        0     6868 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_single_bend_coupler.py
--rw-r--r--   0        0        0     2743 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_single_dut.py
--rw-r--r--   0        0        0     4231 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_single_heater.py
--rw-r--r--   0        0        0     5307 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/ring_single_pn.py
--rw-r--r--   0        0        0     2281 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/seal_ring.py
--rw-r--r--   0        0        0     3745 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/snspd.py
--rw-r--r--   0        0        0     2059 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/spiral_double.py
--rw-r--r--   0        0        0     5832 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/spiral_external_io.py
--rw-r--r--   0        0        0    16624 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/spiral_heater.py
--rw-r--r--   0        0        0     9155 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/spiral_inner_io.py
--rw-r--r--   0        0        0     1733 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/splitter_chain.py
--rw-r--r--   0        0        0     5289 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/splitter_tree.py
--rw-r--r--   0        0        0     2640 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight.py
--rw-r--r--   0        0        0     1033 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight_array.py
--rw-r--r--   0        0        0     7863 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight_heater_doped_rib.py
--rw-r--r--   0        0        0     1922 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight_heater_doped_strip.py
--rw-r--r--   0        0        0     8266 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight_heater_meander.py
--rw-r--r--   0        0        0     8519 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight_heater_meander_doped.py
--rw-r--r--   0        0        0     6044 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight_heater_metal.py
--rw-r--r--   0        0        0     2805 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight_pin.py
--rw-r--r--   0        0        0     3955 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight_pin_slot.py
--rw-r--r--   0        0        0      656 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/straight_rib.py
--rw-r--r--   0        0        0      821 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/switch_tree.py
--rw-r--r--   0        0        0     7973 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/taper.py
--rw-r--r--   0        0        0     3539 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/taper_adiabatic.py
--rw-r--r--   0        0        0     2801 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/taper_cross_section.py
--rw-r--r--   0        0        0     2363 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/taper_from_csv.py
--rw-r--r--   0        0        0     1235 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/taper_parabolic.py
--rw-r--r--   0        0        0     1787 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/terminator.py
--rw-r--r--   0        0        0     2887 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/text.py
--rw-r--r--   0        0        0     3886 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/text_freetype.py
--rw-r--r--   0        0        0     3186 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/text_rectangular.py
--rw-r--r--   0        0        0     3897 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/text_rectangular_font.py
--rw-r--r--   0        0        0     2536 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/triangles.py
--rw-r--r--   0        0        0      715 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/verniers.py
--rw-r--r--   0        0        0     2430 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/version_stamp.py
--rw-r--r--   0        0        0     2413 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/via.py
--rw-r--r--   0        0        0     3034 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/via_corner.py
--rw-r--r--   0        0        0     5342 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/via_cutback.py
--rw-r--r--   0        0        0    15895 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/via_stack.py
--rw-r--r--   0        0        0     4516 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/via_stack_slot.py
--rw-r--r--   0        0        0     4918 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/via_stack_with_offset.py
--rw-r--r--   0        0        0     1065 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/wafer.py
--rw-r--r--   0        0        0     7181 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/wire.py
--rw-r--r--   0        0        0      978 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/components/wire_sbend.py
--rw-r--r--   0        0        0    10085 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/config.py
--rw-r--r--   0        0        0    38409 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/constants.py
--rw-r--r--   0        0        0    83618 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/cross_section.py
--rw-r--r--   0        0        0     2963 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/decorators.py
--rw-r--r--   0        0        0     8406 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/difftest.py
--rw-r--r--   0        0        0      668 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/difftest_git.py
--rw-r--r--   0        0        0     1029 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/events.py
--rw-r--r--   0        0        0      267 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/export/__init__.py
--rw-r--r--   0        0        0     3308 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/export/to_3d.py
--rw-r--r--   0        0        0     7531 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/export/to_gerber.py
--rw-r--r--   0        0        0     1908 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/export/to_np.py
--rw-r--r--   0        0        0     3095 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/export/to_stl.py
--rw-r--r--   0        0        0    11831 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/fill.py
--rw-r--r--   0        0        0     7780 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/font.py
--rw-r--r--   0        0        0     8067 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/functions.py
--rw-r--r--   0        0        0     1025 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/generic_tech/README.md
--rw-r--r--   0        0        0     1957 2023-08-03 14:49:49.394499 gdsfactory-7.0.2/gdsfactory/generic_tech/__init__.py
--rw-r--r--   0        0        0     1008 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/containers.py
--rw-r--r--   0        0        0      169 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/generic_tech.sh
--rw-r--r--   0        0        0     8117 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/get_klayout_pyxs.py
--rw-r--r--   0        0        0      161 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/README.md
--rw-r--r--   0        0        0      104 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/drc/Makefile
--rw-r--r--   0        0        0        0 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/drc/__init__.py
--rw-r--r--   0        0        0     2842 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/drc/errors.py
--rw-r--r--   0        0        0     6192 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/grain.xml
--rw-r--r--   0        0        0    10140 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/icon_128x128.png
--rw-r--r--   0        0        0     4248 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/icon_64x64.png
--rw-r--r--   0        0        0       27 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/.gitignore
--rw-r--r--   0        0        0      494 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/Makefile
--rw-r--r--   0        0        0     4062 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/README.md
--rw-r--r--   0        0        0     2419 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
--rw-r--r--   0        0        0     9696 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
--rw-r--r--   0        0        0    12379 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
--rw-r--r--   0        0        0     7235 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
--rw-r--r--   0        0        0     3446 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
--rw-r--r--   0        0        0      479 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
--rw-r--r--   0        0        0      582 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
--rw-r--r--   0        0        0      108 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
--rw-r--r--   0        0        0      186 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
--rw-r--r--   0        0        0      398 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
--rw-r--r--   0        0        0      574 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
--rw-r--r--   0        0        0     6034 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
--rw-r--r--   0        0        0    10697 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
--rw-r--r--   0        0        0      477 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
--rw-r--r--   0        0        0     4338 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
--rw-r--r--   0        0        0      926 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
--rw-r--r--   0        0        0    10945 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
--rw-r--r--   0        0        0      709 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0      538 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
--rw-r--r--   0        0        0        0 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/python/__init__.py
--rw-r--r--   0        0        0      114 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
--rw-r--r--   0        0        0     4312 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
--rw-r--r--   0        0        0      269 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/Makefile
--rw-r--r--   0        0        0     1800 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
--rw-r--r--   0        0        0     1519 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/generic.layerstack
--rw-r--r--   0        0        0    41073 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
--rw-r--r--   0        0        0    40616 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/layers.lyp
--rw-r--r--   0        0        0     5977 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/tech.lyt
--rw-r--r--   0        0        0     4258 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
--rw-r--r--   0        0        0     4537 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
--rw-r--r--   0        0        0     4690 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
--rw-r--r--   0        0        0     5508 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
--rw-r--r--   0        0        0     1857 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/layer_map.py
--rw-r--r--   0        0        0     6511 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/layer_stack.py
--rw-r--r--   0        0        0    10780 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/layer_views.yaml
--rw-r--r--   0        0        0     3916 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/generic_tech/simulation_settings.py
--rw-r--r--   0        0        0     1431 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/__init__.py
--rw-r--r--   0        0        0     4869 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/boolean.py
--rw-r--r--   0        0        0     3789 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/boolean_klayout.py
--rw-r--r--   0        0        0     1862 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/boolean_polygons.py
--rw-r--r--   0        0        0      567 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/check_duplicated_cells.py
--rw-r--r--   0        0        0     2693 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/check_exclusion.py
--rw-r--r--   0        0        0     2803 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/check_inclusion.py
--rw-r--r--   0        0        0     3540 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/check_space.py
--rw-r--r--   0        0        0     1867 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/check_width.py
--rw-r--r--   0        0        0     4954 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/fill_klayout.py
--rw-r--r--   0        0        0     7017 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/fill_tiled.py
--rw-r--r--   0        0        0     1655 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/fillet.py
--rw-r--r--   0        0        0     6614 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/functions.py
--rw-r--r--   0        0        0     2167 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/invert.py
--rw-r--r--   0        0        0     3686 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/layer_priority.py
--rw-r--r--   0        0        0     3055 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/manhattanize.py
--rw-r--r--   0        0        0     4184 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/maskprep.py
--rw-r--r--   0        0        0     4759 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/maskprep_flat.py
--rw-r--r--   0        0        0     3248 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/offset.py
--rw-r--r--   0        0        0     3810 2023-08-03 14:49:49.398499 gdsfactory-7.0.2/gdsfactory/geometry/outline.py
--rw-r--r--   0        0        0     2465 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/geometry/trim.py
--rw-r--r--   0        0        0     2952 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/geometry/union.py
--rw-r--r--   0        0        0     3626 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/geometry/write_connectivity.py
--rw-r--r--   0        0        0    10476 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/geometry/write_drc.py
--rw-r--r--   0        0        0     1783 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/geometry/xor_diff.py
--rw-r--r--   0        0        0     1152 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/get_factories.py
--rw-r--r--   0        0        0    23637 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/get_netlist.py
--rw-r--r--   0        0        0    14481 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/get_netlist_flat.py
--rw-r--r--   0        0        0     9689 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/grid.py
--rw-r--r--   0        0        0     5083 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/install.py
--rw-r--r--   0        0        0     1855 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/klive.py
--rw-r--r--   0        0        0      585 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/labels/__init__.py
--rw-r--r--   0        0        0     3519 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/labels/add_label_yaml.py
--rw-r--r--   0        0        0     3818 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/labels/ehva.py
--rw-r--r--   0        0        0     3796 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/labels/merge_test_metadata.py
--rw-r--r--   0        0        0     4644 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/labels/siepic.py
--rw-r--r--   0        0        0     4840 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/labels/write_labels.py
--rw-r--r--   0        0        0     5247 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/name.py
--rw-r--r--   0        0        0    11574 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/pack.py
--rw-r--r--   0        0        0    52172 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/path.py
--rw-r--r--   0        0        0    30164 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/pdk.py
--rw-r--r--   0        0        0     6092 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/picmodel.py
--rw-r--r--   0        0        0     5029 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/pixelate.py
--rw-r--r--   0        0        0      303 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/plugins/__init__.py
--rw-r--r--   0        0        0     4262 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/polygon.py
--rw-r--r--   0        0        0    32988 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/port.py
--rw-r--r--   0        0        0    37674 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/quickplotter.py
--rw-r--r--   0        0        0      696 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/__init__.py
--rw-r--r--   0        0        0     1639 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/from_dphox.py
--rw-r--r--   0        0        0     1259 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/from_gdspaths.py
--rw-r--r--   0        0        0     1927 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/from_np.py
--rw-r--r--   0        0        0     2773 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/from_phidl.py
--rw-r--r--   0        0        0     4222 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/from_updk.py
--rw-r--r--   0        0        0    37973 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/from_yaml.py
--rw-r--r--   0        0        0     5997 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/from_yaml_template.py
--rw-r--r--   0        0        0     5632 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/import_gds.py
--rw-r--r--   0        0        0     3369 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/read/labels.py
--rw-r--r--   0        0        0     1614 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/route_info.py
--rw-r--r--   0        0        0     3767 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/__init__.py
--rw-r--r--   0        0        0     2907 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/add_electrical_pads_shortest.py
--rw-r--r--   0        0        0     3002 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/add_electrical_pads_top.py
--rw-r--r--   0        0        0     3031 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/add_electrical_pads_top_dc.py
--rw-r--r--   0        0        0     8726 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/add_fiber_array.py
--rw-r--r--   0        0        0    10573 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/add_fiber_single.py
--rw-r--r--   0        0        0     9220 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/add_pads.py
--rw-r--r--   0        0        0    38995 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/all_angle.py
--rw-r--r--   0        0        0     3879 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/auto_taper.py
--rw-r--r--   0        0        0      981 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/factories.py
--rw-r--r--   0        0        0     4324 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/fanout.py
--rw-r--r--   0        0        0     2796 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/fanout2x2.py
--rw-r--r--   0        0        0    25075 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/get_bundle.py
--rw-r--r--   0        0        0     8642 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/get_bundle_corner.py
--rw-r--r--   0        0        0     6904 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/get_bundle_from_steps.py
--rw-r--r--   0        0        0    12925 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/get_bundle_from_waypoints.py
--rw-r--r--   0        0        0     5258 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/get_bundle_path_length_match.py
--rw-r--r--   0        0        0     1912 2023-08-03 14:49:49.402499 gdsfactory-7.0.2/gdsfactory/routing/get_bundle_sbend.py
--rw-r--r--   0        0        0    17052 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/get_bundle_u.py
--rw-r--r--   0        0        0     1486 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/get_input_labels.py
--rw-r--r--   0        0        0     9226 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/get_route.py
--rw-r--r--   0        0        0    10829 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/get_route_astar.py
--rw-r--r--   0        0        0     6090 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/get_route_from_steps.py
--rw-r--r--   0        0        0     2766 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/get_route_sbend.py
--rw-r--r--   0        0        0     3246 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/get_routes_bend180.py
--rw-r--r--   0        0        0     1773 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/get_routes_straight.py
--rw-r--r--   0        0        0    34260 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/manhattan.py
--rw-r--r--   0        0        0    10037 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/path_length_matching.py
--rw-r--r--   0        0        0    22673 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/route_fiber_array.py
--rw-r--r--   0        0        0     8643 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/route_fiber_single.py
--rw-r--r--   0        0        0    18074 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/route_ports_to_side.py
--rw-r--r--   0        0        0     4341 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/route_quad.py
--rw-r--r--   0        0        0    14296 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/route_sharp.py
--rw-r--r--   0        0        0    10141 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/route_south.py
--rw-r--r--   0        0        0     5040 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/sort_ports.py
--rw-r--r--   0        0        0     2433 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/routing/utils.py
--rw-r--r--   0        0        0     2767 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/01_component_pcell.py
--rw-r--r--   0        0        0      646 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
--rw-r--r--   0        0        0      974 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/01_component_pcell_with_pins.py
--rw-r--r--   0        0        0      664 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
--rw-r--r--   0        0        0      347 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/02_component_autoname.py
--rw-r--r--   0        0        0      887 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/03_move.py
--rw-r--r--   0        0        0      881 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/04_connect.py
--rw-r--r--   0        0        0      698 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/05_remove_layers.py
--rw-r--r--   0        0        0      925 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/06_remapping_layers.py
--rw-r--r--   0        0        0     1081 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/07_flattening_device.py
--rw-r--r--   0        0        0      475 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/08_group.py
--rw-r--r--   0        0        0     1621 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/11_component_layout.py
--rw-r--r--   0        0        0     2225 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/12_component_refs.py
--rw-r--r--   0        0        0     1013 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/13_component_netlist.py
--rw-r--r--   0        0        0     2592 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/14_component_connectivity.py
--rw-r--r--   0        0        0     1683 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/15_component_sequence1.py
--rw-r--r--   0        0        0     1733 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/16_component_sequence2.py
--rw-r--r--   0        0        0     1030 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/17_ports.py
--rw-r--r--   0        0        0      272 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/18_port_markers.py
--rw-r--r--   0        0        0      361 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/19_references.py
--rw-r--r--   0        0        0      561 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/20_components.py
--rw-r--r--   0        0        0      565 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/21_add_fiber_array.py
--rw-r--r--   0        0        0      550 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/22_add_fiber_single.py
--rw-r--r--   0        0        0      632 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/22_add_pads.py
--rw-r--r--   0        0        0      847 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/23_reticle.py
--rw-r--r--   0        0        0      924 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/23_reticle_passives_grid.py
--rw-r--r--   0        0        0     1177 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/23_reticle_passives_pack.py
--rw-r--r--   0        0        0      381 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/24_doe.py
--rw-r--r--   0        0        0      715 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/24_doe_2.py
--rw-r--r--   0        0        0      720 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/24_doe_3.py
--rw-r--r--   0        0        0      306 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/25_slot_cross_section.py
--rw-r--r--   0        0        0     1363 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/30_lidar.py
--rw-r--r--   0        0        0     1434 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/30_lidar_pcell.py
--rw-r--r--   0        0        0     1943 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/30_lidar_with_pads.py
--rw-r--r--   0        0        0        0 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/__init__.py
--rw-r--r--   0        0        0     1308 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing.py
--rw-r--r--   0        0        0      558 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
--rw-r--r--   0        0        0     6062 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
--rw-r--r--   0        0        0      444 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
--rw-r--r--   0        0        0      463 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
--rw-r--r--   0        0        0     1552 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
--rw-r--r--   0        0        0     1315 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
--rw-r--r--   0        0        0      602 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
--rw-r--r--   0        0        0     3317 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
--rw-r--r--   0        0        0     1484 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
--rw-r--r--   0        0        0     3045 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
--rw-r--r--   0        0        0     3782 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
--rw-r--r--   0        0        0     2393 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/big_device.py
--rw-r--r--   0        0        0       19 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/Makefile
--rw-r--r--   0        0        0        0 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/__init__.py
--rw-r--r--   0        0        0     1129 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/benchmark/fill_demo.py
--rw-r--r--   0        0        0      343 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
--rw-r--r--   0        0        0      637 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/circuits/mask.pic.yml
--rw-r--r--   0        0        0      622 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
--rw-r--r--   0        0        0      569 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
--rw-r--r--   0        0        0      453 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/circuits/pads.pic.yml
--rw-r--r--   0        0        0      287 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/circuits/rectangles.pic.yml
--rw-r--r--   0        0        0     2296 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/drc_errors.py
--rw-r--r--   0        0        0      989 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/drc_write.py
--rw-r--r--   0        0        0     4494 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/layers.py
--rw-r--r--   0        0        0      158 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/layers_sky130.py
--rw-r--r--   0        0        0      363 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/layers_xsection.py
--rw-r--r--   0        0        0     1065 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/lvs.py
--rw-r--r--   0        0        0      574 2023-08-03 14:49:49.406499 gdsfactory-7.0.2/gdsfactory/samples/demo/pcell.py
--rw-r--r--   0        0        0     4174 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/netlists/mzi.yml
--rw-r--r--   0        0        0     5840 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/netlists/mzi_full.yml
--rw-r--r--   0        0        0        0 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/.gitignore
--rw-r--r--   0        0        0    10181 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/00_geometry.py
--rw-r--r--   0        0        0    13583 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/01_references.py
--rw-r--r--   0        0        0     5845 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/02_movement.py
--rw-r--r--   0        0        0    29824 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/03_Path_CrossSection.py
--rw-r--r--   0        0        0     6881 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/03_cells_autoname_and_cache.py
--rw-r--r--   0        0        0    16888 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/03_layer_stack.py
--rw-r--r--   0        0        0    11362 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_components_geometry.py
--rw-r--r--   0        0        0     5789 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_components_hierarchy.py
--rw-r--r--   0        0        0     7287 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_components_pack.py
--rw-r--r--   0        0        0     8093 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_components_shapes.py
--rw-r--r--   0        0        0    27801 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_routing.py
--rw-r--r--   0        0        0    10894 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_routing_electrical.py
--rw-r--r--   0        0        0    17498 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_routing_non_manhattan.py
--rw-r--r--   0        0        0    12399 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/07_mask.py
--rw-r--r--   0        0        0    15157 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/08_pdk.py
--rw-r--r--   0        0        0    11094 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/08_pdk_examples.py
--rw-r--r--   0        0        0     8585 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/09_pdk_import.py
--rw-r--r--   0        0        0    17564 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/10_yaml_component.py
--rw-r--r--   0        0        0     4684 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/11_get_netlist.py
--rw-r--r--   0        0        0     2114 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/11_get_netlist_spice.py
--rw-r--r--   0        0        0     4477 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/21_drc.py
--rw-r--r--   0        0        0      437 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/Makefile
--rw-r--r--   0        0        0     6217 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/_0_python.py
--rw-r--r--   0        0        0    16372 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/_1_git.py
--rw-r--r--   0        0        0     1092 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/_2_klayout.py
--rw-r--r--   0        0        0     1384 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/_3_vscode.py
--rw-r--r--   0        0        0     8163 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/_4_gdsfactory.py
--rw-r--r--   0        0        0     4412 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/common_mistakes.py
--rw-r--r--   0        0        0     4018 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/dataprep.py
--rw-r--r--   0        0        0     2660 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/declarative_cell.py
--rw-r--r--   0        0        0    13148 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/images/inkscape_align.png
--rw-r--r--   0        0        0    14726 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/images/inkscape_distribute.png
--rw-r--r--   0        0        0    71039 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/images/pathlength_report.png
--rw-r--r--   0        0        0    67563 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/images/pathlength_report_highlighted.png
--rw-r--r--   0        0        0     6558 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/rib_strip_autotransition.py
--rw-r--r--   0        0        0      591 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back.pic.yml
--rw-r--r--   0        0        0      726 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back2.pic.yml
--rw-r--r--   0        0        0      822 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back3.pic.yml
--rw-r--r--   0        0        0     1417 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_bundles01.pic.yml
--rw-r--r--   0        0        0     1508 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_bundles02.pic.yml
--rw-r--r--   0        0        0     1405 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_bundles03.pic.yml
--rw-r--r--   0        0        0      600 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_indirect.pic.yml
--rw-r--r--   0        0        0      614 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_simple.pic.yml
--rw-r--r--   0        0        0     1152 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_steps01.pic.yml
--rw-r--r--   0        0        0     1066 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_final.pic.yml
--rw-r--r--   0        0        0      778 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_initial.pic.yml
--rw-r--r--   0        0        0     1423 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_steps03.pic.yml
--rw-r--r--   0        0        0      857 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_wonky_connector.pic.yml
--rw-r--r--   0        0        0        0 2023-08-03 14:49:49.410499 gdsfactory-7.0.2/gdsfactory/samples/pdk/__init__.py
--rw-r--r--   0        0        0     3668 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/fab_c.py
--rw-r--r--   0        0        0      233 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/fab_c_to_updk.py
--rw-r--r--   0        0        0      475 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/fab_d/__init__.py
--rw-r--r--   0        0        0     1893 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/fab_d/phase_shifters.py
--rw-r--r--   0        0        0     1745 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c.py
--rw-r--r--   0        0        0       50 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
--rw-r--r--   0        0        0       93 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
--rw-r--r--   0        0        0       85 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
--rw-r--r--   0        0        0      139 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
--rw-r--r--   0        0        0       90 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
--rw-r--r--   0        0        0      126 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
--rw-r--r--   0        0        0       48 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
--rw-r--r--   0        0        0     1023 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
--rw-r--r--   0        0        0     3102 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
--rw-r--r--   0        0        0     2419 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
--rw-r--r--   0        0        0     1283 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
--rw-r--r--   0        0        0     2252 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
--rw-r--r--   0        0        0     1061 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
--rw-r--r--   0        0        0     1054 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
--rw-r--r--   0        0        0     2237 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
--rw-r--r--   0        0        0     6899 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
--rw-r--r--   0        0        0     3625 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
--rw-r--r--   0        0        0     3603 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
--rw-r--r--   0        0        0     6857 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
--rw-r--r--   0        0        0      840 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
--rw-r--r--   0        0        0     3434 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
--rw-r--r--   0        0        0     4531 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/serialization.py
--rw-r--r--   0        0        0     1569 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/show.py
--rw-r--r--   0        0        0      525 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/simulation/__init__.py
--rw-r--r--   0        0        0     1689 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/snap.py
--rw-r--r--   0        0        0     4254 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/symbols.py
--rw-r--r--   0        0        0      308 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/technology/__init__.py
--rw-r--r--   0        0        0      343 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/technology/color_utils.py
--rw-r--r--   0        0        0     7550 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/technology/klayout_tech.py
--rw-r--r--   0        0        0     1041 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/technology/layer_map.py
--rw-r--r--   0        0        0    19086 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/technology/layer_stack.py
--rw-r--r--   0        0        0    41893 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/technology/layer_views.py
--rw-r--r--   0        0        0      674 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/technology/xml_utils.py
--rw-r--r--   0        0        0     1413 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/technology/yaml_utils.py
--rw-r--r--   0        0        0    11084 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/typings.py
--rw-r--r--   0        0        0     5489 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/watch.py
--rw-r--r--   0        0        0     7419 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/gdsfactory/write_cells.py
--rw-r--r--   0        0        0     4328 2023-08-03 14:49:49.414499 gdsfactory-7.0.2/pyproject.toml
--rw-r--r--   0        0        0    11987 1970-01-01 00:00:00.000000 gdsfactory-7.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/LICENSE
+-rw-r--r--   0        0        0     7441 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/README.md
+-rw-r--r--   0        0        0     3417 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/__init__.py
+-rw-r--r--   0        0        0     1870 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/add_keepout.py
+-rw-r--r--   0        0        0    12537 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/add_labels.py
+-rw-r--r--   0        0        0     3682 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/add_loopback.py
+-rw-r--r--   0        0        0     5016 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/add_padding.py
+-rw-r--r--   0        0        0    16012 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/add_pins.py
+-rw-r--r--   0        0        0    14682 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/add_ports.py
+-rw-r--r--   0        0        0     2864 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/add_tapers.py
+-rw-r--r--   0        0        0     2253 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/add_tapers_cross_section.py
+-rw-r--r--   0        0        0     1791 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/add_termination.py
+-rw-r--r--   0        0        0     1856 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/asserts.py
+-rw-r--r--   0        0        0    14884 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/cell.py
+-rw-r--r--   0        0        0     5958 2023-08-05 19:31:52.219140 gdsfactory-7.1.0/gdsfactory/cli.py
+-rw-r--r--   0        0        0   102902 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/component.py
+-rw-r--r--   0        0        0    24269 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/component_layout.py
+-rw-r--r--   0        0        0    30803 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/component_reference.py
+-rw-r--r--   0        0        0     1179 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/C.py
+-rw-r--r--   0        0        0     1105 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/L.py
+-rw-r--r--   0        0        0    21495 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/__init__.py
+-rw-r--r--   0        0        0     2599 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/add_fiducials.py
+-rw-r--r--   0        0        0    13939 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/add_grating_couplers.py
+-rw-r--r--   0        0        0     2014 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/add_trenches.py
+-rw-r--r--   0        0        0     3168 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/align.py
+-rw-r--r--   0        0        0     2528 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/array_component.py
+-rw-r--r--   0        0        0     4664 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/array_with_fanout.py
+-rw-r--r--   0        0        0     4319 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/array_with_via.py
+-rw-r--r--   0        0        0     4042 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/awg.py
+-rw-r--r--   0        0        0     1636 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/bbox.py
+-rw-r--r--   0        0        0     3048 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/bend_circular.py
+-rw-r--r--   0        0        0     2614 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/bend_circular_heater.py
+-rw-r--r--   0        0        0     8029 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/bend_euler.py
+-rw-r--r--   0        0        0     2663 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/bend_port.py
+-rw-r--r--   0        0        0     3807 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/bend_s.py
+-rw-r--r--   0        0        0     5417 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/bezier.py
+-rw-r--r--   0        0        0     1605 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cavity.py
+-rw-r--r--   0        0        0     5740 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cdc.py
+-rw-r--r--   0        0        0     2888 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cdsem_all.py
+-rw-r--r--   0        0        0     1788 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cdsem_bend180.py
+-rw-r--r--   0        0        0     1593 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cdsem_coupler.py
+-rw-r--r--   0        0        0     1374 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cdsem_straight.py
+-rw-r--r--   0        0        0     1552 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cdsem_straight_density.py
+-rw-r--r--   0        0        0      793 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/circle.py
+-rw-r--r--   0        0        0     5933 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coh_rx_dual_pol.py
+-rw-r--r--   0        0        0     8880 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coh_rx_single_pol.py
+-rw-r--r--   0        0        0     5005 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coh_tx_dual_pol.py
+-rw-r--r--   0        0        0     6080 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coh_tx_single_pol.py
+-rw-r--r--   0        0        0     2514 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/compass.py
+-rw-r--r--   0        0        0     9898 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/component_lattice.py
+-rw-r--r--   0        0        0    11731 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/component_lattice_generic.py
+-rw-r--r--   0        0        0     7130 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/component_sequence.py
+-rw-r--r--   0        0        0      812 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/copy_layers.py
+-rw-r--r--   0        0        0     3460 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler.py
+-rw-r--r--   0        0        0     2128 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler90.py
+-rw-r--r--   0        0        0     1802 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler90bend.py
+-rw-r--r--   0        0        0     4666 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler_adiabatic.py
+-rw-r--r--   0        0        0     1909 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler_asymmetric.py
+-rw-r--r--   0        0        0     4667 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler_bent.py
+-rw-r--r--   0        0        0     3970 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler_full.py
+-rw-r--r--   0        0        0     5829 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler_ring.py
+-rw-r--r--   0        0        0     1060 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler_straight.py
+-rw-r--r--   0        0        0     1164 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler_straight_asymmetric.py
+-rw-r--r--   0        0        0     2192 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/coupler_symmetric.py
+-rw-r--r--   0        0        0     1816 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cross.py
+-rw-r--r--   0        0        0    13157 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/crossing_waveguide.py
+-rw-r--r--   0        0        0      500 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
+-rw-r--r--   0        0        0     1014 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
+-rw-r--r--   0        0        0    19749 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
+-rw-r--r--   0        0        0    19751 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
+-rw-r--r--   0        0        0    19749 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
+-rw-r--r--   0        0        0    19751 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
+-rw-r--r--   0        0        0    19775 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
+-rw-r--r--   0        0        0     3143 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
+-rw-r--r--   0        0        0     5256 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cutback_2x2.py
+-rw-r--r--   0        0        0     6743 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cutback_bend.py
+-rw-r--r--   0        0        0     3759 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cutback_component.py
+-rw-r--r--   0        0        0     2708 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/cutback_splitter.py
+-rw-r--r--   0        0        0     2971 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/dbr.py
+-rw-r--r--   0        0        0     4262 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/dbr_tapered.py
+-rw-r--r--   0        0        0     2481 2023-08-05 19:31:52.223140 gdsfactory-7.1.0/gdsfactory/components/delay_snake.py
+-rw-r--r--   0        0        0     3176 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/delay_snake2.py
+-rw-r--r--   0        0        0     3245 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/delay_snake3.py
+-rw-r--r--   0        0        0     4313 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/delay_snake_sbend.py
+-rw-r--r--   0        0        0     1254 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/dicing_lane.py
+-rw-r--r--   0        0        0     3578 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/die.py
+-rw-r--r--   0        0        0     2968 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/die_bbox.py
+-rw-r--r--   0        0        0     2816 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/die_bbox_frame.py
+-rw-r--r--   0        0        0     7984 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/disk.py
+-rw-r--r--   0        0        0     4121 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/edge_coupler_array.py
+-rw-r--r--   0        0        0     1188 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ellipse.py
+-rw-r--r--   0        0        0     1756 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/extend_ports_list.py
+-rw-r--r--   0        0        0     7046 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/extension.py
+-rw-r--r--   0        0        0      981 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/fiber.py
+-rw-r--r--   0        0        0     1432 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/fiber_array.py
+-rw-r--r--   0        0        0      722 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/fiducial_squares.py
+-rw-r--r--   0        0        0     3225 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ge_detector_straight_si_contacts.py
+-rw-r--r--   0        0        0     2458 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_array.py
+-rw-r--r--   0        0        0     4651 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_dual_pol.py
+-rw-r--r--   0        0        0     7137 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_elliptical.py
+-rw-r--r--   0        0        0     7209 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
+-rw-r--r--   0        0        0     4942 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
+-rw-r--r--   0        0        0     4694 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
+-rw-r--r--   0        0        0     1747 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_functions.py
+-rw-r--r--   0        0        0     9054 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_loss.py
+-rw-r--r--   0        0        0     1814 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
+-rw-r--r--   0        0        0     4110 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_rectangular.py
+-rw-r--r--   0        0        0     4650 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
+-rw-r--r--   0        0        0     3855 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
+-rw-r--r--   0        0        0     1579 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/grating_coupler_tree.py
+-rw-r--r--   0        0        0     8722 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/greek_cross.py
+-rw-r--r--   0        0        0     1019 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/hline.py
+-rw-r--r--   0        0        0     3643 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/interdigital_capacitor.py
+-rw-r--r--   0        0        0     1799 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/litho_calipers.py
+-rw-r--r--   0        0        0     1218 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/litho_ruler.py
+-rw-r--r--   0        0        0     1278 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/litho_steps.py
+-rw-r--r--   0        0        0      650 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/logo.py
+-rw-r--r--   0        0        0     1679 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/loop_mirror.py
+-rw-r--r--   0        0        0     5005 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mmi.py
+-rw-r--r--   0        0        0     3978 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mmi1x2.py
+-rw-r--r--   0        0        0     2769 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mmi1x2_with_sbend.py
+-rw-r--r--   0        0        0     3801 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mmi2x2.py
+-rw-r--r--   0        0        0     3192 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mmi2x2_with_sbend.py
+-rw-r--r--   0        0        0     4944 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mmi_90degree_hybrid.py
+-rw-r--r--   0        0        0     3293 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mode_converter.py
+-rw-r--r--   0        0        0     7610 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mzi.py
+-rw-r--r--   0        0        0     2464 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mzi_arm.py
+-rw-r--r--   0        0        0     5822 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mzi_arms.py
+-rw-r--r--   0        0        0    12188 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mzi_lattice.py
+-rw-r--r--   0        0        0     4020 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mzi_pads_center.py
+-rw-r--r--   0        0        0     1264 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mzi_phase_shifter.py
+-rw-r--r--   0        0        0     6310 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mzit.py
+-rw-r--r--   0        0        0     3476 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mzit_lattice.py
+-rw-r--r--   0        0        0     6016 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/mzm.py
+-rw-r--r--   0        0        0     3518 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/nxn.py
+-rw-r--r--   0        0        0     1940 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/optimal_90deg.py
+-rw-r--r--   0        0        0     3876 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/optimal_hairpin.py
+-rw-r--r--   0        0        0     6131 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/optimal_step.py
+-rw-r--r--   0        0        0     6289 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/pack_doe.py
+-rw-r--r--   0        0        0     3833 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/pad.py
+-rw-r--r--   0        0        0     1915 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/pad_gsg.py
+-rw-r--r--   0        0        0     1157 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/pads_shorted.py
+-rw-r--r--   0        0        0     3799 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/polarization_splitter_rotator.py
+-rw-r--r--   0        0        0     1115 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ramp.py
+-rw-r--r--   0        0        0     1475 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/rectangle.py
+-rw-r--r--   0        0        0     2933 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/rectangle_with_slits.py
+-rw-r--r--   0        0        0     1059 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/rectangular_ring.py
+-rw-r--r--   0        0        0     1476 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/regular_polygon.py
+-rw-r--r--   0        0        0     3276 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/resistance_meander.py
+-rw-r--r--   0        0        0     2629 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/resistance_sheet.py
+-rw-r--r--   0        0        0     1260 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring.py
+-rw-r--r--   0        0        0     4118 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_crow.py
+-rw-r--r--   0        0        0     3247 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_crow_couplers.py
+-rw-r--r--   0        0        0     2348 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_double.py
+-rw-r--r--   0        0        0     2846 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_double_bend_coupler.py
+-rw-r--r--   0        0        0     5102 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_double_heater.py
+-rw-r--r--   0        0        0     7747 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_double_pn.py
+-rw-r--r--   0        0        0    12046 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_section_based.py
+-rw-r--r--   0        0        0     2909 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_single.py
+-rw-r--r--   0        0        0     1923 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_single_array.py
+-rw-r--r--   0        0        0     6868 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_single_bend_coupler.py
+-rw-r--r--   0        0        0     2743 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_single_dut.py
+-rw-r--r--   0        0        0     4231 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_single_heater.py
+-rw-r--r--   0        0        0     5307 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/ring_single_pn.py
+-rw-r--r--   0        0        0     2281 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/seal_ring.py
+-rw-r--r--   0        0        0     3745 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/snspd.py
+-rw-r--r--   0        0        0     2059 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/spiral_double.py
+-rw-r--r--   0        0        0     5832 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/spiral_external_io.py
+-rw-r--r--   0        0        0    16624 2023-08-05 19:31:52.227140 gdsfactory-7.1.0/gdsfactory/components/spiral_heater.py
+-rw-r--r--   0        0        0     9155 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/spiral_inner_io.py
+-rw-r--r--   0        0        0     1733 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/splitter_chain.py
+-rw-r--r--   0        0        0     5289 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/splitter_tree.py
+-rw-r--r--   0        0        0     2640 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight.py
+-rw-r--r--   0        0        0     1033 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight_array.py
+-rw-r--r--   0        0        0     7863 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight_heater_doped_rib.py
+-rw-r--r--   0        0        0     1922 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight_heater_doped_strip.py
+-rw-r--r--   0        0        0     8266 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight_heater_meander.py
+-rw-r--r--   0        0        0     8519 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight_heater_meander_doped.py
+-rw-r--r--   0        0        0     6044 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight_heater_metal.py
+-rw-r--r--   0        0        0     2805 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight_pin.py
+-rw-r--r--   0        0        0     3955 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight_pin_slot.py
+-rw-r--r--   0        0        0      656 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/straight_rib.py
+-rw-r--r--   0        0        0      821 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/switch_tree.py
+-rw-r--r--   0        0        0     7973 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/taper.py
+-rw-r--r--   0        0        0     3539 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/taper_adiabatic.py
+-rw-r--r--   0        0        0     2801 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/taper_cross_section.py
+-rw-r--r--   0        0        0     2363 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/taper_from_csv.py
+-rw-r--r--   0        0        0     1235 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/taper_parabolic.py
+-rw-r--r--   0        0        0     1787 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/terminator.py
+-rw-r--r--   0        0        0     2887 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/text.py
+-rw-r--r--   0        0        0     3886 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/text_freetype.py
+-rw-r--r--   0        0        0     3186 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/text_rectangular.py
+-rw-r--r--   0        0        0     3897 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/text_rectangular_font.py
+-rw-r--r--   0        0        0     2536 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/triangles.py
+-rw-r--r--   0        0        0      715 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/verniers.py
+-rw-r--r--   0        0        0     2430 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/version_stamp.py
+-rw-r--r--   0        0        0     2413 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/via.py
+-rw-r--r--   0        0        0     3034 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/via_corner.py
+-rw-r--r--   0        0        0     5342 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/via_cutback.py
+-rw-r--r--   0        0        0    15895 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/via_stack.py
+-rw-r--r--   0        0        0     4516 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/via_stack_slot.py
+-rw-r--r--   0        0        0     4918 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/via_stack_with_offset.py
+-rw-r--r--   0        0        0     1065 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/wafer.py
+-rw-r--r--   0        0        0     7181 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/wire.py
+-rw-r--r--   0        0        0      978 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/components/wire_sbend.py
+-rw-r--r--   0        0        0    10085 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/config.py
+-rw-r--r--   0        0        0    38409 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/constants.py
+-rw-r--r--   0        0        0    83618 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/cross_section.py
+-rw-r--r--   0        0        0     2963 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/decorators.py
+-rw-r--r--   0        0        0     8406 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/difftest.py
+-rw-r--r--   0        0        0      668 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/difftest_git.py
+-rw-r--r--   0        0        0     1029 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/events.py
+-rw-r--r--   0        0        0      267 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/export/__init__.py
+-rw-r--r--   0        0        0     3308 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/export/to_3d.py
+-rw-r--r--   0        0        0     7531 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/export/to_gerber.py
+-rw-r--r--   0        0        0     1908 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/export/to_np.py
+-rw-r--r--   0        0        0     3095 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/export/to_stl.py
+-rw-r--r--   0        0        0    11831 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/fill.py
+-rw-r--r--   0        0        0     7780 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/font.py
+-rw-r--r--   0        0        0     8067 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/functions.py
+-rw-r--r--   0        0        0     1025 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/README.md
+-rw-r--r--   0        0        0     1957 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/__init__.py
+-rw-r--r--   0        0        0     1008 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/containers.py
+-rw-r--r--   0        0        0      169 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/generic_tech.sh
+-rw-r--r--   0        0        0     8117 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/get_klayout_pyxs.py
+-rw-r--r--   0        0        0      161 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/README.md
+-rw-r--r--   0        0        0      104 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/drc/Makefile
+-rw-r--r--   0        0        0        0 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/drc/__init__.py
+-rw-r--r--   0        0        0     2842 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/drc/errors.py
+-rw-r--r--   0        0        0     6192 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/grain.xml
+-rw-r--r--   0        0        0    10140 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/icon_128x128.png
+-rw-r--r--   0        0        0     4248 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/icon_64x64.png
+-rw-r--r--   0        0        0       27 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/.gitignore
+-rw-r--r--   0        0        0      494 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/Makefile
+-rw-r--r--   0        0        0     4062 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/README.md
+-rw-r--r--   0        0        0     2419 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
+-rw-r--r--   0        0        0     9696 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
+-rw-r--r--   0        0        0    12379 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
+-rw-r--r--   0        0        0     7235 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
+-rw-r--r--   0        0        0     3446 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
+-rw-r--r--   0        0        0      479 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
+-rw-r--r--   0        0        0      582 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
+-rw-r--r--   0        0        0      108 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
+-rw-r--r--   0        0        0      186 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
+-rw-r--r--   0        0        0      398 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
+-rw-r--r--   0        0        0      574 2023-08-05 19:31:52.231140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
+-rw-r--r--   0        0        0     6034 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
+-rw-r--r--   0        0        0    10697 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
+-rw-r--r--   0        0        0      477 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
+-rw-r--r--   0        0        0     4338 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
+-rw-r--r--   0        0        0      926 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
+-rw-r--r--   0        0        0    10945 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
+-rw-r--r--   0        0        0      709 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0      538 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
+-rw-r--r--   0        0        0        0 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/python/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
+-rw-r--r--   0        0        0     4312 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
+-rw-r--r--   0        0        0      269 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/Makefile
+-rw-r--r--   0        0        0     1800 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
+-rw-r--r--   0        0        0     1519 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
+-rw-r--r--   0        0        0    41073 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
+-rw-r--r--   0        0        0    40616 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/layers.lyp
+-rw-r--r--   0        0        0     5977 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/tech.lyt
+-rw-r--r--   0        0        0     4258 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
+-rw-r--r--   0        0        0     4537 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
+-rw-r--r--   0        0        0     4690 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
+-rw-r--r--   0        0        0     5508 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
+-rw-r--r--   0        0        0     1857 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/layer_map.py
+-rw-r--r--   0        0        0    10460 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/layer_stack.py
+-rw-r--r--   0        0        0    10780 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/layer_views.yaml
+-rw-r--r--   0        0        0     3916 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/generic_tech/simulation_settings.py
+-rw-r--r--   0        0        0     1431 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/__init__.py
+-rw-r--r--   0        0        0     4869 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/boolean.py
+-rw-r--r--   0        0        0     3789 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/boolean_klayout.py
+-rw-r--r--   0        0        0     1862 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/boolean_polygons.py
+-rw-r--r--   0        0        0      567 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2693 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/check_exclusion.py
+-rw-r--r--   0        0        0     2803 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/check_inclusion.py
+-rw-r--r--   0        0        0     3540 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/check_space.py
+-rw-r--r--   0        0        0     1867 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/check_width.py
+-rw-r--r--   0        0        0     4954 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/fill_klayout.py
+-rw-r--r--   0        0        0     7017 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/fill_tiled.py
+-rw-r--r--   0        0        0     1655 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/fillet.py
+-rw-r--r--   0        0        0     6614 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/functions.py
+-rw-r--r--   0        0        0     2167 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/invert.py
+-rw-r--r--   0        0        0     3686 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/layer_priority.py
+-rw-r--r--   0        0        0     3055 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/manhattanize.py
+-rw-r--r--   0        0        0     4184 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/maskprep.py
+-rw-r--r--   0        0        0     4759 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/maskprep_flat.py
+-rw-r--r--   0        0        0     3248 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/offset.py
+-rw-r--r--   0        0        0     3810 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/outline.py
+-rw-r--r--   0        0        0     2465 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/trim.py
+-rw-r--r--   0        0        0     2952 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/union.py
+-rw-r--r--   0        0        0     3626 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/write_connectivity.py
+-rw-r--r--   0        0        0    10476 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/write_drc.py
+-rw-r--r--   0        0        0     1783 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/geometry/xor_diff.py
+-rw-r--r--   0        0        0     1152 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/get_factories.py
+-rw-r--r--   0        0        0    23637 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/get_netlist.py
+-rw-r--r--   0        0        0    14481 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/get_netlist_flat.py
+-rw-r--r--   0        0        0     9689 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/grid.py
+-rw-r--r--   0        0        0     5083 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/install.py
+-rw-r--r--   0        0        0     1855 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/klive.py
+-rw-r--r--   0        0        0      585 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/labels/__init__.py
+-rw-r--r--   0        0        0     3519 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/labels/add_label_yaml.py
+-rw-r--r--   0        0        0     3818 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/labels/ehva.py
+-rw-r--r--   0        0        0     3796 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/labels/merge_test_metadata.py
+-rw-r--r--   0        0        0     4644 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/labels/siepic.py
+-rw-r--r--   0        0        0     4840 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/labels/write_labels.py
+-rw-r--r--   0        0        0     5247 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/name.py
+-rw-r--r--   0        0        0    11574 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/pack.py
+-rw-r--r--   0        0        0    52172 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/path.py
+-rw-r--r--   0        0        0    29991 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/pdk.py
+-rw-r--r--   0        0        0     6092 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/picmodel.py
+-rw-r--r--   0        0        0     5029 2023-08-05 19:31:52.235140 gdsfactory-7.1.0/gdsfactory/pixelate.py
+-rw-r--r--   0        0        0      303 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/plugins/__init__.py
+-rw-r--r--   0        0        0     4262 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/polygon.py
+-rw-r--r--   0        0        0    32988 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/port.py
+-rw-r--r--   0        0        0    37674 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/quickplotter.py
+-rw-r--r--   0        0        0      696 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/__init__.py
+-rw-r--r--   0        0        0     1639 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/from_dphox.py
+-rw-r--r--   0        0        0     1259 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/from_gdspaths.py
+-rw-r--r--   0        0        0     1927 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/from_np.py
+-rw-r--r--   0        0        0     2773 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/from_phidl.py
+-rw-r--r--   0        0        0     4222 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/from_updk.py
+-rw-r--r--   0        0        0    37973 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/from_yaml.py
+-rw-r--r--   0        0        0     5997 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/from_yaml_template.py
+-rw-r--r--   0        0        0     5632 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/import_gds.py
+-rw-r--r--   0        0        0     3369 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/read/labels.py
+-rw-r--r--   0        0        0     1614 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/route_info.py
+-rw-r--r--   0        0        0     3767 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/__init__.py
+-rw-r--r--   0        0        0     2907 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/add_electrical_pads_shortest.py
+-rw-r--r--   0        0        0     3002 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/add_electrical_pads_top.py
+-rw-r--r--   0        0        0     3031 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/add_electrical_pads_top_dc.py
+-rw-r--r--   0        0        0     8726 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/add_fiber_array.py
+-rw-r--r--   0        0        0    10573 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/add_fiber_single.py
+-rw-r--r--   0        0        0     9220 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/add_pads.py
+-rw-r--r--   0        0        0    38995 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/all_angle.py
+-rw-r--r--   0        0        0     3879 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/auto_taper.py
+-rw-r--r--   0        0        0      981 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/factories.py
+-rw-r--r--   0        0        0     4324 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/fanout.py
+-rw-r--r--   0        0        0     2796 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/fanout2x2.py
+-rw-r--r--   0        0        0    25075 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_bundle.py
+-rw-r--r--   0        0        0     8642 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_bundle_corner.py
+-rw-r--r--   0        0        0     6904 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_bundle_from_steps.py
+-rw-r--r--   0        0        0    12925 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_bundle_from_waypoints.py
+-rw-r--r--   0        0        0     5258 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_bundle_path_length_match.py
+-rw-r--r--   0        0        0     1912 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_bundle_sbend.py
+-rw-r--r--   0        0        0    17052 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_bundle_u.py
+-rw-r--r--   0        0        0     1486 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_input_labels.py
+-rw-r--r--   0        0        0     9226 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_route.py
+-rw-r--r--   0        0        0    10829 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_route_astar.py
+-rw-r--r--   0        0        0     6090 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_route_from_steps.py
+-rw-r--r--   0        0        0     2962 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_route_sbend.py
+-rw-r--r--   0        0        0     3246 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_routes_bend180.py
+-rw-r--r--   0        0        0     1773 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/get_routes_straight.py
+-rw-r--r--   0        0        0    34260 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/manhattan.py
+-rw-r--r--   0        0        0    10037 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/path_length_matching.py
+-rw-r--r--   0        0        0    22673 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/route_fiber_array.py
+-rw-r--r--   0        0        0     8643 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/route_fiber_single.py
+-rw-r--r--   0        0        0    18074 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/route_ports_to_side.py
+-rw-r--r--   0        0        0     4341 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/route_quad.py
+-rw-r--r--   0        0        0    14296 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/route_sharp.py
+-rw-r--r--   0        0        0    10141 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/route_south.py
+-rw-r--r--   0        0        0     5040 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/sort_ports.py
+-rw-r--r--   0        0        0     2433 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/routing/utils.py
+-rw-r--r--   0        0        0     2767 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/01_component_pcell.py
+-rw-r--r--   0        0        0      646 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
+-rw-r--r--   0        0        0      974 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/01_component_pcell_with_pins.py
+-rw-r--r--   0        0        0      664 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
+-rw-r--r--   0        0        0      347 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/02_component_autoname.py
+-rw-r--r--   0        0        0      887 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/03_move.py
+-rw-r--r--   0        0        0      881 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/04_connect.py
+-rw-r--r--   0        0        0      698 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/05_remove_layers.py
+-rw-r--r--   0        0        0      925 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/06_remapping_layers.py
+-rw-r--r--   0        0        0     1081 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/07_flattening_device.py
+-rw-r--r--   0        0        0      475 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/08_group.py
+-rw-r--r--   0        0        0     1621 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/11_component_layout.py
+-rw-r--r--   0        0        0     2225 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/12_component_refs.py
+-rw-r--r--   0        0        0     1013 2023-08-05 19:31:52.239140 gdsfactory-7.1.0/gdsfactory/samples/13_component_netlist.py
+-rw-r--r--   0        0        0     2592 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/14_component_connectivity.py
+-rw-r--r--   0        0        0     1683 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/15_component_sequence1.py
+-rw-r--r--   0        0        0     1733 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/16_component_sequence2.py
+-rw-r--r--   0        0        0     1030 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/17_ports.py
+-rw-r--r--   0        0        0      272 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/18_port_markers.py
+-rw-r--r--   0        0        0      361 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/19_references.py
+-rw-r--r--   0        0        0      561 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/20_components.py
+-rw-r--r--   0        0        0      565 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/21_add_fiber_array.py
+-rw-r--r--   0        0        0      550 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/22_add_fiber_single.py
+-rw-r--r--   0        0        0      632 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/22_add_pads.py
+-rw-r--r--   0        0        0      847 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/23_reticle.py
+-rw-r--r--   0        0        0      924 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/23_reticle_passives_grid.py
+-rw-r--r--   0        0        0     1177 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/23_reticle_passives_pack.py
+-rw-r--r--   0        0        0      381 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/24_doe.py
+-rw-r--r--   0        0        0      715 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/24_doe_2.py
+-rw-r--r--   0        0        0      720 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/24_doe_3.py
+-rw-r--r--   0        0        0      306 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/25_slot_cross_section.py
+-rw-r--r--   0        0        0     1363 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/30_lidar.py
+-rw-r--r--   0        0        0     1434 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/30_lidar_pcell.py
+-rw-r--r--   0        0        0     1943 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/30_lidar_with_pads.py
+-rw-r--r--   0        0        0        0 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/__init__.py
+-rw-r--r--   0        0        0     1308 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing.py
+-rw-r--r--   0        0        0      558 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
+-rw-r--r--   0        0        0     6062 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
+-rw-r--r--   0        0        0      444 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
+-rw-r--r--   0        0        0      463 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
+-rw-r--r--   0        0        0     1552 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
+-rw-r--r--   0        0        0     1315 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
+-rw-r--r--   0        0        0      602 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
+-rw-r--r--   0        0        0     3317 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
+-rw-r--r--   0        0        0     1484 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
+-rw-r--r--   0        0        0     3045 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
+-rw-r--r--   0        0        0     3782 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
+-rw-r--r--   0        0        0     2393 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/big_device.py
+-rw-r--r--   0        0        0       19 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/Makefile
+-rw-r--r--   0        0        0        0 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/__init__.py
+-rw-r--r--   0        0        0     1129 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/benchmark/fill_demo.py
+-rw-r--r--   0        0        0      343 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
+-rw-r--r--   0        0        0      637 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/circuits/mask.pic.yml
+-rw-r--r--   0        0        0      614 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
+-rw-r--r--   0        0        0      638 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
+-rw-r--r--   0        0        0      453 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/circuits/pads.pic.yml
+-rw-r--r--   0        0        0      287 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
+-rw-r--r--   0        0        0     2296 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/drc_errors.py
+-rw-r--r--   0        0        0      989 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/drc_write.py
+-rw-r--r--   0        0        0     4494 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/layers.py
+-rw-r--r--   0        0        0      158 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/layers_sky130.py
+-rw-r--r--   0        0        0      363 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/layers_xsection.py
+-rw-r--r--   0        0        0     1065 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/lvs.py
+-rw-r--r--   0        0        0      574 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/demo/pcell.py
+-rw-r--r--   0        0        0     4174 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/netlists/mzi.yml
+-rw-r--r--   0        0        0     5840 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/netlists/mzi_full.yml
+-rw-r--r--   0        0        0        0 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/.gitignore
+-rw-r--r--   0        0        0    10939 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/00_geometry.py
+-rw-r--r--   0        0        0    13583 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/01_references.py
+-rw-r--r--   0        0        0     5845 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/02_movement.py
+-rw-r--r--   0        0        0    29824 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/03_Path_CrossSection.py
+-rw-r--r--   0        0        0     6881 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/03_cells_autoname_and_cache.py
+-rw-r--r--   0        0        0    19891 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/03_layer_stack.py
+-rw-r--r--   0        0        0    11362 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_components_geometry.py
+-rw-r--r--   0        0        0     5789 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_components_hierarchy.py
+-rw-r--r--   0        0        0     7287 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_components_pack.py
+-rw-r--r--   0        0        0     8093 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_components_shapes.py
+-rw-r--r--   0        0        0    27801 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_routing.py
+-rw-r--r--   0        0        0    10894 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_routing_electrical.py
+-rw-r--r--   0        0        0    17498 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_routing_non_manhattan.py
+-rw-r--r--   0        0        0    12399 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/07_mask.py
+-rw-r--r--   0        0        0    15157 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/08_pdk.py
+-rw-r--r--   0        0        0    11094 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/08_pdk_examples.py
+-rw-r--r--   0        0        0     8585 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/09_pdk_import.py
+-rw-r--r--   0        0        0    15897 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/10_yaml_component.py
+-rw-r--r--   0        0        0     4684 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/11_get_netlist.py
+-rw-r--r--   0        0        0     2114 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/11_get_netlist_spice.py
+-rw-r--r--   0        0        0     4477 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/21_drc.py
+-rw-r--r--   0        0        0      437 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/Makefile
+-rw-r--r--   0        0        0     6217 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/_0_python.py
+-rw-r--r--   0        0        0    16372 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/_1_git.py
+-rw-r--r--   0        0        0     1092 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/_2_klayout.py
+-rw-r--r--   0        0        0     1384 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/_3_vscode.py
+-rw-r--r--   0        0        0     8163 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/_4_gdsfactory.py
+-rw-r--r--   0        0        0     4412 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/common_mistakes.py
+-rw-r--r--   0        0        0     4018 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/dataprep.py
+-rw-r--r--   0        0        0     2660 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/declarative_cell.py
+-rw-r--r--   0        0        0    13148 2023-08-05 19:31:52.243141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/images/inkscape_align.png
+-rw-r--r--   0        0        0    14726 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/images/inkscape_distribute.png
+-rw-r--r--   0        0        0    71039 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/images/pathlength_report.png
+-rw-r--r--   0        0        0    67563 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/images/pathlength_report_highlighted.png
+-rw-r--r--   0        0        0     6500 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/rib_strip_autotransition.py
+-rw-r--r--   0        0        0      591 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back.pic.yml
+-rw-r--r--   0        0        0      726 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back2.pic.yml
+-rw-r--r--   0        0        0      822 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back3.pic.yml
+-rw-r--r--   0        0        0     1417 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles01.pic.yml
+-rw-r--r--   0        0        0     1508 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles02.pic.yml
+-rw-r--r--   0        0        0     1405 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles03.pic.yml
+-rw-r--r--   0        0        0      600 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_indirect.pic.yml
+-rw-r--r--   0        0        0      614 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_simple.pic.yml
+-rw-r--r--   0        0        0     1152 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps01.pic.yml
+-rw-r--r--   0        0        0     1066 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_final.pic.yml
+-rw-r--r--   0        0        0      778 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_initial.pic.yml
+-rw-r--r--   0        0        0     1423 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps03.pic.yml
+-rw-r--r--   0        0        0      857 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_wonky_connector.pic.yml
+-rw-r--r--   0        0        0        0 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/__init__.py
+-rw-r--r--   0        0        0     3668 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/fab_c.py
+-rw-r--r--   0        0        0      233 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/fab_c_to_updk.py
+-rw-r--r--   0        0        0      475 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/fab_d/__init__.py
+-rw-r--r--   0        0        0     1893 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
+-rw-r--r--   0        0        0     1745 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c.py
+-rw-r--r--   0        0        0       50 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
+-rw-r--r--   0        0        0       93 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
+-rw-r--r--   0        0        0       85 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
+-rw-r--r--   0        0        0      139 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
+-rw-r--r--   0        0        0       90 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
+-rw-r--r--   0        0        0      126 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
+-rw-r--r--   0        0        0       48 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
+-rw-r--r--   0        0        0     1023 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
+-rw-r--r--   0        0        0     3102 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
+-rw-r--r--   0        0        0     2419 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
+-rw-r--r--   0        0        0     1283 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
+-rw-r--r--   0        0        0     2252 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
+-rw-r--r--   0        0        0     1061 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
+-rw-r--r--   0        0        0     1054 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
+-rw-r--r--   0        0        0     2237 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
+-rw-r--r--   0        0        0     6899 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
+-rw-r--r--   0        0        0     3625 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
+-rw-r--r--   0        0        0     3603 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
+-rw-r--r--   0        0        0     6857 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
+-rw-r--r--   0        0        0      840 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
+-rw-r--r--   0        0        0     3434 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
+-rw-r--r--   0        0        0     4531 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/serialization.py
+-rw-r--r--   0        0        0     1569 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/show.py
+-rw-r--r--   0        0        0      525 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/simulation/__init__.py
+-rw-r--r--   0        0        0     1689 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/snap.py
+-rw-r--r--   0        0        0     4254 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/symbols.py
+-rw-r--r--   0        0        0      308 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/technology/__init__.py
+-rw-r--r--   0        0        0      343 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/technology/color_utils.py
+-rw-r--r--   0        0        0     7550 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/technology/klayout_tech.py
+-rw-r--r--   0        0        0     1041 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/technology/layer_map.py
+-rw-r--r--   0        0        0    19780 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/technology/layer_stack.py
+-rw-r--r--   0        0        0    41893 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/technology/layer_views.py
+-rw-r--r--   0        0        0     7428 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/technology/processes.py
+-rw-r--r--   0        0        0      674 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/technology/xml_utils.py
+-rw-r--r--   0        0        0     1413 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/technology/yaml_utils.py
+-rw-r--r--   0        0        0    11084 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/typings.py
+-rw-r--r--   0        0        0     5622 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/watch.py
+-rw-r--r--   0        0        0     7419 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/gdsfactory/write_cells.py
+-rw-r--r--   0        0        0     4328 2023-08-05 19:31:52.247141 gdsfactory-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9974 1970-01-01 00:00:00.000000 gdsfactory-7.1.0/PKG-INFO
```

### Comparing `gdsfactory-7.0.2/LICENSE` & `gdsfactory-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/README.md` & `gdsfactory-7.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gdsfactory 7.0.2
+# gdsfactory 7.1.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![Downloads](https://pepy.tech/badge/gdsfactory)](https://pepy.tech/project/gdsfactory)
@@ -56,76 +56,31 @@
 You can also access:
 
 - instructions on [how to build your own PDK](https://gdsfactory.github.io/gdsfactory/notebooks/08_pdk.html)
 - instructions on [how to import a PDK from a library of fixed GDS cells](https://gdsfactory.github.io/gdsfactory/notebooks/09_pdk_import.html)
 
 ![foundry-pdks](https://i.imgur.com/zngqi0B.png)
 
-## Installation
-
-We support Python 3.10 or 3.11, and [VSCode](https://code.visualstudio.com/) as an IDE. If you do not have Python installed, you can [download Anaconda](https://www.anaconda.com/download/).
-
-Upon Python installation, open Anaconda Prompt as Administrator and install the latest gdsfactory core conda (from the conda-forge channel) and Optional `cad` visualization extras using pip.
-
-![anaconda prompt](https://i.imgur.com/eKk2bbs.png)
-
-
-```
-conda install -c conda-forge gdsfactory -y
-pip install "gdsfactory[cad]"--upgrade
-```
-
-Then you can install Klayout-live `klive` integration in the klayout GUI `Tools --> Manage Packages --> Install New Packages --> Klive` as well as the genericpdk layermap `Tools --> Manage Packages --> Install New Packages --> gdsfactory` and restart klayout.
-
-### Update gdsfactory
-
-You can upgrade your gdsfactory package using the following command:
-
-```
-pip install gdsfactory[cad] --upgrade
-```
-
-Please note that some PDKs may only work for a specific version of gdsfactory. Ensure you install the correct gdsfactory version specified in the pyproject.toml file. This will automatically happen when you install gdsfactory as one of the PDK dependencies. For example, pip install gf180 will install the latest gdsfactory version tested for the GlobalFoundries180 PDK.
-
-To determine your current gdsfactory version, use the following code:
-
-```
-import gdsfactory as gf
-
-gf.config.print_version()
-```
-
-### Docker container
-
-As an alternative, you can use the pre-built Docker image from [hub.docker.com/r/joamatab/gdsfactory](https://hub.docker.com/r/joamatab/gdsfactory) or build it yourself with:
-
-
-```bash
-docker build -t joamatab/gdsfactory .
-```
-
-For instance, VS Code supports development inside a container. See [Developing inside a Container](https://code.visualstudio.com/docs/devcontainers/containers) for details.
-
-## Plugins
-
-We maintain gdsfactory plugins in a [separate package](https://github.com/gdsfactory/gplugins)
-These plugins enable interfaces with different tools, and you might need to install some of the tools separately.
-For more details, please visit the [gplugins documentation](https://gdsfactory.github.io/gplugins/).
 
 ## Getting started
 
 - [See slides](https://docs.google.com/presentation/d/1_ZmUxbaHWo_lQP17dlT1FWX-XD8D9w7-FcuEih48d_0/edit#slide=id.g11711f50935_0_5)
 - [Read docs](https://gdsfactory.github.io/gdsfactory/)
 - [![Video Tutorials](https://img.shields.io/badge/youtube-Video_Tutorials-red.svg?logo=youtube)](https://www.youtube.com/@gdsfactory625/playlists)
 - [![Join the chat at https://gitter.im/gdsfactory-dev/community](https://badges.gitter.im/gdsfactory-dev/community.svg)](https://gitter.im/gdsfactory-dev/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 - See announcements on [GitHub](https://github.com/gdsfactory/gdsfactory/discussions/547), [google-groups](https://groups.google.com/g/gdsfactory) or [LinkedIn](https://www.linkedin.com/company/gdsfactory)
 - Run notebooks on [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gdsfactory/binder-sandbox/HEAD)
 - [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=250169028)
 
-## Testimonals
+## Who is using gdsfactory?
+
+Hundreds of organisations are using gdsfactory. Some companies and organizations around the world using gdsfactory include:
+
+![logos](https://i.imgur.com/IqTUq9S.png)
+
 
 "I've used **gdsfactory** since 2017 for all my chip tapeouts. I love that it is fast, easy to use, and easy to extend. It's the only tool that allows us to have an end-to-end chip design flow (design, verification and validation)."
 
 <div style="text-align: right; margin-right: 10%;">Joaquin Matres - <strong>Google</strong></div>
 
 ---
```

### Comparing `gdsfactory-7.0.2/gdsfactory/__init__.py` & `gdsfactory-7.1.0/gdsfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,8 +144,8 @@
     "technology",
     "write_cells",
     "xsection",
     "PATH",
 )
 
 
-__version__ = "7.0.2"
+__version__ = "7.1.0"
```

### Comparing `gdsfactory-7.0.2/gdsfactory/add_keepout.py` & `gdsfactory-7.1.0/gdsfactory/add_keepout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/add_labels.py` & `gdsfactory-7.1.0/gdsfactory/add_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/add_loopback.py` & `gdsfactory-7.1.0/gdsfactory/add_loopback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/add_padding.py` & `gdsfactory-7.1.0/gdsfactory/add_padding.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/add_pins.py` & `gdsfactory-7.1.0/gdsfactory/add_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/add_ports.py` & `gdsfactory-7.1.0/gdsfactory/add_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/add_tapers.py` & `gdsfactory-7.1.0/gdsfactory/add_tapers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/add_tapers_cross_section.py` & `gdsfactory-7.1.0/gdsfactory/add_tapers_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/add_termination.py` & `gdsfactory-7.1.0/gdsfactory/add_termination.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/asserts.py` & `gdsfactory-7.1.0/gdsfactory/asserts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/cell.py` & `gdsfactory-7.1.0/gdsfactory/cell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/cli.py` & `gdsfactory-7.1.0/gdsfactory/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from gdsfactory.write_cells import write_cells as write_cells_to_separate_gds
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
-VERSION = "7.0.2"
+VERSION = "7.1.0"
 LAYER_LABEL = LAYER.LABEL
 
 
 def print_version(ctx: Context, param: Option, value: bool) -> None:
     """Prints the version."""
     if not value or ctx.resilient_parsing:
         return
@@ -139,15 +139,15 @@
 
     uvicorn.run(app, host=host, port=port)
 
 
 @click.argument("path", type=click.Path(exists=True), required=False, default=cwd)
 @click.command()
 def watch(path=cwd) -> None:
-    """Filewatch a folder for changes in python or pic.yaml files."""
+    """Filewatch a folder for changes in *.py or *.pic.yml files."""
     from gdsfactory.watch import watch
 
     path = pathlib.Path(path)
     path = path.parent if path.is_dir() else path
     watch(str(path))
```

### Comparing `gdsfactory-7.0.2/gdsfactory/component.py` & `gdsfactory-7.1.0/gdsfactory/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -3215,3169 +3215,3218 @@
 0000c8e0: 7274 5f6d 6172 6b65 725f 6c61 7965 723d  rt_marker_layer=
 0000c8f0: 706f 7274 5f6d 6172 6b65 725f 6c61 7965  port_marker_laye
 0000c900: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
 0000c910: 6620 7368 6f77 5f70 6f72 7473 0a20 2020  f show_ports.   
 0000c920: 2020 2020 2020 2020 2065 6c73 6520 7365           else se
 0000c930: 6c66 0a20 2020 2020 2020 2029 0a0a 2020  lf.        )..  
 0000c940: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000c950: 2020 2020 2020 2069 6d70 6f72 7420 6b6c         import kl
-0000c960: 6179 6f75 742e 6462 2061 7320 6462 2020  ayout.db as db  
-0000c970: 2320 6e6f 7161 3a20 4634 3031 0a20 2020  # noqa: F401.   
-0000c980: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
-0000c990: 6b6c 6179 6f75 742e 6c61 7920 6173 206c  klayout.lay as l
-0000c9a0: 6179 0a20 2020 2020 2020 2020 2020 2066  ay.            f
-0000c9b0: 726f 6d20 4950 7974 686f 6e2e 6469 7370  rom IPython.disp
-0000c9c0: 6c61 7920 696d 706f 7274 2064 6973 706c  lay import displ
-0000c9d0: 6179 0a20 2020 2020 2020 2020 2020 2066  ay.            f
-0000c9e0: 726f 6d20 6970 7977 6964 6765 7473 2069  rom ipywidgets i
-0000c9f0: 6d70 6f72 7420 496d 6167 650a 0a20 2020  mport Image..   
-0000ca00: 2020 2020 2020 2020 2066 726f 6d20 6764           from gd
-0000ca10: 7366 6163 746f 7279 2e70 646b 2069 6d70  sfactory.pdk imp
-0000ca20: 6f72 7420 6765 745f 6c61 7965 725f 7669  ort get_layer_vi
-0000ca30: 6577 730a 0a20 2020 2020 2020 2020 2020  ews..           
-0000ca40: 2067 6473 7061 7468 203d 2063 6f6d 706f   gdspath = compo
-0000ca50: 6e65 6e74 2e77 7269 7465 5f67 6473 286c  nent.write_gds(l
-0000ca60: 6f67 6769 6e67 3d46 616c 7365 290a 2020  ogging=False).  
-0000ca70: 2020 2020 2020 2020 2020 6c79 705f 7061            lyp_pa
-0000ca80: 7468 203d 2067 6473 7061 7468 2e77 6974  th = gdspath.wit
-0000ca90: 685f 7375 6666 6978 2822 2e6c 7970 2229  h_suffix(".lyp")
-0000caa0: 0a0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-0000cab0: 7965 725f 7669 6577 7320 3d20 6765 745f  yer_views = get_
-0000cac0: 6c61 7965 725f 7669 6577 7328 290a 2020  layer_views().  
-0000cad0: 2020 2020 2020 2020 2020 6c61 7965 725f            layer_
-0000cae0: 7669 6577 732e 746f 5f6c 7970 2866 696c  views.to_lyp(fil
-0000caf0: 6570 6174 683d 6c79 705f 7061 7468 290a  epath=lyp_path).
-0000cb00: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-0000cb10: 6f75 745f 7669 6577 203d 206c 6179 2e4c  out_view = lay.L
-0000cb20: 6179 6f75 7456 6965 7728 290a 2020 2020  ayoutView().    
-0000cb30: 2020 2020 2020 2020 6c61 796f 7574 5f76          layout_v
-0000cb40: 6965 772e 6c6f 6164 5f6c 6179 6f75 7428  iew.load_layout(
-0000cb50: 7374 7228 6764 7370 6174 682e 6162 736f  str(gdspath.abso
-0000cb60: 6c75 7465 2829 2929 0a20 2020 2020 2020  lute())).       
-0000cb70: 2020 2020 206c 6179 6f75 745f 7669 6577       layout_view
-0000cb80: 2e6d 6178 5f68 6965 7228 290a 2020 2020  .max_hier().    
-0000cb90: 2020 2020 2020 2020 6c61 796f 7574 5f76          layout_v
-0000cba0: 6965 772e 6c6f 6164 5f6c 6179 6572 5f70  iew.load_layer_p
-0000cbb0: 726f 7073 2873 7472 286c 7970 5f70 6174  rops(str(lyp_pat
-0000cbc0: 6829 290a 0a20 2020 2020 2020 2020 2020  h))..           
-0000cbd0: 206c 6179 6f75 745f 7669 6577 2e73 6574   layout_view.set
-0000cbe0: 5f63 6f6e 6669 6728 2274 6578 742d 7669  _config("text-vi
-0000cbf0: 7369 626c 6522 2c20 2274 7275 6522 2069  sible", "true" i
-0000cc00: 6620 7368 6f77 5f6c 6162 656c 7320 656c  f show_labels el
-0000cc10: 7365 2022 6661 6c73 6522 290a 0a20 2020  se "false")..   
-0000cc20: 2020 2020 2020 2020 2070 6978 656c 5f62           pixel_b
-0000cc30: 7566 6665 7220 3d20 6c61 796f 7574 5f76  uffer = layout_v
-0000cc40: 6965 772e 6765 745f 7069 7865 6c73 5f77  iew.get_pixels_w
-0000cc50: 6974 685f 6f70 7469 6f6e 7328 3830 302c  ith_options(800,
-0000cc60: 2036 3030 290a 2020 2020 2020 2020 2020   600).          
-0000cc70: 2020 706e 675f 6461 7461 203d 2070 6978    png_data = pix
-0000cc80: 656c 5f62 7566 6665 722e 746f 5f70 6e67  el_buffer.to_png
-0000cc90: 5f64 6174 6128 290a 2020 2020 2020 2020  _data().        
-0000cca0: 2020 2020 696d 6167 6520 3d20 496d 6167      image = Imag
-0000ccb0: 6528 7661 6c75 653d 706e 675f 6461 7461  e(value=png_data
-0000ccc0: 2c20 666f 726d 6174 3d22 706e 6722 290a  , format="png").
-0000ccd0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-0000cce0: 6c61 7928 696d 6167 6529 0a0a 2020 2020  lay(image)..    
-0000ccf0: 2020 2020 6578 6365 7074 2049 6d70 6f72      except Impor
-0000cd00: 7445 7272 6f72 3a0a 2020 2020 2020 2020  tError:.        
-0000cd10: 2020 2020 7072 696e 7428 2259 6f75 2063      print("You c
-0000cd20: 616e 2069 6e73 7461 6c6c 2060 7069 7020  an install `pip 
-0000cd30: 696e 7374 616c 6c20 6764 7366 6163 746f  install gdsfacto
-0000cd40: 7279 6020 666f 7220 6265 7474 6572 2076  ry` for better v
-0000cd50: 6973 7561 6c69 7a61 7469 6f6e 2229 0a20  isualization"). 
-0000cd60: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
-0000cd70: 6e65 6e74 2e70 6c6f 7428 706c 6f74 7465  nent.plot(plotte
-0000cd80: 723d 226d 6174 706c 6f74 6c69 6222 290a  r="matplotlib").
-0000cd90: 0a20 2020 2064 6566 2070 6c6f 745f 6b77  .    def plot_kw
-0000cda0: 6562 2873 656c 6629 3a0a 2020 2020 2020  eb(self):.      
-0000cdb0: 2020 2222 2253 686f 7773 2063 7572 7265    """Shows curre
-0000cdc0: 6e74 2067 6473 2069 6e20 6b77 6562 2e22  nt gds in kweb."
-0000cdd0: 2222 0a20 2020 2020 2020 2069 6d70 6f72  "".        impor
-0000cde0: 7420 6f73 0a20 2020 2020 2020 2066 726f  t os.        fro
-0000cdf0: 6d20 6874 6d6c 2069 6d70 6f72 7420 6573  m html import es
-0000ce00: 6361 7065 0a0a 2020 2020 2020 2020 696d  cape..        im
-0000ce10: 706f 7274 206b 7765 622e 7365 7276 6572  port kweb.server
-0000ce20: 5f6a 7570 7974 6572 2061 7320 6b6a 0a20  _jupyter as kj. 
-0000ce30: 2020 2020 2020 2066 726f 6d20 4950 7974         from IPyt
-0000ce40: 686f 6e2e 6469 7370 6c61 7920 696d 706f  hon.display impo
-0000ce50: 7274 2049 4672 616d 650a 0a20 2020 2020  rt IFrame..     
-0000ce60: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
-0000ce70: 7279 2e63 6f6e 6669 6720 696d 706f 7274  ry.config import
-0000ce80: 2050 4154 480a 2020 2020 2020 2020 6672   PATH.        fr
-0000ce90: 6f6d 2067 6473 6661 6374 6f72 792e 7064  om gdsfactory.pd
-0000cea0: 6b20 696d 706f 7274 2067 6574 5f6c 6179  k import get_lay
-0000ceb0: 6572 5f76 6965 7773 0a0a 2020 2020 2020  er_views..      
-0000cec0: 2020 6764 7370 6174 6820 3d20 7365 6c66    gdspath = self
-0000ced0: 2e77 7269 7465 5f67 6473 2867 6473 6469  .write_gds(gdsdi
-0000cee0: 723d 5041 5448 2e67 6473 6c69 6220 2f20  r=PATH.gdslib / 
-0000cef0: 2265 7874 7261 222c 206c 6f67 6769 6e67  "extra", logging
-0000cf00: 3d46 616c 7365 290a 0a20 2020 2020 2020  =False)..       
-0000cf10: 2064 6972 7061 7468 203d 2047 4453 4449   dirpath = GDSDI
-0000cf20: 525f 5445 4d50 0a20 2020 2020 2020 2064  R_TEMP.        d
-0000cf30: 6972 7061 7468 2e6d 6b64 6972 2865 7869  irpath.mkdir(exi
-0000cf40: 7374 5f6f 6b3d 5472 7565 2c20 7061 7265  st_ok=True, pare
-0000cf50: 6e74 733d 5472 7565 290a 2020 2020 2020  nts=True).      
-0000cf60: 2020 6c79 705f 7061 7468 203d 2064 6972    lyp_path = dir
-0000cf70: 7061 7468 202f 2022 6c61 7965 7273 2e6c  path / "layers.l
-0000cf80: 7970 220a 0a20 2020 2020 2020 206c 6179  yp"..        lay
-0000cf90: 6572 5f70 726f 7073 203d 2067 6574 5f6c  er_props = get_l
-0000cfa0: 6179 6572 5f76 6965 7773 2829 0a20 2020  ayer_views().   
-0000cfb0: 2020 2020 206c 6179 6572 5f70 726f 7073       layer_props
-0000cfc0: 2e74 6f5f 6c79 7028 6669 6c65 7061 7468  .to_lyp(filepath
-0000cfd0: 3d6c 7970 5f70 6174 6829 0a0a 2020 2020  =lyp_path)..    
-0000cfe0: 2020 2020 706f 7274 203d 206b 6a2e 706f      port = kj.po
-0000cff0: 7274 2069 6620 6861 7361 7474 7228 6b6a  rt if hasattr(kj
-0000d000: 2c20 2270 6f72 7422 2920 616e 6420 6b6a  , "port") and kj
-0000d010: 2e70 6f72 7420 656c 7365 2038 3030 300a  .port else 8000.
-0000d020: 2020 2020 2020 2020 7372 6320 3d20 6622          src = f"
-0000d030: 6874 7470 3a2f 2f31 3237 2e30 2e30 2e31  http://127.0.0.1
-0000d040: 3a7b 706f 7274 7d2f 6764 733f 6764 735f  :{port}/gds?gds_
-0000d050: 6669 6c65 3d7b 6573 6361 7065 2873 7472  file={escape(str
-0000d060: 2867 6473 7061 7468 2929 7d26 6c61 7965  (gdspath))}&laye
-0000d070: 725f 7072 6f70 733d 7b65 7363 6170 6528  r_props={escape(
-0000d080: 7374 7228 6c79 705f 7061 7468 2929 7d22  str(lyp_path))}"
-0000d090: 0a0a 2020 2020 2020 2020 6f73 2e65 6e76  ..        os.env
-0000d0a0: 6972 6f6e 5b22 4b57 4542 5f50 4f52 5422  iron["KWEB_PORT"
-0000d0b0: 5d20 3d20 7374 7228 6f73 2e67 6574 656e  ] = str(os.geten
-0000d0c0: 7628 224b 5745 425f 504f 5254 222c 2070  v("KWEB_PORT", p
-0000d0d0: 6f72 7429 290a 0a20 2020 2020 2020 2069  ort))..        i
-0000d0e0: 6620 6e6f 7420 6b6a 2e6a 7570 7974 6572  f not kj.jupyter
-0000d0f0: 5f73 6572 7665 723a 0a20 2020 2020 2020  _server:.       
-0000d100: 2020 2020 2070 6f72 7420 3d20 696e 7428       port = int(
-0000d110: 6f73 2e67 6574 656e 7628 224b 5745 425f  os.getenv("KWEB_
-0000d120: 504f 5254 2229 290a 2020 2020 2020 2020  PORT")).        
-0000d130: 2020 2020 7768 696c 6520 6b6a 2e69 735f      while kj.is_
-0000d140: 706f 7274 5f69 6e5f 7573 6528 706f 7274  port_in_use(port
-0000d150: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000d160: 2020 2070 6f72 7420 2b3d 2031 0a0a 2020     port += 1..  
-0000d170: 2020 2020 2020 2020 2020 6f73 2e65 6e76            os.env
-0000d180: 6972 6f6e 5b22 4b57 4542 5f50 4f52 5422  iron["KWEB_PORT"
-0000d190: 5d20 3d20 7374 7228 706f 7274 290a 2020  ] = str(port).  
-0000d1a0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000d1b0: 2e64 6562 7567 2873 7263 290a 2020 2020  .debug(src).    
-0000d1c0: 2020 2020 2020 2020 6b6a 2e73 7461 7274          kj.start
-0000d1d0: 2829 0a0a 2020 2020 2020 2020 6966 206b  ()..        if k
-0000d1e0: 6a2e 6a75 7079 7465 725f 7365 7276 6572  j.jupyter_server
-0000d1f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000d200: 7475 726e 2049 4672 616d 6528 0a20 2020  turn IFrame(.   
-0000d210: 2020 2020 2020 2020 2020 2020 2073 7263               src
-0000d220: 3d73 7263 2c0a 2020 2020 2020 2020 2020  =src,.          
-0000d230: 2020 2020 2020 7769 6474 683d 3134 3030        width=1400
-0000d240: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d250: 2020 6865 6967 6874 3d36 3030 2c0a 2020    height=600,.  
-0000d260: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000d270: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000d280: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000d290: 662e 706c 6f74 5f6b 6c61 796f 7574 2829  f.plot_klayout()
-0000d2a0: 0a0a 2020 2020 6465 6620 706c 6f74 5f6d  ..    def plot_m
-0000d2b0: 6174 706c 6f74 6c69 6228 7365 6c66 2c20  atplotlib(self, 
-0000d2c0: 2a2a 6b77 6172 6773 2920 2d3e 204e 6f6e  **kwargs) -> Non
-0000d2d0: 653a 0a20 2020 2020 2020 2022 2222 506c  e:.        """Pl
-0000d2e0: 6f74 2063 6f6d 706f 6e65 6e74 2075 7369  ot component usi
-0000d2f0: 6e67 206d 6174 706c 6f74 6c69 622e 0a0a  ng matplotlib...
-0000d300: 2020 2020 2020 2020 4b65 7977 6f72 6420          Keyword 
-0000d310: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000d320: 2020 7368 6f77 5f70 6f72 7473 3a20 5365    show_ports: Se
-0000d330: 7473 2077 6865 7468 6572 2070 6f72 7473  ts whether ports
-0000d340: 2061 7265 2064 7261 776e 2e0a 2020 2020   are drawn..    
-0000d350: 2020 2020 2020 2020 7368 6f77 5f73 7562          show_sub
-0000d360: 706f 7274 733a 2053 6574 7320 7768 6574  ports: Sets whet
-0000d370: 6865 7220 7375 6270 6f72 7473 2028 706f  her subports (po
-0000d380: 7274 7320 7468 6174 2062 656c 6f6e 6720  rts that belong 
-0000d390: 746f 2072 6566 6572 656e 6365 7329 2061  to references) a
-0000d3a0: 7265 2064 7261 776e 2e0a 2020 2020 2020  re drawn..      
-0000d3b0: 2020 2020 2020 6c61 6265 6c5f 616c 6961        label_alia
-0000d3c0: 7365 733a 2053 6574 7320 7768 6574 6865  ses: Sets whethe
-0000d3d0: 7220 616c 6961 7365 7320 6172 6520 6c61  r aliases are la
-0000d3e0: 6265 6c65 6420 7769 7468 2061 2074 6578  beled with a tex
-0000d3f0: 7420 6e61 6d65 2e0a 2020 2020 2020 2020  t name..        
-0000d400: 2020 2020 6e65 775f 7769 6e64 6f77 3a20      new_window: 
-0000d410: 4966 2054 7275 652c 2065 6163 6820 6361  If True, each ca
-0000d420: 6c6c 2074 6f20 7175 6963 6b70 6c6f 7428  ll to quickplot(
-0000d430: 2920 7769 6c6c 2067 656e 6572 6174 6520  ) will generate 
-0000d440: 6120 7365 7061 7261 7465 2077 696e 646f  a separate windo
-0000d450: 772e 0a20 2020 2020 2020 2020 2020 2062  w..            b
-0000d460: 6c6f 636b 696e 673a 2049 6620 5472 7565  locking: If True
-0000d470: 2c20 6361 6c6c 696e 6720 7175 6963 6b70  , calling quickp
-0000d480: 6c6f 7428 2920 7769 6c6c 2070 6175 7365  lot() will pause
-0000d490: 2065 7865 6375 7469 6f6e 206f 6620 2822   execution of ("
-0000d4a0: 626c 6f63 6b22 2920 7468 650a 2020 2020  block") the.    
-0000d4b0: 2020 2020 2020 2020 2020 2020 7265 6d61              rema
-0000d4c0: 696e 6465 7220 6f66 2074 6865 2070 7974  inder of the pyt
-0000d4d0: 686f 6e20 636f 6465 2075 6e74 696c 2074  hon code until t
-0000d4e0: 6865 2071 7569 636b 706c 6f74 2829 2077  he quickplot() w
-0000d4f0: 696e 646f 7720 6973 2063 6c6f 7365 642e  indow is closed.
-0000d500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d510: 2049 6620 4661 6c73 652c 2074 6865 2077   If False, the w
-0000d520: 696e 646f 7720 7769 6c6c 2062 6520 6f70  indow will be op
-0000d530: 656e 6564 2061 6e64 2063 6f64 6520 7769  ened and code wi
-0000d540: 6c6c 2063 6f6e 7469 6e75 6520 746f 2072  ll continue to r
-0000d550: 756e 2e0a 2020 2020 2020 2020 2020 2020  un..            
-0000d560: 7a6f 6f6d 5f66 6163 746f 723a 2053 6574  zoom_factor: Set
-0000d570: 7320 7468 6520 7363 616c 696e 6720 6661  s the scaling fa
-0000d580: 6374 6f72 2077 6865 6e20 7a6f 6f6d 696e  ctor when zoomin
-0000d590: 6720 7468 6520 7175 6963 6b70 6c6f 7420  g the quickplot 
-0000d5a0: 7769 6e64 6f77 2077 6974 6820 7468 650a  window with the.
-0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5c0: 6d6f 7573 6577 6865 656c 2f74 7261 636b  mousewheel/track
-0000d5d0: 7061 642e 0a20 2020 2020 2020 2020 2020  pad..           
-0000d5e0: 2069 6e74 6572 6163 7469 7665 5f7a 6f6f   interactive_zoo
-0000d5f0: 6d3a 2045 6e61 626c 6573 2075 7369 6e67  m: Enables using
-0000d600: 206d 6f75 7365 7768 6565 6c2f 7472 6163   mousewheel/trac
-0000d610: 6b70 6164 2074 6f20 7a6f 6f6d 2e0a 2020  kpad to zoom..  
-0000d620: 2020 2020 2020 2020 2020 666f 6e74 7369            fontsi
-0000d630: 7a65 3a20 666f 7220 6c61 6265 6c73 2e0a  ze: for labels..
-0000d640: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-0000d650: 7273 5f65 7863 6c75 6465 643a 206c 6973  rs_excluded: lis
-0000d660: 7420 6f66 206c 6179 6572 7320 746f 2065  t of layers to e
-0000d670: 7863 6c75 6465 2e0a 2020 2020 2020 2020  xclude..        
-0000d680: 2020 2020 6c61 7965 725f 7669 6577 733a      layer_views:
-0000d690: 206c 6179 6572 5f76 6965 7773 2063 6f6c   layer_views col
-0000d6a0: 6f72 7320 6c6f 6164 6564 2066 726f 6d20  ors loaded from 
-0000d6b0: 4b6c 6179 6f75 742e 0a20 2020 2020 2020  Klayout..       
-0000d6c0: 2020 2020 206d 696e 5f61 7370 6563 743a       min_aspect:
-0000d6d0: 206d 696e 696d 756d 2061 7370 6563 7420   minimum aspect 
-0000d6e0: 7261 7469 6f2e 0a20 2020 2020 2020 2022  ratio..        "
-0000d6f0: 2222 0a20 2020 2020 2020 2066 726f 6d20  "".        from 
-0000d700: 6764 7366 6163 746f 7279 2e71 7569 636b  gdsfactory.quick
-0000d710: 706c 6f74 7465 7220 696d 706f 7274 2071  plotter import q
-0000d720: 7569 636b 706c 6f74 0a0a 2020 2020 2020  uickplot..      
-0000d730: 2020 7175 6963 6b70 6c6f 7428 7365 6c66    quickplot(self
-0000d740: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
-0000d750: 2064 6566 2070 6c6f 7428 7365 6c66 2c20   def plot(self, 
-0000d760: 706c 6f74 7465 723a 2073 7472 207c 204e  plotter: str | N
-0000d770: 6f6e 6520 3d20 4e6f 6e65 2c20 2a2a 6b77  one = None, **kw
-0000d780: 6172 6773 293a 0a20 2020 2020 2020 2022  args):.        "
-0000d790: 2222 5265 7475 726e 7320 636f 6d70 6f6e  ""Returns compon
-0000d7a0: 656e 7420 706c 6f74 2075 7369 6e67 206b  ent plot using k
-0000d7b0: 6c61 796f 7574 2c20 6d61 7470 6c6f 746c  layout, matplotl
-0000d7c0: 6962 2c20 686f 6c6f 7669 6577 7320 6f72  ib, holoviews or
-0000d7d0: 2071 742e 0a0a 2020 2020 2020 2020 5765   qt...        We
-0000d7e0: 2072 6563 6f6d 6d65 6e64 2075 7369 6e67   recommend using
-0000d7f0: 206b 6c61 796f 7574 2e0a 0a20 2020 2020   klayout...     
-0000d800: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000d810: 2020 2020 2070 6c6f 7474 6572 3a20 706c       plotter: pl
-0000d820: 6f74 2062 6163 6b65 6e64 2028 276d 6174  ot backend ('mat
-0000d830: 706c 6f74 6c69 6227 2c20 2777 6964 6765  plotlib', 'widge
-0000d840: 7427 2c20 276b 6c61 796f 7574 272c 2027  t', 'klayout', '
-0000d850: 6b77 6562 2729 2e0a 2020 2020 2020 2020  kweb')..        
-0000d860: 2222 220a 2020 2020 2020 2020 706c 6f74  """.        plot
-0000d870: 7465 7220 3d20 706c 6f74 7465 7220 6f72  ter = plotter or
-0000d880: 2043 4f4e 462e 6469 7370 6c61 795f 7479   CONF.display_ty
-0000d890: 7065 0a0a 2020 2020 2020 2020 6966 2070  pe..        if p
-0000d8a0: 6c6f 7474 6572 206e 6f74 2069 6e20 7661  lotter not in va
-0000d8b0: 6c69 645f 706c 6f74 7465 7273 3a0a 2020  lid_plotters:.  
-0000d8c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000d8d0: 5661 6c75 6545 7272 6f72 2866 227b 706c  ValueError(f"{pl
-0000d8e0: 6f74 7465 7221 727d 206e 6f74 2069 6e20  otter!r} not in 
-0000d8f0: 7b76 616c 6964 5f70 6c6f 7474 6572 737d  {valid_plotters}
-0000d900: 2229 0a0a 2020 2020 2020 2020 6966 2070  ")..        if p
-0000d910: 6c6f 7474 6572 203d 3d20 226b 6c61 796f  lotter == "klayo
-0000d920: 7574 223a 0a20 2020 2020 2020 2020 2020  ut":.           
-0000d930: 2073 656c 662e 706c 6f74 5f6b 6c61 796f   self.plot_klayo
-0000d940: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
-0000d950: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000d960: 656c 6966 2070 6c6f 7474 6572 203d 3d20  elif plotter == 
-0000d970: 226b 7765 6222 3a0a 2020 2020 2020 2020  "kweb":.        
-0000d980: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000d990: 706c 6f74 5f6b 7765 6228 290a 2020 2020  plot_kweb().    
-0000d9a0: 2020 2020 656c 6966 2070 6c6f 7474 6572      elif plotter
-0000d9b0: 203d 3d20 2277 6964 6765 7422 3a0a 2020   == "widget":.  
-0000d9c0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000d9d0: 6c6f 745f 7769 6467 6574 2829 0a20 2020  lot_widget().   
-0000d9e0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000d9f0: 0a20 2020 2020 2020 2065 6c69 6620 706c  .        elif pl
-0000da00: 6f74 7465 7220 3d3d 2022 6d61 7470 6c6f  otter == "matplo
-0000da10: 746c 6962 223a 0a20 2020 2020 2020 2020  tlib":.         
-0000da20: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
-0000da30: 7279 2e71 7569 636b 706c 6f74 7465 7220  ry.quickplotter 
-0000da40: 696d 706f 7274 2071 7569 636b 706c 6f74  import quickplot
-0000da50: 0a0a 2020 2020 2020 2020 2020 2020 7175  ..            qu
-0000da60: 6963 6b70 6c6f 7428 7365 6c66 2c20 2a2a  ickplot(self, **
-0000da70: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
-0000da80: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
-0000da90: 2020 2020 656c 6966 2070 6c6f 7474 6572      elif plotter
-0000daa0: 203d 3d20 2268 6f6c 6f76 6965 7773 223a   == "holoviews":
-0000dab0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-0000dac0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000dad0: 2020 696d 706f 7274 2068 6f6c 6f76 6965    import holovie
-0000dae0: 7773 2061 7320 6876 0a0a 2020 2020 2020  ws as hv..      
-0000daf0: 2020 2020 2020 2020 2020 6876 2e65 7874            hv.ext
-0000db00: 656e 7369 6f6e 2822 626f 6b65 6822 290a  ension("bokeh").
-0000db10: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0000db20: 7074 2049 6d70 6f72 7445 7272 6f72 2061  pt ImportError a
-0000db30: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0000db40: 2020 2020 2070 7269 6e74 2822 796f 7520       print("you 
-0000db50: 6e65 6564 2074 6f20 6070 6970 2069 6e73  need to `pip ins
-0000db60: 7461 6c6c 2068 6f6c 6f76 6965 7773 6022  tall holoviews`"
-0000db70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000db80: 2020 7261 6973 6520 650a 2020 2020 2020    raise e.      
-0000db90: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000dba0: 662e 706c 6f74 5f68 6f6c 6f76 6965 7773  f.plot_holoviews
-0000dbb0: 282a 2a6b 7761 7267 7329 0a0a 2020 2020  (**kwargs)..    
-0000dbc0: 2020 2020 656c 6966 2070 6c6f 7474 6572      elif plotter
-0000dbd0: 203d 3d20 2271 7422 3a0a 2020 2020 2020   == "qt":.      
-0000dbe0: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-0000dbf0: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
-0000dc00: 2020 2020 2022 7174 2070 6c6f 7474 6572       "qt plotter
-0000dc10: 2069 7320 6465 7072 6563 6174 6564 2e20   is deprecated. 
-0000dc20: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000dc30: 2020 2255 7365 2074 6865 2064 6566 6175    "Use the defau
-0000dc40: 6c74 2043 6f6d 706f 6e65 6e74 2e70 6c6f  lt Component.plo
-0000dc50: 7428 292c 2043 6f6d 706f 6e65 6e74 2e70  t(), Component.p
-0000dc60: 6c6f 745f 6b6c 6179 6f75 7428 2920 6f72  lot_klayout() or
-0000dc70: 2043 6f6d 706f 6e65 6e74 2e70 6c6f 745f   Component.plot_
-0000dc80: 7769 6467 6574 2829 222c 0a20 2020 2020  widget()",.     
-0000dc90: 2020 2020 2020 2020 2020 2073 7461 636b             stack
-0000dca0: 6c65 7665 6c3d 332c 0a20 2020 2020 2020  level=3,.       
-0000dcb0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000dcc0: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
-0000dcd0: 7279 2e71 7569 636b 706c 6f74 7465 7220  ry.quickplotter 
-0000dce0: 696d 706f 7274 2071 7569 636b 706c 6f74  import quickplot
-0000dcf0: 320a 0a20 2020 2020 2020 2020 2020 2071  2..            q
-0000dd00: 7569 636b 706c 6f74 3228 7365 6c66 290a  uickplot2(self).
-0000dd10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000dd20: 726e 0a0a 2020 2020 6465 6620 706c 6f74  rn..    def plot
-0000dd30: 5f68 6f6c 6f76 6965 7773 280a 2020 2020  _holoviews(.    
-0000dd40: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000dd50: 2020 6c61 7965 7273 5f65 7863 6c75 6465    layers_exclude
-0000dd60: 643a 204c 6179 6572 7320 7c20 4e6f 6e65  d: Layers | None
-0000dd70: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000dd80: 206c 6179 6572 5f76 6965 7773 3a20 4c61   layer_views: La
-0000dd90: 7965 7256 6965 7773 207c 204e 6f6e 6520  yerViews | None 
-0000dda0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000ddb0: 6d69 6e5f 6173 7065 6374 3a20 666c 6f61  min_aspect: floa
-0000ddc0: 7420 3d20 302e 3235 2c0a 2020 2020 2020  t = 0.25,.      
-0000ddd0: 2020 7061 6464 696e 673a 2066 6c6f 6174    padding: float
-0000dde0: 203d 2030 2e35 2c0a 2020 2020 293a 0a20   = 0.5,.    ):. 
-0000ddf0: 2020 2020 2020 2022 2222 506c 6f74 2063         """Plot c
-0000de00: 6f6d 706f 6e65 6e74 2069 6e20 686f 6c6f  omponent in holo
-0000de10: 7669 6577 732e 0a0a 2020 2020 2020 2020  views...        
-0000de20: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000de30: 2020 6c61 7965 7273 5f65 7863 6c75 6465    layers_exclude
-0000de40: 643a 206c 6973 7420 6f66 206c 6179 6572  d: list of layer
-0000de50: 7320 746f 2065 7863 6c75 6465 2e0a 2020  s to exclude..  
-0000de60: 2020 2020 2020 2020 2020 6c61 7965 725f            layer_
-0000de70: 7669 6577 733a 206c 6179 6572 5f76 6965  views: layer_vie
-0000de80: 7773 2063 6f6c 6f72 7320 6c6f 6164 6564  ws colors loaded
-0000de90: 2066 726f 6d20 4b6c 6179 6f75 742e 0a20   from Klayout.. 
-0000dea0: 2020 2020 2020 2020 2020 206d 696e 5f61             min_a
-0000deb0: 7370 6563 743a 206d 696e 696d 756d 2061  spect: minimum a
-0000dec0: 7370 6563 7420 7261 7469 6f2e 0a20 2020  spect ratio..   
-0000ded0: 2020 2020 2020 2020 2070 6164 6469 6e67           padding
-0000dee0: 3a20 6172 6f75 6e64 2062 6f75 6e64 696e  : around boundin
-0000def0: 6720 626f 782e 0a0a 2020 2020 2020 2020  g box...        
-0000df00: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-0000df10: 2020 2020 2048 6f6c 6f76 6965 7773 204f       Holoviews O
-0000df20: 7665 726c 6179 2074 6f20 6469 7370 6c61  verlay to displa
-0000df30: 7920 616c 6c20 706f 6c79 676f 6e73 2e0a  y all polygons..
-0000df40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000df50: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
-0000df60: 6f72 792e 6164 645f 7069 6e73 2069 6d70  ory.add_pins imp
-0000df70: 6f72 7420 6765 745f 7069 6e5f 7472 6961  ort get_pin_tria
-0000df80: 6e67 6c65 5f70 6f6c 7967 6f6e 5f74 6970  ngle_polygon_tip
-0000df90: 0a20 2020 2020 2020 2066 726f 6d20 6764  .        from gd
-0000dfa0: 7366 6163 746f 7279 2e70 646b 2069 6d70  sfactory.pdk imp
-0000dfb0: 6f72 7420 6765 745f 6c61 7965 725f 7669  ort get_layer_vi
-0000dfc0: 6577 730a 0a20 2020 2020 2020 2077 6172  ews..        war
-0000dfd0: 6e69 6e67 732e 7761 726e 280a 2020 2020  nings.warn(.    
-0000dfe0: 2020 2020 2020 2020 2268 6f6c 6f76 6965          "holovie
-0000dff0: 7773 2070 6c6f 7474 6572 2069 7320 6465  ws plotter is de
-0000e000: 7072 6563 6174 6564 2e20 220a 2020 2020  precated. ".    
-0000e010: 2020 2020 2020 2020 2255 7365 2074 6865          "Use the
-0000e020: 2064 6566 6175 6c74 2043 6f6d 706f 6e65   default Compone
-0000e030: 6e74 2e70 6c6f 7428 292c 2043 6f6d 706f  nt.plot(), Compo
-0000e040: 6e65 6e74 2e70 6c6f 745f 6b6c 6179 6f75  nent.plot_klayou
-0000e050: 7428 2920 6f72 2043 6f6d 706f 6e65 6e74  t() or Component
-0000e060: 2e70 6c6f 745f 7769 6467 6574 2829 222c  .plot_widget()",
-0000e070: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-0000e080: 636b 6c65 7665 6c3d 332c 0a20 2020 2020  cklevel=3,.     
-0000e090: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-0000e0a0: 206c 6179 6572 5f76 6965 7773 2069 7320   layer_views is 
-0000e0b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000e0c0: 2020 6c61 7965 725f 7669 6577 7320 3d20    layer_views = 
-0000e0d0: 6765 745f 6c61 7965 725f 7669 6577 7328  get_layer_views(
-0000e0e0: 290a 0a20 2020 2020 2020 2074 7279 3a0a  )..        try:.
-0000e0f0: 2020 2020 2020 2020 2020 2020 696d 706f              impo
-0000e100: 7274 2068 6f6c 6f76 6965 7773 2061 7320  rt holoviews as 
-0000e110: 6876 0a0a 2020 2020 2020 2020 2020 2020  hv..            
-0000e120: 6876 2e65 7874 656e 7369 6f6e 2822 626f  hv.extension("bo
-0000e130: 6b65 6822 290a 2020 2020 2020 2020 6578  keh").        ex
-0000e140: 6365 7074 2049 6d70 6f72 7445 7272 6f72  cept ImportError
-0000e150: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-0000e160: 2020 2070 7269 6e74 2822 796f 7520 6e65     print("you ne
-0000e170: 6564 2074 6f20 6070 6970 2069 6e73 7461  ed to `pip insta
-0000e180: 6c6c 2068 6f6c 6f76 6965 7773 6022 290a  ll holoviews`").
-0000e190: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000e1a0: 6520 650a 0a20 2020 2020 2020 2073 656c  e e..        sel
-0000e1b0: 662e 5f62 625f 7661 6c69 6420 3d20 4661  f._bb_valid = Fa
-0000e1c0: 6c73 6520 2023 2072 6563 6f6d 7075 7465  lse  # recompute
-0000e1d0: 2074 6865 2062 6f75 6e64 696e 6720 626f   the bounding bo
-0000e1e0: 780a 2020 2020 2020 2020 6220 3d20 7365  x.        b = se
-0000e1f0: 6c66 2e62 626f 7820 2b20 2828 2d70 6164  lf.bbox + ((-pad
-0000e200: 6469 6e67 2c20 2d70 6164 6469 6e67 292c  ding, -padding),
-0000e210: 2028 7061 6464 696e 672c 2070 6164 6469   (padding, paddi
-0000e220: 6e67 2929 0a20 2020 2020 2020 2062 203d  ng)).        b =
-0000e230: 206e 702e 6172 7261 7928 622e 666c 6174   np.array(b.flat
-0000e240: 290a 2020 2020 2020 2020 6365 6e74 6572  ).        center
-0000e250: 203d 206e 702e 6172 7261 7928 286e 702e   = np.array((np.
-0000e260: 7375 6d28 625b 3a3a 325d 2920 2f20 322c  sum(b[::2]) / 2,
-0000e270: 206e 702e 7375 6d28 625b 313a 3a32 5d29   np.sum(b[1::2])
-0000e280: 202f 2032 2929 0a20 2020 2020 2020 2073   / 2)).        s
-0000e290: 697a 6520 3d20 6e70 2e61 7272 6179 2828  ize = np.array((
-0000e2a0: 6e70 2e61 6273 2862 5b32 5d20 2d20 625b  np.abs(b[2] - b[
-0000e2b0: 305d 292c 206e 702e 6162 7328 625b 335d  0]), np.abs(b[3]
-0000e2c0: 202d 2062 5b31 5d29 2929 0a20 2020 2020   - b[1]))).     
-0000e2d0: 2020 2064 7820 3d20 6e70 2e61 7272 6179     dx = np.array
-0000e2e0: 280a 2020 2020 2020 2020 2020 2020 280a  (.            (.
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e300: 6e70 2e6d 6178 696d 756d 286d 696e 5f61  np.maximum(min_a
-0000e310: 7370 6563 7420 2a20 7369 7a65 5b31 5d2c  spect * size[1],
-0000e320: 2073 697a 655b 305d 2920 2f20 322c 0a20   size[0]) / 2,. 
-0000e330: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000e340: 702e 6d61 7869 6d75 6d28 7369 7a65 5b31  p.maximum(size[1
-0000e350: 5d2c 206d 696e 5f61 7370 6563 7420 2a20  ], min_aspect * 
-0000e360: 7369 7a65 5b30 5d29 202f 2032 2c0a 2020  size[0]) / 2,.  
-0000e370: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000e380: 2020 2020 290a 2020 2020 2020 2020 6220      ).        b 
-0000e390: 3d20 6e70 2e68 7374 6163 6b28 2863 656e  = np.hstack((cen
-0000e3a0: 7465 7220 2d20 6478 2c20 6365 6e74 6572  ter - dx, center
-0000e3b0: 202b 2064 7829 290a 0a20 2020 2020 2020   + dx))..       
-0000e3c0: 2070 6c6f 7473 5f74 6f5f 6f76 6572 6c61   plots_to_overla
-0000e3d0: 7920 3d20 5b5d 0a20 2020 2020 2020 206c  y = [].        l
-0000e3e0: 6179 6572 735f 6578 636c 7564 6564 203d  ayers_excluded =
-0000e3f0: 205b 5d20 6966 206c 6179 6572 735f 6578   [] if layers_ex
-0000e400: 636c 7564 6564 2069 7320 4e6f 6e65 2065  cluded is None e
-0000e410: 6c73 6520 6c61 7965 7273 5f65 7863 6c75  lse layers_exclu
-0000e420: 6465 640a 0a20 2020 2020 2020 2066 6f72  ded..        for
-0000e430: 206c 6179 6572 2c20 706f 6c79 676f 6e20   layer, polygon 
-0000e440: 696e 2073 656c 662e 6765 745f 706f 6c79  in self.get_poly
-0000e450: 676f 6e73 2862 795f 7370 6563 3d54 7275  gons(by_spec=Tru
-0000e460: 6529 2e69 7465 6d73 2829 3a0a 2020 2020  e).items():.    
-0000e470: 2020 2020 2020 2020 6966 206c 6179 6572          if layer
-0000e480: 2069 6e20 6c61 7965 7273 5f65 7863 6c75   in layers_exclu
-0000e490: 6465 643a 0a20 2020 2020 2020 2020 2020  ded:.           
-0000e4a0: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-0000e4b0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4d0: 6c61 7965 725f 7669 6577 203d 206c 6179  layer_view = lay
-0000e4e0: 6572 5f76 6965 7773 2e67 6574 5f66 726f  er_views.get_fro
-0000e4f0: 6d5f 7475 706c 6528 6c61 7965 7229 0a20  m_tuple(layer). 
-0000e500: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-0000e510: 7420 5661 6c75 6545 7272 6f72 3a0a 2020  t ValueError:.  
-0000e520: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-0000e530: 7965 7273 203d 206c 6973 7428 6c61 7965  yers = list(laye
-0000e540: 725f 7669 6577 732e 6765 745f 6c61 7965  r_views.get_laye
-0000e550: 725f 7669 6577 7328 292e 6b65 7973 2829  r_views().keys()
-0000e560: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e570: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-0000e580: 6622 7b6c 6179 6572 2172 7d20 6e6f 7420  f"{layer!r} not 
-0000e590: 6465 6669 6e65 6420 696e 207b 6c61 7965  defined in {laye
-0000e5a0: 7273 7d22 2c20 7374 6163 6b6c 6576 656c  rs}", stacklevel
-0000e5b0: 3d33 290a 2020 2020 2020 2020 2020 2020  =3).            
-0000e5c0: 2020 2020 6c61 7965 725f 7669 6577 203d      layer_view =
-0000e5d0: 204c 6179 6572 5669 6577 286c 6179 6572   LayerView(layer
-0000e5e0: 3d6c 6179 6572 290a 2020 2020 2020 2020  =layer).        
-0000e5f0: 2020 2020 2320 544f 444f 3a20 4d61 7463      # TODO: Matc
-0000e600: 6820 7570 206f 7074 696f 6e73 2077 6974  h up options wit
-0000e610: 6820 4c61 7965 7256 6965 7773 0a20 2020  h LayerViews.   
-0000e620: 2020 2020 2020 2020 2070 6c6f 7473 5f74           plots_t
-0000e630: 6f5f 6f76 6572 6c61 792e 6170 7065 6e64  o_overlay.append
-0000e640: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000e650: 2020 6876 2e50 6f6c 7967 6f6e 7328 706f    hv.Polygons(po
-0000e660: 6c79 676f 6e2c 206c 6162 656c 3d73 7472  lygon, label=str
-0000e670: 286c 6179 6572 5f76 6965 772e 6e61 6d65  (layer_view.name
-0000e680: 2929 2e6f 7074 7328 0a20 2020 2020 2020  )).opts(.       
-0000e690: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-0000e6a0: 615f 6173 7065 6374 3d31 2c0a 2020 2020  a_aspect=1,.    
-0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6c0: 6672 616d 655f 7769 6474 683d 3530 302c  frame_width=500,
-0000e6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e6e0: 2020 2020 2079 6c69 6d3d 2862 5b31 5d2c       ylim=(b[1],
-0000e6f0: 2062 5b33 5d29 2c0a 2020 2020 2020 2020   b[3]),.        
-0000e700: 2020 2020 2020 2020 2020 2020 786c 696d              xlim
-0000e710: 3d28 625b 305d 2c20 625b 325d 292c 0a20  =(b[0], b[2]),. 
-0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e730: 2020 2066 696c 6c5f 636f 6c6f 723d 6c61     fill_color=la
-0000e740: 7965 725f 7669 6577 2e66 696c 6c5f 636f  yer_view.fill_co
-0000e750: 6c6f 722e 6173 5f72 6762 2829 206f 7220  lor.as_rgb() or 
-0000e760: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
-0000e770: 2020 2020 2020 2020 6c69 6e65 5f63 6f6c          line_col
-0000e780: 6f72 3d6c 6179 6572 5f76 6965 772e 6672  or=layer_view.fr
-0000e790: 616d 655f 636f 6c6f 722e 6173 5f72 6762  ame_color.as_rgb
-0000e7a0: 2829 206f 7220 2222 2c0a 2020 2020 2020  () or "",.      
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0000e7c0: 6c6c 5f61 6c70 6861 3d6c 6179 6572 5f76  ll_alpha=layer_v
-0000e7d0: 6965 772e 6765 745f 616c 7068 6128 2920  iew.get_alpha() 
-0000e7e0: 6f72 2022 222c 0a20 2020 2020 2020 2020  or "",.         
-0000e7f0: 2020 2020 2020 2020 2020 206c 696e 655f             line_
-0000e800: 616c 7068 613d 6c61 7965 725f 7669 6577  alpha=layer_view
-0000e810: 2e67 6574 5f61 6c70 6861 2829 206f 7220  .get_alpha() or 
-0000e820: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
-0000e830: 2020 2020 2020 2020 746f 6f6c 733d 5b22          tools=["
-0000e840: 686f 7665 7222 5d2c 0a20 2020 2020 2020  hover"],.       
-0000e850: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000e860: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000e870: 2066 6f72 206e 616d 652c 2070 6f72 7420   for name, port 
-0000e880: 696e 2073 656c 662e 706f 7274 732e 6974  in self.ports.it
-0000e890: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-0000e8a0: 2020 206e 616d 6520 3d20 7374 7228 6e61     name = str(na
-0000e8b0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0000e8c0: 706f 6c79 676f 6e2c 2070 7469 7020 3d20  polygon, ptip = 
-0000e8d0: 6765 745f 7069 6e5f 7472 6961 6e67 6c65  get_pin_triangle
-0000e8e0: 5f70 6f6c 7967 6f6e 5f74 6970 2870 6f72  _polygon_tip(por
-0000e8f0: 743d 706f 7274 290a 0a20 2020 2020 2020  t=port)..       
-0000e900: 2020 2020 2070 6c6f 7473 5f74 6f5f 6f76       plots_to_ov
-0000e910: 6572 6c61 792e 6170 7065 6e64 280a 2020  erlay.append(.  
-0000e920: 2020 2020 2020 2020 2020 2020 2020 6876                hv
-0000e930: 2e50 6f6c 7967 6f6e 7328 706f 6c79 676f  .Polygons(polygo
-0000e940: 6e2c 206c 6162 656c 3d6e 616d 6529 2e6f  n, label=name).o
-0000e950: 7074 7328 0a20 2020 2020 2020 2020 2020  pts(.           
-0000e960: 2020 2020 2020 2020 2064 6174 615f 6173           data_as
-0000e970: 7065 6374 3d31 2c0a 2020 2020 2020 2020  pect=1,.        
-0000e980: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-0000e990: 655f 7769 6474 683d 3530 302c 0a20 2020  e_width=500,.   
+0000c950: 2020 2020 2020 2066 726f 6d20 696f 2069         from io i
+0000c960: 6d70 6f72 7420 4279 7465 7349 4f0a 0a20  mport BytesIO.. 
+0000c970: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
+0000c980: 7420 6b6c 6179 6f75 742e 6462 2061 7320  t klayout.db as 
+0000c990: 6462 2020 2320 6e6f 7161 3a20 4634 3031  db  # noqa: F401
+0000c9a0: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
+0000c9b0: 6f72 7420 6b6c 6179 6f75 742e 6c61 7920  ort klayout.lay 
+0000c9c0: 6173 206c 6179 0a20 2020 2020 2020 2020  as lay.         
+0000c9d0: 2020 2069 6d70 6f72 7420 6d61 7470 6c6f     import matplo
+0000c9e0: 746c 6962 2e70 7970 6c6f 7420 6173 2070  tlib.pyplot as p
+0000c9f0: 6c74 0a0a 2020 2020 2020 2020 2020 2020  lt..            
+0000ca00: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
+0000ca10: 7064 6b20 696d 706f 7274 2067 6574 5f6c  pdk import get_l
+0000ca20: 6179 6572 5f76 6965 7773 0a0a 2020 2020  ayer_views..    
+0000ca30: 2020 2020 2020 2020 6764 7370 6174 6820          gdspath 
+0000ca40: 3d20 636f 6d70 6f6e 656e 742e 7772 6974  = component.writ
+0000ca50: 655f 6764 7328 6c6f 6767 696e 673d 4661  e_gds(logging=Fa
+0000ca60: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+0000ca70: 206c 7970 5f70 6174 6820 3d20 6764 7370   lyp_path = gdsp
+0000ca80: 6174 682e 7769 7468 5f73 7566 6669 7828  ath.with_suffix(
+0000ca90: 222e 6c79 7022 290a 0a20 2020 2020 2020  ".lyp")..       
+0000caa0: 2020 2020 206c 6179 6572 5f76 6965 7773       layer_views
+0000cab0: 203d 2067 6574 5f6c 6179 6572 5f76 6965   = get_layer_vie
+0000cac0: 7773 2829 0a20 2020 2020 2020 2020 2020  ws().           
+0000cad0: 206c 6179 6572 5f76 6965 7773 2e74 6f5f   layer_views.to_
+0000cae0: 6c79 7028 6669 6c65 7061 7468 3d6c 7970  lyp(filepath=lyp
+0000caf0: 5f70 6174 6829 0a0a 2020 2020 2020 2020  _path)..        
+0000cb00: 2020 2020 6c61 796f 7574 5f76 6965 7720      layout_view 
+0000cb10: 3d20 6c61 792e 4c61 796f 7574 5669 6577  = lay.LayoutView
+0000cb20: 2829 0a20 2020 2020 2020 2020 2020 206c  ().            l
+0000cb30: 6179 6f75 745f 7669 6577 2e6c 6f61 645f  ayout_view.load_
+0000cb40: 6c61 796f 7574 2873 7472 2867 6473 7061  layout(str(gdspa
+0000cb50: 7468 2e61 6273 6f6c 7574 6528 2929 290a  th.absolute())).
+0000cb60: 2020 2020 2020 2020 2020 2020 6c61 796f              layo
+0000cb70: 7574 5f76 6965 772e 6d61 785f 6869 6572  ut_view.max_hier
+0000cb80: 2829 0a20 2020 2020 2020 2020 2020 206c  ().            l
+0000cb90: 6179 6f75 745f 7669 6577 2e6c 6f61 645f  ayout_view.load_
+0000cba0: 6c61 7965 725f 7072 6f70 7328 7374 7228  layer_props(str(
+0000cbb0: 6c79 705f 7061 7468 2929 0a0a 2020 2020  lyp_path))..    
+0000cbc0: 2020 2020 2020 2020 6c61 796f 7574 5f76          layout_v
+0000cbd0: 6965 772e 7365 745f 636f 6e66 6967 2822  iew.set_config("
+0000cbe0: 7465 7874 2d76 6973 6962 6c65 222c 2022  text-visible", "
+0000cbf0: 7472 7565 2220 6966 2073 686f 775f 6c61  true" if show_la
+0000cc00: 6265 6c73 2065 6c73 6520 2266 616c 7365  bels else "false
+0000cc10: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+0000cc20: 7069 7865 6c5f 6275 6666 6572 203d 206c  pixel_buffer = l
+0000cc30: 6179 6f75 745f 7669 6577 2e67 6574 5f70  ayout_view.get_p
+0000cc40: 6978 656c 735f 7769 7468 5f6f 7074 696f  ixels_with_optio
+0000cc50: 6e73 2838 3030 2c20 3630 3029 0a20 2020  ns(800, 600).   
+0000cc60: 2020 2020 2020 2020 2070 6e67 5f64 6174           png_dat
+0000cc70: 6120 3d20 7069 7865 6c5f 6275 6666 6572  a = pixel_buffer
+0000cc80: 2e74 6f5f 706e 675f 6461 7461 2829 0a0a  .to_png_data()..
+0000cc90: 2020 2020 2020 2020 2020 2020 2320 436f              # Co
+0000cca0: 6e76 6572 7420 504e 4720 6461 7461 2074  nvert PNG data t
+0000ccb0: 6f20 4e75 6d50 7920 6172 7261 7920 616e  o NumPy array an
+0000ccc0: 6420 6469 7370 6c61 7920 7769 7468 206d  d display with m
+0000ccd0: 6174 706c 6f74 6c69 620a 2020 2020 2020  atplotlib.      
+0000cce0: 2020 2020 2020 7769 7468 2042 7974 6573        with Bytes
+0000ccf0: 494f 2870 6e67 5f64 6174 6129 2061 7320  IO(png_data) as 
+0000cd00: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+0000cd10: 2020 2069 6d67 5f61 7272 6179 203d 2070     img_array = p
+0000cd20: 6c74 2e69 6d72 6561 6428 6629 0a0a 2020  lt.imread(f)..  
+0000cd30: 2020 2020 2020 2020 2020 2320 436f 6d70            # Comp
+0000cd40: 7574 6520 7468 6520 6669 6775 7265 2064  ute the figure d
+0000cd50: 696d 656e 7369 6f6e 7320 6261 7365 6420  imensions based 
+0000cd60: 6f6e 2074 6865 2069 6d61 6765 2073 697a  on the image siz
+0000cd70: 6520 616e 6420 6465 7369 7265 6420 4450  e and desired DP
+0000cd80: 490a 2020 2020 2020 2020 2020 2020 6470  I.            dp
+0000cd90: 6920 3d20 3830 0a20 2020 2020 2020 2020  i = 80.         
+0000cda0: 2020 2066 6967 5f77 6964 7468 203d 2069     fig_width = i
+0000cdb0: 6d67 5f61 7272 6179 2e73 6861 7065 5b31  mg_array.shape[1
+0000cdc0: 5d20 2f20 6470 690a 2020 2020 2020 2020  ] / dpi.        
+0000cdd0: 2020 2020 6669 675f 6865 6967 6874 203d      fig_height =
+0000cde0: 2069 6d67 5f61 7272 6179 2e73 6861 7065   img_array.shape
+0000cdf0: 5b30 5d20 2f20 6470 690a 0a20 2020 2020  [0] / dpi..     
+0000ce00: 2020 2020 2020 2066 6967 2c20 6178 203d         fig, ax =
+0000ce10: 2070 6c74 2e73 7562 706c 6f74 7328 6669   plt.subplots(fi
+0000ce20: 6773 697a 653d 2866 6967 5f77 6964 7468  gsize=(fig_width
+0000ce30: 2c20 6669 675f 6865 6967 6874 292c 2064  , fig_height), d
+0000ce40: 7069 3d64 7069 290a 0a20 2020 2020 2020  pi=dpi)..       
+0000ce50: 2020 2020 2023 2052 656d 6f76 6520 6d61       # Remove ma
+0000ce60: 7267 696e 7320 616e 6420 6469 7370 6c61  rgins and displa
+0000ce70: 7920 7468 6520 696d 6167 650a 2020 2020  y the image.    
+0000ce80: 2020 2020 2020 2020 6178 2e69 6d73 686f          ax.imsho
+0000ce90: 7728 696d 675f 6172 7261 7929 0a20 2020  w(img_array).   
+0000cea0: 2020 2020 2020 2020 2061 782e 6178 6973           ax.axis
+0000ceb0: 2822 6f66 6622 2920 2023 2048 6964 6520  ("off")  # Hide 
+0000cec0: 6178 6573 0a20 2020 2020 2020 2020 2020  axes.           
+0000ced0: 2061 782e 7365 745f 706f 7369 7469 6f6e   ax.set_position
+0000cee0: 285b 302c 2030 2c20 312c 2031 5d29 2020  ([0, 0, 1, 1])  
+0000cef0: 2320 5365 7420 6178 6573 2074 6f20 6f63  # Set axes to oc
+0000cf00: 6375 7079 2074 6865 2066 756c 6c20 6669  cupy the full fi
+0000cf10: 6775 7265 2073 7061 6365 0a0a 2020 2020  gure space..    
+0000cf20: 2020 2020 2020 2020 706c 742e 7375 6270          plt.subp
+0000cf30: 6c6f 7473 5f61 646a 7573 7428 0a20 2020  lots_adjust(.   
+0000cf40: 2020 2020 2020 2020 2020 2020 206c 6566               lef
+0000cf50: 743d 302c 2072 6967 6874 3d31 2c20 746f  t=0, right=1, to
+0000cf60: 703d 312c 2062 6f74 746f 6d3d 302c 2077  p=1, bottom=0, w
+0000cf70: 7370 6163 653d 302c 2068 7370 6163 653d  space=0, hspace=
+0000cf80: 300a 2020 2020 2020 2020 2020 2020 2920  0.            ) 
+0000cf90: 2023 2052 656d 6f76 6520 616e 7920 7061   # Remove any pa
+0000cfa0: 6464 696e 670a 2020 2020 2020 2020 2020  dding.          
+0000cfb0: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
+0000cfc0: 7574 2870 6164 3d30 2920 2023 2045 6e73  ut(pad=0)  # Ens
+0000cfd0: 7572 6520 6e6f 2073 7061 6365 2069 7320  ure no space is 
+0000cfe0: 7761 7374 6564 0a20 2020 2020 2020 2020  wasted.         
+0000cff0: 2020 2072 6574 7572 6e20 6669 670a 0a20     return fig.. 
+0000d000: 2020 2020 2020 2065 7863 6570 7420 496d         except Im
+0000d010: 706f 7274 4572 726f 723a 0a20 2020 2020  portError:.     
+0000d020: 2020 2020 2020 2070 7269 6e74 2822 596f         print("Yo
+0000d030: 7520 6361 6e20 696e 7374 616c 6c20 6070  u can install `p
+0000d040: 6970 2069 6e73 7461 6c6c 2067 6473 6661  ip install gdsfa
+0000d050: 6374 6f72 7960 2066 6f72 2062 6574 7465  ctory` for bette
+0000d060: 7220 7669 7375 616c 697a 6174 696f 6e22  r visualization"
+0000d070: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+0000d080: 6d70 6f6e 656e 742e 706c 6f74 2870 6c6f  mponent.plot(plo
+0000d090: 7474 6572 3d22 6d61 7470 6c6f 746c 6962  tter="matplotlib
+0000d0a0: 2229 0a0a 2020 2020 6465 6620 706c 6f74  ")..    def plot
+0000d0b0: 5f6b 7765 6228 7365 6c66 293a 0a20 2020  _kweb(self):.   
+0000d0c0: 2020 2020 2022 2222 5368 6f77 7320 6375       """Shows cu
+0000d0d0: 7272 656e 7420 6764 7320 696e 206b 7765  rrent gds in kwe
+0000d0e0: 622e 2222 220a 2020 2020 2020 2020 696d  b.""".        im
+0000d0f0: 706f 7274 206f 730a 2020 2020 2020 2020  port os.        
+0000d100: 6672 6f6d 2068 746d 6c20 696d 706f 7274  from html import
+0000d110: 2065 7363 6170 650a 0a20 2020 2020 2020   escape..       
+0000d120: 2069 6d70 6f72 7420 6b77 6562 2e73 6572   import kweb.ser
+0000d130: 7665 725f 6a75 7079 7465 7220 6173 206b  ver_jupyter as k
+0000d140: 6a0a 2020 2020 2020 2020 6672 6f6d 2049  j.        from I
+0000d150: 5079 7468 6f6e 2e64 6973 706c 6179 2069  Python.display i
+0000d160: 6d70 6f72 7420 4946 7261 6d65 0a0a 2020  mport IFrame..  
+0000d170: 2020 2020 2020 6672 6f6d 2067 6473 6661        from gdsfa
+0000d180: 6374 6f72 792e 636f 6e66 6967 2069 6d70  ctory.config imp
+0000d190: 6f72 7420 5041 5448 0a20 2020 2020 2020  ort PATH.       
+0000d1a0: 2066 726f 6d20 6764 7366 6163 746f 7279   from gdsfactory
+0000d1b0: 2e70 646b 2069 6d70 6f72 7420 6765 745f  .pdk import get_
+0000d1c0: 6c61 7965 725f 7669 6577 730a 0a20 2020  layer_views..   
+0000d1d0: 2020 2020 2067 6473 7061 7468 203d 2073       gdspath = s
+0000d1e0: 656c 662e 7772 6974 655f 6764 7328 6764  elf.write_gds(gd
+0000d1f0: 7364 6972 3d50 4154 482e 6764 736c 6962  sdir=PATH.gdslib
+0000d200: 202f 2022 6578 7472 6122 2c20 6c6f 6767   / "extra", logg
+0000d210: 696e 673d 4661 6c73 6529 0a0a 2020 2020  ing=False)..    
+0000d220: 2020 2020 6469 7270 6174 6820 3d20 4744      dirpath = GD
+0000d230: 5344 4952 5f54 454d 500a 2020 2020 2020  SDIR_TEMP.      
+0000d240: 2020 6469 7270 6174 682e 6d6b 6469 7228    dirpath.mkdir(
+0000d250: 6578 6973 745f 6f6b 3d54 7275 652c 2070  exist_ok=True, p
+0000d260: 6172 656e 7473 3d54 7275 6529 0a20 2020  arents=True).   
+0000d270: 2020 2020 206c 7970 5f70 6174 6820 3d20       lyp_path = 
+0000d280: 6469 7270 6174 6820 2f20 226c 6179 6572  dirpath / "layer
+0000d290: 732e 6c79 7022 0a0a 2020 2020 2020 2020  s.lyp"..        
+0000d2a0: 6c61 7965 725f 7072 6f70 7320 3d20 6765  layer_props = ge
+0000d2b0: 745f 6c61 7965 725f 7669 6577 7328 290a  t_layer_views().
+0000d2c0: 2020 2020 2020 2020 6c61 7965 725f 7072          layer_pr
+0000d2d0: 6f70 732e 746f 5f6c 7970 2866 696c 6570  ops.to_lyp(filep
+0000d2e0: 6174 683d 6c79 705f 7061 7468 290a 0a20  ath=lyp_path).. 
+0000d2f0: 2020 2020 2020 2070 6f72 7420 3d20 6b6a         port = kj
+0000d300: 2e70 6f72 7420 6966 2068 6173 6174 7472  .port if hasattr
+0000d310: 286b 6a2c 2022 706f 7274 2229 2061 6e64  (kj, "port") and
+0000d320: 206b 6a2e 706f 7274 2065 6c73 6520 3830   kj.port else 80
+0000d330: 3030 0a20 2020 2020 2020 2073 7263 203d  00.        src =
+0000d340: 2066 2268 7474 703a 2f2f 3132 372e 302e   f"http://127.0.
+0000d350: 302e 313a 7b70 6f72 747d 2f67 6473 3f67  0.1:{port}/gds?g
+0000d360: 6473 5f66 696c 653d 7b65 7363 6170 6528  ds_file={escape(
+0000d370: 7374 7228 6764 7370 6174 6829 297d 266c  str(gdspath))}&l
+0000d380: 6179 6572 5f70 726f 7073 3d7b 6573 6361  ayer_props={esca
+0000d390: 7065 2873 7472 286c 7970 5f70 6174 6829  pe(str(lyp_path)
+0000d3a0: 297d 220a 0a20 2020 2020 2020 206f 732e  )}"..        os.
+0000d3b0: 656e 7669 726f 6e5b 224b 5745 425f 504f  environ["KWEB_PO
+0000d3c0: 5254 225d 203d 2073 7472 286f 732e 6765  RT"] = str(os.ge
+0000d3d0: 7465 6e76 2822 4b57 4542 5f50 4f52 5422  tenv("KWEB_PORT"
+0000d3e0: 2c20 706f 7274 2929 0a0a 2020 2020 2020  , port))..      
+0000d3f0: 2020 6966 206e 6f74 206b 6a2e 6a75 7079    if not kj.jupy
+0000d400: 7465 725f 7365 7276 6572 3a0a 2020 2020  ter_server:.    
+0000d410: 2020 2020 2020 2020 706f 7274 203d 2069          port = i
+0000d420: 6e74 286f 732e 6765 7465 6e76 2822 4b57  nt(os.getenv("KW
+0000d430: 4542 5f50 4f52 5422 2929 0a20 2020 2020  EB_PORT")).     
+0000d440: 2020 2020 2020 2077 6869 6c65 206b 6a2e         while kj.
+0000d450: 6973 5f70 6f72 745f 696e 5f75 7365 2870  is_port_in_use(p
+0000d460: 6f72 7429 3a0a 2020 2020 2020 2020 2020  ort):.          
+0000d470: 2020 2020 2020 706f 7274 202b 3d20 310a        port += 1.
+0000d480: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
+0000d490: 656e 7669 726f 6e5b 224b 5745 425f 504f  environ["KWEB_PO
+0000d4a0: 5254 225d 203d 2073 7472 2870 6f72 7429  RT"] = str(port)
+0000d4b0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+0000d4c0: 6765 722e 6465 6275 6728 7372 6329 0a20  ger.debug(src). 
+0000d4d0: 2020 2020 2020 2020 2020 206b 6a2e 7374             kj.st
+0000d4e0: 6172 7428 290a 0a20 2020 2020 2020 2069  art()..        i
+0000d4f0: 6620 6b6a 2e6a 7570 7974 6572 5f73 6572  f kj.jupyter_ser
+0000d500: 7665 723a 0a20 2020 2020 2020 2020 2020  ver:.           
+0000d510: 2072 6574 7572 6e20 4946 7261 6d65 280a   return IFrame(.
+0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d530: 7372 633d 7372 632c 0a20 2020 2020 2020  src=src,.       
+0000d540: 2020 2020 2020 2020 2077 6964 7468 3d31           width=1
+0000d550: 3430 302c 0a20 2020 2020 2020 2020 2020  400,.           
+0000d560: 2020 2020 2068 6569 6768 743d 3630 302c       height=600,
+0000d570: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000d580: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000d590: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000d5a0: 7365 6c66 2e70 6c6f 745f 6b6c 6179 6f75  self.plot_klayou
+0000d5b0: 7428 290a 0a20 2020 2064 6566 2070 6c6f  t()..    def plo
+0000d5c0: 745f 6d61 7470 6c6f 746c 6962 2873 656c  t_matplotlib(sel
+0000d5d0: 662c 202a 2a6b 7761 7267 7329 202d 3e20  f, **kwargs) -> 
+0000d5e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000d5f0: 2250 6c6f 7420 636f 6d70 6f6e 656e 7420  "Plot component 
+0000d600: 7573 696e 6720 6d61 7470 6c6f 746c 6962  using matplotlib
+0000d610: 2e0a 0a20 2020 2020 2020 204b 6579 776f  ...        Keywo
+0000d620: 7264 2041 7267 733a 0a20 2020 2020 2020  rd Args:.       
+0000d630: 2020 2020 2073 686f 775f 706f 7274 733a       show_ports:
+0000d640: 2053 6574 7320 7768 6574 6865 7220 706f   Sets whether po
+0000d650: 7274 7320 6172 6520 6472 6177 6e2e 0a20  rts are drawn.. 
+0000d660: 2020 2020 2020 2020 2020 2073 686f 775f             show_
+0000d670: 7375 6270 6f72 7473 3a20 5365 7473 2077  subports: Sets w
+0000d680: 6865 7468 6572 2073 7562 706f 7274 7320  hether subports 
+0000d690: 2870 6f72 7473 2074 6861 7420 6265 6c6f  (ports that belo
+0000d6a0: 6e67 2074 6f20 7265 6665 7265 6e63 6573  ng to references
+0000d6b0: 2920 6172 6520 6472 6177 6e2e 0a20 2020  ) are drawn..   
+0000d6c0: 2020 2020 2020 2020 206c 6162 656c 5f61           label_a
+0000d6d0: 6c69 6173 6573 3a20 5365 7473 2077 6865  liases: Sets whe
+0000d6e0: 7468 6572 2061 6c69 6173 6573 2061 7265  ther aliases are
+0000d6f0: 206c 6162 656c 6564 2077 6974 6820 6120   labeled with a 
+0000d700: 7465 7874 206e 616d 652e 0a20 2020 2020  text name..     
+0000d710: 2020 2020 2020 206e 6577 5f77 696e 646f         new_windo
+0000d720: 773a 2049 6620 5472 7565 2c20 6561 6368  w: If True, each
+0000d730: 2063 616c 6c20 746f 2071 7569 636b 706c   call to quickpl
+0000d740: 6f74 2829 2077 696c 6c20 6765 6e65 7261  ot() will genera
+0000d750: 7465 2061 2073 6570 6172 6174 6520 7769  te a separate wi
+0000d760: 6e64 6f77 2e0a 2020 2020 2020 2020 2020  ndow..          
+0000d770: 2020 626c 6f63 6b69 6e67 3a20 4966 2054    blocking: If T
+0000d780: 7275 652c 2063 616c 6c69 6e67 2071 7569  rue, calling qui
+0000d790: 636b 706c 6f74 2829 2077 696c 6c20 7061  ckplot() will pa
+0000d7a0: 7573 6520 6578 6563 7574 696f 6e20 6f66  use execution of
+0000d7b0: 2028 2262 6c6f 636b 2229 2074 6865 0a20   ("block") the. 
+0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000d7d0: 656d 6169 6e64 6572 206f 6620 7468 6520  emainder of the 
+0000d7e0: 7079 7468 6f6e 2063 6f64 6520 756e 7469  python code unti
+0000d7f0: 6c20 7468 6520 7175 6963 6b70 6c6f 7428  l the quickplot(
+0000d800: 2920 7769 6e64 6f77 2069 7320 636c 6f73  ) window is clos
+0000d810: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+0000d820: 2020 2020 4966 2046 616c 7365 2c20 7468      If False, th
+0000d830: 6520 7769 6e64 6f77 2077 696c 6c20 6265  e window will be
+0000d840: 206f 7065 6e65 6420 616e 6420 636f 6465   opened and code
+0000d850: 2077 696c 6c20 636f 6e74 696e 7565 2074   will continue t
+0000d860: 6f20 7275 6e2e 0a20 2020 2020 2020 2020  o run..         
+0000d870: 2020 207a 6f6f 6d5f 6661 6374 6f72 3a20     zoom_factor: 
+0000d880: 5365 7473 2074 6865 2073 6361 6c69 6e67  Sets the scaling
+0000d890: 2066 6163 746f 7220 7768 656e 207a 6f6f   factor when zoo
+0000d8a0: 6d69 6e67 2074 6865 2071 7569 636b 706c  ming the quickpl
+0000d8b0: 6f74 2077 696e 646f 7720 7769 7468 2074  ot window with t
+0000d8c0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+0000d8d0: 2020 206d 6f75 7365 7768 6565 6c2f 7472     mousewheel/tr
+0000d8e0: 6163 6b70 6164 2e0a 2020 2020 2020 2020  ackpad..        
+0000d8f0: 2020 2020 696e 7465 7261 6374 6976 655f      interactive_
+0000d900: 7a6f 6f6d 3a20 456e 6162 6c65 7320 7573  zoom: Enables us
+0000d910: 696e 6720 6d6f 7573 6577 6865 656c 2f74  ing mousewheel/t
+0000d920: 7261 636b 7061 6420 746f 207a 6f6f 6d2e  rackpad to zoom.
+0000d930: 0a20 2020 2020 2020 2020 2020 2066 6f6e  .            fon
+0000d940: 7473 697a 653a 2066 6f72 206c 6162 656c  tsize: for label
+0000d950: 732e 0a20 2020 2020 2020 2020 2020 206c  s..            l
+0000d960: 6179 6572 735f 6578 636c 7564 6564 3a20  ayers_excluded: 
+0000d970: 6c69 7374 206f 6620 6c61 7965 7273 2074  list of layers t
+0000d980: 6f20 6578 636c 7564 652e 0a20 2020 2020  o exclude..     
+0000d990: 2020 2020 2020 206c 6179 6572 5f76 6965         layer_vie
+0000d9a0: 7773 3a20 6c61 7965 725f 7669 6577 7320  ws: layer_views 
+0000d9b0: 636f 6c6f 7273 206c 6f61 6465 6420 6672  colors loaded fr
+0000d9c0: 6f6d 204b 6c61 796f 7574 2e0a 2020 2020  om Klayout..    
+0000d9d0: 2020 2020 2020 2020 6d69 6e5f 6173 7065          min_aspe
+0000d9e0: 6374 3a20 6d69 6e69 6d75 6d20 6173 7065  ct: minimum aspe
+0000d9f0: 6374 2072 6174 696f 2e0a 2020 2020 2020  ct ratio..      
+0000da00: 2020 2222 220a 2020 2020 2020 2020 6672    """.        fr
+0000da10: 6f6d 2067 6473 6661 6374 6f72 792e 7175  om gdsfactory.qu
+0000da20: 6963 6b70 6c6f 7474 6572 2069 6d70 6f72  ickplotter impor
+0000da30: 7420 7175 6963 6b70 6c6f 740a 0a20 2020  t quickplot..   
+0000da40: 2020 2020 2071 7569 636b 706c 6f74 2873       quickplot(s
+0000da50: 656c 662c 202a 2a6b 7761 7267 7329 0a0a  elf, **kwargs)..
+0000da60: 2020 2020 6465 6620 706c 6f74 2873 656c      def plot(sel
+0000da70: 662c 2070 6c6f 7474 6572 3a20 7374 7220  f, plotter: str 
+0000da80: 7c20 4e6f 6e65 203d 204e 6f6e 652c 202a  | None = None, *
+0000da90: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+0000daa0: 2020 2222 2252 6574 7572 6e73 2063 6f6d    """Returns com
+0000dab0: 706f 6e65 6e74 2070 6c6f 7420 7573 696e  ponent plot usin
+0000dac0: 6720 6b6c 6179 6f75 742c 206d 6174 706c  g klayout, matpl
+0000dad0: 6f74 6c69 622c 2068 6f6c 6f76 6965 7773  otlib, holoviews
+0000dae0: 206f 7220 7174 2e0a 0a20 2020 2020 2020   or qt...       
+0000daf0: 2057 6520 7265 636f 6d6d 656e 6420 7573   We recommend us
+0000db00: 696e 6720 6b6c 6179 6f75 742e 0a0a 2020  ing klayout...  
+0000db10: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0000db20: 2020 2020 2020 2020 706c 6f74 7465 723a          plotter:
+0000db30: 2070 6c6f 7420 6261 636b 656e 6420 2827   plot backend ('
+0000db40: 6d61 7470 6c6f 746c 6962 272c 2027 7769  matplotlib', 'wi
+0000db50: 6467 6574 272c 2027 6b6c 6179 6f75 7427  dget', 'klayout'
+0000db60: 2c20 276b 7765 6227 292e 0a20 2020 2020  , 'kweb')..     
+0000db70: 2020 2022 2222 0a20 2020 2020 2020 2070     """.        p
+0000db80: 6c6f 7474 6572 203d 2070 6c6f 7474 6572  lotter = plotter
+0000db90: 206f 7220 434f 4e46 2e64 6973 706c 6179   or CONF.display
+0000dba0: 5f74 7970 650a 0a20 2020 2020 2020 2069  _type..        i
+0000dbb0: 6620 706c 6f74 7465 7220 6e6f 7420 696e  f plotter not in
+0000dbc0: 2076 616c 6964 5f70 6c6f 7474 6572 733a   valid_plotters:
+0000dbd0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000dbe0: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+0000dbf0: 7b70 6c6f 7474 6572 2172 7d20 6e6f 7420  {plotter!r} not 
+0000dc00: 696e 207b 7661 6c69 645f 706c 6f74 7465  in {valid_plotte
+0000dc10: 7273 7d22 290a 0a20 2020 2020 2020 2069  rs}")..        i
+0000dc20: 6620 706c 6f74 7465 7220 3d3d 2022 6b6c  f plotter == "kl
+0000dc30: 6179 6f75 7422 3a0a 2020 2020 2020 2020  ayout":.        
+0000dc40: 2020 2020 7365 6c66 2e70 6c6f 745f 6b6c      self.plot_kl
+0000dc50: 6179 6f75 7428 290a 2020 2020 2020 2020  ayout().        
+0000dc60: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000dc70: 2020 2065 6c69 6620 706c 6f74 7465 7220     elif plotter 
+0000dc80: 3d3d 2022 6b77 6562 223a 0a20 2020 2020  == "kweb":.     
+0000dc90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000dca0: 6c66 2e70 6c6f 745f 6b77 6562 2829 0a20  lf.plot_kweb(). 
+0000dcb0: 2020 2020 2020 2065 6c69 6620 706c 6f74         elif plot
+0000dcc0: 7465 7220 3d3d 2022 7769 6467 6574 223a  ter == "widget":
+0000dcd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000dce0: 662e 706c 6f74 5f77 6964 6765 7428 290a  f.plot_widget().
+0000dcf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000dd00: 726e 0a0a 2020 2020 2020 2020 656c 6966  rn..        elif
+0000dd10: 2070 6c6f 7474 6572 203d 3d20 226d 6174   plotter == "mat
+0000dd20: 706c 6f74 6c69 6222 3a0a 2020 2020 2020  plotlib":.      
+0000dd30: 2020 2020 2020 6672 6f6d 2067 6473 6661        from gdsfa
+0000dd40: 6374 6f72 792e 7175 6963 6b70 6c6f 7474  ctory.quickplott
+0000dd50: 6572 2069 6d70 6f72 7420 7175 6963 6b70  er import quickp
+0000dd60: 6c6f 740a 0a20 2020 2020 2020 2020 2020  lot..           
+0000dd70: 2071 7569 636b 706c 6f74 2873 656c 662c   quickplot(self,
+0000dd80: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+0000dd90: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+0000dda0: 2020 2020 2020 2065 6c69 6620 706c 6f74         elif plot
+0000ddb0: 7465 7220 3d3d 2022 686f 6c6f 7669 6577  ter == "holoview
+0000ddc0: 7322 3a0a 2020 2020 2020 2020 2020 2020  s":.            
+0000ddd0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000dde0: 2020 2020 2069 6d70 6f72 7420 686f 6c6f       import holo
+0000ddf0: 7669 6577 7320 6173 2068 760a 0a20 2020  views as hv..   
+0000de00: 2020 2020 2020 2020 2020 2020 2068 762e               hv.
+0000de10: 6578 7465 6e73 696f 6e28 2262 6f6b 6568  extension("bokeh
+0000de20: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+0000de30: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
+0000de40: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
+0000de50: 2020 2020 2020 2020 7072 696e 7428 2279          print("y
+0000de60: 6f75 206e 6565 6420 746f 2060 7069 7020  ou need to `pip 
+0000de70: 696e 7374 616c 6c20 686f 6c6f 7669 6577  install holoview
+0000de80: 7360 2229 0a20 2020 2020 2020 2020 2020  s`").           
+0000de90: 2020 2020 2072 6169 7365 2065 0a20 2020       raise e.   
+0000dea0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000deb0: 7365 6c66 2e70 6c6f 745f 686f 6c6f 7669  self.plot_holovi
+0000dec0: 6577 7328 2a2a 6b77 6172 6773 290a 0a20  ews(**kwargs).. 
+0000ded0: 2020 2020 2020 2065 6c69 6620 706c 6f74         elif plot
+0000dee0: 7465 7220 3d3d 2022 7174 223a 0a20 2020  ter == "qt":.   
+0000def0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0000df00: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+0000df10: 2020 2020 2020 2020 2271 7420 706c 6f74          "qt plot
+0000df20: 7465 7220 6973 2064 6570 7265 6361 7465  ter is deprecate
+0000df30: 642e 2022 0a20 2020 2020 2020 2020 2020  d. ".           
+0000df40: 2020 2020 2022 5573 6520 7468 6520 6465       "Use the de
+0000df50: 6661 756c 7420 436f 6d70 6f6e 656e 742e  fault Component.
+0000df60: 706c 6f74 2829 2c20 436f 6d70 6f6e 656e  plot(), Componen
+0000df70: 742e 706c 6f74 5f6b 6c61 796f 7574 2829  t.plot_klayout()
+0000df80: 206f 7220 436f 6d70 6f6e 656e 742e 706c   or Component.pl
+0000df90: 6f74 5f77 6964 6765 7428 2922 2c0a 2020  ot_widget()",.  
+0000dfa0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000dfb0: 6163 6b6c 6576 656c 3d33 2c0a 2020 2020  acklevel=3,.    
+0000dfc0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000dfd0: 2020 2020 2020 6672 6f6d 2067 6473 6661        from gdsfa
+0000dfe0: 6374 6f72 792e 7175 6963 6b70 6c6f 7474  ctory.quickplott
+0000dff0: 6572 2069 6d70 6f72 7420 7175 6963 6b70  er import quickp
+0000e000: 6c6f 7432 0a0a 2020 2020 2020 2020 2020  lot2..          
+0000e010: 2020 7175 6963 6b70 6c6f 7432 2873 656c    quickplot2(sel
+0000e020: 6629 0a20 2020 2020 2020 2020 2020 2072  f).            r
+0000e030: 6574 7572 6e0a 0a20 2020 2064 6566 2070  eturn..    def p
+0000e040: 6c6f 745f 686f 6c6f 7669 6577 7328 0a20  lot_holoviews(. 
+0000e050: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000e060: 2020 2020 206c 6179 6572 735f 6578 636c       layers_excl
+0000e070: 7564 6564 3a20 4c61 7965 7273 207c 204e  uded: Layers | N
+0000e080: 6f6e 6520 3d20 4e6f 6e65 2c0a 2020 2020  one = None,.    
+0000e090: 2020 2020 6c61 7965 725f 7669 6577 733a      layer_views:
+0000e0a0: 204c 6179 6572 5669 6577 7320 7c20 4e6f   LayerViews | No
+0000e0b0: 6e65 203d 204e 6f6e 652c 0a20 2020 2020  ne = None,.     
+0000e0c0: 2020 206d 696e 5f61 7370 6563 743a 2066     min_aspect: f
+0000e0d0: 6c6f 6174 203d 2030 2e32 352c 0a20 2020  loat = 0.25,.   
+0000e0e0: 2020 2020 2070 6164 6469 6e67 3a20 666c       padding: fl
+0000e0f0: 6f61 7420 3d20 302e 352c 0a20 2020 2029  oat = 0.5,.    )
+0000e100: 3a0a 2020 2020 2020 2020 2222 2250 6c6f  :.        """Plo
+0000e110: 7420 636f 6d70 6f6e 656e 7420 696e 2068  t component in h
+0000e120: 6f6c 6f76 6965 7773 2e0a 0a20 2020 2020  oloviews...     
+0000e130: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000e140: 2020 2020 206c 6179 6572 735f 6578 636c       layers_excl
+0000e150: 7564 6564 3a20 6c69 7374 206f 6620 6c61  uded: list of la
+0000e160: 7965 7273 2074 6f20 6578 636c 7564 652e  yers to exclude.
+0000e170: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+0000e180: 6572 5f76 6965 7773 3a20 6c61 7965 725f  er_views: layer_
+0000e190: 7669 6577 7320 636f 6c6f 7273 206c 6f61  views colors loa
+0000e1a0: 6465 6420 6672 6f6d 204b 6c61 796f 7574  ded from Klayout
+0000e1b0: 2e0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
+0000e1c0: 6e5f 6173 7065 6374 3a20 6d69 6e69 6d75  n_aspect: minimu
+0000e1d0: 6d20 6173 7065 6374 2072 6174 696f 2e0a  m aspect ratio..
+0000e1e0: 2020 2020 2020 2020 2020 2020 7061 6464              padd
+0000e1f0: 696e 673a 2061 726f 756e 6420 626f 756e  ing: around boun
+0000e200: 6469 6e67 2062 6f78 2e0a 0a20 2020 2020  ding box...     
+0000e210: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000e220: 2020 2020 2020 2020 486f 6c6f 7669 6577          Holoview
+0000e230: 7320 4f76 6572 6c61 7920 746f 2064 6973  s Overlay to dis
+0000e240: 706c 6179 2061 6c6c 2070 6f6c 7967 6f6e  play all polygon
+0000e250: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+0000e260: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
+0000e270: 6163 746f 7279 2e61 6464 5f70 696e 7320  actory.add_pins 
+0000e280: 696d 706f 7274 2067 6574 5f70 696e 5f74  import get_pin_t
+0000e290: 7269 616e 676c 655f 706f 6c79 676f 6e5f  riangle_polygon_
+0000e2a0: 7469 700a 2020 2020 2020 2020 6672 6f6d  tip.        from
+0000e2b0: 2067 6473 6661 6374 6f72 792e 7064 6b20   gdsfactory.pdk 
+0000e2c0: 696d 706f 7274 2067 6574 5f6c 6179 6572  import get_layer
+0000e2d0: 5f76 6965 7773 0a0a 2020 2020 2020 2020  _views..        
+0000e2e0: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
+0000e2f0: 2020 2020 2020 2020 2020 2022 686f 6c6f             "holo
+0000e300: 7669 6577 7320 706c 6f74 7465 7220 6973  views plotter is
+0000e310: 2064 6570 7265 6361 7465 642e 2022 0a20   deprecated. ". 
+0000e320: 2020 2020 2020 2020 2020 2022 5573 6520             "Use 
+0000e330: 7468 6520 6465 6661 756c 7420 436f 6d70  the default Comp
+0000e340: 6f6e 656e 742e 706c 6f74 2829 2c20 436f  onent.plot(), Co
+0000e350: 6d70 6f6e 656e 742e 706c 6f74 5f6b 6c61  mponent.plot_kla
+0000e360: 796f 7574 2829 206f 7220 436f 6d70 6f6e  yout() or Compon
+0000e370: 656e 742e 706c 6f74 5f77 6964 6765 7428  ent.plot_widget(
+0000e380: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
+0000e390: 7374 6163 6b6c 6576 656c 3d33 2c0a 2020  stacklevel=3,.  
+0000e3a0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000e3b0: 2069 6620 6c61 7965 725f 7669 6577 7320   if layer_views 
+0000e3c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000e3d0: 2020 2020 206c 6179 6572 5f76 6965 7773       layer_views
+0000e3e0: 203d 2067 6574 5f6c 6179 6572 5f76 6965   = get_layer_vie
+0000e3f0: 7773 2829 0a0a 2020 2020 2020 2020 7472  ws()..        tr
+0000e400: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
+0000e410: 6d70 6f72 7420 686f 6c6f 7669 6577 7320  mport holoviews 
+0000e420: 6173 2068 760a 0a20 2020 2020 2020 2020  as hv..         
+0000e430: 2020 2068 762e 6578 7465 6e73 696f 6e28     hv.extension(
+0000e440: 2262 6f6b 6568 2229 0a20 2020 2020 2020  "bokeh").       
+0000e450: 2065 7863 6570 7420 496d 706f 7274 4572   except ImportEr
+0000e460: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
+0000e470: 2020 2020 2020 7072 696e 7428 2279 6f75        print("you
+0000e480: 206e 6565 6420 746f 2060 7069 7020 696e   need to `pip in
+0000e490: 7374 616c 6c20 686f 6c6f 7669 6577 7360  stall holoviews`
+0000e4a0: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+0000e4b0: 6169 7365 2065 0a0a 2020 2020 2020 2020  aise e..        
+0000e4c0: 7365 6c66 2e5f 6262 5f76 616c 6964 203d  self._bb_valid =
+0000e4d0: 2046 616c 7365 2020 2320 7265 636f 6d70   False  # recomp
+0000e4e0: 7574 6520 7468 6520 626f 756e 6469 6e67  ute the bounding
+0000e4f0: 2062 6f78 0a20 2020 2020 2020 2062 203d   box.        b =
+0000e500: 2073 656c 662e 6262 6f78 202b 2028 282d   self.bbox + ((-
+0000e510: 7061 6464 696e 672c 202d 7061 6464 696e  padding, -paddin
+0000e520: 6729 2c20 2870 6164 6469 6e67 2c20 7061  g), (padding, pa
+0000e530: 6464 696e 6729 290a 2020 2020 2020 2020  dding)).        
+0000e540: 6220 3d20 6e70 2e61 7272 6179 2862 2e66  b = np.array(b.f
+0000e550: 6c61 7429 0a20 2020 2020 2020 2063 656e  lat).        cen
+0000e560: 7465 7220 3d20 6e70 2e61 7272 6179 2828  ter = np.array((
+0000e570: 6e70 2e73 756d 2862 5b3a 3a32 5d29 202f  np.sum(b[::2]) /
+0000e580: 2032 2c20 6e70 2e73 756d 2862 5b31 3a3a   2, np.sum(b[1::
+0000e590: 325d 2920 2f20 3229 290a 2020 2020 2020  2]) / 2)).      
+0000e5a0: 2020 7369 7a65 203d 206e 702e 6172 7261    size = np.arra
+0000e5b0: 7928 286e 702e 6162 7328 625b 325d 202d  y((np.abs(b[2] -
+0000e5c0: 2062 5b30 5d29 2c20 6e70 2e61 6273 2862   b[0]), np.abs(b
+0000e5d0: 5b33 5d20 2d20 625b 315d 2929 290a 2020  [3] - b[1]))).  
+0000e5e0: 2020 2020 2020 6478 203d 206e 702e 6172        dx = np.ar
+0000e5f0: 7261 7928 0a20 2020 2020 2020 2020 2020  ray(.           
+0000e600: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000e610: 2020 206e 702e 6d61 7869 6d75 6d28 6d69     np.maximum(mi
+0000e620: 6e5f 6173 7065 6374 202a 2073 697a 655b  n_aspect * size[
+0000e630: 315d 2c20 7369 7a65 5b30 5d29 202f 2032  1], size[0]) / 2
+0000e640: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e650: 2020 6e70 2e6d 6178 696d 756d 2873 697a    np.maximum(siz
+0000e660: 655b 315d 2c20 6d69 6e5f 6173 7065 6374  e[1], min_aspect
+0000e670: 202a 2073 697a 655b 305d 2920 2f20 322c   * size[0]) / 2,
+0000e680: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000e690: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000e6a0: 2062 203d 206e 702e 6873 7461 636b 2828   b = np.hstack((
+0000e6b0: 6365 6e74 6572 202d 2064 782c 2063 656e  center - dx, cen
+0000e6c0: 7465 7220 2b20 6478 2929 0a0a 2020 2020  ter + dx))..    
+0000e6d0: 2020 2020 706c 6f74 735f 746f 5f6f 7665      plots_to_ove
+0000e6e0: 726c 6179 203d 205b 5d0a 2020 2020 2020  rlay = [].      
+0000e6f0: 2020 6c61 7965 7273 5f65 7863 6c75 6465    layers_exclude
+0000e700: 6420 3d20 5b5d 2069 6620 6c61 7965 7273  d = [] if layers
+0000e710: 5f65 7863 6c75 6465 6420 6973 204e 6f6e  _excluded is Non
+0000e720: 6520 656c 7365 206c 6179 6572 735f 6578  e else layers_ex
+0000e730: 636c 7564 6564 0a0a 2020 2020 2020 2020  cluded..        
+0000e740: 666f 7220 6c61 7965 722c 2070 6f6c 7967  for layer, polyg
+0000e750: 6f6e 2069 6e20 7365 6c66 2e67 6574 5f70  on in self.get_p
+0000e760: 6f6c 7967 6f6e 7328 6279 5f73 7065 633d  olygons(by_spec=
+0000e770: 5472 7565 292e 6974 656d 7328 293a 0a20  True).items():. 
+0000e780: 2020 2020 2020 2020 2020 2069 6620 6c61             if la
+0000e790: 7965 7220 696e 206c 6179 6572 735f 6578  yer in layers_ex
+0000e7a0: 636c 7564 6564 3a0a 2020 2020 2020 2020  cluded:.        
+0000e7b0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000e7c0: 0a0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+0000e7d0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+0000e7e0: 2020 206c 6179 6572 5f76 6965 7720 3d20     layer_view = 
+0000e7f0: 6c61 7965 725f 7669 6577 732e 6765 745f  layer_views.get_
+0000e800: 6672 6f6d 5f74 7570 6c65 286c 6179 6572  from_tuple(layer
+0000e810: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+0000e820: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+0000e830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e840: 206c 6179 6572 7320 3d20 6c69 7374 286c   layers = list(l
+0000e850: 6179 6572 5f76 6965 7773 2e67 6574 5f6c  ayer_views.get_l
+0000e860: 6179 6572 5f76 6965 7773 2829 2e6b 6579  ayer_views().key
+0000e870: 7328 2929 0a20 2020 2020 2020 2020 2020  s()).           
+0000e880: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+0000e890: 726e 2866 227b 6c61 7965 7221 727d 206e  rn(f"{layer!r} n
+0000e8a0: 6f74 2064 6566 696e 6564 2069 6e20 7b6c  ot defined in {l
+0000e8b0: 6179 6572 737d 222c 2073 7461 636b 6c65  ayers}", stackle
+0000e8c0: 7665 6c3d 3329 0a20 2020 2020 2020 2020  vel=3).         
+0000e8d0: 2020 2020 2020 206c 6179 6572 5f76 6965         layer_vie
+0000e8e0: 7720 3d20 4c61 7965 7256 6965 7728 6c61  w = LayerView(la
+0000e8f0: 7965 723d 6c61 7965 7229 0a20 2020 2020  yer=layer).     
+0000e900: 2020 2020 2020 2023 2054 4f44 4f3a 204d         # TODO: M
+0000e910: 6174 6368 2075 7020 6f70 7469 6f6e 7320  atch up options 
+0000e920: 7769 7468 204c 6179 6572 5669 6577 730a  with LayerViews.
+0000e930: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
+0000e940: 735f 746f 5f6f 7665 726c 6179 2e61 7070  s_to_overlay.app
+0000e950: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+0000e960: 2020 2020 2068 762e 506f 6c79 676f 6e73       hv.Polygons
+0000e970: 2870 6f6c 7967 6f6e 2c20 6c61 6265 6c3d  (polygon, label=
+0000e980: 7374 7228 6c61 7965 725f 7669 6577 2e6e  str(layer_view.n
+0000e990: 616d 6529 292e 6f70 7473 280a 2020 2020  ame)).opts(.    
 0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 2066 696c 6c5f 616c 7068 613d 302c 0a20   fill_alpha=0,. 
+0000e9b0: 6461 7461 5f61 7370 6563 743d 312c 0a20  data_aspect=1,. 
 0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9d0: 2020 2079 6c69 6d3d 2862 5b31 5d2c 2062     ylim=(b[1], b
-0000e9e0: 5b33 5d29 2c0a 2020 2020 2020 2020 2020  [3]),.          
-0000e9f0: 2020 2020 2020 2020 2020 786c 696d 3d28            xlim=(
-0000ea00: 625b 305d 2c20 625b 325d 292c 0a20 2020  b[0], b[2]),.   
-0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea20: 2063 6f6c 6f72 3d22 7265 6422 2c0a 2020   color="red",.  
-0000ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea40: 2020 6c69 6e65 5f61 6c70 6861 3d6c 6179    line_alpha=lay
-0000ea50: 6572 5f76 6965 772e 6765 745f 616c 7068  er_view.get_alph
-0000ea60: 6128 2920 6f72 2022 222c 0a20 2020 2020  a() or "",.     
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000ea80: 6f6f 6c73 3d5b 2268 6f76 6572 225d 2c0a  ools=["hover"],.
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000eab0: 2020 2a20 6876 2e54 6578 7428 7074 6970    * hv.Text(ptip
-0000eac0: 5b30 5d2c 2070 7469 705b 315d 2c20 6e61  [0], ptip[1], na
-0000ead0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0000eae0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0000eaf0: 6e20 6876 2e4f 7665 726c 6179 2870 6c6f  n hv.Overlay(plo
-0000eb00: 7473 5f74 6f5f 6f76 6572 6c61 7929 2e6f  ts_to_overlay).o
-0000eb10: 7074 7328 0a20 2020 2020 2020 2020 2020  pts(.           
-0000eb20: 2073 686f 775f 6c65 6765 6e64 3d54 7275   show_legend=Tru
-0000eb30: 652c 2073 6861 7265 645f 6178 6573 3d46  e, shared_axes=F
-0000eb40: 616c 7365 2c20 796c 696d 3d28 625b 315d  alse, ylim=(b[1]
-0000eb50: 2c20 625b 335d 292c 2078 6c69 6d3d 2862  , b[3]), xlim=(b
-0000eb60: 5b30 5d2c 2062 5b32 5d29 0a20 2020 2020  [0], b[2]).     
-0000eb70: 2020 2029 0a0a 2020 2020 6465 6620 7368     )..    def sh
-0000eb80: 6f77 280a 2020 2020 2020 2020 7365 6c66  ow(.        self
-0000eb90: 2c0a 2020 2020 2020 2020 7368 6f77 5f70  ,.        show_p
-0000eba0: 6f72 7473 3a20 626f 6f6c 203d 2046 616c  orts: bool = Fal
-0000ebb0: 7365 2c0a 2020 2020 2020 2020 7368 6f77  se,.        show
-0000ebc0: 5f73 7562 706f 7274 733a 2062 6f6f 6c20  _subports: bool 
-0000ebd0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
-0000ebe0: 2070 6f72 745f 6d61 726b 6572 5f6c 6179   port_marker_lay
-0000ebf0: 6572 3a20 4c61 7965 7220 3d20 2831 2c20  er: Layer = (1, 
-0000ec00: 3130 292c 0a20 2020 2020 2020 202a 2a6b  10),.        **k
-0000ec10: 7761 7267 732c 0a20 2020 2029 202d 3e20  wargs,.    ) -> 
-0000ec20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0000ec30: 2253 686f 7720 636f 6d70 6f6e 656e 7420  "Show component 
-0000ec40: 696e 204b 4c61 796f 7574 2e0a 0a20 2020  in KLayout...   
-0000ec50: 2020 2020 2072 6574 7572 6e73 2061 2063       returns a c
-0000ec60: 6f70 7920 6f66 2074 6865 2043 6f6d 706f  opy of the Compo
-0000ec70: 6e65 6e74 2c20 736f 2074 6865 206f 7269  nent, so the ori
-0000ec80: 6769 6e61 6c20 636f 6d70 6f6e 656e 7420  ginal component 
-0000ec90: 7265 6d61 696e 7320 696e 7461 6374 2e0a  remains intact..
-0000eca0: 2020 2020 2020 2020 7769 7468 2070 696e          with pin
-0000ecb0: 7320 6d61 726b 6572 7320 6f6e 2065 6163  s markers on eac
-0000ecc0: 6820 706f 7274 2073 686f 775f 706f 7274  h port show_port
-0000ecd0: 7320 3d20 5472 7565 2c20 616e 6420 6f70  s = True, and op
-0000ece0: 7469 6f6e 616c 6c79 2061 6c73 6f0a 2020  tionally also.  
-0000ecf0: 2020 2020 2020 7468 6520 706f 7274 7320        the ports 
-0000ed00: 6672 6f6d 2074 6865 2072 6566 6572 656e  from the referen
-0000ed10: 6365 7320 2873 686f 775f 7375 6270 6f72  ces (show_subpor
-0000ed20: 7473 3d54 7275 6529 0a0a 2020 2020 2020  ts=True)..      
-0000ed30: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000ed40: 2020 2020 7368 6f77 5f70 6f72 7473 3a20      show_ports: 
-0000ed50: 7368 6f77 7320 636f 6d70 6f6e 656e 7420  shows component 
-0000ed60: 7769 7468 2070 6f72 7420 6d61 726b 6572  with port marker
-0000ed70: 7320 616e 6420 6c61 6265 6c73 2e0a 2020  s and labels..  
-0000ed80: 2020 2020 2020 2020 2020 7368 6f77 5f73            show_s
-0000ed90: 7562 706f 7274 733a 2061 6464 2070 6f72  ubports: add por
-0000eda0: 7473 206d 6172 6b65 7273 2061 6e64 206c  ts markers and l
-0000edb0: 6162 656c 7320 746f 2072 6566 6572 656e  abels to referen
-0000edc0: 6365 732e 0a20 2020 2020 2020 2020 2020  ces..           
-0000edd0: 2070 6f72 745f 6d61 726b 6572 5f6c 6179   port_marker_lay
-0000ede0: 6572 3a20 666f 7220 7468 6520 706f 7274  er: for the port
-0000edf0: 732e 0a0a 2020 2020 2020 2020 4b65 7977  s...        Keyw
-0000ee00: 6f72 6420 4172 6773 3a0a 2020 2020 2020  ord Args:.      
-0000ee10: 2020 2020 2020 6764 7370 6174 683a 2047        gdspath: G
-0000ee20: 4453 2066 696c 6520 7061 7468 2074 6f20  DS file path to 
-0000ee30: 7772 6974 6520 746f 2e0a 2020 2020 2020  write to..      
-0000ee40: 2020 2020 2020 6764 7364 6972 3a20 6469        gdsdir: di
-0000ee50: 7265 6374 6f72 7920 666f 7220 7468 6520  rectory for the 
-0000ee60: 4744 5320 6669 6c65 2e20 4465 6661 756c  GDS file. Defaul
-0000ee70: 7473 2074 6f20 2f74 6d70 2f2e 0a20 2020  ts to /tmp/..   
-0000ee80: 2020 2020 2020 2020 2075 6e69 743a 2075           unit: u
-0000ee90: 6e69 7420 7369 7a65 2066 6f72 206f 626a  nit size for obj
-0000eea0: 6563 7473 2069 6e20 6c69 6272 6172 792e  ects in library.
-0000eeb0: 2031 756d 2062 7920 6465 6661 756c 742e   1um by default.
-0000eec0: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
-0000eed0: 6369 7369 6f6e 3a20 666f 7220 6f62 6a65  cision: for obje
-0000eee0: 6374 2064 696d 656e 7369 6f6e 7320 696e  ct dimensions in
-0000eef0: 2074 6865 206c 6962 7261 7279 2028 6d29   the library (m)
-0000ef00: 2e20 316e 6d20 6279 2064 6566 6175 6c74  . 1nm by default
-0000ef10: 2e0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-0000ef20: 6d65 7374 616d 703a 2044 6566 6175 6c74  mestamp: Default
-0000ef30: 7320 746f 2032 3031 392d 3130 2d32 352e  s to 2019-10-25.
-0000ef40: 2049 6620 4e6f 6e65 2075 7365 7320 6375   If None uses cu
-0000ef50: 7272 656e 7420 7469 6d65 2e0a 2020 2020  rrent time..    
-0000ef60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000ef70: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
-0000ef80: 6164 645f 7069 6e73 2069 6d70 6f72 7420  add_pins import 
-0000ef90: 6164 645f 7069 6e73 5f74 7269 616e 676c  add_pins_triangl
-0000efa0: 650a 2020 2020 2020 2020 6672 6f6d 2067  e.        from g
-0000efb0: 6473 6661 6374 6f72 792e 7368 6f77 2069  dsfactory.show i
-0000efc0: 6d70 6f72 7420 7368 6f77 0a0a 2020 2020  mport show..    
-0000efd0: 2020 2020 636f 6d70 6f6e 656e 7420 3d20      component = 
-0000efe0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-0000eff0: 6c66 2e61 6464 5f70 696e 735f 7472 6961  lf.add_pins_tria
-0000f000: 6e67 6c65 280a 2020 2020 2020 2020 2020  ngle(.          
-0000f010: 2020 2020 2020 706f 7274 5f6d 6172 6b65        port_marke
-0000f020: 725f 6c61 7965 723d 706f 7274 5f6d 6172  r_layer=port_mar
-0000f030: 6b65 725f 6c61 7965 722c 206c 6179 6572  ker_layer, layer
-0000f040: 5f6c 6162 656c 3d70 6f72 745f 6d61 726b  _label=port_mark
-0000f050: 6572 5f6c 6179 6572 0a20 2020 2020 2020  er_layer.       
-0000f060: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000f070: 2020 2069 6620 7368 6f77 5f70 6f72 7473     if show_ports
-0000f080: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000f090: 6520 7365 6c66 0a20 2020 2020 2020 2029  e self.        )
-0000f0a0: 0a0a 2020 2020 2020 2020 6966 2073 686f  ..        if sho
-0000f0b0: 775f 7375 6270 6f72 7473 3a0a 2020 2020  w_subports:.    
-0000f0c0: 2020 2020 2020 2020 636f 6d70 6f6e 656e          componen
-0000f0d0: 7420 3d20 7365 6c66 2e63 6f70 7928 290a  t = self.copy().
-0000f0e0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
-0000f0f0: 6f6e 656e 742e 6e61 6d65 203d 2073 656c  onent.name = sel
-0000f100: 662e 6e61 6d65 0a20 2020 2020 2020 2020  f.name.         
-0000f110: 2020 2066 6f72 2072 6566 6572 656e 6365     for reference
-0000f120: 2069 6e20 636f 6d70 6f6e 656e 742e 7265   in component.re
-0000f130: 6665 7265 6e63 6573 3a0a 2020 2020 2020  ferences:.      
-0000f140: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-0000f150: 6e73 7461 6e63 6528 636f 6d70 6f6e 656e  nstance(componen
-0000f160: 742c 2043 6f6d 706f 6e65 6e74 5265 6665  t, ComponentRefe
-0000f170: 7265 6e63 6529 3a0a 2020 2020 2020 2020  rence):.        
-0000f180: 2020 2020 2020 2020 2020 2020 6164 645f              add_
-0000f190: 7069 6e73 5f74 7269 616e 676c 6528 0a20  pins_triangle(. 
-0000f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1b0: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
-0000f1c0: 3d63 6f6d 706f 6e65 6e74 2c0a 2020 2020  =component,.    
-0000f1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1e0: 2020 2020 7265 6665 7265 6e63 653d 7265      reference=re
-0000f1f0: 6665 7265 6e63 652c 0a20 2020 2020 2020  ference,.       
-0000f200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f210: 206c 6179 6572 3d70 6f72 745f 6d61 726b   layer=port_mark
-0000f220: 6572 5f6c 6179 6572 2c0a 2020 2020 2020  er_layer,.      
-0000f230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f240: 2020 6c61 7965 725f 6c61 6265 6c3d 706f    layer_label=po
-0000f250: 7274 5f6d 6172 6b65 725f 6c61 7965 722c  rt_marker_layer,
-0000f260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f270: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000f280: 7368 6f77 2863 6f6d 706f 6e65 6e74 2c20  show(component, 
-0000f290: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
-0000f2a0: 6566 205f 7772 6974 655f 6c69 6272 6172  ef _write_librar
-0000f2b0: 7928 0a20 2020 2020 2020 2073 656c 662c  y(.        self,
-0000f2c0: 0a20 2020 2020 2020 2067 6473 7061 7468  .        gdspath
-0000f2d0: 3a20 5061 7468 5479 7065 207c 204e 6f6e  : PathType | Non
-0000f2e0: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-0000f2f0: 2020 6764 7364 6972 3a20 5061 7468 5479    gdsdir: PathTy
-0000f300: 7065 207c 204e 6f6e 6520 3d20 4e6f 6e65  pe | None = None
-0000f310: 2c0a 2020 2020 2020 2020 7469 6d65 7374  ,.        timest
-0000f320: 616d 703a 2064 6174 6574 696d 652e 6461  amp: datetime.da
-0000f330: 7465 7469 6d65 207c 204e 6f6e 6520 3d20  tetime | None = 
-0000f340: 5f74 696d 6573 7461 6d70 3230 3139 2c0a  _timestamp2019,.
-0000f350: 2020 2020 2020 2020 6c6f 6767 696e 673a          logging:
-0000f360: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
-0000f370: 2020 2020 2020 7769 7468 5f6f 6173 6973        with_oasis
-0000f380: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-0000f390: 2020 2020 2020 2020 7769 7468 5f6d 6574          with_met
-0000f3a0: 6164 6174 613a 2062 6f6f 6c20 3d20 4661  adata: bool = Fa
-0000f3b0: 6c73 652c 0a20 2020 2020 2020 202a 2a6b  lse,.        **k
-0000f3c0: 7761 7267 732c 0a20 2020 2029 202d 3e20  wargs,.    ) -> 
-0000f3d0: 5061 7468 3a0a 2020 2020 2020 2020 2222  Path:.        ""
-0000f3e0: 2257 7269 7465 2063 6f6d 706f 6e65 6e74  "Write component
-0000f3f0: 2074 6f20 4744 5320 6f72 204f 4153 4953   to GDS or OASIS
-0000f400: 2061 6e64 2072 6574 7572 6e73 2067 6473   and returns gds
-0000f410: 7061 7468 2e0a 0a20 2020 2020 2020 2041  path...        A
-0000f420: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000f430: 2067 6473 7061 7468 3a20 4744 5320 6669   gdspath: GDS fi
-0000f440: 6c65 2070 6174 6820 746f 2077 7269 7465  le path to write
-0000f450: 2074 6f2e 0a20 2020 2020 2020 2020 2020   to..           
-0000f460: 2067 6473 6469 723a 2064 6972 6563 746f   gdsdir: directo
-0000f470: 7279 2066 6f72 2074 6865 2047 4453 2066  ry for the GDS f
-0000f480: 696c 652e 2044 6566 6175 6c74 7320 746f  ile. Defaults to
-0000f490: 202f 746d 702f 7261 6e64 6f6d 4669 6c65   /tmp/randomFile
-0000f4a0: 2f67 6473 6661 6374 6f72 792e 0a20 2020  /gdsfactory..   
-0000f4b0: 2020 2020 2020 2020 2074 696d 6573 7461           timesta
-0000f4c0: 6d70 3a20 4465 6661 756c 7473 2074 6f20  mp: Defaults to 
-0000f4d0: 3230 3139 2d31 302d 3235 2066 6f72 2063  2019-10-25 for c
-0000f4e0: 6f6e 7369 7374 656e 7420 6861 7368 2e0a  onsistent hash..
-0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f500: 4966 204e 6f6e 6520 7573 6573 2063 7572  If None uses cur
-0000f510: 7265 6e74 2074 696d 652e 0a20 2020 2020  rent time..     
-0000f520: 2020 2020 2020 206c 6f67 6769 6e67 3a20         logging: 
-0000f530: 6469 7361 626c 6520 4744 5320 7061 7468  disable GDS path
-0000f540: 206c 6f67 6769 6e67 2c20 666f 7220 6578   logging, for ex
-0000f550: 616d 706c 6520 666f 7220 7368 6f77 696e  ample for showin
-0000f560: 6720 6974 2069 6e20 4b4c 6179 6f75 742e  g it in KLayout.
-0000f570: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0000f580: 685f 6f61 7369 733a 2049 6620 5472 7565  h_oasis: If True
-0000f590: 2c20 6669 6c65 2077 696c 6c20 6265 2077  , file will be w
-0000f5a0: 7269 7474 656e 2074 6f20 4f41 5349 532e  ritten to OASIS.
-0000f5b0: 204f 7468 6572 7769 7365 2c20 6669 6c65   Otherwise, file
-0000f5c0: 2077 696c 6c20 6265 2077 7269 7474 656e   will be written
-0000f5d0: 2074 6f20 4744 532e 0a20 2020 2020 2020   to GDS..       
-0000f5e0: 2020 2020 2077 6974 685f 6d65 7461 6461       with_metada
-0000f5f0: 7461 3a20 7772 6974 6573 206d 6574 6164  ta: writes metad
-0000f600: 6174 6120 696e 2059 414d 4c20 666f 726d  ata in YAML form
-0000f610: 6174 2e0a 0a20 2020 2020 2020 204b 6579  at...        Key
-0000f620: 776f 7264 2041 7267 733a 0a20 2020 2020  word Args:.     
-0000f630: 2020 2020 2020 204b 6579 776f 7264 2061         Keyword a
-0000f640: 7267 756d 656e 7473 2077 696c 6c20 6f76  rguments will ov
-0000f650: 6572 7269 6465 2074 6865 2061 6374 6976  erride the activ
-0000f660: 6520 5044 4b27 7320 6465 6661 756c 7420  e PDK's default 
-0000f670: 4764 7357 7269 7465 5365 7474 696e 6773  GdsWriteSettings
-0000f680: 2061 6e64 204f 6173 6973 5772 6974 6553   and OasisWriteS
-0000f690: 6574 7469 6e67 732e 0a0a 2020 2020 2020  ettings...      
-0000f6a0: 2020 2020 2020 4764 7320 7365 7474 696e        Gds settin
-0000f6b0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000f6c0: 2020 2020 756e 6974 3a20 756e 6974 2073      unit: unit s
-0000f6d0: 697a 6520 666f 7220 6f62 6a65 6374 7320  ize for objects 
-0000f6e0: 696e 206c 6962 7261 7279 2e20 3175 6d20  in library. 1um 
-0000f6f0: 6279 2064 6566 6175 6c74 2e0a 2020 2020  by default..    
-0000f700: 2020 2020 2020 2020 2020 2020 7072 6563              prec
-0000f710: 6973 696f 6e3a 2066 6f72 2064 696d 656e  ision: for dimen
-0000f720: 7369 6f6e 7320 696e 2074 6865 206c 6962  sions in the lib
-0000f730: 7261 7279 2028 6d29 2e20 316e 6d20 6279  rary (m). 1nm by
-0000f740: 2064 6566 6175 6c74 2e0a 2020 2020 2020   default..      
-0000f750: 2020 2020 2020 2020 2020 6f6e 5f64 7570            on_dup
-0000f760: 6c69 6361 7465 5f63 656c 6c3a 2073 7065  licate_cell: spe
-0000f770: 6369 6679 2068 6f77 2074 6f20 7265 736f  cify how to reso
-0000f780: 6c76 6520 6475 706c 6963 6174 652d 6e61  lve duplicate-na
-0000f790: 6d65 6420 6365 6c6c 732e 2043 686f 6f73  med cells. Choos
-0000f7a0: 6520 6f6e 6520 6f66 2074 6865 2066 6f6c  e one of the fol
-0000f7b0: 6c6f 7769 6e67 3a0a 2020 2020 2020 2020  lowing:.        
-0000f7c0: 2020 2020 2020 2020 2020 2020 2277 6172              "war
-0000f7d0: 6e22 2028 6465 6661 756c 7429 3a20 6f76  n" (default): ov
-0000f7e0: 6572 7772 6974 6520 616c 6c20 6475 706c  erwrite all dupl
-0000f7f0: 6963 6174 6520 6365 6c6c 7320 7769 7468  icate cells with
-0000f800: 206f 6e65 206f 6620 7468 6520 6475 706c   one of the dupl
-0000f810: 6963 6174 6573 2028 6172 6269 7472 6172  icates (arbitrar
-0000f820: 696c 7929 2e0a 2020 2020 2020 2020 2020  ily)..          
-0000f830: 2020 2020 2020 2020 2020 2265 7272 6f72            "error
-0000f840: 223a 2074 6872 6f77 2061 2056 616c 7565  ": throw a Value
-0000f850: 4572 726f 7220 7768 656e 2061 7474 656d  Error when attem
-0000f860: 7074 696e 6720 746f 2077 7269 7465 2061  pting to write a
-0000f870: 2067 6473 2077 6974 6820 6475 706c 6963   gds with duplic
-0000f880: 6174 6520 6365 6c6c 732e 0a20 2020 2020  ate cells..     
-0000f890: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000f8a0: 6f76 6572 7772 6974 6522 3a20 6f76 6572  overwrite": over
-0000f8b0: 7772 6974 6520 616c 6c20 6475 706c 6963  write all duplic
-0000f8c0: 6174 6520 6365 6c6c 7320 7769 7468 206f  ate cells with o
-0000f8d0: 6e65 206f 6620 7468 6520 6475 706c 6963  ne of the duplic
-0000f8e0: 6174 6573 2c20 7769 7468 6f75 7420 7761  ates, without wa
-0000f8f0: 726e 696e 672e 0a20 2020 2020 2020 2020  rning..         
-0000f900: 2020 2020 2020 2020 2020 204e 6f6e 653a             None:
-0000f910: 2064 6f20 6e6f 7420 7472 7920 746f 2072   do not try to r
-0000f920: 6573 6f6c 7665 2028 6174 2079 6f75 7220  esolve (at your 
-0000f930: 6f77 6e20 7269 736b 2129 0a20 2020 2020  own risk!).     
-0000f940: 2020 2020 2020 2020 2020 2066 6c61 7474             flatt
-0000f950: 656e 5f69 6e76 616c 6964 5f72 6566 733a  en_invalid_refs:
-0000f960: 2066 6c61 7474 656e 7320 636f 6d70 6f6e   flattens compon
-0000f970: 656e 7420 7265 6665 7265 6e63 6573 2077  ent references w
-0000f980: 6869 6368 2068 6176 6520 696e 7661 6c69  hich have invali
-0000f990: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
-0000f9a0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-0000f9b0: 2020 206d 6178 5f70 6f69 6e74 733a 204d     max_points: M
-0000f9c0: 6178 696d 616c 206e 756d 6265 7220 6f66  aximal number of
-0000f9d0: 2076 6572 7469 6365 7320 7065 7220 706f   vertices per po
-0000f9e0: 6c79 676f 6e2e 2050 6f6c 7967 6f6e 7320  lygon. Polygons 
-0000f9f0: 7769 7468 206d 6f72 6520 7665 7274 6963  with more vertic
-0000fa00: 6573 2074 6861 7420 7468 6973 2061 7265  es that this are
-0000fa10: 2061 7574 6f6d 6174 6963 616c 6c79 2066   automatically f
-0000fa20: 7261 6374 7572 6564 2e0a 0a20 2020 2020  ractured...     
-0000fa30: 2020 2020 2020 204f 6173 6973 2073 6574         Oasis set
-0000fa40: 7469 6e67 733a 0a20 2020 2020 2020 2020  tings:.         
-0000fa50: 2020 2020 2020 2063 6f6d 7072 6573 7369         compressi
-0000fa60: 6f6e 5f6c 6576 656c 3a20 4c65 7665 6c20  on_level: Level 
-0000fa70: 6f66 2063 6f6d 7072 6573 7369 6f6e 2066  of compression f
-0000fa80: 6f72 2063 656c 6c73 2028 6265 7477 6565  or cells (betwee
-0000fa90: 6e20 3020 616e 6420 3929 2e0a 2020 2020  n 0 and 9)..    
-0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fab0: 5365 7474 696e 6720 746f 2030 2077 696c  Setting to 0 wil
-0000fac0: 6c20 6469 7361 626c 6520 6365 6c6c 2063  l disable cell c
-0000fad0: 6f6d 7072 6573 7369 6f6e 2c20 3120 6769  ompression, 1 gi
-0000fae0: 7665 7320 7468 6520 6265 7374 2073 7065  ves the best spe
-0000faf0: 6564 2061 6e64 2039 2c20 7468 6520 6265  ed and 9, the be
-0000fb00: 7374 2063 6f6d 7072 6573 7369 6f6e 2e0a  st compression..
-0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb20: 6465 7465 6374 5f72 6563 7461 6e67 6c65  detect_rectangle
-0000fb30: 733a 2053 746f 7265 2072 6563 7461 6e67  s: Store rectang
-0000fb40: 6c65 7320 696e 2063 6f6d 7072 6573 7365  les in compresse
-0000fb50: 6420 666f 726d 6174 2e0a 2020 2020 2020  d format..      
-0000fb60: 2020 2020 2020 2020 2020 6465 7465 6374            detect
-0000fb70: 5f74 7261 7065 7a6f 6964 733a 2053 746f  _trapezoids: Sto
-0000fb80: 7265 2074 7261 7065 7a6f 6964 7320 696e  re trapezoids in
-0000fb90: 2063 6f6d 7072 6573 7365 6420 666f 726d   compressed form
-0000fba0: 6174 2e0a 2020 2020 2020 2020 2020 2020  at..            
-0000fbb0: 2020 2020 6369 7263 6c65 5f74 6f6c 6572      circle_toler
-0000fbc0: 616e 6365 3a20 546f 6c65 7261 6e63 6520  ance: Tolerance 
-0000fbd0: 666f 7220 6465 7465 6374 696e 6720 6369  for detecting ci
-0000fbe0: 7263 6c65 732e 2049 6620 6c65 7373 206f  rcles. If less o
-0000fbf0: 7220 6571 7561 6c20 746f 2030 2c20 6e6f  r equal to 0, no
-0000fc00: 2064 6574 6563 7469 6f6e 2069 7320 7065   detection is pe
-0000fc10: 7266 6f72 6d65 642e 2043 6972 636c 6573  rformed. Circles
-0000fc20: 2061 7265 2073 746f 7265 6420 696e 2063   are stored in c
-0000fc30: 6f6d 7072 6573 7365 6420 666f 726d 6174  ompressed format
-0000fc40: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fc50: 2020 7661 6c69 6461 7469 6f6e 2028 2263    validation ("c
-0000fc60: 7263 3332 222c 2022 6368 6563 6b73 756d  rc32", "checksum
-0000fc70: 3332 222c 204e 6f6e 6529 3a20 7479 7065  32", None): type
-0000fc80: 206f 6620 7661 6c69 6461 7469 6f6e 2074   of validation t
-0000fc90: 6f20 696e 636c 7564 6520 696e 2074 6865  o include in the
-0000fca0: 2073 6176 6564 2066 696c 652e 0a20 2020   saved file..   
-0000fcb0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-0000fcc0: 6e64 6172 645f 7072 6f70 6572 7469 6573  ndard_properties
-0000fcd0: 3a20 5374 6f72 6520 7374 616e 6461 7264  : Store standard
-0000fce0: 204f 4153 4953 2070 726f 7065 7274 6965   OASIS propertie
-0000fcf0: 7320 696e 2074 6865 2066 696c 652e 0a0a  s in the file...
-0000fd00: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0000fd10: 2020 2020 2066 726f 6d20 6764 7366 6163       from gdsfac
-0000fd20: 746f 7279 2e70 646b 2069 6d70 6f72 7420  tory.pdk import 
-0000fd30: 6765 745f 6163 7469 7665 5f70 646b 0a0a  get_active_pdk..
-0000fd40: 2020 2020 2020 2020 6966 2067 6473 7061          if gdspa
-0000fd50: 7468 2061 6e64 2067 6473 6469 723a 0a20  th and gdsdir:. 
-0000fd60: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-0000fd70: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
-0000fd80: 2020 2020 2020 2020 2020 2267 6473 7061            "gdspa
-0000fd90: 7468 2061 6e64 2067 6473 6469 7220 6861  th and gdsdir ha
-0000fda0: 7665 2062 6f74 6820 6265 656e 2073 7065  ve both been spe
-0000fdb0: 6369 6669 6564 2e20 6764 7370 6174 6820  cified. gdspath 
-0000fdc0: 7769 6c6c 2074 616b 6520 7072 6563 6564  will take preced
-0000fdd0: 656e 6365 2061 6e64 2067 6473 6469 7220  ence and gdsdir 
-0000fde0: 7769 6c6c 2062 6520 6967 6e6f 7265 642e  will be ignored.
-0000fdf0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000fe00: 2020 2073 7461 636b 6c65 7665 6c3d 332c     stacklevel=3,
-0000fe10: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000fe20: 2020 2020 2020 2020 6465 6661 756c 745f          default_
-0000fe30: 7365 7474 696e 6773 203d 2067 6574 5f61  settings = get_a
-0000fe40: 6374 6976 655f 7064 6b28 292e 6764 735f  ctive_pdk().gds_
-0000fe50: 7772 6974 655f 7365 7474 696e 6773 0a20  write_settings. 
-0000fe60: 2020 2020 2020 2064 6566 6175 6c74 5f6f         default_o
-0000fe70: 6173 6973 5f73 6574 7469 6e67 7320 3d20  asis_settings = 
-0000fe80: 6765 745f 6163 7469 7665 5f70 646b 2829  get_active_pdk()
-0000fe90: 2e6f 6173 6973 5f73 6574 7469 6e67 730a  .oasis_settings.
-0000fea0: 0a20 2020 2020 2020 2065 7870 6c69 6369  .        explici
-0000feb0: 745f 6764 735f 7365 7474 696e 6773 203d  t_gds_settings =
-0000fec0: 207b 0a20 2020 2020 2020 2020 2020 206b   {.            k
-0000fed0: 3a20 760a 2020 2020 2020 2020 2020 2020  : v.            
-0000fee0: 666f 7220 6b2c 2076 2069 6e20 6b77 6172  for k, v in kwar
-0000fef0: 6773 2e69 7465 6d73 2829 0a20 2020 2020  gs.items().     
-0000ff00: 2020 2020 2020 2069 6620 7620 6973 206e         if v is n
-0000ff10: 6f74 204e 6f6e 6520 616e 6420 6b20 696e  ot None and k in
-0000ff20: 2064 6566 6175 6c74 5f73 6574 7469 6e67   default_setting
-0000ff30: 732e 6469 6374 2829 0a20 2020 2020 2020  s.dict().       
-0000ff40: 207d 0a20 2020 2020 2020 2065 7870 6c69   }.        expli
-0000ff50: 6369 745f 6f61 735f 7365 7474 696e 6773  cit_oas_settings
-0000ff60: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0000ff70: 206b 3a20 760a 2020 2020 2020 2020 2020   k: v.          
-0000ff80: 2020 666f 7220 6b2c 2076 2069 6e20 6b77    for k, v in kw
-0000ff90: 6172 6773 2e69 7465 6d73 2829 0a20 2020  args.items().   
-0000ffa0: 2020 2020 2020 2020 2069 6620 7620 6973           if v is
-0000ffb0: 206e 6f74 204e 6f6e 6520 616e 6420 6b20   not None and k 
-0000ffc0: 696e 2064 6566 6175 6c74 5f6f 6173 6973  in default_oasis
-0000ffd0: 5f73 6574 7469 6e67 732e 6469 6374 2829  _settings.dict()
-0000ffe0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-0000fff0: 2020 2023 2075 7064 6174 6520 7468 6520     # update the 
-00010000: 7772 6974 6520 7365 7474 696e 6773 2077  write settings w
-00010010: 6974 6820 616e 7920 7365 7474 696e 6773  ith any settings
-00010020: 2065 7870 6c69 6369 746c 7920 7061 7373   explicitly pass
-00010030: 6564 0a20 2020 2020 2020 2077 7269 7465  ed.        write
-00010040: 5f73 6574 7469 6e67 7320 3d20 6465 6661  _settings = defa
-00010050: 756c 745f 7365 7474 696e 6773 2e63 6f70  ult_settings.cop
-00010060: 7928 7570 6461 7465 3d65 7870 6c69 6369  y(update=explici
-00010070: 745f 6764 735f 7365 7474 696e 6773 290a  t_gds_settings).
-00010080: 2020 2020 2020 2020 6f61 7369 735f 7365          oasis_se
-00010090: 7474 696e 6773 203d 2064 6566 6175 6c74  ttings = default
-000100a0: 5f6f 6173 6973 5f73 6574 7469 6e67 732e  _oasis_settings.
-000100b0: 636f 7079 2875 7064 6174 653d 6578 706c  copy(update=expl
-000100c0: 6963 6974 5f6f 6173 5f73 6574 7469 6e67  icit_oas_setting
-000100d0: 7329 0a0a 2020 2020 2020 2020 5f63 6865  s)..        _che
-000100e0: 636b 5f75 6e63 6163 6865 645f 636f 6d70  ck_uncached_comp
-000100f0: 6f6e 656e 7473 280a 2020 2020 2020 2020  onents(.        
-00010100: 2020 2020 636f 6d70 6f6e 656e 743d 7365      component=se
-00010110: 6c66 2c20 6d6f 6465 3d77 7269 7465 5f73  lf, mode=write_s
-00010120: 6574 7469 6e67 732e 6f6e 5f75 6e63 6163  ettings.on_uncac
-00010130: 6865 645f 636f 6d70 6f6e 656e 740a 2020  hed_component.  
-00010140: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00010150: 2069 6620 7772 6974 655f 7365 7474 696e   if write_settin
-00010160: 6773 2e66 6c61 7474 656e 5f69 6e76 616c  gs.flatten_inval
-00010170: 6964 5f72 6566 733a 0a20 2020 2020 2020  id_refs:.       
-00010180: 2020 2020 2074 6f70 5f63 656c 6c20 3d20       top_cell = 
-00010190: 666c 6174 7465 6e5f 696e 7661 6c69 645f  flatten_invalid_
-000101a0: 7265 6673 5f72 6563 7572 7369 7665 2873  refs_recursive(s
-000101b0: 656c 6629 0a20 2020 2020 2020 2065 6c73  elf).        els
-000101c0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-000101d0: 6f70 5f63 656c 6c20 3d20 7365 6c66 0a0a  op_cell = self..
-000101e0: 2020 2020 2020 2020 6764 7364 6972 203d          gdsdir =
-000101f0: 2067 6473 6469 7220 6f72 2047 4453 4449   gdsdir or GDSDI
-00010200: 525f 5445 4d50 0a20 2020 2020 2020 2067  R_TEMP.        g
-00010210: 6473 6469 7220 3d20 7061 7468 6c69 622e  dsdir = pathlib.
-00010220: 5061 7468 2867 6473 6469 7229 0a20 2020  Path(gdsdir).   
-00010230: 2020 2020 2069 6620 7769 7468 5f6f 6173       if with_oas
-00010240: 6973 3a0a 2020 2020 2020 2020 2020 2020  is:.            
-00010250: 6764 7370 6174 6820 3d20 6764 7370 6174  gdspath = gdspat
-00010260: 6820 6f72 2067 6473 6469 7220 2f20 6622  h or gdsdir / f"
-00010270: 7b74 6f70 5f63 656c 6c2e 6e61 6d65 7d2e  {top_cell.name}.
-00010280: 6f61 7322 0a20 2020 2020 2020 2065 6c73  oas".        els
-00010290: 653a 0a20 2020 2020 2020 2020 2020 2067  e:.            g
-000102a0: 6473 7061 7468 203d 2067 6473 7061 7468  dspath = gdspath
-000102b0: 206f 7220 6764 7364 6972 202f 2066 227b   or gdsdir / f"{
-000102c0: 746f 705f 6365 6c6c 2e6e 616d 657d 2e67  top_cell.name}.g
-000102d0: 6473 220a 2020 2020 2020 2020 6764 7370  ds".        gdsp
-000102e0: 6174 6820 3d20 7061 7468 6c69 622e 5061  ath = pathlib.Pa
-000102f0: 7468 2867 6473 7061 7468 290a 2020 2020  th(gdspath).    
-00010300: 2020 2020 6764 7364 6972 203d 2067 6473      gdsdir = gds
-00010310: 7061 7468 2e70 6172 656e 740a 2020 2020  path.parent.    
-00010320: 2020 2020 6764 7364 6972 2e6d 6b64 6972      gdsdir.mkdir
-00010330: 2865 7869 7374 5f6f 6b3d 5472 7565 2c20  (exist_ok=True, 
-00010340: 7061 7265 6e74 733d 5472 7565 290a 0a20  parents=True).. 
-00010350: 2020 2020 2020 2063 656c 6c73 203d 2074         cells = t
-00010360: 6f70 5f63 656c 6c2e 6765 745f 6465 7065  op_cell.get_depe
-00010370: 6e64 656e 6369 6573 2872 6563 7572 7369  ndencies(recursi
-00010380: 7665 3d54 7275 6529 0a20 2020 2020 2020  ve=True).       
-00010390: 2063 656c 6c5f 6e61 6d65 7320 3d20 5b63   cell_names = [c
-000103a0: 656c 6c2e 6e61 6d65 2066 6f72 2063 656c  ell.name for cel
-000103b0: 6c20 696e 206c 6973 7428 6365 6c6c 7329  l in list(cells)
-000103c0: 5d0a 2020 2020 2020 2020 6365 6c6c 5f6e  ].        cell_n
-000103d0: 616d 6573 5f75 6e69 7175 6520 3d20 7365  ames_unique = se
-000103e0: 7428 6365 6c6c 5f6e 616d 6573 290a 0a20  t(cell_names).. 
-000103f0: 2020 2020 2020 2069 6620 6c65 6e28 6365         if len(ce
-00010400: 6c6c 5f6e 616d 6573 2920 213d 206c 656e  ll_names) != len
-00010410: 2873 6574 2863 656c 6c5f 6e61 6d65 7329  (set(cell_names)
-00010420: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-00010430: 6f72 2063 656c 6c5f 6e61 6d65 2069 6e20  or cell_name in 
-00010440: 6365 6c6c 5f6e 616d 6573 5f75 6e69 7175  cell_names_uniqu
-00010450: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00010460: 2020 2063 656c 6c5f 6e61 6d65 732e 7265     cell_names.re
-00010470: 6d6f 7665 2863 656c 6c5f 6e61 6d65 290a  move(cell_name).
-00010480: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00010490: 7772 6974 655f 7365 7474 696e 6773 2e6f  write_settings.o
-000104a0: 6e5f 6475 706c 6963 6174 655f 6365 6c6c  n_duplicate_cell
-000104b0: 203d 3d20 2265 7272 6f72 223a 0a20 2020   == "error":.   
-000104c0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-000104d0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104f0: 2020 2066 2244 7570 6c69 6361 7465 6420     f"Duplicated 
-00010500: 6365 6c6c 206e 616d 6573 2069 6e20 7b74  cell names in {t
-00010510: 6f70 5f63 656c 6c2e 6e61 6d65 2172 7d3a  op_cell.name!r}:
-00010520: 207b 6365 6c6c 5f6e 616d 6573 2172 7d22   {cell_names!r}"
-00010530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010540: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
-00010550: 6c69 6620 7772 6974 655f 7365 7474 696e  lif write_settin
-00010560: 6773 2e6f 6e5f 6475 706c 6963 6174 655f  gs.on_duplicate_
-00010570: 6365 6c6c 2069 6e20 7b22 7761 726e 222c  cell in {"warn",
-00010580: 2022 6f76 6572 7772 6974 6522 7d3a 0a20   "overwrite"}:. 
-00010590: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000105a0: 6620 7772 6974 655f 7365 7474 696e 6773  f write_settings
-000105b0: 2e6f 6e5f 6475 706c 6963 6174 655f 6365  .on_duplicate_ce
-000105c0: 6c6c 203d 3d20 2277 6172 6e22 3a0a 2020  ll == "warn":.  
-000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105e0: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-000105f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010600: 2020 2020 2020 2020 2066 2244 7570 6c69           f"Dupli
-00010610: 6361 7465 6420 6365 6c6c 206e 616d 6573  cated cell names
-00010620: 2069 6e20 7b74 6f70 5f63 656c 6c2e 6e61   in {top_cell.na
-00010630: 6d65 2172 7d3a 2020 7b63 656c 6c5f 6e61  me!r}:  {cell_na
-00010640: 6d65 737d 222c 0a20 2020 2020 2020 2020  mes}",.         
-00010650: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010660: 7461 636b 6c65 7665 6c3d 332c 0a20 2020  tacklevel=3,.   
-00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010680: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00010690: 2020 2063 656c 6c73 5f64 6963 7420 3d20     cells_dict = 
-000106a0: 7b63 656c 6c2e 6e61 6d65 3a20 6365 6c6c  {cell.name: cell
-000106b0: 2e5f 6365 6c6c 2066 6f72 2063 656c 6c20  ._cell for cell 
-000106c0: 696e 2063 656c 6c73 7d0a 2020 2020 2020  in cells}.      
-000106d0: 2020 2020 2020 2020 2020 6365 6c6c 7320            cells 
-000106e0: 3d20 6365 6c6c 735f 6469 6374 2e76 616c  = cells_dict.val
-000106f0: 7565 7328 290a 2020 2020 2020 2020 2020  ues().          
-00010700: 2020 656c 6966 2077 7269 7465 5f73 6574    elif write_set
-00010710: 7469 6e67 732e 6f6e 5f64 7570 6c69 6361  tings.on_duplica
-00010720: 7465 5f63 656c 6c20 6973 206e 6f74 204e  te_cell is not N
-00010730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00010740: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00010750: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00010760: 2020 2020 2020 2020 2020 2066 226f 6e5f             f"on_
-00010770: 6475 706c 6963 6174 655f 6365 6c6c 3a20  duplicate_cell: 
-00010780: 7b77 7269 7465 5f73 6574 7469 6e67 732e  {write_settings.
-00010790: 6f6e 5f64 7570 6c69 6361 7465 5f63 656c  on_duplicate_cel
-000107a0: 6c21 727d 206e 6f74 2069 6e20 284e 6f6e  l!r} not in (Non
-000107b0: 652c 2077 6172 6e2c 2065 7272 6f72 2c20  e, warn, error, 
-000107c0: 6f76 6572 7772 6974 6529 220a 2020 2020  overwrite)".    
-000107d0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000107e0: 2020 2020 2020 2061 6c6c 5f63 656c 6c73         all_cells
-000107f0: 203d 205b 746f 705f 6365 6c6c 2e5f 6365   = [top_cell._ce
-00010800: 6c6c 5d20 2b20 736f 7274 6564 2863 656c  ll] + sorted(cel
-00010810: 6c73 2c20 6b65 793d 6c61 6d62 6461 2063  ls, key=lambda c
-00010820: 633a 2063 632e 6e61 6d65 290a 0a20 2020  c: cc.name)..   
-00010830: 2020 2020 206e 6f5f 6e61 6d65 5f63 656c       no_name_cel
-00010840: 6c73 203d 205b 0a20 2020 2020 2020 2020  ls = [.         
-00010850: 2020 2063 656c 6c2e 6e61 6d65 2066 6f72     cell.name for
-00010860: 2063 656c 6c20 696e 2061 6c6c 5f63 656c   cell in all_cel
-00010870: 6c73 2069 6620 6365 6c6c 2e6e 616d 652e  ls if cell.name.
-00010880: 7374 6172 7473 7769 7468 2822 556e 6e61  startswith("Unna
-00010890: 6d65 6422 290a 2020 2020 2020 2020 5d0a  med").        ].
-000108a0: 0a20 2020 2020 2020 2069 6620 6e6f 5f6e  .        if no_n
-000108b0: 616d 655f 6365 6c6c 733a 0a20 2020 2020  ame_cells:.     
-000108c0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-000108d0: 7761 726e 280a 2020 2020 2020 2020 2020  warn(.          
-000108e0: 2020 2020 2020 6622 436f 6d70 6f6e 656e        f"Componen
-000108f0: 7420 7b74 6f70 5f63 656c 6c2e 6e61 6d65  t {top_cell.name
-00010900: 2172 7d20 636f 6e74 6169 6e73 207b 6c65  !r} contains {le
-00010910: 6e28 6e6f 5f6e 616d 655f 6365 6c6c 7329  n(no_name_cells)
-00010920: 7d20 556e 6e61 6d65 6420 6365 6c6c 7322  } Unnamed cells"
-00010930: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010940: 2020 7374 6163 6b6c 6576 656c 3d33 2c0a    stacklevel=3,.
-00010950: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00010960: 2020 2020 2020 2023 2066 6f72 2063 656c         # for cel
-00010970: 6c20 696e 2061 6c6c 5f63 656c 6c73 3a0a  l in all_cells:.
-00010980: 2020 2020 2020 2020 2320 2020 2020 7072          #     pr
-00010990: 696e 7428 6365 6c6c 2e6e 616d 652c 2074  int(cell.name, t
-000109a0: 7970 6528 6365 6c6c 2929 0a0a 2020 2020  ype(cell))..    
-000109b0: 2020 2020 6c69 6220 3d20 6764 7374 6b2e      lib = gdstk.
-000109c0: 4c69 6272 6172 7928 0a20 2020 2020 2020  Library(.       
-000109d0: 2020 2020 206e 616d 653d 7772 6974 655f       name=write_
-000109e0: 7365 7474 696e 6773 2e6c 6962 5f6e 616d  settings.lib_nam
-000109f0: 652c 0a20 2020 2020 2020 2020 2020 2075  e,.            u
-00010a00: 6e69 743d 7772 6974 655f 7365 7474 696e  nit=write_settin
-00010a10: 6773 2e75 6e69 742c 0a20 2020 2020 2020  gs.unit,.       
-00010a20: 2020 2020 2070 7265 6369 7369 6f6e 3d77       precision=w
-00010a30: 7269 7465 5f73 6574 7469 6e67 732e 7072  rite_settings.pr
-00010a40: 6563 6973 696f 6e2c 0a20 2020 2020 2020  ecision,.       
-00010a50: 2029 0a20 2020 2020 2020 206c 6962 2e61   ).        lib.a
-00010a60: 6464 2874 6f70 5f63 656c 6c2e 5f63 656c  dd(top_cell._cel
-00010a70: 6c29 0a20 2020 2020 2020 206c 6962 2e61  l).        lib.a
-00010a80: 6464 282a 746f 705f 6365 6c6c 2e5f 6365  dd(*top_cell._ce
-00010a90: 6c6c 2e64 6570 656e 6465 6e63 6965 7328  ll.dependencies(
-00010aa0: 5472 7565 2929 0a0a 2020 2020 2020 2020  True))..        
-00010ab0: 6966 2077 6974 685f 6f61 7369 733a 0a20  if with_oasis:. 
-00010ac0: 2020 2020 2020 2020 2020 206c 6962 2e77             lib.w
-00010ad0: 7269 7465 5f6f 6173 2867 6473 7061 7468  rite_oas(gdspath
-00010ae0: 2c20 2a2a 6f61 7369 735f 7365 7474 696e  , **oasis_settin
-00010af0: 6773 2e64 6963 7428 2929 0a20 2020 2020  gs.dict()).     
-00010b00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00010b10: 2020 2020 206c 6962 2e77 7269 7465 5f67       lib.write_g
-00010b20: 6473 280a 2020 2020 2020 2020 2020 2020  ds(.            
-00010b30: 2020 2020 6764 7370 6174 682c 2074 696d      gdspath, tim
-00010b40: 6573 7461 6d70 3d74 696d 6573 7461 6d70  estamp=timestamp
-00010b50: 2c20 6d61 785f 706f 696e 7473 3d77 7269  , max_points=wri
-00010b60: 7465 5f73 6574 7469 6e67 732e 6d61 785f  te_settings.max_
-00010b70: 706f 696e 7473 0a20 2020 2020 2020 2020  points.         
-00010b80: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-00010b90: 6c6f 6767 696e 673a 0a20 2020 2020 2020  logging:.       
-00010ba0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00010bb0: 2866 2257 726f 7465 2074 6f20 7b73 7472  (f"Wrote to {str
-00010bc0: 2867 6473 7061 7468 2921 727d 2229 0a20  (gdspath)!r}"). 
-00010bd0: 2020 2020 2020 2069 6620 7769 7468 5f6d         if with_m
-00010be0: 6574 6164 6174 613a 0a20 2020 2020 2020  etadata:.       
-00010bf0: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
-00010c00: 6764 7370 6174 682e 7769 7468 5f73 7566  gdspath.with_suf
-00010c10: 6669 7828 222e 796d 6c22 290a 2020 2020  fix(".yml").    
-00010c20: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-00010c30: 2e77 7269 7465 5f74 6578 7428 7365 6c66  .write_text(self
-00010c40: 2e74 6f5f 7961 6d6c 2877 6974 685f 6365  .to_yaml(with_ce
-00010c50: 6c6c 733d 5472 7565 2c20 7769 7468 5f70  lls=True, with_p
-00010c60: 6f72 7473 3d54 7275 6529 290a 2020 2020  orts=True)).    
-00010c70: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00010c80: 6e66 6f28 6622 5772 6974 6520 5941 4d4c  nfo(f"Write YAML
-00010c90: 206d 6574 6164 6174 6120 746f 207b 7374   metadata to {st
-00010ca0: 7228 6d65 7461 6461 7461 2921 727d 2229  r(metadata)!r}")
-00010cb0: 0a0a 2020 2020 2020 2020 434f 4e46 2e6c  ..        CONF.l
-00010cc0: 6173 745f 7361 7665 645f 6669 6c65 732e  ast_saved_files.
-00010cd0: 6170 7065 6e64 2867 6473 7061 7468 290a  append(gdspath).
-00010ce0: 2020 2020 2020 2020 7265 7475 726e 2067          return g
-00010cf0: 6473 7061 7468 0a0a 2020 2020 6465 6620  dspath..    def 
-00010d00: 7772 6974 655f 6764 7328 0a20 2020 2020  write_gds(.     
-00010d10: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00010d20: 2067 6473 7061 7468 3a20 5061 7468 5479   gdspath: PathTy
-00010d30: 7065 207c 204e 6f6e 6520 3d20 4e6f 6e65  pe | None = None
-00010d40: 2c0a 2020 2020 2020 2020 6764 7364 6972  ,.        gdsdir
-00010d50: 3a20 5061 7468 5479 7065 207c 204e 6f6e  : PathType | Non
-00010d60: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-00010d70: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
-00010d80: 2920 2d3e 2050 6174 683a 0a20 2020 2020  ) -> Path:.     
-00010d90: 2020 2022 2222 5772 6974 6520 636f 6d70     """Write comp
-00010da0: 6f6e 656e 7420 746f 2047 4453 2061 6e64  onent to GDS and
-00010db0: 2072 6574 7572 6e73 2067 6473 7061 7468   returns gdspath
-00010dc0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00010dd0: 0a20 2020 2020 2020 2020 2020 2067 6473  .            gds
-00010de0: 7061 7468 3a20 4744 5320 6669 6c65 2070  path: GDS file p
-00010df0: 6174 6820 746f 2077 7269 7465 2074 6f2e  ath to write to.
-00010e00: 0a20 2020 2020 2020 2020 2020 2067 6473  .            gds
-00010e10: 6469 723a 2064 6972 6563 746f 7279 2066  dir: directory f
-00010e20: 6f72 2074 6865 2047 4453 2066 696c 652e  or the GDS file.
-00010e30: 2044 6566 6175 6c74 7320 746f 202f 746d   Defaults to /tm
-00010e40: 702f 7261 6e64 6f6d 4669 6c65 2f67 6473  p/randomFile/gds
-00010e50: 6661 6374 6f72 792e 0a0a 2020 2020 2020  factory...      
-00010e60: 2020 4b65 7977 6f72 6420 4172 6773 3a0a    Keyword Args:.
-00010e70: 2020 2020 2020 2020 2020 2020 756e 6974              unit
-00010e80: 3a20 756e 6974 2073 697a 6520 666f 7220  : unit size for 
-00010e90: 6f62 6a65 6374 7320 696e 206c 6962 7261  objects in libra
-00010ea0: 7279 2e20 3175 6d20 6279 2064 6566 6175  ry. 1um by defau
-00010eb0: 6c74 2e0a 2020 2020 2020 2020 2020 2020  lt..            
-00010ec0: 7072 6563 6973 696f 6e3a 2066 6f72 2064  precision: for d
-00010ed0: 696d 656e 7369 6f6e 7320 696e 2074 6865  imensions in the
-00010ee0: 206c 6962 7261 7279 2028 6d29 2e20 316e   library (m). 1n
-00010ef0: 6d20 6279 2064 6566 6175 6c74 2e0a 2020  m by default..  
-00010f00: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
-00010f10: 673a 2064 6973 6162 6c65 2047 4453 2070  g: disable GDS p
-00010f20: 6174 6820 6c6f 6767 696e 672c 2066 6f72  ath logging, for
-00010f30: 2065 7861 6d70 6c65 2066 6f72 2073 686f   example for sho
-00010f40: 7769 6e67 2069 7420 696e 204b 4c61 796f  wing it in KLayo
-00010f50: 7574 2e0a 2020 2020 2020 2020 2020 2020  ut..            
-00010f60: 6f6e 5f64 7570 6c69 6361 7465 5f63 656c  on_duplicate_cel
-00010f70: 6c3a 2073 7065 6369 6679 2068 6f77 2074  l: specify how t
-00010f80: 6f20 7265 736f 6c76 6520 6475 706c 6963  o resolve duplic
-00010f90: 6174 652d 6e61 6d65 6420 6365 6c6c 732e  ate-named cells.
-00010fa0: 2043 686f 6f73 6520 6f6e 6520 6f66 2074   Choose one of t
-00010fb0: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 2020  he following:.  
-00010fc0: 2020 2020 2020 2020 2020 2020 2020 2277                "w
-00010fd0: 6172 6e22 2028 6465 6661 756c 7429 3a20  arn" (default): 
-00010fe0: 6f76 6572 7772 6974 6520 616c 6c20 6475  overwrite all du
-00010ff0: 706c 6963 6174 6520 6365 6c6c 7320 7769  plicate cells wi
-00011000: 7468 206f 6e65 206f 6620 7468 6520 6475  th one of the du
-00011010: 706c 6963 6174 6573 2028 6172 6269 7472  plicates (arbitr
-00011020: 6172 696c 7929 2e0a 2020 2020 2020 2020  arily)..        
-00011030: 2020 2020 2020 2020 2265 7272 6f72 223a          "error":
-00011040: 2074 6872 6f77 2061 2056 616c 7565 4572   throw a ValueEr
-00011050: 726f 7220 7768 656e 2061 7474 656d 7074  ror when attempt
-00011060: 696e 6720 746f 2077 7269 7465 2061 2067  ing to write a g
-00011070: 6473 2077 6974 6820 6475 706c 6963 6174  ds with duplicat
-00011080: 6520 6365 6c6c 732e 0a20 2020 2020 2020  e cells..       
-00011090: 2020 2020 2020 2020 2022 6f76 6572 7772           "overwr
-000110a0: 6974 6522 3a20 6f76 6572 7772 6974 6520  ite": overwrite 
-000110b0: 616c 6c20 6475 706c 6963 6174 6520 6365  all duplicate ce
-000110c0: 6c6c 7320 7769 7468 206f 6e65 206f 6620  lls with one of 
-000110d0: 7468 6520 6475 706c 6963 6174 6573 2c20  the duplicates, 
-000110e0: 7769 7468 6f75 7420 7761 726e 696e 672e  without warning.
-000110f0: 0a20 2020 2020 2020 2020 2020 206f 6e5f  .            on_
-00011100: 756e 6361 6368 6564 5f63 6f6d 706f 6e65  uncached_compone
-00011110: 6e74 3a20 4c69 7465 7261 6c5b 2277 6172  nt: Literal["war
-00011120: 6e22 2c20 2265 7272 6f72 225d 203d 2022  n", "error"] = "
-00011130: 7761 726e 220a 2020 2020 2020 2020 2020  warn".          
-00011140: 2020 666c 6174 7465 6e5f 696e 7661 6c69    flatten_invali
-00011150: 645f 7265 6673 3a20 666c 6174 7465 6e73  d_refs: flattens
-00011160: 2063 6f6d 706f 6e65 6e74 2072 6566 6572   component refer
-00011170: 656e 6365 7320 7768 6963 6820 6861 7665  ences which have
-00011180: 2069 6e76 616c 6964 2074 7261 6e73 666f   invalid transfo
-00011190: 726d 6174 696f 6e73 2e0a 2020 2020 2020  rmations..      
-000111a0: 2020 2020 2020 6d61 785f 706f 696e 7473        max_points
-000111b0: 3a20 4d61 7869 6d61 6c20 6e75 6d62 6572  : Maximal number
-000111c0: 206f 6620 7665 7274 6963 6573 2070 6572   of vertices per
-000111d0: 2070 6f6c 7967 6f6e 2e0a 2020 2020 2020   polygon..      
-000111e0: 2020 2020 2020 2020 2020 506f 6c79 676f            Polygo
-000111f0: 6e73 2077 6974 6820 6d6f 7265 2076 6572  ns with more ver
-00011200: 7469 6365 7320 7468 6174 2074 6869 7320  tices that this 
-00011210: 6172 6520 6175 746f 6d61 7469 6361 6c6c  are automaticall
-00011220: 7920 6672 6163 7475 7265 642e 0a20 2020  y fractured..   
-00011230: 2020 2020 2020 2020 2077 6974 685f 6d65           with_me
-00011240: 7461 6461 7461 3a20 7772 6974 6573 206d  tadata: writes m
-00011250: 6574 6164 6174 6120 696e 2059 414d 4c20  etadata in YAML 
-00011260: 666f 726d 6174 2e0a 2020 2020 2020 2020  format..        
-00011270: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
-00011280: 7572 6e20 7365 6c66 2e5f 7772 6974 655f  urn self._write_
-00011290: 6c69 6272 6172 7928 0a20 2020 2020 2020  library(.       
-000112a0: 2020 2020 2067 6473 7061 7468 3d67 6473       gdspath=gds
-000112b0: 7061 7468 2c20 6764 7364 6972 3d67 6473  path, gdsdir=gds
-000112c0: 6469 722c 2077 6974 685f 6f61 7369 733d  dir, with_oasis=
-000112d0: 4661 6c73 652c 202a 2a6b 7761 7267 730a  False, **kwargs.
-000112e0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-000112f0: 6566 2077 7269 7465 5f6f 6173 280a 2020  ef write_oas(.  
-00011300: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00011310: 2020 2020 6764 7370 6174 683a 2050 6174      gdspath: Pat
-00011320: 6854 7970 6520 7c20 4e6f 6e65 203d 204e  hType | None = N
-00011330: 6f6e 652c 0a20 2020 2020 2020 2067 6473  one,.        gds
-00011340: 6469 723a 2050 6174 6854 7970 6520 7c20  dir: PathType | 
-00011350: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
-00011360: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
-00011370: 2020 2029 202d 3e20 5061 7468 3a0a 2020     ) -> Path:.  
-00011380: 2020 2020 2020 2222 2257 7269 7465 2063        """Write c
-00011390: 6f6d 706f 6e65 6e74 2074 6f20 4744 5320  omponent to GDS 
-000113a0: 616e 6420 7265 7475 726e 7320 6764 7370  and returns gdsp
-000113b0: 6174 682e 0a0a 2020 2020 2020 2020 4172  ath...        Ar
-000113c0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-000113d0: 6764 7370 6174 683a 2047 4453 2066 696c  gdspath: GDS fil
-000113e0: 6520 7061 7468 2074 6f20 7772 6974 6520  e path to write 
-000113f0: 746f 2e0a 2020 2020 2020 2020 2020 2020  to..            
-00011400: 6764 7364 6972 3a20 6469 7265 6374 6f72  gdsdir: director
-00011410: 7920 666f 7220 7468 6520 4744 5320 6669  y for the GDS fi
-00011420: 6c65 2e20 4465 6661 756c 7473 2074 6f20  le. Defaults to 
-00011430: 2f74 6d70 2f72 616e 646f 6d46 696c 652f  /tmp/randomFile/
-00011440: 6764 7366 6163 746f 7279 2e0a 0a20 2020  gdsfactory...   
-00011450: 2020 2020 204b 6579 776f 7264 2041 7267       Keyword Arg
-00011460: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
-00011470: 6e69 743a 2075 6e69 7420 7369 7a65 2066  nit: unit size f
-00011480: 6f72 206f 626a 6563 7473 2069 6e20 6c69  or objects in li
-00011490: 6272 6172 792e 2031 756d 2062 7920 6465  brary. 1um by de
-000114a0: 6661 756c 742e 0a20 2020 2020 2020 2020  fault..         
-000114b0: 2020 2070 7265 6369 7369 6f6e 3a20 666f     precision: fo
-000114c0: 7220 6469 6d65 6e73 696f 6e73 2069 6e20  r dimensions in 
-000114d0: 7468 6520 6c69 6272 6172 7920 286d 292e  the library (m).
-000114e0: 2031 6e6d 2062 7920 6465 6661 756c 742e   1nm by default.
-000114f0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00011500: 6769 6e67 3a20 6469 7361 626c 6520 4744  ging: disable GD
-00011510: 5320 7061 7468 206c 6f67 6769 6e67 2c20  S path logging, 
-00011520: 666f 7220 6578 616d 706c 6520 666f 7220  for example for 
-00011530: 7368 6f77 696e 6720 6974 2069 6e20 4b4c  showing it in KL
-00011540: 6179 6f75 742e 0a20 2020 2020 2020 2020  ayout..         
-00011550: 2020 206f 6e5f 6475 706c 6963 6174 655f     on_duplicate_
-00011560: 6365 6c6c 3a20 7370 6563 6966 7920 686f  cell: specify ho
-00011570: 7720 746f 2072 6573 6f6c 7665 2064 7570  w to resolve dup
-00011580: 6c69 6361 7465 2d6e 616d 6564 2063 656c  licate-named cel
-00011590: 6c73 2e20 4368 6f6f 7365 206f 6e65 206f  ls. Choose one o
-000115a0: 6620 7468 6520 666f 6c6c 6f77 696e 673a  f the following:
-000115b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000115c0: 2022 7761 726e 2220 2864 6566 6175 6c74   "warn" (default
-000115d0: 293a 206f 7665 7277 7269 7465 2061 6c6c  ): overwrite all
-000115e0: 2064 7570 6c69 6361 7465 2063 656c 6c73   duplicate cells
-000115f0: 2077 6974 6820 6f6e 6520 6f66 2074 6865   with one of the
-00011600: 2064 7570 6c69 6361 7465 7320 2861 7262   duplicates (arb
-00011610: 6974 7261 7269 6c79 292e 0a20 2020 2020  itrarily)..     
-00011620: 2020 2020 2020 2020 2020 2022 6572 726f             "erro
-00011630: 7222 3a20 7468 726f 7720 6120 5661 6c75  r": throw a Valu
-00011640: 6545 7272 6f72 2077 6865 6e20 6174 7465  eError when atte
-00011650: 6d70 7469 6e67 2074 6f20 7772 6974 6520  mpting to write 
-00011660: 6120 6764 7320 7769 7468 2064 7570 6c69  a gds with dupli
-00011670: 6361 7465 2063 656c 6c73 2e0a 2020 2020  cate cells..    
-00011680: 2020 2020 2020 2020 2020 2020 226f 7665              "ove
-00011690: 7277 7269 7465 223a 206f 7665 7277 7269  rwrite": overwri
-000116a0: 7465 2061 6c6c 2064 7570 6c69 6361 7465  te all duplicate
-000116b0: 2063 656c 6c73 2077 6974 6820 6f6e 6520   cells with one 
-000116c0: 6f66 2074 6865 2064 7570 6c69 6361 7465  of the duplicate
-000116d0: 732c 2077 6974 686f 7574 2077 6172 6e69  s, without warni
-000116e0: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-000116f0: 2020 2020 4e6f 6e65 3a20 646f 206e 6f74      None: do not
-00011700: 2074 7279 2074 6f20 7265 736f 6c76 6520   try to resolve 
-00011710: 2861 7420 796f 7572 206f 776e 2072 6973  (at your own ris
-00011720: 6b21 290a 2020 2020 2020 2020 2020 2020  k!).            
-00011730: 6f6e 5f75 6e63 6163 6865 645f 636f 6d70  on_uncached_comp
-00011740: 6f6e 656e 743a 204c 6974 6572 616c 5b22  onent: Literal["
-00011750: 7761 726e 222c 2022 6572 726f 7222 5d20  warn", "error"] 
-00011760: 3d20 2277 6172 6e22 0a20 2020 2020 2020  = "warn".       
-00011770: 2020 2020 2066 6c61 7474 656e 5f69 6e76       flatten_inv
-00011780: 616c 6964 5f72 6566 733a 2066 6c61 7474  alid_refs: flatt
-00011790: 656e 7320 636f 6d70 6f6e 656e 7420 7265  ens component re
-000117a0: 6665 7265 6e63 6573 2077 6869 6368 2068  ferences which h
-000117b0: 6176 6520 696e 7661 6c69 6420 7472 616e  ave invalid tran
-000117c0: 7366 6f72 6d61 7469 6f6e 732e 0a20 2020  sformations..   
-000117d0: 2020 2020 2020 2020 2063 6f6d 7072 6573           compres
-000117e0: 7369 6f6e 5f6c 6576 656c 3a20 4c65 7665  sion_level: Leve
-000117f0: 6c20 6f66 2063 6f6d 7072 6573 7369 6f6e  l of compression
-00011800: 2066 6f72 2063 656c 6c73 2028 6265 7477   for cells (betw
-00011810: 6565 6e20 3020 616e 6420 3929 2e0a 2020  een 0 and 9)..  
-00011820: 2020 2020 2020 2020 2020 2020 2020 5365                Se
-00011830: 7474 696e 6720 746f 2030 2077 696c 6c20  tting to 0 will 
-00011840: 6469 7361 626c 6520 6365 6c6c 2063 6f6d  disable cell com
-00011850: 7072 6573 7369 6f6e 2c20 3120 6769 7665  pression, 1 give
-00011860: 7320 7468 6520 6265 7374 2073 7065 6564  s the best speed
-00011870: 2061 6e64 2039 2c20 7468 6520 6265 7374   and 9, the best
-00011880: 2063 6f6d 7072 6573 7369 6f6e 2e0a 2020   compression..  
-00011890: 2020 2020 2020 2020 2020 6465 7465 6374            detect
-000118a0: 5f72 6563 7461 6e67 6c65 733a 2053 746f  _rectangles: Sto
-000118b0: 7265 2072 6563 7461 6e67 6c65 7320 696e  re rectangles in
-000118c0: 2063 6f6d 7072 6573 7365 6420 666f 726d   compressed form
-000118d0: 6174 2e0a 2020 2020 2020 2020 2020 2020  at..            
-000118e0: 6465 7465 6374 5f74 7261 7065 7a6f 6964  detect_trapezoid
-000118f0: 733a 2053 746f 7265 2074 7261 7065 7a6f  s: Store trapezo
-00011900: 6964 7320 696e 2063 6f6d 7072 6573 7365  ids in compresse
-00011910: 6420 666f 726d 6174 2e0a 2020 2020 2020  d format..      
-00011920: 2020 2020 2020 6369 7263 6c65 5f74 6f6c        circle_tol
-00011930: 6572 616e 6365 3a20 546f 6c65 7261 6e63  erance: Toleranc
-00011940: 6520 666f 7220 6465 7465 6374 696e 6720  e for detecting 
-00011950: 6369 7263 6c65 732e 2049 6620 6c65 7373  circles. If less
-00011960: 206f 7220 6571 7561 6c20 746f 2030 2c20   or equal to 0, 
-00011970: 6e6f 2064 6574 6563 7469 6f6e 2069 7320  no detection is 
-00011980: 7065 7266 6f72 6d65 642e 0a20 2020 2020  performed..     
-00011990: 2020 2020 2020 2020 2020 2043 6972 636c             Circl
-000119a0: 6573 2061 7265 2073 746f 7265 6420 696e  es are stored in
-000119b0: 2063 6f6d 7072 6573 7365 6420 666f 726d   compressed form
-000119c0: 6174 2e0a 2020 2020 2020 2020 2020 2020  at..            
-000119d0: 7661 6c69 6461 7469 6f6e 2028 2263 7263  validation ("crc
-000119e0: 3332 222c 2022 6368 6563 6b73 756d 3332  32", "checksum32
-000119f0: 222c 204e 6f6e 6529 20e2 8093 2074 7970  ", None) ... typ
-00011a00: 6520 6f66 2076 616c 6964 6174 696f 6e20  e of validation 
-00011a10: 746f 2069 6e63 6c75 6465 2069 6e20 7468  to include in th
-00011a20: 6520 7361 7665 6420 6669 6c65 2e0a 2020  e saved file..  
-00011a30: 2020 2020 2020 2020 2020 7374 616e 6461            standa
-00011a40: 7264 5f70 726f 7065 7274 6965 733a 2053  rd_properties: S
-00011a50: 746f 7265 2073 7461 6e64 6172 6420 4f41  tore standard OA
-00011a60: 5349 5320 7072 6f70 6572 7469 6573 2069  SIS properties i
-00011a70: 6e20 7468 6520 6669 6c65 2e0a 2020 2020  n the file..    
-00011a80: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011a90: 7265 7475 726e 2073 656c 662e 5f77 7269  return self._wri
-00011aa0: 7465 5f6c 6962 7261 7279 280a 2020 2020  te_library(.    
-00011ab0: 2020 2020 2020 2020 6764 7370 6174 683d          gdspath=
-00011ac0: 6764 7370 6174 682c 0a20 2020 2020 2020  gdspath,.       
-00011ad0: 2020 2020 2067 6473 6469 723d 6764 7364       gdsdir=gdsd
-00011ae0: 6972 2c0a 2020 2020 2020 2020 2020 2020  ir,.            
-00011af0: 7769 7468 5f6f 6173 6973 3d54 7275 652c  with_oasis=True,
-00011b00: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
-00011b10: 7761 7267 732c 0a20 2020 2020 2020 2029  wargs,.        )
-00011b20: 0a0a 2020 2020 6465 6620 7772 6974 655f  ..    def write_
-00011b30: 6764 735f 7769 7468 5f6d 6574 6164 6174  gds_with_metadat
-00011b40: 6128 7365 6c66 2c20 2a61 7267 732c 202a  a(self, *args, *
-00011b50: 2a6b 7761 7267 7329 202d 3e20 5061 7468  *kwargs) -> Path
-00011b60: 3a0a 2020 2020 2020 2020 2222 2257 7269  :.        """Wri
-00011b70: 7465 2063 6f6d 706f 6e65 6e74 2069 6e20  te component in 
-00011b80: 4744 5320 616e 6420 6d65 7461 6461 7461  GDS and metadata
-00011b90: 2028 636f 6d70 6f6e 656e 7420 7365 7474   (component sett
-00011ba0: 696e 6773 2920 696e 2059 414d 4c2e 2222  ings) in YAML.""
-00011bb0: 220a 2020 2020 2020 2020 7761 726e 696e  ".        warnin
-00011bc0: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
-00011bd0: 2020 2020 2022 436f 6d70 6f6e 656e 742e       "Component.
-00011be0: 7772 6974 655f 6764 735f 7769 7468 5f6d  write_gds_with_m
-00011bf0: 6574 6164 6174 6128 2920 6973 2064 6570  etadata() is dep
-00011c00: 7265 6361 7465 642e 2022 0a20 2020 2020  recated. ".     
-00011c10: 2020 2020 2020 2022 5573 6520 436f 6d70         "Use Comp
-00011c20: 6f6e 656e 742e 7772 6974 655f 6764 7328  onent.write_gds(
-00011c30: 7769 7468 5f6d 6574 6164 6174 613d 5472  with_metadata=Tr
-00011c40: 7565 2920 6f72 2043 6f6d 706f 6e65 6e74  ue) or Component
-00011c50: 2e77 7269 7465 5f6f 6173 2877 6974 685f  .write_oas(with_
-00011c60: 6d65 7461 6461 7461 3d54 7275 6529 2e22  metadata=True)."
-00011c70: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
-00011c80: 6163 6b6c 6576 656c 3d33 2c0a 2020 2020  acklevel=3,.    
-00011c90: 2020 2020 290a 2020 2020 2020 2020 6764      ).        gd
-00011ca0: 7370 6174 6820 3d20 7365 6c66 2e77 7269  spath = self.wri
-00011cb0: 7465 5f67 6473 282a 6172 6773 2c20 2a2a  te_gds(*args, **
-00011cc0: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
-00011cd0: 6d65 7461 6461 7461 203d 2067 6473 7061  metadata = gdspa
-00011ce0: 7468 2e77 6974 685f 7375 6666 6978 2822  th.with_suffix("
-00011cf0: 2e79 6d6c 2229 0a20 2020 2020 2020 206d  .yml").        m
-00011d00: 6574 6164 6174 612e 7772 6974 655f 7465  etadata.write_te
-00011d10: 7874 2873 656c 662e 746f 5f79 616d 6c28  xt(self.to_yaml(
-00011d20: 7769 7468 5f63 656c 6c73 3d54 7275 652c  with_cells=True,
-00011d30: 2077 6974 685f 706f 7274 733d 5472 7565   with_ports=True
-00011d40: 2929 0a20 2020 2020 2020 206c 6f67 6765  )).        logge
-00011d50: 722e 696e 666f 2866 2257 7269 7465 2059  r.info(f"Write Y
-00011d60: 414d 4c20 6d65 7461 6461 7461 2074 6f20  AML metadata to 
-00011d70: 7b73 7472 286d 6574 6164 6174 6129 2172  {str(metadata)!r
-00011d80: 7d22 290a 2020 2020 2020 2020 7265 7475  }").        retu
-00011d90: 726e 2067 6473 7061 7468 0a0a 2020 2020  rn gdspath..    
-00011da0: 6465 6620 746f 5f64 6963 7428 0a20 2020  def to_dict(.   
-00011db0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00011dc0: 2020 2069 676e 6f72 655f 636f 6d70 6f6e     ignore_compon
-00011dd0: 656e 7473 5f70 7265 6669 783a 206c 6973  ents_prefix: lis
-00011de0: 745b 7374 725d 207c 204e 6f6e 6520 3d20  t[str] | None = 
-00011df0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6967  None,.        ig
-00011e00: 6e6f 7265 5f66 756e 6374 696f 6e73 5f70  nore_functions_p
-00011e10: 7265 6669 783a 206c 6973 745b 7374 725d  refix: list[str]
-00011e20: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
-00011e30: 2020 2020 2020 2020 7769 7468 5f63 656c          with_cel
-00011e40: 6c73 3a20 626f 6f6c 203d 2046 616c 7365  ls: bool = False
-00011e50: 2c0a 2020 2020 2020 2020 7769 7468 5f70  ,.        with_p
-00011e60: 6f72 7473 3a20 626f 6f6c 203d 2054 7275  orts: bool = Tru
-00011e70: 652c 0a20 2020 2029 202d 3e20 6469 6374  e,.    ) -> dict
-00011e80: 5b73 7472 2c20 416e 795d 3a0a 2020 2020  [str, Any]:.    
-00011e90: 2020 2020 2222 2252 6574 7572 6e73 2044      """Returns D
-00011ea0: 6963 7420 7265 7072 6573 656e 7461 7469  ict representati
-00011eb0: 6f6e 206f 6620 6120 636f 6d70 6f6e 656e  on of a componen
-00011ec0: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
-00011ed0: 3a0a 2020 2020 2020 2020 2020 2020 6967  :.            ig
-00011ee0: 6e6f 7265 5f63 6f6d 706f 6e65 6e74 735f  nore_components_
-00011ef0: 7072 6566 6978 3a20 666f 7220 636f 6d70  prefix: for comp
-00011f00: 6f6e 656e 7473 2074 6f20 6967 6e6f 7265  onents to ignore
-00011f10: 2077 6865 6e20 6578 706f 7274 696e 672e   when exporting.
-00011f20: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
-00011f30: 6f72 655f 6675 6e63 7469 6f6e 735f 7072  ore_functions_pr
-00011f40: 6566 6978 3a20 666f 7220 6675 6e63 7469  efix: for functi
-00011f50: 6f6e 7320 746f 2069 676e 6f72 6520 7768  ons to ignore wh
-00011f60: 656e 2065 7870 6f72 7469 6e67 2e0a 2020  en exporting..  
-00011f70: 2020 2020 2020 2020 2020 7769 7468 5f63            with_c
-00011f80: 656c 6c73 3a20 7772 6974 6520 6365 6c6c  ells: write cell
-00011f90: 7320 7265 6375 7273 6976 656c 792e 0a20  s recursively.. 
-00011fa0: 2020 2020 2020 2020 2020 2077 6974 685f             with_
-00011fb0: 706f 7274 733a 2077 7269 7465 2070 6f72  ports: write por
-00011fc0: 7420 696e 666f 726d 6174 696f 6e20 6469  t information di
-00011fd0: 6374 2e0a 2020 2020 2020 2020 2222 220a  ct..        """.
-00011fe0: 2020 2020 2020 2020 6420 3d20 7b7d 0a20          d = {}. 
-00011ff0: 2020 2020 2020 2069 6620 7769 7468 5f70         if with_p
-00012000: 6f72 7473 3a0a 2020 2020 2020 2020 2020  orts:.          
-00012010: 2020 706f 7274 7320 3d20 7b70 6f72 742e    ports = {port.
-00012020: 6e61 6d65 3a20 706f 7274 2e74 6f5f 6469  name: port.to_di
-00012030: 6374 2829 2066 6f72 2070 6f72 7420 696e  ct() for port in
-00012040: 2073 656c 662e 6765 745f 706f 7274 735f   self.get_ports_
-00012050: 6c69 7374 2829 7d0a 2020 2020 2020 2020  list()}.        
-00012060: 2020 2020 645b 2270 6f72 7473 225d 203d      d["ports"] =
-00012070: 2070 6f72 7473 0a0a 2020 2020 2020 2020   ports..        
-00012080: 6966 2077 6974 685f 6365 6c6c 733a 0a20  if with_cells:. 
-00012090: 2020 2020 2020 2020 2020 2063 656c 6c73             cells
-000120a0: 203d 2072 6563 7572 7365 5f73 7472 7563   = recurse_struc
-000120b0: 7475 7265 7328 0a20 2020 2020 2020 2020  tures(.         
-000120c0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000120d0: 2020 2020 2020 2020 2020 2020 2069 676e               ign
-000120e0: 6f72 655f 6675 6e63 7469 6f6e 735f 7072  ore_functions_pr
-000120f0: 6566 6978 3d69 676e 6f72 655f 6675 6e63  efix=ignore_func
-00012100: 7469 6f6e 735f 7072 6566 6978 2c0a 2020  tions_prefix,.  
-00012110: 2020 2020 2020 2020 2020 2020 2020 6967                ig
-00012120: 6e6f 7265 5f63 6f6d 706f 6e65 6e74 735f  nore_components_
-00012130: 7072 6566 6978 3d69 676e 6f72 655f 636f  prefix=ignore_co
-00012140: 6d70 6f6e 656e 7473 5f70 7265 6669 782c  mponents_prefix,
-00012150: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00012160: 2020 2020 2020 2020 2020 2064 5b22 6365             d["ce
-00012170: 6c6c 7322 5d20 3d20 636c 6561 6e5f 6469  lls"] = clean_di
-00012180: 6374 2863 656c 6c73 290a 0a20 2020 2020  ct(cells)..     
-00012190: 2020 2064 5b22 6e61 6d65 225d 203d 2073     d["name"] = s
-000121a0: 656c 662e 6e61 6d65 0a20 2020 2020 2020  elf.name.       
-000121b0: 2064 5b22 7365 7474 696e 6773 225d 203d   d["settings"] =
-000121c0: 2063 6c65 616e 5f64 6963 7428 6469 6374   clean_dict(dict
-000121d0: 2873 656c 662e 7365 7474 696e 6773 2929  (self.settings))
-000121e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000121f0: 640a 0a20 2020 2064 6566 2074 6f5f 7961  d..    def to_ya
-00012200: 6d6c 2873 656c 662c 202a 2a6b 7761 7267  ml(self, **kwarg
-00012210: 7329 202d 3e20 7374 723a 0a20 2020 2020  s) -> str:.     
-00012220: 2020 2022 2222 5772 6974 6520 4469 6374     """Write Dict
-00012230: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-00012240: 6f66 2061 2063 6f6d 706f 6e65 6e74 2069  of a component i
-00012250: 6e20 5941 4d4c 2066 6f72 6d61 742e 0a0a  n YAML format...
-00012260: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00012270: 2020 2020 2020 2020 2020 6967 6e6f 7265            ignore
-00012280: 5f63 6f6d 706f 6e65 6e74 735f 7072 6566  _components_pref
-00012290: 6978 3a20 666f 7220 636f 6d70 6f6e 656e  ix: for componen
-000122a0: 7473 2074 6f20 6967 6e6f 7265 2077 6865  ts to ignore whe
-000122b0: 6e20 6578 706f 7274 696e 672e 0a20 2020  n exporting..   
-000122c0: 2020 2020 2020 2020 2069 676e 6f72 655f           ignore_
-000122d0: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
-000122e0: 3a20 666f 7220 6675 6e63 7469 6f6e 7320  : for functions 
-000122f0: 746f 2069 676e 6f72 6520 7768 656e 2065  to ignore when e
-00012300: 7870 6f72 7469 6e67 2e0a 2020 2020 2020  xporting..      
-00012310: 2020 2020 2020 7769 7468 5f63 656c 6c73        with_cells
-00012320: 3a20 7772 6974 6520 6365 6c6c 7320 7265  : write cells re
-00012330: 6375 7273 6976 656c 792e 0a20 2020 2020  cursively..     
-00012340: 2020 2020 2020 2077 6974 685f 706f 7274         with_port
-00012350: 733a 2077 7269 7465 2070 6f72 7420 696e  s: write port in
-00012360: 666f 726d 6174 696f 6e2e 0a20 2020 2020  formation..     
-00012370: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00012380: 6574 7572 6e20 7961 6d6c 2e64 756d 7028  eturn yaml.dump(
-00012390: 636c 6561 6e5f 6469 6374 2873 656c 662e  clean_dict(self.
-000123a0: 746f 5f64 6963 7428 2a2a 6b77 6172 6773  to_dict(**kwargs
-000123b0: 2929 290a 0a20 2020 2064 6566 2061 7574  )))..    def aut
-000123c0: 6f5f 7265 6e61 6d65 5f70 6f72 7473 2873  o_rename_ports(s
-000123d0: 656c 662c 202a 2a6b 7761 7267 7329 202d  elf, **kwargs) -
-000123e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000123f0: 2222 2252 656e 616d 6520 706f 7274 7320  """Rename ports 
-00012400: 6279 206f 7269 656e 7461 7469 6f6e 204e  by orientation N
-00012410: 5345 5720 286e 6f72 7468 2c20 736f 7574  SEW (north, sout
-00012420: 682c 2065 6173 742c 2077 6573 7429 2e0a  h, east, west)..
-00012430: 0a20 2020 2020 2020 204b 6579 776f 7264  .        Keyword
-00012440: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00012450: 2020 2066 756e 6374 696f 6e3a 2074 6f20     function: to 
-00012460: 7265 6e61 6d65 2070 6f72 7473 2e0a 2020  rename ports..  
-00012470: 2020 2020 2020 2020 2020 7365 6c65 6374            select
-00012480: 5f70 6f72 7473 5f6f 7074 6963 616c 3a20  _ports_optical: 
-00012490: 746f 2073 656c 6563 7420 6f70 7469 6361  to select optica
-000124a0: 6c20 706f 7274 732e 0a20 2020 2020 2020  l ports..       
-000124b0: 2020 2020 2073 656c 6563 745f 706f 7274       select_port
-000124c0: 735f 656c 6563 7472 6963 616c 3a20 746f  s_electrical: to
-000124d0: 2073 656c 6563 7420 656c 6563 7472 6963   select electric
-000124e0: 616c 2070 6f72 7473 2e0a 2020 2020 2020  al ports..      
-000124f0: 2020 2020 2020 7072 6566 6978 5f6f 7074        prefix_opt
-00012500: 6963 616c 3a20 7072 6566 6978 2e0a 2020  ical: prefix..  
-00012510: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-00012520: 5f65 6c65 6374 7269 6361 6c3a 2070 7265  _electrical: pre
-00012530: 6669 782e 0a0a 2020 2020 2020 2020 2e2e  fix...        ..
-00012540: 2063 6f64 653a 3a0a 0a20 2020 2020 2020   code::..       
-00012550: 2020 2020 2020 2020 2020 2033 2020 340a             3  4.
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 205f 7c5f 5f7c 5f0a 2020 2020 2020 2020   _|__|_.        
-00012580: 2020 2020 2032 202d 7c20 2020 2020 207c       2 -|      |
-00012590: 2d20 350a 2020 2020 2020 2020 2020 2020  - 5.            
-000125a0: 2020 2020 7c20 2020 2020 207c 0a20 2020      |      |.   
-000125b0: 2020 2020 2020 2020 2020 3120 2d7c 5f5f            1 -|__
-000125c0: 5f5f 5f5f 7c2d 2036 0a20 2020 2020 2020  ____|- 6.       
-000125d0: 2020 2020 2020 2020 2020 207c 2020 7c0a             |  |.
-000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125f0: 2020 3820 2037 0a20 2020 2020 2020 2022    8  7.        "
-00012600: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00012610: 6973 5f75 6e6c 6f63 6b65 6428 290a 2020  is_unlocked().  
-00012620: 2020 2020 2020 6175 746f 5f72 656e 616d        auto_renam
-00012630: 655f 706f 7274 7328 7365 6c66 2c20 2a2a  e_ports(self, **
-00012640: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
-00012650: 2061 7574 6f5f 7265 6e61 6d65 5f70 6f72   auto_rename_por
-00012660: 7473 5f63 6f75 6e74 6572 5f63 6c6f 636b  ts_counter_clock
-00012670: 7769 7365 2873 656c 662c 202a 2a6b 7761  wise(self, **kwa
-00012680: 7267 7329 202d 3e20 4e6f 6e65 3a0a 2020  rgs) -> None:.  
-00012690: 2020 2020 2020 7365 6c66 2e69 735f 756e        self.is_un
-000126a0: 6c6f 636b 6564 2829 0a20 2020 2020 2020  locked().       
-000126b0: 2061 7574 6f5f 7265 6e61 6d65 5f70 6f72   auto_rename_por
-000126c0: 7473 5f63 6f75 6e74 6572 5f63 6c6f 636b  ts_counter_clock
-000126d0: 7769 7365 2873 656c 662c 202a 2a6b 7761  wise(self, **kwa
-000126e0: 7267 7329 0a0a 2020 2020 6465 6620 6175  rgs)..    def au
-000126f0: 746f 5f72 656e 616d 655f 706f 7274 735f  to_rename_ports_
-00012700: 6c61 7965 725f 6f72 6965 6e74 6174 696f  layer_orientatio
-00012710: 6e28 7365 6c66 2c20 2a2a 6b77 6172 6773  n(self, **kwargs
-00012720: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00012730: 2020 2073 656c 662e 6973 5f75 6e6c 6f63     self.is_unloc
-00012740: 6b65 6428 290a 2020 2020 2020 2020 6175  ked().        au
-00012750: 746f 5f72 656e 616d 655f 706f 7274 735f  to_rename_ports_
-00012760: 6c61 7965 725f 6f72 6965 6e74 6174 696f  layer_orientatio
-00012770: 6e28 7365 6c66 2c20 2a2a 6b77 6172 6773  n(self, **kwargs
-00012780: 290a 0a20 2020 2064 6566 2061 7574 6f5f  )..    def auto_
-00012790: 7265 6e61 6d65 5f70 6f72 7473 5f6f 7269  rename_ports_ori
-000127a0: 656e 7461 7469 6f6e 2873 656c 662c 202a  entation(self, *
-000127b0: 2a6b 7761 7267 7329 202d 3e20 4e6f 6e65  *kwargs) -> None
-000127c0: 3a0a 2020 2020 2020 2020 2222 2252 656e  :.        """Ren
-000127d0: 616d 6520 706f 7274 7320 6279 206f 7269  ame ports by ori
-000127e0: 656e 7461 7469 6f6e 204e 5345 5720 286e  entation NSEW (n
-000127f0: 6f72 7468 2c20 736f 7574 682c 2065 6173  orth, south, eas
-00012800: 742c 2077 6573 7429 2e0a 0a20 2020 2020  t, west)...     
-00012810: 2020 204b 6579 776f 7264 2041 7267 733a     Keyword Args:
-00012820: 0a20 2020 2020 2020 2020 2020 2066 756e  .            fun
-00012830: 6374 696f 6e3a 2074 6f20 7265 6e61 6d65  ction: to rename
-00012840: 2070 6f72 7473 2e0a 2020 2020 2020 2020   ports..        
-00012850: 2020 2020 7365 6c65 6374 5f70 6f72 7473      select_ports
-00012860: 5f6f 7074 6963 616c 3a20 746f 2073 656c  _optical: to sel
-00012870: 6563 7420 706f 7274 732e 0a20 2020 2020  ect ports..     
-00012880: 2020 2020 2020 2073 656c 6563 745f 706f         select_po
-00012890: 7274 735f 656c 6563 7472 6963 616c 3a0a  rts_electrical:.
-000128a0: 2020 2020 2020 2020 2020 2020 7072 6566              pref
-000128b0: 6978 5f6f 7074 6963 616c 3a0a 2020 2020  ix_optical:.    
-000128c0: 2020 2020 2020 2020 7072 6566 6978 5f65          prefix_e
-000128d0: 6c65 6374 7269 6361 6c3a 0a0a 2020 2020  lectrical:..    
-000128e0: 2020 2020 2e2e 2063 6f64 653a 3a0a 0a20      .. code::.. 
-000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012900: 4e30 2020 4e31 0a20 2020 2020 2020 2020  N0  N1.         
-00012910: 2020 2020 2020 2020 7c5f 5f5f 7c5f 0a20          |___|_. 
-00012920: 2020 2020 2020 2020 2020 2057 3120 2d7c             W1 -|
-00012930: 2020 2020 2020 7c2d 2045 310a 2020 2020        |- E1.    
-00012940: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00012950: 2020 207c 0a20 2020 2020 2020 2020 2020     |.           
-00012960: 2057 3020 2d7c 5f5f 5f5f 5f5f 7c2d 2045   W0 -|______|- E
-00012970: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-00012980: 2020 207c 2020 207c 0a20 2020 2020 2020     |   |.       
-00012990: 2020 2020 2020 2020 2053 3020 2020 5331           S0   S1
-000129a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000129b0: 2020 2020 2073 656c 662e 6973 5f75 6e6c       self.is_unl
-000129c0: 6f63 6b65 6428 290a 2020 2020 2020 2020  ocked().        
-000129d0: 6175 746f 5f72 656e 616d 655f 706f 7274  auto_rename_port
-000129e0: 735f 6f72 6965 6e74 6174 696f 6e28 7365  s_orientation(se
-000129f0: 6c66 2c20 2a2a 6b77 6172 6773 290a 0a20  lf, **kwargs).. 
-00012a00: 2020 2064 6566 206d 6f76 6528 0a20 2020     def move(.   
-00012a10: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00012a20: 2020 206f 7269 6769 6e3a 2046 6c6f 6174     origin: Float
-00012a30: 3220 3d20 2830 2c20 3029 2c0a 2020 2020  2 = (0, 0),.    
-00012a40: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
-00012a50: 2046 6c6f 6174 3220 7c20 4e6f 6e65 203d   Float2 | None =
-00012a60: 204e 6f6e 652c 0a20 2020 2020 2020 2061   None,.        a
-00012a70: 7869 733a 2041 7869 7320 7c20 4e6f 6e65  xis: Axis | None
-00012a80: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
-00012a90: 3e20 436f 6d70 6f6e 656e 743a 0a20 2020  > Component:.   
-00012aa0: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
-00012ab0: 6e65 7720 436f 6d70 6f6e 656e 7420 7769  new Component wi
-00012ac0: 7468 2061 206d 6f76 6564 2072 6566 6572  th a moved refer
-00012ad0: 656e 6365 2074 6f20 7468 6520 6f72 6967  ence to the orig
-00012ae0: 696e 616c 2e0a 0a20 2020 2020 2020 2063  inal...        c
-00012af0: 6f6d 706f 6e65 6e74 2e0a 0a20 2020 2020  omponent...     
-00012b00: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00012b10: 2020 2020 206f 7269 6769 6e3a 206f 6620       origin: of 
-00012b20: 636f 6d70 6f6e 656e 742e 0a20 2020 2020  component..     
-00012b30: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-00012b40: 6f6e 3a20 782c 2079 2e0a 2020 2020 2020  on: x, y..      
-00012b50: 2020 2020 2020 6178 6973 3a20 7820 6f72        axis: x or
-00012b60: 2079 2e0a 2020 2020 2020 2020 2222 220a   y..        """.
-00012b70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00012b80: 6c75 6545 7272 6f72 286d 6f76 655f 6572  lueError(move_er
-00012b90: 726f 725f 6d65 7373 6167 6529 0a0a 2020  ror_message)..  
-00012ba0: 2020 6465 6620 6d69 7272 6f72 2873 656c    def mirror(sel
-00012bb0: 662c 2070 313a 2046 6c6f 6174 3220 3d20  f, p1: Float2 = 
-00012bc0: 2830 2c20 3129 2c20 7032 3a20 466c 6f61  (0, 1), p2: Floa
-00012bd0: 7432 203d 2028 302c 2030 292c 202a 2a6b  t2 = (0, 0), **k
-00012be0: 7761 7267 7329 202d 3e20 436f 6d70 6f6e  wargs) -> Compon
-00012bf0: 656e 743a 0a20 2020 2020 2020 2022 2222  ent:.        """
-00012c00: 5265 7475 726e 7320 6e65 7720 436f 6d70  Returns new Comp
-00012c10: 6f6e 656e 7420 7769 7468 2061 206d 6972  onent with a mir
-00012c20: 726f 7265 6420 7265 6665 7265 6e63 652e  rored reference.
-00012c30: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00012c40: 2020 2020 2020 2020 2020 2020 7031 3a20              p1: 
-00012c50: 6669 7273 7420 706f 696e 7420 746f 2064  first point to d
-00012c60: 6566 696e 6520 6d69 7272 6f72 2061 7869  efine mirror axi
-00012c70: 732e 0a20 2020 2020 2020 2020 2020 2070  s..            p
-00012c80: 323a 2073 6563 6f6e 6420 706f 696e 7420  2: second point 
-00012c90: 746f 2064 6566 696e 6520 6d69 7272 6f72  to define mirror
-00012ca0: 2061 7869 732e 0a20 2020 2020 2020 2022   axis..        "
-00012cb0: 2222 0a20 2020 2020 2020 2066 726f 6d20  "".        from 
-00012cc0: 6764 7366 6163 746f 7279 2e66 756e 6374  gdsfactory.funct
-00012cd0: 696f 6e73 2069 6d70 6f72 7420 6d69 7272  ions import mirr
-00012ce0: 6f72 0a0a 2020 2020 2020 2020 7265 7475  or..        retu
-00012cf0: 726e 206d 6972 726f 7228 636f 6d70 6f6e  rn mirror(compon
-00012d00: 656e 743d 7365 6c66 2c20 7031 3d70 312c  ent=self, p1=p1,
-00012d10: 2070 323d 7032 2c20 2a2a 6b77 6172 6773   p2=p2, **kwargs
-00012d20: 290a 0a20 2020 2064 6566 2072 6f74 6174  )..    def rotat
-00012d30: 6528 7365 6c66 2c20 616e 676c 653a 2066  e(self, angle: f
-00012d40: 6c6f 6174 203d 2039 302c 202a 2a6b 7761  loat = 90, **kwa
-00012d50: 7267 7329 202d 3e20 436f 6d70 6f6e 656e  rgs) -> Componen
-00012d60: 743a 0a20 2020 2020 2020 2022 2222 5265  t:.        """Re
-00012d70: 7475 726e 7320 6e65 7720 636f 6d70 6f6e  turns new compon
-00012d80: 656e 7420 7769 7468 2061 2072 6f74 6174  ent with a rotat
-00012d90: 6564 2072 6566 6572 656e 6365 2074 6f20  ed reference to 
-00012da0: 7468 6520 6f72 6967 696e 616c 2e0a 0a20  the original... 
-00012db0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00012dc0: 2020 2020 2020 2020 2061 6e67 6c65 3a20           angle: 
-00012dd0: 696e 2064 6567 7265 6573 2e0a 2020 2020  in degrees..    
-00012de0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012df0: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
-00012e00: 6675 6e63 7469 6f6e 7320 696d 706f 7274  functions import
-00012e10: 2072 6f74 6174 650a 0a20 2020 2020 2020   rotate..       
-00012e20: 2072 6574 7572 6e20 726f 7461 7465 2863   return rotate(c
-00012e30: 6f6d 706f 6e65 6e74 3d73 656c 662c 2061  omponent=self, a
-00012e40: 6e67 6c65 3d61 6e67 6c65 2c20 2a2a 6b77  ngle=angle, **kw
-00012e50: 6172 6773 290a 0a20 2020 2064 6566 2061  args)..    def a
-00012e60: 6464 5f70 6164 6469 6e67 2873 656c 662c  dd_padding(self,
-00012e70: 202a 2a6b 7761 7267 7329 202d 3e20 436f   **kwargs) -> Co
-00012e80: 6d70 6f6e 656e 743a 0a20 2020 2020 2020  mponent:.       
-00012e90: 2022 2222 5265 7475 726e 7320 7361 6d65   """Returns same
-00012ea0: 2063 6f6d 706f 6e65 6e74 2077 6974 6820   component with 
-00012eb0: 7061 6464 696e 672e 0a0a 2020 2020 2020  padding...      
-00012ec0: 2020 4b65 7977 6f72 6420 4172 6773 3a0a    Keyword Args:.
-00012ed0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
-00012ee0: 6f6e 656e 743a 2066 6f72 2070 6164 6469  onent: for paddi
-00012ef0: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-00012f00: 6c61 7965 7273 3a20 6c69 7374 206f 6620  layers: list of 
-00012f10: 6c61 7965 7273 2e0a 2020 2020 2020 2020  layers..        
-00012f20: 2020 2020 7375 6666 6978 2066 6f72 206e      suffix for n
-00012f30: 616d 652e 0a20 2020 2020 2020 2020 2020  ame..           
-00012f40: 2064 6566 6175 6c74 3a20 6465 6661 756c   default: defaul
-00012f50: 7420 7061 6464 696e 6720 2835 3075 6d29  t padding (50um)
-00012f60: 2e0a 2020 2020 2020 2020 2020 2020 746f  ..            to
-00012f70: 703a 206e 6f72 7468 2070 6164 6469 6e67  p: north padding
-00012f80: 2e0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
-00012f90: 7474 6f6d 3a20 736f 7574 6820 7061 6464  ttom: south padd
-00012fa0: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
-00012fb0: 2072 6967 6874 3a20 6561 7374 2070 6164   right: east pad
-00012fc0: 6469 6e67 2e0a 2020 2020 2020 2020 2020  ding..          
-00012fd0: 2020 6c65 6674 3a20 7765 7374 2070 6164    left: west pad
-00012fe0: 6469 6e67 2e0a 2020 2020 2020 2020 2222  ding..        ""
-00012ff0: 220a 2020 2020 2020 2020 6672 6f6d 2067  ".        from g
-00013000: 6473 6661 6374 6f72 792e 6164 645f 7061  dsfactory.add_pa
-00013010: 6464 696e 6720 696d 706f 7274 2061 6464  dding import add
-00013020: 5f70 6164 6469 6e67 0a0a 2020 2020 2020  _padding..      
-00013030: 2020 7265 7475 726e 2061 6464 5f70 6164    return add_pad
-00013040: 6469 6e67 2863 6f6d 706f 6e65 6e74 3d73  ding(component=s
-00013050: 656c 662c 202a 2a6b 7761 7267 7329 0a0a  elf, **kwargs)..
-00013060: 2020 2020 6465 6620 6162 736f 7262 2873      def absorb(s
-00013070: 656c 662c 2072 6566 6572 656e 6365 2920  elf, reference) 
-00013080: 2d3e 2043 6f6d 706f 6e65 6e74 3a0a 2020  -> Component:.  
-00013090: 2020 2020 2020 2222 2241 6273 6f72 6273        """Absorbs
-000130a0: 2070 6f6c 7967 6f6e 7320 6672 6f6d 2043   polygons from C
-000130b0: 6f6d 706f 6e65 6e74 5265 6665 7265 6e63  omponentReferenc
-000130c0: 6520 696e 746f 2043 6f6d 706f 6e65 6e74  e into Component
-000130d0: 2e0a 0a20 2020 2020 2020 2044 6573 7472  ...        Destr
-000130e0: 6f79 7320 7468 6520 7265 6665 7265 6e63  oys the referenc
-000130f0: 6520 696e 2074 6865 2070 726f 6365 7373  e in the process
-00013100: 2062 7574 206b 6565 7069 6e67 2074 6865   but keeping the
-00013110: 2070 6f6c 7967 6f6e 2067 656f 6d65 7472   polygon geometr
-00013120: 792e 0a0a 2020 2020 2020 2020 4172 6773  y...        Args
-00013130: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00013140: 6665 7265 6e63 653a 2043 6f6d 706f 6e65  ference: Compone
-00013150: 6e74 5265 6665 7265 6e63 6520 746f 2062  ntReference to b
-00013160: 6520 6162 736f 7262 6564 2069 6e74 6f20  e absorbed into 
-00013170: 7468 6520 436f 6d70 6f6e 656e 742e 0a20  the Component.. 
-00013180: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013190: 2020 2069 6620 7265 6665 7265 6e63 6520     if reference 
-000131a0: 6e6f 7420 696e 2073 656c 662e 7265 6665  not in self.refe
-000131b0: 7265 6e63 6573 3a0a 2020 2020 2020 2020  rences:.        
-000131c0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-000131d0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-000131e0: 2020 2020 2020 2254 6865 2072 6566 6572        "The refer
-000131f0: 656e 6365 2079 6f75 2061 736b 6564 2074  ence you asked t
-00013200: 6f20 6162 736f 7262 2064 6f65 7320 6e6f  o absorb does no
-00013210: 7420 6578 6973 7420 696e 2074 6869 7320  t exist in this 
-00013220: 436f 6d70 6f6e 656e 742e 220a 2020 2020  Component.".    
-00013230: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00013240: 2020 7265 665f 706f 6c79 676f 6e73 203d    ref_polygons =
-00013250: 2072 6566 6572 656e 6365 2e67 6574 5f70   reference.get_p
-00013260: 6f6c 7967 6f6e 7328 0a20 2020 2020 2020  olygons(.       
-00013270: 2020 2020 2062 795f 7370 6563 3d46 616c       by_spec=Fal
-00013280: 7365 2c20 696e 636c 7564 655f 7061 7468  se, include_path
-00013290: 733d 4661 6c73 652c 2061 735f 6172 7261  s=False, as_arra
-000132a0: 793d 4661 6c73 650a 2020 2020 2020 2020  y=False.        
-000132b0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-000132c0: 6164 645f 706f 6c79 676f 6e73 282a 7265  add_polygons(*re
-000132d0: 665f 706f 6c79 676f 6e73 290a 0a20 2020  f_polygons)..   
-000132e0: 2020 2020 2073 656c 662e 6164 6428 7265       self.add(re
-000132f0: 6665 7265 6e63 652e 6765 745f 6c61 6265  ference.get_labe
-00013300: 6c73 2829 290a 2020 2020 2020 2020 7365  ls()).        se
-00013310: 6c66 2e61 6464 2872 6566 6572 656e 6365  lf.add(reference
-00013320: 2e67 6574 5f70 6174 6873 2829 290a 2020  .get_paths()).  
-00013330: 2020 2020 2020 7365 6c66 2e72 656d 6f76        self.remov
-00013340: 6528 7265 6665 7265 6e63 6529 0a20 2020  e(reference).   
-00013350: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00013360: 0a0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
-00013370: 2873 656c 662c 2069 7465 6d73 293a 0a20  (self, items):. 
-00013380: 2020 2020 2020 2022 2222 5265 6d6f 7665         """Remove
-00013390: 7320 6974 656d 7320 6672 6f6d 2061 2043  s items from a C
-000133a0: 6f6d 706f 6e65 6e74 2c20 7768 6963 6820  omponent, which 
-000133b0: 6361 6e20 696e 636c 7564 6520 506f 7274  can include Port
-000133c0: 732c 2050 6f6c 7967 6f6e 5365 7473 205c  s, PolygonSets \
-000133d0: 0a20 2020 2020 2020 2043 656c 6c52 6566  .        CellRef
-000133e0: 6572 656e 6365 732c 2043 6f6d 706f 6e65  erences, Compone
-000133f0: 6e74 5265 6665 7265 6e63 6573 2061 6e64  ntReferences and
-00013400: 204c 6162 656c 732e 0a0a 2020 2020 2020   Labels...      
-00013410: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00013420: 2020 2020 6974 656d 733a 206c 6973 7420      items: list 
-00013430: 6f66 2049 7465 6d73 2074 6f20 6265 2072  of Items to be r
-00013440: 656d 6f76 6564 2066 726f 6d20 7468 6520  emoved from the 
-00013450: 436f 6d70 6f6e 656e 742e 0a20 2020 2020  Component..     
-00013460: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00013470: 6620 6e6f 7420 6861 7361 7474 7228 6974  f not hasattr(it
-00013480: 656d 732c 2022 5f5f 6974 6572 5f5f 2229  ems, "__iter__")
-00013490: 3a0a 2020 2020 2020 2020 2020 2020 6974  :.            it
-000134a0: 656d 7320 3d20 5b69 7465 6d73 5d0a 2020  ems = [items].  
-000134b0: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
-000134c0: 6e20 6974 656d 733a 0a20 2020 2020 2020  n items:.       
-000134d0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-000134e0: 6365 2869 7465 6d2c 2050 6f72 7429 3a0a  ce(item, Port):.
-000134f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013500: 7365 6c66 2e70 6f72 7473 203d 207b 6b3a  self.ports = {k:
-00013510: 2076 2066 6f72 206b 2c20 7620 696e 2073   v for k, v in s
-00013520: 656c 662e 706f 7274 732e 6974 656d 7328  elf.ports.items(
-00013530: 2920 6966 2076 2021 3d20 6974 656d 7d0a  ) if v != item}.
-00013540: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00013550: 2069 7369 6e73 7461 6e63 6528 6974 656d   isinstance(item
-00013560: 2c20 6764 7374 6b2e 5265 6665 7265 6e63  , gdstk.Referenc
-00013570: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00013580: 2020 2020 7365 6c66 2e5f 6365 6c6c 2e72      self._cell.r
-00013590: 656d 6f76 6528 6974 656d 290a 2020 2020  emove(item).    
-000135a0: 2020 2020 2020 2020 2020 2020 6974 656d              item
-000135b0: 2e6f 776e 6572 203d 204e 6f6e 650a 2020  .owner = None.  
-000135c0: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
-000135d0: 7369 6e73 7461 6e63 6528 6974 656d 2c20  sinstance(item, 
-000135e0: 436f 6d70 6f6e 656e 7452 6566 6572 656e  ComponentReferen
-000135f0: 6365 293a 0a20 2020 2020 2020 2020 2020  ce):.           
-00013600: 2020 2020 2073 656c 662e 7265 6665 7265       self.refere
-00013610: 6e63 6573 2e72 656d 6f76 6528 6974 656d  nces.remove(item
-00013620: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013630: 2020 7365 6c66 2e5f 6365 6c6c 2e72 656d    self._cell.rem
-00013640: 6f76 6528 6974 656d 2e5f 7265 6665 7265  ove(item._refere
-00013650: 6e63 6529 0a20 2020 2020 2020 2020 2020  nce).           
-00013660: 2020 2020 2069 7465 6d2e 6f77 6e65 7220       item.owner 
-00013670: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-00013680: 2020 2020 2020 2073 656c 662e 5f6e 616d         self._nam
-00013690: 6564 5f72 6566 6572 656e 6365 732e 706f  ed_references.po
-000136a0: 7028 6974 656d 2e6e 616d 6529 0a20 2020  p(item.name).   
-000136b0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000136c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000136d0: 656c 662e 5f63 656c 6c2e 7265 6d6f 7665  elf._cell.remove
-000136e0: 2869 7465 6d29 0a0a 2020 2020 2020 2020  (item)..        
-000136f0: 7365 6c66 2e5f 6262 5f76 616c 6964 203d  self._bb_valid =
-00013700: 2046 616c 7365 0a20 2020 2020 2020 2072   False.        r
-00013710: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
-00013720: 6465 6620 6861 7368 5f67 656f 6d65 7472  def hash_geometr
-00013730: 7928 7365 6c66 2c20 7072 6563 6973 696f  y(self, precisio
-00013740: 6e3a 2066 6c6f 6174 203d 2031 652d 3429  n: float = 1e-4)
-00013750: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-00013760: 2022 2222 5265 7475 726e 7320 616e 2053   """Returns an S
-00013770: 4841 3120 6861 7368 206f 6620 7468 6520  HA1 hash of the 
-00013780: 6765 6f6d 6574 7279 2069 6e20 7468 6520  geometry in the 
-00013790: 436f 6d70 6f6e 656e 742e 0a0a 2020 2020  Component...    
-000137a0: 2020 2020 466f 7220 6561 6368 206c 6179      For each lay
-000137b0: 6572 2c20 6561 6368 2070 6f6c 7967 6f6e  er, each polygon
-000137c0: 2069 7320 696e 6469 7669 6475 616c 6c79   is individually
-000137d0: 2068 6173 6865 6420 616e 6420 7468 656e   hashed and then
-000137e0: 2074 6865 2070 6f6c 7967 6f6e 2068 6173   the polygon has
-000137f0: 6865 730a 2020 2020 2020 2020 6172 6520  hes.        are 
-00013800: 736f 7274 6564 2c20 746f 2065 6e73 7572  sorted, to ensur
-00013810: 6520 7468 6520 6861 7368 2073 7461 7973  e the hash stays
-00013820: 2063 6f6e 7374 616e 7420 7265 6761 7264   constant regard
-00013830: 6c65 7373 206f 6620 7468 6520 6f72 6465  less of the orde
-00013840: 7269 6e67 0a20 2020 2020 2020 2074 6865  ring.        the
-00013850: 2070 6f6c 7967 6f6e 732e 2020 5369 6d69   polygons.  Simi
-00013860: 6c61 726c 792c 2074 6865 206c 6179 6572  larly, the layer
-00013870: 7320 6172 6520 736f 7274 6564 2062 7920  s are sorted by 
-00013880: 286c 6179 6572 2c20 6461 7461 7479 7065  (layer, datatype
-00013890: 292e 0a0a 2020 2020 2020 2020 4172 6773  )...        Args
-000138a0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-000138b0: 6563 6973 696f 6e3a 2052 6f75 6e64 696e  ecision: Roundin
-000138c0: 6720 7072 6563 6973 696f 6e20 666f 7220  g precision for 
-000138d0: 7468 6520 7468 6520 6f62 6a65 6374 7320  the the objects 
-000138e0: 696e 2074 6865 2043 6f6d 706f 6e65 6e74  in the Component
-000138f0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013900: 2020 466f 7220 696e 7374 616e 6365 2c20    For instance, 
-00013910: 6120 7072 6563 6973 696f 6e20 6f66 2031  a precision of 1
-00013920: 652d 3220 7769 6c6c 2072 6f75 6e64 2061  e-2 will round a
-00013930: 2070 6f69 6e74 2061 740a 2020 2020 2020   point at.      
-00013940: 2020 2020 2020 2020 2020 2830 2e31 3234            (0.124
-00013950: 2c20 312e 3734 3829 2074 6f20 2830 2e31  , 1.748) to (0.1
-00013960: 322c 2031 2e37 3529 2e0a 0a20 2020 2020  2, 1.75)...     
-00013970: 2020 2022 2222 0a20 2020 2020 2020 2070     """.        p
-00013980: 6f6c 7967 6f6e 735f 6279 5f73 7065 6320  olygons_by_spec 
-00013990: 3d20 7365 6c66 2e67 6574 5f70 6f6c 7967  = self.get_polyg
-000139a0: 6f6e 7328 6279 5f73 7065 633d 5472 7565  ons(by_spec=True
-000139b0: 2c20 6173 5f61 7272 6179 3d46 616c 7365  , as_array=False
-000139c0: 290a 2020 2020 2020 2020 6c61 7965 7273  ).        layers
-000139d0: 203d 206e 702e 6172 7261 7928 6c69 7374   = np.array(list
-000139e0: 2870 6f6c 7967 6f6e 735f 6279 5f73 7065  (polygons_by_spe
-000139f0: 632e 6b65 7973 2829 2929 0a20 2020 2020  c.keys())).     
-00013a00: 2020 2073 6f72 7465 645f 6c61 7965 7273     sorted_layers
-00013a10: 203d 206c 6179 6572 735b 6e70 2e6c 6578   = layers[np.lex
-00013a20: 736f 7274 2828 6c61 7965 7273 5b3a 2c20  sort((layers[:, 
-00013a30: 305d 2c20 6c61 7965 7273 5b3a 2c20 315d  0], layers[:, 1]
-00013a40: 2929 5d0a 0a20 2020 2020 2020 2066 696e  ))]..        fin
-00013a50: 616c 5f68 6173 6820 3d20 6861 7368 6c69  al_hash = hashli
-00013a60: 622e 7368 6131 2829 0a20 2020 2020 2020  b.sha1().       
-00013a70: 2066 6f72 206c 6179 6572 2069 6e20 736f   for layer in so
-00013a80: 7274 6564 5f6c 6179 6572 733a 0a20 2020  rted_layers:.   
-00013a90: 2020 2020 2020 2020 206c 6179 6572 5f68           layer_h
-00013aa0: 6173 6820 3d20 6861 7368 6c69 622e 7368  ash = hashlib.sh
-00013ab0: 6131 286c 6179 6572 2e61 7374 7970 6528  a1(layer.astype(
-00013ac0: 6e70 2e69 6e74 3634 2929 2e64 6967 6573  np.int64)).diges
-00013ad0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00013ae0: 706f 6c79 676f 6e73 203d 2070 6f6c 7967  polygons = polyg
-00013af0: 6f6e 735f 6279 5f73 7065 635b 7475 706c  ons_by_spec[tupl
-00013b00: 6528 6c61 7965 7229 5d0a 2020 2020 2020  e(layer)].      
-00013b10: 2020 2020 2020 706f 6c79 676f 6e73 203d        polygons =
-00013b20: 205b 5f72 6e64 2870 2e70 6f69 6e74 732c   [_rnd(p.points,
-00013b30: 2070 7265 6369 7369 6f6e 2920 666f 7220   precision) for 
-00013b40: 7020 696e 2070 6f6c 7967 6f6e 735d 0a20  p in polygons]. 
-00013b50: 2020 2020 2020 2020 2020 2070 6f6c 7967             polyg
-00013b60: 6f6e 5f68 6173 6865 7320 3d20 6e70 2e73  on_hashes = np.s
-00013b70: 6f72 7428 5b68 6173 686c 6962 2e73 6861  ort([hashlib.sha
-00013b80: 3128 7029 2e64 6967 6573 7428 2920 666f  1(p).digest() fo
-00013b90: 7220 7020 696e 2070 6f6c 7967 6f6e 735d  r p in polygons]
-00013ba0: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
-00013bb0: 6e61 6c5f 6861 7368 2e75 7064 6174 6528  nal_hash.update(
-00013bc0: 6c61 7965 725f 6861 7368 290a 2020 2020  layer_hash).    
-00013bd0: 2020 2020 2020 2020 666f 7220 7068 2069          for ph i
-00013be0: 6e20 706f 6c79 676f 6e5f 6861 7368 6573  n polygon_hashes
-00013bf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013c00: 2020 6669 6e61 6c5f 6861 7368 2e75 7064    final_hash.upd
-00013c10: 6174 6528 7068 290a 0a20 2020 2020 2020  ate(ph)..       
-00013c20: 2072 6574 7572 6e20 6669 6e61 6c5f 6861   return final_ha
-00013c30: 7368 2e68 6578 6469 6765 7374 2829 0a0a  sh.hexdigest()..
-00013c40: 2020 2020 6465 6620 6765 745f 6c61 6265      def get_labe
-00013c50: 6c73 280a 2020 2020 2020 2020 7365 6c66  ls(.        self
-00013c60: 2c20 6170 706c 795f 7265 7065 7469 7469  , apply_repetiti
-00013c70: 6f6e 733d 5472 7565 2c20 6465 7074 683a  ons=True, depth:
-00013c80: 2069 6e74 207c 204e 6f6e 6520 3d20 4e6f   int | None = No
-00013c90: 6e65 2c20 6c61 7965 723d 4e6f 6e65 0a20  ne, layer=None. 
-00013ca0: 2020 2029 202d 3e20 6c69 7374 5b4c 6162     ) -> list[Lab
-00013cb0: 656c 5d3a 0a20 2020 2020 2020 2022 2222  el]:.        """
-00013cc0: 5265 7475 726e 206c 6162 656c 732e 0a0a  Return labels...
-00013cd0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00013ce0: 2020 2020 2020 2020 2020 6170 706c 795f            apply_
-00013cf0: 7265 7065 7469 7469 6f6e 733a 2e0a 2020  repetitions:..  
-00013d00: 2020 2020 2020 2020 2020 6465 7074 683a            depth:
-00013d10: 204e 6f6e 6520 7265 7475 726e 7320 616c   None returns al
-00013d20: 6c20 6c61 6265 6c73 2061 6e64 2030 2074  l labels and 0 t
-00013d30: 6f70 206c 6576 656c 2e0a 2020 2020 2020  op level..      
-00013d40: 2020 2020 2020 6c61 7965 723a 206c 6179        layer: lay
-00013d50: 6572 7370 6563 2e0a 2020 2020 2020 2020  erspec..        
-00013d60: 2222 220a 2020 2020 2020 2020 6672 6f6d  """.        from
-00013d70: 2067 6473 6661 6374 6f72 792e 7064 6b20   gdsfactory.pdk 
-00013d80: 696d 706f 7274 2067 6574 5f6c 6179 6572  import get_layer
-00013d90: 0a0a 2020 2020 2020 2020 6966 206c 6179  ..        if lay
-00013da0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00013db0: 6c61 7965 722c 2074 6578 7474 7970 6520  layer, texttype 
-00013dc0: 3d20 6765 745f 6c61 7965 7228 6c61 7965  = get_layer(laye
-00013dd0: 7229 0a20 2020 2020 2020 2065 6c73 653a  r).        else:
-00013de0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-00013df0: 7474 7970 6520 3d20 4e6f 6e65 0a20 2020  ttype = None.   
-00013e00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00013e10: 2e5f 6365 6c6c 2e67 6574 5f6c 6162 656c  ._cell.get_label
-00013e20: 7328 0a20 2020 2020 2020 2020 2020 2061  s(.            a
-00013e30: 7070 6c79 5f72 6570 6574 6974 696f 6e73  pply_repetitions
-00013e40: 3d61 7070 6c79 5f72 6570 6574 6974 696f  =apply_repetitio
-00013e50: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
-00013e60: 6465 7074 683d 6465 7074 682c 0a20 2020  depth=depth,.   
-00013e70: 2020 2020 2020 2020 206c 6179 6572 3d6c           layer=l
-00013e80: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
-00013e90: 2020 7465 7874 7479 7065 3d74 6578 7474    texttype=textt
-00013ea0: 7970 652c 0a20 2020 2020 2020 2029 0a0a  ype,.        )..
-00013eb0: 2020 2020 6465 6620 7265 6d6f 7665 5f6c      def remove_l
-00013ec0: 6162 656c 7328 7365 6c66 2920 2d3e 204e  abels(self) -> N
-00013ed0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00013ee0: 5265 6d6f 7665 206c 6162 656c 732e 2222  Remove labels.""
-00013ef0: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
-00013f00: 6365 6c6c 2e72 656d 6f76 6528 2a73 656c  cell.remove(*sel
-00013f10: 662e 6c61 6265 6c73 290a 0a20 2020 2023  f.labels)..    #
-00013f20: 2044 6570 7265 6361 7465 640a 2020 2020   Deprecated.    
-00013f30: 6465 6620 6765 745f 696e 666f 2873 656c  def get_info(sel
-00013f40: 6629 3a0a 2020 2020 2020 2020 2222 2247  f):.        """G
-00013f50: 6174 6865 7273 2074 6865 202e 696e 666f  athers the .info
-00013f60: 2064 6963 7469 6f6e 6172 6965 7320 6672   dictionaries fr
-00013f70: 6f6d 2065 7665 7279 2073 7562 2d43 6f6d  om every sub-Com
-00013f80: 706f 6e65 6e74 2061 6e64 2072 6574 7572  ponent and retur
-00013f90: 6e73 2074 6865 6d20 696e 2061 206c 6973  ns them in a lis
-00013fa0: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
-00013fb0: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-00013fc0: 7074 683a 2069 6e74 206f 7220 4e6f 6e65  pth: int or None
-00013fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013fe0: 2049 6620 6e6f 7420 4e6f 6e65 2c20 6465   If not None, de
-00013ff0: 6669 6e65 7320 6672 6f6d 2068 6f77 206d  fines from how m
-00014000: 616e 7920 7265 6665 7265 6e63 6520 6c65  any reference le
-00014010: 7665 6c73 2074 6f0a 2020 2020 2020 2020  vels to.        
-00014020: 2020 2020 2020 2020 7265 7472 6965 7665          retrieve
-00014030: 2050 6f72 7473 2066 726f 6d2e 0a0a 2020   Ports from...  
-00014040: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00014050: 2020 2020 2020 2020 2020 206c 6973 7420             list 
-00014060: 6f66 2064 6963 7469 6f6e 6172 6965 730a  of dictionaries.
-00014070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014080: 4c69 7374 206f 6620 7468 6520 222e 696e  List of the ".in
-00014090: 666f 2220 7072 6f70 6572 7479 2064 6963  fo" property dic
-000140a0: 7469 6f6e 6172 6965 7320 6672 6f6d 2061  tionaries from a
-000140b0: 6c6c 2073 7562 2d43 6f6d 706f 6e65 6e74  ll sub-Component
-000140c0: 730a 2020 2020 2020 2020 2222 220a 2020  s.        """.  
-000140d0: 2020 2020 2020 445f 6c69 7374 203d 2073        D_list = s
-000140e0: 656c 662e 6765 745f 6465 7065 6e64 656e  elf.get_dependen
-000140f0: 6369 6573 2872 6563 7572 7369 7665 3d54  cies(recursive=T
-00014100: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
-00014110: 7572 6e20 5b44 2e69 6e66 6f2e 636f 7079  urn [D.info.copy
-00014120: 2829 2066 6f72 2044 2069 6e20 445f 6c69  () for D in D_li
-00014130: 7374 5d0a 0a20 2020 2064 6566 2072 656d  st]..    def rem
-00014140: 6170 5f6c 6179 6572 7328 0a20 2020 2020  ap_layers(.     
-00014150: 2020 2073 656c 662c 206c 6179 6572 6d61     self, layerma
-00014160: 702c 2069 6e63 6c75 6465 5f6c 6162 656c  p, include_label
-00014170: 733a 2062 6f6f 6c20 3d20 5472 7565 2c20  s: bool = True, 
-00014180: 696e 636c 7564 655f 7061 7468 733a 2062  include_paths: b
-00014190: 6f6f 6c20 3d20 5472 7565 0a20 2020 2029  ool = True.    )
-000141a0: 202d 3e20 436f 6d70 6f6e 656e 743a 0a20   -> Component:. 
-000141b0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-000141c0: 7320 6120 636f 7079 206f 6620 7468 6520  s a copy of the 
-000141d0: 636f 6d70 6f6e 656e 7420 7769 7468 2072  component with r
-000141e0: 656d 6170 7065 6420 6c61 7965 7273 2e0a  emapped layers..
-000141f0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00014200: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-00014210: 6d61 703a 2044 6963 7469 6f6e 6172 7920  map: Dictionary 
-00014220: 6f66 2076 616c 7565 7320 696e 2066 6f72  of values in for
-00014230: 6d61 7420 7b6c 6179 6572 5f66 726f 6d20  mat {layer_from 
-00014240: 3a20 6c61 7965 725f 746f 7d2e 0a20 2020  : layer_to}..   
-00014250: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-00014260: 5f6c 6162 656c 733a 2053 656c 6563 7473  _labels: Selects
-00014270: 2077 6865 7468 6572 2074 6f20 6d6f 7665   whether to move
-00014280: 204c 6162 656c 7320 616c 6f6e 6720 7769   Labels along wi
-00014290: 7468 2070 6f6c 7967 6f6e 732e 0a20 2020  th polygons..   
-000142a0: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-000142b0: 5f70 6174 6873 3a20 5365 6c65 6374 7320  _paths: Selects 
-000142c0: 7768 6574 6865 7220 746f 206d 6f76 6520  whether to move 
-000142d0: 5061 7468 7320 616c 6f6e 6720 7769 7468  Paths along with
-000142e0: 2070 6f6c 7967 6f6e 732e 0a20 2020 2020   polygons..     
-000142f0: 2020 2022 2222 0a20 2020 2020 2020 2063     """.        c
-00014300: 6f6d 706f 6e65 6e74 203d 2073 656c 662e  omponent = self.
-00014310: 636f 7079 2829 0a20 2020 2020 2020 206c  copy().        l
-00014320: 6179 6572 6d61 7020 3d20 7b5f 7061 7273  ayermap = {_pars
-00014330: 655f 6c61 7965 7228 6b29 3a20 5f70 6172  e_layer(k): _par
-00014340: 7365 5f6c 6179 6572 2876 2920 666f 7220  se_layer(v) for 
-00014350: 6b2c 2076 2069 6e20 6c61 7965 726d 6170  k, v in layermap
-00014360: 2e69 7465 6d73 2829 7d0a 0a20 2020 2020  .items()}..     
-00014370: 2020 2061 6c6c 5f44 203d 206c 6973 7428     all_D = list(
-00014380: 636f 6d70 6f6e 656e 742e 6765 745f 6465  component.get_de
-00014390: 7065 6e64 656e 6369 6573 2854 7275 6529  pendencies(True)
-000143a0: 290a 2020 2020 2020 2020 616c 6c5f 442e  ).        all_D.
-000143b0: 6170 7065 6e64 2863 6f6d 706f 6e65 6e74  append(component
-000143c0: 290a 2020 2020 2020 2020 666f 7220 4420  ).        for D 
-000143d0: 696e 2061 6c6c 5f44 3a0a 2020 2020 2020  in all_D:.      
-000143e0: 2020 2020 2020 666f 7220 7020 696e 2044        for p in D
-000143f0: 2e70 6f6c 7967 6f6e 733a 0a20 2020 2020  .polygons:.     
-00014400: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-00014410: 203d 2028 702e 6c61 7965 722c 2070 2e64   = (p.layer, p.d
-00014420: 6174 6174 7970 6529 0a20 2020 2020 2020  atatype).       
-00014430: 2020 2020 2020 2020 2069 6620 6c61 7965           if laye
-00014440: 7220 696e 206c 6179 6572 6d61 703a 0a20  r in layermap:. 
-00014450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014460: 2020 206e 6577 5f6c 6179 6572 203d 206c     new_layer = l
-00014470: 6179 6572 6d61 705b 6c61 7965 725d 0a20  ayermap[layer]. 
-00014480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014490: 2020 2070 2e6c 6179 6572 203d 206e 6577     p.layer = new
-000144a0: 5f6c 6179 6572 5b30 5d0a 2020 2020 2020  _layer[0].      
-000144b0: 2020 2020 2020 2020 2020 2020 2020 702e                p.
-000144c0: 6461 7461 7479 7065 203d 206e 6577 5f6c  datatype = new_l
-000144d0: 6179 6572 5b31 5d0a 2020 2020 2020 2020  ayer[1].        
-000144e0: 2020 2020 6966 2069 6e63 6c75 6465 5f6c      if include_l
-000144f0: 6162 656c 733a 0a20 2020 2020 2020 2020  abels:.         
-00014500: 2020 2020 2020 2066 6f72 206c 6162 656c         for label
-00014510: 2069 6e20 442e 6c61 6265 6c73 3a0a 2020   in D.labels:.  
-00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014530: 2020 6f72 6967 696e 616c 5f6c 6179 6572    original_layer
-00014540: 203d 2028 6c61 6265 6c2e 6c61 7965 722c   = (label.layer,
-00014550: 206c 6162 656c 2e74 6578 7474 7970 6529   label.texttype)
-00014560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014570: 2020 2020 206f 7269 6769 6e61 6c5f 6c61       original_la
-00014580: 7965 7220 3d20 5f70 6172 7365 5f6c 6179  yer = _parse_lay
-00014590: 6572 286f 7269 6769 6e61 6c5f 6c61 7965  er(original_laye
-000145a0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-000145b0: 2020 2020 2020 2069 6620 6f72 6967 696e         if origin
-000145c0: 616c 5f6c 6179 6572 2069 6e20 6c61 7965  al_layer in laye
-000145d0: 726d 6170 3a0a 2020 2020 2020 2020 2020  rmap:.          
-000145e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-000145f0: 775f 6c61 7965 7220 3d20 6c61 7965 726d  w_layer = layerm
-00014600: 6170 5b6f 7269 6769 6e61 6c5f 6c61 7965  ap[original_laye
-00014610: 725d 0a20 2020 2020 2020 2020 2020 2020  r].             
-00014620: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00014630: 2e6c 6179 6572 203d 206e 6577 5f6c 6179  .layer = new_lay
-00014640: 6572 5b30 5d0a 2020 2020 2020 2020 2020  er[0].          
-00014650: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00014660: 6265 6c2e 7465 7874 7479 7065 203d 206e  bel.texttype = n
-00014670: 6577 5f6c 6179 6572 5b31 5d0a 0a20 2020  ew_layer[1]..   
-00014680: 2020 2020 2020 2020 2069 6620 696e 636c           if incl
-00014690: 7564 655f 7061 7468 733a 0a20 2020 2020  ude_paths:.     
-000146a0: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
-000146b0: 6174 6820 696e 2044 2e70 6174 6873 3a0a  ath in D.paths:.
-000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 2020 2020 6e65 775f 6c61 7965 7273 203d      new_layers =
-000146e0: 206c 6973 7428 7061 7468 2e6c 6179 6572   list(path.layer
-000146f0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-00014700: 2020 2020 2020 206e 6577 5f64 6174 6174         new_datat
-00014710: 7970 6573 203d 206c 6973 7428 7061 7468  ypes = list(path
-00014720: 2e64 6174 6174 7970 6573 290a 2020 2020  .datatypes).    
-00014730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014740: 666f 7220 6c61 7965 725f 6e75 6d62 6572  for layer_number
-00014750: 2069 6e20 7261 6e67 6528 6c65 6e28 6e65   in range(len(ne
-00014760: 775f 6c61 7965 7273 2929 3a0a 2020 2020  w_layers)):.    
-00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014780: 2020 2020 6f72 6967 696e 616c 5f6c 6179      original_lay
-00014790: 6572 203d 205f 7061 7273 655f 6c61 7965  er = _parse_laye
-000147a0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-000147b0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000147c0: 6e65 775f 6c61 7965 7273 5b6c 6179 6572  new_layers[layer
-000147d0: 5f6e 756d 6265 725d 2c20 6e65 775f 6461  _number], new_da
-000147e0: 7461 7479 7065 735b 6c61 7965 725f 6e75  tatypes[layer_nu
-000147f0: 6d62 6572 5d29 0a20 2020 2020 2020 2020  mber]).         
-00014800: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00014810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014820: 2020 2020 2020 2020 2069 6620 6f72 6967           if orig
-00014830: 696e 616c 5f6c 6179 6572 2069 6e20 6c61  inal_layer in la
-00014840: 7965 726d 6170 3a0a 2020 2020 2020 2020  yermap:.        
-00014850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014860: 2020 2020 6e65 775f 6c61 7965 7220 3d20      new_layer = 
-00014870: 6c61 7965 726d 6170 5b6f 7269 6769 6e61  layermap[origina
-00014880: 6c5f 6c61 7965 725d 0a20 2020 2020 2020  l_layer].       
-00014890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148a0: 2020 2020 206e 6577 5f6c 6179 6572 735b       new_layers[
-000148b0: 6c61 7965 725f 6e75 6d62 6572 5d20 3d20  layer_number] = 
-000148c0: 6e65 775f 6c61 7965 725b 305d 0a20 2020  new_layer[0].   
-000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148e0: 2020 2020 2020 2020 206e 6577 5f64 6174           new_dat
-000148f0: 6174 7970 6573 5b6c 6179 6572 5f6e 756d  atypes[layer_num
-00014900: 6265 725d 203d 206e 6577 5f6c 6179 6572  ber] = new_layer
-00014910: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
-00014920: 2020 2020 2020 2020 7061 7468 2e73 6574          path.set
-00014930: 5f6c 6179 6572 7328 2a6e 6577 5f6c 6179  _layers(*new_lay
-00014940: 6572 7329 0a20 2020 2020 2020 2020 2020  ers).           
-00014950: 2020 2020 2020 2020 2070 6174 682e 7365           path.se
-00014960: 745f 6461 7461 7479 7065 7328 2a6e 6577  t_datatypes(*new
-00014970: 5f64 6174 6174 7970 6573 290a 2020 2020  _datatypes).    
-00014980: 2020 2020 7265 7475 726e 2063 6f6d 706f      return compo
-00014990: 6e65 6e74 0a0a 2020 2020 6465 6620 746f  nent..    def to
-000149a0: 5f33 6428 0a20 2020 2020 2020 2073 656c  _3d(.        sel
-000149b0: 662c 0a20 2020 2020 2020 206c 6179 6572  f,.        layer
-000149c0: 5f76 6965 7773 3a20 4c61 7965 7256 6965  _views: LayerVie
-000149d0: 7773 207c 204e 6f6e 6520 3d20 4e6f 6e65  ws | None = None
-000149e0: 2c0a 2020 2020 2020 2020 6c61 7965 725f  ,.        layer_
-000149f0: 7374 6163 6b3a 204c 6179 6572 5374 6163  stack: LayerStac
-00014a00: 6b20 7c20 4e6f 6e65 203d 204e 6f6e 652c  k | None = None,
-00014a10: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
-00014a20: 5f6c 6179 6572 733a 2074 7570 6c65 5b4c  _layers: tuple[L
-00014a30: 6179 6572 2c20 2e2e 2e5d 207c 204e 6f6e  ayer, ...] | Non
-00014a40: 6520 3d20 4e6f 6e65 2c0a 2020 2020 293a  e = None,.    ):
-00014a50: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00014a60: 726e 2043 6f6d 706f 6e65 6e74 2033 4420  rn Component 3D 
-00014a70: 7472 696d 6573 6820 5363 656e 652e 0a0a  trimesh Scene...
-00014a80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00014a90: 2020 2020 2020 2020 2020 636f 6d70 6f6e            compon
-00014aa0: 656e 743a 2074 6f20 6578 7472 7564 6520  ent: to extrude 
-00014ab0: 696e 2033 442e 0a20 2020 2020 2020 2020  in 3D..         
-00014ac0: 2020 206c 6179 6572 5f76 6965 7773 3a20     layer_views: 
-00014ad0: 6c61 7965 7220 636f 6c6f 7273 2066 726f  layer colors fro
-00014ae0: 6d20 4b6c 6179 6f75 7420 4c61 7965 7220  m Klayout Layer 
-00014af0: 5072 6f70 6572 7469 6573 2066 696c 652e  Properties file.
-00014b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014b10: 2044 6566 6175 6c74 7320 746f 2061 6374   Defaults to act
-00014b20: 6976 6520 5044 4b2e 6c61 7965 725f 7669  ive PDK.layer_vi
-00014b30: 6577 732e 0a20 2020 2020 2020 2020 2020  ews..           
-00014b40: 206c 6179 6572 5f73 7461 636b 3a20 636f   layer_stack: co
-00014b50: 6e74 6169 6e73 2074 6869 636b 6e65 7373  ntains thickness
-00014b60: 2061 6e64 207a 6d69 6e20 666f 7220 6561   and zmin for ea
-00014b70: 6368 206c 6179 6572 2e0a 2020 2020 2020  ch layer..      
-00014b80: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00014b90: 7473 2074 6f20 6163 7469 7665 2050 444b  ts to active PDK
-00014ba0: 2e6c 6179 6572 5f73 7461 636b 2e0a 2020  .layer_stack..  
-00014bb0: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
-00014bc0: 655f 6c61 7965 7273 3a20 6c61 7965 7273  e_layers: layers
-00014bd0: 2074 6f20 6578 636c 7564 652e 0a0a 2020   to exclude...  
-00014be0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00014bf0: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
-00014c00: 792e 6578 706f 7274 2e74 6f5f 3364 2069  y.export.to_3d i
-00014c10: 6d70 6f72 7420 746f 5f33 640a 0a20 2020  mport to_3d..   
-00014c20: 2020 2020 2072 6574 7572 6e20 746f 5f33       return to_3
-00014c30: 6428 0a20 2020 2020 2020 2020 2020 2073  d(.            s
-00014c40: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-00014c50: 206c 6179 6572 5f76 6965 7773 3d6c 6179   layer_views=lay
-00014c60: 6572 5f76 6965 7773 2c0a 2020 2020 2020  er_views,.      
-00014c70: 2020 2020 2020 6c61 7965 725f 7374 6163        layer_stac
-00014c80: 6b3d 6c61 7965 725f 7374 6163 6b2c 0a20  k=layer_stack,. 
-00014c90: 2020 2020 2020 2020 2020 2065 7863 6c75             exclu
-00014ca0: 6465 5f6c 6179 6572 733d 6578 636c 7564  de_layers=exclud
-00014cb0: 655f 6c61 7965 7273 2c0a 2020 2020 2020  e_layers,.      
-00014cc0: 2020 290a 0a20 2020 2064 6566 2074 6f5f    )..    def to_
-00014cd0: 6e70 280a 2020 2020 2020 2020 7365 6c66  np(.        self
-00014ce0: 2c0a 2020 2020 2020 2020 6e6d 5f70 6572  ,.        nm_per
-00014cf0: 5f70 6978 656c 3a20 696e 7420 3d20 3230  _pixel: int = 20
-00014d00: 2c0a 2020 2020 2020 2020 6c61 7965 7273  ,.        layers
-00014d10: 3a20 4c61 7965 7273 203d 2028 2831 2c20  : Layers = ((1, 
-00014d20: 3029 2c29 2c0a 2020 2020 2020 2020 7661  0),),.        va
-00014d30: 6c75 6573 3a20 7475 706c 655b 666c 6f61  lues: tuple[floa
-00014d40: 742c 202e 2e2e 5d20 7c20 4e6f 6e65 203d  t, ...] | None =
-00014d50: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
-00014d60: 6164 5f77 6964 7468 3a20 696e 7420 3d20  ad_width: int = 
-00014d70: 312c 0a20 2020 2029 202d 3e20 6e70 2e6e  1,.    ) -> np.n
-00014d80: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
-00014d90: 2222 2252 6574 7572 6e73 2061 2070 6978  """Returns a pix
-00014da0: 656c 6174 6564 206e 756d 7079 2061 7272  elated numpy arr
-00014db0: 6179 2066 726f 6d20 436f 6d70 6f6e 656e  ay from Componen
-00014dc0: 7420 706f 6c79 676f 6e73 2e0a 0a20 2020  t polygons...   
-00014dd0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00014de0: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
-00014df0: 3a20 436f 6d70 6f6e 656e 742e 0a20 2020  : Component..   
-00014e00: 2020 2020 2020 2020 206e 6d5f 7065 725f           nm_per_
-00014e10: 7069 7865 6c3a 2079 6f75 2063 616e 2067  pixel: you can g
-00014e20: 6f20 6672 6f6d 2032 3020 2863 6f61 7273  o from 20 (coars
-00014e30: 6529 2074 6f20 3420 2866 696e 6529 2e0a  e) to 4 (fine)..
-00014e40: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-00014e50: 7273 3a20 746f 2063 6f6e 7665 7274 2e20  rs: to convert. 
-00014e60: 4f72 6465 7220 6d61 7474 6572 7320 286c  Order matters (l
-00014e70: 6174 7465 7220 6f76 6572 7772 6974 6520  atter overwrite 
-00014e80: 666f 726d 6572 292e 0a20 2020 2020 2020  former)..       
-00014e90: 2020 2020 2076 616c 7565 733a 2061 7373       values: ass
-00014ea0: 6f63 6961 7465 6420 746f 2065 6163 6820  ociated to each 
-00014eb0: 6c61 7965 7220 2864 6566 6175 6c74 7320  layer (defaults 
-00014ec0: 746f 2031 292e 0a20 2020 2020 2020 2020  to 1)..         
-00014ed0: 2020 2070 6164 5f77 6964 7468 3a20 7061     pad_width: pa
-00014ee0: 6464 696e 6720 7069 7865 6c73 2061 726f  dding pixels aro
-00014ef0: 756e 6420 7468 6520 696d 6167 652e 0a0a  und the image...
-00014f00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00014f10: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
-00014f20: 6f72 792e 6578 706f 7274 2e74 6f5f 6e70  ory.export.to_np
-00014f30: 2069 6d70 6f72 7420 746f 5f6e 700a 0a20   import to_np.. 
-00014f40: 2020 2020 2020 2072 6574 7572 6e20 746f         return to
-00014f50: 5f6e 7028 0a20 2020 2020 2020 2020 2020  _np(.           
-00014f60: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-00014f70: 2020 206e 6d5f 7065 725f 7069 7865 6c3d     nm_per_pixel=
-00014f80: 6e6d 5f70 6572 5f70 6978 656c 2c0a 2020  nm_per_pixel,.  
-00014f90: 2020 2020 2020 2020 2020 6c61 7965 7273            layers
-00014fa0: 3d6c 6179 6572 732c 0a20 2020 2020 2020  =layers,.       
-00014fb0: 2020 2020 2076 616c 7565 733d 7661 6c75       values=valu
-00014fc0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00014fd0: 7061 645f 7769 6474 683d 7061 645f 7769  pad_width=pad_wi
-00014fe0: 6474 682c 0a20 2020 2020 2020 2029 0a0a  dth,.        )..
-00014ff0: 2020 2020 6465 6620 7772 6974 655f 7374      def write_st
-00015000: 6c28 0a20 2020 2020 2020 2073 656c 662c  l(.        self,
-00015010: 0a20 2020 2020 2020 2066 696c 6570 6174  .        filepat
-00015020: 683a 2073 7472 2c0a 2020 2020 2020 2020  h: str,.        
-00015030: 6c61 7965 725f 7374 6163 6b3a 204c 6179  layer_stack: Lay
-00015040: 6572 5374 6163 6b20 7c20 4e6f 6e65 203d  erStack | None =
-00015050: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
-00015060: 7863 6c75 6465 5f6c 6179 6572 733a 2074  xclude_layers: t
-00015070: 7570 6c65 5b4c 6179 6572 2c20 2e2e 2e5d  uple[Layer, ...]
-00015080: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
-00015090: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
-000150a0: 2020 2020 2020 2022 2222 5772 6974 6520         """Write 
-000150b0: 6120 436f 6d70 6f6e 656e 7420 746f 2053  a Component to S
-000150c0: 544c 2066 6f72 2033 4420 7072 696e 7469  TL for 3D printi
-000150d0: 6e67 2e0a 0a20 2020 2020 2020 2041 7267  ng...        Arg
-000150e0: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-000150f0: 696c 6570 6174 683a 2074 6f20 7772 6974  ilepath: to writ
-00015100: 6520 5354 4c20 746f 2e0a 2020 2020 2020  e STL to..      
-00015110: 2020 2020 2020 6c61 7965 725f 7374 6163        layer_stac
-00015120: 6b3a 2063 6f6e 7461 696e 7320 7468 6963  k: contains thic
-00015130: 6b6e 6573 7320 616e 6420 7a6d 696e 2066  kness and zmin f
-00015140: 6f72 2065 6163 6820 6c61 7965 722e 0a20  or each layer.. 
-00015150: 2020 2020 2020 2020 2020 2065 7863 6c75             exclu
-00015160: 6465 5f6c 6179 6572 733a 206c 6179 6572  de_layers: layer
-00015170: 7320 746f 2065 7863 6c75 6465 2e0a 2020  s to exclude..  
-00015180: 2020 2020 2020 2020 2020 7573 655f 6c61            use_la
-00015190: 7965 725f 6e61 6d65 3a20 4966 2054 7275  yer_name: If Tru
-000151a0: 652c 2075 7365 7320 4c61 7965 724c 6576  e, uses LayerLev
-000151b0: 656c 206e 616d 6573 2069 6e20 6f75 7470  el names in outp
-000151c0: 7574 2066 696c 656e 616d 6573 2072 6174  ut filenames rat
-000151d0: 6865 7220 7468 616e 2067 6473 5f6c 6179  her than gds_lay
-000151e0: 6572 2061 6e64 2067 6473 5f64 6174 6174  er and gds_datat
-000151f0: 7970 652e 0a20 2020 2020 2020 2020 2020  ype..           
-00015200: 2068 756c 6c5f 696e 7661 6c69 645f 706f   hull_invalid_po
-00015210: 6c79 676f 6e73 3a20 4966 2054 7275 652c  lygons: If True,
-00015220: 2072 6570 6c61 6365 7320 696e 7661 6c69   replaces invali
-00015230: 6420 706f 6c79 676f 6e73 2028 6465 7465  d polygons (dete
-00015240: 726d 696e 6564 2062 7920 7368 6170 656c  rmined by shapel
-00015250: 792e 506f 6c79 676f 6e2e 6973 5f76 616c  y.Polygon.is_val
-00015260: 6964 2920 7769 7468 2069 7473 2063 6f6e  id) with its con
-00015270: 7665 7820 6875 6c6c 2e0a 2020 2020 2020  vex hull..      
-00015280: 2020 2020 2020 7363 616c 653a 204f 7074        scale: Opt
-00015290: 696f 6e61 6c20 6661 6374 6f72 2062 7920  ional factor by 
-000152a0: 7768 6963 6820 746f 2073 6361 6c65 206d  which to scale m
-000152b0: 6573 6865 7320 6265 666f 7265 2077 7269  eshes before wri
-000152c0: 7469 6e67 2e0a 0a20 2020 2020 2020 2022  ting...        "
-000152d0: 2222 0a20 2020 2020 2020 2066 726f 6d20  "".        from 
-000152e0: 6764 7366 6163 746f 7279 2e65 7870 6f72  gdsfactory.expor
-000152f0: 742e 746f 5f73 746c 2069 6d70 6f72 7420  t.to_stl import 
-00015300: 746f 5f73 746c 0a0a 2020 2020 2020 2020  to_stl..        
-00015310: 746f 5f73 746c 280a 2020 2020 2020 2020  to_stl(.        
-00015320: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00015330: 2020 2020 2020 6669 6c65 7061 7468 3d66        filepath=f
-00015340: 696c 6570 6174 682c 0a20 2020 2020 2020  ilepath,.       
-00015350: 2020 2020 206c 6179 6572 5f73 7461 636b       layer_stack
-00015360: 3d6c 6179 6572 5f73 7461 636b 2c0a 2020  =layer_stack,.  
-00015370: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
-00015380: 655f 6c61 7965 7273 3d65 7863 6c75 6465  e_layers=exclude
-00015390: 5f6c 6179 6572 732c 0a20 2020 2020 2020  _layers,.       
-000153a0: 2029 0a0a 2020 2020 6465 6620 7772 6974   )..    def writ
-000153b0: 655f 6765 7262 6572 2873 656c 662c 2064  e_gerber(self, d
-000153c0: 6972 7061 7468 2c20 6c61 7965 726d 6170  irpath, layermap
-000153d0: 5f74 6f5f 6765 7262 6572 5f6c 6179 6572  _to_gerber_layer
-000153e0: 2c20 6f70 7469 6f6e 7329 202d 3e20 4e6f  , options) -> No
-000153f0: 6e65 3a0a 2020 2020 2020 2020 6672 6f6d  ne:.        from
-00015400: 2067 6473 6661 6374 6f72 792e 6578 706f   gdsfactory.expo
-00015410: 7274 2e74 6f5f 6765 7262 6572 2069 6d70  rt.to_gerber imp
-00015420: 6f72 7420 746f 5f67 6572 6265 720a 0a20  ort to_gerber.. 
-00015430: 2020 2020 2020 2074 6f5f 6765 7262 6572         to_gerber
-00015440: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00015450: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00015460: 6469 7270 6174 683d 6469 7270 6174 682c  dirpath=dirpath,
-00015470: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-00015480: 6572 6d61 705f 746f 5f67 6572 6265 725f  ermap_to_gerber_
-00015490: 6c61 7965 723d 6c61 7965 726d 6170 5f74  layer=layermap_t
-000154a0: 6f5f 6765 7262 6572 5f6c 6179 6572 2c0a  o_gerber_layer,.
-000154b0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-000154c0: 6f6e 733d 6f70 7469 6f6e 732c 0a20 2020  ons=options,.   
-000154d0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-000154e0: 746f 5f67 6d73 6828 0a20 2020 2020 2020  to_gmsh(.       
-000154f0: 2073 656c 662c 0a20 2020 2020 2020 2074   self,.        t
-00015500: 7970 652c 0a20 2020 2020 2020 207a 3d4e  ype,.        z=N
-00015510: 6f6e 652c 0a20 2020 2020 2020 2078 7365  one,.        xse
-00015520: 6374 696f 6e5f 626f 756e 6473 3d4e 6f6e  ction_bounds=Non
-00015530: 652c 0a20 2020 2020 2020 206c 6179 6572  e,.        layer
-00015540: 5f73 7461 636b 3d4e 6f6e 652c 0a20 2020  _stack=None,.   
-00015550: 2020 2020 2077 6166 6572 5f70 6164 6469       wafer_paddi
-00015560: 6e67 3d30 2e30 2c0a 2020 2020 2020 2020  ng=0.0,.        
-00015570: 7761 6665 725f 6c61 7965 723d 4c41 5945  wafer_layer=LAYE
-00015580: 522e 5741 4645 522c 0a20 2020 2020 2020  R.WAFER,.       
-00015590: 202a 6172 6773 2c0a 2020 2020 2020 2020   *args,.        
-000155a0: 2a2a 6b77 6172 6773 2c0a 2020 2020 293a  **kwargs,.    ):
-000155b0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-000155c0: 726e 7320 6120 676d 7368 206d 7368 206f  rns a gmsh msh o
-000155d0: 6620 7468 6520 636f 6d70 6f6e 656e 7420  f the component 
-000155e0: 666f 7220 6669 6e69 7465 2065 6c65 6d65  for finite eleme
-000155f0: 6e74 2073 696d 756c 6174 696f 6e2e 0a0a  nt simulation...
-00015600: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
-00015610: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-00015620: 7970 653a 206f 6e65 206f 6620 2278 7922  ype: one of "xy"
-00015630: 2c20 2275 7a22 2c20 6f72 2022 3344 222e  , "uz", or "3D".
-00015640: 2044 6574 6572 6d69 6e65 7320 7468 6520   Determines the 
-00015650: 7479 7065 206f 6620 6d65 7368 2074 6f20  type of mesh to 
-00015660: 7265 7475 726e 2e0a 2020 2020 2020 2020  return..        
-00015670: 2020 2020 7a3a 2075 7365 6420 746f 2064      z: used to d
-00015680: 6566 696e 6520 7a2d 736c 6963 6520 666f  efine z-slice fo
-00015690: 7220 7879 206d 6573 6869 6e67 0a20 2020  r xy meshing.   
-000156a0: 2020 2020 2020 2020 2078 7365 6374 696f           xsectio
-000156b0: 6e5f 626f 756e 6473 3a20 7573 6564 2074  n_bounds: used t
-000156c0: 6f20 6465 6669 6e65 2069 6e2d 706c 616e  o define in-plan
-000156d0: 6520 6c69 6e65 2066 6f72 2075 7a20 6d65  e line for uz me
-000156e0: 7368 696e 670a 2020 2020 2020 2020 2020  shing.          
-000156f0: 2020 7761 6665 725f 7061 6464 696e 673a    wafer_padding:
-00015700: 2070 6164 6469 6e67 2062 6579 6f6e 6420   padding beyond 
-00015710: 6262 6f78 2074 6f20 6164 6420 746f 2057  bbox to add to W
-00015720: 4146 4552 206c 6179 6572 732e 0a0a 2020  AFER layers...  
-00015730: 2020 2020 2020 4b65 7977 6f72 6420 4172        Keyword Ar
-00015740: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00015750: 4172 6775 6d65 6e74 7320 666f 7220 7468  Arguments for th
-00015760: 6520 7461 7267 6574 206d 6573 6869 6e67  e target meshing
-00015770: 2066 756e 6374 696f 6e20 696e 2067 706c   function in gpl
-00015780: 7567 696e 732e 676d 7368 0a20 2020 2020  ugins.gmsh.     
-00015790: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-000157a0: 2041 6464 2057 4146 4552 206c 6179 6572   Add WAFER layer
-000157b0: 3a0a 2020 2020 2020 2020 7061 6464 6564  :.        padded
-000157c0: 5f63 6f6d 706f 6e65 6e74 203d 2043 6f6d  _component = Com
-000157d0: 706f 6e65 6e74 2829 0a20 2020 2020 2020  ponent().       
-000157e0: 2070 6164 6465 645f 636f 6d70 6f6e 656e   padded_componen
-000157f0: 7420 3c3c 2073 656c 660a 2020 2020 2020  t << self.      
-00015800: 2020 2878 6d69 6e2c 2079 6d69 6e29 2c20    (xmin, ymin), 
-00015810: 2878 6d61 782c 2079 6d61 7829 203d 2073  (xmax, ymax) = s
-00015820: 656c 662e 6262 6f78 0a20 2020 2020 2020  elf.bbox.       
-00015830: 2070 6f69 6e74 7320 3d20 5b0a 2020 2020   points = [.    
-00015840: 2020 2020 2020 2020 5b78 6d69 6e20 2d20          [xmin - 
-00015850: 7761 6665 725f 7061 6464 696e 672c 2079  wafer_padding, y
-00015860: 6d69 6e20 2d20 7761 6665 725f 7061 6464  min - wafer_padd
-00015870: 696e 675d 2c0a 2020 2020 2020 2020 2020  ing],.          
-00015880: 2020 5b78 6d61 7820 2b20 7761 6665 725f    [xmax + wafer_
-00015890: 7061 6464 696e 672c 2079 6d69 6e20 2d20  padding, ymin - 
-000158a0: 7761 6665 725f 7061 6464 696e 675d 2c0a  wafer_padding],.
-000158b0: 2020 2020 2020 2020 2020 2020 5b78 6d61              [xma
-000158c0: 7820 2b20 7761 6665 725f 7061 6464 696e  x + wafer_paddin
-000158d0: 672c 2079 6d61 7820 2b20 7761 6665 725f  g, ymax + wafer_
-000158e0: 7061 6464 696e 675d 2c0a 2020 2020 2020  padding],.      
-000158f0: 2020 2020 2020 5b78 6d69 6e20 2d20 7761        [xmin - wa
-00015900: 6665 725f 7061 6464 696e 672c 2079 6d61  fer_padding, yma
-00015910: 7820 2b20 7761 6665 725f 7061 6464 696e  x + wafer_paddin
-00015920: 675d 2c0a 2020 2020 2020 2020 5d0a 2020  g],.        ].  
-00015930: 2020 2020 2020 7061 6464 6564 5f63 6f6d        padded_com
-00015940: 706f 6e65 6e74 2e61 6464 5f70 6f6c 7967  ponent.add_polyg
-00015950: 6f6e 2870 6f69 6e74 732c 206c 6179 6572  on(points, layer
-00015960: 3d77 6166 6572 5f6c 6179 6572 290a 2020  =wafer_layer).  
-00015970: 2020 2020 2020 7061 6464 6564 5f63 6f6d        padded_com
-00015980: 706f 6e65 6e74 2e61 6464 5f70 6f72 7473  ponent.add_ports
-00015990: 2873 656c 662e 6765 745f 706f 7274 735f  (self.get_ports_
-000159a0: 6c69 7374 2829 290a 0a20 2020 2020 2020  list())..       
-000159b0: 2069 6620 6c61 7965 725f 7374 6163 6b20   if layer_stack 
-000159c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000159d0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-000159e0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-000159f0: 2020 2020 2020 2027 4120 4c61 7965 7253         'A LayerS
-00015a00: 7461 636b 206d 7573 7420 6265 2070 726f  tack must be pro
-00015a10: 7669 6465 6420 7468 726f 7567 6820 6172  vided through ar
-00015a20: 6775 6d65 6e74 2022 6c61 7965 725f 7374  gument "layer_st
-00015a30: 6163 6b22 2e27 0a20 2020 2020 2020 2020  ack".'.         
-00015a40: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-00015a50: 7479 7065 203d 3d20 2278 7922 3a0a 2020  type == "xy":.  
-00015a60: 2020 2020 2020 2020 2020 6966 207a 2069            if z i
-00015a70: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00015a80: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00015a90: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-00015aa0: 2020 2020 2020 2020 2020 2020 2020 2746                'F
-00015ab0: 6f72 2078 792d 6d65 7368 696e 672c 2061  or xy-meshing, a
-00015ac0: 207a 2d76 616c 7565 206d 7573 7420 6265   z-value must be
-00015ad0: 2070 726f 7669 6465 6420 7669 6120 7468   provided via th
-00015ae0: 6520 666c 6f61 7420 6172 6775 6d65 6e74  e float argument
-00015af0: 2022 7a22 2e27 0a20 2020 2020 2020 2020   "z".'.         
-00015b00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00015b10: 2020 2020 2066 726f 6d20 6770 6c75 6769       from gplugi
-00015b20: 6e73 2e67 6d73 682e 7879 5f78 7365 6374  ns.gmsh.xy_xsect
-00015b30: 696f 6e5f 6d65 7368 2069 6d70 6f72 7420  ion_mesh import 
-00015b40: 7879 5f78 7365 6374 696f 6e5f 6d65 7368  xy_xsection_mesh
-00015b50: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00015b60: 7475 726e 2078 795f 7873 6563 7469 6f6e  turn xy_xsection
-00015b70: 5f6d 6573 6828 7061 6464 6564 5f63 6f6d  _mesh(padded_com
-00015b80: 706f 6e65 6e74 2c20 7a2c 206c 6179 6572  ponent, z, layer
-00015b90: 5f73 7461 636b 2c20 2a2a 6b77 6172 6773  _stack, **kwargs
-00015ba0: 290a 2020 2020 2020 2020 656c 6966 2074  ).        elif t
-00015bb0: 7970 6520 3d3d 2022 757a 223a 0a20 2020  ype == "uz":.   
-00015bc0: 2020 2020 2020 2020 2069 6620 7873 6563           if xsec
-00015bd0: 7469 6f6e 5f62 6f75 6e64 7320 6973 204e  tion_bounds is N
-00015be0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00015bf0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00015c00: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00015c10: 2020 2020 2020 2020 2020 2022 466f 7220             "For 
-00015c20: 757a 2d6d 6573 6869 6e67 2c20 796f 7520  uz-meshing, you 
-00015c30: 6d75 7374 2070 726f 7669 6465 2061 206c  must provide a l
-00015c40: 696e 6520 696e 2074 6865 2078 792d 706c  ine in the xy-pl
-00015c50: 616e 6520 220a 2020 2020 2020 2020 2020  ane ".          
-00015c60: 2020 2020 2020 2020 2020 2276 6961 2074            "via t
-00015c70: 6865 2054 7570 6c65 2061 7267 756d 656e  he Tuple argumen
-00015c80: 7420 5b5b 7831 2c79 315d 2c20 5b78 322c  t [[x1,y1], [x2,
-00015c90: 7932 5d5d 2078 7365 6374 696f 6e5f 626f  y2]] xsection_bo
-00015ca0: 756e 6473 2e22 0a20 2020 2020 2020 2020  unds.".         
-00015cb0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00015cc0: 2020 2020 2066 726f 6d20 6770 6c75 6769       from gplugi
-00015cd0: 6e73 2e67 6d73 682e 757a 5f78 7365 6374  ns.gmsh.uz_xsect
-00015ce0: 696f 6e5f 6d65 7368 2069 6d70 6f72 7420  ion_mesh import 
-00015cf0: 757a 5f78 7365 6374 696f 6e5f 6d65 7368  uz_xsection_mesh
-00015d00: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00015d10: 7475 726e 2075 7a5f 7873 6563 7469 6f6e  turn uz_xsection
-00015d20: 5f6d 6573 6828 0a20 2020 2020 2020 2020  _mesh(.         
-00015d30: 2020 2020 2020 2070 6164 6465 645f 636f         padded_co
-00015d40: 6d70 6f6e 656e 742c 2078 7365 6374 696f  mponent, xsectio
-00015d50: 6e5f 626f 756e 6473 2c20 6c61 7965 725f  n_bounds, layer_
-00015d60: 7374 6163 6b2c 202a 2a6b 7761 7267 730a  stack, **kwargs.
-00015d70: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00015d80: 2020 2020 2020 656c 6966 2074 7970 6520        elif type 
-00015d90: 3d3d 2022 3344 223a 0a20 2020 2020 2020  == "3D":.       
-00015da0: 2020 2020 2073 7065 6320 3d20 696d 706f       spec = impo
-00015db0: 7274 6c69 622e 7574 696c 2e66 696e 645f  rtlib.util.find_
-00015dc0: 7370 6563 2822 6d65 7368 7765 6c6c 2229  spec("meshwell")
-00015dd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015de0: 7370 6563 2069 7320 4e6f 6e65 3a0a 2020  spec is None:.  
-00015df0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00015e00: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
-00015e10: 2020 2020 2020 2020 2022 3344 206d 6573           "3D mes
-00015e20: 6869 6e67 2072 6571 7569 7265 7320 6d65  hing requires me
-00015e30: 7368 7765 6c6c 2c20 7365 6520 6874 7470  shwell, see http
-00015e40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00015e50: 696d 6269 6c6f 642f 6d65 7368 7765 6c6c  imbilod/meshwell
-00015e60: 206f 7220 7275 6e20 7069 7020 696e 7374   or run pip inst
-00015e70: 616c 6c20 6d65 7368 7765 6c6c 2e22 0a20  all meshwell.". 
-00015e80: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00015e90: 0a0a 2020 2020 2020 2020 2020 2020 6672  ..            fr
-00015ea0: 6f6d 2067 706c 7567 696e 732e 676d 7368  om gplugins.gmsh
-00015eb0: 2e78 797a 5f6d 6573 6820 696d 706f 7274  .xyz_mesh import
-00015ec0: 2078 797a 5f6d 6573 680a 0a20 2020 2020   xyz_mesh..     
-00015ed0: 2020 2020 2020 2072 6574 7572 6e20 7879         return xy
-00015ee0: 7a5f 6d65 7368 2870 6164 6465 645f 636f  z_mesh(padded_co
-00015ef0: 6d70 6f6e 656e 742c 206c 6179 6572 5f73  mponent, layer_s
-00015f00: 7461 636b 2c20 2a2a 6b77 6172 6773 290a  tack, **kwargs).
-00015f10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00015f20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00015f30: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00015f40: 2020 2020 2020 2020 2020 2020 2752 6571              'Req
-00015f50: 7569 7265 6420 6172 6775 6d65 6e74 2022  uired argument "
-00015f60: 7479 7065 2220 6d75 7374 2062 6520 6f6e  type" must be on
-00015f70: 6520 6f66 2022 7879 222c 2022 757a 222c  e of "xy", "uz",
-00015f80: 206f 7220 2233 4422 2e27 0a20 2020 2020   or "3D".'.     
-00015f90: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00015fa0: 6620 6f66 6673 6574 280a 2020 2020 2020  f offset(.      
-00015fb0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00015fc0: 6469 7374 616e 6365 3a20 666c 6f61 7420  distance: float 
-00015fd0: 3d20 302e 312c 0a20 2020 2020 2020 2070  = 0.1,.        p
-00015fe0: 6f6c 7967 6f6e 733d 4e6f 6e65 2c0a 2020  olygons=None,.  
-00015ff0: 2020 2020 2020 7573 655f 756e 696f 6e3a        use_union:
-00016000: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
-00016010: 2020 2020 2020 7072 6563 6973 696f 6e3a        precision:
-00016020: 2066 6c6f 6174 203d 2031 652d 342c 0a20   float = 1e-4,. 
-00016030: 2020 2020 2020 206a 6f69 6e3a 2073 7472         join: str
-00016040: 203d 2022 6d69 7465 7222 2c0a 2020 2020   = "miter",.    
-00016050: 2020 2020 746f 6c65 7261 6e63 653a 2069      tolerance: i
-00016060: 6e74 203d 2032 2c0a 2020 2020 2020 2020  nt = 2,.        
-00016070: 6c61 7965 723a 204c 6179 6572 5370 6563  layer: LayerSpec
-00016080: 203d 2022 5747 222c 0a20 2020 2029 202d   = "WG",.    ) -
-00016090: 3e20 436f 6d70 6f6e 656e 743a 0a20 2020  > Component:.   
-000160a0: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
-000160b0: 6e65 7720 436f 6d70 6f6e 656e 7420 7769  new Component wi
-000160c0: 7468 2070 6f6c 7967 6f6e 7320 6572 6f64  th polygons erod
-000160d0: 6564 206f 7220 6469 6c61 7465 6420 6279  ed or dilated by
-000160e0: 2061 6e20 6f66 6673 6574 2e0a 0a20 2020   an offset...   
-000160f0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00016100: 2020 2020 2020 2064 6973 7461 6e63 653a         distance:
-00016110: 2044 6973 7461 6e63 6520 746f 206f 6666   Distance to off
-00016120: 7365 7420 706f 6c79 676f 6e73 2e20 506f  set polygons. Po
-00016130: 7369 7469 7665 2076 616c 7565 7320 6578  sitive values ex
-00016140: 7061 6e64 2c20 6e65 6761 7469 7665 2073  pand, negative s
-00016150: 6872 696e 6b2e 0a20 2020 2020 2020 2020  hrink..         
-00016160: 2020 2070 7265 6369 7369 6f6e 3a20 4465     precision: De
-00016170: 7369 7265 6420 7072 6563 6973 696f 6e20  sired precision 
-00016180: 666f 7220 726f 756e 6469 6e67 2076 6572  for rounding ver
-00016190: 7465 7820 636f 6f72 6469 6e61 7465 732e  tex coordinates.
-000161a0: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
-000161b0: 6e3a 207b 276d 6974 6572 272c 2027 6265  n: {'miter', 'be
-000161c0: 7665 6c27 2c20 2772 6f75 6e64 277d 2054  vel', 'round'} T
-000161d0: 7970 6520 6f66 206a 6f69 6e20 7573 6564  ype of join used
-000161e0: 2074 6f20 6372 6561 7465 2070 6f6c 7967   to create polyg
-000161f0: 6f6e 206f 6666 7365 740a 2020 2020 2020  on offset.      
-00016200: 2020 2020 2020 746f 6c65 7261 6e63 653a        tolerance:
-00016210: 2046 6f72 206d 6974 6572 206a 6f69 6e74   For miter joint
-00016220: 732c 2074 6869 7320 6e75 6d62 6572 206d  s, this number m
-00016230: 7573 7420 6265 2061 7420 6c65 6173 7420  ust be at least 
-00016240: 3220 7265 7072 6573 656e 7473 2074 6865  2 represents the
-00016250: 0a20 2020 2020 2020 2020 2020 2020 206d  .              m
-00016260: 6178 696d 616c 2064 6973 7461 6e63 6520  aximal distance 
-00016270: 696e 206d 756c 7469 706c 6573 206f 6620  in multiples of 
-00016280: 6f66 6673 6574 2062 6574 7765 656e 206e  offset between n
-00016290: 6577 2076 6572 7469 6365 7320 616e 6420  ew vertices and 
-000162a0: 7468 6569 720a 2020 2020 2020 2020 2020  their.          
-000162b0: 2020 2020 6f72 6967 696e 616c 2070 6f73      original pos
-000162c0: 6974 696f 6e20 6265 666f 7265 2062 6576  ition before bev
-000162d0: 656c 696e 6720 746f 2061 766f 6964 2073  eling to avoid s
-000162e0: 7069 6b65 7320 6174 2061 6375 7465 206a  pikes at acute j
-000162f0: 6f69 6e74 732e 2046 6f72 0a20 2020 2020  oints. For.     
-00016300: 2020 2020 2020 2020 2072 6f75 6e64 206a           round j
-00016310: 6f69 6e74 732c 2069 7420 696e 6469 6361  oints, it indica
-00016320: 7465 7320 7468 6520 6375 7276 6174 7572  tes the curvatur
-00016330: 6520 7265 736f 6c75 7469 6f6e 2069 6e20  e resolution in 
-00016340: 6e75 6d62 6572 206f 660a 2020 2020 2020  number of.      
-00016350: 2020 2020 2020 2020 706f 696e 7473 2070          points p
-00016360: 6572 2066 756c 6c20 6369 7263 6c65 2e0a  er full circle..
-00016370: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-00016380: 723a 2053 7065 6369 6669 6320 6c61 7965  r: Specific laye
-00016390: 7220 666f 7220 6e65 7720 706f 6c79 676f  r for new polygo
-000163a0: 6e73 2e0a 0a20 2020 2020 2020 2022 2222  ns...        """
-000163b0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-000163c0: 6764 7366 6163 746f 7279 2061 7320 6766  gdsfactory as gf
-000163d0: 0a0a 2020 2020 2020 2020 6764 735f 6c61  ..        gds_la
-000163e0: 7965 722c 2067 6473 5f64 6174 6174 7970  yer, gds_datatyp
-000163f0: 6520 3d20 6766 2e67 6574 5f6c 6179 6572  e = gf.get_layer
-00016400: 286c 6179 6572 290a 2020 2020 2020 2020  (layer).        
-00016410: 7020 3d20 6764 7374 6b2e 6f66 6673 6574  p = gdstk.offset
-00016420: 280a 2020 2020 2020 2020 2020 2020 706f  (.            po
-00016430: 6c79 676f 6e73 206f 7220 7365 6c66 2e67  lygons or self.g
-00016440: 6574 5f70 6f6c 7967 6f6e 7328 292c 0a20  et_polygons(),. 
-00016450: 2020 2020 2020 2020 2020 2064 6973 7461             dista
-00016460: 6e63 653d 6469 7374 616e 6365 2c0a 2020  nce=distance,.  
-00016470: 2020 2020 2020 2020 2020 6a6f 696e 3d6a            join=j
-00016480: 6f69 6e2c 0a20 2020 2020 2020 2020 2020  oin,.           
-00016490: 2074 6f6c 6572 616e 6365 3d74 6f6c 6572   tolerance=toler
-000164a0: 616e 6365 2c0a 2020 2020 2020 2020 2020  ance,.          
-000164b0: 2020 7072 6563 6973 696f 6e3d 7072 6563    precision=prec
-000164c0: 6973 696f 6e2c 0a20 2020 2020 2020 2020  ision,.         
-000164d0: 2020 2075 7365 5f75 6e69 6f6e 3d75 7365     use_union=use
-000164e0: 5f75 6e69 6f6e 2c0a 2020 2020 2020 2020  _union,.        
-000164f0: 2020 2020 6c61 7965 723d 6764 735f 6c61      layer=gds_la
-00016500: 7965 722c 0a20 2020 2020 2020 2020 2020  yer,.           
-00016510: 2064 6174 6174 7970 653d 6764 735f 6461   datatype=gds_da
-00016520: 7461 7479 7065 2c0a 2020 2020 2020 2020  tatype,.        
-00016530: 290a 0a20 2020 2020 2020 2063 6f6d 706f  )..        compo
-00016540: 6e65 6e74 203d 2067 662e 436f 6d70 6f6e  nent = gf.Compon
-00016550: 656e 7428 290a 2020 2020 2020 2020 636f  ent().        co
-00016560: 6d70 6f6e 656e 742e 6164 645f 706f 6c79  mponent.add_poly
-00016570: 676f 6e28 702c 206c 6179 6572 3d6c 6179  gon(p, layer=lay
-00016580: 6572 290a 2020 2020 2020 2020 7265 7475  er).        retu
-00016590: 726e 2063 6f6d 706f 6e65 6e74 0a0a 0a64  rn component...d
-000165a0: 6566 2063 6f70 7928 0a20 2020 2044 3a20  ef copy(.    D: 
-000165b0: 436f 6d70 6f6e 656e 742c 0a20 2020 2072  Component,.    r
-000165c0: 6566 6572 656e 6365 733d 4e6f 6e65 2c0a  eferences=None,.
-000165d0: 2020 2020 706f 7274 733d 4e6f 6e65 2c0a      ports=None,.
-000165e0: 2020 2020 706f 6c79 676f 6e73 3d4e 6f6e      polygons=Non
-000165f0: 652c 0a20 2020 2070 6174 6873 3d4e 6f6e  e,.    paths=Non
-00016600: 652c 0a20 2020 206e 616d 653d 4e6f 6e65  e,.    name=None
-00016610: 2c0a 2020 2020 6c61 6265 6c73 3d4e 6f6e  ,.    labels=Non
-00016620: 652c 0a29 202d 3e20 436f 6d70 6f6e 656e  e,.) -> Componen
-00016630: 743a 0a20 2020 2022 2222 5265 7475 726e  t:.    """Return
-00016640: 7320 6120 436f 6d70 6f6e 656e 7420 636f  s a Component co
-00016650: 7079 2e0a 0a20 2020 2041 7267 733a 0a20  py...    Args:. 
-00016660: 2020 2020 2020 2044 3a20 636f 6d70 6f6e         D: compon
-00016670: 656e 7420 746f 2063 6f70 792e 0a20 2020  ent to copy..   
-00016680: 2022 2222 0a20 2020 2044 5f63 6f70 7920   """.    D_copy 
-00016690: 3d20 436f 6d70 6f6e 656e 7428 290a 2020  = Component().  
-000166a0: 2020 445f 636f 7079 2e69 6e66 6f20 3d20    D_copy.info = 
-000166b0: 442e 696e 666f 0a20 2020 2023 2044 5f63  D.info.    # D_c
-000166c0: 6f70 792e 5f63 656c 6c20 3d20 442e 5f63  opy._cell = D._c
-000166d0: 656c 6c2e 636f 7079 286e 616d 653d 445f  ell.copy(name=D_
-000166e0: 636f 7079 2e6e 616d 6529 0a0a 2020 2020  copy.name)..    
-000166f0: 666f 7220 7265 6620 696e 2072 6566 6572  for ref in refer
-00016700: 656e 6365 7320 6966 2072 6566 6572 656e  ences if referen
-00016710: 6365 7320 6973 206e 6f74 204e 6f6e 6520  ces is not None 
-00016720: 656c 7365 2044 2e72 6566 6572 656e 6365  else D.reference
-00016730: 733a 0a20 2020 2020 2020 2044 5f63 6f70  s:.        D_cop
-00016740: 792e 6164 6428 636f 7079 5f72 6566 6572  y.add(copy_refer
-00016750: 656e 6365 2872 6566 2929 0a20 2020 2066  ence(ref)).    f
-00016760: 6f72 2070 6f72 7420 696e 2028 706f 7274  or port in (port
-00016770: 7320 6966 2070 6f72 7473 2069 7320 6e6f  s if ports is no
-00016780: 7420 4e6f 6e65 2065 6c73 6520 442e 706f  t None else D.po
-00016790: 7274 7329 2e76 616c 7565 7328 293a 0a20  rts).values():. 
-000167a0: 2020 2020 2020 2044 5f63 6f70 792e 6164         D_copy.ad
-000167b0: 645f 706f 7274 2870 6f72 743d 706f 7274  d_port(port=port
-000167c0: 290a 2020 2020 666f 7220 706f 6c79 2069  ).    for poly i
-000167d0: 6e20 706f 6c79 676f 6e73 2069 6620 706f  n polygons if po
-000167e0: 6c79 676f 6e73 2069 7320 6e6f 7420 4e6f  lygons is not No
-000167f0: 6e65 2065 6c73 6520 442e 706f 6c79 676f  ne else D.polygo
-00016800: 6e73 3a0a 2020 2020 2020 2020 445f 636f  ns:.        D_co
-00016810: 7079 2e61 6464 5f70 6f6c 7967 6f6e 2870  py.add_polygon(p
-00016820: 6f6c 7929 0a20 2020 2066 6f72 2070 6174  oly).    for pat
-00016830: 6820 696e 2070 6174 6873 2069 6620 7061  h in paths if pa
-00016840: 7468 7320 6973 206e 6f74 204e 6f6e 6520  ths is not None 
-00016850: 656c 7365 2044 2e70 6174 6873 3a0a 2020  else D.paths:.  
-00016860: 2020 2020 2020 445f 636f 7079 2e61 6464        D_copy.add
-00016870: 2870 6174 6829 0a20 2020 2066 6f72 206c  (path).    for l
-00016880: 6162 656c 2069 6e20 6c61 6265 6c73 2069  abel in labels i
-00016890: 6620 6c61 6265 6c73 2069 7320 6e6f 7420  f labels is not 
-000168a0: 4e6f 6e65 2065 6c73 6520 442e 6c61 6265  None else D.labe
-000168b0: 6c73 3a0a 2020 2020 2020 2020 445f 636f  ls:.        D_co
-000168c0: 7079 2e61 6464 5f6c 6162 656c 280a 2020  py.add_label(.  
-000168d0: 2020 2020 2020 2020 2020 7465 7874 3d6c            text=l
-000168e0: 6162 656c 2e74 6578 742c 0a20 2020 2020  abel.text,.     
-000168f0: 2020 2020 2020 2070 6f73 6974 696f 6e3d         position=
-00016900: 6c61 6265 6c2e 6f72 6967 696e 2c0a 2020  label.origin,.  
-00016910: 2020 2020 2020 2020 2020 6c61 7965 723d            layer=
-00016920: 286c 6162 656c 2e6c 6179 6572 2c20 6c61  (label.layer, la
-00016930: 6265 6c2e 7465 7874 7479 7065 292c 0a20  bel.texttype),. 
-00016940: 2020 2020 2020 2029 0a0a 2020 2020 6966         )..    if
-00016950: 206e 616d 6520 6973 206e 6f74 204e 6f6e   name is not Non
-00016960: 653a 0a20 2020 2020 2020 2044 5f63 6f70  e:.        D_cop
-00016970: 792e 6e61 6d65 203d 206e 616d 650a 0a20  y.name = name.. 
-00016980: 2020 2072 6574 7572 6e20 445f 636f 7079     return D_copy
-00016990: 0a0a 0a64 6566 2063 6f70 795f 7265 6665  ...def copy_refe
-000169a0: 7265 6e63 6528 0a20 2020 2072 6566 2c0a  rence(.    ref,.
-000169b0: 2020 2020 7061 7265 6e74 3d4e 6f6e 652c      parent=None,
-000169c0: 0a20 2020 2063 6f6c 756d 6e73 3d4e 6f6e  .    columns=Non
-000169d0: 652c 0a20 2020 2072 6f77 733d 4e6f 6e65  e,.    rows=None
-000169e0: 2c0a 2020 2020 7370 6163 696e 673d 4e6f  ,.    spacing=No
-000169f0: 6e65 2c0a 2020 2020 6f72 6967 696e 3d4e  ne,.    origin=N
-00016a00: 6f6e 652c 0a20 2020 2072 6f74 6174 696f  one,.    rotatio
-00016a10: 6e3d 4e6f 6e65 2c0a 2020 2020 6d61 676e  n=None,.    magn
-00016a20: 6966 6963 6174 696f 6e3d 4e6f 6e65 2c0a  ification=None,.
-00016a30: 2020 2020 785f 7265 666c 6563 7469 6f6e      x_reflection
-00016a40: 3d4e 6f6e 652c 0a20 2020 206e 616d 653d  =None,.    name=
-00016a50: 4e6f 6e65 2c0a 2020 2020 7631 3d4e 6f6e  None,.    v1=Non
-00016a60: 652c 0a20 2020 2076 323d 4e6f 6e65 2c0a  e,.    v2=None,.
-00016a70: 2920 2d3e 2043 6f6d 706f 6e65 6e74 5265  ) -> ComponentRe
-00016a80: 6665 7265 6e63 653a 0a20 2020 2072 6574  ference:.    ret
-00016a90: 7572 6e20 436f 6d70 6f6e 656e 7452 6566  urn ComponentRef
-00016aa0: 6572 656e 6365 280a 2020 2020 2020 2020  erence(.        
-00016ab0: 636f 6d70 6f6e 656e 743d 7061 7265 6e74  component=parent
-00016ac0: 206f 7220 7265 662e 7061 7265 6e74 2c0a   or ref.parent,.
-00016ad0: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-00016ae0: 636f 6c75 6d6e 7320 6f72 2072 6566 2e63  columns or ref.c
-00016af0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
-00016b00: 726f 7773 3d72 6f77 7320 6f72 2072 6566  rows=rows or ref
-00016b10: 2e72 6f77 732c 0a20 2020 2020 2020 2073  .rows,.        s
-00016b20: 7061 6369 6e67 3d73 7061 6369 6e67 206f  pacing=spacing o
-00016b30: 7220 7265 662e 7370 6163 696e 672c 0a20  r ref.spacing,. 
-00016b40: 2020 2020 2020 206f 7269 6769 6e3d 6f72         origin=or
-00016b50: 6967 696e 206f 7220 7265 662e 6f72 6967  igin or ref.orig
-00016b60: 696e 2c0a 2020 2020 2020 2020 726f 7461  in,.        rota
-00016b70: 7469 6f6e 3d72 6f74 6174 696f 6e20 6f72  tion=rotation or
-00016b80: 2072 6566 2e72 6f74 6174 696f 6e2c 0a20   ref.rotation,. 
-00016b90: 2020 2020 2020 206d 6167 6e69 6669 6361         magnifica
-00016ba0: 7469 6f6e 3d6d 6167 6e69 6669 6361 7469  tion=magnificati
-00016bb0: 6f6e 206f 7220 7265 662e 6d61 676e 6966  on or ref.magnif
-00016bc0: 6963 6174 696f 6e2c 0a20 2020 2020 2020  ication,.       
-00016bd0: 2078 5f72 6566 6c65 6374 696f 6e3d 785f   x_reflection=x_
-00016be0: 7265 666c 6563 7469 6f6e 206f 7220 7265  reflection or re
-00016bf0: 662e 785f 7265 666c 6563 7469 6f6e 2c0a  f.x_reflection,.
-00016c00: 2020 2020 2020 2020 6e61 6d65 3d6e 616d          name=nam
-00016c10: 6520 6f72 2072 6566 2e6e 616d 652c 0a20  e or ref.name,. 
-00016c20: 2020 2020 2020 2076 313d 7631 206f 7220         v1=v1 or 
-00016c30: 7265 662e 7631 2c0a 2020 2020 2020 2020  ref.v1,.        
-00016c40: 7632 3d76 3220 6f72 2072 6566 2e76 322c  v2=v2 or ref.v2,
-00016c50: 0a20 2020 2029 0a0a 0a64 6566 2074 6573  .    )...def tes
-00016c60: 745f 6765 745f 6c61 7965 7273 2829 202d  t_get_layers() -
-00016c70: 3e20 4e6f 6e65 3a0a 2020 2020 696d 706f  > None:.    impo
-00016c80: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
-00016c90: 2067 660a 0a20 2020 2063 3120 3d20 6766   gf..    c1 = gf
-00016ca0: 2e63 6f6d 706f 6e65 6e74 732e 7374 7261  .components.stra
-00016cb0: 6967 6874 280a 2020 2020 2020 2020 6c65  ight(.        le
-00016cc0: 6e67 7468 3d31 302c 0a20 2020 2020 2020  ngth=10,.       
-00016cd0: 2077 6964 7468 3d30 2e35 2c0a 2020 2020   width=0.5,.    
-00016ce0: 2020 2020 6c61 7965 723d 2832 2c20 3029      layer=(2, 0)
-00016cf0: 2c0a 2020 2020 2020 2020 6262 6f78 5f6c  ,.        bbox_l
-00016d00: 6179 6572 733d 5b28 3131 312c 2030 295d  ayers=[(111, 0)]
-00016d10: 2c0a 2020 2020 2020 2020 6262 6f78 5f6f  ,.        bbox_o
-00016d20: 6666 7365 7473 3d5b 335d 2c0a 2020 2020  ffsets=[3],.    
-00016d30: 2020 2020 7769 7468 5f62 626f 783d 5472      with_bbox=Tr
-00016d40: 7565 2c0a 2020 2020 2020 2020 636c 6164  ue,.        clad
-00016d50: 6469 6e67 5f6c 6179 6572 733d 4e6f 6e65  ding_layers=None
-00016d60: 2c0a 2020 2020 2020 2020 6164 645f 7069  ,.        add_pi
-00016d70: 6e73 3d4e 6f6e 652c 0a20 2020 2020 2020  ns=None,.       
-00016d80: 2061 6464 5f62 626f 783d 4e6f 6e65 2c0a   add_bbox=None,.
-00016d90: 2020 2020 290a 2020 2020 6173 7365 7274      ).    assert
-00016da0: 2063 312e 6765 745f 6c61 7965 7273 2829   c1.get_layers()
-00016db0: 203d 3d20 7b28 322c 2030 292c 2028 3131   == {(2, 0), (11
-00016dc0: 312c 2030 297d 2c20 6331 2e67 6574 5f6c  1, 0)}, c1.get_l
-00016dd0: 6179 6572 7328 290a 2020 2020 2320 7265  ayers().    # re
-00016de0: 7475 726e 2063 310a 2020 2020 6332 203d  turn c1.    c2 =
-00016df0: 2063 312e 7265 6d6f 7665 5f6c 6179 6572   c1.remove_layer
-00016e00: 7328 5b28 3131 312c 2030 295d 290a 2020  s([(111, 0)]).  
-00016e10: 2020 6173 7365 7274 2063 322e 6765 745f    assert c2.get_
-00016e20: 6c61 7965 7273 2829 203d 3d20 7b28 322c  layers() == {(2,
-00016e30: 2030 297d 2c20 6332 2e67 6574 5f6c 6179   0)}, c2.get_lay
-00016e40: 6572 7328 290a 0a0a 6465 6620 5f66 696c  ers()...def _fil
-00016e50: 7465 725f 706f 6c79 7328 706f 6c79 676f  ter_polys(polygo
-00016e60: 6e73 2c20 6c61 7965 7273 5f65 7863 6c29  ns, layers_excl)
-00016e70: 3a0a 2020 2020 7265 7475 726e 205b 0a20  :.    return [. 
-00016e80: 2020 2020 2020 2070 6f6c 7967 6f6e 0a20         polygon. 
-00016e90: 2020 2020 2020 2066 6f72 2070 6f6c 7967         for polyg
-00016ea0: 6f6e 2c20 6c61 7965 722c 2064 6174 6174  on, layer, datat
-00016eb0: 7970 6520 696e 207a 6970 280a 2020 2020  ype in zip(.    
-00016ec0: 2020 2020 2020 2020 706f 6c79 676f 6e73          polygons
-00016ed0: 2e70 6f6c 7967 6f6e 732c 2070 6f6c 7967  .polygons, polyg
-00016ee0: 6f6e 732e 6c61 7965 7273 2c20 706f 6c79  ons.layers, poly
-00016ef0: 676f 6e73 2e64 6174 6174 7970 6573 0a20  gons.datatypes. 
-00016f00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00016f10: 2069 6620 286c 6179 6572 2c20 6461 7461   if (layer, data
-00016f20: 7479 7065 2920 6e6f 7420 696e 206c 6179  type) not in lay
-00016f30: 6572 735f 6578 636c 0a20 2020 205d 0a0a  ers_excl.    ]..
-00016f40: 0a64 6566 2072 6563 7572 7365 5f73 7472  .def recurse_str
-00016f50: 7563 7475 7265 7328 0a20 2020 2063 6f6d  uctures(.    com
-00016f60: 706f 6e65 6e74 3a20 436f 6d70 6f6e 656e  ponent: Componen
-00016f70: 742c 0a20 2020 2069 676e 6f72 655f 636f  t,.    ignore_co
-00016f80: 6d70 6f6e 656e 7473 5f70 7265 6669 783a  mponents_prefix:
-00016f90: 206c 6973 745b 7374 725d 207c 204e 6f6e   list[str] | Non
-00016fa0: 6520 3d20 4e6f 6e65 2c0a 2020 2020 6967  e = None,.    ig
-00016fb0: 6e6f 7265 5f66 756e 6374 696f 6e73 5f70  nore_functions_p
-00016fc0: 7265 6669 783a 206c 6973 745b 7374 725d  refix: list[str]
-00016fd0: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
-00016fe0: 2920 2d3e 2064 6963 745b 7374 722c 2041  ) -> dict[str, A
-00016ff0: 6e79 5d3a 0a20 2020 2022 2222 5265 6375  ny]:.    """Recu
-00017000: 7273 6520 636f 6d70 6f6e 656e 7420 616e  rse component an
-00017010: 6420 636f 6d70 6f6e 656e 7473 2072 6566  d components ref
-00017020: 6572 656e 6365 7320 7265 6375 7273 6976  erences recursiv
-00017030: 656c 792e 0a0a 2020 2020 4172 6773 3a0a  ely...    Args:.
-00017040: 2020 2020 2020 2020 636f 6d70 6f6e 656e          componen
-00017050: 743a 2063 6f6d 706f 6e65 6e74 2074 6f20  t: component to 
-00017060: 7265 6375 7273 652e 0a20 2020 2020 2020  recurse..       
-00017070: 2069 676e 6f72 655f 636f 6d70 6f6e 656e   ignore_componen
-00017080: 7473 5f70 7265 6669 783a 206c 6973 7420  ts_prefix: list 
-00017090: 6f66 2070 7265 6669 7820 746f 2069 676e  of prefix to ign
-000170a0: 6f72 652e 0a20 2020 2020 2020 2069 676e  ore..        ign
-000170b0: 6f72 655f 6675 6e63 7469 6f6e 735f 7072  ore_functions_pr
-000170c0: 6566 6978 3a20 6c69 7374 206f 6620 7072  efix: list of pr
-000170d0: 6566 6978 2074 6f20 6967 6e6f 7265 2e0a  efix to ignore..
-000170e0: 2020 2020 2222 220a 2020 2020 6967 6e6f      """.    igno
-000170f0: 7265 5f66 756e 6374 696f 6e73 5f70 7265  re_functions_pre
-00017100: 6669 7820 3d20 6967 6e6f 7265 5f66 756e  fix = ignore_fun
-00017110: 6374 696f 6e73 5f70 7265 6669 7820 6f72  ctions_prefix or
-00017120: 205b 5d0a 2020 2020 6967 6e6f 7265 5f63   [].    ignore_c
-00017130: 6f6d 706f 6e65 6e74 735f 7072 6566 6978  omponents_prefix
-00017140: 203d 2069 676e 6f72 655f 636f 6d70 6f6e   = ignore_compon
-00017150: 656e 7473 5f70 7265 6669 7820 6f72 205b  ents_prefix or [
-00017160: 5d0a 0a20 2020 2069 6620 280a 2020 2020  ]..    if (.    
-00017170: 2020 2020 6861 7361 7474 7228 636f 6d70      hasattr(comp
-00017180: 6f6e 656e 742c 2022 6675 6e63 7469 6f6e  onent, "function
-00017190: 5f6e 616d 6522 290a 2020 2020 2020 2020  _name").        
-000171a0: 616e 6420 636f 6d70 6f6e 656e 742e 6675  and component.fu
-000171b0: 6e63 7469 6f6e 5f6e 616d 6520 696e 2069  nction_name in i
-000171c0: 676e 6f72 655f 6675 6e63 7469 6f6e 735f  gnore_functions_
-000171d0: 7072 6566 6978 0a20 2020 2029 3a0a 2020  prefix.    ):.  
-000171e0: 2020 2020 2020 7265 7475 726e 207b 7d0a        return {}.
-000171f0: 0a20 2020 2069 6620 6861 7361 7474 7228  .    if hasattr(
-00017200: 636f 6d70 6f6e 656e 742c 2022 6e61 6d65  component, "name
-00017210: 2229 2061 6e64 2061 6e79 280a 2020 2020  ") and any(.    
-00017220: 2020 2020 636f 6d70 6f6e 656e 742e 6e61      component.na
-00017230: 6d65 2e73 7461 7274 7377 6974 6828 6929  me.startswith(i)
-00017240: 2066 6f72 2069 2069 6e20 6967 6e6f 7265   for i in ignore
-00017250: 5f63 6f6d 706f 6e65 6e74 735f 7072 6566  _components_pref
-00017260: 6978 0a20 2020 2029 3a0a 2020 2020 2020  ix.    ):.      
-00017270: 2020 7265 7475 726e 207b 7d0a 0a20 2020    return {}..   
-00017280: 206f 7574 7075 7420 3d20 7b63 6f6d 706f   output = {compo
-00017290: 6e65 6e74 2e6e 616d 653a 2064 6963 7428  nent.name: dict(
-000172a0: 636f 6d70 6f6e 656e 742e 7365 7474 696e  component.settin
-000172b0: 6773 297d 0a20 2020 2066 6f72 2072 6566  gs)}.    for ref
-000172c0: 6572 656e 6365 2069 6e20 636f 6d70 6f6e  erence in compon
-000172d0: 656e 742e 7265 6665 7265 6e63 6573 3a0a  ent.references:.
-000172e0: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-000172f0: 2020 2020 2020 2020 2069 7369 6e73 7461           isinsta
-00017300: 6e63 6528 7265 6665 7265 6e63 652c 2043  nce(reference, C
-00017310: 6f6d 706f 6e65 6e74 5265 6665 7265 6e63  omponentReferenc
-00017320: 6529 0a20 2020 2020 2020 2020 2020 2061  e).            a
-00017330: 6e64 2072 6566 6572 656e 6365 2e72 6566  nd reference.ref
-00017340: 5f63 656c 6c2e 6e61 6d65 206e 6f74 2069  _cell.name not i
-00017350: 6e20 6f75 7470 7574 0a20 2020 2020 2020  n output.       
-00017360: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00017370: 6f75 7470 7574 2e75 7064 6174 6528 7265  output.update(re
-00017380: 6375 7273 655f 7374 7275 6374 7572 6573  curse_structures
-00017390: 2872 6566 6572 656e 6365 2e72 6566 5f63  (reference.ref_c
-000173a0: 656c 6c29 290a 0a20 2020 2072 6574 7572  ell))..    retur
-000173b0: 6e20 6f75 7470 7574 0a0a 0a64 6566 2066  n output...def f
-000173c0: 6c61 7474 656e 5f69 6e76 616c 6964 5f72  latten_invalid_r
-000173d0: 6566 735f 7265 6375 7273 6976 6528 0a20  efs_recursive(. 
-000173e0: 2020 2063 6f6d 706f 6e65 6e74 3a20 436f     component: Co
-000173f0: 6d70 6f6e 656e 742c 0a20 2020 2067 7269  mponent,.    gri
-00017400: 645f 7369 7a65 3a20 666c 6f61 7420 7c20  d_size: float | 
-00017410: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
-00017420: 2075 7064 6174 6564 5f63 6f6d 706f 6e65   updated_compone
-00017430: 6e74 733d 4e6f 6e65 2c0a 2020 2020 7472  nts=None,.    tr
-00017440: 6176 6572 7365 645f 636f 6d70 6f6e 656e  aversed_componen
-00017450: 7473 3d4e 6f6e 652c 0a29 3a0a 2020 2020  ts=None,.):.    
-00017460: 2222 2252 6563 7572 7369 7665 6c79 2066  """Recursively f
-00017470: 6c61 7474 656e 7320 636f 6d70 6f6e 656e  lattens componen
-00017480: 7420 7265 6665 7265 6e63 6573 2077 6869  t references whi
-00017490: 6368 2068 6176 6520 696e 7661 6c69 6420  ch have invalid 
-000174a0: 7472 616e 7366 6f72 6d61 7469 6f6e 7320  transformations 
-000174b0: 2869 2e65 2e20 6e6f 6e2d 3930 2064 6567  (i.e. non-90 deg
-000174c0: 2072 6f74 6174 696f 6e73 206f 7220 7375   rotations or su
-000174d0: 622d 6772 6964 2074 7261 6e73 6c61 7469  b-grid translati
-000174e0: 6f6e 7329 2061 6e64 2072 6574 7572 6e73  ons) and returns
-000174f0: 2061 2063 6f70 7920 6966 2061 6e79 2073   a copy if any s
-00017500: 7562 6365 6c6c 7320 6861 7665 2062 6565  ubcells have bee
-00017510: 6e20 6d6f 6469 6669 6564 2e0a 0a20 2020  n modified...   
-00017520: 2057 4152 4e49 4e47 3a20 7468 6973 2066   WARNING: this f
-00017530: 756e 6374 696f 6e20 7769 6c6c 2070 726f  unction will pro
-00017540: 6475 6365 2073 616d 652d 6e61 6d65 2063  duce same-name c
-00017550: 6f70 6965 7320 6f66 2063 656c 6c73 2e20  opies of cells. 
-00017560: 4974 2069 7320 7374 7269 6374 6c79 206d  It is strictly m
-00017570: 6561 6e74 2074 6f20 6265 2075 7365 6420  eant to be used 
-00017580: 6f6e 2077 7269 7465 206f 6620 7468 6520  on write of the 
-00017590: 4744 5320 6669 6c65 2061 6e64 0a20 2020  GDS file and.   
-000175a0: 2073 686f 756c 6420 6e6f 7420 6265 206d   should not be m
-000175b0: 6978 6564 2077 6974 6820 6f74 6865 7220  ixed with other 
-000175c0: 6365 6c6c 732c 206f 7220 796f 7520 7769  cells, or you wi
-000175d0: 6c6c 206c 696b 656c 7920 6578 7065 7269  ll likely experi
-000175e0: 656e 6365 2069 7373 7565 7320 7769 7468  ence issues with
-000175f0: 2064 7570 6c69 6361 7465 2063 656c 6c73   duplicate cells
-00017600: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00017610: 2020 2020 636f 6d70 6f6e 656e 743a 2074      component: t
-00017620: 6865 2063 6f6d 706f 6e65 6e74 2074 6f20  he component to 
-00017630: 6669 7820 2869 6e20 706c 6163 6529 2e0a  fix (in place)..
-00017640: 2020 2020 2020 2020 6772 6964 5f73 697a          grid_siz
-00017650: 653a 2074 6865 2047 4453 2067 7269 6420  e: the GDS grid 
-00017660: 7369 7a65 2c20 696e 2075 6d2c 2064 6566  size, in um, def
-00017670: 6175 6c74 7320 746f 2061 6374 6976 6520  aults to active 
-00017680: 5044 4b2e 6765 745f 6772 6964 5f73 697a  PDK.get_grid_siz
-00017690: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-000176a0: 616e 7920 7472 616e 736c 6174 696f 6e73  any translations
-000176b0: 2077 6974 6820 6869 6768 6572 2072 6573   with higher res
-000176c0: 6f6c 7574 696f 6e20 7468 616e 2074 6869  olution than thi
-000176d0: 7320 6172 6520 636f 6e73 6964 6572 6564  s are considered
-000176e0: 2069 6e76 616c 6964 2e0a 2020 2020 2020   invalid..      
-000176f0: 2020 7570 6461 7465 645f 636f 6d70 6f6e    updated_compon
-00017700: 656e 7473 3a20 7468 6520 7275 6e6e 696e  ents: the runnin
-00017710: 6720 6469 6374 696f 6e61 7279 206f 6620  g dictionary of 
-00017720: 636f 6d70 6f6e 656e 7473 2077 6869 6368  components which
-00017730: 2068 6176 6520 6265 656e 206d 6f64 6966   have been modif
-00017740: 6965 6420 6279 2074 6869 7320 7472 616e  ied by this tran
-00017750: 7366 6f72 6d61 7469 6f6e 2e20 5368 6f75  sformation. Shou
-00017760: 6c64 2061 6c77 6179 7320 6265 204e 6f6e  ld always be Non
-00017770: 652c 2065 7863 6570 7420 666f 7220 7265  e, except for re
-00017780: 6375 7273 6976 6520 696e 766f 6361 7469  cursive invocati
-00017790: 6f6e 732e 0a20 2020 2020 2020 2074 7261  ons..        tra
-000177a0: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
-000177b0: 733a 2074 6865 2073 6574 206f 6620 636f  s: the set of co
-000177c0: 6d70 6f6e 656e 7420 6e61 6d65 7320 7768  mponent names wh
-000177d0: 6963 6820 6861 7665 2062 6565 6e20 7472  ich have been tr
-000177e0: 6176 6572 7365 642e 2053 686f 756c 6420  aversed. Should 
-000177f0: 616c 7761 7973 2062 6520 4e6f 6e65 2c20  always be None, 
-00017800: 6578 6365 7074 2066 6f72 2072 6563 7572  except for recur
-00017810: 7369 7665 2069 6e76 6f63 6174 696f 6e73  sive invocations
-00017820: 2e0a 2020 2020 2222 220a 2020 2020 6672  ..    """.    fr
-00017830: 6f6d 2067 6473 6661 6374 6f72 792e 6465  om gdsfactory.de
-00017840: 636f 7261 746f 7273 2069 6d70 6f72 7420  corators import 
-00017850: 6973 5f69 6e76 616c 6964 5f72 6566 0a0a  is_invalid_ref..
-00017860: 2020 2020 696e 7661 6c69 645f 7265 6673      invalid_refs
-00017870: 203d 205b 5d0a 2020 2020 7265 6673 203d   = [].    refs =
-00017880: 2063 6f6d 706f 6e65 6e74 2e72 6566 6572   component.refer
-00017890: 656e 6365 730a 2020 2020 7375 6263 656c  ences.    subcel
-000178a0: 6c5f 6d6f 6469 6669 6564 203d 2046 616c  l_modified = Fal
-000178b0: 7365 0a20 2020 2069 6620 7570 6461 7465  se.    if update
-000178c0: 645f 636f 6d70 6f6e 656e 7473 2069 7320  d_components is 
-000178d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7570  None:.        up
-000178e0: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
-000178f0: 203d 207b 7d0a 2020 2020 6966 2074 7261   = {}.    if tra
-00017900: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
-00017910: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-00017920: 2020 2074 7261 7665 7273 6564 5f63 6f6d     traversed_com
-00017930: 706f 6e65 6e74 7320 3d20 7365 7428 290a  ponents = set().
-00017940: 2020 2020 666f 7220 7265 6620 696e 2072      for ref in r
-00017950: 6566 733a 0a20 2020 2020 2020 2023 206d  efs:.        # m
-00017960: 6172 6b20 616e 7920 696e 7661 6c69 6420  ark any invalid 
-00017970: 7265 6673 2066 6f72 2066 6c61 7474 656e  refs for flatten
-00017980: 696e 670a 2020 2020 2020 2020 2320 6f74  ing.        # ot
-00017990: 6865 7277 6973 652c 2063 6865 636b 2069  herwise, check i
-000179a0: 6620 7468 6572 6520 6172 6520 616e 7920  f there are any 
-000179b0: 6d6f 6469 6669 6564 2063 656c 6c73 2062  modified cells b
-000179c0: 656e 6561 7468 2028 7765 206e 6565 6420  eneath (we need 
-000179d0: 6e6f 7420 646f 2074 6869 7320 6966 2074  not do this if t
-000179e0: 6865 2072 6566 2077 696c 6c20 6265 2066  he ref will be f
-000179f0: 6c61 7474 656e 6564 2061 6e79 7761 7973  lattened anyways
-00017a00: 290a 2020 2020 2020 2020 6966 2069 735f  ).        if is_
-00017a10: 696e 7661 6c69 645f 7265 6628 7265 662c  invalid_ref(ref,
-00017a20: 2067 7269 645f 7369 7a65 293a 0a20 2020   grid_size):.   
-00017a30: 2020 2020 2020 2020 2069 6e76 616c 6964           invalid
-00017a40: 5f72 6566 732e 6170 7065 6e64 2872 6566  _refs.append(ref
-00017a50: 2e6e 616d 6529 0a20 2020 2020 2020 2065  .name).        e
-00017a60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00017a70: 2023 206f 7468 6572 7769 7365 2c20 7265   # otherwise, re
-00017a80: 6375 7273 6976 656c 7920 666c 6174 7465  cursively flatte
-00017a90: 6e20 7265 6673 2069 6620 7468 6520 7375  n refs if the su
-00017aa0: 6263 656c 6c20 6861 7320 6e6f 7420 616c  bcell has not al
-00017ab0: 7265 6164 7920 6265 656e 2074 7261 7665  ready been trave
-00017ac0: 7273 6564 0a20 2020 2020 2020 2020 2020  rsed.           
-00017ad0: 2069 6620 7265 662e 7061 7265 6e74 2e6e   if ref.parent.n
-00017ae0: 616d 6520 6e6f 7420 696e 2074 7261 7665  ame not in trave
-00017af0: 7273 6564 5f63 6f6d 706f 6e65 6e74 733a  rsed_components:
-00017b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017b10: 2066 6c61 7474 656e 5f69 6e76 616c 6964   flatten_invalid
-00017b20: 5f72 6566 735f 7265 6375 7273 6976 6528  _refs_recursive(
-00017b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017b40: 2020 2020 2072 6566 2e70 6172 656e 742c       ref.parent,
-00017b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017b60: 2020 2020 2067 7269 645f 7369 7a65 3d67       grid_size=g
-00017b70: 7269 645f 7369 7a65 2c0a 2020 2020 2020  rid_size,.      
-00017b80: 2020 2020 2020 2020 2020 2020 2020 7570                up
-00017b90: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
-00017ba0: 3d75 7064 6174 6564 5f63 6f6d 706f 6e65  =updated_compone
-00017bb0: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
-00017bc0: 2020 2020 2020 2020 2074 7261 7665 7273           travers
-00017bd0: 6564 5f63 6f6d 706f 6e65 6e74 733d 7472  ed_components=tr
-00017be0: 6176 6572 7365 645f 636f 6d70 6f6e 656e  aversed_componen
-00017bf0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-00017c00: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00017c10: 2020 2320 6e6f 772c 2069 6620 7468 6520    # now, if the 
-00017c20: 7265 6627 7320 6365 6c6c 2062 6565 6e20  ref's cell been 
-00017c30: 6d6f 6469 6669 6564 2c20 6d61 726b 2069  modified, mark i
-00017c40: 7420 6173 2073 7563 680a 2020 2020 2020  t as such.      
-00017c50: 2020 2020 2020 6966 2072 6566 2e70 6172        if ref.par
-00017c60: 656e 742e 6e61 6d65 2069 6e20 7570 6461  ent.name in upda
-00017c70: 7465 645f 636f 6d70 6f6e 656e 7473 3a0a  ted_components:.
-00017c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c90: 7375 6263 656c 6c5f 6d6f 6469 6669 6564  subcell_modified
-00017ca0: 203d 2054 7275 650a 2020 2020 6966 2069   = True.    if i
-00017cb0: 6e76 616c 6964 5f72 6566 7320 6f72 2073  nvalid_refs or s
-00017cc0: 7562 6365 6c6c 5f6d 6f64 6966 6965 643a  ubcell_modified:
-00017cd0: 0a20 2020 2020 2020 206e 6577 5f63 6f6d  .        new_com
-00017ce0: 706f 6e65 6e74 203d 2063 6f6d 706f 6e65  ponent = compone
-00017cf0: 6e74 2e63 6f70 7928 290a 2020 2020 2020  nt.copy().      
-00017d00: 2020 6e65 775f 636f 6d70 6f6e 656e 742e    new_component.
-00017d10: 6e61 6d65 203d 2063 6f6d 706f 6e65 6e74  name = component
-00017d20: 2e6e 616d 650a 2020 2020 2020 2020 2320  .name.        # 
-00017d30: 6d61 6b65 2073 7572 6520 616c 6c20 6d6f  make sure all mo
-00017d40: 6469 6669 6564 2063 656c 6c73 2068 6176  dified cells hav
-00017d50: 6520 7468 6569 7220 7265 6665 7265 6e63  e their referenc
-00017d60: 6573 2075 7064 6174 6564 0a20 2020 2020  es updated.     
-00017d70: 2020 206e 6577 5f72 6566 7320 3d20 6e65     new_refs = ne
-00017d80: 775f 636f 6d70 6f6e 656e 742e 7265 6665  w_component.refe
-00017d90: 7265 6e63 6573 2e63 6f70 7928 290a 2020  rences.copy().  
-00017da0: 2020 2020 2020 666f 7220 7265 6620 696e        for ref in
-00017db0: 206e 6577 5f72 6566 733a 0a20 2020 2020   new_refs:.     
-00017dc0: 2020 2020 2020 2069 6620 7265 662e 6e61         if ref.na
-00017dd0: 6d65 2069 6e20 696e 7661 6c69 645f 7265  me in invalid_re
-00017de0: 6673 3a0a 2020 2020 2020 2020 2020 2020  fs:.            
-00017df0: 2020 2020 6e65 775f 636f 6d70 6f6e 656e      new_componen
-00017e00: 742e 666c 6174 7465 6e5f 7265 6665 7265  t.flatten_refere
-00017e10: 6e63 6528 7265 6629 0a20 2020 2020 2020  nce(ref).       
-00017e20: 2020 2020 2065 6c69 6620 280a 2020 2020       elif (.    
-00017e30: 2020 2020 2020 2020 2020 2020 7265 662e              ref.
-00017e40: 7061 7265 6e74 2e6e 616d 6520 696e 2075  parent.name in u
-00017e50: 7064 6174 6564 5f63 6f6d 706f 6e65 6e74  pdated_component
-00017e60: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00017e70: 2020 616e 6420 7265 662e 7061 7265 6e74    and ref.parent
-00017e80: 2069 7320 6e6f 7420 7570 6461 7465 645f   is not updated_
-00017e90: 636f 6d70 6f6e 656e 7473 5b72 6566 2e70  components[ref.p
-00017ea0: 6172 656e 742e 6e61 6d65 5d0a 2020 2020  arent.name].    
-00017eb0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00017ec0: 2020 2020 2020 2020 2020 2072 6566 2e70             ref.p
-00017ed0: 6172 656e 7420 3d20 7570 6461 7465 645f  arent = updated_
-00017ee0: 636f 6d70 6f6e 656e 7473 5b72 6566 2e70  components[ref.p
-00017ef0: 6172 656e 742e 6e61 6d65 5d0a 2020 2020  arent.name].    
-00017f00: 2020 2020 636f 6d70 6f6e 656e 7420 3d20      component = 
-00017f10: 6e65 775f 636f 6d70 6f6e 656e 740a 2020  new_component.  
-00017f20: 2020 2020 2020 7570 6461 7465 645f 636f        updated_co
-00017f30: 6d70 6f6e 656e 7473 5b63 6f6d 706f 6e65  mponents[compone
-00017f40: 6e74 2e6e 616d 655d 203d 206e 6577 5f63  nt.name] = new_c
-00017f50: 6f6d 706f 6e65 6e74 0a20 2020 2074 7261  omponent.    tra
-00017f60: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
-00017f70: 732e 6164 6428 636f 6d70 6f6e 656e 742e  s.add(component.
-00017f80: 6e61 6d65 290a 2020 2020 7265 7475 726e  name).    return
-00017f90: 2063 6f6d 706f 6e65 6e74 0a0a 0a64 6566   component...def
-00017fa0: 205f 6368 6563 6b5f 756e 6361 6368 6564   _check_uncached
-00017fb0: 5f63 6f6d 706f 6e65 6e74 7328 636f 6d70  _components(comp
-00017fc0: 6f6e 656e 742c 206d 6f64 6529 3a0a 2020  onent, mode):.  
-00017fd0: 2020 7661 6c69 645f 6d6f 6465 7320 3d20    valid_modes = 
-00017fe0: 5b22 7761 726e 222c 2022 6572 726f 7222  ["warn", "error"
-00017ff0: 2c20 2269 676e 6f72 6522 5d0a 0a20 2020  , "ignore"]..   
-00018000: 2069 6620 6d6f 6465 203d 3d20 2269 676e   if mode == "ign
-00018010: 6f72 6522 3a0a 2020 2020 2020 2020 7265  ore":.        re
-00018020: 7475 726e 0a20 2020 2065 6c69 6620 6d6f  turn.    elif mo
-00018030: 6465 206e 6f74 2069 6e20 7661 6c69 645f  de not in valid_
-00018040: 6d6f 6465 733a 0a20 2020 2020 2020 2072  modes:.        r
-00018050: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00018060: 0a20 2020 2020 2020 2020 2020 2066 227b  .            f"{
-00018070: 6d6f 6465 7d20 6973 206e 6f74 2061 2076  mode} is not a v
-00018080: 616c 6964 2076 616c 7565 2066 6f72 206f  alid value for o
-00018090: 6e5f 756e 6361 6368 6564 5f63 6f6d 706f  n_uncached_compo
-000180a0: 6e65 6e74 2e20 5472 7920 6f6e 6520 6f66  nent. Try one of
-000180b0: 2074 6865 7365 3a20 7b76 616c 6964 5f6d   these: {valid_m
-000180c0: 6f64 6573 7d2e 220a 2020 2020 2020 2020  odes}.".        
-000180d0: 290a 0a20 2020 2066 6f72 2073 7562 5f63  )..    for sub_c
-000180e0: 6f6d 706f 6e65 6e74 2069 6e20 636f 6d70  omponent in comp
-000180f0: 6f6e 656e 742e 6765 745f 6465 7065 6e64  onent.get_depend
-00018100: 656e 6369 6573 2872 6563 7572 7369 7665  encies(recursive
-00018110: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-00018120: 6966 206e 6f74 2073 7562 5f63 6f6d 706f  if not sub_compo
-00018130: 6e65 6e74 2e5f 6c6f 636b 6564 3a0a 2020  nent._locked:.  
-00018140: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00018150: 6520 3d20 280a 2020 2020 2020 2020 2020  e = (.          
-00018160: 2020 2020 2020 6622 436f 6d70 6f6e 656e        f"Componen
-00018170: 7420 7b73 7562 5f63 6f6d 706f 6e65 6e74  t {sub_component
-00018180: 2e6e 616d 6521 727d 2077 6173 204e 4f54  .name!r} was NOT
-00018190: 2070 726f 7065 726c 7920 6c6f 636b 6564   properly locked
-000181a0: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-000181b0: 2020 2020 2259 6f75 206e 6565 6420 746f      "You need to
-000181c0: 2077 7269 7465 2069 7420 696e 746f 2061   write it into a
-000181d0: 2066 756e 6374 696f 6e20 7468 6174 2068   function that h
-000181e0: 6173 2074 6865 2040 6365 6c6c 2064 6563  as the @cell dec
-000181f0: 6f72 6174 6f72 2e22 0a20 2020 2020 2020  orator.".       
-00018200: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00018210: 2020 2069 6620 6d6f 6465 203d 3d20 2277     if mode == "w
-00018220: 6172 6e22 3a0a 2020 2020 2020 2020 2020  arn":.          
-00018230: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-00018240: 6172 6e28 6d65 7373 6167 652c 2055 6e63  arn(message, Unc
-00018250: 6163 6865 6443 6f6d 706f 6e65 6e74 5761  achedComponentWa
-00018260: 726e 696e 672c 2073 7461 636b 6c65 7665  rning, stackleve
-00018270: 6c3d 3329 0a0a 2020 2020 2020 2020 2020  l=3)..          
-00018280: 2020 656c 6966 206d 6f64 6520 3d3d 2022    elif mode == "
-00018290: 6572 726f 7222 3a0a 2020 2020 2020 2020  error":.        
-000182a0: 2020 2020 2020 2020 7261 6973 6520 556e          raise Un
-000182b0: 6361 6368 6564 436f 6d70 6f6e 656e 7445  cachedComponentE
-000182c0: 7272 6f72 286d 6573 7361 6765 290a 0a0a  rror(message)...
-000182d0: 6465 6620 7465 7374 5f73 616d 655f 7569  def test_same_ui
-000182e0: 6428 2920 2d3e 204e 6f6e 653a 0a20 2020  d() -> None:.   
-000182f0: 2069 6d70 6f72 7420 6764 7366 6163 746f   import gdsfacto
-00018300: 7279 2061 7320 6766 0a0a 2020 2020 6320  ry as gf..    c 
-00018310: 3d20 436f 6d70 6f6e 656e 7428 290a 2020  = Component().  
-00018320: 2020 6320 3c3c 2067 662e 636f 6d70 6f6e    c << gf.compon
-00018330: 656e 7473 2e72 6563 7461 6e67 6c65 2829  ents.rectangle()
-00018340: 0a20 2020 2063 203c 3c20 6766 2e63 6f6d  .    c << gf.com
-00018350: 706f 6e65 6e74 732e 7265 6374 616e 676c  ponents.rectangl
-00018360: 6528 290a 0a20 2020 2072 3120 3d20 632e  e()..    r1 = c.
-00018370: 7265 6665 7265 6e63 6573 5b30 5d2e 7061  references[0].pa
-00018380: 7265 6e74 0a20 2020 2072 3220 3d20 632e  rent.    r2 = c.
-00018390: 7265 6665 7265 6e63 6573 5b31 5d2e 7061  references[1].pa
-000183a0: 7265 6e74 0a0a 2020 2020 6173 7365 7274  rent..    assert
-000183b0: 2072 312e 7569 6420 3d3d 2072 322e 7569   r1.uid == r2.ui
-000183c0: 642c 2066 227b 7231 2e75 6964 7d20 6d75  d, f"{r1.uid} mu
-000183d0: 7374 2065 7175 616c 207b 7232 2e75 6964  st equal {r2.uid
-000183e0: 7d22 0a0a 0a64 6566 2074 6573 745f 6e65  }"...def test_ne
-000183f0: 746c 6973 745f 7369 6d70 6c65 2829 202d  tlist_simple() -
-00018400: 3e20 4e6f 6e65 3a0a 2020 2020 696d 706f  > None:.    impo
-00018410: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
-00018420: 2067 660a 0a20 2020 2063 203d 2067 662e   gf..    c = gf.
-00018430: 436f 6d70 6f6e 656e 7428 290a 2020 2020  Component().    
-00018440: 6331 203d 2063 203c 3c20 6766 2e63 6f6d  c1 = c << gf.com
-00018450: 706f 6e65 6e74 732e 7374 7261 6967 6874  ponents.straight
-00018460: 286c 656e 6774 683d 312c 2077 6964 7468  (length=1, width
-00018470: 3d32 290a 2020 2020 6332 203d 2063 203c  =2).    c2 = c <
-00018480: 3c20 6766 2e63 6f6d 706f 6e65 6e74 732e  < gf.components.
-00018490: 7374 7261 6967 6874 286c 656e 6774 683d  straight(length=
-000184a0: 322c 2077 6964 7468 3d32 290a 2020 2020  2, width=2).    
-000184b0: 6332 2e63 6f6e 6e65 6374 2870 6f72 743d  c2.connect(port=
-000184c0: 226f 3122 2c20 6465 7374 696e 6174 696f  "o1", destinatio
-000184d0: 6e3d 6331 2e70 6f72 7473 5b22 6f32 225d  n=c1.ports["o2"]
-000184e0: 290a 2020 2020 632e 6164 645f 706f 7274  ).    c.add_port
-000184f0: 2822 6f31 222c 2070 6f72 743d 6331 2e70  ("o1", port=c1.p
-00018500: 6f72 7473 5b22 6f31 225d 290a 2020 2020  orts["o1"]).    
-00018510: 632e 6164 645f 706f 7274 2822 6f32 222c  c.add_port("o2",
-00018520: 2070 6f72 743d 6332 2e70 6f72 7473 5b22   port=c2.ports["
-00018530: 6f32 225d 290a 2020 2020 6e65 746c 6973  o2"]).    netlis
-00018540: 7420 3d20 632e 6765 745f 6e65 746c 6973  t = c.get_netlis
-00018550: 7428 290a 2020 2020 2320 7072 696e 7428  t().    # print(
-00018560: 6e65 746c 6973 742e 7072 6574 7479 2829  netlist.pretty()
-00018570: 290a 2020 2020 6173 7365 7274 206c 656e  ).    assert len
-00018580: 286e 6574 6c69 7374 5b22 696e 7374 616e  (netlist["instan
-00018590: 6365 7322 5d29 203d 3d20 320a 0a0a 6465  ces"]) == 2...de
-000185a0: 6620 7465 7374 5f6e 6574 6c69 7374 5f73  f test_netlist_s
-000185b0: 696d 706c 655f 7769 6474 685f 6d69 736d  imple_width_mism
-000185c0: 6174 6368 5f74 6872 6f77 735f 6572 726f  atch_throws_erro
-000185d0: 7228 2920 2d3e 204e 6f6e 653a 0a20 2020  r() -> None:.   
-000185e0: 2069 6d70 6f72 7420 7079 7465 7374 0a0a   import pytest..
-000185f0: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
-00018600: 6374 6f72 7920 6173 2067 660a 0a20 2020  ctory as gf..   
-00018610: 2063 203d 2067 662e 436f 6d70 6f6e 656e   c = gf.Componen
-00018620: 7428 290a 2020 2020 6331 203d 2063 203c  t().    c1 = c <
-00018630: 3c20 6766 2e63 6f6d 706f 6e65 6e74 732e  < gf.components.
-00018640: 7374 7261 6967 6874 286c 656e 6774 683d  straight(length=
-00018650: 312c 2077 6964 7468 3d31 290a 2020 2020  1, width=1).    
-00018660: 6332 203d 2063 203c 3c20 6766 2e63 6f6d  c2 = c << gf.com
-00018670: 706f 6e65 6e74 732e 7374 7261 6967 6874  ponents.straight
-00018680: 286c 656e 6774 683d 322c 2077 6964 7468  (length=2, width
-00018690: 3d32 290a 2020 2020 6332 2e63 6f6e 6e65  =2).    c2.conne
-000186a0: 6374 2870 6f72 743d 226f 3122 2c20 6465  ct(port="o1", de
-000186b0: 7374 696e 6174 696f 6e3d 6331 2e70 6f72  stination=c1.por
-000186c0: 7473 5b22 6f32 225d 290a 2020 2020 632e  ts["o2"]).    c.
-000186d0: 6164 645f 706f 7274 2822 6f31 222c 2070  add_port("o1", p
-000186e0: 6f72 743d 6331 2e70 6f72 7473 5b22 6f31  ort=c1.ports["o1
-000186f0: 225d 290a 2020 2020 632e 6164 645f 706f  "]).    c.add_po
-00018700: 7274 2822 6f32 222c 2070 6f72 743d 6332  rt("o2", port=c2
-00018710: 2e70 6f72 7473 5b22 6f32 225d 290a 2020  .ports["o2"]).  
-00018720: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
-00018730: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
-00018740: 3a0a 2020 2020 2020 2020 632e 6765 745f  :.        c.get_
-00018750: 6e65 746c 6973 7428 290a 0a0a 6465 6620  netlist()...def 
-00018760: 7465 7374 5f6e 6574 6c69 7374 5f63 6f6d  test_netlist_com
-00018770: 706c 6578 2829 202d 3e20 4e6f 6e65 3a0a  plex() -> None:.
-00018780: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
-00018790: 6374 6f72 7920 6173 2067 660a 0a20 2020  ctory as gf..   
-000187a0: 2063 203d 2067 662e 636f 6d70 6f6e 656e   c = gf.componen
-000187b0: 7473 2e6d 7a69 5f61 726d 7328 290a 2020  ts.mzi_arms().  
-000187c0: 2020 6e65 746c 6973 7420 3d20 632e 6765    netlist = c.ge
-000187d0: 745f 6e65 746c 6973 7428 290a 2020 2020  t_netlist().    
-000187e0: 2320 7072 696e 7428 6e65 746c 6973 742e  # print(netlist.
-000187f0: 7072 6574 7479 2829 290a 2020 2020 6173  pretty()).    as
-00018800: 7365 7274 206c 656e 286e 6574 6c69 7374  sert len(netlist
-00018810: 5b22 696e 7374 616e 6365 7322 5d29 203d  ["instances"]) =
-00018820: 3d20 342c 206c 656e 286e 6574 6c69 7374  = 4, len(netlist
-00018830: 5b22 696e 7374 616e 6365 7322 5d29 0a0a  ["instances"])..
-00018840: 0a64 6566 2074 6573 745f 6578 7472 6163  .def test_extrac
-00018850: 7428 2920 2d3e 204e 6f6e 653a 0a20 2020  t() -> None:.   
-00018860: 2069 6d70 6f72 7420 6764 7366 6163 746f   import gdsfacto
-00018870: 7279 2061 7320 6766 0a0a 2020 2020 6320  ry as gf..    c 
-00018880: 3d20 6766 2e63 6f6d 706f 6e65 6e74 732e  = gf.components.
-00018890: 7374 7261 6967 6874 280a 2020 2020 2020  straight(.      
-000188a0: 2020 6c65 6e67 7468 3d31 302c 0a20 2020    length=10,.   
-000188b0: 2020 2020 2077 6964 7468 3d30 2e35 2c0a       width=0.5,.
-000188c0: 2020 2020 2020 2020 6262 6f78 5f6c 6179          bbox_lay
-000188d0: 6572 733d 5b67 662e 4c41 5945 522e 5747  ers=[gf.LAYER.WG
-000188e0: 434c 4144 5d2c 0a20 2020 2020 2020 2062  CLAD],.        b
-000188f0: 626f 785f 6f66 6673 6574 733d 5b33 5d2c  box_offsets=[3],
-00018900: 0a20 2020 2020 2020 2077 6974 685f 6262  .        with_bb
-00018910: 6f78 3d54 7275 652c 0a20 2020 2020 2020  ox=True,.       
-00018920: 2063 6c61 6464 696e 675f 6c61 7965 7273   cladding_layers
-00018930: 3d4e 6f6e 652c 0a20 2020 2020 2020 2061  =None,.        a
-00018940: 6464 5f70 696e 733d 4e6f 6e65 2c0a 2020  dd_pins=None,.  
-00018950: 2020 2020 2020 6164 645f 6262 6f78 3d4e        add_bbox=N
-00018960: 6f6e 652c 0a20 2020 2029 0a20 2020 2063  one,.    ).    c
-00018970: 3220 3d20 632e 6578 7472 6163 7428 6c61  2 = c.extract(la
-00018980: 7965 7273 3d5b 6766 2e4c 4159 4552 2e57  yers=[gf.LAYER.W
-00018990: 4743 4c41 445d 290a 0a20 2020 2061 7373  GCLAD])..    ass
-000189a0: 6572 7420 6c65 6e28 632e 706f 6c79 676f  ert len(c.polygo
-000189b0: 6e73 2920 3d3d 2032 2c20 6c65 6e28 632e  ns) == 2, len(c.
-000189c0: 706f 6c79 676f 6e73 290a 2020 2020 6173  polygons).    as
-000189d0: 7365 7274 206c 656e 2863 322e 706f 6c79  sert len(c2.poly
-000189e0: 676f 6e73 2920 3d3d 2031 2c20 6c65 6e28  gons) == 1, len(
-000189f0: 6332 2e70 6f6c 7967 6f6e 7329 0a20 2020  c2.polygons).   
-00018a00: 2061 7373 6572 7420 6766 2e4c 4159 4552   assert gf.LAYER
-00018a10: 2e57 4743 4c41 4420 696e 2063 322e 6c61  .WGCLAD in c2.la
-00018a20: 7965 7273 0a0a 0a64 6566 2068 6173 685f  yers...def hash_
-00018a30: 6669 6c65 2866 696c 6570 6174 6829 3a0a  file(filepath):.
-00018a40: 2020 2020 6d64 3520 3d20 6861 7368 6c69      md5 = hashli
-00018a50: 622e 6d64 3528 290a 2020 2020 6d64 352e  b.md5().    md5.
-00018a60: 7570 6461 7465 2866 696c 6570 6174 682e  update(filepath.
-00018a70: 7265 6164 5f62 7974 6573 2829 290a 2020  read_bytes()).  
-00018a80: 2020 7265 7475 726e 206d 6435 2e68 6578    return md5.hex
-00018a90: 6469 6765 7374 2829 0a0a 0a64 6566 2074  digest()...def t
-00018aa0: 6573 745f 6262 6f78 5f72 6566 6572 656e  est_bbox_referen
-00018ab0: 6365 2829 202d 3e20 4e6f 6e65 3a0a 2020  ce() -> None:.  
-00018ac0: 2020 696d 706f 7274 2067 6473 6661 6374    import gdsfact
-00018ad0: 6f72 7920 6173 2067 660a 0a20 2020 2063  ory as gf..    c
-00018ae0: 203d 2067 662e 436f 6d70 6f6e 656e 7428   = gf.Component(
-00018af0: 290a 2020 2020 6331 203d 2063 203c 3c20  ).    c1 = c << 
-00018b00: 6766 2e63 6f6d 706f 6e65 6e74 732e 7265  gf.components.re
-00018b10: 6374 616e 676c 6528 7369 7a65 3d28 312e  ctangle(size=(1.
-00018b20: 3565 2d33 2c20 312e 3565 2d33 292c 2070  5e-3, 1.5e-3), p
-00018b30: 6f72 745f 7479 7065 3d4e 6f6e 6529 0a20  ort_type=None). 
-00018b40: 2020 2063 3220 3d20 6320 3c3c 2067 662e     c2 = c << gf.
-00018b50: 636f 6d70 6f6e 656e 7473 2e72 6563 7461  components.recta
-00018b60: 6e67 6c65 2873 697a 653d 2831 2e35 652d  ngle(size=(1.5e-
-00018b70: 332c 2031 2e35 652d 3329 2c20 706f 7274  3, 1.5e-3), port
-00018b80: 5f74 7970 653d 4e6f 6e65 290a 2020 2020  _type=None).    
-00018b90: 6332 2e78 6d69 6e20 3d20 6331 2e78 6d61  c2.xmin = c1.xma
-00018ba0: 780a 0a20 2020 2061 7373 6572 7420 6332  x..    assert c2
-00018bb0: 2e78 7369 7a65 203d 3d20 312e 3565 2d33  .xsize == 1.5e-3
-00018bc0: 0a0a 0a64 6566 2074 6573 745f 7265 6d6f  ...def test_remo
-00018bd0: 7665 5f6c 6162 656c 7328 2920 2d3e 204e  ve_labels() -> N
-00018be0: 6f6e 653a 0a20 2020 2069 6d70 6f72 7420  one:.    import 
-00018bf0: 6764 7366 6163 746f 7279 2061 7320 6766  gdsfactory as gf
-00018c00: 0a0a 2020 2020 6320 3d20 6766 2e63 2e73  ..    c = gf.c.s
-00018c10: 7472 6169 6768 7428 290a 2020 2020 632e  traight().    c.
-00018c20: 7265 6d6f 7665 5f6c 6162 656c 7328 290a  remove_labels().
-00018c30: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
-00018c40: 632e 6c61 6265 6c73 2920 3d3d 2030 0a0a  c.labels) == 0..
-00018c50: 0a64 6566 2074 6573 745f 696d 706f 7274  .def test_import
-00018c60: 5f67 6473 5f73 6574 7469 6e67 7328 2920  _gds_settings() 
-00018c70: 2d3e 204e 6f6e 653a 0a20 2020 2069 6d70  -> None:.    imp
-00018c80: 6f72 7420 6764 7366 6163 746f 7279 2061  ort gdsfactory a
-00018c90: 7320 6766 0a0a 2020 2020 6320 3d20 6766  s gf..    c = gf
-00018ca0: 2e63 6f6d 706f 6e65 6e74 732e 6d7a 6928  .components.mzi(
-00018cb0: 290a 2020 2020 6764 7370 6174 6820 3d20  ).    gdspath = 
-00018cc0: 632e 7772 6974 655f 6764 7328 7769 7468  c.write_gds(with
-00018cd0: 5f6d 6574 6164 6174 613d 5472 7565 290a  _metadata=True).
-00018ce0: 2020 2020 6332 203d 2067 662e 696d 706f      c2 = gf.impo
-00018cf0: 7274 5f67 6473 2867 6473 7061 7468 2c20  rt_gds(gdspath, 
-00018d00: 6e61 6d65 3d22 6d7a 695f 7361 6d70 6c65  name="mzi_sample
-00018d10: 222c 2072 6561 645f 6d65 7461 6461 7461  ", read_metadata
-00018d20: 3d54 7275 6529 0a20 2020 2063 3320 3d20  =True).    c3 = 
-00018d30: 6766 2e72 6f75 7469 6e67 2e61 6464 5f66  gf.routing.add_f
-00018d40: 6962 6572 5f73 696e 676c 6528 6332 290a  iber_single(c2).
-00018d50: 2020 2020 6173 7365 7274 2063 330a 0a0a      assert c3...
-00018d60: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
-00018d70: 5f5f 6d61 696e 5f5f 223a 0a20 2020 2069  __main__":.    i
-00018d80: 6d70 6f72 7420 6764 7366 6163 746f 7279  mport gdsfactory
-00018d90: 2061 7320 6766 0a0a 2020 2020 6320 3d20   as gf..    c = 
-00018da0: 6766 2e63 2e6d 7a69 2829 0a20 2020 2063  gf.c.mzi().    c
-00018db0: 2e70 7072 696e 745f 706f 7274 7328 290a  .pprint_ports().
-00018dc0: 0a20 2020 2023 2063 203d 2067 662e 436f  .    # c = gf.Co
-00018dd0: 6d70 6f6e 656e 7428 290a 2020 2020 2320  mponent().    # 
-00018de0: 7020 3d20 632e 6164 645f 706f 6c79 676f  p = c.add_polygo
-00018df0: 6e28 0a20 2020 2023 2020 2020 205b 282d  n(.    #     [(-
-00018e00: 382c 2036 2c20 372c 2039 292c 2028 2d36  8, 6, 7, 9), (-6
-00018e10: 2c20 382c 2031 372c 2035 295d 2c20 6c61  , 8, 17, 5)], la
-00018e20: 7965 723d 2831 2c20 3029 0a20 2020 2023  yer=(1, 0).    #
-00018e30: 2029 2020 2320 4744 5320 6c61 7965 7273   )  # GDS layers
-00018e40: 2061 7265 2074 7570 6c65 7320 6f66 2069   are tuples of i
-00018e50: 6e74 7320 2862 7574 2069 6620 7765 2075  nts (but if we u
-00018e60: 7365 206f 6e6c 7920 6f6e 6520 6e75 6d62  se only one numb
-00018e70: 6572 2069 7420 6173 7375 6d65 7320 7468  er it assumes th
-00018e80: 6520 6f74 6865 7220 6e75 6d62 6572 2069  e other number i
-00018e90: 7320 3029 0a20 2020 2023 2063 2e77 7269  s 0).    # c.wri
-00018ea0: 7465 5f67 6473 2822 6869 2e67 6473 2229  te_gds("hi.gds")
-00018eb0: 0a20 2020 2023 2063 2e73 686f 7728 290a  .    # c.show().
-00018ec0: 2020 2020 2320 7072 696e 7428 434f 4e46      # print(CONF
-00018ed0: 2e6c 6173 745f 7361 7665 645f 6669 6c65  .last_saved_file
-00018ee0: 7329 0a                                  s).
+0000e9d0: 2020 2066 7261 6d65 5f77 6964 7468 3d35     frame_width=5
+0000e9e0: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+0000e9f0: 2020 2020 2020 2020 796c 696d 3d28 625b          ylim=(b[
+0000ea00: 315d 2c20 625b 335d 292c 0a20 2020 2020  1], b[3]),.     
+0000ea10: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0000ea20: 6c69 6d3d 2862 5b30 5d2c 2062 5b32 5d29  lim=(b[0], b[2])
+0000ea30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ea40: 2020 2020 2020 6669 6c6c 5f63 6f6c 6f72        fill_color
+0000ea50: 3d6c 6179 6572 5f76 6965 772e 6669 6c6c  =layer_view.fill
+0000ea60: 5f63 6f6c 6f72 2e61 735f 7267 6228 2920  _color.as_rgb() 
+0000ea70: 6f72 2022 222c 0a20 2020 2020 2020 2020  or "",.         
+0000ea80: 2020 2020 2020 2020 2020 206c 696e 655f             line_
+0000ea90: 636f 6c6f 723d 6c61 7965 725f 7669 6577  color=layer_view
+0000eaa0: 2e66 7261 6d65 5f63 6f6c 6f72 2e61 735f  .frame_color.as_
+0000eab0: 7267 6228 2920 6f72 2022 222c 0a20 2020  rgb() or "",.   
+0000eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ead0: 2066 696c 6c5f 616c 7068 613d 6c61 7965   fill_alpha=laye
+0000eae0: 725f 7669 6577 2e67 6574 5f61 6c70 6861  r_view.get_alpha
+0000eaf0: 2829 206f 7220 2222 2c0a 2020 2020 2020  () or "",.      
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000eb10: 6e65 5f61 6c70 6861 3d6c 6179 6572 5f76  ne_alpha=layer_v
+0000eb20: 6965 772e 6765 745f 616c 7068 6128 2920  iew.get_alpha() 
+0000eb30: 6f72 2022 222c 0a20 2020 2020 2020 2020  or "",.         
+0000eb40: 2020 2020 2020 2020 2020 2074 6f6f 6c73             tools
+0000eb50: 3d5b 2268 6f76 6572 225d 2c0a 2020 2020  =["hover"],.    
+0000eb60: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000eb70: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000eb80: 2020 2020 666f 7220 6e61 6d65 2c20 706f      for name, po
+0000eb90: 7274 2069 6e20 7365 6c66 2e70 6f72 7473  rt in self.ports
+0000eba0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+0000ebb0: 2020 2020 2020 6e61 6d65 203d 2073 7472        name = str
+0000ebc0: 286e 616d 6529 0a20 2020 2020 2020 2020  (name).         
+0000ebd0: 2020 2070 6f6c 7967 6f6e 2c20 7074 6970     polygon, ptip
+0000ebe0: 203d 2067 6574 5f70 696e 5f74 7269 616e   = get_pin_trian
+0000ebf0: 676c 655f 706f 6c79 676f 6e5f 7469 7028  gle_polygon_tip(
+0000ec00: 706f 7274 3d70 6f72 7429 0a0a 2020 2020  port=port)..    
+0000ec10: 2020 2020 2020 2020 706c 6f74 735f 746f          plots_to
+0000ec20: 5f6f 7665 726c 6179 2e61 7070 656e 6428  _overlay.append(
+0000ec30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ec40: 2068 762e 506f 6c79 676f 6e73 2870 6f6c   hv.Polygons(pol
+0000ec50: 7967 6f6e 2c20 6c61 6265 6c3d 6e61 6d65  ygon, label=name
+0000ec60: 292e 6f70 7473 280a 2020 2020 2020 2020  ).opts(.        
+0000ec70: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000ec80: 5f61 7370 6563 743d 312c 0a20 2020 2020  _aspect=1,.     
+0000ec90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000eca0: 7261 6d65 5f77 6964 7468 3d35 3030 2c0a  rame_width=500,.
+0000ecb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecc0: 2020 2020 6669 6c6c 5f61 6c70 6861 3d30      fill_alpha=0
+0000ecd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ece0: 2020 2020 2020 796c 696d 3d28 625b 315d        ylim=(b[1]
+0000ecf0: 2c20 625b 335d 292c 0a20 2020 2020 2020  , b[3]),.       
+0000ed00: 2020 2020 2020 2020 2020 2020 2078 6c69               xli
+0000ed10: 6d3d 2862 5b30 5d2c 2062 5b32 5d29 2c0a  m=(b[0], b[2]),.
+0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed30: 2020 2020 636f 6c6f 723d 2272 6564 222c      color="red",
+0000ed40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ed50: 2020 2020 206c 696e 655f 616c 7068 613d       line_alpha=
+0000ed60: 6c61 7965 725f 7669 6577 2e67 6574 5f61  layer_view.get_a
+0000ed70: 6c70 6861 2829 206f 7220 2222 2c0a 2020  lpha() or "",.  
+0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed90: 2020 746f 6f6c 733d 5b22 686f 7665 7222    tools=["hover"
+0000eda0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000edb0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000edc0: 2020 2020 202a 2068 762e 5465 7874 2870       * hv.Text(p
+0000edd0: 7469 705b 305d 2c20 7074 6970 5b31 5d2c  tip[0], ptip[1],
+0000ede0: 206e 616d 6529 0a20 2020 2020 2020 2020   name).         
+0000edf0: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
+0000ee00: 7475 726e 2068 762e 4f76 6572 6c61 7928  turn hv.Overlay(
+0000ee10: 706c 6f74 735f 746f 5f6f 7665 726c 6179  plots_to_overlay
+0000ee20: 292e 6f70 7473 280a 2020 2020 2020 2020  ).opts(.        
+0000ee30: 2020 2020 7368 6f77 5f6c 6567 656e 643d      show_legend=
+0000ee40: 5472 7565 2c20 7368 6172 6564 5f61 7865  True, shared_axe
+0000ee50: 733d 4661 6c73 652c 2079 6c69 6d3d 2862  s=False, ylim=(b
+0000ee60: 5b31 5d2c 2062 5b33 5d29 2c20 786c 696d  [1], b[3]), xlim
+0000ee70: 3d28 625b 305d 2c20 625b 325d 290a 2020  =(b[0], b[2]).  
+0000ee80: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000ee90: 2073 686f 7728 0a20 2020 2020 2020 2073   show(.        s
+0000eea0: 656c 662c 0a20 2020 2020 2020 2073 686f  elf,.        sho
+0000eeb0: 775f 706f 7274 733a 2062 6f6f 6c20 3d20  w_ports: bool = 
+0000eec0: 4661 6c73 652c 0a20 2020 2020 2020 2073  False,.        s
+0000eed0: 686f 775f 7375 6270 6f72 7473 3a20 626f  how_subports: bo
+0000eee0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+0000eef0: 2020 2020 706f 7274 5f6d 6172 6b65 725f      port_marker_
+0000ef00: 6c61 7965 723a 204c 6179 6572 203d 2028  layer: Layer = (
+0000ef10: 312c 2031 3029 2c0a 2020 2020 2020 2020  1, 10),.        
+0000ef20: 2a2a 6b77 6172 6773 2c0a 2020 2020 2920  **kwargs,.    ) 
+0000ef30: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000ef40: 2022 2222 5368 6f77 2063 6f6d 706f 6e65   """Show compone
+0000ef50: 6e74 2069 6e20 4b4c 6179 6f75 742e 0a0a  nt in KLayout...
+0000ef60: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
+0000ef70: 6120 636f 7079 206f 6620 7468 6520 436f  a copy of the Co
+0000ef80: 6d70 6f6e 656e 742c 2073 6f20 7468 6520  mponent, so the 
+0000ef90: 6f72 6967 696e 616c 2063 6f6d 706f 6e65  original compone
+0000efa0: 6e74 2072 656d 6169 6e73 2069 6e74 6163  nt remains intac
+0000efb0: 742e 0a20 2020 2020 2020 2077 6974 6820  t..        with 
+0000efc0: 7069 6e73 206d 6172 6b65 7273 206f 6e20  pins markers on 
+0000efd0: 6561 6368 2070 6f72 7420 7368 6f77 5f70  each port show_p
+0000efe0: 6f72 7473 203d 2054 7275 652c 2061 6e64  orts = True, and
+0000eff0: 206f 7074 696f 6e61 6c6c 7920 616c 736f   optionally also
+0000f000: 0a20 2020 2020 2020 2074 6865 2070 6f72  .        the por
+0000f010: 7473 2066 726f 6d20 7468 6520 7265 6665  ts from the refe
+0000f020: 7265 6e63 6573 2028 7368 6f77 5f73 7562  rences (show_sub
+0000f030: 706f 7274 733d 5472 7565 290a 0a20 2020  ports=True)..   
+0000f040: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000f050: 2020 2020 2020 2073 686f 775f 706f 7274         show_port
+0000f060: 733a 2073 686f 7773 2063 6f6d 706f 6e65  s: shows compone
+0000f070: 6e74 2077 6974 6820 706f 7274 206d 6172  nt with port mar
+0000f080: 6b65 7273 2061 6e64 206c 6162 656c 732e  kers and labels.
+0000f090: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
+0000f0a0: 775f 7375 6270 6f72 7473 3a20 6164 6420  w_subports: add 
+0000f0b0: 706f 7274 7320 6d61 726b 6572 7320 616e  ports markers an
+0000f0c0: 6420 6c61 6265 6c73 2074 6f20 7265 6665  d labels to refe
+0000f0d0: 7265 6e63 6573 2e0a 2020 2020 2020 2020  rences..        
+0000f0e0: 2020 2020 706f 7274 5f6d 6172 6b65 725f      port_marker_
+0000f0f0: 6c61 7965 723a 2066 6f72 2074 6865 2070  layer: for the p
+0000f100: 6f72 7473 2e0a 0a20 2020 2020 2020 204b  orts...        K
+0000f110: 6579 776f 7264 2041 7267 733a 0a20 2020  eyword Args:.   
+0000f120: 2020 2020 2020 2020 2067 6473 7061 7468           gdspath
+0000f130: 3a20 4744 5320 6669 6c65 2070 6174 6820  : GDS file path 
+0000f140: 746f 2077 7269 7465 2074 6f2e 0a20 2020  to write to..   
+0000f150: 2020 2020 2020 2020 2067 6473 6469 723a           gdsdir:
+0000f160: 2064 6972 6563 746f 7279 2066 6f72 2074   directory for t
+0000f170: 6865 2047 4453 2066 696c 652e 2044 6566  he GDS file. Def
+0000f180: 6175 6c74 7320 746f 202f 746d 702f 2e0a  aults to /tmp/..
+0000f190: 2020 2020 2020 2020 2020 2020 756e 6974              unit
+0000f1a0: 3a20 756e 6974 2073 697a 6520 666f 7220  : unit size for 
+0000f1b0: 6f62 6a65 6374 7320 696e 206c 6962 7261  objects in libra
+0000f1c0: 7279 2e20 3175 6d20 6279 2064 6566 6175  ry. 1um by defau
+0000f1d0: 6c74 2e0a 2020 2020 2020 2020 2020 2020  lt..            
+0000f1e0: 7072 6563 6973 696f 6e3a 2066 6f72 206f  precision: for o
+0000f1f0: 626a 6563 7420 6469 6d65 6e73 696f 6e73  bject dimensions
+0000f200: 2069 6e20 7468 6520 6c69 6272 6172 7920   in the library 
+0000f210: 286d 292e 2031 6e6d 2062 7920 6465 6661  (m). 1nm by defa
+0000f220: 756c 742e 0a20 2020 2020 2020 2020 2020  ult..           
+0000f230: 2074 696d 6573 7461 6d70 3a20 4465 6661   timestamp: Defa
+0000f240: 756c 7473 2074 6f20 3230 3139 2d31 302d  ults to 2019-10-
+0000f250: 3235 2e20 4966 204e 6f6e 6520 7573 6573  25. If None uses
+0000f260: 2063 7572 7265 6e74 2074 696d 652e 0a20   current time.. 
+0000f270: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000f280: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
+0000f290: 7279 2e61 6464 5f70 696e 7320 696d 706f  ry.add_pins impo
+0000f2a0: 7274 2061 6464 5f70 696e 735f 7472 6961  rt add_pins_tria
+0000f2b0: 6e67 6c65 0a20 2020 2020 2020 2066 726f  ngle.        fro
+0000f2c0: 6d20 6764 7366 6163 746f 7279 2e73 686f  m gdsfactory.sho
+0000f2d0: 7720 696d 706f 7274 2073 686f 770a 0a20  w import show.. 
+0000f2e0: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
+0000f2f0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+0000f300: 2073 656c 662e 6164 645f 7069 6e73 5f74   self.add_pins_t
+0000f310: 7269 616e 676c 6528 0a20 2020 2020 2020  riangle(.       
+0000f320: 2020 2020 2020 2020 2070 6f72 745f 6d61           port_ma
+0000f330: 726b 6572 5f6c 6179 6572 3d70 6f72 745f  rker_layer=port_
+0000f340: 6d61 726b 6572 5f6c 6179 6572 2c20 6c61  marker_layer, la
+0000f350: 7965 725f 6c61 6265 6c3d 706f 7274 5f6d  yer_label=port_m
+0000f360: 6172 6b65 725f 6c61 7965 720a 2020 2020  arker_layer.    
+0000f370: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000f380: 2020 2020 2020 6966 2073 686f 775f 706f        if show_po
+0000f390: 7274 730a 2020 2020 2020 2020 2020 2020  rts.            
+0000f3a0: 656c 7365 2073 656c 660a 2020 2020 2020  else self.      
+0000f3b0: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+0000f3c0: 7368 6f77 5f73 7562 706f 7274 733a 0a20  show_subports:. 
+0000f3d0: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
+0000f3e0: 6e65 6e74 203d 2073 656c 662e 636f 7079  nent = self.copy
+0000f3f0: 2829 0a20 2020 2020 2020 2020 2020 2063  ().            c
+0000f400: 6f6d 706f 6e65 6e74 2e6e 616d 6520 3d20  omponent.name = 
+0000f410: 7365 6c66 2e6e 616d 650a 2020 2020 2020  self.name.      
+0000f420: 2020 2020 2020 666f 7220 7265 6665 7265        for refere
+0000f430: 6e63 6520 696e 2063 6f6d 706f 6e65 6e74  nce in component
+0000f440: 2e72 6566 6572 656e 6365 733a 0a20 2020  .references:.   
+0000f450: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000f460: 6973 696e 7374 616e 6365 2863 6f6d 706f  isinstance(compo
+0000f470: 6e65 6e74 2c20 436f 6d70 6f6e 656e 7452  nent, ComponentR
+0000f480: 6566 6572 656e 6365 293a 0a20 2020 2020  eference):.     
+0000f490: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000f4a0: 6464 5f70 696e 735f 7472 6961 6e67 6c65  dd_pins_triangle
+0000f4b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000f4c0: 2020 2020 2020 2020 2020 636f 6d70 6f6e            compon
+0000f4d0: 656e 743d 636f 6d70 6f6e 656e 742c 0a20  ent=component,. 
+0000f4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4f0: 2020 2020 2020 2072 6566 6572 656e 6365         reference
+0000f500: 3d72 6566 6572 656e 6365 2c0a 2020 2020  =reference,.    
+0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f520: 2020 2020 6c61 7965 723d 706f 7274 5f6d      layer=port_m
+0000f530: 6172 6b65 725f 6c61 7965 722c 0a20 2020  arker_layer,.   
+0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f550: 2020 2020 206c 6179 6572 5f6c 6162 656c       layer_label
+0000f560: 3d70 6f72 745f 6d61 726b 6572 5f6c 6179  =port_marker_lay
+0000f570: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0000f580: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000f590: 2020 2073 686f 7728 636f 6d70 6f6e 656e     show(componen
+0000f5a0: 742c 202a 2a6b 7761 7267 7329 0a0a 2020  t, **kwargs)..  
+0000f5b0: 2020 6465 6620 5f77 7269 7465 5f6c 6962    def _write_lib
+0000f5c0: 7261 7279 280a 2020 2020 2020 2020 7365  rary(.        se
+0000f5d0: 6c66 2c0a 2020 2020 2020 2020 6764 7370  lf,.        gdsp
+0000f5e0: 6174 683a 2050 6174 6854 7970 6520 7c20  ath: PathType | 
+0000f5f0: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
+0000f600: 2020 2020 2067 6473 6469 723a 2050 6174       gdsdir: Pat
+0000f610: 6854 7970 6520 7c20 4e6f 6e65 203d 204e  hType | None = N
+0000f620: 6f6e 652c 0a20 2020 2020 2020 2074 696d  one,.        tim
+0000f630: 6573 7461 6d70 3a20 6461 7465 7469 6d65  estamp: datetime
+0000f640: 2e64 6174 6574 696d 6520 7c20 4e6f 6e65  .datetime | None
+0000f650: 203d 205f 7469 6d65 7374 616d 7032 3031   = _timestamp201
+0000f660: 392c 0a20 2020 2020 2020 206c 6f67 6769  9,.        loggi
+0000f670: 6e67 3a20 626f 6f6c 203d 2054 7275 652c  ng: bool = True,
+0000f680: 0a20 2020 2020 2020 2077 6974 685f 6f61  .        with_oa
+0000f690: 7369 733a 2062 6f6f 6c20 3d20 4661 6c73  sis: bool = Fals
+0000f6a0: 652c 0a20 2020 2020 2020 2077 6974 685f  e,.        with_
+0000f6b0: 6d65 7461 6461 7461 3a20 626f 6f6c 203d  metadata: bool =
+0000f6c0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+0000f6d0: 2a2a 6b77 6172 6773 2c0a 2020 2020 2920  **kwargs,.    ) 
+0000f6e0: 2d3e 2050 6174 683a 0a20 2020 2020 2020  -> Path:.       
+0000f6f0: 2022 2222 5772 6974 6520 636f 6d70 6f6e   """Write compon
+0000f700: 656e 7420 746f 2047 4453 206f 7220 4f41  ent to GDS or OA
+0000f710: 5349 5320 616e 6420 7265 7475 726e 7320  SIS and returns 
+0000f720: 6764 7370 6174 682e 0a0a 2020 2020 2020  gdspath...      
+0000f730: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000f740: 2020 2020 6764 7370 6174 683a 2047 4453      gdspath: GDS
+0000f750: 2066 696c 6520 7061 7468 2074 6f20 7772   file path to wr
+0000f760: 6974 6520 746f 2e0a 2020 2020 2020 2020  ite to..        
+0000f770: 2020 2020 6764 7364 6972 3a20 6469 7265      gdsdir: dire
+0000f780: 6374 6f72 7920 666f 7220 7468 6520 4744  ctory for the GD
+0000f790: 5320 6669 6c65 2e20 4465 6661 756c 7473  S file. Defaults
+0000f7a0: 2074 6f20 2f74 6d70 2f72 616e 646f 6d46   to /tmp/randomF
+0000f7b0: 696c 652f 6764 7366 6163 746f 7279 2e0a  ile/gdsfactory..
+0000f7c0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000f7d0: 7374 616d 703a 2044 6566 6175 6c74 7320  stamp: Defaults 
+0000f7e0: 746f 2032 3031 392d 3130 2d32 3520 666f  to 2019-10-25 fo
+0000f7f0: 7220 636f 6e73 6973 7465 6e74 2068 6173  r consistent has
+0000f800: 682e 0a20 2020 2020 2020 2020 2020 2020  h..             
+0000f810: 2020 2049 6620 4e6f 6e65 2075 7365 7320     If None uses 
+0000f820: 6375 7272 656e 7420 7469 6d65 2e0a 2020  current time..  
+0000f830: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
+0000f840: 673a 2064 6973 6162 6c65 2047 4453 2070  g: disable GDS p
+0000f850: 6174 6820 6c6f 6767 696e 672c 2066 6f72  ath logging, for
+0000f860: 2065 7861 6d70 6c65 2066 6f72 2073 686f   example for sho
+0000f870: 7769 6e67 2069 7420 696e 204b 4c61 796f  wing it in KLayo
+0000f880: 7574 2e0a 2020 2020 2020 2020 2020 2020  ut..            
+0000f890: 7769 7468 5f6f 6173 6973 3a20 4966 2054  with_oasis: If T
+0000f8a0: 7275 652c 2066 696c 6520 7769 6c6c 2062  rue, file will b
+0000f8b0: 6520 7772 6974 7465 6e20 746f 204f 4153  e written to OAS
+0000f8c0: 4953 2e20 4f74 6865 7277 6973 652c 2066  IS. Otherwise, f
+0000f8d0: 696c 6520 7769 6c6c 2062 6520 7772 6974  ile will be writ
+0000f8e0: 7465 6e20 746f 2047 4453 2e0a 2020 2020  ten to GDS..    
+0000f8f0: 2020 2020 2020 2020 7769 7468 5f6d 6574          with_met
+0000f900: 6164 6174 613a 2077 7269 7465 7320 6d65  adata: writes me
+0000f910: 7461 6461 7461 2069 6e20 5941 4d4c 2066  tadata in YAML f
+0000f920: 6f72 6d61 742e 0a0a 2020 2020 2020 2020  ormat...        
+0000f930: 4b65 7977 6f72 6420 4172 6773 3a0a 2020  Keyword Args:.  
+0000f940: 2020 2020 2020 2020 2020 4b65 7977 6f72            Keywor
+0000f950: 6420 6172 6775 6d65 6e74 7320 7769 6c6c  d arguments will
+0000f960: 206f 7665 7272 6964 6520 7468 6520 6163   override the ac
+0000f970: 7469 7665 2050 444b 2773 2064 6566 6175  tive PDK's defau
+0000f980: 6c74 2047 6473 5772 6974 6553 6574 7469  lt GdsWriteSetti
+0000f990: 6e67 7320 616e 6420 4f61 7369 7357 7269  ngs and OasisWri
+0000f9a0: 7465 5365 7474 696e 6773 2e0a 0a20 2020  teSettings...   
+0000f9b0: 2020 2020 2020 2020 2047 6473 2073 6574           Gds set
+0000f9c0: 7469 6e67 733a 0a20 2020 2020 2020 2020  tings:.         
+0000f9d0: 2020 2020 2020 2075 6e69 743a 2075 6e69         unit: uni
+0000f9e0: 7420 7369 7a65 2066 6f72 206f 626a 6563  t size for objec
+0000f9f0: 7473 2069 6e20 6c69 6272 6172 792e 2031  ts in library. 1
+0000fa00: 756d 2062 7920 6465 6661 756c 742e 0a20  um by default.. 
+0000fa10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000fa20: 7265 6369 7369 6f6e 3a20 666f 7220 6469  recision: for di
+0000fa30: 6d65 6e73 696f 6e73 2069 6e20 7468 6520  mensions in the 
+0000fa40: 6c69 6272 6172 7920 286d 292e 2031 6e6d  library (m). 1nm
+0000fa50: 2062 7920 6465 6661 756c 742e 0a20 2020   by default..   
+0000fa60: 2020 2020 2020 2020 2020 2020 206f 6e5f               on_
+0000fa70: 6475 706c 6963 6174 655f 6365 6c6c 3a20  duplicate_cell: 
+0000fa80: 7370 6563 6966 7920 686f 7720 746f 2072  specify how to r
+0000fa90: 6573 6f6c 7665 2064 7570 6c69 6361 7465  esolve duplicate
+0000faa0: 2d6e 616d 6564 2063 656c 6c73 2e20 4368  -named cells. Ch
+0000fab0: 6f6f 7365 206f 6e65 206f 6620 7468 6520  oose one of the 
+0000fac0: 666f 6c6c 6f77 696e 673a 0a20 2020 2020  following:.     
+0000fad0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000fae0: 7761 726e 2220 2864 6566 6175 6c74 293a  warn" (default):
+0000faf0: 206f 7665 7277 7269 7465 2061 6c6c 2064   overwrite all d
+0000fb00: 7570 6c69 6361 7465 2063 656c 6c73 2077  uplicate cells w
+0000fb10: 6974 6820 6f6e 6520 6f66 2074 6865 2064  ith one of the d
+0000fb20: 7570 6c69 6361 7465 7320 2861 7262 6974  uplicates (arbit
+0000fb30: 7261 7269 6c79 292e 0a20 2020 2020 2020  rarily)..       
+0000fb40: 2020 2020 2020 2020 2020 2020 2022 6572               "er
+0000fb50: 726f 7222 3a20 7468 726f 7720 6120 5661  ror": throw a Va
+0000fb60: 6c75 6545 7272 6f72 2077 6865 6e20 6174  lueError when at
+0000fb70: 7465 6d70 7469 6e67 2074 6f20 7772 6974  tempting to writ
+0000fb80: 6520 6120 6764 7320 7769 7468 2064 7570  e a gds with dup
+0000fb90: 6c69 6361 7465 2063 656c 6c73 2e0a 2020  licate cells..  
+0000fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbb0: 2020 226f 7665 7277 7269 7465 223a 206f    "overwrite": o
+0000fbc0: 7665 7277 7269 7465 2061 6c6c 2064 7570  verwrite all dup
+0000fbd0: 6c69 6361 7465 2063 656c 6c73 2077 6974  licate cells wit
+0000fbe0: 6820 6f6e 6520 6f66 2074 6865 2064 7570  h one of the dup
+0000fbf0: 6c69 6361 7465 732c 2077 6974 686f 7574  licates, without
+0000fc00: 2077 6172 6e69 6e67 2e0a 2020 2020 2020   warning..      
+0000fc10: 2020 2020 2020 2020 2020 2020 2020 4e6f                No
+0000fc20: 6e65 3a20 646f 206e 6f74 2074 7279 2074  ne: do not try t
+0000fc30: 6f20 7265 736f 6c76 6520 2861 7420 796f  o resolve (at yo
+0000fc40: 7572 206f 776e 2072 6973 6b21 290a 2020  ur own risk!).  
+0000fc50: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+0000fc60: 6174 7465 6e5f 696e 7661 6c69 645f 7265  atten_invalid_re
+0000fc70: 6673 3a20 666c 6174 7465 6e73 2063 6f6d  fs: flattens com
+0000fc80: 706f 6e65 6e74 2072 6566 6572 656e 6365  ponent reference
+0000fc90: 7320 7768 6963 6820 6861 7665 2069 6e76  s which have inv
+0000fca0: 616c 6964 2074 7261 6e73 666f 726d 6174  alid transformat
+0000fcb0: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
+0000fcc0: 2020 2020 2020 6d61 785f 706f 696e 7473        max_points
+0000fcd0: 3a20 4d61 7869 6d61 6c20 6e75 6d62 6572  : Maximal number
+0000fce0: 206f 6620 7665 7274 6963 6573 2070 6572   of vertices per
+0000fcf0: 2070 6f6c 7967 6f6e 2e20 506f 6c79 676f   polygon. Polygo
+0000fd00: 6e73 2077 6974 6820 6d6f 7265 2076 6572  ns with more ver
+0000fd10: 7469 6365 7320 7468 6174 2074 6869 7320  tices that this 
+0000fd20: 6172 6520 6175 746f 6d61 7469 6361 6c6c  are automaticall
+0000fd30: 7920 6672 6163 7475 7265 642e 0a0a 2020  y fractured...  
+0000fd40: 2020 2020 2020 2020 2020 4f61 7369 7320            Oasis 
+0000fd50: 7365 7474 696e 6773 3a0a 2020 2020 2020  settings:.      
+0000fd60: 2020 2020 2020 2020 2020 636f 6d70 7265            compre
+0000fd70: 7373 696f 6e5f 6c65 7665 6c3a 204c 6576  ssion_level: Lev
+0000fd80: 656c 206f 6620 636f 6d70 7265 7373 696f  el of compressio
+0000fd90: 6e20 666f 7220 6365 6c6c 7320 2862 6574  n for cells (bet
+0000fda0: 7765 656e 2030 2061 6e64 2039 292e 0a20  ween 0 and 9).. 
+0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdc0: 2020 2053 6574 7469 6e67 2074 6f20 3020     Setting to 0 
+0000fdd0: 7769 6c6c 2064 6973 6162 6c65 2063 656c  will disable cel
+0000fde0: 6c20 636f 6d70 7265 7373 696f 6e2c 2031  l compression, 1
+0000fdf0: 2067 6976 6573 2074 6865 2062 6573 7420   gives the best 
+0000fe00: 7370 6565 6420 616e 6420 392c 2074 6865  speed and 9, the
+0000fe10: 2062 6573 7420 636f 6d70 7265 7373 696f   best compressio
+0000fe20: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
+0000fe30: 2020 2064 6574 6563 745f 7265 6374 616e     detect_rectan
+0000fe40: 676c 6573 3a20 5374 6f72 6520 7265 6374  gles: Store rect
+0000fe50: 616e 676c 6573 2069 6e20 636f 6d70 7265  angles in compre
+0000fe60: 7373 6564 2066 6f72 6d61 742e 0a20 2020  ssed format..   
+0000fe70: 2020 2020 2020 2020 2020 2020 2064 6574               det
+0000fe80: 6563 745f 7472 6170 657a 6f69 6473 3a20  ect_trapezoids: 
+0000fe90: 5374 6f72 6520 7472 6170 657a 6f69 6473  Store trapezoids
+0000fea0: 2069 6e20 636f 6d70 7265 7373 6564 2066   in compressed f
+0000feb0: 6f72 6d61 742e 0a20 2020 2020 2020 2020  ormat..         
+0000fec0: 2020 2020 2020 2063 6972 636c 655f 746f         circle_to
+0000fed0: 6c65 7261 6e63 653a 2054 6f6c 6572 616e  lerance: Toleran
+0000fee0: 6365 2066 6f72 2064 6574 6563 7469 6e67  ce for detecting
+0000fef0: 2063 6972 636c 6573 2e20 4966 206c 6573   circles. If les
+0000ff00: 7320 6f72 2065 7175 616c 2074 6f20 302c  s or equal to 0,
+0000ff10: 206e 6f20 6465 7465 6374 696f 6e20 6973   no detection is
+0000ff20: 2070 6572 666f 726d 6564 2e20 4369 7263   performed. Circ
+0000ff30: 6c65 7320 6172 6520 7374 6f72 6564 2069  les are stored i
+0000ff40: 6e20 636f 6d70 7265 7373 6564 2066 6f72  n compressed for
+0000ff50: 6d61 742e 0a20 2020 2020 2020 2020 2020  mat..           
+0000ff60: 2020 2020 2076 616c 6964 6174 696f 6e20       validation 
+0000ff70: 2822 6372 6333 3222 2c20 2263 6865 636b  ("crc32", "check
+0000ff80: 7375 6d33 3222 2c20 4e6f 6e65 293a 2074  sum32", None): t
+0000ff90: 7970 6520 6f66 2076 616c 6964 6174 696f  ype of validatio
+0000ffa0: 6e20 746f 2069 6e63 6c75 6465 2069 6e20  n to include in 
+0000ffb0: 7468 6520 7361 7665 6420 6669 6c65 2e0a  the saved file..
+0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffd0: 7374 616e 6461 7264 5f70 726f 7065 7274  standard_propert
+0000ffe0: 6965 733a 2053 746f 7265 2073 7461 6e64  ies: Store stand
+0000fff0: 6172 6420 4f41 5349 5320 7072 6f70 6572  ard OASIS proper
+00010000: 7469 6573 2069 6e20 7468 6520 6669 6c65  ties in the file
+00010010: 2e0a 0a20 2020 2020 2020 2022 2222 0a0a  ...        """..
+00010020: 2020 2020 2020 2020 6672 6f6d 2067 6473          from gds
+00010030: 6661 6374 6f72 792e 7064 6b20 696d 706f  factory.pdk impo
+00010040: 7274 2067 6574 5f61 6374 6976 655f 7064  rt get_active_pd
+00010050: 6b0a 0a20 2020 2020 2020 2069 6620 6764  k..        if gd
+00010060: 7370 6174 6820 616e 6420 6764 7364 6972  spath and gdsdir
+00010070: 3a0a 2020 2020 2020 2020 2020 2020 7761  :.            wa
+00010080: 726e 696e 6773 2e77 6172 6e28 0a20 2020  rnings.warn(.   
+00010090: 2020 2020 2020 2020 2020 2020 2022 6764               "gd
+000100a0: 7370 6174 6820 616e 6420 6764 7364 6972  spath and gdsdir
+000100b0: 2068 6176 6520 626f 7468 2062 6565 6e20   have both been 
+000100c0: 7370 6563 6966 6965 642e 2067 6473 7061  specified. gdspa
+000100d0: 7468 2077 696c 6c20 7461 6b65 2070 7265  th will take pre
+000100e0: 6365 6465 6e63 6520 616e 6420 6764 7364  cedence and gdsd
+000100f0: 6972 2077 696c 6c20 6265 2069 676e 6f72  ir will be ignor
+00010100: 6564 2e22 2c0a 2020 2020 2020 2020 2020  ed.",.          
+00010110: 2020 2020 2020 7374 6163 6b6c 6576 656c        stacklevel
+00010120: 3d33 2c0a 2020 2020 2020 2020 2020 2020  =3,.            
+00010130: 290a 0a20 2020 2020 2020 2064 6566 6175  )..        defau
+00010140: 6c74 5f73 6574 7469 6e67 7320 3d20 6765  lt_settings = ge
+00010150: 745f 6163 7469 7665 5f70 646b 2829 2e67  t_active_pdk().g
+00010160: 6473 5f77 7269 7465 5f73 6574 7469 6e67  ds_write_setting
+00010170: 730a 2020 2020 2020 2020 6465 6661 756c  s.        defaul
+00010180: 745f 6f61 7369 735f 7365 7474 696e 6773  t_oasis_settings
+00010190: 203d 2067 6574 5f61 6374 6976 655f 7064   = get_active_pd
+000101a0: 6b28 292e 6f61 7369 735f 7365 7474 696e  k().oasis_settin
+000101b0: 6773 0a0a 2020 2020 2020 2020 6578 706c  gs..        expl
+000101c0: 6963 6974 5f67 6473 5f73 6574 7469 6e67  icit_gds_setting
+000101d0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+000101e0: 2020 6b3a 2076 0a20 2020 2020 2020 2020    k: v.         
+000101f0: 2020 2066 6f72 206b 2c20 7620 696e 206b     for k, v in k
+00010200: 7761 7267 732e 6974 656d 7328 290a 2020  wargs.items().  
+00010210: 2020 2020 2020 2020 2020 6966 2076 2069            if v i
+00010220: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206b  s not None and k
+00010230: 2069 6e20 6465 6661 756c 745f 7365 7474   in default_sett
+00010240: 696e 6773 2e64 6963 7428 290a 2020 2020  ings.dict().    
+00010250: 2020 2020 7d0a 2020 2020 2020 2020 6578      }.        ex
+00010260: 706c 6963 6974 5f6f 6173 5f73 6574 7469  plicit_oas_setti
+00010270: 6e67 7320 3d20 7b0a 2020 2020 2020 2020  ngs = {.        
+00010280: 2020 2020 6b3a 2076 0a20 2020 2020 2020      k: v.       
+00010290: 2020 2020 2066 6f72 206b 2c20 7620 696e       for k, v in
+000102a0: 206b 7761 7267 732e 6974 656d 7328 290a   kwargs.items().
+000102b0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+000102c0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+000102d0: 206b 2069 6e20 6465 6661 756c 745f 6f61   k in default_oa
+000102e0: 7369 735f 7365 7474 696e 6773 2e64 6963  sis_settings.dic
+000102f0: 7428 290a 2020 2020 2020 2020 7d0a 2020  t().        }.  
+00010300: 2020 2020 2020 2320 7570 6461 7465 2074        # update t
+00010310: 6865 2077 7269 7465 2073 6574 7469 6e67  he write setting
+00010320: 7320 7769 7468 2061 6e79 2073 6574 7469  s with any setti
+00010330: 6e67 7320 6578 706c 6963 6974 6c79 2070  ngs explicitly p
+00010340: 6173 7365 640a 2020 2020 2020 2020 7772  assed.        wr
+00010350: 6974 655f 7365 7474 696e 6773 203d 2064  ite_settings = d
+00010360: 6566 6175 6c74 5f73 6574 7469 6e67 732e  efault_settings.
+00010370: 636f 7079 2875 7064 6174 653d 6578 706c  copy(update=expl
+00010380: 6963 6974 5f67 6473 5f73 6574 7469 6e67  icit_gds_setting
+00010390: 7329 0a20 2020 2020 2020 206f 6173 6973  s).        oasis
+000103a0: 5f73 6574 7469 6e67 7320 3d20 6465 6661  _settings = defa
+000103b0: 756c 745f 6f61 7369 735f 7365 7474 696e  ult_oasis_settin
+000103c0: 6773 2e63 6f70 7928 7570 6461 7465 3d65  gs.copy(update=e
+000103d0: 7870 6c69 6369 745f 6f61 735f 7365 7474  xplicit_oas_sett
+000103e0: 696e 6773 290a 0a20 2020 2020 2020 205f  ings)..        _
+000103f0: 6368 6563 6b5f 756e 6361 6368 6564 5f63  check_uncached_c
+00010400: 6f6d 706f 6e65 6e74 7328 0a20 2020 2020  omponents(.     
+00010410: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
+00010420: 3d73 656c 662c 206d 6f64 653d 7772 6974  =self, mode=writ
+00010430: 655f 7365 7474 696e 6773 2e6f 6e5f 756e  e_settings.on_un
+00010440: 6361 6368 6564 5f63 6f6d 706f 6e65 6e74  cached_component
+00010450: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00010460: 2020 2020 6966 2077 7269 7465 5f73 6574      if write_set
+00010470: 7469 6e67 732e 666c 6174 7465 6e5f 696e  tings.flatten_in
+00010480: 7661 6c69 645f 7265 6673 3a0a 2020 2020  valid_refs:.    
+00010490: 2020 2020 2020 2020 746f 705f 6365 6c6c          top_cell
+000104a0: 203d 2066 6c61 7474 656e 5f69 6e76 616c   = flatten_inval
+000104b0: 6964 5f72 6566 735f 7265 6375 7273 6976  id_refs_recursiv
+000104c0: 6528 7365 6c66 290a 2020 2020 2020 2020  e(self).        
+000104d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000104e0: 2020 746f 705f 6365 6c6c 203d 2073 656c    top_cell = sel
+000104f0: 660a 0a20 2020 2020 2020 2067 6473 6469  f..        gdsdi
+00010500: 7220 3d20 6764 7364 6972 206f 7220 4744  r = gdsdir or GD
+00010510: 5344 4952 5f54 454d 500a 2020 2020 2020  SDIR_TEMP.      
+00010520: 2020 6764 7364 6972 203d 2070 6174 686c    gdsdir = pathl
+00010530: 6962 2e50 6174 6828 6764 7364 6972 290a  ib.Path(gdsdir).
+00010540: 2020 2020 2020 2020 6966 2077 6974 685f          if with_
+00010550: 6f61 7369 733a 0a20 2020 2020 2020 2020  oasis:.         
+00010560: 2020 2067 6473 7061 7468 203d 2067 6473     gdspath = gds
+00010570: 7061 7468 206f 7220 6764 7364 6972 202f  path or gdsdir /
+00010580: 2066 227b 746f 705f 6365 6c6c 2e6e 616d   f"{top_cell.nam
+00010590: 657d 2e6f 6173 220a 2020 2020 2020 2020  e}.oas".        
+000105a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000105b0: 2020 6764 7370 6174 6820 3d20 6764 7370    gdspath = gdsp
+000105c0: 6174 6820 6f72 2067 6473 6469 7220 2f20  ath or gdsdir / 
+000105d0: 6622 7b74 6f70 5f63 656c 6c2e 6e61 6d65  f"{top_cell.name
+000105e0: 7d2e 6764 7322 0a20 2020 2020 2020 2067  }.gds".        g
+000105f0: 6473 7061 7468 203d 2070 6174 686c 6962  dspath = pathlib
+00010600: 2e50 6174 6828 6764 7370 6174 6829 0a20  .Path(gdspath). 
+00010610: 2020 2020 2020 2067 6473 6469 7220 3d20         gdsdir = 
+00010620: 6764 7370 6174 682e 7061 7265 6e74 0a20  gdspath.parent. 
+00010630: 2020 2020 2020 2067 6473 6469 722e 6d6b         gdsdir.mk
+00010640: 6469 7228 6578 6973 745f 6f6b 3d54 7275  dir(exist_ok=Tru
+00010650: 652c 2070 6172 656e 7473 3d54 7275 6529  e, parents=True)
+00010660: 0a0a 2020 2020 2020 2020 6365 6c6c 7320  ..        cells 
+00010670: 3d20 746f 705f 6365 6c6c 2e67 6574 5f64  = top_cell.get_d
+00010680: 6570 656e 6465 6e63 6965 7328 7265 6375  ependencies(recu
+00010690: 7273 6976 653d 5472 7565 290a 2020 2020  rsive=True).    
+000106a0: 2020 2020 6365 6c6c 5f6e 616d 6573 203d      cell_names =
+000106b0: 205b 6365 6c6c 2e6e 616d 6520 666f 7220   [cell.name for 
+000106c0: 6365 6c6c 2069 6e20 6c69 7374 2863 656c  cell in list(cel
+000106d0: 6c73 295d 0a20 2020 2020 2020 2063 656c  ls)].        cel
+000106e0: 6c5f 6e61 6d65 735f 756e 6971 7565 203d  l_names_unique =
+000106f0: 2073 6574 2863 656c 6c5f 6e61 6d65 7329   set(cell_names)
+00010700: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00010710: 2863 656c 6c5f 6e61 6d65 7329 2021 3d20  (cell_names) != 
+00010720: 6c65 6e28 7365 7428 6365 6c6c 5f6e 616d  len(set(cell_nam
+00010730: 6573 2929 3a0a 2020 2020 2020 2020 2020  es)):.          
+00010740: 2020 666f 7220 6365 6c6c 5f6e 616d 6520    for cell_name 
+00010750: 696e 2063 656c 6c5f 6e61 6d65 735f 756e  in cell_names_un
+00010760: 6971 7565 3a0a 2020 2020 2020 2020 2020  ique:.          
+00010770: 2020 2020 2020 6365 6c6c 5f6e 616d 6573        cell_names
+00010780: 2e72 656d 6f76 6528 6365 6c6c 5f6e 616d  .remove(cell_nam
+00010790: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
+000107a0: 6966 2077 7269 7465 5f73 6574 7469 6e67  if write_setting
+000107b0: 732e 6f6e 5f64 7570 6c69 6361 7465 5f63  s.on_duplicate_c
+000107c0: 656c 6c20 3d3d 2022 6572 726f 7222 3a0a  ell == "error":.
+000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107e0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000107f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010800: 2020 2020 2020 6622 4475 706c 6963 6174        f"Duplicat
+00010810: 6564 2063 656c 6c20 6e61 6d65 7320 696e  ed cell names in
+00010820: 207b 746f 705f 6365 6c6c 2e6e 616d 6521   {top_cell.name!
+00010830: 727d 3a20 7b63 656c 6c5f 6e61 6d65 7321  r}: {cell_names!
+00010840: 727d 220a 2020 2020 2020 2020 2020 2020  r}".            
+00010850: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00010860: 2020 656c 6966 2077 7269 7465 5f73 6574    elif write_set
+00010870: 7469 6e67 732e 6f6e 5f64 7570 6c69 6361  tings.on_duplica
+00010880: 7465 5f63 656c 6c20 696e 207b 2277 6172  te_cell in {"war
+00010890: 6e22 2c20 226f 7665 7277 7269 7465 227d  n", "overwrite"}
+000108a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000108b0: 2020 6966 2077 7269 7465 5f73 6574 7469    if write_setti
+000108c0: 6e67 732e 6f6e 5f64 7570 6c69 6361 7465  ngs.on_duplicate
+000108d0: 5f63 656c 6c20 3d3d 2022 7761 726e 223a  _cell == "warn":
+000108e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000108f0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+00010900: 726e 280a 2020 2020 2020 2020 2020 2020  rn(.            
+00010910: 2020 2020 2020 2020 2020 2020 6622 4475              f"Du
+00010920: 706c 6963 6174 6564 2063 656c 6c20 6e61  plicated cell na
+00010930: 6d65 7320 696e 207b 746f 705f 6365 6c6c  mes in {top_cell
+00010940: 2e6e 616d 6521 727d 3a20 207b 6365 6c6c  .name!r}:  {cell
+00010950: 5f6e 616d 6573 7d22 2c0a 2020 2020 2020  _names}",.      
+00010960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010970: 2020 7374 6163 6b6c 6576 656c 3d33 2c0a    stacklevel=3,.
+00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010990: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000109a0: 2020 2020 2020 6365 6c6c 735f 6469 6374        cells_dict
+000109b0: 203d 207b 6365 6c6c 2e6e 616d 653a 2063   = {cell.name: c
+000109c0: 656c 6c2e 5f63 656c 6c20 666f 7220 6365  ell._cell for ce
+000109d0: 6c6c 2069 6e20 6365 6c6c 737d 0a20 2020  ll in cells}.   
+000109e0: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+000109f0: 6c73 203d 2063 656c 6c73 5f64 6963 742e  ls = cells_dict.
+00010a00: 7661 6c75 6573 2829 0a20 2020 2020 2020  values().       
+00010a10: 2020 2020 2065 6c69 6620 7772 6974 655f       elif write_
+00010a20: 7365 7474 696e 6773 2e6f 6e5f 6475 706c  settings.on_dupl
+00010a30: 6963 6174 655f 6365 6c6c 2069 7320 6e6f  icate_cell is no
+00010a40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00010a50: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00010a60: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00010a70: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00010a80: 6f6e 5f64 7570 6c69 6361 7465 5f63 656c  on_duplicate_cel
+00010a90: 6c3a 207b 7772 6974 655f 7365 7474 696e  l: {write_settin
+00010aa0: 6773 2e6f 6e5f 6475 706c 6963 6174 655f  gs.on_duplicate_
+00010ab0: 6365 6c6c 2172 7d20 6e6f 7420 696e 2028  cell!r} not in (
+00010ac0: 4e6f 6e65 2c20 7761 726e 2c20 6572 726f  None, warn, erro
+00010ad0: 722c 206f 7665 7277 7269 7465 2922 0a20  r, overwrite)". 
+00010ae0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010af0: 0a0a 2020 2020 2020 2020 616c 6c5f 6365  ..        all_ce
+00010b00: 6c6c 7320 3d20 5b74 6f70 5f63 656c 6c2e  lls = [top_cell.
+00010b10: 5f63 656c 6c5d 202b 2073 6f72 7465 6428  _cell] + sorted(
+00010b20: 6365 6c6c 732c 206b 6579 3d6c 616d 6264  cells, key=lambd
+00010b30: 6120 6363 3a20 6363 2e6e 616d 6529 0a0a  a cc: cc.name)..
+00010b40: 2020 2020 2020 2020 6e6f 5f6e 616d 655f          no_name_
+00010b50: 6365 6c6c 7320 3d20 5b0a 2020 2020 2020  cells = [.      
+00010b60: 2020 2020 2020 6365 6c6c 2e6e 616d 6520        cell.name 
+00010b70: 666f 7220 6365 6c6c 2069 6e20 616c 6c5f  for cell in all_
+00010b80: 6365 6c6c 7320 6966 2063 656c 6c2e 6e61  cells if cell.na
+00010b90: 6d65 2e73 7461 7274 7377 6974 6828 2255  me.startswith("U
+00010ba0: 6e6e 616d 6564 2229 0a20 2020 2020 2020  nnamed").       
+00010bb0: 205d 0a0a 2020 2020 2020 2020 6966 206e   ]..        if n
+00010bc0: 6f5f 6e61 6d65 5f63 656c 6c73 3a0a 2020  o_name_cells:.  
+00010bd0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+00010be0: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
+00010bf0: 2020 2020 2020 2020 2066 2243 6f6d 706f           f"Compo
+00010c00: 6e65 6e74 207b 746f 705f 6365 6c6c 2e6e  nent {top_cell.n
+00010c10: 616d 6521 727d 2063 6f6e 7461 696e 7320  ame!r} contains 
+00010c20: 7b6c 656e 286e 6f5f 6e61 6d65 5f63 656c  {len(no_name_cel
+00010c30: 6c73 297d 2055 6e6e 616d 6564 2063 656c  ls)} Unnamed cel
+00010c40: 6c73 222c 0a20 2020 2020 2020 2020 2020  ls",.           
+00010c50: 2020 2020 2073 7461 636b 6c65 7665 6c3d       stacklevel=
+00010c60: 332c 0a20 2020 2020 2020 2020 2020 2029  3,.            )
+00010c70: 0a0a 2020 2020 2020 2020 2320 666f 7220  ..        # for 
+00010c80: 6365 6c6c 2069 6e20 616c 6c5f 6365 6c6c  cell in all_cell
+00010c90: 733a 0a20 2020 2020 2020 2023 2020 2020  s:.        #    
+00010ca0: 2070 7269 6e74 2863 656c 6c2e 6e61 6d65   print(cell.name
+00010cb0: 2c20 7479 7065 2863 656c 6c29 290a 0a20  , type(cell)).. 
+00010cc0: 2020 2020 2020 206c 6962 203d 2067 6473         lib = gds
+00010cd0: 746b 2e4c 6962 7261 7279 280a 2020 2020  tk.Library(.    
+00010ce0: 2020 2020 2020 2020 6e61 6d65 3d77 7269          name=wri
+00010cf0: 7465 5f73 6574 7469 6e67 732e 6c69 625f  te_settings.lib_
+00010d00: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00010d10: 2020 756e 6974 3d77 7269 7465 5f73 6574    unit=write_set
+00010d20: 7469 6e67 732e 756e 6974 2c0a 2020 2020  tings.unit,.    
+00010d30: 2020 2020 2020 2020 7072 6563 6973 696f          precisio
+00010d40: 6e3d 7772 6974 655f 7365 7474 696e 6773  n=write_settings
+00010d50: 2e70 7265 6369 7369 6f6e 2c0a 2020 2020  .precision,.    
+00010d60: 2020 2020 290a 2020 2020 2020 2020 6c69      ).        li
+00010d70: 622e 6164 6428 746f 705f 6365 6c6c 2e5f  b.add(top_cell._
+00010d80: 6365 6c6c 290a 2020 2020 2020 2020 6c69  cell).        li
+00010d90: 622e 6164 6428 2a74 6f70 5f63 656c 6c2e  b.add(*top_cell.
+00010da0: 5f63 656c 6c2e 6465 7065 6e64 656e 6369  _cell.dependenci
+00010db0: 6573 2854 7275 6529 290a 0a20 2020 2020  es(True))..     
+00010dc0: 2020 2069 6620 7769 7468 5f6f 6173 6973     if with_oasis
+00010dd0: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
+00010de0: 622e 7772 6974 655f 6f61 7328 6764 7370  b.write_oas(gdsp
+00010df0: 6174 682c 202a 2a6f 6173 6973 5f73 6574  ath, **oasis_set
+00010e00: 7469 6e67 732e 6469 6374 2829 290a 2020  tings.dict()).  
+00010e10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00010e20: 2020 2020 2020 2020 6c69 622e 7772 6974          lib.writ
+00010e30: 655f 6764 7328 0a20 2020 2020 2020 2020  e_gds(.         
+00010e40: 2020 2020 2020 2067 6473 7061 7468 2c20         gdspath, 
+00010e50: 7469 6d65 7374 616d 703d 7469 6d65 7374  timestamp=timest
+00010e60: 616d 702c 206d 6178 5f70 6f69 6e74 733d  amp, max_points=
+00010e70: 7772 6974 655f 7365 7474 696e 6773 2e6d  write_settings.m
+00010e80: 6178 5f70 6f69 6e74 730a 2020 2020 2020  ax_points.      
+00010e90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010ea0: 6966 206c 6f67 6769 6e67 3a0a 2020 2020  if logging:.    
+00010eb0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00010ec0: 6e66 6f28 6622 5772 6f74 6520 746f 207b  nfo(f"Wrote to {
+00010ed0: 7374 7228 6764 7370 6174 6829 2172 7d22  str(gdspath)!r}"
+00010ee0: 290a 2020 2020 2020 2020 6966 2077 6974  ).        if wit
+00010ef0: 685f 6d65 7461 6461 7461 3a0a 2020 2020  h_metadata:.    
+00010f00: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+00010f10: 203d 2067 6473 7061 7468 2e77 6974 685f   = gdspath.with_
+00010f20: 7375 6666 6978 2822 2e79 6d6c 2229 0a20  suffix(".yml"). 
+00010f30: 2020 2020 2020 2020 2020 206d 6574 6164             metad
+00010f40: 6174 612e 7772 6974 655f 7465 7874 2873  ata.write_text(s
+00010f50: 656c 662e 746f 5f79 616d 6c28 7769 7468  elf.to_yaml(with
+00010f60: 5f63 656c 6c73 3d54 7275 652c 2077 6974  _cells=True, wit
+00010f70: 685f 706f 7274 733d 5472 7565 2929 0a20  h_ports=True)). 
+00010f80: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00010f90: 722e 696e 666f 2866 2257 7269 7465 2059  r.info(f"Write Y
+00010fa0: 414d 4c20 6d65 7461 6461 7461 2074 6f20  AML metadata to 
+00010fb0: 7b73 7472 286d 6574 6164 6174 6129 2172  {str(metadata)!r
+00010fc0: 7d22 290a 0a20 2020 2020 2020 2043 4f4e  }")..        CON
+00010fd0: 462e 6c61 7374 5f73 6176 6564 5f66 696c  F.last_saved_fil
+00010fe0: 6573 2e61 7070 656e 6428 6764 7370 6174  es.append(gdspat
+00010ff0: 6829 0a20 2020 2020 2020 2072 6574 7572  h).        retur
+00011000: 6e20 6764 7370 6174 680a 0a20 2020 2064  n gdspath..    d
+00011010: 6566 2077 7269 7465 5f67 6473 280a 2020  ef write_gds(.  
+00011020: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00011030: 2020 2020 6764 7370 6174 683a 2050 6174      gdspath: Pat
+00011040: 6854 7970 6520 7c20 4e6f 6e65 203d 204e  hType | None = N
+00011050: 6f6e 652c 0a20 2020 2020 2020 2067 6473  one,.        gds
+00011060: 6469 723a 2050 6174 6854 7970 6520 7c20  dir: PathType | 
+00011070: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
+00011080: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
+00011090: 2020 2029 202d 3e20 5061 7468 3a0a 2020     ) -> Path:.  
+000110a0: 2020 2020 2020 2222 2257 7269 7465 2063        """Write c
+000110b0: 6f6d 706f 6e65 6e74 2074 6f20 4744 5320  omponent to GDS 
+000110c0: 616e 6420 7265 7475 726e 7320 6764 7370  and returns gdsp
+000110d0: 6174 682e 0a0a 2020 2020 2020 2020 4172  ath...        Ar
+000110e0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+000110f0: 6764 7370 6174 683a 2047 4453 2066 696c  gdspath: GDS fil
+00011100: 6520 7061 7468 2074 6f20 7772 6974 6520  e path to write 
+00011110: 746f 2e0a 2020 2020 2020 2020 2020 2020  to..            
+00011120: 6764 7364 6972 3a20 6469 7265 6374 6f72  gdsdir: director
+00011130: 7920 666f 7220 7468 6520 4744 5320 6669  y for the GDS fi
+00011140: 6c65 2e20 4465 6661 756c 7473 2074 6f20  le. Defaults to 
+00011150: 2f74 6d70 2f72 616e 646f 6d46 696c 652f  /tmp/randomFile/
+00011160: 6764 7366 6163 746f 7279 2e0a 0a20 2020  gdsfactory...   
+00011170: 2020 2020 204b 6579 776f 7264 2041 7267       Keyword Arg
+00011180: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
+00011190: 6e69 743a 2075 6e69 7420 7369 7a65 2066  nit: unit size f
+000111a0: 6f72 206f 626a 6563 7473 2069 6e20 6c69  or objects in li
+000111b0: 6272 6172 792e 2031 756d 2062 7920 6465  brary. 1um by de
+000111c0: 6661 756c 742e 0a20 2020 2020 2020 2020  fault..         
+000111d0: 2020 2070 7265 6369 7369 6f6e 3a20 666f     precision: fo
+000111e0: 7220 6469 6d65 6e73 696f 6e73 2069 6e20  r dimensions in 
+000111f0: 7468 6520 6c69 6272 6172 7920 286d 292e  the library (m).
+00011200: 2031 6e6d 2062 7920 6465 6661 756c 742e   1nm by default.
+00011210: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00011220: 6769 6e67 3a20 6469 7361 626c 6520 4744  ging: disable GD
+00011230: 5320 7061 7468 206c 6f67 6769 6e67 2c20  S path logging, 
+00011240: 666f 7220 6578 616d 706c 6520 666f 7220  for example for 
+00011250: 7368 6f77 696e 6720 6974 2069 6e20 4b4c  showing it in KL
+00011260: 6179 6f75 742e 0a20 2020 2020 2020 2020  ayout..         
+00011270: 2020 206f 6e5f 6475 706c 6963 6174 655f     on_duplicate_
+00011280: 6365 6c6c 3a20 7370 6563 6966 7920 686f  cell: specify ho
+00011290: 7720 746f 2072 6573 6f6c 7665 2064 7570  w to resolve dup
+000112a0: 6c69 6361 7465 2d6e 616d 6564 2063 656c  licate-named cel
+000112b0: 6c73 2e20 4368 6f6f 7365 206f 6e65 206f  ls. Choose one o
+000112c0: 6620 7468 6520 666f 6c6c 6f77 696e 673a  f the following:
+000112d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000112e0: 2022 7761 726e 2220 2864 6566 6175 6c74   "warn" (default
+000112f0: 293a 206f 7665 7277 7269 7465 2061 6c6c  ): overwrite all
+00011300: 2064 7570 6c69 6361 7465 2063 656c 6c73   duplicate cells
+00011310: 2077 6974 6820 6f6e 6520 6f66 2074 6865   with one of the
+00011320: 2064 7570 6c69 6361 7465 7320 2861 7262   duplicates (arb
+00011330: 6974 7261 7269 6c79 292e 0a20 2020 2020  itrarily)..     
+00011340: 2020 2020 2020 2020 2020 2022 6572 726f             "erro
+00011350: 7222 3a20 7468 726f 7720 6120 5661 6c75  r": throw a Valu
+00011360: 6545 7272 6f72 2077 6865 6e20 6174 7465  eError when atte
+00011370: 6d70 7469 6e67 2074 6f20 7772 6974 6520  mpting to write 
+00011380: 6120 6764 7320 7769 7468 2064 7570 6c69  a gds with dupli
+00011390: 6361 7465 2063 656c 6c73 2e0a 2020 2020  cate cells..    
+000113a0: 2020 2020 2020 2020 2020 2020 226f 7665              "ove
+000113b0: 7277 7269 7465 223a 206f 7665 7277 7269  rwrite": overwri
+000113c0: 7465 2061 6c6c 2064 7570 6c69 6361 7465  te all duplicate
+000113d0: 2063 656c 6c73 2077 6974 6820 6f6e 6520   cells with one 
+000113e0: 6f66 2074 6865 2064 7570 6c69 6361 7465  of the duplicate
+000113f0: 732c 2077 6974 686f 7574 2077 6172 6e69  s, without warni
+00011400: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
+00011410: 6f6e 5f75 6e63 6163 6865 645f 636f 6d70  on_uncached_comp
+00011420: 6f6e 656e 743a 204c 6974 6572 616c 5b22  onent: Literal["
+00011430: 7761 726e 222c 2022 6572 726f 7222 5d20  warn", "error"] 
+00011440: 3d20 2277 6172 6e22 0a20 2020 2020 2020  = "warn".       
+00011450: 2020 2020 2066 6c61 7474 656e 5f69 6e76       flatten_inv
+00011460: 616c 6964 5f72 6566 733a 2066 6c61 7474  alid_refs: flatt
+00011470: 656e 7320 636f 6d70 6f6e 656e 7420 7265  ens component re
+00011480: 6665 7265 6e63 6573 2077 6869 6368 2068  ferences which h
+00011490: 6176 6520 696e 7661 6c69 6420 7472 616e  ave invalid tran
+000114a0: 7366 6f72 6d61 7469 6f6e 732e 0a20 2020  sformations..   
+000114b0: 2020 2020 2020 2020 206d 6178 5f70 6f69           max_poi
+000114c0: 6e74 733a 204d 6178 696d 616c 206e 756d  nts: Maximal num
+000114d0: 6265 7220 6f66 2076 6572 7469 6365 7320  ber of vertices 
+000114e0: 7065 7220 706f 6c79 676f 6e2e 0a20 2020  per polygon..   
+000114f0: 2020 2020 2020 2020 2020 2020 2050 6f6c               Pol
+00011500: 7967 6f6e 7320 7769 7468 206d 6f72 6520  ygons with more 
+00011510: 7665 7274 6963 6573 2074 6861 7420 7468  vertices that th
+00011520: 6973 2061 7265 2061 7574 6f6d 6174 6963  is are automatic
+00011530: 616c 6c79 2066 7261 6374 7572 6564 2e0a  ally fractured..
+00011540: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00011550: 5f6d 6574 6164 6174 613a 2077 7269 7465  _metadata: write
+00011560: 7320 6d65 7461 6461 7461 2069 6e20 5941  s metadata in YA
+00011570: 4d4c 2066 6f72 6d61 742e 0a20 2020 2020  ML format..     
+00011580: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00011590: 7265 7475 726e 2073 656c 662e 5f77 7269  return self._wri
+000115a0: 7465 5f6c 6962 7261 7279 280a 2020 2020  te_library(.    
+000115b0: 2020 2020 2020 2020 6764 7370 6174 683d          gdspath=
+000115c0: 6764 7370 6174 682c 2067 6473 6469 723d  gdspath, gdsdir=
+000115d0: 6764 7364 6972 2c20 7769 7468 5f6f 6173  gdsdir, with_oas
+000115e0: 6973 3d46 616c 7365 2c20 2a2a 6b77 6172  is=False, **kwar
+000115f0: 6773 0a20 2020 2020 2020 2029 0a0a 2020  gs.        )..  
+00011600: 2020 6465 6620 7772 6974 655f 6f61 7328    def write_oas(
+00011610: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00011620: 2020 2020 2020 2067 6473 7061 7468 3a20         gdspath: 
+00011630: 5061 7468 5479 7065 207c 204e 6f6e 6520  PathType | None 
+00011640: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00011650: 6764 7364 6972 3a20 5061 7468 5479 7065  gdsdir: PathType
+00011660: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
+00011670: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+00011680: 2c0a 2020 2020 2920 2d3e 2050 6174 683a  ,.    ) -> Path:
+00011690: 0a20 2020 2020 2020 2022 2222 5772 6974  .        """Writ
+000116a0: 6520 636f 6d70 6f6e 656e 7420 746f 2047  e component to G
+000116b0: 4453 2061 6e64 2072 6574 7572 6e73 2067  DS and returns g
+000116c0: 6473 7061 7468 2e0a 0a20 2020 2020 2020  dspath...       
+000116d0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+000116e0: 2020 2067 6473 7061 7468 3a20 4744 5320     gdspath: GDS 
+000116f0: 6669 6c65 2070 6174 6820 746f 2077 7269  file path to wri
+00011700: 7465 2074 6f2e 0a20 2020 2020 2020 2020  te to..         
+00011710: 2020 2067 6473 6469 723a 2064 6972 6563     gdsdir: direc
+00011720: 746f 7279 2066 6f72 2074 6865 2047 4453  tory for the GDS
+00011730: 2066 696c 652e 2044 6566 6175 6c74 7320   file. Defaults 
+00011740: 746f 202f 746d 702f 7261 6e64 6f6d 4669  to /tmp/randomFi
+00011750: 6c65 2f67 6473 6661 6374 6f72 792e 0a0a  le/gdsfactory...
+00011760: 2020 2020 2020 2020 4b65 7977 6f72 6420          Keyword 
+00011770: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00011780: 2020 756e 6974 3a20 756e 6974 2073 697a    unit: unit siz
+00011790: 6520 666f 7220 6f62 6a65 6374 7320 696e  e for objects in
+000117a0: 206c 6962 7261 7279 2e20 3175 6d20 6279   library. 1um by
+000117b0: 2064 6566 6175 6c74 2e0a 2020 2020 2020   default..      
+000117c0: 2020 2020 2020 7072 6563 6973 696f 6e3a        precision:
+000117d0: 2066 6f72 2064 696d 656e 7369 6f6e 7320   for dimensions 
+000117e0: 696e 2074 6865 206c 6962 7261 7279 2028  in the library (
+000117f0: 6d29 2e20 316e 6d20 6279 2064 6566 6175  m). 1nm by defau
+00011800: 6c74 2e0a 2020 2020 2020 2020 2020 2020  lt..            
+00011810: 6c6f 6767 696e 673a 2064 6973 6162 6c65  logging: disable
+00011820: 2047 4453 2070 6174 6820 6c6f 6767 696e   GDS path loggin
+00011830: 672c 2066 6f72 2065 7861 6d70 6c65 2066  g, for example f
+00011840: 6f72 2073 686f 7769 6e67 2069 7420 696e  or showing it in
+00011850: 204b 4c61 796f 7574 2e0a 2020 2020 2020   KLayout..      
+00011860: 2020 2020 2020 6f6e 5f64 7570 6c69 6361        on_duplica
+00011870: 7465 5f63 656c 6c3a 2073 7065 6369 6679  te_cell: specify
+00011880: 2068 6f77 2074 6f20 7265 736f 6c76 6520   how to resolve 
+00011890: 6475 706c 6963 6174 652d 6e61 6d65 6420  duplicate-named 
+000118a0: 6365 6c6c 732e 2043 686f 6f73 6520 6f6e  cells. Choose on
+000118b0: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
+000118c0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+000118d0: 2020 2020 2277 6172 6e22 2028 6465 6661      "warn" (defa
+000118e0: 756c 7429 3a20 6f76 6572 7772 6974 6520  ult): overwrite 
+000118f0: 616c 6c20 6475 706c 6963 6174 6520 6365  all duplicate ce
+00011900: 6c6c 7320 7769 7468 206f 6e65 206f 6620  lls with one of 
+00011910: 7468 6520 6475 706c 6963 6174 6573 2028  the duplicates (
+00011920: 6172 6269 7472 6172 696c 7929 2e0a 2020  arbitrarily)..  
+00011930: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00011940: 7272 6f72 223a 2074 6872 6f77 2061 2056  rror": throw a V
+00011950: 616c 7565 4572 726f 7220 7768 656e 2061  alueError when a
+00011960: 7474 656d 7074 696e 6720 746f 2077 7269  ttempting to wri
+00011970: 7465 2061 2067 6473 2077 6974 6820 6475  te a gds with du
+00011980: 706c 6963 6174 6520 6365 6c6c 732e 0a20  plicate cells.. 
+00011990: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000119a0: 6f76 6572 7772 6974 6522 3a20 6f76 6572  overwrite": over
+000119b0: 7772 6974 6520 616c 6c20 6475 706c 6963  write all duplic
+000119c0: 6174 6520 6365 6c6c 7320 7769 7468 206f  ate cells with o
+000119d0: 6e65 206f 6620 7468 6520 6475 706c 6963  ne of the duplic
+000119e0: 6174 6573 2c20 7769 7468 6f75 7420 7761  ates, without wa
+000119f0: 726e 696e 672e 0a20 2020 2020 2020 2020  rning..         
+00011a00: 2020 2020 2020 204e 6f6e 653a 2064 6f20         None: do 
+00011a10: 6e6f 7420 7472 7920 746f 2072 6573 6f6c  not try to resol
+00011a20: 7665 2028 6174 2079 6f75 7220 6f77 6e20  ve (at your own 
+00011a30: 7269 736b 2129 0a20 2020 2020 2020 2020  risk!).         
+00011a40: 2020 206f 6e5f 756e 6361 6368 6564 5f63     on_uncached_c
+00011a50: 6f6d 706f 6e65 6e74 3a20 4c69 7465 7261  omponent: Litera
+00011a60: 6c5b 2277 6172 6e22 2c20 2265 7272 6f72  l["warn", "error
+00011a70: 225d 203d 2022 7761 726e 220a 2020 2020  "] = "warn".    
+00011a80: 2020 2020 2020 2020 666c 6174 7465 6e5f          flatten_
+00011a90: 696e 7661 6c69 645f 7265 6673 3a20 666c  invalid_refs: fl
+00011aa0: 6174 7465 6e73 2063 6f6d 706f 6e65 6e74  attens component
+00011ab0: 2072 6566 6572 656e 6365 7320 7768 6963   references whic
+00011ac0: 6820 6861 7665 2069 6e76 616c 6964 2074  h have invalid t
+00011ad0: 7261 6e73 666f 726d 6174 696f 6e73 2e0a  ransformations..
+00011ae0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00011af0: 7265 7373 696f 6e5f 6c65 7665 6c3a 204c  ression_level: L
+00011b00: 6576 656c 206f 6620 636f 6d70 7265 7373  evel of compress
+00011b10: 696f 6e20 666f 7220 6365 6c6c 7320 2862  ion for cells (b
+00011b20: 6574 7765 656e 2030 2061 6e64 2039 292e  etween 0 and 9).
+00011b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011b40: 2053 6574 7469 6e67 2074 6f20 3020 7769   Setting to 0 wi
+00011b50: 6c6c 2064 6973 6162 6c65 2063 656c 6c20  ll disable cell 
+00011b60: 636f 6d70 7265 7373 696f 6e2c 2031 2067  compression, 1 g
+00011b70: 6976 6573 2074 6865 2062 6573 7420 7370  ives the best sp
+00011b80: 6565 6420 616e 6420 392c 2074 6865 2062  eed and 9, the b
+00011b90: 6573 7420 636f 6d70 7265 7373 696f 6e2e  est compression.
+00011ba0: 0a20 2020 2020 2020 2020 2020 2064 6574  .            det
+00011bb0: 6563 745f 7265 6374 616e 676c 6573 3a20  ect_rectangles: 
+00011bc0: 5374 6f72 6520 7265 6374 616e 676c 6573  Store rectangles
+00011bd0: 2069 6e20 636f 6d70 7265 7373 6564 2066   in compressed f
+00011be0: 6f72 6d61 742e 0a20 2020 2020 2020 2020  ormat..         
+00011bf0: 2020 2064 6574 6563 745f 7472 6170 657a     detect_trapez
+00011c00: 6f69 6473 3a20 5374 6f72 6520 7472 6170  oids: Store trap
+00011c10: 657a 6f69 6473 2069 6e20 636f 6d70 7265  ezoids in compre
+00011c20: 7373 6564 2066 6f72 6d61 742e 0a20 2020  ssed format..   
+00011c30: 2020 2020 2020 2020 2063 6972 636c 655f           circle_
+00011c40: 746f 6c65 7261 6e63 653a 2054 6f6c 6572  tolerance: Toler
+00011c50: 616e 6365 2066 6f72 2064 6574 6563 7469  ance for detecti
+00011c60: 6e67 2063 6972 636c 6573 2e20 4966 206c  ng circles. If l
+00011c70: 6573 7320 6f72 2065 7175 616c 2074 6f20  ess or equal to 
+00011c80: 302c 206e 6f20 6465 7465 6374 696f 6e20  0, no detection 
+00011c90: 6973 2070 6572 666f 726d 6564 2e0a 2020  is performed..  
+00011ca0: 2020 2020 2020 2020 2020 2020 2020 4369                Ci
+00011cb0: 7263 6c65 7320 6172 6520 7374 6f72 6564  rcles are stored
+00011cc0: 2069 6e20 636f 6d70 7265 7373 6564 2066   in compressed f
+00011cd0: 6f72 6d61 742e 0a20 2020 2020 2020 2020  ormat..         
+00011ce0: 2020 2076 616c 6964 6174 696f 6e20 2822     validation ("
+00011cf0: 6372 6333 3222 2c20 2263 6865 636b 7375  crc32", "checksu
+00011d00: 6d33 3222 2c20 4e6f 6e65 2920 e280 9320  m32", None) ... 
+00011d10: 7479 7065 206f 6620 7661 6c69 6461 7469  type of validati
+00011d20: 6f6e 2074 6f20 696e 636c 7564 6520 696e  on to include in
+00011d30: 2074 6865 2073 6176 6564 2066 696c 652e   the saved file.
+00011d40: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00011d50: 6e64 6172 645f 7072 6f70 6572 7469 6573  ndard_properties
+00011d60: 3a20 5374 6f72 6520 7374 616e 6461 7264  : Store standard
+00011d70: 204f 4153 4953 2070 726f 7065 7274 6965   OASIS propertie
+00011d80: 7320 696e 2074 6865 2066 696c 652e 0a20  s in the file.. 
+00011d90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011da0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00011db0: 7772 6974 655f 6c69 6272 6172 7928 0a20  write_library(. 
+00011dc0: 2020 2020 2020 2020 2020 2067 6473 7061             gdspa
+00011dd0: 7468 3d67 6473 7061 7468 2c0a 2020 2020  th=gdspath,.    
+00011de0: 2020 2020 2020 2020 6764 7364 6972 3d67          gdsdir=g
+00011df0: 6473 6469 722c 0a20 2020 2020 2020 2020  dsdir,.         
+00011e00: 2020 2077 6974 685f 6f61 7369 733d 5472     with_oasis=Tr
+00011e10: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00011e20: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
+00011e30: 2020 290a 0a20 2020 2064 6566 2077 7269    )..    def wri
+00011e40: 7465 5f67 6473 5f77 6974 685f 6d65 7461  te_gds_with_meta
+00011e50: 6461 7461 2873 656c 662c 202a 6172 6773  data(self, *args
+00011e60: 2c20 2a2a 6b77 6172 6773 2920 2d3e 2050  , **kwargs) -> P
+00011e70: 6174 683a 0a20 2020 2020 2020 2022 2222  ath:.        """
+00011e80: 5772 6974 6520 636f 6d70 6f6e 656e 7420  Write component 
+00011e90: 696e 2047 4453 2061 6e64 206d 6574 6164  in GDS and metad
+00011ea0: 6174 6120 2863 6f6d 706f 6e65 6e74 2073  ata (component s
+00011eb0: 6574 7469 6e67 7329 2069 6e20 5941 4d4c  ettings) in YAML
+00011ec0: 2e22 2222 0a20 2020 2020 2020 2077 6172  .""".        war
+00011ed0: 6e69 6e67 732e 7761 726e 280a 2020 2020  nings.warn(.    
+00011ee0: 2020 2020 2020 2020 2243 6f6d 706f 6e65          "Compone
+00011ef0: 6e74 2e77 7269 7465 5f67 6473 5f77 6974  nt.write_gds_wit
+00011f00: 685f 6d65 7461 6461 7461 2829 2069 7320  h_metadata() is 
+00011f10: 6465 7072 6563 6174 6564 2e20 220a 2020  deprecated. ".  
+00011f20: 2020 2020 2020 2020 2020 2255 7365 2043            "Use C
+00011f30: 6f6d 706f 6e65 6e74 2e77 7269 7465 5f67  omponent.write_g
+00011f40: 6473 2877 6974 685f 6d65 7461 6461 7461  ds(with_metadata
+00011f50: 3d54 7275 6529 206f 7220 436f 6d70 6f6e  =True) or Compon
+00011f60: 656e 742e 7772 6974 655f 6f61 7328 7769  ent.write_oas(wi
+00011f70: 7468 5f6d 6574 6164 6174 613d 5472 7565  th_metadata=True
+00011f80: 292e 222c 0a20 2020 2020 2020 2020 2020  ).",.           
+00011f90: 2073 7461 636b 6c65 7665 6c3d 332c 0a20   stacklevel=3,. 
+00011fa0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00011fb0: 2067 6473 7061 7468 203d 2073 656c 662e   gdspath = self.
+00011fc0: 7772 6974 655f 6764 7328 2a61 7267 732c  write_gds(*args,
+00011fd0: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+00011fe0: 2020 206d 6574 6164 6174 6120 3d20 6764     metadata = gd
+00011ff0: 7370 6174 682e 7769 7468 5f73 7566 6669  spath.with_suffi
+00012000: 7828 222e 796d 6c22 290a 2020 2020 2020  x(".yml").      
+00012010: 2020 6d65 7461 6461 7461 2e77 7269 7465    metadata.write
+00012020: 5f74 6578 7428 7365 6c66 2e74 6f5f 7961  _text(self.to_ya
+00012030: 6d6c 2877 6974 685f 6365 6c6c 733d 5472  ml(with_cells=Tr
+00012040: 7565 2c20 7769 7468 5f70 6f72 7473 3d54  ue, with_ports=T
+00012050: 7275 6529 290a 2020 2020 2020 2020 6c6f  rue)).        lo
+00012060: 6767 6572 2e69 6e66 6f28 6622 5772 6974  gger.info(f"Writ
+00012070: 6520 5941 4d4c 206d 6574 6164 6174 6120  e YAML metadata 
+00012080: 746f 207b 7374 7228 6d65 7461 6461 7461  to {str(metadata
+00012090: 2921 727d 2229 0a20 2020 2020 2020 2072  )!r}").        r
+000120a0: 6574 7572 6e20 6764 7370 6174 680a 0a20  eturn gdspath.. 
+000120b0: 2020 2064 6566 2074 6f5f 6469 6374 280a     def to_dict(.
+000120c0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000120d0: 2020 2020 2020 6967 6e6f 7265 5f63 6f6d        ignore_com
+000120e0: 706f 6e65 6e74 735f 7072 6566 6978 3a20  ponents_prefix: 
+000120f0: 6c69 7374 5b73 7472 5d20 7c20 4e6f 6e65  list[str] | None
+00012100: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00012110: 2069 676e 6f72 655f 6675 6e63 7469 6f6e   ignore_function
+00012120: 735f 7072 6566 6978 3a20 6c69 7374 5b73  s_prefix: list[s
+00012130: 7472 5d20 7c20 4e6f 6e65 203d 204e 6f6e  tr] | None = Non
+00012140: 652c 0a20 2020 2020 2020 2077 6974 685f  e,.        with_
+00012150: 6365 6c6c 733a 2062 6f6f 6c20 3d20 4661  cells: bool = Fa
+00012160: 6c73 652c 0a20 2020 2020 2020 2077 6974  lse,.        wit
+00012170: 685f 706f 7274 733a 2062 6f6f 6c20 3d20  h_ports: bool = 
+00012180: 5472 7565 2c0a 2020 2020 2920 2d3e 2064  True,.    ) -> d
+00012190: 6963 745b 7374 722c 2041 6e79 5d3a 0a20  ict[str, Any]:. 
+000121a0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+000121b0: 7320 4469 6374 2072 6570 7265 7365 6e74  s Dict represent
+000121c0: 6174 696f 6e20 6f66 2061 2063 6f6d 706f  ation of a compo
+000121d0: 6e65 6e74 2e0a 0a20 2020 2020 2020 2041  nent...        A
+000121e0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+000121f0: 2069 676e 6f72 655f 636f 6d70 6f6e 656e   ignore_componen
+00012200: 7473 5f70 7265 6669 783a 2066 6f72 2063  ts_prefix: for c
+00012210: 6f6d 706f 6e65 6e74 7320 746f 2069 676e  omponents to ign
+00012220: 6f72 6520 7768 656e 2065 7870 6f72 7469  ore when exporti
+00012230: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
+00012240: 6967 6e6f 7265 5f66 756e 6374 696f 6e73  ignore_functions
+00012250: 5f70 7265 6669 783a 2066 6f72 2066 756e  _prefix: for fun
+00012260: 6374 696f 6e73 2074 6f20 6967 6e6f 7265  ctions to ignore
+00012270: 2077 6865 6e20 6578 706f 7274 696e 672e   when exporting.
+00012280: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00012290: 685f 6365 6c6c 733a 2077 7269 7465 2063  h_cells: write c
+000122a0: 656c 6c73 2072 6563 7572 7369 7665 6c79  ells recursively
+000122b0: 2e0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+000122c0: 7468 5f70 6f72 7473 3a20 7772 6974 6520  th_ports: write 
+000122d0: 706f 7274 2069 6e66 6f72 6d61 7469 6f6e  port information
+000122e0: 2064 6963 742e 0a20 2020 2020 2020 2022   dict..        "
+000122f0: 2222 0a20 2020 2020 2020 2064 203d 207b  "".        d = {
+00012300: 7d0a 2020 2020 2020 2020 6966 2077 6974  }.        if wit
+00012310: 685f 706f 7274 733a 0a20 2020 2020 2020  h_ports:.       
+00012320: 2020 2020 2070 6f72 7473 203d 207b 706f       ports = {po
+00012330: 7274 2e6e 616d 653a 2070 6f72 742e 746f  rt.name: port.to
+00012340: 5f64 6963 7428 2920 666f 7220 706f 7274  _dict() for port
+00012350: 2069 6e20 7365 6c66 2e67 6574 5f70 6f72   in self.get_por
+00012360: 7473 5f6c 6973 7428 297d 0a20 2020 2020  ts_list()}.     
+00012370: 2020 2020 2020 2064 5b22 706f 7274 7322         d["ports"
+00012380: 5d20 3d20 706f 7274 730a 0a20 2020 2020  ] = ports..     
+00012390: 2020 2069 6620 7769 7468 5f63 656c 6c73     if with_cells
+000123a0: 3a0a 2020 2020 2020 2020 2020 2020 6365  :.            ce
+000123b0: 6c6c 7320 3d20 7265 6375 7273 655f 7374  lls = recurse_st
+000123c0: 7275 6374 7572 6573 280a 2020 2020 2020  ructures(.      
+000123d0: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
+000123e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123f0: 6967 6e6f 7265 5f66 756e 6374 696f 6e73  ignore_functions
+00012400: 5f70 7265 6669 783d 6967 6e6f 7265 5f66  _prefix=ignore_f
+00012410: 756e 6374 696f 6e73 5f70 7265 6669 782c  unctions_prefix,
+00012420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012430: 2069 676e 6f72 655f 636f 6d70 6f6e 656e   ignore_componen
+00012440: 7473 5f70 7265 6669 783d 6967 6e6f 7265  ts_prefix=ignore
+00012450: 5f63 6f6d 706f 6e65 6e74 735f 7072 6566  _components_pref
+00012460: 6978 2c0a 2020 2020 2020 2020 2020 2020  ix,.            
+00012470: 290a 2020 2020 2020 2020 2020 2020 645b  ).            d[
+00012480: 2263 656c 6c73 225d 203d 2063 6c65 616e  "cells"] = clean
+00012490: 5f64 6963 7428 6365 6c6c 7329 0a0a 2020  _dict(cells)..  
+000124a0: 2020 2020 2020 645b 226e 616d 6522 5d20        d["name"] 
+000124b0: 3d20 7365 6c66 2e6e 616d 650a 2020 2020  = self.name.    
+000124c0: 2020 2020 645b 2273 6574 7469 6e67 7322      d["settings"
+000124d0: 5d20 3d20 636c 6561 6e5f 6469 6374 2864  ] = clean_dict(d
+000124e0: 6963 7428 7365 6c66 2e73 6574 7469 6e67  ict(self.setting
+000124f0: 7329 290a 2020 2020 2020 2020 7265 7475  s)).        retu
+00012500: 726e 2064 0a0a 2020 2020 6465 6620 746f  rn d..    def to
+00012510: 5f79 616d 6c28 7365 6c66 2c20 2a2a 6b77  _yaml(self, **kw
+00012520: 6172 6773 2920 2d3e 2073 7472 3a0a 2020  args) -> str:.  
+00012530: 2020 2020 2020 2222 2257 7269 7465 2044        """Write D
+00012540: 6963 7420 7265 7072 6573 656e 7461 7469  ict representati
+00012550: 6f6e 206f 6620 6120 636f 6d70 6f6e 656e  on of a componen
+00012560: 7420 696e 2059 414d 4c20 666f 726d 6174  t in YAML format
+00012570: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00012580: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
+00012590: 6f72 655f 636f 6d70 6f6e 656e 7473 5f70  ore_components_p
+000125a0: 7265 6669 783a 2066 6f72 2063 6f6d 706f  refix: for compo
+000125b0: 6e65 6e74 7320 746f 2069 676e 6f72 6520  nents to ignore 
+000125c0: 7768 656e 2065 7870 6f72 7469 6e67 2e0a  when exporting..
+000125d0: 2020 2020 2020 2020 2020 2020 6967 6e6f              igno
+000125e0: 7265 5f66 756e 6374 696f 6e73 5f70 7265  re_functions_pre
+000125f0: 6669 783a 2066 6f72 2066 756e 6374 696f  fix: for functio
+00012600: 6e73 2074 6f20 6967 6e6f 7265 2077 6865  ns to ignore whe
+00012610: 6e20 6578 706f 7274 696e 672e 0a20 2020  n exporting..   
+00012620: 2020 2020 2020 2020 2077 6974 685f 6365           with_ce
+00012630: 6c6c 733a 2077 7269 7465 2063 656c 6c73  lls: write cells
+00012640: 2072 6563 7572 7369 7665 6c79 2e0a 2020   recursively..  
+00012650: 2020 2020 2020 2020 2020 7769 7468 5f70            with_p
+00012660: 6f72 7473 3a20 7772 6974 6520 706f 7274  orts: write port
+00012670: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2020   information..  
+00012680: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012690: 2020 7265 7475 726e 2079 616d 6c2e 6475    return yaml.du
+000126a0: 6d70 2863 6c65 616e 5f64 6963 7428 7365  mp(clean_dict(se
+000126b0: 6c66 2e74 6f5f 6469 6374 282a 2a6b 7761  lf.to_dict(**kwa
+000126c0: 7267 7329 2929 0a0a 2020 2020 6465 6620  rgs)))..    def 
+000126d0: 6175 746f 5f72 656e 616d 655f 706f 7274  auto_rename_port
+000126e0: 7328 7365 6c66 2c20 2a2a 6b77 6172 6773  s(self, **kwargs
+000126f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00012700: 2020 2022 2222 5265 6e61 6d65 2070 6f72     """Rename por
+00012710: 7473 2062 7920 6f72 6965 6e74 6174 696f  ts by orientatio
+00012720: 6e20 4e53 4557 2028 6e6f 7274 682c 2073  n NSEW (north, s
+00012730: 6f75 7468 2c20 6561 7374 2c20 7765 7374  outh, east, west
+00012740: 292e 0a0a 2020 2020 2020 2020 4b65 7977  )...        Keyw
+00012750: 6f72 6420 4172 6773 3a0a 2020 2020 2020  ord Args:.      
+00012760: 2020 2020 2020 6675 6e63 7469 6f6e 3a20        function: 
+00012770: 746f 2072 656e 616d 6520 706f 7274 732e  to rename ports.
+00012780: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012790: 6563 745f 706f 7274 735f 6f70 7469 6361  ect_ports_optica
+000127a0: 6c3a 2074 6f20 7365 6c65 6374 206f 7074  l: to select opt
+000127b0: 6963 616c 2070 6f72 7473 2e0a 2020 2020  ical ports..    
+000127c0: 2020 2020 2020 2020 7365 6c65 6374 5f70          select_p
+000127d0: 6f72 7473 5f65 6c65 6374 7269 6361 6c3a  orts_electrical:
+000127e0: 2074 6f20 7365 6c65 6374 2065 6c65 6374   to select elect
+000127f0: 7269 6361 6c20 706f 7274 732e 0a20 2020  rical ports..   
+00012800: 2020 2020 2020 2020 2070 7265 6669 785f           prefix_
+00012810: 6f70 7469 6361 6c3a 2070 7265 6669 782e  optical: prefix.
+00012820: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
+00012830: 6669 785f 656c 6563 7472 6963 616c 3a20  fix_electrical: 
+00012840: 7072 6566 6978 2e0a 0a20 2020 2020 2020  prefix...       
+00012850: 202e 2e20 636f 6465 3a3a 0a0a 2020 2020   .. code::..    
+00012860: 2020 2020 2020 2020 2020 2020 2020 3320                3 
+00012870: 2034 0a20 2020 2020 2020 2020 2020 2020   4.             
+00012880: 2020 2020 5f7c 5f5f 7c5f 0a20 2020 2020      _|__|_.     
+00012890: 2020 2020 2020 2020 3220 2d7c 2020 2020          2 -|    
+000128a0: 2020 7c2d 2035 0a20 2020 2020 2020 2020    |- 5.         
+000128b0: 2020 2020 2020 207c 2020 2020 2020 7c0a         |      |.
+000128c0: 2020 2020 2020 2020 2020 2020 2031 202d               1 -
+000128d0: 7c5f 5f5f 5f5f 5f7c 2d20 360a 2020 2020  |______|- 6.    
+000128e0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000128f0: 207c 0a20 2020 2020 2020 2020 2020 2020   |.             
+00012900: 2020 2020 2038 2020 370a 2020 2020 2020       8  7.      
+00012910: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+00012920: 6c66 2e69 735f 756e 6c6f 636b 6564 2829  lf.is_unlocked()
+00012930: 0a20 2020 2020 2020 2061 7574 6f5f 7265  .        auto_re
+00012940: 6e61 6d65 5f70 6f72 7473 2873 656c 662c  name_ports(self,
+00012950: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
+00012960: 6465 6620 6175 746f 5f72 656e 616d 655f  def auto_rename_
+00012970: 706f 7274 735f 636f 756e 7465 725f 636c  ports_counter_cl
+00012980: 6f63 6b77 6973 6528 7365 6c66 2c20 2a2a  ockwise(self, **
+00012990: 6b77 6172 6773 2920 2d3e 204e 6f6e 653a  kwargs) -> None:
+000129a0: 0a20 2020 2020 2020 2073 656c 662e 6973  .        self.is
+000129b0: 5f75 6e6c 6f63 6b65 6428 290a 2020 2020  _unlocked().    
+000129c0: 2020 2020 6175 746f 5f72 656e 616d 655f      auto_rename_
+000129d0: 706f 7274 735f 636f 756e 7465 725f 636c  ports_counter_cl
+000129e0: 6f63 6b77 6973 6528 7365 6c66 2c20 2a2a  ockwise(self, **
+000129f0: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
+00012a00: 2061 7574 6f5f 7265 6e61 6d65 5f70 6f72   auto_rename_por
+00012a10: 7473 5f6c 6179 6572 5f6f 7269 656e 7461  ts_layer_orienta
+00012a20: 7469 6f6e 2873 656c 662c 202a 2a6b 7761  tion(self, **kwa
+00012a30: 7267 7329 202d 3e20 4e6f 6e65 3a0a 2020  rgs) -> None:.  
+00012a40: 2020 2020 2020 7365 6c66 2e69 735f 756e        self.is_un
+00012a50: 6c6f 636b 6564 2829 0a20 2020 2020 2020  locked().       
+00012a60: 2061 7574 6f5f 7265 6e61 6d65 5f70 6f72   auto_rename_por
+00012a70: 7473 5f6c 6179 6572 5f6f 7269 656e 7461  ts_layer_orienta
+00012a80: 7469 6f6e 2873 656c 662c 202a 2a6b 7761  tion(self, **kwa
+00012a90: 7267 7329 0a0a 2020 2020 6465 6620 6175  rgs)..    def au
+00012aa0: 746f 5f72 656e 616d 655f 706f 7274 735f  to_rename_ports_
+00012ab0: 6f72 6965 6e74 6174 696f 6e28 7365 6c66  orientation(self
+00012ac0: 2c20 2a2a 6b77 6172 6773 2920 2d3e 204e  , **kwargs) -> N
+00012ad0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00012ae0: 5265 6e61 6d65 2070 6f72 7473 2062 7920  Rename ports by 
+00012af0: 6f72 6965 6e74 6174 696f 6e20 4e53 4557  orientation NSEW
+00012b00: 2028 6e6f 7274 682c 2073 6f75 7468 2c20   (north, south, 
+00012b10: 6561 7374 2c20 7765 7374 292e 0a0a 2020  east, west)...  
+00012b20: 2020 2020 2020 4b65 7977 6f72 6420 4172        Keyword Ar
+00012b30: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00012b40: 6675 6e63 7469 6f6e 3a20 746f 2072 656e  function: to ren
+00012b50: 616d 6520 706f 7274 732e 0a20 2020 2020  ame ports..     
+00012b60: 2020 2020 2020 2073 656c 6563 745f 706f         select_po
+00012b70: 7274 735f 6f70 7469 6361 6c3a 2074 6f20  rts_optical: to 
+00012b80: 7365 6c65 6374 2070 6f72 7473 2e0a 2020  select ports..  
+00012b90: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+00012ba0: 5f70 6f72 7473 5f65 6c65 6374 7269 6361  _ports_electrica
+00012bb0: 6c3a 0a20 2020 2020 2020 2020 2020 2070  l:.            p
+00012bc0: 7265 6669 785f 6f70 7469 6361 6c3a 0a20  refix_optical:. 
+00012bd0: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00012be0: 785f 656c 6563 7472 6963 616c 3a0a 0a20  x_electrical:.. 
+00012bf0: 2020 2020 2020 202e 2e20 636f 6465 3a3a         .. code::
+00012c00: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012c10: 2020 204e 3020 204e 310a 2020 2020 2020     N0  N1.      
+00012c20: 2020 2020 2020 2020 2020 207c 5f5f 5f7c             |___|
+00012c30: 5f0a 2020 2020 2020 2020 2020 2020 5731  _.            W1
+00012c40: 202d 7c20 2020 2020 207c 2d20 4531 0a20   -|      |- E1. 
+00012c50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00012c60: 2020 2020 2020 7c0a 2020 2020 2020 2020        |.        
+00012c70: 2020 2020 5730 202d 7c5f 5f5f 5f5f 5f7c      W0 -|______|
+00012c80: 2d20 4530 0a20 2020 2020 2020 2020 2020  - E0.           
+00012c90: 2020 2020 2020 7c20 2020 7c0a 2020 2020        |   |.    
+00012ca0: 2020 2020 2020 2020 2020 2020 5330 2020              S0  
+00012cb0: 2053 310a 2020 2020 2020 2020 2222 220a   S1.        """.
+00012cc0: 2020 2020 2020 2020 7365 6c66 2e69 735f          self.is_
+00012cd0: 756e 6c6f 636b 6564 2829 0a20 2020 2020  unlocked().     
+00012ce0: 2020 2061 7574 6f5f 7265 6e61 6d65 5f70     auto_rename_p
+00012cf0: 6f72 7473 5f6f 7269 656e 7461 7469 6f6e  orts_orientation
+00012d00: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
+00012d10: 0a0a 2020 2020 6465 6620 6d6f 7665 280a  ..    def move(.
+00012d20: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00012d30: 2020 2020 2020 6f72 6967 696e 3a20 466c        origin: Fl
+00012d40: 6f61 7432 203d 2028 302c 2030 292c 0a20  oat2 = (0, 0),. 
+00012d50: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+00012d60: 6f6e 3a20 466c 6f61 7432 207c 204e 6f6e  on: Float2 | Non
+00012d70: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+00012d80: 2020 6178 6973 3a20 4178 6973 207c 204e    axis: Axis | N
+00012d90: 6f6e 6520 3d20 4e6f 6e65 2c0a 2020 2020  one = None,.    
+00012da0: 2920 2d3e 2043 6f6d 706f 6e65 6e74 3a0a  ) -> Component:.
+00012db0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00012dc0: 6e73 206e 6577 2043 6f6d 706f 6e65 6e74  ns new Component
+00012dd0: 2077 6974 6820 6120 6d6f 7665 6420 7265   with a moved re
+00012de0: 6665 7265 6e63 6520 746f 2074 6865 206f  ference to the o
+00012df0: 7269 6769 6e61 6c2e 0a0a 2020 2020 2020  riginal...      
+00012e00: 2020 636f 6d70 6f6e 656e 742e 0a0a 2020    component...  
+00012e10: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00012e20: 2020 2020 2020 2020 6f72 6967 696e 3a20          origin: 
+00012e30: 6f66 2063 6f6d 706f 6e65 6e74 2e0a 2020  of component..  
+00012e40: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+00012e50: 6174 696f 6e3a 2078 2c20 792e 0a20 2020  ation: x, y..   
+00012e60: 2020 2020 2020 2020 2061 7869 733a 2078           axis: x
+00012e70: 206f 7220 792e 0a20 2020 2020 2020 2022   or y..        "
+00012e80: 2222 0a20 2020 2020 2020 2072 6169 7365  "".        raise
+00012e90: 2056 616c 7565 4572 726f 7228 6d6f 7665   ValueError(move
+00012ea0: 5f65 7272 6f72 5f6d 6573 7361 6765 290a  _error_message).
+00012eb0: 0a20 2020 2064 6566 206d 6972 726f 7228  .    def mirror(
+00012ec0: 7365 6c66 2c20 7031 3a20 466c 6f61 7432  self, p1: Float2
+00012ed0: 203d 2028 302c 2031 292c 2070 323a 2046   = (0, 1), p2: F
+00012ee0: 6c6f 6174 3220 3d20 2830 2c20 3029 2c20  loat2 = (0, 0), 
+00012ef0: 2a2a 6b77 6172 6773 2920 2d3e 2043 6f6d  **kwargs) -> Com
+00012f00: 706f 6e65 6e74 3a0a 2020 2020 2020 2020  ponent:.        
+00012f10: 2222 2252 6574 7572 6e73 206e 6577 2043  """Returns new C
+00012f20: 6f6d 706f 6e65 6e74 2077 6974 6820 6120  omponent with a 
+00012f30: 6d69 7272 6f72 6564 2072 6566 6572 656e  mirrored referen
+00012f40: 6365 2e0a 0a20 2020 2020 2020 2041 7267  ce...        Arg
+00012f50: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+00012f60: 313a 2066 6972 7374 2070 6f69 6e74 2074  1: first point t
+00012f70: 6f20 6465 6669 6e65 206d 6972 726f 7220  o define mirror 
+00012f80: 6178 6973 2e0a 2020 2020 2020 2020 2020  axis..          
+00012f90: 2020 7032 3a20 7365 636f 6e64 2070 6f69    p2: second poi
+00012fa0: 6e74 2074 6f20 6465 6669 6e65 206d 6972  nt to define mir
+00012fb0: 726f 7220 6178 6973 2e0a 2020 2020 2020  ror axis..      
+00012fc0: 2020 2222 220a 2020 2020 2020 2020 6672    """.        fr
+00012fd0: 6f6d 2067 6473 6661 6374 6f72 792e 6675  om gdsfactory.fu
+00012fe0: 6e63 7469 6f6e 7320 696d 706f 7274 206d  nctions import m
+00012ff0: 6972 726f 720a 0a20 2020 2020 2020 2072  irror..        r
+00013000: 6574 7572 6e20 6d69 7272 6f72 2863 6f6d  eturn mirror(com
+00013010: 706f 6e65 6e74 3d73 656c 662c 2070 313d  ponent=self, p1=
+00013020: 7031 2c20 7032 3d70 322c 202a 2a6b 7761  p1, p2=p2, **kwa
+00013030: 7267 7329 0a0a 2020 2020 6465 6620 726f  rgs)..    def ro
+00013040: 7461 7465 2873 656c 662c 2061 6e67 6c65  tate(self, angle
+00013050: 3a20 666c 6f61 7420 3d20 3930 2c20 2a2a  : float = 90, **
+00013060: 6b77 6172 6773 2920 2d3e 2043 6f6d 706f  kwargs) -> Compo
+00013070: 6e65 6e74 3a0a 2020 2020 2020 2020 2222  nent:.        ""
+00013080: 2252 6574 7572 6e73 206e 6577 2063 6f6d  "Returns new com
+00013090: 706f 6e65 6e74 2077 6974 6820 6120 726f  ponent with a ro
+000130a0: 7461 7465 6420 7265 6665 7265 6e63 6520  tated reference 
+000130b0: 746f 2074 6865 206f 7269 6769 6e61 6c2e  to the original.
+000130c0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000130d0: 2020 2020 2020 2020 2020 2020 616e 676c              angl
+000130e0: 653a 2069 6e20 6465 6772 6565 732e 0a20  e: in degrees.. 
+000130f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013100: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
+00013110: 7279 2e66 756e 6374 696f 6e73 2069 6d70  ry.functions imp
+00013120: 6f72 7420 726f 7461 7465 0a0a 2020 2020  ort rotate..    
+00013130: 2020 2020 7265 7475 726e 2072 6f74 6174      return rotat
+00013140: 6528 636f 6d70 6f6e 656e 743d 7365 6c66  e(component=self
+00013150: 2c20 616e 676c 653d 616e 676c 652c 202a  , angle=angle, *
+00013160: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
+00013170: 6620 6164 645f 7061 6464 696e 6728 7365  f add_padding(se
+00013180: 6c66 2c20 2a2a 6b77 6172 6773 2920 2d3e  lf, **kwargs) ->
+00013190: 2043 6f6d 706f 6e65 6e74 3a0a 2020 2020   Component:.    
+000131a0: 2020 2020 2222 2252 6574 7572 6e73 2073      """Returns s
+000131b0: 616d 6520 636f 6d70 6f6e 656e 7420 7769  ame component wi
+000131c0: 7468 2070 6164 6469 6e67 2e0a 0a20 2020  th padding...   
+000131d0: 2020 2020 204b 6579 776f 7264 2041 7267       Keyword Arg
+000131e0: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+000131f0: 6f6d 706f 6e65 6e74 3a20 666f 7220 7061  omponent: for pa
+00013200: 6464 696e 672e 0a20 2020 2020 2020 2020  dding..         
+00013210: 2020 206c 6179 6572 733a 206c 6973 7420     layers: list 
+00013220: 6f66 206c 6179 6572 732e 0a20 2020 2020  of layers..     
+00013230: 2020 2020 2020 2073 7566 6669 7820 666f         suffix fo
+00013240: 7220 6e61 6d65 2e0a 2020 2020 2020 2020  r name..        
+00013250: 2020 2020 6465 6661 756c 743a 2064 6566      default: def
+00013260: 6175 6c74 2070 6164 6469 6e67 2028 3530  ault padding (50
+00013270: 756d 292e 0a20 2020 2020 2020 2020 2020  um)..           
+00013280: 2074 6f70 3a20 6e6f 7274 6820 7061 6464   top: north padd
+00013290: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
+000132a0: 2062 6f74 746f 6d3a 2073 6f75 7468 2070   bottom: south p
+000132b0: 6164 6469 6e67 2e0a 2020 2020 2020 2020  adding..        
+000132c0: 2020 2020 7269 6768 743a 2065 6173 7420      right: east 
+000132d0: 7061 6464 696e 672e 0a20 2020 2020 2020  padding..       
+000132e0: 2020 2020 206c 6566 743a 2077 6573 7420       left: west 
+000132f0: 7061 6464 696e 672e 0a20 2020 2020 2020  padding..       
+00013300: 2022 2222 0a20 2020 2020 2020 2066 726f   """.        fro
+00013310: 6d20 6764 7366 6163 746f 7279 2e61 6464  m gdsfactory.add
+00013320: 5f70 6164 6469 6e67 2069 6d70 6f72 7420  _padding import 
+00013330: 6164 645f 7061 6464 696e 670a 0a20 2020  add_padding..   
+00013340: 2020 2020 2072 6574 7572 6e20 6164 645f       return add_
+00013350: 7061 6464 696e 6728 636f 6d70 6f6e 656e  padding(componen
+00013360: 743d 7365 6c66 2c20 2a2a 6b77 6172 6773  t=self, **kwargs
+00013370: 290a 0a20 2020 2064 6566 2061 6273 6f72  )..    def absor
+00013380: 6228 7365 6c66 2c20 7265 6665 7265 6e63  b(self, referenc
+00013390: 6529 202d 3e20 436f 6d70 6f6e 656e 743a  e) -> Component:
+000133a0: 0a20 2020 2020 2020 2022 2222 4162 736f  .        """Abso
+000133b0: 7262 7320 706f 6c79 676f 6e73 2066 726f  rbs polygons fro
+000133c0: 6d20 436f 6d70 6f6e 656e 7452 6566 6572  m ComponentRefer
+000133d0: 656e 6365 2069 6e74 6f20 436f 6d70 6f6e  ence into Compon
+000133e0: 656e 742e 0a0a 2020 2020 2020 2020 4465  ent...        De
+000133f0: 7374 726f 7973 2074 6865 2072 6566 6572  stroys the refer
+00013400: 656e 6365 2069 6e20 7468 6520 7072 6f63  ence in the proc
+00013410: 6573 7320 6275 7420 6b65 6570 696e 6720  ess but keeping 
+00013420: 7468 6520 706f 6c79 676f 6e20 6765 6f6d  the polygon geom
+00013430: 6574 7279 2e0a 0a20 2020 2020 2020 2041  etry...        A
+00013440: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00013450: 2072 6566 6572 656e 6365 3a20 436f 6d70   reference: Comp
+00013460: 6f6e 656e 7452 6566 6572 656e 6365 2074  onentReference t
+00013470: 6f20 6265 2061 6273 6f72 6265 6420 696e  o be absorbed in
+00013480: 746f 2074 6865 2043 6f6d 706f 6e65 6e74  to the Component
+00013490: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000134a0: 2020 2020 2020 6966 2072 6566 6572 656e        if referen
+000134b0: 6365 206e 6f74 2069 6e20 7365 6c66 2e72  ce not in self.r
+000134c0: 6566 6572 656e 6365 733a 0a20 2020 2020  eferences:.     
+000134d0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+000134e0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+000134f0: 2020 2020 2020 2020 2022 5468 6520 7265           "The re
+00013500: 6665 7265 6e63 6520 796f 7520 6173 6b65  ference you aske
+00013510: 6420 746f 2061 6273 6f72 6220 646f 6573  d to absorb does
+00013520: 206e 6f74 2065 7869 7374 2069 6e20 7468   not exist in th
+00013530: 6973 2043 6f6d 706f 6e65 6e74 2e22 0a20  is Component.". 
+00013540: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00013550: 2020 2020 2072 6566 5f70 6f6c 7967 6f6e       ref_polygon
+00013560: 7320 3d20 7265 6665 7265 6e63 652e 6765  s = reference.ge
+00013570: 745f 706f 6c79 676f 6e73 280a 2020 2020  t_polygons(.    
+00013580: 2020 2020 2020 2020 6279 5f73 7065 633d          by_spec=
+00013590: 4661 6c73 652c 2069 6e63 6c75 6465 5f70  False, include_p
+000135a0: 6174 6873 3d46 616c 7365 2c20 6173 5f61  aths=False, as_a
+000135b0: 7272 6179 3d46 616c 7365 0a20 2020 2020  rray=False.     
+000135c0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+000135d0: 662e 5f61 6464 5f70 6f6c 7967 6f6e 7328  f._add_polygons(
+000135e0: 2a72 6566 5f70 6f6c 7967 6f6e 7329 0a0a  *ref_polygons)..
+000135f0: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
+00013600: 2872 6566 6572 656e 6365 2e67 6574 5f6c  (reference.get_l
+00013610: 6162 656c 7328 2929 0a20 2020 2020 2020  abels()).       
+00013620: 2073 656c 662e 6164 6428 7265 6665 7265   self.add(refere
+00013630: 6e63 652e 6765 745f 7061 7468 7328 2929  nce.get_paths())
+00013640: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00013650: 6d6f 7665 2872 6566 6572 656e 6365 290a  move(reference).
+00013660: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00013670: 656c 660a 0a20 2020 2064 6566 2072 656d  elf..    def rem
+00013680: 6f76 6528 7365 6c66 2c20 6974 656d 7329  ove(self, items)
+00013690: 3a0a 2020 2020 2020 2020 2222 2252 656d  :.        """Rem
+000136a0: 6f76 6573 2069 7465 6d73 2066 726f 6d20  oves items from 
+000136b0: 6120 436f 6d70 6f6e 656e 742c 2077 6869  a Component, whi
+000136c0: 6368 2063 616e 2069 6e63 6c75 6465 2050  ch can include P
+000136d0: 6f72 7473 2c20 506f 6c79 676f 6e53 6574  orts, PolygonSet
+000136e0: 7320 5c0a 2020 2020 2020 2020 4365 6c6c  s \.        Cell
+000136f0: 5265 6665 7265 6e63 6573 2c20 436f 6d70  References, Comp
+00013700: 6f6e 656e 7452 6566 6572 656e 6365 7320  onentReferences 
+00013710: 616e 6420 4c61 6265 6c73 2e0a 0a20 2020  and Labels...   
+00013720: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00013730: 2020 2020 2020 2069 7465 6d73 3a20 6c69         items: li
+00013740: 7374 206f 6620 4974 656d 7320 746f 2062  st of Items to b
+00013750: 6520 7265 6d6f 7665 6420 6672 6f6d 2074  e removed from t
+00013760: 6865 2043 6f6d 706f 6e65 6e74 2e0a 2020  he Component..  
+00013770: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013780: 2020 6966 206e 6f74 2068 6173 6174 7472    if not hasattr
+00013790: 2869 7465 6d73 2c20 225f 5f69 7465 725f  (items, "__iter_
+000137a0: 5f22 293a 0a20 2020 2020 2020 2020 2020  _"):.           
+000137b0: 2069 7465 6d73 203d 205b 6974 656d 735d   items = [items]
+000137c0: 0a20 2020 2020 2020 2066 6f72 2069 7465  .        for ite
+000137d0: 6d20 696e 2069 7465 6d73 3a0a 2020 2020  m in items:.    
+000137e0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+000137f0: 7461 6e63 6528 6974 656d 2c20 506f 7274  tance(item, Port
+00013800: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00013810: 2020 2073 656c 662e 706f 7274 7320 3d20     self.ports = 
+00013820: 7b6b 3a20 7620 666f 7220 6b2c 2076 2069  {k: v for k, v i
+00013830: 6e20 7365 6c66 2e70 6f72 7473 2e69 7465  n self.ports.ite
+00013840: 6d73 2829 2069 6620 7620 213d 2069 7465  ms() if v != ite
+00013850: 6d7d 0a20 2020 2020 2020 2020 2020 2065  m}.            e
+00013860: 6c69 6620 6973 696e 7374 616e 6365 2869  lif isinstance(i
+00013870: 7465 6d2c 2067 6473 746b 2e52 6566 6572  tem, gdstk.Refer
+00013880: 656e 6365 293a 0a20 2020 2020 2020 2020  ence):.         
+00013890: 2020 2020 2020 2073 656c 662e 5f63 656c         self._cel
+000138a0: 6c2e 7265 6d6f 7665 2869 7465 6d29 0a20  l.remove(item). 
+000138b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000138c0: 7465 6d2e 6f77 6e65 7220 3d20 4e6f 6e65  tem.owner = None
+000138d0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+000138e0: 6620 6973 696e 7374 616e 6365 2869 7465  f isinstance(ite
+000138f0: 6d2c 2043 6f6d 706f 6e65 6e74 5265 6665  m, ComponentRefe
+00013900: 7265 6e63 6529 3a0a 2020 2020 2020 2020  rence):.        
+00013910: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00013920: 6572 656e 6365 732e 7265 6d6f 7665 2869  erences.remove(i
+00013930: 7465 6d29 0a20 2020 2020 2020 2020 2020  tem).           
+00013940: 2020 2020 2073 656c 662e 5f63 656c 6c2e       self._cell.
+00013950: 7265 6d6f 7665 2869 7465 6d2e 5f72 6566  remove(item._ref
+00013960: 6572 656e 6365 290a 2020 2020 2020 2020  erence).        
+00013970: 2020 2020 2020 2020 6974 656d 2e6f 776e          item.own
+00013980: 6572 203d 204e 6f6e 650a 2020 2020 2020  er = None.      
+00013990: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000139a0: 6e61 6d65 645f 7265 6665 7265 6e63 6573  named_references
+000139b0: 2e70 6f70 2869 7465 6d2e 6e61 6d65 290a  .pop(item.name).
+000139c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000139d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000139e0: 2020 7365 6c66 2e5f 6365 6c6c 2e72 656d    self._cell.rem
+000139f0: 6f76 6528 6974 656d 290a 0a20 2020 2020  ove(item)..     
+00013a00: 2020 2073 656c 662e 5f62 625f 7661 6c69     self._bb_vali
+00013a10: 6420 3d20 4661 6c73 650a 2020 2020 2020  d = False.      
+00013a20: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
+00013a30: 2020 2064 6566 2068 6173 685f 6765 6f6d     def hash_geom
+00013a40: 6574 7279 2873 656c 662c 2070 7265 6369  etry(self, preci
+00013a50: 7369 6f6e 3a20 666c 6f61 7420 3d20 3165  sion: float = 1e
+00013a60: 2d34 2920 2d3e 2073 7472 3a0a 2020 2020  -4) -> str:.    
+00013a70: 2020 2020 2222 2252 6574 7572 6e73 2061      """Returns a
+00013a80: 6e20 5348 4131 2068 6173 6820 6f66 2074  n SHA1 hash of t
+00013a90: 6865 2067 656f 6d65 7472 7920 696e 2074  he geometry in t
+00013aa0: 6865 2043 6f6d 706f 6e65 6e74 2e0a 0a20  he Component... 
+00013ab0: 2020 2020 2020 2046 6f72 2065 6163 6820         For each 
+00013ac0: 6c61 7965 722c 2065 6163 6820 706f 6c79  layer, each poly
+00013ad0: 676f 6e20 6973 2069 6e64 6976 6964 7561  gon is individua
+00013ae0: 6c6c 7920 6861 7368 6564 2061 6e64 2074  lly hashed and t
+00013af0: 6865 6e20 7468 6520 706f 6c79 676f 6e20  hen the polygon 
+00013b00: 6861 7368 6573 0a20 2020 2020 2020 2061  hashes.        a
+00013b10: 7265 2073 6f72 7465 642c 2074 6f20 656e  re sorted, to en
+00013b20: 7375 7265 2074 6865 2068 6173 6820 7374  sure the hash st
+00013b30: 6179 7320 636f 6e73 7461 6e74 2072 6567  ays constant reg
+00013b40: 6172 646c 6573 7320 6f66 2074 6865 206f  ardless of the o
+00013b50: 7264 6572 696e 670a 2020 2020 2020 2020  rdering.        
+00013b60: 7468 6520 706f 6c79 676f 6e73 2e20 2053  the polygons.  S
+00013b70: 696d 696c 6172 6c79 2c20 7468 6520 6c61  imilarly, the la
+00013b80: 7965 7273 2061 7265 2073 6f72 7465 6420  yers are sorted 
+00013b90: 6279 2028 6c61 7965 722c 2064 6174 6174  by (layer, datat
+00013ba0: 7970 6529 2e0a 0a20 2020 2020 2020 2041  ype)...        A
+00013bb0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00013bc0: 2070 7265 6369 7369 6f6e 3a20 526f 756e   precision: Roun
+00013bd0: 6469 6e67 2070 7265 6369 7369 6f6e 2066  ding precision f
+00013be0: 6f72 2074 6865 2074 6865 206f 626a 6563  or the the objec
+00013bf0: 7473 2069 6e20 7468 6520 436f 6d70 6f6e  ts in the Compon
+00013c00: 656e 742e 0a20 2020 2020 2020 2020 2020  ent..           
+00013c10: 2020 2020 2046 6f72 2069 6e73 7461 6e63       For instanc
+00013c20: 652c 2061 2070 7265 6369 7369 6f6e 206f  e, a precision o
+00013c30: 6620 3165 2d32 2077 696c 6c20 726f 756e  f 1e-2 will roun
+00013c40: 6420 6120 706f 696e 7420 6174 0a20 2020  d a point at.   
+00013c50: 2020 2020 2020 2020 2020 2020 2028 302e               (0.
+00013c60: 3132 342c 2031 2e37 3438 2920 746f 2028  124, 1.748) to (
+00013c70: 302e 3132 2c20 312e 3735 292e 0a0a 2020  0.12, 1.75)...  
+00013c80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013c90: 2020 706f 6c79 676f 6e73 5f62 795f 7370    polygons_by_sp
+00013ca0: 6563 203d 2073 656c 662e 6765 745f 706f  ec = self.get_po
+00013cb0: 6c79 676f 6e73 2862 795f 7370 6563 3d54  lygons(by_spec=T
+00013cc0: 7275 652c 2061 735f 6172 7261 793d 4661  rue, as_array=Fa
+00013cd0: 6c73 6529 0a20 2020 2020 2020 206c 6179  lse).        lay
+00013ce0: 6572 7320 3d20 6e70 2e61 7272 6179 286c  ers = np.array(l
+00013cf0: 6973 7428 706f 6c79 676f 6e73 5f62 795f  ist(polygons_by_
+00013d00: 7370 6563 2e6b 6579 7328 2929 290a 2020  spec.keys())).  
+00013d10: 2020 2020 2020 736f 7274 6564 5f6c 6179        sorted_lay
+00013d20: 6572 7320 3d20 6c61 7965 7273 5b6e 702e  ers = layers[np.
+00013d30: 6c65 7873 6f72 7428 286c 6179 6572 735b  lexsort((layers[
+00013d40: 3a2c 2030 5d2c 206c 6179 6572 735b 3a2c  :, 0], layers[:,
+00013d50: 2031 5d29 295d 0a0a 2020 2020 2020 2020   1]))]..        
+00013d60: 6669 6e61 6c5f 6861 7368 203d 2068 6173  final_hash = has
+00013d70: 686c 6962 2e73 6861 3128 290a 2020 2020  hlib.sha1().    
+00013d80: 2020 2020 666f 7220 6c61 7965 7220 696e      for layer in
+00013d90: 2073 6f72 7465 645f 6c61 7965 7273 3a0a   sorted_layers:.
+00013da0: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+00013db0: 725f 6861 7368 203d 2068 6173 686c 6962  r_hash = hashlib
+00013dc0: 2e73 6861 3128 6c61 7965 722e 6173 7479  .sha1(layer.asty
+00013dd0: 7065 286e 702e 696e 7436 3429 292e 6469  pe(np.int64)).di
+00013de0: 6765 7374 2829 0a20 2020 2020 2020 2020  gest().         
+00013df0: 2020 2070 6f6c 7967 6f6e 7320 3d20 706f     polygons = po
+00013e00: 6c79 676f 6e73 5f62 795f 7370 6563 5b74  lygons_by_spec[t
+00013e10: 7570 6c65 286c 6179 6572 295d 0a20 2020  uple(layer)].   
+00013e20: 2020 2020 2020 2020 2070 6f6c 7967 6f6e           polygon
+00013e30: 7320 3d20 5b5f 726e 6428 702e 706f 696e  s = [_rnd(p.poin
+00013e40: 7473 2c20 7072 6563 6973 696f 6e29 2066  ts, precision) f
+00013e50: 6f72 2070 2069 6e20 706f 6c79 676f 6e73  or p in polygons
+00013e60: 5d0a 2020 2020 2020 2020 2020 2020 706f  ].            po
+00013e70: 6c79 676f 6e5f 6861 7368 6573 203d 206e  lygon_hashes = n
+00013e80: 702e 736f 7274 285b 6861 7368 6c69 622e  p.sort([hashlib.
+00013e90: 7368 6131 2870 292e 6469 6765 7374 2829  sha1(p).digest()
+00013ea0: 2066 6f72 2070 2069 6e20 706f 6c79 676f   for p in polygo
+00013eb0: 6e73 5d29 0a20 2020 2020 2020 2020 2020  ns]).           
+00013ec0: 2066 696e 616c 5f68 6173 682e 7570 6461   final_hash.upda
+00013ed0: 7465 286c 6179 6572 5f68 6173 6829 0a20  te(layer_hash). 
+00013ee0: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+00013ef0: 6820 696e 2070 6f6c 7967 6f6e 5f68 6173  h in polygon_has
+00013f00: 6865 733a 0a20 2020 2020 2020 2020 2020  hes:.           
+00013f10: 2020 2020 2066 696e 616c 5f68 6173 682e       final_hash.
+00013f20: 7570 6461 7465 2870 6829 0a0a 2020 2020  update(ph)..    
+00013f30: 2020 2020 7265 7475 726e 2066 696e 616c      return final
+00013f40: 5f68 6173 682e 6865 7864 6967 6573 7428  _hash.hexdigest(
+00013f50: 290a 0a20 2020 2064 6566 2067 6574 5f6c  )..    def get_l
+00013f60: 6162 656c 7328 0a20 2020 2020 2020 2073  abels(.        s
+00013f70: 656c 662c 2061 7070 6c79 5f72 6570 6574  elf, apply_repet
+00013f80: 6974 696f 6e73 3d54 7275 652c 2064 6570  itions=True, dep
+00013f90: 7468 3a20 696e 7420 7c20 4e6f 6e65 203d  th: int | None =
+00013fa0: 204e 6f6e 652c 206c 6179 6572 3d4e 6f6e   None, layer=Non
+00013fb0: 650a 2020 2020 2920 2d3e 206c 6973 745b  e.    ) -> list[
+00013fc0: 4c61 6265 6c5d 3a0a 2020 2020 2020 2020  Label]:.        
+00013fd0: 2222 2252 6574 7572 6e20 6c61 6265 6c73  """Return labels
+00013fe0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00013ff0: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+00014000: 6c79 5f72 6570 6574 6974 696f 6e73 3a2e  ly_repetitions:.
+00014010: 0a20 2020 2020 2020 2020 2020 2064 6570  .            dep
+00014020: 7468 3a20 4e6f 6e65 2072 6574 7572 6e73  th: None returns
+00014030: 2061 6c6c 206c 6162 656c 7320 616e 6420   all labels and 
+00014040: 3020 746f 7020 6c65 7665 6c2e 0a20 2020  0 top level..   
+00014050: 2020 2020 2020 2020 206c 6179 6572 3a20           layer: 
+00014060: 6c61 7965 7273 7065 632e 0a20 2020 2020  layerspec..     
+00014070: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
+00014080: 726f 6d20 6764 7366 6163 746f 7279 2e70  rom gdsfactory.p
+00014090: 646b 2069 6d70 6f72 7420 6765 745f 6c61  dk import get_la
+000140a0: 7965 720a 0a20 2020 2020 2020 2069 6620  yer..        if 
+000140b0: 6c61 7965 723a 0a20 2020 2020 2020 2020  layer:.         
+000140c0: 2020 206c 6179 6572 2c20 7465 7874 7479     layer, textty
+000140d0: 7065 203d 2067 6574 5f6c 6179 6572 286c  pe = get_layer(l
+000140e0: 6179 6572 290a 2020 2020 2020 2020 656c  ayer).        el
+000140f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00014100: 7465 7874 7479 7065 203d 204e 6f6e 650a  texttype = None.
+00014110: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00014120: 656c 662e 5f63 656c 6c2e 6765 745f 6c61  elf._cell.get_la
+00014130: 6265 6c73 280a 2020 2020 2020 2020 2020  bels(.          
+00014140: 2020 6170 706c 795f 7265 7065 7469 7469    apply_repetiti
+00014150: 6f6e 733d 6170 706c 795f 7265 7065 7469  ons=apply_repeti
+00014160: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
+00014170: 2020 2064 6570 7468 3d64 6570 7468 2c0a     depth=depth,.
+00014180: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+00014190: 723d 6c61 7965 722c 0a20 2020 2020 2020  r=layer,.       
+000141a0: 2020 2020 2074 6578 7474 7970 653d 7465       texttype=te
+000141b0: 7874 7479 7065 2c0a 2020 2020 2020 2020  xttype,.        
+000141c0: 290a 0a20 2020 2064 6566 2072 656d 6f76  )..    def remov
+000141d0: 655f 6c61 6265 6c73 2873 656c 6629 202d  e_labels(self) -
+000141e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000141f0: 2222 2252 656d 6f76 6520 6c61 6265 6c73  """Remove labels
+00014200: 2e22 2222 0a20 2020 2020 2020 2073 656c  .""".        sel
+00014210: 662e 5f63 656c 6c2e 7265 6d6f 7665 282a  f._cell.remove(*
+00014220: 7365 6c66 2e6c 6162 656c 7329 0a0a 2020  self.labels)..  
+00014230: 2020 2320 4465 7072 6563 6174 6564 0a20    # Deprecated. 
+00014240: 2020 2064 6566 2067 6574 5f69 6e66 6f28     def get_info(
+00014250: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00014260: 2222 4761 7468 6572 7320 7468 6520 2e69  ""Gathers the .i
+00014270: 6e66 6f20 6469 6374 696f 6e61 7269 6573  nfo dictionaries
+00014280: 2066 726f 6d20 6576 6572 7920 7375 622d   from every sub-
+00014290: 436f 6d70 6f6e 656e 7420 616e 6420 7265  Component and re
+000142a0: 7475 726e 7320 7468 656d 2069 6e20 6120  turns them in a 
+000142b0: 6c69 7374 2e0a 0a20 2020 2020 2020 2041  list...        A
+000142c0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+000142d0: 2064 6570 7468 3a20 696e 7420 6f72 204e   depth: int or N
+000142e0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000142f0: 2020 2020 4966 206e 6f74 204e 6f6e 652c      If not None,
+00014300: 2064 6566 696e 6573 2066 726f 6d20 686f   defines from ho
+00014310: 7720 6d61 6e79 2072 6566 6572 656e 6365  w many reference
+00014320: 206c 6576 656c 7320 746f 0a20 2020 2020   levels to.     
+00014330: 2020 2020 2020 2020 2020 2072 6574 7269             retri
+00014340: 6576 6520 506f 7274 7320 6672 6f6d 2e0a  eve Ports from..
+00014350: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00014360: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
+00014370: 7374 206f 6620 6469 6374 696f 6e61 7269  st of dictionari
+00014380: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00014390: 2020 204c 6973 7420 6f66 2074 6865 2022     List of the "
+000143a0: 2e69 6e66 6f22 2070 726f 7065 7274 7920  .info" property 
+000143b0: 6469 6374 696f 6e61 7269 6573 2066 726f  dictionaries fro
+000143c0: 6d20 616c 6c20 7375 622d 436f 6d70 6f6e  m all sub-Compon
+000143d0: 656e 7473 0a20 2020 2020 2020 2022 2222  ents.        """
+000143e0: 0a20 2020 2020 2020 2044 5f6c 6973 7420  .        D_list 
+000143f0: 3d20 7365 6c66 2e67 6574 5f64 6570 656e  = self.get_depen
+00014400: 6465 6e63 6965 7328 7265 6375 7273 6976  dencies(recursiv
+00014410: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+00014420: 7265 7475 726e 205b 442e 696e 666f 2e63  return [D.info.c
+00014430: 6f70 7928 2920 666f 7220 4420 696e 2044  opy() for D in D
+00014440: 5f6c 6973 745d 0a0a 2020 2020 6465 6620  _list]..    def 
+00014450: 7265 6d61 705f 6c61 7965 7273 280a 2020  remap_layers(.  
+00014460: 2020 2020 2020 7365 6c66 2c20 6c61 7965        self, laye
+00014470: 726d 6170 2c20 696e 636c 7564 655f 6c61  rmap, include_la
+00014480: 6265 6c73 3a20 626f 6f6c 203d 2054 7275  bels: bool = Tru
+00014490: 652c 2069 6e63 6c75 6465 5f70 6174 6873  e, include_paths
+000144a0: 3a20 626f 6f6c 203d 2054 7275 650a 2020  : bool = True.  
+000144b0: 2020 2920 2d3e 2043 6f6d 706f 6e65 6e74    ) -> Component
+000144c0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+000144d0: 7572 6e73 2061 2063 6f70 7920 6f66 2074  urns a copy of t
+000144e0: 6865 2063 6f6d 706f 6e65 6e74 2077 6974  he component wit
+000144f0: 6820 7265 6d61 7070 6564 206c 6179 6572  h remapped layer
+00014500: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
+00014510: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+00014520: 7965 726d 6170 3a20 4469 6374 696f 6e61  yermap: Dictiona
+00014530: 7279 206f 6620 7661 6c75 6573 2069 6e20  ry of values in 
+00014540: 666f 726d 6174 207b 6c61 7965 725f 6672  format {layer_fr
+00014550: 6f6d 203a 206c 6179 6572 5f74 6f7d 2e0a  om : layer_to}..
+00014560: 2020 2020 2020 2020 2020 2020 696e 636c              incl
+00014570: 7564 655f 6c61 6265 6c73 3a20 5365 6c65  ude_labels: Sele
+00014580: 6374 7320 7768 6574 6865 7220 746f 206d  cts whether to m
+00014590: 6f76 6520 4c61 6265 6c73 2061 6c6f 6e67  ove Labels along
+000145a0: 2077 6974 6820 706f 6c79 676f 6e73 2e0a   with polygons..
+000145b0: 2020 2020 2020 2020 2020 2020 696e 636c              incl
+000145c0: 7564 655f 7061 7468 733a 2053 656c 6563  ude_paths: Selec
+000145d0: 7473 2077 6865 7468 6572 2074 6f20 6d6f  ts whether to mo
+000145e0: 7665 2050 6174 6873 2061 6c6f 6e67 2077  ve Paths along w
+000145f0: 6974 6820 706f 6c79 676f 6e73 2e0a 2020  ith polygons..  
+00014600: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00014610: 2020 636f 6d70 6f6e 656e 7420 3d20 7365    component = se
+00014620: 6c66 2e63 6f70 7928 290a 2020 2020 2020  lf.copy().      
+00014630: 2020 6c61 7965 726d 6170 203d 207b 5f70    layermap = {_p
+00014640: 6172 7365 5f6c 6179 6572 286b 293a 205f  arse_layer(k): _
+00014650: 7061 7273 655f 6c61 7965 7228 7629 2066  parse_layer(v) f
+00014660: 6f72 206b 2c20 7620 696e 206c 6179 6572  or k, v in layer
+00014670: 6d61 702e 6974 656d 7328 297d 0a0a 2020  map.items()}..  
+00014680: 2020 2020 2020 616c 6c5f 4420 3d20 6c69        all_D = li
+00014690: 7374 2863 6f6d 706f 6e65 6e74 2e67 6574  st(component.get
+000146a0: 5f64 6570 656e 6465 6e63 6965 7328 5472  _dependencies(Tr
+000146b0: 7565 2929 0a20 2020 2020 2020 2061 6c6c  ue)).        all
+000146c0: 5f44 2e61 7070 656e 6428 636f 6d70 6f6e  _D.append(compon
+000146d0: 656e 7429 0a20 2020 2020 2020 2066 6f72  ent).        for
+000146e0: 2044 2069 6e20 616c 6c5f 443a 0a20 2020   D in all_D:.   
+000146f0: 2020 2020 2020 2020 2066 6f72 2070 2069           for p i
+00014700: 6e20 442e 706f 6c79 676f 6e73 3a0a 2020  n D.polygons:.  
+00014710: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00014720: 7965 7220 3d20 2870 2e6c 6179 6572 2c20  yer = (p.layer, 
+00014730: 702e 6461 7461 7479 7065 290a 2020 2020  p.datatype).    
+00014740: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00014750: 6179 6572 2069 6e20 6c61 7965 726d 6170  ayer in layermap
+00014760: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014770: 2020 2020 2020 6e65 775f 6c61 7965 7220        new_layer 
+00014780: 3d20 6c61 7965 726d 6170 5b6c 6179 6572  = layermap[layer
+00014790: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000147a0: 2020 2020 2020 702e 6c61 7965 7220 3d20        p.layer = 
+000147b0: 6e65 775f 6c61 7965 725b 305d 0a20 2020  new_layer[0].   
+000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147d0: 2070 2e64 6174 6174 7970 6520 3d20 6e65   p.datatype = ne
+000147e0: 775f 6c61 7965 725b 315d 0a20 2020 2020  w_layer[1].     
+000147f0: 2020 2020 2020 2069 6620 696e 636c 7564         if includ
+00014800: 655f 6c61 6265 6c73 3a0a 2020 2020 2020  e_labels:.      
+00014810: 2020 2020 2020 2020 2020 666f 7220 6c61            for la
+00014820: 6265 6c20 696e 2044 2e6c 6162 656c 733a  bel in D.labels:
+00014830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014840: 2020 2020 206f 7269 6769 6e61 6c5f 6c61       original_la
+00014850: 7965 7220 3d20 286c 6162 656c 2e6c 6179  yer = (label.lay
+00014860: 6572 2c20 6c61 6265 6c2e 7465 7874 7479  er, label.textty
+00014870: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
+00014880: 2020 2020 2020 2020 6f72 6967 696e 616c          original
+00014890: 5f6c 6179 6572 203d 205f 7061 7273 655f  _layer = _parse_
+000148a0: 6c61 7965 7228 6f72 6967 696e 616c 5f6c  layer(original_l
+000148b0: 6179 6572 290a 2020 2020 2020 2020 2020  ayer).          
+000148c0: 2020 2020 2020 2020 2020 6966 206f 7269            if ori
+000148d0: 6769 6e61 6c5f 6c61 7965 7220 696e 206c  ginal_layer in l
+000148e0: 6179 6572 6d61 703a 0a20 2020 2020 2020  ayermap:.       
+000148f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014900: 206e 6577 5f6c 6179 6572 203d 206c 6179   new_layer = lay
+00014910: 6572 6d61 705b 6f72 6967 696e 616c 5f6c  ermap[original_l
+00014920: 6179 6572 5d0a 2020 2020 2020 2020 2020  ayer].          
+00014930: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00014940: 6265 6c2e 6c61 7965 7220 3d20 6e65 775f  bel.layer = new_
+00014950: 6c61 7965 725b 305d 0a20 2020 2020 2020  layer[0].       
+00014960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014970: 206c 6162 656c 2e74 6578 7474 7970 6520   label.texttype 
+00014980: 3d20 6e65 775f 6c61 7965 725b 315d 0a0a  = new_layer[1]..
+00014990: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000149a0: 6e63 6c75 6465 5f70 6174 6873 3a0a 2020  nclude_paths:.  
+000149b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000149c0: 7220 7061 7468 2069 6e20 442e 7061 7468  r path in D.path
+000149d0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000149e0: 2020 2020 2020 206e 6577 5f6c 6179 6572         new_layer
+000149f0: 7320 3d20 6c69 7374 2870 6174 682e 6c61  s = list(path.la
+00014a00: 7965 7273 290a 2020 2020 2020 2020 2020  yers).          
+00014a10: 2020 2020 2020 2020 2020 6e65 775f 6461            new_da
+00014a20: 7461 7479 7065 7320 3d20 6c69 7374 2870  tatypes = list(p
+00014a30: 6174 682e 6461 7461 7479 7065 7329 0a20  ath.datatypes). 
+00014a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a50: 2020 2066 6f72 206c 6179 6572 5f6e 756d     for layer_num
+00014a60: 6265 7220 696e 2072 616e 6765 286c 656e  ber in range(len
+00014a70: 286e 6577 5f6c 6179 6572 7329 293a 0a20  (new_layers)):. 
+00014a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a90: 2020 2020 2020 206f 7269 6769 6e61 6c5f         original_
+00014aa0: 6c61 7965 7220 3d20 5f70 6172 7365 5f6c  layer = _parse_l
+00014ab0: 6179 6572 280a 2020 2020 2020 2020 2020  ayer(.          
+00014ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ad0: 2020 286e 6577 5f6c 6179 6572 735b 6c61    (new_layers[la
+00014ae0: 7965 725f 6e75 6d62 6572 5d2c 206e 6577  yer_number], new
+00014af0: 5f64 6174 6174 7970 6573 5b6c 6179 6572  _datatypes[layer
+00014b00: 5f6e 756d 6265 725d 290a 2020 2020 2020  _number]).      
+00014b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b20: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00014b30: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00014b40: 7269 6769 6e61 6c5f 6c61 7965 7220 696e  riginal_layer in
+00014b50: 206c 6179 6572 6d61 703a 0a20 2020 2020   layermap:.     
+00014b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b70: 2020 2020 2020 206e 6577 5f6c 6179 6572         new_layer
+00014b80: 203d 206c 6179 6572 6d61 705b 6f72 6967   = layermap[orig
+00014b90: 696e 616c 5f6c 6179 6572 5d0a 2020 2020  inal_layer].    
+00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bb0: 2020 2020 2020 2020 6e65 775f 6c61 7965          new_laye
+00014bc0: 7273 5b6c 6179 6572 5f6e 756d 6265 725d  rs[layer_number]
+00014bd0: 203d 206e 6577 5f6c 6179 6572 5b30 5d0a   = new_layer[0].
+00014be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bf0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00014c00: 6461 7461 7479 7065 735b 6c61 7965 725f  datatypes[layer_
+00014c10: 6e75 6d62 6572 5d20 3d20 6e65 775f 6c61  number] = new_la
+00014c20: 7965 725b 315d 0a20 2020 2020 2020 2020  yer[1].         
+00014c30: 2020 2020 2020 2020 2020 2070 6174 682e             path.
+00014c40: 7365 745f 6c61 7965 7273 282a 6e65 775f  set_layers(*new_
+00014c50: 6c61 7965 7273 290a 2020 2020 2020 2020  layers).        
+00014c60: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00014c70: 2e73 6574 5f64 6174 6174 7970 6573 282a  .set_datatypes(*
+00014c80: 6e65 775f 6461 7461 7479 7065 7329 0a20  new_datatypes). 
+00014c90: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
+00014ca0: 6d70 6f6e 656e 740a 0a20 2020 2064 6566  mponent..    def
+00014cb0: 2074 6f5f 3364 280a 2020 2020 2020 2020   to_3d(.        
+00014cc0: 7365 6c66 2c0a 2020 2020 2020 2020 6c61  self,.        la
+00014cd0: 7965 725f 7669 6577 733a 204c 6179 6572  yer_views: Layer
+00014ce0: 5669 6577 7320 7c20 4e6f 6e65 203d 204e  Views | None = N
+00014cf0: 6f6e 652c 0a20 2020 2020 2020 206c 6179  one,.        lay
+00014d00: 6572 5f73 7461 636b 3a20 4c61 7965 7253  er_stack: LayerS
+00014d10: 7461 636b 207c 204e 6f6e 6520 3d20 4e6f  tack | None = No
+00014d20: 6e65 2c0a 2020 2020 2020 2020 6578 636c  ne,.        excl
+00014d30: 7564 655f 6c61 7965 7273 3a20 7475 706c  ude_layers: tupl
+00014d40: 655b 4c61 7965 722c 202e 2e2e 5d20 7c20  e[Layer, ...] | 
+00014d50: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
+00014d60: 2029 3a0a 2020 2020 2020 2020 2222 2252   ):.        """R
+00014d70: 6574 7572 6e20 436f 6d70 6f6e 656e 7420  eturn Component 
+00014d80: 3344 2074 7269 6d65 7368 2053 6365 6e65  3D trimesh Scene
+00014d90: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00014da0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+00014db0: 706f 6e65 6e74 3a20 746f 2065 7874 7275  ponent: to extru
+00014dc0: 6465 2069 6e20 3344 2e0a 2020 2020 2020  de in 3D..      
+00014dd0: 2020 2020 2020 6c61 7965 725f 7669 6577        layer_view
+00014de0: 733a 206c 6179 6572 2063 6f6c 6f72 7320  s: layer colors 
+00014df0: 6672 6f6d 204b 6c61 796f 7574 204c 6179  from Klayout Lay
+00014e00: 6572 2050 726f 7065 7274 6965 7320 6669  er Properties fi
+00014e10: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
+00014e20: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00014e30: 6163 7469 7665 2050 444b 2e6c 6179 6572  active PDK.layer
+00014e40: 5f76 6965 7773 2e0a 2020 2020 2020 2020  _views..        
+00014e50: 2020 2020 6c61 7965 725f 7374 6163 6b3a      layer_stack:
+00014e60: 2063 6f6e 7461 696e 7320 7468 6963 6b6e   contains thickn
+00014e70: 6573 7320 616e 6420 7a6d 696e 2066 6f72  ess and zmin for
+00014e80: 2065 6163 6820 6c61 7965 722e 0a20 2020   each layer..   
+00014e90: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+00014ea0: 6175 6c74 7320 746f 2061 6374 6976 6520  aults to active 
+00014eb0: 5044 4b2e 6c61 7965 725f 7374 6163 6b2e  PDK.layer_stack.
+00014ec0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00014ed0: 6c75 6465 5f6c 6179 6572 733a 206c 6179  lude_layers: lay
+00014ee0: 6572 7320 746f 2065 7863 6c75 6465 2e0a  ers to exclude..
+00014ef0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014f00: 2020 2020 2066 726f 6d20 6764 7366 6163       from gdsfac
+00014f10: 746f 7279 2e65 7870 6f72 742e 746f 5f33  tory.export.to_3
+00014f20: 6420 696d 706f 7274 2074 6f5f 3364 0a0a  d import to_3d..
+00014f30: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00014f40: 6f5f 3364 280a 2020 2020 2020 2020 2020  o_3d(.          
+00014f50: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00014f60: 2020 2020 6c61 7965 725f 7669 6577 733d      layer_views=
+00014f70: 6c61 7965 725f 7669 6577 732c 0a20 2020  layer_views,.   
+00014f80: 2020 2020 2020 2020 206c 6179 6572 5f73           layer_s
+00014f90: 7461 636b 3d6c 6179 6572 5f73 7461 636b  tack=layer_stack
+00014fa0: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
+00014fb0: 636c 7564 655f 6c61 7965 7273 3d65 7863  clude_layers=exc
+00014fc0: 6c75 6465 5f6c 6179 6572 732c 0a20 2020  lude_layers,.   
+00014fd0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00014fe0: 746f 5f6e 7028 0a20 2020 2020 2020 2073  to_np(.        s
+00014ff0: 656c 662c 0a20 2020 2020 2020 206e 6d5f  elf,.        nm_
+00015000: 7065 725f 7069 7865 6c3a 2069 6e74 203d  per_pixel: int =
+00015010: 2032 302c 0a20 2020 2020 2020 206c 6179   20,.        lay
+00015020: 6572 733a 204c 6179 6572 7320 3d20 2828  ers: Layers = ((
+00015030: 312c 2030 292c 292c 0a20 2020 2020 2020  1, 0),),.       
+00015040: 2076 616c 7565 733a 2074 7570 6c65 5b66   values: tuple[f
+00015050: 6c6f 6174 2c20 2e2e 2e5d 207c 204e 6f6e  loat, ...] | Non
+00015060: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+00015070: 2020 7061 645f 7769 6474 683a 2069 6e74    pad_width: int
+00015080: 203d 2031 2c0a 2020 2020 2920 2d3e 206e   = 1,.    ) -> n
+00015090: 702e 6e64 6172 7261 793a 0a20 2020 2020  p.ndarray:.     
+000150a0: 2020 2022 2222 5265 7475 726e 7320 6120     """Returns a 
+000150b0: 7069 7865 6c61 7465 6420 6e75 6d70 7920  pixelated numpy 
+000150c0: 6172 7261 7920 6672 6f6d 2043 6f6d 706f  array from Compo
+000150d0: 6e65 6e74 2070 6f6c 7967 6f6e 732e 0a0a  nent polygons...
+000150e0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+000150f0: 2020 2020 2020 2020 2020 636f 6d70 6f6e            compon
+00015100: 656e 743a 2043 6f6d 706f 6e65 6e74 2e0a  ent: Component..
+00015110: 2020 2020 2020 2020 2020 2020 6e6d 5f70              nm_p
+00015120: 6572 5f70 6978 656c 3a20 796f 7520 6361  er_pixel: you ca
+00015130: 6e20 676f 2066 726f 6d20 3230 2028 636f  n go from 20 (co
+00015140: 6172 7365 2920 746f 2034 2028 6669 6e65  arse) to 4 (fine
+00015150: 292e 0a20 2020 2020 2020 2020 2020 206c  )..            l
+00015160: 6179 6572 733a 2074 6f20 636f 6e76 6572  ayers: to conver
+00015170: 742e 204f 7264 6572 206d 6174 7465 7273  t. Order matters
+00015180: 2028 6c61 7474 6572 206f 7665 7277 7269   (latter overwri
+00015190: 7465 2066 6f72 6d65 7229 2e0a 2020 2020  te former)..    
+000151a0: 2020 2020 2020 2020 7661 6c75 6573 3a20          values: 
+000151b0: 6173 736f 6369 6174 6564 2074 6f20 6561  associated to ea
+000151c0: 6368 206c 6179 6572 2028 6465 6661 756c  ch layer (defaul
+000151d0: 7473 2074 6f20 3129 2e0a 2020 2020 2020  ts to 1)..      
+000151e0: 2020 2020 2020 7061 645f 7769 6474 683a        pad_width:
+000151f0: 2070 6164 6469 6e67 2070 6978 656c 7320   padding pixels 
+00015200: 6172 6f75 6e64 2074 6865 2069 6d61 6765  around the image
+00015210: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
+00015220: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
+00015230: 6163 746f 7279 2e65 7870 6f72 742e 746f  actory.export.to
+00015240: 5f6e 7020 696d 706f 7274 2074 6f5f 6e70  _np import to_np
+00015250: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00015260: 2074 6f5f 6e70 280a 2020 2020 2020 2020   to_np(.        
+00015270: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00015280: 2020 2020 2020 6e6d 5f70 6572 5f70 6978        nm_per_pix
+00015290: 656c 3d6e 6d5f 7065 725f 7069 7865 6c2c  el=nm_per_pixel,
+000152a0: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+000152b0: 6572 733d 6c61 7965 7273 2c0a 2020 2020  ers=layers,.    
+000152c0: 2020 2020 2020 2020 7661 6c75 6573 3d76          values=v
+000152d0: 616c 7565 732c 0a20 2020 2020 2020 2020  alues,.         
+000152e0: 2020 2070 6164 5f77 6964 7468 3d70 6164     pad_width=pad
+000152f0: 5f77 6964 7468 2c0a 2020 2020 2020 2020  _width,.        
+00015300: 290a 0a20 2020 2064 6566 2077 7269 7465  )..    def write
+00015310: 5f73 746c 280a 2020 2020 2020 2020 7365  _stl(.        se
+00015320: 6c66 2c0a 2020 2020 2020 2020 6669 6c65  lf,.        file
+00015330: 7061 7468 3a20 7374 722c 0a20 2020 2020  path: str,.     
+00015340: 2020 206c 6179 6572 5f73 7461 636b 3a20     layer_stack: 
+00015350: 4c61 7965 7253 7461 636b 207c 204e 6f6e  LayerStack | Non
+00015360: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+00015370: 2020 6578 636c 7564 655f 6c61 7965 7273    exclude_layers
+00015380: 3a20 7475 706c 655b 4c61 7965 722c 202e  : tuple[Layer, .
+00015390: 2e2e 5d20 7c20 4e6f 6e65 203d 204e 6f6e  ..] | None = Non
+000153a0: 652c 0a20 2020 2029 202d 3e20 4e6f 6e65  e,.    ) -> None
+000153b0: 3a0a 2020 2020 2020 2020 2222 2257 7269  :.        """Wri
+000153c0: 7465 2061 2043 6f6d 706f 6e65 6e74 2074  te a Component t
+000153d0: 6f20 5354 4c20 666f 7220 3344 2070 7269  o STL for 3D pri
+000153e0: 6e74 696e 672e 0a0a 2020 2020 2020 2020  nting...        
+000153f0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00015400: 2020 6669 6c65 7061 7468 3a20 746f 2077    filepath: to w
+00015410: 7269 7465 2053 544c 2074 6f2e 0a20 2020  rite STL to..   
+00015420: 2020 2020 2020 2020 206c 6179 6572 5f73           layer_s
+00015430: 7461 636b 3a20 636f 6e74 6169 6e73 2074  tack: contains t
+00015440: 6869 636b 6e65 7373 2061 6e64 207a 6d69  hickness and zmi
+00015450: 6e20 666f 7220 6561 6368 206c 6179 6572  n for each layer
+00015460: 2e0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+00015470: 636c 7564 655f 6c61 7965 7273 3a20 6c61  clude_layers: la
+00015480: 7965 7273 2074 6f20 6578 636c 7564 652e  yers to exclude.
+00015490: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+000154a0: 5f6c 6179 6572 5f6e 616d 653a 2049 6620  _layer_name: If 
+000154b0: 5472 7565 2c20 7573 6573 204c 6179 6572  True, uses Layer
+000154c0: 4c65 7665 6c20 6e61 6d65 7320 696e 206f  Level names in o
+000154d0: 7574 7075 7420 6669 6c65 6e61 6d65 7320  utput filenames 
+000154e0: 7261 7468 6572 2074 6861 6e20 6764 735f  rather than gds_
+000154f0: 6c61 7965 7220 616e 6420 6764 735f 6461  layer and gds_da
+00015500: 7461 7479 7065 2e0a 2020 2020 2020 2020  tatype..        
+00015510: 2020 2020 6875 6c6c 5f69 6e76 616c 6964      hull_invalid
+00015520: 5f70 6f6c 7967 6f6e 733a 2049 6620 5472  _polygons: If Tr
+00015530: 7565 2c20 7265 706c 6163 6573 2069 6e76  ue, replaces inv
+00015540: 616c 6964 2070 6f6c 7967 6f6e 7320 2864  alid polygons (d
+00015550: 6574 6572 6d69 6e65 6420 6279 2073 6861  etermined by sha
+00015560: 7065 6c79 2e50 6f6c 7967 6f6e 2e69 735f  pely.Polygon.is_
+00015570: 7661 6c69 6429 2077 6974 6820 6974 7320  valid) with its 
+00015580: 636f 6e76 6578 2068 756c 6c2e 0a20 2020  convex hull..   
+00015590: 2020 2020 2020 2020 2073 6361 6c65 3a20           scale: 
+000155a0: 4f70 7469 6f6e 616c 2066 6163 746f 7220  Optional factor 
+000155b0: 6279 2077 6869 6368 2074 6f20 7363 616c  by which to scal
+000155c0: 6520 6d65 7368 6573 2062 6566 6f72 6520  e meshes before 
+000155d0: 7772 6974 696e 672e 0a0a 2020 2020 2020  writing...      
+000155e0: 2020 2222 220a 2020 2020 2020 2020 6672    """.        fr
+000155f0: 6f6d 2067 6473 6661 6374 6f72 792e 6578  om gdsfactory.ex
+00015600: 706f 7274 2e74 6f5f 7374 6c20 696d 706f  port.to_stl impo
+00015610: 7274 2074 6f5f 7374 6c0a 0a20 2020 2020  rt to_stl..     
+00015620: 2020 2074 6f5f 7374 6c28 0a20 2020 2020     to_stl(.     
+00015630: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00015640: 2020 2020 2020 2020 2066 696c 6570 6174           filepat
+00015650: 683d 6669 6c65 7061 7468 2c0a 2020 2020  h=filepath,.    
+00015660: 2020 2020 2020 2020 6c61 7965 725f 7374          layer_st
+00015670: 6163 6b3d 6c61 7965 725f 7374 6163 6b2c  ack=layer_stack,
+00015680: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00015690: 6c75 6465 5f6c 6179 6572 733d 6578 636c  lude_layers=excl
+000156a0: 7564 655f 6c61 7965 7273 2c0a 2020 2020  ude_layers,.    
+000156b0: 2020 2020 290a 0a20 2020 2064 6566 2077      )..    def w
+000156c0: 7269 7465 5f67 6572 6265 7228 7365 6c66  rite_gerber(self
+000156d0: 2c20 6469 7270 6174 682c 206c 6179 6572  , dirpath, layer
+000156e0: 6d61 705f 746f 5f67 6572 6265 725f 6c61  map_to_gerber_la
+000156f0: 7965 722c 206f 7074 696f 6e73 2920 2d3e  yer, options) ->
+00015700: 204e 6f6e 653a 0a20 2020 2020 2020 2066   None:.        f
+00015710: 726f 6d20 6764 7366 6163 746f 7279 2e65  rom gdsfactory.e
+00015720: 7870 6f72 742e 746f 5f67 6572 6265 7220  xport.to_gerber 
+00015730: 696d 706f 7274 2074 6f5f 6765 7262 6572  import to_gerber
+00015740: 0a0a 2020 2020 2020 2020 746f 5f67 6572  ..        to_ger
+00015750: 6265 7228 0a20 2020 2020 2020 2020 2020  ber(.           
+00015760: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00015770: 2020 2064 6972 7061 7468 3d64 6972 7061     dirpath=dirpa
+00015780: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00015790: 6c61 7965 726d 6170 5f74 6f5f 6765 7262  layermap_to_gerb
+000157a0: 6572 5f6c 6179 6572 3d6c 6179 6572 6d61  er_layer=layerma
+000157b0: 705f 746f 5f67 6572 6265 725f 6c61 7965  p_to_gerber_laye
+000157c0: 722c 0a20 2020 2020 2020 2020 2020 206f  r,.            o
+000157d0: 7074 696f 6e73 3d6f 7074 696f 6e73 2c0a  ptions=options,.
+000157e0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+000157f0: 6566 2074 6f5f 676d 7368 280a 2020 2020  ef to_gmsh(.    
+00015800: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00015810: 2020 7479 7065 2c0a 2020 2020 2020 2020    type,.        
+00015820: 7a3d 4e6f 6e65 2c0a 2020 2020 2020 2020  z=None,.        
+00015830: 7873 6563 7469 6f6e 5f62 6f75 6e64 733d  xsection_bounds=
+00015840: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c61  None,.        la
+00015850: 7965 725f 7374 6163 6b3d 4e6f 6e65 2c0a  yer_stack=None,.
+00015860: 2020 2020 2020 2020 7761 6665 725f 7061          wafer_pa
+00015870: 6464 696e 673d 302e 302c 0a20 2020 2020  dding=0.0,.     
+00015880: 2020 2077 6166 6572 5f6c 6179 6572 3d4c     wafer_layer=L
+00015890: 4159 4552 2e57 4146 4552 2c0a 2020 2020  AYER.WAFER,.    
+000158a0: 2020 2020 2a61 7267 732c 0a20 2020 2020      *args,.     
+000158b0: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
+000158c0: 2029 3a0a 2020 2020 2020 2020 2222 2252   ):.        """R
+000158d0: 6574 7572 6e73 2061 2067 6d73 6820 6d73  eturns a gmsh ms
+000158e0: 6820 6f66 2074 6865 2063 6f6d 706f 6e65  h of the compone
+000158f0: 6e74 2066 6f72 2066 696e 6974 6520 656c  nt for finite el
+00015900: 656d 656e 7420 7369 6d75 6c61 7469 6f6e  ement simulation
+00015910: 2e0a 0a20 2020 2020 2020 2041 7267 756d  ...        Argum
+00015920: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
+00015930: 2020 7479 7065 3a20 6f6e 6520 6f66 2022    type: one of "
+00015940: 7879 222c 2022 757a 222c 206f 7220 2233  xy", "uz", or "3
+00015950: 4422 2e20 4465 7465 726d 696e 6573 2074  D". Determines t
+00015960: 6865 2074 7970 6520 6f66 206d 6573 6820  he type of mesh 
+00015970: 746f 2072 6574 7572 6e2e 0a20 2020 2020  to return..     
+00015980: 2020 2020 2020 207a 3a20 7573 6564 2074         z: used t
+00015990: 6f20 6465 6669 6e65 207a 2d73 6c69 6365  o define z-slice
+000159a0: 2066 6f72 2078 7920 6d65 7368 696e 670a   for xy meshing.
+000159b0: 2020 2020 2020 2020 2020 2020 7873 6563              xsec
+000159c0: 7469 6f6e 5f62 6f75 6e64 733a 2075 7365  tion_bounds: use
+000159d0: 6420 746f 2064 6566 696e 6520 696e 2d70  d to define in-p
+000159e0: 6c61 6e65 206c 696e 6520 666f 7220 757a  lane line for uz
+000159f0: 206d 6573 6869 6e67 0a20 2020 2020 2020   meshing.       
+00015a00: 2020 2020 2077 6166 6572 5f70 6164 6469       wafer_paddi
+00015a10: 6e67 3a20 7061 6464 696e 6720 6265 796f  ng: padding beyo
+00015a20: 6e64 2062 626f 7820 746f 2061 6464 2074  nd bbox to add t
+00015a30: 6f20 5741 4645 5220 6c61 7965 7273 2e0a  o WAFER layers..
+00015a40: 0a20 2020 2020 2020 204b 6579 776f 7264  .        Keyword
+00015a50: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00015a60: 2020 2041 7267 756d 656e 7473 2066 6f72     Arguments for
+00015a70: 2074 6865 2074 6172 6765 7420 6d65 7368   the target mesh
+00015a80: 696e 6720 6675 6e63 7469 6f6e 2069 6e20  ing function in 
+00015a90: 6770 6c75 6769 6e73 2e67 6d73 680a 2020  gplugins.gmsh.  
+00015aa0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015ab0: 2020 2320 4164 6420 5741 4645 5220 6c61    # Add WAFER la
+00015ac0: 7965 723a 0a20 2020 2020 2020 2070 6164  yer:.        pad
+00015ad0: 6465 645f 636f 6d70 6f6e 656e 7420 3d20  ded_component = 
+00015ae0: 436f 6d70 6f6e 656e 7428 290a 2020 2020  Component().    
+00015af0: 2020 2020 7061 6464 6564 5f63 6f6d 706f      padded_compo
+00015b00: 6e65 6e74 203c 3c20 7365 6c66 0a20 2020  nent << self.   
+00015b10: 2020 2020 2028 786d 696e 2c20 796d 696e       (xmin, ymin
+00015b20: 292c 2028 786d 6178 2c20 796d 6178 2920  ), (xmax, ymax) 
+00015b30: 3d20 7365 6c66 2e62 626f 780a 2020 2020  = self.bbox.    
+00015b40: 2020 2020 706f 696e 7473 203d 205b 0a20      points = [. 
+00015b50: 2020 2020 2020 2020 2020 205b 786d 696e             [xmin
+00015b60: 202d 2077 6166 6572 5f70 6164 6469 6e67   - wafer_padding
+00015b70: 2c20 796d 696e 202d 2077 6166 6572 5f70  , ymin - wafer_p
+00015b80: 6164 6469 6e67 5d2c 0a20 2020 2020 2020  adding],.       
+00015b90: 2020 2020 205b 786d 6178 202b 2077 6166       [xmax + waf
+00015ba0: 6572 5f70 6164 6469 6e67 2c20 796d 696e  er_padding, ymin
+00015bb0: 202d 2077 6166 6572 5f70 6164 6469 6e67   - wafer_padding
+00015bc0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+00015bd0: 786d 6178 202b 2077 6166 6572 5f70 6164  xmax + wafer_pad
+00015be0: 6469 6e67 2c20 796d 6178 202b 2077 6166  ding, ymax + waf
+00015bf0: 6572 5f70 6164 6469 6e67 5d2c 0a20 2020  er_padding],.   
+00015c00: 2020 2020 2020 2020 205b 786d 696e 202d           [xmin -
+00015c10: 2077 6166 6572 5f70 6164 6469 6e67 2c20   wafer_padding, 
+00015c20: 796d 6178 202b 2077 6166 6572 5f70 6164  ymax + wafer_pad
+00015c30: 6469 6e67 5d2c 0a20 2020 2020 2020 205d  ding],.        ]
+00015c40: 0a20 2020 2020 2020 2070 6164 6465 645f  .        padded_
+00015c50: 636f 6d70 6f6e 656e 742e 6164 645f 706f  component.add_po
+00015c60: 6c79 676f 6e28 706f 696e 7473 2c20 6c61  lygon(points, la
+00015c70: 7965 723d 7761 6665 725f 6c61 7965 7229  yer=wafer_layer)
+00015c80: 0a20 2020 2020 2020 2070 6164 6465 645f  .        padded_
+00015c90: 636f 6d70 6f6e 656e 742e 6164 645f 706f  component.add_po
+00015ca0: 7274 7328 7365 6c66 2e67 6574 5f70 6f72  rts(self.get_por
+00015cb0: 7473 5f6c 6973 7428 2929 0a0a 2020 2020  ts_list())..    
+00015cc0: 2020 2020 6966 206c 6179 6572 5f73 7461      if layer_sta
+00015cd0: 636b 2069 7320 4e6f 6e65 3a0a 2020 2020  ck is None:.    
+00015ce0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00015cf0: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00015d00: 2020 2020 2020 2020 2020 2741 204c 6179            'A Lay
+00015d10: 6572 5374 6163 6b20 6d75 7374 2062 6520  erStack must be 
+00015d20: 7072 6f76 6964 6564 2074 6872 6f75 6768  provided through
+00015d30: 2061 7267 756d 656e 7420 226c 6179 6572   argument "layer
+00015d40: 5f73 7461 636b 222e 270a 2020 2020 2020  _stack".'.      
+00015d50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00015d60: 6966 2074 7970 6520 3d3d 2022 7879 223a  if type == "xy":
+00015d70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00015d80: 7a20 6973 204e 6f6e 653a 0a20 2020 2020  z is None:.     
+00015d90: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00015da0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+00015db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015dc0: 2027 466f 7220 7879 2d6d 6573 6869 6e67   'For xy-meshing
+00015dd0: 2c20 6120 7a2d 7661 6c75 6520 6d75 7374  , a z-value must
+00015de0: 2062 6520 7072 6f76 6964 6564 2076 6961   be provided via
+00015df0: 2074 6865 2066 6c6f 6174 2061 7267 756d   the float argum
+00015e00: 656e 7420 227a 222e 270a 2020 2020 2020  ent "z".'.      
+00015e10: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00015e20: 2020 2020 2020 2020 6672 6f6d 2067 706c          from gpl
+00015e30: 7567 696e 732e 676d 7368 2e78 795f 7873  ugins.gmsh.xy_xs
+00015e40: 6563 7469 6f6e 5f6d 6573 6820 696d 706f  ection_mesh impo
+00015e50: 7274 2078 795f 7873 6563 7469 6f6e 5f6d  rt xy_xsection_m
+00015e60: 6573 680a 0a20 2020 2020 2020 2020 2020  esh..           
+00015e70: 2072 6574 7572 6e20 7879 5f78 7365 6374   return xy_xsect
+00015e80: 696f 6e5f 6d65 7368 2870 6164 6465 645f  ion_mesh(padded_
+00015e90: 636f 6d70 6f6e 656e 742c 207a 2c20 6c61  component, z, la
+00015ea0: 7965 725f 7374 6163 6b2c 202a 2a6b 7761  yer_stack, **kwa
+00015eb0: 7267 7329 0a20 2020 2020 2020 2065 6c69  rgs).        eli
+00015ec0: 6620 7479 7065 203d 3d20 2275 7a22 3a0a  f type == "uz":.
+00015ed0: 2020 2020 2020 2020 2020 2020 6966 2078              if x
+00015ee0: 7365 6374 696f 6e5f 626f 756e 6473 2069  section_bounds i
+00015ef0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00015f00: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00015f10: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00015f20: 2020 2020 2020 2020 2020 2020 2020 2246                "F
+00015f30: 6f72 2075 7a2d 6d65 7368 696e 672c 2079  or uz-meshing, y
+00015f40: 6f75 206d 7573 7420 7072 6f76 6964 6520  ou must provide 
+00015f50: 6120 6c69 6e65 2069 6e20 7468 6520 7879  a line in the xy
+00015f60: 2d70 6c61 6e65 2022 0a20 2020 2020 2020  -plane ".       
+00015f70: 2020 2020 2020 2020 2020 2020 2022 7669               "vi
+00015f80: 6120 7468 6520 5475 706c 6520 6172 6775  a the Tuple argu
+00015f90: 6d65 6e74 205b 5b78 312c 7931 5d2c 205b  ment [[x1,y1], [
+00015fa0: 7832 2c79 325d 5d20 7873 6563 7469 6f6e  x2,y2]] xsection
+00015fb0: 5f62 6f75 6e64 732e 220a 2020 2020 2020  _bounds.".      
+00015fc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00015fd0: 2020 2020 2020 2020 6672 6f6d 2067 706c          from gpl
+00015fe0: 7567 696e 732e 676d 7368 2e75 7a5f 7873  ugins.gmsh.uz_xs
+00015ff0: 6563 7469 6f6e 5f6d 6573 6820 696d 706f  ection_mesh impo
+00016000: 7274 2075 7a5f 7873 6563 7469 6f6e 5f6d  rt uz_xsection_m
+00016010: 6573 680a 0a20 2020 2020 2020 2020 2020  esh..           
+00016020: 2072 6574 7572 6e20 757a 5f78 7365 6374   return uz_xsect
+00016030: 696f 6e5f 6d65 7368 280a 2020 2020 2020  ion_mesh(.      
+00016040: 2020 2020 2020 2020 2020 7061 6464 6564            padded
+00016050: 5f63 6f6d 706f 6e65 6e74 2c20 7873 6563  _component, xsec
+00016060: 7469 6f6e 5f62 6f75 6e64 732c 206c 6179  tion_bounds, lay
+00016070: 6572 5f73 7461 636b 2c20 2a2a 6b77 6172  er_stack, **kwar
+00016080: 6773 0a20 2020 2020 2020 2020 2020 2029  gs.            )
+00016090: 0a20 2020 2020 2020 2065 6c69 6620 7479  .        elif ty
+000160a0: 7065 203d 3d20 2233 4422 3a0a 2020 2020  pe == "3D":.    
+000160b0: 2020 2020 2020 2020 7370 6563 203d 2069          spec = i
+000160c0: 6d70 6f72 746c 6962 2e75 7469 6c2e 6669  mportlib.util.fi
+000160d0: 6e64 5f73 7065 6328 226d 6573 6877 656c  nd_spec("meshwel
+000160e0: 6c22 290a 2020 2020 2020 2020 2020 2020  l").            
+000160f0: 6966 2073 7065 6320 6973 204e 6f6e 653a  if spec is None:
+00016100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016110: 2070 7269 6e74 280a 2020 2020 2020 2020   print(.        
+00016120: 2020 2020 2020 2020 2020 2020 2233 4420              "3D 
+00016130: 6d65 7368 696e 6720 7265 7175 6972 6573  meshing requires
+00016140: 206d 6573 6877 656c 6c2c 2073 6565 2068   meshwell, see h
+00016150: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00016160: 6d2f 7369 6d62 696c 6f64 2f6d 6573 6877  m/simbilod/meshw
+00016170: 656c 6c20 6f72 2072 756e 2070 6970 2069  ell or run pip i
+00016180: 6e73 7461 6c6c 206d 6573 6877 656c 6c2e  nstall meshwell.
+00016190: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000161a0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+000161b0: 2066 726f 6d20 6770 6c75 6769 6e73 2e67   from gplugins.g
+000161c0: 6d73 682e 7879 7a5f 6d65 7368 2069 6d70  msh.xyz_mesh imp
+000161d0: 6f72 7420 7879 7a5f 6d65 7368 0a0a 2020  ort xyz_mesh..  
+000161e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000161f0: 2078 797a 5f6d 6573 6828 7061 6464 6564   xyz_mesh(padded
+00016200: 5f63 6f6d 706f 6e65 6e74 2c20 6c61 7965  _component, laye
+00016210: 725f 7374 6163 6b2c 202a 2a6b 7761 7267  r_stack, **kwarg
+00016220: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
+00016230: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00016240: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00016250: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00016260: 5265 7175 6972 6564 2061 7267 756d 656e  Required argumen
+00016270: 7420 2274 7970 6522 206d 7573 7420 6265  t "type" must be
+00016280: 206f 6e65 206f 6620 2278 7922 2c20 2275   one of "xy", "u
+00016290: 7a22 2c20 6f72 2022 3344 222e 270a 2020  z", or "3D".'.  
+000162a0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000162b0: 2064 6566 206f 6666 7365 7428 0a20 2020   def offset(.   
+000162c0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000162d0: 2020 2064 6973 7461 6e63 653a 2066 6c6f     distance: flo
+000162e0: 6174 203d 2030 2e31 2c0a 2020 2020 2020  at = 0.1,.      
+000162f0: 2020 706f 6c79 676f 6e73 3d4e 6f6e 652c    polygons=None,
+00016300: 0a20 2020 2020 2020 2075 7365 5f75 6e69  .        use_uni
+00016310: 6f6e 3a20 626f 6f6c 203d 2054 7275 652c  on: bool = True,
+00016320: 0a20 2020 2020 2020 2070 7265 6369 7369  .        precisi
+00016330: 6f6e 3a20 666c 6f61 7420 3d20 3165 2d34  on: float = 1e-4
+00016340: 2c0a 2020 2020 2020 2020 6a6f 696e 3a20  ,.        join: 
+00016350: 7374 7220 3d20 226d 6974 6572 222c 0a20  str = "miter",. 
+00016360: 2020 2020 2020 2074 6f6c 6572 616e 6365         tolerance
+00016370: 3a20 696e 7420 3d20 322c 0a20 2020 2020  : int = 2,.     
+00016380: 2020 206c 6179 6572 3a20 4c61 7965 7253     layer: LayerS
+00016390: 7065 6320 3d20 2257 4722 2c0a 2020 2020  pec = "WG",.    
+000163a0: 2920 2d3e 2043 6f6d 706f 6e65 6e74 3a0a  ) -> Component:.
+000163b0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+000163c0: 6e73 206e 6577 2043 6f6d 706f 6e65 6e74  ns new Component
+000163d0: 2077 6974 6820 706f 6c79 676f 6e73 2065   with polygons e
+000163e0: 726f 6465 6420 6f72 2064 696c 6174 6564  roded or dilated
+000163f0: 2062 7920 616e 206f 6666 7365 742e 0a0a   by an offset...
+00016400: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00016410: 2020 2020 2020 2020 2020 6469 7374 616e            distan
+00016420: 6365 3a20 4469 7374 616e 6365 2074 6f20  ce: Distance to 
+00016430: 6f66 6673 6574 2070 6f6c 7967 6f6e 732e  offset polygons.
+00016440: 2050 6f73 6974 6976 6520 7661 6c75 6573   Positive values
+00016450: 2065 7870 616e 642c 206e 6567 6174 6976   expand, negativ
+00016460: 6520 7368 7269 6e6b 2e0a 2020 2020 2020  e shrink..      
+00016470: 2020 2020 2020 7072 6563 6973 696f 6e3a        precision:
+00016480: 2044 6573 6972 6564 2070 7265 6369 7369   Desired precisi
+00016490: 6f6e 2066 6f72 2072 6f75 6e64 696e 6720  on for rounding 
+000164a0: 7665 7274 6578 2063 6f6f 7264 696e 6174  vertex coordinat
+000164b0: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+000164c0: 6a6f 696e 3a20 7b27 6d69 7465 7227 2c20  join: {'miter', 
+000164d0: 2762 6576 656c 272c 2027 726f 756e 6427  'bevel', 'round'
+000164e0: 7d20 5479 7065 206f 6620 6a6f 696e 2075  } Type of join u
+000164f0: 7365 6420 746f 2063 7265 6174 6520 706f  sed to create po
+00016500: 6c79 676f 6e20 6f66 6673 6574 0a20 2020  lygon offset.   
+00016510: 2020 2020 2020 2020 2074 6f6c 6572 616e           toleran
+00016520: 6365 3a20 466f 7220 6d69 7465 7220 6a6f  ce: For miter jo
+00016530: 696e 7473 2c20 7468 6973 206e 756d 6265  ints, this numbe
+00016540: 7220 6d75 7374 2062 6520 6174 206c 6561  r must be at lea
+00016550: 7374 2032 2072 6570 7265 7365 6e74 7320  st 2 represents 
+00016560: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00016570: 2020 6d61 7869 6d61 6c20 6469 7374 616e    maximal distan
+00016580: 6365 2069 6e20 6d75 6c74 6970 6c65 7320  ce in multiples 
+00016590: 6f66 206f 6666 7365 7420 6265 7477 6565  of offset betwee
+000165a0: 6e20 6e65 7720 7665 7274 6963 6573 2061  n new vertices a
+000165b0: 6e64 2074 6865 6972 0a20 2020 2020 2020  nd their.       
+000165c0: 2020 2020 2020 206f 7269 6769 6e61 6c20         original 
+000165d0: 706f 7369 7469 6f6e 2062 6566 6f72 6520  position before 
+000165e0: 6265 7665 6c69 6e67 2074 6f20 6176 6f69  beveling to avoi
+000165f0: 6420 7370 696b 6573 2061 7420 6163 7574  d spikes at acut
+00016600: 6520 6a6f 696e 7473 2e20 466f 720a 2020  e joints. For.  
+00016610: 2020 2020 2020 2020 2020 2020 726f 756e              roun
+00016620: 6420 6a6f 696e 7473 2c20 6974 2069 6e64  d joints, it ind
+00016630: 6963 6174 6573 2074 6865 2063 7572 7661  icates the curva
+00016640: 7475 7265 2072 6573 6f6c 7574 696f 6e20  ture resolution 
+00016650: 696e 206e 756d 6265 7220 6f66 0a20 2020  in number of.   
+00016660: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
+00016670: 7320 7065 7220 6675 6c6c 2063 6972 636c  s per full circl
+00016680: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
+00016690: 6179 6572 3a20 5370 6563 6966 6963 206c  ayer: Specific l
+000166a0: 6179 6572 2066 6f72 206e 6577 2070 6f6c  ayer for new pol
+000166b0: 7967 6f6e 732e 0a0a 2020 2020 2020 2020  ygons...        
+000166c0: 2222 220a 2020 2020 2020 2020 696d 706f  """.        impo
+000166d0: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
+000166e0: 2067 660a 0a20 2020 2020 2020 2067 6473   gf..        gds
+000166f0: 5f6c 6179 6572 2c20 6764 735f 6461 7461  _layer, gds_data
+00016700: 7479 7065 203d 2067 662e 6765 745f 6c61  type = gf.get_la
+00016710: 7965 7228 6c61 7965 7229 0a20 2020 2020  yer(layer).     
+00016720: 2020 2070 203d 2067 6473 746b 2e6f 6666     p = gdstk.off
+00016730: 7365 7428 0a20 2020 2020 2020 2020 2020  set(.           
+00016740: 2070 6f6c 7967 6f6e 7320 6f72 2073 656c   polygons or sel
+00016750: 662e 6765 745f 706f 6c79 676f 6e73 2829  f.get_polygons()
+00016760: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+00016770: 7374 616e 6365 3d64 6973 7461 6e63 652c  stance=distance,
+00016780: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
+00016790: 6e3d 6a6f 696e 2c0a 2020 2020 2020 2020  n=join,.        
+000167a0: 2020 2020 746f 6c65 7261 6e63 653d 746f      tolerance=to
+000167b0: 6c65 7261 6e63 652c 0a20 2020 2020 2020  lerance,.       
+000167c0: 2020 2020 2070 7265 6369 7369 6f6e 3d70       precision=p
+000167d0: 7265 6369 7369 6f6e 2c0a 2020 2020 2020  recision,.      
+000167e0: 2020 2020 2020 7573 655f 756e 696f 6e3d        use_union=
+000167f0: 7573 655f 756e 696f 6e2c 0a20 2020 2020  use_union,.     
+00016800: 2020 2020 2020 206c 6179 6572 3d67 6473         layer=gds
+00016810: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
+00016820: 2020 2020 6461 7461 7479 7065 3d67 6473      datatype=gds
+00016830: 5f64 6174 6174 7970 652c 0a20 2020 2020  _datatype,.     
+00016840: 2020 2029 0a0a 2020 2020 2020 2020 636f     )..        co
+00016850: 6d70 6f6e 656e 7420 3d20 6766 2e43 6f6d  mponent = gf.Com
+00016860: 706f 6e65 6e74 2829 0a20 2020 2020 2020  ponent().       
+00016870: 2063 6f6d 706f 6e65 6e74 2e61 6464 5f70   component.add_p
+00016880: 6f6c 7967 6f6e 2870 2c20 6c61 7965 723d  olygon(p, layer=
+00016890: 6c61 7965 7229 0a20 2020 2020 2020 2072  layer).        r
+000168a0: 6574 7572 6e20 636f 6d70 6f6e 656e 740a  eturn component.
+000168b0: 0a0a 6465 6620 636f 7079 280a 2020 2020  ..def copy(.    
+000168c0: 443a 2043 6f6d 706f 6e65 6e74 2c0a 2020  D: Component,.  
+000168d0: 2020 7265 6665 7265 6e63 6573 3d4e 6f6e    references=Non
+000168e0: 652c 0a20 2020 2070 6f72 7473 3d4e 6f6e  e,.    ports=Non
+000168f0: 652c 0a20 2020 2070 6f6c 7967 6f6e 733d  e,.    polygons=
+00016900: 4e6f 6e65 2c0a 2020 2020 7061 7468 733d  None,.    paths=
+00016910: 4e6f 6e65 2c0a 2020 2020 6e61 6d65 3d4e  None,.    name=N
+00016920: 6f6e 652c 0a20 2020 206c 6162 656c 733d  one,.    labels=
+00016930: 4e6f 6e65 2c0a 2920 2d3e 2043 6f6d 706f  None,.) -> Compo
+00016940: 6e65 6e74 3a0a 2020 2020 2222 2252 6574  nent:.    """Ret
+00016950: 7572 6e73 2061 2043 6f6d 706f 6e65 6e74  urns a Component
+00016960: 2063 6f70 792e 0a0a 2020 2020 4172 6773   copy...    Args
+00016970: 3a0a 2020 2020 2020 2020 443a 2063 6f6d  :.        D: com
+00016980: 706f 6e65 6e74 2074 6f20 636f 7079 2e0a  ponent to copy..
+00016990: 2020 2020 2222 220a 2020 2020 445f 636f      """.    D_co
+000169a0: 7079 203d 2043 6f6d 706f 6e65 6e74 2829  py = Component()
+000169b0: 0a20 2020 2044 5f63 6f70 792e 696e 666f  .    D_copy.info
+000169c0: 203d 2044 2e69 6e66 6f0a 2020 2020 2320   = D.info.    # 
+000169d0: 445f 636f 7079 2e5f 6365 6c6c 203d 2044  D_copy._cell = D
+000169e0: 2e5f 6365 6c6c 2e63 6f70 7928 6e61 6d65  ._cell.copy(name
+000169f0: 3d44 5f63 6f70 792e 6e61 6d65 290a 0a20  =D_copy.name).. 
+00016a00: 2020 2066 6f72 2072 6566 2069 6e20 7265     for ref in re
+00016a10: 6665 7265 6e63 6573 2069 6620 7265 6665  ferences if refe
+00016a20: 7265 6e63 6573 2069 7320 6e6f 7420 4e6f  rences is not No
+00016a30: 6e65 2065 6c73 6520 442e 7265 6665 7265  ne else D.refere
+00016a40: 6e63 6573 3a0a 2020 2020 2020 2020 445f  nces:.        D_
+00016a50: 636f 7079 2e61 6464 2863 6f70 795f 7265  copy.add(copy_re
+00016a60: 6665 7265 6e63 6528 7265 6629 290a 2020  ference(ref)).  
+00016a70: 2020 666f 7220 706f 7274 2069 6e20 2870    for port in (p
+00016a80: 6f72 7473 2069 6620 706f 7274 7320 6973  orts if ports is
+00016a90: 206e 6f74 204e 6f6e 6520 656c 7365 2044   not None else D
+00016aa0: 2e70 6f72 7473 292e 7661 6c75 6573 2829  .ports).values()
+00016ab0: 3a0a 2020 2020 2020 2020 445f 636f 7079  :.        D_copy
+00016ac0: 2e61 6464 5f70 6f72 7428 706f 7274 3d70  .add_port(port=p
+00016ad0: 6f72 7429 0a20 2020 2066 6f72 2070 6f6c  ort).    for pol
+00016ae0: 7920 696e 2070 6f6c 7967 6f6e 7320 6966  y in polygons if
+00016af0: 2070 6f6c 7967 6f6e 7320 6973 206e 6f74   polygons is not
+00016b00: 204e 6f6e 6520 656c 7365 2044 2e70 6f6c   None else D.pol
+00016b10: 7967 6f6e 733a 0a20 2020 2020 2020 2044  ygons:.        D
+00016b20: 5f63 6f70 792e 6164 645f 706f 6c79 676f  _copy.add_polygo
+00016b30: 6e28 706f 6c79 290a 2020 2020 666f 7220  n(poly).    for 
+00016b40: 7061 7468 2069 6e20 7061 7468 7320 6966  path in paths if
+00016b50: 2070 6174 6873 2069 7320 6e6f 7420 4e6f   paths is not No
+00016b60: 6e65 2065 6c73 6520 442e 7061 7468 733a  ne else D.paths:
+00016b70: 0a20 2020 2020 2020 2044 5f63 6f70 792e  .        D_copy.
+00016b80: 6164 6428 7061 7468 290a 2020 2020 666f  add(path).    fo
+00016b90: 7220 6c61 6265 6c20 696e 206c 6162 656c  r label in label
+00016ba0: 7320 6966 206c 6162 656c 7320 6973 206e  s if labels is n
+00016bb0: 6f74 204e 6f6e 6520 656c 7365 2044 2e6c  ot None else D.l
+00016bc0: 6162 656c 733a 0a20 2020 2020 2020 2044  abels:.        D
+00016bd0: 5f63 6f70 792e 6164 645f 6c61 6265 6c28  _copy.add_label(
+00016be0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+00016bf0: 743d 6c61 6265 6c2e 7465 7874 2c0a 2020  t=label.text,.  
+00016c00: 2020 2020 2020 2020 2020 706f 7369 7469            positi
+00016c10: 6f6e 3d6c 6162 656c 2e6f 7269 6769 6e2c  on=label.origin,
+00016c20: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+00016c30: 6572 3d28 6c61 6265 6c2e 6c61 7965 722c  er=(label.layer,
+00016c40: 206c 6162 656c 2e74 6578 7474 7970 6529   label.texttype)
+00016c50: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00016c60: 2069 6620 6e61 6d65 2069 7320 6e6f 7420   if name is not 
+00016c70: 4e6f 6e65 3a0a 2020 2020 2020 2020 445f  None:.        D_
+00016c80: 636f 7079 2e6e 616d 6520 3d20 6e61 6d65  copy.name = name
+00016c90: 0a0a 2020 2020 7265 7475 726e 2044 5f63  ..    return D_c
+00016ca0: 6f70 790a 0a0a 6465 6620 636f 7079 5f72  opy...def copy_r
+00016cb0: 6566 6572 656e 6365 280a 2020 2020 7265  eference(.    re
+00016cc0: 662c 0a20 2020 2070 6172 656e 743d 4e6f  f,.    parent=No
+00016cd0: 6e65 2c0a 2020 2020 636f 6c75 6d6e 733d  ne,.    columns=
+00016ce0: 4e6f 6e65 2c0a 2020 2020 726f 7773 3d4e  None,.    rows=N
+00016cf0: 6f6e 652c 0a20 2020 2073 7061 6369 6e67  one,.    spacing
+00016d00: 3d4e 6f6e 652c 0a20 2020 206f 7269 6769  =None,.    origi
+00016d10: 6e3d 4e6f 6e65 2c0a 2020 2020 726f 7461  n=None,.    rota
+00016d20: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 206d  tion=None,.    m
+00016d30: 6167 6e69 6669 6361 7469 6f6e 3d4e 6f6e  agnification=Non
+00016d40: 652c 0a20 2020 2078 5f72 6566 6c65 6374  e,.    x_reflect
+00016d50: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 6e61  ion=None,.    na
+00016d60: 6d65 3d4e 6f6e 652c 0a20 2020 2076 313d  me=None,.    v1=
+00016d70: 4e6f 6e65 2c0a 2020 2020 7632 3d4e 6f6e  None,.    v2=Non
+00016d80: 652c 0a29 202d 3e20 436f 6d70 6f6e 656e  e,.) -> Componen
+00016d90: 7452 6566 6572 656e 6365 3a0a 2020 2020  tReference:.    
+00016da0: 7265 7475 726e 2043 6f6d 706f 6e65 6e74  return Component
+00016db0: 5265 6665 7265 6e63 6528 0a20 2020 2020  Reference(.     
+00016dc0: 2020 2063 6f6d 706f 6e65 6e74 3d70 6172     component=par
+00016dd0: 656e 7420 6f72 2072 6566 2e70 6172 656e  ent or ref.paren
+00016de0: 742c 0a20 2020 2020 2020 2063 6f6c 756d  t,.        colum
+00016df0: 6e73 3d63 6f6c 756d 6e73 206f 7220 7265  ns=columns or re
+00016e00: 662e 636f 6c75 6d6e 732c 0a20 2020 2020  f.columns,.     
+00016e10: 2020 2072 6f77 733d 726f 7773 206f 7220     rows=rows or 
+00016e20: 7265 662e 726f 7773 2c0a 2020 2020 2020  ref.rows,.      
+00016e30: 2020 7370 6163 696e 673d 7370 6163 696e    spacing=spacin
+00016e40: 6720 6f72 2072 6566 2e73 7061 6369 6e67  g or ref.spacing
+00016e50: 2c0a 2020 2020 2020 2020 6f72 6967 696e  ,.        origin
+00016e60: 3d6f 7269 6769 6e20 6f72 2072 6566 2e6f  =origin or ref.o
+00016e70: 7269 6769 6e2c 0a20 2020 2020 2020 2072  rigin,.        r
+00016e80: 6f74 6174 696f 6e3d 726f 7461 7469 6f6e  otation=rotation
+00016e90: 206f 7220 7265 662e 726f 7461 7469 6f6e   or ref.rotation
+00016ea0: 2c0a 2020 2020 2020 2020 6d61 676e 6966  ,.        magnif
+00016eb0: 6963 6174 696f 6e3d 6d61 676e 6966 6963  ication=magnific
+00016ec0: 6174 696f 6e20 6f72 2072 6566 2e6d 6167  ation or ref.mag
+00016ed0: 6e69 6669 6361 7469 6f6e 2c0a 2020 2020  nification,.    
+00016ee0: 2020 2020 785f 7265 666c 6563 7469 6f6e      x_reflection
+00016ef0: 3d78 5f72 6566 6c65 6374 696f 6e20 6f72  =x_reflection or
+00016f00: 2072 6566 2e78 5f72 6566 6c65 6374 696f   ref.x_reflectio
+00016f10: 6e2c 0a20 2020 2020 2020 206e 616d 653d  n,.        name=
+00016f20: 6e61 6d65 206f 7220 7265 662e 6e61 6d65  name or ref.name
+00016f30: 2c0a 2020 2020 2020 2020 7631 3d76 3120  ,.        v1=v1 
+00016f40: 6f72 2072 6566 2e76 312c 0a20 2020 2020  or ref.v1,.     
+00016f50: 2020 2076 323d 7632 206f 7220 7265 662e     v2=v2 or ref.
+00016f60: 7632 2c0a 2020 2020 290a 0a0a 6465 6620  v2,.    )...def 
+00016f70: 7465 7374 5f67 6574 5f6c 6179 6572 7328  test_get_layers(
+00016f80: 2920 2d3e 204e 6f6e 653a 0a20 2020 2069  ) -> None:.    i
+00016f90: 6d70 6f72 7420 6764 7366 6163 746f 7279  mport gdsfactory
+00016fa0: 2061 7320 6766 0a0a 2020 2020 6331 203d   as gf..    c1 =
+00016fb0: 2067 662e 636f 6d70 6f6e 656e 7473 2e73   gf.components.s
+00016fc0: 7472 6169 6768 7428 0a20 2020 2020 2020  traight(.       
+00016fd0: 206c 656e 6774 683d 3130 2c0a 2020 2020   length=10,.    
+00016fe0: 2020 2020 7769 6474 683d 302e 352c 0a20      width=0.5,. 
+00016ff0: 2020 2020 2020 206c 6179 6572 3d28 322c         layer=(2,
+00017000: 2030 292c 0a20 2020 2020 2020 2062 626f   0),.        bbo
+00017010: 785f 6c61 7965 7273 3d5b 2831 3131 2c20  x_layers=[(111, 
+00017020: 3029 5d2c 0a20 2020 2020 2020 2062 626f  0)],.        bbo
+00017030: 785f 6f66 6673 6574 733d 5b33 5d2c 0a20  x_offsets=[3],. 
+00017040: 2020 2020 2020 2077 6974 685f 6262 6f78         with_bbox
+00017050: 3d54 7275 652c 0a20 2020 2020 2020 2063  =True,.        c
+00017060: 6c61 6464 696e 675f 6c61 7965 7273 3d4e  ladding_layers=N
+00017070: 6f6e 652c 0a20 2020 2020 2020 2061 6464  one,.        add
+00017080: 5f70 696e 733d 4e6f 6e65 2c0a 2020 2020  _pins=None,.    
+00017090: 2020 2020 6164 645f 6262 6f78 3d4e 6f6e      add_bbox=Non
+000170a0: 652c 0a20 2020 2029 0a20 2020 2061 7373  e,.    ).    ass
+000170b0: 6572 7420 6331 2e67 6574 5f6c 6179 6572  ert c1.get_layer
+000170c0: 7328 2920 3d3d 207b 2832 2c20 3029 2c20  s() == {(2, 0), 
+000170d0: 2831 3131 2c20 3029 7d2c 2063 312e 6765  (111, 0)}, c1.ge
+000170e0: 745f 6c61 7965 7273 2829 0a20 2020 2023  t_layers().    #
+000170f0: 2072 6574 7572 6e20 6331 0a20 2020 2063   return c1.    c
+00017100: 3220 3d20 6331 2e72 656d 6f76 655f 6c61  2 = c1.remove_la
+00017110: 7965 7273 285b 2831 3131 2c20 3029 5d29  yers([(111, 0)])
+00017120: 0a20 2020 2061 7373 6572 7420 6332 2e67  .    assert c2.g
+00017130: 6574 5f6c 6179 6572 7328 2920 3d3d 207b  et_layers() == {
+00017140: 2832 2c20 3029 7d2c 2063 322e 6765 745f  (2, 0)}, c2.get_
+00017150: 6c61 7965 7273 2829 0a0a 0a64 6566 205f  layers()...def _
+00017160: 6669 6c74 6572 5f70 6f6c 7973 2870 6f6c  filter_polys(pol
+00017170: 7967 6f6e 732c 206c 6179 6572 735f 6578  ygons, layers_ex
+00017180: 636c 293a 0a20 2020 2072 6574 7572 6e20  cl):.    return 
+00017190: 5b0a 2020 2020 2020 2020 706f 6c79 676f  [.        polygo
+000171a0: 6e0a 2020 2020 2020 2020 666f 7220 706f  n.        for po
+000171b0: 6c79 676f 6e2c 206c 6179 6572 2c20 6461  lygon, layer, da
+000171c0: 7461 7479 7065 2069 6e20 7a69 7028 0a20  tatype in zip(. 
+000171d0: 2020 2020 2020 2020 2020 2070 6f6c 7967             polyg
+000171e0: 6f6e 732e 706f 6c79 676f 6e73 2c20 706f  ons.polygons, po
+000171f0: 6c79 676f 6e73 2e6c 6179 6572 732c 2070  lygons.layers, p
+00017200: 6f6c 7967 6f6e 732e 6461 7461 7479 7065  olygons.datatype
+00017210: 730a 2020 2020 2020 2020 290a 2020 2020  s.        ).    
+00017220: 2020 2020 6966 2028 6c61 7965 722c 2064      if (layer, d
+00017230: 6174 6174 7970 6529 206e 6f74 2069 6e20  atatype) not in 
+00017240: 6c61 7965 7273 5f65 7863 6c0a 2020 2020  layers_excl.    
+00017250: 5d0a 0a0a 6465 6620 7265 6375 7273 655f  ]...def recurse_
+00017260: 7374 7275 6374 7572 6573 280a 2020 2020  structures(.    
+00017270: 636f 6d70 6f6e 656e 743a 2043 6f6d 706f  component: Compo
+00017280: 6e65 6e74 2c0a 2020 2020 6967 6e6f 7265  nent,.    ignore
+00017290: 5f63 6f6d 706f 6e65 6e74 735f 7072 6566  _components_pref
+000172a0: 6978 3a20 6c69 7374 5b73 7472 5d20 7c20  ix: list[str] | 
+000172b0: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
+000172c0: 2069 676e 6f72 655f 6675 6e63 7469 6f6e   ignore_function
+000172d0: 735f 7072 6566 6978 3a20 6c69 7374 5b73  s_prefix: list[s
+000172e0: 7472 5d20 7c20 4e6f 6e65 203d 204e 6f6e  tr] | None = Non
+000172f0: 652c 0a29 202d 3e20 6469 6374 5b73 7472  e,.) -> dict[str
+00017300: 2c20 416e 795d 3a0a 2020 2020 2222 2252  , Any]:.    """R
+00017310: 6563 7572 7365 2063 6f6d 706f 6e65 6e74  ecurse component
+00017320: 2061 6e64 2063 6f6d 706f 6e65 6e74 7320   and components 
+00017330: 7265 6665 7265 6e63 6573 2072 6563 7572  references recur
+00017340: 7369 7665 6c79 2e0a 0a20 2020 2041 7267  sively...    Arg
+00017350: 733a 0a20 2020 2020 2020 2063 6f6d 706f  s:.        compo
+00017360: 6e65 6e74 3a20 636f 6d70 6f6e 656e 7420  nent: component 
+00017370: 746f 2072 6563 7572 7365 2e0a 2020 2020  to recurse..    
+00017380: 2020 2020 6967 6e6f 7265 5f63 6f6d 706f      ignore_compo
+00017390: 6e65 6e74 735f 7072 6566 6978 3a20 6c69  nents_prefix: li
+000173a0: 7374 206f 6620 7072 6566 6978 2074 6f20  st of prefix to 
+000173b0: 6967 6e6f 7265 2e0a 2020 2020 2020 2020  ignore..        
+000173c0: 6967 6e6f 7265 5f66 756e 6374 696f 6e73  ignore_functions
+000173d0: 5f70 7265 6669 783a 206c 6973 7420 6f66  _prefix: list of
+000173e0: 2070 7265 6669 7820 746f 2069 676e 6f72   prefix to ignor
+000173f0: 652e 0a20 2020 2022 2222 0a20 2020 2069  e..    """.    i
+00017400: 676e 6f72 655f 6675 6e63 7469 6f6e 735f  gnore_functions_
+00017410: 7072 6566 6978 203d 2069 676e 6f72 655f  prefix = ignore_
+00017420: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
+00017430: 206f 7220 5b5d 0a20 2020 2069 676e 6f72   or [].    ignor
+00017440: 655f 636f 6d70 6f6e 656e 7473 5f70 7265  e_components_pre
+00017450: 6669 7820 3d20 6967 6e6f 7265 5f63 6f6d  fix = ignore_com
+00017460: 706f 6e65 6e74 735f 7072 6566 6978 206f  ponents_prefix o
+00017470: 7220 5b5d 0a0a 2020 2020 6966 2028 0a20  r []..    if (. 
+00017480: 2020 2020 2020 2068 6173 6174 7472 2863         hasattr(c
+00017490: 6f6d 706f 6e65 6e74 2c20 2266 756e 6374  omponent, "funct
+000174a0: 696f 6e5f 6e61 6d65 2229 0a20 2020 2020  ion_name").     
+000174b0: 2020 2061 6e64 2063 6f6d 706f 6e65 6e74     and component
+000174c0: 2e66 756e 6374 696f 6e5f 6e61 6d65 2069  .function_name i
+000174d0: 6e20 6967 6e6f 7265 5f66 756e 6374 696f  n ignore_functio
+000174e0: 6e73 5f70 7265 6669 780a 2020 2020 293a  ns_prefix.    ):
+000174f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00017500: 7b7d 0a0a 2020 2020 6966 2068 6173 6174  {}..    if hasat
+00017510: 7472 2863 6f6d 706f 6e65 6e74 2c20 226e  tr(component, "n
+00017520: 616d 6522 2920 616e 6420 616e 7928 0a20  ame") and any(. 
+00017530: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
+00017540: 2e6e 616d 652e 7374 6172 7473 7769 7468  .name.startswith
+00017550: 2869 2920 666f 7220 6920 696e 2069 676e  (i) for i in ign
+00017560: 6f72 655f 636f 6d70 6f6e 656e 7473 5f70  ore_components_p
+00017570: 7265 6669 780a 2020 2020 293a 0a20 2020  refix.    ):.   
+00017580: 2020 2020 2072 6574 7572 6e20 7b7d 0a0a       return {}..
+00017590: 2020 2020 6f75 7470 7574 203d 207b 636f      output = {co
+000175a0: 6d70 6f6e 656e 742e 6e61 6d65 3a20 6469  mponent.name: di
+000175b0: 6374 2863 6f6d 706f 6e65 6e74 2e73 6574  ct(component.set
+000175c0: 7469 6e67 7329 7d0a 2020 2020 666f 7220  tings)}.    for 
+000175d0: 7265 6665 7265 6e63 6520 696e 2063 6f6d  reference in com
+000175e0: 706f 6e65 6e74 2e72 6566 6572 656e 6365  ponent.reference
+000175f0: 733a 0a20 2020 2020 2020 2069 6620 280a  s:.        if (.
+00017600: 2020 2020 2020 2020 2020 2020 6973 696e              isin
+00017610: 7374 616e 6365 2872 6566 6572 656e 6365  stance(reference
+00017620: 2c20 436f 6d70 6f6e 656e 7452 6566 6572  , ComponentRefer
+00017630: 656e 6365 290a 2020 2020 2020 2020 2020  ence).          
+00017640: 2020 616e 6420 7265 6665 7265 6e63 652e    and reference.
+00017650: 7265 665f 6365 6c6c 2e6e 616d 6520 6e6f  ref_cell.name no
+00017660: 7420 696e 206f 7574 7075 740a 2020 2020  t in output.    
+00017670: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00017680: 2020 206f 7574 7075 742e 7570 6461 7465     output.update
+00017690: 2872 6563 7572 7365 5f73 7472 7563 7475  (recurse_structu
+000176a0: 7265 7328 7265 6665 7265 6e63 652e 7265  res(reference.re
+000176b0: 665f 6365 6c6c 2929 0a0a 2020 2020 7265  f_cell))..    re
+000176c0: 7475 726e 206f 7574 7075 740a 0a0a 6465  turn output...de
+000176d0: 6620 666c 6174 7465 6e5f 696e 7661 6c69  f flatten_invali
+000176e0: 645f 7265 6673 5f72 6563 7572 7369 7665  d_refs_recursive
+000176f0: 280a 2020 2020 636f 6d70 6f6e 656e 743a  (.    component:
+00017700: 2043 6f6d 706f 6e65 6e74 2c0a 2020 2020   Component,.    
+00017710: 6772 6964 5f73 697a 653a 2066 6c6f 6174  grid_size: float
+00017720: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
+00017730: 2020 2020 7570 6461 7465 645f 636f 6d70      updated_comp
+00017740: 6f6e 656e 7473 3d4e 6f6e 652c 0a20 2020  onents=None,.   
+00017750: 2074 7261 7665 7273 6564 5f63 6f6d 706f   traversed_compo
+00017760: 6e65 6e74 733d 4e6f 6e65 2c0a 293a 0a20  nents=None,.):. 
+00017770: 2020 2022 2222 5265 6375 7273 6976 656c     """Recursivel
+00017780: 7920 666c 6174 7465 6e73 2063 6f6d 706f  y flattens compo
+00017790: 6e65 6e74 2072 6566 6572 656e 6365 7320  nent references 
+000177a0: 7768 6963 6820 6861 7665 2069 6e76 616c  which have inval
+000177b0: 6964 2074 7261 6e73 666f 726d 6174 696f  id transformatio
+000177c0: 6e73 2028 692e 652e 206e 6f6e 2d39 3020  ns (i.e. non-90 
+000177d0: 6465 6720 726f 7461 7469 6f6e 7320 6f72  deg rotations or
+000177e0: 2073 7562 2d67 7269 6420 7472 616e 736c   sub-grid transl
+000177f0: 6174 696f 6e73 2920 616e 6420 7265 7475  ations) and retu
+00017800: 726e 7320 6120 636f 7079 2069 6620 616e  rns a copy if an
+00017810: 7920 7375 6263 656c 6c73 2068 6176 6520  y subcells have 
+00017820: 6265 656e 206d 6f64 6966 6965 642e 0a0a  been modified...
+00017830: 2020 2020 5741 524e 494e 473a 2074 6869      WARNING: thi
+00017840: 7320 6675 6e63 7469 6f6e 2077 696c 6c20  s function will 
+00017850: 7072 6f64 7563 6520 7361 6d65 2d6e 616d  produce same-nam
+00017860: 6520 636f 7069 6573 206f 6620 6365 6c6c  e copies of cell
+00017870: 732e 2049 7420 6973 2073 7472 6963 746c  s. It is strictl
+00017880: 7920 6d65 616e 7420 746f 2062 6520 7573  y meant to be us
+00017890: 6564 206f 6e20 7772 6974 6520 6f66 2074  ed on write of t
+000178a0: 6865 2047 4453 2066 696c 6520 616e 640a  he GDS file and.
+000178b0: 2020 2020 7368 6f75 6c64 206e 6f74 2062      should not b
+000178c0: 6520 6d69 7865 6420 7769 7468 206f 7468  e mixed with oth
+000178d0: 6572 2063 656c 6c73 2c20 6f72 2079 6f75  er cells, or you
+000178e0: 2077 696c 6c20 6c69 6b65 6c79 2065 7870   will likely exp
+000178f0: 6572 6965 6e63 6520 6973 7375 6573 2077  erience issues w
+00017900: 6974 6820 6475 706c 6963 6174 6520 6365  ith duplicate ce
+00017910: 6c6c 730a 0a20 2020 2041 7267 733a 0a20  lls..    Args:. 
+00017920: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
+00017930: 3a20 7468 6520 636f 6d70 6f6e 656e 7420  : the component 
+00017940: 746f 2066 6978 2028 696e 2070 6c61 6365  to fix (in place
+00017950: 292e 0a20 2020 2020 2020 2067 7269 645f  )..        grid_
+00017960: 7369 7a65 3a20 7468 6520 4744 5320 6772  size: the GDS gr
+00017970: 6964 2073 697a 652c 2069 6e20 756d 2c20  id size, in um, 
+00017980: 6465 6661 756c 7473 2074 6f20 6163 7469  defaults to acti
+00017990: 7665 2050 444b 2e67 6574 5f67 7269 645f  ve PDK.get_grid_
+000179a0: 7369 7a65 2829 0a20 2020 2020 2020 2020  size().         
+000179b0: 2020 2061 6e79 2074 7261 6e73 6c61 7469     any translati
+000179c0: 6f6e 7320 7769 7468 2068 6967 6865 7220  ons with higher 
+000179d0: 7265 736f 6c75 7469 6f6e 2074 6861 6e20  resolution than 
+000179e0: 7468 6973 2061 7265 2063 6f6e 7369 6465  this are conside
+000179f0: 7265 6420 696e 7661 6c69 642e 0a20 2020  red invalid..   
+00017a00: 2020 2020 2075 7064 6174 6564 5f63 6f6d       updated_com
+00017a10: 706f 6e65 6e74 733a 2074 6865 2072 756e  ponents: the run
+00017a20: 6e69 6e67 2064 6963 7469 6f6e 6172 7920  ning dictionary 
+00017a30: 6f66 2063 6f6d 706f 6e65 6e74 7320 7768  of components wh
+00017a40: 6963 6820 6861 7665 2062 6565 6e20 6d6f  ich have been mo
+00017a50: 6469 6669 6564 2062 7920 7468 6973 2074  dified by this t
+00017a60: 7261 6e73 666f 726d 6174 696f 6e2e 2053  ransformation. S
+00017a70: 686f 756c 6420 616c 7761 7973 2062 6520  hould always be 
+00017a80: 4e6f 6e65 2c20 6578 6365 7074 2066 6f72  None, except for
+00017a90: 2072 6563 7572 7369 7665 2069 6e76 6f63   recursive invoc
+00017aa0: 6174 696f 6e73 2e0a 2020 2020 2020 2020  ations..        
+00017ab0: 7472 6176 6572 7365 645f 636f 6d70 6f6e  traversed_compon
+00017ac0: 656e 7473 3a20 7468 6520 7365 7420 6f66  ents: the set of
+00017ad0: 2063 6f6d 706f 6e65 6e74 206e 616d 6573   component names
+00017ae0: 2077 6869 6368 2068 6176 6520 6265 656e   which have been
+00017af0: 2074 7261 7665 7273 6564 2e20 5368 6f75   traversed. Shou
+00017b00: 6c64 2061 6c77 6179 7320 6265 204e 6f6e  ld always be Non
+00017b10: 652c 2065 7863 6570 7420 666f 7220 7265  e, except for re
+00017b20: 6375 7273 6976 6520 696e 766f 6361 7469  cursive invocati
+00017b30: 6f6e 732e 0a20 2020 2022 2222 0a20 2020  ons..    """.   
+00017b40: 2066 726f 6d20 6764 7366 6163 746f 7279   from gdsfactory
+00017b50: 2e64 6563 6f72 6174 6f72 7320 696d 706f  .decorators impo
+00017b60: 7274 2069 735f 696e 7661 6c69 645f 7265  rt is_invalid_re
+00017b70: 660a 0a20 2020 2069 6e76 616c 6964 5f72  f..    invalid_r
+00017b80: 6566 7320 3d20 5b5d 0a20 2020 2072 6566  efs = [].    ref
+00017b90: 7320 3d20 636f 6d70 6f6e 656e 742e 7265  s = component.re
+00017ba0: 6665 7265 6e63 6573 0a20 2020 2073 7562  ferences.    sub
+00017bb0: 6365 6c6c 5f6d 6f64 6966 6965 6420 3d20  cell_modified = 
+00017bc0: 4661 6c73 650a 2020 2020 6966 2075 7064  False.    if upd
+00017bd0: 6174 6564 5f63 6f6d 706f 6e65 6e74 7320  ated_components 
+00017be0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00017bf0: 2075 7064 6174 6564 5f63 6f6d 706f 6e65   updated_compone
+00017c00: 6e74 7320 3d20 7b7d 0a20 2020 2069 6620  nts = {}.    if 
+00017c10: 7472 6176 6572 7365 645f 636f 6d70 6f6e  traversed_compon
+00017c20: 656e 7473 2069 7320 4e6f 6e65 3a0a 2020  ents is None:.  
+00017c30: 2020 2020 2020 7472 6176 6572 7365 645f        traversed_
+00017c40: 636f 6d70 6f6e 656e 7473 203d 2073 6574  components = set
+00017c50: 2829 0a20 2020 2066 6f72 2072 6566 2069  ().    for ref i
+00017c60: 6e20 7265 6673 3a0a 2020 2020 2020 2020  n refs:.        
+00017c70: 2320 6d61 726b 2061 6e79 2069 6e76 616c  # mark any inval
+00017c80: 6964 2072 6566 7320 666f 7220 666c 6174  id refs for flat
+00017c90: 7465 6e69 6e67 0a20 2020 2020 2020 2023  tening.        #
+00017ca0: 206f 7468 6572 7769 7365 2c20 6368 6563   otherwise, chec
+00017cb0: 6b20 6966 2074 6865 7265 2061 7265 2061  k if there are a
+00017cc0: 6e79 206d 6f64 6966 6965 6420 6365 6c6c  ny modified cell
+00017cd0: 7320 6265 6e65 6174 6820 2877 6520 6e65  s beneath (we ne
+00017ce0: 6564 206e 6f74 2064 6f20 7468 6973 2069  ed not do this i
+00017cf0: 6620 7468 6520 7265 6620 7769 6c6c 2062  f the ref will b
+00017d00: 6520 666c 6174 7465 6e65 6420 616e 7977  e flattened anyw
+00017d10: 6179 7329 0a20 2020 2020 2020 2069 6620  ays).        if 
+00017d20: 6973 5f69 6e76 616c 6964 5f72 6566 2872  is_invalid_ref(r
+00017d30: 6566 2c20 6772 6964 5f73 697a 6529 3a0a  ef, grid_size):.
+00017d40: 2020 2020 2020 2020 2020 2020 696e 7661              inva
+00017d50: 6c69 645f 7265 6673 2e61 7070 656e 6428  lid_refs.append(
+00017d60: 7265 662e 6e61 6d65 290a 2020 2020 2020  ref.name).      
+00017d70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00017d80: 2020 2020 2320 6f74 6865 7277 6973 652c      # otherwise,
+00017d90: 2072 6563 7572 7369 7665 6c79 2066 6c61   recursively fla
+00017da0: 7474 656e 2072 6566 7320 6966 2074 6865  tten refs if the
+00017db0: 2073 7562 6365 6c6c 2068 6173 206e 6f74   subcell has not
+00017dc0: 2061 6c72 6561 6479 2062 6565 6e20 7472   already been tr
+00017dd0: 6176 6572 7365 640a 2020 2020 2020 2020  aversed.        
+00017de0: 2020 2020 6966 2072 6566 2e70 6172 656e      if ref.paren
+00017df0: 742e 6e61 6d65 206e 6f74 2069 6e20 7472  t.name not in tr
+00017e00: 6176 6572 7365 645f 636f 6d70 6f6e 656e  aversed_componen
+00017e10: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00017e20: 2020 2020 666c 6174 7465 6e5f 696e 7661      flatten_inva
+00017e30: 6c69 645f 7265 6673 5f72 6563 7572 7369  lid_refs_recursi
+00017e40: 7665 280a 2020 2020 2020 2020 2020 2020  ve(.            
+00017e50: 2020 2020 2020 2020 7265 662e 7061 7265          ref.pare
+00017e60: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+00017e70: 2020 2020 2020 2020 6772 6964 5f73 697a          grid_siz
+00017e80: 653d 6772 6964 5f73 697a 652c 0a20 2020  e=grid_size,.   
+00017e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ea0: 2075 7064 6174 6564 5f63 6f6d 706f 6e65   updated_compone
+00017eb0: 6e74 733d 7570 6461 7465 645f 636f 6d70  nts=updated_comp
+00017ec0: 6f6e 656e 7473 2c0a 2020 2020 2020 2020  onents,.        
+00017ed0: 2020 2020 2020 2020 2020 2020 7472 6176              trav
+00017ee0: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
+00017ef0: 3d74 7261 7665 7273 6564 5f63 6f6d 706f  =traversed_compo
+00017f00: 6e65 6e74 732c 0a20 2020 2020 2020 2020  nents,.         
+00017f10: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00017f20: 2020 2020 2023 206e 6f77 2c20 6966 2074       # now, if t
+00017f30: 6865 2072 6566 2773 2063 656c 6c20 6265  he ref's cell be
+00017f40: 656e 206d 6f64 6966 6965 642c 206d 6172  en modified, mar
+00017f50: 6b20 6974 2061 7320 7375 6368 0a20 2020  k it as such.   
+00017f60: 2020 2020 2020 2020 2069 6620 7265 662e           if ref.
+00017f70: 7061 7265 6e74 2e6e 616d 6520 696e 2075  parent.name in u
+00017f80: 7064 6174 6564 5f63 6f6d 706f 6e65 6e74  pdated_component
+00017f90: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00017fa0: 2020 2073 7562 6365 6c6c 5f6d 6f64 6966     subcell_modif
+00017fb0: 6965 6420 3d20 5472 7565 0a20 2020 2069  ied = True.    i
+00017fc0: 6620 696e 7661 6c69 645f 7265 6673 206f  f invalid_refs o
+00017fd0: 7220 7375 6263 656c 6c5f 6d6f 6469 6669  r subcell_modifi
+00017fe0: 6564 3a0a 2020 2020 2020 2020 6e65 775f  ed:.        new_
+00017ff0: 636f 6d70 6f6e 656e 7420 3d20 636f 6d70  component = comp
+00018000: 6f6e 656e 742e 636f 7079 2829 0a20 2020  onent.copy().   
+00018010: 2020 2020 206e 6577 5f63 6f6d 706f 6e65       new_compone
+00018020: 6e74 2e6e 616d 6520 3d20 636f 6d70 6f6e  nt.name = compon
+00018030: 656e 742e 6e61 6d65 0a20 2020 2020 2020  ent.name.       
+00018040: 2023 206d 616b 6520 7375 7265 2061 6c6c   # make sure all
+00018050: 206d 6f64 6966 6965 6420 6365 6c6c 7320   modified cells 
+00018060: 6861 7665 2074 6865 6972 2072 6566 6572  have their refer
+00018070: 656e 6365 7320 7570 6461 7465 640a 2020  ences updated.  
+00018080: 2020 2020 2020 6e65 775f 7265 6673 203d        new_refs =
+00018090: 206e 6577 5f63 6f6d 706f 6e65 6e74 2e72   new_component.r
+000180a0: 6566 6572 656e 6365 732e 636f 7079 2829  eferences.copy()
+000180b0: 0a20 2020 2020 2020 2066 6f72 2072 6566  .        for ref
+000180c0: 2069 6e20 6e65 775f 7265 6673 3a0a 2020   in new_refs:.  
+000180d0: 2020 2020 2020 2020 2020 6966 2072 6566            if ref
+000180e0: 2e6e 616d 6520 696e 2069 6e76 616c 6964  .name in invalid
+000180f0: 5f72 6566 733a 0a20 2020 2020 2020 2020  _refs:.         
+00018100: 2020 2020 2020 206e 6577 5f63 6f6d 706f         new_compo
+00018110: 6e65 6e74 2e66 6c61 7474 656e 5f72 6566  nent.flatten_ref
+00018120: 6572 656e 6365 2872 6566 290a 2020 2020  erence(ref).    
+00018130: 2020 2020 2020 2020 656c 6966 2028 0a20          elif (. 
+00018140: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00018150: 6566 2e70 6172 656e 742e 6e61 6d65 2069  ef.parent.name i
+00018160: 6e20 7570 6461 7465 645f 636f 6d70 6f6e  n updated_compon
+00018170: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
+00018180: 2020 2020 2061 6e64 2072 6566 2e70 6172       and ref.par
+00018190: 656e 7420 6973 206e 6f74 2075 7064 6174  ent is not updat
+000181a0: 6564 5f63 6f6d 706f 6e65 6e74 735b 7265  ed_components[re
+000181b0: 662e 7061 7265 6e74 2e6e 616d 655d 0a20  f.parent.name]. 
+000181c0: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
+000181d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000181e0: 662e 7061 7265 6e74 203d 2075 7064 6174  f.parent = updat
+000181f0: 6564 5f63 6f6d 706f 6e65 6e74 735b 7265  ed_components[re
+00018200: 662e 7061 7265 6e74 2e6e 616d 655d 0a20  f.parent.name]. 
+00018210: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
+00018220: 203d 206e 6577 5f63 6f6d 706f 6e65 6e74   = new_component
+00018230: 0a20 2020 2020 2020 2075 7064 6174 6564  .        updated
+00018240: 5f63 6f6d 706f 6e65 6e74 735b 636f 6d70  _components[comp
+00018250: 6f6e 656e 742e 6e61 6d65 5d20 3d20 6e65  onent.name] = ne
+00018260: 775f 636f 6d70 6f6e 656e 740a 2020 2020  w_component.    
+00018270: 7472 6176 6572 7365 645f 636f 6d70 6f6e  traversed_compon
+00018280: 656e 7473 2e61 6464 2863 6f6d 706f 6e65  ents.add(compone
+00018290: 6e74 2e6e 616d 6529 0a20 2020 2072 6574  nt.name).    ret
+000182a0: 7572 6e20 636f 6d70 6f6e 656e 740a 0a0a  urn component...
+000182b0: 6465 6620 5f63 6865 636b 5f75 6e63 6163  def _check_uncac
+000182c0: 6865 645f 636f 6d70 6f6e 656e 7473 2863  hed_components(c
+000182d0: 6f6d 706f 6e65 6e74 2c20 6d6f 6465 293a  omponent, mode):
+000182e0: 0a20 2020 2076 616c 6964 5f6d 6f64 6573  .    valid_modes
+000182f0: 203d 205b 2277 6172 6e22 2c20 2265 7272   = ["warn", "err
+00018300: 6f72 222c 2022 6967 6e6f 7265 225d 0a0a  or", "ignore"]..
+00018310: 2020 2020 6966 206d 6f64 6520 3d3d 2022      if mode == "
+00018320: 6967 6e6f 7265 223a 0a20 2020 2020 2020  ignore":.       
+00018330: 2072 6574 7572 6e0a 2020 2020 656c 6966   return.    elif
+00018340: 206d 6f64 6520 6e6f 7420 696e 2076 616c   mode not in val
+00018350: 6964 5f6d 6f64 6573 3a0a 2020 2020 2020  id_modes:.      
+00018360: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00018370: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00018380: 6622 7b6d 6f64 657d 2069 7320 6e6f 7420  f"{mode} is not 
+00018390: 6120 7661 6c69 6420 7661 6c75 6520 666f  a valid value fo
+000183a0: 7220 6f6e 5f75 6e63 6163 6865 645f 636f  r on_uncached_co
+000183b0: 6d70 6f6e 656e 742e 2054 7279 206f 6e65  mponent. Try one
+000183c0: 206f 6620 7468 6573 653a 207b 7661 6c69   of these: {vali
+000183d0: 645f 6d6f 6465 737d 2e22 0a20 2020 2020  d_modes}.".     
+000183e0: 2020 2029 0a0a 2020 2020 666f 7220 7375     )..    for su
+000183f0: 625f 636f 6d70 6f6e 656e 7420 696e 2063  b_component in c
+00018400: 6f6d 706f 6e65 6e74 2e67 6574 5f64 6570  omponent.get_dep
+00018410: 656e 6465 6e63 6965 7328 7265 6375 7273  endencies(recurs
+00018420: 6976 653d 5472 7565 293a 0a20 2020 2020  ive=True):.     
+00018430: 2020 2069 6620 6e6f 7420 7375 625f 636f     if not sub_co
+00018440: 6d70 6f6e 656e 742e 5f6c 6f63 6b65 643a  mponent._locked:
+00018450: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
+00018460: 7361 6765 203d 2028 0a20 2020 2020 2020  sage = (.       
+00018470: 2020 2020 2020 2020 2066 2243 6f6d 706f           f"Compo
+00018480: 6e65 6e74 207b 7375 625f 636f 6d70 6f6e  nent {sub_compon
+00018490: 656e 742e 6e61 6d65 2172 7d20 7761 7320  ent.name!r} was 
+000184a0: 4e4f 5420 7072 6f70 6572 6c79 206c 6f63  NOT properly loc
+000184b0: 6b65 642e 2022 0a20 2020 2020 2020 2020  ked. ".         
+000184c0: 2020 2020 2020 2022 596f 7520 6e65 6564         "You need
+000184d0: 2074 6f20 7772 6974 6520 6974 2069 6e74   to write it int
+000184e0: 6f20 6120 6675 6e63 7469 6f6e 2074 6861  o a function tha
+000184f0: 7420 6861 7320 7468 6520 4063 656c 6c20  t has the @cell 
+00018500: 6465 636f 7261 746f 722e 220a 2020 2020  decorator.".    
+00018510: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00018520: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
+00018530: 2022 7761 726e 223a 0a20 2020 2020 2020   "warn":.       
+00018540: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+00018550: 732e 7761 726e 286d 6573 7361 6765 2c20  s.warn(message, 
+00018560: 556e 6361 6368 6564 436f 6d70 6f6e 656e  UncachedComponen
+00018570: 7457 6172 6e69 6e67 2c20 7374 6163 6b6c  tWarning, stackl
+00018580: 6576 656c 3d33 290a 0a20 2020 2020 2020  evel=3)..       
+00018590: 2020 2020 2065 6c69 6620 6d6f 6465 203d       elif mode =
+000185a0: 3d20 2265 7272 6f72 223a 0a20 2020 2020  = "error":.     
+000185b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000185c0: 2055 6e63 6163 6865 6443 6f6d 706f 6e65   UncachedCompone
+000185d0: 6e74 4572 726f 7228 6d65 7373 6167 6529  ntError(message)
+000185e0: 0a0a 0a64 6566 2074 6573 745f 7361 6d65  ...def test_same
+000185f0: 5f75 6964 2829 202d 3e20 4e6f 6e65 3a0a  _uid() -> None:.
+00018600: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
+00018610: 6374 6f72 7920 6173 2067 660a 0a20 2020  ctory as gf..   
+00018620: 2063 203d 2043 6f6d 706f 6e65 6e74 2829   c = Component()
+00018630: 0a20 2020 2063 203c 3c20 6766 2e63 6f6d  .    c << gf.com
+00018640: 706f 6e65 6e74 732e 7265 6374 616e 676c  ponents.rectangl
+00018650: 6528 290a 2020 2020 6320 3c3c 2067 662e  e().    c << gf.
+00018660: 636f 6d70 6f6e 656e 7473 2e72 6563 7461  components.recta
+00018670: 6e67 6c65 2829 0a0a 2020 2020 7231 203d  ngle()..    r1 =
+00018680: 2063 2e72 6566 6572 656e 6365 735b 305d   c.references[0]
+00018690: 2e70 6172 656e 740a 2020 2020 7232 203d  .parent.    r2 =
+000186a0: 2063 2e72 6566 6572 656e 6365 735b 315d   c.references[1]
+000186b0: 2e70 6172 656e 740a 0a20 2020 2061 7373  .parent..    ass
+000186c0: 6572 7420 7231 2e75 6964 203d 3d20 7232  ert r1.uid == r2
+000186d0: 2e75 6964 2c20 6622 7b72 312e 7569 647d  .uid, f"{r1.uid}
+000186e0: 206d 7573 7420 6571 7561 6c20 7b72 322e   must equal {r2.
+000186f0: 7569 647d 220a 0a0a 6465 6620 7465 7374  uid}"...def test
+00018700: 5f6e 6574 6c69 7374 5f73 696d 706c 6528  _netlist_simple(
+00018710: 2920 2d3e 204e 6f6e 653a 0a20 2020 2069  ) -> None:.    i
+00018720: 6d70 6f72 7420 6764 7366 6163 746f 7279  mport gdsfactory
+00018730: 2061 7320 6766 0a0a 2020 2020 6320 3d20   as gf..    c = 
+00018740: 6766 2e43 6f6d 706f 6e65 6e74 2829 0a20  gf.Component(). 
+00018750: 2020 2063 3120 3d20 6320 3c3c 2067 662e     c1 = c << gf.
+00018760: 636f 6d70 6f6e 656e 7473 2e73 7472 6169  components.strai
+00018770: 6768 7428 6c65 6e67 7468 3d31 2c20 7769  ght(length=1, wi
+00018780: 6474 683d 3229 0a20 2020 2063 3220 3d20  dth=2).    c2 = 
+00018790: 6320 3c3c 2067 662e 636f 6d70 6f6e 656e  c << gf.componen
+000187a0: 7473 2e73 7472 6169 6768 7428 6c65 6e67  ts.straight(leng
+000187b0: 7468 3d32 2c20 7769 6474 683d 3229 0a20  th=2, width=2). 
+000187c0: 2020 2063 322e 636f 6e6e 6563 7428 706f     c2.connect(po
+000187d0: 7274 3d22 6f31 222c 2064 6573 7469 6e61  rt="o1", destina
+000187e0: 7469 6f6e 3d63 312e 706f 7274 735b 226f  tion=c1.ports["o
+000187f0: 3222 5d29 0a20 2020 2063 2e61 6464 5f70  2"]).    c.add_p
+00018800: 6f72 7428 226f 3122 2c20 706f 7274 3d63  ort("o1", port=c
+00018810: 312e 706f 7274 735b 226f 3122 5d29 0a20  1.ports["o1"]). 
+00018820: 2020 2063 2e61 6464 5f70 6f72 7428 226f     c.add_port("o
+00018830: 3222 2c20 706f 7274 3d63 322e 706f 7274  2", port=c2.port
+00018840: 735b 226f 3222 5d29 0a20 2020 206e 6574  s["o2"]).    net
+00018850: 6c69 7374 203d 2063 2e67 6574 5f6e 6574  list = c.get_net
+00018860: 6c69 7374 2829 0a20 2020 2023 2070 7269  list().    # pri
+00018870: 6e74 286e 6574 6c69 7374 2e70 7265 7474  nt(netlist.prett
+00018880: 7928 2929 0a20 2020 2061 7373 6572 7420  y()).    assert 
+00018890: 6c65 6e28 6e65 746c 6973 745b 2269 6e73  len(netlist["ins
+000188a0: 7461 6e63 6573 225d 2920 3d3d 2032 0a0a  tances"]) == 2..
+000188b0: 0a64 6566 2074 6573 745f 6e65 746c 6973  .def test_netlis
+000188c0: 745f 7369 6d70 6c65 5f77 6964 7468 5f6d  t_simple_width_m
+000188d0: 6973 6d61 7463 685f 7468 726f 7773 5f65  ismatch_throws_e
+000188e0: 7272 6f72 2829 202d 3e20 4e6f 6e65 3a0a  rror() -> None:.
+000188f0: 2020 2020 696d 706f 7274 2070 7974 6573      import pytes
+00018900: 740a 0a20 2020 2069 6d70 6f72 7420 6764  t..    import gd
+00018910: 7366 6163 746f 7279 2061 7320 6766 0a0a  sfactory as gf..
+00018920: 2020 2020 6320 3d20 6766 2e43 6f6d 706f      c = gf.Compo
+00018930: 6e65 6e74 2829 0a20 2020 2063 3120 3d20  nent().    c1 = 
+00018940: 6320 3c3c 2067 662e 636f 6d70 6f6e 656e  c << gf.componen
+00018950: 7473 2e73 7472 6169 6768 7428 6c65 6e67  ts.straight(leng
+00018960: 7468 3d31 2c20 7769 6474 683d 3129 0a20  th=1, width=1). 
+00018970: 2020 2063 3220 3d20 6320 3c3c 2067 662e     c2 = c << gf.
+00018980: 636f 6d70 6f6e 656e 7473 2e73 7472 6169  components.strai
+00018990: 6768 7428 6c65 6e67 7468 3d32 2c20 7769  ght(length=2, wi
+000189a0: 6474 683d 3229 0a20 2020 2063 322e 636f  dth=2).    c2.co
+000189b0: 6e6e 6563 7428 706f 7274 3d22 6f31 222c  nnect(port="o1",
+000189c0: 2064 6573 7469 6e61 7469 6f6e 3d63 312e   destination=c1.
+000189d0: 706f 7274 735b 226f 3222 5d29 0a20 2020  ports["o2"]).   
+000189e0: 2063 2e61 6464 5f70 6f72 7428 226f 3122   c.add_port("o1"
+000189f0: 2c20 706f 7274 3d63 312e 706f 7274 735b  , port=c1.ports[
+00018a00: 226f 3122 5d29 0a20 2020 2063 2e61 6464  "o1"]).    c.add
+00018a10: 5f70 6f72 7428 226f 3222 2c20 706f 7274  _port("o2", port
+00018a20: 3d63 322e 706f 7274 735b 226f 3222 5d29  =c2.ports["o2"])
+00018a30: 0a20 2020 2077 6974 6820 7079 7465 7374  .    with pytest
+00018a40: 2e72 6169 7365 7328 5661 6c75 6545 7272  .raises(ValueErr
+00018a50: 6f72 293a 0a20 2020 2020 2020 2063 2e67  or):.        c.g
+00018a60: 6574 5f6e 6574 6c69 7374 2829 0a0a 0a64  et_netlist()...d
+00018a70: 6566 2074 6573 745f 6e65 746c 6973 745f  ef test_netlist_
+00018a80: 636f 6d70 6c65 7828 2920 2d3e 204e 6f6e  complex() -> Non
+00018a90: 653a 0a20 2020 2069 6d70 6f72 7420 6764  e:.    import gd
+00018aa0: 7366 6163 746f 7279 2061 7320 6766 0a0a  sfactory as gf..
+00018ab0: 2020 2020 6320 3d20 6766 2e63 6f6d 706f      c = gf.compo
+00018ac0: 6e65 6e74 732e 6d7a 695f 6172 6d73 2829  nents.mzi_arms()
+00018ad0: 0a20 2020 206e 6574 6c69 7374 203d 2063  .    netlist = c
+00018ae0: 2e67 6574 5f6e 6574 6c69 7374 2829 0a20  .get_netlist(). 
+00018af0: 2020 2023 2070 7269 6e74 286e 6574 6c69     # print(netli
+00018b00: 7374 2e70 7265 7474 7928 2929 0a20 2020  st.pretty()).   
+00018b10: 2061 7373 6572 7420 6c65 6e28 6e65 746c   assert len(netl
+00018b20: 6973 745b 2269 6e73 7461 6e63 6573 225d  ist["instances"]
+00018b30: 2920 3d3d 2034 2c20 6c65 6e28 6e65 746c  ) == 4, len(netl
+00018b40: 6973 745b 2269 6e73 7461 6e63 6573 225d  ist["instances"]
+00018b50: 290a 0a0a 6465 6620 7465 7374 5f65 7874  )...def test_ext
+00018b60: 7261 6374 2829 202d 3e20 4e6f 6e65 3a0a  ract() -> None:.
+00018b70: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
+00018b80: 6374 6f72 7920 6173 2067 660a 0a20 2020  ctory as gf..   
+00018b90: 2063 203d 2067 662e 636f 6d70 6f6e 656e   c = gf.componen
+00018ba0: 7473 2e73 7472 6169 6768 7428 0a20 2020  ts.straight(.   
+00018bb0: 2020 2020 206c 656e 6774 683d 3130 2c0a       length=10,.
+00018bc0: 2020 2020 2020 2020 7769 6474 683d 302e          width=0.
+00018bd0: 352c 0a20 2020 2020 2020 2062 626f 785f  5,.        bbox_
+00018be0: 6c61 7965 7273 3d5b 6766 2e4c 4159 4552  layers=[gf.LAYER
+00018bf0: 2e57 4743 4c41 445d 2c0a 2020 2020 2020  .WGCLAD],.      
+00018c00: 2020 6262 6f78 5f6f 6666 7365 7473 3d5b    bbox_offsets=[
+00018c10: 335d 2c0a 2020 2020 2020 2020 7769 7468  3],.        with
+00018c20: 5f62 626f 783d 5472 7565 2c0a 2020 2020  _bbox=True,.    
+00018c30: 2020 2020 636c 6164 6469 6e67 5f6c 6179      cladding_lay
+00018c40: 6572 733d 4e6f 6e65 2c0a 2020 2020 2020  ers=None,.      
+00018c50: 2020 6164 645f 7069 6e73 3d4e 6f6e 652c    add_pins=None,
+00018c60: 0a20 2020 2020 2020 2061 6464 5f62 626f  .        add_bbo
+00018c70: 783d 4e6f 6e65 2c0a 2020 2020 290a 2020  x=None,.    ).  
+00018c80: 2020 6332 203d 2063 2e65 7874 7261 6374    c2 = c.extract
+00018c90: 286c 6179 6572 733d 5b67 662e 4c41 5945  (layers=[gf.LAYE
+00018ca0: 522e 5747 434c 4144 5d29 0a0a 2020 2020  R.WGCLAD])..    
+00018cb0: 6173 7365 7274 206c 656e 2863 2e70 6f6c  assert len(c.pol
+00018cc0: 7967 6f6e 7329 203d 3d20 322c 206c 656e  ygons) == 2, len
+00018cd0: 2863 2e70 6f6c 7967 6f6e 7329 0a20 2020  (c.polygons).   
+00018ce0: 2061 7373 6572 7420 6c65 6e28 6332 2e70   assert len(c2.p
+00018cf0: 6f6c 7967 6f6e 7329 203d 3d20 312c 206c  olygons) == 1, l
+00018d00: 656e 2863 322e 706f 6c79 676f 6e73 290a  en(c2.polygons).
+00018d10: 2020 2020 6173 7365 7274 2067 662e 4c41      assert gf.LA
+00018d20: 5945 522e 5747 434c 4144 2069 6e20 6332  YER.WGCLAD in c2
+00018d30: 2e6c 6179 6572 730a 0a0a 6465 6620 6861  .layers...def ha
+00018d40: 7368 5f66 696c 6528 6669 6c65 7061 7468  sh_file(filepath
+00018d50: 293a 0a20 2020 206d 6435 203d 2068 6173  ):.    md5 = has
+00018d60: 686c 6962 2e6d 6435 2829 0a20 2020 206d  hlib.md5().    m
+00018d70: 6435 2e75 7064 6174 6528 6669 6c65 7061  d5.update(filepa
+00018d80: 7468 2e72 6561 645f 6279 7465 7328 2929  th.read_bytes())
+00018d90: 0a20 2020 2072 6574 7572 6e20 6d64 352e  .    return md5.
+00018da0: 6865 7864 6967 6573 7428 290a 0a0a 6465  hexdigest()...de
+00018db0: 6620 7465 7374 5f62 626f 785f 7265 6665  f test_bbox_refe
+00018dc0: 7265 6e63 6528 2920 2d3e 204e 6f6e 653a  rence() -> None:
+00018dd0: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
+00018de0: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
+00018df0: 2020 6320 3d20 6766 2e43 6f6d 706f 6e65    c = gf.Compone
+00018e00: 6e74 2829 0a20 2020 2063 3120 3d20 6320  nt().    c1 = c 
+00018e10: 3c3c 2067 662e 636f 6d70 6f6e 656e 7473  << gf.components
+00018e20: 2e72 6563 7461 6e67 6c65 2873 697a 653d  .rectangle(size=
+00018e30: 2831 2e35 652d 332c 2031 2e35 652d 3329  (1.5e-3, 1.5e-3)
+00018e40: 2c20 706f 7274 5f74 7970 653d 4e6f 6e65  , port_type=None
+00018e50: 290a 2020 2020 6332 203d 2063 203c 3c20  ).    c2 = c << 
+00018e60: 6766 2e63 6f6d 706f 6e65 6e74 732e 7265  gf.components.re
+00018e70: 6374 616e 676c 6528 7369 7a65 3d28 312e  ctangle(size=(1.
+00018e80: 3565 2d33 2c20 312e 3565 2d33 292c 2070  5e-3, 1.5e-3), p
+00018e90: 6f72 745f 7479 7065 3d4e 6f6e 6529 0a20  ort_type=None). 
+00018ea0: 2020 2063 322e 786d 696e 203d 2063 312e     c2.xmin = c1.
+00018eb0: 786d 6178 0a0a 2020 2020 6173 7365 7274  xmax..    assert
+00018ec0: 2063 322e 7873 697a 6520 3d3d 2031 2e35   c2.xsize == 1.5
+00018ed0: 652d 330a 0a0a 6465 6620 7465 7374 5f72  e-3...def test_r
+00018ee0: 656d 6f76 655f 6c61 6265 6c73 2829 202d  emove_labels() -
+00018ef0: 3e20 4e6f 6e65 3a0a 2020 2020 696d 706f  > None:.    impo
+00018f00: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
+00018f10: 2067 660a 0a20 2020 2063 203d 2067 662e   gf..    c = gf.
+00018f20: 632e 7374 7261 6967 6874 2829 0a20 2020  c.straight().   
+00018f30: 2063 2e72 656d 6f76 655f 6c61 6265 6c73   c.remove_labels
+00018f40: 2829 0a0a 2020 2020 6173 7365 7274 206c  ()..    assert l
+00018f50: 656e 2863 2e6c 6162 656c 7329 203d 3d20  en(c.labels) == 
+00018f60: 300a 0a0a 6465 6620 7465 7374 5f69 6d70  0...def test_imp
+00018f70: 6f72 745f 6764 735f 7365 7474 696e 6773  ort_gds_settings
+00018f80: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
+00018f90: 696d 706f 7274 2067 6473 6661 6374 6f72  import gdsfactor
+00018fa0: 7920 6173 2067 660a 0a20 2020 2063 203d  y as gf..    c =
+00018fb0: 2067 662e 636f 6d70 6f6e 656e 7473 2e6d   gf.components.m
+00018fc0: 7a69 2829 0a20 2020 2067 6473 7061 7468  zi().    gdspath
+00018fd0: 203d 2063 2e77 7269 7465 5f67 6473 2877   = c.write_gds(w
+00018fe0: 6974 685f 6d65 7461 6461 7461 3d54 7275  ith_metadata=Tru
+00018ff0: 6529 0a20 2020 2063 3220 3d20 6766 2e69  e).    c2 = gf.i
+00019000: 6d70 6f72 745f 6764 7328 6764 7370 6174  mport_gds(gdspat
+00019010: 682c 206e 616d 653d 226d 7a69 5f73 616d  h, name="mzi_sam
+00019020: 706c 6522 2c20 7265 6164 5f6d 6574 6164  ple", read_metad
+00019030: 6174 613d 5472 7565 290a 2020 2020 6333  ata=True).    c3
+00019040: 203d 2067 662e 726f 7574 696e 672e 6164   = gf.routing.ad
+00019050: 645f 6669 6265 725f 7369 6e67 6c65 2863  d_fiber_single(c
+00019060: 3229 0a20 2020 2061 7373 6572 7420 6333  2).    assert c3
+00019070: 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f 203d  ...if __name__ =
+00019080: 3d20 225f 5f6d 6169 6e5f 5f22 3a0a 2020  = "__main__":.  
+00019090: 2020 696d 706f 7274 2067 6473 6661 6374    import gdsfact
+000190a0: 6f72 7920 6173 2067 660a 0a20 2020 2063  ory as gf..    c
+000190b0: 203d 2067 662e 632e 6d7a 6928 290a 2020   = gf.c.mzi().  
+000190c0: 2020 632e 7070 7269 6e74 5f70 6f72 7473    c.pprint_ports
+000190d0: 2829 0a0a 2020 2020 2320 6320 3d20 6766  ()..    # c = gf
+000190e0: 2e43 6f6d 706f 6e65 6e74 2829 0a20 2020  .Component().   
+000190f0: 2023 2070 203d 2063 2e61 6464 5f70 6f6c   # p = c.add_pol
+00019100: 7967 6f6e 280a 2020 2020 2320 2020 2020  ygon(.    #     
+00019110: 5b28 2d38 2c20 362c 2037 2c20 3929 2c20  [(-8, 6, 7, 9), 
+00019120: 282d 362c 2038 2c20 3137 2c20 3529 5d2c  (-6, 8, 17, 5)],
+00019130: 206c 6179 6572 3d28 312c 2030 290a 2020   layer=(1, 0).  
+00019140: 2020 2320 2920 2023 2047 4453 206c 6179    # )  # GDS lay
+00019150: 6572 7320 6172 6520 7475 706c 6573 206f  ers are tuples o
+00019160: 6620 696e 7473 2028 6275 7420 6966 2077  f ints (but if w
+00019170: 6520 7573 6520 6f6e 6c79 206f 6e65 206e  e use only one n
+00019180: 756d 6265 7220 6974 2061 7373 756d 6573  umber it assumes
+00019190: 2074 6865 206f 7468 6572 206e 756d 6265   the other numbe
+000191a0: 7220 6973 2030 290a 2020 2020 2320 632e  r is 0).    # c.
+000191b0: 7772 6974 655f 6764 7328 2268 692e 6764  write_gds("hi.gd
+000191c0: 7322 290a 2020 2020 2320 632e 7368 6f77  s").    # c.show
+000191d0: 2829 0a20 2020 2023 2070 7269 6e74 2843  ().    # print(C
+000191e0: 4f4e 462e 6c61 7374 5f73 6176 6564 5f66  ONF.last_saved_f
+000191f0: 696c 6573 290a                           iles).
```

### Comparing `gdsfactory-7.0.2/gdsfactory/component_layout.py` & `gdsfactory-7.1.0/gdsfactory/component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/component_reference.py` & `gdsfactory-7.1.0/gdsfactory/component_reference.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/C.py` & `gdsfactory-7.1.0/gdsfactory/components/C.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/L.py` & `gdsfactory-7.1.0/gdsfactory/components/L.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/__init__.py` & `gdsfactory-7.1.0/gdsfactory/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/add_fiducials.py` & `gdsfactory-7.1.0/gdsfactory/components/add_fiducials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/add_grating_couplers.py` & `gdsfactory-7.1.0/gdsfactory/components/add_grating_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/add_trenches.py` & `gdsfactory-7.1.0/gdsfactory/components/add_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/align.py` & `gdsfactory-7.1.0/gdsfactory/components/align.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/array_component.py` & `gdsfactory-7.1.0/gdsfactory/components/array_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/array_with_fanout.py` & `gdsfactory-7.1.0/gdsfactory/components/array_with_fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/array_with_via.py` & `gdsfactory-7.1.0/gdsfactory/components/array_with_via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/awg.py` & `gdsfactory-7.1.0/gdsfactory/components/awg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/bbox.py` & `gdsfactory-7.1.0/gdsfactory/components/bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/bend_circular.py` & `gdsfactory-7.1.0/gdsfactory/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/bend_circular_heater.py` & `gdsfactory-7.1.0/gdsfactory/components/bend_circular_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/bend_euler.py` & `gdsfactory-7.1.0/gdsfactory/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/bend_port.py` & `gdsfactory-7.1.0/gdsfactory/components/bend_port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/bend_s.py` & `gdsfactory-7.1.0/gdsfactory/components/bend_s.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/bezier.py` & `gdsfactory-7.1.0/gdsfactory/components/bezier.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,19 @@
     c = Component()
     bend = path.extrude(xs)
     bend_ref = c << bend
     c.add_ports(bend_ref.ports)
     c.absorb(bend_ref)
     curv = curvature(path_points, t)
     length = gf.snap.snap_to_grid(path_length(path_points))
-    min_bend_radius = gf.snap.snap_to_grid(1 / max(np.abs(curv)))
+    if max(np.abs(curv)) == 0:
+        min_bend_radius = np.inf
+    else:
+        min_bend_radius = gf.snap.snap_to_grid(1 / max(np.abs(curv)))
+
     c.info["length"] = length
     c.info["min_bend_radius"] = min_bend_radius
     c.info["start_angle"] = path.start_angle
     c.info["end_angle"] = path.end_angle
 
     if with_bbox and xs.bbox_layers:
         padding = []
```

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cavity.py` & `gdsfactory-7.1.0/gdsfactory/components/cavity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cdc.py` & `gdsfactory-7.1.0/gdsfactory/components/cdc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cdsem_all.py` & `gdsfactory-7.1.0/gdsfactory/components/cdsem_all.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cdsem_bend180.py` & `gdsfactory-7.1.0/gdsfactory/components/cdsem_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cdsem_coupler.py` & `gdsfactory-7.1.0/gdsfactory/components/cdsem_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cdsem_straight.py` & `gdsfactory-7.1.0/gdsfactory/components/cdsem_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cdsem_straight_density.py` & `gdsfactory-7.1.0/gdsfactory/components/cdsem_straight_density.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/circle.py` & `gdsfactory-7.1.0/gdsfactory/components/circle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coh_rx_dual_pol.py` & `gdsfactory-7.1.0/gdsfactory/components/coh_rx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coh_rx_single_pol.py` & `gdsfactory-7.1.0/gdsfactory/components/coh_rx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coh_tx_dual_pol.py` & `gdsfactory-7.1.0/gdsfactory/components/coh_tx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coh_tx_single_pol.py` & `gdsfactory-7.1.0/gdsfactory/components/coh_tx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/compass.py` & `gdsfactory-7.1.0/gdsfactory/components/compass.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/component_lattice.py` & `gdsfactory-7.1.0/gdsfactory/components/component_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/component_lattice_generic.py` & `gdsfactory-7.1.0/gdsfactory/components/component_lattice_generic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/component_sequence.py` & `gdsfactory-7.1.0/gdsfactory/components/component_sequence.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/copy_layers.py` & `gdsfactory-7.1.0/gdsfactory/components/copy_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler90.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler90.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler90bend.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler90bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler_adiabatic.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler_asymmetric.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler_bent.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler_bent.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler_full.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler_full.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler_ring.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler_straight.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler_straight_asymmetric.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler_straight_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/coupler_symmetric.py` & `gdsfactory-7.1.0/gdsfactory/components/coupler_symmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cross.py` & `gdsfactory-7.1.0/gdsfactory/components/cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/crossing_waveguide.py` & `gdsfactory-7.1.0/gdsfactory/components/crossing_waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv` & `gdsfactory-7.1.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv` & `gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv` & `gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv` & `gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv` & `gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv` & `gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv` & `gdsfactory-7.1.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cutback_2x2.py` & `gdsfactory-7.1.0/gdsfactory/components/cutback_2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cutback_bend.py` & `gdsfactory-7.1.0/gdsfactory/components/cutback_bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cutback_component.py` & `gdsfactory-7.1.0/gdsfactory/components/cutback_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/cutback_splitter.py` & `gdsfactory-7.1.0/gdsfactory/components/cutback_splitter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/dbr.py` & `gdsfactory-7.1.0/gdsfactory/components/dbr.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/dbr_tapered.py` & `gdsfactory-7.1.0/gdsfactory/components/dbr_tapered.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/delay_snake.py` & `gdsfactory-7.1.0/gdsfactory/components/delay_snake.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/delay_snake2.py` & `gdsfactory-7.1.0/gdsfactory/components/delay_snake2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/delay_snake3.py` & `gdsfactory-7.1.0/gdsfactory/components/delay_snake3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/delay_snake_sbend.py` & `gdsfactory-7.1.0/gdsfactory/components/delay_snake_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/dicing_lane.py` & `gdsfactory-7.1.0/gdsfactory/components/dicing_lane.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/die.py` & `gdsfactory-7.1.0/gdsfactory/components/die.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/die_bbox.py` & `gdsfactory-7.1.0/gdsfactory/components/die_bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/die_bbox_frame.py` & `gdsfactory-7.1.0/gdsfactory/components/die_bbox_frame.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/disk.py` & `gdsfactory-7.1.0/gdsfactory/components/disk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/edge_coupler_array.py` & `gdsfactory-7.1.0/gdsfactory/components/edge_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ellipse.py` & `gdsfactory-7.1.0/gdsfactory/components/ellipse.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/extend_ports_list.py` & `gdsfactory-7.1.0/gdsfactory/components/extend_ports_list.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/extension.py` & `gdsfactory-7.1.0/gdsfactory/components/extension.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/fiber.py` & `gdsfactory-7.1.0/gdsfactory/components/fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/fiber_array.py` & `gdsfactory-7.1.0/gdsfactory/components/fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/fiducial_squares.py` & `gdsfactory-7.1.0/gdsfactory/components/fiducial_squares.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ge_detector_straight_si_contacts.py` & `gdsfactory-7.1.0/gdsfactory/components/ge_detector_straight_si_contacts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_array.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_dual_pol.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_elliptical.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_elliptical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_elliptical_arbitrary.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_elliptical_lumerical.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_elliptical_trenches.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_elliptical_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_functions.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_loss.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_loss.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_loss_fiber_single.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_loss_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_rectangular.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_rectangular_arbitrary.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/grating_coupler_tree.py` & `gdsfactory-7.1.0/gdsfactory/components/grating_coupler_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/greek_cross.py` & `gdsfactory-7.1.0/gdsfactory/components/greek_cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/hline.py` & `gdsfactory-7.1.0/gdsfactory/components/hline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/interdigital_capacitor.py` & `gdsfactory-7.1.0/gdsfactory/components/interdigital_capacitor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/litho_calipers.py` & `gdsfactory-7.1.0/gdsfactory/components/litho_calipers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/litho_ruler.py` & `gdsfactory-7.1.0/gdsfactory/components/litho_ruler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/litho_steps.py` & `gdsfactory-7.1.0/gdsfactory/components/litho_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/logo.py` & `gdsfactory-7.1.0/gdsfactory/components/logo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/loop_mirror.py` & `gdsfactory-7.1.0/gdsfactory/components/loop_mirror.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mmi.py` & `gdsfactory-7.1.0/gdsfactory/components/mmi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mmi1x2.py` & `gdsfactory-7.1.0/gdsfactory/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mmi1x2_with_sbend.py` & `gdsfactory-7.1.0/gdsfactory/components/mmi1x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mmi2x2.py` & `gdsfactory-7.1.0/gdsfactory/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mmi2x2_with_sbend.py` & `gdsfactory-7.1.0/gdsfactory/components/mmi2x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mmi_90degree_hybrid.py` & `gdsfactory-7.1.0/gdsfactory/components/mmi_90degree_hybrid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mode_converter.py` & `gdsfactory-7.1.0/gdsfactory/components/mode_converter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mzi.py` & `gdsfactory-7.1.0/gdsfactory/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mzi_arm.py` & `gdsfactory-7.1.0/gdsfactory/components/mzi_arm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mzi_arms.py` & `gdsfactory-7.1.0/gdsfactory/components/mzi_arms.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mzi_lattice.py` & `gdsfactory-7.1.0/gdsfactory/components/mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mzi_pads_center.py` & `gdsfactory-7.1.0/gdsfactory/components/mzi_pads_center.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mzi_phase_shifter.py` & `gdsfactory-7.1.0/gdsfactory/components/mzi_phase_shifter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mzit.py` & `gdsfactory-7.1.0/gdsfactory/components/mzit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mzit_lattice.py` & `gdsfactory-7.1.0/gdsfactory/components/mzit_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/mzm.py` & `gdsfactory-7.1.0/gdsfactory/components/mzm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/nxn.py` & `gdsfactory-7.1.0/gdsfactory/components/nxn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/optimal_90deg.py` & `gdsfactory-7.1.0/gdsfactory/components/optimal_90deg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/optimal_hairpin.py` & `gdsfactory-7.1.0/gdsfactory/components/optimal_hairpin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/optimal_step.py` & `gdsfactory-7.1.0/gdsfactory/components/optimal_step.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/pack_doe.py` & `gdsfactory-7.1.0/gdsfactory/components/pack_doe.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/pad.py` & `gdsfactory-7.1.0/gdsfactory/components/pad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/pad_gsg.py` & `gdsfactory-7.1.0/gdsfactory/components/pad_gsg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/pads_shorted.py` & `gdsfactory-7.1.0/gdsfactory/components/pads_shorted.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/polarization_splitter_rotator.py` & `gdsfactory-7.1.0/gdsfactory/components/polarization_splitter_rotator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ramp.py` & `gdsfactory-7.1.0/gdsfactory/components/ramp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/rectangle.py` & `gdsfactory-7.1.0/gdsfactory/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/rectangle_with_slits.py` & `gdsfactory-7.1.0/gdsfactory/components/rectangle_with_slits.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/rectangular_ring.py` & `gdsfactory-7.1.0/gdsfactory/components/rectangular_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/regular_polygon.py` & `gdsfactory-7.1.0/gdsfactory/components/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/resistance_meander.py` & `gdsfactory-7.1.0/gdsfactory/components/resistance_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/resistance_sheet.py` & `gdsfactory-7.1.0/gdsfactory/components/resistance_sheet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring.py` & `gdsfactory-7.1.0/gdsfactory/components/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_crow.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_crow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_crow_couplers.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_crow_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_double.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_double_bend_coupler.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_double_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_double_heater.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_double_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_double_pn.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_double_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_section_based.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_section_based.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_single.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_single_array.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_single_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_single_bend_coupler.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_single_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_single_dut.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_single_dut.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_single_heater.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_single_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/ring_single_pn.py` & `gdsfactory-7.1.0/gdsfactory/components/ring_single_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/seal_ring.py` & `gdsfactory-7.1.0/gdsfactory/components/seal_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/snspd.py` & `gdsfactory-7.1.0/gdsfactory/components/snspd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/spiral_double.py` & `gdsfactory-7.1.0/gdsfactory/components/spiral_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/spiral_external_io.py` & `gdsfactory-7.1.0/gdsfactory/components/spiral_external_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/spiral_heater.py` & `gdsfactory-7.1.0/gdsfactory/components/spiral_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/spiral_inner_io.py` & `gdsfactory-7.1.0/gdsfactory/components/spiral_inner_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/splitter_chain.py` & `gdsfactory-7.1.0/gdsfactory/components/splitter_chain.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/splitter_tree.py` & `gdsfactory-7.1.0/gdsfactory/components/splitter_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight.py` & `gdsfactory-7.1.0/gdsfactory/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight_array.py` & `gdsfactory-7.1.0/gdsfactory/components/straight_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight_heater_doped_rib.py` & `gdsfactory-7.1.0/gdsfactory/components/straight_heater_doped_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight_heater_doped_strip.py` & `gdsfactory-7.1.0/gdsfactory/components/straight_heater_doped_strip.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight_heater_meander.py` & `gdsfactory-7.1.0/gdsfactory/components/straight_heater_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight_heater_meander_doped.py` & `gdsfactory-7.1.0/gdsfactory/components/straight_heater_meander_doped.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight_heater_metal.py` & `gdsfactory-7.1.0/gdsfactory/components/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight_pin.py` & `gdsfactory-7.1.0/gdsfactory/components/straight_pin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight_pin_slot.py` & `gdsfactory-7.1.0/gdsfactory/components/straight_pin_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/straight_rib.py` & `gdsfactory-7.1.0/gdsfactory/components/straight_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/switch_tree.py` & `gdsfactory-7.1.0/gdsfactory/components/switch_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/taper.py` & `gdsfactory-7.1.0/gdsfactory/components/taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/taper_adiabatic.py` & `gdsfactory-7.1.0/gdsfactory/components/taper_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/taper_cross_section.py` & `gdsfactory-7.1.0/gdsfactory/components/taper_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/taper_from_csv.py` & `gdsfactory-7.1.0/gdsfactory/components/taper_from_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/taper_parabolic.py` & `gdsfactory-7.1.0/gdsfactory/components/taper_parabolic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/terminator.py` & `gdsfactory-7.1.0/gdsfactory/components/terminator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/text.py` & `gdsfactory-7.1.0/gdsfactory/components/text.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/text_freetype.py` & `gdsfactory-7.1.0/gdsfactory/components/text_freetype.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/text_rectangular.py` & `gdsfactory-7.1.0/gdsfactory/components/text_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/text_rectangular_font.py` & `gdsfactory-7.1.0/gdsfactory/components/text_rectangular_font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/triangles.py` & `gdsfactory-7.1.0/gdsfactory/components/triangles.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/verniers.py` & `gdsfactory-7.1.0/gdsfactory/components/verniers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/version_stamp.py` & `gdsfactory-7.1.0/gdsfactory/components/version_stamp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/via.py` & `gdsfactory-7.1.0/gdsfactory/components/via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/via_corner.py` & `gdsfactory-7.1.0/gdsfactory/components/via_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/via_cutback.py` & `gdsfactory-7.1.0/gdsfactory/components/via_cutback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/via_stack.py` & `gdsfactory-7.1.0/gdsfactory/components/via_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/via_stack_slot.py` & `gdsfactory-7.1.0/gdsfactory/components/via_stack_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/via_stack_with_offset.py` & `gdsfactory-7.1.0/gdsfactory/components/via_stack_with_offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/wafer.py` & `gdsfactory-7.1.0/gdsfactory/components/wafer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/wire.py` & `gdsfactory-7.1.0/gdsfactory/components/wire.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/components/wire_sbend.py` & `gdsfactory-7.1.0/gdsfactory/components/wire_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/config.py` & `gdsfactory-7.1.0/gdsfactory/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from pydantic import BaseModel, BaseSettings, Field
 from rich.console import Console
 from rich.table import Table
 
 if TYPE_CHECKING:
     from loguru import Logger
 
-__version__ = "7.0.2"
+__version__ = "7.1.0"
 PathType = str | pathlib.Path
 
 home = pathlib.Path.home()
 cwd = pathlib.Path.cwd()
 module_path = pathlib.Path(__file__).parent.absolute()
 repo_path = module_path.parent
 home_path = pathlib.Path.home() / ".gdsfactory"
```

### Comparing `gdsfactory-7.0.2/gdsfactory/constants.py` & `gdsfactory-7.1.0/gdsfactory/constants.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/cross_section.py` & `gdsfactory-7.1.0/gdsfactory/cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/decorators.py` & `gdsfactory-7.1.0/gdsfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/difftest.py` & `gdsfactory-7.1.0/gdsfactory/difftest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/difftest_git.py` & `gdsfactory-7.1.0/gdsfactory/difftest_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/events.py` & `gdsfactory-7.1.0/gdsfactory/events.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/export/to_3d.py` & `gdsfactory-7.1.0/gdsfactory/export/to_3d.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/export/to_gerber.py` & `gdsfactory-7.1.0/gdsfactory/export/to_gerber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/export/to_np.py` & `gdsfactory-7.1.0/gdsfactory/export/to_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/export/to_stl.py` & `gdsfactory-7.1.0/gdsfactory/export/to_stl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/fill.py` & `gdsfactory-7.1.0/gdsfactory/fill.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/font.py` & `gdsfactory-7.1.0/gdsfactory/font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/functions.py` & `gdsfactory-7.1.0/gdsfactory/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/README.md` & `gdsfactory-7.1.0/gdsfactory/generic_tech/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/__init__.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/containers.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/containers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/get_klayout_pyxs.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/get_klayout_pyxs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/drc/errors.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/drc/errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/grain.xml`

 * *Files 2% similar despite different names*

#### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>gdsfactory</name>
   <token/>
   <hidden>false</hidden>
-  <version>7.0.2</version>
+  <version>7.1.0</version>
   <api-version/>
   <title>gdsfactory</title>
   <doc>EDA tool to layout integrated circuits</doc>
   <doc-url>https://gdsfactory.github.io/gdsfactory/</doc-url>
   <url>https://github.com/gdsfactory/gdsfactory</url>
   <license>MIT</license>
   <author>Joaquin Matres</author>
```

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/icon_128x128.png` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/icon_64x64.png` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/README.md` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/run_lvs.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

 * *Files 2% similar despite different names*

#### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>gdsfactory.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;7.0.2&quot;
+__version__ = &quot;7.1.0&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;gdsfactory&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/generic.layerstack` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/layers.lyp` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/layers.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/tech.lyt` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/tech.lyt`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs` & `gdsfactory-7.1.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/layer_map.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/layer_views.yaml` & `gdsfactory-7.1.0/gdsfactory/generic_tech/layer_views.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/generic_tech/simulation_settings.py` & `gdsfactory-7.1.0/gdsfactory/generic_tech/simulation_settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/__init__.py` & `gdsfactory-7.1.0/gdsfactory/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/boolean.py` & `gdsfactory-7.1.0/gdsfactory/geometry/boolean.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/boolean_klayout.py` & `gdsfactory-7.1.0/gdsfactory/geometry/boolean_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/boolean_polygons.py` & `gdsfactory-7.1.0/gdsfactory/geometry/boolean_polygons.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/check_duplicated_cells.py` & `gdsfactory-7.1.0/gdsfactory/geometry/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/check_exclusion.py` & `gdsfactory-7.1.0/gdsfactory/geometry/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/check_inclusion.py` & `gdsfactory-7.1.0/gdsfactory/geometry/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/check_space.py` & `gdsfactory-7.1.0/gdsfactory/geometry/check_space.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/check_width.py` & `gdsfactory-7.1.0/gdsfactory/geometry/check_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/fill_klayout.py` & `gdsfactory-7.1.0/gdsfactory/geometry/fill_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/fill_tiled.py` & `gdsfactory-7.1.0/gdsfactory/geometry/fill_tiled.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/fillet.py` & `gdsfactory-7.1.0/gdsfactory/geometry/fillet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/functions.py` & `gdsfactory-7.1.0/gdsfactory/geometry/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/invert.py` & `gdsfactory-7.1.0/gdsfactory/geometry/invert.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/layer_priority.py` & `gdsfactory-7.1.0/gdsfactory/geometry/layer_priority.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/manhattanize.py` & `gdsfactory-7.1.0/gdsfactory/geometry/manhattanize.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/maskprep.py` & `gdsfactory-7.1.0/gdsfactory/geometry/maskprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/maskprep_flat.py` & `gdsfactory-7.1.0/gdsfactory/geometry/maskprep_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/offset.py` & `gdsfactory-7.1.0/gdsfactory/geometry/offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/outline.py` & `gdsfactory-7.1.0/gdsfactory/geometry/outline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/trim.py` & `gdsfactory-7.1.0/gdsfactory/geometry/trim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/union.py` & `gdsfactory-7.1.0/gdsfactory/geometry/union.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/write_connectivity.py` & `gdsfactory-7.1.0/gdsfactory/geometry/write_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/write_drc.py` & `gdsfactory-7.1.0/gdsfactory/geometry/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/geometry/xor_diff.py` & `gdsfactory-7.1.0/gdsfactory/geometry/xor_diff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/get_factories.py` & `gdsfactory-7.1.0/gdsfactory/get_factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/get_netlist.py` & `gdsfactory-7.1.0/gdsfactory/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/get_netlist_flat.py` & `gdsfactory-7.1.0/gdsfactory/get_netlist_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/grid.py` & `gdsfactory-7.1.0/gdsfactory/grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/install.py` & `gdsfactory-7.1.0/gdsfactory/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/klive.py` & `gdsfactory-7.1.0/gdsfactory/klive.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/labels/__init__.py` & `gdsfactory-7.1.0/gdsfactory/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/labels/add_label_yaml.py` & `gdsfactory-7.1.0/gdsfactory/labels/add_label_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/labels/ehva.py` & `gdsfactory-7.1.0/gdsfactory/labels/ehva.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/labels/merge_test_metadata.py` & `gdsfactory-7.1.0/gdsfactory/labels/merge_test_metadata.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/labels/siepic.py` & `gdsfactory-7.1.0/gdsfactory/labels/siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/labels/write_labels.py` & `gdsfactory-7.1.0/gdsfactory/labels/write_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/name.py` & `gdsfactory-7.1.0/gdsfactory/name.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/pack.py` & `gdsfactory-7.1.0/gdsfactory/pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/path.py` & `gdsfactory-7.1.0/gdsfactory/path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/pdk.py` & `gdsfactory-7.1.0/gdsfactory/pdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import omegaconf
 from omegaconf import DictConfig
 from pydantic import BaseModel, Field, validator
 
 from gdsfactory.config import PATH, logger
 from gdsfactory.events import Event
 from gdsfactory.name import MAX_NAME_LENGTH
-from gdsfactory.read import cell_from_yaml
+from gdsfactory.read.from_yaml_template import cell_from_yaml_template
 from gdsfactory.show import show
 from gdsfactory.symbols import floorplan_with_block_letters
 from gdsfactory.technology import LayerStack, LayerViews
 from gdsfactory.typings import (
     CellSpec,
     Component,
     ComponentFactory,
@@ -231,15 +231,14 @@
         constants: dict of constants for the PDK.
         materials_index: material spec names to material spec, which can be:
             string: material name.
             float: refractive index.
             float, float: refractive index real and imaginary part.
             function: function of wavelength.
         routing_strategies: functions enabled to route.
-        circuit_yaml_parser: can parse different YAML formats.
         gds_write_settings: to write GDSII files.
         oasis_settings: to write OASIS files.
         cell_decorator_settings: settings for cell_without_validator decorator function in gdsfactory.cell.
         bend_points_distance: default points distance for bends in um.
 
     """
 
@@ -259,15 +258,14 @@
     sparameters_path: PathType | None = None
     modes_path: PathType | None = PATH.modes
     interconnect_cml_path: PathType | None = None
     warn_off_grid_ports: bool = False
     constants: dict[str, Any] = constants
     materials_index: dict[str, MaterialSpec] = Field(default_factory=dict)
     routing_strategies: dict[str, Callable] | None = None
-    circuit_yaml_parser: Callable = cell_from_yaml
     gds_write_settings: GdsWriteSettings = GdsWriteSettings()
     oasis_settings: OasisWriteSettings = OasisWriteSettings()
     cell_decorator_settings: CellDecoratorSettings = CellDecoratorSettings()
     bend_points_distance: float = 20 * nm
 
     @property
     def grid_size(self):
@@ -284,15 +282,14 @@
         extra = "forbid"
         fields = {
             "cross_sections": {"exclude": True},
             "cells": {"exclude": True},
             "default_symbol_factory": {"exclude": True},
             "default_decorator": {"exclude": True},
             "materials_index": {"exclude": True},
-            "circuit_yaml_parser": {"exclude": True},
         }
 
     @validator("sparameters_path")
     def is_pathlib_path(cls, path):
         return pathlib.Path(path)
 
     def validate_layers(self, layers_required: list[Layer] | None = None):
@@ -392,16 +389,15 @@
 
             for filepath in dirpath.glob("*/**/*.pic.yml"):
                 name = filepath.stem.split(".")[0]
                 if not update and name in self.cells:
                     raise ValueError(
                         f"ERROR: Cell name {name!r} from {filepath} already registered."
                     )
-                parser = self.circuit_yaml_parser
-                self.cells[name] = parser(filepath, name=name)
+                self.cells[name] = cell_from_yaml_template(filepath, name=name)
                 on_yaml_cell_registered.fire(name=name, cell=self.cells[name], pdk=self)
                 logger.info(f"{message} cell {name!r}")
 
         for k, v in kwargs.items():
             if not update and k in self.cells:
                 raise ValueError(f"ERROR: Cell name {k!r} already registered.")
             self.cells[k] = v
```

### Comparing `gdsfactory-7.0.2/gdsfactory/picmodel.py` & `gdsfactory-7.1.0/gdsfactory/picmodel.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/pixelate.py` & `gdsfactory-7.1.0/gdsfactory/pixelate.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/polygon.py` & `gdsfactory-7.1.0/gdsfactory/polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/port.py` & `gdsfactory-7.1.0/gdsfactory/port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/quickplotter.py` & `gdsfactory-7.1.0/gdsfactory/quickplotter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/__init__.py` & `gdsfactory-7.1.0/gdsfactory/read/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/from_dphox.py` & `gdsfactory-7.1.0/gdsfactory/read/from_dphox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/from_gdspaths.py` & `gdsfactory-7.1.0/gdsfactory/read/from_gdspaths.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/from_np.py` & `gdsfactory-7.1.0/gdsfactory/read/from_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/from_phidl.py` & `gdsfactory-7.1.0/gdsfactory/read/from_phidl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/from_updk.py` & `gdsfactory-7.1.0/gdsfactory/read/from_updk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/from_yaml.py` & `gdsfactory-7.1.0/gdsfactory/read/from_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/from_yaml_template.py` & `gdsfactory-7.1.0/gdsfactory/read/from_yaml_template.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/import_gds.py` & `gdsfactory-7.1.0/gdsfactory/read/import_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/read/labels.py` & `gdsfactory-7.1.0/gdsfactory/read/labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/route_info.py` & `gdsfactory-7.1.0/gdsfactory/route_info.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/__init__.py` & `gdsfactory-7.1.0/gdsfactory/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/add_electrical_pads_shortest.py` & `gdsfactory-7.1.0/gdsfactory/routing/add_electrical_pads_shortest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/add_electrical_pads_top.py` & `gdsfactory-7.1.0/gdsfactory/routing/add_electrical_pads_top.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/add_electrical_pads_top_dc.py` & `gdsfactory-7.1.0/gdsfactory/routing/add_electrical_pads_top_dc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/add_fiber_array.py` & `gdsfactory-7.1.0/gdsfactory/routing/add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/add_fiber_single.py` & `gdsfactory-7.1.0/gdsfactory/routing/add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/add_pads.py` & `gdsfactory-7.1.0/gdsfactory/routing/add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/all_angle.py` & `gdsfactory-7.1.0/gdsfactory/routing/all_angle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/auto_taper.py` & `gdsfactory-7.1.0/gdsfactory/routing/auto_taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/factories.py` & `gdsfactory-7.1.0/gdsfactory/routing/factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/fanout.py` & `gdsfactory-7.1.0/gdsfactory/routing/fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/fanout2x2.py` & `gdsfactory-7.1.0/gdsfactory/routing/fanout2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_bundle.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_bundle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_bundle_corner.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_bundle_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_bundle_from_steps.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_bundle_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_bundle_from_waypoints.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_bundle_from_waypoints.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_bundle_path_length_match.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_bundle_path_length_match.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_bundle_sbend.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_bundle_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_bundle_u.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_bundle_u.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_input_labels.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_input_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_route.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_route.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_route_astar.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_route_astar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_route_from_steps.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_route_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_route_sbend.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_route_sbend.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,22 @@
         c.add(route.references)
         c.show()
         c.plot()
 
     """
     ysize = port2.center[1] - port1.center[1]
     xsize = port2.center[0] - port1.center[0]
-    size = (xsize, ysize)
+
+    # We need to act differently if the route is orthogonal in x
+    # or orthogonal in y
+
+    if port1.orientation == 0 or port1.orientation == 180:
+        size = (xsize, ysize)
+    else:
+        size = (ysize, -xsize)
 
     bend = bend_s(size=size, **kwargs)
 
     bend_ref = bend.ref()
     bend_ref.connect(list(bend_ref.ports.keys())[0], port1)
 
     orthogonality_error = abs(abs(port1.orientation - port2.orientation) - 180)
```

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_routes_bend180.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_routes_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/get_routes_straight.py` & `gdsfactory-7.1.0/gdsfactory/routing/get_routes_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/manhattan.py` & `gdsfactory-7.1.0/gdsfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/path_length_matching.py` & `gdsfactory-7.1.0/gdsfactory/routing/path_length_matching.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/route_fiber_array.py` & `gdsfactory-7.1.0/gdsfactory/routing/route_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/route_fiber_single.py` & `gdsfactory-7.1.0/gdsfactory/routing/route_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/route_ports_to_side.py` & `gdsfactory-7.1.0/gdsfactory/routing/route_ports_to_side.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/route_quad.py` & `gdsfactory-7.1.0/gdsfactory/routing/route_quad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/route_sharp.py` & `gdsfactory-7.1.0/gdsfactory/routing/route_sharp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/route_south.py` & `gdsfactory-7.1.0/gdsfactory/routing/route_south.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/sort_ports.py` & `gdsfactory-7.1.0/gdsfactory/routing/sort_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/routing/utils.py` & `gdsfactory-7.1.0/gdsfactory/routing/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/01_component_pcell.py` & `gdsfactory-7.1.0/gdsfactory/samples/01_component_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/01_component_pcell/test_straight_wide.yml` & `gdsfactory-7.1.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/01_component_pcell_with_pins.py` & `gdsfactory-7.1.0/gdsfactory/samples/01_component_pcell_with_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml` & `gdsfactory-7.1.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/03_move.py` & `gdsfactory-7.1.0/gdsfactory/samples/03_move.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/04_connect.py` & `gdsfactory-7.1.0/gdsfactory/samples/04_connect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/05_remove_layers.py` & `gdsfactory-7.1.0/gdsfactory/samples/05_remove_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/06_remapping_layers.py` & `gdsfactory-7.1.0/gdsfactory/samples/06_remapping_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/07_flattening_device.py` & `gdsfactory-7.1.0/gdsfactory/samples/07_flattening_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/11_component_layout.py` & `gdsfactory-7.1.0/gdsfactory/samples/11_component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/12_component_refs.py` & `gdsfactory-7.1.0/gdsfactory/samples/12_component_refs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/13_component_netlist.py` & `gdsfactory-7.1.0/gdsfactory/samples/13_component_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/14_component_connectivity.py` & `gdsfactory-7.1.0/gdsfactory/samples/14_component_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/15_component_sequence1.py` & `gdsfactory-7.1.0/gdsfactory/samples/15_component_sequence1.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/16_component_sequence2.py` & `gdsfactory-7.1.0/gdsfactory/samples/16_component_sequence2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/17_ports.py` & `gdsfactory-7.1.0/gdsfactory/samples/17_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/20_components.py` & `gdsfactory-7.1.0/gdsfactory/samples/20_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/21_add_fiber_array.py` & `gdsfactory-7.1.0/gdsfactory/samples/21_add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/22_add_fiber_single.py` & `gdsfactory-7.1.0/gdsfactory/samples/22_add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/22_add_pads.py` & `gdsfactory-7.1.0/gdsfactory/samples/22_add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/23_reticle.py` & `gdsfactory-7.1.0/gdsfactory/samples/23_reticle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/23_reticle_passives_grid.py` & `gdsfactory-7.1.0/gdsfactory/samples/23_reticle_passives_grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/23_reticle_passives_pack.py` & `gdsfactory-7.1.0/gdsfactory/samples/23_reticle_passives_pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/24_doe_2.py` & `gdsfactory-7.1.0/gdsfactory/samples/24_doe_2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/24_doe_3.py` & `gdsfactory-7.1.0/gdsfactory/samples/24_doe_3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/30_lidar.py` & `gdsfactory-7.1.0/gdsfactory/samples/30_lidar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/30_lidar_pcell.py` & `gdsfactory-7.1.0/gdsfactory/samples/30_lidar_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/30_lidar_with_pads.py` & `gdsfactory-7.1.0/gdsfactory/samples/30_lidar_with_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing.py` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/big_device.py` & `gdsfactory-7.1.0/gdsfactory/samples/big_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/demo/benchmark/fill_demo.py` & `gdsfactory-7.1.0/gdsfactory/samples/demo/benchmark/fill_demo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/demo/circuits/mask.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/demo/circuits/mask.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-name: mzi_lattice_ubcpdk
+name: mzi_lattice_ubc
 pdk: ubcpdk
 
 instances:
   mzi1:
-    component: mzi_ubcpdk
+    component: mzi_ubc
     settings:
-      dy: -100
+      dy: -200
+
 
   mzi2:
-    component: mzi_ubcpdk
+    component: mzi_ubc
     settings:
       dy: -500
 
   gc1:
     component: gc_te1550
 
   gc2:
```

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-name: mzi_ubcpdk
+name: mzi_ubc
 pdk: ubcpdk
 
-
-settings:
-  dy: -100
+default_settings:
+  dy:
+    value: -20
+    description: "The length of lower MZI arm y displacement"
 
 info:
   polarization: te
   wavelength: 1.55
   description: mzi for ubcpdk
 
+
 instances:
   yr:
     component: ebeam_y_1550
   yl:
     component: ebeam_y_1550
 
 placements:
@@ -29,13 +31,13 @@
     settings:
       cross_section: strip
   route_bot:
     links:
       yl,o3: yr,o2
     routing_strategy: get_bundle_from_steps
     settings:
-      steps: [dx: 30, dy: "${settings.dy}", dx: 20]
+      steps: [dx: 30, dy: {{ dy }}, dx: 20]
       cross_section: strip
 
 ports:
   o1: yl,o1
   o2: yr,o1
```

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/demo/drc_errors.py` & `gdsfactory-7.1.0/gdsfactory/samples/demo/drc_errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/demo/drc_write.py` & `gdsfactory-7.1.0/gdsfactory/samples/demo/drc_write.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/demo/layers.py` & `gdsfactory-7.1.0/gdsfactory/samples/demo/layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/demo/lvs.py` & `gdsfactory-7.1.0/gdsfactory/samples/demo/lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/demo/pcell.py` & `gdsfactory-7.1.0/gdsfactory/samples/demo/pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/netlists/mzi.yml` & `gdsfactory-7.1.0/gdsfactory/samples/netlists/mzi.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/netlists/mzi_full.yml` & `gdsfactory-7.1.0/gdsfactory/samples/netlists/mzi_full.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/00_geometry.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/00_geometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+# ---
+# jupyter:
+#   jupytext:
+#     cell_metadata_filter: -all
+#     custom_cell_magics: kql
+#     text_representation:
+#       extension: .py
+#       format_name: percent
+#       format_version: '1.3'
+#       jupytext_version: 1.11.2
+#   kernelspec:
+#     display_name: base
+#     language: python
+#     name: python3
+# ---
+
+# %% [markdown]
 # # Component
 #
 # A `Component` is like an empty canvas, where you can add polygons, references to other Components and ports (to connect to other components)
 #
 # ![](https://i.imgur.com/oeuKGsc.png)
 #
 # In gdsfactory **all dimensions** are in **microns**
 
+# %% [markdown]
 # ## Polygons
 #
 # You can add polygons to different layers.
 
-# +
+# %%
 import gdsfactory as gf
 from gdsfactory.generic_tech import get_generic_pdk
 
 gf.config.rich_output()
 
 PDK = get_generic_pdk()
 PDK.activate()
@@ -26,21 +44,21 @@
 # (Can also be added like [(x1,y1), (x2,y2), (x3,y3), ... ]
 poly1 = c.add_polygon(
     [(-8, 6, 7, 9), (-6, 8, 17, 5)], layer=1
 )  # GDS layers are tuples of ints (but if we use only one number it assumes the other number is 0)
 
 # show it in matplotlib and KLayout (you need to have KLayout open and install gdsfactory from the git repo with make install)
 c.plot()
-# -
 
+# %% [markdown]
 # **Exercise** :
 #
 # Make a component similar to the one above that has a second polygon in layer (2, 0)
 
-# +
+# %%
 c = gf.Component("myComponent2")
 # Create some new geometry from the functions available in the geometry library
 t = gf.components.text("Hello!")
 r = gf.components.rectangle(size=[5, 10], layer=(2, 0))
 
 # Add references to the new geometry to c, our blank component
 text1 = c.add_ref(t)  # Add the text we created as a reference
@@ -53,130 +71,146 @@
 text2.move([5, 30])
 text2.rotate(45)
 r.movex(-15)
 r.movex(-15)
 
 print(c)
 c.plot()
-# -
 
+# %% [markdown]
 # You define polygons both from `gdstk` or `Shapely`
 
-# +
+# %%
 from shapely.geometry.polygon import Polygon
 
 import gdsfactory as gf
 
 c = gf.Component("Mixed_polygons")
 p0 = Polygon(zip((-8, 6, 7, 9), (-6, 8, 17, 5)))
 p1 = p0.buffer(1)
 p2 = p1.simplify(tolerance=0.1)
 c.add_polygon(p0, layer=0)
 c.add_polygon(p1, layer=1)
 c.add_polygon(p2, layer=2)
 
 c.add_polygon([(-8, 6, 7, 9), (-6, 8, 17, 5)], layer=3)
 c.plot()
-# -
 
+# %%
 p0
 
+# %%
 p1 = p0.buffer(1)
 p1
 
+# %%
 pnot = p1 - p0
 pnot
 
+# %%
 c = gf.Component("exterior")
 c.add_polygon(pnot, layer=3)
 c.plot()
 
+# %%
 p_small = p0.buffer(-1)
 p_small
 
+# %%
 p_or = pnot | p_small
 p_or
 
+# %%
 c = gf.Component("p_or")
 c.add_polygon(p_or, layer=1)
 c.plot()
 
-# +
+# %%
 import shapely as sp
 
 p5 = sp.envelope(p0)
 p5
-# -
 
+# %%
 p6 = p5 - p0
 p6
 
+# %%
 c = gf.Component("p6")
 c.add_polygon(p6, layer=1)
 c.plot()
 
+# %%
 c = gf.Component("demo_multilayer")
 p0 = c.add_polygon(p0, layer={2, 3})
 c.plot()
 
+# %%
 c = gf.Component("demo_mirror")
 p0 = c.add_polygon(p0, layer=1)
 p9 = c.add_polygon(p0, layer=2)
 p9.mirror()
 c.plot()
 
+# %%
 c = gf.Component("demo_xmin")
 p0 = c.add_polygon(p0, layer=1)
 p9 = c.add_polygon(p0, layer=2)
 p9.mirror()
 p9.xmin = p0.xmax
 c.plot()
 
+# %%
 c = gf.Component("enclosure1")
 r = c << gf.components.ring_single()
 c.plot()
 
 
+# %%
 c = gf.Component("enclosure2")
 r = c << gf.components.ring_single()
 p = c.get_polygon_bbox()
 c.add_polygon(p, layer=(2, 0))
 c.plot()
 
+# %%
 c = gf.Component("enclosure3")
 r = c << gf.components.ring_single()
 p = c.get_polygon_bbox(top=3, bottom=3)
 c.add_polygon(p, layer=(2, 0))
 c.plot()
 
+# %%
 c = gf.Component("enclosure3")
 r = c << gf.components.ring_single()
 p = c.get_polygon_enclosure()
 c.add_polygon(p, layer=(2, 0))
 c.plot()
 
+# %%
 c = gf.Component("enclosure3")
 r = c << gf.components.ring_single()
 p = c.get_polygon_enclosure()
 p2 = p.buffer(3)
 c.add_polygon(p2, layer=(2, 0))
 c.plot()
 
 
+# %% [markdown]
 # ## Connect **ports**
 #
 # Components can have a "Port" that allows you to connect ComponentReferences together like legos.
 #
 # You can write a simple function to make a rectangular straight, assign ports to the ends, and then connect those rectangles together.
 #
 # Notice that `connect` transform each reference but things won't remain connected if you move any of the references afterwards.
 #
 
 
-# +
+# %%
 @gf.cell
 def straight(length=10, width=1, layer=(1, 0)):
     WG = gf.Component()
     WG.add_polygon([(0, 0), (length, 0), (length, width), (0, width)], layer=layer)
     WG.add_port(
         name="o1", center=[0, width / 2], width=width, orientation=180, layer=layer
     )
@@ -191,43 +225,45 @@
 wg1 = c << straight(length=6, width=2.5, layer=1)
 wg2 = c << straight(length=11, width=2.5, layer=2)
 wg3 = c << straight(length=15, width=2.5, layer=3)
 wg2.movey(10).rotate(10)
 wg3.movey(20).rotate(15)
 
 c.plot()
-# -
 
+# %% [markdown]
 # Now we can connect everything together using the ports:
 #
 # Each straight has two ports: 'o1' and 'o2', respectively on the East and West sides of the rectangular straight component. These are arbitrary
 # names defined in our straight() function above
 
-# +
+# %%
 # Let's keep wg1 in place on the bottom, and connect the other straights to it.
 # To do that, on wg2 we'll grab the "o1" port and connect it to the "o2" on wg1:
 wg2.connect("o1", wg1.ports["o2"])
 # Next, on wg3 let's grab the "o1" port and connect it to the "o2" on wg2:
 wg3.connect("o1", wg2.ports["o2"])
 
 c.plot()
-# -
 
+# %% [markdown]
 # Ports can be added by copying existing ports. In the example below, ports are added at the component-level on c from the existing ports of children wg1 and wg3
 # (i.e. eastmost and westmost ports)
 
+# %%
 c.add_port("o1", port=wg1.ports["o1"])
 c.add_port("o2", port=wg3.ports["o2"])
 c.plot()
 
+# %% [markdown]
 # ## Move and rotate references
 #
 # You can move, rotate, and reflect references to Components.
 
-# +
+# %%
 c = gf.Component("straights_connected")
 
 wg1 = c << straight(length=1, layer=(1, 0))
 wg2 = c << straight(length=2, layer=(2, 0))
 wg3 = c << straight(length=3, layer=(3, 0))
 
 # Create and add a polygon from separate lists of x points and y points
@@ -247,144 +283,167 @@
 # Shift the third straight over by dx = 0, dy = 4. The translation movement consist of the difference between the values of the destination and the origin and can optionally be limited in a single axis.
 wg3.move([1, 1], [5, 5], axis="y")
 
 # Then, move again the third straight "from" x=0 "to" x=10 (dx=10)
 wg3.movex(0, 10)
 
 c.plot()
-# -
 
+# %% [markdown]
 # ## Ports
 #
 # Your straights wg1/wg2/wg3 are references to other waveguide components.
 #
 # If you want to add ports to the new Component `c` you can use `add_port`, where you can create a new port or use a reference to an existing port from the underlying reference.
 
+# %% [markdown]
 # You can access the ports of a Component or ComponentReference
 
+# %%
 wg2.ports
 
+# %% [markdown]
 # ## References
 #
 # Now that your component `c` is a multi-straight component, you can add references to that component in a new blank Component `c2`, then add two references and shift one to see the movement.
 
+# %%
 c2 = gf.Component("MultiWaveguides")
 wg1 = straight()
 wg2 = straight(layer=(2, 0))
 mwg1_ref = c2.add_ref(wg1)
 mwg2_ref = c2.add_ref(wg2)
 mwg2_ref.move(destination=[10, 10])
 c2
 
+# %%
 # Like before, let's connect mwg1 and mwg2 together
 mwg1_ref.connect(port="o2", destination=mwg2_ref.ports["o1"])
 c2
 
+# %% [markdown]
 # ## Labels
 #
 # You can add abstract GDS labels to annotate your Components, in order to record information
 # directly into the final GDS file without putting any extra geometry onto any layer
 # This label will display in a GDS viewer, but will not be rendered or printed
 # like the polygons created by `gf.components.text()`.
 
-# +
+# %%
 c2.add_label(text="First label", position=mwg1_ref.center)
 c2.add_label(text="Second label", position=mwg2_ref.center)
 
 # labels are useful for recording information
 c2.add_label(
     text=f"The x size of this\nlayout is {c2.xsize}",
     position=(c2.xmax, c2.ymax),
     layer=(10, 0),
 )
 c2
-# -
 
+# %% [markdown]
 # Another simple example
 
+# %%
 c = gf.Component("rectangle_with_label")
 r = c << gf.components.rectangle(size=(1, 1))
 r.x = 0
 r.y = 0
 c.add_label(
     text="Demo label",
     position=(0, 0),
     layer=(1, 0),
 )
 c.plot()
 
+# %% [markdown]
 # ## Boolean shapes
 #
 # If you want to subtract one shape from another, merge two shapes, or
 # perform an XOR on them, you can do that with the `boolean()` function.
 #
 #
 # The ``operation`` argument should be {not, and, or, xor, 'A-B', 'B-A', 'A+B'}.
 # Note that 'A+B' is equivalent to 'or', 'A-B' is equivalent to 'not', and
 # 'B-A' is equivalent to 'not' with the operands switched
 
+# %%
 c = gf.Component("boolean_demo")
 e1 = c.add_ref(gf.components.ellipse(layer=(2, 0)))
 e2 = c.add_ref(gf.components.ellipse(radii=(10, 6), layer=(2, 0))).movex(2)
 e3 = c.add_ref(gf.components.ellipse(radii=(10, 4), layer=(2, 0))).movex(5)
 c.plot()
 
+# %%
 c2 = gf.geometry.boolean(A=[e1, e3], B=e2, operation="A-B", layer=(2, 0))
 c2
 
+# %% [markdown]
 # ## Move Reference by port
 
+# %%
 c = gf.Component("ref_port_sample")
 mmi = c.add_ref(gf.components.mmi1x2())
 bend = c.add_ref(gf.components.bend_circular(layer=(2, 0)))
 c.plot()
 
+# %%
 bend.connect("o1", mmi.ports["o2"])  # connects follow Source, destination syntax
 c.plot()
 
+# %% [markdown]
 # ## Mirror reference
 #
 # By default the mirror works along the y-axis.
 
+# %%
 c = gf.Component("ref_mirror")
 mmi = c.add_ref(gf.components.mmi1x2())
 bend = c.add_ref(gf.components.bend_circular(layer=(2, 0)))
 c.plot()
 
+# %%
 mmi.mirror()
 c.plot()
 
 
+# %%
 mmi.mirror_y()
 c.plot()
 
+# %%
 mmi.mirror_x()
 c.plot()
 
+# %% [markdown]
 # ## Write
 #
 # You can write your Component to:
 #
 # - GDS file (Graphical Database System) or OASIS for chips.
 # - gerber for PCB.
 # - STL for 3d printing.
 
-# +
+# %%
 import gdsfactory as gf
 
 c = gf.components.cross()
 c.write_gds("demo.gds")
 c.plot()
-# -
 
+# %% [markdown]
 # You can see the GDS file in Klayout viewer.
 #
 # Sometimes you also want to save the GDS together with metadata (settings, port names, widths, locations ...) in YAML
 
+# %%
 c.write_gds("demo.gds", with_metadata=True)
 
+# %%
 c.write_oas("demo.oas")
 
+# %%
 c.write_stl("demo.stl")
 
+# %%
 scene = c.to_3d()
 scene.show()
```

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/01_references.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/01_references.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/02_movement.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/02_movement.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/03_Path_CrossSection.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/03_Path_CrossSection.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/03_cells_autoname_and_cache.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/03_cells_autoname_and_cache.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/03_layer_stack.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/03_layer_stack.py`

 * *Files 16% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 LAYER_VIEWS.layer_views["WGCLAD"].visible
 
 c_wg_clad = c.extract(layers=gf.LAYER.WGCLAD)
 c_wg_clad
 
 # ## LayerStack
 #
-# Each layer also includes the information of thickness and position of each layer.
+# Each layer also includes the information of thickness and position of each layer after fabrication.
 #
 # This LayerStack can be used for creating a 3D model with `Component.to_3d` or running Simulations.
 #
 # A GDS has different layers to describe the different fabrication process steps. And each grown layer needs thickness information and z-position in the stack.
 #
 # ![layer stack](https://i.imgur.com/GUb1Kav.png)
 #
@@ -567,7 +567,92 @@
 
     # script_path = pathlib.Path(__file__).parent.absolute() / "xsection_planarized.pyxs"
     # script_path.write_text(script)
     print(script)
 
 
 # ![xsection generic](https://i.imgur.com/H5Qiygc.png)
+
+# ## Process
+#
+# The LayerStack uses the GDS layers to generate a representation of the chip after fabrication.
+#
+# The KLayout cross-section module uses the GDS layers to return a geometric approximation of the processed wafer.
+#
+# Sometimes, however, physical process modeling is desired.
+#
+# For these purposes, Processes acting on an initial substrate "wafer stack" can be defined. The waferstack is a LayerStack representing the initial state of the wafer. The processes take in some combination of GDS layers (which may differ from their use in the resulting LayerStack), some processing parameters, and are then run in a sequence.
+#
+# For instance, the early step of the front-end-of-line of the generic process could be approximated as done in `gdsfactory.technology.layer_stack` (the process classes are described in `gdsfactory.technology.processes`):
+
+
+def get_process():
+    """Returns generic process to generate LayerStack.
+
+    Represents processing steps that will result in the GenericLayerStack, starting from the waferstack LayerStack.
+
+    based on paper https://www.degruyter.com/document/doi/10.1515/nanoph-2013-0034/html
+    """
+
+    return (
+        gf.processes.Etch(
+            name="strip_etch",
+            layer=LAYER.WG,
+            positive_tone=False,
+            depth=0.22 + 0.01,  # slight overetch for numerics
+            material="core",
+            resist_thickness=1.0,
+        ),
+        gf.processes.Etch(
+            name="slab_etch",
+            layer=LAYER.SLAB90,
+            layers_diff=[LAYER.WG],
+            depth=0.22 - 0.09,
+            material="core",
+            resist_thickness=1.0,
+        ),
+        # See gplugins.process.implant tables for ballpark numbers
+        # Adjust to your process
+        gf.processes.ImplantPhysical(
+            name="deep_n_implant",
+            layer=LAYER.N,
+            energy=100,
+            ion="P",
+            dose=1e12,
+            resist_thickness=1.0,
+        ),
+        gf.processes.ImplantPhysical(
+            name="shallow_n_implant",
+            layer=LAYER.N,
+            energy=50,
+            ion="P",
+            dose=1e12,
+            resist_thickness=1.0,
+        ),
+        gf.processes.ImplantPhysical(
+            name="deep_p_implant",
+            layer=LAYER.P,
+            energy=50,
+            ion="B",
+            dose=1e12,
+            resist_thickness=1.0,
+        ),
+        gf.processes.ImplantPhysical(
+            name="shallow_p_implant",
+            layer=LAYER.P,
+            energy=15,
+            ion="B",
+            dose=1e12,
+            resist_thickness=1.0,
+        ),
+        # "Temperatures of ~1000C for not more than a few seconds"
+        # Adjust to your process
+        # https://en.wikipedia.org/wiki/Rapid_thermal_processing
+        gf.processes.Anneal(
+            name="dopant_activation",
+            time=1,
+            temperature=1000,
+        ),
+    )
+
+
+# These process dataclasses can then be used in physical simulator plugins.
```

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_components_geometry.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_components_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_components_hierarchy.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_components_hierarchy.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_components_pack.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_components_pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_components_shapes.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_components_shapes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_routing.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_routing_electrical.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_routing_electrical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/04_routing_non_manhattan.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/04_routing_non_manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/07_mask.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/07_mask.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/08_pdk.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/08_pdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 #
 # Make sure you create a `test_components.py` file for pytest to test your PDK. See for example the tests in the [ubc PDK](https://github.com/gdsfactory/ubc)
 #
 # Pytest-regressions automatically creates the CSV and YAML files for you, as well `gdsfactory.gdsdiff` will store the reference GDS in ref_layouts and check for geometry differences using XOR.
 #
 # gdsfactory is **not** backwards compatible, which means that the package will keep improving and evolving.
 #
-# 1. To make your work stable you should install a specific version and [pin the version](https://martin-thoma.com/python-requirements/) in your `requirements.txt` or `pyproject.toml` as `gdsfactory==7.0.2` replacing `7.0.2` by whatever version you end up using.
+# 1. To make your work stable you should install a specific version and [pin the version](https://martin-thoma.com/python-requirements/) in your `requirements.txt` or `pyproject.toml` as `gdsfactory==7.1.0` replacing `7.1.0` by whatever version you end up using.
 # 2. Before you upgrade gdsfactory to a newer version make sure your tests pass to make sure that things behave as expected
 #
 #
 
 # +
 """This code tests all your cells in the PDK
```

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/08_pdk_examples.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/08_pdk_examples.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/09_pdk_import.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/09_pdk_import.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/10_yaml_component.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/10_yaml_component.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-# ---
-# jupyter:
-#   jupytext:
-#     cell_metadata_filter: -all
-#     custom_cell_magics: kql
-#     text_representation:
-#       extension: .py
-#       format_name: percent
-#       format_version: '1.3'
-#       jupytext_version: 1.11.2
-#   kernelspec:
-#     display_name: base
-#     language: python
-#     name: python3
-# ---
-
-# %% [markdown]
 # # YAML Place and AutoRoute
 #
 # You have two options for working with gdsfactory:
 #
 # 1. **python flow**: you define your layout using python functions (Parametric Cells), and connect them with routing functions.
 # 2. **YAML Place and AutoRoute**: you define your circuit (Place and Route) in YAML. From the netlist you can simulate the circuit or generate the layout.
 #
@@ -32,23 +15,16 @@
 #
 # And optionally:
 #
 # - routes: between instance ports
 # - connections: to connect instance ports to other ports (without routes)
 # - ports: define input and output circuit ports
 #
-#
-# When running this tutorial make sure you UNCOMMENT this line `%matplotlib widget` so you can see the changes in the YAML file both in KLayout and matplotlib.
-#
-# `# %matplotlib widget`  -> `%matplotlib widget`
-
-# %%
-# # %matplotlib widget
 
-# %%
+# +
 from functools import partial
 
 import ipywidgets
 from IPython.display import display
 
 import gdsfactory as gf
 from gdsfactory.generic_tech import get_generic_pdk
@@ -99,38 +75,41 @@
         settings:
             radius: 100
         links:
             bl,e4: br,e3
 """
 
 out = ipywidgets.Output()
-display(x, out)
+display_widget = ipywidgets.VBox([x, out])
+display(display_widget)
+
 
+def update_output(change):
+    out.clear_output(wait=True)  # Clear the previous output
 
-def f(change, out=out):
     try:
-        c = gf.read.from_yaml(change["new"])
-        c.show(show_ports=True)
-        c.plot_klayout()
-        out.clear_output()
+        circuit = gf.read.from_yaml(change["new"])
+        circuit.show(show_ports=True)
+        image = circuit.plot_klayout()
+        with out:
+            display(image)
     except Exception as e:
-        out.clear_output()
+        error_message = f"An error occurred: {e}"
         with out:
-            display(e)
+            display(error_message)
 
 
-x.observe(f, "value")
-f({"new": x.value})
+x.observe(update_output, "value")
+update_output({"new": x.value})
+# -
 
-# %% [markdown]
 # Lets start by defining the `instances` and `placements` section in YAML
 #
 # Lets place an `mmi_long` where you can place the `W0` port at `x=20, y=10`
 
-# %%
 x.value = """
 name: mmis
 instances:
     mmi_long:
       component: mmi1x2
       settings:
         width_mmi: 4.5
@@ -146,15 +125,14 @@
         port: o1
         x: 20
         y: 10
         mirror: False
 """
 display(x, out)
 
-# %%
 x.value = """
 name: mmi_mirror
 instances:
     mmi_long:
       component: mmi1x2
       settings:
         width_mmi: 4.5
@@ -170,26 +148,25 @@
         port: o1
         x: 20
         y: 10
         mirror: False
 """
 display(x, out)
 
-# %% [markdown]
 # ## ports
 #
 # You can expose any ports of any instance to the new Component with a `ports` section in YAML
 #
 # Lets expose all the ports from `mmi_long` into the new component.
 #
 # Ports are exposed as `new_port_name: instance_name, port_name`
 #
 # you can see the ports in `red` and subports in `blue`
 
-# %%
+# +
 x.value = """
 name: ports_demo
 instances:
     mmi_long:
       component: mmi1x2
       settings:
         width_mmi: 4.5
@@ -204,21 +181,21 @@
 ports:
     o3: mmi_long,o3
     o2: mmi_long,o2
     o1: mmi_long,o1
 """
 
 display(x, out)
+# -
 
-# %% [markdown]
 # You can also define a mirror placement using a port
 #
 # Try mirroring with other ports `o2`, `o3` or with a number as well as with a rotation `90`, `180`, `270`
 
-# %%
+# +
 x.value = """
 name: mirror_demo
 instances:
     mmi_long:
       component: mmi1x2
       settings:
         width_mmi: 4.5
@@ -228,25 +205,25 @@
         x: 0
         y: 0
         mirror: o1
         rotation: 0
 """
 
 display(x, out)
+# -
 
-# %% [markdown]
 # ## connections
 #
 # You can connect any two instances by defining a `connections` section in the YAML file.
 #
 # it follows the syntax.
 #
 # `instance_source,port : instance_destination,port`
 
-# %%
+# +
 x.value = """
 name: connections_demo
 instances:
     b:
       component: bend_circular
     mmi_long:
       component: mmi1x2
@@ -270,23 +247,23 @@
 ports:
     o1: mmi_short,o1
     o2: mmi_long,o2
     o3: mmi_long,o3
 """
 
 display(x, out)
+# -
 
-# %% [markdown]
 # **Relative port placing**
 #
 # You can also place a component with respect to another instance port
 #
 # You can also define an x and y offset with `dx` and `dy`
 
-# %%
+# +
 x.value = """
 name: rel_port_placing
 instances:
     mmi_long:
       component: mmi1x2
       settings:
         width_mmi: 4.5
@@ -308,16 +285,16 @@
         y: mmi_short,o2
         dx : 10
         dy: -10
 """
 
 
 display(x, out)
+# -
 
-# %% [markdown]
 # ## routes
 #
 # You can define routes between two instances by defining a `routes` section in YAML
 #
 # it follows the syntax
 #
 # ```YAML
@@ -328,15 +305,15 @@
 #             instance_source,port: instance_destination,port
 #         settings:  # for the route (optional)
 #             waveguide: strip
 #             width: 1.2
 #
 # ```
 
-# %%
+# +
 x.value = """
 name: with_routes
 instances:
     mmi_long:
       component: mmi1x2
       settings:
         width_mmi: 4.5
@@ -358,36 +335,33 @@
             cross_section:
                 cross_section: strip
                 settings:
                     layer: [2, 0]
 """
 
 display(x, out)
+# -
 
-# %% [markdown]
 # You can **rotate** and instance specifying the angle in degrees
 
-# %% [markdown]
 # You can also access the routes in the newly created component
 
-# %% [markdown]
 # ## instances, placements, connections, ports, routes
 #
 # Lets combine all you learned so far.
 #
 # You can define the netlist connections of a component by a netlist in YAML format
 #
 # Note that you define the connections as `instance_source.port ->
 # instance_destination.port` so the order is important and therefore you can only
 # change the position of the `instance_destination`
 
-# %% [markdown]
 # You can define several routes that will be connected using `gf.routing.get_bundle`
 
-# %%
+# +
 x.value = """
 name: connections_2x2_problem
 
 instances:
     mmi_bottom:
       component: mmi2x2
     mmi_top:
@@ -403,34 +377,34 @@
         links:
             mmi_bottom,o4: mmi_top,o1
             mmi_bottom,o3: mmi_top,o2
 
 """
 
 display(x, out)
+# -
 
-# %% [markdown]
 # You can also add custom component_factories to `gf.read.from_yaml`
 #
 
 
-# %%
+# +
 @gf.cell
 def pad_new(size=(100, 100), layer=gf.LAYER.WG):
     c = gf.Component()
     compass = c << gf.components.compass(size=size, layer=layer)
     c.ports = compass.ports
     return c
 
 
 gf.get_active_pdk().register_cells(pad_new=pad_new)
 c = pad_new(cache=False)
 f = c.plot()
 
-# %%
+# +
 x.value = """
 name: connections_2x2_problem
 
 instances:
     bot:
       component: pad_new
     top:
@@ -440,15 +414,15 @@
     top:
         x: 0
         y: 200
 """
 
 display(x, out)
 
-# %%
+# +
 x.value = """
 name: custom_routes
 
 instances:
     t:
       component: pad_array
       settings:
@@ -472,19 +446,19 @@
             end_straight_length: 150
         links:
             t,e11: b,e11
             t,e13: b,e13
 """
 
 display(x, out)
+# -
 
-# %% [markdown]
 # Also, you can define route aliases, that have different settings and specify the route `factory` as a parameter as well as the `settings` for that particular route alias.
 
-# %%
+# +
 x.value = """
 name: sample_settings
 
 instances:
     bl:
       component: pad
     tl:
@@ -522,15 +496,15 @@
             layer: [31, 0]
         links:
             bl,e3: br,e3
 """
 
 display(x, out)
 
-# %%
+# +
 x.value = """
 instances:
     t:
       component: pad_array
       settings:
           orientation: 270
           columns: 3
@@ -556,15 +530,15 @@
             t,e11: b,e11
             t,e12: b,e12
             t,e13: b,e13
 """
 
 display(x, out)
 
-# %%
+# +
 x.value = """
 
 instances:
     t:
       component: pad_array
       settings:
           orientation: 270
@@ -590,15 +564,15 @@
         links:
             t,e11: b,e11
             t,e12: b,e12
 """
 
 display(x, out)
 
-# %%
+# +
 x.value = """
 instances:
     t:
       component: pad_array
       settings:
           orientation: 270
           columns: 3
@@ -625,24 +599,23 @@
         links:
             b,e11: t,e11
             b,e12: t,e12
 
 """
 
 display(x, out)
+# -
 
-# %% [markdown]
 # Note that you define the connections as `instance_source.port -> instance_destination.port` so the order is important and therefore you can only change the position of the `instance_destination`
 
-# %% [markdown]
 # ## Custom factories
 #
 # You can leverage netlist defined components to define more complex circuits
 
-# %%
+# +
 mmi1x2_faba = partial(gf.components.mmi1x2, length_mmi=30)
 mmi2x2_faba = partial(gf.components.mmi2x2, length_mmi=30)
 gf.get_active_pdk().register_cells(mmi1x2_faba=mmi1x2_faba, mmi2x2_faba=mmi2x2_faba)
 
 x.value = """
 name: sample_custom_cells
 instances:
@@ -665,59 +638,30 @@
     o1: mmib,o1
     o2: mmit,o2
     o3: mmit,o3
     o4: mmit,o4
 """
 
 display(x, out)
+# -
 
-# %%
 c = gf.components.mzi()
 c.plot()
 
-# %%
 c.plot_netlist()
 
-# %%
 n = c.get_netlist()
 
-# %%
 print(c.get_netlist().keys())
 
-# %% [markdown]
-# ## variables
-#
+# ## Jinja Pcells
 #
-# You can define a global variables `settings` in your YAML file, and use the variable in the other YAML settings by using `${settings.length_mmi}`
+# You use jinja templates in YAML cells to define Pcells.
 
-# %%
-x.value = """
-settings:
-    length_mmi: 10
-
-instances:
-    mmi_long:
-      component: mmi1x2
-      settings:
-        width_mmi: 4.5
-        length_mmi: ${settings.length_mmi}
-    mmi_short:
-      component: mmi1x2
-      settings:
-        width_mmi: 4.5
-        length_mmi: 5
-"""
-
-display(x, out)
-
-# %% [markdown]
-# ## `cell_from_yaml_template`: Jinja-template-based Parser
-# An optional parser variant is also available which is capable of parsing jinja templating directives within the yaml-based cells. This can give python-like flexibility inside the otherwise declaratively-defined yaml circuit syntax.
-
-# %%
+# +
 from IPython.display import Code
 
 from gdsfactory.read import cell_from_yaml_template
 
 gf.clear_cache()
 
 jinja_yaml = """
@@ -754,37 +698,31 @@
     f.write(jinja_yaml)
 
 pic_cell = cell_from_yaml_template(pic_filename, name="demo_jinja")
 gf.get_active_pdk().register_cells(
     demo_jinja=pic_cell
 )  # let's register this cell so we can use it later
 Code(filename=pic_filename, language="yaml+jinja")
+# -
 
-# %% [markdown]
 # You'll see that this generated a python function, with a real signature, default arguments, docstring and all!
 
-# %%
-# pic_cell?
+help(pic_cell)
 
-# %% [markdown]
 # You can invoke this cell without arguments to see the default implementation
 
-# %%
 pic_cell()
 
-# %% [markdown]
 # Or you can provide arguments explicitly, like a normal cell. Note however that yaml-based cells **only accept keyword arguments**, since yaml dictionaries are inherently unordered.
 
-# %%
 pic_cell(length_mmi=100)
 
-# %% [markdown]
 # The power of jinja-templated cells become more apparent with more complex cells, like the following.
 
-# %%
+# +
 gf.clear_cache()
 
 jinja_yaml = """
 default_settings:
     length_mmis:
       value: [10, 20, 30, 100]
       description: "An array of mmi lengths for the DOE"
@@ -829,47 +767,35 @@
 pic_filename = "demo_jinja_loops.pic.yml"
 
 with open(pic_filename, mode="w") as f:
     f.write(jinja_yaml)
 
 big_cell = cell_from_yaml_template(pic_filename, name="demo_jinja_loops")
 Code(filename=pic_filename, language="yaml+jinja")
+# -
 
-# %%
 bc = big_cell()
-bc
+bc.plot()
 
-# %%
 bc2 = big_cell(
     length_mmis=[10, 20, 40, 100, 200, 150, 10, 40],
     spacing_mmi=60,
     mmi_component="demo_jinja",
 )
-bc2
+bc2.plot()
 
-# %% [markdown]
-# ## Choosing your preferred yaml parser
-#
-
-# %% [markdown]
 # In general, the jinja-yaml parser has a superset of the functionalities and syntax of the standard yaml parser. The one notable exception is with `settings`. When reading any yaml files with `settings` blocks, the default settings will be read and applied, but they will not be settable, as the jinja parser has a different mechanism for setting injection with the `default_settings` block and jinja2.
 
-# %%
+# +
 pic_filename = "demo_backwards_compatibility.pic.yml"
 
 with open(pic_filename, mode="w") as f:
     f.write(x.value)
 
 retro_cell = cell_from_yaml_template(
     pic_filename, name="demo_jinja_backwards_compatible"
 )
 Code(filename=pic_filename, language="yaml")
+# -
 
-# %%
 retro_cell()  # this is fine-- because cell_from_yaml_template internally calls from_yaml, cells should work from their default state
 # retro_cell(length_mmi=15) # this fails-- you must use "default_settings" and jinja syntax with the yaml-jinja parser for settings to be settable
-
-# %% [markdown]
-# Because of this incompatibility, you must choose one parser or another to be used by default at the scope of the PDK.
-
-# %%
-gf.get_active_pdk().circuit_yaml_parser = cell_from_yaml_template
```

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/11_get_netlist.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/11_get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/11_get_netlist_spice.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/11_get_netlist_spice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/21_drc.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/21_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/_0_python.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/_0_python.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/_1_git.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/_1_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/_2_klayout.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/_2_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/_3_vscode.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/_3_vscode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/_4_gdsfactory.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/_4_gdsfactory.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/common_mistakes.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/common_mistakes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/dataprep.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/dataprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/declarative_cell.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/declarative_cell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/images/inkscape_align.png` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/images/inkscape_align.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/images/inkscape_distribute.png` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/images/inkscape_distribute.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/images/pathlength_report.png` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/images/pathlength_report.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/images/pathlength_report_highlighted.png` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/images/pathlength_report_highlighted.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/rib_strip_autotransition.py` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/rib_strip_autotransition.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   jupytext:
 #     cell_metadata_filter: -all
 #     custom_cell_magics: kql
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.6
+#       jupytext_version: 1.11.2
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
@@ -38,15 +38,14 @@
 from gdsfactory.route_info import route_info
 from gdsfactory.routing import all_angle
 from gdsfactory.typings import CrossSectionSpec
 
 gf.clear_cache()
 gf.config.rich_output()
 generic_pdk = get_generic_pdk()
-generic_pdk.circuit_yaml_parser = cell_from_yaml_template
 
 # define our rib and strip waveguide intent layers
 RIB_INTENT_LAYER = (2000, 11)
 STRIP_INTENT_LAYER = (2001, 11)
 
 # create strip and rib cross-sections, with differentiated intent layers
 strip_with_intent = partial(
```

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back2.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back2.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back3.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back3.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_bundles01.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_bundles02.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles02.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_bundles03.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles03.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_indirect.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_indirect.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_simple.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_simple.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_steps01.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_final.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_final.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_initial.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_initial.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_steps03.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps03.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/notebooks/yaml_pics/aar_wonky_connector.pic.yml` & `gdsfactory-7.1.0/gdsfactory/samples/notebooks/yaml_pics/aar_wonky_connector.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/fab_c.py` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/fab_d/phase_shifters.py` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c.py` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml` & `gdsfactory-7.1.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/serialization.py` & `gdsfactory-7.1.0/gdsfactory/serialization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/show.py` & `gdsfactory-7.1.0/gdsfactory/show.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/simulation/__init__.py` & `gdsfactory-7.1.0/gdsfactory/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/snap.py` & `gdsfactory-7.1.0/gdsfactory/snap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/symbols.py` & `gdsfactory-7.1.0/gdsfactory/symbols.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/technology/klayout_tech.py` & `gdsfactory-7.1.0/gdsfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/technology/layer_map.py` & `gdsfactory-7.1.0/gdsfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/technology/layer_stack.py` & `gdsfactory-7.1.0/gdsfactory/technology/layer_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         refractive_index: refractive_index
             can be int, complex or function that depends on wavelength (um).
         type: grow, etch, implant, or background.
         mode: octagon, taper, round.
             https://gdsfactory.github.io/klayout_pyxs/DocGrow.html
         into: etch into another layer.
             https://gdsfactory.github.io/klayout_pyxs/DocGrow.html
-        doping_concentration: for implants.
+        background_doping_concentration: uniform base doping level in the material (cm-3)
+        background_doping_ion: uniform base doping ion in the material
+        orientation: of the wafer (Miller indices of the plane)
         resistivity: for metals.
         bias: in um for the etch. Can be a single number or 2 numbers (bias_x, bias_y)
         derived_layer: Optional derived layer, used for layer_type='etch' to define the slab.
         info: simulation_info and other types of metadata.
     """
 
     layer: tuple[int, int] | None
@@ -50,23 +52,25 @@
     sidewall_angle_tolerance: float | None = None
     width_to_z: float = 0.0
     z_to_bias: tuple[list[float], list[float]] | None = None
     mesh_order: int = 3
     layer_type: Literal["grow", "etch", "implant", "background"] = "grow"
     mode: Literal["octagon", "taper", "round"] | None = None
     into: list[str] | None = None
-    doping_concentration: float | None = None
     resistivity: float | None = None
     bias: tuple[float, float] | float | None = None
     derived_layer: tuple[int, int] | None = None
     info: dict[str, Any] = {}
+    background_doping_concentration: float | None = None
+    background_doping_ion: str | None = None
+    orientation: str | None = "100"
 
 
 class LayerStack(BaseModel):
-    """For simulation and 3D rendering.
+    """For simulation and 3D rendering. Captures design intent of the chip layers after fabrication.
 
     Parameters:
         layers: dict of layer_levels.
     """
 
     layers: dict[str, LayerLevel] | None = Field(default_factory=dict)
 
@@ -433,14 +437,28 @@
         layers = [
             layers_to_layername[layer]
             for layer in layerspecs
             if layer in layers_to_layername
         ]
         return self.filtered(layers)
 
+    def z_offset(self, dz):
+        """Translates the z-coordinates of the layerstack."""
+        for layer in self.layers.values():
+            layer.zmin += dz
+
+        return self
+
+    def invert_zaxis(self):
+        """Flips the zmin values about the origin."""
+        for layer in self.layers.values():
+            layer.zmin *= -1
+
+        return self
+
 
 if __name__ == "__main__":
     import gdsfactory as gf
     from gdsfactory.generic_tech import get_generic_pdk
 
     PDK = get_generic_pdk()
     PDK.activate()
```

### Comparing `gdsfactory-7.0.2/gdsfactory/technology/layer_views.py` & `gdsfactory-7.1.0/gdsfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/technology/xml_utils.py` & `gdsfactory-7.1.0/gdsfactory/technology/xml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/technology/yaml_utils.py` & `gdsfactory-7.1.0/gdsfactory/technology/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/typings.py` & `gdsfactory-7.1.0/gdsfactory/typings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/gdsfactory/watch.py` & `gdsfactory-7.1.0/gdsfactory/watch.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from collections.abc import Callable
 
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 
 from gdsfactory.config import cwd
 from gdsfactory.pdk import get_active_pdk
+from gdsfactory.read.from_yaml_template import cell_from_yaml_template
 
 
 class FileWatcher(FileSystemEventHandler):
     """Captures *.py or *.pic.yml file change events."""
 
     def __init__(self, logger=None, path: str | None = None) -> None:
         """Initialize the YAML event handler."""
@@ -64,16 +65,15 @@
 
         pdk = get_active_pdk()
         print(f"Active PDK: {pdk.name}")
         filepath = pathlib.Path(src_path)
         cell_name = filepath.stem.split(".")[0]
         if cell_name in CACHE:
             CACHE.pop(cell_name)
-        parser = pdk.circuit_yaml_parser
-        function = parser(filepath, name=cell_name)
+        function = cell_from_yaml_template(filepath, name=cell_name)
         try:
             pdk.register_cells_yaml(**{cell_name: function}, update=update)
         except ValueError as e:
             print(e)
         return function
 
     def on_moved(self, event) -> None:
@@ -155,15 +155,17 @@
         datefmt="%Y-%m-%d %H:%M:%S",
     )
     if pdk:
         pdk_module = importlib.import_module(pdk)
         pdk_module.PDK.activate()
     watcher = FileWatcher(path=path)
     watcher.start()
-    logging.info(f"Observing {path!r}")
+    logging.info(
+        f"File watcher looking for changes in *.py and *.pic.yml files in {path!r}. Stop with Ctrl+C"
+    )
 
     try:
         while True:
             time.sleep(1)
     except KeyboardInterrupt:
         watcher.stop()
```

### Comparing `gdsfactory-7.0.2/gdsfactory/write_cells.py` & `gdsfactory-7.1.0/gdsfactory/write_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.2/pyproject.toml` & `gdsfactory-7.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ]
 description = "python library to generate GDS layouts"
 keywords = ["eda", "photonics", "python"]
 license = {file = "LICENSE"}
 name = "gdsfactory"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "7.0.2"
+version = "7.1.0"
 
 [project.optional-dependencies]
 cad = [
   "freetype-py",
   "ipycytoscape",
   "ipyevents",
   "ipykernel",
```

### Comparing `gdsfactory-7.0.2/PKG-INFO` & `gdsfactory-7.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsfactory
-Version: 7.0.2
+Version: 7.1.0
 Summary: python library to generate GDS layouts
 Keywords: eda,photonics,python
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -66,15 +66,15 @@
 Requires-Dist: jupyter-book==0.15.1 ; extra == "docs"
 Requires-Dist: pydata_sphinx_theme==0.13.1 ; extra == "docs"
 Requires-Dist: plotly ; extra == "docs"
 Provides-Extra: cad
 Provides-Extra: dev
 Provides-Extra: docs
 
-# gdsfactory 7.0.2
+# gdsfactory 7.1.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![Downloads](https://pepy.tech/badge/gdsfactory)](https://pepy.tech/project/gdsfactory)
@@ -128,76 +128,31 @@
 You can also access:
 
 - instructions on [how to build your own PDK](https://gdsfactory.github.io/gdsfactory/notebooks/08_pdk.html)
 - instructions on [how to import a PDK from a library of fixed GDS cells](https://gdsfactory.github.io/gdsfactory/notebooks/09_pdk_import.html)
 
 ![foundry-pdks](https://i.imgur.com/zngqi0B.png)
 
-## Installation
-
-We support Python 3.10 or 3.11, and [VSCode](https://code.visualstudio.com/) as an IDE. If you do not have Python installed, you can [download Anaconda](https://www.anaconda.com/download/).
-
-Upon Python installation, open Anaconda Prompt as Administrator and install the latest gdsfactory core conda (from the conda-forge channel) and Optional `cad` visualization extras using pip.
-
-![anaconda prompt](https://i.imgur.com/eKk2bbs.png)
-
-
-```
-conda install -c conda-forge gdsfactory -y
-pip install "gdsfactory[cad]"--upgrade
-```
-
-Then you can install Klayout-live `klive` integration in the klayout GUI `Tools --> Manage Packages --> Install New Packages --> Klive` as well as the genericpdk layermap `Tools --> Manage Packages --> Install New Packages --> gdsfactory` and restart klayout.
-
-### Update gdsfactory
-
-You can upgrade your gdsfactory package using the following command:
-
-```
-pip install gdsfactory[cad] --upgrade
-```
-
-Please note that some PDKs may only work for a specific version of gdsfactory. Ensure you install the correct gdsfactory version specified in the pyproject.toml file. This will automatically happen when you install gdsfactory as one of the PDK dependencies. For example, pip install gf180 will install the latest gdsfactory version tested for the GlobalFoundries180 PDK.
-
-To determine your current gdsfactory version, use the following code:
-
-```
-import gdsfactory as gf
-
-gf.config.print_version()
-```
-
-### Docker container
-
-As an alternative, you can use the pre-built Docker image from [hub.docker.com/r/joamatab/gdsfactory](https://hub.docker.com/r/joamatab/gdsfactory) or build it yourself with:
-
-
-```bash
-docker build -t joamatab/gdsfactory .
-```
-
-For instance, VS Code supports development inside a container. See [Developing inside a Container](https://code.visualstudio.com/docs/devcontainers/containers) for details.
-
-## Plugins
-
-We maintain gdsfactory plugins in a [separate package](https://github.com/gdsfactory/gplugins)
-These plugins enable interfaces with different tools, and you might need to install some of the tools separately.
-For more details, please visit the [gplugins documentation](https://gdsfactory.github.io/gplugins/).
 
 ## Getting started
 
 - [See slides](https://docs.google.com/presentation/d/1_ZmUxbaHWo_lQP17dlT1FWX-XD8D9w7-FcuEih48d_0/edit#slide=id.g11711f50935_0_5)
 - [Read docs](https://gdsfactory.github.io/gdsfactory/)
 - [![Video Tutorials](https://img.shields.io/badge/youtube-Video_Tutorials-red.svg?logo=youtube)](https://www.youtube.com/@gdsfactory625/playlists)
 - [![Join the chat at https://gitter.im/gdsfactory-dev/community](https://badges.gitter.im/gdsfactory-dev/community.svg)](https://gitter.im/gdsfactory-dev/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 - See announcements on [GitHub](https://github.com/gdsfactory/gdsfactory/discussions/547), [google-groups](https://groups.google.com/g/gdsfactory) or [LinkedIn](https://www.linkedin.com/company/gdsfactory)
 - Run notebooks on [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gdsfactory/binder-sandbox/HEAD)
 - [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=250169028)
 
-## Testimonals
+## Who is using gdsfactory?
+
+Hundreds of organisations are using gdsfactory. Some companies and organizations around the world using gdsfactory include:
+
+![logos](https://i.imgur.com/IqTUq9S.png)
+
 
 "I've used **gdsfactory** since 2017 for all my chip tapeouts. I love that it is fast, easy to use, and easy to extend. It's the only tool that allows us to have an end-to-end chip design flow (design, verification and validation)."
 
 <div style="text-align: right; margin-right: 10%;">Joaquin Matres - <strong>Google</strong></div>
 
 ---
```

