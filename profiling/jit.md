
## 2to3

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.31% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.34% | `[JIT]` | `jit` | jit |
| 2.55% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.19% | `python` | `gc_collect_main` | gc |
| 2.13% | `python` | `type_new` | memory |
| 2.09% | `python` | `deduce_unreachable` | unknown |
| 1.81% | `python` | `visit_decref` | gc |
| 1.81% | `python` | `tupledealloc` | memory |
| 1.63% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.50% | `python` | `sre_ucs1_match` | library |
| 1.37% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.13% | `python` | `visit_reachable` | gc |
| 1.00% | `python` | `PyDict_GetItemRef` | dict |
| 0.97% | `python` | `_PyCode_New` | memory |
| 0.84% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.77% | `python` | `r_object` | import |
| 0.77% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.73% | `python` | `_PyPegen_fill_token` | interpreter |
| 0.72% | `python` | `list_dealloc` | memory |
| 0.66% | `python` | `gen_dealloc` | memory |
| 0.62% | `python` | `siphash13` | str |
| 0.62% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.60% | `python` | `PyObject_SetAttr` | dynamic |
| 0.59% | `python` | `PyUnicode_FromKindAndData` | str |
| 0.57% | `python` | `make_gen` | unknown |
| 0.56% | `python` | `subtype_traverse` | gc |
| 0.54% | `python` | `PyObject_GetAttr` | dynamic |
| 0.53% | `python` | `dict_dealloc` | memory |
| 0.52% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 0.51% | `python` | `PyObject_GC_Del` | gc |

## aiohttp

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 25.88% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.61% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.42% | `[JIT]` | `jit` | jit |
| 2.26% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.55% | `python` | `tupledealloc` | memory |
| 1.45% | `python` | `type_new` | memory |
| 1.13% | `python` | `gc_collect_main` | gc |
| 1.01% | `python` | `deduce_unreachable` | unknown |
| 1.00% | `python` | `visit_decref` | gc |
| 0.81% | `python` | `PyDict_GetItemRef` | dict |
| 0.79% | `python` | `subtype_dealloc` | memory |
| 0.77% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.73% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.69% | `python` | `unicode_dealloc` | memory |
| 0.66% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.66% | `python` | `visit_reachable` | gc |
| 0.63% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.60% | `python` | `dict_dealloc` | memory |
| 0.58% | `python` | `_PyCode_New` | memory |
| 0.57% | `python` | `find_name_in_mro` | lookup |
| 0.57% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.56% | `python` | `list_dealloc` | memory |
| 0.56% | `python` | `sre_ucs1_match` | library |
| 0.55% | `python` | `_PySuper_Lookup` | dynamic |
| 0.54% | `python` | `siphash13` | str |
| 0.51% | `python` | `r_object` | import |

## async_generators

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 20.26% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 9.22% | `python` | `_PyErr_SetObject` | exceptions |
| 4.25% | `python` | `StopIteration_dealloc` | memory |
| 3.88% | `[JIT]` | `jit` | jit |
| 3.69% | `python` | `BaseException_new` | memory |
| 3.30% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 2.45% | `python` | `StopIteration_init` | dynamic |
| 2.40% | `python` | `async_gen_asend_send` | unknown |
| 2.29% | `python` | `gen_send_ex` | unknown |
| 1.96% | `python` | `tupledealloc` | memory |
| 1.78% | `python` | `gen_send_ex2` | unknown |
| 1.66% | `python` | `async_gen_asend_new` | memory |
| 1.62% | `python` | `PyErr_GivenExceptionMatches` | exceptions |
| 1.56% | `python` | `PyErr_ExceptionMatches` | exceptions |
| 1.50% | `python` | `async_gen_asend_dealloc` | memory |
| 1.46% | `python` | `_PyAsyncGenValueWrapperNew` | memory |
| 1.31% | `python` | `_Py_NewReference` | memory |
| 1.30% | `python` | `async_gen_unwrap_value.isra.0` | unknown |
| 1.23% | `python` | `async_gen_wrapped_val_dealloc` | memory |
| 1.21% | `python` | `deduce_unreachable` | unknown |
| 1.19% | `python` | `gc_collect_main` | gc |
| 1.18% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.06% | `python` | `long_add` | int |
| 1.02% | `python` | `_PyGen_FetchStopIterationValue.cold` | unknown |
| 0.95% | `python` | `_PyEval_EvalFrameDefault.cold` | interpreter |
| 0.87% | `python` | `type_call` | dynamic |
| 0.83% | `python` | `visit_reachable` | gc |
| 0.81% | `python` | `_PyGen_SetStopIterationValue` | unknown |
| 0.79% | `python` | `visit_decref` | gc |
| 0.78% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.74% | `python` | `subtype_traverse` | gc |
| 0.71% | `python` | `PyObject_CallFinalizerFromDealloc` | memory |
| 0.65% | `python` | `_Py_Dealloc` | memory |
| 0.61% | `python` | `long_dealloc` | memory |
| 0.57% | `python` | `range_subscript` | unknown |
| 0.54% | `python` | `subtype_dealloc` | memory |
| 0.53% | `python` | `PyType_GenericAlloc` | memory |

## async_tree

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 18.36% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 14.09% | `python` | `gc_collect_main` | gc |
| 7.87% | `python` | `deduce_unreachable` | unknown |
| 6.11% | `python` | `visit_decref` | gc |
| 6.02% | `python` | `visit_reachable` | gc |
| 3.48% | `[JIT]` | `jit` | jit |
| 1.58% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.47% | `python` | `subtype_traverse` | gc |
| 1.30% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.11% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.93% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.90% | `python` | `tupledealloc` | memory |
| 0.89% | `python` | `PyObject_GC_Del` | gc |
| 0.85% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.82% | `python` | `_PyObject_GC_New` | gc |
| 0.78% | `python` | `gen_traverse` | gc |
| 0.74% | `python` | `insertdict` | dict |
| 0.72% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.70% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.69% | `python` | `slot_tp_init` | unknown |
| 0.66% | `python` | `meth_dealloc` | memory |
| 0.61% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.61% | `python` | `context_tp_dealloc` | memory |
| 0.54% | `python` | `list_dealloc` | memory |
| 0.54% | `python` | `gen_dealloc` | memory |
| 0.53% | `python` | `PyDict_GetItemRef` | dict |
| 0.50% | `python` | `subtype_dealloc` | memory |

## async_tree_cpu_io_mixed

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.30% | `python` | `k_mul` | int |
| 14.34% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 11.01% | `python` | `gc_collect_main` | gc |
| 6.40% | `python` | `deduce_unreachable` | unknown |
| 4.98% | `python` | `visit_decref` | gc |
| 4.72% | `python` | `visit_reachable` | gc |
| 2.45% | `[JIT]` | `jit` | jit |
| 2.26% | `python` | `long_dealloc` | memory |
| 1.33% | `python` | `subtype_traverse` | gc |
| 1.17% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.07% | `python` | `_PyLong_New` | memory |
| 0.94% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.90% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.79% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.62% | `python` | `tupledealloc` | memory |
| 0.62% | `python` | `long_mul` | int |
| 0.61% | `math.cpython-313-x86_64-linux-gnu.so` | `factorial_partial_product` | library |
| 0.59% | `python` | `gen_traverse` | gc |
| 0.56% | `python` | `_PyObject_GC_New` | gc |
| 0.54% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.51% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.50% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.50% | `python` | `PyObject_GC_Del` | gc |

## async_tree_cpu_io_mixed_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 16.73% | `python` | `k_mul` | int |
| 13.25% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 12.62% | `python` | `gc_collect_main` | gc |
| 7.89% | `python` | `deduce_unreachable` | unknown |
| 5.37% | `python` | `visit_decref` | gc |
| 5.19% | `python` | `visit_reachable` | gc |
| 2.23% | `python` | `long_dealloc` | memory |
| 1.98% | `[JIT]` | `jit` | jit |
| 1.42% | `python` | `subtype_traverse` | gc |
| 1.07% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.07% | `python` | `_PyLong_New` | memory |
| 1.00% | `python` | `gen_traverse` | gc |
| 0.95% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.82% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.71% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.70% | `python` | `set_traverse` | gc |
| 0.64% | `math.cpython-313-x86_64-linux-gnu.so` | `factorial_partial_product` | library |
| 0.60% | `python` | `long_mul` | int |
| 0.59% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.54% | `python` | `tupledealloc` | memory |
| 0.53% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |

## async_tree_io

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.44% | `python` | `gc_collect_main` | gc |
| 15.86% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 10.82% | `python` | `deduce_unreachable` | unknown |
| 8.07% | `python` | `visit_reachable` | gc |
| 7.67% | `python` | `visit_decref` | gc |
| 2.60% | `[JIT]` | `jit` | jit |
| 1.67% | `python` | `subtype_traverse` | gc |
| 1.40% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.35% | `python` | `gen_traverse` | gc |
| 0.85% | `python` | `slot_tp_richcompare` | dynamic |
| 0.82% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.65% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.63% | `python` | `tupledealloc` | memory |
| 0.60% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.57% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.56% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.54% | `python` | `PyObject_GC_Del` | gc |
| 0.52% | `_heapq.cpython-313-x86_64-linux-gnu.so` | `_heapq_heappop` | library |

## async_tree_io_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 22.49% | `python` | `gc_collect_main` | gc |
| 14.59% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 12.18% | `python` | `deduce_unreachable` | unknown |
| 8.28% | `python` | `visit_reachable` | gc |
| 7.95% | `python` | `visit_decref` | gc |
| 2.33% | `[JIT]` | `jit` | jit |
| 1.78% | `python` | `gen_traverse` | gc |
| 1.76% | `python` | `subtype_traverse` | gc |
| 1.26% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.87% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.83% | `python` | `slot_tp_richcompare` | dynamic |
| 0.70% | `python` | `set_traverse` | gc |
| 0.66% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.62% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.58% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.55% | `python` | `tupledealloc` | memory |
| 0.55% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.50% | `_heapq.cpython-313-x86_64-linux-gnu.so` | `_heapq_heappop` | library |

## async_tree_memoization

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 18.88% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 14.91% | `python` | `gc_collect_main` | gc |
| 8.57% | `python` | `deduce_unreachable` | unknown |
| 6.75% | `python` | `visit_decref` | gc |
| 6.41% | `python` | `visit_reachable` | gc |
| 3.10% | `[JIT]` | `jit` | jit |
| 1.71% | `python` | `subtype_traverse` | gc |
| 1.63% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.23% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.98% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.83% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.82% | `python` | `tupledealloc` | memory |
| 0.82% | `python` | `gen_traverse` | gc |
| 0.74% | `python` | `_PyObject_GC_New` | gc |
| 0.71% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.69% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.69% | `python` | `meth_dealloc` | memory |
| 0.67% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.65% | `python` | `PyObject_GC_Del` | gc |
| 0.62% | `python` | `slot_tp_init` | unknown |
| 0.60% | `python` | `insertdict` | dict |
| 0.59% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.59% | `python` | `context_tp_dealloc` | memory |
| 0.51% | `python` | `gen_dealloc` | memory |
| 0.50% | `python` | `list_dealloc` | memory |

## async_tree_memoization_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.20% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 16.76% | `python` | `gc_collect_main` | gc |
| 10.85% | `python` | `deduce_unreachable` | unknown |
| 7.18% | `python` | `visit_decref` | gc |
| 6.97% | `python` | `visit_reachable` | gc |
| 2.52% | `[JIT]` | `jit` | jit |
| 1.84% | `python` | `subtype_traverse` | gc |
| 1.45% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.36% | `python` | `gen_traverse` | gc |
| 1.01% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.94% | `python` | `set_traverse` | gc |
| 0.90% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.89% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.80% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.69% | `python` | `tupledealloc` | memory |
| 0.69% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.58% | `python` | `slot_tp_init` | unknown |
| 0.58% | `python` | `meth_dealloc` | memory |
| 0.56% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.54% | `python` | `PyObject_GC_Del` | gc |
| 0.54% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.53% | `python` | `make_gen` | unknown |
| 0.52% | `python` | `PyDict_GetItemRef` | dict |

## async_tree_tg

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 16.48% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 16.16% | `python` | `gc_collect_main` | gc |
| 9.79% | `python` | `deduce_unreachable` | unknown |
| 6.61% | `python` | `visit_reachable` | gc |
| 6.59% | `python` | `visit_decref` | gc |
| 2.83% | `[JIT]` | `jit` | jit |
| 1.63% | `python` | `subtype_traverse` | gc |
| 1.37% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.27% | `python` | `gen_traverse` | gc |
| 1.13% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.07% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 0.99% | `python` | `set_traverse` | gc |
| 0.96% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.77% | `python` | `PyObject_GC_Del` | gc |
| 0.77% | `python` | `tupledealloc` | memory |
| 0.73% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.72% | `_asyncio.cpython-313-x86_64-linux-gnu.so` | `TaskObj_traverse` | library |
| 0.68% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.64% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.63% | `python` | `slot_tp_init` | unknown |
| 0.61% | `python` | `PyDict_GetItemRef` | dict |
| 0.60% | `python` | `meth_dealloc` | memory |
| 0.60% | `python` | `_PyObject_GC_New` | gc |
| 0.52% | `python` | `make_gen` | unknown |
| 0.52% | `python` | `subtype_dealloc` | memory |

## asyncio_tcp

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.00% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 16.98% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 9.18% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.97% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.57% | `[kernel.kallsyms]` | `rmqueue` | kernel |
| 0.56% | `[kernel.kallsyms]` | `tcp_sendmsg_locked` | kernel |
| 0.56% | `[kernel.kallsyms]` | `native_irq_return_iret` | kernel |

## asyncio_tcp_ssl

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 38.98% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 25.71% | `libcrypto.so.1.1` | `CRYPTO_secure_actual_size` | libc |
| 10.96% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 3.50% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.89% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.85% | `libssl.so.1.1` | `SSL_rstate_string` | library |
| 0.59% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.58% | `[JIT]` | `jit` | jit |

## asyncio_websockets

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 63.84% | `libz.so.1.2.11` | `crc32_combine64` | library |
| 20.19% | `libz.so.1.2.11` | `inflateBackEnd` | library |
| 2.84% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.72% | `python` | `_PyEval_EvalFrameDefault` | interpreter |

## chameleon

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 37.45% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.43% | `python` | `long_to_decimal_string_internal` | int |
| 2.51% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.45% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.30% | `python` | `sre_ucs2_charset.isra.0` | library |
| 2.07% | `python` | `PyUnicode_Format` | str |
| 1.82% | `python` | `_PyUnicode_JoinArray` | str |
| 1.79% | `python` | `dict_get` | dict |
| 1.77% | `python` | `type_new` | memory |
| 1.55% | `[JIT]` | `jit` | jit |
| 1.46% | `python` | `insertdict` | dict |
| 1.24% | `python` | `unicode_dealloc` | memory |
| 1.12% | `python` | `list_append` | list |
| 0.95% | `python` | `gc_collect_main` | gc |
| 0.94% | `python` | `deduce_unreachable` | unknown |
| 0.90% | `python` | `visit_decref` | gc |
| 0.84% | `python` | `PyUnicode_Concat` | str |
| 0.83% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 0.82% | `python` | `list_dealloc` | memory |
| 0.78% | `python` | `state_init` | unknown |
| 0.72% | `python` | `_PyCode_New` | memory |
| 0.67% | `python` | `sre_search` | library |
| 0.67% | `python` | `visit_reachable` | gc |
| 0.60% | `python` | `tupledealloc` | memory |
| 0.59% | `python` | `r_object` | import |
| 0.58% | `python` | `PyObject_Str` | dynamic |
| 0.55% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.55% | `libc-2.31.so` | `malloc` | libc |
| 0.52% | `python` | `dict_setdefault_ref_lock_held` | dict |

## chaos

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 30.43% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 19.16% | `[JIT]` | `jit` | jit |
| 2.60% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.18% | `python` | `_PyLong_Subtract` | int |
| 1.84% | `python` | `subtype_dealloc` | memory |
| 1.47% | `python` | `_PyLong_Add` | int |
| 1.43% | `python` | `range_vectorcall` | unknown |
| 1.40% | `python` | `PyFloat_FromDouble` | float |
| 1.34% | `python` | `convert_to_double` | unknown |
| 1.21% | `python` | `float_div` | float |
| 1.09% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.01% | `python` | `PyNumber_Subtract` | dynamic |
| 1.00% | `python` | `PyType_GenericAlloc` | memory |
| 0.95% | `python` | `type_new` | memory |
| 0.94% | `libm-2.31.so` | `f64xsubf128` | library |
| 0.93% | `python` | `float_dealloc` | memory |
| 0.91% | `python` | `range_iter` | unknown |
| 0.88% | `python` | `PyNumber_TrueDivide` | dynamic |
| 0.78% | `python` | `float_richcompare` | float |
| 0.67% | `python` | `float_pow` | float |
| 0.66% | `python` | `float_sub` | float |
| 0.65% | `python` | `tupledealloc` | memory |
| 0.61% | `python` | `gc_collect_main` | gc |
| 0.60% | `python` | `PyType_IsSubtype` | dynamic |
| 0.59% | `python` | `PyLong_FromLong` | int |
| 0.59% | `python` | `deduce_unreachable` | unknown |
| 0.56% | `python` | `visit_decref` | gc |
| 0.55% | `python` | `_PyObject_InitInlineValues` | dynamic |
| 0.53% | `python` | `PyObject_RichCompare` | dynamic |
| 0.51% | `python` | `PyObject_GC_Del` | gc |
| 0.50% | `python` | `range_dealloc` | memory |

## comprehensions

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.44% | `[JIT]` | `jit` | jit |
| 20.10% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.80% | `python` | `dict_get` | dict |
| 2.31% | `python` | `PyFunction_NewWithQualName` | memory |
| 1.81% | `python` | `PyDict_GetItemRef` | dict |
| 1.76% | `python` | `list_dealloc` | memory |
| 1.67% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.51% | `python` | `gen_dealloc` | memory |
| 1.50% | `python` | `list_iter` | list |
| 1.43% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.35% | `python` | `unsafe_tuple_compare` | unknown |
| 1.22% | `python` | `func_dealloc` | memory |
| 1.18% | `python` | `PyMem_Realloc` | memory |
| 1.08% | `python` | `type_new` | memory |
| 1.00% | `python` | `listiter_dealloc` | memory |
| 0.98% | `python` | `tupledealloc` | memory |
| 0.95% | `python` | `make_gen` | unknown |
| 0.90% | `python` | `long_hash` | int |
| 0.89% | `python` | `PyObject_GC_Del` | gc |
| 0.84% | `python` | `long_richcompare` | int |
| 0.83% | `python` | `insertdict` | dict |
| 0.74% | `python` | `PyObject_RichCompare` | dynamic |
| 0.71% | `python` | `_PyDict_SetItem_Take2` | dict |
| 0.69% | `python` | `gc_collect_main` | gc |
| 0.67% | `python` | `_Py_type_getattro` | lookup |
| 0.66% | `python` | `visit_decref` | gc |
| 0.64% | `python` | `_PyObject_Malloc` | memory |
| 0.62% | `python` | `PyObject_IsTrue` | dynamic |
| 0.62% | `python` | `list_resize` | list |
| 0.62% | `python` | `deduce_unreachable` | unknown |
| 0.57% | `python` | `dictresize` | dict |
| 0.53% | `python` | `list_sort_impl` | list |

## concurrent_imap

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.81% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.02% | `[JIT]` | `jit` | jit |
| 2.07% | `[kernel.kallsyms]` | `perf_event_alloc` | kernel |
| 1.85% | `[kernel.kallsyms]` | `memset_erms` | kernel |
| 1.75% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.53% | `python` | `subtype_dealloc` | memory |
| 1.10% | `python` | `tupledealloc` | memory |
| 1.05% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 1.01% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.94% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.83% | `[kernel.kallsyms]` | `mutex_unlock` | kernel |
| 0.81% | `[kernel.kallsyms]` | `_raw_spin_lock` | kernel |
| 0.81% | `python` | `PyObject_GC_Del` | gc |
| 0.78% | `[kernel.kallsyms]` | `mutex_lock` | kernel |
| 0.78% | `[kernel.kallsyms]` | `kfree` | kernel |
| 0.74% | `[kernel.kallsyms]` | `page_counter_cancel` | kernel |
| 0.73% | `[kernel.kallsyms]` | `inherit_event.isra.0` | kernel |
| 0.72% | `[kernel.kallsyms]` | `zap_pte_range.isra.0` | kernel |
| 0.69% | `python` | `list_dealloc` | memory |
| 0.67% | `python` | `long_dealloc` | memory |
| 0.66% | `python` | `method_dealloc` | memory |
| 0.63% | `[kernel.kallsyms]` | `find_vma` | kernel |
| 0.54% | `python` | `type_new` | memory |
| 0.53% | `[kernel.kallsyms]` | `kmem_cache_free` | kernel |
| 0.52% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.50% | `[kernel.kallsyms]` | `_raw_spin_lock_irqsave` | kernel |

