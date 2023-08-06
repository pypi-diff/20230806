# Comparing `tmp/sigmaepsilon.mesh-0.0.2.tar.gz` & `tmp/sigmaepsilon.mesh-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaepsilon.mesh-0.0.2.tar", last modified: Wed Jul 12 18:56:36 2023, max compression
+gzip compressed data, was "sigmaepsilon.mesh-0.0.3.tar", last modified: Sun Aug  6 17:04:15 2023, max compression
```

## Comparing `sigmaepsilon.mesh-0.0.2.tar` & `sigmaepsilon.mesh-0.0.3.tar`

### file list

```diff
@@ -1,189 +1,192 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.881482 sigmaepsilon.mesh-0.0.2/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6009 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/.readthedocs.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8593 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6291 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.881482 sigmaepsilon.mesh-0.0.2/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/make.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      322 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.881482 sigmaepsilon.mesh-0.0.2/docs/source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/README_link.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.885482 sigmaepsilon.mesh-0.0.2/docs/source/_static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/logo.PNG
--rw-r--r--   0 circleci  (1001) circleci  (1002)    57097 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot1.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   131843 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot2.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   179580 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot3.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61611 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot4.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91565 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot4a.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    89629 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot5.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    88428 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot6.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   181162 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/plot7.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    50423 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_1.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    47062 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_2.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   132201 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_3.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106791 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_4.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   132473 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_5.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.885482 sigmaepsilon.mesh-0.0.2/docs/source/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_cells.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_db.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_recipes.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_space.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_topo.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api/api_utils.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      180 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/api.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/doc_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.893482 sigmaepsilon.mesh-0.0.2/docs/source/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   167698 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/compound1.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   273863 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/compound2.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   112067 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/compound3.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   613748 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/cube.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   420021 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/cylinder.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   353852 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/disc.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   186760 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/grids2d.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   250977 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/grids3d.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   610460 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/import_file.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   325635 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/import_gmsh.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   319837 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/import_pyvista.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1260616 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/joint_cube.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   110806 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/lighting.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   259081 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples/trigridQ4.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/examples_gallery.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/logo.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.897482 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   949800 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/data.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   757783 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/grids.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   162584 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/io.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8001 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_analysis.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   135639 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_composition.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25963 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_structure.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   812456 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/plotting.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14480 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/points_and_pointclouds.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5153 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/shape_function_generation.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   383025 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/trafo_geom.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/notebooks/trafo_topo.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)      979 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/references.bib
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/refs.bib
--rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/docs/source/user_guide.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/logo.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/requirements-dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/requirements-devops.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/requirements-test.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.877482 sigmaepsilon.mesh-0.0.2/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.877482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.901482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/abcdata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/akwrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3327 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36505 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cell.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14433 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/celldata.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.901482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      704 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4034 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/h27.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/h8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1502 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/l2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1341 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/l3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/q4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1989 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/q9.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1532 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/t3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2082 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/t6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2089 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/tet10.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1401 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/tet4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/w18.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1663 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/w6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3796 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/downloads.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2196 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/extrude.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21752 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/grid.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/helpers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.901482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/inp2stl.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1481 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/line.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/linedata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/mesh1d.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8279 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/pointdata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    83946 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polydata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polygon.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polyhedron.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1040 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/pop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13756 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/recipes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14606 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/section.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.905482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7879 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/frame.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2736 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19474 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/pointcloud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tetmesh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1947 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tetrahedralize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2350 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4895 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/topoarray.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/triang.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6450 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/trimesh.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.905482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.905482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3252 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/gauss.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30232 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/h27.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7165 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/h8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1622 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/l2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/l3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2398 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/q4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4612 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/q9.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/t3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2630 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/t6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/tet10.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2500 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/tet4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4507 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1372 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/w18.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      994 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/w6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      706 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/colors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4734 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/knn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/locate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11071 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/space.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4568 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/tet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5482 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topodata.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29528 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20845 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/tr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16702 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/tri.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28958 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/voxelize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3208 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/vtkcelltypes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1886 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/vtkutils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.897482 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8593 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5400 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-12 18:56:36.000000 sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:56:36.909482 sigmaepsilon.mesh-0.0.2/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2063 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_cells.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_colors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1709 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_compound.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4456 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_geom.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1044 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_hex.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3350 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6097 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_linalg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_mesh_anal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2932 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_meshing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_pointcloud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2071 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_recipes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1548 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_tet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4082 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_topo_tr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2384 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tests/test_tri.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-07-12 18:55:56.000000 sigmaepsilon.mesh-0.0.2/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.079240 sigmaepsilon.mesh-0.0.3/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.027239 sigmaepsilon.mesh-0.0.3/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6009 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1903 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9081 2023-08-06 17:04:15.079240 sigmaepsilon.mesh-0.0.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6779 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.027239 sigmaepsilon.mesh-0.0.3/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      322 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.031239 sigmaepsilon.mesh-0.0.3/docs/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/README_link.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.035240 sigmaepsilon.mesh-0.0.3/docs/source/_static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/logo.PNG
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57097 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot1.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   131843 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot2.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   179580 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot3.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61611 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot4.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    91565 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot4a.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    89629 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot5.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    88428 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot6.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   181162 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot7.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    50423 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_1.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47062 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_2.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   132201 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_3.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106791 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_4.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   132473 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_5.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.035240 sigmaepsilon.mesh-0.0.3/docs/source/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_cells.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_db.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_recipes.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_space.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_topo.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_utils.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      180 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/doc_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.047240 sigmaepsilon.mesh-0.0.3/docs/source/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   167698 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/compound1.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   273863 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/compound2.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   112067 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/compound3.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   613748 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/cube.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   420021 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/cylinder.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   353852 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/disc.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   186760 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/grids2d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   250977 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/grids3d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   610460 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/import_file.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   325635 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/import_gmsh.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   319837 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/import_pyvista.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1260616 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/joint_cube.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   110806 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/lighting.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   253615 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/shape_functions_1d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   259081 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/trigridQ4.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples_gallery.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/logo.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.051240 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   949800 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/data.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   757783 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/grids.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   162584 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/io.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8001 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_analysis.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   135639 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_composition.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25963 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_structure.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   812456 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/plotting.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14480 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/points_and_pointclouds.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11679 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/shape_function_generation.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   383025 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/trafo_geom.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/trafo_topo.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      979 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/references.bib
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/refs.bib
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/user_guide.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/logo.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/requirements-dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/requirements-test.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-06 17:04:15.079240 sigmaepsilon.mesh-0.0.3/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.023239 sigmaepsilon.mesh-0.0.3/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.023239 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.063240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      985 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/abcdata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/akwrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3327 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43719 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cell.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14433 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/celldata.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.063240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      704 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4088 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/h27.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/h8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/l2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1343 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/l3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/q4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2001 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/q9.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1532 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/t3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2086 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/t6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2117 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/tet10.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1362 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/tet4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2458 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/w18.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1663 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/w6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3796 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/downloads.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2196 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/extrude.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21752 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/grid.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/helpers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.067240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/inp2stl.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/line.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/linedata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/mesh1d.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8279 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/pointdata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    83934 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polydata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polygon.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2617 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polyhedron.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1040 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/pop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13752 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/recipes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14608 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/section.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.067240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7879 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/frame.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2736 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19474 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/pointcloud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tetmesh.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1947 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tetrahedralize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2350 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4895 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/topoarray.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/triang.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6450 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/trimesh.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.067240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.071240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3252 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/gauss.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32014 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/h27.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7165 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/h8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/l2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/l3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2398 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/q4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4756 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/q9.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/t3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2646 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/t6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/tet10.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2506 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/tet4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4507 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1396 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/w18.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      994 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/w6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      706 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/colors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4734 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/knn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/locate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11071 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/space.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4568 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/tet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5482 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topodata.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.075240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29528 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20845 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/tr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16702 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/tri.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30106 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/voxelize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3206 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/vtkcelltypes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1886 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/vtkutils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.055240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9081 2023-08-06 17:04:14.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5490 2023-08-06 17:04:15.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-06 17:04:14.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-08-06 17:04:14.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-08-06 17:04:14.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.075240 sigmaepsilon.mesh-0.0.3/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.079240 sigmaepsilon.mesh-0.0.3/tests/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2016 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/test_cells.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3696 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/test_hex.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1261 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/test_lines.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2014 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/test_tet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_colors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1709 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_compound.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4456 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_geom.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3350 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6097 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_linalg.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_mesh_anal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_meshing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1352 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_pointcloud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2100 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_recipes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4082 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_topo_tr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2392 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_tri.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tox.ini
```

### Comparing `sigmaepsilon.mesh-0.0.2/.circleci/config.yml` & `sigmaepsilon.mesh-0.0.3/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/.gitignore` & `sigmaepsilon.mesh-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/.readthedocs.yaml` & `sigmaepsilon.mesh-0.0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/LICENSE` & `sigmaepsilon.mesh-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/PKG-INFO` & `sigmaepsilon.mesh-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon.mesh
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package to build, manipulate and analyze polygonal meshes.
 Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 License: MIT License
         
         Copyright (c) 2021 SigmaEpsilon
         
