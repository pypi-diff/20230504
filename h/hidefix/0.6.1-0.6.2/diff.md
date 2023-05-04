# Comparing `tmp/hidefix-0.6.1.tar.gz` & `tmp/hidefix-0.6.2.tar.gz`

## Comparing `hidefix-0.6.1.tar` & `hidefix-0.6.2.tar`

### file list

```diff
@@ -1,73 +1,75 @@
--rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 hidefix-0.6.1/Cargo.toml
--rw-r--r--   0     1001      123      197 2023-01-16 13:46:58.000000 hidefix-0.6.1/.envrc
--rw-r--r--   0     1001      123     1325 2023-01-16 13:46:58.000000 hidefix-0.6.1/.github/workflows/python.yml
--rw-r--r--   0     1001      123     3659 2023-01-16 13:46:58.000000 hidefix-0.6.1/.github/workflows/rust.yml
--rw-r--r--   0     1001      123      686 2023-01-16 13:46:58.000000 hidefix-0.6.1/.gitignore
--rw-r--r--   0     1001      123    30420 2023-01-16 13:46:58.000000 hidefix-0.6.1/Cargo.lock
--rw-r--r--   0     1001      123     3723 2023-01-16 13:46:58.000000 hidefix-0.6.1/README.md
--rw-r--r--   0     1001      123     3384 2023-01-16 13:46:58.000000 hidefix-0.6.1/benches/concurrency.rs
--rw-r--r--   0     1001      123      391 2023-01-16 13:46:58.000000 hidefix-0.6.1/benches/dataset.rs
--rw-r--r--   0     1001      123      200 2023-01-16 13:46:58.000000 hidefix-0.6.1/benches/index.rs
--rw-r--r--   0     1001      123     3283 2023-01-16 13:46:58.000000 hidefix-0.6.1/benches/large.rs
--rw-r--r--   0     1001      123     1613 2023-01-16 13:46:58.000000 hidefix-0.6.1/benches/native.rs
--rw-r--r--   0     1001      123     1938 2023-01-16 13:46:58.000000 hidefix-0.6.1/benches/read.rs
--rw-r--r--   0     1001      123     6695 2023-01-16 13:46:58.000000 hidefix-0.6.1/benches/serialize.rs
--rw-r--r--   0     1001      123     2580 2023-01-16 13:46:58.000000 hidefix-0.6.1/benches/stream.rs
--rw-r--r--   0     1001      123      118 2023-01-16 13:46:58.000000 hidefix-0.6.1/codecov.yml
--rw-r--r--   0     1001      123      521 2023-01-16 13:46:58.000000 hidefix-0.6.1/examples/cache.rs
--rw-r--r--   0     1001      123      687 2023-01-16 13:46:58.000000 hidefix-0.6.1/examples/direct.rs
--rw-r--r--   0     1001      123      450 2023-01-16 13:46:58.000000 hidefix-0.6.1/examples/native.rs
--rw-r--r--   0     1001      123    25891 2023-01-16 13:46:58.000000 hidefix-0.6.1/idefix.png
--rw-r--r--   0     1001      123      484 2023-01-16 13:46:58.000000 hidefix-0.6.1/pyproject.toml
--rw-r--r--   0     1001      123      111 2023-01-16 13:46:58.000000 hidefix-0.6.1/python/hidefix/__init__.py
--rw-r--r--   0     1001      123     5634 2023-01-16 13:46:58.000000 hidefix-0.6.1/python/hidefix/xarray.py
--rwxr-xr-x   0     1001      123      976 2023-01-16 13:47:26.000000 hidefix-0.6.1/run-maturin-action.sh
--rw-r--r--   0     1001      123      791 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/bin/hfxidx.rs
--rw-r--r--   0     1001      123     1024 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/bin/hfxlst.rs
--rw-r--r--   0     1001      123     4275 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/filters/byteorder.rs
--rw-r--r--   0     1001      123      337 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/filters/gzip.rs
--rw-r--r--   0     1001      123       63 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/filters/mod.rs
--rw-r--r--   0     1001      123     6686 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/filters/shuffle.rs
--rw-r--r--   0     1001      123     3668 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/filters/xdr.rs
--rw-r--r--   0     1001      123    12933 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/idx/chunk.rs
--rw-r--r--   0     1001      123     4782 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/idx/dataset/any.rs
--rw-r--r--   0     1001      123    19991 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/idx/dataset/dataset.rs
--rw-r--r--   0     1001      123    10754 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/idx/dataset/mod.rs
--rw-r--r--   0     1001      123     1228 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/idx/dataset/types.rs
--rw-r--r--   0     1001      123     5260 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/idx/index.rs
--rw-r--r--   0     1001      123     1606 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/idx/mod.rs
--rw-r--r--   0     1001      123     2452 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/idx/serde.rs
--rw-r--r--   0     1001      123     2622 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/lib.rs
--rw-r--r--   0     1001      123     9075 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/python/mod.rs
--rw-r--r--   0     1001      123     5819 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/reader/cache.rs
--rw-r--r--   0     1001      123     1639 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/reader/chunk.rs
--rw-r--r--   0     1001      123     6751 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/reader/dataset.rs
--rw-r--r--   0     1001      123     6678 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/reader/direct.rs
--rw-r--r--   0     1001      123      173 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/reader/mod.rs
--rw-r--r--   0     1001      123     7139 2023-01-16 13:46:58.000000 hidefix-0.6.1/src/reader/stream.rs
--rw-r--r--   0     1001      123      771 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/conftest.py
--rw-r--r--   0     1001      123  3142149 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/coads_climatology.nc4
--rw-r--r--   0     1001      123 10246776 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/chunked_fourD.h5
--rw-r--r--   0     1001      123    15980 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/chunked_gzipped_twoD.h5
--rw-r--r--   0     1001      123   163496 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/chunked_oneD.h5
--rw-r--r--   0     1001      123    44016 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/chunked_shuffled_twoD.h5
--rw-r--r--   0     1001      123     7032 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/chunked_shufzip_twoD.h5
--rw-r--r--   0     1001      123     3536 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/chunked_string_array.h5
--rw-r--r--   0     1001      123  4006256 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/chunked_threeD.h5
--rw-r--r--   0     1001      123    44016 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/chunked_twoD.h5
--rw-r--r--   0     1001      123     4392 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/t_float.h5
--rw-r--r--   0     1001      123     2148 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/dmrpp/t_int_scalar.h5
--rw-r--r--   0     1001      123    22130 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/feb.nc4
--rw-r--r--   0     1001      123  3520383 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/gzip_shuffle_2d.h5
--rw-r--r--   0     1001      123      299 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/data/gzip_shuffle_2d.py
--rw-r--r--   0     1001      123      371 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/python/test_index.py
--rw-r--r--   0     1001      123      460 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/python/test_netcdf.py
--rw-r--r--   0     1001      123      249 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/python/test_read.py
--rw-r--r--   0     1001      123     1320 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/python/test_slice.py
--rw-r--r--   0     1001      123      660 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/python/test_xarray_backend.py
--rw-r--r--   0     1001      123      956 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/python/test_xarray_large.py
--rw-r--r--   0     1001      123     2698 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/read_dims.rs
--rw-r--r--   0     1001      123     1038 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/read_double.rs
--rw-r--r--   0     1001      123      507 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/read_strings.rs
--rw-r--r--   0     1001      123     1889 2023-01-16 13:46:58.000000 hidefix-0.6.1/tests/read_svim.rs
--rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 hidefix-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 hidefix-0.6.2/Cargo.toml
+-rw-r--r--   0     1001      123      197 2023-05-04 12:52:11.000000 hidefix-0.6.2/.envrc
+-rw-r--r--   0     1001      123     1376 2023-05-04 12:52:11.000000 hidefix-0.6.2/.github/workflows/python.yml
+-rw-r--r--   0     1001      123     3599 2023-05-04 12:52:11.000000 hidefix-0.6.2/.github/workflows/rust.yml
+-rw-r--r--   0     1001      123      681 2023-05-04 12:52:11.000000 hidefix-0.6.2/.gitignore
+-rw-r--r--   0     1001      123    33434 2023-05-04 12:55:51.000000 hidefix-0.6.2/Cargo.lock
+-rw-r--r--   0     1001      123     1072 2023-05-04 12:52:11.000000 hidefix-0.6.2/LICENSE
+-rw-r--r--   0     1001      123     4124 2023-05-04 12:52:11.000000 hidefix-0.6.2/README.md
+-rw-r--r--   0     1001      123     3384 2023-05-04 12:52:11.000000 hidefix-0.6.2/benches/concurrency.rs
+-rw-r--r--   0     1001      123      391 2023-05-04 12:52:11.000000 hidefix-0.6.2/benches/dataset.rs
+-rw-r--r--   0     1001      123      200 2023-05-04 12:52:11.000000 hidefix-0.6.2/benches/index.rs
+-rw-r--r--   0     1001      123     3403 2023-05-04 12:52:11.000000 hidefix-0.6.2/benches/large.rs
+-rw-r--r--   0     1001      123     1613 2023-05-04 12:52:11.000000 hidefix-0.6.2/benches/native.rs
+-rw-r--r--   0     1001      123     1938 2023-05-04 12:52:11.000000 hidefix-0.6.2/benches/read.rs
+-rw-r--r--   0     1001      123     6740 2023-05-04 12:52:11.000000 hidefix-0.6.2/benches/serialize.rs
+-rw-r--r--   0     1001      123     2580 2023-05-04 12:52:11.000000 hidefix-0.6.2/benches/stream.rs
+-rw-r--r--   0     1001      123      118 2023-05-04 12:52:11.000000 hidefix-0.6.2/codecov.yml
+-rw-r--r--   0     1001      123      521 2023-05-04 12:52:11.000000 hidefix-0.6.2/examples/cache.rs
+-rw-r--r--   0     1001      123      687 2023-05-04 12:52:11.000000 hidefix-0.6.2/examples/direct.rs
+-rw-r--r--   0     1001      123      450 2023-05-04 12:52:11.000000 hidefix-0.6.2/examples/native.rs
+-rw-r--r--   0     1001      123    25891 2023-05-04 12:52:11.000000 hidefix-0.6.2/idefix.png
+-rw-r--r--   0     1001      123      646 2023-05-04 12:52:11.000000 hidefix-0.6.2/pyproject.toml
+-rw-r--r--   0     1001      123      132 2023-05-04 12:52:11.000000 hidefix-0.6.2/python/hidefix/__init__.py
+-rw-r--r--   0     1001      123     5647 2023-05-04 12:52:11.000000 hidefix-0.6.2/python/hidefix/xarray.py
+-rwxr-xr-x   0     1001      123     1041 2023-05-04 12:52:42.000000 hidefix-0.6.2/run-maturin-action.sh
+-rw-r--r--   0     1001      123      790 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/bin/hfxidx.rs
+-rw-r--r--   0     1001      123     1023 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/bin/hfxlst.rs
+-rw-r--r--   0     1001      123     4275 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/filters/byteorder.rs
+-rw-r--r--   0     1001      123      337 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/filters/gzip.rs
+-rw-r--r--   0     1001      123       63 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/filters/mod.rs
+-rw-r--r--   0     1001      123     6686 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/filters/shuffle.rs
+-rw-r--r--   0     1001      123     3668 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/filters/xdr.rs
+-rw-r--r--   0     1001      123    12894 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/idx/chunk.rs
+-rw-r--r--   0     1001      123     4782 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/idx/dataset/any.rs
+-rw-r--r--   0     1001      123    19954 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/idx/dataset/dataset.rs
+-rw-r--r--   0     1001      123    10754 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/idx/dataset/mod.rs
+-rw-r--r--   0     1001      123     1228 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/idx/dataset/types.rs
+-rw-r--r--   0     1001      123     5260 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/idx/index.rs
+-rw-r--r--   0     1001      123     1606 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/idx/mod.rs
+-rw-r--r--   0     1001      123     2452 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/idx/serde.rs
+-rw-r--r--   0     1001      123     2622 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/lib.rs
+-rw-r--r--   0     1001      123     9079 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/python/mod.rs
+-rw-r--r--   0     1001      123     5819 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/reader/cache.rs
+-rw-r--r--   0     1001      123     1639 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/reader/chunk.rs
+-rw-r--r--   0     1001      123     6751 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/reader/dataset.rs
+-rw-r--r--   0     1001      123     6678 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/reader/direct.rs
+-rw-r--r--   0     1001      123      173 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/reader/mod.rs
+-rw-r--r--   0     1001      123     7135 2023-05-04 12:52:11.000000 hidefix-0.6.2/src/reader/stream.rs
+-rw-r--r--   0     1001      123      771 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/conftest.py
+-rw-r--r--   0     1001      123  3142149 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/coads_climatology.nc4
+-rw-r--r--   0     1001      123 10246776 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/chunked_fourD.h5
+-rw-r--r--   0     1001      123    15980 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/chunked_gzipped_twoD.h5
+-rw-r--r--   0     1001      123   163496 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/chunked_oneD.h5
+-rw-r--r--   0     1001      123    44016 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/chunked_shuffled_twoD.h5
+-rw-r--r--   0     1001      123     7032 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/chunked_shufzip_twoD.h5
+-rw-r--r--   0     1001      123     3536 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/chunked_string_array.h5
+-rw-r--r--   0     1001      123  4006256 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/chunked_threeD.h5
+-rw-r--r--   0     1001      123    44016 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/chunked_twoD.h5
+-rw-r--r--   0     1001      123     4392 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/t_float.h5
+-rw-r--r--   0     1001      123     2148 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/dmrpp/t_int_scalar.h5
+-rw-r--r--   0     1001      123    22130 2023-05-04 12:52:11.000000 hidefix-0.6.2/tests/data/feb.nc4
+-rw-r--r--   0     1001      123  3520383 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/data/gzip_shuffle_2d.h5
+-rw-r--r--   0     1001      123      299 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/data/gzip_shuffle_2d.py
+-rw-r--r--   0     1001      123    22291 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/data/jan.nc4
+-rw-r--r--   0     1001      123      371 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/python/test_index.py
+-rw-r--r--   0     1001      123      460 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/python/test_netcdf.py
+-rw-r--r--   0     1001      123      249 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/python/test_read.py
+-rw-r--r--   0     1001      123     1320 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/python/test_slice.py
+-rw-r--r--   0     1001      123     1134 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/python/test_xarray_backend.py
+-rw-r--r--   0     1001      123      956 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/python/test_xarray_large.py
+-rw-r--r--   0     1001      123     2698 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/read_dims.rs
+-rw-r--r--   0     1001      123     1038 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/read_double.rs
+-rw-r--r--   0     1001      123      507 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/read_strings.rs
+-rw-r--r--   0     1001      123     1889 2023-05-04 12:52:12.000000 hidefix-0.6.2/tests/read_svim.rs
+-rw-r--r--   0        0        0     4808 1970-01-01 00:00:00.000000 hidefix-0.6.2/PKG-INFO
```