## coroutines

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 39.53% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 14.51% | `python` | `gen_dealloc` | memory |
| 9.30% | `python` | `make_gen` | unknown |
| 6.74% | `python` | `_PyEval_EvalFrameDefault.cold` | interpreter |
| 4.91% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.54% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.54% | `python` | `_PyLong_Subtract` | int |
| 1.89% | `python` | `_PyFrame_ClearExceptCode` | interpreter |
| 1.37% | `python` | `_PyLong_Add` | int |
| 1.01% | `python` | `_PyCoro_GetAwaitableIter` | unknown |
| 0.76% | `python` | `type_new` | memory |
| 0.51% | `python` | `gc_collect_main` | gc |

## coverage

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.78% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.20% | `tracer.cpython-313-x86_64-linux-gnu.so` | `CTracer_trace` | library |
| 4.14% | `python` | `call_instrumentation_vector` | unknown |
| 3.54% | `python` | `unicode_decode_utf8` | str |
| 3.27% | `python` | `PyObject_SetAttrString` | dynamic |
| 2.96% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 2.65% | `python` | `siphash13` | str |
| 2.63% | `python` | `_Py_dict_lookup` | lookup |
| 2.20% | `python` | `PyLong_FromLong` | int |
| 1.92% | `python` | `call_one_instrument` | unknown |
| 1.90% | `python` | `PySet_Add` | unknown |
| 1.87% | `python` | `frame_dealloc` | memory |
| 1.63% | `python` | `_PyFrame_MakeAndSetFrameObject` | unknown |
| 1.56% | `python` | `type_new` | memory |
| 1.47% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.37% | `python` | `_PyObject_VectorcallTstate.lto_priv.5` | dynamic |
| 1.28% | `python` | `PyObject_SetAttr` | dynamic |
| 1.24% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.15% | `python` | `unicode_dealloc` | memory |
| 1.11% | `python` | `dict_getitem` | dict |
| 1.09% | `python` | `_Py_hashtable_get` | unknown |
| 1.06% | `[JIT]` | `jit` | jit |
| 1.03% | `python` | `gc_collect_main` | gc |
| 1.01% | `python` | `deduce_unreachable` | unknown |
| 1.00% | `python` | `visit_decref` | gc |
| 0.94% | `python` | `call_trace_func.isra.0` | unknown |
| 0.77% | `python` | `_PyUnicode_InternInPlace` | str |
| 0.76% | `python` | `visit_reachable` | gc |
| 0.74% | `python` | `_PyCode_New` | memory |
| 0.66% | `python` | `_PyCode_GetCode` | unknown |
| 0.63% | `python` | `_Py_call_instrumentation_jump` | unknown |
| 0.56% | `python` | `r_object` | import |
| 0.54% | `python` | `tupledealloc` | memory |

## crypto_pyaes

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 25.63% | `[JIT]` | `jit` | jit |
| 10.12% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.09% | `python` | `long_dealloc` | memory |
| 7.02% | `python` | `long_bitwise` | int |
| 4.91% | `python` | `long_rshift` | int |
| 3.43% | `python` | `long_mod` | int |
| 3.38% | `python` | `long_and` | int |
| 3.17% | `python` | `_PyLong_New` | memory |
| 1.44% | `python` | `binary_op` | unknown |
| 1.21% | `python` | `PyNumber_And` | dynamic |
| 1.14% | `python` | `_PyLong_Add` | int |
| 1.13% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.11% | `python` | `PyObject_Free` | dynamic |
| 0.98% | `python` | `list_dealloc` | memory |
| 0.90% | `python` | `type_new` | memory |
| 0.88% | `python` | `PyNumber_Remainder` | dynamic |
| 0.84% | `python` | `PyNumber_Rshift` | dynamic |
| 0.78% | `python` | `long_xor` | int |
| 0.69% | `python` | `range_vectorcall` | unknown |
| 0.64% | `python` | `_PyLong_FromSTwoDigits` | int |
| 0.61% | `python` | `gc_collect_main` | gc |
| 0.60% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.56% | `python` | `range_iter` | unknown |
| 0.55% | `python` | `visit_decref` | gc |
| 0.55% | `python` | `deduce_unreachable` | unknown |

## dask

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.73% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.41% | `python` | `gc_collect_main` | gc |
| 2.31% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.12% | `python` | `deduce_unreachable` | unknown |
| 2.10% | `python` | `visit_decref` | gc |
| 1.91% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.78% | `[JIT]` | `jit` | jit |
| 1.61% | `python` | `tupledealloc` | memory |
| 1.59% | `python` | `visit_reachable` | gc |
| 0.99% | `python` | `object_isinstance` | dynamic |
| 0.95% | `python` | `PyDict_GetItemRef` | dict |
| 0.86% | `python` | `dict_dealloc` | memory |
| 0.81% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.80% | `python` | `PyBytes_Repr` | str |
| 0.72% | `python` | `type_new` | memory |
| 0.71% | `python` | `long_dealloc` | memory |
| 0.62% | `python` | `insertdict` | dict |
| 0.55% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.51% | `python` | `_PyObject_GC_New` | gc |
| 0.51% | `python` | `list_dealloc` | memory |

## deepcopy

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 43.51% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.62% | `python` | `dict_get` | dict |
| 4.30% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.61% | `[JIT]` | `jit` | jit |
| 2.64% | `python` | `_PyLong_New` | memory |
| 2.57% | `python` | `long_dealloc` | memory |
| 1.54% | `python` | `insertdict` | dict |
| 1.28% | `python` | `PySys_Audit` | unknown |
| 1.22% | `python` | `long_hash` | int |
| 1.15% | `python` | `builtin_id` | unknown |
| 1.13% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.10% | `python` | `PyDict_GetItemRef` | dict |
| 0.88% | `python` | `tupledealloc` | memory |
| 0.86% | `python` | `insert_to_emptydict` | dict |
| 0.75% | `python` | `list_dealloc` | memory |
| 0.74% | `python` | `type_new` | memory |
| 0.70% | `python` | `dict_dealloc` | memory |
| 0.65% | `python` | `list_append` | list |
| 0.62% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.50% | `python` | `PyMem_Realloc` | memory |

## deltablue

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 46.55% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 9.62% | `[JIT]` | `jit` | jit |
| 4.63% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.27% | `python` | `_PyObject_GetMethod` | dynamic |
| 1.42% | `python` | `gc_collect_main` | gc |
| 1.39% | `python` | `deduce_unreachable` | unknown |
| 1.19% | `python` | `visit_decref` | gc |
| 1.12% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.03% | `python` | `type_new` | memory |
| 1.02% | `python` | `_PySuper_Lookup` | dynamic |
| 0.74% | `python` | `_Py_type_getattro` | lookup |
| 0.71% | `python` | `subtype_traverse` | gc |
| 0.66% | `python` | `PyObject_GC_Del` | gc |
| 0.65% | `python` | `method_dealloc` | memory |
| 0.65% | `python` | `visit_reachable` | gc |
| 0.59% | `python` | `cm_descr_get` | unknown |
| 0.51% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 0.50% | `python` | `PyObject_GetAttr` | dynamic |
| 0.50% | `python` | `_PyCode_New` | memory |

## django_template

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 34.88% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.93% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.20% | `python` | `type_new` | memory |
| 1.96% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.62% | `python` | `object_isinstance` | dynamic |
| 1.46% | `[JIT]` | `jit` | jit |
| 1.32% | `python` | `gc_collect_main` | gc |
| 1.27% | `python` | `PyObject_GC_Del` | gc |
| 1.23% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.22% | `python` | `tupledealloc` | memory |
| 1.22% | `python` | `deduce_unreachable` | unknown |
| 1.16% | `python` | `insertdict` | dict |
| 1.15% | `python` | `visit_decref` | gc |
| 0.93% | `python` | `PyDict_GetItemRef` | dict |
| 0.85% | `python` | `visit_reachable` | gc |
| 0.82% | `python` | `_PyCode_New` | memory |
| 0.81% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.79% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.77% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.72% | `python` | `list_dealloc` | memory |
| 0.67% | `python` | `unicode_replace` | str |
| 0.67% | `python` | `r_object` | import |
| 0.65% | `python` | `dict_dealloc` | memory |
| 0.64% | `python` | `builtin_hasattr` | unknown |
| 0.54% | `python` | `_PyObject_GC_New` | gc |
| 0.54% | `python` | `long_to_decimal_string_internal` | int |
| 0.52% | `python` | `PyUnicode_FromKindAndData` | str |
| 0.52% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |

## djangocms

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.17% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.48% | `python` | `find_name_in_mro` | lookup |
| 3.03% | `python` | `type_new` | memory |
| 2.94% | `[JIT]` | `jit` | jit |
| 2.47% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.26% | `python` | `gc_collect_main` | gc |
| 2.00% | `python` | `deduce_unreachable` | unknown |
| 1.75% | `python` | `visit_decref` | gc |
| 1.52% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.42% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.40% | `libsqlite3.so.0.8.6` | `sqlite3_exec` | library |
| 1.24% | `python` | `visit_reachable` | gc |
| 1.16% | `python` | `tupledealloc` | memory |
| 1.11% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.01% | `python` | `PyDict_GetItemRef` | dict |
| 0.88% | `python` | `sre_ucs1_match` | library |
| 0.75% | `python` | `dict_traverse` | gc |
| 0.72% | `python` | `dict_dealloc` | memory |
| 0.65% | `libz.so.1.2.11` | `inflateBackEnd` | library |
| 0.65% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.63% | `python` | `insertdict` | dict |
| 0.62% | `python` | `unicode_dealloc` | memory |
| 0.57% | `python` | `PyObject_SetAttr` | dynamic |
| 0.55% | `python` | `_PyCode_New` | memory |
| 0.55% | `libpthread-2.31.so` | `__pthread_mutex_lock` | library |
| 0.54% | `python` | `_PyPegen_fill_token` | interpreter |
| 0.53% | `libsqlite3.so.0.8.6` | `sqlite3_str_value` | library |
| 0.51% | `python` | `list_dealloc` | memory |

## docutils

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 22.06% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.52% | `python` | `sre_ucs1_match` | library |
| 5.25% | `[JIT]` | `jit` | jit |
| 3.54% | `python` | `gc_collect_main` | gc |
| 3.31% | `python` | `deduce_unreachable` | unknown |
| 2.78% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 2.32% | `python` | `sre_ucs2_charset.isra.0` | library |
| 2.30% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.28% | `python` | `visit_decref` | gc |
| 1.90% | `python` | `list_dealloc` | memory |
| 1.88% | `python` | `find_name_in_mro` | lookup |
| 1.79% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.30% | `python` | `visit_reachable` | gc |
| 1.08% | `python` | `PyObject_SetAttr` | dynamic |
| 1.08% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.89% | `python` | `tupledealloc` | memory |
| 0.87% | `python` | `_PyUnicode_JoinArray` | str |
| 0.82% | `python` | `subtype_traverse` | gc |
| 0.81% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 0.79% | `python` | `PyDict_GetItemRef` | dict |
| 0.79% | `python` | `PyObject_GetAttr` | dynamic |
| 0.76% | `python` | `object_isinstance` | dynamic |
| 0.73% | `python` | `PyMem_Free` | memory |
| 0.68% | `python` | `list_traverse` | gc |
| 0.67% | `python` | `list_subscript` | list |
| 0.63% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.59% | `python` | `dict_traverse` | gc |
| 0.57% | `python` | `unicode_dealloc` | memory |
| 0.56% | `python` | `dict_dealloc` | memory |
| 0.56% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.54% | `python` | `PyMem_Malloc` | memory |
| 0.54% | `python` | `PyUnicode_Format` | str |
| 0.53% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.52% | `python` | `insertdict` | dict |
| 0.51% | `python` | `dict_subscript` | dict |

## dulwich_log

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 26.80% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.04% | `[JIT]` | `jit` | jit |
| 2.84% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.77% | `libz.so.1.2.11` | `inflateCodesUsed` | library |
| 1.66% | `libz.so.1.2.11` | `inflateBackEnd` | library |
| 1.61% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.46% | `libz.so.1.2.11` | `inflate` | library |
| 1.20% | `python` | `tupledealloc` | memory |
| 1.17% | `python` | `PyBytes_FromStringAndSize` | str |
| 1.09% | `python` | `type_new` | memory |
| 0.91% | `python` | `PyObject_Free` | dynamic |
| 0.86% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.75% | `python` | `gc_collect_main` | gc |
| 0.74% | `python` | `list_dealloc` | memory |
| 0.69% | `python` | `deduce_unreachable` | unknown |
| 0.69% | `python` | `visit_decref` | gc |
| 0.67% | `python` | `long_dealloc` | memory |
| 0.56% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 0.54% | `python` | `PyList_New` | memory |
| 0.51% | `[kernel.kallsyms]` | `__d_lookup_rcu` | kernel |
| 0.50% | `python` | `siphash13` | str |

## fannkuch

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 36.34% | `[JIT]` | `jit` | jit |
| 6.91% | `python` | `list_dealloc` | memory |
| 6.82% | `python` | `list_ass_slice_lock_held` | list |
| 5.89% | `python` | `PySlice_AdjustIndices` | miscobj |
| 4.12% | `python` | `PySlice_Unpack` | miscobj |
| 4.07% | `python` | `list_subscript` | list |
| 3.69% | `python` | `list_new_prealloc` | memory |
| 3.26% | `python` | `slice_dealloc` | memory |
| 2.46% | `python` | `_PyLong_Add` | int |
| 2.27% | `python` | `PySlice_New` | memory |
| 2.22% | `python` | `_PyBuildSlice_ConsumeRefs` | miscobj |
| 1.91% | `python` | `list_ass_subscript` | list |
| 1.50% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 1.40% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.07% | `python` | `PyObject_GetItem` | dynamic |
| 1.01% | `python` | `ins1` | unknown |
| 0.98% | `python` | `PyNumber_AsSsize_t` | dynamic |
| 0.77% | `python` | `list_pop` | list |
| 0.77% | `python` | `PyMem_Malloc` | memory |
| 0.75% | `python` | `_PyLong_Subtract` | int |
| 0.72% | `python` | `_Py_Dealloc` | memory |
| 0.62% | `python` | `PyObject_SetItem` | dynamic |

## float

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.45% | `[JIT]` | `jit` | jit |
| 12.87% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.76% | `libm-2.31.so` | `f64xsubf128` | library |
| 3.47% | `python` | `subtype_traverse` | gc |
| 2.55% | `python` | `visit_decref` | gc |
| 2.42% | `python` | `gc_collect_main` | gc |
| 2.30% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.22% | `python` | `visit_reachable` | gc |
| 2.18% | `python` | `deduce_unreachable` | unknown |
| 1.90% | `python` | `float_div` | float |
| 1.67% | `python` | `PyFloat_FromDouble` | float |
| 1.58% | `python` | `object_new` | memory |
| 1.53% | `python` | `slot_tp_init` | unknown |
| 1.41% | `python` | `_PyObject_Malloc` | memory |
| 1.18% | `python` | `PyFloat_AsDouble` | float |
| 1.08% | `python` | `clear_slots` | unknown |
| 1.04% | `python` | `_PyObject_Free` | memory |
| 1.02% | `python` | `float_dealloc` | memory |
| 0.87% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.86% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.82% | `python` | `tupledealloc` | memory |
| 0.81% | `python` | `type_new` | memory |
| 0.81% | `python` | `long_dealloc` | memory |
| 0.74% | `python` | `subtype_dealloc` | memory |
| 0.74% | `python` | `PyLong_FromLong` | int |
| 0.66% | `python` | `binary_op1` | unknown |
| 0.54% | `python` | `list_dealloc` | memory |
| 0.53% | `python` | `PyObject_GC_Del` | gc |

## gc_collect

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.62% | `python` | `gc_collect_main` | gc |
| 14.45% | `python` | `visit_decref` | gc |
| 14.40% | `python` | `visit_reachable` | gc |
| 11.50% | `python` | `deduce_unreachable` | unknown |
| 6.28% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.83% | `python` | `dict_traverse` | gc |
| 3.00% | `python` | `subtype_traverse` | gc |
| 1.96% | `python` | `func_traverse` | gc |
| 1.69% | `python` | `set_traverse` | gc |
| 0.93% | `[JIT]` | `jit` | jit |
| 0.86% | `python` | `tupletraverse` | tuple |
| 0.85% | `python` | `type_traverse` | gc |
| 0.80% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.74% | `python` | `PyType_GenericAlloc` | memory |
| 0.73% | `python` | `list_traverse` | gc |
| 0.56% | `python` | `subtype_dealloc` | memory |
| 0.51% | `python` | `meth_traverse` | gc |
| 0.51% | `python` | `_PyObject_InitInlineValues` | dynamic |

## gc_traversal

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 29.68% | `python` | `visit_reachable` | gc |
| 21.58% | `python` | `visit_decref` | gc |
| 14.23% | `python` | `list_traverse` | gc |
| 8.90% | `python` | `gc_collect_main` | gc |
| 3.87% | `python` | `deduce_unreachable` | unknown |
| 2.60% | `[JIT]` | `jit` | jit |
| 2.18% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 1.73% | `python` | `dict_traverse` | gc |
| 0.78% | `python` | `func_traverse` | gc |
| 0.66% | `python` | `subtype_traverse` | gc |
| 0.63% | `python` | `set_traverse` | gc |
| 0.52% | `python` | `PyLong_FromLong` | int |
| 0.51% | `python` | `type_new` | memory |

## generators

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 49.01% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.84% | `python` | `gen_dealloc` | memory |
| 2.63% | `python` | `gc_collect_main` | gc |
| 2.52% | `python` | `deduce_unreachable` | unknown |
| 2.32% | `python` | `long_add` | int |
| 1.87% | `python` | `make_gen` | unknown |
| 1.70% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.68% | `python` | `visit_reachable` | gc |
| 1.66% | `python` | `subtype_traverse` | gc |
| 1.57% | `python` | `visit_decref` | gc |
| 1.47% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.32% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.31% | `python` | `long_dealloc` | memory |
| 1.18% | `python` | `range_subscript` | unknown |
| 1.02% | `python` | `subtype_dealloc` | memory |
| 0.78% | `python` | `make_range_object` | unknown |
| 0.74% | `python` | `_PyObject_New` | memory |
| 0.68% | `python` | `type_new` | memory |
| 0.59% | `python` | `range_dealloc` | memory |
| 0.58% | `[JIT]` | `jit` | jit |
| 0.58% | `python` | `slot_tp_iter` | unknown |
| 0.57% | `python` | `PyType_GenericAlloc` | memory |
| 0.50% | `python` | `PyObject_CallOneArg` | dynamic |

## genshi

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.02% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 14.13% | `[JIT]` | `jit` | jit |
| 2.02% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.66% | `python` | `insertdict` | dict |
| 1.49% | `python` | `tupledealloc` | memory |
| 1.31% | `python` | `insert_to_emptydict` | dict |
| 1.30% | `python` | `_PyObject_GetMethod` | dynamic |
| 1.29% | `python` | `_PyObject_GC_New` | gc |
| 1.25% | `python` | `dictresize` | dict |
| 1.14% | `python` | `dict_dealloc` | memory |
| 1.11% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.03% | `python` | `long_to_decimal_string_internal` | int |
| 0.99% | `python` | `PyObject_GC_Del` | gc |
| 0.96% | `python` | `object_isinstance` | dynamic |
| 0.93% | `python` | `_PyDict_FromItems` | dict |
| 0.88% | `python` | `type_new` | memory |
| 0.88% | `python` | `_Py_type_getattro` | lookup |
| 0.87% | `python` | `method_dealloc` | memory |
| 0.86% | `python` | `PyDict_GetItemRef` | dict |
| 0.85% | `python` | `cm_descr_get` | unknown |
| 0.66% | `python` | `dict_get` | dict |
| 0.66% | `python` | `PyDict_SetItem` | dict |
| 0.65% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.61% | `python` | `PyObject_IsTrue` | dynamic |
| 0.61% | `python` | `PyDict_Contains` | dict |
| 0.61% | `python` | `deduce_unreachable` | unknown |
| 0.60% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.59% | `python` | `gen_iternext` | unknown |
| 0.58% | `python` | `gc_collect_main` | gc |
| 0.53% | `python` | `func_dealloc` | memory |

