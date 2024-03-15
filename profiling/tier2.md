
## 2to3

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.87% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.28% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.14% | `python` | `type_new` | memory |
| 2.06% | `python` | `gc_collect_main` | gc |
| 2.00% | `python` | `deduce_unreachable` | unknown |
| 1.78% | `python` | `visit_decref` | gc |
| 1.66% | `python` | `tupledealloc` | memory |
| 1.61% | `python` | `sre_ucs1_match` | library |
| 1.56% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.38% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.06% | `python` | `PyDict_GetItemRef` | dict |
| 1.00% | `python` | `visit_reachable` | gc |
| 0.92% | `python` | `_PyCode_New` | memory |
| 0.78% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.74% | `python` | `r_object` | import |
| 0.73% | `python` | `_PyPegen_fill_token` | interpreter |
| 0.72% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.71% | `python` | `list_dealloc` | memory |
| 0.65% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.62% | `python` | `gen_dealloc` | memory |
| 0.59% | `python` | `siphash13` | str |
| 0.59% | `python` | `PyObject_GetAttr` | dynamic |
| 0.59% | `python` | `PyObject_SetAttr` | dynamic |
| 0.56% | `python` | `PyUnicode_FromKindAndData` | str |
| 0.53% | `python` | `make_gen` | unknown |
| 0.53% | `python` | `dict_dealloc` | memory |
| 0.52% | `python` | `subtype_traverse` | gc |

## aiohttp

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 30.39% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.56% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.20% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.56% | `python` | `tupledealloc` | memory |
| 1.37% | `python` | `type_new` | memory |
| 1.13% | `python` | `gc_collect_main` | gc |
| 1.01% | `python` | `visit_decref` | gc |
| 1.01% | `python` | `deduce_unreachable` | unknown |
| 0.82% | `python` | `PyDict_GetItemRef` | dict |
| 0.80% | `python` | `subtype_dealloc` | memory |
| 0.76% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.71% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.67% | `python` | `visit_reachable` | gc |
| 0.65% | `python` | `unicode_dealloc` | memory |
| 0.64% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.64% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.62% | `python` | `dict_dealloc` | memory |
| 0.59% | `python` | `_PyCode_New` | memory |
| 0.58% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.57% | `python` | `find_name_in_mro` | lookup |
| 0.56% | `python` | `sre_ucs1_match` | library |
| 0.56% | `python` | `list_dealloc` | memory |
| 0.54% | `python` | `_PySuper_Lookup` | dynamic |
| 0.54% | `python` | `siphash13` | str |
| 0.52% | `python` | `r_object` | import |

## async_generators

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.30% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 9.92% | `python` | `_PyErr_SetObject` | exceptions |
| 4.04% | `python` | `StopIteration_dealloc` | memory |
| 3.88% | `python` | `BaseException_new` | memory |
| 3.14% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 2.41% | `python` | `StopIteration_init` | dynamic |
| 2.31% | `python` | `async_gen_asend_send` | unknown |
| 2.24% | `python` | `gen_send_ex` | unknown |
| 1.90% | `python` | `tupledealloc` | memory |
| 1.74% | `python` | `gen_send_ex2` | unknown |
| 1.71% | `python` | `PyErr_ExceptionMatches` | exceptions |
| 1.69% | `python` | `_PyAsyncGenValueWrapperNew` | memory |
| 1.66% | `python` | `PyErr_GivenExceptionMatches` | exceptions |
| 1.63% | `python` | `async_gen_asend_dealloc` | memory |
| 1.56% | `python` | `async_gen_asend_new` | memory |
| 1.45% | `python` | `_PyEval_EvalFrameDefault.cold` | interpreter |
| 1.40% | `python` | `async_gen_wrapped_val_dealloc` | memory |
| 1.37% | `python` | `_Py_NewReference` | memory |
| 1.18% | `python` | `gc_collect_main` | gc |
| 1.17% | `python` | `async_gen_unwrap_value.isra.0` | unknown |
| 1.15% | `python` | `deduce_unreachable` | unknown |
| 1.12% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.05% | `python` | `long_add` | int |
| 0.99% | `python` | `_PyGen_FetchStopIterationValue.cold` | unknown |
| 0.86% | `python` | `type_call` | dynamic |
| 0.78% | `python` | `visit_decref` | gc |
| 0.77% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.77% | `python` | `_PyGen_SetStopIterationValue` | unknown |
| 0.77% | `python` | `visit_reachable` | gc |
| 0.74% | `python` | `subtype_traverse` | gc |
| 0.72% | `python` | `PyObject_CallFinalizerFromDealloc` | memory |
| 0.60% | `python` | `long_dealloc` | memory |
| 0.57% | `python` | `PyType_GenericAlloc` | memory |
| 0.56% | `python` | `range_subscript` | unknown |
| 0.53% | `python` | `_Py_Dealloc` | memory |
| 0.52% | `python` | `subtype_dealloc` | memory |

## async_tree

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 23.77% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 13.32% | `python` | `gc_collect_main` | gc |
| 7.60% | `python` | `deduce_unreachable` | unknown |
| 5.84% | `python` | `visit_decref` | gc |
| 5.71% | `python` | `visit_reachable` | gc |
| 1.56% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.35% | `python` | `subtype_traverse` | gc |
| 1.30% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.06% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.91% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.90% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.89% | `python` | `_PyObject_GC_New` | gc |
| 0.88% | `python` | `tupledealloc` | memory |
| 0.87% | `python` | `PyObject_GC_Del` | gc |
| 0.76% | `python` | `insertdict` | dict |
| 0.72% | `python` | `gen_traverse` | gc |
| 0.69% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.67% | `python` | `slot_tp_init` | unknown |
| 0.67% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.65% | `python` | `meth_dealloc` | memory |
| 0.62% | `python` | `subtype_dealloc` | memory |
| 0.60% | `python` | `context_tp_dealloc` | memory |
| 0.60% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.53% | `python` | `list_dealloc` | memory |
| 0.53% | `python` | `object_new` | memory |
| 0.53% | `python` | `PyDict_GetItemRef` | dict |

## async_tree_cpu_io_mixed

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 18.47% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 16.83% | `python` | `k_mul` | int |
| 10.60% | `python` | `gc_collect_main` | gc |
| 6.26% | `python` | `deduce_unreachable` | unknown |
| 4.90% | `python` | `visit_decref` | gc |
| 4.59% | `python` | `visit_reachable` | gc |
| 2.23% | `python` | `long_dealloc` | memory |
| 1.24% | `python` | `subtype_traverse` | gc |
| 1.09% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.99% | `python` | `_PyLong_New` | memory |
| 0.95% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.92% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.72% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.63% | `python` | `tupledealloc` | memory |
| 0.63% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.63% | `math.cpython-313-x86_64-linux-gnu.so` | `factorial_partial_product` | library |
| 0.61% | `python` | `long_mul` | int |
| 0.56% | `python` | `gen_traverse` | gc |
| 0.56% | `python` | `_PyObject_GC_New` | gc |
| 0.53% | `python` | `insertdict` | dict |
| 0.53% | `python` | `PyObject_GC_Del` | gc |

## async_tree_cpu_io_mixed_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 16.55% | `python` | `k_mul` | int |
| 16.45% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 12.40% | `python` | `gc_collect_main` | gc |
| 7.72% | `python` | `deduce_unreachable` | unknown |
| 5.33% | `python` | `visit_decref` | gc |
| 5.09% | `python` | `visit_reachable` | gc |
| 2.19% | `python` | `long_dealloc` | memory |
| 1.41% | `python` | `subtype_traverse` | gc |
| 1.06% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.97% | `python` | `_PyLong_New` | memory |
| 0.95% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.95% | `python` | `gen_traverse` | gc |
| 0.81% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.70% | `python` | `set_traverse` | gc |
| 0.68% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.60% | `python` | `long_mul` | int |
| 0.60% | `math.cpython-313-x86_64-linux-gnu.so` | `factorial_partial_product` | library |
| 0.58% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.54% | `python` | `tupledealloc` | memory |
| 0.51% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |

## async_tree_io

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 20.81% | `python` | `gc_collect_main` | gc |
| 20.05% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 10.53% | `python` | `deduce_unreachable` | unknown |
| 7.84% | `python` | `visit_reachable` | gc |
| 7.48% | `python` | `visit_decref` | gc |
| 1.62% | `python` | `subtype_traverse` | gc |
| 1.34% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.28% | `python` | `gen_traverse` | gc |
| 0.80% | `python` | `slot_tp_richcompare` | dynamic |
| 0.79% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.63% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.62% | `python` | `tupledealloc` | memory |
| 0.56% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.55% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.55% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.55% | `_heapq.cpython-313-x86_64-linux-gnu.so` | `_heapq_heappop` | library |
| 0.53% | `python` | `PyObject_GC_Del` | gc |
| 0.52% | `python` | `_PyObject_GetMethod` | dynamic |

## async_tree_io_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 22.04% | `python` | `gc_collect_main` | gc |
| 18.27% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 11.92% | `python` | `deduce_unreachable` | unknown |
| 8.08% | `python` | `visit_reachable` | gc |
| 7.71% | `python` | `visit_decref` | gc |
| 1.73% | `python` | `subtype_traverse` | gc |
| 1.72% | `python` | `gen_traverse` | gc |
| 1.23% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.85% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.80% | `python` | `slot_tp_richcompare` | dynamic |
| 0.68% | `python` | `set_traverse` | gc |
| 0.63% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.59% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.57% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.57% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.53% | `python` | `tupledealloc` | memory |
| 0.51% | `_heapq.cpython-313-x86_64-linux-gnu.so` | `_heapq_heappop` | library |

## async_tree_memoization

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 23.96% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 14.12% | `python` | `gc_collect_main` | gc |
| 8.20% | `python` | `deduce_unreachable` | unknown |
| 6.40% | `python` | `visit_decref` | gc |
| 6.09% | `python` | `visit_reachable` | gc |
| 1.70% | `python` | `subtype_traverse` | gc |
| 1.53% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.27% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.94% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.82% | `python` | `tupledealloc` | memory |
| 0.79% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.75% | `python` | `gen_traverse` | gc |
| 0.74% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.74% | `python` | `_PyObject_GC_New` | gc |
| 0.73% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.66% | `python` | `PyObject_GC_Del` | gc |
| 0.66% | `python` | `insertdict` | dict |
| 0.64% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.62% | `python` | `meth_dealloc` | memory |
| 0.60% | `python` | `slot_tp_init` | unknown |
| 0.58% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.57% | `python` | `context_tp_dealloc` | memory |
| 0.53% | `python` | `list_dealloc` | memory |
| 0.52% | `python` | `object_new` | memory |

## async_tree_memoization_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.42% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 16.06% | `python` | `gc_collect_main` | gc |
| 10.37% | `python` | `deduce_unreachable` | unknown |
| 6.89% | `python` | `visit_decref` | gc |
| 6.73% | `python` | `visit_reachable` | gc |
| 1.81% | `python` | `subtype_traverse` | gc |
| 1.41% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.23% | `python` | `gen_traverse` | gc |
| 1.00% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.89% | `python` | `set_traverse` | gc |
| 0.86% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.85% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.81% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.68% | `python` | `tupledealloc` | memory |
| 0.63% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.63% | `python` | `meth_dealloc` | memory |
| 0.59% | `python` | `PyObject_GC_Del` | gc |
| 0.55% | `python` | `make_gen` | unknown |
| 0.54% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.53% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.52% | `python` | `slot_tp_init` | unknown |
| 0.51% | `python` | `PyDict_GetItemRef` | dict |

## async_tree_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 20.83% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 15.67% | `python` | `gc_collect_main` | gc |
| 9.70% | `python` | `deduce_unreachable` | unknown |
| 6.38% | `python` | `visit_decref` | gc |
| 6.36% | `python` | `visit_reachable` | gc |
| 1.61% | `python` | `subtype_traverse` | gc |
| 1.44% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.24% | `python` | `gen_traverse` | gc |
| 1.13% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.98% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.97% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.97% | `python` | `set_traverse` | gc |
| 0.75% | `python` | `tupledealloc` | memory |
| 0.74% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.74% | `python` | `PyObject_GC_Del` | gc |
| 0.66% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.63% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.62% | `python` | `PyDict_GetItemRef` | dict |
| 0.61% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.58% | `python` | `slot_tp_init` | unknown |
| 0.57% | `python` | `_PyObject_GC_New` | gc |
| 0.56% | `python` | `meth_dealloc` | memory |
| 0.56% | `python` | `subtype_dealloc` | memory |
| 0.54% | `python` | `make_gen` | unknown |

## asyncio_tcp

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.21% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 17.31% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 10.54% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.10% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.56% | `[kernel.kallsyms]` | `tcp_sendmsg_locked` | kernel |

## asyncio_tcp_ssl

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 38.71% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 25.65% | `libcrypto.so.1.1` | `CRYPTO_secure_actual_size` | libc |
| 11.07% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 4.49% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.89% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.87% | `libssl.so.1.1` | `SSL_rstate_string` | library |
| 0.54% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |

## asyncio_websockets

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 63.93% | `libz.so.1.2.11` | `crc32_combine64` | library |
| 20.22% | `libz.so.1.2.11` | `inflateBackEnd` | library |
| 2.84% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.16% | `python` | `_PyEval_EvalFrameDefault` | interpreter |

## chameleon

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 42.06% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.42% | `python` | `PyObject_Str` | dynamic |
| 2.35% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.27% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.14% | `python` | `PyUnicode_Format` | str |
| 2.13% | `python` | `sre_ucs2_charset.isra.0` | library |
| 1.83% | `python` | `_PyUnicode_JoinArray` | str |
| 1.79% | `python` | `type_new` | memory |
| 1.56% | `python` | `dict_get` | dict |
| 1.39% | `python` | `insertdict` | dict |
| 1.28% | `python` | `unicode_dealloc` | memory |
| 0.97% | `python` | `gc_collect_main` | gc |
| 0.96% | `python` | `list_append` | list |
| 0.94% | `python` | `deduce_unreachable` | unknown |
| 0.91% | `python` | `PyUnicode_Concat` | str |
| 0.83% | `python` | `visit_decref` | gc |
| 0.82% | `python` | `list_dealloc` | memory |
| 0.80% | `python` | `state_init` | unknown |
| 0.79% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 0.72% | `python` | `visit_reachable` | gc |
| 0.71% | `python` | `_PyCode_New` | memory |
| 0.59% | `python` | `tupledealloc` | memory |
| 0.57% | `python` | `r_object` | import |
| 0.55% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.55% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.54% | `libc-2.31.so` | `malloc` | libc |

## chaos

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 56.09% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.08% | `python` | `_PyLong_Subtract` | int |
| 2.01% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.96% | `python` | `PyFloat_FromDouble` | float |
| 1.66% | `python` | `_PyLong_Add` | int |
| 1.51% | `python` | `subtype_dealloc` | memory |
| 1.24% | `python` | `convert_to_double` | unknown |
| 1.16% | `python` | `range_vectorcall` | unknown |
| 1.07% | `python` | `float_div` | float |
| 0.97% | `python` | `PyNumber_Subtract` | dynamic |
| 0.95% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.94% | `python` | `float_dealloc` | memory |
| 0.84% | `python` | `type_new` | memory |
| 0.83% | `python` | `PyType_GenericAlloc` | memory |
| 0.78% | `libm-2.31.so` | `f64xsubf128` | library |
| 0.78% | `python` | `PyNumber_TrueDivide` | dynamic |
| 0.76% | `python` | `range_iter` | unknown |
| 0.71% | `python` | `float_richcompare` | float |
| 0.65% | `python` | `PyObject_Free` | dynamic |
| 0.56% | `python` | `tupledealloc` | memory |
| 0.55% | `python` | `float_sub` | float |
| 0.55% | `python` | `float_pow` | float |
| 0.52% | `python` | `gc_collect_main` | gc |
| 0.52% | `python` | `PyType_IsSubtype` | dynamic |
| 0.51% | `python` | `visit_decref` | gc |

## comprehensions

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 53.89% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.19% | `python` | `dict_get` | dict |
| 1.95% | `python` | `list_resize` | list |
| 1.78% | `python` | `PyFunction_NewWithQualName` | memory |
| 1.62% | `python` | `PyDict_GetItemRef` | dict |
| 1.44% | `python` | `list_dealloc` | memory |
| 1.42% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.42% | `python` | `list_iter` | list |
| 1.38% | `python` | `insertdict` | dict |
| 1.29% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.16% | `python` | `gen_dealloc` | memory |
| 1.00% | `python` | `unsafe_tuple_compare` | unknown |
| 0.85% | `python` | `func_dealloc` | memory |
| 0.84% | `python` | `type_new` | memory |
| 0.80% | `python` | `listiter_dealloc` | memory |
| 0.74% | `python` | `PyObject_GC_Del` | gc |
| 0.73% | `python` | `_Py_type_getattro` | lookup |
| 0.72% | `python` | `tupledealloc` | memory |
| 0.71% | `python` | `_PyObject_Malloc` | memory |
| 0.69% | `python` | `make_gen` | unknown |
| 0.66% | `python` | `long_richcompare` | int |
| 0.65% | `python` | `PyObject_RichCompare` | dynamic |
| 0.62% | `python` | `long_hash` | int |
| 0.59% | `python` | `gc_collect_main` | gc |
| 0.53% | `python` | `_PyList_FromArraySteal` | list |
| 0.52% | `python` | `dictresize` | dict |

## concurrent_imap

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 27.25% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 1.94% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.60% | `[kernel.kallsyms]` | `perf_event_alloc` | kernel |
| 1.59% | `python` | `subtype_dealloc` | memory |
| 1.52% | `[kernel.kallsyms]` | `memset_erms` | kernel |
| 1.16% | `python` | `tupledealloc` | memory |
| 1.16% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.95% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.88% | `python` | `PyObject_GC_Del` | gc |
| 0.82% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.80% | `[kernel.kallsyms]` | `mutex_lock` | kernel |
| 0.74% | `[kernel.kallsyms]` | `kfree` | kernel |
| 0.74% | `[kernel.kallsyms]` | `mutex_unlock` | kernel |
| 0.70% | `python` | `method_dealloc` | memory |
| 0.70% | `python` | `list_dealloc` | memory |
| 0.67% | `python` | `long_dealloc` | memory |
| 0.66% | `[kernel.kallsyms]` | `inherit_event.isra.0` | kernel |
| 0.66% | `[kernel.kallsyms]` | `page_counter_cancel` | kernel |
| 0.59% | `[kernel.kallsyms]` | `_raw_spin_lock` | kernel |
| 0.52% | `[kernel.kallsyms]` | `copy_page` | kernel |
| 0.51% | `python` | `PyObject_GetAttr` | dynamic |