### Comparing `hidefix-0.6.1/Cargo.toml` & `hidefix-0.6.2/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors = ["Gaute Hope <eg@gaute.vetsj.com>"]
 edition = "2021"
 keywords = ["hdf", "async", "concurrency"]
 license = "LGPL-3.0-or-later"
 name = "hidefix"
 repository = "https://github.com/gauteh/hidefix"
 description = "Concurrent HDF5 and NetCDF4 reader (experimental)"
-version = "0.6.1"
+version = "0.6.2"
 categories = [ "data", "hdf5", "scientific-data" ]
 
 [lib]
 name = "hidefix"
 crate-type = ["rlib", "cdylib"]
 
 [dependencies]
@@ -33,15 +33,15 @@
 libc = "0.2"
 hdf5 = "0.8"
 hdf5-sys = "0.8"
 hdf5-src = "0.8"
 log = "0.4"
 rayon = "1.6"
 ndarray = { version = "0.15", features = [ "rayon" ] }
-pyo3 = { version = "0.17.3", optional = true, features = ["anyhow", "auto-initialize", "abi3-py37"] }
+pyo3 = { version = "0.17.3", optional = true, features = ["anyhow", "auto-initialize", "abi3-py38"] }
 numpy = { version = "0.17.2", optional = true }
 
 [dependencies.serde]
 features = ["derive"]
 version = "1"
 
 [dependencies.tokio]
