
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: incremental-gc
- commit hash: 14e3135
- commit date: 2024-01-07T13:17:57+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 39,940,066,094 | 18.7% | 18.7% |  |
| STORE_FAST | 13,900,197,289 | 6.5% | 25.2% |  |
| LOAD_CONST | 13,442,781,026 | 6.3% | 31.5% |  |
| POP_JUMP_IF_FALSE | 12,067,458,618 | 5.7% | 37.2% |  |
| LOAD_FAST_LOAD_FAST | 11,166,210,084 | 5.2% | 42.4% |  |
| RESUME_CHECK | 7,590,191,891 | 3.6% | 46.0% | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 5,669,196,364 | 2.7% | 48.7% | 5.1% |
| LOAD_GLOBAL_BUILTIN | 5,587,241,402 | 2.6% | 51.3% | 0.0% |
| TO_BOOL_BOOL | 4,721,732,146 | 2.2% | 53.5% | 0.0% |
| JUMP_BACKWARD | 4,575,415,192 | 2.1% | 55.6% |  |
| RETURN_VALUE | 4,372,433,232 | 2.1% | 57.7% |  |
| LOAD_GLOBAL_MODULE | 4,123,462,301 | 1.9% | 59.6% | 0.0% |
| CALL_PY_EXACT_ARGS | 3,927,648,943 | 1.8% | 61.5% | 2.7% |
| POP_TOP | 3,713,285,882 | 1.7% | 63.2% |  |
| BINARY_OP_ADD_INT | 2,975,960,607 | 1.4% | 64.6% | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,719,451,920 | 1.3% | 65.9% | 7.9% |
| CONTAINS_OP | 2,666,420,691 | 1.3% | 67.1% |  |
| STORE_FAST_STORE_FAST | 2,165,418,779 | 1.0% | 68.1% |  |
| LOAD_ATTR_SLOT | 2,162,778,141 | 1.0% | 69.2% | 5.1% |
| COMPARE_OP_STR | 2,124,311,138 | 1.0% | 70.2% | 0.0% |
| NOP | 2,053,471,345 | 1.0% | 71.1% |  |
| POP_JUMP_IF_TRUE | 2,019,353,460 | 0.9% | 72.1% |  |
| INTERPRETER_EXIT | 1,999,331,272 | 0.9% | 73.0% |  |
| RETURN_CONST | 1,979,684,849 | 0.9% | 73.9% |  |
| COMPARE_OP_INT | 1,974,161,893 | 0.9% | 74.9% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,959,707,928 | 0.9% | 75.8% | 2.1% |
| PUSH_NULL | 1,782,636,923 | 0.8% | 76.6% |  |
| FOR_ITER_LIST | 1,661,408,160 | 0.8% | 77.4% | 5.3% |
| BINARY_SUBSCR_STR_INT | 1,660,380,820 | 0.8% | 78.2% | 0.0% |
| LOAD_ATTR | 1,640,318,843 | 0.8% | 78.9% |  |
| STORE_ATTR_SLOT | 1,483,653,421 | 0.7% | 79.6% | 6.3% |
| BINARY_SUBSCR | 1,482,595,558 | 0.7% | 80.3% |  |
| COPY | 1,403,075,334 | 0.7% | 81.0% |  |
| YIELD_VALUE | 1,318,282,134 | 0.6% | 81.6% |  |
| CALL_BUILTIN_FAST | 1,302,667,539 | 0.6% | 82.2% | 0.0% |
| SWAP | 1,238,142,262 | 0.6% | 82.8% |  |
| BINARY_SUBSCR_LIST_INT | 1,193,620,498 | 0.6% | 83.4% | 0.4% |
| CALL_BUILTIN_O | 1,170,327,500 | 0.5% | 83.9% | 0.3% |
| STORE_ATTR_INSTANCE_VALUE | 1,130,440,752 | 0.5% | 84.4% | 8.8% |
| BINARY_OP | 1,127,225,742 | 0.5% | 85.0% |  |
| CALL | 1,112,452,683 | 0.5% | 85.5% |  |
| LOAD_DEREF | 1,107,983,290 | 0.5% | 86.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 1,103,707,382 | 0.5% | 86.5% | 0.8% |
| CALL_ISINSTANCE | 1,048,257,360 | 0.5% | 87.0% |  |
| BUILD_TUPLE | 977,208,930 | 0.5% | 87.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 901,430,243 | 0.4% | 87.9% |  |
| IS_OP | 836,547,855 | 0.4% | 88.3% |  |
| GET_ITER | 808,530,097 | 0.4% | 88.7% |  |
| BINARY_SUBSCR_DICT | 796,198,503 | 0.4% | 89.0% |  |
| FOR_ITER_RANGE | 713,100,077 | 0.3% | 89.4% | 0.0% |
| SEND_GEN | 702,483,219 | 0.3% | 89.7% | 0.0% |
| POP_JUMP_IF_NOT_NONE | 675,806,420 | 0.3% | 90.0% |  |
| BINARY_OP_SUBTRACT_INT | 658,476,282 | 0.3% | 90.3% | 0.1% |
| TO_BOOL_NONE | 624,072,696 | 0.3% | 90.6% | 9.8% |
| JUMP_FORWARD | 603,632,439 | 0.3% | 90.9% |  |
| UNPACK_SEQUENCE_TUPLE | 591,098,228 | 0.3% | 91.2% | 0.3% |
| FOR_ITER_TUPLE | 582,389,595 | 0.3% | 91.4% | 15.0% |
| LOAD_ATTR_MODULE | 575,528,971 | 0.3% | 91.7% | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 546,382,839 | 0.3% | 92.0% |  |
| BINARY_OP_ADD_FLOAT | 525,720,855 | 0.2% | 92.2% | 1.6% |
| FOR_ITER | 492,436,220 | 0.2% | 92.5% |  |
| CALL_TYPE_1 | 475,459,770 | 0.2% | 92.7% |  |
| POP_JUMP_IF_NONE | 467,437,310 | 0.2% | 92.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 465,801,003 | 0.2% | 93.1% | 8.8% |
| EXTENDED_ARG | 458,752,381 | 0.2% | 93.3% |  |
| CALL_LEN | 447,772,119 | 0.2% | 93.5% |  |
| LOAD_ATTR_WITH_HINT | 447,530,230 | 0.2% | 93.7% | 0.5% |
| STORE_SUBSCR | 440,854,509 | 0.2% | 94.0% |  |
| BUILD_LIST | 438,355,145 | 0.2% | 94.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 433,229,996 | 0.2% | 94.4% | 6.4% |
| STORE_SUBSCR_LIST_INT | 424,102,211 | 0.2% | 94.6% | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 412,811,117 | 0.2% | 94.8% | 0.1% |
| RETURN_GENERATOR | 394,766,048 | 0.2% | 94.9% |  |
| BINARY_OP_SUBTRACT_FLOAT | 360,442,564 | 0.2% | 95.1% | 5.6% |
| BINARY_OP_MULTIPLY_INT | 357,991,801 | 0.2% | 95.3% | 3.2% |
| TO_BOOL | 348,292,849 | 0.2% | 95.4% |  |
| COPY_FREE_VARS | 346,957,105 | 0.2% | 95.6% |  |
| TO_BOOL_INT | 329,153,705 | 0.2% | 95.8% | 0.4% |
| CALL_LIST_APPEND | 328,683,867 | 0.2% | 95.9% | 0.0% |
| BINARY_SLICE | 325,359,870 | 0.2% | 96.1% |  |
| END_SEND | 314,295,672 | 0.1% | 96.2% |  |
| BINARY_SUBSCR_TUPLE_INT | 305,787,583 | 0.1% | 96.4% | 0.0% |
| STORE_SUBSCR_DICT | 270,251,457 | 0.1% | 96.5% |  |
| CALL_INTRINSIC_1 | 249,719,566 | 0.1% | 96.6% |  |
| CALL_KW | 243,697,021 | 0.1% | 96.7% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 236,870,464 | 0.1% | 96.8% | 16.0% |
| TO_BOOL_ALWAYS_TRUE | 236,602,833 | 0.1% | 96.9% | 23.7% |
| COMPARE_OP_FLOAT | 220,291,893 | 0.1% | 97.0% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 217,876,676 | 0.1% | 97.1% | 3.1% |
| FOR_ITER_GEN | 217,205,184 | 0.1% | 97.2% | 0.0% |
| BUILD_SLICE | 211,807,816 | 0.1% | 97.3% |  |
| COMPARE_OP | 206,041,520 | 0.1% | 97.4% |  |
| BINARY_SUBSCR_GETITEM | 193,972,460 | 0.1% | 97.5% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 192,505,732 | 0.1% | 97.6% | 35.5% |
| LIST_APPEND | 187,777,308 | 0.1% | 97.7% |  |
| CALL_FUNCTION_EX | 186,719,875 | 0.1% | 97.8% |  |
| CALL_BUILTIN_CLASS | 182,669,689 | 0.1% | 97.9% | 0.0% |
| UNPACK_SEQUENCE_LIST | 179,426,846 | 0.1% | 98.0% | 0.7% |
| DELETE_SUBSCR | 177,698,591 | 0.1% | 98.0% |  |
| TO_BOOL_LIST | 177,642,193 | 0.1% | 98.1% | 0.9% |
| LOAD_ATTR_CLASS | 176,658,758 | 0.1% | 98.2% | 0.9% |
| SEND | 165,323,755 | 0.1% | 98.3% |  |
| STORE_FAST_LOAD_FAST | 161,601,325 | 0.1% | 98.4% |  |
| UNARY_NEGATIVE | 161,340,369 | 0.1% | 98.4% |  |
| STORE_SLICE | 156,895,629 | 0.1% | 98.5% |  |
| GET_AWAITABLE | 152,094,592 | 0.1% | 98.6% |  |
| FORMAT_SIMPLE | 151,434,257 | 0.1% | 98.7% |  |
| CONVERT_VALUE | 139,481,612 | 0.1% | 98.7% |  |
| MAKE_FUNCTION | 136,630,831 | 0.1% | 98.8% |  |
| GET_ANEXT | 133,515,680 | 0.1% | 98.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 125,521,767 | 0.1% | 98.9% | 0.0% |
| LIST_EXTEND | 125,228,706 | 0.1% | 99.0% |  |
| BUILD_MAP | 122,768,085 | 0.1% | 99.0% |  |
| LOAD_SUPER_ATTR_METHOD | 122,439,328 | 0.1% | 99.1% |  |
| SET_FUNCTION_ATTRIBUTE | 119,485,278 | 0.1% | 99.1% |  |
| MAKE_CELL | 104,671,316 | 0.0% | 99.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 104,538,701 | 0.0% | 99.2% | 2.2% |
| BINARY_OP_ADD_UNICODE | 96,720,540 | 0.0% | 99.3% | 0.0% |
| STORE_DEREF | 94,102,882 | 0.0% | 99.3% |  |
| CALL_ALLOC_AND_ENTER_INIT | 92,003,392 | 0.0% | 99.4% | 2.5% |
| EXIT_INIT_CHECK | 89,720,112 | 0.0% | 99.4% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 87,800,575 | 0.0% | 99.5% | 19.4% |
| TO_BOOL_STR | 86,213,024 | 0.0% | 99.5% | 3.9% |
| LOAD_ATTR_PROPERTY | 82,254,374 | 0.0% | 99.5% | 12.8% |
| END_FOR | 76,080,152 | 0.0% | 99.6% |  |
| BUILD_STRING | 76,066,392 | 0.0% | 99.6% |  |
| CALL_STR_1 | 74,887,620 | 0.0% | 99.6% |  |
| LOAD_FAST_AND_CLEAR | 72,533,766 | 0.0% | 99.7% |  |
| UNARY_NOT | 70,025,331 | 0.0% | 99.7% |  |
| STORE_ATTR | 67,394,243 | 0.0% | 99.7% |  |
| STORE_ATTR_WITH_HINT | 67,119,097 | 0.0% | 99.8% | 0.1% |
| LOAD_ATTR_METHOD_LAZY_DICT | 62,472,392 | 0.0% | 99.8% | 0.0% |
| MAP_ADD | 47,756,667 | 0.0% | 99.8% |  |
| DICT_MERGE | 43,228,254 | 0.0% | 99.8% |  |
| GET_YIELD_FROM_ITER | 36,719,752 | 0.0% | 99.9% |  |
| CALL_TUPLE_1 | 25,012,175 | 0.0% | 99.9% | 0.0% |
| PUSH_EXC_INFO | 21,553,062 | 0.0% | 99.9% |  |
| POP_EXCEPT | 21,552,915 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 20,929,449 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 15,184,677 | 0.0% | 99.9% |  |
| LOAD_NAME | 14,047,720 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,092,227 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 11,316,505 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 10,840,682 | 0.0% | 100.0% |  |
| IMPORT_FROM | 10,431,153 | 0.0% | 100.0% |  |
| IMPORT_NAME | 9,412,655 | 0.0% | 100.0% |  |
| BEFORE_WITH | 9,032,316 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 8,205,000 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,824,720 | 0.0% | 100.0% | 0.0% |
| DELETE_ATTR | 5,735,951 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,404 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,710,400 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,614,290 | 0.0% | 100.0% |  |
| SET_ADD | 2,273,600 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,069,069 | 0.0% | 100.0% |  |
| BUILD_SET | 1,667,755 | 0.0% | 100.0% |  |
| STORE_NAME | 980,120 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,520 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 319,651 | 0.0% | 100.0% |  |
| RESUME | 271,342 | 0.0% | 100.0% | 62.7% |
| WITH_EXCEPT_START | 184,300 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 65,189 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,343 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,428 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,268 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,988 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| DELETE_DEREF | 1,600 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,520 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 1,520 | 0.0% | 100.0% |  |
| DELETE_NAME | 900 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NONE | 720 | 0.0% | 100.0% |  |
| SETUP_ANNOTATIONS | 540 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_FORWARD | 400 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NOT_NONE | 400 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_2 | 80 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| STORE_FAST LOAD_FAST | 6,886,811,645 | 3.2% | 3.2% |
| LOAD_FAST LOAD_CONST | 6,695,781,968 | 3.1% | 6.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 6,600,922,964 | 3.1% | 9.5% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 4,911,583,662 | 2.3% | 11.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,611,927,971 | 1.7% | 13.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 3,533,840,281 | 1.7% | 15.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 3,473,560,669 | 1.6% | 16.7% |
| RESUME_CHECK LOAD_FAST | 3,159,423,794 | 1.5% | 18.2% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 2,508,951,289 | 1.2% | 19.4% |
| LOAD_CONST BINARY_OP_ADD_INT | 2,387,671,366 | 1.1% | 20.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 2,262,452,411 | 1.1% | 21.6% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 2,087,403,068 | 1.0% | 22.6% |
| LOAD_CONST COMPARE_OP_STR | 2,083,452,032 | 1.0% | 23.5% |
| LOAD_FAST LOAD_ATTR_SLOT | 2,030,693,934 | 1.0% | 24.5% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,833,078,049 | 0.9% | 25.4% |
| CACHE RESUME_CHECK | 1,695,835,832 | 0.8% | 26.1% |
| BINARY_OP_ADD_INT STORE_FAST | 1,684,845,078 | 0.8% | 26.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,660,804,486 | 0.8% | 27.7% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,627,293,648 | 0.8% | 28.5% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 1,602,967,280 | 0.8% | 29.2% |
| LOAD_CONST LOAD_FAST | 1,481,726,195 | 0.7% | 29.9% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,480,552,267 | 0.7% | 30.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,412,041,392 | 0.7% | 31.3% |
| POP_TOP LOAD_FAST | 1,411,467,394 | 0.7% | 31.9% |
| LOAD_FAST_LOAD_FAST CONTAINS_OP | 1,340,419,685 | 0.6% | 32.6% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 1,311,026,450 | 0.6% | 33.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,287,687,272 | 0.6% | 33.8% |
| NOP LOAD_FAST_LOAD_FAST | 1,280,393,528 | 0.6% | 34.4% |
| JUMP_BACKWARD FOR_ITER_LIST | 1,255,806,503 | 0.6% | 35.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,253,931,882 | 0.6% | 35.6% |
| STORE_FAST JUMP_BACKWARD | 1,242,381,476 | 0.6% | 36.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,232,938,897 | 0.6% | 36.7% |
| LOAD_FAST RETURN_VALUE | 1,232,668,857 | 0.6% | 37.3% |
| BINARY_SUBSCR_STR_INT STORE_FAST | 1,129,317,920 | 0.5% | 37.8% |
| LOAD_CONST LOAD_CONST | 1,103,410,333 | 0.5% | 38.4% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 1,097,397,591 | 0.5% | 38.9% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,087,543,618 | 0.5% | 39.4% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 1,053,109,539 | 0.5% | 39.9% |
| LOAD_FAST LOAD_FAST | 1,036,567,796 | 0.5% | 40.4% |
| POP_TOP JUMP_BACKWARD | 1,034,636,391 | 0.5% | 40.8% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 1,026,426,748 | 0.5% | 41.3% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,017,110,177 | 0.5% | 41.8% |
| LOAD_FAST TO_BOOL_BOOL | 990,299,025 | 0.5% | 42.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 976,247,126 | 0.5% | 42.7% |
| LOAD_FAST PUSH_NULL | 967,059,054 | 0.5% | 43.2% |
| JUMP_BACKWARD NOP | 957,351,878 | 0.4% | 43.6% |
| STORE_FAST STORE_FAST | 956,472,476 | 0.4% | 44.1% |
| RETURN_VALUE STORE_FAST | 941,120,788 | 0.4% | 44.5% |
| LOAD_FAST LOAD_ATTR | 932,573,410 | 0.4% | 45.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 912,338,479 | 0.4% | 45.4% |
| LOAD_CONST COMPARE_OP_INT | 870,995,992 | 0.4% | 45.8% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 862,534,967 | 0.4% | 46.2% |
| POP_JUMP_IF_TRUE LOAD_FAST | 855,970,746 | 0.4% | 46.6% |
| PUSH_NULL LOAD_FAST | 833,346,981 | 0.4% | 47.0% |
| RETURN_CONST POP_TOP | 833,267,712 | 0.4% | 47.4% |
| LOAD_FAST CALL_BUILTIN_O | 803,599,936 | 0.4% | 47.8% |
| FOR_ITER_LIST STORE_FAST | 803,037,934 | 0.4% | 48.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 779,865,242 | 0.4% | 48.5% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 761,594,514 | 0.4% | 48.9% |
| RESUME_CHECK POP_TOP | 758,690,460 | 0.4% | 49.2% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 753,953,298 | 0.4% | 49.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 734,525,088 | 0.3% | 49.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 720,348,317 | 0.3% | 50.2% |
| LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 718,883,480 | 0.3% | 50.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 703,645,561 | 0.3% | 50.9% |
| IS_OP POP_JUMP_IF_FALSE | 695,219,592 | 0.3% | 51.2% |
| RETURN_VALUE RETURN_VALUE | 676,690,116 | 0.3% | 51.6% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 674,155,233 | 0.3% | 51.9% |
| RETURN_CONST INTERPRETER_EXIT | 673,819,931 | 0.3% | 52.2% |
| LOAD_DEREF LOAD_FAST | 669,144,190 | 0.3% | 52.5% |
| LOAD_FAST STORE_ATTR_SLOT | 665,829,345 | 0.3% | 52.8% |
| LOAD_FAST CONTAINS_OP | 662,429,606 | 0.3% | 53.1% |
| BINARY_SUBSCR LOAD_FAST | 659,636,140 | 0.3% | 53.4% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 654,393,208 | 0.3% | 53.7% |
| YIELD_VALUE INTERPRETER_EXIT | 647,600,421 | 0.3% | 54.0% |
| STORE_FAST_STORE_FAST LOAD_FAST | 646,392,938 | 0.3% | 54.3% |
| JUMP_BACKWARD FOR_ITER_RANGE | 642,157,523 | 0.3% | 54.6% |
| POP_JUMP_IF_FALSE JUMP_BACKWARD | 639,354,180 | 0.3% | 54.9% |
| LOAD_CONST STORE_FAST | 632,068,223 | 0.3% | 55.2% |
| RETURN_VALUE INTERPRETER_EXIT | 631,228,003 | 0.3% | 55.5% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 624,747,876 | 0.3% | 55.8% |
| POP_JUMP_IF_TRUE JUMP_BACKWARD | 623,002,831 | 0.3% | 56.1% |
| FOR_ITER_RANGE STORE_FAST | 617,766,289 | 0.3% | 56.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 591,640,693 | 0.3% | 56.7% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 579,374,340 | 0.3% | 57.0% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 577,917,437 | 0.3% | 57.2% |
| NOP LOAD_FAST | 577,175,170 | 0.3% | 57.5% |
| BUILD_TUPLE RETURN_VALUE | 560,660,923 | 0.3% | 57.8% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 558,609,239 | 0.3% | 58.0% |
| STORE_FAST LOAD_GLOBAL_MODULE | 554,380,794 | 0.3% | 58.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 552,132,903 | 0.3% | 58.5% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 546,685,733 | 0.3% | 58.8% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,413,015 | 0.3% | 59.1% |
| YIELD_VALUE YIELD_VALUE | 529,559,801 | 0.2% | 59.3% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,540,261 | 0.2% | 59.6% |
| SEND_GEN RESUME_CHECK | 529,524,133 | 0.2% | 59.8% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 522,830,338 | 0.2% | 60.0% |
| BINARY_SUBSCR_STR_INT LOAD_FAST | 517,397,860 | 0.2% | 60.3% |
| CALL_BUILTIN_O POP_TOP | 516,285,204 | 0.2% | 60.5% |
| RESUME_CHECK NOP | 515,599,714 | 0.2% | 60.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 182,061,341 | 56.0% |
| LOAD_FAST_LOAD_FAST | 53,317,680 | 16.4% |
| BINARY_OP_ADD_INT | 48,047,729 | 14.8% |
| LOAD_FAST | 34,312,120 | 10.5% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 70,800,923 | 21.8% |
| GET_ITER | 44,478,160 | 13.7% |
| CALL_PY_EXACT_ARGS | 33,475,250 | 10.3% |
| BUILD_TUPLE | 32,311,140 | 9.9% |
| CALL_LIST_APPEND | 25,775,289 | 7.9% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 138,548,820 | 88.3% |
| LOAD_CONST | 17,991,409 | 11.5% |
| LOAD_FAST_LOAD_FAST | 344,480 | 0.2% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,483,729 | 91.5% |
| RETURN_CONST | 7,807,680 | 5.0% |
| LOAD_FAST_LOAD_FAST | 5,542,720 | 3.5% |
| JUMP_BACKWARD | 56,300 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,695,835,832 | 84.7% |
| POP_TOP | 145,620,625 | 7.3% |
| COPY_FREE_VARS | 112,292,195 | 5.6% |
| RETURN_GENERATOR | 46,669,797 | 2.3% |
| MAKE_CELL | 1,969,514 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,351,087 | 70.3% |
| RETURN_VALUE | 1,934,995 | 21.4% |
| LOAD_GLOBAL_MODULE | 282,042 | 3.1% |
| LOAD_FAST | 193,540 | 2.1% |
| LOAD_ATTR_WITH_HINT | 176,480 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,370,401 | 92.7% |
| STORE_FAST | 659,995 | 7.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,490,620 | 44.6% |
| BINARY_SLICE | 2,107,400 | 26.9% |
| RETURN_VALUE | 810,480 | 10.4% |
| LOAD_ATTR_SLOT | 478,280 | 6.1% |
| BINARY_OP_ADD_UNICODE | 469,140 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,086,020 | 90.6% |
| JUMP_BACKWARD | 600,120 | 7.7% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 470,539,267 | 31.7% |
| LOAD_FAST_LOAD_FAST | 318,484,482 | 21.5% |
| LOAD_CONST | 173,775,247 | 11.7% |
| COPY | 146,304,522 | 9.9% |
| BUILD_SLICE | 140,574,746 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 659,636,140 | 44.5% |
| STORE_FAST | 165,043,415 | 11.1% |
| LOAD_FAST_LOAD_FAST | 146,949,928 | 9.9% |
| BINARY_OP_MULTIPLY_FLOAT | 90,267,920 | 6.1% |
| BINARY_SUBSCR | 64,435,634 | 4.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,165,828 | 91.6% |
| LOAD_GLOBAL_MODULE | 998,524 | 4.8% |
| BUILD_TUPLE | 629,268 | 3.0% |
| LOAD_ATTR_MODULE | 129,557 | 0.6% |
| LOAD_GLOBAL | 4,264 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,929,129 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,759 | 54.9% |
| BUILD_SLICE | 71,229,230 | 40.1% |
| LOAD_CONST | 7,393,880 | 4.2% |
| LOAD_FAST | 1,355,705 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,443,323 | 80.8% |
| LOAD_CONST | 24,226,765 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| JUMP_BACKWARD | 1,438,740 | 0.8% |
| RETURN_CONST | 720,390 | 0.4% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 89,720,112 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 89,720,112 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 139,481,612 | 92.1% |
| LOAD_FAST | 5,743,807 | 3.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.3% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.0% |
| RETURN_VALUE | 1,182,860 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 76,493,041 | 50.5% |
| BUILD_STRING | 67,713,067 | 44.7% |
| LOAD_FAST | 7,216,269 | 4.8% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 295,082,302 | 36.5% |
| LOAD_ATTR_INSTANCE_VALUE | 91,105,566 | 11.3% |
| CALL_BUILTIN_CLASS | 79,001,148 | 9.8% |
| RETURN_VALUE | 74,959,763 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 58,891,479 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 242,863,784 | 30.0% |
| FOR_ITER_TUPLE | 168,441,600 | 20.8% |
| CALL_PY_EXACT_ARGS | 123,843,978 | 15.3% |
| FOR_ITER | 91,067,096 | 11.3% |
| FOR_ITER_GEN | 75,660,465 | 9.4% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 673,819,931 | 33.7% |
| YIELD_VALUE | 647,600,421 | 32.4% |
| RETURN_VALUE | 631,228,003 | 31.6% |
| RETURN_GENERATOR | 46,682,597 | 2.3% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 136,630,831 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 118,626,671 | 86.8% |
| LOAD_FAST | 10,360,084 | 7.6% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 2.4% |
| LOAD_GLOBAL_BUILTIN | 2,695,725 | 2.0% |
| STORE_FAST | 815,677 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 957,351,878 | 46.6% |
| RESUME_CHECK | 515,599,714 | 25.1% |
| STORE_FAST | 206,898,228 | 10.1% |
| POP_JUMP_IF_FALSE | 105,128,374 | 5.1% |
| STORE_ATTR_INSTANCE_VALUE | 72,209,693 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,280,393,528 | 62.4% |
| LOAD_FAST | 577,175,170 | 28.1% |
| NOP | 70,779,359 | 3.4% |
| LOAD_GLOBAL_BUILTIN | 45,141,228 | 2.2% |
| LOAD_GLOBAL_MODULE | 24,544,229 | 1.2% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,116,954 | 56.2% |
| STORE_SUBSCR_DICT | 4,109,621 | 19.1% |
| SWAP | 2,569,665 | 11.9% |
| COPY | 1,590,410 | 7.4% |
| STORE_FAST | 867,980 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,233,135 | 52.1% |
| RETURN_VALUE | 2,490,065 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.7% |
| POP_TOP | 1,847,200 | 8.6% |
| RERAISE | 1,590,410 | 7.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 833,267,712 | 22.4% |
| RESUME_CHECK | 758,690,460 | 20.4% |
| CALL_BUILTIN_O | 516,285,204 | 13.9% |
| CALL_METHOD_DESCRIPTOR_O | 265,880,992 | 7.2% |
| POP_JUMP_IF_FALSE | 218,378,139 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,411,467,394 | 38.0% |
| JUMP_BACKWARD | 1,034,636,391 | 27.9% |
| RESUME_CHECK | 394,748,560 | 10.6% |
| RETURN_CONST | 303,745,289 | 8.2% |
| LOAD_CONST | 147,981,675 | 4.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 7,184,277 | 33.3% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,116,904 | 14.5% |
| RERAISE | 1,383,620 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,640 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,272,226 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,568,940 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,300 | 0.9% |
| LOAD_GLOBAL | 9,556 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 967,059,054 | 54.2% |
| LOAD_ATTR_MODULE | 475,606,311 | 26.7% |
| LOAD_ATTR | 155,839,774 | 8.7% |
| LOAD_DEREF | 69,294,143 | 3.9% |
| LOAD_FAST_LOAD_FAST | 63,660,885 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 833,346,981 | 46.7% |
| LOAD_FAST_LOAD_FAST | 464,097,599 | 26.0% |
| LOAD_CONST | 262,264,945 | 14.7% |
| CALL | 106,284,524 | 6.0% |
| LOAD_GLOBAL_MODULE | 48,344,756 | 2.7% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 228,352,193 | 57.8% |
| COPY_FREE_VARS | 107,553,577 | 27.2% |
| CACHE | 46,669,797 | 11.8% |
| CALL_PY_WITH_DEFAULTS | 8,944,785 | 2.3% |
| CALL_FUNCTION_EX | 1,146,640 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,265,626 | 33.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 64,521,680 | 16.3% |
| GET_ITER | 50,227,600 | 12.7% |
| INTERPRETER_EXIT | 46,682,597 | 11.8% |
| STORE_FAST | 28,700,978 | 7.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,232,668,857 | 28.2% |
| RETURN_VALUE | 676,690,116 | 15.5% |
| BUILD_TUPLE | 560,660,923 | 12.8% |
| LOAD_ATTR_INSTANCE_VALUE | 322,939,625 | 7.4% |
| BINARY_SUBSCR_DICT | 136,219,539 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 941,120,788 | 21.5% |
| RETURN_VALUE | 676,690,116 | 15.5% |
| INTERPRETER_EXIT | 631,228,003 | 14.4% |
| TO_BOOL_BOOL | 393,504,498 | 9.0% |
| UNPACK_SEQUENCE_TUPLE | 344,983,712 | 7.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 146,314,802 | 33.2% |
| LOAD_FAST | 89,520,784 | 20.3% |
| LOAD_FAST_LOAD_FAST | 77,543,700 | 17.6% |
| BINARY_OP_ADD_INT | 55,376,200 | 12.6% |
| LOAD_CONST | 51,107,206 | 11.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 150,803,320 | 34.2% |
| LOAD_FAST_LOAD_FAST | 139,462,160 | 31.6% |
| RETURN_CONST | 48,411,764 | 11.0% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 8.2% |
| LOAD_FAST | 32,702,664 | 7.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 235,971,585 | 67.8% |
| LOAD_ATTR_INSTANCE_VALUE | 85,805,121 | 24.6% |
| CALL_BUILTIN_FAST | 10,290,912 | 3.0% |
| LOAD_ATTR | 5,298,256 | 1.5% |
| LOAD_ATTR_SLOT | 3,122,440 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 198,894,140 | 57.1% |
| POP_JUMP_IF_FALSE | 148,132,450 | 42.5% |
| TO_BOOL | 466,884 | 0.1% |
| UNARY_NOT | 234,613 | 0.1% |
| TO_BOOL_NONE | 194,931 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,085,932 | 92.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 502,738 | 3.3% |
| LOAD_ATTR_MODULE | 407,407 | 2.7% |
| LOAD_FAST | 175,180 | 1.2% |
| LOAD_FAST_LOAD_FAST | 12,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 15,184,557 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,550,873 | 89.0% |
| LOAD_FAST_LOAD_FAST | 10,670,188 | 6.6% |
| LOAD_GLOBAL_MODULE | 4,067,195 | 2.5% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.0% |
| CALL_LEN | 482,260 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 65.3% |
| BINARY_SUBSCR_LIST_INT | 35,691,400 | 22.1% |
| CALL_PY_EXACT_ARGS | 4,211,600 | 2.6% |
| BINARY_SUBSCR | 3,225,560 | 2.0% |
| STORE_SUBSCR | 3,225,520 | 2.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 61,414,094 | 87.7% |
| COMPARE_OP | 3,442,615 | 4.9% |
| TO_BOOL_LIST | 2,930,546 | 4.2% |
| TO_BOOL_INT | 1,348,783 | 1.9% |
| TO_BOOL_STR | 615,440 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 38,202,056 | 54.6% |
| RETURN_VALUE | 21,002,589 | 30.0% |
| LOAD_CONST | 7,078,772 | 10.1% |
| STORE_FAST | 1,425,174 | 2.0% |
| CALL_PY_EXACT_ARGS | 1,006,200 | 1.4% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 297,231,567 | 26.4% |
| LOAD_FAST | 235,669,542 | 20.9% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 8.5% |
| LOAD_FAST_LOAD_FAST | 75,621,767 | 6.7% |
| LOAD_ATTR_INSTANCE_VALUE | 58,711,780 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 223,265,680 | 19.8% |
| LOAD_FAST | 185,921,257 | 16.5% |
| LOAD_FAST_LOAD_FAST | 142,460,932 | 12.6% |
| RETURN_VALUE | 98,566,143 | 8.7% |
| LOAD_CONST | 92,401,264 | 8.2% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,092,227 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,302 | 41.8% |
| LOAD_FAST | 3,580,829 | 27.4% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.4% |
| STORE_FAST | 766,385 | 5.9% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 150,686,645 | 34.4% |
| LOAD_ATTR_SLOT | 99,799,425 | 22.8% |
| LOAD_FAST | 45,988,137 | 10.5% |
| SWAP | 35,426,701 | 8.1% |
| RESUME_CHECK | 19,399,801 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 172,693,459 | 39.4% |
| STORE_FAST | 168,923,956 | 38.5% |
| SWAP | 35,466,190 | 8.1% |
| RETURN_VALUE | 11,450,586 | 2.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 11,046,306 | 2.5% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,520,515 | 25.7% |
| BUILD_TUPLE | 15,370,802 | 12.5% |
| STORE_FAST | 14,570,976 | 11.9% |
| SWAP | 12,489,089 | 10.2% |
| RESUME_CHECK | 9,880,515 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,256,188 | 41.8% |
| STORE_FAST | 34,059,419 | 27.7% |
| SWAP | 12,489,089 | 10.2% |
| CALL_FUNCTION_EX | 9,564,361 | 7.8% |
| CALL_BUILTIN_FAST | 5,768,772 | 4.7% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,627,059 | 99.4% |
| LOAD_FAST | 1,105,477 | 0.5% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.0% |
| BINARY_OP_ADD_INT | 3,240 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 140,574,746 | 66.4% |
| DELETE_SUBSCR | 71,229,230 | 33.6% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 67,713,067 | 89.0% |
| LOAD_CONST | 8,353,325 | 11.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 48,913,080 | 64.3% |
| CALL | 15,922,100 | 20.9% |
| STORE_FAST | 4,417,278 | 5.8% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 3.5% |
| CALL_LIST_APPEND | 1,864,080 | 2.5% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 306,613,523 | 31.4% |
| LOAD_CONST | 223,702,909 | 22.9% |
| LOAD_FAST_LOAD_FAST | 202,148,423 | 20.7% |
| CALL | 50,201,691 | 5.1% |
| LOAD_GLOBAL_BUILTIN | 37,945,642 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 560,660,923 | 57.4% |
| LOAD_CONST | 119,255,791 | 12.2% |
| YIELD_VALUE | 42,832,960 | 4.4% |
| CALL_ISINSTANCE | 42,623,198 | 4.4% |
| BINARY_SUBSCR_GETITEM | 38,415,920 | 3.9% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 334,039,162 | 30.0% |
| LOAD_FAST_LOAD_FAST | 173,689,036 | 15.6% |
| PUSH_NULL | 106,284,524 | 9.6% |
| BINARY_SUBSCR_TUPLE_INT | 96,082,463 | 8.6% |
| LOAD_ATTR | 83,064,939 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 454,177,828 | 40.8% |
| RESUME_CHECK | 186,258,989 | 16.7% |
| POP_TOP | 90,739,728 | 8.2% |
| LOAD_GLOBAL_MODULE | 56,354,750 | 5.1% |
| RETURN_VALUE | 50,279,005 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 106,213,042 | 56.9% |
| DICT_MERGE | 43,228,254 | 23.2% |
| LOAD_FAST | 23,188,190 | 12.4% |
| BUILD_MAP | 9,564,361 | 5.1% |
| STORE_FAST | 3,083,376 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,989,354 | 58.9% |
| STORE_FAST | 28,334,731 | 15.2% |
| RESUME_CHECK | 21,338,302 | 11.4% |
| RETURN_VALUE | 7,520,123 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 124,151,316 | 49.7% |
| LOAD_FAST | 117,515,680 | 47.1% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 3.2% |
| RERAISE | 35,010 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 50.3% |
| CALL_FUNCTION_EX | 106,213,042 | 42.5% |
| LOAD_CONST | 9,378,761 | 3.8% |
| BUILD_MAP | 8,541,933 | 3.4% |
| RERAISE | 35,330 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 243,697,021 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,740,871 | 49.5% |
| STORE_FAST | 64,291,014 | 26.4% |
| RETURN_VALUE | 24,398,133 | 10.0% |
| POP_TOP | 7,446,148 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 64,079,828 | 31.1% |
| LOAD_CONST | 58,662,935 | 28.5% |
| LOAD_FAST | 23,329,920 | 11.3% |
| LOAD_ATTR | 20,936,318 | 10.2% |
| LOAD_GLOBAL_MODULE | 9,681,400 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 114,022,804 | 55.3% |
| POP_JUMP_IF_TRUE | 53,246,258 | 25.8% |
| COPY | 16,400,358 | 8.0% |
| BINARY_OP | 6,162,440 | 3.0% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 3.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,340,419,685 | 50.3% |
| LOAD_FAST | 662,429,606 | 24.8% |
| LOAD_GLOBAL_MODULE | 413,154,831 | 15.5% |
| BINARY_SUBSCR_DICT | 103,692,020 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 54,650,548 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,508,951,289 | 94.1% |
| POP_JUMP_IF_TRUE | 88,203,684 | 3.3% |
| RETURN_VALUE | 33,077,360 | 1.2% |
| COPY | 28,252,780 | 1.1% |
| EXTENDED_ARG | 4,591,720 | 0.2% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 116,182,320 | 83.3% |
| LOAD_ATTR | 15,441,320 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 1.9% |
| RETURN_VALUE | 2,058,840 | 1.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,847,420 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 139,481,612 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 361,171,077 | 25.7% |
| LOAD_FAST | 306,542,549 | 21.8% |
| LOAD_FAST_LOAD_FAST | 162,157,520 | 11.6% |
| SWAP | 139,461,850 | 9.9% |
| LOAD_CONST | 128,778,351 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 361,171,077 | 25.7% |
| TO_BOOL_BOOL | 294,574,429 | 21.0% |
| BINARY_SUBSCR_LIST_INT | 211,995,640 | 15.1% |
| BINARY_SUBSCR | 146,304,522 | 10.4% |
| COMPARE_OP_INT | 135,328,947 | 9.6% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 171,429,250 | 49.4% |
| CACHE | 112,292,195 | 32.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 37,082,760 | 10.7% |
| CALL_PY_WITH_DEFAULTS | 6,562,843 | 1.9% |
| CALL | 6,530,961 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 239,280,734 | 69.0% |
| RETURN_GENERATOR | 107,553,577 | 31.0% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,234 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,551 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,834 | 77.9% |
| NOP | 1,145,760 | 20.0% |
| RETURN_CONST | 117,237 | 2.0% |
| PUSH_EXC_INFO | 1,600 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,063,526 | 97.3% |
| RETURN_VALUE | 502,240 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 291,729 | 0.7% |
| LOAD_DEREF | 270,570 | 0.6% |
| LOAD_GLOBAL_MODULE | 40,589 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 43,228,254 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,589 | 62.3% |
| LOAD_FAST | 17,520 | 26.9% |
| MAP_ADD | 4,920 | 7.5% |
| BUILD_MAP | 760 | 1.2% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,329 | 63.4% |
| DICT_MERGE | 17,520 | 26.9% |
| BUILD_MAP | 4,380 | 6.7% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,310,606 | 23.8% |
| JUMP_BACKWARD | 95,660,560 | 20.9% |
| LOAD_FAST | 57,740,960 | 12.6% |
| CALL_LIST_APPEND | 41,464,738 | 9.0% |
| POP_TOP | 32,608,740 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 166,392,534 | 36.3% |
| JUMP_BACKWARD | 100,546,294 | 21.9% |
| FOR_ITER_LIST | 55,462,030 | 12.1% |
| POP_JUMP_IF_NONE | 48,769,366 | 10.6% |
| FOR_ITER_GEN | 34,775,860 | 7.6% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 348,780,877 | 70.8% |
| GET_ITER | 91,067,096 | 18.5% |
| EXTENDED_ARG | 24,256,720 | 4.9% |
| SWAP | 16,242,169 | 3.3% |
| LOAD_FAST | 11,784,401 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 263,452,433 | 53.5% |
| STORE_FAST | 121,348,534 | 24.6% |
| LOAD_FAST | 39,101,932 | 7.9% |
| RETURN_CONST | 22,898,286 | 4.7% |
| SWAP | 15,549,269 | 3.2% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,412,635 | 100.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,923,479 | 94.8% |
| STORE_FAST | 475,736 | 5.1% |
| STORE_NAME | 11,440 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 305,532,942 | 36.5% |
| LOAD_GLOBAL_MODULE | 246,340,721 | 29.4% |
| LOAD_FAST_LOAD_FAST | 162,915,690 | 19.5% |
| LOAD_GLOBAL_BUILTIN | 62,172,154 | 7.4% |
| LOAD_CONST | 25,191,021 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 695,219,592 | 83.1% |
| POP_JUMP_IF_TRUE | 80,600,796 | 9.6% |
| EXTENDED_ARG | 24,287,820 | 2.9% |
| STORE_FAST | 16,142,920 | 1.9% |
| YIELD_VALUE | 12,857,729 | 1.5% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,242,381,476 | 27.2% |
| POP_TOP | 1,034,636,391 | 22.6% |
| POP_JUMP_IF_FALSE | 639,354,180 | 14.0% |
| POP_JUMP_IF_TRUE | 623,002,831 | 13.6% |
| LIST_APPEND | 187,627,928 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,255,806,503 | 27.4% |
| NOP | 957,351,878 | 20.9% |
| FOR_ITER_RANGE | 642,157,523 | 14.0% |
| LOAD_FAST | 425,137,950 | 9.3% |
| FOR_ITER_TUPLE | 405,243,295 | 8.9% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,413,015 | 99.8% |
| POP_EXCEPT | 650,460 | 0.1% |
| EXTENDED_ARG | 274,392 | 0.1% |
| DELETE_FAST | 39,808 | 0.0% |
| RESUME | 5,164 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,540,261 | 96.9% |
| SEND | 15,877,918 | 2.9% |
| LOAD_FAST | 576,741 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 124,093 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 259,681,966 | 43.0% |
| POP_JUMP_IF_FALSE | 157,973,285 | 26.2% |
| POP_TOP | 78,192,140 | 13.0% |
| LOAD_ATTR_SLOT | 22,813,740 | 3.8% |
| EXTENDED_ARG | 14,230,100 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 272,358,812 | 45.1% |
| LOAD_FAST_LOAD_FAST | 105,274,490 | 17.4% |
| LOAD_CONST | 50,646,846 | 8.4% |
| LOAD_GLOBAL_BUILTIN | 39,093,736 | 6.5% |
| LOAD_GLOBAL_MODULE | 34,919,041 | 5.8% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 38,618,800 | 20.6% |
| BUILD_TUPLE | 36,813,278 | 19.6% |
| BINARY_OP | 27,485,080 | 14.6% |
| LOAD_FAST | 26,470,910 | 14.1% |
| RETURN_GENERATOR | 17,923,920 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 187,627,928 | 99.9% |
| LOAD_FAST | 128,000 | 0.1% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |
| LOAD_CONST | 620 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 98,427,525 | 78.6% |
| LOAD_FAST | 25,883,116 | 20.7% |
| LOAD_CONST | 499,560 | 0.4% |
| RETURN_VALUE | 260,416 | 0.2% |
| LOAD_DEREF | 104,609 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 124,151,316 | 99.1% |
| STORE_FAST | 546,634 | 0.4% |
| LOAD_FAST | 285,336 | 0.2% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.2% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 932,573,410 | 56.9% |
| LOAD_GLOBAL_BUILTIN | 297,297,856 | 18.1% |
| LOAD_GLOBAL_MODULE | 169,434,747 | 10.3% |
| LOAD_ATTR_SLOT | 157,793,551 | 9.6% |
| LOAD_FAST_LOAD_FAST | 28,738,519 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 305,532,942 | 18.6% |
| STORE_FAST | 265,836,249 | 16.2% |
| LOAD_FAST | 230,852,675 | 14.1% |
| PUSH_NULL | 155,839,774 | 9.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 122,395,889 | 7.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,695,781,968 | 49.8% |
| LOAD_CONST | 1,103,410,333 | 8.2% |
| LOAD_FAST_LOAD_FAST | 674,155,233 | 5.0% |
| STORE_FAST | 405,413,796 | 3.0% |
| POP_JUMP_IF_FALSE | 400,410,238 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 2,387,671,366 | 17.8% |
| COMPARE_OP_STR | 2,083,452,032 | 15.5% |
| LOAD_FAST | 1,481,726,195 | 11.0% |
| LOAD_CONST | 1,103,410,333 | 8.2% |
| COMPARE_OP_INT | 870,995,992 | 6.5% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 453,290,199 | 40.9% |
| LOAD_GLOBAL_BUILTIN | 111,485,766 | 10.1% |
| POP_JUMP_IF_FALSE | 74,162,997 | 6.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,400 | 5.6% |
| STORE_FAST_STORE_FAST | 47,072,228 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 669,144,190 | 60.4% |
| LOAD_CONST | 95,095,970 | 8.6% |
| PUSH_NULL | 69,294,143 | 6.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 47,436,358 | 4.3% |
| CALL_LEN | 26,348,902 | 2.4% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,886,811,645 | 17.2% |
| POP_JUMP_IF_FALSE | 6,600,922,964 | 16.5% |
| LOAD_GLOBAL_BUILTIN | 3,611,927,971 | 9.0% |
| RESUME_CHECK | 3,159,423,794 | 7.9% |
| LOAD_CONST | 1,481,726,195 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,695,781,968 | 16.8% |
| LOAD_ATTR_INSTANCE_VALUE | 4,911,583,662 | 12.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,262,452,411 | 5.7% |
| LOAD_ATTR_SLOT | 2,030,693,934 | 5.1% |
| LOAD_GLOBAL_BUILTIN | 1,480,552,267 | 3.7% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 49,075,550 | 67.7% |
| LOAD_FAST_AND_CLEAR | 23,458,136 | 32.3% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 49,070,030 | 67.7% |
| LOAD_FAST_AND_CLEAR | 23,458,136 | 32.3% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,460 | 42.0% |
| LOAD_ATTR_METHOD_NO_DICT | 2,001,354 | 17.7% |
| POP_TOP | 1,692,612 | 15.0% |
| POP_JUMP_IF_NONE | 1,619,718 | 14.3% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,620 | 42.2% |
| LOAD_FAST | 1,901,620 | 16.8% |
| CALL_LIST_APPEND | 1,562,260 | 13.8% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,833,078,049 | 16.4% |
| POP_JUMP_IF_FALSE | 1,627,293,648 | 14.6% |
| NOP | 1,280,393,528 | 11.5% |
| LOAD_FAST_LOAD_FAST | 753,953,298 | 6.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 703,645,561 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 1,602,967,280 | 14.4% |
| CONTAINS_OP | 1,340,419,685 | 12.0% |
| LOAD_FAST | 912,338,479 | 8.2% |
| CALL_PY_EXACT_ARGS | 862,534,967 | 7.7% |
| STORE_ATTR_SLOT | 761,594,514 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,285 | 1.5% |
| LOAD_FAST | 150,696 | 1.4% |
| POP_JUMP_IF_FALSE | 142,371 | 1.3% |
| POP_TOP | 84,932 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,613 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,827 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,285 | 1.7% |
| LOAD_ATTR | 114,871 | 1.1% |
| CALL | 66,009 | 0.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,923 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,140 | 44.4% |
| CALL | 3,683 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,937,473 | 54.4% |
| CALL_PY_EXACT_ARGS | 32,458,010 | 31.0% |
| CALL_FUNCTION_EX | 6,292,867 | 6.0% |
| CALL_KW | 3,006,747 | 2.9% |
| CACHE | 1,969,514 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,937,473 | 54.4% |
| RESUME_CHECK | 46,851,736 | 44.8% |
| RETURN_GENERATOR | 865,067 | 0.8% |
| RESUME | 11,440 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 22.3% |
| RETURN_VALUE | 8,431,080 | 17.7% |
| LOAD_FAST | 8,115,500 | 17.0% |
| LOAD_FAST_LOAD_FAST | 8,080,747 | 16.9% |
| STORE_FAST | 6,068,240 | 12.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 33,085,747 | 69.3% |
| LOAD_CONST | 13,802,300 | 28.9% |
| CALL_FUNCTION_EX | 809,840 | 1.7% |
| EXTENDED_ARG | 53,160 | 0.1% |
| DICT_UPDATE | 4,920 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,533,840,281 | 29.3% |
| CONTAINS_OP | 2,508,951,289 | 20.8% |
| COMPARE_OP_STR | 2,087,403,068 | 17.3% |
| COMPARE_OP_INT | 1,660,804,486 | 13.8% |
| IS_OP | 695,219,592 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,600,922,964 | 54.7% |
| LOAD_FAST_LOAD_FAST | 1,627,293,648 | 13.5% |
| LOAD_GLOBAL_BUILTIN | 1,311,026,450 | 10.9% |
| JUMP_BACKWARD | 639,354,180 | 5.3% |
| RETURN_CONST | 447,298,867 | 3.7% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 334,404,532 | 71.5% |
| EXTENDED_ARG | 48,769,366 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 33,032,234 | 7.1% |
| LOAD_DEREF | 19,462,360 | 4.2% |
| LOAD_ATTR_SLOT | 17,537,360 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 286,498,674 | 61.3% |
| JUMP_BACKWARD | 56,529,220 | 12.1% |
| LOAD_DEREF | 36,389,479 | 7.8% |
| LOAD_FAST_LOAD_FAST | 23,884,164 | 5.1% |
| LOAD_GLOBAL_BUILTIN | 21,129,085 | 4.5% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 552,132,903 | 81.7% |
| LOAD_ATTR_INSTANCE_VALUE | 68,547,440 | 10.1% |
| LOAD_ATTR | 18,718,383 | 2.8% |
| STORE_FAST_LOAD_FAST | 11,838,480 | 1.8% |
| EXTENDED_ARG | 9,716,960 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 325,820,567 | 48.2% |
| LOAD_FAST_LOAD_FAST | 133,199,909 | 19.7% |
| LOAD_GLOBAL_MODULE | 78,807,510 | 11.7% |
| LOAD_GLOBAL_BUILTIN | 46,686,549 | 6.9% |
| RETURN_CONST | 25,067,414 | 3.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,017,110,177 | 50.4% |
| TO_BOOL | 198,894,140 | 9.8% |
| COMPARE_OP_INT | 155,003,586 | 7.7% |
| TO_BOOL_ALWAYS_TRUE | 109,313,040 | 5.4% |
| TO_BOOL_NONE | 99,117,838 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 855,970,746 | 42.4% |
| JUMP_BACKWARD | 623,002,831 | 30.9% |
| LOAD_GLOBAL_BUILTIN | 138,833,018 | 6.9% |
| LOAD_CONST | 95,647,542 | 4.7% |
| POP_TOP | 88,486,396 | 4.4% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,164 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,904 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,410 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,850 | 7.2% |
| POP_JUMP_IF_TRUE | 183,260 | 7.0% |
| DELETE_FAST | 101,280 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,620 | 57.5% |
| COPY | 988,550 | 41.1% |
| CALL_INTRINSIC_1 | 35,010 | 1.5% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 447,298,867 | 22.6% |
| STORE_ATTR_SLOT | 325,584,315 | 16.4% |
| POP_TOP | 303,745,289 | 15.3% |
| STORE_ATTR_INSTANCE_VALUE | 243,517,460 | 12.3% |
| RESUME_CHECK | 143,631,055 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 833,267,712 | 42.1% |
| INTERPRETER_EXIT | 673,819,931 | 34.0% |
| EXIT_INIT_CHECK | 89,720,112 | 4.5% |
| TO_BOOL_BOOL | 81,255,401 | 4.1% |
| END_FOR | 76,080,152 | 3.8% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 149,393,274 | 90.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,877,918 | 9.6% |
| SEND | 51,983 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,380,026 | 85.5% |
| YIELD_VALUE | 15,865,830 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 51,983 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 118,626,671 | 99.3% |
| SET_FUNCTION_ATTRIBUTE | 858,607 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 81,865,885 | 68.5% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 21.2% |
| STORE_FAST | 7,472,751 | 6.3% |
| CALL_PY_EXACT_ARGS | 1,865,929 | 1.6% |
| SET_FUNCTION_ATTRIBUTE | 858,607 | 0.7% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,039,408 | 60.9% |
| LOAD_FAST_LOAD_FAST | 16,409,358 | 24.3% |
| CALL | 6,424,560 | 9.5% |
| SWAP | 1,726,379 | 2.6% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,288,395 | 30.1% |
| LOAD_DEREF | 17,938,486 | 26.6% |
| RETURN_CONST | 10,771,246 | 16.0% |
| JUMP_BACKWARD | 7,408,080 | 11.0% |
| LOAD_FAST_LOAD_FAST | 3,926,508 | 5.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 38.1% |
| STORE_FAST | 25,623,220 | 27.2% |
| LOAD_CONST | 9,108,050 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,494,600 | 4.8% |
| YIELD_VALUE | 3,225,580 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 29,808,180 | 31.7% |
| LOAD_DEREF | 19,714,407 | 20.9% |
| LOAD_FAST_LOAD_FAST | 17,926,003 | 19.0% |
| LOAD_FAST | 12,413,591 | 13.2% |
| LOAD_CONST | 6,330,360 | 6.7% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,684,845,078 | 12.1% |
| BINARY_SUBSCR_STR_INT | 1,129,317,920 | 8.1% |
| STORE_FAST | 956,472,476 | 6.9% |
| RETURN_VALUE | 941,120,788 | 6.8% |
| FOR_ITER_LIST | 803,037,934 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,886,811,645 | 49.5% |
| LOAD_FAST_LOAD_FAST | 1,833,078,049 | 13.2% |
| JUMP_BACKWARD | 1,242,381,476 | 8.9% |
| STORE_FAST | 956,472,476 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 720,348,317 | 5.2% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 106,582,598 | 66.0% |
| FOR_ITER_RANGE | 29,931,480 | 18.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 7.6% |
| FOR_ITER_TUPLE | 7,556,201 | 4.7% |
| FOR_ITER | 3,395,548 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 39,046,844 | 24.2% |
| LOAD_FAST | 36,533,566 | 22.6% |
| STORE_ATTR_INSTANCE_VALUE | 12,393,569 | 7.7% |
| POP_JUMP_IF_NOT_NONE | 11,838,480 | 7.3% |
| TO_BOOL_ALWAYS_TRUE | 10,655,640 | 6.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,087,543,618 | 50.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 577,917,437 | 26.7% |
| UNPACK_SEQUENCE_TUPLE | 211,313,890 | 9.8% |
| UNPACK_SEQUENCE_LIST | 171,284,186 | 7.9% |
| LOAD_ATTR_SLOT | 61,209,852 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,087,543,618 | 50.2% |
| LOAD_FAST | 646,392,938 | 29.9% |
| LOAD_FAST_LOAD_FAST | 129,278,924 | 6.0% |
| STORE_FAST | 123,684,053 | 5.7% |
| LOAD_GLOBAL_MODULE | 63,369,518 | 2.9% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 8,196,880 | 99.9% |
| RETURN_VALUE | 5,340 | 0.1% |
| LOAD_ATTR | 760 | 0.0% |
| LOAD_FAST | 520 | 0.0% |
| CALL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,485,920 | 79.0% |
| LOAD_GLOBAL_MODULE | 1,714,720 | 20.9% |
| LOAD_CONST | 3,320 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| RETURN_CONST | 220 | 0.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 297,080 | 30.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 293,820 | 30.0% |
| MAKE_FUNCTION | 104,620 | 10.7% |
| LOAD_CONST | 61,260 | 6.3% |
| IMPORT_FROM | 59,020 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 363,340 | 37.1% |
| STORE_NAME | 297,080 | 30.3% |
| LOAD_CONST | 199,880 | 20.4% |
| IMPORT_FROM | 35,740 | 3.6% |
| POP_TOP | 23,300 | 2.4% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 361,171,077 | 29.2% |
| BINARY_OP_ADD_FLOAT | 155,333,959 | 12.5% |
| LOAD_FAST | 133,800,174 | 10.8% |
| BINARY_OP_ADD_INT | 111,282,334 | 9.0% |
| BINARY_OP_SUBTRACT_INT | 93,262,275 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 361,171,077 | 29.2% |
| STORE_SUBSCR_LIST_INT | 211,995,640 | 17.1% |
| STORE_SUBSCR | 146,314,802 | 11.8% |
| COPY | 139,461,850 | 11.3% |
| STORE_ATTR_INSTANCE_VALUE | 98,019,430 | 7.9% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 462,400 | 61.2% |
| YIELD_VALUE | 291,340 | 38.6% |
| CALL_INTRINSIC_1 | 1,280 | 0.2% |
| FOR_ITER | 500 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 755,520 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 40.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.2% |
| LOAD_FAST | 35,079 | 11.0% |
| RETURN_VALUE | 25,790 | 8.1% |
| FOR_ITER | 20,203 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 208,033 | 65.1% |
| STORE_FAST | 64,199 | 20.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,686 | 8.3% |
| UNPACK_SEQUENCE_TUPLE | 13,758 | 4.3% |
| UNPACK_SEQUENCE | 2,795 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,559,801 | 40.2% |
| BINARY_OP_MULTIPLY_FLOAT | 281,242,200 | 21.3% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.5% |
| LOAD_FAST | 91,335,296 | 6.9% |
| BUILD_TUPLE | 42,832,960 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 647,600,421 | 49.1% |
| YIELD_VALUE | 529,559,801 | 40.2% |
| STORE_FAST | 102,610,723 | 7.8% |
| UNPACK_SEQUENCE_TUPLE | 33,263,980 | 2.5% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,904 | 38.7% |
| CACHE | 77,878 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,952 | 6.6% |
| COPY_FREE_VARS | 17,234 | 6.4% |
| POP_TOP | 15,728 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,004 | 40.9% |
| LOAD_GLOBAL | 64,609 | 23.8% |
| LOAD_CONST | 23,923 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,511 | 3.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,387,671,366 | 80.2% |
| LOAD_FAST | 312,747,872 | 10.5% |
| LOAD_FAST_LOAD_FAST | 126,904,669 | 4.3% |
| END_SEND | 38,845,400 | 1.3% |
| BINARY_OP_MULTIPLY_INT | 32,049,852 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,684,845,078 | 56.6% |
| LOAD_CONST | 177,179,109 | 6.0% |
| STORE_SLICE | 138,548,820 | 4.7% |
| BINARY_OP_MULTIPLY_INT | 128,113,818 | 4.3% |
| BINARY_SUBSCR | 117,470,780 | 3.9% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,918,720 | 45.4% |
| BINARY_SLICE | 20,546,260 | 21.2% |
| LOAD_CONST | 14,990,500 | 15.5% |
| CALL_STR_1 | 6,406,760 | 6.6% |
| BUILD_STRING | 2,681,360 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 21.9% |
| LOAD_FAST | 20,597,280 | 21.3% |
| BUILD_TUPLE | 20,394,960 | 21.1% |
| LOAD_CONST | 11,661,540 | 12.1% |
| STORE_FAST | 9,962,620 | 10.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 128,113,818 | 35.8% |
| LOAD_ATTR_INSTANCE_VALUE | 68,312,879 | 19.1% |
| LOAD_FAST_LOAD_FAST | 60,166,667 | 16.8% |
| LOAD_FAST | 51,788,385 | 14.5% |
| BINARY_OP | 36,447,155 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 83,111,509 | 23.2% |
| LOAD_CONST | 82,192,229 | 23.0% |
| LOAD_FAST | 62,827,706 | 17.6% |
| LOAD_FAST_LOAD_FAST | 37,842,866 | 10.6% |
| BINARY_OP_ADD_INT | 32,049,852 | 9.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 145,713,640 | 40.4% |
| LOAD_FAST | 92,723,414 | 25.7% |
| LOAD_FAST_LOAD_FAST | 48,507,198 | 13.5% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,156 | 10.6% |
| BINARY_SUBSCR | 16,972,600 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 128,812,048 | 35.7% |
| LOAD_FAST_LOAD_FAST | 97,735,340 | 27.1% |
| SWAP | 74,443,747 | 20.7% |
| LOAD_FAST | 37,921,452 | 10.5% |
| BINARY_OP_SUBTRACT_FLOAT | 14,316,500 | 4.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 503,866,769 | 76.5% |
| LOAD_FAST | 90,231,845 | 13.7% |
| LOAD_FAST_LOAD_FAST | 46,055,783 | 7.0% |
| LOAD_ATTR_INSTANCE_VALUE | 13,371,100 | 2.0% |
| CALL_LEN | 3,640,940 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 142,814,880 | 21.7% |
| STORE_FAST | 124,764,518 | 18.9% |
| SWAP | 93,262,275 | 14.2% |
| RETURN_VALUE | 53,628,779 | 8.1% |
| BINARY_OP | 50,043,436 | 7.6% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 269,639,606 | 33.9% |
| LOAD_CONST | 240,634,999 | 30.2% |
| LOAD_FAST_LOAD_FAST | 186,563,941 | 23.4% |
| BINARY_SUBSCR | 55,022,240 | 6.9% |
| LOAD_ATTR_INSTANCE_VALUE | 15,148,720 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 311,051,656 | 39.1% |
| RETURN_VALUE | 136,219,539 | 17.1% |
| CONTAINS_OP | 103,692,020 | 13.0% |
| LOAD_FAST | 57,292,386 | 7.2% |
| LOAD_ATTR_METHOD_NO_DICT | 56,170,560 | 7.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 90,026,420 | 46.4% |
| LOAD_CONST | 55,550,952 | 28.6% |
| BUILD_TUPLE | 38,415,920 | 19.8% |
| LOAD_FAST | 4,619,728 | 2.4% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,058,568 | 99.5% |
| MAKE_CELL | 629,628 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360,808,162 | 30.2% |
| LOAD_CONST | 243,039,690 | 20.4% |
| LOAD_FAST_LOAD_FAST | 225,207,939 | 18.9% |
| COPY | 211,995,640 | 17.8% |
| BINARY_OP | 64,465,560 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 317,018,189 | 26.6% |
| LOAD_CONST | 252,513,100 | 21.2% |
| LOAD_FAST | 186,114,199 | 15.6% |
| RETURN_VALUE | 120,829,666 | 10.1% |
| BINARY_OP | 51,776,717 | 4.3% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,602,967,280 | 96.5% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 0.9% |
| LOAD_FAST | 14,072,960 | 0.8% |
| LOAD_ATTR_SLOT | 13,808,080 | 0.8% |
| LOAD_CONST | 8,064,280 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,129,317,920 | 68.0% |
| LOAD_FAST | 517,397,860 | 31.2% |
| LOAD_CONST | 7,660,340 | 0.5% |
| RETURN_VALUE | 4,949,800 | 0.3% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 252,329,265 | 82.5% |
| LOAD_FAST | 53,333,983 | 17.4% |
| LOAD_FAST_LOAD_FAST | 115,720 | 0.0% |
| BINARY_SUBSCR | 8,555 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,082,463 | 31.4% |
| LOAD_GLOBAL_MODULE | 40,548,860 | 13.3% |
| LOAD_FAST | 32,910,122 | 10.8% |
| LOAD_CONST | 32,760,455 | 10.7% |
| YIELD_VALUE | 25,849,800 | 8.5% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 26,911,200 | 29.3% |
| LOAD_GLOBAL_MODULE | 12,291,795 | 13.4% |
| BINARY_OP_MULTIPLY_FLOAT | 11,970,360 | 13.0% |
| RETURN_CONST | 10,486,240 | 11.4% |
| BINARY_OP_ADD_FLOAT | 6,838,640 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 87,239,985 | 94.8% |
| COPY_FREE_VARS | 2,480,587 | 2.7% |
| LOAD_FAST | 2,217,180 | 2.4% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,280,858 | 31.4% |
| LOAD_CONST | 65,595,960 | 27.7% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 12.7% |
| PUSH_NULL | 15,993,990 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 12,257,983 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,675,939 | 81.8% |
| COPY_FREE_VARS | 37,082,760 | 15.7% |
| GET_AWAITABLE | 3,005,400 | 1.3% |
| POP_TOP | 1,466,800 | 0.6% |
| MAKE_CELL | 885,339 | 0.4% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,416,677 | 26.0% |
| CALL_LEN | 30,113,990 | 16.5% |
| LOAD_GLOBAL_BUILTIN | 14,673,448 | 8.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,111,187 | 6.6% |
| BINARY_OP_MULTIPLY_INT | 10,216,529 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 79,001,148 | 43.2% |
| STORE_FAST | 26,261,950 | 14.4% |
| BINARY_OP_MULTIPLY_FLOAT | 17,043,680 | 9.3% |
| LOAD_FAST | 11,284,760 | 6.2% |
| CALL_BUILTIN_CLASS | 7,589,459 | 4.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 579,374,340 | 44.5% |
| LOAD_CONST | 467,838,043 | 35.9% |
| LOAD_FAST_LOAD_FAST | 113,271,315 | 8.7% |
| CALL_BUILTIN_FAST | 49,960,540 | 3.8% |
| LOAD_FAST | 37,858,992 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 654,393,208 | 50.2% |
| STORE_FAST | 440,155,327 | 33.8% |
| POP_TOP | 66,404,603 | 5.1% |
| CALL_BUILTIN_FAST | 49,960,540 | 3.8% |
| RETURN_VALUE | 36,341,938 | 2.8% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 64,521,680 | 51.4% |
| LOAD_FAST | 20,920,150 | 16.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,549 | 6.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,762,500 | 5.4% |
| LOAD_FAST_LOAD_FAST | 6,761,851 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,400 | 49.7% |
| STORE_FAST | 24,343,904 | 19.4% |
| POP_TOP | 8,353,064 | 6.7% |
| LOAD_FAST | 7,177,265 | 5.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,762,500 | 5.4% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 803,599,936 | 68.7% |
| LOAD_CONST | 114,218,836 | 9.8% |
| RETURN_VALUE | 72,240,120 | 6.2% |
| BUILD_STRING | 48,913,080 | 4.2% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 516,285,204 | 44.1% |
| STORE_FAST | 262,646,225 | 22.4% |
| LOAD_CONST | 228,977,778 | 19.6% |
| RETURN_VALUE | 49,088,754 | 4.2% |
| TO_BOOL_BOOL | 22,308,189 | 1.9% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 435,023,684 | 41.5% |
| LOAD_GLOBAL_BUILTIN | 429,301,347 | 41.0% |
| LOAD_FAST_LOAD_FAST | 85,067,445 | 8.1% |
| BUILD_TUPLE | 42,623,198 | 4.1% |
| LOAD_ATTR_MODULE | 33,465,978 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,026,426,748 | 97.9% |
| YIELD_VALUE | 7,577,810 | 0.7% |
| COPY | 6,465,186 | 0.6% |
| RETURN_VALUE | 3,010,120 | 0.3% |
| POP_TOP | 2,662,380 | 0.3% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 295,975,588 | 66.1% |
| LOAD_ATTR_INSTANCE_VALUE | 59,712,633 | 13.3% |
| BINARY_SUBSCR_LIST_INT | 39,397,840 | 8.8% |
| LOAD_DEREF | 26,348,902 | 5.9% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 169,741,485 | 37.9% |
| LOAD_FAST | 58,956,115 | 13.2% |
| STORE_FAST | 51,805,748 | 11.6% |
| COMPARE_OP_INT | 51,125,203 | 11.4% |
| CALL_BUILTIN_CLASS | 30,113,990 | 6.7% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 236,690,299 | 72.0% |
| BINARY_SUBSCR | 26,894,680 | 8.2% |
| BINARY_SLICE | 25,775,289 | 7.8% |
| BINARY_OP | 7,787,520 | 2.4% |
| BINARY_SUBSCR_TUPLE_INT | 6,900,960 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 132,411,451 | 40.3% |
| LOAD_FAST | 90,787,411 | 27.6% |
| EXTENDED_ARG | 41,464,738 | 12.6% |
| RETURN_CONST | 27,374,520 | 8.3% |
| LOAD_CONST | 14,733,040 | 4.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,696,866 | 51.2% |
| LOAD_FAST_LOAD_FAST | 71,966,547 | 15.5% |
| LOAD_ATTR_METHOD_NO_DICT | 56,916,021 | 12.2% |
| LOAD_CONST | 37,386,280 | 8.0% |
| LOAD_GLOBAL_MODULE | 23,820,928 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 327,906,425 | 70.4% |
| LIST_APPEND | 38,618,800 | 8.3% |
| LOAD_FAST | 25,804,049 | 5.5% |
| RETURN_VALUE | 15,612,415 | 3.4% |
| TO_BOOL_BOOL | 11,822,795 | 2.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 84,767,578 | 81.1% |
| LOAD_FAST | 12,104,745 | 11.6% |
| LOAD_ATTR_METHOD_NO_DICT | 5,564,845 | 5.3% |
| LOAD_FAST_LOAD_FAST | 1,396,843 | 1.3% |
| LOAD_ATTR | 387,049 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 81,471,685 | 77.9% |
| CALL_METHOD_DESCRIPTOR_O | 9,246,800 | 8.8% |
| LOAD_ATTR_METHOD_NO_DICT | 3,892,360 | 3.7% |
| RETURN_VALUE | 2,962,080 | 2.8% |
| BINARY_OP | 2,681,320 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 275,530,751 | 63.6% |
| LOAD_ATTR | 122,395,889 | 28.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,805 | 5.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,922,048 | 2.3% |
| LOAD_FAST | 2,104,280 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 160,782,826 | 37.1% |
| TO_BOOL_BOOL | 123,418,761 | 28.5% |
| GET_ITER | 58,891,479 | 13.6% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 5.7% |
| LOAD_FAST | 16,482,747 | 3.8% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 330,663,601 | 80.1% |
| CALL | 44,075,382 | 10.7% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 9,246,800 | 2.2% |
| LOAD_GLOBAL_MODULE | 4,939,560 | 1.2% |
| LOAD_ATTR | 4,016,660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 265,880,992 | 64.4% |
| BINARY_OP | 96,002,520 | 23.3% |
| RETURN_VALUE | 23,240,305 | 5.6% |
| STORE_FAST | 10,328,834 | 2.5% |
| LOAD_FAST | 6,456,900 | 1.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,253,931,882 | 31.9% |
| LOAD_FAST_LOAD_FAST | 862,534,967 | 22.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 734,525,088 | 18.7% |
| LOAD_GLOBAL_MODULE | 224,567,284 | 5.7% |
| LOAD_ATTR_METHOD_NO_DICT | 184,024,727 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,473,560,669 | 88.4% |
| RETURN_GENERATOR | 228,352,193 | 5.8% |
| COPY_FREE_VARS | 171,429,250 | 4.4% |
| MAKE_CELL | 32,458,010 | 0.8% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.5% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 78,074,728 | 35.8% |
| LOAD_FAST | 49,269,227 | 22.6% |
| LOAD_ATTR_METHOD_NO_DICT | 18,063,705 | 8.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,666,551 | 7.2% |
| LOAD_ATTR | 14,799,480 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 200,402,329 | 92.0% |
| RETURN_GENERATOR | 8,944,785 | 4.1% |
| COPY_FREE_VARS | 6,562,843 | 3.0% |
| MAKE_CELL | 1,826,819 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,960 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,968,068 | 85.4% |
| RETURN_VALUE | 8,776,840 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 2.2% |
| LOAD_ATTR_SLOT | 145,520 | 0.2% |
| CALL_TUPLE_1 | 88,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 15,696,800 | 21.0% |
| CALL_PY_EXACT_ARGS | 14,464,480 | 19.3% |
| STORE_FAST | 13,540,948 | 18.1% |
| YIELD_VALUE | 10,243,140 | 13.7% |
| BINARY_OP_ADD_UNICODE | 6,406,760 | 8.6% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,946,386 | 43.8% |
| RETURN_GENERATOR | 7,370,320 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,629 | 18.8% |
| LOAD_ATTR_SLOT | 732,232 | 2.9% |
| CALL | 585,500 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,609,080 | 38.4% |
| BINARY_OP | 4,799,389 | 19.2% |
| BUILD_TUPLE | 3,611,752 | 14.4% |
| YIELD_VALUE | 3,229,160 | 12.9% |
| STORE_FAST | 1,211,504 | 4.8% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 470,388,646 | 98.9% |
| LOAD_CONST | 4,947,424 | 1.0% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 395,073,986 | 83.1% |
| LOAD_GLOBAL_BUILTIN | 24,735,339 | 5.2% |
| LOAD_GLOBAL_MODULE | 18,338,706 | 3.9% |
| CALL_PY_EXACT_ARGS | 10,534,742 | 2.2% |
| LOAD_FAST | 5,977,160 | 1.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 152,313,867 | 69.1% |
| BINARY_SUBSCR | 31,176,840 | 14.2% |
| LOAD_FAST | 12,696,170 | 5.8% |
| LOAD_GLOBAL_MODULE | 8,575,595 | 3.9% |
| LOAD_CONST | 8,434,456 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,314,047 | 58.2% |
| POP_JUMP_IF_FALSE | 48,719,146 | 22.1% |
| POP_JUMP_IF_TRUE | 43,257,880 | 19.6% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 870,995,992 | 44.1% |
| LOAD_ATTR_INSTANCE_VALUE | 239,531,649 | 12.1% |
| LOAD_FAST_LOAD_FAST | 190,118,815 | 9.6% |
| LOAD_FAST | 163,862,849 | 8.3% |
| COPY | 135,328,947 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,660,804,486 | 84.1% |
| POP_JUMP_IF_TRUE | 155,003,586 | 7.9% |
| RETURN_VALUE | 78,989,112 | 4.0% |
| EXTENDED_ARG | 24,097,846 | 1.2% |
| LOAD_FAST | 19,952,260 | 1.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,083,452,032 | 98.1% |
| LOAD_FAST_LOAD_FAST | 11,185,560 | 0.5% |
| LOAD_FAST | 7,627,677 | 0.4% |
| LOAD_GLOBAL_MODULE | 6,933,091 | 0.3% |
| RETURN_VALUE | 4,923,060 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,087,403,068 | 98.3% |
| POP_JUMP_IF_TRUE | 21,894,896 | 1.0% |
| COPY | 6,634,148 | 0.3% |
| RETURN_VALUE | 5,256,970 | 0.2% |
| EXTENDED_ARG | 1,248,800 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,255,806,503 | 75.6% |
| GET_ITER | 242,863,784 | 14.6% |
| LOAD_FAST | 81,087,216 | 4.9% |
| EXTENDED_ARG | 55,462,030 | 3.3% |
| SWAP | 24,506,438 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 803,037,934 | 48.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 422,939,795 | 25.5% |
| RETURN_CONST | 137,192,636 | 8.3% |
| STORE_FAST_LOAD_FAST | 106,582,598 | 6.4% |
| LOAD_FAST | 76,191,731 | 4.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 642,157,523 | 90.1% |
| GET_ITER | 35,291,294 | 4.9% |
| LOAD_FAST | 28,737,640 | 4.0% |
| SWAP | 5,310,740 | 0.7% |
| EXTENDED_ARG | 1,592,260 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 617,766,289 | 86.6% |
| RETURN_CONST | 31,040,694 | 4.4% |
| STORE_FAST_LOAD_FAST | 29,931,480 | 4.2% |
| JUMP_BACKWARD | 12,900,860 | 1.8% |
| LOAD_FAST | 6,590,885 | 0.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 405,243,295 | 69.6% |
| GET_ITER | 168,441,600 | 28.9% |
| SWAP | 3,014,683 | 0.5% |
| LOAD_FAST | 2,193,661 | 0.4% |
| EXTENDED_ARG | 1,839,640 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 404,708,514 | 69.5% |
| LOAD_FAST | 83,035,043 | 14.3% |
| LOAD_FAST_LOAD_FAST | 57,908,180 | 9.9% |
| RETURN_CONST | 17,092,243 | 2.9% |
| STORE_FAST_LOAD_FAST | 7,556,201 | 1.3% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 150,765,573 | 85.3% |
| LOAD_GLOBAL_BUILTIN | 23,035,060 | 13.0% |
| LOAD_FAST | 1,277,860 | 0.7% |
| LOAD_FAST_LOAD_FAST | 805,820 | 0.5% |
| LOAD_ATTR_MODULE | 685,645 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 77,943,947 | 44.1% |
| CALL_PY_EXACT_ARGS | 29,127,778 | 16.5% |
| LOAD_FAST_LOAD_FAST | 23,238,140 | 13.2% |
| LOAD_FAST | 20,932,673 | 11.8% |
| PUSH_NULL | 11,045,720 | 6.3% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,911,583,662 | 86.6% |
| LOAD_FAST_LOAD_FAST | 453,152,126 | 8.0% |
| COPY | 98,019,430 | 1.7% |
| LOAD_ATTR_INSTANCE_VALUE | 78,086,840 | 1.4% |
| BINARY_SUBSCR_LIST_INT | 49,373,960 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,412,041,392 | 24.9% |
| TO_BOOL_BOOL | 779,865,242 | 13.8% |
| LOAD_ATTR_METHOD_NO_DICT | 417,238,585 | 7.4% |
| STORE_FAST | 384,467,338 | 6.8% |
| RETURN_VALUE | 322,939,625 | 5.7% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,053,109,539 | 53.7% |
| LOAD_ATTR_INSTANCE_VALUE | 417,238,585 | 21.3% |
| LOAD_CONST | 121,519,221 | 6.2% |
| LOAD_GLOBAL_MODULE | 67,280,932 | 3.4% |
| BINARY_SUBSCR_DICT | 56,170,560 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 976,247,126 | 49.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 275,530,751 | 14.1% |
| LOAD_CONST | 188,676,150 | 9.6% |
| CALL_PY_EXACT_ARGS | 184,024,727 | 9.4% |
| LOAD_FAST_LOAD_FAST | 145,857,794 | 7.4% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,262,452,411 | 83.2% |
| LOAD_ATTR_SLOT | 124,116,069 | 4.6% |
| LOAD_ATTR_INSTANCE_VALUE | 106,892,991 | 3.9% |
| LOAD_ATTR | 60,678,031 | 2.2% |
| LOAD_ATTR_WITH_HINT | 49,437,332 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,097,397,591 | 40.4% |
| CALL_PY_EXACT_ARGS | 734,525,088 | 27.0% |
| LOAD_FAST_LOAD_FAST | 703,645,561 | 25.9% |
| LOAD_GLOBAL_MODULE | 67,169,256 | 2.5% |
| LOAD_CONST | 62,319,156 | 2.3% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 558,609,239 | 97.1% |
| LOAD_ATTR_MODULE | 12,552,816 | 2.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,441,880 | 0.3% |
| LOAD_FAST | 906,389 | 0.2% |
| LOAD_ATTR_CLASS | 774,400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 475,606,311 | 82.6% |
| CALL_ISINSTANCE | 33,465,978 | 5.8% |
| LOAD_ATTR_MODULE | 12,552,816 | 2.2% |
| LOAD_FAST | 12,413,046 | 2.2% |
| LOAD_FAST_LOAD_FAST | 9,257,860 | 1.6% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 175,022,295 | 90.9% |
| LOAD_FAST_LOAD_FAST | 15,020,647 | 7.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,025,325 | 0.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,366 | 0.5% |
| STORE_FAST_LOAD_FAST | 223,806 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,760,388 | 21.2% |
| LOAD_FAST_LOAD_FAST | 36,818,360 | 19.1% |
| GET_ITER | 25,707,560 | 13.4% |
| LOAD_GLOBAL_BUILTIN | 20,518,820 | 10.7% |
| LOAD_ATTR_METHOD_NO_DICT | 13,673,072 | 7.1% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,310,450 | 89.1% |
| LOAD_ATTR_SLOT | 3,413,549 | 4.1% |
| RETURN_VALUE | 2,411,829 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,192,740 | 1.5% |
| BINARY_SUBSCR | 573,120 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 66,444,585 | 80.8% |
| COPY_FREE_VARS | 5,272,988 | 6.4% |
| TO_BOOL_NONE | 4,444,793 | 5.4% |
| GET_ITER | 1,924,529 | 2.3% |
| TO_BOOL_BOOL | 743,497 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,030,693,934 | 93.9% |
| COPY | 53,867,647 | 2.5% |
| LOAD_ATTR_SLOT | 37,465,010 | 1.7% |
| LOAD_DEREF | 13,206,800 | 0.6% |
| LOAD_FAST_LOAD_FAST | 11,191,689 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 470,794,597 | 21.8% |
| TO_BOOL_NONE | 211,298,323 | 9.8% |
| LOAD_ATTR | 157,793,551 | 7.3% |
| COMPARE_OP_FLOAT | 152,313,867 | 7.0% |
| TO_BOOL_BOOL | 150,188,970 | 6.9% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360,923,168 | 80.6% |
| LOAD_ATTR_WITH_HINT | 29,449,666 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 27,166,035 | 6.1% |
| COPY | 18,716,600 | 4.2% |
| LOAD_FAST_LOAD_FAST | 8,032,397 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 112,601,820 | 25.2% |
| STORE_FAST | 57,037,140 | 12.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 49,437,332 | 11.0% |
| COMPARE_OP_INT | 47,045,299 | 10.5% |
| LOAD_CONST | 34,355,724 | 7.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,480,552,267 | 26.5% |
| POP_JUMP_IF_FALSE | 1,311,026,450 | 23.5% |
| RESUME_CHECK | 1,232,938,897 | 22.1% |
| STORE_FAST | 720,348,317 | 12.9% |
| POP_JUMP_IF_TRUE | 138,833,018 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,611,927,971 | 64.6% |
| CALL_BUILTIN_FAST | 579,374,340 | 10.4% |
| CALL_ISINSTANCE | 429,301,347 | 7.7% |
| LOAD_ATTR | 297,297,856 | 5.3% |
| LOAD_FAST_LOAD_FAST | 177,885,054 | 3.2% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,287,687,272 | 31.2% |
| STORE_FAST | 554,380,794 | 13.4% |
| RESUME_CHECK | 507,883,900 | 12.3% |
| POP_JUMP_IF_FALSE | 399,517,346 | 9.7% |
| LOAD_FAST_LOAD_FAST | 171,560,734 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 624,747,876 | 15.2% |
| LOAD_FAST | 591,640,693 | 14.3% |
| LOAD_ATTR_MODULE | 558,609,239 | 13.5% |
| CALL_ISINSTANCE | 435,023,684 | 10.5% |
| CONTAINS_OP | 413,154,831 | 10.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 122,419,148 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,335,393 | 46.8% |
| LOAD_FAST | 46,060,989 | 37.6% |
| CALL_PY_EXACT_ARGS | 12,732,232 | 10.4% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.2% |
| CALL | 1,599,380 | 1.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,473,560,669 | 45.8% |
| CACHE | 1,695,835,832 | 22.3% |
| SEND_GEN | 529,524,133 | 7.0% |
| POP_TOP | 394,748,560 | 5.2% |
| COPY_FREE_VARS | 239,280,734 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,159,423,794 | 41.6% |
| LOAD_GLOBAL_BUILTIN | 1,232,938,897 | 16.2% |
| POP_TOP | 758,690,460 | 10.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,413,015 | 7.2% |
| NOP | 515,599,714 | 6.8% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 546,685,733 | 48.4% |
| LOAD_FAST_LOAD_FAST | 385,257,304 | 34.1% |
| SWAP | 98,019,430 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.2% |
| RETURN_VALUE | 28,223,040 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 422,762,155 | 37.4% |
| RETURN_CONST | 243,517,460 | 21.5% |
| LOAD_FAST_LOAD_FAST | 204,350,108 | 18.1% |
| LOAD_CONST | 117,439,513 | 10.4% |
| NOP | 72,209,693 | 6.4% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 761,594,514 | 51.3% |
| LOAD_FAST | 665,829,345 | 44.9% |
| SWAP | 53,867,647 | 3.6% |
| STORE_ATTR_SLOT | 1,770,095 | 0.1% |
| LOAD_ATTR_SLOT | 423,780 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 445,253,248 | 30.0% |
| LOAD_FAST | 348,466,159 | 23.5% |
| RETURN_CONST | 325,584,315 | 21.9% |
| LOAD_CONST | 314,390,795 | 21.2% |
| LOAD_GLOBAL_BUILTIN | 18,021,320 | 1.2% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,505,475 | 48.4% |
| SWAP | 18,716,600 | 27.9% |
| LOAD_FAST_LOAD_FAST | 15,563,617 | 23.2% |
| LOAD_DEREF | 322,000 | 0.5% |
| LOAD_ATTR_INSTANCE_VALUE | 6,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,524 | 67.6% |
| JUMP_BACKWARD | 7,082,100 | 10.6% |
| RETURN_CONST | 5,727,880 | 8.5% |
| LOAD_CONST | 4,970,393 | 7.4% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.6% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 125,208,709 | 46.3% |
| LOAD_FAST | 88,380,064 | 32.7% |
| CALL_BUILTIN_O | 18,664,880 | 6.9% |
| RETURN_VALUE | 10,738,440 | 4.0% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,848 | 36.0% |
| LOAD_FAST | 89,134,583 | 33.0% |
| JUMP_BACKWARD | 40,462,309 | 15.0% |
| RETURN_CONST | 22,483,351 | 8.3% |
| LOAD_GLOBAL_MODULE | 9,867,777 | 3.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 211,995,640 | 50.0% |
| LOAD_FAST | 76,709,936 | 18.1% |
| LOAD_FAST_LOAD_FAST | 50,845,046 | 12.0% |
| LOAD_CONST | 36,182,009 | 8.5% |
| BINARY_SUBSCR_LIST_INT | 26,894,680 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 157,499,407 | 37.1% |
| LOAD_FAST | 153,541,480 | 36.2% |
| LOAD_FAST_LOAD_FAST | 105,456,035 | 24.9% |
| RETURN_CONST | 6,264,740 | 1.5% |
| LOAD_CONST | 788,760 | 0.2% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 103,470,883 | 43.7% |
| LOAD_ATTR_INSTANCE_VALUE | 88,803,686 | 37.5% |
| LOAD_ATTR_SLOT | 20,807,060 | 8.8% |
| STORE_FAST_LOAD_FAST | 10,655,640 | 4.5% |
| COPY | 9,441,990 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 125,498,704 | 53.0% |
| POP_JUMP_IF_TRUE | 109,313,040 | 46.2% |
| TO_BOOL_NONE | 919,071 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 138,766 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 1,026,426,748 | 21.7% |
| LOAD_FAST | 990,299,025 | 21.0% |
| LOAD_ATTR_INSTANCE_VALUE | 779,865,242 | 16.5% |
| CALL_BUILTIN_FAST | 654,393,208 | 13.9% |
| RETURN_VALUE | 393,504,498 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,533,840,281 | 74.8% |
| POP_JUMP_IF_TRUE | 1,017,110,177 | 21.5% |
| EXTENDED_ARG | 109,310,606 | 2.3% |
| UNARY_NOT | 61,414,094 | 1.3% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 254,722,512 | 77.4% |
| CALL_BUILTIN_O | 17,121,860 | 5.2% |
| COPY | 16,752,385 | 5.1% |
| BINARY_OP | 13,012,017 | 4.0% |
| LOAD_ATTR_SLOT | 9,167,000 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 280,543,374 | 85.2% |
| POP_JUMP_IF_TRUE | 47,018,772 | 14.3% |
| UNARY_NOT | 1,348,783 | 0.4% |
| EXTENDED_ARG | 218,626 | 0.1% |
| TO_BOOL_BOOL | 18,240 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 99,911,451 | 56.2% |
| LOAD_ATTR_INSTANCE_VALUE | 69,151,356 | 38.9% |
| LOAD_ATTR_SLOT | 3,364,660 | 1.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.3% |
| BINARY_SUBSCR_DICT | 942,200 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 107,692,679 | 60.6% |
| POP_JUMP_IF_TRUE | 66,071,768 | 37.2% |
| UNARY_NOT | 2,930,546 | 1.6% |
| EXTENDED_ARG | 916,120 | 0.5% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 221,178,692 | 35.4% |
| LOAD_ATTR_SLOT | 211,298,323 | 33.9% |
| LOAD_ATTR_INSTANCE_VALUE | 91,354,523 | 14.6% |
| LOAD_ATTR | 47,235,966 | 7.6% |
| RETURN_CONST | 18,540,000 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 522,830,338 | 83.8% |
| POP_JUMP_IF_TRUE | 99,117,838 | 15.9% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 919,507 | 0.1% |
| TO_BOOL | 164,633 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,509,284 | 64.4% |
| LOAD_ATTR_SLOT | 9,303,200 | 10.8% |
| LOAD_ATTR_INSTANCE_VALUE | 5,695,780 | 6.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 5,129,360 | 5.9% |
| COPY | 2,926,860 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,478,744 | 53.9% |
| POP_JUMP_IF_TRUE | 38,858,840 | 45.1% |
| UNARY_NOT | 615,440 | 0.7% |
| EXTENDED_ARG | 186,940 | 0.2% |
| TO_BOOL_NONE | 46,120 | 0.1% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 344,983,712 | 58.4% |
| LOAD_FAST | 138,823,107 | 23.5% |
| YIELD_VALUE | 33,263,980 | 5.6% |
| BINARY_SUBSCR_DICT | 19,025,120 | 3.2% |
| STORE_FAST | 16,267,800 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 347,320,858 | 58.8% |
| STORE_FAST_STORE_FAST | 211,313,890 | 35.7% |
| UNPACK_SEQUENCE_LIST | 32,035,080 | 5.4% |
| LOAD_FAST | 387,280 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 422,939,795 | 46.9% |
| FOR_ITER | 263,452,433 | 29.2% |
| RETURN_VALUE | 131,842,435 | 14.6% |
| LOAD_FAST | 48,967,864 | 5.4% |
| BINARY_SUBSCR_LIST_INT | 20,152,908 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 577,917,437 | 64.1% |
| STORE_FAST | 289,154,466 | 32.1% |
| UNPACK_SEQUENCE_TUPLE | 16,001,520 | 1.8% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 1.4% |
| STORE_DEREF | 4,494,600 | 0.5% |


