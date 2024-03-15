
## 2to3

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 28.07% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.54% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.30% | `python` | `gc_collect_main` | gc |
| 2.24% | `python` | `type_new` | memory |
| 2.16% | `python` | `deduce_unreachable` | unknown |
| 2.13% | `python` | `PyObject_GetAttr` | dynamic |
| 1.98% | `python` | `visit_decref` | gc |
| 1.85% | `python` | `tupledealloc` | memory |
| 1.60% | `python` | `sre_ucs1_match` | library |
| 1.49% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.12% | `python` | `visit_reachable` | gc |
| 1.10% | `python` | `_PyCode_New` | memory |
| 1.05% | `python` | `PyDict_GetItemRef` | dict |
| 0.83% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.82% | `python` | `_PyPegen_fill_token` | interpreter |
| 0.81% | `python` | `r_object` | import |
| 0.78% | `python` | `list_dealloc` | memory |
| 0.78% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.68% | `python` | `gen_dealloc` | memory |
| 0.65% | `python` | `PyObject_SetAttr` | dynamic |
| 0.65% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.64% | `python` | `siphash13` | str |
| 0.63% | `python` | `PyUnicode_FromKindAndData` | str |
| 0.62% | `python` | `dict_dealloc` | memory |
| 0.61% | `python` | `subtype_traverse` | gc |
| 0.59% | `python` | `make_gen` | unknown |
| 0.53% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 0.51% | `python` | `PyObject_GC_Del` | gc |

## aiohttp

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 28.12% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.63% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.18% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.61% | `python` | `tupledealloc` | memory |
| 1.45% | `python` | `type_new` | memory |
| 1.16% | `python` | `gc_collect_main` | gc |
| 1.11% | `python` | `deduce_unreachable` | unknown |
| 1.05% | `python` | `visit_decref` | gc |
| 0.88% | `python` | `PyObject_GetAttr` | dynamic |
| 0.82% | `python` | `subtype_dealloc` | memory |
| 0.81% | `python` | `PyDict_GetItemRef` | dict |
| 0.77% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.74% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.70% | `python` | `visit_reachable` | gc |
| 0.70% | `python` | `unicode_dealloc` | memory |
| 0.67% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.65% | `python` | `dict_dealloc` | memory |
| 0.62% | `python` | `_PyCode_New` | memory |
| 0.59% | `python` | `list_dealloc` | memory |
| 0.58% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.58% | `python` | `sre_ucs1_match` | library |
| 0.56% | `python` | `find_name_in_mro` | lookup |
| 0.56% | `python` | `r_object` | import |
| 0.55% | `python` | `siphash13` | str |
| 0.54% | `python` | `_PySuper_Lookup` | dynamic |
| 0.52% | `python` | `PyObject_GC_Del` | gc |

## async_generators

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 20.78% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 10.25% | `python` | `_PyErr_SetObject` | exceptions |
| 4.64% | `python` | `StopIteration_dealloc` | memory |
| 3.95% | `python` | `BaseException_new` | memory |
| 3.42% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 2.53% | `python` | `StopIteration_init` | dynamic |
| 2.45% | `python` | `async_gen_asend_send` | unknown |
| 2.38% | `python` | `gen_send_ex` | unknown |
| 2.05% | `python` | `tupledealloc` | memory |
| 1.80% | `python` | `_PyEval_EvalFrameDefault.cold` | interpreter |
| 1.78% | `python` | `gen_send_ex2` | unknown |
| 1.77% | `python` | `PyErr_GivenExceptionMatches` | exceptions |
| 1.64% | `python` | `PyErr_ExceptionMatches` | exceptions |
| 1.57% | `python` | `async_gen_asend_dealloc` | memory |
| 1.49% | `python` | `async_gen_wrapped_val_dealloc` | memory |
| 1.42% | `python` | `async_gen_asend_new` | memory |
| 1.41% | `python` | `_PyAsyncGenValueWrapperNew` | memory |
| 1.34% | `python` | `_Py_NewReference` | memory |
| 1.32% | `python` | `async_gen_unwrap_value.isra.0` | unknown |
| 1.29% | `python` | `gc_collect_main` | gc |
| 1.25% | `python` | `deduce_unreachable` | unknown |
| 1.20% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.08% | `python` | `long_add` | int |
| 1.02% | `python` | `_PyGen_FetchStopIterationValue.cold` | unknown |
| 0.88% | `python` | `visit_decref` | gc |
| 0.87% | `python` | `type_call` | dynamic |
| 0.87% | `python` | `visit_reachable` | gc |
| 0.84% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.79% | `python` | `subtype_traverse` | gc |
| 0.75% | `python` | `_PyGen_SetStopIterationValue` | unknown |
| 0.69% | `python` | `PyObject_CallFinalizerFromDealloc` | memory |
| 0.64% | `python` | `long_dealloc` | memory |
| 0.59% | `python` | `_Py_Dealloc` | memory |
| 0.59% | `python` | `range_subscript` | unknown |
| 0.57% | `python` | `PyType_GenericAlloc` | memory |
| 0.55% | `python` | `subtype_dealloc` | memory |

## async_tree

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.11% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 14.38% | `python` | `gc_collect_main` | gc |
| 8.05% | `python` | `deduce_unreachable` | unknown |
| 6.23% | `python` | `visit_decref` | gc |
| 6.19% | `python` | `visit_reachable` | gc |
| 1.73% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.53% | `python` | `subtype_traverse` | gc |
| 1.28% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.10% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.95% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.93% | `python` | `tupledealloc` | memory |
| 0.91% | `python` | `PyObject_GetAttr` | dynamic |
| 0.86% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.85% | `python` | `PyObject_GC_Del` | gc |
| 0.83% | `python` | `_PyObject_GC_New` | gc |
| 0.78% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.75% | `python` | `insertdict` | dict |
| 0.74% | `python` | `gen_traverse` | gc |
| 0.71% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.70% | `python` | `slot_tp_init` | unknown |
| 0.67% | `python` | `meth_dealloc` | memory |
| 0.64% | `python` | `context_tp_dealloc` | memory |
| 0.56% | `python` | `subtype_dealloc` | memory |
| 0.53% | `python` | `list_dealloc` | memory |
| 0.52% | `python` | `gen_dealloc` | memory |
| 0.51% | `python` | `PyDict_GetItemRef` | dict |

## async_tree_cpu_io_mixed

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.29% | `python` | `k_mul` | int |
| 16.78% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 11.05% | `python` | `gc_collect_main` | gc |
| 6.42% | `python` | `deduce_unreachable` | unknown |
| 5.05% | `python` | `visit_decref` | gc |
| 4.86% | `python` | `visit_reachable` | gc |
| 2.35% | `python` | `long_dealloc` | memory |
| 1.31% | `python` | `subtype_traverse` | gc |
| 1.25% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.14% | `python` | `_PyLong_New` | memory |
| 0.95% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.90% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.74% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.69% | `python` | `PyObject_GetAttr` | dynamic |
| 0.64% | `python` | `tupledealloc` | memory |
| 0.59% | `math.cpython-313-x86_64-linux-gnu.so` | `factorial_partial_product` | library |
| 0.55% | `python` | `long_mul` | int |
| 0.55% | `python` | `gen_traverse` | gc |
| 0.55% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.54% | `python` | `PyObject_GC_Del` | gc |
| 0.51% | `python` | `_PyObject_GC_New` | gc |
| 0.51% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |

## async_tree_cpu_io_mixed_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.08% | `python` | `k_mul` | int |
| 14.94% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 12.74% | `python` | `gc_collect_main` | gc |
| 7.99% | `python` | `deduce_unreachable` | unknown |
| 5.36% | `python` | `visit_decref` | gc |
| 5.29% | `python` | `visit_reachable` | gc |
| 2.32% | `python` | `long_dealloc` | memory |
| 1.43% | `python` | `subtype_traverse` | gc |
| 1.12% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.09% | `python` | `_PyLong_New` | memory |
| 0.98% | `python` | `gen_traverse` | gc |
| 0.93% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.80% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.79% | `python` | `PyObject_GetAttr` | dynamic |
| 0.71% | `python` | `set_traverse` | gc |
| 0.68% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.61% | `math.cpython-313-x86_64-linux-gnu.so` | `factorial_partial_product` | library |
| 0.58% | `python` | `long_mul` | int |
| 0.54% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.52% | `python` | `tupledealloc` | memory |

## async_tree_io

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.68% | `python` | `gc_collect_main` | gc |
| 18.38% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 10.96% | `python` | `deduce_unreachable` | unknown |
| 8.22% | `python` | `visit_reachable` | gc |
| 7.72% | `python` | `visit_decref` | gc |
| 1.69% | `python` | `subtype_traverse` | gc |
| 1.42% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.36% | `python` | `gen_traverse` | gc |
| 0.81% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.81% | `python` | `slot_tp_richcompare` | dynamic |
| 0.62% | `python` | `tupledealloc` | memory |
| 0.61% | `python` | `PyObject_GetAttr` | dynamic |
| 0.61% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.60% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.58% | `_heapq.cpython-313-x86_64-linux-gnu.so` | `_heapq_heappop` | library |
| 0.57% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.51% | `python` | `PyObject_GC_Del` | gc |
| 0.50% | `python` | `slot_tp_init` | unknown |

## async_tree_io_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 22.63% | `python` | `gc_collect_main` | gc |
| 16.77% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 12.24% | `python` | `deduce_unreachable` | unknown |
| 8.33% | `python` | `visit_reachable` | gc |
| 7.97% | `python` | `visit_decref` | gc |
| 1.79% | `python` | `gen_traverse` | gc |
| 1.77% | `python` | `subtype_traverse` | gc |
| 1.32% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.87% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.83% | `python` | `slot_tp_richcompare` | dynamic |
| 0.70% | `python` | `set_traverse` | gc |
| 0.67% | `python` | `PyObject_GetAttr` | dynamic |
| 0.64% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.57% | `python` | `tupledealloc` | memory |
| 0.57% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.54% | `_heapq.cpython-313-x86_64-linux-gnu.so` | `_heapq_heappop` | library |
| 0.51% | `python` | `PyObject_VectorcallMethod` | dynamic |

## async_tree_memoization

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.96% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 15.04% | `python` | `gc_collect_main` | gc |
| 8.70% | `python` | `deduce_unreachable` | unknown |
| 6.79% | `python` | `visit_decref` | gc |
| 6.58% | `python` | `visit_reachable` | gc |
| 1.74% | `python` | `subtype_traverse` | gc |
| 1.72% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.20% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.95% | `python` | `PyObject_GetAttr` | dynamic |
| 0.88% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.81% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.80% | `python` | `gen_traverse` | gc |
| 0.80% | `python` | `tupledealloc` | memory |
| 0.70% | `python` | `_PyObject_GC_New` | gc |
| 0.69% | `python` | `meth_dealloc` | memory |
| 0.69% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.68% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.65% | `python` | `PyObject_GC_Del` | gc |
| 0.63% | `python` | `context_tp_dealloc` | memory |
| 0.62% | `python` | `slot_tp_init` | unknown |
| 0.61% | `python` | `insertdict` | dict |
| 0.58% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.52% | `python` | `gen_dealloc` | memory |

## async_tree_memoization_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 19.40% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 16.88% | `python` | `gc_collect_main` | gc |
| 10.95% | `python` | `deduce_unreachable` | unknown |
| 7.17% | `python` | `visit_decref` | gc |
| 7.05% | `python` | `visit_reachable` | gc |
| 1.86% | `python` | `subtype_traverse` | gc |
| 1.53% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.35% | `python` | `gen_traverse` | gc |
| 1.09% | `python` | `PyObject_GetAttr` | dynamic |
| 0.99% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.98% | `python` | `set_traverse` | gc |
| 0.88% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.86% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.72% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.71% | `python` | `tupledealloc` | memory |
| 0.62% | `python` | `meth_dealloc` | memory |
| 0.58% | `python` | `PyObject_GC_Del` | gc |
| 0.56% | `python` | `slot_tp_init` | unknown |
| 0.55% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.54% | `python` | `make_gen` | unknown |
| 0.53% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.51% | `python` | `PyDict_GetItemRef` | dict |

## async_tree_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 18.98% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 16.45% | `python` | `gc_collect_main` | gc |
| 10.06% | `python` | `deduce_unreachable` | unknown |
| 6.75% | `python` | `visit_decref` | gc |
| 6.65% | `python` | `visit_reachable` | gc |
| 1.67% | `python` | `subtype_traverse` | gc |
| 1.54% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.25% | `python` | `gen_traverse` | gc |
| 1.15% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.08% | `python` | `PyObject_GetAttr` | dynamic |
| 1.01% | `python` | `set_traverse` | gc |
| 0.97% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.93% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.77% | `python` | `PyObject_GC_Del` | gc |
| 0.75% | `python` | `tupledealloc` | memory |
| 0.73% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.66% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.63% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.62% | `python` | `slot_tp_init` | unknown |
| 0.60% | `python` | `make_gen` | unknown |
| 0.57% | `python` | `PyDict_GetItemRef` | dict |
| 0.56% | `python` | `meth_dealloc` | memory |
| 0.54% | `python` | `_PyObject_GC_New` | gc |
| 0.53% | `python` | `subtype_dealloc` | memory |

## asyncio_tcp

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.94% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 16.72% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 9.21% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.20% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.59% | `[kernel.kallsyms]` | `tcp_sendmsg_locked` | kernel |

## asyncio_tcp_ssl

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 40.66% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 25.71% | `libcrypto.so.1.1` | `CRYPTO_secure_actual_size` | libc |
| 10.45% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 3.60% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.90% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.87% | `libssl.so.1.1` | `SSL_rstate_string` | library |
| 0.60% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |

## asyncio_websockets

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 64.28% | `libz.so.1.2.11` | `crc32_combine64` | library |
| 20.37% | `libz.so.1.2.11` | `inflateBackEnd` | library |
| 2.87% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.86% | `python` | `_PyEval_EvalFrameDefault` | interpreter |

## chameleon

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 39.71% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.47% | `python` | `long_to_decimal_string_internal` | int |
| 2.62% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.37% | `python` | `sre_ucs2_charset.isra.0` | library |
| 2.28% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.18% | `python` | `PyUnicode_Format` | str |
| 1.96% | `python` | `_PyUnicode_JoinArray` | str |
| 1.76% | `python` | `type_new` | memory |
| 1.64% | `python` | `dict_get` | dict |
| 1.39% | `python` | `insertdict` | dict |
| 1.38% | `python` | `unicode_dealloc` | memory |
| 1.02% | `python` | `list_append` | list |
| 1.00% | `python` | `gc_collect_main` | gc |
| 0.93% | `python` | `visit_decref` | gc |
| 0.89% | `python` | `deduce_unreachable` | unknown |
| 0.87% | `python` | `state_init` | unknown |
| 0.87% | `python` | `PyUnicode_Concat` | str |
| 0.86% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 0.85% | `python` | `list_dealloc` | memory |
| 0.73% | `python` | `PyObject_Str` | dynamic |
| 0.73% | `python` | `_PyCode_New` | memory |
| 0.67% | `python` | `visit_reachable` | gc |
| 0.65% | `python` | `r_object` | import |
| 0.65% | `python` | `tupledealloc` | memory |
| 0.65% | `libc-2.31.so` | `malloc` | libc |
| 0.59% | `python` | `sre_search` | library |
| 0.54% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.54% | `python` | `dict_setdefault_ref_lock_held` | dict |

## chaos

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 49.24% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.68% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.03% | `python` | `subtype_dealloc` | memory |
| 2.00% | `python` | `_PyLong_Subtract` | int |
| 1.61% | `python` | `PyFloat_FromDouble` | float |
| 1.45% | `python` | `float_div` | float |
| 1.39% | `python` | `convert_to_double` | unknown |
| 1.33% | `python` | `_PyLong_Add` | int |
| 1.28% | `python` | `range_vectorcall` | unknown |
| 1.10% | `python` | `PyType_GenericAlloc` | memory |
| 1.08% | `python` | `PyNumber_Subtract` | dynamic |
| 1.07% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.03% | `python` | `type_new` | memory |
| 0.95% | `python` | `range_iter` | unknown |
| 0.91% | `libm-2.31.so` | `f64xsubf128` | library |
| 0.84% | `python` | `PyNumber_TrueDivide` | dynamic |
| 0.79% | `python` | `float_richcompare` | float |
| 0.69% | `python` | `PyObject_Free` | dynamic |
| 0.68% | `python` | `float_pow` | float |
| 0.68% | `python` | `visit_decref` | gc |
| 0.68% | `python` | `tupledealloc` | memory |
| 0.67% | `python` | `gc_collect_main` | gc |
| 0.64% | `python` | `float_dealloc` | memory |
| 0.64% | `python` | `deduce_unreachable` | unknown |
| 0.64% | `python` | `PyLong_FromLong` | int |
| 0.63% | `python` | `_PyObject_InitInlineValues` | dynamic |
| 0.59% | `python` | `PyObject_GC_Del` | gc |
| 0.59% | `python` | `float_sub` | float |
| 0.54% | `python` | `range_dealloc` | memory |
| 0.51% | `python` | `PyType_IsSubtype` | dynamic |
| 0.50% | `python` | `PyObject_RichCompare` | dynamic |

## comprehensions

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 43.06% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.21% | `python` | `dict_get` | dict |
| 2.46% | `python` | `list_resize` | list |
| 2.14% | `python` | `PyFunction_NewWithQualName` | memory |
| 2.01% | `python` | `list_dealloc` | memory |
| 1.98% | `python` | `PyDict_GetItemRef` | dict |
| 1.74% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.70% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.67% | `python` | `list_iter` | list |
| 1.52% | `python` | `insertdict` | dict |
| 1.52% | `python` | `unsafe_tuple_compare` | unknown |
| 1.48% | `python` | `gen_dealloc` | memory |
| 1.23% | `python` | `type_new` | memory |
| 1.19% | `python` | `func_dealloc` | memory |
| 1.00% | `python` | `PyObject_GC_Del` | gc |
| 1.00% | `python` | `tupledealloc` | memory |
| 0.99% | `python` | `listiter_dealloc` | memory |
| 0.95% | `python` | `long_hash` | int |
| 0.90% | `python` | `long_richcompare` | int |
| 0.88% | `python` | `PyObject_RichCompare` | dynamic |
| 0.87% | `python` | `make_gen` | unknown |
| 0.73% | `python` | `gc_collect_main` | gc |
| 0.68% | `python` | `deduce_unreachable` | unknown |
| 0.67% | `python` | `_Py_type_getattro` | lookup |
| 0.64% | `python` | `visit_decref` | gc |
| 0.57% | `python` | `_PyObject_Malloc` | memory |
| 0.55% | `python` | `dictresize` | dict |
| 0.54% | `python` | `list_sort_impl` | list |
| 0.51% | `python` | `PyObject_GetAttr` | dynamic |

## concurrent_imap

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.81% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.06% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.89% | `python` | `subtype_dealloc` | memory |
| 1.70% | `[kernel.kallsyms]` | `perf_event_alloc` | kernel |
| 1.67% | `python` | `PyObject_GetAttr` | dynamic |
| 1.52% | `[kernel.kallsyms]` | `memset_erms` | kernel |
| 1.24% | `python` | `tupledealloc` | memory |
| 1.01% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.99% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.93% | `python` | `PyObject_GC_Del` | gc |
| 0.83% | `[kernel.kallsyms]` | `mutex_lock` | kernel |
| 0.77% | `[kernel.kallsyms]` | `mutex_unlock` | kernel |
| 0.68% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.67% | `[kernel.kallsyms]` | `kfree` | kernel |
| 0.65% | `[kernel.kallsyms]` | `page_counter_cancel` | kernel |
| 0.62% | `[kernel.kallsyms]` | `inherit_event.isra.0` | kernel |
| 0.59% | `python` | `_PySuper_Lookup` | dynamic |
| 0.56% | `[kernel.kallsyms]` | `_raw_spin_lock` | kernel |
| 0.56% | `[kernel.kallsyms]` | `_raw_spin_lock_irqsave` | kernel |
| 0.52% | `python` | `list_dealloc` | memory |