## coroutines

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 41.89% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 13.30% | `python` | `gen_dealloc` | memory |
| 8.30% | `python` | `make_gen` | unknown |
| 6.60% | `python` | `_PyEval_EvalFrameDefault.cold` | interpreter |
| 5.51% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.58% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.28% | `python` | `_PyLong_Subtract` | int |
| 2.03% | `python` | `_PyFrame_ClearExceptCode` | interpreter |
| 1.49% | `python` | `_PyLong_Add` | int |
| 1.39% | `python` | `_PyCoro_GetAwaitableIter` | unknown |
| 0.81% | `python` | `type_new` | memory |
| 0.53% | `python` | `gc_collect_main` | gc |
| 0.51% | `python` | `_PyGen_yf` | unknown |

## coverage

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 20.49% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.66% | `tracer.cpython-313-x86_64-linux-gnu.so` | `CTracer_trace` | library |
| 4.72% | `python` | `call_instrumentation_vector` | unknown |
| 4.12% | `python` | `PyObject_SetAttrString` | dynamic |
| 3.82% | `python` | `unicode_decode_utf8` | str |
| 3.33% | `python` | `_Py_dict_lookup` | lookup |
| 3.17% | `python` | `siphash13` | str |
| 3.02% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 2.48% | `python` | `frame_dealloc` | memory |
| 2.40% | `python` | `PyLong_FromLong` | int |
| 2.40% | `python` | `call_one_instrument` | unknown |
| 2.26% | `python` | `PySet_Add` | unknown |
| 2.01% | `python` | `_PyFrame_MakeAndSetFrameObject` | unknown |
| 1.80% | `python` | `_PyObject_VectorcallTstate.lto_priv.5` | dynamic |
| 1.62% | `python` | `PyObject_SetAttr` | dynamic |
| 1.43% | `python` | `dict_getitem` | dict |
| 1.41% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.38% | `python` | `unicode_dealloc` | memory |
| 1.11% | `python` | `_Py_hashtable_get` | unknown |
| 1.11% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.07% | `python` | `type_new` | memory |
| 1.04% | `python` | `call_trace_func.isra.0` | unknown |
| 0.96% | `python` | `_PyUnicode_InternInPlace` | str |
| 0.80% | `python` | `_Py_call_instrumentation_jump` | unknown |
| 0.79% | `python` | `_PyCode_GetCode` | unknown |
| 0.67% | `python` | `gc_collect_main` | gc |
| 0.63% | `python` | `deduce_unreachable` | unknown |
| 0.56% | `python` | `long_hash` | int |
| 0.55% | `python` | `visit_decref` | gc |
| 0.54% | `python` | `PyFrame_GetCode` | exceptions |
| 0.52% | `python` | `PyEval_GetFrame` | interpreter |

## crypto_pyaes

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 43.28% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.80% | `python` | `long_dealloc` | memory |
| 6.16% | `python` | `long_bitwise` | int |
| 4.03% | `python` | `long_rshift` | int |
| 3.45% | `python` | `long_mod` | int |
| 3.23% | `python` | `_PyLong_New` | memory |
| 3.18% | `python` | `long_and` | int |
| 1.66% | `python` | `PyNumber_And` | dynamic |
| 1.34% | `python` | `binary_op` | unknown |
| 1.27% | `python` | `_PyLong_Add` | int |
| 1.05% | `python` | `_PyObject_Malloc` | memory |
| 0.98% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.97% | `python` | `PyObject_Free` | dynamic |
| 0.89% | `python` | `PyNumber_Remainder` | dynamic |
| 0.85% | `python` | `list_dealloc` | memory |
| 0.75% | `python` | `type_new` | memory |
| 0.75% | `python` | `PyNumber_Rshift` | dynamic |
| 0.66% | `python` | `long_xor` | int |
| 0.60% | `python` | `range_vectorcall` | unknown |
| 0.50% | `python` | `gc_collect_main` | gc |

## dask

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 35.77% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.40% | `python` | `gc_collect_main` | gc |
| 2.26% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.09% | `python` | `visit_decref` | gc |
| 2.08% | `python` | `deduce_unreachable` | unknown |
| 1.84% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.62% | `python` | `tupledealloc` | memory |
| 1.51% | `python` | `visit_reachable` | gc |
| 1.06% | `python` | `object_isinstance` | dynamic |
| 0.98% | `python` | `PyDict_GetItemRef` | dict |
| 0.86% | `python` | `dict_dealloc` | memory |
| 0.79% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.78% | `python` | `PyBytes_Repr` | str |
| 0.74% | `python` | `type_new` | memory |
| 0.73% | `python` | `long_dealloc` | memory |
| 0.60% | `python` | `insertdict` | dict |
| 0.52% | `python` | `list_dealloc` | memory |
| 0.51% | `python` | `PyObject_Free` | dynamic |
| 0.50% | `python` | `_PyTuple_FromArraySteal` | tuple |

## deepcopy

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 51.12% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.26% | `python` | `dict_get` | dict |
| 4.01% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.15% | `python` | `long_dealloc` | memory |
| 2.12% | `python` | `_PyLong_New` | memory |
| 1.39% | `python` | `insertdict` | dict |
| 1.16% | `python` | `PySys_Audit` | unknown |
| 1.12% | `python` | `long_hash` | int |
| 1.08% | `python` | `builtin_id` | unknown |
| 1.06% | `python` | `PyDict_GetItemRef` | dict |
| 1.03% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.85% | `python` | `insert_to_emptydict` | dict |
| 0.79% | `python` | `tupledealloc` | memory |
| 0.74% | `python` | `type_new` | memory |
| 0.68% | `python` | `list_dealloc` | memory |
| 0.63% | `python` | `list_append` | list |
| 0.63% | `python` | `dict_dealloc` | memory |
| 0.57% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.52% | `python` | `long_richcompare` | int |
| 0.51% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.50% | `python` | `PyMem_Realloc` | memory |

## deltablue

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 61.43% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.42% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.21% | `python` | `_PyObject_GetMethod` | dynamic |
| 1.27% | `python` | `gc_collect_main` | gc |
| 1.12% | `python` | `deduce_unreachable` | unknown |
| 1.00% | `python` | `visit_decref` | gc |
| 0.99% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.94% | `python` | `type_new` | memory |
| 0.93% | `python` | `_PySuper_Lookup` | dynamic |
| 0.70% | `python` | `_Py_type_getattro` | lookup |
| 0.62% | `python` | `subtype_traverse` | gc |
| 0.59% | `python` | `PyObject_GC_Del` | gc |
| 0.58% | `python` | `method_dealloc` | memory |
| 0.58% | `python` | `visit_reachable` | gc |

## django_template

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 37.97% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.91% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.31% | `python` | `type_new` | memory |
| 1.79% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.63% | `python` | `object_isinstance` | dynamic |
| 1.35% | `python` | `gc_collect_main` | gc |
| 1.25% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.22% | `python` | `deduce_unreachable` | unknown |
| 1.20% | `python` | `tupledealloc` | memory |
| 1.11% | `python` | `insertdict` | dict |
| 1.09% | `python` | `visit_decref` | gc |
| 1.03% | `python` | `PyDict_GetItemRef` | dict |
| 1.02% | `python` | `PyObject_GC_Del` | gc |
| 0.87% | `python` | `_PyCode_New` | memory |
| 0.80% | `python` | `visit_reachable` | gc |
| 0.79% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.77% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.70% | `python` | `r_object` | import |
| 0.70% | `python` | `PyObject_Str` | dynamic |
| 0.70% | `python` | `unicode_replace` | str |
| 0.69% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.67% | `python` | `list_dealloc` | memory |
| 0.58% | `python` | `builtin_hasattr` | unknown |
| 0.58% | `python` | `dict_dealloc` | memory |
| 0.55% | `python` | `_PyObject_GenericGetAttrWithDict` | dynamic |
| 0.54% | `python` | `PyUnicode_FromKindAndData` | str |
| 0.52% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.51% | `python` | `PyType_GenericAlloc` | memory |

## djangocms

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.59% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.49% | `python` | `find_name_in_mro` | lookup |
| 3.26% | `python` | `type_new` | memory |
| 2.44% | `python` | `gc_collect_main` | gc |
| 2.42% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.13% | `python` | `deduce_unreachable` | unknown |
| 1.85% | `python` | `visit_decref` | gc |
| 1.37% | `python` | `visit_reachable` | gc |
| 1.35% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.28% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.12% | `python` | `tupledealloc` | memory |
| 1.07% | `libsqlite3.so.0.8.6` | `sqlite3_exec` | library |
| 1.02% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.99% | `python` | `PyDict_GetItemRef` | dict |
| 0.85% | `python` | `dict_traverse` | gc |
| 0.80% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.73% | `python` | `dict_dealloc` | memory |
| 0.73% | `libz.so.1.2.11` | `inflateBackEnd` | library |
| 0.65% | `python` | `sre_ucs1_match` | library |
| 0.65% | `python` | `insertdict` | dict |
| 0.64% | `python` | `_PyCode_New` | memory |
| 0.61% | `python` | `unicode_dealloc` | memory |
| 0.58% | `python` | `_PyPegen_fill_token` | interpreter |
| 0.56% | `python` | `PyObject_SetAttr` | dynamic |
| 0.56% | `python` | `r_object` | import |
| 0.53% | `python` | `list_dealloc` | memory |
| 0.51% | `python` | `siphash13` | str |

## docutils

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 31.27% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.13% | `python` | `sre_ucs1_match` | library |
| 3.37% | `python` | `gc_collect_main` | gc |
| 3.14% | `python` | `deduce_unreachable` | unknown |
| 2.57% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 2.22% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.17% | `python` | `visit_decref` | gc |
| 2.13% | `python` | `sre_ucs2_charset.isra.0` | library |
| 1.80% | `python` | `find_name_in_mro` | lookup |
| 1.78% | `python` | `list_dealloc` | memory |
| 1.71% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.26% | `python` | `visit_reachable` | gc |
| 1.06% | `python` | `PyObject_SetAttr` | dynamic |
| 1.04% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.86% | `python` | `tupledealloc` | memory |
| 0.84% | `python` | `_PyUnicode_JoinArray` | str |
| 0.78% | `python` | `subtype_traverse` | gc |
| 0.78% | `python` | `PyDict_GetItemRef` | dict |
| 0.76% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 0.74% | `python` | `PyObject_GetAttr` | dynamic |
| 0.74% | `python` | `object_isinstance` | dynamic |
| 0.64% | `python` | `list_traverse` | gc |
| 0.63% | `python` | `PyMem_Free` | memory |
| 0.61% | `python` | `list_subscript` | list |
| 0.60% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.57% | `python` | `insertdict` | dict |
| 0.55% | `python` | `dict_traverse` | gc |
| 0.55% | `python` | `PyUnicode_Format` | str |
| 0.52% | `python` | `dict_dealloc` | memory |
| 0.52% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.52% | `python` | `unicode_dealloc` | memory |
| 0.51% | `python` | `_PyEvalFramePushAndInit` | interpreter |

## dulwich_log

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 33.45% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.64% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.58% | `libz.so.1.2.11` | `inflateCodesUsed` | library |
| 1.59% | `libz.so.1.2.11` | `inflateBackEnd` | library |
| 1.55% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.38% | `libz.so.1.2.11` | `inflate` | library |
| 1.18% | `python` | `PyBytes_FromStringAndSize` | str |
| 1.06% | `python` | `type_new` | memory |
| 1.04% | `python` | `tupledealloc` | memory |
| 0.89% | `python` | `PyObject_Free` | dynamic |
| 0.80% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.74% | `python` | `long_dealloc` | memory |
| 0.71% | `python` | `gc_collect_main` | gc |
| 0.69% | `python` | `list_dealloc` | memory |
| 0.65% | `python` | `visit_decref` | gc |
| 0.61% | `python` | `deduce_unreachable` | unknown |
| 0.51% | `python` | `visit_reachable` | gc |

## fannkuch

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 50.84% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.17% | `python` | `list_ass_slice_lock_held` | list |
| 4.98% | `python` | `list_dealloc` | memory |
| 4.33% | `python` | `PySlice_AdjustIndices` | miscobj |
| 3.56% | `python` | `PySlice_Unpack` | miscobj |
| 3.37% | `python` | `list_subscript` | list |
| 2.62% | `python` | `list_new_prealloc` | memory |
| 2.57% | `python` | `_PyLong_Add` | int |
| 2.51% | `python` | `slice_dealloc` | memory |
| 2.49% | `python` | `_PyBuildSlice_Consume2` | unknown |
| 2.38% | `python` | `PySlice_New` | memory |
| 1.45% | `python` | `list_ass_subscript` | list |
| 1.00% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.92% | `python` | `PyObject_GetItem` | dynamic |
| 0.80% | `python` | `ins1` | unknown |
| 0.80% | `python` | `_PyLong_Subtract` | int |
| 0.76% | `python` | `PyMem_Malloc` | memory |
| 0.75% | `python` | `PyNumber_AsSsize_t` | dynamic |
| 0.60% | `python` | `list_pop` | list |
| 0.59% | `python` | `PyObject_SetItem` | dynamic |

## float

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 41.73% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.97% | `libm-2.31.so` | `f64xsubf128` | library |
| 2.53% | `python` | `subtype_traverse` | gc |
| 2.33% | `python` | `visit_decref` | gc |
| 2.09% | `python` | `gc_collect_main` | gc |
| 1.95% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.88% | `python` | `visit_reachable` | gc |
| 1.84% | `python` | `deduce_unreachable` | unknown |
| 1.47% | `python` | `float_div` | float |
| 1.39% | `python` | `PyFloat_FromDouble` | float |
| 1.18% | `python` | `slot_tp_init` | unknown |
| 1.13% | `python` | `type_new` | memory |
| 1.10% | `python` | `_PyObject_Malloc` | memory |
| 1.09% | `python` | `_PyEval_EvalFrameDefault.cold` | interpreter |
| 1.07% | `python` | `object_new` | memory |
| 0.98% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.87% | `python` | `long_dealloc` | memory |
| 0.83% | `python` | `clear_slots` | unknown |
| 0.79% | `python` | `PyLong_FromLong` | int |
| 0.77% | `python` | `PyFloat_AsDouble` | float |
| 0.76% | `python` | `tupledealloc` | memory |
| 0.69% | `python` | `float_dealloc` | memory |
| 0.68% | `python` | `_PyObject_Free` | memory |
| 0.62% | `python` | `binary_iop1` | unknown |
| 0.57% | `python` | `binary_op1` | unknown |
| 0.54% | `python` | `subtype_dealloc` | memory |
| 0.53% | `python` | `_PyCode_New` | memory |
| 0.53% | `python` | `list_dealloc` | memory |

## gc_collect

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.36% | `python` | `gc_collect_main` | gc |
| 14.44% | `python` | `visit_decref` | gc |
| 14.10% | `python` | `visit_reachable` | gc |
| 11.19% | `python` | `deduce_unreachable` | unknown |
| 8.61% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.80% | `python` | `dict_traverse` | gc |
| 2.90% | `python` | `subtype_traverse` | gc |
| 1.98% | `python` | `func_traverse` | gc |
| 1.65% | `python` | `set_traverse` | gc |
| 0.88% | `python` | `tupletraverse` | tuple |
| 0.87% | `python` | `type_traverse` | gc |
| 0.82% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.77% | `python` | `PyType_GenericAlloc` | memory |
| 0.75% | `python` | `list_traverse` | gc |
| 0.60% | `python` | `subtype_dealloc` | memory |
| 0.56% | `python` | `PyObject_GC_Del` | gc |
| 0.54% | `python` | `meth_traverse` | gc |

## gc_traversal

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 28.85% | `python` | `visit_reachable` | gc |
| 20.91% | `python` | `visit_decref` | gc |
| 13.70% | `python` | `list_traverse` | gc |
| 8.63% | `python` | `gc_collect_main` | gc |
| 7.33% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.74% | `python` | `deduce_unreachable` | unknown |
| 1.73% | `python` | `dict_traverse` | gc |
| 1.01% | `python` | `PyLong_FromLong` | int |
| 0.75% | `python` | `func_traverse` | gc |
| 0.63% | `python` | `long_dealloc` | memory |
| 0.61% | `python` | `subtype_traverse` | gc |
| 0.60% | `python` | `set_traverse` | gc |
| 0.53% | `python` | `type_new` | memory |

## generators

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 50.47% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.67% | `python` | `gen_dealloc` | memory |
| 2.64% | `python` | `gc_collect_main` | gc |
| 2.55% | `python` | `deduce_unreachable` | unknown |
| 2.24% | `python` | `long_add` | int |
| 2.12% | `python` | `make_gen` | unknown |
| 1.80% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.69% | `python` | `subtype_traverse` | gc |
| 1.56% | `python` | `visit_reachable` | gc |
| 1.54% | `python` | `visit_decref` | gc |
| 1.44% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.34% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.26% | `python` | `range_subscript` | unknown |
| 1.25% | `python` | `long_dealloc` | memory |
| 1.06% | `python` | `subtype_dealloc` | memory |
| 0.79% | `python` | `_PyObject_New` | memory |
| 0.78% | `python` | `make_range_object` | unknown |
| 0.77% | `python` | `type_new` | memory |
| 0.52% | `python` | `PyType_GenericAlloc` | memory |
| 0.51% | `python` | `long_richcompare` | int |
| 0.51% | `python` | `PyNumber_Add` | dynamic |

## genshi

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 50.67% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 1.70% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.45% | `python` | `tupledealloc` | memory |
| 1.27% | `python` | `insertdict` | dict |
| 1.07% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.01% | `python` | `type_new` | memory |
| 0.99% | `python` | `insert_to_emptydict` | dict |
| 0.99% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.95% | `python` | `_PyObject_GC_New` | gc |
| 0.94% | `python` | `dictresize` | dict |
| 0.92% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.91% | `python` | `PyObject_Str` | dynamic |
| 0.88% | `python` | `dict_dealloc` | memory |
| 0.86% | `python` | `dict_get` | dict |
| 0.75% | `python` | `PyObject_GC_Del` | gc |
| 0.73% | `python` | `gc_collect_main` | gc |
| 0.72% | `python` | `PyDict_GetItemRef` | dict |
| 0.72% | `python` | `object_isinstance` | dynamic |
| 0.71% | `python` | `_Py_type_getattro` | lookup |
| 0.67% | `python` | `_PyDict_FromItems` | dict |
| 0.64% | `python` | `deduce_unreachable` | unknown |
| 0.64% | `python` | `method_dealloc` | memory |
| 0.63% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.60% | `python` | `visit_decref` | gc |
| 0.53% | `python` | `PyObject_IsTrue` | dynamic |
| 0.51% | `python` | `cm_descr_get` | unknown |