</details>

### INSTRUMENTED_RESUME

<details>
<summary> Successors and predecessors for INSTRUMENTED_RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 19,436,580 | 100.0% |
| CALL | 4,500 | 0.0% |
| RESUME_CHECK | 1,060 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| RESUME | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,425,760 | 99.9% |
| LOAD_GLOBAL | 16,000 | 0.1% |
| RESUME | 960 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| LOAD_CONST | 240 | 0.0% |


</details>

### INSTRUMENTED_RETURN_VALUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,717,760 | 50.0% |
| BINARY_OP_ADD_INT | 9,711,340 | 50.0% |
| CALL | 1,280 | 0.0% |
| INSTRUMENTED_RETURN_VALUE | 1,280 | 0.0% |
| BINARY_SLICE | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 9,711,320 | 50.0% |
| LOAD_GLOBAL_MODULE | 9,711,320 | 50.0% |
| STORE_FAST | 7,040 | 0.0% |
| TO_BOOL_BOOL | 1,560 | 0.0% |
| INSTRUMENTED_RETURN_VALUE | 1,280 | 0.0% |


</details>

### INSTRUMENTED_RETURN_CONST

<details>
<summary> Successors and predecessors for INSTRUMENTED_RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 6,320 | 87.8% |
| POP_TOP | 420 | 5.8% |
| INSTRUMENTED_FOR_ITER | 320 | 4.4% |
| STORE_GLOBAL | 80 | 1.1% |
| CALL_LIST_APPEND | 60 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,400 | 88.9% |
| TO_BOOL_BOOL | 440 | 6.1% |
| POP_TOP | 240 | 3.3% |
| TO_BOOL | 120 | 1.7% |