## go

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 47.59% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 14.61% | `[JIT]` | `jit` | jit |
| 3.21% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.83% | `python` | `_PyObject_GetMethod` | dynamic |
| 1.36% | `python` | `PyDict_GetItemRef` | dict |
| 1.21% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.15% | `python` | `uop_optimize` | unknown |
| 1.02% | `python` | `long_bitwise` | int |
| 0.99% | `python` | `long_dealloc` | memory |
| 0.92% | `python` | `PyDict_SetItem` | dict |
| 0.81% | `python` | `type_new` | memory |
| 0.70% | `python` | `_PyLong_Add` | int |
| 0.60% | `python` | `gc_collect_main` | gc |
| 0.56% | `python` | `deduce_unreachable` | unknown |
| 0.55% | `python` | `visit_decref` | gc |
| 0.52% | `python` | `list_iter` | list |
| 0.51% | `python` | `PyObject_GC_Del` | gc |

## gunicorn

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 27.63% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.45% | `[JIT]` | `jit` | jit |
| 2.41% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.36% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.62% | `python` | `type_new` | memory |
| 1.57% | `python` | `tupledealloc` | memory |
| 1.13% | `python` | `gc_collect_main` | gc |
| 1.03% | `python` | `deduce_unreachable` | unknown |
| 0.96% | `python` | `visit_decref` | gc |
| 0.83% | `python` | `PyDict_GetItemRef` | dict |
| 0.79% | `python` | `subtype_dealloc` | memory |
| 0.79% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.77% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.69% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.69% | `python` | `visit_reachable` | gc |
| 0.67% | `python` | `_PyCode_New` | memory |
| 0.66% | `python` | `unicode_dealloc` | memory |
| 0.66% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.64% | `python` | `find_name_in_mro` | lookup |
| 0.62% | `python` | `dict_dealloc` | memory |
| 0.58% | `python` | `sre_ucs1_match` | library |
| 0.57% | `python` | `r_object` | import |
| 0.56% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.53% | `python` | `list_dealloc` | memory |
| 0.50% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.50% | `python` | `_PySuper_Lookup` | dynamic |

## hexiom

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 33.61% | `[JIT]` | `jit` | jit |
| 21.09% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.95% | `python` | `list_contains` | list |
| 2.90% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.74% | `python` | `long_richcompare` | int |
| 1.44% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.05% | `python` | `type_new` | memory |
| 0.90% | `python` | `slot_mp_subscript` | unknown |
| 0.82% | `python` | `gen_iternext` | unknown |
| 0.75% | `python` | `PyObject_Size` | dynamic |
| 0.75% | `python` | `builtin_sum` | unknown |
| 0.74% | `python` | `list_dealloc` | memory |
| 0.70% | `python` | `PyLong_FromLong` | int |
| 0.70% | `python` | `gc_collect_main` | gc |
| 0.66% | `python` | `deduce_unreachable` | unknown |
| 0.66% | `python` | `uop_optimize` | unknown |
| 0.65% | `python` | `visit_decref` | gc |
| 0.59% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.53% | `python` | `tupledealloc` | memory |
| 0.52% | `python` | `PyLong_FromSsize_t` | int |

## html5lib

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 34.07% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.94% | `python` | `sre_ucs2_charset.isra.0` | library |
| 3.39% | `[JIT]` | `jit` | jit |
| 1.93% | `python` | `gc_collect_main` | gc |
| 1.80% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.76% | `python` | `PyDict_GetItemRef` | dict |
| 1.68% | `python` | `deduce_unreachable` | unknown |
| 1.66% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.38% | `python` | `visit_decref` | gc |
| 1.15% | `python` | `type_new` | memory |
| 0.84% | `python` | `sre_ucs1_count` | library |
| 0.79% | `python` | `visit_reachable` | gc |
| 0.75% | `python` | `tupledealloc` | memory |
| 0.73% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.72% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.70% | `python` | `insertdict` | dict |
| 0.62% | `python` | `unicode_dealloc` | memory |
| 0.61% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.56% | `python` | `list_dealloc` | memory |
| 0.54% | `python` | `set_contains_lock_held` | miscobj |
| 0.54% | `python` | `_PyCode_New` | memory |
| 0.51% | `python` | `dict_dealloc` | memory |

## json

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 17.99% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_object_unicode` | library |
| 7.85% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.65% | `python` | `PyUnicode_Substring` | str |
| 5.54% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 5.31% | `python` | `siphash13` | str |
| 5.08% | `python` | `PyDict_SetItem` | dict |
| 3.27% | `python` | `unicode_dealloc` | memory |
| 3.19% | `python` | `dictresize` | dict |
| 2.87% | `python` | `PyLong_FromString` | int |
| 2.23% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.20% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 2.15% | `python` | `dict_dealloc` | memory |
| 1.82% | `python` | `_sre_SRE_Pattern_match` | library |
| 1.44% | `_json.cpython-313-x86_64-linux-gnu.so` | `_match_number_unicode.isra.0` | library |
| 1.14% | `[JIT]` | `jit` | jit |
| 1.13% | `python` | `PyBytes_FromStringAndSize` | str |
| 1.04% | `python` | `PyObject_Free` | dynamic |
| 0.83% | `python` | `type_new` | memory |
| 0.82% | `python` | `PyDict_GetItemRef` | dict |
| 0.79% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.77% | `python` | `tupledealloc` | memory |
| 0.72% | `python` | `insert_to_emptydict` | dict |
| 0.67% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.61% | `python` | `sre_ucs1_match` | library |
| 0.58% | `python` | `long_dealloc` | memory |
| 0.55% | `python` | `gc_collect_main` | gc |
| 0.54% | `python` | `deduce_unreachable` | unknown |
| 0.51% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 0.50% | `python` | `unicode_hash` | str |

## json_dumps

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 14.06% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 8.54% | `_json.cpython-313-x86_64-linux-gnu.so` | `encoder_encode_key_value` | library |
| 6.59% | `python` | `PyUnicode_New` | memory |
| 5.05% | `python` | `_PyUnicodeWriter_WriteStr` | str |
| 4.62% | `python` | `unicode_dealloc` | memory |
| 3.24% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 3.02% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.90% | `_json.cpython-313-x86_64-linux-gnu.so` | `py_encode_basestring_ascii` | library |
| 2.53% | `python` | `PyDict_GetItemRef` | dict |
| 2.29% | `python` | `vgetargskeywords.constprop.0` | calls |
| 1.62% | `python` | `resize_compact` | str |
| 1.58% | `python` | `long_to_decimal_string` | int |
| 1.53% | `python` | `tupledealloc` | memory |
| 1.42% | `python` | `_PyObject_Malloc` | memory |
| 1.31% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.27% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.23% | `python` | `PyDict_Next` | dict |
| 1.09% | `python` | `PyDict_SetItem` | dict |
| 1.09% | `python` | `PyFunction_NewWithQualName` | memory |
| 1.04% | `[JIT]` | `jit` | jit |
| 0.91% | `python` | `object_isinstance` | dynamic |
| 0.80% | `python` | `_PyLong_New` | memory |
| 0.80% | `python` | `func_dealloc` | memory |
| 0.79% | `python` | `type_new` | memory |
| 0.77% | `python` | `long_hash` | int |
| 0.73% | `python` | `PyDict_DelItem` | dict |
| 0.68% | `python` | `PyTuple_New` | memory |
| 0.67% | `python` | `_Py_type_getattro` | lookup |
| 0.65% | `python` | `_Py_dict_lookup` | lookup |
| 0.63% | `python` | `long_dealloc` | memory |
| 0.62% | `_json.cpython-313-x86_64-linux-gnu.so` | `encoder_listencode_obj` | library |
| 0.61% | `python` | `PyDict_Contains` | dict |
| 0.60% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.56% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.53% | `python` | `deduce_unreachable` | unknown |

## json_loads

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 19.68% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_object_unicode` | library |
| 10.28% | `python` | `PyUnicode_Substring` | str |
| 6.35% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.21% | `python` | `siphash13` | str |
| 5.85% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 5.30% | `python` | `PyDict_SetItem` | dict |
| 4.13% | `python` | `unicode_dealloc` | memory |
| 3.21% | `python` | `PyLong_FromString` | int |
| 2.41% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.34% | `python` | `dictresize` | dict |
| 1.34% | `python` | `PyBytes_FromStringAndSize` | str |
| 1.24% | `python` | `dict_dealloc` | memory |
| 1.21% | `_json.cpython-313-x86_64-linux-gnu.so` | `_match_number_unicode.isra.0` | library |
| 1.06% | `python` | `PyObject_Free` | dynamic |
| 0.97% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.93% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.89% | `python` | `type_new` | memory |
| 0.85% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_array_unicode` | library |
| 0.73% | `[JIT]` | `jit` | jit |
| 0.60% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.60% | `python` | `gc_collect_main` | gc |
| 0.59% | `python` | `unicode_hash` | str |
| 0.57% | `python` | `deduce_unreachable` | unknown |
| 0.56% | `python` | `tupledealloc` | memory |
| 0.52% | `python` | `visit_decref` | gc |
| 0.51% | `python` | `long_dealloc` | memory |

## logging

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 44.34% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.46% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.31% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 2.83% | `[JIT]` | `jit` | jit |
| 2.11% | `python` | `PyDict_GetItemRef` | dict |
| 1.82% | `python` | `dict_dealloc` | memory |
| 1.79% | `python` | `PyCode_Addr2Line` | exceptions |
| 1.70% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.21% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.89% | `python` | `tupledealloc` | memory |
| 0.71% | `python` | `type_new` | memory |
| 0.67% | `python` | `unicode_subscript` | str |
| 0.63% | `python` | `frame_dealloc` | memory |
| 0.59% | `python` | `PyObject_GetAttr` | dynamic |
| 0.58% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 0.58% | `python` | `meth_dealloc` | memory |
| 0.55% | `python` | `unicode_dealloc` | memory |
| 0.52% | `python` | `PyLong_FromLong` | int |
| 0.51% | `python` | `vgetargs1_impl` | calls |

## mako

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 31.94% | `[JIT]` | `jit` | jit |
| 8.88% | `python` | `long_to_decimal_string_internal` | int |
| 8.27% | `python` | `unicode_replace` | str |
| 4.25% | `python` | `_PyUnicode_JoinArray` | str |
| 4.21% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.54% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.12% | `python` | `dequeiter_next_lock_held.isra.0` | miscobj |
| 2.11% | `python` | `unicode_dealloc` | memory |
| 1.68% | `python` | `deque_append_lock_held` | miscobj |
| 1.57% | `python` | `PyObject_Str` | dynamic |
| 1.29% | `python` | `list_dealloc` | memory |
| 1.24% | `python` | `PySequence_List` | dynamic |
| 1.22% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.10% | `python` | `sre_ucs2_charset.isra.0` | library |
| 0.92% | `python` | `type_new` | memory |
| 0.78% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.75% | `python` | `deque_clear` | miscobj |
| 0.66% | `python` | `deque_append_impl` | miscobj |
| 0.61% | `python` | `gc_collect_main` | gc |
| 0.59% | `python` | `visit_decref` | gc |
| 0.57% | `python` | `deduce_unreachable` | unknown |
| 0.52% | `[kernel.kallsyms]` | `native_irq_return_iret` | kernel |
| 0.51% | `python` | `PyLong_FromLong` | int |

## mdp

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 36.40% | `python` | `tuplehash` | tuple |
| 12.86% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 12.42% | `python` | `long_hash` | int |
| 6.59% | `[JIT]` | `jit` | jit |
| 5.65% | `python` | `dict_subscript` | dict |
| 2.95% | `python` | `tuplerichcompare` | tuple |
| 1.31% | `python` | `insertdict` | dict |
| 1.19% | `python` | `_PyLong_GCD` | int |
| 1.12% | `python` | `PyDict_GetItemRef` | dict |
| 1.05% | `python` | `_PySuper_Lookup` | dynamic |
| 0.88% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.83% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.78% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.59% | `python` | `builtin_sum` | unknown |
| 0.57% | `python` | `gen_dealloc` | memory |
| 0.54% | `python` | `_PySet_Contains` | unknown |
| 0.52% | `python` | `tupledealloc` | memory |

## meteor_contest

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 12.44% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 11.36% | `[JIT]` | `jit` | jit |
| 8.32% | `python` | `set_issubset_impl` | miscobj |
| 5.66% | `python` | `setiter_iternext` | miscobj |
| 4.90% | `python` | `set_lookkey` | miscobj |
| 4.53% | `python` | `set_difference` | miscobj |
| 4.13% | `python` | `set_dealloc` | memory |
| 3.05% | `python` | `builtin_min` | unknown |
| 2.30% | `python` | `list_dealloc` | memory |
| 1.86% | `python` | `set_add_entry` | miscobj |
| 1.65% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.40% | `python` | `PyObject_GC_Del` | gc |
| 1.39% | `python` | `list_subscript` | list |
| 1.26% | `python` | `long_richcompare` | int |
| 1.16% | `python` | `set_table_resize` | miscobj |
| 1.07% | `python` | `type_new` | memory |
| 1.04% | `python` | `PyObject_RichCompare` | dynamic |
| 1.03% | `python` | `make_new_set` | memory |
| 0.88% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.87% | `python` | `set_intersection` | miscobj |
| 0.73% | `python` | `gc_collect_main` | gc |
| 0.70% | `python` | `visit_decref` | gc |
| 0.67% | `python` | `_PyObject_GC_New` | gc |
| 0.65% | `python` | `deduce_unreachable` | unknown |
| 0.59% | `python` | `list_iter` | list |
| 0.56% | `python` | `PyIter_Next` | dynamic |
| 0.54% | `python` | `set_merge_lock_held.part.0` | miscobj |
| 0.53% | `python` | `visit_reachable` | gc |
| 0.52% | `python` | `PyMem_Malloc` | memory |

## mypy2

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 28.83% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.64% | `python` | `gc_collect_main` | gc |
| 6.67% | `python` | `deduce_unreachable` | unknown |
| 4.00% | `[JIT]` | `jit` | jit |
| 2.77% | `python` | `visit_decref` | gc |
| 2.67% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.66% | `python` | `PyDict_GetItemRef` | dict |
| 1.53% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.49% | `python` | `subtype_traverse` | gc |
| 1.35% | `python` | `object_isinstance` | dynamic |
| 1.31% | `python` | `visit_reachable` | gc |
| 1.27% | `_json.cpython-313-x86_64-linux-gnu.so` | `_parse_object_unicode` | library |
| 1.23% | `python` | `_PySuper_Lookup` | dynamic |
| 1.04% | `python` | `list_dealloc` | memory |
| 0.98% | `python` | `subtype_dealloc` | memory |
| 0.98% | `python` | `PyObject_SetAttr` | dynamic |
| 0.96% | `python` | `clear_slots` | unknown |
| 0.95% | `python` | `PyUnicode_Substring` | str |
| 0.92% | `python` | `siphash13` | str |
| 0.84% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.82% | `python` | `tupledealloc` | memory |
| 0.82% | `python` | `dict_dealloc` | memory |
| 0.81% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.80% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.74% | `python` | `slot_tp_init` | unknown |
| 0.72% | `python` | `PyObject_GC_Del` | gc |
| 0.69% | `python` | `unicode_dealloc` | memory |
| 0.64% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.64% | `python` | `object_new` | memory |
| 0.63% | `python` | `PyDict_SetItem` | dict |
| 0.55% | `python` | `list_traverse` | gc |

## nbody

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 61.77% | `[JIT]` | `jit` | jit |
| 5.97% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.44% | `libm-2.31.so` | `f64xsubf128` | library |
| 4.29% | `python` | `PyFloat_FromDouble` | float |
| 2.64% | `python` | `float_dealloc` | memory |
| 1.34% | `python` | `float_pow` | float |
| 1.32% | `python` | `_Py_Dealloc` | memory |
| 0.66% | `python` | `type_new` | memory |
| 0.54% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.50% | `python` | `gc_collect_main` | gc |

## nqueens

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.83% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 20.43% | `[JIT]` | `jit` | jit |
| 4.35% | `python` | `set_vectorcall` | miscobj |
| 2.77% | `python` | `list_dealloc` | memory |
| 2.25% | `python` | `PyFunction_NewWithQualName` | memory |
| 2.00% | `python` | `set_dealloc` | memory |
| 1.97% | `python` | `gen_iternext` | unknown |
| 1.78% | `python` | `func_dealloc` | memory |
| 1.71% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.36% | `python` | `uop_optimize` | unknown |
| 1.30% | `python` | `_PyLong_Add` | int |
| 1.21% | `python` | `PyList_New` | memory |
| 1.19% | `python` | `list_subscript` | list |
| 1.13% | `python` | `tupledealloc` | memory |
| 1.11% | `python` | `gen_dealloc` | memory |
| 1.07% | `python` | `_PyBuildSlice_ConsumeRefs` | miscobj |
| 1.06% | `python` | `make_gen` | unknown |
| 0.94% | `python` | `PySlice_Unpack` | miscobj |
| 0.90% | `python` | `PyMem_Malloc` | memory |
| 0.78% | `python` | `type_new` | memory |
| 0.71% | `python` | `list_ass_slice_lock_held` | list |
| 0.70% | `python` | `PyLong_FromLong` | int |
| 0.69% | `python` | `slice_dealloc` | memory |
| 0.61% | `python` | `PyObject_Free` | dynamic |
| 0.54% | `python` | `_PyLong_Subtract` | int |
| 0.52% | `python` | `gc_collect_main` | gc |
| 0.51% | `python` | `list_iter` | list |

## pathlib

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 14.97% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.16% | `[JIT]` | `jit` | jit |
| 2.18% | `python` | `long_dealloc` | memory |
| 1.91% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.42% | `[kernel.kallsyms]` | `__d_lookup_rcu` | kernel |
| 1.36% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.31% | `python` | `_PySuper_Lookup` | dynamic |
| 1.23% | `libpthread-2.31.so` | `__pthread_mutex_lock` | library |
| 1.21% | `python` | `k_mul` | int |
| 1.10% | `[kernel.kallsyms]` | `memset_erms` | kernel |
| 1.08% | `[kernel.kallsyms]` | `__ext4fs_dirhash` | kernel |
| 1.07% | `libpthread-2.31.so` | `pthread_mutex_unlock` | library |
| 1.05% | `[kernel.kallsyms]` | `ext4_htree_store_dirent` | kernel |
| 1.03% | `python` | `_PyLong_New` | memory |
| 1.00% | `python` | `path_converter` | unknown |
| 0.90% | `python` | `ScandirIterator_iternext` | unknown |
| 0.86% | `python` | `list_dealloc` | memory |
| 0.85% | `python` | `tupledealloc` | memory |
| 0.83% | `python` | `type_new` | memory |
| 0.83% | `python` | `PyUnicode_FSConverter` | str |
| 0.81% | `python` | `unicode_decode_utf8` | str |
| 0.81% | `python` | `PyLong_FromLong` | int |
| 0.76% | `[kernel.kallsyms]` | `filldir64` | kernel |
| 0.74% | `python` | `_Py_dict_lookup` | lookup |
| 0.74% | `[kernel.kallsyms]` | `strncpy_from_user` | kernel |
| 0.72% | `python` | `x_add` | int |
| 0.71% | `python` | `_Py_type_getattro` | lookup |
| 0.70% | `python` | `_sre_SRE_Pattern_match` | library |
| 0.67% | `python` | `PyEval_RestoreThread` | interpreter |
| 0.65% | `python` | `tp_new_wrapper` | memory |
| 0.65% | `python` | `vectorcall_method` | calls |
| 0.64% | `python` | `slot_tp_init` | unknown |
| 0.64% | `python` | `PyObject_GC_Del` | gc |
| 0.63% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.62% | `python` | `PyUnicode_DecodeFSDefault` | str |
| 0.61% | `python` | `sre_ucs1_match` | library |
| 0.61% | `python` | `method_dealloc` | memory |
| 0.59% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.58% | `python` | `unicode_dealloc` | memory |
| 0.57% | `[kernel.kallsyms]` | `link_path_walk.part.0` | kernel |
| 0.56% | `python` | `gc_collect_main` | gc |
| 0.55% | `python` | `visit_decref` | gc |
| 0.55% | `python` | `deduce_unreachable` | unknown |
| 0.54% | `python` | `_PyUnicode_JoinArray` | str |
| 0.52% | `python` | `structseq_dealloc` | memory |
| 0.51% | `[kernel.kallsyms]` | `kmem_cache_alloc` | kernel |
| 0.51% | `python` | `PyList_New` | memory |
| 0.50% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |

## pickle

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.25% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `save` | library |
| 12.75% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_put.isra.0` | library |
| 6.80% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_write_bytes` | library |
| 4.11% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.04% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.67% | `python` | `PyDict_Next` | dict |
| 2.67% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_get.isra.0` | library |
| 2.49% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pickler_dealloc` | library |
| 1.82% | `python` | `PyUnicode_AsUTF8AndSize` | str |
| 1.63% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.42% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_Write` | library |
| 1.16% | `[JIT]` | `jit` | jit |
| 1.05% | `python` | `type_new` | memory |
| 0.73% | `python` | `deduce_unreachable` | unknown |
| 0.69% | `python` | `gc_collect_main` | gc |
| 0.61% | `python` | `visit_decref` | gc |
| 0.58% | `python` | `PyMem_Malloc` | memory |
| 0.53% | `python` | `PyMem_Free` | memory |
| 0.51% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.51% | `python` | `_PyCode_New` | memory |
| 0.51% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_pickle_dumps` | library |
| 0.50% | `python` | `visit_reachable` | gc |

## pickle_dict

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 45.94% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `save` | library |
| 12.42% | `python` | `PyDict_Next` | dict |
| 10.51% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_Write` | library |
| 3.04% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.93% | `python` | `PyLong_AsLongAndOverflow` | int |
| 2.88% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_put.isra.0` | library |
| 1.13% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.73% | `python` | `type_new` | memory |
| 0.69% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005cd4` | library |
| 0.65% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pickler_dealloc` | library |
| 0.65% | `[JIT]` | `jit` | jit |
| 0.58% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005e54` | library |
| 0.52% | `python` | `gc_collect_main` | gc |

