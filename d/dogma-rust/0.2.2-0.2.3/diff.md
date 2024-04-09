# Comparing `tmp/dogma_rust-0.2.2.tar.gz` & `tmp/dogma_rust-0.2.3.tar.gz`

## Comparing `dogma_rust-0.2.2.tar` & `dogma_rust-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.2/Cargo.toml
--rw-r--r--   0    23269      100     3526 2024-04-03 16:48:42.000000 dogma_rust-0.2.2/.github/workflows/CI.yml
--rw-r--r--   0    23269      100      686 2024-04-03 16:48:42.000000 dogma_rust-0.2.2/.gitignore
--rw-r--r--   0    23269      100      377 2024-04-07 01:19:19.000000 dogma_rust-0.2.2/README.md
--rw-r--r--   0    23269      100     2111 2024-04-04 01:54:29.000000 dogma_rust-0.2.2/src/data.rs
--rw-r--r--   0    23269      100     3416 2024-04-07 01:04:04.000000 dogma_rust-0.2.2/src/fasta.rs
--rw-r--r--   0    23269      100     3752 2024-04-05 03:46:03.000000 dogma_rust-0.2.2/src/lib.rs
--rw-r--r--   0    23269      100     2663 2024-04-03 20:34:57.000000 dogma_rust-0.2.2/src/parallel.rs
--rw-r--r--   0    23269      100    19296 2024-04-07 01:25:41.000000 dogma_rust-0.2.2/Cargo.lock
--rw-r--r--   0    23269      100      538 2024-04-07 01:24:54.000000 dogma_rust-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 dogma_rust-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.3/Cargo.toml
+-rw-r--r--   0    23269      100     3526 2024-04-03 16:48:42.000000 dogma_rust-0.2.3/.github/workflows/CI.yml
+-rw-r--r--   0    23269      100      686 2024-04-07 01:43:02.000000 dogma_rust-0.2.3/.gitignore
+-rw-r--r--   0    23269      100      377 2024-04-07 01:19:19.000000 dogma_rust-0.2.3/README.md
+-rw-r--r--   0    23269      100     2140 2024-04-08 22:43:21.000000 dogma_rust-0.2.3/src/data.rs
+-rw-r--r--   0    23269      100     4431 2024-04-08 23:00:26.000000 dogma_rust-0.2.3/src/fasta.rs
+-rw-r--r--   0    23269      100     5871 2024-04-09 06:13:57.000000 dogma_rust-0.2.3/src/lib.rs
+-rw-r--r--   0    23269      100     2708 2024-04-07 02:48:08.000000 dogma_rust-0.2.3/src/parallel.rs
+-rw-r--r--   0    23269      100    19296 2024-04-08 23:03:02.000000 dogma_rust-0.2.3/Cargo.lock
+-rw-r--r--   0    23269      100      538 2024-04-07 01:24:54.000000 dogma_rust-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 dogma_rust-0.2.3/PKG-INFO
```

### Comparing `dogma_rust-0.2.2/.github/workflows/CI.yml` & `dogma_rust-0.2.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.2/.gitignore` & `dogma_rust-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.2/src/data.rs` & `dogma_rust-0.2.3/src/data.rs`

 * *Files 4% similar despite different names*

```diff
@@ -15,32 +15,32 @@
     pub fn new(content: impl Into<Cow<'a, [T]>>, cu_seqlens: impl Into<Cow<'a, [isize]>>) -> Self {
         AwkwardArray {
             content: content.into(),
             cu_seqlens: cu_seqlens.into(),
         }
     }
 