</details>

### INSTRUMENTED_FOR_ITER

<details>
<summary> Successors and predecessors for INSTRUMENTED_FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_JUMP_BACKWARD | 5,908 | 52.4% |
| GET_ITER | 5,280 | 46.9% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,988 | 53.1% |
| NOP | 4,080 | 36.2% |
| LOAD_CONST | 320 | 2.8% |
| INSTRUMENTED_RETURN_CONST | 320 | 2.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 280 | 2.5% |


</details>

### INSTRUMENTED_JUMP_FORWARD

<details>
<summary> Successors and predecessors for INSTRUMENTED_JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 320 | 80.0% |
| STORE_FAST | 80 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320 | 80.0% |
| LOAD_GLOBAL | 80 | 20.0% |


</details>

### INSTRUMENTED_JUMP_BACKWARD

<details>
<summary> Successors and predecessors for INSTRUMENTED_JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.8% |
| STORE_FAST | 4,080 | 40.8% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,268 | 12.7% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,908 | 59.2% |
| LOAD_FAST | 4,080 | 40.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,088 | 52.8% |
| TO_BOOL | 4,280 | 31.9% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.3% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,268 | 9.4% |
| INSTRUMENTED_RETURN_VALUE | 640 | 4.8% |
| POP_TOP | 240 | 1.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 19,422,780 | 99.8% |
| TO_BOOL_BOOL | 18,040 | 0.1% |
| COMPARE_OP_STR | 9,300 | 0.0% |
| TO_BOOL_STR | 8,760 | 0.0% |
| EXTENDED_ARG | 4,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,729,360 | 50.0% |
| LOAD_GLOBAL | 9,716,800 | 49.9% |
| LOAD_FAST_LOAD_FAST | 12,560 | 0.1% |
| INSTRUMENTED_RETURN_CONST | 6,320 | 0.0% |
| POP_TOP | 320 | 0.0% |