## coroutines

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 39.79% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 13.65% | `python` | `gen_dealloc` | memory |
| 10.22% | `python` | `make_gen` | unknown |
| 6.87% | `python` | `_PyEval_EvalFrameDefault.cold` | interpreter |
| 5.14% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.51% | `python` | `_PyLong_Subtract` | int |
| 2.50% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.17% | `python` | `_PyFrame_ClearExceptCode` | interpreter |
| 1.56% | `python` | `_PyLong_Add` | int |
| 1.08% | `python` | `_PyCoro_GetAwaitableIter` | unknown |
| 0.77% | `python` | `type_new` | memory |
| 0.53% | `python` | `gc_collect_main` | gc |
| 0.52% | `python` | `_PyGen_yf` | unknown |

## coverage

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 20.05% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.37% | `tracer.cpython-313-x86_64-linux-gnu.so` | `CTracer_trace` | library |
| 4.87% | `python` | `call_instrumentation_vector` | unknown |
| 4.11% | `python` | `PyObject_SetAttrString` | dynamic |
| 4.01% | `python` | `unicode_decode_utf8` | str |
| 3.34% | `python` | `siphash13` | str |
| 3.18% | `python` | `_Py_dict_lookup` | lookup |
| 2.65% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 2.58% | `python` | `PyLong_FromLong` | int |
| 2.55% | `python` | `call_one_instrument` | unknown |
| 2.46% | `python` | `frame_dealloc` | memory |
| 2.36% | `python` | `PySet_Add` | unknown |
| 2.00% | `python` | `_PyObject_VectorcallTstate.lto_priv.5` | dynamic |
| 1.97% | `python` | `_PyUnicode_InternInPlace` | str |
| 1.65% | `python` | `PyObject_SetAttr` | dynamic |
| 1.61% | `python` | `dict_getitem` | dict |
| 1.54% | `python` | `_PyFrame_MakeAndSetFrameObject` | unknown |
| 1.47% | `python` | `unicode_dealloc` | memory |
| 1.47% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.13% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.08% | `python` | `call_trace_func.isra.0` | unknown |
| 0.99% | `python` | `type_new` | memory |
| 0.90% | `python` | `_Py_call_instrumentation_jump` | unknown |
| 0.79% | `python` | `_PyCode_GetCode` | unknown |
| 0.67% | `python` | `gc_collect_main` | gc |
| 0.65% | `python` | `_Py_call_instrumentation_arg` | unknown |
| 0.64% | `python` | `deduce_unreachable` | unknown |
| 0.59% | `python` | `PyEval_GetFrame` | interpreter |
| 0.58% | `python` | `PyFrame_GetCode` | exceptions |
| 0.57% | `python` | `visit_decref` | gc |
| 0.55% | `python` | `_PyLong_Add` | int |
| 0.53% | `python` | `_PyLong_Subtract` | int |

## crypto_pyaes

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 36.48% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.14% | `python` | `long_dealloc` | memory |
| 7.41% | `python` | `long_bitwise` | int |
| 4.32% | `python` | `long_rshift` | int |
| 3.66% | `python` | `long_mod` | int |
| 3.34% | `python` | `long_and` | int |
| 2.85% | `python` | `_PyLong_New` | memory |
| 1.47% | `python` | `binary_op` | unknown |
| 1.26% | `python` | `PyObject_Free` | dynamic |
| 1.21% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.20% | `python` | `_PyObject_Malloc` | memory |
| 1.17% | `python` | `PyNumber_And` | dynamic |
| 1.13% | `python` | `_PyLong_Add` | int |
| 1.03% | `python` | `list_dealloc` | memory |
| 0.90% | `python` | `type_new` | memory |
| 0.83% | `python` | `PyNumber_Rshift` | dynamic |
| 0.82% | `python` | `long_xor` | int |
| 0.73% | `python` | `PyNumber_Remainder` | dynamic |
| 0.70% | `python` | `range_vectorcall` | unknown |
| 0.64% | `python` | `gc_collect_main` | gc |
| 0.58% | `python` | `deduce_unreachable` | unknown |
| 0.57% | `python` | `visit_decref` | gc |
| 0.51% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.51% | `python` | `range_iter` | unknown |

## dask

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 34.04% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.46% | `python` | `gc_collect_main` | gc |
| 2.41% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.23% | `python` | `visit_decref` | gc |
| 2.15% | `python` | `deduce_unreachable` | unknown |
| 1.93% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.68% | `python` | `tupledealloc` | memory |
| 1.63% | `python` | `visit_reachable` | gc |
| 1.05% | `python` | `PyDict_GetItemRef` | dict |
| 1.02% | `python` | `object_isinstance` | dynamic |
| 0.89% | `python` | `dict_dealloc` | memory |
| 0.82% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.82% | `python` | `PyBytes_Repr` | str |
| 0.76% | `python` | `long_dealloc` | memory |
| 0.72% | `python` | `type_new` | memory |
| 0.58% | `python` | `insertdict` | dict |
| 0.57% | `python` | `PyObject_GetAttr` | dynamic |
| 0.54% | `python` | `PyObject_Free` | dynamic |
| 0.52% | `python` | `list_dealloc` | memory |
| 0.52% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.52% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.51% | `python` | `_PyObject_GC_New` | gc |

## deepcopy

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 46.74% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.86% | `python` | `dict_get` | dict |
| 4.41% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.52% | `python` | `long_dealloc` | memory |
| 2.34% | `python` | `_PyLong_New` | memory |
| 1.76% | `python` | `insertdict` | dict |
| 1.34% | `python` | `long_hash` | int |
| 1.33% | `python` | `PyDict_GetItemRef` | dict |
| 1.33% | `python` | `PySys_Audit` | unknown |
| 1.20% | `python` | `builtin_id` | unknown |
| 1.07% | `python` | `insert_to_emptydict` | dict |
| 1.06% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.93% | `python` | `tupledealloc` | memory |
| 0.82% | `python` | `PyObject_GetAttr` | dynamic |
| 0.79% | `python` | `list_dealloc` | memory |
| 0.79% | `python` | `dict_dealloc` | memory |
| 0.73% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.69% | `python` | `list_append` | list |
| 0.64% | `python` | `type_new` | memory |
| 0.59% | `python` | `dictiter_iternextitem` | dict |
| 0.53% | `python` | `long_richcompare` | int |

## deltablue

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 56.43% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.14% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.04% | `python` | `_PyObject_GetMethod` | dynamic |
| 1.49% | `python` | `gc_collect_main` | gc |
| 1.38% | `python` | `deduce_unreachable` | unknown |
| 1.27% | `python` | `visit_decref` | gc |
| 1.17% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.14% | `python` | `type_new` | memory |
| 1.07% | `python` | `_PySuper_Lookup` | dynamic |
| 0.79% | `python` | `PyObject_GetAttr` | dynamic |
| 0.78% | `python` | `visit_reachable` | gc |
| 0.76% | `python` | `_Py_type_getattro` | lookup |
| 0.74% | `python` | `subtype_traverse` | gc |
| 0.70% | `python` | `method_dealloc` | memory |
| 0.61% | `python` | `PyObject_GC_Del` | gc |
| 0.56% | `python` | `cm_descr_get` | unknown |
| 0.55% | `python` | `_PyCode_New` | memory |

## django_template

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 35.61% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.07% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.19% | `python` | `type_new` | memory |
| 1.96% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.66% | `python` | `object_isinstance` | dynamic |
| 1.34% | `python` | `gc_collect_main` | gc |
| 1.34% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.29% | `python` | `PyObject_GC_Del` | gc |
| 1.23% | `python` | `deduce_unreachable` | unknown |
| 1.21% | `python` | `tupledealloc` | memory |
| 1.21% | `python` | `insertdict` | dict |
| 1.13% | `python` | `visit_decref` | gc |
| 0.98% | `python` | `_PyCode_New` | memory |
| 0.94% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.87% | `python` | `PyDict_GetItemRef` | dict |
| 0.86% | `python` | `visit_reachable` | gc |
| 0.83% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.82% | `python` | `list_dealloc` | memory |
| 0.73% | `python` | `r_object` | import |
| 0.71% | `python` | `unicode_replace` | str |
| 0.70% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.64% | `python` | `dict_dealloc` | memory |
| 0.64% | `python` | `long_to_decimal_string_internal` | int |
| 0.57% | `python` | `_PyObject_GenericGetAttrWithDict` | dynamic |
| 0.55% | `python` | `builtin_hasattr` | unknown |
| 0.55% | `python` | `PyUnicode_FromKindAndData` | str |
| 0.53% | `python` | `unicode_dealloc` | memory |
| 0.53% | `python` | `_PyObject_GC_New` | gc |
| 0.53% | `python` | `PyType_GenericAlloc` | memory |
| 0.53% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |

## djangocms

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 19.69% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.56% | `python` | `find_name_in_mro` | lookup |
| 2.80% | `python` | `type_new` | memory |
| 2.45% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.38% | `python` | `gc_collect_main` | gc |
| 2.07% | `python` | `deduce_unreachable` | unknown |
| 1.82% | `python` | `visit_decref` | gc |
| 1.59% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.51% | `libsqlite3.so.0.8.6` | `sqlite3_exec` | library |
| 1.41% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.30% | `python` | `visit_reachable` | gc |
| 1.17% | `python` | `tupledealloc` | memory |
| 1.14% | `python` | `PyObject_GetAttr` | dynamic |
| 1.04% | `python` | `PyDict_GetItemRef` | dict |
| 0.91% | `python` | `sre_ucs1_match` | library |
| 0.80% | `python` | `dict_traverse` | gc |
| 0.76% | `python` | `dict_dealloc` | memory |
| 0.70% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.68% | `python` | `insertdict` | dict |
| 0.68% | `libz.so.1.2.11` | `inflateBackEnd` | library |
| 0.57% | `python` | `_PyCode_New` | memory |
| 0.57% | `python` | `PyObject_SetAttr` | dynamic |
| 0.56% | `python` | `unicode_dealloc` | memory |
| 0.56% | `python` | `list_dealloc` | memory |
| 0.55% | `libpthread-2.31.so` | `__pthread_mutex_lock` | library |
| 0.55% | `libsqlite3.so.0.8.6` | `sqlite3_str_value` | library |
| 0.51% | `python` | `_PyPegen_fill_token` | interpreter |
| 0.51% | `libpthread-2.31.so` | `pthread_mutex_unlock` | library |

## docutils

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 26.70% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.74% | `python` | `sre_ucs1_match` | library |
| 3.66% | `python` | `gc_collect_main` | gc |
| 3.33% | `python` | `deduce_unreachable` | unknown |
| 2.86% | `python` | `PyObject_GetAttr` | dynamic |
| 2.40% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.39% | `python` | `visit_decref` | gc |
| 2.35% | `python` | `sre_ucs2_charset.isra.0` | library |
| 1.95% | `python` | `list_dealloc` | memory |
| 1.82% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.79% | `python` | `find_name_in_mro` | lookup |
| 1.38% | `python` | `visit_reachable` | gc |
| 1.08% | `python` | `PyObject_SetAttr` | dynamic |
| 1.07% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.95% | `python` | `_PyUnicode_JoinArray` | str |
| 0.92% | `python` | `tupledealloc` | memory |
| 0.83% | `python` | `subtype_traverse` | gc |
| 0.79% | `python` | `PyDict_GetItemRef` | dict |
| 0.78% | `python` | `PyMem_Free` | memory |
| 0.78% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 0.78% | `python` | `object_isinstance` | dynamic |
| 0.71% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.70% | `python` | `list_traverse` | gc |
| 0.67% | `python` | `list_subscript` | list |
| 0.65% | `python` | `insertdict` | dict |
| 0.63% | `python` | `dict_traverse` | gc |
| 0.61% | `python` | `PyUnicode_Format` | str |
| 0.60% | `python` | `PyMem_Malloc` | memory |
| 0.58% | `python` | `_PyObject_GenericGetAttrWithDict` | dynamic |
| 0.57% | `python` | `dict_dealloc` | memory |
| 0.56% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.54% | `python` | `unicode_dealloc` | memory |
| 0.54% | `python` | `dict_subscript` | dict |
| 0.53% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.52% | `python` | `PyObject_GC_Del` | gc |
| 0.52% | `python` | `sre_ucs1_count` | library |
| 0.51% | `python` | `BaseException_new` | memory |
| 0.51% | `python` | `_Py_type_getattro` | lookup |

## dulwich_log

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 30.31% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.84% | `libz.so.1.2.11` | `inflateCodesUsed` | library |
| 2.82% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.76% | `libz.so.1.2.11` | `inflateBackEnd` | library |
| 1.60% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.48% | `libz.so.1.2.11` | `inflate` | library |
| 1.24% | `python` | `PyBytes_FromStringAndSize` | str |
| 1.12% | `python` | `tupledealloc` | memory |
| 1.06% | `python` | `type_new` | memory |
| 1.00% | `python` | `PyObject_Free` | dynamic |
| 0.79% | `python` | `visit_decref` | gc |
| 0.77% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.75% | `python` | `gc_collect_main` | gc |
| 0.74% | `python` | `list_dealloc` | memory |
| 0.72% | `python` | `long_dealloc` | memory |
| 0.70% | `python` | `deduce_unreachable` | unknown |
| 0.55% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 0.53% | `python` | `unicode_dealloc` | memory |
| 0.53% | `python` | `_PyCode_New` | memory |
| 0.52% | `python` | `siphash13` | str |
| 0.52% | `python` | `visit_reachable` | gc |

## fannkuch

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 39.43% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.05% | `python` | `list_ass_slice_lock_held` | list |
| 6.48% | `python` | `list_dealloc` | memory |
| 5.93% | `python` | `PySlice_AdjustIndices` | miscobj |
| 4.46% | `python` | `list_subscript` | list |
| 4.26% | `python` | `PySlice_Unpack` | miscobj |
| 3.59% | `python` | `list_new_prealloc` | memory |
| 3.55% | `python` | `slice_dealloc` | memory |
| 2.62% | `python` | `_PyLong_Add` | int |
| 2.06% | `python` | `list_ass_subscript` | list |
| 1.69% | `python` | `PySlice_New` | memory |
| 1.68% | `python` | `_PyBuildSlice_Consume2` | unknown |
| 1.16% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.10% | `python` | `PyNumber_AsSsize_t` | dynamic |
| 1.09% | `python` | `PyObject_GetItem` | dynamic |
| 1.02% | `python` | `ins1` | unknown |
| 0.81% | `python` | `_PyLong_Subtract` | int |
| 0.79% | `python` | `PyObject_SetItem` | dynamic |
| 0.70% | `python` | `list_pop` | list |
| 0.67% | `python` | `PyMem_Malloc` | memory |

## float

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 37.88% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.66% | `libm-2.31.so` | `f64xsubf128` | library |
| 3.45% | `python` | `subtype_traverse` | gc |
| 2.80% | `python` | `visit_decref` | gc |
| 2.39% | `python` | `gc_collect_main` | gc |
| 2.38% | `python` | `visit_reachable` | gc |
| 2.22% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.08% | `python` | `deduce_unreachable` | unknown |
| 1.88% | `python` | `float_div` | float |
| 1.77% | `python` | `PyFloat_FromDouble` | float |
| 1.69% | `python` | `slot_tp_init` | unknown |
| 1.63% | `python` | `object_new` | memory |
| 1.36% | `python` | `_PyObject_Malloc` | memory |
| 1.31% | `python` | `PyFloat_AsDouble` | float |
| 1.30% | `python` | `clear_slots` | unknown |
| 1.10% | `python` | `_PyObject_Free` | memory |
| 0.98% | `python` | `PyLong_FromLong` | int |
| 0.98% | `python` | `float_dealloc` | memory |
| 0.91% | `python` | `tupledealloc` | memory |
| 0.86% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.83% | `python` | `type_new` | memory |
| 0.78% | `python` | `subtype_dealloc` | memory |
| 0.76% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.75% | `python` | `long_dealloc` | memory |
| 0.66% | `python` | `binary_op1` | unknown |
| 0.56% | `python` | `list_dealloc` | memory |
| 0.53% | `python` | `PyObject_GC_Del` | gc |

## gc_collect

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.51% | `python` | `gc_collect_main` | gc |
| 15.07% | `python` | `visit_reachable` | gc |
| 14.81% | `python` | `visit_decref` | gc |
| 11.39% | `python` | `deduce_unreachable` | unknown |
| 6.86% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.98% | `python` | `dict_traverse` | gc |
| 2.95% | `python` | `subtype_traverse` | gc |
| 2.05% | `python` | `func_traverse` | gc |
| 1.64% | `python` | `set_traverse` | gc |
| 0.86% | `python` | `tupletraverse` | tuple |
| 0.84% | `python` | `PyType_GenericAlloc` | memory |
| 0.84% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.82% | `python` | `type_traverse` | gc |
| 0.77% | `python` | `list_traverse` | gc |
| 0.59% | `python` | `subtype_dealloc` | memory |
| 0.56% | `python` | `PyObject_GC_Del` | gc |
| 0.53% | `python` | `meth_traverse` | gc |
| 0.51% | `python` | `_PyObject_InitInlineValues` | dynamic |

## gc_traversal

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 29.79% | `python` | `visit_reachable` | gc |
| 22.04% | `python` | `visit_decref` | gc |
| 13.59% | `python` | `list_traverse` | gc |
| 9.09% | `python` | `gc_collect_main` | gc |
| 4.76% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.92% | `python` | `deduce_unreachable` | unknown |
| 1.86% | `python` | `dict_traverse` | gc |
| 0.73% | `python` | `func_traverse` | gc |
| 0.65% | `python` | `subtype_traverse` | gc |
| 0.62% | `python` | `set_traverse` | gc |
| 0.54% | `python` | `PyLong_FromLong` | int |
| 0.53% | `python` | `type_new` | memory |

## generators

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 49.86% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.83% | `python` | `gen_dealloc` | memory |
| 2.68% | `python` | `gc_collect_main` | gc |
| 2.58% | `python` | `deduce_unreachable` | unknown |
| 2.31% | `python` | `long_add` | int |
| 2.03% | `python` | `make_gen` | unknown |
| 1.74% | `python` | `visit_reachable` | gc |
| 1.72% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.71% | `python` | `subtype_traverse` | gc |
| 1.67% | `python` | `visit_decref` | gc |
| 1.47% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.36% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.32% | `python` | `long_dealloc` | memory |
| 1.26% | `python` | `range_subscript` | unknown |
| 1.06% | `python` | `subtype_dealloc` | memory |
| 0.82% | `python` | `make_range_object` | unknown |
| 0.73% | `python` | `_PyObject_New` | memory |
| 0.69% | `python` | `type_new` | memory |
| 0.56% | `python` | `_PyType_Lookup` | lookup |
| 0.54% | `python` | `range_dealloc` | memory |
| 0.51% | `python` | `PyType_GenericAlloc` | memory |

