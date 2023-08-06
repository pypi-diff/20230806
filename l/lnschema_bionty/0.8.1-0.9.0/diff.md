# Comparing `tmp/lnschema_bionty-0.8.1.tar.gz` & `tmp/lnschema_bionty-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_bionty-0.8.1.tar", last modified: Mon Mar 20 10:22:20 2023, max compression
+gzip compressed data, was "lnschema_bionty-0.9.0.tar", last modified: Tue Mar 21 06:45:08 2023, max compression
```

## Comparing `lnschema_bionty-0.8.1.tar` & `lnschema_bionty-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     3480 2023-02-14 15:29:33.279664 lnschema_bionty-0.8.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-08-23 11:51:03.186619 lnschema_bionty-0.8.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-08-23 11:51:03.186763 lnschema_bionty-0.8.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1389 2023-02-16 14:34:32.877596 lnschema_bionty-0.8.1/.gitignore
--rw-r--r--   0        0        0     1795 2023-01-06 07:43:46.580344 lnschema_bionty-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2022-08-23 11:51:03.187129 lnschema_bionty-0.8.1/LICENSE
--rw-r--r--   0        0        0      243 2023-01-06 07:43:46.580584 lnschema_bionty-0.8.1/README.md
--rw-r--r--   0        0        0       57 2022-08-23 11:51:03.187375 lnschema_bionty-0.8.1/docs/api.md
--rw-r--r--   0        0        0     8826 2023-03-20 10:21:49.448242 lnschema_bionty-0.8.1/docs/changelog.md
--rw-r--r--   0        0        0       49 2022-09-22 21:00:37.428827 lnschema_bionty-0.8.1/docs/guide/index.md
--rw-r--r--   0        0        0     2887 2023-03-20 08:18:24.365261 lnschema_bionty-0.8.1/docs/guide/tables.ipynb
--rw-r--r--   0        0        0      116 2022-09-22 21:00:37.429270 lnschema_bionty-0.8.1/docs/index.md
--rw-r--r--   0        0        0      170 2022-08-23 11:51:03.188000 lnschema_bionty-0.8.1/lamin-project.yaml
--rw-r--r--   0        0        0      691 2023-03-20 10:21:40.517085 lnschema_bionty-0.8.1/lnschema_bionty/__init__.py
--rw-r--r--   0        0        0     4577 2023-03-20 10:20:31.330436 lnschema_bionty-0.8.1/lnschema_bionty/_core.py
--rw-r--r--   0        0        0     1082 2023-01-06 07:43:46.582239 lnschema_bionty-0.8.1/lnschema_bionty/_link.py
--rw-r--r--   0        0        0      430 2022-12-07 13:27:56.341671 lnschema_bionty-0.8.1/lnschema_bionty/dev/__init__.py
--rw-r--r--   0        0        0     1090 2023-03-07 09:28:31.990011 lnschema_bionty-0.8.1/lnschema_bionty/dev/_bionty.py
--rw-r--r--   0        0        0     1259 2023-01-17 05:20:50.348157 lnschema_bionty-0.8.1/lnschema_bionty/dev/_bionty_versions.py
--rw-r--r--   0        0        0     1637 2023-03-20 10:20:31.331270 lnschema_bionty-0.8.1/lnschema_bionty/dev/_id.py
--rw-r--r--   0        0        0      651 2022-11-03 00:41:22.899176 lnschema_bionty-0.8.1/lnschema_bionty/dev/_versions.py
--rw-r--r--   0        0        0      242 2023-03-20 10:20:31.331484 lnschema_bionty-0.8.1/lnschema_bionty/dev/id.py
--rw-r--r--   0        0        0      189 2023-01-06 07:43:46.583504 lnschema_bionty-0.8.1/lnschema_bionty/link.py
--rw-r--r--   0        0        0     1427 2023-01-06 07:43:46.584131 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-09-22-267d12e6f6f1-v0_4_0.py
--rw-r--r--   0        0        0      803 2023-01-06 07:43:46.584635 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-09-22-7f9a3b24a42b-v0_3_1.py
--rw-r--r--   0        0        0     2234 2023-01-06 07:43:46.585483 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-11-03-afda12fc80a8-v0_5_0.py
--rw-r--r--   0        0        0     2752 2023-01-06 07:43:46.585995 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-11-04-edff8c04b030-v0_5_3.py
--rw-r--r--   0        0        0     4956 2023-01-06 07:43:46.586507 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-11-18-a28d3b7a73b1-v0_6_1.py
--rw-r--r--   0        0        0     4879 2023-01-06 07:43:46.586702 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-12-07-4133eb176df0-v0_6_2.py
--rw-r--r--   0        0        0      837 2023-01-06 07:43:46.586820 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2023-01-05-076bc2188ec3-v0_6_4.py
--rw-r--r--   0        0        0     6249 2023-01-06 07:43:46.587075 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2023-01-05-078d771bc2a0-v0_6_3.py
--rw-r--r--   0        0        0     1222 2023-01-13 14:55:49.604212 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2023-01-05-6cbe4aa9aaec-v0_7_0.py
--rw-r--r--   0        0        0      969 2023-01-13 14:55:49.604331 lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2023-01-13-1df05e5b531f-v0_7_0b.py
--rw-r--r--   0        0        0      577 2023-02-14 11:52:39.345804 lnschema_bionty-0.8.1/noxfile.py
--rw-r--r--   0        0        0      927 2023-03-20 10:20:37.624783 lnschema_bionty-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      233 2023-03-12 09:41:16.165294 lnschema_bionty-0.8.1/tests/test_hash_id.py
--rw-r--r--   0        0        0     1122 2023-03-07 06:15:07.299822 lnschema_bionty-0.8.1/tests/test_migrations.py
--rw-r--r--   0        0        0      490 2022-09-22 21:00:37.430997 lnschema_bionty-0.8.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 lnschema_bionty-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3480 2023-02-14 15:29:33.279664 lnschema_bionty-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-08-23 11:51:03.186619 lnschema_bionty-0.9.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-08-23 11:51:03.186763 lnschema_bionty-0.9.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1389 2023-02-16 14:34:32.877596 lnschema_bionty-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1795 2023-01-06 07:43:46.580344 lnschema_bionty-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2022-08-23 11:51:03.187129 lnschema_bionty-0.9.0/LICENSE
+-rw-r--r--   0        0        0      243 2023-01-06 07:43:46.580584 lnschema_bionty-0.9.0/README.md
+-rw-r--r--   0        0        0       57 2022-08-23 11:51:03.187375 lnschema_bionty-0.9.0/docs/api.md
+-rw-r--r--   0        0        0     9121 2023-03-21 06:44:01.568940 lnschema_bionty-0.9.0/docs/changelog.md
+-rw-r--r--   0        0        0       49 2022-09-22 21:00:37.428827 lnschema_bionty-0.9.0/docs/guide/index.md
+-rw-r--r--   0        0        0     2887 2023-03-20 08:18:24.365261 lnschema_bionty-0.9.0/docs/guide/tables.ipynb
+-rw-r--r--   0        0        0      116 2022-09-22 21:00:37.429270 lnschema_bionty-0.9.0/docs/index.md
+-rw-r--r--   0        0        0      170 2022-08-23 11:51:03.188000 lnschema_bionty-0.9.0/lamin-project.yaml
+-rw-r--r--   0        0        0      802 2023-03-21 06:43:39.767149 lnschema_bionty-0.9.0/lnschema_bionty/__init__.py
+-rw-r--r--   0        0        0     5480 2023-03-21 06:41:27.679823 lnschema_bionty-0.9.0/lnschema_bionty/_core.py
+-rw-r--r--   0        0        0     1082 2023-01-06 07:43:46.582239 lnschema_bionty-0.9.0/lnschema_bionty/_link.py
+-rw-r--r--   0        0        0      430 2022-12-07 13:27:56.341671 lnschema_bionty-0.9.0/lnschema_bionty/dev/__init__.py
+-rw-r--r--   0        0        0     1090 2023-03-07 09:28:31.990011 lnschema_bionty-0.9.0/lnschema_bionty/dev/_bionty.py
+-rw-r--r--   0        0        0     1259 2023-01-17 05:20:50.348157 lnschema_bionty-0.9.0/lnschema_bionty/dev/_bionty_versions.py
+-rw-r--r--   0        0        0     1980 2023-03-21 06:41:27.680170 lnschema_bionty-0.9.0/lnschema_bionty/dev/_id.py
+-rw-r--r--   0        0        0      651 2022-11-03 00:41:22.899176 lnschema_bionty-0.9.0/lnschema_bionty/dev/_versions.py
+-rw-r--r--   0        0        0      356 2023-03-21 06:41:27.680466 lnschema_bionty-0.9.0/lnschema_bionty/dev/id.py
+-rw-r--r--   0        0        0      189 2023-01-06 07:43:46.583504 lnschema_bionty-0.9.0/lnschema_bionty/link.py
+-rw-r--r--   0        0        0     1427 2023-01-06 07:43:46.584131 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-09-22-267d12e6f6f1-v0_4_0.py
+-rw-r--r--   0        0        0      803 2023-01-06 07:43:46.584635 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-09-22-7f9a3b24a42b-v0_3_1.py
+-rw-r--r--   0        0        0     2234 2023-01-06 07:43:46.585483 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-11-03-afda12fc80a8-v0_5_0.py
+-rw-r--r--   0        0        0     2752 2023-01-06 07:43:46.585995 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-11-04-edff8c04b030-v0_5_3.py
+-rw-r--r--   0        0        0     4956 2023-01-06 07:43:46.586507 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-11-18-a28d3b7a73b1-v0_6_1.py
+-rw-r--r--   0        0        0     4879 2023-01-06 07:43:46.586702 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-12-07-4133eb176df0-v0_6_2.py
+-rw-r--r--   0        0        0      837 2023-01-06 07:43:46.586820 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2023-01-05-076bc2188ec3-v0_6_4.py
+-rw-r--r--   0        0        0     6249 2023-01-06 07:43:46.587075 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2023-01-05-078d771bc2a0-v0_6_3.py
+-rw-r--r--   0        0        0     1222 2023-01-13 14:55:49.604212 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2023-01-05-6cbe4aa9aaec-v0_7_0.py
+-rw-r--r--   0        0        0      969 2023-01-13 14:55:49.604331 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2023-01-13-1df05e5b531f-v0_7_0b.py
+-rw-r--r--   0        0        0     2629 2023-03-21 06:42:31.709295 lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2023-03-21-4429de4e490b-v0_9_0.py
+-rw-r--r--   0        0        0      577 2023-02-14 11:52:39.345804 lnschema_bionty-0.9.0/noxfile.py
+-rw-r--r--   0        0        0      927 2023-03-21 05:36:27.881466 lnschema_bionty-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      233 2023-03-12 09:41:16.165294 lnschema_bionty-0.9.0/tests/test_hash_id.py
+-rw-r--r--   0        0        0     1122 2023-03-07 06:15:07.299822 lnschema_bionty-0.9.0/tests/test_migrations.py
+-rw-r--r--   0        0        0      490 2022-09-22 21:00:37.430997 lnschema_bionty-0.9.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 lnschema_bionty-0.9.0/PKG-INFO
```

### Comparing `lnschema_bionty-0.8.1/.github/workflows/build.yml` & `lnschema_bionty-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/.github/workflows/latest-changes.yml` & `lnschema_bionty-0.9.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/.gitignore` & `lnschema_bionty-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/.pre-commit-config.yaml` & `lnschema_bionty-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/LICENSE` & `lnschema_bionty-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/docs/changelog.md` & `lnschema_bionty-0.9.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Add CellLine, Pathway, Phenotype | [63](https://github.com/laminlabs/lnschema-bionty/pull/63) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-21 | 0.9.0
+💚 Fix CI | [62](https://github.com/laminlabs/lnschema-bionty/pull/62) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-21 |
 ⬆️ Upgrade to bionty 0.9.0 | [61](https://github.com/laminlabs/lnschema-bionty/pull/61) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-20 | 0.8.1
 🎨 Allow hashing external IDs | [60](https://github.com/laminlabs/lnschema-bionty/pull/60) | [falexwolf](https://github.com/falexwolf) | 2023-03-10 |
 ⬆️ Stable release of bionty 0.8.0 | [59](https://github.com/laminlabs/lnschema-bionty/pull/59) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-09 | 0.8.0
 ⬆️ Bionty>=0.8rc3 | [58](https://github.com/laminlabs/lnschema-bionty/pull/58) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-09 | 0.8rc2
 ✨ Use ontology_id as the id for Tissue, CellType, Disease | [57](https://github.com/laminlabs/lnschema-bionty/pull/57) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-07 | 0.8.0rc1
 :arrow_up: Upgrade bionty | [56](https://github.com/laminlabs/lnschema-bionty/pull/56) | [falexwolf](https://github.com/falexwolf) | 2023-03-06 |
 🔥 Remove migration files | [51](https://github.com/laminlabs/lnschema-bionty/pull/51) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-14 | 0.7.0
```

### Comparing `lnschema_bionty-0.8.1/docs/guide/tables.ipynb` & `lnschema_bionty-0.9.0/docs/guide/tables.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/_core.py` & `lnschema_bionty-0.9.0/lnschema_bionty/_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,14 +67,35 @@
         sa_relationship_kwargs=dict(secondary=FeaturesProtein.__table__),
     )
 
 
 Features.proteins = relationship(Protein, back_populates="features", secondary=FeaturesProtein.__table__)
 
 
+class CellMarker(SQLModel, table=True):  # type: ignore
+    """Cell markers: protein complexes."""
+
+    __tablename__ = f"{prefix}cell_marker"
+
+    id: str = Field(default_factory=idg.cell_marker, primary_key=True)
+    name: str = Field(default=None, index=True, unique=True)
+    gene_symbols: Optional[str] = None  # TODO: link table
+    ncbi_gene_ids: Optional[str] = None  # TODO: link table
+    protein_names: Optional[str] = None  # TODO: link table
+    uniprotkb_ids: Optional[str] = None  # TODO: link table
+    species_id: str = Field(default=None, foreign_key="bionty.species.id")
+    features: Features = Relationship(
+        back_populates="cell_markers",
+        sa_relationship_kwargs=dict(secondary=FeaturesCellMarker.__table__),
+    )
+
+
+Features.cell_markers = relationship(CellMarker, back_populates="features", secondary=FeaturesCellMarker.__table__)
+
+
 @knowledge(bt.Tissue)
 class Tissue(SQLModel, table=True):  # type: ignore
     """Tissues."""
 
     id: str = Field(default_factory=idg.tissue, primary_key=True)
     ontology_id: str = Field(default=None, index=True, unique=True)
     name: str = Field(default=None, index=True)
@@ -91,31 +112,39 @@
     name: str = Field(default=None, index=True)
 
 
 @knowledge(bt.Disease)
 class Disease(SQLModel, table=True):  # type: ignore
     """Diseases."""
 
-    id: str = Field(default_factory=idg.tissue, primary_key=True)
+    id: str = Field(default_factory=idg.disease, primary_key=True)
     ontology_id: str = Field(default=None, index=True, unique=True)
     name: str = Field(default=None, index=True)
 
 
-class CellMarker(SQLModel, table=True):  # type: ignore
-    """Cell markers: protein complexes."""
+@knowledge(bt.CellLine)
+class CellLine(SQLModel, table=True):  # type: ignore
+    """Cell lines."""
 
-    __tablename__ = f"{prefix}cell_marker"
+    __tablename__ = f"{prefix}cell_line"
 
-    id: str = Field(default_factory=idg.cell_marker, primary_key=True)
-    name: str = Field(default=None, index=True, unique=True)
-    gene_symbols: Optional[str] = None  # TODO: link table
-    ncbi_gene_ids: Optional[str] = None  # TODO: link table
-    protein_names: Optional[str] = None  # TODO: link table
-    uniprotkb_ids: Optional[str] = None  # TODO: link table
-    species_id: str = Field(default=None, foreign_key="bionty.species.id")
-    features: Features = Relationship(
-        back_populates="cell_markers",
-        sa_relationship_kwargs=dict(secondary=FeaturesCellMarker.__table__),
-    )
+    id: str = Field(default_factory=idg.cell_line, primary_key=True)
+    ontology_id: str = Field(default=None, index=True, unique=True)
+    name: str = Field(default=None, index=True)
 
 
-Features.cell_markers = relationship(CellMarker, back_populates="features", secondary=FeaturesCellMarker.__table__)
+@knowledge(bt.Pathway)
+class Pathway(SQLModel, table=True):  # type: ignore
+    """Pathways."""
+
+    id: str = Field(default_factory=idg.pathway, primary_key=True)
+    ontology_id: str = Field(default=None, index=True, unique=True)
+    name: str = Field(default=None, index=True)
+
+
+@knowledge(bt.Phenotype)
+class Phenotype(SQLModel, table=True):  # type: ignore
+    """Phenotypes."""
+
+    id: str = Field(default_factory=idg.phenotype, primary_key=True)
+    ontology_id: str = Field(default=None, index=True, unique=True)
+    name: str = Field(default=None, index=True)
```

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/_link.py` & `lnschema_bionty-0.9.0/lnschema_bionty/_link.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/dev/_bionty.py` & `lnschema_bionty-0.9.0/lnschema_bionty/dev/_bionty.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/dev/_bionty_versions.py` & `lnschema_bionty-0.9.0/lnschema_bionty/dev/_bionty_versions.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/dev/_versions.py` & `lnschema_bionty-0.9.0/lnschema_bionty/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-09-22-267d12e6f6f1-v0_4_0.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-09-22-267d12e6f6f1-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-09-22-7f9a3b24a42b-v0_3_1.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-09-22-7f9a3b24a42b-v0_3_1.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-11-03-afda12fc80a8-v0_5_0.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-11-03-afda12fc80a8-v0_5_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-11-04-edff8c04b030-v0_5_3.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-11-04-edff8c04b030-v0_5_3.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-11-18-a28d3b7a73b1-v0_6_1.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-11-18-a28d3b7a73b1-v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2022-12-07-4133eb176df0-v0_6_2.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2022-12-07-4133eb176df0-v0_6_2.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2023-01-05-076bc2188ec3-v0_6_4.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2023-01-05-076bc2188ec3-v0_6_4.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2023-01-05-078d771bc2a0-v0_6_3.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2023-01-05-078d771bc2a0-v0_6_3.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2023-01-05-6cbe4aa9aaec-v0_7_0.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2023-01-05-6cbe4aa9aaec-v0_7_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/lnschema_bionty/migrations/versions/2023-01-13-1df05e5b531f-v0_7_0b.py` & `lnschema_bionty-0.9.0/lnschema_bionty/migrations/versions/2023-01-13-1df05e5b531f-v0_7_0b.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/noxfile.py` & `lnschema_bionty-0.9.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/pyproject.toml` & `lnschema_bionty-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 dev = [
     "pre-commit",
     "nox",
 ]
 test = [
     "pytest>=6.0",
     "pytest-cov",
-    "lndb>=0.37.4",
+    "lndb>=0.37.5",
 ]
 
 [tool.black]
 preview = true
 
 [tool.pytest.ini_options]
 testpaths = [
```

### Comparing `lnschema_bionty-0.8.1/tests/test_migrations.py` & `lnschema_bionty-0.9.0/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `lnschema_bionty-0.8.1/PKG-INFO` & `lnschema_bionty-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnschema_bionty
-Version: 0.8.1
+Version: 0.9.0
 Summary: Biological entities (`zdno`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Requires-Dist: lnschema_core>=0.29.1
 Requires-Dist: bionty>=0.9.0
 Requires-Dist: requests
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: lndb>=0.37.4 ; extra == "test"
+Requires-Dist: lndb>=0.37.5 ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnschema-bionty
 Provides-Extra: dev
 Provides-Extra: test
 
 [![pypi](https://img.shields.io/pypi/v/lnschema_bionty?color=%2334D058&label=pypi%20package)](https://pypi.org/project/lnschema_bionty)
 
 # lnschema-bionty: Biological entities (`zdno`)
```