-    pub fn parallel_concatenate(arrs: &[AwkwardArray<'_, T>]) -> AwkwardArray<'static, T> {
-        let content_buffers = arrs.iter().map(|arr| arr.content.borrow()).collect::<Vec<_>>();
-        let cat_content = parallel_concatenate_buffers(&content_buffers);
+    pub fn parallel_concatenate(arrs: &[&AwkwardArray<'_, T>]) -> AwkwardArray<'static, T> {
+        let content_buffers = arrs.iter().copied().map(|arr| arr.content.borrow()).collect::<Vec<_>>();
+        let (cat_content, _) = parallel_concatenate_buffers(&content_buffers);
 
-        let cu_seqlen_offsets = arrs.iter().scan(0, |acc, arr| {
+        let cu_seqlen_offsets = arrs.iter().copied().scan(0, |acc, arr| {
             let start = *acc;
             *acc += arr.cu_seqlens.last().copied().unwrap_or(0);
             Some(start)
         }).collect::<Vec<_>>();
 
         let shifted_cu_seqlens = arrs.par_iter().zip(cu_seqlen_offsets).map(|(arr, offset)| {
             let mut shifted = arr.cu_seqlens.clone().into_owned();
             shifted.iter_mut().for_each(|cu_seqlen| *cu_seqlen += offset);
             shifted
         }).collect::<Vec<_>>();
         let shifted_cu_seqlens_bufs = shifted_cu_seqlens.iter().map(|cu_seqlens| cu_seqlens.borrow()).collect::<Vec<_>>();
 
-        let out_cu_seqlens = parallel_concatenate_buffers(&shifted_cu_seqlens_bufs);
+        let (out_cu_seqlens, _) = parallel_concatenate_buffers(&shifted_cu_seqlens_bufs);
 
 
         AwkwardArray::new(cat_content, out_cu_seqlens)
     }
 }
```

### Comparing `dogma_rust-0.2.2/src/fasta.rs` & `dogma_rust-0.2.3/src/fasta.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use std::fs::read;
 use rayon::prelude::*;
 use crate::data::AwkwardArray;
+use crate::parallel::parallel_concatenate_buffers;
 
 
 struct CharMapping {
     a: u8,
     t: u8,
     c: u8,
     g: u8,
@@ -20,17 +21,23 @@
             c: vec[2],
             g: vec[3],
             all_other: vec[4],
         }
     }
 }
 
-fn parse_fasta_chunk(text: &[u8], start_i: usize, end_i: usize, mapping: &CharMapping) -> AwkwardArray<'static, u8> {
+pub struct ParsedFasta {
+    pub sequences: AwkwardArray<'static, u8>,
+    pub taxon_ids: Vec<u64>,
+}
+
+fn parse_fasta_chunk(text: &[u8], start_i: usize, end_i: usize, mapping: &CharMapping) -> ParsedFasta {
     let mut out_content = vec![];
     let mut out_cu_seqlens = vec![0];
+    let mut out_taxon_ids = vec![];
     let mut i = start_i;
 
     let text_length = text.len();
     while i < text_length && unsafe { *text.get_unchecked(i) } != b'>' {
         // Move to first header
         i += 1;
     }
@@ -41,45 +48,55 @@
             b'T' | b'U' => mapping.t,
             b'C' => mapping.c,
             b'G' => mapping.g,
             _ => mapping.all_other,
         }
     };
 
+    let mut current_taxon_id: Option<u64> = None;
+
     while i < text.len() {
         let c = unsafe { *text.get_unchecked(i) };
-        
+
         if c == b'>' { // New header
             if i >= end_i { // Continue until a header shows up that has been handled by a later chunk.
                 break;
             }
+            let taxon_id_start = i + 1;
             // Maybe parse the header in the future?
             while i < text.len() && unsafe { *text.get_unchecked(i) } != b'\n' {
                 i += 1;
             }
+            let taxon_id_end = i;
+            let taxon_str = std::str::from_utf8(&text[taxon_id_start..taxon_id_end]).unwrap();
+            current_taxon_id = Some(taxon_str.parse::<u64>().unwrap());
             i += 1; // Move to next line
             continue;
         } else { // Parse one line
             while i < text_length && unsafe { *text.get_unchecked(i) } != b'\n' {
                 i += 1;
                 unsafe {
                     out_content.push(parse_char(*text.get_unchecked(i)));
                 }
             } // Ends if newline or end of file
             i += 1;
             out_cu_seqlens.push(out_content.len() as isize);
+            out_taxon_ids.push(current_taxon_id.unwrap());
         }
     }
 
-    AwkwardArray::new(out_content, out_cu_seqlens)
+    ParsedFasta {
+        sequences: AwkwardArray::new(out_content, out_cu_seqlens),
+        taxon_ids: out_taxon_ids,
+    }
     
 }
 
 
-pub(crate) fn parse_fasta(path: &str, mapping: &[u8]) -> AwkwardArray<'static, u8>{
+pub(crate) fn parse_fasta(path: &str, mapping: &[u8]) -> ParsedFasta{
     assert!(mapping.len() == 5);
 
     // Read file
     println!("Reading file");
     let data = read(path).unwrap();
 
     let mut n_threads = rayon::current_num_threads();
@@ -92,36 +109,44 @@
 
     let chunk_size = total_length.div_ceil(n_threads);
 
     let char_mapping = CharMapping::from_mapping_vector(mapping);
 
     println!("Parsing file {path} in chunks");
 
-    let chunk_results: Vec<AwkwardArray<u8>> = (0..n_threads).par_bridge().map(|i| {
+    let chunk_results: Vec<ParsedFasta> = (0..n_threads).par_bridge().map(|i| {
         let start_i = i * chunk_size;
         let end_i = std::cmp::min((i + 1) * chunk_size, total_length);
         let chunk_result = parse_fasta_chunk(&data, start_i, end_i, &char_mapping);
         chunk_result
     }).collect();
 
 
     println!("Merging result");
-    let merged_result = AwkwardArray::parallel_concatenate(&chunk_results);
+    let sequences_refs = chunk_results.iter().map(|pf| &pf.sequences).collect::<Vec<_>>();
+    let taxon_ids = chunk_results.iter().map(|pf| pf.taxon_ids.as_slice()).collect::<Vec<_>>();
+
+    let (merged_taxon_ids, _cu) = parallel_concatenate_buffers(&taxon_ids);
+    let merged_sequences = AwkwardArray::parallel_concatenate(&sequences_refs);
     drop(chunk_results);
 
-    merged_result
+    ParsedFasta {
+        sequences: merged_sequences,
+        taxon_ids: merged_taxon_ids,
+    }
 }
 
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn test_big_fasta() {
         let fasta_path = "/lfs/local/0/roed/projects/dogma-data/fasta_data/result_rep_seq.fasta";
         let result = parse_fasta(fasta_path, &[1, 2, 3, 4, 5]);
 
-        println!("Parsed fasta with {} sequences and {} tokens", result.cu_seqlens.len() - 1, result.content.len());
+        println!("Parsed fasta with {} sequences and {} tokens", result.sequences.cu_seqlens.len() - 1, result.sequences.content.len());
+        println!("Got the following taxon ids: {:?}", result.taxon_ids);
         std::hint::black_box(&result);
     }
 }
```

### Comparing `dogma_rust-0.2.2/src/lib.rs` & `dogma_rust-0.2.3/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 mod fasta;
 mod data;
 pub mod parallel;
 
+use fasta::ParsedFasta;
 use pyo3::prelude::*;
 use pyo3::types::{PyList, PyTuple};
-use numpy::{IntoPyArray, PyArray, PyArray1, PyArrayDescr, PyArrayDescrMethods, PyReadonlyArray1, PyUntypedArray, PyUntypedArrayMethods};
+use numpy::{IntoPyArray, PyArray1, PyArrayDescrMethods, PyReadonlyArray1, PyUntypedArray, PyUntypedArrayMethods};
 use crate::data::{AwkwardArray, TreatAsByteSlice};
 
 /// Formats the sum of two numbers as string.
 #[pyfunction]
 fn sum_as_string(a: usize, b: usize) -> PyResult<String> {
     Ok((a + b).to_string())
 }
 
 impl<'a, T: Clone + Sync> From<Bound<'a, PyTuple>> for AwkwardArray<'a, T> {
     fn from(value: Bound<'a, PyTuple>) -> Self {
-        let content = value.get_item(0);
+        let _content = value.get_item(0);
         todo!()
         // AwkwardArray {
 
         // }
     }
 }
 
 #[pyfunction]
-fn parse_fasta<'py>(py: Python<'py>, path: &str, mapping: PyReadonlyArray1<'py, u8>) -> PyResult<(Bound<'py, PyArray1<u8>>, Bound<'py, PyArray1<isize>>)> {
+fn parse_fasta<'py>(py: Python<'py>, path: &str, mapping: PyReadonlyArray1<'py, u8>) -> PyResult<(Bound<'py, PyArray1<u8>>, Bound<'py, PyArray1<isize>>, Bound<'py, PyArray1<u64>>)> {
     let mapping = mapping.as_slice()?;
 
-    let AwkwardArray {content, cu_seqlens} = fasta::parse_fasta(path, mapping);
+    let ParsedFasta{sequences: AwkwardArray {content, cu_seqlens}, taxon_ids} = fasta::parse_fasta(path, mapping);
 
     let content = content.into_owned().into_pyarray_bound(py);
     let cu_seqlens = cu_seqlens.into_owned().into_pyarray_bound(py);
-    Ok((content, cu_seqlens))
+    let taxon_ids = taxon_ids.into_pyarray_bound(py);
+    Ok((content, cu_seqlens, taxon_ids))
 }
 
 #[pyfunction]
 fn concatenate_awkward<'py>(py: Python<'py>, arrays: Bound<'py, PyList>) -> PyResult<(Bound<'py, PyArray1<u8>>, Bound<'py, PyArray1<isize>>)> {
     let awkwards: Vec<AwkwardArray<_>> = arrays.iter().map(|obj| {
         let tuple = obj.downcast::<PyTuple>()?;
         let tup_content = tuple.get_item(0)?;
@@ -44,22 +46,24 @@
         let cu_seqlens = tup_cu_seqlens.downcast::<PyUntypedArray>()?;
 
         let content: &[u8] = content.as_slice();
         let cu_seqlens: &[isize] = cu_seqlens.as_slice();
         Ok(AwkwardArray::<u8>::new(content, cu_seqlens))
     }).collect::<PyResult<_>>()?;
 
-    let AwkwardArray {content, cu_seqlens} = AwkwardArray::parallel_concatenate(&awkwards);
+    let awkward_refs = awkwards.iter().collect::<Vec<_>>();
+
+    let AwkwardArray {content, cu_seqlens} = AwkwardArray::parallel_concatenate(&awkward_refs);
 
     Ok((content.into_owned().into_pyarray_bound(py), cu_seqlens.into_owned().into_pyarray_bound(py)))
 }
 
 
 #[pyfunction]