## genshi

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 46.55% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.04% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.81% | `python` | `insertdict` | dict |
| 1.50% | `python` | `tupledealloc` | memory |
| 1.43% | `python` | `long_to_decimal_string_internal` | int |
| 1.39% | `python` | `_PyObject_GC_New` | gc |
| 1.33% | `python` | `insert_to_emptydict` | dict |
| 1.33% | `python` | `dictresize` | dict |
| 1.23% | `python` | `_PyObject_GetMethod` | dynamic |
| 1.21% | `python` | `_Py_type_getattro` | lookup |
| 1.18% | `python` | `dict_dealloc` | memory |
| 1.09% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.06% | `python` | `PyObject_GC_Del` | gc |
| 0.91% | `python` | `PyDict_GetItemRef` | dict |
| 0.91% | `python` | `type_new` | memory |
| 0.89% | `python` | `method_dealloc` | memory |
| 0.74% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.71% | `python` | `PyDict_SetItem` | dict |
| 0.69% | `python` | `cm_descr_get` | unknown |
| 0.69% | `python` | `dict_get` | dict |
| 0.66% | `python` | `_PyDict_FromItems` | dict |
| 0.65% | `python` | `PyObject_Str` | dynamic |
| 0.63% | `python` | `PyDict_Contains` | dict |
| 0.61% | `python` | `gc_collect_main` | gc |
| 0.61% | `python` | `object_isinstance` | dynamic |
| 0.58% | `python` | `visit_decref` | gc |
| 0.57% | `python` | `PyObject_GetAttr` | dynamic |
| 0.56% | `python` | `deduce_unreachable` | unknown |
| 0.55% | `python` | `func_dealloc` | memory |
| 0.53% | `python` | `PyObject_IsTrue` | dynamic |
| 0.52% | `python` | `PyMem_Free` | memory |
| 0.52% | `python` | `_PyUnicode_JoinArray` | str |
| 0.51% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |

## go

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 62.76% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.80% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.66% | `python` | `_PyObject_GetMethod` | dynamic |
| 1.62% | `python` | `PyDict_GetItemRef` | dict |
| 1.09% | `python` | `long_bitwise` | int |
| 1.05% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.04% | `python` | `long_dealloc` | memory |
| 0.95% | `python` | `type_new` | memory |
| 0.82% | `python` | `PyDict_SetItem` | dict |
| 0.80% | `python` | `_PyLong_Add` | int |
| 0.67% | `python` | `gc_collect_main` | gc |
| 0.65% | `python` | `visit_decref` | gc |
| 0.60% | `python` | `deduce_unreachable` | unknown |
| 0.59% | `python` | `PyObject_GC_Del` | gc |

## gunicorn

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 29.87% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.42% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.41% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.66% | `python` | `tupledealloc` | memory |
| 1.56% | `python` | `type_new` | memory |
| 1.15% | `python` | `gc_collect_main` | gc |
| 1.06% | `python` | `deduce_unreachable` | unknown |
| 1.02% | `python` | `visit_decref` | gc |
| 0.90% | `python` | `PyObject_GetAttr` | dynamic |
| 0.84% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.83% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.83% | `python` | `subtype_dealloc` | memory |
| 0.80% | `python` | `PyDict_GetItemRef` | dict |
| 0.72% | `python` | `unicode_dealloc` | memory |
| 0.72% | `python` | `visit_reachable` | gc |
| 0.70% | `python` | `dict_dealloc` | memory |
| 0.68% | `python` | `_PyCode_New` | memory |
| 0.62% | `python` | `_PySuper_Lookup` | dynamic |
| 0.61% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.59% | `python` | `list_dealloc` | memory |
| 0.59% | `python` | `find_name_in_mro` | lookup |
| 0.57% | `python` | `r_object` | import |
| 0.56% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.55% | `python` | `sre_ucs1_match` | library |
| 0.53% | `python` | `slot_tp_init` | unknown |
| 0.52% | `python` | `PyObject_GC_Del` | gc |

## hexiom

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 62.71% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.53% | `python` | `list_contains` | list |
| 3.13% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.27% | `python` | `long_richcompare` | int |
| 1.23% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.05% | `python` | `gen_iternext` | unknown |
| 0.94% | `python` | `builtin_sum` | unknown |
| 0.88% | `python` | `list_dealloc` | memory |
| 0.74% | `python` | `PyLong_FromLong` | int |
| 0.70% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.69% | `python` | `type_new` | memory |
| 0.50% | `python` | `gc_collect_main` | gc |

## html5lib

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 38.18% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.06% | `python` | `sre_ucs2_charset.isra.0` | library |
| 1.98% | `python` | `gc_collect_main` | gc |
| 1.81% | `python` | `PyDict_GetItemRef` | dict |
| 1.79% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.71% | `python` | `deduce_unreachable` | unknown |
| 1.65% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.52% | `python` | `visit_decref` | gc |
| 1.22% | `python` | `PyObject_GetAttr` | dynamic |
| 1.19% | `python` | `type_new` | memory |
| 0.88% | `python` | `visit_reachable` | gc |
| 0.75% | `python` | `sre_ucs1_count` | library |
| 0.75% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.74% | `python` | `insertdict` | dict |
| 0.72% | `python` | `tupledealloc` | memory |
| 0.62% | `python` | `set_contains_lock_held` | miscobj |
| 0.61% | `python` | `list_dealloc` | memory |
| 0.59% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.57% | `python` | `unicode_dealloc` | memory |
| 0.56% | `python` | `list_contains` | list |
| 0.55% | `python` | `dict_dealloc` | memory |
| 0.52% | `python` | `PyUnicode_Concat` | str |
| 0.52% | `python` | `_PyCode_New` | memory |

## json

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 18.05% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_object_unicode` | library |
| 8.83% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.95% | `python` | `PyUnicode_Substring` | str |
| 5.73% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 5.44% | `python` | `siphash13` | str |
| 5.16% | `python` | `PyDict_SetItem` | dict |
| 3.56% | `python` | `unicode_dealloc` | memory |
| 3.03% | `python` | `dictresize` | dict |
| 3.01% | `python` | `PyLong_FromString` | int |
| 2.28% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 2.13% | `python` | `dict_dealloc` | memory |
| 1.97% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.87% | `python` | `_sre_SRE_Pattern_match` | library |
| 1.36% | `_json.cpython-313-x86_64-linux-gnu.so` | `_match_number_unicode.isra.0` | library |
| 1.25% | `python` | `PyBytes_FromStringAndSize` | str |
| 1.10% | `python` | `PyObject_Free` | dynamic |
| 0.80% | `python` | `PyDict_GetItemRef` | dict |
| 0.76% | `python` | `tupledealloc` | memory |
| 0.74% | `python` | `type_new` | memory |
| 0.74% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.71% | `python` | `insert_to_emptydict` | dict |
| 0.60% | `python` | `sre_ucs1_match` | library |
| 0.60% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.58% | `python` | `long_dealloc` | memory |
| 0.56% | `python` | `gc_collect_main` | gc |
| 0.56% | `python` | `unicode_hash` | str |
| 0.56% | `python` | `visit_decref` | gc |
| 0.54% | `python` | `deduce_unreachable` | unknown |

## json_dumps

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 15.23% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.50% | `_json.cpython-313-x86_64-linux-gnu.so` | `encoder_encode_key_value` | library |
| 6.54% | `python` | `PyUnicode_New` | memory |
| 5.17% | `python` | `unicode_dealloc` | memory |
| 5.07% | `python` | `_PyUnicodeWriter_WriteStr` | str |
| 3.39% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 3.39% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 2.79% | `_json.cpython-313-x86_64-linux-gnu.so` | `py_encode_basestring_ascii` | library |
| 2.36% | `python` | `vgetargskeywords.constprop.0` | calls |
| 2.03% | `python` | `PyDict_GetItemRef` | dict |
| 1.68% | `python` | `resize_compact` | str |
| 1.62% | `python` | `long_to_decimal_string` | int |
| 1.56% | `python` | `tupledealloc` | memory |
| 1.43% | `python` | `_PyObject_Malloc` | memory |
| 1.27% | `python` | `PyDict_SetItem` | dict |
| 1.21% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.18% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.17% | `python` | `PyDict_Next` | dict |
| 1.08% | `python` | `PyFunction_NewWithQualName` | memory |
| 1.01% | `python` | `object_isinstance` | dynamic |
| 0.84% | `python` | `_PyLong_New` | memory |
| 0.83% | `python` | `func_dealloc` | memory |
| 0.81% | `python` | `PyObject_GetAttr` | dynamic |
| 0.77% | `python` | `type_new` | memory |
| 0.74% | `python` | `PyDict_DelItem` | dict |
| 0.73% | `python` | `PyTuple_New` | memory |
| 0.73% | `python` | `_Py_type_getattro` | lookup |
| 0.71% | `python` | `long_hash` | int |
| 0.67% | `python` | `long_dealloc` | memory |
| 0.64% | `python` | `_Py_dict_lookup` | lookup |
| 0.60% | `python` | `dict_dealloc` | memory |
| 0.59% | `python` | `PyDict_Contains` | dict |
| 0.59% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.57% | `_json.cpython-313-x86_64-linux-gnu.so` | `encoder_listencode_obj` | library |
| 0.56% | `python` | `PyMem_Free` | memory |
| 0.54% | `python` | `visit_decref` | gc |
| 0.54% | `python` | `gc_collect_main` | gc |

## json_loads

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 19.46% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_object_unicode` | library |
| 10.78% | `python` | `PyUnicode_Substring` | str |
| 6.88% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.85% | `python` | `siphash13` | str |
| 5.83% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 4.93% | `python` | `PyDict_SetItem` | dict |
| 4.23% | `python` | `unicode_dealloc` | memory |
| 3.24% | `python` | `PyLong_FromString` | int |
| 2.55% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.14% | `python` | `dictresize` | dict |
| 1.52% | `python` | `dict_dealloc` | memory |
| 1.26% | `_json.cpython-313-x86_64-linux-gnu.so` | `_match_number_unicode.isra.0` | library |
| 1.24% | `python` | `PyBytes_FromStringAndSize` | str |
| 1.15% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.01% | `python` | `PyObject_Free` | dynamic |
| 0.99% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.94% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_array_unicode` | library |
| 0.91% | `python` | `type_new` | memory |
| 0.68% | `python` | `unicode_hash` | str |
| 0.61% | `python` | `gc_collect_main` | gc |
| 0.60% | `python` | `visit_decref` | gc |
| 0.59% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.56% | `python` | `deduce_unreachable` | unknown |
| 0.51% | `python` | `tupledealloc` | memory |
| 0.50% | `python` | `long_dealloc` | memory |

## logging

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 47.95% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.64% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.19% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 2.28% | `python` | `PyDict_GetItemRef` | dict |
| 1.83% | `python` | `PyCode_Addr2Line` | exceptions |
| 1.71% | `python` | `PyObject_GetAttr` | dynamic |
| 1.69% | `python` | `dict_dealloc` | memory |
| 1.66% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.95% | `python` | `tupledealloc` | memory |
| 0.74% | `python` | `type_new` | memory |
| 0.66% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 0.60% | `python` | `unicode_subscript` | str |
| 0.59% | `python` | `meth_dealloc` | memory |
| 0.58% | `python` | `unicode_dealloc` | memory |
| 0.52% | `python` | `PyLong_FromLong` | int |
| 0.51% | `python` | `long_dealloc` | memory |

## mako

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 39.51% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.27% | `python` | `long_to_decimal_string_internal` | int |
| 6.93% | `python` | `unicode_replace` | str |
| 4.21% | `python` | `_PyUnicode_JoinArray` | str |
| 2.53% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.29% | `python` | `unicode_dealloc` | memory |
| 1.56% | `python` | `deque_append_lock_held` | miscobj |
| 1.54% | `python` | `dequeiter_next_lock_held.isra.0` | miscobj |
| 1.48% | `python` | `PyObject_Str` | dynamic |
| 1.34% | `python` | `list_dealloc` | memory |
| 1.20% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.19% | `python` | `PySequence_List` | dynamic |
| 1.08% | `python` | `sre_ucs2_charset.isra.0` | library |
| 0.91% | `python` | `type_new` | memory |
| 0.83% | `python` | `deque_clear` | miscobj |
| 0.79% | `python` | `deque_append_impl` | miscobj |
| 0.73% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.63% | `python` | `gc_collect_main` | gc |
| 0.60% | `python` | `deduce_unreachable` | unknown |
| 0.58% | `python` | `PyLong_FromLong` | int |
| 0.55% | `python` | `visit_decref` | gc |

## mdp

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 37.79% | `python` | `tuplehash` | tuple |
| 17.76% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 12.78% | `python` | `long_hash` | int |
| 5.77% | `python` | `dict_subscript` | dict |
| 3.02% | `python` | `tuplerichcompare` | tuple |
| 1.36% | `python` | `insertdict` | dict |
| 1.23% | `python` | `_PyLong_GCD` | int |
| 1.11% | `python` | `PyDict_GetItemRef` | dict |
| 1.09% | `python` | `_PySuper_Lookup` | dynamic |
| 0.94% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.83% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.75% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.58% | `python` | `builtin_sum` | unknown |
| 0.55% | `python` | `gen_dealloc` | memory |
| 0.55% | `python` | `set_contains_lock_held` | miscobj |
| 0.51% | `python` | `tupledealloc` | memory |

## meteor_contest

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 23.18% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.18% | `python` | `set_issubset_impl` | miscobj |
| 6.47% | `python` | `setiter_iternext` | miscobj |
| 5.19% | `python` | `set_lookkey` | miscobj |
| 4.65% | `python` | `set_difference` | miscobj |
| 4.30% | `python` | `set_dealloc` | memory |
| 3.23% | `python` | `builtin_min` | unknown |
| 2.23% | `python` | `list_dealloc` | memory |
| 1.97% | `python` | `set_add_entry` | miscobj |
| 1.62% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.57% | `python` | `list_subscript` | list |
| 1.53% | `python` | `PyObject_GC_Del` | gc |
| 1.21% | `python` | `long_richcompare` | int |
| 1.16% | `python` | `set_table_resize` | miscobj |
| 1.14% | `python` | `PyObject_RichCompare` | dynamic |
| 1.11% | `python` | `type_new` | memory |
| 1.03% | `python` | `make_new_set` | memory |
| 0.97% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.95% | `python` | `set_intersection` | miscobj |
| 0.78% | `python` | `gc_collect_main` | gc |
| 0.72% | `python` | `deduce_unreachable` | unknown |
| 0.69% | `python` | `visit_decref` | gc |
| 0.65% | `python` | `list_iter` | list |
| 0.64% | `python` | `_PyObject_GC_New` | gc |
| 0.56% | `python` | `visit_reachable` | gc |
| 0.55% | `python` | `PyIter_Next` | dynamic |

## mypy2

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 31.73% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.14% | `python` | `gc_collect_main` | gc |
| 7.09% | `python` | `deduce_unreachable` | unknown |
| 2.93% | `python` | `visit_decref` | gc |
| 2.84% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.65% | `python` | `subtype_traverse` | gc |
| 1.60% | `python` | `PyDict_GetItemRef` | dict |
| 1.54% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.40% | `python` | `visit_reachable` | gc |
| 1.36% | `python` | `object_isinstance` | dynamic |
| 1.33% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_object_unicode` | library |
| 1.25% | `python` | `_PySuper_Lookup` | dynamic |
| 1.09% | `python` | `list_dealloc` | memory |
| 1.03% | `python` | `PyUnicode_Substring` | str |
| 1.02% | `python` | `PyObject_SetAttr` | dynamic |
| 1.02% | `python` | `clear_slots` | unknown |
| 0.97% | `python` | `subtype_dealloc` | memory |
| 0.94% | `python` | `siphash13` | str |
| 0.90% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.86% | `python` | `dict_dealloc` | memory |
| 0.85% | `python` | `tupledealloc` | memory |
| 0.76% | `python` | `slot_tp_init` | unknown |
| 0.74% | `python` | `PyObject_GC_Del` | gc |
| 0.72% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.72% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.70% | `python` | `unicode_dealloc` | memory |
| 0.66% | `python` | `object_new` | memory |
| 0.65% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.62% | `python` | `PyDict_SetItem` | dict |
| 0.59% | `python` | `list_traverse` | gc |
| 0.55% | `python` | `PyObject_GetAttr` | dynamic |
| 0.51% | `python` | `insertdict` | dict |

## nbody

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 69.22% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.17% | `python` | `PyFloat_FromDouble` | float |
| 3.58% | `libm-2.31.so` | `f64xsubf128` | library |
| 2.37% | `python` | `float_dealloc` | memory |
| 1.30% | `python` | `float_pow` | float |
| 0.75% | `python` | `type_new` | memory |
| 0.60% | `python` | `_PyNumber_PowerNoMod` | dynamic |
| 0.51% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.51% | `python` | `deduce_unreachable` | unknown |
| 0.51% | `python` | `gc_collect_main` | gc |

## nqueens

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 39.15% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.54% | `python` | `set_vectorcall` | miscobj |
| 2.94% | `python` | `list_dealloc` | memory |
| 2.87% | `python` | `PyFunction_NewWithQualName` | memory |
| 2.34% | `python` | `gen_iternext` | unknown |
| 2.24% | `python` | `set_dealloc` | memory |
| 1.78% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.78% | `python` | `func_dealloc` | memory |
| 1.52% | `python` | `PyList_New` | memory |
| 1.40% | `python` | `make_gen` | unknown |
| 1.38% | `python` | `gen_dealloc` | memory |
| 1.35% | `python` | `list_subscript` | list |
| 1.35% | `python` | `tupledealloc` | memory |
| 1.30% | `python` | `_PyLong_Add` | int |
| 1.11% | `python` | `PySlice_Unpack` | miscobj |
| 1.03% | `python` | `_PyBuildSlice_Consume2` | unknown |
| 0.89% | `python` | `PyLong_FromLong` | int |
| 0.86% | `python` | `list_ass_slice_lock_held` | list |
| 0.83% | `python` | `PyMem_Malloc` | memory |
| 0.79% | `python` | `type_new` | memory |
| 0.78% | `python` | `slice_dealloc` | memory |
| 0.67% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 0.63% | `python` | `PyObject_Free` | dynamic |
| 0.59% | `python` | `_PyLong_Subtract` | int |
| 0.58% | `python` | `gc_collect_main` | gc |
| 0.56% | `python` | `method_get` | dynamic |
| 0.56% | `python` | `deduce_unreachable` | unknown |
| 0.54% | `python` | `PySequence_Tuple` | dynamic |
| 0.54% | `python` | `visit_decref` | gc |
| 0.53% | `python` | `list_ass_subscript` | list |