## pickle_list

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 39.29% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `save` | library |
| 12.72% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `_Pickler_Write` | library |
| 4.92% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `memo_put.isra.0` | library |
| 4.60% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.95% | `python` | `PyLong_AsLongAndOverflow` | int |
| 2.18% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.44% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.17% | `[JIT]` | `jit` | jit |
| 1.11% | `python` | `type_new` | memory |
| 1.07% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pickler_dealloc` | library |
| 0.74% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005cd4` | library |
| 0.74% | `python` | `gc_collect_main` | gc |
| 0.72% | `python` | `PyList_Size` | list |
| 0.71% | `python` | `deduce_unreachable` | unknown |
| 0.66% | `python` | `visit_decref` | gc |
| 0.56% | `python` | `PyMem_Free` | memory |
| 0.54% | `python` | `_PyCode_New` | memory |
| 0.52% | `python` | `visit_reachable` | gc |
| 0.50% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005fc4` | library |

## pickle_pure_python

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 47.08% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.64% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.70% | `python` | `bytes_concat` | str |
| 2.46% | `python` | `dict_get` | dict |
| 2.18% | `python` | `unicode_encode` | str |
| 1.84% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.65% | `python` | `PyObject_Free` | dynamic |
| 1.63% | `[JIT]` | `jit` | jit |
| 1.55% | `python` | `insertdict` | dict |
| 1.37% | `python` | `long_dealloc` | memory |
| 1.35% | `python` | `_PyLong_New` | memory |
| 1.20% | `python` | `PyDict_GetItemRef` | dict |
| 1.09% | `python` | `write_bytes` | unknown |
| 1.03% | `python` | `unicode_encode_utf8` | str |
| 0.96% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.96% | `python` | `tupledealloc` | memory |
| 0.90% | `python` | `PyType_GetModuleByDef` | dynamic |
| 0.82% | `python` | `PyDict_Contains` | dict |
| 0.69% | `python` | `PySys_Audit` | unknown |
| 0.68% | `python` | `type_new` | memory |
| 0.64% | `python` | `long_hash` | int |
| 0.55% | `python` | `builtin_id` | unknown |
| 0.53% | `_struct.cpython-313-x86_64-linux-gnu.so` | `s_pack` | library |

## pidigits

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 33.08% | `python` | `x_divrem` | int |
| 19.79% | `python` | `k_mul` | int |
| 12.32% | `python` | `x_add` | int |
| 7.90% | `python` | `x_sub` | int |
| 3.18% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.62% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.90% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.77% | `[JIT]` | `jit` | jit |
| 0.68% | `python` | `type_new` | memory |

## pprint

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 22.57% | `[JIT]` | `jit` | jit |
| 19.49% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.42% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.36% | `python` | `long_to_decimal_string` | int |
| 2.90% | `python` | `_Py_type_getattro_impl` | dynamic |
| 2.44% | `python` | `_Py_type_getattro` | lookup |
| 2.42% | `python` | `tupledealloc` | memory |
| 2.25% | `python` | `PyUnicode_Format` | str |
| 2.04% | `python` | `_PyUnicode_JoinArray` | str |
| 1.62% | `python` | `unicode_dealloc` | memory |
| 1.57% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.28% | `python` | `_Py_dict_lookup` | lookup |
| 1.19% | `python` | `_PyUnicodeWriter_PrepareInternal` | str |
| 1.17% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.00% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.98% | `python` | `_PyDict_SetItem_Take2` | dict |
| 0.95% | `python` | `_PyObject_Malloc` | memory |
| 0.92% | `python` | `list_dealloc` | memory |
| 0.91% | `python` | `meth_dealloc` | memory |
| 0.87% | `python` | `slot_tp_init` | unknown |
| 0.86% | `python` | `_PySet_Contains` | unknown |
| 0.84% | `python` | `PyDict_Contains` | dict |
| 0.83% | `python` | `builtin_issubclass` | unknown |
| 0.77% | `python` | `slot_tp_richcompare` | dynamic |
| 0.72% | `python` | `_PyLong_New` | memory |
| 0.71% | `python` | `list_sort_impl` | list |
| 0.71% | `python` | `PyObject_GC_Del` | gc |
| 0.67% | `python` | `object_new` | memory |
| 0.63% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.61% | `python` | `PyObject_GetAttr` | dynamic |
| 0.60% | `python` | `builtin_getattr` | lookup |
| 0.57% | `python` | `list_append` | list |
| 0.55% | `python` | `long_hash` | int |
| 0.54% | `python` | `method_get` | dynamic |
| 0.53% | `python` | `set_contains_lock_held` | miscobj |
| 0.52% | `python` | `_PyList_FromArraySteal` | list |

## pycparser

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 25.83% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 14.35% | `python` | `sre_ucs1_match` | library |
| 8.77% | `[JIT]` | `jit` | jit |
| 2.82% | `python` | `_sre_SRE_Pattern_match` | library |
| 2.58% | `python` | `PyDict_GetItemRef` | dict |
| 2.47% | `python` | `gc_collect_main` | gc |
| 2.39% | `python` | `deduce_unreachable` | unknown |
| 2.34% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 2.20% | `python` | `object_new` | memory |
| 1.64% | `python` | `dict_get` | dict |
| 1.50% | `python` | `subtype_dealloc` | memory |
| 1.43% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.32% | `python` | `visit_decref` | gc |
| 1.20% | `python` | `subtype_traverse` | gc |
| 1.19% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.16% | `python` | `visit_reachable` | gc |
| 0.96% | `python` | `list_ass_slice_lock_held` | list |
| 0.88% | `python` | `list_dealloc` | memory |
| 0.84% | `python` | `object_isinstance` | dynamic |
| 0.78% | `python` | `slot_mp_ass_subscript` | unknown |
| 0.78% | `python` | `sre_ucs1_count` | library |
| 0.65% | `python` | `PyObject_GC_Del` | gc |
| 0.61% | `python` | `PyDict_Contains` | dict |
| 0.58% | `python` | `list_subscript` | list |
| 0.51% | `python` | `PySlice_Unpack` | miscobj |

## pyflate

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 35.35% | `[JIT]` | `jit` | jit |
| 8.60% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.24% | `python` | `list_dealloc` | memory |
| 4.03% | `python` | `list_ass_slice_lock_held` | list |
| 2.62% | `python` | `list_subscript` | list |
| 2.48% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 2.42% | `python` | `long_dealloc` | memory |
| 2.41% | `python` | `bytes_subscript` | str |
| 2.02% | `python` | `_PyLong_Add` | int |
| 1.97% | `python` | `list_concat` | list |
| 1.70% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.69% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.40% | `python` | `_PyLong_Subtract` | int |
| 1.31% | `python` | `long_lshift` | int |
| 1.24% | `python` | `stringlib_bytes_join.lto_priv.1` | str |
| 1.15% | `python` | `PySlice_Unpack` | miscobj |
| 1.07% | `python` | `_PyLong_New` | memory |
| 0.94% | `python` | `PyObject_Free` | dynamic |
| 0.85% | `python` | `list_sort_impl` | list |
| 0.63% | `python` | `long_rshift` | int |
| 0.62% | `python` | `unsafe_long_compare` | unknown |
| 0.60% | `python` | `PyObject_GetItem` | dynamic |
| 0.54% | `python` | `long_and` | int |

## pylint

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 23.79% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.97% | `python` | `gc_collect_main` | gc |
| 5.39% | `python` | `deduce_unreachable` | unknown |
| 3.57% | `[JIT]` | `jit` | jit |
| 3.52% | `python` | `visit_decref` | gc |
| 2.85% | `python` | `visit_reachable` | gc |
| 1.99% | `python` | `subtype_traverse` | gc |
| 1.87% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.79% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.67% | `python` | `PyDict_GetItemRef` | dict |
| 1.40% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.14% | `python` | `find_name_in_mro` | lookup |
| 1.02% | `python` | `_PyObject_GetMethod` | dynamic |
| 0.99% | `python` | `object_isinstance` | dynamic |
| 0.97% | `python` | `tupledealloc` | memory |
| 0.84% | `python` | `dict_traverse` | gc |
| 0.80% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.74% | `python` | `dict_dealloc` | memory |
| 0.72% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.69% | `python` | `PyObject_SetAttr` | dynamic |
| 0.66% | `python` | `list_traverse` | gc |
| 0.61% | `python` | `list_dealloc` | memory |
| 0.60% | `python` | `type_new` | memory |
| 0.60% | `python` | `gen_dealloc` | memory |
| 0.53% | `python` | `subtype_dealloc` | memory |
| 0.52% | `python` | `PyObject_GetAttr` | dynamic |
| 0.52% | `python` | `make_gen` | unknown |

## python_startup

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 7.59% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.35% | `python` | `type_new` | memory |
| 3.98% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.65% | `python` | `visit_decref` | gc |
| 2.14% | `python` | `_PyCode_New` | memory |
| 2.06% | `python` | `gc_collect_main` | gc |
| 2.03% | `python` | `deduce_unreachable` | unknown |
| 1.81% | `ld-2.31.so` | `_dl_rtld_di_serinfo` | library |
| 1.76% | `python` | `r_object` | import |
| 1.66% | `python` | `visit_reachable` | gc |
| 1.43% | `python` | `PyUnicode_FromKindAndData` | str |
| 1.42% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 1.17% | `python` | `siphash13` | str |
| 1.09% | `[kernel.kallsyms]` | `perf_iterate_ctx` | kernel |
| 1.05% | `python` | `_Py_hashtable_get` | unknown |
| 1.04% | `python` | `unicode_decode_utf8` | str |
| 1.03% | `[kernel.kallsyms]` | `native_irq_return_iret` | kernel |
| 0.97% | `python` | `tupledealloc` | memory |
| 0.88% | `python` | `type_ready` | dynamic |
| 0.83% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.82% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.81% | `[kernel.kallsyms]` | `sync_regs` | kernel |
| 0.77% | `python` | `dict_traverse` | gc |
| 0.75% | `python` | `PyDict_SetItem` | dict |
| 0.74% | `python` | `find_name_in_mro` | lookup |
| 0.62% | `python` | `_Py_dict_lookup` | lookup |
| 0.61% | `python` | `dictresize` | dict |
| 0.60% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.58% | `python` | `insertdict` | dict |
| 0.56% | `python` | `unicode_dealloc` | memory |
| 0.55% | `[kernel.kallsyms]` | `zap_pte_range.isra.0` | kernel |
| 0.54% | `[kernel.kallsyms]` | `_raw_spin_lock` | kernel |
| 0.54% | `[kernel.kallsyms]` | `filemap_map_pages` | kernel |

## python_startup_no_site

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 6.54% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.85% | `python` | `type_new` | memory |
| 4.05% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.51% | `python` | `visit_decref` | gc |
| 2.30% | `python` | `gc_collect_main` | gc |
| 2.23% | `python` | `_PyCode_New` | memory |
| 2.08% | `python` | `deduce_unreachable` | unknown |
| 1.92% | `python` | `r_object` | import |
| 1.86% | `ld-2.31.so` | `_dl_rtld_di_serinfo` | library |
| 1.57% | `python` | `visit_reachable` | gc |
| 1.48% | `python` | `PyUnicode_FromKindAndData` | str |
| 1.39% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 1.32% | `[kernel.kallsyms]` | `native_irq_return_iret` | kernel |
| 1.24% | `python` | `siphash13` | str |
| 1.22% | `[kernel.kallsyms]` | `perf_iterate_ctx` | kernel |
| 1.07% | `python` | `_Py_hashtable_get` | unknown |
| 0.98% | `python` | `unicode_decode_utf8` | str |
| 0.92% | `[kernel.kallsyms]` | `sync_regs` | kernel |
| 0.89% | `[kernel.kallsyms]` | `clear_page_erms` | kernel |
| 0.87% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.85% | `python` | `type_ready` | dynamic |
| 0.84% | `python` | `tupledealloc` | memory |
| 0.81% | `python` | `dict_traverse` | gc |
| 0.77% | `python` | `PyDict_SetItem` | dict |
| 0.75% | `python` | `find_name_in_mro` | lookup |
| 0.73% | `[kernel.kallsyms]` | `filemap_map_pages` | kernel |
| 0.67% | `python` | `insertdict` | dict |
| 0.65% | `[kernel.kallsyms]` | `_raw_spin_lock` | kernel |
| 0.61% | `[kernel.kallsyms]` | `zap_pte_range.isra.0` | kernel |
| 0.60% | `python` | `dictresize` | dict |
| 0.53% | `libc-2.31.so` | `wcsrtombs` | libc |
| 0.53% | `python` | `_Py_dict_lookup` | lookup |
| 0.52% | `[kernel.kallsyms]` | `native_flush_tlb_one_user` | kernel |

## raytrace

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 36.38% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 20.71% | `[JIT]` | `jit` | jit |
| 5.47% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.52% | `python` | `subtype_dealloc` | memory |
| 1.83% | `python` | `PyFloat_FromDouble` | float |
| 1.62% | `python` | `PyType_GenericAlloc` | memory |
| 1.62% | `python` | `vectorcall_maybe.constprop.0` | unknown |
| 1.45% | `python` | `float_dealloc` | memory |
| 1.12% | `python` | `_PyObject_InitInlineValues` | dynamic |
| 1.11% | `python` | `PyNumber_Subtract` | dynamic |
| 1.04% | `python` | `PyObject_GC_Del` | gc |
| 0.99% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.71% | `python` | `float_mul` | float |
| 0.70% | `python` | `tupledealloc` | memory |
| 0.69% | `python` | `convert_to_double` | unknown |
| 0.63% | `python` | `float_add` | float |
| 0.61% | `python` | `float_sub` | float |
| 0.58% | `python` | `PyNumber_Multiply` | dynamic |
| 0.55% | `python` | `float_richcompare` | float |

## regex_compile

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 26.06% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 17.06% | `[JIT]` | `jit` | jit |
| 3.92% | `python` | `sre_ucs1_match` | library |
| 2.56% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.58% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.54% | `python` | `PyNumber_AsSsize_t` | dynamic |
| 1.09% | `python` | `PyLong_FromLong` | int |
| 1.02% | `python` | `tupledealloc` | memory |
| 1.01% | `python` | `list_dealloc` | memory |
| 0.97% | `python` | `sre_ucs2_charset.isra.0` | library |
| 0.94% | `python` | `long_dealloc` | memory |
| 0.94% | `python` | `object_isinstance` | dynamic |
| 0.77% | `python` | `bytearray_ass_subscript` | miscobj |
| 0.75% | `python` | `type_new` | memory |
| 0.67% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.56% | `python` | `gc_collect_main` | gc |
| 0.56% | `python` | `slot_mp_subscript` | unknown |
| 0.54% | `python` | `deduce_unreachable` | unknown |
| 0.54% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.51% | `python` | `sre_search` | library |

## regex_dna

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 32.94% | `python` | `sre_ucs1_match` | library |
| 28.18% | `python` | `sre_ucs2_charset.isra.0` | library |
| 6.82% | `python` | `sre_search` | library |
| 4.47% | `[JIT]` | `jit` | jit |
| 2.92% | `libm-2.31.so` | `__fmod_finite` | library |
| 2.44% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 1.21% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.02% | `_bisect.cpython-313-x86_64-linux-gnu.so` | `_bisect_bisect_right` | library |
| 0.99% | `python` | `pattern_subx` | library |
| 0.91% | `python` | `float_richcompare` | float |
| 0.65% | `python` | `stringlib_bytes_join.lto_priv.1` | str |
| 0.58% | `python` | `PyFloat_FromDouble` | float |
| 0.54% | `python` | `type_new` | memory |

## regex_effbot

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 37.09% | `python` | `sre_ucs1_match` | library |
| 16.07% | `python` | `sre_ucs2_charset.isra.0` | library |
| 9.05% | `python` | `PyMem_Free` | memory |
| 6.22% | `python` | `sre_search` | library |
| 4.15% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.88% | `python` | `PyMem_Malloc` | memory |
| 1.86% | `python` | `sre_ucs1_count` | library |
| 0.86% | `python` | `type_new` | memory |
| 0.74% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.68% | `[JIT]` | `jit` | jit |
| 0.59% | `python` | `gc_collect_main` | gc |
| 0.55% | `python` | `visit_decref` | gc |
| 0.52% | `python` | `deduce_unreachable` | unknown |

## regex_v8

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 31.71% | `python` | `sre_ucs1_match` | library |
| 7.94% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.28% | `python` | `sre_ucs1_count` | library |
| 3.42% | `python` | `sre_search` | library |
| 3.37% | `python` | `PyCode_Addr2Line` | exceptions |
| 2.63% | `[JIT]` | `jit` | jit |
| 1.81% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 1.61% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.26% | `python` | `pattern_subx` | library |
| 1.14% | `python` | `sre_ucs1_match.cold` | library |
| 1.06% | `python` | `type_new` | memory |
| 0.99% | `python` | `state_init` | unknown |
| 0.98% | `python` | `PyMem_Free` | memory |
| 0.77% | `python` | `gc_collect_main` | gc |
| 0.73% | `python` | `visit_decref` | gc |
| 0.71% | `python` | `deduce_unreachable` | unknown |
| 0.68% | `python` | `PyUnicode_Substring` | str |
| 0.62% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 0.59% | `python` | `list_dealloc` | memory |
| 0.59% | `python` | `_PyUnicode_JoinArray` | str |
| 0.57% | `python` | `PyDict_GetItemRef` | dict |
| 0.56% | `python` | `tupledealloc` | memory |
| 0.55% | `python` | `PyLong_FromLong` | int |
| 0.55% | `libc-2.31.so` | `malloc` | libc |
| 0.55% | `python` | `PyMem_Malloc` | memory |
| 0.53% | `python` | `_PyUnicode_IsAlpha` | str |
| 0.52% | `python` | `_PyCode_New` | memory |
| 0.52% | `python` | `long_dealloc` | memory |
| 0.51% | `python` | `unicode_dealloc` | memory |

## richards

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 38.61% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 21.39% | `[JIT]` | `jit` | jit |
| 4.86% | `python` | `_PyObject_GetMethod` | dynamic |
| 4.41% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 4.30% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 3.40% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 2.23% | `python` | `PyObject_GetAttr` | dynamic |
| 1.21% | `python` | `PyObject_SetAttr` | dynamic |
| 0.84% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.76% | `python` | `long_dealloc` | memory |
| 0.75% | `python` | `type_new` | memory |
| 0.60% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.52% | `python` | `_PyLong_Add` | int |
| 0.51% | `python` | `gc_collect_main` | gc |

## richards_super

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 35.81% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 16.93% | `[JIT]` | `jit` | jit |
| 4.17% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 3.69% | `python` | `_PyObject_GetMethod` | dynamic |
| 3.37% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 2.70% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 2.36% | `python` | `_PySuper_Lookup` | dynamic |
| 1.76% | `python` | `PyObject_SetAttr` | dynamic |
| 1.72% | `python` | `PyObject_GetAttr` | dynamic |
| 1.12% | `python` | `type_new` | memory |
| 1.06% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.73% | `python` | `gc_collect_main` | gc |
| 0.71% | `python` | `deduce_unreachable` | unknown |
| 0.70% | `python` | `visit_decref` | gc |
| 0.63% | `python` | `long_dealloc` | memory |
| 0.53% | `python` | `visit_reachable` | gc |
| 0.51% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.51% | `python` | `_PyCode_New` | memory |

## scimark

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 24.98% | `[JIT]` | `jit` | jit |
| 13.82% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.26% | `python` | `PyNumber_AsSsize_t` | dynamic |
| 4.25% | `python` | `long_dealloc` | memory |
| 3.39% | `array.cpython-313-x86_64-linux-gnu.so` | `array_subscr` | library |
| 2.87% | `python` | `_PyLong_Add` | int |
| 2.53% | `python` | `PyFloat_FromDouble` | float |
| 2.49% | `python` | `PyObject_GetItem` | dynamic |
| 2.24% | `python` | `slot_mp_subscript` | unknown |
| 2.22% | `python` | `PyType_GetModuleByDef` | dynamic |
| 2.09% | `python` | `vgetargs1_impl` | calls |
| 2.04% | `python` | `PyLong_FromLong` | int |
| 1.61% | `python` | `convertitem` | unknown |
| 1.47% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.40% | `array.cpython-313-x86_64-linux-gnu.so` | `array_ass_subscr` | library |
| 1.19% | `python` | `object_isinstance` | dynamic |
| 1.15% | `python` | `_PyLong_Multiply` | int |
| 1.01% | `python` | `float_dealloc` | memory |
| 0.91% | `python` | `PyObject_Free` | dynamic |
| 0.83% | `python` | `PyIndex_Check` | unknown |
| 0.82% | `array.cpython-313-x86_64-linux-gnu.so` | `d_setitem` | library |
| 0.81% | `python` | `PyArg_Parse` | calls |
| 0.64% | `python` | `_Py_Dealloc` | memory |
| 0.63% | `python` | `PyObject_SetItem` | dynamic |
| 0.61% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.56% | `python` | `tupledealloc` | memory |
| 0.54% | `python` | `_PyFloat_ExactDealloc` | memory |

## spectral_norm

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 28.64% | `[JIT]` | `jit` | jit |
| 9.31% | `python` | `_PyLong_Add` | int |
| 4.94% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.43% | `python` | `long_dealloc` | memory |
| 4.26% | `python` | `long_div` | int |
| 4.12% | `python` | `_PyLong_Multiply` | int |
| 3.85% | `python` | `PyObject_Free` | dynamic |
| 3.59% | `python` | `enum_next` | miscobj |
| 3.30% | `python` | `float_div` | float |
| 2.29% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.78% | `python` | `convert_to_double` | unknown |
| 1.56% | `python` | `PyNumber_TrueDivide` | dynamic |
| 1.00% | `python` | `type_new` | memory |
| 0.97% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.80% | `python` | `PyNumber_Multiply` | dynamic |
| 0.79% | `python` | `PyNumber_FloorDivide` | dynamic |
| 0.76% | `python` | `float_dealloc` | memory |
| 0.74% | `python` | `float_mul` | float |
| 0.73% | `python` | `deduce_unreachable` | unknown |
| 0.72% | `python` | `gc_collect_main` | gc |
| 0.69% | `python` | `visit_decref` | gc |

## sqlglot

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 30.52% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.77% | `python` | `object_isinstance` | dynamic |
| 3.14% | `[JIT]` | `jit` | jit |
| 2.24% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.20% | `python` | `tupledealloc` | memory |
| 1.83% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.53% | `python` | `type_new` | memory |
| 1.30% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 1.28% | `python` | `meth_dealloc` | memory |
| 1.26% | `python` | `dictiter_iternextitem` | dict |
| 1.19% | `python` | `method_get` | dynamic |
| 0.96% | `python` | `gc_collect_main` | gc |
| 0.94% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.93% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.90% | `python` | `PyObject_IsInstance` | dynamic |
| 0.88% | `python` | `make_gen` | unknown |
| 0.88% | `python` | `visit_decref` | gc |
| 0.87% | `python` | `deduce_unreachable` | unknown |
| 0.85% | `python` | `dictiter_dealloc` | memory |
| 0.85% | `python` | `gen_dealloc` | memory |
| 0.71% | `python` | `list_dealloc` | memory |
| 0.70% | `python` | `insert_to_emptydict` | dict |
| 0.67% | `python` | `dict_items` | dict |
| 0.66% | `python` | `PyObject_GC_Del` | gc |
| 0.65% | `python` | `PyList_New` | memory |
| 0.63% | `python` | `getset_get` | dynamic |
| 0.61% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.60% | `python` | `dictview_dealloc` | memory |
| 0.60% | `python` | `_PyCode_New` | memory |
| 0.59% | `python` | `visit_reachable` | gc |
| 0.57% | `python` | `unicode_dealloc` | memory |
| 0.57% | `python` | `slot_tp_hash` | unknown |
| 0.56% | `python` | `dictitems_iter` | unknown |
| 0.56% | `python` | `siphash13` | str |
| 0.53% | `python` | `func_dealloc` | memory |
| 0.51% | `python` | `dict_setdefault_ref_lock_held` | dict |

## sqlglot_optimize

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 26.16% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.75% | `[JIT]` | `jit` | jit |
| 5.09% | `python` | `object_isinstance` | dynamic |
| 2.18% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.98% | `python` | `tupledealloc` | memory |
| 1.63% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.45% | `python` | `type_new` | memory |
| 1.44% | `python` | `meth_dealloc` | memory |
| 1.35% | `python` | `dictiter_iternextitem` | dict |
| 1.31% | `python` | `method_get` | dynamic |
| 1.27% | `python` | `_PyObject_LookupSpecial` | dynamic |
| 1.07% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.99% | `python` | `gc_collect_main` | gc |
| 0.97% | `python` | `deduce_unreachable` | unknown |
| 0.91% | `python` | `PyObject_IsInstance` | dynamic |
| 0.90% | `python` | `list_dealloc` | memory |
| 0.90% | `python` | `visit_decref` | gc |
| 0.79% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.78% | `python` | `PyList_New` | memory |
| 0.77% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.68% | `python` | `getset_get` | dynamic |
| 0.66% | `python` | `dictiter_dealloc` | memory |
| 0.65% | `python` | `PyObject_GC_Del` | gc |
| 0.63% | `python` | `visit_reachable` | gc |
| 0.62% | `python` | `dict_get` | dict |
| 0.58% | `python` | `_PyCode_New` | memory |
| 0.57% | `python` | `_Py_dict_lookup` | lookup |
| 0.55% | `python` | `siphash13` | str |
| 0.55% | `python` | `list_iter` | list |
| 0.53% | `python` | `member_get` | unknown |
| 0.53% | `python` | `slot_tp_hash` | unknown |
| 0.52% | `python` | `unicode_dealloc` | memory |
| 0.52% | `python` | `dict_items` | dict |
| 0.51% | `python` | `tuplehash` | tuple |

## sqlglot_parse

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 40.36% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 7.90% | `[JIT]` | `jit` | jit |
| 2.96% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.39% | `python` | `_Py_type_getattro` | lookup |
| 1.37% | `python` | `PyDict_Contains` | dict |
| 1.31% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.20% | `python` | `deduce_unreachable` | unknown |
| 1.18% | `python` | `gc_collect_main` | gc |
| 1.07% | `python` | `visit_decref` | gc |
| 1.06% | `python` | `type_new` | memory |
| 0.89% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.81% | `python` | `PyObject_GetAttr` | dynamic |
| 0.80% | `python` | `long_dealloc` | memory |
| 0.79% | `python` | `dict_get` | dict |
| 0.76% | `python` | `slot_tp_hash` | unknown |
| 0.75% | `python` | `tupledealloc` | memory |
| 0.73% | `python` | `PyObject_RichCompare` | dynamic |
| 0.72% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.72% | `python` | `_PyLong_Add` | int |
| 0.64% | `python` | `object_isinstance` | dynamic |
| 0.64% | `python` | `dict_dealloc` | memory |
| 0.61% | `python` | `visit_reachable` | gc |
| 0.60% | `python` | `PyObject_SetAttr` | dynamic |
| 0.59% | `python` | `object_new` | memory |
| 0.57% | `python` | `find_name_in_mro` | lookup |
| 0.54% | `python` | `subtype_traverse` | gc |
| 0.53% | `python` | `PyDict_SetItem` | dict |
| 0.52% | `python` | `unicode_dealloc` | memory |

## sqlglot_transpile

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 35.84% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 6.35% | `[JIT]` | `jit` | jit |
| 2.79% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.63% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.59% | `python` | `type_new` | memory |
| 1.35% | `python` | `gc_collect_main` | gc |
| 1.31% | `python` | `deduce_unreachable` | unknown |
| 1.20% | `python` | `visit_decref` | gc |
| 1.09% | `python` | `_Py_type_getattro` | lookup |
| 1.08% | `python` | `find_name_in_mro` | lookup |
| 1.06% | `python` | `dict_get` | dict |
| 1.00% | `python` | `PyDict_Contains` | dict |
| 0.95% | `python` | `object_isinstance` | dynamic |
| 0.92% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.83% | `python` | `tupledealloc` | memory |
| 0.77% | `python` | `visit_reachable` | gc |
| 0.76% | `python` | `PyObject_GetAttr` | dynamic |
| 0.70% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.64% | `python` | `long_dealloc` | memory |
| 0.63% | `python` | `unicode_dealloc` | memory |
| 0.62% | `python` | `dict_dealloc` | memory |
| 0.58% | `python` | `_PyCode_New` | memory |
| 0.57% | `python` | `PyObject_RichCompare` | dynamic |
| 0.54% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.54% | `python` | `_PyLong_Add` | int |

## sqlite_synth

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 11.59% | `libpthread-2.31.so` | `__pthread_mutex_lock` | library |
| 11.48% | `libpthread-2.31.so` | `pthread_mutex_unlock` | library |
| 5.42% | `python` | `PyEval_RestoreThread` | interpreter |
| 5.08% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.43% | `libsqlite3.so.0.8.6` | `sqlite3_reset` | library |
| 3.04% | `[JIT]` | `jit` | jit |
| 2.35% | `libm-2.31.so` | `f64xsubf128` | library |
| 1.34% | `python` | `PyEval_SaveThread` | interpreter |
| 1.33% | `libsqlite3.so.0.8.6` | `sqlite3_randomness` | library |
| 1.26% | `python` | `PyTuple_New` | memory |
| 1.26% | `libc-2.31.so` | `pthread_cond_signal` | libc |
| 1.24% | `python` | `long_dealloc` | memory |
| 1.09% | `python` | `tupledealloc` | memory |
| 1.03% | `python` | `long_to_decimal_string_internal` | int |
| 1.02% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.99% | `_sqlite3.cpython-313-x86_64-linux-gnu.so` | `_pysqlite_query_execute` | library |
| 0.91% | `libsqlite3.so.0.8.6` | `sqlite3_value_double` | library |
| 0.89% | `libpthread-2.31.so` | `pthread_cond_signal@@GLIBC_2.3.2` | library |
| 0.88% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.78% | `python` | `PyFloat_AsDouble` | float |
| 0.76% | `libsqlite3.so.0.8.6` | `sqlite3_preupdate_old` | library |
| 0.74% | `python` | `list_dealloc` | memory |
| 0.72% | `python` | `type_new` | memory |
| 0.65% | `libc-2.31.so` | `pthread_mutex_unlock` | libc |
| 0.64% | `libsqlite3.so.0.8.6` | `sqlite3_vtab_config` | library |
| 0.62% | `libsqlite3.so.0.8.6` | `sqlite3_enable_shared_cache` | library |
| 0.61% | `libsqlite3.so.0.8.6` | `sqlite3_value_int64` | library |
| 0.59% | `python` | `unicode_dealloc` | memory |
| 0.59% | `libsqlite3.so.0.8.6` | `sqlite3_wal_checkpoint` | library |
| 0.59% | `python` | `PyFloat_FromDouble` | float |
| 0.57% | `libc-2.31.so` | `pthread_mutex_lock` | libc |
| 0.56% | `libsqlite3.so.0.8.6` | `sqlite3_extended_errcode` | library |
| 0.54% | `python` | `unicode_decode_utf8` | str |
| 0.50% | `python` | `gc_collect_main` | gc |

## sympy

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 25.12% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.85% | `[JIT]` | `jit` | jit |
| 2.30% | `python` | `tupledealloc` | memory |
| 2.10% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.08% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.27% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.19% | `python` | `type_new` | memory |
| 1.15% | `python` | `gc_collect_main` | gc |
| 1.13% | `python` | `deduce_unreachable` | unknown |
| 1.12% | `python` | `_Py_dict_lookup` | lookup |
| 1.08% | `python` | `_Py_type_getattro` | lookup |
| 1.08% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.04% | `python` | `visit_decref` | gc |
| 1.00% | `python` | `PyDict_SetItem` | dict |
| 0.91% | `python` | `PyDict_GetItemRef` | dict |
| 0.86% | `python` | `find_name_in_mro` | lookup |
| 0.86% | `python` | `PyObject_RichCompare` | dynamic |
| 0.81% | `python` | `slot_tp_richcompare` | dynamic |
| 0.80% | `python` | `object_isinstance` | dynamic |
| 0.78% | `python` | `dict_dealloc` | memory |
| 0.76% | `python` | `PyObject_GetAttr` | dynamic |
| 0.76% | `python` | `_PyCode_New` | memory |
| 0.72% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.70% | `python` | `visit_reachable` | gc |
| 0.68% | `python` | `method_get` | dynamic |
| 0.66% | `python` | `list_dealloc` | memory |
| 0.66% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.66% | `python` | `meth_dealloc` | memory |
| 0.60% | `python` | `_PyObject_GenericGetAttrWithDict` | dynamic |
| 0.58% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.58% | `python` | `setiter_iternext` | miscobj |
| 0.55% | `python` | `r_object` | import |
| 0.53% | `python` | `_PyObject_MakeTpCall` | dynamic |

## telco

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 10.33% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.11% | `[JIT]` | `jit` | jit |
| 4.32% | `python` | `PyType_GetModuleByDef` | dynamic |
| 3.54% | `python` | `PyObject_GC_Del` | gc |
| 3.43% | `python` | `_PyObject_GC_New` | gc |
| 2.25% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `_mpd_qaddsub` | library |
| 1.89% | `python` | `tupledealloc` | memory |
| 1.89% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.82% | `python` | `PyContextVar_Get` | unknown |
| 1.82% | `python` | `PyTuple_New` | memory |
| 1.81% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `_mpd_baseshiftr` | library |
| 1.81% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `nm_mpd_qmul` | library |
| 1.79% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.70% | `python` | `meth_dealloc` | memory |
| 1.69% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `nm_mpd_qadd` | library |
| 1.64% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `convert_op` | library |
| 1.33% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `mpd_qshiftr` | library |
| 1.30% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `_mpd_qmul` | library |
| 1.28% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `mpd_qfinalize` | library |
| 1.25% | `python` | `method_get` | dynamic |
| 1.22% | `python` | `vgetargskeywords.constprop.0` | calls |
| 1.09% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_mpd_qquantize` | library |
| 1.06% | `python` | `_PyArg_UnpackKeywordsWithVararg` | calls |
| 0.90% | `python` | `type_new` | memory |
| 0.84% | `python` | `PyUnicode_New` | memory |
| 0.83% | `python` | `method_vectorcall_VARARGS_KEYWORDS` | calls |
| 0.82% | `python` | `PyDict_GetItemRef` | dict |
| 0.77% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_dealloc` | library |
| 0.74% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `dec_addstatus` | library |
| 0.74% | `python` | `_io_BytesIO_read` | unknown |
| 0.69% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `mpd_qquantize` | library |
| 0.65% | `_decimal.cpython-313-x86_64-linux-gnu.so` | `PyDecType_New` | library |
| 0.65% | `python` | `gc_collect_main` | gc |
| 0.65% | `python` | `as_ucs4` | unknown |
| 0.64% | `python` | `visit_decref` | gc |
| 0.64% | `python` | `vgetargs1_impl` | calls |
| 0.62% | `python` | `deduce_unreachable` | unknown |
| 0.56% | `python` | `unicode_dealloc` | memory |
| 0.55% | `_struct.cpython-313-x86_64-linux-gnu.so` | `unpack` | library |
| 0.54% | `python` | `find_keyword` | unknown |

## thrift

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 21.72% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.25% | `python` | `subtype_dealloc` | memory |
| 2.17% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::encodeValue` | library |
| 2.03% | `python` | `object_new` | memory |
| 2.00% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.00% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.83% | `python` | `_PyFunction_Vectorcall` | calls |
| 1.80% | `python` | `slot_tp_init` | unknown |
| 1.79% | `python` | `PyDict_GetItemRef` | dict |
| 1.73% | `python` | `insert_to_emptydict` | dict |
| 1.72% | `python` | `PyUnicode_FromFormatV` | str |
| 1.64% | `python` | `PyDict_SetItem` | dict |
| 1.51% | `python` | `dict_dealloc` | memory |
| 1.38% | `python` | `_PyStack_UnpackDict` | unknown |
| 1.36% | `[JIT]` | `jit` | jit |
| 1.25% | `python` | `tupledealloc` | memory |
| 1.23% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.17% | `python` | `type_new` | memory |
| 1.15% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 1.11% | `python` | `unicode_decode_utf8` | str |
| 1.11% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 1.07% | `python` | `PyObject_GC_Del` | gc |
| 0.91% | `python` | `insertdict` | dict |
| 0.85% | `python` | `_PySuper_Lookup` | dynamic |
| 0.82% | `python` | `list_dealloc` | memory |
| 0.79% | `python` | `PyObject_RichCompare` | dynamic |
| 0.78% | `python` | `gc_collect_main` | gc |
| 0.77% | `python` | `deduce_unreachable` | unknown |
| 0.74% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::decodeValue` | library |
| 0.70% | `python` | `unicode_dealloc` | memory |
| 0.67% | `python` | `PyMem_Free` | memory |
| 0.66% | `python` | `visit_decref` | gc |
| 0.62% | `python` | `PyLong_AsLong` | int |
| 0.60% | `python` | `_Py_type_getattro` | lookup |
| 0.59% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readStruct` | library |
| 0.59% | `python` | `PyObject_GetOptionalAttr` | dynamic |
| 0.57% | `python` | `_Py_dict_lookup` | lookup |
| 0.57% | `python` | `PyTuple_Size` | tuple |
| 0.56% | `python` | `dictresize` | dict |
| 0.53% | `fastbinary.cpython-313-x86_64-linux-gnu.so` | `apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readBytes` | library |
| 0.52% | `python` | `PyUnicode_RichCompare` | str |
| 0.52% | `python` | `PyObject_GetAttr` | dynamic |
| 0.52% | `python` | `visit_reachable` | gc |
| 0.52% | `python` | `unicodekeys_lookup_unicode` | lookup |
| 0.51% | `python` | `_PyCode_New` | memory |