</details>

### INSTRUMENTED_POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 720 | 100.0% |


</details>

### INSTRUMENTED_POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 360 | 90.0% |
| LOAD_ATTR | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 100.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 15,180 | 75.6% |
| STORE_DEREF | 1,800 | 9.0% |
| POP_TOP | 1,600 | 8.0% |
| STORE_FAST | 440 | 2.2% |
| RETURN_VALUE | 240 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 20,080 | 100.0% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,739,160 | 48.0% |
| RESUME_CHECK | 5,281,700 | 37.6% |
| LOAD_NAME | 895,800 | 6.4% |
| STORE_NAME | 363,340 | 2.6% |
| POP_JUMP_IF_FALSE | 284,540 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,290,240 | 44.8% |
| LOAD_CONST | 5,818,640 | 41.4% |
| LOAD_NAME | 895,800 | 6.4% |
| CONTAINS_OP | 297,880 | 2.1% |
| STORE_SUBSCR_DICT | 278,780 | 2.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,380,026 | 45.0% |
| RETURN_VALUE | 108,959,451 | 34.7% |
| RETURN_CONST | 63,940,775 | 20.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,802,904 | 41.3% |
| POP_TOP | 94,363,990 | 30.0% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,040 | 2.7% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,265,626 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,979 | 2.4% |
| RETURN_VALUE | 3,443,387 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,094,592 | 100.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,540,261 | 75.4% |
| LOAD_CONST | 172,936,750 | 24.6% |
| SEND | 6,208 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,524,133 | 75.4% |
| POP_TOP | 172,924,510 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,676 | 0.0% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,996,640 | 99.7% |
| LOAD_ATTR_WITH_HINT | 8,600 | 0.3% |
| CALL | 400 | 0.0% |
| LOAD_FAST | 160 | 0.0% |
| CALL_KW | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 3,005,920 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,923,479 | 85.5% |
| STORE_FAST | 1,283,708 | 12.3% |
| STORE_DEREF | 185,686 | 1.8% |
| STORE_NAME | 35,740 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,276,974 | 79.3% |
| STORE_DEREF | 2,092,419 | 20.1% |
| STORE_NAME | 59,020 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 378,820,300 | 72.1% |
| LOAD_FAST | 91,321,015 | 17.4% |
| RETURN_VALUE | 23,049,480 | 4.4% |
| BINARY_OP_MULTIPLY_INT | 11,249,600 | 2.1% |
| BINARY_OP | 8,323,476 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 155,333,959 | 29.5% |
| STORE_FAST | 154,796,710 | 29.4% |
| LOAD_FAST | 84,006,666 | 16.0% |
| RETURN_VALUE | 41,800,520 | 8.0% |
| LOAD_FAST_LOAD_FAST | 39,159,100 | 7.4% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 718,883,480 | 65.1% |
| LOAD_ATTR_INSTANCE_VALUE | 158,346,040 | 14.3% |
| BINARY_SUBSCR | 90,267,920 | 8.2% |
| LOAD_FAST_LOAD_FAST | 78,973,160 | 7.2% |
| CALL_BUILTIN_CLASS | 17,043,680 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 378,820,300 | 34.3% |
| YIELD_VALUE | 281,242,200 | 25.5% |
| LOAD_FAST | 148,369,380 | 13.4% |
| BINARY_OP_SUBTRACT_FLOAT | 145,713,640 | 13.2% |
| STORE_FAST | 48,096,300 | 4.4% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,912,826 | 73.0% |
| UNPACK_SEQUENCE_TUPLE | 32,035,080 | 17.9% |
| STORE_FAST | 8,002,280 | 4.5% |
| CALL_KW | 7,090,880 | 4.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 970,120 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 171,284,186 | 95.5% |
| STORE_FAST | 8,118,620 | 4.5% |
| UNPACK_SEQUENCE_TUPLE | 24,040 | 0.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,833,220 | 65.4% |
| LOAD_FAST | 21,629,972 | 34.6% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,320,706 | 75.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,922,048 | 15.9% |
| LOAD_CONST | 3,231,020 | 5.2% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.6% |
| CALL | 226,158 | 0.4% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,080,152 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 49,056,660 | 64.5% |
| LOAD_FAST | 25,971,252 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,080 | 0.0% |
| NOP | 6,620 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 106,709,019 | 49.1% |
| GET_ITER | 75,660,465 | 34.8% |
| EXTENDED_ARG | 34,775,860 | 16.0% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 140,990,239 | 64.9% |
| POP_TOP | 76,209,645 | 35.1% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 1,600 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### END_ASYNC_FOR

