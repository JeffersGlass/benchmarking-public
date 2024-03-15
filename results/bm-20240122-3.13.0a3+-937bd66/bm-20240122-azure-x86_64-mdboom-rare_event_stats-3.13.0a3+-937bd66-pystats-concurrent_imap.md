
# Pystats results

- benchmark: concurrent_imap
- fork: mdboom
- ref: rare-event-stats
- commit hash: 937bd66
- commit date: 2024-01-22T10:00:20-05:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 99,050,599 | 17.6% | 17.6% |  |
| RESUME_CHECK | 36,642,582 | 6.5% | 24.1% | 0.0% |
| STORE_FAST | 29,150,577 | 5.2% | 29.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 24,124,000 | 4.3% | 33.6% | 0.9% |
| POP_TOP | 23,799,998 | 4.2% | 37.8% |  |
| RETURN_VALUE | 21,640,731 | 3.8% | 41.7% |  |
| POP_JUMP_IF_FALSE | 18,819,670 | 3.3% | 45.0% |  |
| JUMP_BACKWARD | 17,877,002 | 3.2% | 48.2% |  |
| LOAD_GLOBAL_MODULE | 16,611,489 | 3.0% | 51.1% | 0.0% |
| LOAD_FAST_LOAD_FAST | 15,340,490 | 2.7% | 53.9% |  |
| LOAD_CONST | 15,316,223 | 2.7% | 56.6% |  |
| CALL_PY_EXACT_ARGS | 12,170,553 | 2.2% | 58.7% | 0.0% |
| INTERPRETER_EXIT | 11,814,519 | 2.1% | 60.8% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 10,894,011 | 1.9% | 62.8% | 0.8% |
| CALL | 10,837,602 | 1.9% | 64.7% |  |
| LOAD_ATTR | 10,115,732 | 1.8% | 66.5% |  |
| FOR_ITER_LIST | 9,886,085 | 1.8% | 68.3% |  |
| NOP | 9,821,535 | 1.7% | 70.0% |  |
| RETURN_CONST | 9,112,073 | 1.6% | 71.6% |  |
| LOAD_GLOBAL_BUILTIN | 8,518,907 | 1.5% | 73.1% | 0.0% |
| PUSH_NULL | 7,328,801 | 1.3% | 74.4% |  |
| COPY | 7,154,403 | 1.3% | 75.7% |  |
| YIELD_VALUE | 6,913,660 | 1.2% | 76.9% |  |
| TO_BOOL_BOOL | 6,877,926 | 1.2% | 78.2% |  |
| BINARY_OP | 6,842,347 | 1.2% | 79.4% |  |
| STORE_FAST_LOAD_FAST | 6,464,820 | 1.1% | 80.5% |  |
| FOR_ITER_GEN | 6,347,440 | 1.1% | 81.7% |  |
| LOAD_ATTR_METHOD_NO_DICT | 6,342,041 | 1.1% | 82.8% |  |
| TO_BOOL_INT | 5,049,976 | 0.9% | 83.7% |  |
| POP_JUMP_IF_NOT_NONE | 4,977,271 | 0.9% | 84.6% |  |
| STORE_FAST_STORE_FAST | 4,799,591 | 0.9% | 85.4% |  |
| STORE_ATTR_INSTANCE_VALUE | 4,350,852 | 0.8% | 86.2% | 5.6% |
| BUILD_TUPLE | 4,247,876 | 0.8% | 86.9% |  |
| COMPARE_OP_INT | 3,688,553 | 0.7% | 87.6% | 0.2% |
| LOAD_ATTR_MODULE | 3,541,789 | 0.6% | 88.2% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 2,875,923 | 0.5% | 88.7% |  |
| POP_JUMP_IF_TRUE | 2,719,202 | 0.5% | 89.2% |  |
| SWAP | 2,558,180 | 0.5% | 89.7% |  |
| CALL_FUNCTION_EX | 2,413,974 | 0.4% | 90.1% |  |
| GET_ITER | 2,330,510 | 0.4% | 90.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,112,311 | 0.4% | 90.9% |  |
| CALL_BUILTIN_CLASS | 1,967,984 | 0.3% | 91.2% |  |
| BEFORE_WITH | 1,838,316 | 0.3% | 91.6% |  |
| CALL_BUILTIN_FAST | 1,793,701 | 0.3% | 91.9% |  |
| LOAD_DEREF | 1,783,145 | 0.3% | 92.2% |  |
| COPY_FREE_VARS | 1,733,085 | 0.3% | 92.5% |  |
| CONTAINS_OP | 1,716,182 | 0.3% | 92.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,673,450 | 0.3% | 93.1% |  |
| JUMP_FORWARD | 1,668,378 | 0.3% | 93.4% |  |
| BUILD_MAP | 1,658,383 | 0.3% | 93.7% |  |
| LOAD_SUPER_ATTR_METHOD | 1,636,765 | 0.3% | 94.0% |  |
| UNARY_INVERT | 1,632,790 | 0.3% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,623,532 | 0.3% | 94.6% | 0.0% |
| TO_BOOL | 1,580,185 | 0.3% | 94.9% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,482,047 | 0.3% | 95.1% |  |
| COMPARE_OP_STR | 1,476,117 | 0.3% | 95.4% |  |
| BUILD_LIST | 1,472,145 | 0.3% | 95.7% |  |
| FOR_ITER | 1,305,260 | 0.2% | 95.9% |  |
| STORE_SUBSCR_DICT | 1,229,589 | 0.2% | 96.1% |  |
| UNPACK_SEQUENCE_TUPLE | 1,169,489 | 0.2% | 96.3% |  |
| CALL_ISINSTANCE | 1,156,922 | 0.2% | 96.5% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,138,349 | 0.2% | 96.7% | 0.0% |
| BINARY_OP_ADD_INT | 1,112,440 | 0.2% | 96.9% |  |
| POP_JUMP_IF_NONE | 1,107,993 | 0.2% | 97.1% |  |
| EXIT_INIT_CHECK | 1,023,746 | 0.2% | 97.3% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,023,746 | 0.2% | 97.5% |  |
| LOAD_ATTR_PROPERTY | 1,002,626 | 0.2% | 97.7% | 1.2% |
| CALL_METHOD_DESCRIPTOR_O | 967,555 | 0.2% | 97.8% | 0.0% |
| LOAD_FAST_CHECK | 824,283 | 0.1% | 98.0% |  |
| LIST_APPEND | 802,360 | 0.1% | 98.1% |  |
| FOR_ITER_RANGE | 743,850 | 0.1% | 98.2% |  |
| LOAD_FAST_AND_CLEAR | 738,953 | 0.1% | 98.4% |  |
| BINARY_SUBSCR | 636,709 | 0.1% | 98.5% |  |
| CALL_LEN | 620,577 | 0.1% | 98.6% |  |
| CALL_TUPLE_1 | 583,120 | 0.1% | 98.7% |  |
| COMPARE_OP | 568,187 | 0.1% | 98.8% |  |
| DICT_MERGE | 564,260 | 0.1% | 98.9% |  |
| TO_BOOL_LIST | 532,303 | 0.1% | 99.0% |  |
| BINARY_SUBSCR_LIST_INT | 472,130 | 0.1% | 99.1% |  |
| LIST_EXTEND | 462,010 | 0.1% | 99.2% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 408,896 | 0.1% | 99.2% |  |
| CALL_KW | 347,076 | 0.1% | 99.3% |  |
| BINARY_OP_SUBTRACT_INT | 329,927 | 0.1% | 99.4% |  |
| CALL_LIST_APPEND | 258,754 | 0.0% | 99.4% |  |
| BINARY_OP_ADD_FLOAT | 247,498 | 0.0% | 99.4% |  |
| UNARY_NOT | 246,799 | 0.0% | 99.5% |  |
| TO_BOOL_NONE | 240,468 | 0.0% | 99.5% | 0.1% |
| BINARY_OP_SUBTRACT_FLOAT | 230,949 | 0.0% | 99.6% |  |
| CALL_BUILTIN_O | 154,260 | 0.0% | 99.6% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 142,315 | 0.0% | 99.6% | 4.5% |
| MAKE_CELL | 137,900 | 0.0% | 99.7% |  |
| STORE_DEREF | 137,660 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_DICT | 114,880 | 0.0% | 99.7% |  |
| BINARY_OP_MULTIPLY_FLOAT | 112,600 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_STR_INT | 112,600 | 0.0% | 99.7% |  |
| STORE_ATTR | 100,863 | 0.0% | 99.8% |  |
| LOAD_ATTR_SLOT | 99,760 | 0.0% | 99.8% |  |
| STORE_ATTR_SLOT | 97,980 | 0.0% | 99.8% |  |
| LOAD_ATTR_CLASS | 91,469 | 0.0% | 99.8% |  |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 0.0% | 99.8% |  |
| DELETE_ATTR | 86,397 | 0.0% | 99.8% |  |
| DELETE_SUBSCR | 78,218 | 0.0% | 99.9% |  |
| MAKE_FUNCTION | 63,680 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 55,680 | 0.0% | 99.9% |  |
| POP_EXCEPT | 48,849 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 48,849 | 0.0% | 99.9% |  |
| IS_OP | 47,010 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 43,340 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 43,089 | 0.0% | 99.9% |  |
| BUILD_STRING | 41,600 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,160 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 39,040 | 0.0% | 99.9% |  |
| IMPORT_NAME | 33,760 | 0.0% | 99.9% |  |
| IMPORT_FROM | 33,420 | 0.0% | 99.9% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 32,108 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 31,260 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 30,220 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 28,160 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 27,480 | 0.0% | 100.0% |  |
| BINARY_SLICE | 19,820 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 18,900 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,844 | 0.0% | 100.0% |  |
| RERAISE | 17,281 | 0.0% | 100.0% |  |
| CALL_STR_1 | 11,900 | 0.0% | 100.0% |  |
| END_FOR | 11,520 | 0.0% | 100.0% |  |
| STORE_NAME | 7,480 | 0.0% | 100.0% |  |
| RESUME | 5,980 | 0.0% | 100.0% | 0.0% |
| RAISE_VARARGS | 5,780 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 5,760 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 3,840 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 2,800 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,200 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 1,440 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 970 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 21,830,998 | 3.9% | 3.9% |
| RESUME_CHECK LOAD_FAST | 20,530,864 | 3.6% | 7.5% |
| STORE_FAST LOAD_FAST | 12,630,808 | 2.2% | 9.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 12,123,953 | 2.2% | 11.9% |
| CACHE RESUME_CHECK | 11,700,640 | 2.1% | 14.0% |
| LOAD_FAST RETURN_VALUE | 10,555,115 | 1.9% | 15.9% |
| RETURN_VALUE INTERPRETER_EXIT | 10,363,779 | 1.8% | 17.7% |
| POP_TOP JUMP_BACKWARD | 8,671,365 | 1.5% | 19.3% |
| JUMP_BACKWARD FOR_ITER_LIST | 7,868,640 | 1.4% | 20.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 7,808,290 | 1.4% | 22.1% |
| LOAD_FAST LOAD_ATTR | 7,787,948 | 1.4% | 23.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 7,737,009 | 1.4% | 24.8% |
| POP_TOP LOAD_FAST | 7,321,806 | 1.3% | 26.1% |
| RESUME_CHECK POP_TOP | 6,913,520 | 1.2% | 27.3% |
| RETURN_CONST POP_TOP | 6,429,466 | 1.1% | 28.5% |
| JUMP_BACKWARD FOR_ITER_GEN | 6,335,920 | 1.1% | 29.6% |
| YIELD_VALUE STORE_FAST | 6,335,920 | 1.1% | 30.7% |
| FOR_ITER_GEN RESUME_CHECK | 6,335,920 | 1.1% | 31.9% |
| NOP LOAD_FAST | 6,252,287 | 1.1% | 33.0% |
| FOR_ITER_LIST STORE_FAST_LOAD_FAST | 5,760,060 | 1.0% | 34.0% |
| STORE_FAST JUMP_BACKWARD | 5,760,000 | 1.0% | 35.0% |
| STORE_FAST_LOAD_FAST YIELD_VALUE | 5,760,000 | 1.0% | 36.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 5,521,668 | 1.0% | 37.0% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 5,487,091 | 1.0% | 38.0% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 5,049,836 | 0.9% | 38.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,046,457 | 0.9% | 39.8% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 4,783,603 | 0.9% | 40.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 4,706,958 | 0.8% | 41.5% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,930,903 | 0.7% | 42.2% |
| LOAD_FAST LOAD_CONST | 3,877,359 | 0.7% | 42.9% |
| LOAD_CONST LOAD_CONST | 3,787,503 | 0.7% | 43.5% |
| STORE_FAST NOP | 3,758,750 | 0.7% | 44.2% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,684,729 | 0.7% | 44.9% |
| LOAD_FAST PUSH_NULL | 3,670,465 | 0.7% | 45.5% |
| LOAD_GLOBAL_MODULE BINARY_OP | 3,663,740 | 0.7% | 46.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,649,644 | 0.6% | 46.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,553,567 | 0.6% | 47.4% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,541,748 | 0.6% | 48.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 3,538,550 | 0.6% | 48.7% |
| PUSH_NULL LOAD_FAST | 3,456,118 | 0.6% | 49.3% |
| LOAD_ATTR LOAD_FAST | 3,379,342 | 0.6% | 49.9% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 3,289,526 | 0.6% | 50.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 3,088,569 | 0.5% | 51.1% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 3,029,578 | 0.5% | 51.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 2,995,569 | 0.5% | 52.1% |
| BINARY_OP COPY | 2,771,792 | 0.5% | 52.6% |
| COPY TO_BOOL_INT | 2,771,472 | 0.5% | 53.1% |
| COPY STORE_FAST | 2,630,400 | 0.5% | 53.6% |
| STORE_FAST COPY | 2,629,760 | 0.5% | 54.0% |
| CALL STORE_FAST | 2,599,446 | 0.5% | 54.5% |
| LOAD_CONST CALL | 2,587,839 | 0.5% | 55.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,573,709 | 0.5% | 55.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 2,462,149 | 0.4% | 55.9% |
| CALL RETURN_VALUE | 2,441,962 | 0.4% | 56.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,401,689 | 0.4% | 56.7% |
| LOAD_ATTR_MODULE PUSH_NULL | 2,247,240 | 0.4% | 57.1% |
| CALL POP_TOP | 2,233,883 | 0.4% | 57.5% |
| RETURN_VALUE STORE_FAST | 2,227,245 | 0.4% | 57.9% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,124,452 | 0.4% | 58.3% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 2,105,251 | 0.4% | 58.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,084,403 | 0.4% | 59.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,023,092 | 0.4% | 59.4% |
| PUSH_NULL CALL | 2,018,172 | 0.4% | 59.8% |
| LOAD_CONST COMPARE_OP_INT | 2,005,928 | 0.4% | 60.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 2,003,487 | 0.4% | 60.5% |
| RETURN_VALUE RETURN_VALUE | 1,912,585 | 0.3% | 60.8% |
| POP_TOP RETURN_CONST | 1,903,749 | 0.3% | 61.1% |
| LOAD_FAST_LOAD_FAST CALL | 1,878,954 | 0.3% | 61.5% |
| LOAD_FAST CALL_FUNCTION_EX | 1,849,694 | 0.3% | 61.8% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,847,564 | 0.3% | 62.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,829,934 | 0.3% | 62.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,793,978 | 0.3% | 62.8% |
| NOP LOAD_GLOBAL_MODULE | 1,739,992 | 0.3% | 63.1% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 1,736,921 | 0.3% | 63.4% |
| POP_TOP LOAD_CONST | 1,734,172 | 0.3% | 63.7% |
| COPY_FREE_VARS RESUME_CHECK | 1,732,425 | 0.3% | 64.0% |
| LOAD_DEREF LOAD_FAST | 1,726,805 | 0.3% | 64.3% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,726,285 | 0.3% | 64.6% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 1,715,562 | 0.3% | 64.9% |
| LOAD_ATTR_INSTANCE_VALUE CONTAINS_OP | 1,714,902 | 0.3% | 65.2% |
| LOAD_FAST BUILD_TUPLE | 1,705,882 | 0.3% | 65.5% |
| LOAD_CONST LOAD_FAST | 1,670,061 | 0.3% | 65.8% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,667,852 | 0.3% | 66.1% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 1,636,565 | 0.3% | 66.4% |
| UNARY_INVERT BINARY_OP | 1,632,790 | 0.3% | 66.7% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 1,616,745 | 0.3% | 67.0% |
| FOR_ITER_LIST STORE_FAST | 1,614,752 | 0.3% | 67.3% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,582,068 | 0.3% | 67.6% |
| GET_ITER FOR_ITER_LIST | 1,540,046 | 0.3% | 67.8% |
| POP_TOP NOP | 1,537,381 | 0.3% | 68.1% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,530,102 | 0.3% | 68.4% |
| LOAD_FAST TO_BOOL | 1,518,658 | 0.3% | 68.7% |
| LOAD_FAST GET_ITER | 1,464,325 | 0.3% | 68.9% |
| RETURN_VALUE POP_TOP | 1,451,285 | 0.3% | 69.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,439,028 | 0.3% | 69.4% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,438,467 | 0.3% | 69.7% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,437,145 | 0.3% | 69.9% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,434,703 | 0.3% | 70.2% |
| POP_JUMP_IF_FALSE POP_TOP | 1,429,355 | 0.3% | 70.5% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,415,767 | 0.3% | 70.7% |


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
| RESUME_CHECK | 11,700,640 | 99.0% |
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
| LOAD_ATTR_INSTANCE_VALUE | 1,253,734 | 68.2% |
| RETURN_VALUE | 478,003 | 26.0% |
| LOAD_GLOBAL_MODULE | 82,439 | 4.5% |
| LOAD_FAST | 17,280 | 0.9% |
| CALL | 6,360 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,354,653 | 73.7% |
| STORE_FAST | 483,663 | 26.3% |


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
| LOAD_FAST_LOAD_FAST | 576,080 | 90.5% |
| LOAD_CONST | 59,669 | 9.4% |
| BINARY_SUBSCR | 880 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 575,920 | 90.5% |
| STORE_FAST | 59,389 | 9.3% |
| BINARY_SUBSCR | 880 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 37,928 | 88.0% |
| LOAD_ATTR_MODULE | 5,100 | 11.8% |
| LOAD_GLOBAL | 41 | 0.1% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 43,089 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,899 | 48.5% |
| CALL | 27,519 | 35.2% |
| LOAD_ATTR_INSTANCE_VALUE | 12,718 | 16.3% |
| LOAD_ATTR | 82 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60,799 | 77.7% |
| RETURN_CONST | 10,239 | 13.1% |
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
| RETURN_CONST | 1,023,746 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,023,746 | 100.0% |


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
| LOAD_FAST | 1,464,325 | 62.8% |
| STORE_FAST_LOAD_FAST | 576,000 | 24.7% |
| CALL_BUILTIN_CLASS | 262,645 | 11.3% |
| CALL | 14,340 | 0.6% |
| RETURN_VALUE | 5,760 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,540,046 | 66.1% |
| LOAD_FAST_AND_CLEAR | 492,059 | 21.1% |
| FOR_ITER_RANGE | 255,728 | 11.0% |
| FOR_ITER | 12,117 | 0.5% |
| FOR_ITER_TUPLE | 11,740 | 0.5% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,363,779 | 87.7% |
| RETURN_CONST | 873,000 | 7.4% |
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
| STORE_FAST | 3,758,750 | 38.3% |
| POP_TOP | 1,537,381 | 15.7% |
| RESUME_CHECK | 1,340,702 | 13.7% |
| POP_JUMP_IF_FALSE | 1,312,215 | 13.4% |
| JUMP_BACKWARD | 1,088,000 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,252,287 | 63.7% |
| LOAD_GLOBAL_MODULE | 1,739,992 | 17.7% |
| LOAD_GLOBAL_BUILTIN | 704,556 | 7.2% |
| LOAD_FAST_LOAD_FAST | 583,320 | 5.9% |
| LOAD_CONST | 529,460 | 5.4% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 31,828 | 65.2% |
| COPY | 11,521 | 23.6% |
| POP_TOP | 5,200 | 10.6% |
| STORE_FAST | 280 | 0.6% |
| STORE_SUBSCR_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 32,108 | 65.7% |
| RERAISE | 11,521 | 23.6% |
| JUMP_FORWARD | 5,120 | 10.5% |
| RETURN_CONST | 60 | 0.1% |
| JUMP_BACKWARD | 20 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,913,520 | 29.0% |
| RETURN_CONST | 6,429,466 | 27.0% |
| CALL | 2,233,883 | 9.4% |
| RETURN_VALUE | 1,451,285 | 6.1% |
| POP_JUMP_IF_FALSE | 1,429,355 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 8,671,365 | 36.4% |
| LOAD_FAST | 7,321,806 | 30.8% |
| RETURN_CONST | 1,903,749 | 8.0% |
| LOAD_CONST | 1,734,172 | 7.3% |
| NOP | 1,537,381 | 6.5% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 37,549 | 76.9% |
| RERAISE | 5,760 | 11.8% |
| CALL_KW | 5,120 | 10.5% |
| BINARY_SUBSCR_DICT | 300 | 0.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 37,888 | 77.6% |
| WITH_EXCEPT_START | 5,760 | 11.8% |
| LOAD_GLOBAL_MODULE | 5,080 | 10.4% |
| LOAD_GLOBAL | 121 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,670,465 | 50.1% |
| LOAD_ATTR_MODULE | 2,247,240 | 30.7% |
| LOAD_ATTR | 1,284,376 | 17.5% |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,456,118 | 47.2% |
| CALL | 2,018,172 | 27.5% |
| LOAD_FAST_LOAD_FAST | 1,396,238 | 19.1% |
| LOAD_CONST | 320,997 | 4.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 64,656 | 0.9% |


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
| LOAD_FAST | 10,555,115 | 48.8% |
| CALL | 2,441,962 | 11.3% |
| RETURN_VALUE | 1,912,585 | 8.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,530,102 | 7.1% |
| CALL_FUNCTION_EX | 1,265,514 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 10,363,779 | 47.9% |
| STORE_FAST | 2,227,245 | 10.3% |
| RETURN_VALUE | 1,912,585 | 8.8% |
| POP_TOP | 1,451,285 | 6.7% |
| LOAD_FAST_LOAD_FAST | 1,139,002 | 5.3% |


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
| LOAD_FAST | 1,518,658 | 96.1% |
| LOAD_ATTR_INSTANCE_VALUE | 53,498 | 3.4% |
| TO_BOOL | 3,663 | 0.2% |
| LOAD_ATTR | 882 | 0.1% |
| RETURN_VALUE | 764 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 835,596 | 52.9% |
| POP_JUMP_IF_FALSE | 737,885 | 46.7% |
| TO_BOOL | 3,663 | 0.2% |
| TO_BOOL_BOOL | 2,161 | 0.1% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,139,002 | 69.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 493,708 | 30.2% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,632,790 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 246,759 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 246,799 | 100.0% |


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
| LOAD_GLOBAL_MODULE | 3,663,740 | 53.5% |
| UNARY_INVERT | 1,632,790 | 23.9% |
| POP_JUMP_IF_FALSE | 1,139,002 | 16.6% |
| LOAD_ATTR | 260,994 | 3.8% |
| LOAD_FAST_LOAD_FAST | 84,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,771,792 | 40.5% |
| STORE_FAST | 1,400,316 | 20.5% |
| TO_BOOL_INT | 1,139,062 | 16.6% |
| UNARY_INVERT | 1,139,002 | 16.6% |
| BUILD_TUPLE | 246,894 | 3.6% |


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
| SWAP | 492,059 | 33.4% |
| JUMP_FORWARD | 477,763 | 32.5% |
| LOAD_FAST | 247,558 | 16.8% |
| POP_TOP | 230,225 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 495,003 | 33.6% |
| SWAP | 492,059 | 33.4% |
| STORE_FAST | 479,223 | 32.6% |
| RETURN_VALUE | 5,120 | 0.3% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 576,000 | 34.7% |
| LOAD_FAST | 529,560 | 31.9% |
| RESUME_CHECK | 487,963 | 29.4% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 2.1% |
| POP_JUMP_IF_NOT_NONE | 17,280 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,065,083 | 64.2% |
| BUILD_TUPLE | 576,020 | 34.7% |
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
| LOAD_FAST | 1,705,882 | 40.2% |
| LOAD_FAST_LOAD_FAST | 1,160,320 | 27.3% |
| BUILD_MAP | 576,020 | 13.6% |
| RETURN_VALUE | 512,000 | 12.1% |
| BINARY_OP | 246,894 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 1,152,100 | 27.1% |
| CALL | 1,140,562 | 26.9% |
| BUILD_MAP | 576,000 | 13.6% |
| STORE_FAST | 512,000 | 12.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 12.1% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,587,839 | 23.9% |
| PUSH_NULL | 2,018,172 | 18.6% |
| LOAD_FAST_LOAD_FAST | 1,878,954 | 17.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,438,467 | 13.3% |
| BUILD_TUPLE | 1,140,562 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,599,446 | 24.0% |
| RETURN_VALUE | 2,441,962 | 22.5% |
| POP_TOP | 2,233,883 | 20.6% |
| LOAD_FAST | 1,046,401 | 9.7% |
| TO_BOOL_BOOL | 730,056 | 6.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,694 | 76.6% |
| DICT_MERGE | 564,260 | 23.4% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,265,514 | 52.4% |
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
| LOAD_CONST | 347,076 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 277,505 | 80.0% |
| LOAD_FAST | 28,800 | 8.3% |
| RETURN_VALUE | 21,120 | 6.1% |
| STORE_FAST | 14,220 | 4.1% |
| PUSH_EXC_INFO | 5,120 | 1.5% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 564,299 | 99.3% |
| COMPARE_OP | 1,264 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 690 | 0.1% |
| LOAD_GLOBAL_MODULE | 379 | 0.1% |
| LOAD_FAST | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 564,950 | 99.4% |
| COMPARE_OP | 1,264 | 0.2% |
| COMPARE_OP_INT | 1,174 | 0.2% |
| COMPARE_OP_STR | 439 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,714,902 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,715,562 | 100.0% |
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
| BINARY_OP | 2,771,792 | 38.7% |
| STORE_FAST | 2,629,760 | 36.8% |
| LOAD_CONST | 1,100,800 | 15.4% |
| LOAD_FAST | 590,100 | 8.2% |
| STORE_ATTR_INSTANCE_VALUE | 21,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 2,771,472 | 38.7% |
| STORE_FAST | 2,630,400 | 36.8% |
| STORE_FAST_STORE_FAST | 1,093,760 | 15.3% |
| LOAD_ATTR_INSTANCE_VALUE | 575,880 | 8.0% |
| LOAD_FAST | 28,160 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 1,139,002 | 65.7% |
| CALL_ALLOC_AND_ENTER_INIT | 477,723 | 27.6% |
| CACHE | 109,900 | 6.3% |
| CALL | 5,940 | 0.3% |
| CALL_PY_EXACT_ARGS | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,732,425 | 100.0% |
| RETURN_GENERATOR | 340 | 0.0% |
| RESUME | 320 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,397 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,598 | 66.7% |
| RETURN_CONST | 27,519 | 31.9% |
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
| RETURN_VALUE | 27,520 | 58.5% |
| LOAD_FAST | 17,420 | 37.1% |
| LOAD_GLOBAL_MODULE | 2,030 | 4.3% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,870 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,671,365 | 48.5% |
| STORE_FAST | 5,760,000 | 32.2% |
| POP_JUMP_IF_NOT_NONE | 973,510 | 5.4% |
| LIST_APPEND | 802,360 | 4.5% |
| STORE_FAST_STORE_FAST | 581,760 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 7,868,640 | 44.0% |
| FOR_ITER_GEN | 6,335,920 | 35.4% |
| FOR_ITER | 1,271,223 | 7.1% |
| NOP | 1,088,000 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 575,960 | 3.2% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 32,108 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 31,828 | 99.1% |
| LOAD_FAST | 280 | 0.9% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,028,746 | 61.7% |
| POP_TOP | 621,412 | 37.2% |
| STORE_ATTR_INSTANCE_VALUE | 7,020 | 0.4% |
| BINARY_SUBSCR_TUPLE_INT | 5,720 | 0.3% |
| POP_EXCEPT | 5,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,115,328 | 66.9% |
| BUILD_LIST | 477,763 | 28.6% |
| POP_EXCEPT | 31,828 | 1.9% |
| LOAD_GLOBAL_MODULE | 24,819 | 1.5% |
| LOAD_FAST_LOAD_FAST | 7,320 | 0.4% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 440,806 | 54.9% |
| LOAD_ATTR | 246,914 | 30.8% |
| BINARY_SUBSCR_STR_INT | 112,600 | 14.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,000 | 0.2% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 802,360 | 100.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 231,645 | 50.1% |
| RETURN_VALUE | 230,225 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 230,865 | 50.0% |
| STORE_FAST | 230,225 | 49.8% |
| RETURN_VALUE | 640 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.0% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,787,948 | 77.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,793,978 | 17.7% |
| LOAD_GLOBAL_MODULE | 387,144 | 3.8% |
| CALL | 83,860 | 0.8% |
| LOAD_ATTR | 22,740 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,379,342 | 33.4% |
| PUSH_NULL | 1,284,376 | 12.7% |
| STORE_SUBSCR_DICT | 1,138,922 | 11.3% |
| POP_JUMP_IF_NOT_NONE | 1,111,103 | 11.0% |
| STORE_FAST | 722,101 | 7.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,877,359 | 25.3% |
| LOAD_CONST | 3,787,503 | 24.7% |
| POP_TOP | 1,734,172 | 11.3% |
| POP_JUMP_IF_FALSE | 909,588 | 5.9% |
| LOAD_ATTR_METHOD_NO_DICT | 739,635 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,787,503 | 24.7% |
| CALL | 2,587,839 | 16.9% |
| COMPARE_OP_INT | 2,005,928 | 13.1% |
| LOAD_FAST | 1,670,061 | 10.9% |
| COPY | 1,100,800 | 7.2% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,726,285 | 96.8% |
| POP_JUMP_IF_NOT_NONE | 27,520 | 1.5% |
| STORE_DEREF | 27,520 | 1.5% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,726,805 | 96.8% |
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
| RESUME_CHECK | 20,530,864 | 20.7% |
| STORE_FAST | 12,630,808 | 12.8% |
| POP_JUMP_IF_FALSE | 7,737,009 | 7.8% |
| POP_TOP | 7,321,806 | 7.4% |
| NOP | 6,252,287 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 21,830,998 | 22.0% |
| RETURN_VALUE | 10,555,115 | 10.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,808,290 | 7.9% |
| LOAD_ATTR | 7,787,948 | 7.9% |
| CALL_PY_EXACT_ARGS | 5,046,457 | 5.1% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 492,059 | 66.6% |
| LOAD_FAST_AND_CLEAR | 246,894 | 33.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 492,059 | 66.6% |
| LOAD_FAST_AND_CLEAR | 246,894 | 33.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 576,560 | 69.9% |
| POP_JUMP_IF_NONE | 230,869 | 28.0% |
| LOAD_ATTR_CLASS | 16,534 | 2.0% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 69.9% |
| LOAD_GLOBAL_MODULE | 230,789 | 28.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,494 | 2.0% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,573,709 | 16.8% |
| LOAD_FAST_LOAD_FAST | 2,003,487 | 13.1% |
| POP_JUMP_IF_FALSE | 1,434,703 | 9.4% |
| PUSH_NULL | 1,396,238 | 9.1% |
| LOAD_SUPER_ATTR_METHOD | 1,153,282 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,541,748 | 23.1% |
| LOAD_FAST_LOAD_FAST | 2,003,487 | 13.1% |
| CALL | 1,878,954 | 12.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,667,852 | 10.9% |
| BUILD_TUPLE | 1,160,320 | 7.6% |


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
| LOAD_GLOBAL_MODULE | 6,818 | 38.2% |
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
| TO_BOOL_INT | 5,049,836 | 26.8% |
| TO_BOOL_BOOL | 4,783,603 | 25.4% |
| COMPARE_OP_INT | 3,684,729 | 19.6% |
| CONTAINS_OP | 1,715,562 | 9.1% |
| COMPARE_OP_STR | 1,437,145 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,737,009 | 41.1% |
| RETURN_CONST | 3,088,569 | 16.4% |
| LOAD_FAST_LOAD_FAST | 1,434,703 | 7.6% |
| POP_TOP | 1,429,355 | 7.6% |
| LOAD_GLOBAL_MODULE | 1,415,767 | 7.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,030,193 | 93.0% |
| LOAD_ATTR_INSTANCE_VALUE | 47,800 | 4.3% |
| LOAD_ATTR | 28,300 | 2.6% |
| RETURN_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 284,288 | 25.7% |
| LOAD_FAST | 274,738 | 24.8% |
| NOP | 268,145 | 24.2% |
| LOAD_FAST_CHECK | 230,869 | 20.8% |
| RETURN_CONST | 24,340 | 2.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,401,689 | 48.3% |
| LOAD_ATTR | 1,111,103 | 22.3% |
| LOAD_ATTR_INSTANCE_VALUE | 946,709 | 19.0% |
| RETURN_VALUE | 441,446 | 8.9% |
| LOAD_DEREF | 55,040 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,023,092 | 40.6% |
| RETURN_CONST | 1,112,545 | 22.4% |
| JUMP_BACKWARD | 973,510 | 19.6% |
| NOP | 486,562 | 9.8% |
| LOAD_CONST | 230,505 | 4.6% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,847,564 | 67.9% |
| TO_BOOL | 835,596 | 30.7% |
| TO_BOOL_NONE | 19,700 | 0.7% |
| COMPARE_OP_STR | 10,892 | 0.4% |
| COMPARE_OP_INT | 3,430 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 955,999 | 35.2% |
| LOAD_FAST_LOAD_FAST | 838,394 | 30.8% |
| RETURN_CONST | 739,260 | 27.2% |
| LOAD_GLOBAL_MODULE | 71,607 | 2.6% |
| RETURN_VALUE | 59,349 | 2.2% |


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
| POP_EXCEPT | 11,521 | 66.7% |
| POP_JUMP_IF_TRUE | 5,760 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 5,761 | 50.0% |
| PUSH_EXC_INFO | 5,760 | 50.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,088,569 | 33.9% |
| STORE_ATTR_INSTANCE_VALUE | 2,124,452 | 23.3% |
| POP_TOP | 1,903,749 | 20.9% |
| POP_JUMP_IF_NOT_NONE | 1,112,545 | 12.2% |
| POP_JUMP_IF_TRUE | 739,260 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,429,466 | 70.6% |
| EXIT_INIT_CHECK | 1,023,746 | 11.2% |
| INTERPRETER_EXIT | 873,000 | 9.6% |
| TO_BOOL_BOOL | 687,408 | 7.5% |
| STORE_FAST | 61,189 | 0.7% |


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
| LOAD_FAST | 58,563 | 58.1% |
| LOAD_FAST_LOAD_FAST | 22,040 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 17,280 | 17.1% |
| STORE_ATTR | 2,520 | 2.5% |
| LOAD_ATTR | 240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 44,840 | 44.5% |
| LOAD_FAST_LOAD_FAST | 14,760 | 14.6% |
| LOAD_FAST | 13,620 | 13.5% |
| LOAD_CONST | 12,642 | 12.5% |
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
| YIELD_VALUE | 6,335,920 | 21.7% |
| COPY | 2,630,400 | 9.0% |
| CALL | 2,599,446 | 8.9% |
| RETURN_VALUE | 2,227,245 | 7.6% |
| FOR_ITER_LIST | 1,614,752 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,630,808 | 43.3% |
| JUMP_BACKWARD | 5,760,000 | 19.8% |
| NOP | 3,758,750 | 12.9% |
| COPY | 2,629,760 | 9.0% |
| LOAD_GLOBAL_BUILTIN | 1,162,471 | 4.0% |


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
| UNPACK_SEQUENCE_TWO_TUPLE | 2,105,251 | 43.9% |
| COPY | 1,093,760 | 22.8% |
| UNPACK_SEQUENCE_TUPLE | 1,088,220 | 22.7% |
| STORE_FAST_STORE_FAST | 512,000 | 10.7% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,582,068 | 33.0% |
| STORE_FAST | 1,088,280 | 22.7% |
| LOAD_FAST_LOAD_FAST | 1,019,563 | 21.2% |
| JUMP_BACKWARD | 581,760 | 12.1% |
| STORE_FAST_STORE_FAST | 512,000 | 10.7% |


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
| BINARY_OP_ADD_INT | 575,940 | 22.5% |
| BUILD_LIST | 492,059 | 19.2% |
| LOAD_FAST_AND_CLEAR | 492,059 | 19.2% |
| FOR_ITER_LIST | 477,119 | 18.7% |
| LOAD_FAST | 258,669 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 575,880 | 22.5% |
| LOAD_CONST | 505,563 | 19.8% |
| BUILD_LIST | 492,059 | 19.2% |
| STORE_FAST | 492,059 | 19.2% |
| FOR_ITER_LIST | 477,039 | 18.6% |


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
| LOAD_FAST | 247,458 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 247,498 | 100.0% |


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
| CALL | 230,789 | 99.9% |
| BINARY_OP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 230,949 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 264,778 | 80.3% |
| LOAD_CONST | 59,269 | 18.0% |
| CALL_LEN | 5,680 | 1.7% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 324,207 | 98.3% |
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
| LOAD_FAST_LOAD_FAST | 460,370 | 97.5% |
| LOAD_CONST | 11,640 | 2.5% |
| BINARY_SUBSCR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 460,410 | 97.5% |
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
| LOAD_GLOBAL_MODULE | 505,163 | 49.3% |
| LOAD_FAST | 484,883 | 47.4% |
| CALL | 33,420 | 3.3% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 546,023 | 53.3% |
| COPY_FREE_VARS | 477,723 | 46.7% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 64,656 | 45.4% |
| LOAD_FAST | 64,240 | 45.1% |
| LOAD_CONST | 7,480 | 5.3% |
| BINARY_OP_ADD_INT | 5,680 | 4.0% |
| CALL | 159 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 135,935 | 95.5% |
| POP_TOP | 6,280 | 4.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 698,096 | 35.5% |
| CALL_FUNCTION_EX | 511,960 | 26.0% |
| LOAD_FAST | 265,238 | 13.5% |
| CALL_BUILTIN_CLASS | 230,145 | 11.7% |
| CALL_LEN | 230,145 | 11.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 759,478 | 38.6% |
| STORE_FAST | 698,396 | 35.5% |
| GET_ITER | 262,645 | 13.3% |
| CALL_BUILTIN_CLASS | 230,145 | 11.7% |
| LOAD_FAST | 17,280 | 0.9% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 864,084 | 48.2% |
| LOAD_CONST | 618,330 | 34.5% |
| LOAD_FAST_LOAD_FAST | 173,138 | 9.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,229 | 4.5% |
| LOAD_GLOBAL_MODULE | 27,880 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 608,270 | 33.9% |
| STORE_FAST | 584,012 | 32.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 443,523 | 24.7% |
| UNPACK_SEQUENCE_TUPLE | 81,229 | 4.5% |
| POP_TOP | 14,887 | 0.8% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 519,280 | 45.6% |
| BUILD_TUPLE | 511,960 | 45.0% |
| CALL | 64,955 | 5.7% |
| LOAD_FAST_CHECK | 16,494 | 1.4% |
| LOAD_ATTR | 14,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,053,900 | 92.6% |
| RETURN_VALUE | 82,129 | 7.2% |
| LOAD_FAST | 1,260 | 0.1% |
| STORE_FAST | 860 | 0.1% |
| BEFORE_WITH | 140 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 112,560 | 73.0% |
| LOAD_ATTR | 27,440 | 17.8% |
| LOAD_FAST | 14,140 | 9.2% |
| CALL | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 112,560 | 73.0% |
| LOAD_FAST | 41,520 | 26.9% |
| TO_BOOL_INT | 140 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,156,462 | 100.0% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,156,742 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 592,297 | 95.4% |
| LOAD_ATTR_INSTANCE_VALUE | 27,900 | 4.5% |
| CALL | 380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 344,218 | 55.5% |
| CALL_BUILTIN_CLASS | 230,145 | 37.1% |
| CALL_PY_EXACT_ARGS | 33,160 | 5.3% |
| LOAD_FAST | 5,720 | 0.9% |
| BINARY_OP_SUBTRACT_INT | 5,680 | 0.9% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 246,814 | 95.4% |
| LOAD_FAST | 11,440 | 4.4% |
| LOAD_CONST | 140 | 0.1% |
| LOAD_FAST_CHECK | 140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 246,854 | 95.4% |
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
| LOAD_FAST | 1,616,745 | 99.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,687 | 0.2% |
| LOAD_GLOBAL_MODULE | 2,280 | 0.1% |
| LOAD_CONST | 1,240 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,139,282 | 70.2% |
| STORE_FAST | 480,710 | 29.6% |
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
| LOAD_ATTR_METHOD_NO_DICT | 1,381,304 | 93.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 97,723 | 6.6% |
| LOAD_ATTR | 2,480 | 0.2% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 633,341 | 42.7% |
| STORE_FAST | 575,960 | 38.9% |
| LOAD_FAST | 85,060 | 5.7% |
| CALL_BUILTIN_FAST | 81,229 | 5.5% |
| RETURN_VALUE | 51,628 | 3.5% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 888,115 | 91.8% |
| LOAD_CONST | 33,720 | 3.5% |
| CALL | 29,140 | 3.0% |
| RETURN_VALUE | 14,000 | 1.4% |
| RETURN_GENERATOR | 1,300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 917,395 | 94.8% |
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
| LOAD_ATTR_METHOD_WITH_VALUES | 5,487,091 | 45.1% |
| LOAD_FAST | 5,046,457 | 41.5% |
| LOAD_FAST_LOAD_FAST | 820,345 | 6.7% |
| LOAD_SUPER_ATTR_METHOD | 477,683 | 3.9% |
| LOAD_GLOBAL_MODULE | 93,900 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,123,953 | 99.6% |
| MAKE_CELL | 27,800 | 0.2% |
| RETURN_GENERATOR | 18,420 | 0.2% |
| COPY_FREE_VARS | 360 | 0.0% |
| PUSH_EXC_INFO | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 1,210,093 | 42.1% |
| LOAD_ATTR_MODULE | 1,138,922 | 39.6% |
| LOAD_FAST | 329,854 | 11.5% |
| LOAD_CONST | 107,173 | 3.7% |
| BINARY_OP | 83,760 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,736,921 | 60.4% |
| COPY_FREE_VARS | 1,139,002 | 39.6% |


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
| LOAD_CONST | 2,005,928 | 54.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,062,081 | 28.8% |
| LOAD_FAST | 576,980 | 15.6% |
| LOAD_FAST_LOAD_FAST | 18,480 | 0.5% |
| CALL_BUILTIN_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,684,729 | 99.9% |
| POP_JUMP_IF_TRUE | 3,430 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 94 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,409,998 | 95.5% |
| LOAD_CONST | 59,860 | 4.1% |
| LOAD_FAST | 5,820 | 0.4% |
| COMPARE_OP | 439 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,437,145 | 97.4% |
| COPY | 14,040 | 1.0% |
| LOAD_FAST | 14,040 | 1.0% |
| POP_JUMP_IF_TRUE | 10,892 | 0.7% |


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
| JUMP_BACKWARD | 7,868,640 | 79.6% |
| GET_ITER | 1,540,046 | 15.6% |
| SWAP | 477,039 | 4.8% |
| FOR_ITER | 300 | 0.0% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 5,760,060 | 58.3% |
| STORE_FAST | 1,614,752 | 16.3% |
| LOAD_FAST | 955,526 | 9.7% |
| JUMP_BACKWARD | 576,000 | 5.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 494,188 | 5.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 487,922 | 65.6% |
| GET_ITER | 255,728 | 34.4% |
| FOR_ITER | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 502,585 | 67.6% |
| LOAD_FAST | 230,385 | 31.0% |
| RETURN_CONST | 10,880 | 1.5% |


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
| LOAD_GLOBAL_MODULE | 81,189 | 88.8% |
| LOAD_ATTR_MODULE | 10,200 | 11.2% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,935 | 81.9% |
| LOAD_FAST_CHECK | 16,534 | 18.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,830,998 | 90.5% |
| LOAD_FAST_LOAD_FAST | 1,667,852 | 6.9% |
| COPY | 575,880 | 2.4% |
| LOAD_ATTR_INSTANCE_VALUE | 23,730 | 0.1% |
| RETURN_VALUE | 14,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,521,668 | 22.9% |
| LOAD_FAST | 3,649,644 | 15.1% |
| TO_BOOL_BOOL | 1,829,934 | 7.6% |
| LOAD_ATTR | 1,793,978 | 7.4% |
| CONTAINS_OP | 1,714,902 | 7.1% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 408,716 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,578 | 39.8% |
| CALL | 148,595 | 36.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 97,723 | 23.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,521,668 | 87.1% |
| LOAD_FAST | 620,193 | 9.8% |
| LOAD_ATTR | 85,280 | 1.3% |
| LOAD_ATTR_SLOT | 83,760 | 1.3% |
| LOAD_CONST | 15,520 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,462,149 | 38.8% |
| CALL | 1,438,467 | 22.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,381,304 | 21.8% |
| LOAD_CONST | 739,635 | 11.7% |
| LOAD_FAST_LOAD_FAST | 288,946 | 4.6% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,808,290 | 71.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,322,778 | 12.1% |
| LOAD_FAST_LOAD_FAST | 1,138,922 | 10.5% |
| BINARY_SUBSCR | 575,920 | 5.3% |
| LOAD_GLOBAL_MODULE | 28,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 5,487,091 | 50.4% |
| LOAD_FAST | 3,289,526 | 30.2% |
| CALL_PY_WITH_DEFAULTS | 1,210,093 | 11.1% |
| LOAD_FAST_LOAD_FAST | 678,560 | 6.2% |
| LOAD_CONST | 125,653 | 1.2% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,538,550 | 99.9% |
| LOAD_ATTR | 2,819 | 0.1% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,247,240 | 63.4% |
| CALL_PY_WITH_DEFAULTS | 1,138,922 | 32.2% |
| STORE_DEREF | 55,040 | 1.6% |
| LOAD_CONST | 35,840 | 1.0% |
| LOAD_FAST | 28,800 | 0.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,179,522 | 70.5% |
| LOAD_FAST_LOAD_FAST | 493,628 | 29.5% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,138,962 | 68.1% |
| UNARY_INVERT | 493,708 | 29.5% |
| RETURN_VALUE | 14,040 | 0.8% |
| LOAD_CONST | 14,040 | 0.8% |
| LOAD_FAST_LOAD_FAST | 5,720 | 0.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 973,406 | 97.1% |
| RETURN_VALUE | 27,440 | 2.7% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.1% |
| LOAD_ATTR | 320 | 0.0% |
| LOAD_ATTR_PROPERTY | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 990,246 | 98.8% |
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
| RESUME_CHECK | 3,553,567 | 41.7% |
| LOAD_FAST | 1,183,102 | 13.9% |
| STORE_FAST | 1,162,471 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 972,250 | 11.4% |
| NOP | 704,556 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,930,903 | 46.1% |
| LOAD_DEREF | 1,726,285 | 20.3% |
| CALL_ISINSTANCE | 1,156,462 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 972,250 | 11.4% |
| LOAD_GLOBAL_MODULE | 625,080 | 7.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,706,958 | 28.3% |
| RESUME_CHECK | 3,029,578 | 18.2% |
| NOP | 1,739,992 | 10.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,439,028 | 8.7% |
| POP_JUMP_IF_FALSE | 1,415,767 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,663,740 | 22.1% |
| LOAD_ATTR_MODULE | 3,538,550 | 21.3% |
| LOAD_FAST_LOAD_FAST | 2,573,709 | 15.5% |
| LOAD_FAST | 2,084,403 | 12.5% |
| COMPARE_OP_STR | 1,409,998 | 8.5% |


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
| LOAD_FAST | 1,636,565 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,153,282 | 70.5% |
| CALL_PY_EXACT_ARGS | 477,683 | 29.2% |
| LOAD_FAST | 5,760 | 0.4% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 12,123,953 | 33.1% |
| CACHE | 11,700,640 | 31.9% |
| FOR_ITER_GEN | 6,335,920 | 17.3% |
| CALL_PY_WITH_DEFAULTS | 1,736,921 | 4.7% |
| COPY_FREE_VARS | 1,732,425 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,530,864 | 56.0% |
| POP_TOP | 6,913,520 | 18.9% |
| LOAD_GLOBAL_BUILTIN | 3,553,567 | 9.7% |
| LOAD_GLOBAL_MODULE | 3,029,578 | 8.3% |
| NOP | 1,340,702 | 3.7% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,995,569 | 68.9% |
| LOAD_FAST_LOAD_FAST | 739,463 | 17.0% |
| SWAP | 575,880 | 13.2% |
| LOAD_ATTR_INSTANCE_VALUE | 17,040 | 0.4% |
| STORE_FAST_LOAD_FAST | 14,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,124,452 | 48.8% |
| LOAD_FAST | 940,600 | 21.6% |
| LOAD_GLOBAL_MODULE | 716,303 | 16.5% |
| LOAD_CONST | 302,858 | 7.0% |
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
| LOAD_ATTR | 1,138,922 | 92.6% |
| LOAD_FAST | 44,287 | 3.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,680 | 2.8% |
| CALL | 10,200 | 0.8% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,141,669 | 92.8% |
| RETURN_CONST | 32,520 | 2.6% |
| LOAD_GLOBAL_MODULE | 27,720 | 2.3% |
| LOAD_CONST | 27,480 | 2.2% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,829,934 | 26.6% |
| CALL_ISINSTANCE | 1,156,742 | 16.8% |
| RETURN_VALUE | 855,262 | 12.4% |
| CALL | 730,056 | 10.6% |
| LOAD_FAST | 719,109 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,783,603 | 69.6% |
| POP_JUMP_IF_TRUE | 1,847,564 | 26.9% |
| UNARY_NOT | 246,759 | 3.6% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,771,472 | 54.9% |
| BINARY_OP | 1,139,062 | 22.6% |
| LOAD_FAST | 1,138,922 | 22.6% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,049,836 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 489,183 | 91.9% |
| LOAD_ATTR_INSTANCE_VALUE | 42,900 | 8.1% |
| TO_BOOL | 200 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 532,143 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 191,408 | 79.6% |
| LOAD_FAST | 27,900 | 11.6% |
| COPY | 13,880 | 5.8% |
| WITH_EXCEPT_START | 5,680 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220,768 | 91.8% |
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
| CALL_BUILTIN_FAST | 81,229 | 6.9% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,088,220 | 93.1% |
| STORE_FAST | 81,269 | 6.9% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 581,600 | 27.5% |
| LOAD_FAST_CHECK | 575,920 | 27.3% |
| FOR_ITER_LIST | 494,188 | 23.4% |
| CALL_BUILTIN_FAST | 443,523 | 21.0% |
| CALL | 9,440 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,105,251 | 99.7% |
| LOAD_FAST | 7,000 | 0.3% |
| STORE_DEREF | 60 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 61.9% |
| COPY | 330 | 34.0% |
| TO_BOOL | 40 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 620 | 63.9% |
| POP_JUMP_IF_FALSE | 350 | 36.1% |


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
|     deferred | 6,835,335 | 76.7% |
|          hit | 2,064,734 | 23.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 600 | 8.6% |
| Failure | 6,412 | 91.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,189 | 49.7% |
| or | 1,703 | 26.6% |
| remainder | 780 | 12.2% |
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
|     deferred | 635,589 | 46.2% |
|          hit | 738,770 | 53.7% |

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
|     deferred | 10,805,958 | 27.7% |
|          hit | 28,144,113 | 72.2% |
|         miss | 7,840 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,280 | 23.5% |
| Failure | 30,204 | 76.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,913 | 26.2% |
| cfunc noargs | 6,328 | 21.0% |
| class no vectorcall | 4,000 | 13.2% |
| meth descr varargs keywords | 3,220 | 10.7% |
| class mutable | 1,280 | 4.2% |
| other | 1,180 | 3.9% |
| bound method | 1,123 | 3.7% |
| cfunc varargs | 1,100 | 3.6% |
| cfunc varargs keywords | 920 | 3.0% |
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
|     deferred | 571,814 | 10.0% |
|          hit | 5,158,212 | 90.0% |
|         miss | 6,598 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,613 | 54.3% |
| Failure | 1,358 | 45.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 808 | 59.5% |
| big int | 360 | 26.5% |
| different types | 190 | 14.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,302,940 | 7.1% |
|          hit | 17,007,595 | 92.9% |

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
|     deferred | 10,384,114 | 17.8% |
|          hit | 47,866,705 | 82.1% |
|         miss | 311,337 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,460 | 52.3% |
| Failure | 20,495 | 47.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,620 | 22.5% |
| shadowed | 4,269 | 20.8% |
| not managed dict | 3,726 | 18.2% |
| non overriding descriptor | 2,440 | 11.9% |
| has managed dict | 1,120 | 5.5% |
| class attr descriptor | 1,040 | 5.1% |
| metaclass attribute | 960 | 4.7% |
| class method obj | 920 | 4.5% |
| non object slot | 560 | 2.7% |
| class attr simple | 480 | 2.3% |
| mutable class | 280 | 1.4% |
| overridden | 80 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,634 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 25,126,020 | 99.9% |
|         miss | 4,376 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,586 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,726,285 | 100.0% |

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
|     deferred | 334,623 | 7.4% |
|          hit | 4,203,572 | 92.4% |
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
|          hit | 1,229,589 | 97.5% |

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
|     deferred | 1,573,801 | 11.0% |
|          hit | 12,704,163 | 88.9% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,001 | 45.0% |
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
|          hit | 3,281,800 | 100.0% |

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
| Basic | 316,678,794 | 56.3% |
| Not specialized | 59,681,385 | 10.6% |
| Specialized hits | 185,758,204 | 33.0% |
| Specialized misses | 575,692 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 10,805,958 | 33.3% |
| LOAD_ATTR | 10,384,114 | 32.0% |
| BINARY_OP | 6,835,335 | 21.0% |
| TO_BOOL | 1,573,801 | 4.8% |
| FOR_ITER | 1,302,940 | 4.0% |
| BINARY_SUBSCR | 635,589 | 2.0% |
| COMPARE_OP | 571,814 | 1.8% |
| STORE_ATTR | 334,623 | 1.0% |
| STORE_SUBSCR | 30,340 | 0.1% |
| LOAD_GLOBAL | 12,634 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.6% |
| LOAD_ATTR_INSTANCE_VALUE | 215,832 | 37.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,025 | 14.2% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.2% |
| COMPARE_OP_INT | 6,578 | 1.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,380 | 1.1% |
| LOAD_GLOBAL_MODULE | 4,036 | 0.7% |
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
| Calls to PyEval_EvalDefault | 11,820,300 | 32.2% |
| Calls to Python functions inlined | 24,847,162 | 67.8% |
| Calls via PyEval_EvalFrame (total) | 11,820,300 | 32.2% |
| Calls via PyEval_EvalFrame (vector) | 11,235,180 | 30.6% |
| Calls via PyEval_EvalFrame (generator) | 585,120 | 1.6% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 11,234,480 | 30.6% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 625,920 | 1.7% |
| Calls via PyEval_EvalFrame (function ex) | 535,340 | 1.5% |
| Calls via PyEval_EvalFrame (api) | 616,104 | 1.7% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 48,968 | 0.1% |
| Frames pushed | 18,219,289 | 49.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 18,842,745 | 41.5% |
| Frees to freelist | 18,855,428 |  |
| Allocations | 26,563,300 | 58.5% |
| Allocations to 512 bytes | 26,277,722 | 57.9% |
| Allocations to 4 kbytes | 117,585 | 0.3% |
| Allocations over 4 kbytes | 167,993 | 0.4% |
| Frees | 28,003,299 |  |
| New values | 88,020 |  |
| Interpreter increfs | 220,399,326 | 76.9% |
| Interpreter decrefs | 241,614,858 | 73.7% |
| Increfs | 66,385,795 | 23.1% |
| Decrefs | 86,003,197 | 26.3% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 11,994,343 |  |
| Method cache misses | 61,612 |  |
| Method cache collisions | 109,642 |  |
| Method cache dunder hits | 11,293,330 |  |
| Method cache dunder misses | 51,741 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 39 | 585 | 275,588 |
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

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set_class | 0 |
| set_bases | 0 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 40 |


</details>

---
Stats gathered on: 2024-01-22