## pathlib

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.69% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.29% | `python` | `long_dealloc` | memory |
| 1.82% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.72% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.41% | `[kernel.kallsyms]` | `__d_lookup_rcu` | kernel |
| 1.25% | `python` | `_PySuper_Lookup` | dynamic |
| 1.23% | `python` | `k_mul` | int |
| 1.19% | `libpthread-2.31.so` | `__pthread_mutex_lock` | library |
| 1.16% | `[kernel.kallsyms]` | `ext4_htree_store_dirent` | kernel |
| 1.12% | `[kernel.kallsyms]` | `memset_erms` | kernel |
| 1.08% | `[kernel.kallsyms]` | `__ext4fs_dirhash` | kernel |
| 1.06% | `python` | `path_converter` | unknown |
| 1.05% | `libpthread-2.31.so` | `pthread_mutex_unlock` | library |
| 1.01% | `python` | `tupledealloc` | memory |
| 1.01% | `python` | `unicode_decode_utf8` | str |
| 0.95% | `python` | `_PyLong_New` | memory |
| 0.94% | `python` | `ScandirIterator_iternext` | unknown |
| 0.85% | `python` | `list_dealloc` | memory |
| 0.85% | `python` | `PyUnicode_FSConverter` | str |
| 0.81% | `python` | `PyLong_FromLong` | int |
| 0.80% | `python` | `type_new` | memory |
| 0.77% | `[kernel.kallsyms]` | `filldir64` | kernel |
| 0.75% | `python` | `os_listdir` | unknown |
| 0.75% | `python` | `PyEval_RestoreThread` | interpreter |
| 0.74% | `python` | `_Py_type_getattro` | lookup |
| 0.73% | `python` | `_Py_dict_lookup` | lookup |
| 0.72% | `python` | `x_add` | int |
| 0.67% | `[kernel.kallsyms]` | `strncpy_from_user` | kernel |
| 0.67% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.64% | `python` | `method_dealloc` | memory |
| 0.64% | `python` | `_PyUnicode_JoinArray` | str |
| 0.64% | `python` | `unicode_dealloc` | memory |
| 0.62% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.62% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.61% | `python` | `sre_ucs1_match` | library |
| 0.60% | `python` | `vectorcall_method` | calls |
| 0.60% | `python` | `slot_tp_init` | unknown |
| 0.59% | `[kernel.kallsyms]` | `kmem_cache_alloc` | kernel |
| 0.59% | `python` | `visit_decref` | gc |
| 0.59% | `[kernel.kallsyms]` | `link_path_walk.part.0` | kernel |
| 0.58% | `python` | `PyObject_GC_Del` | gc |
| 0.58% | `python` | `gc_collect_main` | gc |
| 0.57% | `python` | `PyUnicode_DecodeFSDefault` | str |
| 0.56% | `python` | `deduce_unreachable` | unknown |
| 0.55% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 0.55% | `python` | `tp_new_wrapper` | memory |
| 0.52% | `python` | `structseq_dealloc` | memory |
| 0.51% | `python` | `object_isinstance` | dynamic |
| 0.51% | `[kernel.kallsyms]` | `__virt_addr_valid` | kernel |

## pickle

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 25.36% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `save` | library |
| 13.17% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_put.isra.0` | library |
| 6.81% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_write_bytes` | library |
| 4.92% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.16% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.90% | `python` | `PyDict_Next` | dict |
| 2.79% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_get.isra.0` | library |
| 2.64% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pickler_dealloc` | library |
| 1.90% | `python` | `PyUnicode_AsUTF8AndSize` | str |
| 1.66% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.53% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_Write` | library |
| 1.02% | `python` | `type_new` | memory |
| 0.71% | `python` | `gc_collect_main` | gc |
| 0.62% | `python` | `deduce_unreachable` | unknown |
| 0.59% | `python` | `visit_decref` | gc |
| 0.54% | `python` | `PyMem_Malloc` | memory |
| 0.54% | `python` | `unicode_decode_utf8` | str |
| 0.54% | `python` | `tupledealloc` | memory |
| 0.52% | `python` | `_PyCode_New` | memory |

## pickle_dict

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 46.63% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `save` | library |
| 13.35% | `python` | `PyDict_Next` | dict |
| 9.88% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_Write` | library |
| 3.56% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.79% | `python` | `PyLong_AsLongAndOverflow` | int |
| 2.79% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_put.isra.0` | library |
| 1.05% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.79% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pickler_dealloc` | library |
| 0.78% | `python` | `type_new` | memory |
| 0.70% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005cd4` | library |
| 0.67% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005e54` | library |
| 0.56% | `python` | `gc_collect_main` | gc |
| 0.53% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |

## pickle_list

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 41.65% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `save` | library |
| 12.20% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_Write` | library |
| 5.27% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.15% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_put.isra.0` | library |
| 3.25% | `python` | `PyLong_AsLongAndOverflow` | int |
| 2.05% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.41% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.22% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pickler_dealloc` | library |
| 1.19% | `python` | `type_new` | memory |
| 0.81% | `python` | `gc_collect_main` | gc |
| 0.76% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005cd4` | library |
| 0.70% | `python` | `visit_decref` | gc |
| 0.67% | `python` | `deduce_unreachable` | unknown |
| 0.60% | `python` | `_PyThreadState_GetCurrent` | unknown |
| 0.58% | `python` | `PyList_Size` | list |
| 0.52% | `python` | `visit_reachable` | gc |
| 0.51% | `python` | `_PyCode_New` | memory |

## pickle_pure_python

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 48.43% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.88% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.63% | `python` | `bytes_concat` | str |
| 2.52% | `python` | `dict_get` | dict |
| 2.24% | `python` | `unicode_encode` | str |
| 1.91% | `python` | `PyObject_Free` | dynamic |
| 1.72% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.51% | `python` | `insertdict` | dict |
| 1.45% | `python` | `long_dealloc` | memory |
| 1.38% | `python` | `PyDict_GetItemRef` | dict |
| 1.29% | `python` | `_PyLong_New` | memory |
| 1.02% | `python` | `tupledealloc` | memory |
| 0.98% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.97% | `python` | `write_bytes` | unknown |
| 0.88% | `python` | `unicode_encode_utf8` | str |
| 0.76% | `python` | `PyType_GetModuleByDef` | dynamic |
| 0.73% | `python` | `type_new` | memory |
| 0.72% | `python` | `PyDict_Contains` | dict |
| 0.69% | `python` | `PySys_Audit` | unknown |
| 0.67% | `python` | `long_hash` | int |
| 0.56% | `python` | `builtin_id` | unknown |
| 0.55% | `_struct.cpython-313-x86_64-linux-gnu.so` | `s_pack` | library |
| 0.54% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.51% | `python` | `gc_collect_main` | gc |

## pidigits

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 33.43% | `python` | `x_divrem` | int |
| 20.09% | `python` | `k_mul` | int |
| 12.67% | `python` | `x_add` | int |
| 7.98% | `python` | `x_sub` | int |
| 4.89% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.38% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.78% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.76% | `python` | `type_new` | memory |
| 0.51% | `python` | `gc_collect_main` | gc |

## pprint

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 45.26% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.54% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.68% | `python` | `tupledealloc` | memory |
| 2.63% | `python` | `_Py_type_getattro_impl` | dynamic |
| 2.50% | `python` | `long_to_decimal_string` | int |
| 2.28% | `python` | `_Py_type_getattro` | lookup |
| 2.22% | `python` | `PyUnicode_Format` | str |
| 2.11% | `python` | `_PyUnicode_JoinArray` | str |
| 1.99% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.81% | `python` | `unicode_dealloc` | memory |
| 1.28% | `python` | `PyObject_GetAttr` | dynamic |
| 1.17% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 1.06% | `python` | `set_contains_lock_held` | miscobj |
| 1.04% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.97% | `python` | `list_dealloc` | memory |
| 0.95% | `python` | `slot_tp_init` | unknown |
| 0.88% | `python` | `meth_dealloc` | memory |
| 0.83% | `python` | `insertdict` | dict |
| 0.82% | `python` | `builtin_issubclass` | unknown |
| 0.81% | `python` | `PyDict_Contains` | dict |
| 0.76% | `python` | `slot_tp_richcompare` | dynamic |
| 0.69% | `python` | `_PyObject_Malloc` | memory |
| 0.68% | `python` | `PyObject_GC_Del` | gc |
| 0.66% | `python` | `object_new` | memory |
| 0.66% | `python` | `method_get` | dynamic |
| 0.65% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.60% | `python` | `long_hash` | int |
| 0.56% | `python` | `_Py_dict_lookup` | lookup |
| 0.54% | `python` | `_PyLong_New` | memory |
| 0.53% | `python` | `builtin_sorted` | unknown |
| 0.53% | `python` | `list_sort_impl` | list |
| 0.52% | `python` | `builtin_getattr` | lookup |
| 0.51% | `python` | `list_append` | list |

## pycparser

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 34.10% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 16.99% | `python` | `sre_ucs1_match` | library |
| 2.87% | `python` | `_sre_SRE_Pattern_match` | library |
| 2.44% | `python` | `gc_collect_main` | gc |
| 2.43% | `python` | `PyDict_GetItemRef` | dict |
| 2.33% | `python` | `deduce_unreachable` | unknown |
| 2.27% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.99% | `python` | `object_new` | memory |
| 1.47% | `python` | `dict_get` | dict |
| 1.42% | `python` | `subtype_dealloc` | memory |
| 1.40% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.31% | `python` | `visit_decref` | gc |
| 1.24% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.23% | `python` | `visit_reachable` | gc |
| 1.19% | `python` | `subtype_traverse` | gc |
| 0.96% | `python` | `list_ass_slice_lock_held` | list |
| 0.90% | `python` | `list_dealloc` | memory |
| 0.82% | `python` | `object_isinstance` | dynamic |
| 0.76% | `python` | `slot_mp_ass_subscript` | unknown |
| 0.74% | `python` | `sre_ucs1_count` | library |
| 0.64% | `python` | `PyObject_GetAttr` | dynamic |
| 0.62% | `python` | `PyDict_Contains` | dict |
| 0.60% | `python` | `PyObject_GC_Del` | gc |
| 0.56% | `python` | `list_subscript` | list |
| 0.52% | `python` | `sre_ucs2_charset.isra.0` | library |
| 0.51% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.50% | `python` | `slot_tp_init` | unknown |

## pyflate

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 42.97% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.37% | `python` | `list_dealloc` | memory |
| 5.79% | `python` | `list_ass_slice_lock_held` | list |
| 2.69% | `python` | `list_subscript` | list |
| 2.59% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 2.48% | `python` | `long_dealloc` | memory |
| 2.41% | `python` | `list_concat` | list |
| 2.32% | `python` | `bytes_subscript` | str |
| 2.02% | `python` | `_PyLong_Add` | int |
| 1.68% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.36% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.31% | `python` | `long_lshift` | int |
| 1.30% | `python` | `_PyLong_Subtract` | int |
| 1.28% | `python` | `stringlib_bytes_join.lto_priv.1` | str |
| 1.13% | `python` | `PySlice_Unpack` | miscobj |
| 1.02% | `python` | `_PyLong_New` | memory |
| 1.00% | `python` | `PyObject_Free` | dynamic |
| 0.88% | `python` | `list_sort_impl` | list |
| 0.63% | `python` | `unsafe_long_compare` | unknown |
| 0.58% | `python` | `PyObject_GetItem` | dynamic |
| 0.52% | `python` | `long_and` | int |
| 0.51% | `python` | `long_rshift` | int |
| 0.51% | `python` | `_PyBuildSlice_Consume2` | unknown |

## pylint

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 26.94% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.27% | `python` | `gc_collect_main` | gc |
| 5.58% | `python` | `deduce_unreachable` | unknown |
| 3.69% | `python` | `visit_decref` | gc |
| 2.96% | `python` | `visit_reachable` | gc |
| 2.11% | `python` | `subtype_traverse` | gc |
| 1.87% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.78% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.65% | `python` | `PyDict_GetItemRef` | dict |
| 1.63% | `python` | `PyObject_GetAttr` | dynamic |
| 1.15% | `python` | `find_name_in_mro` | lookup |
| 0.99% | `python` | `tupledealloc` | memory |
| 0.98% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.97% | `python` | `object_isinstance` | dynamic |
| 0.86% | `python` | `dict_traverse` | gc |
| 0.83% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.76% | `python` | `dict_dealloc` | memory |
| 0.71% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.70% | `python` | `PyObject_SetAttr` | dynamic |
| 0.70% | `python` | `list_traverse` | gc |
| 0.64% | `python` | `list_dealloc` | memory |
| 0.64% | `python` | `gen_dealloc` | memory |
| 0.61% | `python` | `type_new` | memory |
| 0.58% | `python` | `make_gen` | unknown |
| 0.56% | `python` | `PyObject_GC_Del` | gc |
| 0.56% | `python` | `subtype_dealloc` | memory |

## python_startup

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 8.40% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.63% | `python` | `type_new` | memory |
| 3.47% | `python` | `_PyCode_New` | memory |
| 3.11% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 3.04% | `python` | `r_object` | import |
| 2.63% | `python` | `gc_collect_main` | gc |
| 2.60% | `python` | `visit_decref` | gc |
| 2.46% | `python` | `deduce_unreachable` | unknown |
| 2.31% | `python` | `visit_reachable` | gc |
| 2.30% | `python` | `PyUnicode_FromKindAndData` | str |
| 1.58% | `ld-2.31.so` | `_dl_rtld_di_serinfo` | library |
| 1.58% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 1.44% | `python` | `siphash13` | str |
| 1.33% | `python` | `_PyUnicode_InternInPlace` | str |
| 1.08% | `python` | `tupledealloc` | memory |
| 1.04% | `python` | `unicode_decode_utf8` | str |
| 0.99% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.94% | `python` | `type_ready` | dynamic |
| 0.87% | `python` | `dict_traverse` | gc |
| 0.81% | `[kernel.kallsyms]` | `filemap_map_pages` | kernel |
| 0.81% | `python` | `find_name_in_mro` | lookup |
| 0.77% | `python` | `PyDict_SetItem` | dict |
| 0.74% | `[kernel.kallsyms]` | `native_irq_return_iret` | kernel |
| 0.71% | `python` | `_Py_dict_lookup` | lookup |
| 0.68% | `python` | `insertdict` | dict |
| 0.65% | `python` | `unicode_dealloc` | memory |
| 0.63% | `libc-2.31.so` | `_dl_addr` | libc |
| 0.61% | `python` | `PyBytes_FromStringAndSize` | str |
| 0.61% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.57% | `python` | `PyDict_GetItemRef` | dict |
| 0.57% | `[kernel.kallsyms]` | `sync_regs` | kernel |
| 0.53% | `python` | `dictresize` | dict |

## python_startup_no_site

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 8.20% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.86% | `python` | `type_new` | memory |
| 3.50% | `python` | `_PyCode_New` | memory |
| 3.17% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 3.02% | `python` | `r_object` | import |
| 2.84% | `python` | `gc_collect_main` | gc |
| 2.72% | `python` | `visit_decref` | gc |
| 2.64% | `python` | `deduce_unreachable` | unknown |
| 2.39% | `python` | `visit_reachable` | gc |
| 2.15% | `python` | `PyUnicode_FromKindAndData` | str |
| 1.95% | `ld-2.31.so` | `_dl_rtld_di_serinfo` | library |
| 1.65% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 1.44% | `python` | `siphash13` | str |
| 1.35% | `python` | `_PyUnicode_InternInPlace` | str |
| 1.06% | `python` | `unicode_decode_utf8` | str |
| 1.04% | `python` | `tupledealloc` | memory |
| 1.03% | `python` | `dict_traverse` | gc |
| 1.02% | `python` | `type_ready` | dynamic |
| 1.00% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.88% | `[kernel.kallsyms]` | `filemap_map_pages` | kernel |
| 0.88% | `python` | `PyDict_SetItem` | dict |
| 0.81% | `python` | `find_name_in_mro` | lookup |
| 0.79% | `[kernel.kallsyms]` | `native_irq_return_iret` | kernel |
| 0.78% | `python` | `insertdict` | dict |
| 0.68% | `python` | `_Py_dict_lookup` | lookup |
| 0.65% | `python` | `dictresize` | dict |
| 0.64% | `libc-2.31.so` | `_dl_addr` | libc |
| 0.63% | `python` | `PyBytes_FromStringAndSize` | str |
| 0.61% | `python` | `unicode_dealloc` | memory |
| 0.59% | `[kernel.kallsyms]` | `sync_regs` | kernel |
| 0.57% | `python` | `PyDict_GetItemRef` | dict |
| 0.53% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.52% | `libc-2.31.so` | `wcsrtombs` | libc |
| 0.50% | `python` | `code_dealloc` | memory |

## raytrace

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 56.12% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.99% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.97% | `python` | `subtype_dealloc` | memory |
| 1.99% | `python` | `PyType_GenericAlloc` | memory |
| 1.97% | `python` | `PyFloat_FromDouble` | float |
| 1.53% | `python` | `vectorcall_maybe.constprop.0` | unknown |
| 1.50% | `python` | `_PyObject_InitInlineValues` | dynamic |
| 1.24% | `python` | `PyNumber_Subtract` | dynamic |
| 1.20% | `python` | `PyObject_GC_Del` | gc |
| 1.08% | `python` | `float_dealloc` | memory |
| 1.08% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.77% | `python` | `convert_to_double` | unknown |
| 0.64% | `python` | `tupledealloc` | memory |
| 0.63% | `python` | `float_sub` | float |
| 0.56% | `python` | `type_new` | memory |
| 0.52% | `python` | `float_richcompare` | float |
| 0.51% | `python` | `long_dealloc` | memory |

## regex_compile

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 44.60% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.18% | `python` | `sre_ucs1_match` | library |
| 2.68% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.53% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.50% | `python` | `PyNumber_AsSsize_t` | dynamic |
| 1.15% | `python` | `long_dealloc` | memory |
| 1.08% | `python` | `PyLong_FromLong` | int |
| 1.08% | `python` | `tupledealloc` | memory |
| 1.02% | `python` | `sre_ucs2_charset.isra.0` | library |
| 0.96% | `python` | `list_dealloc` | memory |
| 0.95% | `python` | `object_isinstance` | dynamic |
| 0.89% | `python` | `PyObject_GetAttr` | dynamic |
| 0.84% | `python` | `type_new` | memory |
| 0.72% | `python` | `bytearray_ass_subscript` | miscobj |
| 0.63% | `python` | `gc_collect_main` | gc |
| 0.59% | `python` | `visit_decref` | gc |
| 0.55% | `python` | `deduce_unreachable` | unknown |
| 0.55% | `python` | `PyObject_GC_Del` | gc |
| 0.53% | `python` | `sre_search` | library |
| 0.53% | `python` | `vectorcall_method` | calls |

## regex_dna

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.98% | `python` | `sre_ucs1_match` | library |
| 29.31% | `python` | `sre_ucs2_charset.isra.0` | library |
| 7.15% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.11% | `python` | `sre_search` | library |
| 2.90% | `libm-2.31.so` | `__fmod_finite` | library |
| 1.12% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.07% | `_bisect.cpython-313-x86_64-linux-gnu.so` | `_bisect_bisect_right` | library |
| 0.89% | `python` | `float_richcompare` | float |
| 0.89% | `python` | `pattern_subx` | library |
| 0.61% | `python` | `stringlib_bytes_join.lto_priv.1` | str |
| 0.58% | `python` | `PyFloat_FromDouble` | float |
| 0.56% | `python` | `type_new` | memory |

## regex_effbot

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 38.33% | `python` | `sre_ucs1_match` | library |
| 16.73% | `python` | `sre_ucs2_charset.isra.0` | library |
| 6.15% | `python` | `sre_search` | library |
| 5.51% | `python` | `PyMem_Free` | memory |
| 5.45% | `python` | `PyMem_Malloc` | memory |
| 5.06% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 1.94% | `python` | `sre_ucs1_count` | library |
| 0.89% | `python` | `type_new` | memory |
| 0.64% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.61% | `python` | `gc_collect_main` | gc |
| 0.56% | `python` | `deduce_unreachable` | unknown |
| 0.53% | `python` | `visit_decref` | gc |

