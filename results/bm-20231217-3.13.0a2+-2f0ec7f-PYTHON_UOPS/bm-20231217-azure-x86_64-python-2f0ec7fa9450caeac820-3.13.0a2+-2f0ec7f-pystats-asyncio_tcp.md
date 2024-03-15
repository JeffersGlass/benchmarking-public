
# Pystats results

- benchmark: asyncio_tcp
- fork: python
- ref: 2f0ec7fa9450caeac820a6dc819d17d14fd16a4b
- commit hash: 2f0ec7f
- commit date: 2023-12-17T00:07:32+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 82,529,351 | 21.3% | 21.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 27,049,591 | 7.0% | 28.3% |  |
| RESUME_CHECK | 20,568,544 | 5.3% | 33.6% | 0.0% |
| POP_JUMP_IF_FALSE | 16,511,022 | 4.3% | 37.9% |  |
| STORE_FAST | 16,353,850 | 4.2% | 42.1% |  |
| CALL_PY_EXACT_ARGS | 14,942,135 | 3.9% | 46.0% |  |
| TO_BOOL_BOOL | 13,174,086 | 3.4% | 49.4% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 13,000,343 | 3.4% | 52.8% |  |
| LOAD_CONST | 12,888,330 | 3.3% | 56.1% |  |
| POP_TOP | 12,845,106 | 3.3% | 59.4% |  |
| RETURN_VALUE | 12,549,566 | 3.2% | 62.7% |  |
| LOAD_GLOBAL_MODULE | 7,806,220 | 2.0% | 64.7% |  |
| LOAD_FAST_LOAD_FAST | 7,768,435 | 2.0% | 66.7% |  |
| RETURN_CONST | 7,763,235 | 2.0% | 68.7% |  |
| LOAD_GLOBAL_BUILTIN | 6,717,064 | 1.7% | 70.4% | 0.0% |
| LOAD_ATTR_SLOT | 6,707,877 | 1.7% | 72.2% |  |
| POP_JUMP_IF_TRUE | 6,004,296 | 1.6% | 73.7% |  |
| LOAD_ATTR_METHOD_NO_DICT | 5,781,776 | 1.5% | 75.2% |  |
| STORE_ATTR_SLOT | 5,612,516 | 1.5% | 76.7% |  |
| LOAD_ATTR | 5,521,298 | 1.4% | 78.1% |  |
| NOP | 4,622,963 | 1.2% | 79.3% |  |
| CALL | 4,373,005 | 1.1% | 80.4% |  |
| BINARY_OP | 4,169,081 | 1.1% | 81.5% |  |
| TO_BOOL_INT | 3,819,822 | 1.0% | 82.5% |  |
| LOAD_ATTR_MODULE | 3,421,423 | 0.9% | 83.4% |  |
| PUSH_NULL | 3,026,883 | 0.8% | 84.1% |  |
| COMPARE_OP_INT | 2,741,553 | 0.7% | 84.8% |  |
| INTERPRETER_EXIT | 2,666,472 | 0.7% | 85.5% |  |
| ENTER_EXECUTOR | 2,425,433 | 0.6% | 86.2% |  |
| COPY | 2,311,321 | 0.6% | 86.8% |  |
| POP_JUMP_IF_NONE | 2,287,629 | 0.6% | 87.4% |  |
| STORE_ATTR_INSTANCE_VALUE | 2,268,614 | 0.6% | 87.9% |  |
| POP_JUMP_IF_NOT_NONE | 2,005,772 | 0.5% | 88.5% |  |
| CALL_LEN | 1,982,956 | 0.5% | 89.0% |  |
| FOR_ITER_LIST | 1,969,049 | 0.5% | 89.5% |  |
| JUMP_FORWARD | 1,955,768 | 0.5% | 90.0% |  |
| TO_BOOL | 1,734,043 | 0.4% | 90.4% |  |
| SEND_GEN | 1,636,490 | 0.4% | 90.9% |  |
| GET_ITER | 1,604,276 | 0.4% | 91.3% |  |
| STORE_FAST_STORE_FAST | 1,395,780 | 0.4% | 91.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,395,340 | 0.4% | 92.0% |  |
| CALL_ISINSTANCE | 1,315,148 | 0.3% | 92.3% |  |
| YIELD_VALUE | 1,307,672 | 0.3% | 92.7% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 1,307,512 | 0.3% | 93.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,289,154 | 0.3% | 93.3% |  |
| FOR_ITER_RANGE | 1,283,336 | 0.3% | 93.7% |  |
| UNARY_NOT | 1,280,160 | 0.3% | 94.0% |  |
| BUILD_LIST | 1,275,478 | 0.3% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_O | 1,094,097 | 0.3% | 94.6% | 0.0% |
| BUILD_TUPLE | 1,032,367 | 0.3% | 94.9% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,025,664 | 0.3% | 95.1% | 0.1% |
| CALL_FUNCTION_EX | 1,024,471 | 0.3% | 95.4% |  |
| END_SEND | 987,034 | 0.3% | 95.7% |  |
| GET_AWAITABLE | 987,034 | 0.3% | 95.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 968,714 | 0.3% | 96.2% |  |
| CALL_INTRINSIC_1 | 961,778 | 0.2% | 96.4% |  |
| LIST_EXTEND | 961,778 | 0.2% | 96.7% |  |
| TO_BOOL_LIST | 954,578 | 0.2% | 96.9% |  |
| LOAD_DEREF | 727,330 | 0.2% | 97.1% |  |
| CALL_BUILTIN_CLASS | 719,167 | 0.2% | 97.3% |  |
| SWAP | 710,907 | 0.2% | 97.5% |  |
| COPY_FREE_VARS | 691,622 | 0.2% | 97.7% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 664,399 | 0.2% | 97.8% |  |
| TO_BOOL_NONE | 662,356 | 0.2% | 98.0% |  |
| SEND | 659,236 | 0.2% | 98.2% |  |
| RETURN_GENERATOR | 658,636 | 0.2% | 98.3% |  |
| CALL_PY_WITH_DEFAULTS | 657,814 | 0.2% | 98.5% |  |
| UNARY_INVERT | 648,547 | 0.2% | 98.7% |  |
| LOAD_SUPER_ATTR_METHOD | 642,480 | 0.2% | 98.8% |  |
| BINARY_OP_ADD_FLOAT | 641,258 | 0.2% | 99.0% |  |
| CALL_LIST_APPEND | 373,733 | 0.1% | 99.1% |  |
| BINARY_SLICE | 373,673 | 0.1% | 99.2% |  |
| CALL_KW | 346,932 | 0.1% | 99.3% |  |
| STORE_SUBSCR_DICT | 336,634 | 0.1% | 99.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 336,092 | 0.1% | 99.5% |  |
| CONTAINS_OP | 321,520 | 0.1% | 99.5% |  |
| LOAD_ATTR_PROPERTY | 321,138 | 0.1% | 99.6% |  |
| BINARY_OP_ADD_INT | 320,598 | 0.1% | 99.7% |  |
| DELETE_SUBSCR | 320,318 | 0.1% | 99.8% |  |
| BUILD_SLICE | 320,318 | 0.1% | 99.9% |  |
| BINARY_OP_MULTIPLY_INT | 320,278 | 0.1% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60,855 | 0.0% | 100.0% |  |
| COMPARE_OP | 19,094 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 16,954 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 9,620 | 0.0% | 100.0% |  |
| FOR_ITER | 9,540 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 8,100 | 0.0% | 100.0% |  |
| STORE_ATTR | 7,500 | 0.0% | 100.0% |  |
| RESUME | 4,340 | 0.0% | 100.0% | 0.5% |
| JUMP_BACKWARD | 3,553 | 0.0% | 100.0% |  |
| MAKE_CELL | 1,440 | 0.0% | 100.0% |  |
| IS_OP | 1,360 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 940 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 900 | 0.0% | 100.0% |  |
| STORE_DEREF | 880 | 0.0% | 100.0% |  |
| BUILD_MAP | 800 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 680 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 680 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 680 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 660 | 0.0% | 100.0% |  |
| POP_EXCEPT | 660 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 660 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 560 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 560 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 500 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 440 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 440 | 0.0% | 100.0% |  |
| BUILD_SET | 400 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 380 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 240 | 0.0% | 100.0% | 25.0% |
| DICT_MERGE | 240 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 240 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 200 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 180 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 180 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 160 | 0.0% | 100.0% |  |
| IMPORT_NAME | 100 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 80 | 0.0% | 100.0% |  |
| LIST_APPEND | 80 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 80 | 0.0% | 100.0% |  |
| RERAISE | 80 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% | 100.0% |  |
| BEFORE_WITH | 40 | 0.0% | 100.0% |  |
| IMPORT_FROM | 20 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 20 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 20 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 26,050,843 | 6.7% | 6.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 13,947,143 | 3.6% | 10.3% |
| RESUME_CHECK LOAD_FAST | 13,256,946 | 3.4% | 13.8% |
| STORE_FAST LOAD_FAST | 9,886,676 | 2.6% | 16.3% |
| POP_JUMP_IF_FALSE LOAD_FAST | 9,112,308 | 2.4% | 18.7% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 8,925,412 | 2.3% | 21.0% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 7,040,735 | 1.8% | 22.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 6,698,997 | 1.7% | 24.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 6,429,585 | 1.7% | 26.2% |
| RETURN_CONST POP_TOP | 6,388,999 | 1.7% | 27.8% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,940,136 | 1.5% | 29.4% |
| LOAD_CONST LOAD_FAST | 5,883,926 | 1.5% | 30.9% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 5,834,001 | 1.5% | 32.4% |
| POP_TOP LOAD_FAST | 5,334,585 | 1.4% | 33.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 5,289,558 | 1.4% | 35.2% |
| LOAD_FAST RETURN_VALUE | 4,593,629 | 1.2% | 36.3% |
| LOAD_FAST LOAD_ATTR | 4,509,632 | 1.2% | 37.5% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 4,314,768 | 1.1% | 38.6% |
| POP_JUMP_IF_TRUE LOAD_FAST | 3,700,107 | 1.0% | 39.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 3,635,855 | 0.9% | 40.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 3,627,258 | 0.9% | 41.5% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 3,613,731 | 0.9% | 42.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 3,419,403 | 0.9% | 43.3% |
| NOP LOAD_FAST | 3,308,695 | 0.9% | 44.1% |
| RETURN_VALUE STORE_FAST | 3,303,670 | 0.9% | 45.0% |
| RETURN_VALUE TO_BOOL_BOOL | 3,259,439 | 0.8% | 45.8% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 3,074,294 | 0.8% | 46.6% |
| LOAD_FAST STORE_ATTR_SLOT | 2,977,316 | 0.8% | 47.4% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 2,968,654 | 0.8% | 48.2% |
| LOAD_FAST LOAD_CONST | 2,950,743 | 0.8% | 48.9% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 2,805,922 | 0.7% | 49.6% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 2,741,293 | 0.7% | 50.4% |
| POP_TOP RETURN_CONST | 2,721,380 | 0.7% | 51.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 2,710,876 | 0.7% | 51.8% |
| CACHE RESUME_CHECK | 2,663,872 | 0.7% | 52.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 2,634,740 | 0.7% | 53.1% |
| LOAD_CONST STORE_FAST | 2,348,029 | 0.6% | 53.7% |
| RESUME_CHECK NOP | 2,292,000 | 0.6% | 54.3% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 2,263,414 | 0.6% | 54.9% |
| CALL STORE_FAST | 2,026,964 | 0.5% | 55.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 2,017,903 | 0.5% | 56.0% |
| LOAD_ATTR_MODULE PUSH_NULL | 2,014,123 | 0.5% | 56.5% |
| POP_TOP LOAD_CONST | 2,002,861 | 0.5% | 57.0% |
| LOAD_GLOBAL_MODULE BINARY_OP | 1,998,379 | 0.5% | 57.5% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 1,975,715 | 0.5% | 58.0% |
| POP_JUMP_IF_NONE LOAD_FAST | 1,964,511 | 0.5% | 58.5% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_WITH_VALUES | 1,962,866 | 0.5% | 59.0% |
| LOAD_CONST COMPARE_OP_INT | 1,955,004 | 0.5% | 59.5% |
| LOAD_ATTR_SLOT TO_BOOL_BOOL | 1,777,166 | 0.5% | 60.0% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 1,770,728 | 0.5% | 60.5% |
| TO_BOOL POP_JUMP_IF_TRUE | 1,709,089 | 0.4% | 60.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 1,684,054 | 0.4% | 61.3% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 1,682,845 | 0.4% | 61.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 1,675,129 | 0.4% | 62.2% |
| COPY TO_BOOL_INT | 1,669,741 | 0.4% | 62.6% |
| STORE_ATTR_SLOT LOAD_CONST | 1,645,777 | 0.4% | 63.1% |
| JUMP_FORWARD LOAD_FAST | 1,642,848 | 0.4% | 63.5% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,634,766 | 0.4% | 63.9% |
| STORE_FAST JUMP_FORWARD | 1,634,308 | 0.4% | 64.3% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LEN | 1,593,896 | 0.4% | 64.7% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST_LOAD_FAST | 1,403,209 | 0.4% | 65.1% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 1,395,220 | 0.4% | 65.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,394,980 | 0.4% | 65.8% |
| LOAD_ATTR LOAD_FAST | 1,370,021 | 0.4% | 66.2% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,369,610 | 0.4% | 66.5% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 1,366,543 | 0.4% | 66.9% |
| POP_JUMP_IF_FALSE POP_TOP | 1,358,294 | 0.4% | 67.2% |
| BINARY_OP COPY | 1,357,761 | 0.4% | 67.6% |
| STORE_FAST RETURN_CONST | 1,345,109 | 0.3% | 67.9% |
| POP_JUMP_IF_FALSE LOAD_CONST | 1,340,446 | 0.3% | 68.3% |
| CALL RETURN_VALUE | 1,336,191 | 0.3% | 68.6% |
| RETURN_VALUE RETURN_VALUE | 1,314,968 | 0.3% | 69.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 1,314,888 | 0.3% | 69.3% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 1,314,168 | 0.3% | 69.7% |
| LOAD_FAST STORE_FAST | 1,313,488 | 0.3% | 70.0% |
| NOP LOAD_GLOBAL_MODULE | 1,313,428 | 0.3% | 70.3% |
| LOAD_FAST POP_JUMP_IF_NONE | 1,308,928 | 0.3% | 70.7% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 1,307,032 | 0.3% | 71.0% |
| RETURN_VALUE INTERPRETER_EXIT | 1,300,756 | 0.3% | 71.3% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 1,298,918 | 0.3% | 71.7% |
| LOAD_FAST TO_BOOL | 1,298,015 | 0.3% | 72.0% |
| TO_BOOL_BOOL UNARY_NOT | 1,280,020 | 0.3% | 72.3% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 1,094,017 | 0.3% | 72.6% |
| BINARY_OP TO_BOOL_INT | 1,066,946 | 0.3% | 72.9% |
| PUSH_NULL LOAD_FAST | 1,057,799 | 0.3% | 73.2% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 1,048,189 | 0.3% | 73.4% |
| BINARY_OP STORE_FAST | 1,038,114 | 0.3% | 73.7% |
| RETURN_CONST INTERPRETER_EXIT | 1,036,358 | 0.3% | 74.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 1,032,247 | 0.3% | 74.3% |
| CALL_FUNCTION_EX POP_TOP | 1,023,911 | 0.3% | 74.5% |
| RETURN_VALUE LOAD_FAST | 1,015,091 | 0.3% | 74.8% |
| TO_BOOL_INT POP_JUMP_IF_TRUE | 1,013,840 | 0.3% | 75.0% |
| ENTER_EXECUTOR FOR_ITER_LIST | 1,013,431 | 0.3% | 75.3% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 995,559 | 0.3% | 75.6% |
| STORE_ATTR_SLOT LOAD_FAST | 987,532 | 0.3% | 75.8% |
| STORE_ATTR_SLOT RETURN_CONST | 987,532 | 0.3% | 76.1% |
| GET_AWAITABLE LOAD_CONST | 987,034 | 0.3% | 76.3% |
| POP_JUMP_IF_TRUE LOAD_CONST | 984,407 | 0.3% | 76.6% |
| YIELD_VALUE YIELD_VALUE | 978,714 | 0.3% | 76.8% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 978,374 | 0.3% | 77.1% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,318 | 85.7% |
| LOAD_CONST | 53,355 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 320,358 | 85.7% |
| CALL_METHOD_DESCRIPTOR_O | 44,928 | 12.0% |
| STORE_FAST | 7,907 | 2.1% |
| LIST_EXTEND | 240 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 200 | 0.1% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,663,872 | 99.9% |
| COPY_FREE_VARS | 1,000 | 0.0% |
| RESUME | 640 | 0.0% |
| POP_TOP | 400 | 0.0% |
| RETURN_GENERATOR | 320 | 0.0% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 80 | 100.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 40 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 50.0% |
| RETURN_VALUE | 40 | 25.0% |
| LOAD_CONST | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 60 | 37.5% |
| PUSH_EXC_INFO | 40 | 25.0% |
| STORE_FAST | 20 | 12.5% |
| UNPACK_SEQUENCE | 20 | 12.5% |
| BINARY_SUBSCR_LIST_INT | 20 | 12.5% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 460 | 69.7% |
| BUILD_TUPLE | 160 | 24.2% |
| LOAD_GLOBAL | 40 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 660 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 320,318 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,318 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 336,878 | 34.1% |
| SEND | 328,798 | 33.3% |
| RETURN_VALUE | 321,358 | 32.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 665,836 | 67.5% |
| STORE_FAST | 320,798 | 32.5% |
| UNPACK_SEQUENCE | 120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 120 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 440 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 954,438 | 59.5% |
| CALL_BUILTIN_CLASS | 641,438 | 40.0% |
| LOAD_ATTR_INSTANCE_VALUE | 8,040 | 0.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 160 | 0.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 954,058 | 59.5% |
| FOR_ITER_RANGE | 641,378 | 40.0% |
| FOR_ITER | 8,600 | 0.5% |
| EXTENDED_ARG | 80 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,300,756 | 48.8% |
| RETURN_CONST | 1,036,358 | 38.9% |
| YIELD_VALUE | 328,958 | 12.3% |
| RETURN_GENERATOR | 400 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 560 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,292,000 | 49.6% |
| STORE_FAST | 969,914 | 21.0% |
| POP_JUMP_IF_FALSE | 694,873 | 15.0% |
| POP_JUMP_IF_TRUE | 320,798 | 6.9% |
| STORE_ATTR_INSTANCE_VALUE | 320,298 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,308,695 | 71.6% |
| LOAD_GLOBAL_MODULE | 1,313,428 | 28.4% |
| LOAD_GLOBAL_BUILTIN | 320 | 0.0% |
| LOAD_GLOBAL | 280 | 0.0% |
| LOAD_DEREF | 160 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 420 | 63.6% |
| POP_TOP | 160 | 24.2% |
| COPY | 80 | 12.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 420 | 63.6% |
| POP_TOP | 80 | 12.1% |
| LOAD_CONST | 80 | 12.1% |
| RERAISE | 80 | 12.1% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 6,388,999 | 49.7% |
| POP_JUMP_IF_FALSE | 1,358,294 | 10.6% |
| CALL_METHOD_DESCRIPTOR_O | 1,094,017 | 8.5% |
| CALL_FUNCTION_EX | 1,023,911 | 8.0% |
| END_SEND | 665,836 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,334,585 | 41.5% |
| RETURN_CONST | 2,721,380 | 21.2% |
| LOAD_CONST | 2,002,861 | 15.6% |
| ENTER_EXECUTOR | 771,346 | 6.0% |
| LOAD_GLOBAL_MODULE | 702,380 | 5.5% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 380 | 57.6% |
| RERAISE | 80 | 12.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 80 | 12.1% |
| CALL_METHOD_DESCRIPTOR_O | 60 | 9.1% |
| BINARY_SUBSCR | 40 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 520 | 78.8% |
| LOAD_GLOBAL | 140 | 21.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 2,014,123 | 66.5% |
| LOAD_ATTR | 963,138 | 31.8% |
| LOAD_DEREF | 47,522 | 1.6% |
| LOAD_FAST | 2,100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,057,799 | 34.9% |
| LOAD_FAST_LOAD_FAST | 995,559 | 32.9% |
| CALL | 972,725 | 32.1% |
| LOAD_CONST | 480 | 0.0% |
| CALL_PY_EXACT_ARGS | 160 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 337,258 | 51.2% |
| ENTER_EXECUTOR | 319,918 | 48.6% |
| CALL_KW | 400 | 0.1% |
| CACHE | 320 | 0.0% |
| CALL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 657,836 | 99.9% |
| INTERPRETER_EXIT | 400 | 0.1% |
| STORE_FAST | 160 | 0.0% |
| CALL | 120 | 0.0% |
| LIST_APPEND | 80 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,593,629 | 36.6% |
| LOAD_ATTR_INSTANCE_VALUE | 3,613,731 | 28.8% |
| CALL | 1,336,191 | 10.6% |
| RETURN_VALUE | 1,314,968 | 10.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 656,814 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,303,670 | 26.3% |
| TO_BOOL_BOOL | 3,259,439 | 26.0% |
| RETURN_VALUE | 1,314,968 | 10.5% |
| INTERPRETER_EXIT | 1,300,756 | 10.4% |
| LOAD_FAST | 1,015,091 | 8.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 140 | 28.0% |
| LOAD_CONST | 120 | 24.0% |
| LOAD_ATTR | 100 | 20.0% |
| LOAD_FAST | 100 | 20.0% |
| STORE_SUBSCR | 40 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 180 | 36.0% |
| STORE_SUBSCR_DICT | 140 | 28.0% |
| LOAD_FAST | 60 | 12.0% |
| STORE_SUBSCR | 40 | 8.0% |
| LOAD_CONST | 40 | 8.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,298,015 | 74.9% |
| LOAD_ATTR_INSTANCE_VALUE | 428,328 | 24.7% |
| TO_BOOL | 2,380 | 0.1% |
| LOAD_ATTR | 2,000 | 0.1% |
| RETURN_VALUE | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,709,089 | 98.6% |
| POP_JUMP_IF_FALSE | 19,434 | 1.1% |
| TO_BOOL | 2,380 | 0.1% |
| TO_BOOL_BOOL | 2,300 | 0.1% |
| TO_BOOL_INT | 400 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 328,187 | 50.6% |
| BINARY_OP | 320,320 | 49.4% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 648,547 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,280,020 | 100.0% |
| TO_BOOL | 80 | 0.0% |
| TO_BOOL_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 640,080 | 50.0% |
| RETURN_VALUE | 640,000 | 50.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,998,379 | 47.9% |
| LOAD_ATTR_MODULE | 754,593 | 18.1% |
| UNARY_INVERT | 648,547 | 15.6% |
| POP_JUMP_IF_FALSE | 381,182 | 9.1% |
| LOAD_ATTR | 373,573 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,357,761 | 32.6% |
| TO_BOOL_INT | 1,066,946 | 25.6% |
| STORE_FAST | 1,038,114 | 24.9% |
| BUILD_TUPLE | 373,433 | 9.0% |
| UNARY_INVERT | 320,320 | 7.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 641,438 | 50.3% |
| LOAD_FAST_LOAD_FAST | 320,080 | 25.1% |
| STORE_FAST | 312,420 | 24.5% |
| LOAD_FAST | 640 | 0.1% |
| STORE_ATTR_INSTANCE_VALUE | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 962,098 | 75.4% |
| STORE_FAST | 312,900 | 24.5% |
| RETURN_VALUE | 240 | 0.0% |
| STORE_DEREF | 160 | 0.0% |
| SWAP | 80 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 240 | 30.0% |
| STORE_ATTR_INSTANCE_VALUE | 140 | 17.5% |
| POP_TOP | 80 | 10.0% |
| LOAD_FAST | 80 | 10.0% |
| POP_JUMP_IF_NOT_NONE | 80 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 560 | 70.0% |
| STORE_FAST | 240 | 30.0% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 360 | 90.0% |
| LOAD_ATTR | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 400 | 100.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,318 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 320,318 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 373,433 | 36.2% |
| LOAD_CONST | 328,147 | 31.8% |
| LOAD_FAST | 321,040 | 31.1% |
| LOAD_FAST_LOAD_FAST | 8,707 | 0.8% |
| LOAD_GLOBAL_BUILTIN | 560 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 373,393 | 36.2% |
| CALL_PY_EXACT_ARGS | 335,974 | 32.5% |
| CALL | 320,600 | 31.1% |
| LOAD_CONST | 560 | 0.1% |
| RETURN_VALUE | 400 | 0.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 972,725 | 22.2% |
| LOAD_FAST_LOAD_FAST | 667,252 | 15.3% |
| LOAD_CONST | 658,405 | 15.1% |
| LOAD_ATTR_INSTANCE_VALUE | 649,623 | 14.9% |
| LOAD_ATTR | 324,420 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,026,964 | 46.4% |
| RETURN_VALUE | 1,336,191 | 30.6% |
| POP_TOP | 331,418 | 7.6% |
| RESUME_CHECK | 330,427 | 7.6% |
| LOAD_CONST | 320,438 | 7.3% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 961,778 | 93.9% |
| ENTER_EXECUTOR | 62,213 | 6.1% |
| DICT_MERGE | 240 | 0.0% |
| LOAD_FAST | 160 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,023,911 | 99.9% |
| RESUME_CHECK | 220 | 0.0% |
| GET_AWAITABLE | 160 | 0.0% |
| COPY_FREE_VARS | 80 | 0.0% |
| MAKE_CELL | 80 | 0.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 961,778 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 961,778 | 100.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 346,932 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 328,878 | 94.8% |
| COPY_FREE_VARS | 15,814 | 4.6% |
| STORE_FAST | 800 | 0.2% |
| RESUME_CHECK | 420 | 0.1% |
| RETURN_GENERATOR | 400 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 16,054 | 84.1% |
| LOAD_CONST | 1,020 | 5.3% |
| LOAD_ATTR_MODULE | 940 | 4.9% |
| COMPARE_OP | 540 | 2.8% |
| CALL_BUILTIN_CLASS | 140 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 17,774 | 93.1% |
| COMPARE_OP | 540 | 2.8% |
| COMPARE_OP_INT | 520 | 2.7% |
| POP_JUMP_IF_TRUE | 140 | 0.7% |
| COMPARE_OP_STR | 60 | 0.3% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 320,360 | 99.6% |
| BUILD_SET | 400 | 0.1% |
| LOAD_FAST | 240 | 0.1% |
| LOAD_GLOBAL_MODULE | 220 | 0.1% |
| LOAD_ATTR_SLOT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 321,280 | 99.9% |
| POP_JUMP_IF_TRUE | 240 | 0.1% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,357,761 | 58.7% |
| UNARY_NOT | 640,080 | 27.7% |
| CALL_LEN | 312,240 | 13.5% |
| LOAD_FAST | 480 | 0.0% |
| CALL_BUILTIN_FAST | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 1,669,741 | 72.2% |
| TO_BOOL_BOOL | 640,280 | 27.7% |
| TO_BOOL | 480 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 280 | 0.0% |
| LOAD_ATTR | 200 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 657,734 | 95.1% |
| CALL_KW | 15,814 | 2.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 15,794 | 2.3% |
| CACHE | 1,000 | 0.1% |
| LOAD_ATTR_PROPERTY | 580 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 690,862 | 99.9% |
| RESUME | 600 | 0.1% |
| RETURN_GENERATOR | 80 | 0.0% |
| MAKE_CELL | 80 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 240 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 771,346 | 31.8% |
| POP_JUMP_IF_FALSE | 640,878 | 26.4% |
| CALL_LIST_APPEND | 373,093 | 15.4% |
| POP_JUMP_IF_TRUE | 320,058 | 13.2% |
| STORE_FAST | 319,898 | 13.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,013,431 | 41.8% |
| FOR_ITER_RANGE | 641,158 | 26.4% |
| RETURN_GENERATOR | 319,918 | 13.2% |
| POP_JUMP_IF_TRUE | 311,953 | 12.9% |
| CALL_FUNCTION_EX | 62,213 | 2.6% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 80 | 33.3% |
| POP_TOP | 80 | 33.3% |
| JUMP_BACKWARD | 80 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 160 | 66.7% |
| JUMP_BACKWARD | 80 | 33.3% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,600 | 90.1% |
| JUMP_BACKWARD | 500 | 5.2% |
| FOR_ITER | 260 | 2.7% |
| EXTENDED_ARG | 160 | 1.7% |
| SWAP | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,300 | 87.0% |
| RETURN_CONST | 460 | 4.8% |
| FOR_ITER | 260 | 2.7% |
| FOR_ITER_LIST | 240 | 2.5% |
| LOAD_FAST | 100 | 1.0% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 657,836 | 66.6% |
| LOAD_ATTR_INSTANCE_VALUE | 320,298 | 32.5% |
| LOAD_FAST | 8,240 | 0.8% |
| RETURN_VALUE | 240 | 0.0% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 987,034 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 20 | 100.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 100 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 80.0% |
| IMPORT_FROM | 20 | 20.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 720 | 52.9% |
| LOAD_CONST | 560 | 41.2% |
| LOAD_FAST_LOAD_FAST | 80 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 800 | 58.8% |
| RETURN_VALUE | 400 | 29.4% |
| LOAD_DEREF | 160 | 11.8% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,740 | 49.0% |
| POP_JUMP_IF_FALSE | 533 | 15.0% |
| CALL_LIST_APPEND | 440 | 12.4% |
| POP_JUMP_IF_TRUE | 340 | 9.6% |
| STORE_FAST | 340 | 9.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,260 | 35.5% |
| LOAD_FAST | 753 | 21.2% |
| FOR_ITER_RANGE | 740 | 20.8% |
| FOR_ITER | 500 | 14.1% |
| ENTER_EXECUTOR | 160 | 4.5% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,307,032 | 100.0% |
| RESUME | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 978,374 | 74.8% |
| SEND | 329,138 | 25.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,634,308 | 83.6% |
| POP_TOP | 320,840 | 16.4% |
| STORE_ATTR | 180 | 0.0% |
| CALL_LIST_APPEND | 140 | 0.0% |
| STORE_ATTR_INSTANCE_VALUE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,642,848 | 84.0% |
| LOAD_GLOBAL_BUILTIN | 312,460 | 16.0% |
| LOAD_GLOBAL | 160 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| NOP | 80 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 80 | 100.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 641,438 | 66.7% |
| LOAD_FAST | 320,080 | 33.3% |
| BINARY_SLICE | 240 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 961,778 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,509,632 | 81.7% |
| LOAD_ATTR_SLOT | 961,878 | 17.4% |
| LOAD_FAST_LOAD_FAST | 32,248 | 0.6% |
| LOAD_ATTR | 9,860 | 0.2% |
| LOAD_GLOBAL_MODULE | 2,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,370,021 | 24.8% |
| PUSH_NULL | 963,138 | 17.4% |
| SWAP | 709,447 | 12.8% |
| LOAD_ATTR_METHOD_NO_DICT | 374,953 | 6.8% |
| BINARY_OP | 373,573 | 6.8% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,950,743 | 22.9% |
| POP_TOP | 2,002,861 | 15.5% |
| STORE_ATTR_SLOT | 1,645,777 | 12.8% |
| POP_JUMP_IF_FALSE | 1,340,446 | 10.4% |
| GET_AWAITABLE | 987,034 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,883,926 | 45.7% |
| STORE_FAST | 2,348,029 | 18.2% |
| COMPARE_OP_INT | 1,955,004 | 15.2% |
| CALL | 658,405 | 5.1% |
| SEND_GEN | 657,656 | 5.1% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 643,160 | 88.4% |
| LOAD_ATTR | 31,668 | 4.4% |
| STORE_FAST | 16,294 | 2.2% |
| RESUME_CHECK | 16,114 | 2.2% |
| CALL_LEN | 15,794 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 659,674 | 90.7% |
| PUSH_NULL | 47,522 | 6.5% |
| COMPARE_OP_INT | 15,814 | 2.2% |
| LOAD_ATTR | 760 | 0.1% |
| LOAD_CONST | 560 | 0.1% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 13,256,946 | 16.1% |
| STORE_FAST | 9,886,676 | 12.0% |
| POP_JUMP_IF_FALSE | 9,112,308 | 11.0% |
| LOAD_CONST | 5,883,926 | 7.1% |
| POP_TOP | 5,334,585 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 26,050,843 | 31.6% |
| LOAD_ATTR_SLOT | 6,698,997 | 8.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,429,585 | 7.8% |
| CALL_PY_EXACT_ARGS | 5,940,136 | 7.2% |
| RETURN_VALUE | 4,593,629 | 5.6% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 80 | 100.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 20 | 100.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,975,715 | 25.4% |
| LOAD_ATTR_METHOD_NO_DICT | 1,403,209 | 18.1% |
| PUSH_NULL | 995,559 | 12.8% |
| LOAD_FAST_LOAD_FAST | 652,638 | 8.4% |
| LOAD_GLOBAL_MODULE | 641,860 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 2,634,740 | 33.9% |
| LOAD_FAST | 1,682,845 | 21.7% |
| CALL | 667,252 | 8.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 656,774 | 8.5% |
| LOAD_FAST_LOAD_FAST | 652,638 | 8.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,420 | 14.8% |
| POP_TOP | 940 | 9.8% |
| RESUME | 920 | 9.6% |
| RESUME_CHECK | 900 | 9.4% |
| STORE_FAST | 840 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,080 | 32.0% |
| LOAD_ATTR | 1,900 | 19.8% |
| LOAD_GLOBAL_BUILTIN | 1,660 | 17.3% |
| LOAD_FAST | 800 | 8.3% |
| LOAD_DEREF | 520 | 5.4% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 900 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 400 | 44.4% |
| LOAD_FAST | 200 | 22.2% |
| CALL | 140 | 15.6% |
| LOAD_FAST_LOAD_FAST | 80 | 8.9% |
| LOAD_GLOBAL | 40 | 4.4% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 880 | 61.1% |
| CACHE | 240 | 16.7% |
| CALL_KW | 160 | 11.1% |
| CALL_FUNCTION_EX | 80 | 5.6% |
| COPY_FREE_VARS | 80 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 880 | 61.1% |
| RESUME_CHECK | 260 | 18.1% |
| RETURN_GENERATOR | 240 | 16.7% |
| RESUME | 60 | 4.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 8,925,412 | 54.1% |
| TO_BOOL_INT | 2,805,922 | 17.0% |
| COMPARE_OP_INT | 2,741,293 | 16.6% |
| TO_BOOL_LIST | 954,458 | 5.8% |
| TO_BOOL_NONE | 662,356 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,112,308 | 55.2% |
| RETURN_CONST | 1,369,610 | 8.3% |
| POP_TOP | 1,358,294 | 8.2% |
| LOAD_CONST | 1,340,446 | 8.1% |
| LOAD_GLOBAL_BUILTIN | 961,378 | 5.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,308,928 | 57.2% |
| LOAD_ATTR_INSTANCE_VALUE | 977,941 | 42.7% |
| LOAD_ATTR | 440 | 0.0% |
| CALL | 160 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,964,511 | 85.9% |
| LOAD_CONST | 320,478 | 14.0% |
| RETURN_CONST | 1,280 | 0.1% |
| LOAD_FAST_LOAD_FAST | 400 | 0.0% |
| LOAD_GLOBAL | 260 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,684,054 | 84.0% |
| LOAD_ATTR_INSTANCE_VALUE | 321,198 | 16.0% |
| LOAD_GLOBAL_MODULE | 220 | 0.0% |
| LOAD_ATTR | 100 | 0.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,032,247 | 51.5% |
| LOAD_FAST_LOAD_FAST | 330,238 | 16.5% |
| LOAD_GLOBAL_MODULE | 329,747 | 16.4% |
| LOAD_CONST | 312,180 | 15.6% |
| LOAD_GLOBAL | 400 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,968,654 | 49.4% |
| TO_BOOL | 1,709,089 | 28.5% |
| TO_BOOL_INT | 1,013,840 | 16.9% |
| ENTER_EXECUTOR | 311,953 | 5.2% |
| COMPARE_OP_INT | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,700,107 | 61.6% |
| LOAD_CONST | 984,407 | 16.4% |
| NOP | 320,798 | 5.3% |
| LOAD_GLOBAL_BUILTIN | 320,298 | 5.3% |
| ENTER_EXECUTOR | 320,058 | 5.3% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 80 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 80 | 100.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,721,380 | 35.1% |
| POP_JUMP_IF_FALSE | 1,369,610 | 17.6% |
| STORE_FAST | 1,345,109 | 17.3% |
| STORE_ATTR_SLOT | 987,532 | 12.7% |
| STORE_ATTR_INSTANCE_VALUE | 641,858 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,388,999 | 82.3% |
| INTERPRETER_EXIT | 1,036,358 | 13.3% |
| END_SEND | 336,878 | 4.3% |
| EXIT_INIT_CHECK | 440 | 0.0% |
| RETURN_VALUE | 240 | 0.0% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 329,378 | 50.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 329,138 | 49.9% |
| SEND | 720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 328,798 | 49.9% |
| YIELD_VALUE | 328,798 | 49.9% |
| SEND | 720 | 0.1% |
| POP_TOP | 460 | 0.1% |
| SEND_GEN | 460 | 0.1% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 480 | 85.7% |
| LOAD_FAST_LOAD_FAST | 80 | 14.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,980 | 66.4% |
| LOAD_FAST_LOAD_FAST | 1,540 | 20.5% |
| LOAD_ATTR_INSTANCE_VALUE | 280 | 3.7% |
| STORE_ATTR | 260 | 3.5% |
| LOAD_DEREF | 200 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 2,660 | 35.5% |
| LOAD_FAST | 1,200 | 16.0% |
| LOAD_CONST | 1,140 | 15.2% |
| RETURN_CONST | 780 | 10.4% |
| STORE_ATTR_SLOT | 460 | 6.1% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 320 | 36.4% |
| BUILD_LIST | 160 | 18.2% |
| CALL_KW | 160 | 18.2% |
| BINARY_OP_ADD_INT | 120 | 13.6% |
| CALL | 80 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 54.5% |
| LOAD_CONST | 160 | 18.2% |
| BUILD_LIST | 80 | 9.1% |
| LOAD_DEREF | 80 | 9.1% |
| LOAD_FAST_LOAD_FAST | 80 | 9.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,303,670 | 20.2% |
| LOAD_CONST | 2,348,029 | 14.4% |
| CALL | 2,026,964 | 12.4% |
| LOAD_FAST | 1,313,488 | 8.0% |
| BINARY_OP | 1,038,114 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,886,676 | 60.5% |
| JUMP_FORWARD | 1,634,308 | 10.0% |
| RETURN_CONST | 1,345,109 | 8.2% |
| NOP | 969,914 | 5.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 709,287 | 4.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 20 | 100.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 1,395,220 | 100.0% |
| UNPACK_SEQUENCE | 260 | 0.0% |
| POP_TOP | 80 | 0.0% |
| COPY | 80 | 0.0% |
| STORE_FAST_STORE_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,394,980 | 99.9% |
| LOAD_GLOBAL_MODULE | 320 | 0.0% |
| LOAD_GLOBAL | 160 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |
| LOAD_CONST | 80 | 0.0% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 709,447 | 99.8% |
| LOAD_FAST | 400 | 0.1% |
| BINARY_OP_ADD_INT | 260 | 0.0% |
| BUILD_TUPLE | 240 | 0.0% |
| LOAD_FAST_LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 709,447 | 99.8% |
| POP_EXCEPT | 420 | 0.1% |
| STORE_ATTR_INSTANCE_VALUE | 280 | 0.0% |
| POP_TOP | 240 | 0.0% |
| STORE_ATTR | 200 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 160 | 23.5% |
| END_SEND | 120 | 17.6% |
| RETURN_VALUE | 80 | 11.8% |
| LOAD_FAST | 80 | 11.8% |
| FOR_ITER_LIST | 80 | 11.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 280 | 41.2% |
| STORE_FAST_STORE_FAST | 260 | 38.2% |
| UNPACK_SEQUENCE_TUPLE | 60 | 8.8% |
| STORE_FAST | 40 | 5.9% |
| POP_TOP | 20 | 2.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 978,714 | 74.8% |
| SEND | 328,798 | 25.1% |
| LOAD_CONST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 978,714 | 74.8% |
| INTERPRETER_EXIT | 328,958 | 25.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,080 | 47.9% |
| CACHE | 640 | 14.7% |
| COPY_FREE_VARS | 600 | 13.8% |
| POP_TOP | 480 | 11.1% |
| SEND_GEN | 400 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,220 | 51.2% |
| LOAD_GLOBAL | 920 | 21.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 480 | 11.1% |
| LOAD_CONST | 240 | 5.5% |
| NOP | 180 | 4.1% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 641,238 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 641,258 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 320,198 | 99.9% |
| LOAD_CONST | 280 | 0.1% |
| BINARY_OP | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320,218 | 99.9% |
| SWAP | 260 | 0.1% |
| STORE_DEREF | 120 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 320,198 | 100.0% |
| BINARY_OP | 40 | 0.0% |
| LOAD_CONST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 320,238 | 100.0% |
| COMPARE_OP | 40 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| BINARY_OP | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 7,960 | 98.3% |
| LOAD_CONST | 80 | 1.0% |
| BINARY_OP | 60 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,980 | 98.5% |
| SWAP | 120 | 1.5% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 15,854 | 93.5% |
| LOAD_FAST | 1,040 | 6.1% |
| BINARY_SUBSCR | 60 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 15,794 | 93.2% |
| RETURN_VALUE | 780 | 4.6% |
| PUSH_EXC_INFO | 380 | 2.2% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 80 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 66.7% |
| BINARY_SUBSCR | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TUPLE | 40 | 66.7% |
| UNPACK_SEQUENCE | 20 | 33.3% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 20 | 100.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 160 | 36.4% |
| CALL | 120 | 27.3% |
| LOAD_FAST | 80 | 18.2% |
| PUSH_NULL | 40 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 240 | 54.5% |
| COPY_FREE_VARS | 200 | 45.5% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 320,278 | 95.3% |
| CALL_BUILTIN_CLASS | 15,774 | 4.7% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 320,298 | 95.3% |
| COPY_FREE_VARS | 15,794 | 4.7% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 657,432 | 91.4% |
| LOAD_ATTR_INSTANCE_VALUE | 60,995 | 8.5% |
| CALL | 280 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 220 | 0.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 641,438 | 89.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60,835 | 8.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 15,774 | 2.2% |
| STORE_FAST | 500 | 0.1% |
| LOAD_FAST | 240 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 460 | 67.6% |
| LOAD_ATTR_SLOT | 120 | 17.6% |
| CALL | 80 | 11.8% |
| LOAD_FAST_LOAD_FAST | 20 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 280 | 41.2% |
| COPY | 220 | 32.4% |
| POP_TOP | 140 | 20.6% |
| TO_BOOL | 40 | 5.9% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 60,835 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60,855 | 100.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 50.0% |
| CALL | 80 | 33.3% |
| LOAD_CONST | 40 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 180 | 75.0% |
| CALL_BUILTIN_CLASS | 40 | 16.7% |
| CALL | 20 | 8.3% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,314,168 | 99.9% |
| BUILD_TUPLE | 400 | 0.0% |
| CALL | 260 | 0.0% |
| LOAD_ATTR_MODULE | 160 | 0.0% |
| LOAD_GLOBAL_MODULE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,314,888 | 100.0% |
| TO_BOOL | 260 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,593,896 | 80.4% |
| LOAD_FAST | 388,900 | 19.6% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 694,586 | 35.0% |
| LOAD_CONST | 320,218 | 16.1% |
| BINARY_OP_ADD_INT | 320,198 | 16.1% |
| LOAD_FAST | 319,900 | 16.1% |
| COPY | 312,240 | 15.7% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 373,393 | 99.9% |
| LOAD_FAST | 120 | 0.0% |
| LOAD_ATTR_MODULE | 120 | 0.0% |
| CALL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 373,093 | 99.8% |
| JUMP_BACKWARD | 440 | 0.1% |
| JUMP_FORWARD | 140 | 0.0% |
| LOAD_FAST | 60 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 656,774 | 50.9% |
| RETURN_VALUE | 320,280 | 24.8% |
| LOAD_FAST | 312,020 | 24.2% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 656,814 | 50.9% |
| STORE_FAST | 632,340 | 49.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 336,054 | 34.7% |
| LOAD_ATTR | 320,280 | 33.1% |
| LOAD_FAST_LOAD_FAST | 312,220 | 32.2% |
| CALL | 80 | 0.0% |
| LOAD_CONST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 656,394 | 67.8% |
| STORE_FAST | 312,240 | 32.2% |
| RETURN_VALUE | 80 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 695,486 | 67.8% |
| LOAD_ATTR | 329,038 | 32.1% |
| CALL | 740 | 0.1% |
| LOAD_FAST | 360 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 694,526 | 67.7% |
| TO_BOOL_BOOL | 328,998 | 32.1% |
| POP_TOP | 620 | 0.1% |
| LOAD_FAST | 460 | 0.0% |
| TO_BOOL | 320 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,048,189 | 95.8% |
| BINARY_SLICE | 44,928 | 4.1% |
| CALL | 720 | 0.1% |
| LOAD_CONST | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,094,017 | 100.0% |
| PUSH_EXC_INFO | 60 | 0.0% |
| LOAD_CONST | 20 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 7,040,735 | 47.1% |
| LOAD_FAST | 5,940,136 | 39.8% |
| LOAD_ATTR_METHOD_NO_DICT | 969,965 | 6.5% |
| BUILD_TUPLE | 335,974 | 2.2% |
| LOAD_ATTR_INSTANCE_VALUE | 328,147 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 13,947,143 | 93.3% |
| COPY_FREE_VARS | 657,734 | 4.4% |
| RETURN_GENERATOR | 337,258 | 2.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 656,814 | 99.8% |
| LOAD_ATTR_METHOD_NO_DICT | 360 | 0.1% |
| CALL | 240 | 0.0% |
| LOAD_CONST | 240 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 657,694 | 100.0% |
| RETURN_GENERATOR | 120 | 0.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 920 | 97.9% |
| CALL | 20 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 720 | 76.6% |
| LOAD_GLOBAL_MODULE | 200 | 21.3% |
| LOAD_GLOBAL | 20 | 2.1% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,955,004 | 71.3% |
| BINARY_OP_MULTIPLY_INT | 320,238 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 319,880 | 11.7% |
| LOAD_ATTR_SLOT | 60,795 | 2.2% |
| LOAD_FAST_LOAD_FAST | 52,928 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,741,293 | 100.0% |
| POP_JUMP_IF_TRUE | 260 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 140 | 70.0% |
| COMPARE_OP | 60 | 30.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 80 | 40.0% |
| COPY | 60 | 30.0% |
| STORE_FAST | 60 | 30.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,013,431 | 51.5% |
| GET_ITER | 954,058 | 48.5% |
| JUMP_BACKWARD | 1,260 | 0.1% |
| FOR_ITER | 240 | 0.0% |
| SWAP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 685,293 | 34.8% |
| RETURN_CONST | 641,458 | 32.6% |
| LOAD_FAST | 641,258 | 32.6% |
| STORE_FAST | 660 | 0.0% |
| LOAD_DEREF | 140 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 641,378 | 50.0% |
| ENTER_EXECUTOR | 641,158 | 50.0% |
| JUMP_BACKWARD | 740 | 0.1% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 641,978 | 50.0% |
| LOAD_CONST | 641,278 | 50.0% |
| LOAD_FAST | 80 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 80 | 44.4% |
| JUMP_BACKWARD | 60 | 33.3% |
| ENTER_EXECUTOR | 20 | 11.1% |
| FOR_ITER | 20 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 44.4% |
| LOAD_GLOBAL | 40 | 22.2% |
| LOAD_GLOBAL_MODULE | 40 | 22.2% |
| LOAD_FAST | 20 | 11.1% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360 | 94.7% |
| LOAD_ATTR | 20 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 380 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,050,843 | 96.3% |
| LOAD_ATTR_INSTANCE_VALUE | 656,654 | 2.4% |
| LOAD_FAST_LOAD_FAST | 336,934 | 1.2% |
| LOAD_ATTR | 4,360 | 0.0% |
| LOAD_DEREF | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,834,001 | 21.6% |
| LOAD_ATTR_METHOD_NO_DICT | 3,635,855 | 13.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,627,258 | 13.4% |
| RETURN_VALUE | 3,613,731 | 13.4% |
| CALL_LEN | 1,593,896 | 5.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,635,855 | 62.9% |
| LOAD_FAST | 1,770,728 | 30.6% |
| LOAD_ATTR | 374,953 | 6.5% |
| LOAD_ATTR_SLOT | 120 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,710,876 | 46.9% |
| LOAD_FAST_LOAD_FAST | 1,403,209 | 24.3% |
| CALL_PY_EXACT_ARGS | 969,965 | 16.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 695,486 | 12.0% |
| LOAD_GLOBAL_MODULE | 720 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,429,585 | 49.5% |
| LOAD_ATTR_INSTANCE_VALUE | 3,627,258 | 27.9% |
| LOAD_ATTR_SLOT | 1,962,866 | 15.1% |
| RETURN_VALUE | 656,734 | 5.1% |
| LOAD_FAST_LOAD_FAST | 320,280 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 7,040,735 | 54.2% |
| LOAD_FAST | 5,289,558 | 40.7% |
| LOAD_FAST_LOAD_FAST | 346,792 | 2.7% |
| LOAD_CONST | 320,558 | 2.5% |
| CALL | 1,700 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,419,403 | 99.9% |
| LOAD_ATTR | 1,900 | 0.1% |
| LOAD_FAST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,014,123 | 58.9% |
| BINARY_OP | 754,593 | 22.1% |
| UNARY_INVERT | 328,187 | 9.6% |
| LOAD_FAST | 320,420 | 9.4% |
| COMPARE_OP | 940 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 664,279 | 100.0% |
| LOAD_ATTR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 336,154 | 50.6% |
| CALL | 320,298 | 48.2% |
| BINARY_OP | 7,947 | 1.2% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,758 | 99.9% |
| LOAD_ATTR | 220 | 0.1% |
| LOAD_DEREF | 120 | 0.0% |
| LOAD_FAST_LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 320,558 | 99.8% |
| COPY_FREE_VARS | 580 | 0.2% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,698,997 | 99.9% |
| LOAD_FAST_LOAD_FAST | 7,960 | 0.1% |
| LOAD_ATTR | 840 | 0.0% |
| LOAD_ATTR_MODULE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 1,962,866 | 29.3% |
| TO_BOOL_BOOL | 1,777,166 | 26.5% |
| LOAD_ATTR | 961,878 | 14.3% |
| TO_BOOL_NONE | 660,556 | 9.8% |
| BUILD_LIST | 641,438 | 9.6% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,017,903 | 30.0% |
| LOAD_FAST | 1,634,766 | 24.3% |
| POP_JUMP_IF_FALSE | 961,378 | 14.3% |
| STORE_FAST | 702,573 | 10.5% |
| LOAD_GLOBAL_BUILTIN | 442,828 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,314,768 | 64.2% |
| CALL_ISINSTANCE | 1,314,168 | 19.6% |
| LOAD_DEREF | 643,160 | 9.6% |
| LOAD_GLOBAL_BUILTIN | 442,828 | 6.6% |
| BUILD_TUPLE | 560 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,074,294 | 39.4% |
| RESUME_CHECK | 1,675,129 | 21.5% |
| NOP | 1,313,428 | 16.8% |
| POP_TOP | 702,380 | 9.0% |
| POP_JUMP_IF_NOT_NONE | 329,747 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 3,419,403 | 43.8% |
| BINARY_OP | 1,998,379 | 25.6% |
| LOAD_FAST | 1,366,543 | 17.5% |
| LOAD_FAST_LOAD_FAST | 641,860 | 8.2% |
| LOAD_GLOBAL_MODULE | 320,280 | 4.1% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 94.1% |
| LOAD_SUPER_ATTR | 40 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 640 | 94.1% |
| LOAD_GLOBAL | 40 | 5.9% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 642,080 | 99.9% |
| LOAD_SUPER_ATTR | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,320 | 50.0% |
| LOAD_FAST_LOAD_FAST | 320,720 | 49.9% |
| CALL_PY_EXACT_ARGS | 320 | 0.0% |
| CALL | 120 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 13,947,143 | 67.8% |
| CACHE | 2,663,872 | 13.0% |
| SEND_GEN | 978,314 | 4.8% |
| COPY_FREE_VARS | 690,862 | 3.4% |
| POP_TOP | 658,156 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,256,946 | 64.5% |
| NOP | 2,292,000 | 11.1% |
| LOAD_GLOBAL_BUILTIN | 2,017,903 | 9.8% |
| LOAD_GLOBAL_MODULE | 1,675,129 | 8.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 1,307,032 | 6.4% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 978,374 | 59.8% |
| LOAD_CONST | 657,656 | 40.2% |
| SEND | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 978,314 | 59.8% |
| POP_TOP | 657,776 | 40.2% |
| RESUME | 400 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,263,414 | 99.8% |
| STORE_ATTR | 2,660 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,900 | 0.1% |
| LOAD_DEREF | 360 | 0.0% |
| SWAP | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,298,918 | 57.3% |
| RETURN_CONST | 641,858 | 28.3% |
| NOP | 320,298 | 14.1% |
| LOAD_CONST | 4,160 | 0.2% |
| LOAD_FAST_LOAD_FAST | 780 | 0.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,977,316 | 53.0% |
| LOAD_FAST_LOAD_FAST | 2,634,740 | 46.9% |
| STORE_ATTR | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,975,715 | 35.2% |
| LOAD_CONST | 1,645,777 | 29.3% |
| LOAD_FAST | 987,532 | 17.6% |
| RETURN_CONST | 987,532 | 17.6% |
| NOP | 15,960 | 0.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 336,054 | 99.8% |
| LOAD_CONST | 280 | 0.1% |
| LOAD_FAST | 160 | 0.0% |
| STORE_SUBSCR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 336,154 | 99.9% |
| NOP | 140 | 0.0% |
| LOAD_CONST | 140 | 0.0% |
| RETURN_CONST | 140 | 0.0% |
| LOAD_FAST_LOAD_FAST | 60 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,834,001 | 44.3% |
| RETURN_VALUE | 3,259,439 | 24.7% |
| LOAD_ATTR_SLOT | 1,777,166 | 13.5% |
| CALL_ISINSTANCE | 1,314,888 | 10.0% |
| COPY | 640,280 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,925,412 | 67.7% |
| POP_JUMP_IF_TRUE | 2,968,654 | 22.5% |
| UNARY_NOT | 1,280,020 | 9.7% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,669,741 | 43.7% |
| BINARY_OP | 1,066,946 | 27.9% |
| LOAD_FAST | 709,222 | 18.6% |
| LOAD_ATTR_INSTANCE_VALUE | 373,473 | 9.8% |
| TO_BOOL | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,805,922 | 73.5% |
| POP_JUMP_IF_TRUE | 1,013,840 | 26.5% |
| UNARY_NOT | 60 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 954,338 | 100.0% |
| TO_BOOL | 160 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 954,458 | 100.0% |
| POP_JUMP_IF_TRUE | 120 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 660,556 | 99.7% |
| LOAD_FAST | 1,240 | 0.2% |
| LOAD_ATTR | 360 | 0.1% |
| TO_BOOL | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 662,356 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 44.4% |
| UNPACK_SEQUENCE | 60 | 33.3% |
| BINARY_SUBSCR_LIST_INT | 40 | 22.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 60 | 33.3% |
| STORE_FAST | 60 | 33.3% |
| STORE_FAST_STORE_FAST | 60 | 33.3% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 709,287 | 50.8% |
| FOR_ITER_LIST | 685,293 | 49.1% |
| UNPACK_SEQUENCE | 280 | 0.0% |
| BINARY_SLICE | 200 | 0.0% |
| END_SEND | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,395,220 | 100.0% |
| LOAD_FAST | 60 | 0.0% |
| STORE_FAST | 60 | 0.0% |


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
|     deferred | 4,164,781 | 76.3% |
|          hit | 1,290,294 | 23.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 6.0% |
| Failure | 4,040 | 94.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 2,880 | 71.3% |
| or | 1,100 | 27.2% |
| floor divide | 40 | 1.0% |
| multiply different types | 20 | 0.5% |


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
|     deferred | 80 | 0.5% |
|          hit | 17,114 | 99.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,362,125 | 14.8% |
|          hit | 25,101,961 | 85.2% |
|         miss | 1,960 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,240 | 48.6% |
| Failure | 6,600 | 51.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class no vectorcall | 1,140 | 17.3% |
| cfunc noargs | 880 | 13.3% |
| code complex parameters | 780 | 11.8% |
| meth descr method fastcall keywords | 780 | 11.8% |
| no dict | 720 | 10.9% |
| meth descr varargs | 700 | 10.6% |
| cfunc varargs keywords | 460 | 7.0% |
| class mutable | 460 | 7.0% |
| other | 380 | 5.8% |
| cfunc varargs | 100 | 1.5% |
| operator wrapper | 100 | 1.5% |
| wrong number arguments | 40 | 0.6% |
| cmethod | 40 | 0.6% |
| init not simple | 20 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 17,974 | 0.7% |
|          hit | 2,741,753 | 99.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 580 | 51.8% |
| Failure | 540 | 48.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 220 | 40.7% |
| tuple | 160 | 29.6% |
| different types | 120 | 22.2% |
| bool | 40 | 7.4% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,960 | 0.3% |
|          hit | 3,252,565 | 99.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 320 | 55.2% |
| Failure | 260 | 44.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 140 | 53.8% |
| dict items | 80 | 30.8% |
| set | 40 | 15.4% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,501,398 | 8.8% |
|          hit | 56,946,927 | 91.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 12,080 | 60.7% |
| Failure | 7,820 | 39.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not managed dict | 3,620 | 46.3% |
| method | 1,540 | 19.7% |
| has managed dict | 1,480 | 18.9% |
| shadowed | 640 | 8.2% |
| metaclass attribute | 180 | 2.3% |
| class method obj | 160 | 2.0% |
| non object slot | 80 | 1.0% |
| class attr descriptor | 60 | 0.8% |
| class attr simple | 40 | 0.5% |
| builtin class method | 20 | 0.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,960 | 0.0% |
|        deopt | 80 | 0.0% |
|          hit | 14,523,204 | 99.9% |
|         miss | 80 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,740 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 460 | 0.1% |
|          hit | 643,160 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 440 | 100.0% |
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
|     deferred | 658,056 | 28.7% |
|          hit | 1,636,490 | 71.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 460 | 39.0% |
| Failure | 720 | 61.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 720 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,120 | 0.1% |
|          hit | 7,881,130 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,120 | 92.3% |
| Failure | 260 | 7.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 120 | 46.2% |
| overridden | 80 | 30.8% |
| overriding descriptor | 40 | 15.4% |
| no dict | 20 | 7.7% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 320 | 0.1% |
|          hit | 336,634 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 77.8% |
| Failure | 40 | 22.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 40 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,728,603 | 8.5% |
|          hit | 18,610,842 | 91.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,060 | 56.2% |
| Failure | 2,380 | 43.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytes | 840 | 35.3% |
| sequence | 560 | 23.5% |
| bytearray | 260 | 10.9% |
| mapping | 260 | 10.9% |
| dict | 180 | 7.6% |
| memory view | 140 | 5.9% |
| set | 100 | 4.2% |
| float | 20 | 0.8% |
| tuple | 20 | 0.8% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 340 | 0.0% |
|          hit | 1,395,520 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 340 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 188,595,596 | 48.7% |
| Not specialized | 43,687,049 | 11.3% |
| Specialized hits | 154,610,026 | 40.0% |
| Specialized misses | 2,060 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 5,501,398 | 33.4% |
| CALL | 4,362,125 | 26.5% |
| BINARY_OP | 4,164,781 | 25.3% |
| TO_BOOL | 1,728,603 | 10.5% |
| SEND | 658,056 | 4.0% |
| COMPARE_OP | 17,974 | 0.1% |
| FOR_ITER | 8,960 | 0.1% |
| LOAD_GLOBAL | 4,960 | 0.0% |
| STORE_ATTR | 4,120 | 0.0% |
| LOAD_SUPER_ATTR | 460 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,420 | 68.3% |
| CALL_METHOD_DESCRIPTOR_O | 480 | 23.1% |
| LOAD_GLOBAL_BUILTIN | 80 | 3.8% |
| CALL_BUILTIN_O | 60 | 2.9% |
| RESUME | 20 | 1.0% |
| RESUME_CHECK | 20 | 1.0% |
| CACHE | 0 | 0.0% |
| BEFORE_ASYNC_WITH | 0 | 0.0% |
| BEFORE_WITH | 0 | 0.0% |
| CHECK_EXC_MATCH | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,666,472 | 12.8% |
| Calls to Python functions inlined | 18,245,130 | 87.2% |
| Calls via PyEval_EvalFrame (total) | 2,666,472 | 12.8% |
| Calls via PyEval_EvalFrame (vector) | 2,337,114 | 11.2% |
| Calls via PyEval_EvalFrame (generator) | 329,358 | 1.6% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 2,337,114 | 11.2% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 400 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 1,400 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 659,436 | 3.2% |
| Frame objects created | 740 | 0.0% |
| Frames pushed | 17,625,366 | 84.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 9,611,380 | 43.1% |
| Frees to freelist | 9,628,174 |  |
| Allocations | 12,701,724 | 56.9% |
| Allocations to 512 bytes | 12,059,930 | 54.0% |
| Allocations to 4 kbytes | 600 | 0.0% |
| Allocations over 4 kbytes | 641,194 | 2.9% |
| Frees | 13,167,305 |  |
| New values | 700 |  |
| Interpreter increfs | 175,880,654 | 84.5% |
| Interpreter decrefs | 191,832,352 | 83.9% |
| Increfs | 32,322,926 | 15.5% |
| Decrefs | 36,733,505 | 16.1% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 6,248,183 |  |
| Method cache misses | 9,451 |  |
| Method cache collisions | 8,785 |  |
| Method cache dunder hits | 1,695,244 |  |
| Method cache dunder misses | 1,008 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 1,980 | 160,280 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 160 |  |
| Traces created | 160 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 12.5% |
| Traces executed | 2,425,433 |  |
| Uops executed | 72,466,559 | 29.88 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 20 | 12.5% |
| <= 64 | 20 | 12.5% |
| <= 128 | 80 | 50.0% |
| <= 256 | 20 | 12.5% |
| <= 512 | 20 | 12.5% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 40 | 25.0% |
| <= 64 | 60 | 37.5% |
| <= 128 | 40 | 25.0% |
| <= 256 | 20 | 12.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 753,366 | 31.1% |
| <= 4 | 641,158 | 26.4% |
| <= 8 | 0 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 320,218 | 13.2% |
| <= 64 | 311,860 | 12.9% |
| <= 128 | 337,578 | 13.9% |
| <= 256 | 61,253 | 2.5% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 8,014,571 | 11.1% | 11.1% |  |
| LOAD_FAST | 7,586,965 | 10.5% | 21.5% |  |
| _CHECK_VALIDITY | 7,304,240 | 10.1% | 31.6% |  |
| _GUARD_TYPE_VERSION | 5,477,502 | 7.6% | 39.2% |  |
| STORE_FAST | 3,572,729 | 4.9% | 44.1% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,401,192 | 4.7% | 48.8% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,401,192 | 4.7% | 53.5% |  |
| _GUARD_GLOBALS_VERSION | 2,022,585 | 2.8% | 56.3% |  |
| LOAD_CONST | 1,627,932 | 2.2% | 58.5% |  |
| _GUARD_IS_FALSE_POP | 1,429,162 | 2.0% | 60.5% | 0.0% |
| _GUARD_IS_TRUE_POP | 1,375,607 | 1.9% | 62.4% | 22.7% |
| _CHECK_PEP_523 | 1,367,227 | 1.9% | 64.3% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 1,367,227 | 1.9% | 66.2% |  |
| _CHECK_STACK_SPACE | 1,367,227 | 1.9% | 68.1% |  |
| _INIT_CALL_PY_EXACT_ARGS | 1,367,227 | 1.9% | 69.9% |  |
| _PUSH_FRAME | 1,367,227 | 1.9% | 71.8% |  |
| _SAVE_RETURN_OFFSET | 1,367,227 | 1.9% | 73.7% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 1,305,014 | 1.8% | 75.5% |  |
| _GUARD_KEYS_VERSION | 1,305,014 | 1.8% | 77.3% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 1,305,014 | 1.8% | 79.1% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 1,074,924 | 1.5% | 80.6% | 94.3% |
| _ITER_CHECK_LIST | 1,074,924 | 1.5% | 82.1% |  |
| RESUME_CHECK | 1,047,309 | 1.4% | 83.5% |  |
| _LOAD_GLOBAL_MODULE | 1,022,289 | 1.4% | 84.9% |  |
| _GUARD_BUILTINS_VERSION | 1,000,296 | 1.4% | 86.3% |  |
| _LOAD_GLOBAL_BUILTINS | 1,000,296 | 1.4% | 87.7% |  |
| CALL_LEN | 969,896 | 1.3% | 89.0% |  |
| COMPARE_OP_INT | 969,896 | 1.3% | 90.4% |  |
| _TO_BOOL | 717,451 | 1.0% | 91.4% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 711,031 | 1.0% | 92.3% | 90.2% |
| _ITER_CHECK_RANGE | 711,031 | 1.0% | 93.3% |  |
| TO_BOOL_LIST | 640,878 | 0.9% | 94.2% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 522,384 | 0.7% | 94.9% |  |
| _EXIT_TRACE | 450,891 | 0.6% | 95.6% | 100.0% |
| TO_BOOL_INT | 398,111 | 0.5% | 96.1% |  |
| BUILD_LIST | 391,231 | 0.5% | 96.6% |  |
| COPY | 390,391 | 0.5% | 97.2% |  |
| GET_ITER | 329,018 | 0.5% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 329,018 | 0.5% | 98.1% |  |
| _GUARD_IS_NOT_NONE_POP | 329,018 | 0.5% | 98.5% |  |
| _LOAD_ATTR_SLOT | 248,912 | 0.3% | 98.9% |  |
| TO_BOOL_BOOL | 139,686 | 0.2% | 99.1% |  |
| _LOAD_ATTR | 69,960 | 0.1% | 99.2% |  |
| _ITER_NEXT_RANGE | 69,873 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 62,273 | 0.1% | 99.4% |  |
| PUSH_NULL | 62,213 | 0.1% | 99.4% |  |
| CALL_INTRINSIC_1 | 62,213 | 0.1% | 99.5% |  |
| LIST_EXTEND | 62,213 | 0.1% | 99.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 61,613 | 0.1% | 99.7% |  |
| _ITER_NEXT_LIST | 61,493 | 0.1% | 99.8% |  |
| _BINARY_OP | 61,493 | 0.1% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 61,373 | 0.1% | 100.0% |  |
| _FOR_ITER_TIER_TWO | 7,680 | 0.0% | 100.0% | 100.0% |
| BUILD_TUPLE | 7,600 | 0.0% | 100.0% |  |
| CALL_ISINSTANCE | 7,600 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 7,600 | 0.0% | 100.0% |  |
| SWAP | 120 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 120 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 20 | 0.0% | 100.0% | 100.0% |
| _ITER_CHECK_TUPLE | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 40 |
| RETURN_GENERATOR | 20 |
| CALL_FUNCTION_EX | 20 |
| CALL_LIST_APPEND | 20 |


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2023-12-17
