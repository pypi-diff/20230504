# Comparing `tmp/blobtk-0.3.0.tar.gz` & `tmp/blobtk-0.3.1.tar.gz`

## Comparing `blobtk-0.3.0.tar` & `blobtk-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 blobtk-0.3.0/Cargo.toml
--rw-r--r--   0      501       20    59715 2023-05-03 14:59:16.000000 blobtk-0.3.0/Cargo.lock
--rw-r--r--   0      501       20      313 2023-05-03 14:59:16.000000 blobtk-0.3.0/pyproject.toml
--rw-r--r--   0      501       20     9018 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/bam.rs
--rw-r--r--   0      501       20    16853 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/blobdir.rs
--rw-r--r--   0      501       20     7517 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/cli.rs
--rw-r--r--   0      501       20      553 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/depth.rs
--rw-r--r--   0      501       20     1855 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/fasta.rs
--rw-r--r--   0      501       20     6177 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/fastq.rs
--rw-r--r--   0      501       20     1440 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/filter.rs
--rw-r--r--   0      501       20     2738 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/io.rs
--rw-r--r--   0      501       20      788 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/lib.rs
--rw-r--r--   0      501       20      659 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/main.rs
--rw-r--r--   0      501       20     4015 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/axis.rs
--rw-r--r--   0      501       20    17018 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/blob.rs
--rw-r--r--   0      501       20     2918 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/category.rs
--rw-r--r--   0      501       20     4029 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/chart.rs
--rw-r--r--   0      501       20    34935 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/component.rs
--rw-r--r--   0      501       20     2927 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/data.rs
--rw-r--r--   0      501       20    29455 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/snail.rs
--rw-r--r--   0      501       20     1020 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/style.rs
--rw-r--r--   0      501       20     9156 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot.rs
--rw-r--r--   0      501       20     3172 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/python/depth.rs
--rw-r--r--   0      501       20     3518 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/python/filter.rs
--rw-r--r--   0      501       20     1879 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/python/utils.rs
--rw-r--r--   0      501       20      491 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/python.rs
--rw-r--r--   0      501       20     6721 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/taxonomy.rs
--rw-r--r--   0      501       20     7612 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/utils.rs
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 blobtk-0.3.1/Cargo.toml
+-rw-r--r--   0      501       20    59715 2023-05-04 13:21:58.000000 blobtk-0.3.1/Cargo.lock
+-rw-r--r--   0      501       20      313 2023-05-04 13:21:58.000000 blobtk-0.3.1/pyproject.toml
+-rw-r--r--   0      501       20     9018 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/bam.rs
+-rw-r--r--   0      501       20    16853 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/blobdir.rs
+-rw-r--r--   0      501       20     7517 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/cli.rs
+-rw-r--r--   0      501       20      553 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/depth.rs
+-rw-r--r--   0      501       20     1855 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/fasta.rs
+-rw-r--r--   0      501       20     6177 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/fastq.rs
+-rw-r--r--   0      501       20     1440 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/filter.rs
+-rw-r--r--   0      501       20     2738 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/io.rs
+-rw-r--r--   0      501       20      788 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/lib.rs
+-rw-r--r--   0      501       20      659 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/main.rs
+-rw-r--r--   0      501       20     4015 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/axis.rs
+-rw-r--r--   0      501       20    16954 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/blob.rs
+-rw-r--r--   0      501       20     2888 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/category.rs
+-rw-r--r--   0      501       20     4029 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/chart.rs
+-rw-r--r--   0      501       20    34843 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/component.rs
+-rw-r--r--   0      501       20     2928 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/data.rs
+-rw-r--r--   0      501       20    29455 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/snail.rs
+-rw-r--r--   0      501       20     1020 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/style.rs
+-rw-r--r--   0      501       20     9156 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot.rs
+-rw-r--r--   0      501       20     3172 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/python/depth.rs
+-rw-r--r--   0      501       20     3518 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/python/filter.rs
+-rw-r--r--   0      501       20     1879 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/python/utils.rs
+-rw-r--r--   0      501       20      491 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/python.rs
+-rw-r--r--   0      501       20     4497 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/taxonomy.rs
+-rw-r--r--   0      501       20     7612 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/utils.rs
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.1/PKG-INFO
```

### Comparing `blobtk-0.3.0/Cargo.toml` & `blobtk-0.3.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "blobtk"
-version = "0.3.0"
+version = "0.3.1"
 edition = "2021"
 authors = [
     "Rich Challis <rc28@sanger.ac.uk>",
 ]
 license = "MIT"
 description = "Core utilities for BlobToolKit."
 homepage = "https://github.com/blobtoolkit/blobtk"
```

### Comparing `blobtk-0.3.0/Cargo.lock` & `blobtk-0.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "blobtk"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "atty",
  "clap",
  "colorous",
  "coord_transforms",
  "flate2",
  "glob",
```

### Comparing `blobtk-0.3.0/src/bam.rs` & `blobtk-0.3.1/src/bam.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/blobdir.rs` & `blobtk-0.3.1/src/blobdir.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/cli.rs` & `blobtk-0.3.1/src/cli.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/depth.rs` & `blobtk-0.3.1/src/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/fasta.rs` & `blobtk-0.3.1/src/fasta.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/fastq.rs` & `blobtk-0.3.1/src/fastq.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/filter.rs` & `blobtk-0.3.1/src/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/io.rs` & `blobtk-0.3.1/src/io.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/lib.rs` & `blobtk-0.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/main.rs` & `blobtk-0.3.1/src/main.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/plot/axis.rs` & `blobtk-0.3.1/src/plot/axis.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/plot/blob.rs` & `blobtk-0.3.1/src/plot/blob.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 use std::borrow::Borrow;
 use std::collections::HashMap;