## tomli_loads

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 23.29% | `[JIT]` | `jit` | jit |
| 22.97% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.75% | `python` | `_PyLong_Add` | int |
| 4.38% | `python` | `long_dealloc` | memory |
| 4.23% | `python` | `_PySet_Contains` | unknown |
| 2.55% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.33% | `python` | `PyDict_GetItemRef` | dict |
| 2.20% | `python` | `PyDict_Contains` | dict |
| 2.13% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.07% | `python` | `_PyUnicode_Equal` | str |
| 1.28% | `python` | `_PyIncrementalNewlineDecoder_decode.cold` | memory |
| 1.17% | `python` | `tupledealloc` | memory |
| 1.06% | `python` | `set_contains_lock_held` | miscobj |
| 0.90% | `python` | `object_isinstance` | dynamic |
| 0.72% | `python` | `PyUnicode_New` | memory |
| 0.68% | `python` | `_PyTuple_FromArraySteal` | tuple |
| 0.65% | `python` | `_PyIncrementalNewlineDecoder_decode` | memory |
| 0.60% | `python` | `sre_ucs4_match` | library |
| 0.59% | `python` | `PyFunction_NewWithQualName` | memory |
| 0.55% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.54% | `python` | `unicode_subscript` | str |
| 0.53% | `python` | `_Py_dict_lookup` | lookup |