## regex_v8

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 33.09% | `python` | `sre_ucs1_match` | library |
| 10.44% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.44% | `python` | `sre_ucs1_count` | library |
| 3.45% | `python` | `PyCode_Addr2Line` | exceptions |
| 3.04% | `python` | `sre_search` | library |
| 2.12% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.32% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.25% | `python` | `sre_ucs1_match.cold` | library |
| 1.25% | `python` | `pattern_subx` | library |
| 1.12% | `python` | `type_new` | memory |
| 1.03% | `python` | `PyMem_Free` | memory |
| 1.00% | `python` | `state_init` | unknown |
| 0.79% | `python` | `gc_collect_main` | gc |
| 0.76% | `python` | `visit_decref` | gc |
| 0.71% | `python` | `deduce_unreachable` | unknown |
| 0.67% | `python` | `PyUnicode_Substring` | str |
| 0.64% | `python` | `_PyUnicode_JoinArray` | str |
| 0.61% | `python` | `list_dealloc` | memory |
| 0.59% | `python` | `PyLong_FromLong` | int |
| 0.59% | `libc-2.31.so` | `malloc` | libc |
| 0.57% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.54% | `python` | `unicode_dealloc` | memory |
| 0.53% | `python` | `tupledealloc` | memory |
| 0.53% | `python` | `visit_reachable` | gc |
| 0.53% | `python` | `PyDict_GetItemRef` | dict |
| 0.53% | `python` | `PyMem_Malloc` | memory |
| 0.53% | `python` | `_PyCode_New` | memory |

## richards

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 61.03% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.45% | `python` | `PyObject_GetAttr` | dynamic |
| 4.88% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 4.52% | `python` | `_PyObject_GetMethod` | dynamic |
| 3.69% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 1.24% | `python` | `PyObject_SetAttr` | dynamic |
| 1.06% | `python` | `long_dealloc` | memory |
| 0.97% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.70% | `python` | `type_new` | memory |
| 0.63% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.53% | `python` | `gc_collect_main` | gc |

## richards_super

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 53.88% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.66% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 4.53% | `python` | `PyObject_GetAttr` | dynamic |
| 3.80% | `python` | `_PyObject_GetMethod` | dynamic |
| 2.65% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 2.14% | `python` | `_PySuper_Lookup` | dynamic |
| 1.88% | `python` | `PyObject_SetAttr` | dynamic |
| 1.17% | `python` | `type_new` | memory |
| 1.06% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.87% | `python` | `long_dealloc` | memory |
| 0.81% | `python` | `gc_collect_main` | gc |
| 0.73% | `python` | `visit_decref` | gc |
| 0.66% | `python` | `deduce_unreachable` | unknown |
| 0.53% | `python` | `_PyCode_New` | memory |
| 0.52% | `python` | `visit_reachable` | gc |
| 0.52% | `python` | `_PyEvalFramePushAndInit` | interpreter |

## scimark

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 41.60% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.48% | `python` | `PyNumber_AsSsize_t` | dynamic |
| 4.25% | `python` | `long_dealloc` | memory |
| 3.62% | `array.cpython-313-x86_64-linux-gnu.so` | `array_subscr` | library |
| 3.11% | `python` | `_PyLong_Add` | int |
| 2.72% | `python` | `PyFloat_FromDouble` | float |
| 2.38% | `python` | `PyLong_FromLong` | int |
| 2.36% | `python` | `PyObject_GetItem` | dynamic |
| 2.00% | `python` | `vgetargs1_impl` | calls |
| 1.97% | `python` | `PyType_GetModuleByDef` | dynamic |
| 1.57% | `python` | `convertitem` | unknown |
| 1.55% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.41% | `array.cpython-313-x86_64-linux-gnu.so` | `array_ass_subscr` | library |
| 1.12% | `python` | `_PyLong_Multiply` | int |
| 1.05% | `python` | `object_isinstance` | dynamic |
| 0.95% | `python` | `PyObject_Free` | dynamic |
| 0.94% | `python` | `float_dealloc` | memory |
| 0.87% | `array.cpython-313-x86_64-linux-gnu.so` | `d_setitem` | library |
| 0.80% | `python` | `PyIndex_Check` | unknown |
| 0.73% | `python` | `PyArg_Parse` | calls |
| 0.73% | `python` | `_PyFloat_ExactDealloc` | memory |
| 0.62% | `python` | `PyObject_SetItem` | dynamic |
| 0.61% | `python` | `PyLong_AsDouble.part.0` | int |
| 0.53% | `python` | `tupledealloc` | memory |

## spectral_norm

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 35.65% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 9.21% | `python` | `_PyLong_Add` | int |
| 4.79% | `python` | `long_dealloc` | memory |
| 4.46% | `python` | `PyObject_Free` | dynamic |
| 3.86% | `python` | `enum_next` | miscobj |
| 3.85% | `python` | `long_div` | int |
| 3.77% | `python` | `_PyLong_Multiply` | int |
| 3.44% | `python` | `float_div` | float |
| 2.28% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.83% | `python` | `convert_to_double` | unknown |
| 1.68% | `python` | `PyNumber_TrueDivide` | dynamic |
| 1.08% | `python` | `type_new` | memory |
| 0.85% | `python` | `PyNumber_FloorDivide` | dynamic |
| 0.79% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.73% | `python` | `gc_collect_main` | gc |
| 0.71% | `python` | `deduce_unreachable` | unknown |
| 0.66% | `python` | `visit_decref` | gc |
| 0.55% | `python` | `float_dealloc` | memory |
| 0.51% | `python` | `_PyCode_New` | memory |

## sqlglot

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 33.87% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.99% | `python` | `object_isinstance` | dynamic |
| 2.41% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.34% | `python` | `tupledealloc` | memory |
| 1.70% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.53% | `python` | `type_new` | memory |
| 1.37% | `python` | `dictiter_iternextitem` | dict |
| 1.31% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 1.23% | `python` | `meth_dealloc` | memory |
| 1.20% | `python` | `method_get` | dynamic |
| 0.98% | `python` | `gen_dealloc` | memory |
| 0.97% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.96% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.95% | `python` | `gc_collect_main` | gc |
| 0.93% | `python` | `make_gen` | unknown |
| 0.92% | `python` | `deduce_unreachable` | unknown |
| 0.88% | `python` | `PyObject_IsInstance` | dynamic |
| 0.84% | `python` | `visit_decref` | gc |
| 0.78% | `python` | `dictiter_dealloc` | memory |
| 0.75% | `python` | `list_dealloc` | memory |
| 0.73% | `python` | `getset_get` | dynamic |
| 0.72% | `python` | `insert_to_emptydict` | dict |
| 0.71% | `python` | `_PyCode_New` | memory |
| 0.70% | `python` | `dict_items` | dict |
| 0.67% | `python` | `PyObject_GetAttr` | dynamic |
| 0.66% | `python` | `PyObject_GC_Del` | gc |
| 0.62% | `python` | `visit_reachable` | gc |
| 0.61% | `python` | `func_dealloc` | memory |
| 0.58% | `python` | `PyList_New` | memory |
| 0.56% | `python` | `dictview_dealloc` | memory |
| 0.55% | `python` | `slot_tp_hash` | unknown |
| 0.55% | `python` | `siphash13` | str |
| 0.53% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.52% | `python` | `unicode_dealloc` | memory |
| 0.52% | `python` | `dict_dealloc` | memory |
| 0.52% | `python` | `dict_get` | dict |
| 0.51% | `python` | `r_object` | import |
| 0.50% | `python` | `dictitems_iter` | unknown |

## sqlglot_optimize

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 33.19% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.30% | `python` | `object_isinstance` | dynamic |
| 2.21% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.09% | `python` | `tupledealloc` | memory |
| 1.60% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.54% | `python` | `dictiter_iternextitem` | dict |
| 1.51% | `python` | `meth_dealloc` | memory |
| 1.50% | `python` | `type_new` | memory |
| 1.37% | `python` | `method_get` | dynamic |
| 1.34% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 1.30% | `python` | `PyObject_GetAttr` | dynamic |
| 1.01% | `python` | `deduce_unreachable` | unknown |
| 1.00% | `python` | `gc_collect_main` | gc |
| 0.92% | `python` | `PyObject_IsInstance` | dynamic |
| 0.91% | `python` | `visit_decref` | gc |
| 0.89% | `python` | `list_dealloc` | memory |
| 0.87% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.87% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.73% | `python` | `getset_get` | dynamic |
| 0.67% | `python` | `visit_reachable` | gc |
| 0.65% | `python` | `dictiter_dealloc` | memory |
| 0.63% | `python` | `PyObject_GC_Del` | gc |
| 0.61% | `python` | `dict_dealloc` | memory |
| 0.60% | `python` | `dict_get` | dict |
| 0.59% | `python` | `PyList_New` | memory |
| 0.57% | `python` | `dict_items` | dict |
| 0.55% | `python` | `list_iter` | list |
| 0.55% | `python` | `siphash13` | str |
| 0.55% | `python` | `_PyCode_New` | memory |
| 0.54% | `python` | `slot_tp_hash` | unknown |
| 0.54% | `python` | `insert_to_emptydict` | dict |
| 0.54% | `python` | `make_gen` | unknown |
| 0.54% | `python` | `insertdict` | dict |
| 0.54% | `python` | `find_name_in_mro` | lookup |
| 0.52% | `python` | `tuplehash` | tuple |
| 0.52% | `python` | `unicode_dealloc` | memory |
| 0.52% | `python` | `func_dealloc` | memory |
| 0.51% | `python` | `r_object` | import |

## sqlglot_parse

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 49.17% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.99% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.63% | `python` | `PyObject_GetAttr` | dynamic |
| 1.34% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.32% | `python` | `gc_collect_main` | gc |
| 1.30% | `python` | `_Py_type_getattro` | lookup |
| 1.28% | `python` | `PyDict_Contains` | dict |
| 1.15% | `python` | `type_new` | memory |
| 1.11% | `python` | `visit_decref` | gc |
| 1.08% | `python` | `deduce_unreachable` | unknown |
| 0.86% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.84% | `python` | `PyObject_RichCompare` | dynamic |
| 0.81% | `python` | `dict_get` | dict |
| 0.80% | `python` | `long_dealloc` | memory |
| 0.77% | `python` | `tupledealloc` | memory |
| 0.75% | `python` | `_PyLong_Add` | int |
| 0.70% | `python` | `slot_tp_hash` | unknown |
| 0.67% | `python` | `PyObject_SetAttr` | dynamic |
| 0.65% | `python` | `object_new` | memory |
| 0.65% | `python` | `visit_reachable` | gc |
| 0.64% | `python` | `object_isinstance` | dynamic |
| 0.61% | `python` | `dict_dealloc` | memory |
| 0.55% | `python` | `subtype_traverse` | gc |
| 0.54% | `python` | `PyDict_SetItem` | dict |
| 0.52% | `python` | `insert_to_emptydict` | dict |

## sqlglot_transpile

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 42.83% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.93% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.64% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.57% | `python` | `type_new` | memory |
| 1.53% | `python` | `PyObject_GetAttr` | dynamic |
| 1.48% | `python` | `gc_collect_main` | gc |
| 1.31% | `python` | `deduce_unreachable` | unknown |
| 1.31% | `python` | `visit_decref` | gc |
| 1.05% | `python` | `_Py_type_getattro` | lookup |
| 0.99% | `python` | `dict_get` | dict |
| 0.98% | `python` | `find_name_in_mro` | lookup |
| 0.93% | `python` | `object_isinstance` | dynamic |
| 0.90% | `python` | `PyDict_Contains` | dict |
| 0.87% | `python` | `tupledealloc` | memory |
| 0.84% | `python` | `visit_reachable` | gc |
| 0.70% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.65% | `python` | `long_dealloc` | memory |
| 0.62% | `python` | `_PyCode_New` | memory |
| 0.61% | `python` | `dict_dealloc` | memory |
| 0.59% | `python` | `unicode_dealloc` | memory |
| 0.56% | `python` | `PyObject_RichCompare` | dynamic |
| 0.55% | `python` | `r_object` | import |
| 0.55% | `python` | `siphash13` | str |
| 0.52% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.51% | `python` | `subtype_traverse` | gc |

## sqlite_synth

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 11.66% | `libpthread-2.31.so` | `pthread_mutex_unlock` | library |
| 11.60% | `libpthread-2.31.so` | `__pthread_mutex_lock` | library |
| 9.82% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.45% | `python` | `PyEval_RestoreThread` | interpreter |
| 4.16% | `libsqlite3.so.0.8.6` | `sqlite3_reset` | library |
| 2.18% | `libm-2.31.so` | `f64xsubf128` | library |
| 1.50% | `libsqlite3.so.0.8.6` | `sqlite3_randomness` | library |
| 1.28% | `libc-2.31.so` | `pthread_cond_signal` | libc |
| 1.26% | `python` | `PyEval_SaveThread` | interpreter |
| 1.25% | `python` | `PyTuple_New` | memory |
| 1.20% | `python` | `tupledealloc` | memory |
| 1.07% | `python` | `long_dealloc` | memory |
| 1.01% | `_sqlite3.cpython-313-x86_64-linux-gnu.so` | `_pysqlite_query_execute` | library |
| 0.99% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.98% | `libsqlite3.so.0.8.6` | `sqlite3_value_double` | library |
| 0.91% | `libpthread-2.31.so` | `pthread_cond_signal@@GLIBC_2.3.2` | library |
| 0.83% | `python` | `long_to_decimal_string_internal` | int |
| 0.82% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.76% | `libsqlite3.so.0.8.6` | `sqlite3_extended_errcode` | library |
| 0.71% | `python` | `type_new` | memory |
| 0.71% | `libsqlite3.so.0.8.6` | `sqlite3_preupdate_old` | library |
| 0.70% | `python` | `list_dealloc` | memory |
| 0.68% | `libsqlite3.so.0.8.6` | `sqlite3_value_int64` | library |
| 0.65% | `libc-2.31.so` | `pthread_mutex_unlock` | libc |
| 0.63% | `libsqlite3.so.0.8.6` | `sqlite3_vtab_config` | library |
| 0.63% | `python` | `unicode_decode_utf8` | str |
| 0.61% | `python` | `PyFloat_AsDouble` | float |
| 0.60% | `libsqlite3.so.0.8.6` | `sqlite3_wal_checkpoint` | library |
| 0.59% | `libc-2.31.so` | `pthread_mutex_lock` | libc |
| 0.57% | `libsqlite3.so.0.8.6` | `sqlite3_step` | library |
| 0.55% | `python` | `object_new` | memory |
| 0.53% | `libsqlite3.so.0.8.6` | `sqlite3_enable_shared_cache` | library |
| 0.53% | `python` | `PyList_New` | memory |
| 0.52% | `python` | `_PyObject_Malloc` | memory |
| 0.52% | `python` | `unicode_dealloc` | memory |
| 0.50% | `python` | `gc_collect_main` | gc |

## sympy

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 29.30% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.38% | `python` | `tupledealloc` | memory |
| 2.24% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.04% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.61% | `python` | `PyObject_GetAttr` | dynamic |
| 1.31% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.24% | `python` | `type_new` | memory |
| 1.23% | `python` | `gc_collect_main` | gc |
| 1.17% | `python` | `deduce_unreachable` | unknown |
| 1.11% | `python` | `_Py_type_getattro` | lookup |
| 1.10% | `python` | `visit_decref` | gc |
| 1.07% | `python` | `_Py_dict_lookup` | lookup |
| 1.03% | `python` | `PyDict_SetItem` | dict |
| 0.94% | `python` | `PyDict_GetItemRef` | dict |
| 0.88% | `python` | `PyObject_RichCompare` | dynamic |
| 0.86% | `python` | `find_name_in_mro` | lookup |
| 0.85% | `python` | `object_isinstance` | dynamic |
| 0.83% | `python` | `_PyCode_New` | memory |
| 0.83% | `python` | `slot_tp_richcompare` | dynamic |
| 0.80% | `python` | `dict_dealloc` | memory |
| 0.75% | `python` | `visit_reachable` | gc |
| 0.73% | `python` | `method_get` | dynamic |
| 0.70% | `python` | `meth_dealloc` | memory |
| 0.70% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.69% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.68% | `python` | `list_dealloc` | memory |
| 0.64% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.61% | `python` | `r_object` | import |
| 0.59% | `python` | `_PyObject_GenericGetAttrWithDict` | dynamic |
| 0.57% | `python` | `setiter_iternext` | miscobj |
| 0.53% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.52% | `python` | `dict_merge` | dict |
| 0.50% | `python` | `PyObject_GC_Del` | gc |

## telco

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 15.71% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.26% | `python` | `PyType_GetModuleByDef` | dynamic |
| 4.18% | `python` | `PyObject_GC_Del` | gc |
| 3.38% | `python` | `_PyObject_GC_New` | gc |
| 2.44% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `_mpd_qaddsub` | library |
| 1.87% | `python` | `tupledealloc` | memory |
| 1.78% | `python` | `PyObject_GetAttr` | dynamic |
| 1.77% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `nm_mpd_qadd` | library |
| 1.74% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `nm_mpd_qmul` | library |
| 1.72% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.71% | `python` | `meth_dealloc` | memory |
| 1.71% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `_mpd_baseshiftr` | library |
| 1.70% | `python` | `PyTuple_New` | memory |
| 1.66% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `convert_op` | library |
| 1.59% | `python` | `PyContextVar_Get` | unknown |
| 1.51% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `_mpd_qmul` | library |
| 1.51% | `python` | `method_get` | dynamic |
| 1.41% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `mpd_qfinalize` | library |
| 1.37% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `mpd_qshiftr` | library |
| 1.16% | `python` | `vgetargskeywords.constprop.0` | calls |
| 1.11% | `python` | `_PyArg_UnpackKeywordsWithVararg` | calls |
| 1.08% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_mpd_qquantize` | library |
| 0.90% | `python` | `type_new` | memory |
| 0.88% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_dealloc` | library |
| 0.86% | `python` | `PyUnicode_New` | memory |
| 0.84% | `python` | `PyDict_GetItemRef` | dict |
| 0.75% | `python` | `method_vectorcall_VARARGS_KEYWORDS` | calls |
| 0.75% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `mpd_qquantize` | library |
| 0.74% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.70% | `python` | `vgetargs1_impl` | calls |
| 0.69% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_addstatus` | library |
| 0.68% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `PyDecType_New` | library |
| 0.67% | `python` | `gc_collect_main` | gc |
| 0.67% | `_struct.cpython-313-x86_64-linux-gnu.so` | `unpack` | library |
| 0.63% | `python` | `as_ucs4` | unknown |
| 0.62% | `python` | `visit_decref` | gc |
| 0.61% | `python` | `deduce_unreachable` | unknown |
| 0.61% | `python` | `unicode_dealloc` | memory |
| 0.55% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_str` | library |
| 0.53% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `current_context` | library |
| 0.51% | `python` | `_io_BytesIO_read` | unknown |
| 0.51% | `python` | `PyObject_Str` | dynamic |
| 0.51% | `python` | `_PyObject_MakeTpCall` | dynamic |