## go

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 67.53% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.83% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.70% | `python` | `_PyObject_GetMethod` | dynamic |
| 1.16% | `python` | `PyDict_GetItemRef` | dict |
| 1.04% | `python` | `uop_optimize` | unknown |
| 0.94% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.92% | `python` | `long_bitwise` | int |
| 0.90% | `python` | `PyDict_SetItem` | dict |
| 0.85% | `python` | `long_dealloc` | memory |
| 0.75% | `python` | `_PyLong_Add` | int |
| 0.71% | `python` | `type_new` | memory |
| 0.51% | `python` | `gc_collect_main` | gc |
| 0.50% | `python` | `visit_decref` | gc |

## gunicorn

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 31.91% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.39% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.35% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.60% | `python` | `type_new` | memory |
| 1.56% | `python` | `tupledealloc` | memory |
| 1.11% | `python` | `gc_collect_main` | gc |
| 1.03% | `python` | `deduce_unreachable` | unknown |
| 0.94% | `python` | `visit_decref` | gc |
| 0.81% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.80% | `python` | `PyDict_GetItemRef` | dict |
| 0.79% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.78% | `python` | `subtype_dealloc` | memory |
| 0.71% | `python` | `unicode_dealloc` | memory |
| 0.67% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.65% | `python` | `_PyCode_New` | memory |
| 0.62% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.61% | `python` | `visit_reachable` | gc |
| 0.61% | `python` | `dict_dealloc` | memory |
| 0.58% | `python` | `find_name_in_mro` | lookup |
| 0.58% | `python` | `r_object` | import |
| 0.57% | `python` | `_PySuper_Lookup` | dynamic |
| 0.57% | `python` | `list_dealloc` | memory |
| 0.54% | `python` | `sre_ucs1_match` | library |
| 0.51% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.50% | `python` | `slot_tp_init` | unknown |

## hexiom

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 67.44% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.55% | `python` | `list_contains` | list |
| 2.44% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.35% | `python` | `long_richcompare` | int |
| 1.04% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.76% | `python` | `type_new` | memory |
| 0.66% | `python` | `slot_mp_subscript` | unknown |
| 0.66% | `python` | `gen_iternext` | unknown |
| 0.60% | `python` | `list_dealloc` | memory |
| 0.53% | `python` | `gc_collect_main` | gc |
| 0.52% | `python` | `builtin_sum` | unknown |

## html5lib

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 40.65% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.91% | `python` | `sre_ucs2_charset.isra.0` | library |
| 1.86% | `python` | `gc_collect_main` | gc |
| 1.77% | `python` | `PyDict_GetItemRef` | dict |
| 1.77% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.69% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.68% | `python` | `deduce_unreachable` | unknown |
| 1.37% | `python` | `visit_decref` | gc |
| 1.19% | `python` | `type_new` | memory |
| 0.87% | `python` | `visit_reachable` | gc |
| 0.81% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.78% | `python` | `sre_ucs1_count` | library |
| 0.69% | `python` | `insertdict` | dict |
| 0.68% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.67% | `python` | `tupledealloc` | memory |
| 0.59% | `python` | `set_contains_lock_held` | miscobj |
| 0.59% | `python` | `list_dealloc` | memory |
| 0.56% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.54% | `python` | `unicode_dealloc` | memory |
| 0.53% | `python` | `long_dealloc` | memory |
| 0.53% | `python` | `_PyCode_New` | memory |
| 0.51% | `python` | `dict_dealloc` | memory |

## json

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.72% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_object_unicode` | library |
| 9.77% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.61% | `python` | `PyUnicode_Substring` | str |
| 5.67% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 5.45% | `python` | `siphash13` | str |
| 5.06% | `python` | `PyDict_SetItem` | dict |
| 3.49% | `python` | `unicode_dealloc` | memory |
| 2.89% | `python` | `dictresize` | dict |
| 2.87% | `python` | `PyLong_FromString` | int |
| 2.18% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 2.15% | `python` | `dict_dealloc` | memory |
| 2.13% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.00% | `python` | `_sre_SRE_Pattern_match` | library |
| 1.36% | `_json.cpython-313-x86_64-linux-gnu.so` | `_match_number_unicode.isra.0` | library |
| 1.13% | `python` | `PyBytes_FromStringAndSize` | str |
| 1.09% | `python` | `PyObject_Free` | dynamic |
| 0.87% | `python` | `PyDict_GetItemRef` | dict |
| 0.83% | `python` | `type_new` | memory |
| 0.81% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.75% | `python` | `tupledealloc` | memory |
| 0.67% | `python` | `insert_to_emptydict` | dict |
| 0.61% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.58% | `python` | `long_dealloc` | memory |
| 0.58% | `python` | `sre_ucs1_match` | library |
| 0.56% | `python` | `gc_collect_main` | gc |
| 0.54% | `python` | `deduce_unreachable` | unknown |
| 0.53% | `python` | `unicode_hash` | str |
| 0.52% | `libc-2.31.so` | `malloc` | libc |
| 0.50% | `python` | `visit_decref` | gc |

## json_dumps

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 16.24% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.33% | `_json.cpython-313-x86_64-linux-gnu.so` | `encoder_encode_key_value` | library |
| 6.57% | `python` | `PyUnicode_New` | memory |
| 4.92% | `python` | `_PyUnicodeWriter_WriteStr` | str |
| 4.76% | `python` | `unicode_dealloc` | memory |
| 3.43% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 3.17% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.77% | `_json.cpython-313-x86_64-linux-gnu.so` | `py_encode_basestring_ascii` | library |
| 2.31% | `python` | `vgetargskeywords.constprop.0` | calls |
| 2.27% | `python` | `PyDict_GetItemRef` | dict |
| 1.64% | `python` | `tupledealloc` | memory |
| 1.56% | `python` | `resize_compact` | str |
| 1.56% | `python` | `long_to_decimal_string` | int |
| 1.40% | `python` | `_PyObject_Malloc` | memory |
| 1.30% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.23% | `python` | `PyDict_Next` | dict |
| 1.14% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.08% | `python` | `PyFunction_NewWithQualName` | memory |
| 1.08% | `python` | `PyDict_SetItem` | dict |
| 0.91% | `python` | `object_isinstance` | dynamic |
| 0.85% | `python` | `_PyLong_New` | memory |
| 0.79% | `python` | `type_new` | memory |
| 0.77% | `python` | `PyDict_DelItem` | dict |
| 0.72% | `python` | `_Py_type_getattro` | lookup |
| 0.72% | `python` | `long_hash` | int |
| 0.71% | `python` | `func_dealloc` | memory |
| 0.70% | `python` | `_Py_dict_lookup` | lookup |
| 0.67% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.65% | `python` | `PyTuple_New` | memory |
| 0.63% | `python` | `PyDict_Contains` | dict |
| 0.62% | `python` | `long_dealloc` | memory |
| 0.56% | `python` | `dict_dealloc` | memory |
| 0.54% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.54% | `python` | `PyMem_Free` | memory |
| 0.54% | `_json.cpython-313-x86_64-linux-gnu.so` | `encoder_listencode_obj` | library |
| 0.52% | `python` | `gc_collect_main` | gc |
| 0.50% | `python` | `deduce_unreachable` | unknown |

## json_loads

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 19.50% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_object_unicode` | library |
| 10.28% | `python` | `PyUnicode_Substring` | str |
| 7.52% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.56% | `python` | `siphash13` | str |
| 5.96% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 4.97% | `python` | `PyDict_SetItem` | dict |
| 4.09% | `python` | `unicode_dealloc` | memory |
| 3.12% | `python` | `PyLong_FromString` | int |
| 2.41% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.13% | `python` | `dictresize` | dict |
| 1.35% | `python` | `dict_dealloc` | memory |
| 1.30% | `python` | `PyBytes_FromStringAndSize` | str |
| 1.12% | `_json.cpython-313-x86_64-linux-gnu.so` | `_match_number_unicode.isra.0` | library |
| 1.00% | `python` | `PyObject_Free` | dynamic |
| 0.97% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.96% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.95% | `python` | `type_new` | memory |
| 0.95% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_array_unicode` | library |
| 0.63% | `python` | `deduce_unreachable` | unknown |
| 0.62% | `python` | `unicode_hash` | str |
| 0.59% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.58% | `python` | `visit_decref` | gc |
| 0.56% | `python` | `gc_collect_main` | gc |
| 0.52% | `python` | `long_dealloc` | memory |
| 0.52% | `python` | `PyDict_GetItemRef` | dict |
| 0.51% | `python` | `tupledealloc` | memory |

## logging

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 50.26% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.10% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.07% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 2.05% | `python` | `PyDict_GetItemRef` | dict |
| 1.70% | `python` | `dict_dealloc` | memory |
| 1.67% | `python` | `PyCode_Addr2Line` | exceptions |
| 1.60% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.18% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.82% | `python` | `tupledealloc` | memory |
| 0.67% | `python` | `type_new` | memory |
| 0.65% | `python` | `long_dealloc` | memory |
| 0.58% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 0.58% | `python` | `unicode_subscript` | str |
| 0.58% | `python` | `PyObject_GetAttr` | dynamic |
| 0.55% | `python` | `PyLong_FromLong` | int |
| 0.53% | `python` | `unicode_dealloc` | memory |
| 0.52% | `python` | `vgetargs1_impl` | calls |

## mako

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 44.68% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.30% | `python` | `PyObject_Str` | dynamic |
| 5.43% | `python` | `unicode_replace` | str |
| 2.81% | `python` | `_PyUnicode_JoinArray` | str |
| 2.21% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.54% | `python` | `unicode_dealloc` | memory |
| 1.39% | `python` | `dequeiter_next_lock_held.isra.0` | miscobj |
| 1.31% | `python` | `deque_append_lock_held` | miscobj |
| 1.29% | `python` | `type_new` | memory |
| 1.23% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.00% | `python` | `list_dealloc` | memory |
| 0.87% | `python` | `PySequence_List` | dynamic |
| 0.83% | `python` | `visit_decref` | gc |
| 0.79% | `python` | `gc_collect_main` | gc |
| 0.78% | `python` | `deduce_unreachable` | unknown |
| 0.67% | `python` | `sre_ucs2_charset.isra.0` | library |
| 0.60% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.54% | `python` | `deque_clear` | miscobj |
| 0.54% | `python` | `visit_reachable` | gc |
| 0.53% | `python` | `_PyCode_New` | memory |

## mdp

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.01% | `python` | `tuplehash` | tuple |
| 23.12% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 12.12% | `python` | `long_hash` | int |
| 5.51% | `python` | `dict_subscript` | dict |
| 3.04% | `python` | `tuplerichcompare` | tuple |
| 1.39% | `python` | `insertdict` | dict |
| 1.23% | `python` | `_PyLong_GCD` | int |
| 1.19% | `python` | `_PySuper_Lookup` | dynamic |
| 1.11% | `python` | `PyDict_GetItemRef` | dict |
| 0.90% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.84% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.80% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.58% | `python` | `gen_dealloc` | memory |
| 0.56% | `python` | `builtin_sum` | unknown |
| 0.56% | `python` | `PyObject_GetItem` | dynamic |
| 0.55% | `python` | `set_contains_lock_held` | miscobj |
| 0.54% | `python` | `tupledealloc` | memory |

## meteor_contest

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 29.66% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.11% | `python` | `set_issubset_impl` | miscobj |
| 5.69% | `python` | `setiter_iternext` | miscobj |
| 4.29% | `python` | `set_difference` | miscobj |
| 4.26% | `python` | `set_lookkey` | miscobj |
| 3.83% | `python` | `set_dealloc` | memory |
| 2.81% | `python` | `builtin_min` | unknown |
| 2.10% | `python` | `list_dealloc` | memory |
| 1.84% | `python` | `set_add_entry` | miscobj |
| 1.52% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.42% | `python` | `list_subscript` | list |
| 1.35% | `python` | `PyObject_GC_Del` | gc |
| 1.14% | `python` | `long_richcompare` | int |
| 1.13% | `python` | `PyObject_RichCompare` | dynamic |
| 0.99% | `python` | `set_table_resize` | miscobj |
| 0.98% | `python` | `type_new` | memory |
| 0.97% | `python` | `make_new_set` | memory |
| 0.86% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.74% | `python` | `set_intersection` | miscobj |
| 0.69% | `python` | `gc_collect_main` | gc |
| 0.68% | `python` | `deduce_unreachable` | unknown |
| 0.67% | `python` | `_PyObject_GC_New` | gc |
| 0.65% | `python` | `list_iter` | list |
| 0.64% | `python` | `visit_decref` | gc |
| 0.54% | `python` | `PyMem_Malloc` | memory |

## mypy2

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 35.05% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.54% | `python` | `gc_collect_main` | gc |
| 6.56% | `python` | `deduce_unreachable` | unknown |
| 2.75% | `python` | `visit_decref` | gc |
| 2.60% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.60% | `python` | `PyDict_GetItemRef` | dict |
| 1.49% | `python` | `subtype_traverse` | gc |
| 1.47% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.37% | `python` | `object_isinstance` | dynamic |
| 1.28% | `python` | `visit_reachable` | gc |
| 1.24% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_object_unicode` | library |
| 1.21% | `python` | `_PySuper_Lookup` | dynamic |
| 1.05% | `python` | `list_dealloc` | memory |
| 0.98% | `python` | `PyObject_SetAttr` | dynamic |
| 0.94% | `python` | `PyUnicode_Substring` | str |
| 0.94% | `python` | `clear_slots` | unknown |
| 0.91% | `python` | `subtype_dealloc` | memory |
| 0.88% | `python` | `siphash13` | str |
| 0.86% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.78% | `python` | `tupledealloc` | memory |
| 0.78% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.77% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.77% | `python` | `dict_dealloc` | memory |
| 0.74% | `python` | `slot_tp_init` | unknown |
| 0.69% | `python` | `PyObject_GC_Del` | gc |
| 0.63% | `python` | `unicode_dealloc` | memory |
| 0.63% | `python` | `object_new` | memory |
| 0.61% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.59% | `python` | `PyDict_SetItem` | dict |
| 0.56% | `python` | `list_traverse` | gc |

## nbody

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 68.35% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.46% | `python` | `PyFloat_FromDouble` | float |
| 2.78% | `libm-2.31.so` | `f64xsubf128` | library |
| 1.79% | `python` | `float_dealloc` | memory |
| 1.00% | `python` | `float_pow` | float |
| 0.98% | `python` | `type_new` | memory |
| 0.68% | `python` | `gc_collect_main` | gc |
| 0.66% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.60% | `python` | `deduce_unreachable` | unknown |
| 0.52% | `python` | `visit_decref` | gc |

## nqueens

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 46.08% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.08% | `python` | `set_vectorcall` | miscobj |
| 2.12% | `python` | `list_dealloc` | memory |
| 1.69% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.57% | `python` | `PyFunction_NewWithQualName` | memory |
| 1.47% | `python` | `gen_iternext` | unknown |
| 1.43% | `python` | `set_dealloc` | memory |
| 1.31% | `python` | `func_dealloc` | memory |
| 1.27% | `python` | `_PyLong_Add` | int |
| 1.14% | `python` | `_PyBuildSlice_Consume2` | unknown |
| 1.08% | `python` | `PyList_New` | memory |
| 1.04% | `python` | `uop_optimize` | unknown |
| 1.03% | `python` | `type_new` | memory |
| 0.88% | `python` | `tupledealloc` | memory |
| 0.88% | `python` | `list_subscript` | list |
| 0.86% | `python` | `make_gen` | unknown |
| 0.84% | `python` | `gen_dealloc` | memory |
| 0.71% | `python` | `deduce_unreachable` | unknown |
| 0.69% | `python` | `gc_collect_main` | gc |
| 0.68% | `python` | `visit_decref` | gc |
| 0.66% | `python` | `PySlice_Unpack` | miscobj |
| 0.60% | `python` | `PyLong_FromLong` | int |
| 0.59% | `python` | `PyMem_Malloc` | memory |
| 0.58% | `python` | `list_ass_slice_lock_held` | list |
| 0.54% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.52% | `python` | `_PyCode_New` | memory |
| 0.52% | `python` | `_PyLong_Subtract` | int |

## pathlib

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 19.96% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.07% | `python` | `long_dealloc` | memory |
| 1.73% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.39% | `[kernel.kallsyms]` | `__d_lookup_rcu` | kernel |
| 1.28% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.23% | `python` | `k_mul` | int |
| 1.21% | `libpthread-2.31.so` | `__pthread_mutex_lock` | library |
| 1.18% | `python` | `_PySuper_Lookup` | dynamic |
| 1.15% | `[kernel.kallsyms]` | `ext4_htree_store_dirent` | kernel |
| 1.09% | `python` | `_PyLong_New` | memory |
| 1.06% | `[kernel.kallsyms]` | `memset_erms` | kernel |
| 1.05% | `[kernel.kallsyms]` | `__ext4fs_dirhash` | kernel |
| 1.02% | `libpthread-2.31.so` | `pthread_mutex_unlock` | library |
| 0.92% | `python` | `path_converter` | unknown |
| 0.91% | `python` | `tupledealloc` | memory |
| 0.87% | `python` | `vectorcall_method` | calls |
| 0.85% | `python` | `list_dealloc` | memory |
| 0.85% | `python` | `ScandirIterator_iternext` | unknown |
| 0.84% | `python` | `PyUnicode_FSConverter` | str |
| 0.82% | `python` | `type_new` | memory |
| 0.82% | `python` | `_Py_dict_lookup` | lookup |
| 0.82% | `python` | `PyLong_FromLong` | int |
| 0.79% | `python` | `unicode_decode_utf8` | str |
| 0.77% | `python` | `x_add` | int |
| 0.76% | `[kernel.kallsyms]` | `filldir64` | kernel |
| 0.71% | `python` | `_Py_type_getattro` | lookup |
| 0.69% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.66% | `python` | `method_dealloc` | memory |
| 0.66% | `[kernel.kallsyms]` | `strncpy_from_user` | kernel |
| 0.66% | `python` | `PyObject_GC_Del` | gc |
| 0.66% | `python` | `PyEval_RestoreThread` | interpreter |
| 0.62% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.61% | `python` | `object_isinstance` | dynamic |
| 0.61% | `python` | `unicode_dealloc` | memory |
| 0.60% | `python` | `_PyUnicode_JoinArray` | str |
| 0.58% | `python` | `slot_tp_init` | unknown |
| 0.58% | `python` | `PyUnicode_DecodeFSDefault` | str |
| 0.57% | `[kernel.kallsyms]` | `__virt_addr_valid` | kernel |
| 0.56% | `python` | `deduce_unreachable` | unknown |
| 0.56% | `python` | `gc_collect_main` | gc |
| 0.56% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.55% | `[kernel.kallsyms]` | `kmem_cache_alloc` | kernel |
| 0.54% | `python` | `sre_ucs1_match` | library |
| 0.52% | `[kernel.kallsyms]` | `link_path_walk.part.0` | kernel |
| 0.51% | `python` | `visit_decref` | gc |
| 0.51% | `python` | `tp_new_wrapper` | memory |
| 0.51% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |

