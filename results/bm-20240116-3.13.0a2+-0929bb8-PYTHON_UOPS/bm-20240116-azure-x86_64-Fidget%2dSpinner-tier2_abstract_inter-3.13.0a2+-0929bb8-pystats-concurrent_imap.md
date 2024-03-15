
# Pystats results

- benchmark: concurrent_imap
- fork: Fidget-Spinner
- ref: tier2_abstract_interpreter
- commit hash: 0929bb8
- commit date: 2024-01-16T14:41:58+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 101,667,461 | 18.2% | 18.2% |  |
| RESUME_CHECK | 38,296,677 | 6.8% | 25.0% |  |
| STORE_FAST | 28,581,469 | 5.1% | 30.1% |  |
| LOAD_ATTR_INSTANCE_VALUE | 25,572,254 | 4.6% | 34.7% | 0.8% |
| POP_TOP | 24,914,579 | 4.5% | 39.1% |  |
| RETURN_VALUE | 23,372,720 | 4.2% | 43.3% |  |
| POP_JUMP_IF_FALSE | 20,337,951 | 3.6% | 47.0% |  |
| LOAD_GLOBAL_MODULE | 16,805,615 | 3.0% | 50.0% | 0.0% |
| LOAD_CONST | 15,471,696 | 2.8% | 52.7% |  |
| LOAD_FAST_LOAD_FAST | 13,559,058 | 2.4% | 55.1% |  |
| CALL_PY_EXACT_ARGS | 12,902,795 | 2.3% | 57.5% | 0.0% |
| INTERPRETER_EXIT | 12,188,705 | 2.2% | 59.6% |  |
| ENTER_EXECUTOR | 11,911,098 | 2.1% | 61.8% |  |
| CALL | 11,400,543 | 2.0% | 63.8% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 11,002,608 | 2.0% | 65.8% | 0.7% |
| LOAD_ATTR | 10,624,025 | 1.9% | 67.7% |  |
| RETURN_CONST | 9,755,871 | 1.7% | 69.4% |  |
| NOP | 9,504,705 | 1.7% | 71.1% |  |
| BINARY_OP | 7,829,136 | 1.4% | 72.5% |  |
| LOAD_GLOBAL_BUILTIN | 7,787,610 | 1.4% | 73.9% | 0.0% |
| COPY | 7,559,797 | 1.4% | 75.2% |  |
| TO_BOOL_BOOL | 7,117,727 | 1.3% | 76.5% |  |
| YIELD_VALUE | 6,913,660 | 1.2% | 77.8% |  |
| LOAD_ATTR_METHOD_NO_DICT | 6,643,615 | 1.2% | 78.9% |  |
| JUMP_BACKWARD | 6,351,150 | 1.1% | 80.1% |  |
| FOR_ITER_GEN | 6,347,440 | 1.1% | 81.2% |  |
| TO_BOOL_INT | 5,798,376 | 1.0% | 82.2% |  |
| PUSH_NULL | 5,623,240 | 1.0% | 83.3% |  |
| POP_JUMP_IF_NOT_NONE | 5,318,420 | 1.0% | 84.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 4,688,289 | 0.8% | 85.0% | 5.2% |
| STORE_FAST_STORE_FAST | 4,365,693 | 0.8% | 85.8% |  |
| COMPARE_OP_INT | 3,919,841 | 0.7% | 86.5% | 0.2% |
| FOR_ITER_LIST | 3,609,390 | 0.6% | 87.2% |  |
| BUILD_TUPLE | 3,307,271 | 0.6% | 87.8% |  |
| CALL_PY_WITH_DEFAULTS | 3,147,459 | 0.6% | 88.3% |  |
| SWAP | 2,827,564 | 0.5% | 88.8% |  |
| POP_JUMP_IF_TRUE | 2,750,668 | 0.5% | 89.3% |  |
| LOAD_ATTR_MODULE | 2,508,153 | 0.4% | 89.8% | 0.0% |
| CALL_FUNCTION_EX | 2,413,958 | 0.4% | 90.2% |  |
| LOAD_DEREF | 2,021,245 | 0.4% | 90.6% |  |
| COPY_FREE_VARS | 1,971,225 | 0.4% | 90.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,911,595 | 0.3% | 91.3% |  |
| BEFORE_WITH | 1,901,021 | 0.3% | 91.6% |  |
| CONTAINS_OP | 1,883,428 | 0.3% | 91.9% |  |
| LOAD_SUPER_ATTR_METHOD | 1,874,905 | 0.3% | 92.3% |  |
| UNARY_INVERT | 1,870,935 | 0.3% | 92.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,858,356 | 0.3% | 92.9% | 0.0% |
| JUMP_FORWARD | 1,797,816 | 0.3% | 93.3% |  |
| GET_ITER | 1,741,211 | 0.3% | 93.6% |  |
| CALL_BUILTIN_FAST | 1,699,964 | 0.3% | 93.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,678,373 | 0.3% | 94.2% |  |
| BUILD_LIST | 1,676,311 | 0.3% | 94.5% |  |
| CALL_BUILTIN_CLASS | 1,656,428 | 0.3% | 94.8% |  |
| TO_BOOL | 1,610,579 | 0.3% | 95.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,541,110 | 0.3% | 95.3% |  |
| COMPARE_OP_STR | 1,510,154 | 0.3% | 95.6% |  |
| STORE_SUBSCR_DICT | 1,400,337 | 0.3% | 95.8% |  |
| CALL_ISINSTANCE | 1,327,007 | 0.2% | 96.1% |  |
| POP_JUMP_IF_NONE | 1,210,071 | 0.2% | 96.3% |  |
| UNPACK_SEQUENCE_TUPLE | 1,169,493 | 0.2% | 96.5% |  |
| EXIT_INIT_CHECK | 1,159,856 | 0.2% | 96.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,159,856 | 0.2% | 96.9% |  |
| BUILD_MAP | 1,156,838 | 0.2% | 97.1% |  |
| LOAD_ATTR_PROPERTY | 1,138,702 | 0.2% | 97.3% | 1.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,132,133 | 0.2% | 97.5% | 0.0% |
| BINARY_OP_ADD_INT | 1,109,601 | 0.2% | 97.7% |  |
| CALL_METHOD_DESCRIPTOR_O | 958,749 | 0.2% | 97.9% | 0.0% |
| LIST_APPEND | 903,270 | 0.2% | 98.1% |  |
| LOAD_FAST_CHECK | 858,292 | 0.2% | 98.2% |  |
| LOAD_FAST_AND_CLEAR | 841,039 | 0.2% | 98.4% |  |
| COMPARE_OP | 637,282 | 0.1% | 98.5% |  |
| BINARY_SUBSCR | 633,718 | 0.1% | 98.6% |  |
| TO_BOOL_LIST | 600,358 | 0.1% | 98.7% |  |
| CALL_TUPLE_1 | 583,120 | 0.1% | 98.8% |  |
| DICT_MERGE | 564,260 | 0.1% | 98.9% |  |
| LIST_EXTEND | 530,062 | 0.1% | 99.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 408,912 | 0.1% | 99.1% |  |
| CALL_LEN | 396,751 | 0.1% | 99.1% |  |
| CALL_KW | 381,139 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 326,947 | 0.1% | 99.3% |  |
| FOR_ITER_RANGE | 308,766 | 0.1% | 99.3% |  |
| CALL_LIST_APPEND | 292,784 | 0.1% | 99.4% |  |
| BINARY_OP_ADD_FLOAT | 281,527 | 0.1% | 99.4% |  |
| UNARY_NOT | 280,809 | 0.1% | 99.5% |  |
| BINARY_OP_SUBTRACT_FLOAT | 264,974 | 0.0% | 99.5% |  |
| TO_BOOL_NONE | 240,474 | 0.0% | 99.6% | 0.1% |
| CALL_BUILTIN_O | 154,400 | 0.0% | 99.6% |  |
| MAKE_CELL | 137,900 | 0.0% | 99.6% |  |
| STORE_DEREF | 137,620 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_DICT | 114,880 | 0.0% | 99.7% |  |
| BINARY_OP_MULTIPLY_FLOAT | 112,600 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_STR_INT | 112,600 | 0.0% | 99.7% |  |
| STORE_ATTR | 100,863 | 0.0% | 99.7% |  |
| LOAD_ATTR_SLOT | 99,760 | 0.0% | 99.7% |  |
| STORE_ATTR_SLOT | 97,980 | 0.0% | 99.8% |  |
| LOAD_ATTR_CLASS | 91,473 | 0.0% | 99.8% |  |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 0.0% | 99.8% |  |
| DELETE_ATTR | 86,400 | 0.0% | 99.8% |  |
| DELETE_SUBSCR | 78,220 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 78,175 | 0.0% | 99.8% | 8.2% |
| MAKE_FUNCTION | 63,640 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 55,680 | 0.0% | 99.9% |  |
| IS_OP | 46,633 | 0.0% | 99.9% |  |
| POP_EXCEPT | 45,861 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 45,861 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 43,040 | 0.0% | 99.9% |  |
| BUILD_STRING | 41,600 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 40,101 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,160 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 39,000 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 38,380 | 0.0% | 99.9% |  |
| FOR_ITER | 36,380 | 0.0% | 99.9% |  |
| IMPORT_NAME | 33,760 | 0.0% | 99.9% |  |
| IMPORT_FROM | 33,420 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 31,260 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 29,121 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 28,160 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 27,920 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 27,480 | 0.0% | 100.0% |  |
| BINARY_SLICE | 19,820 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 18,900 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 18,400 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,854 | 0.0% | 100.0% |  |
| RERAISE | 17,280 | 0.0% | 100.0% |  |
| CALL_STR_1 | 11,900 | 0.0% | 100.0% |  |
| END_FOR | 11,520 | 0.0% | 100.0% |  |
| STORE_NAME | 7,480 | 0.0% | 100.0% |  |
| RESUME | 5,980 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 5,780 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 5,760 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 3,420 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,200 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,660 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 1,440 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 974 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 23,043,273 | 4.1% | 4.1% |
| RESUME_CHECK LOAD_FAST | 21,611,979 | 3.9% | 8.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 12,856,235 | 2.3% | 10.3% |
| STORE_FAST LOAD_FAST | 12,407,299 | 2.2% | 12.5% |
| CACHE RESUME_CHECK | 12,074,825 | 2.2% | 14.7% |
| LOAD_FAST RETURN_VALUE | 11,235,514 | 2.0% | 16.7% |
| RETURN_VALUE INTERPRETER_EXIT | 10,669,907 | 1.9% | 18.6% |
| LOAD_FAST LOAD_ATTR | 8,452,600 | 1.5% | 20.1% |
| POP_TOP ENTER_EXECUTOR | 8,247,782 | 1.5% | 21.6% |
| POP_JUMP_IF_FALSE LOAD_FAST | 8,117,330 | 1.5% | 23.0% |
| POP_TOP LOAD_FAST | 7,881,488 | 1.4% | 24.4% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 7,687,688 | 1.4% | 25.8% |
| RESUME_CHECK POP_TOP | 6,913,520 | 1.2% | 27.0% |
| RETURN_CONST POP_TOP | 6,875,670 | 1.2% | 28.3% |
| JUMP_BACKWARD FOR_ITER_GEN | 6,335,920 | 1.1% | 29.4% |
| YIELD_VALUE STORE_FAST | 6,335,920 | 1.1% | 30.5% |
| FOR_ITER_GEN RESUME_CHECK | 6,335,920 | 1.1% | 31.6% |
| ENTER_EXECUTOR YIELD_VALUE | 6,322,640 | 1.1% | 32.8% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 5,924,518 | 1.1% | 33.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 5,807,231 | 1.0% | 34.9% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 5,798,236 | 1.0% | 35.9% |
| STORE_FAST JUMP_BACKWARD | 5,760,000 | 1.0% | 36.9% |
| NOP LOAD_FAST | 5,595,567 | 1.0% | 37.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,497,038 | 1.0% | 38.9% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 4,991,977 | 0.9% | 39.8% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 4,618,411 | 0.8% | 40.6% |
| LOAD_GLOBAL_MODULE BINARY_OP | 4,208,025 | 0.8% | 41.4% |
| STORE_FAST NOP | 4,021,955 | 0.7% | 42.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,961,792 | 0.7% | 42.8% |
| LOAD_CONST LOAD_CONST | 3,923,620 | 0.7% | 43.5% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,915,995 | 0.7% | 44.2% |
| LOAD_FAST LOAD_CONST | 3,910,687 | 0.7% | 44.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,882,667 | 0.7% | 45.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,817,377 | 0.7% | 46.3% |
| LOAD_ATTR LOAD_FAST | 3,563,258 | 0.6% | 46.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,457,418 | 0.6% | 47.5% |
| PUSH_NULL LOAD_FAST | 3,453,672 | 0.6% | 48.2% |
| POP_JUMP_IF_FALSE RETURN_CONST | 3,322,050 | 0.6% | 48.8% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 3,267,789 | 0.6% | 49.3% |
| BINARY_OP COPY | 3,180,022 | 0.6% | 49.9% |
| COPY TO_BOOL_INT | 3,179,702 | 0.6% | 50.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 3,111,963 | 0.6% | 51.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,962,730 | 0.5% | 51.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,942,405 | 0.5% | 52.1% |
| CALL STORE_FAST | 2,766,554 | 0.5% | 52.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 2,689,259 | 0.5% | 53.1% |
| LOAD_CONST CALL | 2,652,230 | 0.5% | 53.5% |
| COPY STORE_FAST | 2,630,400 | 0.5% | 54.0% |
| STORE_FAST COPY | 2,629,760 | 0.5% | 54.5% |
| CALL RETURN_VALUE | 2,612,047 | 0.5% | 54.9% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,504,912 | 0.4% | 55.4% |
| RETURN_VALUE STORE_FAST | 2,499,410 | 0.4% | 55.8% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,466,758 | 0.4% | 56.3% |
| LOAD_FAST PUSH_NULL | 2,405,605 | 0.4% | 56.7% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,396,672 | 0.4% | 57.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,356,212 | 0.4% | 57.6% |
| CALL POP_TOP | 2,292,959 | 0.4% | 58.0% |
| RETURN_VALUE RETURN_VALUE | 2,184,727 | 0.4% | 58.4% |
| LOAD_CONST COMPARE_OP_INT | 2,173,042 | 0.4% | 58.8% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,122,103 | 0.4% | 59.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 2,003,618 | 0.4% | 59.5% |
| NOP LOAD_GLOBAL_MODULE | 1,977,817 | 0.4% | 59.8% |
| COPY_FREE_VARS RESUME_CHECK | 1,970,565 | 0.4% | 60.2% |
| POP_TOP RETURN_CONST | 1,965,943 | 0.4% | 60.5% |
| LOAD_DEREF LOAD_FAST | 1,964,945 | 0.4% | 60.9% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,964,425 | 0.4% | 61.2% |
| ENTER_EXECUTOR FOR_ITER_LIST | 1,952,209 | 0.3% | 61.6% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,906,662 | 0.3% | 61.9% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 1,882,808 | 0.3% | 62.3% |
| LOAD_ATTR_INSTANCE_VALUE CONTAINS_OP | 1,882,148 | 0.3% | 62.6% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 1,874,705 | 0.3% | 62.9% |
| UNARY_INVERT BINARY_OP | 1,870,935 | 0.3% | 63.3% |
| LOAD_FAST BUILD_TUPLE | 1,870,487 | 0.3% | 63.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,862,017 | 0.3% | 63.9% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 1,854,885 | 0.3% | 64.3% |
| LOAD_FAST CALL_FUNCTION_EX | 1,849,678 | 0.3% | 64.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,844,981 | 0.3% | 64.9% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 1,838,372 | 0.3% | 65.3% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,806,551 | 0.3% | 65.6% |
| POP_TOP LOAD_CONST | 1,799,239 | 0.3% | 65.9% |
| LOAD_CONST LOAD_FAST | 1,738,065 | 0.3% | 66.2% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,734,202 | 0.3% | 66.5% |
| ENTER_EXECUTOR CALL | 1,703,421 | 0.3% | 66.8% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 1,671,353 | 0.3% | 67.1% |
| POP_TOP NOP | 1,670,433 | 0.3% | 67.4% |
| LOAD_FAST GET_ITER | 1,668,451 | 0.3% | 67.7% |
| RETURN_VALUE POP_TOP | 1,652,412 | 0.3% | 68.0% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,650,128 | 0.3% | 68.3% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,639,481 | 0.3% | 68.6% |
| POP_JUMP_IF_FALSE POP_TOP | 1,630,486 | 0.3% | 68.9% |
| BINARY_OP STORE_FAST | 1,604,431 | 0.3% | 69.2% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,585,849 | 0.3% | 69.5% |
| LOAD_FAST TO_BOOL | 1,549,038 | 0.3% | 69.8% |
| RESUME_CHECK NOP | 1,510,787 | 0.3% | 70.0% |
| LOAD_FAST_LOAD_FAST CALL | 1,473,655 | 0.3% | 70.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,472,688 | 0.3% | 70.5% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,471,171 | 0.3% | 70.8% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 1,464,107 | 0.3% | 71.1% |
| LOAD_GLOBAL_MODULE COMPARE_OP_STR | 1,444,035 | 0.3% | 71.3% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 1,440,379 | 0.3% | 71.6% |


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
| RESUME_CHECK | 12,074,825 | 99.0% |
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
| LOAD_ATTR_INSTANCE_VALUE | 1,248,383 | 65.7% |
| RETURN_VALUE | 546,058 | 28.7% |
| LOAD_GLOBAL_MODULE | 82,440 | 4.3% |
| LOAD_FAST | 17,280 | 0.9% |
| CALL | 6,360 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,349,303 | 71.0% |
| STORE_FAST | 551,718 | 29.0% |


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
| LOAD_FAST_LOAD_FAST | 576,080 | 90.9% |
| LOAD_CONST | 56,681 | 8.9% |
| BINARY_SUBSCR | 877 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 575,920 | 90.9% |
| STORE_FAST | 56,401 | 8.9% |
| BINARY_SUBSCR | 877 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 34,941 | 87.1% |
| LOAD_ATTR_MODULE | 5,100 | 12.7% |
| LOAD_GLOBAL | 40 | 0.1% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40,101 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,900 | 48.5% |
| CALL | 27,520 | 35.2% |
| LOAD_ATTR_INSTANCE_VALUE | 12,718 | 16.3% |
| LOAD_ATTR | 82 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60,800 | 77.7% |
| RETURN_CONST | 10,240 | 13.1% |
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
| RETURN_CONST | 1,159,856 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,159,856 | 100.0% |


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
| LOAD_FAST | 1,668,451 | 95.8% |
| CALL_BUILTIN_CLASS | 38,820 | 2.2% |
| CALL | 14,340 | 0.8% |
| STORE_FAST_LOAD_FAST | 6,400 | 0.4% |
| RETURN_VALUE | 5,760 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,106,556 | 63.6% |
| LOAD_FAST_AND_CLEAR | 560,115 | 32.2% |
| FOR_ITER_RANGE | 31,907 | 1.8% |
| FOR_ITER | 12,113 | 0.7% |
| FOR_ITER_TUPLE | 11,740 | 0.7% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,669,907 | 87.5% |
| RETURN_CONST | 941,058 | 7.7% |
| YIELD_VALUE | 577,740 | 4.7% |


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
| LOAD_CONST | 63,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 39,000 | 61.3% |
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
| STORE_FAST | 4,021,955 | 42.3% |
| POP_TOP | 1,670,433 | 17.6% |
| RESUME_CHECK | 1,510,787 | 15.9% |
| POP_JUMP_IF_FALSE | 1,414,281 | 14.9% |
| POP_JUMP_IF_NOT_NONE | 554,698 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,595,567 | 58.9% |
| LOAD_GLOBAL_MODULE | 1,977,817 | 20.8% |
| LOAD_GLOBAL_BUILTIN | 806,621 | 8.5% |
| LOAD_FAST_LOAD_FAST | 583,320 | 6.1% |
| LOAD_CONST | 529,460 | 5.6% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 28,841 | 62.9% |
| COPY | 11,520 | 25.1% |
| POP_TOP | 5,200 | 11.3% |
| STORE_FAST | 280 | 0.6% |
| STORE_SUBSCR_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 29,121 | 63.5% |
| RERAISE | 11,520 | 25.1% |
| JUMP_FORWARD | 5,120 | 11.2% |
| RETURN_CONST | 60 | 0.1% |
| JUMP_BACKWARD | 20 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,913,520 | 27.7% |
| RETURN_CONST | 6,875,670 | 27.6% |
| CALL | 2,292,959 | 9.2% |
| RETURN_VALUE | 1,652,412 | 6.6% |
| POP_JUMP_IF_FALSE | 1,630,486 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,247,782 | 33.1% |
| LOAD_FAST | 7,881,488 | 31.6% |
| RETURN_CONST | 1,965,943 | 7.9% |
| LOAD_CONST | 1,799,239 | 7.2% |
| NOP | 1,670,433 | 6.7% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 34,561 | 75.4% |
| RERAISE | 5,760 | 12.6% |
| CALL_KW | 5,120 | 11.2% |
| BINARY_SUBSCR_DICT | 300 | 0.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 34,901 | 76.1% |
| WITH_EXCEPT_START | 5,760 | 12.6% |
| LOAD_GLOBAL_MODULE | 5,080 | 11.1% |
| LOAD_GLOBAL | 120 | 0.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,405,605 | 42.8% |
| LOAD_ATTR_MODULE | 1,806,551 | 32.1% |
| LOAD_ATTR | 1,284,364 | 22.8% |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 1.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,453,672 | 61.4% |
| CALL | 959,499 | 17.1% |
| LOAD_FAST_LOAD_FAST | 820,886 | 14.6% |
| LOAD_CONST | 315,567 | 5.6% |
| CALL_PY_EXACT_ARGS | 49,320 | 0.9% |


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
| LOAD_FAST | 11,235,514 | 48.1% |
| CALL | 2,612,047 | 11.2% |
| RETURN_VALUE | 2,184,727 | 9.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,734,202 | 7.4% |
| CALL_FUNCTION_EX | 1,265,498 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 10,669,907 | 45.7% |
| STORE_FAST | 2,499,410 | 10.7% |
| RETURN_VALUE | 2,184,727 | 9.3% |
| POP_TOP | 1,652,412 | 7.1% |
| LOAD_FAST_LOAD_FAST | 1,309,087 | 5.6% |


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
| LOAD_FAST | 1,549,038 | 96.2% |
| LOAD_ATTR_INSTANCE_VALUE | 53,502 | 3.3% |
| TO_BOOL | 3,670 | 0.2% |
| LOAD_ATTR | 886 | 0.1% |
| RETURN_VALUE | 763 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 869,630 | 54.0% |
| POP_JUMP_IF_FALSE | 734,237 | 45.6% |
| TO_BOOL | 3,670 | 0.2% |
| TO_BOOL_BOOL | 2,162 | 0.1% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,309,087 | 70.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 561,768 | 30.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,870,935 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 280,769 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 280,809 | 100.0% |


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
| LOAD_GLOBAL_MODULE | 4,208,025 | 53.7% |
| UNARY_INVERT | 1,870,935 | 23.9% |
| POP_JUMP_IF_FALSE | 1,309,087 | 16.7% |
| LOAD_ATTR | 295,024 | 3.8% |
| LOAD_FAST_LOAD_FAST | 84,160 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 3,180,022 | 40.6% |
| STORE_FAST | 1,604,431 | 20.5% |
| TO_BOOL_INT | 1,309,147 | 16.7% |
| UNARY_INVERT | 1,309,087 | 16.7% |
| BUILD_TUPLE | 280,924 | 3.6% |


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
| SWAP | 560,115 | 33.4% |
| JUMP_FORWARD | 545,818 | 32.6% |
| LOAD_FAST | 281,587 | 16.8% |
| POP_TOP | 264,251 | 15.8% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 563,058 | 33.6% |
| SWAP | 560,115 | 33.4% |
| STORE_FAST | 547,278 | 32.6% |
| RETURN_VALUE | 5,120 | 0.3% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 556,018 | 48.1% |
| LOAD_FAST | 529,560 | 45.8% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 3.0% |
| POP_JUMP_IF_NOT_NONE | 17,280 | 1.5% |
| POP_TOP | 7,040 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,133,138 | 98.0% |
| STORE_FAST | 17,280 | 1.5% |
| BUILD_TUPLE | 6,420 | 0.6% |


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
| LOAD_FAST | 1,870,487 | 56.6% |
| LOAD_FAST_LOAD_FAST | 590,720 | 17.9% |
| RETURN_VALUE | 512,000 | 15.5% |
| BINARY_OP | 280,924 | 8.5% |
| LOAD_ATTR_INSTANCE_VALUE | 22,880 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,310,647 | 39.6% |
| YIELD_VALUE | 582,460 | 17.6% |
| STORE_FAST | 512,000 | 15.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 15.5% |
| CALL_LIST_APPEND | 280,844 | 8.5% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,652,230 | 23.3% |
| ENTER_EXECUTOR | 1,703,421 | 14.9% |
| LOAD_FAST_LOAD_FAST | 1,473,655 | 12.9% |
| LOAD_ATTR_METHOD_NO_DICT | 1,429,503 | 12.5% |
| BUILD_TUPLE | 1,310,647 | 11.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,766,554 | 24.3% |
| RETURN_VALUE | 2,612,047 | 22.9% |
| POP_TOP | 2,292,959 | 20.1% |
| LOAD_FAST | 1,148,485 | 10.1% |
| TO_BOOL_BOOL | 726,442 | 6.4% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,678 | 76.6% |
| DICT_MERGE | 564,260 | 23.4% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,265,498 | 52.4% |
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
| LOAD_CONST | 375,699 | 98.6% |
| ENTER_EXECUTOR | 5,440 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 311,531 | 81.7% |
| LOAD_FAST | 28,800 | 7.6% |
| RETURN_VALUE | 21,120 | 5.5% |
| STORE_FAST | 14,220 | 3.7% |
| PUSH_EXC_INFO | 5,120 | 1.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 632,363 | 99.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,614 | 0.3% |
| COMPARE_OP | 1,354 | 0.2% |
| LOAD_GLOBAL_MODULE | 379 | 0.1% |
| LOAD_FAST | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 633,936 | 99.5% |
| COMPARE_OP | 1,354 | 0.2% |
| COMPARE_OP_INT | 1,193 | 0.2% |
| COMPARE_OP_STR | 439 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,882,148 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,882,808 | 100.0% |
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
| BINARY_OP | 3,180,022 | 42.1% |
| STORE_FAST | 2,629,760 | 34.8% |
| LOAD_CONST | 1,100,800 | 14.6% |
| LOAD_FAST | 587,261 | 7.8% |
| STORE_ATTR_INSTANCE_VALUE | 21,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 3,179,702 | 42.1% |
| STORE_FAST | 2,630,400 | 34.8% |
| STORE_FAST_STORE_FAST | 1,093,760 | 14.5% |
| LOAD_ATTR_INSTANCE_VALUE | 573,041 | 7.6% |
| LOAD_FAST | 28,160 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 1,309,087 | 66.4% |
| CALL_ALLOC_AND_ENTER_INIT | 545,778 | 27.7% |
| CACHE | 109,900 | 5.6% |
| CALL | 5,940 | 0.3% |
| CALL_PY_EXACT_ARGS | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,970,565 | 100.0% |
| RETURN_GENERATOR | 340 | 0.0% |
| RESUME | 320 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,600 | 66.7% |
| RETURN_CONST | 27,520 | 31.9% |
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

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,247,782 | 69.2% |
| POP_JUMP_IF_NOT_NONE | 1,040,202 | 8.7% |
| LIST_APPEND | 901,570 | 7.6% |
| STORE_FAST_STORE_FAST | 580,400 | 4.9% |
| FOR_ITER_LIST | 575,320 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 6,322,640 | 53.1% |
| FOR_ITER_LIST | 1,952,209 | 16.4% |
| CALL | 1,703,421 | 14.3% |
| CALL_PY_WITH_DEFAULTS | 832,085 | 7.0% |
| LOAD_ATTR_PROPERTY | 776,401 | 6.5% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 14,160 | 38.9% |
| GET_ITER | 12,113 | 33.3% |
| LOAD_FAST | 6,060 | 16.7% |
| JUMP_BACKWARD | 3,107 | 8.5% |
| FOR_ITER | 940 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 21,080 | 57.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,000 | 33.0% |
| FOR_ITER | 940 | 2.6% |
| STORE_FAST | 760 | 2.1% |
| LOAD_GLOBAL_MODULE | 560 | 1.5% |


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
| RETURN_VALUE | 27,520 | 59.0% |
| LOAD_FAST | 17,420 | 37.4% |
| LOAD_GLOBAL_MODULE | 1,653 | 3.5% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,493 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,760,000 | 90.7% |
| POP_TOP | 582,727 | 9.2% |
| LIST_APPEND | 1,700 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 1,360 | 0.0% |
| STORE_FAST_STORE_FAST | 1,360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 6,335,920 | 99.8% |
| FOR_ITER_LIST | 5,170 | 0.1% |
| FOR_ITER | 3,107 | 0.0% |
| FOR_ITER_RANGE | 2,208 | 0.0% |
| LOAD_FAST | 1,675 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 29,121 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 28,841 | 99.0% |
| LOAD_FAST | 280 | 1.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,158,846 | 64.5% |
| POP_TOP | 620,750 | 34.5% |
| STORE_ATTR_INSTANCE_VALUE | 7,020 | 0.4% |
| BINARY_SUBSCR_TUPLE_INT | 5,720 | 0.3% |
| POP_EXCEPT | 5,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,179,697 | 65.6% |
| BUILD_LIST | 545,818 | 30.4% |
| POP_EXCEPT | 28,841 | 1.6% |
| LOAD_GLOBAL_MODULE | 24,820 | 1.4% |
| LOAD_FAST_LOAD_FAST | 7,320 | 0.4% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 508,826 | 56.3% |
| LOAD_ATTR | 280,944 | 31.1% |
| BINARY_SUBSCR_STR_INT | 112,600 | 12.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 860 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 901,570 | 99.8% |
| JUMP_BACKWARD | 1,700 | 0.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 265,671 | 50.1% |
| RETURN_VALUE | 264,251 | 49.9% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 264,891 | 50.0% |
| STORE_FAST | 264,251 | 49.9% |
| RETURN_VALUE | 640 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.0% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,452,600 | 79.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,862,017 | 17.5% |
| LOAD_GLOBAL_MODULE | 162,841 | 1.5% |
| CALL | 83,860 | 0.8% |
| LOAD_ATTR | 22,641 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,563,258 | 33.5% |
| STORE_SUBSCR_DICT | 1,309,007 | 12.3% |
| PUSH_NULL | 1,284,364 | 12.1% |
| POP_JUMP_IF_NOT_NONE | 1,183,041 | 11.1% |
| RETURN_VALUE | 800,501 | 7.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,923,620 | 25.4% |
| LOAD_FAST | 3,910,687 | 25.3% |
| POP_TOP | 1,799,239 | 11.6% |
| POP_JUMP_IF_FALSE | 943,621 | 6.1% |
| LOAD_ATTR_METHOD_NO_DICT | 731,062 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,923,620 | 25.4% |
| CALL | 2,652,230 | 17.1% |
| COMPARE_OP_INT | 2,173,042 | 14.0% |
| LOAD_FAST | 1,738,065 | 11.2% |
| COPY | 1,100,800 | 7.1% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,964,425 | 97.2% |
| POP_JUMP_IF_NOT_NONE | 27,520 | 1.4% |
| STORE_DEREF | 27,520 | 1.4% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,964,945 | 97.2% |
| POP_JUMP_IF_NOT_NONE | 55,040 | 2.7% |
| PUSH_NULL | 460 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,611,979 | 21.3% |
| STORE_FAST | 12,407,299 | 12.2% |
| POP_JUMP_IF_FALSE | 8,117,330 | 8.0% |
| POP_TOP | 7,881,488 | 7.8% |
| NOP | 5,595,567 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 23,043,273 | 22.7% |
| RETURN_VALUE | 11,235,514 | 11.1% |
| LOAD_ATTR | 8,452,600 | 8.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,687,688 | 7.6% |
| CALL_PY_EXACT_ARGS | 5,497,038 | 5.4% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 560,115 | 66.6% |
| LOAD_FAST_AND_CLEAR | 280,924 | 33.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 560,115 | 66.6% |
| LOAD_FAST_AND_CLEAR | 280,924 | 33.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 576,560 | 67.2% |
| POP_JUMP_IF_NONE | 264,894 | 30.9% |
| LOAD_ATTR_CLASS | 16,518 | 1.9% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 67.1% |
| LOAD_GLOBAL_MODULE | 264,814 | 30.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,478 | 1.9% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,942,405 | 21.7% |
| POP_JUMP_IF_FALSE | 1,639,481 | 12.1% |
| LOAD_FAST_LOAD_FAST | 1,380,147 | 10.2% |
| LOAD_SUPER_ATTR_METHOD | 1,323,367 | 9.8% |
| RETURN_VALUE | 1,309,087 | 9.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,457,418 | 25.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,906,662 | 14.1% |
| CALL | 1,473,655 | 10.9% |
| LOAD_FAST_LOAD_FAST | 1,380,147 | 10.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,309,007 | 9.7% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,000 | 11.2% |
| RESUME_CHECK | 1,720 | 9.6% |
| POP_JUMP_IF_FALSE | 1,709 | 9.6% |
| LOAD_FAST | 1,600 | 9.0% |
| RESUME | 1,520 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,820 | 38.2% |
| LOAD_ATTR | 3,326 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,742 | 15.4% |
| LOAD_FAST | 2,166 | 12.1% |
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
| TO_BOOL_INT | 5,798,236 | 28.5% |
| TO_BOOL_BOOL | 4,991,977 | 24.5% |
| COMPARE_OP_INT | 3,915,995 | 19.3% |
| CONTAINS_OP | 1,882,808 | 9.3% |
| COMPARE_OP_STR | 1,471,171 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,117,330 | 39.9% |
| RETURN_CONST | 3,322,050 | 16.3% |
| LOAD_FAST_LOAD_FAST | 1,639,481 | 8.1% |
| POP_TOP | 1,630,486 | 8.0% |
| LOAD_GLOBAL_MODULE | 1,585,849 | 7.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,132,271 | 93.6% |
| LOAD_ATTR_INSTANCE_VALUE | 47,800 | 4.0% |
| LOAD_ATTR | 28,300 | 2.3% |
| RETURN_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 318,321 | 26.3% |
| NOP | 302,171 | 25.0% |
| LOAD_FAST | 274,770 | 22.7% |
| LOAD_FAST_CHECK | 264,894 | 21.9% |
| RETURN_CONST | 24,340 | 2.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,466,758 | 46.4% |
| LOAD_ATTR | 1,183,041 | 22.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,082,799 | 20.4% |
| RETURN_VALUE | 509,466 | 9.6% |
| LOAD_DEREF | 55,040 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,122,103 | 39.9% |
| RETURN_CONST | 1,184,483 | 22.3% |
| ENTER_EXECUTOR | 1,040,202 | 19.6% |
| NOP | 554,698 | 10.4% |
| LOAD_CONST | 264,531 | 5.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,844,981 | 67.1% |
| TO_BOOL | 869,630 | 31.6% |
| TO_BOOL_NONE | 19,700 | 0.7% |
| COMPARE_OP_STR | 10,903 | 0.4% |
| COMPARE_OP_INT | 3,434 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 955,461 | 34.7% |
| LOAD_FAST_LOAD_FAST | 872,424 | 31.7% |
| RETURN_CONST | 743,223 | 27.0% |
| LOAD_GLOBAL_MODULE | 68,637 | 2.5% |
| RETURN_VALUE | 56,361 | 2.0% |


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
| POP_JUMP_IF_FALSE | 3,322,050 | 34.1% |
| STORE_ATTR_INSTANCE_VALUE | 2,396,672 | 24.6% |
| POP_TOP | 1,965,943 | 20.2% |
| POP_JUMP_IF_NOT_NONE | 1,184,483 | 12.1% |
| POP_JUMP_IF_TRUE | 743,223 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,875,670 | 70.5% |
| EXIT_INIT_CHECK | 1,159,856 | 11.9% |
| INTERPRETER_EXIT | 941,058 | 9.6% |
| TO_BOOL_BOOL | 683,790 | 7.0% |
| STORE_FAST | 58,201 | 0.6% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 39,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 37,920 | 97.2% |
| STORE_NAME | 780 | 2.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.7% |
| LOAD_FAST | 20 | 0.1% |


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
| UNPACK_SEQUENCE_TWO_TUPLE | 20 | 0.0% |

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
| YIELD_VALUE | 6,335,920 | 22.2% |
| CALL | 2,766,554 | 9.7% |
| COPY | 2,630,400 | 9.2% |
| RETURN_VALUE | 2,499,410 | 8.7% |
| BINARY_OP | 1,604,431 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,407,299 | 43.4% |
| JUMP_BACKWARD | 5,760,000 | 20.2% |
| NOP | 4,021,955 | 14.1% |
| COPY | 2,629,760 | 9.2% |
| JUMP_FORWARD | 1,158,846 | 4.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 21,080 | 49.0% |
| COPY | 14,080 | 32.7% |
| FOR_ITER_LIST | 7,020 | 16.3% |
| FOR_ITER_TUPLE | 860 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,640 | 34.0% |
| STORE_ATTR_INSTANCE_VALUE | 14,000 | 32.5% |
| YIELD_VALUE | 7,000 | 16.3% |
| GET_ITER | 6,400 | 14.9% |
| TO_BOOL_STR | 860 | 2.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 1,671,353 | 38.3% |
| COPY | 1,093,760 | 25.1% |
| UNPACK_SEQUENCE_TUPLE | 1,088,220 | 24.9% |
| STORE_FAST_STORE_FAST | 512,000 | 11.7% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,650,128 | 37.8% |
| STORE_FAST | 1,088,280 | 24.9% |
| ENTER_EXECUTOR | 580,400 | 13.3% |
| LOAD_FAST_LOAD_FAST | 518,025 | 11.9% |
| STORE_FAST_STORE_FAST | 512,000 | 11.7% |


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
| BINARY_OP_ADD_INT | 573,101 | 20.3% |
| BUILD_LIST | 560,115 | 19.8% |
| LOAD_FAST_AND_CLEAR | 560,115 | 19.8% |
| FOR_ITER_LIST | 545,175 | 19.3% |
| LOAD_FAST | 292,694 | 10.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 573,618 | 20.3% |
| STORE_ATTR_INSTANCE_VALUE | 573,041 | 20.3% |
| BUILD_LIST | 560,115 | 19.8% |
| STORE_FAST | 560,115 | 19.8% |
| FOR_ITER_LIST | 545,095 | 19.3% |


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
| ENTER_EXECUTOR | 6,322,640 | 91.5% |
| BUILD_TUPLE | 582,460 | 8.4% |
| STORE_FAST_LOAD_FAST | 7,000 | 0.1% |
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
| LOAD_FAST | 281,487 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 281,527 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,090,961 | 98.3% |
| LOAD_FAST_LOAD_FAST | 18,480 | 1.7% |
| BINARY_OP | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 573,101 | 51.6% |
| STORE_FAST | 511,980 | 46.1% |
| BINARY_SLICE | 18,520 | 1.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,680 | 0.5% |
| LOAD_CONST | 280 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,240 | 36.3% |
| CALL_METHOD_DESCRIPTOR_O | 1,240 | 36.3% |
| LOAD_FAST_LOAD_FAST | 600 | 17.5% |
| BINARY_SUBSCR_LIST_INT | 280 | 8.2% |
| BINARY_OP | 40 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,740 | 50.9% |
| LOAD_CONST | 1,260 | 36.8% |
| STORE_FAST | 300 | 8.8% |
| CALL | 120 | 3.5% |


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
| CALL | 264,814 | 99.9% |
| BINARY_OP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,974 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 264,786 | 81.0% |
| LOAD_CONST | 56,281 | 17.2% |
| CALL_LEN | 5,680 | 1.7% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 321,227 | 98.3% |
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
| LOAD_CONST | 11,640 | 63.3% |
| LOAD_FAST_LOAD_FAST | 6,640 | 36.1% |
| BINARY_SUBSCR | 120 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,440 | 62.2% |
| STORE_FAST | 6,680 | 36.3% |
| BINARY_OP_ADD_UNICODE | 280 | 1.5% |


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
| LOAD_GLOBAL_MODULE | 573,218 | 49.4% |
| LOAD_FAST | 552,938 | 47.7% |
| CALL | 33,420 | 2.9% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 614,078 | 52.9% |
| COPY_FREE_VARS | 545,778 | 47.1% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,240 | 82.2% |
| LOAD_CONST | 7,000 | 9.0% |
| BINARY_OP_ADD_INT | 5,680 | 7.3% |
| PUSH_NULL | 996 | 1.3% |
| CALL | 159 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 71,795 | 91.8% |
| POP_TOP | 6,280 | 8.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 800,161 | 48.3% |
| CALL_FUNCTION_EX | 511,960 | 30.9% |
| LOAD_FAST | 299,267 | 18.1% |
| LOAD_CONST | 14,600 | 0.9% |
| LOAD_GLOBAL_BUILTIN | 10,260 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 800,461 | 48.3% |
| RETURN_VALUE | 793,507 | 47.9% |
| GET_ITER | 38,820 | 2.3% |
| LOAD_FAST | 17,280 | 1.0% |
| CALL_BUILTIN_CLASS | 6,320 | 0.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 966,214 | 56.8% |
| LOAD_CONST | 422,451 | 24.9% |
| LOAD_FAST_LOAD_FAST | 173,146 | 10.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,233 | 4.8% |
| LOAD_GLOBAL_MODULE | 27,880 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 618,050 | 36.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 511,585 | 30.1% |
| TO_BOOL_BOOL | 412,391 | 24.3% |
| UNPACK_SEQUENCE_TUPLE | 81,233 | 4.8% |
| POP_TOP | 14,925 | 0.9% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,020 | 45.8% |
| BUILD_TUPLE | 511,960 | 45.2% |
| CALL | 64,975 | 5.7% |
| LOAD_FAST_CHECK | 16,478 | 1.5% |
| LOAD_ATTR | 14,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,047,820 | 92.6% |
| RETURN_VALUE | 82,133 | 7.3% |
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
| LOAD_GLOBAL_BUILTIN | 1,326,547 | 100.0% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,326,827 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 368,469 | 92.9% |
| LOAD_ATTR_INSTANCE_VALUE | 27,900 | 7.0% |
| CALL | 382 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 344,226 | 86.8% |
| CALL_PY_EXACT_ARGS | 33,160 | 8.4% |
| CALL_BUILTIN_CLASS | 6,320 | 1.6% |
| LOAD_FAST | 5,720 | 1.4% |
| BINARY_OP_SUBTRACT_INT | 5,680 | 1.4% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 280,844 | 95.9% |
| LOAD_FAST | 11,440 | 3.9% |
| LOAD_CONST | 140 | 0.0% |
| LOAD_FAST_CHECK | 140 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 280,244 | 95.7% |
| LOAD_GLOBAL_MODULE | 11,440 | 3.9% |
| JUMP_BACKWARD | 640 | 0.2% |
| NOP | 280 | 0.1% |
| RETURN_CONST | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,854,885 | 99.8% |
| LOAD_CONST | 1,240 | 0.1% |
| LOAD_GLOBAL_MODULE | 1,140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 511 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,309,367 | 70.5% |
| STORE_FAST | 546,589 | 29.4% |
| TO_BOOL_NONE | 1,240 | 0.1% |
| LIST_APPEND | 860 | 0.0% |
| LOAD_FAST | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 32,520 | 84.7% |
| BUILD_TUPLE | 5,680 | 14.8% |
| CALL | 180 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 26,900 | 70.1% |
| LOAD_FAST | 11,480 | 29.9% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,440,379 | 93.5% |
| LOAD_ATTR_METHOD_LAZY_DICT | 97,711 | 6.3% |
| LOAD_ATTR | 2,480 | 0.2% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 695,420 | 45.1% |
| STORE_FAST | 575,960 | 37.4% |
| LOAD_FAST | 85,060 | 5.5% |
| CALL_BUILTIN_FAST | 81,233 | 5.3% |
| RETURN_VALUE | 51,596 | 3.3% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 879,309 | 91.7% |
| LOAD_CONST | 33,720 | 3.5% |
| CALL | 29,140 | 3.0% |
| RETURN_VALUE | 14,000 | 1.5% |
| RETURN_GENERATOR | 1,300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 908,589 | 94.8% |
| LOAD_CONST | 33,440 | 3.5% |
| RETURN_VALUE | 14,900 | 1.6% |
| BINARY_OP_ADD_UNICODE | 1,240 | 0.1% |
| STORE_FAST | 280 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 5,924,518 | 45.9% |
| LOAD_FAST | 5,497,038 | 42.6% |
| LOAD_FAST_LOAD_FAST | 596,520 | 4.6% |
| LOAD_SUPER_ATTR_METHOD | 545,738 | 4.2% |
| LOAD_GLOBAL_MODULE | 93,900 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,856,235 | 99.6% |
| MAKE_CELL | 27,800 | 0.2% |
| RETURN_GENERATOR | 18,420 | 0.1% |
| COPY_FREE_VARS | 320 | 0.0% |
| PUSH_EXC_INFO | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 1,208,463 | 38.4% |
| ENTER_EXECUTOR | 832,085 | 26.4% |
| LOAD_ATTR_MODULE | 545,937 | 17.3% |
| LOAD_FAST | 363,884 | 11.6% |
| LOAD_CONST | 107,209 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,838,372 | 58.4% |
| COPY_FREE_VARS | 1,309,087 | 41.6% |


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
| LOAD_CONST | 2,173,042 | 55.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,126,232 | 28.7% |
| LOAD_FAST | 576,980 | 14.7% |
| LOAD_FAST_LOAD_FAST | 18,480 | 0.5% |
| CALL_BUILTIN_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,915,995 | 99.9% |
| POP_JUMP_IF_TRUE | 3,434 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 112 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,444,035 | 95.6% |
| LOAD_CONST | 59,860 | 4.0% |
| LOAD_FAST | 5,820 | 0.4% |
| COMPARE_OP | 439 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,471,171 | 97.4% |
| COPY | 14,040 | 0.9% |
| LOAD_FAST | 14,040 | 0.9% |
| POP_JUMP_IF_TRUE | 10,903 | 0.7% |


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
| ENTER_EXECUTOR | 1,952,209 | 54.1% |
| GET_ITER | 1,106,556 | 30.7% |
| SWAP | 545,095 | 15.1% |
| JUMP_BACKWARD | 5,170 | 0.1% |
| FOR_ITER | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,091,636 | 30.2% |
| STORE_FAST | 819,291 | 22.7% |
| ENTER_EXECUTOR | 575,320 | 15.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 561,828 | 15.6% |
| SWAP | 545,175 | 15.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 274,451 | 88.9% |
| GET_ITER | 31,907 | 10.3% |
| JUMP_BACKWARD | 2,208 | 0.7% |
| FOR_ITER | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 264,411 | 85.6% |
| STORE_FAST | 33,475 | 10.8% |
| RETURN_CONST | 10,880 | 3.5% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 13,420 | 48.1% |
| GET_ITER | 11,740 | 42.0% |
| LOAD_FAST | 1,260 | 4.5% |
| SWAP | 860 | 3.1% |
| JUMP_BACKWARD | 600 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,140 | 47.1% |
| LOAD_FAST | 10,460 | 37.5% |
| RETURN_CONST | 2,560 | 9.2% |
| STORE_FAST_LOAD_FAST | 860 | 3.1% |
| SWAP | 860 | 3.1% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 81,193 | 88.8% |
| LOAD_ATTR_MODULE | 10,200 | 11.2% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,955 | 81.9% |
| LOAD_FAST_CHECK | 16,518 | 18.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,043,273 | 90.1% |
| LOAD_FAST_LOAD_FAST | 1,906,662 | 7.5% |
| COPY | 573,041 | 2.2% |
| LOAD_ATTR_INSTANCE_VALUE | 23,734 | 0.1% |
| RETURN_VALUE | 14,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,807,231 | 22.7% |
| LOAD_FAST | 3,882,667 | 15.2% |
| TO_BOOL_BOOL | 2,003,618 | 7.8% |
| CONTAINS_OP | 1,882,148 | 7.4% |
| LOAD_ATTR | 1,862,017 | 7.3% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 408,732 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,586 | 39.8% |
| CALL | 148,615 | 36.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 97,711 | 23.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,807,231 | 87.4% |
| LOAD_FAST | 636,204 | 9.6% |
| LOAD_ATTR | 85,280 | 1.3% |
| LOAD_ATTR_SLOT | 83,760 | 1.3% |
| LOAD_CONST | 15,520 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,689,259 | 40.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,440,379 | 21.7% |
| CALL | 1,429,503 | 21.5% |
| LOAD_CONST | 731,062 | 11.0% |
| LOAD_FAST_LOAD_FAST | 323,012 | 4.9% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,687,688 | 69.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,381,890 | 12.6% |
| LOAD_FAST_LOAD_FAST | 1,309,007 | 11.9% |
| BINARY_SUBSCR | 575,920 | 5.2% |
| LOAD_GLOBAL_MODULE | 28,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 5,924,518 | 53.8% |
| LOAD_FAST | 2,962,730 | 26.9% |
| CALL_PY_WITH_DEFAULTS | 1,208,463 | 11.0% |
| LOAD_FAST_LOAD_FAST | 678,560 | 6.2% |
| LOAD_CONST | 125,689 | 1.1% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,504,912 | 99.9% |
| LOAD_ATTR | 2,821 | 0.1% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,806,551 | 72.0% |
| CALL_PY_WITH_DEFAULTS | 545,937 | 21.8% |
| STORE_DEREF | 55,040 | 2.2% |
| LOAD_CONST | 35,840 | 1.4% |
| LOAD_FAST | 28,800 | 1.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,349,607 | 70.6% |
| LOAD_FAST_LOAD_FAST | 561,688 | 29.4% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,309,047 | 68.5% |
| UNARY_INVERT | 561,768 | 29.4% |
| RETURN_VALUE | 14,040 | 0.7% |
| LOAD_CONST | 14,040 | 0.7% |
| LOAD_FAST_LOAD_FAST | 5,720 | 0.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 776,401 | 68.2% |
| LOAD_FAST | 333,081 | 29.3% |
| RETURN_VALUE | 27,440 | 2.4% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.1% |
| LOAD_ATTR | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,126,322 | 98.9% |
| TO_BOOL_BOOL | 12,160 | 1.1% |
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
| RESUME_CHECK | 3,961,792 | 50.9% |
| LOAD_FAST | 1,353,187 | 17.4% |
| NOP | 806,621 | 10.4% |
| STORE_FAST | 776,804 | 10.0% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,817,377 | 49.0% |
| LOAD_DEREF | 1,964,425 | 25.2% |
| CALL_ISINSTANCE | 1,326,547 | 17.0% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 6.7% |
| LOAD_GLOBAL_MODULE | 49,720 | 0.6% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,618,411 | 27.5% |
| RESUME_CHECK | 3,111,963 | 18.5% |
| NOP | 1,977,817 | 11.8% |
| POP_JUMP_IF_FALSE | 1,585,849 | 9.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,472,688 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,208,025 | 25.0% |
| LOAD_FAST_LOAD_FAST | 2,942,405 | 17.5% |
| LOAD_ATTR_MODULE | 2,504,912 | 14.9% |
| LOAD_FAST | 2,356,212 | 14.0% |
| LOAD_GLOBAL_MODULE | 1,464,107 | 8.7% |


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
| LOAD_FAST | 1,874,705 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,323,367 | 70.6% |
| CALL_PY_EXACT_ARGS | 545,738 | 29.1% |
| LOAD_FAST | 5,760 | 0.3% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 12,856,235 | 33.6% |
| CACHE | 12,074,825 | 31.5% |
| FOR_ITER_GEN | 6,335,920 | 16.5% |
| COPY_FREE_VARS | 1,970,565 | 5.1% |
| CALL_PY_WITH_DEFAULTS | 1,838,372 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,611,979 | 56.4% |
| POP_TOP | 6,913,520 | 18.1% |
| LOAD_GLOBAL_BUILTIN | 3,961,792 | 10.3% |
| LOAD_GLOBAL_MODULE | 3,111,963 | 8.1% |
| NOP | 1,510,787 | 3.9% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,267,789 | 69.7% |
| LOAD_FAST_LOAD_FAST | 807,518 | 17.2% |
| SWAP | 573,041 | 12.2% |
| LOAD_ATTR_INSTANCE_VALUE | 17,040 | 0.4% |
| STORE_FAST_LOAD_FAST | 14,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,396,672 | 51.1% |
| LOAD_FAST | 937,761 | 20.0% |
| LOAD_GLOBAL_MODULE | 784,358 | 16.7% |
| LOAD_CONST | 302,858 | 6.5% |
| LOAD_FAST_LOAD_FAST | 129,480 | 2.8% |


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
| LOAD_ATTR | 1,309,007 | 93.5% |
| LOAD_FAST | 44,950 | 3.2% |
| LOAD_ATTR_INSTANCE_VALUE | 34,680 | 2.5% |
| CALL | 10,200 | 0.7% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,312,417 | 93.7% |
| RETURN_CONST | 32,520 | 2.3% |
| LOAD_GLOBAL_MODULE | 27,720 | 2.0% |
| LOAD_CONST | 27,480 | 2.0% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 61.6% |
| COPY | 334 | 34.3% |
| TO_BOOL | 40 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 620 | 63.7% |
| POP_JUMP_IF_FALSE | 354 | 36.3% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,003,618 | 28.1% |
| CALL_ISINSTANCE | 1,326,827 | 18.6% |
| RETURN_VALUE | 957,360 | 13.5% |
| CALL | 726,442 | 10.2% |
| LOAD_FAST | 716,121 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,991,977 | 70.1% |
| POP_JUMP_IF_TRUE | 1,844,981 | 25.9% |
| UNARY_NOT | 280,769 | 3.9% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 3,179,702 | 54.8% |
| BINARY_OP | 1,309,147 | 22.6% |
| LOAD_FAST | 1,309,007 | 22.6% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,798,236 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 557,238 | 92.8% |
| LOAD_ATTR_INSTANCE_VALUE | 42,900 | 7.1% |
| TO_BOOL | 200 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 600,198 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 191,414 | 79.6% |
| LOAD_FAST | 27,900 | 11.6% |
| COPY | 13,880 | 5.8% |
| WITH_EXCEPT_START | 5,680 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220,774 | 91.8% |
| POP_JUMP_IF_TRUE | 19,700 | 8.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 860 | 51.8% |
| LOAD_FAST | 620 | 37.3% |
| COPY | 160 | 9.6% |
| LOAD_GLOBAL_MODULE | 20 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,460 | 88.0% |
| POP_JUMP_IF_TRUE | 200 | 12.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,087,880 | 93.0% |
| CALL_BUILTIN_FAST | 81,233 | 6.9% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,088,220 | 93.1% |
| STORE_FAST | 81,273 | 6.9% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_CHECK | 575,920 | 34.3% |
| FOR_ITER_LIST | 561,828 | 33.5% |
| CALL_BUILTIN_FAST | 511,585 | 30.5% |
| FOR_ITER | 12,000 | 0.7% |
| CALL | 9,440 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,671,353 | 99.6% |
| LOAD_FAST | 7,000 | 0.4% |
| STORE_DEREF | 20 | 0.0% |


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
|     deferred | 7,821,885 | 78.6% |
|          hit | 2,126,549 | 21.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 600 | 8.3% |
| Failure | 6,651 | 91.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,339 | 50.2% |
| or | 1,793 | 27.0% |
| remainder | 779 | 11.7% |
| add different types | 640 | 9.6% |
| add other | 100 | 1.5% |


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
|     deferred | 632,601 | 68.9% |
|          hit | 285,040 | 31.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 21.5% |
| Failure | 877 | 78.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 877 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,368,770 | 28.1% |
|          hit | 29,004,762 | 71.8% |
|         miss | 7,840 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,284 | 23.4% |
| Failure | 30,329 | 76.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,931 | 26.1% |
| cfunc noargs | 6,357 | 21.0% |
| class no vectorcall | 4,000 | 13.2% |
| meth descr varargs keywords | 3,208 | 10.6% |
| class mutable | 1,320 | 4.4% |
| other | 1,180 | 3.9% |
| bound method | 1,133 | 3.7% |
| cfunc varargs | 1,100 | 3.6% |
| cfunc varargs keywords | 960 | 3.2% |
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
|     deferred | 641,651 | 10.6% |
|          hit | 5,422,668 | 89.4% |
|         miss | 7,467 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,632 | 52.7% |
| Failure | 1,466 | 47.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 826 | 56.3% |
| big int | 360 | 24.6% |
| different types | 280 | 19.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,820 | 0.3% |
|          hit | 10,293,516 | 99.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 39.7% |
| Failure | 940 | 60.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| itertools | 280 | 29.8% |
| other | 220 | 23.4% |
| enumerate | 220 | 23.4% |
| callable | 220 | 23.4% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,892,363 | 18.2% |
|          hit | 49,065,870 | 81.8% |
|         miss | 311,202 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,468 | 52.4% |
| Failure | 20,396 | 47.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,635 | 22.7% |
| shadowed | 4,314 | 21.2% |
| not managed dict | 3,866 | 19.0% |
| non overriding descriptor | 2,126 | 10.4% |
| has managed dict | 1,120 | 5.5% |
| class attr descriptor | 1,040 | 5.1% |
| metaclass attribute | 960 | 4.7% |
| class method obj | 920 | 4.5% |
| non object slot | 560 | 2.7% |
| class attr simple | 495 | 2.4% |
| mutable class | 280 | 1.4% |
| overridden | 80 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,250 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 24,588,227 | 99.9% |
|         miss | 4,998 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,602 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,964,425 | 100.0% |

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
|     deferred | 334,622 | 6.8% |
|          hit | 4,541,009 | 92.9% |
|         miss | 245,260 | 5.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,981 | 78.1% |
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
|     deferred | 30,340 | 2.1% |
|          hit | 1,400,337 | 97.8% |

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
|     deferred | 1,604,187 | 10.4% |
|          hit | 13,759,289 | 89.5% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,002 | 45.0% |
| Failure | 3,670 | 55.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,093 | 29.8% |
| sequence | 877 | 23.9% |
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
|          hit | 2,847,866 | 100.0% |

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
| Basic | 312,890,369 | 55.9% |
| Not specialized | 62,560,010 | 11.2% |
| Specialized hits | 183,524,440 | 32.8% |
| Specialized misses | 577,047 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 11,368,770 | 34.1% |
| LOAD_ATTR | 10,892,363 | 32.6% |
| BINARY_OP | 7,821,885 | 23.4% |
| TO_BOOL | 1,604,187 | 4.8% |
| COMPARE_OP | 641,651 | 1.9% |
| BINARY_SUBSCR | 632,601 | 1.9% |
| STORE_ATTR | 334,622 | 1.0% |
| FOR_ITER | 34,820 | 0.1% |
| STORE_SUBSCR | 30,340 | 0.1% |
| LOAD_GLOBAL | 13,250 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.5% |
| LOAD_ATTR_INSTANCE_VALUE | 215,782 | 37.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 81,940 | 14.2% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.1% |
| COMPARE_OP_INT | 7,447 | 1.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,380 | 1.1% |
| LOAD_GLOBAL_MODULE | 4,658 | 0.8% |
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
| Calls to PyEval_EvalDefault | 12,194,485 | 31.8% |
| Calls to Python functions inlined | 26,127,032 | 68.2% |
| Calls via PyEval_EvalFrame (total) | 12,194,485 | 31.8% |
| Calls via PyEval_EvalFrame (vector) | 11,609,365 | 30.3% |
| Calls via PyEval_EvalFrame (generator) | 585,120 | 1.5% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 11,608,665 | 30.3% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 625,920 | 1.6% |
| Calls via PyEval_EvalFrame (function ex) | 535,340 | 1.4% |
| Calls via PyEval_EvalFrame (api) | 684,126 | 1.8% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 45,979 | 0.1% |
| Frames pushed | 20,281,542 | 52.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 20,197,317 | 42.1% |
| Frees to freelist | 20,210,021 |  |
| Allocations | 27,813,806 | 57.9% |
| Allocations to 512 bytes | 27,524,584 | 57.3% |
| Allocations to 4 kbytes | 117,741 | 0.2% |
| Allocations over 4 kbytes | 171,481 | 0.4% |
| Frees | 29,423,962 |  |
| New values | 88,020 |  |
| Interpreter increfs | 248,268,812 | 77.8% |
| Interpreter decrefs | 271,207,627 | 74.9% |
| Increfs | 70,864,319 | 22.2% |
| Decrefs | 90,989,762 | 25.1% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 13,316,082 |  |
| Method cache misses | 32,232 |  |
| Method cache collisions | 35,820 |  |
| Method cache dunder hits | 11,949,294 |  |
| Method cache dunder misses | 8,095 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 60 | 3,840 | 452,800 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,450 |  |
| Traces created | 870 | 19.6% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 3,580 | 80.4% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 11,911,098 |  |
| Uops executed | 110,069,168 | 9.24 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 120 | 13.8% |
| <= 32 | 380 | 43.7% |
| <= 64 | 200 | 23.0% |
| <= 128 | 150 | 17.2% |
| <= 256 | 20 | 2.3% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 40 | 4.6% |
| <= 8 | 80 | 9.2% |
| <= 16 | 380 | 43.7% |
| <= 32 | 160 | 18.4% |
| <= 64 | 90 | 10.3% |
| <= 128 | 120 | 13.8% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,979,921 | 16.6% |
| <= 4 | 1,292,851 | 10.9% |
| <= 8 | 5,184,196 | 43.5% |
| <= 16 | 1,771,154 | 14.9% |
| <= 32 | 1,354,858 | 11.4% |
| <= 64 | 6,044 | 0.1% |
| <= 128 | 322,024 | 2.7% |
| <= 256 | 5 | 0.0% |
| <= 512 | 1 | 0.0% |
| <= 1,024 | 3 | 0.0% |
| <= 2,048 | 10 | 0.0% |
| <= 4,096 | 9 | 0.0% |
| <= 8,192 | 22 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 18,517,662 | 16.8% | 16.8% |  |
| STORE_FAST | 9,916,292 | 9.0% | 25.8% |  |
| _EXIT_TRACE | 9,640,027 | 8.8% | 34.6% | 100.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 8,739,267 | 7.9% | 42.5% | 22.3% |
| _ITER_CHECK_LIST | 8,739,267 | 7.9% | 50.5% |  |
| _SET_IP | 8,095,000 | 7.4% | 57.8% |  |
| _CHECK_VALIDITY | 7,269,948 | 6.6% | 64.4% |  |
| _ITER_NEXT_LIST | 6,787,058 | 6.2% | 70.6% |  |
| _GUARD_GLOBALS_VERSION | 3,218,907 | 2.9% | 73.5% |  |
| PUSH_NULL | 1,875,781 | 1.7% | 75.2% |  |
| _GUARD_BUILTINS_VERSION | 1,612,844 | 1.5% | 76.7% |  |
| _LOAD_GLOBAL_BUILTINS | 1,612,844 | 1.5% | 78.2% |  |
| _LOAD_GLOBAL_MODULE | 1,606,063 | 1.5% | 79.6% |  |
| _CHECK_ATTR_MODULE | 1,339,931 | 1.2% | 80.8% |  |
| _LOAD_ATTR_MODULE | 1,339,931 | 1.2% | 82.0% |  |
| _FOR_ITER_TIER_TWO | 1,268,120 | 1.2% | 83.2% | 2.4% |
| BUILD_TUPLE | 1,144,720 | 1.0% | 84.2% |  |
| _GUARD_TYPE_VERSION | 1,074,625 | 1.0% | 85.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 966,982 | 0.9% | 86.1% |  |
| _GUARD_KEYS_VERSION | 966,982 | 0.9% | 87.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 966,982 | 0.9% | 87.9% |  |
| GET_ITER | 827,491 | 0.8% | 88.6% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 811,633 | 0.7% | 89.3% | 33.8% |
| _ITER_CHECK_RANGE | 811,633 | 0.7% | 90.1% |  |
| _CHECK_PEP_523 | 714,319 | 0.6% | 90.7% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 714,319 | 0.6% | 91.4% |  |
| _CHECK_STACK_SPACE | 714,319 | 0.6% | 92.0% |  |
| _INIT_CALL_PY_EXACT_ARGS | 714,319 | 0.6% | 92.7% |  |
| _PUSH_FRAME | 714,319 | 0.6% | 93.3% |  |
| _SAVE_RETURN_OFFSET | 714,319 | 0.6% | 94.0% |  |
| RESUME_CHECK | 714,279 | 0.6% | 94.6% |  |
| _LOAD_CONST_INLINE | 669,222 | 0.6% | 95.2% |  |
| _LOAD_ATTR | 580,342 | 0.5% | 95.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 570,060 | 0.5% | 96.3% |  |
| BUILD_MAP | 569,600 | 0.5% | 96.8% |  |
| _ITER_NEXT_RANGE | 537,182 | 0.5% | 97.3% |  |
| BINARY_SUBSCR_LIST_INT | 521,782 | 0.5% | 97.8% |  |
| CALL_BUILTIN_CLASS | 515,702 | 0.5% | 98.2% |  |
| TO_BOOL_BOOL | 328,472 | 0.3% | 98.5% |  |
| _GUARD_IS_TRUE_POP | 322,402 | 0.3% | 98.8% | 0.0% |
| CALL_BUILTIN_FAST | 263,931 | 0.2% | 99.1% |  |
| CALL_LEN | 257,851 | 0.2% | 99.3% |  |
| POP_TOP | 147,915 | 0.1% | 99.4% |  |
| _POP_FRAME | 128,701 | 0.1% | 99.5% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 92,986 | 0.1% | 99.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 92,986 | 0.1% | 99.7% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.1% | 99.8% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.1% | 99.8% |  |
| _GUARD_IS_NOT_NONE_POP | 64,160 | 0.1% | 99.9% |  |
| _JUMP_TO_TOP | 24,616 | 0.0% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 15,720 | 0.0% | 99.9% | 85.4% |
| _ITER_CHECK_TUPLE | 15,720 | 0.0% | 99.9% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 11,818 | 0.0% | 99.9% |  |
| _GUARD_IS_FALSE_POP | 10,430 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,080 | 0.0% | 100.0% |  |
| BEFORE_WITH | 5,335 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,960 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 3,979 | 0.0% | 100.0% |  |
| CONTAINS_OP | 2,839 | 0.0% | 100.0% |  |
| COPY | 2,839 | 0.0% | 100.0% |  |
| SWAP | 2,839 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 2,839 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 2,839 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 2,839 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 2,839 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 2,839 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 2,300 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,140 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,140 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 420 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 420 | 0.0% | 100.0% |  |
| IS_OP | 381 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 40 | 0.0% | 100.0% |  |
| LOAD_CONST | 40 | 0.0% | 100.0% |  |
| LOAD_DEREF | 40 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 40 | 0.0% | 100.0% |  |
| STORE_DEREF | 40 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 3,620 |
| CALL | 214 |
| YIELD_VALUE | 140 |
| LOAD_ATTR_PROPERTY | 140 |
| CALL_PY_WITH_DEFAULTS | 120 |
| CALL_KW | 40 |
| CALL_LIST_APPEND | 40 |


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
Stats gathered on: 2024-01-17