@@ -49,23 +49,23 @@
 version = "1"
 
 [dev-dependencies]
 rand = "0.8"
 sled = "0.34.6"
 
 [patch.crates-io]
-hdf5 = { git = "https://github.com/magnusuMET/hdf5-rust", branch = "hidefix" }
-hdf5-sys = { git = "https://github.com/magnusuMET/hdf5-rust", branch = "hidefix" }
-hdf5-src = { git = "https://github.com/magnusuMET/hdf5-rust", branch = "hidefix" }
+hdf5 = { git = "https://github.com/magnusuMET/hdf5-rust", branch = "hidefix_jan_2023" }
+hdf5-sys = { git = "https://github.com/magnusuMET/hdf5-rust", branch = "hidefix_jan_2023" }
+hdf5-src = { git = "https://github.com/magnusuMET/hdf5-rust", branch = "hidefix_jan_2023" }
 
 [profile.release]
 lto = 'thin'
 codegen-units = 1
 debug = true
 
 [features]
 default = ["static", "fast-index"]
 static = ["hdf5-sys/static", "hdf5-sys/zlib"]
-fast-index = ["hdf5-src/1_13"]
+fast-index = ["hdf5-src/1_14"]
 python = ["pyo3", "numpy"]
 extension-module = ["python", "pyo3/extension-module"]
```

### Comparing `hidefix-0.6.1/.github/workflows/python.yml` & `hidefix-0.6.2/.github/workflows/python.yml`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         rust-toolchain: nightly
         target: ${{ matrix.target }}
         manylinux: auto
         args: --release --sdist --out dist
     - name: Install built wheel
       if: matrix.target == 'x86_64'
       run: |
-        pip install hidefix --no-index --find-links dist --force-reinstall
+        pip install numpy xarray netCDF4
+        pip install hidefix --no-index --find-links dist --force-reinstall --no-deps
         python -c "import hidefix"
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
```

### Comparing `hidefix-0.6.1/.github/workflows/rust.yml` & `hidefix-0.6.2/.github/workflows/rust.yml`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,24 @@
           toolchain: '${{matrix.rust}}'
           override: true
           components: 'rustfmt, clippy'
       - name: Run cargo ${{matrix.command}}
         uses: actions-rs/cargo@v1
         with:
           command: ${{matrix.command}}
-          args: "${{matrix.command == 'fmt' && '--all -- --check' || matrix.command == 'doc' && '--workspace' || '--workspace -- -D warnings -D clippy::cargo'}}"
+          args: "${{matrix.command == 'fmt' && '--all -- --check' || matrix.command == 'doc' && '--workspace' || '--workspace -- -D warnings'}}"
 
   test:
     name: Test
     runs-on: ubuntu-${{matrix.ubuntu}}
     strategy:
       fail-fast: false
       matrix:
         include:
           - {ubuntu: 20.04, rust: nightly}
-          - {ubuntu: 20.04, rust: nightly}
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
       - name: Install Rust (${{matrix.rust}})
         uses: actions-rs/toolchain@v1
         with:
           toolchain: '${{matrix.rust}}'
```

### Comparing `hidefix-0.6.1/.gitignore` & `hidefix-0.6.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 .venv/
 env/
-bin/
 build/
 develop-eggs/
 dist/
 eggs/
 lib/
 lib64/
 parts/
