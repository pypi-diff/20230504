# Comparing `tmp/spiff_element_units-0.2.0.tar.gz` & `tmp/spiff_element_units-0.3.0.tar.gz`

## Comparing `spiff_element_units-0.2.0.tar` & `spiff_element_units-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/Cargo.toml
--rw-r--r--   0     1001      123       20 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/.gitignore
--rw-r--r--   0     1001      123     1122 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/cache.rs
--rw-r--r--   0     1001      123     8367 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/domain.rs
--rw-r--r--   0     1001      123      619 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/element_units.rs
--rw-r--r--   0     1001      123     3076 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/lib.rs
--rw-r--r--   0     1001      123      349 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/manifest.rs
--rw-r--r--   0     1001      123     2452 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/reader.rs
--rw-r--r--   0     1001      123      910 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/writer.rs
--rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 spiff_element_units-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/.gitignore
--rw-r--r--   0     1001      123    35149 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/LICENSE
--rw-r--r--   0     1001      123      473 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      609 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/spiff_element_units.pyi
--rw-r--r--   0     1001      123     1326 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123    11005 2023-04-24 15:39:10.000000 spiff_element_units-0.2.0/Cargo.lock
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 spiff_element_units-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/Cargo.toml
+-rw-r--r--   0     1001      123       20 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/.gitignore
+-rw-r--r--   0     1001      123     3003 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/basis.rs
+-rw-r--r--   0     1001      123     1819 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/cache.rs
+-rw-r--r--   0     1001      123      266 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/config.rs
+-rw-r--r--   0     1001      123     5417 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/element_units.rs
+-rw-r--r--   0     1001      123     3416 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/lib.rs
+-rw-r--r--   0     1001      123      384 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/manifest.rs
+-rw-r--r--   0     1001      123     2451 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/reader.rs
+-rw-r--r--   0     1001      123     7372 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/specs.rs
+-rw-r--r--   0     1001      123     1038 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/writer.rs
+-rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 spiff_element_units-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/.gitignore
+-rw-r--r--   0     1001      123    35149 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/LICENSE
+-rw-r--r--   0     1001      123      473 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123      652 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/spiff_element_units.pyi
+-rw-r--r--   0     1001      123     1375 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123    11005 2023-05-04 02:17:58.000000 spiff_element_units-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 spiff_element_units-0.3.0/PKG-INFO
```

### Comparing `spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/cache.rs` & `spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/cache.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,11 @@
 use std::fs;
 use std::io;
 use std::path::{Path, PathBuf};
 