## pickle

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.28% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `save` | library |
| 12.31% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_put.isra.0` | library |
| 6.92% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_write_bytes` | library |
| 6.33% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.01% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.75% | `python` | `PyDict_Next` | dict |
| 2.56% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_get.isra.0` | library |
| 2.41% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pickler_dealloc` | library |
| 1.92% | `python` | `PyUnicode_AsUTF8AndSize` | str |
| 1.69% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.46% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_Write` | library |
| 0.98% | `python` | `type_new` | memory |
| 0.71% | `python` | `gc_collect_main` | gc |
| 0.68% | `python` | `visit_decref` | gc |
| 0.67% | `python` | `deduce_unreachable` | unknown |
| 0.63% | `python` | `PyMem_Free` | memory |
| 0.56% | `python` | `PyMem_Malloc` | memory |
| 0.53% | `python` | `tupledealloc` | memory |

## pickle_dict

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 46.26% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `save` | library |
| 12.57% | `python` | `PyDict_Next` | dict |
| 10.00% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_Write` | library |
| 4.40% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.90% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_put.isra.0` | library |
| 2.75% | `python` | `PyLong_AsLongAndOverflow` | int |
| 1.13% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.83% | `python` | `type_new` | memory |
| 0.65% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pickler_dealloc` | library |
| 0.64% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005cd4` | library |
| 0.62% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005e54` | library |
| 0.54% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.53% | `python` | `gc_collect_main` | gc |
| 0.51% | `python` | `visit_decref` | gc |

## pickle_list

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 39.98% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `save` | library |
| 12.59% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_Write` | library |
| 6.72% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.81% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_put.isra.0` | library |
| 3.83% | `python` | `PyLong_AsLongAndOverflow` | int |
| 2.02% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.28% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.24% | `python` | `type_new` | memory |
| 1.07% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pickler_dealloc` | library |
| 0.79% | `python` | `gc_collect_main` | gc |
| 0.75% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005cd4` | library |
| 0.68% | `python` | `visit_decref` | gc |
| 0.67% | `python` | `deduce_unreachable` | unknown |
| 0.59% | `python` | `_PyThreadState_GetCurrent` | unknown |
| 0.59% | `python` | `_PyCode_New` | memory |

## pickle_pure_python

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 50.06% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.64% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.61% | `python` | `bytes_concat` | str |
| 2.34% | `python` | `dict_get` | dict |
| 2.23% | `python` | `unicode_encode` | str |
| 1.71% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.65% | `python` | `PyObject_Free` | dynamic |
| 1.53% | `python` | `insertdict` | dict |
| 1.43% | `python` | `_PyLong_New` | memory |
| 1.41% | `python` | `long_dealloc` | memory |
| 1.15% | `python` | `PyDict_GetItemRef` | dict |
| 1.01% | `python` | `PyType_GetModuleByDef` | dynamic |
| 1.00% | `python` | `write_bytes` | unknown |
| 0.97% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.88% | `python` | `tupledealloc` | memory |
| 0.86% | `python` | `unicode_encode_utf8` | str |
| 0.77% | `python` | `PyDict_Contains` | dict |
| 0.71% | `python` | `type_new` | memory |
| 0.68% | `python` | `PySys_Audit` | unknown |
| 0.60% | `python` | `long_hash` | int |
| 0.58% | `python` | `builtin_id` | unknown |
| 0.53% | `_struct.cpython-313-x86_64-linux-gnu.so` | `s_pack` | library |

## pidigits

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.84% | `python` | `x_divrem` | int |
| 19.54% | `python` | `k_mul` | int |
| 12.29% | `python` | `x_add` | int |
| 7.76% | `python` | `x_sub` | int |
| 6.55% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.46% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.85% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.72% | `python` | `type_new` | memory |

## pprint

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 52.63% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.16% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.72% | `python` | `long_to_decimal_string` | int |
| 2.36% | `python` | `_Py_type_getattro_impl` | dynamic |
| 2.03% | `python` | `tupledealloc` | memory |
| 1.85% | `python` | `_Py_type_getattro` | lookup |
| 1.73% | `python` | `PyUnicode_Format` | str |
| 1.68% | `python` | `_PyUnicode_JoinArray` | str |
| 1.66% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.35% | `python` | `unicode_dealloc` | memory |
| 1.18% | `python` | `set_contains_lock_held` | miscobj |
| 1.08% | `python` | `_Py_dict_lookup` | lookup |
| 0.95% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.91% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 0.89% | `python` | `builtin_issubclass` | unknown |
| 0.85% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.79% | `python` | `PyDict_Contains` | dict |
| 0.78% | `python` | `insertdict` | dict |
| 0.73% | `python` | `list_dealloc` | memory |
| 0.70% | `python` | `slot_tp_init` | unknown |
| 0.70% | `python` | `_PyLong_New` | memory |
| 0.67% | `python` | `_PyObject_Malloc` | memory |
| 0.66% | `python` | `slot_tp_richcompare` | dynamic |
| 0.65% | `python` | `meth_dealloc` | memory |
| 0.59% | `python` | `PyObject_GetAttr` | dynamic |
| 0.58% | `python` | `_PyFrame_PushUnchecked.isra.0` | unknown |
| 0.55% | `python` | `PyObject_GC_Del` | gc |
| 0.53% | `python` | `builtin_getattr` | lookup |
| 0.52% | `python` | `object_new` | memory |

## pycparser

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 40.26% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 12.71% | `python` | `sre_ucs1_match` | library |
| 2.50% | `python` | `_sre_SRE_Pattern_match` | library |
| 2.50% | `python` | `PyDict_GetItemRef` | dict |
| 2.22% | `python` | `gc_collect_main` | gc |
| 2.17% | `python` | `deduce_unreachable` | unknown |
| 2.16% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.99% | `python` | `object_new` | memory |
| 1.49% | `python` | `dict_get` | dict |
| 1.32% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.29% | `python` | `subtype_dealloc` | memory |
| 1.22% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.21% | `python` | `visit_decref` | gc |
| 1.07% | `python` | `visit_reachable` | gc |
| 1.06% | `python` | `subtype_traverse` | gc |
| 0.88% | `python` | `list_ass_slice_lock_held` | list |
| 0.80% | `python` | `list_dealloc` | memory |
| 0.76% | `python` | `sre_ucs1_count` | library |
| 0.72% | `python` | `object_isinstance` | dynamic |
| 0.70% | `python` | `slot_mp_ass_subscript` | unknown |
| 0.59% | `python` | `PyDict_Contains` | dict |
| 0.55% | `python` | `PyObject_Vectorcall` | dynamic |
| 0.54% | `python` | `PyObject_GC_Del` | gc |
| 0.52% | `python` | `PyNumber_Negative` | dynamic |
| 0.51% | `python` | `sre_ucs2_charset.isra.0` | library |
| 0.50% | `python` | `list_subscript` | list |

## pyflate

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 55.47% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.57% | `python` | `list_dealloc` | memory |
| 4.15% | `python` | `list_ass_slice_lock_held` | list |
| 2.18% | `python` | `long_dealloc` | memory |
| 2.11% | `python` | `_PyLong_Add` | int |
| 1.91% | `python` | `list_subscript` | list |
| 1.81% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.68% | `python` | `bytes_subscript` | str |
| 1.47% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.36% | `python` | `list_concat` | list |
| 1.34% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.33% | `python` | `_PyLong_Subtract` | int |
| 1.17% | `python` | `long_lshift` | int |
| 0.94% | `python` | `stringlib_bytes_join.lto_priv.1` | str |
| 0.93% | `python` | `_PyLong_New` | memory |
| 0.84% | `python` | `PySlice_Unpack` | miscobj |
| 0.83% | `python` | `PyObject_Free` | dynamic |
| 0.62% | `python` | `list_sort_impl` | list |
| 0.57% | `python` | `long_rshift` | int |
| 0.53% | `python` | `PyObject_GetItem` | dynamic |
| 0.53% | `python` | `_PyBuildSlice_Consume2` | unknown |

## pylint

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 29.62% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.90% | `python` | `gc_collect_main` | gc |
| 5.28% | `python` | `deduce_unreachable` | unknown |
| 3.43% | `python` | `visit_decref` | gc |
| 2.85% | `python` | `visit_reachable` | gc |
| 2.01% | `python` | `subtype_traverse` | gc |
| 1.76% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.69% | `python` | `PyDict_GetItemRef` | dict |
| 1.67% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.32% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.08% | `python` | `find_name_in_mro` | lookup |
| 1.00% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.96% | `python` | `object_isinstance` | dynamic |
| 0.93% | `python` | `tupledealloc` | memory |
| 0.84% | `python` | `dict_traverse` | gc |
| 0.78% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.74% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.72% | `python` | `dict_dealloc` | memory |
| 0.67% | `python` | `PyObject_SetAttr` | dynamic |
| 0.61% | `python` | `list_traverse` | gc |
| 0.60% | `python` | `type_new` | memory |
| 0.60% | `python` | `list_dealloc` | memory |
| 0.56% | `python` | `gen_dealloc` | memory |
| 0.52% | `python` | `subtype_dealloc` | memory |
| 0.50% | `python` | `PyObject_GC_Del` | gc |
| 0.50% | `python` | `PyObject_GetAttr` | dynamic |

## python_startup

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 8.79% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.73% | `python` | `type_new` | memory |
| 3.37% | `python` | `_PyCode_New` | memory |
| 3.09% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 3.04% | `python` | `r_object` | import |
| 2.71% | `python` | `gc_collect_main` | gc |
| 2.66% | `python` | `visit_decref` | gc |
| 2.44% | `python` | `deduce_unreachable` | unknown |
| 2.20% | `python` | `visit_reachable` | gc |
| 2.09% | `python` | `PyUnicode_FromKindAndData` | str |
| 1.61% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 1.54% | `ld-2.31.so` | `_dl_rtld_di_serinfo` | library |
| 1.35% | `python` | `siphash13` | str |
| 1.27% | `python` | `_Py_hashtable_get` | unknown |
| 1.07% | `python` | `tupledealloc` | memory |
| 0.98% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.95% | `python` | `unicode_decode_utf8` | str |
| 0.86% | `python` | `type_ready` | dynamic |
| 0.84% | `python` | `dict_traverse` | gc |
| 0.82% | `python` | `find_name_in_mro` | lookup |
| 0.82% | `[kernel.kallsyms]` | `filemap_map_pages` | kernel |
| 0.79% | `python` | `PyDict_SetItem` | dict |
| 0.77% | `[kernel.kallsyms]` | `native_irq_return_iret` | kernel |
| 0.68% | `python` | `unicode_dealloc` | memory |
| 0.64% | `python` | `insertdict` | dict |
| 0.62% | `python` | `_Py_dict_lookup` | lookup |
| 0.60% | `python` | `dictresize` | dict |
| 0.59% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.54% | `python` | `PyDict_GetItemRef` | dict |
| 0.54% | `python` | `PyBytes_FromStringAndSize` | str |
| 0.54% | `[kernel.kallsyms]` | `sync_regs` | kernel |

## python_startup_no_site

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 8.39% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.23% | `python` | `type_new` | memory |
| 3.40% | `python` | `_PyCode_New` | memory |
| 3.13% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 3.07% | `python` | `r_object` | import |
| 2.84% | `python` | `gc_collect_main` | gc |
| 2.67% | `python` | `visit_decref` | gc |
| 2.58% | `python` | `deduce_unreachable` | unknown |
| 2.34% | `python` | `visit_reachable` | gc |
| 2.11% | `python` | `PyUnicode_FromKindAndData` | str |
| 2.01% | `ld-2.31.so` | `_dl_rtld_di_serinfo` | library |
| 1.67% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 1.39% | `python` | `siphash13` | str |
| 1.16% | `python` | `_Py_hashtable_get` | unknown |
| 1.06% | `python` | `tupledealloc` | memory |
| 1.01% | `python` | `unicode_decode_utf8` | str |
| 0.98% | `python` | `dict_traverse` | gc |
| 0.98% | `python` | `type_ready` | dynamic |
| 0.97% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.84% | `[kernel.kallsyms]` | `native_irq_return_iret` | kernel |
| 0.83% | `python` | `PyDict_SetItem` | dict |
| 0.80% | `python` | `find_name_in_mro` | lookup |
| 0.78% | `[kernel.kallsyms]` | `filemap_map_pages` | kernel |
| 0.75% | `python` | `insertdict` | dict |
| 0.69% | `python` | `dictresize` | dict |
| 0.61% | `python` | `unicode_dealloc` | memory |
| 0.60% | `python` | `_Py_dict_lookup` | lookup |
| 0.59% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.59% | `[kernel.kallsyms]` | `sync_regs` | kernel |
| 0.55% | `python` | `PyBytes_FromStringAndSize` | str |
| 0.53% | `libc-2.31.so` | `wcsrtombs` | libc |
| 0.53% | `python` | `PyDict_GetItemRef` | dict |
| 0.53% | `libc-2.31.so` | `_dl_addr` | libc |
| 0.52% | `python` | `dict_dealloc` | memory |

## raytrace

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 63.64% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.47% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.83% | `python` | `subtype_dealloc` | memory |
| 2.10% | `python` | `PyFloat_FromDouble` | float |
| 1.59% | `python` | `vectorcall_maybe.constprop.0` | unknown |
| 1.43% | `python` | `PyType_GenericAlloc` | memory |
| 1.38% | `python` | `float_dealloc` | memory |
| 1.03% | `python` | `PyNumber_Subtract` | dynamic |
| 0.83% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.82% | `python` | `PyObject_GC_Del` | gc |
| 0.76% | `python` | `_PyObject_InitInlineValues` | dynamic |
| 0.69% | `python` | `float_mul` | float |
| 0.68% | `python` | `PyNumber_Multiply` | dynamic |
| 0.59% | `python` | `convert_to_double` | unknown |
| 0.58% | `python` | `float_add` | float |
| 0.54% | `python` | `float_sub` | float |
| 0.50% | `python` | `tupledealloc` | memory |

## regex_compile

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 53.46% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.03% | `python` | `sre_ucs1_match` | library |
| 2.16% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.60% | `python` | `PyLong_FromLong` | int |
| 1.40% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.19% | `python` | `long_dealloc` | memory |
| 1.15% | `python` | `PyNumber_AsSsize_t` | dynamic |
| 0.81% | `python` | `tupledealloc` | memory |
| 0.80% | `python` | `object_isinstance` | dynamic |
| 0.78% | `python` | `list_dealloc` | memory |
| 0.76% | `python` | `sre_ucs2_charset.isra.0` | library |
| 0.66% | `python` | `type_new` | memory |
| 0.64% | `python` | `bytearray_ass_subscript` | miscobj |
| 0.56% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.55% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.53% | `python` | `slot_mp_subscript` | unknown |

## regex_dna

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 30.98% | `python` | `sre_ucs1_match` | library |
| 28.43% | `python` | `sre_ucs2_charset.isra.0` | library |
| 9.55% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.14% | `python` | `sre_search` | library |
| 3.28% | `libm-2.31.so` | `__fmod_finite` | library |
| 1.18% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.08% | `_bisect.cpython-313-x86_64-linux-gnu.so` | `_bisect_bisect_right` | library |
| 0.95% | `python` | `float_richcompare` | float |
| 0.94% | `python` | `pattern_subx` | library |
| 0.75% | `python` | `PyFloat_FromDouble` | float |
| 0.63% | `python` | `stringlib_bytes_join.lto_priv.1` | str |
| 0.59% | `python` | `float_rem` | float |
| 0.55% | `python` | `type_new` | memory |

## regex_effbot

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 37.90% | `python` | `sre_ucs1_match` | library |
| 16.33% | `python` | `sre_ucs2_charset.isra.0` | library |
| 6.24% | `python` | `sre_search` | library |
| 6.20% | `python` | `PyMem_Free` | memory |
| 6.09% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.63% | `python` | `PyMem_Malloc` | memory |
| 1.67% | `python` | `sre_ucs1_count` | library |
| 0.93% | `python` | `type_new` | memory |
| 0.69% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.66% | `python` | `gc_collect_main` | gc |
| 0.61% | `python` | `visit_decref` | gc |
| 0.59% | `python` | `deduce_unreachable` | unknown |

## regex_v8

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 31.65% | `python` | `sre_ucs1_match` | library |
| 13.37% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.81% | `python` | `sre_ucs1_count` | library |
| 3.39% | `python` | `PyCode_Addr2Line` | exceptions |
| 2.74% | `python` | `sre_search` | library |
| 1.78% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.33% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.22% | `python` | `pattern_subx` | library |
| 1.11% | `python` | `type_new` | memory |
| 1.05% | `python` | `sre_ucs1_match.cold` | library |
| 1.03% | `python` | `state_init` | unknown |
| 1.01% | `python` | `PyMem_Free` | memory |
| 0.80% | `python` | `PyLong_FromLong` | int |
| 0.74% | `python` | `deduce_unreachable` | unknown |
| 0.73% | `python` | `gc_collect_main` | gc |
| 0.70% | `python` | `visit_decref` | gc |
| 0.69% | `python` | `long_dealloc` | memory |
| 0.65% | `python` | `PyUnicode_Substring` | str |
| 0.64% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.59% | `python` | `_PyUnicode_JoinArray` | str |
| 0.59% | `python` | `list_dealloc` | memory |
| 0.55% | `libc-2.31.so` | `malloc` | libc |
| 0.53% | `python` | `unicode_dealloc` | memory |
| 0.53% | `python` | `PyMem_Malloc` | memory |
| 0.51% | `python` | `PyDict_GetItemRef` | dict |