<details>
<summary> Successors and predecessors for END_ASYNC_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 8,000,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 7,999,920 | 100.0% |
| RETURN_CONST | 80 | 0.0% |


</details>

### GET_AITER

<details>
<summary> Successors and predecessors for GET_AITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 7,999,880 | 100.0% |
| RETURN_VALUE | 80 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ANEXT | 8,000,000 | 100.0% |


</details>

### GET_ANEXT

<details>
<summary> Successors and predecessors for GET_ANEXT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 125,515,680 | 94.0% |
| GET_AITER | 8,000,000 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 133,515,680 | 100.0% |


</details>

### LOAD_LOCALS

<details>
<summary> Successors and predecessors for LOAD_LOCALS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,840 | 47.7% |
| STORE_NAME | 1,780 | 46.1% |
| LOAD_CONST | 240 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 99.5% |
| STORE_DEREF | 20 | 0.5% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,159,760 | 69.5% |
| LOAD_GLOBAL_MODULE | 189,829 | 11.4% |
| LOAD_CONST | 135,400 | 8.1% |
| LOAD_FAST | 91,926 | 5.5% |
| LOAD_ATTR | 89,040 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,159,760 | 69.5% |
| CONTAINS_OP | 190,789 | 11.4% |
| LOAD_CONST | 93,780 | 5.6% |
| BINARY_OP | 85,920 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.9% |