@@ -80,28 +80,48 @@
 ## Projects using sigmaepsilon.mesh
 
 - [SigmaEpsilon](https://github.com/dewloosh/SigmaEpsilon) - A Python library for computational solid mechanics.
 - [PyAxisVM](https://github.com/AxisVM/pyaxisvm) - The official Python package of [AxisVM](https://axisvm.eu/), a popular structural analysis and design software.
 
 ## Documentation
 
-The [documentation](https://sigmaepsilon.mesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set examples, and the API Reference.
+The [documentation](https://sigmaepsilonmesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set examples, and the API Reference.
 
 ## Installation
 
 sigmaepsilon.mesh can be installed from PyPI using `pip` on Python >= 3.7:
 
 ```console
 >>> pip install sigmaepsilon.mesh
 ```
 
-## Testing
+or chechkout with the following command using GitHub CLI
 
 ```console
->>> python -m unittest
+gh repo clone sigma-epsilon/sigmaepsilon.mesh
+```
+
+and install from source by typing
+
+```console
+>>> pip install .
+```
+
+If you want to run the tests, you can install the package along with the necessary optional dependencies like this
+
+```console
+>>> pip install ".[test]"
+```
+
+### Development mode
+
+If you are a developer and want to install the library in development mode, the suggested way is by using this command:
+
+```console
+>>> pip install "-e .[test, dev]"
 ```
 
 ## How to contribute?
 
 Contributions are currently expected in any the following ways:
 
 - finding bugs
```

### Comparing `sigmaepsilon.mesh-0.0.2/README.md` & `sigmaepsilon.mesh-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,28 +34,48 @@
 ## Projects using sigmaepsilon.mesh
 
 - [SigmaEpsilon](https://github.com/dewloosh/SigmaEpsilon) - A Python library for computational solid mechanics.
 - [PyAxisVM](https://github.com/AxisVM/pyaxisvm) - The official Python package of [AxisVM](https://axisvm.eu/), a popular structural analysis and design software.
 
 ## Documentation
 
-The [documentation](https://sigmaepsilon.mesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set examples, and the API Reference.
+The [documentation](https://sigmaepsilonmesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set examples, and the API Reference.
 
 ## Installation
 
 sigmaepsilon.mesh can be installed from PyPI using `pip` on Python >= 3.7:
 
 ```console
 >>> pip install sigmaepsilon.mesh
 ```
 
-## Testing
+or chechkout with the following command using GitHub CLI
 
 ```console
->>> python -m unittest
+gh repo clone sigma-epsilon/sigmaepsilon.mesh
+```
+
+and install from source by typing
+
+```console
+>>> pip install .
+```
+
+If you want to run the tests, you can install the package along with the necessary optional dependencies like this
+
+```console
+>>> pip install ".[test]"
+```
+
+### Development mode
+
+If you are a developer and want to install the library in development mode, the suggested way is by using this command:
+
+```console
+>>> pip install "-e .[test, dev]"
 ```
 
 ## How to contribute?
 
 Contributions are currently expected in any the following ways:
 
 - finding bugs
```

### Comparing `sigmaepsilon.mesh-0.0.2/docs/Makefile` & `sigmaepsilon.mesh-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/make.bat` & `sigmaepsilon.mesh-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/logo.PNG` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/logo.PNG`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot1.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot1.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot2.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot2.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot3.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot3.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot4.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot4.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot4a.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot4a.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot5.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot5.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot6.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot6.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/plot7.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot7.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_1.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_1.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_2.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_2.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_3.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_3.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_4.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_4.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/_static/readme_5.png` & `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_5.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/api/api_cells.rst` & `sigmaepsilon.mesh-0.0.3/docs/source/api/api_cells.rst`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/api/api_db.rst` & `sigmaepsilon.mesh-0.0.3/docs/source/api/api_db.rst`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/conf.py` & `sigmaepsilon.mesh-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/doc_utils.py` & `sigmaepsilon.mesh-0.0.3/docs/source/doc_utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/compound1.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/compound1.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/compound2.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/compound2.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/compound3.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/compound3.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/cube.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/cube.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/cylinder.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/cylinder.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/disc.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/disc.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/grids2d.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/grids2d.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/grids3d.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/grids3d.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/import_file.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/import_file.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/import_gmsh.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/import_gmsh.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/import_pyvista.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/import_pyvista.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/joint_cube.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/joint_cube.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/lighting.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/lighting.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/examples/trigridQ4.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/examples/trigridQ4.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/logo.png` & `sigmaepsilon.mesh-0.0.3/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/data.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/data.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/grids.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/grids.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/io.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/io.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_analysis.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_composition.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_composition.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/mesh_structure.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_structure.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/plotting.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/points_and_pointclouds.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/points_and_pointclouds.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/trafo_geom.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/trafo_geom.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/notebooks/trafo_topo.ipynb` & `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/trafo_topo.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/docs/source/references.bib` & `sigmaepsilon.mesh-0.0.3/docs/source/references.bib`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/logo.png` & `sigmaepsilon.mesh-0.0.3/logo.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/pyproject.toml` & `sigmaepsilon.mesh-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools-scm",
     "wheel>=0.38.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sigmaepsilon.mesh"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Python package to build, manipulate and analyze polygonal meshes."
 classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/__init__.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import importlib.metadata
+
 from .space import PointCloud
 from .space import CartesianFrame
 from .polydata import PolyData
 from .linedata import LineData
 from .linedata import LineData as PolyData1d
 from .pointdata import PointData
 from .utils import k_nearest_neighbours as KNN
 from .topoarray import TopologyArray
 from .trimesh import TriMesh
 from .tetmesh import TetMesh
 from .triang import triangulate
 from .grid import grid, Grid
 from .tetrahedralize import tetrahedralize
 from .config import load_pyproject_config
-import importlib.metadata
+
 
 __all__ = [
     "PointCloud",
     "CartesianFrame",
     "PolyData",
     "LineData",
     "PolyData1d",
@@ -29,10 +31,10 @@
     "grid",
     "Grid",
     "tetrahedralize",
 ]
 
 # _config = load_pyproject_config()
 
-__pkg_name__ = "sigmaepsilon.mesh"  # for Sphinx
+__pkg_name__ = "sigmaepsilon.mesh"
 __version__ = importlib.metadata.version(__pkg_name__)
 __description__ = "A Python package to build, manipulate and analyze polygonal meshes."
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/abcdata.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/abcdata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/akwrap.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/akwrap.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/base.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/base.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cell.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cell.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 from sigmaepsilon.math.utils import to_range_1d
 from sigmaepsilon.math.linalg import ReferenceFrame as FrameLike
 
 from sigmaepsilon.mesh.space import PointCloud, CartesianFrame
 from .celldata import CellData
 from .utils.utils import (
     jacobian_matrix_bulk,
+    jacobian_matrix_bulk_1d,
+    jacobian_det_bulk_1d,
     points_of_cells,
     pcoords_to_coords,
     pcoords_to_coords_1d,
     cells_coords,
     lengths_of_lines,
+    global_shape_function_derivatives,
 )
 from .utils.cells.utils import (
     _loc_to_glob_bulk_,
     _find_first_hits_,
     _find_first_hits_knn_,
     _ntet_to_loc_bulk_,
 )
@@ -78,26 +81,37 @@
         Ought to return local coordinates of the master element.
 
         Returns
         -------
         numpy.ndarray
         """
         raise NotImplementedError
+    
+    @classmethod
+    def master_coordinates(cls) -> ndarray:
+        """
+        Returns the coordinates of the master element.
+
+        Returns
+        -------
+        numpy.ndarray
+        """
+        return cls.lcoords()
 
     @classmethod
     def lcenter(cls) -> ndarray:
         """
         Ought to return the local coordinates of the center of the
         master element.
 
         Returns
         -------
         numpy.ndarray
         """
-        return cell_center(cls.lcoords())
+        return cell_center(cls.master_coordinates())
 
     @classmethod
     def polybase(cls) -> Tuple[List]:
         """
         Ought to retrun the polynomial base of the master element.
 
         Returns
@@ -122,14 +136,31 @@
         ----------
         return_symbolic: bool, Optional
             If True, the function returns symbolic expressions of shape functions
             and their derivatives. Default is True.
         update: bool, Optional
             If True, class methods are updated with the generated versions.
             Default is True.
+        
+        Notes
+        -----
+        Some cells are equipped with functions to evaluate shape functions a-priori,
+        other classes rely on symbolic generation of these functions. In the latter case,
+        this function is automatically invoked runtime, there is no need to manually
+        trigger it.
+        
+        Example
+        -------
+        >>> from sigmaepsilon.mesh.cells import H8
+        >>> shp, dshp, shpf, shpmf, dshpf = H8.generate_class_functions()
+        
+        Here `shp` and `dshp` are simbolic matrices for shape functions and
+        their first derivatives, `shpf`, `shpmf` and `dshpf` are functions for
+        fast evaluation of shape function values, the shape function matrix and
+        shape function derivatives, respectively.
         """
         nN = cls.NNODE
         nD = cls.NDIM
         nDOF = getattr(cls, "NDOFN", 3)
         locvars, monoms = cls.polybase()
         monoms.pop(0)
         lcoords = cls.lcoords()
@@ -152,36 +183,39 @@
         _dshpf = lambdify([locvars], dshp, "numpy")
 
         def shpf(p: ndarray) -> ndarray:
             """
             Evaluates the shape functions at multiple points in the
             master domain.
             """
+            p = atleast2d(p, back=True)
             r = np.stack([_shpf(p[i])[0] for i in range(len(p))])
             return ascont(r)
 
         def shpmf(p: ndarray, ndof: int = nDOF) -> ndarray:
             """
             Evaluates the shape function matrix at multiple points
             in the master domain.
             """
+            p = atleast2d(p, back=True)
             nP = p.shape[0]
             eye = np.eye(ndof, dtype=float)
             shp = shpf(p)
             res = np.zeros((nP, ndof, nN * ndof), dtype=float)
             for iP in range(nP):
                 for i in range(nN):
                     res[iP, :, i * ndof : (i + 1) * ndof] = eye * shp[iP, i]
             return ascont(res)
 
         def dshpf(p: ndarray) -> ndarray:
             """
             Evaluates the shape function derivatives at multiple points
             in the master domain.
             """
+            p = atleast2d(p, back=True)
             r = np.stack([_dshpf(p[i]) for i in range(len(p))])
             return ascont(r)
 
         if update:
             cls.shpfnc = shpf
             cls.shpmfnc = shpmf
             cls.dshpfnc = dshpf
@@ -214,15 +248,15 @@
         if cls.NDIM == 3:
             if len(pcoords.shape) == 1:
                 pcoords = atleast2d(pcoords, front=True)
                 return cls.shpfnc(pcoords).astype(float)
         return cls.shpfnc(pcoords).astype(float)
 
     @classmethod
-    def shape_function_matrix(cls, pcoords: ndarray, N: int = None) -> ndarray:
+    def shape_function_matrix(cls, pcoords: ndarray, *, N: int = None) -> ndarray:
         """
         Evaluates the shape function matrix at the specified locations.
 
         Parameters
         ----------
         pcoords: numpy.ndarray
             Locations of the evaluation points.
@@ -249,122 +283,162 @@
                     return cls.shpmfnc(pcoords).astype(float)
         if nDOFN:
             return cls.shpmfnc(pcoords, nDOFN).astype(float)
         else:
             return cls.shpmfnc(pcoords).astype(float)
 
     @classmethod
-    def shape_function_derivatives(cls, pcoords: ndarray) -> ndarray:
+    def shape_function_derivatives(
+        cls, pcoords: Iterable[float], *, jac: ndarray = None, dshp: ndarray = None
+    ) -> ndarray:
         """
-        Evaluates shape function derivatives wrt. the master element.
+        Evaluates shape function derivatives wrt. the master element or the local
+        coordinate frames of some cells. To control the behaviour, either 'jac' or 'wrt'
+        can be provided.
 
         Parameters
         ----------
-        pcoords: numpy.ndarray
+        pcoords: Iterable[float]
             Locations of the evaluation points.
+        jac: Iterable, Optional
+            The jacobian matrix as a float array of shape (nE, nP, nD, nD), evaluated for
+            an nP number of points and nP number cells and nD number of spatial dimensions.
+            Default is None.
+        dshp: numpy.ndarray, Optional
+            Shape function derivatives wrt. the master element. Only relevant if 'jac' is
+            provided. The purpose of this argument is to avoid repeated evaluation in situations
+            where 'dshp' is required on its own and is already at hand when calling this function.
+            Default is None, in which case it is calculated automatically.
+            
+        Notes
+        -----
+        Only first derivatives are calculated.
 
         Returns
         -------
         numpy.ndarray
             An array of shape (nP, nNE, nD), where nP, nNE and nD are
             the number of evaluation points, nodes and spatial dimensions.
         """
-        pcoords = np.array(pcoords)
-        if cls.dshpfnc is None:
-            cls.generate_class_functions(update=True)
-        if cls.NDIM == 3:
-            if len(pcoords.shape) == 1:
-                pcoords = atleast2d(pcoords, front=True)
-                return cls.dshpfnc(pcoords).astype(float)
-        return cls.dshpfnc(pcoords).astype(float)
-
-    def flip(self) -> "PolyCell":
-        """
-        Reverse the order of nodes of the topology.
-        """
-        topo = self.topology().to_numpy()
-        self.nodes = np.flip(topo, axis=1)
-        return self
-
-    def measures(self, *args, **kwargs) -> ndarray:
-        """Ought to return measures for each cell in the database."""
-        raise NotImplementedError
-
-    def measure(self, *args, **kwargs) -> float:
-        """Ought to return the net measure for the cells in the
-        database as a group."""
-        return np.sum(self.measures(*args, **kwargs))
-
-    def area(self, *args, **kwargs) -> float:
-        """Returns the total area of the cells in the database. Only for 2d entities."""
-        return np.sum(self.areas(*args, **kwargs))
-
-    def areas(self, *args, **kwargs) -> ndarray:
-        """Ought to return the areas of the individuall cells in the database."""
-        raise NotImplementedError
-
-    def volume(self, *args, **kwargs) -> float:
-        """Returns the volume of the cells in the database."""
-        return np.sum(self.volumes(*args, **kwargs))
-
-    def volumes(self, *args, **kwargs) -> ndarray:
-        """Ought to return the volumes of the individual cells in the database."""
-        raise NotImplementedError
-
-    def extract_surface(self, detach: bool = False):
-        """Extracts the surface of the mesh. Only for 3d meshes."""
-        raise NotImplementedError
+        if jac is None:
+            pcoords = np.array(pcoords) if pcoords is not None else cls.lcoords()
+            if cls.dshpfnc is None:
+                cls.generate_class_functions(update=True)
+            if cls.NDIM == 3:
+                if len(pcoords.shape) == 1:
+                    pcoords = atleast2d(pcoords, front=True)
+                    return cls.dshpfnc(pcoords).astype(float)
+            return cls.dshpfnc(pcoords).astype(float)
+        else:
+            pcoords = np.array(pcoords) if pcoords is not None else cls.lcoords()
+            if dshp is None:
+                dshp = cls.shape_function_derivatives(pcoords)
+            return global_shape_function_derivatives(dshp, jac)
 
-    def jacobian_matrix(self, *, dshp: ndarray = None, **__) -> ndarray:
+    def jacobian_matrix(
+        self, *, pcoords: Iterable[float] = None, dshp: ndarray = None, **__
+    ) -> ndarray:
         """
-        Returns the jacobian matrices.
+        Returns the jacobian matrices of the cells in the block. The evaluation
+        of the matrix is governed by the inputs in the following way:
+        - if `dshp` is provided, it must be a matrix of shape function derivatives
+          evaluated at the desired locations
+        - the desired locations are specified through `pcoords`
 
         Parameters
         ----------
-        dshp: numpy.ndarray
+        pcoords: Iterable[float], Optional
+            Locations of the evaluation points.
+        dshp: numpy.ndarray, Optional
             3d array of shape function derivatives for the master cell,
             evaluated at some points. The array must have a shape of
-            (nG, nNE, nD), where nG, nNE and nD are he number of evaluation
+            (nG, nNE, nD), where nG, nNE and nD are the number of evaluation
             points, nodes per cell and spatial dimensions.
 
         Returns
         -------
         numpy.ndarray
-            A 4d array of shape (nE, nG, nD, nD), where nE, nG and nD
+            A 4d array of shape (nE, nP, nD, nD), where nE, nP and nD
             are the number of elements, evaluation points and spatial
             dimensions. The number of evaluation points in the output
-            is governed by the parameter 'dshp'.
+            is governed by the parameter 'dshp' or 'pcoords'.
         """
         ecoords = self.local_coordinates()
-        return jacobian_matrix_bulk(dshp, ecoords)
+        if dshp is None:
+            x = np.array(pcoords) if pcoords is not None else self.lcoords()
+            dshp = self.shape_function_derivatives(x)
+        if self.NDIM == 1:
+            return jacobian_matrix_bulk_1d(dshp, ecoords)
+        else:
+            return jacobian_matrix_bulk(dshp, ecoords)
 
     def jacobian(self, *, jac: ndarray = None, **kwargs) -> Union[float, ndarray]:
         """
         Returns the jacobian determinant for one or more cells.
 
         Parameters
         ----------
         jac: numpy.ndarray, Optional
             One or more Jacobian matrices. Default is None.
-        **kwargs : dict
+        **kwargs: dict
             Forwarded to :func:`jacobian_matrix` if the jacobian
             is not provided by the parameter 'jac'.
 
         Returns
         -------
         float or numpy.ndarray
             Value of the Jacobian for one or more cells.
 
         See Also
         --------
         :func:`jacobian_matrix`
         """
         if jac is None:
             jac = self.jacobian_matrix(**kwargs)
-        return np.linalg.det(jac)
+        if self.NDIM == 1:
+            return jacobian_det_bulk_1d(jac)
+        else:
+            return np.linalg.det(jac)
+
+    def flip(self) -> "PolyCell":
+        """
+        Reverse the order of nodes of the topology.
+        """
+        topo = self.topology().to_numpy()
+        self.nodes = np.flip(topo, axis=1)
+        return self
+
+    def measures(self, *args, **kwargs) -> ndarray:
+        """Ought to return measures for each cell in the database."""
+        raise NotImplementedError
+
+    def measure(self, *args, **kwargs) -> float:
+        """Ought to return the net measure for the cells in the
+        database as a group."""
+        return np.sum(self.measures(*args, **kwargs))
+
+    def area(self, *args, **kwargs) -> float:
+        """Returns the total area of the cells in the database. Only for 2d entities."""
+        return np.sum(self.areas(*args, **kwargs))
+
+    def areas(self, *args, **kwargs) -> ndarray:
+        """Ought to return the areas of the individuall cells in the database."""
+        raise NotImplementedError
+
+    def volume(self, *args, **kwargs) -> float:
+        """Returns the volume of the cells in the database."""
+        return np.sum(self.volumes(*args, **kwargs))
+
+    def volumes(self, *args, **kwargs) -> ndarray:
+        """Ought to return the volumes of the individual cells in the database."""
+        raise NotImplementedError
+
+    def extract_surface(self, detach: bool = False):
+        """Extracts the surface of the mesh. Only for 3d meshes."""
+        raise NotImplementedError
 
     def source_points(self) -> PointCloud:
         """
         Returns the hosting pointcloud.
         """
         return self.container.source().points()
 
@@ -385,15 +459,15 @@
         return self.container.source().frame
 
     def points_of_cells(
         self,
         *,
         points: Union[float, Iterable] = None,
         cells: Union[int, Iterable] = None,
-        target: Union[str, CartesianFrame] = "global"
+        target: Union[str, CartesianFrame] = "global",
     ) -> ndarray:
         """
         Returns the points of the cells as a NumPy array.
         """
         if cells is not None:
             cells = atleast1d(cells)
             conds = np.isin(cells, self.id)
@@ -659,16 +733,15 @@
 
 class PolyCell1d(PolyCell):
     """Base class for 1d cells"""
 
     NDIM = 1
 
     def lenth(self) -> float:
-        """Returns the total length of the cells in
-        the database."""
+        """Returns the total length of the cells in the block."""
         return np.sum(self.lengths())
 
     def lengths(self) -> ndarray:
         """
         Returns the lengths as a NumPy array.
         """
         coords = self.container.source().coords()
@@ -702,15 +775,15 @@
         self,
         *,
         points: Union[float, Iterable] = None,
         cells: Union[int, Iterable] = None,
         flatten: bool = False,
         target: Union[str, CartesianFrame] = "global",
         rng: Iterable = None,
-        **kwargs
+        **kwargs,
     ) -> ndarray:
         if isinstance(target, str):
             assert target.lower() in ["global", "g"]
         else:
             raise NotImplementedError
         topo = kwargs.get("topo", self.topology().to_numpy())
         coords = kwargs.get("coords", None)
@@ -748,14 +821,111 @@
         if not flatten:
             nE = ecoords.shape[0]
             nP = points.shape[0]
             res = res.reshape(nE, nP, res.shape[-1])  # (nE, nP, nD)
 
         return res
 
+    @classmethod
+    def shape_function_values(
+        cls, pcoords: ndarray, *, rng: Iterable = None
+    ) -> ndarray:
+        """
+        Evaluates the shape functions at the specified locations.
+
+        Parameters
+        ----------
+        pcoords: float or Iterable[float]
+            Locations of the evaluation points.
+        rng: Iterable, Optional
+            The range in which the locations ought to be understood,
+            typically [0, 1] or [-1, 1]. Default is [0, 1].
+
+        Returns
+        -------
+        numpy.ndarray
+            An array of shape (nP, nNE) where nP and nNE are the number of
+            evaluation points and shape functions. If there is only one
+            evaluation point, the returned array is one dimensional.
+        """
+        rng = np.array([-1, 1]) if rng is None else np.array(rng)
+        pcoords = atleast1d(np.array(pcoords))
+        pcoords = to_range_1d(pcoords, source=rng, target=[-1, 1])
+        return super().shape_function_values(pcoords)
+
+    @classmethod
+    def shape_function_matrix(
+        cls, pcoords: ndarray, *, rng: Iterable = None, N: int = None
+    ) -> ndarray:
+        """
+        Evaluates the shape function matrix at the specified locations.
+
+        Parameters
+        ----------
+        pcoords: float or Iterable[float]
+            Locations of the evaluation points.
+        rng: Iterable, Optional
+            The range in which the locations ought to be understood,
+            typically [0, 1] or [-1, 1]. Default is [0, 1].
+        N: int, Optional
+            Number of unknowns per node.
+
+        Returns
+        -------
+        numpy.ndarray
+            An array of shape (nP, nDOF, nDOF * nNE) where nP, nDOF and nNE
+            are the number of evaluation points, degrees of freedom per node
+            and nodes per cell.
+        """
+        rng = np.array([-1, 1]) if rng is None else np.array(rng)
+        pcoords = atleast1d(np.array(pcoords))
+        pcoords = to_range_1d(pcoords, source=rng, target=[-1, 1])
+        return super().shape_function_matrix(pcoords, N=N)
+
+    @classmethod
+    def shape_function_derivatives(
+        cls,
+        pcoords: Union[float, Iterable[float]] = None,
+        *,
+        rng: Iterable = None,
+        jac: ndarray = None,
+        dshp: ndarray = None
+    ) -> ndarray:
+        """
+        Evaluates shape function derivatives wrt. the master element or the local
+        coordinate frames of some cells. To control the behaviour, either 'jac' or 'wrt'
+        can be provided.
+
+        Parameters
+        ----------
+        pcoords: float or Iterable[float], Optional
+            Locations of the evaluation points.
+        rng: Iterable, Optional
+            The range in which the locations ought to be understood,
+            typically [0, 1] or [-1, 1]. Default is [0, 1].
+        jac: Iterable, Optional
+            The jacobian matrix as a float array of shape (nE, nP, nD=1, nD=1), evaluated for
+            each point in each cell. Default is None.
+        dshp: numpy.ndarray, Optional
+            Shape function derivatives wrt. the master element. Only relevant if 'jac' is
+            provided. The purpose of this argument is to avoid repeated evaluation in situations
+            where 'dshp' is required on its own and is already at hand when calling this function.
+            Default is None, in which case it is calculated automatically.
+
+        Returns
+        -------
+        numpy.ndarray
+            An array of shape (nP, nNE, nD=1), where nP, nNE and nD are
+            the number of evaluation points, nodes and spatial dimensions.
+        """
+        rng = np.array([-1, 1], dtype=float) if rng is None else np.array(rng)
+        pcoords = atleast1d(np.array(pcoords, dtype=float))
+        pcoords = to_range_1d(pcoords, source=rng, target=[-1, 1])
+        return super().shape_function_derivatives(pcoords, jac=jac, dshp=dshp)
+
 
 class PolyCell2d(PolyCell):
     """Base class for 2d cells"""
 
     NDIM = 2
 
     def area(self) -> float:
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/celldata.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/celldata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/__init__.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/h27.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/h27.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,33 +77,33 @@
             r,
             s,
             t,
             s * t,
             r * t,
             r * s,
             r * s * t,
-            r**2,
-            s**2,
-            t**2,
-            r**2 * s,
-            r * s**2,
-            r * t**2,
-            r**2 * t,
-            s**2 * t,
-            s * t**2,
-            r**2 * s * t,
-            r * s**2 * t,
-            r * s * t**2,
-            r**2 * s**2,
-            s**2 * t**2,
-            r**2 * t**2,
-            r**2 * s**2 * t**2,
-            r**2 * s**2 * t,
-            r**2 * s * t**2,
-            r * s**2 * t**2,
+            r ** 2,
+            s ** 2,
+            t ** 2,
+            r ** 2 * s,
+            r * s ** 2,
+            r * t ** 2,
+            r ** 2 * t,
+            s ** 2 * t,
+            s * t ** 2,
+            r ** 2 * s * t,
+            r * s ** 2 * t,
+            r * s * t ** 2,
+            r ** 2 * s ** 2,
+            s ** 2 * t ** 2,
+            r ** 2 * t ** 2,
+            r ** 2 * s ** 2 * t ** 2,
+            r ** 2 * s ** 2 * t,
+            r ** 2 * s * t ** 2,
+            r * s ** 2 * t ** 2,
         ]
         return locvars, monoms
 
     @classmethod
     def lcoords(cls) -> ndarray:
         """
         Returns local coordinates of the cell.
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/h8.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/h8.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/l2.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/l2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 from typing import Tuple, List
+
 import numpy as np
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
 from ..line import Line
 from ..utils.cells.l2 import (
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/l3.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/l3.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         -------
         list
             A list of SymPy symbols.
         list
             A list of monomials.
         """
         locvars = r = symbols("r", real=True)
-        monoms = [1, r, r**2]
+        monoms = [1, r, r ** 2]
         return [locvars], monoms
 
     @classmethod
     def lcoords(cls) -> ndarray:
         """
         Returns local coordinates of the cell.
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/q4.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/q4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/q9.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/q9.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,19 +45,19 @@
         """
         locvars = r, s = symbols("r, s", real=True)
         monoms = [
             1,
             r,
             s,
             r * s,
-            r**2,
-            s**2,
-            r * s**2,
-            s * r**2,
-            s**2 * r**2,
+            r ** 2,
+            s ** 2,
+            r * s ** 2,
+            s * r ** 2,
+            s ** 2 * r ** 2,
         ]
         return locvars, monoms
 
     @classmethod
     def lcoords(cls):
         """
         Returns local coordinates of the cell.
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/t3.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/t3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/t6.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/t6.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         -------
         list
             A list of SymPy symbols.
         list
             A list of monomials.
         """
         locvars = r, s = symbols("r s", real=True)
-        monoms = [1, r, s, r**2, s**2, r * s]
+        monoms = [1, r, s, r ** 2, s ** 2, r * s]
         return locvars, monoms
 
     @classmethod
     def lcoords(cls) -> ndarray:
         """
         Returns local coordinates of the cell.
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/tet10.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/tet10.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,19 @@
         -------
         list
             A list of SymPy symbols.
         list
             A list of monomials.
         """
         locvars = r, s, t = symbols("r s t", real=True)
-        monoms = [1, r, s, t, r * s, r * t, s * t, r**2, s**2, t**2]
+        monoms = [1, r, s, t, r * s, r * t, s * t, r ** 2, s ** 2, t ** 2]
         return locvars, monoms
 
     @classmethod
-    def lcoords(cls):
+    def lcoords(cls) -> ndarray:
         return np.array(
             [
                 [0.0, 0.0, 0.0],
                 [1.0, 0.0, 0.0],
                 [0.0, 1.0, 0.0],
                 [0.0, 0.0, 1.0],
                 [0.5, 0.0, 0.0],
@@ -57,15 +57,15 @@
                 [0.0, 0.0, 0.5],
                 [0.5, 0.0, 0.5],
                 [0.0, 0.5, 0.5],
             ]
         )
 
     @classmethod
-    def lcenter(cls):
+    def lcenter(cls) -> ndarray:
         return np.array([[1 / 3, 1 / 3, 1 / 3]])
 
     def volumes(self, coords: ndarray = None, topo: ndarray = None) -> ndarray:
         if coords is None:
             if self.pointdata is not None:
                 coords = self.pointdata.x
             else:
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/tet4.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/tet4.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         -------
         list
             A list of SymPy symbols.
         list
             A list of monomials.
         """
         locvars = r, s, t = symbols("r s t", real=True)
-        monoms = [1, r, s, t, r * s, r * t, s * t, r**2, s**2, t**2]
+        monoms = [1, r, s, t]
         return locvars, monoms
 
     @classmethod
     def lcoords(cls) -> ndarray:
         return np.array(
             [[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
         )
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/w18.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/w18.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,29 +38,29 @@
             A list of monomials.
         """
         locvars = r, s, t = symbols("r s t", real=True)
         monoms = [
             1,
             r,
             s,
-            r**2,
-            s**2,
+            r ** 2,
+            s ** 2,
             r * s,
             t,
             t * r,
             t * s,
-            t * r**2,
-            t * s**2,
+            t * r ** 2,
+            t * s ** 2,
             t * r * s,
-            t**2,
-            t**2 * r,
-            t**2 * s,
-            t**2 * r**2,
-            t**2 * s**2,
-            t**2 * r * s,
+            t ** 2,
+            t ** 2 * r,
+            t ** 2 * s,
+            t ** 2 * r ** 2,
+            t ** 2 * s ** 2,
+            t ** 2 * r * s,
         ]
         return locvars, monoms
 
     @classmethod
     def lcoords(cls):
         return np.array(
             [
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/cells/w6.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/w6.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/config.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/config.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/downloads.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/downloads.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/extrude.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/extrude.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/grid.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/grid.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/inp2stl.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/inp2stl.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/io/io.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/io.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/linedata.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/linedata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/mesh1d.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/mesh1d.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/pointdata.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/pointdata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polydata.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polydata.py`

 * *Files 0% similar despite different names*

```diff
@@ -2217,15 +2217,15 @@
             if notebook:
                 show_params.update(jupyter_backend=jupyter_backend)
             else:
                 if return_img:
                     plotter.show(auto_close=False)
                     plotter.show(screenshot=True)
                     return plotter.last_image
-            
+
             return plotter.show(**show_params)
 
     def plot(
         self,
         *,
         notebook: bool = False,
         backend: str = "pyvista",
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polygon.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polygon.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/polyhedron.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polyhedron.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/pop.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/pop.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/recipes.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/recipes.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     frame = CartesianFrame(dim=3) if frame is None else frame
     return TriMesh(points=points, triangles=triangles, celltype=T3, frame=frame)
 
 
 def cylinder(
     shape,
     size: Union[tuple, float, int] = None,
-    *args,
+    *,
     regular: bool = True,
     voxelize: bool = False,
     celltype=None,
     frame: CartesianFrame = None,
     **kwargs,
 ) -> PolyData:
     """
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/section.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/section.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     -------
     :class:`sectionproperties.pre.geometry.Geometry`
         The geometry object provided with a finite element mesh.
     """
     area = geometry.calculate_area()
     mesh_sizes_max = []
     if isinstance(l_max, float):
-        mesh_sizes_max.append(l_max**2 * np.sqrt(3) / 4)
+        mesh_sizes_max.append(l_max ** 2 * np.sqrt(3) / 4)
     if isinstance(a_max, float):
         mesh_sizes_max.append(a_max)
     if isinstance(n_max, int):
         mesh_sizes_max.append(area / n_max)
 
     mesh_size_max = None
     if len(mesh_sizes_max) > 0:
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/frame.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/frame.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/point.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/point.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/space/pointcloud.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/pointcloud.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tetmesh.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tetmesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tetrahedralize.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tetrahedralize.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/tile.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tile.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/topoarray.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/topoarray.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/triang.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/triang.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/trimesh.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/trimesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/gauss.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/gauss.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/h8.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/h8.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/l2.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/l2.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,54 +7,47 @@
 
 @njit(nogil=True, cache=__cache)
 def monoms_L2(r: float) -> ndarray:
     return np.array([1, r], dtype=float)
 
 
 @njit(nogil=True, cache=__cache)
-def shp_L2(r):
+def shp_L2(r) -> ndarray:
     """
     Evaluates the shape functions at one location in the range [-1, 1].
     """
     return np.array([1 - r, 1 + r]) / 2
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def shp_L2_multi(pcoords: np.ndarray):
+def shp_L2_multi(pcoords: ndarray) -> ndarray:
     nP = pcoords.shape[0]
     res = np.zeros((nP, 2), dtype=pcoords.dtype)
     for iP in prange(nP):
         res[iP, :] = shp_L2(pcoords[iP])
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def shape_function_matrix_L2(pcoord: ndarray, ndof: int = 2) -> ndarray:
-    eye = np.eye(ndof, dtype=pcoord.dtype)
-    shp = shp_L2(pcoord)
-    res = np.zeros((ndof, ndof * 2), dtype=pcoord.dtype)
-    for i in prange(2):
-        res[:, i * ndof : (i + 1) * ndof] = eye * shp[i]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
 def shape_function_matrix_L2_multi(pcoords: ndarray, ndof: int = 2) -> ndarray:
     nP = pcoords.shape[0]
+    eye = np.eye(ndof, dtype=pcoords.dtype)
     res = np.zeros((nP, ndof, 2 * ndof), dtype=pcoords.dtype)
     for iP in prange(nP):
-        res[iP] = shape_function_matrix_L2(pcoords[iP], ndof)
+        shp = shp_L2(pcoords[iP])
+        for iN in prange(2):
+            res[iP, :, iN * ndof : (iN + 1) * ndof] = eye * shp[iN]
     return res
 
 
 @njit(nogil=True, cache=__cache)
-def dshp_L2(r):
+def dshp_L2(r) -> ndarray:
     return np.array([-1, 1]) / 2
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def dshp_L2_multi(pcoords: ndarray):
+def dshp_L2_multi(pcoords: ndarray) -> ndarray:
     nP = pcoords.shape[0]
-    res = np.zeros((nP, 2), dtype=pcoords.dtype)
+    res = np.zeros((nP, 2, 1), dtype=pcoords.dtype)
     for iP in prange(nP):
-        res[iP, :] = dshp_L2(pcoords[iP])
+        res[iP, :, 0] = dshp_L2(pcoords[iP])
     return res
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/q4.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/q4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/q9.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/q9.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,58 +11,58 @@
     r, s = x
     return np.array(
         [
             1,
             r,
             s,
             r * s,
-            r**2,
-            s**2,
-            r * s**2,
-            s * r**2,
-            s**2 * r**2,
+            r ** 2,
+            s ** 2,
+            r * s ** 2,
+            s * r ** 2,
+            s ** 2 * r ** 2,
         ],
         dtype=float,
     )
 
 
 @njit(nogil=True, cache=__cache)
 def shp_Q9(pcoord: np.ndarray):
     r, s = pcoord[:2]
     return np.array(
         [
             [
-                0.25 * r**2 * s**2
-                - 0.25 * r**2 * s
-                - 0.25 * r * s**2
+                0.25 * r ** 2 * s ** 2
+                - 0.25 * r ** 2 * s
+                - 0.25 * r * s ** 2
                 + 0.25 * r * s
             ],
             [
-                0.25 * r**2 * s**2
-                - 0.25 * r**2 * s
-                + 0.25 * r * s**2
+                0.25 * r ** 2 * s ** 2
+                - 0.25 * r ** 2 * s
+                + 0.25 * r * s ** 2
                 - 0.25 * r * s
             ],
             [
-                0.25 * r**2 * s**2
-                + 0.25 * r**2 * s
-                + 0.25 * r * s**2
+                0.25 * r ** 2 * s ** 2
+                + 0.25 * r ** 2 * s
+                + 0.25 * r * s ** 2
                 + 0.25 * r * s
             ],
             [
-                0.25 * r**2 * s**2
-                + 0.25 * r**2 * s
-                - 0.25 * r * s**2
+                0.25 * r ** 2 * s ** 2
+                + 0.25 * r ** 2 * s
+                - 0.25 * r * s ** 2
                 - 0.25 * r * s
             ],
-            [-0.5 * r**2 * s**2 + 0.5 * r**2 * s + 0.5 * s**2 - 0.5 * s],
-            [-0.5 * r**2 * s**2 + 0.5 * r**2 - 0.5 * r * s**2 + 0.5 * r],
-            [-0.5 * r**2 * s**2 - 0.5 * r**2 * s + 0.5 * s**2 + 0.5 * s],
-            [-0.5 * r**2 * s**2 + 0.5 * r**2 + 0.5 * r * s**2 - 0.5 * r],
-            [1.0 * r**2 * s**2 - 1.0 * r**2 - 1.0 * s**2 + 1.0],
+            [-0.5 * r ** 2 * s ** 2 + 0.5 * r ** 2 * s + 0.5 * s ** 2 - 0.5 * s],
+            [-0.5 * r ** 2 * s ** 2 + 0.5 * r ** 2 - 0.5 * r * s ** 2 + 0.5 * r],
+            [-0.5 * r ** 2 * s ** 2 - 0.5 * r ** 2 * s + 0.5 * s ** 2 + 0.5 * s],
+            [-0.5 * r ** 2 * s ** 2 + 0.5 * r ** 2 + 0.5 * r * s ** 2 - 0.5 * r],
+            [1.0 * r ** 2 * s ** 2 - 1.0 * r ** 2 - 1.0 * s ** 2 + 1.0],
         ],
         dtype=pcoord.dtype,
     )
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def shp_Q9_multi(pcoords: np.ndarray):
@@ -94,46 +94,46 @@
 
 @njit(nogil=True, cache=__cache)
 def dshp_Q9(pcoord: np.ndarray):
     r, s = pcoord[:2]
     return np.array(
         [
             [
-                0.5 * r * s**2 - 0.5 * r * s - 0.25 * s**2 + 0.25 * s,
-                0.5 * r**2 * s - 0.25 * r**2 - 0.5 * r * s + 0.25 * r,
+                0.5 * r * s ** 2 - 0.5 * r * s - 0.25 * s ** 2 + 0.25 * s,
+                0.5 * r ** 2 * s - 0.25 * r ** 2 - 0.5 * r * s + 0.25 * r,
             ],
             [
-                0.5 * r * s**2 - 0.5 * r * s + 0.25 * s**2 - 0.25 * s,
-                0.5 * r**2 * s - 0.25 * r**2 + 0.5 * r * s - 0.25 * r,
+                0.5 * r * s ** 2 - 0.5 * r * s + 0.25 * s ** 2 - 0.25 * s,
+                0.5 * r ** 2 * s - 0.25 * r ** 2 + 0.5 * r * s - 0.25 * r,
             ],
             [
-                0.5 * r * s**2 + 0.5 * r * s + 0.25 * s**2 + 0.25 * s,
-                0.5 * r**2 * s + 0.25 * r**2 + 0.5 * r * s + 0.25 * r,
+                0.5 * r * s ** 2 + 0.5 * r * s + 0.25 * s ** 2 + 0.25 * s,
+                0.5 * r ** 2 * s + 0.25 * r ** 2 + 0.5 * r * s + 0.25 * r,
             ],
             [
-                0.5 * r * s**2 + 0.5 * r * s - 0.25 * s**2 - 0.25 * s,
-                0.5 * r**2 * s + 0.25 * r**2 - 0.5 * r * s - 0.25 * r,
+                0.5 * r * s ** 2 + 0.5 * r * s - 0.25 * s ** 2 - 0.25 * s,
+                0.5 * r ** 2 * s + 0.25 * r ** 2 - 0.5 * r * s - 0.25 * r,
             ],
             [
-                -1.0 * r * s**2 + 1.0 * r * s,
-                -1.0 * r**2 * s + 0.5 * r**2 + 1.0 * s - 0.5,
+                -1.0 * r * s ** 2 + 1.0 * r * s,
+                -1.0 * r ** 2 * s + 0.5 * r ** 2 + 1.0 * s - 0.5,
             ],
             [
-                -1.0 * r * s**2 + 1.0 * r - 0.5 * s**2 + 0.5,
-                -1.0 * r**2 * s - 1.0 * r * s,
+                -1.0 * r * s ** 2 + 1.0 * r - 0.5 * s ** 2 + 0.5,
+                -1.0 * r ** 2 * s - 1.0 * r * s,
             ],
             [
-                -1.0 * r * s**2 - 1.0 * r * s,
-                -1.0 * r**2 * s - 0.5 * r**2 + 1.0 * s + 0.5,
+                -1.0 * r * s ** 2 - 1.0 * r * s,
+                -1.0 * r ** 2 * s - 0.5 * r ** 2 + 1.0 * s + 0.5,
             ],
             [
-                -1.0 * r * s**2 + 1.0 * r + 0.5 * s**2 - 0.5,
-                -1.0 * r**2 * s + 1.0 * r * s,
+                -1.0 * r * s ** 2 + 1.0 * r + 0.5 * s ** 2 - 0.5,
+                -1.0 * r ** 2 * s + 1.0 * r * s,
             ],
-            [2.0 * r * s**2 - 2.0 * r, 2.0 * r**2 * s - 2.0 * s],
+            [2.0 * r * s ** 2 - 2.0 * r, 2.0 * r ** 2 * s - 2.0 * s],
         ],
         dtype=pcoord.dtype,
     )
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def dshp_Q9_multi(pcoords: ndarray):
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/t3.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/t3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/t6.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/t6.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 __cache = True
 
 
 @njit(nogil=True, cache=__cache)
 def monoms_T6(x: ndarray) -> ndarray:
     r, s = x
-    return np.array([1, r, s, r**2, s**2, r * s], dtype=float)
+    return np.array([1, r, s, r ** 2, s ** 2, r * s], dtype=float)
 
 
 @njit(nogil=True, cache=__cache)
 def shp_T6(pcoord: ndarray):
     r, s = pcoord[0:2]
     return np.array(
         [
-            2.0 * r**2 + 4.0 * r * s - 3.0 * r + 2.0 * s**2 - 3.0 * s + 1.0,
-            2.0 * r**2 - 1.0 * r,
-            2.0 * s**2 - 1.0 * s,
-            -4.0 * r**2 - 4.0 * r * s + 4.0 * r,
+            2.0 * r ** 2 + 4.0 * r * s - 3.0 * r + 2.0 * s ** 2 - 3.0 * s + 1.0,
+            2.0 * r ** 2 - 1.0 * r,
+            2.0 * s ** 2 - 1.0 * s,
+            -4.0 * r ** 2 - 4.0 * r * s + 4.0 * r,
             4.0 * r * s,
-            -4.0 * r * s - 4.0 * s**2 + 4.0 * s,
+            -4.0 * r * s - 4.0 * s ** 2 + 4.0 * s,
         ],
         dtype=pcoord.dtype,
     )
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def shp_T6_multi(pcoords: ndarray):
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/tet10.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/tet10.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __cache = True
 
 
 @njit(nogil=True, cache=__cache)
 def monoms_TET10_single(x: ndarray) -> ndarray:
     r, s, t = x
     return np.array(
-        [1, r, s, t, r * s, r * t, s * t, r**2, s**2, t**2], dtype=x.dtype
+        [1, r, s, t, r * s, r * t, s * t, r ** 2, s ** 2, t ** 2], dtype=x.dtype
     )
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def monoms_TET10_multi(x: ndarray) -> ndarray:
     nP = x.shape[0]
     res = np.zeros((nP, 10), dtype=x.dtype)
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/tet4.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/tet4.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __cache = True
 
 
 @njit(nogil=True, cache=__cache)
 def monoms_TET4_single(x: ndarray) -> ndarray:
     r, s, t = x
     return np.array(
-        [1, r, s, t, r * s, r * t, s * t, r**2, s**2, t**2], dtype=x.dtype
+        [1, r, s, t, r * s, r * t, s * t, r ** 2, s ** 2, t ** 2], dtype=x.dtype
     )
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def monoms_TET4_multi(x: ndarray) -> ndarray:
     nP = x.shape[0]
     res = np.zeros((nP, 4), dtype=x.dtype)
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/utils.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/w18.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/w18.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 def monoms_W18_single(x: ndarray) -> ndarray:
     r, s, t = x
     return np.array(
         [
             1,
             r,
             s,
-            r**2,
-            s**2,
+            r ** 2,
+            s ** 2,
             r * s,
             t,
             t * r,
             t * s,
-            t * r**2,
-            t * s**2,
+            t * r ** 2,
+            t * s ** 2,
             t * r * s,
-            t**2,
-            t**2 * r,
-            t**2 * s,
-            t**2 * r**2,
-            t**2 * s**2,
-            t**2 * r * s,
+            t ** 2,
+            t ** 2 * r,
+            t ** 2 * s,
+            t ** 2 * r ** 2,
+            t ** 2 * s ** 2,
+            t ** 2 * r * s,
         ],
         dtype=x.dtype,
     )
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def monoms_W18_multi(x: ndarray) -> ndarray:
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/cells/w6.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/w6.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/colors.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/colors.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/knn.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/knn.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/locate.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/locate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/space.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/space.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/tet.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/tet.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topodata.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topodata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/topo.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/topo.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/topology/tr.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/tr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/tri.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/tri.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/utils/utils.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,15 +678,15 @@
     elif isinstance(data, ndarray):
         return explode_mesh_data_bulk(coords, topo, data)
     else:
         raise NotImplementedError
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
-def decompose(ecoords, topo, coords_out):
+def decompose(ecoords: ndarray, topo: ndarray, coords_out: ndarray) -> None:
     """
     Performes the inverse operation to coordinate explosion.
     Example usage at AxisVM domains. Works for all kinds of arrays.
     """
     for iE in prange(len(topo)):
         for jNE in prange(len(topo[iE])):
             coords_out[topo[iE][jNE]] = np.array(ecoords[iE][jNE])
@@ -995,7 +995,38 @@
 
 def is_ccw(points: Iterable) -> bool:
     """
     Returns True, if the polygon described by the points is counterclockwise,
     False if it is clockwise.
     """
     return not is_cw(points)
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def global_shape_function_derivatives(dshp: ndarray, jac: ndarray) -> ndarray:
+    """
+    Calculates derivatives of shape functions wrt. the local axes of cells
+    using derivatives along master axes evaulated at some points in
+    the interval [-1, 1], and jacobian matrices of local-to-global mappings.
+
+    Parameters
+    ----------
+    dshp: numpy.ndarray
+        Derivatives of an nNE number of shape functions evaluated at an nP number
+        of points as a float array of shape (nP, nNE, nD).
+    jac: numpy.ndarray
+        Jacobian matrices, evaluated for a a nP number of points in nE number of cells
+        and for nD spatial dimensions as a float array of shape (nE, nP, nD, nD).
+
+    Returns
+    -------
+    numpy.ndarray
+        4d float array of shape (nE, nP, nNE, nD).
+    """
+    nP, nNE, nD = dshp.shape
+    nE = jac.shape[0]
+    res = np.zeros((nE, nP, nNE, nD), dtype=dshp.dtype)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            invJ = np.linalg.inv(jac[iE, iP])
+            res[iE, iP] = dshp[iP] @ invJ
+    return res
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/voxelize.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/voxelize.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/vtkcelltypes.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/vtkcelltypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     VTK_HEXAHEDRON = 12
     VTK_WEDGE = 13
     # VTK_PYRAMID = 14
     # VTK_PENTAGONAL_PRISM = 15
     # VTK_HEXAGONAL_PRISM = 16
 
     # # Quadratic, isoparametric cells
-    # VTK_QUADRATIC_EDGE = 21
+    VTK_QUADRATIC_EDGE = 21
     VTK_QUADRATIC_TRIANGLE = 22
     # VTK_QUADRATIC_QUAD = 23
     # VTK_QUADRATIC_POLYGON = 36
     VTK_QUADRATIC_TETRA = 24
     # VTK_QUADRATIC_HEXAHEDRON = 25
     # VTK_QUADRATIC_WEDGE = 26
     # VTK_QUADRATIC_PYRAMID = 27
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon/mesh/vtkutils.py` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/vtkutils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/PKG-INFO` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon.mesh
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package to build, manipulate and analyze polygonal meshes.
 Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 License: MIT License
         
         Copyright (c) 2021 SigmaEpsilon
         
@@ -80,28 +80,48 @@
 ## Projects using sigmaepsilon.mesh
 
 - [SigmaEpsilon](https://github.com/dewloosh/SigmaEpsilon) - A Python library for computational solid mechanics.
 - [PyAxisVM](https://github.com/AxisVM/pyaxisvm) - The official Python package of [AxisVM](https://axisvm.eu/), a popular structural analysis and design software.
 
 ## Documentation
 
-The [documentation](https://sigmaepsilon.mesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set examples, and the API Reference.
+The [documentation](https://sigmaepsilonmesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set examples, and the API Reference.
 
 ## Installation
 
 sigmaepsilon.mesh can be installed from PyPI using `pip` on Python >= 3.7:
 
 ```console
 >>> pip install sigmaepsilon.mesh
 ```
 
-## Testing
+or chechkout with the following command using GitHub CLI
 
 ```console
->>> python -m unittest
+gh repo clone sigma-epsilon/sigmaepsilon.mesh
+```
+
+and install from source by typing
+
+```console
+>>> pip install .
+```
+
+If you want to run the tests, you can install the package along with the necessary optional dependencies like this
+
+```console
+>>> pip install ".[test]"
+```
+
+### Development mode
+
+If you are a developer and want to install the library in development mode, the suggested way is by using this command:
+
+```console
+>>> pip install "-e .[test, dev]"
 ```
 
 ## How to contribute?
 
 Contributions are currently expected in any the following ways:
 
 - finding bugs
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/SOURCES.txt` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
 logo.png
 pyproject.toml
 requirements-dev.txt
-requirements-devops.txt
 requirements-test.txt
 requirements.txt
 tox.ini
 .circleci/config.yml
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
@@ -52,14 +51,15 @@
 docs/source/examples/grids2d.ipynb
 docs/source/examples/grids3d.ipynb
 docs/source/examples/import_file.ipynb
 docs/source/examples/import_gmsh.ipynb
 docs/source/examples/import_pyvista.ipynb
 docs/source/examples/joint_cube.ipynb
 docs/source/examples/lighting.ipynb
+docs/source/examples/shape_functions_1d.ipynb
 docs/source/examples/trigridQ4.ipynb
 docs/source/notebooks/data.ipynb
 docs/source/notebooks/grids.ipynb
 docs/source/notebooks/io.ipynb
 docs/source/notebooks/mesh_analysis.ipynb
 docs/source/notebooks/mesh_composition.ipynb
 docs/source/notebooks/mesh_structure.ipynb
@@ -147,22 +147,24 @@
 src/sigmaepsilon/mesh/utils/cells/utils.py
 src/sigmaepsilon/mesh/utils/cells/w18.py
 src/sigmaepsilon/mesh/utils/cells/w6.py
 src/sigmaepsilon/mesh/utils/topology/__init__.py
 src/sigmaepsilon/mesh/utils/topology/topo.py
 src/sigmaepsilon/mesh/utils/topology/tr.py
 tests/__init__.py
-tests/test_cells.py
 tests/test_colors.py
 tests/test_compound.py
 tests/test_geom.py
-tests/test_hex.py
 tests/test_io.py
 tests/test_linalg.py
 tests/test_mesh_anal.py
 tests/test_meshing.py
 tests/test_pointcloud.py
 tests/test_recipes.py
-tests/test_tet.py
 tests/test_topo.py
 tests/test_topo_tr.py
-tests/test_tri.py
+tests/test_tri.py
+tests/cells/__init__.py
+tests/cells/test_cells.py
+tests/cells/test_hex.py
+tests/cells/test_lines.py
+tests/cells/test_tet.py
```

### Comparing `sigmaepsilon.mesh-0.0.2/src/sigmaepsilon.mesh.egg-info/requires.txt` & `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,23 @@
 networkx>=3.0
 matplotlib
 vtk
 pyvista
 sectionproperties
 pythreejs
 ipyvtklink
+ipykernel
 pandas
 plotly
 tetgen
 autopep8
 awkward
 pyarrow
 
 [devops]
-autopep8
-flake8
-pytest
-pytest-cov
 
 [docs]
 ipython
 myst_parser
 nbsphinx
 sphinx-gallery
 sphinx_copybutton
```

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_cells.py` & `sigmaepsilon.mesh-0.0.3/tests/cells/test_cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 import unittest
 
 from sigmaepsilon.mesh.cells import H8, TET10
 from sigmaepsilon.mesh import grid, PolyData, CartesianFrame
 from sigmaepsilon.mesh.cells import H8
-from sigmaepsilon.mesh.space import PointCloud
 
 
 class TestGeneratedExpressions(unittest.TestCase):
     def test_generated_H8(self):
         pcoords = H8.lcoords()
         shpf = H8.shape_function_values
         shpmf = H8.shape_function_matrix
```

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_compound.py` & `sigmaepsilon.mesh-0.0.3/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_geom.py` & `sigmaepsilon.mesh-0.0.3/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_io.py` & `sigmaepsilon.mesh-0.0.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_linalg.py` & `sigmaepsilon.mesh-0.0.3/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_mesh_anal.py` & `sigmaepsilon.mesh-0.0.3/tests/test_mesh_anal.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_meshing.py` & `sigmaepsilon.mesh-0.0.3/tests/test_meshing.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         zres = 20
         mesh = circular_disk(n_angles, n_radii, min_radius, max_radius)
         points = mesh.coords()
         triangles = mesh.topology()
         points, triangles = detach_mesh_bulk(points, triangles)
         coords, topo = extrude_T3_TET4(points, triangles, h, zres)
 
-        vol_exact = np.pi * (max_radius**2 - min_radius**2) * h
+        vol_exact = np.pi * (max_radius ** 2 - min_radius ** 2) * h
 
         A = StandardFrame(dim=3)
         tetmesh = PolyData(coords=coords, topo=topo, celltype=TET4, frame=A)
         self.assertTrue(np.isclose(vol_exact, tetmesh.volume(), atol=vol_exact / 1000))
 
         trimesh = TriMesh(size=(800, 600), shape=(10, 10), frame=A)
         trimesh.area()
@@ -61,15 +61,15 @@
         zres = 20
         mesh = circular_disk(n_angles, n_radii, min_radius, max_radius)
         points = mesh.coords()
         triangles = mesh.topology()
         points, triangles = detach_mesh_bulk(points, triangles)
         coords, topo = extrude_T3_W6(points, triangles, h, zres)
 
-        vol_exact = np.pi * (max_radius**2 - min_radius**2) * h
+        vol_exact = np.pi * (max_radius ** 2 - min_radius ** 2) * h
 
         A = StandardFrame(dim=3)
         mesh = PolyData(coords=coords, topo=topo, celltype=W6, frame=A)
 
         self.assertTrue(np.isclose(vol_exact, mesh.volume(), atol=vol_exact / 1000))
 
     def test_tet(self):
```

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_pointcloud.py` & `sigmaepsilon.mesh-0.0.3/tests/test_pointcloud.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_recipes.py` & `sigmaepsilon.mesh-0.0.3/tests/test_recipes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import unittest
 import numpy as np
 
 
-from sigmaepsilon.mesh.recipes import circular_disk, ribbed_plate, perforated_cube, cylinder
+from sigmaepsilon.mesh.recipes import (
+    circular_disk,
+    ribbed_plate,
+    perforated_cube,
+    cylinder,
+)
 
 
 class TestRecipes(unittest.TestCase):
     def test_circular_disk(self):
         mesh = circular_disk(120, 60, 5, 25)
-        area = np.pi * (25**2 - 5**2)
+        area = np.pi * (25 ** 2 - 5 ** 2)
         self.assertTrue(np.isclose(mesh.area(), area, rtol=1e-3, atol=1e-3))
 
     def test_ribbed_plate(self):
         mesh = ribbed_plate(lx=5.0, ly=5.0, t=1.0)
         self.assertTrue(np.isclose(mesh.volume(), 25.0, rtol=1e-3, atol=1e-3))
         ribbed_plate(
             lx=5.0, ly=5.0, t=1.0, wx=1.0, hx=2.0, ex=0.05, wy=1.0, hy=2.0, ey=-0.05
@@ -41,15 +46,15 @@
         n_radii = 30
         min_radius = 5
         max_radius = 25
         n_z = 20
         h = 50
         angle = 1
 
-        vol = np.pi * (max_radius**2 - min_radius**2) * h
+        vol = np.pi * (max_radius ** 2 - min_radius ** 2) * h
 
         shape = (min_radius, max_radius), angle, h
         size = n_radii, n_angles, n_z
 
         cyl = cylinder(shape, size, voxelize=True)
         self.assertTrue(np.isclose(cyl.volume(), vol, rtol=1e-3, atol=1e-3))
```

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_tet.py` & `sigmaepsilon.mesh-0.0.3/tests/cells/test_tet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 import unittest
 
 from sigmaepsilon.mesh.trimesh import TriMesh
 from sigmaepsilon.mesh import CartesianFrame
 from sigmaepsilon.mesh.recipes import circular_disk
-from sigmaepsilon.mesh.cells import T3
+from sigmaepsilon.mesh.cells import T3, TET4, TET10
 
 
 class TestTet(unittest.TestCase):
     def test_vol_TET4(self):
         def test_vol_TET4(Lx, Ly, Lz, nx, ny, nz):
             try:
                 A = CartesianFrame(dim=3)
@@ -18,29 +18,43 @@
                 assert np.isclose(mesh3d.volume(), Lx * Ly * Lz)
                 return True
             except AssertionError:
                 return False
             except Exception as e:
                 raise e
 
-        assert test_vol_TET4(1.0, 1.0, 1.0, 2, 2, 2)
+        self.assertTrue(test_vol_TET4(1.0, 1.0, 1.0, 2, 2, 2))
 
     def test_vol_cylinder_TET4(self):
         def test_vol_cylinder_TET4(
             min_radius, max_radius, height, n_angles, n_radii, n_z
         ):
             try:
                 mesh2d = circular_disk(n_angles, n_radii, min_radius, max_radius)
                 mesh3d = mesh2d.extrude(h=height, N=n_z)
-                a = np.pi * (max_radius**2 - min_radius**2) * height
+                a = np.pi * (max_radius ** 2 - min_radius ** 2) * height
                 assert np.isclose(mesh3d.volume(), a, atol=0, rtol=a / 1000)
                 return True
             except AssertionError:
                 return False
             except Exception as e:
                 raise e
 
-        assert test_vol_cylinder_TET4(1.0, 10.0, 10.0, 120, 80, 5)
+        self.assertTrue(test_vol_cylinder_TET4(1.0, 10.0, 10.0, 120, 80, 5))
+
+    def test_shp_TET4(self):
+        pcoords = TET4.lcoords()
+        shpf, shpmf, dshpf = TET4.generate_class_functions(return_symbolic=False)
+        shpf(pcoords)
+        shpmf(pcoords)
+        dshpf(pcoords)
+
+    def test_shp_TET10(self):
+        pcoords = TET10.lcoords()
+        shpf, shpmf, dshpf = TET10.generate_class_functions(return_symbolic=False)
+        shpf(pcoords)
+        shpmf(pcoords)
+        dshpf(pcoords)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_topo_tr.py` & `sigmaepsilon.mesh-0.0.3/tests/test_topo_tr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.2/tests/test_tri.py` & `sigmaepsilon.mesh-0.0.3/tests/test_tri.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,29 +36,29 @@
 
         assert test_area_T6(1.0, 1.0, 2, 2)
 
     def test_area_circular_disk_T3(self):
         def test_area_circular_disk_T3(min_radius, max_radius, n_angles, n_radii):
             try:
                 mesh = circular_disk(n_angles, n_radii, min_radius, max_radius)
-                a = np.pi * (max_radius**2 - min_radius**2)
+                a = np.pi * (max_radius ** 2 - min_radius ** 2)
                 assert np.isclose(mesh.area(), a, atol=0, rtol=a / 1000)
                 return True
             except AssertionError:
                 return False
             except Exception as e:
                 raise e
 
         assert test_area_circular_disk_T3(1.0, 10.0, 120, 80)
 
     def test_area_circular_disk_T6(self):
         def test_area_circular_disk_T6(min_radius, max_radius, n_angles, n_radii):
             try:
                 mesh = circular_disk(n_angles, n_radii, min_radius, max_radius)
-                a = np.pi * (max_radius**2 - min_radius**2)
+                a = np.pi * (max_radius ** 2 - min_radius ** 2)
                 assert np.isclose(mesh.area(), a, atol=0, rtol=a / 1000)
                 return True
             except AssertionError:
                 return False
             except Exception as e:
                 raise e
```