## thrift

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 22.95% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.23% | `python` | `subtype_dealloc` | memory |
| 2.14% | `python` | `object_new` | memory |
| 2.10% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::encodeValue` | library |
| 2.02% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.95% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.91% | `python` | `slot_tp_init` | unknown |
| 1.83% | `python` | `PyObject_GetAttr` | dynamic |
| 1.81% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.78% | `python` | `PyDict_SetItem` | dict |
| 1.75% | `python` | `insert_to_emptydict` | dict |
| 1.73% | `python` | `PyDict_GetItemRef` | dict |
| 1.61% | `python` | `_PyStack_UnpackDict` | unknown |
| 1.45% | `python` | `dict_dealloc` | memory |
| 1.37% | `python` | `tupledealloc` | memory |
| 1.33% | `python` | `PyUnicode_FromFormatV` | str |
| 1.28% | `python` | `PyObject_GC_Del` | gc |
| 1.21% | `python` | `type_new` | memory |
| 1.17% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 1.07% | `python` | `unicode_decode_utf8` | str |
| 1.06% | `python` | `insertdict` | dict |
| 1.02% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.82% | `python` | `PyMem_Free` | memory |
| 0.79% | `python` | `deduce_unreachable` | unknown |
| 0.78% | `python` | `PyObject_RichCompare` | dynamic |
| 0.77% | `python` | `_PySuper_Lookup` | dynamic |
| 0.77% | `python` | `gc_collect_main` | gc |
| 0.77% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::decodeValue` | library |
| 0.73% | `python` | `list_dealloc` | memory |
| 0.68% | `python` | `visit_decref` | gc |
| 0.68% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readStruct` | library |
| 0.67% | `python` | `_Py_dict_lookup` | lookup |
| 0.66% | `python` | `unicode_dealloc` | memory |
| 0.65% | `python` | `_Py_type_getattro` | lookup |
| 0.64% | `python` | `PyLong_AsLong` | int |
| 0.61% | `python` | `_PyObject_GenericGetAttrWithDict` | dynamic |
| 0.60% | `python` | `visit_reachable` | gc |
| 0.56% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readBytes` | library |
| 0.56% | `python` | `_PyCode_New` | memory |
| 0.53% | `python` | `PyUnicode_RichCompare` | str |
| 0.52% | `python` | `dictresize` | dict |
| 0.51% | `python` | `PyObject_GetOptionalAttr` | dynamic |

## tomli_loads

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 53.46% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.67% | `python` | `set_contains_lock_held` | miscobj |
| 4.67% | `python` | `_PyLong_Add` | int |
| 3.79% | `python` | `long_dealloc` | memory |
| 2.47% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.28% | `python` | `PyDict_GetItemRef` | dict |
| 2.03% | `python` | `PyDict_Contains` | dict |
| 1.97% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.23% | `python` | `_PyIncrementalNewlineDecoder_decode.cold` | memory |
| 1.05% | `python` | `tupledealloc` | memory |
| 0.81% | `python` | `object_isinstance` | dynamic |
| 0.76% | `python` | `PyObject_GetAttr` | dynamic |
| 0.65% | `python` | `PyUnicode_New` | memory |
| 0.64% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.62% | `python` | `_PyIncrementalNewlineDecoder_decode` | memory |
| 0.57% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.57% | `python` | `sre_ucs4_match` | library |
| 0.52% | `python` | `unicode_subscript` | str |

## tornado_http

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 28.22% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.03% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.00% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.84% | `python` | `type_new` | memory |
| 1.44% | `python` | `deduce_unreachable` | unknown |
| 1.38% | `python` | `tupledealloc` | memory |
| 1.33% | `python` | `gc_collect_main` | gc |
| 1.32% | `python` | `visit_decref` | gc |
| 1.05% | `python` | `visit_reachable` | gc |
| 0.91% | `python` | `PyObject_GetAttr` | dynamic |
| 0.86% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.77% | `python` | `PyDict_GetItemRef` | dict |
| 0.77% | `python` | `_PyCode_New` | memory |
| 0.69% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 0.65% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.59% | `python` | `r_object` | import |
| 0.57% | `python` | `find_name_in_mro` | lookup |
| 0.56% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.56% | `python` | `unicode_dealloc` | memory |
| 0.55% | `python` | `subtype_dealloc` | memory |
| 0.54% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.52% | `python` | `PyUnicode_FromKindAndData` | str |
| 0.52% | `python` | `PyObject_GC_Del` | gc |
| 0.51% | `python` | `list_dealloc` | memory |

## typing_runtime_protocols

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 31.76% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.55% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 2.90% | `python` | `_Py_dict_lookup` | lookup |
| 2.86% | `python` | `tupledealloc` | memory |
| 2.18% | `python` | `_Py_type_getattro` | lookup |
| 2.14% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.73% | `python` | `PyDict_Contains` | dict |
| 1.52% | `python` | `PyObject_GC_Del` | gc |
| 1.37% | `python` | `PyTraceBack_Here` | exceptions |
| 1.32% | `python` | `tuplehash` | tuple |
| 1.27% | `python` | `type_new` | memory |
| 1.21% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.18% | `python` | `_PyObject_GC_New` | gc |
| 1.17% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.12% | `python` | `frame_dealloc` | memory |
| 1.02% | `python` | `PySet_Contains` | unknown |
| 0.98% | `python` | `bounded_lru_cache_wrapper` | unknown |
| 0.98% | `python` | `getset_get` | dynamic |
| 0.91% | `python` | `_PyFrame_MakeAndSetFrameObject` | unknown |
| 0.86% | `python` | `PyObject_Vectorcall` | dynamic |
| 0.84% | `python` | `PyObject_GetAttr` | dynamic |
| 0.84% | `python` | `gc_collect_main` | gc |
| 0.79% | `python` | `tuple_iter` | tuple |
| 0.77% | `python` | `visit_decref` | gc |
| 0.76% | `python` | `deduce_unreachable` | unknown |
| 0.73% | `python` | `tuplecontains` | tuple |
| 0.66% | `python` | `_Py_type_getattro_impl` | dynamic |
| 0.66% | `python` | `PyObject_RichCompare` | dynamic |
| 0.66% | `python` | `_PyDict_GetItem_KnownHash` | dict |
| 0.61% | `python` | `PyArg_UnpackTuple` | calls |
| 0.60% | `python` | `method_dealloc` | memory |
| 0.60% | `python` | `wrap_descr_get` | unknown |
| 0.58% | `python` | `tb_dealloc` | memory |
| 0.57% | `python` | `_PyCode_New` | memory |
| 0.56% | `python` | `weakref_richcompare` | unknown |
| 0.55% | `python` | `visit_reachable` | gc |
| 0.53% | `python` | `tuplerichcompare` | tuple |
| 0.50% | `python` | `BaseException_new` | memory |

## unpack_sequence

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 81.93% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 0.81% | `python` | `type_new` | memory |
| 0.59% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.54% | `python` | `deduce_unreachable` | unknown |

## unpickle

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 14.96% | `python` | `unicode_decode_utf8` | str |
| 9.45% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `load` | library |
| 8.06% | `python` | `insertdict` | dict |
| 6.09% | `python` | `siphash13` | str |
| 5.33% | `python` | `unicode_dealloc` | memory |
| 4.50% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.43% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `load_counted_binunicode` | library |
| 2.75% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.64% | `python` | `dictresize` | dict |
| 2.00% | `python` | `dict_ass_sub` | dict |
| 1.70% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pdata_clear` | library |
| 1.68% | `python` | `dict_dealloc` | memory |
| 1.67% | `python` | `PyMem_Realloc` | memory |
| 1.55% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Unpickler_dealloc` | library |
| 1.27% | `python` | `PyObject_SetItem` | dynamic |
| 0.92% | `python` | `list_dealloc` | memory |
| 0.85% | `python` | `long_dealloc` | memory |
| 0.82% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pdata_push` | library |
| 0.82% | `python` | `PyLong_FromLong` | int |
| 0.81% | `python` | `type_new` | memory |
| 0.69% | `python` | `PyMem_Free` | memory |
| 0.66% | `python` | `unicode_hash` | str |
| 0.65% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `do_setitems.isra.0` | library |
| 0.65% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.60% | `python` | `gc_collect_main` | gc |
| 0.58% | `python` | `_PyObject_GC_New` | gc |
| 0.54% | `python` | `visit_decref` | gc |
| 0.51% | `python` | `deduce_unreachable` | unknown |

## unpickle_list

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 16.71% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `load` | library |
| 13.99% | `python` | `list_dealloc` | memory |
| 8.97% | `python` | `PyList_New` | memory |
| 5.99% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.46% | `python` | `PyList_SetSlice` | list |
| 5.21% | `python` | `PyLong_FromLong` | int |
| 4.44% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pdata_push` | library |
| 3.61% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `do_append.isra.0` | library |
| 2.47% | `python` | `_PyObject_Malloc` | memory |
| 1.86% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.66% | `python` | `list_resize` | list |
| 1.12% | `python` | `type_new` | memory |
| 0.94% | `python` | `PyMem_Realloc` | memory |
| 0.83% | `python` | `gc_collect_main` | gc |
| 0.79% | `python` | `visit_decref` | gc |
| 0.77% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005ba4` | library |
| 0.76% | `python` | `deduce_unreachable` | unknown |
| 0.59% | `python` | `_PyCode_New` | memory |
| 0.55% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Unpickler_dealloc` | library |
| 0.55% | `python` | `_PyObject_GC_New` | gc |
| 0.54% | `python` | `PyMem_Free` | memory |

## unpickle_pure_python

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 51.83% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.07% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.59% | `python` | `PyDict_GetItemRef` | dict |
| 2.15% | `python` | `_io_BytesIO_read` | unknown |
| 2.01% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.80% | `python` | `PyObject_IsTrue` | dynamic |
| 1.41% | `python` | `insertdict` | dict |
| 1.38% | `python` | `unicode_decode_utf8` | str |
| 1.19% | `python` | `tupledealloc` | memory |
| 1.15% | `python` | `unicode_new` | memory |
| 1.12% | `python` | `bytes_subscript` | str |
| 1.02% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.89% | `python` | `PyObject_GetItem` | dynamic |
| 0.86% | `python` | `type_new` | memory |
| 0.86% | `python` | `PyObject_Free` | dynamic |
| 0.85% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.67% | `python` | `PyObject_IsInstance` | dynamic |
| 0.65% | `python` | `visit_decref` | gc |
| 0.65% | `python` | `gc_collect_main` | gc |
| 0.61% | `python` | `deduce_unreachable` | unknown |
| 0.61% | `python` | `siphash13` | str |
| 0.57% | `python` | `unicode_dealloc` | memory |

## xml_etree

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.20% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.00% | `python` | `PyObject_GetAttr` | dynamic |
| 3.10% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `doContent` | library |
| 2.38% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `PyExpat_XML_Parse` | library |
| 1.96% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.93% | `python` | `_io_TextIOWrapper_write` | unknown |
| 1.87% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `normal_contentTok` | library |
| 1.85% | `python` | `unicode_decode_utf8` | str |
| 1.85% | `python` | `deduce_unreachable` | unknown |
| 1.74% | `python` | `visit_decref` | gc |
| 1.71% | `python` | `visit_reachable` | gc |
| 1.65% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `hash` | library |
| 1.59% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `storeAtts` | library |
| 1.55% | `python` | `unicode_dealloc` | memory |
| 1.49% | `python` | `gc_collect_main` | gc |
| 1.45% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `makeuniversal.isra.0` | library |
| 1.44% | `python` | `_PyObject_GC_New` | gc |
| 1.43% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.32% | `python` | `PyObject_GC_Del` | gc |
| 1.31% | `python` | `PyUnicode_Concat` | str |
| 1.27% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 1.11% | `python` | `object_isinstance` | dynamic |
| 1.10% | `python` | `tupledealloc` | memory |
| 0.94% | `python` | `long_to_decimal_string_internal` | int |
| 0.94% | `python` | `PyBytes_FromStringAndSize` | str |
| 0.92% | `python` | `list_dealloc` | memory |
| 0.92% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.89% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `elementiter_next` | library |
| 0.88% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `element_gc_traverse` | library |
| 0.86% | `python` | `PyUnicode_Format` | str |
| 0.75% | `python` | `PyDict_GetItemWithError` | dict |
| 0.74% | `python` | `PyUnicode_Contains` | str |
| 0.69% | `python` | `getset_get` | dynamic |
| 0.69% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `element_dealloc` | library |
| 0.68% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `treebuilder_handle_start` | library |
| 0.66% | `python` | `PyObject_Free` | dynamic |
| 0.65% | `python` | `siphash13` | str |
| 0.63% | `python` | `vgetargs1_impl` | calls |
| 0.61% | `python` | `type_new` | memory |
| 0.61% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.54% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `treebuilder_handle_end.isra.0` | library |
| 0.54% | `python` | `BaseException_new` | memory |
| 0.53% | `python` | `list_vectorcall` | list |
| 0.52% | `python` | `_PyEvalFramePushAndInit` | interpreter |


## Categories

### interpreter

32.13% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 29.41% | python | _PyEval_EvalFrameDefault |
| 1.79% | python | _PyEval_FrameClearAndPop |
| 0.36% | python | _PyEvalFramePushAndInit |
| 0.12% | python | _PyEval_EvalFrameDefault.cold |
| 0.10% | python | PyEval_RestoreThread |
| 0.08% | python | _PyPegen_fill_token |
| 0.08% | python | _PyFrame_ClearExceptCode |
| 0.03% | python | intern_string_constants |
| 0.03% | python | PyEval_SaveThread |
| 0.03% | python | _PyPegen_update_memo |
| 0.02% | python | _PyPegen_name_token |
| 0.02% | python | _PyCode_Validate |
| 0.01% | python | _PyPegen_Parser_Free |
| 0.01% | python | PyEval_GetFrame |

### library

10.31% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 1.68% | python | sre_ucs1_match |
| 1.34% | _pickle.cpython-313-x86_64-linux-gnu.so | save |
| 0.76% | libz.so.1.2.11 | crc32_combine64 |
| 0.74% | python | sre_ucs2_charset.isra.0 |
| 0.46% | _json.cpython-313-x86_64-linux-gnu.so | _parse_object_unicode |
| 0.31% | _pickle.cpython-313-x86_64-linux-gnu.so | load |
| 0.28% | libz.so.1.2.11 | inflateBackEnd |
| 0.28% | _pickle.cpython-313-x86_64-linux-gnu.so | _Pickler_Write |
| 0.25% | _pickle.cpython-313-x86_64-linux-gnu.so | memo_put.isra.0 |
| 0.21% | python | sre_search |
| 0.20% | libpthread-2.31.so | __pthread_mutex_lock |
| 0.19% | libpthread-2.31.so | pthread_mutex_unlock |
| 0.15% | python | sre_ucs1_count |
| 0.13% | libm-2.31.so | f64xsubf128 |
| 0.13% | ld-2.31.so | _dl_rtld_di_serinfo |
| 0.13% | python | _sre_SRE_Pattern_match |
| 0.10% | _json.cpython-313-x86_64-linux-gnu.so | encoder_encode_key_value |
| 0.09% | tracer.cpython-313-x86_64-linux-gnu.so | CTracer_trace |
| 0.08% | _pickle.cpython-313-x86_64-linux-gnu.so | _Pickler_write_bytes |
| 0.07% | libpython3.11.so.1.0 | _PyEval_EvalFrameDefault |
| 0.06% | _pickle.cpython-313-x86_64-linux-gnu.so | Pdata_push |
| 0.06% | _asyncio.cpython-313-x86_64-linux-gnu.so | TaskObj_traverse |
| 0.06% | _pickle.cpython-313-x86_64-linux-gnu.so | Pickler_dealloc |
| 0.05% | libsqlite3.so.0.8.6 | sqlite3_reset |
| 0.05% | _pickle.cpython-313-x86_64-linux-gnu.so | load_counted_binunicode |
| 0.05% | libmagic.so.1.0.0 | 0x000000000000f936 |
| 0.04% | _pickle.cpython-313-x86_64-linux-gnu.so | do_append.isra.0 |
| 0.04% | array.cpython-313-x86_64-linux-gnu.so | array_subscr |
| 0.04% | libz.so.1.2.11 | inflateCodesUsed |
| 0.04% | ld-2.31.so | _dl_catch_error |
| 0.04% | pyexpat.cpython-313-x86_64-linux-gnu.so | doContent |
| 0.04% | libm-2.31.so | __fmod_finite |
| 0.03% | _json.cpython-313-x86_64-linux-gnu.so | py_encode_basestring_ascii |
| 0.03% | _pickle.cpython-313-x86_64-linux-gnu.so | memo_get.isra.0 |
| 0.03% | _json.cpython-313-x86_64-linux-gnu.so | _match_number_unicode.isra.0 |
| 0.03% | python | pattern_subx |
| 0.03% | libmagic.so.1.0.0 | 0x000000000000f932 |
| 0.03% | _decimal.cpython-313-x86_64-linux-gnu.so | _mpd_qaddsub |
| 0.03% | pyexpat.cpython-313-x86_64-linux-gnu.so | PyExpat_XML_Parse |
| 0.03% | _pickle.cpython-313-x86_64-linux-gnu.so | Unpickler_dealloc |
| 0.02% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::encodeValue |
| 0.02% | libpthread-2.31.so | pthread_cond_signal@@GLIBC_2.3.2 |
| 0.02% | pyexpat.cpython-313-x86_64-linux-gnu.so | normal_contentTok |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | nm_mpd_qadd |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | nm_mpd_qmul |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | _mpd_baseshiftr |
| 0.02% | _pickle.cpython-313-x86_64-linux-gnu.so | Pdata_clear |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | convert_op |
| 0.02% | pyexpat.cpython-313-x86_64-linux-gnu.so | hash |
| 0.02% | _asyncio.cpython-313-x86_64-linux-gnu.so | task_step_impl |
| 0.02% | libz.so.1.2.11 | inflate |
| 0.02% | pyexpat.cpython-313-x86_64-linux-gnu.so | storeAtts |
| 0.02% | libsqlite3.so.0.8.6 | sqlite3_randomness |
| 0.02% | libsqlite3.so.0.8.6 | sqlite3_exec |
| 0.02% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005cd4 |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | _mpd_qmul |
| 0.02% | array.cpython-313-x86_64-linux-gnu.so | array_ass_subscr |
| 0.02% | libpython3.11.so.1.0 | _PyDict_GetItem_KnownHash |
| 0.02% | _elementtree.cpython-313-x86_64-linux-gnu.so | makeuniversal.isra.0 |
| 0.02% | _heapq.cpython-313-x86_64-linux-gnu.so | _heapq_heappop |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | mpd_qfinalize |
| 0.02% | _asyncio.cpython-313-x86_64-linux-gnu.so | TaskStepMethWrapper_traverse |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | mpd_qshiftr |
| 0.02% | python | sre_ucs1_match.cold |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | factorial_partial_product |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | TaskObj_clear |
| 0.01% | _json.cpython-313-x86_64-linux-gnu.so | _parse_array_unicode |
| 0.01% | libpython3.11.so.1.0 | PyObject_Malloc |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_value_double |
| 0.01% | _bisect.cpython-313-x86_64-linux-gnu.so | _bisect_bisect_right |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_mpd_qquantize |
| 0.01% | libpython3.11.so.1.0 | deduce_unreachable |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | element_gc_traverse |
| 0.01% | _sqlite3.cpython-313-x86_64-linux-gnu.so | _pysqlite_query_execute |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | FutureObj_traverse |
| 0.01% | libpython3.11.so.1.0 | visit_decref |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_str_value |
| 0.01% | libpthread-2.31.so | sem_post@@GLIBC_2.2.5 |
| 0.01% | _struct.cpython-313-x86_64-linux-gnu.so | unpack |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | elementiter_next |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_dealloc |
| 0.01% | array.cpython-313-x86_64-linux-gnu.so | d_setitem |
| 0.01% | libssl.so.1.1 | SSL_rstate_string |
| 0.01% | libpython3.11.so.1.0 | type_new |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | math_factorial |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005e54 |
| 0.01% | libpython3.11.so.1.0 | PyDict_SetDefault |
| 0.01% | libpthread-2.31.so | sem_trywait@@GLIBC_2.2.5 |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | _pickle_loads |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005ba4 |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | _asyncio_Future_add_done_callback |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_extended_errcode |
| 0.01% | libpython3.11.so.1.0 | visit_reachable |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | _pickle_dumps |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | _asyncio_Task___init__ |
| 0.01% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::decodeValue |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | element_dealloc |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005fc4 |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | mpd_qquantize |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_preupdate_old |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | future_init |
| 0.01% | libpython3.11.so.1.0 | gc_collect_main |
| 0.01% | libpython3.11.so.1.0 | r_object |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_value_int64 |
| 0.01% | _struct.cpython-313-x86_64-linux-gnu.so | s_pack |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_addstatus |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | PyDecType_New |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | treebuilder_handle_start |
| 0.01% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readStruct |
| 0.01% | python | _sre_SRE_Pattern_search |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | do_setitems.isra.0 |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_vtab_config |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_wal_checkpoint |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | math_sqrt |
| 0.01% | libpython3.11.so.1.0 | PyObject_Free |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_step |
| 0.01% | _json.cpython-313-x86_64-linux-gnu.so | encoder_listencode_obj |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | call_soon |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | task_step |
| 0.01% | python | sre_ucs4_match |
| 0.01% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readBytes |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_enable_shared_cache |
| 0.01% | libm-2.31.so | pow |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_str |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | treebuilder_handle_end.isra.0 |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | current_context |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | FutureIter_traverse |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | FutureObj_clear |
| 0.01% | ld-2.31.so | _dl_debug_state |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_mutex_try |