</details>

### CALL_INTRINSIC_2

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_2 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 60 | 75.0% |
| MAKE_FUNCTION | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60 | 75.0% |
| COPY | 20 | 25.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,285,120 | 62.1% |
| STORE_FAST | 276,016 | 13.3% |
| CALL | 189,618 | 9.2% |
| POP_TOP | 105,388 | 5.1% |
| NOP | 64,929 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.3% |
| BUILD_LIST | 642,560 | 31.1% |
| RETURN_VALUE | 266,418 | 12.9% |
| RETURN_CONST | 129,618 | 6.3% |
| JUMP_FORWARD | 127,488 | 6.2% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| FOR_ITER | 240 | 26.7% |
| STORE_NAME | 200 | 22.2% |
| POP_TOP | 40 | 4.4% |
| JUMP_FORWARD | 20 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| LOAD_NAME | 160 | 17.8% |
| LOAD_CONST | 120 | 13.3% |
| LOAD_BUILD_CLASS | 100 | 11.1% |
| BUILD_LIST | 60 | 6.7% |


</details>

### LOAD_FROM_DICT_OR_DEREF

<details>
<summary> Successors and predecessors for LOAD_FROM_DICT_OR_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_LOCALS | 3,840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,600 | 41.7% |
| CALL_PY_EXACT_ARGS | 1,560 | 40.6% |
| LOAD_CONST | 240 | 6.2% |
| LOAD_ATTR | 200 | 5.2% |
| STORE_NAME | 160 | 4.2% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 88,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 99.4% |
| STORE_FAST | 160 | 0.2% |
| STORE_NAME | 120 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.1% |
| CALL | 80 | 0.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 75,583,148 | 86.1% |
| LOAD_FAST_LOAD_FAST | 7,999,145 | 9.1% |
| LOAD_DEREF | 3,109,100 | 3.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |
| STORE_FAST_LOAD_FAST | 239,435 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 44,301,787 | 50.5% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,872 | 12.7% |
| CONTAINS_OP | 9,239,140 | 10.5% |
| CALL_BUILTIN_O | 5,609,861 | 6.4% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.0% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,631,900 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,619,260 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,920 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 87.1% |
| RETURN_GENERATOR | 4,514,712 | 12.3% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,719,752 | 100.0% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,300 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,100 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 240 | 0.1% |