## richards

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 60.20% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.63% | `python` | `_PyObject_GetMethod` | dynamic |
| 3.42% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.13% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 2.45% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 1.52% | `python` | `PyObject_GetAttr` | dynamic |
| 1.02% | `python` | `type_new` | memory |
| 1.00% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.89% | `python` | `PyObject_SetAttr` | dynamic |
| 0.71% | `python` | `_PyFrame_PushUnchecked.isra.0` | unknown |
| 0.70% | `python` | `gc_collect_main` | gc |
| 0.63% | `python` | `visit_decref` | gc |
| 0.61% | `python` | `deduce_unreachable` | unknown |
| 0.56% | `python` | `long_dealloc` | memory |

## richards_super

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 59.24% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.82% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.51% | `python` | `_PyObject_GetMethod` | dynamic |
| 2.79% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 2.35% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 2.10% | `python` | `_PySuper_Lookup` | dynamic |
| 1.53% | `python` | `PyObject_SetAttr` | dynamic |
| 1.50% | `python` | `PyObject_GetAttr` | dynamic |
| 0.95% | `python` | `type_new` | memory |
| 0.90% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.72% | `python` | `_PyFrame_PushUnchecked.isra.0` | unknown |
| 0.68% | `python` | `deduce_unreachable` | unknown |
| 0.62% | `python` | `gc_collect_main` | gc |
| 0.57% | `python` | `visit_decref` | gc |
| 0.51% | `python` | `long_dealloc` | memory |

## scimark

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 46.56% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.23% | `python` | `PyNumber_AsSsize_t` | dynamic |
| 3.62% | `python` | `long_dealloc` | memory |
| 3.42% | `python` | `_PyLong_Add` | int |
| 2.75% | `python` | `PyObject_GetItem` | dynamic |
| 2.48% | `python` | `PyFloat_FromDouble` | float |
| 2.39% | `array.cpython-313-x86_64-linux-gnu.so` | `array_subscr` | library |
| 2.23% | `python` | `slot_mp_subscript` | unknown |
| 2.20% | `python` | `PyType_GetModuleByDef` | dynamic |
| 1.80% | `python` | `vgetargs1_impl` | calls |
| 1.67% | `python` | `PyLong_FromLong` | int |
| 1.35% | `python` | `convertitem` | unknown |
| 1.27% | `python` | `_PyLong_Multiply` | int |
| 1.18% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.17% | `python` | `float_dealloc` | memory |
| 1.16% | `array.cpython-313-x86_64-linux-gnu.so` | `array_ass_subscr` | library |
| 1.06% | `python` | `object_isinstance` | dynamic |
| 0.86% | `python` | `PyObject_Free` | dynamic |
| 0.85% | `array.cpython-313-x86_64-linux-gnu.so` | `d_setitem` | library |
| 0.78% | `python` | `PyObject_SetItem` | dynamic |
| 0.69% | `python` | `PyArg_Parse` | calls |
| 0.63% | `python` | `PyIndex_Check` | unknown |
| 0.51% | `python` | `tupledealloc` | memory |

## spectral_norm

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 44.40% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 9.48% | `python` | `_PyLong_Add` | int |
| 3.97% | `python` | `_PyLong_Multiply` | int |
| 3.69% | `python` | `long_div` | int |
| 3.47% | `python` | `enum_next` | miscobj |
| 3.41% | `python` | `long_dealloc` | memory |
| 2.99% | `python` | `PyObject_Free` | dynamic |
| 2.66% | `python` | `float_div` | float |
| 1.77% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.69% | `python` | `convert_to_double` | unknown |
| 1.27% | `python` | `PyNumber_TrueDivide` | dynamic |
| 1.11% | `python` | `float_dealloc` | memory |
| 1.05% | `python` | `float_mul` | float |
| 0.79% | `python` | `type_new` | memory |
| 0.61% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.58% | `python` | `PyNumber_FloorDivide` | dynamic |
| 0.56% | `python` | `gc_collect_main` | gc |
| 0.55% | `python` | `visit_decref` | gc |
| 0.52% | `python` | `deduce_unreachable` | unknown |

## sqlglot

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 36.70% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.62% | `python` | `object_isinstance` | dynamic |
| 2.17% | `python` | `tupledealloc` | memory |
| 2.07% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.81% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.49% | `python` | `type_new` | memory |
| 1.29% | `python` | `method_get` | dynamic |
| 1.25% | `python` | `dictiter_iternextitem` | dict |
| 1.19% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 1.16% | `python` | `meth_dealloc` | memory |
| 0.94% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.93% | `python` | `make_gen` | unknown |
| 0.92% | `python` | `gc_collect_main` | gc |
| 0.90% | `python` | `PyObject_IsInstance` | dynamic |
| 0.87% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.86% | `python` | `deduce_unreachable` | unknown |
| 0.82% | `python` | `gen_dealloc` | memory |
| 0.79% | `python` | `visit_decref` | gc |
| 0.73% | `python` | `dictiter_dealloc` | memory |
| 0.69% | `python` | `list_dealloc` | memory |
| 0.68% | `python` | `dict_items` | dict |
| 0.66% | `python` | `insert_to_emptydict` | dict |
| 0.64% | `python` | `getset_get` | dynamic |
| 0.61% | `python` | `PyObject_GC_Del` | gc |
| 0.59% | `python` | `func_dealloc` | memory |
| 0.58% | `python` | `_PyCode_New` | memory |
| 0.57% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.56% | `python` | `visit_reachable` | gc |
| 0.55% | `python` | `PyList_New` | memory |
| 0.55% | `python` | `dictview_dealloc` | memory |
| 0.55% | `python` | `unicode_dealloc` | memory |
| 0.54% | `python` | `siphash13` | str |
| 0.53% | `python` | `slot_tp_hash` | unknown |
| 0.51% | `python` | `dictitems_iter` | unknown |

## sqlglot_optimize

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 38.19% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.98% | `python` | `object_isinstance` | dynamic |
| 2.09% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.96% | `python` | `tupledealloc` | memory |
| 1.56% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.40% | `python` | `type_new` | memory |
| 1.34% | `python` | `method_get` | dynamic |
| 1.29% | `python` | `meth_dealloc` | memory |
| 1.29% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 1.26% | `python` | `dictiter_iternextitem` | dict |
| 1.00% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.96% | `python` | `gc_collect_main` | gc |
| 0.89% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.87% | `python` | `PyObject_IsInstance` | dynamic |
| 0.83% | `python` | `list_dealloc` | memory |
| 0.82% | `python` | `deduce_unreachable` | unknown |
| 0.82% | `python` | `visit_decref` | gc |
| 0.79% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.77% | `python` | `PyList_New` | memory |
| 0.71% | `python` | `getset_get` | dynamic |
| 0.66% | `python` | `dictiter_dealloc` | memory |
| 0.59% | `python` | `dict_get` | dict |
| 0.59% | `python` | `PyObject_GC_Del` | gc |
| 0.59% | `python` | `_PyCode_New` | memory |
| 0.55% | `python` | `list_iter` | list |
| 0.53% | `python` | `_Py_dict_lookup` | lookup |
| 0.53% | `python` | `visit_reachable` | gc |
| 0.52% | `python` | `slot_tp_hash` | unknown |
| 0.51% | `python` | `unicode_dealloc` | memory |
| 0.51% | `python` | `siphash13` | str |
| 0.50% | `python` | `insertdict` | dict |

## sqlglot_parse

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 53.07% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.69% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.46% | `python` | `PyDict_Contains` | dict |
| 1.26% | `python` | `_Py_type_getattro` | lookup |
| 1.26% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.18% | `python` | `gc_collect_main` | gc |
| 1.03% | `python` | `type_new` | memory |
| 1.00% | `python` | `deduce_unreachable` | unknown |
| 0.93% | `python` | `visit_decref` | gc |
| 0.85% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.85% | `python` | `PyObject_GetAttr` | dynamic |
| 0.74% | `python` | `long_dealloc` | memory |
| 0.72% | `python` | `PyObject_RichCompare` | dynamic |
| 0.68% | `python` | `dict_get` | dict |
| 0.68% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.68% | `python` | `tupledealloc` | memory |
| 0.68% | `python` | `slot_tp_hash` | unknown |
| 0.67% | `python` | `_PyLong_Add` | int |
| 0.59% | `python` | `object_isinstance` | dynamic |
| 0.58% | `python` | `PyObject_SetAttr` | dynamic |
| 0.54% | `python` | `dict_dealloc` | memory |
| 0.52% | `python` | `object_new` | memory |
| 0.51% | `python` | `find_name_in_mro` | lookup |
| 0.51% | `python` | `visit_reachable` | gc |

## sqlglot_transpile

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 46.88% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.53% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.53% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.51% | `python` | `type_new` | memory |
| 1.30% | `python` | `gc_collect_main` | gc |
| 1.19% | `python` | `deduce_unreachable` | unknown |
| 1.04% | `python` | `visit_decref` | gc |
| 1.03% | `python` | `PyDict_Contains` | dict |
| 0.97% | `python` | `find_name_in_mro` | lookup |
| 0.95% | `python` | `_Py_type_getattro` | lookup |
| 0.91% | `python` | `dict_get` | dict |
| 0.90% | `python` | `object_isinstance` | dynamic |
| 0.82% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.78% | `python` | `tupledealloc` | memory |
| 0.78% | `python` | `PyObject_GetAttr` | dynamic |
| 0.75% | `python` | `visit_reachable` | gc |
| 0.70% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.68% | `python` | `long_dealloc` | memory |
| 0.63% | `python` | `unicode_dealloc` | memory |
| 0.56% | `python` | `PyObject_RichCompare` | dynamic |
| 0.56% | `python` | `_PyCode_New` | memory |
| 0.55% | `python` | `dict_dealloc` | memory |
| 0.51% | `python` | `_PyUnicode_JoinArray` | str |

## sqlite_synth

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 11.26% | `libpthread-2.31.so` | `__pthread_mutex_lock` | library |
| 11.06% | `libpthread-2.31.so` | `pthread_mutex_unlock` | library |
| 10.73% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.38% | `python` | `PyEval_RestoreThread` | interpreter |
| 4.28% | `libsqlite3.so.0.8.6` | `sqlite3_reset` | library |
| 2.48% | `libm-2.31.so` | `f64xsubf128` | library |
| 1.37% | `python` | `PyEval_SaveThread` | interpreter |
| 1.36% | `libsqlite3.so.0.8.6` | `sqlite3_randomness` | library |
| 1.34% | `python` | `long_dealloc` | memory |
| 1.27% | `libc-2.31.so` | `pthread_cond_signal` | libc |
| 1.19% | `python` | `PyTuple_New` | memory |
| 1.15% | `python` | `PyObject_Str` | dynamic |
| 1.06% | `python` | `tupledealloc` | memory |
| 1.00% | `_sqlite3.cpython-313-x86_64-linux-gnu.so` | `_pysqlite_query_execute` | library |
| 0.94% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.87% | `libpthread-2.31.so` | `pthread_cond_signal@@GLIBC_2.3.2` | library |
| 0.87% | `libsqlite3.so.0.8.6` | `sqlite3_value_double` | library |
| 0.81% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.78% | `python` | `PyFloat_AsDouble` | float |
| 0.72% | `python` | `type_new` | memory |
| 0.70% | `libsqlite3.so.0.8.6` | `sqlite3_preupdate_old` | library |
| 0.69% | `python` | `list_dealloc` | memory |
| 0.67% | `libsqlite3.so.0.8.6` | `sqlite3_wal_checkpoint` | library |
| 0.66% | `libsqlite3.so.0.8.6` | `sqlite3_extended_errcode` | library |
| 0.65% | `python` | `PyFloat_FromDouble` | float |
| 0.62% | `libsqlite3.so.0.8.6` | `sqlite3_vtab_config` | library |
| 0.61% | `libc-2.31.so` | `pthread_mutex_unlock` | libc |
| 0.60% | `libsqlite3.so.0.8.6` | `sqlite3_value_int64` | library |
| 0.59% | `python` | `unicode_decode_utf8` | str |
| 0.55% | `libc-2.31.so` | `pthread_mutex_lock` | libc |
| 0.54% | `libsqlite3.so.0.8.6` | `sqlite3_enable_shared_cache` | library |
| 0.52% | `python` | `object_new` | memory |

## sympy

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 33.78% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.19% | `python` | `tupledealloc` | memory |
| 2.03% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.99% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.20% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.16% | `python` | `type_new` | memory |
| 1.12% | `python` | `gc_collect_main` | gc |
| 1.08% | `python` | `deduce_unreachable` | unknown |
| 1.07% | `python` | `_Py_type_getattro` | lookup |
| 0.98% | `python` | `visit_decref` | gc |
| 0.98% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.97% | `python` | `_Py_dict_lookup` | lookup |
| 0.95% | `python` | `PyDict_SetItem` | dict |
| 0.86% | `python` | `PyDict_GetItemRef` | dict |
| 0.81% | `python` | `object_isinstance` | dynamic |
| 0.80% | `python` | `find_name_in_mro` | lookup |
| 0.78% | `python` | `PyObject_RichCompare` | dynamic |
| 0.76% | `python` | `PyObject_GetAttr` | dynamic |
| 0.75% | `python` | `_PyCode_New` | memory |
| 0.75% | `python` | `slot_tp_richcompare` | dynamic |
| 0.72% | `python` | `dict_dealloc` | memory |
| 0.69% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.67% | `python` | `visit_reachable` | gc |
| 0.67% | `python` | `method_get` | dynamic |
| 0.64% | `python` | `meth_dealloc` | memory |
| 0.62% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.61% | `python` | `list_dealloc` | memory |
| 0.55% | `python` | `_PyObject_GenericGetAttrWithDict` | dynamic |
| 0.55% | `python` | `setiter_iternext` | miscobj |
| 0.54% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.54% | `python` | `r_object` | import |
| 0.51% | `python` | `dictiter_iternextitem` | dict |

## telco

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 19.23% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.13% | `python` | `PyType_GetModuleByDef` | dynamic |
| 3.93% | `python` | `PyObject_GC_Del` | gc |
| 3.50% | `python` | `_PyObject_GC_New` | gc |
| 2.34% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `_mpd_qaddsub` | library |
| 2.04% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.93% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.83% | `python` | `tupledealloc` | memory |
| 1.83% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `_mpd_baseshiftr` | library |
| 1.71% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `nm_mpd_qmul` | library |
| 1.71% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `nm_mpd_qadd` | library |
| 1.63% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `convert_op` | library |
| 1.63% | `python` | `meth_dealloc` | memory |
| 1.63% | `python` | `PyTuple_New` | memory |
| 1.48% | `python` | `PyContextVar_Get` | unknown |
| 1.42% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `_mpd_qmul` | library |
| 1.26% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `mpd_qshiftr` | library |
| 1.23% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `mpd_qfinalize` | library |
| 1.12% | `python` | `method_get` | dynamic |
| 1.05% | `python` | `vgetargskeywords.constprop.0` | calls |
| 1.04% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_mpd_qquantize` | library |
| 1.02% | `python` | `_PyArg_UnpackKeywordsWithVararg` | calls |
| 0.87% | `python` | `type_new` | memory |
| 0.84% | `python` | `PyUnicode_New` | memory |
| 0.80% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `PyDecType_New` | library |
| 0.76% | `python` | `PyDict_GetItemRef` | dict |
| 0.75% | `python` | `method_vectorcall_VARARGS_KEYWORDS` | calls |
| 0.74% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_dealloc` | library |
| 0.73% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `mpd_qquantize` | library |
| 0.64% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_addstatus` | library |
| 0.62% | `python` | `_io_BytesIO_read` | unknown |
| 0.62% | `python` | `gc_collect_main` | gc |
| 0.61% | `python` | `as_ucs4` | unknown |
| 0.59% | `python` | `visit_decref` | gc |
| 0.58% | `python` | `vgetargs1_impl` | calls |
| 0.58% | `_struct.cpython-313-x86_64-linux-gnu.so` | `unpack` | library |
| 0.53% | `python` | `deduce_unreachable` | unknown |
| 0.53% | `python` | `unicode_dealloc` | memory |
| 0.50% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_str` | library |

## thrift

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.76% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.13% | `python` | `object_new` | memory |
| 2.12% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::encodeValue` | library |
| 2.06% | `python` | `subtype_dealloc` | memory |
| 1.96% | `python` | `slot_tp_init` | unknown |
| 1.95% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.95% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.85% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.79% | `python` | `PyDict_GetItemRef` | dict |
| 1.73% | `python` | `PyDict_SetItem` | dict |
| 1.69% | `python` | `insert_to_emptydict` | dict |
| 1.58% | `python` | `dict_dealloc` | memory |
| 1.41% | `python` | `_PyStack_UnpackDict` | unknown |
| 1.28% | `python` | `tupledealloc` | memory |
| 1.21% | `python` | `PyUnicode_FromFormatV` | str |
| 1.18% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.16% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.15% | `python` | `type_new` | memory |
| 1.08% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 1.05% | `python` | `PyObject_GC_Del` | gc |
| 1.02% | `python` | `unicode_decode_utf8` | str |
| 0.86% | `python` | `insertdict` | dict |
| 0.82% | `python` | `deduce_unreachable` | unknown |
| 0.80% | `python` | `gc_collect_main` | gc |
| 0.79% | `python` | `PyMem_Free` | memory |
| 0.75% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::decodeValue` | library |
| 0.71% | `python` | `unicode_dealloc` | memory |
| 0.71% | `python` | `list_dealloc` | memory |
| 0.69% | `python` | `_PySuper_Lookup` | dynamic |
| 0.68% | `python` | `visit_decref` | gc |
| 0.66% | `python` | `_Py_dict_lookup` | lookup |
| 0.66% | `python` | `_Py_type_getattro` | lookup |
| 0.63% | `python` | `PyObject_RichCompare` | dynamic |
| 0.58% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readStruct` | library |
| 0.57% | `python` | `PyLong_AsLong` | int |
| 0.56% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readBytes` | library |
| 0.55% | `python` | `dictresize` | dict |
| 0.54% | `python` | `PyObject_GetOptionalAttr` | dynamic |
| 0.54% | `python` | `PyTuple_Size` | tuple |
| 0.54% | `python` | `_PyObject_GenericGetAttrWithDict` | dynamic |
| 0.53% | `python` | `visit_reachable` | gc |
| 0.52% | `python` | `_PyCode_New` | memory |
| 0.51% | `python` | `PyObject_GetAttr` | dynamic |