```

### Comparing `hidefix-0.6.1/Cargo.lock` & `hidefix-0.6.2/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -11,52 +11,53 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.68"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2cb2f989d18dd141ab8ae82f64d1a8cdd37e0840f73a406896cf5e99502fab61"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "ascii"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d92bec98840b8f03a5ff5413de5293bfcd8bf96467cf5452609f939ec6f5de16"
 
 [[package]]
 name = "async-stream"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dad5c83079eae9969be7fadefe640a1c566901f05ff91ab221de4b6f68d9507e"
+checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
 dependencies = [
  "async-stream-impl",
  "futures-core",
+ "pin-project-lite",
 ]
 
 [[package]]
 name = "async-stream-impl"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10f203db73a71dfa2fb6dd22763990fa26f3d2625a6da2da900d23b87d26be27"
+checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -86,35 +87,35 @@
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "bytes"
-version = "1.3.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfb24e866b15a1af2a1b663f10c6b6b8f397a84aadb828f12e5b289ec23a3a3c"
+checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
 name = "cc"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a20104e2335ce8a659d6dd92a51a767a0c062599c73b343fd152cb401e828c3d"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cmake"
-version = "0.1.49"
+version = "0.1.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db34956e100b30725f2eb215f90d4871051239535632f84fea3bc92722c66b7c"
+checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -122,60 +123,60 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.13"
+version = "0.9.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01a9af1f4c2ef74bb8aa1f7e19706bc72d03598c8a570bb5de72243c7a9d9d5a"
+checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.7.1",
+ "memoffset 0.8.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "flexbuffers"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15d14128f06405808ce75bfebe11e9b0f9da18719ede6d7bdb1702d6bfe0f7e8"
 dependencies = [
@@ -194,88 +195,88 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38390104763dc37a5145a53c29c63c1290b5d316d6086ec32c293f6736051bb0"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52ba265a92256105f45b719605a571ffe2d1f0fea3807304b522c1d778f79eed"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04909a7a7e4633ae6c4a9ab280aeb86da1236243a77b694a49eacd659a4bd3ac"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7acc85df6714c176ab5edf386123fafe217be88c0840ec11f199441134a074e2"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00f5fb52a06bdcadeb54e8d3671f8888a39697dcb0b81b23b55174030427f4eb"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdfb8ce053d86b91919aad980c220b1fb8401a9394410e1c289ed7e66b61835d"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39c15cf1a4aa79df40f1bb462fb39676d0ad9e366c2a33b590d7c66f4f81fcf9"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ffb393ac5d9a6eaa9d3fdf37ae2776656b706e200c8e16b1bdb227f5198e6ea"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "197676987abd2f9cadff84926f410af1c183608d36641465df73ae8211dc65d6"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -292,17 +293,17 @@
 checksum = "c31b6d751ae2c7f11320402d34e41349dd1016f8d5d45e48c4312bc8625af50c"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -313,52 +314,52 @@
 dependencies = [
  "ahash",
 ]
 
 [[package]]
 name = "hdf5"
 version = "0.8.1"
-source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix#038eb65aea4cc52cad26d176e3b17b796c749da3"
+source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix_jan_2023#90f05d0ce4af1ffa684f70255e636638e48ff901"
 dependencies = [
  "bitflags",
  "cfg-if",
  "hdf5-derive",
  "hdf5-sys",
  "hdf5-types",
  "lazy_static",
  "libc",
  "ndarray",
- "parking_lot 0.12.1",
+ "parking_lot 0.11.2",
  "paste",
 ]
 
 [[package]]
 name = "hdf5-derive"
 version = "0.8.1"
-source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix#038eb65aea4cc52cad26d176e3b17b796c749da3"
+source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix_jan_2023#90f05d0ce4af1ffa684f70255e636638e48ff901"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "hdf5-src"
 version = "0.8.1"
-source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix#038eb65aea4cc52cad26d176e3b17b796c749da3"
+source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix_jan_2023#90f05d0ce4af1ffa684f70255e636638e48ff901"
 dependencies = [
  "cmake",
  "libz-sys",
 ]
 
 [[package]]
 name = "hdf5-sys"
 version = "0.8.1"
-source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix#038eb65aea4cc52cad26d176e3b17b796c749da3"
+source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix_jan_2023#90f05d0ce4af1ffa684f70255e636638e48ff901"
 dependencies = [
  "hdf5-src",
  "libc",
  "libloading",
  "libz-sys",
  "pkg-config",
  "regex",
@@ -366,15 +367,15 @@
  "serde_derive",
  "winreg",
 ]
 
 [[package]]
 name = "hdf5-types"
 version = "0.8.1"
-source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix#038eb65aea4cc52cad26d176e3b17b796c749da3"
+source = "git+https://github.com/magnusuMET/hdf5-rust?branch=hidefix_jan_2023#90f05d0ce4af1ffa684f70255e636638e48ff901"
 dependencies = [
  "ascii",
  "cfg-if",
  "hdf5-sys",
  "libc",
 ]
 
@@ -385,15 +386,15 @@
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hidefix"
-version = "0.6.1"
+version = "0.6.2"
 dependencies = [
  "anyhow",
  "async-stream",
  "bincode",
  "byte-slice-cast",
  "byteorder",
  "bytes",
@@ -419,18 +420,28 @@
  "sled",
  "strength_reduce",
  "tokio",
  "zerocopy",
 ]
 
 [[package]]
+name = "indexmap"
+version = "1.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+dependencies = [
+ "autocfg",
+ "hashbrown",
+]
+
+[[package]]
 name = "indoc"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