</details>

### DELETE_DEREF

<details>
<summary> Successors and predecessors for DELETE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR | 1,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_FAST | 1,600 | 100.0% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 1,919,400 | 84.4% |
| STORE_FAST_LOAD_FAST | 112,000 | 4.9% |
| RETURN_VALUE | 90,660 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 83,020 | 3.7% |
| LOAD_FAST | 42,320 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 2,273,600 | 100.0% |


</details>

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 960 | 63.2% |
| CALL_INTRINSIC_1 | 320 | 21.1% |
| JUMP_BACKWARD | 240 | 15.8% |


</details>

### FORMAT_WITH_SPEC

<details>
<summary> Successors and predecessors for FORMAT_WITH_SPEC </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,280 | 84.2% |
| LOAD_CONST | 240 | 15.8% |


</details>

### SETUP_ANNOTATIONS

<details>
<summary> Successors and predecessors for SETUP_ANNOTATIONS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 340 | 63.0% |
| RESUME | 200 | 37.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 500 | 92.6% |
| LOAD_NAME | 40 | 7.4% |


</details>


</details>

## Specialization stats

<details>
<summary> specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,174,985,752 | 16.3% |
|          hit | 6,036,433,884 | 83.7% |
|         miss | 50,410,867 | 0.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 999,595 | 37.7% |
| Failure | 1,651,262 | 62.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 777,368 | 47.1% |
| multiply different types | 249,960 | 15.1% |
| add different types | 216,464 | 13.1% |
| add other | 65,512 | 4.0% |
| and int | 62,814 | 3.8% |
| remainder | 60,359 | 3.7% |
| floor divide | 51,872 | 3.1% |
| rshift | 29,710 | 1.8% |
| lshift | 28,583 | 1.7% |
| true divide different types | 25,023 | 1.5% |
| xor | 18,643 | 1.1% |
| or | 18,495 | 1.1% |
| subtract other | 16,000 | 1.0% |
| true divide float | 11,643 | 0.7% |
| power | 8,901 | 0.5% |
| multiply other | 4,320 | 0.3% |
| true divide other | 3,340 | 0.2% |
| and other | 1,715 | 0.1% |
| and different types | 540 | 0.0% |