## tornado_http

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 26.22% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.01% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.13% | `[JIT]` | `jit` | jit |
| 1.87% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.80% | `python` | `type_new` | memory |
| 1.39% | `python` | `deduce_unreachable` | unknown |
| 1.30% | `python` | `tupledealloc` | memory |
| 1.22% | `python` | `visit_decref` | gc |
| 1.21% | `python` | `gc_collect_main` | gc |
| 0.92% | `python` | `visit_reachable` | gc |
| 0.81% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.73% | `python` | `PyDict_GetItemRef` | dict |
| 0.72% | `python` | `_PyCode_New` | memory |
| 0.70% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 0.69% | `[kernel.kallsyms]` | `copy_user_enhanced_fast_string` | kernel |
| 0.63% | `python` | `list_dealloc` | memory |
| 0.57% | `python` | `dict_setdefault_ref_lock_held` | dict |
| 0.57% | `python` | `find_name_in_mro` | lookup |
| 0.56% | `python` | `r_object` | import |
| 0.56% | `python` | `subtype_dealloc` | memory |
| 0.53% | `python` | `sre_ucs1_match` | library |
| 0.52% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.50% | `python` | `PyUnicode_FromKindAndData` | str |
| 0.50% | `python` | `unicode_dealloc` | memory |

## typing_runtime_protocols

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 28.73% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 3.66% | `[JIT]` | `jit` | jit |
| 3.45% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 3.12% | `python` | `_Py_dict_lookup` | lookup |
| 2.67% | `python` | `tupledealloc` | memory |
| 2.14% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.05% | `python` | `_Py_type_getattro` | lookup |
| 1.60% | `python` | `PyObject_GC_Del` | gc |
| 1.50% | `python` | `PyDict_Contains` | dict |
| 1.37% | `python` | `tuplehash` | tuple |
| 1.26% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.20% | `python` | `type_new` | memory |
| 1.15% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 1.10% | `python` | `frame_dealloc` | memory |
| 1.06% | `python` | `PyTraceBack_Here` | exceptions |
| 1.06% | `python` | `_PyObject_GC_New` | gc |
| 0.98% | `python` | `getset_get` | dynamic |
| 0.92% | `python` | `wrap_descr_get` | unknown |
| 0.90% | `python` | `_PyFrame_MakeAndSetFrameObject` | unknown |
| 0.90% | `python` | `bounded_lru_cache_wrapper` | unknown |
| 0.90% | `python` | `wrapper_call` | unknown |
| 0.87% | `python` | `PySet_Contains` | unknown |
| 0.84% | `python` | `gc_collect_main` | gc |
| 0.83% | `python` | `PyObject_Vectorcall` | dynamic |
| 0.82% | `python` | `tuple_iter` | tuple |
| 0.78% | `python` | `deduce_unreachable` | unknown |
| 0.70% | `python` | `tuplecontains` | tuple |
| 0.70% | `python` | `visit_decref` | gc |
| 0.66% | `python` | `method_dealloc` | memory |
| 0.65% | `python` | `weakref_richcompare` | unknown |
| 0.60% | `python` | `_PyDict_GetItem_KnownHash` | dict |
| 0.59% | `python` | `PyObject_RichCompare` | dynamic |
| 0.56% | `python` | `_Py_type_getattro_impl` | dynamic |
| 0.55% | `python` | `_PyCode_New` | memory |
| 0.55% | `python` | `PyArg_UnpackTuple` | calls |
| 0.53% | `python` | `tb_dealloc` | memory |
| 0.51% | `python` | `BaseException_new` | memory |

## unpack_sequence

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 55.14% | `[JIT]` | `jit` | jit |
| 23.38% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 0.86% | `python` | `type_new` | memory |
| 0.72% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 0.60% | `python` | `visit_decref` | gc |
| 0.59% | `python` | `gc_collect_main` | gc |
| 0.52% | `python` | `deduce_unreachable` | unknown |