## tomli_loads

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 54.26% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.98% | `python` | `_PyLong_Add` | int |
| 5.18% | `python` | `set_contains_lock_held` | miscobj |
| 4.24% | `python` | `long_dealloc` | memory |
| 2.51% | `python` | `_PyUnicode_Equal` | str |
| 2.11% | `python` | `PyDict_GetItemRef` | dict |
| 2.01% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.82% | `python` | `PyDict_Contains` | dict |
| 1.60% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.99% | `python` | `_PyIncrementalNewlineDecoder_decode.cold` | memory |
| 0.90% | `python` | `tupledealloc` | memory |
| 0.79% | `python` | `object_isinstance` | dynamic |
| 0.53% | `python` | `PyUnicode_New` | memory |
| 0.53% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.50% | `python` | `sre_ucs4_match` | library |

## tornado_http

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 30.08% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.93% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.91% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.76% | `python` | `type_new` | memory |
| 1.39% | `python` | `deduce_unreachable` | unknown |
| 1.26% | `python` | `tupledealloc` | memory |
| 1.25% | `python` | `gc_collect_main` | gc |
| 1.16% | `python` | `visit_decref` | gc |
| 0.95% | `python` | `visit_reachable` | gc |
| 0.75% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.75% | `python` | `_PyCode_New` | memory |
| 0.75% | `python` | `PyDict_GetItemRef` | dict |
| 0.69% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.68% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 0.61% | `python` | `find_name_in_mro` | lookup |
| 0.60% | `python` | `r_object` | import |
| 0.57% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.54% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.51% | `python` | `subtype_dealloc` | memory |

## typing_runtime_protocols

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 36.29% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.26% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 2.82% | `python` | `_Py_dict_lookup` | lookup |
| 2.63% | `python` | `tupledealloc` | memory |
| 1.97% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.95% | `python` | `_Py_type_getattro` | lookup |
| 1.48% | `python` | `PyObject_GC_Del` | gc |
| 1.41% | `python` | `PyDict_Contains` | dict |
| 1.24% | `python` | `tuplehash` | tuple |
| 1.19% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.18% | `python` | `type_new` | memory |
| 1.17% | `python` | `PyTraceBack_Here` | exceptions |
| 1.10% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.98% | `python` | `frame_dealloc` | memory |
| 0.96% | `python` | `_PyObject_GC_New` | gc |
| 0.92% | `python` | `bounded_lru_cache_wrapper` | unknown |
| 0.88% | `python` | `_PyFrame_MakeAndSetFrameObject` | unknown |
| 0.88% | `python` | `getset_get` | dynamic |
| 0.84% | `python` | `PyObject_Vectorcall` | dynamic |
| 0.81% | `python` | `PySet_Contains` | unknown |
| 0.81% | `python` | `tuple_iter` | tuple |
| 0.76% | `python` | `gc_collect_main` | gc |
| 0.71% | `python` | `deduce_unreachable` | unknown |
| 0.69% | `python` | `tuplecontains` | tuple |
| 0.68% | `python` | `visit_decref` | gc |
| 0.68% | `python` | `tb_dealloc` | memory |
| 0.66% | `python` | `method_dealloc` | memory |
| 0.62% | `python` | `wrap_descr_get` | unknown |
| 0.61% | `python` | `_PyDict_GetItem_KnownHash` | dict |
| 0.59% | `python` | `PyArg_UnpackTuple` | calls |
| 0.56% | `python` | `PyObject_RichCompare` | dynamic |
| 0.53% | `python` | `_PyCode_New` | memory |
| 0.53% | `python` | `_Py_type_getattro_impl` | dynamic |

## unpack_sequence

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 76.09% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 1.03% | `python` | `type_new` | memory |
| 0.77% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.70% | `python` | `gc_collect_main` | gc |
| 0.66% | `python` | `visit_decref` | gc |
| 0.61% | `python` | `deduce_unreachable` | unknown |