</details>

### BINARY_SLICE

<details>
<summary> specialization stats for BINARY_SLICE family </summary>


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,486,755,359 | 26.4% |
|          hit | 4,145,168,534 | 73.6% |
|         miss | 4,791,330 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,695 | 30.0% |
| Failure | 441,834 | 70.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| array int | 157,600 | 35.7% |
| other | 121,344 | 27.5% |
| out of range | 76,800 | 17.4% |
| buffer int | 41,967 | 9.5% |
| list slice | 34,620 | 7.8% |
| sequence int | 4,280 | 1.0% |
| code complex parameters | 4,080 | 0.9% |
| buffer slice | 960 | 0.2% |
| string slice | 100 | 0.0% |
| tuple slice | 83 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,336,844,927 | 10.8% |
|        deopt | 31,040 | 0.0% |
|          hit | 11,074,232,879 | 89.2% |
|         miss | 230,083,062 | 1.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,851,292 | 85.2% |
| Failure | 839,526 | 14.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,561 | 21.3% |
| code complex parameters | 154,016 | 18.3% |
| no dict | 100,658 | 12.0% |
| cfunc noargs | 67,141 | 8.0% |
| class no vectorcall | 64,231 | 7.7% |
| meth descr varargs | 62,166 | 7.4% |
| class mutable | 51,001 | 6.1% |
| other | 33,100 | 3.9% |
| cfunc varargs keywords | 27,881 | 3.3% |
| meth descr varargs keywords | 17,969 | 2.1% |
| init not python | 17,060 | 2.0% |
| cmethod | 11,820 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cfunc varargs | 11,010 | 1.3% |
| bound method | 10,028 | 1.2% |
| wrong number arguments | 9,580 | 1.1% |
| operator wrapper | 5,448 | 0.6% |
| method wrapper | 4,496 | 0.5% |
| str | 1,700 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 207,601,614 | 4.6% |
|          hit | 4,316,870,055 | 95.4% |
|         miss | 1,894,869 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,886 | 29.5% |
| Failure | 235,889 | 70.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,956 | 25.8% |
| different types | 52,008 | 22.0% |
| baseobject | 30,500 | 12.9% |
| other | 24,292 | 10.3% |
| float long | 19,592 | 8.3% |
| tuple | 14,654 | 6.2% |
| string | 10,600 | 4.5% |
| set | 9,840 | 4.2% |
| bool | 5,158 | 2.2% |
| bytes | 3,480 | 1.5% |
| list | 3,220 | 1.4% |
| long float | 1,589 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 663,708,746 | 18.1% |
|          hit | 2,999,173,768 | 81.8% |
|         miss | 174,929,248 | 4.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,351,765 | 91.7% |
| Failure | 304,957 | 8.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 111,488 | 36.6% |
| enumerate | 43,449 | 14.2% |
| set | 37,204 | 12.2% |
| seq iter | 29,860 | 9.8% |
| other | 19,460 | 6.4% |
| zip | 18,956 | 6.2% |
| dict values | 13,060 | 4.3% |
| dict keys | 8,660 | 2.8% |
| reversed list | 8,040 | 2.6% |
| itertools | 6,900 | 2.3% |
| ascii string | 5,280 | 1.7% |
| map | 1,440 | 0.5% |
| bytes | 660 | 0.2% |
| callable | 480 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,377,371,196 | 15.1% |
|        deopt | 1,816,747 | 0.0% |
|          hit | 13,382,765,047 | 84.8% |
|         miss | 753,120,338 | 4.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 14,925,767 | 92.9% |
| Failure | 1,142,218 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 316,885 | 27.7% |
| metaclass attribute | 253,183 | 22.2% |
| method | 160,412 | 14.0% |
| not managed dict | 139,737 | 12.2% |
| shadowed | 100,643 | 8.8% |
| mutable class | 68,341 | 6.0% |
| class method obj | 24,260 | 2.1% |
| overridden | 18,949 | 1.7% |
| class attr descriptor | 17,780 | 1.6% |
| non overriding descriptor | 11,348 | 1.0% |
| module attr not found | 10,700 | 0.9% |
| not in keys | 7,260 | 0.6% |
| class attr simple | 6,180 | 0.5% |
| non object slot | 3,500 | 0.3% |
| builtin class method | 2,980 | 0.3% |
| property | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,626,694 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 9,710,372,491 | 99.9% |
|         miss | 331,212 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,200 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,243 | 0.0% |
|          hit | 126,149,728 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,100 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


</details>

### POP_JUMP_IF_NONE

<details>
<summary> specialization stats for POP_JUMP_IF_NONE family </summary>


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> specialization stats for POP_JUMP_IF_NOT_NONE family </summary>


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> specialization stats for POP_JUMP_IF_TRUE family </summary>


</details>

### SEND

<details>
<summary> specialization stats for SEND family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 165,295,884 | 19.0% |
|          hit | 702,452,319 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,208 | 10.6% |
| Failure | 52,563 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,883 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 257,093,265 | 9.4% |
|          hit | 2,487,632,157 | 90.5% |
|         miss | 193,581,113 | 7.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,784,965 | 97.5% |
| Failure | 97,126 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 46,060 | 47.4% |
| not in dict | 15,940 | 16.4% |
| overriding descriptor | 10,640 | 11.0% |
| not in keys | 7,820 | 8.1% |
| overridden | 5,180 | 5.3% |
| property | 4,160 | 4.3% |
| no dict | 3,120 | 3.2% |
| not managed dict | 2,646 | 2.7% |
| method | 1,540 | 1.6% |
| mutable class | 20 | 0.0% |


</details>

### STORE_SLICE

<details>
<summary> specialization stats for STORE_SLICE family </summary>


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 440,683,671 | 38.8% |
|          hit | 694,350,788 | 61.2% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,160 | 9.3% |
| Failure | 157,558 | 90.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| array int | 66,240 | 42.0% |
| py simple | 43,498 | 27.6% |
| dict subclass no override | 34,860 | 22.1% |
| bytearray int | 9,320 | 5.9% |
| out of range | 2,820 | 1.8% |
| other | 800 | 0.5% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 470,404,341 | 7.2% |
|          hit | 6,050,037,261 | 92.7% |
|         miss | 125,379,336 | 1.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,590,735 | 79.3% |
| Failure | 677,109 | 20.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 181,681 | 26.8% |
| other | 173,186 | 25.6% |
| tuple | 112,625 | 16.6% |
| mapping | 98,881 | 14.6% |
| dict | 35,551 | 5.3% |
| set | 33,027 | 4.9% |
| bytes | 19,253 | 2.8% |
| sequence | 18,648 | 2.8% |
| float | 2,600 | 0.4% |
| bytearray | 1,237 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,191,332 | 0.2% |
|          hit | 1,668,983,077 | 99.8% |
|         miss | 2,972,240 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,044 | 97.5% |
| Failure | 2,515 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,455 | 57.9% |
| iterator | 680 | 27.0% |
| other | 380 | 15.1% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 118,174,875,908 | 55.4% |
| Not specialized | 22,806,425,905 | 10.7% |
| Specialized hits | 70,752,367,387 | 33.2% |
| Specialized misses | 1,537,697,644 | 0.7% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,377,371,196 | 27.7% |
| BINARY_SUBSCR | 1,486,755,359 | 17.3% |
| CALL | 1,336,844,927 | 15.6% |
| BINARY_OP | 1,174,985,752 | 13.7% |
| FOR_ITER | 663,708,746 | 7.7% |
| TO_BOOL | 470,404,341 | 5.5% |
| STORE_SUBSCR | 440,683,671 | 5.1% |
| STORE_ATTR | 257,093,265 | 3.0% |
| COMPARE_OP | 207,601,614 | 2.4% |
| SEND | 165,295,884 | 1.9% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 286,581,736 | 18.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 215,493,857 | 14.0% |
| LOAD_ATTR_SLOT | 110,891,100 | 7.2% |
| CALL_PY_EXACT_ARGS | 107,973,167 | 7.0% |
| STORE_ATTR_INSTANCE_VALUE | 99,629,995 | 6.5% |
| STORE_ATTR_SLOT | 93,892,140 | 6.1% |
| FOR_ITER_LIST | 87,622,153 | 5.7% |
| FOR_ITER_TUPLE | 87,236,135 | 5.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,348,423 | 4.4% |
| TO_BOOL_NONE | 61,182,845 | 4.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,002,529,279 | 25.0% |
| Calls to Python functions inlined | 6,002,196,840 | 75.0% |
| Calls via PyEval_EvalFrame (total) | 2,002,529,279 | 25.0% |
| Calls via PyEval_EvalFrame (vector) | 1,223,206,536 | 15.3% |
| Calls via PyEval_EvalFrame (generator) | 779,322,743 | 9.7% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,217,891,636 | 15.2% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,034,045 | 4.2% |
| Calls via PyEval_EvalFrame (function ex) | 28,945,868 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 231,360,488 | 2.9% |
| Calls via PyEval_EvalFrame (method) | 212,969,530 | 2.7% |
| Frame objects created | 62,510,418 | 0.8% |
| Frames pushed | 4,674,884,834 | 58.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,041,528,898 | 36.0% |
| Frees to freelist | 6,043,435,276 |  |
| Allocations | 10,753,802,497 | 64.0% |
| Allocations to 512 bytes | 10,638,606,796 | 63.3% |
| Allocations to 4 kbytes | 94,937,118 | 0.6% |
| Allocations over 4 kbytes | 20,258,583 | 0.1% |
| Frees | 11,027,164,542 |  |
| New values | 73,367,022 |  |
| Interpreter increfs | 81,454,080,333 | 77.2% |
| Interpreter decrefs | 94,631,028,676 | 78.1% |
| Increfs | 24,006,543,342 | 22.8% |
| Decrefs | 26,564,113,646 | 21.9% |
| Materialize dict (on request) | 5,306,280 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,200 | 2.8% |
| Method cache hits | 2,839,269,032 |  |
| Method cache misses | 79,897,358 |  |
| Method cache collisions | 91,057,919 |  |
| Method cache dunder hits | 3,228,880,544 |  |
| Method cache dunder misses | 11,330,523 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 0 | 0 | 0 |
| 1 | 0 | 116,897,698 | 17,551,132,993 |
| 2 | 0 | 10,753,920 | 6,929,120,640 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 0 |  |
| Traces created | 0 |  |
| Trace stack overflow | 0 |  |
| Trace stack underflow | 0 |  |
| Trace too long | 0 |  |
| Trace too short | 0 |  |
| Inner loop found | 0 |  |
| Recursive call | 0 |  |
| Low confidence | 0 |  |
| Traces executed | 0 |  |
| Uops executed | 0 |  |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 1,920 |


</details>

---
Stats gathered on: 2024-01-08
