
# Pystats results

- benchmark: concurrent_imap
- fork: python
- ref: 1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8
- commit hash: 1ae7ceb
- commit date: 2024-01-04T15:05:31+01:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 99,754,262 | 17.6% | 17.6% |  |
| RESUME_CHECK | 36,842,892 | 6.5% | 24.1% | 0.0% |
| STORE_FAST | 29,305,243 | 5.2% | 29.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 24,259,489 | 4.3% | 33.6% | 0.9% |
| POP_TOP | 23,912,589 | 4.2% | 37.8% |  |
| RETURN_VALUE | 21,787,565 | 3.8% | 41.7% |  |
| POP_JUMP_IF_FALSE | 18,972,099 | 3.4% | 45.0% |  |
| JUMP_BACKWARD | 17,944,964 | 3.2% | 48.2% |  |
| LOAD_GLOBAL_MODULE | 16,764,199 | 3.0% | 51.1% | 0.0% |
| LOAD_FAST_LOAD_FAST | 15,467,726 | 2.7% | 53.9% |  |
| LOAD_CONST | 15,377,968 | 2.7% | 56.6% |  |
| CALL_PY_EXACT_ARGS | 12,288,810 | 2.2% | 58.8% | 0.0% |
| INTERPRETER_EXIT | 11,846,098 | 2.1% | 60.9% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 10,985,515 | 1.9% | 62.8% | 0.7% |
| CALL | 10,887,547 | 1.9% | 64.7% |  |
| LOAD_ATTR | 10,207,368 | 1.8% | 66.5% |  |
| FOR_ITER_LIST | 9,928,970 | 1.8% | 68.3% |  |
| NOP | 9,889,426 | 1.7% | 70.0% |  |
| RETURN_CONST | 9,176,937 | 1.6% | 71.6% |  |
| LOAD_GLOBAL_BUILTIN | 8,593,915 | 1.5% | 73.2% | 0.0% |
| PUSH_NULL | 7,343,217 | 1.3% | 74.5% |  |
| COPY | 7,188,873 | 1.3% | 75.7% |  |
| BINARY_OP | 6,925,690 | 1.2% | 76.9% |  |
| TO_BOOL_BOOL | 6,925,375 | 1.2% | 78.2% |  |
| YIELD_VALUE | 6,913,660 | 1.2% | 79.4% |  |
| STORE_FAST_LOAD_FAST | 6,464,820 | 1.1% | 80.5% |  |
| LOAD_ATTR_METHOD_NO_DICT | 6,374,803 | 1.1% | 81.7% |  |
| FOR_ITER_GEN | 6,347,440 | 1.1% | 82.8% |  |
| TO_BOOL_INT | 5,113,224 | 0.9% | 83.7% |  |
| POP_JUMP_IF_NOT_NONE | 5,012,022 | 0.9% | 84.6% |  |
| STORE_FAST_STORE_FAST | 4,811,089 | 0.8% | 85.4% |  |
| STORE_ATTR_INSTANCE_VALUE | 4,379,355 | 0.8% | 86.2% | 5.6% |
| BUILD_TUPLE | 4,265,118 | 0.8% | 86.9% |  |
| COMPARE_OP_INT | 3,709,851 | 0.7% | 87.6% | 0.2% |
| LOAD_ATTR_MODULE | 3,567,679 | 0.6% | 88.2% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 2,897,857 | 0.5% | 88.7% |  |
| POP_JUMP_IF_TRUE | 2,727,174 | 0.5% | 89.2% |  |
| SWAP | 2,580,983 | 0.5% | 89.7% |  |
| CALL_FUNCTION_EX | 2,413,983 | 0.4% | 90.1% |  |
| GET_ITER | 2,350,452 | 0.4% | 90.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,123,809 | 0.4% | 90.9% |  |
| CALL_BUILTIN_CLASS | 1,985,119 | 0.4% | 91.2% |  |
| BEFORE_WITH | 1,844,022 | 0.3% | 91.6% |  |
| CALL_BUILTIN_FAST | 1,808,081 | 0.3% | 91.9% |  |
| LOAD_DEREF | 1,803,227 | 0.3% | 92.2% |  |
| COPY_FREE_VARS | 1,753,167 | 0.3% | 92.5% |  |
| CONTAINS_OP | 1,730,564 | 0.3% | 92.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,693,552 | 0.3% | 93.1% |  |
| JUMP_FORWARD | 1,679,780 | 0.3% | 93.4% |  |
| BUILD_MAP | 1,664,083 | 0.3% | 93.7% |  |
| LOAD_SUPER_ATTR_METHOD | 1,656,847 | 0.3% | 94.0% |  |
| UNARY_INVERT | 1,652,892 | 0.3% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,644,638 | 0.3% | 94.6% | 0.0% |
| TO_BOOL | 1,582,482 | 0.3% | 94.9% |  |
| BUILD_LIST | 1,489,246 | 0.3% | 95.1% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,489,194 | 0.3% | 95.4% |  |
| COMPARE_OP_STR | 1,478,966 | 0.3% | 95.7% |  |
| FOR_ITER | 1,305,260 | 0.2% | 95.9% |  |
| STORE_SUBSCR_DICT | 1,244,995 | 0.2% | 96.1% |  |
| CALL_ISINSTANCE | 1,171,304 | 0.2% | 96.3% |  |
| UNPACK_SEQUENCE_TUPLE | 1,169,508 | 0.2% | 96.5% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,138,228 | 0.2% | 96.7% | 0.0% |
| POP_JUMP_IF_NONE | 1,116,529 | 0.2% | 96.9% |  |
| BINARY_OP_ADD_INT | 1,112,440 | 0.2% | 97.1% |  |
| EXIT_INIT_CHECK | 1,035,146 | 0.2% | 97.3% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,035,146 | 0.2% | 97.5% |  |
| LOAD_ATTR_PROPERTY | 1,014,083 | 0.2% | 97.7% | 1.2% |
| CALL_METHOD_DESCRIPTOR_O | 968,530 | 0.2% | 97.8% | 0.0% |
| LOAD_FAST_CHECK | 827,132 | 0.1% | 98.0% |  |
| LIST_APPEND | 811,008 | 0.1% | 98.1% |  |
| FOR_ITER_RANGE | 752,383 | 0.1% | 98.3% |  |
| LOAD_FAST_AND_CLEAR | 747,514 | 0.1% | 98.4% |  |
| BINARY_SUBSCR | 637,179 | 0.1% | 98.5% |  |
| CALL_LEN | 623,450 | 0.1% | 98.6% |  |
| CALL_TUPLE_1 | 583,120 | 0.1% | 98.7% |  |
| COMPARE_OP | 573,775 | 0.1% | 98.8% |  |
| DICT_MERGE | 564,260 | 0.1% | 98.9% |  |
| TO_BOOL_LIST | 538,003 | 0.1% | 99.0% |  |
| BINARY_SUBSCR_LIST_INT | 477,812 | 0.1% | 99.1% |  |
| LIST_EXTEND | 467,692 | 0.1% | 99.2% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 408,972 | 0.1% | 99.2% |  |
| CALL_KW | 349,904 | 0.1% | 99.3% |  |
| BINARY_OP_SUBTRACT_INT | 330,435 | 0.1% | 99.4% |  |
| CALL_LIST_APPEND | 261,614 | 0.0% | 99.4% |  |
| BINARY_OP_ADD_FLOAT | 250,357 | 0.0% | 99.5% |  |
| UNARY_NOT | 249,649 | 0.0% | 99.5% |  |
| TO_BOOL_NONE | 240,449 | 0.0% | 99.5% | 0.1% |
| BINARY_OP_SUBTRACT_FLOAT | 233,789 | 0.0% | 99.6% |  |
| CALL_BUILTIN_O | 154,400 | 0.0% | 99.6% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 142,325 | 0.0% | 99.6% | 4.5% |
| MAKE_CELL | 137,900 | 0.0% | 99.7% |  |
| STORE_DEREF | 137,660 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_DICT | 114,880 | 0.0% | 99.7% |  |
| BINARY_OP_MULTIPLY_FLOAT | 112,600 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_STR_INT | 112,600 | 0.0% | 99.7% |  |
| STORE_ATTR | 100,860 | 0.0% | 99.8% |  |
| LOAD_ATTR_SLOT | 99,760 | 0.0% | 99.8% |  |
| STORE_ATTR_SLOT | 97,980 | 0.0% | 99.8% |  |
| LOAD_ATTR_CLASS | 91,488 | 0.0% | 99.8% |  |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 0.0% | 99.8% |  |
| DELETE_ATTR | 86,388 | 0.0% | 99.8% |  |
| DELETE_SUBSCR | 78,212 | 0.0% | 99.9% |  |
| MAKE_FUNCTION | 63,680 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 55,680 | 0.0% | 99.9% |  |
| POP_EXCEPT | 49,319 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 49,319 | 0.0% | 99.9% |  |
| IS_OP | 46,997 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 43,559 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 43,340 | 0.0% | 99.9% |  |
| BUILD_STRING | 41,600 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,160 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 39,040 | 0.0% | 99.9% |  |
| IMPORT_NAME | 33,760 | 0.0% | 99.9% |  |
| IMPORT_FROM | 33,420 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 31,260 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 30,220 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 28,160 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 27,480 | 0.0% | 100.0% |  |
| BINARY_SLICE | 19,820 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 18,900 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,844 | 0.0% | 100.0% |  |
| RERAISE | 17,280 | 0.0% | 100.0% |  |
| CALL_STR_1 | 11,900 | 0.0% | 100.0% |  |
| END_FOR | 11,520 | 0.0% | 100.0% |  |
| STORE_NAME | 7,480 | 0.0% | 100.0% |  |
| RESUME | 5,980 | 0.0% | 100.0% | 0.1% |
| RAISE_VARARGS | 5,780 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 5,760 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 3,840 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 2,800 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,200 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 1,440 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 957 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 920 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 560 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 520 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 280 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 160 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 140 | 0.0% | 100.0% | 14.3% |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 21,945,316 | 3.9% | 3.9% |
| RESUME_CHECK LOAD_FAST | 20,639,448 | 3.6% | 7.5% |
| STORE_FAST LOAD_FAST | 12,722,994 | 2.2% | 9.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 12,242,210 | 2.2% | 11.9% |
| CACHE RESUME_CHECK | 11,732,222 | 2.1% | 14.0% |
| LOAD_FAST RETURN_VALUE | 10,612,540 | 1.9% | 15.9% |
| RETURN_VALUE INTERPRETER_EXIT | 10,389,667 | 1.8% | 17.7% |
| POP_TOP JUMP_BACKWARD | 8,685,734 | 1.5% | 19.2% |
| JUMP_BACKWARD FOR_ITER_LIST | 7,894,424 | 1.4% | 20.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 7,880,276 | 1.4% | 22.0% |
| LOAD_FAST LOAD_ATTR | 7,871,027 | 1.4% | 23.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 7,791,055 | 1.4% | 24.8% |
| POP_TOP LOAD_FAST | 7,384,765 | 1.3% | 26.1% |
| RESUME_CHECK POP_TOP | 6,913,520 | 1.2% | 27.3% |
| RETURN_CONST POP_TOP | 6,477,537 | 1.1% | 28.5% |
| JUMP_BACKWARD FOR_ITER_GEN | 6,335,920 | 1.1% | 29.6% |
| YIELD_VALUE STORE_FAST | 6,335,920 | 1.1% | 30.7% |
| FOR_ITER_GEN RESUME_CHECK | 6,335,920 | 1.1% | 31.8% |
| NOP LOAD_FAST | 6,291,421 | 1.1% | 32.9% |
| FOR_ITER_LIST STORE_FAST_LOAD_FAST | 5,760,060 | 1.0% | 34.0% |
| STORE_FAST JUMP_BACKWARD | 5,760,000 | 1.0% | 35.0% |
| STORE_FAST_LOAD_FAST YIELD_VALUE | 5,760,000 | 1.0% | 36.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 5,549,804 | 1.0% | 37.0% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 5,535,635 | 1.0% | 37.9% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 5,113,084 | 0.9% | 38.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,107,639 | 0.9% | 39.8% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 4,823,085 | 0.9% | 40.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 4,764,473 | 0.8% | 41.4% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,965,293 | 0.7% | 42.1% |
| LOAD_FAST LOAD_CONST | 3,904,652 | 0.7% | 42.8% |
| LOAD_CONST LOAD_CONST | 3,798,902 | 0.7% | 43.5% |
| STORE_FAST NOP | 3,783,101 | 0.7% | 44.2% |
| LOAD_GLOBAL_MODULE BINARY_OP | 3,709,746 | 0.7% | 44.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,706,042 | 0.7% | 45.5% |
| LOAD_FAST PUSH_NULL | 3,673,367 | 0.6% | 46.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,671,301 | 0.6% | 46.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,588,031 | 0.6% | 47.4% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,579,054 | 0.6% | 48.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 3,564,439 | 0.6% | 48.7% |
| PUSH_NULL LOAD_FAST | 3,464,768 | 0.6% | 49.3% |
| LOAD_ATTR LOAD_FAST | 3,416,626 | 0.6% | 49.9% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 3,327,791 | 0.6% | 50.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 3,107,049 | 0.5% | 51.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 3,058,217 | 0.5% | 51.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 3,018,372 | 0.5% | 52.1% |
| BINARY_OP COPY | 2,806,276 | 0.5% | 52.6% |
| COPY TO_BOOL_INT | 2,805,956 | 0.5% | 53.1% |
| COPY STORE_FAST | 2,630,400 | 0.5% | 53.6% |
| STORE_FAST COPY | 2,629,760 | 0.5% | 54.0% |
| CALL STORE_FAST | 2,614,327 | 0.5% | 54.5% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,605,314 | 0.5% | 54.9% |
| LOAD_CONST CALL | 2,592,986 | 0.5% | 55.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 2,484,192 | 0.4% | 55.8% |
| CALL RETURN_VALUE | 2,456,344 | 0.4% | 56.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,407,746 | 0.4% | 56.7% |
| LOAD_ATTR_MODULE PUSH_NULL | 2,258,745 | 0.4% | 57.1% |
| RETURN_VALUE STORE_FAST | 2,250,220 | 0.4% | 57.5% |
| CALL POP_TOP | 2,240,999 | 0.4% | 57.9% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,147,252 | 0.4% | 58.3% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 2,116,749 | 0.4% | 58.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,107,344 | 0.4% | 59.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,032,184 | 0.4% | 59.4% |
| PUSH_NULL CALL | 2,023,891 | 0.4% | 59.7% |
| LOAD_CONST COMPARE_OP_INT | 2,020,907 | 0.4% | 60.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 2,020,710 | 0.4% | 60.4% |
| RETURN_VALUE RETURN_VALUE | 1,935,620 | 0.3% | 60.8% |
| POP_TOP RETURN_CONST | 1,910,378 | 0.3% | 61.1% |
| LOAD_FAST_LOAD_FAST CALL | 1,893,235 | 0.3% | 61.5% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,852,681 | 0.3% | 61.8% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,849,830 | 0.3% | 62.1% |
| LOAD_FAST CALL_FUNCTION_EX | 1,849,703 | 0.3% | 62.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,799,686 | 0.3% | 62.8% |
| NOP LOAD_GLOBAL_MODULE | 1,760,155 | 0.3% | 63.1% |
| COPY_FREE_VARS RESUME_CHECK | 1,752,507 | 0.3% | 63.4% |
| LOAD_DEREF LOAD_FAST | 1,746,887 | 0.3% | 63.7% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,746,367 | 0.3% | 64.0% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 1,744,473 | 0.3% | 64.3% |
| POP_TOP LOAD_CONST | 1,740,342 | 0.3% | 64.6% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 1,729,944 | 0.3% | 64.9% |
| LOAD_ATTR_INSTANCE_VALUE CONTAINS_OP | 1,729,284 | 0.3% | 65.2% |
| LOAD_FAST BUILD_TUPLE | 1,720,264 | 0.3% | 65.5% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,689,036 | 0.3% | 65.8% |
| LOAD_CONST LOAD_FAST | 1,675,764 | 0.3% | 66.1% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 1,656,647 | 0.3% | 66.4% |
| UNARY_INVERT BINARY_OP | 1,652,892 | 0.3% | 66.7% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 1,636,827 | 0.3% | 67.0% |
| FOR_ITER_LIST STORE_FAST | 1,634,816 | 0.3% | 67.3% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,587,788 | 0.3% | 67.6% |
| GET_ITER FOR_ITER_LIST | 1,551,446 | 0.3% | 67.8% |
| POP_TOP NOP | 1,549,427 | 0.3% | 68.1% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,547,334 | 0.3% | 68.4% |
| LOAD_FAST TO_BOOL | 1,520,962 | 0.3% | 68.7% |
| LOAD_FAST GET_ITER | 1,481,426 | 0.3% | 68.9% |
| RETURN_VALUE POP_TOP | 1,468,997 | 0.3% | 69.2% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,452,969 | 0.3% | 69.4% |
| POP_JUMP_IF_FALSE POP_TOP | 1,447,054 | 0.3% | 69.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,441,863 | 0.3% | 69.9% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,439,986 | 0.3% | 70.2% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,439,877 | 0.3% | 70.5% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,430,143 | 0.3% | 70.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 18,520 | 93.4% |
| LOAD_CONST | 980 | 4.9% |
| LOAD_FAST | 280 | 1.4% |
| BINARY_OP | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 18,900 | 95.4% |
| BUILD_TUPLE | 280 | 1.4% |
| LOAD_DEREF | 280 | 1.4% |
| STORE_FAST | 280 | 1.4% |
| CALL | 80 | 0.4% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,732,222 | 99.0% |
| COPY_FREE_VARS | 109,900 | 0.9% |
| POP_TOP | 7,460 | 0.1% |
| RESUME | 2,280 | 0.0% |
| MAKE_CELL | 20 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,253,743 | 68.0% |
| RETURN_VALUE | 483,703 | 26.2% |
| LOAD_GLOBAL_MODULE | 82,436 | 4.5% |
| LOAD_FAST | 17,280 | 0.9% |
| CALL | 6,360 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,354,659 | 73.5% |
| STORE_FAST | 489,363 | 26.5% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 27,440 | 99.9% |
| BINARY_OP | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 27,480 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 576,080 | 90.4% |
| LOAD_CONST | 60,139 | 9.4% |
| BINARY_SUBSCR | 880 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 575,920 | 90.4% |
| STORE_FAST | 59,859 | 9.4% |
| BINARY_SUBSCR | 880 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 38,399 | 88.2% |
| LOAD_ATTR_MODULE | 5,100 | 11.7% |
| LOAD_GLOBAL | 40 | 0.1% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 43,559 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,896 | 48.5% |
| CALL | 27,516 | 35.2% |
| LOAD_ATTR_INSTANCE_VALUE | 12,720 | 16.3% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60,796 | 77.7% |
| RETURN_CONST | 10,236 | 13.1% |
| LOAD_FAST | 7,040 | 9.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.2% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 5,760 | 50.0% |
| LOAD_FAST | 5,760 | 50.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,035,146 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,035,146 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 28,160 | 50.6% |
| LOAD_FAST | 27,520 | 49.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 41,600 | 74.7% |
| BUILD_STRING | 14,080 | 25.3% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,481,426 | 63.0% |
| STORE_FAST_LOAD_FAST | 576,000 | 24.5% |
| CALL_BUILTIN_CLASS | 265,486 | 11.3% |
| CALL | 14,340 | 0.6% |
| RETURN_VALUE | 5,760 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,551,446 | 66.0% |
| LOAD_FAST_AND_CLEAR | 497,760 | 21.2% |
| FOR_ITER_RANGE | 258,569 | 11.0% |
| FOR_ITER | 12,117 | 0.5% |
| FOR_ITER_TUPLE | 11,740 | 0.5% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,389,667 | 87.7% |
| RETURN_CONST | 878,691 | 7.4% |
| YIELD_VALUE | 577,740 | 4.9% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 500 | 89.3% |
| POP_TOP | 60 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 560 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 63,680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 39,040 | 61.3% |
| STORE_FAST | 14,080 | 22.1% |
| LOAD_FAST | 7,040 | 11.1% |
| STORE_NAME | 2,480 | 3.9% |
| LOAD_CONST | 560 | 0.9% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,783,101 | 38.3% |
| POP_TOP | 1,549,427 | 15.7% |
| RESUME_CHECK | 1,355,084 | 13.7% |
| POP_JUMP_IF_FALSE | 1,320,806 | 13.4% |
| JUMP_BACKWARD | 1,088,000 | 11.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,291,421 | 63.6% |
| LOAD_GLOBAL_MODULE | 1,760,155 | 17.8% |
| LOAD_GLOBAL_BUILTIN | 713,150 | 7.2% |
| LOAD_FAST_LOAD_FAST | 583,320 | 5.9% |
| LOAD_CONST | 529,460 | 5.4% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 32,299 | 65.5% |
| COPY | 11,520 | 23.4% |
| POP_TOP | 5,200 | 10.5% |
| STORE_FAST | 280 | 0.6% |
| STORE_SUBSCR_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 32,599 | 66.1% |
| RERAISE | 11,520 | 23.4% |
| JUMP_FORWARD | 5,120 | 10.4% |
| RETURN_CONST | 60 | 0.1% |
| LOAD_FAST | 20 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,913,520 | 28.9% |
| RETURN_CONST | 6,477,537 | 27.1% |
| CALL | 2,240,999 | 9.4% |
| RETURN_VALUE | 1,468,997 | 6.1% |
| POP_JUMP_IF_FALSE | 1,447,054 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 8,685,734 | 36.3% |
| LOAD_FAST | 7,384,765 | 30.9% |
| RETURN_CONST | 1,910,378 | 8.0% |
| LOAD_CONST | 1,740,342 | 7.3% |
| NOP | 1,549,427 | 6.5% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 38,019 | 77.1% |
| RERAISE | 5,760 | 11.7% |
| CALL_KW | 5,120 | 10.4% |
| BINARY_SUBSCR_DICT | 300 | 0.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 38,359 | 77.8% |
| WITH_EXCEPT_START | 5,760 | 11.7% |
| LOAD_GLOBAL_MODULE | 5,080 | 10.3% |
| LOAD_GLOBAL | 120 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,673,367 | 50.0% |
| LOAD_ATTR_MODULE | 2,258,745 | 30.8% |
| LOAD_ATTR | 1,284,385 | 17.5% |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,464,768 | 47.2% |
| CALL | 2,023,891 | 27.6% |
| LOAD_FAST_LOAD_FAST | 1,396,276 | 19.0% |
| LOAD_CONST | 320,997 | 4.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 64,665 | 0.9% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 18,420 | 97.5% |
| COPY_FREE_VARS | 340 | 1.8% |
| CALL | 140 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,760 | 30.5% |
| LOAD_FAST | 5,760 | 30.5% |
| STORE_FAST | 5,760 | 30.5% |
| CALL_METHOD_DESCRIPTOR_O | 1,300 | 6.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 280 | 1.5% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,612,540 | 48.7% |
| CALL | 2,456,344 | 11.3% |
| RETURN_VALUE | 1,935,620 | 8.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,547,334 | 7.1% |
| CALL_FUNCTION_EX | 1,265,523 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 10,389,667 | 47.7% |
| STORE_FAST | 2,250,220 | 10.3% |
| RETURN_VALUE | 1,935,620 | 8.9% |
| POP_TOP | 1,468,997 | 6.7% |
| LOAD_FAST_LOAD_FAST | 1,153,384 | 5.3% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 14,080 | 45.0% |
| LOAD_FAST | 10,440 | 33.4% |
| LOAD_ATTR_INSTANCE_VALUE | 5,800 | 18.6% |
| STORE_SUBSCR | 660 | 2.1% |
| LOAD_ATTR | 200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 19,960 | 63.9% |
| LOAD_GLOBAL_MODULE | 10,200 | 32.6% |
| STORE_SUBSCR | 660 | 2.1% |
| STORE_SUBSCR_DICT | 260 | 0.8% |
| LOAD_GLOBAL | 80 | 0.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,520,962 | 96.1% |
| LOAD_ATTR_INSTANCE_VALUE | 53,492 | 3.4% |
| TO_BOOL | 3,663 | 0.2% |
| LOAD_ATTR | 882 | 0.1% |
| RETURN_VALUE | 763 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 838,456 | 53.0% |
| POP_JUMP_IF_FALSE | 737,323 | 46.6% |
| TO_BOOL | 3,663 | 0.2% |
| TO_BOOL_BOOL | 2,160 | 0.1% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,153,384 | 69.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 499,428 | 30.2% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,652,892 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 249,609 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 249,649 | 100.0% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 5,680 | 98.6% |
| TO_BOOL | 80 | 1.4% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,709,746 | 53.6% |
| UNARY_INVERT | 1,652,892 | 23.9% |
| POP_JUMP_IF_FALSE | 1,153,384 | 16.7% |
| LOAD_ATTR | 263,854 | 3.8% |
| LOAD_FAST_LOAD_FAST | 84,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,806,276 | 40.5% |
| STORE_FAST | 1,417,558 | 20.5% |
| TO_BOOL_INT | 1,153,444 | 16.7% |
| UNARY_INVERT | 1,153,384 | 16.7% |
| BUILD_TUPLE | 249,754 | 3.6% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 140 | 50.0% |
| STORE_FAST | 140 | 50.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 497,760 | 33.4% |
| JUMP_FORWARD | 483,463 | 32.5% |
| LOAD_FAST | 250,417 | 16.8% |
| POP_TOP | 233,066 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 500,703 | 33.6% |
| SWAP | 497,760 | 33.4% |
| STORE_FAST | 484,923 | 32.6% |
| RETURN_VALUE | 5,120 | 0.3% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 576,000 | 34.6% |
| LOAD_FAST | 529,560 | 31.8% |
| RESUME_CHECK | 493,663 | 29.7% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 2.1% |
| POP_JUMP_IF_NOT_NONE | 17,280 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,070,783 | 64.3% |
| BUILD_TUPLE | 576,020 | 34.6% |
| STORE_FAST | 17,280 | 1.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 27,520 | 66.2% |
| FORMAT_SIMPLE | 14,080 | 33.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 27,440 | 66.0% |
| RETURN_VALUE | 14,080 | 33.8% |
| BINARY_OP | 80 | 0.2% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,720,264 | 40.3% |
| LOAD_FAST_LOAD_FAST | 1,160,320 | 27.2% |
| BUILD_MAP | 576,020 | 13.5% |
| RETURN_VALUE | 512,000 | 12.0% |
| BINARY_OP | 249,754 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,154,944 | 27.1% |
| YIELD_VALUE | 1,152,100 | 27.0% |
| BUILD_MAP | 576,000 | 13.5% |
| STORE_FAST | 512,000 | 12.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 12.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,592,986 | 23.8% |
| PUSH_NULL | 2,023,891 | 18.6% |
| LOAD_FAST_LOAD_FAST | 1,893,235 | 17.4% |
| LOAD_ATTR_METHOD_NO_DICT | 1,439,877 | 13.2% |
| BUILD_TUPLE | 1,154,944 | 10.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,614,327 | 24.0% |
| RETURN_VALUE | 2,456,344 | 22.6% |
| POP_TOP | 2,240,999 | 20.6% |
| LOAD_FAST | 1,054,960 | 9.7% |
| TO_BOOL_BOOL | 729,399 | 6.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,703 | 76.6% |
| DICT_MERGE | 564,260 | 23.4% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,265,523 | 52.4% |
| RESUME_CHECK | 535,040 | 22.2% |
| CALL_BUILTIN_CLASS | 511,960 | 21.2% |
| POP_TOP | 95,360 | 4.0% |
| STORE_FAST | 5,760 | 0.2% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 140 | 87.5% |
| CALL_FUNCTION_EX | 20 | 12.5% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 349,904 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 280,346 | 80.1% |
| LOAD_FAST | 28,800 | 8.2% |
| RETURN_VALUE | 21,120 | 6.0% |
| STORE_FAST | 14,220 | 4.1% |
| PUSH_EXC_INFO | 5,120 | 1.5% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 569,985 | 99.3% |
| COMPARE_OP | 1,255 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 603 | 0.1% |
| LOAD_GLOBAL_MODULE | 380 | 0.1% |
| LOAD_FAST | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 570,550 | 99.4% |
| COMPARE_OP | 1,255 | 0.2% |
| COMPARE_OP_INT | 1,170 | 0.2% |
| COMPARE_OP_STR | 440 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,729,284 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,729,944 | 100.0% |
| POP_JUMP_IF_TRUE | 480 | 0.0% |
| STORE_FAST | 140 | 0.0% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 14,040 | 49.9% |
| CALL_BUILTIN_FAST | 14,040 | 49.9% |
| BINARY_SUBSCR | 40 | 0.1% |
| CALL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 28,160 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 2,806,276 | 39.0% |
| STORE_FAST | 2,629,760 | 36.6% |
| LOAD_CONST | 1,100,800 | 15.3% |
| LOAD_FAST | 590,100 | 8.2% |
| STORE_ATTR_INSTANCE_VALUE | 21,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 2,805,956 | 39.0% |
| STORE_FAST | 2,630,400 | 36.6% |
| STORE_FAST_STORE_FAST | 1,093,760 | 15.2% |
| LOAD_ATTR_INSTANCE_VALUE | 575,880 | 8.0% |
| LOAD_FAST | 28,160 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 1,153,384 | 65.8% |
| CALL_ALLOC_AND_ENTER_INIT | 483,423 | 27.6% |
| CACHE | 109,900 | 6.3% |
| CALL | 5,940 | 0.3% |
| CALL_PY_EXACT_ARGS | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,752,507 | 100.0% |
| RETURN_GENERATOR | 340 | 0.0% |
| RESUME | 320 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,388 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,592 | 66.7% |
| RETURN_CONST | 27,516 | 31.9% |
| LOAD_GLOBAL_MODULE | 1,240 | 1.4% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 529,700 | 93.9% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 6.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 564,260 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,271,223 | 97.4% |
| SWAP | 14,160 | 1.1% |
| GET_ITER | 12,117 | 0.9% |
| LOAD_FAST | 6,060 | 0.5% |
| FOR_ITER | 1,700 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 688,680 | 52.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 581,600 | 44.6% |
| SWAP | 14,080 | 1.1% |
| RETURN_CONST | 11,820 | 0.9% |
| LOAD_GLOBAL_MODULE | 5,680 | 0.4% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 33,080 | 99.0% |
| STORE_NAME | 340 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 32,640 | 97.7% |
| STORE_NAME | 780 | 2.3% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 33,760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 33,080 | 98.0% |
| STORE_NAME | 680 | 2.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 27,520 | 58.6% |
| LOAD_FAST | 17,420 | 37.1% |
| LOAD_GLOBAL_MODULE | 2,017 | 4.3% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,857 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,685,734 | 48.4% |
| STORE_FAST | 5,760,000 | 32.1% |
| POP_JUMP_IF_NOT_NONE | 979,192 | 5.5% |
| LIST_APPEND | 811,008 | 4.5% |
| STORE_FAST_STORE_FAST | 581,760 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 7,894,424 | 44.0% |
| FOR_ITER_GEN | 6,335,920 | 35.3% |
| FOR_ITER | 1,271,223 | 7.1% |
| NOP | 1,088,000 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 575,960 | 3.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,041,175 | 62.0% |
| POP_TOP | 620,385 | 36.9% |
| STORE_ATTR_INSTANCE_VALUE | 7,020 | 0.4% |
| BINARY_SUBSCR_TUPLE_INT | 5,720 | 0.3% |
| POP_EXCEPT | 5,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,120,562 | 66.7% |
| BUILD_LIST | 483,463 | 28.8% |
| POP_EXCEPT | 32,299 | 1.9% |
| LOAD_GLOBAL_MODULE | 24,816 | 1.5% |
| LOAD_FAST_LOAD_FAST | 7,320 | 0.4% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 446,594 | 55.1% |
| LOAD_ATTR | 249,774 | 30.8% |
| BINARY_SUBSCR_STR_INT | 112,600 | 13.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,000 | 0.2% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 811,008 | 100.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 234,486 | 50.1% |
| RETURN_VALUE | 233,066 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,706 | 50.0% |
| STORE_FAST | 233,066 | 49.8% |
| RETURN_VALUE | 640 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.0% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,871,027 | 77.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,799,686 | 17.6% |
| LOAD_GLOBAL_MODULE | 389,986 | 3.8% |
| CALL | 83,860 | 0.8% |
| LOAD_ATTR | 22,747 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,416,626 | 33.5% |
| PUSH_NULL | 1,284,385 | 12.6% |
| STORE_SUBSCR_DICT | 1,153,304 | 11.3% |
| POP_JUMP_IF_NOT_NONE | 1,122,575 | 11.0% |
| STORE_FAST | 727,839 | 7.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,904,652 | 25.4% |
| LOAD_CONST | 3,798,902 | 24.7% |
| POP_TOP | 1,740,342 | 11.3% |
| POP_JUMP_IF_FALSE | 912,434 | 5.9% |
| LOAD_ATTR_METHOD_NO_DICT | 739,066 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,798,902 | 24.7% |
| CALL | 2,592,986 | 16.9% |
| COMPARE_OP_INT | 2,020,907 | 13.1% |
| LOAD_FAST | 1,675,764 | 10.9% |
| COPY | 1,100,800 | 7.2% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,746,367 | 96.8% |
| POP_JUMP_IF_NOT_NONE | 27,520 | 1.5% |
| STORE_DEREF | 27,520 | 1.5% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,746,887 | 96.9% |
| POP_JUMP_IF_NOT_NONE | 55,040 | 3.1% |
| PUSH_NULL | 460 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 20,639,448 | 20.7% |
| STORE_FAST | 12,722,994 | 12.8% |
| POP_JUMP_IF_FALSE | 7,791,055 | 7.8% |
| POP_TOP | 7,384,765 | 7.4% |
| NOP | 6,291,421 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 21,945,316 | 22.0% |
| RETURN_VALUE | 10,612,540 | 10.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,880,276 | 7.9% |
| LOAD_ATTR | 7,871,027 | 7.9% |
| CALL_PY_EXACT_ARGS | 5,107,639 | 5.1% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 497,760 | 66.6% |
| LOAD_FAST_AND_CLEAR | 249,754 | 33.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 497,760 | 66.6% |
| LOAD_FAST_AND_CLEAR | 249,754 | 33.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 576,560 | 69.7% |
| POP_JUMP_IF_NONE | 233,709 | 28.3% |
| LOAD_ATTR_CLASS | 16,543 | 2.0% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 69.6% |
| LOAD_GLOBAL_MODULE | 233,629 | 28.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,503 | 2.0% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,605,314 | 16.8% |
| LOAD_FAST_LOAD_FAST | 2,020,710 | 13.1% |
| POP_JUMP_IF_FALSE | 1,452,969 | 9.4% |
| PUSH_NULL | 1,396,276 | 9.0% |
| LOAD_SUPER_ATTR_METHOD | 1,167,664 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,579,054 | 23.1% |
| LOAD_FAST_LOAD_FAST | 2,020,710 | 13.1% |
| CALL | 1,893,235 | 12.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,689,036 | 10.9% |
| BUILD_TUPLE | 1,160,320 | 7.5% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,000 | 11.2% |
| RESUME_CHECK | 1,720 | 9.6% |
| POP_JUMP_IF_FALSE | 1,711 | 9.6% |
| LOAD_FAST | 1,600 | 9.0% |
| RESUME | 1,520 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,820 | 38.2% |
| LOAD_ATTR | 3,322 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,740 | 15.4% |
| LOAD_FAST | 2,162 | 12.1% |
| CALL | 740 | 4.1% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 820 | 37.3% |
| LOAD_CONST | 600 | 27.3% |
| RESUME | 560 | 25.5% |
| PUSH_NULL | 120 | 5.5% |
| POP_TOP | 80 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 640 | 29.1% |
| CALL | 500 | 22.7% |
| LOAD_ATTR | 420 | 19.1% |
| LOAD_CONST | 380 | 17.3% |
| PUSH_NULL | 220 | 10.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 200 | 38.5% |
| PUSH_NULL | 80 | 15.4% |
| LOAD_FAST_LOAD_FAST | 80 | 15.4% |
| LOAD_SUPER_ATTR_ATTR | 80 | 15.4% |
| CALL | 40 | 7.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 110,080 | 79.8% |
| CALL_PY_EXACT_ARGS | 27,800 | 20.2% |
| CACHE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 110,080 | 79.8% |
| RESUME_CHECK | 27,820 | 20.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 5,113,084 | 27.0% |
| TO_BOOL_BOOL | 4,823,085 | 25.4% |
| COMPARE_OP_INT | 3,706,042 | 19.5% |
| CONTAINS_OP | 1,729,944 | 9.1% |
| COMPARE_OP_STR | 1,439,986 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,791,055 | 41.1% |
| RETURN_CONST | 3,107,049 | 16.4% |
| LOAD_FAST_LOAD_FAST | 1,452,969 | 7.7% |
| POP_TOP | 1,447,054 | 7.6% |
| LOAD_GLOBAL_MODULE | 1,430,143 | 7.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,038,729 | 93.0% |
| LOAD_ATTR_INSTANCE_VALUE | 47,800 | 4.3% |
| LOAD_ATTR | 28,300 | 2.5% |
| RETURN_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 287,134 | 25.7% |
| LOAD_FAST | 274,750 | 24.6% |
| NOP | 270,986 | 24.3% |
| LOAD_FAST_CHECK | 233,709 | 20.9% |
| RETURN_CONST | 24,340 | 2.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,407,746 | 48.0% |
| LOAD_ATTR | 1,122,575 | 22.4% |
| LOAD_ATTR_INSTANCE_VALUE | 958,249 | 19.1% |
| RETURN_VALUE | 447,234 | 8.9% |
| LOAD_DEREF | 55,040 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,032,184 | 40.5% |
| RETURN_CONST | 1,123,999 | 22.4% |
| JUMP_BACKWARD | 979,192 | 19.5% |
| NOP | 492,242 | 9.8% |
| LOAD_CONST | 233,346 | 4.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,852,681 | 67.9% |
| TO_BOOL | 838,456 | 30.7% |
| TO_BOOL_NONE | 19,700 | 0.7% |
| COMPARE_OP_STR | 10,900 | 0.4% |
| COMPARE_OP_INT | 3,417 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 954,585 | 35.0% |
| LOAD_FAST_LOAD_FAST | 841,254 | 30.8% |
| RETURN_CONST | 744,767 | 27.3% |
| LOAD_GLOBAL_MODULE | 72,077 | 2.6% |
| RETURN_VALUE | 59,819 | 2.2% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,760 | 99.7% |
| CALL_KW | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 5,760 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 11,520 | 66.7% |
| POP_JUMP_IF_TRUE | 5,760 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,760 | 50.0% |
| COPY | 5,760 | 50.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,107,049 | 33.9% |
| STORE_ATTR_INSTANCE_VALUE | 2,147,252 | 23.4% |
| POP_TOP | 1,910,378 | 20.8% |
| POP_JUMP_IF_NOT_NONE | 1,123,999 | 12.2% |
| POP_JUMP_IF_TRUE | 744,767 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,477,537 | 70.6% |
| EXIT_INIT_CHECK | 1,035,146 | 11.3% |
| INTERPRETER_EXIT | 878,691 | 9.6% |
| TO_BOOL_BOOL | 686,746 | 7.5% |
| STORE_FAST | 61,659 | 0.7% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 39,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 37,920 | 97.1% |
| STORE_NAME | 780 | 2.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.7% |
| LOAD_FAST | 60 | 0.2% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 58,560 | 58.1% |
| LOAD_FAST_LOAD_FAST | 22,040 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 17,280 | 17.1% |
| STORE_ATTR | 2,520 | 2.5% |
| LOAD_ATTR | 240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 44,840 | 44.5% |
| LOAD_FAST_LOAD_FAST | 14,760 | 14.6% |
| LOAD_FAST | 13,620 | 13.5% |
| LOAD_CONST | 12,640 | 12.5% |
| LOAD_GLOBAL_BUILTIN | 5,680 | 5.6% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 55,040 | 40.0% |
| LOAD_GLOBAL_MODULE | 55,040 | 40.0% |
| LOAD_GLOBAL_BUILTIN | 27,520 | 20.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 54,960 | 39.9% |
| LOAD_DEREF | 27,520 | 20.0% |
| LOAD_FAST | 27,520 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 27,480 | 20.0% |
| LOAD_GLOBAL | 120 | 0.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 6,335,920 | 21.6% |
| COPY | 2,630,400 | 9.0% |
| CALL | 2,614,327 | 8.9% |
| RETURN_VALUE | 2,250,220 | 7.7% |
| FOR_ITER_LIST | 1,634,816 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,722,994 | 43.4% |
| JUMP_BACKWARD | 5,760,000 | 19.7% |
| NOP | 3,783,101 | 12.9% |
| COPY | 2,629,760 | 9.0% |
| LOAD_GLOBAL_BUILTIN | 1,173,891 | 4.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 5,760,060 | 89.1% |
| FOR_ITER | 688,680 | 10.7% |
| COPY | 14,080 | 0.2% |
| FOR_ITER_TUPLE | 2,000 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 5,760,000 | 89.1% |
| GET_ITER | 576,000 | 8.9% |
| LOAD_FAST | 112,640 | 1.7% |
| STORE_ATTR_INSTANCE_VALUE | 14,000 | 0.2% |
| TO_BOOL_STR | 2,000 | 0.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,116,749 | 44.0% |
| COPY | 1,093,760 | 22.7% |
| UNPACK_SEQUENCE_TUPLE | 1,088,220 | 22.6% |
| STORE_FAST_STORE_FAST | 512,000 | 10.6% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,587,788 | 33.0% |
| STORE_FAST | 1,088,280 | 22.6% |
| LOAD_FAST_LOAD_FAST | 1,025,341 | 21.3% |
| JUMP_BACKWARD | 581,760 | 12.1% |
| STORE_FAST_STORE_FAST | 512,000 | 10.6% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 2,480 | 33.2% |
| CALL | 1,200 | 16.0% |
| IMPORT_FROM | 780 | 10.4% |
| SET_FUNCTION_ATTRIBUTE | 780 | 10.4% |
| IMPORT_NAME | 680 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,640 | 62.0% |
| LOAD_NAME | 820 | 11.0% |
| RETURN_CONST | 700 | 9.4% |
| LOAD_BUILD_CLASS | 500 | 6.7% |
| POP_TOP | 440 | 5.9% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 575,940 | 22.3% |
| BUILD_LIST | 497,760 | 19.3% |
| LOAD_FAST_AND_CLEAR | 497,760 | 19.3% |
| FOR_ITER_LIST | 482,820 | 18.7% |
| LOAD_FAST | 261,509 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 575,880 | 22.3% |
| LOAD_CONST | 511,263 | 19.8% |
| BUILD_LIST | 497,760 | 19.3% |
| STORE_FAST | 497,760 | 19.3% |
| FOR_ITER_LIST | 482,740 | 18.7% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 260 | 28.3% |
| FOR_ITER | 240 | 26.1% |
| LOAD_FAST | 120 | 13.0% |
| RETURN_VALUE | 80 | 8.7% |
| LOAD_FAST_CHECK | 80 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 360 | 39.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 340 | 37.0% |
| UNPACK_SEQUENCE_TUPLE | 100 | 10.9% |
| LOAD_FAST | 40 | 4.3% |
| STORE_FAST | 40 | 4.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 5,760,000 | 83.3% |
| BUILD_TUPLE | 1,152,100 | 16.7% |
| CALL_STR_1 | 1,260 | 0.0% |
| CALL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,335,920 | 91.6% |
| INTERPRETER_EXIT | 577,740 | 8.4% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,820 | 47.2% |
| CACHE | 2,280 | 38.1% |
| COPY_FREE_VARS | 320 | 5.4% |
| CALL_KW | 200 | 3.3% |
| POP_TOP | 140 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,880 | 48.2% |
| LOAD_GLOBAL | 1,520 | 25.4% |
| LOAD_NAME | 560 | 9.4% |
| NOP | 280 | 4.7% |
| LOAD_CONST | 240 | 4.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 250,317 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 250,357 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,093,800 | 98.3% |
| LOAD_FAST_LOAD_FAST | 18,480 | 1.7% |
| BINARY_OP | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 575,940 | 51.8% |
| STORE_FAST | 511,980 | 46.0% |
| BINARY_SLICE | 18,520 | 1.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,680 | 0.5% |
| LOAD_CONST | 280 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,240 | 32.3% |
| CALL_METHOD_DESCRIPTOR_O | 1,240 | 32.3% |
| LOAD_FAST_LOAD_FAST | 960 | 25.0% |
| BINARY_SUBSCR_LIST_INT | 280 | 7.3% |
| LOAD_FAST | 80 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,740 | 45.3% |
| LOAD_CONST | 1,260 | 32.8% |
| CALL | 480 | 12.5% |
| STORE_FAST | 360 | 9.4% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 112,560 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 112,560 | 100.0% |
| CALL | 40 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 233,629 | 99.9% |
| BINARY_OP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 233,789 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 264,816 | 80.1% |
| LOAD_CONST | 59,739 | 18.1% |
| CALL_LEN | 5,680 | 1.7% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 324,715 | 98.3% |
| CALL_BUILTIN_CLASS | 5,680 | 1.7% |
| CALL | 40 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 99,860 | 86.9% |
| LOAD_CONST | 14,280 | 12.4% |
| LOAD_FAST | 700 | 0.6% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 99,860 | 86.9% |
| CONVERT_VALUE | 14,040 | 12.2% |
| STORE_FAST | 400 | 0.3% |
| PUSH_EXC_INFO | 300 | 0.3% |
| LOAD_FAST | 140 | 0.1% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 466,052 | 97.5% |
| LOAD_CONST | 11,640 | 2.4% |
| BINARY_SUBSCR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 466,092 | 97.5% |
| LOAD_CONST | 11,440 | 2.4% |
| BINARY_OP_ADD_UNICODE | 280 | 0.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 112,560 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 112,600 | 100.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,120 | 99.9% |
| BINARY_SUBSCR | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,020 | 84.3% |
| JUMP_FORWARD | 5,720 | 14.6% |
| STORE_FAST | 420 | 1.1% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 510,863 | 49.4% |
| LOAD_FAST | 490,583 | 47.4% |
| CALL | 33,420 | 3.2% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 551,723 | 53.3% |
| COPY_FREE_VARS | 483,423 | 46.7% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 64,665 | 45.4% |
| LOAD_FAST | 64,240 | 45.1% |
| LOAD_CONST | 7,480 | 5.3% |
| BINARY_OP_ADD_INT | 5,680 | 4.0% |
| CALL | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 135,945 | 95.5% |
| POP_TOP | 6,280 | 4.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 706,690 | 35.6% |
| CALL_FUNCTION_EX | 511,960 | 25.8% |
| LOAD_FAST | 268,097 | 13.5% |
| CALL_BUILTIN_CLASS | 232,986 | 11.7% |
| CALL_LEN | 232,986 | 11.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 762,337 | 38.4% |
| STORE_FAST | 706,990 | 35.6% |
| GET_ITER | 265,486 | 13.4% |
| CALL_BUILTIN_CLASS | 232,986 | 11.7% |
| LOAD_FAST | 17,280 | 0.9% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 872,725 | 48.3% |
| LOAD_CONST | 624,012 | 34.5% |
| LOAD_FAST_LOAD_FAST | 173,176 | 9.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,248 | 4.5% |
| LOAD_GLOBAL_MODULE | 27,880 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 613,952 | 34.0% |
| STORE_FAST | 586,910 | 32.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 449,301 | 24.8% |
| UNPACK_SEQUENCE_TUPLE | 81,248 | 4.5% |
| POP_TOP | 14,890 | 0.8% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 519,140 | 45.6% |
| BUILD_TUPLE | 511,960 | 45.0% |
| CALL | 64,965 | 5.7% |
| LOAD_FAST_CHECK | 16,503 | 1.4% |
| LOAD_ATTR | 14,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,053,900 | 92.6% |
| RETURN_VALUE | 82,148 | 7.2% |
| LOAD_FAST | 1,260 | 0.1% |
| STORE_FAST | 720 | 0.1% |
| BEFORE_WITH | 140 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 112,560 | 72.9% |
| LOAD_ATTR | 27,440 | 17.8% |
| LOAD_FAST | 14,280 | 9.2% |
| CALL | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 112,560 | 72.9% |
| LOAD_FAST | 41,520 | 26.9% |
| STORE_FAST | 140 | 0.1% |
| TO_BOOL_INT | 140 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,170,844 | 100.0% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,171,124 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 595,170 | 95.5% |
| LOAD_ATTR_INSTANCE_VALUE | 27,900 | 4.5% |
| CALL | 380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 344,256 | 55.2% |
| CALL_BUILTIN_CLASS | 232,986 | 37.4% |
| CALL_PY_EXACT_ARGS | 33,160 | 5.3% |
| LOAD_FAST | 5,720 | 0.9% |
| BINARY_OP_SUBTRACT_INT | 5,680 | 0.9% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 249,674 | 95.4% |
| LOAD_FAST | 11,440 | 4.4% |
| LOAD_CONST | 140 | 0.1% |
| LOAD_FAST_CHECK | 140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 249,714 | 95.5% |
| LOAD_GLOBAL_MODULE | 11,440 | 4.4% |
| NOP | 280 | 0.1% |
| RETURN_CONST | 140 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,636,827 | 99.5% |
| LOAD_ATTR_INSTANCE_VALUE | 3,711 | 0.2% |
| LOAD_GLOBAL_MODULE | 2,280 | 0.1% |
| LOAD_CONST | 1,240 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,153,664 | 70.1% |
| STORE_FAST | 487,434 | 29.6% |
| LIST_APPEND | 2,000 | 0.1% |
| TO_BOOL_NONE | 1,240 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 37,480 | 86.5% |
| BUILD_TUPLE | 5,680 | 13.1% |
| CALL | 180 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 31,860 | 73.5% |
| LOAD_FAST | 11,480 | 26.5% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,388,423 | 93.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 97,751 | 6.6% |
| LOAD_ATTR | 2,480 | 0.2% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 639,981 | 43.0% |
| STORE_FAST | 575,960 | 38.7% |
| LOAD_FAST | 85,060 | 5.7% |
| CALL_BUILTIN_FAST | 81,248 | 5.5% |
| RETURN_VALUE | 51,646 | 3.5% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 889,090 | 91.8% |
| LOAD_CONST | 33,720 | 3.5% |
| CALL | 29,140 | 3.0% |
| RETURN_VALUE | 14,000 | 1.4% |
| RETURN_GENERATOR | 1,300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 918,370 | 94.8% |
| LOAD_CONST | 33,440 | 3.5% |
| RETURN_VALUE | 14,900 | 1.5% |
| BINARY_OP_ADD_UNICODE | 1,240 | 0.1% |
| STORE_FAST | 280 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 5,535,635 | 45.0% |
| LOAD_FAST | 5,107,639 | 41.6% |
| LOAD_FAST_LOAD_FAST | 823,186 | 6.7% |
| LOAD_SUPER_ATTR_METHOD | 483,383 | 3.9% |
| LOAD_GLOBAL_MODULE | 93,900 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,242,210 | 99.6% |
| MAKE_CELL | 27,800 | 0.2% |
| RETURN_GENERATOR | 18,420 | 0.1% |
| COPY_FREE_VARS | 360 | 0.0% |
| PUSH_EXC_INFO | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 1,214,873 | 41.9% |
| LOAD_ATTR_MODULE | 1,153,304 | 39.8% |
| LOAD_FAST | 332,714 | 11.5% |
| LOAD_CONST | 107,086 | 3.7% |
| BINARY_OP | 83,760 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,744,473 | 60.2% |
| COPY_FREE_VARS | 1,153,384 | 39.8% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,860 | 99.7% |
| CALL | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,220 | 85.9% |
| YIELD_VALUE | 1,260 | 10.6% |
| STORE_FAST | 280 | 2.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 140 | 1.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 581,740 | 99.8% |
| LOAD_FAST | 1,240 | 0.2% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 581,720 | 99.8% |
| LOAD_FAST | 1,260 | 0.2% |
| CALL | 140 | 0.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 86.1% |
| LOAD_GLOBAL_MODULE | 140 | 9.7% |
| CALL | 60 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 1,260 | 87.5% |
| PUSH_NULL | 140 | 9.7% |
| LOAD_GLOBAL | 40 | 2.8% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 140 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,020,907 | 54.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,068,417 | 28.8% |
| LOAD_FAST | 576,980 | 15.6% |
| LOAD_FAST_LOAD_FAST | 18,480 | 0.5% |
| CALL_BUILTIN_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,706,042 | 99.9% |
| POP_JUMP_IF_TRUE | 3,417 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 92 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,412,846 | 95.5% |
| LOAD_CONST | 59,860 | 4.0% |
| LOAD_FAST | 5,820 | 0.4% |
| COMPARE_OP | 440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,439,986 | 97.4% |
| COPY | 14,040 | 0.9% |
| LOAD_FAST | 14,040 | 0.9% |
| POP_JUMP_IF_TRUE | 10,900 | 0.7% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 6,335,920 | 99.8% |
| GET_ITER | 11,440 | 0.2% |
| FOR_ITER | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,335,920 | 99.8% |
| POP_TOP | 11,440 | 0.2% |
| RESUME | 80 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 7,894,424 | 79.5% |
| GET_ITER | 1,551,446 | 15.6% |
| SWAP | 482,740 | 4.9% |
| FOR_ITER | 300 | 0.0% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 5,760,060 | 58.0% |
| STORE_FAST | 1,634,816 | 16.5% |
| LOAD_FAST | 966,926 | 9.7% |
| JUMP_BACKWARD | 576,000 | 5.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 499,908 | 5.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 493,614 | 65.6% |
| GET_ITER | 258,569 | 34.4% |
| FOR_ITER | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 508,277 | 67.6% |
| LOAD_FAST | 233,226 | 31.0% |
| RETURN_CONST | 10,880 | 1.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 16,320 | 54.0% |
| GET_ITER | 11,740 | 38.8% |
| LOAD_FAST | 1,260 | 4.2% |
| SWAP | 860 | 2.8% |
| FOR_ITER | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 14,260 | 47.2% |
| LOAD_FAST | 10,460 | 34.6% |
| RETURN_CONST | 2,560 | 8.5% |
| STORE_FAST_LOAD_FAST | 2,000 | 6.6% |
| SWAP | 860 | 2.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 81,208 | 88.8% |
| LOAD_ATTR_MODULE | 10,200 | 11.1% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,945 | 81.9% |
| LOAD_FAST_CHECK | 16,543 | 18.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,945,316 | 90.5% |
| LOAD_FAST_LOAD_FAST | 1,689,036 | 7.0% |
| COPY | 575,880 | 2.4% |
| LOAD_ATTR_INSTANCE_VALUE | 23,717 | 0.1% |
| RETURN_VALUE | 14,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,549,804 | 22.9% |
| LOAD_FAST | 3,671,301 | 15.1% |
| TO_BOOL_BOOL | 1,849,830 | 7.6% |
| LOAD_ATTR | 1,799,686 | 7.4% |
| CONTAINS_OP | 1,729,284 | 7.1% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 408,792 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,616 | 39.8% |
| CALL | 148,605 | 36.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 97,751 | 23.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,549,804 | 87.1% |
| LOAD_FAST | 624,819 | 9.8% |
| LOAD_ATTR | 85,280 | 1.3% |
| LOAD_ATTR_SLOT | 83,760 | 1.3% |
| LOAD_CONST | 15,520 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,484,192 | 39.0% |
| CALL | 1,439,877 | 22.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,388,423 | 21.8% |
| LOAD_CONST | 739,066 | 11.6% |
| LOAD_FAST_LOAD_FAST | 291,705 | 4.6% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,880,276 | 71.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,327,915 | 12.1% |
| LOAD_FAST_LOAD_FAST | 1,153,304 | 10.5% |
| BINARY_SUBSCR | 575,920 | 5.2% |
| LOAD_GLOBAL_MODULE | 28,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 5,535,635 | 50.4% |
| LOAD_FAST | 3,327,791 | 30.3% |
| CALL_PY_WITH_DEFAULTS | 1,214,873 | 11.1% |
| LOAD_FAST_LOAD_FAST | 678,560 | 6.2% |
| LOAD_CONST | 125,566 | 1.1% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,564,439 | 99.9% |
| LOAD_ATTR | 2,820 | 0.1% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,258,745 | 63.3% |
| CALL_PY_WITH_DEFAULTS | 1,153,304 | 32.3% |
| STORE_DEREF | 55,040 | 1.5% |
| LOAD_CONST | 35,840 | 1.0% |
| LOAD_FAST | 28,800 | 0.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,193,904 | 70.5% |
| LOAD_FAST_LOAD_FAST | 499,348 | 29.5% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,153,344 | 68.1% |
| UNARY_INVERT | 499,428 | 29.5% |
| RETURN_VALUE | 14,040 | 0.8% |
| LOAD_CONST | 14,040 | 0.8% |
| LOAD_FAST_LOAD_FAST | 5,720 | 0.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 984,863 | 97.1% |
| RETURN_VALUE | 27,440 | 2.7% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.1% |
| LOAD_ATTR | 320 | 0.0% |
| LOAD_ATTR_PROPERTY | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,001,703 | 98.8% |
| TO_BOOL_BOOL | 12,160 | 1.2% |
| LOAD_ATTR_PROPERTY | 220 | 0.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 98,360 | 98.6% |
| LOAD_ATTR_MODULE | 1,180 | 1.2% |
| RETURN_VALUE | 140 | 0.1% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 83,760 | 84.0% |
| CALL_BUILTIN_FAST | 14,140 | 14.2% |
| LOAD_FAST | 1,040 | 1.0% |
| LOAD_CONST | 600 | 0.6% |
| STORE_FAST | 140 | 0.1% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,588,031 | 41.8% |
| LOAD_FAST | 1,197,484 | 13.9% |
| STORE_FAST | 1,173,891 | 13.7% |
| LOAD_GLOBAL_BUILTIN | 977,932 | 11.4% |
| NOP | 713,150 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,965,293 | 46.1% |
| LOAD_DEREF | 1,746,367 | 20.3% |
| CALL_ISINSTANCE | 1,170,844 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 977,932 | 11.4% |
| LOAD_GLOBAL_MODULE | 625,080 | 7.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,764,473 | 28.4% |
| RESUME_CHECK | 3,058,217 | 18.2% |
| NOP | 1,760,155 | 10.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,441,863 | 8.6% |
| POP_JUMP_IF_FALSE | 1,430,143 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,709,746 | 22.1% |
| LOAD_ATTR_MODULE | 3,564,439 | 21.3% |
| LOAD_FAST_LOAD_FAST | 2,605,314 | 15.5% |
| LOAD_FAST | 2,107,344 | 12.6% |
| COMPARE_OP_STR | 1,412,846 | 8.4% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,440 | 99.9% |
| LOAD_SUPER_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 89,520 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,656,647 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,167,664 | 70.5% |
| CALL_PY_EXACT_ARGS | 483,383 | 29.2% |
| LOAD_FAST | 5,760 | 0.3% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 12,242,210 | 33.2% |
| CACHE | 11,732,222 | 31.8% |
| FOR_ITER_GEN | 6,335,920 | 17.2% |
| COPY_FREE_VARS | 1,752,507 | 4.8% |
| CALL_PY_WITH_DEFAULTS | 1,744,473 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,639,448 | 56.0% |
| POP_TOP | 6,913,520 | 18.8% |
| LOAD_GLOBAL_BUILTIN | 3,588,031 | 9.7% |
| LOAD_GLOBAL_MODULE | 3,058,217 | 8.3% |
| NOP | 1,355,084 | 3.7% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,018,372 | 68.9% |
| LOAD_FAST_LOAD_FAST | 745,163 | 17.0% |
| SWAP | 575,880 | 13.1% |
| LOAD_ATTR_INSTANCE_VALUE | 17,040 | 0.4% |
| STORE_FAST_LOAD_FAST | 14,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,147,252 | 49.0% |
| LOAD_FAST | 940,600 | 21.5% |
| LOAD_GLOBAL_MODULE | 722,003 | 16.5% |
| LOAD_CONST | 302,860 | 6.9% |
| LOAD_FAST_LOAD_FAST | 129,480 | 3.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,760 | 85.5% |
| LOAD_FAST_LOAD_FAST | 14,140 | 14.4% |
| STORE_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 97,980 | 100.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 1,153,304 | 92.6% |
| LOAD_FAST | 45,311 | 3.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,680 | 2.8% |
| CALL | 10,200 | 0.8% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,157,075 | 92.9% |
| RETURN_CONST | 32,520 | 2.6% |
| LOAD_GLOBAL_MODULE | 27,720 | 2.2% |
| LOAD_CONST | 27,480 | 2.2% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 62.7% |
| COPY | 317 | 33.1% |
| TO_BOOL | 40 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 620 | 64.8% |
| POP_JUMP_IF_FALSE | 337 | 35.2% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,849,830 | 26.7% |
| CALL_ISINSTANCE | 1,171,124 | 16.9% |
| RETURN_VALUE | 863,707 | 12.5% |
| CALL | 729,399 | 10.5% |
| LOAD_FAST | 719,579 | 10.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,823,085 | 69.6% |
| POP_JUMP_IF_TRUE | 1,852,681 | 26.8% |
| UNARY_NOT | 249,609 | 3.6% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,805,956 | 54.9% |
| BINARY_OP | 1,153,444 | 22.6% |
| LOAD_FAST | 1,153,304 | 22.6% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,113,084 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 494,883 | 92.0% |
| LOAD_ATTR_INSTANCE_VALUE | 42,900 | 8.0% |
| TO_BOOL | 200 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 537,843 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 191,389 | 79.6% |
| LOAD_FAST | 27,900 | 11.6% |
| COPY | 13,880 | 5.8% |
| WITH_EXCEPT_START | 5,680 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220,749 | 91.8% |
| POP_JUMP_IF_TRUE | 19,700 | 8.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 2,000 | 71.4% |
| LOAD_FAST | 620 | 22.1% |
| COPY | 160 | 5.7% |
| LOAD_GLOBAL_MODULE | 20 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,600 | 92.9% |
| POP_JUMP_IF_TRUE | 200 | 7.1% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,087,880 | 93.0% |
| CALL_BUILTIN_FAST | 81,248 | 6.9% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,088,220 | 93.0% |
| STORE_FAST | 81,288 | 7.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 581,600 | 27.4% |
| LOAD_FAST_CHECK | 575,920 | 27.1% |
| FOR_ITER_LIST | 499,908 | 23.5% |
| CALL_BUILTIN_FAST | 449,301 | 21.2% |
| CALL | 9,440 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,116,749 | 99.7% |
| LOAD_FAST | 7,000 | 0.3% |
| STORE_DEREF | 60 | 0.0% |


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
|     deferred | 6,918,669 | 76.9% |
|          hit | 2,070,941 | 23.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 600 | 8.5% |
| Failure | 6,421 | 91.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,195 | 49.8% |
| or | 1,707 | 26.6% |
| remainder | 779 | 12.1% |
| add different types | 640 | 10.0% |
| add other | 100 | 1.6% |


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
|     deferred | 636,059 | 46.0% |
|          hit | 744,452 | 53.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 21.4% |
| Failure | 880 | 78.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 880 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,855,905 | 27.6% |
|          hit | 28,376,601 | 72.3% |
|         miss | 7,840 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,280 | 23.5% |
| Failure | 30,202 | 76.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,910 | 26.2% |
| cfunc noargs | 6,326 | 20.9% |
| class no vectorcall | 4,000 | 13.2% |
| meth descr varargs keywords | 3,219 | 10.7% |
| class mutable | 1,282 | 4.2% |
| other | 1,180 | 3.9% |
| bound method | 1,123 | 3.7% |
| cfunc varargs | 1,100 | 3.6% |
| cfunc varargs keywords | 922 | 3.1% |
| meth descr method fastcall keywords | 920 | 3.0% |
| operator wrapper | 780 | 2.6% |
| cmethod | 640 | 2.1% |
| wrong number arguments | 480 | 1.6% |
| method wrapper | 280 | 0.9% |
| meth descr varargs | 40 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 577,211 | 10.0% |
|          hit | 5,182,564 | 89.9% |
|         miss | 6,393 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,610 | 54.4% |
| Failure | 1,347 | 45.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 806 | 59.8% |
| big int | 360 | 26.7% |
| different types | 181 | 13.4% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,302,940 | 7.1% |
|          hit | 17,059,013 | 92.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 26.7% |
| Failure | 1,700 | 73.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 520 | 30.6% |
| enumerate | 520 | 30.6% |
| itertools | 400 | 23.5% |
| callable | 260 | 15.3% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,475,530 | 17.8% |
|          hit | 48,184,215 | 82.1% |
|         miss | 311,126 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,460 | 52.3% |
| Failure | 20,504 | 47.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,621 | 22.5% |
| shadowed | 4,278 | 20.9% |
| not managed dict | 3,732 | 18.2% |
| non overriding descriptor | 2,432 | 11.9% |
| has managed dict | 1,120 | 5.5% |
| class attr descriptor | 1,040 | 5.1% |
| metaclass attribute | 960 | 4.7% |
| class method obj | 920 | 4.5% |
| non object slot | 560 | 2.7% |
| class attr simple | 481 | 2.3% |
| mutable class | 280 | 1.4% |
| overridden | 80 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 14,380 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 25,351,942 | 99.9% |
|         miss | 6,172 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,636 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,746,367 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 100.0% |
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

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 334,620 | 7.3% |
|          hit | 4,232,075 | 92.4% |
|         miss | 245,260 | 5.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,980 | 78.1% |
| Failure | 2,520 | 21.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| property | 1,180 | 46.8% |
| class attr simple | 560 | 22.2% |
| not in keys | 520 | 20.6% |
| no dict | 260 | 10.3% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 30,340 | 2.4% |
|          hit | 1,244,995 | 97.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 28.3% |
| Failure | 660 | 71.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 440 | 66.7% |
| other | 220 | 33.3% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,576,099 | 10.9% |
|          hit | 12,820,528 | 89.0% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,000 | 45.0% |
| Failure | 3,663 | 55.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,083 | 29.6% |
| sequence | 880 | 24.0% |
| set | 740 | 20.2% |
| tuple | 740 | 20.2% |
| other | 220 | 6.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 3,293,317 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 440 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 318,464,853 | 56.2% |
| Not specialized | 60,118,349 | 10.6% |
| Specialized hits | 187,013,954 | 33.0% |
| Specialized misses | 577,074 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 10,855,905 | 33.2% |
| LOAD_ATTR | 10,475,530 | 32.0% |
| BINARY_OP | 6,918,669 | 21.1% |
| TO_BOOL | 1,576,099 | 4.8% |
| FOR_ITER | 1,302,940 | 4.0% |
| BINARY_SUBSCR | 636,059 | 1.9% |
| COMPARE_OP | 577,211 | 1.8% |
| STORE_ATTR | 334,620 | 1.0% |
| STORE_SUBSCR | 30,340 | 0.1% |
| LOAD_GLOBAL | 14,380 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.5% |
| LOAD_ATTR_INSTANCE_VALUE | 215,686 | 37.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 81,960 | 14.2% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,380 | 1.1% |
| COMPARE_OP_INT | 6,373 | 1.1% |
| LOAD_GLOBAL_MODULE | 5,832 | 1.0% |
| LOAD_ATTR_MODULE | 1,100 | 0.2% |
| CALL_PY_EXACT_ARGS | 860 | 0.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 420 | 0.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 11,851,882 | 32.1% |
| Calls to Python functions inlined | 25,015,890 | 67.9% |
| Calls via PyEval_EvalFrame (total) | 11,851,882 | 32.1% |
| Calls via PyEval_EvalFrame (vector) | 11,266,762 | 30.6% |
| Calls via PyEval_EvalFrame (generator) | 585,120 | 1.6% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 11,266,062 | 30.6% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 625,920 | 1.7% |
| Calls via PyEval_EvalFrame (function ex) | 535,340 | 1.5% |
| Calls via PyEval_EvalFrame (api) | 621,886 | 1.7% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 49,437 | 0.1% |
| Frames pushed | 18,393,747 | 49.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 19,040,820 | 41.7% |
| Frees to freelist | 19,053,521 |  |
| Allocations | 26,674,240 | 58.3% |
| Allocations to 512 bytes | 26,388,644 | 57.7% |
| Allocations to 4 kbytes | 117,590 | 0.3% |
| Allocations over 4 kbytes | 168,006 | 0.4% |
| Frees | 28,128,219 |  |
| New values | 88,020 |  |
| Interpreter increfs | 221,768,516 | 76.8% |
| Interpreter decrefs | 243,131,459 | 73.7% |
| Increfs | 66,839,270 | 23.2% |
| Decrefs | 86,586,487 | 26.3% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 11,972,391 |  |
| Method cache misses | 110,692 |  |
| Method cache collisions | 249,082 |  |
| Method cache dunder hits | 11,254,675 |  |
| Method cache dunder misses | 142,012 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 600 | 283,968 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


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
| Number of data files | 40 |


</details>

---
Stats gathered on: 2024-01-04