## unpickle

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 13.03% | `python` | `unicode_decode_utf8` | str |
| 9.30% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `load` | library |
| 8.32% | `python` | `insertdict` | dict |
| 5.80% | `python` | `siphash13` | str |
| 5.59% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.49% | `python` | `unicode_dealloc` | memory |
| 5.15% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `load_counted_binunicode` | library |
| 2.75% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.58% | `python` | `dictresize` | dict |
| 2.08% | `python` | `dict_ass_sub` | dict |
| 1.82% | `python` | `PyMem_Realloc` | memory |
| 1.51% | `python` | `dict_dealloc` | memory |
| 1.43% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Unpickler_dealloc` | library |
| 1.34% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pdata_clear` | library |
| 1.30% | `python` | `PyObject_SetItem` | dynamic |
| 1.02% | `python` | `list_dealloc` | memory |
| 0.85% | `python` | `type_new` | memory |
| 0.84% | `python` | `long_dealloc` | memory |
| 0.83% | `python` | `PyLong_FromLong` | int |
| 0.77% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pdata_push` | library |
| 0.76% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `do_setitems.isra.0` | library |
| 0.65% | `python` | `unicode_hash` | str |
| 0.61% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.59% | `python` | `PyMem_Free` | memory |
| 0.58% | `python` | `_PyObject_GC_New` | gc |
| 0.57% | `python` | `gc_collect_main` | gc |
| 0.55% | `python` | `visit_decref` | gc |
| 0.55% | `python` | `deduce_unreachable` | unknown |

## unpickle_list

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 16.17% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `load` | library |
| 13.63% | `python` | `list_dealloc` | memory |
| 7.81% | `python` | `PyList_New` | memory |
| 6.93% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.29% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pdata_push` | library |
| 5.24% | `python` | `PyList_SetSlice` | list |
| 4.97% | `python` | `PyLong_FromLong` | int |
| 3.55% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `do_append.isra.0` | library |
| 3.04% | `python` | `_PyObject_Malloc` | memory |
| 1.88% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.44% | `python` | `list_resize` | list |
| 1.15% | `python` | `type_new` | memory |
| 0.99% | `python` | `PyMem_Realloc` | memory |
| 0.81% | `python` | `gc_collect_main` | gc |
| 0.76% | `python` | `visit_decref` | gc |
| 0.71% | `python` | `deduce_unreachable` | unknown |
| 0.66% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005ba4` | library |
| 0.55% | `python` | `_PyObject_GC_New` | gc |
| 0.51% | `python` | `visit_reachable` | gc |
| 0.50% | `python` | `_PyCode_New` | memory |

## unpickle_pure_python

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 55.08% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.21% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.17% | `python` | `PyObject_IsTrue` | dynamic |
| 1.85% | `python` | `_io_BytesIO_read` | unknown |
| 1.78% | `python` | `PyDict_GetItemRef` | dict |
| 1.70% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.23% | `python` | `type_new` | memory |
| 1.06% | `python` | `insertdict` | dict |
| 0.99% | `python` | `unicode_decode_utf8` | str |
| 0.95% | `python` | `tupledealloc` | memory |
| 0.79% | `python` | `gc_collect_main` | gc |
| 0.74% | `python` | `visit_decref` | gc |
| 0.73% | `python` | `deduce_unreachable` | unknown |
| 0.73% | `python` | `bytes_subscript` | str |
| 0.71% | `python` | `unicode_new` | memory |
| 0.60% | `python` | `PyObject_Free` | dynamic |
| 0.60% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.57% | `python` | `_PyCode_New` | memory |
| 0.56% | `python` | `siphash13` | str |
| 0.53% | `python` | `PyObject_GetItem` | dynamic |
| 0.52% | `python` | `visit_reachable` | gc |

## xml_etree

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.02% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.14% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 2.72% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `doContent` | library |
| 2.20% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `PyExpat_XML_Parse` | library |
| 1.90% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `normal_contentTok` | library |
| 1.87% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.81% | `python` | `_io_TextIOWrapper_write` | unknown |
| 1.79% | `python` | `unicode_decode_utf8` | str |
| 1.72% | `python` | `deduce_unreachable` | unknown |
| 1.66% | `python` | `visit_decref` | gc |
| 1.61% | `python` | `visit_reachable` | gc |
| 1.58% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `hash` | library |
| 1.53% | `python` | `unicode_dealloc` | memory |
| 1.50% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `storeAtts` | library |
| 1.39% | `python` | `gc_collect_main` | gc |
| 1.37% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `makeuniversal.isra.0` | library |
| 1.34% | `python` | `PyUnicode_Concat` | str |
| 1.33% | `python` | `PyObject_GC_Del` | gc |
| 1.32% | `python` | `_PyObject_GC_New` | gc |
| 1.29% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.28% | `python` | `object_isinstance` | dynamic |
| 1.18% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 1.08% | `python` | `tupledealloc` | memory |
| 0.88% | `python` | `list_dealloc` | memory |
| 0.87% | `python` | `PyBytes_FromStringAndSize` | str |
| 0.86% | `python` | `long_to_decimal_string_internal` | int |
| 0.85% | `python` | `PyObject_GetAttr` | dynamic |
| 0.83% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `elementiter_next` | library |
| 0.82% | `python` | `PyUnicode_Format` | str |
| 0.81% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `element_gc_traverse` | library |
| 0.80% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.79% | `python` | `getset_get` | dynamic |
| 0.71% | `python` | `PyUnicode_Contains` | str |
| 0.69% | `python` | `PyDict_GetItemWithError` | dict |
| 0.67% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `element_dealloc` | library |
| 0.65% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `treebuilder_handle_start` | library |
| 0.63% | `python` | `siphash13` | str |
| 0.60% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.59% | `python` | `type_new` | memory |
| 0.56% | `python` | `vgetargs1_impl` | calls |
| 0.55% | `python` | `list_vectorcall` | list |
| 0.54% | `python` | `PyObject_Free` | dynamic |
| 0.52% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.50% | `python` | `PyDict_GetItemRef` | dict |


## Categories

### interpreter

35.08% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 32.60% | python | _PyEval_EvalFrameDefault |
| 1.59% | python | _PyEval_FrameClearAndPop |
| 0.34% | python | _PyEvalFramePushAndInit |
| 0.14% | python | _PyEval_EvalFrameDefault.cold |
| 0.10% | python | PyEval_RestoreThread |
| 0.08% | python | _PyPegen_fill_token |
| 0.07% | python | _PyFrame_ClearExceptCode |
| 0.03% | python | intern_string_constants |
| 0.03% | python | PyEval_SaveThread |
| 0.02% | python | _PyPegen_update_memo |
| 0.02% | python | _PyCode_Validate |
| 0.01% | python | _PyPegen_name_token |
| 0.01% | python | _PyPegen_Parser_Free |
| 0.01% | python | PyEval_GetFrame |

### library

9.90% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 1.56% | python | sre_ucs1_match |
| 1.30% | _pickle.cpython-313-x86_64-linux-gnu.so | save |
| 0.75% | libz.so.1.2.11 | crc32_combine64 |
| 0.71% | python | sre_ucs2_charset.isra.0 |
| 0.45% | _json.cpython-313-x86_64-linux-gnu.so | _parse_object_unicode |
| 0.30% | _pickle.cpython-313-x86_64-linux-gnu.so | load |
| 0.28% | _pickle.cpython-313-x86_64-linux-gnu.so | _Pickler_Write |
| 0.28% | libz.so.1.2.11 | inflateBackEnd |
| 0.24% | _pickle.cpython-313-x86_64-linux-gnu.so | memo_put.isra.0 |
| 0.19% | libpthread-2.31.so | __pthread_mutex_lock |
| 0.19% | python | sre_search |
| 0.18% | libpthread-2.31.so | pthread_mutex_unlock |
| 0.14% | python | sre_ucs1_count |
| 0.12% | ld-2.31.so | _dl_rtld_di_serinfo |
| 0.12% | python | _sre_SRE_Pattern_match |
| 0.11% | libm-2.31.so | f64xsubf128 |
| 0.10% | _json.cpython-313-x86_64-linux-gnu.so | encoder_encode_key_value |
| 0.09% | tracer.cpython-313-x86_64-linux-gnu.so | CTracer_trace |
| 0.08% | _pickle.cpython-313-x86_64-linux-gnu.so | Pdata_push |
| 0.08% | _pickle.cpython-313-x86_64-linux-gnu.so | _Pickler_write_bytes |
| 0.07% | libpython3.11.so.1.0 | _PyEval_EvalFrameDefault |
| 0.06% | _pickle.cpython-313-x86_64-linux-gnu.so | load_counted_binunicode |
| 0.06% | _asyncio.cpython-313-x86_64-linux-gnu.so | TaskObj_traverse |
| 0.05% | libsqlite3.so.0.8.6 | sqlite3_reset |
| 0.05% | _pickle.cpython-313-x86_64-linux-gnu.so | Pickler_dealloc |
| 0.05% | libmagic.so.1.0.0 | 0x000000000000f936 |
| 0.04% | _pickle.cpython-313-x86_64-linux-gnu.so | do_append.isra.0 |
| 0.04% | libm-2.31.so | __fmod_finite |
| 0.04% | libz.so.1.2.11 | inflateCodesUsed |
| 0.04% | ld-2.31.so | _dl_catch_error |
| 0.03% | _json.cpython-313-x86_64-linux-gnu.so | py_encode_basestring_ascii |
| 0.03% | pyexpat.cpython-313-x86_64-linux-gnu.so | doContent |
| 0.03% | python | pattern_subx |
| 0.03% | _pickle.cpython-313-x86_64-linux-gnu.so | memo_get.isra.0 |
| 0.03% | _json.cpython-313-x86_64-linux-gnu.so | _match_number_unicode.isra.0 |
| 0.03% | libmagic.so.1.0.0 | 0x000000000000f932 |
| 0.03% | array.cpython-313-x86_64-linux-gnu.so | array_subscr |
| 0.03% | _decimal.cpython-313-x86_64-linux-gnu.so | _mpd_qaddsub |
| 0.03% | pyexpat.cpython-313-x86_64-linux-gnu.so | PyExpat_XML_Parse |
| 0.02% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::encodeValue |
| 0.02% | _pickle.cpython-313-x86_64-linux-gnu.so | Unpickler_dealloc |
| 0.02% | pyexpat.cpython-313-x86_64-linux-gnu.so | normal_contentTok |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | _mpd_baseshiftr |
| 0.02% | libpthread-2.31.so | pthread_cond_signal@@GLIBC_2.3.2 |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | nm_mpd_qmul |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | nm_mpd_qadd |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | convert_op |
| 0.02% | pyexpat.cpython-313-x86_64-linux-gnu.so | hash |
| 0.02% | _asyncio.cpython-313-x86_64-linux-gnu.so | task_step_impl |
| 0.02% | libz.so.1.2.11 | inflate |
| 0.02% | pyexpat.cpython-313-x86_64-linux-gnu.so | storeAtts |
| 0.02% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005cd4 |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | _mpd_qmul |
| 0.02% | libsqlite3.so.0.8.6 | sqlite3_randomness |
| 0.02% | _elementtree.cpython-313-x86_64-linux-gnu.so | makeuniversal.isra.0 |
| 0.02% | libpython3.11.so.1.0 | _PyDict_GetItem_KnownHash |
| 0.02% | _pickle.cpython-313-x86_64-linux-gnu.so | Pdata_clear |
| 0.02% | _asyncio.cpython-313-x86_64-linux-gnu.so | TaskStepMethWrapper_traverse |
| 0.02% | _heapq.cpython-313-x86_64-linux-gnu.so | _heapq_heappop |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | mpd_qshiftr |
| 0.01% | array.cpython-313-x86_64-linux-gnu.so | array_ass_subscr |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | mpd_qfinalize |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | factorial_partial_product |
| 0.01% | _json.cpython-313-x86_64-linux-gnu.so | _parse_array_unicode |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | TaskObj_clear |
| 0.01% | _bisect.cpython-313-x86_64-linux-gnu.so | _bisect_bisect_right |
| 0.01% | python | sre_ucs1_match.cold |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_exec |
| 0.01% | libpython3.11.so.1.0 | PyObject_Malloc |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_mpd_qquantize |
| 0.01% | _sqlite3.cpython-313-x86_64-linux-gnu.so | _pysqlite_query_execute |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | FutureObj_traverse |
| 0.01% | libpthread-2.31.so | sem_post@@GLIBC_2.2.5 |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | element_gc_traverse |
| 0.01% | libpython3.11.so.1.0 | deduce_unreachable |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_value_double |
| 0.01% | libpython3.11.so.1.0 | visit_decref |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | _pickle_dumps |
| 0.01% | libssl.so.1.1 | SSL_rstate_string |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005e54 |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | _asyncio_Future_add_done_callback |
| 0.01% | array.cpython-313-x86_64-linux-gnu.so | d_setitem |
| 0.01% | libpython3.11.so.1.0 | PyDict_SetDefault |
| 0.01% | libpthread-2.31.so | sem_trywait@@GLIBC_2.2.5 |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | elementiter_next |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | PyDecType_New |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | _pickle_loads |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | math_factorial |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | math_sqrt |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_str_value |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | future_init |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | do_setitems.isra.0 |
| 0.01% | libpython3.11.so.1.0 | type_new |
| 0.01% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::decodeValue |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005fc4 |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_dealloc |
| 0.01% | _struct.cpython-313-x86_64-linux-gnu.so | unpack |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | element_dealloc |
| 0.01% | libpython3.11.so.1.0 | r_object |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | _asyncio_Task___init__ |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | mpd_qquantize |
| 0.01% | libpython3.11.so.1.0 | visit_reachable |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_preupdate_old |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005ba4 |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_wal_checkpoint |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_extended_errcode |
| 0.01% | _struct.cpython-313-x86_64-linux-gnu.so | s_pack |
| 0.01% | libpython3.11.so.1.0 | gc_collect_main |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | treebuilder_handle_start |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_addstatus |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_vtab_config |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_value_int64 |
| 0.01% | libpython3.11.so.1.0 | PyObject_Free |
| 0.01% | python | _sre_SRE_Pattern_search |
| 0.01% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readStruct |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_enable_shared_cache |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | task_step |
| 0.01% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readBytes |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | call_soon |
| 0.01% | _json.cpython-313-x86_64-linux-gnu.so | encoder_listencode_obj |
| 0.01% | libz.so.1.2.11 | adler32_combine64 |
| 0.01% | python | sre_ucs4_match |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_str |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | math_cos |

### memory

9.47% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.99% | python | type_new |
| 0.79% | python | tupledealloc |
| 0.74% | python | list_dealloc |
| 0.64% | python | long_dealloc |
| 0.54% | python | unicode_dealloc |
| 0.44% | python | _PyCode_New |
| 0.34% | python | dict_dealloc |
| 0.33% | python | subtype_dealloc |
| 0.32% | python | gen_dealloc |
| 0.25% | python | PyList_New |
| 0.24% | python | PyMem_Free |
| 0.23% | python | meth_dealloc |
| 0.21% | python | _PyLong_New |
| 0.21% | python | _PyObject_Malloc |
| 0.20% | python | object_new |
| 0.19% | python | PyFunction_NewWithQualName |
| 0.16% | python | PyUnicode_New |
| 0.16% | python | PyMem_Malloc |
| 0.15% | python | PyType_GenericAlloc |
| 0.14% | python | func_dealloc |
| 0.13% | python | method_dealloc |
| 0.12% | python | code_dealloc |
| 0.11% | python | set_dealloc |
| 0.11% | python | frame_dealloc |
| 0.11% | python | BaseException_new |
| 0.11% | python | PyTuple_New |
| 0.10% | python | float_dealloc |
| 0.10% | python | PyMem_Realloc |
| 0.07% | python | slice_dealloc |
| 0.06% | python | StopIteration_dealloc |
| 0.05% | python | allocate_from_new_pool |
| 0.05% | python | _Py_Dealloc |
| 0.05% | python | listiter_dealloc |
| 0.05% | python | list_new_prealloc |
| 0.04% | python | dictiter_dealloc |
| 0.04% | python | PyType_GenericNew |
| 0.04% | python | tb_dealloc |
| 0.04% | python | BaseException_dealloc |
| 0.04% | python | PySlice_New |
| 0.04% | python | make_new_set |
| 0.03% | python | tp_new_wrapper |
| 0.03% | python | cell_dealloc |
| 0.03% | python | slot_tp_new |
| 0.03% | python | _PyObject_Free |
| 0.03% | python | context_tp_dealloc |
| 0.03% | python | dictview_dealloc |
| 0.03% | python | range_dealloc |
| 0.03% | python | weakref_dealloc |
| 0.02% | python | match_dealloc |
| 0.02% | python | _PyObject_New |
| 0.02% | python | tupleiter_dealloc |
| 0.02% | python | _PyAsyncGenValueWrapperNew |
| 0.02% | python | async_gen_asend_dealloc |
| 0.02% | python | weakref___new__ |
| 0.02% | python | _PyIncrementalNewlineDecoder_decode.cold |
| 0.02% | python | async_gen_asend_new |
| 0.02% | python | _PyFloat_ExactDealloc |
| 0.02% | python | _Py_NewReference |
| 0.02% | python | async_gen_wrapped_val_dealloc |
| 0.01% | python | object_dealloc |
| 0.01% | python | unicode_new |
| 0.01% | python | PyDict_New |
| 0.01% | python | PyCMethod_New |
| 0.01% | python | PyObject_CallFinalizerFromDealloc |
| 0.01% | python | structseq_dealloc |
| 0.01% | python | PyWeakref_NewRef |
| 0.01% | python | _PyIncrementalNewlineDecoder_decode |
| 0.01% | python | AttributeError_dealloc |
| 0.01% | python | _PyTokenizer_translate_newlines.constprop.0 |
| 0.01% | python | descr_dealloc |
| 0.01% | python | pattern_new_match.isra.0 |
| 0.01% | python | _PyMem_RawMalloc |
| 0.01% | python | reversed_new_impl |
| 0.01% | python | zip_new |
| 0.01% | python | PyDictProxy_New |
| 0.01% | python | _PyObject_Realloc |

### gc

8.52% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 2.80% | python | gc_collect_main |
| 1.75% | python | visit_decref |
| 1.64% | python | visit_reachable |
| 0.43% | python | PyObject_GC_Del |
| 0.41% | python | subtype_traverse |
| 0.27% | python | dict_traverse |
| 0.27% | python | _PyObject_GC_New |
| 0.24% | python | list_traverse |
| 0.13% | python | set_traverse |
| 0.10% | python | _PyObject_GC_NewVar |
| 0.10% | python | func_traverse |
| 0.10% | python | gen_traverse |
| 0.05% | python | type_traverse |
| 0.03% | python | meth_traverse |
| 0.03% | python | PyObject_GC_UnTrack |
| 0.02% | python | gc_traverse |
| 0.02% | python | PyObject_GC_Track |
| 0.02% | python | context_tp_traverse |
| 0.01% | python | frame_traverse |
| 0.01% | python | descr_traverse |
| 0.01% | python | module_traverse |
| 0.01% | python | executor_traverse |
| 0.01% | python | method_traverse |
| 0.01% | python | PyObject_IS_GC |

### unknown

7.08% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 1.89% | python | deduce_unreachable |
| 0.25% | python | make_gen |
| 0.20% | python | slot_tp_init |
| 0.18% | python | _Py_hashtable_get |
| 0.14% | python | uop_optimize |
| 0.10% | python | _PyBuildSlice_Consume2 |
| 0.09% | python | clear_slots |
| 0.09% | python | func_descr_get |
| 0.08% | python | _PyFrame_MakeAndSetFrameObject |
| 0.08% | python | _PyStack_UnpackDict |
| 0.08% | python | method_vectorcall |
| 0.06% | python | slot_mp_subscript |
| 0.06% | python | _PyFrame_PushUnchecked.isra.0 |
| 0.06% | python | memset@plt |
| 0.06% | python | memcpy@plt |
| 0.06% | python | call_instrumentation_vector |
| 0.05% | python | make_executor_from_uops |
| 0.05% | python | gen_iternext |
| 0.05% | python | convert_to_double |
| 0.05% | python | range_vectorcall |
| 0.05% | python | _stringio_readline.cold |
| 0.04% | python | as_ucs4 |
| 0.04% | python | builtin_min |
| 0.04% | python | builtin_hasattr |
| 0.04% | python | range_iter |
| 0.04% | python | path_converter |
| 0.04% | python | _PyCfg_OptimizeCodeUnit.constprop.0 |
| 0.04% | python | dictkeys_decref.part.0 |
| 0.04% | python | optimize_uops.constprop.0 |
| 0.04% | python | slot_tp_hash |
| 0.03% | python | _Py_module_getattro |
| 0.03% | python | PySet_Add |
| 0.03% | python | gen_send_ex2 |
| 0.03% | python | member_get |
| 0.03% | [vdso] | __vdso_clock_gettime |
| 0.03% | python | PySys_Audit |
| 0.03% | python | ucs4lib_find_max_char |
| 0.03% | python | _io_BytesIO_read |
| 0.03% | python | vectorcall_maybe.constprop.0 |
| 0.03% | python | state_init |
| 0.03% | python | call_one_instrument |
| 0.03% | python | async_gen_asend_send |
| 0.03% | python | dictitems_iter |
| 0.03% | python | gen_send_ex |
| 0.03% | python | _Py_VaBuildStack.constprop.0 |
| 0.02% | python | _PyAssemble_MakeCodeObject |
| 0.02% | python | term_raw |
| 0.02% | python | slot_mp_ass_subscript |
| 0.02% | python | cm_descr_get |
| 0.02% | python | hashtable_unicode_hash |
| 0.02% | python | range_subscript |
| 0.02% | python | vgetargs1_impl.cold |
| 0.02% | python | _io_TextIOWrapper_write |
| 0.02% | python | builtin_id |
| 0.02% | python | code_hash |
| 0.02% | python | _PyOptimizer_Optimize |
| 0.02% | python | bitwise_xor_rule |
| 0.02% | python | bounded_lru_cache_wrapper |
| 0.02% | python | _PyCoro_GetAwaitableIter |
| 0.02% | python | hashtable_unicode_compare |
| 0.02% | python | builtin___import__ |
| 0.02% | python | Py_XDECREF.lto_priv.1 |
| 0.02% | python | binary_op1 |
| 0.02% | python | PyContextVar_Get |
| 0.02% | python | _PyModule_ClearDict |
| 0.02% | python | convertitem |
| 0.02% | python | binary_op |
| 0.02% | python | _PyCfg_OptimizedCfgToInstructionSequence |
| 0.02% | python | member_set |
| 0.02% | python | _Py_slot_tp_getattr_hook |
| 0.02% | python | _Py_module_getattro_impl.part.0 |
| 0.02% | python | do_mktuple |
| 0.02% | python | classmethod_get |
| 0.02% | python | wrapperdescr_call |
| 0.02% | python | write_bytes |
| 0.02% | python | unsafe_tuple_compare |
| 0.02% | python | PySet_Contains |
| 0.01% | python | make_range_object |
| 0.01% | python | _PyDictKeys_StringLookup |
| 0.01% | python | shift_expr_rule |
| 0.01% | python | build_indices_generic |
| 0.01% | python | ScandirIterator_iternext |
| 0.01% | python | builtin_sum |
| 0.01% | python | sum_rule |
| 0.01% | python | async_gen_unwrap_value.isra.0 |
| 0.01% | python | memcmp@plt |
| 0.01% | python | Py_XDECREF.lto_priv.6 |
| 0.01% | python | _PyThreadState_GetCurrent |
| 0.01% | python | _PyBytes_Resize |
| 0.01% | python | os_listdir |
| 0.01% | python | slot_sq_contains |
| 0.01% | python | builtin_issubclass |
| 0.01% | python | va_build_value |
| 0.01% | python | _PyGen_FetchStopIterationValue.cold |
| 0.01% | python | expression_rule |
| 0.01% | python | call_trace_func.isra.0 |
| 0.01% | python | _Py_bytes_lower |
| 0.01% | python | atom_rule |
| 0.01% | python | primary_raw |
| 0.01% | python | get_type_attr_as_size |
| 0.01% | python | context_run |
| 0.01% | python | symtable_add_def_helper |
| 0.01% | python | _add_methods_to_object |
| 0.01% | python | PyIndex_Check |
| 0.01% | python | _PyCode_GetCode |
| 0.01% | python | _io_open |
| 0.01% | python | mro_implementation_unlocked |
| 0.01% | python | lookup_maybe_method |
| 0.01% | python | inversion_rule |
| 0.01% | python | _PyGen_SetStopIterationValue |
| 0.01% | python | _PyType_FromMetaclass_impl |
| 0.01% | python | ins1 |
| 0.01% | python | PyTime_AsSecondsDouble |
| 0.01% | python | zip_next |
| 0.01% | python | slot_sq_item |
| 0.01% | python | binary_iop1 |
| 0.01% | python | _Py_call_instrumentation_jump |
| 0.01% | python | lru_cache_make_key |
| 0.01% | python | builtin_hash |
| 0.01% | python | PyThread_acquire_lock_timed |
| 0.01% | python | _PyContext_Exit |
| 0.01% | python | assign_version_tag |
| 0.01% | python | instr_sequence_to_cfg |
| 0.01% | python | map_next |
| 0.01% | python | ascii_upper_or_lower |
| 0.01% | python | clear_weakref |
| 0.01% | python | fill_time |
| 0.01% | python | builtin_max |
| 0.01% | python | weakref_richcompare |
| 0.01% | python | update_slots_callback |
| 0.01% | python | sm_descr_get |
| 0.01% | python | compiler_nameop |
| 0.01% | python | astfold_expr |
| 0.01% | python | pthread_self@plt |
| 0.01% | python | frozenset_vectorcall |
| 0.01% | python | _PyGen_yf |
| 0.01% | python | map_vectorcall |
| 0.01% | python | new_dict |
| 0.01% | python | weakref_hash |
| 0.01% | python | symtable_visit_expr |
| 0.01% | python | update_slot |
| 0.01% | python | analyze_block |
| 0.01% | python | builtin_any |
| 0.01% | python | _getbytevalue |
| 0.01% | python | pytime_divide |
| 0.01% | python | unsafe_latin_compare |
| 0.01% | python | wrap_descr_get |
| 0.01% | python | make_dict_from_instance_attributes |
| 0.01% | python | _PyLexer_update_fstring_expr |
| 0.01% | python | compiler_visit_expr1 |
| 0.01% | python | wrapper_call |
| 0.01% | python | 0x000000000007e720 |
| 0.01% | python | islice_next |
| 0.01% | python | _io_FileIO___init__ |
| 0.01% | python | super_getattro |
| 0.01% | python | bitwise_or_rule |
| 0.01% | python | slot_tp_iter |
| 0.01% | python | _Py_Executors_InvalidateDependency |
| 0.01% | python | pthread_mutex_unlock@plt |
| 0.01% | python | _abc__abc_instancecheck |
| 0.01% | python | _Py_dg_dtoa |
| 0.01% | python | subtype_clear |
| 0.01% | python | stringio_iternext |
| 0.01% | python | simple_stmt_rule |

### dynamic

5.62% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.54% | python | PyObject_GenericGetAttr |
| 0.35% | python | _PyObject_GetMethod |
| 0.34% | python | object_isinstance |
| 0.30% | python | _PyObject_MakeTpCall |
| 0.25% | python | PyObject_GetAttr |
| 0.23% | python | PyObject_Free |
| 0.19% | python | PyObject_SetAttr |
| 0.18% | python | PyObject_Str |
| 0.17% | python | method_get |
| 0.16% | python | _PySuper_Lookup |
| 0.15% | python | PyObject_Vectorcall |
| 0.15% | python | PyObject_RichCompare |
| 0.13% | python | PyType_GetModuleByDef |
| 0.13% | python | PyObject_VectorcallMethod |
| 0.13% | python | PyObject_IsTrue |
| 0.12% | python | type_ready |
| 0.12% | python | PyObject_GetItem |
| 0.11% | python | _PyObject_LookupSpecial |
| 0.11% | python | PyNumber_AsSsize_t |
| 0.09% | python | getset_get |
| 0.08% | python | PyObject_GetIter |
| 0.07% | python | PyObject_IsInstance |
| 0.07% | python | type_call |
| 0.07% | python | PyObject_GetOptionalAttr |
| 0.07% | python | PyObject_Hash |
| 0.07% | python | _PyObject_GenericGetAttrWithDict |
| 0.06% | python | _Py_type_getattro_impl |
| 0.06% | python | slot_tp_richcompare |
| 0.05% | python | PyObject_SetItem |
| 0.05% | python | _PyObject_Call |
| 0.05% | python | _PyObject_ClearFreeLists |
| 0.05% | python | PyObject_SetAttrString |
| 0.05% | python | PyMapping_GetOptionalItem |
| 0.05% | python | PyObject_CallOneArg |
| 0.04% | python | PyNumber_Multiply |
| 0.04% | python | _PyObject_InitInlineValues |
| 0.04% | python | PyNumber_And |
| 0.04% | python | PyNumber_Add |
| 0.03% | python | _PyObject_VectorcallTstate.lto_priv.5 |
| 0.03% | python | PyType_IsSubtype |
| 0.03% | python | PyNumber_TrueDivide |
| 0.03% | python | StopIteration_init |
| 0.03% | python | PyIter_Send |
| 0.03% | python | PyNumber_Subtract |
| 0.02% | python | PyObject_VisitManagedDict |
| 0.02% | python | PyObject_RichCompareBool |
| 0.02% | python | PyNumber_Remainder |
| 0.02% | python | PySequence_Tuple |
| 0.02% | python | PySequence_List |
| 0.02% | python | PyObject_LengthHint |
| 0.01% | python | object_get_class |
| 0.01% | python | delitem_common |
| 0.01% | python | PyObject_CallFunction |
| 0.01% | python | object_richcompare |
| 0.01% | python | PyObject_ClearManagedDict |
| 0.01% | python | PyNumber_Rshift |
| 0.01% | python | PyObject_ClearWeakRefs |
| 0.01% | python | PyNumber_FloorDivide |
| 0.01% | python | PyNumber_InPlaceAdd |
| 0.01% | python | object_vacall |
| 0.01% | python | PyNumber_Negative |
| 0.01% | python | _PyNumber_Index |
| 0.01% | python | PyIter_Next |
| 0.01% | python | object_recursive_isinstance.part.0 |
| 0.01% | python | object_init |
| 0.01% | python | object_hash |
| 0.01% | python | _PyObject_GenericSetAttrWithDict |
| 0.01% | python | type_dealloc_common |
| 0.01% | python | PyObject_GetBuffer |
| 0.01% | python | PyObject_CallMethodObjArgs |
| 0.01% | python | PyNumber_Index |
| 0.01% | python | PyObject_SelfIter |
| 0.01% | python | PyObject_DelItem |
| 0.01% | python | PyNumber_Lshift |
| 0.01% | python | _PyNumber_PowerNoMod |

### kernel

4.46% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.63% | [kernel.kallsyms] | copy_user_enhanced_fast_string |
| 0.25% | [kernel.kallsyms] | clear_page_erms |
| 0.12% | [kernel.kallsyms] | native_irq_return_iret |
| 0.09% | [kernel.kallsyms] | __d_lookup_rcu |
| 0.09% | [kernel.kallsyms] | sync_regs |
| 0.08% | [kernel.kallsyms] | rmqueue |
| 0.08% | [kernel.kallsyms] | _raw_spin_lock |
| 0.07% | [kernel.kallsyms] | zap_pte_range.isra.0 |
| 0.05% | [kernel.kallsyms] | memset_erms |
| 0.05% | [kernel.kallsyms] | free_pcppages_bulk |
| 0.05% | [kernel.kallsyms] | __handle_mm_fault |
| 0.05% | [kernel.kallsyms] | filemap_map_pages |
| 0.04% | [kernel.kallsyms] | smp_call_function_single |
| 0.04% | [kernel.kallsyms] | link_path_walk.part.0 |
| 0.04% | [kernel.kallsyms] | try_charge |
| 0.04% | [kernel.kallsyms] | release_pages |
| 0.03% | [kernel.kallsyms] | get_mem_cgroup_from_mm |
| 0.03% | [kernel.kallsyms] | kmem_cache_alloc |
| 0.03% | [kernel.kallsyms] | __pagevec_lru_add_fn |
| 0.03% | [kernel.kallsyms] | syscall_return_via_sysret |
| 0.03% | [kernel.kallsyms] | ext4_htree_store_dirent |
| 0.03% | [kernel.kallsyms] | mem_cgroup_throttle_swaprate |
| 0.03% | [kernel.kallsyms] | __ext4fs_dirhash |
| 0.03% | [kernel.kallsyms] | handle_mm_fault |
| 0.03% | [kernel.kallsyms] | mem_cgroup_try_charge |
| 0.02% | [kernel.kallsyms] | page_remove_rmap |
| 0.02% | [kernel.kallsyms] | kmem_cache_free |
| 0.02% | [kernel.kallsyms] | __alloc_pages_nodemask |
| 0.02% | [kernel.kallsyms] | kfree |
| 0.02% | [kernel.kallsyms] | strncpy_from_user |
| 0.02% | [kernel.kallsyms] | __virt_addr_valid |
| 0.02% | [kernel.kallsyms] | filldir64 |
| 0.02% | [kernel.kallsyms] | find_get_entry |
| 0.02% | [kernel.kallsyms] | entry_SYSCALL_64 |
| 0.02% | [kernel.kallsyms] | copy_page |
| 0.02% | [kernel.kallsyms] | inode_permission |
| 0.02% | [kernel.kallsyms] | perf_event_alloc |
| 0.02% | [kernel.kallsyms] | lookup_fast |
| 0.02% | [kernel.kallsyms] | memcg_kmem_get_cache |
| 0.02% | [kernel.kallsyms] | find_vma |
| 0.02% | [kernel.kallsyms] | do_syscall_64 |
| 0.02% | [kernel.kallsyms] | do_user_addr_fault |
| 0.02% | [kernel.kallsyms] | generic_permission |
| 0.02% | [kernel.kallsyms] | _raw_spin_lock_irqsave |
| 0.02% | [kernel.kallsyms] | prep_new_page |
| 0.02% | [kernel.kallsyms] | get_page_from_freelist |
| 0.02% | [kernel.kallsyms] | do_anonymous_page |
| 0.02% | [kernel.kallsyms] | __slab_free |
| 0.02% | [kernel.kallsyms] | walk_component |
| 0.01% | [kernel.kallsyms] | rb_insert_color |
| 0.01% | [kernel.kallsyms] | __fget_light |
| 0.01% | [kernel.kallsyms] | __count_memcg_events |
| 0.01% | [kernel.kallsyms] | vmacache_find |
| 0.01% | [kernel.kallsyms] | str2hashbuf_signed |
| 0.01% | [kernel.kallsyms] | memcpy_erms |
| 0.01% | [kernel.kallsyms] | __mod_memcg_state |
| 0.01% | [kernel.kallsyms] | page_fault |
| 0.01% | [kernel.kallsyms] | ext4_getattr |
| 0.01% | [kernel.kallsyms] | mutex_lock |
| 0.01% | [kernel.kallsyms] | error_entry |
| 0.01% | [kernel.kallsyms] | rb_next |
| 0.01% | [kernel.kallsyms] | perf_iterate_ctx |
| 0.01% | [kernel.kallsyms] | __mod_lruvec_state |
| 0.01% | [kernel.kallsyms] | entry_SYSCALL_64_after_hwframe |
| 0.01% | [kernel.kallsyms] | psi_task_change |
| 0.01% | [kernel.kallsyms] | security_inode_getattr |
| 0.01% | [kernel.kallsyms] | _cond_resched |
| 0.01% | [kernel.kallsyms] | page_add_file_rmap |
| 0.01% | [kernel.kallsyms] | mutex_unlock |
| 0.01% | [kernel.kallsyms] | tcp_sendmsg_locked |
| 0.01% | [kernel.kallsyms] | vsnprintf |
| 0.01% | [kernel.kallsyms] | xas_load |
| 0.01% | [kernel.kallsyms] | generic_file_buffered_read |
| 0.01% | [kernel.kallsyms] | fsnotify |
| 0.01% | [kernel.kallsyms] | __kmalloc |
| 0.01% | [kernel.kallsyms] | __check_object_size |
| 0.01% | [kernel.kallsyms] | up_read |
| 0.01% | [kernel.kallsyms] | lru_cache_add_active_or_unevictable |
| 0.01% | [kernel.kallsyms] | down_read_trylock |
| 0.01% | [kernel.kallsyms] | show_cpuinfo |
| 0.01% | [kernel.kallsyms] | ___slab_alloc |
| 0.01% | [kernel.kallsyms] | page_counter_cancel |
| 0.01% | [kernel.kallsyms] | __lru_cache_add |
| 0.01% | [kernel.kallsyms] | __lock_text_start |
| 0.01% | [kernel.kallsyms] | free_unref_page_prepare.part.0 |
| 0.01% | [kernel.kallsyms] | native_flush_tlb_one_user |
| 0.01% | [kernel.kallsyms] | pagevec_lru_move_fn |
| 0.01% | [kernel.kallsyms] | alloc_set_pte |
| 0.01% | [kernel.kallsyms] | fpregs_assert_state_consistent |
| 0.01% | [kernel.kallsyms] | format_decode |
| 0.01% | [kernel.kallsyms] | inherit_event.isra.0 |
| 0.01% | [kernel.kallsyms] | __follow_mount_rcu.isra.0 |
| 0.01% | [kernel.kallsyms] | swapgs_restore_regs_and_return_to_usermode |
| 0.01% | [kernel.kallsyms] | __ext4_check_dir_entry |
| 0.01% | [kernel.kallsyms] | native_write_msr |
| 0.01% | [kernel.kallsyms] | __mod_node_page_state |
| 0.01% | [kernel.kallsyms] | set_root |
| 0.01% | [kernel.kallsyms] | in_group_p |
| 0.01% | [kernel.kallsyms] | unlock_page |
| 0.01% | [kernel.kallsyms] | free_pages_and_swap_cache |
| 0.01% | [kernel.kallsyms] | alloc_pages_vma |
| 0.01% | [kernel.kallsyms] | memcg_kmem_put_cache |
| 0.01% | [kernel.kallsyms] | rcu_all_qs |
| 0.01% | [kernel.kallsyms] | update_curr |
| 0.01% | [kernel.kallsyms] | free_unref_page_list |
| 0.01% | [kernel.kallsyms] | __legitimize_mnt |
| 0.01% | [kernel.kallsyms] | kmem_cache_alloc_trace |
| 0.01% | [kernel.kallsyms] | __vma_adjust |
| 0.01% | [kernel.kallsyms] | security_inode_permission |
| 0.01% | [kernel.kallsyms] | mem_cgroup_commit_charge |
| 0.01% | [kernel.kallsyms] | __mod_zone_page_state |
| 0.01% | [kernel.kallsyms] | update_cfs_group |
| 0.01% | [kernel.kallsyms] | mem_cgroup_from_task |
| 0.01% | [kernel.kallsyms] | __update_load_avg_se |
| 0.01% | [kernel.kallsyms] | __d_lookup |
| 0.01% | [kernel.kallsyms] | __free_pages_ok |
| 0.01% | [kernel.kallsyms] | __fput |
| 0.01% | [kernel.kallsyms] | free_unref_page_commit |
| 0.01% | [kernel.kallsyms] | xas_start |
| 0.01% | [kernel.kallsyms] | __tcp_transmit_skb |
| 0.01% | [kernel.kallsyms] | skb_release_data |
| 0.01% | [kernel.kallsyms] | memchr |
| 0.01% | [kernel.kallsyms] | update_load_avg |
| 0.01% | [kernel.kallsyms] | read_tsc |
| 0.01% | [kernel.kallsyms] | do_dentry_open |
| 0.01% | [kernel.kallsyms] | lockref_put_return |
| 0.01% | [kernel.kallsyms] | unmapped_area_topdown |
| 0.01% | [kernel.kallsyms] | call_filldir |
| 0.01% | [kernel.kallsyms] | exit_to_usermode_loop |

### libc

3.56% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 2.24% | libc-2.31.so | __nss_database_lookup |
| 0.48% | libc-2.31.so | pthread_attr_setschedparam |
| 0.30% | libcrypto.so.1.1 | CRYPTO_secure_actual_size |
| 0.13% | libc-2.31.so | malloc |
| 0.04% | libc-2.31.so | free |
| 0.03% | libc-2.31.so | __gconv_get_alias_db |
| 0.03% | libc-2.31.so | pthread_cond_signal |
| 0.02% | libc-2.31.so | _dl_addr |
| 0.02% | libc-2.31.so | wcsrtombs |
| 0.02% | libc-2.31.so | pthread_mutex_lock |
| 0.02% | libc-2.31.so | __errno_location |
| 0.02% | libc-2.31.so | clock_gettime |
| 0.02% | libc-2.31.so | pthread_self |
| 0.02% | libc-2.31.so | __libc_realloc |
| 0.01% | libc-2.31.so | pthread_mutex_unlock |
| 0.01% | libc-2.31.so | __xstat |
| 0.01% | libc-2.31.so | __wcsncasecmp_l |

### dict

3.43% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.56% | python | PyDict_GetItemRef |
| 0.48% | python | dict_setdefault_ref_lock_held |
| 0.46% | python | insertdict |
| 0.33% | python | PyDict_SetItem |
| 0.27% | python | dict_get |
| 0.23% | python | dictresize |
| 0.20% | python | PyDict_Next |
| 0.19% | python | insert_to_emptydict |
| 0.17% | python | PyDict_Contains |
| 0.10% | python | dict_subscript |
| 0.08% | python | dictiter_iternextitem |
| 0.05% | python | dict_merge |
| 0.03% | python | dict_ass_sub |
| 0.03% | python | dict_items |
| 0.03% | python | PyDict_GetItemWithError |
| 0.03% | python | PyDict_Copy |
| 0.02% | python | PyDict_DelItem |
| 0.02% | python | _PyDict_GetItem_KnownHash |
| 0.02% | python | _PyDict_FromItems |
| 0.02% | python | dict_getitem |
| 0.02% | python | _PyDict_Next |
| 0.02% | python | dictiter_iternextkey |
| 0.01% | python | dictiter_iternextvalue |
| 0.01% | python | PyDict_SetItemString |

### int

3.35% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.65% | python | k_mul |
| 0.45% | python | _PyLong_Add |
| 0.39% | python | x_divrem |
| 0.30% | python | PyLong_FromLong |
| 0.22% | python | long_hash |
| 0.16% | python | x_add |
| 0.13% | python | _PyLong_Subtract |
| 0.09% | python | x_sub |
| 0.09% | python | PyLong_AsLongAndOverflow |
| 0.08% | python | long_bitwise |
| 0.08% | python | _PyLong_Multiply |
| 0.07% | python | PyLong_FromString |
| 0.07% | python | long_richcompare |
| 0.06% | python | long_and |
| 0.06% | python | long_div |
| 0.06% | python | long_rshift |
| 0.05% | python | long_to_decimal_string |
| 0.05% | python | long_add |
| 0.04% | python | long_mod |
| 0.03% | python | long_mul |
| 0.02% | python | PyLong_FromUnsignedLongLong |
| 0.02% | python | long_lshift |
| 0.01% | python | long_to_decimal_string_internal |
| 0.01% | python | _PyLong_GCD |
| 0.01% | python | PyLong_FromUnsignedLong |
| 0.01% | python | _PyLong_FromBytes |
| 0.01% | python | PyLong_AsLong |
| 0.01% | python | PyLong_FromSsize_t |
| 0.01% | python | long_vectorcall |
| 0.01% | python | long_xor |
| 0.01% | python | PyLong_AsSsize_t |
| 0.01% | python | _PyLong_Lshift |
| 0.01% | python | PyLong_AsDouble.part.0 |
| 0.01% | python | _PyLong_FromByteArray |
| 0.01% | python | PyLong_AsInt |

### str

3.10% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.49% | python | siphash13 |
| 0.39% | python | unicode_decode_utf8 |
| 0.27% | python | PyUnicode_FromKindAndData |
| 0.24% | python | PyUnicode_Substring |
| 0.18% | python | _PyUnicode_JoinArray |
| 0.14% | python | PyBytes_FromStringAndSize |
| 0.09% | python | _PyUnicodeWriter_PrepareInternal |
| 0.08% | python | PyUnicode_Format |
| 0.08% | python | unicode_replace |
| 0.07% | python | _PyUnicodeWriter_WriteStr |
| 0.06% | python | PyUnicode_Concat |
| 0.06% | python | _PyUnicode_InternInPlace |
| 0.06% | python | PyUnicode_FromFormatV |
| 0.05% | python | unicode_subscript |
| 0.05% | python | PyUnicode_FSConverter |
| 0.04% | python | PyUnicode_RichCompare |
| 0.04% | python | _PyUnicode_FromUCS4 |
| 0.04% | python | _PyUnicode_Equal |
| 0.04% | python | unicode_hash |
| 0.04% | python | PyUnicode_Contains |
| 0.04% | python | unicode_encode |
| 0.03% | python | bytes_concat |
| 0.03% | python | bytes_subscript |
| 0.03% | python | PyUnicode_AsUTF8AndSize |
| 0.03% | python | unicode_encode_utf8 |
| 0.02% | python | _PyUnicode_FromASCII |
| 0.02% | python | resize_compact |
| 0.02% | python | stringlib_bytes_join.lto_priv.1 |
| 0.02% | python | unicode_startswith |
| 0.02% | python | unicode_split |
| 0.02% | python | PyUnicode_FromWideChar |
| 0.01% | python | unicode_repr |
| 0.01% | python | unicode_join |
| 0.01% | python | PyUnicode_DecodeFSDefault |
| 0.01% | python | bytes_decode |
| 0.01% | python | _PyUnicodeWriter_Finish |
| 0.01% | python | _PyUnicodeWriter_Init |
| 0.01% | python | PyBytes_Repr |
| 0.01% | python | unicode_rfind |
| 0.01% | python | unicode_rstrip |
| 0.01% | python | _PyUnicode_IsAlpha |
| 0.01% | python | unicode_splitlines |
| 0.01% | python | bytes_richcompare |
| 0.01% | python | unicode_strip |
| 0.01% | python | unicode_endswith |
| 0.01% | python | unicode_find |

### list

1.10% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.15% | python | list_iter |
| 0.14% | python | list_resize |
| 0.14% | python | list_ass_slice_lock_held |
| 0.13% | python | list_subscript |
| 0.08% | python | _PyList_FromArraySteal |
| 0.07% | python | PyList_SetSlice |
| 0.06% | python | list_contains |
| 0.04% | python | PyList_Append |
| 0.04% | python | list_vectorcall |
| 0.04% | python | list_sort_impl |
| 0.04% | python | list_append |
| 0.03% | python | list_extend |
| 0.03% | python | list_ass_subscript |
| 0.03% | python | listiter_next |
| 0.02% | python | list_concat |
| 0.02% | python | list_pop |
| 0.01% | python | list_clear_impl.constprop.0 |
| 0.01% | python | list_length |
| 0.01% | python | list_richcompare |

### tuple

1.03% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.43% | python | tuplehash |
| 0.20% | python | _PyTuple_FromArraySteal |
| 0.13% | python | tupletraverse |
| 0.07% | python | tuple_iter |
| 0.06% | python | tuplerichcompare |
| 0.04% | python | PyTuple_Pack |
| 0.03% | python | tuplecontains |
| 0.03% | python | _PyTuple_FromArray |
| 0.01% | python | tupleiter_next |
| 0.01% | python | tuplesubscript |
| 0.01% | python | _PyTuple_Resize |
| 0.01% | python | PyTuple_Size |

### lookup

1.03% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.30% | python | _Py_dict_lookup |
| 0.29% | python | find_name_in_mro |
| 0.24% | python | _Py_type_getattro |
| 0.15% | python | unicodekeys_lookup_unicode |
| 0.03% | python | builtin_getattr |
| 0.02% | python | _PyType_Lookup |

### miscobj

1.00% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.13% | python | set_contains_lock_held |
| 0.10% | python | set_issubset_impl |
| 0.09% | python | PySlice_Unpack |
| 0.09% | python | setiter_iternext |
| 0.08% | python | set_lookkey |
| 0.07% | python | PySlice_AdjustIndices |
| 0.06% | python | enum_next |
| 0.06% | python | set_vectorcall |
| 0.05% | python | set_difference |
| 0.03% | python | set_add |
| 0.02% | python | set_table_resize |
| 0.02% | python | deque_append_lock_held |
| 0.02% | python | set_add_entry |
| 0.02% | python | bytearray_ass_subscript |
| 0.02% | python | dequeiter_next_lock_held.isra.0 |
| 0.01% | python | deque_popleft_impl |
| 0.01% | python | set_merge_lock_held.part.0 |
| 0.01% | python | PyBuffer_Release |
| 0.01% | python | set_intersection |
| 0.01% | python | deque_append_impl |
| 0.01% | python | deque_clear |
| 0.01% | python | _PySlice_GetLongIndices |

### calls

0.90% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.31% | python | _PyFunction_Vectorcall |
| 0.11% | python | vgetargs1_impl |
| 0.07% | python | vectorcall_method |
| 0.06% | python | vgetargskeywords.constprop.0 |
| 0.05% | python | method_vectorcall_VARARGS |
| 0.04% | python | _PyArg_UnpackKeywords |
| 0.03% | python | cfunction_vectorcall_FASTCALL_KEYWORDS |
| 0.02% | python | method_vectorcall_VARARGS_KEYWORDS |
| 0.02% | python | cfunction_vectorcall_NOARGS |
| 0.02% | python | PyArg_UnpackTuple |
| 0.02% | python | cfunction_vectorcall_O |
| 0.02% | python | PyArg_ParseTuple |
| 0.02% | python | method_vectorcall_FASTCALL_KEYWORDS_METHOD |
| 0.01% | python | _Py_CheckFunctionResult |
| 0.01% | python | method_vectorcall_NOARGS |
| 0.01% | python | cfunction_call |
| 0.01% | python | _PyArg_UnpackKeywordsWithVararg |
| 0.01% | python | PyArg_ParseTupleAndKeywords |
| 0.01% | python | method_vectorcall_FASTCALL |
| 0.01% | python | PyArg_Parse |
| 0.01% | python | method_vectorcall_O |
| 0.01% | python | cfunction_vectorcall_FASTCALL_KEYWORDS_METHOD |

### exceptions

0.43% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.15% | python | _PyErr_SetObject |
| 0.06% | python | PyTraceBack_Here |
| 0.06% | python | PyCode_Addr2Line |
| 0.04% | python | PyErr_GivenExceptionMatches |
| 0.03% | python | PyErr_ExceptionMatches |
| 0.02% | python | BaseException_init |
| 0.01% | python | PyErr_Occurred |
| 0.01% | python | PyErr_Format |
| 0.01% | python | AttributeError_init |
| 0.01% | python | PyFrame_GetCode |

### import

0.39% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.36% | python | r_object |
| 0.02% | python | PyImport_ImportModuleLevelObject |
| 0.01% | python | PyImport_Import |

### float

0.39% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.18% | python | PyFloat_FromDouble |
| 0.07% | python | float_div |
| 0.03% | python | float_richcompare |
| 0.03% | python | float_mul |
| 0.02% | python | PyFloat_AsDouble |
| 0.02% | python | float_pow |
| 0.01% | python | float_sub |
| 0.01% | python | float_add |
| 0.01% | python | float_rem |

### gil

0.00% total

| percentage | object | symbol |
| ---: | :--- | :--- |
