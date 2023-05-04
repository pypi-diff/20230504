# Comparing `tmp/pywry-0.5.0.tar.gz` & `tmp/pywry-0.5.1.tar.gz`

## Comparing `pywry-0.5.0.tar` & `pywry-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 pywry-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 pywry-0.5.0/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     2678 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     2149 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/websocket.rs
--rw-r--r--   0     1001      123    20668 2023-04-26 14:02:46.000000 pywry-0.5.0/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    61106 2023-04-26 14:02:46.000000 pywry-0.5.0/Cargo.lock
--rw-r--r--   0     1001      123    11147 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/core.py
--rw-r--r--   0     1001      123      985 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/backend.py
--rw-r--r--   0     1001      123      370 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123      180 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-26 14:02:46.000000 pywry-0.5.0/python/pywry/py.typed
--rw-r--r--   0     1001      123      792 2023-04-26 14:02:46.000000 pywry-0.5.0/Cargo.toml
--rw-r--r--   0     1001      123     2149 2023-04-26 14:02:46.000000 pywry-0.5.0/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-04-26 14:02:46.000000 pywry-0.5.0/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-04-26 14:02:46.000000 pywry-0.5.0/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-04-26 14:02:46.000000 pywry-0.5.0/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-04-26 14:02:46.000000 pywry-0.5.0/src/websocket.rs
--rw-r--r--   0     1001      123    20668 2023-04-26 14:02:46.000000 pywry-0.5.0/src/window.rs
--rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 pywry-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 pywry-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 pywry-0.5.1/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     2678 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     2149 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     1301 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123      334 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/ports.rs
+-rw-r--r--   0     1001      123     2896 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123     2507 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/websocket.rs
+-rw-r--r--   0     1001      123    21600 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    61106 2023-05-04 04:52:53.000000 pywry-0.5.1/Cargo.lock
+-rw-r--r--   0     1001      123      985 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/backend.py
+-rw-r--r--   0     1001      123        0 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/py.typed
+-rw-r--r--   0     1001      123      370 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123    11147 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/core.py
+-rw-r--r--   0     1001      123      180 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/__init__.py
+-rw-r--r--   0     1001      123      792 2023-05-04 04:52:53.000000 pywry-0.5.1/Cargo.toml
+-rw-r--r--   0     1001      123     2149 2023-05-04 04:52:53.000000 pywry-0.5.1/src/constants.rs
+-rw-r--r--   0     1001      123     1301 2023-05-04 04:52:53.000000 pywry-0.5.1/src/lib.rs
+-rw-r--r--   0     1001      123      334 2023-05-04 04:52:53.000000 pywry-0.5.1/src/ports.rs
+-rw-r--r--   0     1001      123     2896 2023-05-04 04:52:53.000000 pywry-0.5.1/src/structs.rs
+-rw-r--r--   0     1001      123     2507 2023-05-04 04:52:53.000000 pywry-0.5.1/src/websocket.rs
+-rw-r--r--   0     1001      123    21600 2023-05-04 04:52:53.000000 pywry-0.5.1/src/window.rs
+-rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 pywry-0.5.1/PKG-INFO
```

### Comparing `pywry-0.5.0/pyproject.toml` & `pywry-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywry"
-version = "0.5.0"
+version = "0.5.1"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
```

### Comparing `pywry-0.5.0/rust_src/pywry/Cargo.toml` & `pywry-0.5.1/rust_src/pywry/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.0"
+version = "0.5.1"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.0/rust_src/pywry/LICENSE` & `pywry-0.5.1/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/rust_src/pywry/README.md` & `pywry-0.5.1/rust_src/pywry/README.md`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/rust_src/pywry/src/constants.rs` & `pywry-0.5.1/rust_src/pywry/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/rust_src/pywry/src/lib.rs` & `pywry-0.5.1/rust_src/pywry/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/rust_src/pywry/src/structs.rs` & `pywry-0.5.1/rust_src/pywry/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/rust_src/pywry/src/websocket.rs` & `pywry-0.5.1/rust_src/pywry/src/websocket.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/rust_src/pywry/src/window.rs` & `pywry-0.5.1/rust_src/pywry/src/window.rs`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     DownloadComplete(Option<PathBuf>, bool, String, String, WindowId),
     #[cfg(not(target_os = "macos"))]
     BlobReceived(String, WindowId),
     BlobChunk(Option<String>),
     CloseWindow(WindowId),
     DevTools(WindowId),
     NewWindowCreated(WindowId),
+    OpenFile(Option<PathBuf>),
     #[cfg(not(target_os = "windows"))]
     NewWindow(String, Option<Icon>),
 }
 
 fn get_icon(icon: &str) -> Option<Icon> {
     let icon_object = match read(icon) {
         Err(_) => None,
@@ -186,15 +187,18 @@
 
                 let initialization_script = if !export_image.is_empty() {
                     format!(
                         "window.{} = {}; window.save_image = true; window.export_image = '{}';",
                         variable_name, variable_value, export_image
                     )
                 } else {
-                    format!("window.{} = {};", variable_name, variable_value)
+                    format!(
+                        "window.{} = {}; window.download_path = {:?};",
+                        variable_name, variable_value, download_path
+                    )
                 };
 
                 protocol.with_initialization_script(&initialization_script)
             } else {
                 protocol
             };
 
@@ -245,14 +249,18 @@
                     move |_, string| match string.as_str() {
                         _ if string.starts_with("data:") => {
                             let _ = proxy.send_event(UserEvent::BlobChunk(Some(string)));
                         }
                         "#EOF" => {
                             let _ = proxy.send_event(UserEvent::BlobChunk(None));
                         }
+                        _ if string.starts_with("#OPEN:") => {
+                            let _ = proxy
+                                .send_event(UserEvent::OpenFile(Some(PathBuf::from(&string[6..]))));
+                        }
                         "#DEVTOOLS" => {
                             let _ = proxy.send_event(UserEvent::DevTools(window_id));
                         }
                         _ => {}
                     }
                 })
                 .with_initialization_script(BLOBINIT_SCRIPT);