## unpickle

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 12.92% | `python` | `unicode_decode_utf8` | str |
| 8.78% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `load` | library |
| 7.98% | `python` | `insertdict` | dict |
| 5.98% | `python` | `siphash13` | str |
| 5.43% | `python` | `unicode_dealloc` | memory |
| 5.10% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `load_counted_binunicode` | library |
| 3.74% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 2.89% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 2.81% | `python` | `dictresize` | dict |
| 2.00% | `python` | `dict_ass_sub` | dict |
| 1.85% | `python` | `PyMem_Realloc` | memory |
| 1.57% | `python` | `dict_dealloc` | memory |
| 1.47% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pdata_clear` | library |
| 1.39% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Unpickler_dealloc` | library |
| 1.35% | `python` | `PyObject_SetItem` | dynamic |
| 0.96% | `[JIT]` | `jit` | jit |
| 0.93% | `python` | `list_dealloc` | memory |
| 0.88% | `python` | `long_dealloc` | memory |
| 0.85% | `python` | `type_new` | memory |
| 0.82% | `python` | `PyLong_FromLong` | int |
| 0.81% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pdata_push` | library |
| 0.71% | `libc-2.31.so` | `pthread_attr_setschedparam` | libc |
| 0.63% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `do_setitems.isra.0` | library |
| 0.62% | `python` | `PyMem_Free` | memory |
| 0.62% | `python` | `unicode_hash` | str |
| 0.61% | `python` | `_PyObject_GC_New` | gc |
| 0.60% | `python` | `gc_collect_main` | gc |
| 0.55% | `python` | `visit_decref` | gc |
| 0.54% | `python` | `deduce_unreachable` | unknown |

## unpickle_list

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 16.52% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `load` | library |
| 13.27% | `python` | `list_dealloc` | memory |
| 8.30% | `python` | `PyList_New` | memory |
| 5.17% | `python` | `PyList_SetSlice` | list |
| 5.07% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 5.04% | `python` | `PyLong_FromLong` | int |
| 5.03% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `Pdata_push` | library |
| 3.45% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `do_append.isra.0` | library |
| 3.03% | `python` | `_PyObject_Malloc` | memory |
| 1.91% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.38% | `python` | `list_resize` | list |
| 1.08% | `[JIT]` | `jit` | jit |
| 1.03% | `python` | `type_new` | memory |
| 0.86% | `python` | `PyMem_Realloc` | memory |
| 0.81% | `python` | `gc_collect_main` | gc |
| 0.80% | `_pickle.cpython-313-x86_64-linux-gnu.so` | `0x0000000000005ba4` | library |
| 0.73% | `python` | `deduce_unreachable` | unknown |
| 0.73% | `python` | `visit_decref` | gc |
| 0.57% | `python` | `_PyCode_New` | memory |
| 0.56% | `python` | `PyMem_Free` | memory |
| 0.54% | `python` | `visit_reachable` | gc |
| 0.52% | `python` | `_PyObject_GC_New` | gc |

## unpickle_pure_python

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 29.93% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 21.86% | `[JIT]` | `jit` | jit |
| 2.96% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 2.75% | `python` | `PyObject_IsTrue` | dynamic |
| 2.73% | `python` | `PyDict_GetItemRef` | dict |
| 2.61% | `python` | `_io_BytesIO_read` | unknown |
| 1.61% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.35% | `python` | `unicode_decode_utf8` | str |
| 1.04% | `python` | `bytes_subscript` | str |
| 0.97% | `python` | `unicode_new` | memory |
| 0.94% | `python` | `tupledealloc` | memory |
| 0.84% | `python` | `type_new` | memory |
| 0.83% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.77% | `python` | `PyObject_GetItem` | dynamic |
| 0.76% | `python` | `insertdict` | dict |
| 0.74% | `python` | `PyObject_Free` | dynamic |
| 0.67% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.62% | `python` | `gc_collect_main` | gc |
| 0.59% | `python` | `PyObject_Size` | dynamic |
| 0.57% | `python` | `PyObject_IsInstance` | dynamic |
| 0.55% | `python` | `_PyDict_SetItem_Take2` | dict |
| 0.55% | `python` | `deduce_unreachable` | unknown |
| 0.55% | `python` | `siphash13` | str |
| 0.50% | `python` | `visit_decref` | gc |

## xml_etree

| percentage | object | symbol | category |
| ---: | :--- | :--- | :--- |
| 15.91% | `python` | `_PyEval_EvalFrameDefault` | interpreter |
| 4.63% | `[JIT]` | `jit` | jit |
| 3.21% | `python` | `PyObject_GenericGetAttr` | dynamic |
| 3.01% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `doContent` | library |
| 2.28% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `PyExpat_XML_Parse` | library |
| 2.06% | `libc-2.31.so` | `__nss_database_lookup` | libc |
| 1.91% | `python` | `_io_TextIOWrapper_write` | unknown |
| 1.91% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `normal_contentTok` | library |
| 1.91% | `python` | `unicode_decode_utf8` | str |
| 1.78% | `python` | `deduce_unreachable` | unknown |
| 1.72% | `python` | `visit_decref` | gc |
| 1.67% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `hash` | library |
| 1.63% | `python` | `visit_reachable` | gc |
| 1.62% | `pyexpat.cpython-313-x86_64-linux-gnu.so` | `storeAtts` | library |
| 1.57% | `python` | `unicode_dealloc` | memory |
| 1.48% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `makeuniversal.isra.0` | library |
| 1.44% | `python` | `gc_collect_main` | gc |
| 1.41% | `python` | `_PyObject_GC_New` | gc |
| 1.37% | `python` | `PyUnicode_Concat` | str |
| 1.36% | `python` | `_PyEval_FrameClearAndPop` | interpreter |
| 1.35% | `python` | `PyObject_GC_Del` | gc |
| 1.21% | `python` | `PyObject_VectorcallMethod` | dynamic |
| 1.17% | `python` | `object_isinstance` | dynamic |
| 1.03% | `python` | `tupledealloc` | memory |
| 0.93% | `python` | `list_dealloc` | memory |
| 0.89% | `python` | `PyBytes_FromStringAndSize` | str |
| 0.89% | `python` | `long_to_decimal_string_internal` | int |
| 0.89% | `python` | `PyObject_GetAttr` | dynamic |
| 0.86% | `python` | `PyUnicode_Format` | str |
| 0.85% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `elementiter_next` | library |
| 0.85% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `element_gc_traverse` | library |
| 0.82% | `python` | `_PyFunction_Vectorcall` | calls |
| 0.76% | `python` | `PyUnicode_Contains` | str |
| 0.75% | `python` | `getset_get` | dynamic |
| 0.73% | `python` | `PyDict_GetItemWithError` | dict |
| 0.66% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `treebuilder_handle_start` | library |
| 0.66% | `python` | `siphash13` | str |
| 0.66% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `element_dealloc` | library |
| 0.64% | `python` | `PyObject_Free` | dynamic |
| 0.64% | `python` | `vgetargs1_impl` | calls |
| 0.63% | `python` | `_PyObject_MakeTpCall` | dynamic |
| 0.61% | `python` | `type_new` | memory |
| 0.59% | `python` | `_PyEvalFramePushAndInit` | interpreter |
| 0.53% | `python` | `BaseException_new` | memory |
| 0.52% | `python` | `list_vectorcall` | list |
| 0.50% | `_elementtree.cpython-313-x86_64-linux-gnu.so` | `treebuilder_handle_end.isra.0` | library |


## Categories

### interpreter

22.50% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 19.89% | python | _PyEval_EvalFrameDefault |
| 1.71% | python | _PyEval_FrameClearAndPop |
| 0.36% | python | _PyEvalFramePushAndInit |
| 0.10% | python | _PyEval_EvalFrameDefault.cold |
| 0.10% | python | PyEval_RestoreThread |
| 0.08% | python | _PyPegen_fill_token |
| 0.07% | python | _PyFrame_ClearExceptCode |
| 0.03% | python | PyEval_SaveThread |
| 0.03% | python | intern_string_constants |
| 0.02% | python | _PyPegen_update_memo |
| 0.02% | python | _PyCode_Validate |
| 0.01% | python | _PyPegen_name_token |
| 0.01% | python | _PyPegen_Parser_Free |

### library

10.12% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 1.61% | python | sre_ucs1_match |
| 1.29% | _pickle.cpython-313-x86_64-linux-gnu.so | save |
| 0.75% | libz.so.1.2.11 | crc32_combine64 |
| 0.73% | python | sre_ucs2_charset.isra.0 |
| 0.46% | _json.cpython-313-x86_64-linux-gnu.so | _parse_object_unicode |
| 0.30% | _pickle.cpython-313-x86_64-linux-gnu.so | load |
| 0.29% | _pickle.cpython-313-x86_64-linux-gnu.so | _Pickler_Write |
| 0.28% | libz.so.1.2.11 | inflateBackEnd |
| 0.24% | _pickle.cpython-313-x86_64-linux-gnu.so | memo_put.isra.0 |
| 0.22% | python | sre_search |
| 0.19% | libpthread-2.31.so | __pthread_mutex_lock |
| 0.18% | libpthread-2.31.so | pthread_mutex_unlock |
| 0.15% | libm-2.31.so | f64xsubf128 |
| 0.15% | python | sre_ucs1_count |
| 0.13% | ld-2.31.so | _dl_rtld_di_serinfo |
| 0.13% | python | _sre_SRE_Pattern_match |
| 0.10% | _json.cpython-313-x86_64-linux-gnu.so | encoder_encode_key_value |
| 0.08% | _pickle.cpython-313-x86_64-linux-gnu.so | _Pickler_write_bytes |
| 0.08% | libpython3.11.so.1.0 | _PyEval_EvalFrameDefault |
| 0.07% | tracer.cpython-313-x86_64-linux-gnu.so | CTracer_trace |
| 0.07% | _pickle.cpython-313-x86_64-linux-gnu.so | Pdata_push |
| 0.06% | _pickle.cpython-313-x86_64-linux-gnu.so | load_counted_binunicode |
| 0.06% | _asyncio.cpython-313-x86_64-linux-gnu.so | TaskObj_traverse |
| 0.06% | libsqlite3.so.0.8.6 | sqlite3_reset |
| 0.05% | _pickle.cpython-313-x86_64-linux-gnu.so | Pickler_dealloc |
| 0.05% | libmagic.so.1.0.0 | 0x000000000000f936 |
| 0.04% | _pickle.cpython-313-x86_64-linux-gnu.so | do_append.isra.0 |
| 0.04% | libz.so.1.2.11 | inflateCodesUsed |
| 0.04% | array.cpython-313-x86_64-linux-gnu.so | array_subscr |
| 0.04% | ld-2.31.so | _dl_catch_error |
| 0.04% | pyexpat.cpython-313-x86_64-linux-gnu.so | doContent |
| 0.03% | libm-2.31.so | __fmod_finite |
| 0.03% | _json.cpython-313-x86_64-linux-gnu.so | py_encode_basestring_ascii |
| 0.03% | _json.cpython-313-x86_64-linux-gnu.so | _match_number_unicode.isra.0 |
| 0.03% | _pickle.cpython-313-x86_64-linux-gnu.so | memo_get.isra.0 |
| 0.03% | python | pattern_subx |
| 0.03% | libmagic.so.1.0.0 | 0x000000000000f932 |
| 0.03% | pyexpat.cpython-313-x86_64-linux-gnu.so | PyExpat_XML_Parse |
| 0.03% | _decimal.cpython-313-x86_64-linux-gnu.so | _mpd_qaddsub |
| 0.03% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::encodeValue |
| 0.02% | _pickle.cpython-313-x86_64-linux-gnu.so | Unpickler_dealloc |
| 0.02% | pyexpat.cpython-313-x86_64-linux-gnu.so | normal_contentTok |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | _mpd_baseshiftr |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | nm_mpd_qmul |
| 0.02% | libpthread-2.31.so | pthread_cond_signal@@GLIBC_2.3.2 |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | nm_mpd_qadd |
| 0.02% | pyexpat.cpython-313-x86_64-linux-gnu.so | hash |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | convert_op |
| 0.02% | libz.so.1.2.11 | inflate |
| 0.02% | pyexpat.cpython-313-x86_64-linux-gnu.so | storeAtts |
| 0.02% | _asyncio.cpython-313-x86_64-linux-gnu.so | task_step_impl |
| 0.02% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005cd4 |
| 0.02% | array.cpython-313-x86_64-linux-gnu.so | array_ass_subscr |
| 0.02% | _elementtree.cpython-313-x86_64-linux-gnu.so | makeuniversal.isra.0 |
| 0.02% | _pickle.cpython-313-x86_64-linux-gnu.so | Pdata_clear |
| 0.02% | libsqlite3.so.0.8.6 | sqlite3_exec |
| 0.02% | libpython3.11.so.1.0 | _PyDict_GetItem_KnownHash |
| 0.02% | libsqlite3.so.0.8.6 | sqlite3_randomness |
| 0.02% | _asyncio.cpython-313-x86_64-linux-gnu.so | TaskStepMethWrapper_traverse |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | mpd_qshiftr |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | _mpd_qmul |
| 0.02% | _heapq.cpython-313-x86_64-linux-gnu.so | _heapq_heappop |
| 0.02% | _decimal.cpython-313-x86_64-linux-gnu.so | mpd_qfinalize |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | factorial_partial_product |
| 0.01% | python | sre_ucs1_match.cold |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | TaskObj_clear |
| 0.01% | libpython3.11.so.1.0 | PyObject_Malloc |
| 0.01% | _json.cpython-313-x86_64-linux-gnu.so | _parse_array_unicode |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_mpd_qquantize |
| 0.01% | _bisect.cpython-313-x86_64-linux-gnu.so | _bisect_bisect_right |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_value_double |
| 0.01% | libpython3.11.so.1.0 | deduce_unreachable |
| 0.01% | libpthread-2.31.so | sem_post@@GLIBC_2.2.5 |
| 0.01% | _sqlite3.cpython-313-x86_64-linux-gnu.so | _pysqlite_query_execute |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | FutureObj_traverse |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | element_gc_traverse |
| 0.01% | libpython3.11.so.1.0 | visit_decref |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | _pickle_dumps |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_str_value |
| 0.01% | libpython3.11.so.1.0 | type_new |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005ba4 |
| 0.01% | libssl.so.1.1 | SSL_rstate_string |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | elementiter_next |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | math_factorial |
| 0.01% | libpthread-2.31.so | sem_trywait@@GLIBC_2.2.5 |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005fc4 |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | _asyncio_Future_add_done_callback |
| 0.01% | libpython3.11.so.1.0 | PyDict_SetDefault |
| 0.01% | array.cpython-313-x86_64-linux-gnu.so | d_setitem |
| 0.01% | libpython3.11.so.1.0 | visit_reachable |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | 0x0000000000005e54 |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_preupdate_old |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_dealloc |
| 0.01% | libpython3.11.so.1.0 | r_object |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | _asyncio_Task___init__ |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | _pickle_loads |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | dec_addstatus |
| 0.01% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::decodeValue |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | element_dealloc |
| 0.01% | math.cpython-313-x86_64-linux-gnu.so | math_sqrt |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | future_init |
| 0.01% | _struct.cpython-313-x86_64-linux-gnu.so | unpack |
| 0.01% | libpython3.11.so.1.0 | gc_collect_main |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | mpd_qquantize |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | treebuilder_handle_start |
| 0.01% | _struct.cpython-313-x86_64-linux-gnu.so | s_pack |
| 0.01% | _decimal.cpython-313-x86_64-linux-gnu.so | PyDecType_New |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_vtab_config |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_enable_shared_cache |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_value_int64 |
| 0.01% | _pickle.cpython-313-x86_64-linux-gnu.so | do_setitems.isra.0 |
| 0.01% | _json.cpython-313-x86_64-linux-gnu.so | encoder_listencode_obj |
| 0.01% | python | _sre_SRE_Pattern_search |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_wal_checkpoint |
| 0.01% | python | sre_ucs4_match |
| 0.01% | libsqlite3.so.0.8.6 | sqlite3_extended_errcode |
| 0.01% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readStruct |
| 0.01% | libpython3.11.so.1.0 | PyObject_Free |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | task_step |
| 0.01% | fastbinary.cpython-313-x86_64-linux-gnu.so | apache::thrift::py::ProtocolBase<apache::thrift::py::BinaryProtocol>::readBytes |
| 0.01% | libm-2.31.so | pow |
| 0.01% | _asyncio.cpython-313-x86_64-linux-gnu.so | call_soon |
| 0.01% | _elementtree.cpython-313-x86_64-linux-gnu.so | treebuilder_handle_end.isra.0 |
| 0.01% | python | _sre_compile |

### memory

9.99% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.95% | python | type_new |
| 0.83% | python | tupledealloc |
| 0.81% | python | list_dealloc |
| 0.67% | python | long_dealloc |
| 0.55% | python | unicode_dealloc |
| 0.41% | python | _PyCode_New |
| 0.36% | python | dict_dealloc |
| 0.35% | python | subtype_dealloc |
| 0.35% | python | gen_dealloc |
| 0.30% | python | PyList_New |
| 0.29% | python | PyMem_Free |
| 0.24% | python | meth_dealloc |
| 0.21% | python | PyFunction_NewWithQualName |
| 0.21% | python | _PyLong_New |
| 0.20% | python | object_new |
| 0.20% | python | _PyObject_Malloc |
| 0.17% | python | PyMem_Malloc |
| 0.16% | python | PyType_GenericAlloc |
| 0.16% | python | PyUnicode_New |
| 0.15% | python | func_dealloc |
| 0.13% | python | _Py_Dealloc |
| 0.13% | python | method_dealloc |
| 0.12% | python | code_dealloc |
| 0.12% | python | set_dealloc |
| 0.12% | python | PyMem_Realloc |
| 0.11% | python | BaseException_new |
| 0.11% | python | float_dealloc |
| 0.11% | python | PyTuple_New |
| 0.11% | python | frame_dealloc |
| 0.09% | python | slice_dealloc |
| 0.06% | python | list_new_prealloc |
| 0.06% | python | listiter_dealloc |
| 0.06% | python | StopIteration_dealloc |
| 0.06% | python | allocate_from_new_pool |
| 0.05% | python | dictiter_dealloc |
| 0.04% | python | tb_dealloc |
| 0.04% | python | PyType_GenericNew |
| 0.04% | python | BaseException_dealloc |
| 0.04% | python | make_new_set |
| 0.04% | python | _PyObject_Free |
| 0.04% | python | PySlice_New |
| 0.04% | python | tp_new_wrapper |
| 0.04% | python | range_dealloc |
| 0.03% | python | cell_dealloc |
| 0.03% | python | dictview_dealloc |
| 0.03% | python | slot_tp_new |
| 0.03% | python | context_tp_dealloc |
| 0.03% | python | weakref_dealloc |
| 0.02% | python | tupleiter_dealloc |
| 0.02% | python | _PyIncrementalNewlineDecoder_decode.cold |
| 0.02% | python | match_dealloc |
| 0.02% | python | _PyObject_New |
| 0.02% | python | _PyFloat_ExactDealloc |
| 0.02% | python | async_gen_asend_new |
| 0.02% | python | unicode_new |
| 0.02% | python | async_gen_asend_dealloc |
| 0.02% | python | _PyAsyncGenValueWrapperNew |
| 0.02% | python | _Py_NewReference |
| 0.02% | python | weakref___new__ |
| 0.02% | python | PyObject_CallFinalizerFromDealloc |
| 0.02% | python | structseq_dealloc |
| 0.01% | python | async_gen_wrapped_val_dealloc |
| 0.01% | python | PyDict_New |
| 0.01% | python | PyCMethod_New |
| 0.01% | python | object_dealloc |
| 0.01% | python | PyWeakref_NewRef |
| 0.01% | python | _PyIncrementalNewlineDecoder_decode |
| 0.01% | python | _PyTokenizer_translate_newlines.constprop.0 |
| 0.01% | python | AttributeError_dealloc |
| 0.01% | python | _PyObject_Realloc |
| 0.01% | python | descr_dealloc |
| 0.01% | python | pattern_new_match.isra.0 |
| 0.01% | python | reversed_new_impl |
| 0.01% | python | _PyMem_RawMalloc |
| 0.01% | python | zip_new |

### jit

9.21% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 9.21% | [JIT] | jit |

### gc

8.76% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 2.86% | python | gc_collect_main |
| 1.80% | python | visit_decref |
| 1.68% | python | visit_reachable |
| 0.46% | python | PyObject_GC_Del |
| 0.43% | python | subtype_traverse |
| 0.28% | python | _PyObject_GC_New |
| 0.28% | python | dict_traverse |
| 0.25% | python | list_traverse |
| 0.13% | python | set_traverse |
| 0.11% | python | gen_traverse |
| 0.10% | python | func_traverse |
| 0.10% | python | _PyObject_GC_NewVar |
| 0.06% | python | type_traverse |
| 0.03% | python | PyObject_GC_UnTrack |
| 0.03% | python | meth_traverse |
| 0.02% | python | gc_traverse |
| 0.02% | python | PyObject_GC_Track |
| 0.02% | python | context_tp_traverse |
| 0.01% | python | frame_traverse |
| 0.01% | python | descr_traverse |
| 0.01% | python | module_traverse |
| 0.01% | python | executor_traverse |
| 0.01% | python | method_traverse |
| 0.01% | python | PyObject_IS_GC |
| 0.01% | python | cell_traverse |

### unknown

7.31% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 1.94% | python | deduce_unreachable |
| 0.27% | python | make_gen |
| 0.21% | python | slot_tp_init |
| 0.18% | python | _Py_hashtable_get |
| 0.16% | python | uop_optimize |
| 0.10% | python | clear_slots |
| 0.09% | python | func_descr_get |
| 0.08% | python | _PyFrame_MakeAndSetFrameObject |
| 0.08% | python | _PySet_Contains |
| 0.08% | python | method_vectorcall |
| 0.08% | python | _PyStack_UnpackDict |
| 0.07% | python | slot_mp_subscript |
| 0.06% | python | gen_iternext |
| 0.06% | python | memcpy@plt |
| 0.06% | python | memset@plt |
| 0.06% | python | range_vectorcall |
| 0.05% | python | make_executor_from_uops |
| 0.05% | python | convert_to_double |
| 0.05% | python | call_instrumentation_vector |
| 0.05% | python | _PyJIT_Compile |
| 0.05% | python | range_iter |
| 0.04% | python | builtin_min |
| 0.04% | python | _stringio_readline.cold |
| 0.04% | python | builtin_hasattr |
| 0.04% | python | as_ucs4 |
| 0.04% | python | _PyBuildSlice_Consume2 |
| 0.04% | python | path_converter |
| 0.04% | python | _io_BytesIO_read |
| 0.04% | python | _PyCfg_OptimizeCodeUnit.constprop.0 |
| 0.04% | python | slot_tp_hash |
| 0.04% | python | dictkeys_decref.part.0 |
| 0.04% | python | member_get |
| 0.03% | python | PySys_Audit |
| 0.03% | python | _Py_module_getattro |
| 0.03% | python | optimize_uops.constprop.0 |
| 0.03% | python | ucs4lib_find_max_char |
| 0.03% | python | gen_send_ex2 |
| 0.03% | [vdso] | __vdso_clock_gettime |
| 0.03% | python | vectorcall_maybe.constprop.0 |
| 0.03% | python | _PyOptimizer_Optimize |
| 0.03% | python | PySet_Add |
| 0.03% | python | cm_descr_get |
| 0.03% | python | dictitems_iter |
| 0.03% | python | async_gen_asend_send |
| 0.03% | python | state_init |
| 0.03% | python | gen_send_ex |
| 0.03% | python | _Py_VaBuildStack.constprop.0 |
| 0.03% | python | slot_mp_ass_subscript |
| 0.03% | python | _PyAssemble_MakeCodeObject |
| 0.02% | python | term_raw |
| 0.02% | python | _io_TextIOWrapper_write |
| 0.02% | python | builtin_id |
| 0.02% | python | range_subscript |
| 0.02% | python | call_one_instrument |
| 0.02% | python | code_hash |
| 0.02% | python | bitwise_xor_rule |
| 0.02% | python | hashtable_unicode_compare |
| 0.02% | python | PyContextVar_Get |
| 0.02% | python | bounded_lru_cache_wrapper |
| 0.02% | python | binary_op1 |
| 0.02% | python | builtin___import__ |
| 0.02% | python | hashtable_unicode_hash |
| 0.02% | python | convertitem |
| 0.02% | python | vgetargs1_impl.cold |
| 0.02% | python | unsafe_tuple_compare |
| 0.02% | python | Py_XDECREF.lto_priv.1 |
| 0.02% | python | binary_op |
| 0.02% | python | wrapperdescr_call |
| 0.02% | python | builtin_sum |
| 0.02% | python | _PyCfg_OptimizedCfgToInstructionSequence |
| 0.02% | python | _PyCoro_GetAwaitableIter |
| 0.02% | python | _Py_slot_tp_getattr_hook |
| 0.02% | python | _PyModule_ClearDict |
| 0.02% | python | write_bytes |
| 0.02% | python | make_range_object |
| 0.02% | python | _PyDictKeys_StringLookup |
| 0.02% | python | classmethod_get |
| 0.02% | python | member_set |
| 0.02% | python | PySet_Contains |
| 0.02% | python | async_gen_unwrap_value.isra.0 |
| 0.01% | python | shift_expr_rule |
| 0.01% | python | ScandirIterator_iternext |
| 0.01% | python | build_indices_generic |
| 0.01% | python | memcmp@plt |
| 0.01% | python | do_mktuple |
| 0.01% | python | _PyBytes_Resize |
| 0.01% | python | os_listdir |
| 0.01% | python | _add_methods_to_object |
| 0.01% | python | sum_rule |
| 0.01% | python | slot_sq_contains |
| 0.01% | python | builtin_issubclass |
| 0.01% | python | _Py_bytes_lower |
| 0.01% | python | Py_XDECREF.lto_priv.6 |
| 0.01% | python | _PyGen_FetchStopIterationValue.cold |
| 0.01% | python | primary_raw |
| 0.01% | python | wrapper_call |
| 0.01% | python | expression_rule |
| 0.01% | python | PyIndex_Check |
| 0.01% | python | atom_rule |
| 0.01% | python | ins1 |
| 0.01% | python | _io_open |
| 0.01% | python | get_type_attr_as_size |
| 0.01% | python | _PyThreadState_GetCurrent |
| 0.01% | python | lookup_maybe_method |
| 0.01% | python | mro_implementation_unlocked |
| 0.01% | python | call_trace_func.isra.0 |
| 0.01% | python | symtable_add_def_helper |
| 0.01% | python | va_build_value |
| 0.01% | python | slot_sq_item |
| 0.01% | python | wrap_descr_get |
| 0.01% | python | context_run |
| 0.01% | python | pthread_self@plt |
| 0.01% | python | _PyType_FromMetaclass_impl |
| 0.01% | python | PyThread_acquire_lock_timed |
| 0.01% | python | builtin_max |
| 0.01% | python | _PyGen_SetStopIterationValue |
| 0.01% | python | weakref_richcompare |
| 0.01% | python | PyTime_AsSecondsDouble |
| 0.01% | python | map_next |
| 0.01% | python | builtin_hash |
| 0.01% | python | lru_cache_make_key |
| 0.01% | python | _PyCode_GetCode |
| 0.01% | python | inversion_rule |
| 0.01% | python | ascii_upper_or_lower |
| 0.01% | python | clear_weakref |
| 0.01% | python | assign_version_tag |
| 0.01% | python | builtin_sorted |
| 0.01% | python | fill_time |
| 0.01% | python | update_slots_callback |
| 0.01% | python | frozenset_vectorcall |
| 0.01% | python | _Py_module_getattro_impl.part.0 |
| 0.01% | python | instr_sequence_to_cfg |
| 0.01% | python | astfold_expr |
| 0.01% | python | weakref_hash |
| 0.01% | python | slot_tp_iter |
| 0.01% | python | builtin_any |
| 0.01% | python | unsafe_latin_compare |
| 0.01% | python | pytime_divide |
| 0.01% | python | symtable_visit_expr |
| 0.01% | python | compiler_nameop |
| 0.01% | python | sm_descr_get |
| 0.01% | python | unsafe_long_compare |
| 0.01% | python | make_dict_from_instance_attributes |
| 0.01% | python | 0x0000000000086720 |
| 0.01% | python | _Py_call_instrumentation_jump |
| 0.01% | python | binary_iop1 |
| 0.01% | python | bitwise_or_rule |
| 0.01% | python | islice_next |
| 0.01% | python | _PyLexer_update_fstring_expr |
| 0.01% | python | update_slot |
| 0.01% | python | _PyBytes_FromList |
| 0.01% | python | analyze_block |
| 0.01% | python | _getbytevalue |
| 0.01% | python | _PyContext_Exit |
| 0.01% | python | new_dict |
| 0.01% | python | zip_next |
| 0.01% | python | map_vectorcall |
| 0.01% | python | compiler_visit_expr1 |
| 0.01% | python | _Py_dg_dtoa |
| 0.01% | python | _abc__abc_instancecheck |
| 0.01% | python | write_str |
| 0.01% | python | super_getattro |
| 0.01% | python | dictbytype |
| 0.01% | python | ucs4lib_utf8_encoder |
| 0.01% | python | _PyGen_yf |
| 0.01% | python | find_keyword |
| 0.01% | python | simple_stmt_rule |
| 0.01% | python | subtype_clear |
| 0.01% | python | pthread_mutex_unlock@plt |
| 0.01% | python | pthread_mutex_lock@plt |
| 0.01% | python | ucs4lib_utf8_decode |
| 0.01% | python | Py_UNICODE_ISALNUM.lto_priv.1 |
| 0.01% | python | _loop1_104_rule |
| 0.01% | python | _Py_SourceAsString |
| 0.01% | python | PyThread_get_thread_ident_ex |
| 0.01% | python | _PyCfg_ToInstructionSequence |

### dynamic

5.79% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.57% | python | PyObject_GenericGetAttr |
| 0.37% | python | _PyObject_GetMethod |
| 0.35% | python | object_isinstance |
| 0.32% | python | _PyObject_MakeTpCall |
| 0.27% | python | PyObject_GetAttr |
| 0.25% | python | PyObject_Free |
| 0.20% | python | PyObject_SetAttr |
| 0.17% | python | method_get |
| 0.16% | python | PyObject_RichCompare |
| 0.16% | python | _PySuper_Lookup |
| 0.15% | python | PyObject_IsTrue |
| 0.15% | python | PyObject_Vectorcall |
| 0.14% | python | PyType_GetModuleByDef |
| 0.14% | python | PyNumber_AsSsize_t |
| 0.13% | python | PyObject_VectorcallMethod |
| 0.12% | python | type_ready |
| 0.12% | python | PyObject_GetItem |
| 0.11% | python | _PyObject_LookupSpecial |
| 0.09% | python | PyObject_GetIter |
| 0.09% | python | getset_get |
| 0.08% | python | PyObject_IsInstance |
| 0.08% | python | type_call |
| 0.07% | python | PyObject_Hash |
| 0.07% | python | PyObject_GetOptionalAttr |
| 0.07% | python | _PyObject_GenericGetAttrWithDict |
| 0.07% | python | _Py_type_getattro_impl |
| 0.06% | python | slot_tp_richcompare |
| 0.06% | python | _PyObject_Call |
| 0.05% | python | PyObject_SetItem |
| 0.05% | python | PyObject_Str |
| 0.05% | python | PyMapping_GetOptionalItem |
| 0.05% | python | PyNumber_Multiply |
| 0.05% | python | _PyObject_ClearFreeLists |
| 0.05% | python | PyObject_CallOneArg |
| 0.05% | python | _PyObject_InitInlineValues |
| 0.04% | python | PyObject_SetAttrString |
| 0.04% | python | PyNumber_TrueDivide |
| 0.04% | python | PyNumber_Add |
| 0.04% | python | PyType_IsSubtype |
| 0.03% | python | PyNumber_And |
| 0.03% | python | StopIteration_init |
| 0.03% | python | _PyObject_VectorcallTstate.lto_priv.5 |
| 0.03% | python | PyNumber_Subtract |
| 0.03% | python | PyObject_Size |
| 0.03% | python | PyIter_Send |
| 0.02% | python | PySequence_Tuple |
| 0.02% | python | PySequence_List |
| 0.02% | python | PyObject_VisitManagedDict |
| 0.02% | python | PyObject_RichCompareBool |
| 0.02% | python | PyNumber_Remainder |
| 0.02% | python | PyObject_LengthHint |
| 0.01% | python | PyNumber_FloorDivide |
| 0.01% | python | PyObject_CallFunction |
| 0.01% | python | object_get_class |
| 0.01% | python | PyNumber_Rshift |
| 0.01% | python | PyNumber_InPlaceAdd |
| 0.01% | python | PyObject_ClearManagedDict |
| 0.01% | python | PyIter_Next |
| 0.01% | python | object_richcompare |
| 0.01% | python | _PyNumber_Index |
| 0.01% | python | PyObject_ClearWeakRefs |
| 0.01% | python | delitem_common |
| 0.01% | python | PySequence_Contains |
| 0.01% | python | object_recursive_isinstance.part.0 |
| 0.01% | python | object_vacall |
| 0.01% | python | PyNumber_Negative |
| 0.01% | python | _PyObject_GenericSetAttrWithDict |
| 0.01% | python | PyObject_CallMethodObjArgs |
| 0.01% | python | type_dealloc_common |
| 0.01% | python | object_hash |
| 0.01% | python | PyNumber_Index |
| 0.01% | python | PyObject_GetBuffer |
| 0.01% | python | object_init |
| 0.01% | python | _PyNumber_PowerNoMod |
| 0.01% | python | PyObject_SelfIter |
| 0.01% | python | PyObject_DelItem |
| 0.01% | python | PyNumber_Lshift |

### kernel

5.58% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.63% | [kernel.kallsyms] | copy_user_enhanced_fast_string |
| 0.28% | [kernel.kallsyms] | clear_page_erms |
| 0.16% | [kernel.kallsyms] | native_irq_return_iret |
| 0.11% | [kernel.kallsyms] | sync_regs |
| 0.11% | [kernel.kallsyms] | rmqueue |
| 0.10% | [kernel.kallsyms] | _raw_spin_lock |
| 0.10% | [kernel.kallsyms] | zap_pte_range.isra.0 |
| 0.10% | [kernel.kallsyms] | __d_lookup_rcu |
| 0.07% | [kernel.kallsyms] | perf_iterate_ctx |
| 0.07% | [kernel.kallsyms] | free_pcppages_bulk |
| 0.06% | [kernel.kallsyms] | memset_erms |
| 0.06% | [kernel.kallsyms] | __handle_mm_fault |
| 0.05% | [kernel.kallsyms] | find_vma |
| 0.05% | [kernel.kallsyms] | try_charge |
| 0.05% | [kernel.kallsyms] | release_pages |
| 0.05% | [kernel.kallsyms] | kmem_cache_alloc |
| 0.05% | [kernel.kallsyms] | filemap_map_pages |
| 0.04% | [kernel.kallsyms] | unmapped_area_topdown |
| 0.04% | [kernel.kallsyms] | __pagevec_lru_add_fn |
| 0.04% | [kernel.kallsyms] | get_mem_cgroup_from_mm |
| 0.04% | [kernel.kallsyms] | smp_call_function_single |
| 0.04% | [kernel.kallsyms] | syscall_return_via_sysret |
| 0.04% | [kernel.kallsyms] | mem_cgroup_throttle_swaprate |
| 0.04% | [kernel.kallsyms] | link_path_walk.part.0 |
| 0.04% | [kernel.kallsyms] | memcg_kmem_get_cache |
| 0.04% | [kernel.kallsyms] | native_flush_tlb_one_user |
| 0.04% | [kernel.kallsyms] | mem_cgroup_try_charge |
| 0.04% | [kernel.kallsyms] | handle_mm_fault |
| 0.03% | [kernel.kallsyms] | kmem_cache_free |
| 0.03% | [kernel.kallsyms] | __alloc_pages_nodemask |
| 0.03% | [kernel.kallsyms] | __slab_free |
| 0.03% | [kernel.kallsyms] | page_remove_rmap |
| 0.03% | [kernel.kallsyms] | anon_vma_interval_tree_insert |
| 0.03% | [kernel.kallsyms] | __ext4fs_dirhash |
| 0.03% | [kernel.kallsyms] | memcpy_erms |
| 0.03% | [kernel.kallsyms] | ext4_htree_store_dirent |
| 0.03% | [kernel.kallsyms] | entry_SYSCALL_64 |
| 0.03% | [kernel.kallsyms] | perf_event_alloc |
| 0.02% | [kernel.kallsyms] | kfree |
| 0.02% | [kernel.kallsyms] | find_get_entry |
| 0.02% | [kernel.kallsyms] | __perf_addr_filters_adjust |
| 0.02% | [kernel.kallsyms] | strncpy_from_user |
| 0.02% | [kernel.kallsyms] | __vma_adjust |
| 0.02% | [kernel.kallsyms] | do_syscall_64 |
| 0.02% | [kernel.kallsyms] | do_user_addr_fault |
| 0.02% | [kernel.kallsyms] | do_anonymous_page |
| 0.02% | [kernel.kallsyms] | filldir64 |
| 0.02% | [kernel.kallsyms] | vmacache_find |
| 0.02% | [kernel.kallsyms] | inode_permission |
| 0.02% | [kernel.kallsyms] | get_page_from_freelist |
| 0.02% | [kernel.kallsyms] | lookup_fast |
| 0.02% | [kernel.kallsyms] | perf_event_mmap |
| 0.02% | [kernel.kallsyms] | prep_new_page |
| 0.02% | [kernel.kallsyms] | __virt_addr_valid |
| 0.02% | [kernel.kallsyms] | __count_memcg_events |
| 0.02% | [kernel.kallsyms] | __mod_memcg_state |
| 0.02% | [kernel.kallsyms] | copy_page |
| 0.02% | [kernel.kallsyms] | _raw_spin_lock_irqsave |
| 0.02% | [kernel.kallsyms] | page_fault |
| 0.02% | [kernel.kallsyms] | error_entry |
| 0.02% | [kernel.kallsyms] | __mod_lruvec_state |
| 0.02% | [kernel.kallsyms] | walk_component |
| 0.02% | [kernel.kallsyms] | generic_permission |
| 0.02% | [kernel.kallsyms] | _cond_resched |
| 0.02% | [kernel.kallsyms] | rb_insert_color |
| 0.02% | [kernel.kallsyms] | change_protection_range |
| 0.02% | [kernel.kallsyms] | __rb_insert_augmented |
| 0.01% | [kernel.kallsyms] | ext4_getattr |
| 0.01% | [kernel.kallsyms] | entry_SYSCALL_64_after_hwframe |
| 0.01% | [kernel.kallsyms] | up_write |
| 0.01% | [kernel.kallsyms] | perf_iterate_sb |
| 0.01% | [kernel.kallsyms] | __vma_link_rb |
| 0.01% | [kernel.kallsyms] | str2hashbuf_signed |
| 0.01% | [kernel.kallsyms] | acct_collect |
| 0.01% | [kernel.kallsyms] | rb_next |
| 0.01% | [kernel.kallsyms] | __fget_light |
| 0.01% | [kernel.kallsyms] | psi_task_change |
| 0.01% | [kernel.kallsyms] | mmap_region |
| 0.01% | [kernel.kallsyms] | rcu_all_qs |
| 0.01% | [kernel.kallsyms] | free_unref_page_prepare.part.0 |
| 0.01% | [kernel.kallsyms] | free_pages_and_swap_cache |
| 0.01% | [kernel.kallsyms] | mutex_lock |
| 0.01% | [kernel.kallsyms] | up_read |
| 0.01% | [kernel.kallsyms] | __lru_cache_add |
| 0.01% | [kernel.kallsyms] | xas_load |
| 0.01% | [kernel.kallsyms] | page_counter_cancel |
| 0.01% | [kernel.kallsyms] | mutex_unlock |
| 0.01% | [kernel.kallsyms] | lru_cache_add_active_or_unevictable |
| 0.01% | [kernel.kallsyms] | security_inode_getattr |
| 0.01% | [kernel.kallsyms] | down_read_trylock |
| 0.01% | [kernel.kallsyms] | down_write |
| 0.01% | [kernel.kallsyms] | ___slab_alloc |
| 0.01% | [kernel.kallsyms] | pagevec_lru_move_fn |
| 0.01% | [kernel.kallsyms] | __mod_node_page_state |
| 0.01% | [kernel.kallsyms] | swapgs_restore_regs_and_return_to_usermode |
| 0.01% | [kernel.kallsyms] | fsnotify |
| 0.01% | [kernel.kallsyms] | tcp_sendmsg_locked |
| 0.01% | [kernel.kallsyms] | free_unref_page_list |
| 0.01% | [kernel.kallsyms] | generic_file_buffered_read |
| 0.01% | [kernel.kallsyms] | unmap_page_range |
| 0.01% | [kernel.kallsyms] | set_root |
| 0.01% | [kernel.kallsyms] | fpregs_assert_state_consistent |
| 0.01% | [kernel.kallsyms] | __check_object_size |
| 0.01% | [kernel.kallsyms] | __mod_zone_page_state |
| 0.01% | [kernel.kallsyms] | __follow_mount_rcu.isra.0 |
| 0.01% | [kernel.kallsyms] | __kmalloc |
| 0.01% | [kernel.kallsyms] | __lock_text_start |
| 0.01% | [kernel.kallsyms] | inherit_event.isra.0 |
| 0.01% | [kernel.kallsyms] | format_decode |
| 0.01% | [kernel.kallsyms] | alloc_pages_vma |
| 0.01% | [kernel.kallsyms] | mem_cgroup_commit_charge |
| 0.01% | [kernel.kallsyms] | page_add_file_rmap |
| 0.01% | [kernel.kallsyms] | update_curr |
| 0.01% | [kernel.kallsyms] | vsnprintf |
| 0.01% | [kernel.kallsyms] | show_cpuinfo |
| 0.01% | [kernel.kallsyms] | mem_cgroup_try_charge_delay |
| 0.01% | [kernel.kallsyms] | __legitimize_mnt |
| 0.01% | [kernel.kallsyms] | kmem_cache_alloc_trace |
| 0.01% | [kernel.kallsyms] | __ext4_check_dir_entry |
| 0.01% | [kernel.kallsyms] | anon_vma_interval_tree_remove |
| 0.01% | [kernel.kallsyms] | native_write_msr |
| 0.01% | [kernel.kallsyms] | in_group_p |
| 0.01% | [kernel.kallsyms] | update_cfs_group |
| 0.01% | [kernel.kallsyms] | native_sched_clock |
| 0.01% | [kernel.kallsyms] | __rb_erase_color |
| 0.01% | [kernel.kallsyms] | update_load_avg |
| 0.01% | [kernel.kallsyms] | free_unref_page_commit |
| 0.01% | [kernel.kallsyms] | memcg_kmem_put_cache |
| 0.01% | [kernel.kallsyms] | change_pte_range |
| 0.01% | [kernel.kallsyms] | mem_cgroup_from_task |
| 0.01% | [kernel.kallsyms] | unmap_single_vma |
| 0.01% | [kernel.kallsyms] | string_nocheck |
| 0.01% | [kernel.kallsyms] | perf_output_copy |
| 0.01% | [kernel.kallsyms] | perf_event_mmap_output |
| 0.01% | [kernel.kallsyms] | __update_load_avg_se |
| 0.01% | [kernel.kallsyms] | page_counter_try_charge |
| 0.01% | [kernel.kallsyms] | unlock_page |
| 0.01% | [kernel.kallsyms] | lockref_put_return |
| 0.01% | [kernel.kallsyms] | exit_to_usermode_loop |
| 0.01% | [kernel.kallsyms] | memchr |
| 0.01% | [kernel.kallsyms] | flush_tlb_mm_range |
| 0.01% | [kernel.kallsyms] | security_inode_permission |
| 0.01% | [kernel.kallsyms] | vma_interval_tree_insert |
| 0.01% | [kernel.kallsyms] | xas_start |
| 0.01% | [kernel.kallsyms] | alloc_set_pte |
| 0.01% | [kernel.kallsyms] | uncharge_page |
| 0.01% | [kernel.kallsyms] | kthread_blkcg |
| 0.01% | [kernel.kallsyms] | unlink_anon_vmas |
| 0.01% | [kernel.kallsyms] | do_mprotect_pkey |
| 0.01% | [kernel.kallsyms] | _raw_spin_lock_irq |
| 0.01% | [kernel.kallsyms] | __free_pages_ok |
| 0.01% | [kernel.kallsyms] | down_write_killable |
| 0.01% | [kernel.kallsyms] | __fput |
| 0.01% | [kernel.kallsyms] | page_add_new_anon_rmap |
| 0.01% | [kernel.kallsyms] | __alloc_file |
| 0.01% | [kernel.kallsyms] | __tcp_transmit_skb |
| 0.01% | [kernel.kallsyms] | __do_munmap |
| 0.01% | [kernel.kallsyms] | getname_flags |
| 0.01% | [kernel.kallsyms] | pmd_devmap_trans_unstable |
| 0.01% | [kernel.kallsyms] | skb_release_data |
| 0.01% | [kernel.kallsyms] | vfs_getattr_nosec |

### libc

3.71% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 2.34% | libc-2.31.so | __nss_database_lookup |
| 0.51% | libc-2.31.so | pthread_attr_setschedparam |
| 0.30% | libcrypto.so.1.1 | CRYPTO_secure_actual_size |
| 0.13% | libc-2.31.so | malloc |
| 0.04% | libc-2.31.so | free |
| 0.03% | libc-2.31.so | __gconv_get_alias_db |
| 0.02% | libc-2.31.so | pthread_cond_signal |
| 0.02% | libc-2.31.so | wcsrtombs |
| 0.02% | libc-2.31.so | pthread_mutex_lock |
| 0.02% | libc-2.31.so | pthread_self |
| 0.02% | libc-2.31.so | __errno_location |
| 0.02% | libc-2.31.so | clock_gettime |
| 0.01% | libc-2.31.so | pthread_mutex_unlock |
| 0.01% | libc-2.31.so | __libc_realloc |
| 0.01% | libc-2.31.so | _dl_addr |
| 0.01% | libc-2.31.so | __xstat |
| 0.01% | libc-2.31.so | __mprotect |
| 0.01% | libc-2.31.so | __wcsncasecmp_l |
| 0.01% | libc-2.31.so | psiginfo |

### int

3.61% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.66% | python | k_mul |
| 0.42% | python | _PyLong_Add |
| 0.39% | python | x_divrem |
| 0.28% | python | PyLong_FromLong |
| 0.23% | python | long_hash |
| 0.20% | python | long_to_decimal_string_internal |
| 0.16% | python | x_add |
| 0.14% | python | _PyLong_Subtract |
| 0.09% | python | long_bitwise |
| 0.09% | python | x_sub |
| 0.08% | python | long_richcompare |
| 0.08% | python | PyLong_AsLongAndOverflow |
| 0.08% | python | _PyLong_Multiply |
| 0.07% | python | PyLong_FromString |
| 0.07% | python | long_and |
| 0.07% | python | long_rshift |
| 0.07% | python | long_div |
| 0.06% | python | long_to_decimal_string |
| 0.05% | python | long_add |
| 0.04% | python | long_mod |
| 0.03% | python | long_mul |
| 0.03% | python | PyLong_FromSsize_t |
| 0.03% | python | PyLong_FromUnsignedLongLong |
| 0.02% | python | long_lshift |
| 0.02% | python | _PyLong_FromBytes |
| 0.01% | python | _PyLong_GCD |
| 0.01% | python | PyLong_AsLong |
| 0.01% | python | _PyLong_FromSTwoDigits |
| 0.01% | python | PyLong_FromUnsignedLong |
| 0.01% | python | long_xor |
| 0.01% | python | long_vectorcall |
| 0.01% | python | PyLong_AsSsize_t |
| 0.01% | python | _PyLong_Lshift |
| 0.01% | python | PyLong_AsInt |
| 0.01% | python | PyLong_AsDouble.part.0 |
| 0.01% | python | PyLong_FromUnicodeObject |

### dict

3.56% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.59% | python | PyDict_GetItemRef |
| 0.48% | python | dict_setdefault_ref_lock_held |
| 0.43% | python | insertdict |
| 0.34% | python | PyDict_SetItem |
| 0.28% | python | dict_get |
| 0.25% | python | dictresize |
| 0.20% | python | PyDict_Next |
| 0.19% | python | insert_to_emptydict |
| 0.17% | python | PyDict_Contains |
| 0.10% | python | dict_subscript |
| 0.08% | python | dictiter_iternextitem |
| 0.05% | python | dict_merge |
| 0.04% | python | _PyDict_SetItem_Take2 |
| 0.04% | python | dict_items |
| 0.03% | python | PyDict_GetItemWithError |
| 0.03% | python | dict_ass_sub |
| 0.03% | python | PyDict_Copy |
| 0.03% | python | _PyDict_FromItems |
| 0.02% | python | PyDict_DelItem |
| 0.02% | python | _PyDict_GetItem_KnownHash |
| 0.02% | python | _PyDict_Next |
| 0.02% | python | dictiter_iternextvalue |
| 0.02% | python | dictiter_iternextkey |
| 0.01% | python | _PyDict_LoadGlobal |
| 0.01% | python | dict_getitem |
| 0.01% | python | PyDict_SetItemString |
| 0.01% | python | dict_iter |

### str

3.21% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.49% | python | siphash13 |
| 0.40% | python | unicode_decode_utf8 |
| 0.26% | python | PyUnicode_FromKindAndData |
| 0.24% | python | PyUnicode_Substring |
| 0.20% | python | _PyUnicode_JoinArray |
| 0.14% | python | PyBytes_FromStringAndSize |
| 0.11% | python | unicode_replace |
| 0.09% | python | _PyUnicodeWriter_PrepareInternal |
| 0.09% | python | PyUnicode_Format |
| 0.07% | python | _PyUnicodeWriter_WriteStr |
| 0.07% | python | PyUnicode_FromFormatV |
| 0.07% | python | PyUnicode_Concat |
| 0.06% | python | _PyUnicode_InternInPlace |
| 0.05% | python | unicode_subscript |
| 0.05% | python | PyUnicode_RichCompare |
| 0.05% | python | PyUnicode_FSConverter |
| 0.05% | python | bytes_subscript |
| 0.05% | python | _PyUnicode_FromUCS4 |
| 0.04% | python | unicode_hash |
| 0.04% | python | PyUnicode_Contains |
| 0.04% | python | _PyUnicode_Equal |
| 0.04% | python | unicode_encode |
| 0.03% | python | bytes_concat |
| 0.03% | python | PyUnicode_AsUTF8AndSize |
| 0.03% | python | unicode_encode_utf8 |
| 0.03% | python | stringlib_bytes_join.lto_priv.1 |
| 0.02% | python | _PyUnicode_FromASCII |
| 0.02% | python | resize_compact |
| 0.02% | python | unicode_startswith |
| 0.02% | python | unicode_split |
| 0.02% | python | PyUnicode_FromWideChar |
| 0.01% | python | unicode_repr |
| 0.01% | python | unicode_join |
| 0.01% | python | PyUnicode_DecodeFSDefault |
| 0.01% | python | bytes_decode |
| 0.01% | python | _PyUnicodeWriter_Init |
| 0.01% | python | _PyUnicodeWriter_Finish |
| 0.01% | python | PyBytes_Repr |
| 0.01% | python | bytes_richcompare |
| 0.01% | python | unicode_rstrip |
| 0.01% | python | _PyUnicode_IsAlpha |
| 0.01% | python | unicode_splitlines |
| 0.01% | python | unicode_endswith |
| 0.01% | python | unicode_find |
| 0.01% | python | unicode_rfind |
| 0.01% | python | _PyUnicode_IsLowercase |
| 0.01% | python | unicode_strip |
| 0.01% | python | _PyUnicode_TranslateCharmap |

### list

1.12% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.16% | python | list_subscript |
| 0.16% | python | list_ass_slice_lock_held |
| 0.15% | python | list_iter |
| 0.11% | python | list_resize |
| 0.07% | python | PyList_SetSlice |
| 0.06% | python | list_contains |
| 0.05% | python | list_sort_impl |
| 0.04% | python | list_append |
| 0.04% | python | list_vectorcall |
| 0.04% | python | PyList_Append |
| 0.04% | python | list_ass_subscript |
| 0.03% | python | list_concat |
| 0.03% | python | list_extend |
| 0.02% | python | listiter_next |
| 0.02% | python | _PyList_FromArraySteal |
| 0.02% | python | list_pop |
| 0.01% | python | PyList_Size |
| 0.01% | python | list_clear_impl.constprop.0 |
| 0.01% | python | _PyList_AppendTakeRefListResize |
| 0.01% | python | list_length |
| 0.01% | python | list_richcompare |

### tuple

1.09% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.49% | python | tuplehash |
| 0.19% | python | _PyTuple_FromArraySteal |
| 0.12% | python | tupletraverse |
| 0.07% | python | tuple_iter |
| 0.06% | python | tuplerichcompare |
| 0.05% | python | PyTuple_Pack |
| 0.03% | python | tuplecontains |
| 0.02% | python | _PyTuple_FromArray |
| 0.01% | python | tuplesubscript |
| 0.01% | python | tupleiter_next |
| 0.01% | python | _PyTuple_Resize |
| 0.01% | python | PyTuple_Size |

### lookup

1.08% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.31% | python | _Py_dict_lookup |
| 0.30% | python | find_name_in_mro |
| 0.25% | python | _Py_type_getattro |
| 0.17% | python | unicodekeys_lookup_unicode |
| 0.03% | python | builtin_getattr |
| 0.02% | python | _PyType_Lookup |

### miscobj

1.08% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.10% | python | PySlice_Unpack |
| 0.10% | python | set_issubset_impl |
| 0.09% | python | setiter_iternext |
| 0.09% | python | set_lookkey |
| 0.09% | python | PySlice_AdjustIndices |
| 0.07% | python | set_vectorcall |
| 0.06% | python | enum_next |
| 0.06% | python | set_contains_lock_held |
| 0.05% | python | set_difference |
| 0.05% | python | _PyBuildSlice_ConsumeRefs |
| 0.03% | python | set_add |
| 0.03% | python | deque_append_lock_held |
| 0.03% | python | dequeiter_next_lock_held.isra.0 |
| 0.03% | python | set_table_resize |
| 0.02% | python | set_add_entry |
| 0.02% | python | bytearray_ass_subscript |
| 0.01% | python | set_merge_lock_held.part.0 |
| 0.01% | python | deque_popleft_impl |
| 0.01% | python | set_intersection |
| 0.01% | python | PyBuffer_Release |
| 0.01% | python | deque_append_impl |
| 0.01% | python | deque_clear |
| 0.01% | python | _PySlice_GetLongIndices |
| 0.01% | python | set_iter |

### calls

0.90% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.31% | python | _PyFunction_Vectorcall |
| 0.12% | python | vgetargs1_impl |
| 0.07% | python | vectorcall_method |
| 0.07% | python | vgetargskeywords.constprop.0 |
| 0.05% | python | method_vectorcall_VARARGS |
| 0.04% | python | _PyArg_UnpackKeywords |
| 0.03% | python | method_vectorcall_VARARGS_KEYWORDS |
| 0.02% | python | cfunction_vectorcall_NOARGS |
| 0.02% | python | PyArg_UnpackTuple |
| 0.02% | python | cfunction_vectorcall_FASTCALL_KEYWORDS |
| 0.02% | python | cfunction_vectorcall_O |
| 0.02% | python | method_vectorcall_FASTCALL_KEYWORDS_METHOD |
| 0.02% | python | PyArg_ParseTuple |
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

0.44% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.15% | python | _PyErr_SetObject |
| 0.07% | python | PyTraceBack_Here |
| 0.06% | python | PyCode_Addr2Line |
| 0.04% | python | PyErr_GivenExceptionMatches |
| 0.03% | python | PyErr_ExceptionMatches |
| 0.02% | python | BaseException_init |
| 0.01% | python | PyErr_Occurred |
| 0.01% | python | PyErr_Format |
| 0.01% | python | AttributeError_init |

### float

0.41% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.17% | python | PyFloat_FromDouble |
| 0.09% | python | float_div |
| 0.04% | python | float_richcompare |
| 0.03% | python | PyFloat_AsDouble |
| 0.03% | python | float_mul |
| 0.02% | python | float_pow |
| 0.02% | python | float_sub |
| 0.01% | python | float_add |

### import

0.37% total

| percentage | object | symbol |
| ---: | :--- | :--- |
| 0.33% | python | r_object |
| 0.02% | python | PyImport_ImportModuleLevelObject |

### gil

0.00% total

| percentage | object | symbol |
| ---: | :--- | :--- |