### memory

10.08% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.98% | python | type_new |
| 0.86% | python | tupledealloc |
| 0.82% | python | list_dealloc |
| 0.69% | python | long_dealloc |
| 0.57% | python | unicode_dealloc |
| 0.45% | python | _PyCode_New |
| 0.37% | python | dict_dealloc |
| 0.37% | python | subtype_dealloc |
| 0.35% | python | gen_dealloc |
| 0.26% | python | PyList_New |
| 0.25% | python | PyMem_Free |
| 0.24% | python | meth_dealloc |
| 0.23% | python | PyFunction_NewWithQualName |
| 0.21% | python | object_new |
| 0.21% | python | _PyObject_Malloc |
| 0.20% | python | _PyLong_New |
| 0.19% | python | PyMem_Malloc |
| 0.17% | python | PyType_GenericAlloc |
| 0.16% | python | PyUnicode_New |
| 0.15% | python | func_dealloc |
| 0.14% | python | method_dealloc |
| 0.13% | python | set_dealloc |
| 0.12% | python | code_dealloc |
| 0.11% | python | frame_dealloc |
| 0.11% | python | BaseException_new |
| 0.11% | python | PyTuple_New |
| 0.10% | python | PyMem_Realloc |
| 0.09% | python | float_dealloc |
| 0.09% | python | slice_dealloc |
| 0.06% | python | StopIteration_dealloc |
| 0.06% | python | listiter_dealloc |
| 0.06% | python | list_new_prealloc |
| 0.06% | python | _Py_Dealloc |
| 0.06% | python | allocate_from_new_pool |
| 0.05% | python | dictiter_dealloc |
| 0.04% | python | PyType_GenericNew |
| 0.04% | python | BaseException_dealloc |
| 0.04% | python | tb_dealloc |
| 0.04% | python | _PyObject_Free |
| 0.04% | python | make_new_set |
| 0.04% | python | range_dealloc |
| 0.04% | python | cell_dealloc |
| 0.04% | python | tp_new_wrapper |
| 0.03% | python | slot_tp_new |
| 0.03% | python | dictview_dealloc |
| 0.03% | python | context_tp_dealloc |
| 0.03% | python | PySlice_New |
| 0.03% | python | weakref_dealloc |
| 0.02% | python | tupleiter_dealloc |
| 0.02% | python | _PyObject_New |
| 0.02% | python | match_dealloc |
| 0.02% | python | _PyIncrementalNewlineDecoder_decode.cold |
| 0.02% | python | unicode_new |
| 0.02% | python | _PyFloat_ExactDealloc |
| 0.02% | python | async_gen_asend_dealloc |
| 0.02% | python | async_gen_wrapped_val_dealloc |
| 0.02% | python | object_dealloc |
| 0.02% | python | _Py_NewReference |
| 0.02% | python | async_gen_asend_new |
| 0.02% | python | _PyAsyncGenValueWrapperNew |
| 0.02% | python | weakref___new__ |
| 0.02% | python | structseq_dealloc |
| 0.01% | python | PyCMethod_New |
| 0.01% | python | PyDict_New |
| 0.01% | python | PyObject_CallFinalizerFromDealloc |
| 0.01% | python | PyWeakref_NewRef |
| 0.01% | python | _PyIncrementalNewlineDecoder_decode |
| 0.01% | python | AttributeError_dealloc |
| 0.01% | python | descr_dealloc |
| 0.01% | python | _PyTokenizer_translate_newlines.constprop.0 |
| 0.01% | python | pattern_new_match.isra.0 |
| 0.01% | python | _PyObject_Realloc |
| 0.01% | python | reversed_new_impl |
| 0.01% | python | _PyMem_RawMalloc |
| 0.01% | python | zip_new |

### gc

8.95% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 2.92% | python | gc_collect_main |
| 1.85% | python | visit_decref |
| 1.74% | python | visit_reachable |
| 0.48% | python | PyObject_GC_Del |
| 0.44% | python | subtype_traverse |
| 0.29% | python | dict_traverse |
| 0.28% | python | _PyObject_GC_New |
| 0.25% | python | list_traverse |
| 0.13% | python | set_traverse |
| 0.11% | python | func_traverse |
| 0.11% | python | _PyObject_GC_NewVar |
| 0.10% | python | gen_traverse |
| 0.06% | python | type_traverse |
| 0.03% | python | meth_traverse |
| 0.03% | python | PyObject_GC_UnTrack |
| 0.02% | python | gc_traverse |
| 0.02% | python | PyObject_GC_Track |
| 0.02% | python | context_tp_traverse |
| 0.02% | python | frame_traverse |
| 0.01% | python | descr_traverse |
| 0.01% | python | module_traverse |
| 0.01% | python | method_traverse |
| 0.01% | python | cell_traverse |

### unknown

6.88% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 1.96% | python | deduce_unreachable |
| 0.29% | python | make_gen |
| 0.22% | python | slot_tp_init |
| 0.10% | python | clear_slots |
| 0.09% | python | func_descr_get |
| 0.09% | python | _PyStack_UnpackDict |
| 0.08% | python | _PyFrame_MakeAndSetFrameObject |
| 0.08% | python | method_vectorcall |
| 0.08% | python | _PyBuildSlice_Consume2 |
| 0.07% | python | gen_iternext |
| 0.06% | python | memset@plt |
| 0.06% | python | memcpy@plt |
| 0.06% | python | call_instrumentation_vector |
| 0.06% | python | range_vectorcall |
| 0.06% | python | convert_to_double |
| 0.05% | python | _stringio_readline.cold |
| 0.05% | python | range_iter |
| 0.05% | python | builtin_min |
| 0.04% | python | as_ucs4 |
| 0.04% | python | builtin_hasattr |
| 0.04% | python | path_converter |
| 0.04% | python | _PyCfg_OptimizeCodeUnit.constprop.0 |
| 0.04% | python | slot_tp_hash |
| 0.04% | python | dictkeys_decref.part.0 |
| 0.04% | python | _Py_module_getattro |
| 0.04% | python | PySys_Audit |
| 0.04% | python | PySet_Add |
| 0.03% | python | ucs4lib_find_max_char |
| 0.03% | python | _io_BytesIO_read |
| 0.03% | [vdso] | __vdso_clock_gettime |
| 0.03% | python | member_get |
| 0.03% | python | gen_send_ex2 |
| 0.03% | python | dictitems_iter |
| 0.03% | python | state_init |
| 0.03% | python | call_one_instrument |
| 0.03% | python | vectorcall_maybe.constprop.0 |
| 0.03% | python | async_gen_asend_send |
| 0.03% | python | os_listdir |
| 0.03% | python | gen_send_ex |
| 0.03% | python | _Py_VaBuildStack.constprop.0 |
| 0.03% | python | cm_descr_get |
| 0.03% | python | _PyAssemble_MakeCodeObject |
| 0.02% | python | hashtable_unicode_hash |
| 0.02% | python | term_raw |
| 0.02% | python | slot_mp_ass_subscript |
| 0.02% | python | range_subscript |
| 0.02% | python | builtin_id |
| 0.02% | python | _io_TextIOWrapper_write |
| 0.02% | python | bitwise_xor_rule |
| 0.02% | python | code_hash |
| 0.02% | python | builtin___import__ |
| 0.02% | python | bounded_lru_cache_wrapper |
| 0.02% | python | vgetargs1_impl.cold |
| 0.02% | python | unsafe_tuple_compare |
| 0.02% | python | hashtable_unicode_compare |
| 0.02% | python | Py_XDECREF.lto_priv.1 |
| 0.02% | python | convertitem |
| 0.02% | python | builtin_sum |
| 0.02% | python | slot_mp_subscript |
| 0.02% | python | _Py_hashtable_get_entry_generic |
| 0.02% | python | binary_op1 |
| 0.02% | python | PyContextVar_Get |
| 0.02% | python | wrapperdescr_call |
| 0.02% | python | binary_op |
| 0.02% | python | _PyModule_ClearDict |
| 0.02% | python | _PyCfg_OptimizedCfgToInstructionSequence |
| 0.02% | python | PySet_Contains |
| 0.02% | python | _Py_slot_tp_getattr_hook |
| 0.02% | python | _PyCoro_GetAwaitableIter |
| 0.02% | python | member_set |
| 0.02% | python | build_indices_generic |
| 0.02% | python | make_range_object |
| 0.02% | python | classmethod_get |
| 0.02% | python | atom_rule |
| 0.02% | python | ScandirIterator_iternext |
| 0.02% | python | async_gen_unwrap_value.isra.0 |
| 0.02% | python | do_mktuple |
| 0.02% | python | _PyDictKeys_StringLookup |
| 0.02% | python | memcmp@plt |
| 0.02% | python | Py_XDECREF.lto_priv.6 |
| 0.02% | python | write_bytes |
| 0.02% | python | shift_expr_rule |
| 0.01% | python | _PyBytes_Resize |
| 0.01% | python | slot_sq_contains |
| 0.01% | python | _PyThreadState_GetCurrent |
| 0.01% | python | builtin_issubclass |
| 0.01% | python | sum_rule |
| 0.01% | python | _PyGen_FetchStopIterationValue.cold |
| 0.01% | python | primary_raw |
| 0.01% | python | call_trace_func.isra.0 |
| 0.01% | python | expression_rule |
| 0.01% | python | va_build_value |
| 0.01% | python | ins1 |
| 0.01% | python | get_type_attr_as_size |
| 0.01% | python | _Py_bytes_lower |
| 0.01% | python | PyIndex_Check |
| 0.01% | python | _add_methods_to_object |
| 0.01% | python | builtin_sorted |
| 0.01% | python | lookup_maybe_method |
| 0.01% | python | symtable_add_def_helper |
| 0.01% | python | _io_open |
| 0.01% | python | _PyCode_GetCode |
| 0.01% | python | context_run |
| 0.01% | python | slot_sq_item |
| 0.01% | python | builtin_max |
| 0.01% | python | _Py_call_instrumentation_jump |
| 0.01% | python | pthread_self@plt |
| 0.01% | python | ascii_upper_or_lower |
| 0.01% | python | mro_implementation_unlocked |
| 0.01% | python | PyTime_AsSecondsDouble |
| 0.01% | python | inversion_rule |
| 0.01% | python | fill_time |
| 0.01% | python | builtin_hash |
| 0.01% | python | _PyType_FromMetaclass_impl |
| 0.01% | python | map_next |
| 0.01% | python | _PyGen_SetStopIterationValue |
| 0.01% | python | clear_weakref |
| 0.01% | python | lru_cache_make_key |
| 0.01% | python | assign_version_tag |
| 0.01% | python | weakref_richcompare |
| 0.01% | python | _getbytevalue |
| 0.01% | python | PyThread_acquire_lock_timed |
| 0.01% | python | builtin_any |
| 0.01% | python | _copy_characters |
| 0.01% | python | astfold_expr |
| 0.01% | python | unsafe_latin_compare |
| 0.01% | python | symtable_visit_expr |
| 0.01% | python | sm_descr_get |
| 0.01% | python | update_slots_callback |
| 0.01% | python | _PyContext_Exit |
| 0.01% | python | compiler_nameop |
| 0.01% | python | frozenset_vectorcall |
| 0.01% | python | weakref_hash |
| 0.01% | python | instr_sequence_to_cfg |
| 0.01% | python | update_slot |
| 0.01% | python | unsafe_long_compare |
| 0.01% | python | wrapper_call |
| 0.01% | python | new_dict |
| 0.01% | python | _Py_call_instrumentation_arg |
| 0.01% | python | zip_next |
| 0.01% | python | 0x000000000007e720 |
| 0.01% | python | make_dict_from_instance_attributes |
| 0.01% | python | islice_next |
| 0.01% | python | _PyLexer_update_fstring_expr |
| 0.01% | python | _PyGen_yf |
| 0.01% | python | _Py_module_getattro_impl.part.0 |
| 0.01% | python | _abc__abc_instancecheck |
| 0.01% | python | binary_iop1 |
| 0.01% | python | map_vectorcall |
| 0.01% | python | pthread_mutex_unlock@plt |
| 0.01% | python | bitwise_or_rule |
| 0.01% | python | wrap_descr_get |
| 0.01% | python | compiler_visit_expr1 |
| 0.01% | python | analyze_block |
| 0.01% | python | _io_FileIO___init__ |
| 0.01% | python | pytime_divide |
| 0.01% | python | super_getattro |
| 0.01% | python | slot_tp_iter |
| 0.01% | python | _PyCfg_ToInstructionSequence |
| 0.01% | python | subtype_clear |
| 0.01% | python | Py_UNICODE_ISALNUM.lto_priv.1 |
| 0.01% | python | _Py_dg_dtoa |
| 0.01% | python | simple_stmt_rule |
| 0.01% | python | PyThread_get_thread_ident_ex |
| 0.01% | python | ucs4lib_utf8_decode |
| 0.01% | python | stringio_iternext |
| 0.01% | python | _PyBytes_FromList |
| 0.01% | python | strlen@plt |
| 0.01% | python | write_str |
| 0.01% | python | _Py_SourceAsString |
| 0.01% | python | binary_iop |
| 0.01% | python | iter_iternext |
| 0.01% | python | unsafe_object_compare |

### dynamic

5.79% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.75% | python | PyObject_GetAttr |
| 0.36% | python | _PyObject_GetMethod |
| 0.36% | python | object_isinstance |
| 0.33% | python | _PyObject_MakeTpCall |
| 0.28% | python | PyObject_Free |
| 0.20% | python | PyObject_SetAttr |
| 0.19% | python | method_get |
| 0.16% | python | _PySuper_Lookup |
| 0.16% | python | PyObject_RichCompare |
| 0.15% | python | PyNumber_AsSsize_t |
| 0.15% | python | PyObject_Vectorcall |
| 0.14% | python | PyType_GetModuleByDef |
| 0.13% | python | PyObject_VectorcallMethod |
| 0.13% | python | type_ready |
| 0.12% | python | PyObject_IsTrue |
| 0.12% | python | _PyObject_LookupSpecial |
| 0.11% | python | PyObject_GetItem |
| 0.09% | python | PyObject_GetIter |
| 0.09% | python | getset_get |
| 0.09% | python | _PyObject_GenericGetAttrWithDict |
| 0.08% | python | type_call |
| 0.08% | python | PyObject_IsInstance |
| 0.08% | python | PyObject_Hash |
| 0.07% | python | PyObject_GetOptionalAttr |
| 0.06% | python | _Py_type_getattro_impl |
| 0.06% | python | PyObject_Str |
| 0.06% | python | slot_tp_richcompare |
| 0.06% | python | PyObject_SetItem |
| 0.06% | python | _PyObject_InitInlineValues |
| 0.05% | python | PyMapping_GetOptionalItem |
| 0.05% | python | _PyObject_Call |
| 0.05% | python | _PyObject_ClearFreeLists |
| 0.05% | python | PyObject_SetAttrString |
| 0.05% | python | PyObject_CallOneArg |
| 0.04% | python | _PyObject_VectorcallTstate.lto_priv.5 |
| 0.04% | python | PyNumber_TrueDivide |
| 0.04% | python | PyNumber_Multiply |
| 0.04% | python | PyType_IsSubtype |
| 0.04% | python | PyNumber_Add |
| 0.03% | python | StopIteration_init |
| 0.03% | python | PyNumber_And |
| 0.03% | python | PyNumber_Subtract |
| 0.03% | python | PyObject_GenericGetAttr |
| 0.03% | python | PyIter_Send |
| 0.02% | python | PySequence_Tuple |
| 0.02% | python | PyObject_RichCompareBool |
| 0.02% | python | PyObject_VisitManagedDict |
| 0.02% | python | PySequence_List |
| 0.02% | python | PyNumber_Remainder |
| 0.02% | python | PyObject_LengthHint |
| 0.02% | python | PyNumber_FloorDivide |
| 0.01% | python | object_get_class |
| 0.01% | python | PyObject_CallFunction |
| 0.01% | python | PyObject_ClearManagedDict |
| 0.01% | python | PyNumber_Rshift |
| 0.01% | python | PyObject_ClearWeakRefs |
| 0.01% | python | _PyNumber_Index |
| 0.01% | python | object_richcompare |
| 0.01% | python | PyIter_Next |
| 0.01% | python | _PyNumber_PowerNoMod |
| 0.01% | python | PyNumber_Negative |
| 0.01% | python | delitem_common |
| 0.01% | python | object_recursive_isinstance.part.0 |
| 0.01% | python | object_hash |
| 0.01% | python | type_dealloc_common |
| 0.01% | python | object_vacall |
| 0.01% | python | PyNumber_InPlaceAdd |
| 0.01% | python | _PyObject_GenericSetAttrWithDict |
| 0.01% | python | PyObject_CallMethodObjArgs |
| 0.01% | python | PyObject_GetBuffer |
| 0.01% | python | object_init |
| 0.01% | python | PyNumber_Index |
| 0.01% | python | PyObject_DelItem |
| 0.01% | python | PyObject_SelfIter |
| 0.01% | python | object___reduce_ex__ |

### kernel