@@ -482,14 +490,26 @@
                 if let Some(webview) = webviews.get(&window_id) {
                     if debug {
                         println!("Opening DevTools");
                     }
                     let _ = webview.open_devtools();
                 }
             }
+            // UserEvent::OpenFile
+            Event::UserEvent(UserEvent::OpenFile(filepath)) => {
+                if filepath.is_some() {
+                    let decoded = urldecode(&filepath.unwrap().to_str().unwrap())
+                        .expect("UTF-8")
+                        .to_string();
+                    let path = PathBuf::from(decoded);
+                    if let Err(error) = open::that(&path.to_str().unwrap()) {
+                        println!("Error opening file: {}", error);
+                    }
+                }
+            }
             // WindowEvent::NewWindow
             #[cfg(not(target_os = "windows"))]
             Event::UserEvent(UserEvent::NewWindow(uri, window_icon)) => {
                 if debug {
                     println!("\nNew Window Requested: {}", uri);
                 }
                 if uri.starts_with("http://") || uri.starts_with("https://") {
```

### Comparing `pywry-0.5.0/Cargo.lock` & `pywry-0.5.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1494,15 +1494,15 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.5.0"
+version = "0.5.1"
 dependencies = [
  "futures-util",
  "image",
  "mime_guess",
  "open",
  "pyo3",
  "serde",
```

### Comparing `pywry-0.5.0/python/pywry/core.py` & `pywry-0.5.1/python/pywry/core.py`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/python/pywry/backend.py` & `pywry-0.5.1/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/Cargo.toml` & `pywry-0.5.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.0"
+version = "0.5.1"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.0/src/constants.rs` & `pywry-0.5.1/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/src/lib.rs` & `pywry-0.5.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/src/structs.rs` & `pywry-0.5.1/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/src/websocket.rs` & `pywry-0.5.1/src/websocket.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.0/src/window.rs` & `pywry-0.5.1/src/window.rs`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     DownloadComplete(Option<PathBuf>, bool, String, String, WindowId),
     #[cfg(not(target_os = "macos"))]
     BlobReceived(String, WindowId),
     BlobChunk(Option<String>),
     CloseWindow(WindowId),
     DevTools(WindowId),
     NewWindowCreated(WindowId),
+    OpenFile(Option<PathBuf>),
     #[cfg(not(target_os = "windows"))]
     NewWindow(String, Option<Icon>),
 }
 
 fn get_icon(icon: &str) -> Option<Icon> {
     let icon_object = match read(icon) {
         Err(_) => None,
@@ -186,15 +187,18 @@
 
                 let initialization_script = if !export_image.is_empty() {
                     format!(
                         "window.{} = {}; window.save_image = true; window.export_image = '{}';",
                         variable_name, variable_value, export_image
                     )
                 } else {
-                    format!("window.{} = {};", variable_name, variable_value)
+                    format!(
+                        "window.{} = {}; window.download_path = {:?};",
+                        variable_name, variable_value, download_path
+                    )
                 };
 
                 protocol.with_initialization_script(&initialization_script)
             } else {
                 protocol
             };
 
@@ -245,14 +249,18 @@
                     move |_, string| match string.as_str() {
                         _ if string.starts_with("data:") => {
                             let _ = proxy.send_event(UserEvent::BlobChunk(Some(string)));
                         }
                         "#EOF" => {
                             let _ = proxy.send_event(UserEvent::BlobChunk(None));
                         }
+                        _ if string.starts_with("#OPEN:") => {
+                            let _ = proxy
+                                .send_event(UserEvent::OpenFile(Some(PathBuf::from(&string[6..]))));
+                        }
                         "#DEVTOOLS" => {
                             let _ = proxy.send_event(UserEvent::DevTools(window_id));
                         }
                         _ => {}
                     }
                 })
                 .with_initialization_script(BLOBINIT_SCRIPT);
@@ -482,14 +490,26 @@
                 if let Some(webview) = webviews.get(&window_id) {
                     if debug {
                         println!("Opening DevTools");
                     }
                     let _ = webview.open_devtools();
                 }
             }
+            // UserEvent::OpenFile
+            Event::UserEvent(UserEvent::OpenFile(filepath)) => {
+                if filepath.is_some() {
+                    let decoded = urldecode(&filepath.unwrap().to_str().unwrap())
+                        .expect("UTF-8")
+                        .to_string();
+                    let path = PathBuf::from(decoded);
+                    if let Err(error) = open::that(&path.to_str().unwrap()) {
+                        println!("Error opening file: {}", error);
+                    }
+                }
+            }
             // WindowEvent::NewWindow
             #[cfg(not(target_os = "windows"))]
             Event::UserEvent(UserEvent::NewWindow(uri, window_icon)) => {
                 if debug {
                     println!("\nNew Window Requested: {}", uri);
                 }
                 if uri.starts_with("http://") || uri.starts_with("https://") {
```

### Comparing `pywry-0.5.0/PKG-INFO` & `pywry-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.5.0
+Version: 0.5.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: websockets
```