-fn concatenate_numpy<'py>(py: Python<'py>, arrays: Bound<'py, PyList>) -> PyResult<Bound<'py, PyArray1<u8>>> {
+fn concatenate_numpy<'py>(py: Python<'py>, arrays: Bound<'py, PyList>) -> PyResult<(Bound<'py, PyArray1<u8>>, Bound<'py, PyArray1<usize>>)> {
     // Takes in a list of numpy arrays of the same dtype, and concatenates them into a single numpy array
     // The output array is always of dtype u8, so must be casted to the correct dtype after concatenation using `numpy.ndarray.view(dtype)`
     
     let buf_refs: Vec<_> = arrays.iter().map(|obj| -> PyResult<_> {
         let arr = obj.downcast::<PyUntypedArray>()?;
         Ok((arr.dtype(), unsafe{let arr = *arr.as_array_ptr(); arr.data}, arr.len(), arr.is_contiguous()))
     }).collect::<PyResult<_>>()?;
@@ -70,24 +74,70 @@
         return Err(pyo3::exceptions::PyValueError::new_err("All arrays must have the same dtype and be contiguous"));
     }
 
     let itemsize = first_dtype.itemsize();
 
     let slices: Vec<&[u8]> = buf_refs.iter().map(|(_dtype, ptr, len, _contiguous)| unsafe { std::slice::from_raw_parts(*ptr as *const u8, len * itemsize) }).collect();
 