@@ -450,17 +461,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libdeflate-sys"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "216b62f1994d8186da0187ad3f925ba267ad44ae67761c7285577583b85b5c6d"
 dependencies = [
@@ -484,17 +495,17 @@
 dependencies = [
  "cfg-if",
  "winapi",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.8"
+version = "1.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9702761c3935f8cc2f101793272e202c72b99da8f4224a19ddcf1279a6450bbf"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -524,18 +535,19 @@
 checksum = "e999beba7b6e8345721bd280141ed958096a2e4abdf74f67ff4ce49b4b54e47a"
 dependencies = [
  "hashbrown",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -548,17 +560,17 @@
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
@@ -571,17 +583,17 @@
  "num-traits",
  "rawpointer",
  "rayon",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ae39348c8bc5fbd7f40c727a9925f03517afd2ab27d46702108b6a7e5414c19"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.45"
@@ -609,31 +621,31 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "num_enum"
-version = "0.5.7"
+version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf5395665662ef45796a4ff5486c5d41d29e0c09640af4c5f17fd94ee2c119c9"
+checksum = "1f646caf906c20226733ed5b1374287eb97e3c2a5c227ce668c1f2ce20ae57c9"
 dependencies = [
  "num_enum_derive",
 ]
 
 [[package]]
 name = "num_enum_derive"
-version = "0.5.7"
+version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b0498641e53dd6ac1a4f22547548caa6864cc4933784319cd1775271c5a46ce"
+checksum = "dcbff9bc912032c62bf65ef1d5aea88983b420f4f839db1e9b0c281a25c9c799"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "numpy"
 version = "0.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a462c1af5ba1fddec1488c4646993a23ae7931f9e170ccba23e9c7c834277797"
@@ -645,17 +657,17 @@
  "num-integer",
  "num-traits",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
 dependencies = [
@@ -667,15 +679,15 @@
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core 0.9.6",
+ "parking_lot_core 0.9.7",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
@@ -686,30 +698,30 @@
  "redox_syscall",
  "smallvec",
  "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.6"
+version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba1ef8814b5c993410bb3adfad7a5ed269563e4a2f90c41f5d85be7fb47133bf"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d01a5bd0424d00070b0098dd17ebca6f961a959dead1dbcbbbc1d1cd8d3deeba"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
@@ -717,33 +729,32 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro-crate"
-version = "1.2.1"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eda0fc3b0fb7c975631757e14d9049da17374063edb6ebbcbc54d880d4fe94e9"
+checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
 dependencies = [
  "once_cell",
- "thiserror",
- "toml",
+ "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
@@ -763,17 +774,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
@@ -817,33 +828,33 @@
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -878,27 +889,27 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cac410af5d00ab6884528b4ab69d1e8e146e8d471201800fa1b4524126de6ad3"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
@@ -909,69 +920,69 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
-version = "0.11.8"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "718dc5fff5b36f99093fc49b280cfc96ce6fc824317783bff5a1fed0c7a64819"
+checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "slab"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4614a76b2a8be0058caa9dbbaf66d988527d86d003c11a94fbd335d7661edcef"
+checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "sled"
 version = "0.34.7"
@@ -998,87 +1009,86 @@
 name = "strength_reduce"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "target-lexicon"
-version = "0.12.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
-
-[[package]]
-name = "thiserror"
-version = "1.0.38"
+name = "syn"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
- "thiserror-impl",
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
 ]
 
 [[package]]
-name = "thiserror-impl"
-version = "1.0.38"
+name = "target-lexicon"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tokio"
-version = "1.24.1"
+version = "1.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d9f76183f91ecfb55e1d7d5602bd1d979e38a3a522fe900241cf195624d67ae"
+checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
 dependencies = [
  "autocfg",
  "num_cpus",
  "pin-project-lite",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.8.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d266c00fde287f55d3f1c3e96c500c362a2b8c695076ec180f27918820bc6df8"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
-name = "toml"
-version = "0.5.10"
+name = "toml_datetime"
+version = "0.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
+
+[[package]]
+name = "toml_edit"
+version = "0.19.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1333c76748e868a4d9d1017b5ab53171dfd095f70c712fdb4653a406547f598f"
+checksum = "239410c8609e8125456927e6707163a3b1fdb40561e4b803bc041f466ccfdc13"
 dependencies = [
- "serde",
+ "indexmap",
+ "toml_datetime",
+ "winnow",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -1120,68 +1130,152 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.45.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+dependencies = [
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
+name = "windows-targets"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
+]
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "winnow"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
+dependencies = [
+ "memchr",
+]
 
 [[package]]
 name = "winreg"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
 dependencies = [
@@ -1203,9 +1297,9 @@
 name = "zerocopy-derive"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6505e6815af7de1746a08f69c69606bb45695a17149517680f3b2149713b19a3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
```

### Comparing `hidefix-0.6.1/README.md` & `hidefix-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 [![Crates.io](https://img.shields.io/crates/v/hidefix.svg)](https://crates.io/crates/hidefix)
+[![PyPI](https://img.shields.io/pypi/v/hidefix.svg)](https://pypi.org/project/hidefix/)
 [![Documentation](https://docs.rs/hidefix/badge.svg)](https://docs.rs/hidefix/)
-[![Build Status](https://github.com/gauteh/hidefix/workflows/CI/badge.svg)](https://github.com/gauteh/hidefix/actions?query=branch%3Amain)
+[![Build (rust)](https://github.com/gauteh/hidefix/workflows/Rust/badge.svg)](https://github.com/gauteh/hidefix/actions?query=branch%3Amain)
+[![Build (python)](https://github.com/gauteh/hidefix/workflows/Python/badge.svg)](https://github.com/gauteh/hidefix/actions?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/gauteh/hidefix/branch/main/graph/badge.svg)](https://codecov.io/gh/gauteh/hidefix)
 [![Rust nightly](https://img.shields.io/badge/rustc-nightly-orange)](https://rust-lang.github.io/rustup/installation/other.html)
 
 <img src="https://raw.githubusercontent.com/gauteh/hidefix/main/idefix.png">
 
 # HIDEFIX
 
-This library provides an alternative reader for the
+This Rust and Python library provides an alternative reader for the
 [HDF5](https://support.hdfgroup.org/HDF5/doc/H5.format.html) file or [NetCDF4
 file](https://www.unidata.ucar.edu/software/netcdf/docs/file_format_specifications.html)
 (which uses HDF5) which supports concurrent access to data. This is achieved by
 building an index of the chunks, allowing a thread to use many file handles to
 read the file. The original (native) HDF5 library is used to build the index,
 but once it has been created it is no longer needed. The index can be
 serialized to disk so that performing the indexing is not necessary.
 
+In Rust:
+
 ```rust
 use hidefix::prelude::*;
 
 let idx = Index::index("tests/data/coads_climatology.nc4").unwrap();
 let mut r = idx.reader("SST").unwrap();
 
 let values = r.values::<f32>(None, None).unwrap();
 
 println!("SST: {:?}", values);
 ```
 
+or with Python using Xarray:
+```python
+import xarray as xr
+import hidefix
+
+ds = xr.open_dataset('file.nc', engine='hidefix')
+print(ds)
+```
+
 ## Motivation
 
 The HDF5 library requires internal locks to be _thread-safe_ since it relies on
 internal buffers which cannot be safely accessed/written to from multiple
 threads. This effectively causes multi-threaded applications to use sequential
 reads, while competing for the locks. And also apparently cause each other
 trouble, perhaps through dropping cached chunks which other threads still need.
```

### Comparing `hidefix-0.6.1/benches/concurrency.rs` & `hidefix-0.6.2/benches/concurrency.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/benches/native.rs` & `hidefix-0.6.2/benches/native.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/benches/read.rs` & `hidefix-0.6.2/benches/read.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/benches/serialize.rs` & `hidefix-0.6.2/benches/serialize.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-#![feature(const_option_ext)]
 #![feature(test)]
 extern crate test;
 use test::Bencher;
 
 use hidefix::idx::Index;
 
-const FILE: &'static str = option_env!("HIDEFIX_LARGE_FILE").unwrap_or("");
+const FILE: Option<&'static str> = option_env!("HIDEFIX_LARGE_FILE");
 // const VAR: &'static str = env!("HIDEFIX_LARGE_VAR");
 
 mod serde_bincode {
     use super::*;
 
     #[bench]
     fn serialize_coads(b: &mut Bencher) {
@@ -48,57 +47,57 @@
             bincode::deserialize::<Index>(&b).unwrap();
         })
     }
 
     #[ignore]
     #[bench]
     fn serialize_large_bincode(b: &mut Bencher) {
-        let i = Index::index(FILE).unwrap();
+        let i = Index::index(FILE.unwrap()).unwrap();
 
         b.iter(|| bincode::serialize(&i).unwrap())
     }
 
     #[ignore]
     #[bench]
     fn deserialize_large_bincode(b: &mut Bencher) {
-        let i = Index::index(FILE).unwrap();
+        let i = Index::index(FILE.unwrap()).unwrap();
         let bb = bincode::serialize(&i).unwrap();
 
         b.iter(|| bincode::deserialize::<Index>(&bb).unwrap())
     }
 
     #[ignore]
     #[bench]
     fn serialize_large_bincode_file(b: &mut Bencher) {
-        let i = Index::index(FILE).unwrap();
+        let i = Index::index(FILE.unwrap()).unwrap();
 
         b.iter(|| {
             let f = std::fs::File::create("/tmp/large.idx.bc").unwrap();
             let w = std::io::BufWriter::new(f);
             bincode::serialize_into(w, &i).unwrap()
         })
     }
 
     #[ignore]
     #[bench]
     fn deserialize_large_bincode_file(b: &mut Bencher) {
-        let i = Index::index(FILE).unwrap();
+        let i = Index::index(FILE.unwrap()).unwrap();
         let f = std::fs::File::create("/tmp/large.idx.bc").unwrap();
         bincode::serialize_into(f, &i).unwrap();
 
         b.iter(|| {
             let b = std::fs::read("/tmp/large.idx.bc").unwrap();
             bincode::deserialize::<Index>(&b).unwrap();
         })
     }
 
     #[ignore]
     #[bench]
     fn deserialize_large_bincode_db_sled(b: &mut Bencher) {
-        let i = Index::index(FILE).unwrap();
+        let i = Index::index(FILE.unwrap()).unwrap();
 
         let bts = bincode::serialize(&i).unwrap();
 
         let db = sled::Config::default()
             .temporary(true)
             .print_profile_on_drop(true)
             .open()
@@ -111,15 +110,15 @@
             test::black_box(bincode::deserialize::<Index>(&bts).unwrap());
         })
     }
 
     #[ignore]
     #[bench]
     fn deserialize_large_bincode_db_sled_only_read(b: &mut Bencher) {
-        let i = Index::index(FILE).unwrap();
+        let i = Index::index(FILE.unwrap()).unwrap();
 
         let bts = bincode::serialize(&i).unwrap();
 
         let db = sled::Config::default()
             .temporary(true)
             .print_profile_on_drop(true)
             .open()
@@ -131,15 +130,15 @@
             test::black_box(db.get("large").unwrap().unwrap());
         })
     }
 
     #[ignore]
     #[bench]
     fn deserialize_large_file_only_read(b: &mut Bencher) {
-        let i = Index::index(FILE).unwrap();
+        let i = Index::index(FILE.unwrap()).unwrap();
         let f = std::fs::File::create("/tmp/large.idx.bc").unwrap();
         bincode::serialize_into(f, &i).unwrap();
 
         b.iter(|| {
             test::black_box(std::fs::read("/tmp/large.idx.bc").unwrap());
         })
     }
@@ -206,29 +205,29 @@
             test::black_box(std::fs::read("/tmp/coads.idx.fx").unwrap());
         })
     }
 
     #[ignore]
     #[bench]
     fn deserialize_large_file(b: &mut Bencher) {
-        let i = Index::index(FILE).unwrap();
+        let i = Index::index(FILE.unwrap()).unwrap();
         let mut s = ser::new();
         i.serialize(&mut s).unwrap();
         std::fs::write("/tmp/large.idx.fx", s.view()).unwrap();
 
         b.iter(|| {
             let b = std::fs::read("/tmp/large.idx.fx").unwrap();
             flexbuffers::from_slice::<Index>(&b).unwrap();
         })
     }
 
     #[ignore]
     #[bench]
     fn deserialize_large_file_only_read(b: &mut Bencher) {
-        let i = Index::index(FILE).unwrap();
+        let i = Index::index(FILE.unwrap()).unwrap();
         let mut s = ser::new();
         i.serialize(&mut s).unwrap();
         std::fs::write("/tmp/large.idx.fx", s.view()).unwrap();
 
         b.iter(|| {
             test::black_box(std::fs::read("/tmp/large.idx.fx").unwrap());
         })
```

### Comparing `hidefix-0.6.1/benches/stream.rs` & `hidefix-0.6.2/benches/stream.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/examples/cache.rs` & `hidefix-0.6.2/examples/cache.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/examples/direct.rs` & `hidefix-0.6.2/examples/direct.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/idefix.png` & `hidefix-0.6.2/idefix.png`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/python/hidefix/xarray.py` & `hidefix-0.6.2/python/hidefix/xarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,8 +185,8 @@
         array = self.store.idx[self.variable_name]
         data = array[key]
         if self.fill_value is not None:
             array.apply_fill_value(self.fill_value, np.nan, data)
         return data
 
 
-BACKEND_ENTRYPOINTS["hidefix"] = HidefixBackendEntrypoint
+BACKEND_ENTRYPOINTS["hidefix"] = ('hidefix', HidefixBackendEntrypoint)
```

### Comparing `hidefix-0.6.1/run-maturin-action.sh` & `hidefix-0.6.2/run-maturin-action.sh`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 set -e
 echo "::group::Install Rust"
 which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain nightly
 export PATH="$HOME/.cargo/bin:$PATH"
 rustup override set nightly
 rustup component add llvm-tools-preview || true
 echo "::endgroup::"
-export PATH="$PATH:/opt/python/cp36-cp36m/bin:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin"
+export PATH="$PATH:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin:/opt/python/cp310-cp310/bin:/opt/python/cp311-cp311/bin"
 echo "::group::Install maturin"
-curl -L https://github.com/PyO3/maturin/releases/download/v0.14.10/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
+curl -L https://github.com/PyO3/maturin/releases/download/v0.14.17/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
+python3 -m pip install cffi || true
 echo "::endgroup::"
 echo "::group::Install Rust target"
 if [[ ! -d $(rustc --print target-libdir --target x86_64-unknown-linux-gnu) ]]; then rustup target add x86_64-unknown-linux-gnu; fi
 echo "::endgroup::"
-maturin build --release --sdist --out dist --target x86_64-unknown-linux-gnu
+maturin build --target x86_64-unknown-linux-gnu --release --sdist --out dist
```

### Comparing `hidefix-0.6.1/src/bin/hfxidx.rs` & `hidefix-0.6.2/src/bin/hfxidx.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-///! Create an index serialized to a flexbuffer.
+//! Create an index serialized to a flexbuffer.
 use std::env;
 
 #[macro_use]
 extern crate anyhow;
 
 use flexbuffers::FlexbufferSerializer as ser;
 use hidefix::idx::Index;
```

### Comparing `hidefix-0.6.1/src/bin/hfxlst.rs` & `hidefix-0.6.2/src/bin/hfxlst.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-///! List a summary of a flexbuffer serialized index to stdout.
+//! List a summary of a flexbuffer serialized index to stdout.
 use std::env;
 
 #[macro_use]
 extern crate anyhow;
 
 fn usage() {
     println!("Usage: hfxlst input.h5.idx");
```

### Comparing `hidefix-0.6.1/src/filters/byteorder.rs` & `hidefix-0.6.2/src/filters/byteorder.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/filters/shuffle.rs` & `hidefix-0.6.2/src/filters/shuffle.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/filters/xdr.rs` & `hidefix-0.6.2/src/filters/xdr.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/idx/chunk.rs` & `hidefix-0.6.2/src/idx/chunk.rs`

 * *Files 2% similar despite different names*

```diff
@@ -97,21 +97,21 @@
     /// on unsafe code.
     pub fn slice_as_u64s(chunks: &[Chunk<D>]) -> &[ULE] {
         let ptr = chunks.as_ptr() as *const Chunk<D>;
         let slice: &[ULE] = unsafe {
             let ptr = ptr as *const ULE;
             std::slice::from_raw_parts(
                 ptr,
-                chunks.len() * std::mem::size_of::<Self>() / std::mem::size_of::<ULE>(),
+                std::mem::size_of_val(chunks) / std::mem::size_of::<ULE>(),
             )
         };
 
         assert_eq!(
             slice.len(),
-            chunks.len() * std::mem::size_of::<Self>() / std::mem::size_of::<ULE>()
+            std::mem::size_of_val(chunks) / std::mem::size_of::<ULE>()
         );
 
         slice
     }
 
     /// Reintepret a slice of `u64`s to a slice of `Chunk<D>`. This is efficient, but relies
     /// on unsafe code.
@@ -123,15 +123,15 @@
         let n = slice.len() / (std::mem::size_of::<Self>() / std::mem::size_of::<ULE>());
 
         let ptr = slice.as_ptr() as *const _;
         let chunks: &[Chunk<D>] = unsafe { std::slice::from_raw_parts(ptr, n) };
 
         assert_eq!(
             slice.len(),
-            chunks.len() * std::mem::size_of::<Self>() / std::mem::size_of::<ULE>()
+            std::mem::size_of_val(chunks) / std::mem::size_of::<ULE>()
         );
 
         chunks
     }
 }
 
 impl<const D: usize> Hash for Chunk<D> {
```

### Comparing `hidefix-0.6.1/src/idx/dataset/any.rs` & `hidefix-0.6.2/src/idx/dataset/any.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/idx/dataset/dataset.rs` & `hidefix-0.6.2/src/idx/dataset/dataset.rs`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,16 @@
                     let mut v = Vec::with_capacity(n);
 
                     ds.chunks_visit(|ci| {
                         v.push(Chunk {
                             offset: ci
                                 .offset
                                 .iter()
-                                .zip(chunk_shape.as_slice())
-                                .map(|(o, s)| ULE::new(*o * *s))
+                                .copied()
+                                .map(ULE::new)
                                 .collect::<Vec<_>>()
                                 .as_slice()
                                 .try_into()
                                 .unwrap(),
                             size: ULE::new(ci.size),
                             addr: ULE::new(ci.addr),
                         });
```

### Comparing `hidefix-0.6.1/src/idx/dataset/mod.rs` & `hidefix-0.6.2/src/idx/dataset/mod.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/idx/dataset/types.rs` & `hidefix-0.6.2/src/idx/dataset/types.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/idx/index.rs` & `hidefix-0.6.2/src/idx/index.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/idx/mod.rs` & `hidefix-0.6.2/src/idx/mod.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/idx/serde.rs` & `hidefix-0.6.2/src/idx/serde.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/lib.rs` & `hidefix-0.6.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/python/mod.rs` & `hidefix-0.6.2/src/python/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 //! Wrappers for using hidefix in Python.
 
 use crate::filters::byteorder::ToNative;
 use byte_slice_cast::ToMutByteSlice;
-use numpy::{IntoPyArray, PyArray, PyArray1, PyArrayDyn};
+use numpy::{PyArray, PyArray1, PyArrayDyn};
 use pyo3::{
     prelude::*,
     types::{PyInt, PySlice, PyTuple},
 };
 use std::path::PathBuf;
 use std::sync::Arc;
 
@@ -99,14 +99,15 @@
             let r = ds.as_par_reader(&self.idx.path().unwrap())?;
             r.values_to_par(Some(indices), Some(counts), dst)
         })?;
 
         Ok(a.as_ref())
     }
 
+    #[cfg(off)]
     fn read_ndarray<'py, T>(
         &self,
         py: Python<'py>,
         ds: &idx::DatasetD<'_>,
         indices: &[u64],
         counts: &[u64],
     ) -> PyResult<&'py PyAny>
@@ -122,15 +123,15 @@
         let a = a.into_pyarray(py);
 
         Ok(a)
     }
 
     fn apply_fill_value_impl<'py, T>(
         &self,
-        py: Python<'py>,
+        _py: Python<'py>,
         cond: &'py PyAny,
         fv: &'py PyAny,
         arr: &'py PyAny,
     ) where
         T: Clone
             + pyo3::conversion::FromPyObject<'py>
             + numpy::Element
```

### Comparing `hidefix-0.6.1/src/reader/cache.rs` & `hidefix-0.6.2/src/reader/cache.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/reader/chunk.rs` & `hidefix-0.6.2/src/reader/chunk.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/reader/dataset.rs` & `hidefix-0.6.2/src/reader/dataset.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/reader/direct.rs` & `hidefix-0.6.2/src/reader/direct.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/src/reader/stream.rs` & `hidefix-0.6.2/src/reader/stream.rs`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                 let start = start as usize;
                 let end = end as usize;
                 debug_assert!(start <= end);
 
                 if let Some(cache) = ds_cache.get(&addr) {
                     debug_assert!(start <= cache.len());
                     debug_assert!(end <= cache.len());
-                    yield Ok((cache.slice(start..end)));
+                    yield Ok(cache.slice(start..end));
                 } else {
                     let cache = read_chunk(&mut fd, addr, sz, chunk_sz, dsz, gzip.is_some(), shuffle, true)?;
                     let cache = Bytes::from(cache);
 
                     ds_cache.put(addr, cache.clone());
 
                     debug_assert!(start <= cache.len());
@@ -142,15 +142,15 @@
                 let start = start as usize * x;
                 let end = end as usize * x;
                 debug_assert!(start <= end);
 
                 if let Some(cache) = ds_cache.get(&addr) {
                     debug_assert!(start <= cache.len());
                     debug_assert!(end <= cache.len());
-                    yield Ok((cache.slice(start..end)));
+                    yield Ok(cache.slice(start..end));
                 } else {
                     let cache = read_chunk(&mut fd, addr, sz, chunk_sz, dsz, gzip.is_some(), shuffle, true)?;
 
                     // Upcast 16-bit datatypes to 32-bit datatypes and swap to big-endian if
                     // necessary.
                     let cache = xdr::xdr(cache, dtype, order)?;
```

### Comparing `hidefix-0.6.1/tests/conftest.py` & `hidefix-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/coads_climatology.nc4` & `hidefix-0.6.2/tests/data/coads_climatology.nc4`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/chunked_fourD.h5` & `hidefix-0.6.2/tests/data/dmrpp/chunked_fourD.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/chunked_gzipped_twoD.h5` & `hidefix-0.6.2/tests/data/dmrpp/chunked_gzipped_twoD.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/chunked_oneD.h5` & `hidefix-0.6.2/tests/data/dmrpp/chunked_oneD.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/chunked_shuffled_twoD.h5` & `hidefix-0.6.2/tests/data/dmrpp/chunked_shuffled_twoD.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/chunked_shufzip_twoD.h5` & `hidefix-0.6.2/tests/data/dmrpp/chunked_shufzip_twoD.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/chunked_string_array.h5` & `hidefix-0.6.2/tests/data/dmrpp/chunked_string_array.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/chunked_threeD.h5` & `hidefix-0.6.2/tests/data/dmrpp/chunked_threeD.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/chunked_twoD.h5` & `hidefix-0.6.2/tests/data/dmrpp/chunked_twoD.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/t_float.h5` & `hidefix-0.6.2/tests/data/dmrpp/t_float.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/dmrpp/t_int_scalar.h5` & `hidefix-0.6.2/tests/data/dmrpp/t_int_scalar.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/feb.nc4` & `hidefix-0.6.2/tests/data/feb.nc4`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/data/gzip_shuffle_2d.h5` & `hidefix-0.6.2/tests/data/gzip_shuffle_2d.h5`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/python/test_slice.py` & `hidefix-0.6.2/tests/python/test_slice.py`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/python/test_xarray_large.py` & `hidefix-0.6.2/tests/python/test_xarray_large.py`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/read_dims.rs` & `hidefix-0.6.2/tests/read_dims.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/read_double.rs` & `hidefix-0.6.2/tests/read_double.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/tests/read_svim.rs` & `hidefix-0.6.2/tests/read_svim.rs`

 * *Files identical despite different names*

### Comparing `hidefix-0.6.1/PKG-INFO` & `hidefix-0.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,69 @@
 Metadata-Version: 2.1
 Name: hidefix
-Version: 0.6.1
+Version: 0.6.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: numpy
+Requires-Dist: xarray>=2023
+Requires-Dist: netCDF4
+License-File: LICENSE
 Summary: Concurrent HDF5 and NetCDF4 reader (experimental)
 Keywords: hdf,async,concurrency
 Author: Gaute Hope <eg@gaute.vetsj.com>
 Author-email: Gaute Hope <eg@gaute.vetsj.com>
 License: LGPL-3.0-or-later
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/gauteh/hidefix
 
 [![Crates.io](https://img.shields.io/crates/v/hidefix.svg)](https://crates.io/crates/hidefix)
+[![PyPI](https://img.shields.io/pypi/v/hidefix.svg)](https://pypi.org/project/hidefix/)
 [![Documentation](https://docs.rs/hidefix/badge.svg)](https://docs.rs/hidefix/)
-[![Build Status](https://github.com/gauteh/hidefix/workflows/CI/badge.svg)](https://github.com/gauteh/hidefix/actions?query=branch%3Amain)
+[![Build (rust)](https://github.com/gauteh/hidefix/workflows/Rust/badge.svg)](https://github.com/gauteh/hidefix/actions?query=branch%3Amain)
+[![Build (python)](https://github.com/gauteh/hidefix/workflows/Python/badge.svg)](https://github.com/gauteh/hidefix/actions?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/gauteh/hidefix/branch/main/graph/badge.svg)](https://codecov.io/gh/gauteh/hidefix)
 [![Rust nightly](https://img.shields.io/badge/rustc-nightly-orange)](https://rust-lang.github.io/rustup/installation/other.html)
 
 <img src="https://raw.githubusercontent.com/gauteh/hidefix/main/idefix.png">
 
 # HIDEFIX
 
-This library provides an alternative reader for the
+This Rust and Python library provides an alternative reader for the
 [HDF5](https://support.hdfgroup.org/HDF5/doc/H5.format.html) file or [NetCDF4
 file](https://www.unidata.ucar.edu/software/netcdf/docs/file_format_specifications.html)
 (which uses HDF5) which supports concurrent access to data. This is achieved by
 building an index of the chunks, allowing a thread to use many file handles to
 read the file. The original (native) HDF5 library is used to build the index,
 but once it has been created it is no longer needed. The index can be
 serialized to disk so that performing the indexing is not necessary.
 
+In Rust:
+
 ```rust
 use hidefix::prelude::*;
 
 let idx = Index::index("tests/data/coads_climatology.nc4").unwrap();
 let mut r = idx.reader("SST").unwrap();
 
 let values = r.values::<f32>(None, None).unwrap();
 
 println!("SST: {:?}", values);
 ```
 
+or with Python using Xarray:
+```python
+import xarray as xr
+import hidefix
+
+ds = xr.open_dataset('file.nc', engine='hidefix')
+print(ds)
+```
+
 ## Motivation
 
 The HDF5 library requires internal locks to be _thread-safe_ since it relies on
 internal buffers which cannot be safely accessed/written to from multiple
 threads. This effectively causes multi-threaded applications to use sequential
 reads, while competing for the locks. And also apparently cause each other
 trouble, perhaps through dropping cached chunks which other threads still need.
```

