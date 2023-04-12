| CVE_issue_number                                                           | JIRA__number  |                     Summary                                          | Affected version | 1.10.9 | 1.14.0 | CVE file      | Reproducing_command |
| :------------------------------------------------------------------------- | :----------- | :------------------------------------------------------------------- | :----------------| :----- | :----- | :--------------- | :------- |
| [GitHub Vul 11](https://github.com/magicSwordsMan/PAAFS/tree/master/vul11) | HDFFV-10722  | Invalid write in H5O_mtime_encode() | 1.10.4 | only failed | only failed | H5O_mtime_encode_invalid-write-memory-access | ./h5repack $file1 $file2 |
| [GitHub Vul 10](https://github.com/magicSwordsMan/PAAFS/tree/master/vul10) | HDFFV-10721  | Invalid read in H5S_close() | 1.10.4 | only failed | only failed | H5S_close_invalid-read-memory-access | ./h5repack $file1 $file2 |
| [GitHub Vul 9](https://github.com/magicSwordsMan/PAAFS/tree/master/vul9)   | HDFFV-10720  | Invalid write in H5F_addr_encode_len() | 1.10.4 | only failed | only failed | H5F_addr_encode_len_invalid-write-memory-access | ./h5repack $file1 $file2 |
| [CVE-2022-26061](https://nvd.nist.gov/vuln/detail/CVE-2022-26061)          | SUPPORT-1923 | A heap-based buffer overflow vulnerability exists in the gif2h5 | 1.10.4 | gif2h5 | gif2h5 | missing cve file | |
| [CVE-2022-25972](https://nvd.nist.gov/vuln/detail/CVE-2022-25972)          | SUPPORT-1923 | An out-of-bounds write vulnerability exists in the gif2h5 | 1.10.4 | gif2h5 | gif2h5 | missing cve file | |
| [CVE-2022-25942](https://nvd.nist.gov/vuln/detail/CVE-2022-25942)          | SUPPORT-1923 | An out-of-bounds read vulnerability exists in the gif2h5 | 1.10.4 | gif2h5 | gif2h5 | missing cve file | |
| CVE-2021-46244                                                             | [github #1327](https://github.com/HDFGroup/hdf5/issues/1327) | Divide By Zero in H5T__complete_copy () | 1.13.1-1 |Floating exception (core dumped)|failed with unable to open dataset | POC-GH1327 | |
| CVE-2021-46243                                                             | [github #1326](https://github.com/HDFGroup/hdf5/issues/1326) | An untrusted pointer dereference in H5O__dtype_decode_helper () | 1.13.1-1 |Segmentation fault (core dumped)| Dataset *ERROR* | POC-GH1326 | |
| CVE-2021-46242                                                             | [github #1329](https://github.com/HDFGroup/hdf5/issues/1329) | Heap-use-after free via the component H5AC_unpin_entry() | 1.13.1-1 |Segmentation fault (core dumped)| error: unable to open file | POC1-GH1329 | |
| CVE-2021-45833                                                             | [github #1313](https://github.com/HDFGroup/hdf5/issues/1313) | Stack buffer overflow in H5D__create_chunk_file_map_hyper() | 1.13.1-1 |error: unable to open file|error: unable to open file| POC3-GH1313 | |
| CVE-2021-45832                                                             | [github #1315](https://github.com/HDFGroup/hdf5/issues/1315) | Stack overflow in H5I_inc_ref() | 1.13.1-1 |OPEN|OPEN|wrong file provided, POC6-GH1315.md | |
| CVE-2021-45830                                                             | [github #1314](https://github.com/HDFGroup/hdf5/issues/1314) | Heap Buffer Overflow in H5F_addr_decode_len() | 1.13.1-1 |error: unable to open file|error: unable to open file| POC5-GH1314 | |
| CVE-2021-45829                                                             | [github #1317](https://github.com/HDFGroup/hdf5/issues/1317) | Segmentation fault via h5stat | 1.13.1-1 |error: unable to traverse|error: unable to traverse|POC8-GH1317| |
| [CVE-2020-10812](https://nvd.nist.gov/vuln/detail/CVE-2020-10812)          | [HDFFV-11052](https://jira.hdfgroup.org/browse/HDFFV-11052)  | NULL pointer dereference exists in the function H5F_get_nrefs() | 1.12.0 |Segfault|no SIGSEGV |h5_nrefs_POC||
| [CVE-2020-10811](https://nvd.nist.gov/vuln/detail/CVE-2020-10811)          | [HDFFV-11049](https://jira.hdfgroup.org/browse/HDFFV-11049)  | Heap-based buffer over-read exists in the function H5O__layout_decode() | 1.12.0 | fixed | fixed | h5dump_H5O__layout_decode_POC |./h5dump -r -d BAG_root/metadata |
| [CVE-2020-10810](https://nvd.nist.gov/vuln/detail/CVE-2020-10810)          | [HDFFV-11053](https://jira.hdfgroup.org/browse/HDFFV-11053)  | NULL pointer dereference exists in the function H5AC_unpin_entry()  | 1.13.0 |no SIGSEGV|no SIGSEGV| H5AC_unpin_entry_POC | ./h5clear -s -m |
| [CVE-2020-10809](https://nvd.nist.gov/vuln/detail/CVE-2020-10809)          | [HDFFV-11048](https://jira.hdfgroup.org/browse/HDFFV-11048)  | Heap-based buffer overflow exists in Decompress() via gif2h5 | 1.12.0 | gif2h5 | gif2h5 | gif2h5_Decompress_POC | gif2h5 |
| [CVE-2019-9152](https://github.com/magicSwordsMan/PAAFS/tree/master/vul8)  | [HDFFV-10719](https://jira.hdfgroup.org/browse/HDFFV-10719)  | Invalid read in H5MM_xstrdup() | 1.10.4 || OPEN | H5MM_xstrdup_invalid-read-memory-access |   |
| [CVE-2019-9151](https://github.com/magicSwordsMan/PAAFS/tree/master/vul7)  | [HDFFV-10718](https://jira.hdfgroup.org/browse/HDFFV-10718)  | Invalid read in H5VM_memcpyvv() | 1.10.4 | fixed | fixed | H5VM_memcpyvv_invalid-read-memory-access | h5repack file1 file2 |
| [CVE-2019-8398](https://nvd.nist.gov/vuln/detail/CVE-2019-8398)            | [HDFFV-10710](https://jira.hdfgroup.org/browse/HDFFV-10710)  | Invalid read H5T_get_size | missing ver | fixed | fixed | H5T_get_size_invalid-read-memory-access | h5repack file1 file2 |
| [CVE-2019-8397](https://nvd.nist.gov/vuln/detail/CVE-2019-8397)            | [HDFFV-10711](https://jira.hdfgroup.org/browse/HDFFV-10711)  | Out of bounds read in the function H5T_close_real()  | 1.10.4 | 0 errors | 0 errors | H5T_close_real_invalid-read-memory-access | h5repack file1 file2 |
| [CVE-2019-8396](https://nvd.nist.gov/vuln/detail/CVE-2019-8396)            | [HDFFV-10712](https://jira.hdfgroup.org/browse/HDFFV-10712)  | Invalid read in H5O__pline_decode | 1.10.4 | 16 errors from 8 contexts | 0 errors | H5O__pline_decode_invalid-read-memory-access |   |
| [CVE-2018-17439](https://nvd.nist.gov/vuln/detail/CVE-2018-17439)          | [HDFFV-10589](https://jira.hdfgroup.org/browse/HDFFV-10589)  | Stack-based buffer overflow in H5S_extent_get_dims() via h52gif | 1.10.3 | gif2h5 | gif2h5 | stackoverflow_H5S_extent_get_dims_H5S | gif2h5 |
| [CVE-2018-17438](https://nvd.nist.gov/vuln/detail/CVE-2018-17438)          | [HDFFV-10587](https://jira.hdfgroup.org/browse/HDFFV-10587)  | Incorrect protection against division by zero in H5D__select_io() | 1.8.20, 1.10.3 | gif2h5 |  1.12.0 | SIGFPE_H5D__select_io_H5Dselect |  gif2h5 |
| [CVE-2018-17437](https://nvd.nist.gov/vuln/detail/CVE-2018-17437)          | [HDFFV-10588](https://jira.hdfgroup.org/browse/HDFFV-10588)  | Memory leak in H5O_dtype_decode_helper | 1.10.3 | fixed 1.10.5 | check 1.14.0 | memleak_H5O_dtype_decode_helper_H5Odtype | h52gif |
| [CVE-2018-17436](https://nvd.nist.gov/vuln/detail/CVE-2018-17436)          | [HDFFV-10593](https://jira.hdfgroup.org/browse/HDFFV-10593)  | Invalid write memory access in decompress.c | 1.8.20, 1.10.3 | gif2h5 | gif2h5 | ReadCode_decompress_memoryAccess | gif2h5 |
| [CVE-2018-17435](https://nvd.nist.gov/vuln/detail/CVE-2018-17435)          | [HDFFV-10591](https://jira.hdfgroup.org/browse/HDFFV-10591)  | Heap-buffer-overflow was discovered in H5O_attr_decode() | 1.10.3 | fixed | fixed | Heap_Overflow_H5O_attr_decode | h52gif file image1.gif -i image |
| [CVE-2018-17434](https://nvd.nist.gov/vuln/detail/CVE-2018-17434)          | [HDFFV-10586](https://jira.hdfgroup.org/browse/HDFFV-10586)  | Divide by zero in h5repack_filters() | 1.10.3 | only fails | only fails | SIGFPE_apply_filters_h5repack_filters | h5repack -f GZIP=8 -l dset1:CHUNK=5x6 file|
| [CVE-2018-17433](https://nvd.nist.gov/vuln/detail/CVE-2018-17433)          | [HDFFV-10592](https://jira.hdfgroup.org/browse/HDFFV-10592)  | Heap overflow in ReadGifImageDesc() | 1.10.3 | gif2h5 | gif2h5 | HeapOverflow_ReadGifImageDesc | gif2h5 |
| [CVE-2018-17432](https://nvd.nist.gov/vuln/detail/CVE-2018-17432)          | [HDFFV-10590](https://jira.hdfgroup.org/browse/HDFFV-10590)  | NULL pointer dereference was discovered in H5O_sdspace_encode() | 1.10.3 | fixed | fixed | Null_Pointer_H5O_sdspace_encode | h5repack file1 file2 |
| [CVE-2018-17237](https://nvd.nist.gov/vuln/detail/CVE-2018-17237)          | [HDFFV-10571](https://jira.hdfgroup.org/browse/HDFFV-10571)  | Divide by zero in H5D__chunk_set_info_real()  | 1.10.3 | fixed | fixed | H5D__chunk_set_info_real_div_by_zero | h5dump |
| [CVE-2018-17234](https://nvd.nist.gov/vuln/detail/CVE-2018-17234)          | [HDFFV-10578](https://jira.hdfgroup.org/browse/HDFFV-10578)  | Memory Leaks in "H5O__chunk_deserialize()" | 1.10.3 | fixed | fixed | H5O__chunk_deserialize_memory_leak | h5dump |
| [CVE-2018-17233](https://nvd.nist.gov/vuln/detail/CVE-2018-17233)          | [HDFFV-10577](https://jira.hdfgroup.org/browse/HDFFV-10577)  | Divided by zero in "H5D__create_chunk_file_map_hyper()" | 1.10.3 | fixed | fixed | H5D__create_chunk_file_map_hyper_div_zero |   |
| [CVE-2018-16438](https://nvd.nist.gov/vuln/detail/CVE-2018-16438)          | no JIRA#  | Invalid read in H5L_extern_query | 1.8.20 | Segmentation fault (core dumped) | only failed | H5L_extern_query@H5Lexternal.c_498-10___out-of-bounds-read | h5dump |
| [CVE-2018-15672](https://nvd.nist.gov/vuln/detail/CVE-20)                  | [HDFFV-10556](https://jira.hdfgroup.org/browse/HDFFV-)  | Division by zero in H5D__chunk_init() | 1.10.2 | fixed | fixed | SIGPFE_Crash | h5dump |
| [CVE-2018-15671](https://github.com/SegfaultMasters/covering360/tree/master/HDF5#stack-overflow---stackoverflow_h5p__get_cb) | [HDFFV-10557](https://jira.hdfgroup.org/browse/HDFFV-10557) |Excessive stack consumption H5P__get_cb() | 1.10.2 | Infinite loop | Infinite loop | stackoverflow_H5P__get_cb | h5dump |
| [CVE-2018-14460](https://nvd.nist.gov/vuln/detail/CVE-2018-14460)          | [HDFFV-11223](https://jira.hdfgroup.org/browse/HDFFV-11223) | Buffer over-read in the function H5O_sdspace_decode() | 1.8.20 | fixed | fixed | H5O_sdspace_decode-heap-buffer-overflow | h5dump |
| [CVE-2018-14035](https://nvd.nist.gov/vuln/detail/CVE-2018-14035)          | no JIRA#     | Buffer over-read in the function H5VM_memcpyvv() | 1.8.20 | only failed | only failed | H5VM_memcpyvv-heap-buffer-overflow | h5dump |
| [CVE-2018-14034](https://nvd.nist.gov/vuln/detail/CVE-2018-14034)          | no JIRA#     | Out-of-bounds read in the function H5O_pline_reset() | 1.8.20 || missing fixed | missing cve file |   |
| [CVE-2018-14033](https://nvd.nist.gov/vuln/detail/CVE-2018-14033)          | [HDFFV-11159](https://jira.hdfgroup.org/browse/HDFFV-)  | Buffer over-read in the function H5O_layout_decode() | 1.8.20 || missing fixed | dev: PR#405 (with test) |   |
| [CVE-2018-14032](https://nvd.nist.gov/vuln/detail/CVE-2018-14032)          | no JIRA#     | Duplicate of CVE-2018-11206 | missing ver || missing fixed | missing cve file |   |
| [CVE-2018-14031](https://nvd.nist.gov/vuln/detail/CVE-2018-14031)          | no JIRA#     | Buffer over-read in the function H5T_copy | 1.8.20 || missing fixed | missing cve file |   |
| [CVE-2018-13876](https://nvd.nist.gov/vuln/detail/CVE-2018-13876)          | no JIRA#     | Buffer overflow in the function H5FD_sec2_read | 1.8.20 || missing fixed | Related to H5Dread |   |
| [CVE-2018-13875](https://nvd.nist.gov/vuln/detail/CVE-2018-13875)          | no JIRA#     | Out-of-bounds read in the function H5VM_memcpyvv | 1.8.20 || missing fixed | missing cve file |   |
| [CVE-2018-13874](https://nvd.nist.gov/vuln/detail/CVE-2018-13874)          | no JIRA#     | Buffer overflow in the function H5FD_sec2_read | 1.8.20 || missing fixed | Related to Hdmemset |   |
| [CVE-2018-13873](https://nvd.nist.gov/vuln/detail/CVE-2018-13873)          | [HDFFV-10676](https://jira.hdfgroup.org/browse/HDFFV-10676) |Buffer over-read in H5O_chunk_deserialize | 1.8.20 | only fails | only fails | H5O_chunk_deserialize-global-buffer-overflow | h5dump |
| [CVE-2018-13872](https://nvd.nist.gov/vuln/detail/CVE-2018-13872)          | no JIRA#     | Buffer overflow in the function H5G_ent_decode | 1.8.20 || missing fixed | missing cve file |   |
| [CVE-2018-13871](https://nvd.nist.gov/vuln/detail/CVE-2018-13871)          | no JIRA#     | Buffer overflow in the function H5FL_blk_malloc | 1.8.20 || missing fixed | missing cve file |   |
| [CVE-2018-13870](https://nvd.nist.gov/vuln/detail/CVE-2018-13870)          | no JIRA#     | Buffer over-read in the function H5O_link_decode | 1.8.20 || missing fixed | missing cve file |   |
| [CVE-2018-13869](https://nvd.nist.gov/vuln/detail/CVE-2018-13869)          | no JIRA#     | Memcpy parameter overlap in the function H5O_link_decode | 1.8.20 || missing fixed | missing cve file |   |
| [CVE-2018-13868](https://nvd.nist.gov/vuln/detail/CVE-2018-13868)          | [HDFFV-10548](https://jira.hdfgroup.org/browse/HDFFV-10548) | Buffer over-read in the function H5O_fill_old_decode | 1.8.20 | only fails | only fails | h5dump |
| [CVE-2018-13867](https://nvd.nist.gov/vuln/detail/CVE-2018-13867)          | no JIRA#     | Out-of-bounds read in the function H5F__accum_read | 1.8.20 | Segmentation fault (core dumped) | Assertion, Abort (core dumped) | H5F__accum_read-Out_Of_Bound_Read |   |
| [CVE-2018-13866](https://nvd.nist.gov/vuln/detail/CVE-2018-13866)          | no JIRA#     | Buffer over-read in the function H5F_addr_decode_len | 1.8.20 || missing fixed | missing cve file |   |
| [CVE-2018-11207](https://nvd.nist.gov/vuln/detail/CVE-2018-11207)          | [HDFFV-10481](https://jira.hdfgroup.org/browse/HDFFV-10481) | A division by zero was discovered in H5D__chunk_init() | 1.10.2 | fixed | fixed | DivByZero__H5D_chunk_POC | h5stat -A -T -G -D -S file |
| [CVE-2018-11206](https://nvd.nist.gov/vuln/detail/CVE-2018-11206)          | [HDFFV-10480](https://jira.hdfgroup.org/browse/HDFFV-10480) | Out-of-bounds read in H5O_fill_new_decode and H5O_fill_old_decode | 1.8.20 | fixed | fixed | H5O_fill\_[new/old]\_decode-heap-buffer-overflow | h5dump |
| [CVE-2018-11205](https://nvd.nist.gov/vuln/detail/CVE-2018-11205)          | [HDFFV-10479](https://jira.hdfgroup.org/browse/HDFFV-10479) | Out-of-bounds in H5VM_memcpyvv | 1.10.2 | Segmentation fault (core dumped) | Assertion, Abort (core dumped) | H5VM_memcpyvv-H5VM.c_1626-oob_read | h5dump |
| [CVE-2018-11204](https://nvd.nist.gov/vuln/detail/CVE-2018-11204)          | [HDFFV-10478](https://jira.hdfgroup.org/browse/HDFFV-10478) | A NULL pointer dereference in H5O__chunk_deserialize | 1.10.2 | fixed | fixed | H5O__chunk_deserialize-H5Ocache.c_1566-null_point_dereference | h5dump |
| [CVE-2018-11203](https://nvd.nist.gov/vuln/detail/CVE-2018-11203)          | [HDFFV-10477](https://jira.hdfgroup.org/browse/HDFFV-10477) | A division by zero was discovered in H5D__btree_decode_key | 1.10.2 | fixed | fixed | H5D__btree_decode_key-H5Dbtree.c_697-div_by_zero | h5dump |
| [CVE-2018-11202](https://nvd.nist.gov/vuln/detail/CVE-2018-11202)          | [HDFFV-10476](https://jira.hdfgroup.org/browse/HDFFV-10476) | A NULL pointer dereference was discovered in H5S_hyper_make_spans | 1.10.2 | Infinite loop | Assertion, Abort (core dumped) | H5S_hyper_make_spans-H5Shyper.c_6139-null_pointer_dereference | h5dump |
| [CVE-2017-17509](https://nvd.nist.gov/vuln/detail/CVE-2017-17509)          | [HDFFV-10358](https://jira.hdfgroup.org/browse/HDFFV-10358) | Out-of-bounds write vulnerability in H5G__ent_decode_vec | 1.10.1 | fixed | fixed | 5-hdf5-heap-overflow-H5G__ent_decode_vec | h5dump |
| [CVE-2017-17508](https://nvd.nist.gov/vuln/detail/CVE-2017-17508)          | [HDFFV-10357](https://jira.hdfgroup.org/browse/HDFFV-10357) | Divide-by-zero in H5T_set_loc | 1.10.1 | fixed | fixed | 1-hdf5-divbyzero-H5T_set_loc | h5dump |
| [CVE-2017-17507](https://nvd.nist.gov/vuln/detail/CVE-2017-17507)          | [HDFFV-10356](https://jira.hdfgroup.org/browse/HDFFV-10356) | Out-of-bounds read in H5T_conv_struct_opt | 1.10.1 | Dana: | Will not fix | 3-hdf5-outbound-read-H5T_conv_struct_opt |   |
| [CVE-2017-17506](https://nvd.nist.gov/vuln/detail/CVE-2017-17506)          | [HDFFV-10355](https://jira.hdfgroup.org/browse/HDFFV-10355) | Out-of-bounds read vulnerability in H5Opline_pline_decode | 1.10.1 | fixed | fixed | 4-hdf5-outbound-read-H5Opline_pline_decode | h5dump |
| [CVE-2017-17505](https://nvd.nist.gov/vuln/detail/CVE-2017-17505)          | [HDFFV-10354](https://jira.hdfgroup.org/browse/HDFFV-10354) | NULL pointer dereference in the function H5O_pline_decode | 1.10.1 | fixed | fixed | 2-hdf5-null-pointer-H5O_pline_reset.h5 | |
| [CVE-2016-4333](https://nvd.nist.gov/vuln/detail/CVE-2016-4333)            | [HDFFV-9993](https://jira.hdfgroup.org/browse/HDFFV-9993)   | Out-of-bounds access in H5O_dtype_decode_helper | 1.8.16 | fixed in | 1.8.18, 1.10.1 | missing cve file | still need test: [HDFFV-10008](https://jira.hdfgroup.org/browse/HDFFV-10008)  |
| [CVE-2016-4332](https://nvd.nist.gov/vuln/detail/CVE-2016-4332)            | [HDFFV-9950](https://jira.hdfgroup.org/browse/HDFFV-9950)   | Out-of-bounds write in H5O_msg_read_oh | 1.8.16 | fixed in | 1.8.18, 1.10.1 | missing cve file | still need test: [HDFFV-10008](https://jira.hdfgroup.org/browse/HDFFV-10008) |
| [CVE-2016-4331](https://nvd.nist.gov/vuln/detail/CVE-2016-4331)            | [HDFFV-9951](https://jira.hdfgroup.org/browse/HDFFV-9951)   | Out-of-bounds write in H5Z_nbit_decompress_one_atomic | 1.8.16 | fixed in | 1.8.18, 1.10.1 | missing cve file | still need test: [HDFFV-10008](https://jira.hdfgroup.org/browse/HDFFV-10008) |
| [CVE-2016-4330](https://nvd.nist.gov/vuln/detail/CVE-2016-4330)            | [HDFFV-9992](https://jira.hdfgroup.org/browse/HDFFV-9952)   | Out-of-bounds read in H5O_dtype_decode_helper | 1.8.16 | fixed in | 1.8.18, 1.10.1 | missing cve file | still need test: [HDFFV-10008](https://jira.hdfgroup.org/browse/HDFFV-10008) |