-    let result: Vec<u8> = parallel::parallel_concatenate_buffers(&slices);
+    let (sequences, cu_seqlens) = parallel::parallel_concatenate_buffers(&slices);
     
-    let result_arr = result.into_pyarray_bound(py);
+    let sequences = sequences.into_pyarray_bound(py);
+    let cu_seqlens = cu_seqlens.into_pyarray_bound(py);
+
+    Ok((sequences, cu_seqlens))
+}
+
+#[pyfunction]
+fn awkward_from_list_of_numpy<'py>(py: Python<'py>, arrays: Bound<'py, PyList>) -> PyResult<Bound<'py, PyTuple>> {
+    if arrays.len() == 0 {
+        return Err(pyo3::exceptions::PyValueError::new_err("Must provide at least one array"));
+    }
+    struct ArrStorage {
+        data: *const u8,
+        len: usize,
+    }
+    unsafe impl Sync for ArrStorage {}
+
+    let mut first_dtype = None;
+    let buf_refs: Vec<_> = arrays.iter().map(|obj| -> PyResult<_> {
+        let arr = obj.downcast::<PyUntypedArray>()?;
+        let arrobj = unsafe {*arr.as_array_ptr()};
+        match &mut first_dtype {
+            None => {first_dtype = Some(arr.dtype());},
+            Some(first) => {
+                if !first.is_equiv_to(&arr.dtype()) {
+                    return Err(pyo3::exceptions::PyValueError::new_err("All arrays must have the same dtype"));
+                }
+            }
+        };
+        if !arr.is_contiguous() {
+            return Err(pyo3::exceptions::PyValueError::new_err("All arrays must be contiguous"));
+        }
+        Ok(ArrStorage{data: arrobj.data as *const u8, len: arr.len()})
+    }).collect::<PyResult<_>>()?;
+
+    let first_dtype = first_dtype.unwrap();
+
+    let itemsize: usize = first_dtype.itemsize();
+
+    let slices: Vec<&[u8]> = buf_refs.into_iter().map(|arr| unsafe { std::slice::from_raw_parts(arr.data, arr.len * itemsize) }).collect();
+
+    let (content, mut cu_seqlens) = parallel::parallel_concatenate_buffers(&slices);
+    cu_seqlens.push(content.len());  // Add the final index
+
+    let content_arr = content.into_pyarray_bound(py);
+    let cu_seqlens_arr = cu_seqlens.into_pyarray_bound(py);
 
-    Ok(result_arr)
+    Ok(PyTuple::new_bound(py, &[content_arr.to_object(py), cu_seqlens_arr.to_object(py)]))
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn dogma_rust(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(sum_as_string, m)?)?;
     m.add_function(wrap_pyfunction!(parse_fasta, m)?)?;
     m.add_function(wrap_pyfunction!(concatenate_numpy, m)?)?;
     m.add_function(wrap_pyfunction!(concatenate_awkward, m)?)?;
+    m.add_function(wrap_pyfunction!(awkward_from_list_of_numpy, m)?)?;
     // m.add_function
     Ok(())
 }