-use std::default;
+
 use std::str::FromStr;
 
 use svg::node::element::{Circle, Group, Rectangle};
 use svg::Document;
 
-use crate::blobdir::FieldMeta;
-use crate::utils::{max_float, scale_float, scale_floats};
+use crate::utils::{max_float, scale_floats};
 use crate::{blobdir, cli, plot};
 
 use plot::category::Category;
 
 use super::axis::{AxisName, AxisOptions, ChartAxes, Position, Scale};
 use super::chart::{Chart, Dimensions};
 use super::component::{chart_axis, legend, LegendShape};
-use super::data::{self, Bin, HistogramData, ScatterData, ScatterPoint};
+use super::data::{Bin, HistogramData, ScatterData, ScatterPoint};
 use super::style::{path_filled, path_open};
 
 #[derive(Clone, Debug)]
 pub struct BlobData {
     pub x: Vec<f64>,
     pub y: Vec<f64>,
     pub z: Vec<f64>,
@@ -127,15 +126,15 @@
     (histograms, max_bin)
 }
 
 pub fn blob_points(
     axes: HashMap<String, String>,
     blob_data: &BlobData,
     meta: &blobdir::Meta,
-    options: &cli::PlotOptions,
+    _options: &cli::PlotOptions,
 ) -> ScatterData {
     let dimensions = BlobDimensions {
         ..Default::default()
     };
     let default_clamp = 0.1;
     let fields = meta.field_list.clone().unwrap();
     let x_meta = fields[axes["x"].as_str()].clone();
@@ -239,15 +238,15 @@
 pub fn plot(
     blob_dimensions: BlobDimensions,
     scatter_data: ScatterData,
     hist_data_x: Vec<HistogramData>,
     hist_data_y: Vec<HistogramData>,
     x_max: f64,
     y_max: f64,
-    options: &cli::PlotOptions,
+    _options: &cli::PlotOptions,
 ) -> Document {
     let height = blob_dimensions.height
         + blob_dimensions.hist_height
         + blob_dimensions.margin[0]
         + blob_dimensions.margin[2]
         + blob_dimensions.padding[0]
         + blob_dimensions.padding[2];
@@ -445,15 +444,15 @@
 }
 
 pub fn svg(
     dimensions: &BlobDimensions,
     scatter_data: &ScatterData,
     hist_data_x: &Vec<HistogramData>,
     hist_data_y: &Vec<HistogramData>,
-    options: &cli::PlotOptions,
+    _options: &cli::PlotOptions,
 ) -> Document {
     let mut scatter_group = Group::new().set(
         "transform",
         format!(
             "translate({}, {})",
             dimensions.padding[3], dimensions.padding[0]
         ),
```

### Comparing `blobtk-0.3.0/src/plot/category.rs` & `blobtk-0.3.1/src/plot/category.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 use std::borrow::BorrowMut;
 use std::collections::HashMap;
 
-use rust_htslib::bam::index;
-
 #[derive(Clone, Debug)]
 pub struct Category {
     pub label: String,
     pub members: Vec<String>,
     pub indices: Vec<usize>,
     pub color: String,
 }
```

### Comparing `blobtk-0.3.0/src/plot/chart.rs` & `blobtk-0.3.1/src/plot/chart.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/plot/component.rs` & `blobtk-0.3.1/src/plot/component.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 use num_integer::div_rem;
 use svg::node::element::path::Data;
 use svg::node::element::{Circle, Group, Line, Path, Rectangle, Text};
 use svg::node::Text as nodeText;
 
 use crate::utils::{format_si, linear_scale, linear_scale_float, scale_float, scale_floats};
 
-use super::axis::{self, AxisOptions, Position, Scale, ScatterAxis, TickOptions, TickStatus};
-use super::blob::BlobDimensions;
-use super::data::{self, HistogramData};
+use super::axis::{AxisOptions, Position, Scale, TickOptions, TickStatus};
 
 #[derive(Clone, Debug)]
 pub struct RadialTick {
     pub index: usize,
     pub offset: f64,
     pub angle: f64,
     pub label: Text,
```

### Comparing `blobtk-0.3.0/src/plot/data.rs` & `blobtk-0.3.1/src/plot/data.rs`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             axis: AxisName::X,
             category: None,
         }
     }
 }
 
 impl HistogramData {
-    pub fn to_path_data(self, position: Position, filled: bool) -> Data {
+    pub fn to_path_data(self, position: Position, _filled: bool) -> Data {
         let shift = self.max_bin;
         let (mut offset, mut path_data) = match position {
             Position::TOP | Position::BOTTOM => (0.0, Data::new().move_to((0.0, shift))),
             Position::RIGHT | Position::LEFT => {
                 (self.width, Data::new().move_to((0.0, self.width)))
             }
         };
```

### Comparing `blobtk-0.3.0/src/plot/snail.rs` & `blobtk-0.3.1/src/plot/snail.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/plot/style.rs` & `blobtk-0.3.1/src/plot/style.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/plot.rs` & `blobtk-0.3.1/src/plot.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/python/depth.rs` & `blobtk-0.3.1/src/python/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/python/filter.rs` & `blobtk-0.3.1/src/python/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/python/utils.rs` & `blobtk-0.3.1/src/python/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/src/utils.rs` & `blobtk-0.3.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.0/PKG-INFO` & `blobtk-0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobtk
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Core utilities for BlobToolKit.
 Keywords: bioinformatics,blobtoolkit,genome,genomics
 Home-Page: https://github.com/blobtoolkit/blobtk
 Author: Rich Challis <rc28@sanger.ac.uk>
```

