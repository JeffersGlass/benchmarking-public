
# Pystats results

- benchmark: async_tree_memoization_tg
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 457,907,544 | 20.4% | 20.4% |  |
| LOAD_ATTR_INSTANCE_VALUE | 129,539,432 | 5.8% | 26.2% |  |
| POP_JUMP_IF_FALSE | 122,856,286 | 5.5% | 31.7% |  |
| RESUME_CHECK | 118,289,176 | 5.3% | 37.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 107,931,974 | 4.8% | 41.8% |  |
| LOAD_CONST | 101,151,946 | 4.5% | 46.3% |  |
| POP_TOP | 92,185,102 | 4.1% | 50.4% |  |
| STORE_FAST | 87,437,738 | 3.9% | 54.4% |  |
| STORE_ATTR_SLOT | 75,466,694 | 3.4% | 57.7% | 6.2% |
| TO_BOOL_BOOL | 70,517,468 | 3.1% | 60.9% | 0.0% |
| RETURN_VALUE | 69,027,188 | 3.1% | 64.0% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 63,077,776 | 2.8% | 66.8% |  |
| RETURN_CONST | 57,476,048 | 2.6% | 69.3% |  |
| INTERPRETER_EXIT | 51,855,320 | 2.3% | 71.7% |  |
| CALL_PY_EXACT_ARGS | 51,134,796 | 2.3% | 73.9% |  |
| LOAD_GLOBAL_MODULE | 49,619,176 | 2.2% | 76.1% |  |
| LOAD_ATTR_SLOT | 42,517,228 | 1.9% | 78.0% | 1.6% |
| CALL | 36,221,174 | 1.6% | 79.7% |  |
| LOAD_ATTR_METHOD_NO_DICT | 35,465,882 | 1.6% | 81.2% | 0.0% |
| PUSH_NULL | 33,664,468 | 1.5% | 82.8% |  |
| LOAD_ATTR | 33,240,760 | 1.5% | 84.2% |  |
| POP_JUMP_IF_NOT_NONE | 30,605,074 | 1.4% | 85.6% |  |
| CALL_METHOD_DESCRIPTOR_O | 27,992,894 | 1.2% | 86.9% | 0.0% |
| TO_BOOL_NONE | 25,751,560 | 1.1% | 88.0% | 0.0% |
| LOAD_ATTR_MODULE | 24,628,968 | 1.1% | 89.1% |  |
| COMPARE_OP_INT | 20,234,848 | 0.9% | 90.0% |  |
| CALL_BUILTIN_O | 16,124,634 | 0.7% | 90.7% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 13,811,974 | 0.6% | 91.3% | 0.0% |
| POP_JUMP_IF_NONE | 13,437,680 | 0.6% | 91.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 11,946,640 | 0.5% | 92.5% |  |
| TO_BOOL | 11,205,694 | 0.5% | 93.0% |  |
| CALL_FUNCTION_EX | 10,821,540 | 0.5% | 93.5% |  |
| ENTER_EXECUTOR | 10,629,408 | 0.5% | 93.9% |  |
| POP_JUMP_IF_TRUE | 10,453,408 | 0.5% | 94.4% |  |
| RETURN_GENERATOR | 10,449,160 | 0.5% | 94.9% |  |
| CALL_KW | 10,076,780 | 0.4% | 95.3% |  |
| BINARY_OP_SUBTRACT_INT | 8,211,380 | 0.4% | 95.7% |  |
| SEND_GEN | 7,833,600 | 0.3% | 96.0% |  |
| BINARY_OP_ADD_INT | 7,464,980 | 0.3% | 96.4% |  |
| END_SEND | 7,088,980 | 0.3% | 96.7% |  |
| GET_AWAITABLE | 7,088,980 | 0.3% | 97.0% |  |
| LOAD_GLOBAL_BUILTIN | 6,706,356 | 0.3% | 97.3% | 0.0% |
| TO_BOOL_LIST | 5,229,582 | 0.2% | 97.5% |  |
| FOR_ITER_RANGE | 5,229,268 | 0.2% | 97.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,493,320 | 0.2% | 98.0% | 16.9% |
| JUMP_FORWARD | 4,483,202 | 0.2% | 98.2% |  |
| JUMP_BACKWARD | 4,481,674 | 0.2% | 98.4% |  |
| COMPARE_OP_FLOAT | 4,459,288 | 0.2% | 98.6% |  |
| CALL_ISINSTANCE | 4,459,220 | 0.2% | 98.8% |  |
| CALL_PY_WITH_DEFAULTS | 4,105,120 | 0.2% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 3,362,160 | 0.2% | 99.1% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 2,982,320 | 0.1% | 99.2% |  |
| YIELD_VALUE | 2,982,320 | 0.1% | 99.4% |  |
| SEND | 2,238,780 | 0.1% | 99.5% |  |
| CALL_BUILTIN_CLASS | 1,495,454 | 0.1% | 99.5% |  |
| NOP | 1,123,174 | 0.1% | 99.6% |  |
| BUILD_LIST | 1,122,494 | 0.1% | 99.6% |  |
| GET_ITER | 752,242 | 0.0% | 99.7% |  |
| BEFORE_ASYNC_WITH | 746,480 | 0.0% | 99.7% |  |
| EXIT_INIT_CHECK | 746,460 | 0.0% | 99.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 746,460 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 746,460 | 0.0% | 99.8% |  |
| LOAD_DEREF | 745,820 | 0.0% | 99.8% |  |
| COPY_FREE_VARS | 745,660 | 0.0% | 99.9% |  |
| LOAD_SUPER_ATTR_METHOD | 745,180 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_FLOAT | 374,094 | 0.0% | 99.9% |  |
| CALL_INTRINSIC_1 | 373,940 | 0.0% | 99.9% |  |
| LIST_EXTEND | 373,940 | 0.0% | 99.9% |  |
| COMPARE_OP | 373,400 | 0.0% | 100.0% |  |
| BUILD_MAP | 372,700 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 372,520 | 0.0% | 100.0% |  |
| CALL_LEN | 5,442 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,620 | 0.0% | 100.0% |  |
| STORE_ATTR | 3,700 | 0.0% | 100.0% |  |
| FOR_ITER_LIST | 3,688 | 0.0% | 100.0% |  |
| COPY | 2,574 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 2,194 | 0.0% | 100.0% |  |
| RESUME | 2,040 | 0.0% | 100.0% | 1,511.5% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 2,014 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 1,840 | 0.0% | 100.0% |  |
| BINARY_OP | 1,154 | 0.0% | 100.0% |  |
| BUILD_TUPLE | 640 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 588 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 460 | 0.0% | 100.0% |  |
| FOR_ITER | 440 | 0.0% | 100.0% |  |
| IS_OP | 400 | 0.0% | 100.0% |  |
| SWAP | 340 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 240 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 240 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 180 | 0.0% | 100.0% |  |
| POP_EXCEPT | 180 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 180 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 180 | 0.0% | 100.0% |  |
| UNARY_INVERT | 160 | 0.0% | 100.0% |  |
| UNARY_NOT | 160 | 0.0% | 100.0% |  |
| CONTAINS_OP | 160 | 0.0% | 100.0% |  |
| STORE_FAST_STORE_FAST | 160 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 140 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 140 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 120 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 120 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 100 | 0.0% | 100.0% |  |
| IMPORT_NAME | 100 | 0.0% | 100.0% |  |
| DICT_MERGE | 80 | 0.0% | 100.0% |  |
| MAKE_CELL | 80 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 80 | 0.0% | 100.0% |  |
| RERAISE | 80 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 60 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 60 | 0.0% | 100.0% |  |
| BEFORE_WITH | 40 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 40 | 0.0% | 100.0% |  |
| IMPORT_FROM | 20 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 20 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 20 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 20 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 125,058,132 | 5.6% | 5.6% |
| RESUME_CHECK LOAD_FAST | 89,570,088 | 4.0% | 9.6% |
| POP_JUMP_IF_FALSE LOAD_FAST | 89,456,676 | 4.0% | 13.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 64,546,848 | 2.9% | 16.5% |
| STORE_FAST LOAD_FAST | 58,986,180 | 2.6% | 19.1% |
| CACHE RESUME_CHECK | 45,510,580 | 2.0% | 21.1% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 42,922,682 | 1.9% | 23.0% |
| LOAD_FAST LOAD_ATTR_SLOT | 42,502,974 | 1.9% | 24.9% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 42,178,216 | 1.9% | 26.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 42,168,420 | 1.9% | 28.7% |
| LOAD_CONST LOAD_FAST | 41,797,654 | 1.9% | 30.6% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 40,309,134 | 1.8% | 32.4% |
| POP_TOP LOAD_FAST | 39,936,568 | 1.8% | 34.2% |
| LOAD_FAST RETURN_VALUE | 37,891,374 | 1.7% | 35.8% |
| LOAD_FAST STORE_ATTR_SLOT | 33,209,454 | 1.5% | 37.3% |
| LOAD_FAST LOAD_ATTR | 31,731,080 | 1.4% | 38.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 31,359,122 | 1.4% | 40.1% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 31,349,468 | 1.4% | 41.5% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 31,347,180 | 1.4% | 42.9% |
| RETURN_CONST INTERPRETER_EXIT | 28,737,900 | 1.3% | 44.2% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 27,992,874 | 1.2% | 45.5% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 26,875,934 | 1.2% | 46.7% |
| RETURN_CONST POP_TOP | 26,872,668 | 1.2% | 47.9% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 25,751,540 | 1.1% | 49.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 24,627,868 | 1.1% | 50.1% |
| LOAD_ATTR_MODULE PUSH_NULL | 24,256,008 | 1.1% | 51.2% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 23,886,314 | 1.1% | 52.3% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 23,513,694 | 1.0% | 53.3% |
| STORE_ATTR_SLOT LOAD_CONST | 21,642,900 | 1.0% | 54.3% |
| LOAD_ATTR_SLOT TO_BOOL_NONE | 21,270,100 | 0.9% | 55.2% |
| RETURN_VALUE INTERPRETER_EXIT | 20,505,680 | 0.9% | 56.2% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 20,234,848 | 0.9% | 57.1% |
| CALL STORE_FAST | 20,152,320 | 0.9% | 58.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 19,407,254 | 0.9% | 58.8% |
| RETURN_VALUE STORE_FAST | 19,035,214 | 0.8% | 59.7% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 18,288,000 | 0.8% | 60.5% |
| LOAD_FAST LOAD_CONST | 17,916,294 | 0.8% | 61.3% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 16,419,540 | 0.7% | 62.0% |
| LOAD_FAST CALL_BUILTIN_O | 16,123,980 | 0.7% | 62.7% |
| POP_JUMP_IF_FALSE RETURN_CONST | 16,047,360 | 0.7% | 63.5% |
| CALL_BUILTIN_O STORE_FAST | 15,752,234 | 0.7% | 64.2% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 15,300,660 | 0.7% | 64.9% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 14,928,200 | 0.7% | 65.5% |
| POP_TOP RETURN_CONST | 14,554,940 | 0.6% | 66.2% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 14,186,108 | 0.6% | 66.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 13,439,308 | 0.6% | 67.4% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 12,690,400 | 0.6% | 68.0% |
| POP_JUMP_IF_NONE LOAD_FAST | 12,690,400 | 0.6% | 68.5% |
| LOAD_CONST COMPARE_OP_INT | 11,946,034 | 0.5% | 69.1% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 11,945,020 | 0.5% | 69.6% |
| POP_TOP LOAD_CONST | 11,570,354 | 0.5% | 70.1% |
| LOAD_CONST STORE_FAST | 11,204,730 | 0.5% | 70.6% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL | 11,199,394 | 0.5% | 71.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 11,197,900 | 0.5% | 71.6% |
| STORE_ATTR_SLOT LOAD_FAST | 11,194,294 | 0.5% | 72.1% |
| STORE_ATTR_SLOT RETURN_CONST | 11,193,840 | 0.5% | 72.6% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_WITH_VALUES | 11,193,640 | 0.5% | 73.1% |
| POP_JUMP_IF_FALSE LOAD_CONST | 10,827,168 | 0.5% | 73.6% |
| RETURN_VALUE TO_BOOL_BOOL | 10,821,860 | 0.5% | 74.1% |
| STORE_FAST RETURN_CONST | 10,450,834 | 0.5% | 74.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 10,449,480 | 0.5% | 75.0% |
| LOAD_FAST_LOAD_FAST CALL | 10,449,200 | 0.5% | 75.5% |
| CALL_FUNCTION_EX POP_TOP | 10,449,160 | 0.5% | 76.0% |
| POP_TOP RESUME_CHECK | 10,449,000 | 0.5% | 76.4% |
| POP_TOP ENTER_EXECUTOR | 10,448,660 | 0.5% | 76.9% |
| ENTER_EXECUTOR CALL_FUNCTION_EX | 10,447,340 | 0.5% | 77.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 10,076,960 | 0.4% | 77.8% |
| LOAD_CONST CALL_KW | 10,076,780 | 0.4% | 78.3% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST_LOAD_FAST | 10,076,700 | 0.4% | 78.7% |
| LOAD_ATTR CALL_METHOD_DESCRIPTOR_NOARGS | 10,076,500 | 0.4% | 79.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS TO_BOOL_BOOL | 10,076,460 | 0.4% | 79.6% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_MODULE | 9,330,500 | 0.4% | 80.0% |
| LOAD_FAST PUSH_NULL | 9,033,820 | 0.4% | 80.4% |
| LOAD_ATTR CALL | 8,959,720 | 0.4% | 80.8% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 8,659,540 | 0.4% | 81.2% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 8,583,660 | 0.4% | 81.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 8,565,414 | 0.4% | 82.0% |
| LOAD_FAST POP_JUMP_IF_NONE | 8,211,840 | 0.4% | 82.3% |
| PUSH_NULL LOAD_FAST | 7,539,134 | 0.3% | 82.7% |
| GET_AWAITABLE LOAD_CONST | 7,088,980 | 0.3% | 83.0% |
| TO_BOOL POP_JUMP_IF_FALSE | 6,719,500 | 0.3% | 83.3% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NOT_NONE | 6,718,340 | 0.3% | 83.6% |
| PUSH_NULL CALL | 6,345,514 | 0.3% | 83.9% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 5,972,054 | 0.3% | 84.1% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,970,560 | 0.3% | 84.4% |
| END_SEND POP_TOP | 5,970,200 | 0.3% | 84.7% |
| SEND_GEN POP_TOP | 5,970,060 | 0.3% | 84.9% |
| LOAD_CONST SEND_GEN | 5,969,960 | 0.3% | 85.2% |
| CALL POP_TOP | 5,598,460 | 0.2% | 85.5% |
| TO_BOOL_LIST POP_JUMP_IF_FALSE | 5,229,582 | 0.2% | 85.7% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_LIST | 5,229,482 | 0.2% | 85.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 5,227,394 | 0.2% | 86.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 5,226,060 | 0.2% | 86.4% |
| LOAD_CONST LOAD_CONST | 5,225,620 | 0.2% | 86.6% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NONE | 5,225,580 | 0.2% | 86.9% |
| LOAD_ATTR LOAD_FAST | 4,852,420 | 0.2% | 87.1% |
| CALL RESUME_CHECK | 4,851,840 | 0.2% | 87.3% |
| RETURN_VALUE END_SEND | 4,851,260 | 0.2% | 87.5% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 4,833,814 | 0.2% | 87.7% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 4,554,360 | 0.2% | 87.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 45,510,580 | 87.8% |
| POP_TOP | 4,478,960 | 8.6% |
| RETURN_GENERATOR | 1,492,960 | 2.9% |
| COPY_FREE_VARS | 372,480 | 0.7% |
| RESUME | 340 | 0.0% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 746,460 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 746,480 | 100.0% |


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
| LOAD_CONST | 80 | 66.7% |
| LOAD_FAST | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 40 | 33.3% |
| PUSH_EXC_INFO | 20 | 16.7% |
| LOAD_ATTR | 20 | 16.7% |
| STORE_FAST | 20 | 16.7% |
| BINARY_SUBSCR_DICT | 20 | 16.7% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 160 | 88.9% |
| LOAD_GLOBAL | 20 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 180 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,851,260 | 68.4% |
| RETURN_CONST | 1,118,940 | 15.8% |
| SEND | 1,118,780 | 15.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,970,200 | 84.2% |
| STORE_FAST | 746,480 | 10.5% |
| LOAD_FAST | 372,300 | 5.3% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 746,460 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 746,460 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 748,334 | 99.5% |
| LOAD_FAST | 3,688 | 0.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 160 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 748,274 | 99.5% |
| FOR_ITER_LIST | 3,628 | 0.5% |
| FOR_ITER | 320 | 0.0% |
| FOR_ITER_TUPLE | 20 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 28,737,900 | 55.4% |
| RETURN_VALUE | 20,505,680 | 39.5% |
| RETURN_GENERATOR | 1,492,960 | 2.9% |
| YIELD_VALUE | 1,118,780 | 2.2% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 240 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 746,460 | 66.5% |
| STORE_FAST | 374,294 | 33.3% |
| RESUME_CHECK | 1,660 | 0.1% |
| POP_TOP | 400 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,122,614 | 100.0% |
| LOAD_GLOBAL_MODULE | 320 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |
| LOAD_GLOBAL | 80 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 100 | 55.6% |
| COPY | 80 | 44.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 100 | 55.6% |
| RERAISE | 80 | 44.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 27,992,874 | 30.4% |
| RETURN_CONST | 26,872,668 | 29.2% |
| CALL_FUNCTION_EX | 10,449,160 | 11.3% |
| END_SEND | 5,970,200 | 6.5% |
| SEND_GEN | 5,970,060 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,936,568 | 43.3% |
| RETURN_CONST | 14,554,940 | 15.8% |
| LOAD_CONST | 11,570,354 | 12.6% |
| RESUME_CHECK | 10,449,000 | 11.3% |
| ENTER_EXECUTOR | 10,448,660 | 11.3% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RERAISE | 80 | 44.4% |
| BINARY_SUBSCR_DICT | 80 | 44.4% |
| BINARY_SUBSCR | 20 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 160 | 88.9% |
| LOAD_GLOBAL | 20 | 11.1% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 24,256,008 | 72.1% |
| LOAD_FAST | 9,033,820 | 26.8% |
| LOAD_ATTR | 374,560 | 1.1% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,928,200 | 44.3% |
| LOAD_FAST | 7,539,134 | 22.4% |
| CALL | 6,345,514 | 18.8% |
| LOAD_CONST | 3,732,720 | 11.1% |
| CALL_ALLOC_AND_ENTER_INIT | 746,440 | 2.2% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 8,583,660 | 82.1% |
| CACHE | 1,492,960 | 14.3% |
| CALL_PY_WITH_DEFAULTS | 372,280 | 3.6% |
| CALL | 120 | 0.0% |
| COPY_FREE_VARS | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 4,478,920 | 42.9% |
| GET_AWAITABLE | 4,477,240 | 42.8% |
| INTERPRETER_EXIT | 1,492,960 | 14.3% |
| CALL_PY_EXACT_ARGS | 40 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,891,374 | 54.9% |
| LOAD_ATTR_INSTANCE_VALUE | 16,419,540 | 23.8% |
| COMPARE_OP_FLOAT | 4,458,700 | 6.5% |
| RETURN_VALUE | 3,732,960 | 5.4% |
| BINARY_OP_ADD_INT | 3,732,460 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 20,505,680 | 29.7% |
| STORE_FAST | 19,035,214 | 27.6% |
| TO_BOOL_BOOL | 10,821,860 | 15.7% |
| END_SEND | 4,851,260 | 7.0% |
| POP_TOP | 4,479,120 | 6.5% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 60.0% |
| LOAD_ATTR | 40 | 40.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 40.0% |
| STORE_SUBSCR_DICT | 40 | 40.0% |
| LOAD_CONST | 20 | 20.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 11,199,394 | 99.9% |
| TO_BOOL | 3,800 | 0.0% |
| LOAD_ATTR | 760 | 0.0% |
| RETURN_VALUE | 480 | 0.0% |
| CALL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,719,500 | 60.0% |
| POP_JUMP_IF_TRUE | 4,480,974 | 40.0% |
| TO_BOOL | 3,800 | 0.0% |
| TO_BOOL_BOOL | 980 | 0.0% |
| TO_BOOL_INT | 160 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 80 | 50.0% |
| LOAD_ATTR_MODULE | 60 | 37.5% |
| LOAD_ATTR | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 160 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 60 | 37.5% |
| TO_BOOL_INT | 60 | 37.5% |
| TO_BOOL | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 80 | 50.0% |
| STORE_FAST | 80 | 50.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 234 | 20.3% |
| LOAD_GLOBAL_MODULE | 180 | 15.6% |
| UNARY_INVERT | 160 | 13.9% |
| BINARY_OP | 160 | 13.9% |
| LOAD_CONST | 160 | 13.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 220 | 19.1% |
| BINARY_OP | 160 | 13.9% |
| COPY | 160 | 13.9% |
| LOAD_GLOBAL_MODULE | 114 | 9.9% |
| UNARY_INVERT | 80 | 6.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 746,680 | 66.5% |
| LOAD_FAST | 372,300 | 33.2% |
| STORE_FAST | 1,834 | 0.2% |
| LOAD_ATTR_SLOT | 1,620 | 0.1% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,120,660 | 99.8% |
| STORE_FAST | 1,834 | 0.2% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 372,300 | 99.9% |
| STORE_ATTR_INSTANCE_VALUE | 140 | 0.0% |
| POP_TOP | 80 | 0.0% |
| BUILD_TUPLE | 80 | 0.0% |
| RESUME_CHECK | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 372,300 | 99.9% |
| LOAD_FAST | 400 | 0.1% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 37.5% |
| CALL | 80 | 12.5% |
| LOAD_CONST | 80 | 12.5% |
| LOAD_FAST_LOAD_FAST | 80 | 12.5% |
| LOAD_GLOBAL_MODULE | 80 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 240 | 37.5% |
| CALL | 160 | 25.0% |
| RETURN_VALUE | 80 | 12.5% |
| BUILD_MAP | 80 | 12.5% |
| CALL_ISINSTANCE | 40 | 6.2% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,449,200 | 28.8% |
| LOAD_ATTR | 8,959,720 | 24.7% |
| PUSH_NULL | 6,345,514 | 17.5% |
| LOAD_ATTR_INSTANCE_VALUE | 4,479,120 | 12.4% |
| RETURN_GENERATOR | 4,478,920 | 12.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 20,152,320 | 55.6% |
| POP_TOP | 5,598,460 | 15.5% |
| RESUME_CHECK | 4,851,840 | 13.4% |
| CALL_METHOD_DESCRIPTOR_O | 4,479,100 | 12.4% |
| LOAD_FAST | 747,200 | 2.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 10,447,340 | 96.5% |
| BUILD_MAP | 372,300 | 3.4% |
| CALL_INTRINSIC_1 | 1,640 | 0.0% |
| DICT_MERGE | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 10,449,160 | 96.6% |
| STORE_FAST | 372,300 | 3.4% |
| COPY_FREE_VARS | 80 | 0.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 373,940 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 372,300 | 99.6% |
| CALL_FUNCTION_EX | 1,640 | 0.4% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,076,780 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,478,960 | 44.4% |
| RESUME_CHECK | 4,478,940 | 44.4% |
| RETURN_VALUE | 1,118,780 | 11.1% |
| POP_TOP | 80 | 0.0% |
| RESUME | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 372,600 | 99.8% |
| COMPARE_OP | 320 | 0.1% |
| CALL_BUILTIN_CLASS | 140 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 372,760 | 99.8% |
| COMPARE_OP | 320 | 0.1% |
| COMPARE_OP_INT | 220 | 0.1% |
| COMPARE_OP_FLOAT | 60 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 60 | 37.5% |
| LOAD_GLOBAL_MODULE | 60 | 37.5% |
| LOAD_ATTR | 20 | 12.5% |
| LOAD_GLOBAL | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 160 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 1,814 | 70.5% |
| BINARY_OP | 160 | 6.2% |
| LOAD_FAST | 160 | 6.2% |
| CALL_BUILTIN_FAST | 140 | 5.4% |
| UNARY_NOT | 80 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 1,874 | 72.8% |
| TO_BOOL | 240 | 9.3% |
| TO_BOOL_BOOL | 200 | 7.8% |
| POP_EXCEPT | 80 | 3.1% |
| LOAD_ATTR | 80 | 3.1% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 372,920 | 50.0% |
| CACHE | 372,480 | 50.0% |
| CALL | 180 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 745,260 | 99.9% |
| RESUME | 240 | 0.0% |
| RETURN_GENERATOR | 80 | 0.0% |
| MAKE_CELL | 80 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 80 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 10,448,660 | 98.3% |
| POP_JUMP_IF_FALSE | 178,774 | 1.7% |
| LOAD_FAST | 1,674 | 0.0% |
| ENTER_EXECUTOR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 10,447,340 | 98.3% |
| RETURN_VALUE | 178,620 | 1.7% |
| FOR_ITER_RANGE | 1,794 | 0.0% |
| LOAD_ATTR_SLOT | 900 | 0.0% |
| ENTER_EXECUTOR | 300 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 320 | 72.7% |
| FOR_ITER | 80 | 18.2% |
| JUMP_BACKWARD | 40 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 120 | 27.3% |
| LOAD_FAST | 100 | 22.7% |
| FOR_ITER | 80 | 18.2% |
| FOR_ITER_LIST | 60 | 13.6% |
| STORE_FAST | 40 | 9.1% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 4,477,240 | 63.2% |
| BEFORE_ASYNC_WITH | 746,480 | 10.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 746,460 | 10.5% |
| LOAD_ATTR_INSTANCE_VALUE | 746,460 | 10.5% |
| LOAD_FAST | 372,300 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,088,980 | 100.0% |


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
| LOAD_CONST | 400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 400 | 100.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,479,220 | 99.9% |
| POP_JUMP_IF_FALSE | 2,454 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 4,479,160 | 99.9% |
| LOAD_FAST | 2,414 | 0.1% |
| FOR_ITER | 40 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |
| CALL_FUNCTION_EX | 20 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,982,160 | 100.0% |
| RESUME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 1,863,500 | 62.5% |
| SEND | 1,118,820 | 37.5% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,482,948 | 100.0% |
| POP_TOP | 100 | 0.0% |
| POP_JUMP_IF_FALSE | 80 | 0.0% |
| ENTER_EXECUTOR | 54 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,481,274 | 100.0% |
| LOAD_GLOBAL_BUILTIN | 1,868 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_FAST_CHECK | 20 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 372,300 | 99.6% |
| LOAD_ATTR_SLOT | 1,620 | 0.4% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 373,940 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,731,080 | 95.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,493,560 | 4.5% |
| LOAD_ATTR | 11,860 | 0.0% |
| LOAD_ATTR_SLOT | 1,440 | 0.0% |
| LOAD_GLOBAL_MODULE | 980 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,076,500 | 30.3% |
| CALL | 8,959,720 | 27.0% |
| LOAD_FAST | 4,852,420 | 14.6% |
| TO_BOOL_NONE | 4,478,920 | 13.5% |
| STORE_FAST | 3,732,640 | 11.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 21,642,900 | 21.4% |
| LOAD_FAST | 17,916,294 | 17.7% |
| LOAD_FAST_LOAD_FAST | 12,690,400 | 12.5% |
| POP_TOP | 11,570,354 | 11.4% |
| POP_JUMP_IF_FALSE | 10,827,168 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,797,654 | 41.3% |
| COMPARE_OP_INT | 11,946,034 | 11.8% |
| STORE_FAST | 11,204,730 | 11.1% |
| CALL_KW | 10,076,780 | 10.0% |
| SEND_GEN | 5,969,960 | 5.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 745,180 | 99.9% |
| LOAD_GLOBAL | 240 | 0.0% |
| STORE_FAST | 160 | 0.0% |
| NOP | 80 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 745,420 | 99.9% |
| LOAD_CONST | 160 | 0.0% |
| PUSH_NULL | 80 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 80 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 89,570,088 | 19.6% |
| POP_JUMP_IF_FALSE | 89,456,676 | 19.5% |
| STORE_FAST | 58,986,180 | 12.9% |
| LOAD_CONST | 41,797,654 | 9.1% |
| POP_TOP | 39,936,568 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 125,058,132 | 27.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 42,922,682 | 9.4% |
| LOAD_ATTR_SLOT | 42,502,974 | 9.3% |
| RETURN_VALUE | 37,891,374 | 8.3% |
| STORE_ATTR_SLOT | 33,209,454 | 7.3% |


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
| STORE_ATTR_SLOT | 31,347,180 | 29.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 18,288,000 | 16.9% |
| LOAD_FAST_LOAD_FAST | 15,300,660 | 14.2% |
| PUSH_NULL | 14,928,200 | 13.8% |
| POP_JUMP_IF_NOT_NONE | 10,076,700 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 42,168,420 | 39.1% |
| LOAD_FAST_LOAD_FAST | 15,300,660 | 14.2% |
| LOAD_CONST | 12,690,400 | 11.8% |
| LOAD_FAST | 10,449,480 | 9.7% |
| CALL | 10,449,200 | 9.7% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME | 600 | 13.0% |
| RESUME_CHECK | 580 | 12.6% |
| POP_TOP | 500 | 10.8% |
| LOAD_FAST | 500 | 10.8% |
| POP_JUMP_IF_FALSE | 460 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,580 | 34.2% |
| LOAD_ATTR | 960 | 20.8% |
| LOAD_GLOBAL_BUILTIN | 660 | 14.3% |
| LOAD_FAST | 400 | 8.7% |
| CALL | 300 | 6.5% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 460 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 220 | 47.8% |
| CALL | 140 | 30.4% |
| LOAD_FAST | 60 | 13.0% |
| LOAD_FAST_LOAD_FAST | 40 | 8.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60 | 75.0% |
| RESUME | 20 | 25.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 64,546,848 | 52.5% |
| TO_BOOL_NONE | 25,751,540 | 21.0% |
| COMPARE_OP_INT | 20,234,848 | 16.5% |
| TO_BOOL | 6,719,500 | 5.5% |
| TO_BOOL_LIST | 5,229,582 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,456,676 | 72.8% |
| RETURN_CONST | 16,047,360 | 13.1% |
| LOAD_CONST | 10,827,168 | 8.8% |
| LOAD_FAST_LOAD_FAST | 4,104,880 | 3.3% |
| LOAD_GLOBAL_MODULE | 2,236,114 | 1.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,211,840 | 61.1% |
| LOAD_ATTR_INSTANCE_VALUE | 5,225,580 | 38.9% |
| CALL | 160 | 0.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,690,400 | 94.4% |
| LOAD_CONST | 746,480 | 5.6% |
| RETURN_CONST | 480 | 0.0% |
| LOAD_GLOBAL | 100 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 100 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,886,314 | 78.0% |
| LOAD_ATTR_INSTANCE_VALUE | 6,718,340 | 22.0% |
| LOAD_GLOBAL_MODULE | 220 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,076,700 | 32.9% |
| LOAD_GLOBAL_MODULE | 9,330,500 | 30.5% |
| LOAD_FAST | 5,972,054 | 19.5% |
| RETURN_CONST | 4,478,880 | 14.6% |
| LOAD_CONST | 746,500 | 2.4% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,970,560 | 57.1% |
| TO_BOOL | 4,480,974 | 42.9% |
| TO_BOOL_INT | 1,874 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,076,960 | 96.4% |
| LOAD_CONST | 374,214 | 3.6% |
| STORE_FAST | 1,834 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 100 | 0.0% |
| POP_TOP | 80 | 0.0% |


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
| POP_JUMP_IF_FALSE | 16,047,360 | 27.9% |
| POP_TOP | 14,554,940 | 25.3% |
| STORE_ATTR_SLOT | 11,193,840 | 19.5% |
| STORE_FAST | 10,450,834 | 18.2% |
| POP_JUMP_IF_NOT_NONE | 4,478,880 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 28,737,900 | 50.0% |
| POP_TOP | 26,872,668 | 46.8% |
| END_SEND | 1,118,940 | 1.9% |
| EXIT_INIT_CHECK | 746,460 | 1.3% |
| TO_BOOL | 40 | 0.0% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,119,020 | 50.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 1,118,820 | 50.0% |
| SEND | 940 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 1,118,780 | 50.0% |
| YIELD_VALUE | 1,118,780 | 50.0% |
| SEND | 940 | 0.0% |
| POP_TOP | 140 | 0.0% |
| SEND_GEN | 140 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 240 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,860 | 77.3% |
| LOAD_FAST_LOAD_FAST | 340 | 9.2% |
| LOAD_ATTR_INSTANCE_VALUE | 280 | 7.6% |
| STORE_ATTR | 100 | 2.7% |
| SWAP | 80 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 1,280 | 34.6% |
| LOAD_FAST | 620 | 16.8% |
| LOAD_CONST | 520 | 14.1% |
| RETURN_CONST | 520 | 14.1% |
| STORE_ATTR_SLOT | 340 | 9.2% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 20,152,320 | 23.0% |
| RETURN_VALUE | 19,035,214 | 21.8% |
| CALL_BUILTIN_O | 15,752,234 | 18.0% |
| LOAD_CONST | 11,204,730 | 12.8% |
| FOR_ITER_RANGE | 4,480,954 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 58,986,180 | 67.5% |
| RETURN_CONST | 10,450,834 | 12.0% |
| LOAD_FAST_LOAD_FAST | 8,659,540 | 9.9% |
| JUMP_FORWARD | 4,482,948 | 5.1% |
| LOAD_GLOBAL_MODULE | 3,732,640 | 4.3% |


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
| UNPACK_SEQUENCE_TWO_TUPLE | 120 | 75.0% |
| UNPACK_SEQUENCE | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 50.0% |
| LOAD_GLOBAL | 40 | 25.0% |
| LOAD_GLOBAL_MODULE | 40 | 25.0% |


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
| LOAD_ATTR | 80 | 23.5% |
| LOAD_FAST | 80 | 23.5% |
| BINARY_OP_ADD_INT | 60 | 17.6% |
| BINARY_OP_SUBTRACT_INT | 60 | 17.6% |
| BINARY_OP | 40 | 11.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 100 | 29.4% |
| STORE_ATTR | 80 | 23.5% |
| STORE_FAST | 80 | 23.5% |
| STORE_ATTR_INSTANCE_VALUE | 80 | 23.5% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 33.3% |
| CALL | 40 | 33.3% |
| STORE_FAST | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 60 | 50.0% |
| STORE_FAST_STORE_FAST | 40 | 33.3% |
| LOAD_FAST | 20 | 16.7% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 1,863,540 | 62.5% |
| SEND | 1,118,780 | 37.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 1,863,540 | 62.5% |
| INTERPRETER_EXIT | 1,118,780 | 37.5% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,160 | 56.9% |
| CACHE | 340 | 16.7% |
| COPY_FREE_VARS | 240 | 11.8% |
| POP_TOP | 160 | 7.8% |
| SEND_GEN | 100 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 960 | 47.1% |
| LOAD_GLOBAL | 600 | 29.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 160 | 7.8% |
| LOAD_CONST | 140 | 6.9% |
| NOP | 100 | 4.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 372,260 | 99.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,794 | 0.5% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 372,280 | 99.5% |
| STORE_FAST | 1,814 | 0.5% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,732,480 | 50.0% |
| RETURN_VALUE | 3,732,440 | 50.0% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,732,460 | 50.0% |
| CALL_PY_WITH_DEFAULTS | 3,732,440 | 50.0% |
| SWAP | 60 | 0.0% |
| CALL | 20 | 0.0% |


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
| LOAD_CONST | 4,478,880 | 54.5% |
| LOAD_FAST_LOAD_FAST | 3,732,440 | 45.5% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,478,840 | 54.5% |
| STORE_FAST | 3,732,460 | 45.5% |
| SWAP | 60 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 80 | 57.1% |
| LOAD_FAST | 40 | 28.6% |
| BINARY_SUBSCR | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 80 | 57.1% |
| RETURN_VALUE | 60 | 42.9% |


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
| LOAD_CONST | 548 | 93.2% |
| BINARY_SUBSCR | 40 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 454 | 77.2% |
| LOAD_ATTR_SLOT | 114 | 19.4% |
| LOAD_ATTR | 20 | 3.4% |


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
| PUSH_NULL | 746,440 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 746,460 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,478,880 | 99.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,340 | 0.3% |
| CALL | 60 | 0.0% |
| PUSH_NULL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,732,460 | 83.1% |
| GET_AWAITABLE | 746,460 | 16.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,340 | 0.3% |
| RETURN_GENERATOR | 60 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 746,660 | 49.9% |
| LOAD_GLOBAL_MODULE | 746,440 | 49.9% |
| LOAD_FAST | 1,974 | 0.1% |
| CALL | 180 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 748,334 | 50.0% |
| LOAD_FAST | 746,700 | 49.9% |
| COMPARE_OP | 140 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 372,260 | 99.9% |
| LOAD_CONST | 180 | 0.0% |
| CALL | 60 | 0.0% |
| LOAD_FAST_LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 372,280 | 99.9% |
| COPY | 140 | 0.0% |
| TO_BOOL_BOOL | 80 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 746,440 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 746,460 | 100.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,123,980 | 100.0% |
| LOAD_ATTR_INSTANCE_VALUE | 434 | 0.0% |
| CALL | 180 | 0.0% |
| LOAD_CONST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 15,752,234 | 97.7% |
| TO_BOOL_BOOL | 372,260 | 2.3% |
| POP_TOP | 120 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,458,720 | 100.0% |
| LOAD_GLOBAL_BUILTIN | 380 | 0.0% |
| CALL | 80 | 0.0% |
| BUILD_TUPLE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,459,140 | 100.0% |
| TO_BOOL | 80 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,382 | 98.9% |
| CALL | 60 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,628 | 66.7% |
| COPY | 1,814 | 33.3% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,361,940 | 100.0% |
| LOAD_FAST_LOAD_FAST | 120 | 0.0% |
| CALL | 60 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,359,540 | 99.9% |
| TO_BOOL_NONE | 2,400 | 0.1% |
| RETURN_VALUE | 140 | 0.0% |
| STORE_FAST | 60 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,794 | 89.1% |
| LOAD_CONST | 80 | 4.0% |
| CALL | 60 | 3.0% |
| LOAD_ATTR | 40 | 2.0% |
| LOAD_FAST | 40 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,814 | 90.1% |
| POP_TOP | 120 | 6.0% |
| RETURN_VALUE | 80 | 4.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 10,076,500 | 73.0% |
| LOAD_ATTR_METHOD_NO_DICT | 3,734,954 | 27.0% |
| CALL | 400 | 0.0% |
| LOAD_FAST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 10,076,460 | 73.0% |
| STORE_FAST | 3,734,554 | 27.0% |
| POP_TOP | 380 | 0.0% |
| GET_ITER | 160 | 0.0% |
| CALL | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,513,694 | 84.0% |
| CALL | 4,479,100 | 16.0% |
| LOAD_CONST | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 27,992,874 | 100.0% |
| LOAD_CONST | 20 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 31,349,468 | 61.3% |
| LOAD_FAST | 14,186,108 | 27.7% |
| BINARY_OP_SUBTRACT_INT | 4,478,840 | 8.8% |
| LOAD_ATTR_METHOD_NO_DICT | 373,380 | 0.7% |
| LOAD_SUPER_ATTR_METHOD | 372,460 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,178,216 | 82.5% |
| RETURN_GENERATOR | 8,583,660 | 16.8% |
| COPY_FREE_VARS | 372,920 | 0.7% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 3,732,440 | 90.9% |
| LOAD_GLOBAL_MODULE | 372,260 | 9.1% |
| CALL | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,732,840 | 90.9% |
| RETURN_GENERATOR | 372,280 | 9.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| CALL | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 40 | 66.7% |
| LOAD_GLOBAL | 20 | 33.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 4,458,680 | 100.0% |
| LOAD_FAST | 434 | 0.0% |
| LOAD_GLOBAL_MODULE | 114 | 0.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,458,700 | 100.0% |
| POP_JUMP_IF_FALSE | 588 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,946,034 | 59.0% |
| LOAD_FAST_LOAD_FAST | 4,554,360 | 22.5% |
| LOAD_GLOBAL_MODULE | 3,734,234 | 18.5% |
| COMPARE_OP | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,234,848 | 100.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20 | 100.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 3,628 | 98.4% |
| FOR_ITER | 60 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,874 | 50.8% |
| LOAD_FAST | 1,814 | 49.2% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 4,479,160 | 85.7% |
| GET_ITER | 748,274 | 14.3% |
| ENTER_EXECUTOR | 1,794 | 0.0% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,480,954 | 85.7% |
| LOAD_CONST | 748,314 | 14.3% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 20 | 50.0% |
| ENTER_EXECUTOR | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20 | 50.0% |
| STORE_FAST | 20 | 50.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 85.7% |
| LOAD_ATTR | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 125,058,132 | 96.5% |
| LOAD_FAST_LOAD_FAST | 4,479,120 | 3.5% |
| LOAD_ATTR | 1,980 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 0.0% |
| COPY | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 40,309,134 | 31.1% |
| LOAD_ATTR_METHOD_NO_DICT | 31,359,122 | 24.2% |
| RETURN_VALUE | 16,419,540 | 12.7% |
| TO_BOOL | 11,199,394 | 8.6% |
| POP_JUMP_IF_NOT_NONE | 6,718,340 | 5.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 31,359,122 | 88.4% |
| LOAD_FAST | 4,105,760 | 11.6% |
| LOAD_ATTR | 620 | 0.0% |
| ENTER_EXECUTOR | 300 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,875,934 | 75.8% |
| LOAD_GLOBAL_MODULE | 4,478,960 | 12.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 3,734,954 | 10.5% |
| CALL_PY_EXACT_ARGS | 373,380 | 1.1% |
| LOAD_FAST_LOAD_FAST | 1,954 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,922,682 | 68.0% |
| LOAD_ATTR_SLOT | 11,193,640 | 17.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,227,394 | 8.3% |
| LOAD_FAST_LOAD_FAST | 3,732,480 | 5.9% |
| LOAD_ATTR | 1,260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 31,349,468 | 49.7% |
| LOAD_FAST_LOAD_FAST | 18,288,000 | 29.0% |
| LOAD_FAST | 13,439,308 | 21.3% |
| CALL | 700 | 0.0% |
| LOAD_CONST | 120 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 24,627,868 | 100.0% |
| LOAD_ATTR | 980 | 0.0% |
| LOAD_FAST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 24,256,008 | 98.5% |
| LOAD_FAST_LOAD_FAST | 372,280 | 1.5% |
| LOAD_ATTR | 200 | 0.0% |
| LOAD_FAST | 120 | 0.0% |
| LOAD_ATTR_SLOT | 80 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| LOAD_ATTR | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,502,974 | 100.0% |
| LOAD_ATTR_SLOT | 12,680 | 0.0% |
| ENTER_EXECUTOR | 900 | 0.0% |
| LOAD_ATTR | 480 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 114 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 21,270,100 | 50.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 11,193,640 | 26.3% |
| LOAD_FAST | 4,459,154 | 10.5% |
| COMPARE_OP_FLOAT | 4,458,680 | 10.5% |
| TO_BOOL_BOOL | 1,117,674 | 2.6% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,833,814 | 72.1% |
| STORE_FAST | 748,294 | 11.2% |
| STORE_ATTR_INSTANCE_VALUE | 746,580 | 11.1% |
| POP_TOP | 372,460 | 5.6% |
| JUMP_FORWARD | 1,868 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,467,256 | 66.6% |
| CALL_BUILTIN_CLASS | 746,660 | 11.1% |
| LOAD_GLOBAL_MODULE | 746,480 | 11.1% |
| LOAD_DEREF | 745,180 | 11.1% |
| CALL_ISINSTANCE | 380 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 19,407,254 | 39.1% |
| POP_JUMP_IF_NOT_NONE | 9,330,500 | 18.8% |
| LOAD_FAST | 8,565,414 | 17.3% |
| LOAD_ATTR_METHOD_NO_DICT | 4,478,960 | 9.0% |
| STORE_FAST | 3,732,640 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 24,627,868 | 49.6% |
| LOAD_FAST | 11,197,900 | 22.6% |
| LOAD_FAST_LOAD_FAST | 4,479,200 | 9.0% |
| CALL_ISINSTANCE | 4,458,720 | 9.0% |
| COMPARE_OP_INT | 3,734,234 | 7.5% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 744,960 | 100.0% |
| LOAD_SUPER_ATTR | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 372,460 | 50.0% |
| LOAD_FAST_LOAD_FAST | 372,340 | 50.0% |
| LOAD_FAST | 260 | 0.0% |
| CALL | 120 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 45,510,580 | 38.5% |
| CALL_PY_EXACT_ARGS | 42,178,216 | 35.7% |
| POP_TOP | 10,449,000 | 8.8% |
| CALL | 4,851,840 | 4.1% |
| CALL_KW | 4,478,940 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,570,088 | 75.7% |
| LOAD_GLOBAL_MODULE | 19,407,254 | 16.4% |
| LOAD_GLOBAL_BUILTIN | 4,833,814 | 4.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 2,982,160 | 2.5% |
| LOAD_CONST | 1,493,380 | 1.3% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,969,960 | 76.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 1,863,500 | 23.8% |
| SEND | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,970,060 | 76.2% |
| RESUME_CHECK | 1,863,440 | 23.8% |
| RESUME | 100 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,945,020 | 100.0% |
| STORE_ATTR | 1,280 | 0.0% |
| LOAD_FAST_LOAD_FAST | 260 | 0.0% |
| SWAP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,226,060 | 43.7% |
| LOAD_FAST | 2,986,600 | 25.0% |
| RETURN_CONST | 747,120 | 6.3% |
| LOAD_GLOBAL_MODULE | 746,800 | 6.3% |
| BUILD_LIST | 746,680 | 6.3% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 42,168,420 | 55.9% |
| LOAD_FAST | 33,209,454 | 44.0% |
| STORE_ATTR_SLOT | 88,480 | 0.1% |
| STORE_ATTR | 340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 31,347,180 | 41.5% |
| LOAD_CONST | 21,642,900 | 28.7% |
| LOAD_FAST | 11,194,294 | 14.8% |
| RETURN_CONST | 11,193,840 | 14.8% |
| STORE_ATTR_SLOT | 88,480 | 0.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,760 | 95.7% |
| STORE_SUBSCR | 40 | 2.2% |
| LOAD_ATTR | 40 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,840 | 100.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,309,134 | 57.2% |
| RETURN_VALUE | 10,821,860 | 15.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,076,460 | 14.3% |
| CALL_ISINSTANCE | 4,459,140 | 6.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,359,540 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 64,546,848 | 91.5% |
| POP_JUMP_IF_TRUE | 5,970,560 | 8.5% |
| UNARY_NOT | 60 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,874 | 85.4% |
| TO_BOOL | 160 | 7.3% |
| LOAD_FAST | 80 | 3.6% |
| BINARY_OP | 40 | 1.8% |
| LOAD_ATTR_SLOT | 40 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,874 | 85.4% |
| POP_JUMP_IF_FALSE | 260 | 11.9% |
| UNARY_NOT | 60 | 2.7% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,229,482 | 100.0% |
| TO_BOOL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,229,582 | 100.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 21,270,100 | 82.6% |
| LOAD_ATTR | 4,478,920 | 17.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,400 | 0.0% |
| TO_BOOL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 25,751,540 | 100.0% |
| TO_BOOL_BOOL | 20 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE | 60 | 33.3% |
| RETURN_VALUE | 40 | 22.2% |
| CALL | 40 | 22.2% |
| STORE_FAST | 40 | 22.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 120 | 66.7% |
| LOAD_FAST | 60 | 33.3% |


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
|     deferred | 814 | 0.0% |
|          hit | 16,050,514 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 52.9% |
| Failure | 160 | 47.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 80 | 50.0% |
| or | 40 | 25.0% |
| true divide other | 40 | 25.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 6.3% |
|          hit | 828 | 87.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 36,952,734 | 21.9% |
|          hit | 131,823,868 | 78.1% |
|         miss | 761,180 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 17,460 | 58.9% |
| Failure | 12,160 | 41.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 3,280 | 27.0% |
| no dict | 2,960 | 24.3% |
| code complex parameters | 1,620 | 13.3% |
| cfunc noargs | 1,380 | 11.3% |
| class no vectorcall | 1,340 | 11.0% |
| other | 1,280 | 10.5% |
| class mutable | 80 | 0.7% |
| metaclass | 60 | 0.5% |
| wrong number arguments | 40 | 0.3% |
| cfunc varargs | 40 | 0.3% |
| operator wrapper | 40 | 0.3% |
| cmethod | 20 | 0.2% |
| cfunc varargs keywords | 20 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 372,800 | 1.5% |
|          hit | 24,694,156 | 98.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 46.7% |
| Failure | 320 | 53.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 280 | 87.5% |
| bool | 40 | 12.5% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 260 | 0.0% |
|          hit | 5,232,996 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 55.6% |
| Failure | 80 | 44.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 80 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 33,886,340 | 10.3% |
|          hit | 294,554,886 | 89.7% |
|         miss | 674,600 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 18,040 | 62.2% |
| Failure | 10,980 | 37.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 6,560 | 59.7% |
| method | 2,900 | 26.4% |
| class attr descriptor | 1,280 | 11.7% |
| not managed dict | 140 | 1.3% |
| metaclass attribute | 60 | 0.5% |
| class attr simple | 40 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,460 | 0.0% |
|        deopt | 80 | 0.0% |
|          hit | 56,325,452 | 100.0% |
|         miss | 80 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,240 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 745,180 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 100.0% |
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
|     deferred | 2,237,700 | 22.2% |
|          hit | 7,833,600 | 77.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 13.0% |
| Failure | 940 | 87.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 940 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,607,380 | 5.3% |
|          hit | 82,719,454 | 94.6% |
|         miss | 4,693,880 | 5.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 90,100 | 99.9% |
| Failure | 100 | 0.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| overridden | 80 | 80.0% |
| overriding descriptor | 20 | 20.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 3.1% |
|          hit | 1,840 | 94.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,201,974 | 9.9% |
|          hit | 101,499,324 | 90.1% |
|         miss | 1,480 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,400 | 26.9% |
| Failure | 3,800 | 73.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| set | 3,700 | 97.4% |
| sequence | 100 | 2.6% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 20.0% |
|          hit | 180 | 60.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 1,136,832,796 | 50.8% |
| Not specialized | 260,642,970 | 11.6% |
| Specialized hits | 836,008,100 | 37.3% |
| Specialized misses | 6,162,054 | 0.3% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 36,952,734 | 41.4% |
| LOAD_ATTR | 33,886,340 | 38.0% |
| TO_BOOL | 11,201,974 | 12.5% |
| STORE_ATTR | 4,607,380 | 5.2% |
| SEND | 2,237,700 | 2.5% |
| COMPARE_OP | 372,800 | 0.4% |
| LOAD_GLOBAL | 2,460 | 0.0% |
| BINARY_OP | 814 | 0.0% |
| FOR_ITER | 260 | 0.0% |
| LOAD_SUPER_ATTR | 240 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 4,693,880 | 75.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 760,800 | 12.3% |
| LOAD_ATTR_SLOT | 674,000 | 10.9% |
| RESUME | 30,834 | 0.5% |
| RESUME_CHECK | 30,834 | 0.5% |
| TO_BOOL_NONE | 1,060 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 600 | 0.0% |
| TO_BOOL_BOOL | 420 | 0.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 260 | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 120 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 51,855,320 | 40.3% |
| Calls to Python functions inlined | 76,885,056 | 59.7% |
| Calls via PyEval_EvalFrame (total) | 51,855,320 | 40.3% |
| Calls via PyEval_EvalFrame (vector) | 46,257,580 | 35.9% |
| Calls via PyEval_EvalFrame (generator) | 5,597,740 | 4.3% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 46,257,580 | 35.9% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 4,458,720 | 3.5% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 4,479,100 | 3.5% |
| Calls via PyEval_EvalFrame (method) | 20,153,400 | 15.7% |
| Frame objects created | 180 | 0.0% |
| Frames pushed | 70,913,396 | 55.1% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 56,534,624 | 34.8% |
| Frees to freelist | 56,875,250 |  |
| Allocations | 105,708,369 | 65.2% |
| Allocations to 512 bytes | 104,899,702 | 64.7% |
| Allocations to 4 kbytes | 808,539 | 0.5% |
| Allocations over 4 kbytes | 128 | 0.0% |
| Frees | 105,623,302 |  |
| New values | 440 |  |
| Interpreter increfs | 1,286,142,812 | 79.3% |
| Interpreter decrefs | 1,357,843,598 | 77.0% |
| Increfs | 336,285,247 | 20.7% |
| Decrefs | 406,630,109 | 23.0% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 70,696,813 |  |
| Method cache misses | 4,321 |  |
| Method cache collisions | 4,117 |  |
| Method cache dunder hits | 16,402,089 |  |
| Method cache dunder misses | 491 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 55,354 | 2,040 | 379,772,656 |
| 1 | 5,020 | 0 | 392,014,132 |
| 2 | 446 | 0 | 995,659,196 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 2,400 |  |
| Traces created | 2,480 | 103.3% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 5,600 | 233.3% |
| Trace too long | 0 | 0.0% |
| Trace too short | 332,080 | 13,836.7% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 2,300 | 95.8% |
| Low confidence | 0 | 0.0% |
| Traces executed | 22,793,242 |  |
| Uops executed | 695,817,820 | 30.53 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 20 | 0.8% |
| <= 32 | 80 | 3.2% |
| <= 64 | 2,340 | 94.4% |
| <= 128 | 40 | 1.6% |


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
| <= 32 | 0 | 0.0% |
| <= 64 | 0 | 0.0% |
| <= 128 | 0 | 0.0% |
| <= 256 | 0 | 0.0% |
| <= 512 | 60 | 2.4% |
| <= 1,024 | 40 | 1.6% |
| <= 2,048 | 40 | 1.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 1,814 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 1,714,960 | 7.5% |
| <= 32 | 372,300 | 1.6% |
| <= 64 | 10,076,260 | 44.2% |
| <= 128 | 0 | 0.0% |
| <= 256 | 0 | 0.0% |
| <= 512 | 0 | 0.0% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 0 | 0.0% |
| <= 16,384 | 0 | 0.0% |
| <= 32,768 | 0 | 0.0% |
| <= 65,536 | 0 | 0.0% |
| <= 131,072 | 74 | 0.0% |
| <= 262,144 | 80 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _GUARD_TYPE_VERSION | 86,183,088 | 12.4% | 12.4% | 1.7% |
| LOAD_FAST | 77,201,782 | 11.1% | 23.5% |  |
| _SET_IP | 65,748,304 | 9.4% | 32.9% |  |
| _CHECK_VALIDITY | 65,374,510 | 9.4% | 42.3% |  |
| _LOAD_ATTR_SLOT | 41,046,366 | 5.9% | 48.2% |  |
| _CHECK_VALIDITY_AND_SET_IP | 32,084,706 | 4.6% | 52.8% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 22,382,524 | 3.2% | 56.1% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 22,382,524 | 3.2% | 59.3% |  |
| STORE_FAST | 21,866,258 | 3.1% | 62.4% |  |
| _GUARD_IS_FALSE_POP | 21,497,180 | 3.1% | 65.5% | 0.2% |
| TO_BOOL_BOOL | 20,896,520 | 3.0% | 68.5% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 20,894,972 | 3.0% | 71.5% |  |
| _START_EXECUTOR | 12,165,488 | 1.7% | 73.3% |  |
| _LOAD_ATTR | 11,935,534 | 1.7% | 75.0% |  |
| PUSH_NULL | 11,048,246 | 1.6% | 76.6% |  |
| _COLD_EXIT | 10,627,754 | 1.5% | 78.1% |  |
| _EXIT_TRACE | 10,626,000 | 1.5% | 79.6% | 100.0% |
| _GUARD_NOT_EXHAUSTED_RANGE | 10,448,680 | 1.5% | 81.1% | 0.0% |
| _ITER_CHECK_RANGE | 10,448,680 | 1.5% | 82.6% |  |
| RESUME_CHECK | 10,447,960 | 1.5% | 84.1% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 10,447,960 | 1.5% | 85.6% |  |
| _CHECK_STACK_SPACE | 10,447,960 | 1.5% | 87.1% |  |
| _INIT_CALL_PY_EXACT_ARGS | 10,447,960 | 1.5% | 88.6% |  |
| _PUSH_FRAME | 10,447,960 | 1.5% | 90.1% |  |
| _SAVE_RETURN_OFFSET | 10,447,960 | 1.5% | 91.6% |  |
| BUILD_LIST | 10,447,360 | 1.5% | 93.1% |  |
| CALL_INTRINSIC_1 | 10,447,360 | 1.5% | 94.6% |  |
| LIST_EXTEND | 10,447,360 | 1.5% | 96.1% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,446,886 | 1.5% | 97.6% |  |
| _ITER_NEXT_RANGE | 10,446,886 | 1.5% | 99.1% |  |
| _LOAD_CONST_INLINE_BORROW | 743,726 | 0.1% | 99.2% |  |
| CALL_BUILTIN_O | 600,586 | 0.1% | 99.3% |  |
| BINARY_SUBSCR_LIST_INT | 371,900 | 0.1% | 99.4% |  |
| COMPARE_OP_FLOAT | 371,900 | 0.1% | 99.4% |  |
| _GUARD_IS_TRUE_POP | 371,826 | 0.1% | 99.5% | 0.0% |
| POP_TOP | 371,826 | 0.1% | 99.5% |  |
| CALL_METHOD_DESCRIPTOR_O | 371,826 | 0.1% | 99.6% |  |
| TO_BOOL_LIST | 371,826 | 0.1% | 99.6% |  |
| _CHECK_ATTR_MODULE | 371,826 | 0.1% | 99.7% |  |
| _LOAD_ATTR_MODULE | 371,826 | 0.1% | 99.8% |  |
| _STORE_ATTR_SLOT | 371,826 | 0.1% | 99.8% |  |
| _LOAD_CONST_INLINE | 371,826 | 0.1% | 99.9% |  |
| _CHECK_GLOBALS | 371,826 | 0.1% | 99.9% |  |
| _JUMP_TO_TOP | 371,746 | 0.1% | 100.0% |  |
| COMPARE_OP_INT | 228,760 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 20 | 0.0% | 100.0% | 100.0% |
| _ITER_CHECK_TUPLE | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL_FUNCTION_EX | 326,600 |


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set class | 0 |
| set bases | 0 |
| set eval frame func | 0 |
| builtin dict | 0 |
| func modification | 0 |
| watched dict modification | 0 |
| watched globals modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-14