```

### Comparing `dogma_rust-0.2.2/src/parallel.rs` & `dogma_rust-0.2.3/src/parallel.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 use rayon::prelude::*;
 
 struct SendPtr<T>(*mut T);
 
 // unsafe impl<T> Send for SendPtr<T> {}
 unsafe impl<T> Sync for SendPtr<T> {}
 
-pub fn parallel_concatenate_buffers<T: Sync>(bufs: &[&[T]]) -> Vec<T> {
-    let out_buf_size = bufs.iter().map(|buf| buf.len()).sum();
+pub fn parallel_concatenate_buffers<T: Sync>(bufs: &[&[T]]) -> (Vec<T>, Vec<usize>) {
+    let out_buf_size = bufs.iter().map(|&buf| buf.len()).sum();
 
     let mut out_buf = Vec::with_capacity(out_buf_size);
     unsafe {out_buf.set_len(out_buf_size);}
     let data = SendPtr(out_buf.as_mut_ptr());
 
     let starting_indices = bufs.iter().scan(0, |acc, buf| {
         let start = *acc;
@@ -26,15 +26,15 @@
             let dest_base: *mut T = send_dest.0;
             let dest: *mut T = dest_base.add(start);
             let src = buf_ptr;
             std::ptr::copy_nonoverlapping(src, dest, buf_len);
         }
     });
     
-    out_buf
+    (out_buf, starting_indices)
 }
 
 
 
 #[cfg(test)]
 mod tests {
     use std::hint::black_box;
@@ -43,15 +43,15 @@
     use rand::prelude::*;
 
     #[test]
     fn test_parallel_concatenate_buffers() {
         let bufs = (0..10_000).into_par_iter().map(|_| (0..1_000).map(|_| random::<u8>()).collect::<Vec<_>>()).collect::<Vec<_>>();
         let ref_bufs = bufs.iter().map(|buf| buf.as_slice()).collect::<Vec<_>>();
         eprintln!("Starting test");
-        let out_buf = parallel_concatenate_buffers(&ref_bufs);
+        let (out_buf, _) = parallel_concatenate_buffers(&ref_bufs);
         eprintln!("Finished test");
         let flattened = bufs.iter().flatten().copied().collect::<Vec<_>>();
         assert_eq!(out_buf, flattened);
     }
 
     #[test]
     fn test_run_parallel_flatten() {
@@ -60,15 +60,15 @@
         let ref_bufs = bufs.iter().map(|buf| buf.as_slice()).collect::<Vec<_>>();
 
         eprintln!("starting seq");
         // let seq_flat_buf: Vec<u8> = ref_bufs.iter().map(|&inner| inner.iter()).flatten().copied().collect();
         eprintln!("starting par");
         let par_flat_buf: Vec<u8> = ref_bufs.par_iter().map(|&inner| inner).flatten().copied().collect();
         eprintln!("starting par efficient");
-        let par_efficient_buf = parallel_concatenate_buffers(&ref_bufs);
+        let (par_efficient_buf, _) = parallel_concatenate_buffers(&ref_bufs);
         eprintln!("finished");
 
         // Feed these to black box to stop them from being optimized away
         black_box(&par_flat_buf);
         black_box(&par_efficient_buf);
```

### Comparing `dogma_rust-0.2.2/Cargo.lock` & `dogma_rust-0.2.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -96,15 +96,15 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "dogma-rust"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "anyhow",
  "chrono",
  "eyre",
  "num-bigint",
  "numpy",
  "pyo3",
@@ -126,17 +126,17 @@
 dependencies = [
  "indenter",
  "once_cell",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
```

### Comparing `dogma_rust-0.2.2/pyproject.toml` & `dogma_rust-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.2/PKG-INFO` & `dogma_rust-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dogma_rust
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/marcelroed/dogma-data
 Project-URL: repository, https://github.com/marcelroed/dogma-data
```