-pub mod entry {
-
-    pub enum Type {
-        OriginalWorkflowSpecsJSON,
-        Manifest,
-        ManifestEntry(String),
-    }
-
-    impl Type {
-        pub fn filename(&self) -> String {
-            use Type::*;
-
-            match self {
-                OriginalWorkflowSpecsJSON => "workflow_specs.json".to_string(),
-                Manifest => "manifest.json".to_string(),
-                ManifestEntry(id) => format!("{}.json", id),
-            }
-        }
-    }
-}
-
 const CACHE_VERSION: &str = "v1";
 
 pub fn created_path_for_entry(
     cache_dir: &str,
     cache_key: &str,
     entry_type: entry::Type,
 ) -> io::Result<PathBuf> {
@@ -39,7 +18,52 @@
 pub fn path_for_entry(cache_dir: &str, cache_key: &str, entry_type: entry::Type) -> PathBuf {
     cache_path(cache_dir, cache_key).join(entry_type.filename())
 }
 
 fn cache_path(cache_dir: &str, cache_key: &str) -> PathBuf {
     Path::new(cache_dir).join(CACHE_VERSION).join(cache_key)
 }
+
+pub mod entry {
+    use sha2::{Digest, Sha256};
+
+    pub enum Type<'a> {
+        OriginalWorkflowSpecsJSON,
+        Manifest(&'a str),
+        ManifestEntry(&'a str),
+    }
+
+    impl<'a> Type<'a> {
+        pub fn filename(&self) -> String {
+            use Type::*;
+
+            match self {
+                OriginalWorkflowSpecsJSON => "workflow_specs.json".to_string(),
+                Manifest(process_id) => format!("manifest.{:x}.json", Sha256::digest(process_id)),
+                ManifestEntry(sha2) => format!("{}.json", sha2),
+            }
+        }
+    }
+}
+
+pub mod manifest {
+    use crate::basis::IndexedVec;
+    use crate::element_units::{ElementUnit, ElementUnitType};
+    use serde::{Deserialize, Serialize};
+
+    #[derive(Debug, Deserialize, Serialize)]
+    pub struct ManifestEntry {
+        pub sha2: String,
+        pub r#type: ElementUnitType,
+    }
+
+    pub type Manifest = IndexedVec<ManifestEntry>;
+
+    impl ManifestEntry {
+        pub fn from_element_unit(element_unit: &ElementUnit) -> Self {
+            Self {
+                sha2: element_unit.sha2_str(),
+                r#type: element_unit.r#type(),
+            }
+        }
+    }
+}
```

### Comparing `spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/lib.rs` & `spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 use std::error::Error;
 use std::iter::zip;
 
+mod basis;
 mod cache;
-mod domain;
+mod config;
 mod element_units;
 mod manifest;
 mod reader;
+mod specs;
 mod writer;
 
 use cache::entry::Type as CacheEntryType;
-use domain::{ElementUnit, Manifest, WorkflowSpec};
+use cache::manifest::Manifest;
+use element_units::ElementUnit;
+
+const VERSION: &str = env!("CARGO_PKG_VERSION");
 
 //
 // this is the public api. it is a thin waist on purpose to make other
 // language bindings and caller interactions simple. we don't want to be
 // chatty or pass complicated structures across boundaries.
 //
 
@@ -40,53 +45,64 @@
     let entry_path = cache::created_path_for_entry(
         cache_dir,
         cache_key,
         CacheEntryType::OriginalWorkflowSpecsJSON,
     )?;
     writer::write_string(&entry_path, workflow_specs_json)?;
 
-    let el_units = element_units::from_json_string(&workflow_specs_json)?;
-    let manifest = manifest::from_element_units(&el_units);
-    let el_units_and_manifest_entries = zip(&el_units.items, &manifest.items);
+    let el_units_by_process_id = element_units::from_json_string(&workflow_specs_json)?;
+
+    for (process_id, el_units) in el_units_by_process_id.iter() {
+        let manifest = manifest::from_element_units(&el_units);
+        let el_units_and_manifest_entries = zip(&el_units.items, &manifest.items);
+
+        for (el_unit, manifest_entry) in el_units_and_manifest_entries {
+            let entry_path = cache::created_path_for_entry(
+                cache_dir,
+                cache_key,
+                CacheEntryType::ManifestEntry(&manifest_entry.sha2),
+            )?;
+            writer::write(&entry_path, el_unit)?;
+        }
 
-    for (el_unit, manifest_entry) in el_units_and_manifest_entries {
         let entry_path = cache::created_path_for_entry(
             cache_dir,
             cache_key,
-            CacheEntryType::ManifestEntry(manifest_entry.sha2.to_string()),
+            CacheEntryType::Manifest(process_id),
         )?;
-        writer::write(&entry_path, el_unit)?;
+        writer::write(&entry_path, &manifest)?;
     }
 
-    let entry_path = cache::created_path_for_entry(cache_dir, cache_key, CacheEntryType::Manifest)?;
-    writer::write(&entry_path, &manifest)?;
-
     Ok(())
 }
 
 //
 // get a workflow which can run a previously cached element unit that contains
 // the given element id.
 //
 pub fn workflow_from_cached_element_unit(
     cache_dir: &str,
     cache_key: &str,
+    process_id: &str,
     element_id: &str,
 ) -> ApiResult<String> {
-    let entry_path = cache::path_for_entry(cache_dir, cache_key, CacheEntryType::Manifest);
+    let entry_path =
+        cache::path_for_entry(cache_dir, cache_key, CacheEntryType::Manifest(process_id));
     let manifest = reader::read::<Manifest>(&entry_path)?;
     let manifest_entry = manifest
         .last_item_for_key(element_id.to_string())
         .ok_or("Element unit not found.")?;
 
     let entry_path = cache::path_for_entry(
         cache_dir,
         cache_key,
-        CacheEntryType::ManifestEntry(manifest_entry.sha2.to_string()),
+        CacheEntryType::ManifestEntry(&manifest_entry.sha2),
     );
     let element_unit = reader::read::<ElementUnit>(&entry_path)?;
-    let workflow_spec = WorkflowSpec::from_element_unit(&element_unit);
+    let mut workflow_spec = element_unit.to_workflow_spec();
+
+    workflow_spec.set_serializer_version(VERSION);
 
-    let contents = writer::write_to_string(workflow_spec)?;
+    let contents = writer::write_to_string(&workflow_spec)?;
 
     Ok(contents)
 }
```

### Comparing `spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/reader.rs` & `spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/reader.rs`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use std::path::Path;
 
-    use crate::domain::WorkflowSpec;
+    use crate::specs::WorkflowSpec;
 
     type ReadResult<T> = Result<T, Box<dyn Error>>;
 
     // don't need to fully test serde just that our structs line up against the json
 
     #[test]
     fn test_can_read_no_tasks() -> ReadResult<()> {
```

### Comparing `spiff_element_units-0.2.0/local_dependencies/spiff-element-units-rs/src/writer.rs` & `spiff_element_units-0.3.0/local_dependencies/spiff-element-units-rs/src/writer.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 use serde;
 use serde_json;
 use std::error::Error;
 use std::fs::File;
 use std::io::{self, BufWriter, Write};
 use std::path::PathBuf;
 
+use crate::config;
+
 //
 // write `contents` to file at `path`.
 //
 pub fn write_string(path: &PathBuf, contents: &str) -> io::Result<()> {
     let mut file = File::create(path)?;
     file.write_all(contents.as_bytes())?;
 
@@ -30,12 +32,18 @@
 //
 pub fn write<T>(path: &PathBuf, value: &T) -> Result<(), Box<dyn Error>>
 where
     T: ?Sized + serde::Serialize,
 {
     let file = File::create(path)?;
     let mut writer = BufWriter::new(file);
-    serde_json::to_writer_pretty(&mut writer, value)?;
+
+    if config::pretty_json() {
+        serde_json::to_writer_pretty(&mut writer, value)?;
+    } else {
+        serde_json::to_writer(&mut writer, value)?;
+    }
+
     writer.flush()?;
 
     Ok(())
 }
```

### Comparing `spiff_element_units-0.2.0/.gitignore` & `spiff_element_units-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spiff_element_units-0.2.0/LICENSE` & `spiff_element_units-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spiff_element_units-0.2.0/spiff_element_units.pyi` & `spiff_element_units-0.3.0/spiff_element_units.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -7,13 +7,14 @@
     workflow_specs_json and associates them with cache_key for later 
     retrieval.
     """
 
 def workflow_from_cached_element_unit(
         cache_dir: str,
         cache_key: str,
+        process_id: str,
         element_id: str) -> str:
     """
     Returns a workflow described in specs json format that is capable of 
-    executing an element unit that contains element_id and is associated 
-    with cache_key.
+    executing an element unit that contains element_id within process_id 
+    and is associated with cache_key.
     """
```

### Comparing `spiff_element_units-0.2.0/src/lib.rs` & `spiff_element_units-0.3.0/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,20 @@
     Ok(result)
 }
 
 #[pyfunction]
 fn workflow_from_cached_element_unit(
     cache_dir: String,
     cache_key: String,
+    process_id: String,
     element_id: String,
 ) -> PyResult<String> {
-    let result = lib::workflow_from_cached_element_unit(&cache_dir, &cache_key, &element_id)
-        .map_err(|e| PyValueError::new_err(e.to_string()))?;
+    let result =
+        lib::workflow_from_cached_element_unit(&cache_dir, &cache_key, &process_id, &element_id)
+            .map_err(|e| PyValueError::new_err(e.to_string()))?;
 
     Ok(result)
 }
 
 #[pymodule]
 fn spiff_element_units(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(cache_element_units_for_workflow, m)?)?;
```

### Comparing `spiff_element_units-0.2.0/Cargo.lock` & `spiff_element_units-0.3.0/Cargo.lock`

 * *Files identical despite different names*

```diff
@@ -279,23 +279,23 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "spiff-element-units"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "pyo3",
  "spiff-element-units-rs",
 ]
 
 [[package]]
 name = "spiff-element-units-rs"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "serde",
  "serde_json",
  "sha2",
 ]
 
 [[package]]
```