4.62% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.63% | [kernel.kallsyms] | copy_user_enhanced_fast_string |
| 0.26% | [kernel.kallsyms] | clear_page_erms |
| 0.13% | [kernel.kallsyms] | native_irq_return_iret |
| 0.10% | [kernel.kallsyms] | __d_lookup_rcu |
| 0.09% | [kernel.kallsyms] | sync_regs |
| 0.08% | [kernel.kallsyms] | rmqueue |
| 0.08% | [kernel.kallsyms] | _raw_spin_lock |
| 0.07% | [kernel.kallsyms] | zap_pte_range.isra.0 |
| 0.06% | [kernel.kallsyms] | memset_erms |
| 0.06% | [kernel.kallsyms] | free_pcppages_bulk |
| 0.05% | [kernel.kallsyms] | __handle_mm_fault |
| 0.05% | [kernel.kallsyms] | filemap_map_pages |
| 0.04% | [kernel.kallsyms] | try_charge |
| 0.04% | [kernel.kallsyms] | smp_call_function_single |
| 0.04% | [kernel.kallsyms] | release_pages |
| 0.04% | [kernel.kallsyms] | link_path_walk.part.0 |
| 0.04% | [kernel.kallsyms] | get_mem_cgroup_from_mm |
| 0.04% | [kernel.kallsyms] | __pagevec_lru_add_fn |
| 0.03% | [kernel.kallsyms] | kmem_cache_alloc |
| 0.03% | [kernel.kallsyms] | syscall_return_via_sysret |
| 0.03% | [kernel.kallsyms] | mem_cgroup_throttle_swaprate |
| 0.03% | [kernel.kallsyms] | ext4_htree_store_dirent |
| 0.03% | [kernel.kallsyms] | handle_mm_fault |
| 0.03% | [kernel.kallsyms] | __ext4fs_dirhash |
| 0.03% | [kernel.kallsyms] | mem_cgroup_try_charge |
| 0.03% | [kernel.kallsyms] | __alloc_pages_nodemask |
| 0.02% | [kernel.kallsyms] | page_remove_rmap |
| 0.02% | [kernel.kallsyms] | strncpy_from_user |
| 0.02% | [kernel.kallsyms] | kmem_cache_free |
| 0.02% | [kernel.kallsyms] | kfree |
| 0.02% | [kernel.kallsyms] | filldir64 |
| 0.02% | [kernel.kallsyms] | entry_SYSCALL_64 |
| 0.02% | [kernel.kallsyms] | perf_event_alloc |
| 0.02% | [kernel.kallsyms] | copy_page |
| 0.02% | [kernel.kallsyms] | inode_permission |
| 0.02% | [kernel.kallsyms] | find_get_entry |
| 0.02% | [kernel.kallsyms] | memcg_kmem_get_cache |
| 0.02% | [kernel.kallsyms] | lookup_fast |
| 0.02% | [kernel.kallsyms] | __virt_addr_valid |
| 0.02% | [kernel.kallsyms] | find_vma |
| 0.02% | [kernel.kallsyms] | do_syscall_64 |
| 0.02% | [kernel.kallsyms] | do_user_addr_fault |
| 0.02% | [kernel.kallsyms] | _raw_spin_lock_irqsave |
| 0.02% | [kernel.kallsyms] | do_anonymous_page |
| 0.02% | [kernel.kallsyms] | prep_new_page |
| 0.02% | [kernel.kallsyms] | generic_permission |
| 0.02% | [kernel.kallsyms] | rb_insert_color |
| 0.02% | [kernel.kallsyms] | walk_component |
| 0.02% | [kernel.kallsyms] | __slab_free |
| 0.02% | [kernel.kallsyms] | get_page_from_freelist |
| 0.02% | [kernel.kallsyms] | str2hashbuf_signed |
| 0.02% | [kernel.kallsyms] | memcpy_erms |
| 0.02% | [kernel.kallsyms] | vmacache_find |
| 0.01% | [kernel.kallsyms] | error_entry |
| 0.01% | [kernel.kallsyms] | __count_memcg_events |
| 0.01% | [kernel.kallsyms] | __fget_light |
| 0.01% | [kernel.kallsyms] | page_fault |
| 0.01% | [kernel.kallsyms] | ext4_getattr |
| 0.01% | [kernel.kallsyms] | __mod_memcg_state |
| 0.01% | [kernel.kallsyms] | psi_task_change |
| 0.01% | [kernel.kallsyms] | perf_iterate_ctx |
| 0.01% | [kernel.kallsyms] | mutex_lock |
| 0.01% | [kernel.kallsyms] | rb_next |
| 0.01% | [kernel.kallsyms] | __mod_lruvec_state |
| 0.01% | [kernel.kallsyms] | security_inode_getattr |
| 0.01% | [kernel.kallsyms] | entry_SYSCALL_64_after_hwframe |
| 0.01% | [kernel.kallsyms] | generic_file_buffered_read |
| 0.01% | [kernel.kallsyms] | xas_load |
| 0.01% | [kernel.kallsyms] | _cond_resched |
| 0.01% | [kernel.kallsyms] | tcp_sendmsg_locked |
| 0.01% | [kernel.kallsyms] | mutex_unlock |
| 0.01% | [kernel.kallsyms] | __check_object_size |
| 0.01% | [kernel.kallsyms] | fsnotify |
| 0.01% | [kernel.kallsyms] | up_read |
| 0.01% | [kernel.kallsyms] | page_add_file_rmap |
| 0.01% | [kernel.kallsyms] | vsnprintf |
| 0.01% | [kernel.kallsyms] | set_root |
| 0.01% | [kernel.kallsyms] | down_read_trylock |
| 0.01% | [kernel.kallsyms] | __lock_text_start |
| 0.01% | [kernel.kallsyms] | page_counter_cancel |
| 0.01% | [kernel.kallsyms] | free_unref_page_prepare.part.0 |
| 0.01% | [kernel.kallsyms] | __kmalloc |
| 0.01% | [kernel.kallsyms] | lru_cache_add_active_or_unevictable |
| 0.01% | [kernel.kallsyms] | pagevec_lru_move_fn |
| 0.01% | [kernel.kallsyms] | alloc_set_pte |
| 0.01% | [kernel.kallsyms] | __lru_cache_add |
| 0.01% | [kernel.kallsyms] | swapgs_restore_regs_and_return_to_usermode |
| 0.01% | [kernel.kallsyms] | format_decode |
| 0.01% | [kernel.kallsyms] | native_flush_tlb_one_user |
| 0.01% | [kernel.kallsyms] | show_cpuinfo |
| 0.01% | [kernel.kallsyms] | __follow_mount_rcu.isra.0 |
| 0.01% | [kernel.kallsyms] | fpregs_assert_state_consistent |
| 0.01% | [kernel.kallsyms] | native_write_msr |
| 0.01% | [kernel.kallsyms] | ___slab_alloc |
| 0.01% | [kernel.kallsyms] | __mod_node_page_state |
| 0.01% | [kernel.kallsyms] | free_unref_page_list |
| 0.01% | [kernel.kallsyms] | unlock_page |
| 0.01% | [kernel.kallsyms] | inherit_event.isra.0 |
| 0.01% | [kernel.kallsyms] | free_pages_and_swap_cache |
| 0.01% | [kernel.kallsyms] | update_cfs_group |
| 0.01% | [kernel.kallsyms] | rcu_all_qs |
| 0.01% | [kernel.kallsyms] | alloc_pages_vma |
| 0.01% | [kernel.kallsyms] | __vma_adjust |
| 0.01% | [kernel.kallsyms] | __ext4_check_dir_entry |
| 0.01% | [kernel.kallsyms] | in_group_p |
| 0.01% | [kernel.kallsyms] | update_curr |
| 0.01% | [kernel.kallsyms] | security_inode_permission |
| 0.01% | [kernel.kallsyms] | memchr |
| 0.01% | [kernel.kallsyms] | vma_interval_tree_insert |
| 0.01% | [kernel.kallsyms] | memcg_kmem_put_cache |
| 0.01% | [kernel.kallsyms] | __mod_zone_page_state |
| 0.01% | [kernel.kallsyms] | update_load_avg |
| 0.01% | [kernel.kallsyms] | mem_cgroup_commit_charge |
| 0.01% | [kernel.kallsyms] | __legitimize_mnt |
| 0.01% | [kernel.kallsyms] | lockref_put_return |
| 0.01% | [kernel.kallsyms] | mem_cgroup_from_task |
| 0.01% | [kernel.kallsyms] | free_unref_page_commit |
| 0.01% | [kernel.kallsyms] | __update_load_avg_se |
| 0.01% | [kernel.kallsyms] | __fput |
| 0.01% | [kernel.kallsyms] | exit_to_usermode_loop |
| 0.01% | [kernel.kallsyms] | __free_pages_ok |
| 0.01% | [kernel.kallsyms] | skb_release_data |
| 0.01% | [kernel.kallsyms] | __check_heap_object |
| 0.01% | [kernel.kallsyms] | call_filldir |
| 0.01% | [kernel.kallsyms] | kmem_cache_alloc_trace |
| 0.01% | [kernel.kallsyms] | __tcp_transmit_skb |
| 0.01% | [kernel.kallsyms] | unmapped_area_topdown |
| 0.01% | [kernel.kallsyms] | _raw_spin_lock_irq |
| 0.01% | [kernel.kallsyms] | fput_many |
| 0.01% | [kernel.kallsyms] | mem_cgroup_try_charge_delay |
| 0.01% | [kernel.kallsyms] | __update_load_avg_cfs_rq |
| 0.01% | [kernel.kallsyms] | xas_start |
| 0.01% | [kernel.kallsyms] | read_tsc |

### libc

3.69% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 2.32% | libc-2.31.so | __nss_database_lookup |
| 0.52% | libc-2.31.so | pthread_attr_setschedparam |
| 0.30% | libcrypto.so.1.1 | CRYPTO_secure_actual_size |
| 0.13% | libc-2.31.so | malloc |
| 0.04% | libc-2.31.so | free |
| 0.03% | libc-2.31.so | _dl_addr |
| 0.03% | libc-2.31.so | __gconv_get_alias_db |
| 0.02% | libc-2.31.so | pthread_cond_signal |
| 0.02% | libc-2.31.so | wcsrtombs |
| 0.02% | libc-2.31.so | pthread_self |
| 0.02% | libc-2.31.so | pthread_mutex_lock |
| 0.02% | libc-2.31.so | __errno_location |
| 0.02% | libc-2.31.so | __libc_realloc |
| 0.02% | libc-2.31.so | pthread_mutex_unlock |
| 0.02% | libc-2.31.so | clock_gettime |
| 0.01% | libc-2.31.so | __xstat |
| 0.01% | libc-2.31.so | __wcsncasecmp_l |

### int

3.62% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.67% | python | k_mul |
| 0.41% | python | _PyLong_Add |
| 0.39% | python | x_divrem |
| 0.31% | python | PyLong_FromLong |
| 0.24% | python | long_hash |
| 0.19% | python | long_to_decimal_string_internal |
| 0.17% | python | x_add |
| 0.14% | python | _PyLong_Subtract |
| 0.10% | python | long_bitwise |
| 0.09% | python | x_sub |
| 0.09% | python | long_richcompare |
| 0.08% | python | PyLong_AsLongAndOverflow |
| 0.08% | python | PyLong_FromString |
| 0.07% | python | _PyLong_Multiply |
| 0.07% | python | long_and |
| 0.06% | python | long_div |
| 0.06% | python | long_rshift |
| 0.05% | python | long_to_decimal_string |
| 0.05% | python | long_add |
| 0.04% | python | long_mod |
| 0.03% | python | long_mul |
| 0.02% | python | PyLong_FromUnsignedLongLong |
| 0.02% | python | long_lshift |
| 0.02% | python | _PyLong_FromBytes |
| 0.01% | python | _PyLong_GCD |
| 0.01% | python | PyLong_AsLong |
| 0.01% | python | PyLong_FromUnsignedLong |
| 0.01% | python | PyLong_FromSsize_t |
| 0.01% | python | long_xor |
| 0.01% | python | PyLong_AsDouble.part.0 |
| 0.01% | python | PyLong_AsSsize_t |
| 0.01% | python | long_vectorcall |
| 0.01% | python | _PyLong_Lshift |
| 0.01% | python | PyLong_FromUnicodeObject |
| 0.01% | python | PyLong_AsInt |

### dict

3.56% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.59% | python | PyDict_GetItemRef |
| 0.48% | python | dict_setdefault_ref_lock_held |
| 0.48% | python | insertdict |
| 0.34% | python | PyDict_SetItem |
| 0.27% | python | dict_get |
| 0.24% | python | dictresize |
| 0.21% | python | PyDict_Next |
| 0.20% | python | insert_to_emptydict |
| 0.17% | python | PyDict_Contains |
| 0.10% | python | dict_subscript |
| 0.08% | python | dictiter_iternextitem |
| 0.06% | python | dict_merge |
| 0.03% | python | PyDict_GetItemWithError |
| 0.03% | python | dict_items |
| 0.03% | python | dict_ass_sub |
| 0.03% | python | PyDict_Copy |
| 0.03% | python | PyDict_DelItem |
| 0.02% | python | _PyDict_GetItem_KnownHash |
| 0.02% | python | _PyDict_FromItems |
| 0.02% | python | dict_getitem |
| 0.02% | python | _PyDict_Next |
| 0.02% | python | dictiter_iternextvalue |
| 0.01% | python | dictiter_iternextkey |
| 0.01% | python | PyDict_SetItemString |
| 0.01% | python | dict_iter |

### str

3.42% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.52% | python | siphash13 |
| 0.44% | python | unicode_decode_utf8 |
| 0.28% | python | PyUnicode_FromKindAndData |
| 0.25% | python | PyUnicode_Substring |
| 0.21% | python | _PyUnicode_InternInPlace |
| 0.20% | python | _PyUnicode_JoinArray |
| 0.15% | python | PyBytes_FromStringAndSize |
| 0.10% | python | unicode_replace |
| 0.09% | python | _PyUnicodeWriter_PrepareInternal |
| 0.09% | python | PyUnicode_Format |
| 0.07% | python | _PyUnicodeWriter_WriteStr |
| 0.06% | python | PyUnicode_FromFormatV |
| 0.06% | python | PyUnicode_Concat |
| 0.05% | python | unicode_subscript |
| 0.05% | python | PyUnicode_RichCompare |
| 0.05% | python | PyUnicode_FSConverter |
| 0.05% | python | _PyUnicode_FromUCS4 |
| 0.05% | python | bytes_subscript |
| 0.04% | python | unicode_hash |
| 0.04% | python | PyUnicode_Contains |
| 0.04% | python | unicode_encode |
| 0.03% | python | bytes_concat |
| 0.03% | python | unicode_encode_utf8 |
| 0.03% | python | PyUnicode_AsUTF8AndSize |
| 0.03% | python | stringlib_bytes_join.lto_priv.1 |
| 0.03% | python | resize_compact |
| 0.02% | python | _PyUnicode_FromASCII |
| 0.02% | python | unicode_startswith |
| 0.02% | python | unicode_split |
| 0.02% | python | PyUnicode_FromWideChar |
| 0.01% | python | unicode_repr |
| 0.01% | python | unicode_join |
| 0.01% | python | bytes_decode |
| 0.01% | python | _PyUnicodeWriter_Finish |
| 0.01% | python | PyUnicode_DecodeFSDefault |
| 0.01% | python | PyBytes_Repr |
| 0.01% | python | _PyUnicodeWriter_Init |
| 0.01% | python | unicode_find |
| 0.01% | python | unicode_rfind |
| 0.01% | python | bytes_richcompare |
| 0.01% | python | unicode_splitlines |
| 0.01% | python | _PyUnicode_IsAlpha |
| 0.01% | python | unicode_rstrip |
| 0.01% | python | unicode_strip |
| 0.01% | python | _PyUnicode_TranslateCharmap |
| 0.01% | python | PyUnicode_RPartition |
| 0.01% | python | unicode_endswith |

### list

1.28% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.18% | python | list_ass_slice_lock_held |
| 0.17% | python | list_subscript |
| 0.16% | python | list_iter |
| 0.15% | python | list_resize |
| 0.08% | python | list_contains |
| 0.08% | python | _PyList_FromArraySteal |
| 0.07% | python | PyList_SetSlice |
| 0.05% | python | list_sort_impl |
| 0.04% | python | PyList_Append |
| 0.04% | python | list_vectorcall |
| 0.04% | python | list_append |
| 0.04% | python | list_ass_subscript |
| 0.03% | python | list_concat |
| 0.03% | python | list_extend |
| 0.03% | python | listiter_next |
| 0.02% | python | list_pop |
| 0.01% | python | PyList_Size |
| 0.01% | python | list_length |
| 0.01% | python | list_clear_impl.constprop.0 |
| 0.01% | python | list_richcompare |

### tuple

1.12% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.51% | python | tuplehash |
| 0.20% | python | _PyTuple_FromArraySteal |
| 0.13% | python | tupletraverse |
| 0.07% | python | tuple_iter |
| 0.06% | python | tuplerichcompare |
| 0.05% | python | PyTuple_Pack |
| 0.03% | python | tuplecontains |
| 0.02% | python | _PyTuple_FromArray |
| 0.01% | python | tupleiter_next |
| 0.01% | python | tuplesubscript |
| 0.01% | python | _PyTuple_Resize |
| 0.01% | python | PyTuple_Size |

### miscobj

1.12% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.14% | python | set_contains_lock_held |
| 0.11% | python | PySlice_Unpack |
| 0.10% | python | setiter_iternext |
| 0.10% | python | set_issubset_impl |
| 0.09% | python | set_lookkey |
| 0.09% | python | PySlice_AdjustIndices |
| 0.07% | python | set_vectorcall |
| 0.06% | python | enum_next |
| 0.05% | python | set_difference |
| 0.03% | python | set_add |
| 0.03% | python | deque_append_lock_held |
| 0.03% | python | set_table_resize |
| 0.02% | python | set_add_entry |
| 0.02% | python | dequeiter_next_lock_held.isra.0 |
| 0.02% | python | bytearray_ass_subscript |
| 0.01% | python | set_merge_lock_held.part.0 |
| 0.01% | python | deque_append_impl |
| 0.01% | python | deque_popleft_impl |
| 0.01% | python | set_intersection |
| 0.01% | python | PyBuffer_Release |
| 0.01% | python | deque_clear |
| 0.01% | python | _PySlice_GetLongIndices |
| 0.01% | python | set_iter |

### lookup

1.07% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.30% | python | find_name_in_mro |
| 0.29% | python | _Py_dict_lookup |
| 0.25% | python | _Py_type_getattro |
| 0.17% | python | unicodekeys_lookup_unicode |
| 0.03% | python | builtin_getattr |
| 0.02% | python | _PyType_Lookup |

### calls

0.90% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.31% | python | _PyFunction_Vectorcall |
| 0.11% | python | vgetargs1_impl |
| 0.07% | python | vgetargskeywords.constprop.0 |
| 0.07% | python | vectorcall_method |
| 0.05% | python | method_vectorcall_VARARGS |
| 0.04% | python | _PyArg_UnpackKeywords |
| 0.03% | python | cfunction_vectorcall_FASTCALL_KEYWORDS |
| 0.03% | python | method_vectorcall_VARARGS_KEYWORDS |
| 0.03% | python | cfunction_vectorcall_NOARGS |
| 0.02% | python | PyArg_UnpackTuple |
| 0.02% | python | cfunction_vectorcall_O |
| 0.02% | python | method_vectorcall_FASTCALL_KEYWORDS_METHOD |
| 0.02% | python | PyArg_ParseTuple |
| 0.01% | python | cfunction_call |
| 0.01% | python | _Py_CheckFunctionResult |
| 0.01% | python | _PyArg_UnpackKeywordsWithVararg |
| 0.01% | python | method_vectorcall_NOARGS |
| 0.01% | python | method_vectorcall_FASTCALL |
| 0.01% | python | PyArg_ParseTupleAndKeywords |
| 0.01% | python | PyArg_Parse |
| 0.01% | python | method_vectorcall_O |
| 0.01% | python | cfunction_vectorcall_FASTCALL_KEYWORDS_METHOD |

### exceptions

0.46% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.16% | python | _PyErr_SetObject |
| 0.07% | python | PyTraceBack_Here |
| 0.06% | python | PyCode_Addr2Line |
| 0.04% | python | PyErr_GivenExceptionMatches |
| 0.03% | python | PyErr_ExceptionMatches |
| 0.02% | python | BaseException_init |
| 0.01% | python | PyErr_Occurred |
| 0.01% | python | PyErr_Format |
| 0.01% | python | AttributeError_init |
| 0.01% | python | PyFrame_GetCode |

### float

0.41% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.18% | python | PyFloat_FromDouble |
| 0.09% | python | float_div |
| 0.04% | python | float_richcompare |
| 0.03% | python | PyFloat_AsDouble |
| 0.02% | python | float_pow |
| 0.02% | python | float_mul |
| 0.02% | python | float_sub |
| 0.01% | python | float_add |

### import

0.41% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.38% | python | r_object |
| 0.02% | python | PyImport_ImportModuleLevelObject |

### gil

0.00% total

| percentage | object | symbol |
| ---: | :--- | :--- |
